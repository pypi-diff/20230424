# Comparing `tmp/miso2-2.5.6.tar.gz` & `tmp/miso2-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miso2-2.5.6.tar", last modified: Tue Dec 13 10:28:48 2022, max compression
+gzip compressed data, was "miso2-3.0.0.tar", last modified: Mon Apr 24 08:19:48 2023, max compression
```

## Comparing `miso2-2.5.6.tar` & `miso2-3.0.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:48.095005 miso2-2.5.6/
--rw-rw-rw-   0        0        0     1062 2022-03-10 10:07:02.000000 miso2-2.5.6/LICENCE.txt
--rw-rw-rw-   0        0        0      875 2022-12-13 10:28:48.093980 miso2-2.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      195 2022-03-10 10:07:02.000000 miso2-2.5.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:47.838314 miso2-2.5.6/miso/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/__init__.py
--rw-rw-rw-   0        0        0     2257 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:47.906269 miso2-2.5.6/miso/data/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/__init__.py
--rw-rw-rw-   0        0        0     2829 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/dataset.py
--rw-rw-rw-   0        0        0     1610 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/download.py
--rw-rw-rw-   0        0        0     7520 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/filenames_dataset.py
--rw-rw-rw-   0        0        0     3213 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/image_dataset.py
--rw-rw-rw-   0        0        0     2651 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/image_loader.py
--rw-rw-rw-   0        0        0     4074 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/image_utils.py
--rw-rw-rw-   0        0        0     8146 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/tf_generator.py
--rw-rw-rw-   0        0        0     5479 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/training_dataset.py
--rw-rw-rw-   0        0        0     3565 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/data/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:47.933595 miso2-2.5.6/miso/deploy/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/deploy/__init__.py
--rw-rw-rw-   0        0        0     5993 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/deploy/inference.py
--rw-rw-rw-   0        0        0     6285 2022-11-30 13:38:25.000000 miso2-2.5.6/miso/deploy/model_info.py
--rw-rw-rw-   0        0        0     8391 2022-10-09 23:22:54.000000 miso2-2.5.6/miso/deploy/saving.py
--rw-rw-rw-   0        0        0     5275 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/deploy/server.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:47.970107 miso2-2.5.6/miso/layers/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/__init__.py
--rw-rw-rw-   0        0        0     4432 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/_common_blocks.py
--rw-rw-rw-   0        0        0     2127 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/asoftmax.py
--rw-rw-rw-   0        0        0     2904 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/batch_instance_normalisation.py
--rw-rw-rw-   0        0        0     3386 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/cyclic.py
--rw-rw-rw-   0        0        0     8188 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/group_normalisation.py
--rw-rw-rw-   0        0        0     2546 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/layers/msoftmax.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:47.998641 miso2-2.5.6/miso/models/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/models/__init__.py
--rw-rw-rw-   0        0        0     4596 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/models/base_cyclic.py
--rw-rw-rw-   0        0        0     5798 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/models/factory.py
--rw-rw-rw-   0        0        0       56 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/models/model_zoo.py
--rw-rw-rw-   0        0        0    13297 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/models/resnet_cyclic.py
--rw-rw-rw-   0        0        0     4884 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/models/transfer_learning.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:48.033666 miso2-2.5.6/miso/stats/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/__init__.py
--rw-rw-rw-   0        0        0     1490 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/accuracy.py
--rw-rw-rw-   0        0        0    14013 2022-04-29 12:22:30.000000 miso2-2.5.6/miso/stats/confusion_matrix.py
--rw-rw-rw-   0        0        0     6294 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/embedding.py
--rw-rw-rw-   0        0        0     4983 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/mislabelling.py
--rw-rw-rw-   0        0        0      909 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/most_representative.py
--rw-rw-rw-   0        0        0     1496 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/projections.py
--rw-rw-rw-   0        0        0      993 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/stats/training.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:48.060970 miso2-2.5.6/miso/training/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/training/__init__.py
--rw-rw-rw-   0        0        0     5042 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/training/adaptive_learning_rate.py
--rw-rw-rw-   0        0        0     3282 2022-10-07 22:59:01.000000 miso2-2.5.6/miso/training/parameters.py
--rw-rw-rw-   0        0        0     5374 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/training/tf_augmentation.py
--rw-rw-rw-   0        0        0    25489 2022-11-30 13:58:59.000000 miso2-2.5.6/miso/training/trainer.py
--rw-rw-rw-   0        0        0     1757 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/training/training_result.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:48.092460 miso2-2.5.6/miso/utils/
--rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/utils/__init__.py
--rw-rw-rw-   0        0        0    10218 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/utils/flowcam.py
--rw-rw-rw-   0        0        0      757 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/utils/lock.py
--rw-rw-rw-   0        0        0      227 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/utils/misc.py
--rw-rw-rw-   0        0        0     1455 2022-08-11 23:05:55.000000 miso2-2.5.6/miso/utils/rolling_buffer.py
--rw-rw-rw-   0        0        0     5300 2022-11-22 03:13:42.000000 miso2-2.5.6/miso/utils/singleton.py
--rw-rw-rw-   0        0        0    10056 2022-03-10 10:07:02.000000 miso2-2.5.6/miso/utils/wave.py
-drwxrwxrwx   0        0        0        0 2022-12-13 10:28:47.852269 miso2-2.5.6/miso2.egg-info/
--rw-rw-rw-   0        0        0      875 2022-12-13 10:28:47.000000 miso2-2.5.6/miso2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2022-12-13 10:28:47.000000 miso2-2.5.6/miso2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-13 10:28:47.000000 miso2-2.5.6/miso2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2022-12-13 10:28:47.000000 miso2-2.5.6/miso2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-13 10:28:47.000000 miso2-2.5.6/miso2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-13 10:28:48.095005 miso2-2.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1799 2022-12-13 10:27:59.000000 miso2-2.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.539449 miso2-3.0.0/
+-rw-rw-rw-   0        0        0     1062 2022-03-10 10:07:02.000000 miso2-3.0.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      875 2023-04-24 08:19:48.539449 miso2-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2022-03-10 10:07:02.000000 miso2-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.217083 miso2-3.0.0/miso/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/__init__.py
+-rw-rw-rw-   0        0        0     2257 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.311788 miso2-3.0.0/miso/data/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/__init__.py
+-rw-rw-rw-   0        0        0     2829 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/dataset.py
+-rw-rw-rw-   0        0        0     1610 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/download.py
+-rw-rw-rw-   0        0        0     7520 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/filenames_dataset.py
+-rw-rw-rw-   0        0        0     3213 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/image_dataset.py
+-rw-rw-rw-   0        0        0     2651 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/image_loader.py
+-rw-rw-rw-   0        0        0     4074 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/image_utils.py
+-rw-rw-rw-   0        0        0     8146 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/tf_generator.py
+-rw-rw-rw-   0        0        0     5479 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/training_dataset.py
+-rw-rw-rw-   0        0        0     3565 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.345825 miso2-3.0.0/miso/deploy/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/deploy/__init__.py
+-rw-rw-rw-   0        0        0     5993 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/deploy/inference.py
+-rw-rw-rw-   0        0        0     6285 2022-11-30 13:38:25.000000 miso2-3.0.0/miso/deploy/model_info.py
+-rw-rw-rw-   0        0        0     8391 2022-10-09 23:22:54.000000 miso2-3.0.0/miso/deploy/saving.py
+-rw-rw-rw-   0        0        0     5275 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/deploy/server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.391867 miso2-3.0.0/miso/layers/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/__init__.py
+-rw-rw-rw-   0        0        0     4432 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/_common_blocks.py
+-rw-rw-rw-   0        0        0     2127 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/asoftmax.py
+-rw-rw-rw-   0        0        0     2904 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/batch_instance_normalisation.py
+-rw-rw-rw-   0        0        0     3386 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/cyclic.py
+-rw-rw-rw-   0        0        0     8188 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/group_normalisation.py
+-rw-rw-rw-   0        0        0     2546 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/layers/msoftmax.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.426001 miso2-3.0.0/miso/models/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/models/__init__.py
+-rw-rw-rw-   0        0        0     4596 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/models/base_cyclic.py
+-rw-rw-rw-   0        0        0     5798 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/models/factory.py
+-rw-rw-rw-   0        0        0       56 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/models/model_zoo.py
+-rw-rw-rw-   0        0        0    13297 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/models/resnet_cyclic.py
+-rw-rw-rw-   0        0        0     4884 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/models/transfer_learning.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.468726 miso2-3.0.0/miso/stats/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/__init__.py
+-rw-rw-rw-   0        0        0     1490 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/accuracy.py
+-rw-rw-rw-   0        0        0    14013 2022-04-29 12:22:30.000000 miso2-3.0.0/miso/stats/confusion_matrix.py
+-rw-rw-rw-   0        0        0     6294 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/embedding.py
+-rw-rw-rw-   0        0        0     4983 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/mislabelling.py
+-rw-rw-rw-   0        0        0      909 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/most_representative.py
+-rw-rw-rw-   0        0        0     1496 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/projections.py
+-rw-rw-rw-   0        0        0      993 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/stats/training.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.496778 miso2-3.0.0/miso/training/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/training/__init__.py
+-rw-rw-rw-   0        0        0     5042 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/training/adaptive_learning_rate.py
+-rw-rw-rw-   0        0        0     3282 2022-10-07 22:59:01.000000 miso2-3.0.0/miso/training/parameters.py
+-rw-rw-rw-   0        0        0     5374 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/training/tf_augmentation.py
+-rw-rw-rw-   0        0        0    25504 2023-04-24 08:19:30.000000 miso2-3.0.0/miso/training/trainer.py
+-rw-rw-rw-   0        0        0     1757 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/training/training_result.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.538041 miso2-3.0.0/miso/utils/
+-rw-rw-rw-   0        0        0        0 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/utils/__init__.py
+-rw-rw-rw-   0        0        0    10218 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/utils/flowcam.py
+-rw-rw-rw-   0        0        0      757 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/utils/lock.py
+-rw-rw-rw-   0        0        0      227 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/utils/misc.py
+-rw-rw-rw-   0        0        0     1455 2022-08-11 23:05:55.000000 miso2-3.0.0/miso/utils/rolling_buffer.py
+-rw-rw-rw-   0        0        0     5300 2022-11-22 03:13:42.000000 miso2-3.0.0/miso/utils/singleton.py
+-rw-rw-rw-   0        0        0    10056 2022-03-10 10:07:02.000000 miso2-3.0.0/miso/utils/wave.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:19:48.233785 miso2-3.0.0/miso2.egg-info/
+-rw-rw-rw-   0        0        0      875 2023-04-24 08:19:48.000000 miso2-3.0.0/miso2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-04-24 08:19:48.000000 miso2-3.0.0/miso2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:19:48.000000 miso2-3.0.0/miso2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      231 2023-04-24 08:19:48.000000 miso2-3.0.0/miso2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-24 08:19:48.000000 miso2-3.0.0/miso2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:19:48.539449 miso2-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1843 2023-04-24 08:19:30.000000 miso2-3.0.0/setup.py
```

### Comparing `miso2-2.5.6/LICENCE.txt` & `miso2-3.0.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/PKG-INFO` & `miso2-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miso2
-Version: 2.5.6
+Version: 3.0.0
 Summary: Python scripts for training CNNs for particle classification
 Home-page: https://github.com/microfossil/particle-classification
 Author: Ross Marchant
 Author-email: ross.g.marchant@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/microfossil/particle-classification
 Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
