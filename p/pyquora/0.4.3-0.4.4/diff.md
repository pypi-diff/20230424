# Comparing `tmp/pyquora-0.4.3.tar.gz` & `tmp/pyquora-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquora-0.4.3.tar", last modified: Mon Apr 24 06:49:01 2023, max compression
+gzip compressed data, was "pyquora-0.4.4.tar", last modified: Mon Apr 24 07:17:03 2023, max compression
```

## Comparing `pyquora-0.4.3.tar` & `pyquora-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:49:01.463251 pyquora-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 06:48:44.000000 pyquora-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 06:48:44.000000 pyquora-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 06:49:01.463251 pyquora-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 06:48:44.000000 pyquora-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:49:01.459251 pyquora-0.4.3/pyquora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 06:49:01.000000 pyquora-0.4.3/pyquora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-24 06:49:01.000000 pyquora-0.4.3/pyquora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:49:01.000000 pyquora-0.4.3/pyquora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 06:49:01.000000 pyquora-0.4.3/pyquora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 06:49:01.000000 pyquora-0.4.3/pyquora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:49:01.463251 pyquora-0.4.3/quora/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/content.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/question.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-24 06:48:44.000000 pyquora-0.4.3/quora/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:49:01.463251 pyquora-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 06:48:44.000000 pyquora-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:17:03.790868 pyquora-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 07:16:47.000000 pyquora-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 07:16:47.000000 pyquora-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 07:17:03.790868 pyquora-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 07:16:47.000000 pyquora-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:17:03.786868 pyquora-0.4.4/pyquora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 07:17:03.000000 pyquora-0.4.4/pyquora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-24 07:17:03.000000 pyquora-0.4.4/pyquora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:17:03.000000 pyquora-0.4.4/pyquora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 07:17:03.000000 pyquora-0.4.4/pyquora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 07:17:03.000000 pyquora-0.4.4/pyquora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:17:03.786868 pyquora-0.4.4/quora/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/question.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-24 07:16:47.000000 pyquora-0.4.4/quora/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:17:03.790868 pyquora-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 07:16:47.000000 pyquora-0.4.4/setup.py
```

### Comparing `pyquora-0.4.3/LICENSE` & `pyquora-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/PKG-INFO` & `pyquora-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquora
-Version: 0.4.3
+Version: 0.4.4
 Summary: Fetch profiles and data from Quora.
 Home-page: https://github.com/TheShubhendra/pyquora
 Author: Shubhendra Kushwaha
 Author-email: shubhendrakushwaha94@gmail.com
 License: MIT
 Keywords: scraper,quora
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyquora-0.4.3/README.md` & `pyquora-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/pyquora.egg-info/PKG-INFO` & `pyquora-0.4.4/pyquora.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquora
-Version: 0.4.3
+Version: 0.4.4
 Summary: Fetch profiles and data from Quora.
 Home-page: https://github.com/TheShubhendra/pyquora
 Author: Shubhendra Kushwaha
 Author-email: shubhendrakushwaha94@gmail.com
 License: MIT
 Keywords: scraper,quora
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyquora-0.4.3/quora/_parsers.py` & `pyquora-0.4.4/quora/_parsers.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/answer.py` & `pyquora-0.4.4/quora/answer.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/cache.py` & `pyquora-0.4.4/quora/cache.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/content.py` & `pyquora-0.4.4/quora/content.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/profile.py` & `pyquora-0.4.4/quora/profile.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/sync.py` & `pyquora-0.4.4/quora/sync.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/topic.py` & `pyquora-0.4.4/quora/topic.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/quora/user.py` & `pyquora-0.4.4/quora/user.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.3/setup.py` & `pyquora-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         requirements = f.read()
     return requirements
 
 
 setup(
     name="pyquora",
     packages=find_packages(),
-    version="0.4.3",
+    version="0.4.4",
     license="MIT",
     description="""Fetch profiles and data from Quora.""",
     author="Shubhendra Kushwaha",
     author_email="shubhendrakushwaha94@gmail.com",
     url="https://github.com/TheShubhendra/pyquora",
     keywords=[
         "scraper",
```

