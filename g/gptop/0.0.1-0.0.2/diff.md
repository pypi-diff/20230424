# Comparing `tmp/gptop-0.0.1.tar.gz` & `tmp/gptop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptop-0.0.1.tar", last modified: Mon Apr 24 01:05:43 2023, max compression
+gzip compressed data, was "gptop-0.0.2.tar", last modified: Mon Apr 24 01:32:14 2023, max compression
```

## Comparing `gptop-0.0.1.tar` & `gptop-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:05:43.659536 gptop-0.0.1/
--rw-r--r--   0 nickcrews   (501) staff       (20)     1066 2023-04-21 22:10:41.000000 gptop-0.0.1/LICENSE
--rw-r--r--   0 nickcrews   (501) staff       (20)     2073 2023-04-24 01:05:43.659248 gptop-0.0.1/PKG-INFO
--rw-r--r--   0 nickcrews   (501) staff       (20)     1732 2023-04-22 16:38:46.000000 gptop-0.0.1/README.md
--rw-r--r--   0 nickcrews   (501) staff       (20)       38 2023-04-24 01:05:43.659618 gptop-0.0.1/setup.cfg
--rw-r--r--   0 nickcrews   (501) staff       (20)     1178 2023-04-24 01:05:26.000000 gptop-0.0.1/setup.py
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:05:43.655854 gptop-0.0.1/src/
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:05:43.655982 gptop-0.0.1/src/gptop/
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:05:43.658852 gptop-0.0.1/src/gptop/gptop.egg-info/
--rw-r--r--   0 nickcrews   (501) staff       (20)     2073 2023-04-24 01:05:43.000000 gptop-0.0.1/src/gptop/gptop.egg-info/PKG-INFO
--rw-r--r--   0 nickcrews   (501) staff       (20)      220 2023-04-24 01:05:43.000000 gptop-0.0.1/src/gptop/gptop.egg-info/SOURCES.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)        1 2023-04-24 01:05:43.000000 gptop-0.0.1/src/gptop/gptop.egg-info/dependency_links.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)      277 2023-04-24 01:05:43.000000 gptop-0.0.1/src/gptop/gptop.egg-info/requires.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)        1 2023-04-24 01:05:43.000000 gptop-0.0.1/src/gptop/gptop.egg-info/top_level.txt
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:32:14.070700 gptop-0.0.2/
+-rw-r--r--   0 nickcrews   (501) staff       (20)     1066 2023-04-21 22:10:41.000000 gptop-0.0.2/LICENSE
+-rw-r--r--   0 nickcrews   (501) staff       (20)     2073 2023-04-24 01:32:14.070392 gptop-0.0.2/PKG-INFO
+-rw-r--r--   0 nickcrews   (501) staff       (20)     1732 2023-04-22 16:38:46.000000 gptop-0.0.2/README.md
+-rw-r--r--   0 nickcrews   (501) staff       (20)       38 2023-04-24 01:32:14.070793 gptop-0.0.2/setup.cfg
+-rw-r--r--   0 nickcrews   (501) staff       (20)     1308 2023-04-24 01:31:30.000000 gptop-0.0.2/setup.py
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:32:14.063867 gptop-0.0.2/src/
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:32:14.068325 gptop-0.0.2/src/gptop/
+-rw-r--r--   0 nickcrews   (501) staff       (20)      286 2023-04-23 22:25:39.000000 gptop-0.0.2/src/gptop/__init__.py
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 01:32:14.069954 gptop-0.0.2/src/gptop/gptop.egg-info/
+-rw-r--r--   0 nickcrews   (501) staff       (20)     2073 2023-04-24 01:32:14.000000 gptop-0.0.2/src/gptop/gptop.egg-info/PKG-INFO
+-rw-r--r--   0 nickcrews   (501) staff       (20)      335 2023-04-24 01:32:14.000000 gptop-0.0.2/src/gptop/gptop.egg-info/SOURCES.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)        1 2023-04-24 01:32:14.000000 gptop-0.0.2/src/gptop/gptop.egg-info/dependency_links.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)      277 2023-04-24 01:32:14.000000 gptop-0.0.2/src/gptop/gptop.egg-info/requires.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)       50 2023-04-24 01:32:14.000000 gptop-0.0.2/src/gptop/gptop.egg-info/top_level.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)     3779 2023-04-23 21:47:39.000000 gptop-0.0.2/src/gptop/operation.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)     4318 2023-04-23 22:08:45.000000 gptop-0.0.2/src/gptop/operation_utils.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)     5060 2023-04-23 21:10:02.000000 gptop-0.0.2/src/gptop/operator.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)      459 2023-04-23 21:06:19.000000 gptop-0.0.2/src/gptop/utils.py
```

### Comparing `gptop-0.0.1/LICENSE` & `gptop-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptop-0.0.1/PKG-INFO` & `gptop-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptop
-Version: 0.0.1
+Version: 0.0.2
 Summary: Handles communication with GPTs
 Author: Nick Crews
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `gptop-0.0.1/README.md` & `gptop-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gptop-0.0.1/setup.py` & `gptop-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gptop",
-    version="0.0.1",
+    version="0.0.2",
     author="Nick Crews",
     description="Handles communication with GPTs",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages('src/gptop'),
+    packages=setuptools.find_packages('./src/gptop'),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    py_modules=[
+        "__init__",
+        "operation_utils",
+        "operation",
+        "operator",
+        "utils"
+    ],
     package_dir={'': 'src/gptop'},
     python_requires='>=3.6',
     include_package_data=True,
     install_requires=[
         "requests >= 2.20",
         "scikit-learn >= 1.0.2",
         "tenacity >= 8.0.1",
```

### Comparing `gptop-0.0.1/src/gptop/gptop.egg-info/PKG-INFO` & `gptop-0.0.2/src/gptop/gptop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptop
-Version: 0.0.1
+Version: 0.0.2
 Summary: Handles communication with GPTs
 Author: Nick Crews
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

