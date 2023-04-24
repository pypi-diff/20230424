# Comparing `tmp/touch_sdk-0.6.4.tar.gz` & `tmp/touch_sdk-0.6.5.tar.gz`

## Comparing `touch_sdk-0.6.4.tar` & `touch_sdk-0.6.5.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/.gitlab-ci.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/.pylintrc
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/version.sh
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/basic.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/custom_data.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/magnetometer.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/osc.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/plotter.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/pressure.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/raycasting.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/examples/sensors.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/basic.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/pressure.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/__init__.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/gatt_scanner.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/utils.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/uuids.py
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/watch.py
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/watch_connector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/vec_pb2.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_input_pb2.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_output_pb2.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/.gitignore
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/LICENSE
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.DS_Store
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.pylintrc
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/version.sh
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/basic.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/basic_threaded.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/custom_data.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/magnetometer.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/osc.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/plotter.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/pressure.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/raycasting.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/examples/sensors.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/basic.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/pressure.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/gatt_scanner.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/utils.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/uuids.py
+-rw-r--r--   0        0        0     9918 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/watch.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/watch_connector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/vec_pb2.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_input_pb2.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_output_pb2.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/.gitignore
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/LICENSE
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 touch_sdk-0.6.5/PKG-INFO
```

### Comparing `touch_sdk-0.6.4/examples/basic.py` & `touch_sdk-0.6.5/examples/magnetometer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from touch_sdk import Watch
 
 class MyWatch(Watch):
 
-    # def on_sensors(self, sensors):
-    #     print(sensors)
+    def on_sensors(self, sensors):
+        print(sensors.magnetic_field, sensors.magnetic_field_calibration)
 
     def on_tap(self):
         print('tap')
 
     def on_touch_down(self, x, y):
         print('touch down', x, y)
```

### Comparing `touch_sdk-0.6.4/examples/plotter.py` & `touch_sdk-0.6.5/examples/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,9 +65,9 @@
 
     _ = FuncAnimation(
         fig, anim, fargs=(watch, ax, lines, gyro_data), interval=1, blit=True,
         cache_frame_data=False
     )
 
     plt.show()
-
+    watch.stop()
     thread.join()
```

### Comparing `touch_sdk-0.6.4/examples/raycasting.py` & `touch_sdk-0.6.5/examples/raycasting.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/examples/sensors.py` & `touch_sdk-0.6.5/examples/sensors.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/src/basic.py` & `touch_sdk-0.6.5/src/basic.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/src/touch_sdk/gatt_scanner.py` & `touch_sdk-0.6.5/src/touch_sdk/gatt_scanner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import asyncio
-
 from bleak import BleakScanner
 
 __doc__ = """Scans for Bluetooth devices with a given GATT service UUID."""
 
 class GattScanner:
     """Scans for Bluetooth devices with service_uuid.
 
@@ -18,25 +16,23 @@
         self.on_scan_result = on_scan_result
         self.service_uuid = service_uuid
         self.name_filter = name_filter
         self.scanner = None
         self._addresses = set()
         self._scanning = False
 
-    async def run(self):
-        """Run the scanner."""
+    async def start(self):
+        """Start the scanner."""
 
         scanner = BleakScanner(
             self._detection_callback, service_uuids=[self.service_uuid]
         )
 
         await self.start_scanning()
         await scanner.start()
-        while True:
-            await asyncio.sleep(0)
 
     async def stop_scanning(self):
         """Stop scanning."""
         self._scanning = False
 
     async def start_scanning(self):
         """Start scanning. This function should not be called before GattScanner.run
```

### Comparing `touch_sdk-0.6.4/src/touch_sdk/utils.py` & `touch_sdk-0.6.5/src/touch_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/src/touch_sdk/watch.py` & `touch_sdk-0.6.5/src/touch_sdk/watch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum
 import asyncio
 from typing import Tuple, Optional
+import asyncio_atexit
 
 from touch_sdk.uuids import PROTOBUF_OUTPUT, PROTOBUF_INPUT
 from touch_sdk.utils import unpack_chained
 from touch_sdk.watch_connector import WatchConnector
 
 # pylint: disable=no-name-in-module
 from touch_sdk.protobuf.watch_output_pb2 import Update, Gesture, TouchEvent
