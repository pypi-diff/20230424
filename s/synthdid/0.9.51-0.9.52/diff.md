# Comparing `tmp/synthdid-0.9.51.tar.gz` & `tmp/synthdid-0.9.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synthdid-0.9.51.tar", last modified: Mon Apr 24 17:17:59 2023, max compression
+gzip compressed data, was "dist\synthdid-0.9.52.tar", last modified: Mon Apr 24 17:24:33 2023, max compression
```

## Comparing `synthdid-0.9.51.tar` & `synthdid-0.9.52.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:17:59.324706 synthdid-0.9.51/
--rw-rw-rw-   0        0        0     8824 2023-04-24 17:17:59.324706 synthdid-0.9.51/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 17:17:59.324706 synthdid-0.9.51/setup.cfg
--rw-rw-rw-   0        0        0     1858 2023-04-24 17:17:05.000000 synthdid-0.9.51/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:17:59.309706 synthdid-0.9.51/synthdid/
--rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/get_data.py
--rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/placebo_simulations.py
--rw-rw-rw-   0        0        0     6066 2023-04-24 17:10:42.000000 synthdid-0.9.51/synthdid/plots.py
--rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/sdid.py
--rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/solver.py
--rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.51/synthdid/summary.py
--rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.51/synthdid/synthdid.py
--rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/utils.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.51/synthdid/vcov.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:17:59.323704 synthdid-0.9.51/synthdid.egg-info/
--rw-rw-rw-   0        0        0     8824 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      623 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 17:17:59.000000 synthdid-0.9.51/synthdid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:24:33.548229 synthdid-0.9.52/
+-rw-rw-rw-   0        0        0     8824 2023-04-24 17:24:33.547226 synthdid-0.9.52/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:24:33.548229 synthdid-0.9.52/setup.cfg
+-rw-rw-rw-   0        0        0     2009 2023-04-24 17:24:29.000000 synthdid-0.9.52/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:24:33.538225 synthdid-0.9.52/synthdid/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/get_data.py
+-rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/placebo_simulations.py
+-rw-rw-rw-   0        0        0     6066 2023-04-24 17:10:42.000000 synthdid-0.9.52/synthdid/plots.py
+-rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/sdid.py
+-rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/solver.py
+-rw-rw-rw-   0        0        0      410 2023-04-18 01:36:21.000000 synthdid-0.9.52/synthdid/summary.py
+-rw-rw-rw-   0        0        0      792 2023-04-18 01:32:26.000000 synthdid-0.9.52/synthdid/synthdid.py
+-rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/utils.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9.52/synthdid/vcov.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:24:33.547226 synthdid-0.9.52/synthdid.egg-info/
+-rw-rw-rw-   0        0        0     8824 2023-04-24 17:24:33.000000 synthdid-0.9.52/synthdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-24 17:24:33.000000 synthdid-0.9.52/synthdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:24:33.000000 synthdid-0.9.52/synthdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      623 2023-04-24 17:24:33.000000 synthdid-0.9.52/synthdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 17:24:33.000000 synthdid-0.9.52/synthdid.egg-info/top_level.txt
```

### Comparing `synthdid-0.9.51/PKG-INFO` & `synthdid-0.9.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthdid
-Version: 0.9.51
+Version: 0.9.52
 Summary: Synthdid
 Home-page: https://github.com/d2cml-ai/synthdid.py
 Author: D2CML Team, Alexander Quispe, Rodrigo  Grijalba, Jhon Flores, Franco Caceres
 License: MIT
 Keywords: causal-inference
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `synthdid-0.9.51/setup.py` & `synthdid-0.9.52/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from setuptools import setup, find_packages
 
-with open("./Readme.md", "r", encoding="utf-8") as f:
+
+import os
+
+from setuptools import setup
+
+
+here = os.path.abspath(os.path.dirname(__file__))
+_readme_path = os.path.join(here, "Readme.md")
+
+with open(_readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     dependency_links=[],
     install_requires=[
         "appdirs==1.4.3",
         "attrs==19.1.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -30,15 +39,15 @@
         "six==1.16.0",
         "statsmodels==0.13.5",
         "toml==0.10.0",
         "zipp==3.15.0",
     ],
     name="synthdid",
     author="D2CML Team, Alexander Quispe, Rodrigo  Grijalba, Jhon Flores, Franco Caceres",
-    version="0.9.51",
+    version="0.9.52",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="causal-inference",
     url="https://github.com/d2cml-ai/synthdid.py",
     license="MIT",
     description="Synthdid",
@@ -46,7 +55,8 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Scientific/Engineering",
     ],
 )
+
```

### Comparing `synthdid-0.9.51/synthdid/get_data.py` & `synthdid-0.9.52/synthdid/get_data.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/placebo_simulations.py` & `synthdid-0.9.52/synthdid/placebo_simulations.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/plots.py` & `synthdid-0.9.52/synthdid/plots.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/sdid.py` & `synthdid-0.9.52/synthdid/sdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/solver.py` & `synthdid-0.9.52/synthdid/solver.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/synthdid.py` & `synthdid-0.9.52/synthdid/synthdid.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/utils.py` & `synthdid-0.9.52/synthdid/utils.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid/vcov.py` & `synthdid-0.9.52/synthdid/vcov.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.9.51/synthdid.egg-info/PKG-INFO` & `synthdid-0.9.52/synthdid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthdid
-Version: 0.9.51
+Version: 0.9.52
 Summary: Synthdid
 Home-page: https://github.com/d2cml-ai/synthdid.py
 Author: D2CML Team, Alexander Quispe, Rodrigo  Grijalba, Jhon Flores, Franco Caceres
 License: MIT
 Keywords: causal-inference
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `synthdid-0.9.51/synthdid.egg-info/requires.txt` & `synthdid-0.9.52/synthdid.egg-info/requires.txt`

 * *Files identical despite different names*

