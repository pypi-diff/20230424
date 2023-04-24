# Comparing `tmp/tap-deputy-1.1.0.tar.gz` & `tmp/tap-deputy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-deputy-1.1.0.tar", last modified: Mon Nov  7 14:32:10 2022, max compression
+gzip compressed data, was "tap-deputy-1.1.1.tar", last modified: Mon Apr 24 08:45:37 2023, max compression
```

## Comparing `tap-deputy-1.1.0.tar` & `tap-deputy-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-07 14:32:10.455867 tap-deputy-1.1.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-09-16 10:26:28.000000 tap-deputy-1.1.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2022-11-07 14:32:10.455867 tap-deputy-1.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1859 2022-09-16 10:26:28.000000 tap-deputy-1.1.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-11-07 14:32:10.455867 tap-deputy-1.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2022-11-07 14:29:31.000000 tap-deputy-1.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-07 14:32:10.455867 tap-deputy-1.1.0/tap_deputy/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1416 2022-11-07 12:44:55.000000 tap-deputy-1.1.0/tap_deputy/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4389 2022-11-07 12:44:55.000000 tap-deputy-1.1.0/tap_deputy/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3974 2022-09-16 10:26:28.000000 tap-deputy-1.1.0/tap_deputy/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3101 2022-09-16 10:26:28.000000 tap-deputy-1.1.0/tap_deputy/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-11-07 12:44:55.000000 tap-deputy-1.1.0/tap_deputy/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-07 14:32:10.455867 tap-deputy-1.1.0/tap_deputy.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2022-11-07 14:32:10.000000 tap-deputy-1.1.0/tap_deputy.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-11-07 14:32:10.000000 tap-deputy-1.1.0/tap_deputy.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-07 14:32:10.000000 tap-deputy-1.1.0/tap_deputy.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2022-11-07 14:32:10.000000 tap-deputy-1.1.0/tap_deputy.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2022-11-07 14:32:10.000000 tap-deputy-1.1.0/tap_deputy.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-07 14:32:10.000000 tap-deputy-1.1.0/tap_deputy.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 08:45:37.949144 tap-deputy-1.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-11-11 04:31:39.000000 tap-deputy-1.1.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      289 2023-04-24 08:45:37.949144 tap-deputy-1.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1859 2022-11-11 04:31:39.000000 tap-deputy-1.1.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-24 08:45:37.949144 tap-deputy-1.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-24 08:42:59.000000 tap-deputy-1.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 08:45:37.949144 tap-deputy-1.1.1/tap_deputy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1416 2023-04-24 08:21:57.000000 tap-deputy-1.1.1/tap_deputy/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4389 2023-04-24 08:21:57.000000 tap-deputy-1.1.1/tap_deputy/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4153 2023-04-24 08:42:59.000000 tap-deputy-1.1.1/tap_deputy/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3101 2022-11-11 04:31:39.000000 tap-deputy-1.1.1/tap_deputy/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      662 2023-04-24 08:21:57.000000 tap-deputy-1.1.1/tap_deputy/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 08:45:37.949144 tap-deputy-1.1.1/tap_deputy.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      289 2023-04-24 08:45:37.000000 tap-deputy-1.1.1/tap_deputy.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2023-04-24 08:45:37.000000 tap-deputy-1.1.1/tap_deputy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-24 08:45:37.000000 tap-deputy-1.1.1/tap_deputy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-04-24 08:45:37.000000 tap-deputy-1.1.1/tap_deputy.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-04-24 08:45:37.000000 tap-deputy-1.1.1/tap_deputy.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-04-24 08:45:37.000000 tap-deputy-1.1.1/tap_deputy.egg-info/top_level.txt
```

### Comparing `tap-deputy-1.1.0/LICENSE` & `tap-deputy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-deputy-1.1.0/README.md` & `tap-deputy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-deputy-1.1.0/setup.py` & `tap-deputy-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-deputy',
-      version='1.1.0',
+      version='1.1.1',
       description='Singer.io tap for extracting data from the Deputy API',
       author='Deputy',
       url='https://www.deputy.com',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       python_requires='>=3.5.3',
       py_modules=['tap_deputy'],
       install_requires=[
```

### Comparing `tap-deputy-1.1.0/tap_deputy/__init__.py` & `tap-deputy-1.1.1/tap_deputy/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-deputy-1.1.0/tap_deputy/client.py` & `tap-deputy-1.1.1/tap_deputy/client.py`

 * *Files identical despite different names*

### Comparing `tap-deputy-1.1.0/tap_deputy/discover.py` & `tap-deputy-1.1.1/tap_deputy/discover.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,18 @@
             'metadata': {
                 'tap-deputy.resource': resource_name
             }
         }
     ]
 
     for field_name, field_type in data['fields'].items():
+        # Skipping all fields of type Json until we decide on how to handle "[]" as null response
+        # Json data fields
+        if field_type == "Json":
+            continue
         if field_type in ['Date', 'DateTime']:
             json_schema = {
                 'type': ['null', 'string'],
                 'format': 'date-time'
             }
         else:
             json_schema = {
```

### Comparing `tap-deputy-1.1.0/tap_deputy/sync.py` & `tap-deputy-1.1.1/tap_deputy/sync.py`

 * *Files identical despite different names*

### Comparing `tap-deputy-1.1.0/tap_deputy/utils.py` & `tap-deputy-1.1.1/tap_deputy/utils.py`

 * *Files identical despite different names*

