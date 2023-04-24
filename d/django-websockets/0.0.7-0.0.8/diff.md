# Comparing `tmp/django_websockets-0.0.7.tar.gz` & `tmp/django_websockets-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_websockets-0.0.7.tar", last modified: Fri Apr 21 20:13:07 2023, max compression
+gzip compressed data, was "django_websockets-0.0.8.tar", last modified: Mon Apr 24 14:55:22 2023, max compression
```

## Comparing `django_websockets-0.0.7.tar` & `django_websockets-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.795282 django_websockets-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-21 20:13:07.795282 django_websockets-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-21 20:12:50.000000 django_websockets-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 20:12:50.000000 django_websockets-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:13:07.795282 django_websockets-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.787282 django_websockets-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/consumers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/groups/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/groups/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/management/commands/websockets_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/middlewares/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/middlewares/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/middlewares/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/middlewares/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.795282 django_websockets-0.0.7/src/django_websockets/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/server/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/server/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/server/horchestration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/server/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/teste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.795282 django_websockets-0.0.7/src/django_websockets/transport/
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.795282 django_websockets-0.0.7/src/django_websockets/transport/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/transport/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/transport/proto/wstransport_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/transport/proto/wstransport_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-21 20:12:50.000000 django_websockets-0.0.7/src/django_websockets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:13:07.791282 django_websockets-0.0.7/src/django_websockets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-21 20:13:07.000000 django_websockets-0.0.7/src/django_websockets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-21 20:13:07.000000 django_websockets-0.0.7/src/django_websockets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:13:07.000000 django_websockets-0.0.7/src/django_websockets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 20:13:07.000000 django_websockets-0.0.7/src/django_websockets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 20:13:07.000000 django_websockets-0.0.7/src/django_websockets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 14:55:22.453704 django_websockets-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-24 14:55:10.000000 django_websockets-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 14:55:10.000000 django_websockets-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:55:22.453704 django_websockets-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.445704 django_websockets-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.445704 django_websockets-0.0.8/src/django_websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/consumers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/groups/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/groups/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/management/commands/websockets_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/middlewares/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/src/django_websockets/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/horchestration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/teste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/src/django_websockets/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.453704 django_websockets-0.0.8/src/django_websockets/transport/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-24 14:55:10.000000 django_websockets-0.0.8/src/django_websockets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:55:22.449705 django_websockets-0.0.8/src/django_websockets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:55:22.000000 django_websockets-0.0.8/src/django_websockets.egg-info/top_level.txt
```

### Comparing `django_websockets-0.0.7/PKG-INFO` & `django_websockets-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_websockets
-Version: 0.0.7
+Version: 0.0.8
 Summary: This project is a case study of using Python Websockets as a websocket backend for Django.
 Author-email: JRaylan <jeffersonraylan@gmail.com>
 Project-URL: Homepage, https://github.com/jraylan/django_websockets
 Project-URL: Bug Tracker, https://github.com/jraylan/django_websockets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `django_websockets-0.0.7/README.md` & `django_websockets-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/pyproject.toml` & `django_websockets-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_websockets"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="JRaylan", email="jeffersonraylan@gmail.com" },
 ]
 description = "This project is a case study of using Python Websockets as a websocket backend for Django."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_websockets-0.0.7/src/django_websockets/consumers/__init__.py` & `django_websockets-0.0.8/src/django_websockets/consumers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import inspect
 import traceback
-from typing import AsyncIterable, Awaitable, Callable, Dict, Iterable, Set, Type, Union
+from typing import AsyncIterable, Awaitable, Callable, Coroutine, Dict, Iterable, Set, Type, Union
 import warnings
 import websockets
 from websockets.server import WebSocketServerProtocol
 from websockets.typing import Data
 import asyncio
 import functools
 from django_websockets.groups import GroupMessage
-from django_websockets.utils import async_partial
+
 
 
 class StopConsumer(Exception): ...
 
 
 class BaseConsumer(object):
     """
@@ -37,14 +37,19 @@
     @property
     def __process_message_timeout(self):
         try:
             return int(self.get_process_message_timeout())
         except:
             return 0
 
+    @property
+    def channel_layer(self):
+        from django_websockets.transport import get_channel_layer
+        return get_channel_layer()
+
     async def __process(self, message: GroupMessage):
         if not isinstance(message, GroupMessage):
             try:
                 message = GroupMessage(**message)
             except:
                 warnings.warn(
                     "Consumer '{}' received a group message that is not a instance of 'GroupMessage'"
@@ -101,25 +106,26 @@
                     return True
             
             self.__group_queues[group_name] = group_queue
             self.__group_callbacks[group_name] = on_stop
             
         return True
 
-    async def _stop_listen_to_group(self, group_name:str):
+    async def _stop_listen_to_group(self, group_name:str, run_callback=True):
         """
         Pop the task from the groups and listeners maps and wait for the task to finish
         """
         callback = None
         async with self.__group_lock:
             callback = self.__group_callbacks.pop(group_name, None)
             self.__group_queues.pop(group_name, None)
             
-        if callback:
-            await asyncio.wait_for(callback(), timeout=1)
+        if run_callback and callback:
+            callback_coroutine = callback()
+            await callback_coroutine
         
         return group_name
 
         
     async def __dispose(self):
         """
         Mark consumer as closing and cleanup all tasks
