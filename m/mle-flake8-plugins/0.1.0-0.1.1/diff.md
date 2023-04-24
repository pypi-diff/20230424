# Comparing `tmp/mle_flake8_plugins-0.1.0.tar.gz` & `tmp/mle_flake8_plugins-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mle_flake8_plugins-0.1.0.tar", max compression
+gzip compressed data, was "mle_flake8_plugins-0.1.1.tar", max compression
```

## Comparing `mle_flake8_plugins-0.1.0.tar` & `mle_flake8_plugins-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/__init__.py
--rw-r--r--   0        0        0      680 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/__init__.py
--rw-r--r--   0        0        0      143 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/errors.py
--rw-r--r--   0        0        0     1303 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
--rw-r--r--   0        0        0     1275 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
--rw-r--r--   0        0        0     2178 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_docstring/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
--rw-r--r--   0        0        0      105 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_docstring/errors.py
--rw-r--r--   0        0        0      576 2023-04-12 10:31:06.066084 mle_flake8_plugins-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/__init__.py
+-rw-r--r--   0        0        0      680 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/errors.py
+-rw-r--r--   0        0        0     1303 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
+-rw-r--r--   0        0        0     1287 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
+-rw-r--r--   0        0        0     2178 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/__init__.py
+-rw-r--r--   0        0        0     1910 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
+-rw-r--r--   0        0        0      105 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/errors.py
+-rw-r--r--   0        0        0      576 2023-04-24 11:57:49.114226 mle_flake8_plugins-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.1.1/PKG-INFO
```

### Comparing `mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/__init__.py` & `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py` & `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py` & `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,12 +44,12 @@
 
     def visit_FunctionDef(self, node: ast.FunctionDef) -> None:
         has_only_pass = len(node.body) == 1 and isinstance(node.body[0], ast.Pass)
 
         if not has_only_pass:
             operations_count = self._count_operations(node)
             if operations_count < 1:
-                self.errors.append((node.lineno, node.col_offset, error_codes["no_operation"]))
+                self.errors.append((node.lineno, node.col_offset, error_codes["no_operation"], type(self)))
         self.generic_visit(node)
 
     def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> None:
         self.visit_FunctionDef(node)
```

### Comparing `mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_docstring/__init__.py` & `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.0/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py` & `mle_flake8_plugins-0.1.1/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.1.0/pyproject.toml` & `mle_flake8_plugins-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mle-flake8-plugins"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docstring-parser = "^0.15"
 flake8 = "^5.0.4"
```

