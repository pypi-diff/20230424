# Comparing `tmp/django_websockets-0.0.8.tar.gz` & `tmp/django_websockets-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_websockets-0.0.8.tar", last modified: Mon Apr 24 14:55:22 2023, max compression
+gzip compressed data, was "django_websockets-0.0.9.tar", last modified: Mon Apr 24 17:42:20 2023, max compression
```

## Comparing `django_websockets-0.0.8.tar` & `django_websockets-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 14:55:22.453704 django_websockets-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-24 14:55:10.000000 django_websockets-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 14:55:10.000000 django_websockets-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:55:22.453704 django_websockets-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.445704 django_websockets-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.445704 django_websockets-0.0.8/src/django_websockets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/consumers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/groups/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/groups/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/management/commands/websockets_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/src/django_websockets/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/horchestration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/teste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/src/django_websockets/transport/
--rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/src/django_websockets/transport/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 17:42:20.746591 django_websockets-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-24 17:42:09.000000 django_websockets-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 17:42:09.000000 django_websockets-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:42:20.750591 django_websockets-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.738591 django_websockets-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.742591 django_websockets-0.0.9/src/django_websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.742591 django_websockets-0.0.9/src/django_websockets/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/consumers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.742591 django_websockets-0.0.9/src/django_websockets/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.742591 django_websockets-0.0.9/src/django_websockets/groups/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/groups/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/src/django_websockets/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/src/django_websockets/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/management/commands/websockets_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/src/django_websockets/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/middlewares/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/middlewares/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/middlewares/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/middlewares/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/src/django_websockets/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/server/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/server/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/server/horchestration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/server/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/teste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/src/django_websockets/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.746591 django_websockets-0.0.9/src/django_websockets/transport/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/transport/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/transport/proto/wstransport_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/transport/proto/wstransport_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-24 17:42:09.000000 django_websockets-0.0.9/src/django_websockets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:42:20.742591 django_websockets-0.0.9/src/django_websockets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 17:42:20.000000 django_websockets-0.0.9/src/django_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 17:42:20.000000 django_websockets-0.0.9/src/django_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:42:20.000000 django_websockets-0.0.9/src/django_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 17:42:20.000000 django_websockets-0.0.9/src/django_websockets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 17:42:20.000000 django_websockets-0.0.9/src/django_websockets.egg-info/top_level.txt
```

### Comparing `django_websockets-0.0.8/PKG-INFO` & `django_websockets-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_websockets
-Version: 0.0.8
+Version: 0.0.9
 Summary: This project is a case study of using Python Websockets as a websocket backend for Django.
 Author-email: JRaylan <jeffersonraylan@gmail.com>
 Project-URL: Homepage, https://github.com/jraylan/django_websockets
 Project-URL: Bug Tracker, https://github.com/jraylan/django_websockets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `django_websockets-0.0.8/README.md` & `django_websockets-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/pyproject.toml` & `django_websockets-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_websockets"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="JRaylan", email="jeffersonraylan@gmail.com" },
 ]
 description = "This project is a case study of using Python Websockets as a websocket backend for Django."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_websockets-0.0.8/src/django_websockets/consumers/__init__.py` & `django_websockets-0.0.9/src/django_websockets/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/groups/__init__.py` & `django_websockets-0.0.9/src/django_websockets/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/groups/backends/__init__.py` & `django_websockets-0.0.9/src/django_websockets/groups/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/management/commands/websockets_server.py` & `django_websockets-0.0.9/src/django_websockets/management/commands/websockets_server.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/middlewares/__init__.py` & `django_websockets-0.0.9/src/django_websockets/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/middlewares/auth.py` & `django_websockets-0.0.9/src/django_websockets/middlewares/auth.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/middlewares/route.py` & `django_websockets-0.0.9/src/django_websockets/middlewares/route.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/middlewares/scope.py` & `django_websockets-0.0.9/src/django_websockets/middlewares/scope.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/middlewares/utils.py` & `django_websockets-0.0.9/src/django_websockets/middlewares/utils.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/server/arguments.py` & `django_websockets-0.0.9/src/django_websockets/server/arguments.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/server/handler.py` & `django_websockets-0.0.9/src/django_websockets/server/handler.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/server/horchestration.py` & `django_websockets-0.0.9/src/django_websockets/server/horchestration.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/server/main.py` & `django_websockets-0.0.9/src/django_websockets/server/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import time
 import traceback
 from typing import Dict
 import signal
 import websockets
 import sys
