# Comparing `tmp/osdatahub-1.2.3.tar.gz` & `tmp/osdatahub-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osdatahub-1.2.3.tar", last modified: Wed Apr 12 14:40:39 2023, max compression
+gzip compressed data, was "osdatahub-1.2.4.tar", last modified: Mon Apr 24 14:28:50 2023, max compression
```

## Comparing `osdatahub-1.2.3.tar` & `osdatahub-1.2.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 14:40:17.000000 osdatahub-1.2.3/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.700413 osdatahub-1.2.3/Examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/CRS pitfalls.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   231081 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Converting API Results into Common Data Formats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1837789 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Defining Extents for API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Filtering Attributes for API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Interactive Plotting for API Results - Folium.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   945983 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Post Processing API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Quick Start Guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Setting up an API key.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    86367 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/Using the NGD Features API.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.704413 osdatahub-1.2.3/Examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)  2124067 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/1_homescreen.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   178174 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/2_sign_up.PNG
--rw-r--r--   0 runner    (1001) docker     (123)  1883255 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/3_datahub_homepage.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   115385 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/4_new_project.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   153664 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/5_add_api_to_project.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   113078 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/6_view_api_key.PNG
--rw-r--r--   0 runner    (1001) docker     (123)  1790610 2023-04-12 14:40:17.000000 osdatahub-1.2.3/Examples/images/CRS.png
--rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-04-12 14:40:17.000000 osdatahub-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 14:40:17.000000 osdatahub-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-12 14:40:39.716413 osdatahub-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-12 14:40:17.000000 osdatahub-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.708413 osdatahub-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/DownloadsAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/Extent.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/FeaturesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/LinkedIdentifiersAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/NGD.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/NamesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/PlacesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/Utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.708413 osdatahub-1.2.3/docs/media/
--rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/media/os-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/readme_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 14:40:17.000000 osdatahub-1.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.708413 osdatahub-1.2.3/media/
--rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-12 14:40:17.000000 osdatahub-1.2.3/media/os-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 14:40:17.000000 osdatahub-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 14:40:17.000000 osdatahub-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-12 14:40:39.720413 osdatahub-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 14:40:17.000000 osdatahub-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.692412 osdatahub-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/data_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/downloads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/DownloadsAPI/opendata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/feature_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/FeaturesAPI/features_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/NGD/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NGD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NGD/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NGD/ngd_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/NamesAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NamesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NamesAPI/local_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/NamesAPI/names_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub/PlacesAPI/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/PlacesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/PlacesAPI/places_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/grow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/ons_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/requests_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/spatial_filter_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-12 14:40:17.000000 osdatahub-1.2.3/src/osdatahub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.712413 osdatahub-1.2.3/src/osdatahub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:40:39.000000 osdatahub-1.2.3/src/osdatahub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/clean_polygon_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/
--rw-r--r--   0 runner    (1001) docker     (123)    29650 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    45345 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    32875 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:40:39.716413 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/
--rw-r--r--   0 runner    (1001) docker     (123)    37512 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    58496 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    33032 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data/get_uncleaned_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/clean_polygon_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/downloads_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/extent_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/features_api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/filters_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/linked_identifiers_api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/names_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/ngd_crs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24199 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/ngd_merge_geojsons_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/ngd_query_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/places_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/data/utils_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/run_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_clean_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_downloads_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_extent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_features_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_grow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_linked_identifiers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_names_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_ngd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_places_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-12 14:40:17.000000 osdatahub-1.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.939198 osdatahub-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-24 14:28:21.000000 osdatahub-1.2.4/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.911196 osdatahub-1.2.4/Examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/CRS pitfalls.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   231081 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Converting API Results into Common Data Formats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1837789 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Defining Extents for API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Filtering Attributes for API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Interactive Plotting for API Results - Folium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   945983 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Post Processing API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Quick Start Guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Setting up an API key.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    86367 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/Using the NGD Features API.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.919196 osdatahub-1.2.4/Examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  2124067 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/1_homescreen.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   178174 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/2_sign_up.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)  1883255 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/3_datahub_homepage.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   115385 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/4_new_project.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   153664 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/5_add_api_to_project.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   113078 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/6_view_api_key.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)  1790610 2023-04-24 14:28:21.000000 osdatahub-1.2.4/Examples/images/CRS.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-04-24 14:28:21.000000 osdatahub-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 14:28:21.000000 osdatahub-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-24 14:28:50.939198 osdatahub-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-24 14:28:21.000000 osdatahub-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.923197 osdatahub-1.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/DownloadsAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/Extent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/FeaturesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/LinkedIdentifiersAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/NGD.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/NamesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/PlacesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/Utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.923197 osdatahub-1.2.4/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/media/os-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/readme_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 14:28:21.000000 osdatahub-1.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.923197 osdatahub-1.2.4/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-24 14:28:21.000000 osdatahub-1.2.4/media/os-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 14:28:21.000000 osdatahub-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 14:28:21.000000 osdatahub-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-24 14:28:50.939198 osdatahub-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 14:28:21.000000 osdatahub-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.903195 osdatahub-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.927197 osdatahub-1.2.4/src/osdatahub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.927197 osdatahub-1.2.4/src/osdatahub/DownloadsAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/DownloadsAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/DownloadsAPI/data_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/DownloadsAPI/downloads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/DownloadsAPI/opendata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.931197 osdatahub-1.2.4/src/osdatahub/FeaturesAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/FeaturesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/FeaturesAPI/feature_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/FeaturesAPI/features_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.931197 osdatahub-1.2.4/src/osdatahub/LinkedIdentifiersAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/LinkedIdentifiersAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.931197 osdatahub-1.2.4/src/osdatahub/NGD/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/NGD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/NGD/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/NGD/ngd_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.931197 osdatahub-1.2.4/src/osdatahub/NamesAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/NamesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/NamesAPI/local_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/NamesAPI/names_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.931197 osdatahub-1.2.4/src/osdatahub/PlacesAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/PlacesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/PlacesAPI/places_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/grow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/ons_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/requests_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/spatial_filter_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-24 14:28:21.000000 osdatahub-1.2.4/src/osdatahub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.927197 osdatahub-1.2.4/src/osdatahub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-24 14:28:50.000000 osdatahub-1.2.4/src/osdatahub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-24 14:28:50.000000 osdatahub-1.2.4/src/osdatahub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:28:50.000000 osdatahub-1.2.4/src/osdatahub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 14:28:50.000000 osdatahub-1.2.4/src/osdatahub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 14:28:50.000000 osdatahub-1.2.4/src/osdatahub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.935198 osdatahub-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.935198 osdatahub-1.2.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.935198 osdatahub-1.2.4/tests/data/clean_polygon_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.939198 osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/
+-rw-r--r--   0 runner    (1001) docker     (123)    29650 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    45345 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    32875 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:50.939198 osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/
+-rw-r--r--   0 runner    (1001) docker     (123)    37512 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    58496 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    33032 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data/get_uncleaned_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/clean_polygon_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/downloads_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/extent_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/features_api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/filters_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/linked_identifiers_api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/names_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/ngd_crs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24199 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/ngd_merge_geojsons_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/ngd_query_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/places_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/data/utils_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/run_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_clean_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_downloads_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_features_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_grow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_linked_identifiers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_names_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_ngd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_places_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-24 14:28:21.000000 osdatahub-1.2.4/tox.ini
```

### Comparing `osdatahub-1.2.3/.readthedocs.yaml` & `osdatahub-1.2.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/CRS pitfalls.ipynb` & `osdatahub-1.2.4/Examples/CRS pitfalls.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Converting API Results into Common Data Formats.ipynb` & `osdatahub-1.2.4/Examples/Converting API Results into Common Data Formats.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Defining Extents for API Queries.ipynb` & `osdatahub-1.2.4/Examples/Defining Extents for API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Filtering Attributes for API Queries.ipynb` & `osdatahub-1.2.4/Examples/Filtering Attributes for API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Interactive Plotting for API Results - Folium.ipynb` & `osdatahub-1.2.4/Examples/Interactive Plotting for API Results - Folium.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb` & `osdatahub-1.2.4/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Post Processing API Queries.ipynb` & `osdatahub-1.2.4/Examples/Post Processing API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Quick Start Guide.ipynb` & `osdatahub-1.2.4/Examples/Quick Start Guide.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Setting up an API key.ipynb` & `osdatahub-1.2.4/Examples/Setting up an API key.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/Using the NGD Features API.ipynb` & `osdatahub-1.2.4/Examples/Using the NGD Features API.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/1_homescreen.PNG` & `osdatahub-1.2.4/Examples/images/1_homescreen.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/2_sign_up.PNG` & `osdatahub-1.2.4/Examples/images/2_sign_up.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/3_datahub_homepage.PNG` & `osdatahub-1.2.4/Examples/images/3_datahub_homepage.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/4_new_project.PNG` & `osdatahub-1.2.4/Examples/images/4_new_project.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/5_add_api_to_project.PNG` & `osdatahub-1.2.4/Examples/images/5_add_api_to_project.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/6_view_api_key.PNG` & `osdatahub-1.2.4/Examples/images/6_view_api_key.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/Examples/images/CRS.png` & `osdatahub-1.2.4/Examples/images/CRS.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/LICENSE.txt` & `osdatahub-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/PKG-INFO` & `osdatahub-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdatahub
-Version: 1.2.3
+Version: 1.2.4
 Summary: osdatahub is Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS Data Hub APIs readily accessible to developers.
 Home-page: https://github.com/OrdnanceSurvey/osdatahub
 Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping
 Author-email: rapidprototyping@os.uk
 License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osdatahub Version: 1.2.3 Summary: osdatahub is
