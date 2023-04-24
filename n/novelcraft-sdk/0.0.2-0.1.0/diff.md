# Comparing `tmp/novelcraft_sdk-0.0.2.tar.gz` & `tmp/novelcraft_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelcraft_sdk-0.0.2.tar", max compression
+gzip compressed data, was "novelcraft_sdk-0.1.0.tar", max compression
```

## Comparing `novelcraft_sdk-0.0.2.tar` & `novelcraft_sdk-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1211 2023-04-13 14:59:03.030990 novelcraft_sdk-0.0.2/LICENSE
--rw-r--r--   0        0        0     1132 2023-04-13 14:59:03.030990 novelcraft_sdk-0.0.2/README.md
--rw-r--r--   0        0        0      396 2023-04-13 14:59:03.030990 novelcraft_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       43 2023-04-13 14:59:03.030990 novelcraft_sdk-0.0.2/src/novelcraft/__init__.py
--rw-r--r--   0        0        0      729 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/__init__.py
--rw-r--r--   0        0        0     5942 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/agent.py
--rw-r--r--   0        0        0     1030 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/block.py
--rw-r--r--   0        0        0     2690 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/block_source.py
--rw-r--r--   0        0        0     3203 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/client.py
--rw-r--r--   0        0        0     1981 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/entity.py
--rw-r--r--   0        0        0     1652 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/entity_source.py
--rw-r--r--   0        0        0     6173 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/inventory.py
--rw-r--r--   0        0        0     1091 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/item_stack.py
--rw-r--r--   0        0        0     2917 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/logger.py
--rw-r--r--   0        0        0     2298 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/message.py
--rw-r--r--   0        0        0      353 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/orientation.py
--rw-r--r--   0        0        0      389 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/position.py
--rw-r--r--   0        0        0    13564 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/sdk.py
--rw-r--r--   0        0        0     1372 2023-04-13 14:59:03.034989 novelcraft_sdk-0.0.2/src/novelcraft/sdk/section.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 novelcraft_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-24 02:28:54.242174 novelcraft_sdk-0.1.0/LICENSE
+-rw-r--r--   0        0        0      806 2023-04-24 02:28:54.242174 novelcraft_sdk-0.1.0/README.md
+-rw-r--r--   0        0        0      604 2023-04-24 02:28:54.242174 novelcraft_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/__init__.py
+-rw-r--r--   0        0        0     5942 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/agent.py
+-rw-r--r--   0        0        0     1030 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/block.py
+-rw-r--r--   0        0        0     2690 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/block_source.py
+-rw-r--r--   0        0        0     3203 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/client.py
+-rw-r--r--   0        0        0     1981 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity.py
+-rw-r--r--   0        0        0     1652 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity_source.py
+-rw-r--r--   0        0        0     6173 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/inventory.py
+-rw-r--r--   0        0        0     1091 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/item_stack.py
+-rw-r--r--   0        0        0     2917 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/logger.py
+-rw-r--r--   0        0        0     2298 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/message.py
+-rw-r--r--   0        0        0      353 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/orientation.py
+-rw-r--r--   0        0        0      389 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/position.py
+-rw-r--r--   0        0        0    13588 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/sdk.py
+-rw-r--r--   0        0        0     1372 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/section.py
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 novelcraft_sdk-0.1.0/PKG-INFO
```

### Comparing `novelcraft_sdk-0.0.2/LICENSE` & `novelcraft_sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/__init__.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/agent.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/agent.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/block.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/block.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/block_source.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/block_source.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/client.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/client.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/entity.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/entity_source.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity_source.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/inventory.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/inventory.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/item_stack.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/item_stack.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/logger.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/logger.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/message.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/message.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/sdk.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """The SDK APIs.
 
-The SDK API is the root of all APIs provided by the SDK. It is the entry
-point of the SDK.
+Here is an example of how to use the SDK APIs:
+```python
+import novelcraft.sdk as sdk
+
+agent = sdk.get_agent()
+```
 """
 
 from __future__ import annotations
 
 import argparse
 import asyncio
 from dataclasses import dataclass
```

### Comparing `novelcraft_sdk-0.0.2/src/novelcraft/sdk/section.py` & `novelcraft_sdk-0.1.0/src/novelcraft/sdk/section.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.0.2/PKG-INFO` & `novelcraft_sdk-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: novelcraft-sdk
-Version: 0.0.2
-Summary: 
+Version: 0.1.0
+Summary: A Python library for communicating with NovelCraft Servers and accessing NovelCraft game data
 License: Unlicense
 Author: NovelCraft
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,38 +27,31 @@
 ```bash
 pip install novelcraft.sdk
 ```
 
 ## Usage
 
 ```python
-import novelcraft.sdk as ncsdk
+import asyncio
 
-async def main():
-    await sdk.initialize()
-    get_logger().info('Hello, world!')
+import novelcraft.sdk as sdk
 
-    while True:
-        await asyncio.sleep(0)
 
-        if ncsdk.get_agent() is None:
-            await asyncio.sleep(1)
-            continue
+async def main():
+    await sdk.initialize()
 
-        agent = ncsdk.get_agent()
-        agent.set_movement(IAgent.MovementKind.FORWARD)
+    # Do something
 
     await ncsdk.finalize()
-    ncsdk.get_logger().info('Goodbye, world!')
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-For more information, please refer to the [documentation](https://python.sdk.novelcraft.games).
+For more information, please start with _placeholder_.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

