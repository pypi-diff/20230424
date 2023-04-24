# Comparing `tmp/NikeCA-0.1.81.tar.gz` & `tmp/NikeCA-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.81.tar", last modified: Mon Apr 24 07:02:42 2023, max compression
+gzip compressed data, was "NikeCA-0.1.82.tar", last modified: Mon Apr 24 07:06:20 2023, max compression
```

## Comparing `NikeCA-0.1.81.tar` & `NikeCA-0.1.82.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:02:42.293687 NikeCA-0.1.81/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.81/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:02:42.293120 NikeCA-0.1.81/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.81/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 07:02:42.293821 NikeCA-0.1.81/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 07:02:37.000000 NikeCA-0.1.81/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:02:42.286665 NikeCA-0.1.81/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:02:42.287589 NikeCA-0.1.81/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4073 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:02:42.288554 NikeCA-0.1.81/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:02:42.289957 NikeCA-0.1.81/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5903 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6677 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:02:42.292493 NikeCA-0.1.81/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:02:42.000000 NikeCA-0.1.81/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 07:02:42.000000 NikeCA-0.1.81/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 07:02:42.000000 NikeCA-0.1.81/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 07:02:42.000000 NikeCA-0.1.81/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 07:02:42.000000 NikeCA-0.1.81/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      332 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23561 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:01:59.000000 NikeCA-0.1.81/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.971609 NikeCA-0.1.82/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.82/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:06:20.971327 NikeCA-0.1.82/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.82/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-24 07:06:20.971693 NikeCA-0.1.82/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2504 2023-04-24 07:05:44.000000 NikeCA-0.1.82/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.966243 NikeCA-0.1.82/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.967122 NikeCA-0.1.82/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.967912 NikeCA-0.1.82/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.969169 NikeCA-0.1.82/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5903 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6622 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-24 07:06:20.970905 NikeCA-0.1.82/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-04-24 07:06:20.000000 NikeCA-0.1.82/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      332 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23561 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-04-24 07:05:21.000000 NikeCA-0.1.82/src/__init__.py
```

### Comparing `NikeCA-0.1.81/LICENSE` & `NikeCA-0.1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/PKG-INFO` & `NikeCA-0.1.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.81
+Version: 0.1.82
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.81/README.md` & `NikeCA-0.1.82/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/setup.py` & `NikeCA-0.1.82/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.81',
+	version='0.1.82',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.81/src/Dashboards/Dashboards.py` & `NikeCA-0.1.82/src/Dashboards/Dashboards.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 
 
 from .Telemetry.Telemetry import Telemetry
 from .InclusionExclusion.InclusionExclusion import InclusionExclusion
-from .Telemetry.Telemetry import ProductUsage
 
 
-class Dashboards(Telemetry, InclusionExclusion, ProductUsage):
+class Dashboards(Telemetry, InclusionExclusion):
 
     Telemetry = Telemetry()
-    Telemetry.ProductUsage = ProductUsage()
     InclusionExclusion = InclusionExclusion()
 
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
```

### Comparing `NikeCA-0.1.81/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.82/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.82/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.82/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 
 
-from .ProductUsage import ProductUsage
-
-
-class Telemetry(ProductUsage):
+class Telemetry:
 
     class ProductUsage:
         def product_viewed(self
                            , username: str
                            , warehouse: str
                            , database: str
                            , role: str
```

### Comparing `NikeCA-0.1.81/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.82/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.81
+Version: 0.1.82
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.81/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.82/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.82/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/NikeQA.py` & `NikeCA-0.1.82/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/NikeSF.py` & `NikeCA-0.1.82/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_BuildSearchQuery.py` & `NikeCA-0.1.82/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_GitHub.py` & `NikeCA-0.1.82/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_QA.py` & `NikeCA-0.1.82/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_SearchFiles.py` & `NikeCA-0.1.82/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_SnowflakeData.py` & `NikeCA-0.1.82/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_SnowflakeDependencies.py` & `NikeCA-0.1.82/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.81/src/_SnowflakePull.py` & `NikeCA-0.1.82/src/_SnowflakePull.py`

 * *Files identical despite different names*

