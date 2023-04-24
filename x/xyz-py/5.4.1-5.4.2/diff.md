# Comparing `tmp/xyz_py-5.4.1.tar.gz` & `tmp/xyz_py-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.4.1.tar", last modified: Mon Apr 24 09:41:24 2023, max compression
+gzip compressed data, was "xyz_py-5.4.2.tar", last modified: Mon Apr 24 13:21:47 2023, max compression
```

## Comparing `xyz_py-5.4.1.tar` & `xyz_py-5.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:41:24.752729 xyz_py-5.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-24 09:40:57.000000 xyz_py-5.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 09:41:24.750729 xyz_py-5.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-24 09:40:57.000000 xyz_py-5.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-24 09:40:57.000000 xyz_py-5.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 09:41:24.752729 xyz_py-5.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-24 09:41:20.000000 xyz_py-5.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:41:24.744729 xyz_py-5.4.1/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     9876 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 09:41:20.000000 xyz_py-5.4.1/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    37858 2023-04-24 09:40:57.000000 xyz_py-5.4.1/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:41:24.750729 xyz_py-5.4.1/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-24 09:41:24.000000 xyz_py-5.4.1/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:21:47.325545 xyz_py-5.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-04-24 13:21:19.000000 xyz_py-5.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 13:21:47.325545 xyz_py-5.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-24 13:21:19.000000 xyz_py-5.4.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-24 13:21:19.000000 xyz_py-5.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 13:21:47.325545 xyz_py-5.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-24 13:21:43.000000 xyz_py-5.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:21:47.320545 xyz_py-5.4.2/xyz_py/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7424 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9876 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 13:21:43.000000 xyz_py-5.4.2/xyz_py/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    37858 2023-04-24 13:21:19.000000 xyz_py-5.4.2/xyz_py/xyz_py.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:21:47.323545 xyz_py-5.4.2/xyz_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-24 13:21:47.000000 xyz_py-5.4.2/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.4.1/LICENSE` & `xyz_py-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.1/PKG-INFO` & `xyz_py-5.4.2/xyz_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.4.1
+Name: xyz-py
+Version: 5.4.2
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.4.1/README.md` & `xyz_py-5.4.2/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.1/setup.py` & `xyz_py-5.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.4.1"
+__version__ = "5.4.2"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.4.1/xyz_py/atomic.py` & `xyz_py-5.4.2/xyz_py/atomic.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 actinides = f_block_row_1
 
 f_block = f_block_row_1 + f_block_row_2
 
 metals = s_block + d_block + f_block
 metals += ["Al", "Ge", "Ga", "In", "Sn", "Tl", "Pb", "Bi", "Po"]
 
-non_metals = list(set(p_block).difference(metals))
+non_metals = list(set(p_block).difference(metals)) + ['H']
 
-elements = s_block + p_block + d_block + f_block
+elements = s_block + p_block + d_block + f_block + ['H']
 
 # Dictionary of relative atomic masses
 masses = {
     "H": 1.0076, "He": 4.0026, "Li": 6.941, "Be": 9.0122, "B": 10.811,
     "C": 12.0107, "N": 14.0067, "O": 15.9994, "F": 18.9984, "Ne": 20.1797,
     "Na": 22.9897, "Mg": 24.305, "Al": 26.9815, "Si": 28.0855, "P": 30.9738,
     "S": 32.065, "Cl": 35.453, "K": 39.0983, "Ar": 39.948, "Ca": 40.078,
```

### Comparing `xyz_py-5.4.1/xyz_py/cli.py` & `xyz_py-5.4.2/xyz_py/cli.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.1/xyz_py/xyz_py.py` & `xyz_py-5.4.2/xyz_py/xyz_py.py`

 * *Files identical despite different names*

### Comparing `xyz_py-5.4.1/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.4.1
+Name: xyz_py
+Version: 5.4.2
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

