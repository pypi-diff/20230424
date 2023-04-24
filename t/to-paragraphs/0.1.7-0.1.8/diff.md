# Comparing `tmp/to_paragraphs-0.1.7.tar.gz` & `tmp/to_paragraphs-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_paragraphs-0.1.7.tar", max compression
+gzip compressed data, was "to_paragraphs-0.1.8.tar", max compression
```

## Comparing `to_paragraphs-0.1.7.tar` & `to_paragraphs-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2731 2023-04-23 22:55:23.561355 to_paragraphs-0.1.7/README.md
--rw-r--r--   0        0        0      385 2023-04-23 23:22:32.971776 to_paragraphs-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       40 2023-04-23 23:21:55.376793 to_paragraphs-0.1.7/to_paragraphs/__init__.py
--rw-r--r--   0        0        0     2395 2023-04-23 22:46:21.402761 to_paragraphs-0.1.7/to_paragraphs/to_paragraphs.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 to_paragraphs-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2810 2023-04-24 09:28:34.303214 to_paragraphs-0.1.8/README.md
+-rw-r--r--   0        0        0      489 2023-04-24 10:07:28.861243 to_paragraphs-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-04-23 23:21:55.376793 to_paragraphs-0.1.8/to_paragraphs/__init__.py
+-rw-r--r--   0        0        0     1961 2023-04-24 10:00:03.989991 to_paragraphs-0.1.8/to_paragraphs/to_paragraphs.py
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 to_paragraphs-0.1.8/PKG-INFO
```

### Comparing `to_paragraphs-0.1.7/README.md` & `to_paragraphs-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # to_paragraphs
 
+> Note, the code is currently ~slow and messy. It's a work in progress.
+
 Extracts paragraphs from a string, using the semantic similarity between sentences to determine paragraph boundaries.
 This tends to work better than the naive approach of splitting on newlines.
 
 ## Installation
 
 ```bash
 pip install to_paragraphs
@@ -32,30 +34,30 @@
 ```
 
 ### Example embedding function
 
 ```python
 import torch
 import torch.nn.functional as F
-import numpy as np
 from transformers import AutoTokenizer, AutoModel
 
+CACHE_PATH = '/tmp/transformers'
+TOKENIZER = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
+MODEL = AutoModel.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
+
 
 def mean_pooling(model_output, attention_mask):
     token_embeddings = model_output[0]  # First element of model_output contains all token embeddings
     input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
     return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
 
 def embed(sentences):
-    tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
-    model = AutoModel.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
-
-    encoded_input = tokenizer(sentences, padding=True, truncation=True, return_tensors='pt')
+    encoded_input = TOKENIZER(sentences, padding=True, truncation=True, return_tensors='pt')
 
     with torch.no_grad():
-        model_output = model(**encoded_input)
+        model_output = MODEL(**encoded_input)
 
     sentence_embeddings = mean_pooling(model_output, encoded_input['attention_mask'])
 
     return F.normalize(sentence_embeddings, p=2, dim=1)
 ```
```

### Comparing `to_paragraphs-0.1.7/to_paragraphs/to_paragraphs.py` & `to_paragraphs-0.1.8/to_paragraphs/to_paragraphs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,26 @@
 
 import numpy as np
 from nltk import tokenize
 from scipy.signal import argrelextrema
 
 
 def _activate_text_similarities(similarities, paragraph_size: int) -> np.ndarray:
-    x = np.linspace(-10, 10, paragraph_size)
-    ys = 1 / (1 + np.exp(0.5 * x))
+    xs = np.linspace(-10, 10, paragraph_size)
+    ys = 1 / (1 + np.exp(0.5 * xs))
+    activation_weights = ys.reshape(1, -1)
+
+    diagonals = np.zeros_like(similarities)
+    for k in range(similarities.shape[0]):
+        diag = np.diag(similarities, k)
+        diagonals[k:k + diag.shape[0], k] = diag.reshape(-1)
 
-    diagonals = np.array([
-        np.pad(
-            np.diag(similarities, k),
-            (0, similarities.shape[0] - np.diag(similarities, k).size)
-        ) for k in range(similarities.shape[0])
-    ])
+    activated_similarities = diagonals * activation_weights
 
-    activation_weights = np.pad(ys, (0, similarities.shape[0] - paragraph_size))
-
-    activated_similarities = diagonals * activation_weights.reshape(-1, 1)
-
-    activated_similarities = np.sum(activated_similarities, axis=0)
-
-    return activated_similarities
+    return np.sum(activated_similarities, axis=1)
 
 
 def cosine_similarity(embeddings: np.ndarray) -> np.ndarray:
     norm = np.linalg.norm(embeddings, axis=1)
     normalized_embeddings = embeddings / norm.reshape(-1, 1)
 
     return np.dot(normalized_embeddings, normalized_embeddings.T)
@@ -48,23 +43,15 @@
 
     # Activate the similarities to create paragraph boundaries.
     paragraph_boundaries = _activate_text_similarities(similarities, len(sentences))
 
     # Identify the split points where paragraphs end and new ones begin.
     split_points = argrelextrema(paragraph_boundaries, np.less, order=2)[0]
 
-    # Group the sentences into paragraphs.
-    paragraphs = [[]]
-    current_paragraph_index = 0
-
-    for sentence_index, sentence in enumerate(sentences):
-        # Add the current sentence to the current paragraph.
-        paragraphs[current_paragraph_index].append(sentence)
-
-        # Check if the current sentence is a split point.
-        if sentence_index in split_points:
-            # If it is, start a new paragraph.
-            current_paragraph_index += 1
-            paragraphs.append([])
+    last_split_point = 0
+
+    for split_point in split_points:
+        yield " ".join(sentences[last_split_point:split_point])
+        last_split_point = split_point
 
-    # Return the resulting list of paragraphs.
-    return paragraphs
+    if last_split_point < len(sentences):
+        yield " ".join(sentences[last_split_point:])
```

### Comparing `to_paragraphs-0.1.7/PKG-INFO` & `to_paragraphs-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: to-paragraphs
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 License: GPL-3.0
 Author: Félix Dorn
 Author-email: github@felixdorn.fr
-Requires-Python: >=3.9
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # to_paragraphs
 
+> Note, the code is currently ~slow and messy. It's a work in progress.
+
 Extracts paragraphs from a string, using the semantic similarity between sentences to determine paragraph boundaries.
 This tends to work better than the naive approach of splitting on newlines.
 
 ## Installation
 
 ```bash
 pip install to_paragraphs
@@ -50,31 +53,31 @@
 ```
 
 ### Example embedding function
 
 ```python
 import torch
 import torch.nn.functional as F
-import numpy as np
 from transformers import AutoTokenizer, AutoModel
 
+CACHE_PATH = '/tmp/transformers'
+TOKENIZER = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
+MODEL = AutoModel.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
+
 
 def mean_pooling(model_output, attention_mask):
     token_embeddings = model_output[0]  # First element of model_output contains all token embeddings
     input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
     return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
 
 def embed(sentences):
-    tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
-    model = AutoModel.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', cache_dir=CACHE_PATH)
-
-    encoded_input = tokenizer(sentences, padding=True, truncation=True, return_tensors='pt')
+    encoded_input = TOKENIZER(sentences, padding=True, truncation=True, return_tensors='pt')
 
     with torch.no_grad():
-        model_output = model(**encoded_input)
+        model_output = MODEL(**encoded_input)
 
     sentence_embeddings = mean_pooling(model_output, encoded_input['attention_mask'])
 
     return F.normalize(sentence_embeddings, p=2, dim=1)
 ```
```

