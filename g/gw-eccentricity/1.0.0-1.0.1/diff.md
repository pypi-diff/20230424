# Comparing `tmp/gw_eccentricity-1.0.0.tar.gz` & `tmp/gw_eccentricity-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gw_eccentricity-1.0.0.tar", last modified: Thu Feb 23 15:41:48 2023, max compression
+gzip compressed data, was "dist/gw_eccentricity-1.0.1.tar", last modified: Mon Apr 24 13:20:50 2023, max compression
```

## Comparing `gw_eccentricity-1.0.0.tar` & `gw_eccentricity-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-02-23 15:41:48.154806 gw_eccentricity-1.0.0/
--rw-r--r--   0 vijay      (502) staff       (20)     5102 2023-02-23 15:41:48.154616 gw_eccentricity-1.0.0/PKG-INFO
--rw-r--r--   0 vijay      (502) staff       (20)     3612 2023-02-23 08:47:15.000000 gw_eccentricity-1.0.0/README.md
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-02-23 15:41:48.150520 gw_eccentricity-1.0.0/gw_eccentricity/
--rw-r--r--   0 vijay      (502) staff       (20)      435 2023-02-11 16:46:41.000000 gw_eccentricity-1.0.0/gw_eccentricity/__init__.py
--rw-r--r--   0 vijay      (502) staff       (20)     4505 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/gw_eccentricity/compare_methods.py
--rw-r--r--   0 vijay      (502) staff       (20)   139256 2023-02-23 08:47:15.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinition.py
--rw-r--r--   0 vijay      (502) staff       (20)     1884 2022-09-20 13:37:08.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingAmplitude.py
--rw-r--r--   0 vijay      (502) staff       (20)     2545 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
--rw-r--r--   0 vijay      (502) staff       (20)      810 2022-09-20 13:37:08.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingFrequency.py
--rw-r--r--   0 vijay      (502) staff       (20)    48055 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingFrequencyFits.py
--rw-r--r--   0 vijay      (502) staff       (20)     2184 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
--rw-r--r--   0 vijay      (502) staff       (20)     1294 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingResidualFrequency.py
--rw-r--r--   0 vijay      (502) staff       (20)     3211 2022-06-16 18:35:52.000000 gw_eccentricity-1.0.0/gw_eccentricity/group_nr_waveforms.py
--rw-r--r--   0 vijay      (502) staff       (20)    18160 2023-02-23 15:41:17.000000 gw_eccentricity-1.0.0/gw_eccentricity/gw_eccentricity.py
--rw-r--r--   0 vijay      (502) staff       (20)    49274 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.0/gw_eccentricity/load_data.py
--rw-r--r--   0 vijay      (502) staff       (20)     5823 2023-02-09 10:23:14.000000 gw_eccentricity-1.0.0/gw_eccentricity/plot_settings.py
--rw-r--r--   0 vijay      (502) staff       (20)     5299 2022-10-10 19:26:56.000000 gw_eccentricity-1.0.0/gw_eccentricity/truncate_waveform_by_flow.py
--rw-r--r--   0 vijay      (502) staff       (20)    12427 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.0/gw_eccentricity/utils.py
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-02-23 15:41:48.152239 gw_eccentricity-1.0.0/gw_eccentricity.egg-info/
--rw-r--r--   0 vijay      (502) staff       (20)     5102 2023-02-23 15:41:47.000000 gw_eccentricity-1.0.0/gw_eccentricity.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (502) staff       (20)      960 2023-02-23 15:41:47.000000 gw_eccentricity-1.0.0/gw_eccentricity.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (502) staff       (20)        1 2023-02-23 15:41:47.000000 gw_eccentricity-1.0.0/gw_eccentricity.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (502) staff       (20)       26 2023-02-23 15:41:47.000000 gw_eccentricity-1.0.0/gw_eccentricity.egg-info/requires.txt
--rw-r--r--   0 vijay      (502) staff       (20)       16 2023-02-23 15:41:47.000000 gw_eccentricity-1.0.0/gw_eccentricity.egg-info/top_level.txt
--rw-r--r--   0 vijay      (502) staff       (20)       38 2023-02-23 15:41:48.154862 gw_eccentricity-1.0.0/setup.cfg
--rw-r--r--   0 vijay      (502) staff       (20)     1393 2023-02-22 10:38:49.000000 gw_eccentricity-1.0.0/setup.py
-drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-02-23 15:41:48.154263 gw_eccentricity-1.0.0/test/
--rw-r--r--   0 vijay      (502) staff       (20)     1524 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.0/test/test_example_notebooks.py
--rw-r--r--   0 vijay      (502) staff       (20)     2275 2022-11-24 23:10:42.000000 gw_eccentricity-1.0.0/test/test_interface.py
--rw-r--r--   0 vijay      (502) staff       (20)     9141 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/test/test_mks_vs_dimless_units.py
--rw-r--r--   0 vijay      (502) staff       (20)     2871 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/test/test_regression.py
--rw-r--r--   0 vijay      (502) staff       (20)     2498 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.0/test/test_time_convention.py
+drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.558048 gw_eccentricity-1.0.1/
+-rw-r--r--   0 vijay      (502) staff       (20)     5128 2023-04-24 13:20:50.557856 gw_eccentricity-1.0.1/PKG-INFO
+-rw-r--r--   0 vijay      (502) staff       (20)     3638 2023-02-24 09:47:49.000000 gw_eccentricity-1.0.1/README.md
+drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.554904 gw_eccentricity-1.0.1/gw_eccentricity/
+-rw-r--r--   0 vijay      (502) staff       (20)      435 2023-02-11 16:46:41.000000 gw_eccentricity-1.0.1/gw_eccentricity/__init__.py
+-rw-r--r--   0 vijay      (502) staff       (20)     4505 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/compare_methods.py
+-rw-r--r--   0 vijay      (502) staff       (20)   139591 2023-04-24 13:07:54.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinition.py
+-rw-r--r--   0 vijay      (502) staff       (20)     1884 2022-09-20 13:37:08.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitude.py
+-rw-r--r--   0 vijay      (502) staff       (20)     2545 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
+-rw-r--r--   0 vijay      (502) staff       (20)      810 2022-09-20 13:37:08.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequency.py
+-rw-r--r--   0 vijay      (502) staff       (20)    48055 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequencyFits.py
+-rw-r--r--   0 vijay      (502) staff       (20)     2184 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
+-rw-r--r--   0 vijay      (502) staff       (20)     1294 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualFrequency.py
+-rw-r--r--   0 vijay      (502) staff       (20)     3211 2022-06-16 18:35:52.000000 gw_eccentricity-1.0.1/gw_eccentricity/group_nr_waveforms.py
+-rw-r--r--   0 vijay      (502) staff       (20)    18160 2023-04-24 13:18:54.000000 gw_eccentricity-1.0.1/gw_eccentricity/gw_eccentricity.py
+-rw-r--r--   0 vijay      (502) staff       (20)    49274 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.1/gw_eccentricity/load_data.py
+-rw-r--r--   0 vijay      (502) staff       (20)     5846 2023-04-24 13:07:54.000000 gw_eccentricity-1.0.1/gw_eccentricity/plot_settings.py
+-rw-r--r--   0 vijay      (502) staff       (20)     5299 2022-10-10 19:26:56.000000 gw_eccentricity-1.0.1/gw_eccentricity/truncate_waveform_by_flow.py
+-rw-r--r--   0 vijay      (502) staff       (20)    12427 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.1/gw_eccentricity/utils.py
+drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.556328 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/
+-rw-r--r--   0 vijay      (502) staff       (20)     5128 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (502) staff       (20)      960 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (502) staff       (20)        1 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (502) staff       (20)       26 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/requires.txt
+-rw-r--r--   0 vijay      (502) staff       (20)       16 2023-04-24 13:20:50.000000 gw_eccentricity-1.0.1/gw_eccentricity.egg-info/top_level.txt
+-rw-r--r--   0 vijay      (502) staff       (20)       38 2023-04-24 13:20:50.558096 gw_eccentricity-1.0.1/setup.cfg
+-rw-r--r--   0 vijay      (502) staff       (20)     1393 2023-02-22 10:38:49.000000 gw_eccentricity-1.0.1/setup.py
+drwxr-xr-x   0 vijay      (502) staff       (20)        0 2023-04-24 13:20:50.557622 gw_eccentricity-1.0.1/test/
+-rw-r--r--   0 vijay      (502) staff       (20)     1524 2023-02-22 10:21:11.000000 gw_eccentricity-1.0.1/test/test_example_notebooks.py
+-rw-r--r--   0 vijay      (502) staff       (20)     2275 2022-11-24 23:10:42.000000 gw_eccentricity-1.0.1/test/test_interface.py
+-rw-r--r--   0 vijay      (502) staff       (20)     9141 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/test/test_mks_vs_dimless_units.py
+-rw-r--r--   0 vijay      (502) staff       (20)     2871 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/test/test_regression.py
+-rw-r--r--   0 vijay      (502) staff       (20)     2498 2023-02-06 07:18:30.000000 gw_eccentricity-1.0.1/test/test_time_convention.py
```

### Comparing `gw_eccentricity-1.0.0/PKG-INFO` & `gw_eccentricity-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gw_eccentricity
-Version: 1.0.0
+Version: 1.0.1
 Summary: Defining eccentricity for gravitational wave astronomy.
 Home-page: https://github.com/vijayvarma392/gw_eccentricity
 Author: Md Arif Shaikh, Vijay Varma, Harald Pfeiffer
 Author-email: arifshaikh.astro@gmail.com, vijay.varma392@gmail.com
 License: UNKNOWN
 Description: <h1> <img src="https://raw.githubusercontent.com/vijayvarma392/gw_eccentricity/main/data/hreal.png"></h1>
         
         <h3 align="center"> Defining eccentricity for gravitational wave astronomy </h4>
         
         <div align="center">
         
         [![github](https://img.shields.io/badge/GitHub-gw_eccentricity-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity)
-        [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg)](https://pypi.org/project/gw_eccentricity)
+        [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg?kill_cache=1)](https://pypi.org/project/gw_eccentricity)
         [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity/blob/main/LICENSE)
-        [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
+        [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg?kill_cache=1)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
         
         </div>
         
         # About
         
         **gw_eccentricity** provides methods to measure eccentricity and mean anomaly
         from gravitational waveforms.
```

### Comparing `gw_eccentricity-1.0.0/README.md` & `gw_eccentricity-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <h1> <img src="https://raw.githubusercontent.com/vijayvarma392/gw_eccentricity/main/data/hreal.png"></h1>
 
 <h3 align="center"> Defining eccentricity for gravitational wave astronomy </h4>
 
 <div align="center">
 
 [![github](https://img.shields.io/badge/GitHub-gw_eccentricity-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity)
-[![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg)](https://pypi.org/project/gw_eccentricity)
+[![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg?kill_cache=1)](https://pypi.org/project/gw_eccentricity)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity/blob/main/LICENSE)
-[![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
+[![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg?kill_cache=1)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
 
 </div>
 
 # About
 
 **gw_eccentricity** provides methods to measure eccentricity and mean anomaly
 from gravitational waveforms.
```

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/compare_methods.py` & `gw_eccentricity-1.0.1/gw_eccentricity/compare_methods.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinition.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1918,15 +1918,15 @@
                                 "waveform has insufficient identifiable "
                                 "pericenters/apocenters.")
         return fref_out
 
     def make_diagnostic_plots(
             self,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style=None,
             use_fancy_settings=True,
             twocol=False,
             **kwargs):
         """Make diagnostic plots for the eccDefinition method.
 
         We plot different quantities to asses how well our eccentricity
@@ -1973,15 +1973,15 @@
         Parameters:
         -----------
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.  If None, then uses "Notebook"
             when twocol is False and uses "APS" if twocol is True.
@@ -2058,15 +2058,15 @@
         return fig, axarr
 
     def plot_eccentricity(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             add_vline_at_tref=True,
             **kwargs):
         """Plot measured ecc as function of time.
 
         Parameters:
@@ -2078,15 +2078,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2130,15 +2130,15 @@
             return ax
 
     def plot_decc_dt(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             **kwargs):
         """Plot decc_dt as function of time to check monotonicity.
 
         If decc_dt becomes positive, ecc(t) is not monotonically decreasing.
 
@@ -2151,15 +2151,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2203,15 +2203,15 @@
             return ax
 
     def plot_mean_anomaly(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             add_vline_at_tref=True,
             **kwargs):
         """Plot measured mean anomaly as function of time.
 
         Parameters:
@@ -2223,15 +2223,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2275,15 +2275,15 @@
             return ax
 
     def plot_omega22(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             **kwargs):
         """Plot omega22, the locations of the apocenters and pericenters.
 
         Also plots their corresponding interpolants.
         This would show if the method is missing any pericenters/apocenters or
@@ -2298,15 +2298,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2346,20 +2346,28 @@
         # set reasonable ylims
         ymin = min(self.omega22)
         ymax = max(self.omega22)
         pad = 0.05 * ymax  # 5 % buffer for better visibility
         ax.set_ylim(ymin - pad, ymax + pad)
         # add help text
         if add_help_text:
+            if usetex:
+                help_text = (
+                    r"\noindent To avoid extrapolation, first and last\\"
+                    r"extrema are excluded when\\"
+                    r"evaluating $\omega_{a}$/$\omega_{p}$ interpolants")
+            else:
+                help_text = (
+                    "To avoid extrapolation, first and last\n"
+                    "extrema are excluded when\n"
+                    r"evaluating $\omega_{a}$/$\omega_{p}$ interpolants")
             ax.text(
                 0.22,
                 0.98,
-                (r"\noindent To avoid extrapolation, first and last\\"
-                 r"extrema are excluded when\\"
-                 r"evaluating $\omega_{a}$/$\omega_{p}$ interpolants"),
+                help_text,
                 ha="left",
                 va="top",
                 transform=ax.transAxes)
         ax.set_xlabel(r"$t$")
         ax.set_ylabel(labelsDict["omega22"])
         ax.legend(frameon=True,
                   handlelength=1, labelspacing=0.2, columnspacing=1)
@@ -2369,15 +2377,15 @@
             return ax
 
     def plot_omega22_average(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             plot_omega22=True,
             plot_orbit_averaged_omega22_at_extrema=False,
             **kwargs):
         """Plot omega22_average.
 
@@ -2390,15 +2398,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2455,15 +2463,15 @@
         ax.set_xlabel(r"$t$")
         ax.set_ylabel("Averaged frequency")
         # add help text
         if add_help_text:
             ax.text(
                 0.35,
                 0.98,
-                (r"\noindent omega22_average should be "
+                (r"omega22_average should be "
                  "monotonically increasing."),
                 ha="left",
                 va="top",
                 transform=ax.transAxes)
         ax.legend(frameon=True,
                   handlelength=1, labelspacing=0.2, columnspacing=1)
         if fig is None or ax is None:
@@ -2472,15 +2480,15 @@
             return ax
 
     def plot_amp22(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             **kwargs):
         """Plot amp22, the locations of the apocenters and pericenters.
 
         This would show if the method is missing any pericenters/apocenters or
         selecting one which is not a pericenter/apocenter.
@@ -2494,15 +2502,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2542,15 +2550,15 @@
             return ax
 
     def plot_phase_diff_ratio_between_extrema(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             **kwargs):
         """Plot phase diff ratio between consecutive extrema as function of time.
 
         Plots deltaPhi_orb(i)/deltaPhi_orb(i-1), where deltaPhi_orb is the
         change in orbital phase from the previous extrema to the ith extrema.
@@ -2567,15 +2575,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2633,15 +2641,15 @@
             return ax
 
     def plot_residual_omega22(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             **kwargs):
         """Plot residual omega22, the locations of the apocenters and pericenters.
 
         Useful to look for bad omega22 data near merger.
         We also throw away post merger before since it makes the plot
@@ -2656,15 +2664,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.  Default is Notebook.
         use_fancy_settings:
@@ -2706,15 +2714,15 @@
             return ax
 
     def plot_residual_amp22(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             **kwargs):
         """Plot residual amp22, the locations of the apocenters and pericenters.
 
         Parameters:
         -----------
@@ -2725,15 +2733,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
@@ -2777,15 +2785,15 @@
             return ax
 
     def plot_data_used_for_finding_extrema(
             self,
             fig=None,
             ax=None,
             add_help_text=True,
-            usetex=True,
+            usetex=False,
             style="Notebook",
             use_fancy_settings=True,
             add_vline_at_tref=True,
             **kwargs):
         """Plot the data that is being used.
 
         Also the locations of the apocenters and pericenters.
@@ -2798,15 +2806,15 @@
             Axis object to add the plot to. If None, initiates a new axis
             object.  Default is None.
         add_help_text:
             If True, add text to describe features in the plot.
             Default is True.
         usetex:
             If True, use TeX to render texts.
-            Default is True.
+            Default is False.
         style:
             Set font size, figure size suitable for particular use case. For
             example, to generate plot for "APS" journals, use style="APS".  For
             showing plots in a jupyter notebook, use "Notebook" so that plots
             are bigger and fonts are appropriately larger and so on.  See
             plot_settings.py for more details.
             Default is Notebook.
```

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingAmplitude.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitude.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingFrequency.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequency.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingFrequencyFits.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingFrequencyFits.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/eccDefinitionUsingResidualFrequency.py` & `gw_eccentricity-1.0.1/gw_eccentricity/eccDefinitionUsingResidualFrequency.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/group_nr_waveforms.py` & `gw_eccentricity-1.0.1/gw_eccentricity/group_nr_waveforms.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/gw_eccentricity.py` & `gw_eccentricity-1.0.1/gw_eccentricity/gw_eccentricity.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 See our paper https://arxiv.org/abs/2302.11257 and
 https://pypi.org/project/gw_eccentricity for more details.
 """
 __copyright__ = "Copyright (C) 2023 Md Arif Shaikh, Vijay Varma, Harald Pfeiffer"
 __email__ = "arifshaikh.astro@gmail.com, vijay.varma392@gmail.com"
 __status__ = "testing"
 __author__ = "Md Arif Shaikh, Vijay Varma, Harald Pfeiffer"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __license__ = """
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/load_data.py` & `gw_eccentricity-1.0.1/gw_eccentricity/load_data.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/plot_settings.py` & `gw_eccentricity-1.0.1/gw_eccentricity/plot_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,16 +121,17 @@
     rc("ytick", labelsize=ticklabelSizeDict[style])
     rc("xtick", direction="in")
     rc("ytick", direction="in")
     # Legend
     rc("legend", frameon=False)
     rc("legend", fontsize=fontSizeDict[style])
     # Fonts
-    rc("font", family="serif")
-    rc("font", serif="times")
+    if usetex:
+        rc("font", family="serif")
+        rc("font", serif="times")
     rc("font", size=fontSizeDict[style])
     # Lines
     rc("lines", linewidth=1.0)
 
 
 # Dictionary of labels to use in plots.
 labelsDict = {
```

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/truncate_waveform_by_flow.py` & `gw_eccentricity-1.0.1/gw_eccentricity/truncate_waveform_by_flow.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity/utils.py` & `gw_eccentricity-1.0.1/gw_eccentricity/utils.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity.egg-info/PKG-INFO` & `gw_eccentricity-1.0.1/gw_eccentricity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gw-eccentricity
-Version: 1.0.0
+Version: 1.0.1
 Summary: Defining eccentricity for gravitational wave astronomy.
 Home-page: https://github.com/vijayvarma392/gw_eccentricity
 Author: Md Arif Shaikh, Vijay Varma, Harald Pfeiffer
 Author-email: arifshaikh.astro@gmail.com, vijay.varma392@gmail.com
 License: UNKNOWN
 Description: <h1> <img src="https://raw.githubusercontent.com/vijayvarma392/gw_eccentricity/main/data/hreal.png"></h1>
         
         <h3 align="center"> Defining eccentricity for gravitational wave astronomy </h4>
         
         <div align="center">
         
         [![github](https://img.shields.io/badge/GitHub-gw_eccentricity-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity)
-        [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg)](https://pypi.org/project/gw_eccentricity)
+        [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg?kill_cache=1)](https://pypi.org/project/gw_eccentricity)
         [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity/blob/main/LICENSE)
-        [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
+        [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg?kill_cache=1)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
         
         </div>
         
         # About
         
         **gw_eccentricity** provides methods to measure eccentricity and mean anomaly
         from gravitational waveforms.
```

### Comparing `gw_eccentricity-1.0.0/gw_eccentricity.egg-info/SOURCES.txt` & `gw_eccentricity-1.0.1/gw_eccentricity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/setup.py` & `gw_eccentricity-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/test/test_example_notebooks.py` & `gw_eccentricity-1.0.1/test/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/test/test_interface.py` & `gw_eccentricity-1.0.1/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/test/test_mks_vs_dimless_units.py` & `gw_eccentricity-1.0.1/test/test_mks_vs_dimless_units.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/test/test_regression.py` & `gw_eccentricity-1.0.1/test/test_regression.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.0/test/test_time_convention.py` & `gw_eccentricity-1.0.1/test/test_time_convention.py`

 * *Files identical despite different names*

