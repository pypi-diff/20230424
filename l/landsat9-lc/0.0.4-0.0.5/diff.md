# Comparing `tmp/landsat9_lc-0.0.4.tar.gz` & `tmp/landsat9_lc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\landsat9_lc-0.0.4.tar", last modified: Sun Apr 23 20:57:32 2023, max compression
+gzip compressed data, was "dist\landsat9_lc-0.0.5.tar", last modified: Sun Apr 23 23:25:51 2023, max compression
```

## Comparing `landsat9_lc-0.0.4.tar` & `landsat9_lc-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/
--rw-rw-rw-   0        0        0      176 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      127 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1422 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-04-22 16:46:50.000000 landsat9_lc-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc/
--rw-rw-rw-   0        0        0       52 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/__init__.py
--rw-rw-rw-   0        0        0     3356 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/l9_lc_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/
--rw-rw-rw-   0        0        0       38 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1782 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/model_pipeline.py
--rw-rw-rw-   0        0        0     2366 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/pipeline/spyndex_transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc/processing/
--rw-rw-rw-   0        0        0       22 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/processing/__init__.py
--rw-rw-rw-   0        0        0     2113 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/processing/data_manager.py
--rw-rw-rw-   0        0        0     9008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/processing/utils.py
--rw-rw-rw-   0        0        0     1008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/landsat9_lc/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/
--rw-rw-rw-   0        0        0     1422 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      266 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-22 17:23:39.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      266 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 20:57:31.000000 landsat9_lc-0.0.4/landsat9_lc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      593 2023-04-23 20:57:20.000000 landsat9_lc-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      279 2023-04-22 16:46:51.000000 landsat9_lc-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0      482 2023-04-23 20:57:32.000000 landsat9_lc-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2206 2023-04-23 20:57:20.000000 landsat9_lc-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/
+-rw-rw-rw-   0        0        0      176 2023-04-22 16:46:50.000000 landsat9_lc-0.0.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2023-04-22 16:46:50.000000 landsat9_lc-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-23 23:17:32.000000 landsat9_lc-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1334 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2023-04-22 16:46:50.000000 landsat9_lc-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc/
+-rw-rw-rw-   0        0        0       52 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/__init__.py
+-rw-rw-rw-   0        0        0     3356 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/l9_lc_classifier.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/
+-rw-rw-rw-   0        0        0       38 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/__init__.py
+-rw-rw-rw-   0        0        0     1782 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/model_pipeline.py
+-rw-rw-rw-   0        0        0     2366 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/pipeline/spyndex_transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/
+-rw-rw-rw-   0        0        0       22 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/__init__.py
+-rw-rw-rw-   0        0        0     2113 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/data_manager.py
+-rw-rw-rw-   0        0        0     9008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/processing/utils.py
+-rw-rw-rw-   0        0        0     1008 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/landsat9_lc/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/
+-rw-rw-rw-   0        0        0     1334 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      266 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-22 17:23:39.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      266 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-23 23:25:50.000000 landsat9_lc-0.0.5/landsat9_lc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      279 2023-04-22 16:46:51.000000 landsat9_lc-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0      482 2023-04-23 23:25:51.000000 landsat9_lc-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2206 2023-04-23 23:25:45.000000 landsat9_lc-0.0.5/setup.py
```

### Comparing `landsat9_lc-0.0.4/LICENSE` & `landsat9_lc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/PKG-INFO` & `landsat9_lc-0.0.5/landsat9_lc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: landsat9_lc
-Version: 0.0.4
-Summary: A python ML model to classify landsat 9 images
+Name: landsat9-lc
+Version: 0.0.5
+Summary: A Short description
 Home-page: https://github.com/hectorpatino/landsat9_lc
 Author: Hector Patino
-Author-email: Hector Patiño <hectorpatino24@gmail.com>
+Author-email: hectorpatino24@gmail.com
 License: MIT license
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: landsat9_lc
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # landsat9_lc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `landsat9_lc-0.0.4/README.md` & `landsat9_lc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc/l9_lc_classifier.py` & `landsat9_lc-0.0.5/landsat9_lc/l9_lc_classifier.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc/pipeline/model_pipeline.py` & `landsat9_lc-0.0.5/landsat9_lc/pipeline/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc/pipeline/spyndex_transformer.py` & `landsat9_lc-0.0.5/landsat9_lc/pipeline/spyndex_transformer.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc/processing/data_manager.py` & `landsat9_lc-0.0.5/landsat9_lc/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc/processing/utils.py` & `landsat9_lc-0.0.5/landsat9_lc/processing/utils.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc/train_pipeline.py` & `landsat9_lc-0.0.5/landsat9_lc/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `landsat9_lc-0.0.4/landsat9_lc.egg-info/PKG-INFO` & `landsat9_lc-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: landsat9-lc
-Version: 0.0.4
-Summary: A python ML model to classify landsat 9 images
+Name: landsat9_lc
+Version: 0.0.5
+Summary: A Short description
 Home-page: https://github.com/hectorpatino/landsat9_lc
 Author: Hector Patino
-Author-email: Hector Patiño <hectorpatino24@gmail.com>
+Author-email: hectorpatino24@gmail.com
 License: MIT license
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: landsat9_lc
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # landsat9_lc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `landsat9_lc-0.0.4/landsat9_lc.egg-info/SOURCES.txt` & `landsat9_lc-0.0.5/landsat9_lc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 AUTHORS.rst
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 landsat9_lc/__init__.py
 landsat9_lc/l9_lc_classifier.py
 landsat9_lc/train_pipeline.py
 landsat9_lc.egg-info/PKG-INFO
```

### Comparing `landsat9_lc-0.0.4/setup.py` & `landsat9_lc-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,10 +65,10 @@
     keywords='landsat9_lc',
     name='landsat9_lc',
     packages=find_packages(include=['landsat9_lc', 'landsat9_lc.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/hectorpatino/landsat9_lc',
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

