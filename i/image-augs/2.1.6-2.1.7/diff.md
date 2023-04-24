# Comparing `tmp/image_augs-2.1.6.tar.gz` & `tmp/image_augs-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-2.1.6.tar", last modified: Mon Apr 24 09:37:12 2023, max compression
+gzip compressed data, was "dist/image_augs-2.1.7.tar", last modified: Mon Apr 24 09:58:14 2023, max compression
```

## Comparing `image_augs-2.1.6.tar` & `image_augs-2.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:37:12.000000 image_augs-2.1.6/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.6/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.6/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.6/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.6/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.6/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      496 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       28 2023-04-24 09:37:11.000000 image_augs-2.1.6/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:37:12.000000 image_augs-2.1.6/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.6/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.6/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.6/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.6/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.6/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.6/instance_seg/yml_writer_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 09:37:12.000000 image_augs-2.1.6/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.6/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:58:14.000000 image_augs-2.1.7/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.7/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.7/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.7/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.7/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.7/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      496 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       28 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.7/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.7/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.7/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.7/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.7/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.7/instance_seg/yml_writer_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 09:58:14.000000 image_augs-2.1.7/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.7/setup.py
```

### Comparing `image_augs-2.1.6/PKG-INFO` & `image_augs-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 2.1.6
+Version: 2.1.7
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.1.6/README.md` & `image_augs-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/classification/classification_.py` & `image_augs-2.1.7/classification/classification_.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/classification/classification_combined.py` & `image_augs-2.1.7/classification/classification_combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/classification/logging_util.py` & `image_augs-2.1.7/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/image_augs.egg-info/PKG-INFO` & `image_augs-2.1.7/image_augs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-augs
-Version: 2.1.6
+Version: 2.1.7
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.1.6/instance_seg/augment_poly.py` & `image_augs-2.1.7/instance_seg/augment_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/instance_seg/json_reader_poly.py` & `image_augs-2.1.7/instance_seg/json_reader_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/instance_seg/logging_util.py` & `image_augs-2.1.7/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/instance_seg/utils_poly.py` & `image_augs-2.1.7/instance_seg/utils_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/instance_seg/yml_writer_poly.py` & `image_augs-2.1.7/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.6/setup.py` & `image_augs-2.1.7/setup.py`

 * *Files identical despite different names*

