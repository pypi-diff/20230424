# Comparing `tmp/gkligo-0.0.2.tar.gz` & `tmp/gkligo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gkligo-0.0.2.tar", last modified: Wed Mar  8 22:10:52 2023, max compression
+gzip compressed data, was "gkligo-0.0.3.tar", last modified: Mon Apr 24 12:56:05 2023, max compression
```

## Comparing `gkligo-0.0.2.tar` & `gkligo-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-03-08 22:10:52.805523 gkligo-0.0.2/
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.2/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1461 2023-03-08 22:10:52.805010 gkligo-0.0.2/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      772 2023-03-08 21:50:03.000000 gkligo-0.0.2/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-03-08 22:10:52.798534 gkligo-0.0.2/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.2/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 22:09:29.000000 gkligo-0.0.2/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-03-08 22:10:52.801900 gkligo-0.0.2/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.2/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-03-08 22:10:52.804096 gkligo-0.0.2/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.2/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       91 2023-03-08 21:07:47.000000 gkligo-0.0.2/gkligo/scripts/python/config_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     5001 2023-03-04 15:58:35.000000 gkligo-0.0.2/gkligo/scripts/python/downloadGWAlerts.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-03-08 22:10:52.801331 gkligo-0.0.2/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1461 2023-03-08 22:10:52.000000 gkligo-0.0.2/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      398 2023-03-08 22:10:52.000000 gkligo-0.0.2/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-03-08 22:10:52.000000 gkligo-0.0.2/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)       82 2023-03-08 22:10:52.000000 gkligo-0.0.2/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       71 2023-03-08 22:10:52.000000 gkligo-0.0.2/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-03-08 22:10:52.000000 gkligo-0.0.2/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-03-08 22:10:52.805753 gkligo-0.0.2/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1150 2023-03-08 22:09:15.000000 gkligo-0.0.2/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.683825 gkligo-0.0.3/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.3/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.3/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 12:56:05.683273 gkligo-0.0.3/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.3/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.671709 gkligo-0.0.3/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.3/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-24 12:30:42.000000 gkligo-0.0.3/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.676018 gkligo-0.0.3/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.3/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.682247 gkligo-0.0.3/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.3/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.3/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.3/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      520 2023-04-24 12:50:32.000000 gkligo-0.0.3/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     8993 2023-04-24 09:27:27.000000 gkligo-0.0.3/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     4922 2023-04-18 21:48:34.000000 gkligo-0.0.3/gkligo/scripts/python/generateGWReports.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2538 2023-04-20 14:57:17.000000 gkligo-0.0.3/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.675170 gkligo-0.0.3/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       71 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-24 12:56:05.684045 gkligo-0.0.3/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1281 2023-04-24 12:38:44.000000 gkligo-0.0.3/setup.py
```

### Comparing `gkligo-0.0.2/setup.py` & `gkligo-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 import os
 
 moduleDirectory = os.path.dirname(os.path.realpath(__file__))
+exec(open(moduleDirectory + "/gkligo/__version__.py").read())
 
 
 def readme():
     with open(moduleDirectory + '/README.md') as f:
         return f.read()
 
 
 setup(
     name="gkligo",
     description='GW (LIGO) utilities',
     long_description=readme(),
     long_description_content_type="text/markdown",
-    version="0.0.2",
+    version=__version__,
     author='genghisken',
     author_email='ken.w.smith@gmail.com',
     license='MIT',
     url='https://github.com/genghisken/gkligo',
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
@@ -36,10 +37,10 @@
           'ligo.skymap',
           'astropy',
           'mocpy',
           'pyYAML',
       ],
     python_requires='>=3.7',
     entry_points = {
-        'console_scripts': ['downloadGWAlerts=gkligo.scripts.python.downloadGWAlerts:main'],
+        'console_scripts': ['downloadGWAlerts=gkligo.scripts.python.downloadGWAlerts:main','generateGWReports=gkligo.scripts.python.generateGWReports:main'],
     },
 )
```

