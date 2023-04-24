# Comparing `tmp/unravel-python-1.2.1.tar.gz` & `tmp/unravel-python-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.1.tar", last modified: Thu Apr 20 08:12:29 2023, max compression
+gzip compressed data, was "unravel-python-1.2.2.tar", last modified: Mon Apr 24 11:41:24 2023, max compression
```

## Comparing `unravel-python-1.2.1.tar` & `unravel-python-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:12:29.850000 unravel-python-1.2.1/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3897 2023-04-20 08:12:30.000000 unravel-python-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 08:12:30.000000 unravel-python-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:12:29.850000 unravel-python-1.2.1/unravel/
--rw-rw-rw-   0        0        0      358 2023-04-20 08:12:00.000000 unravel-python-1.2.1/unravel/__init__.py
--rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.1/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.1/unravel/example.py
--rw-rw-rw-   0        0        0    14119 2023-04-20 08:05:44.000000 unravel-python-1.2.1/unravel/utils.py
--rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.1/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:12:29.860000 unravel-python-1.2.1/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3897 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 08:12:30.000000 unravel-python-1.2.1/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 11:41:24.120000 unravel-python-1.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3897 2023-04-24 11:41:26.000000 unravel-python-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 11:41:26.000000 unravel-python-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:41:24.140000 unravel-python-1.2.2/unravel/
+-rw-rw-rw-   0        0        0      358 2023-04-24 11:41:10.000000 unravel-python-1.2.2/unravel/__init__.py
+-rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.2/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.2/unravel/example.py
+-rw-rw-rw-   0        0        0    14562 2023-04-24 11:36:50.000000 unravel-python-1.2.2/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.2/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:41:24.140000 unravel-python-1.2.2/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3897 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-24 11:41:26.000000 unravel-python-1.2.2/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.1/LICENSE` & `unravel-python-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.1/PKG-INFO` & `unravel-python-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.1
+Version: 1.2.2
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `unravel-python-1.2.1/README.md` & `unravel-python-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.1/setup.py` & `unravel-python-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.1/unravel/core.py` & `unravel-python-1.2.2/unravel/core.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.1/unravel/example.py` & `unravel-python-1.2.2/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.1/unravel/utils.py` & `unravel-python-1.2.2/unravel/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Jun  4 22:17:13 2022
 
 @author: DELINTE Nicolas
 """
 
+import warnings
 import numpy as np
 from dipy.io.streamline import load_tractogram
 
 
 def tract_to_ROI(trk_file: str):
     '''
     Returns a binary mask of each voxel containing a tractography node.The
@@ -38,29 +39,32 @@
     for i in range(b.shape[0]):
 
         ROI[(int(b[i, 0]), int(b[i, 1]), int(b[i, 2]))] = 1
 
     return ROI
 
 
-def peaks_to_RGB(peaksList: list, fracList: list = None, fvfList: list = None):
+def peaks_to_RGB(peaksList: list, fracList: list = None, fvfList: list = None,
+                 order: str = 'rgb'):
     '''
     Returns a RGB map of shape (x,y,z,3) representing the main direction of
     of the peaks. Optionnaly scaled by fraction and/or fiber volume fraction.
 
     Parameters
     ----------
     peaksList : list of 4-D arrays
         List of arrays containing the peaks of shape (x,y,z,3)
     fracList : list of 3-D arrays, optional
         List of arrays of shape (x,y,z) containing the fraction of each fixel.
         The default is None.
     fvfList : list of 3-D arrays, optional
         List of arrays of shape (x,y,z) containing the fiber volume fraction of
         each fixel. The default is None.
+    order : str, optional
+        Order of colors, either 'rgb', 'gbr' or 'brg'. The default is 'rgb'.
 
     Returns
     -------
     rgb : 4-D array of shape (x,y,z,3)
         RGB map of shape (x,y,z,3) representing the main direction of
         of the peaks. With type float64 [0,1].
 
@@ -75,19 +79,19 @@
                 peaksList.append(peaksArray[:, :, :, :, k])
         else:
             peaksList = [peaksList]
 
     K = len(peaksList)
     dim = len(peaksList[0].shape[:-1])
 
-    len_ratio = np.ones(peaksList[0].shape[:-1])
+    peak_count = np.zeros(peaksList[0].shape[:-1])
 
     for k in range(K):
         peaksList[k] = np.nan_to_num(peaksList[k])
-        len_ratio += np.where(np.sum(peaksList[k], axis=dim) == 0, 1, 0)
+        peak_count += np.where(np.sum(peaksList[k], axis=dim) != 0, 1, 0)
 
     if fracList is None:
         fracList = []
         for k in range(K):
             fracList.append(np.ones(peaksList[0].shape[:-1]))
 
     if fvfList is None:
@@ -98,18 +102,27 @@
     rgb = np.zeros(peaksList[0].shape)
 
     for xyz in np.ndindex(peaksList[0].shape[:-1]):
         for k in range(K):
             rgb[xyz] += abs(peaksList[k][xyz])*fracList[k][xyz]*fvfList[k][xyz]
 
     # Normalize between [0,1] and by number of peaks per voxel
-    rgb *= np.repeat(1+len_ratio[(slice(None),) *
-                     dim + (np.newaxis,)]/K, 3, axis=dim)
+    p = peak_count[(slice(None),) * dim + (np.newaxis,)]
+    warnings.filterwarnings("ignore")
+    rgb *= np.repeat(1+(K-p)/p, 3, axis=dim)
+    warnings.filterwarnings("default")
+    rgb[np.isnan(rgb)] = 0
     rgb /= np.max(rgb)
 
+    # Color order
+    if order == 'brg':
+        rgb = rgb[(slice(None),) * 3 + ([2, 0, 1],)]
+    elif order == 'gbr':
+        rgb = rgb[(slice(None),) * 3 + ([1, 2, 0],)]
+
     return rgb
 
 
 def peaks_to_peak(peaksList: list, fixel_weights, fracList: list = None,
                   fvfList: list = None):
     '''
     Fuse peaks into a single peak based on fixel weight and fvf, intensity
```

### Comparing `unravel-python-1.2.1/unravel/viz.py` & `unravel-python-1.2.2/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.1/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.2/unravel_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.1
+Version: 1.2.2
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

