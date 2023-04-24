# Comparing `tmp/python_bebop-1.0.3.tar.gz` & `tmp/python_bebop-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bebop-1.0.3.tar", last modified: Mon Apr 24 18:53:06 2023, max compression
+gzip compressed data, was "python_bebop-1.0.4.tar", last modified: Mon Apr 24 18:56:41 2023, max compression
```

## Comparing `python_bebop-1.0.3.tar` & `python_bebop-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:53:06.804875 python_bebop-1.0.3/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)     1075 2023-04-24 10:30:47.000000 python_bebop-1.0.3/LICENSE
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:53:06.804875 python_bebop-1.0.3/PKG-INFO
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      381 2023-04-23 18:52:15.000000 python_bebop-1.0.3/README.md
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       86 2023-04-23 18:52:15.000000 python_bebop-1.0.3/pyproject.toml
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:53:06.800875 python_bebop-1.0.3/python-bebop/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:48:23.000000 python_bebop-1.0.3/python-bebop/__init__.py
--rw-rw-r--   0 secretone  (1000) secretone  (1000)     4586 2023-04-24 10:26:05.000000 python_bebop-1.0.3/python-bebop/bebop.py
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:53:06.804875 python_bebop-1.0.3/python_bebop.egg-info/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/PKG-INFO
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      233 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/SOURCES.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)        1 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/dependency_links.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       13 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/top_level.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      589 2023-04-24 18:53:06.804875 python_bebop-1.0.3/setup.cfg
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:56:41.465553 python_bebop-1.0.4/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)     1075 2023-04-24 10:30:47.000000 python_bebop-1.0.4/LICENSE
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:56:41.469553 python_bebop-1.0.4/PKG-INFO
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      381 2023-04-23 18:52:15.000000 python_bebop-1.0.4/README.md
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       86 2023-04-23 18:52:15.000000 python_bebop-1.0.4/pyproject.toml
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:56:41.465553 python_bebop-1.0.4/python_bebop/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:48:23.000000 python_bebop-1.0.4/python_bebop/__init__.py
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)     4586 2023-04-24 10:26:05.000000 python_bebop-1.0.4/python_bebop/bebop.py
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:56:41.465553 python_bebop-1.0.4/python_bebop.egg-info/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:56:41.000000 python_bebop-1.0.4/python_bebop.egg-info/PKG-INFO
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      233 2023-04-24 18:56:41.000000 python_bebop-1.0.4/python_bebop.egg-info/SOURCES.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)        1 2023-04-24 18:56:41.000000 python_bebop-1.0.4/python_bebop.egg-info/dependency_links.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       13 2023-04-24 18:56:41.000000 python_bebop-1.0.4/python_bebop.egg-info/top_level.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      589 2023-04-24 18:56:41.469553 python_bebop-1.0.4/setup.cfg
```

### Comparing `python_bebop-1.0.3/LICENSE` & `python_bebop-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_bebop-1.0.3/PKG-INFO` & `python_bebop-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_bebop
-Version: 1.0.3
+Version: 1.0.4
 Summary: bebop runtime bindings for Python
 Home-page: https://github.com/betwixt-labs/bebop
 Author: Korbinian Habereder
 Author-email: korbinian.habereder@gmail.com
 Project-URL: Bug Tracker, https://github.com/betwixt-labs/bebop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_bebop-1.0.3/python-bebop/bebop.py` & `python_bebop-1.0.4/python_bebop/bebop.py`

 * *Files identical despite different names*

### Comparing `python_bebop-1.0.3/python_bebop.egg-info/PKG-INFO` & `python_bebop-1.0.4/python_bebop.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bebop
-Version: 1.0.3
+Version: 1.0.4
 Summary: bebop runtime bindings for Python
 Home-page: https://github.com/betwixt-labs/bebop
 Author: Korbinian Habereder
 Author-email: korbinian.habereder@gmail.com
 Project-URL: Bug Tracker, https://github.com/betwixt-labs/bebop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_bebop-1.0.3/setup.cfg` & `python_bebop-1.0.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python_bebop
-version = 1.0.3
+version = 1.0.4
 author = Korbinian Habereder
 author_email = korbinian.habereder@gmail.com
 description = bebop runtime bindings for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/betwixt-labs/bebop
 project_urls =
```

