# Comparing `tmp/NeuralBasics-1.0.1.tar.gz` & `tmp/NeuralBasics-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralBasics-1.0.1.tar", last modified: Mon Apr 24 12:29:36 2023, max compression
+gzip compressed data, was "NeuralBasics-1.0.2.tar", last modified: Mon Apr 24 12:37:51 2023, max compression
```

## Comparing `NeuralBasics-1.0.1.tar` & `NeuralBasics-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hcook     (1000) hcook     (1000)        0 2023-04-24 12:29:36.304030 NeuralBasics-1.0.1/
--rw-r--r--   0 hcook     (1000) hcook     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.1/MANIFEST.in
-drwxr-xr-x   0 hcook     (1000) hcook     (1000)        0 2023-04-24 12:29:36.301031 NeuralBasics-1.0.1/NeuralBasics.egg-info/
--rw-r--r--   0 hcook     (1000) hcook     (1000)      543 2023-04-24 12:29:36.000000 NeuralBasics-1.0.1/NeuralBasics.egg-info/PKG-INFO
--rw-r--r--   0 hcook     (1000) hcook     (1000)      224 2023-04-24 12:29:36.000000 NeuralBasics-1.0.1/NeuralBasics.egg-info/SOURCES.txt
--rw-r--r--   0 hcook     (1000) hcook     (1000)        1 2023-04-24 12:29:36.000000 NeuralBasics-1.0.1/NeuralBasics.egg-info/dependency_links.txt
--rw-r--r--   0 hcook     (1000) hcook     (1000)       49 2023-04-24 12:29:36.000000 NeuralBasics-1.0.1/NeuralBasics.egg-info/requires.txt
--rw-r--r--   0 hcook     (1000) hcook     (1000)        1 2023-04-24 12:29:36.000000 NeuralBasics-1.0.1/NeuralBasics.egg-info/top_level.txt
--rw-r--r--   0 hcook     (1000) hcook     (1000)      543 2023-04-24 12:29:36.302031 NeuralBasics-1.0.1/PKG-INFO
--rw-r--r--   0 hcook     (1000) hcook     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.1/README.md
--rw-r--r--   0 hcook     (1000) hcook     (1000)      620 2023-04-24 12:28:58.000000 NeuralBasics-1.0.1/pyproject.toml
--rw-r--r--   0 hcook     (1000) hcook     (1000)       38 2023-04-24 12:29:36.304030 NeuralBasics-1.0.1/setup.cfg
--rw-r--r--   0 hcook     (1000) hcook     (1000)      382 2023-04-24 12:28:53.000000 NeuralBasics-1.0.1/setup.py
+drwxr-xr-x   0 hcook     (1000) hcook     (1000)        0 2023-04-24 12:37:51.807139 NeuralBasics-1.0.2/
+-rw-r--r--   0 hcook     (1000) hcook     (1000)      256 2023-04-24 11:59:34.000000 NeuralBasics-1.0.2/MANIFEST.in
+drwxr-xr-x   0 hcook     (1000) hcook     (1000)        0 2023-04-24 12:37:51.804140 NeuralBasics-1.0.2/NeuralBasics.egg-info/
+-rw-r--r--   0 hcook     (1000) hcook     (1000)      543 2023-04-24 12:37:51.000000 NeuralBasics-1.0.2/NeuralBasics.egg-info/PKG-INFO
+-rw-r--r--   0 hcook     (1000) hcook     (1000)      224 2023-04-24 12:37:51.000000 NeuralBasics-1.0.2/NeuralBasics.egg-info/SOURCES.txt
+-rw-r--r--   0 hcook     (1000) hcook     (1000)        1 2023-04-24 12:37:51.000000 NeuralBasics-1.0.2/NeuralBasics.egg-info/dependency_links.txt
+-rw-r--r--   0 hcook     (1000) hcook     (1000)       49 2023-04-24 12:37:51.000000 NeuralBasics-1.0.2/NeuralBasics.egg-info/requires.txt
+-rw-r--r--   0 hcook     (1000) hcook     (1000)        1 2023-04-24 12:37:51.000000 NeuralBasics-1.0.2/NeuralBasics.egg-info/top_level.txt
+-rw-r--r--   0 hcook     (1000) hcook     (1000)      543 2023-04-24 12:37:51.805139 NeuralBasics-1.0.2/PKG-INFO
+-rw-r--r--   0 hcook     (1000) hcook     (1000)        0 2023-04-24 12:20:17.000000 NeuralBasics-1.0.2/README.md
+-rw-r--r--   0 hcook     (1000) hcook     (1000)      620 2023-04-24 12:37:25.000000 NeuralBasics-1.0.2/pyproject.toml
+-rw-r--r--   0 hcook     (1000) hcook     (1000)       38 2023-04-24 12:37:51.807139 NeuralBasics-1.0.2/setup.cfg
+-rw-r--r--   0 hcook     (1000) hcook     (1000)      382 2023-04-24 12:37:23.000000 NeuralBasics-1.0.2/setup.py
```

### Comparing `NeuralBasics-1.0.1/NeuralBasics.egg-info/PKG-INFO` & `NeuralBasics-1.0.2/NeuralBasics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.1
+Version: 1.0.2
 Summary: Neural network basics module. Number detection on images.
 Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuralBasics-1.0.1/PKG-INFO` & `NeuralBasics-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralBasics
-Version: 1.0.1
+Version: 1.0.2
 Summary: Neural network basics module. Number detection on images.
 Author: Henry Cook
 Author-email: Henry Cook <henryscookolaizola@gmail.com>
 Project-URL: Homepage, https://github.com/HCook86/NeuralBasics
 Project-URL: Bug Tracker, https://github.com/HCook86/NeuralBasics/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuralBasics-1.0.1/pyproject.toml` & `NeuralBasics-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeuralBasics"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Henry Cook", email="henryscookolaizola@gmail.com" },
 ]
 description = "Neural network basics module. Number detection on images."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

