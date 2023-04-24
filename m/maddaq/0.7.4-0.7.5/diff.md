# Comparing `tmp/maddaq-0.7.4.tar.gz` & `tmp/maddaq-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.4.tar", last modified: Sat Apr 22 09:47:25 2023, max compression
+gzip compressed data, was "maddaq-0.7.5.tar", last modified: Mon Apr 24 11:18:08 2023, max compression
```

## Comparing `maddaq-0.7.4.tar` & `maddaq-0.7.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.716365 maddaq-0.7.4/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-22 09:47:25.716060 maddaq-0.7.4/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.4/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.709880 maddaq-0.7.4/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.4/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.4/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.4/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.4/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.4/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-22 09:45:49.000000 maddaq-0.7.4/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.715549 maddaq-0.7.4/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.4/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.4/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.4/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.4/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-22 09:37:21.000000 maddaq-0.7.4/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.4/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.4/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-22 09:47:25.712659 maddaq-0.7.4/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-22 09:47:25.000000 maddaq-0.7.4/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-22 09:45:49.000000 maddaq-0.7.4/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-22 09:47:25.716508 maddaq-0.7.4/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.080302 maddaq-0.7.5/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-24 11:18:08.079809 maddaq-0.7.5/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.5/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.073951 maddaq-0.7.5/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.5/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.5/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.5/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.5/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.5/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-24 11:13:35.000000 maddaq-0.7.5/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.079262 maddaq-0.7.5/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.5/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.5/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.5/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.5/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     6170 2023-04-24 11:10:08.000000 maddaq-0.7.5/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.5/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.5/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-24 11:18:08.076372 maddaq-0.7.5/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-24 11:18:08.000000 maddaq-0.7.5/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-24 11:13:35.000000 maddaq-0.7.5/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-24 11:18:08.080406 maddaq-0.7.5/setup.cfg
```

### Comparing `maddaq-0.7.4/PKG-INFO` & `maddaq-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.4
+Version: 0.7.5
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.4/README.md` & `maddaq-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/GTimer.py` & `maddaq-0.7.5/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/MadDAQData.py` & `maddaq-0.7.5/maddaq/MadDAQData.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/MadDAQModule.py` & `maddaq-0.7.5/maddaq/MadDAQModule.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/Progress.py` & `maddaq-0.7.5/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/ScanManager.py` & `maddaq-0.7.5/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.5/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/cmmds/file_info.py` & `maddaq-0.7.5/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.5/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.5/maddaq/cmmds/getSpectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,79 +82,88 @@
         md.noise,
         axis_title="Noise",
         x_label="Channel"
     )
     print("Noise mean {:.1f} std {:.1f}".format(mnoise, stnoise))
 
 
-def do_getSpectrum(fnam, options):
+def do_getSpectrum(files, options):
     """Main entry."""
-    # Check that the file exists
-    if not os.path.exists(fnam):
-        print("Input file", fnam, "does not exist")
-        return
-
-    # We open here the file with MadDAQData
-    maddaq = MadDAQData(fnam)
-    maddaq.show_info(True)
-
-    # Find the module
-    keys = list(maddaq.modules.keys())
-    if options.mid in keys:
-        mid = options.mid
-    else:
-        mid = keys[0]
-
-    print("\n## Looking at data from module {}.".format(mid))
-    md = maddaq.modules[mid]
-
-    # Show pedeswtals and noise
-    show_pedestals(md)
-
-    # Create the iterator
-    if options.scan_point is not None:
-        maddaq_iter = maddaq.create_iterator_at_scanpoint(options.scan_point, [mid])
-    elif options.start_time is not None:
-        maddaq_iter = maddaq.create_iterator_at_time(options.start_time, [mid])
-    elif options.start_evt is not None:
-        maddaq_iter = maddaq.create_iterator_at_event(options.start_evt, [mid])
-    else:
-        maddaq_iter = maddaq.create_module_iterator(md)
-
-    amplitude = []
-    prg = ShowProgress(maddaq.nevts, width=24)
-    prg.start()
-
-    for evt in maddaq_iter:
-        data = md.process_event(evt)
-        if data is not None:
-            for C, E in data:
-                if E > options.thrs:
-                    amplitude.append(E)
+    
+    amplitudes = []
+    for fnam in files:
+        # Check that the file exists
+        if not os.path.exists(fnam):
+            print("Input file", fnam, "does not exist")
+            continue
+        
+        # We open here the file with MadDAQData
+        maddaq = MadDAQData(fnam)
+        maddaq.show_info(True)
+
+        # Find the module
+        keys = list(maddaq.modules.keys())
+        if options.mid in keys:
+            mid = options.mid
+        else:
+            mid = keys[0]
 
