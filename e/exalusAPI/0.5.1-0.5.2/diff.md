# Comparing `tmp/exalusAPI-0.5.1.tar.gz` & `tmp/exalusAPI-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exalusAPI-0.5.1.tar", last modified: Mon Apr 24 06:42:42 2023, max compression
+gzip compressed data, was "exalusAPI-0.5.2.tar", last modified: Mon Apr 24 11:01:07 2023, max compression
```

## Comparing `exalusAPI-0.5.1.tar` & `exalusAPI-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:42:42.849476 exalusAPI-0.5.1/
--rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    13973 2023-04-24 06:42:42.847479 exalusAPI-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 06:42:42.839755 exalusAPI-0.5.1/exalusAPI.egg-info/
--rw-rw-rw-   0        0        0    13973 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1045 2023-04-24 06:41:30.000000 exalusAPI-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 06:42:42.849476 exalusAPI-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-04-24 06:39:37.000000 exalusAPI-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:42:42.843789 exalusAPI-0.5.1/src/
--rw-rw-rw-   0        0        0     6588 2023-04-24 06:27:01.000000 exalusAPI-0.5.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:01:07.476934 exalusAPI-0.5.2/
+-rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    13973 2023-04-24 11:01:07.475807 exalusAPI-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 11:01:07.464804 exalusAPI-0.5.2/exalusAPI.egg-info/
+-rw-rw-rw-   0        0        0    13973 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-24 11:01:07.000000 exalusAPI-0.5.2/exalusAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-24 11:00:58.000000 exalusAPI-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 11:01:07.477925 exalusAPI-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      639 2023-04-24 11:00:45.000000 exalusAPI-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:01:07.470810 exalusAPI-0.5.2/src/
+-rw-rw-rw-   0        0        0     6588 2023-04-24 06:27:01.000000 exalusAPI-0.5.2/src/__init__.py
```

### Comparing `exalusAPI-0.5.1/LICENSE` & `exalusAPI-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exalusAPI-0.5.1/PKG-INFO` & `exalusAPI-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
 Home-page: https://github.com/marceljanicki/ExalusAPI
 Author: Marcel Janicki
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exalusAPI-0.5.1/exalusAPI.egg-info/PKG-INFO` & `exalusAPI-0.5.2/exalusAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
 Home-page: https://github.com/marceljanicki/ExalusAPI
 Author: Marcel Janicki
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exalusAPI-0.5.1/pyproject.toml` & `exalusAPI-0.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "exalusAPI"
-version = "0.5.1"
+version = "0.5.2"
 description = "Simple Exalus integration wrapper, created specifically for HomeAssistant integration."
 readme = "README.md"
 authors = [{ name = "Marcel Janicki", email = "majanicki00@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["HomeAssistant", "Exalus"]
 requires-python = ">=3.10.6"
+dependencies = ["requests", "signalrcore"]
 [project.urls]
 Homepage = "https://github.com/marceljanicki/exalusAPI"
 [tool.bumpver]
 current_version = "2023.1001-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
```

### Comparing `exalusAPI-0.5.1/src/__init__.py` & `exalusAPI-0.5.2/src/__init__.py`

 * *Files identical despite different names*

