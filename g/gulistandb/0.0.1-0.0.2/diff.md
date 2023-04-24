# Comparing `tmp/gulistandb-0.0.1.tar.gz` & `tmp/gulistandb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulistandb-0.0.1.tar", last modified: Sun Apr 23 16:55:33 2023, max compression
+gzip compressed data, was "gulistandb-0.0.2.tar", last modified: Mon Apr 24 07:41:34 2023, max compression
```

## Comparing `gulistandb-0.0.1.tar` & `gulistandb-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:55:33.237630 gulistandb-0.0.1/
--rw-rw-rw-   0        0        0    34917 2023-04-23 16:50:50.000000 gulistandb-0.0.1/License
--rw-rw-rw-   0        0        0      191 2023-04-23 16:55:33.231634 gulistandb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-04-22 15:15:50.000000 gulistandb-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-23 16:55:33.237630 gulistandb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-04-23 16:42:25.000000 gulistandb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:55:33.174672 gulistandb-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:55:33.226649 gulistandb-0.0.1/src/gulistandb.egg-info/
--rw-rw-rw-   0        0        0      191 2023-04-23 16:55:32.000000 gulistandb-0.0.1/src/gulistandb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-23 16:55:33.000000 gulistandb-0.0.1/src/gulistandb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:55:32.000000 gulistandb-0.0.1/src/gulistandb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 16:55:32.000000 gulistandb-0.0.1/src/gulistandb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 16:55:32.000000 gulistandb-0.0.1/src/gulistandb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4694 2023-04-22 14:38:34.000000 gulistandb-0.0.1/src/main.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:41:34.310097 gulistandb-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-04-24 06:50:57.000000 gulistandb-0.0.2/License
+-rw-rw-rw-   0        0        0     4492 2023-04-24 07:41:34.305102 gulistandb-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3720 2023-04-24 07:21:02.000000 gulistandb-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:41:34.320091 gulistandb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1021 2023-04-24 07:40:50.000000 gulistandb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:41:34.247137 gulistandb-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:38:14.000000 gulistandb-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:41:34.301103 gulistandb-0.0.2/src/gulistandb.egg-info/
+-rw-rw-rw-   0        0        0     4492 2023-04-24 07:41:33.000000 gulistandb-0.0.2/src/gulistandb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-24 07:41:33.000000 gulistandb-0.0.2/src/gulistandb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:41:33.000000 gulistandb-0.0.2/src/gulistandb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 07:41:33.000000 gulistandb-0.0.2/src/gulistandb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-24 07:41:33.000000 gulistandb-0.0.2/src/gulistandb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4089 2023-04-24 06:51:18.000000 gulistandb-0.0.2/src/gulistandb.py
```

