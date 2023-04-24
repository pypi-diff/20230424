# Comparing `tmp/TimeForge-0.1.0.tar.gz` & `tmp/TimeForge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.0.tar", last modified: Mon Apr 24 09:07:08 2023, max compression
+gzip compressed data, was "TimeForge-0.1.1.tar", last modified: Mon Apr 24 09:09:25 2023, max compression
```

## Comparing `TimeForge-0.1.0.tar` & `TimeForge-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.908790 TimeForge-0.1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.0/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 09:07:08.908790 TimeForge-0.1.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-17 13:44:59.000000 TimeForge-0.1.0/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 09:07:08.908790 TimeForge-0.1.0/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.905456 TimeForge-0.1.0/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.908790 TimeForge-0.1.0/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      274 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.908790 TimeForge-0.1.0/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)     2986 2023-04-05 15:27:53.000000 TimeForge-0.1.0/src/timeforge/generation.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6497 2023-04-24 09:06:11.000000 TimeForge-0.1.0/src/timeforge/timeforge.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:09:25.784276 TimeForge-0.1.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.1/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 09:09:25.780943 TimeForge-0.1.1/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-24 09:08:47.000000 TimeForge-0.1.1/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 09:09:25.784276 TimeForge-0.1.1/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:09:25.780943 TimeForge-0.1.1/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:09:25.780943 TimeForge-0.1.1/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 09:09:25.000000 TimeForge-0.1.1/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-04-24 09:09:25.000000 TimeForge-0.1.1/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 09:09:25.000000 TimeForge-0.1.1/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 09:09:25.000000 TimeForge-0.1.1/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 09:09:25.000000 TimeForge-0.1.1/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:09:25.780943 TimeForge-0.1.1/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6497 2023-04-24 09:06:11.000000 TimeForge-0.1.1/src/timeforge/timeforge.py
```

### Comparing `TimeForge-0.1.0/LICENSE.md` & `TimeForge-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.0/PKG-INFO` & `TimeForge-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.0/pyproject.toml` & `TimeForge-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `TimeForge-0.1.0/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.1/src/TimeForge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.0/src/timeforge/timeforge.py` & `TimeForge-0.1.1/src/timeforge/timeforge.py`

 * *Files identical despite different names*

