# Comparing `tmp/maxrf4u-0.1.2.tar.gz` & `tmp/maxrf4u-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maxrf4u-0.1.2.tar", last modified: Mon Apr 17 20:07:10 2023, max compression
+gzip compressed data, was "dist/maxrf4u-0.1.3.tar", last modified: Mon Apr 24 21:26:23 2023, max compression
```

## Comparing `maxrf4u-0.1.2.tar` & `maxrf4u-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/
--rw-rw-r--   0 frank     (1000) frank     (1000)    35149 2022-02-01 10:31:49.000000 maxrf4u-0.1.2/LICENSE
--rw-rw-r--   0 frank     (1000) frank     (1000)      111 2021-02-17 00:39:42.000000 maxrf4u-0.1.2/MANIFEST.in
--rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)      916 2023-03-22 10:41:52.000000 maxrf4u-0.1.2/README.md
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u/
--rw-rw-r--   0 frank     (1000) frank     (1000)      328 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/__init__.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    11890 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/_modidx.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     2821 2023-02-08 12:52:01.000000 maxrf4u-0.1.2/maxrf4u/_nbdev.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      171 2022-08-11 10:43:22.000000 maxrf4u-0.1.2/maxrf4u/absorption.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     7929 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/calibration.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      119 2022-09-23 13:00:31.000000 maxrf4u-0.1.2/maxrf4u/fingerprints.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    16909 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/hotmax.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     6169 2023-03-22 15:38:39.000000 maxrf4u-0.1.2/maxrf4u/interactive_visualization.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      127 2022-10-07 13:48:18.000000 maxrf4u-0.1.2/maxrf4u/iplotting.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      133 2023-02-08 12:52:01.000000 maxrf4u-0.1.2/maxrf4u/peak_pattern_puzzle_solver.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    13069 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/peakmaps.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    12230 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/peakpuzzle.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      115 2022-09-23 13:00:31.000000 maxrf4u-0.1.2/maxrf4u/speckles.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    11818 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/storage.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    10026 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/warp.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     4131 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/xphysics.py
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/
--rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)      626 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/SOURCES.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        1 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/dependency_links.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)       57 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/entry_points.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        1 2022-02-01 23:46:37.000000 maxrf4u-0.1.2/maxrf4u.egg-info/not-zip-safe
--rw-rw-r--   0 frank     (1000) frank     (1000)      170 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/requires.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        8 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/top_level.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)      958 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/settings.ini
--rw-rw-r--   0 frank     (1000) frank     (1000)       38 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/setup.cfg
--rw-rw-r--   0 frank     (1000) frank     (1000)     2560 2023-01-20 02:50:04.000000 maxrf4u-0.1.2/setup.py
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/
+-rw-rw-r--   0 frank     (1000) frank     (1000)    35149 2022-02-01 10:31:49.000000 maxrf4u-0.1.3/LICENSE
+-rw-rw-r--   0 frank     (1000) frank     (1000)      111 2021-02-17 00:39:42.000000 maxrf4u-0.1.3/MANIFEST.in
+-rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/PKG-INFO
+-rw-rw-r--   0 frank     (1000) frank     (1000)      916 2023-03-22 10:41:52.000000 maxrf4u-0.1.3/README.md
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u/
+-rw-rw-r--   0 frank     (1000) frank     (1000)      328 2023-04-24 21:26:14.000000 maxrf4u-0.1.3/maxrf4u/__init__.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    11890 2023-04-24 21:26:14.000000 maxrf4u-0.1.3/maxrf4u/_modidx.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     2821 2023-02-08 12:52:01.000000 maxrf4u-0.1.3/maxrf4u/_nbdev.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      171 2022-08-11 10:43:22.000000 maxrf4u-0.1.3/maxrf4u/absorption.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     8257 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/calibration.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      119 2022-09-23 13:00:31.000000 maxrf4u-0.1.3/maxrf4u/fingerprints.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    16909 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/hotmax.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     6169 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/interactive_visualization.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      127 2022-10-07 13:48:18.000000 maxrf4u-0.1.3/maxrf4u/iplotting.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      133 2023-02-08 12:52:01.000000 maxrf4u-0.1.3/maxrf4u/peak_pattern_puzzle_solver.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    13069 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/peakmaps.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    12230 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/peakpuzzle.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      115 2022-09-23 13:00:31.000000 maxrf4u-0.1.3/maxrf4u/speckles.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    11818 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/storage.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    10026 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/maxrf4u/warp.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     4131 2023-04-24 21:26:14.000000 maxrf4u-0.1.3/maxrf4u/xphysics.py
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/
+-rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/PKG-INFO
+-rw-rw-r--   0 frank     (1000) frank     (1000)      626 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/SOURCES.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        1 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/dependency_links.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)       57 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/entry_points.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        1 2022-02-01 23:46:37.000000 maxrf4u-0.1.3/maxrf4u.egg-info/not-zip-safe
+-rw-rw-r--   0 frank     (1000) frank     (1000)      170 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/requires.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        8 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/maxrf4u.egg-info/top_level.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)      958 2023-04-24 21:26:13.000000 maxrf4u-0.1.3/settings.ini
+-rw-rw-r--   0 frank     (1000) frank     (1000)       38 2023-04-24 21:26:23.000000 maxrf4u-0.1.3/setup.cfg
+-rw-rw-r--   0 frank     (1000) frank     (1000)     2560 2023-01-20 02:50:04.000000 maxrf4u-0.1.3/setup.py
```

### Comparing `maxrf4u-0.1.2/LICENSE` & `maxrf4u-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/PKG-INFO` & `maxrf4u-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxrf4u
-Version: 0.1.2
+Version: 0.1.3
 Summary: Explore your X-Ray Fluorescence spectral images
 Home-page: https://github.com/fligt/maxrf4u
 Author: Frank Ligterink
 Author-email: frank.ligterink@gmail.com
 License: GNU General Public License v3
 Description: # Welcome to maxrf4u
