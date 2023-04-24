# Comparing `tmp/bgdiscovery-0.9.5.tar.gz` & `tmp/bgdiscovery-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgdiscovery-0.9.5.tar", last modified: Mon Apr 24 09:03:30 2023, max compression
+gzip compressed data, was "bgdiscovery-0.9.6.tar", last modified: Mon Apr 24 09:04:57 2023, max compression
```

## Comparing `bgdiscovery-0.9.5.tar` & `bgdiscovery-0.9.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:03:30.275303 bgdiscovery-0.9.5/
--rw-rw-rw-   0        0        0     2325 2023-04-24 09:03:30.273308 bgdiscovery-0.9.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 09:03:30.271323 bgdiscovery-0.9.5/bgdiscovery.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-04-24 09:03:30.000000 bgdiscovery-0.9.5/bgdiscovery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-04-24 09:03:30.000000 bgdiscovery-0.9.5/bgdiscovery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:03:30.000000 bgdiscovery-0.9.5/bgdiscovery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-24 09:03:30.000000 bgdiscovery-0.9.5/bgdiscovery.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-04-24 09:03:30.000000 bgdiscovery-0.9.5/bgdiscovery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 09:03:30.000000 bgdiscovery-0.9.5/bgdiscovery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 09:03:30.275303 bgdiscovery-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     3340 2023-04-17 06:44:31.000000 bgdiscovery-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:04:57.471576 bgdiscovery-0.9.6/
+-rw-rw-rw-   0        0        0     2325 2023-04-24 09:04:57.470577 bgdiscovery-0.9.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 09:04:57.468715 bgdiscovery-0.9.6/bgdiscovery.egg-info/
+-rw-rw-rw-   0        0        0     2325 2023-04-24 09:04:57.000000 bgdiscovery-0.9.6/bgdiscovery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-24 09:04:57.000000 bgdiscovery-0.9.6/bgdiscovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:04:57.000000 bgdiscovery-0.9.6/bgdiscovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-24 09:04:57.000000 bgdiscovery-0.9.6/bgdiscovery.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-04-24 09:04:57.000000 bgdiscovery-0.9.6/bgdiscovery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 09:04:57.000000 bgdiscovery-0.9.6/bgdiscovery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:04:57.471576 bgdiscovery-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     3340 2023-04-17 06:44:31.000000 bgdiscovery-0.9.6/setup.py
```

### Comparing `bgdiscovery-0.9.5/PKG-INFO` & `bgdiscovery-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgdiscovery
-Version: 0.9.5
+Version: 0.9.6
 Summary: biGENIUS Discovery App.
 Home-page: https://www.bigenius.info/
 Author: biGENIUS AG
 Author-email: gergely.szecsenyi@bigenius.info
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `bgdiscovery-0.9.5/bgdiscovery.egg-info/PKG-INFO` & `bgdiscovery-0.9.6/bgdiscovery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgdiscovery
-Version: 0.9.5
+Version: 0.9.6
 Summary: biGENIUS Discovery App.
 Home-page: https://www.bigenius.info/
 Author: biGENIUS AG
 Author-email: gergely.szecsenyi@bigenius.info
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `bgdiscovery-0.9.5/setup.py` & `bgdiscovery-0.9.6/setup.py`

 * *Files identical despite different names*

