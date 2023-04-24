# Comparing `tmp/rwthcolors-0.2.0.tar.gz` & `tmp/rwthcolors-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwthcolors-0.2.0.tar", max compression
+gzip compressed data, was "rwthcolors-0.2.1.tar", max compression
```

## Comparing `rwthcolors-0.2.0.tar` & `rwthcolors-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      735 2023-04-24 13:43:51.487688 rwthcolors-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.0/README.md
--rw-r--r--   0        0        0       30 2022-05-13 09:37:38.111913 rwthcolors-0.2.0/RWTHColors/__init__.py
--rw-r--r--   0        0        0     6381 2022-06-21 12:19:23.066702 rwthcolors-0.2.0/RWTHColors/cm.py
--rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.0/RWTHColors/colors/__init__.py
--rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.0/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.0/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0        0        0     5090 2022-02-01 15:18:59.876053 rwthcolors-0.2.0/RWTHColors/colors/colors.py
--rw-r--r--   0        0        0      584 2023-04-24 13:41:58.268837 rwthcolors-0.2.0/RWTHColors/rwth-full.mplstyle
--rw-r--r--   0        0        0      144 2023-04-24 13:41:05.383390 rwthcolors-0.2.0/RWTHColors/rwth.mplstyle
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 rwthcolors-0.2.0/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 rwthcolors-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      735 2023-04-24 14:38:25.794390 rwthcolors-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.1/README.md
+-rw-r--r--   0        0        0      933 2023-04-24 14:29:37.538409 rwthcolors-0.2.1/RWTHColors/__init__.py
+-rw-r--r--   0        0        0     6381 2022-06-21 12:19:23.066702 rwthcolors-0.2.1/RWTHColors/cm.py
+-rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.1/RWTHColors/colors/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.1/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.1/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0        0        0     5090 2022-02-01 15:18:59.876053 rwthcolors-0.2.1/RWTHColors/colors/colors.py
+-rw-r--r--   0        0        0      585 2023-04-24 13:56:29.944561 rwthcolors-0.2.1/RWTHColors/mpl-styles/rwth-full.mplstyle
+-rw-r--r--   0        0        0      149 2023-04-24 13:55:29.484164 rwthcolors-0.2.1/RWTHColors/mpl-styles/rwth.mplstyle
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 rwthcolors-0.2.1/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 rwthcolors-0.2.1/PKG-INFO
```

### Comparing `rwthcolors-0.2.0/pyproject.toml` & `rwthcolors-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RWTHColors"
-version = "0.2.0"
+version = "0.2.1"
 description = "Simple library that makes it easier to use RWTH CI colors in python projects"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 classifiers = [
     "Topic :: Scientific/Engineering :: Information Analysis",
```

### Comparing `rwthcolors-0.2.0/RWTHColors/cm.py` & `rwthcolors-0.2.1/RWTHColors/cm.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.0/RWTHColors/colors/__pycache__/colors.cpython-39.pyc` & `rwthcolors-0.2.1/RWTHColors/colors/__pycache__/colors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.0/RWTHColors/colors/colors.py` & `rwthcolors-0.2.1/RWTHColors/colors/colors.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.0/RWTHColors/rwth-full.mplstyle` & `rwthcolors-0.2.1/RWTHColors/mpl-styles/rwth-full.mplstyle`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-axes.prop_cycle : cycler(color=['#00549F', '#F6A800', '#57AB27', '#CC071E', '#612158', '#A11035', '#7A6FAC', '#006165', '#BDCD00', '#0098A1', '#407FB7', '#FABE50', '#8DC060', '#D85C41', '#834E75', '#B65256', '#9B91C1', '#2D7F83', '#D0D95C', '#00B1B7', '#8EBAE5', '#FDD48F', '#B8D698', '#E69679', '#A8859E', '#CD8B87', '#BCB5D7', '#7DA4A7', '#E0E69A', '#89CCCF', '#C7DDF2', '#FEEAC9', '#DDEBCE', '#F3CDBB', '#D2C0CD', '#E5C5C0', '#DEDAEB', '#BFD0D1', '#F0F3D0', '#CAE7E7', '#E8F1FA', '#FFF7EA', '#F2F7EC', '#FAEBE3', '#EDE5EA', '#F5E8E5', '#F2F0F7', '#E6ECEC', '#F9FAED', '#EBF6F6'])
+axes.prop_cycle : cycler('color', ['#00549F', '#F6A800', '#57AB27', '#CC071E', '#612158', '#A11035', '#7A6FAC', '#006165', '#BDCD00', '#0098A1', '#407FB7', '#FABE50', '#8DC060', '#D85C41', '#834E75', '#B65256', '#9B91C1', '#2D7F83', '#D0D95C', '#00B1B7', '#8EBAE5', '#FDD48F', '#B8D698', '#E69679', '#A8859E', '#CD8B87', '#BCB5D7', '#7DA4A7', '#E0E69A', '#89CCCF', '#C7DDF2', '#FEEAC9', '#DDEBCE', '#F3CDBB', '#D2C0CD', '#E5C5C0', '#DEDAEB', '#BFD0D1', '#F0F3D0', '#CAE7E7', '#E8F1FA', '#FFF7EA', '#F2F7EC', '#FAEBE3', '#EDE5EA', '#F5E8E5', '#F2F0F7', '#E6ECEC', '#F9FAED', '#EBF6F6'])
```

### Comparing `rwthcolors-0.2.0/setup.py` & `rwthcolors-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['rwthcolors', 'rwthcolors.colors']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'rwthcolors': ['mpl-styles/*']}
 
 install_requires = \
 ['cycler>=0.11.0,<0.12.0', 'matplotlib>=3.5.2,<4.0.0', 'pytest>=7.1.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'rwthcolors',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Simple library that makes it easier to use RWTH CI colors in python projects',
     'long_description': '',
     'author': 'Philipp Simon Leibner',
     'author_email': 'philipp.leibner@ifs.rwth-aachen.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rwthcolors-0.2.0/PKG-INFO` & `rwthcolors-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwthcolors
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple library that makes it easier to use RWTH CI colors in python projects
 License: Apache-2.0
 Keywords: rwth,aachen,rwth aachen,farbwelt
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Science/Research
```

