# Comparing `tmp/spycio-0.2.7.tar.gz` & `tmp/spycio-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spycio-0.2.7.tar", max compression
+gzip compressed data, was "spycio-0.2.8.tar", max compression
```

## Comparing `spycio-0.2.7.tar` & `spycio-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.7/LICENSE
--rw-r--r--   0        0        0     3088 2023-04-23 21:32:05.272425 spycio-0.2.7/README.md
--rw-r--r--   0        0        0     1376 2023-04-24 21:14:37.961344 spycio-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.7/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
--rw-r--r--   0        0        0      412 2023-04-24 21:12:30.128846 spycio-0.2.7/spycio/__init__.py
--rw-r--r--   0        0        0     7409 2023-04-23 21:33:14.616696 spycio-0.2.7/spycio/spycio.py
--rw-r--r--   0        0        0     4279 2023-04-23 11:21:08.123530 spycio-0.2.7/spycio/utils.py
--rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 spycio-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-01 13:17:00.225289 spycio-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3088 2023-04-23 21:32:05.272425 spycio-0.2.8/README.md
+-rw-r--r--   0        0        0     1376 2023-04-24 21:21:58.595062 spycio-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    14858 2023-04-01 13:17:00.225289 spycio-0.2.8/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb
+-rw-r--r--   0        0        0      417 2023-04-24 21:21:21.710918 spycio-0.2.8/spycio/__init__.py
+-rw-r--r--   0        0        0     7409 2023-04-23 21:33:14.616696 spycio-0.2.8/spycio/spycio.py
+-rw-r--r--   0        0        0     4279 2023-04-23 11:21:08.123530 spycio-0.2.8/spycio/utils.py
+-rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 spycio-0.2.8/PKG-INFO
```

### Comparing `spycio-0.2.7/LICENSE` & `spycio-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spycio-0.2.7/README.md` & `spycio-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `spycio-0.2.7/pyproject.toml` & `spycio-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spycio"
-version = "0.2.7"
+version = "0.2.8"
 description = "Distances in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "spycio"}]
 homepage = "https://pypi.org/project/spycio/"
 repository = "https://github.com/trouchet/spycio"
```

### Comparing `spycio-0.2.7/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb` & `spycio-0.2.8/spycio/.ipynb_checkpoints/euler_diagram-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `spycio-0.2.7/spycio/spycio.py` & `spycio-0.2.8/spycio/spycio.py`

 * *Files identical despite different names*

### Comparing `spycio-0.2.7/spycio/utils.py` & `spycio-0.2.8/spycio/utils.py`

 * *Files identical despite different names*

### Comparing `spycio-0.2.7/PKG-INFO` & `spycio-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spycio
-Version: 0.2.7
+Version: 0.2.8
 Summary: Distances in python
 Home-page: https://pypi.org/project/spycio/
 License: MIT
 Keywords: distance
 Author: Bruno Peixoto
 Author-email: brunolnetto@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

