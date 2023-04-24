# Comparing `tmp/coscontents-2023.1005.tar.gz` & `tmp/coscontents-2023.1006.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coscontents-2023.1005.tar", last modified: Sun Apr 23 19:51:01 2023, max compression
+gzip compressed data, was "coscontents-2023.1006.tar", last modified: Mon Apr 24 18:34:54 2023, max compression
```

## Comparing `coscontents-2023.1005.tar` & `coscontents-2023.1006.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gines      (501) staff       (20)        0 2023-04-23 19:51:01.534973 coscontents-2023.1005/
--rw-r--r--   0 gines      (501) staff       (20)    11357 2023-03-31 07:24:34.000000 coscontents-2023.1005/LICENSE
--rw-r--r--   0 gines      (501) staff       (20)    17541 2023-04-23 19:51:01.534105 coscontents-2023.1005/PKG-INFO
--rw-r--r--   0 gines      (501) staff       (20)     4011 2023-04-02 18:31:47.000000 coscontents-2023.1005/README.md
-drwxr-xr-x   0 gines      (501) staff       (20)        0 2023-04-23 19:51:01.530736 coscontents-2023.1005/coscontents/
--rw-r--r--   0 gines      (501) staff       (20)      167 2023-04-02 18:23:10.000000 coscontents-2023.1005/coscontents/__init__.py
--rw-rw-r--   0 gines      (501) staff       (20)     1580 2023-04-02 18:19:10.000000 coscontents-2023.1005/coscontents/api_utils.py
--rw-r--r--   0 gines      (501) staff       (20)     1620 2023-03-31 08:02:44.000000 coscontents-2023.1005/coscontents/chunks.py
--rw-r--r--   0 gines      (501) staff       (20)     5573 2023-03-31 10:51:01.000000 coscontents-2023.1005/coscontents/coscontents.py
--rw-r--r--   0 gines      (501) staff       (20)     1864 2023-03-31 10:06:39.000000 coscontents-2023.1005/coscontents/genericfs.py
--rw-r--r--   0 gines      (501) staff       (20)    18381 2023-03-31 11:06:34.000000 coscontents-2023.1005/coscontents/genericmanager.py
--rw-rw-r--   0 gines      (501) staff       (20)     9691 2023-04-23 19:35:42.000000 coscontents-2023.1005/coscontents/hybridmanager.py
--rw-r--r--   0 gines      (501) staff       (20)    11175 2023-03-31 10:48:35.000000 coscontents-2023.1005/coscontents/s3_fs.py
-drwxr-xr-x   0 gines      (501) staff       (20)        0 2023-04-23 19:51:01.533514 coscontents-2023.1005/coscontents.egg-info/
--rw-r--r--   0 gines      (501) staff       (20)    17541 2023-04-23 19:51:01.000000 coscontents-2023.1005/coscontents.egg-info/PKG-INFO
--rw-r--r--   0 gines      (501) staff       (20)      418 2023-04-23 19:51:01.000000 coscontents-2023.1005/coscontents.egg-info/SOURCES.txt
--rw-r--r--   0 gines      (501) staff       (20)        1 2023-04-23 19:51:01.000000 coscontents-2023.1005/coscontents.egg-info/dependency_links.txt
--rw-r--r--   0 gines      (501) staff       (20)      111 2023-04-23 19:51:01.000000 coscontents-2023.1005/coscontents.egg-info/requires.txt
--rw-r--r--   0 gines      (501) staff       (20)       12 2023-04-23 19:51:01.000000 coscontents-2023.1005/coscontents.egg-info/top_level.txt
--rw-r--r--   0 gines      (501) staff       (20)     1203 2023-04-23 19:42:59.000000 coscontents-2023.1005/pyproject.toml
--rw-r--r--   0 gines      (501) staff       (20)       38 2023-04-23 19:51:01.535085 coscontents-2023.1005/setup.cfg
--rw-r--r--   0 gines      (501) staff       (20)       49 2023-04-01 10:03:43.000000 coscontents-2023.1005/setup.py
+drwxr-xr-x   0 gines      (501) staff       (20)        0 2023-04-24 18:34:54.220311 coscontents-2023.1006/
+-rw-r--r--   0 gines      (501) staff       (20)    11357 2023-03-31 07:24:34.000000 coscontents-2023.1006/LICENSE
+-rw-r--r--   0 gines      (501) staff       (20)    17541 2023-04-24 18:34:54.219836 coscontents-2023.1006/PKG-INFO
+-rw-r--r--   0 gines      (501) staff       (20)     4011 2023-04-02 18:31:47.000000 coscontents-2023.1006/README.md
+drwxr-xr-x   0 gines      (501) staff       (20)        0 2023-04-24 18:34:54.216332 coscontents-2023.1006/coscontents/
+-rw-r--r--   0 gines      (501) staff       (20)      167 2023-04-02 18:23:10.000000 coscontents-2023.1006/coscontents/__init__.py
+-rw-rw-r--   0 gines      (501) staff       (20)     1580 2023-04-02 18:19:10.000000 coscontents-2023.1006/coscontents/api_utils.py
+-rw-r--r--   0 gines      (501) staff       (20)     1620 2023-03-31 08:02:44.000000 coscontents-2023.1006/coscontents/chunks.py
+-rw-r--r--   0 gines      (501) staff       (20)     5573 2023-03-31 10:51:01.000000 coscontents-2023.1006/coscontents/coscontents.py
+-rw-r--r--   0 gines      (501) staff       (20)     1864 2023-03-31 10:06:39.000000 coscontents-2023.1006/coscontents/genericfs.py
+-rw-r--r--   0 gines      (501) staff       (20)    18381 2023-03-31 11:06:34.000000 coscontents-2023.1006/coscontents/genericmanager.py
+-rw-rw-r--   0 gines      (501) staff       (20)     9702 2023-04-24 18:33:22.000000 coscontents-2023.1006/coscontents/hybridmanager.py
+-rw-r--r--   0 gines      (501) staff       (20)    11175 2023-03-31 10:48:35.000000 coscontents-2023.1006/coscontents/s3_fs.py
+drwxr-xr-x   0 gines      (501) staff       (20)        0 2023-04-24 18:34:54.219119 coscontents-2023.1006/coscontents.egg-info/
+-rw-r--r--   0 gines      (501) staff       (20)    17541 2023-04-24 18:34:54.000000 coscontents-2023.1006/coscontents.egg-info/PKG-INFO
+-rw-r--r--   0 gines      (501) staff       (20)      418 2023-04-24 18:34:54.000000 coscontents-2023.1006/coscontents.egg-info/SOURCES.txt
+-rw-r--r--   0 gines      (501) staff       (20)        1 2023-04-24 18:34:54.000000 coscontents-2023.1006/coscontents.egg-info/dependency_links.txt
+-rw-r--r--   0 gines      (501) staff       (20)      111 2023-04-24 18:34:54.000000 coscontents-2023.1006/coscontents.egg-info/requires.txt
+-rw-r--r--   0 gines      (501) staff       (20)       12 2023-04-24 18:34:54.000000 coscontents-2023.1006/coscontents.egg-info/top_level.txt
+-rw-r--r--   0 gines      (501) staff       (20)     1203 2023-04-24 18:33:42.000000 coscontents-2023.1006/pyproject.toml
+-rw-r--r--   0 gines      (501) staff       (20)       38 2023-04-24 18:34:54.220481 coscontents-2023.1006/setup.cfg
+-rw-r--r--   0 gines      (501) staff       (20)       49 2023-04-01 10:03:43.000000 coscontents-2023.1006/setup.py
```

### Comparing `coscontents-2023.1005/LICENSE` & `coscontents-2023.1006/LICENSE`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/PKG-INFO` & `coscontents-2023.1006/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscontents
-Version: 2023.1005
+Version: 2023.1006
 Summary: COS Contents Manage for storing Jupyterlab Notebooks in IBM Cloud Object Storage
 Author-email: Gines Carrascal <gines_carrascal@es.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `coscontents-2023.1005/README.md` & `coscontents-2023.1006/README.md`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents/api_utils.py` & `coscontents-2023.1006/coscontents/api_utils.py`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents/chunks.py` & `coscontents-2023.1006/coscontents/chunks.py`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents/coscontents.py` & `coscontents-2023.1006/coscontents/coscontents.py`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents/genericfs.py` & `coscontents-2023.1006/coscontents/genericfs.py`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents/genericmanager.py` & `coscontents-2023.1006/coscontents/genericmanager.py`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents/hybridmanager.py` & `coscontents-2023.1006/coscontents/hybridmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 @outside_root_to_404
 def _resolve_path(path, manager_dict):
     """Resolve a path based on a dictionary of manager prefixes.
 
     Returns a triple of (prefix, manager, manager_relative_path).
     """
-    path = normalize_api_path(path)
+    path = normalize_api_path(path).strip('/')
     parts = path.split('/')
 
     # Try to find a sub-manager for the first subdirectory.
     mgr = manager_dict.get(parts[0])
     if mgr is not None:
         return parts[0], mgr, '/'.join(parts[1:])
```

### Comparing `coscontents-2023.1005/coscontents/s3_fs.py` & `coscontents-2023.1006/coscontents/s3_fs.py`

 * *Files identical despite different names*

### Comparing `coscontents-2023.1005/coscontents.egg-info/PKG-INFO` & `coscontents-2023.1006/coscontents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscontents
-Version: 2023.1005
+Version: 2023.1006
 Summary: COS Contents Manage for storing Jupyterlab Notebooks in IBM Cloud Object Storage
 Author-email: Gines Carrascal <gines_carrascal@es.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `coscontents-2023.1005/pyproject.toml` & `coscontents-2023.1006/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coscontents"
-version = "2023.1005"
+version = "2023.1006"
 description = "COS Contents Manage for storing Jupyterlab Notebooks in IBM Cloud Object Storage"
 readme = "README.md"
 authors = [{ name = "Gines Carrascal", email = "gines_carrascal@es.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
```

