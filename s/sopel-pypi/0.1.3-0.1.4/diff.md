# Comparing `tmp/sopel-pypi-0.1.3.tar.gz` & `tmp/sopel-pypi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-pypi-0.1.3.tar", last modified: Tue Nov 15 01:48:46 2022, max compression
+gzip compressed data, was "sopel-pypi-0.1.4.tar", last modified: Mon Apr 24 02:13:29 2023, max compression
```

## Comparing `sopel-pypi-0.1.3.tar` & `sopel-pypi-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-15 01:48:46.778833 sopel-pypi-0.1.3/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-11-14 04:12:10.000000 sopel-pypi-0.1.3/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      109 2022-11-14 04:12:10.000000 sopel-pypi-0.1.3/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)      506 2022-11-15 01:44:11.000000 sopel-pypi-0.1.3/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1566 2022-11-15 01:48:46.778833 sopel-pypi-0.1.3/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)       82 2022-11-14 04:12:10.000000 sopel-pypi-0.1.3/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)      702 2022-11-15 01:48:46.780833 sopel-pypi-0.1.3/setup.cfg
--rw-r--r--   0 dgw       (1000) dgw       (1000)      687 2022-11-14 04:12:10.000000 sopel-pypi-0.1.3/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-15 01:48:46.737332 sopel-pypi-0.1.3/sopel_pypi/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     3668 2022-11-15 01:46:18.000000 sopel-pypi-0.1.3/sopel_pypi/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-15 01:48:46.777833 sopel-pypi-0.1.3/sopel_pypi.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1566 2022-11-15 01:48:46.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      315 2022-11-15 01:48:46.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2022-11-15 01:48:46.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       35 2022-11-15 01:48:46.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/entry_points.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2022-11-14 04:18:29.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/not-zip-safe
--rw-r--r--   0 dgw       (1000) dgw       (1000)       11 2022-11-15 01:48:46.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       11 2022-11-15 01:48:46.000000 sopel-pypi-0.1.3/sopel_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-24 02:13:28.993739 sopel-pypi-0.1.4/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-11-14 04:12:10.000000 sopel-pypi-0.1.4/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      109 2022-11-14 04:12:10.000000 sopel-pypi-0.1.4/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      586 2023-04-22 07:44:54.000000 sopel-pypi-0.1.4/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1710 2023-04-24 02:13:28.994740 sopel-pypi-0.1.4/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       82 2022-11-14 04:12:10.000000 sopel-pypi-0.1.4/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      702 2023-04-24 02:13:29.001740 sopel-pypi-0.1.4/setup.cfg
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      687 2022-11-14 04:12:10.000000 sopel-pypi-0.1.4/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-24 02:13:28.943742 sopel-pypi-0.1.4/sopel_pypi/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     3688 2023-04-22 07:43:03.000000 sopel-pypi-0.1.4/sopel_pypi/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-24 02:13:28.992740 sopel-pypi-0.1.4/sopel_pypi.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1710 2023-04-24 02:13:28.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      315 2023-04-24 02:13:28.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-24 02:13:28.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       35 2023-04-24 02:13:28.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/entry_points.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2022-11-14 04:18:29.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/not-zip-safe
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       11 2023-04-24 02:13:28.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       11 2023-04-24 02:13:28.000000 sopel-pypi-0.1.4/sopel_pypi.egg-info/top_level.txt
```

### Comparing `sopel-pypi-0.1.3/COPYING` & `sopel-pypi-0.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-pypi-0.1.3/PKG-INFO` & `sopel-pypi-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: sopel-pypi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Sopel 7.0+ plugin to show information about linked PyPI packages.
 Home-page: https://github.com/sopel-irc/sopel-pypi
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Description: # sopel-pypi
         
         A Sopel 7.0+ plugin to show information about linked PyPI packages.
         
         
         NEWS
         ====
         
+        Version 0.1.4
+        -------------
+        
+        Fixed:
+        
+        * Package author field can be empty (#4)
+        
+        
         Version 0.1.3
         -------------
         
         Fixed:
         
         * PyPI API changed (#3)
```

### Comparing `sopel-pypi-0.1.3/setup.cfg` & `sopel-pypi-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-pypi
-version = 0.1.3
+version = 0.1.4
 description = A Sopel 7.0+ plugin to show information about linked PyPI packages.
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-pypi
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `sopel-pypi-0.1.3/setup.py` & `sopel-pypi-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-pypi-0.1.3/sopel_pypi/__init__.py` & `sopel-pypi-0.1.4/sopel_pypi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 def format_pypi_info(data):
     """Format a PyPI project data dict for output."""
     template = "{name} {version} | Author: {author} | Released {release_relative} | {summary}"
 
     name = data['info']['name']
     version = data['info']['version']
-    author = data['info']['author']
+    author = data['info']['author'] or '(unknown name)'
     summary = data['info']['summary']
     release_date = get_release_date(data['urls'])
     release_relative = tools.time.seconds_to_human(datetime.utcnow() - release_date)
 
     return template.format(
         name=name,
         version=version,
```

### Comparing `sopel-pypi-0.1.3/sopel_pypi.egg-info/PKG-INFO` & `sopel-pypi-0.1.4/sopel_pypi.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: sopel-pypi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Sopel 7.0+ plugin to show information about linked PyPI packages.
 Home-page: https://github.com/sopel-irc/sopel-pypi
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
 Description: # sopel-pypi
         
         A Sopel 7.0+ plugin to show information about linked PyPI packages.
         
         
         NEWS
         ====
         
+        Version 0.1.4
+        -------------
+        
+        Fixed:
+        
+        * Package author field can be empty (#4)
+        
+        
         Version 0.1.3
         -------------
         
         Fixed:
         
         * PyPI API changed (#3)
```

