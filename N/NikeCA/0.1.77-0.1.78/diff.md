# Comparing `tmp/NikeCA-0.1.77.tar.gz` & `tmp/NikeCA-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.77.tar", last modified: Mon Apr 24 06:14:29 2023, max compression
+gzip compressed data, was "NikeCA-0.1.78.tar", last modified: Mon Apr 24 06:21:40 2023, max compression
```

## Comparing `NikeCA-0.1.77.tar` & `NikeCA-0.1.78.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:14:29.786421 NikeCA-0.1.77/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.77/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:14:29.785252 NikeCA-0.1.77/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.77/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 06:14:29.786569 NikeCA-0.1.77/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 06:14:19.000000 NikeCA-0.1.77/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:14:29.771808 NikeCA-0.1.77/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:14:29.774790 NikeCA-0.1.77/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3934 2023-04-21 03:17:38.000000 NikeCA-0.1.77/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:14:29.776337 NikeCA-0.1.77/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:14:29.779775 NikeCA-0.1.77/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-04-24 05:47:44.000000 NikeCA-0.1.77/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-24 05:47:44.000000 NikeCA-0.1.77/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       39 2023-04-24 06:06:29.000000 NikeCA-0.1.77/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:38.000000 NikeCA-0.1.77/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:14:29.784025 NikeCA-0.1.77/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:14:29.000000 NikeCA-0.1.77/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 06:14:29.000000 NikeCA-0.1.77/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 06:14:29.000000 NikeCA-0.1.77/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 06:14:29.000000 NikeCA-0.1.77/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 06:14:29.000000 NikeCA-0.1.77/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      414 2023-04-24 05:55:00.000000 NikeCA-0.1.77/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23528 2023-04-21 04:54:42.000000 NikeCA-0.1.77/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14111 2023-04-21 03:48:25.000000 NikeCA-0.1.77/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-21 03:17:39.000000 NikeCA-0.1.77/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:21:40.955670 NikeCA-0.1.78/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.78/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:21:40.955327 NikeCA-0.1.78/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.78/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 06:21:40.955770 NikeCA-0.1.78/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 06:21:36.000000 NikeCA-0.1.78/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:21:40.946720 NikeCA-0.1.78/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:21:40.948747 NikeCA-0.1.78/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3934 2023-04-21 03:17:38.000000 NikeCA-0.1.78/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:21:40.950006 NikeCA-0.1.78/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:21:40.951673 NikeCA-0.1.78/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-04-24 05:47:44.000000 NikeCA-0.1.78/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-24 05:47:44.000000 NikeCA-0.1.78/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       39 2023-04-24 06:06:29.000000 NikeCA-0.1.78/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:38.000000 NikeCA-0.1.78/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:21:40.954747 NikeCA-0.1.78/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:21:40.000000 NikeCA-0.1.78/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 06:21:40.000000 NikeCA-0.1.78/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 06:21:40.000000 NikeCA-0.1.78/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 06:21:40.000000 NikeCA-0.1.78/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 06:21:40.000000 NikeCA-0.1.78/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      414 2023-04-24 05:55:00.000000 NikeCA-0.1.78/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23528 2023-04-21 04:54:42.000000 NikeCA-0.1.78/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14111 2023-04-21 03:48:25.000000 NikeCA-0.1.78/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-21 03:17:39.000000 NikeCA-0.1.78/src/__init__.py
```

### Comparing `NikeCA-0.1.77/LICENSE` & `NikeCA-0.1.78/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/PKG-INFO` & `NikeCA-0.1.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.77
+Version: 0.1.78
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.77/README.md` & `NikeCA-0.1.78/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/setup.py` & `NikeCA-0.1.78/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.77',
+	version='0.1.78',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.77/src/Dashboards/Dashboards.py` & `NikeCA-0.1.78/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.78/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.78/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.78/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.77
+Version: 0.1.78
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.77/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.78/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.78/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/NikeQA.py` & `NikeCA-0.1.78/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/NikeSF.py` & `NikeCA-0.1.78/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_BuildSearchQuery.py` & `NikeCA-0.1.78/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_GitHub.py` & `NikeCA-0.1.78/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_QA.py` & `NikeCA-0.1.78/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_SearchFiles.py` & `NikeCA-0.1.78/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_SnowflakeData.py` & `NikeCA-0.1.78/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_SnowflakeDependencies.py` & `NikeCA-0.1.78/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.77/src/_SnowflakePull.py` & `NikeCA-0.1.78/src/_SnowflakePull.py`

 * *Files identical despite different names*

