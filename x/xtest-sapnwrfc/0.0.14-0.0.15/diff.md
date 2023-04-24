# Comparing `tmp/xtest_sapnwrfc-0.0.14.tar.gz` & `tmp/xtest_sapnwrfc-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtest_sapnwrfc-0.0.14.tar", last modified: Mon Apr 24 14:12:17 2023, max compression
+gzip compressed data, was "xtest_sapnwrfc-0.0.15.tar", last modified: Mon Apr 24 17:30:25 2023, max compression
```

## Comparing `xtest_sapnwrfc-0.0.14.tar` & `xtest_sapnwrfc-0.0.15.tar`

### file list

```diff
@@ -1,34 +1,22 @@
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 14:12:17.424008 xtest_sapnwrfc-0.0.14/
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 14:12:17.405631 xtest_sapnwrfc-0.0.14/LICENSES/
--rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.14/LICENSES/Apache-2.0.txt
--rw-r--r--   0 d037732    (501) wheel        (0)    23591 2023-04-24 14:12:17.423629 xtest_sapnwrfc-0.0.14/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)    10368 2023-04-24 13:13:41.000000 xtest_sapnwrfc-0.0.14/README.md
--rw-r--r--   0 d037732    (501) wheel        (0)     1976 2023-04-24 14:12:14.000000 xtest_sapnwrfc-0.0.14/pyproject.toml
--rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 14:12:17.424060 xtest_sapnwrfc-0.0.14/setup.cfg
--rw-r--r--   0 d037732    (501) wheel        (0)     5751 2023-04-24 14:07:09.000000 xtest_sapnwrfc-0.0.14/setup.py
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 14:12:17.402285 xtest_sapnwrfc-0.0.14/src/
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 14:12:17.413105 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/
--rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/__init__.py
--rw-r--r--   0 d037732    (501) wheel        (0)  2315334 2023-04-24 13:40:35.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_cyrfc.cpp
--rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_cyrfc.pyx
--rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_exception.py
--rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_utils.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)    23820 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/csapnwrfc.pxd
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 14:12:17.415442 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc.egg-info/
--rw-r--r--   0 d037732    (501) wheel        (0)    23591 2023-04-24 14:12:17.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc.egg-info/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)      691 2023-04-24 14:12:17.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc.egg-info/SOURCES.txt
--rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 14:12:17.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc.egg-info/dependency_links.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 14:12:17.000000 xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc.egg-info/top_level.txt
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 14:12:17.423008 xtest_sapnwrfc-0.0.14/tests/
--rwxr-xr-x   0 d037732    (501) wheel        (0)     4386 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_client_config.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     8887 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_connection.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)    26084 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_datatypes.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     3943 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_errors.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     7218 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_errors_abap.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     3471 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_options.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)      690 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_rfcsdk.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     2703 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_server.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)      988 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_table_type.py
--rw-r--r--   0 d037732    (501) wheel        (0)     4887 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_throughput.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     2227 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_timeout.py
--rwxr-xr-x   0 d037732    (501) wheel        (0)     1519 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.14/tests/test_wsrfc.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:30:25.414883 xtest_sapnwrfc-0.0.15/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:30:25.399293 xtest_sapnwrfc-0.0.15/LICENSES/
+-rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.15/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)       78 2023-04-24 14:29:18.000000 xtest_sapnwrfc-0.0.15/MANIFEST.in
+-rw-r--r--   0 d037732    (501) wheel        (0)    23591 2023-04-24 17:30:25.413863 xtest_sapnwrfc-0.0.15/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)    10368 2023-04-24 13:13:41.000000 xtest_sapnwrfc-0.0.15/README.md
+-rw-r--r--   0 d037732    (501) wheel        (0)     1838 2023-04-24 17:30:21.000000 xtest_sapnwrfc-0.0.15/pyproject.toml
+-rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 17:30:25.414934 xtest_sapnwrfc-0.0.15/setup.cfg
+-rw-r--r--   0 d037732    (501) wheel        (0)     5751 2023-04-24 17:29:54.000000 xtest_sapnwrfc-0.0.15/setup.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:30:25.396778 xtest_sapnwrfc-0.0.15/src/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:30:25.409719 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/__init__.py
+-rw-r--r--   0 d037732    (501) wheel        (0)  2315334 2023-04-24 13:40:35.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_cyrfc.cpp
+-rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_cyrfc.pyx
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_exception.py
+-rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_utils.py
+-rwxr-xr-x   0 d037732    (501) wheel        (0)    23820 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/csapnwrfc.pxd
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 17:30:25.413194 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc.egg-info/
+-rw-r--r--   0 d037732    (501) wheel        (0)    23591 2023-04-24 17:30:25.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc.egg-info/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)      423 2023-04-24 17:30:25.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 17:30:25.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 17:30:25.000000 xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc.egg-info/top_level.txt
```

### Comparing `xtest_sapnwrfc-0.0.14/LICENSES/Apache-2.0.txt` & `xtest_sapnwrfc-0.0.15/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/PKG-INFO` & `xtest_sapnwrfc-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtest_sapnwrfc
-Version: 0.0.14
+Version: 0.0.15
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

### Comparing `xtest_sapnwrfc-0.0.14/README.md` & `xtest_sapnwrfc-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/pyproject.toml` & `xtest_sapnwrfc-0.0.15/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["Cython ~= 0.29.0", "setuptools ~= 67.7.0", "wheel ~= 0.40.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "xtest_sapnwrfc"
-version = "0.0.14"
+version = "0.0.15"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"} ]
 maintainers = [ { name = "Srdjan Boskovic", email = "srdjan.boskovic@sap.com" } ]
 requires-python = ">=3.7"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
@@ -38,22 +38,16 @@
 repository = "https://github.com/SAP/PyRFC.git"
 
 [tool.cython-lint]
 max-line-length = 148
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [tool.setuptools]
-include-package-data = false
-# exclude-package-data = {"*" = ["*.cpp", "*.html", "*.pyx", "*.pxd"]}
+#include-package-data = false
+exclude-package-data = {"*" = ["*.cpp", "*.html", "*.pxd"]}
 license-files=["LICENSES/*.txt"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.setuptools.package-data]
-xtest_sapnwrfc = ["*.pxd"]
-
-#[tool.setuptools.exclude-package-data]
-#xtest_sapnwrfc = ["*.pyx"]
-
 [tool.setuptools.dynamic]
 readme = {file = "README.md"}
```

### Comparing `xtest_sapnwrfc-0.0.14/setup.py` & `xtest_sapnwrfc-0.0.15/setup.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/__init__.py` & `xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/__init__.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_cyrfc.cpp` & `xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_cyrfc.cpp`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_cyrfc.pyx` & `xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/_exception.py` & `xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/_exception.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc/csapnwrfc.pxd` & `xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc/csapnwrfc.pxd`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.14/src/xtest_sapnwrfc.egg-info/PKG-INFO` & `xtest_sapnwrfc-0.0.15/src/xtest_sapnwrfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtest-sapnwrfc
-Version: 0.0.14
+Version: 0.0.15
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Maintainer-email: Srdjan Boskovic <srdjan.boskovic@sap.com>
 License: Apache License
         
         Version 2.0, January 2004
```

