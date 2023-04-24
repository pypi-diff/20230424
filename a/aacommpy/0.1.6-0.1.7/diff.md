# Comparing `tmp/aacommpy-0.1.6.tar.gz` & `tmp/aacommpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommpy-0.1.6.tar", last modified: Mon Apr 24 13:14:12 2023, max compression
+gzip compressed data, was "aacommpy-0.1.7.tar", last modified: Mon Apr 24 13:28:53 2023, max compression
```

## Comparing `aacommpy-0.1.6.tar` & `aacommpy-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:14:12.900543 aacommpy-0.1.6/
--rw-rw-rw-   0        0        0      533 2023-04-24 13:14:12.900543 aacommpy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-04-24 12:46:06.000000 aacommpy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 13:14:12.888039 aacommpy-0.1.6/aacommpy/
--rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.6/aacommpy/__init__.py
--rw-rw-rw-   0        0        0      263 2023-04-24 13:14:00.000000 aacommpy-0.1.6/aacommpy/__version__.py
--rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.6/aacommpy/curves.py
--rw-rw-rw-   0        0        0     1614 2023-04-24 13:12:31.000000 aacommpy-0.1.6/aacommpy/entry_points.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:14:12.899546 aacommpy-0.1.6/aacommpy.egg-info/
--rw-rw-rw-   0        0        0      533 2023-04-24 13:14:12.000000 aacommpy-0.1.6/aacommpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-24 13:14:12.000000 aacommpy-0.1.6/aacommpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:14:12.000000 aacommpy-0.1.6/aacommpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 13:14:12.000000 aacommpy-0.1.6/aacommpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.6/aacommpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-24 13:14:12.000000 aacommpy-0.1.6/aacommpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 13:14:12.000000 aacommpy-0.1.6/aacommpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:14:12.901541 aacommpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-24 13:12:42.000000 aacommpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:28:53.993817 aacommpy-0.1.7/
+-rw-rw-rw-   0        0        0      533 2023-04-24 13:28:53.992818 aacommpy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-04-24 12:46:06.000000 aacommpy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:28:53.973795 aacommpy-0.1.7/aacommpy/
+-rw-rw-rw-   0        0        0       95 2023-04-24 11:51:36.000000 aacommpy-0.1.7/aacommpy/__init__.py
+-rw-rw-rw-   0        0        0      263 2023-04-24 13:28:20.000000 aacommpy-0.1.7/aacommpy/__version__.py
+-rw-rw-rw-   0        0        0    10361 2023-04-23 17:15:24.000000 aacommpy-0.1.7/aacommpy/curves.py
+-rw-rw-rw-   0        0        0     1994 2023-04-24 13:28:15.000000 aacommpy-0.1.7/aacommpy/entry_points.py
+-rw-rw-rw-   0        0        0      104 2023-04-24 13:18:38.000000 aacommpy-0.1.7/aacommpy/nugetmanagement.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:28:53.991795 aacommpy-0.1.7/aacommpy.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-04-24 13:28:53.000000 aacommpy-0.1.7/aacommpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-24 13:28:53.000000 aacommpy-0.1.7/aacommpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:28:53.000000 aacommpy-0.1.7/aacommpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 13:28:53.000000 aacommpy-0.1.7/aacommpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 12:09:32.000000 aacommpy-0.1.7/aacommpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-04-24 13:28:53.000000 aacommpy-0.1.7/aacommpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 13:28:53.000000 aacommpy-0.1.7/aacommpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:28:53.993817 aacommpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-04-24 13:28:24.000000 aacommpy-0.1.7/setup.py
```

### Comparing `aacommpy-0.1.6/PKG-INFO` & `aacommpy-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aacommpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: aacommpy - AACOMM nuget package wrapper
 Home-page: https://github.com/jamesbond90/aacommpyDownloader
 Author: HIEU
 Author-email: trunghieupcs@gmail.com
 License: MIT
 Keywords: package development stage
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aacommpy-0.1.6/aacommpy/curves.py` & `aacommpy-0.1.7/aacommpy/curves.py`

 * *Files identical despite different names*

### Comparing `aacommpy-0.1.6/aacommpy/entry_points.py` & `aacommpy-0.1.7/aacommpy/entry_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,25 +23,34 @@
     return None
 
 def download_nuget() -> None:
     nuget_path = os.path.join(os.path.dirname(__file__), 'aacommpyDownloader-main', 'nuget.exe')
     nuget_cmd = [nuget_path, 'install', 'Agito.AAComm', '-OutputDirectory', os.path.join(os.path.dirname(nuget_path)), '-Source', 'https://api.nuget.org/v3/index.json']
     subprocess.run(nuget_cmd, check=True)
     return None
+def nuget_version() -> None:
+    nuget_path = os.path.join(os.path.dirname(__file__), 'aacommpyDownloader-main', 'nuget.exe')
+    nuget_cmd = [nuget_path, 'list Agito.AAcomm']
+    subprocess.run(nuget_cmd, check=True)
+    output = subprocess.check_output(nuget_cmd)
+    print(output.decode())
+    return None
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(description='Download aacommpy package.')
-    parser.add_argument('command', choices=['install', 'downloadnuget'], help='Choose a command to execute.')
+    parser.add_argument('command', choices=['install', 'downloadnuget', 'version'], help='Choose a command to execute.')
     args = parser.parse_args()
 
     if args.command == 'install':
         install_template()
     elif args.command == 'downloadnuget':
         download_nuget()
+    elif args.command == 'version':
+        nuget_version()
     else:
         raise RuntimeError('Please supply a valid command for aacommpy - e.g. install.')
 
     return None
 
 
 if __name__ == '__main__':
```

### Comparing `aacommpy-0.1.6/aacommpy.egg-info/PKG-INFO` & `aacommpy-0.1.7/aacommpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aacommpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: aacommpy - AACOMM nuget package wrapper
 Home-page: https://github.com/jamesbond90/aacommpyDownloader
 Author: HIEU
 Author-email: trunghieupcs@gmail.com
 License: MIT
 Keywords: package development stage
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aacommpy-0.1.6/setup.py` & `aacommpy-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from setuptools import setup
 
 about = {
     'name': 'aacommpy',
     'description': 'A Python package for wrapping aacomm nuget package',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'author': 'HIEU',
     'author_email': 'trunghieupcs@gmail.com',
     'url': 'https://github.com/hieu/aacommpy',
     'license': 'MIT',
 }
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, 'aacommpy', '__version__.py')) as f:
```

