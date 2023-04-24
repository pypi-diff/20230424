# Comparing `tmp/fancybbox-0.0.10.tar.gz` & `tmp/fancybbox-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancybbox-0.0.10.tar", last modified: Sun Apr 23 16:45:59 2023, max compression
+gzip compressed data, was "fancybbox-0.0.11.tar", last modified: Mon Apr 24 01:45:03 2023, max compression
```

## Comparing `fancybbox-0.0.10.tar` & `fancybbox-0.0.11.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:45:59.309766 fancybbox-0.0.10/
--rw-rw-rw-   0        0        0     1067 2023-04-23 16:35:21.000000 fancybbox-0.0.10/LICENSE.txt
--rw-rw-rw-   0        0        0     1202 2023-04-23 16:45:59.305787 fancybbox-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-04-23 16:33:02.000000 fancybbox-0.0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 16:45:59.302766 fancybbox-0.0.10/fancybbox.egg-info/
--rw-rw-rw-   0        0        0     1202 2023-04-23 16:45:58.000000 fancybbox-0.0.10/fancybbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-23 16:45:59.000000 fancybbox-0.0.10/fancybbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:45:58.000000 fancybbox-0.0.10/fancybbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 16:45:58.000000 fancybbox-0.0.10/fancybbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:45:58.000000 fancybbox-0.0.10/fancybbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 16:45:59.309766 fancybbox-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0     1513 2023-04-23 16:24:01.000000 fancybbox-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:45:03.565336 fancybbox-0.0.11/
+-rw-rw-rw-   0        0        0     1067 2023-04-23 16:35:21.000000 fancybbox-0.0.11/LICENSE.txt
+-rw-rw-rw-   0        0        0     1850 2023-04-24 01:45:03.562329 fancybbox-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-04-23 16:33:02.000000 fancybbox-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:45:03.506851 fancybbox-0.0.11/fancybbox/
+-rw-rw-rw-   0        0        0      252 2023-04-24 01:30:58.000000 fancybbox-0.0.11/fancybbox/__init__.py
+-rw-rw-rw-   0        0        0     8283 2023-04-23 15:48:01.000000 fancybbox-0.0.11/fancybbox/fancy_bbox.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:45:03.559333 fancybbox-0.0.11/fancybbox.egg-info/
+-rw-rw-rw-   0        0        0     1850 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 01:45:03.000000 fancybbox-0.0.11/fancybbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:45:03.566333 fancybbox-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-04-24 01:43:55.000000 fancybbox-0.0.11/setup.py
```

### Comparing `fancybbox-0.0.10/LICENSE.txt` & `fancybbox-0.0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancybbox-0.0.10/README.md` & `fancybbox-0.0.11/README.md`

 * *Files identical despite different names*