```

### Comparing `maxrf4u-0.1.2/README.md` & `maxrf4u-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/_modidx.py` & `maxrf4u-0.1.3/maxrf4u/_modidx.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/_nbdev.py` & `maxrf4u-0.1.3/maxrf4u/_nbdev.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/calibration.py` & `maxrf4u-0.1.3/maxrf4u/calibration.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import matplotlib.cm as cm 
 import math
 
 # %% ../notebooks/20_calibration.ipynb 14
 RHODIUM_Ka = 20.210105052526263 # Rh_KL3 
 IRON_Ka = 6.4032016008004 # Fe_KL3 
 
-def calibrate(datastack_file, anode='Rh', prominence=0.1): 
+def calibrate(datastack_file, anode='Rh', prominence=0.1, tube_keV=40): 
     '''Automatic two step energy energy calibration. 
     
     In step 1 a preliminary calibration is done assuming that the  
     sensor peak is located at 0 keV and the Rhodium anode Ka peak 
     is next to it's high and broad Compton scattering peak in the sum spectrum. 
     
     This preliminary calibration the enables the identification of Fe_Ka peak in 
@@ -35,15 +35,15 @@
     ds = maxrf4u.DataStack(datastack_file)
     
     y_max = ds.read(ds.MAXRF_MAXSPECTRUM)
     y_sum = ds.read(ds.MAXRF_SUMSPECTRUM) 
     
     # LOCATE INSTRUMENT PEAK INDICES IN SUM SPECTRUM 
     
-    left_peak_i, compton_peak_i, right_peak_i = find_instrument_peaks(y_sum) 
+    left_peak_i, compton_peak_i, right_peak_i = find_instrument_peaks(y_sum, tube_keV=tube_keV) 
     
     # STEP 1: PRELIMINARY SENSOR + ANODE CALIBRATION TO LOCATE IRON Fe_Ka PEAK  
     
     left_keV = 0
     right_keV = RHODIUM_Ka 
     
     n_channels = len(y_sum) 
@@ -160,57 +160,64 @@
     E1 = 1000 * keV1 * e 
 
     theta = (180 / pi) * np.arccos(1 - m0 * c**2 * (1/E0 - 1/E1))
 
     return theta 
 
 
-def find_instrument_peaks(y_sum, prominence=0.1):  
+def find_instrument_peaks(y_sum, prominence=0.1, tube_keV=40):  
     '''Locate key instrument peaks: 
     
               1) left hand sensor peak index  
               2) anode Compton peak index  
               3) right hand (rhodium) anode Ka peak index  
               
               in sum spectrum `y_sum`. 
     
