# Comparing `tmp/TimeForge-0.1.3.tar.gz` & `tmp/TimeForge-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.3.tar", last modified: Mon Apr 24 11:53:50 2023, max compression
+gzip compressed data, was "TimeForge-0.1.4.tar", last modified: Mon Apr 24 12:48:29 2023, max compression
```

## Comparing `TimeForge-0.1.3.tar` & `TimeForge-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.354179 TimeForge-0.1.3/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.3/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 11:53:50.354179 TimeForge-0.1.3/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.3/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-24 11:53:39.000000 TimeForge-0.1.3/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 11:53:50.354179 TimeForge-0.1.3/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.350845 TimeForge-0.1.3/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.354179 TimeForge-0.1.3/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.354179 TimeForge-0.1.3/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.3/src/timeforge/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:49.000000 TimeForge-0.1.3/src/timeforge/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6626 2023-04-24 11:49:59.000000 TimeForge-0.1.3/src/timeforge/timeforge.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.4/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 12:48:29.403894 TimeForge-0.1.4/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.4/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-24 12:48:24.000000 TimeForge-0.1.4/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 12:48:29.403894 TimeForge-0.1.4/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.4/src/timeforge/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6626 2023-04-24 11:49:59.000000 TimeForge-0.1.4/src/timeforge/__main__.py
```

### Comparing `TimeForge-0.1.3/LICENSE.md` & `TimeForge-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.3/PKG-INFO` & `TimeForge-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.3/pyproject.toml` & `TimeForge-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `TimeForge-0.1.3/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.4/src/TimeForge.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.3/src/timeforge/timeforge.py` & `TimeForge-0.1.4/src/timeforge/__main__.py`

 * *Files identical despite different names*

