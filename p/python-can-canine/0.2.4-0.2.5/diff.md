# Comparing `tmp/python-can-canine-0.2.4.tar.gz` & `tmp/python-can-canine-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-canine-0.2.4.tar", last modified: Wed Apr  5 20:27:10 2023, max compression
+gzip compressed data, was "python-can-canine-0.2.5.tar", last modified: Mon Apr 24 07:03:41 2023, max compression
```

## Comparing `python-can-canine-0.2.4.tar` & `python-can-canine-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-05 20:27:10.017598 python-can-canine-0.2.4/
--rw-r--r--   0 yanconst   (501) staff       (20)     1135 2023-04-05 20:27:10.017044 python-can-canine-0.2.4/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      862 2023-04-03 19:31:44.000000 python-can-canine-0.2.4/README.md
--rw-r--r--   0 yanconst   (501) staff       (20)     8006 2023-04-05 20:26:45.000000 python-can-canine-0.2.4/canine.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-05 20:27:10.016411 python-can-canine-0.2.4/python_can_canine.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)     1135 2023-04-05 20:27:09.000000 python-can-canine-0.2.4/python_can_canine.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)      276 2023-04-05 20:27:09.000000 python-can-canine-0.2.4/python_can_canine.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-05 20:27:09.000000 python-can-canine-0.2.4/python_can_canine.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       42 2023-04-05 20:27:09.000000 python-can-canine-0.2.4/python_can_canine.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       22 2023-04-05 20:27:09.000000 python-can-canine-0.2.4/python_can_canine.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        7 2023-04-05 20:27:09.000000 python-can-canine-0.2.4/python_can_canine.egg-info/top_level.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-05 20:27:10.017707 python-can-canine-0.2.4/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)      799 2023-04-05 20:17:43.000000 python-can-canine-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:03:41.074638 python-can-canine-0.2.5/
+-rw-rw-rw-   0        0        0     1210 2023-04-24 07:03:41.073660 python-can-canine-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      886 2023-04-03 09:37:43.000000 python-can-canine-0.2.5/README.md
+-rw-rw-rw-   0        0        0     8294 2023-04-24 06:40:18.000000 python-can-canine-0.2.5/canine.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:03:41.071640 python-can-canine-0.2.5/python_can_canine.egg-info/
+-rw-rw-rw-   0        0        0     1210 2023-04-24 07:03:39.000000 python-can-canine-0.2.5/python_can_canine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-24 07:03:40.000000 python-can-canine-0.2.5/python_can_canine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:03:39.000000 python-can-canine-0.2.5/python_can_canine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:03:40.000000 python-can-canine-0.2.5/python_can_canine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-04-24 07:03:40.000000 python-can-canine-0.2.5/python_can_canine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 07:03:40.000000 python-can-canine-0.2.5/python_can_canine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:03:41.074638 python-can-canine-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-04-24 06:40:02.000000 python-can-canine-0.2.5/setup.py
```

### Comparing `python-can-canine-0.2.4/PKG-INFO` & `python-can-canine-0.2.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-Metadata-Version: 2.1
-Name: python-can-canine
-Version: 0.2.4
-Summary: Python-can CANine
-Home-page: https://github.com/yconst/python-can-canine
-Author: Yannis Chatzikonstantinou
-Author-email: info@tinymovr.com
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
-## python-can-canine
-
-
-
-This module is a plugin that lets you use [CANine adapters](https://tinymovr.com/products/can-bus-adapter) with the [CANine firmware](https://github.com/tinymovr/CANine) in python-can.
-
-
-### Installation
-
-Install using pip:
-
-    $ pip install python-can-canine
-
-
-### Usage
-
-Overall, using this plugin is quite similar to the main Python-CAN library, with the interface named `canine`. To integrate the Canine interface into your scripts, you can import constants, device designations, and more from the Python-CAN-Canine module using `import canine`. For most scenarios, incorporating a Canine interface is as easy as modifying Python-CAN examples with the lines provided below:
-
-Create python-can bus with the Canine USB interface:
-
-    import can
-    from canine import CANineBus
-
-    bus = can.Bus(interface="canine", bitrate=1000000)
+## python-can-canine
+
+
+
+This module is a plugin that lets you use [CANine adapters](https://tinymovr.com/products/can-bus-adapter) with the [CANine firmware](https://github.com/tinymovr/CANine) in python-can.
+
+
+### Installation
+
+Install using pip:
+
+    $ pip install python-can-canine
+
+
+### Usage
+
+Overall, using this plugin is quite similar to the main Python-CAN library, with the interface named `canine`. To integrate the Canine interface into your scripts, you can import constants, device designations, and more from the Python-CAN-Canine module using `import canine`. For most scenarios, incorporating a Canine interface is as easy as modifying Python-CAN examples with the lines provided below:
+
+Create python-can bus with the Canine USB interface:
+
+    import can
+    from canine import CANineBus
+
+    bus = can.Bus(interface="canine", bitrate=1000000)
```

### Comparing `python-can-canine-0.2.4/README.md` & `python-can-canine-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,38 @@
-## python-can-canine
-
-
-
-This module is a plugin that lets you use [CANine adapters](https://tinymovr.com/products/can-bus-adapter) with the [CANine firmware](https://github.com/tinymovr/CANine) in python-can.
-
-
-### Installation
-
-Install using pip:
-
-    $ pip install python-can-canine
-
-
-### Usage
-
-Overall, using this plugin is quite similar to the main Python-CAN library, with the interface named `canine`. To integrate the Canine interface into your scripts, you can import constants, device designations, and more from the Python-CAN-Canine module using `import canine`. For most scenarios, incorporating a Canine interface is as easy as modifying Python-CAN examples with the lines provided below:
-
-Create python-can bus with the Canine USB interface:
-
-    import can
-    from canine import CANineBus
-
-    bus = can.Bus(interface="canine", bitrate=1000000)
+Metadata-Version: 2.1
+Name: python-can-canine
+Version: 0.2.5
+Summary: Python-can CANine
+Home-page: https://github.com/yconst/python-can-canine
+Author: Yannis Chatzikonstantinou
+Author-email: info@tinymovr.com
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
+## python-can-canine
+
+
+
+This module is a plugin that lets you use [CANine adapters](https://tinymovr.com/products/can-bus-adapter) with the [CANine firmware](https://github.com/tinymovr/CANine) in python-can.
+
+
+### Installation
+
+Install using pip:
+
+    $ pip install python-can-canine
+
+
+### Usage
+
+Overall, using this plugin is quite similar to the main Python-CAN library, with the interface named `canine`. To integrate the Canine interface into your scripts, you can import constants, device designations, and more from the Python-CAN-Canine module using `import canine`. For most scenarios, incorporating a Canine interface is as easy as modifying Python-CAN examples with the lines provided below:
+
+Create python-can bus with the Canine USB interface:
+
+    import can
+    from canine import CANineBus
+
+    bus = can.Bus(interface="canine", bitrate=1000000)
+
+
```

### Comparing `python-can-canine-0.2.4/canine.py` & `python-can-canine-0.2.5/canine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-"""
-Interface for CANine over USB (win32/macos/linux).
-
-"""
-
-# USB Packet format
-# {remaining packets in sequence}{partial frame data}
-# or
-# 0{command}{CAN frame}
-
-from typing import Any, Optional, Tuple
-
-from can.exceptions import error_check
-
-import struct
-import time
-import logging
-
-from usb import USBError
-import usb.core
-import usb.util
-
-from can import BusABC, Message, typechecking
-
-logger = logging.getLogger(__name__)
-
-
-class CANineBus(BusABC):
-    """
-    CANine bus class
-    CANine is a USB to CAN adapter evolved from canable.
-    https://github.com/tinymovr/CANine
-    """
-
-    # the supported bitrates and their commands
-    _BITRATES = {
-        10000: b"S\x00",
-        20000: b"S\x01",
-        50000: b"S\x02",
-        100000: b"S\x03",
-        125000: b"S\x04",
-        250000: b"S\x05",
-        500000: b"S\x06",
-        750000: b"S\x07",
-        1000000: b"S\x08",
-    }
-
-    def __init__(
-        self,
-        channel: typechecking.ChannelStr,
-        bitrate: Optional[int] = None,
-        usb_dev: Optional[usb.core.Device] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :param channel:
-            Optional channel, corresponds to USB product ID
-        :param bitrate:
-            Bitrate in bit/s
-        :param usb_dev:
-            A pyusb device to use
-        """
-
-        self._buffer = bytearray()
-
-        if usb_dev:
-            dev = usb_dev
-        else:
-            dev = usb.core.find(idProduct=0xC1B0)
-        assert dev is not None, "Could not create CANine device"
-        dev.set_configuration()
-        self.dev = dev
-
-        if bitrate is not None:
-            self.set_bitrate(bitrate)
-
-        self.open()
-
-        super().__init__(channel, bitrate=None, **kwargs)
-
-    def set_bitrate(self, bitrate: int) -> None:
-        """
-        :raise ValueError: if both *bitrate* is not among the possible values
-
-        :param bitrate:
-            Bitrate in bit/s
-        """
-        if bitrate in self._BITRATES:
-            self.close()
-            self._write(self._BITRATES[bitrate])
-            self.open()
-        else:
-            raise ValueError(
-                "Invalid bitrate, choose one of "
-                + (", ".join(str(k) for k in self._BITRATES.keys()))
-                + "."
-            )
-
-    def _write(self, payload: bytes) -> None:
-        """
-        Write to the interface
-
-        :param payload:
-            The payload to write as an array of bytes
-        """
-        # can only send single packet frames for now
-        # TODO: update for CAN-FD
-        payload = b"\x00" + payload
-        self.dev.write(0x1, payload)
-
-    def _read(self, timeout: Optional[float]) -> Any:
-        """
-        Read from the interface
-
-        :param timeout:
-            Optional read timeout in seconds
-        """
-        # TODO: handle multiple packets sequence
-        # NOTE: pyusb specifies timeout in milliseconds.
-        # in case you dont want to spend a full
-        # hour finding this, here it is:
-        # https://github.com/pyusb/pyusb/blob/777dea9d718e70d7323c821d4497c706b35742da/usb/core.py#L1014 .
-        timeout_ms: int = 0
-        if timeout == 0:
-            timeout_ms = 1
-        elif timeout is None:
-            timeout_ms = 1000000
-        elif timeout > 0:
-            timeout_ms = int(timeout * 1000)
-        with error_check("Could not read from USB device"):
-            try:
-                packet = self.dev.read(0x81, 64, timeout_ms)
-                remaining_packets = packet[0]
-                assert remaining_packets == 0  # avoid multi-packet sequence for now
-                payload = packet[1:]
-
-                return payload
-            except USBError as e:
-                # do we really need to check for token in string??
-                if "time" in str(e):
-                    return None
-                raise e
-
-    def flush(self) -> None:
-        """
-        Flush buffer and attempt to read all waiting messages from interface
-        """
-        del self._buffer[:]
-        try:
-            p = self.dev.read()
-            if p:
-                p = self.dev.read()
-        except TimeoutError:
-            pass
-
-    def open(self) -> None:
-        """
-        Write the token to open the interface
-        """
-        self._write(b"O")
-
-    def close(self) -> None:
-        """
-        Write the token to close the interface
-        """
-        self._write(b"C")
-
-    def _recv_internal(
-        self, timeout: Optional[float]
-    ) -> Tuple[Optional[Message], bool]:
-        canId = None
-        remote = False
-        extended = False
-        frame = []
-
-        payload = self._read(timeout)
-
-        if not payload:
-            return None, False
-        elif payload[0] == ord(b"T"):
-            # extended frame
-            canId, dlc = struct.unpack("<LB", payload[1:6])
-            extended = True
-            frame = payload[6 : dlc + 6]
-        elif payload[0] == ord(b"t"):
-            # normal frame
-            canId, dlc = struct.unpack("<HB", payload[1:4])
-            frame = payload[4 : dlc + 4]
-        elif payload[0] == ord(b"r"):
-            # remote frame
-            canId, dlc = struct.unpack("<HB", payload[1:4])
-            remote = True
-        elif payload[0] == ord(b"R"):
-            # remote extended frame
-            canId, dlc = struct.unpack("<LB", payload[1:6])
-            extended = True
-            remote = True
-        else:
-            raise ConnectionError("Unknown frame type identifier")
-
-        msg = Message(
-            arbitration_id=canId,
-            is_extended_id=extended,
-            timestamp=time.time(),  # Better than nothing...
-            is_remote_frame=remote,
-            dlc=dlc,
-            data=frame,
-        )
-        return msg, False
-
-    def send(self, msg: Message, timeout: Optional[float] = None) -> None:
-        if msg.is_remote_frame:
-            if msg.is_extended_id:
-                header = ord("R")
-                encoding = "<BLB"
-            else:
-                header = ord("r")
-                encoding = "<BHB"
-            payload = struct.pack(encoding, header, msg.arbitration_id, msg.dlc)
-        else:
-            if msg.is_extended_id:
-                header = ord("T")
-                encoding = "<BLB"
-            else:
-                header = ord("t")
-                encoding = "<BHB"
-            payload = struct.pack(
-                encoding, header, msg.arbitration_id, msg.dlc
-            ) + bytes(msg.data)
-        self._write(payload)
-
-    def shutdown(self) -> None:
-        """
-        Shutdown by closing the interface and freeing resources
-        """
-        self.close()
-        usb.util.dispose_resources(self.dev)
-
-    def fileno(self) -> int:
-        raise NotImplementedError(
-            "fileno is not implemented using current CAN bus on this platform"
-        )
-
-    def get_version(
-        self, timeout: Optional[float]
-    ) -> Tuple[Optional[int], Optional[int]]:
-        """Get HW and SW version of the adapter.
-
-        :param timeout:
-            seconds to wait for version or None to wait indefinitely
-
-        :returns: tuple (hw_version, sw_version)
-            WHERE
-            int hw_version is the hardware version or None on timeout
-            int sw_version is the software version or None on timeout
-        """
-        cmd = b"V"
-        self._write(cmd)
-
-        payload = self._read(timeout)
-        assert payload[0] == ord(b"V")
-        hw_version, sw_version = struct.unpack("<HH", payload[1:5])
-        return hw_version, sw_version
-
-    @staticmethod
-    def _detect_available_configs():
-        """
-        Identify CANine devices
-        """
-        channels = []
-        try:
-            channels = usb.core.find(idProduct=0xC1B0, find_all=True)
-        except usb.core.NoBackendError:
-            pass
-        return [
-            {
-                "interface": "canine",
-                "channel": usb.util.get_string(channel, channel.iSerialNumber),
-            }
-            for channel in channels
-        ]
+"""
+Interface for CANine over USB (win32/macos/linux).
+
+"""
+
+# USB Packet format
+# {remaining packets in sequence}{partial frame data}
+# or
+# 0{command}{CAN frame}
+
+from typing import Any, Optional, Tuple
+
+from can.exceptions import error_check
+
+import struct
+import time
+import logging
+
+from usb import USBError
+import usb.core
+import usb.util
+
+from can import BusABC, Message, typechecking
+
+logger = logging.getLogger(__name__)
+
+
+class CANineBus(BusABC):
+    """
+    CANine bus class
+    CANine is a USB to CAN adapter evolved from canable.
+    https://github.com/tinymovr/CANine
+    """
+
+    # the supported bitrates and their commands
+    _BITRATES = {
+        10000: b"S\x00",
+        20000: b"S\x01",
+        50000: b"S\x02",
+        100000: b"S\x03",
+        125000: b"S\x04",
+        250000: b"S\x05",
+        500000: b"S\x06",
+        750000: b"S\x07",
+        1000000: b"S\x08",
+    }
+
+    def __init__(
+        self,
+        channel: typechecking.ChannelStr = None,
+        bitrate: Optional[int] = None,
+        usb_dev: Optional[usb.core.Device] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :param channel:
+            Optional channel, corresponds to USB product ID
+        :param bitrate:
+            Bitrate in bit/s
+        :param usb_dev:
+            A pyusb device to use
+        """
+
+        self._buffer = bytearray()
+
+        if usb_dev:
+            dev = usb_dev
+        else:
+            dev = usb.core.find(idProduct=0xC1B0)
+        assert dev is not None, "Could not create CANine device"
+        dev.set_configuration()
+        self.dev = dev
+
+        if bitrate is not None:
+            self.set_bitrate(bitrate)
+
+        self.open()
+
+        super().__init__(channel, bitrate=None, **kwargs)
+
+    def set_bitrate(self, bitrate: int) -> None:
+        """
+        :raise ValueError: if both *bitrate* is not among the possible values
+
+        :param bitrate:
+            Bitrate in bit/s
+        """
+        if bitrate in self._BITRATES:
+            self.close()
+            self._write(self._BITRATES[bitrate])
+            self.open()
+        else:
+            raise ValueError(
+                "Invalid bitrate, choose one of "
+                + (", ".join(str(k) for k in self._BITRATES.keys()))
+                + "."
+            )
+
+    def _write(self, payload: bytes) -> None:
+        """
+        Write to the interface
+
+        :param payload:
+            The payload to write as an array of bytes
+        """
+        # can only send single packet frames for now
+        # TODO: update for CAN-FD
+        payload = b"\x00" + payload
+        self.dev.write(0x1, payload)
+
+    def _read(self, timeout: Optional[float]) -> Any:
+        """
+        Read from the interface
+
+        :param timeout:
+            Optional read timeout in seconds
+        """
+        # TODO: handle multiple packets sequence
+        # NOTE: pyusb specifies timeout in milliseconds.
+        # in case you dont want to spend a full
+        # hour finding this, here it is:
+        # https://github.com/pyusb/pyusb/blob/777dea9d718e70d7323c821d4497c706b35742da/usb/core.py#L1014 .
+        timeout_ms: int = 0
+        if timeout == 0:
+            timeout_ms = 1
+        elif timeout is None:
+            timeout_ms = 1000000
+        elif timeout > 0:
+            timeout_ms = int(timeout * 1000)
+        with error_check("Could not read from USB device"):
+            try:
+                packet = self.dev.read(0x81, 64, timeout_ms)
+                remaining_packets = packet[0]
+                assert remaining_packets == 0  # avoid multi-packet sequence for now
+                payload = packet[1:]
+
+                return payload
+            except USBError as e:
+                # do we really need to check for token in string??
+                if "time" in str(e):
+                    return None
+                raise e
+
+    def flush(self) -> None:
+        """
+        Flush buffer and attempt to read all waiting messages from interface
+        """
+        del self._buffer[:]
+        try:
+            p = self.dev.read()
+            if p:
+                p = self.dev.read()
+        except TimeoutError:
+            pass
+
+    def open(self) -> None:
+        """
+        Write the token to open the interface
+        """
+        self._write(b"O")
+
+    def close(self) -> None:
+        """
+        Write the token to close the interface
+        """
+        self._write(b"C")
+
+    def _recv_internal(
+        self, timeout: Optional[float]
+    ) -> Tuple[Optional[Message], bool]:
+        canId = None
+        remote = False
+        extended = False
+        frame = []
+
+        payload = self._read(timeout)
+
+        if not payload:
+            return None, False
+        elif payload[0] == ord(b"T"):
+            # extended frame
+            canId, dlc = struct.unpack("<LB", payload[1:6])
+            extended = True
+            frame = payload[6 : dlc + 6]
+        elif payload[0] == ord(b"t"):
+            # normal frame
+            canId, dlc = struct.unpack("<HB", payload[1:4])
+            frame = payload[4 : dlc + 4]
+        elif payload[0] == ord(b"r"):
+            # remote frame
+            canId, dlc = struct.unpack("<HB", payload[1:4])
+            remote = True
+        elif payload[0] == ord(b"R"):
+            # remote extended frame
+            canId, dlc = struct.unpack("<LB", payload[1:6])
+            extended = True
+            remote = True
+        else:
+            raise ConnectionError("Unknown frame type identifier")
+
+        msg = Message(
+            arbitration_id=canId,
+            is_extended_id=extended,
+            timestamp=time.time(),  # Better than nothing...
+            is_remote_frame=remote,
+            dlc=dlc,
+            data=frame,
+        )
+        return msg, False
+
+    def send(self, msg: Message, timeout: Optional[float] = None) -> None:
+        if msg.is_remote_frame:
+            if msg.is_extended_id:
+                header = ord("R")
+                encoding = "<BLB"
+            else:
+                header = ord("r")
+                encoding = "<BHB"
+            payload = struct.pack(encoding, header, msg.arbitration_id, msg.dlc)
+        else:
+            if msg.is_extended_id:
+                header = ord("T")
+                encoding = "<BLB"
+            else:
+                header = ord("t")
+                encoding = "<BHB"
+            payload = struct.pack(
+                encoding, header, msg.arbitration_id, msg.dlc
+            ) + bytes(msg.data)
+        self._write(payload)
+
+    def shutdown(self) -> None:
+        """
+        Shutdown by closing the interface and freeing resources
+        """
+        self.close()
+        usb.util.dispose_resources(self.dev)
+
+    def fileno(self) -> int:
+        raise NotImplementedError(
+            "fileno is not implemented using current CAN bus on this platform"
+        )
+
+    def get_version(
+        self, timeout: Optional[float]
+    ) -> Tuple[Optional[int], Optional[int]]:
+        """Get HW and SW version of the adapter.
+
+        :param timeout:
+            seconds to wait for version or None to wait indefinitely
+
+        :returns: tuple (hw_version, sw_version)
+            WHERE
+            int hw_version is the hardware version or None on timeout
+            int sw_version is the software version or None on timeout
+        """
+        cmd = b"V"
+        self._write(cmd)
+
+        payload = self._read(timeout)
+        assert payload[0] == ord(b"V")
+        hw_version, sw_version = struct.unpack("<HH", payload[1:5])
+        return hw_version, sw_version
+
+    @staticmethod
+    def _detect_available_configs():
+        """
+        Identify CANine devices
+        """
+        channels = []
+        try:
+            channels = usb.core.find(idProduct=0xC1B0, find_all=True)
+        except usb.core.NoBackendError:
+            pass
+        return [
+            {
+                "interface": "canine",
+                "channel": usb.util.get_string(channel, channel.iSerialNumber),
+            }
+            for channel in channels
+        ]
```

