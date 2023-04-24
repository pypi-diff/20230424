# Comparing `tmp/simplification-0.6.6.tar.gz` & `tmp/simplification-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplification-0.6.6.tar", last modified: Tue Mar 21 14:07:21 2023, max compression
+gzip compressed data, was "simplification-0.6.7.tar", last modified: Fri Mar 24 13:20:54 2023, max compression
```

## Comparing `simplification-0.6.6.tar` & `simplification-0.6.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.904389 simplification-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-21 14:07:03.000000 simplification-0.6.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.896389 simplification-0.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.896389 simplification-0.6.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-21 14:07:03.000000 simplification-0.6.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-21 14:07:03.000000 simplification-0.6.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-21 14:07:03.000000 simplification-0.6.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.896389 simplification-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-03-21 14:07:03.000000 simplification-0.6.6/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-21 14:07:03.000000 simplification-0.6.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-21 14:07:21.904389 simplification-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-03-21 14:07:03.000000 simplification-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-21 14:07:03.000000 simplification-0.6.6/benchmark_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-21 14:07:03.000000 simplification-0.6.6/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-21 14:07:03.000000 simplification-0.6.6/manifest.in
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-21 14:07:03.000000 simplification-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 14:07:03.000000 simplification-0.6.6/rdp_p.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-21 14:07:03.000000 simplification-0.6.6/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-21 14:07:21.908389 simplification-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-21 14:07:03.000000 simplification-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.900389 simplification-0.6.6/simplification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:03.000000 simplification-0.6.6/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   896000 2023-03-21 14:07:20.000000 simplification-0.6.6/simplification/cutil.c
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-03-21 14:07:03.000000 simplification-0.6.6/simplification/cutil.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-03-21 14:07:03.000000 simplification-0.6.6/simplification/header.h
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 14:07:03.000000 simplification-0.6.6/simplification/rdp_p.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-21 14:07:03.000000 simplification-0.6.6/simplification/stdbool.h
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-03-21 14:07:03.000000 simplification-0.6.6/simplification/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.900389 simplification-0.6.6/simplification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-21 14:07:21.000000 simplification-0.6.6/simplification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-21 14:07:21.000000 simplification-0.6.6/simplification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:07:21.000000 simplification-0.6.6/simplification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:07:21.000000 simplification-0.6.6/simplification.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-21 14:07:21.000000 simplification-0.6.6/simplification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-21 14:07:21.000000 simplification-0.6.6/simplification.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:07:21.904389 simplification-0.6.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)    68527 2023-03-21 14:07:03.000000 simplification-0.6.6/test/coords.json
--rw-r--r--   0 runner    (1001) docker     (123)  5789046 2023-03-21 14:07:03.000000 simplification-0.6.6/test/coords_complex.json
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-21 14:07:03.000000 simplification-0.6.6/test/cprofile_rust_cython.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-21 14:07:03.000000 simplification-0.6.6/test/cprofile_rust_cython_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-21 14:07:03.000000 simplification-0.6.6/test/cprofile_rust_cython_shapely.py
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-03-21 14:07:03.000000 simplification-0.6.6/test/output_stats_rust_cython
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-21 14:07:03.000000 simplification-0.6.6/test/output_stats_rust_cython_complex
--rw-r--r--   0 runner    (1001) docker     (123)    64880 2023-03-21 14:07:03.000000 simplification-0.6.6/test/output_stats_rust_cython_shapely
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-21 14:07:03.000000 simplification-0.6.6/test/test_simplification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.573845 simplification-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-24 13:20:40.000000 simplification-0.6.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.553844 simplification-0.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.557844 simplification-0.6.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-24 13:20:40.000000 simplification-0.6.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 13:20:40.000000 simplification-0.6.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-24 13:20:40.000000 simplification-0.6.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.557844 simplification-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-03-24 13:20:40.000000 simplification-0.6.7/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-24 13:20:40.000000 simplification-0.6.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-24 13:20:54.573845 simplification-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-03-24 13:20:40.000000 simplification-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-24 13:20:40.000000 simplification-0.6.7/benchmark_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-24 13:20:40.000000 simplification-0.6.7/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-24 13:20:40.000000 simplification-0.6.7/manifest.in
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-24 13:20:40.000000 simplification-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-24 13:20:40.000000 simplification-0.6.7/rdp_p.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-24 13:20:40.000000 simplification-0.6.7/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-24 13:20:54.577845 simplification-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-24 13:20:40.000000 simplification-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.561844 simplification-0.6.7/simplification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:40.000000 simplification-0.6.7/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   896000 2023-03-24 13:20:53.000000 simplification-0.6.7/simplification/cutil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-03-24 13:20:40.000000 simplification-0.6.7/simplification/cutil.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-03-24 13:20:40.000000 simplification-0.6.7/simplification/header.h
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-24 13:20:40.000000 simplification-0.6.7/simplification/rdp_p.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 13:20:40.000000 simplification-0.6.7/simplification/stdbool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-03-24 13:20:40.000000 simplification-0.6.7/simplification/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.565844 simplification-0.6.7/simplification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-24 13:20:54.000000 simplification-0.6.7/simplification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-24 13:20:54.000000 simplification-0.6.7/simplification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 13:20:54.000000 simplification-0.6.7/simplification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 13:20:54.000000 simplification-0.6.7/simplification.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-24 13:20:54.000000 simplification-0.6.7/simplification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-24 13:20:54.000000 simplification-0.6.7/simplification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:20:54.573845 simplification-0.6.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    68527 2023-03-24 13:20:40.000000 simplification-0.6.7/test/coords.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5789046 2023-03-24 13:20:40.000000 simplification-0.6.7/test/coords_complex.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 13:20:40.000000 simplification-0.6.7/test/cprofile_rust_cython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-24 13:20:40.000000 simplification-0.6.7/test/cprofile_rust_cython_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-24 13:20:40.000000 simplification-0.6.7/test/cprofile_rust_cython_shapely.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-03-24 13:20:40.000000 simplification-0.6.7/test/output_stats_rust_cython
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-24 13:20:40.000000 simplification-0.6.7/test/output_stats_rust_cython_complex
+-rw-r--r--   0 runner    (1001) docker     (123)    64880 2023-03-24 13:20:40.000000 simplification-0.6.7/test/output_stats_rust_cython_shapely
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-24 13:20:40.000000 simplification-0.6.7/test/test_simplification.py
```

### Comparing `simplification-0.6.6/.github/ISSUE_TEMPLATE/bug_report.md` & `simplification-0.6.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/.github/workflows/wheels.yml` & `simplification-0.6.7/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/CITATION.cff` & `simplification-0.6.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/PKG-INFO` & `simplification-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplification
-Version: 0.6.6
+Version: 0.6.7
 Summary: Fast linestring simplification using RDP or Visvalingam-Whyatt and a Rust binary
 Home-page: https://github.com/urschrei/simplification
 Author: Stephan Hügel
 Author-email: urschrei@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/urschrei/simplification
 Project-URL: Tracker, https://github.com/urschrei/simplification/issues
