# Comparing `tmp/SfMLearner_installable-0.3.0.tar.gz` & `tmp/SfMLearner_installable-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SfMLearner_installable-0.3.0.tar", last modified: Sun Apr 23 23:02:17 2023, max compression
+gzip compressed data, was "SfMLearner_installable-1.0.0.tar", last modified: Sun Apr 23 23:05:37 2023, max compression
```

## Comparing `SfMLearner_installable-0.3.0.tar` & `SfMLearner_installable-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 23:02:17.085056 SfMLearner_installable-0.3.0/
--rw-rw-rw-   0        0        0     1090 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     8268 2023-04-23 23:02:17.084056 SfMLearner_installable-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7533 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 23:02:17.037056 SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/
--rw-rw-rw-   0        0        0     8268 2023-04-23 23:02:16.000000 SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-23 23:02:16.000000 SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 23:02:16.000000 SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-04-23 23:02:16.000000 SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-23 23:02:16.000000 SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 23:02:17.044057 SfMLearner_installable-0.3.0/data/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:02:17.050055 SfMLearner_installable-0.3.0/data/cityscapes/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/data/cityscapes/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/data/cityscapes/cityscapes_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:02:17.060055 SfMLearner_installable-0.3.0/data/kitti/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/data/kitti/__init__.py
--rw-rw-rw-   0        0        0     6338 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/data/kitti/kitti_odom_loader.py
--rw-rw-rw-   0        0        0     6338 2023-04-23 22:42:34.000000 SfMLearner_installable-0.3.0/data/kitti/kitti_raw_loader.py
--rw-rw-rw-   0        0        0     4693 2023-04-23 22:42:35.000000 SfMLearner_installable-0.3.0/data/prepare_train_data.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:02:17.079057 SfMLearner_installable-0.3.0/kitti_eval/
--rw-rw-rw-   0        0        0        0 2023-04-23 22:42:35.000000 SfMLearner_installable-0.3.0/kitti_eval/__init__.py
--rw-rw-rw-   0        0        0     7651 2023-04-23 22:42:35.000000 SfMLearner_installable-0.3.0/kitti_eval/depth_evaluation_utils.py
--rw-rw-rw-   0        0        0     3585 2023-04-23 22:42:35.000000 SfMLearner_installable-0.3.0/kitti_eval/eval_depth.py
--rw-rw-rw-   0        0        0      989 2023-04-23 22:42:35.000000 SfMLearner_installable-0.3.0/kitti_eval/eval_pose.py
--rw-rw-rw-   0        0        0    13974 2023-04-23 22:42:35.000000 SfMLearner_installable-0.3.0/kitti_eval/pose_evaluation_utils.py
--rw-rw-rw-   0        0        0       42 2023-04-23 23:02:17.086058 SfMLearner_installable-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-04-23 23:01:29.000000 SfMLearner_installable-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:05:37.002357 SfMLearner_installable-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     8268 2023-04-23 23:05:37.000355 SfMLearner_installable-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7533 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.900357 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/
+-rw-rw-rw-   0        0        0     8268 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-23 23:05:36.000000 SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.906356 SfMLearner_installable-1.0.0/data/
+-rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.959355 SfMLearner_installable-1.0.0/data/cityscapes/
+-rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/cityscapes/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/cityscapes/cityscapes_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.981358 SfMLearner_installable-1.0.0/data/kitti/
+-rw-rw-rw-   0        0        0        0 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/kitti/__init__.py
+-rw-rw-rw-   0        0        0     6338 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/kitti/kitti_odom_loader.py
+-rw-rw-rw-   0        0        0     6338 2023-04-23 22:42:34.000000 SfMLearner_installable-1.0.0/data/kitti/kitti_raw_loader.py
+-rw-rw-rw-   0        0        0     4693 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/data/prepare_train_data.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:05:36.997360 SfMLearner_installable-1.0.0/kitti_eval/
+-rw-rw-rw-   0        0        0        0 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/__init__.py
+-rw-rw-rw-   0        0        0     7651 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/depth_evaluation_utils.py
+-rw-rw-rw-   0        0        0     3585 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/eval_depth.py
+-rw-rw-rw-   0        0        0      989 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/eval_pose.py
+-rw-rw-rw-   0        0        0    13974 2023-04-23 22:42:35.000000 SfMLearner_installable-1.0.0/kitti_eval/pose_evaluation_utils.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 23:05:37.002357 SfMLearner_installable-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     3944 2023-04-23 23:05:31.000000 SfMLearner_installable-1.0.0/setup.py
```

### Comparing `SfMLearner_installable-0.3.0/LICENSE` & `SfMLearner_installable-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/PKG-INFO` & `SfMLearner_installable-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SfMLearner_installable
-Version: 0.3.0
+Version: 1.0.0
 Summary: Fork of the original SfMLearner with a setup.py file for installation with pip.
 Home-page: https://github.com/topher097/SfMLearner_installable
 Author: Christopher Endres
 Author-email: cmendres400@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `SfMLearner_installable-0.3.0/README.md` & `SfMLearner_installable-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/PKG-INFO` & `SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SfMLearner-installable
-Version: 0.3.0
+Version: 1.0.0
 Summary: Fork of the original SfMLearner with a setup.py file for installation with pip.
 Home-page: https://github.com/topher097/SfMLearner_installable
 Author: Christopher Endres
 Author-email: cmendres400@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `SfMLearner_installable-0.3.0/SfMLearner_installable.egg-info/SOURCES.txt` & `SfMLearner_installable-1.0.0/SfMLearner_installable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/data/cityscapes/cityscapes_loader.py` & `SfMLearner_installable-1.0.0/data/cityscapes/cityscapes_loader.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/data/kitti/kitti_odom_loader.py` & `SfMLearner_installable-1.0.0/data/kitti/kitti_odom_loader.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/data/kitti/kitti_raw_loader.py` & `SfMLearner_installable-1.0.0/data/kitti/kitti_raw_loader.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/data/prepare_train_data.py` & `SfMLearner_installable-1.0.0/data/prepare_train_data.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/kitti_eval/depth_evaluation_utils.py` & `SfMLearner_installable-1.0.0/kitti_eval/depth_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/kitti_eval/eval_depth.py` & `SfMLearner_installable-1.0.0/kitti_eval/eval_depth.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/kitti_eval/eval_pose.py` & `SfMLearner_installable-1.0.0/kitti_eval/eval_pose.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/kitti_eval/pose_evaluation_utils.py` & `SfMLearner_installable-1.0.0/kitti_eval/pose_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `SfMLearner_installable-0.3.0/setup.py` & `SfMLearner_installable-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'SfMLearner_installable'
 DESCRIPTION = 'Fork of the original SfMLearner with a setup.py file for installation with pip.'
 URL = 'https://github.com/topher097/SfMLearner_installable'
 EMAIL = 'cmendres400@gmail.com'
 AUTHOR = 'Christopher Endres'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.0'
+VERSION = '1.0.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'joblib == 1.2.0', 
     'matplotlib == 3.7.1', 
     'numpy == 1.24.3' , 
     'Pillow == 9.5.0',
```

