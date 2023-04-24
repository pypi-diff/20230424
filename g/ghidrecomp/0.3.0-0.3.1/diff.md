# Comparing `tmp/ghidrecomp-0.3.0.tar.gz` & `tmp/ghidrecomp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghidrecomp-0.3.0.tar", last modified: Mon Apr 24 19:13:20 2023, max compression
+gzip compressed data, was "ghidrecomp-0.3.1.tar", last modified: Mon Apr 24 19:36:07 2023, max compression
```

## Comparing `ghidrecomp-0.3.0.tar` & `ghidrecomp-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.908262 ghidrecomp-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:13:20.908262 ghidrecomp-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.904262 ghidrecomp-0.3.0/ghidrecomp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/decompile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.904262 ghidrecomp-0.3.0/ghidrecomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 19:13:20.908262 ghidrecomp-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.904262 ghidrecomp-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/tests/test_gdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/tests/test_ghidrecomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.482876 ghidrecomp-0.3.1/ghidrecomp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/decompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/ghidrecomp/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/ghidrecomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 19:36:07.000000 ghidrecomp-0.3.1/ghidrecomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:36:07.486876 ghidrecomp-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/tests/test_gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 19:35:50.000000 ghidrecomp-0.3.1/tests/test_ghidrecomp.py
```

### Comparing `ghidrecomp-0.3.0/LICENSE` & `ghidrecomp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.0/PKG-INFO` & `ghidrecomp-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.3.0
+Version: 0.3.1
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
-Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.0 Summary: A comand line
+Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.1 Summary: A comand line
 Ghidra Decomplier Home-page: https://github.com/clearbluejar/ghidrecomp Author:
 clearbluejar Author-email: clearbluejar@clearbluejar.com License: GPL-3.0
 license Keywords: ghidra,decompiler,callgraph Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ghidrecomp-0.3.0/README.md` & `ghidrecomp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.0/ghidrecomp/decompile.py` & `ghidrecomp-0.3.1/ghidrecomp/decompile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from pathlib import Path
 from typing import TYPE_CHECKING
 from argparse import Namespace
 import concurrent.futures
 from time import time
-import pyhidra
+from pyhidra import HeadlessPyhidraLauncher, open_program
 
-from .utility import set_pdb, setup_symbol_server, set_remote_pdbs, analyze_program, apply_gdt
+from .utility import set_pdb, setup_symbol_server, set_remote_pdbs, analyze_program, get_pdb, apply_gdt
 
 # needed for ghidra python vscode autocomplete
 if TYPE_CHECKING:
     import ghidra
     from ghidra_builtins import *
 
 
@@ -31,45 +31,45 @@
 
     return decompilers
 
 
 def decompile_func(func: 'ghidra.program.model.listing.Function',
                    decompilers: dict,
                    thread_id: int = 0,
-                   TIMEOUT: int = 0,
+                   timeout: int = 0,
                    monitor=None) -> list:
     """
     Decompile function and return [funcname, decompilation]
     Ghidra/Features/Decompiler/src/main/java/ghidra/app/util/exporter/CppExporter.java#L514
     """
     MAX_PATH_LEN = 50
     from ghidra.util.task import ConsoleTaskMonitor
     from ghidra.app.decompiler import DecompiledFunction, DecompileResults
 
     if monitor is None:
         monitor = ConsoleTaskMonitor()
 
-    result: "DecompileResults" = decompilers[thread_id].decompileFunction(func, TIMEOUT, monitor)
+    result: "DecompileResults" = decompilers[thread_id].decompileFunction(func, timeout, monitor)
 
     if '' == result.getErrorMessage():
         code = result.decompiledFunction.getC()
         sig = result.decompiledFunction.getSignature()
     else:
         code = result.getErrorMessage()
         sig = None
 
     return [f'{func.getName()[:MAX_PATH_LEN]}-{func.entryPoint}', code, sig]
 
 
 def decompile_to_single_file(path: Path,
                              prog: "ghidra.program.model.listing.Program",
                              create_header: bool = True,
-                             createFile: bool = True,
+                             create_file: bool = True,
                              emit_types: bool = True,
-                             excludeTags: bool = True,
+                             exclude_tags: bool = False,
                              tags: str = None,
                              verbose: bool = True):
     """
     Use Ghidra's CppExporter to decompile all functions to a single file
     """
     from ghidra.app.util.exporter import CppExporter
     from ghidra.util.task import ConsoleTaskMonitor
