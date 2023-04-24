# Comparing `tmp/pystrum-0.2.tar.gz` & `tmp/pystrum-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystrum-0.2.tar", last modified: Fri Jun  3 12:02:10 2022, max compression
+gzip compressed data, was "pystrum-0.3.tar", last modified: Mon Apr 24 14:09:54 2023, max compression
```

## Comparing `pystrum-0.2.tar` & `pystrum-0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2022-06-03 12:02:10.388761 pystrum-0.2/
--rw-rw-r--   0 avd12    (3018093) recon     (1046)      394 2022-06-03 12:02:10.388761 pystrum-0.2/PKG-INFO
-drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2022-06-03 12:02:10.383761 pystrum-0.2/pystrum/
--rw-rw-r--   0 avd12    (3018093) recon     (1046)       62 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/__init__.py
-drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2022-06-03 12:02:10.385761 pystrum-0.2/pystrum/medipy/
--rw-rw-r--   0 avd12    (3018093) recon     (1046)       22 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/medipy/__init__.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)     1665 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/medipy/metrics.py
-drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2022-06-03 12:02:10.386761 pystrum-0.2/pystrum/pynd/
--rw-rw-r--   0 avd12    (3018093) recon     (1046)       68 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pynd/__init__.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)      555 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pynd/imutils.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)    21089 2021-08-25 21:23:02.000000 pystrum-0.2/pystrum/pynd/ndutils.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)    17657 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pynd/patchlib.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)     3181 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pynd/segutils.py
-drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2022-06-03 12:02:10.387761 pystrum-0.2/pystrum/pytools/
--rw-rw-r--   0 avd12    (3018093) recon     (1046)       40 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pytools/__init__.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)     1053 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pytools/core.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)     4990 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pytools/iniparse.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)     2214 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pytools/plot.py
--rw-rw-r--   0 avd12    (3018093) recon     (1046)      781 2021-04-19 17:53:46.000000 pystrum-0.2/pystrum/pytools/timer.py
-drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2022-06-03 12:02:10.384761 pystrum-0.2/pystrum.egg-info/
--rw-rw-r--   0 avd12    (3018093) recon     (1046)      394 2022-06-03 12:02:09.000000 pystrum-0.2/pystrum.egg-info/PKG-INFO
--rw-rw-r--   0 avd12    (3018093) recon     (1046)      487 2022-06-03 12:02:10.000000 pystrum-0.2/pystrum.egg-info/SOURCES.txt
--rw-rw-r--   0 avd12    (3018093) recon     (1046)        1 2022-06-03 12:02:09.000000 pystrum-0.2/pystrum.egg-info/dependency_links.txt
--rw-rw-r--   0 avd12    (3018093) recon     (1046)       27 2022-06-03 12:02:10.000000 pystrum-0.2/pystrum.egg-info/requires.txt
--rw-rw-r--   0 avd12    (3018093) recon     (1046)        8 2022-06-03 12:02:10.000000 pystrum-0.2/pystrum.egg-info/top_level.txt
--rw-rw-r--   0 avd12    (3018093) recon     (1046)       38 2022-06-03 12:02:10.388761 pystrum-0.2/setup.cfg
--rw-rw-r--   0 avd12    (3018093) recon     (1046)      579 2021-04-19 17:53:46.000000 pystrum-0.2/setup.py
+drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2023-04-24 14:09:54.549514 pystrum-0.3/
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)      394 2023-04-24 14:09:54.549514 pystrum-0.3/PKG-INFO
+drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2023-04-24 14:09:54.547514 pystrum-0.3/pystrum/
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)       83 2023-04-24 14:09:34.000000 pystrum-0.3/pystrum/__init__.py
+drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2023-04-24 14:09:54.547514 pystrum-0.3/pystrum/medipy/
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)       22 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/medipy/__init__.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)     1665 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/medipy/metrics.py
+drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2023-04-24 14:09:54.548514 pystrum-0.3/pystrum/pynd/
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)       68 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pynd/__init__.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)      555 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pynd/imutils.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)    18675 2023-03-24 18:11:37.000000 pystrum-0.3/pystrum/pynd/ndutils.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)    17657 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pynd/patchlib.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)     3109 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pynd/segutils.py
+drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2023-04-24 14:09:54.549514 pystrum-0.3/pystrum/pytools/
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)       40 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pytools/__init__.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)     1053 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pytools/core.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)     4990 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pytools/iniparse.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)     2214 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pytools/plot.py
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)      781 2022-06-15 19:01:15.000000 pystrum-0.3/pystrum/pytools/timer.py
+drwxrwsr-x   0 avd12    (3018093) recon     (1046)        0 2023-04-24 14:09:54.547514 pystrum-0.3/pystrum.egg-info/
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)      394 2023-04-24 14:09:54.000000 pystrum-0.3/pystrum.egg-info/PKG-INFO
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)      487 2023-04-24 14:09:54.000000 pystrum-0.3/pystrum.egg-info/SOURCES.txt
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)        1 2023-04-24 14:09:54.000000 pystrum-0.3/pystrum.egg-info/dependency_links.txt
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)       27 2023-04-24 14:09:54.000000 pystrum-0.3/pystrum.egg-info/requires.txt
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)        8 2023-04-24 14:09:54.000000 pystrum-0.3/pystrum.egg-info/top_level.txt
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)       38 2023-04-24 14:09:54.549514 pystrum-0.3/setup.cfg
+-rw-rw-r--   0 avd12    (3018093) recon     (1046)     1277 2023-03-24 18:11:37.000000 pystrum-0.3/setup.py
```

### Comparing `pystrum-0.2/pystrum/medipy/metrics.py` & `pystrum-0.3/pystrum/medipy/metrics.py`

 * *Files identical despite different names*

### Comparing `pystrum-0.2/pystrum/pynd/imutils.py` & `pystrum-0.3/pystrum/pynd/imutils.py`

 * *Files identical despite different names*

### Comparing `pystrum-0.2/pystrum/pynd/ndutils.py` & `pystrum-0.3/pystrum/pynd/ndutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 Tested on Python 3.5
 
 Contact: adalca@csail.mit.edu
 """
 
 import builtins
 import sys
-import re
-from ast import literal_eval
 
 import numpy as np
 import scipy as sp
 import scipy.ndimage
 from scipy.spatial import ConvexHull
-from scipy.ndimage.filters import convolve
 
 
 def boundingbox(bwvol):
     """
     bounding box coordinates of a nd volume
 
     Parameters
