# Comparing `tmp/tinyshap-0.0.1.tar.gz` & `tmp/tinyshap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyshap-0.0.1.tar", last modified: Mon Apr 24 17:47:20 2023, max compression
+gzip compressed data, was "tinyshap-0.0.2.tar", last modified: Mon Apr 24 17:53:59 2023, max compression
```

## Comparing `tinyshap-0.0.1.tar` & `tinyshap-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:47:20.580622 tinyshap-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-04-09 14:34:23.000000 tinyshap-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      835 2023-04-24 17:47:20.578626 tinyshap-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-09 14:34:58.000000 tinyshap-0.0.1/README.md
--rw-rw-rw-   0        0        0     1076 2023-04-24 17:46:55.000000 tinyshap-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 17:47:20.580622 tinyshap-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 17:47:20.574627 tinyshap-0.0.1/tinyshap.egg-info/
--rw-rw-rw-   0        0        0      835 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 17:47:20.000000 tinyshap-0.0.1/tinyshap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:53:59.793523 tinyshap-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-04-09 14:34:23.000000 tinyshap-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      897 2023-04-24 17:53:59.779526 tinyshap-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-09 14:34:58.000000 tinyshap-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1148 2023-04-24 17:53:37.000000 tinyshap-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:53:59.793523 tinyshap-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 17:53:59.768539 tinyshap-0.0.2/tinyshap.egg-info/
+-rw-rw-rw-   0        0        0      897 2023-04-24 17:53:59.000000 tinyshap-0.0.2/tinyshap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-04-24 17:53:59.000000 tinyshap-0.0.2/tinyshap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:53:59.000000 tinyshap-0.0.2/tinyshap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-24 17:53:59.000000 tinyshap-0.0.2/tinyshap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 17:53:59.000000 tinyshap-0.0.2/tinyshap.egg-info/top_level.txt
```

### Comparing `tinyshap-0.0.1/LICENCE` & `tinyshap-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `tinyshap-0.0.1/PKG-INFO` & `tinyshap-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
+Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `tinyshap-0.0.1/pyproject.toml` & `tinyshap-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'tinyshap'
-version = '0.0.1'
+version = '0.0.2'
 description = 'Minimal implementation of approximate Kernel SHAP algorithm'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
@@ -26,13 +26,16 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
+[project.urls]
+"Homepage" = "https://github.com/tsitsimis/tinyshap"
+
 [tool.setuptools]
 py-modules = ["tinyshap"]
 
 [tool.black]
 line-length = 120
 target-version = ['py37', 'py38']
```

### Comparing `tinyshap-0.0.1/tinyshap.egg-info/PKG-INFO` & `tinyshap-0.0.2/tinyshap.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: tinyshap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal implementation of approximate Kernel SHAP algorithm
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
+Project-URL: Homepage, https://github.com/tsitsimis/tinyshap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

