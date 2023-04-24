# Comparing `tmp/AegosIN-0.1.tar.gz` & `tmp/AegosIN-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AegosIN-0.1.tar", last modified: Mon Apr 24 00:42:17 2023, max compression
+gzip compressed data, was "AegosIN-0.2.tar", last modified: Mon Apr 24 13:59:41 2023, max compression
```

## Comparing `AegosIN-0.1.tar` & `AegosIN-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 00:42:17.903342 AegosIN-0.1/
-drwxrwxrwx   0        0        0        0 2023-04-24 00:42:17.854371 AegosIN-0.1/AegosIN/
--rw-rw-rw-   0        0        0       27 2023-04-24 00:40:15.000000 AegosIN-0.1/AegosIN/__init__.py
--rw-rw-rw-   0        0        0      689 2023-04-24 00:39:42.000000 AegosIN-0.1/AegosIN/in_tik.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:42:17.896361 AegosIN-0.1/AegosIN.egg-info/
--rw-rw-rw-   0        0        0      348 2023-04-24 00:42:17.000000 AegosIN-0.1/AegosIN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-24 00:42:17.000000 AegosIN-0.1/AegosIN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 00:42:17.000000 AegosIN-0.1/AegosIN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 00:42:17.000000 AegosIN-0.1/AegosIN.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-24 00:42:17.000000 AegosIN-0.1/AegosIN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      348 2023-04-24 00:42:17.901352 AegosIN-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 00:42:17.904341 AegosIN-0.1/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-04-24 00:41:57.000000 AegosIN-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:59:41.726935 AegosIN-0.2/
+drwxrwxrwx   0        0        0        0 2023-04-24 13:59:41.688139 AegosIN-0.2/AegosIN/
+-rw-rw-rw-   0        0        0       27 2023-04-24 00:40:15.000000 AegosIN-0.2/AegosIN/__init__.py
+-rw-rw-rw-   0        0        0      689 2023-04-24 00:39:42.000000 AegosIN-0.2/AegosIN/in_tik.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:59:41.722967 AegosIN-0.2/AegosIN.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-24 13:59:41.000000 AegosIN-0.2/AegosIN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-04-24 13:59:41.000000 AegosIN-0.2/AegosIN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:59:41.000000 AegosIN-0.2/AegosIN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 13:59:41.000000 AegosIN-0.2/AegosIN.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-04-24 13:59:41.000000 AegosIN-0.2/AegosIN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      303 2023-04-24 13:59:41.724942 AegosIN-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:59:41.727932 AegosIN-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-04-24 13:59:01.000000 AegosIN-0.2/setup.py
```

### Comparing `AegosIN-0.1/AegosIN/in_tik.py` & `AegosIN-0.2/AegosIN/in_tik.py`

 * *Files identical despite different names*

