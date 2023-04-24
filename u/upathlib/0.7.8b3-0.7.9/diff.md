# Comparing `tmp/upathlib-0.7.8b3.tar.gz` & `tmp/upathlib-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.8b3.tar", last modified: Thu Apr 20 04:32:59 2023, max compression
+gzip compressed data, was "upathlib-0.7.9.tar", last modified: Mon Apr 24 18:30:06 2023, max compression
```

## Comparing `upathlib-0.7.8b3.tar` & `upathlib-0.7.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.8b3/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.8b3/README.rst
--rw-r--r--   0        0        0     1726 2023-04-15 03:57:22.660027 upathlib-0.7.8b3/pyproject.toml
--rw-r--r--   0        0        0     2320 2023-04-20 04:26:10.814627 upathlib-0.7.8b3/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4694 2023-04-20 04:26:10.454625 upathlib-0.7.8b3/src/upathlib/_blob.py
--rw-r--r--   0        0        0    10997 2023-04-18 03:08:39.636189 upathlib-0.7.8b3/src/upathlib/_local.py
--rw-r--r--   0        0        0     7935 2023-04-17 17:40:01.495217 upathlib-0.7.8b3/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34468 2023-04-17 17:41:36.641457 upathlib-0.7.8b3/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.8b3/src/upathlib/azure.py
--rw-r--r--   0        0        0    26061 2023-04-20 04:26:10.804627 upathlib-0.7.8b3/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.8b3/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.8b3/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.7.8b3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.9/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.9/README.rst
+-rw-r--r--   0        0        0     1726 2023-04-24 18:14:03.529696 upathlib-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     2317 2023-04-24 18:28:07.086273 upathlib-0.7.9/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4694 2023-04-20 04:34:46.179551 upathlib-0.7.9/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    10997 2023-04-20 04:34:46.179551 upathlib-0.7.9/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.7.9/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34513 2023-04-24 18:21:32.197286 upathlib-0.7.9/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.9/src/upathlib/azure.py
+-rw-r--r--   0        0        0    26106 2023-04-24 18:21:32.197286 upathlib-0.7.9/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.9/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.9/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 upathlib-0.7.9/PKG-INFO
```

### Comparing `upathlib-0.7.8b3/LICENSE` & `upathlib-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/README.rst` & `upathlib-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/pyproject.toml` & `upathlib-0.7.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
     "filelock >= 3.9.1",
     "deprecation",
     "tqdm",
     "typing-extensions",
-    "mpservice >= 0.11.9",
+    "mpservice >= 0.12.5",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
```

### Comparing `upathlib-0.7.8b3/src/upathlib/__init__.py` & `upathlib-0.7.9/src/upathlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.8b3"
-
+__version__ = "0.7.9"
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalPathType, LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
```

### Comparing `upathlib-0.7.8b3/src/upathlib/_blob.py` & `upathlib-0.7.9/src/upathlib/_blob.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/src/upathlib/_local.py` & `upathlib-0.7.9/src/upathlib/_local.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/src/upathlib/_tests.py` & `upathlib-0.7.9/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/src/upathlib/_upath.py` & `upathlib-0.7.9/src/upathlib/_upath.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 from io import BufferedReader, UnsupportedOperation
 from typing import (
     Any,
     Callable,
     Optional,
 )
 
-from mpservice.util import MAX_THREADS, get_shared_thread_pool
+from mpservice.concurrent.futures import get_shared_thread_pool
+from mpservice.threading import MAX_THREADS
 from tqdm.auto import tqdm
 from typing_extensions import Self
 
 from .serializer import (
     JsonSerializer,
     PickleSerializer,
     ZPickleSerializer,
```

### Comparing `upathlib-0.7.8b3/src/upathlib/azure.py` & `upathlib-0.7.9/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/src/upathlib/gcs.py` & `upathlib-0.7.9/src/upathlib/gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 # `google.cloud` is repo python-cloud-core.
 from google.cloud.storage.retry import (
     DEFAULT_RETRY,
     DEFAULT_RETRY_IF_GENERATION_SPECIFIED,
     ConditionalRetryPolicy,
     is_generation_specified,
 )
-from mpservice.util import MAX_THREADS, get_shared_thread_pool
+from mpservice.concurrent.futures import get_shared_thread_pool
+from mpservice.threading import MAX_THREADS
 from typing_extensions import Self
 
 from ._blob import BlobUpath, LocalPathType, _resolve_local_path
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
 # To see retry info, uncomment the following. The printout is typically not overwhelming.
 # logging.getLogger('google.api_core.retry').setLevel(logging.DEBUG)
```

### Comparing `upathlib-0.7.8b3/src/upathlib/serializer.py` & `upathlib-0.7.9/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.8b3/PKG-INFO` & `upathlib-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.8b3
+Version: 0.7.9
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: filelock >= 3.9.1
 Requires-Dist: deprecation
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
-Requires-Dist: mpservice >= 0.11.9
+Requires-Dist: mpservice >= 0.12.5
 Requires-Dist: azure-storage-blob >=12.9.0,<13.0 ; extra == "abs"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
 Requires-Dist: google-auth ; extra == "gcs"
 Requires-Dist: google-api-python-client >=2.13.9,<3.0 ; extra == "gcs"
 Requires-Dist: google-cloud-storage >=2.0,<3.0 ; extra == "gcs"
```