-    Assumes anode material is rhodium, and Compton peak is second highest in sum spectrum.  
+    Assumes anode material is rhodium, and Compton peak energy is 
+    first peak below (uncalibrated) 20 keV, based on tube keV.     
     
     Returns: [left_peak_i, compton_peak_i, right_peak_i] 
     '''
     
-    # find peaks in sum spectrum 
+    # find all prominent peaks in sum spectrum 
     n_channels = len(y_sum) 
     x_indices = np.arange(n_channels)
     sum_peak_indices, shapes_dict = ssg.find_peaks(y_sum, prominence=prominence)
     
+    # Sensor peak 
     # assume sensor peak index is first peak index in list    
     left_peak_i = sum_peak_indices[0] 
     
-    # clean spectrum by clipping first 5% channels 
-    # that should remove the (typically highest) sensor peak  
-    # now assume highest peak in clean spectrum 
-    # is Compton scattering of anode Ka emission  
-    n_sensor = n_channels // 20
-    y_sum_clean = y_sum.copy()
-    y_sum_clean[0:n_sensor] = 0 
-
-    compton_peak_i = np.argmax(y_sum_clean) 
+    # Compton peak (new approach)
+    # assume that Compton peak is first peak below 20 keV 
+    # in `tube_keV` based uncalibrated spectrum 
+    # i.e. with energies ranging from 0 to `tube_keV` 
+     
+    x_approx_keVs = np.linspace(0, tube_keV, n_channels)
+    peak_approx_keVs = x_approx_keVs[sum_peak_indices] # approximate peak keVs from tube keV 
+    is_below20keV = peak_approx_keVs < 20 
+    
+    i = np.argmax(peak_approx_keVs[is_below20keV]) # peak number 
+    compton_peak_i = sum_peak_indices[i]
     
+    # Anode peak 
     # find anode peak channel index right next to Compton peak    
     right_peak_i = sum_peak_indices[list(sum_peak_indices).index(compton_peak_i) + 1] 
     
     return [left_peak_i, compton_peak_i, right_peak_i]
       
 
 
 
 def compton_shift(keV_in, theta): 
     '''Compute Compton shift for photon energies `keV_in` and scatter angle `theta`. 
     
+    Assuming single scattering. 
+    
     Returns: keV_out'''
     
 
     # See: https://en.wikipedia.org/wiki/Compton_scattering 
 
     # constants 
     e = 1.602e-19 # electron charge
```

### Comparing `maxrf4u-0.1.2/maxrf4u/hotmax.py` & `maxrf4u-0.1.3/maxrf4u/hotmax.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/interactive_visualization.py` & `maxrf4u-0.1.3/maxrf4u/interactive_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../notebooks/91_interactive-plotting.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../notebooks/80_interactive-plotting.ipynb.
 
 # %% auto 0
 __all__ = ['UploadDir', 'make_filenames', 'make_gridbox_widget']
 
-# %% ../notebooks/91_interactive-plotting.ipynb 25
+# %% ../notebooks/80_interactive-plotting.ipynb 25
 import json 
 import os 
 
 import IPython 
 
 from IPython.display import display
 from IPython.display import Image
@@ -23,15 +23,15 @@
 import os 
 
 import PIL
 import urllib 
 import numpy as np 
 import matplotlib.pyplot as plt
 
-# %% ../notebooks/91_interactive-plotting.ipynb 26
+# %% ../notebooks/80_interactive-plotting.ipynb 26
 class UploadDir(): 
     
     def __init__(self, mount_dir, objnr, bucket_url, subdir='images'):
         '''Creates a standard upload (image) directory object. '''
         
         self._mount_dir = mount_dir
         self._objnr = objnr
```

### Comparing `maxrf4u-0.1.2/maxrf4u/peakmaps.py` & `maxrf4u-0.1.3/maxrf4u/peakmaps.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/peakpuzzle.py` & `maxrf4u-0.1.3/maxrf4u/peakpuzzle.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/storage.py` & `maxrf4u-0.1.3/maxrf4u/storage.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/warp.py` & `maxrf4u-0.1.3/maxrf4u/warp.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u/xphysics.py` & `maxrf4u-0.1.3/maxrf4u/xphysics.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/maxrf4u.egg-info/PKG-INFO` & `maxrf4u-0.1.3/maxrf4u.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxrf4u
-Version: 0.1.2
+Version: 0.1.3
 Summary: Explore your X-Ray Fluorescence spectral images
 Home-page: https://github.com/fligt/maxrf4u
 Author: Frank Ligterink
 Author-email: frank.ligterink@gmail.com
 License: GNU General Public License v3
 Description: # Welcome to maxrf4u
```

### Comparing `maxrf4u-0.1.2/maxrf4u.egg-info/SOURCES.txt` & `maxrf4u-0.1.3/maxrf4u.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.2/settings.ini` & `maxrf4u-0.1.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = maxrf4u
 lib_name = maxrf4u
-version = 0.1.2
+version = 0.1.3
 min_python = 3.7
 license = gpl3
 black_formatting = False
 doc_path = _docs
 lib_path = maxrf4u
 nbs_path = notebooks
 recursive = True
```

### Comparing `maxrf4u-0.1.2/setup.py` & `maxrf4u-0.1.3/setup.py`

 * *Files identical despite different names*

