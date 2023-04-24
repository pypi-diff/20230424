# Comparing `tmp/luhn-validator-1.2.0.tar.gz` & `tmp/luhn-validator-1.2.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luhn-validator-1.2.0.tar", last modified: Mon Apr 24 16:51:44 2023, max compression
+gzip compressed data, was "luhn-validator-1.2.0.post4.tar", last modified: Mon Apr 24 18:12:05 2023, max compression
```

## Comparing `luhn-validator-1.2.0.tar` & `luhn-validator-1.2.0.post4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 16:51:44.330870 luhn-validator-1.2.0/
--rw-r--r--   0 mohd       (501) staff       (20)     1993 2023-04-24 16:47:20.000000 luhn-validator-1.2.0/CHANGELOG.md
--rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-23 00:13:23.000000 luhn-validator-1.2.0/LICENSE
--rw-r--r--   0 mohd       (501) staff       (20)       63 2023-04-24 16:47:20.000000 luhn-validator-1.2.0/MANIFEST.in
--rw-r--r--   0 mohd       (501) staff       (20)      768 2023-04-24 16:51:44.330914 luhn-validator-1.2.0/PKG-INFO
--rw-r--r--   0 mohd       (501) staff       (20)      354 2023-04-24 16:47:21.000000 luhn-validator-1.2.0/README.md
--rw-r--r--   0 mohd       (501) staff       (20)     1155 2023-04-23 00:13:23.000000 luhn-validator-1.2.0/pyproject.toml
--rw-r--r--   0 mohd       (501) staff       (20)      660 2023-04-24 16:51:44.331142 luhn-validator-1.2.0/setup.cfg
--rw-r--r--   0 mohd       (501) staff       (20)      298 2023-04-24 16:47:20.000000 luhn-validator-1.2.0/setup.py
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 16:51:44.328688 luhn-validator-1.2.0/src/
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 16:51:44.329902 luhn-validator-1.2.0/src/luhn_validator/
--rw-r--r--   0 mohd       (501) staff       (20)     1661 2023-04-24 16:47:20.000000 luhn-validator-1.2.0/src/luhn_validator/__init__.py
--rw-r--r--   0 mohd       (501) staff       (20)       26 2023-04-23 00:13:23.000000 luhn-validator-1.2.0/src/luhn_validator/py.typed
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 16:51:44.330666 luhn-validator-1.2.0/src/luhn_validator.egg-info/
--rw-r--r--   0 mohd       (501) staff       (20)      768 2023-04-24 16:51:44.000000 luhn-validator-1.2.0/src/luhn_validator.egg-info/PKG-INFO
--rw-r--r--   0 mohd       (501) staff       (20)      368 2023-04-24 16:51:44.000000 luhn-validator-1.2.0/src/luhn_validator.egg-info/SOURCES.txt
--rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 16:51:44.000000 luhn-validator-1.2.0/src/luhn_validator.egg-info/dependency_links.txt
--rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 03:59:30.000000 luhn-validator-1.2.0/src/luhn_validator.egg-info/not-zip-safe
--rw-r--r--   0 mohd       (501) staff       (20)       15 2023-04-24 16:51:44.000000 luhn-validator-1.2.0/src/luhn_validator.egg-info/top_level.txt
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 16:51:44.330777 luhn-validator-1.2.0/tests/
--rw-r--r--   0 mohd       (501) staff       (20)     4893 2023-04-24 16:47:20.000000 luhn-validator-1.2.0/tests/test_validator.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:12:05.828027 luhn-validator-1.2.0.post4/
+-rw-r--r--   0 mohd       (501) staff       (20)     1993 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post4/CHANGELOG.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post4/LICENSE
+-rw-r--r--   0 mohd       (501) staff       (20)       63 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post4/MANIFEST.in
+-rw-r--r--   0 mohd       (501) staff       (20)      744 2023-04-24 18:12:05.828074 luhn-validator-1.2.0.post4/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)      324 2023-04-24 18:10:58.000000 luhn-validator-1.2.0.post4/README.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1155 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post4/pyproject.toml
+-rw-r--r--   0 mohd       (501) staff       (20)      660 2023-04-24 18:12:05.828298 luhn-validator-1.2.0.post4/setup.cfg
+-rw-r--r--   0 mohd       (501) staff       (20)      298 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post4/setup.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:12:05.825729 luhn-validator-1.2.0.post4/src/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:12:05.827052 luhn-validator-1.2.0.post4/src/luhn_validator/
+-rw-r--r--   0 mohd       (501) staff       (20)     1667 2023-04-24 18:11:58.000000 luhn-validator-1.2.0.post4/src/luhn_validator/__init__.py
+-rw-r--r--   0 mohd       (501) staff       (20)       26 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post4/src/luhn_validator/py.typed
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:12:05.827813 luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/
+-rw-r--r--   0 mohd       (501) staff       (20)      744 2023-04-24 18:12:05.000000 luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)      368 2023-04-24 18:12:05.000000 luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 18:12:05.000000 luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 03:59:30.000000 luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/not-zip-safe
+-rw-r--r--   0 mohd       (501) staff       (20)       15 2023-04-24 18:12:05.000000 luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/top_level.txt
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:12:05.827914 luhn-validator-1.2.0.post4/tests/
+-rw-r--r--   0 mohd       (501) staff       (20)     4893 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post4/tests/test_validator.py
```

### Comparing `luhn-validator-1.2.0/CHANGELOG.md` & `luhn-validator-1.2.0.post4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0/LICENSE` & `luhn-validator-1.2.0.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0/PKG-INFO` & `luhn-validator-1.2.0.post4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luhn-validator
-Version: 1.2.0
+Version: 1.2.0.post4
 Summary: Simple validator for identification numbers based on the Luhn algorithm
 Home-page: 
 Author: Mohammed Alshehri
 Author-email: 
 License: MIT
 Keywords: luhn,validator,validation,numbers,identification,imei,credit-card
 Classifier: Development Status :: 7 - Inactive
