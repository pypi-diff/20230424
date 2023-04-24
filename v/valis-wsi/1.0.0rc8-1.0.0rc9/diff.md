# Comparing `tmp/valis_wsi-1.0.0rc8.tar.gz` & `tmp/valis_wsi-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valis_wsi-1.0.0rc8.tar", last modified: Fri Jul  1 19:13:56 2022, max compression
+gzip compressed data, was "valis_wsi-1.0.0rc9.tar", last modified: Fri Aug  5 16:25:58 2022, max compression
```

## Comparing `valis_wsi-1.0.0rc8.tar` & `valis_wsi-1.0.0rc9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 gatenbcd (36240) HLM\Domain Users (20000)        0 2022-07-01 19:13:56.478871 valis_wsi-1.0.0rc8/
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)     1060 2022-01-05 14:37:34.000000 valis_wsi-1.0.0rc8/LICENSE.txt
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    41382 2022-07-01 19:13:56.479393 valis_wsi-1.0.0rc8/PKG-INFO
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    40753 2022-07-01 19:05:52.000000 valis_wsi-1.0.0rc8/README.rst
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)      103 2022-01-26 02:26:43.000000 valis_wsi-1.0.0rc8/pyproject.toml
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)      976 2022-07-01 19:13:56.482820 valis_wsi-1.0.0rc8/setup.cfg
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)       72 2022-01-25 21:05:49.000000 valis_wsi-1.0.0rc8/setup.py
-drwxr-xr-x   0 gatenbcd (36240) HLM\Domain Users (20000)        0 2022-07-01 19:13:56.436738 valis_wsi-1.0.0rc8/tests/
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)        0 2022-01-27 19:36:40.000000 valis_wsi-1.0.0rc8/tests/__init__.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)      175 2022-01-27 19:41:00.000000 valis_wsi-1.0.0rc8/tests/test_build.py
-drwxr-xr-x   0 gatenbcd (36240) HLM\Domain Users (20000)        0 2022-07-01 19:13:56.458645 valis_wsi-1.0.0rc8/valis/
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)      749 2022-07-01 18:47:45.000000 valis_wsi-1.0.0rc8/valis/__init__.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    36979 2022-01-25 21:40:23.000000 valis_wsi-1.0.0rc8/valis/affine_optimizer.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    12279 2022-01-25 21:40:23.000000 valis_wsi-1.0.0rc8/valis/feature_detectors.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    34154 2022-06-27 19:37:18.000000 valis_wsi-1.0.0rc8/valis/feature_matcher.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    53508 2022-07-01 18:46:37.000000 valis_wsi-1.0.0rc8/valis/non_rigid_registrars.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    16667 2022-07-01 18:58:20.000000 valis_wsi-1.0.0rc8/valis/preprocessing.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)   156118 2022-07-01 18:46:37.000000 valis_wsi-1.0.0rc8/valis/registration.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    43742 2022-06-27 19:37:18.000000 valis_wsi-1.0.0rc8/valis/serial_non_rigid.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    55892 2022-06-30 18:02:39.000000 valis_wsi-1.0.0rc8/valis/serial_rigid.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    82574 2022-06-28 14:49:36.000000 valis_wsi-1.0.0rc8/valis/slide_io.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)     9216 2022-06-30 20:16:03.000000 valis_wsi-1.0.0rc8/valis/slide_tools.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)     3478 2022-06-27 19:37:18.000000 valis_wsi-1.0.0rc8/valis/valtils.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    29812 2022-06-27 19:37:18.000000 valis_wsi-1.0.0rc8/valis/viz.py
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    94356 2022-06-27 19:37:18.000000 valis_wsi-1.0.0rc8/valis/warp_tools.py
-drwxr-xr-x   0 gatenbcd (36240) HLM\Domain Users (20000)        0 2022-07-01 19:13:56.477944 valis_wsi-1.0.0rc8/valis_wsi.egg-info/
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)    41382 2022-07-01 19:13:55.000000 valis_wsi-1.0.0rc8/valis_wsi.egg-info/PKG-INFO
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)      566 2022-07-01 19:13:56.000000 valis_wsi-1.0.0rc8/valis_wsi.egg-info/SOURCES.txt
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)        1 2022-07-01 19:13:55.000000 valis_wsi-1.0.0rc8/valis_wsi.egg-info/dependency_links.txt
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)      247 2022-07-01 19:13:55.000000 valis_wsi-1.0.0rc8/valis_wsi.egg-info/requires.txt
--rw-r--r--   0 gatenbcd (36240) HLM\Domain Users (20000)       12 2022-07-01 19:13:56.000000 valis_wsi-1.0.0rc8/valis_wsi.egg-info/top_level.txt
+drwxr-xr-x   0 gatenbcd (36240)    20000        0 2022-08-05 16:25:58.729966 valis_wsi-1.0.0rc9/
+-rw-r--r--   0 gatenbcd (36240)    20000     1060 2022-01-05 14:37:34.000000 valis_wsi-1.0.0rc9/LICENSE.txt
+-rw-r--r--   0 gatenbcd (36240)    20000    42426 2022-08-05 16:25:58.730266 valis_wsi-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 gatenbcd (36240)    20000    41797 2022-08-05 16:25:10.000000 valis_wsi-1.0.0rc9/README.rst
+-rw-r--r--   0 gatenbcd (36240)    20000      103 2022-01-26 02:26:43.000000 valis_wsi-1.0.0rc9/pyproject.toml
+-rw-r--r--   0 gatenbcd (36240)    20000      976 2022-08-05 16:25:58.731873 valis_wsi-1.0.0rc9/setup.cfg
+-rw-r--r--   0 gatenbcd (36240)    20000       72 2022-01-25 21:05:49.000000 valis_wsi-1.0.0rc9/setup.py
+drwxr-xr-x   0 gatenbcd (36240)    20000        0 2022-08-05 16:25:58.690221 valis_wsi-1.0.0rc9/tests/
+-rw-r--r--   0 gatenbcd (36240)    20000        0 2022-01-27 19:36:40.000000 valis_wsi-1.0.0rc9/tests/__init__.py
+-rw-r--r--   0 gatenbcd (36240)    20000      175 2022-01-27 19:41:00.000000 valis_wsi-1.0.0rc9/tests/test_build.py
+drwxr-xr-x   0 gatenbcd (36240)    20000        0 2022-08-05 16:25:58.721314 valis_wsi-1.0.0rc9/valis/
+-rw-r--r--   0 gatenbcd (36240)    20000      749 2022-08-04 17:31:53.000000 valis_wsi-1.0.0rc9/valis/__init__.py
+-rw-r--r--   0 gatenbcd (36240)    20000    36979 2022-01-25 21:40:23.000000 valis_wsi-1.0.0rc9/valis/affine_optimizer.py
+-rw-r--r--   0 gatenbcd (36240)    20000    12279 2022-07-22 22:08:32.000000 valis_wsi-1.0.0rc9/valis/feature_detectors.py
+-rw-r--r--   0 gatenbcd (36240)    20000    34184 2022-08-03 16:39:15.000000 valis_wsi-1.0.0rc9/valis/feature_matcher.py
+-rw-r--r--   0 gatenbcd (36240)    20000    55354 2022-08-03 16:39:15.000000 valis_wsi-1.0.0rc9/valis/non_rigid_registrars.py
+-rw-r--r--   0 gatenbcd (36240)    20000    16647 2022-08-03 16:39:15.000000 valis_wsi-1.0.0rc9/valis/preprocessing.py
+-rw-r--r--   0 gatenbcd (36240)    20000   155516 2022-08-04 17:13:52.000000 valis_wsi-1.0.0rc9/valis/registration.py
+-rw-r--r--   0 gatenbcd (36240)    20000    45413 2022-08-03 16:39:15.000000 valis_wsi-1.0.0rc9/valis/serial_non_rigid.py
+-rw-r--r--   0 gatenbcd (36240)    20000    56271 2022-08-03 20:13:03.000000 valis_wsi-1.0.0rc9/valis/serial_rigid.py
+-rw-r--r--   0 gatenbcd (36240)    20000    83180 2022-08-03 20:13:03.000000 valis_wsi-1.0.0rc9/valis/slide_io.py
+-rw-r--r--   0 gatenbcd (36240)    20000     9423 2022-08-03 20:13:03.000000 valis_wsi-1.0.0rc9/valis/slide_tools.py
+-rw-r--r--   0 gatenbcd (36240)    20000     3478 2022-06-27 19:37:18.000000 valis_wsi-1.0.0rc9/valis/valtils.py
+-rw-r--r--   0 gatenbcd (36240)    20000    31304 2022-08-03 20:13:03.000000 valis_wsi-1.0.0rc9/valis/viz.py
+-rw-r--r--   0 gatenbcd (36240)    20000   100521 2022-08-03 20:57:18.000000 valis_wsi-1.0.0rc9/valis/warp_tools.py
+drwxr-xr-x   0 gatenbcd (36240)    20000        0 2022-08-05 16:25:58.729261 valis_wsi-1.0.0rc9/valis_wsi.egg-info/
+-rw-r--r--   0 gatenbcd (36240)    20000    42426 2022-08-05 16:25:58.000000 valis_wsi-1.0.0rc9/valis_wsi.egg-info/PKG-INFO
+-rw-r--r--   0 gatenbcd (36240)    20000      566 2022-08-05 16:25:58.000000 valis_wsi-1.0.0rc9/valis_wsi.egg-info/SOURCES.txt
+-rw-r--r--   0 gatenbcd (36240)    20000        1 2022-08-05 16:25:58.000000 valis_wsi-1.0.0rc9/valis_wsi.egg-info/dependency_links.txt
+-rw-r--r--   0 gatenbcd (36240)    20000      247 2022-08-05 16:25:58.000000 valis_wsi-1.0.0rc9/valis_wsi.egg-info/requires.txt
+-rw-r--r--   0 gatenbcd (36240)    20000       12 2022-08-05 16:25:58.000000 valis_wsi-1.0.0rc9/valis_wsi.egg-info/top_level.txt
```

### Comparing `valis_wsi-1.0.0rc8/LICENSE.txt` & `valis_wsi-1.0.0rc9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `valis_wsi-1.0.0rc8/PKG-INFO` & `valis_wsi-1.0.0rc9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: valis_wsi
-Version: 1.0.0rc8
-Summary: A package to register whole slide images
-Home-page: https://valis.readthedocs.io/en/latest/
-Author: Chandler Gatenbee
-Author-email: Chandler.Gatenbee@moffitt.org
-Project-URL: Bug Tracker, https://github.com/MathOnco/valis/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
 
 |docs| |CI| |pypi|
 
 .. .. |Upload Python Package| image:: https://github.com/MathOnco/valis/actions/workflows/python-publish.yml/badge.svg
     :target: https://github.com/MathOnco/valis/actions/workflows/python-publish.yml
 
 .. .. |build-status| image:: https://circleci.com/gh/readthedocs/readthedocs.org.svg?style=svg
@@ -71,17 +54,19 @@
         * aliging each image towards the reference image following the same sequence used during rigid registation.
         * using groupwise registration that non-rigidly aligns the images to a common frame of reference. Currently this is only possible if `SimpleElastix <https://simpleelastix.github.io>`__ is installed.
 
    #. One can optionally perform a second non-rigid registration using higher resolution versions of each image. This is intended to better align micro-features not visible in the original images, and so is referred to as micro-registration
 
    #. Error is estimated by calculating the distance between registered matched features in the full resolution images.
 
-The transformations found by VALIS can then be used to warp the full resolution slides. It is also possible to merge non-RGB registered slides to create a highly multiplexed image. These aligned and/or merged slides can then be saved as ome.tiff images.
+The transformations found by VALIS can then be used to warp the full resolution slides. It is also possible to merge non-RGB registered slides to create a highly multiplexed image. These aligned and/or merged slides can then be saved as ome.tiff images. The transformations can also be use to warp point data, such as cell centroids, polygon vertices, etc...
+
+In addition to registering images, VALIS provides tools to read slides using Bio-Formats and OpenSlide, which can be read at multiple resolutions and converted to numpy arrays or pyvips.Image objects. One can also slice regions of interest from these slides. VALIS also provides functions to convert slides to the ome.tiff format, preserving the original metadata. Please see examples and documentation for more details.
+
 
-In addition to warping images and slides, VALIS can also warp point data, such as cell centoids or ROI coordinates.
 
 Full documentation can be found at `ReadTheDocs <https://valis.readthedocs.io/en/latest/>`_.
 
 .. contents:: Table of Contents
    :local:
    :depth: 1
 
@@ -578,14 +563,21 @@
     rigid_registrar, non_rigid_registrar, error_df = registrar.register()
 
     registration.kill_jvm() # Kill the JVM
 
 Change Log
 ==========
 
