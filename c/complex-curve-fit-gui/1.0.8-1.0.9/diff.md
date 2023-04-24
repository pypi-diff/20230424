# Comparing `tmp/complex-curve-fit-gui-1.0.8.tar.gz` & `tmp/complex-curve-fit-gui-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex-curve-fit-gui-1.0.8.tar", last modified: Fri Mar 31 04:39:50 2023, max compression
+gzip compressed data, was "complex-curve-fit-gui-1.0.9.tar", last modified: Mon Apr 24 03:28:06 2023, max compression
```

## Comparing `complex-curve-fit-gui-1.0.8.tar` & `complex-curve-fit-gui-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,49 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.247597 complex-curve-fit-gui-1.0.8/
--rw-r--r--   0 kojo       (501) staff       (20)     8196 2023-03-24 01:24:42.000000 complex-curve-fit-gui-1.0.8/.DS_Store
--rw-r--r--   0 kojo       (501) staff       (20)       31 2023-01-24 05:50:18.000000 complex-curve-fit-gui-1.0.8/.gitignore
--rw-rw-rw-   0 kojo       (501) staff       (20)       30 2021-07-05 10:22:07.000000 complex-curve-fit-gui-1.0.8/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)     8827 2023-03-31 04:39:50.247752 complex-curve-fit-gui-1.0.8/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     8385 2023-03-27 19:21:02.000000 complex-curve-fit-gui-1.0.8/README.md
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.224950 complex-curve-fit-gui-1.0.8/__pycache__/
--rw-r--r--   0 kojo       (501) staff       (20)     1275 2023-01-31 04:10:58.000000 complex-curve-fit-gui-1.0.8/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    12574 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.8/__pycache__/tools.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      159 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.8/__pycache__/version.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    14087 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.8/__pycache__/widgets.cpython-39.pyc
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.225598 complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)     8827 2023-03-31 04:39:50.000000 complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     1438 2023-03-31 04:39:50.000000 complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-03-31 04:39:50.000000 complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-03-31 04:39:50.000000 complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)      927 2023-03-31 04:38:31.000000 complex-curve-fit-gui-1.0.8/curve.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.227522 complex-curve-fit-gui-1.0.8/curvefitgui/
--rw-r--r--   0 kojo       (501) staff       (20)     6148 2023-03-24 01:24:37.000000 complex-curve-fit-gui-1.0.8/curvefitgui/.DS_Store
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__init__.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.231000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/
--rw-r--r--   0 kojo       (501) staff       (20)      424 2023-02-10 20:02:50.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      341 2023-01-31 03:15:43.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     7837 2023-02-23 16:53:13.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     6506 2023-03-31 04:21:23.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    18255 2023-03-02 19:00:48.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_gui.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     9930 2023-03-31 04:32:41.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_gui.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     2547 2023-02-10 20:02:50.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_settings.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     1280 2023-01-31 03:15:43.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_settings.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    13924 2023-02-24 17:27:58.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_tools.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      171 2023-03-31 03:43:38.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_version.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    17570 2023-03-31 04:04:08.000000 complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_widgets.cpython-39.pyc
--rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-03-31 04:21:21.000000 complex-curve-fit-gui-1.0.8/curvefitgui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    13547 2023-03-31 04:32:39.000000 complex-curve-fit-gui-1.0.8/curvefitgui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.8/curvefitgui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16626 2023-02-24 17:24:25.000000 complex-curve-fit-gui-1.0.8/curvefitgui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-03-31 04:39:38.000000 complex-curve-fit-gui-1.0.8/curvefitgui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    23281 2023-03-31 04:03:40.000000 complex-curve-fit-gui-1.0.8/curvefitgui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.8/curvefitgui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.228428 complex-curve-fit-gui-1.0.8/curvefitgui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)     4611 2023-03-02 19:18:36.000000 complex-curve-fit-gui-1.0.8/curvefitgui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     1061 2023-03-02 19:18:36.000000 complex-curve-fit-gui-1.0.8/curvefitgui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-03-02 19:18:36.000000 complex-curve-fit-gui-1.0.8/curvefitgui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-03-02 19:18:36.000000 complex-curve-fit-gui-1.0.8/curvefitgui.egg-info/top_level.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-03-31 04:39:50.243013 complex-curve-fit-gui-1.0.8/images/
--rw-r--r--   0 kojo       (501) staff       (20)   588681 2023-03-24 01:20:24.000000 complex-curve-fit-gui-1.0.8/images/arrows_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585322 2023-03-24 01:17:35.000000 complex-curve-fit-gui-1.0.8/images/customize_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585544 2023-03-24 01:22:29.000000 complex-curve-fit-gui-1.0.8/images/home_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   589105 2023-03-24 01:13:01.000000 complex-curve-fit-gui-1.0.8/images/model_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)  1934108 2023-03-24 01:21:22.000000 complex-curve-fit-gui-1.0.8/images/pan_zoom_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585291 2023-03-24 01:16:21.000000 complex-curve-fit-gui-1.0.8/images/range_selector_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585414 2023-03-24 01:14:53.000000 complex-curve-fit-gui-1.0.8/images/toolbar_scr.png
--rw-rw-rw-   0 kojo       (501) staff       (20)       38 2023-03-31 04:39:50.248196 complex-curve-fit-gui-1.0.8/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1226 2023-03-02 19:50:20.000000 complex-curve-fit-gui-1.0.8/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.484715 complex-curve-fit-gui-1.0.9/
+-rw-r--r--   0 kojo       (501) staff       (20)     8196 2023-03-24 01:24:42.000000 complex-curve-fit-gui-1.0.9/.DS_Store
+-rw-r--r--   0 kojo       (501) staff       (20)       31 2023-01-24 05:50:18.000000 complex-curve-fit-gui-1.0.9/.gitignore
+-rw-rw-rw-   0 kojo       (501) staff       (20)       30 2021-07-05 10:22:07.000000 complex-curve-fit-gui-1.0.9/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:28:06.484874 complex-curve-fit-gui-1.0.9/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     8826 2023-04-14 18:42:27.000000 complex-curve-fit-gui-1.0.9/README.md
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.465648 complex-curve-fit-gui-1.0.9/__pycache__/
+-rw-r--r--   0 kojo       (501) staff       (20)     1275 2023-01-31 04:10:58.000000 complex-curve-fit-gui-1.0.9/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    12574 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.9/__pycache__/tools.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      159 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.9/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    14087 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.9/__pycache__/widgets.cpython-39.pyc
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.466196 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     1298 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)       12 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)     1001 2023-04-24 03:20:08.000000 complex-curve-fit-gui-1.0.9/curve.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.468369 complex-curve-fit-gui-1.0.9/curvefitgui/
+-rw-r--r--   0 kojo       (501) staff       (20)     6148 2023-03-24 01:24:37.000000 complex-curve-fit-gui-1.0.9/curvefitgui/.DS_Store
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__init__.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.470770 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/
+-rw-r--r--   0 kojo       (501) staff       (20)      424 2023-02-10 20:02:50.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      341 2023-01-31 03:15:43.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     7837 2023-02-23 16:53:13.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     6506 2023-03-31 04:21:23.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    18255 2023-03-02 19:00:48.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    11089 2023-04-22 02:23:13.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     2547 2023-02-10 20:02:50.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     1280 2023-01-31 03:15:43.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    14114 2023-04-24 03:20:12.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_tools.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      171 2023-03-31 04:42:55.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_version.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    23105 2023-04-22 02:23:13.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_widgets.cpython-39.pyc
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-03-31 04:21:21.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15523 2023-04-22 02:23:11.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16582 2023-04-22 02:34:16.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-24 03:27:55.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    30979 2023-04-22 02:21:36.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.9/curvefitgui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.483167 complex-curve-fit-gui-1.0.9/images/
+-rw-r--r--   0 kojo       (501) staff       (20)   588681 2023-03-24 01:20:24.000000 complex-curve-fit-gui-1.0.9/images/arrows_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585322 2023-03-24 01:17:35.000000 complex-curve-fit-gui-1.0.9/images/customize_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585544 2023-03-24 01:22:29.000000 complex-curve-fit-gui-1.0.9/images/home_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   589105 2023-03-24 01:13:01.000000 complex-curve-fit-gui-1.0.9/images/model_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)  1934108 2023-03-24 01:21:22.000000 complex-curve-fit-gui-1.0.9/images/pan_zoom_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585291 2023-03-24 01:16:21.000000 complex-curve-fit-gui-1.0.9/images/range_selector_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585414 2023-03-24 01:14:53.000000 complex-curve-fit-gui-1.0.9/images/toolbar_scr.png
+-rw-rw-rw-   0 kojo       (501) staff       (20)       38 2023-04-24 03:28:06.485283 complex-curve-fit-gui-1.0.9/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1213 2023-04-24 03:20:55.000000 complex-curve-fit-gui-1.0.9/setup.py
```

### Comparing `complex-curve-fit-gui-1.0.8/.DS_Store` & `complex-curve-fit-gui-1.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/PKG-INFO` & `complex-curve-fit-gui-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.0.8
+Version: 1.0.9
 Summary: GUI for lmfit
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,20 @@
     - Set first parameter to None to be able to select predefined functions
     - For example: 
 
        `curve_fit_gui(None,xdata,ydata)`
 5. Optionally disable gui and immediately get fit results as tuple (popt, pcov, result) where popt is an array of the best-fit parameters, pcov is an array of the confidence intervals, and result is an lmfit ModelResult object. [Model Result](https://lmfit.github.io/lmfit-py/model.html#lmfit.model.ModelResult)
        `curve_fit_gui(function,xdata,ydata, showgui=False)`
 
+### Open Multiple Windows
+ - Appending `&` to the end of the command used to run program will give access to current terminal, allowing for another window to be openned. Ex: `python3 curve.py&`
+
+### Plot multiple dataset on single window
+ - Use the keyword argument `add` and format argument as an array of tuples i.e `[(np.array, np.array, string)]` where the first index is xdata, the next in y-data, and the last is a label for the data
+
 
 ### curve_fit_gui function:
 This starts up the GUI. The call signature is `curve_fit_gui(f,xdata,ydata,xerr=None -> [optional],yerr=None -> [optional],p0=None  -> [optional],xlabel="x-axis" -> [optional],ylabel="y-axis" -> [optional],absolute_sigma=False -> [optional],jac=None -> [optional],showgui=True -> [optional],**kwargs, -> [optional])`
  - f : callable
         the fit function which if set to None, gives option of selection predefined fit functions
  -  xdata : 1-D numpy array
         x-coordinates of the data
```

### Comparing `complex-curve-fit-gui-1.0.8/README.md` & `complex-curve-fit-gui-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     - Set first parameter to None to be able to select predefined functions
     - For example: 
 
        `curve_fit_gui(None,xdata,ydata)`
 5. Optionally disable gui and immediately get fit results as tuple (popt, pcov, result) where popt is an array of the best-fit parameters, pcov is an array of the confidence intervals, and result is an lmfit ModelResult object. [Model Result](https://lmfit.github.io/lmfit-py/model.html#lmfit.model.ModelResult)
        `curve_fit_gui(function,xdata,ydata, showgui=False)`
 
+### Open Multiple Windows
+ - Appending `&` to the end of the command used to run program will give access to current terminal, allowing for another window to be openned. Ex: `python3 curve.py&`
+
+### Plot multiple dataset on single window
+ - Use the keyword argument `add` and format argument as an array of tuples i.e `[(np.array, np.array, string)]` where the first index is xdata, the next in y-data, and the last is a label for the data
+
 
 ### curve_fit_gui function:
 This starts up the GUI. The call signature is `curve_fit_gui(f,xdata,ydata,xerr=None -> [optional],yerr=None -> [optional],p0=None  -> [optional],xlabel="x-axis" -> [optional],ylabel="y-axis" -> [optional],absolute_sigma=False -> [optional],jac=None -> [optional],showgui=True -> [optional],**kwargs, -> [optional])`
  - f : callable
         the fit function which if set to None, gives option of selection predefined fit functions
  -  xdata : 1-D numpy array
         x-coordinates of the data
```

### Comparing `complex-curve-fit-gui-1.0.8/__pycache__/settings.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/__pycache__/tools.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/__pycache__/tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/__pycache__/widgets.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/__pycache__/widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.0.8
+Version: 1.0.9
 Summary: GUI for lmfit
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,20 @@
     - Set first parameter to None to be able to select predefined functions
     - For example: 
 
        `curve_fit_gui(None,xdata,ydata)`
 5. Optionally disable gui and immediately get fit results as tuple (popt, pcov, result) where popt is an array of the best-fit parameters, pcov is an array of the confidence intervals, and result is an lmfit ModelResult object. [Model Result](https://lmfit.github.io/lmfit-py/model.html#lmfit.model.ModelResult)
        `curve_fit_gui(function,xdata,ydata, showgui=False)`
 
+### Open Multiple Windows
+ - Appending `&` to the end of the command used to run program will give access to current terminal, allowing for another window to be openned. Ex: `python3 curve.py&`
+
+### Plot multiple dataset on single window
+ - Use the keyword argument `add` and format argument as an array of tuples i.e `[(np.array, np.array, string)]` where the first index is xdata, the next in y-data, and the last is a label for the data
+
 
 ### curve_fit_gui function:
 This starts up the GUI. The call signature is `curve_fit_gui(f,xdata,ydata,xerr=None -> [optional],yerr=None -> [optional],p0=None  -> [optional],xlabel="x-axis" -> [optional],ylabel="y-axis" -> [optional],absolute_sigma=False -> [optional],jac=None -> [optional],showgui=True -> [optional],**kwargs, -> [optional])`
  - f : callable
         the fit function which if set to None, gives option of selection predefined fit functions
  -  xdata : 1-D numpy array
         x-coordinates of the data
```

### Comparing `complex-curve-fit-gui-1.0.8/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 curvefitgui/_curvefitgui.py
 curvefitgui/_gui.py
 curvefitgui/_settings.py
 curvefitgui/_tools.py
 curvefitgui/_version.py
 curvefitgui/_widgets.py
 curvefitgui/config.txt
-curvefitgui.egg-info/PKG-INFO
-curvefitgui.egg-info/SOURCES.txt
-curvefitgui.egg-info/dependency_links.txt
-curvefitgui.egg-info/top_level.txt
 curvefitgui/__pycache__/__init__.cpython-311.pyc
 curvefitgui/__pycache__/__init__.cpython-39.pyc
 curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
 curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
 curvefitgui/__pycache__/_gui.cpython-311.pyc
 curvefitgui/__pycache__/_gui.cpython-39.pyc
 curvefitgui/__pycache__/_settings.cpython-311.pyc
```

### Comparing `complex-curve-fit-gui-1.0.8/curve.py` & `complex-curve-fit-gui-1.0.9/curve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-
+import os
 from curvefitgui import curve_fit_gui
 
 
 class Main:
     def __init__(self):
         """
         This function are only here to create test data
@@ -13,24 +13,26 @@
             return a * np.exp(-x / b) + c
 
         self.xdata = np.linspace(0, 4, 50)
 
         # y data is only set to None because dummy data generated in backend
         # make to return fit result
         # have option to get rid of guess line
+
         printout = curve_fit_gui(
             None,
             self.xdata,
             None,
-            title="Complex Graph",
+            title="Sin Graph",
             xlabel="y axis",
             ylabel="Imaginary",
             fitline_color="red",
             color="black",
         )
+        # add=[(np.array([1, 2, 3]), np.array([4, 5, 6]), "data2")]
 
 
 w = Main()
 
 # y = exp_decay(self.xdata, 2.5, 1.3, 0.5)
 # rng = np.random.default_rng()
 # yerr = 0.2 * np.ones_like(self.xdata)
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/.DS_Store` & `complex-curve-fit-gui-1.0.9/curvefitgui/.DS_Store`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_gui.cpython-311.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_gui.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Mar 31 04:32:39 2023 UTC, .py size: 13547 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 6762 2664 eb34 0000  a.......gb&d.4..
+00000000: 610d 0d0a 0000 0000 0f45 4364 a33c 0000  a........ECd.<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c05 5a06 6400 6403 6c07  ..d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6404 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6405 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -18,604 +18,677 @@
 00000110: 0000 2901 da08 7365 7474 696e 6773 2902  ..)...settings).
 00000120: da06 4669 7474 6572 da0f 7661 6c75 655f  ..Fitter..value_
 00000130: 746f 5f73 7472 696e 6729 01da 0b5f 5f76  to_string)...__v
 00000140: 6572 7369 6f6e 5f5f 2903 da0b 4d6f 6465  ersion__)...Mode
 00000150: 6c57 6964 6765 74da 0a50 6c6f 7457 6964  lWidget..PlotWid
 00000160: 6765 74da 0c52 6570 6f72 7457 6964 6765  get..ReportWidge
 00000170: 7463 0000 0000 0000 0000 0000 0000 0000  tc..............
-00000180: 0000 0300 0000 0000 0000 7362 0000 0065  ..........sb...e
+00000180: 0000 0300 0000 0000 0000 736a 0000 0065  ..........sj...e
 00000190: 005a 0164 005a 0264 015a 0387 0066 0164  .Z.d.Z.d.Z...f.d
 000001a0: 0264 0384 085a 0464 0464 0584 005a 0564  .d...Z.d.d...Z.d
-000001b0: 0664 0784 005a 0664 1564 0964 0a84 015a  .d...Z.d.d.d...Z
+000001b0: 0664 0784 005a 0664 1764 0964 0a84 015a  .d...Z.d.d.d...Z
 000001c0: 0764 0b64 0c84 005a 0864 0d64 0e84 005a  .d.d...Z.d.d...Z
 000001d0: 0964 0f64 1084 005a 0a64 1164 1284 005a  .d.d...Z.d.d...Z
-000001e0: 0b64 1364 1484 005a 0c87 0004 005a 0d53  .d.d...Z.....Z.S
-000001f0: 0029 16da 0a4d 6169 6e57 696e 646f 777a  .)...MainWindowz
-00000200: 4d0a 2020 2020 4d61 696e 2063 7572 7665  M.    Main curve
-00000210: 2066 6974 7469 6e67 2077 696e 646f 7720   fitting window 
-00000220: 7769 7468 2064 6174 6120 706c 6f74 2c20  with data plot, 
-00000230: 7265 7369 6475 616c 2070 6c6f 742c 2061  residual plot, a
-00000240: 6e64 2072 6570 6f72 740a 2020 2020 6304  nd report.    c.
-00000250: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000260: 0000 000b 0000 0073 5000 0000 7400 7401  .......sP...t.t.
-00000270: 7c00 8302 a002 a100 0100 7c01 7c00 5f03  |.........|.|._.
-00000280: 7c02 7c03 0200 7c00 5f04 7c00 5f05 6401  |.|...|._.|._.d.
-00000290: 7c00 5f06 7407 6402 1900 7c00 5f08 7c00  |._.t.d...|._.|.
-000002a0: 6a09 6600 6900 7c04 a401 8e01 0100 7c00  j.f.i.|.......|.
-000002b0: 6a0a a00b a100 0100 6400 5300 2903 4e29  j.......d.S.).N)
-000002c0: 024e 4eda 0d58 4552 524f 5257 4152 4e49  .NN..XERRORWARNI
-000002d0: 4e47 290c da05 7375 7065 7272 0e00 0000  NG)...superr....
-000002e0: da08 5f5f 696e 6974 5f5f da06 6669 7474  ..__init__..fitt
-000002f0: 6572 da06 786c 6162 656c da06 796c 6162  er..xlabel..ylab
-00000300: 656c da06 6f75 7470 7574 7207 0000 00da  el..outputr.....
-00000310: 0d78 6572 726f 7277 6172 6e69 6e67 da07  .xerrorwarning..
-00000320: 696e 6974 4755 49da 0a70 6c6f 7477 6964  initGUI..plotwid
-00000330: 6765 74da 0b75 7064 6174 655f 706c 6f74  get..update_plot
-00000340: 2905 da04 7365 6c66 da07 6166 6974 7465  )...self..afitte
-00000350: 7272 1300 0000 7214 0000 00da 066b 7761  rr....r......kwa
-00000360: 7267 73a9 01da 095f 5f63 6c61 7373 5f5f  rgs....__class__
-00000370: a900 fa37 2f55 7365 7273 2f6b 6f6a 6f2f  ...7/Users/kojo/
-00000380: 6170 7073 2f73 656e 696f 725f 7072 6f6a  apps/senior_proj
-00000390: 6563 745f 7573 632f 6375 7276 6566 6974  ect_usc/curvefit
-000003a0: 6775 692f 5f67 7569 2e70 7972 1100 0000  gui/_gui.pyr....
-000003b0: 1600 0000 730e 0000 0000 010e 0606 010e  ....s...........
-000003c0: 0106 010a 0110 047a 134d 6169 6e57 696e  .......z.MainWin
-000003d0: 646f 772e 5f5f 696e 6974 5f5f 6302 0000  dow.__init__c...
-000003e0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-000003f0: 0043 0000 0073 0e00 0000 7400 6a01 a002  .C...s....t.j...
-00000400: a100 0100 6401 5300 2902 7a44 6e65 6564  ....d.S.).zDneed
-00000410: 6564 2074 6f20 7072 6f70 6572 6c79 2071  ed to properly q
-00000420: 7569 7420 7768 656e 2072 756e 6e69 6e67  uit when running
-00000430: 2069 6e20 4950 7974 686f 6e20 636f 6e73   in IPython cons
-00000440: 6f6c 6520 2f20 5370 7964 6572 2049 4445  ole / Spyder IDE
-00000450: 4e29 0372 0400 0000 da0c 5141 7070 6c69  N).r......QAppli
-00000460: 6361 7469 6f6e da04 7175 6974 2902 721a  cation..quit).r.
-00000470: 0000 00da 0565 7665 6e74 721f 0000 0072  .....eventr....r
-00000480: 1f00 0000 7220 0000 00da 0a63 6c6f 7365  ....r .....close
-00000490: 4576 656e 7427 0000 0073 0200 0000 0002  Event'...s......
-000004a0: 7a15 4d61 696e 5769 6e64 6f77 2e63 6c6f  z.MainWindow.clo
-000004b0: 7365 4576 656e 7463 0100 0000 0000 0000  seEventc........
-000004c0: 0000 0000 0700 0000 0600 0000 4b00 0000  ............K...
-000004d0: 736a 0100 007c 00a0 0064 0164 0164 0264  sj...|...d.d.d.d
-000004e0: 03a1 0401 007c 00a0 0164 0474 0217 00a1  .....|...d.t....
-000004f0: 0101 0074 03a0 04a1 007c 005f 057c 00a0  ...t.....|._.|..
-00000500: 067c 006a 05a1 0101 007c 006a 07a0 08a1  .|.j.....|.j....
-00000510: 007c 005f 0974 0a7c 006a 077c 006a 0b7c  .|._.t.|.j.|.j.|
-00000520: 006a 0c66 0369 007c 01a4 018e 017c 005f  .j.f.i.|.....|._
-00000530: 0d74 0e7c 006a 076a 0f7c 006a 07a0 10a1  .t.|.j.j.|.j....
-00000540: 0083 027c 005f 1174 036a 1264 057c 006a  ...|._.t.j.d.|.j
-00000550: 1364 068d 027c 005f 1474 036a 1264 077c  .d...|._.t.j.d.|
-00000560: 006a 1564 068d 027c 005f 1674 1783 007c  .j.d...|._.t...|
-00000570: 005f 1874 036a 1264 087c 006a 1964 068d  ._.t.j.d.|.j.d..
-00000580: 027c 005f 1a74 03a0 1ba1 007c 005f 1c74  .|._.t.....|._.t
-00000590: 03a0 1da1 007d 027c 02a0 1e7c 006a 16a1  .....}.|...|.j..
-000005a0: 0101 007c 02a0 1e7c 006a 14a1 0101 007c  ...|...|.j.....|
-000005b0: 006a 1ca0 1f7c 02a1 0101 0074 03a0 1ba1  .j...|.....t....
-000005c0: 007c 005f 2074 03a0 21a1 007d 037c 006a  .|._ t..!..}.|.j
-000005d0: 117c 006a 1c7c 006a 187c 006a 1a66 0444  .|.j.|.j.|.j.f.D
-000005e0: 005d 107d 047c 03a0 1e7c 04a1 0101 0090  .].}.|...|......
-000005f0: 0171 0c7c 006a 20a0 1f7c 03a1 0101 0074  .q.|.j ..|.....t
-00000600: 03a0 1d7c 006a 05a1 017d 0574 03a0 2274  ...|.j...}.t.."t
-00000610: 236a 246a 25a1 017d 067c 06a0 1e7c 006a  #j$j%..}.|...|.j
-00000620: 0da1 0101 007c 06a0 1e7c 006a 20a1 0101  .....|...|.j ...
-00000630: 007c 05a0 1e7c 06a1 0101 0064 0053 0029  .|...|.....d.S.)
-00000640: 094e e964 0000 0069 8705 0000 6984 0300  .N.d...i....i...
-00000650: 007a 0c63 7572 7665 6669 7467 7569 205a  .z.curvefitgui Z
-00000660: 0346 4954 2901 da07 636c 6963 6b65 647a  .FIT)...clickedz
-00000670: 1249 4e49 5449 414c 2045 5641 4c55 4154  .INITIAL EVALUAT
-00000680: 494f 4e5a 0451 5549 5429 265a 0b73 6574  IONZ.QUIT)&Z.set
-00000690: 4765 6f6d 6574 7279 da0e 7365 7457 696e  Geometry..setWin
-000006a0: 646f 7754 6974 6c65 da0a 4346 4776 6572  dowTitle..CFGver
-000006b0: 7369 6f6e 7204 0000 005a 0751 5769 6467  sionr....Z.QWidg
-000006c0: 6574 da05 5f6d 6169 6e5a 1073 6574 4365  et.._mainZ.setCe
-000006d0: 6e74 7261 6c57 6964 6765 7472 1200 0000  ntralWidgetr....
-000006e0: 5a10 6765 745f 6d6f 6465 6c5f 7265 7375  Z.get_model_resu
-000006f0: 6c74 5a0c 6d6f 6465 6c5f 7265 7375 6c74  ltZ.model_result
-00000700: 720c 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000710: 1800 0000 720b 0000 00da 056d 6f64 656c  ....r......model
-00000720: 5a11 6765 745f 7765 6967 6874 6f70 7469  Z.get_weightopti
-00000730: 6f6e 73da 096d 6f64 656c 7669 6577 da0b  ons..modelview..
-00000740: 5150 7573 6842 7574 746f 6eda 0366 6974  QPushButton..fit
-00000750: 5a09 6669 7462 7574 746f 6eda 0865 7661  Z.fitbutton..eva
-00000760: 6c75 6174 655a 0a65 7661 6c62 7574 746f  luateZ.evalbutto
-00000770: 6e72 0d00 0000 da0a 7265 706f 7274 7669  nr......reportvi
-00000780: 6577 da05 636c 6f73 655a 0a71 7569 7462  ew..closeZ.quitb
-00000790: 7574 746f 6e5a 0951 4772 6f75 7042 6f78  uttonZ.QGroupBox
-000007a0: 5a07 6275 7474 6f6e 735a 0b51 4842 6f78  Z.buttonsZ.QHBox
-000007b0: 4c61 796f 7574 da09 6164 6457 6964 6765  Layout..addWidge
-000007c0: 74da 0973 6574 4c61 796f 7574 5a0f 6669  t..setLayoutZ.fi
-000007d0: 7463 6f6e 7472 6f6c 6672 616d 65da 0b51  tcontrolframe..Q
-000007e0: 5642 6f78 4c61 796f 7574 5a09 5153 706c  VBoxLayoutZ.QSpl
-000007f0: 6974 7465 7272 0300 0000 5a02 5174 5a0a  itterr....Z.QtZ.
-00000800: 486f 7269 7a6f 6e74 616c 2907 721a 0000  Horizontal).r...
-00000810: 0072 1c00 0000 5a0d 6275 7474 6f6e 736c  .r....Z.buttonsl
-00000820: 6179 6f75 745a 1066 6974 636f 6e74 726f  ayoutZ.fitcontro
-00000830: 6c6c 6179 6f75 745a 0677 6964 6765 745a  llayoutZ.widgetZ
-00000840: 0a6d 6169 6e6c 6179 6f75 745a 0873 706c  .mainlayoutZ.spl
-00000850: 6974 7465 7272 1f00 0000 721f 0000 0072  itterr....r....r
-00000860: 2000 0000 7217 0000 002b 0000 0073 5000   ...r....+...sP.
-00000870: 0000 0002 1001 0e01 0a01 0c05 0c03 0201  ................
-00000880: 0401 0401 04fd 0404 02fc 0806 0201 0eff  ................
-00000890: 0603 1201 0401 06ff 0803 0801 1203 0a01  ................
-000008a0: 0801 0c01 0c01 0c03 0a01 0802 0401 0401  ................
-000008b0: 0401 04fc 0806 0e01 0c03 0c01 0e01 0c01  ................
-000008c0: 0c01 7a12 4d61 696e 5769 6e64 6f77 2e69  ..z.MainWindow.i
-000008d0: 6e69 7447 5549 da00 6305 0000 0000 0000  nitGUI..c.......
-000008e0: 0000 0000 0006 0000 0003 0000 0043 0000  .............C..
-000008f0: 0073 7600 0000 7400 a001 a100 7d05 7c02  .sv...t.....}.|.
-00000900: 6401 6b02 721e 7c05 a002 7400 6a01 6a03  d.k.r.|...t.j.j.
-00000910: a101 0100 7c02 6402 6b02 7234 7c05 a002  ....|.d.k.r4|...
-00000920: 7400 6a01 6a04 a101 0100 7c05 a005 7c01  t.j.j.....|...|.
-00000930: a101 0100 7c05 a006 7c03 a101 0100 7c05  ....|...|.....|.
-00000940: a007 6403 a101 0100 7c05 a008 7c04 a101  ..d.....|...|...
-00000950: 0100 7c05 a009 7400 6a01 6a0a a101 0100  ..|...t.j.j.....
-00000960: 7c05 a00b a100 0100 6404 5300 2905 7a14  |.......d.S.).z.
-00000970: 7368 6f77 7320 616e 2069 6e66 6f20 6469  shows an info di
-00000980: 616c 6f67 da08 6372 6974 6963 616c da07  alog..critical..
-00000990: 7761 726e 696e 675a 074d 6573 7361 6765  warningZ.Message
-000009a0: 4e29 0c72 0400 0000 5a0b 514d 6573 7361  N).r....Z.QMessa
-000009b0: 6765 426f 785a 0773 6574 4963 6f6e 5a08  geBoxZ.setIconZ.
-000009c0: 4372 6974 6963 616c da07 5761 726e 696e  Critical..Warnin
-000009d0: 675a 0773 6574 5465 7874 5a12 7365 7449  gZ.setTextZ.setI
-000009e0: 6e66 6f72 6d61 7469 7665 5465 7874 7227  nformativeTextr'
-000009f0: 0000 005a 0f73 6574 4465 7461 696c 6564  ...Z.setDetailed
-00000a00: 5465 7874 5a12 7365 7453 7461 6e64 6172  TextZ.setStandar
-00000a10: 6442 7574 746f 6e73 5a02 4f6b da05 6578  dButtonsZ.Ok..ex
-00000a20: 6563 5f29 0672 1a00 0000 da07 6d65 7373  ec_).r......mess
-00000a30: 6167 655a 0469 636f 6eda 0469 6e66 6fda  ageZ.icon..info.
-00000a40: 0764 6574 6169 6c73 da03 6d73 6772 1f00  .details..msgr..
-00000a50: 0000 721f 0000 0072 2000 0000 da0a 7368  ..r....r .....sh
-00000a60: 6f77 6469 616c 6f67 6200 0000 7316 0000  owdialogb...s...
-00000a70: 0000 0208 0108 010e 0108 010e 010a 010a  ................
-00000a80: 010a 010a 010e 017a 154d 6169 6e57 696e  .......z.MainWin
-00000a90: 646f 772e 7368 6f77 6469 616c 6f67 6302  dow.showdialogc.
-00000aa0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000ab0: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-00000ac0: 5f00 6401 5300 2902 7a4e 6f75 7470 7574  _.d.S.).zNoutput
-00000ad0: 2073 686f 756c 6420 6265 2061 2074 7570   should be a tup
-00000ae0: 6c65 2077 6974 6820 7661 7269 6162 6c65  le with variable
-00000af0: 7320 7468 6174 2061 7265 2072 6574 7572  s that are retur
-00000b00: 6e65 6420 7768 656e 2063 6c6f 7369 6e67  ned when closing
-00000b10: 2074 6865 2061 7070 4ea9 0172 1500 0000   the appN..r....
-00000b20: 2902 721a 0000 0072 1500 0000 721f 0000  ).r....r....r...
-00000b30: 0072 1f00 0000 7220 0000 00da 0a73 6574  .r....r .....set
-00000b40: 5f6f 7574 7075 7470 0000 0073 0200 0000  _outputp...s....
-00000b50: 0002 7a15 4d61 696e 5769 6e64 6f77 2e73  ..z.MainWindow.s
-00000b60: 6574 5f6f 7574 7075 7463 0100 0000 0000  et_outputc......
-00000b70: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00000b80: 0000 7306 0000 007c 006a 0053 0029 017a  ..s....|.j.S.).z
-00000b90: 4361 6c6c 6f77 7320 746f 2072 6574 7572  Callows to retur
-00000ba0: 6e20 7468 6520 6375 7272 656e 746c 7920  n the currently 
-00000bb0: 7374 6f72 6564 206f 7574 7075 7420 6f66  stored output of
-00000bc0: 2074 6865 2061 7070 2077 6865 6e20 636c   the app when cl
-00000bd0: 6f73 6564 723e 0000 00a9 0172 1a00 0000  osedr>.....r....
-00000be0: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-00000bf0: 0a67 6574 5f6f 7574 7075 7474 0000 0073  .get_outputt...s
-00000c00: 0200 0000 0002 7a15 4d61 696e 5769 6e64  ......z.MainWind
-00000c10: 6f77 2e67 6574 5f6f 7574 7075 7463 0100  ow.get_outputc..
-00000c20: 0000 0000 0000 0000 0000 0100 0000 0800  ................
-00000c30: 0000 4300 0000 7382 0000 007a 0e7c 006a  ..C...s....z.|.j
-00000c40: 00a0 01a1 0001 0057 006e 2004 0074 0279  .......W.n ..t.y
-00000c50: 2e01 0001 0001 007c 00a0 0364 0164 02a1  .......|...d.d..
-00000c60: 0201 0059 0064 0353 0030 007c 006a 04a0  ...Y.d.S.0.|.j..
-00000c70: 0569 00a1 0101 007c 006a 066a 07a0 087c  .i.....|.j.j...|
-00000c80: 006a 09a0 0aa1 00a1 0101 007c 006a 066a  .j.........|.j.j
-00000c90: 07a0 0b7c 006a 096a 0c64 0464 058d 01a1  ...|.j.j.d.d....
-00000ca0: 0101 007c 006a 066a 07a0 0da1 0001 007c  ...|.j.j.......|
-00000cb0: 006a 06a0 0ea1 0001 0064 0353 0029 067a  .j.......d.S.).z
-00000cc0: 5075 7064 6174 6573 2074 6865 206d 6f64  Pupdates the mod
-00000cd0: 656c 2061 6e64 2063 6f6d 7075 7465 7320  el and computes 
-00000ce0: 7468 6520 6d6f 6465 6c20 6375 7276 6520  the model curve 
-00000cf0: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
-00000d00: 2070 6172 616d 6574 6572 2076 616c 7565   parameter value
-00000d10: 73fa 2a4e 6f74 2061 2076 616c 6964 2069  s.*Not a valid i
-00000d20: 6e70 7574 2069 6e69 7469 616c 2070 6172  nput initial par
-00000d30: 616d 6574 6572 2076 616c 7565 7372 3500  ameter valuesr5.
-00000d40: 0000 4e46 2901 da05 6368 6563 6b29 0f72  ..NF)...check).r
-00000d50: 2b00 0000 da0b 7265 6164 5f76 616c 7565  +.....read_value
-00000d60: 73da 0a56 616c 7565 4572 726f 7272 3d00  s..ValueErrorr=.
-00000d70: 0000 722f 0000 00da 0d75 7064 6174 655f  ..r/.....update_
-00000d80: 7265 706f 7274 7218 0000 00da 0663 616e  reportr......can
-00000d90: 7661 73da 0b73 6574 5f66 6974 6c69 6e65  vas..set_fitline
-00000da0: 7212 0000 005a 0967 6574 5f63 7572 7665  r....Z.get_curve
-00000db0: da0d 7365 745f 7265 7369 6475 616c 73da  ..set_residuals.
-00000dc0: 0d67 6574 5f72 6573 6964 7561 6c73 5a13  .get_residualsZ.
-00000dd0: 6469 7361 626c 655f 7265 7375 6c74 735f  disable_results_
-00000de0: 626f 7872 1900 0000 7240 0000 0072 1f00  boxr....r@...r..
-00000df0: 0000 721f 0000 0072 2000 0000 722e 0000  ..r....r ...r...
-00000e00: 0078 0000 0073 1c00 0000 0003 0201 0e01  .x...s..........
-00000e10: 0c01 0401 04ff 0403 0803 0c01 1401 0801  ................
-00000e20: 0cff 0403 0c01 7a13 4d61 696e 5769 6e64  ......z.MainWind
-00000e30: 6f77 2e65 7661 6c75 6174 6563 0100 0000  ow.evaluatec....
-00000e40: 0000 0000 0000 0000 0400 0000 0b00 0000  ................
-00000e50: 4300 0000 7354 0100 007a 0e7c 006a 00a0  C...sT...z.|.j..
-00000e60: 01a1 0001 0057 006e 2004 0074 0279 2e01  .....W.n ..t.y..
-00000e70: 0001 0001 007c 00a0 0364 0164 02a1 0201  .....|...d.d....
-00000e80: 0059 0064 0353 0030 007c 006a 046a 05a0  .Y.d.S.0.|.j.j..
-00000e90: 06a1 0001 007c 006a 076a 086a 0964 0375  .....|.j.j.j.d.u
-00000ea0: 0172 627c 006a 0a72 627c 00a0 0364 0464  .rb|.j.rb|...d.d
-00000eb0: 05a1 0201 0064 067c 005f 0a74 0ba0 0ca1  .....d.|._.t....
-00000ec0: 008f d401 0074 0ba0 0d64 0774 0ea1 0201  .....t...d.t....
-00000ed0: 007a 147c 006a 07a0 0fa1 005c 037d 017d  .z.|.j.....\.}.}
-00000ee0: 027d 0357 006e 3004 0074 0274 1074 0e66  .}.W.n0..t.t.t.f
-00000ef0: 0379 bc01 0001 0001 007c 00a0 0374 1174  .y.......|...t.t
-00000f00: 12a0 13a1 0064 0819 0083 0164 02a1 0201  .....d.....d....
-00000f10: 0059 006e 7430 007c 00a0 147c 017c 027c  .Y.nt0.|...|.|.|
-00000f20: 0366 03a1 0101 007c 006a 00a0 15a1 0001  .f.....|.j......
-00000f30: 007c 006a 16a0 177c 006a 07a0 18a1 00a1  .|.j...|.j......
-00000f40: 0101 007c 006a 046a 05a0 197c 006a 07a0  ...|.j.j...|.j..
-00000f50: 1aa1 00a1 0101 007c 006a 046a 05a0 1b7c  .......|.j.j...|
-00000f60: 006a 07a0 1ca1 00a1 0101 007c 006a 046a  .j.........|.j.j
-00000f70: 05a0 1d7c 00a0 1ea1 0064 09a1 0201 007c  ...|.....d.....|
-00000f80: 006a 04a0 1fa1 0001 0057 0064 0304 0004  .j.......W.d....
-00000f90: 0083 0301 006e 1231 0090 0173 4630 0001  .....n.1...sF0..
-00000fa0: 0001 0001 0059 0001 0064 0353 0029 0a7a  .....Y...d.S.).z
-00000fb0: 4b75 7064 6174 6573 2074 6865 206d 6f64  Kupdates the mod
-00000fc0: 656c 2070 6572 666f 726d 7320 7468 6520  el performs the 
-00000fd0: 6669 7420 616e 6420 7570 6461 7465 7320  fit and updates 
-00000fe0: 7468 6520 7769 6467 6574 7320 7769 7468  the widgets with
-00000ff0: 2074 6865 2072 6573 756c 7473 7242 0000   the resultsrB..
-00001000: 0072 3500 0000 4e7a 2554 6865 2065 7272  .r5...Nz%The err
-00001010: 6f72 2069 6e20 7820 6973 2069 676e 6f72  or in x is ignor
-00001020: 6564 2069 6e20 7468 6520 6669 7421 7236  ed in the fit!r6
-00001030: 0000 0046 da05 6572 726f 7272 0600 0000  ...F..errorr....
-00001040: e902 0000 0029 2072 2b00 0000 7244 0000  .....) r+...rD..
-00001050: 0072 4500 0000 723d 0000 0072 1800 0000  .rE...r=...r....
-00001060: 7247 0000 005a 0967 6574 5f72 616e 6765  rG...Z.get_range
-00001070: 7212 0000 00da 0464 6174 615a 0278 6572  r......dataZ.xer
-00001080: 1600 0000 da08 7761 726e 696e 6773 da0e  ......warnings..
-00001090: 6361 7463 685f 7761 726e 696e 6773 da0c  catch_warnings..
-000010a0: 7369 6d70 6c65 6669 6c74 6572 7205 0000  simplefilterr...
-000010b0: 0072 2d00 0000 da0c 5275 6e74 696d 6545  .r-.....RuntimeE
-000010c0: 7272 6f72 da03 7374 72da 0373 7973 da08  rror..str..sys..
-000010d0: 6578 635f 696e 666f 723f 0000 005a 0d75  exc_infor?...Z.u
-000010e0: 7064 6174 655f 7661 6c75 6573 722f 0000  pdate_valuesr/..
-000010f0: 0072 4600 0000 5a0a 6765 745f 7265 706f  .rF...Z.get_repo
-00001100: 7274 7248 0000 005a 0c67 6574 5f66 6974  rtrH...Z.get_fit
-00001110: 6375 7276 6572 4900 0000 724a 0000 005a  curverI...rJ...Z
-00001120: 0f73 6574 5f72 6573 756c 7473 5f62 6f78  .set_results_box
-00001130: da14 5f67 6574 5f72 6573 756c 745f 626f  .._get_result_bo
-00001140: 785f 7465 7874 7219 0000 0029 0472 1a00  x_textr....).r..
-00001150: 0000 da07 6669 7470 6172 735a 0666 6974  ....fitparsZ.fit
-00001160: 636f 76da 0672 6573 756c 7472 1f00 0000  cov..resultr....
-00001170: 721f 0000 0072 2000 0000 722d 0000 008c  r....r ...r-....
-00001180: 0000 0073 3c00 0000 0003 0201 0e01 0c01  ...s<...........
-00001190: 0401 04ff 0403 0803 0c03 1401 0c01 0603  ................
-000011a0: 0a01 0401 04ff 0403 0201 1401 1201 1e07  ................
-000011b0: 1003 0a01 1201 1401 0801 08ff 0403 0801  ................
-000011c0: 08ff 0403 7a0e 4d61 696e 5769 6e64 6f77  ....z.MainWindow
-000011d0: 2e66 6974 6301 0000 0000 0000 0000 0000  .fitc...........
-000011e0: 0007 0000 0007 0000 0043 0000 0073 5c00  .........C...s\.
-000011f0: 0000 6401 7d01 7c01 6402 1700 6403 1700  ..d.}.|.d...d...
-00001200: 7c00 6a00 6a01 6a02 1700 7d01 7c00 6a00  |.j.j.j...}.|.j.
-00001210: 6a01 6a03 4400 5d32 7d02 7c02 6a04 7d03  j.j.D.]2}.|.j.}.
-00001220: 7c02 6a05 7d04 7c02 6a06 7d05 7c02 6a07  |.j.}.|.j.}.|.j.
-00001230: 7d06 7c01 6402 1700 7408 7c03 7c04 7c05  }.|.d...t.|.|.|.
-00001240: 7c06 8304 1700 7d01 7124 7c01 5300 2904  |.....}.q$|.S.).
-00001250: 4e7a 0c46 6974 2072 6573 756c 7473 3ada  Nz.Fit results:.
-00001260: 010a 7a07 7765 6967 6874 3a29 0972 1200  ..z.weight:).r..
-00001270: 0000 722a 0000 005a 0677 6569 6768 7472  ..r*...Z.weightr
-00001280: 5600 0000 da04 6e61 6d65 da05 7661 6c75  V.....name..valu
-00001290: 65da 0573 6967 6d61 da05 6669 7865 6472  e..sigma..fixedr
-000012a0: 0900 0000 2907 721a 0000 00da 0474 6578  ....).r......tex
-000012b0: 745a 0370 6172 da01 6eda 0176 da01 65da  tZ.par..n..v..e.
-000012c0: 0166 721f 0000 0072 1f00 0000 7220 0000  .fr....r....r ..
-000012d0: 0072 5500 0000 bc00 0000 7312 0000 0000  .rU.......s.....
-000012e0: 0104 0116 010e 0106 0106 0106 0106 0118  ................
-000012f0: 017a 1f4d 6169 6e57 696e 646f 772e 5f67  .z.MainWindow._g
-00001300: 6574 5f72 6573 756c 745f 626f 785f 7465  et_result_box_te
-00001310: 7874 2902 7234 0000 0072 3400 0000 290e  xt).r4...r4...).
-00001320: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001330: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001340: 6d65 5f5f da07 5f5f 646f 635f 5f72 1100  me__..__doc__r..
-00001350: 0000 7224 0000 0072 1700 0000 723d 0000  ..r$...r....r=..
-00001360: 0072 3f00 0000 7241 0000 0072 2e00 0000  .r?...rA...r....
-00001370: 722d 0000 0072 5500 0000 da0d 5f5f 636c  r-...rU.....__cl
-00001380: 6173 7363 656c 6c5f 5f72 1f00 0000 721f  asscell__r....r.
-00001390: 0000 0072 1d00 0000 7220 0000 0072 0e00  ...r....r ...r..
-000013a0: 0000 1100 0000 7314 0000 0008 0104 040c  ......s.........
-000013b0: 1108 0408 370a 0e08 0408 0408 1408 3072  ....7.........0r
-000013c0: 0e00 0000 630a 0000 0000 0000 0000 0000  ....c...........
-000013d0: 001b 0000 000a 0000 000b 0000 0073 aa01  .............s..
-000013e0: 0000 7400 6a01 a002 a100 7316 7400 a001  ..t.j.....s.t...
-000013f0: 6700 a101 7d0b 6e0a 7400 6a01 a002 a100  g...}.n.t.j.....
-00001400: 7d0b 6401 8800 7601 722c 6402 6e06 8800  }.d...v.r,d.n...
-00001410: 6401 1900 7d0c 6403 8800 7601 7240 6404  d...}.d...v.r@d.
-00001420: 6e06 8800 6403 1900 7d0d 7c0d 7374 7403  n...d...}.|.stt.
-00001430: 7c00 7c01 7c02 7c03 7c04 7c05 7c08 7c09  |.|.|.|.|.|.|.|.
-00001440: 7c0c 6609 6900 8800 a401 8e01 7d0e 7c0e  |.f.i.......}.|.
-00001450: a004 a100 5300 4700 8700 6601 6405 6406  ....S.G...f.d.d.
-00001460: 8408 6406 7400 6a05 8303 7d0f 7c0f 8300  ..d.t.j...}.|...
-00001470: 7d10 7c10 a006 a100 0100 7c00 6407 7500  }.|.......|.d.u.
-00001480: 72a6 7c10 6a07 7d00 7c02 6407 7500 9001  r.|.j.}.|.d.u...
-00001490: 724c 7408 7c00 8301 7d11 7c11 6a09 7d12  rLt.|...}.|.j.}.
-000014a0: 740a 7c12 8301 7d13 6408 6701 7c13 1400  t.|...}.d.g.|...
-000014b0: 7d14 740b 740a 7c14 8301 8301 4400 5d14  }.t.t.|.....D.].
-000014c0: 7d15 740c a00d 6409 640a a102 7c14 7c15  }.t...d.d...|.|.
-000014d0: 3c00 71dc 7c00 7c01 6701 7c14 640b 6407  <.q.|.|.g.|.d.d.
-000014e0: 8502 1900 a201 5200 8e00 7d16 740e 7c14  ......R...}.t.|.
-000014f0: 640b 6407 8502 1900 8301 0100 740f 6a0c  d.d.........t.j.
-00001500: a010 a100 7d17 640c 740f a011 7c01 a101  ....}.d.t...|...
-00001510: 1400 7d18 7c18 7c17 6a12 7c01 6a13 640d  ..}.|.|.j.|.j.d.
-00001520: 8d01 1400 7d19 7c16 7c19 1700 7d02 7c10  ....}.|.|...}.|.
-00001530: 6a14 9001 725c 6404 8800 6401 3c00 7403  j...r\d...d.<.t.
-00001540: 7c00 7c01 7c02 7c03 7c04 7c05 7c08 7c09  |.|.|.|.|.|.|.|.
-00001550: 7c10 6a14 6609 6900 8800 a401 8e01 7d0e  |.j.f.i.......}.
-00001560: 7415 7c0e 7c06 7c07 6603 6900 8800 a401  t.|.|.|.f.i.....
-00001570: 8e01 7d1a 7c1a a016 a100 0100 7c0b a006  ..}.|.......|...
-00001580: a100 0100 7c1a a017 a100 5300 290e 7a54  ....|.....S.).zT
-00001590: 0a20 2020 2068 656c 7065 7220 6675 6e63  .    helper func
-000015a0: 7469 6f6e 2074 6861 7420 6578 6563 7574  tion that execut
-000015b0: 6573 2074 6865 2047 5549 2077 6974 6820  es the GUI with 
-000015c0: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
-000015d0: 6865 2066 6974 7465 7220 636c 6173 730a  he fitter class.
-000015e0: 2020 2020 da07 636f 6d70 6c65 7846 da07      ..complexF..
-000015f0: 7368 6f77 6775 6954 6300 0000 0000 0000  showguiTc.......
-00001600: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-00001610: 0073 2a00 0000 6500 5a01 6400 5a02 6401  .s*...e.Z.d.Z.d.
-00001620: 5a03 8700 8701 6602 6402 6403 8408 5a04  Z.....f.d.d...Z.
-00001630: 6404 6405 8400 5a05 8700 0400 5a06 5300  d.d...Z.....Z.S.
-00001640: 2906 7a21 6578 6563 7574 655f 6775 692e  ).z!execute_gui.
-00001650: 3c6c 6f63 616c 733e 2e43 7573 746f 6d44  <locals>.CustomD
-00001660: 6961 6c6f 677a 4c0a 2020 2020 2020 2020  ialogzL.        
-00001670: 6368 6f6f 7365 2066 6974 2c20 7374 6172  choose fit, star
-00001680: 7469 6e67 2064 6961 6c6f 6720 7468 6174  ting dialog that
-00001690: 2061 6c6c 6f77 7320 7573 6572 2074 6f20   allows user to 
-000016a0: 6368 6f6f 7365 2066 6974 0a20 2020 2020  choose fit.     
-000016b0: 2020 2063 0100 0000 0000 0000 0000 0000     c............
-000016c0: 0a00 0000 0800 0000 1300 0000 7312 0100  ............s...
-000016d0: 0074 0083 00a0 01a1 0001 0064 0188 0176  .t.........d...v
-000016e0: 0172 1664 026e 0688 0164 0119 007c 005f  .r.d.n...d...|._
-000016f0: 0264 0364 0484 007d 0164 0564 0684 007d  .d.d...}.d.d...}
-00001700: 0264 0764 0884 007d 0364 0964 0a84 007d  .d.d...}.d.d...}
-00001710: 0464 0b64 0c84 007d 0564 0d64 0e84 007d  .d.d...}.d.d...}
-00001720: 0664 0f64 1084 007d 077c 017c 027c 037c  .d.d...}.|.|.|.|
-00001730: 047c 057c 067c 0764 119c 077c 005f 037c  .|.|.|.d...|._.|
-00001740: 00a0 0464 12a1 0101 0074 05a0 0664 13a1  ...d.....t...d..
-00001750: 017c 005f 0774 05a0 08a1 007c 005f 0974  .|._.t.....|._.t
-00001760: 05a0 0a64 14a1 017d 0874 05a0 0ba1 007c  ...d...}.t.....|
-00001770: 005f 0c7c 006a 0344 005d 107d 097c 006a  ._.|.j.D.].}.|.j
-00001780: 0ca0 0d7c 09a1 0101 0071 a87c 006a 09a0  ...|.....q.|.j..
-00001790: 0e7c 08a1 0101 007c 006a 09a0 0e7c 006a  .|.....|.j...|.j
-000017a0: 0ca1 0101 007c 006a 09a0 0e7c 006a 07a1  .....|.j...|.j..
-000017b0: 0101 007c 006a 076a 0fa0 107c 006a 11a1  ...|.j.j...|.j..
-000017c0: 0101 007c 006a 076a 0fa0 107c 006a 12a1  ...|.j.j...|.j..
-000017d0: 0101 007c 00a0 137c 006a 09a1 0101 0064  ...|...|.j.....d
-000017e0: 0053 0029 154e 7267 0000 0046 6303 0000  .S.).Nrg...Fc...
-000017f0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00001800: 0053 0000 0073 0c00 0000 7c01 7c00 1400  .S...s....|.|...
-00001810: 7c02 1700 5300 2901 7a49 0a20 2020 2020  |...S.).zI.     
-00001820: 2020 2020 2020 2020 2020 206c 696e 6561             linea
-00001830: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00001840: 2020 6675 6e63 7469 6f6e 3a20 6178 202b    function: ax +
-00001850: 2062 0a20 2020 2020 2020 2020 2020 2020   b.             
-00001860: 2020 2072 1f00 0000 2903 da01 78da 0161     r....)...x..a
-00001870: da01 6272 1f00 0000 721f 0000 0072 2000  ..br....r....r .
-00001880: 0000 da06 6c69 6e65 6172 fe00 0000 7302  ....linear....s.
-00001890: 0000 0000 067a 3a65 7865 6375 7465 5f67  .....z:execute_g
-000018a0: 7569 2e3c 6c6f 6361 6c73 3e2e 4375 7374  ui.<locals>.Cust
-000018b0: 6f6d 4469 616c 6f67 2e5f 5f69 6e69 745f  omDialog.__init_
-000018c0: 5f2e 3c6c 6f63 616c 733e 2e6c 696e 6561  _.<locals>.linea
-000018d0: 7263 0400 0000 0000 0000 0000 0000 0400  rc..............
-000018e0: 0000 0500 0000 5300 0000 7318 0000 007c  ......S...s....|
-000018f0: 0174 00a0 017c 000b 007c 021b 00a1 0114  .t...|...|......
-00001900: 007c 0317 0053 0029 017a b30a 2020 2020  .|...S.).z..    
-00001910: 2020 2020 2020 2020 2020 2020 6578 706f              expo
-00001920: 6e65 6e74 6961 6c20 6465 6361 790a 2020  nential decay.  
-00001930: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-00001940: 6e63 7469 6f6e 3a20 6120 2a20 6578 7028  nction: a * exp(
-00001950: 2d78 202f 2062 2920 2b20 630a 2020 2020  -x / b) + c.    
-00001960: 2020 2020 2020 2020 2020 2020 6120 3a20              a : 
-00001970: 616d 706c 6974 7564 650a 2020 2020 2020  amplitude.      
-00001980: 2020 2020 2020 2020 2020 6220 3a20 7261            b : ra
-00001990: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
-000019a0: 2020 2063 203a 206f 6666 7365 740a 2020     c : offset.  
-000019b0: 2020 2020 2020 2020 2020 2020 2020 a902                ..
-000019c0: da02 6e70 da03 6578 7029 0472 6900 0000  ..np..exp).ri...
-000019d0: 726a 0000 0072 6b00 0000 da01 6372 1f00  rj...rk.....cr..
-000019e0: 0000 721f 0000 0072 2000 0000 da09 6578  ..r....r .....ex
-000019f0: 705f 6465 6361 7906 0100 0073 0200 0000  p_decay....s....
-00001a00: 0008 7a3d 6578 6563 7574 655f 6775 692e  ..z=execute_gui.
-00001a10: 3c6c 6f63 616c 733e 2e43 7573 746f 6d44  <locals>.CustomD
-00001a20: 6961 6c6f 672e 5f5f 696e 6974 5f5f 2e3c  ialog.__init__.<
-00001a30: 6c6f 6361 6c73 3e2e 6578 705f 6465 6361  locals>.exp_deca
-00001a40: 7963 0500 0000 0000 0000 0000 0000 0500  yc..............
-00001a50: 0000 0500 0000 5300 0000 731a 0000 007c  ......S...s....|
-00001a60: 0174 00a0 017c 027c 0014 007c 0317 00a1  .t...|.|...|....
-00001a70: 0114 007c 0417 0053 0029 017a 3c0a 2020  ...|...S.).z<.  
-00001a80: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-00001a90: 3d20 6120 2a20 636f 7328 6220 2a20 7820  = a * cos(b * x 
-00001aa0: 2b20 6329 202b 2064 0a20 2020 2020 2020  + c) + d.       
-00001ab0: 2020 2020 2020 2020 2029 0272 6e00 0000           ).rn...
-00001ac0: da03 636f 73a9 0572 6900 0000 726a 0000  ..cos..ri...rj..
-00001ad0: 0072 6b00 0000 7270 0000 00da 0164 721f  .rk...rp.....dr.
-00001ae0: 0000 0072 1f00 0000 7220 0000 00da 0f63  ...r....r .....c
-00001af0: 6f73 696e 655f 6675 6e63 7469 6f6e 1001  osine_function..
-00001b00: 0000 7302 0000 0000 047a 4365 7865 6375  ..s......zCexecu
-00001b10: 7465 5f67 7569 2e3c 6c6f 6361 6c73 3e2e  te_gui.<locals>.
-00001b20: 4375 7374 6f6d 4469 616c 6f67 2e5f 5f69  CustomDialog.__i
-00001b30: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e63  nit__.<locals>.c
-00001b40: 6f73 696e 655f 6675 6e63 7469 6f6e 6306  osine_functionc.
-00001b50: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00001b60: 0000 0053 0000 0073 2a00 0000 7c01 7400  ...S...s*...|.t.
-00001b70: a001 7c00 0b00 7c02 1b00 a101 1400 7400  ..|...|.......t.
-00001b80: a002 7c03 7c00 1400 7c04 1700 a101 1400  ..|.|...|.......
-00001b90: 7c05 1700 5300 2901 7a4a 0a20 2020 2020  |...S.).zJ.     
-00001ba0: 2020 2020 2020 2020 2020 2079 203d 2061             y = a
-00001bb0: 202a 2065 7870 282d 7820 2f20 6229 202a   * exp(-x / b) *
-00001bc0: 2063 6f73 2863 202a 2078 202b 2064 2920   cos(c * x + d) 
-00001bd0: 2b20 650a 2020 2020 2020 2020 2020 2020  + e.            
-00001be0: 2020 2020 a903 726e 0000 0072 6f00 0000      ..rn...ro...
-00001bf0: 7272 0000 00a9 0672 6900 0000 726a 0000  rr.....ri...rj..
-00001c00: 0072 6b00 0000 7270 0000 0072 7400 0000  .rk...rp...rt...
-00001c10: 7260 0000 0072 1f00 0000 721f 0000 0072  r`...r....r....r
-00001c20: 2000 0000 da14 6465 6361 7969 6e67 5f6f   .....decaying_o
-00001c30: 7363 696c 6c61 7469 6f6e 1601 0000 7302  scillation....s.
-00001c40: 0000 0000 047a 4865 7865 6375 7465 5f67  .....zHexecute_g
-00001c50: 7569 2e3c 6c6f 6361 6c73 3e2e 4375 7374  ui.<locals>.Cust
-00001c60: 6f6d 4469 616c 6f67 2e5f 5f69 6e69 745f  omDialog.__init_
-00001c70: 5f2e 3c6c 6f63 616c 733e 2e64 6563 6179  _.<locals>.decay
-00001c80: 696e 675f 6f73 6369 6c6c 6174 696f 6e63  ing_oscillationc
-00001c90: 0600 0000 0000 0000 0000 0000 0600 0000  ................
-00001ca0: 0500 0000 5300 0000 732e 0000 007c 0174  ....S...s....|.t
-00001cb0: 00a0 017c 000b 007c 021b 00a1 0164 0113  ...|...|.....d..
-00001cc0: 0014 0074 00a0 027c 037c 0014 007c 0417  ...t...|.|...|..
-00001cd0: 00a1 0114 007c 0517 0053 0029 027a 4c0a  .....|...S.).zL.
-00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cf0: 7920 3d20 6120 2a20 6578 7028 2d78 202f  y = a * exp(-x /
-00001d00: 2062 295e 3220 2a20 636f 7328 6320 2a20   b)^2 * cos(c * 
-00001d10: 7820 2b20 6429 202b 2065 0a20 2020 2020  x + d) + e.     
-00001d20: 2020 2020 2020 2020 2020 2072 4c00 0000             rL...
-00001d30: 7276 0000 0072 7700 0000 721f 0000 0072  rv...rw...r....r
-00001d40: 1f00 0000 7220 0000 00da 1564 6563 6179  ....r .....decay
-00001d50: 696e 675f 6f73 6369 6c6c 6174 696f 6e32  ing_oscillation2
-00001d60: 1c01 0000 7302 0000 0000 047a 4965 7865  ....s......zIexe
-00001d70: 6375 7465 5f67 7569 2e3c 6c6f 6361 6c73  cute_gui.<locals
-00001d80: 3e2e 4375 7374 6f6d 4469 616c 6f67 2e5f  >.CustomDialog._
-00001d90: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00001da0: 2e64 6563 6179 696e 675f 6f73 6369 6c6c  .decaying_oscill
-00001db0: 6174 696f 6e32 6302 0000 0000 0000 0000  ation2c.........
-00001dc0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-00001dd0: 1200 0000 7c01 7400 a001 6401 7c00 1400  ....|.t...d.|...
-00001de0: a101 1400 5300 2902 7a4c 0a20 2020 2020  ....S.).zL.     
-00001df0: 2020 2020 2020 2020 2020 2045 756c 6572             Euler
-00001e00: 2773 0a20 2020 2020 2020 2020 2020 2020  's.             
-00001e10: 2020 2079 203d 2061 202a 2065 7870 2869     y = a * exp(i
-00001e20: 202a 2078 290a 2020 2020 2020 2020 2020   * x).          
-00001e30: 2020 2020 2020 f900 0000 0000 0000 0000        ..........
-00001e40: 0000 0000 00f0 3f72 6d00 0000 2902 7269  ......?rm...).ri
-00001e50: 0000 0072 6a00 0000 721f 0000 0072 1f00  ...rj...r....r..
-00001e60: 0000 7220 0000 00da 0565 756c 6572 2201  ..r .....euler".
-00001e70: 0000 7302 0000 0000 057a 3965 7865 6375  ..s......z9execu
-00001e80: 7465 5f67 7569 2e3c 6c6f 6361 6c73 3e2e  te_gui.<locals>.
-00001e90: 4375 7374 6f6d 4469 616c 6f67 2e5f 5f69  CustomDialog.__i
-00001ea0: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e65  nit__.<locals>.e
-00001eb0: 756c 6572 6305 0000 0000 0000 0000 0000  ulerc...........
-00001ec0: 0005 0000 0006 0000 0053 0000 0073 1e00  .........S...s..
-00001ed0: 0000 7c01 7400 a001 6401 7c02 7c00 1400  ..|.t...d.|.|...
-00001ee0: 7c03 1700 1400 a101 1400 7c04 1700 5300  |.........|...S.
-00001ef0: 2902 7a5e 0a20 2020 2020 2020 2020 2020  ).z^.           
-00001f00: 2020 2020 2063 6f6d 706c 6578 2065 7870       complex exp
-00001f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f20: 2079 203d 2061 202a 2065 7870 2869 202a   y = a * exp(i *
-00001f30: 2028 6220 2a20 7720 2b20 6329 2920 2b20   (b * w + c)) + 
-00001f40: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00001f50: 2020 727a 0000 0072 6d00 0000 7273 0000    rz...rm...rs..
-00001f60: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00001f70: da10 636f 6d70 6c65 785f 6675 6e63 7469  ..complex_functi
-00001f80: 6f6e 2901 0000 7302 0000 0000 057a 4465  on)...s......zDe
-00001f90: 7865 6375 7465 5f67 7569 2e3c 6c6f 6361  xecute_gui.<loca
-00001fa0: 6c73 3e2e 4375 7374 6f6d 4469 616c 6f67  ls>.CustomDialog
-00001fb0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-00001fc0: 733e 2e63 6f6d 706c 6578 5f66 756e 6374  s>.complex_funct
-00001fd0: 696f 6e29 077a 0a79 203d 2061 7820 2b20  ion).z.y = ax + 
-00001fe0: 627a 1779 203d 2061 202a 2065 7870 282d  bz.y = a * exp(-
-00001ff0: 7820 2f20 6229 202b 2063 7a18 7920 3d20  x / b) + cz.y = 
-00002000: 6120 2a20 636f 7328 622a 7820 2b20 6329  a * cos(b*x + c)
-00002010: 202b 2064 7a28 7920 3d20 6120 2a20 6578   + dz(y = a * ex
-00002020: 7028 2d78 202f 2062 2920 2a20 636f 7328  p(-x / b) * cos(
-00002030: 6320 2a20 7820 2b20 6429 202b 2065 7a2a  c * x + d) + ez*
-00002040: 7920 3d20 6120 2a20 6578 7028 2d78 202f  y = a * exp(-x /
-00002050: 2062 295e 3220 2a20 636f 7328 6320 2a20   b)^2 * cos(c * 
-00002060: 7820 2b20 6429 202b 2065 7a12 7920 3d20  x + d) + ez.y = 
-00002070: 6120 2a20 6578 7028 6920 2a20 7829 7a20  a * exp(i * x)z 
-00002080: 7920 3d20 6120 2a20 6578 7028 6920 2a20  y = a * exp(i * 
-00002090: 2862 202a 2077 202b 2063 2929 202b 2064  (b * w + c)) + d
-000020a0: 7a0a 4368 6f6f 7365 2046 6974 5a05 5374  z.Choose FitZ.St
-000020b0: 6172 747a 0c43 686f 6f73 6520 4375 7276  artz.Choose Curv
-000020c0: 6529 1472 1000 0000 7211 0000 00da 0a69  e).r....r......i
-000020d0: 735f 636f 6d70 6c65 78da 0c66 756e 6374  s_complex..funct
-000020e0: 696f 6e5f 6d61 7072 2700 0000 7204 0000  ion_mapr'...r...
-000020f0: 0072 2c00 0000 5a06 6275 7474 6f6e 7233  .r,...Z.buttonr3
-00002100: 0000 005a 0d64 6961 6c6f 675f 6c61 796f  ...Z.dialog_layo
-00002110: 7574 5a06 514c 6162 656c 5a09 5143 6f6d  utZ.QLabelZ.QCom
-00002120: 626f 426f 78da 0863 6f6d 626f 626f 785a  boBox..comboboxZ
-00002130: 0761 6464 4974 656d 7231 0000 0072 2600  .addItemr1...r&.
-00002140: 0000 5a07 636f 6e6e 6563 74da 0867 6574  ..Z.connect..get
-00002150: 5f74 6578 7472 3000 0000 7232 0000 0029  _textr0...r2...)
-00002160: 0a72 1a00 0000 726c 0000 0072 7100 0000  .r....rl...rq...
-00002170: 7275 0000 0072 7800 0000 7279 0000 0072  ru...rx...ry...r
-00002180: 7b00 0000 727c 0000 0072 3900 0000 da04  {...r|...r9.....
-00002190: 6974 656d 2902 721e 0000 0072 1c00 0000  item).r....r....
-000021a0: 721f 0000 0072 2000 0000 7211 0000 00f7  r....r ...r.....
-000021b0: 0000 0073 3e00 0000 0001 0a03 12ff 0404  ...s>...........
-000021c0: 0808 080a 0806 0806 0806 0807 0808 0201  ................
-000021d0: 0201 0201 0201 0201 0201 02f9 080d 0a01  ................
-000021e0: 0c01 0a01 0a02 0a02 0a01 0e05 0c01 0e01  ................
-000021f0: 0e01 1001 1002 7a2a 6578 6563 7574 655f  ......z*execute_
-00002200: 6775 692e 3c6c 6f63 616c 733e 2e43 7573  gui.<locals>.Cus
-00002210: 746f 6d44 6961 6c6f 672e 5f5f 696e 6974  tomDialog.__init
-00002220: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-00002230: 0000 0003 0000 0053 0000 0073 3000 0000  .......S...s0...
-00002240: 6401 7c00 6a00 a001 a100 7600 7212 6402  d.|.j.....v.r.d.
-00002250: 6e04 7c00 6a02 7c00 5f02 7c00 6a03 7c00  n.|.j.|._.|.j.|.
-00002260: 6a00 a001 a100 1900 7c00 5f04 6403 5300  j.......|._.d.S.
-00002270: 2904 7a58 0a20 2020 2020 2020 2020 2020  ).zX.           
-00002280: 204f 6e20 6f6b 2066 726f 6d20 7374 6172   On ok from star
-00002290: 7469 6e67 2070 6f70 2075 7020 7468 6973  ting pop up this
-000022a0: 2066 756e 6374 696f 6e20 7365 7473 2074   function sets t
-000022b0: 6865 2066 6974 2066 756e 6374 696f 6e0a  he fit function.
-000022c0: 2020 2020 2020 2020 2020 2020 da01 6954              ..iT
-000022d0: 4e29 0572 7f00 0000 5a0b 6375 7272 656e  N).r....Z.curren
-000022e0: 7454 6578 7472 7d00 0000 727e 0000 00da  tTextr}...r~....
-000022f0: 0466 756e 6372 4000 0000 721f 0000 0072  .funcr@...r....r
-00002300: 1f00 0000 7220 0000 0072 8000 0000 5201  ....r ...r....R.
-00002310: 0000 7306 0000 0000 0516 ff04 037a 2a65  ..s..........z*e
-00002320: 7865 6375 7465 5f67 7569 2e3c 6c6f 6361  xecute_gui.<loca
-00002330: 6c73 3e2e 4375 7374 6f6d 4469 616c 6f67  ls>.CustomDialog
-00002340: 2e67 6574 5f74 6578 7429 0772 6200 0000  .get_text).rb...
-00002350: 7263 0000 0072 6400 0000 7265 0000 0072  rc...rd...re...r
-00002360: 1100 0000 7280 0000 0072 6600 0000 721f  ....r....rf...r.
-00002370: 0000 00a9 0172 1c00 0000 721d 0000 0072  .....r....r....r
-00002380: 2000 0000 da0c 4375 7374 6f6d 4469 616c   .....CustomDial
-00002390: 6f67 f200 0000 7306 0000 0008 0104 040e  og....s.........
-000023a0: 5b72 8500 0000 4e72 0100 0000 6700 0000  [r....Nr....g...
-000023b0: 0000 00e0 3fe9 0400 0000 7206 0000 0067  ....?.....r....g
-000023c0: 9a99 9999 9999 c93f 2901 da04 7369 7a65  .......?)...size
-000023d0: 2918 7204 0000 0072 2100 0000 da08 696e  ).r....r!.....in
-000023e0: 7374 616e 6365 7208 0000 0072 2d00 0000  stancer....r-...
-000023f0: 5a07 5144 6961 6c6f 6772 3800 0000 7283  Z.QDialogr8...r.
-00002400: 0000 0072 0200 0000 da0a 7061 7261 6d65  ...r......parame
-00002410: 7465 7273 da03 6c65 6eda 0572 616e 6765  ters..len..range
-00002420: da06 7261 6e64 6f6d da07 756e 6966 6f72  ..random..unifor
-00002430: 6dda 0570 7269 6e74 726e 0000 00da 0b64  m..printrn.....d
-00002440: 6566 6175 6c74 5f72 6e67 da09 6f6e 6573  efault_rng..ones
-00002450: 5f6c 696b 65da 066e 6f72 6d61 6c72 8700  _like..normalr..
-00002460: 0000 727d 0000 0072 0e00 0000 da04 7368  ..r}...r......sh
-00002470: 6f77 7241 0000 0029 1b72 6100 0000 da05  owrA...).ra.....
-00002480: 7864 6174 61da 0579 6461 7461 da04 7865  xdata..ydata..xe
-00002490: 7272 da04 7965 7272 da02 7030 7213 0000  rr..yerr..p0r...
-000024a0: 0072 1400 0000 da0e 6162 736f 6c75 7465  .r......absolute
-000024b0: 5f73 6967 6d61 da03 6a61 6372 1c00 0000  _sigma..jacr....
-000024c0: 5a03 6170 7072 7d00 0000 7268 0000 0072  Z.appr}...rh...r
-000024d0: 1b00 0000 7285 0000 005a 0364 6c67 da03  ....r....Z.dlg..
-000024e0: 7369 67da 0670 6172 616d 735a 0d6e 756d  sig..paramsZ.num
-000024f0: 5f6f 665f 7061 7261 6d73 5a0a 7261 6e64  _of_paramsZ.rand
-00002500: 6f6d 5f61 7272 7282 0000 00da 0179 da03  om_arrr......y..
-00002510: 726e 675a 0974 6573 745f 7965 7272 da07  rngZ.test_yerr..
-00002520: 795f 6e6f 6973 655a 0d4d 7941 7070 6c69  y_noiseZ.MyAppli
-00002530: 6361 7469 6f6e 721f 0000 0072 8400 0000  cationr....r....
-00002540: 7220 0000 00da 0b65 7865 6375 7465 5f67  r .....execute_g
-00002550: 7569 c900 0000 7372 0000 0000 110a 010c  ui....sr........
-00002560: 020a 0214 0214 0204 0102 0102 0102 0102  ................
-00002570: 0102 0102 0102 0102 0102 0102 f704 0a02  ................
-00002580: f606 0c08 0216 6906 0108 0108 0106 0f0a  ......i.........
-00002590: 0108 0106 0108 010a 0110 0112 0518 0110  ................
-000025a0: 050a 010e 0112 0108 0608 0108 0202 0102  ................
-000025b0: 0102 0102 0102 0102 0102 0102 0102 0104  ................
-000025c0: f704 0a02 f606 0d14 0108 0108 0172 9f00  .............r..
-000025d0: 0000 291b 728c 0000 0072 5300 0000 724e  ..).r....rS...rN
-000025e0: 0000 00da 0769 6e73 7065 6374 7202 0000  .....inspectr...
-000025f0: 00da 056e 756d 7079 726e 0000 005a 0550  ...numpyrn...Z.P
-00002600: 7951 7435 7203 0000 0072 0400 0000 5a0e  yQt5r....r....Z.
-00002610: 7363 6970 792e 6f70 7469 6d69 7a65 7205  scipy.optimizer.
-00002620: 0000 00da 095f 7365 7474 696e 6773 7207  ....._settingsr.
-00002630: 0000 005a 065f 746f 6f6c 7372 0800 0000  ...Z._toolsr....
-00002640: 7209 0000 00da 085f 7665 7273 696f 6e72  r......_versionr
-00002650: 0a00 0000 7228 0000 005a 085f 7769 6467  ....r(...Z._widg
-00002660: 6574 7372 0b00 0000 720c 0000 0072 0d00  etsr....r....r..
-00002670: 0000 5a0b 514d 6169 6e57 696e 646f 7772  ..Z.QMainWindowr
-00002680: 0e00 0000 729f 0000 0072 1f00 0000 721f  ....r....r....r.
-00002690: 0000 0072 1f00 0000 7220 0000 00da 083c  ...r....r .....<
-000026a0: 6d6f 6475 6c65 3e02 0000 0073 1a00 0000  module>....s....
-000026b0: 0801 0801 0801 0c02 0801 1001 0c02 0c01  ................
-000026c0: 1001 0c01 1403 127f 0039                 .........9
+000001e0: 0b64 1364 1484 005a 0c64 1564 1684 005a  .d.d...Z.d.d...Z
+000001f0: 0d87 0004 005a 0e53 0029 18da 0a4d 6169  .....Z.S.)...Mai
+00000200: 6e57 696e 646f 777a 4d0a 2020 2020 4d61  nWindowzM.    Ma
+00000210: 696e 2063 7572 7665 2066 6974 7469 6e67  in curve fitting
+00000220: 2077 696e 646f 7720 7769 7468 2064 6174   window with dat
+00000230: 6120 706c 6f74 2c20 7265 7369 6475 616c  a plot, residual
+00000240: 2070 6c6f 742c 2061 6e64 2072 6570 6f72   plot, and repor
+00000250: 740a 2020 2020 6304 0000 0000 0000 0000  t.    c.........
+00000260: 0000 0005 0000 0004 0000 000b 0000 0073  ...............s
+00000270: 6000 0000 7400 7401 7c00 8302 a002 a100  `...t.t.|.......
+00000280: 0100 7c01 7c00 5f03 7c02 7c03 0200 7c00  ..|.|._.|.|...|.
+00000290: 5f04 7c00 5f05 6401 7c00 5f06 7407 6402  _.|._.d.|._.t.d.
+000002a0: 1900 7c00 5f08 7c04 7c00 5f09 7c00 6a0a  ..|._.|.|._.|.j.
+000002b0: 6600 6900 7c04 a401 8e01 0100 7c00 6a0b  f.i.|.......|.j.
+000002c0: a00c a100 0100 7c00 6a03 6a0d 7c00 5f0e  ......|.j.j.|._.
+000002d0: 6400 5300 2903 4e29 024e 4eda 0d58 4552  d.S.).N).NN..XER
+000002e0: 524f 5257 4152 4e49 4e47 290f da05 7375  RORWARNING)...su
+000002f0: 7065 7272 0e00 0000 da08 5f5f 696e 6974  perr......__init
+00000300: 5f5f da06 6669 7474 6572 da06 786c 6162  __..fitter..xlab
+00000310: 656c da06 796c 6162 656c da06 6f75 7470  el..ylabel..outp
+00000320: 7574 7207 0000 00da 0d78 6572 726f 7277  utr......xerrorw
+00000330: 6172 6e69 6e67 da06 6b77 6172 6773 da07  arning..kwargs..
+00000340: 696e 6974 4755 49da 0a70 6c6f 7477 6964  initGUI..plotwid
+00000350: 6765 74da 0b75 7064 6174 655f 706c 6f74  get..update_plot
+00000360: da05 6d6f 6465 6cda 084f 475f 6d6f 6465  ..model..OG_mode
+00000370: 6c29 05da 0473 656c 66da 0761 6669 7474  l)...self..afitt
+00000380: 6572 7213 0000 0072 1400 0000 7217 0000  err....r....r...
+00000390: 00a9 01da 095f 5f63 6c61 7373 5f5f a900  .....__class__..
+000003a0: fa37 2f55 7365 7273 2f6b 6f6a 6f2f 6170  .7/Users/kojo/ap
+000003b0: 7073 2f73 656e 696f 725f 7072 6f6a 6563  ps/senior_projec
+000003c0: 745f 7573 632f 6375 7276 6566 6974 6775  t_usc/curvefitgu
+000003d0: 692f 5f67 7569 2e70 7972 1100 0000 1600  i/_gui.pyr......
+000003e0: 0000 7312 0000 0000 010e 0606 010e 0106  ..s.............
+000003f0: 010a 0106 0110 040a 017a 134d 6169 6e57  .........z.MainW
+00000400: 696e 646f 772e 5f5f 696e 6974 5f5f 6302  indow.__init__c.
+00000410: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000420: 0000 0043 0000 0073 0e00 0000 7400 6a01  ...C...s....t.j.
+00000430: a002 a100 0100 6401 5300 2902 7a44 6e65  ......d.S.).zDne
+00000440: 6564 6564 2074 6f20 7072 6f70 6572 6c79  eded to properly
+00000450: 2071 7569 7420 7768 656e 2072 756e 6e69   quit when runni
+00000460: 6e67 2069 6e20 4950 7974 686f 6e20 636f  ng in IPython co
+00000470: 6e73 6f6c 6520 2f20 5370 7964 6572 2049  nsole / Spyder I
+00000480: 4445 4e29 0372 0400 0000 da0c 5141 7070  DEN).r......QApp
+00000490: 6c69 6361 7469 6f6e da04 7175 6974 2902  lication..quit).
+000004a0: 721d 0000 00da 0565 7665 6e74 7221 0000  r......eventr!..
+000004b0: 0072 2100 0000 7222 0000 00da 0a63 6c6f  .r!...r".....clo
+000004c0: 7365 4576 656e 7429 0000 0073 0200 0000  seEvent)...s....
+000004d0: 0002 7a15 4d61 696e 5769 6e64 6f77 2e63  ..z.MainWindow.c
+000004e0: 6c6f 7365 4576 656e 7463 0100 0000 0000  loseEventc......
+000004f0: 0000 0000 0000 0600 0000 0600 0000 4b00  ..............K.
+00000500: 0000 7380 0100 007c 00a0 0064 0164 0164  ..s....|...d.d.d
+00000510: 0264 03a1 0401 007c 00a0 0164 0474 0217  .d.....|...d.t..
+00000520: 00a1 0101 0074 03a0 04a1 007c 005f 057c  .....t.....|._.|
+00000530: 00a0 067c 006a 05a1 0101 007c 006a 07a0  ...|.j.....|.j..
+00000540: 08a1 007c 005f 0974 0a7c 006a 077c 006a  ...|._.t.|.j.|.j
+00000550: 0b7c 006a 0c66 0369 007c 01a4 018e 017c  .|.j.f.i.|.....|
+00000560: 005f 0d7c 006a 0d6a 0ea0 0f7c 006a 10a1  ._.|.j.j...|.j..
+00000570: 0101 0074 117c 006a 076a 127c 006a 07a0  ...t.|.j.j.|.j..
+00000580: 13a1 0083 027c 005f 1474 036a 1564 057c  .....|._.t.j.d.|
+00000590: 006a 1664 068d 027c 005f 1774 036a 1564  .j.d...|._.t.j.d
+000005a0: 077c 006a 1864 068d 027c 005f 1974 1a83  .|.j.d...|._.t..
+000005b0: 007c 005f 1b74 036a 1564 087c 006a 1c64  .|._.t.j.d.|.j.d
+000005c0: 068d 027c 005f 1d74 03a0 1ea1 007c 005f  ...|._.t.....|._
+000005d0: 1f74 03a0 20a1 007d 027c 02a0 217c 006a  .t.. ..}.|..!|.j
+000005e0: 19a1 0101 007c 02a0 217c 006a 17a1 0101  .....|..!|.j....
+000005f0: 007c 006a 1fa0 227c 02a1 0101 0074 03a0  .|.j.."|.....t..
+00000600: 1ea1 007c 005f 2374 03a0 24a1 007c 005f  ...|._#t..$..|._
+00000610: 257c 006a 147c 006a 1f7c 006a 1b7c 006a  %|.j.|.j.|.j.|.j
+00000620: 1d66 0444 005d 127d 037c 006a 25a0 217c  .f.D.].}.|.j%.!|
+00000630: 03a1 0101 0090 0171 1e7c 006a 23a0 227c  .......q.|.j#."|
+00000640: 006a 25a1 0101 0074 03a0 207c 006a 05a1  .j%....t.. |.j..
+00000650: 017d 0474 03a0 2674 276a 286a 29a1 017d  .}.t..&t'j(j)..}
+00000660: 057c 05a0 217c 006a 0da1 0101 007c 05a0  .|..!|.j.....|..
+00000670: 217c 006a 23a1 0101 007c 04a0 217c 05a1  !|.j#....|..!|..
+00000680: 0101 0064 0053 0029 094e e964 0000 0069  ...d.S.).N.d...i
+00000690: 8705 0000 6984 0300 007a 0c63 7572 7665  ....i....z.curve
+000006a0: 6669 7467 7569 205a 0346 4954 2901 da07  fitgui Z.FIT)...
+000006b0: 636c 6963 6b65 647a 1249 4e49 5449 414c  clickedz.INITIAL
+000006c0: 2045 5641 4c55 4154 494f 4e5a 0451 5549   EVALUATIONZ.QUI
+000006d0: 5429 2a5a 0b73 6574 4765 6f6d 6574 7279  T)*Z.setGeometry
+000006e0: da0e 7365 7457 696e 646f 7754 6974 6c65  ..setWindowTitle
+000006f0: da0a 4346 4776 6572 7369 6f6e 7204 0000  ..CFGversionr...
+00000700: 005a 0751 5769 6467 6574 da05 5f6d 6169  .Z.QWidget.._mai
+00000710: 6e5a 1073 6574 4365 6e74 7261 6c57 6964  nZ.setCentralWid
+00000720: 6765 7472 1200 0000 5a10 6765 745f 6d6f  getr....Z.get_mo
+00000730: 6465 6c5f 7265 7375 6c74 5a0c 6d6f 6465  del_resultZ.mode
+00000740: 6c5f 7265 7375 6c74 720c 0000 0072 1300  l_resultr....r..
+00000750: 0000 7214 0000 0072 1900 0000 5a07 7265  ..r....r....Z.re
+00000760: 5f69 6e69 74da 0763 6f6e 6e65 6374 da07  _init..connect..
+00000770: 7265 6672 6573 6872 0b00 0000 721b 0000  refreshr....r...
+00000780: 00da 1167 6574 5f77 6569 6768 746f 7074  ...get_weightopt
+00000790: 696f 6e73 da09 6d6f 6465 6c76 6965 77da  ions..modelview.
+000007a0: 0b51 5075 7368 4275 7474 6f6e da03 6669  .QPushButton..fi
+000007b0: 745a 0966 6974 6275 7474 6f6e da08 6576  tZ.fitbutton..ev
+000007c0: 616c 7561 7465 5a0a 6576 616c 6275 7474  aluateZ.evalbutt
+000007d0: 6f6e 720d 0000 00da 0a72 6570 6f72 7476  onr......reportv
+000007e0: 6965 77da 0563 6c6f 7365 da0a 7175 6974  iew..close..quit
+000007f0: 6275 7474 6f6e 5a09 5147 726f 7570 426f  buttonZ.QGroupBo
+00000800: 78da 0762 7574 746f 6e73 5a0b 5148 426f  x..buttonsZ.QHBo
+00000810: 784c 6179 6f75 74da 0961 6464 5769 6467  xLayout..addWidg
+00000820: 6574 da09 7365 744c 6179 6f75 74da 0f66  et..setLayout..f
+00000830: 6974 636f 6e74 726f 6c66 7261 6d65 da0b  itcontrolframe..
+00000840: 5156 426f 784c 6179 6f75 74da 1066 6974  QVBoxLayout..fit
+00000850: 636f 6e74 726f 6c6c 6179 6f75 745a 0951  controllayoutZ.Q
+00000860: 5370 6c69 7474 6572 7203 0000 005a 0251  Splitterr....Z.Q
+00000870: 745a 0a48 6f72 697a 6f6e 7461 6c29 0672  tZ.Horizontal).r
+00000880: 1d00 0000 7217 0000 005a 0d62 7574 746f  ....r....Z.butto
+00000890: 6e73 6c61 796f 7574 da06 7769 6467 6574  nslayout..widget
+000008a0: 5a0a 6d61 696e 6c61 796f 7574 5a08 7370  Z.mainlayoutZ.sp
+000008b0: 6c69 7474 6572 7221 0000 0072 2100 0000  litterr!...r!...
+000008c0: 7222 0000 0072 1800 0000 2d00 0000 7356  r"...r....-...sV
+000008d0: 0000 0000 0210 010e 010a 010c 050c 0302  ................
+000008e0: 0104 0104 0104 fd04 0402 fc08 0708 0104  ................
+000008f0: ff04 0402 010e ff06 0312 0104 0106 ff08  ................
+00000900: 0308 0112 030a 0108 010c 010c 010c 030a  ................
+00000910: 010a 0204 0104 0104 0104 fc08 0610 010e  ................
+00000920: 030c 010e 010c 010c 017a 124d 6169 6e57  .........z.MainW
+00000930: 696e 646f 772e 696e 6974 4755 49da 0063  indow.initGUI..c
+00000940: 0500 0000 0000 0000 0000 0000 0600 0000  ................
+00000950: 0300 0000 4300 0000 7376 0000 0074 00a0  ....C...sv...t..
+00000960: 01a1 007d 057c 0264 016b 0272 1e7c 05a0  ...}.|.d.k.r.|..
+00000970: 0274 006a 016a 03a1 0101 007c 0264 026b  .t.j.j.....|.d.k
+00000980: 0272 347c 05a0 0274 006a 016a 04a1 0101  .r4|...t.j.j....
+00000990: 007c 05a0 057c 01a1 0101 007c 05a0 067c  .|...|.....|...|
+000009a0: 03a1 0101 007c 05a0 0764 03a1 0101 007c  .....|...d.....|
+000009b0: 05a0 087c 04a1 0101 007c 05a0 0974 006a  ...|.....|...t.j
+000009c0: 016a 0aa1 0101 007c 05a0 0ba1 0001 0064  .j.....|.......d
+000009d0: 0453 0029 057a 1473 686f 7773 2061 6e20  .S.).z.shows an 
+000009e0: 696e 666f 2064 6961 6c6f 67da 0863 7269  info dialog..cri
+000009f0: 7469 6361 6cda 0777 6172 6e69 6e67 5a07  tical..warningZ.
+00000a00: 4d65 7373 6167 654e 290c 7204 0000 005a  MessageN).r....Z
+00000a10: 0b51 4d65 7373 6167 6542 6f78 5a07 7365  .QMessageBoxZ.se
+00000a20: 7449 636f 6e5a 0843 7269 7469 6361 6cda  tIconZ.Critical.
+00000a30: 0757 6172 6e69 6e67 5a07 7365 7454 6578  .WarningZ.setTex
+00000a40: 745a 1273 6574 496e 666f 726d 6174 6976  tZ.setInformativ
+00000a50: 6554 6578 7472 2900 0000 5a0f 7365 7444  eTextr)...Z.setD
+00000a60: 6574 6169 6c65 6454 6578 745a 1273 6574  etailedTextZ.set
+00000a70: 5374 616e 6461 7264 4275 7474 6f6e 735a  StandardButtonsZ
+00000a80: 024f 6bda 0565 7865 635f 2906 721d 0000  .Ok..exec_).r...
+00000a90: 00da 076d 6573 7361 6765 5a04 6963 6f6e  ...messageZ.icon
+00000aa0: da04 696e 666f da07 6465 7461 696c 73da  ..info..details.
+00000ab0: 036d 7367 7221 0000 0072 2100 0000 7222  .msgr!...r!...r"
+00000ac0: 0000 00da 0a73 686f 7764 6961 6c6f 6769  .....showdialogi
+00000ad0: 0000 0073 1600 0000 0002 0801 0801 0e01  ...s............
+00000ae0: 0801 0e01 0a01 0a01 0a01 0a01 0e01 7a15  ..............z.
+00000af0: 4d61 696e 5769 6e64 6f77 2e73 686f 7764  MainWindow.showd
+00000b00: 6961 6c6f 6763 0200 0000 0000 0000 0000  ialogc..........
+00000b10: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000b20: 0000 007c 017c 005f 0064 0153 0029 027a  ...|.|._.d.S.).z
+00000b30: 4e6f 7574 7075 7420 7368 6f75 6c64 2062  Noutput should b
+00000b40: 6520 6120 7475 706c 6520 7769 7468 2076  e a tuple with v
+00000b50: 6172 6961 626c 6573 2074 6861 7420 6172  ariables that ar
+00000b60: 6520 7265 7475 726e 6564 2077 6865 6e20  e returned when 
+00000b70: 636c 6f73 696e 6720 7468 6520 6170 704e  closing the appN
+00000b80: a901 7215 0000 0029 0272 1d00 0000 7215  ..r....).r....r.
+00000b90: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00000ba0: 0000 da0a 7365 745f 6f75 7470 7574 7700  ....set_outputw.
+00000bb0: 0000 7302 0000 0000 027a 154d 6169 6e57  ..s......z.MainW
+00000bc0: 696e 646f 772e 7365 745f 6f75 7470 7574  indow.set_output
+00000bd0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000be0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00000bf0: 6a00 5300 2901 7a43 616c 6c6f 7773 2074  j.S.).zCallows t
+00000c00: 6f20 7265 7475 726e 2074 6865 2063 7572  o return the cur
+00000c10: 7265 6e74 6c79 2073 746f 7265 6420 6f75  rently stored ou
+00000c20: 7470 7574 206f 6620 7468 6520 6170 7020  tput of the app 
+00000c30: 7768 656e 2063 6c6f 7365 6472 4700 0000  when closedrG...
+00000c40: a901 721d 0000 0072 2100 0000 7221 0000  ..r....r!...r!..
+00000c50: 0072 2200 0000 da0a 6765 745f 6f75 7470  .r".....get_outp
+00000c60: 7574 7b00 0000 7302 0000 0000 027a 154d  ut{...s......z.M
+00000c70: 6169 6e57 696e 646f 772e 6765 745f 6f75  ainWindow.get_ou
+00000c80: 7470 7574 6301 0000 0000 0000 0000 0000  tputc...........
+00000c90: 0001 0000 0008 0000 0043 0000 0073 8200  .........C...s..
+00000ca0: 0000 7a0e 7c00 6a00 a001 a100 0100 5700  ..z.|.j.......W.
+00000cb0: 6e20 0400 7402 792e 0100 0100 0100 7c00  n ..t.y.......|.
+00000cc0: a003 6401 6402 a102 0100 5900 6403 5300  ..d.d.....Y.d.S.
+00000cd0: 3000 7c00 6a04 a005 6900 a101 0100 7c00  0.|.j...i.....|.
+00000ce0: 6a06 6a07 a008 7c00 6a09 a00a a100 a101  j.j...|.j.......
+00000cf0: 0100 7c00 6a06 6a07 a00b 7c00 6a09 6a0c  ..|.j.j...|.j.j.
+00000d00: 6404 6405 8d01 a101 0100 7c00 6a06 6a07  d.d.......|.j.j.
+00000d10: a00d a100 0100 7c00 6a06 a00e a100 0100  ......|.j.......
+00000d20: 6403 5300 2906 7a50 7570 6461 7465 7320  d.S.).zPupdates 
+00000d30: 7468 6520 6d6f 6465 6c20 616e 6420 636f  the model and co
+00000d40: 6d70 7574 6573 2074 6865 206d 6f64 656c  mputes the model
+00000d50: 2063 7572 7665 2077 6974 6820 7468 6520   curve with the 
+00000d60: 6375 7272 656e 7420 7061 7261 6d65 7465  current paramete
+00000d70: 7220 7661 6c75 6573 fa2a 4e6f 7420 6120  r values.*Not a 
+00000d80: 7661 6c69 6420 696e 7075 7420 696e 6974  valid input init
+00000d90: 6961 6c20 7061 7261 6d65 7465 7220 7661  ial parameter va
+00000da0: 6c75 6573 723e 0000 004e 4629 01da 0563  luesr>...NF)...c
+00000db0: 6865 636b 290f 722f 0000 00da 0b72 6561  heck).r/.....rea
+00000dc0: 645f 7661 6c75 6573 da0a 5661 6c75 6545  d_values..ValueE
+00000dd0: 7272 6f72 7246 0000 0072 3300 0000 da0d  rrorrF...r3.....
+00000de0: 7570 6461 7465 5f72 6570 6f72 7472 1900  update_reportr..
+00000df0: 0000 da06 6361 6e76 6173 da0b 7365 745f  ....canvas..set_
+00000e00: 6669 746c 696e 6572 1200 0000 5a09 6765  fitliner....Z.ge
+00000e10: 745f 6375 7276 65da 0d73 6574 5f72 6573  t_curve..set_res
+00000e20: 6964 7561 6c73 da0d 6765 745f 7265 7369  iduals..get_resi
+00000e30: 6475 616c 735a 1364 6973 6162 6c65 5f72  dualsZ.disable_r
+00000e40: 6573 756c 7473 5f62 6f78 721a 0000 0072  esults_boxr....r
+00000e50: 4900 0000 7221 0000 0072 2100 0000 7222  I...r!...r!...r"
+00000e60: 0000 0072 3200 0000 7f00 0000 731c 0000  ...r2.......s...
+00000e70: 0000 0302 010e 010c 0104 0104 ff04 0308  ................
+00000e80: 030c 0114 0108 010c ff04 030c 017a 134d  .............z.M
+00000e90: 6169 6e57 696e 646f 772e 6576 616c 7561  ainWindow.evalua
+00000ea0: 7465 6301 0000 0000 0000 0000 0000 0007  tec.............
+00000eb0: 0000 000b 0000 0003 0000 0073 c601 0000  ...........s....
+00000ec0: 7a0e 8800 6a00 a001 a100 0100 5700 6e20  z...j.......W.n 
+00000ed0: 0400 7402 792e 0100 0100 0100 8800 a003  ..t.y...........
+00000ee0: 6401 6402 a102 0100 5900 6403 5300 3000  d.d.....Y.d.S.0.
+00000ef0: 7404 8800 6a05 6a06 8301 0100 7a4a 7407  t...j.j.....zJt.
+00000f00: 8700 6601 6404 6405 8408 8800 6a05 6a08  ..f.d.d.....j.j.
+00000f10: 6a09 a00a a100 4400 8301 8301 7d01 7404  j.....D.....}.t.
+00000f20: 7c01 8301 0100 7c01 a00b a100 5c02 7d02  |.....|.....\.}.
+00000f30: 7d03 8800 6a0c a00d 7c02 7c03 6403 6403  }...j...|.|.d.d.
+00000f40: a104 0100 5700 6e18 0100 0100 0100 8800  ....W.n.........
+00000f50: a003 6406 6402 a102 0100 5900 6e02 3000  ..d.d.....Y.n.0.
+00000f60: 8800 6a05 6a08 a00e a100 0100 8800 6a0c  ..j.j.........j.
+00000f70: 6a0f 6a10 6403 7501 72d2 8800 6a11 72d2  j.j.d.u.r...j.r.
+00000f80: 8800 a003 6407 6408 a102 0100 6409 8800  ....d.d.....d...
+00000f90: 5f11 7412 a013 a100 8fd6 0100 7412 a014  _.t.........t...
+00000fa0: 640a 7415 a102 0100 7a14 8800 6a0c a016  d.t.....z...j...
+00000fb0: a100 5c03 7d04 7d05 7d06 5700 6e32 0400  ..\.}.}.}.W.n2..
+00000fc0: 7402 7417 7415 6603 9001 792e 0100 0100  t.t.t.f...y.....
+00000fd0: 0100 8800 a003 7418 7419 a01a a100 640b  ......t.t.....d.
+00000fe0: 1900 8301 6402 a102 0100 5900 6e74 3000  ....d.....Y.nt0.
+00000ff0: 8800 a01b 7c04 7c05 7c06 6603 a101 0100  ....|.|.|.f.....
+00001000: 8800 6a00 a01c a100 0100 8800 6a1d a01e  ..j.........j...
+00001010: 8800 6a0c a01f a100 a101 0100 8800 6a05  ..j...........j.
+00001020: 6a08 a020 8800 6a0c a021 a100 a101 0100  j.. ..j..!......
+00001030: 8800 6a05 6a08 a022 8800 6a0c a023 a100  ..j.j.."..j..#..
+00001040: a101 0100 8800 6a05 6a08 a024 8800 a025  ......j.j..$...%
+00001050: a100 640c a102 0100 8800 6a05 a026 a100  ..d.......j..&..
+00001060: 0100 5700 6403 0400 0400 8303 0100 6e12  ..W.d.........n.
+00001070: 3100 9001 73b8 3000 0100 0100 0100 5900  1...s.0.......Y.
+00001080: 0100 6403 5300 290d 7a4b 7570 6461 7465  ..d.S.).zKupdate
+00001090: 7320 7468 6520 6d6f 6465 6c20 7065 7266  s the model perf
+000010a0: 6f72 6d73 2074 6865 2066 6974 2061 6e64  orms the fit and
+000010b0: 2075 7064 6174 6573 2074 6865 2077 6964   updates the wid
+000010c0: 6765 7473 2077 6974 6820 7468 6520 7265  gets with the re
+000010d0: 7375 6c74 7372 4b00 0000 723e 0000 004e  sultsrK...r>...N
+000010e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000010f0: 0003 0000 0033 0000 0073 2200 0000 7c00  .....3...s"...|.
+00001100: 5d1a 7d01 7c01 a000 a100 8800 6a01 6a02  ].}.|.......j.j.
+00001110: 6b02 7202 7c01 5600 0100 7102 6400 5300  k.r.|.V...q.d.S.
+00001120: 2901 4e29 035a 0967 6574 5f6c 6162 656c  ).N).Z.get_label
+00001130: 7219 0000 00da 0e73 656c 6563 7465 645f  r......selected_
+00001140: 6375 7276 6529 02da 022e 30da 0178 7249  curve)....0..xrI
+00001150: 0000 0072 2100 0000 7222 0000 00da 093c  ...r!...r".....<
+00001160: 6765 6e65 7870 723e 9f00 0000 7306 0000  genexpr>....s...
+00001170: 0004 0202 0110 fe7a 214d 6169 6e57 696e  .......z!MainWin
+00001180: 646f 772e 6669 742e 3c6c 6f63 616c 733e  dow.fit.<locals>
+00001190: 2e3c 6765 6e65 7870 723e 7a0f 4361 6e27  .<genexpr>z.Can'
+000011a0: 7420 6669 6e64 2070 6c6f 747a 2554 6865  t find plotz%The
+000011b0: 2065 7272 6f72 2069 6e20 7820 6973 2069   error in x is i
+000011c0: 676e 6f72 6564 2069 6e20 7468 6520 6669  gnored in the fi
+000011d0: 7421 723f 0000 0046 da05 6572 726f 7272  t!r?...F..errorr
+000011e0: 0600 0000 e902 0000 0029 2772 2f00 0000  .........)'r/...
+000011f0: 724d 0000 0072 4e00 0000 7246 0000 00da  rM...rN...rF....
+00001200: 0570 7269 6e74 7219 0000 0072 5400 0000  .printr....rT...
+00001210: da04 6e65 7874 7250 0000 005a 0361 7831  ..nextrP...Z.ax1
+00001220: da09 6765 745f 6c69 6e65 73da 0867 6574  ..get_lines..get
+00001230: 5f64 6174 6172 1200 0000 5a0b 6368 616e  _datar....Z.chan
+00001240: 6765 5f64 6174 615a 0967 6574 5f72 616e  ge_dataZ.get_ran
+00001250: 6765 da04 6461 7461 5a02 7865 7216 0000  ge..dataZ.xer...
+00001260: 00da 0877 6172 6e69 6e67 73da 0e63 6174  ...warnings..cat
+00001270: 6368 5f77 6172 6e69 6e67 73da 0c73 696d  ch_warnings..sim
+00001280: 706c 6566 696c 7465 7272 0500 0000 7231  plefilterr....r1
+00001290: 0000 00da 0c52 756e 7469 6d65 4572 726f  .....RuntimeErro
+000012a0: 72da 0373 7472 da03 7379 73da 0865 7863  r..str..sys..exc
+000012b0: 5f69 6e66 6f72 4800 0000 5a0d 7570 6461  _inforH...Z.upda
+000012c0: 7465 5f76 616c 7565 7372 3300 0000 724f  te_valuesr3...rO
+000012d0: 0000 005a 0a67 6574 5f72 6570 6f72 7472  ...Z.get_reportr
+000012e0: 5100 0000 5a0c 6765 745f 6669 7463 7572  Q...Z.get_fitcur
+000012f0: 7665 7252 0000 0072 5300 0000 5a0f 7365  verR...rS...Z.se
+00001300: 745f 7265 7375 6c74 735f 626f 78da 145f  t_results_box.._
+00001310: 6765 745f 7265 7375 6c74 5f62 6f78 5f74  get_result_box_t
+00001320: 6578 7472 1a00 0000 2907 721d 0000 005a  extr....).r....Z
+00001330: 0d73 656c 6563 7465 645f 6c69 6e65 5a09  .selected_lineZ.
+00001340: 6375 7272 656e 745f 785a 0963 7572 7265  current_xZ.curre
+00001350: 6e74 5f79 da07 6669 7470 6172 735a 0666  nt_y..fitparsZ.f
+00001360: 6974 636f 76da 0672 6573 756c 7472 2100  itcov..resultr!.
+00001370: 0000 7249 0000 0072 2200 0000 7231 0000  ..rI...r"...r1..
+00001380: 0093 0000 0073 5000 0000 0003 0201 0e01  .....sP.........
+00001390: 0c01 0401 04ff 0403 0801 0c01 0201 0c02  ................
+000013a0: 0cfe 0805 0801 0c01 1602 0601 1202 0c03  ................
+000013b0: 1401 0c01 0603 0a01 0401 04ff 0404 0201  ................
+000013c0: 1401 1401 1e07 1003 0a01 1201 1401 0801  ................
+000013d0: 08ff 0403 0801 08ff 0403 7a0e 4d61 696e  ..........z.Main
+000013e0: 5769 6e64 6f77 2e66 6974 6301 0000 0000  Window.fitc.....
+000013f0: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
+00001400: 0000 0073 5c00 0000 6401 7d01 7c01 6402  ...s\...d.}.|.d.
+00001410: 1700 6403 1700 7c00 6a00 6a01 6a02 1700  ..d...|.j.j.j...
+00001420: 7d01 7c00 6a00 6a01 6a03 4400 5d32 7d02  }.|.j.j.j.D.]2}.
+00001430: 7c02 6a04 7d03 7c02 6a05 7d04 7c02 6a06  |.j.}.|.j.}.|.j.
+00001440: 7d05 7c02 6a07 7d06 7c01 6402 1700 7408  }.|.j.}.|.d...t.
+00001450: 7c03 7c04 7c05 7c06 8304 1700 7d01 7124  |.|.|.|.....}.q$
+00001460: 7c01 5300 2904 4e7a 0c46 6974 2072 6573  |.S.).Nz.Fit res
+00001470: 756c 7473 3ada 010a 7a07 7765 6967 6874  ults:...z.weight
+00001480: 3a29 0972 1200 0000 721b 0000 005a 0677  :).r....r....Z.w
+00001490: 6569 6768 7472 6700 0000 da04 6e61 6d65  eightrg.....name
+000014a0: da05 7661 6c75 65da 0573 6967 6d61 da05  ..value..sigma..
+000014b0: 6669 7865 6472 0900 0000 2907 721d 0000  fixedr....).r...
+000014c0: 00da 0474 6578 745a 0370 6172 da01 6eda  ...textZ.par..n.
+000014d0: 0176 da01 65da 0166 7221 0000 0072 2100  .v..e..fr!...r!.
+000014e0: 0000 7222 0000 0072 6600 0000 d000 0000  ..r"...rf.......
+000014f0: 7312 0000 0000 0104 0116 010e 0106 0106  s...............
+00001500: 0106 0106 0118 017a 1f4d 6169 6e57 696e  .......z.MainWin
+00001510: 646f 772e 5f67 6574 5f72 6573 756c 745f  dow._get_result_
+00001520: 626f 785f 7465 7874 6303 0000 0000 0000  box_textc.......
+00001530: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
+00001540: 0073 b400 0000 7c01 7c00 6a00 6a01 6a02  .s....|.|.j.j.j.
+00001550: 6b02 7316 7c01 6401 7500 722c 7c00 6a03  k.s.|.d.u.r,|.j.
+00001560: a004 7c00 6a00 6a01 6401 6401 a103 0100  ..|.j.j.d.d.....
+00001570: 6e10 7c00 6a03 a004 7c01 6401 6401 a103  n.|.j...|.d.d...
+00001580: 0100 7405 7c00 6a03 6a06 7c00 6a03 a007  ..t.|.j.j.|.j...
+00001590: a100 8302 7c00 5f08 7409 6402 740a 7c00  ....|._.t.d.t.|.
+000015a0: 6a03 8301 8302 0100 7c00 6a0b a00c 6403  j.......|.j...d.
+000015b0: a101 7d03 7c03 a00d a100 7284 7c03 a00d  ..}.|.....r.|...
+000015c0: a100 a00e 6401 a101 0100 7c00 6a08 7c00  ....d.....|.j.|.
+000015d0: 6a0f 7c00 6a10 7c00 6a11 6604 4400 5d10  j.|.j.|.j.f.D.].
+000015e0: 7d04 7c00 6a0b a012 7c04 a101 0100 7198  }.|.j...|.....q.
+000015f0: 7c00 6a13 0100 6401 5300 2904 7a91 0a20  |.j...d.S.).z.. 
+00001600: 2020 2020 2020 2072 6574 7269 6576 6573         retrieves
+00001610: 2064 6174 6120 6672 6f6d 2075 7064 6174   data from updat
+00001620: 6520 7369 676e 616c 2c20 706c 6f74 7769  e signal, plotwi
+00001630: 6467 6574 2e72 655f 696e 6974 2829 2c20  dget.re_init(), 
+00001640: 616e 6420 7570 6461 7465 7320 6775 6920  and updates gui 
+00001650: 6163 636f 7264 696e 6720 746f 2075 7365  according to use
+00001660: 7220 696e 7075 740a 2020 2020 2020 2020  r input.        
+00001670: 6361 6c6c 6564 2061 726f 756e 6420 6c69  called around li
+00001680: 6e65 2036 340a 0a20 2020 2020 2020 204e  ne 64..        N
+00001690: 722d 0000 0072 0100 0000 2914 721c 0000  r-...r....).r...
+000016a0: 00da 0466 756e 63da 085f 5f6e 616d 655f  ...func..__name_
+000016b0: 5f72 1200 0000 5a0c 6368 616e 6765 5f6d  _r....Z.change_m
+000016c0: 6f64 656c 720b 0000 0072 1b00 0000 722e  odelr....r....r.
+000016d0: 0000 0072 2f00 0000 725a 0000 00da 0269  ...r/...rZ.....i
+000016e0: 6472 3b00 0000 5a06 7461 6b65 4174 723c  dr;...Z.takeAtr<
+000016f0: 0000 005a 0973 6574 5061 7265 6e74 7236  ...Z.setParentr6
+00001700: 0000 0072 3300 0000 7235 0000 0072 3700  ...r3...r5...r7.
+00001710: 0000 7239 0000 0029 0572 1d00 0000 721b  ..r9...).r....r.
+00001720: 0000 00da 0179 da05 6368 696c 6472 3c00  .....y..childr<.
+00001730: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+00001740: 0072 2d00 0000 db00 0000 7322 0000 0000  .r-.......s"....
+00001750: 0616 0116 0210 0102 010e ff06 0310 060c  ................
+00001760: 0108 010e 0304 0104 0104 0104 fc08 060e  ................
+00001770: 027a 124d 6169 6e57 696e 646f 772e 7265  .z.MainWindow.re
+00001780: 6672 6573 6829 0272 3d00 0000 723d 0000  fresh).r=...r=..
+00001790: 0029 0f72 7400 0000 da0a 5f5f 6d6f 6475  .).rt.....__modu
+000017a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000017b0: 5f5f da07 5f5f 646f 635f 5f72 1100 0000  __..__doc__r....
+000017c0: 7226 0000 0072 1800 0000 7246 0000 0072  r&...r....rF...r
+000017d0: 4800 0000 724a 0000 0072 3200 0000 7231  H...rJ...r2...r1
+000017e0: 0000 0072 6600 0000 722d 0000 00da 0d5f  ...rf...r-....._
+000017f0: 5f63 6c61 7373 6365 6c6c 5f5f 7221 0000  _classcell__r!..
+00001800: 0072 2100 0000 721f 0000 0072 2200 0000  .r!...r....r"...
+00001810: 720e 0000 0011 0000 0073 1600 0000 0801  r........s......
+00001820: 0404 0c13 0804 083c 0a0e 0804 0804 0814  .......<........
+00001830: 083d 080b 720e 0000 0063 0a00 0000 0000  .=..r....c......
+00001840: 0000 0000 0000 1b00 0000 0a00 0000 0b00  ................
+00001850: 0000 73b4 0100 0074 006a 01a0 02a1 0073  ..s....t.j.....s
+00001860: 1674 00a0 0167 00a1 017d 0b6e 0a74 006a  .t...g...}.n.t.j
+00001870: 01a0 02a1 007d 0b64 0188 0076 0172 2c64  .....}.d...v.r,d
+00001880: 026e 0688 0064 0119 007d 0c64 0388 0076  .n...d...}.d...v
+00001890: 0172 4064 046e 0688 0064 0319 007d 0d7c  .r@d.n...d...}.|
+000018a0: 0d73 7474 037c 007c 017c 027c 037c 047c  .stt.|.|.|.|.|.|
+000018b0: 057c 087c 097c 0c66 0969 0088 00a4 018e  .|.|.|.f.i......
+000018c0: 017d 0e7c 0ea0 04a1 0053 0047 0087 0066  .}.|.....S.G...f
+000018d0: 0164 0564 0684 0864 0674 006a 0583 037d  .d.d...d.t.j...}
+000018e0: 0f7c 0f83 007d 107c 10a0 06a1 0001 007c  .|...}.|.......|
+000018f0: 0064 0775 0072 a67c 106a 077d 007c 0264  .d.u.r.|.j.}.|.d
+00001900: 0775 0090 0172 5674 087c 0083 017d 117c  .u...rVt.|...}.|
+00001910: 116a 097d 1274 0a7c 1283 017d 1364 0867  .j.}.t.|...}.d.g
+00001920: 017c 1314 007d 1474 0b74 0a7c 1483 0183  .|...}.t.t.|....
+00001930: 0144 005d 147d 1574 0ca0 0d64 0964 0aa1  .D.].}.t...d.d..
+00001940: 027c 147c 153c 0071 dc7c 007c 0167 017c  .|.|.<.q.|.|.g.|
+00001950: 1464 0b64 0785 0219 00a2 0152 008e 007d  .d.d.......R...}
+00001960: 1674 0e7c 1464 0b64 0785 0219 0083 0101  .t.|.d.d........
+00001970: 0074 0f6a 0ca0 10a1 007d 1764 0c74 0fa0  .t.j.....}.d.t..
+00001980: 117c 01a1 0114 007d 187c 187c 176a 127c  .|.....}.|.|.j.|
+00001990: 016a 1364 0d8d 0114 007d 197c 167c 1917  .j.d.....}.|.|..
+000019a0: 007d 0274 0fa0 147c 02a1 017d 027c 106a  .}.t...|...}.|.j
+000019b0: 1590 0172 6664 0488 0064 013c 0074 037c  ...rfd...d.<.t.|
+000019c0: 007c 017c 027c 037c 047c 057c 087c 097c  .|.|.|.|.|.|.|.|
+000019d0: 106a 1566 0969 0088 00a4 018e 017d 0e74  .j.f.i.......}.t
+000019e0: 167c 0e7c 067c 0766 0369 0088 00a4 018e  .|.|.|.f.i......
+000019f0: 017d 1a7c 1aa0 17a1 0001 007c 0ba0 06a1  .}.|.......|....
+00001a00: 0001 007c 1aa0 18a1 0053 0029 0e7a 540a  ...|.....S.).zT.
+00001a10: 2020 2020 6865 6c70 6572 2066 756e 6374      helper funct
+00001a20: 696f 6e20 7468 6174 2065 7865 6375 7465  ion that execute
+00001a30: 7320 7468 6520 4755 4920 7769 7468 2061  s the GUI with a
+00001a40: 6e20 696e 7374 616e 6365 206f 6620 7468  n instance of th
+00001a50: 6520 6669 7474 6572 2063 6c61 7373 0a20  e fitter class. 
+00001a60: 2020 20da 0763 6f6d 706c 6578 46da 0773     ..complexF..s
+00001a70: 686f 7767 7569 5463 0000 0000 0000 0000  howguiTc........
+00001a80: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00001a90: 732a 0000 0065 005a 0164 005a 0264 015a  s*...e.Z.d.Z.d.Z
+00001aa0: 0387 0087 0166 0264 0264 0384 085a 0464  .....f.d.d...Z.d
+00001ab0: 0464 0584 005a 0587 0004 005a 0653 0029  .d...Z.....Z.S.)
+00001ac0: 067a 2165 7865 6375 7465 5f67 7569 2e3c  .z!execute_gui.<
+00001ad0: 6c6f 6361 6c73 3e2e 4375 7374 6f6d 4469  locals>.CustomDi
+00001ae0: 616c 6f67 7a4c 0a20 2020 2020 2020 2063  alogzL.        c
+00001af0: 686f 6f73 6520 6669 742c 2073 7461 7274  hoose fit, start
+00001b00: 696e 6720 6469 616c 6f67 2074 6861 7420  ing dialog that 
+00001b10: 616c 6c6f 7773 2075 7365 7220 746f 2063  allows user to c
+00001b20: 686f 6f73 6520 6669 740a 2020 2020 2020  hoose fit.      
+00001b30: 2020 6301 0000 0000 0000 0000 0000 000a    c.............
+00001b40: 0000 0008 0000 0013 0000 0073 1201 0000  ...........s....
+00001b50: 7400 8300 a001 a100 0100 6401 8801 7601  t.........d...v.
+00001b60: 7216 6402 6e06 8801 6401 1900 7c00 5f02  r.d.n...d...|._.
+00001b70: 6403 6404 8400 7d01 6405 6406 8400 7d02  d.d...}.d.d...}.
+00001b80: 6407 6408 8400 7d03 6409 640a 8400 7d04  d.d...}.d.d...}.
+00001b90: 640b 640c 8400 7d05 640d 640e 8400 7d06  d.d...}.d.d...}.
+00001ba0: 640f 6410 8400 7d07 7c01 7c02 7c03 7c04  d.d...}.|.|.|.|.
+00001bb0: 7c05 7c06 7c07 6411 9c07 7c00 5f03 7c00  |.|.|.d...|._.|.
+00001bc0: a004 6412 a101 0100 7405 a006 6413 a101  ..d.....t...d...
+00001bd0: 7c00 5f07 7405 a008 a100 7c00 5f09 7405  |._.t.....|._.t.
+00001be0: a00a 6414 a101 7d08 7405 a00b a100 7c00  ..d...}.t.....|.
+00001bf0: 5f0c 7c00 6a03 4400 5d10 7d09 7c00 6a0c  _.|.j.D.].}.|.j.
+00001c00: a00d 7c09 a101 0100 71a8 7c00 6a09 a00e  ..|.....q.|.j...
+00001c10: 7c08 a101 0100 7c00 6a09 a00e 7c00 6a0c  |.....|.j...|.j.
+00001c20: a101 0100 7c00 6a09 a00e 7c00 6a07 a101  ....|.j...|.j...
+00001c30: 0100 7c00 6a07 6a0f a010 7c00 6a11 a101  ..|.j.j...|.j...
+00001c40: 0100 7c00 6a07 6a0f a010 7c00 6a12 a101  ..|.j.j...|.j...
+00001c50: 0100 7c00 a013 7c00 6a09 a101 0100 6400  ..|...|.j.....d.
+00001c60: 5300 2915 4e72 7c00 0000 4663 0300 0000  S.).Nr|...Fc....
+00001c70: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+00001c80: 5300 0000 730c 0000 007c 017c 0014 007c  S...s....|.|...|
+00001c90: 0217 0053 0029 017a 490a 2020 2020 2020  ...S.).zI.      
+00001ca0: 2020 2020 2020 2020 2020 6c69 6e65 6172            linear
+00001cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001cc0: 2066 756e 6374 696f 6e3a 2061 7820 2b20   function: ax + 
+00001cd0: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
+00001ce0: 2020 7221 0000 0029 0372 5600 0000 da01    r!...).rV.....
+00001cf0: 61da 0162 7221 0000 0072 2100 0000 7222  a..br!...r!...r"
+00001d00: 0000 00da 066c 696e 6561 7233 0100 0073  .....linear3...s
+00001d10: 0200 0000 0006 7a3a 6578 6563 7574 655f  ......z:execute_
+00001d20: 6775 692e 3c6c 6f63 616c 733e 2e43 7573  gui.<locals>.Cus
+00001d30: 746f 6d44 6961 6c6f 672e 5f5f 696e 6974  tomDialog.__init
+00001d40: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6c69 6e65  __.<locals>.line
+00001d50: 6172 6304 0000 0000 0000 0000 0000 0004  arc.............
+00001d60: 0000 0005 0000 0053 0000 0073 1800 0000  .......S...s....
+00001d70: 7c01 7400 a001 7c00 0b00 7c02 1b00 a101  |.t...|...|.....
+00001d80: 1400 7c03 1700 5300 2901 7ab3 0a20 2020  ..|...S.).z..   
+00001d90: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00001da0: 6f6e 656e 7469 616c 2064 6563 6179 0a20  onential decay. 
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001dc0: 756e 6374 696f 6e3a 2061 202a 2065 7870  unction: a * exp
+00001dd0: 282d 7820 2f20 6229 202b 2063 0a20 2020  (-x / b) + c.   
+00001de0: 2020 2020 2020 2020 2020 2020 2061 203a               a :
+00001df0: 2061 6d70 6c69 7475 6465 0a20 2020 2020   amplitude.     
+00001e00: 2020 2020 2020 2020 2020 2062 203a 2072             b : r
+00001e10: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+00001e20: 2020 2020 6320 3a20 6f66 6673 6574 0a20      c : offset. 
+00001e30: 2020 2020 2020 2020 2020 2020 2020 20a9                 .
+00001e40: 02da 026e 70da 0365 7870 2904 7256 0000  ...np..exp).rV..
+00001e50: 0072 7e00 0000 727f 0000 00da 0163 7221  .r~...r......cr!
+00001e60: 0000 0072 2100 0000 7222 0000 00da 0965  ...r!...r".....e
+00001e70: 7870 5f64 6563 6179 3b01 0000 7302 0000  xp_decay;...s...
+00001e80: 0000 087a 3d65 7865 6375 7465 5f67 7569  ...z=execute_gui
+00001e90: 2e3c 6c6f 6361 6c73 3e2e 4375 7374 6f6d  .<locals>.Custom
+00001ea0: 4469 616c 6f67 2e5f 5f69 6e69 745f 5f2e  Dialog.__init__.
+00001eb0: 3c6c 6f63 616c 733e 2e65 7870 5f64 6563  <locals>.exp_dec
+00001ec0: 6179 6305 0000 0000 0000 0000 0000 0005  ayc.............
+00001ed0: 0000 0005 0000 0053 0000 0073 1a00 0000  .......S...s....
+00001ee0: 7c01 7400 a001 7c02 7c00 1400 7c03 1700  |.t...|.|...|...
+00001ef0: a101 1400 7c04 1700 5300 2901 7a3c 0a20  ....|...S.).z<. 
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00001f10: 203d 2061 202a 2063 6f73 2862 202a 2078   = a * cos(b * x
+00001f20: 202b 2063 2920 2b20 640a 2020 2020 2020   + c) + d.      
+00001f30: 2020 2020 2020 2020 2020 2902 7282 0000            ).r...
+00001f40: 00da 0363 6f73 a905 7256 0000 0072 7e00  ...cos..rV...r~.
+00001f50: 0000 727f 0000 0072 8400 0000 da01 6472  ..r....r......dr
+00001f60: 2100 0000 7221 0000 0072 2200 0000 da0f  !...r!...r".....
+00001f70: 636f 7369 6e65 5f66 756e 6374 696f 6e45  cosine_functionE
+00001f80: 0100 0073 0200 0000 0004 7a43 6578 6563  ...s......zCexec
+00001f90: 7574 655f 6775 692e 3c6c 6f63 616c 733e  ute_gui.<locals>
+00001fa0: 2e43 7573 746f 6d44 6961 6c6f 672e 5f5f  .CustomDialog.__
+00001fb0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00001fc0: 636f 7369 6e65 5f66 756e 6374 696f 6e63  cosine_functionc
+00001fd0: 0600 0000 0000 0000 0000 0000 0600 0000  ................
+00001fe0: 0500 0000 5300 0000 732a 0000 007c 0174  ....S...s*...|.t
+00001ff0: 00a0 017c 000b 007c 021b 00a1 0114 0074  ...|...|.......t
+00002000: 00a0 027c 037c 0014 007c 0417 00a1 0114  ...|.|...|......
+00002010: 007c 0517 0053 0029 017a 4a0a 2020 2020  .|...S.).zJ.    
+00002020: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+00002030: 6120 2a20 6578 7028 2d78 202f 2062 2920  a * exp(-x / b) 
+00002040: 2a20 636f 7328 6320 2a20 7820 2b20 6429  * cos(c * x + d)
+00002050: 202b 2065 0a20 2020 2020 2020 2020 2020   + e.           
+00002060: 2020 2020 20a9 0372 8200 0000 7283 0000       ..r....r...
+00002070: 0072 8600 0000 a906 7256 0000 0072 7e00  .r......rV...r~.
+00002080: 0000 727f 0000 0072 8400 0000 7288 0000  ..r....r....r...
+00002090: 0072 7100 0000 7221 0000 0072 2100 0000  .rq...r!...r!...
+000020a0: 7222 0000 00da 1464 6563 6179 696e 675f  r".....decaying_
+000020b0: 6f73 6369 6c6c 6174 696f 6e4b 0100 0073  oscillationK...s
+000020c0: 0200 0000 0004 7a48 6578 6563 7574 655f  ......zHexecute_
+000020d0: 6775 692e 3c6c 6f63 616c 733e 2e43 7573  gui.<locals>.Cus
+000020e0: 746f 6d44 6961 6c6f 672e 5f5f 696e 6974  tomDialog.__init
+000020f0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6465 6361  __.<locals>.deca
+00002100: 7969 6e67 5f6f 7363 696c 6c61 7469 6f6e  ying_oscillation
+00002110: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
+00002120: 0005 0000 0053 0000 0073 2e00 0000 7c01  .....S...s....|.
+00002130: 7400 a001 7c00 0b00 7c02 1b00 a101 6401  t...|...|.....d.
+00002140: 1300 1400 7400 a002 7c03 7c00 1400 7c04  ....t...|.|...|.
+00002150: 1700 a101 1400 7c05 1700 5300 2902 7a4c  ......|...S.).zL
+00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002170: 2079 203d 2061 202a 2065 7870 282d 7820   y = a * exp(-x 
+00002180: 2f20 6229 5e32 202a 2063 6f73 2863 202a  / b)^2 * cos(c *
+00002190: 2078 202b 2064 2920 2b20 650a 2020 2020   x + d) + e.    
+000021a0: 2020 2020 2020 2020 2020 2020 7259 0000              rY..
+000021b0: 0072 8a00 0000 728b 0000 0072 2100 0000  .r....r....r!...
+000021c0: 7221 0000 0072 2200 0000 da15 6465 6361  r!...r".....deca
+000021d0: 7969 6e67 5f6f 7363 696c 6c61 7469 6f6e  ying_oscillation
+000021e0: 3251 0100 0073 0200 0000 0004 7a49 6578  2Q...s......zIex
+000021f0: 6563 7574 655f 6775 692e 3c6c 6f63 616c  ecute_gui.<local
+00002200: 733e 2e43 7573 746f 6d44 6961 6c6f 672e  s>.CustomDialog.
+00002210: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00002220: 3e2e 6465 6361 7969 6e67 5f6f 7363 696c  >.decaying_oscil
+00002230: 6c61 7469 6f6e 3263 0200 0000 0000 0000  lation2c........
+00002240: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00002250: 7312 0000 007c 0174 00a0 0164 017c 0014  s....|.t...d.|..
+00002260: 00a1 0114 0053 0029 027a 4c0a 2020 2020  .....S.).zL.    
+00002270: 2020 2020 2020 2020 2020 2020 4575 6c65              Eule
+00002280: 7227 730a 2020 2020 2020 2020 2020 2020  r's.            
+00002290: 2020 2020 7920 3d20 6120 2a20 6578 7028      y = a * exp(
+000022a0: 6920 2a20 7829 0a20 2020 2020 2020 2020  i * x).         
+000022b0: 2020 2020 2020 20f9 0000 0000 0000 0000         .........
+000022c0: 0000 0000 0000 f03f 7281 0000 0029 0272  .......?r....).r
+000022d0: 5600 0000 727e 0000 0072 2100 0000 7221  V...r~...r!...r!
+000022e0: 0000 0072 2200 0000 da05 6575 6c65 7257  ...r".....eulerW
+000022f0: 0100 0073 0200 0000 0005 7a39 6578 6563  ...s......z9exec
+00002300: 7574 655f 6775 692e 3c6c 6f63 616c 733e  ute_gui.<locals>
+00002310: 2e43 7573 746f 6d44 6961 6c6f 672e 5f5f  .CustomDialog.__
+00002320: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00002330: 6575 6c65 7263 0500 0000 0000 0000 0000  eulerc..........
+00002340: 0000 0500 0000 0600 0000 5300 0000 731e  ..........S...s.
+00002350: 0000 007c 0174 00a0 0164 017c 027c 0014  ...|.t...d.|.|..
+00002360: 007c 0317 0014 00a1 0114 007c 0417 0053  .|.........|...S
+00002370: 0029 027a 5e0a 2020 2020 2020 2020 2020  .).z^.          
+00002380: 2020 2020 2020 636f 6d70 6c65 7820 6578        complex ex
+00002390: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+000023a0: 2020 7920 3d20 6120 2a20 6578 7028 6920    y = a * exp(i 
+000023b0: 2a20 2862 202a 2077 202b 2063 2929 202b  * (b * w + c)) +
+000023c0: 2064 0a20 2020 2020 2020 2020 2020 2020   d.             
+000023d0: 2020 2072 8e00 0000 7281 0000 0072 8700     r....r....r..
+000023e0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+000023f0: 00da 1063 6f6d 706c 6578 5f66 756e 6374  ...complex_funct
+00002400: 696f 6e5e 0100 0073 0200 0000 0005 7a44  ion^...s......zD
+00002410: 6578 6563 7574 655f 6775 692e 3c6c 6f63  execute_gui.<loc
+00002420: 616c 733e 2e43 7573 746f 6d44 6961 6c6f  als>.CustomDialo
+00002430: 672e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  g.__init__.<loca
+00002440: 6c73 3e2e 636f 6d70 6c65 785f 6675 6e63  ls>.complex_func
+00002450: 7469 6f6e 2907 7a0a 7920 3d20 6178 202b  tion).z.y = ax +
+00002460: 2062 7a17 7920 3d20 6120 2a20 6578 7028   bz.y = a * exp(
+00002470: 2d78 202f 2062 2920 2b20 637a 1879 203d  -x / b) + cz.y =
+00002480: 2061 202a 2063 6f73 2862 2a78 202b 2063   a * cos(b*x + c
+00002490: 2920 2b20 647a 2879 203d 2061 202a 2065  ) + dz(y = a * e
+000024a0: 7870 282d 7820 2f20 6229 202a 2063 6f73  xp(-x / b) * cos
+000024b0: 2863 202a 2078 202b 2064 2920 2b20 657a  (c * x + d) + ez
+000024c0: 2a79 203d 2061 202a 2065 7870 282d 7820  *y = a * exp(-x 
+000024d0: 2f20 6229 5e32 202a 2063 6f73 2863 202a  / b)^2 * cos(c *
+000024e0: 2078 202b 2064 2920 2b20 657a 1279 203d   x + d) + ez.y =
+000024f0: 2061 202a 2065 7870 2869 202a 2078 297a   a * exp(i * x)z
+00002500: 2079 203d 2061 202a 2065 7870 2869 202a   y = a * exp(i *
+00002510: 2028 6220 2a20 7720 2b20 6329 2920 2b20   (b * w + c)) + 
+00002520: 647a 0a43 686f 6f73 6520 4669 745a 0553  dz.Choose FitZ.S
+00002530: 7461 7274 7a0c 4368 6f6f 7365 2043 7572  tartz.Choose Cur
+00002540: 7665 2914 7210 0000 0072 1100 0000 da0a  ve).r....r......
+00002550: 6973 5f63 6f6d 706c 6578 da0c 6675 6e63  is_complex..func
+00002560: 7469 6f6e 5f6d 6170 7229 0000 0072 0400  tion_mapr)...r..
+00002570: 0000 7230 0000 005a 0662 7574 746f 6e72  ..r0...Z.buttonr
+00002580: 3a00 0000 5a0d 6469 616c 6f67 5f6c 6179  :...Z.dialog_lay
+00002590: 6f75 745a 0651 4c61 6265 6c5a 0951 436f  outZ.QLabelZ.QCo
+000025a0: 6d62 6f42 6f78 da08 636f 6d62 6f62 6f78  mboBox..combobox
+000025b0: 5a07 6164 6449 7465 6d72 3700 0000 7228  Z.addItemr7...r(
+000025c0: 0000 0072 2c00 0000 da08 6765 745f 7465  ...r,.....get_te
+000025d0: 7874 7234 0000 0072 3800 0000 290a 721d  xtr4...r8...).r.
+000025e0: 0000 0072 8000 0000 7285 0000 0072 8900  ...r....r....r..
+000025f0: 0000 728c 0000 0072 8d00 0000 728f 0000  ..r....r....r...
+00002600: 0072 9000 0000 7242 0000 00da 0469 7465  .r....rB.....ite
+00002610: 6d29 0272 2000 0000 7217 0000 0072 2100  m).r ...r....r!.
+00002620: 0000 7222 0000 0072 1100 0000 2c01 0000  ..r"...r....,...
+00002630: 733e 0000 0000 010a 0312 ff04 0408 0808  s>..............
+00002640: 0a08 0608 0608 0608 0708 0802 0102 0102  ................
+00002650: 0102 0102 0102 0102 f908 0d0a 010c 010a  ................
+00002660: 010a 020a 020a 010e 050c 010e 010e 0110  ................
+00002670: 0110 027a 2a65 7865 6375 7465 5f67 7569  ...z*execute_gui
+00002680: 2e3c 6c6f 6361 6c73 3e2e 4375 7374 6f6d  .<locals>.Custom
+00002690: 4469 616c 6f67 2e5f 5f69 6e69 745f 5f63  Dialog.__init__c
+000026a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000026b0: 0300 0000 5300 0000 7330 0000 0064 017c  ....S...s0...d.|
+000026c0: 006a 00a0 01a1 0076 0072 1264 026e 047c  .j.....v.r.d.n.|
+000026d0: 006a 027c 005f 027c 006a 037c 006a 00a0  .j.|._.|.j.|.j..
+000026e0: 01a1 0019 007c 005f 0464 0353 0029 047a  .....|._.d.S.).z
+000026f0: 580a 2020 2020 2020 2020 2020 2020 4f6e  X.            On
+00002700: 206f 6b20 6672 6f6d 2073 7461 7274 696e   ok from startin
+00002710: 6720 706f 7020 7570 2074 6869 7320 6675  g pop up this fu
+00002720: 6e63 7469 6f6e 2073 6574 7320 7468 6520  nction sets the 
+00002730: 6669 7420 6675 6e63 7469 6f6e 0a20 2020  fit function.   
+00002740: 2020 2020 2020 2020 20da 0169 544e 2905           ..iTN).
+00002750: 7293 0000 005a 0b63 7572 7265 6e74 5465  r....Z.currentTe
+00002760: 7874 7291 0000 0072 9200 0000 7273 0000  xtr....r....rs..
+00002770: 0072 4900 0000 7221 0000 0072 2100 0000  .rI...r!...r!...
+00002780: 7222 0000 0072 9400 0000 8701 0000 7306  r"...r........s.
+00002790: 0000 0000 0516 ff04 037a 2a65 7865 6375  .........z*execu
+000027a0: 7465 5f67 7569 2e3c 6c6f 6361 6c73 3e2e  te_gui.<locals>.
+000027b0: 4375 7374 6f6d 4469 616c 6f67 2e67 6574  CustomDialog.get
+000027c0: 5f74 6578 7429 0772 7400 0000 7278 0000  _text).rt...rx..
+000027d0: 0072 7900 0000 727a 0000 0072 1100 0000  .ry...rz...r....
+000027e0: 7294 0000 0072 7b00 0000 7221 0000 00a9  r....r{...r!....
+000027f0: 0172 1700 0000 721f 0000 0072 2200 0000  .r....r....r"...
+00002800: da0c 4375 7374 6f6d 4469 616c 6f67 2701  ..CustomDialog'.
+00002810: 0000 7306 0000 0008 0104 040e 5b72 9800  ..s.........[r..
+00002820: 0000 4e72 0100 0000 6700 0000 0000 00e0  ..Nr....g.......
+00002830: 3fe9 0400 0000 7206 0000 0067 9a99 9999  ?.....r....g....
+00002840: 9999 c93f 2901 da04 7369 7a65 2919 7204  ...?)...size).r.
+00002850: 0000 0072 2300 0000 da08 696e 7374 616e  ...r#.....instan
+00002860: 6365 7208 0000 0072 3100 0000 5a07 5144  cer....r1...Z.QD
+00002870: 6961 6c6f 6772 4100 0000 7273 0000 0072  ialogrA...rs...r
+00002880: 0200 0000 da0a 7061 7261 6d65 7465 7273  ......parameters
+00002890: da03 6c65 6eda 0572 616e 6765 da06 7261  ..len..range..ra
+000028a0: 6e64 6f6d da07 756e 6966 6f72 6d72 5a00  ndom..uniformrZ.
+000028b0: 0000 7282 0000 00da 0b64 6566 6175 6c74  ..r......default
+000028c0: 5f72 6e67 da09 6f6e 6573 5f6c 696b 65da  _rng..ones_like.
+000028d0: 066e 6f72 6d61 6c72 9a00 0000 da07 6173  .normalr......as
+000028e0: 6172 7261 7972 9100 0000 720e 0000 00da  arrayr....r.....
+000028f0: 0473 686f 7772 4a00 0000 291b 7272 0000  .showrJ...).rr..
+00002900: 00da 0578 6461 7461 da05 7964 6174 61da  ...xdata..ydata.
+00002910: 0478 6572 72da 0479 6572 72da 0270 3072  .xerr..yerr..p0r
+00002920: 1300 0000 7214 0000 00da 0e61 6273 6f6c  ....r......absol
+00002930: 7574 655f 7369 676d 61da 036a 6163 7217  ute_sigma..jacr.
+00002940: 0000 005a 0361 7070 7291 0000 0072 7d00  ...Z.appr....r}.
+00002950: 0000 721e 0000 0072 9800 0000 5a03 646c  ..r....r....Z.dl
+00002960: 67da 0373 6967 da06 7061 7261 6d73 5a0d  g..sig..paramsZ.
+00002970: 6e75 6d5f 6f66 5f70 6172 616d 735a 0a72  num_of_paramsZ.r
+00002980: 616e 646f 6d5f 6172 7272 9600 0000 7276  andom_arrr....rv
+00002990: 0000 00da 0372 6e67 5a09 7465 7374 5f79  .....rngZ.test_y
+000029a0: 6572 72da 0779 5f6e 6f69 7365 5a0d 4d79  err..y_noiseZ.My
+000029b0: 4170 706c 6963 6174 696f 6e72 2100 0000  Applicationr!...
+000029c0: 7297 0000 0072 2200 0000 da0b 6578 6563  r....r".....exec
+000029d0: 7574 655f 6775 69fe 0000 0073 7400 0000  ute_gui....st...
+000029e0: 0011 0a01 0c02 0a02 1402 1402 0401 0201  ................
+000029f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00002a00: 02f7 040a 02f6 060c 0802 1669 0601 0801  ...........i....
+00002a10: 0801 060f 0a01 0801 0601 0801 0a01 1001  ................
+00002a20: 1205 1801 1005 0a01 0e01 1201 0801 0a06  ................
+00002a30: 0801 0802 0201 0201 0201 0201 0201 0201  ................
+00002a40: 0201 0201 0201 04f7 040a 02f6 060e 1401  ................
+00002a50: 0801 0801 72b1 0000 0029 1b72 9f00 0000  ....r....).r....
+00002a60: 7264 0000 0072 5f00 0000 da07 696e 7370  rd...r_.....insp
+00002a70: 6563 7472 0200 0000 da05 6e75 6d70 7972  ectr......numpyr
+00002a80: 8200 0000 5a05 5079 5174 3572 0300 0000  ....Z.PyQt5r....
+00002a90: 7204 0000 005a 0e73 6369 7079 2e6f 7074  r....Z.scipy.opt
+00002aa0: 696d 697a 6572 0500 0000 da09 5f73 6574  imizer......_set
+00002ab0: 7469 6e67 7372 0700 0000 5a06 5f74 6f6f  tingsr....Z._too
+00002ac0: 6c73 7208 0000 0072 0900 0000 da08 5f76  lsr....r......_v
+00002ad0: 6572 7369 6f6e 720a 0000 0072 2a00 0000  ersionr....r*...
+00002ae0: 5a08 5f77 6964 6765 7473 720b 0000 0072  Z._widgetsr....r
+00002af0: 0c00 0000 720d 0000 005a 0b51 4d61 696e  ....r....Z.QMain
+00002b00: 5769 6e64 6f77 720e 0000 0072 b100 0000  Windowr....r....
+00002b10: 7221 0000 0072 2100 0000 7221 0000 0072  r!...r!...r!...r
+00002b20: 2200 0000 da08 3c6d 6f64 756c 653e 0200  ".....<module>..
+00002b30: 0000 731a 0000 0008 0108 0108 010c 0208  ..s.............
+00002b40: 0110 010c 020c 0110 010c 0114 0312 7f00  ................
+00002b50: 6e                                       n
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_settings.cpython-311.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_settings.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_tools.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_tools.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Feb 24 17:24:25 2023 UTC, .py size: 16626 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,871 +1,883 @@
-00000000: 610d 0d0a 0000 0000 c9f2 f863 f240 0000  a..........c.@..
+00000000: 610d 0d0a 0000 0000 a847 4364 c640 0000  a........GCd.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 0100 6400 6401 6c07 5a08 6400  m.Z...d.d.l.Z.d.
-00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 6d0f 5a0f 0100 6407 6408 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
-00000090: 0100 6502 4700 6409 640a 8400 640a 8302  ..e.G.d.d...d...
-000000a0: 8301 5a12 6502 4700 640b 640c 8400 640c  ..Z.e.G.d.d...d.
-000000b0: 8302 8301 5a13 6502 4700 640d 640e 8400  ....Z.e.G.d.d...
-000000c0: 640e 8302 8301 5a14 4700 640f 6410 8400  d.....Z.G.d.d...
-000000d0: 6410 8302 5a15 6401 6401 6401 6411 6412  d...Z.d.d.d.d.d.
-000000e0: 9c04 6413 6414 8402 5a16 6415 6416 8400  ..d.d...Z.d.d...
-000000f0: 5a17 6417 6418 8400 5a18 6419 641a 8400  Z.d.d...Z.d.d...
-00000100: 5a19 6401 5300 291b e900 0000 004e 2902  Z.d.S.)......N).
-00000110: da09 6461 7461 636c 6173 73da 0566 6965  ..dataclass..fie
-00000120: 6c64 2902 da03 416e 79da 044c 6973 7429  ld)...Any..List)
-00000130: 01da 054d 6f64 656c 2901 da05 7374 6174  ...Model)...stat
-00000140: 7329 02da 0f4f 7074 696d 697a 6557 6172  s)...OptimizeWar
-00000150: 6e69 6e67 da09 6375 7276 655f 6669 74e9  ning..curve_fit.
-00000160: 0100 0000 a901 da08 7365 7474 696e 6773  ........settings
-00000170: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000180: 0003 0000 0040 0000 0073 3e00 0000 6500  .....@...s>...e.
-00000190: 5a01 6400 5a02 5500 6401 5a03 6504 6505  Z.d.Z.U.d.Z.e.e.
-000001a0: 6402 3c00 6403 5a06 6507 6505 6404 3c00  d.<.d.Z.e.e.d.<.
-000001b0: 6405 5a08 6507 6505 6406 3c00 6407 5a09  d.Z.e.e.d.<.d.Z.
-000001c0: 650a 6505 6408 3c00 6409 5300 290a da0c  e.e.d.<.d.S.)...
-000001d0: 4669 7450 6172 616d 6574 6572 7a1f 0a20  FitParameterz.. 
-000001e0: 2020 2073 746f 7265 7320 6120 6669 7470     stores a fitp
-000001f0: 6172 616d 6574 6572 0a20 2020 20da 046e  arameter.    ..n
-00000200: 616d 65e7 0000 0000 0000 f03f da05 7661  ame........?..va
-00000210: 6c75 6567 0000 0000 0000 0000 da05 7369  lueg..........si
-00000220: 676d 6146 da05 6669 7865 644e 290b da08  gmaF..fixedN)...
-00000230: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000240: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000250: 5f5f da07 5f5f 646f 635f 5fda 0373 7472  __..__doc__..str
-00000260: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00000270: 5f72 1000 0000 da05 666c 6f61 7472 1100  _r......floatr..
-00000280: 0000 7212 0000 00da 0462 6f6f 6ca9 0072  ..r......bool..r
-00000290: 1b00 0000 721b 0000 00fa 392f 5573 6572  ....r.....9/User
-000002a0: 732f 6b6f 6a6f 2f61 7070 732f 7365 6e69  s/kojo/apps/seni
-000002b0: 6f72 5f70 726f 6a65 6374 5f75 7363 2f63  or_project_usc/c
-000002c0: 7572 7665 6669 7467 7569 2f5f 746f 6f6c  urvefitgui/_tool
-000002d0: 732e 7079 720d 0000 000d 0000 0073 0a00  s.pyr........s..
-000002e0: 0000 0a02 0404 0801 0c01 0c01 720d 0000  ............r...
-000002f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000300: 0000 0300 0000 4000 0000 7368 0000 0065  ......@...sh...e
-00000310: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
-00000320: 0564 023c 0065 0465 0564 033c 0065 0665  .d.<.e.e.d.<.e.e
-00000330: 0564 043c 0065 0765 0819 0065 0564 053c  .d.<.e.e...e.d.<
-00000340: 0064 065a 0965 0665 0564 073c 0064 0864  .d.Z.e.e.d.<.d.d
-00000350: 099c 0164 0a64 0b84 045a 0a64 0c64 0d84  ...d.d...Z.d.d..
-00000360: 005a 0b64 0e64 0f84 005a 0c64 1064 1184  .Z.d.d...Z.d.d..
-00000370: 005a 0d64 0853 0029 12da 0846 6974 4d6f  .Z.d.S.)...FitMo
-00000380: 6465 6c7a 1a0a 2020 2020 7374 6f72 6573  delz..    stores
-00000390: 2074 6865 206d 6f64 656c 0a20 2020 20da   the model.    .
-000003a0: 0466 756e 63da 036a 6163 da06 7765 6967  .func..jac..weig
-000003b0: 6874 da07 6669 7470 6172 73da 00da 0b64  ht..fitpars....d
-000003c0: 6573 6372 6970 7469 6f6e 4e29 01da 0672  escriptionN)...r
-000003d0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-000003e0: 0000 0200 0000 0400 0000 4300 0000 734a  ..........C...sJ
-000003f0: 0000 0074 007c 006a 0183 017c 005f 027c  ...t.|.j...|._.|
-00000400: 006a 02a0 03a1 007c 005f 047c 006a 0544  .j.....|._.|.j.D
-00000410: 005d 267d 017c 016a 060c 007c 006a 047c  .]&}.|.j...|.j.|
-00000420: 016a 0719 005f 087c 016a 097c 006a 047c  .j..._.|.j.|.j.|
-00000430: 016a 0719 005f 0971 1e64 0153 0029 027a  .j..._.q.d.S.).z
-00000440: 3a0a 2020 2020 2020 2020 496e 6974 6961  :.        Initia
-00000450: 6c69 7a65 7320 6c6d 6669 7420 6d6f 6465  lizes lmfit mode
-00000460: 6c20 616e 6420 7061 7261 7265 6d65 7465  l and pararemete
-00000470: 7273 0a20 2020 2020 2020 204e 290a 7206  rs.        N).r.
-00000480: 0000 0072 1e00 0000 da0b 6c6d 6669 745f  ...r......lmfit_
-00000490: 6d6f 6465 6c5a 0b6d 616b 655f 7061 7261  modelZ.make_para
-000004a0: 6d73 da0a 7061 7261 6d65 7465 7273 7221  ms..parametersr!
-000004b0: 0000 0072 1200 0000 720e 0000 00da 0476  ...r....r......v
-000004c0: 6172 7972 1000 0000 a902 da04 7365 6c66  aryr........self
-000004d0: da03 7061 7272 1b00 0000 721b 0000 0072  ..parr....r....r
-000004e0: 1c00 0000 da0d 5f5f 706f 7374 5f69 6e69  ......__post_ini
-000004f0: 745f 5f27 0000 0073 0a00 0000 0004 0c06  t__'...s........
-00000500: 0c01 0a01 1201 7a16 4669 744d 6f64 656c  ......z.FitModel
-00000510: 2e5f 5f70 6f73 745f 696e 6974 5f5f 6302  .__post_init__c.
-00000520: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000530: 0000 0043 0000 0073 1e00 0000 7c00 6a00  ...C...s....|.j.
-00000540: 7c01 6701 6401 6402 8400 7c00 6a01 4400  |.g.d.d...|.j.D.
-00000550: 8301 a201 5200 8e00 5300 2903 4e63 0100  ....R...S.).Nc..
-00000560: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000570: 0000 7300 0000 7314 0000 007c 005d 0c7d  ..s...s....|.].}
-00000580: 017c 016a 0056 0001 0071 0264 0053 00a9  .|.j.V...q.d.S..
-00000590: 014e a901 7210 0000 00a9 02da 022e 3072  .N..r.........0r
-000005a0: 2a00 0000 721b 0000 0072 1b00 0000 721c  *...r....r....r.
-000005b0: 0000 00da 093c 6765 6e65 7870 723e 3700  .....<genexpr>7.
-000005c0: 0000 f300 0000 007a 2446 6974 4d6f 6465  .......z$FitMode
-000005d0: 6c2e 6576 616c 7561 7465 2e3c 6c6f 6361  l.evaluate.<loca
-000005e0: 6c73 3e2e 3c67 656e 6578 7072 3e29 0272  ls>.<genexpr>).r
-000005f0: 1e00 0000 7221 0000 0029 0272 2900 0000  ....r!...).r)...
-00000600: da01 7872 1b00 0000 721b 0000 0072 1c00  ..xr....r....r..
-00000610: 0000 da08 6576 616c 7561 7465 3600 0000  ....evaluate6...
-00000620: 7302 0000 0000 017a 1146 6974 4d6f 6465  s......z.FitMode
-00000630: 6c2e 6576 616c 7561 7465 6301 0000 0000  l.evaluatec.....
-00000640: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000650: 0000 0073 1400 0000 7400 6401 6402 8400  ...s....t.d.d...
-00000660: 7c00 6a01 4400 8301 8301 5300 2903 4e63  |.j.D.....S.).Nc
-00000670: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000680: 0300 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000690: 005d 0c7d 017c 016a 000c 0091 0271 0453  .].}.|.j.....q.S
-000006a0: 0072 1b00 0000 a901 7212 0000 0072 2e00  .r......r....r..
-000006b0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000006c0: 00da 0a3c 6c69 7374 636f 6d70 3e3a 0000  ...<listcomp>:..
-000006d0: 0072 3100 0000 7a2b 4669 744d 6f64 656c  .r1...z+FitModel
-000006e0: 2e67 6574 5f6e 756d 6669 7470 6172 732e  .get_numfitpars.
-000006f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000700: 6d70 3e29 02da 0373 756d 7221 0000 00a9  mp>)...sumr!....
-00000710: 0172 2900 0000 721b 0000 0072 1b00 0000  .r)...r....r....
-00000720: 721c 0000 00da 0e67 6574 5f6e 756d 6669  r......get_numfi
-00000730: 7470 6172 7339 0000 0073 0200 0000 0001  tpars9...s......
-00000740: 7a17 4669 744d 6f64 656c 2e67 6574 5f6e  z.FitModel.get_n
-00000750: 756d 6669 7470 6172 7363 0100 0000 0000  umfitparsc......
-00000760: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000770: 0000 7332 0000 007c 006a 0044 005d 267d  ..s2...|.j.D.]&}
-00000780: 017c 016a 010c 007c 006a 027c 016a 0319  .|.j...|.j.|.j..
-00000790: 005f 047c 016a 057c 006a 027c 016a 0319  ._.|.j.|.j.|.j..
-000007a0: 005f 0571 0664 0053 0072 2c00 0000 2906  ._.q.d.S.r,...).
-000007b0: 7221 0000 0072 1200 0000 7226 0000 0072  r!...r....r&...r
-000007c0: 0e00 0000 7227 0000 0072 1000 0000 7228  ....r'...r....r(
-000007d0: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-000007e0: 0000 da06 7570 6461 7465 3c00 0000 7306  ....update<...s.
-000007f0: 0000 0000 010a 0112 017a 0f46 6974 4d6f  .........z.FitMo
-00000800: 6465 6c2e 7570 6461 7465 290e 7213 0000  del.update).r...
-00000810: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000820: 7204 0000 0072 1800 0000 7217 0000 0072  r....r....r....r
-00000830: 0500 0000 720d 0000 0072 2300 0000 722b  ....r....r#...r+
-00000840: 0000 0072 3300 0000 7238 0000 0072 3900  ...r3...r8...r9.
-00000850: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00000860: 0072 1c00 0000 721d 0000 0019 0000 0073  .r....r........s
-00000870: 1400 0000 0a02 0404 0801 0801 0803 0c01  ................
-00000880: 0c02 0e0f 0803 0803 721d 0000 0063 0000  ........r....c..
-00000890: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000008a0: 0000 4000 0000 7374 0000 0065 005a 0164  ..@...st...e.Z.d
-000008b0: 005a 0255 0065 036a 0465 0564 013c 0065  .Z.U.e.j.e.d.<.e
-000008c0: 036a 0465 0564 023c 0064 035a 0665 036a  .j.e.d.<.d.Z.e.j
-000008d0: 0465 0564 043c 0064 035a 0765 036a 0465  .e.d.<.d.Z.e.j.e
-000008e0: 0564 053c 0065 0864 0664 078d 015a 0965  .d.<.e.d.d...Z.e
-000008f0: 0a65 0b19 0065 0564 083c 0064 0964 0a84  .e...e.d.<.d.d..
-00000900: 005a 0c64 0b64 0c84 005a 0d64 0d64 0e84  .Z.d.d...Z.d.d..
-00000910: 005a 0e64 0f64 1084 005a 0f64 0353 0029  .Z.d.d...Z.d.S.)
-00000920: 11da 0746 6974 4461 7461 7232 0000 00da  ...FitDatar2....
-00000930: 0179 4eda 0278 65da 0279 6546 2901 da04  .yN..xe..yeF)...
-00000940: 696e 6974 da04 6d61 736b 6301 0000 0000  init..maskc.....
-00000950: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00000960: 0000 0073 1600 0000 7c00 a000 7401 6a02  ...s....|...t.j.
-00000970: 0b00 7401 6a02 a102 0100 6400 5300 722c  ..t.j.....d.S.r,
-00000980: 0000 0029 03da 0873 6574 5f6d 6173 6bda  ...)...set_mask.
-00000990: 026e 70da 0369 6e66 7237 0000 0072 1b00  .np..infr7...r..
-000009a0: 0000 721b 0000 0072 1c00 0000 722b 0000  ..r....r....r+..
-000009b0: 004a 0000 0073 0200 0000 0001 7a15 4669  .J...s......z.Fi
-000009c0: 7444 6174 612e 5f5f 706f 7374 5f69 6e69  tData.__post_ini
-000009d0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-000009e0: 0200 0000 0500 0000 0300 0000 7326 0000  ............s&..
-000009f0: 0087 0066 0164 0164 0284 0888 006a 0088  ...f.d.d.....j..
-00000a00: 006a 0188 006a 0288 006a 0366 0444 0083  .j...j...j.f.D..
-00000a10: 017d 017c 0153 0029 034e 6301 0000 0000  .}.|.S.).Nc.....
-00000a20: 0000 0000 0000 0002 0000 0003 0000 0033  ...............3
-00000a30: 0000 0073 2400 0000 7c00 5d1c 7d01 7c01  ...s$...|.].}.|.
-00000a40: 6400 7501 7218 7c01 8800 6a00 1900 6e02  d.u.r.|...j...n.
-00000a50: 6400 5600 0100 7102 6400 5300 722c 0000  d.V...q.d.S.r,..
-00000a60: 0029 0172 3f00 0000 2902 722f 0000 00da  .).r?...).r/....
-00000a70: 0376 6172 7237 0000 0072 1b00 0000 721c  .varr7...r....r.
-00000a80: 0000 0072 3000 0000 4e00 0000 7304 0000  ...r0...N...s...
-00000a90: 0004 0202 ff7a 1e46 6974 4461 7461 2e67  .....z.FitData.g
-00000aa0: 6574 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  et.<locals>.<gen
-00000ab0: 6578 7072 3e29 0472 3200 0000 723b 0000  expr>).r2...r;..
-00000ac0: 0072 3c00 0000 723d 0000 0029 0272 2900  .r<...r=...).r).
-00000ad0: 0000 da06 7265 7375 6c74 721b 0000 0072  ....resultr....r
-00000ae0: 3700 0000 721c 0000 00da 0367 6574 4d00  7...r......getM.
-00000af0: 0000 7308 0000 0000 010a 0212 fe06 047a  ..s............z
-00000b00: 0b46 6974 4461 7461 2e67 6574 6303 0000  .FitData.getc...
-00000b10: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000b20: 0003 0000 0073 1c00 0000 8700 8701 6602  .....s........f.
-00000b30: 6401 6402 8408 7c00 6a00 4400 8301 7c00  d.d...|.j.D...|.
-00000b40: 5f01 6400 5300 2903 4e63 0100 0000 0000  _.d.S.).Nc......
-00000b50: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-00000b60: 0000 7324 0000 0067 007c 005d 1c7d 0188  ..s$...g.|.].}..
-00000b70: 017c 0104 0003 006b 016f 1a88 006b 016e  .|.....k.o...k.n
-00000b80: 0402 0001 0091 0271 0453 0072 1b00 0000  .......q.S.r....
-00000b90: 721b 0000 0029 0272 2f00 0000 7232 0000  r....).r/...r2..
-00000ba0: 00a9 02da 0478 6d61 78da 0478 6d69 6e72  .....xmax..xminr
-00000bb0: 1b00 0000 721c 0000 0072 3500 0000 5500  ....r....r5...U.
-00000bc0: 0000 7231 0000 007a 2446 6974 4461 7461  ..r1...z$FitData
-00000bd0: 2e73 6574 5f6d 6173 6b2e 3c6c 6f63 616c  .set_mask.<local
-00000be0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0272  s>.<listcomp>).r
-00000bf0: 3200 0000 723f 0000 0029 0372 2900 0000  2...r?...).r)...
-00000c00: 7248 0000 0072 4700 0000 721b 0000 0072  rH...rG...r....r
-00000c10: 4600 0000 721c 0000 0072 4000 0000 5400  F...r....r@...T.
-00000c20: 0000 7302 0000 0000 017a 1046 6974 4461  ..s......z.FitDa
-00000c30: 7461 2e73 6574 5f6d 6173 6b63 0100 0000  ta.set_maskc....
-00000c40: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000c50: 4300 0000 7310 0000 0074 007c 006a 017c  C...s....t.|.j.|
-00000c60: 006a 0219 0083 0153 0072 2c00 0000 2903  .j.....S.r,...).
-00000c70: da03 6c65 6e72 3200 0000 723f 0000 0072  ..lenr2...r?...r
-00000c80: 3700 0000 721b 0000 0072 1b00 0000 721c  7...r....r....r.
-00000c90: 0000 00da 1067 6574 5f6e 756d 6669 7470  .....get_numfitp
-00000ca0: 6f69 6e74 7357 0000 0073 0200 0000 0001  ointsW...s......
-00000cb0: 7a18 4669 7444 6174 612e 6765 745f 6e75  z.FitData.get_nu
-00000cc0: 6d66 6974 706f 696e 7473 2910 7213 0000  mfitpoints).r...
-00000cd0: 0072 1400 0000 7215 0000 0072 4100 0000  .r....r....rA...
-00000ce0: da05 6172 7261 7972 1800 0000 723c 0000  ..arrayr....r<..
-00000cf0: 0072 3d00 0000 7203 0000 0072 3f00 0000  .r=...r....r?...
-00000d00: 7205 0000 0072 1a00 0000 722b 0000 0072  r....r....r+...r
-00000d10: 4500 0000 7240 0000 0072 4a00 0000 721b  E...r@...rJ...r.
-00000d20: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000d30: 0000 723a 0000 0042 0000 0073 1200 0000  ..r:...B...s....
-00000d40: 0a02 0a01 0a01 0e01 0e01 1602 0803 0807  ................
-00000d50: 0803 723a 0000 0063 0000 0000 0000 0000  ..r:...c........
-00000d60: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000d70: 738e 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000d80: 0364 025a 0464 0364 0484 005a 0564 0564  .d.Z.d.d...Z.d.d
-00000d90: 0684 005a 0664 0764 0884 005a 0764 0964  ...Z.d.d...Z.d.d
-00000da0: 0a84 005a 0864 0b64 0b65 0964 0c19 0066  ...Z.d.d.e.d...f
-00000db0: 0364 0d64 0e84 015a 0a64 0f64 1084 005a  .d.d...Z.d.d...Z
-00000dc0: 0b64 0b64 0b65 0964 0c19 0066 0364 1164  .d.d.e.d...f.d.d
-00000dd0: 1284 015a 0c64 1e64 1464 1584 015a 0d64  ...Z.d.d.d...Z.d
-00000de0: 1664 1784 005a 0e64 1864 1984 005a 0f64  .d...Z.d.d...Z.d
-00000df0: 1a64 1b84 005a 1064 1c64 1d84 005a 1164  .d...Z.d.d...Z.d
-00000e00: 0b53 0029 1fda 0646 6974 7465 727a 1763  .S.)...Fitterz.c
-00000e10: 6c61 7373 2074 6f20 6861 6e64 6c65 2074  lass to handle t
-00000e20: 6865 2066 6974 2903 da04 6e6f 6e65 da08  he fit)...none..
-00000e30: 7265 6c61 7469 7665 da08 6162 736f 6c75  relative..absolu
-00000e40: 7465 630a 0000 0000 0000 0000 0000 000b  tec.............
-00000e50: 0000 0006 0000 004b 0000 0073 6400 0000  .......K...sd...
-00000e60: 7c0a 7c00 5f00 7c00 a001 7c02 7c03 7c04  |.|._.|...|.|.|.
-00000e70: 7c05 a104 7c00 5f02 7c00 a003 7c01 7c06  |...|._.|...|.|.
-00000e80: 7c07 7c08 a104 7c00 5f04 6400 7c00 5f05  |.|...|._.d.|._.
-00000e90: 6401 7c00 5f06 6400 7c00 5f07 6900 7c00  d.|._.d.|._.i.|.
-00000ea0: 5f08 7c09 7c00 5f09 6402 7c00 5f0a 6403  _.|.|._.d.|._.d.
-00000eb0: 7c0a 7600 7260 7c0a 6403 1900 7c00 5f0a  |.v.r`|.d...|._.
-00000ec0: 6400 5300 2904 4e46 da07 6c65 6173 7473  d.S.).NF..leasts
-00000ed0: 71da 066d 6574 686f 6429 0bda 066b 7761  q..method)...kwa
-00000ee0: 7267 73da 0a5f 696e 6974 5f64 6174 61da  rgs.._init_data.
-00000ef0: 0464 6174 61da 0b5f 696e 6974 5f6d 6f64  .data.._init_mod
-00000f00: 656c da05 6d6f 6465 6cda 0c6d 6f64 656c  el..model..model
-00000f10: 5f72 6573 756c 74da 0c66 6974 5f69 735f  _result..fit_is_
-00000f20: 7661 6c69 64da 126d 6561 6e5f 7371 7561  valid..mean_squa
-00000f30: 7265 645f 6572 726f 72da 0966 6974 7265  red_error..fitre
-00000f40: 706f 7274 da0a 6973 5f63 6f6d 706c 6578  port..is_complex
-00000f50: 7251 0000 0029 0b72 2900 0000 721e 0000  rQ...).r)...r...
-00000f60: 00da 0578 6461 7461 da05 7964 6174 61da  ...xdata..ydata.
-00000f70: 0478 6572 72da 0479 6572 72da 0270 30da  .xerr..yerr..p0.
-00000f80: 0e61 6273 6f6c 7574 655f 7369 676d 6172  .absolute_sigmar
-00000f90: 1f00 0000 725b 0000 0072 5200 0000 721b  ....r[...rR...r.
-00000fa0: 0000 0072 1b00 0000 721c 0000 00da 085f  ...r....r......_
-00000fb0: 5f69 6e69 745f 5f60 0000 0073 1600 0000  _init__`...s....
-00000fc0: 000e 0601 1201 1202 0601 0601 0601 0601  ................
-00000fd0: 0601 0601 0801 7a0f 4669 7474 6572 2e5f  ......z.Fitter._
-00000fe0: 5f69 6e69 745f 5f63 0500 0000 0000 0000  _init__c........
-00000ff0: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-00001000: 73b6 0000 007c 017c 0266 0244 005d 1a7d  s....|.|.f.D.].}
-00001010: 0574 007c 0583 0174 016a 0275 0172 0874  .t.|...t.j.u.r.t
-00001020: 0364 0183 0182 0171 0874 047c 0183 0174  .d.....q.t.|...t
-00001030: 047c 0283 016b 0372 3c74 0364 0283 0182  .|...k.r<t.d....
-00001040: 017c 0464 0075 0172 7274 007c 0483 0174  .|.d.u.rrt.|...t
-00001050: 016a 0275 0172 5a74 0364 0183 0182 0174  .j.u.rZt.d.....t
-00001060: 047c 0483 0174 047c 0283 016b 0372 7274  .|...t.|...k.rrt
-00001070: 0364 0383 0182 017c 0364 0075 0172 a874  .d.....|.d.u.r.t
-00001080: 007c 0383 0174 016a 0275 0172 9074 0364  .|...t.j.u.r.t.d
-00001090: 0183 0182 0174 047c 0383 0174 047c 0183  .....t.|...t.|..
-000010a0: 016b 0372 a874 0364 0483 0182 0174 057c  .k.r.t.d.....t.|
-000010b0: 017c 027c 037c 0483 0453 0029 054e 7a21  .|.|.|...S.).Nz!
-000010c0: 6461 7461 2073 686f 756c 6420 6861 7665  data should have
-000010d0: 2074 7970 6520 6e75 6d70 7920 6172 7261   type numpy arra
-000010e0: 797a 2978 6461 7461 2061 6e64 2079 6461  yz)xdata and yda
-000010f0: 7461 2073 686f 756c 6420 6265 206f 6620  ta should be of 
-00001100: 6571 7561 6c20 6c65 6e67 7468 7a28 7965  equal lengthz(ye
-00001110: 7272 2061 6e64 2079 6461 7461 2073 686f  rr and ydata sho
-00001120: 756c 6420 6265 206f 6620 6571 7561 6c20  uld be of equal 
-00001130: 6c65 6e67 7468 7a28 7865 7272 2061 6e64  lengthz(xerr and
-00001140: 2078 6461 7461 2073 686f 756c 6420 6265   xdata should be
-00001150: 206f 6620 6571 7561 6c20 6c65 6e67 7468   of equal length
-00001160: 2906 da04 7479 7065 7241 0000 00da 076e  )...typerA.....n
-00001170: 6461 7272 6179 da09 4578 6365 7074 696f  darray..Exceptio
-00001180: 6e72 4900 0000 723a 0000 0029 0672 2900  nrI...r:...).r).
-00001190: 0000 7232 0000 0072 3b00 0000 723c 0000  ..r2...r;...r<..
-000011a0: 0072 3d00 0000 7243 0000 0072 1b00 0000  .r=...rC...r....
-000011b0: 721b 0000 0072 1c00 0000 7253 0000 007b  r....r....rS...{
-000011c0: 0000 0073 2000 0000 0003 0c01 0e01 0a01  ...s ...........
-000011d0: 1001 0803 0801 0e01 0801 1001 0802 0801  ................
-000011e0: 0e01 0801 1001 0802 7a11 4669 7474 6572  ........z.Fitter
-000011f0: 2e5f 696e 6974 5f64 6174 6163 0500 0000  ._init_datac....
-00001200: 0000 0000 0000 0000 0b00 0000 0600 0000  ................
-00001210: 4300 0000 73c8 0000 0074 007c 0183 0173  C...s....t.|...s
-00001220: 1074 0164 0183 0182 0174 02a0 037c 01a1  .t.d.....t...|..
-00001230: 016a 047d 0564 0264 0384 007c 05a0 05a1  .j.}.d.d...|....
-00001240: 0044 0083 017d 067c 0264 0075 0072 4c64  .D...}.|.d.u.rLd
-00001250: 0467 0174 067c 0664 0564 0085 0219 0083  .g.t.|.d.d......
-00001260: 0114 007d 0264 0664 0384 0074 077c 0664  ...}.d.d...t.|.d
-00001270: 0564 0085 0219 007c 0283 0244 0083 017d  .d.....|...D...}
-00001280: 077c 006a 086a 0964 0075 0172 907c 0372  .|.j.j.d.u.r.|.r
-00001290: 847c 006a 0a64 0719 007d 0871 9a7c 006a  .|.j.d...}.q.|.j
-000012a0: 0a64 0519 007d 086e 0a7c 006a 0a64 0819  .d...}.n.|.j.d..
-000012b0: 007d 087c 016a 0b64 0075 0072 aa64 097d  .}.|.j.d.u.r.d.}
-000012c0: 096e 0a74 0c7c 016a 0b83 017d 0974 0d7c  .n.t.|.j...}.t.|
-000012d0: 017c 047c 087c 077c 0983 057d 0a7c 0a53  .|.|.|.|...}.|.S
-000012e0: 0029 0a4e 7a18 4e6f 7420 6120 7661 6c69  .).Nz.Not a vali
-000012f0: 6420 6669 7420 6675 6e63 7469 6f6e 6301  d fit functionc.
-00001300: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001310: 0000 0053 0000 0073 1200 0000 6700 7c00  ...S...s....g.|.
-00001320: 5d0a 7d01 7c01 6a00 9102 7104 5300 721b  ].}.|.j...q.S.r.
-00001330: 0000 00a9 0172 0e00 0000 a902 722f 0000  .....r......r/..
-00001340: 00da 0361 7267 721b 0000 0072 1b00 0000  ...argr....r....
-00001350: 721c 0000 0072 3500 0000 9a00 0000 7231  r....r5.......r1
-00001360: 0000 007a 2646 6974 7465 722e 5f69 6e69  ...z&Fitter._ini
-00001370: 745f 6d6f 6465 6c2e 3c6c 6f63 616c 733e  t_model.<locals>
-00001380: 2e3c 6c69 7374 636f 6d70 3e72 0f00 0000  .<listcomp>r....
-00001390: 720a 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000013a0: 0000 0300 0000 0500 0000 5300 0000 731a  ..........S...s.
-000013b0: 0000 0067 007c 005d 125c 027d 017d 0274  ...g.|.].\.}.}.t
-000013c0: 007c 017c 0283 0291 0271 0453 0072 1b00  .|.|.....q.S.r..
-000013d0: 0000 2901 720d 0000 0029 0372 2f00 0000  ..).r....).r/...
-000013e0: 7268 0000 0072 1000 0000 721b 0000 0072  rh...r....r....r
-000013f0: 1b00 0000 721c 0000 0072 3500 0000 a100  ....r....r5.....
-00001400: 0000 7302 0000 0006 01e9 0200 0000 7201  ..s...........r.
-00001410: 0000 007a 106e 6f20 696e 666f 206f 6e20  ...z.no info on 
-00001420: 6d6f 6465 6c29 0eda 0863 616c 6c61 626c  model)...callabl
-00001430: 6572 6500 0000 da07 696e 7370 6563 74da  ere.....inspect.
-00001440: 0973 6967 6e61 7475 7265 7226 0000 00da  .signaturer&....
-00001450: 0676 616c 7565 7372 4900 0000 da03 7a69  .valuesrI.....zi
-00001460: 7072 5400 0000 723d 0000 00da 0d57 4549  prT...r=.....WEI
-00001470: 4748 544f 5054 494f 4e53 7216 0000 00da  GHTOPTIONSr.....
-00001480: 1473 7472 6970 5f6c 6561 6469 6e67 5f73  .strip_leading_s
-00001490: 7061 6365 7372 1d00 0000 290b 7229 0000  pacesr....).r)..
-000014a0: 0072 1e00 0000 7260 0000 0072 6100 0000  .r....r`...ra...
-000014b0: 721f 0000 005a 0d5f 4669 7474 6572 5f5f  r....Z._Fitter__
-000014c0: 6172 6773 da04 6172 6773 7221 0000 0072  args..argsr!...r
-000014d0: 2000 0000 7223 0000 005a 0961 6669 746d   ...r#...Z.afitm
-000014e0: 6f64 656c 721b 0000 0072 1b00 0000 721c  odelr....r....r.
-000014f0: 0000 0072 5500 0000 9300 0000 7326 0000  ...rU.......s&..
-00001500: 0000 0208 0108 030c 0112 0308 0116 0306  ................
-00001510: 0110 ff06 050c 0104 010c 020c 020a 030a  ................
-00001520: 0106 020a 0210 017a 1246 6974 7465 722e  .......z.Fitter.
-00001530: 5f69 6e69 745f 6d6f 6465 6c63 0100 0000  _init_modelc....
-00001540: 0000 0000 0000 0000 0f00 0000 0b00 0000  ................
-00001550: 4300 0000 732e 0100 0064 0164 0284 007c  C...s....d.d...|
-00001560: 006a 006a 0144 0083 017d 0164 0364 0284  .j.j.D...}.d.d..
-00001570: 007c 006a 006a 0144 0083 017d 027c 006a  .|.j.j.D...}.|.j
-00001580: 02a0 03a1 005c 047d 037d 047d 057d 067c  .....\.}.}.}.}.|
-00001590: 006a 00a0 04a1 0064 046b 0272 4c74 0564  .j.....d.k.rLt.d
-000015a0: 0583 0182 017c 00a0 06a1 0064 046b 0172  .....|.....d.k.r
-000015b0: 6074 0564 0683 0182 017c 006a 006a 077c  `t.d.....|.j.j.|
-000015c0: 006a 0864 0719 006b 027d 077c 006a 006a  .j.d...k.}.|.j.j
-000015d0: 077c 006a 0864 0419 006b 0272 9274 09a0  .|.j.d...k.r.t..
-000015e0: 0a74 0b7c 0483 01a1 017d 0674 0c7c 006a  .t.|.....}.t.|.j
-000015f0: 007c 037c 047c 067c 017c 027c 006a 0d7c  .|.|.|.|.|.|.j.|
-00001600: 077c 006a 006a 0e64 088d 095c 037d 087d  .|.j.j.d...\.}.}
-00001610: 097d 0a7c 0a7c 005f 0f64 097c 005f 1074  .}.|.|._.d.|._.t
-00001620: 09a0 1174 09a0 127c 09a1 01a1 017d 0b74  ...t...|.....}.t
-00001630: 137c 006a 006a 017c 087c 0b83 0344 005d  .|.j.j.|.|...D.]
-00001640: 165c 037d 0c7d 0d7d 0e7c 0d7c 0c5f 147c  .\.}.}.}.|.|._.|
-00001650: 0e7c 0c5f 1571 e674 167c 047c 006a 00a0  .|._.q.t.|.|.j..
-00001660: 177c 03a1 0118 007c 061b 0064 0713 0083  .|.....|...d....
-00001670: 017c 005f 187c 00a0 19a1 0001 007c 087c  .|._.|.......|.|
-00001680: 097c 0a66 0353 0029 0a7a 220a 2020 2020  .|.f.S.).z".    
-00001690: 2020 2020 7065 7266 6f72 6d73 2074 6865      performs the
-000016a0: 2066 6974 0a20 2020 2020 2020 2063 0100   fit.        c..
-000016b0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000016c0: 0000 5300 0000 7312 0000 0067 007c 005d  ..S...s....g.|.]
-000016d0: 0a7d 017c 016a 0091 0271 0453 0072 1b00  .}.|.j...q.S.r..
-000016e0: 0000 722d 0000 00a9 0272 2f00 0000 da06  ..r-.....r/.....
-000016f0: 6669 7470 6172 721b 0000 0072 1b00 0000  fitparr....r....
-00001700: 721c 0000 0072 3500 0000 bc00 0000 7231  r....r5.......r1
-00001710: 0000 007a 1e46 6974 7465 722e 6669 742e  ...z.Fitter.fit.
-00001720: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00001730: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00001740: 0200 0000 0300 0000 5300 0000 7312 0000  ........S...s...
-00001750: 0067 007c 005d 0a7d 017c 016a 0091 0271  .g.|.].}.|.j...q
-00001760: 0453 0072 1b00 0000 7234 0000 0072 7200  .S.r....r4...rr.
-00001770: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001780: 0072 3500 0000 bd00 0000 7231 0000 0072  .r5.......r1...r
-00001790: 0100 0000 7a2e 5468 6572 6520 7368 6f75  ....z.There shou
-000017a0: 6c64 2062 6520 6174 206c 6561 7374 206f  ld be at least o
-000017b0: 6e65 2066 7265 6520 6669 7470 6172 616d  ne free fitparam
-000017c0: 6574 6572 7a98 5468 6520 6e75 6d62 6572  eterz.The number
-000017d0: 206f 6620 6465 6772 6565 7320 6f66 2066   of degrees of f
-000017e0: 7265 6564 6f6d 2028 646f 6629 2073 686f  reedom (dof) sho
-000017f0: 756c 6420 6265 2061 7420 6c65 6173 7420  uld be at least 
-00001800: 6f6e 652e 2054 7279 2074 6f20 696e 6372  one. Try to incr
-00001810: 6561 7365 2074 6865 206e 756d 6265 7220  ease the number 
-00001820: 6f66 2064 6174 6170 6f69 6e74 7320 6f72  of datapoints or
-00001830: 2074 6f20 6465 6372 6561 7365 2074 6865   to decrease the
-00001840: 206e 756d 6265 7220 6f66 2066 7265 6520   number of free 
-00001850: 6669 7470 6172 616d 6574 6572 732e 7269  fitparameters.ri
-00001860: 0000 0029 0672 1100 0000 7260 0000 00da  ...).r....r`....
-00001870: 0270 4672 5100 0000 7261 0000 0072 1f00  .pFrQ...ra...r..
-00001880: 0000 5429 1a72 5600 0000 7221 0000 0072  ..T).rV...r!...r
-00001890: 5400 0000 7245 0000 0072 3800 0000 7208  T...rE...r8...r.
-000018a0: 0000 00da 135f 6465 6772 6565 735f 6f66  ....._degrees_of
-000018b0: 5f66 7265 6564 6f6d 7220 0000 0072 6f00  _freedomr ...ro.
-000018c0: 0000 7241 0000 00da 046f 6e65 7372 4900  ..rA.....onesrI.
-000018d0: 0000 da11 6375 7276 655f 6669 745f 7772  ....curve_fit_wr
-000018e0: 6170 7065 7272 5100 0000 721f 0000 0072  apperrQ...r....r
-000018f0: 5700 0000 7258 0000 00da 0473 7172 74da  W...rX.....sqrt.
-00001900: 0464 6961 6772 6e00 0000 7210 0000 0072  .diagrn...r....r
-00001910: 1100 0000 7236 0000 0072 3300 0000 7259  ....r6...r3...rY
-00001920: 0000 00da 0e5f 6372 6561 7465 5f72 6570  ....._create_rep
-00001930: 6f72 7429 0f72 2900 0000 7260 0000 0072  ort).r)...r`...r
-00001940: 7400 0000 7232 0000 0072 3b00 0000 723c  t...r2...r;...r<
-00001950: 0000 0072 3d00 0000 7261 0000 00da 0470  ...r=...ra.....p
-00001960: 6f70 74da 0470 636f 7672 4400 0000 5a09  opt..pcovrD...Z.
-00001970: 7374 6465 7272 6f72 7372 7300 0000 7210  stderrorsrs...r.
-00001980: 0000 00da 0673 7464 6572 7272 1b00 0000  .....stderrr....
-00001990: 721b 0000 0072 1c00 0000 da03 6669 74b7  r....r......fit.
-000019a0: 0000 0073 4400 0000 0005 1201 1202 1203  ...sD...........
-000019b0: 0e01 0201 02ff 0404 0c01 0201 02ff 0405  ................
-000019c0: 1201 1201 0e02 0201 0401 0201 0201 0201  ................
-000019d0: 0201 0201 0401 0201 06f7 0c0c 0603 0601  ................
-000019e0: 1001 1a01 0601 0802 1e02 0801 7a0a 4669  ............z.Fi
-000019f0: 7474 6572 2e66 6974 4eda 0f4d 4f44 454c  tter.fitN..MODEL
-00001a00: 5f4e 554d 504f 494e 5453 6304 0000 0000  _NUMPOINTSc.....
-00001a10: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-00001a20: 0000 0073 7000 0000 7c01 6400 7500 7214  ...sp...|.d.u.r.
-00001a30: 7c00 6a00 6a01 a002 a100 7d01 7c02 6400  |.j.j.....}.|.d.
-00001a40: 7500 7228 7c00 6a00 6a01 a003 a100 7d02  u.r(|.j.j.....}.
-00001a50: 7404 a005 7c01 7c02 7c03 a103 7d04 7c00  t...|.|.|...}.|.
-00001a60: 6a06 7354 7c00 6a07 6a08 6a09 7c00 6a07  j.sT|.j.j.j.|.j.
-00001a70: 6a0a 7c04 6401 8d02 7d05 6e14 7c00 6a06  j.|.d...}.n.|.j.
-00001a80: 6a09 7c00 6a06 6a0b 7c04 6401 8d02 7d05  j.|.j.j.|.d...}.
-00001a90: 7c04 7c05 6602 5300 2902 4e29 0172 3200  |.|.f.S.).N).r2.
-00001aa0: 0000 290c 7254 0000 0072 3200 0000 da03  ..).rT...r2.....
-00001ab0: 6d69 6eda 036d 6178 7241 0000 00da 086c  min..maxrA.....l
-00001ac0: 696e 7370 6163 6572 5700 0000 7256 0000  inspacerW...rV..
-00001ad0: 0072 2500 0000 da04 6576 616c 7226 0000  .r%.....evalr&..
-00001ae0: 00da 0670 6172 616d 7329 0672 2900 0000  ...params).r)...
-00001af0: 7248 0000 0072 4700 0000 da09 6e75 6d70  rH...rG.....nump
-00001b00: 6f69 6e74 735a 0678 6375 7276 655a 0679  ointsZ.xcurveZ.y
-00001b10: 6375 7276 6572 1b00 0000 721b 0000 0072  curver....r....r
-00001b20: 1c00 0000 da09 6765 745f 6375 7276 65eb  ......get_curve.
-00001b30: 0000 0073 1600 0000 0003 0801 0c01 0801  ...s............
-00001b40: 0c01 0e03 0602 0801 08ff 0805 1401 7a10  ..............z.
-00001b50: 4669 7474 6572 2e67 6574 5f63 7572 7665  Fitter.get_curve
-00001b60: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001b70: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00001b80: 6a00 5300 722c 0000 0029 0172 5700 0000  j.S.r,...).rW...
-00001b90: 7237 0000 0072 1b00 0000 721b 0000 0072  r7...r....r....r
-00001ba0: 1c00 0000 da10 6765 745f 6d6f 6465 6c5f  ......get_model_
-00001bb0: 7265 7375 6c74 ff00 0000 7302 0000 0000  result....s.....
-00001bc0: 017a 1746 6974 7465 722e 6765 745f 6d6f  .z.Fitter.get_mo
-00001bd0: 6465 6c5f 7265 7375 6c74 6304 0000 0000  del_resultc.....
-00001be0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-00001bf0: 0000 0073 1800 0000 7c00 6a00 730a 6400  ...s....|.j.s.d.
-00001c00: 5300 7c00 a001 7c01 7c02 7c03 a103 5300  S.|...|.|.|...S.
-00001c10: 722c 0000 0029 0272 5800 0000 7286 0000  r,...).rX...r...
-00001c20: 0029 0472 2900 0000 7248 0000 0072 4700  .).r)...rH...rG.
-00001c30: 0000 7285 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00001c40: 0072 1c00 0000 da0c 6765 745f 6669 7463  .r......get_fitc
-00001c50: 7572 7665 0201 0000 7306 0000 0000 0306  urve....s.......
-00001c60: 0104 017a 1346 6974 7465 722e 6765 745f  ...z.Fitter.get_
-00001c70: 6669 7463 7572 7665 5463 0200 0000 0000  fitcurveTc......
-00001c80: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-00001c90: 0000 7320 0000 007c 006a 0073 0e7c 0172  ..s ...|.j.s.|.r
-00001ca0: 0e64 0153 007c 006a 0173 1864 0153 007c  .d.S.|.j.s.d.S.|
-00001cb0: 006a 016a 0253 0029 027a 850a 2020 2020  .j.j.S.).z..    
-00001cc0: 2020 2020 7265 7475 726e 2074 6865 2072      return the r
-00001cd0: 6573 6964 7561 6c73 2061 7320 7920 2d20  esiduals as y - 
-00001ce0: 6628 7829 0a20 2020 2020 2020 2069 6620  f(x).        if 
-00001cf0: 6368 6563 6b20 6973 2054 7275 6528 6465  check is True(de
-00001d00: 6661 756c 7429 206f 6e6c 7920 7265 7475  fault) only retu
-00001d10: 726e 7320 7661 6c75 6573 2069 6620 6120  rns values if a 
-00001d20: 7661 6c69 6420 6669 7420 6973 2070 6572  valid fit is per
-00001d30: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-00001d40: 4e29 0372 5800 0000 7257 0000 00da 0872  N).rX...rW.....r
-00001d50: 6573 6964 7561 6c29 0272 2900 0000 da05  esidual).r).....
-00001d60: 6368 6563 6b72 1b00 0000 721b 0000 0072  checkr....r....r
-00001d70: 1c00 0000 da0d 6765 745f 7265 7369 6475  ......get_residu
-00001d80: 616c 7309 0100 0073 0a00 0000 0006 0a01  als....s........
-00001d90: 0401 0601 0403 7a14 4669 7474 6572 2e67  ......z.Fitter.g
-00001da0: 6574 5f72 6573 6964 7561 6c73 6301 0000  et_residualsc...
-00001db0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00001dc0: 0043 0000 0073 1800 0000 7400 7c00 6a01  .C...s....t.|.j.
-00001dd0: a002 a100 7c00 6a03 a004 a100 1800 8301  ....|.j.........
-00001de0: 5300 722c 0000 0029 05da 0369 6e74 7254  S.r,...)...intrT
-00001df0: 0000 0072 4a00 0000 7256 0000 0072 3800  ...rJ...rV...r8.
-00001e00: 0000 7237 0000 0072 1b00 0000 721b 0000  ..r7...r....r...
-00001e10: 0072 1c00 0000 7275 0000 0017 0100 0073  .r....ru.......s
-00001e20: 0200 0000 0001 7a1a 4669 7474 6572 2e5f  ......z.Fitter._
-00001e30: 6465 6772 6565 735f 6f66 5f66 7265 6564  degrees_of_freed
-00001e40: 6f6d 6301 0000 0000 0000 0000 0000 0002  omc.............
-00001e50: 0000 0009 0000 0003 0000 0073 5e00 0000  ...........s^...
-00001e60: 8700 6601 6401 6402 8408 7d01 8800 6a00  ..f.d.d...}...j.
-00001e70: 6a01 8800 6a00 6a02 8800 6a03 a004 a100  j...j.j...j.....
-00001e80: 8800 a005 a100 7406 6a07 a008 6403 8800  ......t.j...d...
-00001e90: a005 a100 a102 6404 9c05 7c01 8300 8800  ......d...|.....
-00001ea0: 6a09 8800 6a0a 6a0b 8800 6a0a 6a0c 6405  j...j.j...j.j.d.
-00001eb0: 9c03 6406 9c03 8800 5f0d 6400 5300 2907  ..d....._.d.S.).
-00001ec0: 4e63 0000 0000 0000 0000 0000 0000 0100  Nc..............
-00001ed0: 0000 0200 0000 1300 0000 7316 0000 0064  ..........s....d
-00001ee0: 0164 0284 0088 006a 006a 0144 0083 017d  .d.....j.j.D...}
-00001ef0: 007c 0053 0029 034e 6301 0000 0000 0000  .|.S.).Nc.......
-00001f00: 0000 0000 0002 0000 0008 0000 0053 0000  .............S..
-00001f10: 0073 2400 0000 6900 7c00 5d1c 7d01 7c01  .s$...i.|.].}.|.
-00001f20: 6a00 7401 7c01 6a02 7c01 6a03 7c01 6a04  j.t.|.j.|.j.|.j.
-00001f30: 6400 8d03 9302 7104 5300 2901 2903 7210  d.....q.S.).).r.
-00001f40: 0000 0072 7d00 0000 7212 0000 0029 0572  ...r}...r....).r
-00001f50: 0e00 0000 da04 6469 6374 7210 0000 0072  ......dictr....r
-00001f60: 1100 0000 7212 0000 0072 2e00 0000 721b  ....r....r....r.
-00001f70: 0000 0072 1b00 0000 721c 0000 00da 0a3c  ...r....r......<
-00001f80: 6469 6374 636f 6d70 3e1c 0100 0073 0800  dictcomp>....s..
-00001f90: 0000 0604 02fd 0601 0cff 7a3f 4669 7474  ..........z?Fitt
-00001fa0: 6572 2e5f 6372 6561 7465 5f72 6570 6f72  er._create_repor
-00001fb0: 742e 3c6c 6f63 616c 733e 2e70 6172 735f  t.<locals>.pars_
-00001fc0: 746f 5f64 6963 742e 3c6c 6f63 616c 733e  to_dict.<locals>
-00001fd0: 2e3c 6469 6374 636f 6d70 3e29 0272 5600  .<dictcomp>).rV.
-00001fe0: 0000 7221 0000 0029 015a 0870 6172 7364  ..r!...).Z.parsd
-00001ff0: 6963 7472 3700 0000 721b 0000 0072 1c00  ictr7...r....r..
-00002000: 0000 da0c 7061 7273 5f74 6f5f 6469 6374  ....pars_to_dict
-00002010: 1b01 0000 7308 0000 0000 0106 0406 fc06  ....s...........
-00002020: 067a 2b46 6974 7465 722e 5f63 7265 6174  .z+Fitter._creat
-00002030: 655f 7265 706f 7274 2e3c 6c6f 6361 6c73  e_report.<locals
-00002040: 3e2e 7061 7273 5f74 6f5f 6469 6374 6733  >.pars_to_dictg3
-00002050: 3333 3333 33ef 3f29 0572 5600 0000 7220  33333.?).rV...r 
-00002060: 0000 00da 014e da03 646f 667a 0774 3935  .....N..dofz.t95
-00002070: 2d76 616c 2903 7a18 536d 696e 2c20 6d65  -val).z.Smin, me
-00002080: 616e 2073 7175 6172 6564 2065 7272 6f72  an squared error
-00002090: 7a0b 4368 6920 5371 7561 7265 647a 0352  z.Chi Squaredz.R
-000020a0: 5e32 2903 5a0d 4649 5450 4152 414d 4554  ^2).Z.FITPARAMET
-000020b0: 4552 535a 0a46 4954 5245 5355 4c54 535a  ERSZ.FITRESULTSZ
-000020c0: 0a53 5441 5449 5354 4943 5329 0e72 5600  .STATISTICS).rV.
-000020d0: 0000 7223 0000 0072 2000 0000 7254 0000  ..r#...r ...rT..
-000020e0: 0072 4a00 0000 7275 0000 0072 0700 0000  .rJ...ru...r....
-000020f0: da01 745a 0370 7066 7259 0000 0072 5700  ..tZ.ppfrY...rW.
-00002100: 0000 5a06 6368 6973 7172 5a08 7273 7175  ..Z.chisqrZ.rsqu
-00002110: 6172 6564 725a 0000 0029 0272 2900 0000  aredrZ...).r)...
-00002120: 728f 0000 0072 1b00 0000 7237 0000 0072  r....r....r7...r
-00002130: 1c00 0000 727a 0000 001a 0100 0073 1a00  ....rz.......s..
-00002140: 0000 0001 0c0b 0601 0601 0801 0601 10fb  ................
-00002150: 0407 0402 0401 0601 06fd 04f7 7a15 4669  ............z.Fi
-00002160: 7474 6572 2e5f 6372 6561 7465 5f72 6570  tter._create_rep
-00002170: 6f72 7463 0100 0000 0000 0000 0000 0000  ortc............
-00002180: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-00002190: 007c 006a 0053 0072 2c00 0000 2901 725a  .|.j.S.r,...).rZ
-000021a0: 0000 0072 3700 0000 721b 0000 0072 1b00  ...r7...r....r..
-000021b0: 0000 721c 0000 00da 0a67 6574 5f72 6570  ..r......get_rep
-000021c0: 6f72 7434 0100 0073 0200 0000 0001 7a11  ort4...s......z.
-000021d0: 4669 7474 6572 2e67 6574 5f72 6570 6f72  Fitter.get_repor
-000021e0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-000021f0: 0000 0300 0000 4300 0000 7324 0000 007c  ......C...s$...|
-00002200: 006a 006a 0164 0075 0172 127c 006a 0253  .j.j.d.u.r.|.j.S
-00002210: 007c 006a 0264 0164 0285 0219 0053 0064  .|.j.d.d.....S.d
-00002220: 0053 0029 034e 7201 0000 0072 0a00 0000  .S.).Nr....r....
-00002230: 2903 7254 0000 0072 3d00 0000 726f 0000  ).rT...r=...ro..
-00002240: 0072 3700 0000 721b 0000 0072 1b00 0000  .r7...r....r....
-00002250: 721c 0000 00da 1167 6574 5f77 6569 6768  r......get_weigh
-00002260: 746f 7074 696f 6e73 3701 0000 7306 0000  toptions7...s...
-00002270: 0000 010c 0106 037a 1846 6974 7465 722e  .......z.Fitter.
-00002280: 6765 745f 7765 6967 6874 6f70 7469 6f6e  get_weightoption
-00002290: 7329 0154 2912 7213 0000 0072 1400 0000  s).T).r....r....
-000022a0: 7215 0000 0072 1600 0000 726f 0000 0072  r....r....ro...r
-000022b0: 6200 0000 7253 0000 0072 5500 0000 727e  b...rS...rU...r~
-000022c0: 0000 0072 0c00 0000 7286 0000 0072 8700  ...r....r....r..
-000022d0: 0000 7288 0000 0072 8b00 0000 7275 0000  ..r....r....ru..
-000022e0: 0072 7a00 0000 7293 0000 0072 9400 0000  .rz...r....r....
-000022f0: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00002300: 1c00 0000 724c 0000 005b 0000 0073 2000  ....rL...[...s .
-00002310: 0000 0801 0402 0402 081b 0818 0824 0835  .............$.5
-00002320: 0aff 0a14 0804 0aff 0a07 0a0e 0803 081a  ................
-00002330: 0803 724c 0000 0072 5000 0000 2904 7260  ..rL...rP...).r`
-00002340: 0000 0072 7400 0000 721f 0000 0072 5100  ...rt...r....rQ.
-00002350: 0000 6301 0000 0000 0000 0004 0000 0019  ..c.............
-00002360: 0000 0008 0000 004f 0000 0073 1802 0000  .......O...s....
-00002370: 7400 a001 7c00 6a02 a101 6a03 7d07 6401  t...|.j...j.}.d.
-00002380: 6402 8400 7c07 a004 a100 4400 8301 7d08  d...|.....D...}.
-00002390: 7c02 6403 7500 7244 7405 a006 6404 6402  |.d.u.rDt...d.d.
-000023a0: 8400 7c08 6405 6403 8502 1900 4400 8301  ..|.d.d.....D...
-000023b0: a101 7d02 7c01 6403 7500 7268 7405 a006  ..}.|.d.u.rht...
-000023c0: 6406 6402 8400 7c08 6405 6403 8502 1900  d.d...|.d.d.....
-000023d0: 4400 8301 a101 7d01 7c08 6407 1900 6701  D.....}.|.d...g.
-000023e0: 6408 6402 8400 7407 7c08 6405 6403 8502  d.d...t.|.d.d...
-000023f0: 1900 7c02 8302 4400 8301 1700 7d09 7c08  ..|...D.....}.|.
-00002400: 6407 1900 6701 6409 6402 8400 7407 7c08  d...g.d.d...t.|.
-00002410: 6405 6403 8502 1900 7c02 7c01 8303 4400  d.d.....|.|...D.
-00002420: 8301 1700 7d0a 7408 640a 640b a009 7c09  ....}.t.d.d...|.
-00002430: a101 9b00 640c 640b a009 7c0a a101 9b00  ....d.d...|.....
-00002440: 640d 9d05 740a 8300 8302 7d0b 740b 7c03  d...t.....}.t.|.
-00002450: 8301 9001 7226 7405 a006 640e 6402 8400  ....r&t...d.d...
-00002460: 740c 7c02 8301 4400 8301 a101 7d0c 7408  t.|...D.....}.t.
-00002470: 640a 640b a009 7c09 a101 9b00 640f 640b  d.d...|.....d.d.
-00002480: a009 7c0a a101 9b00 6410 9d05 740a 8300  ..|.....d...t...
-00002490: 8302 7d0d 6e04 7c03 7d0d 7405 a006 6411  ..}.n.|.}.t...d.
-000024a0: 6402 8400 7407 7c01 7c02 8302 4400 8301  d...t.|.|...D...
-000024b0: a101 7d0e 7c00 6a03 7d0f 7407 7c08 6405  ..}.|.j.}.t.|.d.
-000024c0: 6403 8502 1900 7c02 7c01 8303 4400 5d22  d.....|.|...D.]"
-000024d0: 5c03 7d10 7d11 7d12 7c11 0c00 7c0f 7c10  \.}.}.}.|...|.|.
-000024e0: 1900 5f0d 7c12 7c0f 7c10 1900 5f0e 9001  .._.|.|.|..._...
-000024f0: 715e 7c00 6a0f 6a10 7c05 6405 1900 7c0f  q^|.j.j.|.d...|.
-00002500: 7c05 6407 1900 6412 6413 7c04 6414 8d06  |.d...d.d.|.d...
-00002510: 7d13 7405 a006 7411 7c13 6a12 a004 a100  }.t...t.|.j.....
-00002520: 8301 a101 7d14 7c13 6a13 7d15 6415 6402  ....}.|.j.}.d.d.
-00002530: 8400 7407 7c01 7c02 8302 4400 8301 7d16  ..t.|.|...D...}.
-00002540: 7405 a014 7c02 a101 6407 1900 7d17 7c17  t...|...d...}.|.
-00002550: 4400 5d2a 7d18 7405 6a15 7c15 7c18 6407  D.]*}.t.j.|.|.d.
-00002560: 6405 6416 8d04 7d15 7405 6a15 7c15 7c18  d.d...}.t.j.|.|.
-00002570: 6407 6407 6416 8d04 7d15 9001 71e2 7c14  d.d.d...}...q.|.
-00002580: 7c15 7c13 6603 5300 2917 613f 0100 000a  |.|.f.S.).a?....
-00002590: 2020 2020 7772 6170 7065 7220 6172 6f75      wrapper arou
-000025a0: 6e64 2074 6865 2073 6369 7079 2063 7572  nd the scipy cur
-000025b0: 7665 5f66 6974 2829 2066 756e 6374 696f  ve_fit() functio
-000025c0: 6e20 746f 2061 6c6c 6f77 2070 6172 616d  n to allow param
-000025d0: 6574 6572 7320 746f 2062 6520 6669 7865  eters to be fixe
-000025e0: 640a 2020 2020 7361 6d65 2063 616c 6c20  d.    same call 
-000025f0: 7369 676e 6174 7572 6520 6173 2074 6865  signature as the
-00002600: 2063 7572 7665 5f66 6974 2829 2066 756e   curve_fit() fun
-00002610: 6374 696f 6e20 6578 6365 7074 2066 6f72  ction except for
-00002620: 3a0a 2020 2020 7046 203a 2031 4420 6e75  :.    pF : 1D nu
-00002630: 6d70 7920 6172 7261 7920 6f66 2073 697a  mpy array of siz
-00002640: 6520 6e2c 2077 6974 6820 6e20 7468 6520  e n, with n the 
-00002650: 6e75 6d62 6572 206f 6620 6669 7470 6172  number of fitpar
-00002660: 616d 6574 6572 7320 6f66 2074 6865 2066  ameters of the f
-00002670: 756e 6374 696f 6e0a 2020 2020 7265 7475  unction.    retu
-00002680: 726e 7320 7468 6520 706f 7074 2061 6e64  rns the popt and
-00002690: 2063 6f76 206d 6174 7269 6365 7320 6a75   cov matrices ju
-000026a0: 7374 206c 696b 6520 7468 6520 6f72 6967  st like the orig
-000026b0: 696e 616c 2063 7572 7665 5f66 6974 2829  inal curve_fit()
-000026c0: 2066 756e 6374 696f 6e0a 2020 2020 6301   function.    c.
-000026d0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000026e0: 0000 0053 0000 0073 1200 0000 6700 7c00  ...S...s....g.|.
-000026f0: 5d0a 7d01 7c01 6a00 9102 7104 5300 721b  ].}.|.j...q.S.r.
-00002700: 0000 0072 6600 0000 7267 0000 0072 1b00  ...rf...rg...r..
-00002710: 0000 721b 0000 0072 1c00 0000 7235 0000  ..r....r....r5..
-00002720: 004b 0100 0072 3100 0000 7a25 6375 7276  .K...r1...z%curv
-00002730: 655f 6669 745f 7772 6170 7065 722e 3c6c  e_fit_wrapper.<l
-00002740: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00002750: 3e4e 6301 0000 0000 0000 0000 0000 0002  >Nc.............
-00002760: 0000 0003 0000 0053 0000 0073 1000 0000  .......S...s....
-00002770: 6700 7c00 5d08 7d01 6400 9102 7104 5300  g.|.].}.d...q.S.
-00002780: a901 4672 1b00 0000 a902 722f 0000 00da  ..Fr......r/....
-00002790: 015f 721b 0000 0072 1b00 0000 721c 0000  ._r....r....r...
-000027a0: 0072 3500 0000 4f01 0000 7231 0000 0072  .r5...O...r1...r
-000027b0: 0a00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000027c0: 0002 0000 0003 0000 0053 0000 0073 1000  .........S...s..
-000027d0: 0000 6700 7c00 5d08 7d01 6400 9102 7104  ..g.|.].}.d...q.
-000027e0: 5300 2901 720a 0000 0072 1b00 0000 7296  S.).r....r....r.
-000027f0: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-00002800: 0000 7235 0000 0051 0100 0072 3100 0000  ..r5...Q...r1...
-00002810: 7201 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00002820: 0000 0300 0000 0400 0000 5300 0000 7318  ..........S...s.
-00002830: 0000 0067 007c 005d 105c 027d 017d 027c  ...g.|.].\.}.}.|
-00002840: 0273 047c 0191 0271 0453 0072 1b00 0000  .s.|...q.S.r....
-00002850: 721b 0000 0029 0372 2f00 0000 7268 0000  r....).r/...rh..
-00002860: 00da 0366 6978 721b 0000 0072 1b00 0000  ...fixr....r....
-00002870: 721c 0000 0072 3500 0000 5401 0000 7302  r....r5...T...s.
-00002880: 0000 0006 0163 0100 0000 0000 0000 0000  .....c..........
-00002890: 0000 0400 0000 0500 0000 5300 0000 7322  ..........S...s"
-000028a0: 0000 0067 007c 005d 1a5c 037d 017d 027d  ...g.|.].\.}.}.}
-000028b0: 037c 0273 167c 016e 0674 007c 0383 0191  .|.s.|.n.t.|....
-000028c0: 0271 0453 0072 1b00 0000 2901 7217 0000  .q.S.r....).r...
-000028d0: 0029 0472 2f00 0000 7268 0000 0072 9800  .).r/...rh...r..
-000028e0: 0000 da01 7072 1b00 0000 721b 0000 0072  ....pr....r....r
-000028f0: 1c00 0000 7235 0000 0057 0100 0073 0200  ....r5...W...s..
-00002900: 0000 0601 7a07 6c61 6d62 6461 207a 022c  ....z.lambda z.,
-00002910: 207a 0820 3a20 6675 6e63 28fa 0129 6301   z. : func(..)c.
-00002920: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00002930: 0000 0053 0000 0073 1c00 0000 6700 7c00  ...S...s....g.|.
-00002940: 5d14 5c02 7d01 7d02 7c02 6400 6b02 7204  ].\.}.}.|.d.k.r.
-00002950: 7c01 9102 7104 5300 7295 0000 0072 1b00  |...q.S.r....r..
-00002960: 0000 2903 722f 0000 00da 0569 6e64 6578  ..).r/.....index
-00002970: 7210 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
-00002980: 1c00 0000 7235 0000 0064 0100 0072 3100  ....r5...d...r1.
-00002990: 0000 7a07 203a 206a 6163 287a 0d29 5b3a  ..z. : jac(z.)[:
-000029a0: 2c20 696e 6469 6365 735d 6301 0000 0000  , indices]c.....
-000029b0: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
-000029c0: 0000 0073 1800 0000 6700 7c00 5d10 5c02  ...s....g.|.].\.
-000029d0: 7d01 7d02 7c02 7304 7c01 9102 7104 5300  }.}.|.s.|...q.S.
-000029e0: 721b 0000 0072 1b00 0000 a903 722f 0000  r....r......r/..
-000029f0: 0072 9900 0000 7298 0000 0072 1b00 0000  .r....r....r....
-00002a00: 721b 0000 0072 1c00 0000 7235 0000 006e  r....r....r5...n
-00002a10: 0100 0072 3100 0000 545a 046f 6d69 7429  ...r1...TZ.omit)
-00002a20: 0472 3200 0000 5a0a 6361 6c63 5f63 6f76  .r2...Z.calc_cov
-00002a30: 6172 5a0a 6e61 6e5f 706f 6c69 6379 7251  arZ.nan_policyrQ
-00002a40: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00002a50: 0300 0000 0400 0000 5300 0000 7318 0000  ........S...s...
-00002a60: 0067 007c 005d 105c 027d 017d 027c 0272  .g.|.].\.}.}.|.r
-00002a70: 047c 0191 0271 0453 0072 1b00 0000 721b  .|...q.S.r....r.
-00002a80: 0000 0072 9c00 0000 721b 0000 0072 1b00  ...r....r....r..
-00002a90: 0000 721c 0000 0072 3500 0000 8b01 0000  ..r....r5.......
-00002aa0: 7231 0000 0029 01da 0461 7869 7329 1672  r1...)...axis).r
-00002ab0: 6b00 0000 726c 0000 0072 1e00 0000 7226  k...rl...r....r&
-00002ac0: 0000 0072 6d00 0000 7241 0000 0072 4b00  ...rm...rA...rK.
-00002ad0: 0000 726e 0000 0072 8300 0000 da04 6a6f  ..rn...r......jo
-00002ae0: 696e da06 6c6f 6361 6c73 726a 0000 00da  in..localsrj....
-00002af0: 0965 6e75 6d65 7261 7465 7227 0000 0072  .enumerater'...r
-00002b00: 1000 0000 7225 0000 0072 7e00 0000 da04  ....r%...r~.....
-00002b10: 6c69 7374 5a0b 6265 7374 5f76 616c 7565  listZ.best_value
-00002b20: 735a 0563 6f76 6172 da05 7768 6572 65da  sZ.covar..where.
-00002b30: 0669 6e73 6572 7429 1972 5600 0000 7260  .insert).rV...r`
-00002b40: 0000 0072 7400 0000 721f 0000 0072 5100  ...rt...r....rQ.
-00002b50: 0000 5a05 7061 7267 7372 5200 0000 5a06  ..Z.pargsrR...Z.
-00002b60: 5f5f 6172 6773 7271 0000 005a 0c6e 6577  __argsrq...Z.new
-00002b70: 6675 6e63 5f61 7267 735a 0c6f 7269 6675  func_argsZ.orifu
-00002b80: 6e63 5f61 7267 735a 0866 6974 5f66 756e  nc_argsZ.fit_fun
-00002b90: 63da 0769 6e64 6963 6573 5a07 6669 745f  c..indicesZ.fit_
-00002ba0: 6a61 635a 0670 305f 6669 7472 8400 0000  jacZ.p0_fitr....
-00002bb0: 7268 0000 0072 9800 0000 7299 0000 0072  rh...r....r....r
-00002bc0: 4400 0000 727b 0000 00da 0363 6f76 5a06  D...r{.....covZ.
-00002bd0: 7030 5f66 6978 5a06 6964 5f66 6978 da02  p0_fixZ.id_fix..
-00002be0: 6964 721b 0000 0072 1b00 0000 721c 0000  idr....r....r...
-00002bf0: 0072 7700 0000 3f01 0000 7360 0000 0000  .rw...?...s`....
-00002c00: 0b0e 0112 0308 011c 0108 011c 030e 0110  ................
-00002c10: ff08 030e 0112 ff08 0502 011c 0104 fe04  ................
-00002c20: 060a 0104 0110 ff04 0302 011c 0104 fe06  ................
-00002c30: 0504 031a 0b06 011e 010c 010e 0206 0106  ................
-00002c40: 0102 0106 0102 0102 0102 fa06 0914 0106  ................
-00002c50: 0314 010e 0a08 0104 0108 ff06 0316 0272  ...............r
-00002c60: 7700 0000 6304 0000 0000 0000 0000 0000  w...c...........
-00002c70: 000d 0000 0005 0000 0003 0000 0073 d800  .............s..
-00002c80: 0000 6401 6402 8400 8900 640a 8700 6601  ..d.d.....d...f.
-00002c90: 6404 6405 8409 7d04 640b 6406 6407 8401  d.d...}.d.d.d...
-00002ca0: 7d05 8800 7c01 8301 7d06 7c03 724a 7c04  }...|...}.|.rJ|.
-00002cb0: 7c01 7c06 7400 6408 1900 8303 5c02 7d07  |.|.t.d.....\.}.
-00002cc0: 7d08 6400 7d09 7c06 7d0a 6e7a 8800 7c02  }.d.}.|.}.nz..|.
-00002cd0: 8301 7d0b 7c06 7c0b 6b05 7290 7c04 7c01  ..}.|.|.k.r.|.|.
-00002ce0: 7c06 7400 6409 1900 7c06 1700 7c0b 1800  |.t.d...|...|...
-00002cf0: 8303 5c02 7d07 7d08 7c04 7c02 7c06 7400  ..\.}.}.|.|.|.t.
-00002d00: 6409 1900 8303 5c02 7d09 7d08 7c06 7d0a  d.....\.}.}.|.}.
-00002d10: 6e34 7c04 7c01 7c0b 7400 6409 1900 7c06  n4|.|.|.t.d...|.
-00002d20: 1700 7c0b 1800 8303 5c02 7d07 7d08 7c04  ..|.....\.}.}.|.
-00002d30: 7c02 7c0b 7400 6409 1900 8303 5c02 7d09  |.|.t.d.....\.}.
-00002d40: 7d08 7c0b 7d0a 7c00 7c05 7c07 7c0a 7c09  }.|.}.|.|.|.|.|.
-00002d50: 8303 1700 7d0c 7c0c 5300 290c 4e63 0100  ....}.|.S.).Nc..
-00002d60: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-00002d70: 0000 5300 0000 734e 0000 0064 017d 017c  ..S...sN...d.}.|
-00002d80: 0064 027c 019b 0064 039d 039b 047d 027c  .d.|...d.....}.|
-00002d90: 02a0 0064 03a1 0164 0417 007d 037c 027c  ...d...d...}.|.|
-00002da0: 0364 0585 0219 0064 066b 0272 3a74 0164  .d.....d.k.r:t.d
-00002db0: 0783 0153 0074 0174 027c 027c 0364 0585  ...S.t.t.|.|.d..
-00002dc0: 0219 0083 0183 0153 0029 087a 4472 6574  .......S.).zDret
-00002dd0: 7572 6e73 2074 6865 2065 7870 6f6e 656e  urns the exponen
-00002de0: 7420 6173 2061 6e20 696e 7420 6765 6e65  t as an int gene
-00002df0: 7261 7465 6420 6279 2074 6865 203a 2e65  rated by the :.e
-00002e00: 2066 6f72 6d61 7420 7370 6563 6966 6965   format specifie
-00002e10: 72e9 0500 0000 da01 2eda 0165 720a 0000  r..........er...
-00002e20: 004e da03 6e61 6e7a 032b 3030 2903 da04  .N..nanz.+00)...
-00002e30: 6669 6e64 728c 0000 0072 1900 0000 2904  findr....r....).
-00002e40: 7210 0000 00da 0464 6563 69da 0173 5a0a  r......deci..sZ.
-00002e50: 696e 6465 785f 7369 676e 721b 0000 0072  index_signr....r
-00002e60: 1b00 0000 721c 0000 00da 0c67 6574 5f65  ....r......get_e
-00002e70: 7870 6f6e 656e 74a0 0100 0073 0c00 0000  xponent....s....
-00002e80: 0002 0401 1001 0e03 1001 0801 7a25 7661  ............z%va
-00002e90: 6c75 655f 746f 5f73 7472 696e 672e 3c6c  lue_to_string.<l
-00002ea0: 6f63 616c 733e 2e67 6574 5f65 7870 6f6e  ocals>.get_expon
-00002eb0: 656e 7472 6900 0000 6303 0000 0000 0000  entri...c.......
-00002ec0: 0000 0000 0006 0000 0004 0000 0013 0000  ................
-00002ed0: 0073 5400 0000 7c02 7c01 1700 8800 7c00  .sT...|.|.....|.
-00002ee0: 8301 1800 6401 1800 7d03 7c03 6402 6b00  ....d...}.|.d.k.
-00002ef0: 7220 6402 7d03 7c00 6403 7c01 1300 1b00  r d.}.|.d.|.....
-00002f00: 6404 7c03 9b00 6405 9d03 9b04 7d04 6403  d.|...d.....}.d.
-00002f10: 7c01 1300 6406 9b04 6401 6407 8502 1900  |...d...d.d.....
-00002f20: 7d05 7c04 7c05 6602 5300 2908 6119 0100  }.|.|.f.S.).a...
-00002f30: 000a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002f40: 7320 6120 7374 7269 6e67 2072 6570 7265  s a string repre
-00002f50: 7365 6e74 6174 696f 6e20 696e 2073 6369  sentation in sci
-00002f60: 656e 7469 6669 6320 6e6f 7461 7469 6f6e  entific notation
-00002f70: 206f 6620 6120 6e75 6d62 6572 0a20 2020   of a number.   
-00002f80: 2020 2020 2073 7065 6369 6669 6564 2062       specified b
-00002f90: 7920 7661 6c75 652e 0a20 2020 2020 2020  y value..       
-00002fa0: 2076 616c 7565 3a20 7468 6520 6e75 6d62   value: the numb
-00002fb0: 6572 2074 6861 7420 6973 2063 6f6e 7665  er that is conve
-00002fc0: 7274 6564 0a20 2020 2020 2020 2065 7870  rted.        exp
-00002fd0: 6f6e 656e 743a 2074 6865 2065 7870 6f6e  onent: the expon
-00002fe0: 656e 7420 7573 6564 2066 6f72 2074 6865  ent used for the
-00002ff0: 2072 6570 7265 7365 6e74 6174 696f 6e0a   representation.
-00003000: 2020 2020 2020 2020 7369 675f 6469 6769          sig_digi
-00003010: 7473 3a20 7468 6520 6e75 6d62 6572 206f  ts: the number o
-00003020: 6620 7369 676e 6966 6963 616e 7420 6469  f significant di
-00003030: 6769 7473 2074 6861 7420 6973 2075 7365  gits that is use
-00003040: 640a 2020 2020 2020 2020 720a 0000 0072  d.        r....r
-00003050: 0100 0000 e90a 0000 0072 a800 0000 da01  .........r......
-00003060: 667a 032e 3065 4e72 1b00 0000 2906 7210  fz..0eNr....).r.
-00003070: 0000 00da 0865 7870 6f6e 656e 745a 0a73  .....exponentZ.s
-00003080: 6967 5f64 6967 6974 7372 ac00 0000 5a07  ig_digitsr....Z.
-00003090: 7265 7375 6c74 315a 0772 6573 756c 7432  result1Z.result2
-000030a0: a901 72ae 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000030b0: 00da 0f66 6c6f 6174 5f74 6f5f 7374 7269  ...float_to_stri
-000030c0: 6e67 ab01 0000 730c 0000 0000 0814 0108  ng....s.........
-000030d0: 0104 0118 0114 017a 2876 616c 7565 5f74  .......z(value_t
-000030e0: 6f5f 7374 7269 6e67 2e3c 6c6f 6361 6c73  o_string.<locals
-000030f0: 3e2e 666c 6f61 745f 746f 5f73 7472 696e  >.float_to_strin
-00003100: 6763 0300 0000 0000 0000 0000 0000 0400  gc..............
-00003110: 0000 0400 0000 5300 0000 735a 0000 007c  ......S...sZ...|
-00003120: 0264 0175 0072 0c64 026e 027c 027d 027c  .d.u.r.d.n.|.}.|
-00003130: 0272 3e7c 0264 036b 0372 3e64 047c 0017  .r>|.d.k.r>d.|..
-00003140: 0064 0517 007c 0217 0064 0617 0064 077c  .d...|...d...d.|
-00003150: 019b 0064 089d 0317 007d 036e 1864 097c  ...d.....}.n.d.|
-00003160: 0017 0064 0a17 0064 077c 019b 0064 089d  ...d...d.|...d..
-00003170: 0317 007d 037c 0353 0029 0b7a 9172 6574  ...}.|.S.).z.ret
-00003180: 7572 6e20 6120 6c61 7465 7820 7374 7269  urn a latex stri
-00003190: 6e67 0a20 2020 2020 2020 2028 7661 6c75  ng.        (valu
-000031a0: 655f 7374 7220 2b2f 2d20 6572 726f 725f  e_str +/- error_
-000031b0: 7374 7229 2078 2031 305e 2865 7870 6f6e  str) x 10^(expon
-000031c0: 656e 7429 0a20 2020 2020 2020 2063 6865  ent).        che
-000031d0: 636b 7320 666f 7220 6e61 6e20 6f72 204e  cks for nan or N
-000031e0: 6f6e 6520 746f 2070 7265 7665 6e74 2070  one to prevent p
-000031f0: 726f 6772 616d 2063 7261 7368 2070 6f73  rogram crash pos
-00003200: 7369 626c 790a 2020 2020 2020 2020 4eda  sibly.        N.
-00003210: 0130 72aa 0000 007a 0424 3d20 287a 035c  .0r....z.$= (z.\
-00003220: 706d 7a08 295c 7469 6d65 7324 7a05 2431  pmz.)\times$z.$1
-00003230: 305e 7b7a 027d 247a 0224 3d7a 075c 7469  0^{z.}$z.$=z.\ti
-00003240: 6d65 7324 721b 0000 0029 04da 0976 616c  mes$r....)...val
-00003250: 7565 5f73 7472 72b1 0000 00da 0965 7272  ue_strr......err
-00003260: 6f72 5f73 7472 5a0c 6c61 7465 785f 7374  or_strZ.latex_st
-00003270: 7269 6e67 721b 0000 0072 1b00 0000 721c  ringr....r....r.
-00003280: 0000 00da 0874 6f5f 6c61 7465 78ba 0100  .....to_latex...
-00003290: 0073 2200 0000 0005 1002 0c03 0201 02ff  .s".............
-000032a0: 0202 02fe 0203 02fd 0204 02fc 0205 0afb  ................
-000032b0: 02ff 040a 16ff 0203 7a21 7661 6c75 655f  ........z!value_
-000032c0: 746f 5f73 7472 696e 672e 3c6c 6f63 616c  to_string.<local
-000032d0: 733e 2e74 6f5f 6c61 7465 78da 1643 4d5f  s>.to_latex..CM_
-000032e0: 5349 475f 4449 4749 5453 5f4e 4f5f 4552  SIG_DIGITS_NO_ER
-000032f0: 524f 52da 0d43 4d5f 5349 475f 4449 4749  ROR..CM_SIG_DIGI
-00003300: 5453 2901 7269 0000 0029 014e 720b 0000  TS).ri...).Nr...
-00003310: 0029 0d72 0e00 0000 7210 0000 00da 0565  .).r....r......e
-00003320: 7272 6f72 7212 0000 0072 b300 0000 72b7  rrorr....r....r.
-00003330: 0000 005a 0378 5f65 72b5 0000 0072 9700  ...Z.x_er....r..
-00003340: 0000 72b6 0000 0072 b100 0000 5a04 6478  ..r....r....Z.dx
-00003350: 5f65 da08 636f 6d62 696e 6564 721b 0000  _e..combinedr...
-00003360: 0072 b200 0000 721c 0000 00da 0f76 616c  .r....r......val
-00003370: 7565 5f74 6f5f 7374 7269 6e67 9f01 0000  ue_to_string....
-00003380: 7338 0000 0000 0108 0b0e 0f0a 1708 0104  s8..............
-00003390: 0102 010a ff08 0304 0106 0208 0108 0102  ................
-000033a0: 0112 ff08 0302 010a ff08 0306 0202 0112  ................
-000033b0: ff08 0302 010a ff08 0304 0110 0272 bc00  .............r..
-000033c0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-000033d0: 0000 0004 0000 0043 0000 0073 1000 0000  .......C...s....
-000033e0: 7c00 6401 7c01 9b00 6402 9d03 9b04 5300  |.d.|...d.....S.
-000033f0: 2903 7a7e 0a20 2020 2072 6574 7572 6e20  ).z~.    return 
-00003400: 6120 7374 7269 6e67 2072 6570 7320 6f66  a string reps of
-00003410: 2061 2076 616c 7565 2069 6e20 7363 6965   a value in scie
-00003420: 6e74 6966 6963 206e 6f74 6174 696f 6e20  ntific notation 
-00003430: 7769 7468 2074 6865 206e 756d 6265 720a  with the number.
-00003440: 2020 2020 6f66 2073 6967 6e69 6669 6361      of significa
-00003450: 6e74 2064 6967 6974 7320 7370 6563 6966  nt digits specif
-00003460: 6965 6420 6279 2064 6967 6974 730a 2020  ied by digits.  
-00003470: 2020 7a02 312e 72a9 0000 0072 1b00 0000    z.1.r....r....
-00003480: 2902 7210 0000 00da 0664 6967 6974 7372  ).r......digitsr
-00003490: 1b00 0000 721b 0000 0072 1c00 0000 da0c  ....r....r......
-000034a0: 666c 6f61 745f 746f 5f73 7472 ef01 0000  float_to_str....
-000034b0: 7302 0000 0000 0572 be00 0000 6301 0000  s......r....c...
-000034c0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-000034d0: 0043 0000 0073 2000 0000 7c00 a000 6401  .C...s ...|...d.
-000034e0: a101 6402 6b04 721c 7c00 a001 6401 6403  ..d.k.r.|...d.d.
-000034f0: a102 7d00 7100 7c00 5300 2904 7a20 7265  ..}.q.|.S.).z re
-00003500: 6d6f 7665 7320 6c65 6164 696e 6720 7370  moves leading sp
-00003510: 6163 6573 2066 726f 6d20 7465 7874 7a05  aces from textz.
-00003520: 0a20 2020 2072 0100 0000 da01 0a29 02da  .    r.......)..
-00003530: 0563 6f75 6e74 da07 7265 706c 6163 6529  .count..replace)
-00003540: 01da 0474 6578 7472 1b00 0000 721b 0000  ...textr....r...
-00003550: 0072 1c00 0000 7270 0000 00f7 0100 0073  .r....rp.......s
-00003560: 0600 0000 0002 0e01 0e01 7270 0000 0029  ..........rp...)
-00003570: 1a72 6b00 0000 da0b 6461 7461 636c 6173  .rk.....dataclas
-00003580: 7365 7372 0200 0000 7203 0000 00da 0674  sesr....r......t
-00003590: 7970 696e 6772 0400 0000 7205 0000 00da  ypingr....r.....
-000035a0: 056e 756d 7079 7241 0000 005a 056c 6d66  .numpyrA...Z.lmf
-000035b0: 6974 7206 0000 00da 0573 6369 7079 7207  itr......scipyr.
-000035c0: 0000 00da 0e73 6369 7079 2e6f 7074 696d  .....scipy.optim
-000035d0: 697a 6572 0800 0000 7209 0000 00da 095f  izer....r......_
-000035e0: 7365 7474 696e 6773 720c 0000 0072 0d00  settingsr....r..
-000035f0: 0000 721d 0000 0072 3a00 0000 724c 0000  ..r....r:...rL..
-00003600: 0072 7700 0000 72bc 0000 0072 be00 0000  .rw...r....r....
-00003610: 7270 0000 0072 1b00 0000 721b 0000 0072  rp...r....r....r
-00003620: 1b00 0000 721c 0000 00da 083c 6d6f 6475  ....r......<modu
-00003630: 6c65 3e01 0000 0073 2800 0000 0801 1001  le>....s(.......
-00003640: 1002 0801 0c01 0c01 1002 0c03 0201 100b  ................
-00003650: 0201 1028 0201 1018 0e7f 0066 08ff 0c60  ...(.......f...`
-00003660: 0850 0808                                .P..
+00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
+00000060: 6401 6c08 5a09 6400 6404 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
+00000070: 0100 6400 6405 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6406 6c0e 6d0f 5a0f 6d10 5a10 0100 6407  d.l.m.Z.m.Z...d.
+00000090: 6408 6c11 6d12 5a12 0100 6502 4700 6409  d.l.m.Z...e.G.d.
+000000a0: 640a 8400 640a 8302 8301 5a13 6502 4700  d...d.....Z.e.G.
+000000b0: 640b 640c 8400 640c 8302 8301 5a14 6502  d.d...d.....Z.e.
+000000c0: 4700 640d 640e 8400 640e 8302 8301 5a15  G.d.d...d.....Z.
+000000d0: 4700 640f 6410 8400 6410 8302 5a16 6401  G.d.d...d...Z.d.
+000000e0: 6401 6411 6412 9c03 6413 6414 8402 5a17  d.d.d...d.d...Z.
+000000f0: 6415 6416 8400 5a18 6417 6418 8400 5a19  d.d...Z.d.d...Z.
+00000100: 6419 641a 8400 5a1a 6401 5300 291b e900  d.d...Z.d.S.)...
+00000110: 0000 004e 2902 da09 6461 7461 636c 6173  ...N)...dataclas
+00000120: 73da 0566 6965 6c64 2902 da03 416e 79da  s..field)...Any.
+00000130: 044c 6973 7429 01da 054d 6f64 656c 2901  .List)...Model).
+00000140: da05 7374 6174 7329 02da 0f4f 7074 696d  ..stats)...Optim
+00000150: 697a 6557 6172 6e69 6e67 da09 6375 7276  izeWarning..curv
+00000160: 655f 6669 74e9 0100 0000 a901 da08 7365  e_fit.........se
+00000170: 7474 696e 6773 6300 0000 0000 0000 0000  ttingsc.........
+00000180: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000190: 3e00 0000 6500 5a01 6400 5a02 5500 6401  >...e.Z.d.Z.U.d.
+000001a0: 5a03 6504 6505 6402 3c00 6403 5a06 6507  Z.e.e.d.<.d.Z.e.
+000001b0: 6505 6404 3c00 6405 5a08 6507 6505 6406  e.d.<.d.Z.e.e.d.
+000001c0: 3c00 6407 5a09 650a 6505 6408 3c00 6409  <.d.Z.e.e.d.<.d.
+000001d0: 5300 290a da0c 4669 7450 6172 616d 6574  S.)...FitParamet
+000001e0: 6572 7a1f 0a20 2020 2073 746f 7265 7320  erz..    stores 
+000001f0: 6120 6669 7470 6172 616d 6574 6572 0a20  a fitparameter. 
+00000200: 2020 20da 046e 616d 65e7 0000 0000 0000     ..name.......
+00000210: f03f da05 7661 6c75 6567 0000 0000 0000  .?..valueg......
+00000220: 0000 da05 7369 676d 6146 da05 6669 7865  ....sigmaF..fixe
+00000230: 644e 290b da08 5f5f 6e61 6d65 5f5f da0a  dN)...__name__..
+00000240: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000250: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000260: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
+00000270: 7469 6f6e 735f 5f72 1000 0000 da05 666c  tions__r......fl
+00000280: 6f61 7472 1100 0000 7212 0000 00da 0462  oatr....r......b
+00000290: 6f6f 6ca9 0072 1b00 0000 721b 0000 00fa  ool..r....r.....
+000002a0: 392f 5573 6572 732f 6b6f 6a6f 2f61 7070  9/Users/kojo/app
+000002b0: 732f 7365 6e69 6f72 5f70 726f 6a65 6374  s/senior_project
+000002c0: 5f75 7363 2f63 7572 7665 6669 7467 7569  _usc/curvefitgui
+000002d0: 2f5f 746f 6f6c 732e 7079 720d 0000 000e  /_tools.pyr.....
+000002e0: 0000 0073 0a00 0000 0a02 0404 0801 0c01  ...s............
+000002f0: 0c01 720d 0000 0063 0000 0000 0000 0000  ..r....c........
+00000300: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000310: 7360 0000 0065 005a 0164 005a 0255 0064  s`...e.Z.d.Z.U.d
+00000320: 015a 0365 0465 0564 023c 0065 0665 0564  .Z.e.e.d.<.e.e.d
+00000330: 033c 0065 0765 0819 0065 0564 043c 0064  .<.e.e...e.d.<.d
+00000340: 055a 0965 0665 0564 063c 0064 0764 089c  .Z.e.e.d.<.d.d..
+00000350: 0164 0964 0a84 045a 0a64 0b64 0c84 005a  .d.d...Z.d.d...Z
+00000360: 0b64 0d64 0e84 005a 0c64 0f64 1084 005a  .d.d...Z.d.d...Z
+00000370: 0d64 0753 0029 11da 0846 6974 4d6f 6465  .d.S.)...FitMode
+00000380: 6c7a 1a0a 2020 2020 7374 6f72 6573 2074  lz..    stores t
+00000390: 6865 206d 6f64 656c 0a20 2020 20da 0466  he model.    ..f
+000003a0: 756e 63da 0677 6569 6768 74da 0766 6974  unc..weight..fit
+000003b0: 7061 7273 da00 da0b 6465 7363 7269 7074  pars....descript
+000003c0: 696f 6e4e 2901 da06 7265 7475 726e 6301  ionN)...returnc.
+000003d0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000003e0: 0000 0043 0000 0073 4a00 0000 7400 7c00  ...C...sJ...t.|.
+000003f0: 6a01 8301 7c00 5f02 7c00 6a02 a003 a100  j...|._.|.j.....
+00000400: 7c00 5f04 7c00 6a05 4400 5d26 7d01 7c01  |._.|.j.D.]&}.|.
+00000410: 6a06 0c00 7c00 6a04 7c01 6a07 1900 5f08  j...|.j.|.j..._.
+00000420: 7c01 6a09 7c00 6a04 7c01 6a07 1900 5f09  |.j.|.j.|.j..._.
+00000430: 711e 6401 5300 2902 7a3a 0a20 2020 2020  q.d.S.).z:.     
+00000440: 2020 2049 6e69 7469 616c 697a 6573 206c     Initializes l
+00000450: 6d66 6974 206d 6f64 656c 2061 6e64 2070  mfit model and p
+00000460: 6172 6172 656d 6574 6572 730a 2020 2020  araremeters.    
+00000470: 2020 2020 4e29 0a72 0600 0000 721e 0000      N).r....r...
+00000480: 00da 0b6c 6d66 6974 5f6d 6f64 656c 5a0b  ...lmfit_modelZ.
+00000490: 6d61 6b65 5f70 6172 616d 73da 0a70 6172  make_params..par
+000004a0: 616d 6574 6572 7372 2000 0000 7212 0000  ametersr ...r...
+000004b0: 0072 0e00 0000 da04 7661 7279 7210 0000  .r......varyr...
+000004c0: 00a9 02da 0473 656c 66da 0370 6172 721b  .....self..parr.
+000004d0: 0000 0072 1b00 0000 721c 0000 00da 0d5f  ...r....r......_
+000004e0: 5f70 6f73 745f 696e 6974 5f5f 2700 0000  _post_init__'...
+000004f0: 730a 0000 0000 040c 060c 010a 0112 017a  s..............z
+00000500: 1646 6974 4d6f 6465 6c2e 5f5f 706f 7374  .FitModel.__post
+00000510: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00000520: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000530: 731e 0000 007c 006a 007c 0167 0164 0164  s....|.j.|.g.d.d
+00000540: 0284 007c 006a 0144 0083 01a2 0152 008e  ...|.j.D.....R..
+00000550: 0053 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+00000560: 0000 0002 0000 0002 0000 0073 0000 0073  ...........s...s
+00000570: 1400 0000 7c00 5d0c 7d01 7c01 6a00 5600  ....|.].}.|.j.V.
+00000580: 0100 7102 6400 5300 a901 4ea9 0172 1000  ..q.d.S...N..r..
+00000590: 0000 a902 da02 2e30 7229 0000 0072 1b00  .......0r)...r..
+000005a0: 0000 721b 0000 0072 1c00 0000 da09 3c67  ..r....r......<g
+000005b0: 656e 6578 7072 3e37 0000 00f3 0000 0000  enexpr>7........
+000005c0: 7a24 4669 744d 6f64 656c 2e65 7661 6c75  z$FitModel.evalu
+000005d0: 6174 652e 3c6c 6f63 616c 733e 2e3c 6765  ate.<locals>.<ge
+000005e0: 6e65 7870 723e 2902 721e 0000 0072 2000  nexpr>).r....r .
+000005f0: 0000 2902 7228 0000 00da 0178 721b 0000  ..).r(.....xr...
+00000600: 0072 1b00 0000 721c 0000 00da 0865 7661  .r....r......eva
+00000610: 6c75 6174 6536 0000 0073 0200 0000 0001  luate6...s......
+00000620: 7a11 4669 744d 6f64 656c 2e65 7661 6c75  z.FitModel.evalu
+00000630: 6174 6563 0100 0000 0000 0000 0000 0000  atec............
+00000640: 0100 0000 0300 0000 4300 0000 7314 0000  ........C...s...
+00000650: 0074 0064 0164 0284 007c 006a 0144 0083  .t.d.d...|.j.D..
+00000660: 0183 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
+00000670: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00000680: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
+00000690: 6a00 0c00 9102 7104 5300 721b 0000 00a9  j.....q.S.r.....
+000006a0: 0172 1200 0000 722d 0000 0072 1b00 0000  .r....r-...r....
+000006b0: 721b 0000 0072 1c00 0000 da0a 3c6c 6973  r....r......<lis
+000006c0: 7463 6f6d 703e 3a00 0000 7230 0000 007a  tcomp>:...r0...z
+000006d0: 2b46 6974 4d6f 6465 6c2e 6765 745f 6e75  +FitModel.get_nu
+000006e0: 6d66 6974 7061 7273 2e3c 6c6f 6361 6c73  mfitpars.<locals
+000006f0: 3e2e 3c6c 6973 7463 6f6d 703e 2902 da03  >.<listcomp>)...
+00000700: 7375 6d72 2000 0000 a901 7228 0000 0072  sumr .....r(...r
+00000710: 1b00 0000 721b 0000 0072 1c00 0000 da0e  ....r....r......
+00000720: 6765 745f 6e75 6d66 6974 7061 7273 3900  get_numfitpars9.
+00000730: 0000 7302 0000 0000 017a 1746 6974 4d6f  ..s......z.FitMo
+00000740: 6465 6c2e 6765 745f 6e75 6d66 6974 7061  del.get_numfitpa
+00000750: 7273 6301 0000 0000 0000 0000 0000 0002  rsc.............
+00000760: 0000 0004 0000 0043 0000 0073 3200 0000  .......C...s2...
+00000770: 7c00 6a00 4400 5d26 7d01 7c01 6a01 0c00  |.j.D.]&}.|.j...
+00000780: 7c00 6a02 7c01 6a03 1900 5f04 7c01 6a05  |.j.|.j..._.|.j.
+00000790: 7c00 6a02 7c01 6a03 1900 5f05 7106 6400  |.j.|.j..._.q.d.
+000007a0: 5300 722b 0000 0029 0672 2000 0000 7212  S.r+...).r ...r.
+000007b0: 0000 0072 2500 0000 720e 0000 0072 2600  ...r%...r....r&.
+000007c0: 0000 7210 0000 0072 2700 0000 721b 0000  ..r....r'...r...
+000007d0: 0072 1b00 0000 721c 0000 00da 0675 7064  .r....r......upd
+000007e0: 6174 653c 0000 0073 0600 0000 0001 0a01  ate<...s........
+000007f0: 1201 7a0f 4669 744d 6f64 656c 2e75 7064  ..z.FitModel.upd
+00000800: 6174 6529 0e72 1300 0000 7214 0000 0072  ate).r....r....r
+00000810: 1500 0000 7216 0000 0072 0400 0000 7218  ....r....r....r.
+00000820: 0000 0072 1700 0000 7205 0000 0072 0d00  ...r....r....r..
+00000830: 0000 7222 0000 0072 2a00 0000 7232 0000  ..r"...r*...r2..
+00000840: 0072 3700 0000 7238 0000 0072 1b00 0000  .r7...r8...r....
+00000850: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000860: 1d00 0000 1a00 0000 7312 0000 000a 0204  ........s.......
+00000870: 0408 0108 030c 010c 020e 0f08 0308 0372  ...............r
+00000880: 1d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000890: 0000 0000 0003 0000 0040 0000 0073 7400  .........@...st.
+000008a0: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
+000008b0: 6505 6401 3c00 6503 6a04 6505 6402 3c00  e.d.<.e.j.e.d.<.
+000008c0: 6403 5a06 6503 6a04 6505 6404 3c00 6403  d.Z.e.j.e.d.<.d.
+000008d0: 5a07 6503 6a04 6505 6405 3c00 6508 6406  Z.e.j.e.d.<.e.d.
+000008e0: 6407 8d01 5a09 650a 650b 1900 6505 6408  d...Z.e.e...e.d.
+000008f0: 3c00 6409 640a 8400 5a0c 640b 640c 8400  <.d.d...Z.d.d...
+00000900: 5a0d 640d 640e 8400 5a0e 640f 6410 8400  Z.d.d...Z.d.d...
+00000910: 5a0f 6403 5300 2911 da07 4669 7444 6174  Z.d.S.)...FitDat
+00000920: 6172 3100 0000 da01 794e da02 7865 da02  ar1.....yN..xe..
+00000930: 7965 4629 01da 0469 6e69 74da 046d 6173  yeF)...init..mas
+00000940: 6b63 0100 0000 0000 0000 0000 0000 0100  kc..............
+00000950: 0000 0400 0000 4300 0000 7316 0000 007c  ......C...s....|
+00000960: 00a0 0074 016a 020b 0074 016a 02a1 0201  ...t.j...t.j....
+00000970: 0064 0053 0072 2b00 0000 2903 da08 7365  .d.S.r+...)...se
+00000980: 745f 6d61 736b da02 6e70 da03 696e 6672  t_mask..np..infr
+00000990: 3600 0000 721b 0000 0072 1b00 0000 721c  6...r....r....r.
+000009a0: 0000 0072 2a00 0000 4a00 0000 7302 0000  ...r*...J...s...
+000009b0: 0000 017a 1546 6974 4461 7461 2e5f 5f70  ...z.FitData.__p
+000009c0: 6f73 745f 696e 6974 5f5f 6301 0000 0000  ost_init__c.....
+000009d0: 0000 0000 0000 0002 0000 0005 0000 0003  ................
+000009e0: 0000 0073 2600 0000 8700 6601 6401 6402  ...s&.....f.d.d.
+000009f0: 8408 8800 6a00 8800 6a01 8800 6a02 8800  ....j...j...j...
+00000a00: 6a03 6604 4400 8301 7d01 7c01 5300 2903  j.f.D...}.|.S.).
+00000a10: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00000a20: 0000 0300 0000 3300 0000 7324 0000 007c  ......3...s$...|
+00000a30: 005d 1c7d 017c 0164 0075 0172 187c 0188  .].}.|.d.u.r.|..
+00000a40: 006a 0019 006e 0264 0056 0001 0071 0264  .j...n.d.V...q.d
+00000a50: 0053 0072 2b00 0000 2901 723e 0000 0029  .S.r+...).r>...)
+00000a60: 0272 2e00 0000 da03 7661 7272 3600 0000  .r......varr6...
+00000a70: 721b 0000 0072 1c00 0000 722f 0000 004e  r....r....r/...N
+00000a80: 0000 0073 0400 0000 0402 02ff 7a1e 4669  ...s........z.Fi
+00000a90: 7444 6174 612e 6765 742e 3c6c 6f63 616c  tData.get.<local
+00000aa0: 733e 2e3c 6765 6e65 7870 723e 2904 7231  s>.<genexpr>).r1
+00000ab0: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
+00000ac0: 0000 2902 7228 0000 00da 0672 6573 756c  ..).r(.....resul
+00000ad0: 7472 1b00 0000 7236 0000 0072 1c00 0000  tr....r6...r....
+00000ae0: da03 6765 744d 0000 0073 0800 0000 0001  ..getM...s......
+00000af0: 0a02 12fe 0604 7a0b 4669 7444 6174 612e  ......z.FitData.
+00000b00: 6765 7463 0300 0000 0000 0000 0000 0000  getc............
+00000b10: 0300 0000 0300 0000 0300 0000 731c 0000  ............s...
+00000b20: 0087 0087 0166 0264 0164 0284 087c 006a  .....f.d.d...|.j
+00000b30: 0044 0083 017c 005f 0164 0053 0029 034e  .D...|._.d.S.).N
+00000b40: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000b50: 0005 0000 0013 0000 0073 2400 0000 6700  .........s$...g.
+00000b60: 7c00 5d1c 7d01 8801 7c01 0400 0300 6b01  |.].}...|.....k.
+00000b70: 6f1a 8800 6b01 6e04 0200 0100 9102 7104  o...k.n.......q.
+00000b80: 5300 721b 0000 0072 1b00 0000 2902 722e  S.r....r....).r.
+00000b90: 0000 0072 3100 0000 a902 da04 786d 6178  ...r1.......xmax
+00000ba0: da04 786d 696e 721b 0000 0072 1c00 0000  ..xminr....r....
+00000bb0: 7234 0000 0055 0000 0072 3000 0000 7a24  r4...U...r0...z$
+00000bc0: 4669 7444 6174 612e 7365 745f 6d61 736b  FitData.set_mask
+00000bd0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000be0: 6f6d 703e 2902 7231 0000 0072 3e00 0000  omp>).r1...r>...
+00000bf0: 2903 7228 0000 0072 4700 0000 7246 0000  ).r(...rG...rF..
+00000c00: 0072 1b00 0000 7245 0000 0072 1c00 0000  .r....rE...r....
+00000c10: 723f 0000 0054 0000 0073 0200 0000 0001  r?...T...s......
+00000c20: 7a10 4669 7444 6174 612e 7365 745f 6d61  z.FitData.set_ma
+00000c30: 736b 6301 0000 0000 0000 0000 0000 0001  skc.............
+00000c40: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
+00000c50: 7400 7c00 6a01 7c00 6a02 1900 8301 5300  t.|.j.|.j.....S.
+00000c60: 722b 0000 0029 03da 036c 656e 7231 0000  r+...)...lenr1..
+00000c70: 0072 3e00 0000 7236 0000 0072 1b00 0000  .r>...r6...r....
+00000c80: 721b 0000 0072 1c00 0000 da10 6765 745f  r....r......get_
+00000c90: 6e75 6d66 6974 706f 696e 7473 5700 0000  numfitpointsW...
+00000ca0: 7302 0000 0000 017a 1846 6974 4461 7461  s......z.FitData
+00000cb0: 2e67 6574 5f6e 756d 6669 7470 6f69 6e74  .get_numfitpoint
+00000cc0: 7329 1072 1300 0000 7214 0000 0072 1500  s).r....r....r..
+00000cd0: 0000 7240 0000 00da 0561 7272 6179 7218  ..r@.....arrayr.
+00000ce0: 0000 0072 3b00 0000 723c 0000 0072 0300  ...r;...r<...r..
+00000cf0: 0000 723e 0000 0072 0500 0000 721a 0000  ..r>...r....r...
+00000d00: 0072 2a00 0000 7244 0000 0072 3f00 0000  .r*...rD...r?...
+00000d10: 7249 0000 0072 1b00 0000 721b 0000 0072  rI...r....r....r
+00000d20: 1b00 0000 721c 0000 0072 3900 0000 4200  ....r....r9...B.
+00000d30: 0000 7312 0000 000a 020a 010a 010e 010e  ..s.............
+00000d40: 0116 0208 0308 0708 0372 3900 0000 6300  .........r9...c.
+00000d50: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000d60: 0000 0040 0000 0073 9e00 0000 6500 5a01  ...@...s....e.Z.
+00000d70: 6400 5a02 6401 5a03 6402 5a04 6403 6404  d.Z.d.Z.d.Z.d.d.
+00000d80: 8400 5a05 6405 6406 8400 5a06 6407 6408  ..Z.d.d...Z.d.d.
+00000d90: 8400 5a07 6409 640a 8400 5a08 640b 640b  ..Z.d.d...Z.d.d.
+00000da0: 6509 640c 1900 6603 640d 640e 8401 5a0a  e.d...f.d.d...Z.
+00000db0: 640f 6410 8400 5a0b 640b 640b 6509 640c  d.d...Z.d.d.e.d.
+00000dc0: 1900 6603 6411 6412 8401 5a0c 6422 6414  ..f.d.d...Z.d"d.
+00000dd0: 6415 8401 5a0d 6416 6417 8400 5a0e 6418  d...Z.d.d...Z.d.
+00000de0: 6419 8400 5a0f 641a 641b 8400 5a10 641c  d...Z.d.d...Z.d.
+00000df0: 641d 8400 5a11 641e 641f 8400 5a12 6420  d...Z.d.d...Z.d 
+00000e00: 6421 8400 5a13 640b 5300 2923 da06 4669  d!..Z.d.S.)#..Fi
+00000e10: 7474 6572 7a17 636c 6173 7320 746f 2068  tterz.class to h
+00000e20: 616e 646c 6520 7468 6520 6669 7429 03da  andle the fit)..
+00000e30: 046e 6f6e 65da 0872 656c 6174 6976 65da  .none..relative.
+00000e40: 0861 6273 6f6c 7574 6563 0a00 0000 0000  .absolutec......
+00000e50: 0000 0000 0000 0b00 0000 0600 0000 4b00  ..............K.
+00000e60: 0000 7370 0000 007c 0a7c 005f 007c 00a0  ..sp...|.|._.|..
+00000e70: 017c 027c 037c 047c 05a1 047c 005f 027c  .|.|.|.|...|._.|
+00000e80: 00a0 037c 017c 067c 07a1 037c 005f 0464  ...|.|.|...|._.d
+00000e90: 007c 005f 0564 017c 005f 0664 007c 005f  .|._.d.|._.d.|._
+00000ea0: 0769 007c 005f 087c 097c 005f 0964 027c  .i.|._.|.|._.d.|
+00000eb0: 005f 0a64 037c 0a76 0072 5e7c 0a64 0319  ._.d.|.v.r^|.d..
+00000ec0: 007c 005f 0a74 0ba0 0c7c 006a 04a1 017c  .|._.t...|.j...|
+00000ed0: 005f 0d64 0053 0029 044e 46da 076c 6561  ._.d.S.).NF..lea
+00000ee0: 7374 7371 da06 6d65 7468 6f64 290e da06  stsq..method)...
+00000ef0: 6b77 6172 6773 da0a 5f69 6e69 745f 6461  kwargs.._init_da
+00000f00: 7461 da04 6461 7461 da0b 5f69 6e69 745f  ta..data.._init_
+00000f10: 6d6f 6465 6cda 056d 6f64 656c da0c 6d6f  model..model..mo
+00000f20: 6465 6c5f 7265 7375 6c74 da0c 6669 745f  del_result..fit_
+00000f30: 6973 5f76 616c 6964 da12 6d65 616e 5f73  is_valid..mean_s
+00000f40: 7175 6172 6564 5f65 7272 6f72 da09 6669  quared_error..fi
+00000f50: 7472 6570 6f72 74da 0a69 735f 636f 6d70  treport..is_comp
+00000f60: 6c65 7872 5000 0000 da04 636f 7079 da08  lexrP.....copy..
+00000f70: 6465 6570 636f 7079 5a0a 6f72 6967 5f6d  deepcopyZ.orig_m
+00000f80: 6f64 656c 290b 7228 0000 0072 1e00 0000  odel).r(...r....
+00000f90: da05 7864 6174 61da 0579 6461 7461 da04  ..xdata..ydata..
+00000fa0: 7865 7272 da04 7965 7272 da02 7030 da0e  xerr..yerr..p0..
+00000fb0: 6162 736f 6c75 7465 5f73 6967 6d61 da03  absolute_sigma..
+00000fc0: 6a61 6372 5a00 0000 7251 0000 0072 1b00  jacrZ...rQ...r..
+00000fd0: 0000 721b 0000 0072 1c00 0000 da08 5f5f  ..r....r......__
+00000fe0: 696e 6974 5f5f 6000 0000 7318 0000 0000  init__`...s.....
+00000ff0: 0e06 0112 0110 0206 0106 0106 0106 0106  ................
+00001000: 0106 0108 010a 017a 0f46 6974 7465 722e  .......z.Fitter.
+00001010: 5f5f 696e 6974 5f5f 6305 0000 0000 0000  __init__c.......
+00001020: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
+00001030: 0073 b600 0000 7c01 7c02 6602 4400 5d1a  .s....|.|.f.D.].
+00001040: 7d05 7400 7c05 8301 7401 6a02 7501 7208  }.t.|...t.j.u.r.
+00001050: 7403 6401 8301 8201 7108 7404 7c01 8301  t.d.....q.t.|...
+00001060: 7404 7c02 8301 6b03 723c 7403 6402 8301  t.|...k.r<t.d...
+00001070: 8201 7c04 6400 7501 7272 7400 7c04 8301  ..|.d.u.rrt.|...
+00001080: 7401 6a02 7501 725a 7403 6401 8301 8201  t.j.u.rZt.d.....
+00001090: 7404 7c04 8301 7404 7c02 8301 6b03 7272  t.|...t.|...k.rr
+000010a0: 7403 6403 8301 8201 7c03 6400 7501 72a8  t.d.....|.d.u.r.
+000010b0: 7400 7c03 8301 7401 6a02 7501 7290 7403  t.|...t.j.u.r.t.
+000010c0: 6401 8301 8201 7404 7c03 8301 7404 7c01  d.....t.|...t.|.
+000010d0: 8301 6b03 72a8 7403 6404 8301 8201 7405  ..k.r.t.d.....t.
+000010e0: 7c01 7c02 7c03 7c04 8304 5300 2905 4e7a  |.|.|.|...S.).Nz
+000010f0: 2164 6174 6120 7368 6f75 6c64 2068 6176  !data should hav
+00001100: 6520 7479 7065 206e 756d 7079 2061 7272  e type numpy arr
+00001110: 6179 7a29 7864 6174 6120 616e 6420 7964  ayz)xdata and yd
+00001120: 6174 6120 7368 6f75 6c64 2062 6520 6f66  ata should be of
+00001130: 2065 7175 616c 206c 656e 6774 687a 2879   equal lengthz(y
+00001140: 6572 7220 616e 6420 7964 6174 6120 7368  err and ydata sh
+00001150: 6f75 6c64 2062 6520 6f66 2065 7175 616c  ould be of equal
+00001160: 206c 656e 6774 687a 2878 6572 7220 616e   lengthz(xerr an
+00001170: 6420 7864 6174 6120 7368 6f75 6c64 2062  d xdata should b
+00001180: 6520 6f66 2065 7175 616c 206c 656e 6774  e of equal lengt
+00001190: 6829 06da 0474 7970 6572 4000 0000 da07  h)...typer@.....
+000011a0: 6e64 6172 7261 79da 0945 7863 6570 7469  ndarray..Excepti
+000011b0: 6f6e 7248 0000 0072 3900 0000 2906 7228  onrH...r9...).r(
+000011c0: 0000 0072 3100 0000 723a 0000 0072 3b00  ...r1...r:...r;.
+000011d0: 0000 723c 0000 0072 4200 0000 721b 0000  ..r<...rB...r...
+000011e0: 0072 1b00 0000 721c 0000 0072 5200 0000  .r....r....rR...
+000011f0: 7c00 0000 7320 0000 0000 030c 010e 010a  |...s ..........
+00001200: 0110 0108 0308 010e 0108 0110 0108 0208  ................
+00001210: 010e 0108 0110 0108 027a 1146 6974 7465  .........z.Fitte
+00001220: 722e 5f69 6e69 745f 6461 7461 6304 0000  r._init_datac...
+00001230: 0000 0000 0000 0000 000a 0000 0005 0000  ................
+00001240: 0043 0000 0073 c600 0000 7400 7c01 8301  .C...s....t.|...
+00001250: 7310 7401 6401 8301 8201 7402 a003 7c01  s.t.d.....t...|.
+00001260: a101 6a04 7d04 6402 6403 8400 7c04 a005  ..j.}.d.d...|...
+00001270: a100 4400 8301 7d05 7c02 6400 7500 724c  ..D...}.|.d.u.rL
+00001280: 6404 6701 7406 7c05 6405 6400 8502 1900  d.g.t.|.d.d.....
+00001290: 8301 1400 7d02 6406 6403 8400 7407 7c05  ....}.d.d...t.|.
+000012a0: 6405 6400 8502 1900 7c02 8302 4400 8301  d.d.....|...D...
+000012b0: 7d06 7c00 6a08 6a09 6400 7501 7290 7c03  }.|.j.j.d.u.r.|.
+000012c0: 7284 7c00 6a0a 6407 1900 7d07 719a 7c00  r.|.j.d...}.q.|.
+000012d0: 6a0a 6405 1900 7d07 6e0a 7c00 6a0a 6408  j.d...}.n.|.j.d.
+000012e0: 1900 7d07 7c01 6a0b 6400 7500 72aa 6409  ..}.|.j.d.u.r.d.
+000012f0: 7d08 6e0a 740c 7c01 6a0b 8301 7d08 740d  }.n.t.|.j...}.t.
+00001300: 7c01 7c07 7c06 7c08 8304 7d09 7c09 5300  |.|.|.|...}.|.S.
+00001310: 290a 4e7a 184e 6f74 2061 2076 616c 6964  ).Nz.Not a valid
+00001320: 2066 6974 2066 756e 6374 696f 6e63 0100   fit functionc..
+00001330: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001340: 0000 5300 0000 7312 0000 0067 007c 005d  ..S...s....g.|.]
+00001350: 0a7d 017c 016a 0091 0271 0453 0072 1b00  .}.|.j...q.S.r..
+00001360: 0000 a901 720e 0000 00a9 0272 2e00 0000  ....r......r....
+00001370: da03 6172 6772 1b00 0000 721b 0000 0072  ..argr....r....r
+00001380: 1c00 0000 7234 0000 009b 0000 0072 3000  ....r4.......r0.
+00001390: 0000 7a26 4669 7474 6572 2e5f 696e 6974  ..z&Fitter._init
+000013a0: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
+000013b0: 3c6c 6973 7463 6f6d 703e 720f 0000 0072  <listcomp>r....r
+000013c0: 0a00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000013d0: 0003 0000 0005 0000 0053 0000 0073 1a00  .........S...s..
+000013e0: 0000 6700 7c00 5d12 5c02 7d01 7d02 7400  ..g.|.].\.}.}.t.
+000013f0: 7c01 7c02 8302 9102 7104 5300 721b 0000  |.|.....q.S.r...
+00001400: 0029 0172 0d00 0000 2903 722e 0000 0072  .).r....).r....r
+00001410: 6a00 0000 7210 0000 0072 1b00 0000 721b  j...r....r....r.
+00001420: 0000 0072 1c00 0000 7234 0000 00a2 0000  ...r....r4......
+00001430: 0073 0200 0000 0601 e902 0000 0072 0100  .s...........r..
+00001440: 0000 7a10 6e6f 2069 6e66 6f20 6f6e 206d  ..z.no info on m
+00001450: 6f64 656c 290e da08 6361 6c6c 6162 6c65  odel)...callable
+00001460: 7267 0000 00da 0769 6e73 7065 6374 da09  rg.....inspect..
+00001470: 7369 676e 6174 7572 6572 2500 0000 da06  signaturer%.....
+00001480: 7661 6c75 6573 7248 0000 00da 037a 6970  valuesrH.....zip
+00001490: 7253 0000 0072 3c00 0000 da0d 5745 4947  rS...r<.....WEIG
+000014a0: 4854 4f50 5449 4f4e 5372 1600 0000 da14  HTOPTIONSr......
+000014b0: 7374 7269 705f 6c65 6164 696e 675f 7370  strip_leading_sp
+000014c0: 6163 6573 721d 0000 0029 0a72 2800 0000  acesr....).r(...
+000014d0: 721e 0000 0072 6100 0000 7262 0000 005a  r....ra...rb...Z
+000014e0: 0d5f 4669 7474 6572 5f5f 6172 6773 da04  ._Fitter__args..
+000014f0: 6172 6773 7220 0000 0072 1f00 0000 7222  argsr ...r....r"
+00001500: 0000 005a 0961 6669 746d 6f64 656c 721b  ...Z.afitmodelr.
+00001510: 0000 0072 1b00 0000 721c 0000 0072 5400  ...r....r....rT.
+00001520: 0000 9400 0000 7326 0000 0000 0208 0108  ......s&........
+00001530: 030c 0112 0308 0116 0306 0110 ff06 050c  ................
+00001540: 0104 010c 020c 020a 030a 0106 020a 020e  ................
+00001550: 017a 1246 6974 7465 722e 5f69 6e69 745f  .z.Fitter._init_
+00001560: 6d6f 6465 6c63 0100 0000 0000 0000 0000  modelc..........
+00001570: 0000 0f00 0000 0a00 0000 4300 0000 7332  ..........C...s2
+00001580: 0100 0064 0164 0284 007c 006a 006a 0144  ...d.d...|.j.j.D
+00001590: 0083 017d 0164 0364 0284 007c 006a 006a  ...}.d.d...|.j.j
+000015a0: 0144 0083 017d 027c 006a 02a0 03a1 005c  .D...}.|.j.....\
+000015b0: 047d 037d 047d 057d 067c 006a 00a0 04a1  .}.}.}.}.|.j....
+000015c0: 0064 046b 0272 4c74 0564 0583 0182 017c  .d.k.rLt.d.....|
+000015d0: 00a0 06a1 0064 046b 0172 6074 0564 0683  .....d.k.r`t.d..
+000015e0: 0182 017c 006a 006a 077c 006a 0864 0719  ...|.j.j.|.j.d..
+000015f0: 006b 027d 077c 006a 006a 077c 006a 0864  .k.}.|.j.j.|.j.d
+00001600: 0419 006b 0272 9274 09a0 0a74 0b7c 0483  ...k.r.t...t.|..
+00001610: 01a1 017d 0674 0c7c 006a 007c 037c 047c  ...}.t.|.j.|.|.|
+00001620: 067c 017c 027c 006a 0d7c 0764 088d 085c  .|.|.|.j.|.d...\
+00001630: 037d 087d 097d 0a7c 0a7c 005f 0e64 097c  .}.}.}.|.|._.d.|
+00001640: 005f 0f74 1064 0a7c 0983 0201 0074 09a0  ._.t.d.|.....t..
+00001650: 1174 09a0 127c 09a1 01a1 017d 0b74 137c  .t...|.....}.t.|
+00001660: 006a 006a 017c 087c 0b83 0344 005d 165c  .j.j.|.|...D.].\
+00001670: 037d 0c7d 0d7d 0e7c 0d7c 0c5f 147c 0e7c  .}.}.}.|.|._.|.|
+00001680: 0c5f 1571 ea74 167c 047c 006a 00a0 177c  ._.q.t.|.|.j...|
+00001690: 03a1 0118 007c 061b 0064 0713 0083 017c  .....|...d.....|
+000016a0: 005f 187c 00a0 19a1 0001 007c 087c 097c  ._.|.......|.|.|
+000016b0: 0a66 0353 0029 0b7a 220a 2020 2020 2020  .f.S.).z".      
+000016c0: 2020 7065 7266 6f72 6d73 2074 6865 2066    performs the f
+000016d0: 6974 0a20 2020 2020 2020 2063 0100 0000  it.        c....
+000016e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000016f0: 5300 0000 7312 0000 0067 007c 005d 0a7d  S...s....g.|.].}
+00001700: 017c 016a 0091 0271 0453 0072 1b00 0000  .|.j...q.S.r....
+00001710: 722c 0000 00a9 0272 2e00 0000 da06 6669  r,.....r......fi
+00001720: 7470 6172 721b 0000 0072 1b00 0000 721c  tparr....r....r.
+00001730: 0000 0072 3400 0000 bd00 0000 7230 0000  ...r4.......r0..
+00001740: 007a 1e46 6974 7465 722e 6669 742e 3c6c  .z.Fitter.fit.<l
+00001750: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001760: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00001770: 0000 0300 0000 5300 0000 7312 0000 0067  ......S...s....g
+00001780: 007c 005d 0a7d 017c 016a 0091 0271 0453  .|.].}.|.j...q.S
+00001790: 0072 1b00 0000 7233 0000 0072 7400 0000  .r....r3...rt...
+000017a0: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+000017b0: 3400 0000 be00 0000 7230 0000 0072 0100  4.......r0...r..
+000017c0: 0000 7a2e 5468 6572 6520 7368 6f75 6c64  ..z.There should
+000017d0: 2062 6520 6174 206c 6561 7374 206f 6e65   be at least one
+000017e0: 2066 7265 6520 6669 7470 6172 616d 6574   free fitparamet
+000017f0: 6572 7a98 5468 6520 6e75 6d62 6572 206f  erz.The number o
+00001800: 6620 6465 6772 6565 7320 6f66 2066 7265  f degrees of fre
+00001810: 6564 6f6d 2028 646f 6629 2073 686f 756c  edom (dof) shoul
+00001820: 6420 6265 2061 7420 6c65 6173 7420 6f6e  d be at least on
+00001830: 652e 2054 7279 2074 6f20 696e 6372 6561  e. Try to increa
+00001840: 7365 2074 6865 206e 756d 6265 7220 6f66  se the number of
+00001850: 2064 6174 6170 6f69 6e74 7320 6f72 2074   datapoints or t
+00001860: 6f20 6465 6372 6561 7365 2074 6865 206e  o decrease the n
+00001870: 756d 6265 7220 6f66 2066 7265 6520 6669  umber of free fi
+00001880: 7470 6172 616d 6574 6572 732e 726b 0000  tparameters.rk..
+00001890: 0029 0572 1100 0000 7261 0000 00da 0270  .).r....ra.....p
+000018a0: 4672 5000 0000 7262 0000 0054 da03 636f  FrP...rb...T..co
+000018b0: 7629 1a72 5500 0000 7220 0000 0072 5300  v).rU...r ...rS.
+000018c0: 0000 7244 0000 0072 3700 0000 7208 0000  ..rD...r7...r...
+000018d0: 00da 135f 6465 6772 6565 735f 6f66 5f66  ..._degrees_of_f
+000018e0: 7265 6564 6f6d 721f 0000 0072 7100 0000  reedomr....rq...
+000018f0: 7240 0000 00da 046f 6e65 7372 4800 0000  r@.....onesrH...
+00001900: da11 6375 7276 655f 6669 745f 7772 6170  ..curve_fit_wrap
+00001910: 7065 7272 5000 0000 7256 0000 0072 5700  perrP...rV...rW.
+00001920: 0000 da05 7072 696e 74da 0473 7172 74da  ....print..sqrt.
+00001930: 0464 6961 6772 7000 0000 7210 0000 0072  .diagrp...r....r
+00001940: 1100 0000 7235 0000 0072 3200 0000 7258  ....r5...r2...rX
+00001950: 0000 00da 0e5f 6372 6561 7465 5f72 6570  ....._create_rep
+00001960: 6f72 7429 0f72 2800 0000 7261 0000 0072  ort).r(...ra...r
+00001970: 7600 0000 7231 0000 0072 3a00 0000 723b  v...r1...r:...r;
+00001980: 0000 0072 3c00 0000 7262 0000 00da 0470  ...r<...rb.....p
+00001990: 6f70 74da 0470 636f 7672 4300 0000 5a09  opt..pcovrC...Z.
+000019a0: 7374 6465 7272 6f72 7372 7500 0000 7210  stderrorsru...r.
+000019b0: 0000 00da 0673 7464 6572 7272 1b00 0000  .....stderrr....
+000019c0: 721b 0000 0072 1c00 0000 da03 6669 74b8  r....r......fit.
+000019d0: 0000 0073 4400 0000 0005 1201 1202 1203  ...sD...........
+000019e0: 0e01 0201 02ff 0404 0c01 0201 02ff 0405  ................
+000019f0: 1201 1201 0e02 0201 0401 0201 0201 0201  ................
+00001a00: 0201 0201 0401 02f8 0c0b 0603 0601 0a01  ................
+00001a10: 1001 1a01 0601 0802 1e02 0801 7a0a 4669  ............z.Fi
+00001a20: 7474 6572 2e66 6974 4eda 0f4d 4f44 454c  tter.fitN..MODEL
+00001a30: 5f4e 554d 504f 494e 5453 6304 0000 0000  _NUMPOINTSc.....
+00001a40: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
+00001a50: 0000 0073 7000 0000 7c01 6400 7500 7214  ...sp...|.d.u.r.
+00001a60: 7c00 6a00 6a01 a002 a100 7d01 7c02 6400  |.j.j.....}.|.d.
+00001a70: 7500 7228 7c00 6a00 6a01 a003 a100 7d02  u.r(|.j.j.....}.
+00001a80: 7404 a005 7c01 7c02 7c03 a103 7d04 7c00  t...|.|.|...}.|.
+00001a90: 6a06 7354 7c00 6a07 6a08 6a09 7c00 6a07  j.sT|.j.j.j.|.j.
+00001aa0: 6a0a 7c04 6401 8d02 7d05 6e14 7c00 6a06  j.|.d...}.n.|.j.
+00001ab0: 6a09 7c00 6a06 6a0b 7c04 6401 8d02 7d05  j.|.j.j.|.d...}.
+00001ac0: 7c04 7c05 6602 5300 2902 4e29 0172 3100  |.|.f.S.).N).r1.
+00001ad0: 0000 290c 7253 0000 0072 3100 0000 da03  ..).rS...r1.....
+00001ae0: 6d69 6eda 036d 6178 7240 0000 00da 086c  min..maxr@.....l
+00001af0: 696e 7370 6163 6572 5600 0000 7255 0000  inspacerV...rU..
+00001b00: 0072 2400 0000 da04 6576 616c 7225 0000  .r$.....evalr%..
+00001b10: 00da 0670 6172 616d 7329 0672 2800 0000  ...params).r(...
+00001b20: 7247 0000 0072 4600 0000 da09 6e75 6d70  rG...rF.....nump
+00001b30: 6f69 6e74 735a 0678 6375 7276 655a 0679  ointsZ.xcurveZ.y
+00001b40: 6375 7276 6572 1b00 0000 721b 0000 0072  curver....r....r
+00001b50: 1c00 0000 da09 6765 745f 6375 7276 65ec  ......get_curve.
+00001b60: 0000 0073 1600 0000 0003 0801 0c01 0801  ...s............
+00001b70: 0c01 0e03 0602 0801 08ff 0805 1401 7a10  ..............z.
+00001b80: 4669 7474 6572 2e67 6574 5f63 7572 7665  Fitter.get_curve
+00001b90: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001ba0: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00001bb0: 6a00 5300 722b 0000 0029 0172 5600 0000  j.S.r+...).rV...
+00001bc0: 7236 0000 0072 1b00 0000 721b 0000 0072  r6...r....r....r
+00001bd0: 1c00 0000 da10 6765 745f 6d6f 6465 6c5f  ......get_model_
+00001be0: 7265 7375 6c74 0001 0000 7302 0000 0000  result....s.....
+00001bf0: 017a 1746 6974 7465 722e 6765 745f 6d6f  .z.Fitter.get_mo
+00001c00: 6465 6c5f 7265 7375 6c74 6304 0000 0000  del_resultc.....
+00001c10: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+00001c20: 0000 0073 1800 0000 7c00 6a00 730a 6400  ...s....|.j.s.d.
+00001c30: 5300 7c00 a001 7c01 7c02 7c03 a103 5300  S.|...|.|.|...S.
+00001c40: 722b 0000 0029 0272 5700 0000 728a 0000  r+...).rW...r...
+00001c50: 0029 0472 2800 0000 7247 0000 0072 4600  .).r(...rG...rF.
+00001c60: 0000 7289 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00001c70: 0072 1c00 0000 da0c 6765 745f 6669 7463  .r......get_fitc
+00001c80: 7572 7665 0301 0000 7306 0000 0000 0306  urve....s.......
+00001c90: 0104 017a 1346 6974 7465 722e 6765 745f  ...z.Fitter.get_
+00001ca0: 6669 7463 7572 7665 5463 0200 0000 0000  fitcurveTc......
+00001cb0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
+00001cc0: 0000 7320 0000 007c 006a 0073 0e7c 0172  ..s ...|.j.s.|.r
+00001cd0: 0e64 0153 007c 006a 0173 1864 0153 007c  .d.S.|.j.s.d.S.|
+00001ce0: 006a 016a 0253 0029 027a 850a 2020 2020  .j.j.S.).z..    
+00001cf0: 2020 2020 7265 7475 726e 2074 6865 2072      return the r
+00001d00: 6573 6964 7561 6c73 2061 7320 7920 2d20  esiduals as y - 
+00001d10: 6628 7829 0a20 2020 2020 2020 2069 6620  f(x).        if 
+00001d20: 6368 6563 6b20 6973 2054 7275 6528 6465  check is True(de
+00001d30: 6661 756c 7429 206f 6e6c 7920 7265 7475  fault) only retu
+00001d40: 726e 7320 7661 6c75 6573 2069 6620 6120  rns values if a 
+00001d50: 7661 6c69 6420 6669 7420 6973 2070 6572  valid fit is per
+00001d60: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
+00001d70: 4e29 0372 5700 0000 7256 0000 00da 0872  N).rW...rV.....r
+00001d80: 6573 6964 7561 6c29 0272 2800 0000 da05  esidual).r(.....
+00001d90: 6368 6563 6b72 1b00 0000 721b 0000 0072  checkr....r....r
+00001da0: 1c00 0000 da0d 6765 745f 7265 7369 6475  ......get_residu
+00001db0: 616c 730a 0100 0073 0a00 0000 0006 0a01  als....s........
+00001dc0: 0401 0601 0403 7a14 4669 7474 6572 2e67  ......z.Fitter.g
+00001dd0: 6574 5f72 6573 6964 7561 6c73 6301 0000  et_residualsc...
+00001de0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00001df0: 0043 0000 0073 1800 0000 7400 7c00 6a01  .C...s....t.|.j.
+00001e00: a002 a100 7c00 6a03 a004 a100 1800 8301  ....|.j.........
+00001e10: 5300 722b 0000 0029 05da 0369 6e74 7253  S.r+...)...intrS
+00001e20: 0000 0072 4900 0000 7255 0000 0072 3700  ...rI...rU...r7.
+00001e30: 0000 7236 0000 0072 1b00 0000 721b 0000  ..r6...r....r...
+00001e40: 0072 1c00 0000 7278 0000 0018 0100 0073  .r....rx.......s
+00001e50: 0200 0000 0001 7a1a 4669 7474 6572 2e5f  ......z.Fitter._
+00001e60: 6465 6772 6565 735f 6f66 5f66 7265 6564  degrees_of_freed
+00001e70: 6f6d 6301 0000 0000 0000 0000 0000 0002  omc.............
+00001e80: 0000 0009 0000 0003 0000 0073 5e00 0000  ...........s^...
+00001e90: 8700 6601 6401 6402 8408 7d01 8800 6a00  ..f.d.d...}...j.
+00001ea0: 6a01 8800 6a00 6a02 8800 6a03 a004 a100  j...j.j...j.....
+00001eb0: 8800 a005 a100 7406 6a07 a008 6403 8800  ......t.j...d...
+00001ec0: a005 a100 a102 6404 9c05 7c01 8300 8800  ......d...|.....
+00001ed0: 6a09 8800 6a0a 6a0b 8800 6a0a 6a0c 6405  j...j.j...j.j.d.
+00001ee0: 9c03 6406 9c03 8800 5f0d 6400 5300 2907  ..d....._.d.S.).
+00001ef0: 4e63 0000 0000 0000 0000 0000 0000 0100  Nc..............
+00001f00: 0000 0200 0000 1300 0000 7316 0000 0064  ..........s....d
+00001f10: 0164 0284 0088 006a 006a 0144 0083 017d  .d.....j.j.D...}
+00001f20: 007c 0053 0029 034e 6301 0000 0000 0000  .|.S.).Nc.......
+00001f30: 0000 0000 0002 0000 0008 0000 0053 0000  .............S..
+00001f40: 0073 2400 0000 6900 7c00 5d1c 7d01 7c01  .s$...i.|.].}.|.
+00001f50: 6a00 7401 7c01 6a02 7c01 6a03 7c01 6a04  j.t.|.j.|.j.|.j.
+00001f60: 6400 8d03 9302 7104 5300 2901 2903 7210  d.....q.S.).).r.
+00001f70: 0000 0072 8100 0000 7212 0000 0029 0572  ...r....r....).r
+00001f80: 0e00 0000 da04 6469 6374 7210 0000 0072  ......dictr....r
+00001f90: 1100 0000 7212 0000 0072 2d00 0000 721b  ....r....r-...r.
+00001fa0: 0000 0072 1b00 0000 721c 0000 00da 0a3c  ...r....r......<
+00001fb0: 6469 6374 636f 6d70 3e1d 0100 0073 0800  dictcomp>....s..
+00001fc0: 0000 0604 02fd 0601 0cff 7a3f 4669 7474  ..........z?Fitt
+00001fd0: 6572 2e5f 6372 6561 7465 5f72 6570 6f72  er._create_repor
+00001fe0: 742e 3c6c 6f63 616c 733e 2e70 6172 735f  t.<locals>.pars_
+00001ff0: 746f 5f64 6963 742e 3c6c 6f63 616c 733e  to_dict.<locals>
+00002000: 2e3c 6469 6374 636f 6d70 3e29 0272 5500  .<dictcomp>).rU.
+00002010: 0000 7220 0000 0029 015a 0870 6172 7364  ..r ...).Z.parsd
+00002020: 6963 7472 3600 0000 721b 0000 0072 1c00  ictr6...r....r..
+00002030: 0000 da0c 7061 7273 5f74 6f5f 6469 6374  ....pars_to_dict
+00002040: 1c01 0000 7308 0000 0000 0106 0406 fc06  ....s...........
+00002050: 067a 2b46 6974 7465 722e 5f63 7265 6174  .z+Fitter._creat
+00002060: 655f 7265 706f 7274 2e3c 6c6f 6361 6c73  e_report.<locals
+00002070: 3e2e 7061 7273 5f74 6f5f 6469 6374 6733  >.pars_to_dictg3
+00002080: 3333 3333 33ef 3f29 0572 5500 0000 721f  33333.?).rU...r.
+00002090: 0000 00da 014e da03 646f 667a 0774 3935  .....N..dofz.t95
+000020a0: 2d76 616c 2903 7a18 536d 696e 2c20 6d65  -val).z.Smin, me
+000020b0: 616e 2073 7175 6172 6564 2065 7272 6f72  an squared error
+000020c0: 7a0b 4368 6920 5371 7561 7265 647a 0352  z.Chi Squaredz.R
+000020d0: 5e32 2903 5a0d 4649 5450 4152 414d 4554  ^2).Z.FITPARAMET
+000020e0: 4552 535a 0a46 4954 5245 5355 4c54 535a  ERSZ.FITRESULTSZ
+000020f0: 0a53 5441 5449 5354 4943 5329 0e72 5500  .STATISTICS).rU.
+00002100: 0000 7222 0000 0072 1f00 0000 7253 0000  ..r"...r....rS..
+00002110: 0072 4900 0000 7278 0000 0072 0700 0000  .rI...rx...r....
+00002120: da01 745a 0370 7066 7258 0000 0072 5600  ..tZ.ppfrX...rV.
+00002130: 0000 5a06 6368 6973 7172 5a08 7273 7175  ..Z.chisqrZ.rsqu
+00002140: 6172 6564 7259 0000 0029 0272 2800 0000  aredrY...).r(...
+00002150: 7293 0000 0072 1b00 0000 7236 0000 0072  r....r....r6...r
+00002160: 1c00 0000 727e 0000 001b 0100 0073 1a00  ....r~.......s..
+00002170: 0000 0001 0c0b 0601 0601 0801 0601 10fb  ................
+00002180: 0407 0402 0401 0601 06fd 04f7 7a15 4669  ............z.Fi
+00002190: 7474 6572 2e5f 6372 6561 7465 5f72 6570  tter._create_rep
+000021a0: 6f72 7463 0100 0000 0000 0000 0000 0000  ortc............
+000021b0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+000021c0: 007c 006a 0053 0072 2b00 0000 2901 7259  .|.j.S.r+...).rY
+000021d0: 0000 0072 3600 0000 721b 0000 0072 1b00  ...r6...r....r..
+000021e0: 0000 721c 0000 00da 0a67 6574 5f72 6570  ..r......get_rep
+000021f0: 6f72 7435 0100 0073 0200 0000 0001 7a11  ort5...s......z.
+00002200: 4669 7474 6572 2e67 6574 5f72 6570 6f72  Fitter.get_repor
+00002210: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00002220: 0000 0300 0000 4300 0000 7324 0000 007c  ......C...s$...|
+00002230: 006a 006a 0164 0075 0172 127c 006a 0253  .j.j.d.u.r.|.j.S
+00002240: 007c 006a 0264 0164 0285 0219 0053 0064  .|.j.d.d.....S.d
+00002250: 0053 0029 034e 7201 0000 0072 0a00 0000  .S.).Nr....r....
+00002260: 2903 7253 0000 0072 3c00 0000 7271 0000  ).rS...r<...rq..
+00002270: 0072 3600 0000 721b 0000 0072 1b00 0000  .r6...r....r....
+00002280: 721c 0000 00da 1167 6574 5f77 6569 6768  r......get_weigh
+00002290: 746f 7074 696f 6e73 3801 0000 7306 0000  toptions8...s...
+000022a0: 0000 010c 0106 037a 1846 6974 7465 722e  .......z.Fitter.
+000022b0: 6765 745f 7765 6967 6874 6f70 7469 6f6e  get_weightoption
+000022c0: 7363 0500 0000 0000 0000 0000 0000 0500  sc..............
+000022d0: 0000 0600 0000 4300 0000 7316 0000 007c  ......C...s....|
+000022e0: 00a0 007c 017c 027c 037c 04a1 047c 005f  ...|.|.|.|...|._
+000022f0: 0164 0053 0072 2b00 0000 2902 7252 0000  .d.S.r+...).rR..
+00002300: 0072 5300 0000 2905 7228 0000 0072 3100  .rS...).r(...r1.
+00002310: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
+00002320: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00002330: da0b 6368 616e 6765 5f64 6174 613f 0100  ..change_data?..
+00002340: 0073 0200 0000 0001 7a12 4669 7474 6572  .s......z.Fitter
+00002350: 2e63 6861 6e67 655f 6461 7461 6304 0000  .change_datac...
+00002360: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00002370: 0043 0000 0073 1400 0000 7c00 a000 7c01  .C...s....|...|.
+00002380: 7c02 7c03 a103 7c00 5f01 6400 5300 722b  |.|...|._.d.S.r+
+00002390: 0000 0029 0272 5400 0000 7255 0000 0029  ...).rT...rU...)
+000023a0: 0472 2800 0000 721e 0000 0072 6100 0000  .r(...r....ra...
+000023b0: 7262 0000 0072 1b00 0000 721b 0000 0072  rb...r....r....r
+000023c0: 1c00 0000 da0c 6368 616e 6765 5f6d 6f64  ......change_mod
+000023d0: 656c 4301 0000 7302 0000 0000 017a 1346  elC...s......z.F
+000023e0: 6974 7465 722e 6368 616e 6765 5f6d 6f64  itter.change_mod
+000023f0: 656c 2901 5429 1472 1300 0000 7214 0000  el).T).r....r...
+00002400: 0072 1500 0000 7216 0000 0072 7100 0000  .r....r....rq...
+00002410: 7264 0000 0072 5200 0000 7254 0000 0072  rd...rR...rT...r
+00002420: 8200 0000 720c 0000 0072 8a00 0000 728b  ....r....r....r.
+00002430: 0000 0072 8c00 0000 728f 0000 0072 7800  ...r....r....rx.
+00002440: 0000 727e 0000 0072 9700 0000 7298 0000  ..r~...r....r...
+00002450: 0072 9900 0000 729a 0000 0072 1b00 0000  .r....r....r....
+00002460: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00002470: 4b00 0000 5b00 0000 7324 0000 0008 0104  K...[...s$......
+00002480: 0204 0208 1c08 1808 2408 350a ff0a 1408  ........$.5.....
+00002490: 040a ff0a 070a 0e08 0308 1a08 0308 0708  ................
+000024a0: 0472 4b00 0000 da05 736c 7371 7029 0372  .rK.....slsqp).r
+000024b0: 6100 0000 7276 0000 0072 5000 0000 6301  a...rv...rP...c.
+000024c0: 0000 0000 0000 0003 0000 0016 0000 0009  ................
+000024d0: 0000 004f 0000 0073 e801 0000 7400 a001  ...O...s....t...
+000024e0: 7c00 6a02 a101 6a03 7d06 6401 6402 8400  |.j...j.}.d.d...
+000024f0: 7c06 a004 a100 4400 8301 7d07 7c02 6403  |.....D...}.|.d.
+00002500: 7500 7244 7405 a006 6404 6402 8400 7c07  u.rDt...d.d...|.
+00002510: 6405 6403 8502 1900 4400 8301 a101 7d02  d.d.....D.....}.
+00002520: 7c01 6403 7500 7268 7405 a006 6406 6402  |.d.u.rht...d.d.
+00002530: 8400 7c07 6405 6403 8502 1900 4400 8301  ..|.d.d.....D...
+00002540: a101 7d01 7c07 6407 1900 6701 6408 6402  ..}.|.d...g.d.d.
+00002550: 8400 7407 7c07 6405 6403 8502 1900 7c02  ..t.|.d.d.....|.
+00002560: 8302 4400 8301 1700 7d08 7c07 6407 1900  ..D.....}.|.d...
+00002570: 6701 6409 6402 8400 7407 7c07 6405 6403  g.d.d...t.|.d.d.
+00002580: 8502 1900 7c02 7c01 8303 4400 8301 1700  ....|.|...D.....
+00002590: 7d09 7408 640a 640b a009 7c08 a101 9b00  }.t.d.d...|.....
+000025a0: 640c 640b a009 7c09 a101 9b00 640d 9d05  d.d...|.....d...
+000025b0: 740a 8300 8302 7d0a 7405 a006 640e 6402  t.....}.t...d.d.
+000025c0: 8400 7407 7c01 7c02 8302 4400 8301 a101  ..t.|.|...D.....
+000025d0: 7d0b 7c00 6a03 7d0c 7407 7c07 6405 6403  }.|.j.}.t.|.d.d.
+000025e0: 8502 1900 7c02 7c01 8303 4400 5d22 5c03  ....|.|...D.]"\.
+000025f0: 7d0d 7d0e 7d0f 7c0e 0c00 7c0c 7c0d 1900  }.}.}.|...|.|...
+00002600: 5f0b 7c0f 7c0c 7c0d 1900 5f0c 9001 7110  _.|.|.|..._...q.
+00002610: 7c00 6a0d 6a0e 7c04 6405 1900 7c0c 7c04  |.j.j.|.d...|.|.
+00002620: 6407 1900 640f 6410 7c03 6411 6412 8d07  d...d.d.|.d.d...
+00002630: 7d10 7405 a006 740f 7c10 6a10 a004 a100  }.t...t.|.j.....
+00002640: 8301 a101 7d11 7411 6413 7c10 6a12 8302  ....}.t.d.|.j...
+00002650: 0100 7405 a006 7c10 6a12 a101 7d12 7411  ..t...|.j...}.t.
+00002660: 6414 7c12 8302 0100 6415 6402 8400 7407  d.|.....d.d...t.
+00002670: 7c01 7c02 8302 4400 8301 7d13 7405 a013  |.|...D...}.t...
+00002680: 7c02 a101 6407 1900 7d14 7c14 4400 5d2a  |...d...}.|.D.]*
+00002690: 7d15 7405 6a14 7c12 7c15 6407 6405 6416  }.t.j.|.|.d.d.d.
+000026a0: 8d04 7d12 7405 6a14 7c12 7c15 6407 6407  ..}.t.j.|.|.d.d.
+000026b0: 6416 8d04 7d12 9001 71b2 7c11 7c12 7c10  d...}...q.|.|.|.
+000026c0: 6603 5300 2917 613f 0100 000a 2020 2020  f.S.).a?....    
+000026d0: 7772 6170 7065 7220 6172 6f75 6e64 2074  wrapper around t
+000026e0: 6865 2073 6369 7079 2063 7572 7665 5f66  he scipy curve_f
+000026f0: 6974 2829 2066 756e 6374 696f 6e20 746f  it() function to
+00002700: 2061 6c6c 6f77 2070 6172 616d 6574 6572   allow parameter
+00002710: 7320 746f 2062 6520 6669 7865 640a 2020  s to be fixed.  
+00002720: 2020 7361 6d65 2063 616c 6c20 7369 676e    same call sign
+00002730: 6174 7572 6520 6173 2074 6865 2063 7572  ature as the cur
+00002740: 7665 5f66 6974 2829 2066 756e 6374 696f  ve_fit() functio
+00002750: 6e20 6578 6365 7074 2066 6f72 3a0a 2020  n except for:.  
+00002760: 2020 7046 203a 2031 4420 6e75 6d70 7920    pF : 1D numpy 
+00002770: 6172 7261 7920 6f66 2073 697a 6520 6e2c  array of size n,
+00002780: 2077 6974 6820 6e20 7468 6520 6e75 6d62   with n the numb
+00002790: 6572 206f 6620 6669 7470 6172 616d 6574  er of fitparamet
+000027a0: 6572 7320 6f66 2074 6865 2066 756e 6374  ers of the funct
+000027b0: 696f 6e0a 2020 2020 7265 7475 726e 7320  ion.    returns 
+000027c0: 7468 6520 706f 7074 2061 6e64 2063 6f76  the popt and cov
+000027d0: 206d 6174 7269 6365 7320 6a75 7374 206c   matrices just l
+000027e0: 696b 6520 7468 6520 6f72 6967 696e 616c  ike the original
+000027f0: 2063 7572 7665 5f66 6974 2829 2066 756e   curve_fit() fun
+00002800: 6374 696f 6e0a 2020 2020 6301 0000 0000  ction.    c.....
+00002810: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
+00002820: 0000 0073 1200 0000 6700 7c00 5d0a 7d01  ...s....g.|.].}.
+00002830: 7c01 6a00 9102 7104 5300 721b 0000 0072  |.j...q.S.r....r
+00002840: 6800 0000 7269 0000 0072 1b00 0000 721b  h...ri...r....r.
+00002850: 0000 0072 1c00 0000 7234 0000 0054 0100  ...r....r4...T..
+00002860: 0072 3000 0000 7a25 6375 7276 655f 6669  .r0...z%curve_fi
+00002870: 745f 7772 6170 7065 722e 3c6c 6f63 616c  t_wrapper.<local
+00002880: 733e 2e3c 6c69 7374 636f 6d70 3e4e 6301  s>.<listcomp>Nc.
+00002890: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000028a0: 0000 0053 0000 0073 1000 0000 6700 7c00  ...S...s....g.|.
+000028b0: 5d08 7d01 6400 9102 7104 5300 2901 4672  ].}.d...q.S.).Fr
+000028c0: 1b00 0000 a902 722e 0000 00da 015f 721b  ......r......_r.
+000028d0: 0000 0072 1b00 0000 721c 0000 0072 3400  ...r....r....r4.
+000028e0: 0000 5801 0000 7230 0000 0072 0a00 0000  ..X...r0...r....
+000028f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00002900: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
+00002910: 7c00 5d08 7d01 6400 9102 7104 5300 2901  |.].}.d...q.S.).
+00002920: 720a 0000 0072 1b00 0000 729c 0000 0072  r....r....r....r
+00002930: 1b00 0000 721b 0000 0072 1c00 0000 7234  ....r....r....r4
+00002940: 0000 005a 0100 0072 3000 0000 7201 0000  ...Z...r0...r...
+00002950: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+00002960: 0000 0400 0000 5300 0000 7318 0000 0067  ......S...s....g
+00002970: 007c 005d 105c 027d 017d 027c 0273 047c  .|.].\.}.}.|.s.|
+00002980: 0191 0271 0453 0072 1b00 0000 721b 0000  ...q.S.r....r...
+00002990: 0029 0372 2e00 0000 726a 0000 00da 0366  .).r....rj.....f
+000029a0: 6978 721b 0000 0072 1b00 0000 721c 0000  ixr....r....r...
+000029b0: 0072 3400 0000 5d01 0000 7302 0000 0006  .r4...]...s.....
+000029c0: 0163 0100 0000 0000 0000 0000 0000 0400  .c..............
+000029d0: 0000 0500 0000 5300 0000 7322 0000 0067  ......S...s"...g
+000029e0: 007c 005d 1a5c 037d 017d 027d 037c 0273  .|.].\.}.}.}.|.s
+000029f0: 167c 016e 0674 007c 0383 0191 0271 0453  .|.n.t.|.....q.S
+00002a00: 0072 1b00 0000 2901 7217 0000 0029 0472  .r....).r....).r
+00002a10: 2e00 0000 726a 0000 0072 9e00 0000 da01  ....rj...r......
+00002a20: 7072 1b00 0000 721b 0000 0072 1c00 0000  pr....r....r....
+00002a30: 7234 0000 0060 0100 0073 0200 0000 0601  r4...`...s......
+00002a40: 7a07 6c61 6d62 6461 207a 022c 207a 0820  z.lambda z., z. 
+00002a50: 3a20 6675 6e63 28fa 0129 6301 0000 0000  : func(..)c.....
+00002a60: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
+00002a70: 0000 0073 1800 0000 6700 7c00 5d10 5c02  ...s....g.|.].\.
+00002a80: 7d01 7d02 7c02 7304 7c01 9102 7104 5300  }.}.|.s.|...q.S.
+00002a90: 721b 0000 0072 1b00 0000 a903 722e 0000  r....r......r...
+00002aa0: 0072 9f00 0000 729e 0000 0072 1b00 0000  .r....r....r....
+00002ab0: 721b 0000 0072 1c00 0000 7234 0000 006b  r....r....r4...k
+00002ac0: 0100 0072 3000 0000 545a 046f 6d69 7469  ...r0...TZ.omiti
+00002ad0: f401 0000 2905 7231 0000 005a 0a63 616c  ....).r1...Z.cal
+00002ae0: 635f 636f 7661 725a 0a6e 616e 5f70 6f6c  c_covarZ.nan_pol
+00002af0: 6963 7972 5000 0000 da08 6d61 785f 6e66  icyrP.....max_nf
+00002b00: 6576 7a0a 636f 7620 7661 6c75 6573 7a18  evz.cov valuesz.
+00002b10: 636f 7620 7661 6c75 6573 2061 6674 6572  cov values after
+00002b20: 2061 7272 6179 6564 6301 0000 0000 0000   arrayedc.......
+00002b30: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
+00002b40: 0073 1800 0000 6700 7c00 5d10 5c02 7d01  .s....g.|.].\.}.
+00002b50: 7d02 7c02 7204 7c01 9102 7104 5300 721b  }.|.r.|...q.S.r.
+00002b60: 0000 0072 1b00 0000 72a1 0000 0072 1b00  ...r....r....r..
+00002b70: 0000 721b 0000 0072 1c00 0000 7234 0000  ..r....r....r4..
+00002b80: 008b 0100 0072 3000 0000 2901 da04 6178  .....r0...)...ax
+00002b90: 6973 2915 726d 0000 0072 6e00 0000 721e  is).rm...rn...r.
+00002ba0: 0000 0072 2500 0000 726f 0000 0072 4000  ...r%...ro...r@.
+00002bb0: 0000 724a 0000 0072 7000 0000 7287 0000  ..rJ...rp...r...
+00002bc0: 00da 046a 6f69 6eda 066c 6f63 616c 7372  ...join..localsr
+00002bd0: 2600 0000 7210 0000 0072 2400 0000 7282  &...r....r$...r.
+00002be0: 0000 00da 046c 6973 745a 0b62 6573 745f  .....listZ.best_
+00002bf0: 7661 6c75 6573 727b 0000 005a 0563 6f76  valuesr{...Z.cov
+00002c00: 6172 da05 7768 6572 65da 0669 6e73 6572  ar..where..inser
+00002c10: 7429 1672 5500 0000 7261 0000 0072 7600  t).rU...ra...rv.
+00002c20: 0000 7250 0000 005a 0570 6172 6773 7251  ..rP...Z.pargsrQ
+00002c30: 0000 005a 065f 5f61 7267 7372 7300 0000  ...Z.__argsrs...
+00002c40: 5a0c 6e65 7766 756e 635f 6172 6773 5a0c  Z.newfunc_argsZ.
+00002c50: 6f72 6966 756e 635f 6172 6773 5a08 6669  orifunc_argsZ.fi
+00002c60: 745f 6675 6e63 5a06 7030 5f66 6974 7288  t_funcZ.p0_fitr.
+00002c70: 0000 0072 6a00 0000 729e 0000 0072 9f00  ...rj...r....r..
+00002c80: 0000 7243 0000 0072 7f00 0000 7277 0000  ..rC...r....rw..
+00002c90: 005a 0670 305f 6669 785a 0669 645f 6669  .Z.p0_fixZ.id_fi
+00002ca0: 78da 0269 6472 1b00 0000 721b 0000 0072  x..idr....r....r
+00002cb0: 1c00 0000 727a 0000 0048 0100 0073 5400  ....rz...H...sT.
+00002cc0: 0000 000b 0e01 1203 0801 1c01 0801 1c03  ................
+00002cd0: 0e01 10ff 0803 0e01 12ff 0805 0201 1c01  ................
+00002ce0: 04fe 0406 1a0b 0601 1e01 0c01 0e02 0601  ................
+00002cf0: 0601 0201 0601 0201 0201 0201 02f9 060a  ................
+00002d00: 1401 0c01 0c01 0a03 1401 0e0a 0801 0401  ................
+00002d10: 08ff 0603 1603 727a 0000 0063 0400 0000  ......rz...c....
+00002d20: 0000 0000 0000 0000 0d00 0000 0500 0000  ................
+00002d30: 0300 0000 73d8 0000 0064 0164 0284 0089  ....s....d.d....
+00002d40: 0064 0a87 0066 0164 0464 0584 097d 0464  .d...f.d.d...}.d
+00002d50: 0b64 0664 0784 017d 0588 007c 0183 017d  .d.d...}...|...}
+00002d60: 067c 0372 4a7c 047c 017c 0674 0064 0819  .|.rJ|.|.|.t.d..
+00002d70: 0083 035c 027d 077d 0864 007d 097c 067d  ...\.}.}.d.}.|.}
+00002d80: 0a6e 7a88 007c 0283 017d 0b7c 067c 0b6b  .nz..|...}.|.|.k
+00002d90: 0572 907c 047c 017c 0674 0064 0919 007c  .r.|.|.|.t.d...|
+00002da0: 0617 007c 0b18 0083 035c 027d 077d 087c  ...|.....\.}.}.|
+00002db0: 047c 027c 0674 0064 0919 0083 035c 027d  .|.|.t.d.....\.}
+00002dc0: 097d 087c 067d 0a6e 347c 047c 017c 0b74  .}.|.}.n4|.|.|.t
+00002dd0: 0064 0919 007c 0617 007c 0b18 0083 035c  .d...|...|.....\
+00002de0: 027d 077d 087c 047c 027c 0b74 0064 0919  .}.}.|.|.|.t.d..
+00002df0: 0083 035c 027d 097d 087c 0b7d 0a7c 007c  ...\.}.}.|.}.|.|
+00002e00: 057c 077c 0a7c 0983 0317 007d 0c7c 0c53  .|.|.|.....}.|.S
+00002e10: 0029 0c4e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00002e20: 0004 0000 0005 0000 0053 0000 0073 4e00  .........S...sN.
+00002e30: 0000 6401 7d01 7c00 6402 7c01 9b00 6403  ..d.}.|.d.|...d.
+00002e40: 9d03 9b04 7d02 7c02 a000 6403 a101 6404  ....}.|...d...d.
+00002e50: 1700 7d03 7c02 7c03 6405 8502 1900 6406  ..}.|.|.d.....d.
+00002e60: 6b02 723a 7401 6407 8301 5300 7401 7402  k.r:t.d...S.t.t.
+00002e70: 7c02 7c03 6405 8502 1900 8301 8301 5300  |.|.d.........S.
+00002e80: 2908 7a44 7265 7475 726e 7320 7468 6520  ).zDreturns the 
+00002e90: 6578 706f 6e65 6e74 2061 7320 616e 2069  exponent as an i
+00002ea0: 6e74 2067 656e 6572 6174 6564 2062 7920  nt generated by 
+00002eb0: 7468 6520 3a2e 6520 666f 726d 6174 2073  the :.e format s
+00002ec0: 7065 6369 6669 6572 e905 0000 00da 012e  pecifier........
+00002ed0: da01 6572 0a00 0000 4eda 036e 616e 7a03  ..er....N..nanz.
+00002ee0: 2b30 3029 03da 0466 696e 6472 9000 0000  +00)...findr....
+00002ef0: 7219 0000 0029 0472 1000 0000 da04 6465  r....).r......de
+00002f00: 6369 da01 735a 0a69 6e64 6578 5f73 6967  ci..sZ.index_sig
+00002f10: 6e72 1b00 0000 721b 0000 0072 1c00 0000  nr....r....r....
+00002f20: da0c 6765 745f 6578 706f 6e65 6e74 a101  ..get_exponent..
+00002f30: 0000 730c 0000 0000 0204 0110 010e 0310  ..s.............
+00002f40: 0108 017a 2576 616c 7565 5f74 6f5f 7374  ...z%value_to_st
+00002f50: 7269 6e67 2e3c 6c6f 6361 6c73 3e2e 6765  ring.<locals>.ge
+00002f60: 745f 6578 706f 6e65 6e74 726b 0000 0063  t_exponentrk...c
+00002f70: 0300 0000 0000 0000 0000 0000 0600 0000  ................
+00002f80: 0400 0000 1300 0000 7354 0000 007c 027c  ........sT...|.|
+00002f90: 0117 0088 007c 0083 0118 0064 0118 007d  .....|.....d...}
+00002fa0: 037c 0364 026b 0072 2064 027d 037c 0064  .|.d.k.r d.}.|.d
+00002fb0: 037c 0113 001b 0064 047c 039b 0064 059d  .|.....d.|...d..
+00002fc0: 039b 047d 0464 037c 0113 0064 069b 0464  ...}.d.|...d...d
+00002fd0: 0164 0785 0219 007d 057c 047c 0566 0253  .d.....}.|.|.f.S
+00002fe0: 0029 0861 1901 0000 0a20 2020 2020 2020  .).a.....       
+00002ff0: 2072 6574 7572 6e73 2061 2073 7472 696e   returns a strin
+00003000: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
+00003010: 2069 6e20 7363 6965 6e74 6966 6963 206e   in scientific n
+00003020: 6f74 6174 696f 6e20 6f66 2061 206e 756d  otation of a num
+00003030: 6265 720a 2020 2020 2020 2020 7370 6563  ber.        spec
+00003040: 6966 6965 6420 6279 2076 616c 7565 2e0a  ified by value..
+00003050: 2020 2020 2020 2020 7661 6c75 653a 2074          value: t
+00003060: 6865 206e 756d 6265 7220 7468 6174 2069  he number that i
+00003070: 7320 636f 6e76 6572 7465 640a 2020 2020  s converted.    
+00003080: 2020 2020 6578 706f 6e65 6e74 3a20 7468      exponent: th
+00003090: 6520 6578 706f 6e65 6e74 2075 7365 6420  e exponent used 
+000030a0: 666f 7220 7468 6520 7265 7072 6573 656e  for the represen
+000030b0: 7461 7469 6f6e 0a20 2020 2020 2020 2073  tation.        s
+000030c0: 6967 5f64 6967 6974 733a 2074 6865 206e  ig_digits: the n
+000030d0: 756d 6265 7220 6f66 2073 6967 6e69 6669  umber of signifi
+000030e0: 6361 6e74 2064 6967 6974 7320 7468 6174  cant digits that
+000030f0: 2069 7320 7573 6564 0a20 2020 2020 2020   is used.       
+00003100: 2072 0a00 0000 7201 0000 00e9 0a00 0000   r....r.........
+00003110: 72ab 0000 00da 0166 7a03 2e30 654e 721b  r......fz..0eNr.
+00003120: 0000 0029 0672 1000 0000 da08 6578 706f  ...).r......expo
+00003130: 6e65 6e74 5a0a 7369 675f 6469 6769 7473  nentZ.sig_digits
+00003140: 72af 0000 005a 0772 6573 756c 7431 5a07  r....Z.result1Z.
+00003150: 7265 7375 6c74 32a9 0172 b100 0000 721b  result2..r....r.
+00003160: 0000 0072 1c00 0000 da0f 666c 6f61 745f  ...r......float_
+00003170: 746f 5f73 7472 696e 67ac 0100 0073 0c00  to_string....s..
+00003180: 0000 0008 1401 0801 0401 1801 1401 7a28  ..............z(
+00003190: 7661 6c75 655f 746f 5f73 7472 696e 672e  value_to_string.
+000031a0: 3c6c 6f63 616c 733e 2e66 6c6f 6174 5f74  <locals>.float_t
+000031b0: 6f5f 7374 7269 6e67 6303 0000 0000 0000  o_stringc.......
+000031c0: 0000 0000 0004 0000 0004 0000 0053 0000  .............S..
+000031d0: 0073 5a00 0000 7c02 6401 7500 720c 6402  .sZ...|.d.u.r.d.
+000031e0: 6e02 7c02 7d02 7c02 723e 7c02 6403 6b03  n.|.}.|.r>|.d.k.
+000031f0: 723e 6404 7c00 1700 6405 1700 7c02 1700  r>d.|...d...|...
+00003200: 6406 1700 6407 7c01 9b00 6408 9d03 1700  d...d.|...d.....
+00003210: 7d03 6e18 6409 7c00 1700 640a 1700 6407  }.n.d.|...d...d.
+00003220: 7c01 9b00 6408 9d03 1700 7d03 7c03 5300  |...d.....}.|.S.
+00003230: 290b 7a91 7265 7475 726e 2061 206c 6174  ).z.return a lat
+00003240: 6578 2073 7472 696e 670a 2020 2020 2020  ex string.      
+00003250: 2020 2876 616c 7565 5f73 7472 202b 2f2d    (value_str +/-
+00003260: 2065 7272 6f72 5f73 7472 2920 7820 3130   error_str) x 10
+00003270: 5e28 6578 706f 6e65 6e74 290a 2020 2020  ^(exponent).    
+00003280: 2020 2020 6368 6563 6b73 2066 6f72 206e      checks for n
+00003290: 616e 206f 7220 4e6f 6e65 2074 6f20 7072  an or None to pr
+000032a0: 6576 656e 7420 7072 6f67 7261 6d20 6372  event program cr
+000032b0: 6173 6820 706f 7373 6962 6c79 0a20 2020  ash possibly.   
+000032c0: 2020 2020 204e da01 3072 ad00 0000 7a04       N..0r....z.
+000032d0: 243d 2028 7a03 5c70 6d7a 0829 5c74 696d  $= (z.\pmz.)\tim
+000032e0: 6573 247a 0524 3130 5e7b 7a02 7d24 7a02  es$z.$10^{z.}$z.
+000032f0: 243d 7a07 5c74 696d 6573 2472 1b00 0000  $=z.\times$r....
+00003300: 2904 da09 7661 6c75 655f 7374 7272 b400  )...value_strr..
+00003310: 0000 da09 6572 726f 725f 7374 725a 0c6c  ....error_strZ.l
+00003320: 6174 6578 5f73 7472 696e 6772 1b00 0000  atex_stringr....
+00003330: 721b 0000 0072 1c00 0000 da08 746f 5f6c  r....r......to_l
+00003340: 6174 6578 bb01 0000 7322 0000 0000 0510  atex....s"......
+00003350: 020c 0302 0102 ff02 0202 fe02 0302 fd02  ................
+00003360: 0402 fc02 050a fb02 ff04 0a16 ff02 037a  ...............z
+00003370: 2176 616c 7565 5f74 6f5f 7374 7269 6e67  !value_to_string
+00003380: 2e3c 6c6f 6361 6c73 3e2e 746f 5f6c 6174  .<locals>.to_lat
+00003390: 6578 da16 434d 5f53 4947 5f44 4947 4954  ex..CM_SIG_DIGIT
+000033a0: 535f 4e4f 5f45 5252 4f52 da0d 434d 5f53  S_NO_ERROR..CM_S
+000033b0: 4947 5f44 4947 4954 5329 0172 6b00 0000  IG_DIGITS).rk...
+000033c0: 2901 4e72 0b00 0000 290d 720e 0000 0072  ).Nr....).r....r
+000033d0: 1000 0000 da05 6572 726f 7272 1200 0000  ......errorr....
+000033e0: 72b6 0000 0072 ba00 0000 5a03 785f 6572  r....r....Z.x_er
+000033f0: b800 0000 729d 0000 0072 b900 0000 72b4  ....r....r....r.
+00003400: 0000 005a 0464 785f 65da 0863 6f6d 6269  ...Z.dx_e..combi
+00003410: 6e65 6472 1b00 0000 72b5 0000 0072 1c00  nedr....r....r..
+00003420: 0000 da0f 7661 6c75 655f 746f 5f73 7472  ....value_to_str
+00003430: 696e 67a0 0100 0073 3800 0000 0001 080b  ing....s8.......
+00003440: 0e0f 0a17 0801 0401 0201 0aff 0803 0401  ................
+00003450: 0602 0801 0801 0201 12ff 0803 0201 0aff  ................
+00003460: 0803 0602 0201 12ff 0803 0201 0aff 0803  ................
+00003470: 0401 1002 72bf 0000 0063 0200 0000 0000  ....r....c......
+00003480: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00003490: 0000 7310 0000 007c 0064 017c 019b 0064  ..s....|.d.|...d
+000034a0: 029d 039b 0453 0029 037a 7e0a 2020 2020  .....S.).z~.    
+000034b0: 7265 7475 726e 2061 2073 7472 696e 6720  return a string 
+000034c0: 7265 7073 206f 6620 6120 7661 6c75 6520  reps of a value 
+000034d0: 696e 2073 6369 656e 7469 6669 6320 6e6f  in scientific no
+000034e0: 7461 7469 6f6e 2077 6974 6820 7468 6520  tation with the 
+000034f0: 6e75 6d62 6572 0a20 2020 206f 6620 7369  number.    of si
+00003500: 676e 6966 6963 616e 7420 6469 6769 7473  gnificant digits
+00003510: 2073 7065 6369 6669 6564 2062 7920 6469   specified by di
+00003520: 6769 7473 0a20 2020 207a 0231 2e72 ac00  gits.    z.1.r..
+00003530: 0000 721b 0000 0029 0272 1000 0000 da06  ..r....).r......
+00003540: 6469 6769 7473 721b 0000 0072 1b00 0000  digitsr....r....
+00003550: 721c 0000 00da 0c66 6c6f 6174 5f74 6f5f  r......float_to_
+00003560: 7374 72f0 0100 0073 0200 0000 0005 72c1  str....s......r.
+00003570: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00003580: 0100 0000 0400 0000 4300 0000 7320 0000  ........C...s ..
+00003590: 007c 00a0 0064 01a1 0164 026b 0472 1c7c  .|...d...d.k.r.|
+000035a0: 00a0 0164 0164 03a1 027d 0071 007c 0053  ...d.d...}.q.|.S
+000035b0: 0029 047a 2072 656d 6f76 6573 206c 6561  .).z removes lea
+000035c0: 6469 6e67 2073 7061 6365 7320 6672 6f6d  ding spaces from
+000035d0: 2074 6578 747a 050a 2020 2020 7201 0000   textz..    r...
+000035e0: 00da 010a 2902 da05 636f 756e 74da 0772  ....)...count..r
+000035f0: 6570 6c61 6365 2901 da04 7465 7874 721b  eplace)...textr.
+00003600: 0000 0072 1b00 0000 721c 0000 0072 7200  ...r....r....rr.
+00003610: 0000 f801 0000 7306 0000 0000 020e 010e  ......s.........
+00003620: 0172 7200 0000 291b 726d 0000 00da 0b64  .rr...).rm.....d
+00003630: 6174 6163 6c61 7373 6573 7202 0000 0072  ataclassesr....r
+00003640: 0300 0000 da06 7479 7069 6e67 7204 0000  ......typingr...
+00003650: 0072 0500 0000 725b 0000 00da 056e 756d  .r....r[.....num
+00003660: 7079 7240 0000 005a 056c 6d66 6974 7206  pyr@...Z.lmfitr.
+00003670: 0000 00da 0573 6369 7079 7207 0000 00da  .....scipyr.....
+00003680: 0e73 6369 7079 2e6f 7074 696d 697a 6572  .scipy.optimizer
+00003690: 0800 0000 7209 0000 00da 095f 7365 7474  ....r......_sett
+000036a0: 696e 6773 720c 0000 0072 0d00 0000 721d  ingsr....r....r.
+000036b0: 0000 0072 3900 0000 724b 0000 0072 7a00  ...r9...rK...rz.
+000036c0: 0000 72bf 0000 0072 c100 0000 7272 0000  ..r....r....rr..
+000036d0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+000036e0: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000036f0: 0000 0073 2a00 0000 0801 1001 1001 0801  ...s*...........
+00003700: 0801 0c01 0c01 1003 0c03 0201 100b 0201  ................
+00003710: 1027 0201 1018 0e7f 006f 06ff 0c58 0850  .'.......o...X.P
+00003720: 0808                                     ..
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/__pycache__/_widgets.cpython-39.pyc` & `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_widgets.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Mar 31 04:03:40 2023 UTC, .py size: 23281 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,1099 +1,1445 @@
-00000000: 610d 0d0a 0000 0000 9c5b 2664 f15a 0000  a........[&d.Z..
+00000000: 610d 0d0a 0000 0000 b044 4364 0379 0000  a........DCd.y..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6401 6c03 5a03 6500 a004 6403  ..d.d.l.Z.e...d.
-00000050: a101 0100 6400 6401 6c05 6d06 5a06 0100  ....d.d.l.m.Z...
-00000060: 6400 6401 6c07 5a08 6400 6404 6c09 6d0a  d.d.l.Z.d.d.l.m.
-00000070: 5a0a 0100 6400 6405 6c0b 6d0c 5a0c 0100  Z...d.d.l.m.Z...
-00000080: 6400 6406 6c0d 6d0e 5a0f 0100 6400 6407  d.d.l.m.Z...d.d.
-00000090: 6c0d 6d10 5a11 0100 6400 6408 6c12 6d13  l.m.Z...d.d.l.m.
-000000a0: 5a13 0100 6400 6409 6c14 6d15 5a15 0100  Z...d.d.l.m.Z...
-000000b0: 6400 640a 6c16 6d17 5a17 6d18 5a18 6d19  d.d.l.m.Z.m.Z.m.
-000000c0: 5a19 0100 6400 640b 6c1a 6d1b 5a1b 0100  Z...d.d.l.m.Z...
-000000d0: 6400 640c 6c1c 6d1d 5a1d 0100 640d 640e  d.d.l.m.Z...d.d.
-000000e0: 6c1e 6d1f 5a1f 0100 640d 640f 6c20 6d21  l.m.Z...d.d.l m!
-000000f0: 5a21 0100 6410 650c 6411 3c00 4700 6412  Z!..d.e.d.<.G.d.
-00000100: 6413 8400 6413 8302 5a22 4700 6414 6415  d...d...Z"G.d.d.
-00000110: 8400 6415 8302 5a23 4700 6416 6417 8400  ..d...Z#G.d.d...
-00000120: 6417 6519 6a24 8303 5a25 4700 6418 6419  d.e.j$..Z%G.d.d.
-00000130: 8400 6419 650f 8303 5a26 4700 641a 641b  ..d.e...Z&G.d.d.
-00000140: 8400 641b 6519 6a24 8303 5a27 4700 641c  ..d.e.j$..Z'G.d.
-00000150: 641d 8400 641d 6519 6a28 8303 5a29 4700  d...d.e.j(..Z)G.
-00000160: 641e 641f 8400 641f 6519 6a2a 8303 5a2b  d.d...d.e.j*..Z+
-00000170: 6401 5300 2920 e900 0000 004e a901 da0b  d.S.) .....N....
-00000180: 6465 6661 756c 7464 6963 74da 0669 676e  defaultdict..ign
-00000190: 6f72 6529 01da 054d 6f64 656c 2901 da08  ore)...Model)...
-000001a0: 7263 5061 7261 6d73 2901 da11 4669 6775  rcParams)...Figu
-000001b0: 7265 4361 6e76 6173 5154 4167 6729 01da  reCanvasQTAgg)..
-000001c0: 144e 6176 6967 6174 696f 6e54 6f6f 6c62  .NavigationToolb
-000001d0: 6172 3251 5429 01da 0646 6967 7572 6529  ar2QT)...Figure)
-000001e0: 01da 0450 6174 6829 03da 0651 7443 6f72  ...Path)...QtCor
-000001f0: 65da 0551 7447 7569 da09 5174 5769 6467  e..QtGui..QtWidg
-00000200: 6574 7329 01da 0651 496d 6167 6529 01da  ets)...QImage)..
-00000210: 0c51 4170 706c 6963 6174 696f 6ee9 0100  .QApplication...
-00000220: 0000 2901 da08 7365 7474 696e 6773 2901  ..)...settings).
-00000230: da0c 666c 6f61 745f 746f 5f73 7472 da02  ..float_to_str..
-00000240: 636d 7a10 6d61 7468 7465 7874 2e66 6f6e  cmz.mathtext.fon
-00000250: 7473 6574 6300 0000 0000 0000 0000 0000  tsetc...........
-00000260: 0000 0000 0003 0000 0040 0000 0073 5600  .........@...sV.
-00000270: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000280: 5a04 6416 6406 6407 8401 5a05 6408 6409  Z.d.d.d...Z.d.d.
-00000290: 8400 5a06 640a 640b 8400 5a07 640c 640d  ..Z.d.d...Z.d.d.
-000002a0: 8400 5a08 640e 640f 8400 5a09 6410 6411  ..Z.d.d...Z.d.d.
-000002b0: 8400 5a0a 6412 6413 8400 5a0b 6414 6415  ..Z.d.d...Z.d.d.
-000002c0: 8400 5a0c 6402 5300 2917 da0e 4472 6167  ..Z.d.S.)...Drag
-000002d0: 6761 626c 6556 4c69 6e65 7a33 636c 6173  gableVLinez3clas
-000002e0: 7320 746f 2063 7265 6174 6520 6120 6472  s to create a dr
-000002f0: 6167 6761 626c 6520 7665 7274 6963 616c  aggable vertical
-00000300: 206c 696e 6520 696e 2061 2070 6c6f 744e   line in a plotN
-00000310: e904 0000 00fa 022d 2dda 0467 7261 7963  .......--..grayc
-00000320: 0600 0000 0000 0000 0000 0000 0600 0000  ................
-00000330: 0600 0000 4300 0000 7326 0000 007c 016a  ....C...s&...|.j
-00000340: 007c 027c 037c 047c 0564 018d 047c 005f  .|.|.|.|.d...|._
-00000350: 0164 007c 005f 027c 00a0 03a1 0001 0064  .d.|._.|.......d
-00000360: 0053 0029 024e 2904 da01 78da 096c 696e  .S.).N)...x..lin
-00000370: 6577 6964 7468 da09 6c69 6e65 7374 796c  ewidth..linestyl
-00000380: 65da 0563 6f6c 6f72 2904 5a07 6178 766c  e..color).Z.axvl
-00000390: 696e 65da 046c 696e 65da 0570 7265 7373  ine..line..press
-000003a0: da07 636f 6e6e 6563 7429 06da 0473 656c  ..connect)...sel
-000003b0: 66da 0261 7872 1800 0000 7219 0000 0072  f..axr....r....r
-000003c0: 1a00 0000 721b 0000 00a9 0072 2100 0000  ....r......r!...
-000003d0: fa3b 2f55 7365 7273 2f6b 6f6a 6f2f 6170  .;/Users/kojo/ap
-000003e0: 7073 2f73 656e 696f 725f 7072 6f6a 6563  ps/senior_projec
-000003f0: 745f 7573 632f 6375 7276 6566 6974 6775  t_usc/curvefitgu
-00000400: 692f 5f77 6964 6765 7473 2e70 79da 085f  i/_widgets.py.._
-00000410: 5f69 6e69 745f 5f27 0000 0073 0a00 0000  _init__'...s....
-00000420: 0001 0401 08ff 0803 0601 7a17 4472 6167  ..........z.Drag
-00000430: 6761 626c 6556 4c69 6e65 2e5f 5f69 6e69  gableVLine.__ini
-00000440: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-00000450: 0100 0000 0200 0000 4300 0000 730e 0000  ........C...s...
-00000460: 007c 006a 00a0 01a1 0064 0119 0053 00a9  .|.j.....d...S..
-00000470: 024e 7201 0000 0029 0272 1c00 0000 da09  .Nr....).r......
-00000480: 6765 745f 7864 6174 61a9 0172 1f00 0000  get_xdata..r....
-00000490: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-000004a0: 0767 6574 5f70 6f73 2e00 0000 7302 0000  .get_pos....s...
-000004b0: 0000 017a 1644 7261 6767 6162 6c65 564c  ...z.DraggableVL
-000004c0: 696e 652e 6765 745f 706f 7363 0100 0000  ine.get_posc....
-000004d0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000004e0: 4300 0000 730e 0000 007c 006a 00a0 01a1  C...s....|.j....
-000004f0: 0001 0064 0053 00a9 014e 2902 721c 0000  ...d.S...N).r...
-00000500: 00da 0672 656d 6f76 6572 2600 0000 7221  ...remover&...r!
-00000510: 0000 0072 2100 0000 7222 0000 0072 2900  ...r!...r"...r).
-00000520: 0000 3100 0000 7302 0000 0000 017a 1544  ..1...s......z.D
-00000530: 7261 6767 6162 6c65 564c 696e 652e 7265  raggableVLine.re
-00000540: 6d6f 7665 6301 0000 0000 0000 0000 0000  movec...........
-00000550: 0001 0000 0004 0000 0043 0000 0073 4600  .........C...sF.
-00000560: 0000 7c00 6a00 6a01 6a02 a003 6401 7c00  ..|.j.j.j...d.|.
-00000570: 6a04 a102 7c00 5f05 7c00 6a00 6a01 6a02  j...|._.|.j.j.j.
-00000580: a003 6402 7c00 6a06 a102 7c00 5f07 7c00  ..d.|.j...|._.|.
-00000590: 6a00 6a01 6a02 a003 6403 7c00 6a08 a102  j.j.j...d.|.j...
-000005a0: 7c00 5f09 6404 5300 2905 7a21 636f 6e6e  |._.d.S.).z!conn
-000005b0: 6563 7420 746f 2061 6c6c 2074 6865 2065  ect to all the e
-000005c0: 7665 6e74 7320 7765 206e 6565 645a 1262  vents we needZ.b
-000005d0: 7574 746f 6e5f 7072 6573 735f 6576 656e  utton_press_even
-000005e0: 745a 1462 7574 746f 6e5f 7265 6c65 6173  tZ.button_releas
-000005f0: 655f 6576 656e 745a 136d 6f74 696f 6e5f  e_eventZ.motion_
-00000600: 6e6f 7469 6679 5f65 7665 6e74 4e29 0a72  notify_eventN).r
-00000610: 1c00 0000 da06 6669 6775 7265 da06 6361  ......figure..ca
-00000620: 6e76 6173 da0b 6d70 6c5f 636f 6e6e 6563  nvas..mpl_connec
-00000630: 74da 086f 6e5f 7072 6573 73da 0863 6964  t..on_press..cid
-00000640: 7072 6573 73da 0a6f 6e5f 7265 6c65 6173  press..on_releas
-00000650: 65da 0a63 6964 7265 6c65 6173 65da 096f  e..cidrelease..o
-00000660: 6e5f 6d6f 7469 6f6e da09 6369 646d 6f74  n_motion..cidmot
-00000670: 696f 6e72 2600 0000 7221 0000 0072 2100  ionr&...r!...r!.
-00000680: 0000 7222 0000 0072 1e00 0000 3400 0000  ..r"...r....4...
-00000690: 7312 0000 0000 020a 0106 ff06 030a 0106  s...............
-000006a0: ff06 030a 0106 ff7a 1644 7261 6767 6162  .......z.Draggab
-000006b0: 6c65 564c 696e 652e 636f 6e6e 6563 7463  leVLine.connectc
-000006c0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-000006d0: 0300 0000 4300 0000 735c 0000 007c 016a  ....C...s\...|.j
-000006e0: 007c 006a 016a 026b 0372 1264 0053 0074  .|.j.j.k.r.d.S.t
-000006f0: 036a 0464 0075 0172 2064 0053 007c 006a  .j.d.u.r d.S.|.j
-00000700: 01a0 057c 01a1 015c 027d 027d 037c 0273  ...|...\.}.}.|.s
-00000710: 3864 0053 007c 006a 01a0 06a1 005c 027d  8d.S.|.j.....\.}
-00000720: 047d 037c 047c 016a 0766 027c 005f 087c  .}.|.|.j.f.|._.|
-00000730: 0074 035f 0464 0053 0072 2800 0000 2909  .t._.d.S.r(...).
-00000740: da06 696e 6178 6573 721c 0000 00da 0461  ..inaxesr......a
-00000750: 7865 7372 1400 0000 da04 6c6f 636b da08  xesr......lock..
-00000760: 636f 6e74 6169 6e73 7225 0000 00da 0578  containsr%.....x
-00000770: 6461 7461 721d 0000 0029 0572 1f00 0000  datar....).r....
-00000780: da05 6576 656e 7472 3600 0000 da01 5f72  ..eventr6....._r
-00000790: 1800 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-000007a0: 0000 0072 2d00 0000 4000 0000 7314 0000  ...r-...@...s...
-000007b0: 0000 010e 0104 010a 0104 0110 0104 0104  ................
-000007c0: 010e 010c 017a 1744 7261 6767 6162 6c65  .....z.Draggable
-000007d0: 564c 696e 652e 6f6e 5f70 7265 7373 6302  VLine.on_pressc.
-000007e0: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-000007f0: 0000 0043 0000 0073 6c00 0000 7c00 6a00  ...C...sl...|.j.
-00000800: 6400 7500 720e 6400 5300 7401 6a02 7c00  d.u.r.d.S.t.j.|.
-00000810: 7501 721c 6400 5300 7c01 6a03 7c00 6a04  u.r.d.S.|.j.|.j.
-00000820: 6a05 6b03 722e 6400 5300 7c00 6a00 5c02  j.k.r.d.S.|.j.\.
-00000830: 7d02 7d03 7c01 6a06 7c03 1800 7d04 7c02  }.}.|.j.|...}.|.
-00000840: 7c04 1700 7d05 7c00 6a04 a007 7c05 7c05  |...}.|.j...|.|.
-00000850: 6702 a101 0100 7c00 6a04 6a08 6a09 a00a  g.....|.j.j.j...
-00000860: a100 0100 6400 5300 7228 0000 0029 0b72  ....d.S.r(...).r
-00000870: 1d00 0000 7214 0000 0072 3500 0000 7233  ....r....r5...r3
-00000880: 0000 0072 1c00 0000 7234 0000 0072 3700  ...r....r4...r7.
-00000890: 0000 5a09 7365 745f 7864 6174 6172 2a00  ..Z.set_xdatar*.
-000008a0: 0000 722b 0000 00da 0464 7261 7729 0672  ..r+.....draw).r
-000008b0: 1f00 0000 7238 0000 0072 1800 0000 5a06  ....r8...r....Z.
-000008c0: 7870 7265 7373 da02 6478 5a06 785f 636c  xpress..dxZ.x_cl
-000008d0: 6970 7221 0000 0072 2100 0000 7222 0000  ipr!...r!...r"..
-000008e0: 0072 3100 0000 4c00 0000 7316 0000 0000  .r1...L...s.....
-000008f0: 010a 0104 010a 0104 010e 0104 010a 010a  ................
-00000900: 0108 0110 017a 1844 7261 6767 6162 6c65  .....z.Draggable
-00000910: 564c 696e 652e 6f6e 5f6d 6f74 696f 6e63  VLine.on_motionc
-00000920: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000930: 0200 0000 4300 0000 732c 0000 0074 006a  ....C...s,...t.j
-00000940: 017c 0075 0172 0e64 0053 0064 0074 005f  .|.u.r.d.S.d.t._
-00000950: 0164 007c 005f 027c 006a 036a 046a 05a0  .d.|._.|.j.j.j..
-00000960: 06a1 0001 0064 0053 0072 2800 0000 2907  .....d.S.r(...).
-00000970: 7214 0000 0072 3500 0000 721d 0000 0072  r....r5...r....r
-00000980: 1c00 0000 722a 0000 0072 2b00 0000 723a  ....r*...r+...r:
-00000990: 0000 00a9 0272 1f00 0000 7238 0000 0072  .....r....r8...r
-000009a0: 2100 0000 7221 0000 0072 2200 0000 722f  !...r!...r"...r/
-000009b0: 0000 0059 0000 0073 0a00 0000 0001 0a01  ...Y...s........
-000009c0: 0401 0601 0601 7a19 4472 6167 6761 626c  ......z.Draggabl
-000009d0: 6556 4c69 6e65 2e6f 6e5f 7265 6c65 6173  eVLine.on_releas
-000009e0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-000009f0: 0000 0300 0000 4300 0000 733a 0000 007c  ......C...s:...|
-00000a00: 006a 006a 016a 02a0 037c 006a 04a1 0101  .j.j.j...|.j....
-00000a10: 007c 006a 006a 016a 02a0 037c 006a 05a1  .|.j.j.j...|.j..
-00000a20: 0101 007c 006a 006a 016a 02a0 037c 006a  ...|.j.j.j...|.j
-00000a30: 06a1 0101 0064 0053 0072 2800 0000 2907  .....d.S.r(...).
-00000a40: 721c 0000 0072 2a00 0000 722b 0000 005a  r....r*...r+...Z
-00000a50: 0e6d 706c 5f64 6973 636f 6e6e 6563 7472  .mpl_disconnectr
-00000a60: 2e00 0000 7230 0000 0072 3200 0000 7226  ....r0...r2...r&
-00000a70: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00000a80: 0000 da0a 6469 7363 6f6e 6e65 6374 6000  ....disconnect`.
-00000a90: 0000 7306 0000 0000 0112 0112 017a 1944  ..s..........z.D
-00000aa0: 7261 6767 6162 6c65 564c 696e 652e 6469  raggableVLine.di
-00000ab0: 7363 6f6e 6e65 6374 2903 7215 0000 0072  sconnect).r....r
-00000ac0: 1600 0000 7217 0000 0029 0dda 085f 5f6e  ....r....)...__n
-00000ad0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000ae0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000af0: 075f 5f64 6f63 5f5f 7235 0000 0072 2300  .__doc__r5...r#.
-00000b00: 0000 7227 0000 0072 2900 0000 721e 0000  ..r'...r)...r...
-00000b10: 0072 2d00 0000 7231 0000 0072 2f00 0000  .r-...r1...r/...
-00000b20: 723d 0000 0072 2100 0000 7221 0000 0072  r=...r!...r!...r
-00000b30: 2100 0000 7222 0000 0072 1400 0000 2200  !...r"...r....".
-00000b40: 0000 7314 0000 0008 0104 0204 020a 0708  ..s.............
-00000b50: 0308 0308 0c08 0c08 0d08 0772 1400 0000  ...........r....
-00000b60: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000b70: 0002 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
-00000b80: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
-00000b90: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
-00000ba0: 5a06 6408 5300 2909 da0d 5261 6e67 6553  Z.d.S.)...RangeS
-00000bb0: 656c 6563 746f 727a 5763 6c61 7373 2074  electorzWclass t
-00000bc0: 6861 7420 6372 6561 7465 7320 6120 7261  hat creates a ra
-00000bd0: 6e67 6573 656c 6563 746f 7220 696e 2061  ngeselector in a
-00000be0: 2070 6c6f 7420 636f 6e73 6973 7469 6e67   plot consisting
-00000bf0: 206f 6620 7477 6f20 6472 6167 6761 626c   of two draggabl
-00000c00: 6520 7665 7274 6963 616c 206c 696e 6573  e vertical lines
-00000c10: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00000c20: 0003 0000 0003 0000 0073 2a00 0000 7c01  .........s*...|.
-00000c30: 8800 5f00 7c02 7c03 6702 8800 5f01 8700  .._.|.|.g..._...
-00000c40: 6601 6401 6402 8408 8800 6a01 4400 8301  f.d.d.....j.D...
-00000c50: 8800 5f02 6400 5300 2903 4e63 0100 0000  .._.d.S.).Nc....
-00000c60: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000c70: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
-00000c80: 0174 0088 006a 017c 0183 0291 0271 0453  .t...j.|.....q.S
-00000c90: 0072 2100 0000 2902 7214 0000 0072 2000  .r!...).r....r .
-00000ca0: 0000 2902 da02 2e30 da03 706f 7372 2600  ..)....0..posr&.
-00000cb0: 0000 7221 0000 0072 2200 0000 da0a 3c6c  ..r!...r".....<l
-00000cc0: 6973 7463 6f6d 703e 6c00 0000 f300 0000  istcomp>l.......
-00000cd0: 007a 2a52 616e 6765 5365 6c65 6374 6f72  .z*RangeSelector
-00000ce0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-00000cf0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0372  s>.<listcomp>).r
-00000d00: 2000 0000 7244 0000 00da 0a64 7261 675f   ...rD.....drag_
-00000d10: 6c69 6e65 7329 0472 1f00 0000 7220 0000  lines).r....r ..
-00000d20: 005a 0470 6f73 31da 0470 6f73 3272 2100  .Z.pos1..pos2r!.
-00000d30: 0000 7226 0000 0072 2200 0000 7223 0000  ..r&...r"...r#..
-00000d40: 0069 0000 0073 0600 0000 0001 0601 0a01  .i...s..........
-00000d50: 7a16 5261 6e67 6553 656c 6563 746f 722e  z.RangeSelector.
-00000d60: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00000d70: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00000d80: 0073 1c00 0000 6401 6402 8400 7c00 6a00  .s....d.d...|.j.
-00000d90: 4400 8301 7d01 7c01 a001 a100 0100 7c01  D...}.|.......|.
-00000da0: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00000db0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00000dc0: 0000 0067 007c 005d 0c7d 017c 01a0 00a1  ...g.|.].}.|....
-00000dd0: 0091 0271 0453 0072 2100 0000 2901 7227  ...q.S.r!...).r'
-00000de0: 0000 0029 0272 4300 0000 da08 6472 6167  ...).rC.....drag
-00000df0: 6c69 6e65 7221 0000 0072 2100 0000 7222  liner!...r!...r"
-00000e00: 0000 0072 4500 0000 6f00 0000 7246 0000  ...rE...o...rF..
-00000e10: 007a 2b52 616e 6765 5365 6c65 6374 6f72  .z+RangeSelector
-00000e20: 2e67 6574 5f72 616e 6765 2e3c 6c6f 6361  .get_range.<loca
-00000e30: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2902  ls>.<listcomp>).
-00000e40: 7247 0000 00da 0473 6f72 7429 0272 1f00  rG.....sort).r..
-00000e50: 0000 7244 0000 0072 2100 0000 7221 0000  ..rD...r!...r!..
-00000e60: 0072 2200 0000 da09 6765 745f 7261 6e67  .r".....get_rang
-00000e70: 656e 0000 0073 0600 0000 0001 1001 0801  en...s..........
-00000e80: 7a17 5261 6e67 6553 656c 6563 746f 722e  z.RangeSelector.
-00000e90: 6765 745f 7261 6e67 6563 0100 0000 0000  get_rangec......
-00000ea0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000eb0: 0000 7318 0000 007c 006a 0044 005d 0c7d  ..s....|.j.D.].}
-00000ec0: 017c 01a0 01a1 0001 0071 0664 0053 0072  .|.......q.d.S.r
-00000ed0: 2800 0000 2902 7247 0000 0072 2900 0000  (...).rG...r)...
-00000ee0: 2902 721f 0000 0072 4900 0000 7221 0000  ).r....rI...r!..
-00000ef0: 0072 2100 0000 7222 0000 0072 2900 0000  .r!...r"...r)...
-00000f00: 7300 0000 7304 0000 0000 010a 017a 1452  s...s........z.R
-00000f10: 616e 6765 5365 6c65 6374 6f72 2e72 656d  angeSelector.rem
-00000f20: 6f76 654e 2907 723e 0000 0072 3f00 0000  oveN).r>...r?...
-00000f30: 7240 0000 0072 4100 0000 7223 0000 0072  r@...rA...r#...r
-00000f40: 4b00 0000 7229 0000 0072 2100 0000 7221  K...r)...r!...r!
-00000f50: 0000 0072 2100 0000 7222 0000 0072 4200  ...r!...r"...rB.
-00000f60: 0000 6600 0000 7308 0000 0008 0104 0208  ..f...s.........
-00000f70: 0508 0572 4200 0000 6300 0000 0000 0000  ...rB...c.......
-00000f80: 0000 0000 0000 0000 0003 0000 0000 0000  ................
-00000f90: 0073 4800 0000 6500 5a01 6400 5a02 6401  .sH...e.Z.d.Z.d.
-00000fa0: 5a03 6504 a005 a100 5a06 6402 6403 8400  Z.e.....Z.d.d...
-00000fb0: 5a07 8700 6601 6404 6405 8408 5a08 6406  Z...f.d.d...Z.d.
-00000fc0: 6407 8400 5a09 6408 6409 8400 5a0a 640a  d...Z.d.d...Z.d.
-00000fd0: 640b 8400 5a0b 8700 0400 5a0c 5300 290c  d...Z.....Z.S.).
-00000fe0: da0a 506c 6f74 5769 6467 6574 7a54 5174  ..PlotWidgetzTQt
-00000ff0: 2077 6964 6765 7420 746f 2068 6f6c 6420   widget to hold 
-00001000: 7468 6520 6d61 7470 6c6f 746c 6962 2063  the matplotlib c
-00001010: 616e 7661 7320 616e 6420 7468 6520 746f  anvas and the to
-00001020: 6f6c 7320 666f 7220 696e 7465 7261 6374  ols for interact
-00001030: 696e 6720 7769 7468 2074 6865 2070 6c6f  ing with the plo
-00001040: 7473 6304 0000 0000 0000 0000 0000 0005  tsc.............
-00001050: 0000 0007 0000 004b 0000 0073 3801 0000  .......K...s8...
-00001060: 7400 6a01 a002 7c00 a101 0100 7c00 a003  t.j...|.....|...
-00001070: 7400 a004 a100 a101 0100 7405 7c01 7c02  t.........t.|.|.
-00001080: 7c03 6603 6900 7c04 a401 8e01 7c00 5f06  |.f.i.|.....|._.
-00001090: 7407 7c00 6a06 7c00 8302 7c00 5f08 7c00  t.|.j.|...|._.|.
-000010a0: 6a08 a009 a100 0100 7400 a00a 6401 a101  j.......t...d...
-000010b0: 7c00 5f0b 7c00 6a0b a00c 6402 a101 0100  |._.|.j...d.....
-000010c0: 7c00 6a0b a00d 740e a00f 6403 6404 740e  |.j...t...d.d.t.
-000010d0: 6a0f 6a10 a103 a101 0100 7c00 6a0b 6a11  j.j.......|.j.j.
-000010e0: a012 7c00 6a13 a101 0100 7c00 6a08 a009  ..|.j.....|.j...
-000010f0: a100 0100 7400 a00a 6405 a101 7c00 5f14  ....t...d...|._.
-00001100: 7c00 6a14 a00c 6406 a101 0100 7c00 6a14  |.j...d.....|.j.
-00001110: a00d 740e a00f 6403 6404 740e 6a0f 6a10  ..t...d.d.t.j.j.
-00001120: a103 a101 0100 7c00 6a14 6a11 a012 7c00  ......|.j.j...|.
-00001130: 6a15 a101 0100 7c00 6a08 a009 a100 0100  j.....|.j.......
-00001140: 7c00 6a08 a016 7c00 6a0b a101 0100 7c00  |.j...|.j.....|.
-00001150: 6a08 a016 7c00 6a14 a101 0100 7c00 6a08  j...|.j.....|.j.
-00001160: a009 a100 0100 7c00 a017 a100 a018 7c00  ......|.......|.
-00001170: 6a08 a101 0100 7c00 a017 a100 a018 7c00  j.....|.......|.
-00001180: 6a06 a101 0100 7c00 6a19 a012 7c00 6a1a  j.....|.j...|.j.
-00001190: a101 0100 6400 5300 2907 4e7a 0b55 7064  ....d.S.).Nz.Upd
-000011a0: 6174 6520 4461 7461 7a0b 5550 4441 5445  ate Dataz.UPDATE
-000011b0: 2044 4154 415a 0554 696d 6573 e90c 0000   DATAZ.Times....
-000011c0: 007a 1c41 6374 6976 6174 652f 436c 6561  .z.Activate/Clea
-000011d0: 7220 5261 6e67 6553 656c 6563 746f 727a  r RangeSelectorz
-000011e0: 0e52 414e 4745 2053 454c 4543 544f 5229  .RANGE SELECTOR)
-000011f0: 1b72 0d00 0000 da07 5157 6964 6765 7472  .r......QWidgetr
-00001200: 2300 0000 da09 7365 744c 6179 6f75 74da  #.....setLayout.
-00001210: 0b51 5642 6f78 4c61 796f 7574 da0a 506c  .QVBoxLayout..Pl
-00001220: 6f74 4361 6e76 6173 722b 0000 00da 114e  otCanvasr+.....N
-00001230: 6176 6967 6174 696f 6e54 6f6f 6c62 6172  avigationToolbar
-00001240: da07 746f 6f6c 6261 725a 0c61 6464 5365  ..toolbarZ.addSe
-00001250: 7061 7261 746f 725a 0751 4163 7469 6f6e  paratorZ.QAction
-00001260: 5a0a 7570 6461 7465 4461 7461 5a0b 7365  Z.updateDataZ.se
-00001270: 7449 636f 6e54 6578 74da 0773 6574 466f  tIconText..setFo
-00001280: 6e74 720c 0000 00da 0551 466f 6e74 5a04  ntr......QFontZ.
-00001290: 426f 6c64 5a09 7472 6967 6765 7265 6472  BoldZ.triggeredr
-000012a0: 1e00 0000 da0b 7570 6461 7465 5f64 6174  ......update_dat
-000012b0: 615a 0e41 4373 686f 7773 656c 6563 746f  aZ.ACshowselecto
-000012c0: 72da 145f 746f 6767 6c65 5f73 686f 7773  r.._toggle_shows
-000012d0: 656c 6563 746f 725a 0961 6464 4163 7469  electorZ.addActi
-000012e0: 6f6e da06 6c61 796f 7574 da09 6164 6457  on..layout..addW
-000012f0: 6964 6765 74da 0772 6573 697a 6564 da0b  idget..resized..
-00001300: 7570 6461 7465 5f70 6c6f 7429 0572 1f00  update_plot).r..
-00001310: 0000 da06 6669 7474 6572 da06 786c 6162  ....fitter..xlab
-00001320: 656c da06 796c 6162 656c da06 6b77 6172  el..ylabel..kwar
-00001330: 6773 7221 0000 0072 2100 0000 7222 0000  gsr!...r!...r"..
-00001340: 0072 2300 0000 7d00 0000 732e 0000 0000  .r#...}...s.....
-00001350: 010c 020e 0116 010e 010a 050c 010c 011a  ................
-00001360: 0110 020a 020c 010c 011a 0110 020a 020e  ................
-00001370: 010e 020a 0110 0110 0206 0104 ff7a 1350  .............z.P
-00001380: 6c6f 7457 6964 6765 742e 5f5f 696e 6974  lotWidget.__init
-00001390: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-000013a0: 0000 0003 0000 0003 0000 0073 1a00 0000  ...........s....
-000013b0: 7c00 6a00 a001 a100 0100 7402 7403 7c00  |.j.......t.t.|.
-000013c0: 8302 a004 7c01 a101 5300 7228 0000 0029  ....|...S.r(...)
-000013d0: 0572 5a00 0000 da04 656d 6974 da05 7375  .rZ.....emit..su
-000013e0: 7065 7272 4c00 0000 da0b 7265 7369 7a65  perrL.....resize
-000013f0: 4576 656e 7472 3c00 0000 a901 da09 5f5f  Eventr<.......__
-00001400: 636c 6173 735f 5f72 2100 0000 7222 0000  class__r!...r"..
-00001410: 0072 6200 0000 a100 0000 7304 0000 0000  .rb.......s.....
-00001420: 010a 017a 1650 6c6f 7457 6964 6765 742e  ...z.PlotWidget.
-00001430: 7265 7369 7a65 4576 656e 7463 0100 0000  resizeEventc....
-00001440: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001450: 4300 0000 730e 0000 007c 006a 00a0 01a1  C...s....|.j....
-00001460: 0001 0064 0053 0072 2800 0000 2902 722b  ...d.S.r(...).r+
-00001470: 0000 0072 5b00 0000 7226 0000 0072 2100  ...r[...r&...r!.
-00001480: 0000 7221 0000 0072 2200 0000 725b 0000  ..r!...r"...r[..
-00001490: 00a5 0000 0073 0200 0000 0001 7a16 506c  .....s......z.Pl
-000014a0: 6f74 5769 6467 6574 2e75 7064 6174 655f  otWidget.update_
-000014b0: 706c 6f74 6301 0000 0000 0000 0000 0000  plotc...........
-000014c0: 0001 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-000014d0: 0000 7c00 6a00 a001 a100 0100 6400 5300  ..|.j.......d.S.
-000014e0: 7228 0000 0029 0272 2b00 0000 da14 746f  r(...).r+.....to
-000014f0: 6767 6c65 5f72 616e 6765 7365 6c65 6374  ggle_rangeselect
-00001500: 6f72 7226 0000 0072 2100 0000 7221 0000  orr&...r!...r!..
-00001510: 0072 2200 0000 7257 0000 00a8 0000 0073  .r"...rW.......s
-00001520: 0200 0000 0001 7a1f 506c 6f74 5769 6467  ......z.PlotWidg
-00001530: 6574 2e5f 746f 6767 6c65 5f73 686f 7773  et._toggle_shows
-00001540: 656c 6563 746f 7263 0100 0000 0000 0000  electorc........
-00001550: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-00001560: 7304 0000 0064 0053 0072 2800 0000 7221  s....d.S.r(...r!
-00001570: 0000 0072 2600 0000 7221 0000 0072 2100  ...r&...r!...r!.
-00001580: 0000 7222 0000 0072 5600 0000 ab00 0000  ..r"...rV.......
-00001590: 7302 0000 0000 017a 1650 6c6f 7457 6964  s......z.PlotWid
-000015a0: 6765 742e 7570 6461 7465 5f64 6174 6129  get.update_data)
-000015b0: 0d72 3e00 0000 723f 0000 0072 4000 0000  .r>...r?...r@...
-000015c0: 7241 0000 0072 0b00 0000 da0a 7079 7174  rA...r......pyqt
-000015d0: 5369 676e 616c 725a 0000 0072 2300 0000  SignalrZ...r#...
-000015e0: 7262 0000 0072 5b00 0000 7257 0000 0072  rb...r[...rW...r
-000015f0: 5600 0000 da0d 5f5f 636c 6173 7363 656c  V.....__classcel
-00001600: 6c5f 5f72 2100 0000 7221 0000 0072 6300  l__r!...r!...rc.
-00001610: 0000 7222 0000 0072 4c00 0000 7800 0000  ..r"...rL...x...
-00001620: 730e 0000 0008 0104 0208 0208 240c 0408  s...........$...
-00001630: 0308 0372 4c00 0000 6300 0000 0000 0000  ...rL...c.......
-00001640: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00001650: 0073 7800 0000 6500 5a01 6400 5a02 6401  .sx...e.Z.d.Z.d.
-00001660: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
-00001670: 5a05 6406 6407 8400 5a06 6408 6409 8400  Z.d.d...Z.d.d...
-00001680: 5a07 640a 640b 8400 5a08 640c 640d 8400  Z.d.d...Z.d.d...
-00001690: 5a09 640e 640f 8400 5a0a 6410 6411 8400  Z.d.d...Z.d.d...
-000016a0: 5a0b 6412 6413 8400 5a0c 6414 6415 8400  Z.d.d...Z.d.d...
-000016b0: 5a0d 6416 6417 8400 5a0e 6418 6419 8400  Z.d.d...Z.d.d...
-000016c0: 5a0f 641a 641b 8400 5a10 641c 5300 291d  Z.d.d...Z.d.S.).
-000016d0: 7251 0000 007a 6063 6c61 7373 2074 6f20  rQ...z`class to 
-000016e0: 686f 6c64 2061 2063 616e 7661 7320 7769  hold a canvas wi
-000016f0: 7468 2061 206d 6174 706c 6f74 6c69 6220  th a matplotlib 
-00001700: 6669 6775 7265 2061 6e64 2074 776f 2073  figure and two s
-00001710: 7562 706c 6f74 7320 666f 7220 706c 6f74  ubplots for plot
-00001720: 7469 6e67 2064 6174 6120 616e 6420 7265  ting data and re
-00001730: 7369 6475 616c 7363 0400 0000 0000 0000  sidualsc........
-00001740: 0000 0000 0a00 0000 0900 0000 0b00 0000  ................
-00001750: 7358 0400 007c 0188 005f 007c 016a 0188  sX...|..._.|.j..
-00001760: 005f 0164 0088 005f 0264 0088 005f 0364  ._.d..._.d..._.d
-00001770: 0088 005f 0464 0088 005f 057c 0488 005f  ..._.d..._.|..._
-00001780: 0674 0774 0883 0188 005f 0964 0188 006a  .t.t....._.d...j
-00001790: 0676 0172 4464 026e 0888 006a 0664 0119  .v.rDd.n...j.d..
-000017a0: 0088 005f 0a64 0388 006a 0676 0072 6488  ..._.d...j.v.rd.
-000017b0: 006a 0664 0319 006e 0264 0488 005f 0b64  .j.d...n.d..._.d
-000017c0: 0388 006a 0676 0072 7c88 006a 0664 033d  ...j.v.r|..j.d.=
-000017d0: 0064 0588 006a 0676 0072 8e88 006a 0664  .d...j.v.r...j.d
-000017e0: 053d 0064 0188 006a 0676 0072 a088 006a  .=.d...j.v.r...j
-000017f0: 0664 013d 0064 0688 006a 0676 0072 be7c  .d.=.d...j.v.r.|
-00001800: 0464 0619 0088 006a 0964 073c 007c 0464  .d.....j.d.<.|.d
-00001810: 063d 0064 0888 006a 0676 0072 dc7c 0464  .=.d...j.v.r.|.d
-00001820: 0819 0088 006a 0964 093c 007c 0464 083d  .....j.d.<.|.d.=
-00001830: 0064 0a88 006a 0676 0072 fa7c 0464 0a19  .d...j.v.r.|.d..
-00001840: 0088 006a 0964 0b3c 007c 0464 0a3d 0064  ...j.d.<.|.d.=.d
-00001850: 0c88 006a 0676 0090 0172 1a7c 0464 0c19  ...j.v...r.|.d..
-00001860: 0088 006a 0964 0d3c 007c 0464 0c3d 0088  ...j.d.<.|.d.=..
-00001870: 006a 0c66 0069 0088 006a 06a4 018e 0188  .j.f.i...j......
-00001880: 005f 0688 006a 0d66 0069 0088 006a 09a4  ._...j.f.i...j..
-00001890: 018e 0188 005f 0974 0e74 0f64 0e19 0064  ....._.t.t.d...d
-000018a0: 0f64 108d 0288 005f 1074 11a0 1288 0088  .d....._.t......
-000018b0: 006a 10a1 0201 0074 11a0 1388 0074 146a  .j.....t.....t.j
-000018c0: 156a 1674 146a 156a 16a1 0301 0074 11a0  .j.t.j.j.....t..
-000018d0: 1788 00a1 0101 0064 0088 005f 1888 006a  .......d..._...j
-000018e0: 10a0 1964 1164 12a1 027d 0588 006a 10a0  ...d.d...}...j..
-000018f0: 1a7c 0564 1319 00a1 0188 005f 1b88 006a  .|.d......._...j
-00001900: 1b6a 1ca0 1d64 14a1 0101 0088 006a 106a  .j...d.......j.j
-00001910: 1a7c 0564 1564 1685 0264 1566 0219 0088  .|.d.d...d.f....
-00001920: 006a 1b64 178d 0288 005f 1e88 006a 1e6a  .j.d....._...j.j
-00001930: 1ca0 1d88 006a 0ba1 0101 0088 006a 1ea0  .....j.......j..
-00001940: 1fa1 0001 0088 006a 1ba0 1fa1 0001 0088  .......j........
-00001950: 006a 1e6a 207c 0374 0f64 1819 0074 0f64  .j.j |.t.d...t.d
-00001960: 1919 0064 1a8d 0301 0088 006a 1b6a 2064  ...d.......j.j d
-00001970: 1b74 0f64 1819 0074 0f64 1919 0064 1a8d  .t.d...t.d...d..
-00001980: 0301 0088 006a 1b6a 217c 0274 0f64 1819  .....j.j!|.t.d..
-00001990: 0074 0f64 1919 0064 1a8d 0301 0088 006a  .t.d...d.......j
-000019a0: 1e6a 2267 0067 0066 0269 0088 006a 06a4  .j"g.g.f.i...j..
-000019b0: 018e 015c 0188 005f 2388 006a 1e6a 2267  ...\..._#..j.j"g
-000019c0: 0067 0066 0269 0088 006a 09a4 018e 015c  .g.f.i...j.....\
-000019d0: 0188 005f 2488 006a 1b6a 2267 0067 0064  ..._$..j.j"g.g.d
-000019e0: 1c64 1d64 1264 1e8d 055c 0188 005f 2564  .d.d.d...\..._%d
-000019f0: 0088 005f 2688 006a 1e6a 2764 1f64 0f64  ..._&..j.j'd.d.d
-00001a00: 2074 0f64 1819 0074 0f64 1919 0064 219c   t.d...t.d...d!.
-00001a10: 0264 228d 0401 0074 2874 296a 2a64 2364  .d"....t(t)j*d#d
-00001a20: 2064 248d 0264 2564 2064 268d 037d 0688   d$..d%d d&..}..
-00001a30: 006a 1e6a 2b64 2764 2864 2974 0f64 1819  .j.j+d'd(d)t.d..
-00001a40: 0074 0f64 1919 007c 0664 2a8d 0688 005f  .t.d...|.d*...._
-00001a50: 2c88 006a 2ca0 2da1 0001 0088 006a 006a  ,..j,.-......j.j
-00001a60: 2e90 0373 2888 006a 23a0 2f88 006a 016a  ...s(..j#./..j.j
-00001a70: 3088 006a 016a 31a1 0201 006e 3288 006a  0..j.j1....n2..j
-00001a80: 23a0 32a1 0001 0088 006a 3388 006a 016a  #.2......j3..j.j
-00001a90: 3164 2b66 0269 0088 006a 06a4 018e 015c  1d+f.i...j.....\
-00001aa0: 0188 005f 2388 006a 1ea0 27a1 0001 0088  ..._#..j..'.....
-00001ab0: 006a 016a 3464 0075 0190 0372 9888 006a  .j.j4d.u...r...j
-00001ac0: 1e6a 3588 006a 016a 3088 006a 016a 3188  .j5..j.j0..j.j1.
-00001ad0: 006a 016a 3464 2c74 0f64 2d19 0074 0f64  .j.j4d,t.d-..t.d
-00001ae0: 2e19 0064 1664 2f8d 0788 005f 3688 006a  ...d.d/...._6..j
-00001af0: 016a 3764 0075 0190 0372 d688 006a 1e6a  .j7d.u...r...j.j
-00001b00: 3588 006a 016a 3088 006a 016a 3188 006a  5..j.j0..j.j1..j
-00001b10: 016a 3764 2c74 0f64 3019 0074 0f64 3119  .j7d,t.d0..t.d1.
-00001b20: 0064 1664 328d 0788 005f 3888 006a 1ea0  .d.d2...._8..j..
-00001b30: 39a1 0088 006a 1ea0 3aa1 0088 006a 1ba0  9....j..:....j..
-00001b40: 39a1 0088 006a 1ba0 3aa1 0066 0444 005d  9....j..:..f.D.]
-00001b50: 3c7d 077c 0744 005d 307d 087c 08a0 3b74  <}.|.D.]0}.|..;t
-00001b60: 0f64 3319 00a1 0101 007c 08a0 3c74 0f64  .d3......|..<t.d
-00001b70: 3419 00a1 0101 007c 08a0 3d74 0f64 3519  4......|..=t.d5.
-00001b80: 00a1 0101 0090 0471 0290 0371 fa87 0066  .......q...q...f
-00001b90: 0164 3664 3784 087d 0988 006a 106a 3ea0  .d6d7..}...j.j>.
-00001ba0: 3f64 387c 09a1 0201 0064 0053 0029 394e  ?d8|.....d.S.)9N
-00001bb0: da07 636f 6d70 6c65 7846 da05 7469 746c  ..complexF..titl
-00001bc0: 65da 0444 6174 61da 066d 6574 686f 64da  e..Data..method.
-00001bd0: 0d66 6974 6c69 6e65 5f63 6f6c 6f72 721b  .fitline_colorr.
-00001be0: 0000 005a 1166 6974 6c69 6e65 5f6c 696e  ...Z.fitline_lin
-00001bf0: 6573 7479 6c65 721a 0000 005a 1166 6974  estyler....Z.fit
-00001c00: 6c69 6e65 5f6c 696e 6577 6964 7468 7219  line_linewidthr.
-00001c10: 0000 005a 0d66 6974 6c69 6e65 5f6c 6162  ...Z.fitline_lab
-00001c20: 656c da05 6c61 6265 6cda 0746 4947 5f44  el..label..FIG_D
-00001c30: 5049 5429 02da 0364 7069 5a0c 7469 6768  PIT)...dpiZ.tigh
-00001c40: 745f 6c61 796f 7574 e903 0000 0072 1000  t_layout.....r..
-00001c50: 0000 2902 e902 0000 0072 0100 0000 7a0e  ..)......r....z.
-00001c60: 5265 7369 6475 616c 2047 7261 7068 7201  Residual Graphr.
-00001c70: 0000 0072 7100 0000 2901 da06 7368 6172  ...rq...)...shar
-00001c80: 6578 da09 5445 5854 5f46 4f4e 54da 0954  ex..TEXT_FONT..T
-00001c90: 4558 545f 5349 5a45 2902 da08 666f 6e74  EXT_SIZE)...font
-00001ca0: 6e61 6d65 da08 666f 6e74 7369 7a65 da08  name..fontsize..
-00001cb0: 7265 7369 6475 616c da01 6bda 012e 2903  residual..k...).
-00001cc0: 721b 0000 00da 066d 6172 6b65 72da 026c  r......marker..l
-00001cd0: 77da 0462 6573 74e7 0000 0000 0000 e03f  w..best........?
-00001ce0: 2902 da06 6661 6d69 6c79 da04 7369 7a65  )...family..size
-00001cf0: 2904 da03 6c6f 635a 0866 616e 6379 626f  )...locZ.fancybo
-00001d00: 785a 0a66 7261 6d65 616c 7068 61da 0470  xZ.framealpha..p
-00001d10: 726f 70da 0572 6f75 6e64 2901 da03 7061  rop..round)...pa
-00001d20: 647a 0330 2e39 2903 5a08 626f 7873 7479  dz.0.9).Z.boxsty
-00001d30: 6c65 da02 6663 da05 616c 7068 61da 0029  le..fc..alpha..)
-00001d40: 0272 7d00 0000 727d 0000 007a 0d61 7865  .r}...r}...z.axe
-00001d50: 7320 6672 6163 7469 6f6e 2905 da02 7879  s fraction)...xy
-00001d60: 5a08 7879 636f 6f72 6473 7275 0000 0072  Z.xycoordsru...r
-00001d70: 7f00 0000 da04 6262 6f78 da01 6fda 046e  ......bbox..o..n
-00001d80: 6f6e 65da 0b42 4152 5f59 5f43 4f4c 4f52  one..BAR_Y_COLOR
-00001d90: da0f 4241 525f 595f 5448 4943 4b4e 4553  ..BAR_Y_THICKNES
-00001da0: 5329 05da 0479 6572 72da 0366 6d74 721b  S)...yerr..fmtr.
-00001db0: 0000 00da 0a65 6c69 6e65 7769 6474 68da  .....elinewidth.
-00001dc0: 0763 6170 7369 7a65 da0b 4241 525f 585f  .capsize..BAR_X_
-00001dd0: 434f 4c4f 52da 0f42 4152 5f58 5f54 4849  COLOR..BAR_X_THI
-00001de0: 434b 4e45 5353 2905 da04 7865 7272 728e  CKNESS)...xerrr.
-00001df0: 0000 0072 1b00 0000 728f 0000 0072 9000  ...r....r....r..
-00001e00: 0000 da0a 5449 434b 5f43 4f4c 4f52 da09  ....TICK_COLOR..
-00001e10: 5449 434b 5f46 4f4e 54da 0954 4943 4b5f  TICK_FONT..TICK_
-00001e20: 5349 5a45 6301 0000 0000 0000 0000 0000  SIZEc...........
-00001e30: 0002 0000 0008 0000 0013 0000 0073 5a00  .............sZ.
-00001e40: 0000 7c00 6a00 6401 6b02 7256 7401 a002  ..|.j.d.k.rVt...
-00001e50: a100 8f34 7d01 8800 6a03 a004 7c01 a101  ...4}...j...|...
-00001e60: 0100 7405 a006 a100 a007 7408 a009 7c01  ..t.......t...|.
-00001e70: a00a a100 a101 a101 0100 5700 6400 0400  ..........W.d...
-00001e80: 0400 8303 0100 6e10 3100 734c 3000 0100  ......n.1.sL0...
-00001e90: 0100 0100 5900 0100 6400 5300 2902 4e7a  ....Y...d.S.).Nz
-00001ea0: 0663 7472 6c2b 6329 0bda 036b 6579 da02  .ctrl+c)...key..
-00001eb0: 696f da07 4279 7465 7349 4fda 0366 6967  io..BytesIO..fig
-00001ec0: 5a07 7361 7665 6669 6772 0f00 0000 da09  Z.savefigr......
-00001ed0: 636c 6970 626f 6172 645a 0873 6574 496d  clipboardZ.setIm
-00001ee0: 6167 6572 0e00 0000 5a08 6672 6f6d 4461  ager....Z.fromDa
-00001ef0: 7461 da08 6765 7476 616c 7565 2902 7238  ta..getvalue).r8
-00001f00: 0000 00da 0662 7566 6665 7272 2600 0000  .....bufferr&...
-00001f10: 7221 0000 0072 2200 0000 da17 6164 645f  r!...r".....add_
-00001f20: 6669 6775 7265 5f74 6f5f 636c 6970 626f  figure_to_clipbo
-00001f30: 6172 6468 0100 0073 0c00 0000 0001 0a01  ardh...s........
-00001f40: 0a01 0c01 0801 0cff 7a34 506c 6f74 4361  ........z4PlotCa
-00001f50: 6e76 6173 2e5f 5f69 6e69 745f 5f2e 3c6c  nvas.__init__.<l
-00001f60: 6f63 616c 733e 2e61 6464 5f66 6967 7572  ocals>.add_figur
-00001f70: 655f 746f 5f63 6c69 7062 6f61 7264 5a0f  e_to_clipboardZ.
-00001f80: 6b65 795f 7072 6573 735f 6576 656e 7429  key_press_event)
-00001f90: 4072 5c00 0000 da04 6461 7461 da07 6669  @r\.....data..fi
-00001fa0: 746c 696e 65da 0972 6573 6964 7561 6c73  tline..residuals
-00001fb0: da11 636f 6d70 6c65 785f 7265 7369 6475  ..complex_residu
-00001fc0: 616c 73da 1269 6e69 7469 616c 5f67 7565  als..initial_gue
-00001fd0: 7373 5f6c 696e 6572 5f00 0000 7203 0000  ss_liner_...r...
-00001fe0: 00da 0373 7472 da0e 6669 746c 696e 655f  ...str..fitline_
-00001ff0: 6b77 6172 6773 7268 0000 005a 0961 7831  kwargsrh...Z.ax1
-00002000: 5f74 6974 6c65 da15 7365 745f 6461 7461  _title..set_data
-00002010: 5f70 6c6f 745f 6465 6661 756c 74da 1473  _plot_default..s
-00002020: 6574 5f66 6974 5f70 6c6f 745f 6465 6661  et_fit_plot_defa
-00002030: 756c 7472 0900 0000 7211 0000 0072 9a00  ultr....r....r..
-00002040: 0000 da0c 4669 6775 7265 4361 6e76 6173  ....FigureCanvas
-00002050: 7223 0000 005a 0d73 6574 5369 7a65 506f  r#...Z.setSizePo
-00002060: 6c69 6379 720d 0000 005a 0b51 5369 7a65  licyr....Z.QSize
-00002070: 506f 6c69 6379 da09 4578 7061 6e64 696e  Policy..Expandin
-00002080: 675a 0e75 7064 6174 6547 656f 6d65 7472  gZ.updateGeometr
-00002090: 79da 0e72 616e 6765 5f73 656c 6563 746f  y..range_selecto
-000020a0: 725a 0c61 6464 5f67 7269 6473 7065 63da  rZ.add_gridspec.
-000020b0: 0b61 6464 5f73 7562 706c 6f74 da03 6178  .add_subplot..ax
-000020c0: 3272 6900 0000 da08 7365 745f 7465 7874  2ri.....set_text
-000020d0: da03 6178 31da 0467 7269 64da 0a73 6574  ..ax1..grid..set
-000020e0: 5f79 6c61 6265 6cda 0a73 6574 5f78 6c61  _ylabel..set_xla
-000020f0: 6265 6cda 0470 6c6f 745a 0964 6174 615f  bel..plotZ.data_
-00002100: 6c69 6e65 da0b 6669 7474 6564 5f6c 696e  line..fitted_lin
-00002110: 65da 0d72 6573 6964 7561 6c5f 6c69 6e65  e..residual_line
-00002120: da08 7a65 726f 5f72 6573 da06 6c65 6765  ..zero_res..lege
-00002130: 6e64 da04 6469 6374 da07 7061 7463 6865  nd..dict..patche
-00002140: 735a 0842 6f78 5374 796c 655a 0861 6e6e  sZ.BoxStyleZ.ann
-00002150: 6f74 6174 65da 0a72 6573 756c 745f 626f  otate..result_bo
-00002160: 785a 0964 7261 6767 6162 6c65 da0a 6973  xZ.draggable..is
-00002170: 5f63 6f6d 706c 6578 da08 7365 745f 6461  _complex..set_da
-00002180: 7461 7218 0000 00da 0179 7229 0000 00da  tar......yr)....
-00002190: 0c70 6c6f 745f 636f 6d70 6c65 78da 0279  .plot_complex..y
-000021a0: 65da 0865 7272 6f72 6261 725a 0879 6572  e..errorbarZ.yer
-000021b0: 726f 6261 72da 0278 655a 0878 6572 726f  robar..xeZ.xerro
-000021c0: 6261 72da 0f67 6574 5f78 7469 636b 6c61  bar..get_xtickla
-000021d0: 6265 6c73 5a0f 6765 745f 7974 6963 6b6c  belsZ.get_ytickl
-000021e0: 6162 656c 735a 0973 6574 5f63 6f6c 6f72  abelsZ.set_color
-000021f0: 5a12 7365 745f 666f 6e74 7072 6f70 6572  Z.set_fontproper
-00002200: 7469 6573 5a0c 7365 745f 666f 6e74 7369  tiesZ.set_fontsi
-00002210: 7a65 722b 0000 0072 2c00 0000 290a 721f  zer+...r,...).r.
-00002220: 0000 0072 5c00 0000 725d 0000 0072 5e00  ...r\...r]...r^.
-00002230: 0000 725f 0000 00da 0267 735a 0962 626f  ..r_.....gsZ.bbo
-00002240: 785f 6172 6773 da06 6c61 6265 6c73 da04  x_args..labels..
-00002250: 7469 636b 729e 0000 0072 2100 0000 7226  tickr....r!...r&
-00002260: 0000 0072 2200 0000 7223 0000 00b2 0000  ...r"...r#......
-00002270: 0073 1401 0000 0001 0601 0801 0601 0601  .s..............
-00002280: 0601 0601 0601 0a02 16ff 0406 16ff 0404  ................
-00002290: 0a01 0801 0a01 0801 0a01 0803 0a01 0e01  ................
-000022a0: 0601 0a01 0e01 0601 0a01 0e01 0601 0c01  ................
-000022b0: 0e01 0603 1401 1403 1201 0e01 0401 0201  ................
-000022c0: 0601 06fd 0405 0a03 0603 0e03 0601 06ff  ................
-000022d0: 0603 0e01 0601 12ff 0803 1002 0a01 0a01  ................
-000022e0: 0601 0201 0601 06fd 0605 0601 0201 0601  ................
-000022f0: 06fd 0605 0601 0201 0601 06fd 0610 0601  ................
-00002300: 0201 02fe 0403 04fd 0a05 1c01 0601 0aff  ................
-00002310: 0a03 0603 0601 0201 0201 0202 0601 06fe  ................
-00002320: 04fc 060b 0201 10ff 0603 0601 0201 0201  ................
-00002330: 0201 0601 0601 02fa 0808 0a08 0a01 1802  ................
-00002340: 0a01 0401 08ff 0401 04ff 0a03 0a03 0e01  ................
-00002350: 0601 0601 0601 0601 0201 0601 0601 02f9  ................
-00002360: 0809 0e01 0601 0601 0601 0601 0201 0601  ................
-00002370: 0601 02f9 080c 0801 0801 0801 08fc 0806  ................
-00002380: 0801 0e01 0e01 1602 0c08 7a13 506c 6f74  ..........z.Plot
-00002390: 4361 6e76 6173 2e5f 5f69 6e69 745f 5f63  Canvas.__init__c
-000023a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000023b0: 0300 0000 4b00 0000 734c 0000 0064 017c  ....K...sL...d.|
-000023c0: 0176 0172 0c64 026e 067c 0164 0119 007c  .v.r.d.n.|.d...|
-000023d0: 0164 013c 0064 037c 0176 0172 2464 046e  .d.<.d.|.v.r$d.n
-000023e0: 067c 0164 0319 007c 0164 033c 0064 057c  .|.d...|.d.<.d.|
-000023f0: 0176 0172 3c64 066e 067c 0164 0519 007c  .v.r<d.n.|.d...|
-00002400: 0164 053c 007c 0153 0029 074e 727a 0000  .d.<.|.S.).Nrz..
-00002410: 0072 8900 0000 7219 0000 0072 0100 0000  .r....r....r....
-00002420: 726d 0000 0072 9f00 0000 7221 0000 00a9  rm...r....r!....
-00002430: 0272 1f00 0000 725f 0000 0072 2100 0000  .r....r_...r!...
-00002440: 7221 0000 0072 2200 0000 72a6 0000 0072  r!...r"...r....r
-00002450: 0100 0073 0a00 0000 0001 1802 12ff 0603  ...s............
-00002460: 1801 7a20 506c 6f74 4361 6e76 6173 2e73  ..z PlotCanvas.s
-00002470: 6574 5f64 6174 615f 706c 6f74 5f64 6566  et_data_plot_def
-00002480: 6175 6c74 6301 0000 0000 0000 0000 0000  aultc...........
-00002490: 0002 0000 0003 0000 004b 0000 0073 4c00  .........K...sL.
-000024a0: 0000 6401 7c01 7601 720c 6402 6e06 7c01  ..d.|.v.r.d.n.|.
-000024b0: 6401 1900 7c01 6401 3c00 6403 7c01 7601  d...|.d.<.d.|.v.
-000024c0: 7224 6404 6e06 7c01 6403 1900 7c01 6403  r$d.n.|.d...|.d.
-000024d0: 3c00 6405 7c01 7601 723c 6406 6e06 7c01  <.d.|.v.r<d.n.|.
-000024e0: 6405 1900 7c01 6405 3c00 7c01 5300 2907  d...|.d.<.|.S.).
-000024f0: 4e72 1b00 0000 da05 626c 6163 6b72 1a00  Nr......blackr..
-00002500: 0000 7216 0000 0072 6d00 0000 7a0c 6669  ..r....rm...z.fi
-00002510: 7474 6564 2063 7572 7665 7221 0000 0072  tted curver!...r
-00002520: c500 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
-00002530: 0000 0072 a700 0000 7a01 0000 730c 0000  ...r....z...s...
-00002540: 0000 0118 0212 ff06 0412 ff06 037a 1f50  .............z.P
-00002550: 6c6f 7443 616e 7661 732e 7365 745f 6669  lotCanvas.set_fi
-00002560: 745f 706c 6f74 5f64 6566 6175 6c74 6303  t_plot_defaultc.
-00002570: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00002580: 0000 0043 0000 0073 1c00 0000 7c00 6a00  ...C...s....|.j.
-00002590: a001 7c01 a101 0100 7c00 6a00 a002 6401  ..|.....|.j...d.
-000025a0: a101 0100 6400 5300 a902 4e54 2903 72b9  ....d.S...NT).r.
-000025b0: 0000 0072 ad00 0000 da0b 7365 745f 7669  ...r......set_vi
-000025c0: 7369 626c 6529 0372 1f00 0000 da04 7465  sible).r......te
-000025d0: 7874 7280 0000 0072 2100 0000 7221 0000  xtr....r!...r!..
-000025e0: 0072 2200 0000 da0f 7365 745f 7265 7375  .r".....set_resu
-000025f0: 6c74 735f 626f 7884 0100 0073 0400 0000  lts_box....s....
-00002600: 0001 0c02 7a1a 506c 6f74 4361 6e76 6173  ....z.PlotCanvas
-00002610: 2e73 6574 5f72 6573 756c 7473 5f62 6f78  .set_results_box
-00002620: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002630: 0003 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-00002640: 6a00 a001 6401 a101 0100 6400 5300 2902  j...d.....d.S.).
-00002650: 4e46 2902 72b9 0000 0072 c800 0000 7226  NF).r....r....r&
-00002660: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00002670: 0000 da13 6469 7361 626c 655f 7265 7375  ....disable_resu
-00002680: 6c74 735f 626f 7889 0100 0073 0200 0000  lts_box....s....
-00002690: 0001 7a1e 506c 6f74 4361 6e76 6173 2e64  ..z.PlotCanvas.d
-000026a0: 6973 6162 6c65 5f72 6573 756c 7473 5f62  isable_results_b
-000026b0: 6f78 6301 0000 0000 0000 0000 0000 0001  oxc.............
-000026c0: 0000 0006 0000 0043 0000 0073 8000 0000  .......C...s....
-000026d0: 7c00 6a00 6400 7500 7264 7c00 6a01 7236  |.j.d.u.rd|.j.r6
-000026e0: 7402 7c00 6a03 7404 a005 7c00 6a06 6a07  t.|.j.t...|.j.j.
-000026f0: a101 7404 a008 7c00 6a06 6a07 a101 8303  ..t...|.j.j.....
-00002700: 7c00 5f00 6e24 7402 7c00 6a03 7404 a005  |._.n$t.|.j.t...
-00002710: 7c00 6a06 6a09 a101 7404 a008 7c00 6a06  |.j.j...t...|.j.
-00002720: 6a09 a101 8303 7c00 5f00 7c00 a00a a100  j.....|._.|.....
-00002730: 0100 6e18 7c00 6a00 a00b a100 0100 6400  ..n.|.j.......d.
-00002740: 7c00 5f00 7c00 a00a a100 0100 6400 5300  |._.|.......d.S.
-00002750: 7228 0000 0029 0c72 aa00 0000 7268 0000  r(...).r....rh..
-00002760: 0072 4200 0000 72ae 0000 00da 026e 70da  .rB...r......np.
-00002770: 036d 696e 729f 0000 0072 bc00 0000 da03  .minr....r......
-00002780: 6d61 7872 1800 0000 da06 7265 6472 6177  maxr......redraw
-00002790: 7229 0000 0072 2600 0000 7221 0000 0072  r)...r&...r!...r
-000027a0: 2100 0000 7222 0000 0072 6500 0000 8c01  !...r"...re.....
-000027b0: 0000 7318 0000 0000 010a 0106 0102 011c  ..s.............
-000027c0: ff08 0402 011c ff06 030a 020a 0106 017a  ...............z
-000027d0: 1f50 6c6f 7443 616e 7661 732e 746f 6767  .PlotCanvas.togg
-000027e0: 6c65 5f72 616e 6765 7365 6c65 6374 6f72  le_rangeselector
-000027f0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002800: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00002810: 7c00 5f00 6400 5300 7228 0000 0029 0172  |._.d.S.r(...).r
-00002820: a100 0000 2902 721f 0000 0072 a100 0000  ....).r....r....
-00002830: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-00002840: 0d73 6574 5f72 6573 6964 7561 6c73 9c01  .set_residuals..
-00002850: 0000 7302 0000 0000 017a 1850 6c6f 7443  ..s......z.PlotC
-00002860: 616e 7661 732e 7365 745f 7265 7369 6475  anvas.set_residu
-00002870: 616c 7363 0200 0000 0000 0000 0000 0000  alsc............
-00002880: 0200 0000 0500 0000 4300 0000 7344 0000  ........C...sD..
-00002890: 007c 006a 006a 0172 3a7c 006a 006a 0273  .|.j.j.r:|.j.j.s
-000028a0: 3a7c 006a 0373 407c 006a 047c 0164 0119  :|.j.s@|.j.|.d..
-000028b0: 0064 0264 0364 048d 035c 017c 005f 037c  .d.d.d...\.|._.|
-000028c0: 006a 05a0 06a1 0001 006e 067c 017c 005f  .j.......n.|.|._
-000028d0: 0764 0553 0029 067a 470a 2020 2020 2020  .d.S.).zG.      
-000028e0: 2020 5365 7473 2062 6f74 6820 7468 6520    Sets both the 
-000028f0: 696e 6974 6961 6c20 6775 6573 7320 6669  initial guess fi
-00002900: 746c 696e 6520 616e 6420 6265 7374 2066  tline and best f
-00002910: 6974 206c 696e 650a 2020 2020 2020 2020  it line.        
-00002920: 7210 0000 007a 032d 2d67 7a0d 696e 6974  r....z.--gz.init
-00002930: 6961 6c20 6775 6573 7329 0172 6d00 0000  ial guess).rm...
-00002940: 4e29 0872 5c00 0000 72ba 0000 00da 0c6d  N).r\...r......m
-00002950: 6f64 656c 5f72 6573 756c 7472 a300 0000  odel_resultr....
-00002960: 72bd 0000 0072 ae00 0000 72b6 0000 0072  r....r....r....r
-00002970: a000 0000 2902 721f 0000 0072 a000 0000  ....).r....r....
-00002980: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-00002990: 0b73 6574 5f66 6974 6c69 6e65 9f01 0000  .set_fitline....
-000029a0: 730e 0000 0000 0410 0106 0404 010a ff0a  s...............
-000029b0: 030c 027a 1650 6c6f 7443 616e 7661 732e  ...z.PlotCanvas.
-000029c0: 7365 745f 6669 746c 696e 6563 0100 0000  set_fitlinec....
-000029d0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-000029e0: 4300 0000 7336 0000 007c 006a 0064 0075  C...s6...|.j.d.u
-000029f0: 0072 207c 006a 01a0 0274 036a 040b 0074  .r |.j...t.j...t
-00002a00: 036a 04a1 0201 006e 127c 006a 016a 027c  .j.....n.|.j.j.|
-00002a10: 006a 00a0 05a1 008e 0001 0064 0053 0072  .j.........d.S.r
-00002a20: 2800 0000 2906 72aa 0000 0072 9f00 0000  (...).r....r....
-00002a30: da08 7365 745f 6d61 736b 72cc 0000 00da  ..set_maskr.....
-00002a40: 0369 6e66 724b 0000 0072 2600 0000 7221  .infrK...r&...r!
-00002a50: 0000 0072 2100 0000 7222 0000 0072 4b00  ...r!...r"...rK.
-00002a60: 0000 af01 0000 7306 0000 0000 010a 0116  ......s.........
-00002a70: 027a 1450 6c6f 7443 616e 7661 732e 6765  .z.PlotCanvas.ge
-00002a80: 745f 7261 6e67 6563 0200 0000 0000 0000  t_rangec........
-00002a90: 0000 0000 0400 0000 0400 0000 4f00 0000  ............O...
-00002aa0: 7320 0000 007c 006a 006a 017c 016a 027c  s ...|.j.j.|.j.|
-00002ab0: 016a 0367 027c 02a2 0152 0069 007c 03a4  .j.g.|...R.i.|..
-00002ac0: 018e 0153 0029 017a 460a 2020 2020 2020  ...S.).zF.      
-00002ad0: 2020 636f 6e76 656e 6965 6e63 6520 6675    convenience fu
-00002ae0: 6e63 7469 6f6e 2066 6f72 2070 6c6f 7474  nction for plott
-00002af0: 696e 6720 636f 6d70 6c65 7820 7175 616e  ing complex quan
-00002b00: 7469 7469 6573 0a20 2020 2020 2020 2029  tities.        )
-00002b10: 0472 ae00 0000 72b2 0000 00da 0472 6561  .r....r......rea
-00002b20: 6cda 0469 6d61 6729 0472 1f00 0000 729f  l..imag).r....r.
-00002b30: 0000 00da 0461 7267 7372 5f00 0000 7221  .....argsr_...r!
-00002b40: 0000 0072 2100 0000 7222 0000 0072 bd00  ...r!...r"...r..
-00002b50: 0000 b501 0000 7302 0000 0000 047a 1750  ......s......z.P
-00002b60: 6c6f 7443 616e 7661 732e 706c 6f74 5f63  lotCanvas.plot_c
-00002b70: 6f6d 706c 6578 6301 0000 0000 0000 0000  omplexc.........
-00002b80: 0000 0003 0000 0003 0000 004b 0000 0073  ...........K...s
-00002b90: 2000 0000 7400 6401 8301 7d02 6402 7c01   ...t.d...}.d.|.
-00002ba0: 7600 721c 7c01 6402 1900 7c02 6403 3c00  v.r.|.d...|.d.<.
-00002bb0: 7c02 5300 2904 4e72 a400 0000 726c 0000  |.S.).Nr....rl..
-00002bc0: 0072 1b00 0000 7202 0000 0029 0372 1f00  .r....r....).r..
-00002bd0: 0000 725f 0000 0072 a500 0000 7221 0000  ..r_...r....r!..
-00002be0: 0072 2100 0000 7222 0000 00da 1563 7265  .r!...r".....cre
-00002bf0: 6174 655f 6669 746c 696e 655f 6b77 6172  ate_fitline_kwar
-00002c00: 6773 bb01 0000 7308 0000 0000 0108 0108  gs....s.........
-00002c10: 010c 017a 2050 6c6f 7443 616e 7661 732e  ...z PlotCanvas.
-00002c20: 6372 6561 7465 5f66 6974 6c69 6e65 5f6b  create_fitline_k
-00002c30: 7761 7267 7363 0100 0000 0000 0000 0000  wargsc..........
-00002c40: 0000 0600 0000 0800 0000 4300 0000 73f4  ..........C...s.
-00002c50: 0100 007c 006a 006a 0172 a47c 006a 006a  ...|.j.j.r.|.j.j
-00002c60: 0272 a47c 006a 006a 016a 037c 006a 006a  .r.|.j.j.j.|.j.j
-00002c70: 016a 047c 006a 006a 056a 0664 018d 027d  .j.|.j.j.j.d...}
-00002c80: 017c 006a 0772 3e7c 006a 07a0 08a1 0001  .|.j.r>|.j......
-00002c90: 007c 006a 0972 547c 006a 09a0 08a1 0001  .|.j.rT|.j......
-00002ca0: 0064 007c 005f 097c 006a 0a6a 0ba0 0ca1  .d.|._.|.j.j....
-00002cb0: 0001 007c 006a 0d7c 0164 0266 0269 007c  ...|.j.|.d.f.i.|
-00002cc0: 006a 0ea4 018e 015c 017c 005f 077c 006a  .j.....\.|._.|.j
-00002cd0: 006a 016a 0f7c 006a 0a64 0364 0464 0564  .j.j.|.j.d.d.d.d
-00002ce0: 0669 0164 078d 047c 005f 107c 006a 11a0  .i.d...|._.|.j..
-00002cf0: 12a1 0001 006e f87c 006a 1364 0075 0190  .....n.|.j.d.u..
-00002d00: 0172 767c 006a 1464 0075 0072 cc7c 006a  .rv|.j.d.u.r.|.j
-00002d10: 0a6a 1564 0864 0964 0a64 0b8d 0301 0074  .j.d.d.d.d.....t
-00002d20: 1664 0c19 0072 e474 17a0 187c 006a 056a  .d...r.t...|.j.j
-00002d30: 06a1 017d 026e 1474 17a0 1964 0874 1a7c  ...}.n.t...d.t.|
-00002d40: 006a 056a 0683 01a1 027d 0274 17a0 1b67  .j.j.....}.t...g
-00002d50: 00a1 017d 0374 1c74 1a7c 006a 056a 0683  ...}.t.t.|.j.j..
-00002d60: 0183 0144 005d 2e7d 047c 006a 056a 1d7c  ...D.].}.|.j.j.|
-00002d70: 0419 0064 0d6b 0290 0172 1274 17a0 1e7c  ...d.k...r.t...|
-00002d80: 037c 006a 056a 067c 0419 0067 01a1 027d  .|.j.j.|...g...}
-00002d90: 0390 0171 127c 006a 1fa0 207c 037c 0264  ...q.|.j.. |.|.d
-00002da0: 0074 1a7c 006a 1383 0185 0219 0019 007c  .t.|.j.........|
-00002db0: 006a 137c 0264 0074 1a7c 006a 1383 0185  .j.|.d.t.|.j....
-00002dc0: 0219 0019 00a1 0201 007c 006a 2164 0075  .........|.j!d.u
-00002dd0: 0190 0172 9c7c 006a 07a0 207c 006a 2164  ...r.|.j.. |.j!d
-00002de0: 0819 007c 006a 2164 0e19 00a1 0201 007c  ...|.j!d.......|
-00002df0: 006a 11a0 22a1 0001 007c 006a 11a0 23a1  .j.."....|.j..#.
-00002e00: 0001 007c 006a 0aa0 22a1 0001 007c 006a  ...|.j.."....|.j
-00002e10: 0aa0 23a1 0001 0074 2474 17a0 257c 006a  ..#....t$t..%|.j
-00002e20: 0aa0 26a1 00a1 0183 017d 057c 006a 0aa0  ..&......}.|.j..
-00002e30: 277c 050b 007c 05a1 0201 007c 00a0 28a1  '|...|.....|..(.
-00002e40: 0001 0064 0053 0029 0f4e 2902 da06 7061  ...d.S.).N)...pa
-00002e50: 7261 6d73 7218 0000 007a 032d 2d6b 7a03  ramsr....z.--kz.
-00002e60: 2e2d 6bda 0361 6273 726d 0000 0072 7700  .-k..absrm...rw.
-00002e70: 0000 2904 7220 0000 00da 0764 6174 6166  ..).r .....dataf
-00002e80: 6d74 da0d 7061 7273 655f 636f 6d70 6c65  mt..parse_comple
-00002e90: 78da 0864 6174 615f 6b77 7372 0100 0000  x..data_kwsr....
-00002ea0: 7216 0000 0072 c600 0000 2903 72bc 0000  r....r....).r...
-00002eb0: 0072 1a00 0000 721b 0000 00da 0e53 4f52  .r....r......SOR
-00002ec0: 545f 5245 5349 4455 414c 5354 7210 0000  T_RESIDUALSTr...
-00002ed0: 0029 2972 5c00 0000 72d1 0000 0072 ba00  .))r\...r....r..
-00002ee0: 0000 da04 6576 616c 72d9 0000 0072 9f00  ....evalr....r..
-00002ef0: 0000 7218 0000 0072 b300 0000 7229 0000  ..r....r....r)..
-00002f00: 0072 a300 0000 72ac 0000 00da 056c 696e  .r....r......lin
-00002f10: 6573 da05 636c 6561 7272 bd00 0000 72a5  es..clearr....r.
-00002f20: 0000 00da 0e70 6c6f 745f 7265 7369 6475  .....plot_residu
-00002f30: 616c 7372 a200 0000 72ae 0000 0072 b600  alsr....r....r..
-00002f40: 0000 72a1 0000 0072 b500 0000 da07 6178  ..r....r......ax
-00002f50: 686c 696e 6572 1100 0000 72cc 0000 00da  hliner....r.....
-00002f60: 0761 7267 736f 7274 da06 6172 616e 6765  .argsort..arange
-00002f70: da03 6c65 6eda 0561 7272 6179 da05 7261  ..len..array..ra
-00002f80: 6e67 65da 046d 6173 6bda 0661 7070 656e  nge..mask..appen
-00002f90: 6472 b400 0000 72bb 0000 0072 a000 0000  dr....r....r....
-00002fa0: 5a05 7265 6c69 6dda 0961 7574 6f73 6361  Z.relim..autosca
-00002fb0: 6c65 72ce 0000 0072 da00 0000 5a08 6765  ler....r....Z.ge
-00002fc0: 745f 796c 696d da08 7365 745f 796c 696d  t_ylim..set_ylim
-00002fd0: 72cf 0000 0029 0672 1f00 0000 5a07 6669  r....).r....Z.fi
-00002fe0: 745f 7332 31da 056f 7264 6572 5a09 6461  t_s21..orderZ.da
-00002ff0: 7461 5f63 6f70 79da 0169 da04 796d 6178  ta_copy..i..ymax
-00003000: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00003010: 5b00 0000 c101 0000 735a 0000 0000 0310  [.......sZ......
-00003020: 0108 0110 ff06 0606 010a 0106 010a 0106  ................
-00003030: 020c 0604 0104 ff04 0104 ff0a 0308 0104  ................
-00003040: 0102 0102 0106 fc08 060c 020c 020a 0112  ................
-00003050: 0308 0110 0214 0d0a 0114 0112 011a 0106  ................
-00003060: 0114 0116 fe04 0a0c 011a 030a 010a 010a  ................
-00003070: 010a 0314 0110 037a 1650 6c6f 7443 616e  .......z.PlotCan
-00003080: 7661 732e 7570 6461 7465 5f70 6c6f 7463  vas.update_plotc
-00003090: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000030a0: 0200 0000 4300 0000 730c 0000 007c 00a0  ....C...s....|..
-000030b0: 00a1 0001 0064 0053 0072 2800 0000 2901  .....d.S.r(...).
-000030c0: 723a 0000 0072 2600 0000 7221 0000 0072  r:...r&...r!...r
-000030d0: 2100 0000 7222 0000 0072 cf00 0000 1602  !...r"...r......
-000030e0: 0000 7302 0000 0000 027a 1150 6c6f 7443  ..s......z.PlotC
-000030f0: 616e 7661 732e 7265 6472 6177 4e29 1172  anvas.redrawN).r
-00003100: 3e00 0000 723f 0000 0072 4000 0000 7241  >...r?...r@...rA
-00003110: 0000 0072 2300 0000 72a6 0000 0072 a700  ...r#...r....r..
-00003120: 0000 72ca 0000 0072 cb00 0000 7265 0000  ..r....r....re..
-00003130: 0072 d000 0000 72d2 0000 0072 4b00 0000  .r....r....rK...
-00003140: 72bd 0000 0072 d800 0000 725b 0000 0072  r....r....r[...r
-00003150: cf00 0000 7221 0000 0072 2100 0000 7221  ....r!...r!...r!
-00003160: 0000 0072 2200 0000 7251 0000 00af 0000  ...r"...rQ......
-00003170: 0073 1e00 0000 0801 0402 087f 0041 0808  .s...........A..
-00003180: 080a 0805 0803 0810 0803 0810 0806 0806  ................
-00003190: 0806 0855 7251 0000 0063 0000 0000 0000  ...UrQ...c......
-000031a0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-000031b0: 0000 7328 0000 0065 005a 0164 005a 0264  ..s(...e.Z.d.Z.d
-000031c0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
-000031d0: 005a 0564 0664 0784 005a 0664 0853 0029  .Z.d.d...Z.d.S.)
-000031e0: 09da 0b50 6172 616d 5769 6467 6574 7a2b  ...ParamWidgetz+
-000031f0: 5174 2077 6964 6765 7420 746f 2073 686f  Qt widget to sho
-00003200: 7720 616e 6420 6368 616e 6765 2061 2066  w and change a f
-00003210: 6974 7061 7261 6d65 7465 7263 0200 0000  itparameterc....
-00003220: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00003230: 4300 0000 737a 0000 0074 006a 01a0 027c  C...sz...t.j...|
-00003240: 00a1 0101 007c 017c 005f 0374 00a0 047c  .....|.|._.t...|
-00003250: 016a 05a1 017c 005f 0674 00a0 0764 01a1  .j...|._.t...d..
-00003260: 017c 005f 087c 00a0 09a1 0001 0074 00a0  .|._.|.......t..
-00003270: 0a64 02a1 017c 005f 0b74 00a0 0ca1 007d  .d...|._.t.....}
-00003280: 027c 02a0 0d7c 006a 06a1 0101 007c 02a0  .|...|.j.....|..
-00003290: 0d7c 006a 08a1 0101 007c 02a0 0d7c 006a  .|.j.....|...|.j
-000032a0: 0ba1 0101 007c 00a0 0e7c 02a1 0101 0064  .....|...|.....d
-000032b0: 0053 0029 034e 7286 0000 00da 0366 6978  .S.).Nr......fix
-000032c0: 290f 720d 0000 0072 4e00 0000 7223 0000  ).r....rN...r#..
-000032d0: 00da 0370 6172 da06 514c 6162 656c da04  ...par..QLabel..
-000032e0: 6e61 6d65 726d 0000 005a 0951 4c69 6e65  namerm...Z.QLine
-000032f0: 4564 6974 da04 6564 6974 da0c 7570 6461  Edit..edit..upda
-00003300: 7465 5f76 616c 7565 5a09 5143 6865 636b  te_valueZ.QCheck
-00003310: 426f 78da 0563 6865 636b da0b 5148 426f  Box..check..QHBo
-00003320: 784c 6179 6f75 7472 5900 0000 724f 0000  xLayoutrY...rO..
-00003330: 0029 0372 1f00 0000 72f2 0000 0072 5800  .).r....r....rX.
-00003340: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00003350: 0072 2300 0000 1e02 0000 7316 0000 0000  .r#.......s.....
-00003360: 010c 0106 010e 010c 0108 010c 0108 010c  ................
-00003370: 010c 010c 017a 1450 6172 616d 5769 6467  .....z.ParamWidg
-00003380: 6574 2e5f 5f69 6e69 745f 5f63 0100 0000  et.__init__c....
-00003390: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000033a0: 4300 0000 7324 0000 0074 007c 006a 01a0  C...s$...t.|.j..
-000033b0: 02a1 0083 017c 006a 035f 047c 006a 05a0  .....|.j._.|.j..
-000033c0: 06a1 007c 006a 035f 0764 0153 0029 027a  ...|.j._.d.S.).z
-000033d0: 3672 6561 6420 7573 6572 696e 7075 7420  6read userinput 
-000033e0: 2876 616c 7565 2061 6e64 2066 6978 6564  (value and fixed
-000033f0: 2920 696e 2074 6865 2070 6172 616d 6574  ) in the paramet
-00003400: 6572 2064 6174 614e 2908 da05 666c 6f61  er dataN)...floa
-00003410: 7472 f500 0000 72c9 0000 0072 f200 0000  tr....r....r....
-00003420: da05 7661 6c75 6572 f700 0000 5a09 6973  ..valuer....Z.is
-00003430: 4368 6563 6b65 64da 0566 6978 6564 7226  Checked..fixedr&
-00003440: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00003450: 0000 da0a 7265 6164 5f76 616c 7565 2b02  ....read_value+.
-00003460: 0000 7306 0000 0000 0212 010e 017a 1650  ..s..........z.P
-00003470: 6172 616d 5769 6467 6574 2e72 6561 645f  aramWidget.read_
-00003480: 7661 6c75 6563 0100 0000 0000 0000 0000  valuec..........
-00003490: 0000 0200 0000 0600 0000 4300 0000 7322  ..........C...s"
-000034a0: 0000 007c 006a 006a 017d 017c 006a 02a0  ...|.j.j.}.|.j..
-000034b0: 0374 047c 0174 0564 0119 0083 02a1 0101  .t.|.t.d........
-000034c0: 0064 0053 0029 024e da12 5349 474e 4946  .d.S.).N..SIGNIF
-000034d0: 4943 414e 545f 4449 4749 5453 2906 72f2  ICANT_DIGITS).r.
-000034e0: 0000 0072 fa00 0000 72f5 0000 00da 0773  ...r....r......s
-000034f0: 6574 5465 7874 7212 0000 0072 1100 0000  etTextr....r....
-00003500: 2902 721f 0000 0072 fa00 0000 7221 0000  ).r....r....r!..
-00003510: 0072 2100 0000 7222 0000 0072 f600 0000  .r!...r"...r....
-00003520: 3102 0000 7306 0000 0000 0108 0116 017a  1...s..........z
-00003530: 1850 6172 616d 5769 6467 6574 2e75 7064  .ParamWidget.upd
-00003540: 6174 655f 7661 6c75 654e 2907 723e 0000  ate_valueN).r>..
-00003550: 0072 3f00 0000 7240 0000 0072 4100 0000  .r?...r@...rA...
-00003560: 7223 0000 0072 fc00 0000 72f6 0000 0072  r#...r....r....r
-00003570: 2100 0000 7221 0000 0072 2100 0000 7222  !...r!...r!...r"
-00003580: 0000 0072 f000 0000 1b02 0000 7308 0000  ...r........s...
-00003590: 0008 0104 0208 0d08 0672 f000 0000 6300  .........r....c.
-000035a0: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-000035b0: 0000 0040 0000 0073 2000 0000 6500 5a01  ...@...s ...e.Z.
-000035c0: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
-000035d0: 6404 6405 8400 5a05 6406 5300 2907 da0c  d.d...Z.d.S.)...
-000035e0: 5265 706f 7274 5769 6467 6574 7a54 7072  ReportWidgetzTpr
-000035f0: 696e 7473 2061 2066 6974 7265 706f 7274  ints a fitreport
-00003600: 2069 6e20 6120 6e6f 6e2d 6564 6974 6162   in a non-editab
-00003610: 6c65 2074 6578 7462 6f78 2e20 5265 706f  le textbox. Repo
-00003620: 7274 2073 686f 756c 6420 6265 2061 2028  rt should be a (
-00003630: 6e65 7374 6564 2920 6469 6374 696f 6e61  nested) dictiona
-00003640: 7279 6301 0000 0000 0000 0000 0000 0001  ryc.............
-00003650: 0000 0007 0000 0043 0000 0073 3600 0000  .......C...s6...
-00003660: 7400 6a01 a002 7c00 6401 a102 0100 7c00  t.j...|.d.....|.
-00003670: a003 7404 a005 7406 6402 1900 7406 6403  ..t...t.d...t.d.
-00003680: 1900 a102 a101 0100 7c00 a007 6404 a101  ........|...d...
-00003690: 0100 6400 5300 2905 4e72 8a00 0000 da0b  ..d.S.).Nr......
-000036a0: 5245 504f 5254 5f46 4f4e 54da 0b52 4550  REPORT_FONT..REP
-000036b0: 4f52 545f 5349 5a45 5429 0872 0d00 0000  ORT_SIZET).r....
-000036c0: da09 5154 6578 7445 6469 7472 2300 0000  ..QTextEditr#...
-000036d0: 7254 0000 0072 0c00 0000 7255 0000 0072  rT...r....rU...r
-000036e0: 1100 0000 5a0b 7365 7452 6561 644f 6e6c  ....Z.setReadOnl
-000036f0: 7972 2600 0000 7221 0000 0072 2100 0000  yr&...r!...r!...
-00003700: 7222 0000 0072 2300 0000 3a02 0000 7310  r"...r#...:...s.
-00003710: 0000 0000 0106 0102 0102 fe04 0404 0112  ................
-00003720: ff04 037a 1552 6570 6f72 7457 6964 6765  ...z.ReportWidge
-00003730: 742e 5f5f 696e 6974 5f5f 6302 0000 0000  t.__init__c.....
-00003740: 0000 0000 0000 0002 0000 0003 0000 0003  ................
-00003750: 0000 0073 2400 0000 8700 8701 6602 6401  ...s$.......f.d.
-00003760: 6402 8408 8900 8801 a000 a100 0100 8800  d...............
-00003770: 7c01 6403 8302 0100 6404 5300 2905 7a57  |.d.....d.S.).zW
-00003780: 7570 6461 7465 7320 7468 6520 7465 7874  updates the text
-00003790: 206f 6620 7468 6520 7465 7874 6564 6974   of the textedit
-000037a0: 626f 7820 7769 7468 2074 6865 2063 6f6e  box with the con
-000037b0: 7465 6e74 206f 6620 6120 286e 6573 7465  tent of a (neste
-000037c0: 6429 2064 6963 7469 6f6e 6172 7920 6669  d) dictionary fi
-000037d0: 7472 6570 6f72 7463 0200 0000 0000 0000  treportc........
-000037e0: 0000 0000 0500 0000 0500 0000 1300 0000  ................
-000037f0: 73b8 0000 007c 00a0 00a1 0044 005d a05c  s....|.....D.].\
-00003800: 027d 027d 0374 017c 0383 0174 0275 0072  .}.}.t.|...t.u.r
-00003810: 687c 0164 016b 0272 2e88 01a0 0364 02a1  h|.d.k.r.....d..
-00003820: 0101 0088 01a0 0374 047c 0283 01a1 0101  .......t.|......
-00003830: 007c 0164 016b 0272 4e88 01a0 0364 03a1  .|.d.k.rN....d..
-00003840: 0101 0088 01a0 0364 04a1 0101 0088 007c  .......d.......|
-00003850: 037c 0164 0117 0083 0201 0071 0874 017c  .|.d.......q.t.|
-00003860: 0383 0174 056a 066b 0272 8674 077c 0374  ...t.j.k.r.t.|.t
-00003870: 0864 0519 0083 027d 046e 0874 047c 0383  .d.....}.n.t.|..
-00003880: 017d 0488 01a0 0374 047c 0283 0164 0617  .}.....t.|...d..
-00003890: 007c 0417 0064 0717 00a1 0101 0071 0888  .|...d.......q..
-000038a0: 01a0 0364 07a1 0101 0064 0053 0029 084e  ...d.....d.S.).N
-000038b0: 7210 0000 007a 0b3d 3d3d 3d3d 3d3d 3d3d  r....z.=========
-000038c0: 3d20 7a0c 203d 3d3d 3d3d 3d3d 3d3d 3d20  = z. ========== 
-000038d0: 7a02 0a0a 72fd 0000 007a 0409 093a 20da  z...r....z...: .
-000038e0: 010a 2909 da05 6974 656d 73da 0474 7970  ..)...items..typ
-000038f0: 6572 b700 0000 5a0f 696e 7365 7274 506c  er....Z.insertPl
-00003900: 6169 6e54 6578 7472 a400 0000 72cc 0000  ainTextr....r...
-00003910: 00da 0766 6c6f 6174 3634 7212 0000 0072  ...float64r....r
-00003920: 1100 0000 2905 da05 6164 6963 74da 056c  ....)...adict..l
-00003930: 6576 656c 7297 0000 00da 0469 7465 6d5a  evelr......itemZ
-00003940: 0869 7465 6d5f 7374 72a9 02da 0a70 7269  .item_str....pri
-00003950: 6e74 5f64 6963 7472 1f00 0000 7221 0000  nt_dictr....r!..
-00003960: 0072 2200 0000 720b 0100 0047 0200 0073  .r"...r....G...s
-00003970: 2000 0000 0001 1001 0c01 0801 0a01 0e01   ...............
-00003980: 0801 0a01 0a01 1002 0e01 0201 08ff 0604  ................
-00003990: 0801 1c01 7a2e 5265 706f 7274 5769 6467  ....z.ReportWidg
-000039a0: 6574 2e75 7064 6174 655f 7265 706f 7274  et.update_report
-000039b0: 2e3c 6c6f 6361 6c73 3e2e 7072 696e 745f  .<locals>.print_
-000039c0: 6469 6374 7210 0000 004e 2901 72e1 0000  dictr....N).r...
-000039d0: 0029 0272 1f00 0000 da09 6669 7472 6570  .).r......fitrep
-000039e0: 6f72 7472 2100 0000 720a 0100 0072 2200  ortr!...r....r".
-000039f0: 0000 da0d 7570 6461 7465 5f72 6570 6f72  ....update_repor
-00003a00: 7444 0200 0073 0600 0000 0003 0e14 0801  tD...s..........
-00003a10: 7a1a 5265 706f 7274 5769 6467 6574 2e75  z.ReportWidget.u
-00003a20: 7064 6174 655f 7265 706f 7274 4e29 0672  pdate_reportN).r
-00003a30: 3e00 0000 723f 0000 0072 4000 0000 7241  >...r?...r@...rA
-00003a40: 0000 0072 2300 0000 720d 0100 0072 2100  ...r#...r....r!.
-00003a50: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00003a60: 0072 ff00 0000 3702 0000 7306 0000 0008  .r....7...s.....
-00003a70: 0104 0208 0a72 ff00 0000 6300 0000 0000  .....r....c.....
-00003a80: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-00003a90: 0000 0073 5000 0000 6500 5a01 6400 5a02  ...sP...e.Z.d.Z.
-00003aa0: 6401 5a03 6402 6403 8400 5a04 6404 6405  d.Z.d.d...Z.d.d.
-00003ab0: 8400 5a05 6406 6407 8400 5a06 6408 6409  ..Z.d.d...Z.d.d.
-00003ac0: 8400 5a07 640a 640b 8400 5a08 640c 640d  ..Z.d.d...Z.d.d.
-00003ad0: 8400 5a09 640e 640f 8400 5a0a 6410 6411  ..Z.d.d...Z.d.d.
-00003ae0: 8400 5a0b 6412 5300 2913 da0b 4d6f 6465  ..Z.d.S.)...Mode
-00003af0: 6c57 6964 6765 747a 2b51 7420 7769 6467  lWidgetz+Qt widg
-00003b00: 6574 2074 6f20 7368 6f77 2061 6e64 2063  et to show and c
-00003b10: 6f6e 7472 6f6c 2074 6865 2066 6974 206d  ontrol the fit m
-00003b20: 6f64 656c 6303 0000 0000 0000 0000 0000  odelc...........
-00003b30: 0003 0000 0004 0000 0043 0000 0073 2a00  .........C...s*.
-00003b40: 0000 7c01 7c00 5f00 7401 6a02 a003 7c00  ..|.|._.t.j...|.
-00003b50: 6401 a102 0100 7c00 a004 7c02 a101 0100  d.....|...|.....
-00003b60: 7c00 a005 a100 0100 6400 5300 2902 4e7a  |.......d.S.).Nz
-00003b70: 0e4d 6f64 656c 2073 6574 7469 6e67 7329  .Model settings)
-00003b80: 06da 056d 6f64 656c 720d 0000 00da 0951  ...modelr......Q
-00003b90: 4772 6f75 7042 6f78 7223 0000 00da 0769  GroupBoxr#.....i
-00003ba0: 6e69 7447 5549 da0a 7365 745f 7765 6967  nitGUI..set_weig
-00003bb0: 6874 2903 721f 0000 0072 0f01 0000 da0d  ht).r....r......
-00003bc0: 7765 6967 6874 6f70 7469 6f6e 7372 2100  weightoptionsr!.
-00003bd0: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
-00003be0: 0062 0200 0073 0800 0000 0001 0601 0e01  .b...s..........
-00003bf0: 0a01 7a14 4d6f 6465 6c57 6964 6765 742e  ..z.ModelWidget.
-00003c00: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
-00003c10: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-00003c20: 0073 9600 0000 7400 a001 a100 7d02 7400  .s....t.....}.t.
-00003c30: a002 a100 7d03 6401 6402 8400 7c00 6a03  ....}.d.d...|.j.
-00003c40: 6a04 4400 8301 7c00 5f05 7400 a006 6403  j.D...|._.t...d.
-00003c50: a101 7c00 5f07 7400 a008 a100 7c00 5f09  ..|._.t.....|._.
-00003c60: 7c00 6a09 a00a 7c01 a101 0100 7c03 a00b  |.j...|.....|...
-00003c70: 7c00 6a07 a101 0100 7c03 a00b 7c00 6a09  |.j.....|...|.j.
-00003c80: a101 0100 7c03 a00c 6404 a101 0100 7c00  ....|...d.....|.
-00003c90: 6a05 4400 5d0e 7d04 7c02 a00b 7c04 a101  j.D.].}.|...|...
-00003ca0: 0100 716e 7c02 a00d 7c03 a101 0100 7c00  ..qn|...|.....|.
-00003cb0: a00e 7c02 a101 0100 6400 5300 2905 4e63  ..|.....d.S.).Nc
-00003cc0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00003cd0: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00003ce0: 005d 0c7d 0174 007c 0183 0191 0271 0453  .].}.t.|.....q.S
-00003cf0: 0072 2100 0000 2901 72f0 0000 0029 0272  .r!...).r....).r
-00003d00: 4300 0000 72f2 0000 0072 2100 0000 7221  C...r....r!...r!
-00003d10: 0000 0072 2200 0000 7245 0000 006b 0200  ...r"...rE...k..
-00003d20: 0072 4600 0000 7a27 4d6f 6465 6c57 6964  .rF...z'ModelWid
-00003d30: 6765 742e 696e 6974 4755 492e 3c6c 6f63  get.initGUI.<loc
-00003d40: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
-00003d50: 0d57 6569 6768 7465 6420 4669 743a 7210  .Weighted Fit:r.
-00003d60: 0000 0029 0f72 0d00 0000 7250 0000 0072  ...).r....rP...r
-00003d70: f800 0000 720f 0100 00da 0766 6974 7061  ....r......fitpa
-00003d80: 7273 da08 7061 7276 6965 7773 72f3 0000  rs..parviewsr...
-00003d90: 005a 0b57 6569 6768 744c 6162 656c da09  .Z.WeightLabel..
-00003da0: 5143 6f6d 626f 426f 78da 0f59 7765 6967  QComboBox..Yweig
-00003db0: 6874 636f 6d62 6f62 6f78 5a08 6164 6449  htcomboboxZ.addI
-00003dc0: 7465 6d73 7259 0000 005a 0a61 6464 5374  temsrY...Z.addSt
-00003dd0: 7265 7463 685a 0961 6464 4c61 796f 7574  retchZ.addLayout
-00003de0: 724f 0000 0029 0572 1f00 0000 7213 0100  rO...).r....r...
-00003df0: 005a 0456 426f 785a 0448 426f 78da 0770  .Z.VBoxZ.HBox..p
-00003e00: 6172 7669 6577 7221 0000 0072 2100 0000  arviewr!...r!...
-00003e10: 7222 0000 0072 1101 0000 6802 0000 731c  r"...r....h...s.
-00003e20: 0000 0000 0108 0108 0114 010c 010a 010c  ................
-00003e30: 010c 010c 010a 010a 010c 010a 010a 017a  ...............z
-00003e40: 134d 6f64 656c 5769 6467 6574 2e69 6e69  .ModelWidget.ini
-00003e50: 7447 5549 6301 0000 0000 0000 0000 0000  tGUIc...........
-00003e60: 0001 0000 0003 0000 0043 0000 0073 1000  .........C...s..
-00003e70: 0000 7c00 6a00 a001 6401 a101 0100 6400  ..|.j...d.....d.
-00003e80: 5300 72c7 0000 0029 0272 1701 0000 5a0b  S.r....).r....Z.
-00003e90: 7365 7444 6973 6162 6c65 6472 2600 0000  setDisabledr&...
-00003ea0: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
-00003eb0: 0e64 6973 6162 6c65 5f77 6569 6768 7478  .disable_weightx
-00003ec0: 0200 0073 0200 0000 0001 7a1a 4d6f 6465  ...s......z.Mode
-00003ed0: 6c57 6964 6765 742e 6469 7361 626c 655f  lWidget.disable_
-00003ee0: 7765 6967 6874 6301 0000 0000 0000 0000  weightc.........
-00003ef0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00003f00: 1000 0000 7c00 6a00 a001 6401 a101 0100  ....|.j...d.....
-00003f10: 6400 5300 72c7 0000 0029 0272 1701 0000  d.S.r....).r....
-00003f20: 5a0a 7365 7445 6e61 626c 6564 7226 0000  Z.setEnabledr&..
-00003f30: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00003f40: da0d 656e 6162 6c65 5f77 6569 6768 747b  ..enable_weight{
-00003f50: 0200 0073 0200 0000 0001 7a19 4d6f 6465  ...s......z.Mode
-00003f60: 6c57 6964 6765 742e 656e 6162 6c65 5f77  lWidget.enable_w
-00003f70: 6569 6768 7463 0100 0000 0000 0000 0000  eightc..........
-00003f80: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
-00003f90: 0000 007c 006a 00a0 01a1 0053 0072 2800  ...|.j.....S.r(.
-00003fa0: 0000 2902 7217 0100 00da 0b63 7572 7265  ..).r......curre
-00003fb0: 6e74 5465 7874 7226 0000 0072 2100 0000  ntTextr&...r!...
-00003fc0: 7221 0000 0072 2200 0000 da0a 6765 745f  r!...r".....get_
-00003fd0: 7765 6967 6874 7e02 0000 7302 0000 0000  weight~...s.....
-00003fe0: 017a 164d 6f64 656c 5769 6467 6574 2e67  .z.ModelWidget.g
-00003ff0: 6574 5f77 6569 6768 7463 0100 0000 0000  et_weightc......
-00004000: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00004010: 0000 732e 0000 007c 006a 00a0 017c 006a  ..s....|.j...|.j
-00004020: 026a 0374 046a 056a 06a1 027d 017c 0164  .j.t.j.j...}.|.d
-00004030: 016b 0572 2a7c 006a 00a0 077c 01a1 0101  .k.r*|.j...|....
-00004040: 0064 0053 0072 2400 0000 2908 7217 0100  .d.S.r$...).r...
-00004050: 005a 0866 696e 6454 6578 7472 0f01 0000  .Z.findTextr....
-00004060: da06 7765 6967 6874 720b 0000 00da 0251  ..weightr......Q
-00004070: 745a 104d 6174 6368 4669 7865 6453 7472  tZ.MatchFixedStr
-00004080: 696e 675a 0f73 6574 4375 7272 656e 7449  ingZ.setCurrentI
-00004090: 6e64 6578 2902 721f 0000 00da 0569 6e64  ndex).r......ind
-000040a0: 6578 7221 0000 0072 2100 0000 7222 0000  exr!...r!...r"..
-000040b0: 0072 1201 0000 8102 0000 730a 0000 0000  .r........s.....
-000040c0: 0106 010c ff04 0308 017a 164d 6f64 656c  .........z.Model
-000040d0: 5769 6467 6574 2e73 6574 5f77 6569 6768  Widget.set_weigh
-000040e0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-000040f0: 0000 0300 0000 4300 0000 732e 0000 007c  ......C...s....|
-00004100: 006a 0044 005d 0c7d 017c 01a0 01a1 0001  .j.D.].}.|......
-00004110: 0071 067c 00a0 02a1 007c 006a 035f 047c  .q.|.....|.j._.|
-00004120: 006a 03a0 05a1 0001 0064 0153 0029 027a  .j.......d.S.).z
-00004130: 2a72 6561 6473 2076 616c 7565 7320 6672  *reads values fr
-00004140: 6f6d 2075 7365 7269 6e70 7574 2069 6e74  om userinput int
-00004150: 6f20 7468 6520 6d6f 6465 6c4e 2906 7215  o the modelN).r.
-00004160: 0100 0072 fc00 0000 721c 0100 0072 0f01  ...r....r....r..
-00004170: 0000 721d 0100 00da 0675 7064 6174 65a9  ..r......update.
-00004180: 0272 1f00 0000 7218 0100 0072 2100 0000  .r....r....r!...
-00004190: 7221 0000 0072 2200 0000 da0b 7265 6164  r!...r".....read
-000041a0: 5f76 616c 7565 7388 0200 0073 0a00 0000  _values....s....
-000041b0: 0002 0a01 0a01 0c01 0a01 7a17 4d6f 6465  ..........z.Mode
-000041c0: 6c57 6964 6765 742e 7265 6164 5f76 616c  lWidget.read_val
-000041d0: 7565 7363 0100 0000 0000 0000 0000 0000  uesc............
-000041e0: 0200 0000 0300 0000 4300 0000 7318 0000  ........C...s...
-000041f0: 007c 006a 0044 005d 0c7d 017c 01a0 01a1  .|.j.D.].}.|....
-00004200: 0001 0071 0664 0053 0072 2800 0000 2902  ...q.d.S.r(...).
-00004210: 7215 0100 0072 f600 0000 7221 0100 0072  r....r....r!...r
-00004220: 2100 0000 7221 0000 0072 2200 0000 da0d  !...r!...r".....
-00004230: 7570 6461 7465 5f76 616c 7565 7390 0200  update_values...
-00004240: 0073 0600 0000 0001 0a01 0a01 7a19 4d6f  .s..........z.Mo
-00004250: 6465 6c57 6964 6765 742e 7570 6461 7465  delWidget.update
-00004260: 5f76 616c 7565 734e 290c 723e 0000 0072  _valuesN).r>...r
-00004270: 3f00 0000 7240 0000 0072 4100 0000 7223  ?...r@...rA...r#
-00004280: 0000 0072 1101 0000 7219 0100 0072 1a01  ...r....r....r..
-00004290: 0000 721c 0100 0072 1201 0000 7222 0100  ..r....r....r"..
-000042a0: 0072 2301 0000 7221 0000 0072 2100 0000  .r#...r!...r!...
-000042b0: 7221 0000 0072 2200 0000 720e 0100 005f  r!...r"...r...._
-000042c0: 0200 0073 1200 0000 0801 0402 0806 0810  ...s............
-000042d0: 0803 0803 0803 0807 0808 720e 0100 0029  ..........r....)
-000042e0: 2cda 0877 6172 6e69 6e67 73da 0b63 6f6c  ,..warnings..col
-000042f0: 6c65 6374 696f 6e73 7203 0000 0072 9800  lectionsr....r..
-00004300: 0000 da0e 6669 6c74 6572 7761 726e 696e  ....filterwarnin
-00004310: 6773 5a12 6d61 7470 6c6f 746c 6962 2e70  gsZ.matplotlib.p
-00004320: 6174 6368 6573 72b8 0000 00da 056e 756d  atchesr......num
-00004330: 7079 72cc 0000 00da 056c 6d66 6974 7205  pyr......lmfitr.
-00004340: 0000 00da 0a6d 6174 706c 6f74 6c69 6272  .....matplotlibr
-00004350: 0600 0000 5a22 6d61 7470 6c6f 746c 6962  ....Z"matplotlib
-00004360: 2e62 6163 6b65 6e64 732e 6261 636b 656e  .backends.backen
-00004370: 645f 7174 3561 6767 7207 0000 0072 a800  d_qt5aggr....r..
-00004380: 0000 7208 0000 0072 5200 0000 5a11 6d61  ..r....rR...Z.ma
-00004390: 7470 6c6f 746c 6962 2e66 6967 7572 6572  tplotlib.figurer
-000043a0: 0900 0000 5a0f 6d61 7470 6c6f 746c 6962  ....Z.matplotlib
-000043b0: 2e70 6174 6872 0a00 0000 da05 5079 5174  .pathr......PyQt
-000043c0: 3572 0b00 0000 720c 0000 0072 0d00 0000  5r....r....r....
-000043d0: 5a0b 5079 5174 352e 5174 4775 6972 0e00  Z.PyQt5.QtGuir..
-000043e0: 0000 5a0f 5079 5174 352e 5174 5769 6467  ..Z.PyQt5.QtWidg
-000043f0: 6574 7372 0f00 0000 da09 5f73 6574 7469  etsr......_setti
-00004400: 6e67 7372 1100 0000 da06 5f74 6f6f 6c73  ngsr......_tools
-00004410: 7212 0000 0072 1400 0000 7242 0000 0072  r....r....rB...r
-00004420: 4e00 0000 724c 0000 0072 5100 0000 72f0  N...rL...rQ...r.
-00004430: 0000 0072 0201 0000 72ff 0000 0072 1001  ...r....r....r..
-00004440: 0000 720e 0100 0072 2100 0000 7221 0000  ..r....r!...r!..
-00004450: 0072 2100 0000 7222 0000 00da 083c 6d6f  .r!...r".....<mo
-00004460: 6475 6c65 3e02 0000 0073 3400 0000 0801  dule>....s4.....
-00004470: 0c01 0802 0a03 0c01 0801 0c01 0c03 0c03  ................
-00004480: 0c03 0c01 0c01 1401 0c01 0c02 0c01 0c03  ................
-00004490: 0803 0e44 0e12 1237 107f 007f 006e 121c  ...D...7.....n..
-000044a0: 1228                                     .(
+00000020: 0004 0000 0040 0000 0073 7201 0000 6400  .....@...sr...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
+00000050: 6402 6c05 5a05 6400 6402 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6404 6c07 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6502 a00b 6406 a101 0100  m.Z...e...d.....
+00000080: 6400 6402 6c0c 6d0d 5a0d 0100 6400 6402  d.d.l.m.Z...d.d.
+00000090: 6c0e 5a0f 6400 6407 6c10 6d11 5a11 0100  l.Z.d.d.l.m.Z...
+000000a0: 6400 6408 6c12 6d13 5a13 0100 6400 6409  d.d.l.m.Z...d.d.
+000000b0: 6c14 6d15 5a16 0100 6400 640a 6c14 6d17  l.m.Z...d.d.l.m.
+000000c0: 5a18 0100 6400 640b 6c19 6d1a 5a1a 0100  Z...d.d.l.m.Z...
+000000d0: 6400 640c 6c1b 6d1c 5a1c 0100 6400 640d  d.d.l.m.Z...d.d.
+000000e0: 6c1d 6d1e 5a1e 6d1f 5a1f 6d20 5a20 0100  l.m.Z.m.Z.m Z ..
+000000f0: 6400 640e 6c21 6d22 5a22 0100 6400 640f  d.d.l!m"Z"..d.d.
+00000100: 6c23 6d24 5a24 0100 6410 6411 6c25 6d26  l#m$Z$..d.d.l%m&
+00000110: 5a26 0100 6410 6412 6c27 6d28 5a28 0100  Z&..d.d.l'm(Z(..
+00000120: 6413 6513 6414 3c00 4700 6415 6416 8400  d.e.d.<.G.d.d...
+00000130: 6416 8302 5a29 4700 6417 6418 8400 6418  d...Z)G.d.d...d.
+00000140: 8302 5a2a 4700 6419 641a 8400 641a 6520  ..Z*G.d.d...d.e 
+00000150: 6a2b 8303 5a2c 4700 641b 641c 8400 641c  j+..Z,G.d.d...d.
+00000160: 6516 8303 5a2d 4700 641d 641e 8400 641e  e...Z-G.d.d...d.
+00000170: 6520 6a2b 8303 5a2e 4700 641f 6420 8400  e j+..Z.G.d.d ..
+00000180: 6420 6520 6a2f 8303 5a30 4700 6421 6422  d e j/..Z0G.d!d"
+00000190: 8400 6422 6520 6a31 8303 5a32 6402 5300  ..d"e j1..Z2d.S.
+000001a0: 2923 e900 0000 0029 01da 0843 616c 6c61  )#.....)...Calla
+000001b0: 626c 654e a901 da0b 6465 6661 756c 7464  bleN....defaultd
+000001c0: 6963 7429 01da 0573 6f6c 7665 2901 da07  ict)...solve)...
+000001d0: 7379 6d62 6f6c 73da 0669 676e 6f72 6529  symbols..ignore)
+000001e0: 01da 054d 6f64 656c 2901 da08 7263 5061  ...Model)...rcPa
+000001f0: 7261 6d73 2901 da11 4669 6775 7265 4361  rams)...FigureCa
+00000200: 6e76 6173 5154 4167 6729 01da 144e 6176  nvasQTAgg)...Nav
+00000210: 6967 6174 696f 6e54 6f6f 6c62 6172 3251  igationToolbar2Q
+00000220: 5429 01da 0646 6967 7572 6529 01da 0450  T)...Figure)...P
+00000230: 6174 6829 03da 0651 7443 6f72 65da 0551  ath)...QtCore..Q
+00000240: 7447 7569 da09 5174 5769 6467 6574 7329  tGui..QtWidgets)
+00000250: 01da 0651 496d 6167 6529 01da 0c51 4170  ...QImage)...QAp
+00000260: 706c 6963 6174 696f 6ee9 0100 0000 2901  plication.....).
+00000270: da08 7365 7474 696e 6773 2901 da0c 666c  ..settings)...fl
+00000280: 6f61 745f 746f 5f73 7472 da02 636d 7a10  oat_to_str..cmz.
+00000290: 6d61 7468 7465 7874 2e66 6f6e 7473 6574  mathtext.fontset
+000002a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000002b0: 0003 0000 0040 0000 0073 5600 0000 6500  .....@...sV...e.
+000002c0: 5a01 6400 5a02 6401 5a03 6402 5a04 6416  Z.d.Z.d.Z.d.Z.d.
+000002d0: 6406 6407 8401 5a05 6408 6409 8400 5a06  d.d...Z.d.d...Z.
+000002e0: 640a 640b 8400 5a07 640c 640d 8400 5a08  d.d...Z.d.d...Z.
+000002f0: 640e 640f 8400 5a09 6410 6411 8400 5a0a  d.d...Z.d.d...Z.
+00000300: 6412 6413 8400 5a0b 6414 6415 8400 5a0c  d.d...Z.d.d...Z.
+00000310: 6402 5300 2917 da0e 4472 6167 6761 626c  d.S.)...Draggabl
+00000320: 6556 4c69 6e65 7a33 636c 6173 7320 746f  eVLinez3class to
+00000330: 2063 7265 6174 6520 6120 6472 6167 6761   create a dragga
+00000340: 626c 6520 7665 7274 6963 616c 206c 696e  ble vertical lin
+00000350: 6520 696e 2061 2070 6c6f 744e e904 0000  e in a plotN....
+00000360: 00fa 022d 2dda 0467 7261 7963 0600 0000  ...--..grayc....
+00000370: 0000 0000 0000 0000 0600 0000 0600 0000  ................
+00000380: 4300 0000 7326 0000 007c 016a 007c 027c  C...s&...|.j.|.|
+00000390: 037c 047c 0564 018d 047c 005f 0164 007c  .|.|.d...|._.d.|
+000003a0: 005f 027c 00a0 03a1 0001 0064 0053 0029  ._.|.......d.S.)
+000003b0: 024e 2904 da01 78da 096c 696e 6577 6964  .N)...x..linewid
+000003c0: 7468 da09 6c69 6e65 7374 796c 65da 0563  th..linestyle..c
+000003d0: 6f6c 6f72 2904 5a07 6178 766c 696e 65da  olor).Z.axvline.
+000003e0: 046c 696e 65da 0570 7265 7373 da07 636f  .line..press..co
+000003f0: 6e6e 6563 7429 06da 0473 656c 66da 0261  nnect)...self..a
+00000400: 7872 1b00 0000 721c 0000 0072 1d00 0000  xr....r....r....
+00000410: 721e 0000 00a9 0072 2400 0000 fa3b 2f55  r......r$....;/U
+00000420: 7365 7273 2f6b 6f6a 6f2f 6170 7073 2f73  sers/kojo/apps/s
+00000430: 656e 696f 725f 7072 6f6a 6563 745f 7573  enior_project_us
+00000440: 632f 6375 7276 6566 6974 6775 692f 5f77  c/curvefitgui/_w
+00000450: 6964 6765 7473 2e70 79da 085f 5f69 6e69  idgets.py..__ini
+00000460: 745f 5f2b 0000 0073 0a00 0000 0001 0401  t__+...s........
+00000470: 08ff 0803 0601 7a17 4472 6167 6761 626c  ......z.Draggabl
+00000480: 6556 4c69 6e65 2e5f 5f69 6e69 745f 5f63  eVLine.__init__c
+00000490: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000004a0: 0200 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+000004b0: 00a0 01a1 0064 0119 0053 00a9 024e 7201  .....d...S...Nr.
+000004c0: 0000 0029 0272 1f00 0000 da09 6765 745f  ...).r......get_
+000004d0: 7864 6174 61a9 0172 2200 0000 7224 0000  xdata..r"...r$..
+000004e0: 0072 2400 0000 7225 0000 00da 0767 6574  .r$...r%.....get
+000004f0: 5f70 6f73 3200 0000 7302 0000 0000 017a  _pos2...s......z
+00000500: 1644 7261 6767 6162 6c65 564c 696e 652e  .DraggableVLine.
+00000510: 6765 745f 706f 7363 0100 0000 0000 0000  get_posc........
+00000520: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000530: 730e 0000 007c 006a 00a0 01a1 0001 0064  s....|.j.......d
+00000540: 0053 00a9 014e 2902 721f 0000 00da 0672  .S...N).r......r
+00000550: 656d 6f76 6572 2900 0000 7224 0000 0072  emover)...r$...r
+00000560: 2400 0000 7225 0000 0072 2c00 0000 3500  $...r%...r,...5.
+00000570: 0000 7302 0000 0000 017a 1544 7261 6767  ..s......z.Dragg
+00000580: 6162 6c65 564c 696e 652e 7265 6d6f 7665  ableVLine.remove
+00000590: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000005a0: 0004 0000 0043 0000 0073 4600 0000 7c00  .....C...sF...|.
+000005b0: 6a00 6a01 6a02 a003 6401 7c00 6a04 a102  j.j.j...d.|.j...
+000005c0: 7c00 5f05 7c00 6a00 6a01 6a02 a003 6402  |._.|.j.j.j...d.
+000005d0: 7c00 6a06 a102 7c00 5f07 7c00 6a00 6a01  |.j...|._.|.j.j.
+000005e0: 6a02 a003 6403 7c00 6a08 a102 7c00 5f09  j...d.|.j...|._.
+000005f0: 6404 5300 2905 7a21 636f 6e6e 6563 7420  d.S.).z!connect 
+00000600: 746f 2061 6c6c 2074 6865 2065 7665 6e74  to all the event
+00000610: 7320 7765 206e 6565 645a 1262 7574 746f  s we needZ.butto
+00000620: 6e5f 7072 6573 735f 6576 656e 745a 1462  n_press_eventZ.b
+00000630: 7574 746f 6e5f 7265 6c65 6173 655f 6576  utton_release_ev
+00000640: 656e 745a 136d 6f74 696f 6e5f 6e6f 7469  entZ.motion_noti
+00000650: 6679 5f65 7665 6e74 4e29 0a72 1f00 0000  fy_eventN).r....
+00000660: da06 6669 6775 7265 da06 6361 6e76 6173  ..figure..canvas
+00000670: da0b 6d70 6c5f 636f 6e6e 6563 74da 086f  ..mpl_connect..o
+00000680: 6e5f 7072 6573 73da 0863 6964 7072 6573  n_press..cidpres
+00000690: 73da 0a6f 6e5f 7265 6c65 6173 65da 0a63  s..on_release..c
+000006a0: 6964 7265 6c65 6173 65da 096f 6e5f 6d6f  idrelease..on_mo
+000006b0: 7469 6f6e da09 6369 646d 6f74 696f 6e72  tion..cidmotionr
+000006c0: 2900 0000 7224 0000 0072 2400 0000 7225  )...r$...r$...r%
+000006d0: 0000 0072 2100 0000 3800 0000 7312 0000  ...r!...8...s...
+000006e0: 0000 020a 0106 ff06 030a 0106 ff06 030a  ................
+000006f0: 0106 ff7a 1644 7261 6767 6162 6c65 564c  ...z.DraggableVL
+00000700: 696e 652e 636f 6e6e 6563 7463 0200 0000  ine.connectc....
+00000710: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00000720: 4300 0000 735c 0000 007c 016a 007c 006a  C...s\...|.j.|.j
+00000730: 016a 026b 0372 1264 0053 0074 036a 0464  .j.k.r.d.S.t.j.d
+00000740: 0075 0172 2064 0053 007c 006a 01a0 057c  .u.r d.S.|.j...|
+00000750: 01a1 015c 027d 027d 037c 0273 3864 0053  ...\.}.}.|.s8d.S
+00000760: 007c 006a 01a0 06a1 005c 027d 047d 037c  .|.j.....\.}.}.|
+00000770: 047c 016a 0766 027c 005f 087c 0074 035f  .|.j.f.|._.|.t._
+00000780: 0464 0053 0072 2b00 0000 2909 da06 696e  .d.S.r+...)...in
+00000790: 6178 6573 721f 0000 00da 0461 7865 7372  axesr......axesr
+000007a0: 1700 0000 da04 6c6f 636b da08 636f 6e74  ......lock..cont
+000007b0: 6169 6e73 7228 0000 00da 0578 6461 7461  ainsr(.....xdata
+000007c0: 7220 0000 0029 0572 2200 0000 da05 6576  r ...).r".....ev
+000007d0: 656e 7472 3900 0000 da01 5f72 1b00 0000  entr9....._r....
+000007e0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+000007f0: 3000 0000 4400 0000 7314 0000 0000 010e  0...D...s.......
+00000800: 0104 010a 0104 0110 0104 0104 010e 010c  ................
+00000810: 017a 1744 7261 6767 6162 6c65 564c 696e  .z.DraggableVLin
+00000820: 652e 6f6e 5f70 7265 7373 6302 0000 0000  e.on_pressc.....
+00000830: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
+00000840: 0000 0073 6c00 0000 7c00 6a00 6400 7500  ...sl...|.j.d.u.
+00000850: 720e 6400 5300 7401 6a02 7c00 7501 721c  r.d.S.t.j.|.u.r.
+00000860: 6400 5300 7c01 6a03 7c00 6a04 6a05 6b03  d.S.|.j.|.j.j.k.
+00000870: 722e 6400 5300 7c00 6a00 5c02 7d02 7d03  r.d.S.|.j.\.}.}.
+00000880: 7c01 6a06 7c03 1800 7d04 7c02 7c04 1700  |.j.|...}.|.|...
+00000890: 7d05 7c00 6a04 a007 7c05 7c05 6702 a101  }.|.j...|.|.g...
+000008a0: 0100 7c00 6a04 6a08 6a09 a00a a100 0100  ..|.j.j.j.......
+000008b0: 6400 5300 722b 0000 0029 0b72 2000 0000  d.S.r+...).r ...
+000008c0: 7217 0000 0072 3800 0000 7236 0000 0072  r....r8...r6...r
+000008d0: 1f00 0000 7237 0000 0072 3a00 0000 5a09  ....r7...r:...Z.
+000008e0: 7365 745f 7864 6174 6172 2d00 0000 722e  set_xdatar-...r.
+000008f0: 0000 00da 0464 7261 7729 0672 2200 0000  .....draw).r"...
+00000900: 723b 0000 0072 1b00 0000 5a06 7870 7265  r;...r....Z.xpre
+00000910: 7373 da02 6478 5a06 785f 636c 6970 7224  ss..dxZ.x_clipr$
+00000920: 0000 0072 2400 0000 7225 0000 0072 3400  ...r$...r%...r4.
+00000930: 0000 5000 0000 7316 0000 0000 010a 0104  ..P...s.........
+00000940: 010a 0104 010e 0104 010a 010a 0108 0110  ................
+00000950: 017a 1844 7261 6767 6162 6c65 564c 696e  .z.DraggableVLin
+00000960: 652e 6f6e 5f6d 6f74 696f 6e63 0200 0000  e.on_motionc....
+00000970: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000980: 4300 0000 732c 0000 0074 006a 017c 0075  C...s,...t.j.|.u
+00000990: 0172 0e64 0053 0064 0074 005f 0164 007c  .r.d.S.d.t._.d.|
+000009a0: 005f 027c 006a 036a 046a 05a0 06a1 0001  ._.|.j.j.j......
+000009b0: 0064 0053 0072 2b00 0000 2907 7217 0000  .d.S.r+...).r...
+000009c0: 0072 3800 0000 7220 0000 0072 1f00 0000  .r8...r ...r....
+000009d0: 722d 0000 0072 2e00 0000 723d 0000 00a9  r-...r....r=....
+000009e0: 0272 2200 0000 723b 0000 0072 2400 0000  .r"...r;...r$...
+000009f0: 7224 0000 0072 2500 0000 7232 0000 005d  r$...r%...r2...]
+00000a00: 0000 0073 0a00 0000 0001 0a01 0401 0601  ...s............
+00000a10: 0601 7a19 4472 6167 6761 626c 6556 4c69  ..z.DraggableVLi
+00000a20: 6e65 2e6f 6e5f 7265 6c65 6173 6563 0100  ne.on_releasec..
+00000a30: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000a40: 0000 4300 0000 733a 0000 007c 006a 006a  ..C...s:...|.j.j
+00000a50: 016a 02a0 037c 006a 04a1 0101 007c 006a  .j...|.j.....|.j
+00000a60: 006a 016a 02a0 037c 006a 05a1 0101 007c  .j.j...|.j.....|
+00000a70: 006a 006a 016a 02a0 037c 006a 06a1 0101  .j.j.j...|.j....
+00000a80: 0064 0053 0072 2b00 0000 2907 721f 0000  .d.S.r+...).r...
+00000a90: 0072 2d00 0000 722e 0000 005a 0e6d 706c  .r-...r....Z.mpl
+00000aa0: 5f64 6973 636f 6e6e 6563 7472 3100 0000  _disconnectr1...
+00000ab0: 7233 0000 0072 3500 0000 7229 0000 0072  r3...r5...r)...r
+00000ac0: 2400 0000 7224 0000 0072 2500 0000 da0a  $...r$...r%.....
+00000ad0: 6469 7363 6f6e 6e65 6374 6400 0000 7306  disconnectd...s.
+00000ae0: 0000 0000 0112 0112 017a 1944 7261 6767  .........z.Dragg
+00000af0: 6162 6c65 564c 696e 652e 6469 7363 6f6e  ableVLine.discon
+00000b00: 6e65 6374 2903 7218 0000 0072 1900 0000  nect).r....r....
+00000b10: 721a 0000 0029 0dda 085f 5f6e 616d 655f  r....)...__name_
+00000b20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000b30: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00000b40: 6f63 5f5f 7238 0000 0072 2600 0000 722a  oc__r8...r&...r*
+00000b50: 0000 0072 2c00 0000 7221 0000 0072 3000  ...r,...r!...r0.
+00000b60: 0000 7234 0000 0072 3200 0000 7240 0000  ..r4...r2...r@..
+00000b70: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
+00000b80: 7225 0000 0072 1700 0000 2600 0000 7314  r%...r....&...s.
+00000b90: 0000 0008 0104 0204 020a 0708 0308 0308  ................
+00000ba0: 0c08 0c08 0d08 0772 1700 0000 6300 0000  .......r....c...
+00000bb0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00000bc0: 0040 0000 0073 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
+00000bd0: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
+00000be0: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
+00000bf0: 5300 2909 da0d 5261 6e67 6553 656c 6563  S.)...RangeSelec
+00000c00: 746f 727a 5763 6c61 7373 2074 6861 7420  torzWclass that 
+00000c10: 6372 6561 7465 7320 6120 7261 6e67 6573  creates a ranges
+00000c20: 656c 6563 746f 7220 696e 2061 2070 6c6f  elector in a plo
+00000c30: 7420 636f 6e73 6973 7469 6e67 206f 6620  t consisting of 
+00000c40: 7477 6f20 6472 6167 6761 626c 6520 7665  two draggable ve
+00000c50: 7274 6963 616c 206c 696e 6573 6304 0000  rtical linesc...
+00000c60: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00000c70: 0003 0000 0073 2a00 0000 7c01 8800 5f00  .....s*...|..._.
+00000c80: 7c02 7c03 6702 8800 5f01 8700 6601 6401  |.|.g..._...f.d.
+00000c90: 6402 8408 8800 6a01 4400 8301 8800 5f02  d.....j.D....._.
+00000ca0: 6400 5300 2903 4e63 0100 0000 0000 0000  d.S.).Nc........
+00000cb0: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+00000cc0: 7318 0000 0067 007c 005d 107d 0174 0088  s....g.|.].}.t..
+00000cd0: 006a 017c 0183 0291 0271 0453 0072 2400  .j.|.....q.S.r$.
+00000ce0: 0000 2902 7217 0000 0072 2300 0000 2902  ..).r....r#...).
+00000cf0: da02 2e30 da03 706f 7372 2900 0000 7224  ...0..posr)...r$
+00000d00: 0000 0072 2500 0000 da0a 3c6c 6973 7463  ...r%.....<listc
+00000d10: 6f6d 703e 7000 0000 f300 0000 007a 2a52  omp>p........z*R
+00000d20: 616e 6765 5365 6c65 6374 6f72 2e5f 5f69  angeSelector.__i
+00000d30: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e3c  nit__.<locals>.<
+00000d40: 6c69 7374 636f 6d70 3e29 0372 2300 0000  listcomp>).r#...
+00000d50: 7247 0000 00da 0a64 7261 675f 6c69 6e65  rG.....drag_line
+00000d60: 7329 0472 2200 0000 7223 0000 005a 0470  s).r"...r#...Z.p
+00000d70: 6f73 31da 0470 6f73 3272 2400 0000 7229  os1..pos2r$...r)
+00000d80: 0000 0072 2500 0000 7226 0000 006d 0000  ...r%...r&...m..
+00000d90: 0073 0600 0000 0001 0601 0a01 7a16 5261  .s..........z.Ra
+00000da0: 6e67 6553 656c 6563 746f 722e 5f5f 696e  ngeSelector.__in
+00000db0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00000dc0: 0002 0000 0002 0000 0043 0000 0073 1c00  .........C...s..
+00000dd0: 0000 6401 6402 8400 7c00 6a00 4400 8301  ..d.d...|.j.D...
+00000de0: 7d01 7c01 a001 a100 0100 7c01 5300 2903  }.|.......|.S.).
+00000df0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00000e00: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00000e10: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
+00000e20: 0453 0072 2400 0000 2901 722a 0000 0029  .S.r$...).r*...)
+00000e30: 0272 4600 0000 da08 6472 6167 6c69 6e65  .rF.....dragline
+00000e40: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
+00000e50: 4800 0000 7300 0000 7249 0000 007a 2b52  H...s...rI...z+R
+00000e60: 616e 6765 5365 6c65 6374 6f72 2e67 6574  angeSelector.get
+00000e70: 5f72 616e 6765 2e3c 6c6f 6361 6c73 3e2e  _range.<locals>.
+00000e80: 3c6c 6973 7463 6f6d 703e 2902 724a 0000  <listcomp>).rJ..
+00000e90: 00da 0473 6f72 7429 0272 2200 0000 7247  ...sort).r"...rG
+00000ea0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00000eb0: 0000 da09 6765 745f 7261 6e67 6572 0000  ....get_ranger..
+00000ec0: 0073 0600 0000 0001 1001 0801 7a17 5261  .s..........z.Ra
+00000ed0: 6e67 6553 656c 6563 746f 722e 6765 745f  ngeSelector.get_
+00000ee0: 7261 6e67 6563 0100 0000 0000 0000 0000  rangec..........
+00000ef0: 0000 0200 0000 0300 0000 4300 0000 7318  ..........C...s.
+00000f00: 0000 007c 006a 0044 005d 0c7d 017c 01a0  ...|.j.D.].}.|..
+00000f10: 01a1 0001 0071 0664 0053 0072 2b00 0000  .....q.d.S.r+...
+00000f20: 2902 724a 0000 0072 2c00 0000 2902 7222  ).rJ...r,...).r"
+00000f30: 0000 0072 4c00 0000 7224 0000 0072 2400  ...rL...r$...r$.
+00000f40: 0000 7225 0000 0072 2c00 0000 7700 0000  ..r%...r,...w...
+00000f50: 7304 0000 0000 010a 017a 1452 616e 6765  s........z.Range
+00000f60: 5365 6c65 6374 6f72 2e72 656d 6f76 654e  Selector.removeN
+00000f70: 2907 7241 0000 0072 4200 0000 7243 0000  ).rA...rB...rC..
+00000f80: 0072 4400 0000 7226 0000 0072 4e00 0000  .rD...r&...rN...
+00000f90: 722c 0000 0072 2400 0000 7224 0000 0072  r,...r$...r$...r
+00000fa0: 2400 0000 7225 0000 0072 4500 0000 6a00  $...r%...rE...j.
+00000fb0: 0000 7308 0000 0008 0104 0208 0508 0572  ..s............r
+00000fc0: 4500 0000 6300 0000 0000 0000 0000 0000  E...c...........
+00000fd0: 0000 0000 0005 0000 0000 0000 0073 7e00  .............s~.
+00000fe0: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00000ff0: a005 a100 5a06 6504 a005 6402 6402 6402  ....Z.e...d.d.d.
+00001000: a103 5a07 6403 6404 8400 5a08 8700 6601  ..Z.d.d...Z...f.
+00001010: 6405 6406 8408 5a09 6407 6408 8400 5a0a  d.d...Z.d.d...Z.
+00001020: 6409 640a 8400 5a0b 640b 640c 8400 5a0c  d.d...Z.d.d...Z.
+00001030: 640d 640e 8400 5a0d 640f 6410 8400 5a0e  d.d...Z.d.d...Z.
+00001040: 6411 6412 8400 5a0f 6413 6414 8400 5a10  d.d...Z.d.d...Z.
+00001050: 6415 6416 8400 5a11 8700 0400 5a12 5300  d.d...Z.....Z.S.
+00001060: 2917 da0a 506c 6f74 5769 6467 6574 7a54  )...PlotWidgetzT
+00001070: 5174 2077 6964 6765 7420 746f 2068 6f6c  Qt widget to hol
+00001080: 6420 7468 6520 6d61 7470 6c6f 746c 6962  d the matplotlib
+00001090: 2063 616e 7661 7320 616e 6420 7468 6520   canvas and the 
+000010a0: 746f 6f6c 7320 666f 7220 696e 7465 7261  tools for intera
+000010b0: 6374 696e 6720 7769 7468 2074 6865 2070  cting with the p
+000010c0: 6c6f 7473 5a0d 5079 5174 5f50 794f 626a  lotsZ.PyQt_PyObj
+000010d0: 6563 7463 0400 0000 0000 0000 0000 0000  ectc............
+000010e0: 0c00 0000 0800 0000 4b00 0000 73ee 0100  ........K...s...
+000010f0: 0074 006a 01a0 027c 00a1 0101 007c 00a0  .t.j...|.....|..
+00001100: 0374 00a0 04a1 00a1 0101 0074 057c 017c  .t.........t.|.|
+00001110: 027c 0366 0369 007c 04a4 018e 017c 005f  .|.f.i.|.....|._
+00001120: 0674 077c 006a 067c 0083 027c 005f 087c  .t.|.j.|...|._.|
+00001130: 006a 066a 09a0 0aa1 0064 0119 00a0 0ba1  .j.j.....d......
+00001140: 007c 005f 0c64 007c 005f 0d64 007c 005f  .|._.d.|._.d.|._
+00001150: 0e74 00a0 0f64 02a1 017c 005f 107c 006a  .t...d...|._.|.j
+00001160: 10a0 1164 02a1 0101 007c 006a 10a0 1274  ...d.....|.j...t
+00001170: 13a0 1464 0364 0474 136a 146a 15a1 03a1  ...d.d.t.j.j....
+00001180: 0101 007c 006a 106a 16a0 177c 006a 18a1  ...|.j.j...|.j..
+00001190: 0101 0074 00a0 0f64 05a1 017c 005f 197c  ...t...d...|._.|
+000011a0: 006a 19a0 1164 06a1 0101 007c 006a 19a0  .j...d.....|.j..
+000011b0: 1274 13a0 1464 0364 0474 136a 146a 15a1  .t...d.d.t.j.j..
+000011c0: 03a1 0101 007c 006a 196a 16a0 177c 006a  .....|.j.j...|.j
+000011d0: 1aa1 0101 0074 00a0 0f64 07a1 017c 005f  .....t...d...|._
+000011e0: 1b7c 006a 1ba0 1164 08a1 0101 007c 006a  .|.j...d.....|.j
+000011f0: 1ba0 1274 13a0 1464 0364 0474 136a 146a  ...t...d.d.t.j.j
+00001200: 15a1 03a1 0101 007c 006a 1b6a 16a0 177c  .......|.j.j...|
+00001210: 006a 1ca1 0101 007c 006a 08a0 1d7c 006a  .j.....|.j...|.j
+00001220: 10a1 0101 007c 006a 08a0 1ea1 0001 007c  .....|.j.......|
+00001230: 006a 08a0 1d7c 006a 19a1 0101 007c 006a  .j...|.j.....|.j
+00001240: 08a0 1ea1 0001 007c 006a 08a0 1d7c 006a  .......|.j...|.j
+00001250: 1ba1 0101 007c 006a 08a0 1ea1 0001 007c  .....|.j.......|
+00001260: 00a0 1fa1 00a0 207c 006a 08a1 0101 007c  ...... |.j.....|
+00001270: 00a0 1fa1 00a0 207c 006a 06a1 0101 007c  ...... |.j.....|
+00001280: 006a 21a0 177c 006a 22a1 0101 0064 0964  .j!..|.j"....d.d
+00001290: 0a84 007d 0564 0b64 0c84 007d 0664 0d64  ...}.d.d...}.d.d
+000012a0: 0e84 007d 0764 0f64 1084 007d 0864 1164  ...}.d.d...}.d.d
+000012b0: 1284 007d 0964 1364 1484 007d 0a64 1564  ...}.d.d...}.d.d
+000012c0: 1684 007d 0b7c 057c 067c 077c 087c 097c  ...}.|.|.|.|.|.|
+000012d0: 0a7c 0b64 179c 077c 005f 2364 0053 0029  .|.d...|._#d.S.)
+000012e0: 184e 7201 0000 007a 0f54 4f47 474c 4520  .Nr....z.TOGGLE 
+000012f0: 5245 5349 4455 414c 5a05 5469 6d65 73e9  RESIDUALZ.Times.
+00001300: 0c00 0000 fa0b 5377 6974 6368 2044 6174  ......Switch Dat
+00001310: 617a 0b53 5749 5443 4820 4441 5441 7a1c  az.SWITCH DATAz.
+00001320: 4163 7469 7661 7465 2f43 6c65 6172 2052  Activate/Clear R
+00001330: 616e 6765 5365 6c65 6374 6f72 7a0e 5241  angeSelectorz.RA
+00001340: 4e47 4520 5345 4c45 4354 4f52 6303 0000  NGE SELECTORc...
+00001350: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00001360: 0053 0000 0073 0c00 0000 7c01 7c00 1400  .S...s....|.|...
+00001370: 7c02 1700 5300 2901 7a3d 0a20 2020 2020  |...S.).z=.     
+00001380: 2020 2020 2020 206c 696e 6561 720a 2020         linear.  
+00001390: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+000013a0: 6f6e 3a20 6178 202b 2062 0a20 2020 2020  on: ax + b.     
+000013b0: 2020 2020 2020 2072 2400 0000 2903 721b         r$...).r.
+000013c0: 0000 00da 0161 da01 6272 2400 0000 7224  .....a..br$...r$
+000013d0: 0000 0072 2500 0000 da06 6c69 6e65 6172  ...r%.....linear
+000013e0: ad00 0000 7302 0000 0000 067a 2350 6c6f  ....s......z#Plo
+000013f0: 7457 6964 6765 742e 5f5f 696e 6974 5f5f  tWidget.__init__
+00001400: 2e3c 6c6f 6361 6c73 3e2e 6c69 6e65 6172  .<locals>.linear
+00001410: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00001420: 0005 0000 0053 0000 0073 1800 0000 7c01  .....S...s....|.
+00001430: 7400 a001 7c00 0b00 7c02 1b00 a101 1400  t...|...|.......
+00001440: 7c03 1700 5300 2901 7a9b 0a20 2020 2020  |...S.).z..     
+00001450: 2020 2020 2020 2065 7870 6f6e 656e 7469         exponenti
+00001460: 616c 2064 6563 6179 0a20 2020 2020 2020  al decay.       
+00001470: 2020 2020 2066 756e 6374 696f 6e3a 2061       function: a
+00001480: 202a 2065 7870 282d 7820 2f20 6229 202b   * exp(-x / b) +
+00001490: 2063 0a20 2020 2020 2020 2020 2020 2061   c.            a
+000014a0: 203a 2061 6d70 6c69 7475 6465 0a20 2020   : amplitude.   
+000014b0: 2020 2020 2020 2020 2062 203a 2072 6174           b : rat
+000014c0: 650a 2020 2020 2020 2020 2020 2020 6320  e.            c 
+000014d0: 3a20 6f66 6673 6574 0a20 2020 2020 2020  : offset.       
+000014e0: 2020 2020 20a9 02da 026e 70da 0365 7870       ....np..exp
+000014f0: 2904 721b 0000 0072 5200 0000 7253 0000  ).r....rR...rS..
+00001500: 00da 0163 7224 0000 0072 2400 0000 7225  ...cr$...r$...r%
+00001510: 0000 00da 0965 7870 5f64 6563 6179 b500  .....exp_decay..
+00001520: 0000 7302 0000 0000 087a 2650 6c6f 7457  ..s......z&PlotW
+00001530: 6964 6765 742e 5f5f 696e 6974 5f5f 2e3c  idget.__init__.<
+00001540: 6c6f 6361 6c73 3e2e 6578 705f 6465 6361  locals>.exp_deca
+00001550: 7963 0500 0000 0000 0000 0000 0000 0500  yc..............
+00001560: 0000 0500 0000 5300 0000 731a 0000 007c  ......S...s....|
+00001570: 0174 00a0 017c 027c 0014 007c 0317 00a1  .t...|.|...|....
+00001580: 0114 007c 0417 0053 0029 017a 340a 2020  ...|...S.).z4.  
+00001590: 2020 2020 2020 2020 2020 7920 3d20 6120            y = a 
+000015a0: 2a20 636f 7328 6220 2a20 7820 2b20 6329  * cos(b * x + c)
+000015b0: 202b 2064 0a20 2020 2020 2020 2020 2020   + d.           
+000015c0: 2029 0272 5600 0000 da03 636f 73a9 0572   ).rV.....cos..r
+000015d0: 1b00 0000 7252 0000 0072 5300 0000 7258  ....rR...rS...rX
+000015e0: 0000 00da 0164 7224 0000 0072 2400 0000  .....dr$...r$...
+000015f0: 7225 0000 00da 0f63 6f73 696e 655f 6675  r%.....cosine_fu
+00001600: 6e63 7469 6f6e bf00 0000 7302 0000 0000  nction....s.....
+00001610: 047a 2c50 6c6f 7457 6964 6765 742e 5f5f  .z,PlotWidget.__
+00001620: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00001630: 636f 7369 6e65 5f66 756e 6374 696f 6e63  cosine_functionc
+00001640: 0600 0000 0000 0000 0000 0000 0600 0000  ................
+00001650: 0500 0000 5300 0000 732a 0000 007c 0174  ....S...s*...|.t
+00001660: 00a0 017c 000b 007c 021b 00a1 0114 0074  ...|...|.......t
+00001670: 00a0 027c 037c 0014 007c 0417 00a1 0114  ...|.|...|......
+00001680: 007c 0517 0053 0029 017a 420a 2020 2020  .|...S.).zB.    
+00001690: 2020 2020 2020 2020 7920 3d20 6120 2a20          y = a * 
+000016a0: 6578 7028 2d78 202f 2062 2920 2a20 636f  exp(-x / b) * co
+000016b0: 7328 6320 2a20 7820 2b20 6429 202b 2065  s(c * x + d) + e
+000016c0: 0a20 2020 2020 2020 2020 2020 20a9 0372  .            ..r
+000016d0: 5600 0000 7257 0000 0072 5a00 0000 a906  V...rW...rZ.....
+000016e0: 721b 0000 0072 5200 0000 7253 0000 0072  r....rR...rS...r
+000016f0: 5800 0000 725c 0000 00da 0165 7224 0000  X...r\.....er$..
+00001700: 0072 2400 0000 7225 0000 00da 1464 6563  .r$...r%.....dec
+00001710: 6179 696e 675f 6f73 6369 6c6c 6174 696f  aying_oscillatio
+00001720: 6ec5 0000 0073 0200 0000 0004 7a31 506c  n....s......z1Pl
+00001730: 6f74 5769 6467 6574 2e5f 5f69 6e69 745f  otWidget.__init_
+00001740: 5f2e 3c6c 6f63 616c 733e 2e64 6563 6179  _.<locals>.decay
+00001750: 696e 675f 6f73 6369 6c6c 6174 696f 6e63  ing_oscillationc
+00001760: 0600 0000 0000 0000 0000 0000 0600 0000  ................
+00001770: 0500 0000 5300 0000 732e 0000 007c 0174  ....S...s....|.t
+00001780: 00a0 017c 000b 007c 021b 00a1 0164 0113  ...|...|.....d..
+00001790: 0014 0074 00a0 027c 037c 0014 007c 0417  ...t...|.|...|..
+000017a0: 00a1 0114 007c 0517 0053 0029 027a 440a  .....|...S.).zD.
+000017b0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+000017c0: 6120 2a20 6578 7028 2d78 202f 2062 295e  a * exp(-x / b)^
+000017d0: 3220 2a20 636f 7328 6320 2a20 7820 2b20  2 * cos(c * x + 
+000017e0: 6429 202b 2065 0a20 2020 2020 2020 2020  d) + e.         
+000017f0: 2020 20e9 0200 0000 725e 0000 0072 5f00     .....r^...r_.
+00001800: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00001810: 00da 1564 6563 6179 696e 675f 6f73 6369  ...decaying_osci
+00001820: 6c6c 6174 696f 6e32 cb00 0000 7302 0000  llation2....s...
+00001830: 0000 047a 3250 6c6f 7457 6964 6765 742e  ...z2PlotWidget.
+00001840: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00001850: 3e2e 6465 6361 7969 6e67 5f6f 7363 696c  >.decaying_oscil
+00001860: 6c61 7469 6f6e 3263 0200 0000 0000 0000  lation2c........
+00001870: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00001880: 7312 0000 007c 0174 00a0 0164 017c 0014  s....|.t...d.|..
+00001890: 00a1 0114 0053 0029 027a 400a 2020 2020  .....S.).z@.    
+000018a0: 2020 2020 2020 2020 4575 6c65 7227 730a          Euler's.
+000018b0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+000018c0: 6120 2a20 6578 7028 6920 2a20 7829 0a20  a * exp(i * x). 
+000018d0: 2020 2020 2020 2020 2020 20f9 0000 0000             .....
+000018e0: 0000 0000 0000 0000 0000 f03f 7255 0000  ...........?rU..
+000018f0: 0029 0272 1b00 0000 7252 0000 0072 2400  .).r....rR...r$.
+00001900: 0000 7224 0000 0072 2500 0000 da05 6575  ..r$...r%.....eu
+00001910: 6c65 72d1 0000 0073 0200 0000 0005 7a22  ler....s......z"
+00001920: 506c 6f74 5769 6467 6574 2e5f 5f69 6e69  PlotWidget.__ini
+00001930: 745f 5f2e 3c6c 6f63 616c 733e 2e65 756c  t__.<locals>.eul
+00001940: 6572 6305 0000 0000 0000 0000 0000 0005  erc.............
+00001950: 0000 0006 0000 0053 0000 0073 1e00 0000  .......S...s....
+00001960: 7c01 7400 a001 6401 7c02 7c00 1400 7c03  |.t...d.|.|...|.
+00001970: 1700 1400 a101 1400 7c04 1700 5300 2902  ........|...S.).
+00001980: 7a52 0a20 2020 2020 2020 2020 2020 2063  zR.            c
+00001990: 6f6d 706c 6578 2065 7870 0a20 2020 2020  omplex exp.     
+000019a0: 2020 2020 2020 2079 203d 2061 202a 2065         y = a * e
+000019b0: 7870 2869 202a 2028 6220 2a20 7720 2b20  xp(i * (b * w + 
+000019c0: 6329 2920 2b20 640a 2020 2020 2020 2020  c)) + d.        
+000019d0: 2020 2020 7264 0000 0072 5500 0000 725b      rd...rU...r[
+000019e0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+000019f0: 0000 da10 636f 6d70 6c65 785f 6675 6e63  ....complex_func
+00001a00: 7469 6f6e d800 0000 7302 0000 0000 057a  tion....s......z
+00001a10: 2d50 6c6f 7457 6964 6765 742e 5f5f 696e  -PlotWidget.__in
+00001a20: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 636f  it__.<locals>.co
+00001a30: 6d70 6c65 785f 6675 6e63 7469 6f6e 2907  mplex_function).
+00001a40: 7a0a 7920 3d20 6178 202b 2062 7a17 7920  z.y = ax + bz.y 
+00001a50: 3d20 6120 2a20 6578 7028 2d78 202f 2062  = a * exp(-x / b
+00001a60: 2920 2b20 637a 1879 203d 2061 202a 2063  ) + cz.y = a * c
+00001a70: 6f73 2862 2a78 202b 2063 2920 2b20 647a  os(b*x + c) + dz
+00001a80: 2879 203d 2061 202a 2065 7870 282d 7820  (y = a * exp(-x 
+00001a90: 2f20 6229 202a 2063 6f73 2863 202a 2078  / b) * cos(c * x
+00001aa0: 202b 2064 2920 2b20 657a 2a79 203d 2061   + d) + ez*y = a
+00001ab0: 202a 2065 7870 282d 7820 2f20 6229 5e32   * exp(-x / b)^2
+00001ac0: 202a 2063 6f73 2863 202a 2078 202b 2064   * cos(c * x + d
+00001ad0: 2920 2b20 657a 1279 203d 2061 202a 2065  ) + ez.y = a * e
+00001ae0: 7870 2869 202a 2078 297a 2079 203d 2061  xp(i * x)z y = a
+00001af0: 202a 2065 7870 2869 202a 2028 6220 2a20   * exp(i * (b * 
+00001b00: 7720 2b20 6329 2920 2b20 6429 2472 1000  w + c)) + d)$r..
+00001b10: 0000 da07 5157 6964 6765 7472 2600 0000  ....QWidgetr&...
+00001b20: da09 7365 744c 6179 6f75 74da 0b51 5642  ..setLayout..QVB
+00001b30: 6f78 4c61 796f 7574 da0a 506c 6f74 4361  oxLayout..PlotCa
+00001b40: 6e76 6173 722e 0000 00da 114e 6176 6967  nvasr......Navig
+00001b50: 6174 696f 6e54 6f6f 6c62 6172 da07 746f  ationToolbar..to
+00001b60: 6f6c 6261 72da 0361 7831 da09 6765 745f  olbar..ax1..get_
+00001b70: 6c69 6e65 73da 0967 6574 5f6c 6162 656c  lines..get_label
+00001b80: da0e 7365 6c65 6374 6564 5f63 7572 7665  ..selected_curve
+00001b90: da0e 7365 6c65 6374 6564 5f6d 6f64 656c  ..selected_model
+00001ba0: da0a 696e 7075 745f 6675 6e63 5a07 5141  ..input_funcZ.QA
+00001bb0: 6374 696f 6e5a 0768 6964 6552 6573 5a0b  ctionZ.hideResZ.
+00001bc0: 7365 7449 636f 6e54 6578 74da 0773 6574  setIconText..set
+00001bd0: 466f 6e74 720f 0000 00da 0551 466f 6e74  Fontr......QFont
+00001be0: 5a04 426f 6c64 5a09 7472 6967 6765 7265  Z.BoldZ.triggere
+00001bf0: 6472 2100 0000 da1a 746f 6767 6c65 5f72  dr!.....toggle_r
+00001c00: 6573 6964 7561 6c5f 7669 7369 6269 6c69  esidual_visibili
+00001c10: 7479 5a0a 7377 6974 6368 4461 7461 da0b  tyZ.switchData..
+00001c20: 7377 6974 6368 5f64 6174 615a 0e41 4373  switch_dataZ.ACs
+00001c30: 686f 7773 656c 6563 746f 72da 145f 746f  howselector.._to
+00001c40: 6767 6c65 5f73 686f 7773 656c 6563 746f  ggle_showselecto
+00001c50: 725a 0961 6464 4163 7469 6f6e 5a0c 6164  rZ.addActionZ.ad
+00001c60: 6453 6570 6172 6174 6f72 da06 6c61 796f  dSeparator..layo
+00001c70: 7574 da09 6164 6457 6964 6765 74da 0772  ut..addWidget..r
+00001c80: 6573 697a 6564 da0b 7570 6461 7465 5f70  esized..update_p
+00001c90: 6c6f 74da 0c66 756e 6374 696f 6e5f 6d61  lot..function_ma
+00001ca0: 7029 0c72 2200 0000 da06 6669 7474 6572  p).r".....fitter
+00001cb0: da06 786c 6162 656c da06 796c 6162 656c  ..xlabel..ylabel
+00001cc0: da06 6b77 6172 6773 7254 0000 0072 5900  ..kwargsrT...rY.
+00001cd0: 0000 725d 0000 0072 6100 0000 7263 0000  ..r]...ra...rc..
+00001ce0: 0072 6500 0000 7266 0000 0072 2400 0000  .re...rf...r$...
+00001cf0: 7224 0000 0072 2500 0000 7226 0000 0084  r$...r%...r&....
+00001d00: 0000 0073 5a00 0000 0001 0c01 0e01 1601  ...sZ...........
+00001d10: 0e01 1601 0601 0602 0c01 0c01 1a01 1002  ................
+00001d20: 0c01 0c01 1a01 1002 0c01 0c01 1a01 1001  ................
+00001d30: 0e02 0a02 0e02 0a02 0e02 0a01 1001 1002  ................
+00001d40: 0601 04ff 0404 0808 080a 0806 0806 0806  ................
+00001d50: 0807 0808 0201 0201 0201 0201 0201 0201  ................
+00001d60: 02f9 7a13 506c 6f74 5769 6467 6574 2e5f  ..z.PlotWidget._
+00001d70: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00001d80: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+00001d90: 731a 0000 007c 006a 00a0 01a1 0001 0074  s....|.j.......t
+00001da0: 0274 037c 0083 02a0 047c 01a1 0153 0072  .t.|.....|...S.r
+00001db0: 2b00 0000 2905 727a 0000 00da 0465 6d69  +...).rz.....emi
+00001dc0: 74da 0573 7570 6572 724f 0000 00da 0b72  t..superrO.....r
+00001dd0: 6573 697a 6545 7665 6e74 723f 0000 00a9  esizeEventr?....
+00001de0: 01da 095f 5f63 6c61 7373 5f5f 7224 0000  ...__class__r$..
+00001df0: 0072 2500 0000 7283 0000 00e9 0000 0073  .r%...r........s
+00001e00: 0400 0000 0001 0a01 7a16 506c 6f74 5769  ........z.PlotWi
+00001e10: 6467 6574 2e72 6573 697a 6545 7665 6e74  dget.resizeEvent
+00001e20: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001e30: 0002 0000 0043 0000 0073 0e00 0000 7c00  .....C...s....|.
+00001e40: 6a00 a001 a100 0100 6400 5300 722b 0000  j.......d.S.r+..
+00001e50: 0029 0272 2e00 0000 727b 0000 0072 2900  .).r....r{...r).
+00001e60: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+00001e70: 0072 7b00 0000 ed00 0000 7302 0000 0000  .r{.......s.....
+00001e80: 017a 1650 6c6f 7457 6964 6765 742e 7570  .z.PlotWidget.up
+00001e90: 6461 7465 5f70 6c6f 7463 0100 0000 0000  date_plotc......
+00001ea0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00001eb0: 0000 730e 0000 007c 006a 00a0 01a1 0001  ..s....|.j......
+00001ec0: 0064 0053 0072 2b00 0000 2902 722e 0000  .d.S.r+...).r...
+00001ed0: 00da 1474 6f67 676c 655f 7261 6e67 6573  ...toggle_ranges
+00001ee0: 656c 6563 746f 7272 2900 0000 7224 0000  electorr)...r$..
+00001ef0: 0072 2400 0000 7225 0000 0072 7700 0000  .r$...r%...rw...
+00001f00: f000 0000 7302 0000 0000 017a 1f50 6c6f  ....s......z.Plo
+00001f10: 7457 6964 6765 742e 5f74 6f67 676c 655f  tWidget._toggle_
+00001f20: 7368 6f77 7365 6c65 6374 6f72 6301 0000  showselectorc...
+00001f30: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00001f40: 0043 0000 0073 6400 0000 7c00 6a00 6a01  .C...sd...|.j.j.
+00001f50: a002 a100 731e 7c00 6a00 6a03 6a04 6400  ....s.|.j.j.j.d.
+00001f60: 6401 8d01 0100 6e20 7c00 6a00 6a03 6a05  d.....n |.j.j.j.
+00001f70: 7c00 6a00 6a06 7407 6402 1900 7407 6403  |.j.j.t.d...t.d.
+00001f80: 1900 6404 8d03 0100 7c00 6a00 6a01 a008  ..d.....|.j.j...
+00001f90: 7c00 6a00 6a01 a002 a100 0c00 a101 0100  |.j.j...........
+00001fa0: 7c00 6a00 a009 a100 0100 6400 5300 2905  |.j.......d.S.).
+00001fb0: 4e29 0172 7e00 0000 da09 5445 5854 5f46  N).r~.....TEXT_F
+00001fc0: 4f4e 54da 0954 4558 545f 5349 5a45 a902  ONT..TEXT_SIZE..
+00001fd0: da08 666f 6e74 6e61 6d65 da08 666f 6e74  ..fontname..font
+00001fe0: 7369 7a65 290a 722e 0000 00da 0361 7832  size).r......ax2
+00001ff0: 5a0b 6765 745f 7669 7369 626c 6572 6d00  Z.get_visiblerm.
+00002000: 0000 da03 7365 74da 0a73 6574 5f78 6c61  ....set..set_xla
+00002010: 6265 6c72 7e00 0000 7214 0000 00da 0b73  belr~...r......s
+00002020: 6574 5f76 6973 6962 6c65 da06 7265 6472  et_visible..redr
+00002030: 6177 7229 0000 0072 2400 0000 7224 0000  awr)...r$...r$..
+00002040: 0072 2500 0000 7275 0000 00f3 0000 0073  .r%...ru.......s
+00002050: 1200 0000 0001 0c01 1202 0801 0601 0601  ................
+00002060: 06fd 0605 1801 7a25 506c 6f74 5769 6467  ......z%PlotWidg
+00002070: 6574 2e74 6f67 676c 655f 7265 7369 6475  et.toggle_residu
+00002080: 616c 5f76 6973 6962 696c 6974 7963 0100  al_visibilityc..
+00002090: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+000020a0: 0000 4300 0000 734e 0000 0074 00a0 0167  ..C...sN...t...g
+000020b0: 0064 01a2 01a1 017d 0174 00a0 0167 0064  .d.....}.t...g.d
+000020c0: 02a2 01a1 017d 027c 006a 026a 036a 047c  .....}.|.j.j.j.|
+000020d0: 017c 0264 0364 0464 0564 068d 0501 007c  .|.d.d.d.d.....|
+000020e0: 006a 026a 03a0 05a1 0001 007c 006a 02a0  .j.j.......|.j..
+000020f0: 06a1 0001 0064 0053 0029 074e 2903 7213  .....d.S.).N).r.
+00002100: 0000 0072 6200 0000 e903 0000 0029 0372  ...rb........).r
+00002110: 1800 0000 e905 0000 00e9 0600 0000 da01  ................
+00002120: 6f72 0100 0000 da05 6461 7461 3229 03da  or......data2)..
+00002130: 066d 6172 6b65 72da 026c 77da 056c 6162  .marker..lw..lab
+00002140: 656c 2907 7256 0000 00da 0561 7272 6179  el).rV.....array
+00002150: 722e 0000 0072 6d00 0000 da04 706c 6f74  r....rm.....plot
+00002160: da06 6c65 6765 6e64 7290 0000 0029 0372  ..legendr....).r
+00002170: 2200 0000 721b 0000 00da 0179 7224 0000  "...r......yr$..
+00002180: 0072 2400 0000 7225 0000 00da 0b75 7064  .r$...r%.....upd
+00002190: 6174 655f 6461 7461 ff00 0000 7316 0000  ate_data....s...
+000021a0: 0000 010e 010e 0108 0102 0102 0102 0102  ................
+000021b0: 0102 fb06 070c 017a 1650 6c6f 7457 6964  .......z.PlotWid
+000021c0: 6765 742e 7570 6461 7465 5f64 6174 6163  get.update_datac
+000021d0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000021e0: 0500 0000 0300 0000 7372 0100 0087 0066  ........sr.....f
+000021f0: 0164 0164 0284 087d 0187 0066 0164 0364  .d.d...}...f.d.d
+00002200: 0484 087d 0274 00a0 01a1 0088 005f 0288  ...}.t......._..
+00002210: 006a 02a0 0364 05a1 0101 0074 00a0 04a1  .j...d.....t....
+00002220: 0088 005f 0574 00a0 06a1 0088 005f 0774  ..._.t......._.t
+00002230: 00a0 06a1 0088 005f 0874 00a0 09a1 0088  ......._.t......
+00002240: 005f 0a74 00a0 0b64 06a1 0188 005f 0c88  ._.t...d....._..
+00002250: 006a 0c6a 0da0 0e7c 01a1 0101 0088 006a  .j.j...|.......j
+00002260: 0c6a 0da0 0e7c 02a1 0101 0088 006a 0c6a  .j...|.......j.j
+00002270: 0da0 0e88 006a 0fa1 0101 0088 006a 0c6a  .....j.......j.j
+00002280: 0da0 0e88 006a 026a 10a1 0101 0088 006a  .....j.j.......j
+00002290: 116a 12a0 13a1 0044 005d 207d 037c 03a0  .j.....D.] }.|..
+000022a0: 14a1 0064 076b 0372 ac88 006a 07a0 157c  ...d.k.r...j...|
+000022b0: 03a0 14a1 00a1 0101 0071 ac88 006a 116a  .........q...j.j
+000022c0: 12a0 13a1 0044 005d 207d 037c 03a0 14a1  .....D.] }.|....
+000022d0: 0064 076b 0272 da88 006a 07a0 157c 03a0  .d.k.r...j...|..
+000022e0: 14a1 00a1 0101 0071 da88 006a 08a0 1588  .......q...j....
+000022f0: 006a 116a 166a 176a 186a 19a1 0101 0088  .j.j.j.j.j......
+00002300: 006a 1a44 005d 127d 0388 006a 08a0 157c  .j.D.].}...j...|
+00002310: 03a1 0101 0090 0171 1888 006a 05a0 1b88  .......q...j....
+00002320: 006a 07a1 0101 0088 006a 05a0 1b88 006a  .j.......j.....j
+00002330: 08a1 0101 0088 006a 05a0 1b88 006a 0ca1  .......j.....j..
+00002340: 0101 0088 006a 02a0 1c88 006a 05a1 0101  .....j.....j....
+00002350: 0088 006a 02a0 1da1 0001 0064 0053 0029  ...j.......d.S.)
+00002360: 084e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
+00002370: 0000 0002 0000 0013 0000 0073 1000 0000  ...........s....
+00002380: 8800 6a00 a001 a100 8800 5f02 6400 5300  ..j......._.d.S.
+00002390: 722b 0000 0029 03da 0863 6f6d 626f 626f  r+...)...combobo
+000023a0: 78da 0b63 7572 7265 6e74 5465 7874 7270  x..currentTextrp
+000023b0: 0000 0072 2400 0000 7229 0000 0072 2400  ...r$...r)...r$.
+000023c0: 0000 7225 0000 00da 1267 6574 5f73 656c  ..r%.....get_sel
+000023d0: 6563 7465 645f 6375 7276 6529 0100 0073  ected_curve)...s
+000023e0: 0200 0000 0001 7a32 506c 6f74 5769 6467  ......z2PlotWidg
+000023f0: 6574 2e73 7769 7463 685f 6461 7461 2e3c  et.switch_data.<
+00002400: 6c6f 6361 6c73 3e2e 6765 745f 7365 6c65  locals>.get_sele
+00002410: 6374 6564 5f63 7572 7665 6300 0000 0000  cted_curvec.....
+00002420: 0000 0000 0000 0000 0000 0002 0000 0013  ................
+00002430: 0000 0073 1000 0000 8800 6a00 a001 a100  ...s......j.....
+00002440: 8800 5f02 6400 5300 722b 0000 0029 03da  .._.d.S.r+...)..
+00002450: 0e6d 6f64 656c 5f63 6f6d 626f 626f 7872  .model_comboboxr
+00002460: 9f00 0000 7271 0000 0072 2400 0000 7229  ....rq...r$...r)
+00002470: 0000 0072 2400 0000 7225 0000 00da 1267  ...r$...r%.....g
+00002480: 6574 5f73 656c 6563 7465 645f 6d6f 6465  et_selected_mode
+00002490: 6c2c 0100 0073 0200 0000 0001 7a32 506c  l,...s......z2Pl
+000024a0: 6f74 5769 6467 6574 2e73 7769 7463 685f  otWidget.switch_
+000024b0: 6461 7461 2e3c 6c6f 6361 6c73 3e2e 6765  data.<locals>.ge
+000024c0: 745f 7365 6c65 6374 6564 5f6d 6f64 656c  t_selected_model
+000024d0: 7251 0000 005a 0653 656c 6563 745a 0c66  rQ...Z.SelectZ.f
+000024e0: 6974 7465 645f 6375 7276 6529 1e72 1000  itted_curve).r..
+000024f0: 0000 da07 5144 6961 6c6f 675a 0664 6961  ....QDialogZ.dia
+00002500: 6c6f 67da 0e73 6574 5769 6e64 6f77 5469  log..setWindowTi
+00002510: 746c 6572 6900 0000 7278 0000 00da 0951  tleri...rx.....Q
+00002520: 436f 6d62 6f42 6f78 729e 0000 0072 a100  ComboBoxr....r..
+00002530: 0000 da09 514c 696e 6545 6469 74da 0a75  ....QLineEdit..u
+00002540: 7365 725f 696e 7075 74da 0b51 5075 7368  ser_input..QPush
+00002550: 4275 7474 6f6e da06 6275 7474 6f6e da07  Button..button..
+00002560: 636c 6963 6b65 6472 2100 0000 da0d 7265  clickedr!.....re
+00002570: 5f69 6e69 745f 6d6f 6465 6cda 0563 6c6f  _init_model..clo
+00002580: 7365 722e 0000 0072 6d00 0000 726e 0000  ser....rm...rn..
+00002590: 0072 6f00 0000 da07 6164 6449 7465 6d72  .ro.....addItemr
+000025a0: 7d00 0000 da0a 6f72 6967 5f6d 6f64 656c  }.....orig_model
+000025b0: da04 6675 6e63 7241 0000 0072 7c00 0000  ..funcrA...r|...
+000025c0: 7279 0000 0072 6800 0000 da05 6578 6563  ry...rh.....exec
+000025d0: 5f29 0472 2200 0000 72a0 0000 0072 a200  _).r"...r....r..
+000025e0: 0000 da04 6974 656d 7224 0000 0072 2900  ....itemr$...r).
+000025f0: 0000 7225 0000 0072 7600 0000 2801 0000  ..r%...rv...(...
+00002600: 733a 0000 0000 010c 030c 040a 010c 010a  s:..............
+00002610: 020a 010a 010a 010c 010e 010e 0110 0212  ................
+00002620: 0210 010c 0112 0210 010c 0112 0206 010c  ................
+00002630: ff04 030a 0110 020e 010e 020e 020e 017a  ...............z
+00002640: 1650 6c6f 7457 6964 6765 742e 7377 6974  .PlotWidget.swit
+00002650: 6368 5f64 6174 6163 0200 0000 0000 0000  ch_datac........
+00002660: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+00002670: 7358 0000 0064 007d 027c 006a 007c 006a  sX...d.}.|.j.|.j
+00002680: 016a 026a 036a 046a 056b 0372 247c 006a  .j.j.j.j.k.r$|.j
+00002690: 067c 006a 0019 007d 0264 017c 006a 0076  .|.j...}.d.|.j.v
+000026a0: 0072 3a64 027c 006a 016a 025f 076e 0a64  .r:d.|.j.j._.n.d
+000026b0: 037c 006a 016a 025f 077c 006a 08a0 097c  .|.j.j._.|.j...|
+000026c0: 0264 0064 00a1 0301 0064 0053 0029 044e  .d.d.....d.S.).N
+000026d0: da01 6954 4629 0a72 7100 0000 722e 0000  ..iTF).rq...r...
+000026e0: 0072 7d00 0000 72ae 0000 0072 af00 0000  .r}...r....r....
+000026f0: 7241 0000 0072 7c00 0000 da0a 6973 5f63  rA...r|.....is_c
+00002700: 6f6d 706c 6578 da07 7265 5f69 6e69 7472  omplex..re_initr
+00002710: 8100 0000 2903 7222 0000 0072 3b00 0000  ....).r"...r;...
+00002720: 5a09 6e65 775f 6d6f 6465 6c72 2400 0000  Z.new_modelr$...
+00002730: 7224 0000 0072 2500 0000 72ab 0000 0054  r$...r%...r....T
+00002740: 0100 0073 0e00 0000 0001 0401 1401 0c01  ...s............
+00002750: 0a01 0c02 0a01 7a18 506c 6f74 5769 6467  ......z.PlotWidg
+00002760: 6574 2e72 655f 696e 6974 5f6d 6f64 656c  et.re_init_model
+00002770: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00002780: 0004 0000 0047 0000 0073 2800 0000 7400  .....G...s(...t.
+00002790: 7c01 8301 6401 1800 7d02 6402 7401 7c02  |...d...}.d.t.|.
+000027a0: 8301 1700 7d03 7402 7c00 6a03 7404 7c03  ....}.t.|.j.t.|.
+000027b0: 8301 8302 5300 2903 4e72 1300 0000 7a02  ....S.).Nr....z.
+000027c0: 783a 2905 da03 6c65 6eda 0373 7472 7205  x:)...len..strr.
+000027d0: 0000 0072 7200 0000 7206 0000 0029 0472  ...rr...r....).r
+000027e0: 2200 0000 da04 6172 6773 da01 6e5a 0a73  ".....args..nZ.s
+000027f0: 796d 626f 6c5f 7374 7272 2400 0000 7224  ymbol_strr$...r$
+00002800: 0000 0072 2500 0000 da14 6375 7374 6f6d  ...r%.....custom
+00002810: 5f75 7365 725f 6675 6e63 7469 6f6e 5e01  _user_function^.
+00002820: 0000 7306 0000 0000 010c 010c 017a 1f50  ..s..........z.P
+00002830: 6c6f 7457 6964 6765 742e 6375 7374 6f6d  lotWidget.custom
+00002840: 5f75 7365 725f 6675 6e63 7469 6f6e 6301  _user_functionc.
+00002850: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00002860: 0000 0043 0000 0073 6800 0000 7400 7c00  ...C...sh...t.|.
+00002870: 6a01 a002 a100 8301 6401 6b04 7264 6402  j.......d.k.rdd.
+00002880: 6701 7d01 7c00 6a01 a002 a100 7c00 5f03  g.}.|.j.....|._.
+00002890: 7c00 6a03 4400 5d18 7d02 7c02 7404 6a05  |.j.D.].}.|.t.j.
+000028a0: 7600 722a 7c01 a006 7c02 a101 0100 712a  v.r*|...|.....q*
+000028b0: 7c00 6a07 7c01 8e00 7c00 6a08 7c00 6a03  |.j.|...|.j.|.j.
+000028c0: 3c00 7c00 6a09 a00a 7c00 6a03 a101 0100  <.|.j...|.j.....
+000028d0: 6400 5300 2903 4e72 6200 0000 721b 0000  d.S.).Nrb...r...
+000028e0: 0029 0b72 b500 0000 72a7 0000 00da 0474  .).r....r......t
+000028f0: 6578 7472 7200 0000 da06 7374 7269 6e67  extrr.....string
+00002900: da0f 6173 6369 695f 7570 7065 7263 6173  ..ascii_uppercas
+00002910: 65da 0661 7070 656e 6472 b900 0000 727c  e..appendr....r|
+00002920: 0000 0072 a100 0000 72ad 0000 0029 0372  ...r....r....).r
+00002930: 2200 0000 da08 6e65 775f 6172 6773 7258  ".....new_argsrX
+00002940: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00002950: 0000 da0f 6372 6561 7465 5f63 616c 6c61  ....create_calla
+00002960: 626c 6563 0100 0073 1400 0000 0001 1201  blec...s........
+00002970: 0601 0c01 0a01 0a01 0c01 0401 02ff 0c03  ................
+00002980: 7a1a 506c 6f74 5769 6467 6574 2e63 7265  z.PlotWidget.cre
+00002990: 6174 655f 6361 6c6c 6162 6c65 2913 7241  ate_callable).rA
+000029a0: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+000029b0: 0000 720e 0000 00da 0a70 7971 7453 6967  ..r......pyqtSig
+000029c0: 6e61 6c72 7a00 0000 72b4 0000 0072 2600  nalrz...r....r&.
+000029d0: 0000 7283 0000 0072 7b00 0000 7277 0000  ..r....r{...rw..
+000029e0: 0072 7500 0000 729d 0000 0072 7600 0000  .ru...r....rv...
+000029f0: 72ab 0000 0072 b900 0000 72bf 0000 00da  r....r....r.....
+00002a00: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7224  .__classcell__r$
+00002a10: 0000 0072 2400 0000 7284 0000 0072 2500  ...r$...r....r%.
+00002a20: 0000 724f 0000 007c 0000 0073 1e00 0000  ..rO...|...s....
+00002a30: 0801 0402 0801 0401 06ff 0404 0865 0c04  .............e..
+00002a40: 0803 0803 080c 0829 082c 080a 0805 724f  .......).,....rO
+00002a50: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002a60: 0000 0000 0200 0000 4000 0000 7380 0000  ........@...s...
+00002a70: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+00002a80: 0384 005a 0464 0464 0584 005a 0564 0664  ...Z.d.d...Z.d.d
+00002a90: 0784 005a 0664 0864 0984 005a 0764 0a64  ...Z.d.d...Z.d.d
+00002aa0: 0b84 005a 0864 0c64 0d84 005a 0964 0e64  ...Z.d.d...Z.d.d
+00002ab0: 0f84 005a 0a64 1064 1184 005a 0b64 1264  ...Z.d.d...Z.d.d
+00002ac0: 1384 005a 0c64 1464 1584 005a 0d64 1664  ...Z.d.d...Z.d.d
+00002ad0: 1784 005a 0e64 1864 1984 005a 0f64 1a64  ...Z.d.d...Z.d.d
+00002ae0: 1b84 005a 1064 1c64 1d84 005a 1164 1e53  ...Z.d.d...Z.d.S
+00002af0: 0029 1f72 6a00 0000 7a60 636c 6173 7320  .).rj...z`class 
+00002b00: 746f 2068 6f6c 6420 6120 6361 6e76 6173  to hold a canvas
+00002b10: 2077 6974 6820 6120 6d61 7470 6c6f 746c   with a matplotl
+00002b20: 6962 2066 6967 7572 6520 616e 6420 7477  ib figure and tw
+00002b30: 6f20 7375 6270 6c6f 7473 2066 6f72 2070  o subplots for p
+00002b40: 6c6f 7474 696e 6720 6461 7461 2061 6e64  lotting data and
+00002b50: 2072 6573 6964 7561 6c73 6304 0000 0000   residualsc.....
+00002b60: 0000 0000 0000 000a 0000 0009 0000 000b  ................
+00002b70: 0000 0073 9404 0000 7c01 8800 5f00 7c02  ...s....|..._.|.
+00002b80: 8800 5f01 7c01 6a02 8800 5f02 6400 8800  .._.|.j..._.d...
+00002b90: 5f03 6400 8800 5f04 6400 8800 5f05 6400  _.d..._.d..._.d.
+00002ba0: 8800 5f06 7c04 8800 5f07 6400 8800 5f08  .._.|..._.d..._.
+00002bb0: 7409 740a 8301 8800 5f0b 6401 8800 6a07  t.t....._.d...j.
+00002bc0: 7601 7250 6402 6e08 8800 6a07 6401 1900  v.rPd.n...j.d...
+00002bd0: 8800 5f0c 6403 8800 6a07 7600 7270 8800  .._.d...j.v.rp..
+00002be0: 6a07 6403 1900 6e02 6404 8800 5f0d 6403  j.d...n.d..._.d.
+00002bf0: 8800 6a07 7600 7288 8800 6a07 6403 3d00  ..j.v.r...j.d.=.
+00002c00: 6405 8800 6a07 7600 729a 8800 6a07 6405  d...j.v.r...j.d.
+00002c10: 3d00 6401 8800 6a07 7600 72ac 8800 6a07  =.d...j.v.r...j.
+00002c20: 6401 3d00 6406 8800 6a07 7600 72ca 8800  d.=.d...j.v.r...
+00002c30: 6a07 6406 1900 8800 5f08 8800 6a07 6406  j.d....._...j.d.
+00002c40: 3d00 6407 8800 6a07 7600 72e8 7c04 6407  =.d...j.v.r.|.d.
+00002c50: 1900 8800 6a0b 6408 3c00 7c04 6407 3d00  ....j.d.<.|.d.=.
+00002c60: 6409 8800 6a07 7600 9001 7208 7c04 6409  d...j.v...r.|.d.
+00002c70: 1900 8800 6a0b 640a 3c00 7c04 6409 3d00  ....j.d.<.|.d.=.
+00002c80: 640b 8800 6a07 7600 9001 7228 7c04 640b  d...j.v...r(|.d.
+00002c90: 1900 8800 6a0b 640c 3c00 7c04 640b 3d00  ....j.d.<.|.d.=.
+00002ca0: 640d 8800 6a07 7600 9001 7248 7c04 640d  d...j.v...rH|.d.
+00002cb0: 1900 8800 6a0b 640e 3c00 7c04 640d 3d00  ....j.d.<.|.d.=.
+00002cc0: 8800 6a0e 6600 6900 8800 6a07 a401 8e01  ..j.f.i...j.....
+00002cd0: 8800 5f07 8800 6a0f 6600 6900 8800 6a0b  .._...j.f.i...j.
+00002ce0: a401 8e01 8800 5f0b 7410 7411 640f 1900  ......_.t.t.d...
+00002cf0: 6410 6411 8d02 8800 5f12 7413 a014 8800  d.d....._.t.....
+00002d00: 8800 6a12 a102 0100 7413 a015 8800 7416  ..j.....t.....t.
+00002d10: 6a17 6a18 7416 6a17 6a18 a103 0100 7413  j.j.t.j.j.....t.
+00002d20: a019 8800 a101 0100 6400 8800 5f1a 8800  ........d..._...
+00002d30: 6a12 a01b 6412 6413 a102 7d05 8800 6a12  j...d.d...}...j.
+00002d40: a01c 7c05 6414 1900 a101 8800 5f1d 8800  ..|.d......._...
+00002d50: 6a1d 6a1e a01f 6415 a101 0100 8800 6a12  j.j...d.......j.
+00002d60: 6a1c 7c05 6416 6417 8502 6416 6602 1900  j.|.d.d...d.f...
+00002d70: 8800 6a1d 6418 8d02 8800 5f20 8800 6a20  ..j.d....._ ..j 
+00002d80: 6a1e a01f 8800 6a0d a101 0100 8800 6a20  j.....j.......j 
+00002d90: a021 a100 0100 8800 6a1d a021 a100 0100  .!......j..!....
+00002da0: 8800 6a20 6a22 7c03 7411 6419 1900 7411  ..j j"|.t.d...t.
+00002db0: 641a 1900 641b 8d03 0100 8800 6a1d 6a22  d...d.......j.j"
+00002dc0: 641c 7411 6419 1900 7411 641a 1900 641b  d.t.d...t.d...d.
+00002dd0: 8d03 0100 8800 6a1d 6a23 7c02 7411 6419  ......j.j#|.t.d.
+00002de0: 1900 7411 641a 1900 641b 8d03 0100 8800  ..t.d...d.......
+00002df0: 6a20 6a24 6700 6700 6602 6900 8800 6a07  j j$g.g.f.i...j.
+00002e00: a401 8e01 5c01 8800 5f25 8800 6a20 6a24  ....\..._%..j j$
+00002e10: 6700 6700 6602 6900 8800 6a0b a401 8e01  g.g.f.i...j.....
+00002e20: 5c01 8800 5f26 8800 6a1d 6a24 6700 6700  \..._&..j.j$g.g.
+00002e30: 641d 641e 6413 641f 8d05 5c01 8800 5f27  d.d.d.d...\..._'
+00002e40: 6400 8800 5f28 8800 a029 a100 0100 8800  d..._(...)......
+00002e50: 6a20 6a2a 6420 6410 6421 7411 6419 1900  j j*d d.d!t.d...
+00002e60: 7411 641a 1900 6422 9c02 6423 8d04 0100  t.d...d"..d#....
+00002e70: 742b 742c 6a2d 6424 6421 6425 8d02 6426  t+t,j-d$d!d%..d&
+00002e80: 6421 6427 8d03 7d06 8800 6a20 6a2e 6428  d!d'..}...j j.d(
+00002e90: 6429 642a 7411 6419 1900 7411 641a 1900  d)d*t.d...t.d...
+00002ea0: 7c06 642b 8d06 8800 5f2f 8800 6a2f a030  |.d+...._/..j/.0
+00002eb0: a100 0100 8800 6a00 6a31 9003 7362 8800  ......j.j1..sb..
+00002ec0: 6a25 a032 8800 6a00 6a02 6a33 8800 6a00  j%.2..j.j.j3..j.
+00002ed0: 6a02 6a34 a102 0100 6e34 8800 6a25 a035  j.j4....n4..j%.5
+00002ee0: a100 0100 8800 6a36 8800 6a00 6a02 6a34  ......j6..j.j.j4
+00002ef0: 642c 6602 6900 8800 6a07 a401 8e01 5c01  d,f.i...j.....\.
+00002f00: 8800 5f25 8800 6a20 a02a a100 0100 8800  .._%..j .*......
+00002f10: 6a02 6a37 6400 7501 9003 72d4 8800 6a20  j.j7d.u...r...j 
+00002f20: 6a38 8800 6a02 6a33 8800 6a02 6a34 8800  j8..j.j3..j.j4..
+00002f30: 6a02 6a37 642d 7411 642e 1900 7411 642f  j.j7d-t.d...t.d/
+00002f40: 1900 6417 6430 8d07 8800 5f39 8800 6a02  ..d.d0...._9..j.
+00002f50: 6a3a 6400 7501 9004 7212 8800 6a20 6a38  j:d.u...r...j j8
+00002f60: 8800 6a02 6a33 8800 6a02 6a34 8800 6a02  ..j.j3..j.j4..j.
+00002f70: 6a3a 642d 7411 6431 1900 7411 6432 1900  j:d-t.d1..t.d2..
+00002f80: 6417 6433 8d07 8800 5f3b 8800 6a20 a03c  d.d3...._;..j .<
+00002f90: a100 8800 6a20 a03d a100 8800 6a1d a03c  ....j .=....j..<
+00002fa0: a100 8800 6a1d a03d a100 6604 4400 5d3c  ....j..=..f.D.]<
+00002fb0: 7d07 7c07 4400 5d30 7d08 7c08 a03e 7411  }.|.D.]0}.|..>t.
+00002fc0: 6434 1900 a101 0100 7c08 a03f 7411 6435  d4......|..?t.d5
+00002fd0: 1900 a101 0100 7c08 a040 7411 6436 1900  ......|..@t.d6..
+00002fe0: a101 0100 9004 713e 9004 7136 8700 6601  ......q>..q6..f.
+00002ff0: 6437 6438 8408 7d09 8800 6a12 6a41 a042  d7d8..}...j.jA.B
+00003000: 6439 7c09 a102 0100 6400 5300 293a 4eda  d9|.....d.S.):N.
+00003010: 0763 6f6d 706c 6578 46da 0574 6974 6c65  .complexF..title
+00003020: da04 4461 7461 da06 6d65 7468 6f64 da03  ..Data..method..
+00003030: 6164 64da 0d66 6974 6c69 6e65 5f63 6f6c  add..fitline_col
+00003040: 6f72 721e 0000 005a 1166 6974 6c69 6e65  orr....Z.fitline
+00003050: 5f6c 696e 6573 7479 6c65 721d 0000 005a  _linestyler....Z
+00003060: 1166 6974 6c69 6e65 5f6c 696e 6577 6964  .fitline_linewid
+00003070: 7468 721c 0000 005a 0d66 6974 6c69 6e65  thr....Z.fitline
+00003080: 5f6c 6162 656c 7298 0000 00da 0746 4947  _labelr......FIG
+00003090: 5f44 5049 5429 02da 0364 7069 5a0c 7469  _DPIT)...dpiZ.ti
+000030a0: 6768 745f 6c61 796f 7574 7291 0000 0072  ght_layoutr....r
+000030b0: 1300 0000 2902 7262 0000 0072 0100 0000  ....).rb...r....
+000030c0: 7a0e 5265 7369 6475 616c 2047 7261 7068  z.Residual Graph
+000030d0: 7201 0000 0072 6200 0000 2901 da06 7368  r....rb...)...sh
+000030e0: 6172 6578 7287 0000 0072 8800 0000 7289  arexr....r....r.
+000030f0: 0000 00da 0872 6573 6964 7561 6cda 016b  .....residual..k
+00003100: da01 2e29 0372 1e00 0000 7296 0000 0072  ...).r....r....r
+00003110: 9700 0000 da04 6265 7374 e700 0000 0000  ......best......
+00003120: 00e0 3f29 02da 0666 616d 696c 79da 0473  ..?)...family..s
+00003130: 697a 6529 04da 036c 6f63 5a08 6661 6e63  ize)...locZ.fanc
+00003140: 7962 6f78 5a0a 6672 616d 6561 6c70 6861  yboxZ.framealpha
+00003150: da04 7072 6f70 da05 726f 756e 6429 01da  ..prop..round)..
+00003160: 0370 6164 7a03 302e 3929 035a 0862 6f78  .padz.0.9).Z.box
+00003170: 7374 796c 65da 0266 63da 0561 6c70 6861  style..fc..alpha
+00003180: da00 2902 72cf 0000 0072 cf00 0000 7a0d  ..).r....r....z.
+00003190: 6178 6573 2066 7261 6374 696f 6e29 05da  axes fraction)..
+000031a0: 0278 795a 0878 7963 6f6f 7264 7372 8a00  .xyZ.xycoordsr..
+000031b0: 0000 72d1 0000 00da 0462 626f 7872 9400  ..r......bboxr..
+000031c0: 0000 da04 6e6f 6e65 da0b 4241 525f 595f  ....none..BAR_Y_
+000031d0: 434f 4c4f 52da 0f42 4152 5f59 5f54 4849  COLOR..BAR_Y_THI
+000031e0: 434b 4e45 5353 2905 da04 7965 7272 da03  CKNESS)...yerr..
+000031f0: 666d 7472 1e00 0000 da0a 656c 696e 6577  fmtr......elinew
+00003200: 6964 7468 da07 6361 7073 697a 65da 0b42  idth..capsize..B
+00003210: 4152 5f58 5f43 4f4c 4f52 da0f 4241 525f  AR_X_COLOR..BAR_
+00003220: 585f 5448 4943 4b4e 4553 5329 05da 0478  X_THICKNESS)...x
+00003230: 6572 7272 df00 0000 721e 0000 0072 e000  errr....r....r..
+00003240: 0000 72e1 0000 00da 0a54 4943 4b5f 434f  ..r......TICK_CO
+00003250: 4c4f 52da 0954 4943 4b5f 464f 4e54 da09  LOR..TICK_FONT..
+00003260: 5449 434b 5f53 495a 4563 0100 0000 0000  TICK_SIZEc......
+00003270: 0000 0000 0000 0200 0000 0800 0000 1300  ................
+00003280: 0000 735a 0000 007c 006a 0064 016b 0272  ..sZ...|.j.d.k.r
+00003290: 5674 01a0 02a1 008f 347d 0188 006a 03a0  Vt......4}...j..
+000032a0: 047c 01a1 0101 0074 05a0 06a1 00a0 0774  .|.....t.......t
+000032b0: 08a0 097c 01a0 0aa1 00a1 01a1 0101 0057  ...|...........W
+000032c0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+000032d0: 4c30 0001 0001 0001 0059 0001 0064 0053  L0.......Y...d.S
+000032e0: 0029 024e 7a06 6374 726c 2b63 290b da03  .).Nz.ctrl+c)...
+000032f0: 6b65 79da 0269 6fda 0742 7974 6573 494f  key..io..BytesIO
+00003300: da03 6669 675a 0773 6176 6566 6967 7212  ..figZ.savefigr.
+00003310: 0000 00da 0963 6c69 7062 6f61 7264 5a08  .....clipboardZ.
+00003320: 7365 7449 6d61 6765 7211 0000 005a 0866  setImager....Z.f
+00003330: 726f 6d44 6174 61da 0867 6574 7661 6c75  romData..getvalu
+00003340: 6529 0272 3b00 0000 da06 6275 6666 6572  e).r;.....buffer
+00003350: 7229 0000 0072 2400 0000 7225 0000 00da  r)...r$...r%....
+00003360: 1761 6464 5f66 6967 7572 655f 746f 5f63  .add_figure_to_c
+00003370: 6c69 7062 6f61 7264 2e02 0000 730c 0000  lipboard....s...
+00003380: 0000 010a 010a 010c 0108 010c ff7a 3450  .............z4P
+00003390: 6c6f 7443 616e 7661 732e 5f5f 696e 6974  lotCanvas.__init
+000033a0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6164 645f  __.<locals>.add_
+000033b0: 6669 6775 7265 5f74 6f5f 636c 6970 626f  figure_to_clipbo
+000033c0: 6172 645a 0f6b 6579 5f70 7265 7373 5f65  ardZ.key_press_e
+000033d0: 7665 6e74 2943 727d 0000 0072 7e00 0000  vent)Cr}...r~...
+000033e0: da04 6461 7461 da07 6669 746c 696e 65da  ..data..fitline.
+000033f0: 0972 6573 6964 7561 6c73 da11 636f 6d70  .residuals..comp
+00003400: 6c65 785f 7265 7369 6475 616c 73da 1269  lex_residuals..i
+00003410: 6e69 7469 616c 5f67 7565 7373 5f6c 696e  nitial_guess_lin
+00003420: 6572 8000 0000 da0f 6164 6469 7469 6f6e  er......addition
+00003430: 616c 5f64 6174 6172 0400 0000 72b6 0000  al_datar....r...
+00003440: 00da 0e66 6974 6c69 6e65 5f6b 7761 7267  ...fitline_kwarg
+00003450: 7372 c200 0000 5a09 6178 315f 7469 746c  sr....Z.ax1_titl
+00003460: 65da 1573 6574 5f64 6174 615f 706c 6f74  e..set_data_plot
+00003470: 5f64 6566 6175 6c74 da14 7365 745f 6669  _default..set_fi
+00003480: 745f 706c 6f74 5f64 6566 6175 6c74 720c  t_plot_defaultr.
+00003490: 0000 0072 1400 0000 72eb 0000 00da 0c46  ...r....r......F
+000034a0: 6967 7572 6543 616e 7661 7372 2600 0000  igureCanvasr&...
+000034b0: 5a0d 7365 7453 697a 6550 6f6c 6963 7972  Z.setSizePolicyr
+000034c0: 1000 0000 5a0b 5153 697a 6550 6f6c 6963  ....Z.QSizePolic
+000034d0: 79da 0945 7870 616e 6469 6e67 5a0e 7570  y..ExpandingZ.up
+000034e0: 6461 7465 4765 6f6d 6574 7279 da0e 7261  dateGeometry..ra
+000034f0: 6e67 655f 7365 6c65 6374 6f72 5a0c 6164  nge_selectorZ.ad
+00003500: 645f 6772 6964 7370 6563 da0b 6164 645f  d_gridspec..add_
+00003510: 7375 6270 6c6f 7472 8c00 0000 72c3 0000  subplotr....r...
+00003520: 00da 0873 6574 5f74 6578 7472 6d00 0000  ...set_textrm...
+00003530: da04 6772 6964 da0a 7365 745f 796c 6162  ..grid..set_ylab
+00003540: 656c 728e 0000 0072 9a00 0000 5a09 6461  elr....r....Z.da
+00003550: 7461 5f6c 696e 65da 0b66 6974 7465 645f  ta_line..fitted_
+00003560: 6c69 6e65 da0d 7265 7369 6475 616c 5f6c  line..residual_l
+00003570: 696e 65da 087a 6572 6f5f 7265 73da 1470  ine..zero_res..p
+00003580: 6c6f 745f 6164 6469 7469 6f6e 616c 5f64  lot_additional_d
+00003590: 6174 6172 9b00 0000 da04 6469 6374 da07  atar......dict..
+000035a0: 7061 7463 6865 735a 0842 6f78 5374 796c  patchesZ.BoxStyl
+000035b0: 655a 0861 6e6e 6f74 6174 65da 0a72 6573  eZ.annotate..res
+000035c0: 756c 745f 626f 785a 0964 7261 6767 6162  ult_boxZ.draggab
+000035d0: 6c65 72b3 0000 00da 0873 6574 5f64 6174  ler......set_dat
+000035e0: 6172 1b00 0000 729c 0000 0072 2c00 0000  ar....r....r,...
+000035f0: da0c 706c 6f74 5f63 6f6d 706c 6578 da02  ..plot_complex..
+00003600: 7965 da08 6572 726f 7262 6172 5a08 7965  ye..errorbarZ.ye
+00003610: 7272 6f62 6172 da02 7865 5a08 7865 7272  rrobar..xeZ.xerr
+00003620: 6f62 6172 da0f 6765 745f 7874 6963 6b6c  obar..get_xtickl
+00003630: 6162 656c 735a 0f67 6574 5f79 7469 636b  abelsZ.get_ytick
+00003640: 6c61 6265 6c73 5a09 7365 745f 636f 6c6f  labelsZ.set_colo
+00003650: 725a 1273 6574 5f66 6f6e 7470 726f 7065  rZ.set_fontprope
+00003660: 7274 6965 735a 0c73 6574 5f66 6f6e 7473  rtiesZ.set_fonts
+00003670: 697a 6572 2e00 0000 722f 0000 0029 0a72  izer....r/...).r
+00003680: 2200 0000 727d 0000 0072 7e00 0000 727f  "...r}...r~...r.
+00003690: 0000 0072 8000 0000 da02 6773 5a09 6262  ...r......gsZ.bb
+000036a0: 6f78 5f61 7267 73da 066c 6162 656c 73da  ox_args..labels.
+000036b0: 0474 6963 6b72 ef00 0000 7224 0000 0072  .tickr....r$...r
+000036c0: 2900 0000 7225 0000 0072 2600 0000 7301  )...r%...r&...s.
+000036d0: 0000 7320 0100 0000 0106 0106 0108 0106  ..s ............
+000036e0: 0106 0106 0106 0106 0106 010a 0216 ff04  ................
+000036f0: 0716 ff04 040a 0108 010a 0108 010a 0108  ................
+00003700: 010a 010c 0108 020a 010e 0106 010c 010e  ................
+00003710: 0106 010c 010e 0106 010c 010e 0106 0314  ................
+00003720: 0114 0312 010e 0104 0102 0106 0106 fd04  ................
+00003730: 050a 0306 030e 0306 0106 ff06 030e 0106  ................
+00003740: 0112 ff08 0310 020a 010a 0106 0102 0106  ................
+00003750: 0106 fd06 0506 0102 0106 0106 fd06 0506  ................
+00003760: 0102 0106 0106 fd06 1006 0102 0102 fe04  ................
+00003770: 0304 fd0a 051c 0106 010a ff0a 0306 0108  ................
+00003780: 0206 0102 0102 0102 0206 0106 fe04 fc06  ................
+00003790: 0b02 0110 ff06 0306 0102 0102 0102 0106  ................
+000037a0: 0106 0102 fa08 080a 080a 011c 020a 0104  ................
+000037b0: 010a ff04 0104 ff0a 030a 030e 0106 0106  ................
+000037c0: 0106 0106 0102 0106 0106 0102 f908 090e  ................
+000037d0: 0106 0106 0106 0106 0102 0106 0106 0102  ................
+000037e0: f908 0c08 0108 0108 0108 fc08 0608 010e  ................
+000037f0: 010e 0116 020c 087a 1350 6c6f 7443 616e  .......z.PlotCan
+00003800: 7661 732e 5f5f 696e 6974 5f5f 6301 0000  vas.__init__c...
+00003810: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00003820: 004b 0000 0073 4c00 0000 6401 7c01 7601  .K...sL...d.|.v.
+00003830: 720c 6402 6e06 7c01 6401 1900 7c01 6401  r.d.n.|.d...|.d.
+00003840: 3c00 6403 7c01 7601 7224 6404 6e06 7c01  <.d.|.v.r$d.n.|.
+00003850: 6403 1900 7c01 6403 3c00 6405 7c01 7601  d...|.d.<.d.|.v.
+00003860: 723c 6406 6e06 7c01 6405 1900 7c01 6405  r<d.n.|.d...|.d.
+00003870: 3c00 7c01 5300 2907 4e72 9600 0000 7294  <.|.S.).Nr....r.
+00003880: 0000 0072 1c00 0000 7201 0000 0072 9800  ...r....r....r..
+00003890: 0000 72f0 0000 0072 2400 0000 a902 7222  ..r....r$.....r"
+000038a0: 0000 0072 8000 0000 7224 0000 0072 2400  ...r....r$...r$.
+000038b0: 0000 7225 0000 0072 f700 0000 3802 0000  ..r%...r....8...
+000038c0: 730a 0000 0000 0118 0212 ff06 0318 017a  s..............z
+000038d0: 2050 6c6f 7443 616e 7661 732e 7365 745f   PlotCanvas.set_
+000038e0: 6461 7461 5f70 6c6f 745f 6465 6661 756c  data_plot_defaul
+000038f0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00003900: 0000 0300 0000 4b00 0000 734c 0000 0064  ......K...sL...d
+00003910: 017c 0176 0172 0c64 026e 067c 0164 0119  .|.v.r.d.n.|.d..
+00003920: 007c 0164 013c 0064 037c 0176 0172 2464  .|.d.<.d.|.v.r$d
+00003930: 046e 067c 0164 0319 007c 0164 033c 0064  .n.|.d...|.d.<.d
+00003940: 057c 0176 0172 3c64 066e 067c 0164 0519  .|.v.r<d.n.|.d..
+00003950: 007c 0164 053c 007c 0153 0029 074e 721e  .|.d.<.|.S.).Nr.
+00003960: 0000 00da 0562 6c61 636b 721d 0000 0072  .....blackr....r
+00003970: 1900 0000 7298 0000 007a 0c66 6974 7465  ....r....z.fitte
+00003980: 6420 6375 7276 6572 2400 0000 7210 0100  d curver$...r...
+00003990: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+000039a0: 72f8 0000 0040 0200 0073 0c00 0000 0001  r....@...s......
+000039b0: 1802 12ff 0604 12ff 0603 7a1f 506c 6f74  ..........z.Plot
+000039c0: 4361 6e76 6173 2e73 6574 5f66 6974 5f70  Canvas.set_fit_p
+000039d0: 6c6f 745f 6465 6661 756c 7463 0300 0000  lot_defaultc....
+000039e0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000039f0: 4300 0000 731c 0000 007c 006a 00a0 017c  C...s....|.j...|
+00003a00: 01a1 0101 007c 006a 00a0 0264 01a1 0101  .....|.j...d....
+00003a10: 0064 0053 00a9 024e 5429 0372 0601 0000  .d.S...NT).r....
+00003a20: 72fd 0000 0072 8f00 0000 2903 7222 0000  r....r....).r"..
+00003a30: 0072 ba00 0000 72d2 0000 0072 2400 0000  .r....r....r$...
+00003a40: 7224 0000 0072 2500 0000 da0f 7365 745f  r$...r%.....set_
+00003a50: 7265 7375 6c74 735f 626f 784a 0200 0073  results_boxJ...s
+00003a60: 0400 0000 0001 0c02 7a1a 506c 6f74 4361  ........z.PlotCa
+00003a70: 6e76 6173 2e73 6574 5f72 6573 756c 7473  nvas.set_results
+00003a80: 5f62 6f78 6301 0000 0000 0000 0000 0000  _boxc...........
+00003a90: 0001 0000 0003 0000 0043 0000 0073 1000  .........C...s..
+00003aa0: 0000 7c00 6a00 a001 6401 a101 0100 6400  ..|.j...d.....d.
+00003ab0: 5300 2902 4e46 2902 7206 0100 0072 8f00  S.).NF).r....r..
+00003ac0: 0000 7229 0000 0072 2400 0000 7224 0000  ..r)...r$...r$..
+00003ad0: 0072 2500 0000 da13 6469 7361 626c 655f  .r%.....disable_
+00003ae0: 7265 7375 6c74 735f 626f 784f 0200 0073  results_boxO...s
+00003af0: 0200 0000 0001 7a1e 506c 6f74 4361 6e76  ......z.PlotCanv
+00003b00: 6173 2e64 6973 6162 6c65 5f72 6573 756c  as.disable_resul
+00003b10: 7473 5f62 6f78 6301 0000 0000 0000 0000  ts_boxc.........
+00003b20: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
+00003b30: 8800 0000 7c00 6a00 6400 7500 726c 7c00  ....|.j.d.u.rl|.
+00003b40: 6a01 723a 7402 7c00 6a03 7404 a005 7c00  j.r:t.|.j.t...|.
+00003b50: 6a06 6a07 6a08 a101 7404 a009 7c00 6a06  j.j.j...t...|.j.
+00003b60: 6a07 6a08 a101 8303 7c00 5f00 6e28 7402  j.j.....|._.n(t.
+00003b70: 7c00 6a03 7404 a005 7c00 6a06 6a07 6a0a  |.j.t...|.j.j.j.
+00003b80: a101 7404 a009 7c00 6a06 6a07 6a0a a101  ..t...|.j.j.j...
+00003b90: 8303 7c00 5f00 7c00 a00b a100 0100 6e18  ..|._.|.......n.
+00003ba0: 7c00 6a00 a00c a100 0100 6400 7c00 5f00  |.j.......d.|._.
+00003bb0: 7c00 a00b a100 0100 6400 5300 722b 0000  |.......d.S.r+..
+00003bc0: 0029 0d72 fb00 0000 72c2 0000 0072 4500  .).r....r....rE.
+00003bd0: 0000 726d 0000 0072 5600 0000 da03 6d69  ..rm...rV.....mi
+00003be0: 6e72 7d00 0000 72f0 0000 0072 9c00 0000  nr}...r....r....
+00003bf0: da03 6d61 7872 1b00 0000 7290 0000 0072  ..maxr....r....r
+00003c00: 2c00 0000 7229 0000 0072 2400 0000 7224  ,...r)...r$...r$
+00003c10: 0000 0072 2500 0000 7286 0000 0052 0200  ...r%...r....R..
+00003c20: 0073 2000 0000 0001 0a01 0601 0201 0401  .s .............
+00003c30: 0e01 0efd 0806 0201 0401 0e01 0efd 0605  ................
+00003c40: 0a02 0a01 0601 7a1f 506c 6f74 4361 6e76  ......z.PlotCanv
+00003c50: 6173 2e74 6f67 676c 655f 7261 6e67 6573  as.toggle_ranges
+00003c60: 656c 6563 746f 7263 0200 0000 0000 0000  electorc........
+00003c70: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00003c80: 730a 0000 007c 017c 005f 0064 0053 0072  s....|.|._.d.S.r
+00003c90: 2b00 0000 2901 72f2 0000 0029 0272 2200  +...).r....).r".
+00003ca0: 0000 72f2 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
+00003cb0: 0072 2500 0000 da0d 7365 745f 7265 7369  .r%.....set_resi
+00003cc0: 6475 616c 7366 0200 0073 0200 0000 0001  dualsf...s......
+00003cd0: 7a18 506c 6f74 4361 6e76 6173 2e73 6574  z.PlotCanvas.set
+00003ce0: 5f72 6573 6964 7561 6c73 6302 0000 0000  _residualsc.....
+00003cf0: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00003d00: 0000 0073 4400 0000 7c00 6a00 6a01 723a  ...sD...|.j.j.r:
+00003d10: 7c00 6a00 6a02 733a 7c00 6a03 7340 7c00  |.j.j.s:|.j.s@|.
+00003d20: 6a04 7c01 6401 1900 6402 6403 6404 8d03  j.|.d...d.d.d...
+00003d30: 5c01 7c00 5f03 7c00 6a05 a006 a100 0100  \.|._.|.j.......
+00003d40: 6e06 7c01 7c00 5f07 6405 5300 2906 7a47  n.|.|._.d.S.).zG
+00003d50: 0a20 2020 2020 2020 2053 6574 7320 626f  .        Sets bo
+00003d60: 7468 2074 6865 2069 6e69 7469 616c 2067  th the initial g
+00003d70: 7565 7373 2066 6974 6c69 6e65 2061 6e64  uess fitline and
+00003d80: 2062 6573 7420 6669 7420 6c69 6e65 0a20   best fit line. 
+00003d90: 2020 2020 2020 2072 1300 0000 7a03 2d2d         r....z.--
+00003da0: 677a 0d69 6e69 7469 616c 2067 7565 7373  gz.initial guess
+00003db0: 2901 7298 0000 004e 2908 727d 0000 0072  ).r....N).r}...r
+00003dc0: b300 0000 da0c 6d6f 6465 6c5f 7265 7375  ......model_resu
+00003dd0: 6c74 72f4 0000 0072 0801 0000 726d 0000  ltr....r....rm..
+00003de0: 0072 9b00 0000 72f1 0000 0029 0272 2200  .r....r....).r".
+00003df0: 0000 72f1 0000 0072 2400 0000 7224 0000  ..r....r$...r$..
+00003e00: 0072 2500 0000 da0b 7365 745f 6669 746c  .r%.....set_fitl
+00003e10: 696e 6569 0200 0073 0e00 0000 0004 1001  inei...s........
+00003e20: 0604 0401 0aff 0a03 0c02 7a16 506c 6f74  ..........z.Plot
+00003e30: 4361 6e76 6173 2e73 6574 5f66 6974 6c69  Canvas.set_fitli
+00003e40: 6e65 6301 0000 0000 0000 0000 0000 0001  nec.............
+00003e50: 0000 0004 0000 0043 0000 0073 3a00 0000  .......C...s:...
+00003e60: 7c00 6a00 6400 7500 7222 7c00 6a01 6a02  |.j.d.u.r"|.j.j.
+00003e70: a003 7404 6a05 0b00 7404 6a05 a102 0100  ..t.j...t.j.....
+00003e80: 6e14 7c00 6a01 6a02 6a03 7c00 6a00 a006  n.|.j.j.j.|.j...
+00003e90: a100 8e00 0100 6400 5300 722b 0000 0029  ......d.S.r+...)
+00003ea0: 0772 fb00 0000 727d 0000 0072 f000 0000  .r....r}...r....
+00003eb0: da08 7365 745f 6d61 736b 7256 0000 00da  ..set_maskrV....
+00003ec0: 0369 6e66 724e 0000 0072 2900 0000 7224  .infrN...r)...r$
+00003ed0: 0000 0072 2400 0000 7225 0000 0072 4e00  ...r$...r%...rN.
+00003ee0: 0000 7902 0000 7306 0000 0000 010a 0118  ..y...s.........
+00003ef0: 027a 1450 6c6f 7443 616e 7661 732e 6765  .z.PlotCanvas.ge
+00003f00: 745f 7261 6e67 6563 0200 0000 0000 0000  t_rangec........
+00003f10: 0000 0000 0400 0000 0400 0000 4f00 0000  ............O...
+00003f20: 7320 0000 007c 006a 006a 017c 016a 027c  s ...|.j.j.|.j.|
+00003f30: 016a 0367 027c 02a2 0152 0069 007c 03a4  .j.g.|...R.i.|..
+00003f40: 018e 0153 0029 017a 460a 2020 2020 2020  ...S.).zF.      
+00003f50: 2020 636f 6e76 656e 6965 6e63 6520 6675    convenience fu
+00003f60: 6e63 7469 6f6e 2066 6f72 2070 6c6f 7474  nction for plott
+00003f70: 696e 6720 636f 6d70 6c65 7820 7175 616e  ing complex quan
+00003f80: 7469 7469 6573 0a20 2020 2020 2020 2029  tities.        )
+00003f90: 0472 6d00 0000 729a 0000 00da 0472 6561  .rm...r......rea
+00003fa0: 6cda 0469 6d61 6729 0472 2200 0000 72f0  l..imag).r"...r.
+00003fb0: 0000 0072 b700 0000 7280 0000 0072 2400  ...r....r....r$.
+00003fc0: 0000 7224 0000 0072 2500 0000 7208 0100  ..r$...r%...r...
+00003fd0: 007f 0200 0073 0200 0000 0004 7a17 506c  .....s......z.Pl
+00003fe0: 6f74 4361 6e76 6173 2e70 6c6f 745f 636f  otCanvas.plot_co
+00003ff0: 6d70 6c65 7863 0100 0000 0000 0000 0000  mplexc..........
+00004000: 0000 0300 0000 0300 0000 4b00 0000 7320  ..........K...s 
+00004010: 0000 0074 0064 0183 017d 0264 027c 0176  ...t.d...}.d.|.v
+00004020: 0072 1c7c 0164 0219 007c 0264 033c 007c  .r.|.d...|.d.<.|
+00004030: 0253 0029 044e 72b6 0000 0072 c700 0000  .S.).Nr....r....
+00004040: 721e 0000 0072 0300 0000 2903 7222 0000  r....r....).r"..
+00004050: 0072 8000 0000 72f6 0000 0072 2400 0000  .r....r....r$...
+00004060: 7224 0000 0072 2500 0000 da15 6372 6561  r$...r%.....crea
+00004070: 7465 5f66 6974 6c69 6e65 5f6b 7761 7267  te_fitline_kwarg
+00004080: 7385 0200 0073 0800 0000 0001 0801 0801  s....s..........
+00004090: 0c01 7a20 506c 6f74 4361 6e76 6173 2e63  ..z PlotCanvas.c
+000040a0: 7265 6174 655f 6669 746c 696e 655f 6b77  reate_fitline_kw
+000040b0: 6172 6773 6301 0000 0000 0000 0000 0000  argsc...........
+000040c0: 0006 0000 0008 0000 0043 0000 0073 0002  .........C...s..
+000040d0: 0000 7c00 6a00 6a01 72a6 7c00 6a00 6a02  ..|.j.j.r.|.j.j.
+000040e0: 72a6 7c00 6a00 6a01 6a03 7c00 6a00 6a01  r.|.j.j.j.|.j.j.
+000040f0: 6a04 7c00 6a00 6a05 6a06 6401 8d02 7d01  j.|.j.j.j.d...}.
+00004100: 7c00 6a07 723e 7c00 6a07 a008 a100 0100  |.j.r>|.j.......
+00004110: 7c00 6a09 7254 7c00 6a09 a008 a100 0100  |.j.rT|.j.......
+00004120: 6400 7c00 5f09 7c00 6a0a 6a0b a00c a100  d.|._.|.j.j.....
+00004130: 0100 7c00 6a0d 7c01 6402 6602 6900 7c00  ..|.j.|.d.f.i.|.
+00004140: 6a0e a401 8e01 5c01 7c00 5f07 7c00 6a00  j.....\.|._.|.j.
+00004150: 6a01 6a0f 7c00 6a0a 6403 6404 6405 6406  j.j.|.j.d.d.d.d.
+00004160: 6901 6407 8d04 7c00 5f10 7c00 6a11 a012  i.d...|._.|.j...
+00004170: a100 0100 9001 6e02 7c00 6a13 6400 7501  ......n.|.j.d.u.
+00004180: 9001 7282 7c00 6a14 6400 7500 72ce 7c00  ..r.|.j.d.u.r.|.
+00004190: 6a0a 6a15 6408 6409 640a 640b 8d03 0100  j.j.d.d.d.d.....
+000041a0: 7416 640c 1900 72e8 7417 a018 7c00 6a00  t.d...r.t...|.j.
+000041b0: 6a05 6a06 a101 7d02 6e16 7417 a019 6408  j.j...}.n.t...d.
+000041c0: 741a 7c00 6a00 6a05 6a06 8301 a102 7d02  t.|.j.j.j.....}.
+000041d0: 7417 a01b 6700 a101 7d03 741c 741a 7c00  t...g...}.t.t.|.
+000041e0: 6a00 6a05 6a06 8301 8301 4400 5d32 7d04  j.j.j.....D.]2}.
+000041f0: 7c00 6a00 6a05 6a1d 7c04 1900 640d 6b02  |.j.j.j.|...d.k.
+00004200: 9001 721a 7417 a01e 7c03 7c00 6a00 6a05  ..r.t...|.|.j.j.
+00004210: 6a06 7c04 1900 6701 a102 7d03 9001 711a  j.|...g...}...q.
+00004220: 7c00 6a1f a020 7c03 7c02 6400 741a 7c00  |.j.. |.|.d.t.|.
+00004230: 6a13 8301 8502 1900 1900 7c00 6a13 7c02  j.........|.j.|.
+00004240: 6400 741a 7c00 6a13 8301 8502 1900 1900  d.t.|.j.........
+00004250: a102 0100 7c00 6a21 6400 7501 9001 72a8  ....|.j!d.u...r.
+00004260: 7c00 6a07 a020 7c00 6a21 6408 1900 7c00  |.j.. |.j!d...|.
+00004270: 6a21 640e 1900 a102 0100 7c00 6a11 a022  j!d.......|.j.."
+00004280: a100 0100 7c00 6a11 a023 a100 0100 7c00  ....|.j..#....|.
+00004290: 6a0a a022 a100 0100 7c00 6a0a a023 a100  j.."....|.j..#..
+000042a0: 0100 7424 7417 a025 7c00 6a0a a026 a100  ..t$t..%|.j..&..
+000042b0: a101 8301 7d05 7c00 6a0a a027 7c05 0b00  ....}.|.j..'|...
+000042c0: 7c05 a102 0100 7c00 a028 a100 0100 6400  |.....|..(....d.
+000042d0: 5300 290f 4e29 02da 0670 6172 616d 7372  S.).N)...paramsr
+000042e0: 1b00 0000 7a03 2d2d 6b7a 032e 2d6b da03  ....z.--kz..-k..
+000042f0: 6162 7372 9800 0000 72cb 0000 0029 0472  absr....r....).r
+00004300: 2300 0000 da07 6461 7461 666d 74da 0d70  #.....datafmt..p
+00004310: 6172 7365 5f63 6f6d 706c 6578 da08 6461  arse_complex..da
+00004320: 7461 5f6b 7773 7201 0000 0072 1900 0000  ta_kwsr....r....
+00004330: 7211 0100 0029 0372 9c00 0000 721d 0000  r....).r....r...
+00004340: 0072 1e00 0000 da0e 534f 5254 5f52 4553  .r......SORT_RES
+00004350: 4944 5541 4c53 5472 1300 0000 2929 727d  IDUALSTr....))r}
+00004360: 0000 0072 1801 0000 72b3 0000 00da 0465  ...r....r......e
+00004370: 7661 6c72 1f01 0000 72f0 0000 0072 1b00  valr....r....r..
+00004380: 0000 7200 0100 0072 2c00 0000 72f4 0000  ..r....r,...r...
+00004390: 0072 8c00 0000 da05 6c69 6e65 73da 0563  .r......lines..c
+000043a0: 6c65 6172 7208 0100 0072 f600 0000 da0e  learr....r......
+000043b0: 706c 6f74 5f72 6573 6964 7561 6c73 72f3  plot_residualsr.
+000043c0: 0000 0072 6d00 0000 729b 0000 0072 f200  ...rm...r....r..
+000043d0: 0000 7202 0100 00da 0761 7868 6c69 6e65  ..r......axhline
+000043e0: 7214 0000 0072 5600 0000 da07 6172 6773  r....rV.....args
+000043f0: 6f72 74da 0661 7261 6e67 6572 b500 0000  ort..aranger....
+00004400: 7299 0000 00da 0572 616e 6765 da04 6d61  r......range..ma
+00004410: 736b 72bd 0000 0072 0101 0000 7207 0100  skr....r....r...
+00004420: 0072 f100 0000 5a05 7265 6c69 6dda 0961  .r....Z.relim..a
+00004430: 7574 6f73 6361 6c65 7216 0100 0072 2001  utoscaler....r .
+00004440: 0000 5a08 6765 745f 796c 696d da08 7365  ..Z.get_ylim..se
+00004450: 745f 796c 696d 7290 0000 0029 0672 2200  t_ylimr....).r".
+00004460: 0000 5a07 6669 745f 7332 31da 056f 7264  ..Z.fit_s21..ord
+00004470: 6572 5a09 6461 7461 5f63 6f70 7972 b200  erZ.data_copyr..
+00004480: 0000 da04 796d 6178 7224 0000 0072 2400  ....ymaxr$...r$.
+00004490: 0000 7225 0000 0072 7b00 0000 8b02 0000  ..r%...r{.......
+000044a0: 735e 0000 0000 0310 0208 0110 ff06 0606  s^..............
+000044b0: 010a 0106 010a 0106 020c 0604 0104 ff04  ................
+000044c0: 0104 ff0a 0308 0104 0102 0102 0106 fc08  ................
+000044d0: 060e 020c 020a 0112 0308 0112 0216 0d0a  ................
+000044e0: 0116 0114 0104 0110 ff08 0306 0114 0116  ................
+000044f0: fe04 0a0c 011a 030a 010a 010a 010a 0314  ................
+00004500: 0110 037a 1650 6c6f 7443 616e 7661 732e  ...z.PlotCanvas.
+00004510: 7570 6461 7465 5f70 6c6f 7463 0100 0000  update_plotc....
+00004520: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+00004530: 4300 0000 7338 0000 007c 006a 0072 347c  C...s8...|.j.r4|
+00004540: 006a 0044 005d 267d 017c 006a 016a 027c  .j.D.]&}.|.j.j.|
+00004550: 0164 0119 007c 0164 0219 007c 0164 0319  .d...|.d...|.d..
+00004560: 0064 0464 0164 058d 0501 0071 0c64 0053  .d.d.d.....q.d.S
+00004570: 0029 064e 7201 0000 0072 1300 0000 7262  .).Nr....r....rb
+00004580: 0000 0072 9400 0000 2903 7298 0000 0072  ...r....).r....r
+00004590: 9600 0000 7297 0000 0029 0372 f500 0000  ....r....).r....
+000045a0: 726d 0000 0072 9a00 0000 2902 7222 0000  rm...r....).r"..
+000045b0: 0072 b100 0000 7224 0000 0072 2400 0000  .r....r$...r$...
+000045c0: 7225 0000 0072 0301 0000 e302 0000 730a  r%...r........s.
+000045d0: 0000 0000 0106 010a 0106 0116 ff7a 1f50  .............z.P
+000045e0: 6c6f 7443 616e 7661 732e 706c 6f74 5f61  lotCanvas.plot_a
+000045f0: 6464 6974 696f 6e61 6c5f 6461 7461 6301  dditional_datac.
+00004600: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00004610: 0000 0043 0000 0073 0c00 0000 7c00 a000  ...C...s....|...
+00004620: a100 0100 6400 5300 722b 0000 0029 0172  ....d.S.r+...).r
+00004630: 3d00 0000 7229 0000 0072 2400 0000 7224  =...r)...r$...r$
+00004640: 0000 0072 2500 0000 7290 0000 00ea 0200  ...r%...r.......
+00004650: 0073 0200 0000 0002 7a11 506c 6f74 4361  .s......z.PlotCa
+00004660: 6e76 6173 2e72 6564 7261 774e 2912 7241  nvas.redrawN).rA
+00004670: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+00004680: 0000 7226 0000 0072 f700 0000 72f8 0000  ..r&...r....r...
+00004690: 0072 1301 0000 7214 0100 0072 8600 0000  .r....r....r....
+000046a0: 7217 0100 0072 1901 0000 724e 0000 0072  r....r....rN...r
+000046b0: 0801 0000 721e 0100 0072 7b00 0000 7203  ....r....r{...r.
+000046c0: 0100 0072 9000 0000 7224 0000 0072 2400  ...r....r$...r$.
+000046d0: 0000 7224 0000 0072 2500 0000 726a 0000  ..r$...r%...rj..
+000046e0: 0070 0100 0073 2000 0000 0801 0402 087f  .p...s .........
+000046f0: 0046 0808 080a 0805 0803 0814 0803 0810  .F..............
+00004700: 0806 0806 0806 0858 0807 726a 0000 0063  .......X..rj...c
+00004710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004720: 0200 0000 4000 0000 7328 0000 0065 005a  ....@...s(...e.Z
+00004730: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
+00004740: 0464 0464 0584 005a 0564 0664 0784 005a  .d.d...Z.d.d...Z
+00004750: 0664 0853 0029 09da 0b50 6172 616d 5769  .d.S.)...ParamWi
+00004760: 6467 6574 7a2b 5174 2077 6964 6765 7420  dgetz+Qt widget 
+00004770: 746f 2073 686f 7720 616e 6420 6368 616e  to show and chan
+00004780: 6765 2061 2066 6974 7061 7261 6d65 7465  ge a fitparamete
+00004790: 7263 0200 0000 0000 0000 0000 0000 0300  rc..............
+000047a0: 0000 0300 0000 4300 0000 737a 0000 0074  ......C...sz...t
+000047b0: 006a 01a0 027c 00a1 0101 007c 017c 005f  .j...|.....|.|._
+000047c0: 0374 00a0 047c 016a 05a1 017c 005f 0674  .t...|.j...|._.t
+000047d0: 00a0 0764 01a1 017c 005f 087c 00a0 09a1  ...d...|._.|....
+000047e0: 0001 0074 00a0 0a64 02a1 017c 005f 0b74  ...t...d...|._.t
+000047f0: 00a0 0ca1 007d 027c 02a0 0d7c 006a 06a1  .....}.|...|.j..
+00004800: 0101 007c 02a0 0d7c 006a 08a1 0101 007c  ...|...|.j.....|
+00004810: 02a0 0d7c 006a 0ba1 0101 007c 00a0 0e7c  ...|.j.....|...|
+00004820: 02a1 0101 0064 0053 0029 034e 72d8 0000  .....d.S.).Nr...
+00004830: 00da 0366 6978 290f 7210 0000 0072 6700  ...fix).r....rg.
+00004840: 0000 7226 0000 00da 0370 6172 da06 514c  ..r&.....par..QL
+00004850: 6162 656c da04 6e61 6d65 7298 0000 0072  abel..namer....r
+00004860: a600 0000 da04 6564 6974 da0c 7570 6461  ......edit..upda
+00004870: 7465 5f76 616c 7565 5a09 5143 6865 636b  te_valueZ.QCheck
+00004880: 426f 78da 0563 6865 636b da0b 5148 426f  Box..check..QHBo
+00004890: 784c 6179 6f75 7472 7900 0000 7268 0000  xLayoutry...rh..
+000048a0: 0029 0372 2200 0000 7234 0100 0072 7800  .).r"...r4...rx.
+000048b0: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+000048c0: 0072 2600 0000 f202 0000 7316 0000 0000  .r&.......s.....
+000048d0: 010c 0106 010e 010c 0108 010c 0108 010c  ................
+000048e0: 010c 010c 017a 1450 6172 616d 5769 6467  .....z.ParamWidg
+000048f0: 6574 2e5f 5f69 6e69 745f 5f63 0100 0000  et.__init__c....
+00004900: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00004910: 4300 0000 7324 0000 0074 007c 006a 01a0  C...s$...t.|.j..
+00004920: 02a1 0083 017c 006a 035f 047c 006a 05a0  .....|.j._.|.j..
+00004930: 06a1 007c 006a 035f 0764 0153 0029 027a  ...|.j._.d.S.).z
+00004940: 3672 6561 6420 7573 6572 696e 7075 7420  6read userinput 
+00004950: 2876 616c 7565 2061 6e64 2066 6978 6564  (value and fixed
+00004960: 2920 696e 2074 6865 2070 6172 616d 6574  ) in the paramet
+00004970: 6572 2064 6174 614e 2908 da05 666c 6f61  er dataN)...floa
+00004980: 7472 3701 0000 72ba 0000 0072 3401 0000  tr7...r....r4...
+00004990: da05 7661 6c75 6572 3901 0000 5a09 6973  ..valuer9...Z.is
+000049a0: 4368 6563 6b65 64da 0566 6978 6564 7229  Checked..fixedr)
+000049b0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+000049c0: 0000 da0a 7265 6164 5f76 616c 7565 ff02  ....read_value..
+000049d0: 0000 7306 0000 0000 0212 010e 017a 1650  ..s..........z.P
+000049e0: 6172 616d 5769 6467 6574 2e72 6561 645f  aramWidget.read_
+000049f0: 7661 6c75 6563 0100 0000 0000 0000 0000  valuec..........
+00004a00: 0000 0200 0000 0600 0000 4300 0000 7322  ..........C...s"
+00004a10: 0000 007c 006a 006a 017d 017c 006a 02a0  ...|.j.j.}.|.j..
+00004a20: 0374 047c 0174 0564 0119 0083 02a1 0101  .t.|.t.d........
+00004a30: 0064 0053 0029 024e da12 5349 474e 4946  .d.S.).N..SIGNIF
+00004a40: 4943 414e 545f 4449 4749 5453 2906 7234  ICANT_DIGITS).r4
+00004a50: 0100 0072 3c01 0000 7237 0100 00da 0773  ...r<...r7.....s
+00004a60: 6574 5465 7874 7215 0000 0072 1400 0000  etTextr....r....
+00004a70: 2902 7222 0000 0072 3c01 0000 7224 0000  ).r"...r<...r$..
+00004a80: 0072 2400 0000 7225 0000 0072 3801 0000  .r$...r%...r8...
+00004a90: 0503 0000 7306 0000 0000 0108 0116 017a  ....s..........z
+00004aa0: 1850 6172 616d 5769 6467 6574 2e75 7064  .ParamWidget.upd
+00004ab0: 6174 655f 7661 6c75 654e 2907 7241 0000  ate_valueN).rA..
+00004ac0: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
+00004ad0: 7226 0000 0072 3e01 0000 7238 0100 0072  r&...r>...r8...r
+00004ae0: 2400 0000 7224 0000 0072 2400 0000 7225  $...r$...r$...r%
+00004af0: 0000 0072 3201 0000 ef02 0000 7308 0000  ...r2.......s...
+00004b00: 0008 0104 0208 0d08 0672 3201 0000 6300  .........r2...c.
+00004b10: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00004b20: 0000 0040 0000 0073 2000 0000 6500 5a01  ...@...s ...e.Z.
+00004b30: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
+00004b40: 6404 6405 8400 5a05 6406 5300 2907 da0c  d.d...Z.d.S.)...
+00004b50: 5265 706f 7274 5769 6467 6574 7a54 7072  ReportWidgetzTpr
+00004b60: 696e 7473 2061 2066 6974 7265 706f 7274  ints a fitreport
+00004b70: 2069 6e20 6120 6e6f 6e2d 6564 6974 6162   in a non-editab
+00004b80: 6c65 2074 6578 7462 6f78 2e20 5265 706f  le textbox. Repo
+00004b90: 7274 2073 686f 756c 6420 6265 2061 2028  rt should be a (
+00004ba0: 6e65 7374 6564 2920 6469 6374 696f 6e61  nested) dictiona
+00004bb0: 7279 6301 0000 0000 0000 0000 0000 0001  ryc.............
+00004bc0: 0000 0007 0000 0043 0000 0073 3600 0000  .......C...s6...
+00004bd0: 7400 6a01 a002 7c00 6401 a102 0100 7c00  t.j...|.d.....|.
+00004be0: a003 7404 a005 7406 6402 1900 7406 6403  ..t...t.d...t.d.
+00004bf0: 1900 a102 a101 0100 7c00 a007 6404 a101  ........|...d...
+00004c00: 0100 6400 5300 2905 4e72 db00 0000 da0b  ..d.S.).Nr......
+00004c10: 5245 504f 5254 5f46 4f4e 54da 0b52 4550  REPORT_FONT..REP
+00004c20: 4f52 545f 5349 5a45 5429 0872 1000 0000  ORT_SIZET).r....
+00004c30: da09 5154 6578 7445 6469 7472 2600 0000  ..QTextEditr&...
+00004c40: 7273 0000 0072 0f00 0000 7274 0000 0072  rs...r....rt...r
+00004c50: 1400 0000 5a0b 7365 7452 6561 644f 6e6c  ....Z.setReadOnl
+00004c60: 7972 2900 0000 7224 0000 0072 2400 0000  yr)...r$...r$...
+00004c70: 7225 0000 0072 2600 0000 0e03 0000 7310  r%...r&.......s.
+00004c80: 0000 0000 0106 0102 0102 fe04 0404 0112  ................
+00004c90: ff04 037a 1552 6570 6f72 7457 6964 6765  ...z.ReportWidge
+00004ca0: 742e 5f5f 696e 6974 5f5f 6302 0000 0000  t.__init__c.....
+00004cb0: 0000 0000 0000 0002 0000 0003 0000 0003  ................
+00004cc0: 0000 0073 2400 0000 8700 8701 6602 6401  ...s$.......f.d.
+00004cd0: 6402 8408 8900 8801 a000 a100 0100 8800  d...............
+00004ce0: 7c01 6403 8302 0100 6404 5300 2905 7a57  |.d.....d.S.).zW
+00004cf0: 7570 6461 7465 7320 7468 6520 7465 7874  updates the text
+00004d00: 206f 6620 7468 6520 7465 7874 6564 6974   of the textedit
+00004d10: 626f 7820 7769 7468 2074 6865 2063 6f6e  box with the con
+00004d20: 7465 6e74 206f 6620 6120 286e 6573 7465  tent of a (neste
+00004d30: 6429 2064 6963 7469 6f6e 6172 7920 6669  d) dictionary fi
+00004d40: 7472 6570 6f72 7463 0200 0000 0000 0000  treportc........
+00004d50: 0000 0000 0500 0000 0500 0000 1300 0000  ................
+00004d60: 73b8 0000 007c 00a0 00a1 0044 005d a05c  s....|.....D.].\
+00004d70: 027d 027d 0374 017c 0383 0174 0275 0072  .}.}.t.|...t.u.r
+00004d80: 687c 0164 016b 0272 2e88 01a0 0364 02a1  h|.d.k.r.....d..
+00004d90: 0101 0088 01a0 0374 047c 0283 01a1 0101  .......t.|......
+00004da0: 007c 0164 016b 0272 4e88 01a0 0364 03a1  .|.d.k.rN....d..
+00004db0: 0101 0088 01a0 0364 04a1 0101 0088 007c  .......d.......|
+00004dc0: 037c 0164 0117 0083 0201 0071 0874 017c  .|.d.......q.t.|
+00004dd0: 0383 0174 056a 066b 0272 8674 077c 0374  ...t.j.k.r.t.|.t
+00004de0: 0864 0519 0083 027d 046e 0874 047c 0383  .d.....}.n.t.|..
+00004df0: 017d 0488 01a0 0374 047c 0283 0164 0617  .}.....t.|...d..
+00004e00: 007c 0417 0064 0717 00a1 0101 0071 0888  .|...d.......q..
+00004e10: 01a0 0364 07a1 0101 0064 0053 0029 084e  ...d.....d.S.).N
+00004e20: 7213 0000 007a 0b3d 3d3d 3d3d 3d3d 3d3d  r....z.=========
+00004e30: 3d20 7a0c 203d 3d3d 3d3d 3d3d 3d3d 3d20  = z. ========== 
+00004e40: 7a02 0a0a 723f 0100 007a 0409 093a 20da  z...r?...z...: .
+00004e50: 010a 2909 da05 6974 656d 73da 0474 7970  ..)...items..typ
+00004e60: 6572 0401 0000 5a0f 696e 7365 7274 506c  er....Z.insertPl
+00004e70: 6169 6e54 6578 7472 b600 0000 7256 0000  ainTextr....rV..
+00004e80: 00da 0766 6c6f 6174 3634 7215 0000 0072  ...float64r....r
+00004e90: 1400 0000 2905 da05 6164 6963 74da 056c  ....)...adict..l
+00004ea0: 6576 656c 72e8 0000 0072 b100 0000 5a08  evelr....r....Z.
+00004eb0: 6974 656d 5f73 7472 a902 da0a 7072 696e  item_str....prin
+00004ec0: 745f 6469 6374 7222 0000 0072 2400 0000  t_dictr"...r$...
+00004ed0: 7225 0000 0072 4c01 0000 1b03 0000 7320  r%...rL.......s 
+00004ee0: 0000 0000 0110 010c 0108 010a 010e 0108  ................
+00004ef0: 010a 010a 0110 020e 0102 0108 ff06 0408  ................
+00004f00: 011c 017a 2e52 6570 6f72 7457 6964 6765  ...z.ReportWidge
+00004f10: 742e 7570 6461 7465 5f72 6570 6f72 742e  t.update_report.
+00004f20: 3c6c 6f63 616c 733e 2e70 7269 6e74 5f64  <locals>.print_d
+00004f30: 6963 7472 1300 0000 4e29 0172 2701 0000  ictr....N).r'...
+00004f40: 2902 7222 0000 00da 0966 6974 7265 706f  ).r".....fitrepo
+00004f50: 7274 7224 0000 0072 4b01 0000 7225 0000  rtr$...rK...r%..
+00004f60: 00da 0d75 7064 6174 655f 7265 706f 7274  ...update_report
+00004f70: 1803 0000 7306 0000 0000 030e 1408 017a  ....s..........z
+00004f80: 1a52 6570 6f72 7457 6964 6765 742e 7570  .ReportWidget.up
+00004f90: 6461 7465 5f72 6570 6f72 744e 2906 7241  date_reportN).rA
+00004fa0: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
+00004fb0: 0000 7226 0000 0072 4e01 0000 7224 0000  ..r&...rN...r$..
+00004fc0: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
+00004fd0: 7241 0100 000b 0300 0073 0600 0000 0801  rA.......s......
+00004fe0: 0402 080a 7241 0100 0063 0000 0000 0000  ....rA...c......
+00004ff0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00005000: 0000 7350 0000 0065 005a 0164 005a 0264  ..sP...e.Z.d.Z.d
+00005010: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
+00005020: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
+00005030: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
+00005040: 005a 0964 0e64 0f84 005a 0a64 1064 1184  .Z.d.d...Z.d.d..
+00005050: 005a 0b64 1253 0029 13da 0b4d 6f64 656c  .Z.d.S.)...Model
+00005060: 5769 6467 6574 7a2b 5174 2077 6964 6765  Widgetz+Qt widge
+00005070: 7420 746f 2073 686f 7720 616e 6420 636f  t to show and co
+00005080: 6e74 726f 6c20 7468 6520 6669 7420 6d6f  ntrol the fit mo
+00005090: 6465 6c63 0300 0000 0000 0000 0000 0000  delc............
+000050a0: 0300 0000 0400 0000 4300 0000 732a 0000  ........C...s*..
+000050b0: 007c 017c 005f 0074 016a 02a0 037c 0064  .|.|._.t.j...|.d
+000050c0: 01a1 0201 007c 00a0 047c 02a1 0101 007c  .....|...|.....|
+000050d0: 00a0 05a1 0001 0064 0053 0029 024e 7a0e  .......d.S.).Nz.
+000050e0: 4d6f 6465 6c20 7365 7474 696e 6773 2906  Model settings).
+000050f0: da05 6d6f 6465 6c72 1000 0000 da09 5147  ..modelr......QG
+00005100: 726f 7570 426f 7872 2600 0000 da07 696e  roupBoxr&.....in
+00005110: 6974 4755 49da 0a73 6574 5f77 6569 6768  itGUI..set_weigh
+00005120: 7429 0372 2200 0000 7250 0100 00da 0d77  t).r"...rP.....w
+00005130: 6569 6768 746f 7074 696f 6e73 7224 0000  eightoptionsr$..
+00005140: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00005150: 3603 0000 7308 0000 0000 0106 010e 010a  6...s...........
+00005160: 017a 144d 6f64 656c 5769 6467 6574 2e5f  .z.ModelWidget._
+00005170: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00005180: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00005190: 7396 0000 0074 00a0 01a1 007d 0274 00a0  s....t.....}.t..
+000051a0: 02a1 007d 0364 0164 0284 007c 006a 036a  ...}.d.d...|.j.j
+000051b0: 0444 0083 017c 005f 0574 00a0 0664 03a1  .D...|._.t...d..
+000051c0: 017c 005f 0774 00a0 08a1 007c 005f 097c  .|._.t.....|._.|
+000051d0: 006a 09a0 0a7c 01a1 0101 007c 03a0 0b7c  .j...|.....|...|
+000051e0: 006a 07a1 0101 007c 03a0 0b7c 006a 09a1  .j.....|...|.j..
+000051f0: 0101 007c 03a0 0c64 04a1 0101 007c 006a  ...|...d.....|.j
+00005200: 0544 005d 0e7d 047c 02a0 0b7c 04a1 0101  .D.].}.|...|....
+00005210: 0071 6e7c 02a0 0d7c 03a1 0101 007c 00a0  .qn|...|.....|..
+00005220: 0e7c 02a1 0101 0064 0053 0029 054e 6301  .|.....d.S.).Nc.
+00005230: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00005240: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00005250: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
+00005260: 7224 0000 0029 0172 3201 0000 2902 7246  r$...).r2...).rF
+00005270: 0000 0072 3401 0000 7224 0000 0072 2400  ...r4...r$...r$.
+00005280: 0000 7225 0000 0072 4800 0000 3f03 0000  ..r%...rH...?...
+00005290: 7249 0000 007a 274d 6f64 656c 5769 6467  rI...z'ModelWidg
+000052a0: 6574 2e69 6e69 7447 5549 2e3c 6c6f 6361  et.initGUI.<loca
+000052b0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7a0d  ls>.<listcomp>z.
+000052c0: 5765 6967 6874 6564 2046 6974 3a72 1300  Weighted Fit:r..
+000052d0: 0000 290f 7210 0000 0072 6900 0000 723a  ..).r....ri...r:
+000052e0: 0100 0072 5001 0000 da07 6669 7470 6172  ...rP.....fitpar
+000052f0: 73da 0870 6172 7669 6577 7372 3501 0000  s..parviewsr5...
+00005300: 5a0b 5765 6967 6874 4c61 6265 6c72 a500  Z.WeightLabelr..
+00005310: 0000 da0f 5977 6569 6768 7463 6f6d 626f  ....Yweightcombo
+00005320: 626f 785a 0861 6464 4974 656d 7372 7900  boxZ.addItemsry.
+00005330: 0000 5a0a 6164 6453 7472 6574 6368 5a09  ..Z.addStretchZ.
+00005340: 6164 644c 6179 6f75 7472 6800 0000 2905  addLayoutrh...).
+00005350: 7222 0000 0072 5401 0000 5a04 5642 6f78  r"...rT...Z.VBox
+00005360: 5a04 4842 6f78 da07 7061 7276 6965 7772  Z.HBox..parviewr
+00005370: 2400 0000 7224 0000 0072 2500 0000 7252  $...r$...r%...rR
+00005380: 0100 003c 0300 0073 1c00 0000 0001 0801  ...<...s........
+00005390: 0801 1401 0c01 0a01 0c01 0c01 0c01 0a01  ................
+000053a0: 0a01 0c01 0a01 0a01 7a13 4d6f 6465 6c57  ........z.ModelW
+000053b0: 6964 6765 742e 696e 6974 4755 4963 0100  idget.initGUIc..
+000053c0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000053d0: 0000 4300 0000 7310 0000 007c 006a 00a0  ..C...s....|.j..
+000053e0: 0164 01a1 0101 0064 0053 0072 1201 0000  .d.....d.S.r....
+000053f0: 2902 7257 0100 005a 0b73 6574 4469 7361  ).rW...Z.setDisa
+00005400: 626c 6564 7229 0000 0072 2400 0000 7224  bledr)...r$...r$
+00005410: 0000 0072 2500 0000 da0e 6469 7361 626c  ...r%.....disabl
+00005420: 655f 7765 6967 6874 4c03 0000 7302 0000  e_weightL...s...
+00005430: 0000 017a 1a4d 6f64 656c 5769 6467 6574  ...z.ModelWidget
+00005440: 2e64 6973 6162 6c65 5f77 6569 6768 7463  .disable_weightc
+00005450: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00005460: 0300 0000 4300 0000 7310 0000 007c 006a  ....C...s....|.j
+00005470: 00a0 0164 01a1 0101 0064 0053 0072 1201  ...d.....d.S.r..
+00005480: 0000 2902 7257 0100 005a 0a73 6574 456e  ..).rW...Z.setEn
+00005490: 6162 6c65 6472 2900 0000 7224 0000 0072  abledr)...r$...r
+000054a0: 2400 0000 7225 0000 00da 0d65 6e61 626c  $...r%.....enabl
+000054b0: 655f 7765 6967 6874 4f03 0000 7302 0000  e_weightO...s...
+000054c0: 0000 017a 194d 6f64 656c 5769 6467 6574  ...z.ModelWidget
+000054d0: 2e65 6e61 626c 655f 7765 6967 6874 6301  .enable_weightc.
+000054e0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000054f0: 0000 0043 0000 0073 0a00 0000 7c00 6a00  ...C...s....|.j.
+00005500: a001 a100 5300 722b 0000 0029 0272 5701  ....S.r+...).rW.
+00005510: 0000 729f 0000 0072 2900 0000 7224 0000  ..r....r)...r$..
+00005520: 0072 2400 0000 7225 0000 00da 0a67 6574  .r$...r%.....get
+00005530: 5f77 6569 6768 7452 0300 0073 0200 0000  _weightR...s....
+00005540: 0001 7a16 4d6f 6465 6c57 6964 6765 742e  ..z.ModelWidget.
+00005550: 6765 745f 7765 6967 6874 6301 0000 0000  get_weightc.....
+00005560: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00005570: 0000 0073 2e00 0000 7c00 6a00 a001 7c00  ...s....|.j...|.
+00005580: 6a02 6a03 7404 6a05 6a06 a102 7d01 7c01  j.j.t.j.j...}.|.
+00005590: 6401 6b05 722a 7c00 6a00 a007 7c01 a101  d.k.r*|.j...|...
+000055a0: 0100 6400 5300 7227 0000 0029 0872 5701  ..d.S.r'...).rW.
+000055b0: 0000 5a08 6669 6e64 5465 7874 7250 0100  ..Z.findTextrP..
+000055c0: 00da 0677 6569 6768 7472 0e00 0000 da02  ...weightr......
+000055d0: 5174 5a10 4d61 7463 6846 6978 6564 5374  QtZ.MatchFixedSt
+000055e0: 7269 6e67 5a0f 7365 7443 7572 7265 6e74  ringZ.setCurrent
+000055f0: 496e 6465 7829 0272 2200 0000 da05 696e  Index).r".....in
+00005600: 6465 7872 2400 0000 7224 0000 0072 2500  dexr$...r$...r%.
+00005610: 0000 7253 0100 0055 0300 0073 0a00 0000  ..rS...U...s....
+00005620: 0001 0601 0cff 0403 0801 7a16 4d6f 6465  ..........z.Mode
+00005630: 6c57 6964 6765 742e 7365 745f 7765 6967  lWidget.set_weig
+00005640: 6874 6301 0000 0000 0000 0000 0000 0002  htc.............
+00005650: 0000 0003 0000 0043 0000 0073 2e00 0000  .......C...s....
+00005660: 7c00 6a00 4400 5d0c 7d01 7c01 a001 a100  |.j.D.].}.|.....
+00005670: 0100 7106 7c00 a002 a100 7c00 6a03 5f04  ..q.|.....|.j._.
+00005680: 7c00 6a03 a005 a100 0100 6401 5300 2902  |.j.......d.S.).
+00005690: 7a2a 7265 6164 7320 7661 6c75 6573 2066  z*reads values f
+000056a0: 726f 6d20 7573 6572 696e 7075 7420 696e  rom userinput in
+000056b0: 746f 2074 6865 206d 6f64 656c 4e29 0672  to the modelN).r
+000056c0: 5601 0000 723e 0100 0072 5b01 0000 7250  V...r>...r[...rP
+000056d0: 0100 0072 5c01 0000 da06 7570 6461 7465  ...r\.....update
+000056e0: a902 7222 0000 0072 5801 0000 7224 0000  ..r"...rX...r$..
+000056f0: 0072 2400 0000 7225 0000 00da 0b72 6561  .r$...r%.....rea
+00005700: 645f 7661 6c75 6573 5c03 0000 730a 0000  d_values\...s...
+00005710: 0000 020a 010a 010c 010a 017a 174d 6f64  ...........z.Mod
+00005720: 656c 5769 6467 6574 2e72 6561 645f 7661  elWidget.read_va
+00005730: 6c75 6573 6301 0000 0000 0000 0000 0000  luesc...........
+00005740: 0002 0000 0003 0000 0043 0000 0073 1800  .........C...s..
+00005750: 0000 7c00 6a00 4400 5d0c 7d01 7c01 a001  ..|.j.D.].}.|...
+00005760: a100 0100 7106 6400 5300 722b 0000 0029  ....q.d.S.r+...)
+00005770: 0272 5601 0000 7238 0100 0072 6001 0000  .rV...r8...r`...
+00005780: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00005790: 0d75 7064 6174 655f 7661 6c75 6573 6403  .update_valuesd.
+000057a0: 0000 7306 0000 0000 010a 010a 017a 194d  ..s..........z.M
+000057b0: 6f64 656c 5769 6467 6574 2e75 7064 6174  odelWidget.updat
+000057c0: 655f 7661 6c75 6573 4e29 0c72 4100 0000  e_valuesN).rA...
+000057d0: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+000057e0: 2600 0000 7252 0100 0072 5901 0000 725a  &...rR...rY...rZ
+000057f0: 0100 0072 5b01 0000 7253 0100 0072 6101  ...r[...rS...ra.
+00005800: 0000 7262 0100 0072 2400 0000 7224 0000  ..rb...r$...r$..
+00005810: 0072 2400 0000 7225 0000 0072 4f01 0000  .r$...r%...rO...
+00005820: 3303 0000 7312 0000 0008 0104 0208 0608  3...s...........
+00005830: 1008 0308 0308 0308 0708 0872 4f01 0000  ...........rO...
+00005840: 2933 da06 7479 7069 6e67 7202 0000 00da  )3..typingr.....
+00005850: 0877 6172 6e69 6e67 73da 0b63 6f6c 6c65  .warnings..colle
+00005860: 6374 696f 6e73 7204 0000 0072 e900 0000  ctionsr....r....
+00005870: 72bb 0000 005a 0d73 796d 7079 2e73 6f6c  r....Z.sympy.sol
+00005880: 7665 7273 7205 0000 005a 0573 796d 7079  versr....Z.sympy
+00005890: 7206 0000 00da 0e66 696c 7465 7277 6172  r......filterwar
+000058a0: 6e69 6e67 735a 126d 6174 706c 6f74 6c69  ningsZ.matplotli
+000058b0: 622e 7061 7463 6865 7372 0501 0000 da05  b.patchesr......
+000058c0: 6e75 6d70 7972 5600 0000 da05 6c6d 6669  numpyrV.....lmfi
+000058d0: 7472 0800 0000 da0a 6d61 7470 6c6f 746c  tr......matplotl
+000058e0: 6962 7209 0000 005a 226d 6174 706c 6f74  ibr....Z"matplot
+000058f0: 6c69 622e 6261 636b 656e 6473 2e62 6163  lib.backends.bac
+00005900: 6b65 6e64 5f71 7435 6167 6772 0a00 0000  kend_qt5aggr....
+00005910: 72f9 0000 0072 0b00 0000 726b 0000 005a  r....r....rk...Z
+00005920: 116d 6174 706c 6f74 6c69 622e 6669 6775  .matplotlib.figu
+00005930: 7265 720c 0000 005a 0f6d 6174 706c 6f74  rer....Z.matplot
+00005940: 6c69 622e 7061 7468 720d 0000 00da 0550  lib.pathr......P
+00005950: 7951 7435 720e 0000 0072 0f00 0000 7210  yQt5r....r....r.
+00005960: 0000 005a 0b50 7951 7435 2e51 7447 7569  ...Z.PyQt5.QtGui
+00005970: 7211 0000 005a 0f50 7951 7435 2e51 7457  r....Z.PyQt5.QtW
+00005980: 6964 6765 7473 7212 0000 00da 095f 7365  idgetsr......_se
+00005990: 7474 696e 6773 7214 0000 00da 065f 746f  ttingsr......_to
+000059a0: 6f6c 7372 1500 0000 7217 0000 0072 4500  olsr....r....rE.
+000059b0: 0000 7267 0000 0072 4f00 0000 726a 0000  ..rg...rO...rj..
+000059c0: 0072 3201 0000 7244 0100 0072 4101 0000  .r2...rD...rA...
+000059d0: 7251 0100 0072 4f01 0000 7224 0000 0072  rQ...rO...r$...r
+000059e0: 2400 0000 7224 0000 0072 2500 0000 da08  $...r$...r%.....
+000059f0: 3c6d 6f64 756c 653e 0200 0000 7340 0000  <module>....s@..
+00005a00: 000c 0108 010c 0108 0108 010c 010c 020a  ................
+00005a10: 030c 0108 010c 010c 030c 030c 030c 010c  ................
+00005a20: 0114 010c 010c 020c 010c 0308 030e 440e  ..............D.
+00005a30: 1212 7f00 7510 7f00 7f00 7f00 0212 1c12  ....u...........
+00005a40: 28                                       (
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/_curvefitgui.py` & `complex-curve-fit-gui-1.0.9/curvefitgui/_curvefitgui.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/_gui.py` & `complex-curve-fit-gui-1.0.9/curvefitgui/_gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,19 +26,21 @@
         """
         We could check here if fitter.model.func is complex, then immediately call fit after initGUI() so that model.result populates 
         """
         self.fitter = afitter
         self.xlabel, self.ylabel = xlabel, ylabel
         self.output = (None, None)
         self.xerrorwarning = settings["XERRORWARNING"]
+        self.kwargs = kwargs
         self.initGUI(**kwargs)
         # call fit here if complex
         # if self.fitter.is_complex:
         #     self.fit()
         self.plotwidget.update_plot()
+        self.OG_model = self.fitter.model  # original model/ user entered model
 
     def closeEvent(self, event):
         """needed to properly quit when running in IPython console / Spyder IDE"""
         QtWidgets.QApplication.quit()
 
     def initGUI(self, **kwargs):
         # main GUI proprieties
@@ -55,14 +57,19 @@
         # creating the required widgets
         self.plotwidget = PlotWidget(
             self.fitter,
             self.xlabel,
             self.ylabel,
             **kwargs,
         )  # holds the plot
+
+        self.plotwidget.re_init.connect(
+            self.refresh
+        )  # signal for from update plot button
+
         self.modelview = ModelWidget(
             self.fitter.model, self.fitter.get_weightoptions()
         )  # shows the model and allows users to set fitproperties
         self.fitbutton = QtWidgets.QPushButton("FIT", clicked=self.fit)
         self.evalbutton = QtWidgets.QPushButton(
             "INITIAL EVALUATION", clicked=self.evaluate
         )
@@ -74,23 +81,23 @@
         buttonslayout = QtWidgets.QHBoxLayout()
         buttonslayout.addWidget(self.evalbutton)
         buttonslayout.addWidget(self.fitbutton)
         self.buttons.setLayout(buttonslayout)
 
         # create a frame with a vertical layout to organize the modelview, fitbutton and reportview
         self.fitcontrolframe = QtWidgets.QGroupBox()
-        fitcontrollayout = QtWidgets.QVBoxLayout()
+        self.fitcontrollayout = QtWidgets.QVBoxLayout()
         for widget in (
             self.modelview,
             self.buttons,
             self.reportview,
             self.quitbutton,
         ):
-            fitcontrollayout.addWidget(widget)
-        self.fitcontrolframe.setLayout(fitcontrollayout)
+            self.fitcontrollayout.addWidget(widget)
+        self.fitcontrolframe.setLayout(self.fitcontrollayout)
 
         # putting it all together: Setup the main layout
         mainlayout = QtWidgets.QHBoxLayout(self._main)
         splitter = QtWidgets.QSplitter(QtCore.Qt.Horizontal)
         splitter.addWidget(self.plotwidget)
         splitter.addWidget(self.fitcontrolframe)
         mainlayout.addWidget(splitter)
@@ -143,28 +150,41 @@
         try:
             self.modelview.read_values()
         except ValueError:
             self.showdialog(
                 "Not a valid input initial parameter values", "critical"
             )
             return None
-
+        print(self.plotwidget.selected_curve)
+        try:
+            selected_line = next(
+                x
+                for x in self.plotwidget.canvas.ax1.get_lines()
+                if x.get_label() == self.plotwidget.selected_curve
+            )
+            print(selected_line)
+            (current_x, current_y) = selected_line.get_data()
+            self.fitter.change_data(current_x, current_y, None, None)
+            # print("after change", self.fitter.data)
+        except:
+            self.showdialog("Can't find plot", "critical")
         # update fitrange
         self.plotwidget.canvas.get_range()
 
         # show warning on xerror data
         if (self.fitter.data.xe is not None) and self.xerrorwarning:
             self.showdialog("The error in x is ignored in the fit!", "warning")
             self.xerrorwarning = False
 
         # perform the fit
         with warnings.catch_warnings():
             warnings.simplefilter(
                 "error", OptimizeWarning
             )  # make sure the OptimizeWarning is raised as an exception
+
             try:
                 fitpars, fitcov, result = self.fitter.fit()
             except (ValueError, RuntimeError, OptimizeWarning):
                 self.showdialog(str(sys.exc_info()[1]), "critical")
 
             else:
                 """
@@ -192,14 +212,47 @@
             n = par.name
             v = par.value
             e = par.sigma
             f = par.fixed
             text = text + "\n" + value_to_string(n, v, e, f)
         return text
 
+    def refresh(self, model, y):
+        """
+        retrieves data from update signal, plotwidget.re_init(), and updates gui according to user input
+        called around line 64
+
+        """
+        if model == self.OG_model.func.__name__ or model is None:
+            self.fitter.change_model(self.OG_model.func, None, None)
+        else:
+            self.fitter.change_model(model, None, None)
+        self.modelview = ModelWidget(
+            self.fitter.model, self.fitter.get_weightoptions()
+        )
+        print("refresh", id(self.fitter))
+
+        # self.fitter.data = self.fitter._init_data(x, y, None, None)
+        # self.ylabel = "IM"
+        # self.fitcontrollayout = QtWidgets.QVBoxLayout()
+
+        child = self.fitcontrollayout.takeAt(0)
+        if child.widget():
+            child.widget().setParent(None)
+
+        for widget in (
+            self.modelview,
+            self.buttons,
+            self.reportview,
+            self.quitbutton,
+        ):
+            self.fitcontrollayout.addWidget(widget)
+
+        self.fitcontrolframe
+
 
 # add is_complex parameter
 def execute_gui(
     f,
     xdata,
     ydata,
     xerr,
@@ -379,14 +432,15 @@
         """
         Create error for test data
         """
         rng = np.random.default_rng()
         test_yerr = 0.2 * np.ones_like(xdata)
         y_noise = test_yerr * rng.normal(size=xdata.size)
         ydata = y + y_noise
+        ydata = np.asarray(ydata)
 
     """
     gonna have to add sigma to this and other places
     """
     # Here so that complex bool passes through to widgets
     if dlg.is_complex:
         kwargs["complex"] = True
@@ -400,11 +454,12 @@
         p0,
         absolute_sigma,
         jac,
         dlg.is_complex,
         **kwargs,
     )
 
+    # print("original", afitter.data)
     MyApplication = MainWindow(afitter, xlabel, ylabel, **kwargs)
     MyApplication.show()
     app.exec_()
     return MyApplication.get_output()
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/_settings.py` & `complex-curve-fit-gui-1.0.9/curvefitgui/_settings.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/_tools.py` & `complex-curve-fit-gui-1.0.9/curvefitgui/_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
 from dataclasses import dataclass, field
 from typing import Any, List
-
+import copy
 import numpy as np
 from lmfit import Model
 from scipy import stats
 from scipy.optimize import OptimizeWarning, curve_fit
 
+
 from ._settings import settings
 
 
 @dataclass
 class FitParameter:
     """
     stores a fitparameter
@@ -25,15 +26,14 @@
 @dataclass
 class FitModel:
     """
     stores the model
     """
 
     func: Any
-    jac: Any
     weight: str
     # lmfit_model: Model
     # lmfit_parameters: Any
     fitpars: List[FitParameter]
     description: str = ""
 
     def __post_init__(self) -> None:
@@ -105,24 +105,25 @@
         jac,
         is_complex,
         **kwargs,
     ):
 
         self.kwargs = kwargs
         self.data = self._init_data(xdata, ydata, xerr, yerr)
-        self.model = self._init_model(func, p0, absolute_sigma, jac)
+        self.model = self._init_model(func, p0, absolute_sigma)
         # Model Result from lmfit
         self.model_result = None
         self.fit_is_valid = False  # becomes True a a valid fit is computed
         self.mean_squared_error = None
         self.fitreport = {}
         self.is_complex = is_complex
         self.method = "leastsq"
         if "method" in kwargs:
             self.method = kwargs["method"]
+        self.orig_model = copy.deepcopy(self.model)
 
     def _init_data(self, x, y, xe, ye):
 
         # validate data
         for var in [x, y]:
             if type(var) is not np.ndarray:
                 raise Exception("data should have type numpy array")
@@ -140,15 +141,15 @@
             if type(xe) is not np.ndarray:
                 raise Exception("data should have type numpy array")
             if len(xe) != len(x):
                 raise Exception("xerr and xdata should be of equal length")
 
         return FitData(x, y, xe, ye)
 
-    def _init_model(self, func, p0, absolute_sigma, jac):
+    def _init_model(self, func, p0, absolute_sigma):
         # validate function
         if not callable(func):
             raise Exception("Not a valid fit function")
 
         # determine fitparameters from function
         __args = inspect.signature(func).parameters
         args = [arg.name for arg in __args.values()]
@@ -173,15 +174,15 @@
 
         # create and return the FitModel class
         if func.__doc__ is None:
             description = "no info on model"
         else:
             description = strip_leading_spaces(func.__doc__)
 
-        afitmodel = FitModel(func, jac, weight, fitpars, description)
+        afitmodel = FitModel(func, weight, fitpars, description)
         return afitmodel
 
     def fit(self):
         """
         performs the fit
         """
         # prepare model and data p0 are user guesses and pf is whether the guess is fixed or not
@@ -211,21 +212,21 @@
             x,
             y,
             sigma=ye,
             p0=p0,
             pF=pF,
             method=self.method,
             absolute_sigma=absolute_sigma,
-            jac=self.model.jac,
         )
         # lmfit model result
         self.model_result = result
 
         # process results
         self.fit_is_valid = True
+        print("cov", pcov)
         stderrors = np.sqrt(np.diag(pcov))
         for fitpar, value, stderr in zip(self.model.fitpars, popt, stderrors):
             fitpar.value = value
             fitpar.sigma = stderr
 
         self.mean_squared_error = sum(((y - self.model.evaluate(x)) / ye) ** 2)
 
@@ -311,17 +312,25 @@
     def get_weightoptions(self):
         if self.data.ye is not None:
             return self.WEIGHTOPTIONS
         else:
             # no error data so only one option remains
             return self.WEIGHTOPTIONS[0:1]
 
+    def change_data(self, x, y, xe, ye):
+        self.data = self._init_data(x, y, xe, ye)
+        # print(self)
+
+    def change_model(self, func, p0, absolute_sigma):
+        self.model = self._init_model(func, p0, absolute_sigma)
+        # print(self)
+
 
 def curve_fit_wrapper(
-    model, *pargs, p0=None, pF=None, jac=None, method="leastsq", **kwargs
+    model, *pargs, p0=None, pF=None, method="slsqp", **kwargs
 ):
     """
     wrapper around the scipy curve_fit() function to allow parameters to be fixed
     same call signature as the curve_fit() function except for:
     pF : 1D numpy array of size n, with n the number of fitparameters of the function
     returns the popt and cov matrices just like the original curve_fit() function
     """
@@ -346,26 +355,14 @@
 
     # make a string defining the new function as a lambda expression and evaluate to function
     fit_func = eval(
         f"lambda {', '.join(newfunc_args)} : func({', '.join(orifunc_args)})",
         locals(),
     )
 
-    # make a string defining the new jacobian function (if specified) as a lambda expression and evaluate to function
-    if callable(jac):
-        indices = np.array(
-            [index for index, value in enumerate(pF) if value == False]
-        )
-        fit_jac = eval(
-            f"lambda {', '.join(newfunc_args)} : jac({', '.join(orifunc_args)})[:, indices]",
-            locals(),
-        )
-    else:
-        fit_jac = jac
-
     # populate a list of initial values for free fit-parameters
     p0_fit = np.array([p for p, fix in zip(p0, pF) if not fix])
 
     # peform the fit with the reduced function
     # popt, cov = curve_fit(fit_func, *pargs, p0=p0_fit, jac=fit_jac, **kwargs)
 
     """
@@ -382,18 +379,21 @@
     result = model.lmfit_model.fit(
         pargs[1],
         params,
         x=pargs[0],
         calc_covar=True,
         nan_policy="omit",
         method=method,
+        max_nfev=500,
     )
 
     popt = np.array(list(result.best_values.values()))
-    cov = result.covar
+    print("cov values", result.covar)
+    cov = np.array(result.covar)
+    print("cov values after arrayed", cov)
 
     # rebuild the popt and cov to include fixed parameters
     p0_fix = [p for p, fix in zip(p0, pF) if fix]  # values of fixed parameters
     id_fix = np.where(pF)[0]  # indices of fixed parameters
     """
     No longer needed when using lmfit model
     """
@@ -404,14 +404,15 @@
 
     # rebuild covariance matrix to include both fixed and optimized pars
     for id in id_fix:
         cov = np.insert(
             cov, id, 0, axis=1
         )  # add zero rows and columns for fixed par
         cov = np.insert(cov, id, 0, axis=0)
+
     # params here temporarily, in future move lmfit model to fitmodel so that params does not need to be returned here
     return popt, cov, result
 
 
 def value_to_string(name, value, error, fixed):
     def get_exponent(value):
         """returns the exponent as an int generated by the :.e format specifier"""
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/_widgets.py` & `complex-curve-fit-gui-1.0.9/curvefitgui/_widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # import required packges
+from typing import Callable
 import warnings
 from collections import defaultdict
 import io
+import string
+from sympy.solvers import solve
+from sympy import symbols
 
 warnings.filterwarnings("ignore")
 
 
 import matplotlib.patches as patches
 import numpy as np
 from lmfit import Model
@@ -117,93 +121,287 @@
             dragline.remove()
 
 
 class PlotWidget(QtWidgets.QWidget):
     """Qt widget to hold the matplotlib canvas and the tools for interacting with the plots"""
 
     resized = QtCore.pyqtSignal()  # emits when the widget is resized
+    re_init = QtCore.pyqtSignal(
+        "PyQt_PyObject", "PyQt_PyObject", "PyQt_PyObject"
+    )  # emits when plot is updated
 
     def __init__(self, fitter, xlabel, ylabel, **kwargs):
         QtWidgets.QWidget.__init__(self)
-
         self.setLayout(QtWidgets.QVBoxLayout())
         self.canvas = PlotCanvas(fitter, xlabel, ylabel, **kwargs)
         self.toolbar = NavigationToolbar(self.canvas, self)
-        self.toolbar.addSeparator()
-
-        """
-        Change Data Button
-        """
-        self.updateData = QtWidgets.QAction("Update Data")
-        self.updateData.setIconText("UPDATE DATA")
-        self.updateData.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
-        self.updateData.triggered.connect(self.update_data)
-
-        self.toolbar.addSeparator()
+        self.selected_curve = self.canvas.ax1.get_lines()[0].get_label()
+        self.selected_model = None
+        self.input_func = None
+
+        self.hideRes = QtWidgets.QAction("TOGGLE RESIDUAL")
+        self.hideRes.setIconText("TOGGLE RESIDUAL")
+        self.hideRes.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
+        self.hideRes.triggered.connect(self.toggle_residual_visibility)
+
+        self.switchData = QtWidgets.QAction("Switch Data")
+        self.switchData.setIconText("SWITCH DATA")
+        self.switchData.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
+        self.switchData.triggered.connect(self.switch_data)
 
         self.ACshowselector = QtWidgets.QAction("Activate/Clear RangeSelector")
         self.ACshowselector.setIconText("RANGE SELECTOR")
         self.ACshowselector.setFont(QtGui.QFont("Times", 12, QtGui.QFont.Bold))
         self.ACshowselector.triggered.connect(self._toggle_showselector)
+        self.toolbar.addAction(self.hideRes)
+
+        self.toolbar.addSeparator()
+
+        self.toolbar.addAction(self.switchData)
 
         self.toolbar.addSeparator()
 
-        self.toolbar.addAction(self.updateData)
         self.toolbar.addAction(self.ACshowselector)
 
         self.toolbar.addSeparator()
         self.layout().addWidget(self.toolbar)
         self.layout().addWidget(self.canvas)
 
         self.resized.connect(
             self.update_plot
         )  # update plot when window is resized to fit plot in window
 
+        def linear(x, a, b):
+            """
+            linear
+            function: ax + b
+            """
+
+            return a * x + b
+
+        def exp_decay(x, a, b, c):
+            """
+            exponential decay
+            function: a * exp(-x / b) + c
+            a : amplitude
+            b : rate
+            c : offset
+            """
+            return a * np.exp(-x / b) + c
+
+        def cosine_function(x, a, b, c, d):
+            """
+            y = a * cos(b * x + c) + d
+            """
+            return a * np.cos(b * x + c) + d
+
+        def decaying_oscillation(x, a, b, c, d, e):
+            """
+            y = a * exp(-x / b) * cos(c * x + d) + e
+            """
+            return a * np.exp(-x / b) * np.cos(c * x + d) + e
+
+        def decaying_oscillation2(x, a, b, c, d, e):
+            """
+            y = a * exp(-x / b)^2 * cos(c * x + d) + e
+            """
+            return a * (np.exp(-x / b) ** 2) * np.cos(c * x + d) + e
+
+        def euler(x, a):
+            """
+            Euler's
+            y = a * exp(i * x)
+            """
+            return a * (np.exp(1j * (x)))
+
+        def complex_function(x, a, b, c, d):
+            """
+            complex exp
+            y = a * exp(i * (b * w + c)) + d
+            """
+            return a * np.exp(1j * (b * x + c)) + d
+
+        self.function_map = {
+            "y = ax + b": linear,
+            "y = a * exp(-x / b) + c": exp_decay,
+            "y = a * cos(b*x + c) + d": cosine_function,
+            "y = a * exp(-x / b) * cos(c * x + d) + e": decaying_oscillation,
+            "y = a * exp(-x / b)^2 * cos(c * x + d) + e": decaying_oscillation2,
+            "y = a * exp(i * x)": euler,
+            "y = a * exp(i * (b * w + c)) + d": complex_function,
+        }
+
     def resizeEvent(self, event):
         self.resized.emit()
         return super(PlotWidget, self).resizeEvent(event)
 
     def update_plot(self):
         self.canvas.update_plot()
 
     def _toggle_showselector(self):
         self.canvas.toggle_rangeselector()
 
+    def toggle_residual_visibility(self):
+        if not self.canvas.ax2.get_visible():
+            self.canvas.ax1.set(xlabel=None)
+        else:
+            self.canvas.ax1.set_xlabel(
+                self.canvas.xlabel,
+                fontname=settings["TEXT_FONT"],
+                fontsize=settings["TEXT_SIZE"],
+            )
+        self.canvas.ax2.set_visible(not self.canvas.ax2.get_visible())
+        self.canvas.redraw()
+
     def update_data(self):
-        return
+        x = np.array([1, 2, 3])
+        y = np.array([4, 5, 6])
+        self.canvas.ax1.plot(
+            x,
+            y,
+            marker="o",
+            lw=0,
+            label="data2",
+        )
+        self.canvas.ax1.legend()
+        self.canvas.redraw()
+
+        # dialog = QtWidgets.QDialog()
+        # dialog.setWindowTitle("Update Data")
+        # layout = QtWidgets.QVBoxLayout()
+
+        # ind_layout = QtWidgets.QHBoxLayout()
+        # ind_label = QtWidgets.QLabel("Independent Values: ")
+        # self.independent_variable = QtWidgets.QLineEdit()
+        # ind_layout.addWidget(ind_label)
+        # ind_layout.addWidget(self.independent_variable)
+
+        # dep_layout = QtWidgets.QHBoxLayout()
+        # dep_label = QtWidgets.QLabel("Dependent Values: ")
+        # self.dependent_variable = QtWidgets.QLineEdit()
+        # dep_layout.addWidget(dep_label)
+        # dep_layout.addWidget(self.dependent_variable)
+
+        # button = QtWidgets.QPushButton("Update")
+        # # button.clicked.connect(self.re_init_plot)
+
+        # layout.addLayout(ind_layout)
+        # layout.addLayout(dep_layout)
+        # layout.addWidget(button)
+
+        # button.clicked.connect(dialog.close)
+
+        # dialog.setLayout(layout)
+        # dialog.exec_()
+
+    def switch_data(self):
+        def get_selected_curve():
+            self.selected_curve = self.combobox.currentText()
+
+        def get_selected_model():
+            self.selected_model = self.model_combobox.currentText()
+
+        # print(self.canvas.ax1.get_lines()[1].get_label())
+        self.dialog = QtWidgets.QDialog()
+        self.dialog.setWindowTitle("Switch Data")
+        self.layout = QtWidgets.QVBoxLayout()
+
+        self.combobox = QtWidgets.QComboBox()
+        self.model_combobox = QtWidgets.QComboBox()
+        self.user_input = QtWidgets.QLineEdit()
+        self.button = QtWidgets.QPushButton("Select")
+        self.button.clicked.connect(get_selected_curve)
+        self.button.clicked.connect(get_selected_model)
+        self.button.clicked.connect(self.re_init_model)
+        # self.button.clicked.connect(self.create_callable)
+        self.button.clicked.connect(self.dialog.close)
+
+        for item in self.canvas.ax1.get_lines():
+            if item.get_label() != "fitted_curve":
+                self.combobox.addItem(item.get_label())
+
+        for item in self.canvas.ax1.get_lines():
+            if item.get_label() == "fitted_curve":
+                self.combobox.addItem(item.get_label())
+
+        self.model_combobox.addItem(
+            self.canvas.fitter.orig_model.func.__name__
+        )
+        for item in self.function_map:
+            self.model_combobox.addItem(item)
+
+        self.layout.addWidget(self.combobox)
+        self.layout.addWidget(self.model_combobox)
+        # self.layout.addWidget(self.user_input)
+        self.layout.addWidget(self.button)
+
+        self.dialog.setLayout(self.layout)
+        self.dialog.exec_()
+
+    def re_init_model(self, event):
+        new_model = None
+        if self.selected_model != self.canvas.fitter.orig_model.func.__name__:
+            new_model = self.function_map[self.selected_model]
+        if "i" in self.selected_model:
+            self.canvas.fitter.is_complex = True
+        else:
+            self.canvas.fitter.is_complex = False
+        self.re_init.emit(new_model, None, None)
+
+    def custom_user_function(self, *args):
+        n = len(args) - 1
+        symbol_str = "x" + ":" + str(n)
+        return solve(self.input_func, symbols(symbol_str))
+
+    def create_callable(self):
+        if len(self.user_input.text()) > 2:
+            new_args = ["x"]
+            self.input_func = self.user_input.text()
+            for c in self.input_func:
+                if c in string.ascii_uppercase:
+                    new_args.append(c)
+            self.function_map[self.input_func] = self.custom_user_function(
+                *new_args
+            )
+            self.model_combobox.addItem(self.input_func)
 
 
 class PlotCanvas(FigureCanvas):
     """class to hold a canvas with a matplotlib figure and two subplots for plotting data and residuals"""
 
     def __init__(self, fitter, xlabel, ylabel, **kwargs):
         self.fitter = fitter
+        self.xlabel = xlabel
         self.data = fitter.data  # contains the x, y and error data
         self.fitline = None  # contains the fitline if available
         self.residuals = None  # contains the residuals if available
         self.complex_residuals = None
         self.initial_guess_line = None
         self.kwargs = kwargs
+        self.additional_data = None
         self.fitline_kwargs = defaultdict(str)
         self.complex = (
             False if "complex" not in self.kwargs else self.kwargs["complex"]
         )
+        # print(id(self.fitter))
 
         # Get Axis titles
         self.ax1_title = (
             self.kwargs["title"] if "title" in self.kwargs else "Data"
         )
         # delete from kwargs to remove matplotlib error
         if "title" in self.kwargs:
             del self.kwargs["title"]
         if "method" in self.kwargs:
             del self.kwargs["method"]
         if "complex" in self.kwargs:
             del self.kwargs["complex"]
-
+        if "add" in self.kwargs:
+            self.additional_data = self.kwargs["add"]
+            del self.kwargs["add"]
         # Separate Fitline kwargs from data kwargs, at this point kwargs and self.kwargs are same thing
         if "fitline_color" in self.kwargs:
             self.fitline_kwargs["color"] = kwargs["fitline_color"]
             del kwargs["fitline_color"]
         if "fitline_linestyle" in self.kwargs:
             self.fitline_kwargs["linestyle"] = kwargs["fitline_linestyle"]
             del kwargs["fitline_linestyle"]
@@ -278,15 +476,15 @@
             **self.kwargs,
         )
         (self.fitted_line,) = self.ax1.plot([], [], **self.fitline_kwargs)
         (self.residual_line,) = self.ax2.plot(
             [], [], color="k", marker=".", lw=1
         )
         self.zero_res = None  # holder for a dashed hline to indicate zero in the residual plot
-
+        self.plot_additional_data()
         # create legend
         self.ax1.legend(
             loc="best",
             fancybox=True,
             framealpha=0.5,
             prop={
                 "family": settings["TEXT_FONT"],
@@ -311,19 +509,19 @@
         """
         self.data.y should be complex still at this point put a print line to check,
         but set_data most likely casts to real so at this point,
         
         """
         # populate plotlines if not complex data since different plot interpretation needed for complex values (the clear circles)
         if not self.fitter.is_complex:
-            self.data_line.set_data(self.data.x, self.data.y)
+            self.data_line.set_data(self.fitter.data.x, self.fitter.data.y)
         else:
             self.data_line.remove()
             (self.data_line,) = self.plot_complex(
-                self.data.y, "o", **self.kwargs
+                self.fitter.data.y, "o", **self.kwargs
             )
             self.ax1.legend()
 
         # create errorbars if required
         if self.data.ye is not None:
             self.yerrobar = self.ax1.errorbar(
                 self.data.x,
@@ -393,19 +591,23 @@
     def disable_results_box(self):
         self.result_box.set_visible(False)
 
     def toggle_rangeselector(self):
         if self.range_selector is None:
             if self.complex:
                 self.range_selector = RangeSelector(
-                    self.ax1, np.min(self.data.y), np.max(self.data.y)
+                    self.ax1,
+                    np.min(self.fitter.data.y),
+                    np.max(self.fitter.data.y),
                 )
             else:
                 self.range_selector = RangeSelector(
-                    self.ax1, np.min(self.data.x), np.max(self.data.x)
+                    self.ax1,
+                    np.min(self.fitter.data.x),
+                    np.max(self.fitter.data.x),
                 )
             self.redraw()
         else:
             self.range_selector.remove()
             self.range_selector = None
             self.redraw()
 
@@ -426,17 +628,17 @@
                 )
                 self.ax1.legend()
         else:
             self.fitline = fitline
 
     def get_range(self):
         if self.range_selector is None:
-            self.data.set_mask(-np.inf, np.inf)
+            self.fitter.data.set_mask(-np.inf, np.inf)
         else:
-            self.data.set_mask(*self.range_selector.get_range())
+            self.fitter.data.set_mask(*self.range_selector.get_range())
 
     def plot_complex(self, data, *args, **kwargs):
         """
         convenience function for plotting complex quantities
         """
         return self.ax1.plot(data.real, data.imag, *args, **kwargs)
 
@@ -446,14 +648,15 @@
             fitline_kwargs["color"] = kwargs["fitline_color"]
         return fitline_kwargs
 
     def update_plot(self):
         # update the residuals and/or fitline if present
 
         if self.fitter.model_result and self.fitter.is_complex:
+            # print(id(self.fitter))
             fit_s21 = self.fitter.model_result.eval(
                 params=self.fitter.model_result.params, x=self.fitter.data.x
             )
             # clear previous fit line
             # if self.data_line:
             #     self.data_line.remove()
             if self.fitted_line:
@@ -482,33 +685,35 @@
             if self.residuals is not None:
                 # if the zero residual line is not yet created, do so
                 if self.zero_res is None:
                     self.ax2.axhline(y=0, linestyle="--", color="black")
 
                 # sort data if required
                 if settings["SORT_RESIDUALS"]:
-                    order = np.argsort(self.data.x)
+                    order = np.argsort(self.fitter.data.x)
                 else:
-                    order = np.arange(0, len(self.data.x))
+                    order = np.arange(0, len(self.fitter.data.x))
                 # print("self.data.x", self.data.x, type(self.data.x))
                 # print("self.residuals", self.residuals, type(self.residuals))
                 # print("order slice", order[: len(self.residuals)], type(order))
                 # print("len of mask", len(self.data.mask), type(self.data.mask))
                 # print("self mask", self.data.mask)
 
                 """
                 Make a copy of data.x
                 iterate thru mask
                 if data.mask[i] is false then delete data.x[i] in the copy
                 use that copy in the residual line set data.
                 """
                 data_copy = np.array([])
-                for i in range(len(self.data.x)):
-                    if self.data.mask[i] == True:
-                        data_copy = np.append(data_copy, [self.data.x[i]])
+                for i in range(len(self.fitter.data.x)):
+                    if self.fitter.data.mask[i] == True:
+                        data_copy = np.append(
+                            data_copy, [self.fitter.data.x[i]]
+                        )
                 self.residual_line.set_data(
                     data_copy[order[: len(self.residuals)]],
                     self.residuals[order[: len(self.residuals)]],
                 )
 
                 # self.residual_line.set_data(
                 #     self.data.x[order],
@@ -527,14 +732,21 @@
         # make the min and max yscale limits of the residual plot equal
         ymax = max(np.abs(self.ax2.get_ylim()))
         self.ax2.set_ylim(-ymax, ymax)
 
         # draw the plot
         self.redraw()
 
+    def plot_additional_data(self):
+        if self.additional_data:
+            for item in self.additional_data:
+                self.ax1.plot(
+                    item[0], item[1], label=item[2], marker="o", lw=0
+                )
+
     def redraw(self):
         # self.fig.canvas.draw()
         self.draw()
 
 
 class ParamWidget(QtWidgets.QWidget):
     """Qt widget to show and change a fitparameter"""
```

### Comparing `complex-curve-fit-gui-1.0.8/curvefitgui/config.txt` & `complex-curve-fit-gui-1.0.9/curvefitgui/config.txt`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/arrows_scr.png` & `complex-curve-fit-gui-1.0.9/images/arrows_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/customize_scr.png` & `complex-curve-fit-gui-1.0.9/images/customize_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/home_scr.png` & `complex-curve-fit-gui-1.0.9/images/home_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/model_scr.png` & `complex-curve-fit-gui-1.0.9/images/model_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/pan_zoom_scr.png` & `complex-curve-fit-gui-1.0.9/images/pan_zoom_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/range_selector_scr.png` & `complex-curve-fit-gui-1.0.9/images/range_selector_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/images/toolbar_scr.png` & `complex-curve-fit-gui-1.0.9/images/toolbar_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.8/setup.py` & `complex-curve-fit-gui-1.0.9/setup.py`

 * *Files 2% similar despite different names*

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

