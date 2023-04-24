# Comparing `tmp/NeuralBasics-1.0.6.tar.gz` & `tmp/NeuralBasics-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralBasics-1.0.6.tar", last modified: Mon Apr 24 18:58:07 2023, max compression
+gzip compressed data, was "NeuralBasics-1.0.7.tar", last modified: Mon Apr 24 19:04:58 2023, max compression
```

## Comparing `NeuralBasics-1.0.6.tar` & `NeuralBasics-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 18:58:07.006539 NeuralBasics-1.0.6/
--rw-r--r--   0 henry     (1000) henry     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.6/MANIFEST.in
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 18:58:07.006539 NeuralBasics-1.0.6/NeuralBasics.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 18:58:07.000000 NeuralBasics-1.0.6/NeuralBasics.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      224 2023-04-24 18:58:07.000000 NeuralBasics-1.0.6/NeuralBasics.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 18:58:07.000000 NeuralBasics-1.0.6/NeuralBasics.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       49 2023-04-24 18:58:07.000000 NeuralBasics-1.0.6/NeuralBasics.egg-info/requires.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 18:58:07.000000 NeuralBasics-1.0.6/NeuralBasics.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 18:58:07.006539 NeuralBasics-1.0.6/PKG-INFO
--rw-r--r--   0 henry     (1000) henry     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.6/README.md
--rw-r--r--   0 henry     (1000) henry     (1000)      620 2023-04-24 18:57:57.000000 NeuralBasics-1.0.6/pyproject.toml
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-04-24 18:58:07.006539 NeuralBasics-1.0.6/setup.cfg
--rw-r--r--   0 henry     (1000) henry     (1000)      408 2023-04-24 18:58:01.000000 NeuralBasics-1.0.6/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 19:04:58.481070 NeuralBasics-1.0.7/
+-rw-r--r--   0 henry     (1000) henry     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.7/MANIFEST.in
+-rw-rw-r--   0 henry     (1000) henry     (1000)      524 2023-04-24 19:04:58.481070 NeuralBasics-1.0.7/PKG-INFO
+-rw-r--r--   0 henry     (1000) henry     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.7/README.md
+-rw-r--r--   0 henry     (1000) henry     (1000)      620 2023-04-24 19:04:32.000000 NeuralBasics-1.0.7/pyproject.toml
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-04-24 19:04:58.481070 NeuralBasics-1.0.7/setup.cfg
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 19:04:58.481070 NeuralBasics-1.0.7/src/
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 19:04:58.481070 NeuralBasics-1.0.7/src/NeuralBasics/
+-rw-r--r--   0 henry     (1000) henry     (1000)      159 2023-04-24 18:57:31.000000 NeuralBasics-1.0.7/src/NeuralBasics/__init__.py
+-rw-r--r--   0 henry     (1000) henry     (1000)    15103 2023-04-24 07:36:54.000000 NeuralBasics-1.0.7/src/NeuralBasics/network.py
+-rw-r--r--   0 henry     (1000) henry     (1000)      336 2023-04-24 07:48:41.000000 NeuralBasics-1.0.7/src/NeuralBasics/test.py
+-rw-r--r--   0 henry     (1000) henry     (1000)     2173 2023-04-24 07:36:54.000000 NeuralBasics-1.0.7/src/NeuralBasics/utils.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 19:04:58.481070 NeuralBasics-1.0.7/src/NeuralBasics.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      524 2023-04-24 19:04:58.000000 NeuralBasics-1.0.7/src/NeuralBasics.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)      304 2023-04-24 19:04:58.000000 NeuralBasics-1.0.7/src/NeuralBasics.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 19:04:58.000000 NeuralBasics-1.0.7/src/NeuralBasics.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       13 2023-04-24 19:04:58.000000 NeuralBasics-1.0.7/src/NeuralBasics.egg-info/top_level.txt
```

### Comparing `NeuralBasics-1.0.6/NeuralBasics.egg-info/PKG-INFO` & `NeuralBasics-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.6
+Version: 1.0.7
 Summary: Neural network basics module. Number detection on images.
-Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `NeuralBasics-1.0.6/PKG-INFO` & `NeuralBasics-1.0.7/src/NeuralBasics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.6
+Version: 1.0.7
 Summary: Neural network basics module. Number detection on images.
-Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `NeuralBasics-1.0.6/pyproject.toml` & `NeuralBasics-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuralBasics"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Henry Cook", email="henryscookolaizola@gmail.com" },
 ]
 description = "Neural network basics module. Number detection on images."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

