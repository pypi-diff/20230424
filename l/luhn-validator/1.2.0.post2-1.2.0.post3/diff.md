# Comparing `tmp/luhn-validator-1.2.0.post2.tar.gz` & `tmp/luhn-validator-1.2.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luhn-validator-1.2.0.post2.tar", last modified: Mon Apr 24 18:07:42 2023, max compression
+gzip compressed data, was "luhn-validator-1.2.0.post3.tar", last modified: Mon Apr 24 18:09:30 2023, max compression
```

## Comparing `luhn-validator-1.2.0.post2.tar` & `luhn-validator-1.2.0.post3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:07:42.731102 luhn-validator-1.2.0.post2/
--rw-r--r--   0 mohd       (501) staff       (20)     1993 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post2/CHANGELOG.md
--rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post2/LICENSE
--rw-r--r--   0 mohd       (501) staff       (20)       63 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post2/MANIFEST.in
--rw-r--r--   0 mohd       (501) staff       (20)      756 2023-04-24 18:07:42.731153 luhn-validator-1.2.0.post2/PKG-INFO
--rw-r--r--   0 mohd       (501) staff       (20)      336 2023-04-24 18:07:29.000000 luhn-validator-1.2.0.post2/README.md
--rw-r--r--   0 mohd       (501) staff       (20)     1155 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post2/pyproject.toml
--rw-r--r--   0 mohd       (501) staff       (20)      660 2023-04-24 18:07:42.731386 luhn-validator-1.2.0.post2/setup.cfg
--rw-r--r--   0 mohd       (501) staff       (20)      298 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post2/setup.py
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:07:42.728374 luhn-validator-1.2.0.post2/src/
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:07:42.729826 luhn-validator-1.2.0.post2/src/luhn_validator/
--rw-r--r--   0 mohd       (501) staff       (20)     1667 2023-04-24 18:07:36.000000 luhn-validator-1.2.0.post2/src/luhn_validator/__init__.py
--rw-r--r--   0 mohd       (501) staff       (20)       26 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post2/src/luhn_validator/py.typed
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:07:42.730755 luhn-validator-1.2.0.post2/src/luhn_validator.egg-info/
--rw-r--r--   0 mohd       (501) staff       (20)      756 2023-04-24 18:07:42.000000 luhn-validator-1.2.0.post2/src/luhn_validator.egg-info/PKG-INFO
--rw-r--r--   0 mohd       (501) staff       (20)      368 2023-04-24 18:07:42.000000 luhn-validator-1.2.0.post2/src/luhn_validator.egg-info/SOURCES.txt
--rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 18:07:42.000000 luhn-validator-1.2.0.post2/src/luhn_validator.egg-info/dependency_links.txt
--rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 03:59:30.000000 luhn-validator-1.2.0.post2/src/luhn_validator.egg-info/not-zip-safe
--rw-r--r--   0 mohd       (501) staff       (20)       15 2023-04-24 18:07:42.000000 luhn-validator-1.2.0.post2/src/luhn_validator.egg-info/top_level.txt
-drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:07:42.730887 luhn-validator-1.2.0.post2/tests/
--rw-r--r--   0 mohd       (501) staff       (20)     4893 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post2/tests/test_validator.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:09:30.032777 luhn-validator-1.2.0.post3/
+-rw-r--r--   0 mohd       (501) staff       (20)     1993 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post3/CHANGELOG.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post3/LICENSE
+-rw-r--r--   0 mohd       (501) staff       (20)       63 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post3/MANIFEST.in
+-rw-r--r--   0 mohd       (501) staff       (20)      735 2023-04-24 18:09:30.032836 luhn-validator-1.2.0.post3/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)      315 2023-04-24 18:09:16.000000 luhn-validator-1.2.0.post3/README.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1155 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post3/pyproject.toml
+-rw-r--r--   0 mohd       (501) staff       (20)      660 2023-04-24 18:09:30.033090 luhn-validator-1.2.0.post3/setup.cfg
+-rw-r--r--   0 mohd       (501) staff       (20)      298 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post3/setup.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:09:30.030634 luhn-validator-1.2.0.post3/src/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:09:30.031659 luhn-validator-1.2.0.post3/src/luhn_validator/
+-rw-r--r--   0 mohd       (501) staff       (20)     1667 2023-04-24 18:09:22.000000 luhn-validator-1.2.0.post3/src/luhn_validator/__init__.py
+-rw-r--r--   0 mohd       (501) staff       (20)       26 2023-04-23 00:13:23.000000 luhn-validator-1.2.0.post3/src/luhn_validator/py.typed
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:09:30.032537 luhn-validator-1.2.0.post3/src/luhn_validator.egg-info/
+-rw-r--r--   0 mohd       (501) staff       (20)      735 2023-04-24 18:09:30.000000 luhn-validator-1.2.0.post3/src/luhn_validator.egg-info/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)      368 2023-04-24 18:09:30.000000 luhn-validator-1.2.0.post3/src/luhn_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 18:09:30.000000 luhn-validator-1.2.0.post3/src/luhn_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 03:59:30.000000 luhn-validator-1.2.0.post3/src/luhn_validator.egg-info/not-zip-safe
+-rw-r--r--   0 mohd       (501) staff       (20)       15 2023-04-24 18:09:30.000000 luhn-validator-1.2.0.post3/src/luhn_validator.egg-info/top_level.txt
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:09:30.032663 luhn-validator-1.2.0.post3/tests/
+-rw-r--r--   0 mohd       (501) staff       (20)     4893 2023-04-24 16:47:20.000000 luhn-validator-1.2.0.post3/tests/test_validator.py
```

### Comparing `luhn-validator-1.2.0.post2/CHANGELOG.md` & `luhn-validator-1.2.0.post3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0.post2/LICENSE` & `luhn-validator-1.2.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0.post2/pyproject.toml` & `luhn-validator-1.2.0.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0.post2/setup.cfg` & `luhn-validator-1.2.0.post3/setup.cfg`

 * *Files identical despite different names*

### Comparing `luhn-validator-1.2.0.post2/src/luhn_validator/__init__.py` & `luhn-validator-1.2.0.post3/src/luhn_validator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Simple validator for identification numbers based on the Luhn algorithm.
 
 https://github.com/dralshehri/luhn-validator
 """
 
-__version__ = "1.2.0.post2"
+__version__ = "1.2.0.post3"
 
 from typing import List, Optional, Union
 
 
 def validate(
     number: str,
     length: Optional[int] = None,
```

### Comparing `luhn-validator-1.2.0.post2/tests/test_validator.py` & `luhn-validator-1.2.0.post3/tests/test_validator.py`

 * *Files identical despite different names*

