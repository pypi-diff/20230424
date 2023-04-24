# Comparing `tmp/adt_cache-0.0.5.tar.gz` & `tmp/adt_cache-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adt_cache-0.0.5.tar", last modified: Mon Apr 24 11:58:44 2023, max compression
+gzip compressed data, was "dist/adt_cache-0.0.6.tar", last modified: Mon Apr 24 15:01:56 2023, max compression
```

## Comparing `adt_cache-0.0.5.tar` & `adt_cache-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:58:44.000000 adt_cache-0.0.5/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 11:58:44.000000 adt_cache-0.0.5/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:58:44.000000 adt_cache-0.0.5/cache/
--rw-r--r--   0 nezah      (501) staff       (20)     2496 2023-04-24 11:58:43.000000 adt_cache-0.0.5/cache/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.5/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:58:44.000000 adt_cache-0.0.5/adt_cache.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 11:58:44.000000 adt_cache-0.0.5/adt_cache.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 11:58:44.000000 adt_cache-0.0.5/adt_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 11:58:44.000000 adt_cache-0.0.5/adt_cache.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 11:58:44.000000 adt_cache-0.0.5/adt_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.5/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 11:58:43.000000 adt_cache-0.0.5/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 11:58:44.000000 adt_cache-0.0.5/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:01:56.000000 adt_cache-0.0.6/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:01:56.000000 adt_cache-0.0.6/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:01:56.000000 adt_cache-0.0.6/cache/
+-rw-r--r--   0 nezah      (501) staff       (20)     2543 2023-04-24 15:01:55.000000 adt_cache-0.0.6/cache/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.6/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 15:01:56.000000 adt_cache-0.0.6/adt_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.6/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 15:01:55.000000 adt_cache-0.0.6/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 15:01:56.000000 adt_cache-0.0.6/setup.cfg
```

### Comparing `adt_cache-0.0.5/PKG-INFO` & `adt_cache-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt_cache
-Version: 0.0.5
+Version: 0.0.6
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.5/cache/__init__.py` & `adt_cache-0.0.6/cache/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from abc import abstractmethod, ABCMeta
-from typing import List
+from typing import List, Dict
 import redis
 
 logger = logging.getLogger("adt_cache")
 
 
 class AdtCache(metaclass=ABCMeta):
     def __init__(self):
@@ -23,19 +23,19 @@
         pass
 
     @abstractmethod
     def keys(self):
         pass
 
     @abstractmethod
-    def hget(self, hash_name: str, key: str):
+    def hget(self, hash_name: str) -> Dict:
         pass
 
     @abstractmethod
-    def hset(self, hash_name: str, key: str, val):
+    def hset(self, hash_name: str, dict: Dict[str, any]):
         pass
 
 
 class RedisCache(AdtCache):
     def __init__(self, host: str, port, db, expire_mins=60*24, clear_cache=False):
         logger.info(f"init redis cache with {host}:{port}:{db}")
         super().__init__()
@@ -53,20 +53,21 @@
     def push_values(self, key, vals: List):
         self.redis.expire(key, 60 * self.expire_mins)
         return self.redis.sadd(key, *set(vals))
 
     def keys(self):
         return self.redis.keys()
 
-    def hget(self, hash_name: str, key: str):
-        return self.redis.hget(hash_name, key)
+    def hget(self, hash_name: str) -> Dict:
+        return self.redis.hgetall(hash_name)
 
-    def hset(self, hash_name: str, key: str, val):
-        self.redis.expire(key, 60 * self.expire_mins)
-        return self.redis.hset(hash_name, key, val)
+    def hset(self, hash_name: str, dict: Dict[str, any]):
+        for items in dict.items():
+            self.redis.hset(hash_name, items[0], items[1])
+        self.redis.expire(hash_name, 60 * self.expire_mins)
 
 
 class MemoryCache(AdtCache):
     def __init__(self):
         super().__init__()
         self.cache = {}
 
@@ -82,12 +83,12 @@
             self.cache[key] = set(vals)
         else:
             c.update(vals)
 
     def keys(self):
         return self.cache.keys()
 
-    def hget(self, hash_name: str, key: str):
-        return self.cache.get(f"{hash_name}_{key}")
+    def hget(self, hash_name: str) -> Dict :
+        return self.cache.get(hash_name)
 
-    def hset(self, hash_name: str, key: str, val):
-        self.cache[f"{hash_name}_{key}"] = val
+    def hset(self, hash_name: str, dict: Dict[str, any]):
+        self.cache[hash_name] = dict
```

### Comparing `adt_cache-0.0.5/LICENSE` & `adt_cache-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.5/adt_cache.egg-info/PKG-INFO` & `adt_cache-0.0.6/adt_cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-cache
-Version: 0.0.5
+Version: 0.0.6
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.5/setup.py` & `adt_cache-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="adt_cache",
-    version="0.0.5",
+    version="0.0.6",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="abstract cache with in memory cache or redis (sentinel)",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/pypi_adt_cache",
     packages=setuptools.find_packages(),
```

