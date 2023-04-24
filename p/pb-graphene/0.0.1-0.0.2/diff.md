# Comparing `tmp/pb-graphene-0.0.1.tar.gz` & `tmp/pb-graphene-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pb-graphene-0.0.1.tar", last modified: Mon Apr 24 12:35:19 2023, max compression
+gzip compressed data, was "pb-graphene-0.0.2.tar", last modified: Mon Apr 24 14:29:25 2023, max compression
```

## Comparing `pb-graphene-0.0.1.tar` & `pb-graphene-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:35:19.990873 pb-graphene-0.0.1/
--rw-rw-rw-   0        0        0     1302 2023-04-24 12:23:57.000000 pb-graphene-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      521 2023-04-24 12:35:19.989905 pb-graphene-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 12:24:04.000000 pb-graphene-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 12:35:19.987912 pb-graphene-0.0.1/pb_graphene.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-24 12:35:19.000000 pb-graphene-0.0.1/pb_graphene.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-24 12:35:19.000000 pb-graphene-0.0.1/pb_graphene.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:35:19.000000 pb-graphene-0.0.1/pb_graphene.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:35:19.000000 pb-graphene-0.0.1/pb_graphene.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      510 2023-04-24 12:29:48.000000 pb-graphene-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 12:35:19.990873 pb-graphene-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 14:29:25.024072 pb-graphene-0.0.2/
+-rw-rw-rw-   0        0        0     1302 2023-04-24 12:23:57.000000 pb-graphene-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      586 2023-04-24 14:29:25.024072 pb-graphene-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 12:24:04.000000 pb-graphene-0.0.2/README.md
+-rw-rw-rw-   0        0        0      510 2023-04-24 13:49:04.000000 pb-graphene-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1074 2023-04-24 14:29:25.025071 pb-graphene-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-24 13:57:44.000000 pb-graphene-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:29:24.985446 pb-graphene-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 14:29:25.010450 pb-graphene-0.0.2/src/pb_graphene/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:24:46.000000 pb-graphene-0.0.2/src/pb_graphene/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:29:25.022546 pb-graphene-0.0.2/src/pb_graphene/django/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:16:38.000000 pb-graphene-0.0.2/src/pb_graphene/django/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-04-24 14:24:11.000000 pb-graphene-0.0.2/src/pb_graphene/django/mutation.py
+-rw-rw-rw-   0        0        0      637 2023-04-24 14:24:45.000000 pb-graphene-0.0.2/src/pb_graphene/global_id.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:29:25.018278 pb-graphene-0.0.2/src/pb_graphene.egg-info/
+-rw-rw-rw-   0        0        0      586 2023-04-24 14:29:24.000000 pb-graphene-0.0.2/src/pb_graphene.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-04-24 14:29:24.000000 pb-graphene-0.0.2/src/pb_graphene.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:29:24.000000 pb-graphene-0.0.2/src/pb_graphene.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-24 14:29:24.000000 pb-graphene-0.0.2/src/pb_graphene.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 14:29:24.000000 pb-graphene-0.0.2/src/pb_graphene.egg-info/top_level.txt
```

### Comparing `pb-graphene-0.0.1/LICENSE` & `pb-graphene-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pb-graphene-0.0.1/PKG-INFO` & `pb-graphene-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: pb-graphene
-Version: 0.0.1
+Version: 0.0.2
 Summary: Additional utils to work with graphene, such as file uploads
+Home-page: https://github.com/gpabois/pb-graphene
 Author: Gaël Pabois
+License: MIT
 Project-URL: Homepage, https://github.com/gpabois/pb-graphene
 Project-URL: Bug Tracker, https://github.com/pypa/pb-graphene/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pb-graphene-0.0.1/pb_graphene.egg-info/PKG-INFO` & `pb-graphene-0.0.2/src/pb_graphene.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: pb-graphene
-Version: 0.0.1
+Version: 0.0.2
 Summary: Additional utils to work with graphene, such as file uploads
+Home-page: https://github.com/gpabois/pb-graphene
 Author: Gaël Pabois
+License: MIT
 Project-URL: Homepage, https://github.com/gpabois/pb-graphene
 Project-URL: Bug Tracker, https://github.com/pypa/pb-graphene/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

