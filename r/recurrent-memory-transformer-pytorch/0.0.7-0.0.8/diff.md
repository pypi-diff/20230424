# Comparing `tmp/recurrent-memory-transformer-pytorch-0.0.7.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.7.tar", last modified: Mon Apr 24 20:02:45 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.8.tar", last modified: Mon Apr 24 20:57:14 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.0.7.tar` & `recurrent-memory-transformer-pytorch-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:57:14.455706 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 20:57:14.000000 recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:57:14.459706 recurrent-memory-transformer-pytorch-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 20:57:01.000000 recurrent-memory-transformer-pytorch-0.0.8/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/LICENSE` & `recurrent-memory-transformer-pytorch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/README.md` & `recurrent-memory-transformer-pytorch-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import math
+
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat
 
 from recurrent_memory_transformer_pytorch.attend import Attend
@@ -13,14 +15,45 @@
 
 def default(vals):
     for val in vals:
         if exists(val):
             return val
     return None
 
+def eval_decorator(fn):
+    def inner(self, *args, **kwargs):
+        was_training = self.training
+        self.eval()
+        out = fn(self, *args, **kwargs)
+        self.train(was_training)
+        return out
+    return inner
+
+def divisible_by(numer, denom):
+    return (numer % denom) == 0
+
+# sampling helpers
+
+def log(t, eps = 1e-20):
+    return torch.log(t.clamp(min = eps))
+
+def gumbel_noise(t):
+    noise = torch.zeros_like(t).uniform_(0, 1)
+    return -log(-log(noise))
+
+def gumbel_sample(t, temperature = 1., dim = -1):
+    return ((t / max(temperature, 1e-10)) + gumbel_noise(t)).argmax(dim = dim)
+
+def top_k(logits, thres = 0.9):
+    k = math.ceil((1 - thres) * logits.shape[-1])
+    val, ind = torch.topk(logits, k)
+    probs = torch.full_like(logits, float('-inf'))
+    probs.scatter_(1, ind, val)
+    return probs
+
 # rotary embedding
 
 class RotaryEmbedding(nn.Module):
     def __init__(self, dim, theta = 32768):
         super().__init__()
         inv_freq = 1. / (theta ** (torch.arange(0, dim, 2).float() / dim))
         self.register_buffer('inv_freq', inv_freq)
@@ -123,16 +156,15 @@
         depth,
         num_memory_tokens,
         seq_len,
         causal = True,        
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
-        use_flash_attn = False,
-        sum_past_memories_to_future = False
+        use_flash_attn = False
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
         assert num_memory_tokens > 0
 
@@ -146,16 +178,14 @@
         # memory related
 
         self.num_memory_tokens = num_memory_tokens
 
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
         nn.init.normal_(self.memory_tokens, std = 0.02)
 
-        self.sum_past_memories_to_future  = sum_past_memories_to_future
-
         # layers
 
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 Attention(
@@ -184,28 +214,24 @@
 
         x = self.token_emb(x)
         x = x + self.pos_emb(pos)
 
         # concat memories into the future, to be passed onto the next segment
 
         future_memories = repeat(self.memory_tokens, 'm d -> b m d', b = b)
+        x = torch.cat((x, future_memories), dim = -2)
 
         # concat past memories, if needed
 
         past_length = 0
 
         if exists(past_memories):
             x = torch.cat((past_memories, x), dim = -2)
             past_length = mem_length
 
-            if self.sum_past_memories_to_future:
-                future_memories = future_memories + past_memories
-
-        x = torch.cat((x, future_memories), dim = -2)
-
         # rotary embedding - offset main positions by 10000, and keep all memories at position 0
 
         pos = pos + 10000
         pos = F.pad(pos, (past_length, mem_length), value = 0)
 
         rotary_emb = self.rotary_pos_emb(pos)
 
@@ -233,18 +259,44 @@
         super().__init__()
         self.transformer = transformer
         self.seq_len = transformer.seq_len
 
     @torch.no_grad()
     def generate(
         self,
-        length
+        prime,
+        *,
+        length,
+        memories = None,
+        temperature = 1.,
+        filter_thres = 0.9,
     ):
         assert self.transformer.causal, 'only autoregressive transformers can generate'
-        raise NotImplementedError
+
+        start_len = prime.shape[-1]
+
+        output = prime
+
+        for ind in range(length - start_len):
+
+            logits, next_memories = self.forward(output, memories)
+
+            logits = logits[:, -1]
+
+            filtered_logits = top_k(logits, thres = filter_thres)
+            sampled = gumbel_sample(filtered_logits, temperature = temperature)
+            sampled = rearrange(sampled, 'b -> b 1')
+
+            output = torch.cat((output, sampled), dim = -1)
+
+            if divisible_by(output.shape[-1] - 1, self.seq_len):
+                memories = next_memories
+
+        output = output[:, start_len:]
+        return output
 
     def forward(
         self,
         x,
         memories = None,
         return_loss = False
     ):
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.8/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.7/setup.py` & `recurrent-memory-transformer-pytorch-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

