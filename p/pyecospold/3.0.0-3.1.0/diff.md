# Comparing `tmp/pyecospold-3.0.0.tar.gz` & `tmp/pyecospold-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecospold-3.0.0.tar", last modified: Mon Mar 27 01:55:13 2023, max compression
+gzip compressed data, was "pyecospold-3.1.0.tar", last modified: Mon Apr 24 13:29:58 2023, max compression
```

## Comparing `pyecospold-3.0.0.tar` & `pyecospold-3.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.520601 pyecospold-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-27 01:55:04.000000 pyecospold-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 01:55:04.000000 pyecospold-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-27 01:55:13.520601 pyecospold-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-03-27 01:55:04.000000 pyecospold-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.516601 pyecospold-3.0.0/pyecospold/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58157 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/model_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    93293 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/model_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.512601 pyecospold-3.0.0/pyecospold/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.516601 pyecospold-3.0.0/pyecospold/schemas/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventCategories.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventUnits.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    59234 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v1/XmlNamespace.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.516601 pyecospold-3.0.0/pyecospold/schemas/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    52466 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    70861 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    49965 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    52230 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/schemas/v2/XmlNamespace.xsd
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyecospold/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.520601 pyecospold-3.0.0/pyecospold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-27 01:55:13.000000 pyecospold-3.0.0/pyecospold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-27 01:55:13.000000 pyecospold-3.0.0/pyecospold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 01:55:13.000000 pyecospold-3.0.0/pyecospold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 01:55:13.000000 pyecospold-3.0.0/pyecospold.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-27 01:55:13.000000 pyecospold-3.0.0/pyecospold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-27 01:55:13.000000 pyecospold-3.0.0/pyecospold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 01:55:04.000000 pyecospold-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-27 01:55:13.520601 pyecospold-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 01:55:13.520601 pyecospold-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-27 01:55:04.000000 pyecospold-3.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-03-27 01:55:04.000000 pyecospold-3.0.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-27 01:55:04.000000 pyecospold-3.0.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-03-27 01:55:04.000000 pyecospold-3.0.0/tests/test_model_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    30087 2023-03-27 01:55:04.000000 pyecospold-3.0.0/tests/test_model_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.056487 pyecospold-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-24 13:29:46.000000 pyecospold-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 13:29:46.000000 pyecospold-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-24 13:29:58.056487 pyecospold-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-24 13:29:46.000000 pyecospold-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.052487 pyecospold-3.1.0/pyecospold/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58157 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94861 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/model_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.040488 pyecospold-3.1.0/pyecospold/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.048488 pyecospold-3.1.0/pyecospold/schemas/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCategories.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventUnits.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    59234 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v1/XmlNamespace.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.052487 pyecospold-3.1.0/pyecospold/schemas/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    52466 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    70861 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    49965 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    52230 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/schemas/v2/XmlNamespace.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyecospold/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.056487 pyecospold-3.1.0/pyecospold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:29:57.000000 pyecospold-3.1.0/pyecospold.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-24 13:29:58.000000 pyecospold-3.1.0/pyecospold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 13:29:46.000000 pyecospold-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-24 13:29:58.056487 pyecospold-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:29:58.056487 pyecospold-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18094 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30087 2023-04-24 13:29:46.000000 pyecospold-3.1.0/tests/test_model_v2.py
```

### Comparing `pyecospold-3.0.0/LICENSE` & `pyecospold-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/PKG-INFO` & `pyecospold-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecospold
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Python package that converts ecospold XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyecospold
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: BSD license
```

### Comparing `pyecospold-3.0.0/README.md` & `pyecospold-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/config.py` & `pyecospold-3.1.0/pyecospold/config.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/core.py` & `pyecospold-3.1.0/pyecospold/core.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/helpers.py` & `pyecospold-3.1.0/pyecospold/helpers.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/model_v1.py` & `pyecospold-3.1.0/pyecospold/model_v1.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/model_v2.py` & `pyecospold-3.1.0/pyecospold/model_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1089,14 +1089,40 @@
         """Uncertainty of the transfer coefficient amount."""
         return get_element_list(self, "uncertainty")
 
 
 class IntermediateExchange(CustomExchange):
     """Comprises intermediate product and waste inputs and outputs for the activity."""
 
