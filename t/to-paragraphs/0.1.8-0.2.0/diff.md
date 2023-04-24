# Comparing `tmp/to_paragraphs-0.1.8.tar.gz` & `tmp/to_paragraphs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_paragraphs-0.1.8.tar", max compression
+gzip compressed data, was "to_paragraphs-0.2.0.tar", max compression
```

## Comparing `to_paragraphs-0.1.8.tar` & `to_paragraphs-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2810 2023-04-24 09:28:34.303214 to_paragraphs-0.1.8/README.md
--rw-r--r--   0        0        0      489 2023-04-24 10:07:28.861243 to_paragraphs-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       40 2023-04-23 23:21:55.376793 to_paragraphs-0.1.8/to_paragraphs/__init__.py
--rw-r--r--   0        0        0     1961 2023-04-24 10:00:03.989991 to_paragraphs-0.1.8/to_paragraphs/to_paragraphs.py
--rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 to_paragraphs-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2810 2023-04-24 09:28:34.303214 to_paragraphs-0.2.0/README.md
+-rw-r--r--   0        0        0      489 2023-04-24 11:41:36.539205 to_paragraphs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-04-23 23:21:55.376793 to_paragraphs-0.2.0/to_paragraphs/__init__.py
+-rw-r--r--   0        0        0     2006 2023-04-24 11:41:07.147931 to_paragraphs-0.2.0/to_paragraphs/to_paragraphs.py
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 to_paragraphs-0.2.0/PKG-INFO
```

### Comparing `to_paragraphs-0.1.8/README.md` & `to_paragraphs-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `to_paragraphs-0.1.8/to_paragraphs/to_paragraphs.py` & `to_paragraphs-0.2.0/to_paragraphs/to_paragraphs.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,35 +23,38 @@
 def cosine_similarity(embeddings: np.ndarray) -> np.ndarray:
     norm = np.linalg.norm(embeddings, axis=1)
     normalized_embeddings = embeddings / norm.reshape(-1, 1)
 
     return np.dot(normalized_embeddings, normalized_embeddings.T)
 
 
-def to_paragraphs(content: str, embed_fn: Callable[[str], Any]) -> List[List[str]]:
+async def to_paragraphs(content: str, embed_fn: Callable[[str], Any]) -> List[List[str]]:
     # Tokenize the content into individual sentences.
     sentences = tokenize.sent_tokenize(content)
 
     # If no sentences are found, return an empty list.
     if len(sentences) == 0:
         return []
 
-    # Calculate the sentence embeddings for all the sentences.
-    embeddings = embed_fn(sentences)
+    loop = asyncio.get_event_loop()
+    embeddings = await loop.run_in_executor(None, embed_fn, sentences)
 
     # Calculate the pairwise cosine similarities between all the sentence embeddings.
     similarities = cosine_similarity(embeddings)
 
     # Activate the similarities to create paragraph boundaries.
     paragraph_boundaries = _activate_text_similarities(similarities, len(sentences))
 
     # Identify the split points where paragraphs end and new ones begin.
     split_points = argrelextrema(paragraph_boundaries, np.less, order=2)[0]
 
     last_split_point = 0
+    result = []
 
     for split_point in split_points:
-        yield " ".join(sentences[last_split_point:split_point])
+        result.append(sentences[last_split_point:split_point])
         last_split_point = split_point
 
     if last_split_point < len(sentences):
-        yield " ".join(sentences[last_split_point:])
+        result.append(sentences[last_split_point:])
+
+    return result
```

### Comparing `to_paragraphs-0.1.8/PKG-INFO` & `to_paragraphs-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-paragraphs
-Version: 0.1.8
+Version: 0.2.0
 Summary: 
 License: GPL-3.0
 Author: Félix Dorn
 Author-email: github@felixdorn.fr
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