+Version 1.0.0rc9 (August 4, 2022)
+---------------------------------
+#. Reduced memory usage for micro-registration and warping. No longer copying memory before warping, and large displacement fields saved as .tiff images instead of .vips images.
+#. Reduced unwanted accumulation of displacements
+#. :code:`viz.draw_matches` now returns an image instead of a matplotlib pyplot
+#. Pull request 9-11 bug fixes (many thanks to crobbins327 and zindy): Not converting uint16 to uint8 when reading using Bio-Formats or pyvips; fixed rare error when filtering neighbor matches; :code:`viz.get_grid` consistent on Linux and Windows; typos.
+
 
 Version 1.0.0rc8 (July 1, 2022)
 -------------------------------
 #. Now compatible with single channel images. These images are treated as immunofluorescent images, and so custom pre-processing classes and arguments should be passed to :code:`if_processing_cls` and :code:`if_processing_kwargs` of the :code:`Valis.register` method. The current method will perform adaptive histogram equalization and scales the image to 0-255 (see :code:`preprocessing.ChannelGetter`). Also, since it isn't possible to determine if the single channel image is a greyscale RGB (light background) or single channel immunofluorescence (or similar with dark background), the background color will not be estimated, meaning that in the registered image the area outside of the warped image will be black (as opposed to the estimated background color). Tissue masks will still be created, but if it seems they are not covering enough area then try setting :code:`create_masks` to `False` when initializing the :code:`Valis` object.
 
 
 Version 1.0.0rc7 (June 27, 2022)
```

### Comparing `valis_wsi-1.0.0rc8/README.rst` & `valis_wsi-1.0.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: valis_wsi
+Version: 1.0.0rc9
+Summary: A package to register whole slide images
+Home-page: https://valis.readthedocs.io/en/latest/
+Author: Chandler Gatenbee
+Author-email: Chandler.Gatenbee@moffitt.org
+Project-URL: Bug Tracker, https://github.com/MathOnco/valis/issues
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 
 |docs| |CI| |pypi|
 
 .. .. |Upload Python Package| image:: https://github.com/MathOnco/valis/actions/workflows/python-publish.yml/badge.svg
     :target: https://github.com/MathOnco/valis/actions/workflows/python-publish.yml
 
 .. .. |build-status| image:: https://circleci.com/gh/readthedocs/readthedocs.org.svg?style=svg
@@ -54,17 +71,19 @@
         * aliging each image towards the reference image following the same sequence used during rigid registation.
         * using groupwise registration that non-rigidly aligns the images to a common frame of reference. Currently this is only possible if `SimpleElastix <https://simpleelastix.github.io>`__ is installed.
 
    #. One can optionally perform a second non-rigid registration using higher resolution versions of each image. This is intended to better align micro-features not visible in the original images, and so is referred to as micro-registration
 
    #. Error is estimated by calculating the distance between registered matched features in the full resolution images.
 
-The transformations found by VALIS can then be used to warp the full resolution slides. It is also possible to merge non-RGB registered slides to create a highly multiplexed image. These aligned and/or merged slides can then be saved as ome.tiff images.
+The transformations found by VALIS can then be used to warp the full resolution slides. It is also possible to merge non-RGB registered slides to create a highly multiplexed image. These aligned and/or merged slides can then be saved as ome.tiff images. The transformations can also be use to warp point data, such as cell centroids, polygon vertices, etc...
+
+In addition to registering images, VALIS provides tools to read slides using Bio-Formats and OpenSlide, which can be read at multiple resolutions and converted to numpy arrays or pyvips.Image objects. One can also slice regions of interest from these slides. VALIS also provides functions to convert slides to the ome.tiff format, preserving the original metadata. Please see examples and documentation for more details.
+
 
-In addition to warping images and slides, VALIS can also warp point data, such as cell centoids or ROI coordinates.
 
 Full documentation can be found at `ReadTheDocs <https://valis.readthedocs.io/en/latest/>`_.
 
 .. contents:: Table of Contents
    :local:
    :depth: 1
 
@@ -561,14 +580,21 @@
     rigid_registrar, non_rigid_registrar, error_df = registrar.register()
 
     registration.kill_jvm() # Kill the JVM
 
 Change Log
 ==========
 
+Version 1.0.0rc9 (August 4, 2022)
+---------------------------------
+#. Reduced memory usage for micro-registration and warping. No longer copying memory before warping, and large displacement fields saved as .tiff images instead of .vips images.
+#. Reduced unwanted accumulation of displacements
+#. :code:`viz.draw_matches` now returns an image instead of a matplotlib pyplot
+#. Pull request 9-11 bug fixes (many thanks to crobbins327 and zindy): Not converting uint16 to uint8 when reading using Bio-Formats or pyvips; fixed rare error when filtering neighbor matches; :code:`viz.get_grid` consistent on Linux and Windows; typos.
+
 
 Version 1.0.0rc8 (July 1, 2022)
 -------------------------------
 #. Now compatible with single channel images. These images are treated as immunofluorescent images, and so custom pre-processing classes and arguments should be passed to :code:`if_processing_cls` and :code:`if_processing_kwargs` of the :code:`Valis.register` method. The current method will perform adaptive histogram equalization and scales the image to 0-255 (see :code:`preprocessing.ChannelGetter`). Also, since it isn't possible to determine if the single channel image is a greyscale RGB (light background) or single channel immunofluorescence (or similar with dark background), the background color will not be estimated, meaning that in the registered image the area outside of the warped image will be black (as opposed to the estimated background color). Tissue masks will still be created, but if it seems they are not covering enough area then try setting :code:`create_masks` to `False` when initializing the :code:`Valis` object.
 
 
 Version 1.0.0rc7 (June 27, 2022)
```

### Comparing `valis_wsi-1.0.0rc8/setup.cfg` & `valis_wsi-1.0.0rc9/setup.cfg`

 * *Files identical despite different names*

### Comparing `valis_wsi-1.0.0rc8/valis/__init__.py` & `valis_wsi-1.0.0rc9/valis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0rc8"
+__version__ = "1.0.0rc9"
 
 from . import affine_optimizer
 from . import feature_detectors
 from . import feature_matcher
 from . import non_rigid_registrars
 from . import preprocessing
 from . import registration
```

### Comparing `valis_wsi-1.0.0rc8/valis/affine_optimizer.py` & `valis_wsi-1.0.0rc9/valis/affine_optimizer.py`

 * *Files identical despite different names*

### Comparing `valis_wsi-1.0.0rc8/valis/feature_detectors.py` & `valis_wsi-1.0.0rc9/valis/feature_detectors.py`

 * *Files identical despite different names*

### Comparing `valis_wsi-1.0.0rc8/valis/feature_matcher.py` & `valis_wsi-1.0.0rc9/valis/feature_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     if len(good_idx) == 0:
         filtered_src_points = []
         filtered_dst_points = []
     else:
         filtered_src_points = kp1_xy[good_idx, :]
         filtered_dst_points = kp2_xy[good_idx, :]
 
-    return filtered_src_points, filtered_dst_points, good_idx
+    return np.array(filtered_src_points), np.array(filtered_dst_points), np.array(good_idx)
 
 
 
 def filter_matches_tukey(src_xy, dst_xy):
     """Detect and remove outliers using Tukey's method
     Adapted from https://towardsdatascience.com/detecting-and-treating-outliers-in-python-part-1-4ece5098b755
```

### Comparing `valis_wsi-1.0.0rc8/valis/non_rigid_registrars.py` & `valis_wsi-1.0.0rc9/valis/non_rigid_registrars.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import SimpleITK as sitk
 from skimage import transform, color, filters, exposure, util
 from skimage import color as skcolor
 import pyvips
 import multiprocessing
 from joblib import Parallel, delayed, parallel_backend
+
 from tqdm import tqdm
 
 from . import viz
 from . import warp_tools
 from . import preprocessing
 
 NR_CLS_KEY = "non_rigid_registrar_cls"
@@ -1229,95 +1230,143 @@
 
         self.fwd_dxdy_tiles = None
         self.fwd_dxdy = None
 
         self.pbar = None
 
 
-    def norm_image(self, img):
+    def norm_img(self, img, stats, mask=None):
+        normed_img = exposure.rescale_intensity(img, out_range=(0, 255)).astype(np.uint8)
+        normed_img = preprocessing.norm_img_stats(normed_img, stats, mask)
+        normed_img = exposure.rescale_intensity(normed_img, out_range=(0, 255)).astype(np.uint8)
+
+        return normed_img
+
+    def norm_tiles(self, moving_img, fixed_img, tile_mask):
+        try:
+            # Try norming using these tile stats
+            if tile_mask is not None:
+                pos_px = np.where(tile_mask != 0)
+                tile_v = np.hstack([fixed_img[pos_px], moving_img[pos_px]])
+            else:
+                tile_v = np.hstack([fixed_img.reshape(-1), moving_img.reshape(-1)])
+
+            target_processing_stats = preprocessing.get_channel_stats(tile_v)
+
+            fixed_normed = self.norm_img(fixed_img, target_processing_stats, tile_mask)
+            moving_normed = self.norm_img(moving_img, target_processing_stats, tile_mask)
+
+        except ValueError:
+            # Norm using full image's stats
+            if self.target_stats is not None:
+                try:
+                    fixed_normed = self.norm_img(fixed_img, self.target_stats, tile_mask)
+                    moving_normed = self.norm_img(moving_img, self.target_stats, tile_mask)
+                except ValueError:
+                    fixed_normed = fixed_img
+                    moving_normed = moving_img
+            else:
+                fixed_normed = fixed_img
+                moving_normed = moving_img
+
+        return moving_normed, fixed_normed
+
+    def process_tile(self, img):
         """Process tiles
         """
         processor = self.processing_cls(image=img, src_f=None, level=None, series=None)
         try:
             processed_img = processor.process_image(**self.processing_kwargs)
         except TypeError:
             # processor.process_image doesn't take kwargs
             processed_img = processor.process_image()
 
-        if len(np.unique(processed_img)) == 1:
-            return processed_img
-        if self.target_stats is not None:
-            try:
-                processed_img = exposure.rescale_intensity(processed_img, out_range=(0, 255)).astype(np.uint8)
-                processed_img = preprocessing.norm_img_stats(processed_img, self.target_stats)
-                processed_img = exposure.rescale_intensity(processed_img, out_range=(0, 255)).astype(np.uint8)
-            except ValueError:
-                return processed_img
-
         return processed_img
 
+
     def reg_tile(self, tile_idx, lock):
 
         with lock:
             # Use lock when accessing images
-            fixed_tile = self.fixed_tiles[tile_idx]
-            moving_tile = self.moving_tiles[tile_idx]
-            if self.mask is not None:
-                tile_mask = self.mask_tiles[tile_idx]
+            tile_bbox_xywh = self.expanded_bboxes[tile_idx]
+            moving_tile = self.moving_img.extract_area(*tile_bbox_xywh)
+            fixed_tile = self.fixed_img.extract_area(*tile_bbox_xywh)
 
-                if tile_mask.max() == 0:
-                    # Nothing to register
-                    empty_dxdy = pyvips.Image.black(moving_tile.width, moving_tile.height, bands=2)
-                    self.bk_dxdy_tiles[tile_idx] = empty_dxdy
-                    self.fwd_dxdy_tiles[tile_idx] = empty_dxdy
-                    self.pbar.update(1)
-
-                    return None
-
-                # Apply mask #
-                moving_tile = (tile_mask == 0).ifthenelse(0, moving_tile)
-                fixed_tile = (tile_mask == 0).ifthenelse(0, fixed_tile)
-                np_mask = warp_tools.vips2numpy(tile_mask)
+            np_fixed = warp_tools.vips2numpy(fixed_tile)
+            np_moving = warp_tools.vips2numpy(moving_tile)
 
+            if self.mask is not None:
+                tile_mask = self.mask.extract_area(*tile_bbox_xywh)
+                np_mask = warp_tools.vips2numpy(tile_mask)
             else:
                 np_mask = None
 
-            np_fixed = warp_tools.vips2numpy(fixed_tile)
-            np_moving = warp_tools.vips2numpy(moving_tile)
+            if moving_tile.interpretation == "srgb":
+                # Limit registration to be inside image
+                # Warped areas outside image have the same pixel values, usually 0
+                edge_mask = 255*((np_moving.min(axis=2) != np_moving.max(axis=2)) & (np_fixed.min(axis=2) != np_fixed.max(axis=2))).astype(np.uint8)
+
+                if np_mask is not None:
+                    np_mask = 255*((edge_mask > 0) & (np_mask > 0)).astype(np.uint8)
+                else:
+                    np_mask = edge_mask
+
+
+            # Check if either of the tiles are empty
+            is_empty = fixed_tile.max() == fixed_tile.min() or moving_tile.max() == moving_tile.min()
+            if np_mask is not None:
+                is_empty = is_empty or np_mask.max() == 0
+
+            if is_empty:
+                # Nothing to register
+                empty_dxdy = pyvips.Image.black(moving_tile.width, moving_tile.height, bands=2).cast("float")
+                self.bk_dxdy_tiles[tile_idx] = empty_dxdy
+                self.fwd_dxdy_tiles[tile_idx] = empty_dxdy
+                self.pbar.update(1)
+
+                return None
 
             if self.processing_cls is not None:
                 # Process tiles #
-                fixed_normed = self.norm_image(np_fixed)
-                moving_normed = self.norm_image(np_moving)
+                fixed_processed = self.process_tile(np_fixed)
+                moving_processed = self.process_tile(np_moving)
+
             else:
 
                 if np_fixed.ndim > 2:
                     fixed_g = np.abs(1 - skcolor.rgb2gray(np_fixed))
-                    fixed_normed = util.img_as_ubyte(fixed_g)
+                    fixed_processed = util.img_as_ubyte(fixed_g)
                 else:
-                    fixed_normed = np_fixed
+                    fixed_processed = np_fixed
 
                 if np_moving.ndim > 2:
                     moving_g = np.abs(1 - skcolor.rgb2gray(np_moving))
-                    moving_normed = util.img_as_ubyte(moving_g)
+                    moving_processed = util.img_as_ubyte(moving_g)
                 else:
-                    moving_normed = np_moving
+                    moving_processed = np_moving
 
-            # Register tiles #
+            moving_normed, fixed_normed = self.norm_tiles(moving_processed, fixed_processed, np_mask)
 
+            if np_mask is not None:
+                moving_normed[np_mask == 0] = 0
+                fixed_normed[np_mask == 0] = 0
+
+            # Register tiles #
             tile_non_rigid_reg_obj = self.non_rigid_registrar_cls()
             _, _, bk_dxdy = tile_non_rigid_reg_obj.register(moving_normed, fixed_normed, mask=np_mask)
-            vips_tile_bk_dxdy = warp_tools.numpy2vips(np.dstack(bk_dxdy))
+            bk_dxdy = warp_tools.remove_invasive_displacements(bk_dxdy, M=None, src_shape_rc=None, out_shape_rc=moving_normed.shape[0:2])
+            vips_tile_bk_dxdy = warp_tools.numpy2vips(np.dstack(bk_dxdy).astype(np.float32))
 
             fwd_dxdy = warp_tools.get_inverse_field(bk_dxdy)
-            vips_tile_fwd_dxdy = warp_tools.numpy2vips(np.dstack(fwd_dxdy))
+            vips_tile_fwd_dxdy = warp_tools.numpy2vips(np.dstack(fwd_dxdy).astype(np.float32))
 
-            if self.mask is not None:
-                vips_tile_bk_dxdy = (tile_mask == 0).ifthenelse(0, vips_tile_bk_dxdy)
-                vips_tile_fwd_dxdy = (tile_mask == 0).ifthenelse(0, vips_tile_fwd_dxdy)
+            if np_mask is not None:
+                temp_tile_mask = warp_tools.numpy2vips(np_mask)
+                vips_tile_bk_dxdy = (temp_tile_mask == 0).ifthenelse(0, vips_tile_bk_dxdy)
+                vips_tile_fwd_dxdy = (temp_tile_mask == 0).ifthenelse(0, vips_tile_fwd_dxdy)
 
             self.bk_dxdy_tiles[tile_idx] = vips_tile_bk_dxdy
             self.fwd_dxdy_tiles[tile_idx] = vips_tile_fwd_dxdy
 
             self.pbar.update(1)
 
     def calc(self, *args, **kwargs):
@@ -1403,51 +1452,47 @@
 
         if self.is_array:
             shape_rc = np.array(moving_img.shape)
         else:
             shape_rc = np.array([moving_img.height, moving_img.width])
 
         self.shape = shape_rc
-        self.moving_img = moving_img
-        self.fixed_img = fixed_img
-        self.mask = mask
+
         self.non_rigid_registrar_cls = non_rigid_registrar_cls
         self.processing_cls = processing_cls
         self.target_stats = target_stats
         self.processing_kwargs = processing_kwargs
 
         if self.is_array:
             moving_img = warp_tools.numpy2vips(moving_img)
             fixed_img = warp_tools.numpy2vips(fixed_img)
             if mask is not None:
                 mask = warp_tools.numpy2vips(mask)
 
+        self.moving_img = moving_img
+        self.fixed_img = fixed_img
+        self.mask = mask
+
         temp_tile_bboxes = warp_tools.get_grid_bboxes(self.shape, self.tile_wh, self.tile_wh, inclusive=True)
         self.expanded_bboxes = np.array([warp_tools.expand_bbox(bbox_xywh, self.tile_buffer, self.shape) for bbox_xywh in temp_tile_bboxes])
-        self.moving_tiles = [moving_img.extract_area(*bbox_xywh).copy() for bbox_xywh in self.expanded_bboxes]
-        self.fixed_tiles = [fixed_img.extract_area(*bbox_xywh).copy() for bbox_xywh in self.expanded_bboxes]
 
         self.n_tiles = len(temp_tile_bboxes)
         self.bk_dxdy_tiles = [None] * self.n_tiles
         self.fwd_dxdy_tiles = [None] * self.n_tiles
         self.n_cols = len(np.unique(temp_tile_bboxes[:, 0]))
         self.n_rows = len(np.unique(temp_tile_bboxes[:, 1]))
 
-        if mask is not None:
-            self.mask_tiles = [mask.extract_area(*bbox_xywh).copy() for bbox_xywh in self.expanded_bboxes]
-        else:
-            self.mask_tiles = None
-
         bk_dxdy, fwd_dxdy = self.calc()
 
         warped_img = warp_tools.warp_img(moving_img, bk_dxdy=bk_dxdy)
         if self.is_array:
             bk_dxdy = warp_tools.vips2numpy(bk_dxdy)
             bk_dxdy = [bk_dxdy[..., 0], bk_dxdy[..., 1]]
 
             warped_img = warp_tools.vips2numpy(warped_img)
 
         self.bk_dxdy = bk_dxdy
         self.fwd_dxdy = fwd_dxdy
 
         return warped_img, fwd_dxdy, bk_dxdy
 
+
```

### Comparing `valis_wsi-1.0.0rc8/valis/preprocessing.py` & `valis_wsi-1.0.0rc9/valis/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
 Collection of pre-processing methods for aligning images
 """
