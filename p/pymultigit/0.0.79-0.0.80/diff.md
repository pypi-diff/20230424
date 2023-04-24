# Comparing `tmp/pymultigit-0.0.79.tar.gz` & `tmp/pymultigit-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultigit-0.0.79.tar", last modified: Mon Apr 24 06:05:55 2023, max compression
+gzip compressed data, was "pymultigit-0.0.80.tar", last modified: Mon Apr 24 06:07:07 2023, max compression
```

## Comparing `pymultigit-0.0.79.tar` & `pymultigit-0.0.80.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:05:55.768068 pymultigit-0.0.79/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-24 06:05:31.000000 pymultigit-0.0.79/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1399 2023-04-24 06:05:55.768068 pymultigit-0.0.79/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-04-24 06:05:31.000000 pymultigit-0.0.79/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:05:55.768068 pymultigit-0.0.79/pymultigit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:38:18.000000 pymultigit-0.0.79/pymultigit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2661 2023-04-24 06:04:18.000000 pymultigit-0.0.79/pymultigit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     8687 2023-04-24 06:04:46.000000 pymultigit-0.0.79/pymultigit/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5084 2022-10-17 03:51:11.000000 pymultigit-0.0.79/pymultigit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      196 2023-04-24 06:05:31.000000 pymultigit-0.0.79/pymultigit/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:05:55.768068 pymultigit-0.0.79/pymultigit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1399 2023-04-24 06:05:55.000000 pymultigit-0.0.79/pymultigit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      347 2023-04-24 06:05:55.000000 pymultigit-0.0.79/pymultigit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-24 06:05:55.000000 pymultigit-0.0.79/pymultigit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-24 06:05:55.000000 pymultigit-0.0.79/pymultigit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-04-24 06:05:55.000000 pymultigit-0.0.79/pymultigit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-24 06:05:55.000000 pymultigit-0.0.79/pymultigit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-24 06:05:55.769068 pymultigit-0.0.79/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1612 2023-04-24 06:05:31.000000 pymultigit-0.0.79/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:07:07.707380 pymultigit-0.0.80/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-24 06:06:56.000000 pymultigit-0.0.80/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1399 2023-04-24 06:07:07.707380 pymultigit-0.0.80/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-04-24 06:06:56.000000 pymultigit-0.0.80/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:07:07.706380 pymultigit-0.0.80/pymultigit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:38:18.000000 pymultigit-0.0.80/pymultigit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2661 2023-04-24 06:04:18.000000 pymultigit-0.0.80/pymultigit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     8687 2023-04-24 06:04:46.000000 pymultigit-0.0.80/pymultigit/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5084 2022-10-17 03:51:11.000000 pymultigit-0.0.80/pymultigit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      196 2023-04-24 06:06:56.000000 pymultigit-0.0.80/pymultigit/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:07:07.707380 pymultigit-0.0.80/pymultigit/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-04-24 06:06:42.000000 pymultigit-0.0.80/pymultigit/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      797 2023-04-24 06:05:04.000000 pymultigit-0.0.80/pymultigit/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-24 06:07:07.707380 pymultigit-0.0.80/pymultigit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1399 2023-04-24 06:07:07.000000 pymultigit-0.0.80/pymultigit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      407 2023-04-24 06:07:07.000000 pymultigit-0.0.80/pymultigit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-24 06:07:07.000000 pymultigit-0.0.80/pymultigit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-24 06:07:07.000000 pymultigit-0.0.80/pymultigit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-04-24 06:07:07.000000 pymultigit-0.0.80/pymultigit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-24 06:07:07.000000 pymultigit-0.0.80/pymultigit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-24 06:07:07.707380 pymultigit-0.0.80/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1640 2023-04-24 06:06:56.000000 pymultigit-0.0.80/setup.py
```

### Comparing `pymultigit-0.0.79/LICENSE` & `pymultigit-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.79/PKG-INFO` & `pymultigit-0.0.80/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.79
+Version: 0.0.80
 Summary: Help you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
 Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.79
+version: 0.0.80
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.79/pymultigit/configs.py` & `pymultigit-0.0.80/pymultigit/configs.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.79/pymultigit/core.py` & `pymultigit-0.0.80/pymultigit/core.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.79/pymultigit/main.py` & `pymultigit-0.0.80/pymultigit/main.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.79/pymultigit.egg-info/PKG-INFO` & `pymultigit-0.0.80/pymultigit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.79
+Version: 0.0.80
 Summary: Help you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
 Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.79
+version: 0.0.80
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.79/setup.py` & `pymultigit-0.0.80/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pymultigit",
-    version="0.0.79",
+    version="0.0.80",
     packages=[
         "pymultigit",
+        "pymultigit.utils",
     ],
     # from here all is optional
     description="Help you deal with multiple git repositories",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
```

