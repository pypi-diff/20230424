# Comparing `tmp/zigpy-deconz-0.9.2.tar.gz` & `tmp/zigpy-deconz-0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zigpy-deconz-0.9.2.tar", last modified: Fri May  8 20:09:19 2020, max compression
+gzip compressed data, was "dist/zigpy-deconz-0.9a1.tar", last modified: Mon Apr 13 17:56:38 2020, max compression
```

## Comparing `zigpy-deconz-0.9.2.tar` & `zigpy-deconz-0.9a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-08 20:09:19.359813 zigpy-deconz-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)     3906 2020-05-08 20:09:19.359813 zigpy-deconz-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3128 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      536 2020-05-08 20:09:19.359813 zigpy-deconz-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      845 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-08 20:09:19.355813 zigpy-deconz-0.9.2/zigpy_deconz/
--rw-r--r--   0 runner    (1001) docker     (116)      200 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18352 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/api.py
--rw-r--r--   0 runner    (1001) docker     (116)      427 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      266 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/exception.py
--rw-r--r--   0 runner    (1001) docker     (116)     6542 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/types.py
--rw-r--r--   0 runner    (1001) docker     (116)     4212 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-08 20:09:19.359813 zigpy-deconz-0.9.2/zigpy_deconz/zigbee/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12661 2020-05-08 20:09:17.000000 zigpy-deconz-0.9.2/zigpy_deconz/zigbee/application.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-08 20:09:19.359813 zigpy-deconz-0.9.2/zigpy_deconz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3906 2020-05-08 20:09:19.000000 zigpy-deconz-0.9.2/zigpy_deconz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      411 2020-05-08 20:09:19.000000 zigpy-deconz-0.9.2/zigpy_deconz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-08 20:09:19.000000 zigpy-deconz-0.9.2/zigpy_deconz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-05-08 20:09:19.000000 zigpy-deconz-0.9.2/zigpy_deconz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2020-05-08 20:09:19.000000 zigpy-deconz-0.9.2/zigpy_deconz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-13 17:56:38.366121 zigpy-deconz-0.9a1/
+-rw-r--r--   0 runner    (1001) docker     (116)     3068 2020-04-13 17:56:38.366121 zigpy-deconz-0.9a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2466 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      536 2020-04-13 17:56:38.366121 zigpy-deconz-0.9a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      845 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-13 17:56:38.362121 zigpy-deconz-0.9a1/zigpy_deconz/
+-rw-r--r--   0 runner    (1001) docker     (116)      201 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17840 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      408 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/exception.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6542 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4212 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-13 17:56:38.366121 zigpy-deconz-0.9a1/zigpy_deconz/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12146 2020-04-13 17:56:28.000000 zigpy-deconz-0.9a1/zigpy_deconz/zigbee/application.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-13 17:56:38.366121 zigpy-deconz-0.9a1/zigpy_deconz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3068 2020-04-13 17:56:38.000000 zigpy-deconz-0.9a1/zigpy_deconz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      411 2020-04-13 17:56:38.000000 zigpy-deconz-0.9a1/zigpy_deconz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-13 17:56:38.000000 zigpy-deconz-0.9a1/zigpy_deconz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2020-04-13 17:56:38.000000 zigpy-deconz-0.9a1/zigpy_deconz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2020-04-13 17:56:38.000000 zigpy-deconz-0.9a1/zigpy_deconz.egg-info/top_level.txt
```

### Comparing `zigpy-deconz-0.9.2/PKG-INFO` & `zigpy-deconz-0.9a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-deconz
-Version: 0.9.2
+Version: 0.9a1
 Summary: A library which communicates with Deconz radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-deconz
 Author: Daniel Schmidt
 Author-email: schmidt.d@aon.at
 License: GPL-3.0
 Description: # zigpy-deconz
         
