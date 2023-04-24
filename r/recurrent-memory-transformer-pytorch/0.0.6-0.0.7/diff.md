# Comparing `tmp/recurrent-memory-transformer-pytorch-0.0.6.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.6.tar", last modified: Mon Apr 24 19:56:08 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.7.tar", last modified: Mon Apr 24 20:02:45 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.0.6.tar` & `recurrent-memory-transformer-pytorch-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:08.931280 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 19:56:08.000000 recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:56:08.935279 recurrent-memory-transformer-pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 19:55:55.000000 recurrent-memory-transformer-pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 20:02:45.000000 recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:02:45.129834 recurrent-memory-transformer-pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 20:02:31.000000 recurrent-memory-transformer-pytorch-0.0.7/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/LICENSE` & `recurrent-memory-transformer-pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/README.md` & `recurrent-memory-transformer-pytorch-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         if exists(val):
             return val
     return None
 
 # rotary embedding
 
 class RotaryEmbedding(nn.Module):
-    def __init__(self, dim, theta = 64000):
+    def __init__(self, dim, theta = 32768):
         super().__init__()
         inv_freq = 1. / (theta ** (torch.arange(0, dim, 2).float() / dim))
         self.register_buffer('inv_freq', inv_freq)
 
     def forward(self, positions):
         freqs = torch.einsum('i , j -> i j', positions, self.inv_freq)
         freqs = torch.cat((freqs, freqs), dim = -1)
@@ -75,15 +75,14 @@
         dim_head = 64,
         heads = 8,
         dropout = 0.,
         use_flash_attn = False
     ):
         super().__init__()
         dim_inner = dim_head * heads
-        self.scale = dim_head ** -0.5
         self.heads = heads
 
         self.attend = Attend(causal = causal, dropout = dropout, use_flash = use_flash_attn)
 
         self.norm = RMSNorm(dim)
 
         self.to_q = nn.Linear(dim, dim_inner, bias = False)
@@ -124,31 +123,41 @@
         depth,
         num_memory_tokens,
         seq_len,
         causal = True,        
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
-        use_flash_attn = False
+        use_flash_attn = False,
+        sum_past_memories_to_future = False
     ):
         super().__init__()
+        self.causal = causal
         self.seq_len = seq_len
 
         assert num_memory_tokens > 0
 
         self.token_emb = nn.Embedding(num_tokens, dim)
-        self.pos_emb = nn.Embedding(seq_len, dim)
 
+        # positions
+
+        self.pos_emb = nn.Embedding(seq_len, dim)
         self.rotary_pos_emb = RotaryEmbedding(dim_head)
 
+        # memory related
+
         self.num_memory_tokens = num_memory_tokens
 
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
         nn.init.normal_(self.memory_tokens, std = 0.02)
 
+        self.sum_past_memories_to_future  = sum_past_memories_to_future
+
+        # layers
+
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 Attention(
                     dim = dim,
                     dim_head = dim_head,
@@ -172,24 +181,29 @@
         b, n, device, mem_length = *x.shape, x.device, self.num_memory_tokens
 
         pos = torch.arange(n, device = device)
 
         x = self.token_emb(x)
         x = x + self.pos_emb(pos)
 
+        # concat memories into the future, to be passed onto the next segment
+
+        future_memories = repeat(self.memory_tokens, 'm d -> b m d', b = b)
+
         # concat past memories, if needed
 
         past_length = 0
+
         if exists(past_memories):
             x = torch.cat((past_memories, x), dim = -2)
             past_length = mem_length
 
-        # concat memories into the future, to be passed onto the next segment
+            if self.sum_past_memories_to_future:
+                future_memories = future_memories + past_memories
 
-        future_memories = repeat(self.memory_tokens, 'm d -> b m d', b = b)
         x = torch.cat((x, future_memories), dim = -2)
 
         # rotary embedding - offset main positions by 10000, and keep all memories at position 0
 
         pos = pos + 10000
         pos = F.pad(pos, (past_length, mem_length), value = 0)
 
@@ -216,14 +230,22 @@
         self,
         transformer: RecurrentMemoryTransformer
     ):
         super().__init__()
         self.transformer = transformer
         self.seq_len = transformer.seq_len
 
+    @torch.no_grad()
+    def generate(
+        self,
+        length
+    ):
+        assert self.transformer.causal, 'only autoregressive transformers can generate'
+        raise NotImplementedError
+
     def forward(
         self,
         x,
         memories = None,
         return_loss = False
     ):
         if return_loss:
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.7/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.6/setup.py` & `recurrent-memory-transformer-pytorch-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

