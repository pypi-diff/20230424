# Comparing `tmp/aacommpy-0.1.4.tar.gz` & `tmp/aacommpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommpy-0.1.4.tar", last modified: Mon Apr 24 13:07:19 2023, max compression
+gzip compressed data, was "aacommpy-0.1.5.tar", last modified: Mon Apr 24 13:11:09 2023, max compression
```

## Comparing `aacommpy-0.1.4.tar` & `aacommpy-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:07:19.065147 aacommpy-0.1.4/
--rw-rw-rw-   0        0        0      533 2023-04-24 13:07:19.064150 aacommpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-04-24 12:46:06.000000 aacommpy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 13:07:19.052776 aacommpy-0.1.4/aacommpy/
--rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.4/aacommpy/__init__.py
--rw-rw-rw-   0        0        0      263 2023-04-24 13:05:02.000000 aacommpy-0.1.4/aacommpy/__version__.py
--rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.4/aacommpy/curves.py
--rw-rw-rw-   0        0        0     1597 2023-04-24 13:07:17.000000 aacommpy-0.1.4/aacommpy/entry_points.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:07:19.064150 aacommpy-0.1.4/aacommpy.egg-info/
--rw-rw-rw-   0        0        0      533 2023-04-24 13:07:18.000000 aacommpy-0.1.4/aacommpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-24 13:07:19.000000 aacommpy-0.1.4/aacommpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:07:18.000000 aacommpy-0.1.4/aacommpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 13:07:18.000000 aacommpy-0.1.4/aacommpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.4/aacommpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-24 13:07:18.000000 aacommpy-0.1.4/aacommpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 13:07:18.000000 aacommpy-0.1.4/aacommpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:07:19.065147 aacommpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-24 13:05:06.000000 aacommpy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:11:09.067240 aacommpy-0.1.5/
+-rw-rw-rw-   0        0        0      533 2023-04-24 13:11:09.067240 aacommpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-04-24 12:46:06.000000 aacommpy-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:11:09.054762 aacommpy-0.1.5/aacommpy/
+-rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.5/aacommpy/__init__.py
+-rw-rw-rw-   0        0        0      263 2023-04-24 13:11:01.000000 aacommpy-0.1.5/aacommpy/__version__.py
+-rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.5/aacommpy/curves.py
+-rw-rw-rw-   0        0        0     1614 2023-04-24 13:10:43.000000 aacommpy-0.1.5/aacommpy/entry_points.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:11:09.066241 aacommpy-0.1.5/aacommpy.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-04-24 13:11:08.000000 aacommpy-0.1.5/aacommpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-24 13:11:09.000000 aacommpy-0.1.5/aacommpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:11:08.000000 aacommpy-0.1.5/aacommpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 13:11:08.000000 aacommpy-0.1.5/aacommpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.5/aacommpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-04-24 13:11:08.000000 aacommpy-0.1.5/aacommpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 13:11:08.000000 aacommpy-0.1.5/aacommpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:11:09.067240 aacommpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-04-24 13:11:05.000000 aacommpy-0.1.5/setup.py
```

### Comparing `aacommpy-0.1.4/PKG-INFO` & `aacommpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aacommpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: aacommpy - AACOMM nuget package wrapper
 Home-page: https://github.com/jamesbond90/aacommpyDownloader
 Author: HIEU
 Author-email: trunghieupcs@gmail.com
 License: MIT
 Keywords: package development stage
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aacommpy-0.1.4/aacommpy/curves.py` & `aacommpy-0.1.5/aacommpy/curves.py`

 * *Files identical despite different names*

### Comparing `aacommpy-0.1.4/aacommpy/entry_points.py` & `aacommpy-0.1.5/aacommpy/entry_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     nuget_cmd = [nuget_path, 'install', 'Agito.AAComm', '-OutputDirectory', os.path.join(os.path.dirname(nuget_path)), '-Source', 'https://api.nuget.org/v3/index.json']
     subprocess.run(nuget_cmd, check=True)
     return None
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(description='Download aacommpy package.')
-    parser.add_argument('command', choices=['install'], help='Choose a command to execute.')
+    parser.add_argument('command', choices=['install', 'downloadNuget'], help='Choose a command to execute.')
     args = parser.parse_args()
 
     if args.command == 'install':
         install_template()
     elif args.command == 'downloadnuget':
         download_nuget()
     else:
```

### Comparing `aacommpy-0.1.4/aacommpy.egg-info/PKG-INFO` & `aacommpy-0.1.5/aacommpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aacommpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: aacommpy - AACOMM nuget package wrapper
 Home-page: https://github.com/jamesbond90/aacommpyDownloader
 Author: HIEU
 Author-email: trunghieupcs@gmail.com
 License: MIT
 Keywords: package development stage
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aacommpy-0.1.4/setup.py` & `aacommpy-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 about = {
     'name': 'aacommpy',
     'description': 'A Python package for wrapping aacomm nuget package',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'author': 'HIEU',
     'author_email': 'trunghieupcs@gmail.com',
     'url': 'https://github.com/hieu/aacommpy',
     'license': 'MIT',
 }
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'aacommpy', '__version__.py')) as f:
```

