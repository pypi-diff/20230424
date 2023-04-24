# Comparing `tmp/obpgenerator-0.0.18.tar.gz` & `tmp/obpgenerator-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obpgenerator-0.0.18.tar", last modified: Mon Apr 24 09:18:00 2023, max compression
+gzip compressed data, was "obpgenerator-0.0.19.tar", last modified: Mon Apr 24 09:33:03 2023, max compression
```

## Comparing `obpgenerator-0.0.18.tar` & `obpgenerator-0.0.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:18:00.273429 obpgenerator-0.0.18/
--rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.18/LICENSE
--rw-rw-rw-   0        0        0     2880 2023-04-24 09:18:00.274428 obpgenerator-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0     2390 2023-04-21 15:00:47.000000 obpgenerator-0.0.18/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:18:00.232663 obpgenerator-0.0.18/obpgenerator/
--rw-rw-rw-   0        0        0     3681 2023-04-21 12:27:56.000000 obpgenerator-0.0.18/obpgenerator/Layer.py
--rw-rw-rw-   0        0        0     5214 2023-04-24 09:15:08.000000 obpgenerator-0.0.18/obpgenerator/Part.py
--rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.18/obpgenerator/Shape.py
--rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.18/obpgenerator/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.18/obpgenerator/file_import.py
--rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.18/obpgenerator/generate_obp.py
--rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.18/obpgenerator/layer_sorting.py
--rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.18/obpgenerator/manufacturing_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:18:00.267421 obpgenerator-0.0.18/obpgenerator/melt_strategies/
--rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.18/obpgenerator/melt_strategies/__init__.py
--rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.18/obpgenerator/melt_strategies/line_melting.py
--rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.18/obpgenerator/melt_strategies/point_melting.py
--rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.18/obpgenerator/shape_melting.py
--rw-rw-rw-   0        0        0     3131 2023-04-24 09:15:40.000000 obpgenerator-0.0.18/obpgenerator/slicer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:18:00.272422 obpgenerator-0.0.18/obpgenerator/visualization/
--rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.18/obpgenerator/visualization/__init__.py
--rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.18/obpgenerator/visualization/obp_to_matplotlib.py
--rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.18/obpgenerator/visualization/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:18:00.261412 obpgenerator-0.0.18/obpgenerator.egg-info/
--rw-rw-rw-   0        0        0     2880 2023-04-24 09:18:00.000000 obpgenerator-0.0.18/obpgenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-04-24 09:18:00.000000 obpgenerator-0.0.18/obpgenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:18:00.000000 obpgenerator-0.0.18/obpgenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-24 09:18:00.000000 obpgenerator-0.0.18/obpgenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 09:18:00.000000 obpgenerator-0.0.18/obpgenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.18/pyproject.toml
--rw-rw-rw-   0        0        0      662 2023-04-24 09:18:00.282424 obpgenerator-0.0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.860252 obpgenerator-0.0.19/
+-rw-rw-rw-   0        0        0     1091 2023-03-14 16:54:43.000000 obpgenerator-0.0.19/LICENSE
+-rw-rw-rw-   0        0        0     2880 2023-04-24 09:33:03.860252 obpgenerator-0.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0     2390 2023-04-21 15:00:47.000000 obpgenerator-0.0.19/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.775915 obpgenerator-0.0.19/obpgenerator/
+-rw-rw-rw-   0        0        0     3681 2023-04-21 12:27:56.000000 obpgenerator-0.0.19/obpgenerator/Layer.py
+-rw-rw-rw-   0        0        0     5214 2023-04-24 09:15:08.000000 obpgenerator-0.0.19/obpgenerator/Part.py
+-rw-rw-rw-   0        0        0     4647 2023-04-21 13:56:52.000000 obpgenerator-0.0.19/obpgenerator/Shape.py
+-rw-rw-rw-   0        0        0      171 2023-03-21 14:44:59.000000 obpgenerator-0.0.19/obpgenerator/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-03-20 20:01:41.000000 obpgenerator-0.0.19/obpgenerator/file_import.py
+-rw-rw-rw-   0        0        0      842 2023-03-24 15:54:31.000000 obpgenerator-0.0.19/obpgenerator/generate_obp.py
+-rw-rw-rw-   0        0        0     3352 2023-03-22 07:43:38.000000 obpgenerator-0.0.19/obpgenerator/layer_sorting.py
+-rw-rw-rw-   0        0        0     3150 2023-02-24 22:18:01.000000 obpgenerator-0.0.19/obpgenerator/manufacturing_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.832781 obpgenerator-0.0.19/obpgenerator/melt_strategies/
+-rw-rw-rw-   0        0        0       56 2023-04-11 11:45:09.000000 obpgenerator-0.0.19/obpgenerator/melt_strategies/__init__.py
+-rw-rw-rw-   0        0        0     2940 2023-02-24 19:34:30.000000 obpgenerator-0.0.19/obpgenerator/melt_strategies/line_melting.py
+-rw-rw-rw-   0        0        0      558 2023-02-24 19:10:25.000000 obpgenerator-0.0.19/obpgenerator/melt_strategies/point_melting.py
+-rw-rw-rw-   0        0        0      703 2023-03-17 14:49:52.000000 obpgenerator-0.0.19/obpgenerator/shape_melting.py
+-rw-rw-rw-   0        0        0     3131 2023-04-24 09:15:40.000000 obpgenerator-0.0.19/obpgenerator/slicer.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.858252 obpgenerator-0.0.19/obpgenerator/visualization/
+-rw-rw-rw-   0        0        0       60 2023-04-12 12:20:29.000000 obpgenerator-0.0.19/obpgenerator/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1155 2023-04-12 14:51:19.000000 obpgenerator-0.0.19/obpgenerator/visualization/obp_to_matplotlib.py
+-rw-rw-rw-   0        0        0     3178 2023-04-12 14:51:18.000000 obpgenerator-0.0.19/obpgenerator/visualization/visualization.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:03.805754 obpgenerator-0.0.19/obpgenerator.egg-info/
+-rw-rw-rw-   0        0        0     2880 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 09:33:03.000000 obpgenerator-0.0.19/obpgenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-03-20 19:39:06.000000 obpgenerator-0.0.19/pyproject.toml
+-rw-rw-rw-   0        0        0      646 2023-04-24 09:33:03.863256 obpgenerator-0.0.19/setup.cfg
```

### Comparing `obpgenerator-0.0.18/LICENSE` & `obpgenerator-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/PKG-INFO` & `obpgenerator-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpgenerator
-Version: 0.0.18
+Version: 0.0.19
 Summary: Generation of open beam path files based on different strategies
 Home-page: https://github.com/wiberganton/obpgenerator
 Author: Anton Wiberg
 Author-email: wiberg.anton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `obpgenerator-0.0.18/README.md` & `obpgenerator-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/Layer.py` & `obpgenerator-0.0.19/obpgenerator/Layer.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/Part.py` & `obpgenerator-0.0.19/obpgenerator/Part.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/Shape.py` & `obpgenerator-0.0.19/obpgenerator/Shape.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/file_import.py` & `obpgenerator-0.0.19/obpgenerator/file_import.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/generate_obp.py` & `obpgenerator-0.0.19/obpgenerator/generate_obp.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/layer_sorting.py` & `obpgenerator-0.0.19/obpgenerator/layer_sorting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/manufacturing_settings.py` & `obpgenerator-0.0.19/obpgenerator/manufacturing_settings.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/melt_strategies/line_melting.py` & `obpgenerator-0.0.19/obpgenerator/melt_strategies/line_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/melt_strategies/point_melting.py` & `obpgenerator-0.0.19/obpgenerator/melt_strategies/point_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/shape_melting.py` & `obpgenerator-0.0.19/obpgenerator/shape_melting.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/slicer.py` & `obpgenerator-0.0.19/obpgenerator/slicer.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/visualization/obp_to_matplotlib.py` & `obpgenerator-0.0.19/obpgenerator/visualization/obp_to_matplotlib.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator/visualization/visualization.py` & `obpgenerator-0.0.19/obpgenerator/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/obpgenerator.egg-info/PKG-INFO` & `obpgenerator-0.0.19/obpgenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obpgenerator
-Version: 0.0.18
+Version: 0.0.19
 Summary: Generation of open beam path files based on different strategies
 Home-page: https://github.com/wiberganton/obpgenerator
 Author: Anton Wiberg
 Author-email: wiberg.anton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `obpgenerator-0.0.18/obpgenerator.egg-info/SOURCES.txt` & `obpgenerator-0.0.19/obpgenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obpgenerator-0.0.18/setup.cfg` & `obpgenerator-0.0.19/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6270 6765 6e65 7261 746f 720d   = obpgenerator.
 00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
