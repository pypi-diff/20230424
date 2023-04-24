# Comparing `tmp/ghidrecomp-0.2.0.tar.gz` & `tmp/ghidrecomp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghidrecomp-0.2.0.tar", last modified: Mon Apr  3 16:41:24 2023, max compression
+gzip compressed data, was "ghidrecomp-0.3.0.tar", last modified: Mon Apr 24 19:13:20 2023, max compression
```

## Comparing `ghidrecomp-0.2.0.tar` & `ghidrecomp-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:41:24.234977 ghidrecomp-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-03 16:41:24.234977 ghidrecomp-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:41:24.230976 ghidrecomp-0.2.0/ghidrecomp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/ghidrecomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/ghidrecomp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/ghidrecomp/decompile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/ghidrecomp/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:41:24.234977 ghidrecomp-0.2.0/ghidrecomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-03 16:41:24.000000 ghidrecomp-0.2.0/ghidrecomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-03 16:41:24.234977 ghidrecomp-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:41:24.234977 ghidrecomp-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-03 16:41:10.000000 ghidrecomp-0.2.0/tests/test_ghidrecomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.908262 ghidrecomp-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:13:20.908262 ghidrecomp-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.904262 ghidrecomp-0.3.0/ghidrecomp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/decompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/ghidrecomp/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.904262 ghidrecomp-0.3.0/ghidrecomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 19:13:20.000000 ghidrecomp-0.3.0/ghidrecomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 19:13:20.908262 ghidrecomp-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:13:20.904262 ghidrecomp-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/tests/test_gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 19:13:06.000000 ghidrecomp-0.3.0/tests/test_ghidrecomp.py
```

### Comparing `ghidrecomp-0.2.0/LICENSE` & `ghidrecomp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.2.0/PKG-INFO` & `ghidrecomp-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.2.0
+Version: 0.3.0
 Summary: A comand line Ghidra Decomplier
 Home-page: https://github.com/clearbluejar/ghidrecomp
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: ghidra,decompiler,callgraph
 Platform: any
@@ -117,41 +117,43 @@
 - Specify the pdb for the binary (`--sym-file-path`)
 - Filter functions to decompile that match regex (`--filter`)
 - Apply custom data types (`--gdt`)
 
 ## Usage
 
 ```
-usage: ghidrecomp [-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [-o OUTPUT_PATH] [-v]
-                  [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-symbols] [-t THREAD_COUNT] [--va] [--max-ram-percent MAX_RAM_PERCENT]
+usage: ghidrecomp [-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [--gdt [GDT]] [-o OUTPUT_PATH] [-v]
+                  [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-symbols] [-t THREAD_COUNT] [--va] [--fa] [--max-ram-percent MAX_RAM_PERCENT]
                   [--print-flags]
                   bin
 
 ghidrecomp - A Command Line Ghidra Decompiler
 
 positional arguments:
   bin                   Path to binary used for analysis
 
 options:
   -h, --help            show this help message and exit
   --cppexport           Use Ghidras CppExporter to decompile to single file (default: False)
   --filter FILTERS      Regex match for function name (default: None)
   --project-path PROJECT_PATH
                         Path to base ghidra projects (default: .ghidra_projects)
+  --gdt [GDT]           Additional GDT to apply (default: None)
   -o OUTPUT_PATH, --output-path OUTPUT_PATH
                         Location for all decompilations (default: decompilations)
   -v, --version         show program's version number and exit
   --sym-file-path SYM_FILE_PATH
                         Specify single pdb symbol file for bin (default: None)
   -s SYMBOLS_PATH, --symbols-path SYMBOLS_PATH
                         Path for local symbols directory (default: .symbols)
   --skip-symbols        Do not apply symbols (default: False)
   -t THREAD_COUNT, --thread-count THREAD_COUNT
                         Threads to use for processing. Defaults to cpu count (default: 8)
   --va                  Enable verbose analysis (default: False)
+  --fa                  Force new analysis (even if already analyzed) (default: False)
 
 JVM Options:
   --max-ram-percent MAX_RAM_PERCENT
                         Set JVM Max Ram % of host RAM (default: 50.0)
   --print-flags         Print JVM flags at start (default: False)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghidrecomp Version: 0.2.0 Summary: A comand line
+Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.0 Summary: A comand line
 Ghidra Decomplier Home-page: https://github.com/clearbluejar/ghidrecomp Author:
 clearbluejar Author-email: clearbluejar@clearbluejar.com License: GPL-3.0
 license Keywords: ghidra,decompiler,callgraph Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -40,33 +40,35 @@
 - Auto-downloaded symbols for supported symbol servers (`-s SYMBOLS_PATH`) -
 https://msdl.microsoft.com/download/symbols/ - https://chromium-browser-
 symsrv.commondatastorage.googleapis.com/ - https://symbols.mozilla.org/ -
 https://software.intel.com/sites/downloads/symbols/ - https://driver-
 symbols.nvidia.com/ - https://download.amd.com/dir/bin/ - Specify the pdb for
 the binary (`--sym-file-path`) - Filter functions to decompile that match regex
 (`--filter`) - Apply custom data types (`--gdt`) ## Usage ``` usage: ghidrecomp
