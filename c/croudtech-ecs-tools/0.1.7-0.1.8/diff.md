# Comparing `tmp/croudtech-ecs-tools-0.1.7.tar.gz` & `tmp/croudtech-ecs-tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croudtech-ecs-tools-0.1.7.tar", last modified: Tue Oct  4 15:57:56 2022, max compression
+gzip compressed data, was "croudtech-ecs-tools-0.1.8.tar", last modified: Tue Oct  4 16:07:06 2022, max compression
```

## Comparing `croudtech-ecs-tools-0.1.7.tar` & `croudtech-ecs-tools-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 15:57:56.299471 croudtech-ecs-tools-0.1.7/
--rw-r--r--   0 vsts      (1001) docker     (121)    11357 2022-10-04 15:57:25.000000 croudtech-ecs-tools-0.1.7/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)     1942 2022-10-04 15:57:56.299471 croudtech-ecs-tools-0.1.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1370 2022-10-04 15:57:25.000000 croudtech-ecs-tools-0.1.7/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 15:57:56.299471 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-04 15:57:25.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7543 2022-10-04 15:57:25.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools/cli.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3385 2022-10-04 15:57:25.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools/ecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 15:57:56.299471 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     1942 2022-10-04 15:57:56.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      372 2022-10-04 15:57:56.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-04 15:57:56.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       68 2022-10-04 15:57:56.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-10-04 15:57:56.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-10-04 15:57:56.000000 croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-10-04 15:57:56.299471 croudtech-ecs-tools-0.1.7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     1762 2022-10-04 15:57:25.000000 croudtech-ecs-tools-0.1.7/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11357 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)     1942 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1370 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7543 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3386 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/ecs.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1942 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      372 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       68 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      430 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-10-04 16:07:06.000000 croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-10-04 16:07:06.748370 croudtech-ecs-tools-0.1.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)     1762 2022-10-04 16:06:37.000000 croudtech-ecs-tools-0.1.8/setup.py
```

### Comparing `croudtech-ecs-tools-0.1.7/LICENSE` & `croudtech-ecs-tools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-0.1.7/PKG-INFO` & `croudtech-ecs-tools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-0.1.7/README.md` & `croudtech-ecs-tools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-0.1.7/croudtech_ecs_tools/cli.py` & `croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/cli.py`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-0.1.7/croudtech_ecs_tools/ecs.py` & `croudtech-ecs-tools-0.1.8/croudtech_ecs_tools/ecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,11 +79,11 @@
 
     def list_ecs_service_endpoints(self):
         self._ecs_service_endpoints = {}        
         for service in self.services:
             for service_registry_arn in service["serviceRegistries"]:
                 sd = self.servicediscovery_client.get_service(Id=parse_arn(service_registry_arn["registryArn"])["resource"])
                 hostname = ".".join([sd["Service"]["Name"], self.namespaces[sd["Service"]["NamespaceId"]]["Name"]])
-                self._ecs_service_endpoints[hostname] = sd["Service"]["Name"]
+                self._ecs_service_endpoints[hostname] = service["serviceName"]
 
         return self._ecs_service_endpoints
```

### Comparing `croudtech-ecs-tools-0.1.7/croudtech_ecs_tools.egg-info/PKG-INFO` & `croudtech-ecs-tools-0.1.8/croudtech_ecs_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-0.1.7/setup.py` & `croudtech-ecs-tools-0.1.8/setup.py`

 * *Files identical despite different names*