```

### Comparing `miso2-2.5.6/miso/__main__.py` & `miso2-3.0.0/miso/__main__.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/dataset.py` & `miso2-3.0.0/miso/data/dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/download.py` & `miso2-3.0.0/miso/data/download.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/filenames_dataset.py` & `miso2-3.0.0/miso/data/filenames_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/image_dataset.py` & `miso2-3.0.0/miso/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/image_loader.py` & `miso2-3.0.0/miso/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/image_utils.py` & `miso2-3.0.0/miso/data/image_utils.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/tf_generator.py` & `miso2-3.0.0/miso/data/tf_generator.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/training_dataset.py` & `miso2-3.0.0/miso/data/training_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/data/utils.py` & `miso2-3.0.0/miso/data/utils.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/deploy/inference.py` & `miso2-3.0.0/miso/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/deploy/model_info.py` & `miso2-3.0.0/miso/deploy/model_info.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/deploy/saving.py` & `miso2-3.0.0/miso/deploy/saving.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/deploy/server.py` & `miso2-3.0.0/miso/deploy/server.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/layers/_common_blocks.py` & `miso2-3.0.0/miso/layers/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/layers/asoftmax.py` & `miso2-3.0.0/miso/layers/asoftmax.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/layers/batch_instance_normalisation.py` & `miso2-3.0.0/miso/layers/batch_instance_normalisation.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/layers/cyclic.py` & `miso2-3.0.0/miso/layers/cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/layers/group_normalisation.py` & `miso2-3.0.0/miso/layers/group_normalisation.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/layers/msoftmax.py` & `miso2-3.0.0/miso/layers/msoftmax.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/models/base_cyclic.py` & `miso2-3.0.0/miso/models/base_cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/models/factory.py` & `miso2-3.0.0/miso/models/factory.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/models/resnet_cyclic.py` & `miso2-3.0.0/miso/models/resnet_cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/models/transfer_learning.py` & `miso2-3.0.0/miso/models/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/accuracy.py` & `miso2-3.0.0/miso/stats/accuracy.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/confusion_matrix.py` & `miso2-3.0.0/miso/stats/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/embedding.py` & `miso2-3.0.0/miso/stats/embedding.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/mislabelling.py` & `miso2-3.0.0/miso/stats/mislabelling.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/most_representative.py` & `miso2-3.0.0/miso/stats/most_representative.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/projections.py` & `miso2-3.0.0/miso/stats/projections.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/stats/training.py` & `miso2-3.0.0/miso/stats/training.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/training/adaptive_learning_rate.py` & `miso2-3.0.0/miso/training/adaptive_learning_rate.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/training/parameters.py` & `miso2-3.0.0/miso/training/parameters.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/training/tf_augmentation.py` & `miso2-3.0.0/miso/training/tf_augmentation.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/training/trainer.py` & `miso2-3.0.0/miso/training/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,22 +268,22 @@
 
         # Training generator
         train_gen = ds.train_generator(batch_size=tp.training.batch_size,
                                        map_fn=augment_fn,
                                        undersample=tp.training.use_class_undersampling)
 
         # Save example of training data
