# Comparing `tmp/cachetory-2.0.2.tar.gz` & `tmp/cachetory-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.0.2.tar", max compression
+gzip compressed data, was "cachetory-2.0.3.tar", max compression
```

## Comparing `cachetory-2.0.2.tar` & `cachetory-2.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11355 2023-03-08 22:29:11.770466 cachetory-2.0.2/LICENSE
--rw-r--r--   0        0        0    12891 2023-03-08 22:29:11.770466 cachetory-2.0.2/README.md
--rw-r--r--   0        0        0        0 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/__init__.py
--rw-r--r--   0        0        0      999 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     1539 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1727 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2502 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0      993 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     1427 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2361 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2197 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     2041 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     1953 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3644 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3478 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      255 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/private/datetime.py
--rw-r--r--   0        0        0      205 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/py.typed
--rw-r--r--   0        0        0      359 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2170 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      538 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-03-08 22:29:11.770466 cachetory-2.0.2/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3087 2023-03-08 22:29:24.334863 cachetory-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    14563 1970-01-01 00:00:00.000000 cachetory-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-04-24 20:01:45.657741 cachetory-2.0.3/LICENSE
+-rw-r--r--   0        0        0    12891 2023-04-24 20:01:45.657741 cachetory-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0      999 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1727 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2502 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0      993 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     1427 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2361 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2197 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     2041 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     1953 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3644 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3478 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      255 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      205 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2170 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      538 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-04-24 20:01:45.657741 cachetory-2.0.3/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3087 2023-04-24 20:01:59.890282 cachetory-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    14563 1970-01-01 00:00:00.000000 cachetory-2.0.3/PKG-INFO
```

### Comparing `cachetory-2.0.2/LICENSE` & `cachetory-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/README.md` & `cachetory-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/async_/__init__.py` & `cachetory-2.0.3/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/async_/dummy.py` & `cachetory-2.0.3/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/async_/memory.py` & `cachetory-2.0.3/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/async_/redis.py` & `cachetory-2.0.3/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/sync/__init__.py` & `cachetory-2.0.3/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/sync/dummy.py` & `cachetory-2.0.3/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/sync/memory.py` & `cachetory-2.0.3/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/backends/sync/redis.py` & `cachetory-2.0.3/cachetory/backends/sync/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/caches/async_.py` & `cachetory-2.0.3/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/caches/sync.py` & `cachetory-2.0.3/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/decorators/async_.py` & `cachetory-2.0.3/cachetory/decorators/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/decorators/shared.py` & `cachetory-2.0.3/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/decorators/sync.py` & `cachetory-2.0.3/cachetory/decorators/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/interfaces/backends/async_.py` & `cachetory-2.0.3/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/interfaces/backends/private.py` & `cachetory-2.0.3/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/interfaces/backends/sync.py` & `cachetory-2.0.3/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/interfaces/serializers.py` & `cachetory-2.0.3/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/serializers/chained.py` & `cachetory-2.0.3/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/serializers/compressors/zlib.py` & `cachetory-2.0.3/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/serializers/compressors/zstd.py` & `cachetory-2.0.3/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/serializers/noop.py` & `cachetory-2.0.3/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/cachetory/serializers/pickle.py` & `cachetory-2.0.3/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.0.2/pyproject.toml` & `cachetory-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.0.2"
+version = "2.0.3"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `cachetory-2.0.2/PKG-INFO` & `cachetory-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.0.2
+Version: 2.0.3
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.7.0,<4.0.0
```

