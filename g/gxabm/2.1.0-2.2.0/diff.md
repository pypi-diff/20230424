# Comparing `tmp/gxabm-2.1.0.tar.gz` & `tmp/gxabm-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.1.0.tar", last modified: Wed Jan 18 21:46:20 2023, max compression
+gzip compressed data, was "gxabm-2.2.0.tar", last modified: Mon Apr 24 20:25:34 2023, max compression
```

## Comparing `gxabm-2.1.0.tar` & `gxabm-2.2.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-01-18 21:46:20.034044 gxabm-2.1.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.1.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-01-18 21:46:20.033852 gxabm-2.1.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.1.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-01-18 21:46:20.029671 gxabm-2.1.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-01-18 21:46:14.000000 gxabm-2.1.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8537 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-01-18 21:46:20.032115 gxabm-2.1.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    16622 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     5443 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6229 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7433 2023-01-18 20:21:02.000000 gxabm-2.1.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.1.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)     9105 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     2342 2023-01-18 20:21:02.000000 gxabm-2.1.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2022-03-07 12:56:12.000000 gxabm-2.1.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    10382 2023-01-18 20:21:02.000000 gxabm-2.1.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     4447 2022-10-19 17:36:24.000000 gxabm-2.1.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-01-18 21:46:20.032959 gxabm-2.1.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-01-18 21:46:19.000000 gxabm-2.1.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      652 2023-01-18 21:46:19.000000 gxabm-2.1.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-01-18 21:46:19.000000 gxabm-2.1.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-01-18 21:46:19.000000 gxabm-2.1.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-01-18 21:46:19.000000 gxabm-2.1.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-01-18 21:46:19.000000 gxabm-2.1.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-01-18 21:46:20.034093 gxabm-2.1.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.1.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-01-18 21:46:20.033545 gxabm-2.1.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.1.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.1.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.1.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.1.0/test/test_environments.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.747554 gxabm-2.2.0/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.2.0/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-24 20:25:34.747338 gxabm-2.2.0/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.2.0/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.737892 gxabm-2.2.0/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-04-24 20:24:53.000000 gxabm-2.2.0/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.743372 gxabm-2.2.0/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    16622 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5443 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6229 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7433 2023-01-18 20:21:02.000000 gxabm-2.2.0/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.2.0/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     9582 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2342 2023-01-18 20:21:02.000000 gxabm-2.2.0/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.2.0/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.2.0/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    10513 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.2.0/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5499 2023-04-24 20:24:38.000000 gxabm-2.2.0/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.745358 gxabm-2.2.0/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-24 20:25:34.000000 gxabm-2.2.0/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-24 20:25:34.747617 gxabm-2.2.0/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.2.0/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-24 20:25:34.746857 gxabm-2.2.0/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.2.0/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.2.0/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.2.0/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.2.0/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.2.0/test/workflow.py
```

### Comparing `gxabm-2.1.0/PKG-INFO` & `gxabm-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.1.0
+Version: 2.2.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.1.0/README.md` & `gxabm-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/__main__.py` & `gxabm-2.2.0/abm/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 """
 The Automated Benchmarking Tool
 
-Copyright 2021 The Galaxy Project. All rights reserved.
+Copyright 2023 The Galaxy Project. All rights reserved.
 
 """
 
 import yaml
 import sys
 import os
 import logging
@@ -54,14 +54,17 @@
     print(bold(text))
 
 
 def command_list(commands:list):
     return '|'.join(bold(c) for c in commands)
 
 
+def copyright():
+    print(f"    Copyright 2023 The Galaxy Project. All Rights Reserved.\n")
+
 def print_main_help(menu_data):
     print()
     head("    DESCRIPTION")
     print("        Workflow and data management for remote Galaxy instances")
     print()
     head("    SYNOPSIS")
     print(f"        abm COMMAND [SUBCOMMAND] [OPTIONS]")
@@ -75,15 +78,15 @@
     print(f"        {command_list(help_args)}")
     print("            print this help screen and exit")
     print()
     head("    NOTES")
     print(f"        Available SUBCOMMANDS and OPTIONS depend on the command. Use the {bold('help')} subcommand")
     print(f"        to learn more about each of the commands. For example:\n")
     print(f"        $> abm workflow help\n")
-    print("    Copyright 2022 The Galaxy Project\n")
+    copyright()
 
 
 def print_help(menu_data, command):
     submenu = None
     for menu_item in menu_data:
         if command in menu_item['name']:
             submenu = menu_item
@@ -104,15 +107,15 @@
     head("    SUBCOMMANDS")
     for menu_item in submenu['menu']:
         print(f"        {'|'.join(bold(x) for x in menu_item['name'])} {menu_item['params'] if 'params' in menu_item else ''}")
         print(f"            {menu_item['help']}")
     print(f"        {bold('help')}")
     print("            print this help screen and exit")
     print()
-    print("    Copyright 2022 The Galaxy Project\n")
+    copyright()
 
 
 all_commands = {}
 
 
 def get_menu(name: str):
     if name in all_commands:
