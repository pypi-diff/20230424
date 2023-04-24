# Comparing `tmp/revistas-0.1.tar.gz` & `tmp/revistas-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revistas-0.1.tar", last modified: Mon Apr 24 08:08:24 2023, max compression
+gzip compressed data, was "revistas-1.0.0.tar", last modified: Mon Apr 24 08:37:54 2023, max compression
```

## Comparing `revistas-0.1.tar` & `revistas-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:08:24.821802 revistas-0.1/
--rw-rw-rw-   0        0        0      596 2023-04-24 08:08:24.811801 revistas-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      476 2023-04-24 08:03:41.000000 revistas-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 08:08:24.793800 revistas-0.1/revistas.egg-info/
--rw-rw-rw-   0        0        0      596 2023-04-24 08:08:21.000000 revistas-0.1/revistas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-04-24 08:08:22.000000 revistas-0.1/revistas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:08:21.000000 revistas-0.1/revistas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 08:08:21.000000 revistas-0.1/revistas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:08:21.000000 revistas-0.1/revistas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 08:08:24.826802 revistas-0.1/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-04-24 08:06:36.000000 revistas-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:37:53.922956 revistas-1.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 revistas-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1013 2023-04-24 08:37:53.913956 revistas-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-04-24 08:24:48.000000 revistas-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:37:53.794949 revistas-1.0.0/revistas/
+-rw-rw-rw-   0        0        0     1372 2023-04-24 07:44:24.000000 revistas-1.0.0/revistas/client.py
+-rw-rw-rw-   0        0        0       75 2023-04-24 08:31:10.000000 revistas-1.0.0/revistas/version.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:37:53.894955 revistas-1.0.0/revistas.egg-info/
+-rw-rw-rw-   0        0        0     1013 2023-04-24 08:37:49.000000 revistas-1.0.0/revistas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-04-24 08:37:52.000000 revistas-1.0.0/revistas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:37:49.000000 revistas-1.0.0/revistas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 08:37:49.000000 revistas-1.0.0/revistas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 08:37:49.000000 revistas-1.0.0/revistas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 08:37:49.000000 revistas-1.0.0/revistas.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:37:53.927956 revistas-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1634 2023-04-24 08:37:31.000000 revistas-1.0.0/setup.py
```

