# Comparing `tmp/python_bebop-1.0.1.tar.gz` & `tmp/python_bebop-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bebop-1.0.1.tar", last modified: Mon Apr 24 11:42:51 2023, max compression
+gzip compressed data, was "python_bebop-1.0.2.tar", last modified: Mon Apr 24 18:40:38 2023, max compression
```

## Comparing `python_bebop-1.0.1.tar` & `python_bebop-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 11:42:51.798157 python_bebop-1.0.1/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)     1075 2023-04-24 10:30:47.000000 python_bebop-1.0.1/LICENSE
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 11:42:51.798157 python_bebop-1.0.1/PKG-INFO
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      381 2023-04-23 18:52:15.000000 python_bebop-1.0.1/README.md
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       86 2023-04-23 18:52:15.000000 python_bebop-1.0.1/pyproject.toml
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      648 2023-04-24 11:42:51.798157 python_bebop-1.0.1/setup.cfg
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 11:42:51.790158 python_bebop-1.0.1/src/
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 11:42:51.794158 python_bebop-1.0.1/src/python_bebop/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       19 2023-04-24 11:42:34.000000 python_bebop-1.0.1/src/python_bebop/__init__.py
--rw-rw-r--   0 secretone  (1000) secretone  (1000)     4586 2023-04-24 10:26:05.000000 python_bebop-1.0.1/src/python_bebop/bebop.py
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 11:42:51.798157 python_bebop-1.0.1/src/python_bebop.egg-info/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 11:42:51.000000 python_bebop-1.0.1/src/python_bebop.egg-info/PKG-INFO
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      257 2023-04-24 11:42:51.000000 python_bebop-1.0.1/src/python_bebop.egg-info/SOURCES.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)        1 2023-04-24 11:42:51.000000 python_bebop-1.0.1/src/python_bebop.egg-info/dependency_links.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       13 2023-04-24 11:42:51.000000 python_bebop-1.0.1/src/python_bebop.egg-info/top_level.txt
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.024514 python_bebop-1.0.2/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)     1075 2023-04-24 10:30:47.000000 python_bebop-1.0.2/LICENSE
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:40:38.024514 python_bebop-1.0.2/PKG-INFO
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      381 2023-04-23 18:52:15.000000 python_bebop-1.0.2/README.md
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       86 2023-04-23 18:52:15.000000 python_bebop-1.0.2/pyproject.toml
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      648 2023-04-24 18:40:38.024514 python_bebop-1.0.2/setup.cfg
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.020514 python_bebop-1.0.2/src/
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.020514 python_bebop-1.0.2/src/python_bebop/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       42 2023-04-24 18:39:05.000000 python_bebop-1.0.2/src/python_bebop/__init__.py
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)     4586 2023-04-24 10:26:05.000000 python_bebop-1.0.2/src/python_bebop/bebop.py
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.024514 python_bebop-1.0.2/src/python_bebop.egg-info/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/PKG-INFO
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      257 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/SOURCES.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)        1 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/dependency_links.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       13 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/top_level.txt
```

### Comparing `python_bebop-1.0.1/LICENSE` & `python_bebop-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_bebop-1.0.1/PKG-INFO` & `python_bebop-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_bebop
-Version: 1.0.1
+Version: 1.0.2
 Summary: bebop runtime bindings for Python
 Home-page: https://github.com/betwixt-labs/bebop
 Author: Korbinian Habereder
 Author-email: korbinian.habereder@gmail.com
 Project-URL: Bug Tracker, https://github.com/betwixt-labs/bebop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_bebop-1.0.1/setup.cfg` & `python_bebop-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python_bebop
-version = 1.0.1
+version = 1.0.2
 author = Korbinian Habereder
 author_email = korbinian.habereder@gmail.com
 description = bebop runtime bindings for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/betwixt-labs/bebop
 project_urls =
```

### Comparing `python_bebop-1.0.1/src/python_bebop/bebop.py` & `python_bebop-1.0.2/src/python_bebop/bebop.py`

 * *Files identical despite different names*

### Comparing `python_bebop-1.0.1/src/python_bebop.egg-info/PKG-INFO` & `python_bebop-1.0.2/src/python_bebop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bebop
-Version: 1.0.1
+Version: 1.0.2
 Summary: bebop runtime bindings for Python
 Home-page: https://github.com/betwixt-labs/bebop
 Author: Korbinian Habereder
 Author-email: korbinian.habereder@gmail.com
 Project-URL: Bug Tracker, https://github.com/betwixt-labs/bebop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