+Metadata-Version: 2.1 Name: osdatahub Version: 1.2.4 Summary: osdatahub is
 Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS
 Data Hub APIs readily accessible to developers. Home-page: https://github.com/
 OrdnanceSurvey/osdatahub Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping Author-email: rapidprototyping@os.uk License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub Project-URL:
 Documentation, https://osdatahub.readthedocs.io/en/latest/ Project-URL: Issues,
 https://github.com/OrdnanceSurvey/osdatahub/issues Keywords: Ordnance-
```

### Comparing `osdatahub-1.2.3/README.md` & `osdatahub-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/docs/Utilities.rst` & `osdatahub-1.2.4/docs/Utilities.rst`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/docs/conf.py` & `osdatahub-1.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/docs/index.rst` & `osdatahub-1.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/docs/media/os-logo.png` & `osdatahub-1.2.4/docs/media/os-logo.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/media/os-logo.png` & `osdatahub-1.2.4/media/os-logo.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/setup.cfg` & `osdatahub-1.2.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osdatahub
-version = 1.2.3
+version = 1.2.4
 author = OS Rapid Prototyping
 author_email = rapidprototyping@os.uk
 classifiers = 
 	Natural Language :: English
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Programming Language :: Python :: 3.7
```

### Comparing `osdatahub-1.2.3/src/osdatahub/DownloadsAPI/data_package.py` & `osdatahub-1.2.4/src/osdatahub/DownloadsAPI/data_package.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/DownloadsAPI/downloads_api.py` & `osdatahub-1.2.4/src/osdatahub/DownloadsAPI/downloads_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,28 +39,28 @@
         output_path = os.path.join(output_dir, self.file_name)
 
         if os.path.isfile(output_path) and not overwrite:
             logging.warning(f"Overwrite is set to False and there is a file already in the location {output_path}. "
                             f"Skipping download...")
             return output_path
 