@@ -295,15 +301,15 @@
         message: Union[Data, Iterable[Data], AsyncIterable[Data]]): ...
 
     @classmethod
     def as_handler(cls, **initkwargs):
 
         async def app(websocket, *args, **kwargs):
             consumer = cls(**initkwargs)
-            consumer.send = async_partial(consumer.__send, websocket)
+            consumer.send = functools.partial(consumer.__send, websocket)
             functools.update_wrapper(consumer.send, websocket.send)
             return await consumer(websocket, *args, **kwargs)
 
         app.consumer_class = cls
         app.consumer_initkwargs = initkwargs
 
         # take name and docstring from class
```

### Comparing `django_websockets-0.0.7/src/django_websockets/groups/__init__.py` & `django_websockets-0.0.8/src/django_websockets/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/groups/backends/__init__.py` & `django_websockets-0.0.8/src/django_websockets/groups/backends/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
+from functools import partial
 from typing import Dict, NoReturn, Set
 import warnings
 from django_websockets.consumers import BaseConsumer
-from django_websockets.utils import async_partial
+
 from django_websockets.groups import GroupMessage
 
 class BaseGroupBackend(object):
     __group_listeners_lock: asyncio.Lock = asyncio.Lock()
     __group_listeners: Dict[str, Set[asyncio.Queue]] = {}
 
     def __init__(self, prefix=""):
@@ -48,15 +49,15 @@
         async with self.__group_listeners_lock:
             if group_name not in self.__group_listeners:
                 self.__group_listeners[group_name]: Set[asyncio.Queue] = set()
         
         queue = asyncio.Queue()
     
         # Callback to remove queue from list
-        on_stop = async_partial(self.__on_stop, group_name, queue)
+        on_stop = partial(self.__on_stop, group_name, queue)
 
         self.__group_listeners[group_name].add(queue)
         
         response = await consumer._listen_to_group(group_name, queue, on_stop)
         # if consumer returns false, call on_stop()
         if not response:
             await on_stop()
