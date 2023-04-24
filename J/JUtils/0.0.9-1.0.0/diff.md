# Comparing `tmp/JUtils-0.0.9.tar.gz` & `tmp/JUtils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JUtils-0.0.9.tar", last modified: Mon Apr 24 19:09:52 2023, max compression
+gzip compressed data, was "JUtils-1.0.0.tar", last modified: Mon Apr 24 19:15:19 2023, max compression
```

## Comparing `JUtils-0.0.9.tar` & `JUtils-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.759222 JUtils-0.0.9/
--rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     8815 2023-04-24 19:09:52.759222 JUtils-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     8369 2023-01-06 11:38:01.000000 JUtils-0.0.9/README.md
--rw-rw-rw-   0        0        0      522 2023-04-24 15:27:30.000000 JUtils-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 19:09:52.759222 JUtils-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.731665 JUtils-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.745706 JUtils-0.0.9/src/JUtils/
--rw-rw-rw-   0        0        0     1715 2023-04-24 19:00:30.000000 JUtils-0.0.9/src/JUtils/AutoDoc.py
--rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-0.0.9/src/JUtils/JArr.py
--rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-0.0.9/src/JUtils/JColors.py
--rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-0.0.9/src/JUtils/JConst.py
--rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-0.0.9/src/JUtils/JConv.py
--rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-0.0.9/src/JUtils/JNum.py
--rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-0.0.9/src/JUtils/JOut.py
--rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-0.0.9/src/JUtils/JStr.py
--rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-0.0.9/src/JUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:52.757223 JUtils-0.0.9/src/JUtils.egg-info/
--rw-rw-rw-   0        0        0     8815 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 19:09:52.000000 JUtils-0.0.9/src/JUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:15:19.196532 JUtils-1.0.0/
+-rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     8726 2023-04-24 19:15:19.195532 JUtils-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8280 2023-04-24 19:05:20.000000 JUtils-1.0.0/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-24 19:13:42.000000 JUtils-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:15:19.196532 JUtils-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 19:15:19.173494 JUtils-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:15:19.183019 JUtils-1.0.0/src/JUtils/
+-rw-rw-rw-   0        0        0     1715 2023-04-24 19:00:30.000000 JUtils-1.0.0/src/JUtils/AutoDoc.py
+-rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-1.0.0/src/JUtils/JArr.py
+-rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-1.0.0/src/JUtils/JColors.py
+-rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-1.0.0/src/JUtils/JConst.py
+-rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-1.0.0/src/JUtils/JConv.py
+-rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-1.0.0/src/JUtils/JNum.py
+-rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-1.0.0/src/JUtils/JOut.py
+-rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-1.0.0/src/JUtils/JStr.py
+-rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-1.0.0/src/JUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:15:19.194532 JUtils-1.0.0/src/JUtils.egg-info/
+-rw-rw-rw-   0        0        0     8726 2023-04-24 19:15:19.000000 JUtils-1.0.0/src/JUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-04-24 19:15:19.000000 JUtils-1.0.0/src/JUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:15:19.000000 JUtils-1.0.0/src/JUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 19:15:19.000000 JUtils-1.0.0/src/JUtils.egg-info/top_level.txt
```

### Comparing `JUtils-0.0.9/LICENSE` & `JUtils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/pyproject.toml` & `JUtils-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "JUtils"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
   { name="Jan Seifert", email="jan@seifert-online.de" },
 ]
 description = "Package containing various utility functions i needed now and then, that i wanted to share"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `JUtils-0.0.9/src/JUtils/AutoDoc.py` & `JUtils-1.0.0/src/JUtils/AutoDoc.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/src/JUtils/JArr.py` & `JUtils-1.0.0/src/JUtils/JArr.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/src/JUtils/JColors.py` & `JUtils-1.0.0/src/JUtils/JColors.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/src/JUtils/JConv.py` & `JUtils-1.0.0/src/JUtils/JConv.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/src/JUtils/JNum.py` & `JUtils-1.0.0/src/JUtils/JNum.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/src/JUtils/JOut.py` & `JUtils-1.0.0/src/JUtils/JOut.py`

 * *Files identical despite different names*

### Comparing `JUtils-0.0.9/src/JUtils/JStr.py` & `JUtils-1.0.0/src/JUtils/JStr.py`

 * *Files identical despite different names*

