# Comparing `tmp/TimeForge-0.0.1.tar.gz` & `tmp/TimeForge-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.0.1.tar", last modified: Tue Apr  4 12:07:19 2023, max compression
+gzip compressed data, was "TimeForge-0.1.0.tar", last modified: Mon Apr 24 09:07:08 2023, max compression
```

## Comparing `TimeForge-0.0.1.tar` & `TimeForge-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 12:07:19.756383 TimeForge-0.0.1/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.0.1/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)      914 2023-04-04 12:07:19.756383 TimeForge-0.0.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      241 2023-04-04 11:29:53.000000 TimeForge-0.0.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      776 2023-04-04 11:55:46.000000 TimeForge-0.0.1/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-04 12:07:19.756383 TimeForge-0.0.1/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 12:07:19.753050 TimeForge-0.0.1/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 12:07:19.756383 TimeForge-0.0.1/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)      914 2023-04-04 12:07:19.000000 TimeForge-0.0.1/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      211 2023-04-04 12:07:19.000000 TimeForge-0.0.1/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-04 12:07:19.000000 TimeForge-0.0.1/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-04 12:07:19.000000 TimeForge-0.0.1/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-04 12:07:19.756383 TimeForge-0.0.1/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)     2993 2023-04-04 11:28:34.000000 TimeForge-0.0.1/src/timeforge/generation.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.908790 TimeForge-0.1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.0/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 09:07:08.908790 TimeForge-0.1.0/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.0/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-17 13:44:59.000000 TimeForge-0.1.0/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 09:07:08.908790 TimeForge-0.1.0/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.905456 TimeForge-0.1.0/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.908790 TimeForge-0.1.0/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      274 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 09:07:08.000000 TimeForge-0.1.0/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 09:07:08.908790 TimeForge-0.1.0/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2986 2023-04-05 15:27:53.000000 TimeForge-0.1.0/src/timeforge/generation.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6497 2023-04-24 09:06:11.000000 TimeForge-0.1.0/src/timeforge/timeforge.py
```

### Comparing `TimeForge-0.0.1/LICENSE.md` & `TimeForge-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.0.1/PKG-INFO` & `TimeForge-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.0.1
+Version: 0.1.0
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
@@ -24,8 +24,14 @@
 ``` bash
 $ pip install timeforge
 ```
 
 
 ## Usage
 
-This program has currently only a command line interface.
+This program has currently only a command line interface. Use
+
+``` bash
+$ python -m timeforge --help
+```
+
+to get an overview of the functionality.
```

### Comparing `TimeForge-0.0.1/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.0/src/TimeForge.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.0.1
+Version: 0.1.0
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
@@ -24,8 +24,14 @@
 ``` bash
 $ pip install timeforge
 ```
 
 
 ## Usage
 
-This program has currently only a command line interface.
+This program has currently only a command line interface. Use
+
+``` bash
+$ python -m timeforge --help
+```
+
+to get an overview of the functionality.
```

### Comparing `TimeForge-0.0.1/src/timeforge/generation.py` & `TimeForge-0.1.0/src/timeforge/generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 job = "job"
 fields = pdf_reader.getFormTextFields()
 pdf_writer = PdfFileWriter()
 holidays = 0
 pay = 12
 personal_nr = "007"
 name = "Faula"
-oe = ""out_PDF
+oe = ""
 form_data = {
 'Std': hours,
 'Urlaub anteilig': holidays,
 'Summe': hours, 
 'monatliche SollArbeitszeit': hours, 
 'Übertrag vom Vormonat': 0, 
 'Übertrag in den Folgemonat': 0,
```