@@ -13,36 +13,14 @@
         
         [zigpy-deconz](https://github.com/zigpy/zigpy-deconz) is a Python 3 implementation for the [Zigpy](https://github.com/zigpy/) project to implement [deCONZ](https://www.dresden-elektronik.de/funktechnik/products/software/pc/deconz/) based [Zigbee](https://www.zigbee.org) radio devices.
         
         The goal of this project to add native support for the Dresden-Elektronik deCONZ based ZigBee modules in Home Assistant via [Zigpy](https://github.com/zigpy/).
         
         This library uses the deCONZ serial protocol for communicating with [ConBee](https://www.dresden-elektronik.de/conbee/), [ConBee II (ConBee 2)](https://shop.dresden-elektronik.de/conbee-2.html), and [RaspBee](https://www.dresden-elektronik.de/raspbee/) adapters from [Dresden-Elektronik](https://github.com/dresden-elektronik/).
         
-        # Testing new releases
-        
-        Testing a new release of the zigpy-deconz library before it is released in Home Assistant.
-        
-        If you are using Supervised Home Assistant (formerly known as the Hassio/Hass.io distro):
-        - Add https://github.com/home-assistant/hassio-addons-development as "add-on" repository
-        - Install "Custom deps deployment" addon
-        - Update config like: 
-          ```
-          pypi:
-            - zigpy-deconz==0.9.0
-          apk: []
-          ```
-          where 0.5.1 is the new version
-        - Start the addon
-        
-        If you are instead using some custom python installation of Home Assistant then do this:
-        - Activate your python virtual env
-        - Update package with ``pip``
-          ```
-          pip install zigpy-deconz==0.9.0
-        
         # Releases via PyPI
         Tagged versions are also released via PyPI
         
         - https://pypi.org/project/zigpy-deconz/
         - https://pypi.org/project/zigpy-deconz/#history
         - https://pypi.org/project/zigpy-deconz/#files
```

### Comparing `zigpy-deconz-0.9.2/README.md` & `zigpy-deconz-0.9a1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -5,36 +5,14 @@
 
 [zigpy-deconz](https://github.com/zigpy/zigpy-deconz) is a Python 3 implementation for the [Zigpy](https://github.com/zigpy/) project to implement [deCONZ](https://www.dresden-elektronik.de/funktechnik/products/software/pc/deconz/) based [Zigbee](https://www.zigbee.org) radio devices.
 
 The goal of this project to add native support for the Dresden-Elektronik deCONZ based ZigBee modules in Home Assistant via [Zigpy](https://github.com/zigpy/).
 
 This library uses the deCONZ serial protocol for communicating with [ConBee](https://www.dresden-elektronik.de/conbee/), [ConBee II (ConBee 2)](https://shop.dresden-elektronik.de/conbee-2.html), and [RaspBee](https://www.dresden-elektronik.de/raspbee/) adapters from [Dresden-Elektronik](https://github.com/dresden-elektronik/).
 
-# Testing new releases
-
-Testing a new release of the zigpy-deconz library before it is released in Home Assistant.
-
-If you are using Supervised Home Assistant (formerly known as the Hassio/Hass.io distro):
-- Add https://github.com/home-assistant/hassio-addons-development as "add-on" repository
-- Install "Custom deps deployment" addon
-- Update config like: 
-  ```
-  pypi:
-    - zigpy-deconz==0.9.0
-  apk: []
-  ```
-  where 0.5.1 is the new version
-- Start the addon
-
-If you are instead using some custom python installation of Home Assistant then do this:
-- Activate your python virtual env
-- Update package with ``pip``
-  ```
-  pip install zigpy-deconz==0.9.0
-
 # Releases via PyPI
 Tagged versions are also released via PyPI
 
 - https://pypi.org/project/zigpy-deconz/
 - https://pypi.org/project/zigpy-deconz/#history
 - https://pypi.org/project/zigpy-deconz/#files
```

### Comparing `zigpy-deconz-0.9.2/setup.cfg` & `zigpy-deconz-0.9a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-deconz-0.9.2/setup.py` & `zigpy-deconz-0.9a1/setup.py`

 * *Files identical despite different names*

### Comparing `zigpy-deconz-0.9.2/zigpy_deconz/api.py` & `zigpy-deconz-0.9a1/zigpy_deconz/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 import binascii
 import enum
 import logging
 from typing import Any, Callable, Dict, Optional, Tuple
 
 import serial
 from zigpy.config import CONF_DEVICE_PATH
-from zigpy.types import APSStatus
 
 from zigpy_deconz.exception import APIException, CommandError
 import zigpy_deconz.types as t
 import zigpy_deconz.uart
 
 LOGGER = logging.getLogger(__name__)
 
-COMMAND_TIMEOUT = 1
-PROBE_TIMEOUT = 2
+COMMAND_TIMEOUT = 2
+PROBE_TIMEOUT = 3
 MIN_PROTO_VERSION = 0x010B
 
 
 class Status(t.uint8_t, enum.Enum):
     SUCCESS = 0
     FAILURE = 1
     BUSY = 2
@@ -70,26 +69,14 @@
     aps_data_request = 0x12
     aps_data_indication = 0x17
     zigbee_green_power = 0x19
     mac_poll = 0x1C
     simplified_beacon = 0x1F
 
 
-class TXStatus(t.uint8_t, enum.Enum):
-    SUCCESS = 0x00
-
-    @classmethod
-    def _missing_(cls, value):
-        chained = APSStatus(value)
-        status = t.uint8_t.__new__(cls, chained.value)
-        status._name_ = chained.name
-        status._value_ = value
-        return status
-
-
 TX_COMMANDS = {
     Command.aps_data_confirm: (t.uint16_t,),
     Command.aps_data_indication: (t.uint16_t, t.uint8_t),
     Command.aps_data_request: (
         t.uint16_t,
         t.uint8_t,
         t.uint8_t,
@@ -112,15 +99,15 @@
     Command.aps_data_confirm: (
         (
             t.uint16_t,
             DeviceState,
             t.uint8_t,
             t.DeconzAddressEndpoint,
             t.uint8_t,
-            TXStatus,
+            t.uint8_t,
             t.uint8_t,
             t.uint8_t,
             t.uint8_t,
             t.uint8_t,
         ),
         True,
     ),
@@ -200,15 +187,14 @@
 
 
 class Deconz:
     def __init__(self, app: Callable, device_config: Dict[str, Any]):
         self._app = app
         self._aps_data_ind_flags: int = 0x01
         self._awaiting = {}
-        self._command_lock = asyncio.Lock()
         self._config = device_config
         self._conn_lost_task: Optional[asyncio.Task] = None
         self._data_indication: bool = False
         self._data_confirm: bool = False
         self._device_state = DeviceState(NetworkState.OFFLINE)
         self._seq = 1
         self._proto_ver: Optional[int] = None
@@ -272,31 +258,28 @@
 
     def close(self):
         if self._uart:
             self._uart.close()
             self._uart = None
 
     async def _command(self, cmd, *args):
+        LOGGER.debug("Command %s %s", cmd, args)
         if self._uart is None:
             # connection was lost
             raise CommandError(Status.ERROR, "API is not running")
-        async with self._command_lock:
-            LOGGER.debug("Command %s %s", cmd, args)
-            data, seq = self._api_frame(cmd, *args)
-            self._uart.send(data)
-            fut = asyncio.Future()
-            self._awaiting[seq] = fut
-            try:
-                return await asyncio.wait_for(fut, timeout=COMMAND_TIMEOUT)
-            except asyncio.TimeoutError:
-                LOGGER.warning(
-                    "No response to '%s' command with seq id '0x%02x'", cmd, seq
-                )
-                self._awaiting.pop(seq)
-                raise
+        data, seq = self._api_frame(cmd, *args)
+        self._uart.send(data)
+        fut = asyncio.Future()
+        self._awaiting[seq] = fut
+        try:
+            return await asyncio.wait_for(fut, timeout=COMMAND_TIMEOUT)
+        except asyncio.TimeoutError:
+            LOGGER.warning("No response to '%s' command", cmd)
+            self._awaiting.pop(seq)
+            raise
 
     def _api_frame(self, cmd, *args):
         schema = TX_COMMANDS[cmd]
         d = t.serialize(args, schema)
         data = t.uint8_t(cmd).serialize()
         self._seq = (self._seq % 255) + 1
         data += t.uint8_t(self._seq).serialize()
```

### Comparing `zigpy-deconz-0.9.2/zigpy_deconz/types.py` & `zigpy-deconz-0.9a1/zigpy_deconz/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-deconz-0.9.2/zigpy_deconz/uart.py` & `zigpy-deconz-0.9a1/zigpy_deconz/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-deconz-0.9.2/zigpy_deconz/zigbee/application.py` & `zigpy-deconz-0.9a1/zigpy_deconz/zigbee/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import asyncio
 import binascii
 import logging
-import re
 from typing import Any, Dict
 
 import zigpy.application
 import zigpy.config
 import zigpy.device
 import zigpy.endpoint
 import zigpy.exceptions
 import zigpy.types
 import zigpy.util
 
 from zigpy_deconz import types as t
 from zigpy_deconz.api import Deconz, NetworkParameter, NetworkState, Status
-from zigpy_deconz.config import CONF_WATCHDOG_TTL, CONFIG_SCHEMA, SCHEMA_DEVICE
+from zigpy_deconz.config import CONF_WATCHDOG_TTL, CONFIG_SCHEMA
 import zigpy_deconz.exception
 
 LOGGER = logging.getLogger(__name__)
 
 CHANGE_NETWORK_WAIT = 1
 SEND_CONFIRM_TIMEOUT = 60
 PROTO_VER_WATCHDOG = 0x0108
 WATCHDOG_TTL = 600
 
 
 class ControllerApplication(zigpy.application.ControllerApplication):
     SCHEMA = CONFIG_SCHEMA
-    SCHEMA_DEVICE = SCHEMA_DEVICE
-
-    probe = Deconz.probe
 
     def __init__(self, config: Dict[str, Any]):
         super().__init__(config=zigpy.config.ZIGPY_SCHEMA(config))
         self._api = None
         self._pending = zigpy.util.Requests()
         self._nwk = 0
         self.version = 0
@@ -73,21 +69,15 @@
         self._api[NetworkParameter.aps_designed_coordinator] = 1
 
         if self._api.protocol_version >= PROTO_VER_WATCHDOG:
             asyncio.ensure_future(self._reset_watchdog())
 
         if auto_form:
             await self.form_network()
-        self.devices[self.ieee] = await DeconzDevice.new(
-            self,
-            self.ieee,
-            self.nwk,
-            self.version,
-            self._config[zigpy.config.CONF_DEVICE][zigpy.config.CONF_DEVICE_PATH],
-        )
+        self.devices[self.ieee] = await ConBeeDevice.new(self, self.ieee, self.nwk)
 
     async def force_remove(self, dev):
         """Forcibly remove device from NCP."""
         pass
 
     async def form_network(self, channel=15, pan_id=None, extended_pan_id=None):
         LOGGER.info("Forming network")
@@ -147,15 +137,15 @@
                     req_id, dst_addr_ep, profile, cluster, min(1, src_ep), data
                 )
             except zigpy_deconz.exception.CommandError as ex:
                 return ex.status, "Couldn't enqueue send data request: {}".format(ex)
 
             r = await asyncio.wait_for(req.result, SEND_CONFIRM_TIMEOUT)
             if r:
-                LOGGER.debug("Error while sending %s req id frame: %s", req_id, r)
+                LOGGER.warning("Error while sending %s req id frame: 0x%02x", req_id, r)
                 return r, "message send failure"
 
         return Status.SUCCESS, "message send success"
 
     @zigpy.util.retryable_request
     async def request(
         self,
@@ -192,15 +182,15 @@
                 )
             except zigpy_deconz.exception.CommandError as ex:
                 return ex.status, "Couldn't enqueue send data request: {}".format(ex)
 
             r = await asyncio.wait_for(req.result, SEND_CONFIRM_TIMEOUT)
 
             if r:
-                LOGGER.debug("Error while sending %s req id frame: %s", req_id, r)
+                LOGGER.warning("Error while sending %s req id frame: 0x%02x", req_id, r)
                 return r, "message send failure"
 
             return r, "message send success"
 
     async def broadcast(
         self,
         profile,
@@ -234,15 +224,17 @@
                     ex.status,
                     "Couldn't enqueue send data request for broadcast: {}".format(ex),
                 )
 
             r = await asyncio.wait_for(req.result, SEND_CONFIRM_TIMEOUT)
 
             if r:
-                LOGGER.debug("Error while sending %s req id broadcast: %s", req_id, r)
+                LOGGER.warning(
+                    "Error while sending %s req id broadcast: 0x%02x", req_id, r
+                )
                 return r, "broadcast send failure"
             return r, "broadcast send success"
 
     async def permit_ncp(self, time_s=60):
         assert 0 <= time_s <= 254
         await self._api.write_parameter(NetworkParameter.permit_join, time_s)
 
@@ -275,35 +267,30 @@
         device.radio_details(lqi, rssi)
         self.handle_message(device, profile_id, cluster_id, src_ep, dst_ep, data)
 
     def handle_tx_confirm(self, req_id, status):
         try:
             self._pending[req_id].result.set_result(status)
             return
-        except KeyError:
+        except KeyError as exc:
             LOGGER.warning(
-                "Unexpected transmit confirm for request id %s, Status: %s",
+                "Unexpected transmit confirm for request id %s, Status: 0x%02x, %s",
                 req_id,
                 status,
+                exc,
             )
         except asyncio.InvalidStateError as exc:
             LOGGER.debug(
                 "Invalid state on future - probably duplicate response: %s", exc
             )
 
 
-class DeconzDevice(zigpy.device.Device):
+class ConBeeDevice(zigpy.device.Device):
     """Zigpy Device representing Coordinator."""
 
-    def __init__(self, version: int, device_path: str, *args):
-        super().__init__(*args)
-        is_gpio_device = re.match(r"/dev/tty(S|AMA)\d+", device_path)
-        self._model = "RaspBee" if is_gpio_device else "ConBee"
-        self._model += " II" if ((version & 0x0000FF00) == 0x00000700) else ""
-
     async def add_to_group(self, grp_id: int, name: str = None) -> None:
         group = self.application.groups.add_group(grp_id, name)
 
         for epid in self.endpoints:
             if not epid:
                 continue  # skip ZDO
             group.add_member(self.endpoints[epid])
@@ -318,20 +305,20 @@
 
     @property
     def manufacturer(self):
         return "dresden elektronik"
 
     @property
     def model(self):
-        return self._model
+        return "ConBee"
 
     @classmethod
-    async def new(cls, application, ieee, nwk, version: int, device_path: str):
+    async def new(cls, application, ieee, nwk):
         """Create or replace zigpy device."""
-        dev = cls(version, device_path, application, ieee, nwk)
+        dev = cls(application, ieee, nwk)
 
         if ieee in application.devices:
             from_dev = application.get_device(ieee=ieee)
             dev.status = from_dev.status
             dev.node_desc = from_dev.node_desc
             for ep_id, from_ep in from_dev.endpoints.items():
                 if not ep_id:
```

### Comparing `zigpy-deconz-0.9.2/zigpy_deconz.egg-info/PKG-INFO` & `zigpy-deconz-0.9a1/zigpy_deconz.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy-deconz
-Version: 0.9.2
+Version: 0.9a1
 Summary: A library which communicates with Deconz radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-deconz
 Author: Daniel Schmidt
 Author-email: schmidt.d@aon.at
 License: GPL-3.0
 Description: # zigpy-deconz
         
@@ -13,36 +13,14 @@
         
         [zigpy-deconz](https://github.com/zigpy/zigpy-deconz) is a Python 3 implementation for the [Zigpy](https://github.com/zigpy/) project to implement [deCONZ](https://www.dresden-elektronik.de/funktechnik/products/software/pc/deconz/) based [Zigbee](https://www.zigbee.org) radio devices.
         
         The goal of this project to add native support for the Dresden-Elektronik deCONZ based ZigBee modules in Home Assistant via [Zigpy](https://github.com/zigpy/).
         
         This library uses the deCONZ serial protocol for communicating with [ConBee](https://www.dresden-elektronik.de/conbee/), [ConBee II (ConBee 2)](https://shop.dresden-elektronik.de/conbee-2.html), and [RaspBee](https://www.dresden-elektronik.de/raspbee/) adapters from [Dresden-Elektronik](https://github.com/dresden-elektronik/).
         
-        # Testing new releases
-        
-        Testing a new release of the zigpy-deconz library before it is released in Home Assistant.
-        
-        If you are using Supervised Home Assistant (formerly known as the Hassio/Hass.io distro):
-        - Add https://github.com/home-assistant/hassio-addons-development as "add-on" repository
-        - Install "Custom deps deployment" addon
-        - Update config like: 
-          ```
-          pypi:
-            - zigpy-deconz==0.9.0
-          apk: []
-          ```
-          where 0.5.1 is the new version
-        - Start the addon
-        
-        If you are instead using some custom python installation of Home Assistant then do this:
-        - Activate your python virtual env
-        - Update package with ``pip``
-          ```
-          pip install zigpy-deconz==0.9.0
-        
         # Releases via PyPI
         Tagged versions are also released via PyPI
         
         - https://pypi.org/project/zigpy-deconz/
         - https://pypi.org/project/zigpy-deconz/#history
         - https://pypi.org/project/zigpy-deconz/#files
```

