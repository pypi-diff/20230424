# Comparing `tmp/pychunkbuffers-1.0.0.tar.gz` & `tmp/pychunkbuffers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychunkbuffers-1.0.0.tar", last modified: Thu Apr 20 10:29:20 2023, max compression
+gzip compressed data, was "pychunkbuffers-1.0.1.tar", last modified: Mon Apr 24 06:56:26 2023, max compression
```

## Comparing `pychunkbuffers-1.0.0.tar` & `pychunkbuffers-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 10:29:20.446296 pychunkbuffers-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-04-20 07:29:14.000000 pychunkbuffers-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2792 2023-04-20 10:29:20.442017 pychunkbuffers-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2144 2023-04-20 10:26:02.000000 pychunkbuffers-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 10:29:20.440522 pychunkbuffers-1.0.0/pychunkbuffers.egg-info/
--rw-rw-rw-   0        0        0     2792 2023-04-20 10:29:20.000000 pychunkbuffers-1.0.0/pychunkbuffers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-20 10:29:20.000000 pychunkbuffers-1.0.0/pychunkbuffers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 10:29:20.000000 pychunkbuffers-1.0.0/pychunkbuffers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 10:29:20.000000 pychunkbuffers-1.0.0/pychunkbuffers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 10:29:20.446664 pychunkbuffers-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      931 2023-04-20 10:26:02.000000 pychunkbuffers-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:56:26.055147 pychunkbuffers-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-20 07:29:14.000000 pychunkbuffers-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2792 2023-04-24 06:56:26.054085 pychunkbuffers-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2144 2023-04-20 10:26:02.000000 pychunkbuffers-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:56:26.053076 pychunkbuffers-1.0.1/pychunkbuffers.egg-info/
+-rw-rw-rw-   0        0        0     2792 2023-04-24 06:56:25.000000 pychunkbuffers-1.0.1/pychunkbuffers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-24 06:56:26.000000 pychunkbuffers-1.0.1/pychunkbuffers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:56:26.000000 pychunkbuffers-1.0.1/pychunkbuffers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:56:26.000000 pychunkbuffers-1.0.1/pychunkbuffers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:56:26.055439 pychunkbuffers-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      931 2023-04-24 06:56:10.000000 pychunkbuffers-1.0.1/setup.py
```

### Comparing `pychunkbuffers-1.0.0/LICENSE` & `pychunkbuffers-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychunkbuffers-1.0.0/PKG-INFO` & `pychunkbuffers-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunkbuffers
-Version: 1.0.0
+Version: 1.0.1
 Summary: An open-source python library for writing large amounts of data to buffers via chunks
 Home-page: https://github.com/AdityaIyer2k7/pychunkbuffers
 Author: AdityaIyer2k7
 Author-email: adityaiyer2007@gmail.com
 Keywords: python 3,threading,thread,chunking,buffers,pychunk,pybuffer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pychunkbuffers-1.0.0/README.md` & `pychunkbuffers-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pychunkbuffers-1.0.0/pychunkbuffers.egg-info/PKG-INFO` & `pychunkbuffers-1.0.1/pychunkbuffers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunkbuffers
-Version: 1.0.0
+Version: 1.0.1
 Summary: An open-source python library for writing large amounts of data to buffers via chunks
 Home-page: https://github.com/AdityaIyer2k7/pychunkbuffers
 Author: AdityaIyer2k7
 Author-email: adityaiyer2007@gmail.com
 Keywords: python 3,threading,thread,chunking,buffers,pychunk,pybuffer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pychunkbuffers-1.0.0/setup.py` & `pychunkbuffers-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md") as fl: ldesc = fl.read()
 setuptools.setup(
     name="pychunkbuffers",
-    version="1.0.0",
+    version="1.0.1",
     author="AdityaIyer2k7",
     author_email="adityaiyer2007@gmail.com",
     description="An open-source python library for writing large amounts of data to buffers via chunks",
     long_description=ldesc,
     long_description_content_type="text/markdown",
     url="https://github.com/AdityaIyer2k7/pychunkbuffers",
     packages=setuptools.find_packages(),
```