-
-#import csaps
 from scipy.interpolate import Akima1DInterpolator
 from skimage import exposure, filters, measure, morphology, restoration
 import numpy as np
 import cv2
 from skimage import color as skcolor
 from . import slide_io
 import colour
@@ -322,31 +320,27 @@
         cnt_xy = np.squeeze(cnt, 1)
         on_border_idx = np.where((cnt_xy[:, 0] == 0) |
                                  (cnt_xy[:, 0] == dark_regions.shape[1]-1) |
                                  (cnt_xy[:, 1] == 0) |
                                  (cnt_xy[:, 1] == dark_regions.shape[0]-1)
                                 )[0]
 
-        if len(on_border_idx) > 0 :
+        if len(on_border_idx) > 0:
             cv2.drawContours(edge_artifact_mask, [cnt], 0, 255, -1)
 
     cam_d_t, _ = filters.threshold_multiotsu(cam_d[edge_artifact_mask == 0])
     tissue_mask = np.zeros(cam_d.shape, dtype=np.uint8)
     tissue_mask[cam_d >= cam_d_t] = 255
     tissue_mask = 255*ndimage.binary_fill_holes(tissue_mask).astype(np.uint8)
 
     concave_tissue_mask = mask2contours(tissue_mask)
 
     return tissue_mask, concave_tissue_mask
 
 
-
-
-
-
 def create_tissue_mask_from_multichannel(img):
     """
     Get foreground of multichannel imaage
     """
 
     tissue_mask = np.zeros(img.shape[:2], dtype=np.uint8)
     if img.ndim > 2:
```

### Comparing `valis_wsi-1.0.0rc8/valis/registration.py` & `valis_wsi-1.0.0rc9/valis/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """
 Classes and functions to register a collection of images
 """
 
-from ctypes import util
-from genericpath import exists
-from importlib.resources import path
-from statistics import pvariance
 import traceback
 import re
 import os
 import numpy as np
 import pathlib
-from skimage import transform, exposure, measure
+from skimage import transform, exposure
 from time import time
 import tqdm
 import pandas as pd
 import pickle
 import colour
 import pyvips
 from scipy import ndimage
@@ -28,14 +24,16 @@
 from . import preprocessing
 from . import slide_tools
 from . import slide_io
 from . import viz
 from . import warp_tools
 from . import serial_non_rigid
 
+pyvips.cache_set_max(0)
+
 # Destination directories #
 CONVERTED_IMG_DIR = "images"
 PROCESSED_IMG_DIR = "processed"
 RIGID_REG_IMG_DIR = "rigid_registration"
 NON_RIGID_REG_IMG_DIR = "non_rigid_registration"
 DEFORMATION_FIELD_IMG_DIR = "deformation_fields"
 OVERLAP_IMG_DIR = "overlaps"
@@ -58,15 +56,15 @@
 DEFAULT_AFFINE_OPTIMIZER_CLASS = None
 DEFAULT_MAX_PROCESSED_IMG_SIZE = 850
 DEFAULT_MAX_IMG_DIM = 850
 DEFAULT_THUMBNAIL_SIZE = 500
 DEFAULT_MAX_NON_RIGID_REG_SIZE = 3000
 
 # Tiled non-rigid registration arguments
-TILER_THRESH_GB = 10 # Use a tiled non-rigid registrar if saved displacement fields bigger than this
+TILER_THRESH_GB = 2
 DEFAULT_NR_TILE_WH = 512
 
 # Rigid registration kwarg keys #
 AFFINE_OPTIMIZER_KEY = "affine_optimizer"
 TRANSFORMER_KEY = "transformer"
 SIM_METRIC_KEY = "similarity_metric"
 FD_KEY = "feature_detector"
@@ -248,14 +246,22 @@
 
     _bk_dxdy_f : str
         Path to file containing bk_dxdy, if saved
 
     _fwd_dxdy_f : str
         Path to file containing fwd_dxdy, if saved
 
+    _bk_dxdy_np : ndarray
+        `bk_dxdy` as a numpy array. Only not None if `bk_dxdy` becomes
+        associated with a file
+
+    _fwd_dxdy_np : ndarray
+        `fwd_dxdy` as a numpy array. Only not None if `fwd_dxdy` becomes
+        associated with a file
+
     stored_dxdy : bool
         Whether or not the non-rigid displacements are saved in a file
         Should only occur if image is very large.
 
     fixed_slide : Slide
         Slide object to which this one was aligned.
 
@@ -336,14 +342,16 @@
         self.M = None
         self.bk_dxdy = None
         self.fwd_dxdy = None
 
         self.stored_dxdy = False
         self._bk_dxdy_f = None
         self._fwd_dxdy_f = None
+        self._bk_dxdy_np = None
+        self._fwd_dxdy_np = None
         self.processed_img_f = None
         self.rigid_reg_img_f = None
         self.non_rigid_reg_img_f = None
 
         self.fixed_slide = None
         self.xy_matched_to_prev = None
         self.xy_in_prev = None
@@ -550,30 +558,29 @@
             # IF. Get darkest pixel
             sum_img = self.image.sum(axis=2)
             bg_px = np.unravel_index(np.argmin(sum_img, axis=None), sum_img.shape)
 
         self.bg_px_pos_rc = bg_px
         self.bg_color = list(self.image[bg_px])
 
-
     def update_results_img_paths(self):
         n_digits = len(str(self.val_obj.size))
         stack_id = str.zfill(str(self.stack_idx), n_digits)
 
         self.processed_img_f = os.path.join(self.val_obj.processed_dir, self.name + ".png")
         self.rigid_reg_img_f = os.path.join(self.val_obj.reg_dst_dir, f"{stack_id}_f{self.name}.png")
         self.non_rigid_reg_img_f = os.path.join(self.val_obj.non_rigid_dst_dir, f"{stack_id}_f{self.name}.png")
         if self.stored_dxdy:
             bk_dxdy_f, fwd_dxdy_f = self.get_displacement_f()
             self._bk_dxdy_f = bk_dxdy_f
             self._fwd_dxdy_f = fwd_dxdy_f
 
     def get_displacement_f(self):
-        bk_dxdy_f = os.path.join(self.val_obj.displacements_dir, f"{self.name}_bk_dxdy.vips")
-        fwd_dxdy_f = os.path.join(self.val_obj.displacements_dir, f"{self.name}_fwd_dxdy.vips")
+        bk_dxdy_f = os.path.join(self.val_obj.displacements_dir, f"{self.name}_bk_dxdy.tiff")
+        fwd_dxdy_f = os.path.join(self.val_obj.displacements_dir, f"{self.name}_fwd_dxdy.tiff")
 
         return bk_dxdy_f, fwd_dxdy_f
 
     def get_bk_dxdy(self):
         if self.stored_dxdy:
             bk_dxdy_f, _ = self.get_displacement_f()
             return pyvips.Image.new_from_file(bk_dxdy_f)
@@ -640,23 +647,27 @@
             img = self.image
 
         if non_rigid:
             dxdy = self.bk_dxdy
         else:
             dxdy = None
 