-00000030: 380d 0a61 7574 686f 7220 3d20 416e 746f  8..author = Anto
+00000030: 390d 0a61 7574 686f 7220 3d20 416e 746f  9..author = Anto
 00000040: 6e20 5769 6265 7267 0d0a 6175 7468 6f72  n Wiberg..author
 00000050: 5f65 6d61 696c 203d 2077 6962 6572 672e  _email = wiberg.
 00000060: 616e 746f 6e40 676d 6169 6c2e 636f 6d0d  anton@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2047  .description = G
 00000080: 656e 6572 6174 696f 6e20 6f66 206f 7065  eneration of ope
 00000090: 6e20 6265 616d 2070 6174 6820 6669 6c65  n beam path file
 000000a0: 7320 6261 7365 6420 6f6e 2064 6966 6665  s based on diffe
@@ -28,15 +28,14 @@
 000001b0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
 000001c0: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
 000001d0: 7469 6f6e 735d 0d0a 696e 7374 616c 6c5f  tions]..install_
 000001e0: 7265 7175 6972 6573 203d 200d 0a09 7376  requires = ...sv
 000001f0: 6770 6174 6874 6f6f 6c73 0d0a 096e 756d  gpathtools...num
 00000200: 7079 0d0a 096d 6174 706c 6f74 6c69 620d  py...matplotlib.
 00000210: 0a09 6f62 706c 6962 0d0a 0970 7976 6973  ..obplib...pyvis
-00000220: 7461 0d0a 0979 616d 6c0d 0a09 7079 7961  ta...yaml...pyya
-00000230: 6d6c 0d0a 7079 7468 6f6e 5f72 6571 7569  ml..python_requi
-00000240: 7265 7320 3d20 3e3d 332e 370d 0a69 6e63  res = >=3.7..inc
-00000250: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000260: 6120 3d20 5472 7565 0d0a 0d0a 5b65 6767  a = True....[egg
-00000270: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000280: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000290: 2030 0d0a 0d0a                            0....
+00000220: 7461 0d0a 7079 7468 6f6e 5f72 6571 7569  ta..python_requi
+00000230: 7265 7320 3d20 3e3d 332e 370d 0a69 6e63  res = >=3.7..inc
+00000240: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000250: 6120 3d20 5472 7565 0d0a 0d0a 5b65 6767  a = True....[egg
+00000260: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000270: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000280: 2030 0d0a 0d0a                            0....
```