-        response = osdatahub.get(self.url, stream=True, proxies=osdatahub.get_proxies())
+        response = requests.get(self.url, stream=True, proxies=osdatahub.get_proxies())
         response.raise_for_status()
         size = int(response.headers.get('content-length'))
         chunk_size = 1024
         if response.status_code == 200:
             with open(output_path, 'wb') as f:
                 if not pbar:
                     pbar = tqdm(total=size, desc=self.file_name, unit="B", unit_scale=True, leave=True)
                 for chunk in response.iter_content(chunk_size=chunk_size):
                     f.write(chunk)
                     f.flush()
                     pbar.update(chunk_size)
 
-        pbar.write(f"Finished downloading {self.file_name} to {output_path}")
+        # pbar.write(f"Finished downloading {self.file_name} to {output_path}")
         return output_path
 
 
 class _DownloadsAPIBase(ABC):
     """Parent class for Product and DataPackage classes as part of the DownloadsAPI
     (https://osdatahub.os.uk/docs/downloads/overview)
 
@@ -150,21 +150,21 @@
 
         # downloads in parallel if multiple files need to be downloaded
         if isinstance(download_list, list) and len(download_list) > 1 and download_multiple:
             if not processes:
                 processes = cpu_count()
             with ThreadPoolExecutor(max_workers=processes) as executor:
                 pbar = tqdm(total=sum([d.size for d in download_list]), unit="B", unit_scale=True, leave=True,
-                            desc=f"Downloading {len(download_list)} files from osdatahub")
+                            desc=f"Downloaded 0/{len(download_list)} files from osdatahub")
                 results = list([executor.submit(p.download, output_dir, overwrite, pbar) for p in download_list])
 
                 num_downloads_completed = 0
                 for _ in as_completed(results):
                     num_downloads_completed += 1
                     pbar.set_description(
-                        f"Downloading {len(download_list) - num_downloads_completed} files from osdatahub")
+                        f"Downloaded {num_downloads_completed}/{len(download_list)} files from osdatahub")
         else:
             # download single file
             d = download_list[0] if isinstance(download_list, list) else download_list
             results = [d.download(output_dir, overwrite)]
 
         return results
```

### Comparing `osdatahub-1.2.3/src/osdatahub/DownloadsAPI/opendata.py` & `osdatahub-1.2.4/src/osdatahub/DownloadsAPI/opendata.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/FeaturesAPI/feature_products.py` & `osdatahub-1.2.4/src/osdatahub/FeaturesAPI/feature_products.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/FeaturesAPI/features_api.py` & `osdatahub-1.2.4/src/osdatahub/FeaturesAPI/features_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py` & `osdatahub-1.2.4/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py` & `osdatahub-1.2.4/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/NGD/crs.py` & `osdatahub-1.2.4/src/osdatahub/NGD/crs.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/NGD/ngd_api.py` & `osdatahub-1.2.4/src/osdatahub/NGD/ngd_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/NamesAPI/local_types.py` & `osdatahub-1.2.4/src/osdatahub/NamesAPI/local_types.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/NamesAPI/names_api.py` & `osdatahub-1.2.4/src/osdatahub/NamesAPI/names_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/PlacesAPI/places_api.py` & `osdatahub-1.2.4/src/osdatahub/PlacesAPI/places_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/__init__.py` & `osdatahub-1.2.4/src/osdatahub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def set_proxies(proxies):
     os.environ["_OSDATAHUB_PROXIES"] = json.dumps(proxies)
 
 def get_proxies():
     return json.loads(os.environ["_OSDATAHUB_PROXIES"])
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 
 from osdatahub.extent import Extent
 from osdatahub.FeaturesAPI import FeaturesAPI
 from osdatahub.PlacesAPI import PlacesAPI
 from osdatahub.NamesAPI import NamesAPI
 from osdatahub.LinkedIdentifiersAPI import LinkedIdentifiersAPI
 from osdatahub.DownloadsAPI import OpenDataDownload, DataPackageDownload
```

### Comparing `osdatahub-1.2.3/src/osdatahub/bbox.py` & `osdatahub-1.2.4/src/osdatahub/bbox.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/codes.py` & `osdatahub-1.2.4/src/osdatahub/codes.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/errors.py` & `osdatahub-1.2.4/src/osdatahub/errors.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/extent.py` & `osdatahub-1.2.4/src/osdatahub/extent.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/filters.py` & `osdatahub-1.2.4/src/osdatahub/filters.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/grow_list.py` & `osdatahub-1.2.4/src/osdatahub/grow_list.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/ons_api.py` & `osdatahub-1.2.4/src/osdatahub/ons_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/requests_wrapper.py` & `osdatahub-1.2.4/src/osdatahub/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/spatial_filter_types.py` & `osdatahub-1.2.4/src/osdatahub/spatial_filter_types.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub/utils.py` & `osdatahub-1.2.4/src/osdatahub/utils.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/src/osdatahub.egg-info/PKG-INFO` & `osdatahub-1.2.4/src/osdatahub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdatahub
-Version: 1.2.3
+Version: 1.2.4
 Summary: osdatahub is Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS Data Hub APIs readily accessible to developers.
 Home-page: https://github.com/OrdnanceSurvey/osdatahub
 Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping
 Author-email: rapidprototyping@os.uk
 License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osdatahub Version: 1.2.3 Summary: osdatahub is
+Metadata-Version: 2.1 Name: osdatahub Version: 1.2.4 Summary: osdatahub is
 Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS
 Data Hub APIs readily accessible to developers. Home-page: https://github.com/
 OrdnanceSurvey/osdatahub Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping Author-email: rapidprototyping@os.uk License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub Project-URL:
 Documentation, https://osdatahub.readthedocs.io/en/latest/ Project-URL: Issues,
 https://github.com/OrdnanceSurvey/osdatahub/issues Keywords: Ordnance-
```

### Comparing `osdatahub-1.2.3/src/osdatahub.egg-info/SOURCES.txt` & `osdatahub-1.2.4/src/osdatahub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson` & `osdatahub-1.2.4/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data/get_uncleaned_polygons.py` & `osdatahub-1.2.4/tests/data/clean_polygon_data/get_uncleaned_polygons.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/clean_polygon_data.py` & `osdatahub-1.2.4/tests/data/clean_polygon_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/downloads_data.py` & `osdatahub-1.2.4/tests/data/downloads_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/extent_data.py` & `osdatahub-1.2.4/tests/data/extent_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/features_api_data.py` & `osdatahub-1.2.4/tests/data/features_api_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/filters_data.py` & `osdatahub-1.2.4/tests/data/filters_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/linked_identifiers_api_data.py` & `osdatahub-1.2.4/tests/data/linked_identifiers_api_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/names_data.py` & `osdatahub-1.2.4/tests/data/names_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/ngd_crs_data.py` & `osdatahub-1.2.4/tests/data/ngd_crs_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/ngd_merge_geojsons_data.py` & `osdatahub-1.2.4/tests/data/ngd_merge_geojsons_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/ngd_query_data.py` & `osdatahub-1.2.4/tests/data/ngd_query_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/places_data.py` & `osdatahub-1.2.4/tests/data/places_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/data/utils_data.py` & `osdatahub-1.2.4/tests/data/utils_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/run_functions.py` & `osdatahub-1.2.4/tests/run_functions.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_downloads_api.py` & `osdatahub-1.2.4/tests/test_downloads_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import os
+import tempfile
 import unittest.mock as mock
+import dotenv
+
+dotenv.load_dotenv()
 
 import pytest
 from osdatahub import OpenDataDownload, DataPackageDownload
 from osdatahub.DownloadsAPI.downloads_api import _DownloadObj
 
 from tests.data import downloads_data as data
 
@@ -66,14 +70,27 @@
 
 class TestDataPackage:
     @pytest.fixture()
     def data_package(self):
         data_package = DataPackageDownload(key="test_key", product_id="test_id")
         yield data_package
 
+    @pytest.mark.skipif(API_KEY is None, reason="Test API key not available")
+    def test_download_pass(self):
+        # Arrange
+        product_package = DataPackageDownload(API_KEY, "98")
+        files_to_download = product_package.product_list("156")
+
+        # Act
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            downloaded = product_package.download("156", tmpdirname)
+
+        # Assert
+        assert len(downloaded) == len(files_to_download["downloads"])
+
     def test_download_list_pass(self):
         # TODO: implement download_list_pass
         pass
 
     def test_download_list_fail(self):
         # TODO: implement download_list_fail
         pass
```

### Comparing `osdatahub-1.2.3/tests/test_extent.py` & `osdatahub-1.2.4/tests/test_extent.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_features_api.py` & `osdatahub-1.2.4/tests/test_features_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_filters.py` & `osdatahub-1.2.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_grow_list.py` & `osdatahub-1.2.4/tests/test_grow_list.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_linked_identifiers_api.py` & `osdatahub-1.2.4/tests/test_linked_identifiers_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_names_api.py` & `osdatahub-1.2.4/tests/test_names_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_ngd.py` & `osdatahub-1.2.4/tests/test_ngd.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_places_api.py` & `osdatahub-1.2.4/tests/test_places_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.3/tests/test_utils.py` & `osdatahub-1.2.4/tests/test_utils.py`

 * *Files identical despite different names*

