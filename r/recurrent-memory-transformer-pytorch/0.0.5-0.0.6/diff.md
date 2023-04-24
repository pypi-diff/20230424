# Comparing `tmp/recurrent-memory-transformer-pytorch-0.0.5.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.5.tar", last modified: Mon Apr 24 19:42:40 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.6.tar", last modified: Mon Apr 24 19:56:08 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.0.5.tar` & `recurrent-memory-transformer-pytorch-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:40.641164 recurrent-memory-transformer-pytorch-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 19:42:29.000000 recurrent-memory-transformer-pytorch-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 19:42:40.641164 recurrent-memory-transformer-pytorch-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 19:42:29.000000 recurrent-memory-transformer-pytorch-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:40.641164 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 19:42:29.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 19:42:29.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-24 19:42:29.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:42:40.641164 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 19:42:40.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 19:42:40.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:42:40.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 19:42:40.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 19:42:40.000000 recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:42:40.641164 recurrent-memory-transformer-pytorch-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 19:42:29.000000 recurrent-memory-transformer-pytorch-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:08.931280 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/LICENSE` & `recurrent-memory-transformer-pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/README.md` & `recurrent-memory-transformer-pytorch-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         # concat memories into the future, to be passed onto the next segment
 
         future_memories = repeat(self.memory_tokens, 'm d -> b m d', b = b)
         x = torch.cat((x, future_memories), dim = -2)
 
         # rotary embedding - offset main positions by 10000, and keep all memories at position 0
 
-        pos += 10000
+        pos = pos + 10000
         pos = F.pad(pos, (past_length, mem_length), value = 0)
 
         rotary_emb = self.rotary_pos_emb(pos)
 
         # attention and feedforward
 
         for attn, ff in self.layers:
@@ -219,18 +219,28 @@
         super().__init__()
         self.transformer = transformer
         self.seq_len = transformer.seq_len
 
     def forward(
         self,
         x,
-        memories = None
+        memories = None,
+        return_loss = False
     ):
+        if return_loss:
+            x, labels = x[:, :-1], x[:, 1:]
+
         segments = x.split(self.seq_len, dim = -1)
 
         all_logits = []
 
         for segment in segments:
             logits, memories = self.transformer(segment, memories)
             all_logits.append(logits)
 
-        return torch.cat(all_logits, dim = -2), memories
+        all_logits = torch.cat(all_logits, dim = -2)
+
+        if return_loss:
+            all_logits = rearrange(all_logits, 'b n c -> b c n')
+            return F.cross_entropy(all_logits, labels)
+
+        return all_logits, memories
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.5/setup.py` & `recurrent-memory-transformer-pytorch-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

