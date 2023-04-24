# Comparing `tmp/python_bebop-1.0.2.tar.gz` & `tmp/python_bebop-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bebop-1.0.2.tar", last modified: Mon Apr 24 18:40:38 2023, max compression
+gzip compressed data, was "python_bebop-1.0.3.tar", last modified: Mon Apr 24 18:53:06 2023, max compression
```

## Comparing `python_bebop-1.0.2.tar` & `python_bebop-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.024514 python_bebop-1.0.2/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)     1075 2023-04-24 10:30:47.000000 python_bebop-1.0.2/LICENSE
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:40:38.024514 python_bebop-1.0.2/PKG-INFO
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      381 2023-04-23 18:52:15.000000 python_bebop-1.0.2/README.md
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       86 2023-04-23 18:52:15.000000 python_bebop-1.0.2/pyproject.toml
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      648 2023-04-24 18:40:38.024514 python_bebop-1.0.2/setup.cfg
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.020514 python_bebop-1.0.2/src/
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.020514 python_bebop-1.0.2/src/python_bebop/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       42 2023-04-24 18:39:05.000000 python_bebop-1.0.2/src/python_bebop/__init__.py
--rw-rw-r--   0 secretone  (1000) secretone  (1000)     4586 2023-04-24 10:26:05.000000 python_bebop-1.0.2/src/python_bebop/bebop.py
-drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:40:38.024514 python_bebop-1.0.2/src/python_bebop.egg-info/
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/PKG-INFO
--rw-rw-r--   0 secretone  (1000) secretone  (1000)      257 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/SOURCES.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)        1 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/dependency_links.txt
--rw-rw-r--   0 secretone  (1000) secretone  (1000)       13 2023-04-24 18:40:38.000000 python_bebop-1.0.2/src/python_bebop.egg-info/top_level.txt
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:53:06.804875 python_bebop-1.0.3/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)     1075 2023-04-24 10:30:47.000000 python_bebop-1.0.3/LICENSE
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:53:06.804875 python_bebop-1.0.3/PKG-INFO
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      381 2023-04-23 18:52:15.000000 python_bebop-1.0.3/README.md
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       86 2023-04-23 18:52:15.000000 python_bebop-1.0.3/pyproject.toml
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:53:06.800875 python_bebop-1.0.3/python-bebop/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:48:23.000000 python_bebop-1.0.3/python-bebop/__init__.py
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)     4586 2023-04-24 10:26:05.000000 python_bebop-1.0.3/python-bebop/bebop.py
+drwxrwxr-x   0 secretone  (1000) secretone  (1000)        0 2023-04-24 18:53:06.804875 python_bebop-1.0.3/python_bebop.egg-info/
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      905 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/PKG-INFO
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      233 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/SOURCES.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)        1 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/dependency_links.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)       13 2023-04-24 18:53:06.000000 python_bebop-1.0.3/python_bebop.egg-info/top_level.txt
+-rw-rw-r--   0 secretone  (1000) secretone  (1000)      589 2023-04-24 18:53:06.804875 python_bebop-1.0.3/setup.cfg
```

### Comparing `python_bebop-1.0.2/LICENSE` & `python_bebop-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_bebop-1.0.2/PKG-INFO` & `python_bebop-1.0.3/python_bebop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_bebop
-Version: 1.0.2
+Name: python-bebop
+Version: 1.0.3
 Summary: bebop runtime bindings for Python
 Home-page: https://github.com/betwixt-labs/bebop
 Author: Korbinian Habereder
 Author-email: korbinian.habereder@gmail.com
 Project-URL: Bug Tracker, https://github.com/betwixt-labs/bebop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python_bebop-1.0.2/src/python_bebop/bebop.py` & `python_bebop-1.0.3/python-bebop/bebop.py`

 * *Files identical despite different names*

### Comparing `python_bebop-1.0.2/src/python_bebop.egg-info/PKG-INFO` & `python_bebop-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-bebop
-Version: 1.0.2
+Name: python_bebop
+Version: 1.0.3
 Summary: bebop runtime bindings for Python
 Home-page: https://github.com/betwixt-labs/bebop
 Author: Korbinian Habereder
 Author-email: korbinian.habereder@gmail.com
 Project-URL: Bug Tracker, https://github.com/betwixt-labs/bebop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

