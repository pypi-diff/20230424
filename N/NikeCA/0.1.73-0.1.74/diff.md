# Comparing `tmp/NikeCA-0.1.73.tar.gz` & `tmp/NikeCA-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.73.tar", last modified: Mon Apr 24 05:33:38 2023, max compression
+gzip compressed data, was "NikeCA-0.1.74.tar", last modified: Mon Apr 24 05:41:26 2023, max compression
```

## Comparing `NikeCA-0.1.73.tar` & `NikeCA-0.1.74.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:33:38.151099 NikeCA-0.1.73/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.73/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 05:33:38.150651 NikeCA-0.1.73/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.73/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 05:33:38.151231 NikeCA-0.1.73/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 05:33:06.000000 NikeCA-0.1.73/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:33:38.140276 NikeCA-0.1.73/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:33:38.143105 NikeCA-0.1.73/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3934 2023-04-21 03:17:38.000000 NikeCA-0.1.73/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:33:38.144383 NikeCA-0.1.73/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:33:38.146972 NikeCA-0.1.73/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:38.000000 NikeCA-0.1.73/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:33:38.149880 NikeCA-0.1.73/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 05:33:37.000000 NikeCA-0.1.73/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 05:33:37.000000 NikeCA-0.1.73/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 05:33:37.000000 NikeCA-0.1.73/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 05:33:37.000000 NikeCA-0.1.73/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 05:33:37.000000 NikeCA-0.1.73/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23528 2023-04-21 04:54:42.000000 NikeCA-0.1.73/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14111 2023-04-21 03:48:25.000000 NikeCA-0.1.73/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-21 03:17:39.000000 NikeCA-0.1.73/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:41:26.656527 NikeCA-0.1.74/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.74/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 05:41:26.656029 NikeCA-0.1.74/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.74/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 05:41:26.656682 NikeCA-0.1.74/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 05:41:06.000000 NikeCA-0.1.74/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:41:26.648741 NikeCA-0.1.74/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:41:26.650686 NikeCA-0.1.74/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3934 2023-04-21 03:17:38.000000 NikeCA-0.1.74/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:41:26.651851 NikeCA-0.1.74/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:41:26.653726 NikeCA-0.1.74/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)      253 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       94 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-21 03:17:38.000000 NikeCA-0.1.74/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 05:41:26.655473 NikeCA-0.1.74/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 05:41:26.000000 NikeCA-0.1.74/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 05:41:26.000000 NikeCA-0.1.74/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 05:41:26.000000 NikeCA-0.1.74/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 05:41:26.000000 NikeCA-0.1.74/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 05:41:26.000000 NikeCA-0.1.74/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23528 2023-04-21 04:54:42.000000 NikeCA-0.1.74/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14111 2023-04-21 03:48:25.000000 NikeCA-0.1.74/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-21 03:17:39.000000 NikeCA-0.1.74/src/__init__.py
```

### Comparing `NikeCA-0.1.73/LICENSE` & `NikeCA-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/PKG-INFO` & `NikeCA-0.1.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.73
+Version: 0.1.74
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.73/README.md` & `NikeCA-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/setup.py` & `NikeCA-0.1.74/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.73',
+	version='0.1.74',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.73/src/Dashboards/Dashboards.py` & `NikeCA-0.1.74/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.74/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.74/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.73
+Version: 0.1.74
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.73/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.74/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.74/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/NikeQA.py` & `NikeCA-0.1.74/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/NikeSF.py` & `NikeCA-0.1.74/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_BuildSearchQuery.py` & `NikeCA-0.1.74/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_GitHub.py` & `NikeCA-0.1.74/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_QA.py` & `NikeCA-0.1.74/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_SearchFiles.py` & `NikeCA-0.1.74/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_SnowflakeData.py` & `NikeCA-0.1.74/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_SnowflakeDependencies.py` & `NikeCA-0.1.74/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.73/src/_SnowflakePull.py` & `NikeCA-0.1.74/src/_SnowflakePull.py`

 * *Files identical despite different names*

