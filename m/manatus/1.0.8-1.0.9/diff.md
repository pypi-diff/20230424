# Comparing `tmp/manatus-1.0.8.tar.gz` & `tmp/manatus-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manatus-1.0.8.tar", last modified: Tue Nov 15 19:28:32 2022, max compression
+gzip compressed data, was "manatus-1.0.9.tar", last modified: Wed Nov 16 14:42:58 2022, max compression
```

## Comparing `manatus-1.0.8.tar` & `manatus-1.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.755309 manatus-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 19:28:17.000000 manatus-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:17.000000 manatus-1.0.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-15 19:28:17.000000 manatus-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-15 19:28:17.000000 manatus-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-15 19:28:32.755309 manatus-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-15 19:28:17.000000 manatus-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.751309 manatus-1.0.8/manatus/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9630 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.751309 manatus-1.0.8/manatus/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     7061 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/cli/harvest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6115 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/cli/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/maps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/organizations.py
--rw-r--r--   0 runner    (1001) docker     (121)    19531 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (121)     8636 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/source_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.755309 manatus-1.0.8/manatus/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/harvest_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5933 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/maps_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/organiztions_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8856 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/scenarios_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4739 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/source_resource_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.755309 manatus-1.0.8/manatus/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/DCdebugSmall.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/FlMemSmall.xml
--rw-r--r--   0 runner    (1001) docker     (121)    13222 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/MODSdebugSmall.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8077 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/QDCdebugSmall.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.755309 manatus-1.0.8/manatus/tests/test_data/dc/
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/dc/usf_boucicault.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/fsu_susanbradfordeppespapers.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.755309 manatus-1.0.8/manatus/tests/test_data/mods/
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/mods/fsu_susanbradfordeppespapers.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.755309 manatus-1.0.8/manatus/tests/test_data/qdc/
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/qdc/um_chc0336.xml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/record_group_error_test
--rw-r--r--   0 runner    (1001) docker     (121)    14342 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/record_group_json.json
--rw-r--r--   0 runner    (1001) docker     (121)    10712 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/record_group_jsonl.jsonl
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/test_scenario_config.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/um_chc0336.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/test_data/usf_boucicault.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7764 2022-11-15 19:28:17.000000 manatus-1.0.8/manatus/tests/transform_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 19:28:32.751309 manatus-1.0.8/manatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-15 19:28:32.000000 manatus-1.0.8/manatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-11-15 19:28:32.000000 manatus-1.0.8/manatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 19:28:32.000000 manatus-1.0.8/manatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-15 19:28:32.000000 manatus-1.0.8/manatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-15 19:28:32.000000 manatus-1.0.8/manatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-15 19:28:17.000000 manatus-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-15 19:28:32.755309 manatus-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-11-15 19:28:17.000000 manatus-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-16 14:42:44.000000 manatus-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:44.000000 manatus-1.0.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-16 14:42:44.000000 manatus-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-16 14:42:44.000000 manatus-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-16 14:42:58.792513 manatus-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-16 14:42:44.000000 manatus-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9630 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     7061 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/cli/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6115 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/cli/transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19549 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8636 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/source_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/harvest_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5933 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/maps_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/organiztions_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8856 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/scenarios_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4739 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/source_resource_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/DCdebugSmall.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/FlMemSmall.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    13222 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/MODSdebugSmall.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     8077 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/QDCdebugSmall.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/tests/test_data/dc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/dc/usf_boucicault.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/fsu_susanbradfordeppespapers.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/tests/test_data/mods/
+-rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/mods/fsu_susanbradfordeppespapers.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus/tests/test_data/qdc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/qdc/um_chc0336.xml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/record_group_error_test
+-rw-r--r--   0 runner    (1001) docker     (121)    14342 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/record_group_json.json
+-rw-r--r--   0 runner    (1001) docker     (121)    10712 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/record_group_jsonl.jsonl
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/test_scenario_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/um_chc0336.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/test_data/usf_boucicault.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     7764 2022-11-16 14:42:44.000000 manatus-1.0.9/manatus/tests/transform_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 14:42:58.792513 manatus-1.0.9/manatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-16 14:42:58.000000 manatus-1.0.9/manatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-11-16 14:42:58.000000 manatus-1.0.9/manatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 14:42:58.000000 manatus-1.0.9/manatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-16 14:42:58.000000 manatus-1.0.9/manatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-16 14:42:58.000000 manatus-1.0.9/manatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-16 14:42:44.000000 manatus-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-16 14:42:58.792513 manatus-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-11-16 14:42:44.000000 manatus-1.0.9/setup.py
```

### Comparing `manatus-1.0.8/LICENSE` & `manatus-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/PKG-INFO` & `manatus-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manatus
-Version: 1.0.8
+Version: 1.0.9
 Summary: Metadata aggregation and transformation library
 Home-page: http://github.com/SunshineStateDigitalNetwork/manatus
 Author: Matthew Miguez
 Author-email: r.m.miguez@gmail.com
 License: MIT
 Keywords: oai-pmh metadata digital-libraries
 Platform: any
