# Comparing `tmp/xmipp_metadata-1.0.8.tar.gz` & `tmp/xmipp_metadata-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmipp_metadata-1.0.8.tar", last modified: Wed Apr 19 08:14:13 2023, max compression
+gzip compressed data, was "xmipp_metadata-1.0.9.tar", last modified: Mon Apr 24 15:14:02 2023, max compression
```

## Comparing `xmipp_metadata-1.0.8.tar` & `xmipp_metadata-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.299775 xmipp_metadata-1.0.8/xmipp_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_em.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3039 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_mrc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9178 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/metadata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9142 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/metadata/xmipp_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/test_image_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.299775 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:14:02.744038 xmipp_metadata-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-24 15:14:02.740038 xmipp_metadata-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:14:02.744038 xmipp_metadata-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:14:02.740038 xmipp_metadata-1.0.9/xmipp_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:14:02.740038 xmipp_metadata-1.0.9/xmipp_metadata/image_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/image_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_em.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16662 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3039 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_mrc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9178 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:14:02.740038 xmipp_metadata-1.0.9/xmipp_metadata/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/metadata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9142 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/metadata/xmipp_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:14:02.740038 xmipp_metadata-1.0.9/xmipp_metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/tests/test_image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-24 15:13:26.000000 xmipp_metadata-1.0.9/xmipp_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:14:02.740038 xmipp_metadata-1.0.9/xmipp_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-24 15:14:02.000000 xmipp_metadata-1.0.9/xmipp_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-24 15:14:02.000000 xmipp_metadata-1.0.9/xmipp_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:14:02.000000 xmipp_metadata-1.0.9/xmipp_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 15:14:02.000000 xmipp_metadata-1.0.9/xmipp_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 15:14:02.000000 xmipp_metadata-1.0.9/xmipp_metadata.egg-info/top_level.txt
```

### Comparing `xmipp_metadata-1.0.8/LICENSE` & `xmipp_metadata-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/PKG-INFO` & `xmipp_metadata-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: xmipp_metadata
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package to handle Xmipp Metadata and image binary data
 Home-page: https://github.com/DavidHerreros/xmipp_metadata
 Author: David Herreros
 Author-email: dherreros@cnb.csic.es
 License: UNKNOWN
 Description: =======================
         Xmipp Metadata Handler
```

### Comparing `xmipp_metadata-1.0.8/README.rst` & `xmipp_metadata-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/setup.py` & `xmipp_metadata-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/__init__.py` & `xmipp_metadata-1.0.9/xmipp_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/__init__.py` & `xmipp_metadata-1.0.9/xmipp_metadata/image_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_em.py` & `xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_em.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_handler.py` & `xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from pathlib import Path
 
 import numpy as np
 
 from skimage.transform import rescale, resize, warp
 from skimage import filters
 from skimage.measure import label
+from skimage.morphology import opening, ball
 
 import morphsnakes as ms
 
 from scipy.ndimage.filters import gaussian_filter, median_filter
 
 from .image_mrc import ImageMRC
 
@@ -300,15 +301,15 @@
         self.read(input_file)
         data = np.squeeze(self.getData())
         noise = np.random.normal(loc=avg, scale=std, size=data.shape)
         data_noise = data + noise
         self.write(data_noise, output_file, overwrite=overwrite, sr=self.getSamplingRate())
 
     def generateMask(self, iterations=150, smoothing=0, lambda1=1, lambda2=2, std=1, boxsize=128,
-                     smoothStairEdges=False, keep_largest=True):
+                     smoothStairEdges=False, keep_largest=True, dust_size=None):
         '''Generate automatically a binary protein mask based on a combination of snakes and
         Otsu method.
             :param int iterations: Number of iterations for computing the snake mask.
             :param int smoothing: Number of times the smoothing operator is applied per iteration.
                                   Reasonable values are around 0-4. Larger values lead to smoother
                                   segmentations.
             :param int lambda1: Weight parameter for the outer region. If `lambda1` is larger than
@@ -358,14 +359,24 @@
             acwe_ls1 = labels == np.argmax(np.bincount(labels.flat)[1:]) + 1
 
         # Upscale mask (if downscaling was applied)
         if boxsize is not None:
             finalDimension = ori_boxsize * np.ones(len(data.shape))
             acwe_ls1 = resize(acwe_ls1.astype(bool), finalDimension).astype(np.float32)
 
+        # Remove dust
+        if dust_size is not None:
+            acwe_ls1 = opening(acwe_ls1.astype(bool), ball(5))
+            labels = label(acwe_ls1)
+            assert (labels.max() != 0)  # assume at least 1 CC
+            keep_regions = (np.argwhere(np.bincount(labels.flat)[1:] > dust_size) + 1)
+            aux = np.zeros(acwe_ls1.shape)
+            for lid in keep_regions:
+                aux += labels == lid
+            acwe_ls1 = aux.astype(np.float32)
 
         if smoothStairEdges:
             acwe_ls1 = (median_filter(acwe_ls1, size=5) >= 0.001).astype(np.float32)
 
         data_ori = data_ori * acwe_ls1
         acwe_ls1 = (data_ori >= filters.threshold_otsu(data_ori)).astype(np.float32)
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_mrc.py` & `xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_mrc.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_spider.py` & `xmipp_metadata-1.0.9/xmipp_metadata/image_handler/image_spider.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/metadata/__init__.py` & `xmipp_metadata-1.0.9/xmipp_metadata/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/metadata/xmipp_metadata.py` & `xmipp_metadata-1.0.9/xmipp_metadata/metadata/xmipp_metadata.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/tests/test_image_handler.py` & `xmipp_metadata-1.0.9/xmipp_metadata/tests/test_image_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,11 +203,12 @@
                         os.path.join("test_outputs", "test_tr.vol"),
                         avg=0.0, std=0.2, overwrite=True)
 
 
 # Generate mask (VOL)
 ih = ImageHandler(os.path.join("test_outputs", "test_tr.vol"))
 start_time = time.time()
-mask = ih.generateMask(iterations=50, boxsize=64, smoothStairEdges=False)
+mask = ih.generateMask(iterations=50, boxsize=64, smoothStairEdges=False, dust_size=50)
 end_time = time.time()
 print(end_time - start_time)
-ih.write(mask, os.path.join("test_outputs", "test_generated_mask.vol"), sr=2.0)
+ih.write(mask, os.path.join("test_outputs", "test_generated_mask.vol"), sr=ih.getSamplingRate())
+ih.write(ih.getData() * mask, os.path.join("test_outputs", "test_generated_masked.vol"), sr=ih.getSamplingRate())
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/tests/test_metadata.py` & `xmipp_metadata-1.0.9/xmipp_metadata/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/utils.py` & `xmipp_metadata-1.0.9/xmipp_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata.egg-info/PKG-INFO` & `xmipp_metadata-1.0.9/xmipp_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: xmipp-metadata
-Version: 1.0.8
+Version: 1.0.9
 Summary: Package to handle Xmipp Metadata and image binary data
 Home-page: https://github.com/DavidHerreros/xmipp_metadata
 Author: David Herreros
 Author-email: dherreros@cnb.csic.es
 License: UNKNOWN
 Description: =======================
         Xmipp Metadata Handler
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata.egg-info/SOURCES.txt` & `xmipp_metadata-1.0.9/xmipp_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