@@ -172,16 +175,15 @@
     return menu_data
 
 
 def version():
     version = getVersion()
     print()
     print(f"    Galaxy Automated Benchmarking v{version}")
-    print(f"    Copyright 2022 The Galaxy Project. All Rights Reserved.\n")
-
+    copyright()
 
 def _get_logopt(args: list):
     OPTS = ['-log', '--log', '-logging', '--logging']
     for i in range(len(args)):
         if args[i] in OPTS:
             return i
     return -1
@@ -251,17 +253,14 @@
     if subcommand and subcommand in help_args:
         print_help(menu_data, command)
         return
 
     context = None
     if profile is not None:
         context = Context(profile)
-#        if context.GALAXY_SERVER is None:
-#            print("ERROR: GALAXY_SERVER was not set in the profile.")
-#            return
     if command in all_commands:
         subcommands = all_commands[command]
         if subcommand not in subcommands:
             print(f'ERROR: unrecognized subcommand "{subcommand}"')
             print(f'Type "{program} {command} help" for more help.')
             return
         handler = subcommands[subcommand]
```

### Comparing `gxabm-2.1.0/abm/lib/benchmark.py` & `gxabm-2.2.0/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/cloudlaunch.py` & `gxabm-2.2.0/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/common.py` & `gxabm-2.2.0/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/config.py` & `gxabm-2.2.0/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/dataset.py` & `gxabm-2.2.0/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/experiment.py` & `gxabm-2.2.0/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/folder.py` & `gxabm-2.2.0/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/helm.py` & `gxabm-2.2.0/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/history.py` & `gxabm-2.2.0/abm/lib/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,14 +246,29 @@
         print('ERROR: please provide the history ID')
         return
     gi = connect(context)
     gi.histories.delete_history(args[0], True)
     print(f"Deleted history {args[0]}")
 
 
+def copy(context:Context, args:list):
+    if len(args) != 2:
+        print("ERROR: Invalid parameters. Provide a history ID and new history name.")
+        return
+    id = args[0]
+    name = args[1]
+
+    gi = connect(context)
+    new_history = gi.histories.create_history(name)
+    datasets = gi.datasets.get_datasets(history_id=id)
+    for dataset in datasets:
+        gi.histories.copy_dataset(new_history['id'], dataset['id'])
+    print(json.dumps(new_history, indent=4))
+
+
 def purge(context: Context, args:list):
     if len(args) != 1:
         print("ERROR: Please pass a string used to filter histories to be deleted.")
         print("Use 'abm <cloud> history purge *' to remove ALL histories.")
         return
     all = args[0] == '0'
     gi = connect(context)
```

### Comparing `gxabm-2.1.0/abm/lib/job.py` & `gxabm-2.2.0/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/kubectl.py` & `gxabm-2.2.0/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/library.py` & `gxabm-2.2.0/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/abm/lib/menu.yml` & `gxabm-2.2.0/abm/lib/menu.yml`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
       params: "[CLOUD HISTORY_ID JEHA_ID | URL | [dna|rna]] [-n|--no-wait]"
       handler: history.himport
       help: import a history from another Galaxy server
     - name: [create, new]
       params: NAME
       handler: history.create
       help: create a new history and return its ID
+    - name: [copy, cp]
+      params: HISTORY_ID NAME
+      handler: history.copy
+      help: create a copy of an existing history
     - name: ['export', 'exp', 'ex']
       handler: history.export
       params: "ID [-n|--no-wait]"
       help: prepares a history for export to another Galaxy server
     - name: [find]
       handler: history.find
       help: find a history by name
@@ -283,15 +287,15 @@
   menu:
     - name: [list, ls]
       handler: cloudlaunch.list
       help: list deployments on all cloud providers
     - name: [create, launch, new]
       handler: cloudlaunch.create
       help: create a new deployment on the specified provider
-      params: "[aws|gcp] NAME [-|--type vmType] [-k|--keypair keyName] [-c|--config config-app]"
+      params: "[aws|gcp] NAME [-t|--type vmType] [-k|--keypair keyName] [-c|--config config-app]"
     - name: [delete, rm]
       help: delete a deployment
       handler: cloudlaunch.delete
       params: "ID"
 - name: [library, lib]
   help: manage data libraries on the server
   menu:
```

### Comparing `gxabm-2.1.0/abm/lib/users.py` & `gxabm-2.2.0/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.2.0/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.1.0
+Version: 2.2.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.1.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.2.0/gxabm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 gxabm.egg-info/dependency_links.txt
 gxabm.egg-info/entry_points.txt
 gxabm.egg-info/requires.txt
 gxabm.egg-info/top_level.txt
 test/__init__.py
 test/check_tools.py
 test/metrics.py
-test/test_environments.py
+test/test_environments.py
+test/workflow.py
```

### Comparing `gxabm-2.1.0/setup.py` & `gxabm-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/test/check_tools.py` & `gxabm-2.2.0/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.1.0/test/metrics.py` & `gxabm-2.2.0/test/metrics.py`

 * *Files identical despite different names*

