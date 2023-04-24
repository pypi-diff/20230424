# Comparing `tmp/image_augs-2.1.5.tar.gz` & `tmp/image_augs-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-2.1.5.tar", last modified: Mon Apr 24 05:39:42 2023, max compression
+gzip compressed data, was "dist/image_augs-2.1.6.tar", last modified: Mon Apr 24 09:37:12 2023, max compression
```

## Comparing `image_augs-2.1.5.tar` & `image_augs-2.1.6.tar`

### file list

```diff
@@ -1,34 +1,23 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:42.000000 image_augs-2.1.5/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 05:39:42.000000 image_augs-2.1.5/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.5/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:41.000000 image_augs-2.1.5/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.5/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.5/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.5/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.5/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      860 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:41.000000 image_augs-2.1.5/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.5/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.5/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.5/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.5/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.5/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.5/instance_seg/yml_writer_poly.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:42.000000 image_augs-2.1.5/object_detection_aug/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.1.5/object_detection_aug/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9500 2022-11-01 10:58:37.000000 image_augs-2.1.5/object_detection_aug/augmentations.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    30104 2023-03-29 06:13:27.000000 image_augs-2.1.5/object_detection_aug/combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      745 2023-03-29 11:39:36.000000 image_augs-2.1.5/object_detection_aug/config_loads.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9353 2023-03-28 07:50:19.000000 image_augs-2.1.5/object_detection_aug/converter_for_txtToYolo.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2651 2023-03-27 10:01:27.000000 image_augs-2.1.5/object_detection_aug/draw_bbox.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     1079 2022-11-01 10:58:43.000000 image_augs-2.1.5/object_detection_aug/filereads_py.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2049 2022-11-01 10:58:45.000000 image_augs-2.1.5/object_detection_aug/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     3394 2022-11-04 11:56:18.000000 image_augs-2.1.5/object_detection_aug/rotations.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4824 2023-04-20 13:38:06.000000 image_augs-2.1.5/object_detection_aug/utils_py.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 05:39:42.000000 image_augs-2.1.5/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.5/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:37:12.000000 image_augs-2.1.6/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.6/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.6/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.6/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.6/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.6/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      496 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       28 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.6/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.6/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.6/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.6/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.6/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.6/instance_seg/yml_writer_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 09:37:12.000000 image_augs-2.1.6/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.6/setup.py
```

### Comparing `image_augs-2.1.5/PKG-INFO` & `image_augs-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 2.1.5
+Version: 2.1.6
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.1.5/README.md` & `image_augs-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/classification/classification_.py` & `image_augs-2.1.6/classification/classification_.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/classification/classification_combined.py` & `image_augs-2.1.6/classification/classification_combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/classification/logging_util.py` & `image_augs-2.1.6/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/image_augs.egg-info/PKG-INFO` & `image_augs-2.1.6/image_augs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-augs
-Version: 2.1.5
+Version: 2.1.6
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.1.5/instance_seg/augment_poly.py` & `image_augs-2.1.6/instance_seg/augment_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/instance_seg/json_reader_poly.py` & `image_augs-2.1.6/instance_seg/json_reader_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/instance_seg/logging_util.py` & `image_augs-2.1.6/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/instance_seg/utils_poly.py` & `image_augs-2.1.6/instance_seg/utils_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/instance_seg/yml_writer_poly.py` & `image_augs-2.1.6/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.5/setup.py` & `image_augs-2.1.6/setup.py`

 * *Files identical despite different names*

