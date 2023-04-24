# Comparing `tmp/sara_compis1_tools-0.0.7.tar.gz` & `tmp/sara_compis1_tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.7.tar", last modified: Mon Apr 24 05:46:04 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.8.tar", last modified: Mon Apr 24 06:12:25 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.7.tar` & `sara_compis1_tools-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 05:46:04.363636 sara_compis1_tools-0.0.7/
--rw-rw-rw-   0        0        0      303 2023-04-24 05:36:05.000000 sara_compis1_tools-0.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      904 2023-04-24 05:46:04.358351 sara_compis1_tools-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 05:46:04.317601 sara_compis1_tools-0.0.7/sara_compis1_tools/
--rw-rw-rw-   0        0        0     4483 2023-04-24 01:35:25.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/AFD_tools.py
--rw-rw-rw-   0        0        0      155 2023-04-23 15:56:11.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Error.py
--rw-rw-rw-   0        0        0     6092 2023-04-24 03:38:02.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      263 2023-04-21 02:28:08.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0     1385 2023-04-23 04:32:41.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/Visualizer.py
--rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0     7598 2023-04-24 05:29:24.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/generated.py
--rw-rw-rw-   0        0        0    10130 2023-04-24 05:10:59.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/lexEval.py
--rw-rw-rw-   0        0        0    17009 2023-04-24 05:33:59.000000 sara_compis1_tools-0.0.7/sara_compis1_tools/lexGen.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:46:04.351861 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      904 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-04-24 05:46:04.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-24 05:46:03.000000 sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 05:46:04.363636 sara_compis1_tools-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-04-24 05:36:28.000000 sara_compis1_tools-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:12:25.935989 sara_compis1_tools-0.0.8/
+-rw-rw-rw-   0        0        0      357 2023-04-24 06:11:52.000000 sara_compis1_tools-0.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-04-24 06:12:25.930874 sara_compis1_tools-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/README.txt
+-rw-rw-rw-   0        0        0     1947 2023-04-24 06:02:26.000000 sara_compis1_tools-0.0.8/generated.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:12:25.881622 sara_compis1_tools-0.0.8/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     4483 2023-04-24 01:35:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/AFD_tools.py
+-rw-rw-rw-   0        0        0      155 2023-04-23 15:56:11.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Error.py
+-rw-rw-rw-   0        0        0     6092 2023-04-24 03:38:02.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      263 2023-04-21 02:28:08.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0     1385 2023-04-23 04:32:41.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/Visualizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0     7598 2023-04-24 06:11:03.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0    10130 2023-04-24 06:09:40.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/lexEval.py
+-rw-rw-rw-   0        0        0    17009 2023-04-24 06:09:16.000000 sara_compis1_tools-0.0.8/sara_compis1_tools/lexGen.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:12:25.923139 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-24 06:12:25.000000 sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:12:25.936429 sara_compis1_tools-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-04-24 06:12:07.000000 sara_compis1_tools-0.0.8/setup.py
```

### Comparing `sara_compis1_tools-0.0.7/LICENSE.txt` & `sara_compis1_tools-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/PKG-INFO` & `sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sara_compis1_tools
-Version: 0.0.7
+Name: sara-compis1-tools
+Version: 0.0.8
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -29,7 +29,11 @@
 0.0.6 (19/04/2023)
 ------------------
 - More fields for the StateAFD class.
 
 0.0.7 (23/04/2023)
 ------------------
 - Additions for AFN simulation.
+
+0.0.8 (24/04/2023)
+------------------
+- Fixes.
```

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/AFD_tools.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/AFD_tools.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/Format.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/Visualizer.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/Visualizer.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/directAFD.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/generated.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/generated.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/lexEval.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/lexEval.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools/lexGen.py` & `sara_compis1_tools-0.0.8/sara_compis1_tools/lexGen.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sara-compis1-tools
-Version: 0.0.7
+Name: sara_compis1_tools
+Version: 0.0.8
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -29,7 +29,11 @@
 0.0.6 (19/04/2023)
 ------------------
 - More fields for the StateAFD class.
 
 0.0.7 (23/04/2023)
 ------------------
 - Additions for AFN simulation.
+
+0.0.8 (24/04/2023)
+------------------
+- Fixes.
```

### Comparing `sara_compis1_tools-0.0.7/sara_compis1_tools.egg-info/SOURCES.txt` & `sara_compis1_tools-0.0.8/sara_compis1_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.txt
 LICENSE.txt
 MANIFEST.in
 README.txt
+generated.py
 setup.py
 sara_compis1_tools/AFD_tools.py
 sara_compis1_tools/Error.py
 sara_compis1_tools/Format.py
 sara_compis1_tools/StateAFD.py
 sara_compis1_tools/Syntax.py
 sara_compis1_tools/Visualizer.py
```

### Comparing `sara_compis1_tools-0.0.7/setup.py` & `sara_compis1_tools-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sara_compis1_tools',
-    version='0.0.7',
+    version='0.0.8',
     description='A collection of tools for the Language Design course',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/MGonza20/Compis_Lab4',
     author='Sara Paguaga',
     author_email='sara.paguaga@gmail.com',
     license='MIT',
     classifiers=[
```

