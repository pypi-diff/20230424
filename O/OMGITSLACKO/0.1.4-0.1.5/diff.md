# Comparing `tmp/OMGITSLACKO-0.1.4.tar.gz` & `tmp/OMGITSLACKO-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMGITSLACKO-0.1.4.tar", last modified: Sat Apr 22 10:55:36 2023, max compression
+gzip compressed data, was "OMGITSLACKO-0.1.5.tar", last modified: Mon Apr 24 07:34:31 2023, max compression
```

## Comparing `OMGITSLACKO-0.1.4.tar` & `OMGITSLACKO-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 10:55:36.982061 OMGITSLACKO-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-22 10:55:36.974040 OMGITSLACKO-0.1.4/OMGITSLACKO/
--rw-rw-rw-   0        0        0      195 2023-04-22 10:43:33.000000 OMGITSLACKO-0.1.4/OMGITSLACKO/__init__.py
--rw-rw-rw-   0        0        0    11508 2023-04-21 22:28:48.000000 OMGITSLACKO-0.1.4/OMGITSLACKO/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-22 10:55:36.980056 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/
--rw-rw-rw-   0        0        0      235 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 10:55:36.000000 OMGITSLACKO-0.1.4/OMGITSLACKO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-04-22 10:55:36.981129 OMGITSLACKO-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 10:55:36.982061 OMGITSLACKO-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-04-22 10:55:04.000000 OMGITSLACKO-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:34:31.530947 OMGITSLACKO-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-04-24 07:34:31.521923 OMGITSLACKO-0.1.5/OMGITSLACKO/
+-rw-rw-rw-   0        0        0      340 2023-04-24 07:33:25.000000 OMGITSLACKO-0.1.5/OMGITSLACKO/__init__.py
+-rw-rw-rw-   0        0        0    21142 2023-04-24 07:33:31.000000 OMGITSLACKO-0.1.5/OMGITSLACKO/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:34:31.527938 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-04-24 07:34:31.000000 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-24 07:34:31.000000 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:34:31.000000 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 11:06:38.000000 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-24 07:34:31.000000 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 07:34:31.000000 OMGITSLACKO-0.1.5/OMGITSLACKO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-04-24 07:34:31.530024 OMGITSLACKO-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-21 12:10:35.000000 OMGITSLACKO-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:34:31.530947 OMGITSLACKO-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      399 2023-04-24 07:34:00.000000 OMGITSLACKO-0.1.5/setup.py
```

