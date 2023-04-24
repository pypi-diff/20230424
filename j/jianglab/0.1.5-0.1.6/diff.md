# Comparing `tmp/jianglab-0.1.5.tar.gz` & `tmp/jianglab-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.1.5.tar", last modified: Thu Apr 13 14:25:13 2023, max compression
+gzip compressed data, was "jianglab-0.1.6.tar", last modified: Mon Apr 24 15:35:55 2023, max compression
```

## Comparing `jianglab-0.1.5.tar` & `jianglab-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 14:25:13.460523 jianglab-0.1.5/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 14:25:13.460180 jianglab-0.1.5/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      956 2023-04-13 14:16:26.000000 jianglab-0.1.5/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 14:25:13.457489 jianglab-0.1.5/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.5/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)     2340 2023-04-13 12:49:12.000000 jianglab-0.1.5/jianglab/common_functions.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-13 14:25:13.459634 jianglab-0.1.5/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-13 14:25:13.000000 jianglab-0.1.5/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-13 14:25:13.000000 jianglab-0.1.5/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-13 14:25:13.000000 jianglab-0.1.5/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       32 2023-04-13 14:25:13.000000 jianglab-0.1.5/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-13 14:25:13.000000 jianglab-0.1.5/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-13 14:25:13.460667 jianglab-0.1.5/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      771 2023-04-13 14:24:14.000000 jianglab-0.1.5/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 15:35:55.501066 jianglab-0.1.6/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 15:35:55.500741 jianglab-0.1.6/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.1.6/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 15:35:55.497844 jianglab-0.1.6/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.6/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     3517 2023-04-24 15:35:39.000000 jianglab-0.1.6/jianglab/common_functions.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 15:35:55.499974 jianglab-0.1.6/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       52 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-24 15:35:55.501194 jianglab-0.1.6/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      813 2023-04-24 15:35:49.000000 jianglab-0.1.6/setup.py
```

### Comparing `jianglab-0.1.5/PKG-INFO` & `jianglab-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.5/README.md` & `jianglab-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 conda install treelib
 
+** In your package's root directory, create a setup.py file. **
+
+
 
 1. Update your package version:
 In your `setup.py` file, increment the version number. For example, if the current version is `0.1`, you can update it to `0.1.1` or `0.2`:
 ```python
 setup(
     name="my-package",
     version="0.1.1",  # Increment the version number here
@@ -21,14 +24,17 @@
 
 Rebuild your package using the following command:
 ```bash
 python setup.py sdist bdist_wheel
 
 ```
 This command will create a new `dist` directory with the updated package files.
+dist, build and *.egg-info should be in root when created
+
+
 1. Upload the new version:
 Now you can upload the new version of your package to PyPI using twine:
 
 ```bash
 twine upload dist/*
 
 ```
```

### Comparing `jianglab-0.1.5/jianglab.egg-info/PKG-INFO` & `jianglab-0.1.6/jianglab.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.5/setup.py` & `jianglab-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
+        "McsPyDataTools",
+        "tqdm",
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

