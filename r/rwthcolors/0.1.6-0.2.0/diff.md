# Comparing `tmp/RWTHColors-0.1.6.tar.gz` & `tmp/rwthcolors-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWTHColors-0.1.6.tar", max compression
+gzip compressed data, was "rwthcolors-0.2.0.tar", max compression
```

## Comparing `RWTHColors-0.1.6.tar` & `rwthcolors-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0      735 2022-06-21 12:19:23.062701 RWTHColors-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 RWTHColors-0.1.6/README.md
--rw-r--r--   0        0        0       30 2022-05-13 09:37:38.111913 RWTHColors-0.1.6/RWTHColors/__init__.py
--rw-r--r--   0        0        0     6381 2022-06-21 12:19:23.066702 RWTHColors-0.1.6/RWTHColors/cm.py
--rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 RWTHColors-0.1.6/RWTHColors/colors/__init__.py
--rw-r--r--   0        0        0     5090 2022-02-01 15:18:59.876053 RWTHColors-0.1.6/RWTHColors/colors/colors.py
--rw-r--r--   0        0        0      762 2022-06-21 12:20:39.445639 RWTHColors-0.1.6/setup.py
--rw-r--r--   0        0        0      905 2022-06-21 12:20:39.445639 RWTHColors-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      735 2023-04-24 13:43:51.487688 rwthcolors-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.0/README.md
+-rw-r--r--   0        0        0       30 2022-05-13 09:37:38.111913 rwthcolors-0.2.0/RWTHColors/__init__.py
+-rw-r--r--   0        0        0     6381 2022-06-21 12:19:23.066702 rwthcolors-0.2.0/RWTHColors/cm.py
+-rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.0/RWTHColors/colors/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.0/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.0/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0        0        0     5090 2022-02-01 15:18:59.876053 rwthcolors-0.2.0/RWTHColors/colors/colors.py
+-rw-r--r--   0        0        0      584 2023-04-24 13:41:58.268837 rwthcolors-0.2.0/RWTHColors/rwth-full.mplstyle
+-rw-r--r--   0        0        0      144 2023-04-24 13:41:05.383390 rwthcolors-0.2.0/RWTHColors/rwth.mplstyle
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 rwthcolors-0.2.0/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 rwthcolors-0.2.0/PKG-INFO
```

### Comparing `RWTHColors-0.1.6/pyproject.toml` & `rwthcolors-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RWTHColors"
-version = "0.1.6"
+version = "0.2.0"
 description = "Simple library that makes it easier to use RWTH CI colors in python projects"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 classifiers = [
     "Topic :: Scientific/Engineering :: Information Analysis",
```

### Comparing `RWTHColors-0.1.6/RWTHColors/cm.py` & `rwthcolors-0.2.0/RWTHColors/cm.py`

 * *Files identical despite different names*

### Comparing `RWTHColors-0.1.6/RWTHColors/colors/colors.py` & `rwthcolors-0.2.0/RWTHColors/colors/colors.py`

 * *Files identical despite different names*

### Comparing `RWTHColors-0.1.6/setup.py` & `rwthcolors-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['cycler>=0.11.0,<0.12.0', 'matplotlib>=3.5.2,<4.0.0', 'pytest>=7.1.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'rwthcolors',
-    'version': '0.1.6',
+    'version': '0.2.0',
     'description': 'Simple library that makes it easier to use RWTH CI colors in python projects',
     'long_description': '',
     'author': 'Philipp Simon Leibner',
     'author_email': 'philipp.leibner@ifs.rwth-aachen.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `RWTHColors-0.1.6/PKG-INFO` & `rwthcolors-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rwthcolors
-Version: 0.1.6
+Version: 0.2.0
 Summary: Simple library that makes it easier to use RWTH CI colors in python projects
 License: Apache-2.0
 Keywords: rwth,aachen,rwth aachen,farbwelt
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: cycler (>=0.11.0,<0.12.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: pytest (>=7.1.1,<8.0.0)
 Description-Content-Type: text/markdown
```

