# Comparing `tmp/asyncblink-0.3.2.tar.gz` & `tmp/asyncblink-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncblink-0.3.2.tar", last modified: Thu Nov  8 23:37:45 2018, max compression
+gzip compressed data, was "asyncblink-0.4.0.tar", last modified: Mon Apr 24 04:35:28 2023, max compression
```

## Comparing `asyncblink-0.3.2.tar` & `asyncblink-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-11-08 23:37:45.000000 asyncblink-0.3.2/
--rw-r--r--   0 juca      (1000) juca      (1000)     1241 2018-11-08 23:36:22.000000 asyncblink-0.3.2/setup.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1639 2017-12-30 02:45:35.000000 asyncblink-0.3.2/README
--rw-r--r--   0 juca      (1000) juca      (1000)     2975 2018-11-08 23:37:45.000000 asyncblink-0.3.2/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)       38 2018-11-08 23:37:45.000000 asyncblink-0.3.2/setup.cfg
--rw-r--r--   0 juca      (1000) juca      (1000)     2629 2018-11-08 23:29:44.000000 asyncblink-0.3.2/asyncblink.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2018-11-08 23:37:45.000000 asyncblink-0.3.2/asyncblink.egg-info/
--rw-r--r--   0 juca      (1000) juca      (1000)        1 2018-11-08 23:37:45.000000 asyncblink-0.3.2/asyncblink.egg-info/dependency_links.txt
--rw-r--r--   0 juca      (1000) juca      (1000)     2975 2018-11-08 23:37:45.000000 asyncblink-0.3.2/asyncblink.egg-info/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)      198 2018-11-08 23:37:45.000000 asyncblink-0.3.2/asyncblink.egg-info/SOURCES.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       13 2018-11-08 23:37:45.000000 asyncblink-0.3.2/asyncblink.egg-info/requires.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       11 2018-11-08 23:37:45.000000 asyncblink-0.3.2/asyncblink.egg-info/top_level.txt
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-24 04:35:28.629929 asyncblink-0.4.0/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1674 2023-04-24 04:35:28.629929 asyncblink-0.4.0/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1198 2023-04-24 02:41:16.000000 asyncblink-0.4.0/README.md
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-24 04:35:28.629929 asyncblink-0.4.0/asyncblink.egg-info/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1674 2023-04-24 04:35:28.000000 asyncblink-0.4.0/asyncblink.egg-info/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      207 2023-04-24 04:35:28.000000 asyncblink-0.4.0/asyncblink.egg-info/SOURCES.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)        1 2023-04-24 04:35:28.000000 asyncblink-0.4.0/asyncblink.egg-info/dependency_links.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       13 2023-04-24 04:35:28.000000 asyncblink-0.4.0/asyncblink.egg-info/requires.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       11 2023-04-24 04:35:28.000000 asyncblink-0.4.0/asyncblink.egg-info/top_level.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1770 2023-04-24 02:20:50.000000 asyncblink-0.4.0/asyncblink.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)      642 2023-04-24 04:03:43.000000 asyncblink-0.4.0/pyproject.toml
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-04-24 04:35:28.629929 asyncblink-0.4.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

