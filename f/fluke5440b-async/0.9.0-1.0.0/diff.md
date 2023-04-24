# Comparing `tmp/fluke5440b_async-0.9.0.tar.gz` & `tmp/fluke5440b_async-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluke5440b_async-0.9.0.tar", last modified: Sun Apr 23 03:41:55 2023, max compression
+gzip compressed data, was "fluke5440b_async-1.0.0.tar", last modified: Mon Apr 24 13:03:49 2023, max compression
```

## Comparing `fluke5440b_async-0.9.0.tar` & `fluke5440b_async-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maat      (1000) maat      (1000)        0 2023-04-23 03:41:55.352148 fluke5440b_async-0.9.0/
--rw-r--r--   0 maat      (1000) maat      (1000)    35147 2020-10-29 12:04:51.000000 fluke5440b_async-0.9.0/LICENSE
--rw-r--r--   0 maat      (1000) maat      (1000)    19548 2023-04-23 03:41:55.352148 fluke5440b_async-0.9.0/PKG-INFO
--rw-r--r--   0 maat      (1000) maat      (1000)    18208 2023-04-22 23:24:14.000000 fluke5440b_async-0.9.0/README.md
-drwxr-xr-x   0 maat      (1000) maat      (1000)        0 2023-04-23 03:41:55.352148 fluke5440b_async-0.9.0/fluke5440b_async/
--rw-r-----   0 maat      (1000) maat      (1000)      397 2023-04-22 23:24:15.000000 fluke5440b_async-0.9.0/fluke5440b_async/__init__.py
--rw-r--r--   0 maat      (1000) maat      (1000)       65 2023-04-22 22:55:48.000000 fluke5440b_async-0.9.0/fluke5440b_async/_version.py
--rw-r--r--   0 maat      (1000) maat      (1000)     2032 2023-04-23 01:17:12.000000 fluke5440b_async-0.9.0/fluke5440b_async/enums.py
--rw-r--r--   0 maat      (1000) maat      (1000)      488 2023-04-23 03:07:05.000000 fluke5440b_async-0.9.0/fluke5440b_async/errors.py
--rw-r--r--   0 maat      (1000) maat      (1000)      728 2023-04-22 22:59:53.000000 fluke5440b_async-0.9.0/fluke5440b_async/flags.py
--rw-rw-r--   0 maat      (1000) maat      (1000)    26613 2023-04-23 03:40:11.000000 fluke5440b_async-0.9.0/fluke5440b_async/fluke_5440b.py
-drwxr-xr-x   0 maat      (1000) maat      (1000)        0 2023-04-23 03:41:55.352148 fluke5440b_async-0.9.0/fluke5440b_async.egg-info/
--rw-r--r--   0 maat      (1000) maat      (1000)    19548 2023-04-23 03:41:55.000000 fluke5440b_async-0.9.0/fluke5440b_async.egg-info/PKG-INFO
--rw-r--r--   0 maat      (1000) maat      (1000)      409 2023-04-23 03:41:55.000000 fluke5440b_async-0.9.0/fluke5440b_async.egg-info/SOURCES.txt
--rw-r--r--   0 maat      (1000) maat      (1000)        1 2023-04-23 03:41:55.000000 fluke5440b_async-0.9.0/fluke5440b_async.egg-info/dependency_links.txt
--rw-r--r--   0 maat      (1000) maat      (1000)      237 2023-04-23 03:41:55.000000 fluke5440b_async-0.9.0/fluke5440b_async.egg-info/requires.txt
--rw-r--r--   0 maat      (1000) maat      (1000)       17 2023-04-23 03:41:55.000000 fluke5440b_async-0.9.0/fluke5440b_async.egg-info/top_level.txt
--rw-r--r--   0 maat      (1000) maat      (1000)     1914 2023-04-23 03:35:40.000000 fluke5440b_async-0.9.0/pyproject.toml
--rw-r--r--   0 maat      (1000) maat      (1000)       38 2023-04-23 03:41:55.352148 fluke5440b_async-0.9.0/setup.cfg
--rw-r--r--   0 maat      (1000) maat      (1000)      134 2022-07-10 04:26:05.000000 fluke5440b_async-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:03:49.419991 fluke5440b_async-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 13:03:49.419991 fluke5440b_async-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:03:49.415991 fluke5440b_async-1.0.0/fluke5440b_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/fluke5440b_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/fluke5440b_async/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/fluke5440b_async/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/fluke5440b_async/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/fluke5440b_async/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/fluke5440b_async/fluke_5440b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:03:49.419991 fluke5440b_async-1.0.0/fluke5440b_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 13:03:49.000000 fluke5440b_async-1.0.0/fluke5440b_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 13:03:49.000000 fluke5440b_async-1.0.0/fluke5440b_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:03:49.000000 fluke5440b_async-1.0.0/fluke5440b_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 13:03:49.000000 fluke5440b_async-1.0.0/fluke5440b_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 13:03:49.000000 fluke5440b_async-1.0.0/fluke5440b_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:03:49.419991 fluke5440b_async-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:03:18.000000 fluke5440b_async-1.0.0/setup.py
```

### Comparing `fluke5440b_async-0.9.0/LICENSE` & `fluke5440b_async-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluke5440b_async-0.9.0/pyproject.toml` & `fluke5440b_async-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -39,20 +39,25 @@
 prologix-gpib = ["prologix-gpib-async"]
 
 dev = [
     "async-gpib", "black", "build", "gpib-ctypes", "isort", "mypy", "pre-commit", "prologix-gpib-async", "pylint",
     "twine",
 ]
 
+doc = [
+    "myst-parser", "sphinx",
+]
+
 test = [
     "mypy", "pylint",
 ]
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 120
+notes = ["FIXME", "XXX",]
 
 [tool.isort]
 line_length = 120
 profile = "black"
 
 [tool.black]
 line-length = 120
```

