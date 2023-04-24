# Comparing `tmp/autoplot-0.5.2.tar.gz` & `tmp/autoplot-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplot-0.5.2.tar", last modified: Wed Apr 19 17:08:01 2023, max compression
+gzip compressed data, was "autoplot-0.6.1.tar", last modified: Mon Apr 24 14:24:06 2023, max compression
```

## Comparing `autoplot-0.5.2.tar` & `autoplot-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:08:01.994746 autoplot-0.5.2/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.5.2/LICENSE.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:08:01.994746 autoplot-0.5.2/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1636 2023-04-12 16:42:58.000000 autoplot-0.5.2/README.rst
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:08:01.994746 autoplot-0.5.2/autoplot/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      271 2023-04-19 17:00:38.000000 autoplot-0.5.2/autoplot/__init__.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)    22041 2023-04-19 17:06:47.000000 autoplot-0.5.2/autoplot/autoplot.py
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-19 17:08:01.994746 autoplot-0.5.2/autoplot.egg-info/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2260 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/requires.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-19 17:08:01.000000 autoplot-0.5.2/autoplot.egg-info/top_level.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-19 17:08:01.994746 autoplot-0.5.2/setup.cfg
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-19 17:07:08.000000 autoplot-0.5.2/setup.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:24:06.018203 autoplot-0.6.1/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.6.1/LICENSE.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:24:06.018203 autoplot-0.6.1/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1818 2023-04-24 14:22:53.000000 autoplot-0.6.1/README.rst
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:24:06.018203 autoplot-0.6.1/autoplot/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      310 2023-04-24 14:19:03.000000 autoplot-0.6.1/autoplot/__init__.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)    22169 2023-04-24 14:21:05.000000 autoplot-0.6.1/autoplot/autoplot.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:24:06.018203 autoplot-0.6.1/autoplot.egg-info/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/requires.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-24 14:24:05.000000 autoplot-0.6.1/autoplot.egg-info/top_level.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-24 14:24:06.018203 autoplot-0.6.1/setup.cfg
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-24 14:18:57.000000 autoplot-0.6.1/setup.py
```

### Comparing `autoplot-0.5.2/LICENSE.txt` & `autoplot-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoplot-0.5.2/README.rst` & `autoplot-0.6.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can 
+also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
 Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
 
 Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
 These URIs can be created using the Autoplot application, available at http://autoplot.org/.
 Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-Helper procedures from the autoplot package convert QDataSets into ndarrays.
+Helper procedures from the Autoplot package convert QDataSets into ndarrays.
 
 Autoplot/Python Interface Tools
 -------------------------------
 
 Install using `pip install autoplot`
 
 .. code:: python
 
   from autoplot import *
 
-  # Download autoplot.jar if needed and return Python bridge object
+  # Download autoplot.jar, if needed, and load it into JPype's classpath.
   javaaddpath('http://autoplot.org/latest/autoplot.jar')
   
-  # Create Autoplot Data Set
+  # Create Autoplot Data Set, which is an object that loads and temporarily holds data.
   apds = APDataSet()
 
-  # Set URI
+  # Set URI which will be loaded.
   apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
 
-  # Get the data
+  # Load the data, initially downloading files into Autoplot's cache.
   apds.doGetDataSet()
 
   print(apds.toString())
   # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
   # data: data[dep0=288] (dimensionless)
   # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
 
   # Extract data values
-  vv = to_ndarray(apds, 'data')
+  vv = to_ndarray(apds)
   tt = to_ndarray(apds, 'dep0')
 
   from matplotlib import pyplot as plt
   plt.plot(tt,vv)
   plt.show()
 
 Contact
 -------------------------------
 Jeremy Faden <faden@cottagesystems.com>
 
+See also https://github.com/autoplot/python/wiki
```

### Comparing `autoplot-0.5.2/autoplot/autoplot.py` & `autoplot-0.6.1/autoplot/autoplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import print_function
 
 
 def version():
-    return '0.5.2'
+    return '0.6.1'
 
 
 def printNoNewline(s):
     print(s, end=' ')
 
 
 def javaaddpath(url='', jdwpPort=-1):
@@ -89,18 +89,21 @@
 def APDataSet():
     """create a new container for loading data"""
     import jpype
     clas = jpype.JClass("org.autoplot.idlsupport.APDataSet")
     return clas()
 
 
-def to_ndarray(apds, name):
-    """extract the data identified by name to numpy array, using datetime64 for times."""
+def to_ndarray(apds, name=None):
+    """extract the data identified by name to numpy array, using datetime64 for times.  If name is empty or not specified, then
+    the default dataset is returned."""
     import numpy as np
     import jpype
+    if name==None:
+        name= apds.name()
     Units = jpype.JClass('org.das2.datum.Units')
     apds.setPreferredUnits('microseconds since 2000-01-01T00:00')
     u = Units.lookupUnits(apds.propertyAsString(name, 'UNITS'))
     if u.isConvertibleTo(Units.us2000):
         g_base = np.datetime64('2000-01-01T00:00:00Z')
         dd = apds.values(name)
         result = np.array([g_base + np.timedelta64(int(dd[i]*1000), 'ns') for i in range(len(dd))])
@@ -147,15 +150,15 @@
         xds = to_qdataset(X)
         yds = to_qdataset(Y)
         zds = to_qdataset(Z)
         return link(xds, yds, zds)
 
 
 def show_completions( s ):
-    'print completions for the given URI.'
+    "print completions for the given URI."
     import jpype
     sc = jpype.JClass('org.autoplot.ScriptContext')
     xxs = sc.getCompletions(s)
     for x in xxs:
         print(x)
```

### Comparing `autoplot-0.5.2/setup.py` & `autoplot-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = ["jpype1","numpy"]
 
 if sys.argv[1] == 'develop':
     install_requires.append("pytest")
 
 setup(
     name='autoplot',
-    version='0.5.2',
+    version='0.6.1',
     author='Jeremy Faden',
     author_email='faden@cottagesystems.com',
     packages=find_packages(), 
     url='https://github.com/autoplot/python/',
     license='LICENSE.txt',
     description='Interface to Autoplot Java library',
     long_description=open('README.rst').read(),
```

