# Comparing `tmp/kozh_fig_pac3-0.3.tar.gz` & `tmp/kozh_fig_pac3-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kozh_fig_pac3-0.3.tar", last modified: Mon Apr 24 13:27:07 2023, max compression
+gzip compressed data, was "kozh_fig_pac3-0.4.tar", last modified: Mon Apr 24 13:31:05 2023, max compression
```

## Comparing `kozh_fig_pac3-0.3.tar` & `kozh_fig_pac3-0.4.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:07.193908 kozh_fig_pac3-0.3/
--rw-rw-rw-   0        0        0      133 2023-04-24 13:27:07.194894 kozh_fig_pac3-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:07.156541 kozh_fig_pac3-0.3/kozh_fig_pac3/
--rw-rw-rw-   0        0        0      315 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.3/kozh_fig_pac3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:07.189894 kozh_fig_pac3-0.3/kozh_fig_pac3.egg-info/
--rw-rw-rw-   0        0        0      133 2023-04-24 13:27:06.000000 kozh_fig_pac3-0.3/kozh_fig_pac3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-24 13:27:07.000000 kozh_fig_pac3-0.3/kozh_fig_pac3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:27:06.000000 kozh_fig_pac3-0.3/kozh_fig_pac3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 13:27:06.000000 kozh_fig_pac3-0.3/kozh_fig_pac3.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-04-24 13:27:06.000000 kozh_fig_pac3-0.3/kozh_fig_pac3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:27:07.197905 kozh_fig_pac3-0.3/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-04-24 13:23:39.000000 kozh_fig_pac3-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:05.611960 kozh_fig_pac3-0.4/
+-rw-rw-rw-   0        0        0      133 2023-04-24 13:31:05.612962 kozh_fig_pac3-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:05.513634 kozh_fig_pac3-0.4/kozh_fig_pac3/
+-rw-rw-rw-   0        0        0      315 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:05.578850 kozh_fig_pac3-0.4/kozh_fig_pac3/circle/
+-rw-rw-rw-   0        0        0       49 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/circle/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/circle/code.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:05.592897 kozh_fig_pac3-0.4/kozh_fig_pac3/square/
+-rw-rw-rw-   0        0        0       51 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/square/__init__.py
+-rw-rw-rw-   0        0        0      124 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/square/code.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:05.606943 kozh_fig_pac3-0.4/kozh_fig_pac3/triangle/
+-rw-rw-rw-   0        0        0       53 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/triangle/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-04-24 08:50:42.000000 kozh_fig_pac3-0.4/kozh_fig_pac3/triangle/code.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:05.558783 kozh_fig_pac3-0.4/kozh_fig_pac3.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-04-24 13:31:05.000000 kozh_fig_pac3-0.4/kozh_fig_pac3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2023-04-24 13:31:05.000000 kozh_fig_pac3-0.4/kozh_fig_pac3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:31:05.000000 kozh_fig_pac3-0.4/kozh_fig_pac3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 13:27:06.000000 kozh_fig_pac3-0.4/kozh_fig_pac3.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-24 13:31:05.000000 kozh_fig_pac3-0.4/kozh_fig_pac3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:31:05.614970 kozh_fig_pac3-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-04-24 13:30:57.000000 kozh_fig_pac3-0.4/setup.py
```

