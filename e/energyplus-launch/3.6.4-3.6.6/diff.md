# Comparing `tmp/energyplus_launch-3.6.4.tar.gz` & `tmp/energyplus_launch-3.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.4.tar", last modified: Mon Apr 24 15:05:47 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.6.tar", last modified: Mon Apr 24 17:23:21 2023, max compression
```

## Comparing `energyplus_launch-3.6.4.tar` & `energyplus_launch-3.6.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.163026 energyplus_launch-3.6.4/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.163026 energyplus_launch-3.6.4/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    70664 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.666286 energyplus_launch-3.6.6/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-24 17:23:21.000000 energyplus_launch-3.6.6/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.666286 energyplus_launch-3.6.6/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.670286 energyplus_launch-3.6.6/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70664 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.670286 energyplus_launch-3.6.6/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-24 17:23:21.674286 energyplus_launch-3.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-24 17:23:12.000000 energyplus_launch-3.6.6/setup.py
```

### Comparing `energyplus_launch-3.6.4/LICENSE` & `energyplus_launch-3.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/PKG-INFO` & `energyplus_launch-3.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.4
+Version: 3.6.6
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.4/README.md` & `energyplus_launch-3.6.6/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.6/energyplus_launch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.4
+Version: 3.6.6
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.4/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.6/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/config.py` & `energyplus_launch-3.6.6/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.6/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.6/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.6/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.6/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.6/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.6/eplaunch/interface/frame_main.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.6/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.6/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.6/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.6/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/utilities/version.py` & `energyplus_launch-3.6.6/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/base.py` & `energyplus_launch-3.6.6/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.6/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.6/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.6/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.6/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.6/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.6/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.6/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.4/setup.py` & `energyplus_launch-3.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "eplaunch": ["icons/*.png", "icons/*.ico", "icons/*.icns"],
         "eplaunch.interface": ["resources/*.png"]
     },
     include_package_data=True,
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     author="Jason Glazer and Edwin Lee for the United States Department of Energy",
-    install_requires=['PLAN-Tools>=0.6', 'tkmacosx'],
+    install_requires=['PLAN-Tools>=0.7', 'tkmacosx'],
     entry_points={
         'gui_scripts': [
             'energyplus_launch=eplaunch.tk_runner:main_gui',
         ],
         'console_scripts': [
             'energyplus_launch_configure=eplaunch.configure:configure_cli',
             'energyplus_launch_workflow_tester=eplaunch.workflows.workflow_tester:cli'
```

