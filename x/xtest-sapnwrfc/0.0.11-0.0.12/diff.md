# Comparing `tmp/xtest_sapnwrfc-0.0.11.tar.gz` & `tmp/xtest_sapnwrfc-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtest_sapnwrfc-0.0.11.tar", last modified: Mon Apr 24 11:54:43 2023, max compression
+gzip compressed data, was "xtest_sapnwrfc-0.0.12.tar", last modified: Mon Apr 24 11:58:27 2023, max compression
```

## Comparing `xtest_sapnwrfc-0.0.11.tar` & `xtest_sapnwrfc-0.0.12.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:54:43.640716 xtest_sapnwrfc-0.0.11/
--rw-r--r--   0 d037732    (501) wheel        (0)    10273 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.11/LICENSE
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:54:43.630130 xtest_sapnwrfc-0.0.11/LICENSES/
--rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.11/LICENSES/Apache-2.0.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       79 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.11/MANIFEST.in
--rw-r--r--   0 d037732    (501) wheel        (0)    23350 2023-04-24 11:54:43.640237 xtest_sapnwrfc-0.0.11/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)    10133 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.11/README.md
--rw-r--r--   0 d037732    (501) wheel        (0)     1764 2023-04-24 11:54:18.000000 xtest_sapnwrfc-0.0.11/pyproject.toml
--rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 11:54:43.640802 xtest_sapnwrfc-0.0.11/setup.cfg
--rw-r--r--   0 d037732    (501) wheel        (0)     6358 2023-04-24 11:54:39.000000 xtest_sapnwrfc-0.0.11/setup.py
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:54:43.624593 xtest_sapnwrfc-0.0.11/src/
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:54:43.635098 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/
--rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/__init__.py
--rw-r--r--   0 d037732    (501) wheel        (0)  2353011 2023-04-24 11:28:26.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_cyrfc.cpp
--rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_cyrfc.pyx
--rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_exception.py
--rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_utils.py
-drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:54:43.639687 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc.egg-info/
--rw-r--r--   0 d037732    (501) wheel        (0)    23350 2023-04-24 11:54:43.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc.egg-info/PKG-INFO
--rw-r--r--   0 d037732    (501) wheel        (0)      398 2023-04-24 11:54:43.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc.egg-info/SOURCES.txt
--rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 11:54:43.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc.egg-info/dependency_links.txt
--rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 11:54:43.000000 xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc.egg-info/top_level.txt
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.391621 xtest_sapnwrfc-0.0.12/
+-rw-r--r--   0 d037732    (501) wheel        (0)    10273 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/LICENSE
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.378096 xtest_sapnwrfc-0.0.12/LICENSES/
+-rw-r--r--   0 d037732    (501) wheel        (0)    10283 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)       79 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/MANIFEST.in
+-rw-r--r--   0 d037732    (501) wheel        (0)    23350 2023-04-24 11:58:27.391325 xtest_sapnwrfc-0.0.12/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)    10133 2023-04-24 08:04:52.000000 xtest_sapnwrfc-0.0.12/README.md
+-rw-r--r--   0 d037732    (501) wheel        (0)     1764 2023-04-24 11:57:59.000000 xtest_sapnwrfc-0.0.12/pyproject.toml
+-rw-r--r--   0 d037732    (501) wheel        (0)       38 2023-04-24 11:58:27.391679 xtest_sapnwrfc-0.0.12/setup.cfg
+-rw-r--r--   0 d037732    (501) wheel        (0)     6349 2023-04-24 11:57:35.000000 xtest_sapnwrfc-0.0.12/setup.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.375329 xtest_sapnwrfc-0.0.12/src/
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.386857 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     1339 2023-04-24 11:29:18.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/__init__.py
+-rw-r--r--   0 d037732    (501) wheel        (0)  2353011 2023-04-24 11:28:26.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.cpp
+-rwxr-xr-x   0 d037732    (501) wheel        (0)   129750 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.pyx
+-rwxr-xr-x   0 d037732    (501) wheel        (0)     5594 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_exception.py
+-rw-r--r--   0 d037732    (501) wheel        (0)      292 2023-04-24 08:04:53.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_utils.py
+drwxr-xr-x   0 d037732    (501) wheel        (0)        0 2023-04-24 11:58:27.390858 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/
+-rw-r--r--   0 d037732    (501) wheel        (0)    23350 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/PKG-INFO
+-rw-r--r--   0 d037732    (501) wheel        (0)      398 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)        1 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 d037732    (501) wheel        (0)       15 2023-04-24 11:58:27.000000 xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/top_level.txt
```

### Comparing `xtest_sapnwrfc-0.0.11/LICENSE` & `xtest_sapnwrfc-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/LICENSES/Apache-2.0.txt` & `xtest_sapnwrfc-0.0.12/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/PKG-INFO` & `xtest_sapnwrfc-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtest_sapnwrfc
-Version: 0.0.11
+Version: 0.0.12
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Maintainer: Srdjan Boskovic
 Maintainer-email: srdjan.boskovic@sap.com
 License: Apache License
         
         Version 2.0, January 2004
