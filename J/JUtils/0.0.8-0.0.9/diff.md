# Comparing `tmp/JUtils-0.0.8.tar.gz` & `tmp/JUtils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JUtils-0.0.8.tar", last modified: Mon Apr 10 22:29:03 2023, max compression
+gzip compressed data, was "JUtils-0.0.9.tar", last modified: Mon Apr 24 19:09:52 2023, max compression
```

## Comparing `JUtils-0.0.8.tar` & `JUtils-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.823045 JUtils-0.0.8/
--rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     8815 2023-04-10 22:29:03.823045 JUtils-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8369 2023-01-06 11:38:01.000000 JUtils-0.0.8/README.md
--rw-rw-rw-   0        0        0      522 2023-04-10 22:22:08.000000 JUtils-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 22:29:03.823045 JUtils-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.770974 JUtils-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.807173 JUtils-0.0.8/src/JUtils/
--rw-rw-rw-   0        0        0     1336 2023-01-06 11:03:26.000000 JUtils-0.0.8/src/JUtils/JArr.py
--rw-rw-rw-   0        0        0     8605 2023-01-06 11:03:27.000000 JUtils-0.0.8/src/JUtils/JColors.py
--rw-rw-rw-   0        0        0      105 2023-01-09 17:49:41.000000 JUtils-0.0.8/src/JUtils/JConst.py
--rw-rw-rw-   0        0        0     3302 2023-04-10 21:34:08.000000 JUtils-0.0.8/src/JUtils/JConv.py
--rw-rw-rw-   0        0        0     1148 2023-04-10 22:10:19.000000 JUtils-0.0.8/src/JUtils/JNum.py
--rw-rw-rw-   0        0        0      645 2023-04-10 21:58:23.000000 JUtils-0.0.8/src/JUtils/JOut.py
--rw-rw-rw-   0        0        0     2123 2023-04-10 22:21:29.000000 JUtils-0.0.8/src/JUtils/JStr.py
--rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-0.0.8/src/JUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:29:03.820987 JUtils-0.0.8/src/JUtils.egg-info/
--rw-rw-rw-   0        0        0     8815 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 22:29:03.000000 JUtils-0.0.8/src/JUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.759222 JUtils-0.0.9/
+-rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     8815 2023-04-24 19:09:52.759222 JUtils-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8369 2023-01-06 11:38:01.000000 JUtils-0.0.9/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-24 15:27:30.000000 JUtils-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:09:52.759222 JUtils-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.731665 JUtils-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.745706 JUtils-0.0.9/src/JUtils/
+-rw-rw-rw-   0        0        0     1715 2023-04-24 19:00:30.000000 JUtils-0.0.9/src/JUtils/AutoDoc.py
+-rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-0.0.9/src/JUtils/JArr.py
+-rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-0.0.9/src/JUtils/JColors.py
+-rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-0.0.9/src/JUtils/JConst.py
+-rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-0.0.9/src/JUtils/JConv.py
+-rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-0.0.9/src/JUtils/JNum.py
+-rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-0.0.9/src/JUtils/JOut.py
+-rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-0.0.9/src/JUtils/JStr.py
+-rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-0.0.9/src/JUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.757223 JUtils-0.0.9/src/JUtils.egg-info/
+-rw-rw-rw-   0        0        0     8815 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/top_level.txt
```

### Comparing `JUtils-0.0.8/LICENSE` & `JUtils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.8/PKG-INFO` & `JUtils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `JUtils-0.0.8/README.md` & `JUtils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.8/pyproject.toml` & `JUtils-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "JUtils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jan Seifert", email="jan@seifert-online.de" },
 ]
 description = "Package containing various utility functions i needed now and then, that i wanted to share"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `JUtils-0.0.8/src/JUtils/JColors.py` & `JUtils-0.0.9/src/JUtils/JColors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Color constants importable by name
+"""Color constants importable by name"""
 
 #https://htmlcolorcodes.com/color-names/
 #stripped and renamed by Jan
 
 from random import randint
 
 def randColor() -> tuple:
```

### Comparing `JUtils-0.0.8/src/JUtils/JConv.py` & `JUtils-0.0.9/src/JUtils/JConv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Functions for converting values
+"""Functions for converting values"""
 
 from math import sin, cos, sqrt, atan2, pi
 
 def rgb2hex(rgb: tuple) -> str:
     '''
     Convert an RGB tuple to a hexadecimal string representation.
```

### Comparing `JUtils-0.0.8/src/JUtils/JNum.py` & `JUtils-0.0.9/src/JUtils/JNum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Functions for handling numbers
+"""Functions for handling numbers"""
 
 def sgn(n: float) -> int:
     '''Returns the sign of a number.
 
     Parameters:
         n: An int/float number.
```

### Comparing `JUtils-0.0.8/src/JUtils/JOut.py` & `JUtils-0.0.9/src/JUtils/JOut.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Functions for handling console output
+"""Functions for handling console output"""
 
 from time import sleep
 
 def printn(*args):
     '''Prints the given arguments, with newlines before and after (works with multiple args like print)
     
     Parameters:
```

### Comparing `JUtils-0.0.8/src/JUtils/JStr.py` & `JUtils-0.0.9/src/JUtils/JStr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Functions for string analysing and modification
+"""Functions for string analysing and modification"""
 
 from os import listdir
 
 NL = '\n' #newline constant to keep code clean
 
 def locBrac(string: str, brac: str, ix: int) -> int:
     '''
```

### Comparing `JUtils-0.0.8/src/JUtils.egg-info/PKG-INFO` & `JUtils-0.0.9/src/JUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

