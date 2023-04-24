# Comparing `tmp/image_augs-1.1.5.tar.gz` & `tmp/image_augs-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-1.1.5.tar", last modified: Thu Apr  6 11:48:13 2023, max compression
+gzip compressed data, was "dist/image_augs-2.1.5.tar", last modified: Mon Apr 24 05:39:42 2023, max compression
```

## Comparing `image_augs-1.1.5.tar` & `image_augs-2.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-06 11:48:13.000000 image_augs-1.1.5/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     6945 2023-04-06 11:48:13.000000 image_augs-1.1.5/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     6365 2023-04-04 07:30:45.000000 image_augs-1.1.5/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-06 11:48:13.000000 image_augs-1.1.5/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-1.1.5/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-1.1.5/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-03-29 13:10:25.000000 image_augs-1.1.5/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-1.1.5/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-06 11:48:13.000000 image_augs-1.1.5/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     6945 2023-04-06 11:48:13.000000 image_augs-1.1.5/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      860 2023-04-06 11:48:13.000000 image_augs-1.1.5/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-06 11:48:13.000000 image_augs-1.1.5/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-06 11:48:13.000000 image_augs-1.1.5/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-06 11:48:13.000000 image_augs-1.1.5/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-06 11:48:13.000000 image_augs-1.1.5/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-1.1.5/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    16984 2023-04-06 11:47:51.000000 image_augs-1.1.5/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    22944 2023-04-04 12:48:52.000000 image_augs-1.1.5/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-1.1.5/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4350 2023-04-03 08:26:37.000000 image_augs-1.1.5/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-1.1.5/instance_seg/yml_writer_poly.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-06 11:48:13.000000 image_augs-1.1.5/object_detection_aug/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-1.1.5/object_detection_aug/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9500 2022-11-01 10:58:37.000000 image_augs-1.1.5/object_detection_aug/augmentations.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    30104 2023-03-29 06:13:27.000000 image_augs-1.1.5/object_detection_aug/combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      745 2023-03-29 11:39:36.000000 image_augs-1.1.5/object_detection_aug/config_loads.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9353 2023-03-28 07:50:19.000000 image_augs-1.1.5/object_detection_aug/converter_for_txtToYolo.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2651 2023-03-27 10:01:27.000000 image_augs-1.1.5/object_detection_aug/draw_bbox.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     1079 2022-11-01 10:58:43.000000 image_augs-1.1.5/object_detection_aug/filereads_py.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2049 2022-11-01 10:58:45.000000 image_augs-1.1.5/object_detection_aug/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     3394 2022-11-04 11:56:18.000000 image_augs-1.1.5/object_detection_aug/rotations.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4824 2023-04-03 12:07:52.000000 image_augs-1.1.5/object_detection_aug/utils_py.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-06 11:48:13.000000 image_augs-1.1.5/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-1.1.5/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:42.000000 image_augs-2.1.5/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 05:39:42.000000 image_augs-2.1.5/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.5/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:41.000000 image_augs-2.1.5/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.5/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.5/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.5/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.5/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      860 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-24 05:39:41.000000 image_augs-2.1.5/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:41.000000 image_augs-2.1.5/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.5/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.5/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.5/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.5/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.5/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.5/instance_seg/yml_writer_poly.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 05:39:42.000000 image_augs-2.1.5/object_detection_aug/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.1.5/object_detection_aug/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9500 2022-11-01 10:58:37.000000 image_augs-2.1.5/object_detection_aug/augmentations.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    30104 2023-03-29 06:13:27.000000 image_augs-2.1.5/object_detection_aug/combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      745 2023-03-29 11:39:36.000000 image_augs-2.1.5/object_detection_aug/config_loads.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9353 2023-03-28 07:50:19.000000 image_augs-2.1.5/object_detection_aug/converter_for_txtToYolo.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2651 2023-03-27 10:01:27.000000 image_augs-2.1.5/object_detection_aug/draw_bbox.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     1079 2022-11-01 10:58:43.000000 image_augs-2.1.5/object_detection_aug/filereads_py.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2049 2022-11-01 10:58:45.000000 image_augs-2.1.5/object_detection_aug/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     3394 2022-11-04 11:56:18.000000 image_augs-2.1.5/object_detection_aug/rotations.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4824 2023-04-20 13:38:06.000000 image_augs-2.1.5/object_detection_aug/utils_py.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 05:39:42.000000 image_augs-2.1.5/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.5/setup.py
```

### Comparing `image_augs-1.1.5/PKG-INFO` & `image_augs-2.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 1.1.5
+Version: 2.1.5
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -47,58 +47,85 @@
 
 **This Script is for OBJECT DETECTION**
 
 ```python
 #import these modules in your created <scriptname>.py file
 
 
-from object_detection_aug.combined import main
-from object_detection_aug.converter_for_txtToYolo import converter
+from object_detection_new.txt_reader_rect import RectAugmentation
 
 
 
-annotation_folder = 'test_objectDetection'  # YOUR ANNOTATION FOLDER NAME
-new_aug_saved_folder = 'test_object'        # AUGMENTATION SAVED FOLDER
-resize_image = 640                          # REIZE IMAGE
-test_split = 0.20                           # TEST SPLIT 
 
 
+################# image height and width combination  ##################
 
-output = converter(annotation_folder,resize_im=resize_image)
+# first combination --> for custom image size
+#  image_height = < custom image size > ; 640
+#  image_width = < custom image size > ; 320
 
-# DO YOUR DESIRED AUGMENTATION
-# IF BLUR TRUE AND BLUR_F SET TO 0.7 THEN IT WILL TAKE 50% OF YOUR TRAINNING DATA AND APPLY BLUR ON IT.
-dicc = main(folder=new_aug_saved_folder,
 
+# second combination --> keep aspect ratio of the image
+#  image_height = 640
+#  image_width  = 'keep_aspect_ratio_true'
 
-    test_split=test_split,
+# Third combination --> keeping original image height and width
+#  image_height = < keep_original_image_height >
+#  image_width = < keep_original_image_width >
 
-    blurs=True, blur_f=0.7,
 
-    noise=True, noise_f=0.6,
 
-    NB=True, NB_f=0.5,
+annotation_folder = 'your annotation folder'
+new_aug_saved_folder = 'any folder name'
+train_split = .90
+image_H = 640  #check above for height and width setting
+image_W = 'keep_aspect_ratio'
 
-    hue=True, hue_f=0.5,
 
-    sat=True, sat_f=0.5,
+rect_aug = RectAugmentation(new_aug_saved_folder)
 
-    bright=True, bright_f=0.7,
+rect_aug.Image_augmentation(annotation_folder,
+                                 
+                                train_split=train_split,
+                                 image_height= image_H,
+                                 image_width= image_W,
 
-    contrast=True , contrast_f=0.5,
 
-    rotation=True, rotation_f=0.5,
+                                 blur=True,  blur_f=0.7,
 
-    zoom=True, zoom_f=0.5,
+                                 rotate=True, rotate_f = 0.7, 
 
-    affine=True, affine_f=0.5,
+                                 noise=True, noise_f=0.8,
 
-    translation=True, translation_f=0.5,
+                                 perspective=True, perspective_f = 0.7,
 
-    vertical_flip=True, vertical_f=0.5)
+                                 affine=True, affine_f=0.7,
+
+                                 brightness=True, brightness_f=0.7,
+                                    
+                                 hue=True, hue_f=0.7,
+
+                                 removesaturation=True, removesaturation_f=0.8,
+
+                                 contrast=True, contrast_f=0.5,
+
+                                 upflip=False, upflip_f=0.5,
+
+                                 shear=True , shear_f=0.7, 
+
+                                 rotate90=True, rotate90_f =0.6,
+
+                                 blur_and_noise=True, blur_and_noise_f=0.7,
+
+                                 image_cutout = True, image_cutout_f=0.8,
+                                    
+                                 mix_aug=True, mix_aug_f=0.4,
+                                    
+                                 temperature_change=True, temperature_change_f=0.7), 
+                                
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
 ```python
