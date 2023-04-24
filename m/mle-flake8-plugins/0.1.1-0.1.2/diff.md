# Comparing `tmp/mle_flake8_plugins-0.1.1.tar.gz` & `tmp/mle_flake8_plugins-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mle_flake8_plugins-0.1.1.tar", max compression
+gzip compressed data, was "mle_flake8_plugins-0.1.2.tar", max compression
```

## Comparing `mle_flake8_plugins-0.1.1.tar` & `mle_flake8_plugins-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/__init__.py
--rw-r--r--   0        0        0      680 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/__init__.py
--rw-r--r--   0        0        0      143 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/errors.py
--rw-r--r--   0        0        0     1303 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
--rw-r--r--   0        0        0     1287 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
--rw-r--r--   0        0        0     2178 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
--rw-r--r--   0        0        0      105 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/errors.py
--rw-r--r--   0        0        0      576 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/__init__.py
+-rw-r--r--   0        0        0      680 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_convention/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_convention/errors.py
+-rw-r--r--   0        0        0     1303 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
+-rw-r--r--   0        0        0     1883 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
+-rw-r--r--   0        0        0     2178 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_docstring/__init__.py
+-rw-r--r--   0        0        0     1910 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
+-rw-r--r--   0        0        0      105 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_docstring/errors.py
+-rw-r--r--   0        0        0      576 2023-04-24 12:40:03.080157 mle_flake8_plugins-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.1.2/PKG-INFO
```

### Comparing `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/__init__.py` & `mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_convention/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py` & `mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/__init__.py` & `mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_docstring/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py` & `mle_flake8_plugins-0.1.2/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.1/pyproject.toml` & `mle_flake8_plugins-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mle-flake8-plugins"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docstring-parser = "^0.15"
 flake8 = "^5.0.4"
```