@@ -78,15 +78,15 @@
     c_file = File(path.absolute())
 
     if verbose:
         monitor = ConsoleTaskMonitor()
     else:
         monitor = ConsoleTaskMonitor().DUMMY
 
-    decompiler = CppExporter(True, True, True, False, None)
+    decompiler = CppExporter(create_header, create_file, emit_types, exclude_tags, tags)
     decompiler.export(c_file, prog, prog.getMemory(), monitor)
 
 
 def decompile(args: Namespace):
 
     print(f'Starting decompliations: {args}')
 
@@ -94,17 +94,22 @@
     project_location = Path(args.project_path)
     thread_count = args.thread_count
 
     output_path = Path(args.output_path) / bin_path.name
     output_path.mkdir(exist_ok=True, parents=True)
 
     # turn on verbose
-    pyhidra.start(True)
+    launcher = HeadlessPyhidraLauncher(True)
 
-    with pyhidra.open_program(bin_path, project_location=project_location, project_name=bin_path.name, analyze=False) as flat_api:
+    # set max % of host RAM
+    launcher.add_vmargs(f'-XX:MaxRAMPercentage={args.max_ram_percent}')
+    if args.print_flags:
+        launcher.add_vmargs('-XX:+PrintFlagsFinal')
+
+    with open_program(bin_path, project_location=project_location, project_name=bin_path.name, analyze=False) as flat_api:
 
         from ghidra.util.task import ConsoleTaskMonitor
         from ghidra.program.model.listing import Program
         monitor = ConsoleTaskMonitor()
 
         program: "Program" = flat_api.getCurrentProgram()
 
@@ -112,16 +117,17 @@
             if args.sym_file_path:
                 set_pdb(program, args.sym_file_path)
             else:
                 setup_symbol_server(args.symbols_path)
 
                 set_remote_pdbs(program, True)
 
-                # pdb = get_pdb(program)
-                # assert pdb is not None
+            pdb = get_pdb(program)
+            if pdb is None:
+                print(f"Failed to find pdb for {program}")
 
         # apply GDT
         if args.gdt:
             for gdt_path in args.gdt:
                 print(f'Applying gdt {gdt_path}...')
                 apply_gdt(program, gdt_path, verbose=args.va)
 
@@ -137,15 +143,16 @@
                 if any([re.search(fil, f.name, re.IGNORECASE) for fil in args.filters]):
                     all_funcs.append(f)
                 else:
                     skip_count += 1
             else:
                 all_funcs.append(f)
 
-        print(f'Skipped {skip_count} functions that failed to match any of {args.filters}')
+        if skip_count > 0:
+            print(f'Skipped {skip_count} functions that failed to match any of {args.filters}')
 
         if args.cppexport:
             print(f"Decompiling {len(all_funcs)} functions using Ghidra's CppExporter")
             c_file = Path(args.output_path) / Path(bin_path.name + '.c')
             start = time()
             decompile_to_single_file(c_file, program)
             print(f'Decompiled {len(all_funcs)} functions for {program.name} in {time() - start}')
```

### Comparing `ghidrecomp-0.3.0/ghidrecomp/utility.py` & `ghidrecomp-0.3.1/ghidrecomp/utility.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.0/ghidrecomp.egg-info/PKG-INFO` & `ghidrecomp-0.3.1/ghidrecomp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.3.0
+Version: 0.3.1
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
-Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.0 Summary: A comand line
+Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.1 Summary: A comand line
 Ghidra Decomplier Home-page: https://github.com/clearbluejar/ghidrecomp Author:
 clearbluejar Author-email: clearbluejar@clearbluejar.com License: GPL-3.0
 license Keywords: ghidra,decompiler,callgraph Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ghidrecomp-0.3.0/setup.cfg` & `ghidrecomp-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.0/tests/test_gdt.py` & `ghidrecomp-0.3.1/tests/test_gdt.py`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.3.0/tests/test_ghidrecomp.py` & `ghidrecomp-0.3.1/tests/test_ghidrecomp.py`

 * *Files identical despite different names*

