# Comparing `tmp/pyecotrend-ista-2.0.0.tar.gz` & `tmp/pyecotrend-ista-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecotrend-ista-2.0.0.tar", last modified: Mon Apr 24 08:31:11 2023, max compression
+gzip compressed data, was "pyecotrend-ista-2.0.1.tar", last modified: Mon Apr 24 08:52:26 2023, max compression
```

## Comparing `pyecotrend-ista-2.0.0.tar` & `pyecotrend-ista-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.481258 pyecotrend-ista-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/src/pyecotrend_ista/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/helper_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/ista_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-04-24 08:30:57.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista/pyecotrend_ista.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:31:11.485258 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 08:31:11.000000 pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:52:26.480858 pyecotrend-ista-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 08:52:26.480858 pyecotrend-ista-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:52:26.480858 pyecotrend-ista-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:52:26.480858 pyecotrend-ista-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:52:26.480858 pyecotrend-ista-2.0.1/src/pyecotrend_ista/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista/helper_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista/ista_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-04-24 08:52:13.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista/pyecotrend_ista.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:52:26.480858 pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 08:52:26.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 08:52:26.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:52:26.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 08:52:26.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 08:52:26.000000 pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/top_level.txt
```

### Comparing `pyecotrend-ista-2.0.0/LICENSE` & `pyecotrend-ista-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.0/PKG-INFO` & `pyecotrend-ista-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

### Comparing `pyecotrend-ista-2.0.0/README.md` & `pyecotrend-ista-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.0/setup.py` & `pyecotrend-ista-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.0/src/pyecotrend_ista/helper_object.py` & `pyecotrend-ista-2.0.1/src/pyecotrend_ista/helper_object.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.0/src/pyecotrend_ista/ista_object.py` & `pyecotrend-ista-2.0.1/src/pyecotrend_ista/ista_object.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.0/src/pyecotrend_ista/pyecotrend_ista.py` & `pyecotrend-ista-2.0.1/src/pyecotrend_ista/pyecotrend_ista.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.0/src/pyecotrend_ista.egg-info/PKG-INFO` & `pyecotrend-ista-2.0.1/src/pyecotrend_ista.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

