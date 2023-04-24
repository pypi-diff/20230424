# Comparing `tmp/bm_utilities-0.0.2.tar.gz` & `tmp/bm_utilities-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.0.2.tar", last modified: Mon Apr 24 20:18:42 2023, max compression
+gzip compressed data, was "bm_utilities-0.0.3.tar", last modified: Mon Apr 24 20:33:00 2023, max compression
```

## Comparing `bm_utilities-0.0.2.tar` & `bm_utilities-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 20:18:42.578358 bm_utilities-0.0.2/
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-04-24 20:18:42.578358 bm_utilities-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 20:18:42.564356 bm_utilities-0.0.2/bm_utilities/
--rw-rw-rw-   0        0        0      136 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     4953 2023-04-24 20:17:18.000000 bm_utilities-0.0.2/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/bm_utilities/common.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:18:42.576357 bm_utilities-0.0.2/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0      420 2023-04-24 20:18:42.579358 bm_utilities-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-04-24 20:16:42.000000 bm_utilities-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:33:00.128076 bm_utilities-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-04-24 20:33:00.128076 bm_utilities-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 20:33:00.111081 bm_utilities-0.0.3/bm_utilities/
+-rw-rw-rw-   0        0        0      136 2023-04-24 13:32:39.000000 bm_utilities-0.0.3/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     4954 2023-04-24 20:31:58.000000 bm_utilities-0.0.3/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.3/bm_utilities/common.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:33:00.126081 bm_utilities-0.0.3/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-04-24 20:32:59.000000 bm_utilities-0.0.3/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-24 20:32:59.000000 bm_utilities-0.0.3/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 20:32:59.000000 bm_utilities-0.0.3/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 20:32:59.000000 bm_utilities-0.0.3/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-24 20:32:59.000000 bm_utilities-0.0.3/bm_utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0      420 2023-04-24 20:33:00.130077 bm_utilities-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-04-24 20:32:44.000000 bm_utilities-0.0.3/setup.py
```

### Comparing `bm_utilities-0.0.2/LICENSE` & `bm_utilities-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.2/PKG-INFO` & `bm_utilities-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.2/README.md` & `bm_utilities-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.2/bm_utilities/bm_utilities.py` & `bm_utilities-0.0.3/bm_utilities/bm_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pip install geopandas arcgis pyarabic
+!pip install geopandas arcgis pyarabic
 
 
 import re
 import geopandas as gpd
 from shapely.geometry import Point, Polygon
 import numpy as np
 from arcgis.gis import GIS
```

### Comparing `bm_utilities-0.0.2/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.0.3/bm_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.2/setup.py` & `bm_utilities-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='bm_utilities',
     name='bm_utilities',
     packages=find_packages(include=['bm_utilities', 'bm_utilities.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/bm_utilities',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