@@ -60,38 +61,54 @@
         devices. Use Watch.start to enter the scanning and connection event loop.
 
         Optional name_filter connects only to watches with that name (case insensitive)"""
         self._connector = WatchConnector(
             self._on_approved_connection, self._on_protobuf, name_filter
         )
 
+        self._client = None
+        self._stop_event = None
+
+        self._event_loop = None
+
         self.custom_data = None
         if hasattr(self.__class__, "custom_data"):
             self.custom_data = self.__class__.custom_data
 
-        self.client = None
         self.hand = Hand.NONE
 
     def start(self):
         """Blocking event loop that starts the Bluetooth scanner
 
         More handy than Watch.run when only this event loop is needed."""
         try:
             asyncio.run(self.run())
         except KeyboardInterrupt:
             pass
 
+    def stop(self):
+        """Stop the watch, disconnecting any connected devices."""
+        self._stop_event.set()
+
     async def run(self):
         """Asynchronous blocking event loop that starts the Bluetooth scanner.
 
         Makes it possible to run multiple async event loops with e.g. asyncio.gather."""
-        await self._connector.run()
+
+        self._event_loop = asyncio.get_running_loop()
+        self._stop_event = asyncio.Event()
+
+        asyncio_atexit.register(self.stop)
+
+        await self._connector.start()
+        await self._stop_event.wait()
+        await self._connector.stop()
 
     async def _on_approved_connection(self, client):
-        self.client = client
+        self._client = client
 
         await self._fetch_info(client)
         await self._subscribe_to_custom_characteristics(client)
 
     async def _fetch_info(self, client):
         data = await client.read_gatt_char(PROTOBUF_OUTPUT)
         update = Update()
@@ -254,30 +271,30 @@
 
     def trigger_haptics(self, intensity: float, duration_ms: int):
         """Trigger vibration haptics on the watch.
 
         intensity: between 0 and 1
         duration_ms: between 0 and 5000"""
         input_update = self._create_haptics_update(intensity, duration_ms)
-        self._write_input_characteristic(input_update.SerializeToString(), self.client)
+        self._write_input_characteristic(input_update.SerializeToString(), self._client)
 
     @staticmethod
     def _create_haptics_update(intensity, length):
         clamped_intensity = min(max(intensity, 0.0), 1.0)
         clamped_length = min(max(int(length), 0), 5000)
         haptic_event = HapticEvent()
         haptic_event.type = HapticEvent.HapticType.ONESHOT
         haptic_event.length = clamped_length
         haptic_event.intensity = clamped_intensity
         input_update = InputUpdate()
         input_update.hapticEvent.CopyFrom(haptic_event)
         return input_update
 
     def _write_input_characteristic(self, data, client):
-        loop = asyncio.get_running_loop()
-        loop.create_task(
-            self._async_write_input_characteristic(PROTOBUF_INPUT, data, client)
-        )
+        if self._event_loop is not None:
+            self._event_loop.create_task(
+                self._async_write_input_characteristic(PROTOBUF_INPUT, data, client)
+            )
 
     async def _async_write_input_characteristic(self, characteristic, data, client):
         if client:
             await client.write_gatt_char(characteristic, data, True)
```

### Comparing `touch_sdk-0.6.4/src/touch_sdk/watch_connector.py` & `touch_sdk-0.6.5/src/touch_sdk/watch_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,48 +45,57 @@
             set()
         )  # Bluetooth addresses to which client info has successfully been sent
         self._tasks = set()
         self._clients = {}
         self._on_approved_connection = on_approved_connection
         self._on_message = on_message
 
-    async def run(self):
+    async def start(self):
         """Asynchronous blocking event loop that starts the Bluetooth scanner and connection loop.
 
         Makes it possible to run multiple async event loops with e.g. asyncio.gather."""
         await self._start_connection_monitor()
-        await self._scanner.run()
+        await self._scanner.start()
+
+    async def stop(self):
+        """Stop the connector, disconnecting any connected devices."""
+        await self._scanner.stop_scanning()
+        disconnect_tasks = [
+            self._disconnect(address, resume=False)
+            for address, client in self._clients.items()
+        ]
+        await asyncio.gather(*disconnect_tasks)
 
     async def _start_connection_monitor(self):
         loop = asyncio.get_running_loop()
         task = loop.create_task(self._monitor_connections())
         self._tasks.add(task)
         task.add_done_callback(self._tasks.discard)
 
     async def _monitor_connections(self):
         while True:
             # Make sure disconnect is called for all clients for which
             # is_connected is False (because of a physical disconnect, for example)
             disconnect_tasks = [
-                self.disconnect(address)
+                self._disconnect(address)
                 for address, client in self._clients.items()
                 if not client.is_connected
             ]
 
             await asyncio.gather(*disconnect_tasks)
             await asyncio.sleep(2)
 
     async def _on_scan_result(self, device, name):
         client = BleakClient(device)
         address = device.address
 
         try:
             await client.connect()
         except asyncio.exceptions.TimeoutError:
-            await self.disconnect(address)
+            await self._disconnect(address)
             return
 
         self._clients[address] = client
 
         await self._send_client_info(client)
 
         try:
@@ -97,28 +106,25 @@
             # [org.bluez.Error.NotConnected] Not Connected
             #
             # Sometimes (~50%) Bleak thinks the client is connected even though
             # BlueZ thinks it's not. We could try to reconnect, but that messes
             # up with _monitor_connections. Easier to just give up and try again
             # through the scanner, even though it adds a delay and a bit of
             # noise to the console.
-            print('Connecting failed, trying again')
-            await self.disconnect(address)
+            print("Connecting failed, trying again")
+            await self._disconnect(address)
 
-    async def disconnect(self, address):
-        """Disconnect the client associated with the argument device if it exists,
-        and clean up.
-        """
+    async def _disconnect(self, address, resume=True):
         if (client := self._clients.pop(address, None)) is not None:
             await client.disconnect()
 
         self._approved_addresses.discard(address)
         self._scanner.forget_address(address)
 
-        if not self._approved_addresses:
+        if not self._approved_addresses and resume:
             await self._scanner.start_scanning()
 
     async def _on_protobuf(self, device, name, _, data):
         message = Update()
         message.ParseFromString(bytes(data))
 
         # Watch sent a disconnect signal. Might be because the user pressed "no"
@@ -139,30 +145,30 @@
         self._approved_addresses.add(device.address)
 
         if (client := self._clients.get(device.address)) is not None:
             print(f"Connection approved by {name}")
             await self._scanner.stop_scanning()
 
             disconnect_tasks = [
-                self.disconnect(address)
+                self._disconnect(address)
                 for address in self._clients
                 if address != device.address
             ]
 
             await asyncio.gather(*disconnect_tasks)
 
             try:
                 await self._on_approved_connection(client)
             except bleak.exc.BleakDBusError as _:
                 # Catches "Unlikely GATT error"
-                await self.disconnect(device.address)
+                await self._disconnect(device.address)
 
     async def _handle_disconnect_signal(self, device, name):
         print(f"Connection declined from {name}")
-        await self.disconnect(device.address)
+        await self._disconnect(device.address)
 
     async def _send_client_info(self, client):
         if client.address in self._informed_addresses:
             return
 
         client_info = ClientInfo()
         client_info.appName = sys.argv[0]
```

### Comparing `touch_sdk-0.6.4/src/touch_sdk/protobuf/vec_pb2.py` & `touch_sdk-0.6.5/src/touch_sdk/protobuf/vec_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_input_pb2.py` & `touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_input_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/src/touch_sdk/protobuf/watch_output_pb2.py` & `touch_sdk-0.6.5/src/touch_sdk/protobuf/watch_output_pb2.py`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/LICENSE` & `touch_sdk-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/README.md` & `touch_sdk-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `touch_sdk-0.6.4/pyproject.toml` & `touch_sdk-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "touch-sdk"
-version = "0.6.4"
+version = "0.6.5"
 description = "Port 6 Touch SDK"
 license = "ISC"
 authors = [
     { name="Port 6", email="developer@port6.io" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `touch_sdk-0.6.4/PKG-INFO` & `touch_sdk-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touch-sdk
-Version: 0.6.4
+Version: 0.6.5
 Summary: Port 6 Touch SDK
 Project-URL: Homepage, https://github.com/port6io/touch-sdk-py#readme
 Project-URL: Bug Tracker, https://github.com/port6io/touch-sdk-py/issues
 Author-email: Port 6 <developer@port6.io>
 License-Expression: ISC
 License-File: LICENSE
 Keywords: bluetooth
```

