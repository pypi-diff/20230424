# Comparing `tmp/system_superset_driver-0.0.5.tar.gz` & `tmp/system_superset_driver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_superset_driver-0.0.5.tar", last modified: Mon Apr 24 07:48:15 2023, max compression
+gzip compressed data, was "system_superset_driver-0.0.6.tar", last modified: Mon Apr 24 07:51:48 2023, max compression
```

## Comparing `system_superset_driver-0.0.5.tar` & `system_superset_driver-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:48:15.107381 system_superset_driver-0.0.5/
--rw-rw-rw-   0        0        0      157 2023-04-24 07:48:15.107381 system_superset_driver-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 07:48:15.107381 system_superset_driver-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      366 2023-04-24 07:48:14.000000 system_superset_driver-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:48:15.106384 system_superset_driver-0.0.5/system_superset_driver.egg-info/
--rw-rw-rw-   0        0        0      157 2023-04-24 07:48:15.000000 system_superset_driver-0.0.5/system_superset_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-24 07:48:15.000000 system_superset_driver-0.0.5/system_superset_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:48:15.000000 system_superset_driver-0.0.5/system_superset_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-04-24 07:48:15.000000 system_superset_driver-0.0.5/system_superset_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:48:15.000000 system_superset_driver-0.0.5/system_superset_driver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 07:51:48.502005 system_superset_driver-0.0.6/
+-rw-rw-rw-   0        0        0      157 2023-04-24 07:51:48.501008 system_superset_driver-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:51:48.502005 system_superset_driver-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      370 2023-04-24 07:51:48.000000 system_superset_driver-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:51:48.501008 system_superset_driver-0.0.6/system_superset_driver.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-04-24 07:51:48.000000 system_superset_driver-0.0.6/system_superset_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-24 07:51:48.000000 system_superset_driver-0.0.6/system_superset_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:51:48.000000 system_superset_driver-0.0.6/system_superset_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-04-24 07:51:48.000000 system_superset_driver-0.0.6/system_superset_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:51:48.000000 system_superset_driver-0.0.6/system_superset_driver.egg-info/top_level.txt
```

