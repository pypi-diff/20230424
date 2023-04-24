# Comparing `tmp/croudtech-ecs-tools-0.1.8.tar.gz` & `tmp/croudtech-ecs-tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croudtech-ecs-tools-0.1.8.tar", last modified: Tue Oct  4 16:07:06 2022, max compression
+gzip compressed data, was "croudtech-ecs-tools-0.1.9.tar", last modified: Mon Apr 24 10:39:03 2023, max compression
```

## Comparing `croudtech-ecs-tools-0.1.8.tar` & `croudtech-ecs-tools-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/
--rw-r--r--   0 vsts      (1001) docker     (121)    11357 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     1942 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1370 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7543 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/cli.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3386 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/ecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     1942 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      372 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       68 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     1762 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 10:39:03.772773 croudtech-ecs-tools-0.1.9/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11357 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     1942 2023-04-24 10:39:03.772773 croudtech-ecs-tools-0.1.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1370 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 10:39:03.772773 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8044 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6871 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools/ecs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 10:39:03.772773 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1942 2023-04-24 10:39:03.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      406 2023-04-24 10:39:03.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-24 10:39:03.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       68 2023-04-24 10:39:03.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-04-24 10:39:03.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-04-24 10:39:03.000000 croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-24 10:39:03.772773 croudtech-ecs-tools-0.1.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1762 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 10:39:03.772773 croudtech-ecs-tools-0.1.9/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)      307 2023-04-24 10:38:25.000000 croudtech-ecs-tools-0.1.9/tests/test_croudtech_ecs_tools.py
```

### Comparing `croudtech-ecs-tools-0.1.8/LICENSE` & `croudtech-ecs-tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-0.1.8/PKG-INFO` & `croudtech-ecs-tools-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-0.1.8/README.md` & `croudtech-ecs-tools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/cli.py` & `croudtech-ecs-tools-0.1.9/croudtech_ecs_tools/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from email.policy import default
 import click
 import boto3
 from botocore.config import Config as Boto3Config
 from click.decorators import command
 from click.termui import prompt
 import os
-from croudtech_ecs_tools.ecs import Ecs
+from croudtech_ecs_tools.ecs import Ecs, EcsScaler
 import json
 
 
 
 class EcsTools:
     _services = {}
     _tasks = {}
@@ -202,9 +202,27 @@
 
 @cli.command()
 @click.option("--cluster", required=True)
 def list_service_discovery_endpoints(cluster):
     ecs_manager = Ecs(cluster=cluster)
     print(json.dumps(ecs_manager.list_ecs_service_endpoints(), indent=2, default=str))
 
+@cli.command()
+@click.option("--cluster", required=True)
+def show_service_ips(cluster):
+    ecs_manager = Ecs(cluster=cluster)
+    print(json.dumps(ecs_manager.show_service_ips(), indent=2, default=str))
+
+@cli.command()
+@click.argument("environment")
+def scale_up(environment):
+    ecs_scaler = EcsScaler(environment)
+    ecs_scaler.scale_up()
+
+@cli.command()
+@click.argument("environment")
+def scale_down(environment):
+    ecs_scaler = EcsScaler(environment)
+    ecs_scaler.scale_down()
+
 if __name__ == "__main__":
-    cli()
+    cli()
```

### Comparing `croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/PKG-INFO` & `croudtech-ecs-tools-0.1.9/croudtech_ecs_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-0.1.8/setup.py` & `croudtech-ecs-tools-0.1.9/setup.py`

 * *Files identical despite different names*

