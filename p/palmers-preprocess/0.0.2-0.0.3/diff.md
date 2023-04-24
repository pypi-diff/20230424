# Comparing `tmp/palmers_preprocess-0.0.2.tar.gz` & `tmp/palmers_preprocess-0.0.3.tar.gz`

## Comparing `palmers_preprocess-0.0.2.tar` & `palmers_preprocess-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/sdatta_packages.iml
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/src/palmers_preprocess/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/src/palmers_preprocess/example.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/sdatta_packages.iml
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/src/palmers_preprocess/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/src/palmers_preprocess/example.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.3/PKG-INFO
```

### Comparing `palmers_preprocess-0.0.2/.idea/workspace.xml` & `palmers_preprocess-0.0.3/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `palmers_preprocess-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.2/LICENSE` & `palmers_preprocess-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.2/pyproject.toml` & `palmers_preprocess-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_preprocess"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_preprocess-0.0.2/PKG-INFO` & `palmers_preprocess-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_preprocess
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

