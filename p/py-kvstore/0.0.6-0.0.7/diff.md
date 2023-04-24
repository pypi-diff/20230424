# Comparing `tmp/py_kvstore-0.0.6.tar.gz` & `tmp/py_kvstore-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_kvstore-0.0.6.tar", last modified: Wed Apr 19 21:13:07 2023, max compression
+gzip compressed data, was "py_kvstore-0.0.7.tar", last modified: Mon Apr 24 20:23:50 2023, max compression
```

## Comparing `py_kvstore-0.0.6.tar` & `py_kvstore-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-19 21:13:07.637548 py_kvstore-0.0.6/
--rw-r--r--   0 reece     (1000) reece     (1001)     2180 2023-04-19 21:13:07.637548 py_kvstore-0.0.6/PKG-INFO
--rw-r--r--   0 reece     (1000) reece     (1001)     1531 2023-04-19 21:12:46.000000 py_kvstore-0.0.6/README.md
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-19 21:13:07.637548 py_kvstore-0.0.6/py_kvstore/
--rw-r--r--   0 reece     (1000) reece     (1001)       78 2023-04-18 04:17:04.000000 py_kvstore-0.0.6/py_kvstore/__init__.py
--rw-r--r--   0 reece     (1000) reece     (1001)     7960 2023-04-19 21:13:01.000000 py_kvstore-0.0.6/py_kvstore/py_kvstore.py
--rw-r--r--   0 reece     (1000) reece     (1001)     3401 2023-04-19 20:00:40.000000 py_kvstore-0.0.6/py_kvstore/test.py
-drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-19 21:13:07.637548 py_kvstore-0.0.6/py_kvstore.egg-info/
--rw-r--r--   0 reece     (1000) reece     (1001)     2180 2023-04-19 21:13:07.000000 py_kvstore-0.0.6/py_kvstore.egg-info/PKG-INFO
--rw-r--r--   0 reece     (1000) reece     (1001)      221 2023-04-19 21:13:07.000000 py_kvstore-0.0.6/py_kvstore.egg-info/SOURCES.txt
--rw-r--r--   0 reece     (1000) reece     (1001)        1 2023-04-19 21:13:07.000000 py_kvstore-0.0.6/py_kvstore.egg-info/dependency_links.txt
--rw-r--r--   0 reece     (1000) reece     (1001)       11 2023-04-19 21:13:07.000000 py_kvstore-0.0.6/py_kvstore.egg-info/top_level.txt
--rw-r--r--   0 reece     (1000) reece     (1001)       38 2023-04-19 21:13:07.637548 py_kvstore-0.0.6/setup.cfg
--rw-r--r--   0 reece     (1000) reece     (1001)      966 2023-04-19 21:00:10.000000 py_kvstore-0.0.6/setup.py
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-24 20:23:50.785502 py_kvstore-0.0.7/
+-rw-r--r--   0 reece     (1000) reece     (1001)     2250 2023-04-24 20:23:50.785502 py_kvstore-0.0.7/PKG-INFO
+-rw-r--r--   0 reece     (1000) reece     (1001)     1601 2023-04-19 21:53:16.000000 py_kvstore-0.0.7/README.md
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-24 20:23:50.785502 py_kvstore-0.0.7/py_kvstore/
+-rw-r--r--   0 reece     (1000) reece     (1001)       78 2023-04-18 04:17:04.000000 py_kvstore-0.0.7/py_kvstore/__init__.py
+-rw-r--r--   0 reece     (1000) reece     (1001)     8016 2023-04-24 20:23:30.000000 py_kvstore-0.0.7/py_kvstore/py_kvstore.py
+-rw-r--r--   0 reece     (1000) reece     (1001)     3401 2023-04-24 20:07:49.000000 py_kvstore-0.0.7/py_kvstore/test.py
+drwxr-xr-x   0 reece     (1000) reece     (1001)        0 2023-04-24 20:23:50.785502 py_kvstore-0.0.7/py_kvstore.egg-info/
+-rw-r--r--   0 reece     (1000) reece     (1001)     2250 2023-04-24 20:23:50.000000 py_kvstore-0.0.7/py_kvstore.egg-info/PKG-INFO
+-rw-r--r--   0 reece     (1000) reece     (1001)      221 2023-04-24 20:23:50.000000 py_kvstore-0.0.7/py_kvstore.egg-info/SOURCES.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)        1 2023-04-24 20:23:50.000000 py_kvstore-0.0.7/py_kvstore.egg-info/dependency_links.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)       11 2023-04-24 20:23:50.000000 py_kvstore-0.0.7/py_kvstore.egg-info/top_level.txt
+-rw-r--r--   0 reece     (1000) reece     (1001)       38 2023-04-24 20:23:50.785502 py_kvstore-0.0.7/setup.cfg
+-rw-r--r--   0 reece     (1000) reece     (1001)      966 2023-04-24 20:23:48.000000 py_kvstore-0.0.7/setup.py
```

### Comparing `py_kvstore-0.0.6/PKG-INFO` & `py_kvstore-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_kvstore
-Version: 0.0.6
+Version: 0.0.7
 Summary: A key value store
 Home-page: https://github.com/Reecepbcups/py_kvstore
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -12,20 +12,32 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
-# py_kvstore
+# Python KVStore
+
+[pypi py-kvstore](https://pypi.org/project/py-kvstore/)
+
+---
 
 A simple Key-Value store (similar to redis) built in python.
 
 Sets can expire, not expire, and be saved with any arbitrary data. So you can set it as a JSON string, a dict, int, or any other value. It is up to the developer to implement and parse types correctly.
 
+---
+
+## Projects Using
+
+- [CosmosSDK Endpoint Cache](https://github.com/Reecepbcups/cosmos-endpoint-cache)
+
+---
+
 ## Notable Features
 
 ```py
 # create a new KVStore
 kv1 = KVStore(name="transactions", dump_dir="/home/reece/kvstores")
 
 # Set a key. Defaults to -1 timeout (no timeout)
@@ -59,11 +71,8 @@
 # clear the store
 kv1.clear()
 
 # Load the previous dump from file
 kv1.load()
 ```
 
-## Example Repos using this
-
-- [Cosmos Endpoint Cache](https://github.com/Reecepbcups/cosmos-endpoint-cache)
```

### Comparing `py_kvstore-0.0.6/README.md` & `py_kvstore-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,25 @@
-# py_kvstore
+# Python KVStore
+
+[pypi py-kvstore](https://pypi.org/project/py-kvstore/)
+
+---
 
 A simple Key-Value store (similar to redis) built in python.
 
 Sets can expire, not expire, and be saved with any arbitrary data. So you can set it as a JSON string, a dict, int, or any other value. It is up to the developer to implement and parse types correctly.
 
+---
+
+## Projects Using
+
+- [CosmosSDK Endpoint Cache](https://github.com/Reecepbcups/cosmos-endpoint-cache)
+
+---
+
 ## Notable Features
 
 ```py
 # create a new KVStore
 kv1 = KVStore(name="transactions", dump_dir="/home/reece/kvstores")
 
 # Set a key. Defaults to -1 timeout (no timeout)
@@ -40,11 +52,7 @@
 
 # clear the store
 kv1.clear()
 
 # Load the previous dump from file
 kv1.load()
 ```
-
-## Example Repos using this
-
-- [Cosmos Endpoint Cache](https://github.com/Reecepbcups/cosmos-endpoint-cache)
```

### Comparing `py_kvstore-0.0.6/py_kvstore/py_kvstore.py` & `py_kvstore-0.0.7/py_kvstore/py_kvstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # Do this with a local dictionary. have a .set method which sets a key, value, and timeout.
 # if no timeout is specified, set it as -1.
 
 import json
 import os
 import re as regex
 import time
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
 
 
 class StoreType(Enum):
     PAIR = "pair"
     HASHSET = "hashset"
 
     def __str__(self):
         return self.value
 
 
 @dataclass
 class Pair:
-    value: Any
-    timeout: int
+    value: Any = ""
+    timeout: int = 0
     store_type: str = str(StoreType.PAIR)
 
     def toJSON(self):
         return {
             "value": self.value,
             "timeout": self.timeout,
             "ttl_seconds": self.get_ttl_seconds(),
@@ -40,24 +40,24 @@
     @staticmethod
     def fromJSON(json: dict):
         return Pair(json["value"], json["timeout"])
 
 
 @dataclass
 class HashSet(Pair):
-    value: dict[str, Any]
-    timeout: int
+    value: Dict[str, Any] = field(default_factory=dict)
+    timeout: int = 0
     store_type: str = str(StoreType.HASHSET)
 
 
 class KVStore:
     # TODO: Specify in memory or on the disk (slower, but better for large data sets)
     def __init__(self, name: Optional[str] = None, dump_dir: str = ""):
         self.name = name
-        self.store: dict[str, Pair] = {}
+        self.store: Dict[str, Pair] = {}
 
         self.dump_dir = current_dir
         if len(dump_dir) > 0:
             self.dump_dir = dump_dir
 
     def get_dump_dir(self):
         return self.dump_dir
```

### Comparing `py_kvstore-0.0.6/py_kvstore/test.py` & `py_kvstore-0.0.7/py_kvstore/test.py`

 * *Files identical despite different names*

### Comparing `py_kvstore-0.0.6/py_kvstore.egg-info/PKG-INFO` & `py_kvstore-0.0.7/py_kvstore.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-kvstore
-Version: 0.0.6
+Version: 0.0.7
 Summary: A key value store
 Home-page: https://github.com/Reecepbcups/py_kvstore
 Author: Reece Willims
 Author-email: reecepbcups@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -12,20 +12,32 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
-# py_kvstore
+# Python KVStore
+
+[pypi py-kvstore](https://pypi.org/project/py-kvstore/)
+
+---
 
 A simple Key-Value store (similar to redis) built in python.
 
 Sets can expire, not expire, and be saved with any arbitrary data. So you can set it as a JSON string, a dict, int, or any other value. It is up to the developer to implement and parse types correctly.
 
+---
+
+## Projects Using
+
+- [CosmosSDK Endpoint Cache](https://github.com/Reecepbcups/cosmos-endpoint-cache)
+
+---
+
 ## Notable Features
 
 ```py
 # create a new KVStore
 kv1 = KVStore(name="transactions", dump_dir="/home/reece/kvstores")
 
 # Set a key. Defaults to -1 timeout (no timeout)
@@ -59,11 +71,8 @@
 # clear the store
 kv1.clear()
 
 # Load the previous dump from file
 kv1.load()
 ```
 
-## Example Repos using this
-
-- [Cosmos Endpoint Cache](https://github.com/Reecepbcups/cosmos-endpoint-cache)
```

### Comparing `py_kvstore-0.0.6/setup.py` & `py_kvstore-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # pip install twine
 # python setup.py bdist
 # twine upload -r py_kvstore dist/*
 
 setup(
     name="py_kvstore",
-    version="0.0.6",
+    version="0.0.7",
     description="A key value store",
     url="https://github.com/Reecepbcups/py_kvstore",
     author="Reece Willims",
     author_email="reecepbcups@gmail.com",
     license="Apache 2.0",
     packages=["py_kvstore"],
     install_requires=[],
```

