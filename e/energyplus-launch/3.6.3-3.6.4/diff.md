# Comparing `tmp/energyplus_launch-3.6.3.tar.gz` & `tmp/energyplus_launch-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.3.tar", last modified: Fri Apr 14 15:30:34 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.4.tar", last modified: Mon Apr 24 15:05:47 2023, max compression
```

## Comparing `energyplus_launch-3.6.3.tar` & `energyplus_launch-3.6.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    69368 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10103 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2063 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.163026 energyplus_launch-3.6.4/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-24 15:05:46.000000 energyplus_launch-3.6.4/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.163026 energyplus_launch-3.6.4/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70664 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-24 15:05:47.167026 energyplus_launch-3.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-24 15:05:39.000000 energyplus_launch-3.6.4/setup.py
```

### Comparing `energyplus_launch-3.6.3/LICENSE` & `energyplus_launch-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/PKG-INFO` & `energyplus_launch-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.3
+Version: 3.6.4
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.3/README.md` & `energyplus_launch-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.4/energyplus_launch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.3
+Version: 3.6.4
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
```

### Comparing `energyplus_launch-3.6.3/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.4/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/config.py` & `energyplus_launch-3.6.4/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.4/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.4/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.4/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.4/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.4/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.4/eplaunch/interface/frame_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from fnmatch import fnmatch
 
 from json import dumps
 from mimetypes import guess_type
 from pathlib import Path
 from platform import system
 from queue import Queue
+from sys import version_info
 
 from subprocess import Popen
 from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, Frame, Label, NSEW, E, VERTICAL, \
     SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, NORMAL, RIGHT, EW, NS, filedialog, \
     ALL, Listbox, Scrollbar, SINGLE, Variable, HORIZONTAL
 from tkinter.ttk import Combobox, PanedWindow as ttkPanedWindow, OptionMenu, LabelFrame
 if system() == 'Darwin':
@@ -68,14 +69,17 @@
             else:
                 print(f"Could not set icon for Windows, expecting to find it at {self.icon_path}")
         fixup_taskbar_icon_on_windows(NAME)
         self.pad = {'padx': 3, 'pady': 3}
         self.dd_only_string = '<No_Weather_File>'  # Can we change to just using blank?  It's fine for now.
         self.generic_dialogs = TkGenericDialog(self.pad)
 
+        # check the version of python for whether we can show extended UTF characters
+        self.extended_utf8 = version_info >= (3, 7, 6)
+
         # initialize variables which will track output dialogs
         self.dialog_counter: int = 0
         self.output_dialogs: Dict[str, TkOutputDialog] = {}
 
         # create a config manager and load up the saved, or default, configuration
         self.conf = ConfigManager()
         self.conf.load()
@@ -243,42 +247,63 @@
         self.option_workflow_instance = OptionMenu(lf, self._tk_var_workflow_instance, '<instance>')
         self.option_workflow_instance.grid(row=1, column=1, sticky=EW, **self.pad)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=0, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Run Workflow on...")
-        b = Button(lf, text=u"\U000025B6 Selected File(s)", command=self._run_workflow_on_selection, state=NORMAL)
+        if self.extended_utf8:
+            b = Button(lf, text=u"\U000025B6 Selected File(s)", command=self._run_workflow_on_selection, state=NORMAL)
+        else:
+            b = Button(lf, text="Selected File(s)", command=self._run_workflow_on_selection, state=NORMAL)
         b.grid(row=0, column=0, sticky=EW, **self.pad)
-        b = Button(lf, text=u"\U000025B6 Current Group", command=self._run_workflow_on_group, state=NORMAL)
+        if self.extended_utf8:
+            b = Button(lf, text=u"\U000025B6 Current Group", command=self._run_workflow_on_group, state=NORMAL)
+        else:
+            b = Button(lf, text="Current Group", command=self._run_workflow_on_group, state=NORMAL)
         b.grid(row=1, column=0, sticky=EW, **self.pad)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=1, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Weather Selection")
         Label(lf, text="Recent: ", justify=RIGHT).grid(row=0, column=0, **self.pad)
         self.option_weather_recent = OptionMenu(lf, self._tk_var_weather_recent, '<weather>')
         self.option_weather_recent.grid(row=0, column=1, sticky=EW, **self.pad)
