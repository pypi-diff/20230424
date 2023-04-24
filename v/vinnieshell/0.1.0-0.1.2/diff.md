# Comparing `tmp/vinnieshell-0.1.0.tar.gz` & `tmp/vinnieshell-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinnieshell-0.1.0.tar", last modified: Mon Apr 24 01:32:17 2023, max compression
+gzip compressed data, was "vinnieshell-0.1.2.tar", last modified: Mon Apr 24 01:59:57 2023, max compression
```

## Comparing `vinnieshell-0.1.0.tar` & `vinnieshell-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-24 01:32:17.225695 vinnieshell-0.1.0/
--rw-r--r--   0 user      (1000) user      (1000)       53 2023-04-24 01:26:03.000000 vinnieshell-0.1.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      203 2023-04-24 01:32:17.225695 vinnieshell-0.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      835 2023-04-24 01:05:41.000000 vinnieshell-0.1.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-24 01:32:17.225695 vinnieshell-0.1.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      457 2023-04-24 01:28:58.000000 vinnieshell-0.1.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-24 01:32:17.225695 vinnieshell-0.1.0/vinnieshell.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      203 2023-04-24 01:32:17.000000 vinnieshell-0.1.0/vinnieshell.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      242 2023-04-24 01:32:17.000000 vinnieshell-0.1.0/vinnieshell.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-24 01:32:17.000000 vinnieshell-0.1.0/vinnieshell.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       49 2023-04-24 01:32:17.000000 vinnieshell-0.1.0/vinnieshell.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)        9 2023-04-24 01:32:17.000000 vinnieshell-0.1.0/vinnieshell.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-24 01:32:17.000000 vinnieshell-0.1.0/vinnieshell.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-24 01:59:57.837732 vinnieshell-0.1.2/
+-rw-r--r--   0 user      (1000) user      (1000)       53 2023-04-24 01:26:03.000000 vinnieshell-0.1.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      203 2023-04-24 01:59:57.837732 vinnieshell-0.1.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      835 2023-04-24 01:05:41.000000 vinnieshell-0.1.2/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-24 01:59:57.837732 vinnieshell-0.1.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      450 2023-04-24 01:59:07.000000 vinnieshell-0.1.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-24 01:59:57.837732 vinnieshell-0.1.2/vinnieshell.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      203 2023-04-24 01:59:57.000000 vinnieshell-0.1.2/vinnieshell.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      242 2023-04-24 01:59:57.000000 vinnieshell-0.1.2/vinnieshell.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-24 01:59:57.000000 vinnieshell-0.1.2/vinnieshell.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       42 2023-04-24 01:59:57.000000 vinnieshell-0.1.2/vinnieshell.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2023-04-24 01:59:57.000000 vinnieshell-0.1.2/vinnieshell.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-24 01:59:57.000000 vinnieshell-0.1.2/vinnieshell.egg-info/top_level.txt
```

### Comparing `vinnieshell-0.1.0/README.md` & `vinnieshell-0.1.2/README.md`

 * *Files identical despite different names*

