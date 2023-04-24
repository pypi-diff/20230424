# Comparing `tmp/NikeCA-0.1.79.tar.gz` & `tmp/NikeCA-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.79.tar", last modified: Mon Apr 24 06:29:59 2023, max compression
+gzip compressed data, was "NikeCA-0.1.80.tar", last modified: Mon Apr 24 06:57:49 2023, max compression
```

## Comparing `NikeCA-0.1.79.tar` & `NikeCA-0.1.80.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:59.950999 NikeCA-0.1.79/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.79/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:29:59.950535 NikeCA-0.1.79/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.79/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 06:29:59.951114 NikeCA-0.1.79/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 06:29:54.000000 NikeCA-0.1.79/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:59.944451 NikeCA-0.1.79/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:59.945430 NikeCA-0.1.79/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3990 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:59.946340 NikeCA-0.1.79/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:59.947938 NikeCA-0.1.79/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      103 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:29:59.949933 NikeCA-0.1.79/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:29:59.000000 NikeCA-0.1.79/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 06:29:59.000000 NikeCA-0.1.79/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 06:29:59.000000 NikeCA-0.1.79/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 06:29:59.000000 NikeCA-0.1.79/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 06:29:59.000000 NikeCA-0.1.79/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      417 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23636 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 06:29:20.000000 NikeCA-0.1.79/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:57:49.012164 NikeCA-0.1.80/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.80/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:57:49.011881 NikeCA-0.1.80/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.80/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 06:57:49.012251 NikeCA-0.1.80/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 06:57:43.000000 NikeCA-0.1.80/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:57:49.007192 NikeCA-0.1.80/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:57:49.008071 NikeCA-0.1.80/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4073 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:57:49.008745 NikeCA-0.1.80/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:57:49.009741 NikeCA-0.1.80/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5903 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       87 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 06:57:49.011475 NikeCA-0.1.80/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 06:57:48.000000 NikeCA-0.1.80/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 06:57:48.000000 NikeCA-0.1.80/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 06:57:48.000000 NikeCA-0.1.80/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 06:57:48.000000 NikeCA-0.1.80/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 06:57:48.000000 NikeCA-0.1.80/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      330 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23561 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 06:56:49.000000 NikeCA-0.1.80/src/__init__.py
```

### Comparing `NikeCA-0.1.79/LICENSE` & `NikeCA-0.1.80/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/PKG-INFO` & `NikeCA-0.1.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.79
+Version: 0.1.80
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.79/README.md` & `NikeCA-0.1.80/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/setup.py` & `NikeCA-0.1.80/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.79',
+	version='0.1.80',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.79/src/Dashboards/Dashboards.py` & `NikeCA-0.1.80/src/Dashboards/Dashboards.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 
 from .Telemetry.Telemetry import Telemetry
 from .InclusionExclusion.InclusionExclusion import InclusionExclusion
+from .Telemetry.Telemetry import ProductUsage
 
 
-class Dashboards:
+class Dashboards(Telemetry, InclusionExclusion, ProductUsage):
 
     Telemetry = Telemetry()
-    Telemetry.ProductUsage = Telemetry.ProductUsage()
-    InclusionExclusion = InclusionExclusion
+    Telemetry.ProductUsage = ProductUsage()
+    InclusionExclusion = InclusionExclusion()
 
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
                               , date_min: str = '1900-01-01'
```

### Comparing `NikeCA-0.1.79/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.80/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.80/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 class ProductUsage:
 
+
     def get_base_query(self
                        , filters: list | None = None
                        , start_date: str = '1900-01-01'
                        , end_date: str = '9999-12-31'
                        ):
 
         import configparser
```

### Comparing `NikeCA-0.1.79/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.80/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.79
+Version: 0.1.80
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.79/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.80/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.80/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/NikeQA.py` & `NikeCA-0.1.80/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/NikeSF.py` & `NikeCA-0.1.80/src/NikeSF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
 from Dashboards.Dashboards import Dashboards
 from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
-from Dashboards.Telemetry.Telemetry import Telemetry, ProductUsage
 
 
-class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery, InclusionExclusion, Telemetry,
-                ProductUsage):
+class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):#, InclusionExclusion):
+
+    Dashboards = Dashboards
+
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
     def __init__(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
```

### Comparing `NikeCA-0.1.79/src/_BuildSearchQuery.py` & `NikeCA-0.1.80/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/_GitHub.py` & `NikeCA-0.1.80/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/_QA.py` & `NikeCA-0.1.80/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/_SearchFiles.py` & `NikeCA-0.1.80/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/_SnowflakeData.py` & `NikeCA-0.1.80/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/_SnowflakeDependencies.py` & `NikeCA-0.1.80/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.79/src/_SnowflakePull.py` & `NikeCA-0.1.80/src/_SnowflakePull.py`

 * *Files identical despite different names*

