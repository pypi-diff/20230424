# Comparing `tmp/nudeny-0.0.6.tar.gz` & `tmp/nudeny-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudeny-0.0.6.tar", max compression
+gzip compressed data, was "nudeny-0.0.7.tar", max compression
```

## Comparing `nudeny-0.0.6.tar` & `nudeny-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1091 2023-03-25 16:00:24.478955 nudeny-0.0.6/LICENSE
--rw-r--r--   0        0        0      527 2023-04-21 16:36:09.058748 nudeny-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-25 16:00:24.478955 nudeny-0.0.6/src/nudeny/__init__.py
--rw-r--r--   0        0        0     5281 2023-04-21 16:35:44.022507 nudeny-0.0.6/src/nudeny/nudeny.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 nudeny-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-25 16:00:24.478955 nudeny-0.0.7/LICENSE
+-rw-r--r--   0        0        0      527 2023-04-24 14:14:26.977299 nudeny-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-03-25 16:00:24.478955 nudeny-0.0.7/src/nudeny/__init__.py
+-rw-r--r--   0        0        0     5281 2023-04-24 14:11:42.740289 nudeny-0.0.7/src/nudeny/nudeny.py
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 nudeny-0.0.7/PKG-INFO
```

### Comparing `nudeny-0.0.6/LICENSE` & `nudeny-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nudeny-0.0.6/pyproject.toml` & `nudeny-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Nudeny"
-version = "0.0.6"
+version = "0.0.7"
 description = "Image nudity classification and detection package."
 authors = ["Nudeny <thesis.nudeny69@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Nudeny/Nudeny-python-module"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `nudeny-0.0.6/src/nudeny/nudeny.py` & `nudeny-0.0.7/src/nudeny/nudeny.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import requests
 from urllib.parse import urlparse
 from PIL import Image
 
 class Classify:
     def __init__(self):
         self.LOCALHOST_URL = "http://127.0.0.1:8000/"
-        self.URL = "http://ec2-18-142-227-173.ap-southeast-1.compute.amazonaws.com/"
+        self.URL = "http://ec2-18-136-200-224.ap-southeast-1.compute.amazonaws.com/"
     
     def imageClassify(self, paths=[]):
         """
         Classify an image, from path provided, if it contains nudity, or if it is sexy or safe.
 
         Args:
             paths (list): List of Image path
```

### Comparing `nudeny-0.0.6/PKG-INFO` & `nudeny-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudeny
-Version: 0.0.6
+Version: 0.0.7
 Summary: Image nudity classification and detection package.
 Home-page: https://github.com/Nudeny/Nudeny-python-module
 License: MIT
 Author: Nudeny
 Author-email: thesis.nudeny69@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