+import os
 from django_websockets.middlewares.utils import database_sync_to_async
 import django_websockets.server.arguments as arguments
 from django_websockets.server.handler import connection_handler, master_handler
 from concurrent.futures import ProcessPoolExecutor
 from multiprocessing import queues
 
 # Fix multiprocessing error
@@ -22,15 +23,15 @@
 
 
 def __main(bind: arguments.WebsocketBindAddress, handler, settings=None, namespace="", workers_list=None):
 
     from django_websockets.transport import get_channel_layer, channel_layers
     
     async def run():
-
+        loop = asyncio.get_running_loop()
         if settings:
             import django
             import os
 
             if not django.apps.apps.ready:
                 try:
                     os.environ.setdefault("DJANGO_SETTINGS_MODULE", settings)
@@ -49,38 +50,37 @@
                 try:
                     worker_index = int(re.sub(r'[^0-9]', '', namespace)) + 1
                 except ValueError:
                     worker_index = 0
                     
                 target = f"{bind.address}:{bind.port + worker_index}"
                 server = websockets.serve(
-                    handler, bind.address, bind.port + worker_index)
+                    handler, bind.address, bind.port + worker_index, loop=loop)
             else:
                 target = f"{bind.address}:{bind.port}"
                 server = websockets.serve(
-                    handler, bind.address, bind.port)
+                    handler, bind.address, bind.port, loop=loop)
                 
 
         
         print(f'running {namespace} at {target}')
 
         def run_channel_layer(layer):
             if namespace == 'master':
-                return asyncio.ensure_future(get_channel_layer(using=layer).as_forwarder(namespace=namespace, workers_queue=workers_list))
+                return get_channel_layer(using=layer).as_forwarder(namespace=namespace, workers_queue=workers_list)
             else:
-                return asyncio.ensure_future(get_channel_layer(using=layer).as_server(namespace=namespace))
+                return get_channel_layer(using=layer).as_server(namespace=namespace)
 
         try:
             async with server:
-
                 futures_stack = [
                     run_channel_layer(layer)
                     for layer in channel_layers
                 ]
-                await asyncio.wait(futures_stack, return_when=asyncio.FIRST_COMPLETED)
+                await asyncio.gather(*futures_stack, return_exceptions=True)
 
         except asyncio.CancelledError:
             pass
 
         print(f"leaving {namespace}...")
 
     has_event_loop = False
@@ -172,15 +172,14 @@
     master_worker.cancel()
 
 
 
 def main(bind: arguments.WebsocketBindAddress, settings=None, workers=1):
     if settings:
         import django
-        import os
         os.environ.setdefault("DJANGO_SETTINGS_MODULE", settings)
         django.setup()
     
     if workers == 1:
         return __main(bind, connection_handler)
     
     stop_event =  {}
```

### Comparing `django_websockets-0.0.8/src/django_websockets/setup.py` & `django_websockets-0.0.9/src/django_websockets/setup.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/transport/__init__.py` & `django_websockets-0.0.9/src/django_websockets/transport/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django_websockets.groups.backends import BaseGroupBackend
 from django_websockets.transport.proto import wstransport_pb2_grpc, wstransport_pb2
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 from typing import Any, Union
 import grpc.aio as grpc
+import grpc as sync_grpc
 import re
 
 
 class TransportConfig(dict):
     __inited = False
 
     def __init__(self, dict:dict):
@@ -194,15 +195,17 @@
             for worker in self._workers_queue:
                 if worker in self._stubs:
                     stub = self._stubs[worker]
                 else:
                     address = self.get_namespaced_address(worker)
                     conn = grpc.insecure_channel(address)
                     stub = wstransport_pb2_grpc.WSGroupManagerStub(conn)
-                    self._stubs[worker] = stub                    
+                    self._stubs[worker] = stub
+                await stub.SendMessage(request)
+
             return wstransport_pb2.WSResponse(ack=True)
 
         return wstransport_pb2.WSResponse(ack=False)
 
 
 class gGPCTransportLayer(BaseTransportLayer, wstransport_pb2_grpc.WSGroupManagerServicer):
 
@@ -272,73 +275,95 @@
         # It's necessary to access self.connection to ensure
         # it's instantiate
         self.connection
         return self.__stub
     
     @property
     def connection(self):
