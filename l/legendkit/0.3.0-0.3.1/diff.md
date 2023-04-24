# Comparing `tmp/legendkit-0.3.0.tar.gz` & `tmp/legendkit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legendkit-0.3.0.tar", max compression
+gzip compressed data, was "legendkit-0.3.1.tar", max compression
```

## Comparing `legendkit-0.3.0.tar` & `legendkit-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      772 2023-03-18 08:07:51.299041 legendkit-0.3.0/README.md
--rw-r--r--   0        0        0      357 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/__init__.py
--rw-r--r--   0        0        0    23821 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/_colorart.py
--rw-r--r--   0        0        0     7040 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/_colorbar.py
--rw-r--r--   0        0        0     2897 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/_handlers.py
--rw-r--r--   0        0        0    20083 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/_legend.py
--rw-r--r--   0        0        0     2167 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/_locs.py
--rw-r--r--   0        0        0     2330 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/_register.py
--rw-r--r--   0        0        0     1394 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/handles.py
--rw-r--r--   0        0        0     5442 2023-03-18 08:07:51.311041 legendkit-0.3.0/legendkit/layout.py
--rw-r--r--   0        0        0      848 2023-03-18 08:07:51.311041 legendkit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1471 1970-01-01 00:00:00.000000 legendkit-0.3.0/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 legendkit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      772 2023-04-24 09:46:48.367401 legendkit-0.3.1/README.md
+-rw-r--r--   0        0        0      357 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/__init__.py
+-rw-r--r--   0        0        0    23821 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/_colorart.py
+-rw-r--r--   0        0        0     7040 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/_colorbar.py
+-rw-r--r--   0        0        0     2897 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/_handlers.py
+-rw-r--r--   0        0        0    20520 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/_legend.py
+-rw-r--r--   0        0        0     2167 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/_locs.py
+-rw-r--r--   0        0        0     2330 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/_register.py
+-rw-r--r--   0        0        0     1394 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/handles.py
+-rw-r--r--   0        0        0     5442 2023-04-24 09:46:48.379401 legendkit-0.3.1/legendkit/layout.py
+-rw-r--r--   0        0        0      848 2023-04-24 09:46:48.379401 legendkit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1471 1970-01-01 00:00:00.000000 legendkit-0.3.1/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 legendkit-0.3.1/PKG-INFO
```

### Comparing `legendkit-0.3.0/README.md` & `legendkit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/_colorart.py` & `legendkit-0.3.1/legendkit/_colorart.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/_colorbar.py` & `legendkit-0.3.1/legendkit/_colorbar.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/_handlers.py` & `legendkit-0.3.1/legendkit/_handlers.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/_legend.py` & `legendkit-0.3.1/legendkit/_legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import _api
-from matplotlib.axes import Axes
 from matplotlib.collections import Collection
 from matplotlib.colors import is_color_like
 from matplotlib.font_manager import FontProperties
 from matplotlib.legend import Legend
 from matplotlib.lines import Line2D
 from matplotlib.markers import MarkerStyle
 from matplotlib.offsetbox import VPacker, HPacker
@@ -471,14 +470,16 @@
         The color of the entry
     fmt : str, :class:`Formatter <matplotlib.ticker.Formatter>`
         The format or formatter to use for the labels.
     func : Callable, default: `lambda x: x`
         A function to calculate the labels.
     show_at : array-like, default: [.25, .5, .75, 1.]
         The percentile to show the sizes
+    spacing : {"percentile", "uniform"}, default: "percentile"
+        The spacing of the sizes
     handle : str or sizable handle
         You can use any markers in :module:matplotlib.markers
     handler_kw : mapping
         Use this to control the style of handler
     fill : bool, default: True
         If not filled, the color will draw on the edge.
     kwargs : mapping
@@ -517,14 +518,15 @@
                  ax=None,
                  labels=None,
                  array=None,
                  colors=None,
                  fmt=None,  # label
                  func=lambda x: x,  # label
                  show_at=None,
