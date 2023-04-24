# Comparing `tmp/aacommpy-0.1.0.tar.gz` & `tmp/aacommpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommpy-0.1.0.tar", last modified: Mon Apr 24 12:09:33 2023, max compression
+gzip compressed data, was "aacommpy-0.1.1.tar", last modified: Mon Apr 24 12:31:06 2023, max compression
```

## Comparing `aacommpy-0.1.0.tar` & `aacommpy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:09:33.090377 aacommpy-0.1.0/
--rw-rw-rw-   0        0        0      482 2023-04-24 12:09:33.088872 aacommpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 11:43:52.000000 aacommpy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 12:09:33.068841 aacommpy-0.1.0/aacommpy/
--rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.0/aacommpy/__init__.py
--rw-rw-rw-   0        0        0      379 2023-04-24 11:52:26.000000 aacommpy-0.1.0/aacommpy/__version__.py
--rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.0/aacommpy/curves.py
--rw-rw-rw-   0        0        0     1012 2023-04-24 12:02:21.000000 aacommpy-0.1.0/aacommpy/entry_points.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:09:33.088872 aacommpy-0.1.0/aacommpy.egg-info/
--rw-rw-rw-   0        0        0      482 2023-04-24 12:09:32.000000 aacommpy-0.1.0/aacommpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-24 12:09:33.000000 aacommpy-0.1.0/aacommpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:09:32.000000 aacommpy-0.1.0/aacommpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 12:09:32.000000 aacommpy-0.1.0/aacommpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.0/aacommpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-24 12:09:32.000000 aacommpy-0.1.0/aacommpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 12:09:32.000000 aacommpy-0.1.0/aacommpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 12:09:33.090377 aacommpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-24 12:09:24.000000 aacommpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:31:06.893365 aacommpy-0.1.1/
+-rw-rw-rw-   0        0        0      479 2023-04-24 12:31:06.892366 aacommpy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 11:43:52.000000 aacommpy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 12:31:06.881324 aacommpy-0.1.1/aacommpy/
+-rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.1/aacommpy/__init__.py
+-rw-rw-rw-   0        0        0      263 2023-04-24 12:31:04.000000 aacommpy-0.1.1/aacommpy/__version__.py
+-rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.1/aacommpy/curves.py
+-rw-rw-rw-   0        0        0     1012 2023-04-24 12:02:21.000000 aacommpy-0.1.1/aacommpy/entry_points.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:31:06.892366 aacommpy-0.1.1/aacommpy.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.1/aacommpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:31:06.893365 aacommpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-04-24 12:27:46.000000 aacommpy-0.1.1/setup.py
```

### Comparing `aacommpy-0.1.0/aacommpy/curves.py` & `aacommpy-0.1.1/aacommpy/curves.py`

 * *Files identical despite different names*

### Comparing `aacommpy-0.1.0/aacommpy/entry_points.py` & `aacommpy-0.1.1/aacommpy/entry_points.py`

 * *Files identical despite different names*

### Comparing `aacommpy-0.1.0/setup.py` & `aacommpy-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 about = {
     'name': 'aacommpy',
     'description': 'A Python package for wrapping aacomm nuget package',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'author': 'HIEU',
     'author_email': 'trunghieupcs@gmail.com',
     'url': 'https://github.com/hieu/aacommpy',
     'license': 'MIT',
 }
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'aacommpy', '__version__.py')) as f:
```

