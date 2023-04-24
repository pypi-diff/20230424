# Comparing `tmp/biglist-0.8.0b1.tar.gz` & `tmp/biglist-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.8.0b1.tar", last modified: Mon Apr 17 15:38:20 2023, max compression
+gzip compressed data, was "biglist-0.8.1.tar", last modified: Mon Apr 24 18:37:43 2023, max compression
```

## Comparing `biglist-0.8.0b1.tar` & `biglist-0.8.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.0b1/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.8.0b1/README.rst
--rw-r--r--   0        0        0     1623 2023-04-15 03:17:01.146252 biglist-0.8.0b1/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-17 15:35:58.651653 biglist-0.8.0b1/src/biglist/__init__.py
--rw-r--r--   0        0        0    17990 2023-04-15 03:17:01.146252 biglist-0.8.0b1/src/biglist/_base.py
--rw-r--r--   0        0        0    44414 2023-04-15 03:17:01.146252 biglist-0.8.0b1/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34773 2023-04-17 15:34:16.400044 biglist-0.8.0b1/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-14 07:17:29.111106 biglist-0.8.0b1/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.0b1/src/biglist/py.typed
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 biglist-0.8.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.1/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.8.1/README.rst
+-rw-r--r--   0        0        0     1527 2023-04-24 18:36:06.413180 biglist-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2215 2023-04-24 18:28:48.591995 biglist-0.8.1/src/biglist/__init__.py
+-rw-r--r--   0        0        0    18004 2023-04-24 18:29:53.379253 biglist-0.8.1/src/biglist/_base.py
+-rw-r--r--   0        0        0    44435 2023-04-24 18:32:33.472154 biglist-0.8.1/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34773 2023-04-18 03:17:34.278504 biglist-0.8.1/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-14 07:17:29.111106 biglist-0.8.1/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.1/src/biglist/py.typed
+-rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 biglist-0.8.1/PKG-INFO
```

### Comparing `biglist-0.8.0b1/LICENSE` & `biglist-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0b1/README.rst` & `biglist-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0b1/pyproject.toml` & `biglist-0.8.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 [project]
 name = "biglist"
 authors = [
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
-    "upathlib >= 0.7.7",
+    "upathlib >= 0.7.9",
     "deprecation",
-    "mpservice >= 0.11.9",
+    "mpservice >= 0.12.5",
     "pyarrow >= 10.0.0",
     "typing-extensions",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
@@ -35,34 +35,30 @@
 lz4 = ["lz4"]
 doc = [
     "sphinx",
     "numpydoc",
     "pydata-sphinx-theme",
 ]
 gcs = [
-    "upathlib[gcs] >= 0.7.7",
+    "upathlib[gcs] >= 0.7.9",
     "google-auth",
 ]
-parquet = []
 test = [
     "boltons",
     "mypy",
     "ruff",
     "pytest-asyncio",
 ]
 
-# `parquet` option became empty in 0.7.5 because `arrow` became mandatory.
-# To be removed later.
-
 
 # See https://beta.ruff.rs/docs/rules/
 [tool.ruff]
 target-version = "py38"
 select = ["E", "F", "S", "I001"]  # isort
-ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S608"]
+ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S603", "S607", "S608"]
 
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 
 [tool.pytest.ini_options]
```

### Comparing `biglist-0.8.0b1/src/biglist/__init__.py` & `biglist-0.8.1/src/biglist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.8.0b1"
+__version__ = "0.8.1"
```

### Comparing `biglist-0.8.0b1/src/biglist/_base.py` & `biglist-0.8.1/src/biglist/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from abc import abstractmethod
 from collections.abc import Iterator
 from typing import (
     Optional,
     TypeVar,
 )
 
-from mpservice.util import get_shared_thread_pool
+from mpservice.concurrent.futures import get_shared_thread_pool
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
 from ._util import Element, Seq
 
 logger = logging.getLogger(__name__)
```

### Comparing `biglist-0.8.0b1/src/biglist/_biglist.py` & `biglist-0.8.1/src/biglist/_biglist.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
         In the processes, use independent ``Biglist`` objects that point to the same "path".
         Each of the objects will maintain its own in-memory buffer and save its own files once the buffer
         fills up. Remember to :meth:`flush` at the end of work in each process.
 
         .. note:: Use the "spawn" method to start processes.
             In ``multiprocessing``, look for the method `get_context <https://docs.python.org/3/library/multiprocessing.html#multiprocessing.get_context>`_.
             In ``concurrent.futures.ProcessPoolExecutor``, look for the parameter `mp_context <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ProcessPoolExecutor>`_.
-            Also check out `mpservice.util.MP_SPAWN_CTX <https://mpservice.readthedocs.io/en/latest/util.html#mpservice.util.MP_SPAWN_CTX>`_.
+            Also check out `mpservice.multiprocesing.MP_SPAWN_CTX <https://mpservice.readthedocs.io/en/latest/util.html#mpservice.multiprocessing.MP_SPAWN_CTX>`_.
         """
         self._append_buffer.append(x)
         self._flushed = False  # This is about `flush`, not `_flush`.
         if len(self._append_buffer) >= self.batch_size:
             self._flush()
 
     def extend(self, x: Iterable[Element]) -> None:
```

### Comparing `biglist-0.8.0b1/src/biglist/_parquet.py` & `biglist-0.8.1/src/biglist/_parquet.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0b1/src/biglist/_util.py` & `biglist-0.8.1/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.8.0b1/PKG-INFO` & `biglist-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.8.0b1
+Version: 0.8.1
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: upathlib >= 0.7.7
+Requires-Dist: upathlib >= 0.7.9
 Requires-Dist: deprecation
-Requires-Dist: mpservice >= 0.11.9
+Requires-Dist: mpservice >= 0.12.5
 Requires-Dist: pyarrow >= 10.0.0
 Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
-Requires-Dist: upathlib[gcs] >= 0.7.7 ; extra == "gcs"
+Requires-Dist: upathlib[gcs] >= 0.7.9 ; extra == "gcs"
 Requires-Dist: google-auth ; extra == "gcs"
 Requires-Dist: lz4 ; extra == "lz4"
 Requires-Dist: boltons ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: zstandard ; extra == "zstandard"
 Project-URL: Source, https://github.com/zpz/biglist
 Provides-Extra: doc
 Provides-Extra: gcs
 Provides-Extra: lz4
-Provides-Extra: parquet
 Provides-Extra: test
 Provides-Extra: zstandard
 
 biglist
 =======
 
 The package ``biglist`` provides persisted, out-of-memory Python data structures
```

