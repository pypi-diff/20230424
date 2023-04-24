# Comparing `tmp/recurrent-memory-transformer-pytorch-0.0.3.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.3.tar", last modified: Mon Apr 24 17:08:18 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.4.tar", last modified: Mon Apr 24 17:14:51 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.0.3.tar` & `recurrent-memory-transformer-pytorch-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:14:51.685768 recurrent-memory-transformer-pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 17:14:40.000000 recurrent-memory-transformer-pytorch-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:14:51.685768 recurrent-memory-transformer-pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-24 17:14:40.000000 recurrent-memory-transformer-pytorch-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:14:51.685768 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 17:14:40.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 17:14:40.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-24 17:14:40.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:14:51.685768 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:14:51.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 17:14:51.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:14:51.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 17:14:51.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 17:14:51.000000 recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:14:51.685768 recurrent-memory-transformer-pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 17:14:40.000000 recurrent-memory-transformer-pytorch-0.0.4/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/LICENSE` & `recurrent-memory-transformer-pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/README.md` & `recurrent-memory-transformer-pytorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch/attend.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             mask = mask.expand(-1, heads, q_len, -1)
 
         # Check if there is a compatible device for flash attention
 
         config = self.cuda_config if is_cuda else self.cpu_config
 
         # pytorch 2.0 flash attn: q, k, v, mask, dropout, causal, softmax_scale
-        
+
         with torch.backends.cuda.sdp_kernel(**config._asdict()):
             out = F.scaled_dot_product_attention(
                 q, k, v,
                 attn_mask = mask,
                 dropout_p = self.dropout if self.training else 0., 
                 is_causal = self.causal
             )
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,17 @@
         assert num_memory_tokens > 0
         self.max_segments = max_segments
 
         self.token_emb = nn.Embedding(num_tokens, dim)
         self.pos_emb = nn.Embedding(seq_len, dim)
 
         self.num_memory_tokens = num_memory_tokens
+
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
+        nn.init.normal_(self.memory_tokens, std = 0.02)
 
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 Attention(
                     dim = dim,
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.4/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.3/setup.py` & `recurrent-memory-transformer-pytorch-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

