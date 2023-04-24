# Comparing `tmp/ghidrecomp-0.3.1.tar.gz` & `tmp/ghidrecomp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghidrecomp-0.3.1.tar", last modified: Mon Apr 24 19:36:07 2023, max compression
+gzip compressed data, was "ghidrecomp-0.3.2.tar", last modified: Mon Apr 24 19:52:16 2023, max compression
```

## Comparing `ghidrecomp-0.3.1.tar` & `ghidrecomp-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.482876 ghidrecomp-0.3.1/ghidrecomp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/decompile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/ghidrecomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/tests/test_gdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/tests/test_ghidrecomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:16.128796 ghidrecomp-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:52:16.128796 ghidrecomp-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:16.124796 ghidrecomp-0.3.2/ghidrecomp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/ghidrecomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/ghidrecomp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/ghidrecomp/decompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/ghidrecomp/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:16.128796 ghidrecomp-0.3.2/ghidrecomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:52:16.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 19:52:16.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:52:16.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 19:52:16.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:52:15.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:52:16.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 19:52:16.000000 ghidrecomp-0.3.2/ghidrecomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 19:52:16.128796 ghidrecomp-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:52:16.128796 ghidrecomp-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/tests/test_gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 19:52:02.000000 ghidrecomp-0.3.2/tests/test_ghidrecomp.py
```

### Comparing `ghidrecomp-0.3.1/LICENSE` & `ghidrecomp-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.1/PKG-INFO` & `ghidrecomp-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.3.1
+Version: 0.3.2
 Summary: A comand line Ghidra Decomplier
 Home-page: https://github.com/clearbluejar/ghidrecomp
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: ghidra,decompiler,callgraph
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.1 Summary: A comand line
+Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.2 Summary: A comand line
 Ghidra Decomplier Home-page: https://github.com/clearbluejar/ghidrecomp Author:
 clearbluejar Author-email: clearbluejar@clearbluejar.com License: GPL-3.0
 license Keywords: ghidra,decompiler,callgraph Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ghidrecomp-0.3.1/README.md` & `ghidrecomp-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.1/ghidrecomp/decompile.py` & `ghidrecomp-0.3.2/ghidrecomp/decompile.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,16 @@
     launcher = HeadlessPyhidraLauncher(True)
 
     # set max % of host RAM
     launcher.add_vmargs(f'-XX:MaxRAMPercentage={args.max_ram_percent}')
     if args.print_flags:
         launcher.add_vmargs('-XX:+PrintFlagsFinal')
 
+    launcher.start()
+
     with open_program(bin_path, project_location=project_location, project_name=bin_path.name, analyze=False) as flat_api:
 
         from ghidra.util.task import ConsoleTaskMonitor
         from ghidra.program.model.listing import Program
         monitor = ConsoleTaskMonitor()
 
         program: "Program" = flat_api.getCurrentProgram()
```

### Comparing `ghidrecomp-0.3.1/ghidrecomp/utility.py` & `ghidrecomp-0.3.2/ghidrecomp/utility.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.1/ghidrecomp.egg-info/PKG-INFO` & `ghidrecomp-0.3.2/ghidrecomp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.3.1
+Version: 0.3.2
 Summary: A comand line Ghidra Decomplier
 Home-page: https://github.com/clearbluejar/ghidrecomp
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: ghidra,decompiler,callgraph
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.1 Summary: A comand line
+Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.2 Summary: A comand line
 Ghidra Decomplier Home-page: https://github.com/clearbluejar/ghidrecomp Author:
 clearbluejar Author-email: clearbluejar@clearbluejar.com License: GPL-3.0
 license Keywords: ghidra,decompiler,callgraph Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ghidrecomp-0.3.1/setup.cfg` & `ghidrecomp-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.1/tests/test_gdt.py` & `ghidrecomp-0.3.2/tests/test_gdt.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.1/tests/test_ghidrecomp.py` & `ghidrecomp-0.3.2/tests/test_ghidrecomp.py`

 * *Files identical despite different names*

