# Comparing `tmp/app01-0.1.1.tar.gz` & `tmp/app01-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app01-0.1.1.tar", last modified: Sun Apr 23 10:17:25 2023, max compression
+gzip compressed data, was "app01-0.1.5.tar", last modified: Mon Apr 24 01:39:02 2023, max compression
```

## Comparing `app01-0.1.1.tar` & `app01-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-23 10:17:25.573532 app01-0.1.1/
--rw-r--r--   0 lihaijian   (501) staff       (20)      150 2023-04-23 06:59:22.000000 app01-0.1.1/AUTHORS.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)     3500 2023-04-23 06:59:22.000000 app01-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)       89 2023-04-23 06:59:22.000000 app01-0.1.1/HISTORY.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)     1068 2023-04-23 06:59:22.000000 app01-0.1.1/LICENSE
--rw-r--r--   0 lihaijian   (501) staff       (20)      262 2023-04-23 06:59:22.000000 app01-0.1.1/MANIFEST.in
--rw-r--r--   0 lihaijian   (501) staff       (20)     1559 2023-04-23 10:17:25.573716 app01-0.1.1/PKG-INFO
--rw-r--r--   0 lihaijian   (501) staff       (20)      812 2023-04-23 06:59:22.000000 app01-0.1.1/README.rst
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-23 10:17:25.562096 app01-0.1.1/app01/
--rw-r--r--   0 lihaijian   (501) staff       (20)      117 2023-04-23 06:59:22.000000 app01-0.1.1/app01/__init__.py
--rw-r--r--   0 lihaijian   (501) staff       (20)       19 2023-04-23 06:59:22.000000 app01-0.1.1/app01/app01.py
--rw-r--r--   0 lihaijian   (501) staff       (20)      576 2023-04-23 10:15:18.000000 app01-0.1.1/app01/cli.py
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-23 10:17:25.565752 app01-0.1.1/app01/matt/
--rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-23 09:15:37.000000 app01-0.1.1/app01/matt/__init__.py
--rw-r--r--   0 lihaijian   (501) staff       (20)      107 2023-04-23 10:14:45.000000 app01-0.1.1/app01/matt/math_add.py
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-23 10:17:25.565122 app01-0.1.1/app01.egg-info/
--rw-r--r--   0 lihaijian   (501) staff       (20)     1559 2023-04-23 10:17:25.000000 app01-0.1.1/app01.egg-info/PKG-INFO
--rw-r--r--   0 lihaijian   (501) staff       (20)      561 2023-04-23 10:17:25.000000 app01-0.1.1/app01.egg-info/SOURCES.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-23 10:17:25.000000 app01-0.1.1/app01.egg-info/dependency_links.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)       41 2023-04-23 10:17:25.000000 app01-0.1.1/app01.egg-info/entry_points.txt
--rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-23 07:37:05.000000 app01-0.1.1/app01.egg-info/not-zip-safe
--rw-r--r--   0 lihaijian   (501) staff       (20)        6 2023-04-23 10:17:25.000000 app01-0.1.1/app01.egg-info/top_level.txt
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-23 10:17:25.572039 app01-0.1.1/docs/
--rw-r--r--   0 lihaijian   (501) staff       (20)      606 2023-04-23 06:59:22.000000 app01-0.1.1/docs/Makefile
--rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.1/docs/authors.rst
--rwxr-xr-x   0 lihaijian   (501) staff       (20)     4743 2023-04-23 06:59:22.000000 app01-0.1.1/docs/conf.py
--rw-r--r--   0 lihaijian   (501) staff       (20)       33 2023-04-23 06:59:22.000000 app01-0.1.1/docs/contributing.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.1/docs/history.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)      302 2023-04-23 06:59:22.000000 app01-0.1.1/docs/index.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)     1098 2023-04-23 06:59:22.000000 app01-0.1.1/docs/installation.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)      803 2023-04-23 06:59:22.000000 app01-0.1.1/docs/make.bat
--rw-r--r--   0 lihaijian   (501) staff       (20)       27 2023-04-23 06:59:22.000000 app01-0.1.1/docs/readme.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)       65 2023-04-23 06:59:22.000000 app01-0.1.1/docs/usage.rst
--rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-23 10:17:25.574576 app01-0.1.1/setup.cfg
--rw-r--r--   0 lihaijian   (501) staff       (20)     1307 2023-04-23 10:17:08.000000 app01-0.1.1/setup.py
-drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-23 10:17:25.573115 app01-0.1.1/tests/
--rw-r--r--   0 lihaijian   (501) staff       (20)       35 2023-04-23 06:59:22.000000 app01-0.1.1/tests/__init__.py
--rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-23 06:59:22.000000 app01-0.1.1/tests/test_app01.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.419999 app01-0.1.5/
+-rw-r--r--   0 lihaijian   (501) staff       (20)      150 2023-04-23 06:59:22.000000 app01-0.1.5/AUTHORS.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)     3500 2023-04-23 06:59:22.000000 app01-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)       89 2023-04-23 06:59:22.000000 app01-0.1.5/HISTORY.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1068 2023-04-23 06:59:22.000000 app01-0.1.5/LICENSE
+-rw-r--r--   0 lihaijian   (501) staff       (20)      262 2023-04-23 06:59:22.000000 app01-0.1.5/MANIFEST.in
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1559 2023-04-24 01:39:02.420289 app01-0.1.5/PKG-INFO
+-rw-r--r--   0 lihaijian   (501) staff       (20)      812 2023-04-23 06:59:22.000000 app01-0.1.5/README.rst
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.406324 app01-0.1.5/app01/
+-rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-23 12:21:07.000000 app01-0.1.5/app01/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)       19 2023-04-23 06:59:22.000000 app01-0.1.5/app01/app01.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)      582 2023-04-23 12:23:26.000000 app01-0.1.5/app01/cli.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.412025 app01-0.1.5/app01/matt/
+-rw-r--r--   0 lihaijian   (501) staff       (20)        0 2023-04-23 09:15:37.000000 app01-0.1.5/app01/matt/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)       96 2023-04-23 12:18:06.000000 app01-0.1.5/app01/matt/math_add.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.410813 app01-0.1.5/app01.egg-info/
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1559 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/PKG-INFO
+-rw-r--r--   0 lihaijian   (501) staff       (20)      589 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/SOURCES.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/dependency_links.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)       41 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/entry_points.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)        1 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/not-zip-safe
+-rw-r--r--   0 lihaijian   (501) staff       (20)        4 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/requires.txt
+-rw-r--r--   0 lihaijian   (501) staff       (20)        6 2023-04-24 01:39:02.000000 app01-0.1.5/app01.egg-info/top_level.txt
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.418352 app01-0.1.5/docs/
+-rw-r--r--   0 lihaijian   (501) staff       (20)      606 2023-04-23 06:59:22.000000 app01-0.1.5/docs/Makefile
+-rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.5/docs/authors.rst
+-rwxr-xr-x   0 lihaijian   (501) staff       (20)     4743 2023-04-23 06:59:22.000000 app01-0.1.5/docs/conf.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)       33 2023-04-23 06:59:22.000000 app01-0.1.5/docs/contributing.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)       28 2023-04-23 06:59:22.000000 app01-0.1.5/docs/history.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)      302 2023-04-23 06:59:22.000000 app01-0.1.5/docs/index.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1098 2023-04-23 06:59:22.000000 app01-0.1.5/docs/installation.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)      803 2023-04-23 06:59:22.000000 app01-0.1.5/docs/make.bat
+-rw-r--r--   0 lihaijian   (501) staff       (20)       27 2023-04-23 06:59:22.000000 app01-0.1.5/docs/readme.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)       65 2023-04-23 06:59:22.000000 app01-0.1.5/docs/usage.rst
+-rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-24 01:39:02.421746 app01-0.1.5/setup.cfg
+-rw-r--r--   0 lihaijian   (501) staff       (20)     1336 2023-04-24 01:38:37.000000 app01-0.1.5/setup.py
+drwxr-xr-x   0 lihaijian   (501) staff       (20)        0 2023-04-24 01:39:02.419520 app01-0.1.5/tests/
+-rw-r--r--   0 lihaijian   (501) staff       (20)       35 2023-04-23 06:59:22.000000 app01-0.1.5/tests/__init__.py
+-rw-r--r--   0 lihaijian   (501) staff       (20)      377 2023-04-23 06:59:22.000000 app01-0.1.5/tests/test_app01.py
```

### Comparing `app01-0.1.1/CONTRIBUTING.rst` & `app01-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/LICENSE` & `app01-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/PKG-INFO` & `app01-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app01
-Version: 0.1.1
+Version: 0.1.5
 Summary: my first app01
 Home-page: https://github.com/near2sea/app01
 Author: lihaijian
 Author-email: sanan.li@qq.com
 License: MIT license
 Keywords: app01
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `app01-0.1.1/README.rst` & `app01-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/app01/cli.py` & `app01-0.1.5/app01/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Console script for app01."""
 import argparse
 import sys
-from argparse import Namespace
-
-from matt import math_add
-
+# from argparse import Namespace
+from app01.matt import math_add
 
 def main():
     """Console script for app01."""
     parser = argparse.ArgumentParser()
     parser.add_argument('_', nargs='*')
     args = parser.parse_args()
```

