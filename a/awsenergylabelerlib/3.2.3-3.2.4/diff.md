# Comparing `tmp/awsenergylabelerlib-3.2.3.tar.gz` & `tmp/awsenergylabelerlib-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsenergylabelerlib-3.2.3.tar", last modified: Thu Apr 13 14:51:20 2023, max compression
+gzip compressed data, was "awsenergylabelerlib-3.2.4.tar", last modified: Mon Apr 24 12:08:26 2023, max compression
```

## Comparing `awsenergylabelerlib-3.2.3.tar` & `awsenergylabelerlib-3.2.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/USAGE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.985839 awsenergylabelerlib-3.2.3/awsenergylabelerlib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7719 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlibexceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7304 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7446 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/datamodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/dev-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    40747 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2419 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/schemas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8929 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.985839 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 14:51:20.000000 awsenergylabelerlib-3.2.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:20.989838 awsenergylabelerlib-3.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/tests/test_awsenergylabelerlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-13 14:49:50.000000 awsenergylabelerlib-3.2.3/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3780 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/USAGE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/awsenergylabelerlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3780 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    71531 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7719 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/awsenergylabelerlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/awsenergylabelerlibexceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7304 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7446 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/datamodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/dev-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40579 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2419 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8929 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6814 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9048 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-24 12:08:26.000000 awsenergylabelerlib-3.2.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:08:26.461531 awsenergylabelerlib-3.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/tests/test_awsenergylabelerlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-24 12:07:00.000000 awsenergylabelerlib-3.2.4/tests/test_validations.py
```

### Comparing `awsenergylabelerlib-3.2.3/CONTRIBUTING.rst` & `awsenergylabelerlib-3.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/HISTORY.rst` & `awsenergylabelerlib-3.2.4/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -200,7 +200,13 @@
 * Convert Dataclasses to Frozen for compatibility with latest python.
 
 
 3.2.3 (13-04-2023)
 ------------------
 
 * Changed from dataclass to normal.
+
+
+3.2.4 (24-04-2023)
+------------------
+
+* Writing to S3 now does not attempt to write to a temporary file first, accomodating read-only filesystems when only writing to S3.
```

### Comparing `awsenergylabelerlib-3.2.3/LICENSE` & `awsenergylabelerlib-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/PKG-INFO` & `awsenergylabelerlib-3.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelerlib
-Version: 3.2.3
+Version: 3.2.4
 Summary: Project energy labeling accounts and landing zone based on findings of Security Hub in AWS cloud.
 Home-page: https://github.com/schubergphilis/awsenergylabelerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelerlib energy labeling aws security hub landing zone
 Classifier: Development Status :: 4 - Beta
@@ -287,7 +287,13 @@
 * Convert Dataclasses to Frozen for compatibility with latest python.
 
 
 3.2.3 (13-04-2023)
 ------------------
 
 * Changed from dataclass to normal.
+
+
+3.2.4 (24-04-2023)
+------------------
+
+* Writing to S3 now does not attempt to write to a temporary file first, accomodating read-only filesystems when only writing to S3.
```

### Comparing `awsenergylabelerlib-3.2.3/Pipfile` & `awsenergylabelerlib-3.2.4/Pipfile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/Pipfile.lock` & `awsenergylabelerlib-3.2.4/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926103136629453%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:1ff703152553f4d5fc9774071d114dbf06ec661eb1b29b6051f6b1f9d0c24873', "*

 * *              "'sha256:d0ed43228952b55c9f44d1c733f74656418c39c55dbe36bc37feeef6aa583ded'], "*

 * *              "'version': '==1.26.118'}, 'botocore': {'hashes': "*

 * *              "['sha256:44cb088a73b02dd716c5c5715143a64d5f10388957285246e11f3cc893eebf9d', "*

 * *              "'sha256:b51fc5d50cbc43edaf58b3ec4fa933b82755801c453bf8908c8d3e70ae1142c1'], "*

 * *              "'version': '==1.29.11 […]*

