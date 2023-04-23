# Comparing `tmp/prepipy-0.6.1.tar.gz` & `tmp/prepipy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepipy-0.6.1.tar", max compression
+gzip compressed data, was "prepipy-0.6.2.tar", max compression
```

## Comparing `prepipy-0.6.1.tar` & `prepipy-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.1/LICENSE
--rw-r--r--   0        0        0     1104 2023-04-23 23:15:18.096830 prepipy-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2049 2023-03-19 20:16:59.384002 prepipy-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.1/src/prepipy/__init__.py
--rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.1/src/prepipy/auxiliaries.py
--rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.1/src/prepipy/config/config_comments.yml
--rw-r--r--   0        0        0      859 2023-03-31 20:54:09.462366 prepipy-0.6.1/src/prepipy/config/logging_config.yml
--rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.1/src/prepipy/config/masking_example.yml
--rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.1/src/prepipy/config_file_examples/bands.yml
--rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.1/src/prepipy/config_file_examples/config_single.yml
--rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.1/src/prepipy/config_file_examples/mask.yml
--rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.1/src/prepipy/configuration.py
--rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.1/src/prepipy/framework.py
--rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.1/src/prepipy/framework_sources.py
--rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.1/src/prepipy/masking.py
--rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.1/src/prepipy/resources/grey_values.yml
--rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.1/src/prepipy/resources/html_templates.yml
--rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.1/src/prepipy/resources/stiff_params.yml
--rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.1/src/prepipy/rgbcombo.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 prepipy-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1104 2023-04-23 23:25:03.376984 prepipy-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2049 2023-03-19 20:16:59.384002 prepipy-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.2/src/prepipy/__init__.py
+-rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.2/src/prepipy/auxiliaries.py
+-rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.2/src/prepipy/config/config_comments.yml
+-rw-r--r--   0        0        0      861 2023-04-23 23:24:40.005896 prepipy-0.6.2/src/prepipy/config/logging_config.yml
+-rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.2/src/prepipy/config/masking_example.yml
+-rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.2/src/prepipy/config_file_examples/bands.yml
+-rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.2/src/prepipy/config_file_examples/config_single.yml
+-rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.2/src/prepipy/config_file_examples/mask.yml
+-rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.2/src/prepipy/configuration.py
+-rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.2/src/prepipy/framework.py
+-rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.2/src/prepipy/framework_sources.py
+-rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.2/src/prepipy/masking.py
+-rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.2/src/prepipy/resources/grey_values.yml
+-rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.2/src/prepipy/resources/html_templates.yml
+-rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.2/src/prepipy/resources/stiff_params.yml
+-rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.2/src/prepipy/rgbcombo.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 prepipy-0.6.2/PKG-INFO
```

### Comparing `prepipy-0.6.1/LICENSE` & `prepipy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/pyproject.toml` & `prepipy-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prepipy"
-version = "0.6.1"
+version = "0.6.2"
 description = "Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images."
 authors = ["Fabian Haberhauer <fabian.haberhauer@univie.ac.at>"]
 maintainers = ["teutoburg <ghost@instruct.at>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/teutoburg/prepipy"
 classifiers = [
```

### Comparing `prepipy-0.6.1/README.md` & `prepipy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/auxiliaries.py` & `prepipy-0.6.2/src/prepipy/auxiliaries.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/config/config_comments.yml` & `prepipy-0.6.2/src/prepipy/config/config_comments.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/config/logging_config.yml` & `prepipy-0.6.2/src/prepipy/config/logging_config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,12 +32,12 @@
   simple:
     format: '%(module)s - %(levelname)-8s - %(message)s'
   datetime:
     format: '%(asctime)s - %(name)s - %(module)s - %(levelname)-8s - %(message)s'
   script:
     format: '%(message)s'
   color:
-    '()': rgbcombo.ColoredFormatter
+    '()': ..rgbcombo.ColoredFormatter
 
 root:
   level: INFO
   handlers: [file]
```

### Comparing `prepipy-0.6.1/src/prepipy/config/masking_example.yml` & `prepipy-0.6.2/src/prepipy/config/masking_example.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/config_file_examples/bands.yml` & `prepipy-0.6.2/src/prepipy/config_file_examples/bands.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/config_file_examples/config_single.yml` & `prepipy-0.6.2/src/prepipy/config_file_examples/config_single.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/configuration.py` & `prepipy-0.6.2/src/prepipy/configuration.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/framework.py` & `prepipy-0.6.2/src/prepipy/framework.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/framework_sources.py` & `prepipy-0.6.2/src/prepipy/framework_sources.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/masking.py` & `prepipy-0.6.2/src/prepipy/masking.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/resources/html_templates.yml` & `prepipy-0.6.2/src/prepipy/resources/html_templates.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/src/prepipy/rgbcombo.py` & `prepipy-0.6.2/src/prepipy/rgbcombo.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.1/PKG-INFO` & `prepipy-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepipy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images.
 Home-page: https://github.com/teutoburg/prepipy
 License: GPL-3.0-or-later
 Author: Fabian Haberhauer
 Author-email: fabian.haberhauer@univie.ac.at
 Maintainer: teutoburg
 Maintainer-email: ghost@instruct.at
```