@@ -104,51 +101,14 @@
     notbwvol = np.logical_not(bwvol)
     negdst = bwdist(notbwvol)
 
     # combine the positive and negative map
     return posdst * notbwvol - negdst * bwvol
 
 
-def bw2boundary(bwvol, thickness=1):
-    """
-    computes the boundary between the binary True/False elements of logical bwvol
-
-    Parameters
-    ----------
-    bwvol : nd array
-        The logical volume
-
-    Returns
-    -------
-    sdtrf : nd array
-        the signed distance transform
-
-    See Also
-    --------
-    bwdist
-    """
-
-    # create a second-order difference filter kernel from Pascal's triangle
-    if np.round(thickness) == 1:
-        kern = np.array([-1, +2, -1]).reshape([3] + [1] * (bwvol.ndim - 1))
-    elif np.round(thickness) == 2:
-        kern = np.array([+1, -4, +6, -4, +1]).reshape([5] + [1] * (bwvol.ndim - 1))
-    elif np.round(thickness) == 3:
-        kern = np.array([-1, +6, -15, +20, -15, +6, -1]).reshape([7] + [1] * (bwvol.ndim - 1))
-    else:
-        assert np.round(thickness) in [1, 2, 3], 'thickness should be between 1 and 3'
-    # mark boundaries
-    conv = np.zeros_like(bwvol)
-    for i in range(0, bwvol.ndim):
-        filt = np.swapaxes(kern, 0, i)
-        conv = conv + np.abs(convolve(bwvol, filt))
-
-    return conv > 0
-
-
 bw_to_sdtrf = bw2sdtrf
 
 
 def bw_grid(vol_shape, spacing, thickness=1):
     """
     draw a black and white ND grid.
 
@@ -183,15 +143,15 @@
     # transform bw to nd grid.
     grid = volsize2ndgrid(bwvol.shape)
 
     # get the 1 points
     return np.concatenate([grid[d].flat for d in bwvol.ndims], 1)
 
 
-def bw2contour(bwvol, type='both', thr=1.01, method='sdt'):
+def bw2contour(bwvol, type='both', thr=1.01):
     """
     computes the contour of island(s) on a nd logical volume
 
     Parameters
     ----------
     bwvol : nd array
         The logical volume
@@ -206,37 +166,24 @@
         the contour map of the same size of the input
 
     See Also
     --------
     bwdist, bw2dstrf
     """
 
-    if method == 'sdt':
-        # obtain a signed distance transform for the bw volume
-        sdtrf = bw2sdtrf(bwvol)
-        if type == 'inner':
-            return np.logical_and(sdtrf <= 0, sdtrf > -thr)
-        elif type == 'outer':
-            return np.logical_and(sdtrf >= 0, sdtrf < thr)
-        else:
-            assert type == 'both', 'type should only be inner, outer or both'
-            return np.abs(sdtrf) < thr
+    # obtain a signed distance transform for the bw volume
+    sdtrf = bw2sdtrf(bwvol)
 
-    elif method == 'conv':
-        # obtain boundaries
-        sdtrf = bw2boundary(bwvol, thr)
-        if type == 'inner':
-            return np.logical_and(sdtrf, bwvol - 0)
-        elif type == 'outer':
-            return np.logical_and(sdtrf, 1 - bwvol)
-        else:
-            assert type == 'both', 'type should only be inner, outer or both'
-            return sdtrf
+    if type == 'inner':
+        return np.logical_and(sdtrf <= 0, sdtrf > -thr)
+    elif type == 'outer':
+        return np.logical_and(sdtrf >= 0, sdtrf < thr)
     else:
-        assert method in ['sdt', 'conv'], 'method must be either sdt or conv'
+        assert type == 'both', 'type should only be inner, outer or both'
+        return np.abs(sdtrf) < thr
 
 
 bw_to_contour = bw2contour
 
 
 def bw_sphere(volshape, rad, loc=None):
     """