```

### Comparing `xtest_sapnwrfc-0.0.11/README.md` & `xtest_sapnwrfc-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/pyproject.toml` & `xtest_sapnwrfc-0.0.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["Cython >= 0.29.0", "setuptools >= 67.7.0", "wheel >= 0.40.0"]
+requires = ["Cython ~= 0.29.0", "setuptools ~= 67.7.0", "wheel ~= 0.40.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "xtest_sapnwrfc"
-version = "0.0.11"
+version = "0.0.12"
 readme = "README.md"
 license = { file = "LICENSES/Apache-2.0.txt" }
 description = "Python bindings for SAP NetWeaver RFC SDK"
 authors = [ { name = "SAP SE"} ]
 maintainers = [ { name = "Srdjan Boskovic" } ]
 requires-python = ">=3.7"
 keywords = ["pyrfc", "sap", "nwrfc", "sapnwrfc", "abap"]
```

### Comparing `xtest_sapnwrfc-0.0.11/setup.py` & `xtest_sapnwrfc-0.0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 setup(
     name=PACKAGE_NAME,
     #version="2.8.3", # __version__,
     #description=("Python bindings for SAP NetWeaver RFC SDK"),
     #long_description="readme_md",
     #long_description_content_type="text/markdown",
     #download_url="https://github.com/SAP/PyRFC/tarball/main",
-    packages=find_packages(where="src", exclude=["*.cpp", "*.pxd", "*.html"]),
+    packages=find_packages(where="src", exclude=["*.cpp", "*.html"]),
     package_dir={"": "src"},
     #keywords=f"pyrfc sap rfc nwrfc sapnwrfc",
     #author="SAP SE",
     #url="https://github.com/SAP/pyrfc",
     #license="OSI Approved :: Apache Software License",
     maintainer="Srdjan Boskovic",
     maintainer_email="srdjan.boskovic@sap.com",
```

### Comparing `xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/__init__.py` & `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/__init__.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_cyrfc.cpp` & `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.cpp`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_cyrfc.pyx` & `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_cyrfc.pyx`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc/_exception.py` & `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc/_exception.py`

 * *Files identical despite different names*

### Comparing `xtest_sapnwrfc-0.0.11/src/xtest_sapnwrfc.egg-info/PKG-INFO` & `xtest_sapnwrfc-0.0.12/src/xtest_sapnwrfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtest-sapnwrfc
-Version: 0.0.11
+Version: 0.0.12
 Summary: Python bindings for SAP NetWeaver RFC SDK
 Author: SAP SE
 Maintainer: Srdjan Boskovic
 Maintainer-email: srdjan.boskovic@sap.com
 License: Apache License
         
         Version 2.0, January 2004
```

