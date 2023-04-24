# Comparing `tmp/count-sats-0.0.1.tar.gz` & `tmp/count-sats-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "count-sats-0.0.1.tar", last modified: Mon Apr 24 00:50:47 2023, max compression
+gzip compressed data, was "count-sats-0.0.2.tar", last modified: Mon Apr 24 00:54:58 2023, max compression
```

## Comparing `count-sats-0.0.1.tar` & `count-sats-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:50:47.221187 count-sats-0.0.1/
--rw-r--r--   0 nicholasprowse   (501) staff       (20)    35148 2023-04-22 07:36:46.000000 count-sats-0.0.1/LICENSE
--rw-r--r--   0 nicholasprowse   (501) staff       (20)       56 2023-04-24 00:44:48.000000 count-sats-0.0.1/MANIFEST.in
--rw-r--r--   0 nicholasprowse   (501) staff       (20)     1036 2023-04-24 00:50:47.221032 count-sats-0.0.1/PKG-INFO
--rw-r--r--   0 nicholasprowse   (501) staff       (20)      473 2023-04-24 00:43:08.000000 count-sats-0.0.1/README.md
-drwxr-xr-x   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:50:47.219828 count-sats-0.0.1/count_sats.egg-info/
--rw-r--r--   0 nicholasprowse   (501) staff       (20)     1036 2023-04-24 00:50:47.000000 count-sats-0.0.1/count_sats.egg-info/PKG-INFO
--rw-r--r--   0 nicholasprowse   (501) staff       (20)      325 2023-04-24 00:50:47.000000 count-sats-0.0.1/count_sats.egg-info/SOURCES.txt
--rw-r--r--   0 nicholasprowse   (501) staff       (20)        1 2023-04-24 00:50:47.000000 count-sats-0.0.1/count_sats.egg-info/dependency_links.txt
--rw-r--r--   0 nicholasprowse   (501) staff       (20)       57 2023-04-24 00:50:47.000000 count-sats-0.0.1/count_sats.egg-info/entry_points.txt
--rw-r--r--   0 nicholasprowse   (501) staff       (20)       17 2023-04-24 00:50:47.000000 count-sats-0.0.1/count_sats.egg-info/requires.txt
--rw-r--r--   0 nicholasprowse   (501) staff       (20)       12 2023-04-24 00:50:47.000000 count-sats-0.0.1/count_sats.egg-info/top_level.txt
-drwxr-xr-x   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:50:47.220432 count-sats-0.0.1/sat_counter/
--rw-r--r--   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:39:53.000000 count-sats-0.0.1/sat_counter/__init__.py
--rwxr-xr-x   0 nicholasprowse   (501) staff       (20)     2561 2023-04-24 00:40:13.000000 count-sats-0.0.1/sat_counter/__main__.py
--rw-r--r--   0 nicholasprowse   (501) staff       (20)    30687 2023-04-12 08:58:49.000000 count-sats-0.0.1/sat_counter/pizza_sat_ranges.txt
--rw-r--r--   0 nicholasprowse   (501) staff       (20)       38 2023-04-24 00:50:47.221231 count-sats-0.0.1/setup.cfg
--rw-r--r--   0 nicholasprowse   (501) staff       (20)     1086 2023-04-24 00:46:52.000000 count-sats-0.0.1/setup.py
+drwxr-xr-x   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:54:58.287459 count-sats-0.0.2/
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)    35148 2023-04-22 07:36:46.000000 count-sats-0.0.2/LICENSE
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)       56 2023-04-24 00:44:48.000000 count-sats-0.0.2/MANIFEST.in
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)     1034 2023-04-24 00:54:58.287330 count-sats-0.0.2/PKG-INFO
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)      473 2023-04-24 00:43:08.000000 count-sats-0.0.2/README.md
+drwxr-xr-x   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:54:58.286274 count-sats-0.0.2/count_sats.egg-info/
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)     1034 2023-04-24 00:54:58.000000 count-sats-0.0.2/count_sats.egg-info/PKG-INFO
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)      325 2023-04-24 00:54:58.000000 count-sats-0.0.2/count_sats.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)        1 2023-04-24 00:54:58.000000 count-sats-0.0.2/count_sats.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)       57 2023-04-24 00:54:58.000000 count-sats-0.0.2/count_sats.egg-info/entry_points.txt
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)       17 2023-04-24 00:54:58.000000 count-sats-0.0.2/count_sats.egg-info/requires.txt
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)       12 2023-04-24 00:54:58.000000 count-sats-0.0.2/count_sats.egg-info/top_level.txt
+drwxr-xr-x   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:54:58.286806 count-sats-0.0.2/sat_counter/
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)        0 2023-04-24 00:39:53.000000 count-sats-0.0.2/sat_counter/__init__.py
+-rwxr-xr-x   0 nicholasprowse   (501) staff       (20)     2561 2023-04-24 00:40:13.000000 count-sats-0.0.2/sat_counter/__main__.py
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)    30687 2023-04-12 08:58:49.000000 count-sats-0.0.2/sat_counter/pizza_sat_ranges.txt
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)       38 2023-04-24 00:54:58.287498 count-sats-0.0.2/setup.cfg
+-rw-r--r--   0 nicholasprowse   (501) staff       (20)     1084 2023-04-24 00:54:47.000000 count-sats-0.0.2/setup.py
```

### Comparing `count-sats-0.0.1/LICENSE` & `count-sats-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `count-sats-0.0.1/PKG-INFO` & `count-sats-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: count-sats
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool to help with isolating rare/exotic BTC sats
 Author: Vannix
 License: GNU General Public License v3.0
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sat counter
 
 Given a BTC UTXO, finds any sats that are not common, early, or from the pizza transaction and gives the number of sats
 before that for the purposes of isolating the sat.
```

### Comparing `count-sats-0.0.1/count_sats.egg-info/PKG-INFO` & `count-sats-0.0.2/count_sats.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: count-sats
-Version: 0.0.1
+Version: 0.0.2
 Summary: Command line tool to help with isolating rare/exotic BTC sats
 Author: Vannix
 License: GNU General Public License v3.0
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sat counter
 
 Given a BTC UTXO, finds any sats that are not common, early, or from the pizza transaction and gives the number of sats
 before that for the purposes of isolating the sat.
```

### Comparing `count-sats-0.0.1/sat_counter/__main__.py` & `count-sats-0.0.2/sat_counter/__main__.py`

 * *Files identical despite different names*

### Comparing `count-sats-0.0.1/sat_counter/pizza_sat_ranges.txt` & `count-sats-0.0.2/sat_counter/pizza_sat_ranges.txt`

 * *Files identical despite different names*

### Comparing `count-sats-0.0.1/setup.py` & `count-sats-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='count-sats',
-    version='0.0.1',
+    version='0.0.2',
     author='Vannix',
     license='GNU General Public License v3.0',
     description='Command line tool to help with isolating rare/exotic BTC sats',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=['sat_counter'],
     packages=find_packages(),
     install_requires=[requirements],
-    python_requires='>=3.11',
+    python_requires='>=3.8',
     classifiers=[
-        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English"
     ],
     entry_points='''
```

