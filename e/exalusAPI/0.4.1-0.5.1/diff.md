# Comparing `tmp/exalusAPI-0.4.1.tar.gz` & `tmp/exalusAPI-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exalusAPI-0.4.1.tar", last modified: Thu Mar 16 07:09:26 2023, max compression
+gzip compressed data, was "exalusAPI-0.5.1.tar", last modified: Mon Apr 24 06:42:42 2023, max compression
```

## Comparing `exalusAPI-0.4.1.tar` & `exalusAPI-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 07:09:26.881532 exalusAPI-0.4.1/
--rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.4.1/LICENSE
--rw-rw-rw-   0        0        0    13894 2023-03-16 07:09:26.880494 exalusAPI-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.4.1/README.md
--rw-rw-rw-   0        0        0     1112 2023-03-16 07:06:48.000000 exalusAPI-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-16 07:09:26.881532 exalusAPI-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-16 07:09:26.848335 exalusAPI-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-16 07:09:26.858438 exalusAPI-0.4.1/src/exalusAPI/
--rw-rw-rw-   0        0        0     5211 2023-03-16 07:02:12.000000 exalusAPI-0.4.1/src/exalusAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 07:09:26.875582 exalusAPI-0.4.1/src/exalusAPI.egg-info/
--rw-rw-rw-   0        0        0    13894 2023-03-16 07:09:26.000000 exalusAPI-0.4.1/src/exalusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-03-16 07:09:26.000000 exalusAPI-0.4.1/src/exalusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 07:09:26.000000 exalusAPI-0.4.1/src/exalusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-03-16 07:09:26.000000 exalusAPI-0.4.1/src/exalusAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 07:09:26.000000 exalusAPI-0.4.1/src/exalusAPI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 06:42:42.849476 exalusAPI-0.5.1/
+-rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    13973 2023-04-24 06:42:42.847479 exalusAPI-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:42:42.839755 exalusAPI-0.5.1/exalusAPI.egg-info/
+-rw-rw-rw-   0        0        0    13973 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-24 06:42:42.000000 exalusAPI-0.5.1/exalusAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1045 2023-04-24 06:41:30.000000 exalusAPI-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:42:42.849476 exalusAPI-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-04-24 06:39:37.000000 exalusAPI-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:42:42.843789 exalusAPI-0.5.1/src/
+-rw-rw-rw-   0        0        0     6588 2023-04-24 06:27:01.000000 exalusAPI-0.5.1/src/__init__.py
```

### Comparing `exalusAPI-0.4.1/LICENSE` & `exalusAPI-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exalusAPI-0.4.1/PKG-INFO` & `exalusAPI-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.4.1
+Version: 0.5.1
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
+Home-page: https://github.com/marceljanicki/ExalusAPI
+Author: Marcel Janicki
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `exalusAPI-0.4.1/pyproject.toml` & `exalusAPI-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "exalusAPI"
-version = "0.4.1"
+version = "0.5.1"
 description = "Simple Exalus integration wrapper, created specifically for HomeAssistant integration."
 readme = "README.md"
 authors = [{ name = "Marcel Janicki", email = "majanicki00@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["HomeAssistant", "Exalus"]
-dependencies = ["events",
-    "signalrcore",
-    "requests",
-]
 requires-python = ">=3.10.6"
 [project.urls]
 Homepage = "https://github.com/marceljanicki/exalusAPI"
 [tool.bumpver]
 current_version = "2023.1001-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
```

### Comparing `exalusAPI-0.4.1/src/exalusAPI/__init__.py` & `exalusAPI-0.5.1/src/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import asyncio, logging, uuid, requests
+import asyncio, logging, uuid, requests, time
+import dataclasses
+import json
+import events
 
 from json import dumps, loads
 from dataclasses import dataclass, asdict
 from typing import Any
-from events import Events
 from enum import Enum
 from signalrcore.hub_connection_builder import HubConnectionBuilder
 
 SERVER_BROKER_URL: str = "http://broker.tr7.pl"
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -44,126 +46,117 @@
     ResourceIsNotAvailable = 9
     Error = 10
     NoData = 11
     NotSupportedMethod = 12
     UserNotLoggedIn = 13
 
 
