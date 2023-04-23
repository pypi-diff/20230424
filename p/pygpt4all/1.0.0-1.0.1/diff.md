# Comparing `tmp/pygpt4all-1.0.0.tar.gz` & `tmp/pygpt4all-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt4all-1.0.0.tar", last modified: Sun Apr 23 07:28:23 2023, max compression
+gzip compressed data, was "pygpt4all-1.0.1.tar", last modified: Sun Apr 23 23:25:20 2023, max compression
```

## Comparing `pygpt4all-1.0.0.tar` & `pygpt4all-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:28:23.128749 pygpt4all-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 07:28:12.000000 pygpt4all-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-23 07:28:23.128749 pygpt4all-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 07:28:12.000000 pygpt4all-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:28:23.128749 pygpt4all-1.0.0/pygpt4all.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-23 07:28:23.000000 pygpt4all-1.0.0/pygpt4all.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-23 07:28:23.000000 pygpt4all-1.0.0/pygpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:28:23.000000 pygpt4all-1.0.0/pygpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:28:22.000000 pygpt4all-1.0.0/pygpt4all.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 07:28:23.000000 pygpt4all-1.0.0/pygpt4all.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:28:23.000000 pygpt4all-1.0.0/pygpt4all.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:28:23.128749 pygpt4all-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-23 07:28:12.000000 pygpt4all-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/pygpt4all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/pygpt4all/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/models/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/models/gpt4all_j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/pygpt4all.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/setup.py
```

### Comparing `pygpt4all-1.0.0/LICENSE` & `pygpt4all-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt4all-1.0.0/PKG-INFO` & `pygpt4all-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: pygpt4all
-Version: 1.0.0
+Version: 1.0.1
 Summary: Official Python CPU inference for GPT4All language models based on llama.cpp and ggml
 Author: Abdeladim Sadiki
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyGPT4All
-Official Python CPU inference for [GPT4All](https://github.com/nomic-ai/gpt4all) language models based on [llama.cpp](https://github.com/ggerganov/llama.cpp) and [ggml](https://github.com/ggerganov/ggml).
+Official Python CPU inference for [GPT4All](https://github.com/nomic-ai/gpt4all) language models based on [llama.cpp](https://github.com/ggerganov/llama.cpp) and [ggml](https://github.com/ggerganov/ggml)
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
+[//]: # ([![PyPi version]&#40;https://badgen.net/pypi/v/ptgpt4all&#41;]&#40;https://pypi.org/project/pygpt4all/&#41;)
+
 **NB: Under active development**
 
 # Installation
-1. The easy way is to use the prebuilt wheels
+
 ```bash
 pip install pygpt4all
 ```
 
-2. Build it from source:
-
-```shell
-git clone --recursive https://github.com/nomic-ai/pygpt4all && cd pygpt4all
-pip install .
-```
-
 # Usage
 
 ### GPT4All model
 
-Download a GPT4All model from https://the-eye.eu/public/AI/models/nomic-ai/gpt4all/. The easiest approach is download a file whose name ends in ggml.bin
+Download a GPT4All model from https://the-eye.eu/public/AI/models/nomic-ai/gpt4all/
 
 ```python
 from pygpt4all.models.gpt4all import GPT4All
 
 def new_text_callback(text):
     print(text, end="")
```

### Comparing `pygpt4all-1.0.0/README.md` & `pygpt4all-1.0.1/pygpt4all.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+Metadata-Version: 2.1
+Name: pygpt4all
+Version: 1.0.1
+Summary: Official Python CPU inference for GPT4All language models based on llama.cpp and ggml
+Author: Abdeladim Sadiki
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyGPT4All
-Official Python CPU inference for [GPT4All](https://github.com/nomic-ai/gpt4all) language models based on [llama.cpp](https://github.com/ggerganov/llama.cpp) and [ggml](https://github.com/ggerganov/ggml).
+Official Python CPU inference for [GPT4All](https://github.com/nomic-ai/gpt4all) language models based on [llama.cpp](https://github.com/ggerganov/llama.cpp) and [ggml](https://github.com/ggerganov/ggml)
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
+[//]: # ([![PyPi version]&#40;https://badgen.net/pypi/v/ptgpt4all&#41;]&#40;https://pypi.org/project/pygpt4all/&#41;)
+
 **NB: Under active development**
 
 # Installation
-1. The easy way is to use the prebuilt wheels
+
 ```bash
 pip install pygpt4all
 ```
 
-2. Build it from source:
-
-```shell
-git clone --recursive https://github.com/nomic-ai/pygpt4all && cd pygpt4all
-pip install .
-```
-
 # Usage
 
 ### GPT4All model
 
-Download a GPT4All model from https://the-eye.eu/public/AI/models/nomic-ai/gpt4all/. The easiest approach is download a file whose name ends in ggml.bin
+Download a GPT4All model from https://the-eye.eu/public/AI/models/nomic-ai/gpt4all/
 
 ```python
 from pygpt4all.models.gpt4all import GPT4All
 
 def new_text_callback(text):
     print(text, end="")
```

### Comparing `pygpt4all-1.0.0/pygpt4all.egg-info/PKG-INFO` & `pygpt4all-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,27 @@
-Metadata-Version: 2.1
-Name: pygpt4all
-Version: 1.0.0
-Summary: Official Python CPU inference for GPT4All language models based on llama.cpp and ggml
-Author: Abdeladim Sadiki
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyGPT4All
-Official Python CPU inference for [GPT4All](https://github.com/nomic-ai/gpt4all) language models based on [llama.cpp](https://github.com/ggerganov/llama.cpp) and [ggml](https://github.com/ggerganov/ggml).
+Official Python CPU inference for [GPT4All](https://github.com/nomic-ai/gpt4all) language models based on [llama.cpp](https://github.com/ggerganov/llama.cpp) and [ggml](https://github.com/ggerganov/ggml)
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
+[//]: # ([![PyPi version]&#40;https://badgen.net/pypi/v/ptgpt4all&#41;]&#40;https://pypi.org/project/pygpt4all/&#41;)
+
 **NB: Under active development**
 
 # Installation
-1. The easy way is to use the prebuilt wheels
+
 ```bash
 pip install pygpt4all
 ```
 
-2. Build it from source:
-
-```shell
-git clone --recursive https://github.com/nomic-ai/pygpt4all && cd pygpt4all
-pip install .
-```
-
 # Usage
 
 ### GPT4All model
 
-Download a GPT4All model from https://the-eye.eu/public/AI/models/nomic-ai/gpt4all/. The easiest approach is download a file whose name ends in ggml.bin
+Download a GPT4All model from https://the-eye.eu/public/AI/models/nomic-ai/gpt4all/
 
 ```python
 from pygpt4all.models.gpt4all import GPT4All
 
 def new_text_callback(text):
     print(text, end="")
```

### Comparing `pygpt4all-1.0.0/setup.py` & `pygpt4all-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="pygpt4all",
-    version="1.0.0",
+    version="1.0.1",
     author="Abdeladim Sadiki",
     description="Official Python CPU inference for GPT4All language models based on llama.cpp and ggml",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
```

