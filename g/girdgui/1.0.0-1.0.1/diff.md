# Comparing `tmp/girdgui-1.0.0.tar.gz` & `tmp/girdgui-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girdgui-1.0.0.tar", last modified: Fri Apr 21 11:17:04 2023, max compression
+gzip compressed data, was "girdgui-1.0.1.tar", last modified: Mon Apr 24 12:17:11 2023, max compression
```

## Comparing `girdgui-1.0.0.tar` & `girdgui-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:17:04.446397 girdgui-1.0.0/
--rw-rw-rw-   0        0        0       99 2023-04-21 11:17:04.445399 girdgui-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 11:17:04.443396 girdgui-1.0.0/girdgui.egg-info/
--rw-rw-rw-   0        0        0       99 2023-04-21 11:17:04.000000 girdgui-1.0.0/girdgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-04-21 11:17:04.000000 girdgui-1.0.0/girdgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:17:04.000000 girdgui-1.0.0/girdgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:17:04.000000 girdgui-1.0.0/girdgui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:17:04.446397 girdgui-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      198 2023-04-21 11:10:20.000000 girdgui-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.780628 girdgui-1.0.1/
+-rw-rw-rw-   0        0        0     1192 2023-04-24 12:17:11.774630 girdgui-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:17:11.780628 girdgui-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-04-24 12:17:06.000000 girdgui-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.736628 girdgui-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.740627 girdgui-1.0.1/src/girdgui/
+-rw-rw-rw-   0        0        0      932 2023-03-25 13:38:07.000000 girdgui-1.0.1/src/girdgui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:11.771628 girdgui-1.0.1/src/girdgui.egg-info/
+-rw-rw-rw-   0        0        0     1192 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 12:17:11.000000 girdgui-1.0.1/src/girdgui.egg-info/top_level.txt
```

