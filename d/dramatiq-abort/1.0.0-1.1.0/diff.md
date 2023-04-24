# Comparing `tmp/dramatiq-abort-1.0.0.tar.gz` & `tmp/dramatiq-abort-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dramatiq-abort-1.0.0.tar", last modified: Wed Jul 20 15:06:05 2022, max compression
+gzip compressed data, was "dist/dramatiq-abort-1.1.0.tar", last modified: Mon Apr 24 12:40:54 2023, max compression
```

## Comparing `dramatiq-abort-1.0.0.tar` & `dramatiq-abort-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/CHANGELOGS.md
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5291 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/abort_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/backends/stub.py
--rw-r--r--   0 runner    (1001) docker     (121)     8420 2022-07-20 15:06:02.000000 dramatiq-abort-1.0.0/src/dramatiq_abort/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-20 15:06:05.000000 dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/abort_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/backends/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/src/dramatiq_abort/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:40:54.000000 dramatiq-abort-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-24 12:40:48.000000 dramatiq-abort-1.1.0/tests/test_abortable.py
```

### Comparing `dramatiq-abort-1.0.0/CONTRIBUTING.md` & `dramatiq-abort-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/LICENSE` & `dramatiq-abort-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/PKG-INFO` & `dramatiq-abort-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq-abort
-Version: 1.0.0
+Version: 1.1.0
 Summary: Dramatiq middleware to abort tasks.
 Home-page: https://github.com/flared/dramatiq-abort
 Author: Flare Systems Inc.
 Author-email: oss@flare.systems
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dramatiq-abort-1.0.0/README.md` & `dramatiq-abort-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/setup.cfg` & `dramatiq-abort-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/setup.py` & `dramatiq-abort-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 dependencies = [
     "dramatiq",
 ]
 
 extra_dependencies = {
     "gevent": ["gevent>=1.1"],
-    "redis": ["redis>=2.0,<4.0"],
+    "redis": ["redis>=2.0,<5.0"],
 }
 
 extra_dependencies["all"] = list(set(sum(extra_dependencies.values(), [])))
 extra_dependencies["dev"] = extra_dependencies["all"] + [
     # Linting
     "flake8",
     "flake8-bugbear",
```

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort/abort_manager.py` & `dramatiq-abort-1.1.0/src/dramatiq_abort/abort_manager.py`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort/backend.py` & `dramatiq-abort-1.1.0/src/dramatiq_abort/backend.py`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort/backends/redis.py` & `dramatiq-abort-1.1.0/src/dramatiq_abort/backends/redis.py`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort/backends/stub.py` & `dramatiq-abort-1.1.0/src/dramatiq_abort/backends/stub.py`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort/middleware.py` & `dramatiq-abort-1.1.0/src/dramatiq_abort/middleware.py`

 * *Files identical despite different names*

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/PKG-INFO` & `dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq-abort
-Version: 1.0.0
+Version: 1.1.0
 Summary: Dramatiq middleware to abort tasks.
 Home-page: https://github.com/flared/dramatiq-abort
 Author: Flare Systems Inc.
 Author-email: oss@flare.systems
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dramatiq-abort-1.0.0/src/dramatiq_abort.egg-info/SOURCES.txt` & `dramatiq-abort-1.1.0/src/dramatiq_abort.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 src/dramatiq_abort.egg-info/SOURCES.txt
 src/dramatiq_abort.egg-info/dependency_links.txt
 src/dramatiq_abort.egg-info/not-zip-safe
 src/dramatiq_abort.egg-info/requires.txt
 src/dramatiq_abort.egg-info/top_level.txt
 src/dramatiq_abort/backends/__init__.py
 src/dramatiq_abort/backends/redis.py
-src/dramatiq_abort/backends/stub.py
+src/dramatiq_abort/backends/stub.py
+tests/test_abortable.py
```

