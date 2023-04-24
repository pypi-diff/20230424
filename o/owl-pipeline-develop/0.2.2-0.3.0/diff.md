# Comparing `tmp/owl-pipeline-develop-0.2.2.tar.gz` & `tmp/owl-pipeline-develop-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/owl-pipeline-develop/owl-pipeline-develop/dist/tmppnso5t52/owl-pipeline-develop-0.2.2.tar", last modified: Fri Aug 27 16:26:05 2021, max compression
+gzip compressed data, was "owl-pipeline-develop-0.3.0.tar", last modified: Mon Apr 24 07:58:35 2023, max compression
```

## Comparing `owl-pipeline-develop-0.2.2.tar` & `owl-pipeline-develop-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (116)      278 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      934 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      160 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_dev/
--rw-r--r--   0 runner    (1001) docker     (116)     2641 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/owl_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_dev/database/
--rw-r--r--   0 runner    (1001) docker     (116)      827 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/owl_dev/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      371 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/owl_dev/database/model.py
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/owl_dev/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      934 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      414 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       34 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       34 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      651 2021-08-27 16:26:05.000000 owl-pipeline-develop-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     1420 2021-08-27 16:25:55.000000 owl-pipeline-develop-0.2.2/setup.py
+drwxr-xr-x   0 eglez      (501) staff       (20)        0 2023-04-24 07:58:35.767611 owl-pipeline-develop-0.3.0/
+-rw-r--r--   0 eglez      (501) staff       (20)      278 2021-08-26 21:26:32.000000 owl-pipeline-develop-0.3.0/MANIFEST.in
+-rw-r--r--   0 eglez      (501) staff       (20)      914 2023-04-24 07:58:35.767694 owl-pipeline-develop-0.3.0/PKG-INFO
+-rw-r--r--   0 eglez      (501) staff       (20)      160 2021-08-27 11:56:32.000000 owl-pipeline-develop-0.3.0/README.rst
+drwxr-xr-x   0 eglez      (501) staff       (20)        0 2023-04-24 07:58:35.760805 owl-pipeline-develop-0.3.0/owl_dev/
+-rw-r--r--   0 eglez      (501) staff       (20)     2641 2023-04-23 04:43:40.000000 owl-pipeline-develop-0.3.0/owl_dev/__init__.py
+drwxr-xr-x   0 eglez      (501) staff       (20)        0 2023-04-24 07:58:35.761587 owl-pipeline-develop-0.3.0/owl_dev/database/
+-rw-r--r--   0 eglez      (501) staff       (20)      827 2021-08-26 21:26:32.000000 owl-pipeline-develop-0.3.0/owl_dev/database/__init__.py
+-rw-r--r--   0 eglez      (501) staff       (20)      371 2021-08-26 21:26:32.000000 owl-pipeline-develop-0.3.0/owl_dev/database/model.py
+-rw-r--r--   0 eglez      (501) staff       (20)       60 2023-04-23 04:42:25.000000 owl-pipeline-develop-0.3.0/owl_dev/logging.py
+drwxr-xr-x   0 eglez      (501) staff       (20)        0 2023-04-24 07:58:35.767180 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/
+-rw-r--r--   0 eglez      (501) staff       (20)      914 2023-04-24 07:58:35.000000 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/PKG-INFO
+-rw-r--r--   0 eglez      (501) staff       (20)      435 2023-04-24 07:58:35.000000 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 eglez      (501) staff       (20)        1 2023-04-24 07:58:35.000000 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/dependency_links.txt
+-rw-r--r--   0 eglez      (501) staff       (20)        1 2021-08-27 10:47:41.000000 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/not-zip-safe
+-rw-r--r--   0 eglez      (501) staff       (20)       34 2023-04-24 07:58:35.000000 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/requires.txt
+-rw-r--r--   0 eglez      (501) staff       (20)        8 2023-04-24 07:58:35.000000 owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/top_level.txt
+-rw-r--r--   0 eglez      (501) staff       (20)       34 2021-08-27 16:22:05.000000 owl-pipeline-develop-0.3.0/requirements.txt
+-rw-r--r--   0 eglez      (501) staff       (20)      651 2023-04-24 07:58:35.768135 owl-pipeline-develop-0.3.0/setup.cfg
+-rwxr--r--   0 eglez      (501) staff       (20)     1420 2023-04-23 04:43:40.000000 owl-pipeline-develop-0.3.0/setup.py
+drwxr-xr-x   0 eglez      (501) staff       (20)        0 2023-04-24 07:58:35.767438 owl-pipeline-develop-0.3.0/tests/
+-rw-r--r--   0 eglez      (501) staff       (20)      104 2021-08-26 21:26:32.000000 owl-pipeline-develop-0.3.0/tests/test_import.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `owl-pipeline-develop-0.2.2/PKG-INFO` & `owl-pipeline-develop-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: owl-pipeline-develop
-Version: 0.2.2
+Version: 0.3.0
 Summary: Pipeline Framework
 Home-page: https://github.com/IMAXT/owl-pipeline-develop
+Download-URL: https://github.com/IMAXT/owl-pipeline-develop/archive/v0.1.20.tar.gz
 Author: Eduardo Gonzalez Solares
 Author-email: eglez@ast.cam.ac.uk
 License: GNU General Public License v3
-Download-URL: https://github.com/IMAXT/owl-pipeline-develop/archive/v0.1.20.tar.gz
 Keywords: owl,pipeline
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3
 
 Owl Pipeline Developer Library
 ==============================
 
 This is the library used to develop
 `Owl Pipelines <https://eddienko.github.io/owl-pipeline>`__.
