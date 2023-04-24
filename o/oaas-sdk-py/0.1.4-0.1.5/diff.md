# Comparing `tmp/oaas_sdk_py-0.1.4.tar.gz` & `tmp/oaas_sdk_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.1.4.tar", last modified: Sun Apr 16 05:52:02 2023, max compression
+gzip compressed data, was "oaas_sdk_py-0.1.5.tar", last modified: Mon Apr 24 10:23:26 2023, max compression
```

## Comparing `oaas_sdk_py-0.1.4.tar` & `oaas_sdk_py-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 05:52:02.544505 oaas_sdk_py-0.1.4/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      258 2023-04-16 05:52:02.544505 oaas_sdk_py-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.4/README.md
--rw-rw-rw-   0        0        0      495 2023-04-16 05:49:05.000000 oaas_sdk_py-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 05:52:02.544505 oaas_sdk_py-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 05:52:02.532063 oaas_sdk_py-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 05:52:02.537067 oaas_sdk_py-0.1.4/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     8897 2023-04-16 05:49:05.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1740 2023-04-14 09:02:39.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2023-04-16 05:52:02.542094 oaas_sdk_py-0.1.4/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-04-16 05:52:02.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-16 05:52:02.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 05:52:02.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-16 05:52:02.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 05:52:02.000000 oaas_sdk_py-0.1.4/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:26.960773 oaas_sdk_py-0.1.5/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      258 2023-04-24 10:23:26.959773 oaas_sdk_py-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.5/README.md
+-rw-rw-rw-   0        0        0      495 2023-04-24 10:23:04.000000 oaas_sdk_py-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:23:26.960773 oaas_sdk_py-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:26.946593 oaas_sdk_py-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:26.951913 oaas_sdk_py-0.1.5/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     8911 2023-04-24 10:22:35.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1740 2023-04-14 09:02:39.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:23:26.958776 oaas_sdk_py-0.1.5/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-04-24 10:23:26.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-24 10:23:26.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:23:26.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-24 10:23:26.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 10:23:26.000000 oaas_sdk_py-0.1.5/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.1.4/LICENSE` & `oaas_sdk_py-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.4/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.1.5/src/oaas_sdk_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import asyncio
 import json
 from abc import abstractmethod
-from asyncio import StreamReader
 from typing import Dict, List
-import aiofiles.os
+
 import aiofiles
-import aiohttp
+import aiofiles.os
 from aiohttp import ClientSession, ClientResponse
 
 from .model import *
 
 
 class OaasException(BaseException):
     pass
 
 
-async def load_file(url: str) -> ClientResponse:
-    async with aiohttp.ClientSession() as session:
-        resp = await session.get(url)
-        if not resp.ok:
-            raise OaasException("Got error when get the data to S3")
-        return resp
+async def _load_file(session: ClientSession,
+                     url: str) -> ClientResponse:
+    resp = await session.get(url)
+    if not resp.ok:
+        raise OaasException("Got error when get the data to S3")
+    return resp
 
 
 async def _allocate(session: ClientSession,
                     url):
     client_resp = await session.get(url)
     if not client_resp.ok:
         raise OaasException("Got error when allocate keys")
@@ -106,17 +105,17 @@
             raise OaasException(f"The output object not accept '{key}' as key")
         resp = await session.put(url, data=data)
         if not resp.ok:
             raise OaasException("Got error when put the data to S3")
         self.task.output_obj.updated_keys.append(key)
 
     async def upload_main_byte_data(self,
-                               session: ClientSession,
-                               key: str,
-                               data: bytearray) -> None:
+                                    session: ClientSession,
+                                    key: str,
+                                    data: bytearray) -> None:
         if self.allocate_main_url_dict is None:
             await self.allocate_main_file(session)
         url = self.allocate_main_url_dict[key]
         if url is None:
             raise OaasException(f"The main object not accept '{key}' as key")
         resp = await session.put(url, data=data)
         if not resp.ok:
@@ -151,25 +150,25 @@
                                 session: ClientSession,
                                 key_to_file: Dict[str, str]) -> None:
         await self.allocate_collection(session, list(key_to_file.keys()))
         promise_list = [self.upload_file(session, k, v) for k, v in key_to_file.items()]
         self.task.output_obj.updated_keys.extend(list(key_to_file.keys()))
         await asyncio.gather(*promise_list)
 
-    async def load_main_file(self, key: str) -> ClientResponse:
+    async def load_main_file(self, session: ClientSession, key: str) -> ClientResponse:
         if key not in self.task.main_keys:
             raise OaasException(f"NO such key '{key}' in main object")
-        return await load_file(self.task.main_keys[key])
+        return await _load_file(session, self.task.main_keys[key])
 
-    async def load_input_file(self, input_index: int, key: str) -> ClientResponse:
+    async def load_input_file(self, session: ClientSession, input_index: int, key: str) -> ClientResponse:
         if input_index > len(self.task.input_keys):
             raise OaasException(f"Input index {input_index} out of range({len(self.task.input_keys)})")
         if key not in self.task.input_keys[input_index]:
             raise OaasException(f"No such key '{key}' in input object")
-        return await load_file(self.task.input_keys[input_index][key])
+        return await _load_file(session, self.task.input_keys[input_index][key])
 
     def create_completion(self,
                           main_data: Dict = None,
                           output_data: Dict = None):
         main_update = {}
         if not self.task.immutable:
             if main_data is None:
```

### Comparing `oaas_sdk_py-0.1.4/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.1.5/src/oaas_sdk_py/model.py`

 * *Files identical despite different names*

