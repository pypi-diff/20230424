# Comparing `tmp/pmkoalas-0.0.1a0.tar.gz` & `tmp/pmkoalas-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmkoalas-0.0.1a0.tar", last modified: Mon Apr 24 04:20:45 2023, max compression
+gzip compressed data, was "pmkoalas-0.0.1a1.tar", last modified: Mon Apr 24 04:36:48 2023, max compression
```

## Comparing `pmkoalas-0.0.1a0.tar` & `pmkoalas-0.0.1a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 04:20:45.831719 pmkoalas-0.0.1a0/
--rw-rw-rw-   0        0        0     1094 2022-08-18 07:14:37.000000 pmkoalas-0.0.1a0/LICENSE
--rw-rw-rw-   0        0        0     3152 2023-04-24 04:20:45.830719 pmkoalas-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0     1222 2023-04-24 04:05:36.000000 pmkoalas-0.0.1a0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 04:20:45.804758 pmkoalas-0.0.1a0/pmkoalas/
--rw-rw-rw-   0        0        0       23 2023-04-24 04:16:47.000000 pmkoalas-0.0.1a0/pmkoalas/__init__.py
--rw-rw-rw-   0        0        0     2705 2022-10-25 06:44:44.000000 pmkoalas-0.0.1a0/pmkoalas/_logging.py
--rw-rw-rw-   0        0        0    11208 2023-04-24 04:07:53.000000 pmkoalas-0.0.1a0/pmkoalas/complex.py
--rw-rw-rw-   0        0        0    17693 2023-04-24 04:07:21.000000 pmkoalas-0.0.1a0/pmkoalas/directly.py
--rw-rw-rw-   0        0        0      706 2023-04-24 04:07:26.000000 pmkoalas-0.0.1a0/pmkoalas/dtlog.py
--rw-rw-rw-   0        0        0        0 2022-08-25 07:59:30.000000 pmkoalas-0.0.1a0/pmkoalas/eventlog.py
--rw-rw-rw-   0        0        0     9574 2023-04-24 04:07:29.000000 pmkoalas-0.0.1a0/pmkoalas/export.py
--rw-rw-rw-   0        0        0    10090 2023-04-24 04:07:33.000000 pmkoalas-0.0.1a0/pmkoalas/read.py
--rw-rw-rw-   0        0        0     9240 2023-04-24 04:07:36.000000 pmkoalas-0.0.1a0/pmkoalas/simple.py
--rw-rw-rw-   0        0        0        0 2022-08-25 07:59:30.000000 pmkoalas-0.0.1a0/pmkoalas/work.py
--rw-rw-rw-   0        0        0      192 2022-09-09 04:54:03.000000 pmkoalas-0.0.1a0/pmkoalas/xes.py
--rw-rw-rw-   0        0        0     5221 2023-04-17 23:44:09.000000 pmkoalas-0.0.1a0/pmkoalas/xes_export.py
-drwxrwxrwx   0        0        0        0 2023-04-24 04:20:45.812737 pmkoalas-0.0.1a0/pmkoalas.egg-info/
--rw-rw-rw-   0        0        0     3152 2023-04-24 04:20:45.000000 pmkoalas-0.0.1a0/pmkoalas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-04-24 04:20:45.000000 pmkoalas-0.0.1a0/pmkoalas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 04:20:45.000000 pmkoalas-0.0.1a0/pmkoalas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-24 04:20:45.000000 pmkoalas-0.0.1a0/pmkoalas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 04:20:45.000000 pmkoalas-0.0.1a0/pmkoalas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      911 2023-04-24 04:16:30.000000 pmkoalas-0.0.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 04:20:45.831719 pmkoalas-0.0.1a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 04:20:45.828694 pmkoalas-0.0.1a0/tests/
--rw-rw-rw-   0        0        0     7858 2023-04-24 04:06:41.000000 pmkoalas-0.0.1a0/tests/test_alpha.py
--rw-rw-rw-   0        0        0     3819 2023-04-24 04:06:44.000000 pmkoalas-0.0.1a0/tests/test_drelations.py
--rw-rw-rw-   0        0        0     1214 2023-04-24 04:06:46.000000 pmkoalas-0.0.1a0/tests/test_dtlog.py
--rw-rw-rw-   0        0        0     3260 2023-04-24 04:06:52.000000 pmkoalas-0.0.1a0/tests/test_export_complex.py
--rw-rw-rw-   0        0        0     2278 2023-04-24 04:06:54.000000 pmkoalas-0.0.1a0/tests/test_export_simple.py
--rw-rw-rw-   0        0        0     4079 2023-04-24 04:06:56.000000 pmkoalas-0.0.1a0/tests/test_read_complex.py
--rw-rw-rw-   0        0        0     1976 2023-04-24 04:07:00.000000 pmkoalas-0.0.1a0/tests/test_read_simple.py
--rw-rw-rw-   0        0        0     1577 2023-04-24 04:07:04.000000 pmkoalas-0.0.1a0/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:36:48.186837 pmkoalas-0.0.1a1/
+-rw-rw-rw-   0        0        0     1094 2022-08-18 07:14:37.000000 pmkoalas-0.0.1a1/LICENSE
+-rw-rw-rw-   0        0        0     3152 2023-04-24 04:36:48.185839 pmkoalas-0.0.1a1/PKG-INFO
+-rw-rw-rw-   0        0        0     1222 2023-04-24 04:23:20.000000 pmkoalas-0.0.1a1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 04:36:48.161904 pmkoalas-0.0.1a1/pmkoalas/
+-rw-rw-rw-   0        0        0       29 2023-04-24 04:35:43.000000 pmkoalas-0.0.1a1/pmkoalas/__init__.py
+-rw-rw-rw-   0        0        0     2705 2022-10-25 06:44:44.000000 pmkoalas-0.0.1a1/pmkoalas/_logging.py
+-rw-rw-rw-   0        0        0    11208 2023-04-24 04:07:53.000000 pmkoalas-0.0.1a1/pmkoalas/complex.py
+-rw-rw-rw-   0        0        0    17693 2023-04-24 04:07:21.000000 pmkoalas-0.0.1a1/pmkoalas/directly.py
+-rw-rw-rw-   0        0        0      706 2023-04-24 04:07:26.000000 pmkoalas-0.0.1a1/pmkoalas/dtlog.py
+-rw-rw-rw-   0        0        0        0 2022-08-25 07:59:30.000000 pmkoalas-0.0.1a1/pmkoalas/eventlog.py
+-rw-rw-rw-   0        0        0     9574 2023-04-24 04:07:29.000000 pmkoalas-0.0.1a1/pmkoalas/export.py
+-rw-rw-rw-   0        0        0    10090 2023-04-24 04:07:33.000000 pmkoalas-0.0.1a1/pmkoalas/read.py
+-rw-rw-rw-   0        0        0     9240 2023-04-24 04:07:36.000000 pmkoalas-0.0.1a1/pmkoalas/simple.py
+-rw-rw-rw-   0        0        0        0 2022-08-25 07:59:30.000000 pmkoalas-0.0.1a1/pmkoalas/work.py
+-rw-rw-rw-   0        0        0      192 2022-09-09 04:54:03.000000 pmkoalas-0.0.1a1/pmkoalas/xes.py
+-rw-rw-rw-   0        0        0     5221 2023-04-17 23:44:09.000000 pmkoalas-0.0.1a1/pmkoalas/xes_export.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:36:48.169883 pmkoalas-0.0.1a1/pmkoalas.egg-info/
+-rw-rw-rw-   0        0        0     3152 2023-04-24 04:36:48.000000 pmkoalas-0.0.1a1/pmkoalas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-04-24 04:36:48.000000 pmkoalas-0.0.1a1/pmkoalas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 04:36:48.000000 pmkoalas-0.0.1a1/pmkoalas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-24 04:36:48.000000 pmkoalas-0.0.1a1/pmkoalas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 04:36:48.000000 pmkoalas-0.0.1a1/pmkoalas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      917 2023-04-24 04:35:37.000000 pmkoalas-0.0.1a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 04:36:48.186837 pmkoalas-0.0.1a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 04:36:48.183844 pmkoalas-0.0.1a1/tests/
+-rw-rw-rw-   0        0        0     7858 2023-04-24 04:06:41.000000 pmkoalas-0.0.1a1/tests/test_alpha.py
+-rw-rw-rw-   0        0        0     3819 2023-04-24 04:06:44.000000 pmkoalas-0.0.1a1/tests/test_drelations.py
+-rw-rw-rw-   0        0        0     1214 2023-04-24 04:06:46.000000 pmkoalas-0.0.1a1/tests/test_dtlog.py
+-rw-rw-rw-   0        0        0     3260 2023-04-24 04:06:52.000000 pmkoalas-0.0.1a1/tests/test_export_complex.py
+-rw-rw-rw-   0        0        0     2278 2023-04-24 04:06:54.000000 pmkoalas-0.0.1a1/tests/test_export_simple.py
+-rw-rw-rw-   0        0        0     4079 2023-04-24 04:06:56.000000 pmkoalas-0.0.1a1/tests/test_read_complex.py
+-rw-rw-rw-   0        0        0     1976 2023-04-24 04:07:00.000000 pmkoalas-0.0.1a1/tests/test_read_simple.py
+-rw-rw-rw-   0        0        0     1577 2023-04-24 04:07:04.000000 pmkoalas-0.0.1a1/tests/test_simple.py
```

### Comparing `pmkoalas-0.0.1a0/LICENSE` & `pmkoalas-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/PKG-INFO` & `pmkoalas-0.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmkoalas
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A process mining library that focuses on providing pythonic interactions with event logs and languages.
 Author-email: Adam Banham <adam_banham@hotmail.com>, Adam Burke <adam_burke_mail@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 Adam Peter Banham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pmkoalas-0.0.1a0/README.md` & `pmkoalas-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/_logging.py` & `pmkoalas-0.0.1a1/pmkoalas/_logging.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/complex.py` & `pmkoalas-0.0.1a1/pmkoalas/complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/directly.py` & `pmkoalas-0.0.1a1/pmkoalas/directly.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/dtlog.py` & `pmkoalas-0.0.1a1/pmkoalas/dtlog.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/export.py` & `pmkoalas-0.0.1a1/pmkoalas/export.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/read.py` & `pmkoalas-0.0.1a1/pmkoalas/read.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/simple.py` & `pmkoalas-0.0.1a1/pmkoalas/simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas/xes_export.py` & `pmkoalas-0.0.1a1/pmkoalas/xes_export.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pmkoalas.egg-info/PKG-INFO` & `pmkoalas-0.0.1a1/pmkoalas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmkoalas
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A process mining library that focuses on providing pythonic interactions with event logs and languages.
 Author-email: Adam Banham <adam_banham@hotmail.com>, Adam Burke <adam_burke_mail@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 Adam Peter Banham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pmkoalas-0.0.1a0/pmkoalas.egg-info/SOURCES.txt` & `pmkoalas-0.0.1a1/pmkoalas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/pyproject.toml` & `pmkoalas-0.0.1a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmkoalas"
-version = "0.0.1.a"
+version = "0.0.1-alpha.1"
 authors = [
   { name="Adam Banham", email="adam_banham@hotmail.com" },
   { name="Adam Burke", email="adam_burke_mail@yahoo.com" },
 ]
 description = "A process mining library that focuses on providing pythonic interactions with event logs and languages."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `pmkoalas-0.0.1a0/tests/test_alpha.py` & `pmkoalas-0.0.1a1/tests/test_alpha.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_drelations.py` & `pmkoalas-0.0.1a1/tests/test_drelations.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_dtlog.py` & `pmkoalas-0.0.1a1/tests/test_dtlog.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_export_complex.py` & `pmkoalas-0.0.1a1/tests/test_export_complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_export_simple.py` & `pmkoalas-0.0.1a1/tests/test_export_simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_read_complex.py` & `pmkoalas-0.0.1a1/tests/test_read_complex.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_read_simple.py` & `pmkoalas-0.0.1a1/tests/test_read_simple.py`

 * *Files identical despite different names*

### Comparing `pmkoalas-0.0.1a0/tests/test_simple.py` & `pmkoalas-0.0.1a1/tests/test_simple.py`

 * *Files identical despite different names*

