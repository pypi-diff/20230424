# Comparing `tmp/tharos-pytools-0.0.8.tar.gz` & `tmp/tharos-pytools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tharos-pytools-0.0.8.tar", last modified: Mon Feb  6 15:35:51 2023, max compression
+gzip compressed data, was "tharos-pytools-0.0.9.tar", last modified: Wed Feb  8 10:05:00 2023, max compression
```

## Comparing `tharos-pytools-0.0.8.tar` & `tharos-pytools-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-02-06 15:35:51.520968 tharos-pytools-0.0.8/
--rw-r--r--   0 sidubois (669136) genscale (35005)     1048 2023-02-06 10:02:11.000000 tharos-pytools-0.0.8/LICENCE
--rw-r--r--   0 sidubois (669136) genscale (35005)      818 2023-02-06 15:35:51.496968 tharos-pytools-0.0.8/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      198 2023-02-06 10:49:39.000000 tharos-pytools-0.0.8/README.md
--rw-r--r--   0 sidubois (669136) genscale (35005)      610 2023-02-06 15:35:42.000000 tharos-pytools-0.0.8/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2023-02-06 15:35:51.521968 tharos-pytools-0.0.8/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)      388 2023-02-06 15:35:43.000000 tharos-pytools-0.0.8/setup.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-02-06 15:35:51.479969 tharos-pytools-0.0.8/tharos_pytools.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)      818 2023-02-06 15:35:51.000000 tharos-pytools-0.0.8/tharos_pytools.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      388 2023-02-06 15:35:51.000000 tharos-pytools-0.0.8/tharos_pytools.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-02-06 15:35:51.000000 tharos-pytools-0.0.8/tharos_pytools.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-02-06 15:35:51.000000 tharos-pytools-0.0.8/tharos_pytools.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       21 2023-02-06 15:35:51.000000 tharos-pytools-0.0.8/tharos_pytools.egg-info/requires.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)       14 2023-02-06 15:35:51.000000 tharos-pytools-0.0.8/tharos_pytools.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-02-06 15:35:51.492970 tharos-pytools-0.0.8/tharospytools/
--rw-r--r--   0 sidubois (669136) genscale (35005)      172 2023-02-06 13:04:19.000000 tharos-pytools-0.0.8/tharospytools/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     1797 2023-02-06 13:01:00.000000 tharos-pytools-0.0.8/tharospytools/matplotlib_tools.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     2442 2023-02-06 15:34:38.000000 tharos-pytools-0.0.8/tharospytools/multithreading.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      737 2023-02-06 13:03:39.000000 tharos-pytools-0.0.8/tharospytools/overloading.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-02-08 10:05:00.685582 tharos-pytools-0.0.9/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1048 2023-02-06 10:02:11.000000 tharos-pytools-0.0.9/LICENCE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1135 2023-02-08 10:05:00.684558 tharos-pytools-0.0.9/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      515 2023-02-08 10:04:24.000000 tharos-pytools-0.0.9/README.md
+-rw-r--r--   0 sidubois (669136) genscale (35005)      610 2023-02-08 09:57:26.000000 tharos-pytools-0.0.9/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2023-02-08 10:05:00.687517 tharos-pytools-0.0.9/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)      388 2023-02-08 09:57:33.000000 tharos-pytools-0.0.9/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-02-08 10:05:00.658513 tharos-pytools-0.0.9/tharos_pytools.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1135 2023-02-08 10:05:00.000000 tharos-pytools-0.0.9/tharos_pytools.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      416 2023-02-08 10:05:00.000000 tharos-pytools-0.0.9/tharos_pytools.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-02-08 10:05:00.000000 tharos-pytools-0.0.9/tharos_pytools.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-02-08 10:05:00.000000 tharos-pytools-0.0.9/tharos_pytools.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       21 2023-02-08 10:05:00.000000 tharos-pytools-0.0.9/tharos_pytools.egg-info/requires.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)       14 2023-02-08 10:05:00.000000 tharos-pytools-0.0.9/tharos_pytools.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-02-08 10:05:00.678587 tharos-pytools-0.0.9/tharospytools/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      239 2023-02-08 09:57:53.000000 tharos-pytools-0.0.9/tharospytools/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      804 2023-02-08 09:50:00.000000 tharos-pytools-0.0.9/tharospytools/list_tools.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1797 2023-02-06 13:01:00.000000 tharos-pytools-0.0.9/tharospytools/matplotlib_tools.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2442 2023-02-06 15:34:38.000000 tharos-pytools-0.0.9/tharospytools/multithreading.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      737 2023-02-06 13:03:39.000000 tharos-pytools-0.0.9/tharospytools/overloading.py
```

### Comparing `tharos-pytools-0.0.8/LICENCE` & `tharos-pytools-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `tharos-pytools-0.0.8/PKG-INFO` & `tharos-pytools-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tharos-pytools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package that packs some utility functions.
 Home-page: https://github.com/Tharos-ux/tharos-pytools
 Author: Tharos
 Author-email: Tharos <dubois.siegfried@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Tharos-ux/tharos-pytools
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/tharos-pytools/issues
@@ -14,8 +14,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # tharos-pytools
 
 This package contains cool functions in order to better manage Python projects.
-For now, it only contains functions to ensure multithreading on a function, with respect to memory.
+
+## Contents
+
++ `futures_collector` is a function that ensures multithreading.
++ `limit_memory` allows to define a percentage-based memorylock for current Python thread.
++ `get_palette` allows to create a N-sized color palette.
++ `get_palette_from_list` returns a list of colors, normalizing a data array.
++ `overload` is a decorator that allows C-like overloading of functions.
++ `flatten` is a fast list flattener.
```

### Comparing `tharos-pytools-0.0.8/pyproject.toml` & `tharos-pytools-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tharos-pytools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Tharos", email="dubois.siegfried@gmail.com" },
 ]
 description = "Package that packs some utility functions."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `tharos-pytools-0.0.8/tharos_pytools.egg-info/PKG-INFO` & `tharos-pytools-0.0.9/tharos_pytools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tharos-pytools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package that packs some utility functions.
 Home-page: https://github.com/Tharos-ux/tharos-pytools
 Author: Tharos
 Author-email: Tharos <dubois.siegfried@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Tharos-ux/tharos-pytools
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/tharos-pytools/issues
@@ -14,8 +14,16 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # tharos-pytools
 
 This package contains cool functions in order to better manage Python projects.
-For now, it only contains functions to ensure multithreading on a function, with respect to memory.
+
+## Contents
+
++ `futures_collector` is a function that ensures multithreading.
++ `limit_memory` allows to define a percentage-based memorylock for current Python thread.
++ `get_palette` allows to create a N-sized color palette.
++ `get_palette_from_list` returns a list of colors, normalizing a data array.
++ `overload` is a decorator that allows C-like overloading of functions.
++ `flatten` is a fast list flattener.
```

### Comparing `tharos-pytools-0.0.8/tharospytools/matplotlib_tools.py` & `tharos-pytools-0.0.9/tharospytools/matplotlib_tools.py`

 * *Files identical despite different names*

### Comparing `tharos-pytools-0.0.8/tharospytools/multithreading.py` & `tharos-pytools-0.0.9/tharospytools/multithreading.py`

 * *Files identical despite different names*

### Comparing `tharos-pytools-0.0.8/tharospytools/overloading.py` & `tharos-pytools-0.0.9/tharospytools/overloading.py`

 * *Files identical despite different names*

