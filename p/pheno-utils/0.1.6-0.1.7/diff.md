# Comparing `tmp/pheno-utils-0.1.6.tar.gz` & `tmp/pheno-utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.1.6.tar", last modified: Mon Apr 24 07:18:35 2023, max compression
+gzip compressed data, was "pheno-utils-0.1.7.tar", last modified: Mon Apr 24 09:30:34 2023, max compression
```

## Comparing `pheno-utils-0.1.6.tar` & `pheno-utils-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 07:18:35.397408 pheno-utils-0.1.6/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.6/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.6/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-24 07:18:35.397005 pheno-utils-0.1.6/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.6/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 07:18:35.391991 pheno-utils-0.1.6/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)      328 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13667 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/basic_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/cgm_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    17037 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/dates_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/ecg_analysis.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-24 07:03:40.000000 pheno-utils-0.1.6/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 07:18:35.396354 pheno-utils-0.1.6/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      625 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.6/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-24 07:18:35.000000 pheno-utils-0.1.6/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-24 07:03:30.000000 pheno-utils-0.1.6/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-24 07:18:35.397578 pheno-utils-0.1.6/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.6/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 09:30:34.794911 pheno-utils-0.1.7/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.1.7/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.1.7/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-24 09:30:34.794462 pheno-utils-0.1.7/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.1.7/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 09:30:34.787433 pheno-utils-0.1.7/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)      328 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13907 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     5300 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/basic_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2789 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     7865 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/cgm_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     3599 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    17037 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/dates_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2113 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    13210 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/sleep_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)      808 2023-04-24 09:28:12.000000 pheno-utils-0.1.7/pheno_utils/subset_loader.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-24 09:30:34.793672 pheno-utils-0.1.7/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-24 09:30:34.000000 pheno-utils-0.1.7/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      654 2023-04-24 09:30:34.000000 pheno-utils-0.1.7/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-24 09:30:34.000000 pheno-utils-0.1.7/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-24 09:30:34.000000 pheno-utils-0.1.7/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.1.7/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)      127 2023-04-24 09:30:34.000000 pheno-utils-0.1.7/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-24 09:30:34.000000 pheno-utils-0.1.7/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1068 2023-04-24 09:23:41.000000 pheno-utils-0.1.7/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-24 09:30:34.795116 pheno-utils-0.1.7/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.1.7/setup.py
```

### Comparing `pheno-utils-0.1.6/LICENSE` & `pheno-utils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/PKG-INFO` & `pheno-utils-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.6/pheno_utils/_modidx.py` & `pheno-utils-0.1.7/pheno_utils/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,8 +100,10 @@
                                          'pheno_utils.sleep_plots.get_legend_colors': ( 'sleep_plots.html#get_legend_colors',
                                                                                         'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_channels': ( 'sleep_plots.html#plot_channels',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_events': ( 'sleep_plots.html#plot_events',
                                                                                   'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_sleep': ( 'sleep_plots.html#plot_sleep',
-                                                                                 'pheno_utils/sleep_plots.py')}}}
+                                                                                 'pheno_utils/sleep_plots.py')},
+            'pheno_utils.subset_loader': { 'pheno_utils.subset_loader.load_subset': ( 'subset_loader.html#load_subset',
+                                                                                      'pheno_utils/subset_loader.py')}}}
```

### Comparing `pheno-utils-0.1.6/pheno_utils/age_reference_plots.py` & `pheno-utils-0.1.7/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/basic_analysis.py` & `pheno-utils-0.1.7/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/basic_plots.py` & `pheno-utils-0.1.7/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.1.7/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/cgm_plots.py` & `pheno-utils-0.1.7/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/config.py` & `pheno-utils-0.1.7/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/data_loader.py` & `pheno-utils-0.1.7/pheno_utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/dates_plots.py` & `pheno-utils-0.1.7/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/ecg_analysis.py` & `pheno-utils-0.1.7/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils/sleep_plots.py` & `pheno-utils-0.1.7/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.1.6/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.1.7/pheno_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.1.6/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.1.7/pheno_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pheno_utils/blandaltman_plots.py
 pheno_utils/cgm_plots.py
 pheno_utils/config.py
 pheno_utils/data_loader.py
 pheno_utils/dates_plots.py
 pheno_utils/ecg_analysis.py
 pheno_utils/sleep_plots.py
+pheno_utils/subset_loader.py
 pheno_utils.egg-info/PKG-INFO
 pheno_utils.egg-info/SOURCES.txt
 pheno_utils.egg-info/dependency_links.txt
 pheno_utils.egg-info/entry_points.txt
 pheno_utils.egg-info/not-zip-safe
 pheno_utils.egg-info/requires.txt
 pheno_utils.egg-info/top_level.txt
```

### Comparing `pheno-utils-0.1.6/settings.ini` & `pheno-utils-0.1.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.1.6
+version = 0.1.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.1.6/setup.py` & `pheno-utils-0.1.7/setup.py`

 * *Files identical despite different names*