@@ -627,23 +574,23 @@
 
         # add to existing volume
         vol = vol + wts[sci] * interp_vol
 
     return vol
 
 
-def sphere_vol(vol_shape, radius, center=None, dtype=np.bool):
+def sphere_vol(vol_shape, radius, center=None, dtype=bool):
     """
     draw nd sphere volume
 
     Args:
         vol_shape (list): volume shape, a list of integers
         center (list or int): list or integer, if list then same length as vol_shape list
         radius (float): radius of the circle
-        dtype (np.dtype): np.bool (binary sphere) or np.float32 (sphere with partial volume at edge)
+        dtype (np.dtype): bool (binary sphere) or np.float32 (sphere with partial volume at edge)
 
     Returns:
         [tf.bool or tf.float32]: bw sphere, either 0/1 (if bool) or [0,1] if float32
     """
 
     # prepare inputs
     assert isinstance(vol_shape, (list, tuple)), 'vol_shape needs to be a list or tuple'
@@ -654,15 +601,15 @@
             center = [(f - 1) / 2 for f in vol_shape]
         else:
             center = [center] * ndims
     else:
         assert len(center) == ndims, "center list length does not match vol_shape length"
 
     # check dtype
-    assert dtype in [np.bool, np.float32], 'dtype should be np.bool, np.float32'
+    assert dtype in [bool, np.float32], 'dtype should be bool, np.float32'
 
     # prepare mesh
     mesh = volsize2ndgrid(vol_shape)
     centered_mesh = [(mesh[f] - center[f])**2 for f in range(ndims)]
     dist_from_center = np.sqrt(np.sum(np.stack(centered_mesh, ndims), ndims))
 
     # create sphere
@@ -673,43 +620,18 @@
         edge = np.logical_and(df < 0, df > -1)
         sphere = float_sphere + edge * (1 + df)
 
     # done!
     return sphere
 
 
-def printed_numpy_to_array(string):
-    '''
-    transform a printed numpy array (string) to a numpy array
-
-    Example:
-    printed_array = """[[0.74268087, 0.23098959, 0.24466867, 0.69201753],
-       [0.09907753, 0.1472794 , 0.57733857, 0.35489757],
-       [0.91808391, 0.51522785, 0.86230898, 0.06236136]]
-       """
-    my_array = printed_numpy_to_array(printed_array)
-
-    '''
-    string = string.replace(',', ' ')
-    res = re.sub(r"([^[])\s+([^]])", r"\1, \2", string)
-    return np.array(literal_eval(res))
-
-
-def printed_file_to_array(file):
-    '''
-    read file of printed numpy array (string) to numpy array
-    '''
-    with open(file, 'r') as file:
-        return printed_numpy_to_array(file.read())
-
 ###############################################################################
 # internal
 ###############################################################################
 
-
 def _prep_range(*args):
     """
     _prep_range([start], end [,step])
     prepare the start, end and step for range and arange
 
     Parameters:
         [start] (vector): the start
```

### Comparing `pystrum-0.2/pystrum/pynd/patchlib.py` & `pystrum-0.3/pystrum/pynd/patchlib.py`

 * *Files identical despite different names*

### Comparing `pystrum-0.2/pystrum/pynd/segutils.py` & `pystrum-0.3/pystrum/pynd/segutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Contact: adalca@csail.mit.edu
 '''
 
 import numpy as np
 from . import ndutils as nd
 
 
-def seg2contour(seg, exclude_zero=True, contour_type='inner', thickness=1, method='sdt'):
+def seg2contour(seg, exclude_zero=True, contour_type='inner', thickness=1):
     '''
     transform nd segmentation (label maps) to contour maps
 
     Parameters
     ----------
     seg : nd array
         volume of labels/segmentations
@@ -42,16 +42,15 @@
     for lab in labels:
 
         # extract binary label map for this label
         label_map = seg == lab
 
         # extract contour map for this label
         thickness = thickness + 0.01
-        label_contour_map = nd.bw2contour(label_map, type=contour_type, thr=thickness, 
-                                          method=method)
+        label_contour_map = nd.bw2contour(label_map, type=contour_type, thr=thickness)
 
         # assign contour to this label
         contour_map[label_contour_map] = lab
 
     return contour_map
```

### Comparing `pystrum-0.2/pystrum/pytools/core.py` & `pystrum-0.3/pystrum/pytools/core.py`

 * *Files identical despite different names*

### Comparing `pystrum-0.2/pystrum/pytools/iniparse.py` & `pystrum-0.3/pystrum/pytools/iniparse.py`

 * *Files identical despite different names*

### Comparing `pystrum-0.2/pystrum/pytools/plot.py` & `pystrum-0.3/pystrum/pytools/plot.py`

 * *Files identical despite different names*

### Comparing `pystrum-0.2/pystrum/pytools/timer.py` & `pystrum-0.3/pystrum/pytools/timer.py`

 * *Files identical despite different names*

