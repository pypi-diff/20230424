# Comparing `tmp/autoplot-0.6.1.tar.gz` & `tmp/autoplot-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplot-0.6.1.tar", last modified: Mon Apr 24 14:24:06 2023, max compression
+gzip compressed data, was "autoplot-0.6.2.tar", last modified: Mon Apr 24 14:54:45 2023, max compression
```

## Comparing `autoplot-0.6.1.tar` & `autoplot-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:24:06.018203 autoplot-0.6.1/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.6.1/LICENSE.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:24:06.018203 autoplot-0.6.1/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1818 2023-04-24 14:22:53.000000 autoplot-0.6.1/README.rst
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:24:06.018203 autoplot-0.6.1/autoplot/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      310 2023-04-24 14:19:03.000000 autoplot-0.6.1/autoplot/__init__.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)    22169 2023-04-24 14:21:05.000000 autoplot-0.6.1/autoplot/autoplot.py
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:24:06.018203 autoplot-0.6.1/autoplot.egg-info/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/requires.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/top_level.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-24 14:24:06.018203 autoplot-0.6.1/setup.cfg
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-24 14:18:57.000000 autoplot-0.6.1/setup.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:54:45.490496 autoplot-0.6.2/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.6.2/LICENSE.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:54:45.490496 autoplot-0.6.2/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1818 2023-04-24 14:22:53.000000 autoplot-0.6.2/README.rst
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:54:45.490496 autoplot-0.6.2/autoplot/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      310 2023-04-24 14:19:03.000000 autoplot-0.6.2/autoplot/__init__.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)    22099 2023-04-24 14:47:20.000000 autoplot-0.6.2/autoplot/autoplot.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:54:45.490496 autoplot-0.6.2/autoplot.egg-info/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/requires.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/top_level.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-24 14:54:45.490496 autoplot-0.6.2/setup.cfg
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-24 14:47:57.000000 autoplot-0.6.2/setup.py
```

### Comparing `autoplot-0.6.1/LICENSE.txt` & `autoplot-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoplot-0.6.1/PKG-INFO` & `autoplot-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplot
-Version: 0.6.1
+Version: 0.6.2
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
 License-File: LICENSE.txt
```

### Comparing `autoplot-0.6.1/README.rst` & `autoplot-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `autoplot-0.6.1/autoplot/autoplot.py` & `autoplot-0.6.2/autoplot/autoplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import print_function
 
 
 def version():
-    return '0.6.1'
+    return '0.6.2'
 
 
 def printNoNewline(s):
     print(s, end=' ')
 
 
 def javaaddpath(url='', jdwpPort=-1):
-    """Start up JVM, import JAR at URL, and import the paths starting with org
-    into the Python namespace.
+    """Start up JVM, import JAR at URL.
       com= jpype.JPackage('com') 
     can be used to the com package into the Python namespace.
     Example:
       javaaddpath('http://autoplot.org/devel/autoplot.jar')
     if no url is provided, then the default http://autoplot.org/latest/autoplot.jar is used.
     """
```

### Comparing `autoplot-0.6.1/autoplot.egg-info/PKG-INFO` & `autoplot-0.6.2/autoplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoplot
-Version: 0.6.1
+Version: 0.6.2
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
 License-File: LICENSE.txt
```

### Comparing `autoplot-0.6.1/setup.py` & `autoplot-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = ["jpype1","numpy"]
 
 if sys.argv[1] == 'develop':
     install_requires.append("pytest")
 
 setup(
     name='autoplot',
-    version='0.6.1',
+    version='0.6.2',
     author='Jeremy Faden',
     author_email='faden@cottagesystems.com',
     packages=find_packages(), 
     url='https://github.com/autoplot/python/',
     license='LICENSE.txt',
     description='Interface to Autoplot Java library',
     long_description=open('README.rst').read(),
```

