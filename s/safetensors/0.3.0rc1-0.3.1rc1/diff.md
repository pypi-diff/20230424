# Comparing `tmp/safetensors-0.3.0rc1.tar.gz` & `tmp/safetensors-0.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safetensors-0.3.0rc1.tar", last modified: Thu Mar  2 11:23:07 2023, max compression
+gzip compressed data, was "safetensors-0.3.1rc1.tar", last modified: Mon Apr 24 15:00:13 2023, max compression
```

## Comparing `safetensors-0.3.0rc1.tar` & `safetensors-0.3.1rc1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-02 11:23:05.000000 safetensors-0.3.0rc1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.228886 safetensors-0.3.0rc1/py_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/py_src/safetensors/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/py_src/safetensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/py_src/safetensors/flax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/py_src/safetensors/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/py_src/safetensors/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/py_src/safetensors/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/py_src/safetensors/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/py_src/safetensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-02 11:23:07.000000 safetensors-0.3.0rc1/py_src/safetensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-02 11:23:07.000000 safetensors-0.3.0rc1/py_src/safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 11:23:07.000000 safetensors-0.3.0rc1/py_src/safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 11:23:07.000000 safetensors-0.3.0rc1/py_src/safetensors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-02 11:23:07.000000 safetensors-0.3.0rc1/py_src/safetensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-02 11:23:07.000000 safetensors-0.3.0rc1/py_src/safetensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/safetensors-lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/safetensors-lib/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/benches/benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/safetensors-lib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/safetensors-lib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/safetensors-lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/src/slice.rs
--rw-r--r--   0 runner    (1001) docker     (123)    27589 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/safetensors-lib/src/tensor.rs
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-02 11:23:07.236886 safetensors-0.3.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 11:23:07.232886 safetensors-0.3.0rc1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    32919 2023-03-02 11:22:43.000000 safetensors-0.3.0rc1/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 15:00:12.000000 safetensors-0.3.1rc1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.598883 safetensors-0.3.1rc1/py_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.598883 safetensors-0.3.1rc1/py_src/safetensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/flax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/py_src/safetensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/README.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/benches/benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/tensor.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    33654 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/src/lib.rs
```

### Comparing `safetensors-0.3.0rc1/PKG-INFO` & `safetensors-0.3.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.3.0rc1
+Version: 0.3.1rc1
 Summary: Fast and Safe Tensor serialization
 Home-page: https://github.com/huggingface/safetensors
 Author: 
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `safetensors-0.3.0rc1/README.md` & `safetensors-0.3.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.0rc1/py_src/safetensors/flax.py` & `safetensors-0.3.1rc1/py_src/safetensors/flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.0rc1/py_src/safetensors/numpy.py` & `safetensors-0.3.1rc1/py_src/safetensors/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     for k, v in safeview:
         dtype = _getdtype(v["dtype"])
         arr = np.frombuffer(v["data"], dtype=dtype).reshape(v["shape"])
         result[k] = arr
     return result
 
 
-def _is_little_endian(tensor: np.ndarray) -> str:
+def _is_little_endian(tensor: np.ndarray) -> bool:
     byteorder = tensor.dtype.byteorder
     if byteorder == "=":
         if sys.byteorder == "little":
             return True
         else:
             return False
     elif byteorder == "|":
```

### Comparing `safetensors-0.3.0rc1/py_src/safetensors/paddle.py` & `safetensors-0.3.1rc1/py_src/safetensors/paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.0rc1/py_src/safetensors/tensorflow.py` & `safetensors-0.3.1rc1/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.0rc1/py_src/safetensors.egg-info/PKG-INFO` & `safetensors-0.3.1rc1/py_src/safetensors.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.3.0rc1
+Version: 0.3.1rc1
 Summary: Fast and Safe Tensor serialization
 Home-page: https://github.com/huggingface/safetensors
 Author: 
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `safetensors-0.3.0rc1/py_src/safetensors.egg-info/SOURCES.txt` & `safetensors-0.3.1rc1/py_src/safetensors.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 py_src/safetensors.egg-info/SOURCES.txt
 py_src/safetensors.egg-info/dependency_links.txt
 py_src/safetensors.egg-info/not-zip-safe
 py_src/safetensors.egg-info/requires.txt
 py_src/safetensors.egg-info/top_level.txt
 safetensors-lib/Cargo.toml
 safetensors-lib/README.md
+safetensors-lib/README.tpl
 safetensors-lib/benches/benchmark.rs
 safetensors-lib/fuzz/.gitignore
 safetensors-lib/fuzz/Cargo.toml
 safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
 safetensors-lib/src/lib.rs
 safetensors-lib/src/slice.rs
 safetensors-lib/src/tensor.rs
```

### Comparing `safetensors-0.3.0rc1/safetensors-lib/Cargo.toml` & `safetensors-0.3.1rc1/safetensors-lib/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [package]
 name = "safetensors"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 homepage = "https://github.com/huggingface/safetensors"
 repository = "https://github.com/huggingface/safetensors"
 documentation = "https://docs.rs/safetensors/"
 license = "Apache-2.0"