```

### Comparing `manatus-1.0.8/README.rst` & `manatus-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/__main__.py` & `manatus-1.0.9/manatus/__main__.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/cli/__init__.py` & `manatus-1.0.9/manatus/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/cli/harvest.py` & `manatus-1.0.9/manatus/cli/harvest.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/cli/transform.py` & `manatus-1.0.9/manatus/cli/transform.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/exceptions.py` & `manatus-1.0.9/manatus/exceptions.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/maps.py` & `manatus-1.0.9/manatus/maps.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/organizations.py` & `manatus-1.0.9/manatus/organizations.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/scenarios.py` & `manatus-1.0.9/manatus/scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -641,17 +641,17 @@
                 rights_info['uri'] = rights.uri
             else:
                 if rights.text.startswith('http://rightsstatements'):
                     rights_info['uri'] = rights.text
                 else:
                     rights_info['text'] = rights.text
             continue
-        if rights_info['uri']:
+        if 'uri' in rights_info.keys():
             return rights_info['uri']
-        elif rights_info['text']:
+        elif 'text' in rights_info.keys():
             return rights_info['text']
         else:
             return None
 
 
 class InternetArchiveRecord(ManatusRecord):
```

### Comparing `manatus-1.0.8/manatus/source_resource.py` & `manatus-1.0.9/manatus/source_resource.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/__init__.py` & `manatus-1.0.9/manatus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/harvest_test.py` & `manatus-1.0.9/manatus/tests/harvest_test.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/maps_test.py` & `manatus-1.0.9/manatus/tests/maps_test.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/organiztions_test.py` & `manatus-1.0.9/manatus/tests/organiztions_test.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/scenarios_test.py` & `manatus-1.0.9/manatus/tests/scenarios_test.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/source_resource_test.py` & `manatus-1.0.9/manatus/tests/source_resource_test.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/DCdebugSmall.xml` & `manatus-1.0.9/manatus/tests/test_data/DCdebugSmall.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/FlMemSmall.xml` & `manatus-1.0.9/manatus/tests/test_data/FlMemSmall.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/MODSdebugSmall.xml` & `manatus-1.0.9/manatus/tests/test_data/MODSdebugSmall.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/QDCdebugSmall.xml` & `manatus-1.0.9/manatus/tests/test_data/QDCdebugSmall.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/dc/usf_boucicault.xml` & `manatus-1.0.9/manatus/tests/test_data/dc/usf_boucicault.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/fsu_susanbradfordeppespapers.xml` & `manatus-1.0.9/manatus/tests/test_data/fsu_susanbradfordeppespapers.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/mods/fsu_susanbradfordeppespapers.xml` & `manatus-1.0.9/manatus/tests/test_data/mods/fsu_susanbradfordeppespapers.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/qdc/um_chc0336.xml` & `manatus-1.0.9/manatus/tests/test_data/qdc/um_chc0336.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/record_group_json.json` & `manatus-1.0.9/manatus/tests/test_data/record_group_json.json`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/record_group_jsonl.jsonl` & `manatus-1.0.9/manatus/tests/test_data/record_group_jsonl.jsonl`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/um_chc0336.xml` & `manatus-1.0.9/manatus/tests/test_data/um_chc0336.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/test_data/usf_boucicault.xml` & `manatus-1.0.9/manatus/tests/test_data/usf_boucicault.xml`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus/tests/transform_test.py` & `manatus-1.0.9/manatus/tests/transform_test.py`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/manatus.egg-info/PKG-INFO` & `manatus-1.0.9/manatus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manatus
-Version: 1.0.8
+Version: 1.0.9
 Summary: Metadata aggregation and transformation library
 Home-page: http://github.com/SunshineStateDigitalNetwork/manatus
 Author: Matthew Miguez
 Author-email: r.m.miguez@gmail.com
 License: MIT
 Keywords: oai-pmh metadata digital-libraries
 Platform: any
```

### Comparing `manatus-1.0.8/manatus.egg-info/SOURCES.txt` & `manatus-1.0.9/manatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manatus-1.0.8/setup.py` & `manatus-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='manatus',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     url='http://github.com/SunshineStateDigitalNetwork/manatus',
     license='MIT',
     author='Matthew Miguez',
     author_email='r.m.miguez@gmail.com',
     description='Metadata aggregation and transformation library',
     long_description=open('README.rst').read() + '\n\n' +
```

