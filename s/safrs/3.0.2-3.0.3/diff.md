# Comparing `tmp/safrs-3.0.2.tar.gz` & `tmp/safrs-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safrs-3.0.2.tar", last modified: Mon Apr 17 19:55:50 2023, max compression
+gzip compressed data, was "safrs-3.0.3.tar", last modified: Mon Apr 24 17:20:34 2023, max compression
```

## Comparing `safrs-3.0.2.tar` & `safrs-3.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-17 19:55:50.874974 safrs-3.0.2/
--rwxrwxrwx   0 t         (1000) t         (1000)    35120 2023-02-11 17:18:46.000000 safrs-3.0.2/LICENSE
--rwxrwxrwx   0 t         (1000) t         (1000)       90 2021-03-16 11:22:28.000000 safrs-3.0.2/MANIFEST.in
--rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-04-17 19:55:50.874974 safrs-3.0.2/PKG-INFO
--rwxrwxrwx   0 t         (1000) t         (1000)    16881 2023-02-18 08:57:06.000000 safrs-3.0.2/README.md
--rwxrwxrwx   0 t         (1000) t         (1000)     1374 2023-02-11 17:18:46.000000 safrs-3.0.2/README.rst
--rwxrwxrwx   0 t         (1000) t         (1000)     1422 2023-02-18 09:30:29.000000 safrs-3.0.2/pyproject.toml
--rwxrwxrwx   0 t         (1000) t         (1000)      433 2023-02-11 20:26:11.000000 safrs-3.0.2/requirements.txt
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-17 19:55:50.833125 safrs-3.0.2/safrs/
--rwxrwxrwx   0 t         (1000) t         (1000)       93 2023-04-17 19:55:11.000000 safrs-3.0.2/safrs/__about__.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1242 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/__init__.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1980 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/_safrs_relationship.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4082 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/api_methods.py
--rwxrwxrwx   0 t         (1000) t         (1000)     3349 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/attr_parse.py
--rwxrwxrwx   0 t         (1000) t         (1000)    49278 2023-04-17 19:48:20.000000 safrs-3.0.2/safrs/base.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4047 2023-02-11 20:14:12.000000 safrs-3.0.2/safrs/config.py
--rwxrwxrwx   0 t         (1000) t         (1000)     3782 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/errors.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1401 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/jabase.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4531 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/json_encoder.py
--rwxrwxrwx   0 t         (1000) t         (1000)    41386 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/jsonapi.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1682 2023-02-11 20:14:16.000000 safrs-3.0.2/safrs/jsonapi_attr.py
--rwxrwxrwx   0 t         (1000) t         (1000)     5857 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/jsonapi_filters.py
--rwxrwxrwx   0 t         (1000) t         (1000)     9866 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/jsonapi_formatting.py
--rwxrwxrwx   0 t         (1000) t         (1000)     5188 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/request.py
--rwxrwxrwx   0 t         (1000) t         (1000)      262 2023-02-11 17:18:47.000000 safrs-3.0.2/safrs/response.py
--rwxrwxrwx   0 t         (1000) t         (1000)    31273 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/safrs_api.py
--rwxrwxrwx   0 t         (1000) t         (1000)     6085 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/safrs_init.py
--rwxrwxrwx   0 t         (1000) t         (1000)     7458 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/safrs_types.py
--rwxrwxrwx   0 t         (1000) t         (1000)    26470 2023-02-18 08:46:45.000000 safrs-3.0.2/safrs/swagger_doc.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1205 2023-02-18 08:46:44.000000 safrs-3.0.2/safrs/util.py
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-17 19:55:50.871231 safrs-3.0.2/safrs.egg-info/
--rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-04-17 19:55:49.000000 safrs-3.0.2/safrs.egg-info/PKG-INFO
--rwxrwxrwx   0 t         (1000) t         (1000)      648 2023-04-17 19:55:49.000000 safrs-3.0.2/safrs.egg-info/SOURCES.txt
--rwxrwxrwx   0 t         (1000) t         (1000)        1 2023-04-17 19:55:49.000000 safrs-3.0.2/safrs.egg-info/dependency_links.txt
--rwxrwxrwx   0 t         (1000) t         (1000)      522 2023-04-17 19:55:49.000000 safrs-3.0.2/safrs.egg-info/requires.txt
--rwxrwxrwx   0 t         (1000) t         (1000)        6 2023-04-17 19:55:49.000000 safrs-3.0.2/safrs.egg-info/top_level.txt
--rwxrwxrwx   0 t         (1000) t         (1000)      263 2023-04-17 19:55:50.878962 safrs-3.0.2/setup.cfg
--rwxrwxrwx   0 t         (1000) t         (1000)     1687 2023-04-17 19:54:59.000000 safrs-3.0.2/setup.py
+drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-24 17:20:34.221684 safrs-3.0.3/
+-rwxrwxrwx   0 t         (1000) t         (1000)    35120 2023-02-11 17:18:46.000000 safrs-3.0.3/LICENSE
+-rwxrwxrwx   0 t         (1000) t         (1000)       90 2021-03-16 11:22:28.000000 safrs-3.0.3/MANIFEST.in
+-rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-04-24 17:20:34.221684 safrs-3.0.3/PKG-INFO
+-rwxrwxrwx   0 t         (1000) t         (1000)    16881 2023-02-18 08:57:06.000000 safrs-3.0.3/README.md
+-rwxrwxrwx   0 t         (1000) t         (1000)     1374 2023-02-11 17:18:46.000000 safrs-3.0.3/README.rst
+-rwxrwxrwx   0 t         (1000) t         (1000)     1422 2023-04-24 17:19:50.000000 safrs-3.0.3/pyproject.toml
+-rwxrwxrwx   0 t         (1000) t         (1000)      433 2023-02-11 20:26:11.000000 safrs-3.0.3/requirements.txt
+drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-24 17:20:34.210979 safrs-3.0.3/safrs/
+-rwxrwxrwx   0 t         (1000) t         (1000)       93 2023-04-24 17:20:18.000000 safrs-3.0.3/safrs/__about__.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1242 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/__init__.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1980 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/_safrs_relationship.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     4082 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/api_methods.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     3349 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/attr_parse.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    49278 2023-04-17 19:48:20.000000 safrs-3.0.3/safrs/base.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     4047 2023-02-11 20:14:12.000000 safrs-3.0.3/safrs/config.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     3782 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/errors.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1401 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/jabase.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     4531 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/json_encoder.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    41386 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/jsonapi.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1682 2023-02-11 20:14:16.000000 safrs-3.0.3/safrs/jsonapi_attr.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     5857 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/jsonapi_filters.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     9866 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/jsonapi_formatting.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     5188 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/request.py
+-rwxrwxrwx   0 t         (1000) t         (1000)      262 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/response.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    31273 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/safrs_api.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     6085 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/safrs_init.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     7458 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/safrs_types.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    26470 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/swagger_doc.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1205 2023-02-18 08:46:44.000000 safrs-3.0.3/safrs/util.py
+drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-24 17:20:34.220493 safrs-3.0.3/safrs.egg-info/
+-rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/PKG-INFO
+-rwxrwxrwx   0 t         (1000) t         (1000)      648 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)        1 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)      522 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/requires.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)        6 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/top_level.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)      263 2023-04-24 17:20:34.223867 safrs-3.0.3/setup.cfg
+-rwxrwxrwx   0 t         (1000) t         (1000)     1687 2023-04-24 17:20:28.000000 safrs-3.0.3/setup.py
```

### Comparing `safrs-3.0.2/LICENSE` & `safrs-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/PKG-INFO` & `safrs-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.0.2
+Version: 3.0.3
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.2.tar.gz
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.3.tar.gz
 Description: SAFRS: Python OpenAPI & JSON:API Framework
         ==========================================
         
         Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
         
         Overview
         --------