### Comparing `app01-0.1.1/app01.egg-info/PKG-INFO` & `app01-0.1.5/app01.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app01
-Version: 0.1.1
+Version: 0.1.5
 Summary: my first app01
 Home-page: https://github.com/near2sea/app01
 Author: lihaijian
 Author-email: sanan.li@qq.com
 License: MIT license
 Keywords: app01
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `app01-0.1.1/app01.egg-info/SOURCES.txt` & `app01-0.1.5/app01.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 app01/app01.py
 app01/cli.py
 app01.egg-info/PKG-INFO
 app01.egg-info/SOURCES.txt
 app01.egg-info/dependency_links.txt
 app01.egg-info/entry_points.txt
 app01.egg-info/not-zip-safe
+app01.egg-info/requires.txt
 app01.egg-info/top_level.txt
 app01/matt/__init__.py
 app01/matt/math_add.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
```

### Comparing `app01-0.1.1/docs/Makefile` & `app01-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/docs/conf.py` & `app01-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/docs/installation.rst` & `app01-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/docs/make.bat` & `app01-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `app01-0.1.1/setup.py` & `app01-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = [ ]
+requirements = ['pip']
 
-test_requirements = [ ]
+test_requirements = [
+    'pyyaml',
+    'twine']
 
 setup(
     author="lihaijian",
     author_email='sanan.li@qq.com',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -40,10 +42,10 @@
     include_package_data=True,
     keywords='app01',
     name='app01',
     packages=find_packages(include=['app01', 'app01.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/near2sea/app01',
-    version='0.1.1',
+    version='0.1.5',
     zip_safe=False,
 )
```

