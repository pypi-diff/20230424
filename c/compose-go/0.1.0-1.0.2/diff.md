# Comparing `tmp/compose-go-0.1.0.tar.gz` & `tmp/compose-go-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-go-0.1.0.tar", last modified: Mon Apr 24 05:03:01 2023, max compression
+gzip compressed data, was "compose-go-1.0.2.tar", last modified: Mon Apr 24 07:59:26 2023, max compression
```

## Comparing `compose-go-0.1.0.tar` & `compose-go-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 05:03:01.654188 compose-go-0.1.0/
--rw-rw-r--   0 luabida   (1000) luabida   (1000)     1514 2023-04-19 20:20:05.000000 compose-go-0.1.0/LICENSE
--rw-rw-r--   0 luabida   (1000) luabida   (1000)      211 2023-04-24 05:03:01.654188 compose-go-0.1.0/PKG-INFO
-drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 05:03:01.654188 compose-go-0.1.0/compose_go.egg-info/
--rw-rw-r--   0 luabida   (1000) luabida   (1000)      211 2023-04-24 05:03:01.000000 compose-go-0.1.0/compose_go.egg-info/PKG-INFO
--rw-rw-r--   0 luabida   (1000) luabida   (1000)      262 2023-04-24 05:03:01.000000 compose-go-0.1.0/compose_go.egg-info/SOURCES.txt
--rw-rw-r--   0 luabida   (1000) luabida   (1000)        1 2023-04-24 05:03:01.000000 compose-go-0.1.0/compose_go.egg-info/dependency_links.txt
--rw-rw-r--   0 luabida   (1000) luabida   (1000)       62 2023-04-24 05:03:01.000000 compose-go-0.1.0/compose_go.egg-info/entry_points.txt
--rw-rw-r--   0 luabida   (1000) luabida   (1000)        6 2023-04-24 05:03:01.000000 compose-go-0.1.0/compose_go.egg-info/requires.txt
--rw-rw-r--   0 luabida   (1000) luabida   (1000)        4 2023-04-24 05:03:01.000000 compose-go-0.1.0/compose_go.egg-info/top_level.txt
--rw-rw-r--   0 luabida   (1000) luabida   (1000)       38 2023-04-24 05:03:01.654188 compose-go-0.1.0/setup.cfg
--rw-rw-r--   0 luabida   (1000) luabida   (1000)      516 2023-04-20 20:39:18.000000 compose-go-0.1.0/setup.py
-drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 05:03:01.654188 compose-go-0.1.0/src/
--rw-rw-r--   0 luabida   (1000) luabida   (1000)      326 2023-04-20 20:38:07.000000 compose-go-0.1.0/src/__init__.py
-drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 05:03:01.654188 compose-go-0.1.0/src/compose/
--rw-rw-r--   0 luabida   (1000) luabida   (1000)      448 2023-04-20 20:37:44.000000 compose-go-0.1.0/src/compose/__init__.py
+drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 07:59:26.804950 compose-go-1.0.2/
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)     1514 2023-04-19 20:20:05.000000 compose-go-1.0.2/LICENSE
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)      211 2023-04-24 07:59:26.804950 compose-go-1.0.2/PKG-INFO
+drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 07:59:26.800950 compose-go-1.0.2/compose_go.egg-info/
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)      211 2023-04-24 07:59:26.000000 compose-go-1.0.2/compose_go.egg-info/PKG-INFO
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)      262 2023-04-24 07:59:26.000000 compose-go-1.0.2/compose_go.egg-info/SOURCES.txt
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)        1 2023-04-24 07:59:26.000000 compose-go-1.0.2/compose_go.egg-info/dependency_links.txt
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)       62 2023-04-24 07:59:26.000000 compose-go-1.0.2/compose_go.egg-info/entry_points.txt
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)        6 2023-04-24 07:59:26.000000 compose-go-1.0.2/compose_go.egg-info/requires.txt
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)        4 2023-04-24 07:59:26.000000 compose-go-1.0.2/compose_go.egg-info/top_level.txt
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)       38 2023-04-24 07:59:26.804950 compose-go-1.0.2/setup.cfg
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)      516 2023-04-24 07:56:27.000000 compose-go-1.0.2/setup.py
+drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 07:59:26.804950 compose-go-1.0.2/src/
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)      326 2023-04-24 07:56:27.000000 compose-go-1.0.2/src/__init__.py
+drwxrwxr-x   0 luabida   (1000) luabida   (1000)        0 2023-04-24 07:59:26.804950 compose-go-1.0.2/src/compose/
+-rw-rw-r--   0 luabida   (1000) luabida   (1000)      438 2023-04-24 05:14:18.000000 compose-go-1.0.2/src/compose/__init__.py
```

### Comparing `compose-go-0.1.0/LICENSE` & `compose-go-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-go-0.1.0/setup.py` & `compose-go-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="compose-go",
-    version="0.1.0", # changed by semantic-release
+    version="1.0.2", # changed by semantic-release
     author="Luã Bida Vacaro",
     author_email="luabidaa@gmail.com",
     description="Docker Compose v2 (GoLang) wrapped in a Python Package",
     packages=find_packages(include=["src", "src.*"]),
     license='BSD',
     install_requires=[
         'click',
```