```diff
@@ -12,27 +12,27 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "boto3": {
             "hashes": [
-                "sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f",
-                "sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69"
+                "sha256:1ff703152553f4d5fc9774071d114dbf06ec661eb1b29b6051f6b1f9d0c24873",
+                "sha256:d0ed43228952b55c9f44d1c733f74656418c39c55dbe36bc37feeef6aa583ded"
             ],
             "index": "pypi",
-            "version": "==1.26.112"
+            "version": "==1.26.118"
         },
         "botocore": {
             "hashes": [
-                "sha256:1f52d9371d7b5ee30a53dcef7954c3cf22e04b131cfab5268035f3299ccde9e1",
-                "sha256:2cbaddb09b46dcb0a05490724d51acb224d3a8df433c347f995b4d78bfb02c8a"
+                "sha256:44cb088a73b02dd716c5c5715143a64d5f10388957285246e11f3cc893eebf9d",
+                "sha256:b51fc5d50cbc43edaf58b3ec4fa933b82755801c453bf8908c8d3e70ae1142c1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.112"
+            "version": "==1.29.118"
         },
         "cachetools": {
             "hashes": [
                 "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "index": "pypi",
@@ -110,19 +110,19 @@
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd",
-                "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"
+                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
+                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.2"
+            "version": "==2.15.4"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -397,36 +397,36 @@
                 "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "index": "pypi",
             "version": "==7.2.3"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
-                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
-                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
-                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
-                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
-                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
-                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
-                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
-                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
-                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
-                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
-                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
-                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
-                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
-                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
-                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
-                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
-                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
-                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==40.0.1"
+            "version": "==40.0.2"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -459,19 +459,19 @@
                 "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
             ],
             "index": "pypi",
             "version": "==2.2.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37",
-                "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.12.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -530,19 +530,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402",
-                "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.3.0"
+            "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -811,19 +811,19 @@
                 "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
-                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.15.0"
+            "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
                 "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
                 "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
             ],
             "markers": "python_full_version >= '3.7.2'",
@@ -1010,19 +1010,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
+                "sha256:9ef22c2941bc3d0ff080d25a797f7521fc317e857395c712ddde97a19d5bb440",
+                "sha256:ff1c2a1167bef9cdcd8ec71339e85fe10f26d4e9ef9382ef10b2687c876c936b"
             ],
             "index": "pypi",
-            "version": "==6.1.3"
+            "version": "==6.2.0"
         },
         "sphinx-rtd-theme": {
             "hashes": [
                 "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
                 "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
             ],
             "index": "pypi",
@@ -1106,19 +1106,19 @@
                 "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.7"
         },
         "tox": {
             "hashes": [
-                "sha256:6fa4dbd933d0e335b5392c81e9cd467630119b3669705dbad47814a93b6c9586",
-                "sha256:cd88e41aef9c71f0ba02b6d7939f102760b192b63458fbe04dbbaed82f7bf5f5"
+                "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e",
+                "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"
             ],
             "index": "pypi",
-            "version": "==4.4.11"
+            "version": "==4.4.12"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
@@ -1138,19 +1138,19 @@
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.15"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3",
+                "sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "version": "==20.22.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `awsenergylabelerlib-3.2.3/README.rst` & `awsenergylabelerlib-3.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/USAGE.rst` & `awsenergylabelerlib-3.2.4/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/CONTRIBUTING.rst` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/HISTORY.rst` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -200,7 +200,13 @@
 * Convert Dataclasses to Frozen for compatibility with latest python.
 
 
 3.2.3 (13-04-2023)
 ------------------
 
 * Changed from dataclass to normal.
+
+
+3.2.4 (24-04-2023)
+------------------
+
+* Writing to S3 now does not attempt to write to a temporary file first, accomodating read-only filesystems when only writing to S3.
```

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/LICENSE` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/LICENSE`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/Pipfile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/Pipfile.lock` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926103136629453%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:1ff703152553f4d5fc9774071d114dbf06ec661eb1b29b6051f6b1f9d0c24873', "*

 * *              "'sha256:d0ed43228952b55c9f44d1c733f74656418c39c55dbe36bc37feeef6aa583ded'], "*

 * *              "'version': '==1.26.118'}, 'botocore': {'hashes': "*

 * *              "['sha256:44cb088a73b02dd716c5c5715143a64d5f10388957285246e11f3cc893eebf9d', "*

 * *              "'sha256:b51fc5d50cbc43edaf58b3ec4fa933b82755801c453bf8908c8d3e70ae1142c1'], "*

 * *              "'version': '==1.29.11 […]*