+                 spacing="percentile",
                  handle="circle",
                  handler_kw=None,
                  fill=True,
                  **kwargs
                  ):
 
         size_handles = []
@@ -551,17 +553,25 @@
         fmt.axis.set_view_interval(display_min, display_max)
         fmt.axis.set_data_interval(display_min, display_max)
 
         # decide on locator to use
         if show_at is None:
             show_at = np.array([.25, .5, .75, 1.])
         show_at = np.asarray(show_at)
-        ix = np.clip((show_at * len(sizes) - 1), 0, len(sizes) - 1).astype(int)
-        handle_sizes = sizes[ix]
-        handle_labels = array[ix]
+        if spacing == "percentile":
+            ix = np.clip((show_at * len(sizes) - 1), 0, len(sizes) - 1).astype(int)
+            handle_sizes = sizes[ix]
+            handle_labels = array[ix]
+        else:
+            amin = np.amin(array)
+            amax = np.amax(array)
+            smin = np.amin(sizes)
+            smax = np.amax(sizes)
+            handle_sizes = np.interp(show_at, [0, 1], [smin, smax])
+            handle_labels = np.interp(show_at, [0, 1], [amin, amax])
         handle_labels = func(handle_labels)
 
         num_entry = len(handle_labels)
         if colors is None:
             handle_colors = ['black' for _ in range(num_entry)]
         elif is_color_like(colors):
             handle_colors = [colors for _ in range(num_entry)]
```

### Comparing `legendkit-0.3.0/legendkit/_locs.py` & `legendkit-0.3.1/legendkit/_locs.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/_register.py` & `legendkit-0.3.1/legendkit/_register.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/handles.py` & `legendkit-0.3.1/legendkit/handles.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/legendkit/layout.py` & `legendkit-0.3.1/legendkit/layout.py`

 * *Files identical despite different names*

### Comparing `legendkit-0.3.0/pyproject.toml` & `legendkit-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "legendkit"
-version = "0.3.0"
+version = "0.3.1"
 description = "Legend creation and manipulation with ease for matplotlib"
 authors = ["Mr-Milk <yb97643@um.edu.mo>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Heatgraphy/legendkit"
 classifiers = [
       "License :: OSI Approved :: MIT License",
```

### Comparing `legendkit-0.3.0/setup.py` & `legendkit-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6,<4.0']
 
 setup_kwargs = {
     'name': 'legendkit',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Legend creation and manipulation with ease for matplotlib',
     'long_description': '<p align="center">\n<img src="https://raw.githubusercontent.com/Mr-Milk/legendkit/main/images/legendkit-project.svg">\n</p>\n\n[![Documentation Status](https://img.shields.io/readthedocs/legendkit?logo=readthedocs&logoColor=white&style=flat-square)](https://legendkit.readthedocs.io/en/stable)\n![pypi version](https://img.shields.io/pypi/v/legendkit?color=blue&logo=python&logoColor=white&style=flat-square)\n\nWhen you want to create or adjust the legend in matplotlib, things can get dirty. \nLegendkit may solve your headache.\n\n<img src="https://legendkit.readthedocs.io/en/latest/_images/cover.svg">\n\n## Features\n\n- Easy title placement and alignment\n- Easy colorbar with shape\n- Layout for multiple legends and colorbar*\n\n## Installation\n\n```shell\npip install legendkit\n```\n',
     'author': 'Mr-Milk',
     'author_email': 'yb97643@um.edu.mo',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Heatgraphy/legendkit',
```

### Comparing `legendkit-0.3.0/PKG-INFO` & `legendkit-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legendkit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Legend creation and manipulation with ease for matplotlib
 Home-page: https://github.com/Heatgraphy/legendkit
 License: MIT
 Author: Mr-Milk
 Author-email: yb97643@um.edu.mo
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
```

