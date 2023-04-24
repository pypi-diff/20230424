# Comparing `tmp/fwdviewpy-0.1.5.tar.gz` & `tmp/fwdviewpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.1.5.tar", last modified: Thu Apr 20 14:58:21 2023, max compression
+gzip compressed data, was "fwdviewpy-0.1.6.tar", last modified: Mon Apr 24 08:41:56 2023, max compression
```

## Comparing `fwdviewpy-0.1.5.tar` & `fwdviewpy-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 14:58:21.351387 fwdviewpy-0.1.5/
--rw-rw-rw-   0        0        0      623 2023-04-20 14:58:21.351387 fwdviewpy-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-20 14:58:21.286531 fwdviewpy-0.1.5/fwdviewpy/
--rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.5/fwdviewpy/__init__.py
--rw-rw-rw-   0        0        0    10707 2023-04-20 14:54:14.000000 fwdviewpy-0.1.5/fwdviewpy/main.py
-drwxrwxrwx   0        0        0        0 2023-04-20 14:58:21.344372 fwdviewpy-0.1.5/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      623 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 14:58:21.000000 fwdviewpy-0.1.5/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 14:58:21.359398 fwdviewpy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-04-18 14:43:43.000000 fwdviewpy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:41:56.203409 fwdviewpy-0.1.6/
+-rw-rw-rw-   0        0        0      620 2023-04-24 08:41:56.189909 fwdviewpy-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 08:41:56.156209 fwdviewpy-0.1.6/fwdviewpy/
+-rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.6/fwdviewpy/__init__.py
+-rw-rw-rw-   0        0        0    10707 2023-04-20 14:54:14.000000 fwdviewpy-0.1.6/fwdviewpy/main.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:41:56.189909 fwdviewpy-0.1.6/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:41:56.203409 fwdviewpy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-04-24 08:41:27.000000 fwdviewpy-0.1.6/setup.py
```

### Comparing `fwdviewpy-0.1.5/PKG-INFO` & `fwdviewpy-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 
-Python package developed by FWD View to aid automation of Delphix actions on both the Virtulaization and Continuous Compliance Delphix engines.
+Python package developed by FWD View to automate actions on both the Delphix Virtualization engine and Delphix Continuous Compliance engine.
```

### Comparing `fwdviewpy-0.1.5/fwdviewpy/main.py` & `fwdviewpy-0.1.6/fwdviewpy/main.py`

 * *Files identical despite different names*

### Comparing `fwdviewpy-0.1.5/fwdviewpy.egg-info/PKG-INFO` & `fwdviewpy-0.1.6/fwdviewpy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 
-Python package developed by FWD View to aid automation of Delphix actions on both the Virtulaization and Continuous Compliance Delphix engines.
+Python package developed by FWD View to automate actions on both the Delphix Virtualization engine and Delphix Continuous Compliance engine.
```

### Comparing `fwdviewpy-0.1.5/setup.py` & `fwdviewpy-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fwdviewpy',
-    version='0.1.5',
+    version='0.1.6',
     description='Python package developed by FWD View - The Data Transformation Specialists.',
-    long_description='Python package developed by FWD View to aid automation of Delphix actions on both the Virtulaization and Continuous Compliance Delphix engines.',
+    long_description='Python package developed by FWD View to automate actions on both the Delphix Virtualization engine and Delphix Continuous Compliance engine.',
     packages=find_packages(),
     author='Cameron Bose & Ryan Springett',
     author_email="cameron.bose@fwdview.com",
 
     install_requires=[
         'requests'
     ],
```

