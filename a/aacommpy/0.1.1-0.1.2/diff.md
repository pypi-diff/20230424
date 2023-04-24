# Comparing `tmp/aacommpy-0.1.1.tar.gz` & `tmp/aacommpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommpy-0.1.1.tar", last modified: Mon Apr 24 12:31:06 2023, max compression
+gzip compressed data, was "aacommpy-0.1.2.tar", last modified: Mon Apr 24 12:43:58 2023, max compression
```

## Comparing `aacommpy-0.1.1.tar` & `aacommpy-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:31:06.893365 aacommpy-0.1.1/
--rw-rw-rw-   0        0        0      479 2023-04-24 12:31:06.892366 aacommpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 11:43:52.000000 aacommpy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 12:31:06.881324 aacommpy-0.1.1/aacommpy/
--rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.1/aacommpy/__init__.py
--rw-rw-rw-   0        0        0      263 2023-04-24 12:31:04.000000 aacommpy-0.1.1/aacommpy/__version__.py
--rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.1/aacommpy/curves.py
--rw-rw-rw-   0        0        0     1012 2023-04-24 12:02:21.000000 aacommpy-0.1.1/aacommpy/entry_points.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:31:06.892366 aacommpy-0.1.1/aacommpy.egg-info/
--rw-rw-rw-   0        0        0      479 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.1/aacommpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 12:31:06.000000 aacommpy-0.1.1/aacommpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 12:31:06.893365 aacommpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-24 12:27:46.000000 aacommpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:43:58.888834 aacommpy-0.1.2/
+-rw-rw-rw-   0        0        0      479 2023-04-24 12:43:58.888834 aacommpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 11:43:52.000000 aacommpy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 12:43:58.869638 aacommpy-0.1.2/aacommpy/
+-rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.2/aacommpy/__init__.py
+-rw-rw-rw-   0        0        0      263 2023-04-24 12:43:34.000000 aacommpy-0.1.2/aacommpy/__version__.py
+-rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.2/aacommpy/curves.py
+-rw-rw-rw-   0        0        0     1157 2023-04-24 12:43:28.000000 aacommpy-0.1.2/aacommpy/entry_points.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:43:58.886838 aacommpy-0.1.2/aacommpy.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-04-24 12:43:58.000000 aacommpy-0.1.2/aacommpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-24 12:43:58.000000 aacommpy-0.1.2/aacommpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:43:58.000000 aacommpy-0.1.2/aacommpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 12:43:58.000000 aacommpy-0.1.2/aacommpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.2/aacommpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-04-24 12:43:58.000000 aacommpy-0.1.2/aacommpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 12:43:58.000000 aacommpy-0.1.2/aacommpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:43:58.888834 aacommpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-04-24 12:43:45.000000 aacommpy-0.1.2/setup.py
```

### Comparing `aacommpy-0.1.1/aacommpy/curves.py` & `aacommpy-0.1.2/aacommpy/curves.py`

 * *Files identical despite different names*

### Comparing `aacommpy-0.1.1/setup.py` & `aacommpy-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 about = {
     'name': 'aacommpy',
     'description': 'A Python package for wrapping aacomm nuget package',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'author': 'HIEU',
     'author_email': 'trunghieupcs@gmail.com',
     'url': 'https://github.com/hieu/aacommpy',
     'license': 'MIT',
 }
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'aacommpy', '__version__.py')) as f:
```