@@ -66,16 +67,19 @@
         Make consumer stop listening go a group and remove the group queue
         """
 
         # Wraped group name
         group_name = self.__get_group_name(group_name)
 
         async with self.__group_listeners_lock:
-            await consumer._stop_listen_to_group(group_name)
-            await self.__on_stop(group_name, consumer)
+            try:
+                await consumer._stop_listen_to_group(group_name, False)
+                await self.__on_stop(group_name, consumer)
+            except RuntimeError:
+                pass
 
     async def group_message(self, name, message: GroupMessage):
         """
         Send message put the message in all queues from a group
         """
 
         # Wraped group name
```

### Comparing `django_websockets-0.0.7/src/django_websockets/management/commands/websockets_server.py` & `django_websockets-0.0.8/src/django_websockets/management/commands/websockets_server.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/middlewares/__init__.py` & `django_websockets-0.0.8/src/django_websockets/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/middlewares/auth.py` & `django_websockets-0.0.8/src/django_websockets/middlewares/auth.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/middlewares/route.py` & `django_websockets-0.0.8/src/django_websockets/middlewares/route.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/middlewares/scope.py` & `django_websockets-0.0.8/src/django_websockets/middlewares/scope.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/middlewares/utils.py` & `django_websockets-0.0.8/src/django_websockets/middlewares/utils.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/server/arguments.py` & `django_websockets-0.0.8/src/django_websockets/server/arguments.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/server/horchestration.py` & `django_websockets-0.0.8/src/django_websockets/server/horchestration.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/setup.py` & `django_websockets-0.0.8/src/django_websockets/setup.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/transport/__init__.py` & `django_websockets-0.0.8/src/django_websockets/transport/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from django_websockets.groups import GroupMessage
 from django_websockets.groups.backends import BaseGroupBackend
 from django_websockets.transport.proto import wstransport_pb2_grpc, wstransport_pb2
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 from typing import Any, Union
-import grpc as sync_grpc
 import grpc.aio as grpc
 import re
 
 
 class TransportConfig(dict):
     __inited = False
 
@@ -195,17 +194,15 @@
             for worker in self._workers_queue:
                 if worker in self._stubs:
                     stub = self._stubs[worker]
                 else:
                     address = self.get_namespaced_address(worker)
                     conn = grpc.insecure_channel(address)
                     stub = wstransport_pb2_grpc.WSGroupManagerStub(conn)
-                    self._stubs[worker] = stub
-                await stub.SendMessage(request)
-                    
+                    self._stubs[worker] = stub                    
             return wstransport_pb2.WSResponse(ack=True)
 
         return wstransport_pb2.WSResponse(ack=False)
 
 
 class gGPCTransportLayer(BaseTransportLayer, wstransport_pb2_grpc.WSGroupManagerServicer):
 
@@ -230,17 +227,24 @@
                     address = f'{address}{self._namespace}.sock'
                 else:
                     address = f'{address}{self._namespace}.socket'
         return address
     
     @property
     def graceful(self):
-        return self.config.num_connections or 0
+        return self.config.gareceul or 0
     
-    async def SendMessage(self, request, context):
+    async def group_add(self, group, consumer):
+        await super().group_add(group, consumer)
+
+    async def group_discard(self, group, consumer):
+        await super().group_discard(group, consumer)
+
+
+    async def SendMessage(self, request, context=None):
         message = GroupMessage(
             request.message.type,
             request.message.message
         )
 
         try:
             if self.role is FORWARDER:
@@ -268,49 +272,55 @@
         # It's necessary to access self.connection to ensure
         # it's instantiate
         self.connection
         return self.__stub
     
     @property
     def connection(self):
-        if self.__connection:
+        if self.__connection and self.__stub:
             return self.__connection
         
         if self.role in [SERVER, FORWARDER]:
-            self.__connection = grpc.server(
-                futures.ThreadPoolExecutor(max_workers=self.num_connections))
+            self.__connection = grpc.server(maximum_concurrent_rpcs=100)
             self.__connection.add_insecure_port(self.address)
-            self.__stub = wstransport_pb2_grpc.add_WSGroupManagerServicer_to_server(
+            wstransport_pb2_grpc.add_WSGroupManagerServicer_to_server(
                 self, self.__connection)
+            
+            if self.role is SERVER and self._namespace:
+                address = self.config.address
+                conn = grpc.insecure_channel(address)
+                self.__stub = wstransport_pb2_grpc.WSGroupManagerStub(
+                    conn)
+            else:
+                self.__stub = self
         else:
-            self.__connection = sync_grpc.insecure_channel(self.address)
-            self.__stub = wstransport_pb2_grpc.WSGroupManagerStub(self.__connection)
+            self.__connection = grpc.insecure_channel(self.address)
+            self.__stub = wstransport_pb2_grpc.WSGroupManagerStub(
+                self.__connection)
         return self.__connection
     
 
     async def group_send(self, group:str, message:Union[dict, GroupMessage]):
         '''
         Broadcast a message 
         '''
 
         # If its a SERVER, we don't need to call RPC
         # (What about horizontaly scaling???)
-        if self.role is SERVER:
-            return await super().group_send(group, message)
-        
-        elif self.role is FORWARDER:
-            self.forward_stub.SendMessage(
+        if self.role is FORWARDER:
+            await self.forward_stub.SendMessage(
                 wstransport_pb2.WSSendMessageRequest(
                     group=group,
                     message=wstransport_pb2.WSMessage(
                         **message
                     )))
-        
+        elif self.role is SERVER and not self._namespace:
+            return await super().group_send(message)
         else:
-            self.stub.SendMessage(
+            await self.stub.SendMessage(
                 wstransport_pb2.WSSendMessageRequest(
                     group=group,
                     message=wstransport_pb2.WSMessage(
                         **message
                     )))
     
     async def __call__(self, namespace, workers_queue=None):
```

### Comparing `django_websockets-0.0.7/src/django_websockets/transport/proto/wstransport_pb2.py` & `django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/transport/proto/wstransport_pb2_grpc.py` & `django_websockets-0.0.8/src/django_websockets/transport/proto/wstransport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets/utils.py` & `django_websockets-0.0.8/src/django_websockets/utils.py`

 * *Files identical despite different names*

### Comparing `django_websockets-0.0.7/src/django_websockets.egg-info/PKG-INFO` & `django_websockets-0.0.8/src/django_websockets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-websockets
-Version: 0.0.7
+Version: 0.0.8
 Summary: This project is a case study of using Python Websockets as a websocket backend for Django.
 Author-email: JRaylan <jeffersonraylan@gmail.com>
 Project-URL: Homepage, https://github.com/jraylan/django_websockets
 Project-URL: Bug Tracker, https://github.com/jraylan/django_websockets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `django_websockets-0.0.7/src/django_websockets.egg-info/SOURCES.txt` & `django_websockets-0.0.8/src/django_websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