-        if not np.all(img.shape[0:2] == self.processed_img_shape_rc):
+        if isinstance(img, pyvips.Image):
+            img_shape_rc = (img.width, img.height)
+        else:
+            img_shape_rc = img.shape[0:2]
+        if not np.all(img_shape_rc == self.processed_img_shape_rc):
             msg = ("scaling transformation for image with different shape. "
                    "However, without knowing all of other image's shapes, "
                    "the scaling may not be the same for all images, and so"
                    "may not overlap."
                    )
             valtils.print_warning(msg)
             same_shape = False
-            img_scale_rc = np.array(img.shape[0:2])/(np.array(self.processed_img_shape_rc))
+            img_scale_rc = np.array(img_shape_rc)/(np.array(self.processed_img_shape_rc))
             out_shape_rc = self.val_obj.get_aligned_slide_shape(img_scale_rc)
 
         else:
             same_shape = True
             out_shape_rc = self.reg_img_shape_rc
 
         crop_method = self.get_crop_method(crop)
@@ -1902,15 +1913,15 @@
                         rigid_reg_mask = warp_tools.rescale_img(rigid_reg_mask, scaling)
                         tissue_mask = warp_tools.rescale_img(tissue_mask, scaling)
 
                 processed_img[rigid_reg_mask == 0] = 0
 
             else:
                 tissue_mask = None
-                rigid_reg_mask = None
+                rigid_reg_mask = np.full_like(processed_img, 255)
 
             slide_obj.tissue_mask = tissue_mask
             slide_obj.rigid_reg_mask = rigid_reg_mask
             slide_obj.processed_img = processed_img
 
             processed_f_out = os.path.join(self.processed_dir, slide_obj.name + ".png")
             slide_obj.processed_img_f = processed_f_out
@@ -2381,15 +2392,15 @@
 
         return rigid_registrar
 
     def create_non_rigid_reg_mask(self):
         ref_slide = self.get_ref_slide()
         temp_non_rigid_mask = np.zeros(ref_slide.reg_img_shape_rc, dtype=np.uint8)
         for slide_obj in self.slide_dict.values():
-            rigid_mask = slide_obj.warp_img(slide_obj.tissue_mask, non_rigid=False, crop=False)
+            rigid_mask = slide_obj.warp_img(slide_obj.rigid_reg_mask, non_rigid=False, crop=False)
             temp_non_rigid_mask = cv2.bitwise_or(temp_non_rigid_mask, rigid_mask)
 
         # Draw convex hull around each region
         non_rigid_mask = 255*ndimage.binary_fill_holes(temp_non_rigid_mask).astype(np.uint8)
         non_rigid_mask = preprocessing.mask2contours(non_rigid_mask)
         for slide_obj in self.slide_dict.values():
             slide_obj.non_rigid_reg_mask = non_rigid_mask
@@ -2457,16 +2468,23 @@
             s = np.min(max_img_dim/np.array(ref_slide.processed_img_shape_rc))
             out_shape = self.get_aligned_slide_shape(s)
         else:
             # Will register full size
             out_shape = self.get_aligned_slide_shape(0)
 
         use_tiler = False
-        estimated_gb = self.size*warp_tools.calc_memory_size_gb(out_shape, 2, 64)
-        if estimated_gb >= TILER_THRESH_GB:
+        if ref_slide.reader.metadata.bf_datatype is not None:
+            np_dtype = slide_tools.BF_FORMAT_NUMPY_DTYPE[ref_slide.reader.metadata.bf_datatype]
+        else:
+            # Assuming images not read by bio-formats are RGB read using from openslide or png, jpeg, etc...
+            np_dtype = "uint8"
+
+        estimated_gb = warp_tools.calc_memory_size_gb(out_shape, ref_slide.reader.metadata.n_channels, np_dtype)
+
+        if estimated_gb > TILER_THRESH_GB:
             use_tiler = True
 
         scaled_warped_img_list = [None] * self.size
         scaled_mask_list = [None] * self.size
         img_names_list = [None] * self.size
         img_f_list = [None] * self.size
 
@@ -2487,14 +2505,19 @@
                     closest_img_level = len(slide_obj.slide_dimensions_wh) - 1
             else:
                 closest_img_level = 0
 
             vips_level_img = slide_obj.slide2vips(closest_img_level)
             img_to_warp = warp_tools.resize_img(vips_level_img, src_img_shape_rc)
 
+            if updating_non_rigid:
+                dxdy = slide_obj.bk_dxdy
+            else:
+                dxdy = None
+
             if not use_tiler:
                 # Process image using same method for rigid registration #
                 img_to_warp = warp_tools.vips2numpy(img_to_warp)
                 if slide_obj.img_type == slide_tools.IHC_NAME:
                     processing_cls = brightfield_processing_cls
                     processing_kwargs = brightfield_processing_kwargs
                 else:
@@ -2511,50 +2534,34 @@
                 processed_img = exposure.rescale_intensity(processed_img, out_range=(0, 255)).astype(np.uint8)
 
                 # Normalize images using stats collected for rigid registration #
                 normed_img = preprocessing.norm_img_stats(processed_img, self.target_processing_stats)
                 normed_img = exposure.rescale_intensity(normed_img, out_range=(0, 255)).astype(np.uint8)
 
                 # Warp image #
-                if updating_non_rigid:
-                    slide_sxy = (np.array(out_shape)/np.array(slide_obj.bk_dxdy[0].shape[0:2]))[::-1]
-                    dxdy = warp_tools.resize_img(np.dstack(slide_obj.bk_dxdy), out_shape)
-                    dxdy = [slide_sxy[0]*dxdy[..., 0], slide_sxy[1]*dxdy[..., 1]]
-                else:
-                    dxdy = None
-
-                warped_img = warp_tools.warp_img(normed_img, M=src_M,
-                                                bk_dxdy=dxdy,
-                                                out_shape_rc=out_shape)
+                warped_img = warp_tools.warp_img(img=normed_img, M=slide_obj.M,
+                                bk_dxdy=dxdy,
+                                transformation_src_shape_rc=slide_obj.processed_img_shape_rc,
+                                transformation_dst_shape_rc=slide_obj.reg_img_shape_rc,
+                                out_shape_rc=out_shape)
             if use_tiler:
                 if not warp_full_img:
-                    if isinstance(slide_obj.bk_dxdy[0], pyvips.Image):
-                        vips_dx = warp_tools.numpy2vips(slide_obj.bk_dxdy[0])
-                        vips_dy = warp_tools.numpy2vips(slide_obj.bk_dxdy[1])
-                        slide_sxy = (np.array(out_shape)/np.array([vips_dy.height, vips_dy.width]))[::-1]
-                        vips_dx = slide_sxy[0] * vips_dx
-                        vips_dy = slide_sxy[1] * vips_dy
-                        vips_dxdy = vips_dx.bandjoin(vips_dy)
-                    else:
-
-                        slide_sxy = (np.array(out_shape)/np.array(slide_obj.bk_dxdy[0].shape[0:2]))[::-1]
-                        dxdy = np.dstack([slide_sxy[0]*slide_obj.bk_dxdy[0], slide_sxy[1]*slide_obj.bk_dxdy[1]])
-                        vips_dxdy = warp_tools.numpy2vips(dxdy)
-
-                    vips_dxdy = warp_tools.resize_img(vips_dxdy, out_shape)
-                    warped_img = warp_tools.warp_img(img_to_warp, M=src_M,
-                                    bk_dxdy=vips_dxdy,
-                                    out_shape_rc=out_shape)
+                    warped_img = warp_tools.warp_img(img=img_to_warp, M=slide_obj.M,
+                                bk_dxdy=dxdy,
+                                transformation_src_shape_rc=slide_obj.processed_img_shape_rc,
+                                transformation_dst_shape_rc=slide_obj.reg_img_shape_rc,
+                                out_shape_rc=out_shape)
                 else:
                     warped_img = slide_obj.warp_slide(0, non_rigid=updating_non_rigid, crop=False)
 
             # Get mask #
+
             img_fg =  pyvips.Image.black(slide_obj.processed_img_shape_rc[1], slide_obj.processed_img_shape_rc[0]).invert()
             temp_mask = warp_tools.warp_img(img_fg, M=slide_obj.M, out_shape_rc=slide_obj.reg_img_shape_rc)
-            vips_mask = warp_tools.resize_img(temp_mask, out_shape)
+            vips_mask = warp_tools.resize_img(temp_mask, out_shape, interp_method="nearest")
 
             if use_tiler:
                 mask = vips_mask
             else:
                 mask = warp_tools.vips2numpy(vips_mask).astype(np.uint8)
 
             # Update lists
@@ -2569,17 +2576,17 @@
                     serial_non_rigid.MASK_LIST_KEY: scaled_mask_list,
                     serial_non_rigid.IMG_NAME_KEY: img_names_list
                     }
 
         if ref_slide.non_rigid_reg_mask is not None:
             if use_tiler:
                 vips_nr_mask = warp_tools.numpy2vips(ref_slide.non_rigid_reg_mask)
-                scaled_non_rigid_mask = warp_tools.resize_img(vips_nr_mask, out_shape)
+                scaled_non_rigid_mask = warp_tools.resize_img(vips_nr_mask, out_shape, interp_method="nearest")
             else:
-                scaled_non_rigid_mask = warp_tools.resize_img(ref_slide.non_rigid_reg_mask, out_shape)
+                scaled_non_rigid_mask = warp_tools.resize_img(ref_slide.non_rigid_reg_mask, out_shape, interp_method="nearest")
         else:
             scaled_non_rigid_mask = None
 
         return img_dict, max_img_dim, scaled_non_rigid_mask
 
     def non_rigid_register(self, rigid_registrar,
         brightfield_processing_cls, brightfield_processing_kwargs,
@@ -2630,27 +2637,39 @@
                                                                **self.non_rigid_reg_kwargs)
         self.end_non_rigid_time = time()
 
         for d in  [self.non_rigid_dst_dir, self.deformation_field_dir]:
             pathlib.Path(d).mkdir(exist_ok=True, parents=True)
         self.non_rigid_registrar = non_rigid_registrar
 
+        # Clean up displacements
+        for nr_name, nr_obj in non_rigid_registrar.non_rigid_obj_dict.items():
+            rigid_obj = self.rigid_registrar.img_obj_dict[nr_name]
+            cleaned_bk_dxdy = warp_tools.remove_invasive_displacements(nr_obj.bk_dxdy,
+                                                                    M=rigid_obj.M,
+                                                                    src_shape_rc=rigid_obj.image.shape[0:2],
+                                                                    out_shape_rc=rigid_obj.registered_shape_rc)
+
+            cleaned_fwd_dxdy = warp_tools.get_inverse_field(cleaned_bk_dxdy)
+            nr_obj.bk_dxdy = cleaned_bk_dxdy
+            nr_obj.fwd_dxdy = cleaned_fwd_dxdy
+
         # Draw overlap image #
         overlap_mask, overlap_mask_bbox_xywh = self.get_crop_mask(self.crop)
         overlap_mask_bbox_xywh = overlap_mask_bbox_xywh.astype(int)
         overlap_min_r = overlap_mask_bbox_xywh[1]
         overlap_min_c = overlap_mask_bbox_xywh[0]
         overlap_max_r = overlap_mask_bbox_xywh[1] + overlap_mask_bbox_xywh[3]
         overlap_max_c = overlap_mask_bbox_xywh[0] + overlap_mask_bbox_xywh[2]
 
         if self.max_processed_image_dim_px == self.max_non_rigid_registartion_dim_px:
             non_rigid_img_list = [nr_img_obj.registered_img for nr_img_obj in non_rigid_registrar.non_rigid_obj_list]
         else:
             non_rigid_img_list = [warp_tools.warp_img(img=o.image,
-                                                    M= o.M,
+                                                    M=o.M,
                                                     bk_dxdy= non_rigid_registrar.non_rigid_obj_dict[o.name].bk_dxdy,
                                                     out_shape_rc=o.registered_img.shape[0:2],
                                                     transformation_src_shape_rc=o.image.shape[0:2],
                                                     transformation_dst_shape_rc=o.registered_img.shape[0:2])
                                                 for o in rigid_registrar.img_obj_list]
 
         self.non_rigid_overlap_img  = self.draw_overlap_img(non_rigid_img_list)[overlap_min_r:overlap_max_r, overlap_min_c:overlap_max_c]
@@ -2803,84 +2822,60 @@
 
             img_T = warp_tools.get_padding_matrix(slide_obj.processed_img_shape_rc,
                                                   slide_obj.reg_img_shape_rc)
 
             prev_T = warp_tools.get_padding_matrix(prev_slide_obj.processed_img_shape_rc,
                                                    prev_slide_obj.reg_img_shape_rc)
 
