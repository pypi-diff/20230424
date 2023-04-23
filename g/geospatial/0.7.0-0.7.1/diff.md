# Comparing `tmp/geospatial-0.7.0.tar.gz` & `tmp/geospatial-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospatial-0.7.0.tar", last modified: Tue Nov 29 14:29:39 2022, max compression
+gzip compressed data, was "geospatial-0.7.1.tar", last modified: Sun Apr 23 22:40:39 2023, max compression
```

## Comparing `geospatial-0.7.0.tar` & `geospatial-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:29:39.548625 geospatial-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 14:29:32.000000 geospatial-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      122 2022-11-29 14:29:32.000000 geospatial-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2022-11-29 14:29:39.548625 geospatial-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2022-11-29 14:29:32.000000 geospatial-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:29:39.548625 geospatial-0.7.0/geospatial/
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-11-29 14:29:32.000000 geospatial-0.7.0/geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-29 14:29:32.000000 geospatial-0.7.0/geospatial/geospatial.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 14:29:39.548625 geospatial-0.7.0/geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2022-11-29 14:29:39.000000 geospatial-0.7.0/geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      315 2022-11-29 14:29:39.000000 geospatial-0.7.0/geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      821 2022-11-29 14:29:39.000000 geospatial-0.7.0/geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 14:29:39.000000 geospatial-0.7.0/geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      612 2022-11-29 14:29:39.000000 geospatial-0.7.0/geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-29 14:29:39.000000 geospatial-0.7.0/geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      820 2022-11-29 14:29:32.000000 geospatial-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      393 2022-11-29 14:29:39.548625 geospatial-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2022-11-29 14:29:32.000000 geospatial-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:40:39.243448 geospatial-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-23 22:40:26.000000 geospatial-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 22:40:26.000000 geospatial-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-23 22:40:39.243448 geospatial-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-23 22:40:26.000000 geospatial-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:40:39.243448 geospatial-0.7.1/geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 22:40:26.000000 geospatial-0.7.1/geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 22:40:26.000000 geospatial-0.7.1/geospatial/geospatial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:40:39.243448 geospatial-0.7.1/geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-23 22:40:39.000000 geospatial-0.7.1/geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-23 22:40:39.000000 geospatial-0.7.1/geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-23 22:40:39.000000 geospatial-0.7.1/geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:40:39.000000 geospatial-0.7.1/geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-23 22:40:39.000000 geospatial-0.7.1/geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 22:40:39.000000 geospatial-0.7.1/geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-23 22:40:26.000000 geospatial-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 22:40:39.243448 geospatial-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-23 22:40:26.000000 geospatial-0.7.1/setup.py
```

### Comparing `geospatial-0.7.0/LICENSE` & `geospatial-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geospatial-0.7.0/PKG-INFO` & `geospatial-0.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: geospatial
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package for installing commonly used packages for geospatial analysis and data visualization with only one command.
 Home-page: https://github.com/giswqs/geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: geospatial
-Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geospatial
 
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://gishub.org/geospatial-colab)
 [![image](https://mybinder.org/badge_logo.svg)](https://gishub.org/geospatial-binder)
```

### Comparing `geospatial-0.7.0/README.md` & `geospatial-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `geospatial-0.7.0/geospatial.egg-info/PKG-INFO` & `geospatial-0.7.1/geospatial.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: geospatial
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package for installing commonly used packages for geospatial analysis and data visualization with only one command.
 Home-page: https://github.com/giswqs/geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: geospatial
-Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # geospatial
 
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://gishub.org/geospatial-colab)
 [![image](https://mybinder.org/badge_logo.svg)](https://gishub.org/geospatial-binder)
```

### Comparing `geospatial-0.7.0/geospatial.egg-info/dependency_links.txt` & `geospatial-0.7.1/geospatial.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,59 @@
-# --find-links https://girder.github.io/large_image_wheels GDAL
-# cartopy; platform_platform != "Windows"
 bokeh
 cenpy
 contextily
 dask-geopandas
 datashader
 earthengine-api
 earthpy
-easystac; python_version > '3.7'
+easystac
 eemont
-# eomaps
 eoreader
 folium>=0.12.1
 geemap>=0.13.7
 gemgis
 geoalchemy2
 geocube
 geopandas
-geosnap
-# geoviews
 h3
 here-map-widget-for-jupyter
 hvplot
 ipygany
 ipyleaflet
 ipyvtklink
 keplergl
 laspy
 leafmap>=0.9.3
-# lidar
 localtileserver>=0.5.8
 mapboxgl
-# movingpandas
+mapwidget
 mss
 netcdf4
 odc-stac
 osmnx
 owslib
 panel
 palettable
 planetary-computer
 plotly
 proplot
 psycopg2
 pydeck
 pygis>=0.3.1
 pyntcloud
-# pysal
-# pyvista
 radiant-mlhub
 rasterio
 rasterstats
 rio-cogeo
 rioxarray
 s2cloudless
 sarpy
 satpy
 sentinelsat
 shapely
+simplekml
 sliderule
 spyndex
 sqlalchemy
-stackstac; python_version > '3.7'
-# tropycal
+stackstac
 xarray-spatial
-# xmovie
 wxee
-
```

### Comparing `geospatial-0.7.0/requirements.txt` & `geospatial-0.7.1/geospatial.egg-info/dependency_links.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 bokeh
 cenpy
 contextily
 dask-geopandas
 datashader
 earthengine-api
 earthpy
-easystac; python_version > '3.7'
+easystac
 eemont
 # eomaps
 eoreader
 folium>=0.12.1
 geemap>=0.13.7
 gemgis
 geoalchemy2
 geocube
 geopandas
-geosnap
+# geosnap
 # geoviews
 h3
 here-map-widget-for-jupyter
 hvplot
 ipygany
 ipyleaflet
 ipyvtklink
 keplergl
 laspy
 leafmap>=0.9.3
 # lidar
 localtileserver>=0.5.8
 mapboxgl
+mapwidget
 # movingpandas
 mss
 netcdf4
 odc-stac
 osmnx
 owslib
 panel
@@ -54,15 +55,17 @@
 rio-cogeo
 rioxarray
 s2cloudless
 sarpy
 satpy
 sentinelsat
 shapely
+simplekml
 sliderule
 spyndex
 sqlalchemy
-stackstac; python_version > '3.7'
+stackstac
 # tropycal
 xarray-spatial
 # xmovie
 wxee
+
```

### Comparing `geospatial-0.7.0/setup.py` & `geospatial-0.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     author="Qiusheng Wu",
     author_email='giswqs@gmail.com',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="A Python package for installing commonly used packages for geospatial analysis and data visualization with only one command.",
     install_requires=install_requires,
     dependency_links=dependency_links,
     license="MIT license",
     long_description=readme,
     long_description_content_type='text/markdown',
@@ -47,10 +47,10 @@
     keywords='geospatial',
     name='geospatial',
     packages=find_packages(include=['geospatial', 'geospatial.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/giswqs/geospatial',
-    version='0.7.0',
+    version='0.7.1',
     zip_safe=False,
 )
```

