# Comparing `tmp/ShellcodeTester-0.2.8.tar.gz` & `tmp/ShellcodeTester-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellcodeTester-0.2.8.tar", last modified: Sun Apr 23 12:59:37 2023, max compression
+gzip compressed data, was "ShellcodeTester-0.2.9.tar", last modified: Mon Apr 24 00:58:46 2023, max compression
```

## Comparing `ShellcodeTester-0.2.8.tar` & `ShellcodeTester-0.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.648876 ShellcodeTester-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-23 12:59:37.648876 ShellcodeTester-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.612876 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 12:59:37.000000 ShellcodeTester-0.2.8/ShellcodeTester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.612876 ShellcodeTester-0.2.8/nasmshell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.612876 ShellcodeTester-0.2.8/nasmshell/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/libs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/nasmshell/nasmshell.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:59:37.648876 ShellcodeTester-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.612876 ShellcodeTester-0.2.8/shell_bins/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:59:25.000000 ShellcodeTester-0.2.8/shell_bins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.616876 ShellcodeTester-0.2.8/shell_bins/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:59:25.000000 ShellcodeTester-0.2.8/shell_bins/linux/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1951840 2023-04-23 12:58:20.000000 ShellcodeTester-0.2.8/shell_bins/linux/nasm
--rw-r--r--   0 runner    (1001) docker     (123) 12329280 2023-04-23 12:58:06.000000 ShellcodeTester-0.2.8/shell_bins/linux/objdump
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.636876 ShellcodeTester-0.2.8/shell_bins/macosx/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:59:25.000000 ShellcodeTester-0.2.8/shell_bins/macosx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  3237896 2023-04-23 12:58:20.000000 ShellcodeTester-0.2.8/shell_bins/macosx/nasm
--rw-r--r--   0 runner    (1001) docker     (123)   167120 2023-04-23 12:58:06.000000 ShellcodeTester-0.2.8/shell_bins/macosx/objdump
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.640876 ShellcodeTester-0.2.8/shell_bins/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:59:25.000000 ShellcodeTester-0.2.8/shell_bins/windows/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1638912 2023-04-23 12:58:20.000000 ShellcodeTester-0.2.8/shell_bins/windows/nasm.exe
--rwxr-xr-x   0 runner    (1001) docker     (123)  2410600 2023-04-23 12:58:19.000000 ShellcodeTester-0.2.8/shell_bins/windows/objdump.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.644876 ShellcodeTester-0.2.8/shell_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/asmfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/inlineassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shell_libs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.648876 ShellcodeTester-0.2.8/shellcodetester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shellcodetester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shellcodetester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shellcodetester/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shellcodetester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shellcodetester/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/shellcodetester/shellcodetester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:37.648876 ShellcodeTester-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-23 12:59:23.000000 ShellcodeTester-0.2.8/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:46.008099 ShellcodeTester-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-24 00:58:46.008099 ShellcodeTester-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:45.984098 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 00:58:45.000000 ShellcodeTester-0.2.9/ShellcodeTester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:45.984098 ShellcodeTester-0.2.9/nasmshell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:45.984098 ShellcodeTester-0.2.9/nasmshell/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/libs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/nasmshell/nasmshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:58:46.008099 ShellcodeTester-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:45.984098 ShellcodeTester-0.2.9/shell_bins/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:58:33.000000 ShellcodeTester-0.2.9/shell_bins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:45.984098 ShellcodeTester-0.2.9/shell_bins/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:58:33.000000 ShellcodeTester-0.2.9/shell_bins/linux/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1951840 2023-04-24 00:57:42.000000 ShellcodeTester-0.2.9/shell_bins/linux/nasm
+-rw-r--r--   0 runner    (1001) docker     (123) 12329280 2023-04-24 00:57:31.000000 ShellcodeTester-0.2.9/shell_bins/linux/objdump
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:46.000099 ShellcodeTester-0.2.9/shell_bins/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:58:33.000000 ShellcodeTester-0.2.9/shell_bins/macosx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  3237896 2023-04-24 00:57:42.000000 ShellcodeTester-0.2.9/shell_bins/macosx/nasm
+-rw-r--r--   0 runner    (1001) docker     (123)   167120 2023-04-24 00:57:31.000000 ShellcodeTester-0.2.9/shell_bins/macosx/objdump
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:46.004099 ShellcodeTester-0.2.9/shell_bins/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:58:33.000000 ShellcodeTester-0.2.9/shell_bins/windows/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1638912 2023-04-24 00:57:42.000000 ShellcodeTester-0.2.9/shell_bins/windows/nasm.exe
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2410600 2023-04-24 00:57:40.000000 ShellcodeTester-0.2.9/shell_bins/windows/objdump.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:46.008099 ShellcodeTester-0.2.9/shell_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/asmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/inlineassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shell_libs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:46.008099 ShellcodeTester-0.2.9/shellcodetester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shellcodetester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shellcodetester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shellcodetester/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shellcodetester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shellcodetester/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/shellcodetester/shellcodetester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:46.008099 ShellcodeTester-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 00:58:32.000000 ShellcodeTester-0.2.9/tests/tests.py
```

### Comparing `ShellcodeTester-0.2.8/LICENSE` & `ShellcodeTester-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/PKG-INFO` & `ShellcodeTester-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.8
+Version: 0.2.9
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
```

### Comparing `ShellcodeTester-0.2.8/README.md` & `ShellcodeTester-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/ShellcodeTester.egg-info/PKG-INFO` & `ShellcodeTester-0.2.9/ShellcodeTester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.8
+Version: 0.2.9
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
```

### Comparing `ShellcodeTester-0.2.8/ShellcodeTester.egg-info/SOURCES.txt` & `ShellcodeTester-0.2.9/ShellcodeTester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/nasmshell/args.py` & `ShellcodeTester-0.2.9/nasmshell/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/nasmshell/config.py` & `ShellcodeTester-0.2.9/nasmshell/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/nasmshell/libs/cmd.py` & `ShellcodeTester-0.2.9/nasmshell/libs/cmd.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/nasmshell/nasmshell.py` & `ShellcodeTester-0.2.9/nasmshell/nasmshell.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/setup.py` & `ShellcodeTester-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_bins/linux/nasm` & `ShellcodeTester-0.2.9/shell_bins/linux/nasm`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_bins/linux/objdump` & `ShellcodeTester-0.2.9/shell_bins/linux/objdump`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_bins/macosx/nasm` & `ShellcodeTester-0.2.9/shell_bins/macosx/nasm`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_bins/macosx/objdump` & `ShellcodeTester-0.2.9/shell_bins/macosx/objdump`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_bins/windows/nasm.exe` & `ShellcodeTester-0.2.9/shell_bins/windows/nasm.exe`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_bins/windows/objdump.exe` & `ShellcodeTester-0.2.9/shell_bins/windows/objdump.exe`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/asmfile.py` & `ShellcodeTester-0.2.9/shell_libs/asmfile.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/assembler.py` & `ShellcodeTester-0.2.9/shell_libs/assembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/color.py` & `ShellcodeTester-0.2.9/shell_libs/color.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/disassembler.py` & `ShellcodeTester-0.2.9/shell_libs/disassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/inlineassembler.py` & `ShellcodeTester-0.2.9/shell_libs/inlineassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/logger.py` & `ShellcodeTester-0.2.9/shell_libs/logger.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/process.py` & `ShellcodeTester-0.2.9/shell_libs/process.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/runner.py` & `ShellcodeTester-0.2.9/shell_libs/runner.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/tools.py` & `ShellcodeTester-0.2.9/shell_libs/tools.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shell_libs/transform.py` & `ShellcodeTester-0.2.9/shell_libs/transform.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shellcodetester/args.py` & `ShellcodeTester-0.2.9/shellcodetester/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shellcodetester/config.py` & `ShellcodeTester-0.2.9/shellcodetester/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shellcodetester/password.py` & `ShellcodeTester-0.2.9/shellcodetester/password.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.8/shellcodetester/shellcodetester.py` & `ShellcodeTester-0.2.9/shellcodetester/shellcodetester.py`

 * *Files identical despite different names*

