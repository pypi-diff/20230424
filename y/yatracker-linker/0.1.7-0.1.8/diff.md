# Comparing `tmp/yatracker_linker-0.1.7.tar.gz` & `tmp/yatracker_linker-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatracker_linker-0.1.7.tar", max compression
+gzip compressed data, was "yatracker_linker-0.1.8.tar", max compression
```

## Comparing `yatracker_linker-0.1.7.tar` & `yatracker_linker-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/LICENSE
--rw-r--r--   0        0        0      111 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/README.rst
--rw-r--r--   0        0        0     1030 2023-04-24 19:23:07.552797 yatracker_linker-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/__init__.py
--rw-r--r--   0        0        0     1155 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/__main__.py
--rw-r--r--   0        0        0      634 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/args.py
--rw-r--r--   0        0        0      607 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/deps.py
--rw-r--r--   0        0        0      495 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/service.py
--rw-r--r--   0        0        0     1090 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/st_client.py
--rw-r--r--   0        0        0        0 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/views/__init__.py
--rw-r--r--   0        0        0     2352 2023-04-24 19:22:43.380833 yatracker_linker-0.1.7/yatracker_linker/views/event.py
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 yatracker_linker-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/LICENSE
+-rw-r--r--   0        0        0      111 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/README.rst
+-rw-r--r--   0        0        0     1030 2023-04-24 19:45:12.973058 yatracker_linker-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/__init__.py
+-rw-r--r--   0        0        0     1155 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/__main__.py
+-rw-r--r--   0        0        0      634 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/args.py
+-rw-r--r--   0        0        0      607 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/deps.py
+-rw-r--r--   0        0        0      495 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/service.py
+-rw-r--r--   0        0        0     1090 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/st_client.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/views/__init__.py
+-rw-r--r--   0        0        0     2352 2023-04-24 19:44:38.847118 yatracker_linker-0.1.8/yatracker_linker/views/event.py
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 yatracker_linker-0.1.8/PKG-INFO
```

### Comparing `yatracker_linker-0.1.7/LICENSE` & `yatracker_linker-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.7/pyproject.toml` & `yatracker_linker-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yatracker-linker"
-version = "0.1.7"
+version = "0.1.8"
 description = "Yandex Tracker issues integration"
 license = "MIT"
 authors = ["Alexander Vasin <hi@alvass.in>"]
 readme = "README.rst"
 packages = [{include = "yatracker_linker"}]
 
 [tool.poetry.scripts]
```

### Comparing `yatracker_linker-0.1.7/yatracker_linker/__main__.py` & `yatracker_linker-0.1.8/yatracker_linker/__main__.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.7/yatracker_linker/args.py` & `yatracker_linker-0.1.8/yatracker_linker/args.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.7/yatracker_linker/deps.py` & `yatracker_linker-0.1.8/yatracker_linker/deps.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.7/yatracker_linker/st_client.py` & `yatracker_linker-0.1.8/yatracker_linker/st_client.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.7/yatracker_linker/views/event.py` & `yatracker_linker-0.1.8/yatracker_linker/views/event.py`

 * *Files identical despite different names*

### Comparing `yatracker_linker-0.1.7/PKG-INFO` & `yatracker_linker-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatracker-linker
-Version: 0.1.7
+Version: 0.1.8
 Summary: Yandex Tracker issues integration
 License: MIT
 Author: Alexander Vasin
 Author-email: hi@alvass.in
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

