# Comparing `tmp/NeuralBasics-1.0.3.tar.gz` & `tmp/NeuralBasics-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralBasics-1.0.3.tar", last modified: Mon Apr 24 15:51:25 2023, max compression
+gzip compressed data, was "NeuralBasics-1.0.5.tar", last modified: Mon Apr 24 15:58:32 2023, max compression
```

## Comparing `NeuralBasics-1.0.3.tar` & `NeuralBasics-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 15:51:25.064647 NeuralBasics-1.0.3/
--rw-r--r--   0 henry     (1000) henry     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.3/MANIFEST.in
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 15:51:25.064647 NeuralBasics-1.0.3/NeuralBasics.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 15:51:25.000000 NeuralBasics-1.0.3/NeuralBasics.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      224 2023-04-24 15:51:25.000000 NeuralBasics-1.0.3/NeuralBasics.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 15:51:25.000000 NeuralBasics-1.0.3/NeuralBasics.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       49 2023-04-24 15:51:25.000000 NeuralBasics-1.0.3/NeuralBasics.egg-info/requires.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 15:51:25.000000 NeuralBasics-1.0.3/NeuralBasics.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 15:51:25.064647 NeuralBasics-1.0.3/PKG-INFO
--rw-r--r--   0 henry     (1000) henry     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.3/README.md
--rw-r--r--   0 henry     (1000) henry     (1000)      620 2023-04-24 15:50:06.000000 NeuralBasics-1.0.3/pyproject.toml
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-04-24 15:51:25.064647 NeuralBasics-1.0.3/setup.cfg
--rw-r--r--   0 henry     (1000) henry     (1000)      382 2023-04-24 15:50:04.000000 NeuralBasics-1.0.3/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 15:58:32.955096 NeuralBasics-1.0.5/
+-rw-r--r--   0 henry     (1000) henry     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.5/MANIFEST.in
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-04-24 15:58:32.955096 NeuralBasics-1.0.5/NeuralBasics.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 15:58:32.000000 NeuralBasics-1.0.5/NeuralBasics.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)      224 2023-04-24 15:58:32.000000 NeuralBasics-1.0.5/NeuralBasics.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 15:58:32.000000 NeuralBasics-1.0.5/NeuralBasics.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       49 2023-04-24 15:58:32.000000 NeuralBasics-1.0.5/NeuralBasics.egg-info/requires.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-04-24 15:58:32.000000 NeuralBasics-1.0.5/NeuralBasics.egg-info/top_level.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)      543 2023-04-24 15:58:32.955096 NeuralBasics-1.0.5/PKG-INFO
+-rw-r--r--   0 henry     (1000) henry     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.5/README.md
+-rw-r--r--   0 henry     (1000) henry     (1000)      620 2023-04-24 15:57:12.000000 NeuralBasics-1.0.5/pyproject.toml
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-04-24 15:58:32.955096 NeuralBasics-1.0.5/setup.cfg
+-rw-r--r--   0 henry     (1000) henry     (1000)      408 2023-04-24 15:58:27.000000 NeuralBasics-1.0.5/setup.py
```

### Comparing `NeuralBasics-1.0.3/NeuralBasics.egg-info/PKG-INFO` & `NeuralBasics-1.0.5/NeuralBasics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.3
+Version: 1.0.5
 Summary: Neural network basics module. Number detection on images.
 Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuralBasics-1.0.3/PKG-INFO` & `NeuralBasics-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.3
+Version: 1.0.5
 Summary: Neural network basics module. Number detection on images.
 Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuralBasics-1.0.3/pyproject.toml` & `NeuralBasics-1.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuralBasics"
-version = "1.0.3"
+version = "1.0.5"
 authors = [
   { name="Henry Cook", email="henryscookolaizola@gmail.com" },
 ]
 description = "Neural network basics module. Number detection on images."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

