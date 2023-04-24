# Comparing `tmp/kozh_fig_pac2-0.1.tar.gz` & `tmp/kozh_fig_pac2-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kozh_fig_pac2-0.1.tar", last modified: Mon Apr 24 12:53:32 2023, max compression
+gzip compressed data, was "kozh_fig_pac2-0.2.tar", last modified: Mon Apr 24 12:53:58 2023, max compression
```

## Comparing `kozh_fig_pac2-0.1.tar` & `kozh_fig_pac2-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:53:32.080672 kozh_fig_pac2-0.1/
--rw-rw-rw-   0        0        0      132 2023-04-24 12:53:32.081673 kozh_fig_pac2-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 12:53:32.052513 kozh_fig_pac2-0.1/kozh_fig_pac2/
--rw-rw-rw-   0        0        0      315 2023-04-24 08:50:42.000000 kozh_fig_pac2-0.1/kozh_fig_pac2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:53:32.076657 kozh_fig_pac2-0.1/kozh_fig_pac2.egg-info/
--rw-rw-rw-   0        0        0      132 2023-04-24 12:53:31.000000 kozh_fig_pac2-0.1/kozh_fig_pac2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-24 12:53:31.000000 kozh_fig_pac2-0.1/kozh_fig_pac2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:53:31.000000 kozh_fig_pac2-0.1/kozh_fig_pac2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 12:00:55.000000 kozh_fig_pac2-0.1/kozh_fig_pac2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-04-24 12:53:31.000000 kozh_fig_pac2-0.1/kozh_fig_pac2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 12:53:32.083334 kozh_fig_pac2-0.1/setup.cfg
--rw-rw-rw-   0        0        0      233 2023-04-24 12:43:49.000000 kozh_fig_pac2-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:58.774410 kozh_fig_pac2-0.2/
+-rw-rw-rw-   0        0        0      132 2023-04-24 12:53:58.775492 kozh_fig_pac2-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:58.739334 kozh_fig_pac2-0.2/kozh_fig_pac2/
+-rw-rw-rw-   0        0        0      315 2023-04-24 08:50:42.000000 kozh_fig_pac2-0.2/kozh_fig_pac2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:53:58.769136 kozh_fig_pac2-0.2/kozh_fig_pac2.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-04-24 12:53:58.000000 kozh_fig_pac2-0.2/kozh_fig_pac2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-24 12:53:58.000000 kozh_fig_pac2-0.2/kozh_fig_pac2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:53:58.000000 kozh_fig_pac2-0.2/kozh_fig_pac2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 12:00:55.000000 kozh_fig_pac2-0.2/kozh_fig_pac2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-24 12:53:58.000000 kozh_fig_pac2-0.2/kozh_fig_pac2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:53:58.777850 kozh_fig_pac2-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      233 2023-04-24 12:53:49.000000 kozh_fig_pac2-0.2/setup.py
```

