# Comparing `tmp/onsale-0.0.3.tar.gz` & `tmp/onsale-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onsale-0.0.3.tar", last modified: Sun Apr 23 21:33:37 2023, max compression
+gzip compressed data, was "onsale-0.0.4.tar", last modified: Sun Apr 23 21:58:11 2023, max compression
```

## Comparing `onsale-0.0.3.tar` & `onsale-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:33:37.910120 onsale-0.0.3/
--rw-r--r--   0 apple      (501) staff       (20)     1056 2023-04-22 10:29:15.000000 onsale-0.0.3/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:33:37.909875 onsale-0.0.3/PKG-INFO
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:33:37.908177 onsale-0.0.3/onsale/
--rw-r--r--   0 apple      (501) staff       (20)        0 2023-04-23 21:33:13.000000 onsale-0.0.3/onsale/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      216 2023-04-23 21:00:22.000000 onsale-0.0.3/onsale/sale.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:33:37.909510 onsale-0.0.3/onsale.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:33:37.000000 onsale-0.0.3/onsale.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      170 2023-04-23 21:33:37.000000 onsale-0.0.3/onsale.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-04-23 21:33:37.000000 onsale-0.0.3/onsale.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2023-04-23 21:33:37.000000 onsale-0.0.3/onsale.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2023-04-23 21:33:37.910208 onsale-0.0.3/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      673 2023-04-23 21:33:26.000000 onsale-0.0.3/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:58:11.463217 onsale-0.0.4/
+-rw-r--r--   0 apple      (501) staff       (20)     1056 2023-04-22 10:29:15.000000 onsale-0.0.4/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:58:11.462956 onsale-0.0.4/PKG-INFO
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:58:11.460940 onsale-0.0.4/onsale/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2023-04-23 21:39:17.000000 onsale-0.0.4/onsale/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      223 2023-04-23 21:58:02.000000 onsale-0.0.4/onsale/sale.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-04-23 21:58:11.462563 onsale-0.0.4/onsale.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)      525 2023-04-23 21:58:11.000000 onsale-0.0.4/onsale.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      170 2023-04-23 21:58:11.000000 onsale-0.0.4/onsale.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-04-23 21:58:11.000000 onsale-0.0.4/onsale.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        7 2023-04-23 21:58:11.000000 onsale-0.0.4/onsale.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2023-04-23 21:58:11.463310 onsale-0.0.4/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      673 2023-04-23 21:58:07.000000 onsale-0.0.4/setup.py
```

### Comparing `onsale-0.0.3/LICENSE` & `onsale-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onsale-0.0.3/PKG-INFO` & `onsale-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onsale
-Version: 0.0.3
+Version: 0.0.4
 Summary: Put your shop on sale
 Home-page: UNKNOWN
 Author: Sandesh
 Author-email: <mail@sandesh.com>
 License: UNKNOWN
 Keywords: python,sale,discount
 Platform: UNKNOWN
```

### Comparing `onsale-0.0.3/onsale.egg-info/PKG-INFO` & `onsale-0.0.4/onsale.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onsale
-Version: 0.0.3
+Version: 0.0.4
 Summary: Put your shop on sale
 Home-page: UNKNOWN
 Author: Sandesh
 Author-email: <mail@sandesh.com>
 License: UNKNOWN
 Keywords: python,sale,discount
 Platform: UNKNOWN
```

### Comparing `onsale-0.0.3/setup.py` & `onsale-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Put your shop on sale'
 
 # Setting up
 setup(
     name="onsale",
     version=VERSION,
     author="Sandesh",
```

