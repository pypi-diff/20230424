# Comparing `tmp/efel-4.1.93.tar.gz` & `tmp/efel-4.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.1.93.tar", last modified: Thu Apr 20 11:46:28 2023, max compression
+gzip compressed data, was "efel-4.1.95.tar", last modified: Mon Apr 24 14:35:18 2023, max compression
```

## Comparing `efel-4.1.93.tar` & `efel-4.1.95.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-20 11:46:25.000000 efel-4.1.93/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-04-20 11:46:25.000000 efel-4.1.93/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-04-20 11:46:25.000000 efel-4.1.93/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-20 11:46:25.000000 efel-4.1.93/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-20 11:46:25.000000 efel-4.1.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-20 11:46:27.991787 efel-4.1.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-04-20 11:46:25.000000 efel-4.1.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12805 2023-04-20 11:46:25.000000 efel-4.1.93/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-20 11:46:25.000000 efel-4.1.93/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-20 11:46:27.991787 efel-4.1.93/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-04-20 11:46:25.000000 efel-4.1.93/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   136506 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-20 11:46:25.000000 efel-4.1.93/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-04-20 11:46:25.000000 efel-4.1.93/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.991787 efel-4.1.93/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-20 11:46:25.000000 efel-4.1.93/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-04-20 11:46:25.000000 efel-4.1.93/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-20 11:46:25.000000 efel-4.1.93/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 11:46:27.987787 efel-4.1.93/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-20 11:46:27.000000 efel-4.1.93/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-20 11:46:27.991787 efel-4.1.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-04-20 11:46:25.000000 efel-4.1.93/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-04-20 11:46:25.000000 efel-4.1.93/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:18.712840 efel-4.1.95/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-24 14:35:17.000000 efel-4.1.95/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-04-24 14:35:17.000000 efel-4.1.95/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-04-24 14:35:17.000000 efel-4.1.95/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-24 14:35:17.000000 efel-4.1.95/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-24 14:35:17.000000 efel-4.1.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-24 14:35:18.712840 efel-4.1.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-04-24 14:35:17.000000 efel-4.1.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:18.716840 efel-4.1.95/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-04-24 14:35:17.000000 efel-4.1.95/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-24 14:35:17.000000 efel-4.1.95/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-24 14:35:18.716840 efel-4.1.95/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-04-24 14:35:17.000000 efel-4.1.95/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:18.712840 efel-4.1.95/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   136807 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-24 14:35:17.000000 efel-4.1.95/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-04-24 14:35:17.000000 efel-4.1.95/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:18.712840 efel-4.1.95/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-24 14:35:17.000000 efel-4.1.95/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-04-24 14:35:17.000000 efel-4.1.95/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-24 14:35:17.000000 efel-4.1.95/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:18.712840 efel-4.1.95/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-24 14:35:18.000000 efel-4.1.95/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-24 14:35:18.000000 efel-4.1.95/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 14:35:18.000000 efel-4.1.95/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-24 14:35:18.000000 efel-4.1.95/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-24 14:35:18.000000 efel-4.1.95/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-24 14:35:18.716840 efel-4.1.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-04-24 14:35:17.000000 efel-4.1.95/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-04-24 14:35:17.000000 efel-4.1.95/versioneer.py
```

### Comparing `efel-4.1.93/COPYING` & `efel-4.1.95/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/COPYING.less` & `efel-4.1.95/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/LICENSE.txt` & `efel-4.1.95/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/PKG-INFO` & `efel-4.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.1.93
+Version: 4.1.95
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.1.93/README.md` & `efel-4.1.95/README.md`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/DependencyV5.txt` & `efel-4.1.95/efel/DependencyV5.txt`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 LibV5:inv_second_ISI   #LibV5:all_ISI_values #LibV1:interpolate 
 LibV5:inv_third_ISI   #LibV5:all_ISI_values #LibV1:interpolate 
 LibV5:inv_fourth_ISI   #LibV5:all_ISI_values #LibV1:interpolate 
 LibV5:inv_fifth_ISI   #LibV5:all_ISI_values #LibV1:interpolate 
 LibV5:inv_last_ISI   #LibV5:all_ISI_values #LibV1:interpolate 
 LibV5:inv_time_to_first_spike   #LibV1:time_to_first_spike #LibV1:interpolate 
 LibV5:spike_half_width 	    #LibV5:min_AHP_indices	#LibV5:peak_indices #LibV1:interpolate 
-LibV5:AP_begin_indices      #LibV5:min_AHP_indices #LibV1:interpolate
+LibV5:AP_begin_indices      #LibV5:min_AHP_indices #LibV5:peak_indices #LibV1:interpolate
 LibV5:AHP_depth_abs         #LibV5:min_AHP_values #LibV1:interpolate 
 LibV5:AP_begin_width 	    #LibV5:min_AHP_indices	#LibV5:AP_begin_indices #LibV1:interpolate 
 LibV5:AP_begin_voltage  #LibV5:AP_begin_indices #LibV1:interpolate 
 LibV5:AP_begin_time     #LibV5:AP_begin_indices #LibV1:interpolate 
 LibV5:AP1_begin_voltage  #LibV5:AP_begin_voltage #LibV1:interpolate 
 LibV5:AP2_begin_voltage  #LibV5:AP_begin_voltage #LibV1:interpolate 
 LibV5:AP1_begin_width  #LibV5:AP_begin_width #LibV1:interpolate
