# Comparing `tmp/mfrc522-python-0.0.5.dev1.tar.gz` & `tmp/mfrc522-python-0.0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.5.dev1.tar", last modified: Wed Apr 19 16:34:26 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.5.dev2.tar", last modified: Mon Apr 24 08:02:59 2023, max compression
```

## Comparing `mfrc522-python-0.0.5.dev1.tar` & `mfrc522-python-0.0.5.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:34:26.895637 mfrc522-python-0.0.5.dev1/
--rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev1/LICENSE
--rw-rw-rw-   0        0        0     3018 2023-04-19 16:34:26.887640 mfrc522-python-0.0.5.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev1/README.md
--rw-rw-rw-   0        0        0      665 2023-04-19 16:21:23.000000 mfrc522-python-0.0.5.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 16:34:26.895637 mfrc522-python-0.0.5.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 16:34:26.839631 mfrc522-python-0.0.5.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 16:34:26.871649 mfrc522-python-0.0.5.dev1/src/mfrc522/
--rw-rw-rw-   0        0        0     5618 2023-04-19 16:03:53.000000 mfrc522-python-0.0.5.dev1/src/mfrc522/BasicMFRC522.py
--rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev1/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0     3368 2023-04-19 16:18:45.000000 mfrc522-python-0.0.5.dev1/src/mfrc522/SimpleMFRC522.py
--rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev1/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:34:26.887640 mfrc522-python-0.0.5.dev1/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0     3018 2023-04-19 16:34:26.000000 mfrc522-python-0.0.5.dev1/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-19 16:34:26.000000 mfrc522-python-0.0.5.dev1/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:34:26.000000 mfrc522-python-0.0.5.dev1/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 16:34:26.000000 mfrc522-python-0.0.5.dev1/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.545494 mfrc522-python-0.0.5.dev2/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev2/LICENSE
+-rw-rw-rw-   0        0        0     3018 2023-04-24 08:02:59.543495 mfrc522-python-0.0.5.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev2/README.md
+-rw-rw-rw-   0        0        0      665 2023-04-24 07:59:38.000000 mfrc522-python-0.0.5.dev2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:02:59.546562 mfrc522-python-0.0.5.dev2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.349629 mfrc522-python-0.0.5.dev2/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.497467 mfrc522-python-0.0.5.dev2/src/mfrc522/
+-rw-rw-rw-   0        0        0     5617 2023-04-24 07:58:49.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/BasicMFRC522.py
+-rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0     3368 2023-04-19 16:18:45.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/SimpleMFRC522.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.540496 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3018 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.5.dev1/LICENSE` & `mfrc522-python-0.0.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev1/PKG-INFO` & `mfrc522-python-0.0.5.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.5.dev1
+Version: 0.0.5.dev2
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mfrc522-python-0.0.5.dev1/README.md` & `mfrc522-python-0.0.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev1/pyproject.toml` & `mfrc522-python-0.0.5.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.5.dev1"
+version = "0.0.5.dev2"
 authors = [
   { name="Aditya"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mfrc522-python-0.0.5.dev1/src/mfrc522/BasicMFRC522.py` & `mfrc522-python-0.0.5.dev2/src/mfrc522/BasicMFRC522.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import MFRC522
 
-class SimpleMFRC522:
+class BasicMFRC522:
     def __init__(self, KEY=[0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]):
         self.MFRC522 = MFRC522()
         self.KEY = KEY
     
     def read_sector(self, trailer_block=11):
         id, text = self.read_no_block(trailer_block, (trailer_block-3, trailer_block-2, trailer_block-1))
         while not id:
```

### Comparing `mfrc522-python-0.0.5.dev1/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.5.dev2/src/mfrc522/MFRC522.py`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev1/src/mfrc522/SimpleMFRC522.py` & `mfrc522-python-0.0.5.dev2/src/mfrc522/SimpleMFRC522.py`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev1/src/mfrc522_python.egg-info/PKG-INFO` & `mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.5.dev1
+Version: 0.0.5.dev2
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

