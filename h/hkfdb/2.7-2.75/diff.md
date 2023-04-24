# Comparing `tmp/hkfdb-2.7.tar.gz` & `tmp/hkfdb-2.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-2.7.tar", last modified: Mon Apr 24 10:23:06 2023, max compression
+gzip compressed data, was "hkfdb-2.75.tar", last modified: Mon Apr 24 10:24:20 2023, max compression
```

## Comparing `hkfdb-2.7.tar` & `hkfdb-2.75.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:23:06.642122 hkfdb-2.7/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.7/LICENSE
--rw-rw-rw-   0        0        0     1651 2023-04-24 10:23:06.642122 hkfdb-2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 10:23:06.631468 hkfdb-2.7/hkfdb/
--rw-rw-rw-   0        0        0    90787 2023-04-24 10:19:26.000000 hkfdb-2.7/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.7/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:23:06.641111 hkfdb-2.7/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1651 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 10:23:06.000000 hkfdb-2.7/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 10:23:06.642122 hkfdb-2.7/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-04-24 10:20:36.000000 hkfdb-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:24:20.560833 hkfdb-2.75/
+-rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.75/LICENSE
+-rw-rw-rw-   0        0        0     1652 2023-04-24 10:24:20.560833 hkfdb-2.75/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.75/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 10:24:20.550830 hkfdb-2.75/hkfdb/
+-rw-rw-rw-   0        0        0    90787 2023-04-24 10:19:26.000000 hkfdb-2.75/hkfdb/Database.py
+-rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.75/hkfdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:24:20.559832 hkfdb-2.75/hkfdb.egg-info/
+-rw-rw-rw-   0        0        0     1652 2023-04-24 10:24:20.000000 hkfdb-2.75/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-24 10:24:20.000000 hkfdb-2.75/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:24:20.000000 hkfdb-2.75/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-24 10:24:20.000000 hkfdb-2.75/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 10:24:20.000000 hkfdb-2.75/hkfdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:24:20.561833 hkfdb-2.75/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-04-24 10:23:59.000000 hkfdb-2.75/setup.py
```

### Comparing `hkfdb-2.7/LICENSE` & `hkfdb-2.75/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-2.7/PKG-INFO` & `hkfdb-2.75/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.7
+Version: 2.75
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.7/README.md` & `hkfdb-2.75/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-2.7/hkfdb/Database.py` & `hkfdb-2.75/hkfdb/Database.py`

 * *Files identical despite different names*

### Comparing `hkfdb-2.7/hkfdb.egg-info/PKG-INFO` & `hkfdb-2.75/hkfdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.7
+Version: 2.75
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.7/setup.py` & `hkfdb-2.75/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="2.7",
+    version="2.75",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

