# Comparing `tmp/hone-0.2.1.tar.gz` & `tmp/hone-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hone-0.2.1.tar", last modified: Sat Jun 20 23:34:13 2020, max compression
+gzip compressed data, was "hone-0.2.2.tar", last modified: Mon Apr 24 20:32:30 2023, max compression
```

## Comparing `hone-0.2.1.tar` & `hone-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2020-06-20 23:34:13.000000 hone-0.2.1/
--rw-rw-rw-   0        0        0      541 2020-06-20 23:34:13.000000 hone-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3673 2020-06-04 01:43:54.000000 hone-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2020-06-20 23:34:13.000000 hone-0.2.1/hone/
--rw-rw-rw-   0        0        0       26 2020-05-31 00:14:52.000000 hone-0.2.1/hone/__init__.py
--rw-rw-rw-   0        0        0     1552 2020-06-04 01:40:54.000000 hone-0.2.1/hone/__main__.py
--rw-rw-rw-   0        0        0     6638 2020-06-04 01:24:11.000000 hone-0.2.1/hone/hone.py
-drwxrwxrwx   0        0        0        0 2020-06-20 23:34:13.000000 hone-0.2.1/hone/test/
--rw-rw-rw-   0        0        0        0 2020-05-27 02:13:42.000000 hone-0.2.1/hone/test/__init__.py
--rw-rw-rw-   0        0        0     1724 2020-05-27 02:13:42.000000 hone-0.2.1/hone/test/test_csv_utils.py
--rw-rw-rw-   0        0        0     1954 2020-06-04 01:04:18.000000 hone-0.2.1/hone/test/test_hone.py
-drwxrwxrwx   0        0        0        0 2020-06-20 23:34:13.000000 hone-0.2.1/hone/utils/
--rw-rw-rw-   0        0        0        0 2019-03-23 06:11:24.000000 hone-0.2.1/hone/utils/__init__.py
--rw-rw-rw-   0        0        0     1045 2020-06-20 22:55:44.000000 hone-0.2.1/hone/utils/csv_utils.py
--rw-rw-rw-   0        0        0      443 2020-05-31 01:22:15.000000 hone-0.2.1/hone/utils/json_utils.py
--rw-rw-rw-   0        0        0      432 2020-05-31 00:56:21.000000 hone-0.2.1/hone/utils/test_utils.py
-drwxrwxrwx   0        0        0        0 2020-06-20 23:34:13.000000 hone-0.2.1/hone.egg-info/
--rw-rw-rw-   0        0        0      541 2020-06-20 23:34:13.000000 hone-0.2.1/hone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2020-06-20 23:34:13.000000 hone-0.2.1/hone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-20 23:34:13.000000 hone-0.2.1/hone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2020-06-20 23:34:13.000000 hone-0.2.1/hone.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2020-06-20 23:34:13.000000 hone-0.2.1/hone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-20 23:34:13.000000 hone-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      772 2020-06-20 23:33:08.000000 hone-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:32:30.257372 hone-0.2.2/
+-rw-rw-rw-   0        0        0     1097 2023-04-24 20:29:26.000000 hone-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-04-24 20:32:30.257372 hone-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3673 2023-04-24 20:29:26.000000 hone-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 20:32:30.212503 hone-0.2.2/hone/
+-rw-rw-rw-   0        0        0       26 2023-04-24 20:29:26.000000 hone-0.2.2/hone/__init__.py
+-rw-rw-rw-   0        0        0     1552 2023-04-24 20:29:26.000000 hone-0.2.2/hone/__main__.py
+-rw-rw-rw-   0        0        0     6638 2023-04-24 20:29:26.000000 hone-0.2.2/hone/hone.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:32:30.238476 hone-0.2.2/hone/test/
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:29:26.000000 hone-0.2.2/hone/test/__init__.py
+-rw-rw-rw-   0        0        0     1724 2023-04-24 20:29:26.000000 hone-0.2.2/hone/test/test_csv_utils.py
+-rw-rw-rw-   0        0        0     1954 2023-04-24 20:29:26.000000 hone-0.2.2/hone/test/test_hone.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:32:30.256364 hone-0.2.2/hone/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:29:26.000000 hone-0.2.2/hone/utils/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-04-24 20:29:26.000000 hone-0.2.2/hone/utils/csv_utils.py
+-rw-rw-rw-   0        0        0      443 2023-04-24 20:29:26.000000 hone-0.2.2/hone/utils/json_utils.py
+-rw-rw-rw-   0        0        0      432 2023-04-24 20:29:26.000000 hone-0.2.2/hone/utils/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:32:30.227335 hone-0.2.2/hone.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-04-24 20:32:29.000000 hone-0.2.2/hone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-04-24 20:32:30.000000 hone-0.2.2/hone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 20:32:29.000000 hone-0.2.2/hone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-24 20:32:29.000000 hone-0.2.2/hone.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-04-24 20:32:29.000000 hone-0.2.2/hone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 20:32:30.257372 hone-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-04-24 20:31:31.000000 hone-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hone-0.2.1/README.md` & `hone-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hone-0.2.1/hone/__main__.py` & `hone-0.2.2/hone/__main__.py`

 * *Files identical despite different names*

### Comparing `hone-0.2.1/hone/hone.py` & `hone-0.2.2/hone/hone.py`

 * *Files identical despite different names*

### Comparing `hone-0.2.1/hone/test/test_csv_utils.py` & `hone-0.2.2/hone/test/test_csv_utils.py`

 * *Files identical despite different names*

### Comparing `hone-0.2.1/hone/test/test_hone.py` & `hone-0.2.2/hone/test/test_hone.py`

 * *Files identical despite different names*

### Comparing `hone-0.2.1/hone/utils/csv_utils.py` & `hone-0.2.2/hone/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `hone-0.2.1/setup.py` & `hone-0.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='hone',
-    version='0.2.1',
-    author='Chamantha Kankanamge',
+    version='0.2.2',
     author_email='chamkdev@gmail.com',
     license='MIT',
     description='Convert CSV to automatically nested JSON.',
     keywords="convert csv auto nested json",
     url='https://github.com/chamkank/hone',
     project_urls={
         "Source Code": 'https://github.com/chamkank/hone'
     },
     packages=find_packages(),
     install_requires=[],
     python_requires='>=3.0',
     entry_points={'console_scripts': ['hone=hone.__main__:main']},
     classifiers=[
-        "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities"
     ]
 )
```

