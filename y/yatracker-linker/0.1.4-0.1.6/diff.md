# Comparing `tmp/yatracker_linker-0.1.4.tar.gz` & `tmp/yatracker_linker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.1.4.tar", max compression
+gzip compressed data, was "yatracker_linker-0.1.6.tar", max compression
```

## Comparing `yatracker_linker-0.1.4.tar` & `yatracker_linker-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-04-23 08:27:49.474002 yatracker_linker-0.1.4/LICENSE
--rw-r--r--   0        0        0      111 2023-04-23 08:31:02.609765 yatracker_linker-0.1.4/README.rst
--rw-r--r--   0        0        0     1030 2023-04-23 08:45:47.693910 yatracker_linker-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 08:27:49.475738 yatracker_linker-0.1.4/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1155 2023-04-23 08:33:13.814861 yatracker_linker-0.1.4/yatracker_linker/__main__.py
--rw-r--r--   0        0        0      634 2023-04-23 08:27:49.475936 yatracker_linker-0.1.4/yatracker_linker/args.py
--rw-r--r--   0        0        0      607 2023-04-23 08:43:12.319161 yatracker_linker-0.1.4/yatracker_linker/deps.py
--rw-r--r--   0        0        0      495 2023-04-23 08:45:11.738851 yatracker_linker-0.1.4/yatracker_linker/service.py
--rw-r--r--   0        0        0     1090 2023-04-23 08:27:49.476213 yatracker_linker-0.1.4/yatracker_linker/st_client.py
--rw-r--r--   0        0        0        0 2023-04-23 08:27:49.476306 yatracker_linker-0.1.4/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0     2352 2023-04-23 08:45:11.735379 yatracker_linker-0.1.4/yatracker_linker/views/event.py
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 yatracker_linker-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-24 18:56:58.598089 yatracker_linker-0.1.6/LICENSE
+-rw-r--r--   0        0        0      111 2023-04-24 18:56:58.598089 yatracker_linker-0.1.6/README.rst
+-rw-r--r--   0        0        0     1030 2023-04-24 18:57:29.046302 yatracker_linker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1155 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0      634 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/args.py
+-rw-r--r--   0        0        0      607 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      495 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/service.py
+-rw-r--r--   0        0        0     1090 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/st_client.py
+-rw-r--r--   0        0        0        0 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0     2352 2023-04-24 18:56:58.602089 yatracker_linker-0.1.6/yatracker_linker/views/event.py
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 yatracker_linker-0.1.6/PKG-INFO
```

### Comparing `yatracker_linker-0.1.4/LICENSE` & `yatracker_linker-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.4/pyproject.toml` & `yatracker_linker-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.1.4"
+version = "0.1.6"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.1.4/yatracker_linker/__main__.py` & `yatracker_linker-0.1.6/yatracker_linker/__main__.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.4/yatracker_linker/args.py` & `yatracker_linker-0.1.6/yatracker_linker/args.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.4/yatracker_linker/deps.py` & `yatracker_linker-0.1.6/yatracker_linker/deps.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.4/yatracker_linker/st_client.py` & `yatracker_linker-0.1.6/yatracker_linker/st_client.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.4/yatracker_linker/views/event.py` & `yatracker_linker-0.1.6/yatracker_linker/views/event.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.4/PKG-INFO` & `yatracker_linker-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.1.4
+Version: 0.1.6
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

