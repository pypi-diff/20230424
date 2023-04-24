# Comparing `tmp/NeuralBasics-1.0.8.tar.gz` & `tmp/NeuralBasics-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralBasics-1.0.8.tar", last modified: Mon Apr 24 19:35:49 2023, max compression
+gzip compressed data, was "NeuralBasics-1.0.9.tar", last modified: Mon Apr 24 20:06:17 2023, max compression
```

## Comparing `NeuralBasics-1.0.8.tar` & `NeuralBasics-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 19:35:49.229481 NeuralBasics-1.0.8/
--rw-r--r--   0 henry     (1000) henry     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.8/MANIFEST.in
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 19:35:49.229481 NeuralBasics-1.0.8/NeuralBasics.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 19:35:49.000000 NeuralBasics-1.0.8/NeuralBasics.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      224 2023-04-24 19:35:49.000000 NeuralBasics-1.0.8/NeuralBasics.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 19:35:49.000000 NeuralBasics-1.0.8/NeuralBasics.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       49 2023-04-24 19:35:49.000000 NeuralBasics-1.0.8/NeuralBasics.egg-info/requires.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 19:35:49.000000 NeuralBasics-1.0.8/NeuralBasics.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 19:35:49.229481 NeuralBasics-1.0.8/PKG-INFO
--rw-r--r--   0 henry     (1000) henry     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.8/README.md
--rw-r--r--   0 henry     (1000) henry     (1000)      620 2023-04-24 19:34:33.000000 NeuralBasics-1.0.8/pyproject.toml
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-04-24 19:35:49.229481 NeuralBasics-1.0.8/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)      382 2023-04-24 19:35:33.000000 NeuralBasics-1.0.8/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 20:06:17.892486 NeuralBasics-1.0.9/
+-rw-r--r--   0 henry     (1000) henry     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.9/MANIFEST.in
+-rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 20:06:17.892486 NeuralBasics-1.0.9/PKG-INFO
+-rw-r--r--   0 henry     (1000) henry     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.9/README.md
+-rw-r--r--   0 henry     (1000) henry     (1000)      620 2023-04-24 20:05:36.000000 NeuralBasics-1.0.9/pyproject.toml
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-04-24 20:06:17.892486 NeuralBasics-1.0.9/setup.cfg
+-rw-rw-r--   0 henry     (1000) henry     (1000)      424 2023-04-24 20:05:29.000000 NeuralBasics-1.0.9/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 20:06:17.892486 NeuralBasics-1.0.9/src/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 20:06:17.892486 NeuralBasics-1.0.9/src/NeuralBasics/
+-rw-r--r--   0 henry     (1000) henry     (1000)      159 2023-04-24 18:57:31.000000 NeuralBasics-1.0.9/src/NeuralBasics/__init__.py
+-rw-r--r--   0 henry     (1000) henry     (1000)    15103 2023-04-24 07:36:54.000000 NeuralBasics-1.0.9/src/NeuralBasics/network.py
+-rw-r--r--   0 henry     (1000) henry     (1000)      408 2023-04-24 18:58:01.000000 NeuralBasics-1.0.9/src/NeuralBasics/setup.py
+-rw-r--r--   0 henry     (1000) henry     (1000)      336 2023-04-24 07:48:41.000000 NeuralBasics-1.0.9/src/NeuralBasics/test.py
+-rw-r--r--   0 henry     (1000) henry     (1000)     2173 2023-04-24 07:36:54.000000 NeuralBasics-1.0.9/src/NeuralBasics/utils.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 20:06:17.892486 NeuralBasics-1.0.9/src/NeuralBasics.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 20:06:17.000000 NeuralBasics-1.0.9/src/NeuralBasics.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)      378 2023-04-24 20:06:17.000000 NeuralBasics-1.0.9/src/NeuralBasics.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 20:06:17.000000 NeuralBasics-1.0.9/src/NeuralBasics.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       49 2023-04-24 20:06:17.000000 NeuralBasics-1.0.9/src/NeuralBasics.egg-info/requires.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       13 2023-04-24 20:06:17.000000 NeuralBasics-1.0.9/src/NeuralBasics.egg-info/top_level.txt
```

### Comparing `NeuralBasics-1.0.8/NeuralBasics.egg-info/PKG-INFO` & `NeuralBasics-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.8
+Version: 1.0.9
 Summary: Neural network basics module. Number detection on images.
 Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuralBasics-1.0.8/PKG-INFO` & `NeuralBasics-1.0.9/src/NeuralBasics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.8
+Version: 1.0.9
 Summary: Neural network basics module. Number detection on images.
 Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuralBasics-1.0.8/pyproject.toml` & `NeuralBasics-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuralBasics"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Henry Cook", email="henryscookolaizola@gmail.com" },
 ]
 description = "Neural network basics module. Number detection on images."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