```

### Comparing `image_augs-1.1.5/README.md` & `image_augs-2.1.5/image_augs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: image-augs
+Version: 2.1.5
+Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
+Author: Souvik Saha
+Author-email: ssouvik.191@gmail.com
+Keywords: machine_learning,development,data_augmentations
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Image Augmentations
 
 This is a bounding box level image augmentation tool, it can perform 14 annotations. The important ones are rotation, affine, zooming in and out, noise, and blur. The augmentations were applied to a fraction of the data (40 - 50 percent of the images out of 100 can be augmented).When rotating or zooming in and out, the bounding box coordinates will also change as the image is rotated or zoomed.
 
 ### Create a folder first, inside that folder keep your image annotation folder.
 
 ### Create a virtual environment
@@ -32,58 +47,85 @@
 
 **This Script is for OBJECT DETECTION**
 
 ```python
 #import these modules in your created <scriptname>.py file
 
 
-from object_detection_aug.combined import main
-from object_detection_aug.converter_for_txtToYolo import converter
+from object_detection_new.txt_reader_rect import RectAugmentation
+
+
+
+
+
+################# image height and width combination  ##################
+
+# first combination --> for custom image size
+#  image_height = < custom image size > ; 640
+#  image_width = < custom image size > ; 320
+
+
+# second combination --> keep aspect ratio of the image
+#  image_height = 640
+#  image_width  = 'keep_aspect_ratio_true'
 
+# Third combination --> keeping original image height and width
+#  image_height = < keep_original_image_height >
+#  image_width = < keep_original_image_width >
 
 
-annotation_folder = 'test_objectDetection'  # YOUR ANNOTATION FOLDER NAME
-new_aug_saved_folder = 'test_object'        # AUGMENTATION SAVED FOLDER
-resize_image = 640                          # REIZE IMAGE
-test_split = 0.20                           # TEST SPLIT 
 
+annotation_folder = 'your annotation folder'
+new_aug_saved_folder = 'any folder name'
+train_split = .90
+image_H = 640  #check above for height and width setting
+image_W = 'keep_aspect_ratio'
 
 
-output = converter(annotation_folder,resize_im=resize_image)
+rect_aug = RectAugmentation(new_aug_saved_folder)
 
-# DO YOUR DESIRED AUGMENTATION
-# IF BLUR TRUE AND BLUR_F SET TO 0.7 THEN IT WILL TAKE 50% OF YOUR TRAINNING DATA AND APPLY BLUR ON IT.
-dicc = main(folder=new_aug_saved_folder,
+rect_aug.Image_augmentation(annotation_folder,
+                                 
+                                train_split=train_split,
+                                 image_height= image_H,
+                                 image_width= image_W,
 
 
-    test_split=test_split,
+                                 blur=True,  blur_f=0.7,
 
-    blurs=True, blur_f=0.7,
+                                 rotate=True, rotate_f = 0.7, 
 
-    noise=True, noise_f=0.6,
+                                 noise=True, noise_f=0.8,
 
-    NB=True, NB_f=0.5,
+                                 perspective=True, perspective_f = 0.7,
 
-    hue=True, hue_f=0.5,
+                                 affine=True, affine_f=0.7,
 
-    sat=True, sat_f=0.5,
+                                 brightness=True, brightness_f=0.7,
+                                    
+                                 hue=True, hue_f=0.7,
 
-    bright=True, bright_f=0.7,
+                                 removesaturation=True, removesaturation_f=0.8,
 
-    contrast=True , contrast_f=0.5,
+                                 contrast=True, contrast_f=0.5,
 
-    rotation=True, rotation_f=0.5,
+                                 upflip=False, upflip_f=0.5,
 
-    zoom=True, zoom_f=0.5,
+                                 shear=True , shear_f=0.7, 
 
-    affine=True, affine_f=0.5,
+                                 rotate90=True, rotate90_f =0.6,
 
-    translation=True, translation_f=0.5,
+                                 blur_and_noise=True, blur_and_noise_f=0.7,
 
-    vertical_flip=True, vertical_f=0.5)
+                                 image_cutout = True, image_cutout_f=0.8,
+                                    
+                                 mix_aug=True, mix_aug_f=0.4,
+                                    
+                                 temperature_change=True, temperature_change_f=0.7), 
+                                
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
 ```python
