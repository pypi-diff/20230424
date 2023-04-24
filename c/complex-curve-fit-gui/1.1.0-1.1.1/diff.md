# Comparing `tmp/complex_curve_fit_gui-1.1.0.tar.gz` & `tmp/complex_curve_fit_gui-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_curve_fit_gui-1.1.0.tar", last modified: Mon Apr 24 03:40:28 2023, max compression
+gzip compressed data, was "complex_curve_fit_gui-1.1.1.tar", last modified: Mon Apr 24 03:52:42 2023, max compression
```

## Comparing `complex_curve_fit_gui-1.1.0.tar` & `complex_curve_fit_gui-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.592375 complex_curve_fit_gui-1.1.0/
--rw-r--r--   0 kojo       (501) staff       (20)     8196 2023-04-24 03:28:58.000000 complex_curve_fit_gui-1.1.0/.DS_Store
--rw-r--r--   0 kojo       (501) staff       (20)       31 2023-01-24 05:50:18.000000 complex_curve_fit_gui-1.1.0/.gitignore
--rw-rw-rw-   0 kojo       (501) staff       (20)       30 2021-07-05 10:22:07.000000 complex_curve_fit_gui-1.1.0/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:40:28.592548 complex_curve_fit_gui-1.1.0/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     8826 2023-04-14 18:42:27.000000 complex_curve_fit_gui-1.1.0/README.md
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.570248 complex_curve_fit_gui-1.1.0/__pycache__/
--rw-r--r--   0 kojo       (501) staff       (20)     1275 2023-01-31 04:10:58.000000 complex_curve_fit_gui-1.1.0/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    12574 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.0/__pycache__/tools.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      159 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.0/__pycache__/version.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    14087 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.0/__pycache__/widgets.cpython-39.pyc
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.570909 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     1298 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)     1001 2023-04-24 03:20:08.000000 complex_curve_fit_gui-1.1.0/curve.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.573342 complex_curve_fit_gui-1.1.0/curvefitgui/
--rw-r--r--   0 kojo       (501) staff       (20)     6148 2023-03-24 01:24:37.000000 complex_curve_fit_gui-1.1.0/curvefitgui/.DS_Store
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__init__.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.577060 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/
--rw-r--r--   0 kojo       (501) staff       (20)      424 2023-02-10 20:02:50.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      341 2023-01-31 03:15:43.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     7837 2023-02-23 16:53:13.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     6506 2023-03-31 04:21:23.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    18255 2023-03-02 19:00:48.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    11089 2023-04-22 02:23:13.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     2547 2023-02-10 20:02:50.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     1280 2023-01-31 03:15:43.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    14114 2023-04-24 03:20:12.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_tools.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      171 2023-03-31 04:42:55.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_version.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    23105 2023-04-22 02:23:13.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_widgets.cpython-39.pyc
--rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-03-31 04:21:21.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    15523 2023-04-22 02:23:11.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16582 2023-04-22 02:34:16.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-24 03:39:28.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    30979 2023-04-22 02:21:36.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.0/curvefitgui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.590844 complex_curve_fit_gui-1.1.0/images/
--rw-r--r--   0 kojo       (501) staff       (20)   588681 2023-03-24 01:20:24.000000 complex_curve_fit_gui-1.1.0/images/arrows_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585322 2023-03-24 01:17:35.000000 complex_curve_fit_gui-1.1.0/images/customize_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585544 2023-03-24 01:22:29.000000 complex_curve_fit_gui-1.1.0/images/home_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   589105 2023-03-24 01:13:01.000000 complex_curve_fit_gui-1.1.0/images/model_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)  1934108 2023-03-24 01:21:22.000000 complex_curve_fit_gui-1.1.0/images/pan_zoom_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585291 2023-03-24 01:16:21.000000 complex_curve_fit_gui-1.1.0/images/range_selector_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585414 2023-03-24 01:14:53.000000 complex_curve_fit_gui-1.1.0/images/toolbar_scr.png
--rw-rw-rw-   0 kojo       (501) staff       (20)       38 2023-04-24 03:40:28.593015 complex_curve_fit_gui-1.1.0/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1226 2023-04-24 03:39:11.000000 complex_curve_fit_gui-1.1.0/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:52:42.451043 complex_curve_fit_gui-1.1.1/
+-rw-r--r--   0 kojo       (501) staff       (20)     8196 2023-04-24 03:28:58.000000 complex_curve_fit_gui-1.1.1/.DS_Store
+-rw-r--r--   0 kojo       (501) staff       (20)       31 2023-01-24 05:50:18.000000 complex_curve_fit_gui-1.1.1/.gitignore
+-rw-rw-rw-   0 kojo       (501) staff       (20)       30 2021-07-05 10:22:07.000000 complex_curve_fit_gui-1.1.1/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:52:42.451223 complex_curve_fit_gui-1.1.1/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     8826 2023-04-14 18:42:27.000000 complex_curve_fit_gui-1.1.1/README.md
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:52:42.428357 complex_curve_fit_gui-1.1.1/__pycache__/
+-rw-r--r--   0 kojo       (501) staff       (20)     1275 2023-01-31 04:10:58.000000 complex_curve_fit_gui-1.1.1/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    12574 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.1/__pycache__/tools.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      159 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.1/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    14087 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.1/__pycache__/widgets.cpython-39.pyc
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:52:42.428948 complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:52:42.000000 complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     1298 2023-04-24 03:52:42.000000 complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:52:42.000000 complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)       12 2023-04-24 03:52:42.000000 complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)     1001 2023-04-24 03:20:08.000000 complex_curve_fit_gui-1.1.1/curve.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:52:42.431732 complex_curve_fit_gui-1.1.1/curvefitgui/
+-rw-r--r--   0 kojo       (501) staff       (20)     6148 2023-03-24 01:24:37.000000 complex_curve_fit_gui-1.1.1/curvefitgui/.DS_Store
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__init__.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:52:42.435553 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/
+-rw-r--r--   0 kojo       (501) staff       (20)      424 2023-02-10 20:02:50.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      341 2023-01-31 03:15:43.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     7837 2023-02-23 16:53:13.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     6506 2023-03-31 04:21:23.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    18255 2023-03-02 19:00:48.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_gui.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    11089 2023-04-22 02:23:13.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_gui.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     2547 2023-02-10 20:02:50.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_settings.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     1280 2023-01-31 03:15:43.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_settings.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    14114 2023-04-24 03:20:12.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_tools.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      171 2023-03-31 04:42:55.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_version.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    23105 2023-04-22 02:23:13.000000 complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_widgets.cpython-39.pyc
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-03-31 04:21:21.000000 complex_curve_fit_gui-1.1.1/curvefitgui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15523 2023-04-22 02:23:11.000000 complex_curve_fit_gui-1.1.1/curvefitgui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.1/curvefitgui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16582 2023-04-22 02:34:16.000000 complex_curve_fit_gui-1.1.1/curvefitgui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-24 03:52:36.000000 complex_curve_fit_gui-1.1.1/curvefitgui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    30979 2023-04-22 02:21:36.000000 complex_curve_fit_gui-1.1.1/curvefitgui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.1/curvefitgui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:52:42.449465 complex_curve_fit_gui-1.1.1/images/
+-rw-r--r--   0 kojo       (501) staff       (20)   588681 2023-03-24 01:20:24.000000 complex_curve_fit_gui-1.1.1/images/arrows_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585322 2023-03-24 01:17:35.000000 complex_curve_fit_gui-1.1.1/images/customize_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585544 2023-03-24 01:22:29.000000 complex_curve_fit_gui-1.1.1/images/home_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   589105 2023-03-24 01:13:01.000000 complex_curve_fit_gui-1.1.1/images/model_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)  1934108 2023-03-24 01:21:22.000000 complex_curve_fit_gui-1.1.1/images/pan_zoom_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585291 2023-03-24 01:16:21.000000 complex_curve_fit_gui-1.1.1/images/range_selector_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585414 2023-03-24 01:14:53.000000 complex_curve_fit_gui-1.1.1/images/toolbar_scr.png
+-rw-rw-rw-   0 kojo       (501) staff       (20)       38 2023-04-24 03:52:42.454241 complex_curve_fit_gui-1.1.1/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1213 2023-04-24 03:49:40.000000 complex_curve_fit_gui-1.1.1/setup.py
```

### Comparing `complex_curve_fit_gui-1.1.0/.DS_Store` & `complex_curve_fit_gui-1.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/PKG-INFO` & `complex_curve_fit_gui-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex_curve_fit_gui
-Version: 1.1.0
+Version: 1.1.1
 Summary: GUI for lmfit
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `complex_curve_fit_gui-1.1.0/README.md` & `complex_curve_fit_gui-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/__pycache__/settings.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/__pycache__/tools.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/__pycache__/tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/__pycache__/widgets.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/__pycache__/widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.1.0
+Version: 1.1.1
 Summary: GUI for lmfit
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex_curve_fit_gui-1.1.1/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curve.py` & `complex_curve_fit_gui-1.1.1/curve.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/.DS_Store` & `complex_curve_fit_gui-1.1.1/curvefitgui/.DS_Store`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-311.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_gui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-311.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_tools.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_widgets.cpython-39.pyc` & `complex_curve_fit_gui-1.1.1/curvefitgui/__pycache__/_widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/_curvefitgui.py` & `complex_curve_fit_gui-1.1.1/curvefitgui/_curvefitgui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/_gui.py` & `complex_curve_fit_gui-1.1.1/curvefitgui/_gui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/_settings.py` & `complex_curve_fit_gui-1.1.1/curvefitgui/_settings.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/_tools.py` & `complex_curve_fit_gui-1.1.1/curvefitgui/_tools.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/_widgets.py` & `complex_curve_fit_gui-1.1.1/curvefitgui/_widgets.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/curvefitgui/config.txt` & `complex_curve_fit_gui-1.1.1/curvefitgui/config.txt`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/arrows_scr.png` & `complex_curve_fit_gui-1.1.1/images/arrows_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/customize_scr.png` & `complex_curve_fit_gui-1.1.1/images/customize_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/home_scr.png` & `complex_curve_fit_gui-1.1.1/images/home_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/model_scr.png` & `complex_curve_fit_gui-1.1.1/images/model_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/pan_zoom_scr.png` & `complex_curve_fit_gui-1.1.1/images/pan_zoom_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/range_selector_scr.png` & `complex_curve_fit_gui-1.1.1/images/range_selector_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/images/toolbar_scr.png` & `complex_curve_fit_gui-1.1.1/images/toolbar_scr.png`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.0/setup.py` & `complex_curve_fit_gui-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7, <4",
-    packages=find_packages("curvefitgui"),
+    packages=find_packages(),
     include_package_data=True,
     package_data={
         "curvefitgui": ["config.txt"],
     },
     # conda
     # install_requires=["matplotlib", "numpy", "scipy", "pyqt", "qtpy"], # need to check versions
     # PyPi
```

