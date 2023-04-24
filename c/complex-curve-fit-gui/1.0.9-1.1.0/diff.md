# Comparing `tmp/complex-curve-fit-gui-1.0.9.tar.gz` & `tmp/complex_curve_fit_gui-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex-curve-fit-gui-1.0.9.tar", last modified: Mon Apr 24 03:28:06 2023, max compression
+gzip compressed data, was "complex_curve_fit_gui-1.1.0.tar", last modified: Mon Apr 24 03:40:28 2023, max compression
```

## Comparing `complex-curve-fit-gui-1.0.9.tar` & `complex_curve_fit_gui-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.484715 complex-curve-fit-gui-1.0.9/
--rw-r--r--   0 kojo       (501) staff       (20)     8196 2023-03-24 01:24:42.000000 complex-curve-fit-gui-1.0.9/.DS_Store
--rw-r--r--   0 kojo       (501) staff       (20)       31 2023-01-24 05:50:18.000000 complex-curve-fit-gui-1.0.9/.gitignore
--rw-rw-rw-   0 kojo       (501) staff       (20)       30 2021-07-05 10:22:07.000000 complex-curve-fit-gui-1.0.9/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:28:06.484874 complex-curve-fit-gui-1.0.9/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     8826 2023-04-14 18:42:27.000000 complex-curve-fit-gui-1.0.9/README.md
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.465648 complex-curve-fit-gui-1.0.9/__pycache__/
--rw-r--r--   0 kojo       (501) staff       (20)     1275 2023-01-31 04:10:58.000000 complex-curve-fit-gui-1.0.9/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    12574 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.9/__pycache__/tools.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      159 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.9/__pycache__/version.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    14087 2023-01-31 04:11:28.000000 complex-curve-fit-gui-1.0.9/__pycache__/widgets.cpython-39.pyc
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.466196 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     1298 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)       12 2023-04-24 03:28:06.000000 complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)     1001 2023-04-24 03:20:08.000000 complex-curve-fit-gui-1.0.9/curve.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.468369 complex-curve-fit-gui-1.0.9/curvefitgui/
--rw-r--r--   0 kojo       (501) staff       (20)     6148 2023-03-24 01:24:37.000000 complex-curve-fit-gui-1.0.9/curvefitgui/.DS_Store
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__init__.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.470770 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/
--rw-r--r--   0 kojo       (501) staff       (20)      424 2023-02-10 20:02:50.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      341 2023-01-31 03:15:43.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     7837 2023-02-23 16:53:13.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     6506 2023-03-31 04:21:23.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    18255 2023-03-02 19:00:48.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    11089 2023-04-22 02:23:13.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     2547 2023-02-10 20:02:50.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-311.pyc
--rw-r--r--   0 kojo       (501) staff       (20)     1280 2023-01-31 03:15:43.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    14114 2023-04-24 03:20:12.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_tools.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)      171 2023-03-31 04:42:55.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_version.cpython-39.pyc
--rw-r--r--   0 kojo       (501) staff       (20)    23105 2023-04-22 02:23:13.000000 complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_widgets.cpython-39.pyc
--rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-03-31 04:21:21.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    15523 2023-04-22 02:23:11.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16582 2023-04-22 02:34:16.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-24 03:27:55.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    30979 2023-04-22 02:21:36.000000 complex-curve-fit-gui-1.0.9/curvefitgui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex-curve-fit-gui-1.0.9/curvefitgui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:28:06.483167 complex-curve-fit-gui-1.0.9/images/
--rw-r--r--   0 kojo       (501) staff       (20)   588681 2023-03-24 01:20:24.000000 complex-curve-fit-gui-1.0.9/images/arrows_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585322 2023-03-24 01:17:35.000000 complex-curve-fit-gui-1.0.9/images/customize_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585544 2023-03-24 01:22:29.000000 complex-curve-fit-gui-1.0.9/images/home_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   589105 2023-03-24 01:13:01.000000 complex-curve-fit-gui-1.0.9/images/model_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)  1934108 2023-03-24 01:21:22.000000 complex-curve-fit-gui-1.0.9/images/pan_zoom_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585291 2023-03-24 01:16:21.000000 complex-curve-fit-gui-1.0.9/images/range_selector_scr.png
--rw-r--r--   0 kojo       (501) staff       (20)   585414 2023-03-24 01:14:53.000000 complex-curve-fit-gui-1.0.9/images/toolbar_scr.png
--rw-rw-rw-   0 kojo       (501) staff       (20)       38 2023-04-24 03:28:06.485283 complex-curve-fit-gui-1.0.9/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1213 2023-04-24 03:20:55.000000 complex-curve-fit-gui-1.0.9/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.592375 complex_curve_fit_gui-1.1.0/
+-rw-r--r--   0 kojo       (501) staff       (20)     8196 2023-04-24 03:28:58.000000 complex_curve_fit_gui-1.1.0/.DS_Store
+-rw-r--r--   0 kojo       (501) staff       (20)       31 2023-01-24 05:50:18.000000 complex_curve_fit_gui-1.1.0/.gitignore
+-rw-rw-rw-   0 kojo       (501) staff       (20)       30 2021-07-05 10:22:07.000000 complex_curve_fit_gui-1.1.0/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:40:28.592548 complex_curve_fit_gui-1.1.0/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     8826 2023-04-14 18:42:27.000000 complex_curve_fit_gui-1.1.0/README.md
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.570248 complex_curve_fit_gui-1.1.0/__pycache__/
+-rw-r--r--   0 kojo       (501) staff       (20)     1275 2023-01-31 04:10:58.000000 complex_curve_fit_gui-1.1.0/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    12574 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.0/__pycache__/tools.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      159 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.0/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    14087 2023-01-31 04:11:28.000000 complex_curve_fit_gui-1.1.0/__pycache__/widgets.cpython-39.pyc
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.570909 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)     9268 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     1298 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 03:40:28.000000 complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)     1001 2023-04-24 03:20:08.000000 complex_curve_fit_gui-1.1.0/curve.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.573342 complex_curve_fit_gui-1.1.0/curvefitgui/
+-rw-r--r--   0 kojo       (501) staff       (20)     6148 2023-03-24 01:24:37.000000 complex_curve_fit_gui-1.1.0/curvefitgui/.DS_Store
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__init__.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.577060 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/
+-rw-r--r--   0 kojo       (501) staff       (20)      424 2023-02-10 20:02:50.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      341 2023-01-31 03:15:43.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     7837 2023-02-23 16:53:13.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     6506 2023-03-31 04:21:23.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    18255 2023-03-02 19:00:48.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    11089 2023-04-22 02:23:13.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     2547 2023-02-10 20:02:50.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-311.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)     1280 2023-01-31 03:15:43.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    14114 2023-04-24 03:20:12.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_tools.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)      171 2023-03-31 04:42:55.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_version.cpython-39.pyc
+-rw-r--r--   0 kojo       (501) staff       (20)    23105 2023-04-22 02:23:13.000000 complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_widgets.cpython-39.pyc
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7183 2023-03-31 04:21:21.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15523 2023-04-22 02:23:11.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16582 2023-04-22 02:34:16.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-24 03:39:28.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    30979 2023-04-22 02:21:36.000000 complex_curve_fit_gui-1.1.0/curvefitgui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.0/curvefitgui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-24 03:40:28.590844 complex_curve_fit_gui-1.1.0/images/
+-rw-r--r--   0 kojo       (501) staff       (20)   588681 2023-03-24 01:20:24.000000 complex_curve_fit_gui-1.1.0/images/arrows_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585322 2023-03-24 01:17:35.000000 complex_curve_fit_gui-1.1.0/images/customize_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585544 2023-03-24 01:22:29.000000 complex_curve_fit_gui-1.1.0/images/home_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   589105 2023-03-24 01:13:01.000000 complex_curve_fit_gui-1.1.0/images/model_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)  1934108 2023-03-24 01:21:22.000000 complex_curve_fit_gui-1.1.0/images/pan_zoom_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585291 2023-03-24 01:16:21.000000 complex_curve_fit_gui-1.1.0/images/range_selector_scr.png
+-rw-r--r--   0 kojo       (501) staff       (20)   585414 2023-03-24 01:14:53.000000 complex_curve_fit_gui-1.1.0/images/toolbar_scr.png
+-rw-rw-rw-   0 kojo       (501) staff       (20)       38 2023-04-24 03:40:28.593015 complex_curve_fit_gui-1.1.0/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1226 2023-04-24 03:39:11.000000 complex_curve_fit_gui-1.1.0/setup.py
```

### Comparing `complex-curve-fit-gui-1.0.9/.DS_Store` & `complex_curve_fit_gui-1.1.0/.DS_Store`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0022  ..............."
+00000040: 0000 0000 0000 0002 0000 0000 0000 001e  ................
 00000050: 0000 0001 0000 1000 6c67 3153 636f 6d70  ........lg1Scomp
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,15 +250,15 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0022 0000 0004  ..........."....
+00001000: 0000 0000 0000 0000 0000 001e 0000 0004  ................
 00001010: 002e 0067 0069 0074 6c67 3153 636f 6d70  ...g.i.tlg1Scomp
 00001020: 0000 0000 0004 523d 0000 0004 002e 0067  ......R=.......g
 00001030: 0069 0074 6d6f 4444 626c 6f62 0000 0008  .i.tmoDDblob....
 00001040: c108 55c5 dadd c441 0000 0004 002e 0067  ..U....A.......g
 00001050: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
 00001060: c108 55c5 dadd c441 0000 0004 002e 0067  ..U....A.......g
 00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
@@ -312,47 +312,47 @@
 00001370: 7500 696d 6f44 4462 6c6f 6200 0000 08e3  u.imoDDblob.....
 00001380: 0a0a 57da ddc4 4100 0000 0b00 6300 7500  ..W...A.....c.u.
 00001390: 7200 7600 6500 6600 6900 7400 6700 7500  r.v.e.f.i.t.g.u.
 000013a0: 696d 6f64 4462 6c6f 6200 0000 08e3 0a0a  imodDblob.......
 000013b0: 57da ddc4 4100 0000 0b00 6300 7500 7200  W...A.....c.u.r.
 000013c0: 7600 6500 6600 6900 7400 6700 7500 6970  v.e.f.i.t.g.u.ip
 000013d0: 6831 5363 6f6d 7000 0000 0000 0310 0000  h1Scomp.........
-000013e0: 0000 1400 6300 7500 7200 7600 6500 6600  ....c.u.r.v.e.f.
-000013f0: 6900 7400 6700 7500 6900 2e00 6500 6700  i.t.g.u.i...e.g.
-00001400: 6700 2d00 6900 6e00 6600 6f6c 6731 5363  g.-.i.n.f.olg1Sc
-00001410: 6f6d 7000 0000 0000 0016 2a00 0000 1400  omp.......*.....
-00001420: 6300 7500 7200 7600 6500 6600 6900 7400  c.u.r.v.e.f.i.t.
-00001430: 6700 7500 6900 2e00 6500 6700 6700 2d00  g.u.i...e.g.g.-.
-00001440: 6900 6e00 6600 6f6d 6f44 4462 6c6f 6200  i.n.f.omoDDblob.
-00001450: 0000 08c2 562d 0697 d8c4 4100 0000 1400  ....V-....A.....
-00001460: 6300 7500 7200 7600 6500 6600 6900 7400  c.u.r.v.e.f.i.t.
-00001470: 6700 7500 6900 2e00 6500 6700 6700 2d00  g.u.i...e.g.g.-.
-00001480: 6900 6e00 6600 6f6d 6f64 4462 6c6f 6200  i.n.f.omodDblob.
-00001490: 0000 08c2 562d 0697 d8c4 4100 0000 1400  ....V-....A.....
-000014a0: 6300 7500 7200 7600 6500 6600 6900 7400  c.u.r.v.e.f.i.t.
-000014b0: 6700 7500 6900 2e00 6500 6700 6700 2d00  g.u.i...e.g.g.-.
-000014c0: 6900 6e00 6600 6f70 6831 5363 6f6d 7000  i.n.f.oph1Scomp.
-000014d0: 0000 0000 0050 0000 0000 0400 6400 6900  .....P......d.i.
-000014e0: 7300 746c 6731 5363 6f6d 7000 0000 0000  s.tlg1Scomp.....
-000014f0: 00f1 4e00 0000 0400 6400 6900 7300 746d  ..N.....d.i.s.tm
-00001500: 6f44 4462 6c6f 6200 0000 08ec 87d2 c39a  oDDblob.........
-00001510: d8c4 4100 0000 0400 6400 6900 7300 746d  ..A.....d.i.s.tm
-00001520: 6f64 4462 6c6f 6200 0000 08ec 87d2 c39a  odDblob.........
-00001530: d8c4 4100 0000 0400 6400 6900 7300 7470  ..A.....d.i.s.tp
-00001540: 6831 5363 6f6d 7000 0000 0000 0100 0000  h1Scomp.........
-00001550: 0000 0600 6900 6d00 6100 6700 6500 7364  ....i.m.a.g.e.sd
-00001560: 7363 6c62 6f6f 6c01 0000 0006 0069 006d  sclbool......i.m
-00001570: 0061 0067 0065 0073 6c67 3153 636f 6d70  .a.g.e.slg1Scomp
-00001580: 0000 0000 0000 0000 0000 0006 0069 006d  .............i.m
-00001590: 0061 0067 0065 0073 6d6f 4444 626c 6f62  .a.g.e.smoDDblob
-000015a0: 0000 0008 aa74 d98f 99e6 c441 0000 0006  .....t.....A....
-000015b0: 0069 006d 0061 0067 0065 0073 6d6f 6444  .i.m.a.g.e.smodD
-000015c0: 626c 6f62 0000 0008 aa74 d98f 99e6 c441  blob.....t.....A
-000015d0: 0000 0006 0069 006d 0061 0067 0065 0073  .....i.m.a.g.e.s
-000015e0: 7068 3153 636f 6d70 0000 0000 0000 0000  ph1Scomp........
+000013e0: 0000 0400 6400 6900 7300 746c 6731 5363  ....d.i.s.tlg1Sc
+000013f0: 6f6d 7000 0000 0000 00f1 4e00 0000 0400  omp.......N.....
+00001400: 6400 6900 7300 746d 6f44 4462 6c6f 6200  d.i.s.tmoDDblob.
+00001410: 0000 08ec 87d2 c39a d8c4 4100 0000 0400  ..........A.....
+00001420: 6400 6900 7300 746d 6f64 4462 6c6f 6200  d.i.s.tmodDblob.
+00001430: 0000 08ec 87d2 c39a d8c4 4100 0000 0400  ..........A.....
+00001440: 6400 6900 7300 7470 6831 5363 6f6d 7000  d.i.s.tph1Scomp.
+00001450: 0000 0000 0100 0000 0000 0600 6900 6d00  ............i.m.
+00001460: 6100 6700 6500 7364 7363 6c62 6f6f 6c01  a.g.e.sdsclbool.
+00001470: 0000 0006 0069 006d 0061 0067 0065 0073  .....i.m.a.g.e.s
+00001480: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
+00001490: 0000 0006 0069 006d 0061 0067 0065 0073  .....i.m.a.g.e.s
+000014a0: 6d6f 4444 626c 6f62 0000 0008 aa74 d98f  moDDblob.....t..
+000014b0: 99e6 c441 0000 0006 0069 006d 0061 0067  ...A.....i.m.a.g
+000014c0: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
+000014d0: aa74 d98f 99e6 c441 0000 0006 0069 006d  .t.....A.....i.m
+000014e0: 0061 0067 0065 0073 7068 3153 636f 6d70  .a.g.e.sph1Scomp
+000014f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,30 +457,30 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0000 746d  .....@........tm
-00001d00: 6f44 4462 6c6f 6200 0000 08ec 87d2 c39a  oDDblob.........
-00001d10: d8c4 4100 0000 0400 6400 6900 7300 746d  ..A.....d.i.s.tm
-00001d20: 6f64 4462 6c6f 6200 0000 08ec 87d2 c39a  odDblob.........
-00001d30: d8c4 4100 0000 0400 6400 6900 7300 7470  ..A.....d.i.s.tp
-00001d40: 6831 5363 6f6d 7000 0000 0000 0100 0000  h1Scomp.........
-00001d50: 0000 0600 6900 6d00 6100 6700 6500 7364  ....i.m.a.g.e.sd
-00001d60: 7363 6c62 6f6f 6c01 0000 0006 0069 006d  sclbool......i.m
-00001d70: 0061 0067 0065 0073 6c67 3153 636f 6d70  .a.g.e.slg1Scomp
-00001d80: 0000 0000 0000 0000 0000 0006 0069 006d  .............i.m
-00001d90: 0061 0067 0065 0073 6d6f 4444 626c 6f62  .a.g.e.smoDDblob
-00001da0: 0000 0008 aa74 d98f 99e6 c441 0000 0006  .....t.....A....
-00001db0: 0069 006d 0061 0067 0065 0073 6d6f 6444  .i.m.a.g.e.smodD
-00001dc0: 626c 6f62 0000 0008 aa74 d98f 99e6 c441  blob.....t.....A
-00001dd0: 0000 0006 0069 006d 0061 0067 0065 0073  .....i.m.a.g.e.s
-00001de0: 7068 3153 636f 6d70 0000 0000 0000 0000  ph1Scomp........
+00001cf0: 0000 0000 0140 0000 0000 0000 0000 0000  .....@..........
+00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `complex-curve-fit-gui-1.0.9/PKG-INFO` & `complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.0.9
+Version: 1.1.0
 Summary: GUI for lmfit
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `complex-curve-fit-gui-1.0.9/README.md` & `complex_curve_fit_gui-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/__pycache__/settings.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/__pycache__/tools.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/__pycache__/tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/__pycache__/widgets.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/__pycache__/widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex_curve_fit_gui-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: complex-curve-fit-gui
-Version: 1.0.9
+Name: complex_curve_fit_gui
+Version: 1.1.0
 Summary: GUI for lmfit
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `complex-curve-fit-gui-1.0.9/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex_curve_fit_gui-1.1.0/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curve.py` & `complex_curve_fit_gui-1.1.0/curve.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/.DS_Store` & `complex_curve_fit_gui-1.1.0/curvefitgui/.DS_Store`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_curvefitgui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-311.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_gui.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_gui.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-311.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_settings.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_tools.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/__pycache__/_widgets.cpython-39.pyc` & `complex_curve_fit_gui-1.1.0/curvefitgui/__pycache__/_widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/_curvefitgui.py` & `complex_curve_fit_gui-1.1.0/curvefitgui/_curvefitgui.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/_gui.py` & `complex_curve_fit_gui-1.1.0/curvefitgui/_gui.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/_settings.py` & `complex_curve_fit_gui-1.1.0/curvefitgui/_settings.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/_tools.py` & `complex_curve_fit_gui-1.1.0/curvefitgui/_tools.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/_widgets.py` & `complex_curve_fit_gui-1.1.0/curvefitgui/_widgets.py`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/curvefitgui/config.txt` & `complex_curve_fit_gui-1.1.0/curvefitgui/config.txt`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/arrows_scr.png` & `complex_curve_fit_gui-1.1.0/images/arrows_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/customize_scr.png` & `complex_curve_fit_gui-1.1.0/images/customize_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/home_scr.png` & `complex_curve_fit_gui-1.1.0/images/home_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/model_scr.png` & `complex_curve_fit_gui-1.1.0/images/model_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/pan_zoom_scr.png` & `complex_curve_fit_gui-1.1.0/images/pan_zoom_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/range_selector_scr.png` & `complex_curve_fit_gui-1.1.0/images/range_selector_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/images/toolbar_scr.png` & `complex_curve_fit_gui-1.1.0/images/toolbar_scr.png`

 * *Files identical despite different names*

### Comparing `complex-curve-fit-gui-1.0.9/setup.py` & `complex_curve_fit_gui-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 exec(open("./curvefitgui/_version.py").read())
 
 # This call to setup() does all the work
 setup(
-    name="complex-curve-fit-gui",
+    name="complex_curve_fit_gui",
     version=__version__,
     description="GUI for lmfit",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/boakyeni/data-visualization-and-curve-fitting",
     author="Kojo Nimako",
     author_email="boakyeni@usc.edu",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7, <4",
-    packages=find_packages(),
+    packages=find_packages("curvefitgui"),
     include_package_data=True,
     package_data={
         "curvefitgui": ["config.txt"],
     },
     # conda
     # install_requires=["matplotlib", "numpy", "scipy", "pyqt", "qtpy"], # need to check versions
     # PyPi
```