@@ -13,14 +13,12 @@
 License-File: LICENSE
 
 # luhn-validator
 
 A Python package to validate identification numbers using the Luhn algorithm
 with additional optional checks.
 
-> ⚠️⚠️⚠️
+> ⚠️ **Deprecation Notice**
 >
-> The `luhn-validator` package has been **deprecated** and will not receive
-> future updates. Please use the
-> [`luhncheck`](https://pypi.org/project/luhncheck/) package instead.
->
-> ⚠️⚠️⚠️
+> This package has been **deprecated** and will not receive future updates.
+> Please use the [luhncheck](https://pypi.org/project/luhncheck/) package
+> instead.
```

### Comparing `luhn-validator-1.2.0/pyproject.toml` & `luhn-validator-1.2.0.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0/setup.cfg` & `luhn-validator-1.2.0.post4/setup.cfg`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0/src/luhn_validator/__init__.py` & `luhn-validator-1.2.0.post4/src/luhn_validator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Simple validator for identification numbers based on the Luhn algorithm.
 
 https://github.com/dralshehri/luhn-validator
 """
 
-__version__ = "1.2.0"
+__version__ = "1.2.0.post4"
 
 from typing import List, Optional, Union
 
 
 def validate(
     number: str,
     length: Optional[int] = None,
```

### Comparing `luhn-validator-1.2.0/src/luhn_validator.egg-info/PKG-INFO` & `luhn-validator-1.2.0.post4/src/luhn_validator.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luhn-validator
-Version: 1.2.0
+Version: 1.2.0.post4
 Summary: Simple validator for identification numbers based on the Luhn algorithm
 Home-page: 
 Author: Mohammed Alshehri
 Author-email: 
 License: MIT
 Keywords: luhn,validator,validation,numbers,identification,imei,credit-card
 Classifier: Development Status :: 7 - Inactive
@@ -13,14 +13,12 @@
 License-File: LICENSE
 
 # luhn-validator
 
 A Python package to validate identification numbers using the Luhn algorithm
 with additional optional checks.
 
-> ⚠️⚠️⚠️
+> ⚠️ **Deprecation Notice**
 >
-> The `luhn-validator` package has been **deprecated** and will not receive
-> future updates. Please use the
-> [`luhncheck`](https://pypi.org/project/luhncheck/) package instead.
->
-> ⚠️⚠️⚠️
+> This package has been **deprecated** and will not receive future updates.
+> Please use the [luhncheck](https://pypi.org/project/luhncheck/) package
+> instead.
```

### Comparing `luhn-validator-1.2.0/tests/test_validator.py` & `luhn-validator-1.2.0.post4/tests/test_validator.py`

 * *Files identical despite different names*

