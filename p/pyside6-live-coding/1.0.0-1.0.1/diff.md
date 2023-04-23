# Comparing `tmp/pyside6-live-coding-1.0.0.tar.gz` & `tmp/pyside6-live-coding-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside6-live-coding-1.0.0.tar", last modified: Sun Apr 23 22:30:13 2023, max compression
+gzip compressed data, was "pyside6-live-coding-1.0.1.tar", last modified: Sun Apr 23 22:42:27 2023, max compression
```

## Comparing `pyside6-live-coding-1.0.0.tar` & `pyside6-live-coding-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.873618 pyside6-live-coding-1.0.0/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      178 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/MANIFEST.in
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4854 2023-04-23 22:30:13.873618 pyside6-live-coding-1.0.0/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3739 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/bin/
--rwxrwxr-x   0 alexander  (1000) alexander  (1000)      633 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/bin/pyside6-live-coding
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/examples/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/examples/integrated/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1113 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/integrated/live.qml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1622 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/integrated/main.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      215 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/integrated/main.qml
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/examples/integrated/myapp/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      102 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/integrated/myapp/MainPanel.qml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2023-04-23 21:14:42.000000 pyside6-live-coding-1.0.0/examples/integrated/myapp/qmldir
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/examples/standalone/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      633 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/standalone/MainScreen.qml
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/examples/standalone/module/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      206 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/standalone/module/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1133 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/examples/standalone/module/calculator.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       30 2023-04-23 21:14:42.000000 pyside6-live-coding-1.0.0/examples/standalone/qmldir
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-04-23 22:30:13.873618 pyside6-live-coding-1.0.0/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      977 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/setup.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.869618 pyside6-live-coding-1.0.0/src/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.873618 pyside6-live-coding-1.0.0/src/pyside6_live_coding/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1720 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/FileSelectionDialog.qml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5464 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/LiveCodingPanel.qml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      288 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/__init__.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4435 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/filewatcher.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2738 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/gui.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     5591 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/icon.png
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1117 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/live.qml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      803 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/live_coding_helper.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1303 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/moduleloader.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2205 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/projectbrowser.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      770 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/pythonreloader.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       88 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/qmldir
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      462 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding/register_qml_types.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:30:13.873618 pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4854 2023-04-23 22:30:13.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1100 2023-04-23 22:30:13.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-04-23 22:30:13.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       73 2023-04-23 22:30:13.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       20 2023-04-23 22:30:13.000000 pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/top_level.txt
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.544927 pyside6-live-coding-1.0.1/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      178 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/MANIFEST.in
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4854 2023-04-23 22:42:27.544927 pyside6-live-coding-1.0.1/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     3739 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/bin/
+-rwxrwxr-x   0 alexander  (1000) alexander  (1000)      633 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/bin/pyside6-live-coding
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.536927 pyside6-live-coding-1.0.1/examples/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/examples/integrated/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1113 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/integrated/live.qml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1622 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/integrated/main.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      215 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/integrated/main.qml
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/examples/integrated/myapp/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      102 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/integrated/myapp/MainPanel.qml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       28 2023-04-23 21:14:42.000000 pyside6-live-coding-1.0.1/examples/integrated/myapp/qmldir
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/examples/standalone/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      633 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/standalone/MainScreen.qml
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/examples/standalone/module/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      206 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/standalone/module/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1133 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/examples/standalone/module/calculator.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       30 2023-04-23 21:14:42.000000 pyside6-live-coding-1.0.1/examples/standalone/qmldir
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-04-23 22:42:27.544927 pyside6-live-coding-1.0.1/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      973 2023-04-23 22:42:04.000000 pyside6-live-coding-1.0.1/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/src/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.540927 pyside6-live-coding-1.0.1/src/pyside6_live_coding/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1720 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/FileSelectionDialog.qml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5464 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/LiveCodingPanel.qml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      288 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/__init__.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4435 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/filewatcher.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2738 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/gui.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     5591 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/icon.png
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1117 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/live.qml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      803 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/live_coding_helper.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1303 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/moduleloader.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2205 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/projectbrowser.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      770 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/pythonreloader.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       88 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/qmldir
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      462 2023-04-23 22:22:31.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding/register_qml_types.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-04-23 22:42:27.544927 pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4854 2023-04-23 22:42:27.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1100 2023-04-23 22:42:27.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-04-23 22:42:27.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       72 2023-04-23 22:42:27.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       20 2023-04-23 22:42:27.000000 pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/top_level.txt
```

### Comparing `pyside6-live-coding-1.0.0/PKG-INFO` & `pyside6-live-coding-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside6-live-coding
-Version: 1.0.0
+Version: 1.0.1
 Summary: Live coding for Python, Qt and QML
 Home-page: https://github.com/machinekoder/pyside6-live-coding/
 Author: Alexander Rössler
 Author-email: alex@machinekoder.com
 License: MIT
 Description: # Live Coding Environment for Python, Qt and QML
         [![PyPI version](https://badge.fury.io/py/pyside6-live-coding.svg)](https://badge.fury.io/py/pyside6-live-coding)
```

### Comparing `pyside6-live-coding-1.0.0/README.md` & `pyside6-live-coding-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/bin/pyside6-live-coding` & `pyside6-live-coding-1.0.1/bin/pyside6-live-coding`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/examples/integrated/live.qml` & `pyside6-live-coding-1.0.1/examples/integrated/live.qml`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/examples/integrated/main.py` & `pyside6-live-coding-1.0.1/examples/integrated/main.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/examples/standalone/MainScreen.qml` & `pyside6-live-coding-1.0.1/examples/standalone/MainScreen.qml`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/examples/standalone/module/calculator.py` & `pyside6-live-coding-1.0.1/examples/standalone/module/calculator.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/setup.py` & `pyside6-live-coding-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='pyside6-live-coding',
-    version='1.0.0',
+    version='1.0.1',
     packages=['pyside6_live_coding'],
     package_dir={'': 'src'},
     url='https://github.com/machinekoder/pyside6-live-coding/',
     license='MIT',
     author='Alexander Rössler',
     author_email='alex@machinekoder.com',
     description='Live coding for Python, Qt and QML',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['six', 'qtpy'],
+    install_requires=['PySide6'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov',
             'pytest-qt',
             'black',
```

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/FileSelectionDialog.qml` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/FileSelectionDialog.qml`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/LiveCodingPanel.qml` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/LiveCodingPanel.qml`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/filewatcher.py` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/filewatcher.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/gui.py` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/gui.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/icon.png` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/icon.png`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/live.qml` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/live.qml`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/live_coding_helper.py` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/live_coding_helper.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/moduleloader.py` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/moduleloader.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/projectbrowser.py` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/projectbrowser.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding/pythonreloader.py` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding/pythonreloader.py`

 * *Files identical despite different names*

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/PKG-INFO` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside6-live-coding
-Version: 1.0.0
+Version: 1.0.1
 Summary: Live coding for Python, Qt and QML
 Home-page: https://github.com/machinekoder/pyside6-live-coding/
 Author: Alexander Rössler
 Author-email: alex@machinekoder.com
 License: MIT
 Description: # Live Coding Environment for Python, Qt and QML
         [![PyPI version](https://badge.fury.io/py/pyside6-live-coding.svg)](https://badge.fury.io/py/pyside6-live-coding)
```

### Comparing `pyside6-live-coding-1.0.0/src/pyside6_live_coding.egg-info/SOURCES.txt` & `pyside6-live-coding-1.0.1/src/pyside6_live_coding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