+    INPUT_GROUP_MAP: Dict[int, str] = {
+        1: "Materials/Fuels",
+        2: "Electricity/Heat",
+        3: "Services",
+        5: "From Technosphere (unspecified)",
+    }
+
+    OUTPUT_GROUP_MAP: Dict[int, str] = {
+        0: "ReferenceProduct",
+        2: "By-product",
+        3: "MaterialForTreatment",
+        5: "Stock Additions",
+    }
+
+    inputGroup = create_element_text_v2("inputGroup", int)
+    """int: Indicates the kind of input flow. The codes are: 1=Materials/Fuels,
+    2=Electricity/Heat, 3=Services, 5=From Technosphere (unspecified). For each
+    exchange only an inputGroup or outputGroup shall exist. This indicates the
+    direction of the flow."""
+
+    outputGroup = create_element_text_v2("outputGroup", int)
+    """int: Indicates the kind of output flow. The codes are: 0=ReferenceProduct,
+    2=By-product, 3=MaterialForTreatment, 5=Stock Additions. For each exchange only
+    an inputGroup or outputGroup shall exist. This indicates the direction of the
+    flow."""
+
     productionVolumeComments = create_attribute_list_v2("productionVolumeComments", str)
     """lits[str]: A general comment can be made on the data source, assumptions and
     calculations for the production volume data."""
 
     intermediateExchangeId = create_attribute_v2("intermediateExchangeId", str)
     """str: Reference to the master data entry for this intermediate exchange"""
 
@@ -1166,14 +1192,27 @@
     )
     """str: Indicates the first author by surname and abbreviated name
     (e.g., Einstein A.). In case of measurement on site, oral communication, personal
     written communication and questionnaries ('sourceType'=4, 5, 6, 7) the name of the
     communicating person is"""
 
     @property
+    def inputGroupStr(self) -> str:
+        """String representation for inputGroup. See inputGroup for explanations.
+        1=Materials/Fuels, 2=Electricity/Heat, 3=Services, 5=From Technosphere
+        (unspecified)."""
+        return self.INPUT_GROUP_MAP[self.inputGroup]
+
+    @property
+    def outputGroupStr(self) -> str:
+        """String representation for outputGroup. See outputGroup for explanations.
+        0=ReferenceProduct, 2=By-product, 3=MaterialForTreatment, 5=Stock Additions."""
+        return self.OUTPUT_GROUP_MAP[self.outputGroup]
+
+    @property
     def productionVolumeUncertainties(self) -> List["Uncertainty"]:
         """Uncertainty information in the form of distribution functions and their
         parameters and/or pedigree data."""
         return get_element_list(self, "productionVolumeUncertainty")
 
     @property
     def classifications(self) -> List["Classification"]:
```

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventCategories.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCategories.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoInventUnits.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoInventUnits.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01Dataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01FlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v1/XmlNamespace.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v1/XmlNamespace.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02Activity.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02FlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/schemas/v2/XmlNamespace.xsd` & `pyecospold-3.1.0/pyecospold/schemas/v2/XmlNamespace.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold/version.py` & `pyecospold-3.1.0/pyecospold/version.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/pyecospold.egg-info/PKG-INFO` & `pyecospold-3.1.0/pyecospold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecospold
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Python package that converts ecospold XML formats to their Python equivalents and export the same data back to XML.
 Home-page: https://github.com/sami-m-g/pyecospold
 Author: Mina Sami
 Author-email: <sami.mg@outlook.com>
 Maintainer: Mina Sami
 Maintainer-email: <sami.mg@outlook.com>
 License: BSD license
```

### Comparing `pyecospold-3.0.0/pyecospold.egg-info/SOURCES.txt` & `pyecospold-3.1.0/pyecospold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/setup.cfg` & `pyecospold-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/tests/test_config.py` & `pyecospold-3.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/tests/test_core.py` & `pyecospold-3.1.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/tests/test_helpers.py` & `pyecospold-3.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/tests/test_model_v1.py` & `pyecospold-3.1.0/tests/test_model_v1.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.0.0/tests/test_model_v2.py` & `pyecospold-3.1.0/tests/test_model_v2.py`

 * *Files identical despite different names*

