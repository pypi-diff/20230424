# Comparing `tmp/loop_step-2023.2.15.tar.gz` & `tmp/loop_step-2023.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loop_step-2023.2.15.tar", last modified: Wed Feb 15 01:33:31 2023, max compression
+gzip compressed data, was "loop_step-2023.4.24.tar", last modified: Mon Apr 24 19:51:14 2023, max compression
```

## Comparing `loop_step-2023.2.15.tar` & `loop_step-2023.4.24.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.907461 loop_step-2023.2.15/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-15 01:33:19.000000 loop_step-2023.2.15/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-15 01:33:19.000000 loop_step-2023.2.15/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-15 01:33:19.000000 loop_step-2023.2.15/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-15 01:33:19.000000 loop_step-2023.2.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-15 01:33:19.000000 loop_step-2023.2.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-02-15 01:33:31.907461 loop_step-2023.2.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-15 01:33:19.000000 loop_step-2023.2.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.903460 loop_step-2023.2.15/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.903460 loop_step-2023.2.15/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.903460 loop_step-2023.2.15/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9510 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.903460 loop_step-2023.2.15/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/developer_guide/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.903460 loop_step-2023.2.15/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.903460 loop_step-2023.2.15/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-15 01:33:19.000000 loop_step-2023.2.15/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.907461 loop_step-2023.2.15/loop_step/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-15 01:33:19.000000 loop_step-2023.2.15/loop_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-15 01:33:31.907461 loop_step-2023.2.15/loop_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    31300 2023-02-15 01:33:19.000000 loop_step-2023.2.15/loop_step/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-02-15 01:33:19.000000 loop_step-2023.2.15/loop_step/loop_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-15 01:33:19.000000 loop_step-2023.2.15/loop_step/loop_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-02-15 01:33:19.000000 loop_step-2023.2.15/loop_step/tk_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.907461 loop_step-2023.2.15/loop_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-02-15 01:33:31.000000 loop_step-2023.2.15/loop_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-15 01:33:31.000000 loop_step-2023.2.15/loop_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 01:33:31.000000 loop_step-2023.2.15/loop_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-15 01:33:31.000000 loop_step-2023.2.15/loop_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 01:33:20.000000 loop_step-2023.2.15/loop_step.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-15 01:33:31.000000 loop_step-2023.2.15/loop_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-15 01:33:31.000000 loop_step-2023.2.15/loop_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-15 01:33:31.907461 loop_step-2023.2.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-15 01:33:19.000000 loop_step-2023.2.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 01:33:31.907461 loop_step-2023.2.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-15 01:33:19.000000 loop_step-2023.2.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-15 01:33:19.000000 loop_step-2023.2.15/tests/test_loop_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.632547 loop_step-2023.4.24/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 19:51:01.000000 loop_step-2023.4.24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 19:51:01.000000 loop_step-2023.4.24/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-24 19:51:01.000000 loop_step-2023.4.24/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-24 19:51:01.000000 loop_step-2023.4.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-24 19:51:01.000000 loop_step-2023.4.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-24 19:51:14.632547 loop_step-2023.4.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 19:51:01.000000 loop_step-2023.4.24/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9510 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/developer_guide/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 19:51:01.000000 loop_step-2023.4.24/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.632547 loop_step-2023.4.24/loop_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-24 19:51:01.000000 loop_step-2023.4.24/loop_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 19:51:14.632547 loop_step-2023.4.24/loop_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31373 2023-04-24 19:51:01.000000 loop_step-2023.4.24/loop_step/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-24 19:51:01.000000 loop_step-2023.4.24/loop_step/loop_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-24 19:51:01.000000 loop_step-2023.4.24/loop_step/loop_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-04-24 19:51:01.000000 loop_step-2023.4.24/loop_step/tk_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.628547 loop_step-2023.4.24/loop_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-24 19:51:14.000000 loop_step-2023.4.24/loop_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-24 19:51:14.000000 loop_step-2023.4.24/loop_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:51:14.000000 loop_step-2023.4.24/loop_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 19:51:14.000000 loop_step-2023.4.24/loop_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:51:05.000000 loop_step-2023.4.24/loop_step.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 19:51:14.000000 loop_step-2023.4.24/loop_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 19:51:14.000000 loop_step-2023.4.24/loop_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 19:51:14.632547 loop_step-2023.4.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-24 19:51:01.000000 loop_step-2023.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:51:14.632547 loop_step-2023.4.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 19:51:01.000000 loop_step-2023.4.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 19:51:01.000000 loop_step-2023.4.24/tests/test_loop_step.py
```

### Comparing `loop_step-2023.2.15/CONTRIBUTING.rst` & `loop_step-2023.4.24/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/HISTORY.rst` & `loop_step-2023.4.24/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =======
 History
 =======
 
