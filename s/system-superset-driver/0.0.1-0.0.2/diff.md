# Comparing `tmp/system_superset_driver-0.0.1.tar.gz` & `tmp/system_superset_driver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_superset_driver-0.0.1.tar", last modified: Mon Apr 24 07:22:44 2023, max compression
+gzip compressed data, was "system_superset_driver-0.0.2.tar", last modified: Mon Apr 24 07:32:48 2023, max compression
```

## Comparing `system_superset_driver-0.0.1.tar` & `system_superset_driver-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:22:44.258880 system_superset_driver-0.0.1/
--rw-rw-rw-   0        0        0      157 2023-04-24 07:22:44.258880 system_superset_driver-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 07:22:44.259849 system_superset_driver-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      267 2023-04-24 07:22:43.000000 system_superset_driver-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:22:44.253694 system_superset_driver-0.0.1/system_superset_driver.egg-info/
--rw-rw-rw-   0        0        0      157 2023-04-24 07:22:44.000000 system_superset_driver-0.0.1/system_superset_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-24 07:22:44.000000 system_superset_driver-0.0.1/system_superset_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:22:44.000000 system_superset_driver-0.0.1/system_superset_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-24 07:22:44.000000 system_superset_driver-0.0.1/system_superset_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:22:44.000000 system_superset_driver-0.0.1/system_superset_driver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 07:32:48.488113 system_superset_driver-0.0.2/
+-rw-rw-rw-   0        0        0      157 2023-04-24 07:32:48.487116 system_superset_driver-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:32:48.488113 system_superset_driver-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      271 2023-04-24 07:32:46.000000 system_superset_driver-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:32:48.487116 system_superset_driver-0.0.2/system_superset_driver.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-04-24 07:32:48.000000 system_superset_driver-0.0.2/system_superset_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-24 07:32:48.000000 system_superset_driver-0.0.2/system_superset_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:32:48.000000 system_superset_driver-0.0.2/system_superset_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-24 07:32:48.000000 system_superset_driver-0.0.2/system_superset_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:32:48.000000 system_superset_driver-0.0.2/system_superset_driver.egg-info/top_level.txt
```

