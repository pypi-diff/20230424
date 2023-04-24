# Comparing `tmp/cullinan-0.51.tar.gz` & `tmp/cullinan-0.52a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cullinan-0.51.tar", last modified: Sun Apr 16 12:37:04 2023, max compression
+gzip compressed data, was "cullinan-0.52a1.tar", last modified: Mon Apr 24 09:31:36 2023, max compression
```

## Comparing `cullinan-0.51.tar` & `cullinan-0.52a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hansion    (501) staff       (20)        0 2023-04-16 12:37:04.928964 cullinan-0.51/
--rw-r--r--   0 hansion    (501) staff       (20)    11357 2023-04-11 05:12:10.000000 cullinan-0.51/LICENSE
--rw-r--r--   0 hansion    (501) staff       (20)     3244 2023-04-16 12:37:04.928517 cullinan-0.51/PKG-INFO
-drwxr-xr-x   0 hansion    (501) staff       (20)        0 2023-04-16 12:37:04.925787 cullinan-0.51/cullinan/
--rw-r--r--   0 hansion    (501) staff       (20)     5589 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/application.py
--rw-r--r--   0 hansion    (501) staff       (20)    23605 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/controller.py
--rw-r--r--   0 hansion    (501) staff       (20)      881 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/dao.py
--rw-r--r--   0 hansion    (501) staff       (20)     4564 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/request.py
--rw-r--r--   0 hansion    (501) staff       (20)     2111 2023-04-11 05:12:10.000000 cullinan-0.51/cullinan/service.py
-drwxr-xr-x   0 hansion    (501) staff       (20)        0 2023-04-16 12:37:04.927576 cullinan-0.51/cullinan.egg-info/
--rw-r--r--   0 hansion    (501) staff       (20)     3244 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/PKG-INFO
--rw-r--r--   0 hansion    (501) staff       (20)      278 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/SOURCES.txt
--rw-r--r--   0 hansion    (501) staff       (20)        1 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/dependency_links.txt
--rw-r--r--   0 hansion    (501) staff       (20)       41 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/requires.txt
--rw-r--r--   0 hansion    (501) staff       (20)        9 2023-04-16 12:37:04.000000 cullinan-0.51/cullinan.egg-info/top_level.txt
--rw-r--r--   0 hansion    (501) staff       (20)       38 2023-04-16 12:37:04.929187 cullinan-0.51/setup.cfg
--rw-r--r--   0 hansion    (501) staff       (20)     1282 2023-04-16 12:36:58.000000 cullinan-0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:31:36.352076 cullinan-0.52a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-04-24 09:31:23.000000 cullinan-0.52a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-24 09:31:36.352076 cullinan-0.52a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:31:36.352076 cullinan-0.52a1/cullinan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-24 09:31:23.000000 cullinan-0.52a1/cullinan/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-04-24 09:31:23.000000 cullinan-0.52a1/cullinan/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-24 09:31:23.000000 cullinan-0.52a1/cullinan/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-24 09:31:23.000000 cullinan-0.52a1/cullinan/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-24 09:31:23.000000 cullinan-0.52a1/cullinan/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:31:36.352076 cullinan-0.52a1/cullinan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-24 09:31:36.000000 cullinan-0.52a1/cullinan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-24 09:31:36.000000 cullinan-0.52a1/cullinan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:31:36.000000 cullinan-0.52a1/cullinan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 09:31:36.000000 cullinan-0.52a1/cullinan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 09:31:36.000000 cullinan-0.52a1/cullinan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:31:36.352076 cullinan-0.52a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-24 09:31:23.000000 cullinan-0.52a1/setup.py
```

### Comparing `cullinan-0.51/LICENSE` & `cullinan-0.52a1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 plumeink
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cullinan-0.51/PKG-INFO` & `cullinan-0.52a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.51
+Version: 0.52a1
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: python@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.51/cullinan/application.py` & `cullinan-0.52a1/cullinan/application.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/controller.py` & `cullinan-0.52a1/cullinan/controller.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/dao.py` & `cullinan-0.52a1/cullinan/dao.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/request.py` & `cullinan-0.52a1/cullinan/request.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan/service.py` & `cullinan-0.52a1/cullinan/service.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.51/cullinan.egg-info/PKG-INFO` & `cullinan-0.52a1/cullinan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.51
+Version: 0.52a1
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: python@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.51/setup.py` & `cullinan-0.52a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
-with open("README.md", "r", encoding="UTF-8") as fh:
+with open("README.MD", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cullinan',
-    version='0.51',
+    version='0.52a1',
     packages=['cullinan'],
     description='Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application',
     author='plumeink',
     project_urls={
             'Source': 'https://github.com/plumeink/Cullinan',
             'Wiki': 'https://github.com/plumeink/Cullinan/wiki',
       },
```

