# Comparing `tmp/backtracker-0.0.3.tar.gz` & `tmp/backtracker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\backtracker-0.0.3.tar", last modified: Mon Apr 24 08:05:08 2023, max compression
+gzip compressed data, was "dist\backtracker-0.0.4.tar", last modified: Mon Apr 24 08:19:08 2023, max compression
```

## Comparing `backtracker-0.0.3.tar` & `backtracker-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:05:08.127369 backtracker-0.0.3/
--rw-rw-rw-   0        0        0      632 2023-04-24 08:05:08.111710 backtracker-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-24 03:27:33.000000 backtracker-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 08:05:08.096088 backtracker-0.0.3/backtracker.egg-info/
--rw-rw-rw-   0        0        0      632 2023-04-24 08:05:07.000000 backtracker-0.0.3/backtracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-04-24 08:05:08.000000 backtracker-0.0.3/backtracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:05:07.000000 backtracker-0.0.3/backtracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 08:05:07.000000 backtracker-0.0.3/backtracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 08:05:08.127369 backtracker-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1091 2023-04-24 07:59:03.000000 backtracker-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:05:08.111710 backtracker-0.0.3/src/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:20:13.000000 backtracker-0.0.3/src/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-04-24 07:14:08.000000 backtracker-0.0.3/src/backtracker.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:05:08.111710 backtracker-0.0.3/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:58:25.000000 backtracker-0.0.3/src/tests/__init__.py
--rw-rw-rw-   0        0        0      957 2023-04-24 07:36:29.000000 backtracker-0.0.3/src/tests/test_backtracker.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:08.741618 backtracker-0.0.4/
+-rw-rw-rw-   0        0        0      632 2023-04-24 08:19:08.741618 backtracker-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-24 03:27:33.000000 backtracker-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:08.710374 backtracker-0.0.4/backtracker/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:20:13.000000 backtracker-0.0.4/backtracker/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-04-24 07:14:08.000000 backtracker-0.0.4/backtracker/backtracker.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:08.741618 backtracker-0.0.4/backtracker/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:58:25.000000 backtracker-0.0.4/backtracker/tests/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-04-24 08:17:26.000000 backtracker-0.0.4/backtracker/tests/test_backtracker.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:08.725995 backtracker-0.0.4/backtracker.egg-info/
+-rw-rw-rw-   0        0        0      632 2023-04-24 08:19:08.000000 backtracker-0.0.4/backtracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-24 08:19:08.000000 backtracker-0.0.4/backtracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:19:08.000000 backtracker-0.0.4/backtracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 08:19:08.000000 backtracker-0.0.4/backtracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:19:08.741618 backtracker-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-24 08:19:02.000000 backtracker-0.0.4/setup.py
```

### Comparing `backtracker-0.0.3/PKG-INFO` & `backtracker-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: backtracker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Backtracking Python package
 Home-page: UNKNOWN
 Author: Ryan Najafi
 Author-email: ryan.m.najafi@gmail.com
 License: UNKNOWN
 Description: Generic implementation of a backtracker algorithm based on Steven Skiena in python.
 Keywords: python,backtracker
```

### Comparing `backtracker-0.0.3/backtracker.egg-info/PKG-INFO` & `backtracker-0.0.4/backtracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: backtracker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Backtracking Python package
 Home-page: UNKNOWN
 Author: Ryan Najafi
 Author-email: ryan.m.najafi@gmail.com
 License: UNKNOWN
 Description: Generic implementation of a backtracker algorithm based on Steven Skiena in python.
 Keywords: python,backtracker
```

### Comparing `backtracker-0.0.3/setup.py` & `backtracker-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Backtracking Python package'
 LONG_DESCRIPTION = 'Generic implementation of a backtracker algorithm based on Steven Skiena in python.'
 
 # Setting up
 setup(
-       # the name must match the folder name 'verysimplemodule'
+       # the name must match the folder name
         name="backtracker", 
         version=VERSION,
         author="Ryan Najafi",
         author_email="ryan.m.najafi@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
```

### Comparing `backtracker-0.0.3/src/backtracker.py` & `backtracker-0.0.4/backtracker/backtracker.py`

 * *Files identical despite different names*

### Comparing `backtracker-0.0.3/src/tests/test_backtracker.py` & `backtracker-0.0.4/backtracker/tests/test_backtracker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src import backtracker as bt
+from backtracker import backtracker as bt
 
 
 def test_backtracker_subsets():
     a = []
     k = 0
     input = ['a', 'b', 'c', 'd']
```