-
-
```

### Comparing `owl-pipeline-develop-0.2.2/owl_dev/__init__.py` & `owl-pipeline-develop-0.3.0/owl_dev/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from toolz import curry
 
 from owl_dev import database as db
 
 __author__ = "Eduardo Gonzalez Solares"
 __email__ = "eglez@ast.cam.ac.uk"
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 
 OWL_SUCCESS = "OWL_SUCCESS"
 OWL_ERROR = "OWL_ERROR"
 
 SQLITEDB = "sqlite.db"
```

### Comparing `owl-pipeline-develop-0.2.2/owl_dev/database/__init__.py` & `owl-pipeline-develop-0.3.0/owl_dev/database/__init__.py`

 * *Files identical despite different names*

### Comparing `owl-pipeline-develop-0.2.2/owl_pipeline_develop.egg-info/PKG-INFO` & `owl-pipeline-develop-0.3.0/owl_pipeline_develop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: owl-pipeline-develop
-Version: 0.2.2
+Version: 0.3.0
 Summary: Pipeline Framework
 Home-page: https://github.com/IMAXT/owl-pipeline-develop
+Download-URL: https://github.com/IMAXT/owl-pipeline-develop/archive/v0.1.20.tar.gz
 Author: Eduardo Gonzalez Solares
 Author-email: eglez@ast.cam.ac.uk
 License: GNU General Public License v3
-Download-URL: https://github.com/IMAXT/owl-pipeline-develop/archive/v0.1.20.tar.gz
 Keywords: owl,pipeline
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3
 
 Owl Pipeline Developer Library
 ==============================
 
 This is the library used to develop
 `Owl Pipelines <https://eddienko.github.io/owl-pipeline>`__.
-
-
```

### Comparing `owl-pipeline-develop-0.2.2/setup.cfg` & `owl-pipeline-develop-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.3.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = {current_version}
 replace = {new_version}
```

### Comparing `owl-pipeline-develop-0.2.2/setup.py` & `owl-pipeline-develop-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,11 +31,11 @@
     name="owl-pipeline-develop",
     packages=find_packages(include=["owl_dev*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/IMAXT/owl-pipeline-develop",
     download_url="https://github.com/IMAXT/owl-pipeline-develop/archive/v0.1.20.tar.gz",
-    version="0.2.2",
+    version="0.3.0",
     zip_safe=False,
     python_requires=">=3",
 )
```