```

### Comparing `simplification-0.6.6/README.md` & `simplification-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/benchmark_runner.py` & `simplification-0.6.7/benchmark_runner.py`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/license.txt` & `simplification-0.6.7/license.txt`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/rdp_p.pxd` & `simplification-0.6.7/rdp_p.pxd`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/release.py` & `simplification-0.6.7/release.py`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/setup.cfg` & `simplification-0.6.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/setup.py` & `simplification-0.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/simplification/cutil.c` & `simplification-0.6.7/simplification/cutil.c`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "extra_link_args": [
             "-Wl,-rpath",
             "-Wl,$ORIGIN"
         ],
         "include_dirs": [
             "./simplification",
             "simplification",
-            "/tmp/build-env-d6wrpyfe/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-upp5g_73/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "libraries": [
             "rdp"
         ],
         "library_dirs": [
             "simplification"
```

### Comparing `simplification-0.6.6/simplification/cutil.pyx` & `simplification-0.6.7/simplification/cutil.pyx`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/simplification/header.h` & `simplification-0.6.7/simplification/header.h`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/simplification/rdp_p.pxd` & `simplification-0.6.7/simplification/rdp_p.pxd`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/simplification/util.py` & `simplification-0.6.7/simplification/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 numpy_installed = True
 try:
     import numpy as np
 except ImportError:
     numpy_installed = False
 
 __author__ = "Stephan Hügel"
-__version__ = "0.6.6"
+__version__ = "0.6.7"
 
 file_path = os.path.dirname(__file__)
 
 prefix = {"win32": ""}.get(platform, "lib")
 extension = {"darwin": ".dylib", "win32": ".dll"}.get(platform, ".so")
 fpath = {"darwin": "", "win32": ""}.get(platform, os.path.join(file_path, ".libs"))
```

### Comparing `simplification-0.6.6/simplification.egg-info/PKG-INFO` & `simplification-0.6.7/simplification.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplification
-Version: 0.6.6
+Version: 0.6.7
 Summary: Fast linestring simplification using RDP or Visvalingam-Whyatt and a Rust binary
 Home-page: https://github.com/urschrei/simplification
 Author: Stephan Hügel
 Author-email: urschrei@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/urschrei/simplification
 Project-URL: Tracker, https://github.com/urschrei/simplification/issues
```

### Comparing `simplification-0.6.6/simplification.egg-info/SOURCES.txt` & `simplification-0.6.7/simplification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/test/coords.json` & `simplification-0.6.7/test/coords.json`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/test/coords_complex.json` & `simplification-0.6.7/test/coords_complex.json`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/test/output_stats_rust_cython` & `simplification-0.6.7/test/output_stats_rust_cython`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/test/output_stats_rust_cython_complex` & `simplification-0.6.7/test/output_stats_rust_cython_complex`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/test/output_stats_rust_cython_shapely` & `simplification-0.6.7/test/output_stats_rust_cython_shapely`

 * *Files identical despite different names*

### Comparing `simplification-0.6.6/test/test_simplification.py` & `simplification-0.6.7/test/test_simplification.py`

 * *Files identical despite different names*

