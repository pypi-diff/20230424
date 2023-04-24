# Comparing `tmp/microllama-0.4.7.tar.gz` & `tmp/microllama-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microllama-0.4.7.tar", last modified: Wed Apr 12 13:03:48 2023, max compression
+gzip compressed data, was "microllama-0.4.8.tar", last modified: Mon Apr 24 08:31:48 2023, max compression
```

## Comparing `microllama-0.4.7.tar` & `microllama-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       60 2023-03-13 12:38:15.340959 microllama-0.4.7/.dockerignore
--rw-r--r--   0        0        0     3127 2023-03-21 15:46:26.361821 microllama-0.4.7/.gitignore
--rw-r--r--   0        0        0     1066 2023-03-13 12:38:15.341213 microllama-0.4.7/LICENSE
--rw-r--r--   0        0        0     3559 2023-03-19 21:29:23.436615 microllama-0.4.7/README.md
--rw-r--r--   0        0        0      262 2023-03-19 21:29:23.437372 microllama-0.4.7/microllama/Dockerfile
--rw-r--r--   0        0        0     7763 2023-04-12 13:03:32.635581 microllama-0.4.7/microllama/__init__.py
--rw-r--r--   0        0        0    19314 2023-03-14 13:05:44.551702 microllama-0.4.7/microllama/example.source.json
--rw-r--r--   0        0        0     4092 2023-03-20 17:59:23.179760 microllama-0.4.7/microllama/index.html
--rw-r--r--   0        0        0      599 2023-04-12 12:59:15.537398 microllama-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 microllama-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-03-13 12:38:15.340959 microllama-0.4.8/.dockerignore
+-rw-r--r--   0        0        0     3127 2023-03-21 15:46:26.361821 microllama-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1066 2023-03-13 12:38:15.341213 microllama-0.4.8/LICENSE
+-rw-r--r--   0        0        0     3559 2023-03-19 21:29:23.436615 microllama-0.4.8/README.md
+-rw-r--r--   0        0        0      262 2023-03-19 21:29:23.437372 microllama-0.4.8/microllama/Dockerfile
+-rw-r--r--   0        0        0     7764 2023-04-24 08:31:26.019482 microllama-0.4.8/microllama/__init__.py
+-rw-r--r--   0        0        0    19314 2023-03-14 13:05:44.551702 microllama-0.4.8/microllama/example.source.json
+-rw-r--r--   0        0        0     4092 2023-03-20 17:59:23.179760 microllama-0.4.8/microllama/index.html
+-rw-r--r--   0        0        0      599 2023-04-12 12:59:15.537398 microllama-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 microllama-0.4.8/PKG-INFO
```

### Comparing `microllama-0.4.7/.gitignore` & `microllama-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `microllama-0.4.7/LICENSE` & `microllama-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `microllama-0.4.7/README.md` & `microllama-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `microllama-0.4.7/microllama/__init__.py` & `microllama-0.4.8/microllama/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The smallest possible LLM API"""
 
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 
 import inspect
 import json
 import os
 import sys
 from functools import lru_cache
 from typing import Optional, Union
@@ -24,15 +24,15 @@
 FAISS_INDEX_PATH = os.environ.get("FAISS_INDEX_PATH", "faiss_index")
 SOURCE_JSON = os.environ.get("SOURCE_JSON", "source.json")
 MAX_RELATED_DOCUMENTS = int(os.environ.get("MAX_RELATED_DOCUMENTS", 5))
 EXTRA_CONTEXT = os.environ.get(
     "EXTRA_CONTEXT",
     """
         Answer in no more than three sentences. If the answer is not included 
-        in the context, say 'Sorry, this is no answer for this in my sources.'.
+        in the context, say 'Sorry, there is no answer for this in my sources.'.
     """,
 )
 UVICORN_HOST = os.environ.get("UVICORN_HOST", "0.0.0.0")
 UVICORN_PORT = int(os.environ.get("UVICORN_PORT", 8080))
 
 
 def log(msg):
```

### Comparing `microllama-0.4.7/microllama/example.source.json` & `microllama-0.4.8/microllama/example.source.json`

 * *Files identical despite different names*

### Comparing `microllama-0.4.7/microllama/index.html` & `microllama-0.4.8/microllama/index.html`

 * *Files identical despite different names*

### Comparing `microllama-0.4.7/pyproject.toml` & `microllama-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microllama-0.4.7/PKG-INFO` & `microllama-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microllama
-Version: 0.4.7
+Version: 0.4.8
 Summary: The smallest possible LLM API
 Author-email: Tom Dyson <tom@torchbox.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: langchain
 Requires-Dist: tiktoken
 Requires-Dist: faiss-cpu
```