-        print(" - saving example training batch")
-        training_examples_dir = os.path.join(save_dir, "examples", "training")
-        os.makedirs(training_examples_dir)
-        images, labels = next(iter(train_gen.create()))
-        for t_idx, im in enumerate(images):
-            im = (im * 255)
-            im[im > 255] = 255
-            skimage.io.imsave(os.path.join(training_examples_dir, "{:03d}.jpg".format(t_idx)), im.astype(np.uint8))
+        # print("- saving example training batch")
+        # training_examples_dir = os.path.join(save_dir, "examples", "training")
+        # os.makedirs(training_examples_dir)
+        # images, labels = next(iter(train_gen.create()))
+        # for t_idx, im in enumerate(images):
+        #     im = (im * 255)
+        #     im[im > 255] = 255
+        #     skimage.io.imsave(os.path.join(training_examples_dir, "{:03d}.jpg".format(t_idx)), im.astype(np.uint8))
 
         # Validation generator
         if tf_version == 2:
             val_one_shot = True
         else:
             # One repeat for validation for TF1 otherwise we get end of dataset errors
             val_one_shot = False
```

### Comparing `miso2-2.5.6/miso/training/training_result.py` & `miso2-3.0.0/miso/training/training_result.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/utils/flowcam.py` & `miso2-3.0.0/miso/utils/flowcam.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/utils/lock.py` & `miso2-3.0.0/miso/utils/lock.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/utils/rolling_buffer.py` & `miso2-3.0.0/miso/utils/rolling_buffer.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/utils/singleton.py` & `miso2-3.0.0/miso/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso/utils/wave.py` & `miso2-3.0.0/miso/utils/wave.py`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/miso2.egg-info/PKG-INFO` & `miso2-3.0.0/miso2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miso2
-Version: 2.5.6
+Version: 3.0.0
 Summary: Python scripts for training CNNs for particle classification
 Home-page: https://github.com/microfossil/particle-classification
 Author: Ross Marchant
 Author-email: ross.g.marchant@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/microfossil/particle-classification
 Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
```

### Comparing `miso2-2.5.6/miso2.egg-info/SOURCES.txt` & `miso2-3.0.0/miso2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miso2-2.5.6/setup.py` & `miso2-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='miso2',
-    version='2.5.6',
+    version='3.0.0',
     description='Python scripts for training CNNs for particle classification',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ross Marchant',
     author_email='ross.g.marchant@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -34,15 +34,16 @@
                       'flask==1.1.2',
                       'itsdangerous==1.1.0',
                       'tqdm',
                       'openpyxl',
                       'imblearn',
                       'tf2onnx',
                       'cleanlab',
-                      'packaging'],
+                      'packaging',
+                      'tensorflow_addons'],
     url='https://github.com/microfossil/particle-classification',
     license='MIT',
     project_urls={  # Optional
         'Source': 'https://github.com/microfossil/particle-classification',
         'Paper': 'https://jm.copernicus.org/articles/39/183/2020/',
     },
 )
```

