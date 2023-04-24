# Comparing `tmp/recurrent-memory-transformer-pytorch-0.0.2.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.2.tar", last modified: Mon Apr 24 17:06:11 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.0.3.tar", last modified: Mon Apr 24 17:08:18 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.0.2.tar` & `recurrent-memory-transformer-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:06:11.438485 recurrent-memory-transformer-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 17:06:00.000000 recurrent-memory-transformer-pytorch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:06:11.438485 recurrent-memory-transformer-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-24 17:06:00.000000 recurrent-memory-transformer-pytorch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:06:11.438485 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 17:06:00.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-24 17:06:00.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 17:06:00.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:06:11.438485 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:06:11.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 17:06:11.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:06:11.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 17:06:11.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 17:06:11.000000 recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:06:11.438485 recurrent-memory-transformer-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 17:06:00.000000 recurrent-memory-transformer-pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 17:08:18.000000 recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:08:18.500656 recurrent-memory-transformer-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 17:08:07.000000 recurrent-memory-transformer-pytorch-0.0.3/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/LICENSE` & `recurrent-memory-transformer-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/README.md` & `recurrent-memory-transformer-pytorch-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from recurrent_memory_transformer_pytorch import RecurrentMemoryTransformer
 
 model = RecurrentMemoryTransformer(
     num_tokens = 256,                 # number of tokens
     num_memory_tokens = 128,          # number of memory tokens, this will determine the bottleneck for information being passed to the future
     dim = 512,                        # model dimensions
     depth = 6,                        # transformer depth
+    causal = True,                    # autoregressive or not
     dim_head = 64,                    # dimension per head
     heads = 8,                        # heads
     seq_len = 1024,                   # sequence length of a segment
     use_flash_attn = True             # whether to use flash attention
 )
 
 x = torch.randint(0, 256, (1, 1024))
```

#### html2text {}

```diff
@@ -5,31 +5,31 @@
 their generous sponsorships to work on and open source cutting edge artificial
 intelligence research ## Install ```bash $ pip install recurrent-memory-
 transformer-pytorch ``` ## Usage ```python import torch from
 recurrent_memory_transformer_pytorch import RecurrentMemoryTransformer model =
 RecurrentMemoryTransformer( num_tokens = 256, # number of tokens
 num_memory_tokens = 128, # number of memory tokens, this will determine the
 bottleneck for information being passed to the future dim = 512, # model
-dimensions depth = 6, # transformer depth dim_head = 64, # dimension per head
-heads = 8, # heads seq_len = 1024, # sequence length of a segment
-use_flash_attn = True # whether to use flash attention ) x = torch.randint(0,
-256, (1, 1024)) logits1, mem1 = model(x) # (1, 1024, 512), (1, 128, 512)
-logits2, mem2 = model(x, mem1) # (1, 1024, 512), (1, 128, 512) logits3, mem3 =
-model(x, mem2) # (1, 1024, 512), (1, 128, 512) # and so on ... ``` ## Todo -
-[ ] add a wrapper that does simple memory checkpointing for starters - [ ]
-relative positional encoding, with positional encoding for each recurrence step
-- [ ] add an axial attention down the past memories axis as an option - [ ] add
-the memory replay backprop technique from memformer paper ## Alternatives -
-Block_Recurrent_Transformer - Memformer ## Citations ```bibtex @inproceedings
-{bulatov2022recurrent, title = {Recurrent Memory Transformer}, author = {Aydar
-Bulatov and Yuri Kuratov and Mikhail Burtsev}, booktitle = {Advances in Neural
-Information Processing Systems}, editor = {Alice H. Oh and Alekh Agarwal and
-Danielle Belgrave and Kyunghyun Cho}, year = {2022}, url = {https://
-openreview.net/forum?id=Uynr3iPhksa} } ``` ```bibtex @misc{bulatov2023scaling,
-title = {Scaling Transformer to 1M tokens and beyond with RMT}, author = {Aydar
-Bulatov and Yuri Kuratov and Mikhail S. Burtsev}, year = {2023}, eprint =
-{2304.11062}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ```
+dimensions depth = 6, # transformer depth causal = True, # autoregressive or
+not dim_head = 64, # dimension per head heads = 8, # heads seq_len = 1024, #
+sequence length of a segment use_flash_attn = True # whether to use flash
+attention ) x = torch.randint(0, 256, (1, 1024)) logits1, mem1 = model(x) # (1,
+1024, 512), (1, 128, 512) logits2, mem2 = model(x, mem1) # (1, 1024, 512), (1,
+128, 512) logits3, mem3 = model(x, mem2) # (1, 1024, 512), (1, 128, 512) # and
+so on ... ``` ## Todo - [ ] add a wrapper that does simple memory checkpointing
+for starters - [ ] relative positional encoding, with positional encoding for
+each recurrence step - [ ] add an axial attention down the past memories axis
+as an option - [ ] add the memory replay backprop technique from memformer
+paper ## Alternatives - Block_Recurrent_Transformer - Memformer ## Citations
+```bibtex @inproceedings{bulatov2022recurrent, title = {Recurrent Memory
+Transformer}, author = {Aydar Bulatov and Yuri Kuratov and Mikhail Burtsev},
+booktitle = {Advances in Neural Information Processing Systems}, editor =
+{Alice H. Oh and Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho}, year =
+{2022}, url = {https://openreview.net/forum?id=Uynr3iPhksa} } ``` ```bibtex
+@misc{bulatov2023scaling, title = {Scaling Transformer to 1M tokens and beyond
+with RMT}, author = {Aydar Bulatov and Yuri Kuratov and Mikhail S. Burtsev},
+year = {2023}, eprint = {2304.11062}, archivePrefix = {arXiv}, primaryClass =
+{cs.CL} } ``` ```bibtex @inproceedings{dao2022flashattention, title = {Flash
+{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R
+{\'e}, Christopher}, booktitle = {Advances in Neural Information Processing
+Systems}, year = {2022} } ```
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         self,
         dim,
         *,
         num_tokens,
         depth,
         num_memory_tokens,
         seq_len,
+        causal = True,
         max_segments = 7,   # in the paper, they went up to 7 segments
         dim_head = 64,
         heads = 8,
         ff_mult = 4,
         use_flash_attn = False
     ):
         super().__init__()
@@ -115,14 +116,15 @@
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
                 Attention(
                     dim = dim,
                     dim_head = dim_head,
+                    causal = causal,
                     heads = heads,
                     use_flash_attn = use_flash_attn
                 ),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
         self.to_logits = nn.Sequential(
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.0.3/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.0.2/setup.py` & `recurrent-memory-transformer-pytorch-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

