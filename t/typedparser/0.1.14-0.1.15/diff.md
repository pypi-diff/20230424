# Comparing `tmp/typedparser-0.1.14.tar.gz` & `tmp/typedparser-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedparser-0.1.14.tar", last modified: Mon Apr 24 09:16:04 2023, max compression
+gzip compressed data, was "typedparser-0.1.15.tar", last modified: Mon Apr 24 09:21:05 2023, max compression
```

## Comparing `typedparser-0.1.14.tar` & `typedparser-0.1.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:16:04.360462 typedparser-0.1.14/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.1.14/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     3524 2023-04-24 09:16:04.356461 typedparser-0.1.14/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     2710 2023-04-24 09:05:46.000000 typedparser-0.1.14/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.1.14/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-04-24 08:59:42.000000 typedparser-0.1.14/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-04-24 09:16:04.360462 typedparser-0.1.14/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:16:04.304460 typedparser-0.1.14/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:16:04.328461 typedparser-0.1.14/src/typedparser/
--rw-------   0 gings    (14999) lmb-mit   (1061)      246 2023-04-24 08:59:42.000000 typedparser-0.1.14/src/typedparser/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3521 2023-04-24 08:59:42.000000 typedparser-0.1.14/src/typedparser/_typedparser.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-04-24 08:59:42.000000 typedparser-0.1.14/src/typedparser/custom_format.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5406 2023-04-24 08:59:42.000000 typedparser-0.1.14/src/typedparser/funcs.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:16:04.352461 typedparser-0.1.14/src/typedparser.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     3524 2023-04-24 09:16:04.000000 typedparser-0.1.14/src/typedparser.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      395 2023-04-24 09:16:04.000000 typedparser-0.1.14/src/typedparser.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-04-24 09:16:04.000000 typedparser-0.1.14/src/typedparser.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-04-24 09:16:04.000000 typedparser-0.1.14/src/typedparser.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-04-24 09:16:04.000000 typedparser-0.1.14/src/typedparser.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-04-24 09:16:04.000000 typedparser-0.1.14/src/typedparser.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:21:05.482710 typedparser-0.1.15/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.1.15/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3578 2023-04-24 09:21:05.478709 typedparser-0.1.15/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2764 2023-04-24 09:20:50.000000 typedparser-0.1.15/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.1.15/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-04-24 09:20:50.000000 typedparser-0.1.15/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-04-24 09:21:05.482710 typedparser-0.1.15/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:21:05.430708 typedparser-0.1.15/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:21:05.454709 typedparser-0.1.15/src/typedparser/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      246 2023-04-24 09:20:50.000000 typedparser-0.1.15/src/typedparser/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3521 2023-04-24 09:20:50.000000 typedparser-0.1.15/src/typedparser/_typedparser.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-04-24 09:20:50.000000 typedparser-0.1.15/src/typedparser/custom_format.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5406 2023-04-24 09:20:50.000000 typedparser-0.1.15/src/typedparser/funcs.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-04-24 09:21:05.478709 typedparser-0.1.15/src/typedparser.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3578 2023-04-24 09:21:05.000000 typedparser-0.1.15/src/typedparser.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      395 2023-04-24 09:21:05.000000 typedparser-0.1.15/src/typedparser.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-04-24 09:21:05.000000 typedparser-0.1.15/src/typedparser.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-04-24 09:21:05.000000 typedparser-0.1.15/src/typedparser.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-04-24 09:21:05.000000 typedparser-0.1.15/src/typedparser.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-04-24 09:16:04.000000 typedparser-0.1.15/src/typedparser.egg-info/zip-safe
```

### Comparing `typedparser-0.1.14/LICENSE` & `typedparser-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.14/PKG-INFO` & `typedparser-0.1.15/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.1.14
+Version: 0.1.15
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -20,20 +20,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # typedparser
 
 <p align="center">
 <a href="https://github.com/gingsi/typedparser/actions/workflows/build_py37.yml">
-  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedparser/build_py37.yml?branch=main&label=build%203.7" />
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py37.yml?branch=main&label=build%203.7" />
 </a>
 <a href="https://github.com/gingsi/typedparser/actions/workflows/build_py39.yml">
-  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedparser/build_py39.yml?branch=main&label=build%203.9" />
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py39.yml?branch=main&label=build%203.9" />
 </a>
-<img alt="coverage" title="coverage" src="docs/coverage.svg" />
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/typedparser/main/docs/coverage.svg" />
 <a href="https://pypi.org/project/typedparser/">
   <img alt="version" title="version" src="https://img.shields.io/pypi/v/typedparser?color=success" />
 </a>
 </p>
 
 Typing extension for python argparse using [attrs](https://www.attrs.org/en/stable/) and
 [typedattr](https://github.com/gingsi/typedattr).
```

### Comparing `typedparser-0.1.14/README.md` & `typedparser-0.1.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # typedparser
 
 <p align="center">
 <a href="https://github.com/gingsi/typedparser/actions/workflows/build_py37.yml">
-  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedparser/build_py37.yml?branch=main&label=build%203.7" />
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py37.yml?branch=main&label=build%203.7" />
 </a>
 <a href="https://github.com/gingsi/typedparser/actions/workflows/build_py39.yml">
-  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedparser/build_py39.yml?branch=main&label=build%203.9" />
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py39.yml?branch=main&label=build%203.9" />
 </a>
-<img alt="coverage" title="coverage" src="docs/coverage.svg" />
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/typedparser/main/docs/coverage.svg" />
 <a href="https://pypi.org/project/typedparser/">
   <img alt="version" title="version" src="https://img.shields.io/pypi/v/typedparser?color=success" />
 </a>
 </p>
 
 Typing extension for python argparse using [attrs](https://www.attrs.org/en/stable/) and
 [typedattr](https://github.com/gingsi/typedattr).
```

### Comparing `typedparser-0.1.14/pyproject.toml` & `typedparser-0.1.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.14/src/typedparser/_typedparser.py` & `typedparser-0.1.15/src/typedparser/_typedparser.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.14/src/typedparser/custom_format.py` & `typedparser-0.1.15/src/typedparser/custom_format.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.14/src/typedparser/funcs.py` & `typedparser-0.1.15/src/typedparser/funcs.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.14/src/typedparser.egg-info/PKG-INFO` & `typedparser-0.1.15/src/typedparser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.1.14
+Version: 0.1.15
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -20,20 +20,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # typedparser
 
 <p align="center">
 <a href="https://github.com/gingsi/typedparser/actions/workflows/build_py37.yml">
-  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedparser/build_py37.yml?branch=main&label=build%203.7" />
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py37.yml?branch=main&label=build%203.7" />
 </a>
 <a href="https://github.com/gingsi/typedparser/actions/workflows/build_py39.yml">
-  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedparser/build_py39.yml?branch=main&label=build%203.9" />
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py39.yml?branch=main&label=build%203.9" />
 </a>
-<img alt="coverage" title="coverage" src="docs/coverage.svg" />
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/typedparser/main/docs/coverage.svg" />
 <a href="https://pypi.org/project/typedparser/">
   <img alt="version" title="version" src="https://img.shields.io/pypi/v/typedparser?color=success" />
 </a>
 </p>
 
 Typing extension for python argparse using [attrs](https://www.attrs.org/en/stable/) and
 [typedattr](https://github.com/gingsi/typedattr).
```

