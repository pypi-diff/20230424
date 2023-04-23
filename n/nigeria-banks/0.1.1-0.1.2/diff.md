# Comparing `tmp/nigeria_banks-0.1.1.tar.gz` & `tmp/nigeria_banks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nigeria_banks-0.1.1.tar", last modified: Sun Aug 28 20:47:46 2022, max compression
+gzip compressed data, was "nigeria_banks-0.1.2.tar", last modified: Sun Apr 23 23:51:51 2023, max compression
```

## Comparing `nigeria_banks-0.1.1.tar` & `nigeria_banks-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:46.803473 nigeria_banks-0.1.1/cbn_banks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/cbn_banks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/cbn_banks/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/cbn_banks/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/cbn_banks/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/cbn_banks/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5271 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/cbn_banks/database/db.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/nigeria_banks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/nigeria_banks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/nigeria_banks/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/nigeria_banks/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/nigeria_banks/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/nigeria_banks/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9469 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/nigeria_banks/database/db.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/nigeria_banks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-08-28 20:47:46.000000 nigeria_banks-0.1.1/nigeria_banks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-08-28 20:47:46.000000 nigeria_banks-0.1.1/nigeria_banks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 20:47:46.000000 nigeria_banks-0.1.1/nigeria_banks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-28 20:47:46.000000 nigeria_banks-0.1.1/nigeria_banks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-28 20:47:46.807473 nigeria_banks-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-08-28 20:47:37.000000 nigeria_banks-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/cbn_banks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/cbn_banks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/cbn_banks/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/cbn_banks/bank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/cbn_banks/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/cbn_banks/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/cbn_banks/database/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/nigeria_banks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/nigeria_banks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/nigeria_banks/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/nigeria_banks/bank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/nigeria_banks/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/nigeria_banks/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61777 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/nigeria_banks/database/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/nigeria_banks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-23 23:51:51.000000 nigeria_banks-0.1.2/nigeria_banks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-23 23:51:51.000000 nigeria_banks-0.1.2/nigeria_banks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:51:51.000000 nigeria_banks-0.1.2/nigeria_banks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 23:51:51.000000 nigeria_banks-0.1.2/nigeria_banks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 23:51:51.384814 nigeria_banks-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-23 23:51:41.000000 nigeria_banks-0.1.2/setup.py
```

### Comparing `nigeria_banks-0.1.1/LICENSE` & `nigeria_banks-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.1/PKG-INFO` & `nigeria_banks-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nigeria_banks
-Version: 0.1.1
+Version: 0.1.2
 Summary: Get details of specific bank in Nigeria
 Home-page: https://github.com/Josephchinedu/nigeria_banks
 Author: Devjoseph
 Author-email: joseph4jubilant@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nigeria_banks-0.1.1/README.md` & `nigeria_banks-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.1/cbn_banks/bank.py` & `nigeria_banks-0.1.2/cbn_banks/bank.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.1/cbn_banks/database/db.py` & `nigeria_banks-0.1.2/cbn_banks/database/db.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.1/nigeria_banks/bank.py` & `nigeria_banks-0.1.2/nigeria_banks/bank.py`

 * *Files identical despite different names*

### Comparing `nigeria_banks-0.1.1/nigeria_banks.egg-info/PKG-INFO` & `nigeria_banks-0.1.2/nigeria_banks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nigeria-banks
-Version: 0.1.1
+Version: 0.1.2
 Summary: Get details of specific bank in Nigeria
 Home-page: https://github.com/Josephchinedu/nigeria_banks
 Author: Devjoseph
 Author-email: joseph4jubilant@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nigeria_banks-0.1.1/setup.py` & `nigeria_banks-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 NAME = 'nigeria_banks'
 DESCRIPTION = 'Get details of specific bank in Nigeria'
 URL = 'https://github.com/Josephchinedu/nigeria_banks'
 EMAIL = 'joseph4jubilant@gmail.com'
 AUTHOR = 'Devjoseph'
 REQUIRES_PYTHON = '>=3.7.9'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
 EXTRAS = {
```

