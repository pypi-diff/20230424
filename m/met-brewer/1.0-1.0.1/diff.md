# Comparing `tmp/met-brewer-1.0.tar.gz` & `tmp/met-brewer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "met-brewer-1.0.tar", last modified: Sat Apr 22 15:28:57 2023, max compression
+gzip compressed data, was "met-brewer-1.0.1.tar", last modified: Mon Apr 24 09:43:47 2023, max compression
```

## Comparing `met-brewer-1.0.tar` & `met-brewer-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 15:28:57.449151 met-brewer-1.0/
--rw-rw-rw-   0        0        0       55 2023-04-22 15:28:57.448151 met-brewer-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 15:28:57.434166 met-brewer-1.0/met_brewer/
--rw-rw-rw-   0        0        0      248 2023-04-22 15:17:59.000000 met-brewer-1.0/met_brewer/__init__.py
--rw-rw-rw-   0        0        0    13272 2023-04-22 15:17:59.000000 met-brewer-1.0/met_brewer/palettes.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:28:57.445152 met-brewer-1.0/met_brewer.egg-info/
--rw-rw-rw-   0        0        0       55 2023-04-22 15:28:57.000000 met-brewer-1.0/met_brewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-22 15:28:57.000000 met-brewer-1.0/met_brewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 15:28:57.000000 met-brewer-1.0/met_brewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-22 15:28:57.000000 met-brewer-1.0/met_brewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 15:28:57.000000 met-brewer-1.0/met_brewer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 15:28:57.449151 met-brewer-1.0/setup.cfg
--rw-rw-rw-   0        0        0      193 2023-04-22 15:17:59.000000 met-brewer-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:43:47.757023 met-brewer-1.0.1/
+-rw-rw-rw-   0        0        0    21147 2023-04-24 09:43:47.755028 met-brewer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20561 2023-04-24 08:58:03.000000 met-brewer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:43:47.739030 met-brewer-1.0.1/met_brewer/
+-rw-rw-rw-   0        0        0      265 2023-04-22 19:04:51.000000 met-brewer-1.0.1/met_brewer/__init__.py
+-rw-rw-rw-   0        0        0    19399 2023-04-24 08:45:56.000000 met-brewer-1.0.1/met_brewer/palettes.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:43:47.752025 met-brewer-1.0.1/met_brewer.egg-info/
+-rw-rw-rw-   0        0        0    21147 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 09:43:47.000000 met-brewer-1.0.1/met_brewer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:43:47.757023 met-brewer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      420 2023-04-24 09:41:40.000000 met-brewer-1.0.1/setup.py
```

