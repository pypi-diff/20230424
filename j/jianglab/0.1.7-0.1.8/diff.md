# Comparing `tmp/jianglab-0.1.7.tar.gz` & `tmp/jianglab-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.1.7.tar", last modified: Mon Apr 24 16:31:26 2023, max compression
+gzip compressed data, was "jianglab-0.1.8.tar", last modified: Mon Apr 24 20:50:46 2023, max compression
```

## Comparing `jianglab-0.1.7.tar` & `jianglab-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 16:31:26.507375 jianglab-0.1.7/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 16:31:26.507104 jianglab-0.1.7/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.1.7/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 16:31:26.504789 jianglab-0.1.7/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.7/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)     5590 2023-04-24 16:30:31.000000 jianglab-0.1.7/jianglab/common_functions.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 16:31:26.506640 jianglab-0.1.7/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       52 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-24 16:31:26.507530 jianglab-0.1.7/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      813 2023-04-24 16:30:47.000000 jianglab-0.1.7/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 20:50:46.906574 jianglab-0.1.8/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 20:50:46.906199 jianglab-0.1.8/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.1.8/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 20:50:46.903134 jianglab-0.1.8/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.8/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     9216 2023-04-24 20:50:22.000000 jianglab-0.1.8/jianglab/common_functions.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 20:50:46.905699 jianglab-0.1.8/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 20:50:46.000000 jianglab-0.1.8/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-24 20:50:46.000000 jianglab-0.1.8/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-24 20:50:46.000000 jianglab-0.1.8/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       58 2023-04-24 20:50:46.000000 jianglab-0.1.8/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-24 20:50:46.000000 jianglab-0.1.8/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-24 20:50:46.906705 jianglab-0.1.8/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      830 2023-04-24 20:50:39.000000 jianglab-0.1.8/setup.py
```

### Comparing `jianglab-0.1.7/PKG-INFO` & `jianglab-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.7/README.md` & `jianglab-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.1.7/jianglab.egg-info/PKG-INFO` & `jianglab-0.1.8/jianglab.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.1.7/setup.py` & `jianglab-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
         "tqdm",
+        "scipy",
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

