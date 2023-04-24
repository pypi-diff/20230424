# Comparing `tmp/api-Rocket-1.2.0.tar.gz` & `tmp/api-Rocket-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.2.0.tar", last modified: Mon Apr 24 09:31:31 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.3.0.tar", last modified: Mon Apr 24 09:35:22 2023, max compression
```

## Comparing `api-Rocket-1.2.0.tar` & `api-Rocket-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:31:31.297140 api-Rocket-1.2.0/
--rw-rw-rw-   0        0        0       20 2023-04-24 09:31:29.000000 api-Rocket-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      379 2023-04-24 09:31:31.298117 api-Rocket-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 09:31:31.280539 api-Rocket-1.2.0/api_Rocket/
--rw-rw-rw-   0        0        0      671 2023-03-24 14:25:46.000000 api-Rocket-1.2.0/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:31:31.294211 api-Rocket-1.2.0/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      379 2023-04-24 09:31:31.000000 api-Rocket-1.2.0/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-24 09:31:31.000000 api-Rocket-1.2.0/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:31:31.000000 api-Rocket-1.2.0/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 09:31:31.000000 api-Rocket-1.2.0/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 09:31:31.301046 api-Rocket-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      360 2023-04-24 09:31:29.000000 api-Rocket-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:35:22.757101 api-Rocket-1.3.0/
+-rw-rw-rw-   0        0        0       20 2023-04-24 09:35:21.000000 api-Rocket-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      526 2023-04-24 09:35:22.759054 api-Rocket-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 09:35:22.741476 api-Rocket-1.3.0/api_Rocket/
+-rw-rw-rw-   0        0        0      671 2023-03-24 14:25:46.000000 api-Rocket-1.3.0/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:35:22.755148 api-Rocket-1.3.0/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:35:22.763937 api-Rocket-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-04-24 09:35:21.000000 api-Rocket-1.3.0/setup.py
```

### Comparing `api-Rocket-1.2.0/api_Rocket/__init__.py` & `api-Rocket-1.3.0/api_Rocket/__init__.py`

 * *Files identical despite different names*