+2023.4.24 -- Better support for rerunning/restarting jobs
+    * Remove 'iteration.out' if it already exists.
+      
 2023.2.15 -- Starting to add loops over structures in the database
 
 * Reorganized the documentation and changed to the standard MolSSI theme.
 
 2022.1.16 -- Improved error handling
 
 * Wrote the traceback for any errors caught to item_nnn/stderr.out to aid debugging.
```

### Comparing `loop_step-2023.2.15/LICENSE` & `loop_step-2023.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/PKG-INFO` & `loop_step-2023.4.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loop_step
-Version: 2023.2.15
+Version: 2023.4.24
 Summary: A SEAMM plug-in which provides loops in flowcharts.
 Home-page: https://github.com/molssi-seamm/loop_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,control,loops
 Platform: Linux
@@ -86,14 +86,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.4.24 -- Better support for rerunning/restarting jobs
+    * Remove 'iteration.out' if it already exists.
+      
 2023.2.15 -- Starting to add loops over structures in the database
 
 * Reorganized the documentation and changed to the standard MolSSI theme.
 
 2022.1.16 -- Improved error handling
 
 * Wrote the traceback for any errors caught to item_nnn/stderr.out to aid debugging.
```

### Comparing `loop_step-2023.2.15/README.rst` & `loop_step-2023.4.24/README.rst`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/Makefile` & `loop_step-2023.4.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/_static/SEAMM inverted.png` & `loop_step-2023.4.24/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/_static/SEAMM logo.png` & `loop_step-2023.4.24/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/_static/molssi_main_logo.png` & `loop_step-2023.4.24/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/_static/molssi_main_logo_inverted_white.png` & `loop_step-2023.4.24/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/_static/molssi_square.png` & `loop_step-2023.4.24/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/_static/nsf.png` & `loop_step-2023.4.24/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/conf.py` & `loop_step-2023.4.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/developer_guide/installation.rst` & `loop_step-2023.4.24/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/getting_started/index.rst` & `loop_step-2023.4.24/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/index.rst` & `loop_step-2023.4.24/docs/index.rst`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/docs/make.bat` & `loop_step-2023.4.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/loop_step/__init__.py` & `loop_step-2023.4.24/loop_step/__init__.py`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/loop_step/loop.py` & `loop_step-2023.4.24/loop_step/loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,17 @@
                 # A handler for the file
                 iter_dir = self.working_path
                 iter_dir.mkdir(parents=True, exist_ok=True)
 
                 if self._file_handler is not None:
                     self._file_handler.close()
                     job.removeHandler(self._file_handler)
-                self._file_handler = logging.FileHandler(iter_dir / "iteration.out")
+                path = iter_dir / "iteration.out"
+                path.unlink(missing_ok=True)
+                self._file_handler = logging.FileHandler(path)
                 self._file_handler.setLevel(printing.NORMAL)
                 formatter = logging.Formatter(fmt="{message:s}", style="{")
                 self._file_handler.setFormatter(formatter)
                 job.addHandler(self._file_handler)
 
                 # Add the iteration to the ids so the directory structure is
                 # reasonable
```

### Comparing `loop_step-2023.2.15/loop_step/loop_parameters.py` & `loop_step-2023.4.24/loop_step/loop_parameters.py`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/loop_step/loop_step.py` & `loop_step-2023.4.24/loop_step/loop_step.py`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/loop_step/tk_loop.py` & `loop_step-2023.4.24/loop_step/tk_loop.py`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/loop_step.egg-info/PKG-INFO` & `loop_step-2023.4.24/loop_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loop-step
-Version: 2023.2.15
+Version: 2023.4.24
 Summary: A SEAMM plug-in which provides loops in flowcharts.
 Home-page: https://github.com/molssi-seamm/loop_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,control,loops
 Platform: Linux
@@ -86,14 +86,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.4.24 -- Better support for rerunning/restarting jobs
+    * Remove 'iteration.out' if it already exists.
+      
 2023.2.15 -- Starting to add loops over structures in the database
 
 * Reorganized the documentation and changed to the standard MolSSI theme.
 
 2022.1.16 -- Improved error handling
 
 * Wrote the traceback for any errors caught to item_nnn/stderr.out to aid debugging.
```

### Comparing `loop_step-2023.2.15/loop_step.egg-info/SOURCES.txt` & `loop_step-2023.4.24/loop_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/setup.py` & `loop_step-2023.4.24/setup.py`

 * *Files identical despite different names*

### Comparing `loop_step-2023.2.15/tests/test_loop_step.py` & `loop_step-2023.4.24/tests/test_loop_step.py`

 * *Files identical despite different names*

