# Comparing `tmp/newtgw-0.0.4.tar.gz` & `tmp/newtgw-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newtgw-0.0.4.tar", last modified: Mon Apr 24 11:51:06 2023, max compression
+gzip compressed data, was "newtgw-0.0.5.tar", last modified: Mon Apr 24 12:01:09 2023, max compression
```

## Comparing `newtgw-0.0.4.tar` & `newtgw-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:51:06.772557 newtgw-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 11:50:51.000000 newtgw-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 11:50:51.000000 newtgw-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 11:51:06.772557 newtgw-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 11:50:51.000000 newtgw-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 11:50:51.000000 newtgw-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:51:06.772557 newtgw-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-24 11:50:51.000000 newtgw-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:51:06.768557 newtgw-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:51:06.772557 newtgw-0.0.4/src/newtgw/
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-24 11:50:51.000000 newtgw-0.0.4/src/newtgw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:51:06.772557 newtgw-0.0.4/src/newtgw/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 11:50:51.000000 newtgw-0.0.4/src/newtgw/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23098 2023-04-24 11:50:51.000000 newtgw-0.0.4/src/newtgw/_jsii/newtgw@0.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:50:51.000000 newtgw-0.0.4/src/newtgw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:51:06.772557 newtgw-0.0.4/src/newtgw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 11:51:06.000000 newtgw-0.0.4/src/newtgw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 11:51:06.000000 newtgw-0.0.4/src/newtgw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:51:06.000000 newtgw-0.0.4/src/newtgw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 11:51:06.000000 newtgw-0.0.4/src/newtgw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 11:51:06.000000 newtgw-0.0.4/src/newtgw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:09.399881 newtgw-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 12:00:58.000000 newtgw-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 12:00:58.000000 newtgw-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 12:01:09.399881 newtgw-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 12:00:58.000000 newtgw-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 12:00:58.000000 newtgw-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:01:09.399881 newtgw-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-24 12:00:58.000000 newtgw-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:09.395881 newtgw-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:09.399881 newtgw-0.0.5/src/newtgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-04-24 12:00:58.000000 newtgw-0.0.5/src/newtgw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:09.399881 newtgw-0.0.5/src/newtgw/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 12:00:58.000000 newtgw-0.0.5/src/newtgw/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-04-24 12:00:58.000000 newtgw-0.0.5/src/newtgw/_jsii/newtgw@0.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:00:58.000000 newtgw-0.0.5/src/newtgw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:09.399881 newtgw-0.0.5/src/newtgw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 12:01:09.000000 newtgw-0.0.5/src/newtgw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 12:01:09.000000 newtgw-0.0.5/src/newtgw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:01:09.000000 newtgw-0.0.5/src/newtgw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 12:01:09.000000 newtgw-0.0.5/src/newtgw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 12:01:09.000000 newtgw-0.0.5/src/newtgw.egg-info/top_level.txt
```

### Comparing `newtgw-0.0.4/LICENSE` & `newtgw-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `newtgw-0.0.4/PKG-INFO` & `newtgw-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtgw
-Version: 0.0.4
+Version: 0.0.5
 Summary: newtgw
 Home-page: https://github.com/cmorgia/newtgw.git
 Author: Claudio Morgia<cmorgia@amazon.ch>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cmorgia/newtgw.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `newtgw-0.0.4/setup.py` & `newtgw-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "newtgw",
-    "version": "0.0.4",
+    "version": "0.0.5",
     "description": "newtgw",
     "license": "Apache-2.0",
     "url": "https://github.com/cmorgia/newtgw.git",
     "long_description_content_type": "text/markdown",
     "author": "Claudio Morgia<cmorgia@amazon.ch>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "newtgw",
         "newtgw._jsii"
     ],
     "package_data": {
         "newtgw._jsii": [
-            "newtgw@0.0.4.jsii.tgz"
+            "newtgw@0.0.5.jsii.tgz"
         ],
         "newtgw": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `newtgw-0.0.4/src/newtgw/__init__.py` & `newtgw-0.0.5/src/newtgw/__init__.py`

 * *Files identical despite different names*

### Comparing `newtgw-0.0.4/src/newtgw.egg-info/PKG-INFO` & `newtgw-0.0.5/src/newtgw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtgw
-Version: 0.0.4
+Version: 0.0.5
 Summary: newtgw
 Home-page: https://github.com/cmorgia/newtgw.git
 Author: Claudio Morgia<cmorgia@amazon.ch>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cmorgia/newtgw.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