```

### Comparing `safrs-3.0.2/README.md` & `safrs-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/README.rst` & `safrs-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/pyproject.toml` & `safrs-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "safrs"
 
-version = "3.0.1"
+version = "3.0.3"
 
 description="SAFRS : SqlAlchemy Flask-Restful Swagger"
 
 readme = "README.md"
 
 requires-python = ">=3.7"
```

### Comparing `safrs-3.0.2/safrs/__init__.py` & `safrs-3.0.3/safrs/__init__.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/_safrs_relationship.py` & `safrs-3.0.3/safrs/_safrs_relationship.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/api_methods.py` & `safrs-3.0.3/safrs/api_methods.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/attr_parse.py` & `safrs-3.0.3/safrs/attr_parse.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/base.py` & `safrs-3.0.3/safrs/base.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/config.py` & `safrs-3.0.3/safrs/config.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/errors.py` & `safrs-3.0.3/safrs/errors.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/jabase.py` & `safrs-3.0.3/safrs/jabase.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/json_encoder.py` & `safrs-3.0.3/safrs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/jsonapi.py` & `safrs-3.0.3/safrs/jsonapi.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/jsonapi_attr.py` & `safrs-3.0.3/safrs/jsonapi_attr.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/jsonapi_filters.py` & `safrs-3.0.3/safrs/jsonapi_filters.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/jsonapi_formatting.py` & `safrs-3.0.3/safrs/jsonapi_formatting.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/request.py` & `safrs-3.0.3/safrs/request.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/safrs_api.py` & `safrs-3.0.3/safrs/safrs_api.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/safrs_init.py` & `safrs-3.0.3/safrs/safrs_init.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/safrs_types.py` & `safrs-3.0.3/safrs/safrs_types.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/swagger_doc.py` & `safrs-3.0.3/safrs/swagger_doc.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs/util.py` & `safrs-3.0.3/safrs/util.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs.egg-info/PKG-INFO` & `safrs-3.0.3/safrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.0.2
+Version: 3.0.3
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.2.tar.gz
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.3.tar.gz
 Description: SAFRS: Python OpenAPI & JSON:API Framework
         ==========================================
         
         Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
         
         Overview
         --------
```

### Comparing `safrs-3.0.2/safrs.egg-info/SOURCES.txt` & `safrs-3.0.3/safrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/safrs.egg-info/requires.txt` & `safrs-3.0.3/safrs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `safrs-3.0.2/setup.py` & `safrs-3.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 
 def safrs_setup():
     with open("requirements.txt", "rt") as fp:
         install_requires = fp.read().strip().split("\n")
 
-    version = "3.0.2"
+    version = "3.0.3"
 
     setup(
         name="safrs",
         packages=find_packages(exclude=['test']),
         version=version,
         license="MIT",
         description="safrs : SqlAlchemy Flask-Restful Swagger2",
```

