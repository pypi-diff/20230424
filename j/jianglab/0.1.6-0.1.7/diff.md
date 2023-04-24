# Comparing `tmp/jianglab-0.1.6.tar.gz` & `tmp/jianglab-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.1.6.tar", last modified: Mon Apr 24 15:35:55 2023, max compression
+gzip compressed data, was "jianglab-0.1.7.tar", last modified: Mon Apr 24 16:31:26 2023, max compression
```

## Comparing `jianglab-0.1.6.tar` & `jianglab-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 15:35:55.501066 jianglab-0.1.6/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 15:35:55.500741 jianglab-0.1.6/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.1.6/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 15:35:55.497844 jianglab-0.1.6/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.6/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)     3517 2023-04-24 15:35:39.000000 jianglab-0.1.6/jianglab/common_functions.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 15:35:55.499974 jianglab-0.1.6/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       52 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-24 15:35:55.000000 jianglab-0.1.6/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-24 15:35:55.501194 jianglab-0.1.6/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      813 2023-04-24 15:35:49.000000 jianglab-0.1.6/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 16:31:26.507375 jianglab-0.1.7/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 16:31:26.507104 jianglab-0.1.7/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.1.7/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 16:31:26.504789 jianglab-0.1.7/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.7/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     5590 2023-04-24 16:30:31.000000 jianglab-0.1.7/jianglab/common_functions.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 16:31:26.506640 jianglab-0.1.7/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       52 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-24 16:31:26.000000 jianglab-0.1.7/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-24 16:31:26.507530 jianglab-0.1.7/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      813 2023-04-24 16:30:47.000000 jianglab-0.1.7/setup.py
```

### Comparing `jianglab-0.1.6/README.md` & `jianglab-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.1.6/jianglab/common_functions.py` & `jianglab-0.1.7/jianglab/common_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,63 @@
 import os
 from treelib import Tree, Node 
 import numpy as np
 import McsPy.McsCMOSMEA as McsCMOSMEA
 from tqdm import tqdm
 
 def load_light_ref(filepath, sampling_rate=2000):
+    ''' load light reference from .cmcr file
+    filepath: path to the .cmcr or .cmtr file
+    sampling_rate: sampling rate of the light reference
+    '''
     raw_data = McsCMOSMEA.McsData(filepath)
     light_ref = raw_data.Acquisition.Analog_Data.ChannelData_1[:,::sampling_rate]
     return light_ref
 
 def load_raw_data(filepath):
+    ''' load raw data from .cmcr or .cmtr file
+    filepath: path to the .cmcr or .cmtr file'''
     raw_data = McsCMOSMEA.McsData(filepath)
     return raw_data
 
-def import_cmtr(filename):
+def import_cmtr_firing_rate(filename, bin_size = 100): 
+    """Import a .cmtr file and return a dictionary of units holding the timestamps and waveforms.
+    :param filename: The path to the .cmtr file.
+    :return: A dictionary of units holding the timestamps and waveforms.
+
+    Note: 
+    1. This function is used for GUI, where is named as import_cmtr_gui
+    2. interval is set to 100ms, which is 10Hz
+    3. Time scale of timestamps is in nanoseconds and bin_size is defined in milliseconds
+    """
+    all_units = {}
+    processed = McsCMOSMEA.McsData(filename)
+
+    def event_rate_in_interval(timestamps, length, interval):
+        bins = np.arange(0, length, interval)
+        hist, _ = np.histogram(timestamps, bins=bins)
+        event_rate = hist / interval *1_000_000
+        return event_rate
+
+    for unit in tqdm(range(processed.Spike_Sorter.Units.shape[0])):
+        data = eval("np.array(processed.Spike_Sorter.Unit_" + str(unit+1)+".get_peaks_timestamps())")
+        data = event_rate_in_interval(data, length = processed.attributes["LB.RecordingDuration"], interval=bin_size * 1000) # 100ms interval, 10 hz
+        col = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Column']")
+        row = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Row']")
+        waveform = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".get_peaks_cutouts().T.mean(axis=1)")
+        all_units[str(unit+1)] = {"unitID": unit+1, "data": data, "col": col, "row": row, \
+            "waveform": waveform, "filename": filename, "globalID": -1}
+    return all_units
+
+
+def import_cmtr_raw(filename):
+    """Import a .cmtr file and return a list of units holding the timestamps and waveforms.
+    :param filename: The path to the .cmtr file.
+    :return: A list of units holding the timestamps and waveforms.
+    """
     all_units = {"units_data":[], "meta_data":[]}
     processed = McsCMOSMEA.McsData(filename)
     for unit in tqdm(range(processed.Spike_Sorter.Units.shape[0])):
         data = eval("np.array(processed.Spike_Sorter.Unit_" + str(unit+1)+".get_peaks_timestamps())")
         col = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Column']")
         row = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Row']")
         waveform = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".get_peaks_cutouts().T.mean(axis=1)")
```

### Comparing `jianglab-0.1.6/setup.py` & `jianglab-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

