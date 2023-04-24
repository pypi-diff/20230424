# Comparing `tmp/zigpy-xbee-0.17.0.tar.gz` & `tmp/zigpy-xbee-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-xbee-0.17.0.tar", last modified: Thu Mar 30 19:40:31 2023, max compression
+gzip compressed data, was "zigpy-xbee-0.18.0.tar", last modified: Mon Apr 24 18:12:50 2023, max compression
```

## Comparing `zigpy-xbee-0.17.0.tar` & `zigpy-xbee-0.18.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:40:31.674345 zigpy-xbee-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-03-30 19:40:31.674345 zigpy-xbee-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-30 19:40:31.674345 zigpy-xbee-0.17.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:40:31.670345 zigpy-xbee-0.17.0/zigpy_xbee/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:40:31.674345 zigpy-xbee-0.17.0/zigpy_xbee/zigbee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-03-30 19:40:25.000000 zigpy-xbee-0.17.0/zigpy_xbee/zigbee/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:40:31.674345 zigpy-xbee-0.17.0/zigpy_xbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-03-30 19:40:31.000000 zigpy-xbee-0.17.0/zigpy_xbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-30 19:40:31.000000 zigpy-xbee-0.17.0/zigpy_xbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:40:31.000000 zigpy-xbee-0.17.0/zigpy_xbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 19:40:31.000000 zigpy-xbee-0.17.0/zigpy_xbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-30 19:40:31.000000 zigpy-xbee-0.17.0/zigpy_xbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/zigpy_xbee/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/zigpy_xbee/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-24 18:12:46.000000 zigpy-xbee-0.18.0/zigpy_xbee/zigbee/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:12:50.370391 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 18:12:50.000000 zigpy-xbee-0.18.0/zigpy_xbee.egg-info/top_level.txt
```

### Comparing `zigpy-xbee-0.17.0/COPYING` & `zigpy-xbee-0.18.0/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/LICENSE` & `zigpy-xbee-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/PKG-INFO` & `zigpy-xbee-0.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-xbee
-Version: 0.17.0
+Version: 0.18.0
 Summary: A library which communicates with XBee radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-xbee
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zigpy-xbee-0.17.0/README.md` & `zigpy-xbee-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/setup.cfg` & `zigpy-xbee-0.18.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/setup.py` & `zigpy-xbee-0.18.0/setup.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/zigpy_xbee/api.py` & `zigpy-xbee-0.18.0/zigpy_xbee/api.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/zigpy_xbee/types.py` & `zigpy-xbee-0.18.0/zigpy_xbee/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/zigpy_xbee/uart.py` & `zigpy-xbee-0.18.0/zigpy_xbee/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-xbee-0.17.0/zigpy_xbee/zigbee/application.py` & `zigpy-xbee-0.18.0/zigpy_xbee/zigbee/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any
 
 import zigpy.application
 import zigpy.config
 import zigpy.device
 import zigpy.exceptions
 import zigpy.quirks
+import zigpy.state
 import zigpy.types
 import zigpy.util
 from zigpy.zcl import foundation
 from zigpy.zcl.clusters.general import Groups
 import zigpy.zdo.types as zdo_t
 
 import zigpy_xbee
@@ -65,21 +66,24 @@
         association_state = await asyncio.wait_for(
             self._get_association_state(), timeout=4
         )
 
         # Enable ZDO passthrough
         await self._api._at_command("AO", 0x03)
 
+        if self.state.node_info == zigpy.state.NodeInfo():
+            await self.load_network_info()
+
         enc_enabled = await self._api._at_command("EE")
         enc_options = await self._api._at_command("EO")
         zb_profile = await self._api._at_command("ZS")
 
         if (
             enc_enabled != 1
-            or enc_options != 2
+            or enc_options & 0b0010 != 0b0010
             or zb_profile != 2
             or association_state != 0
             or self.state.node_info.nwk != 0x0000
         ):
             raise zigpy.exceptions.NetworkNotFormed("Network is not formed")
 
         # Disable joins
@@ -130,24 +134,26 @@
         )
         network_info.channel = await self._api._at_command("CH")
 
     async def reset_network_info(self) -> None:
         await self._api._at_command("NR", 0)
 
     async def write_network_info(self, *, network_info, node_info):
-        scan_bitmask = 1 << (network_info.channel - 11)
+        epid, _ = zigpy.types.uint64_t.deserialize(
+            network_info.extended_pan_id.serialize()
+        )
+        await self._api._queued_at("ID", epid)
 
         await self._api._queued_at("ZS", 2)
+        scan_bitmask = 1 << (network_info.channel - 11)
         await self._api._queued_at("SC", scan_bitmask)
         await self._api._queued_at("EE", 1)
-        await self._api._queued_at("EO", 2)
-
+        await self._api._queued_at("EO", 0b0010)
         await self._api._queued_at("NK", network_info.network_key.key.serialize())
         await self._api._queued_at("KY", network_info.tc_link_key.key.serialize())
-
         await self._api._queued_at("NJ", 0)
         await self._api._queued_at("SP", CONF_CYCLIC_SLEEP_PERIOD)
         await self._api._queued_at("SN", CONF_POLL_TIMEOUT)
 
         try:
             await self._api._queued_at("CE", 1)
         except RuntimeError:
@@ -157,14 +163,21 @@
 
         await asyncio.wait_for(self._api.coordinator_started_event.wait(), timeout=10)
         association_state = await asyncio.wait_for(
             self._get_association_state(), timeout=10
         )
         LOGGER.debug("Association state: %s", association_state)
 
+    async def _move_network_to_channel(
+        self, new_channel: int, new_nwk_update_id: int
+    ) -> None:
+        """Moves the coordinator to a new channel."""
+        scan_bitmask = 1 << (new_channel - 11)
+        await self._api._queued_at("SC", scan_bitmask)
+
     async def force_remove(self, dev):
         """Forcibly remove device from NCP."""
         pass
 
     async def add_endpoint(self, descriptor):
         """Register a new endpoint on the device."""
         # This is not provided by the XBee API
```

### Comparing `zigpy-xbee-0.17.0/zigpy_xbee.egg-info/PKG-INFO` & `zigpy-xbee-0.18.0/zigpy_xbee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-xbee
-Version: 0.17.0
+Version: 0.18.0
 Summary: A library which communicates with XBee radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-xbee
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

