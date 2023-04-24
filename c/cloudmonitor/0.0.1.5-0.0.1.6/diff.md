# Comparing `tmp/cloudmonitor-0.0.1.5.tar.gz` & `tmp/cloudmonitor-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmonitor-0.0.1.5.tar", last modified: Mon Apr 24 13:11:36 2023, max compression
+gzip compressed data, was "cloudmonitor-0.0.1.6.tar", last modified: Mon Apr 24 13:18:00 2023, max compression
```

## Comparing `cloudmonitor-0.0.1.5.tar` & `cloudmonitor-0.0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/
--rw-rw-r--   0 wnjxyk    (1000) wnjxyk    (1000)     1044 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      284 2023-04-23 14:47:47.000000 cloudmonitor-0.0.1.5/README.md
-drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/cloudmonitor/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-24 13:11:34.000000 cloudmonitor-0.0.1.5/cloudmonitor/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.5/cloudmonitor/__main__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2683 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.5/cloudmonitor/config.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2010 2023-04-24 13:04:20.000000 cloudmonitor-0.0.1.5/cloudmonitor/server.py
-drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/cloudmonitor/ssh/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.5/cloudmonitor/ssh/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1135 2023-04-23 14:10:51.000000 cloudmonitor-0.0.1.5/cloudmonitor/ssh/client.py
-drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/cloudmonitor/status/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.5/cloudmonitor/status/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.5/cloudmonitor/status/define.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.5/cloudmonitor/status/query.py
-drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1044 2023-04-24 13:11:36.000000 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      479 2023-04-24 13:11:36.000000 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-24 13:11:36.000000 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       85 2023-04-24 13:11:36.000000 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/entry_points.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       41 2023-04-24 13:11:36.000000 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/requires.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-24 13:11:36.000000 cloudmonitor-0.0.1.5/cloudmonitor.egg-info/top_level.txt
--rw-rw-r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-24 13:11:36.055915 cloudmonitor-0.0.1.5/setup.cfg
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2539 2023-04-23 14:25:35.000000 cloudmonitor-0.0.1.5/setup.py
+drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/
+-rw-rw-r--   0 wnjxyk    (1000) wnjxyk    (1000)     1044 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      284 2023-04-23 14:47:47.000000 cloudmonitor-0.0.1.6/README.md
+drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/cloudmonitor/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-24 13:17:56.000000 cloudmonitor-0.0.1.6/cloudmonitor/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.6/cloudmonitor/__main__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2683 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.6/cloudmonitor/config.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2010 2023-04-24 13:04:20.000000 cloudmonitor-0.0.1.6/cloudmonitor/server.py
+drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/cloudmonitor/ssh/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.6/cloudmonitor/ssh/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1135 2023-04-23 14:10:51.000000 cloudmonitor-0.0.1.6/cloudmonitor/ssh/client.py
+drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/cloudmonitor/status/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.6/cloudmonitor/status/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.6/cloudmonitor/status/define.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.6/cloudmonitor/status/query.py
+drwxrwxr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1044 2023-04-24 13:18:00.000000 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      479 2023-04-24 13:18:00.000000 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-24 13:18:00.000000 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       85 2023-04-24 13:18:00.000000 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       41 2023-04-24 13:18:00.000000 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/requires.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-24 13:18:00.000000 cloudmonitor-0.0.1.6/cloudmonitor.egg-info/top_level.txt
+-rw-rw-r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-24 13:18:00.064804 cloudmonitor-0.0.1.6/setup.cfg
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2539 2023-04-24 13:17:17.000000 cloudmonitor-0.0.1.6/setup.py
```

### Comparing `cloudmonitor-0.0.1.5/PKG-INFO` & `cloudmonitor-0.0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: A Web-GUI Monitor for Academic Linux Servers
 Home-page: https://github.com/WNJXYK/cloudmonitor
 License: MIT Licence
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
```

### Comparing `cloudmonitor-0.0.1.5/cloudmonitor/config.py` & `cloudmonitor-0.0.1.6/cloudmonitor/config.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.5/cloudmonitor/server.py` & `cloudmonitor-0.0.1.6/cloudmonitor/server.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.5/cloudmonitor/ssh/client.py` & `cloudmonitor-0.0.1.6/cloudmonitor/ssh/client.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.5/cloudmonitor/status/define.py` & `cloudmonitor-0.0.1.6/cloudmonitor/status/define.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.5/cloudmonitor/status/query.py` & `cloudmonitor-0.0.1.6/cloudmonitor/status/query.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.5/cloudmonitor.egg-info/PKG-INFO` & `cloudmonitor-0.0.1.6/cloudmonitor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: A Web-GUI Monitor for Academic Linux Servers
 Home-page: https://github.com/WNJXYK/cloudmonitor
 License: MIT Licence
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
```

### Comparing `cloudmonitor-0.0.1.5/setup.py` & `cloudmonitor-0.0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # not sure about setuptools).
 if os.path.exists("MANIFEST"):
     os.remove("MANIFEST")
 
 # What packages are required for this module to be executed?
 # `estimator` may depend on other packages. In order to reduce dependencies, it is not written here.
 REQUIRED = [
-    "flask>=2.2.2",
+    "flask>=2.0.0",
     "paramiko>=3.0.0",
     "pyyaml>=6.0",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
```

