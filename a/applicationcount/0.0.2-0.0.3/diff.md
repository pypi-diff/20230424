# Comparing `tmp/applicationcount-0.0.2.tar.gz` & `tmp/applicationcount-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applicationcount-0.0.2.tar", last modified: Mon Apr 24 10:14:38 2023, max compression
+gzip compressed data, was "applicationcount-0.0.3.tar", last modified: Mon Apr 24 10:26:45 2023, max compression
```

## Comparing `applicationcount-0.0.2.tar` & `applicationcount-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-24 10:14:38.174790 applicationcount-0.0.2/
--rw-r--r--   0 apple      (501) staff       (20)     1056 2023-04-24 08:51:59.000000 applicationcount-0.0.2/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      601 2023-04-24 10:14:38.174534 applicationcount-0.0.2/PKG-INFO
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-24 10:14:38.172868 applicationcount-0.0.2/applicationcount.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)      601 2023-04-24 10:14:38.000000 applicationcount-0.0.2/applicationcount.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      209 2023-04-24 10:14:38.000000 applicationcount-0.0.2/applicationcount.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-04-24 10:14:38.000000 applicationcount-0.0.2/applicationcount.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2023-04-24 10:14:38.000000 applicationcount-0.0.2/applicationcount.egg-info/top_level.txt
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-24 10:14:38.173680 applicationcount-0.0.2/count/
--rw-r--r--   0 apple      (501) staff       (20)        0 2023-04-24 08:52:50.000000 applicationcount-0.0.2/count/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      568 2023-04-24 08:57:48.000000 applicationcount-0.0.2/count/count.py
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-04-24 10:14:38.174879 applicationcount-0.0.2/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      749 2023-04-24 10:14:32.000000 applicationcount-0.0.2/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-24 10:26:45.617450 applicationcount-0.0.3/
+-rw-r--r--   0 apple      (501) staff       (20)     1056 2023-04-24 08:51:59.000000 applicationcount-0.0.3/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)      601 2023-04-24 10:26:45.617189 applicationcount-0.0.3/PKG-INFO
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-24 10:26:45.615326 applicationcount-0.0.3/applicationcount/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2023-04-24 08:52:50.000000 applicationcount-0.0.3/applicationcount/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      457 2023-04-24 10:22:44.000000 applicationcount-0.0.3/applicationcount/generate.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-24 10:26:45.616831 applicationcount-0.0.3/applicationcount.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)      601 2023-04-24 10:26:45.000000 applicationcount-0.0.3/applicationcount.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      234 2023-04-24 10:26:45.000000 applicationcount-0.0.3/applicationcount.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-04-24 10:26:45.000000 applicationcount-0.0.3/applicationcount.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       17 2023-04-24 10:26:45.000000 applicationcount-0.0.3/applicationcount.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2023-04-24 10:26:45.617546 applicationcount-0.0.3/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      749 2023-04-24 10:25:39.000000 applicationcount-0.0.3/setup.py
```

### Comparing `applicationcount-0.0.2/LICENSE` & `applicationcount-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `applicationcount-0.0.2/PKG-INFO` & `applicationcount-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applicationcount
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get number of candidates that applied to the job. You can now generate passsword too.
 Home-page: UNKNOWN
 Author: Siddesh
 Author-email: <mail@siddesh.com>
 License: UNKNOWN
 Keywords: python,job,application
 Platform: UNKNOWN
```

### Comparing `applicationcount-0.0.2/applicationcount.egg-info/PKG-INFO` & `applicationcount-0.0.3/applicationcount.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applicationcount
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get number of candidates that applied to the job. You can now generate passsword too.
 Home-page: UNKNOWN
 Author: Siddesh
 Author-email: <mail@siddesh.com>
 License: UNKNOWN
 Keywords: python,job,application
 Platform: UNKNOWN
```

### Comparing `applicationcount-0.0.2/setup.py` & `applicationcount-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Get number of candidates that applied to the job. You can now generate passsword too.'
 
 # Setting up
 setup(
     name="applicationcount",
     version=VERSION,
     author="Siddesh",
```