-        prg.increase(show=True)
+        print("\n## Looking at data from module {}.".format(mid))
+        md = maddaq.modules[mid]
 
-    prg.stop()
-    print("")
-    # Draw the signal
-    fig, ax = plt.subplots(1, 1)
-    n, bins, *_ = ax.hist(amplitude, bins=options.nbin)
-    mean = np.mean(amplitude)
-    std = np.std(amplitude)
-    if options.fit:
-        if options.two_peaks:
-            result, out, legend = fit_two_peaks(mean, std, std, n, bins)
+        # Show pedeswtals and noise
+        show_pedestals(md)
 
+        # Create the iterator
+        if options.scan_point is not None:
+            maddaq_iter = maddaq.create_iterator_at_scanpoint(options.scan_point, [mid])
+        elif options.start_time is not None:
+            maddaq_iter = maddaq.create_iterator_at_time(options.start_time, [mid])
+        elif options.start_evt is not None:
+            maddaq_iter = maddaq.create_iterator_at_event(options.start_evt, [mid])
         else:
-            result, out, legend = fit_gaussian(n, bins, mean, width=std)
+            maddaq_iter = maddaq.create_module_iterator(md)
 
-        draw_best_fit(ax, result, bins)
-        ax.legend([legend], loc=1)
+        amplitude = []
+        prg = ShowProgress(maddaq.nevts, width=24)
+        prg.start()
+
+        for evt in maddaq_iter:
+            data = md.process_event(evt)
+            if data is not None:
+                for C, E in data:
+                    if E > options.thrs:
+                        amplitude.append(E)
+
+            prg.increase(show=True)
+
+        amplitudes.append(amplitude)
+        prg.stop()
+        print("")
+        
+    # Draw the signal
+    fig, ax = plt.subplots(1, 1)
+    n, bins, *_ = ax.hist(amplitudes, bins=options.nbin)
+    legends = []
+    if options.fit:
+        for amplitude in amplitudes:
+            mean = np.mean(amplitude)
+            std = np.std(amplitude)
+            if options.two_peaks:
+                result, out, legend = fit_two_peaks(mean, std, std, n, bins)
+
+            else:
+                result, out, legend = fit_gaussian(n, bins, mean, width=std)
+
+            draw_best_fit(ax, result, bins)
+            legends.append(legend)
+            
+        ax.legend(legends, loc=1)
 
-    ax.set_title("Signel Channel signal")
+    ax.set_title("Signal")
     ax.set_xlabel("Charge (ADC)")
     if options.logY:
         ax.set_yscale("log")
 
     plt.show()
 
 
@@ -174,26 +183,26 @@
     parser.add_argument("--start-time", dest="start_time", default=None, type=float,
                         help="Event time to start")
     parser.add_argument("--start-evt", dest="start_evt", default=None,
                         action=CommaSeparatedListAction,
                         help="Event number to start showing")
     parser.add_argument("--scan-point", dest="scan_point", type=int, default=None,
                         help="Scan point number to visit")
-    parser.add_argument("--nbin", default=50, help="Number of bins in histogram.")
+    parser.add_argument("--nbin", default=50, type=int, help="Number of bins in histogram.")
     parser.add_argument("--logY", default=False, action="store_true", help="Log axis")
     parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
     parser.add_argument("--two_peaks", default=False, action="store_true", help="Min E to show in histogram")
     parser.add_argument("--no-fit", dest="fit", default=True, action="store_false")
     parser.add_argument("--mid", dest="mid", default=-1,
                         type=int, help="The module ID")
 
     options = parser.parse_args()
 
     if len(options.files) == 0:
         print("I need an input file")
         sys.exit()
 
-    do_getSpectrum(options.files[0], options)
+    do_getSpectrum(options.files, options)
 
 
 if __name__ == "__main__":
     getSpectrum()
```

### Comparing `maddaq-0.7.4/maddaq/cmmds/read_data.py` & `maddaq-0.7.5/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq/cmmds/show_data.py` & `maddaq-0.7.5/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.5/maddaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.4
+Version: 0.7.5
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.4/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.5/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.4/pyproject.toml` & `maddaq-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

