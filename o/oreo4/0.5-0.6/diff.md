# Comparing `tmp/oreo4-0.5.tar.gz` & `tmp/oreo4-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oreo4-0.5.tar", last modified: Mon Apr 24 19:30:04 2023, max compression
+gzip compressed data, was "oreo4-0.6.tar", last modified: Mon Apr 24 19:45:49 2023, max compression
```

## Comparing `oreo4-0.5.tar` & `oreo4-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:30:04.006905 oreo4-0.5/
--rw-rw-rw-   0        0        0       28 2023-04-23 08:50:47.000000 oreo4-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      326 2023-04-24 19:30:04.006905 oreo4-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 19:30:03.955950 oreo4-0.5/oreo4/
--rw-rw-rw-   0        0        0       24 2023-04-24 19:19:22.000000 oreo4-0.5/oreo4/__init__.py
--rw-rw-rw-   0        0        0      150 2023-04-24 19:12:04.000000 oreo4-0.5/oreo4/oreoGG.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:30:03.998911 oreo4-0.5/oreo4.egg-info/
--rw-rw-rw-   0        0        0      326 2023-04-24 19:30:03.000000 oreo4-0.5/oreo4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-04-24 19:30:03.000000 oreo4-0.5/oreo4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:30:03.000000 oreo4-0.5/oreo4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 19:30:03.000000 oreo4-0.5/oreo4.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-04-24 19:30:03.000000 oreo4-0.5/oreo4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 19:30:04.008905 oreo4-0.5/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-04-24 19:29:15.000000 oreo4-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:45:49.434140 oreo4-0.6/
+-rw-rw-rw-   0        0        0       28 2023-04-23 08:50:47.000000 oreo4-0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      326 2023-04-24 19:45:49.435140 oreo4-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 19:45:49.395163 oreo4-0.6/oreo4/
+-rw-rw-rw-   0        0        0       25 2023-04-24 19:43:47.000000 oreo4-0.6/oreo4/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-04-24 19:45:22.000000 oreo4-0.6/oreo4/in_ttik.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:45:49.426146 oreo4-0.6/oreo4.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-04-24 19:45:48.000000 oreo4-0.6/oreo4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-04-24 19:45:49.000000 oreo4-0.6/oreo4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:45:48.000000 oreo4-0.6/oreo4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 19:45:48.000000 oreo4-0.6/oreo4.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-24 19:45:48.000000 oreo4-0.6/oreo4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:45:49.437140 oreo4-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-04-24 19:42:36.000000 oreo4-0.6/setup.py
```