-class ConnectionError(Exception):
-    """Raised when connection error."""
+class DataFrameEvent(asyncio.Event):
+    def __init__(self, dataframe, transaction_id):
+        super().__init__()
+        self.df = dataframe
+        self.tid = transaction_id
 
-    def __init__(self, message: str = "Connection error!") -> None:
-        """Init"""
-        super().__init__(message)
-        self.message = message
 
-
-class Controller:
+class ExalusAPIClient:
     def __init__(self, controller_serial, controller_pin, login, password):
         self.controller_serial: str = controller_serial
-
-        self.controller_pin: int = controller_pin
-
+        self.controller_pin: str = controller_pin
         self.server_uri: str = ""
-
         self.hub_connection: None or HubConnectionBuilder = None
-
-        self._on_receive: Events = Events
-
         self.login: str = login
-
         self.password: str = password
-
-    def start(self) -> None:
-        """Authorize user"""
-
-        self.hub_connection.send(
-            "AuthorizeTo", [self.controller_serial, self.controller_pin]
+        self.is_authorized = False
+        self.last_response = None
+        self.devices_list = None
+
+    async def wait_for_authorization(self):
+        while not self.is_authorized:
+            await asyncio.sleep(0.1)
+
+    def handle_devices_list(self):
+        for i in range(len(self.devices_list)):
+            print(i + 1, self.devices_list[i])
+
+    def data_parser(self, resp, event):
+        obj = json.loads(resp[1])
+        tid = obj["TransactionId"]
+        df = DataFrame(
+            obj["Resource"],
+            obj["Status"],
+            obj["Method"],
+            obj["TransactionId"],
+            obj["Data"],
         )
+        event = DataFrameEvent(df, tid)
+        event.set()
+        print(obj)
+        return obj
+
+    async def process_data(event):
+        try:
+            async with asyncio.wait(10):
+                await event.wait()
+        except asyncio.TimeoutError():
+            print("Timeout!")
+            return
+        df = event.df
+        tid = event.tid
+        event.clear()
 
-    def auth_result(self, auth_result) -> None:
-        """Check if user has been authorized"""
-
+    async def authorize_async(self, auth_result):
         if auth_result:
-            _LOGGER.info("User has been authorized")
-
-            frame = dumps(
-                asdict(
-                    DataFrame(
-                        "/users/user/login",
-                        Status.WrongData.value,
-                        Method.Put.value,
-                        str(uuid.uuid1()),
-                        {"Email": self.login, "Password": self.password},
-                    )
-                )
+            login_frame = DataFrame(
+                "/users/user/login",
+                Status.WrongData.value,
+                Method.Put.value,
+                str(uuid.uuid1()),
+                {"Email": self.login, "Password": self.password},
             )
-
-            _LOGGER.info("Sent frame: %s", frame)
-
-            self.send_frame(frame)
-
+            await self.send_and_wait(login_frame)
         else:
-            _LOGGER.info("Authorization failed!")
-
-    async def send_and_wait_for_response(
-        self, dataframe: DataFrame, ms_timeout: int = 5000
-    ) -> DataFrame:
-        """Send frames and wait for response"""
-
-        result = asyncio.Future()
-
-        def on_response_received(frame: DataFrame):
-            if frame.TransactionId == dataframe.TransactionId:
-                self._on_receive.on_change -= on_response_received
-
-                result.set_result(frame)
-
-        self.send_frame()
-
-        self._on_receive.on_change += on_response_received
+            print("Authorization falied!")
 
-        await asyncio.wait_for(result, timeout=ms_timeout)
-
-        return result.result
+    def authorize(self, auth_result):
+        asyncio.run(self.authorize_async(auth_result))
 
     def data_handler(self, data: list) -> None:
         """Handle incoming data"""
 
-        frame = loads(data[1])
-
-        if frame["Resource"] != "/homemessaging/notify/message/new":
-            _LOGGER.info("Sent by: %s data:\n %s", data[0], {dumps(frame, indent=3)})
-
-    def send_frame(self, data_frame) -> None:
-        """Send frame to controller"""
+        self.last_response = loads(data[1])
 
-        self.hub_connection.send("SendTo", [self.controller_serial, data_frame])
+        if self.last_response["Resource"] != "/homemessaging/notify/message/new":
+            print(
+                "Sent by: %s data:\n %s", data[0], {dumps(self.last_response, indent=3)}
+            )
+            if self.last_response["Resource"] == "/users/user/login":
+                self.is_authorized = True
+                print("User has been authorized!")
+
+            if self.last_response["Resource"] == "/devices/list":
+                self.devices_list = self.last_response["Data"]
+                self.handle_devices_list()
 
     def establish_connection(self) -> None:
         """Main function used for connecting with controller and handle callbacks"""
 
         result = requests.get(
             f"{SERVER_BROKER_URL}/api/connections/broker/whichserver/{self.controller_serial}",
             timeout=5000,
         )
-
-        _LOGGER.info("Entered")
-
+        print(result)
         if result.status_code != 200:
             raise requests.exceptions.ConnectionError
 
         else:
-            _LOGGER.info("Broker address has been acquired!")
+            print("Broker address has been acquired!")
 
             self.server_uri = f"https://{result.text}/broker"
 
-            _LOGGER.info(self.server_uri)
-
-            _LOGGER.info(self.server_uri)
+            print(self.server_uri)
 
             self.hub_connection = (
                 HubConnectionBuilder()
                 .with_url(self.server_uri)
                 .configure_logging(logging.INFO)
                 .with_automatic_reconnect(
                     {
@@ -172,13 +165,50 @@
                         "reconnect_interval": 5,
                         "max_attempts": 5,
                     }
                 )
                 .build()
             )
 
-        self.hub_connection.on("SendError", _LOGGER.info)
-        self.hub_connection.on("Registration", _LOGGER.info)
-        self.hub_connection.on("Authorization", self.auth_result)
-        self.hub_connection.on("Data", self.data_handler)
-        self.hub_connection.on_open(self.start)
-        self.hub_connection.start()
+            event = None
+
+            self.hub_connection.on("SendError", print)
+            self.hub_connection.on("Authorization", self.authorize)
+            self.hub_connection.on("Registration", print)
+            self.hub_connection.on("Data", lambda data: self.data_parser(data, event))
+            self.hub_connection.on_open(self.start)
+            self.hub_connection.start()
+
+    async def send_and_wait(self, sent_frame: DataFrame, ms_timeout=5000):
+        """"""
+        ack_event = asyncio.Event()
+
+        event = None
+
+        print("Sent frame", sent_frame)
+
+        def ack_received(response):
+            recieved_frame = self.data_parser(response, event)
+            print(recieved_frame["TransactionId"], sent_frame.TransactionId)
+            if recieved_frame["TransactionId"] == sent_frame.TransactionId:
+                ack_event.set()
+
+        self.hub_connection.on("Data", ack_received)
+        self.hub_connection.send(
+            "SendTo", [self.controller_serial, dataclasses.asdict(sent_frame)]
+        )
+
+        try:
+            await asyncio.wait_for(ack_event.wait(), timeout=ms_timeout / 1000)
+
+        except asyncio.TimeoutError:
+            print("Timeout error!")
+
+    def start(self):
+        self.hub_connection.send(
+            "AuthorizeTo", [self.controller_serial, self.controller_pin]
+        )
+
+    def send_frame(self, data_frame: DataFrame) -> None:
+        """Send frame to controller"""
+
+        self.hub_connection.send("SendTo", [self.controller_serial, data_frame])
```

### Comparing `exalusAPI-0.4.1/src/exalusAPI.egg-info/PKG-INFO` & `exalusAPI-0.5.1/exalusAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.4.1
+Version: 0.5.1
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
+Home-page: https://github.com/marceljanicki/ExalusAPI
+Author: Marcel Janicki
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