```

### Comparing `image_augs-1.1.5/classification/classification_.py` & `image_augs-2.1.5/classification/classification_.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/classification/classification_combined.py` & `image_augs-2.1.5/classification/classification_combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/classification/logging_util.py` & `image_augs-2.1.5/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/image_augs.egg-info/PKG-INFO` & `image_augs-2.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: image-augs
-Version: 1.1.5
-Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
-Author: Souvik Saha
-Author-email: ssouvik.191@gmail.com
-Keywords: machine_learning,development,data_augmentations
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Image Augmentations
 
 This is a bounding box level image augmentation tool, it can perform 14 annotations. The important ones are rotation, affine, zooming in and out, noise, and blur. The augmentations were applied to a fraction of the data (40 - 50 percent of the images out of 100 can be augmented).When rotating or zooming in and out, the bounding box coordinates will also change as the image is rotated or zoomed.
 
 ### Create a folder first, inside that folder keep your image annotation folder.
 
 ### Create a virtual environment
@@ -47,58 +32,85 @@
 
 **This Script is for OBJECT DETECTION**
 
 ```python
 #import these modules in your created <scriptname>.py file
 
 
-from object_detection_aug.combined import main
-from object_detection_aug.converter_for_txtToYolo import converter
+from object_detection_new.txt_reader_rect import RectAugmentation
+
+
+
+
+
+################# image height and width combination  ##################
+
+# first combination --> for custom image size
+#  image_height = < custom image size > ; 640
+#  image_width = < custom image size > ; 320
+
+
+# second combination --> keep aspect ratio of the image
+#  image_height = 640
+#  image_width  = 'keep_aspect_ratio_true'
 
+# Third combination --> keeping original image height and width
+#  image_height = < keep_original_image_height >
+#  image_width = < keep_original_image_width >
 
 
-annotation_folder = 'test_objectDetection'  # YOUR ANNOTATION FOLDER NAME
-new_aug_saved_folder = 'test_object'        # AUGMENTATION SAVED FOLDER
-resize_image = 640                          # REIZE IMAGE
-test_split = 0.20                           # TEST SPLIT 
 
+annotation_folder = 'your annotation folder'
+new_aug_saved_folder = 'any folder name'
+train_split = .90
+image_H = 640  #check above for height and width setting
+image_W = 'keep_aspect_ratio'
 
 
-output = converter(annotation_folder,resize_im=resize_image)
+rect_aug = RectAugmentation(new_aug_saved_folder)
 
-# DO YOUR DESIRED AUGMENTATION
-# IF BLUR TRUE AND BLUR_F SET TO 0.7 THEN IT WILL TAKE 50% OF YOUR TRAINNING DATA AND APPLY BLUR ON IT.
-dicc = main(folder=new_aug_saved_folder,
+rect_aug.Image_augmentation(annotation_folder,
+                                 
+                                train_split=train_split,
+                                 image_height= image_H,
+                                 image_width= image_W,
 
 
-    test_split=test_split,
+                                 blur=True,  blur_f=0.7,
 
-    blurs=True, blur_f=0.7,
+                                 rotate=True, rotate_f = 0.7, 
 
-    noise=True, noise_f=0.6,
+                                 noise=True, noise_f=0.8,
 
-    NB=True, NB_f=0.5,
+                                 perspective=True, perspective_f = 0.7,
 
-    hue=True, hue_f=0.5,
+                                 affine=True, affine_f=0.7,
 
-    sat=True, sat_f=0.5,
+                                 brightness=True, brightness_f=0.7,
+                                    
+                                 hue=True, hue_f=0.7,
 
-    bright=True, bright_f=0.7,
+                                 removesaturation=True, removesaturation_f=0.8,
 
-    contrast=True , contrast_f=0.5,
+                                 contrast=True, contrast_f=0.5,
 
-    rotation=True, rotation_f=0.5,
+                                 upflip=False, upflip_f=0.5,
 
-    zoom=True, zoom_f=0.5,
+                                 shear=True , shear_f=0.7, 
 
-    affine=True, affine_f=0.5,
+                                 rotate90=True, rotate90_f =0.6,
 
-    translation=True, translation_f=0.5,
+                                 blur_and_noise=True, blur_and_noise_f=0.7,
 
-    vertical_flip=True, vertical_f=0.5)
+                                 image_cutout = True, image_cutout_f=0.8,
+                                    
+                                 mix_aug=True, mix_aug_f=0.4,
+                                    
+                                 temperature_change=True, temperature_change_f=0.7), 
+                                
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
 ```python
