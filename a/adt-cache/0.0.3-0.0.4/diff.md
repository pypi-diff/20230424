# Comparing `tmp/adt_cache-0.0.3.tar.gz` & `tmp/adt_cache-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adt_cache-0.0.3.tar", last modified: Mon Apr 24 11:07:44 2023, max compression
+gzip compressed data, was "dist/adt_cache-0.0.4.tar", last modified: Mon Apr 24 11:51:56 2023, max compression
```

## Comparing `adt_cache-0.0.3.tar` & `adt_cache-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:07:44.000000 adt_cache-0.0.3/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 11:07:44.000000 adt_cache-0.0.3/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:07:44.000000 adt_cache-0.0.3/cache/
--rw-r--r--   0 nezah      (501) staff       (20)     2250 2023-04-24 11:07:42.000000 adt_cache-0.0.3/cache/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.3/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:07:44.000000 adt_cache-0.0.3/adt_cache.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 11:07:44.000000 adt_cache-0.0.3/adt_cache.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 11:07:44.000000 adt_cache-0.0.3/adt_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 11:07:44.000000 adt_cache-0.0.3/adt_cache.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 11:07:44.000000 adt_cache-0.0.3/adt_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.3/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 11:07:42.000000 adt_cache-0.0.3/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 11:07:44.000000 adt_cache-0.0.3/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:51:56.000000 adt_cache-0.0.4/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 11:51:56.000000 adt_cache-0.0.4/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:51:56.000000 adt_cache-0.0.4/cache/
+-rw-r--r--   0 nezah      (501) staff       (20)     2340 2023-04-24 11:51:55.000000 adt_cache-0.0.4/cache/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.4/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-24 11:51:56.000000 adt_cache-0.0.4/adt_cache.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-24 11:51:55.000000 adt_cache-0.0.4/adt_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-24 11:51:55.000000 adt_cache-0.0.4/adt_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-24 11:51:55.000000 adt_cache-0.0.4/adt_cache.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-24 11:51:55.000000 adt_cache-0.0.4/adt_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.4/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-24 11:51:55.000000 adt_cache-0.0.4/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-24 11:51:56.000000 adt_cache-0.0.4/setup.cfg
```

### Comparing `adt_cache-0.0.3/PKG-INFO` & `adt_cache-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt_cache
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.3/cache/__init__.py` & `adt_cache-0.0.4/cache/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,19 @@
     def push_values(self, key: str, vals: List):
         pass
 
     @abstractmethod
     def keys(self):
         pass
 
+    @abstractmethod
     def get(self, key: str):
         pass
 
+    @abstractmethod
     def push(self, key: str, val):
         pass
 
 
 class RedisCache(AdtCache):
     def __init__(self, host: str, port, db, expire_mins=60*24, clear_cache=False):
         logger.info(f"init redis cache with {host}:{port}:{db}")
@@ -54,15 +56,16 @@
     def keys(self):
         return self.redis.keys()
 
     def get(self, key: str):
         return self.redis.get(key)
 
     def push(self, key: str, val):
-        return self.redis.sadd(str, *set(val))
+        self.redis.expire(key, 60 * self.expire_mins)
+        return self.redis.append(str, val)
 
 class MemoryCache(AdtCache):
     def __init__(self):
         super().__init__()
         self.cache = {}
 
     def intersect(self, key, vals: List):
```

### Comparing `adt_cache-0.0.3/LICENSE` & `adt_cache-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.3/adt_cache.egg-info/PKG-INFO` & `adt_cache-0.0.4/adt_cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-cache
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.3/setup.py` & `adt_cache-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="adt_cache",
-    version="0.0.3",
+    version="0.0.4",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="abstract cache with in memory cache or redis (sentinel)",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/pypi_adt_cache",
     packages=setuptools.find_packages(),
```

