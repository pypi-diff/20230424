# Comparing `tmp/rustimport-1.2.5.tar.gz` & `tmp/rustimport-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustimport-1.2.5.tar", last modified: Mon Apr 17 23:08:31 2023, max compression
+gzip compressed data, was "rustimport-1.3.0.tar", last modified: Mon Apr 24 13:07:32 2023, max compression
```

## Comparing `rustimport-1.2.5.tar` & `rustimport-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.108228 rustimport-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 23:08:16.000000 rustimport-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 23:08:16.000000 rustimport-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-17 23:08:31.108228 rustimport-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-17 23:08:16.000000 rustimport-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 23:08:16.000000 rustimport-1.2.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.104227 rustimport-1.2.5/rustimport/
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/importable.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.104227 rustimport-1.2.5/rustimport/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/pre_processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/pre_processing/pyo3_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.104227 rustimport-1.2.5/rustimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:08:30.000000 rustimport-1.2.5/rustimport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:08:31.108228 rustimport-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-17 23:08:16.000000 rustimport-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.108228 rustimport-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 23:08:16.000000 rustimport-1.2.5/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-17 23:08:16.000000 rustimport-1.2.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-17 23:08:16.000000 rustimport-1.2.5/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:07:32.421646 rustimport-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 13:07:11.000000 rustimport-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 13:07:11.000000 rustimport-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-24 13:07:32.421646 rustimport-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-24 13:07:11.000000 rustimport-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:07:11.000000 rustimport-1.3.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:07:32.417646 rustimport-1.3.0/rustimport/
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/importable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:07:32.421646 rustimport-1.3.0/rustimport/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/pre_processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/pre_processing/pyo3_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-24 13:07:11.000000 rustimport-1.3.0/rustimport/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:07:32.421646 rustimport-1.3.0/rustimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-24 13:07:32.000000 rustimport-1.3.0/rustimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-24 13:07:32.000000 rustimport-1.3.0/rustimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:07:32.000000 rustimport-1.3.0/rustimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:07:32.000000 rustimport-1.3.0/rustimport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 13:07:32.000000 rustimport-1.3.0/rustimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 13:07:32.000000 rustimport-1.3.0/rustimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:07:32.421646 rustimport-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-24 13:07:11.000000 rustimport-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:07:32.421646 rustimport-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:07:11.000000 rustimport-1.3.0/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-24 13:07:11.000000 rustimport-1.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-24 13:07:11.000000 rustimport-1.3.0/tests/test_examples.py
```

### Comparing `rustimport-1.2.5/LICENSE` & `rustimport-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/PKG-INFO` & `rustimport-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.2.5
+Version: 1.3.0
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.2.5/README.md` & `rustimport-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/__init__.py` & `rustimport-1.3.0/rustimport/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/__main__.py` & `rustimport-1.3.0/rustimport/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 # "cdylib" is necessary to produce a shared library for Python to import from.
 # Downstream Rust code (including code in `bin/`, `examples/`, and `examples/`) will not be able
 # to `use {{EXTENSION_NAME}};` unless the "rlib" or "lib" crate type is also included, e.g.:
 # crate-type = ["cdylib", "rlib"]
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.16.2", features = ["extension-module"] }
+pyo3 = { version = "0.18.3", features = ["extension-module"] }
 """
 
 
 def create_extension(name: str):
     if not re.match(r'^[a-zA-Z]\w*(\.rs)?$', name):
         raise ValueError(f"Invalid extension name: {name}. The name may only contain letters (preferably lowercase), "
                          f"numbers and underscores and should start with a letter.")
```

### Comparing `rustimport-1.2.5/rustimport/checksum.py` & `rustimport-1.3.0/rustimport/checksum.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/compiler.py` & `rustimport-1.3.0/rustimport/compiler.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/error_handling.py` & `rustimport-1.3.0/rustimport/error_handling.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/find.py` & `rustimport-1.3.0/rustimport/find.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/import_hook.py` & `rustimport-1.3.0/rustimport/import_hook.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/importable.py` & `rustimport-1.3.0/rustimport/importable.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/load.py` & `rustimport-1.3.0/rustimport/load.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/pre_processing/__init__.py` & `rustimport-1.3.0/rustimport/pre_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/pre_processing/base.py` & `rustimport-1.3.0/rustimport/pre_processing/base.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport/pre_processing/pyo3_template.py` & `rustimport-1.3.0/rustimport/pre_processing/pyo3_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,28 @@
                 'edition': '2021',
             },
             'lib': {
                 'name': self.lib_name,
                 'crate-type': ['cdylib'],
             },
             'dependencies': {
-                'pyo3': {'version': '0.16.2', 'features': ['extension-module']}
+                'pyo3': {'version': '0.18.3', 'features': ['extension-module']}
             }
         })
 
     def __process_content(self) -> bytes:
         if not re.search(rb'#\[pymodule]\s*(?:\w\s+)*?fn\s+([\w0-9]+)', self.contents):
             # If the file doesn't contain the "pymodule" macro, we generate it automatically
             return self.contents + b"\n\n" + self.__generate_pymodule()
 
     def __generate_pymodule(self) -> bytes:
         # A rather rudimentary implementation of generating PyO3 the "pymodule" macro's contents
-        functions = re.finditer(rb'#\[pyfunction]\s*(?:\w+\s+)*?fn\s+([\w0-9]+)', self.contents, re.MULTILINE)
+        functions = re.finditer(
+            rb'#\[pyfunction.*\s*(?:\w+\s+)*?(?:#\[pyo3.*)?\s*(?:\w+\s+)*?fn\s+([\w0-9]+)', self.contents, re.MULTILINE
+        )
         structs = re.finditer(rb'#\[pyclass]\s*(?:\w+\s+)*?(?:struct|enum)\s+([\w0-9]+)', self.contents, re.MULTILINE)
 
         res = [
             b'#[pymodule]',
             b'fn ' + self.lib_name.encode() + b'(_py: Python, m: &PyModule) -> PyResult<()> {',
             *[
                 b'  m.add_function(wrap_pyfunction!(' + func.group(1) + b', m)?)?;'
```

### Comparing `rustimport-1.2.5/rustimport/settings.py` & `rustimport-1.3.0/rustimport/settings.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/rustimport.egg-info/PKG-INFO` & `rustimport-1.3.0/rustimport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.2.5
+Version: 1.3.0
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.2.5/rustimport.egg-info/SOURCES.txt` & `rustimport-1.3.0/rustimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/setup.py` & `rustimport-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/tests/test_cli.py` & `rustimport-1.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.5/tests/test_examples.py` & `rustimport-1.3.0/tests/test_examples.py`

 * *Files identical despite different names*