-        if self.__connection and self.__stub:
+        if self.__connection:
             return self.__connection
         
         if self.role in [SERVER, FORWARDER]:
-            self.__connection = grpc.server(maximum_concurrent_rpcs=100)
+            self.__connection = grpc.server(
+                maximum_concurrent_rpcs=self.num_connections)
             self.__connection.add_insecure_port(self.address)
             wstransport_pb2_grpc.add_WSGroupManagerServicer_to_server(
                 self, self.__connection)
+            self.__stub = self
             
-            if self.role is SERVER and self._namespace:
-                address = self.config.address
-                conn = grpc.insecure_channel(address)
-                self.__stub = wstransport_pb2_grpc.WSGroupManagerStub(
-                    conn)
-            else:
-                self.__stub = self
+            if self.role is SERVER:
+                if self._namespace:
+                    # If is server and has namespace, stub is the forwarder server
+                    address = self.config.address or "unix:/tmp/rpc.socket"
+                    self.__stub = wstransport_pb2_grpc.WSGroupManagerStub(
+                        sync_grpc.insecure_channel(address))
         else:
-            self.__connection = grpc.insecure_channel(self.address)
+            self.__connection = sync_grpc.insecure_channel(self.address)
             self.__stub = wstransport_pb2_grpc.WSGroupManagerStub(
                 self.__connection)
+            
         return self.__connection
     
 
     async def group_send(self, group:str, message:Union[dict, GroupMessage]):
         '''
         Broadcast a message 
         '''
 
-        # If its a SERVER, we don't need to call RPC
-        # (What about horizontaly scaling???)
         if self.role is FORWARDER:
+            # Fowards the message to to all workers
             await self.forward_stub.SendMessage(
                 wstransport_pb2.WSSendMessageRequest(
                     group=group,
                     message=wstransport_pb2.WSMessage(
                         **message
                     )))
-        elif self.role is SERVER and not self._namespace:
-            return await super().group_send(message)
+        elif self.role is SERVER:
+            if self._namespace:
+                # If it has namespace, redirext message to forwarder
+                self.stub.SendMessage(
+                    wstransport_pb2.WSSendMessageRequest(
+                        group=group,
+                        message=wstransport_pb2.WSMessage(
+                            **message
+                        )))
+            else:
+                # Otherwise, dispatch to groups
+                return print("2.2", await super().group_send(message))
         else:
-            await self.stub.SendMessage(
+            # Send message to the forwarder/server
+            self.stub.SendMessage(
                 wstransport_pb2.WSSendMessageRequest(
                     group=group,
                     message=wstransport_pb2.WSMessage(
                         **message
                     )))
     
     async def __call__(self, namespace, workers_queue=None):
+        '''
+        Starts the layer
+
+        *namespace*: The namespace of the current layer. Used for multi
+        workers.
+
+        *workers_queue*: list of current workers
+
+        '''
         try:
             self._namespace = namespace
             self._workers_queue = workers_queue
             if self.role in [SERVER, FORWARDER]:
                 self.__connection = None
                 await self.connection.start()
                 await self.connection.wait_for_termination()
                 return 'ok'
 
             return self.role
         except Exception as e:
+            traceback.print_exc()
             return e
 
     async def stop(self):
         if self.role in [SERVER, FORWARDER]:
             self.connection.stop()
```

### Comparing `django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2.py` & `django_websockets-0.0.9/src/django_websockets/transport/proto/wstransport_pb2.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2_grpc.py` & `django_websockets-0.0.9/src/django_websockets/transport/proto/wstransport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets/utils.py` & `django_websockets-0.0.9/src/django_websockets/utils.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.8/src/django_websockets.egg-info/PKG-INFO` & `django_websockets-0.0.9/src/django_websockets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-websockets
-Version: 0.0.8
+Version: 0.0.9
 Summary: This project is a case study of using Python Websockets as a websocket backend for Django.
 Author-email: JRaylan <jeffersonraylan@gmail.com>
 Project-URL: Homepage, https://github.com/jraylan/django_websockets
 Project-URL: Bug Tracker, https://github.com/jraylan/django_websockets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `django_websockets-0.0.8/src/django_websockets.egg-info/SOURCES.txt` & `django_websockets-0.0.9/src/django_websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

