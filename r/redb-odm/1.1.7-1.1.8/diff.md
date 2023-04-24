# Comparing `tmp/redb-odm-1.1.7.tar.gz` & `tmp/redb-odm-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.1.7.tar", last modified: Mon Apr 17 16:31:26 2023, max compression
+gzip compressed data, was "redb-odm-1.1.8.tar", last modified: Mon Apr 24 14:59:31 2023, max compression
```

## Comparing `redb-odm-1.1.7.tar` & `redb-odm-1.1.8.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 16:31:10.000000 redb-odm-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 16:31:26.051141 redb-odm-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 16:31:10.000000 redb-odm-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.047141 redb-odm-1.1.7/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 16:31:10.000000 redb-odm-1.1.7/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 16:31:26.000000 redb-odm-1.1.7/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 16:31:10.000000 redb-odm-1.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 16:31:10.000000 redb-odm-1.1.7/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 16:31:10.000000 redb-odm-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:31:26.051141 redb-odm-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-17 16:31:10.000000 redb-odm-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:31:26.051141 redb-odm-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 16:31:10.000000 redb-odm-1.1.7/tests/test_soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.862716 redb-odm-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 14:59:14.000000 redb-odm-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 14:59:31.862716 redb-odm-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 14:59:14.000000 redb-odm-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.850715 redb-odm-1.1.8/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.850715 redb-odm-1.1.8/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.854715 redb-odm-1.1.8/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.854715 redb-odm-1.1.8/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:59:14.000000 redb-odm-1.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 14:59:14.000000 redb-odm-1.1.8/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 14:59:14.000000 redb-odm-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:59:31.862716 redb-odm-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 14:59:14.000000 redb-odm-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.862716 redb-odm-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_soft_deletion.py
```

### Comparing `redb-odm-1.1.7/redb/behaviors/soft_deletion.py` & `redb-odm-1.1.8/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/core/base.py` & `redb-odm-1.1.8/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/core/document.py` & `redb-odm-1.1.8/redb/core/document.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/core/instance.py` & `redb-odm-1.1.8/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/core/transaction.py` & `redb-odm-1.1.8/redb/core/transaction.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/interface/client.py` & `redb-odm-1.1.8/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/interface/collection.py` & `redb-odm-1.1.8/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/interface/configs.py` & `redb-odm-1.1.8/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/interface/database.py` & `redb-odm-1.1.8/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/interface/fields.py` & `redb-odm-1.1.8/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/interface/results.py` & `redb-odm-1.1.8/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/json_system/client.py` & `redb-odm-1.1.8/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/json_system/collection.py` & `redb-odm-1.1.8/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/json_system/database.py` & `redb-odm-1.1.8/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/migo_system/client.py` & `redb-odm-1.1.8/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/migo_system/collection.py` & `redb-odm-1.1.8/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/migo_system/database.py` & `redb-odm-1.1.8/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/mongo_system/client.py` & `redb-odm-1.1.8/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/mongo_system/collection.py` & `redb-odm-1.1.8/redb/mongo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb/mongo_system/database.py` & `redb-odm-1.1.8/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.1.8/redb_odm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 redb/behaviors/__init__.py
 redb/behaviors/soft_deletion.py
 redb/core/__init__.py
 redb/core/base.py
 redb/core/document.py
 redb/core/instance.py
 redb/core/transaction.py
+redb/core/utils.py
 redb/interface/__init__.py
 redb/interface/client.py
 redb/interface/collection.py
 redb/interface/configs.py
 redb/interface/database.py
 redb/interface/errors.py
 redb/interface/fields.py
```

### Comparing `redb-odm-1.1.7/setup.py` & `redb-odm-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/tests/test_bson_objs.py` & `redb-odm-1.1.8/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/tests/test_hashing.py` & `redb-odm-1.1.8/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/tests/test_json_client.py` & `redb-odm-1.1.8/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/tests/test_mongo_system.py` & `redb-odm-1.1.8/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/tests/test_return_cls.py` & `redb-odm-1.1.8/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.7/tests/test_soft_deletion.py` & `redb-odm-1.1.8/tests/test_soft_deletion.py`

 * *Files identical despite different names*

