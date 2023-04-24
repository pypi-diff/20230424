# Comparing `tmp/auto_find_date pdf-0.1.0.tar.gz` & `tmp/auto_find_date_pdf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_find_date pdf-0.1.0.tar", last modified: Mon Apr 24 01:02:14 2023, max compression
+gzip compressed data, was "auto_find_date_pdf-0.1.1.tar", last modified: Mon Apr 24 01:29:26 2023, max compression
```

## Comparing `auto_find_date pdf-0.1.0.tar` & `auto_find_date_pdf-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:02:14.512549 auto_find_date pdf-0.1.0/
--rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date pdf-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      212 2023-04-24 01:02:14.510969 auto_find_date pdf-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 01:02:14.510969 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/
--rw-rw-rw-   0        0        0      212 2023-04-24 01:02:14.000000 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-24 01:02:14.000000 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:02:14.000000 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-24 01:02:14.000000 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-04-24 01:02:14.000000 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 01:02:14.000000 auto_find_date pdf-0.1.0/auto_find_date_pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1320 2023-04-24 00:40:25.000000 auto_find_date pdf-0.1.0/main.py
--rw-rw-rw-   0        0        0       42 2023-04-24 01:02:14.512549 auto_find_date pdf-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      530 2023-04-24 00:59:52.000000 auto_find_date pdf-0.1.0/setup.py
--rw-rw-rw-   0        0        0     5989 2023-04-24 00:48:27.000000 auto_find_date pdf-0.1.0/text_search.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:29:26.217960 auto_find_date_pdf-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      212 2023-04-24 01:29:26.217960 auto_find_date_pdf-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 01:29:26.217960 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1320 2023-04-24 00:40:25.000000 auto_find_date_pdf-0.1.1/main.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:29:26.219463 auto_find_date_pdf-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      530 2023-04-24 01:29:15.000000 auto_find_date_pdf-0.1.1/setup.py
+-rw-rw-rw-   0        0        0     5989 2023-04-24 00:48:27.000000 auto_find_date_pdf-0.1.1/text_search.py
```

### Comparing `auto_find_date pdf-0.1.0/LICENSE` & `auto_find_date_pdf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_find_date pdf-0.1.0/main.py` & `auto_find_date_pdf-0.1.1/main.py`

 * *Files identical despite different names*

### Comparing `auto_find_date pdf-0.1.0/setup.py` & `auto_find_date_pdf-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='auto_find_date pdf',
-    version='0.1.0',
+    name='auto_find_date_pdf',
+    version='0.1.1',
     description='A simple lib to find dates from any txt/ pdf/ rtf source',
     author='Your Name',
     packages=find_packages(),
     author_email='opensource@marvsai.com',
     py_modules=['text_search', 'main'],
     install_requires=[
         'pypdf',
```

### Comparing `auto_find_date pdf-0.1.0/text_search.py` & `auto_find_date_pdf-0.1.1/text_search.py`

 * *Files identical despite different names*

