# Comparing `tmp/TimeForge-0.1.2.tar.gz` & `tmp/TimeForge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.2.tar", last modified: Mon Apr 24 11:18:36 2023, max compression
+gzip compressed data, was "TimeForge-0.1.3.tar", last modified: Mon Apr 24 11:53:50 2023, max compression
```

## Comparing `TimeForge-0.1.2.tar` & `TimeForge-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:18:36.969528 TimeForge-0.1.2/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.2/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 11:18:36.969528 TimeForge-0.1.2/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-24 11:17:24.000000 TimeForge-0.1.2/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 11:18:36.969528 TimeForge-0.1.2/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:18:36.966194 TimeForge-0.1.2/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:18:36.969528 TimeForge-0.1.2/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 11:18:36.000000 TimeForge-0.1.2/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-04-24 11:18:36.000000 TimeForge-0.1.2/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 11:18:36.000000 TimeForge-0.1.2/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 11:18:36.000000 TimeForge-0.1.2/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 11:18:36.000000 TimeForge-0.1.2/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:18:36.969528 TimeForge-0.1.2/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.2/src/timeforge/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:49.000000 TimeForge-0.1.2/src/timeforge/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6497 2023-04-24 09:06:11.000000 TimeForge-0.1.2/src/timeforge/timeforge.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.354179 TimeForge-0.1.3/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.3/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 11:53:50.354179 TimeForge-0.1.3/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-24 11:53:39.000000 TimeForge-0.1.3/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 11:53:50.354179 TimeForge-0.1.3/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.350845 TimeForge-0.1.3/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.354179 TimeForge-0.1.3/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      298 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 11:53:50.000000 TimeForge-0.1.3/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 11:53:50.354179 TimeForge-0.1.3/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.3/src/timeforge/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:49.000000 TimeForge-0.1.3/src/timeforge/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6626 2023-04-24 11:49:59.000000 TimeForge-0.1.3/src/timeforge/timeforge.py
```

### Comparing `TimeForge-0.1.2/LICENSE.md` & `TimeForge-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.2/PKG-INFO` & `TimeForge-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.2/pyproject.toml` & `TimeForge-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `TimeForge-0.1.2/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.3/src/TimeForge.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.2/src/timeforge/timeforge.py` & `TimeForge-0.1.3/src/timeforge/timeforge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 
 import argparse, argcomplete
+from datetime import date, timedelta, datetime, time
 
 parser = argparse.ArgumentParser(
     prog='TimeForge',
     description = 'Create fake but realistic looking working time documentation for your student job at KIT',
     epilog='For further information take a look at the Repository for this program: https://github.com/MitchiLaser/timeforge')
 
 parser.add_argument('-n', '--name', type=str, required=True,
                    help='Name of the working person')
 
-parser.add_argument('-m', '--month', type=int, required=True,
-                    help='The month in which the job was done')
+parser.add_argument('-m', '--month', type=int, default= datetime.now().month,
+                    help='The month in which the job was done, default value will be taken from the system clock')
 
-parser.add_argument('-y', '--year', type=int, required=True,
-                    help='the year in which the work was done')
+parser.add_argument('-y', '--year', type=int, default= datetime.now().year,
+                    help='the year in which the work was done, default value will be taken from the system clock')
 
 parser.add_argument('-t', '--time', type=float, required=True,
                     help='the amount of working time in a month') 
 
 parser.add_argument('-p', '--personell', type=int, required=True,
                     help='personell number (please do not put it in quotation marks')
 
@@ -70,15 +71,14 @@
 #########################################
 
 # prevent autopep8 from moving these imports to the front
 if True:
     import sys, os
     from deutschland import feiertage
     from deutschland.feiertage.api import default_api
-    from datetime import date, timedelta, datetime, time
     from pypdf import PdfReader, PdfWriter
 
 #########################################
 
 with feiertage.ApiClient() as api_client:
     api_instance = default_api.DefaultApi(api_client)
     nur_land = "BW" # only check for the federal state of Baden-Württemberg
```