-keywords = ["safetensors", "huggingface", "Tensors", "Pytorch", "Tensorflow", "PaddlePaddle"]
+keywords = ["safetensors", "huggingface", "Tensors", "Pytorch", "Tensorflow"]
 readme = "./README.md"
 description = """
 Provides functions to read and write safetensors which aim to be safer than
 their PyTorch counterpart.
 The format is 8 bytes which is an unsized int, being the size of a JSON header,
 the JSON header refers the `dtype` the `shape` and `data_offsets` which are the offsets
 for the values in the rest of the file.
@@ -22,11 +22,13 @@
 
 [dependencies]
 serde = {version = "1.0", features = ["derive"]}
 serde_json = "1.0"
 
 [dev-dependencies]
 criterion = "0.4"
+memmap2 = "0.5"
+proptest = "1.1"
 
 [[bench]]
 name = "benchmark"
 harness = false
```

### Comparing `safetensors-0.3.0rc1/safetensors-lib/README.md` & `safetensors-0.3.1rc1/safetensors-lib/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Python
+[![Pypi](https://img.shields.io/pypi/v/safetensors.svg)](https://pypi.org/pypi/safetensors/)
+[![Documentation](https://img.shields.io/website/http/huggingface.co/docs/safetensors/index.svg?label=docs)](https://huggingface.co/docs/safetensors/index)
+[![Codecov](https://codecov.io/github/huggingface/safetensors/coverage.svg?branch=main)](https://codecov.io/gh/huggingface/safetensors)
+[![Downloads](https://static.pepy.tech/badge/safetensors/month)](https://pepy.tech/project/safetensors)
+
+Rust
+[![Crates.io](https://img.shields.io/crates/v/safetensors.svg)](https://crates.io/crates/safetensors)
+[![Documentation](https://docs.rs/safetensors/badge.svg)](https://docs.rs/safetensors/)
+[![Codecov](https://codecov.io/github/huggingface/safetensors/coverage.svg?branch=main)](https://codecov.io/gh/huggingface/safetensors)
+[![Dependency status](https://deps.rs/repo/github/huggingface/safetensors/status.svg?path=safetensors)](https://deps.rs/repo/github/huggingface/safetensors?path=safetensors)
+
 # safetensors
 
 ## Safetensors
 
 This repository implements a new simple format for storing tensors
 safely (as opposed to pickle) and that is still fast (zero-copy).
 
@@ -28,14 +40,15 @@
 pip install setuptools_rust
 pip install -e .
 ```
 
 ### Getting started
 
 ```python
+import torch
 from safetensors import safe_open
 from safetensors.torch import save_file
 
 tensors = {
    "weight1": torch.zeros((1024, 1024)),
    "weight2": torch.zeros((1024, 1024))
 }
@@ -50,18 +63,32 @@
 [Python documentation](https://huggingface.co/docs/safetensors/index)
 
 
 ### Format
 
 - 8 bytes: `N`, a u64 int, containing the size of the header
 - N bytes: a JSON utf-8 string representing the header.
-  - The header is a dict like {"TENSOR_NAME": {"dtype": "float16", "shape": [1, 16, 256], "offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}, where offsets point to the tensor data relative to the beginning of the byte buffer, with BEGIN as the starting offset and END as the one-past offset (so total tensor byte size = END - BEGIN).
-  - A special key `__metadata__` is allowed to contain free form text map.
+  - The header is a dict like `{"TENSOR_NAME": {"dtype": "F16", "shape": [1, 16, 256], "offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}`, where offsets point to the tensor data relative to the beginning of the byte buffer, with `BEGIN` as the starting offset and `END` as the one-past offset (so total tensor byte size = `END - BEGIN`).
+  - A special key `__metadata__` is allowed to contain free form text-to-text map.
 - Rest of the file: byte-buffer.
 
+Notes:
+ - Duplicate keys are disallowed. Not all parsers may respect this.
+ - In general the subset of JSON is implicitly decided by `serde_json` for
+ this library. Anything obscure might be modified at a later time, that odd ways
+ to represent integer, newlines and escapes in utf-8 strings. This would only
+ be done for safety concerns
+ - Tensor values are not checked against, in particular NaN and +/-Inf could
+ be in the file
+ - Empty tensors (tensors with 1 dimension being 0) are allowed.
+ They are not storing any data in the databuffer, yet retaining size in the header.
+ They don't really bring a lot of values but are accepted since they are valid tensors
+ from traditional tensor libraries perspective (torch, tensorflow, numpy, ..).
+ - 0-rank Tensors (tensors with shape `[]`) are allowed, they are merely a scalar.
+
 
 ### Yet another format ?
 
 The main rationale for this crate is to remove the need to use
 `pickle` on `PyTorch` which is used by default.
 There are other formats out there used by machine learning and more general
 formats.
@@ -98,24 +125,25 @@
 
 - Pickle: Unsafe, runs arbitrary code
 - H5: Apparently now discouraged for TF/Keras. Seems like a great fit otherwise actually. Some classic use after free issues: <https://www.cvedetails.com/vulnerability-list/vendor_id-15991/product_id-35054/Hdfgroup-Hdf5.html>. On a very different level than pickle security-wise. Also 210k lines of code vs ~400 lines for this lib currently.
 - SavedModel: Tensorflow specific (it contains TF graph information).
 - MsgPack: No layout control to enable lazy loading (important for loading specific parts in distributed setting)
 - Protobuf: Hard 2Go max file size limit
 - Cap'n'proto: Float16 support is not present [link](https://capnproto.org/language.html#built-in-types) so using a manual wrapper over a byte-buffer would be necessary. Layout control seems possible but not trivial as buffers have limitations [link](https://stackoverflow.com/questions/48458839/capnproto-maximum-filesize).
-- Numpy (npz): No `bfloat16` support. Vulnerable to zip bombs (DOS).
+- Numpy (npz): No `bfloat16` support. Vulnerable to zip bombs (DOS). Not zero-copy.
 - Arrow: No `bfloat16` support. Seem to require decoding [link](https://arrow.apache.org/docs/python/parquet.html#reading-parquet-and-memory-mapping)
 
 ### Notes
 
-- Zero-copy: No format is really zero-copy in ML, it needs to go from disk to RAM/GPU RAM (that takes time). Also
-   In PyTorch/numpy, you need a mutable buffer, and we don't really want to mutate a mmaped file, so 1 copy is really necessary to use the thing freely in user code. That being said, zero-copy is achievable in Rust if it's wanted and safety can be guaranteed by some other means.
+- Zero-copy: No format is really zero-copy in ML, it needs to go from disk to RAM/GPU RAM (that takes time). On CPU, if the file is already in cache, then it can
+truly be zero-copy, whereas on GPU there is not such disk cache, so a copy is always required
+but you can bypass allocating all the tensors on CPU at any given point.
    SafeTensors is not zero-copy for the header. The choice of JSON is pretty arbitrary, but since deserialization is <<< of the time required to load the actual tensor data and is readable I went that way, (also space is <<< to the tensor data).
 
-- Endianness: Little-endian. This can be modified later, but it feels really unecessary at the
+- Endianness: Little-endian. This can be modified later, but it feels really unnecessary at the
 moment.
 - Order: 'C' or row-major. This seems to have won. We can add that information later if needed.
 - Stride: No striding, all tensors need to be packed before being serialized. I have yet to see a case where it seems useful to have a strided tensor stored in serialized format.
 
 ### Benefits
 
 Since we can invent a new format we can propose additional benefits:
@@ -125,19 +153,19 @@
 on the size of the header of 100MB to prevent parsing extremely large JSON.
  Also when reading the file, there's a guarantee that addresses in the file
  do not overlap in any way, meaning when you're loading a file you should never
  exceed the size of the file in memory
 
 - Faster load: PyTorch seems to be the fastest file to load out in the major
 ML formats. However, it does seem to have an extra copy on CPU, which we
-can bypass in this lib [link](https://github.com/huggingface/safetensors/pull/33).
+can bypass in this lib by using `torch.UntypedStorage.from_file`.
 Currently, CPU loading times are extremely fast with this lib compared to pickle.
-GPU loading times can be sped up but are still hidden behind an environment variable
-(`SAFETENSORS_FAST_GPU=1`) because it hasn't received enough external scrutiny to be safe.
-But it does load roughly 2X faster than PyTorch on regular Linux hardware because of this extra CPU copy skip.
+GPU loading times are as fast or faster than PyTorch equivalent.
+Loading first on CPU with memmapping with torch, and then moving all tensors to GPU seems
+to be faster too somehow (similar behavior in torch pickle)
 
 - Lazy loading: in distributed (multi-node or multi-gpu) settings, it's nice to be able to
 load only part of the tensors on the various models. For
 [BLOOM](https://huggingface.co/bigscience/bloom) using this format enabled
 to load the model on 8 GPUs from 10mn with regular PyTorch weights down to 45s.
 This really speeds up feedbacks loops when developing on the model. For instance
 you don't have to have separate copies of the weights when changing the distribution
```

### Comparing `safetensors-0.3.0rc1/safetensors-lib/benches/benchmark.rs` & `safetensors-0.3.1rc1/safetensors-lib/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.0rc1/safetensors-lib/src/lib.rs` & `safetensors-0.3.1rc1/safetensors-lib/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 //!pip install setuptools_rust
 //!pip install -e .
 //!```
 //!
 //!## Getting started
 //!
 //!```python
+//!import torch
 //!from safetensors import safe_open
 //!from safetensors.torch import save_file
 //!
 //!tensors = {
 //!    "weight1": torch.zeros((1024, 1024)),
 //!    "weight2": torch.zeros((1024, 1024))
 //!}
@@ -49,18 +50,32 @@
 //![Python documentation](https://huggingface.co/docs/safetensors/index)
 //!
 //!
 //!## Format
 //!
 //! - 8 bytes: `N`, a u64 int, containing the size of the header
 //! - N bytes: a JSON utf-8 string representing the header.
-//!   - The header is a dict like {"TENSOR_NAME": {"dtype": "float16", "shape": [1, 16, 256], "offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}, where offsets point to the tensor data relative to the beginning of the byte buffer, with BEGIN as the starting offset and END as the one-past offset (so total tensor byte size = END - BEGIN).
-//!   - A special key `__metadata__` is allowed to contain free form text map.
+//!   - The header is a dict like `{"TENSOR_NAME": {"dtype": "F16", "shape": [1, 16, 256], "offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}`, where offsets point to the tensor data relative to the beginning of the byte buffer, with `BEGIN` as the starting offset and `END` as the one-past offset (so total tensor byte size = `END - BEGIN`).
+//!   - A special key `__metadata__` is allowed to contain free form text-to-text map.
 //! - Rest of the file: byte-buffer.
 //!
+//! Notes:
+//!  - Duplicate keys are disallowed. Not all parsers may respect this.
+//!  - In general the subset of JSON is implicitly decided by `serde_json` for
+//!  this library. Anything obscure might be modified at a later time, that odd ways
+//!  to represent integer, newlines and escapes in utf-8 strings. This would only
+//!  be done for safety concerns
+//!  - Tensor values are not checked against, in particular NaN and +/-Inf could
+//!  be in the file
+//!  - Empty tensors (tensors with 1 dimension being 0) are allowed.
+//!  They are not storing any data in the databuffer, yet retaining size in the header.
+//!  They don't really bring a lot of values but are accepted since they are valid tensors
+//!  from traditional tensor libraries perspective (torch, tensorflow, numpy, ..).
+//!  - 0-rank Tensors (tensors with shape `[]`) are allowed, they are merely a scalar.
+//!
 //!
 //!## Yet another format ?
 //!
 //!The main rationale for this crate is to remove the need to use
 //!`pickle` on `PyTorch` which is used by default.
 //!There are other formats out there used by machine learning and more general
 //!formats.
@@ -97,24 +112,25 @@
 //!
 //!- Pickle: Unsafe, runs arbitrary code
 //!- H5: Apparently now discouraged for TF/Keras. Seems like a great fit otherwise actually. Some classic use after free issues: <https://www.cvedetails.com/vulnerability-list/vendor_id-15991/product_id-35054/Hdfgroup-Hdf5.html>. On a very different level than pickle security-wise. Also 210k lines of code vs ~400 lines for this lib currently.
 //!- SavedModel: Tensorflow specific (it contains TF graph information).
 //!- MsgPack: No layout control to enable lazy loading (important for loading specific parts in distributed setting)
 //!- Protobuf: Hard 2Go max file size limit
 //!- Cap'n'proto: Float16 support is not present [link](https://capnproto.org/language.html#built-in-types) so using a manual wrapper over a byte-buffer would be necessary. Layout control seems possible but not trivial as buffers have limitations [link](https://stackoverflow.com/questions/48458839/capnproto-maximum-filesize).
-//!- Numpy (npz): No `bfloat16` support. Vulnerable to zip bombs (DOS).
+//!- Numpy (npz): No `bfloat16` support. Vulnerable to zip bombs (DOS). Not zero-copy.
 //!- Arrow: No `bfloat16` support. Seem to require decoding [link](https://arrow.apache.org/docs/python/parquet.html#reading-parquet-and-memory-mapping)
 //!
 //!## Notes
 //!
-//!- Zero-copy: No format is really zero-copy in ML, it needs to go from disk to RAM/GPU RAM (that takes time). Also
-//!    In PyTorch/numpy, you need a mutable buffer, and we don't really want to mutate a mmaped file, so 1 copy is really necessary to use the thing freely in user code. That being said, zero-copy is achievable in Rust if it's wanted and safety can be guaranteed by some other means.
+//!- Zero-copy: No format is really zero-copy in ML, it needs to go from disk to RAM/GPU RAM (that takes time). On CPU, if the file is already in cache, then it can
+//! truly be zero-copy, whereas on GPU there is not such disk cache, so a copy is always required
+//! but you can bypass allocating all the tensors on CPU at any given point.
 //!    SafeTensors is not zero-copy for the header. The choice of JSON is pretty arbitrary, but since deserialization is <<< of the time required to load the actual tensor data and is readable I went that way, (also space is <<< to the tensor data).
 //!
-//!- Endianness: Little-endian. This can be modified later, but it feels really unecessary at the
+//!- Endianness: Little-endian. This can be modified later, but it feels really unnecessary at the
 //!moment.
 //!- Order: 'C' or row-major. This seems to have won. We can add that information later if needed.
 //!- Stride: No striding, all tensors need to be packed before being serialized. I have yet to see a case where it seems useful to have a strided tensor stored in serialized format.
 //!
 //!## Benefits
 //!
 //!Since we can invent a new format we can propose additional benefits:
@@ -124,19 +140,19 @@
 //!on the size of the header of 100MB to prevent parsing extremely large JSON.
 //!  Also when reading the file, there's a guarantee that addresses in the file
 //!  do not overlap in any way, meaning when you're loading a file you should never
 //!  exceed the size of the file in memory
 //!
 //!- Faster load: PyTorch seems to be the fastest file to load out in the major
 //! ML formats. However, it does seem to have an extra copy on CPU, which we
-//! can bypass in this lib [link](https://github.com/huggingface/safetensors/pull/33).
+//! can bypass in this lib by using `torch.UntypedStorage.from_file`.
 //! Currently, CPU loading times are extremely fast with this lib compared to pickle.
-//! GPU loading times can be sped up but are still hidden behind an environment variable
-//! (`SAFETENSORS_FAST_GPU=1`) because it hasn't received enough external scrutiny to be safe.
-//! But it does load roughly 2X faster than PyTorch on regular Linux hardware because of this extra CPU copy skip.
+//! GPU loading times are as fast or faster than PyTorch equivalent.
+//! Loading first on CPU with memmapping with torch, and then moving all tensors to GPU seems
+//! to be faster too somehow (similar behavior in torch pickle)
 //!
 //!- Lazy loading: in distributed (multi-node or multi-gpu) settings, it's nice to be able to
 //!load only part of the tensors on the various models. For
 //![BLOOM](https://huggingface.co/bigscience/bloom) using this format enabled
 //!to load the model on 8 GPUs from 10mn with regular PyTorch weights down to 45s.
 //!This really speeds up feedbacks loops when developing on the model. For instance
 //!you don't have to have separate copies of the weights when changing the distribution
```

### Comparing `safetensors-0.3.0rc1/safetensors-lib/src/slice.rs` & `safetensors-0.3.1rc1/safetensors-lib/src/slice.rs`

 * *Files 1% similar despite different names*

```diff
@@ -80,51 +80,51 @@
 }
 
 impl<'data, A> IndexOp<'data, A> for TensorView<'data>
 where
     A: Into<TensorIndexer>,
 {
     fn slice(&'data self, index: A) -> Result<SliceIterator<'data>, InvalidSlice> {
-        self.sliced_data(vec![index.into()])
+        self.sliced_data(&[index.into()])
     }
 }
 
 impl<'data, A> IndexOp<'data, (A,)> for TensorView<'data>
 where
     A: Into<TensorIndexer>,
 {
     fn slice(&'data self, index: (A,)) -> Result<SliceIterator<'data>, InvalidSlice> {
         let idx_a = index.0.into();
-        self.sliced_data(vec![idx_a])
+        self.sliced_data(&[idx_a])
     }
 }
 
 impl<'data, A, B> IndexOp<'data, (A, B)> for TensorView<'data>
 where
     A: Into<TensorIndexer>,
     B: Into<TensorIndexer>,
 {
     fn slice(&'data self, index: (A, B)) -> Result<SliceIterator<'data>, InvalidSlice> {
         let idx_a = index.0.into();
         let idx_b = index.1.into();
-        self.sliced_data(vec![idx_a, idx_b])
+        self.sliced_data(&[idx_a, idx_b])
     }
 }
 
 impl<'data, A, B, C> IndexOp<'data, (A, B, C)> for TensorView<'data>
 where
     A: Into<TensorIndexer>,
     B: Into<TensorIndexer>,
     C: Into<TensorIndexer>,
 {
     fn slice(&'data self, index: (A, B, C)) -> Result<SliceIterator<'data>, InvalidSlice> {
         let idx_a = index.0.into();
         let idx_b = index.1.into();
         let idx_c = index.2.into();
-        self.sliced_data(vec![idx_a, idx_b, idx_c])
+        self.sliced_data(&[idx_a, idx_b, idx_c])
     }
 }
 
 // impl<A, B, C, D> IndexOp<(A, B, C, D)> for TensorView<'data>
 // where
 //     A: Into<TensorIndexer>,
 //     B: Into<TensorIndexer>,
@@ -207,15 +207,15 @@
     indices: Vec<(usize, usize)>,
     newshape: Vec<usize>,
 }
 
 impl<'data> SliceIterator<'data> {
     pub(crate) fn new(
         view: &'data TensorView<'data>,
-        slices: Vec<TensorIndexer>,
+        slices: &[TensorIndexer],
     ) -> Result<Self, InvalidSlice> {
         // Make sure n. axis does not exceed n. of dimensions
         let n_slice = slices.len();
         let n_shape = view.shape().len();
         if n_slice > n_shape {
             return Err(InvalidSlice::TooManySlices);
         }
@@ -323,23 +323,23 @@
             .flat_map(|f| f.to_le_bytes())
             .collect();
 
         let attn_0 = TensorView::new(Dtype::F32, vec![1, 2, 3], &data).unwrap();
 
         let iterator = SliceIterator::new(
             &attn_0,
-            vec![TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded)],
+            &[TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded)],
         )
         .unwrap();
         assert_eq!(iterator.remaining_byte_len(), 24);
         assert_eq!(iterator.newshape(), vec![1, 2, 3]);
 
         let iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Included(0), Bound::Excluded(1)),
             ],
         )
         .unwrap();
         assert_eq!(iterator.remaining_byte_len(), 12);
         assert_eq!(iterator.newshape(), vec![1, 1, 3]);
@@ -352,57 +352,57 @@
             .flat_map(|f| f.to_le_bytes())
             .collect();
 
         let attn_0 = TensorView::new(Dtype::F32, vec![1, 2, 3], &data).unwrap();
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded)],
+            &[TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded)],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..24]));
         assert_eq!(iterator.next(), None);
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..24]));
         assert_eq!(iterator.next(), None);
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..24]));
         assert_eq!(iterator.next(), None);
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..24]));
         assert_eq!(iterator.next(), None);
 
         assert!(SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
             ],
         )
         .is_err(),);
@@ -415,50 +415,50 @@
             .flat_map(|f| f.to_le_bytes())
             .collect();
 
         let attn_0 = TensorView::new(Dtype::F32, vec![1, 2, 3], &data).unwrap();
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![TensorIndexer::Narrow(
+            &[TensorIndexer::Narrow(
                 Bound::Included(0),
                 Bound::Excluded(1),
             )],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..24]));
         assert_eq!(iterator.next(), None);
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Included(0), Bound::Excluded(1)),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..12]));
         assert_eq!(iterator.next(), None);
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Included(0), Bound::Excluded(1)),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[0..4]));
         assert_eq!(iterator.next(), Some(&data[12..16]));
         assert_eq!(iterator.next(), None);
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Included(1), Bound::Excluded(2)),
                 TensorIndexer::Narrow(Bound::Included(0), Bound::Excluded(1)),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[12..16]));
@@ -472,15 +472,15 @@
             .flat_map(|f| f.to_le_bytes())
             .collect();
 
         let attn_0 = TensorView::new(Dtype::F32, vec![2, 3], &data).unwrap();
 
         let mut iterator = SliceIterator::new(
             &attn_0,
-            vec![
+            &[
                 TensorIndexer::Narrow(Bound::Unbounded, Bound::Unbounded),
                 TensorIndexer::Narrow(Bound::Included(1), Bound::Excluded(3)),
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[4..12]));
         assert_eq!(iterator.next(), Some(&data[16..24]));
```

### Comparing `safetensors-0.3.0rc1/safetensors-lib/src/tensor.rs` & `safetensors-0.3.1rc1/safetensors-lib/src/tensor.rs`

 * *Files 21% similar despite different names*

```diff
@@ -20,31 +20,46 @@
     /// The header is large than 100Mo which is considered too large (Might evolve in the future).
     HeaderTooLarge,
     /// The header is smaller than 8 bytes
     HeaderTooSmall,
     /// The header length is invalid
     InvalidHeaderLength,
     /// The tensor name was not found in the archive
-    TensorNotFound,
+    TensorNotFound(String),
     /// Invalid information between shape, dtype and the proposed offsets in the file
     TensorInvalidInfo,
     /// The offsets declared for tensor with name `String` in the header are invalid
     InvalidOffset(String),
     /// IoError
     IoError(std::io::Error),
+    /// JSON error
+    JsonError(serde_json::Error),
     /// The follow tensor cannot be created because the buffer size doesn't match shape + dtype
     InvalidTensorView(Dtype, Vec<usize>, usize),
+    /// The metadata is invalid because the data offsets of the tensor does not
+    /// fully cover the buffer part of the file. The last offset **must** be
+    /// the end of the file.
+    MetadataIncompleteBuffer,
+    /// The metadata contains information (shape or shape * dtype size) which lead to an
+    /// arithmetic overflow. This is most likely an error in the file.
+    ValidationOverflow,
 }
 
 impl From<std::io::Error> for SafeTensorError {
     fn from(error: std::io::Error) -> SafeTensorError {
         SafeTensorError::IoError(error)
     }
 }
 
+impl From<serde_json::Error> for SafeTensorError {
+    fn from(error: serde_json::Error) -> SafeTensorError {
+        SafeTensorError::JsonError(error)
+    }
+}
+
 impl std::fmt::Display for SafeTensorError {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "{self:?}")
     }
 }
 
 impl std::error::Error for SafeTensorError {}
@@ -172,17 +187,17 @@
         };
         offset += n;
         hmetadata.push((name.to_string(), tensor_info));
         tensors.push(tensor);
     }
 
     let metadata: Metadata = Metadata::new(data_info.clone(), hmetadata)?;
-    let mut metadata_buf = serde_json::to_string(&metadata).unwrap().into_bytes();
-    // Force alignment
-    let extra = metadata_buf.len() % 8;
+    let mut metadata_buf = serde_json::to_string(&metadata)?.into_bytes();
+    // Force alignment to 8 bytes.
+    let extra = (8 - metadata_buf.len() % 8) % 8;
     metadata_buf.extend(vec![b' '; extra]);
 
     let n: u64 = metadata_buf.len() as u64;
 
     Ok((
         PreparedData {
             n,
@@ -246,14 +261,15 @@
     }
     f.flush()?;
     Ok(())
 }
 
 /// A structure owning some metadata to lookup tensors on a shared `data`
 /// byte-buffer (not owned).
+#[derive(Debug)]
 pub struct SafeTensors<'data> {
     metadata: Metadata,
     data: &'data [u8],
 }
 
 impl<'data> SafeTensors<'data> {
     /// Given a byte-buffer representing the whole safetensor file
@@ -284,19 +300,39 @@
         if stop > buffer_len {
             return Err(SafeTensorError::InvalidHeaderLength);
         }
         let string =
             std::str::from_utf8(&buffer[8..stop]).map_err(|_| SafeTensorError::InvalidHeader)?;
         let metadata: Metadata = serde_json::from_str(string)
             .map_err(|_| SafeTensorError::InvalidHeaderDeserialization)?;
-        metadata.validate()?;
+        let buffer_end = metadata.validate()?;
+        if buffer_end + 8 + n != buffer_len {
+            return Err(SafeTensorError::MetadataIncompleteBuffer);
+        }
         Ok((n, metadata))
     }
     /// Given a byte-buffer representing the whole safetensor file
     /// parses it and returns the Deserialized form (No Tensor allocation).
+    ///
+    /// ```
+    /// use safetensors::SafeTensors;
+    /// use memmap2::MmapOptions;
+    /// use std::fs::File;
+    ///
+    /// let filename = "model.safetensors";
+    /// # use std::io::Write;
+    /// # let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00";
+    /// # File::create(filename).unwrap().write(serialized).unwrap();
+    /// let file = File::open(filename).unwrap();
+    /// let buffer = unsafe { MmapOptions::new().map(&file).unwrap() };
+    /// let tensors = SafeTensors::deserialize(&buffer).unwrap();
+    /// let tensor = tensors
+    ///         .tensor("test")
+    ///         .unwrap();
+    /// ```
     pub fn deserialize<'in_data>(buffer: &'in_data [u8]) -> Result<Self, SafeTensorError>
     where
         'in_data: 'data,
     {
         let (n, metadata) = SafeTensors::read_metadata(buffer)?;
         let data = &buffer[n + 8..];
         Ok(Self { metadata, data })
@@ -327,32 +363,32 @@
             if let Some(info) = &self.metadata.tensors.get(**index) {
                 Ok(TensorView {
                     dtype: info.dtype,
                     shape: info.shape.clone(),
                     data: &self.data[info.data_offsets.0..info.data_offsets.1],
                 })
             } else {
-                Err(SafeTensorError::TensorNotFound)
+                Err(SafeTensorError::TensorNotFound(tensor_name.to_string()))
             }
         } else {
-            Err(SafeTensorError::TensorNotFound)
+            Err(SafeTensorError::TensorNotFound(tensor_name.to_string()))
         }
     }
 
     /// Allow the user to get a specific tensor within the SafeTensors.
     /// The tensor returned is merely a view and the data is not owned by this
     /// structure.
     pub fn names(&self) -> Vec<&'_ String> {
         self.metadata.index_map.keys().collect()
     }
 }
 
 /// The stuct representing the header of safetensor files which allow
 /// indexing into the raw byte-buffer array and how to interpret it.
-#[derive(Debug)]
+#[derive(Debug, Clone)]
 pub struct Metadata {
     metadata: Option<HashMap<String, String>>,
     tensors: Vec<TensorInfo>,
     index_map: HashMap<String, usize>,
 }
 
 /// Helper struct used only for serialization deserialization
@@ -425,36 +461,41 @@
             tensors,
             index_map,
         };
         // metadata.validate()?;
         Ok(metadata)
     }
 
-    fn validate(&self) -> Result<(), SafeTensorError> {
+    fn validate(&self) -> Result<usize, SafeTensorError> {
         let mut start = 0;
         for (i, info) in self.tensors.iter().enumerate() {
             let (s, e) = info.data_offsets;
             if s != start || e < s {
                 let tensor_name = self
                     .index_map
                     .iter()
-                    .filter_map(|(name, &index)| if index == i { Some(&name[..]) } else { None })
-                    .next()
+                    .find_map(|(name, &index)| if index == i { Some(&name[..]) } else { None })
                     .unwrap_or("no_tensor");
                 return Err(SafeTensorError::InvalidOffset(tensor_name.to_string()));
             }
             start = e;
-            let nelements: usize = info.shape.iter().product();
-            let nbytes = nelements * info.dtype.size();
+            let nelements: usize = info
+                .shape
+                .iter()
+                .cloned()
+                .try_fold(1usize, usize::checked_mul)
+                .ok_or(SafeTensorError::ValidationOverflow)?;
+            let nbytes = nelements
+                .checked_mul(info.dtype.size())
+                .ok_or(SafeTensorError::ValidationOverflow)?;
             if (e - s) != nbytes {
                 return Err(SafeTensorError::TensorInvalidInfo);
             }
         }
-
-        Ok(())
+        Ok(start)
     }
 
     /// Gives back the tensor metadata
     pub fn tensors(&self) -> HashMap<String, &TensorInfo> {
         self.index_map
             .iter()
             .map(|(tensor_name, index)| (tensor_name.clone(), &self.tensors[*index]))
@@ -466,15 +507,15 @@
         &self.metadata
     }
 }
 
 /// A view of a Tensor within the file.
 /// Contains references to data within the full byte-buffer
 /// And is thus a readable view of a single tensor
-#[derive(Debug)]
+#[derive(Debug, PartialEq, Eq)]
 pub struct TensorView<'data> {
     dtype: Dtype,
     shape: Vec<usize>,
     data: &'data [u8],
 }
 
 impl<'data> View for &TensorView<'data> {
@@ -524,15 +565,15 @@
     pub fn data(&self) -> &'data [u8] {
         self.data
     }
 
     /// The various pieces of the data buffer according to the asked slice
     pub fn sliced_data(
         &'data self,
-        slices: Vec<TensorIndexer>,
+        slices: &[TensorIndexer],
     ) -> Result<SliceIterator<'data>, InvalidSlice> {
         SliceIterator::new(self, slices)
     }
 }
 
 /// A single tensor information.
 /// Endianness is assumed to be little endian
@@ -600,14 +641,125 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::slice::IndexOp;
+    use proptest::prelude::*;
+
+    const MAX_DIMENSION: usize = 8;
+    const MAX_SIZE: usize = 8;
+    const MAX_TENSORS: usize = 8;
+
+    fn arbitrary_dtype() -> impl Strategy<Value = Dtype> {
+        prop_oneof![
+            Just(Dtype::BOOL),
+            Just(Dtype::U8),
+            Just(Dtype::I8),
+            Just(Dtype::I16),
+            Just(Dtype::U16),
+            Just(Dtype::I32),
+            Just(Dtype::U32),
+            Just(Dtype::I64),
+            Just(Dtype::U64),
+            Just(Dtype::F16),
+            Just(Dtype::BF16),
+            Just(Dtype::F32),
+            Just(Dtype::F64),
+        ]
+    }
+
+    fn arbitrary_shape() -> impl Strategy<Value = Vec<usize>> {
+        // We do not allow empty shapes or 0 sizes.
+        (1..MAX_DIMENSION).prop_flat_map(|length| prop::collection::vec(1..MAX_SIZE, length))
+    }
+
+    fn arbitrary_metadata() -> impl Strategy<Value = Metadata> {
+        // We generate at least one tensor.
+        (1..MAX_TENSORS)
+            .prop_flat_map(|size| {
+                // Returns a strategy generating `size` data types and shapes.
+                (
+                    prop::collection::vec(arbitrary_dtype(), size),
+                    prop::collection::vec(arbitrary_shape(), size),
+                )
+            })
+            .prop_map(|(dtypes, shapes)| {
+                // Returns a valid metadata object for a random (length, dtypes, shapes) triple.
+                let mut start = 0;
+                let tensors: Vec<TensorInfo> = dtypes
+                    .iter()
+                    .zip(shapes.into_iter())
+                    .map(|(dtype, shape)| {
+                        // This cannot overflow because the size of
+                        // the vector and elements are so small.
+                        let length: usize = shape.iter().product();
+                        let end = start + length * dtype.size();
+                        let tensor = TensorInfo {
+                            dtype: *dtype,
+                            shape,
+                            data_offsets: (start, end),
+                        };
+                        start = end;
+                        tensor
+                    })
+                    .collect();
+                let index_map = (0..tensors.len())
+                    .map(|index| (format!("t.{index}"), index))
+                    .collect();
+                Metadata {
+                    metadata: None,
+                    tensors,
+                    index_map,
+                }
+            })
+    }
+
+    /// This method returns the size of the data corresponding to the metadata. It
+    /// assumes that `metadata` contains at least one tensor, and that tensors are
+    /// ordered by offset in `metadata.tensors`.
+    ///
+    /// # Panics
+    ///
+    /// This method will panic if `metadata` does not contain any tensors.
+    fn data_size(metadata: &Metadata) -> usize {
+        metadata.tensors.last().unwrap().data_offsets.1
+    }
+
+    proptest! {
+        #![proptest_config(ProptestConfig::with_cases(20))]
+
+        #[test]
+        fn test_indexing(metadata in arbitrary_metadata()) {
+            let data = vec![0u8; data_size(&metadata)];
+            let tensors = SafeTensors { metadata, data: &data };
+            for name in tensors.names() {
+                assert!(tensors.tensor(name).is_ok());
+            }
+        }
+        #[test]
+        fn test_roundtrip(metadata in arbitrary_metadata()) {
+            let data: Vec<u8> = (0..data_size(&metadata)).map(|x| x as u8).collect();
+            let before = SafeTensors { metadata, data: &data };
+            let tensors = before.tensors();
+            let bytes = serialize(tensors.iter().map(|(name, view)| (name.to_string(), view)), &None).unwrap();
+
+            let after = SafeTensors::deserialize(&bytes).unwrap();
+
+            // Check that the tensors are the same after deserialization.
+            assert_eq!(before.names().len(), after.names().len());
+            for name in before.names() {
+                let tensor_before = before.tensor(name).unwrap();
+                let tensor_after = after.tensor(name).unwrap();
+                assert_eq!(tensor_after.data().as_ptr() as usize % tensor_after.dtype().size(), 0);
+                assert_eq!(tensor_before, tensor_after);
+            }
+        }
+    }
 
     #[test]
     fn test_serialization() {
         let data: Vec<u8> = vec![0.0f32, 1.0, 2.0, 3.0, 4.0, 5.0]
             .into_iter()
             .flat_map(|f| f.to_le_bytes())
             .collect();
@@ -632,34 +784,37 @@
 
     #[test]
     fn test_serialization_forced_alignement() {
         let data: Vec<u8> = vec![0.0f32, 1.0, 2.0, 3.0, 4.0, 5.0]
             .into_iter()
             .flat_map(|f| f.to_le_bytes())
             .collect();
-        let shape = vec![1, 2, 3];
+        let shape = vec![1, 1, 2, 3];
         let attn_0 = TensorView::new(Dtype::F32, shape, &data).unwrap();
         let metadata: HashMap<String, TensorView> =
             // Smaller string to force misalignment compared to previous test.
             [("attn0".to_string(), attn_0)].into_iter().collect();
 
         let out = serialize(&metadata, &None).unwrap();
         assert_eq!(
             out,
             [
-                70, 0, 0, 0, 0, 0, 0, 0, 123, 34, 97, 116, 116, 110, 48, 34, 58, 123, 34, 100, 116,
+                72, 0, 0, 0, 0, 0, 0, 0, 123, 34, 97, 116, 116, 110, 48, 34, 58, 123, 34, 100, 116,
                 121, 112, 101, 34, 58, 34, 70, 51, 50, 34, 44, 34, 115, 104, 97, 112, 101, 34, 58,
-                91, 49, 44, 50, 44, 51, 93, 44, 34, 100, 97, 116, 97, 95, 111, 102, 102, 115, 101,
+                91, 49, 44, 49, 44, 50, 44, 51, 93, 44, 34, 100, 97, 116, 97, 95, 111, 102, 102,
                 // All the 32 are forcing alignement of the tensor data for casting to f32, f64
                 // etc..
-                116, 115, 34, 58, 91, 48, 44, 50, 52, 93, 125, 125, 32, 32, 32, 32, 32, 32, 32, 0,
-                0, 0, 0, 0, 0, 128, 63, 0, 0, 0, 64, 0, 0, 64, 64, 0, 0, 128, 64, 0, 0, 160, 64
-            ]
+                115, 101, 116, 115, 34, 58, 91, 48, 44, 50, 52, 93, 125, 125, 32, 32, 32, 32, 32,
+                32, 32, 0, 0, 0, 0, 0, 0, 128, 63, 0, 0, 0, 64, 0, 0, 64, 64, 0, 0, 128, 64, 0, 0,
+                160, 64
+            ],
         );
-        let _parsed = SafeTensors::deserialize(&out).unwrap();
+        let parsed = SafeTensors::deserialize(&out).unwrap();
+        let tensor = parsed.tensor("attn0").unwrap();
+        assert_eq!(tensor.data().as_ptr() as usize % tensor.dtype().size(), 0);
     }
 
     #[test]
     fn test_slicing() {
         let data: Vec<u8> = vec![0.0f32, 1.0, 2.0, 3.0, 4.0, 5.0]
             .into_iter()
             .flat_map(|f| f.to_le_bytes())
@@ -752,26 +907,43 @@
             let n: usize = shape.iter().product();
             let buffer = &all_data[offset..offset + n * dtype.size()];
             let tensor = TensorView::new(dtype, shape, buffer).unwrap();
             metadata.insert(name, tensor);
             offset += n;
         }
 
-        let filename = format!("./out_{model_id}.bin");
+        let filename = format!("./out_{model_id}.safetensors");
 
         let out = serialize(&metadata, &None).unwrap();
-
         std::fs::write(&filename, out).unwrap();
+        let raw = std::fs::read(&filename).unwrap();
+        let _deserialized = SafeTensors::deserialize(&raw).unwrap();
+        std::fs::remove_file(&filename).unwrap();
 
+        // File api
+        serialize_to_file(&metadata, &None, Path::new(&filename)).unwrap();
         let raw = std::fs::read(&filename).unwrap();
         let _deserialized = SafeTensors::deserialize(&raw).unwrap();
         std::fs::remove_file(&filename).unwrap();
     }
 
     #[test]
+    fn test_empty_shapes_allowed() {
+        let serialized = b"8\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[],\"data_offsets\":[0,4]}}\x00\x00\x00\x00";
+
+        let loaded = SafeTensors::deserialize(serialized).unwrap();
+        assert_eq!(loaded.names(), vec!["test"]);
+        let tensor = loaded.tensor("test").unwrap();
+        assert!(tensor.shape().is_empty());
+        assert_eq!(tensor.dtype(), Dtype::I32);
+        // 4 bytes
+        assert_eq!(tensor.data(), b"\0\0\0\0");
+    }
+
+    #[test]
     fn test_deserialization() {
         let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00";
 
         let loaded = SafeTensors::deserialize(serialized).unwrap();
 
         assert_eq!(loaded.names(), vec!["test"]);
         let tensor = loaded.tensor("test").unwrap();
@@ -821,18 +993,129 @@
             }
             Err(err) => panic!("Unexpected error {err:?}"),
             Ok(_) => panic!("This should not be able to be deserialized"),
         }
     }
 
     #[test]
+    fn test_metadata_incomplete_buffer() {
+        let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00extra_bogus_data_for_polyglot_file";
+
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::MetadataIncompleteBuffer) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+
+        // Missing data in the buffer
+        let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"; // <--- missing 2 bytes
+
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::MetadataIncompleteBuffer) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
+
+    #[test]
     fn test_header_too_large() {
         let serialized = b"<\x00\x00\x00\x00\xff\xff\xff{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00";
 
         match SafeTensors::deserialize(serialized) {
             Err(SafeTensorError::HeaderTooLarge) => {
                 // Yes we have the correct error
             }
             _ => panic!("This should not be able to be deserialized"),
         }
     }
+
+    #[test]
+    fn test_header_too_small() {
+        let serialized = b"";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::HeaderTooSmall) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
+
+    #[test]
+    fn test_invalid_header_length() {
+        let serialized = b"<\x00\x00\x00\x00\x00\x00\x00";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::InvalidHeaderLength) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
+
+    #[test]
+    fn test_invalid_header_non_utf8() {
+        let serialized = b"\x01\x00\x00\x00\x00\x00\x00\x00\xff";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::InvalidHeader) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
+
+    #[test]
+    fn test_invalid_header_not_json() {
+        let serialized = b"\x01\x00\x00\x00\x00\x00\x00\x00{";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::InvalidHeaderDeserialization) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
+
+    #[test]
+    fn test_zero_sized_tensor() {
+        let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,0],\"data_offsets\":[0, 0]}}";
+        let loaded = SafeTensors::deserialize(serialized).unwrap();
+
+        assert_eq!(loaded.names(), vec!["test"]);
+        let tensor = loaded.tensor("test").unwrap();
+        assert_eq!(tensor.shape(), vec![2, 0]);
+        assert_eq!(tensor.dtype(), Dtype::I32);
+        assert_eq!(tensor.data(), b"");
+    }
+
+    #[test]
+    fn test_invalid_info() {
+        let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0, 4]}}";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::TensorInvalidInfo) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
+
+    #[test]
+    fn test_validation_overflow() {
+        // u64::MAX =  18_446_744_073_709_551_615u64
+        // Overflow the shape calculation.
+        let serialized = b"O\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,18446744073709551614],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::ValidationOverflow) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+        // u64::MAX =  18_446_744_073_709_551_615u64
+        // Overflow the num_elements * total shape.
+        let serialized = b"N\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,9223372036854775807],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00";
+        match SafeTensors::deserialize(serialized) {
+            Err(SafeTensorError::ValidationOverflow) => {
+                // Yes we have the correct error
+            }
+            _ => panic!("This should not be able to be deserialized"),
+        }
+    }
 }
```

### Comparing `safetensors-0.3.0rc1/setup.cfg` & `safetensors-0.3.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.0rc1/setup.py` & `safetensors-0.3.1rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,41 +6,44 @@
 
 # IMPORTANT:
 # 1. all dependencies should be listed here with their version requirements if any
 _deps = [
     "black==22.3",  # after updating to black 2023, also update Python version in pyproject.toml to 3.7
     "click==8.0.4",
     "flake8>=3.8.3",
-    "flax",
-    "h5py",
-    "huggingface_hub",
+    "flax>=0.6.3",
+    "h5py>=3.7.0",
+    "huggingface_hub>=0.12.1",
     "isort>=5.5.4",
-    "jax",
-    "numpy",
-    "setuptools_rust",
-    "pytest",
-    "pytest-benchmark",
-    "tensorflow",
-    "torch",
-    "paddlepaddle",
+    "jax>=0.3.25",
+    "jaxlib>=0.3.25",
+    "numpy>=1.21.6",
+    "setuptools_rust>=1.5.2",
+    "pytest>=7.2.0",
+    "pytest-benchmark>=4.0.0",
+    "tensorflow>=2.11.0",
+    "torch>=1.10",
+    "paddlepaddle>=2.4.1",
+    "python-afl>=0.7.3",
+    "hypothesis>=6.70.2",
 ]
 
 
 deps = {b: a for a, b in (re.findall(r"^(([^!=<>~ ]+)(?:[!=<>~ ].*)?$)", x)[0] for x in _deps)}
 
 
 def deps_list(*pkgs):
     return [deps[pkg] for pkg in pkgs]
 
 
 extras = {}
 extras["torch"] = deps_list("torch")
 extras["numpy"] = deps_list("numpy")
 extras["tensorflow"] = deps_list("tensorflow")
-extras["jax"] = deps_list("jax", "flax")
+extras["jax"] = deps_list("jax", "flax", "jaxlib")
 extras["paddlepaddle"] = deps_list("paddlepaddle")
 extras["quality"] = deps_list("black", "isort", "flake8", "click")
 extras["testing"] = (
     deps_list("setuptools_rust", "huggingface_hub", "pytest", "pytest-benchmark", "h5py") + extras["numpy"]
 )
 extras["all"] = (
     extras["torch"]
```

### Comparing `safetensors-0.3.0rc1/src/lib.rs` & `safetensors-0.3.1rc1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -367,18 +367,23 @@
                 // Untyped storage only exists for versions over 1.11.0
                 // Same for torch.asarray which is necessary for zero-copy tensor
                 if version >= Version::new(1, 11, 0) {
                     // storage = torch.ByteStorage.from_file(filename, shared=False, size=size).untyped()
                     let py_filename: PyObject = filename.into_py(py);
                     let size: PyObject = buffer.len().into_py(py);
                     let shared: PyObject = false.into_py(py);
-                    let kwargs = [(intern!(py, "shared"), shared), (intern!(py, "size"), size)]
-                        .into_py_dict(py);
+                    let (size_name, storage_name) = if version >= Version::new(2, 0, 0) {
+                        (intern!(py, "nbytes"), intern!(py, "UntypedStorage"))
+                    } else {
+                        (intern!(py, "size"), intern!(py, "ByteStorage"))
+                    };
+                    let kwargs =
+                        [(intern!(py, "shared"), shared), (size_name, size)].into_py_dict(py);
                     let storage = module
-                        .getattr(intern!(py, "ByteStorage"))?
+                        .getattr(storage_name)?
                         .getattr(intern!(py, "from_file"))?
                         .call((py_filename,), Some(kwargs))?;
 
                     let untyped: &PyAny = match storage.getattr(intern!(py, "untyped")) {
                         Ok(untyped) => untyped,
                         Err(_) => storage.getattr(intern!(py, "_untyped"))?,
                     };
@@ -704,15 +709,15 @@
                         SafetensorError::new_err(format!("Error preparing tensor view: {e:?}"))
                     })?;
                 let slices: Vec<TensorIndexer> = slices
                     .into_iter()
                     .map(slice_to_indexer)
                     .collect::<Result<_, _>>()?;
 
-                let iterator = tensor.sliced_data(slices.clone()).map_err(|e| {
+                let iterator = tensor.sliced_data(&slices).map_err(|e| {
                     SafetensorError::new_err(format!(
                         "Error during slicing {slices:?} vs {:?}:  {:?}",
                         self.info.shape, e
                     ))
                 })?;
                 let newshape = iterator.newshape();
 
@@ -804,24 +809,34 @@
     Python::with_gil(|py| -> PyResult<PyObject> {
         let module: &PyModule = match framework {
             Framework::Pytorch => TORCH_MODULE.get(py),
             _ => NUMPY_MODULE.get(py),
         }
         .ok_or_else(|| SafetensorError::new_err(format!("Could not find module {framework:?}",)))?
         .as_ref(py);
-        let frombuffer = module.getattr(intern!(py, "frombuffer"))?;
         let dtype: PyObject = get_pydtype(module, dtype)?;
-        let kwargs = [
-            (intern!(py, "buffer"), array),
-            (intern!(py, "dtype"), dtype),
-        ]
-        .into_py_dict(py);
-        let tensor = frombuffer.call((), Some(kwargs))?;
+        let count: usize = shape.iter().product();
         let shape = shape.to_vec();
         let shape: PyObject = shape.into_py(py);
+        let tensor = if count == 0 {
+            // Torch==1.10 does not allow frombuffer on empty buffers so we create
+            // the tensor manually.
+            let zeros = module.getattr(intern!(py, "zeros"))?;
+            let args = (shape.clone(),);
+            let kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict(py);
+            zeros.call(args, Some(kwargs))?
+        } else {
+            let frombuffer = module.getattr(intern!(py, "frombuffer"))?;
+            let kwargs = [
+                (intern!(py, "buffer"), array),
+                (intern!(py, "dtype"), dtype),
+            ]
+            .into_py_dict(py);
+            frombuffer.call((), Some(kwargs))?
+        };
         let mut tensor: &PyAny = tensor.getattr(intern!(py, "reshape"))?.call1((shape,))?;
         let tensor = match framework {
             Framework::Flax => {
                 let module = Python::with_gil(|py| -> PyResult<&Py<PyModule>> {
                     let module = PyModule::import(py, intern!(py, "jax"))?;
                     Ok(FLAX_MODULE.get_or_init(py, || module.into()))
                 })?
```

