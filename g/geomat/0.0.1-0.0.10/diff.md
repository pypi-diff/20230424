# Comparing `tmp/geomat-0.0.1.tar.gz` & `tmp/geomat-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomat-0.0.1.tar", last modified: Sun Apr 23 23:34:28 2023, max compression
+gzip compressed data, was "geomat-0.0.10.tar", last modified: Sun Apr 23 23:49:25 2023, max compression
```

## Comparing `geomat-0.0.1.tar` & `geomat-0.0.10.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-23 23:34:28.960092 geomat-0.0.1/
--rw-r--r--   0 mac        (501) admin       (80)      168 2023-04-23 23:34:28.959952 geomat-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) admin       (80)     8191 2023-04-23 22:38:47.000000 geomat-0.0.1/README.md
-drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-23 23:34:28.959747 geomat-0.0.1/geomat.egg-info/
--rw-r--r--   0 mac        (501) admin       (80)      168 2023-04-23 23:34:28.000000 geomat-0.0.1/geomat.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) admin       (80)      167 2023-04-23 23:34:28.000000 geomat-0.0.1/geomat.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-23 23:34:28.000000 geomat-0.0.1/geomat.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) admin       (80)       36 2023-04-23 23:34:28.000000 geomat-0.0.1/geomat.egg-info/requires.txt
--rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-23 23:34:28.000000 geomat-0.0.1/geomat.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) admin       (80)       38 2023-04-23 23:34:28.960166 geomat-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) admin       (80)     1213 2023-04-23 23:34:22.000000 geomat-0.0.1/setup.py
+drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-23 23:49:25.577098 geomat-0.0.10/
+-rw-r--r--   0 mac        (501) admin       (80)     8744 2023-04-23 23:49:25.576230 geomat-0.0.10/PKG-INFO
+-rw-r--r--   0 mac        (501) admin       (80)     8191 2023-04-23 22:38:47.000000 geomat-0.0.10/README.md
+drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-23 23:49:25.576000 geomat-0.0.10/geomat.egg-info/
+-rw-r--r--   0 mac        (501) admin       (80)     8744 2023-04-23 23:49:25.000000 geomat-0.0.10/geomat.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) admin       (80)      167 2023-04-23 23:49:25.000000 geomat-0.0.10/geomat.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-23 23:49:25.000000 geomat-0.0.10/geomat.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) admin       (80)       36 2023-04-23 23:49:25.000000 geomat-0.0.10/geomat.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-23 23:49:25.000000 geomat-0.0.10/geomat.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) admin       (80)       38 2023-04-23 23:49:25.577178 geomat-0.0.10/setup.cfg
+-rw-r--r--   0 mac        (501) admin       (80)     1994 2023-04-23 23:45:56.000000 geomat-0.0.10/setup.py
```

### Comparing `geomat-0.0.1/README.md` & `geomat-0.0.10/README.md`

 * *Files identical despite different names*