```diff
@@ -12,27 +12,27 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "boto3": {
             "hashes": [
-                "sha256:03c2e1ddd29d993a6ab9b8a8fe184027957fc32bd405c496ad0c30311445925f",
-                "sha256:4ea3319bba2e8ff7cd9560259ae64f073c7fb6312158aa375777687231cabe69"
+                "sha256:1ff703152553f4d5fc9774071d114dbf06ec661eb1b29b6051f6b1f9d0c24873",
+                "sha256:d0ed43228952b55c9f44d1c733f74656418c39c55dbe36bc37feeef6aa583ded"
             ],
             "index": "pypi",
-            "version": "==1.26.112"
+            "version": "==1.26.118"
         },
         "botocore": {
             "hashes": [
-                "sha256:1f52d9371d7b5ee30a53dcef7954c3cf22e04b131cfab5268035f3299ccde9e1",
-                "sha256:2cbaddb09b46dcb0a05490724d51acb224d3a8df433c347f995b4d78bfb02c8a"
+                "sha256:44cb088a73b02dd716c5c5715143a64d5f10388957285246e11f3cc893eebf9d",
+                "sha256:b51fc5d50cbc43edaf58b3ec4fa933b82755801c453bf8908c8d3e70ae1142c1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.112"
+            "version": "==1.29.118"
         },
         "cachetools": {
             "hashes": [
                 "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "index": "pypi",
@@ -110,19 +110,19 @@
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd",
-                "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"
+                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
+                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.2"
+            "version": "==2.15.4"
         },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
@@ -397,36 +397,36 @@
                 "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "index": "pypi",
             "version": "==7.2.3"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
-                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
-                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
-                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
-                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
-                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
-                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
-                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
-                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
-                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
-                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
-                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
-                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
-                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
-                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
-                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
-                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
-                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
-                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==40.0.1"
+            "version": "==40.0.2"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
@@ -459,19 +459,19 @@
                 "sha256:a2986c21e4aba6b9870df40ef487a17be863cb7778dcf1c01e25917b7cd210bb"
             ],
             "index": "pypi",
             "version": "==2.2.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37",
-                "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.12.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
                 "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -530,19 +530,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402",
-                "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version < '3.10'",
-            "version": "==6.3.0"
+            "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
                 "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "markers": "python_full_version >= '3.8.0'",
@@ -811,19 +811,19 @@
                 "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
-                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.15.0"
+            "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
                 "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8",
                 "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"
             ],
             "markers": "python_full_version >= '3.7.2'",
@@ -1010,19 +1010,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
+                "sha256:9ef22c2941bc3d0ff080d25a797f7521fc317e857395c712ddde97a19d5bb440",
+                "sha256:ff1c2a1167bef9cdcd8ec71339e85fe10f26d4e9ef9382ef10b2687c876c936b"
             ],
             "index": "pypi",
-            "version": "==6.1.3"
+            "version": "==6.2.0"
         },
         "sphinx-rtd-theme": {
             "hashes": [
                 "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
                 "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
             ],
             "index": "pypi",
@@ -1106,19 +1106,19 @@
                 "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.7"
         },
         "tox": {
             "hashes": [
-                "sha256:6fa4dbd933d0e335b5392c81e9cd467630119b3669705dbad47814a93b6c9586",
-                "sha256:cd88e41aef9c71f0ba02b6d7939f102760b192b63458fbe04dbbaed82f7bf5f5"
+                "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e",
+                "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"
             ],
             "index": "pypi",
-            "version": "==4.4.11"
+            "version": "==4.4.12"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
@@ -1138,19 +1138,19 @@
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.15"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3",
+                "sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "version": "==20.22.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/README.rst` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/README.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/USAGE.rst` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/__init__.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/__init__.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/_version.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/_version.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlib.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/awsenergylabelerlib.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/awsenergylabelerlibexceptions.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/awsenergylabelerlibexceptions.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/configuration.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/configuration.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/datamodels.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/datamodels.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/dev-requirements.txt` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/dev-requirements.txt`

 * *Files 25% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # by pipenv through Pipfile and Pipfile.lock .
 #
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
-sphinx>=6.1.3
+sphinx>=6.2.0
 sphinx-rtd-theme>=1.2.0
 prospector>=1.9.0
 coverage>=7.2.3
 nose>=1.3.7
 nose-htmloutput>=0.6.0
-tox>=4.4.11
+tox>=4.4.12
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=2.13.0
 gitwrapperlib>=1.0.0
 twine>=4.0.2
 coloredlogs>=15.0.1
 emoji>=2.2.0
```

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/entities.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 Import all parts from entities here
 
 .. _Google Python Style Guide:
    http://google.github.io/styleguide/pyguide.html
 """
 
 import logging
-import tempfile
 from abc import ABC, abstractmethod
 from collections import Counter
 from copy import copy, deepcopy
 from datetime import datetime
 from pathlib import Path
 from urllib.parse import urlparse, urljoin
 
@@ -970,20 +969,18 @@
 
     def _export_to_s3(self, s3_url, filename, data):
         """Exports as json to S3 object storage."""
         s3 = boto3.client('s3')  # pylint: disable=invalid-name
         parsed_url = urlparse(s3_url)
         bucket_name = parsed_url.netloc
         dst_path = parsed_url.path
-        with tempfile.NamedTemporaryFile() as temp_file:
-            temp_file.write(data.encode('utf-8'))
-            temp_file.flush()
-            dst_filename = urljoin(dst_path, filename).lstrip("/")
-            s3.upload_file(temp_file.name, bucket_name, dst_filename)
-            temp_file.close()
+
+        dst_filename = urljoin(dst_path, filename).lstrip("/")
+        s3.put_object(Body=data.encode('utf-8'), Bucket=bucket_name, Key=dst_filename)
+
         self._logger.info(f'File {filename} copied to {s3_url}')
 
 
 class DataFileFactory:
     """Data export factory to handle the different data types returned."""
 
     #  pylint: disable=too-many-arguments, unused-argument
```

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/labels.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/labels.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/schemas.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/schemas.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib/validations.py` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib/validations.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/PKG-INFO` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsenergylabelerlib
-Version: 3.2.3
+Version: 3.2.4
 Summary: Project energy labeling accounts and landing zone based on findings of Security Hub in AWS cloud.
 Home-page: https://github.com/schubergphilis/awsenergylabelerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Keywords: awsenergylabelerlib energy labeling aws security hub landing zone
 Classifier: Development Status :: 4 - Beta
@@ -287,7 +287,13 @@
 * Convert Dataclasses to Frozen for compatibility with latest python.
 
 
 3.2.3 (13-04-2023)
 ------------------
 
 * Changed from dataclass to normal.
+
+
+3.2.4 (24-04-2023)
+------------------
+
+* Writing to S3 now does not attempt to write to a temporary file first, accomodating read-only filesystems when only writing to S3.
```

### Comparing `awsenergylabelerlib-3.2.3/awsenergylabelerlib.egg-info/SOURCES.txt` & `awsenergylabelerlib-3.2.4/awsenergylabelerlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/dev-requirements.txt` & `awsenergylabelerlib-3.2.4/dev-requirements.txt`

 * *Files 25% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # by pipenv through Pipfile and Pipfile.lock .
 #
 # This file is created and managed automatically by the template and it is left
 # here only for backwards compatibility reasons with python's ecosystem.
 #
 # Please use Pipfile to update the requirements.
 #
-sphinx>=6.1.3
+sphinx>=6.2.0
 sphinx-rtd-theme>=1.2.0
 prospector>=1.9.0
 coverage>=7.2.3
 nose>=1.3.7
 nose-htmloutput>=0.6.0
-tox>=4.4.11
+tox>=4.4.12
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=2.13.0
 gitwrapperlib>=1.0.0
 twine>=4.0.2
 coloredlogs>=15.0.1
 emoji>=2.2.0
```

### Comparing `awsenergylabelerlib-3.2.3/docs/Makefile` & `awsenergylabelerlib-3.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/docs/conf.py` & `awsenergylabelerlib-3.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/docs/index.rst` & `awsenergylabelerlib-3.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/setup.py` & `awsenergylabelerlib-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/tests/test_awsenergylabelerlib.py` & `awsenergylabelerlib-3.2.4/tests/test_awsenergylabelerlib.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/tests/test_entities.py` & `awsenergylabelerlib-3.2.4/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `awsenergylabelerlib-3.2.3/tests/test_validations.py` & `awsenergylabelerlib-3.2.4/tests/test_validations.py`

 * *Files identical despite different names*

