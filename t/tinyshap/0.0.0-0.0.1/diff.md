# Comparing `tmp/tinyshap-0.0.0.tar.gz` & `tmp/tinyshap-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyshap-0.0.0.tar", last modified: Mon Apr 24 17:37:45 2023, max compression
+gzip compressed data, was "tinyshap-0.0.1.tar", last modified: Mon Apr 24 17:47:20 2023, max compression
```

## Comparing `tinyshap-0.0.0.tar` & `tinyshap-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:37:45.400091 tinyshap-0.0.0/
--rw-rw-rw-   0        0        0     1086 2023-04-09 14:34:23.000000 tinyshap-0.0.0/LICENCE
--rw-rw-rw-   0        0        0      835 2023-04-24 17:37:45.398092 tinyshap-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-09 14:34:58.000000 tinyshap-0.0.0/README.md
--rw-rw-rw-   0        0        0     1086 2023-04-24 17:37:04.000000 tinyshap-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 17:37:45.400091 tinyshap-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 17:37:45.394096 tinyshap-0.0.0/tinyshap.egg-info/
--rw-rw-rw-   0        0        0      835 2023-04-24 17:37:45.000000 tinyshap-0.0.0/tinyshap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-24 17:37:45.000000 tinyshap-0.0.0/tinyshap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:37:45.000000 tinyshap-0.0.0/tinyshap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-24 17:37:45.000000 tinyshap-0.0.0/tinyshap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 17:37:45.000000 tinyshap-0.0.0/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:47:20.580622 tinyshap-0.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-04-09 14:34:23.000000 tinyshap-0.0.1/LICENCE
+-rw-rw-rw-   0        0        0      835 2023-04-24 17:47:20.578626 tinyshap-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-09 14:34:58.000000 tinyshap-0.0.1/README.md
+-rw-rw-rw-   0        0        0     1076 2023-04-24 17:46:55.000000 tinyshap-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:47:20.580622 tinyshap-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 17:47:20.574627 tinyshap-0.0.1/tinyshap.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/top_level.txt
```

### Comparing `tinyshap-0.0.0/LICENCE` & `tinyshap-0.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.0/PKG-INFO` & `tinyshap-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.0
+Version: 0.0.1
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `tinyshap-0.0.0/pyproject.toml` & `tinyshap-0.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'tinyshap'
-dynamic = [
-  'version'
-]
+version = '0.0.1'
 description = 'Minimal implementation of approximate Kernel SHAP algorithm'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
```

### Comparing `tinyshap-0.0.0/tinyshap.egg-info/PKG-INFO` & `tinyshap-0.0.1/tinyshap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.0
+Version: 0.0.1
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