-            # prev_kp_in_slide = prev_slide_obj.warp_xy(slide_obj.xy_in_prev_in_bbox,
-            #                                          M=prev_T,
-            #                                          pt_level= prev_slide_obj.processed_img_shape_rc,
-            #                                          non_rigid=False)
-
-            # current_kp_in_slide = slide_obj.warp_xy(slide_obj.xy_matched_to_prev_in_bbox,
-            #                                         M=img_T,
-            #                                         pt_level= slide_obj.processed_img_shape_rc,
-            #                                         non_rigid=False)
 
             prev_kp_in_slide = prev_slide_obj.warp_xy(slide_obj.xy_in_prev,
                                                      M=prev_T,
                                                      pt_level= prev_slide_obj.processed_img_shape_rc,
                                                      non_rigid=False)
 
             current_kp_in_slide = slide_obj.warp_xy(slide_obj.xy_matched_to_prev,
                                                     M=img_T,
                                                     pt_level= slide_obj.processed_img_shape_rc,
                                                     non_rigid=False)
 
             og_d = warp_tools.calc_d(prev_kp_in_slide, current_kp_in_slide)
+
             og_rtre = og_d/ref_diagonal
             median_og_tre = np.median(og_rtre)
             og_d *= slide_obj.resolution
             median_d_og = np.median(og_d)
 
             all_og_d[i] = median_d_og
             all_og_tre[i] = median_og_tre
 
-            # prev_warped_rigid = prev_slide_obj.warp_xy(slide_obj.xy_in_prev_in_bbox,
-            #                                            M=prev_slide_obj.M,
-            #                                            pt_level= prev_slide_obj.processed_img_shape_rc,
-            #                                            non_rigid=False)
-
-            # current_warped_rigid = slide_obj.warp_xy(slide_obj.xy_matched_to_prev_in_bbox,
-            #                                          M=slide_obj.M,
-            #                                          pt_level= slide_obj.processed_img_shape_rc,
-            #                                          non_rigid=False)
 
             prev_warped_rigid = prev_slide_obj.warp_xy(slide_obj.xy_in_prev,
                                                        M=prev_slide_obj.M,
                                                        pt_level= prev_slide_obj.processed_img_shape_rc,
                                                        non_rigid=False)
 
             current_warped_rigid = slide_obj.warp_xy(slide_obj.xy_matched_to_prev,
                                                      M=slide_obj.M,
                                                      pt_level= slide_obj.processed_img_shape_rc,
                                                      non_rigid=False)
 
+
             rigid_d = warp_tools.calc_d(prev_warped_rigid, current_warped_rigid)
             rtre = rigid_d/ref_diagonal
             median_rigid_tre = np.median(rtre)
             rigid_d *= slide_obj.resolution
             median_d_rigid = np.median(rigid_d)
 
             all_rigid_d[i] = median_d_rigid
             all_n[i] = len(rigid_d)
             all_rigid_tre[i] = median_rigid_tre
 
             if slide_obj.bk_dxdy is not None:
 