-        self.button_weather_select = Button(
-            lf, text=u"\U0001f325 Select Weather File...", command=self._open_weather_dialog
-        )
+        if self.extended_utf8:
+            self.button_weather_select = Button(
+                lf, text=u"\U0001f325 Select Weather File...", command=self._open_weather_dialog
+            )
+        else:
+            self.button_weather_select = Button(
+                lf, text="Select Weather File...", command=self._open_weather_dialog
+            )
         self.button_weather_select.grid(row=1, column=0, columnspan=2, sticky=EW, **self.pad)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=2, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Quicklinks")
-        self.button_open_in_text = Button(
-            lf, text=u"\U0001F5B9 Open File in Text Editor", command=self._open_text_editor, state=DISABLED
-        )
+        if self.extended_utf8:
+            self.button_open_in_text = Button(
+                lf, text=u"\U0001F5B9 Open File in Text Editor", command=self._open_text_editor, state=DISABLED
+            )
+        else:
+            self.button_open_in_text = Button(
+                lf, text="Open File in Text Editor", command=self._open_text_editor, state=DISABLED
+            )
         self.button_open_in_text.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
-        Button(
-            lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser, state=NORMAL
-        ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        if self.extended_utf8:
+            Button(
+                lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser, state=NORMAL
+            ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        else:
+            Button(
+                lf, text="Open Dir in File Browser", command=self._open_file_browser, state=NORMAL
+            ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=3, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Open Outputs")
         sub_frame = Frame(lf)
         self.button_open_output_1 = Button(
@@ -304,15 +329,18 @@
         sub_frame.grid_columnconfigure(ALL, weight=1)
         sub_frame.grid_rowconfigure(ALL, weight=1)
         sub_frame.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
         Label(lf, text="Full List: ", justify=RIGHT).grid(row=1, column=0, **self.pad)
         self.option_workflow_outputs = Combobox(lf, textvariable=self._tk_var_output_suffix)
         self.option_workflow_outputs.grid(row=1, column=1, **self.pad)
         self.option_workflow_outputs['state'] = 'readonly'
-        self.button_open_output_file = Button(lf, text=u"\U0001f325 Open", command=self._open_output_file)
+        if self.extended_utf8:
+            self.button_open_output_file = Button(lf, text=u"\U0001f325 Open", command=self._open_output_file)
+        else:
+            self.button_open_output_file = Button(lf, text="Open", command=self._open_output_file)
         self.button_open_output_file.grid(row=1, column=2, **self.pad)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid(row=0, column=4, sticky=NS, **self.pad)
 
     def _build_listings(self, container: Frame):
         # use vertical for the primary paned window
```

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.4/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.4/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.4/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.4/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/utilities/version.py` & `energyplus_launch-3.6.4/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/base.py` & `energyplus_launch-3.6.4/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.4/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.4/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.4/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.4/eplaunch/workflows/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,31 +25,39 @@
     def workflow_instances(self, workflow_context: str) -> List[Workflow]:
         return [x for x in self.workflows if x.context == workflow_context]
 
     def auto_find_workflow_directories(self) -> None:
         """Locate the (EnergyPlus) workflow directories that are in predestined locations"""
         self.auto_found_workflow_dirs = []
         # then search for e+ workflows
-        search_roots: Dict[int, List[Path]] = {
-            Platform.WINDOWS: [Path(f"{c}:\\") for c in ascii_uppercase],
-            Platform.LINUX: [Path('/usr/local/bin/'), Path('/tmp/')],
-            Platform.MAC: [Path('/Applications/'), Path('/tmp/')],
-            Platform.UNKNOWN: [],
-        }
-        current_search_roots = search_roots[Platform.get_current_platform()]
+        if Platform.get_current_platform() == Platform.WINDOWS:
+            from ctypes import windll
+            bitmask = windll.kernel32.GetLogicalDrives()
+            roots: List[Path] = []
+            for letter in ascii_uppercase:
+                if bitmask & 1:
+                    roots.append(Path(f"{letter}:\\"))
+                bitmask >>= 1
+        elif Platform.get_current_platform() == Platform.LINUX:
+            roots = [Path('/usr/local/bin/'), Path('/tmp/'), Path('/opt')]
+        else:  # Assuming Platform.get_current_platform() == Platform.MAC:
+            roots = [Path('/Applications/'), Path('/tmp/')]
         search_names = ["EnergyPlus*", "EP*", "ep*", "E+*", "e+*"]
         if Platform.get_current_platform() == Platform.LINUX:
             search_names.append("energyplus*")  # add lower case check on case-sensitive file systems (typically Linux)
-        for search_root in current_search_roots:
-            for search_name in search_names:
-                eplus_folder_matches = search_root.glob(search_name)
-                for ep_folder in eplus_folder_matches:  # pragma: no cover, would have to install into system folders
-                    ep_workflow_dir = ep_folder / 'workflows'
-                    if ep_workflow_dir.exists():
-                        self.auto_found_workflow_dirs.append(ep_workflow_dir)
+        for search_root in roots:
+            try:
+                for search_name in search_names:
+                    eplus_folder_matches = search_root.glob(search_name)
+                    for ep_folder in eplus_folder_matches:  # pragma: no cover, would have to install in system folders
+                        ep_workflow_dir = ep_folder / 'workflows'
+                        if ep_workflow_dir.exists():
+                            self.auto_found_workflow_dirs.append(ep_workflow_dir)
+            except PermissionError:  # pragma: no cover -- this could be quite hard to reproduce :)
+                continue  # just skip it, it could be like an empty DVD drive
 
     def instantiate_all_workflows(self, disable_builtins=False, extra_workflow_dir: Optional[Path] = None) -> None:
         this_file_directory_path = Path(__file__).parent.resolve()
         this_project_root_dir = this_file_directory_path.parent
         built_in_workflow_dir = this_project_root_dir / 'workflows' / 'default'
         all_workflow_directories = self.workflow_directories
         if disable_builtins:
```

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.4/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.4/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.4/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.3/setup.py` & `energyplus_launch-3.6.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from pathlib import Path
-from platform import system
 from setuptools import setup
 
 from eplaunch import NAME, VERSION
 
 
 readme_file = Path(__file__).parent.resolve() / 'README.md'
 readme_contents = readme_file.read_text()
 
-install_requires = ['PLAN-Tools>=0.5', 'tkmacosx']
-if system() == 'Windows':
-    install_requires.append('pypiwin32')
-
 setup(
     name=NAME,
     version=VERSION,
     description='Graphical Interface and Workflow Manager for EnergyPlus',
     url='https://github.com/NREL/EP-Launch',
     license='ModifiedBSD',
     packages=[
@@ -25,15 +20,15 @@
         "eplaunch": ["icons/*.png", "icons/*.ico", "icons/*.icns"],
         "eplaunch.interface": ["resources/*.png"]
     },
     include_package_data=True,
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     author="Jason Glazer and Edwin Lee for the United States Department of Energy",
-    install_requires=install_requires,
+    install_requires=['PLAN-Tools>=0.6', 'tkmacosx'],
     entry_points={
         'gui_scripts': [
             'energyplus_launch=eplaunch.tk_runner:main_gui',
         ],
         'console_scripts': [
             'energyplus_launch_configure=eplaunch.configure:configure_cli',
             'energyplus_launch_workflow_tester=eplaunch.workflows.workflow_tester:cli'
```

