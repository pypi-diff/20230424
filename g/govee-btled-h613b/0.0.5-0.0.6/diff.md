# Comparing `tmp/govee_btled_h613b-0.0.5.tar.gz` & `tmp/govee_btled_h613b-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govee_btled_h613b-0.0.5.tar", max compression
+gzip compressed data, was "govee_btled_h613b-0.0.6.tar", max compression
```

## Comparing `govee_btled_h613b-0.0.5.tar` & `govee_btled_h613b-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11355 2022-12-10 11:21:10.080280 govee_btled_h613b-0.0.5/LICENSE
--rw-r--r--   0        0        0      155 2022-12-10 11:31:51.710251 govee_btled_h613b-0.0.5/README.md
--rw-r--r--   0        0        0     2102 2023-03-05 14:36:54.668963 govee_btled_h613b-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      374 2023-03-05 14:37:02.072224 govee_btled_h613b-0.0.5/src/govee_btled_H613B/__init__.py
--rw-r--r--   0        0        0     4857 2023-03-05 14:31:40.952001 govee_btled_h613b-0.0.5/src/govee_btled_H613B/const.py
--rw-r--r--   0        0        0      356 2022-12-06 22:51:40.437600 govee_btled_h613b-0.0.5/src/govee_btled_H613B/exceptions.py
--rw-r--r--   0        0        0    17836 2023-03-05 14:32:45.501379 govee_btled_h613b-0.0.5/src/govee_btled_H613B/govee_btled_H613B.py
--rw-r--r--   0        0        0      229 2023-03-05 14:00:50.992610 govee_btled_h613b-0.0.5/src/govee_btled_H613B/models.py
--rw-r--r--   0        0        0      684 2022-12-11 12:11:33.449185 govee_btled_h613b-0.0.5/src/govee_btled_H613B/utils.py
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 govee_btled_h613b-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11355 2022-12-10 11:21:10.080280 govee_btled_h613b-0.0.6/LICENSE
+-rw-r--r--   0        0        0      155 2022-12-10 11:31:51.710251 govee_btled_h613b-0.0.6/README.md
+-rw-r--r--   0        0        0     2102 2023-04-24 20:32:13.436988 govee_btled_h613b-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      374 2023-04-24 20:32:18.806938 govee_btled_h613b-0.0.6/src/govee_btled_H613B/__init__.py
+-rw-r--r--   0        0        0     4857 2023-03-05 14:31:40.952001 govee_btled_h613b-0.0.6/src/govee_btled_H613B/const.py
+-rw-r--r--   0        0        0      356 2022-12-06 22:51:40.437600 govee_btled_h613b-0.0.6/src/govee_btled_H613B/exceptions.py
+-rw-r--r--   0        0        0    18289 2023-04-24 20:47:18.735142 govee_btled_h613b-0.0.6/src/govee_btled_H613B/govee_btled_H613B.py
+-rw-r--r--   0        0        0      229 2023-03-05 14:00:50.992610 govee_btled_h613b-0.0.6/src/govee_btled_H613B/models.py
+-rw-r--r--   0        0        0      684 2022-12-11 12:11:33.449185 govee_btled_h613b-0.0.6/src/govee_btled_H613B/utils.py
+-rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 govee_btled_h613b-0.0.6/PKG-INFO
```

### Comparing `govee_btled_h613b-0.0.5/LICENSE` & `govee_btled_h613b-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `govee_btled_h613b-0.0.5/pyproject.toml` & `govee_btled_h613b-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "govee-btled-H613B"
-version = "0.0.5"
+version = "0.0.6"
 description = "Control Govee LED BLE device H613B"
 authors = ["gilcu3 <gilcu3@github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/gilcu3/govee-btled-H613B"
 documentation = ""
 classifiers = [
```

### Comparing `govee_btled_h613b-0.0.5/src/govee_btled_H613B/const.py` & `govee_btled_h613b-0.0.6/src/govee_btled_H613B/const.py`

 * *Files identical despite different names*

### Comparing `govee_btled_h613b-0.0.5/src/govee_btled_H613B/govee_btled_H613B.py` & `govee_btled_h613b-0.0.6/src/govee_btled_H613B/govee_btled_H613B.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,43 +38,54 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_ATTEMPTS = 3
 
 
 class GoveeInstance:
-    def __init__(self, device: BLEDevice) -> None:
-        self._ble_device = device
-        self._client = BleakClientWithServiceCache(device)
+    def __init__(self, ble_device: BLEDevice, advertisement_data: AdvertisementData | None = None) -> None:
+        self._ble_device = ble_device
+        self._client = BleakClientWithServiceCache(ble_device)
         self._write_uuid = None
         self._read_uuid = None
+        self._advertisement_data = advertisement_data
 
         
         self._operation_lock = asyncio.Lock()
         self._state = GoveeState()
         self._connect_lock: asyncio.Lock = asyncio.Lock()
         self._disconnect_timer = None
         self._expected_disconnect = False
         self.loop = asyncio.get_running_loop()
         self._callbacks: list[Callable[[GoveeState], None]] = []
     
+
+    def set_ble_device_and_advertisement_data(
+        self, ble_device: BLEDevice, advertisement_data: AdvertisementData
+    ) -> None:
+        """Set the ble device."""
+        self._ble_device = ble_device
+        self._advertisement_data = advertisement_data
+
     @property
     def address(self) -> str:
         """Return the address."""
         return self._ble_device.address
 
     @property
     def name(self) -> str:
         """Get the name of the device."""
         return self._ble_device.name or self._ble_device.address
 
     @property
     def rssi(self) -> int | None:
         """Get the rssi of the device."""
-        return self._ble_device.rssi
+        if self._advertisement_data:
+            return self._advertisement_data.rssi
+        return None
 
     @property
     def state(self) -> GoveeState:
         """Return the state."""
         return self._state
```

### Comparing `govee_btled_h613b-0.0.5/src/govee_btled_H613B/utils.py` & `govee_btled_h613b-0.0.6/src/govee_btled_H613B/utils.py`

 * *Files identical despite different names*

### Comparing `govee_btled_h613b-0.0.5/PKG-INFO` & `govee_btled_h613b-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govee-btled-h613b
-Version: 0.0.5
+Version: 0.0.6
 Summary: Control Govee LED BLE device H613B
 Home-page: https://github.com/gilcu3/govee-btled-H613B
 License: Apache Software License 2.0
 Author: gilcu3
 Author-email: gilcu3@github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