```

### Comparing `efel-4.1.93/efel/__init__.py` & `efel-4.1.95/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/api.py` & `efel-4.1.95/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/DependencyTree.cpp` & `efel-4.1.95/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/DependencyTree.h` & `efel-4.1.95/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/FillFptrTable.cpp` & `efel-4.1.95/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/FillFptrTable.h` & `efel-4.1.95/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/Global.h` & `efel-4.1.95/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV1.cpp` & `efel-4.1.95/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV1.h` & `efel-4.1.95/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV2.cpp` & `efel-4.1.95/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV2.h` & `efel-4.1.95/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV3.cpp` & `efel-4.1.95/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV3.h` & `efel-4.1.95/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV4.cpp` & `efel-4.1.95/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV4.h` & `efel-4.1.95/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/LibV5.cpp` & `efel-4.1.95/efel/cppcore/LibV5.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -620,50 +620,56 @@
 }
 
 //
 // *** AP begin indices ***
 //
 static int __AP_begin_indices(const vector<double>& t, const vector<double>& v,
                               double stimstart, double stimend,
+                              const vector<int>& pi,
                               const vector<int>& ahpi, vector<int>& apbi,
                               double dTh, int derivative_window) {
   const double derivativethreshold = dTh;
   vector<double> dvdt(v.size());
   vector<double> dv;
   vector<double> dt;
   getCentralDifferenceDerivative(1., v, dv);
   getCentralDifferenceDerivative(1., t, dt);
   transform(dv.begin(), dv.end(), dt.begin(), dvdt.begin(),
             std::divides<double>());
 
   // restrict to time interval where stimulus is applied
-  vector<int> minima;
+  vector<int> minima, peak_indices;
   int stimbeginindex =
       distance(t.begin(),
                find_if(t.begin(), t.end(),
                        std::bind2nd(std::greater_equal<double>(), stimstart)));
   minima.push_back(stimbeginindex);
   for (size_t i = 0; i < ahpi.size(); i++) {
     if (ahpi[i] > stimbeginindex) {
       minima.push_back(ahpi[i]);
     }
     // if(t[ahpi[i]] > stimend) {
     //    break;
     //}
   }
-  // if the AHP_indices are already restricted make sure that we do not miss
-  // the last spike
-  // if(t[minima.back()] < stimend) {
+   for (size_t i = 0; i < pi.size(); i++) {
+    if (pi[i] > stimbeginindex) {
+      peak_indices.push_back(pi[i]);
+    }
+  }
   int endindex = distance(t.begin(), t.end());
-  minima.push_back(endindex);
-  //}
+  if (minima.size() < peak_indices.size()){
+    GErrorStr += "\nMore peaks than min_AHP in AP_begin_indices\n";
+    return -1;
+  }
+
   // printf("Found %d minima\n", minima.size());
-  for (size_t i = 0; i < minima.size() - 2; i++) {
+  for (size_t i = 0; i < peak_indices.size(); i++) {
     // assure that the width of the slope is bigger than 4
-    int newbegin = minima[i + 1];
+    int newbegin = peak_indices[i];
     int begin = minima[i];
     int width = derivative_window;
     bool skip = false;
 
     // Detect where the derivate crosses derivativethreshold, and make sure
     // this happens in a window of 'width' sampling point
     do {
@@ -719,14 +725,17 @@
   if (retVal < 0) return -1;
   vector<double> stimstart;
   retVal = getVec(DoubleFeatureData, StringData, "stim_start", stimstart);
   if (retVal < 0) return -1;
   vector<double> stimend;
   retVal = getVec(DoubleFeatureData, StringData, "stim_end", stimend);
   if (retVal < 0) return -1;
+  vector<int> pi;
+  retVal = getVec(IntFeatureData, StringData, "peak_indices", pi);
+  if (retVal < 0) return -1;
   vector<int> ahpi;
   retVal = getVec(IntFeatureData, StringData, "min_AHP_indices", ahpi);
   if (retVal < 0) return -1;
   vector<int> apbi;
 
   // Get DerivativeThreshold
   vector<double> dTh;
@@ -743,15 +752,16 @@
   if (retVal <= 0) {
     GErrorStr += "\nDerivativeWindow not set\n";
     return -1;
   }
   
   // Calculate feature
   retVal =
-      __AP_begin_indices(t, v, stimstart[0], stimend[0], ahpi, apbi, dTh[0], derivative_window[0]);
+      __AP_begin_indices(t, v, stimstart[0], stimend[0], 
+                         pi, ahpi, apbi, dTh[0], derivative_window[0]);
 
   // Save feature value
   if (retVal >= 0) {
     setVec(IntFeatureData, StringData, "AP_begin_indices", apbi);
   }
   return retVal;
 }
```

### Comparing `efel-4.1.93/efel/cppcore/LibV5.h` & `efel-4.1.95/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/Utils.cpp` & `efel-4.1.95/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/Utils.h` & `efel-4.1.95/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/cfeature.cpp` & `efel-4.1.95/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/cfeature.h` & `efel-4.1.95/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/cppcore.cpp` & `efel-4.1.95/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/eFELLogger.h` & `efel-4.1.95/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/efel.cpp` & `efel-4.1.95/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/efel.h` & `efel-4.1.95/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/mapoperations.cpp` & `efel-4.1.95/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/mapoperations.h` & `efel-4.1.95/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/cppcore/types.h` & `efel-4.1.95/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/io.py` & `efel-4.1.95/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/pyfeatures/__init__.py` & `efel-4.1.95/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/pyfeatures/pyfeatures.py` & `efel-4.1.95/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel/settings.py` & `efel-4.1.95/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/efel.egg-info/PKG-INFO` & `efel-4.1.95/efel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.1.93
+Version: 4.1.95
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.1.93/efel.egg-info/SOURCES.txt` & `efel-4.1.95/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/setup.py` & `efel-4.1.95/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.93/versioneer.py` & `efel-4.1.95/versioneer.py`

 * *Files identical despite different names*

