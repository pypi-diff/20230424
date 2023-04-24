# Comparing `tmp/gkligo-0.0.3.tar.gz` & `tmp/gkligo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.0.3.tar", last modified: Mon Apr 24 12:56:05 2023, max compression
+gzip compressed data, was "gkligo-0.0.4.tar", last modified: Mon Apr 24 13:32:09 2023, max compression
```

## Comparing `gkligo-0.0.3.tar` & `gkligo-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.683825 gkligo-0.0.3/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.3/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.3/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 12:56:05.683273 gkligo-0.0.3/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.3/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.671709 gkligo-0.0.3/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.3/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-24 12:30:42.000000 gkligo-0.0.3/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.676018 gkligo-0.0.3/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.3/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.682247 gkligo-0.0.3/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.3/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.3/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.3/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      520 2023-04-24 12:50:32.000000 gkligo-0.0.3/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     8993 2023-04-24 09:27:27.000000 gkligo-0.0.3/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     4922 2023-04-18 21:48:34.000000 gkligo-0.0.3/gkligo/scripts/python/generateGWReports.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2538 2023-04-20 14:57:17.000000 gkligo-0.0.3/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 12:56:05.675170 gkligo-0.0.3/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       71 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-24 12:56:05.000000 gkligo-0.0.3/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-24 12:56:05.684045 gkligo-0.0.3/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1281 2023-04-24 12:38:44.000000 gkligo-0.0.3/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.395295 gkligo-0.0.4/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.4/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.4/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 13:32:09.394739 gkligo-0.0.4/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.4/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.382921 gkligo-0.0.4/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.4/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-24 13:28:47.000000 gkligo-0.0.4/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.386959 gkligo-0.0.4/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.4/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.393466 gkligo-0.0.4/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.4/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.4/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.4/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      520 2023-04-24 12:50:32.000000 gkligo-0.0.4/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     8993 2023-04-24 09:27:27.000000 gkligo-0.0.4/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     4927 2023-04-24 13:29:46.000000 gkligo-0.0.4/gkligo/scripts/python/generateGWReports.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2538 2023-04-20 14:57:17.000000 gkligo-0.0.4/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.386349 gkligo-0.0.4/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-24 13:32:09.395529 gkligo-0.0.4/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.4/setup.py
```

### Comparing `gkligo-0.0.3/LICENSE` & `gkligo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.3/PKG-INFO` & `gkligo-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.3
+Version: 0.0.4
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.3/README.md` & `gkligo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.3/gkligo/scripts/python/config_reports_example.yaml` & `gkligo-0.0.4/gkligo/scripts/python/config_reports_example.yaml`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.3/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.0.4/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.3/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.0.4/gkligo/scripts/python/generateGWReports.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     opts = cleanOptions(opts)
     options = Struct(**opts)
 
     configFile = options.configfile
 
     import yaml
     with open(configFile) as yaml_file:
-        config = yaml.load(yaml_file)
+        config = yaml.safe_load(yaml_file)
 
     usernameatlas = config['databases']['atlas']['username']
     passwordatlas = config['databases']['atlas']['password']
     databaseatlas = config['databases']['atlas']['database']
     hostnameatlas = config['databases']['atlas']['hostname']
 
     usernameps = config['databases']['ps']['username']
```

### Comparing `gkligo-0.0.3/gkligo/scripts/python/testDaemon.py` & `gkligo-0.0.4/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.3/gkligo.egg-info/PKG-INFO` & `gkligo-0.0.4/gkligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.3
+Version: 0.0.4
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.3/gkligo.egg-info/SOURCES.txt` & `gkligo-0.0.4/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.3/setup.py` & `gkligo-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,13 +34,14 @@
           'gkutils',
           'docopt',
           'numpy',
           'ligo.skymap',
           'astropy',
           'mocpy',
           'pyYAML',
+          'python-daemon',
       ],
     python_requires='>=3.7',
     entry_points = {
         'console_scripts': ['downloadGWAlerts=gkligo.scripts.python.downloadGWAlerts:main','generateGWReports=gkligo.scripts.python.generateGWReports:main'],
     },
 )
```

