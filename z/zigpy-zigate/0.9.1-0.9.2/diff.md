# Comparing `tmp/zigpy-zigate-0.9.1.tar.gz` & `tmp/zigpy-zigate-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-zigate-0.9.1.tar", last modified: Fri Aug  5 04:47:27 2022, max compression
+gzip compressed data, was "zigpy-zigate-0.9.2.tar", last modified: Fri Aug 19 19:03:52 2022, max compression
```

## Comparing `zigpy-zigate-0.9.1.tar` & `zigpy-zigate-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11746 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11387 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/zigpy_zigate/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18215 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/zigpy_zigate/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/tools/firmware.py
--rw-r--r--   0 runner    (1001) docker     (121)    14440 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/tools/flasher.py
--rw-r--r--   0 runner    (1001) docker     (121)     7984 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/zigpy_zigate/zigbee/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11800 2022-08-05 04:47:25.000000 zigpy-zigate-0.9.1/zigpy_zigate/zigbee/application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:47:27.893193 zigpy-zigate-0.9.1/zigpy_zigate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11746 2022-08-05 04:47:27.000000 zigpy-zigate-0.9.1/zigpy_zigate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-05 04:47:27.000000 zigpy-zigate-0.9.1/zigpy_zigate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 04:47:27.000000 zigpy-zigate-0.9.1/zigpy_zigate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-05 04:47:27.000000 zigpy-zigate-0.9.1/zigpy_zigate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-05 04:47:27.000000 zigpy-zigate-0.9.1/zigpy_zigate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:52.133747 zigpy-zigate-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    11726 2022-08-19 19:03:52.133747 zigpy-zigate-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11387 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-19 19:03:52.133747 zigpy-zigate-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:52.129747 zigpy-zigate-0.9.2/zigpy_zigate/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18215 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:52.129747 zigpy-zigate-0.9.2/zigpy_zigate/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/tools/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14440 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/tools/flasher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7984 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:52.133747 zigpy-zigate-0.9.2/zigpy_zigate/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11976 2022-08-19 19:03:50.000000 zigpy-zigate-0.9.2/zigpy_zigate/zigbee/application.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:03:52.129747 zigpy-zigate-0.9.2/zigpy_zigate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11726 2022-08-19 19:03:52.000000 zigpy-zigate-0.9.2/zigpy_zigate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-19 19:03:52.000000 zigpy-zigate-0.9.2/zigpy_zigate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 19:03:52.000000 zigpy-zigate-0.9.2/zigpy_zigate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-19 19:03:52.000000 zigpy-zigate-0.9.2/zigpy_zigate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-19 19:03:52.000000 zigpy-zigate-0.9.2/zigpy_zigate.egg-info/top_level.txt
```

### Comparing `zigpy-zigate-0.9.1/COPYING` & `zigpy-zigate-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/LICENSE` & `zigpy-zigate-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/PKG-INFO` & `zigpy-zigate-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: zigpy-zigate
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library which communicates with ZiGate radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-zigate
 Author: Sébastien RAMAGE
 Author-email: sebatien.ramage@gmail.com
 License: GPL-3.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
 
 # zigpy-zigate
 
 ![Build & Tests](https://github.com/zigpy/zigpy-zigate/workflows/Build%20&%20Tests/badge.svg?branch=master)
@@ -155,9 +154,7 @@
 [zha-network-card](https://github.com/dmulcahey/zha-network-card) is a custom Lovelace card for Home Assistant that displays ZHA component Zigbee network and device information in Home Assistant
 
 #### Zigzag
 [Zigzag](https://github.com/Samantha-uk/zigzag) is an custom card/panel for [Home Assistant](https://www.home-assistant.io/) that displays a graphical layout of Zigbee devices and the connections between them. Zigzag can be installed as a panel or a custom card and relies on the data provided by the [zha-map](https://github.com/zha-ng/zha-map) integration commponent.
 
 #### ZHA Device Exporter
 [zha-device-exporter](https://github.com/dmulcahey/zha-device-exporter) is a custom component for Home Assistant to allow the ZHA component to export lists of Zigbee devices.
-
-
```

### Comparing `zigpy-zigate-0.9.1/README.md` & `zigpy-zigate-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/setup.py` & `zigpy-zigate-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/api.py` & `zigpy-zigate-0.9.2/zigpy_zigate/api.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/common.py` & `zigpy-zigate-0.9.2/zigpy_zigate/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,32 +77,32 @@
     """ detect zigate din """
     return port.startswith('socket://')
 
 
 def set_pizigate_running_mode():
     LOGGER.info('Put PiZiGate in running mode')
 
-    gpio0 = UnclosableOutputDevice(pin=GPIO_PIN0, initial_state=None)
-    gpio2 = UnclosableOutputDevice(pin=GPIO_PIN2, initial_state=None)
+    gpio0 = UnclosableOutputDevice(pin=GPIO_PIN0, initial_value=None)
+    gpio2 = UnclosableOutputDevice(pin=GPIO_PIN2, initial_value=None)
 
     gpio2.on()
     time.sleep(0.5)
 
     gpio0.off()
     time.sleep(0.5)
 
     gpio0.on()
     time.sleep(0.5)
 
 
 def set_pizigate_flashing_mode():
     LOGGER.info('Put PiZiGate in flashing mode')
 
-    gpio0 = UnclosableOutputDevice(pin=GPIO_PIN0, initial_state=None)
-    gpio2 = UnclosableOutputDevice(pin=GPIO_PIN2, initial_state=None)
+    gpio0 = UnclosableOutputDevice(pin=GPIO_PIN0, initial_value=None)
+    gpio2 = UnclosableOutputDevice(pin=GPIO_PIN2, initial_value=None)
 
     gpio2.off()
     time.sleep(0.5)
 
     gpio0.off()
     time.sleep(0.5)
```

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/tools/cli.py` & `zigpy-zigate-0.9.2/zigpy_zigate/tools/cli.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/tools/firmware.py` & `zigpy-zigate-0.9.2/zigpy_zigate/tools/firmware.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/tools/flasher.py` & `zigpy-zigate-0.9.2/zigpy_zigate/tools/flasher.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/types.py` & `zigpy-zigate-0.9.2/zigpy_zigate/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/uart.py` & `zigpy-zigate-0.9.2/zigpy_zigate/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate/zigbee/application.py` & `zigpy-zigate-0.9.2/zigpy_zigate/zigbee/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,23 @@
         self._api = api
 
         if self.version < '3.21':
             LOGGER.warning('Old ZiGate firmware detected, you should upgrade to 3.21 or newer')
 
     async def disconnect(self):
         # TODO: how do you stop the network? Is it possible?
-        await self._api.reset(wait=False)
 
-        if self._api:
-            self._api.close()
-            self._api = None
+        if self._api is not None:
+            try:
+                await self._api.reset(wait=False)
+            except Exception as e:
+                LOGGER.warning("Failed to reset before disconnect: %s", e)
+            finally:
+                self._api.close()
+                self._api = None
 
     async def start_network(self):
         # TODO: how do you start the network? Is it always automatically started?
         dev = ZiGateDevice(self, self.state.node_info.ieee, self.state.node_info.nwk)
         self.devices[dev.ieee] = dev
         await dev.schedule_initialize()
```

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate.egg-info/PKG-INFO` & `zigpy-zigate-0.9.2/zigpy_zigate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: zigpy-zigate
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library which communicates with ZiGate radios for zigpy
 Home-page: http://github.com/zigpy/zigpy-zigate
 Author: Sébastien RAMAGE
 Author-email: sebatien.ramage@gmail.com
 License: GPL-3.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
 
 # zigpy-zigate
 
 ![Build & Tests](https://github.com/zigpy/zigpy-zigate/workflows/Build%20&%20Tests/badge.svg?branch=master)
@@ -155,9 +154,7 @@
 [zha-network-card](https://github.com/dmulcahey/zha-network-card) is a custom Lovelace card for Home Assistant that displays ZHA component Zigbee network and device information in Home Assistant
 
 #### Zigzag
 [Zigzag](https://github.com/Samantha-uk/zigzag) is an custom card/panel for [Home Assistant](https://www.home-assistant.io/) that displays a graphical layout of Zigbee devices and the connections between them. Zigzag can be installed as a panel or a custom card and relies on the data provided by the [zha-map](https://github.com/zha-ng/zha-map) integration commponent.
 
 #### ZHA Device Exporter
 [zha-device-exporter](https://github.com/dmulcahey/zha-device-exporter) is a custom component for Home Assistant to allow the ZHA component to export lists of Zigbee devices.
-
-
```

### Comparing `zigpy-zigate-0.9.1/zigpy_zigate.egg-info/SOURCES.txt` & `zigpy-zigate-0.9.2/zigpy_zigate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

