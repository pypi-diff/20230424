# Comparing `tmp/bm_utilities-0.0.1.tar.gz` & `tmp/bm_utilities-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.0.1.tar", last modified: Mon Apr 24 18:51:04 2023, max compression
+gzip compressed data, was "bm_utilities-0.0.2.tar", last modified: Mon Apr 24 20:18:42 2023, max compression
```

## Comparing `bm_utilities-0.0.1.tar` & `bm_utilities-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.530729 bm_utilities-0.0.1/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.185691 bm_utilities-0.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.201335 bm_utilities-0.0.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.216954 bm_utilities-0.0.1/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-04-24 18:51:04.530729 bm_utilities-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.358006 bm_utilities-0.0.1/bm_utilities/
--rw-rw-rw-   0        0        0      136 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     4912 2023-04-24 16:19:54.000000 bm_utilities-0.0.1/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/bm_utilities/common.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.405280 bm_utilities-0.0.1/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-04-24 18:51:03.000000 bm_utilities-0.0.1/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-04-24 18:51:04.000000 bm_utilities-0.0.1/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 18:51:03.000000 bm_utilities-0.0.1/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 18:51:03.000000 bm_utilities-0.0.1/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-24 18:51:03.000000 bm_utilities-0.0.1/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.420905 bm_utilities-0.0.1/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.420905 bm_utilities-0.0.1/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.420905 bm_utilities-0.0.1/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      152 2023-04-24 18:47:41.000000 bm_utilities-0.0.1/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-04-24 18:51:04.530729 bm_utilities-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:51:04.483844 bm_utilities-0.0.1/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.0.1/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:18:42.578358 bm_utilities-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-04-24 20:18:42.578358 bm_utilities-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 20:18:42.564356 bm_utilities-0.0.2/bm_utilities/
+-rw-rw-rw-   0        0        0      136 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     4953 2023-04-24 20:17:18.000000 bm_utilities-0.0.2/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/bm_utilities/common.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:18:42.576357 bm_utilities-0.0.2/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-24 20:18:42.000000 bm_utilities-0.0.2/bm_utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-24 13:32:39.000000 bm_utilities-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      420 2023-04-24 20:18:42.579358 bm_utilities-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-04-24 20:16:42.000000 bm_utilities-0.0.2/setup.py
```

### Comparing `bm_utilities-0.0.1/LICENSE` & `bm_utilities-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.1/PKG-INFO` & `bm_utilities-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.1/README.md` & `bm_utilities-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.0.1/bm_utilities/bm_utilities.py` & `bm_utilities-0.0.2/bm_utilities/bm_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+pip install geopandas arcgis pyarabic
+
+
 import re
 import geopandas as gpd
 from shapely.geometry import Point, Polygon
 import numpy as np
 from arcgis.gis import GIS
 from arcgis.geocoding import geocode
 from tqdm import tqdm
@@ -102,8 +105,8 @@
 
                 if country == 'EGY':
                     Latitude = geocode_results[0]["location"].get("y",np.NAN)
                     Longitude =  geocode_results[0]["location"].get("x",np.NAN)
                     input_data = pd.DataFrame({"Latitude":Latitude,"Longitude":Longitude,"address":address_1,"id":idz},index=[0])
                     get_polygon = PolygonFinder(self.polygons)
                     address = get_polygon.get_closest_polygon(Latitude,Longitude)
-        return address
+        return address
```

### Comparing `bm_utilities-0.0.1/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.0.2/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.0.1/setup.py` & `bm_utilities-0.0.2/setup.py`

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
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