```

### Comparing `image_augs-1.1.5/image_augs.egg-info/SOURCES.txt` & `image_augs-2.1.5/image_augs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/instance_seg/augment_poly.py` & `image_augs-2.1.5/instance_seg/augment_poly.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,80 +43,83 @@
 
         : return :
         : new polygon points    : it will return after rotation polygon points
         : aug rotated image     : it will return rotated image
         
         '''
         try:
-            aug = iaa.Sequential([iaa.Rotate((-rotation_angle,rotation_angle),fit_output=True),
+            aug = iaa.Sequential([iaa.Rotate((-rotation_angle,rotation_angle),fit_output=False),
+                                iaa.SaltAndPepper(p=(0.01,0.06)),
+                                iaa.Multiply((0.2, 1.5), per_channel=1.0,),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_rotated_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_rotated_image
         except Exception as e:
             logger.warning(f'problem: Image rotation    desc : {e}')
         
         
-    def image_affine(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.5,1.5)) -> Tuple[Polygon,np.array]:
+    def image_affine(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.5,1.7)) -> Tuple[Polygon,np.array]:
         try:
-            aug = iaa.Sequential([iaa.Affine(scale=scale_range,fit_output=True,),
+            aug = iaa.Sequential([iaa.Affine(scale=scale_range,fit_output=False,),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image affine    desc : {e}')
 
-    def image_perspective_transform(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.03,0.09)) -> Tuple[Polygon,np.array]:
+    def image_perspective_transform(self,image:np.array,polygons:Polygon,H,W,scale_range:range=(0.10,0.17)) -> Tuple[Polygon,np.array]:
         try:
-            aug = iaa.Sequential([iaa.PerspectiveTransform(scale=scale_range,fit_output=True),
+            aug = iaa.Sequential([iaa.PerspectiveTransform(scale=scale_range,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
             logger.warning(f'problem: Image perspective transform    desc : {e}')
 
 
     def image_noise(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
-                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0,0.03)),
+                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.06)),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug = iaa.AdditiveLaplaceNoise(scale=(5,0.1*200), per_channel=True)
-                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0,0.03),per_channel=True),
+                aug = iaa.Sequential([iaa.SaltAndPepper(p=(0.01,0.06),per_channel=True),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
             logger.warning(f'problem: Image noise    desc : {e}')
 
 
     def image_blur(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
-            aug = iaa.Sequential([iaa.GaussianBlur(sigma=(0.8, 2.5)),
+            aug = iaa.Sequential([iaa.GaussianBlur(sigma=(1.2, 4.0)),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         
         except Exception as e:
             logger.warning(f'problem: Image blur    desc : {e}')
 
     
     #chnag thissssssss
     def image_hue(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             # aug = iaa.Multiply((0.5, 1.5), per_channel=0.5)
             aug = iaa.Sequential([iaa.Multiply((0.5, 1.5), per_channel=1.0,),
+                                  iaa.WithBrightnessChannels(iaa.Add((-40,40))),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image hue    desc : {e}')
 
@@ -138,14 +141,15 @@
         except Exception as e:
             logger.warning(f'problem: Image brightness    desc : {e}')
 
     def image_change_colorTemperature(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             # aug =  iaa.ChangeColorTemperature((1100, 10000))
             aug = iaa.Sequential([iaa.ChangeColorTemperature((1100, 6500)),
+                                  iaa.GaussianBlur(sigma=(1.2, 2.7)),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image color temp    desc : {e}')
 
@@ -160,15 +164,15 @@
 
         except Exception as e:
             logger.warning(f'problem: Image removeSaturation    desc : {e}')
 
     def image_contrast(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
         
-            aug = iaa.Sequential([iaa.LinearContrast((0.8, 1.4)),
+            aug = iaa.Sequential([iaa.LinearContrast((0.8, 1.7)),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
             logger.warning(f'problem: Image contrast    desc : {e}')
@@ -185,37 +189,37 @@
             logger.warning(f'problem: Image uplfip    desc : {e}')
 
     def image_shear(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 # aug =  iaa.ShearX(shear=(-12,12))
-                aug = iaa.Sequential([iaa.ShearX(shear=(-12,12),fit_output=True),
+                aug = iaa.Sequential([iaa.ShearX(shear=(-16,16),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug =  iaa.ShearY(shear=(-12,12))
-                aug = iaa.Sequential([iaa.ShearY(shear=(-12,12),fit_output=True),
+                aug = iaa.Sequential([iaa.ShearY(shear=(-16,16),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
             logger.warning(f'problem: Image shear    desc : {e}')
 
     def image_rotate90(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
                 # aug =  iaa.Rotate(rotate=90,fit_output=True)
-                aug = iaa.Sequential([iaa.Rotate(rotate=90,fit_output=True),
+                aug = iaa.Sequential([iaa.Rotate(rotate=90,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             else:
                 # aug =  iaa.Rotate(rotate=-90,fit_output=True)
-                aug = iaa.Sequential([iaa.Rotate(rotate=-90,fit_output=True),
+                aug = iaa.Sequential([iaa.Rotate(rotate=-90,fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image rotate90   desc : {e}')
             
@@ -253,65 +257,65 @@
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image cutout    desc : {e}')
     
     def blur_and_noise(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
-            aug = iaa.Sequential([iaa.GaussianBlur(sigma=(0.8, 2.5)),
+            aug = iaa.Sequential([iaa.GaussianBlur(sigma=(0.8, 3.5)),
                                 iaa.Resize({"height": H, "width": W}),
-                                iaa.SaltAndPepper(p=(0,0.03))])
+                                iaa.SaltAndPepper(p=(0.02,0.07))])
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
 
         except Exception as e:
             logger.warning(f'problem: Image blur and noise    desc : {e}')
     
     def mixed_aug_1(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
-            aug = iaa.Sequential([iaa.Affine(scale=(0.5,1.2),fit_output=True),
+            aug = iaa.Sequential([iaa.Affine(scale=(0.5,1.2),fit_output=False),
                                 iaa.Multiply((0.5, 1.5), per_channel=0.5),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Mix aug 1    desc : {e}')
     
     def mixed_aug_2(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choices = random.choice([0.4,0.5,0.6,0.7,0.8])
             # aug = iaa.RemoveSaturation(choices)
-            aug = iaa.Sequential([iaa.Rotate((-10,10),fit_output=True),
-                                iaa.WithBrightnessChannels(iaa.Add((-30,30))),
+            aug = iaa.Sequential([iaa.Rotate((-10,10),fit_output=False),
+                                iaa.WithBrightnessChannels(iaa.Add((-40,40))),
                                 iaa.RemoveSaturation(choices),
-                                iaa.PerspectiveTransform(scale=(0.03,0.09),fit_output=True),
+                                iaa.PerspectiveTransform(scale=(0.08,0.15),fit_output=False),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: mix aug 2    desc : {e}')
     
     def mixed_aug_3(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1])
             if choice == 0:
-                aug = iaa.Sequential([iaa.ShearX(shear=(-10,10),fit_output=True),
-                                    iaa.GaussianBlur(sigma=(0.8, 2.0)),
+                aug = iaa.Sequential([iaa.ShearX(shear=(-15,15),fit_output=False),
+                                    iaa.GaussianBlur(sigma=(0.8, 1.6)),
                                     iaa.ChangeColorTemperature((1100, 7000)),
                                     iaa.Resize({"height": H, "width":W})])
             
             else:
-                aug = iaa.Sequential([iaa.ShearY(shear=(-10,10),fit_output=True),
+                aug = iaa.Sequential([iaa.ShearY(shear=(-10,10),fit_output=False),
                                     iaa.LinearContrast((0.8, 1.6)),
                                     iaa.Resize({"height": H, "width":W})])
     
                             
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
@@ -322,23 +326,24 @@
     def mixed_aug_4(self,image:np.array,polygons:Polygon,H,W) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([-90,90])
             choices =  random.choice([0,1])
             
             if choices == 0:
             
-                aug = iaa.Sequential([iaa.Rotate(rotate=choice,fit_output=True),
+                aug = iaa.Sequential([iaa.Rotate(rotate=choice,fit_output=False),
                                 iaa.Multiply((0.5, 1.5), per_channel=0.5),
+                                iaa.SaltAndPepper(p=(0.01,0.06)),
                                 iaa.Resize({"height": H, "width": W})])
                 
             else:
                 
-                aug = iaa.Sequential([iaa.Rotate(rotate=choice,fit_output=True),
+                aug = iaa.Sequential([iaa.Rotate(rotate=choice,fit_output=False),
                                 iaa.WithBrightnessChannels(iaa.Add((-20,20))),
-                                iaa.SaltAndPepper(p=(0,0.03)),
+                                iaa.SaltAndPepper(p=(0.01,0.06)),
                                 iaa.Resize({"height": H, "width": W})])
             
                                 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
```

### Comparing `image_augs-1.1.5/instance_seg/json_reader_poly.py` & `image_augs-2.1.5/instance_seg/json_reader_poly.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         
         console.print(f'[bold cyan] [+] Total images : {self.len_total_images}   |   Train Split : {self.split} images   |    Test split : {self.len_total_images-self.split} images [bold cyan]')
         
         if train_split == 1.0:
                     shutil.rmtree(f'{self.aug_save_folder_name}/test')
         
         # if c value less than equal to train split then we will add those images in training data and rest will go for test data            
-        for c ,images in enumerate(track(all_images,description='Image Augmentation..',)):
+        for c ,images in enumerate(track(all_images,description='Image Augmentation..',total=len(all_images[:self.split]))):
 
             if c+1 <= self.split:
                 
                 poly = list(self.json_converter(images))
 
                 #if we want to keep original image height and width -->
                 if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
```

### Comparing `image_augs-1.1.5/instance_seg/logging_util.py` & `image_augs-2.1.5/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/instance_seg/utils_poly.py` & `image_augs-2.1.5/instance_seg/utils_poly.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
                 for ps in p: 
 
                     points.append(list(ps))
                     x , y = list(ps)
                     normalize_X = x/new_width
                     normalize_Y = y/new_height
-                    new_name += f'{normalize_X:.6f} {normalize_Y:.6f}'
+
+                    
+                    new_name += f'{normalize_X} {normalize_Y}'
                     new_name += ' '
 
                
                 with open(txt_path,'a+') as f:
                     
                     f.write(new_name)
                     f.write('\n')
```

### Comparing `image_augs-1.1.5/instance_seg/yml_writer_poly.py` & `image_augs-2.1.5/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/augmentations.py` & `image_augs-2.1.5/object_detection_aug/augmentations.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/combined.py` & `image_augs-2.1.5/object_detection_aug/combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/config_loads.py` & `image_augs-2.1.5/object_detection_aug/config_loads.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/converter_for_txtToYolo.py` & `image_augs-2.1.5/object_detection_aug/converter_for_txtToYolo.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/draw_bbox.py` & `image_augs-2.1.5/object_detection_aug/draw_bbox.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/filereads_py.py` & `image_augs-2.1.5/object_detection_aug/filereads_py.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/logging_util.py` & `image_augs-2.1.5/object_detection_aug/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/rotations.py` & `image_augs-2.1.5/object_detection_aug/rotations.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/object_detection_aug/utils_py.py` & `image_augs-2.1.5/object_detection_aug/utils_py.py`

 * *Files identical despite different names*

### Comparing `image_augs-1.1.5/setup.py` & `image_augs-2.1.5/setup.py`

 * *Files identical despite different names*

