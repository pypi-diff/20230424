# Comparing `tmp/system_superset_driver-0.0.7.tar.gz` & `tmp/system_superset_driver-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_superset_driver-0.0.7.tar", last modified: Mon Apr 24 07:59:15 2023, max compression
+gzip compressed data, was "system_superset_driver-0.0.8.tar", last modified: Mon Apr 24 08:01:34 2023, max compression
```

## Comparing `system_superset_driver-0.0.7.tar` & `system_superset_driver-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:59:15.519917 system_superset_driver-0.0.7/
--rw-rw-rw-   0        0        0      157 2023-04-24 07:59:15.519917 system_superset_driver-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 07:59:15.510942 system_superset_driver-0.0.7/apm_system/
--rw-rw-rw-   0        0        0        0 2023-04-24 07:32:21.000000 system_superset_driver-0.0.7/apm_system/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-04-24 06:56:16.000000 system_superset_driver-0.0.7/apm_system/apm_adapter.py
--rw-rw-rw-   0        0        0     1032 2023-04-24 07:58:06.000000 system_superset_driver-0.0.7/apm_system/apm_dialect.py
--rw-rw-rw-   0        0        0      590 2023-04-24 07:31:18.000000 system_superset_driver-0.0.7/apm_system/db_engine_specs.py
--rw-rw-rw-   0        0        0       42 2023-04-24 07:59:15.519917 system_superset_driver-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      392 2023-04-24 07:59:15.000000 system_superset_driver-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:59:15.518920 system_superset_driver-0.0.7/system_superset_driver.egg-info/
--rw-rw-rw-   0        0        0      157 2023-04-24 07:59:15.000000 system_superset_driver-0.0.7/system_superset_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-04-24 07:59:15.000000 system_superset_driver-0.0.7/system_superset_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:59:15.000000 system_superset_driver-0.0.7/system_superset_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-04-24 07:59:15.000000 system_superset_driver-0.0.7/system_superset_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 07:59:15.000000 system_superset_driver-0.0.7/system_superset_driver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 08:01:34.186977 system_superset_driver-0.0.8/
+-rw-rw-rw-   0        0        0      157 2023-04-24 08:01:34.186977 system_superset_driver-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 08:01:34.171019 system_superset_driver-0.0.8/apm_system/
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:32:21.000000 system_superset_driver-0.0.8/apm_system/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-04-24 06:56:16.000000 system_superset_driver-0.0.8/apm_system/apm_adapter.py
+-rw-rw-rw-   0        0        0     1032 2023-04-24 07:58:06.000000 system_superset_driver-0.0.8/apm_system/apm_dialect.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 07:31:18.000000 system_superset_driver-0.0.8/apm_system/db_engine_specs.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:01:34.186977 system_superset_driver-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-04-24 08:01:33.000000 system_superset_driver-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:01:34.185979 system_superset_driver-0.0.8/system_superset_driver.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/top_level.txt
```

### Comparing `system_superset_driver-0.0.7/apm_system/apm_adapter.py` & `system_superset_driver-0.0.8/apm_system/apm_adapter.py`

 * *Files identical despite different names*

### Comparing `system_superset_driver-0.0.7/apm_system/apm_dialect.py` & `system_superset_driver-0.0.8/apm_system/apm_dialect.py`

 * *Files identical despite different names*

### Comparing `system_superset_driver-0.0.7/apm_system/db_engine_specs.py` & `system_superset_driver-0.0.8/apm_system/db_engine_specs.py`

 * *Files identical despite different names*