-[-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [-
-o OUTPUT_PATH] [-v] [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-
-symbols] [-t THREAD_COUNT] [--va] [--max-ram-percent MAX_RAM_PERCENT] [--print-
-flags] bin ghidrecomp - A Command Line Ghidra Decompiler positional arguments:
-bin Path to binary used for analysis options: -h, --help show this help message
-and exit --cppexport Use Ghidras CppExporter to decompile to single file
-(default: False) --filter FILTERS Regex match for function name (default: None)
---project-path PROJECT_PATH Path to base ghidra projects (default:
-.ghidra_projects) -o OUTPUT_PATH, --output-path OUTPUT_PATH Location for all
+[-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [--gdt
+[GDT]] [-o OUTPUT_PATH] [-v] [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH |
+--skip-symbols] [-t THREAD_COUNT] [--va] [--fa] [--max-ram-percent
+MAX_RAM_PERCENT] [--print-flags] bin ghidrecomp - A Command Line Ghidra
+Decompiler positional arguments: bin Path to binary used for analysis options:
+-h, --help show this help message and exit --cppexport Use Ghidras CppExporter
+to decompile to single file (default: False) --filter FILTERS Regex match for
+function name (default: None) --project-path PROJECT_PATH Path to base ghidra
+projects (default: .ghidra_projects) --gdt [GDT] Additional GDT to apply
+(default: None) -o OUTPUT_PATH, --output-path OUTPUT_PATH Location for all
 decompilations (default: decompilations) -v, --version show program's version
 number and exit --sym-file-path SYM_FILE_PATH Specify single pdb symbol file
 for bin (default: None) -s SYMBOLS_PATH, --symbols-path SYMBOLS_PATH Path for
 local symbols directory (default: .symbols) --skip-symbols Do not apply symbols
 (default: False) -t THREAD_COUNT, --thread-count THREAD_COUNT Threads to use
 for processing. Defaults to cpu count (default: 8) --va Enable verbose analysis
-(default: False) JVM Options: --max-ram-percent MAX_RAM_PERCENT Set JVM Max Ram
-% of host RAM (default: 50.0) --print-flags Print JVM flags at start (default:
-False) ``` ## Example Usage with Windows afd.sys: ### Command line ```bash wget
-https://msdl.microsoft.com/download/symbols/afd.sys/50989142a9000/afd.sys -
+(default: False) --fa Force new analysis (even if already analyzed) (default:
+False) JVM Options: --max-ram-percent MAX_RAM_PERCENT Set JVM Max Ram % of host
+RAM (default: 50.0) --print-flags Print JVM flags at start (default: False) ```
+## Example Usage with Windows afd.sys: ### Command line ```bash wget https://
+msdl.microsoft.com/download/symbols/afd.sys/50989142a9000/afd.sys -
 O afd.sys.10.0.22621.1415 ghidrecomp afd.sys.10.0.22621.1415 ``` ### Output
 ```bash Starting decompliations: Namespace(bin='tests/data/
 afd.sys.10.0.22621.1344', cppexport=False, filters=None,
 project_path='.ghidra_projects', output_path='decompilations',
 sym_file_path=None, symbols_path='.symbols', skip_symbols=False,
 thread_count=8, va=False) INFO Using log config file: jar:file:/ghidra/Ghidra/
 Framework/Generic/lib/Generic.jar!/generic.log4j.xml (LoggingInitialization)
```

### Comparing `ghidrecomp-0.2.0/README.md` & `ghidrecomp-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -94,41 +94,43 @@
 - Specify the pdb for the binary (`--sym-file-path`)
 - Filter functions to decompile that match regex (`--filter`)
 - Apply custom data types (`--gdt`)
 
 ## Usage
 
 ```
-usage: ghidrecomp [-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [-o OUTPUT_PATH] [-v]
-                  [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-symbols] [-t THREAD_COUNT] [--va] [--max-ram-percent MAX_RAM_PERCENT]
+usage: ghidrecomp [-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [--gdt [GDT]] [-o OUTPUT_PATH] [-v]
+                  [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-symbols] [-t THREAD_COUNT] [--va] [--fa] [--max-ram-percent MAX_RAM_PERCENT]
                   [--print-flags]
                   bin
 
 ghidrecomp - A Command Line Ghidra Decompiler
 
 positional arguments:
   bin                   Path to binary used for analysis
 
 options:
   -h, --help            show this help message and exit
   --cppexport           Use Ghidras CppExporter to decompile to single file (default: False)
   --filter FILTERS      Regex match for function name (default: None)
   --project-path PROJECT_PATH
                         Path to base ghidra projects (default: .ghidra_projects)
+  --gdt [GDT]           Additional GDT to apply (default: None)
   -o OUTPUT_PATH, --output-path OUTPUT_PATH
                         Location for all decompilations (default: decompilations)
   -v, --version         show program's version number and exit
   --sym-file-path SYM_FILE_PATH
                         Specify single pdb symbol file for bin (default: None)
   -s SYMBOLS_PATH, --symbols-path SYMBOLS_PATH
                         Path for local symbols directory (default: .symbols)
   --skip-symbols        Do not apply symbols (default: False)
   -t THREAD_COUNT, --thread-count THREAD_COUNT
                         Threads to use for processing. Defaults to cpu count (default: 8)
   --va                  Enable verbose analysis (default: False)
+  --fa                  Force new analysis (even if already analyzed) (default: False)
 
 JVM Options:
   --max-ram-percent MAX_RAM_PERCENT
                         Set JVM Max Ram % of host RAM (default: 50.0)
   --print-flags         Print JVM flags at start (default: False)
 ```
```

#### html2text {}

```diff
@@ -29,33 +29,35 @@
 - Auto-downloaded symbols for supported symbol servers (`-s SYMBOLS_PATH`) -
 https://msdl.microsoft.com/download/symbols/ - https://chromium-browser-
 symsrv.commondatastorage.googleapis.com/ - https://symbols.mozilla.org/ -
 https://software.intel.com/sites/downloads/symbols/ - https://driver-
 symbols.nvidia.com/ - https://download.amd.com/dir/bin/ - Specify the pdb for
 the binary (`--sym-file-path`) - Filter functions to decompile that match regex
 (`--filter`) - Apply custom data types (`--gdt`) ## Usage ``` usage: ghidrecomp
-[-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [-
-o OUTPUT_PATH] [-v] [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-
-symbols] [-t THREAD_COUNT] [--va] [--max-ram-percent MAX_RAM_PERCENT] [--print-
-flags] bin ghidrecomp - A Command Line Ghidra Decompiler positional arguments:
-bin Path to binary used for analysis options: -h, --help show this help message
-and exit --cppexport Use Ghidras CppExporter to decompile to single file
-(default: False) --filter FILTERS Regex match for function name (default: None)
---project-path PROJECT_PATH Path to base ghidra projects (default:
-.ghidra_projects) -o OUTPUT_PATH, --output-path OUTPUT_PATH Location for all
+[-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [--gdt
+[GDT]] [-o OUTPUT_PATH] [-v] [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH |
+--skip-symbols] [-t THREAD_COUNT] [--va] [--fa] [--max-ram-percent
+MAX_RAM_PERCENT] [--print-flags] bin ghidrecomp - A Command Line Ghidra
+Decompiler positional arguments: bin Path to binary used for analysis options:
+-h, --help show this help message and exit --cppexport Use Ghidras CppExporter
+to decompile to single file (default: False) --filter FILTERS Regex match for
+function name (default: None) --project-path PROJECT_PATH Path to base ghidra
+projects (default: .ghidra_projects) --gdt [GDT] Additional GDT to apply
+(default: None) -o OUTPUT_PATH, --output-path OUTPUT_PATH Location for all
 decompilations (default: decompilations) -v, --version show program's version
 number and exit --sym-file-path SYM_FILE_PATH Specify single pdb symbol file
 for bin (default: None) -s SYMBOLS_PATH, --symbols-path SYMBOLS_PATH Path for
 local symbols directory (default: .symbols) --skip-symbols Do not apply symbols
 (default: False) -t THREAD_COUNT, --thread-count THREAD_COUNT Threads to use
 for processing. Defaults to cpu count (default: 8) --va Enable verbose analysis
-(default: False) JVM Options: --max-ram-percent MAX_RAM_PERCENT Set JVM Max Ram
-% of host RAM (default: 50.0) --print-flags Print JVM flags at start (default:
-False) ``` ## Example Usage with Windows afd.sys: ### Command line ```bash wget
-https://msdl.microsoft.com/download/symbols/afd.sys/50989142a9000/afd.sys -
+(default: False) --fa Force new analysis (even if already analyzed) (default:
+False) JVM Options: --max-ram-percent MAX_RAM_PERCENT Set JVM Max Ram % of host
+RAM (default: 50.0) --print-flags Print JVM flags at start (default: False) ```
+## Example Usage with Windows afd.sys: ### Command line ```bash wget https://
+msdl.microsoft.com/download/symbols/afd.sys/50989142a9000/afd.sys -
 O afd.sys.10.0.22621.1415 ghidrecomp afd.sys.10.0.22621.1415 ``` ### Output
 ```bash Starting decompliations: Namespace(bin='tests/data/
 afd.sys.10.0.22621.1344', cppexport=False, filters=None,
 project_path='.ghidra_projects', output_path='decompilations',
 sym_file_path=None, symbols_path='.symbols', skip_symbols=False,
 thread_count=8, va=False) INFO Using log config file: jar:file:/ghidra/Ghidra/
 Framework/Generic/lib/Generic.jar!/generic.log4j.xml (LoggingInitialization)
```

### Comparing `ghidrecomp-0.2.0/ghidrecomp/decompile.py` & `ghidrecomp-0.3.0/ghidrecomp/decompile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from pathlib import Path
 from typing import TYPE_CHECKING
 from argparse import Namespace
 import concurrent.futures
 from time import time
-from pyhidra import HeadlessPyhidraLauncher, open_program
+import pyhidra
 
-from .utility import set_pdb, setup_symbol_server, set_remote_pdbs, analyze_program, get_pdb
+from .utility import set_pdb, setup_symbol_server, set_remote_pdbs, analyze_program, apply_gdt
 
 # needed for ghidra python vscode autocomplete
 if TYPE_CHECKING:
     import ghidra
     from ghidra_builtins import *
 
 
@@ -31,45 +31,45 @@
 
     return decompilers
 
 
 def decompile_func(func: 'ghidra.program.model.listing.Function',
                    decompilers: dict,
                    thread_id: int = 0,
-                   timeout: int = 0,
+                   TIMEOUT: int = 0,
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
 
-    result: "DecompileResults" = decompilers[thread_id].decompileFunction(func, timeout, monitor)
+    result: "DecompileResults" = decompilers[thread_id].decompileFunction(func, TIMEOUT, monitor)
 
-    if '' == result.errorMessage:
+    if '' == result.getErrorMessage():
         code = result.decompiledFunction.getC()
         sig = result.decompiledFunction.getSignature()
     else:
-        code = result.errorMessage
+        code = result.getErrorMessage()
         sig = None
 
     return [f'{func.getName()[:MAX_PATH_LEN]}-{func.entryPoint}', code, sig]
 
 
 def decompile_to_single_file(path: Path,
                              prog: "ghidra.program.model.listing.Program",
                              create_header: bool = True,
-                             create_file: bool = True,
+                             createFile: bool = True,
                              emit_types: bool = True,
-                             exclude_tags: bool = False,
+                             excludeTags: bool = True,
                              tags: str = None,
                              verbose: bool = True):
     """
     Use Ghidra's CppExporter to decompile all functions to a single file
     """
     from ghidra.app.util.exporter import CppExporter
     from ghidra.util.task import ConsoleTaskMonitor
@@ -78,16 +78,15 @@
     c_file = File(path.absolute())
 
     if verbose:
         monitor = ConsoleTaskMonitor()
     else:
         monitor = ConsoleTaskMonitor().DUMMY
 
-    decompiler = CppExporter(create_header, create_file, emit_types, exclude_tags, tags)
-
+    decompiler = CppExporter(True, True, True, False, None)
     decompiler.export(c_file, prog, prog.getMemory(), monitor)
 
 
 def decompile(args: Namespace):
 
     print(f'Starting decompliations: {args}')
 
@@ -95,24 +94,17 @@
     project_location = Path(args.project_path)
     thread_count = args.thread_count
 
     output_path = Path(args.output_path) / bin_path.name
     output_path.mkdir(exist_ok=True, parents=True)
 
     # turn on verbose
-    launcher = HeadlessPyhidraLauncher(True)
-
-    # set max % of host RAM
-    launcher.add_vmargs(f'-XX:MaxRAMPercentage={args.max_ram_percent}')
-    if args.print_flags:
-        launcher.add_vmargs('-XX:+PrintFlagsFinal')
+    pyhidra.start(True)
 
-    launcher.start()
-
-    with open_program(bin_path, project_location=project_location, project_name=bin_path.name, analyze=False) as flat_api:
+    with pyhidra.open_program(bin_path, project_location=project_location, project_name=bin_path.name, analyze=False) as flat_api:
 
         from ghidra.util.task import ConsoleTaskMonitor
         from ghidra.program.model.listing import Program
         monitor = ConsoleTaskMonitor()
 
         program: "Program" = flat_api.getCurrentProgram()
 
@@ -120,36 +112,40 @@
             if args.sym_file_path:
                 set_pdb(program, args.sym_file_path)
             else:
                 setup_symbol_server(args.symbols_path)
 
                 set_remote_pdbs(program, True)
 
-                pdb = get_pdb(program)
-                if pdb is None:
-                    print(f"Failed to find pdb for {program}")
+                # pdb = get_pdb(program)
+                # assert pdb is not None
+
+        # apply GDT
+        if args.gdt:
+            for gdt_path in args.gdt:
+                print(f'Applying gdt {gdt_path}...')
+                apply_gdt(program, gdt_path, verbose=args.va)
 
         # analyze program if we haven't yet
-        analyze_program(program, verbose=args.va)
+        analyze_program(program, verbose=args.va, force_analysis=args.fa)
 
         all_funcs = []
         skip_count = 0
 
         for f in program.functionManager.getFunctions(True):
 
             if args.filters:
                 if any([re.search(fil, f.name, re.IGNORECASE) for fil in args.filters]):
                     all_funcs.append(f)
                 else:
                     skip_count += 1
             else:
                 all_funcs.append(f)
 
-        if skip_count > 0:
-            print(f'Skipped {skip_count} functions that failed to match any of {args.filters}')
+        print(f'Skipped {skip_count} functions that failed to match any of {args.filters}')
 
         if args.cppexport:
             print(f"Decompiling {len(all_funcs)} functions using Ghidra's CppExporter")
             c_file = Path(args.output_path) / Path(bin_path.name + '.c')
             start = time()
             decompile_to_single_file(c_file, program)
             print(f'Decompiled {len(all_funcs)} functions for {program.name} in {time() - start}')
```

### Comparing `ghidrecomp-0.2.0/ghidrecomp/utility.py` & `ghidrecomp-0.3.0/ghidrecomp/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,53 +18,58 @@
     parser = argparse.ArgumentParser(description='ghidrecomp - A Command Line Ghidra Decompiler',
                                      formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument('bin', help='Path to binary used for analysis')
     parser.add_argument('--cppexport', action='store_true', help='Use Ghidras CppExporter to decompile to single file')
     parser.add_argument('--filter', dest='filters', action='append', help='Regex match for function name')
     parser.add_argument('--project-path', help='Path to base ghidra projects ', default='.ghidra_projects')
+    parser.add_argument('--gdt', help='Additional GDT to apply', nargs='?', action='append')
     parser.add_argument('-o', '--output-path', help='Location for all decompilations', default='decompilations')
     parser.add_argument("-v", "--version", action="version", version=__version__)
 
     group = parser.add_mutually_exclusive_group()
     group.add_argument('--sym-file-path', help='Specify single pdb symbol file for bin')
     group.add_argument('-s', '--symbols-path', help='Path for local symbols directory', default='.symbols')
     group.add_argument('--skip-symbols', help='Do not apply symbols', action='store_true')
 
     parser.add_argument('-t', '--thread-count', type=int,
                         help='Threads to use for processing. Defaults to cpu count', default=THREAD_COUNT)
     parser.add_argument('--va', help='Enable verbose analysis', action='store_true')
+    parser.add_argument('--fa', help='Force new analysis (even if already analyzed)', action='store_true')
 
     group = parser.add_argument_group('JVM Options')
     group.add_argument('--max-ram-percent', help='Set JVM Max Ram %% of host RAM', default=50.0)
     group.add_argument('--print-flags', help='Print JVM flags at start', action='store_true')
 
     return parser
 
 
-def analyze_program(program, verbose: bool = False):
-    # modified pyhidra.core._analyze_program
-
-    print(f"Analyzing program {program.name}")
+def analyze_program(program, verbose: bool = False, force_analysis: bool = False):
+    """
+    Modified pyhidra.core._analyze_program    
+    """
 
     from ghidra.program.flatapi import FlatProgramAPI
     from ghidra.util.task import ConsoleTaskMonitor
     from ghidra.program.util import GhidraProgramUtilities
     from ghidra.app.script import GhidraScriptUtil
 
     if verbose:
-        print('Enabling verbose analysis..')
+        print('Enabling verbose analysis...')
         monitor = ConsoleTaskMonitor()
         flat_api = FlatProgramAPI(program, monitor)
     else:
         flat_api = FlatProgramAPI(program)
 
-    if GhidraProgramUtilities.shouldAskToAnalyze(program):
+    if GhidraProgramUtilities.shouldAskToAnalyze(program) or force_analysis:
+        print(f"Analyzing program {program.name}...")
+
         GhidraScriptUtil.acquireBundleHostReference()
         try:
+            print(f"Running analyzers...")
             flat_api.analyzeAll(program)
             GhidraProgramUtilities.setAnalyzedFlag(program, True)
         finally:
             GhidraScriptUtil.releaseBundleHostReference()
     else:
         print(f'{program} already analyzed... skipping')
 
@@ -168,7 +173,33 @@
 
     from ghidra.app.plugin.core.analysis import PdbAnalyzer
     from ghidra.app.plugin.core.analysis import PdbUniversalAnalyzer
     # Enable Remote Symbol Servers
 
     PdbUniversalAnalyzer.setAllowRemoteOption(program, allow)
     PdbAnalyzer.setAllowRemoteOption(program, allow)
+
+
+def apply_gdt(program: "ghidra.program.model.listing.Program", gdt_path:  Union[str, Path], verbose: bool = False):
+    """
+    Apply GDT to program
+    """
+
+    from ghidra.app.cmd.function import ApplyFunctionDataTypesCmd
+    from ghidra.program.model.symbol import SourceType
+    from java.io import File
+    from java.util import List
+    from ghidra.program.model.data import FileDataTypeManager
+    from ghidra.util.task import ConsoleTaskMonitor
+
+    gdt_path = Path(gdt_path)
+
+    if verbose:
+        print('Enabling verbose gdt..')
+        monitor = ConsoleTaskMonitor()
+    else:
+        monitor = ConsoleTaskMonitor().DUMMY_MONITOR
+
+    archiveGDT = File(gdt_path)
+    archiveDTM = FileDataTypeManager.openFileArchive(archiveGDT, False)
+    cmd = ApplyFunctionDataTypesCmd(List.of(archiveDTM), None, SourceType.USER_DEFINED, True, True)
+    cmd.applyTo(program, monitor)
```

### Comparing `ghidrecomp-0.2.0/ghidrecomp.egg-info/PKG-INFO` & `ghidrecomp-0.3.0/ghidrecomp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidrecomp
-Version: 0.2.0
+Version: 0.3.0
 Summary: A comand line Ghidra Decomplier
 Home-page: https://github.com/clearbluejar/ghidrecomp
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: ghidra,decompiler,callgraph
 Platform: any
@@ -117,41 +117,43 @@
 - Specify the pdb for the binary (`--sym-file-path`)
 - Filter functions to decompile that match regex (`--filter`)
 - Apply custom data types (`--gdt`)
 
 ## Usage
 
 ```
-usage: ghidrecomp [-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [-o OUTPUT_PATH] [-v]
-                  [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-symbols] [-t THREAD_COUNT] [--va] [--max-ram-percent MAX_RAM_PERCENT]
+usage: ghidrecomp [-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [--gdt [GDT]] [-o OUTPUT_PATH] [-v]
+                  [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-symbols] [-t THREAD_COUNT] [--va] [--fa] [--max-ram-percent MAX_RAM_PERCENT]
                   [--print-flags]
                   bin
 
 ghidrecomp - A Command Line Ghidra Decompiler
 
 positional arguments:
   bin                   Path to binary used for analysis
 
 options:
   -h, --help            show this help message and exit
   --cppexport           Use Ghidras CppExporter to decompile to single file (default: False)
   --filter FILTERS      Regex match for function name (default: None)
   --project-path PROJECT_PATH
                         Path to base ghidra projects (default: .ghidra_projects)
+  --gdt [GDT]           Additional GDT to apply (default: None)
   -o OUTPUT_PATH, --output-path OUTPUT_PATH
                         Location for all decompilations (default: decompilations)
   -v, --version         show program's version number and exit
   --sym-file-path SYM_FILE_PATH
                         Specify single pdb symbol file for bin (default: None)
   -s SYMBOLS_PATH, --symbols-path SYMBOLS_PATH
                         Path for local symbols directory (default: .symbols)
   --skip-symbols        Do not apply symbols (default: False)
   -t THREAD_COUNT, --thread-count THREAD_COUNT
                         Threads to use for processing. Defaults to cpu count (default: 8)
   --va                  Enable verbose analysis (default: False)
+  --fa                  Force new analysis (even if already analyzed) (default: False)
 
 JVM Options:
   --max-ram-percent MAX_RAM_PERCENT
                         Set JVM Max Ram % of host RAM (default: 50.0)
   --print-flags         Print JVM flags at start (default: False)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghidrecomp Version: 0.2.0 Summary: A comand line
+Metadata-Version: 2.1 Name: ghidrecomp Version: 0.3.0 Summary: A comand line
 Ghidra Decomplier Home-page: https://github.com/clearbluejar/ghidrecomp Author:
 clearbluejar Author-email: clearbluejar@clearbluejar.com License: GPL-3.0
 license Keywords: ghidra,decompiler,callgraph Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -40,33 +40,35 @@
 - Auto-downloaded symbols for supported symbol servers (`-s SYMBOLS_PATH`) -
 https://msdl.microsoft.com/download/symbols/ - https://chromium-browser-
 symsrv.commondatastorage.googleapis.com/ - https://symbols.mozilla.org/ -
 https://software.intel.com/sites/downloads/symbols/ - https://driver-
 symbols.nvidia.com/ - https://download.amd.com/dir/bin/ - Specify the pdb for
 the binary (`--sym-file-path`) - Filter functions to decompile that match regex
 (`--filter`) - Apply custom data types (`--gdt`) ## Usage ``` usage: ghidrecomp
-[-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [-
-o OUTPUT_PATH] [-v] [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH | --skip-
-symbols] [-t THREAD_COUNT] [--va] [--max-ram-percent MAX_RAM_PERCENT] [--print-
-flags] bin ghidrecomp - A Command Line Ghidra Decompiler positional arguments:
-bin Path to binary used for analysis options: -h, --help show this help message
-and exit --cppexport Use Ghidras CppExporter to decompile to single file
-(default: False) --filter FILTERS Regex match for function name (default: None)
---project-path PROJECT_PATH Path to base ghidra projects (default:
-.ghidra_projects) -o OUTPUT_PATH, --output-path OUTPUT_PATH Location for all
+[-h] [--cppexport] [--filter FILTERS] [--project-path PROJECT_PATH] [--gdt
+[GDT]] [-o OUTPUT_PATH] [-v] [--sym-file-path SYM_FILE_PATH | -s SYMBOLS_PATH |
+--skip-symbols] [-t THREAD_COUNT] [--va] [--fa] [--max-ram-percent
+MAX_RAM_PERCENT] [--print-flags] bin ghidrecomp - A Command Line Ghidra
+Decompiler positional arguments: bin Path to binary used for analysis options:
+-h, --help show this help message and exit --cppexport Use Ghidras CppExporter
+to decompile to single file (default: False) --filter FILTERS Regex match for
+function name (default: None) --project-path PROJECT_PATH Path to base ghidra
+projects (default: .ghidra_projects) --gdt [GDT] Additional GDT to apply
+(default: None) -o OUTPUT_PATH, --output-path OUTPUT_PATH Location for all
 decompilations (default: decompilations) -v, --version show program's version
 number and exit --sym-file-path SYM_FILE_PATH Specify single pdb symbol file
 for bin (default: None) -s SYMBOLS_PATH, --symbols-path SYMBOLS_PATH Path for
 local symbols directory (default: .symbols) --skip-symbols Do not apply symbols
 (default: False) -t THREAD_COUNT, --thread-count THREAD_COUNT Threads to use
 for processing. Defaults to cpu count (default: 8) --va Enable verbose analysis
-(default: False) JVM Options: --max-ram-percent MAX_RAM_PERCENT Set JVM Max Ram
-% of host RAM (default: 50.0) --print-flags Print JVM flags at start (default:
-False) ``` ## Example Usage with Windows afd.sys: ### Command line ```bash wget
-https://msdl.microsoft.com/download/symbols/afd.sys/50989142a9000/afd.sys -
+(default: False) --fa Force new analysis (even if already analyzed) (default:
+False) JVM Options: --max-ram-percent MAX_RAM_PERCENT Set JVM Max Ram % of host
+RAM (default: 50.0) --print-flags Print JVM flags at start (default: False) ```
+## Example Usage with Windows afd.sys: ### Command line ```bash wget https://
+msdl.microsoft.com/download/symbols/afd.sys/50989142a9000/afd.sys -
 O afd.sys.10.0.22621.1415 ghidrecomp afd.sys.10.0.22621.1415 ``` ### Output
 ```bash Starting decompliations: Namespace(bin='tests/data/
 afd.sys.10.0.22621.1344', cppexport=False, filters=None,
 project_path='.ghidra_projects', output_path='decompilations',
 sym_file_path=None, symbols_path='.symbols', skip_symbols=False,
 thread_count=8, va=False) INFO Using log config file: jar:file:/ghidra/Ghidra/
 Framework/Generic/lib/Generic.jar!/generic.log4j.xml (LoggingInitialization)
```

### Comparing `ghidrecomp-0.2.0/setup.cfg` & `ghidrecomp-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghidrecomp-0.2.0/tests/test_ghidrecomp.py` & `ghidrecomp-0.3.0/tests/test_ghidrecomp.py`

 * *Files identical despite different names*