-                # prev_warped_nr = prev_slide_obj.warp_xy(slide_obj.xy_in_prev_in_bbox,
-                #                                         M=prev_slide_obj.M,
-                #                                         pt_level= prev_slide_obj.processed_img_shape_rc,
-                #                                         non_rigid=True)
-
-                # current_warped_nr = slide_obj.warp_xy(slide_obj.xy_matched_to_prev_in_bbox,
-                #                                       M=slide_obj.M,
-                #                                       pt_level= slide_obj.processed_img_shape_rc,
-                #                                       non_rigid=True)
+
                 prev_warped_nr = prev_slide_obj.warp_xy(slide_obj.xy_in_prev,
                                                         M=prev_slide_obj.M,
                                                         pt_level= prev_slide_obj.processed_img_shape_rc,
                                                         non_rigid=True)
 
                 current_warped_nr = slide_obj.warp_xy(slide_obj.xy_matched_to_prev,
                                                       M=slide_obj.M,
@@ -3186,17 +3181,22 @@
 
         img0 = nr_reg_src[serial_non_rigid.IMG_LIST_KEY][0]
         img_specific_args = None
         write_dxdy = False
 
 
         if isinstance(img0, pyvips.Image):
-            estimated_gb = self.size*warp_tools.calc_memory_size_gb([img0.width, img0.height], 2, 64)
-            if estimated_gb >= TILER_THRESH_GB:
-                msg = (f"Registered image will be larger than {TILER_THRESH_GB}Gb. "
+
+
+            np_format = str(slide_tools.VIPS_FORMAT_NUMPY_DTYPE[img0.format]().dtype)
+            estimated_gb = warp_tools.calc_memory_size_gb([img0.width, img0.height], img0.bands, np_format)
+
+
+            if estimated_gb > TILER_THRESH_GB:
+                msg = (f"Registered image will be larger than {TILER_THRESH_GB} GB. "
                        f"Will use NonRigidTileRegistrar to register cooresponding tiles, "
                        f"but this method is experimental")
 
                 valtils.print_warning(msg)
 
                 write_dxdy = True
                 img_specific_args = {}
@@ -3239,23 +3239,30 @@
         micro_reg_imgs = [None] * self.size
         for slide_obj in self.slide_dict.values():
 
             nr_obj = non_rigid_registrar.non_rigid_obj_dict[slide_obj.name]
             is_array = False
             if not isinstance(nr_obj.bk_dxdy[0], pyvips.Image):
                 is_array = True
-                new_bk_dxdy = warp_tools.numpy2vips(np.dstack(nr_obj.bk_dxdy))
-                new_fwd_dxdy = warp_tools.numpy2vips(np.dstack(nr_obj.fwd_dxdy))
+                cleaned_bk_dxdy = warp_tools.remove_invasive_displacements(nr_obj.bk_dxdy,
+                                                                    M=slide_obj.M,
+                                                                    src_shape_rc=slide_obj.processed_img_shape_rc,
+                                                                    out_shape_rc=slide_obj.reg_img_shape_rc)
+                cleaned_fwd_dxdy = warp_tools.get_inverse_field(cleaned_bk_dxdy)
+
+                new_bk_dxdy = warp_tools.numpy2vips(np.dstack(cleaned_bk_dxdy))
+                new_fwd_dxdy = warp_tools.numpy2vips(np.dstack(cleaned_fwd_dxdy))
+
             else:
                 new_bk_dxdy = nr_obj.bk_dxdy
                 new_fwd_dxdy = nr_obj.fwd_dxdy
 
             if not isinstance(slide_obj.bk_dxdy[0], pyvips.Image):
-                current_bk_dxdy = warp_tools.numpy2vips(np.dstack(slide_obj.bk_dxdy))
-                current_fwd_dxdy = warp_tools.numpy2vips(np.dstack(slide_obj.fwd_dxdy))
+                current_bk_dxdy = warp_tools.numpy2vips(np.dstack(slide_obj.bk_dxdy)).cast("float")
+                current_fwd_dxdy = warp_tools.numpy2vips(np.dstack(slide_obj.fwd_dxdy)).cast("float")
             else:
                 current_bk_dxdy = slide_obj.bk_dxdy
                 current_fwd_dxdy = slide_obj.fwd_dxdy
 
             slide_sxy = (np.array(out_shape)/np.array([current_bk_dxdy.height, current_bk_dxdy.width]))[::-1]
             if not np.all(slide_sxy == 1):
                 scaled_bk_dx = float(slide_sxy[0])*current_bk_dxdy[0]
@@ -3282,26 +3289,25 @@
                 pathlib.Path(self.displacements_dir).mkdir(exist_ok=True, parents=True)
                 slide_obj.stored_dxdy = True
 
                 bk_dxdy_f, fwd_dxdy_f = slide_obj.get_displacement_f()
                 slide_obj._bk_dxdy_f = bk_dxdy_f
                 slide_obj._fwd_dxdy_f = fwd_dxdy_f
 
-
-                updated_bk_dxdy.write_to_file(slide_obj._bk_dxdy_f)
-                updated_fwd_dxdy.write_to_file(slide_obj._fwd_dxdy_f)
-
+                updated_bk_dxdy.cast("float").tiffsave(slide_obj._bk_dxdy_f, compression="lzw", lossless=True, tile=True, bigtiff=True)
+                updated_fwd_dxdy.cast("float").tiffsave(slide_obj._fwd_dxdy_f, compression="lzw", lossless=True, tile=True, bigtiff=True)
 
             if not slide_obj.is_rgb:
                 img_to_warp = slide_obj.processed_img
             else:
                 img_to_warp = slide_obj.image
 
             micro_reg_img = slide_obj.warp_img(img_to_warp, non_rigid=True, crop=self.crop)
 
+
             img_save_id = str.zfill(str(slide_obj.stack_idx), n_digits)
             micro_fout = os.path.join(self.micro_reg_dir, f"{img_save_id}_{slide_obj.name}.png")
             micro_thumb = self.create_thumbnail(micro_reg_img)
             warp_tools.save_img(micro_fout, micro_thumb)
 
             processed_micro_reg_img = slide_obj.warp_img(slide_obj.processed_img)
             micro_reg_imgs[slide_obj.stack_idx] = processed_micro_reg_img
```

### Comparing `valis_wsi-1.0.0rc8/valis/serial_non_rigid.py` & `valis_wsi-1.0.0rc9/valis/serial_non_rigid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Classes and functions to perform serial non-rigid registration of a set of images
 
 """
 
 import numpy as np
-from skimage import io, util
+from skimage import io
 from tqdm import tqdm
 import os
 import imghdr
 from time import time
 import pathlib
 import pandas as pd
 import pickle
@@ -248,15 +248,15 @@
         Used to warp points
 
     warped_grid : ndarray
         Image showing deformation applied to a regular grid.
 
     """
 
-    def __init__(self, image, name, stack_idx, moving_xy=None, fixed_xy=None, mask=None):
+    def __init__(self, reg_obj, image, name, stack_idx, moving_xy=None, fixed_xy=None, mask=None):
         """
         Parameters
         ----------
 
         image : ndarray
             Original, unwarped image with shape (P, Q)
 
@@ -275,14 +275,15 @@
             (V, 2) array containing points in the fixed image that correspond
             to those in the moving image
 
         mask : ndarray, optional
             Mask covering area to be registered.
 
         """
+        self.reg_obj = reg_obj
         self.image = image
         self.name = name
         self.stack_idx = stack_idx
         self.moving_xy = moving_xy
         self.fixed_xy = fixed_xy
         self.registered_img = None
         self.warped_grid = None
@@ -380,14 +381,20 @@
         mask : ndarray, optional
             2D array with shape (P,Q) where non-zero pixel values are foreground,
             and 0 is background, which is ignnored during registration. If None,
             then all non-zero pixels in images will be used to create the mask.
 
         """
 
+        if self.reg_obj.from_rigid_reg:
+            rigid_img_obj = self.reg_obj.src.img_obj_dict[self.name]
+            M = rigid_img_obj.M
+            unwarped_shape = rigid_img_obj.image.shape[0:2]
+            og_reg_shape_rc = rigid_img_obj.registered_shape_rc
+
         if mask is not None:
             if self.mask is not None:
                 if isinstance(self.mask, pyvips.Image):
                     if not isinstance(mask, pyvips.Image):
                         vips_mask = warp_tools.numpy2vips(mask)
                     else:
                         vips_mask = mask
@@ -408,14 +415,21 @@
                 bk_dxdy = np.array(bk_dxdy)
 
             if self.mask is not None:
                 for_reg_dxdy = self.mask_dxdy(bk_dxdy, self.mask)
             else:
                 for_reg_dxdy = bk_dxdy
 
+            if self.reg_obj.from_rigid_reg:
+                for_reg_dxdy = warp_tools.remove_invasive_displacements(for_reg_dxdy,
+                                                                        M=M,
+                                                                        src_shape_rc=unwarped_shape,
+                                                                        out_shape_rc=og_reg_shape_rc
+                                                                        )
+
             moving_img = warp_tools.warp_img(self.image, bk_dxdy=for_reg_dxdy)
             if reg_mask is not None:
                 # Update mask too
                 reg_mask = warp_tools.warp_img(reg_mask, bk_dxdy=for_reg_dxdy)
 
         else:
             moving_img = self.image.copy()
@@ -448,14 +462,21 @@
 
         warped_moving, moving_grid_img, moving_bk_dxdy = \
             non_rigid_reg.register(moving_img=moving_img,
                                    fixed_img=registered_fixed_image,
                                    mask=reg_mask,
                                    **reg_kwargs)
 
+        if self.reg_obj.from_rigid_reg:
+            moving_bk_dxdy = warp_tools.remove_invasive_displacements(moving_bk_dxdy,
+                                                                      M=M,
+                                                                      src_shape_rc=unwarped_shape,
+                                                                      out_shape_rc=og_reg_shape_rc
+                                                                      )
+
         if not self.check_if_vips(moving_bk_dxdy):
             if self.mask is not None:
                 # Only add new transformations
                 moving_bk_dxdy = self.mask_dxdy(moving_bk_dxdy, reg_mask)
             bk_dxdy_from_ref = np.array([bk_dxdy[0] + moving_bk_dxdy[0],
                                          bk_dxdy[1] + moving_bk_dxdy[1]])
         else:
@@ -463,14 +484,20 @@
                 moving_bk_dxdy = self.mask_dxdy(moving_bk_dxdy, reg_mask)
                 bk_dxdy_from_ref = bk_dxdy + moving_bk_dxdy
 
         img_bk_dxdy = bk_dxdy_from_ref.copy()
         if self.mask is not None:
             img_bk_dxdy = self.mask_dxdy(img_bk_dxdy, self.mask)
 
+        if self.reg_obj.from_rigid_reg:
+            img_bk_dxdy = warp_tools.remove_invasive_displacements(img_bk_dxdy,
+                                                                   M=M,
+                                                                   src_shape_rc=unwarped_shape,
+                                                                   out_shape_rc=og_reg_shape_rc
+                                                                   )
         self.bk_dxdy = img_bk_dxdy
         if hasattr(non_rigid_reg, "fwd_dxdy"):
             # Already calculated
             self.fwd_dxdy = non_rigid_reg.fwd_dxdy
         else:
             self.fwd_dxdy = warp_tools.get_inverse_field(self.bk_dxdy)
 
@@ -740,31 +767,30 @@
             assert np.all(img_shape == self.shape), \
                 valtils.print_warning("Images must all have the shape")
 
             img_name = img_names[i]
             mask = mask_list[i]
             if self.mask is not None:
                 if isinstance(self.mask, pyvips.Image):
-                    combo_mask = self.mask.bandjoin(mask)
-                    mask = combo_mask.bandand()
+                    mask = self.mask.bandjoin(mask).bandand()
                 else:
                     mask = cv2.bitwise_and(self.mask, mask)
 
             moving_xy = None
             fixed_xy = None
             if moving_to_fixed_xy is not None and img_name != reference_img_f:
                 if isinstance(moving_to_fixed_xy, dict):
                     xy_coords = moving_to_fixed_xy[img_name]
                     moving_xy = xy_coords[0]
                     fixed_xy = xy_coords[1]
                 else:
                     msg = "moving_to_fixed_xy is not a dictionary. Will be ignored"
                     valtils.print_warning(msg)
 
-            nr_obj = NonRigidZImage(img, img_name, stack_idx=i,
+            nr_obj = NonRigidZImage(self, img, img_name, stack_idx=i,
                                     moving_xy=moving_xy,
                                     fixed_xy=fixed_xy,
                                     mask=mask)
 
             if i == ref_img_idx:
                 # Set reference image attributes #
                 zero_displacement = np.zeros(self.shape)
```

### Comparing `valis_wsi-1.0.0rc8/valis/serial_rigid.py` & `valis_wsi-1.0.0rc9/valis/serial_rigid.py`

 * *Files 2% similar despite different names*

```diff
@@ -629,16 +629,22 @@
         xy_to_prev = img_obj.match_dict[prev_img_obj].matched_kp1_xy
         xy_to_next = img_obj.match_dict[next_img_obj].matched_kp1_xy
 
         xy_to_prev_idx = warp_tools.index2d_to_1d(xy_to_prev[:, 1], xy_to_prev[:, 0], img_obj.image.shape[1])
         xy_to_next_idx = warp_tools.index2d_to_1d(xy_to_next[:, 1], xy_to_next[:, 0], img_obj.image.shape[1])
 
         shared_pts, nf_prev_idx, nf_next_idx  = np.intersect1d(xy_to_prev_idx, xy_to_next_idx, return_indices=True)
+        # assert np.all(xy_to_prev[nf_prev_idx, :] == xy_to_next[nf_next_idx, :])
 
-        assert np.all(xy_to_prev[nf_prev_idx, :] == xy_to_next[nf_next_idx, :])
+        #trying to remove diff features if they are different... (possible due to some very rare rounding errors?)
+        diff = np.where(xy_to_prev[nf_prev_idx, :] != xy_to_next[nf_next_idx, :])
+        if diff[0].any():
+            diff = list(np.unique(diff[0]))
+            nf_prev_idx = np.delete(nf_prev_idx, diff)
+            nf_next_idx = np.delete(nf_next_idx, diff)
 
         return nf_prev_idx, nf_next_idx
 
 
     def get_common_desc(self, current_img_obj, neighbor_obj, nf_kp_idx):
         """Get descriptors that correspond to filtered neighbor points
             Parameters
```

### Comparing `valis_wsi-1.0.0rc8/valis/slide_io.py` & `valis_wsi-1.0.0rc9/valis/slide_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Methods and classes to read and write slides in the .ome.tiff format
 
 """
 
-from csv import excel
 import os
-from skimage import util, io, transform
+from skimage import io, transform
 import pyvips
 import numpy as np
 from PIL import Image
 import pathlib
 import re
 import multiprocessing
 from joblib import Parallel, delayed, parallel_backend
@@ -28,14 +27,16 @@
 from tqdm import tqdm
 import scyjava
 
 from . import valtils
 from . import slide_tools
 from . import warp_tools
 
+pyvips.cache_set_max(0)
+
 MAX_TILE_SIZE = 2**10
 """int: maximum tile used to read or write images"""
 
 BF_RDR = "bioformats"
 """str: Name of Bioformats reader."""
 
 VIPS_RDR = "libvips"
@@ -519,15 +520,15 @@
     is_rgb : bool
         Whether or not the image is RGB.
 
     pixel_physical_size_xyu :
         Physical size per pixel and the unit.
 
     channel_names : list
-        List of channel names.
+        List of channel names. None if image is RGB
 
     n_channels : int
         Number of channels.
 
     original_xml : str
         Xml string created by bio-formats
 
@@ -833,15 +834,15 @@
             series = np.argmax(img_areas)
             msg = (f"No series provided. "
                    f"Selecting series with largest image, "
                    f"which is series {series}")
 
             valtils.print_warning(msg, warning_type=None, rgb=valtils.Fore.GREEN)
 
-        self._seris = series
+        self._series = series
         self.series = series
 
     def _set_series(self, series):
         self._series = series
         self.metadata = self.meta_list[series]
 
     def _get_series(self):
@@ -863,18 +864,18 @@
             xywh = tile_bbox_list[idx]
             # javabridge.attach()
             jpype.attachThreadToJVM()
             tile = self.slide2image(level, series, xywh=tuple(xywh))
             # javabridge.detach()
             jpype.detachThreadFromJVM()
 
-            if np.issubdtype(pixel_type, np.unsignedinteger):
-                tile = util.img_as_ubyte(tile)
+            # if np.issubdtype(pixel_type, np.unsignedinteger):
+            #     tile = util.img_as_ubyte(tile)
 
-            tile_array[idx] = slide_tools.numpy2vips(tile)
+            tile_array[idx] = slide_tools.numpy2vips(tile, self.metadata.pyvips_interpretation)
 
         n_cpu = multiprocessing.cpu_count() - 1
         with parallel_backend("threading", n_jobs=n_cpu):
             Parallel()(delayed(tile2vips_threaded)(i) for i in tqdm(range(n_tiles)))
 
         return tile_array
 
@@ -1008,17 +1009,23 @@
                 full_name = f"{temp_name}_Series_{i}"
                 full_name = full_name.replace(" ", "_")
 
                 series_meta = MetaData(full_name, slide_format, series=i)
 
                 series_meta.is_rgb = self._check_rgb(rdr)
                 series_meta.channel_names = self._get_channel_names(rdr, meta)
+                series_meta.n_channels = int(rdr.getSizeC())
                 series_meta.slide_dimensions = self._get_slide_dimensions(rdr)
+                if series_meta.is_rgb:
+                    series_meta.pyvips_interpretation = 'srgb'
+                elif series_meta.n_channels == 1:
+                    series_meta.pyvips_interpretation = 'b-w'
+                else:
+                    series_meta.pyvips_interpretation = 'multiband'
                 series_meta.pixel_physical_size_xyu = self._get_pixel_physical_size(rdr, meta)
-                series_meta.n_channels = int(rdr.getSizeC())
                 series_meta.bf_pixel_type = str(rdr.getPixelType())
                 series_meta.is_little_endian = rdr.isLittleEndian()
                 series_meta.original_xml = str(meta_xml)
                 series_meta.bf_datatype = str(FormatTools.getPixelTypeString(rdr.getPixelType()))
                 series_meta.optimal_tile_wh = int(rdr.getOptimalTileWidth())
                 meta_list[i] = series_meta
 
@@ -1284,25 +1291,26 @@
             slide_meta.n_channels = vips_img.bands - vips_img.hasalpha()
 
         slide_meta.slide_dimensions = self._get_slide_dimensions(vips_img)
         if f_extension in BF_READABLE_FORMATS:
             with valtils.HiddenPrints():
                 bf_reader = BioFormatsSlideReader(self.src_f)
 
-            slide_meta.channel_names = bf_reader.metadata.channel_names
+            slide_meta.channel_names = bf_reader.metadata.channel_names # None if RGB
+            # Need to update the n_channels based on bioformats metadata if toilet roll .ome.tiff
+            slide_meta.n_channels = bf_reader.metadata.n_channels
             slide_meta.pixel_physical_size_xyu = bf_reader.metadata.pixel_physical_size_xyu
             slide_meta.bf_pixel_type = bf_reader.metadata.bf_pixel_type
             slide_meta.is_little_endian = bf_reader.metadata.is_little_endian
             slide_meta.original_xml = bf_reader.metadata.original_xml
             slide_meta.bf_datatype = bf_reader.metadata.bf_datatype
             slide_meta.optimal_tile_wh = bf_reader.metadata.optimal_tile_wh
         else:
             slide_meta.pixel_physical_size_xyu = self._get_pixel_physical_size(vips_img)
 
-
         if slide_meta.is_rgb:
             slide_meta.channel_names = None
 
         return slide_meta
 
     def _slide2vips_ome_one_series(self, level, *args, **kwargs):
         """Use pyvips to read an ome.tiff image that has only 1 series
@@ -1339,14 +1347,15 @@
                      y in range(0, toilet_roll.height, page_height)]
 
             vips_slide = pages[0].bandjoin(pages[1:])
             if vips_slide.bands == 1:
                 vips_slide = vips_slide.copy(interpretation="b-w")
             else:
                 vips_slide = vips_slide.copy(interpretation="multiband")
+                self.metadata.n_channels = vips_slide.bands
 
         return vips_slide
 
     def slide2vips(self, level, xywh=None, *args, **kwargs):
         """Convert slide to pyvips.Image
 
         Parameters
@@ -1943,31 +1952,31 @@
 
     f_extension = slide_tools.get_slide_extension(src_f)
     what_img = imghdr.what(src_f)
     can_use_openslide = check_to_use_openslide(src_f)
     can_only_use_openslide = f_extension in OPENSLIDE_ONLY
     if can_only_use_openslide and not can_use_openslide:
         msg = (f"file {os.path.split(src_f)[1]} can only be read by OpenSlide, "
-               f"which is required to open files with the follwing extensions: {', '.join(OPENSLIDE_ONLY)}."
+               f"which is required to open files with the follwing extensions: {', '.join(OPENSLIDE_ONLY)}. "
                f"However, OpenSlide cannot be found. Unable to read this slide."
                )
 
         valtils.print_warning(msg)
 
     can_use_bf = f_extension in BF_READABLE_FORMATS and not can_only_use_openslide
     is_tiff = f_extension == ".tiff" or f_extension == ".tif"
     can_use_skimage = ".".join(f_extension.split(".")[1:]) == what_img and not is_tiff
     try:
         pyvips.Image.new_from_file(src_f)
         can_use_pyvips = True
     except:
         can_use_pyvips = False
 
-    fail_msg = f"Can't find reader to open {os.path.split(src_f)[1]}. May need to create a new one by subclassing SlideReader. Returning None"
     if not can_use_openslide and not can_use_bf and not can_use_skimage and not can_use_pyvips:
+        fail_msg = f"Can't find reader to open {os.path.split(src_f)[1]}. May need to create a new one by subclassing SlideReader. Returning None"
         valtils.print_warning(fail_msg)
 
         return None
 
     if can_use_skimage and not can_use_pyvips:
         reader = ImageReader
         return reader
```

### Comparing `valis_wsi-1.0.0rc8/valis/slide_tools.py` & `valis_wsi-1.0.0rc9/valis/slide_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import colour
 import re
 import imghdr
 from collections import Counter
 from . import warp_tools
 from . import slide_io
-from .import viz
+from . import viz
 
 IHC_NAME = "brightfield"
 IF_NAME = "fluorescence"
 MULTI_MODAL_NAME = "multi"
 TYPE_IMG_NAME = "img"
 TYPE_SLIDE_NAME = "slide"
 BG_AUTO_FILL_STR = "auto"
@@ -71,28 +71,31 @@
                      shape=[vi.height, vi.width, vi.bands])
     if vi.bands == 1:
         img = img[..., 0]
 
     return img
 
 
-def numpy2vips(a):
+def numpy2vips(a, pyvips_interpretation=None):
     """
 
     """
 
     if a.ndim > 2:
         height, width, bands = a.shape
     else:
         height, width = a.shape
         bands = 1
 
     linear = a.reshape(width * height * bands)
     vi = pyvips.Image.new_from_memory(linear.data, width, height, bands,
                                       NUMPY_FORMAT_VIPS_DTYPE[str(a.dtype)])
+    # maybe a try catch is better here, but could be slower performance-wise
+    if pyvips_interpretation is not None:
+        vi = vi.copy(interpretation=pyvips_interpretation)
     return vi
 
 
 def get_slide_extension(src_f):
     """Get slide format
 
     Parameters
```

### Comparing `valis_wsi-1.0.0rc8/valis/valtils.py` & `valis_wsi-1.0.0rc9/valis/valtils.py`

 * *Files identical despite different names*

### Comparing `valis_wsi-1.0.0rc8/valis/viz.py` & `valis_wsi-1.0.0rc9/valis/viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """Various functions used to visualize registration results
 
 """
 import colour
 import matplotlib.pyplot as plt
-from skimage import feature, draw, color, exposure, transform
+from skimage import draw, color, exposure, transform
 from scipy.cluster.hierarchy import dendrogram
 from scipy.spatial import distance
 import numpy as np
 import numba as nb
 from . import warp_tools
 import cv2
+import platform
 # JzAzBz #
 DXDY_CSPACE = "JzAzBz"
 DXDY_CRANGE = (0, 0.025)
 DXDY_LRANGE = (0.004, 0.015)
 
+if platform.system() == 'Windows' or platform.system() == 'Darwin':
+    uniTupleDtype = np.int32
+else:
+    uniTupleDtype = np.int64
+
+
 # CAM16-UCS #
 # DXDY_CSPACE = "CAM16UCS"
 # DXDY_CRANGE = (0, 0.5)
 # DXDY_LRANGE = (0.5, 0.9)
 
 
 def draw_features(kp_xy, image, n_features=500):
@@ -41,41 +48,85 @@
     for c, r in kp_xy[0:n_features].astype(np.int):
         circ_r, circ_c = draw.circle_perimeter(r, c, rad, shape=image.shape[0:2])
         feature_img[circ_r, circ_c] = np.random.randint(0, 256, 3)
 
     return feature_img
 
 
-def draw_matches(src_img, kp1_xy, dst_img, kp2_xy, alignment='horizontal'):
-    """
-    Draw all matches between src_img and dst_img, using scikit-image. Assumes they have already been filtered
+def draw_matches(src_img, kp1_xy, dst_img, kp2_xy, rad=3, alignment='horizontal'):
+    """Draw feature matches between two images
+
     Parameters
     ----------
-        src_img : ndarray
-            Image from which kp1_xy were detected
+    src_img : ndarray
+        Image associated with `kp1_xy`
+
+    kp1_xy : ndarray
+        xy coordinates of feature points found in `src_img`
 
-        kp1_xy : (N, 2) array
-            Image 1s keypoint positions, in xy coordinates,  for each of the N descriptors in desc1
+    dst_img : ndarray
+        Image associated with `kp2_xy`
 
-        dst_img : ndarray
-            Image from which kp2_xy were detected
+    kp2_xy : ndarray
+        xy coordinates of feature points found in `dst_img`
+
+    rad : int
+        Radius of circles used to draw feature points
+
+    alignment : string
+        How to stack the images, either 'veritcal' or 'horizontal'.
+
+    Returns
+    -------
+    feature_img : ndarray
+        Image show corresponding features of `src_img` and `dst_img`
 
-        kp2_xy : (M, 2) array
-            Image 1s keypoint positions, in xy coordinates,  for each of the M descriptors in desc2
     """
-    fig, ax = plt.subplots(nrows=1, ncols=1)
 
-    plt.gray()
-    match_idx = np.arange(0, len(kp1_xy))
-    matches = np.dstack([match_idx, match_idx])[0]
+    all_dims = np.array([src_img.shape, dst_img.shape])
+    out_shape = np.max(all_dims, axis=0)[0:2]
+
+    padded_src, src_T = warp_tools.pad_img(src_img, out_shape)
+    padded_dst, dst_T = warp_tools.pad_img(dst_img, out_shape)
+
+    if alignment.lower().startswith("v"):
+        feature_img = np.vstack([padded_src, padded_dst])
+        dst_xy_shift = np.array([0, out_shape[0]])
+    else:
+        feature_img = np.hstack([padded_src, padded_dst])
+        dst_xy_shift = np.array([out_shape[1], 0])
+
+    if feature_img.ndim == 2:
+        feature_img = color.gray2rgb(feature_img).astype(np.uint8)
+
+    dst_T[0:2, 2] -= dst_xy_shift
+    dst_xy_in_feature_img = warp_tools.warp_xy(kp2_xy, M=dst_T)
+
+    n_pt = np.min([kp1_xy.shape[0], kp2_xy.shape[0]])
+    cmap = (255*jzazbz_cmap()).astype(np.uint8)
+    all_color_idx = np.arange(0, cmap.shape[0])
+    colors = cmap[np.random.choice(all_color_idx, n_pt), :]
+    for i in range(n_pt):
+
+        xy1 = kp1_xy[i]
+        xy2 = dst_xy_in_feature_img[i]
+        pt_color = colors[i]
+
+        circ_rc_1 = draw.ellipse(*xy1[::-1], rad, rad, shape=feature_img.shape)
+        circ_rc_2 = draw.ellipse(*xy2[::-1], rad, rad, shape=feature_img.shape)
+        line_rc = np.array(draw.line_aa(*np.round(xy1[::-1]).astype(int), *np.round(xy2[::-1]).astype(int)))
+        line_rc[0] = np.clip(line_rc[0], 0, feature_img.shape[0]).astype(int)
+        line_rc[1] = np.clip(line_rc[1], 0, feature_img.shape[1]).astype(int)
+
+        feature_img[line_rc[0].astype(int), line_rc[1].astype(int)] = pt_color*line_rc[2][..., np.newaxis]
+        feature_img[circ_rc_1] = pt_color
+        feature_img[circ_rc_2] = pt_color
+
+    return feature_img
 
-    feature.plot_matches(ax, src_img, dst_img, kp1_xy[:, ::-1], kp2_xy[:, ::-1], matches, alignment=alignment)
-    plt.title(" ".join([str(len(kp1_xy)), "matches"]))
-    ax.axis('off')
-    plt.tight_layout()
 
 def draw_clusterd_D(D, optimal_Z):
     """Draw clustered distance matrix with dendrograms along the axes
 
     """
 
     fig = plt.figure()
@@ -99,15 +150,15 @@
     axmatrix.set_yticks([])
 
     axcolor = fig.add_axes([0.75, 0.05, 0.03, 0.798])
     plt.colorbar(im, cax=axcolor)
 
 
 # Non-rigid visualization #
-@nb.njit(nb.typeof((np.array([1]), np.array([1])))(nb.typeof((1, 1)), nb.typeof(10), nb.typeof(1)))
+@nb.njit()
 def get_grid(shape, grid_spacing, thickness=1):
     """
     Get points for a grid. Can be used to view deformation field
 
     Parameters
     ----------
     shape : (int, int)
@@ -155,15 +206,15 @@
                 if c >= 0 and c < shape[1]:
                     all_rows.append(i)
                     all_cols.append(c)
 
         if k % 2 == 0:
             col_add_idx += 1
 
-    return np.array(all_rows), np.array(all_cols)
+    return np.array(all_rows, dtype=uniTupleDtype), np.array(all_cols, dtype=uniTupleDtype)
 
 
 def jzazbz_cmap(luminosity=0.012, colorfulness=0.02, max_h=260):
     """
     Get colormap based on JzAzBz colorspace, which has good hue linearity.
     Already preceptually uniform.
 
@@ -633,15 +684,14 @@
 
     warped_hcl = [None] * 3
     for i in range(3):
         warped_hcl[i] = transform.warp(grid_img[..., i], np.array([img_warp_r, img_warp_c]))
 
     grid_img = np.dstack(warped_hcl).astype(np.uint8)
 
-
     return grid_img
 
 
 def draw_trimesh(shape_rc, tri_verts, tri_faces, thickness=2):
     """Draw a triangular mesh
     """
```

### Comparing `valis_wsi-1.0.0rc8/valis/warp_tools.py` & `valis_wsi-1.0.0rc9/valis/warp_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from logging.config import valid_ident
 import multiprocessing
 from scipy.optimize import fmin_l_bfgs_b
 from scipy import ndimage, spatial
 from shapely.ops import unary_union
 from shapely.strtree import STRtree
 from shapely.geometry import Polygon, MultiPolygon
 import matplotlib.pyplot as plt
 import numpy as np
-import skimage
 from joblib import Parallel, delayed, parallel_backend
-from skimage import draw, restoration, transform, filters
+from skimage import draw, restoration, transform, filters, morphology
 import tqdm
 import cv2
 from PIL import Image, ImageDraw
 import numpy as np
 import weightedstats
 import warnings
 import pyvips
 from interpolation.splines import UCGrid, filter_cubic, eval_cubic
 import SimpleITK as sitk
 from colorama import Fore
 import os
 import re
+from copy import deepcopy
 from . import valtils
 
+pyvips.cache_set_max(0)
+
 
 def is_pyvips_22():
     pvips_ver = pyvips.__version__.split(".")
     pyvips_22 = eval(pvips_ver[0]) >= 2 and eval(pvips_ver[1]) >= 2
     return pyvips_22
 
 
@@ -132,23 +133,184 @@
         next_idx = i
         matching_indices[idx] = (current_idx, next_idx)
         idx += 1
 
     return matching_indices
 
 
-def calc_memory_size_gb(shape, nchannels=1, bitdepth=8):
+def calc_memory_size_gb(shape, nchannels, np_dtype):
     """Estimate amount of space an image will take up, in Gb
     """
+
+    bitdepth = "".join(re.findall(r'\d+', np_dtype))
+    if len(bitdepth) > 0:
+        bitdepth = eval(bitdepth)
+    else:
+        bitdepth = 1
+
     n_px = nchannels*np.multiply(*shape)
     gb = ((n_px*8)/bitdepth)/(2**30)
 
     return gb
 
 
+def remove_invasive_displacements(bk_dxdy, M, src_shape_rc, out_shape_rc, inpaint_holes=False):
+    """Remove displacements that would distort the image edges
+    Finds areas where areas outside of the image get brought inside. Can
+    happen if displacements are combined.
+
+    Parameters
+    ----------
+    bk_dxdy : list
+        Displacement fields [x, y]
+
+    M : ndarray
+        3x3 transformation matrix
+
+    src_shape_rc : tuple
+        Shape (row, col) of the image before affine transform
+
+    Returns
+    -------
+    new_dxdy : list
+        `bk_dxdy` but with invasive displacements set to 0
+
+    """
+
+    new_dx = bk_dxdy[0].copy()
+    new_dy = bk_dxdy[1].copy()
+    if M is not None:
+        affine_mask = warp_img(np.full(src_shape_rc, 255, dtype=np.uint8), M, out_shape_rc=out_shape_rc, interp_method="nearest")
+        if not np.all(out_shape_rc == bk_dxdy[0].shape):
+            affine_mask = resize_img(affine_mask, bk_dxdy[0].shape, interp_method="nearest")
+            new_dx[affine_mask == 0] = 0
+            new_dy[affine_mask == 0] = 0
+
+    else:
+        affine_mask = np.full(out_shape_rc, 255, dtype=np.uint8)
+
+    inv_mask = 255*(affine_mask == 0).astype(np.uint8)
+    inv_nr = warp_img(inv_mask, bk_dxdy=bk_dxdy)
+    out_to_in = ((inv_nr > 0) & (affine_mask > 0))
+
+    selem = morphology.disk(3)
+    out_to_in  = morphology.binary_dilation(out_to_in, selem)
+
+    new_dy = bk_dxdy[1].copy()
+    new_dx = bk_dxdy[0].copy()
+
+    new_dx[out_to_in] = 0
+    new_dy[out_to_in] = 0
+
+    nr_img = np.round(warp_img(affine_mask, bk_dxdy=[new_dx, new_dy])).astype(np.uint8)
+
+    holes_mask = ((nr_img == 0) & (affine_mask > 0))
+    holes_mask = 255*(morphology.binary_dilation(holes_mask, selem)).astype(np.uint8)
+
+    if inpaint_holes and holes_mask.max() > 0:
+        new_dx = cv2.inpaint(new_dx.astype(np.float32), holes_mask, 3, cv2.INPAINT_TELEA)
+        new_dy = cv2.inpaint(new_dy.astype(np.float32), holes_mask, 3, cv2.INPAINT_TELEA)
+    else:
+        new_dx[holes_mask > 0] = 0
+        new_dy[holes_mask > 0] = 0
+
+    new_dxdy = np.array([new_dx, new_dy])
+
+    return new_dxdy
+
+
+# def remove_invasive_displacements(bk_dxdy, M, src_shape_rc, out_shape_rc, inpaint_holes=False):
+#     """Remove displacements that would distort the image edges
+#     Finds areas where areas outside of the image get brought inside. Can
+#     happen if displacements are combined.
+
+#     Parameters
+#     ----------
+#     bk_dxdy : list
+#         Displacement fields [x, y]
+
+#     M : ndarray
+#         3x3 transformation matrix
+
+#     src_shape_rc : tuple
+#         Shape (row, col) of the image before affine transform
+
+#     Returns
+#     -------
+#     new_dxdy : list
+#         `bk_dxdy` but with invasive displacements set to 0
+
+#     """
+
+#     cleaned_dxdy = deepcopy(bk_dxdy)
+#     if M is not None:
+#         affine_mask = warp_img(np.full(src_shape_rc, 255, dtype=np.uint8), M, out_shape_rc=out_shape_rc, interp_method="nearest")
+#         if not np.all(out_shape_rc == bk_dxdy[0].shape):
+#             affine_mask = resize_img(affine_mask, bk_dxdy[0].shape, interp_method="nearest")
+#             cleaned_dxdy[0][affine_mask == 0] = 0
+#             cleaned_dxdy[1][affine_mask == 0] = 0
+
+#     else:
+#         affine_mask = np.full(out_shape_rc, 255, dtype=np.uint8)
+
+#     # cleaned_dxdy = deepcopy(bk_dxdy)
+#     # cleaned_dxdy[0][affine_mask == 0] = 0
+#     # cleaned_dxdy[1][affine_mask == 0] = 0
+#     inv_mask = 255*(affine_mask == 0).astype(np.uint8)
+#     inv_nr = warp_img(inv_mask, bk_dxdy=bk_dxdy, interp_method="nearest")
+#     out_to_in = ((inv_nr > 0) & (affine_mask > 0))
+
+#     # warp_tools.save_img("mask_out_to_in.png", out_to_in)
+#     # warp_tools.save_img("mask_inv.png", inv_mask)
+#     # warp_tools.save_img("mask_inv_warped.png", inv_nr)
+
+#     # fwd_dxdy = get_inverse_field(bk_dxdy)
+#     # in_out_inv_warp = warp_img(out_to_in, bk_dxdy=fwd_dxdy)
+#     # in_out_inv_warp[in_out_inv_warp != 0] = 255
+
+
+#     # warp_tools.save_img("mask_out_to_in_inv.png", in_out_inv_warp)
+#     # cleaned_dxdy = deepcopy(bk_dxdy)
+#     # cleaned_dxdy[0][in_out_inv_warp > 0] = 0
+#     # cleaned_dxdy[1][in_out_inv_warp > 0] = 0
+#     holes_mask = 255*out_to_in.astype(np.uint8)
+#     new_dx = cv2.inpaint(cleaned_dxdy[0].astype(np.float32), holes_mask, 3, cv2.INPAINT_TELEA)
+#     new_dy = cv2.inpaint(cleaned_dxdy[1].astype(np.float32), holes_mask, 3, cv2.INPAINT_TELEA)
+
+#     new_dxdy = np.array([new_dx, new_dy])
+#     # warped_clean = warp_img(slide_obj.image, M, bk_dxdy=cleaned_dxdy, out_shape_rc=out_shape_rc)
+#     # warp_tools.save_img("masked_out_to_paint.png", warped_clean)
+
+#     # selem = morphology.disk(3)
+#     # out_to_in  = morphology.binary_dilation(out_to_in, selem)
+
+#     # new_dy = bk_dxdy[1].copy()
+#     # new_dx = bk_dxdy[0].copy()
+
+#     # new_dx[out_to_in] = 0
+#     # new_dy[out_to_in] = 0
+
+#     # nr_img = np.round(warp_img(affine_mask, bk_dxdy=[new_dx, new_dy])).astype(np.uint8)
+
+#     # holes_mask = ((nr_img == 0) & (affine_mask > 0))
+#     # holes_mask = 255*(morphology.binary_dilation(holes_mask, selem)).astype(np.uint8)
+
+#     # if inpaint_holes and holes_mask.max() > 0:
+#     #     new_dx = cv2.inpaint(new_dx.astype(np.float32), holes_mask, 3, cv2.INPAINT_TELEA)
+#     #     new_dy = cv2.inpaint(new_dy.astype(np.float32), holes_mask, 3, cv2.INPAINT_TELEA)
+#     # else:
+#     #     new_dx[holes_mask > 0] = 0
+#     #     new_dy[holes_mask > 0] = 0
+
+#     # new_dxdy = np.array([new_dx, new_dy])
+
+#     return new_dxdy
+
+
+
 def rescale_img(img, scaling):
     is_array = False
     if not isinstance(img, pyvips.Image):
         is_array = True
         img = numpy2vips(img)
 
     resized = img.resize(scaling)
@@ -168,15 +330,14 @@
     out_h, out_w = out_shape_rc
 
     src_shape_rc = np.array([img.height, img.width])
     sy, sx = (np.array(out_shape_rc)/src_shape_rc)
     S = [sx, 0, 0, sy]
 
     interpolator = pyvips.Interpolate.new(interp_method)
-    img = img.copy_memory()
     resized = img.affine(S,
                          oarea=[0, 0, out_w, out_h],
                          interpolate=interpolator,
                          premultiplied=True
                          )
 
     if is_array:
@@ -756,14 +917,21 @@
         a = _vips2numpy_22(vi)
     else:
         a = _vips2numpy_pre_22(vi)
 
     return a
 
 
+def pad_img(img, padded_shape):
+    padding_T = get_padding_matrix(img.shape[0:2], padded_shape)
+    padded_img = warp_img(img, padding_T, out_shape_rc=padded_shape)
+
+    return padded_img, padding_T
+
+
 def warp_img(img, M=None, bk_dxdy=None, out_shape_rc=None,
              transformation_src_shape_rc=None,
              transformation_dst_shape_rc=None,
              bbox_xywh=None,
              bg_color=None,
              interp_method="bicubic"):
     """Warp an image using rigid and/or non-rigid transformations
@@ -883,15 +1051,14 @@
         bg_color = [0] * img.bands
         bg_extender = pyvips.enums.Extend.BLACK
     else:
         bg_extender = pyvips.enums.Extend.BACKGROUND
         bg_color = list(bg_color)
 
     interpolator = pyvips.Interpolate.new(interp_method)
-    img = img.copy_memory()
     if do_rigid:
         if not np.all(src_sxy == 1):
             img_corners_xy = get_corners_of_image(src_shape_rc)[::-1]
             warped_corners = warp_xy(img_corners_xy, M=M,
                                      transformation_src_shape_rc=transformation_src_shape_rc,
                                      transformation_dst_shape_rc=transformation_dst_shape_rc,
                                      src_shape_rc=src_shape_rc,
@@ -930,28 +1097,42 @@
         if dst_sxy is not None:
             scaled_dx = float(dst_sxy[0]) * temp_dxdy[0]
             scaled_dy = float(dst_sxy[1]) * temp_dxdy[1]
             vips_dxdy = scaled_dx.bandjoin(scaled_dy)
         else:
             vips_dxdy = temp_dxdy
 
-        sim_tform = transform.SimilarityTransform(scale=dst_sxy)
-        S = sim_tform.params[0:2, 0:2].reshape(-1).tolist()
+        if dst_sxy is not None:
+            S = [dst_sxy[0], 0, 0, dst_sxy[1]]
+        else:
+            S = [1.0, 0.0, 0.0, 1.0]
+
         warp_dxdy = vips_dxdy.affine(S,
                         oarea=[0, 0, out_w, out_h],
                         interpolate=interpolator,
+                        premultiplied=True,
                         odx=-crop_x,
                         ody=-crop_y)
 
         index = pyvips.Image.xyz(affine_warped.width, affine_warped.height)
         warp_index = (index[0] + warp_dxdy[0]).bandjoin(index[1] + warp_dxdy[1])
-        warped = affine_warped.mapim(warp_index, interpolate=interpolator)
 
-        if bg_color is not None:
-            warped = (warped==0).bandand().ifthenelse(bg_color, warped)
+        try:
+            #Option to set backround color in mapim added in libvips 8.13
+            warped = affine_warped.mapim(warp_index,
+                premultiplied=True,
+                background=bg_color,
+                extend=bg_extender,
+                interpolate=interpolator)
+
+        except pyvips.error.Error:
+            warped = affine_warped.mapim(warp_index, interpolate=interpolator)
+            if bg_color is not None:
+                warped = (warped == 0).ifthenelse(bg_color, warped)
+
     else:
         warped = affine_warped
 
     if is_array:
         warped = vips2numpy(warped)
 
     return warped
@@ -1070,15 +1251,14 @@
     if return_xy:
         c1, c2 = 0, 1
     else:
         c1, c2 = 1, 0
 
     coord_map = np.array([xy_pos_in_src[c1], xy_pos_in_src[c2]])
 
-
     return coord_map
 
 
 def get_padding_matrix(img_shape_rc, out_shape_rc):
     img_h, img_w = img_shape_rc
     out_h, out_w = out_shape_rc
 
@@ -1122,15 +1302,15 @@
     :param x:
     :param y:
     :param w:
     :param h:
     :return:
     '''
 
-    ### Center smaller image inside larger image ###
+    # Center smaller image inside larger image #
     img_center_w = int(img_shape_rc[1] / 2)
     img_center_h = int(img_shape_rc[0] / 2)
 
 
     out_center_w = int(w / 2) + x
     out_center_h = int(h / 2) + y
```

### Comparing `valis_wsi-1.0.0rc8/valis_wsi.egg-info/PKG-INFO` & `valis_wsi-1.0.0rc9/valis_wsi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valis-wsi
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: A package to register whole slide images
 Home-page: https://valis.readthedocs.io/en/latest/
 Author: Chandler Gatenbee
 Author-email: Chandler.Gatenbee@moffitt.org
 Project-URL: Bug Tracker, https://github.com/MathOnco/valis/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -71,17 +71,19 @@
         * aliging each image towards the reference image following the same sequence used during rigid registation.
         * using groupwise registration that non-rigidly aligns the images to a common frame of reference. Currently this is only possible if `SimpleElastix <https://simpleelastix.github.io>`__ is installed.
 
    #. One can optionally perform a second non-rigid registration using higher resolution versions of each image. This is intended to better align micro-features not visible in the original images, and so is referred to as micro-registration
 
    #. Error is estimated by calculating the distance between registered matched features in the full resolution images.
 
-The transformations found by VALIS can then be used to warp the full resolution slides. It is also possible to merge non-RGB registered slides to create a highly multiplexed image. These aligned and/or merged slides can then be saved as ome.tiff images.
+The transformations found by VALIS can then be used to warp the full resolution slides. It is also possible to merge non-RGB registered slides to create a highly multiplexed image. These aligned and/or merged slides can then be saved as ome.tiff images. The transformations can also be use to warp point data, such as cell centroids, polygon vertices, etc...
+
+In addition to registering images, VALIS provides tools to read slides using Bio-Formats and OpenSlide, which can be read at multiple resolutions and converted to numpy arrays or pyvips.Image objects. One can also slice regions of interest from these slides. VALIS also provides functions to convert slides to the ome.tiff format, preserving the original metadata. Please see examples and documentation for more details.
+
 
-In addition to warping images and slides, VALIS can also warp point data, such as cell centoids or ROI coordinates.
 
 Full documentation can be found at `ReadTheDocs <https://valis.readthedocs.io/en/latest/>`_.
 
 .. contents:: Table of Contents
    :local:
    :depth: 1
 
@@ -578,14 +580,21 @@
     rigid_registrar, non_rigid_registrar, error_df = registrar.register()
 
     registration.kill_jvm() # Kill the JVM
 
 Change Log
 ==========
 
+Version 1.0.0rc9 (August 4, 2022)
+---------------------------------
+#. Reduced memory usage for micro-registration and warping. No longer copying memory before warping, and large displacement fields saved as .tiff images instead of .vips images.
+#. Reduced unwanted accumulation of displacements
+#. :code:`viz.draw_matches` now returns an image instead of a matplotlib pyplot
+#. Pull request 9-11 bug fixes (many thanks to crobbins327 and zindy): Not converting uint16 to uint8 when reading using Bio-Formats or pyvips; fixed rare error when filtering neighbor matches; :code:`viz.get_grid` consistent on Linux and Windows; typos.
+
 
 Version 1.0.0rc8 (July 1, 2022)
 -------------------------------
 #. Now compatible with single channel images. These images are treated as immunofluorescent images, and so custom pre-processing classes and arguments should be passed to :code:`if_processing_cls` and :code:`if_processing_kwargs` of the :code:`Valis.register` method. The current method will perform adaptive histogram equalization and scales the image to 0-255 (see :code:`preprocessing.ChannelGetter`). Also, since it isn't possible to determine if the single channel image is a greyscale RGB (light background) or single channel immunofluorescence (or similar with dark background), the background color will not be estimated, meaning that in the registered image the area outside of the warped image will be black (as opposed to the estimated background color). Tissue masks will still be created, but if it seems they are not covering enough area then try setting :code:`create_masks` to `False` when initializing the :code:`Valis` object.
 
 
 Version 1.0.0rc7 (June 27, 2022)
```

### Comparing `valis_wsi-1.0.0rc8/valis_wsi.egg-info/SOURCES.txt` & `valis_wsi-1.0.0rc9/valis_wsi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

