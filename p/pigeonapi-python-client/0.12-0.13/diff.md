# Comparing `tmp/pigeonapi-python-client-0.12.tar.gz` & `tmp/pigeonapi-python-client-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pigeonapi-python-client-0.12.tar", last modified: Wed Apr 19 21:43:46 2023, max compression
+gzip compressed data, was "dist/pigeonapi-python-client-0.13.tar", last modified: Mon Apr 24 15:03:41 2023, max compression
```

## Comparing `pigeonapi-python-client-0.12.tar` & `pigeonapi-python-client-0.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-04-18 19:31:49.000000 pigeonapi-python-client-0.12/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1910 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1236 2023-04-19 21:40:32.000000 pigeonapi-python-client-0.12/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeon/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1174 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/config.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/exceptions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeon/rest/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/rest/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1291 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/rest/authenticator.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2982 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/rest/historical_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5733 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/rest/intraday_candles.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeon/websocket/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/websocket/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6371 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/websocket/websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/pigeon/websocket/websocket_default_functions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1910 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      571 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        7 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.12/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-04-19 21:43:46.000000 pigeonapi-python-client-0.12/setup.cfg
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1205 2023-04-19 21:37:50.000000 pigeonapi-python-client-0.12/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-04-18 19:31:49.000000 pigeonapi-python-client-0.13/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1910 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1236 2023-04-19 21:40:32.000000 pigeonapi-python-client-0.13/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeon/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1174 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/exceptions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeon/rest/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/rest/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1291 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/rest/authenticator.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2982 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/rest/historical_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5733 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/rest/intraday_candles.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeon/websocket/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/websocket/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6644 2023-04-24 15:01:49.000000 pigeonapi-python-client-0.13/pigeon/websocket/websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/pigeon/websocket/websocket_default_functions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1910 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      571 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        7 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-04-18 18:47:07.000000 pigeonapi-python-client-0.13/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-04-24 15:03:41.000000 pigeonapi-python-client-0.13/setup.cfg
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1205 2023-04-24 15:02:02.000000 pigeonapi-python-client-0.13/setup.py
```

### Comparing `pigeonapi-python-client-0.12/PKG-INFO` & `pigeonapi-python-client-0.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonapi-python-client
-Version: 0.12
+Version: 0.13
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/pigeonapi-python-client
 Author: PigeonAPI powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # Pigeon
         
         Pigeon is a Python library to get Brazilian Financial Market Data.
```

### Comparing `pigeonapi-python-client-0.12/README.md` & `pigeonapi-python-client-0.13/README.md`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/pigeon/config.py` & `pigeonapi-python-client-0.13/pigeon/config.py`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/pigeon/exceptions.py` & `pigeonapi-python-client-0.13/pigeon/exceptions.py`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/pigeon/rest/authenticator.py` & `pigeonapi-python-client-0.13/pigeon/rest/authenticator.py`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/pigeon/rest/historical_candles.py` & `pigeonapi-python-client-0.13/pigeon/rest/historical_candles.py`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/pigeon/rest/intraday_candles.py` & `pigeonapi-python-client-0.13/pigeon/rest/intraday_candles.py`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/pigeon/websocket/websocket_client.py` & `pigeonapi-python-client-0.13/pigeon/websocket/websocket_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional, List
 from ..exceptions import WSTypeError, DelayedError, FeedError
 from ..rest import Authenticator
 from ..config import valid_feeds, valid_ws_options, valid_delayed_options, socket_urls
 from .websocket_default_functions import _on_open, _on_message, _on_error, _on_close
 import websocket 
 import json
+import ssl
 import threading
  
 class WebSocketClient:
     """
     This class connects with Pigeon WebSocket, receiving trade and index data, in real time or delayed.
 
     * Main use case:
@@ -49,28 +50,34 @@
         If the feed is 'indices' this field is not used.
         Field is not required. Default: 'trades'.
 
     instruments: list
         List of tickers or indexes to subscribe.
         Field is not required. Default: [].
 
+    ssl: bool
+    Enable or disable ssl configuration.
+    Field is not required. Default: True (enable).
     """
     def __init__(
         self,
         api_key:str,
         feed:Optional[str] = 'stocks',
         target:Optional[str] = 'realtime',
         ws_type:Optional[str] = 'trade',
         instruments:Optional[List[str]] = [],
+        ssl:Optional[bool] = True,
         **kwargs,
     ):
         self.api_key = api_key
         self.token = Authenticator(self.api_key).token
         self.protocol_str = {"Sec-WebSocket-Protocol": self.token}
         self.instruments = instruments
+        self.ssl = ssl
+
         if feed not in valid_feeds:
             raise FeedError(
                 f"Must provide a valid 'feed' parameter. Valid options are: {valid_feeds}"
             )
         if target not in valid_delayed_options:
             raise DelayedError(
                 f"Must provide a valid 'target' parameter. Valid options are: {valid_delayed_options}"
@@ -155,15 +162,16 @@
             on_open=intermediary_on_open,
             on_message=intermediary_on_message,
             on_error=intermediary_on_error,
             on_close=intermediary_on_close, 
             header=self.protocol_str
         )
 
-        wst = threading.Thread(target=self.ws.run_forever)
+        ssl_conf = {} if self.ssl else {"sslopt": {"cert_reqs": ssl.CERT_NONE}}
+        wst = threading.Thread(target=self.ws.run_forever, kwargs=ssl_conf)
         wst.daemon = True
         wst.start()
 
     def __send(self, data):
         """
         Class method to be used internally. Sends data to the Pigeon WebSocket.
         """
```

### Comparing `pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/PKG-INFO` & `pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonapi-python-client
-Version: 0.12
+Version: 0.13
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/pigeonapi-python-client
 Author: PigeonAPI powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # Pigeon
         
         Pigeon is a Python library to get Brazilian Financial Market Data.
```

### Comparing `pigeonapi-python-client-0.12/pigeonapi_python_client.egg-info/SOURCES.txt` & `pigeonapi-python-client-0.13/pigeonapi_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.12/setup.py` & `pigeonapi-python-client-0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(requirementPath) as f:
             install_requires = f.read().splitlines()
 
 description = "Python package containing several classes and data for extracting and manipulating market and trading data."
 
 setup(
     name='pigeonapi-python-client',
-    version='0.12',
+    version='0.13',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="PigeonAPI powered by BTG Pactual Solutions",
     packages=find_packages(),
     url="https://github.com/BTG-Pactual-Solutions/pigeonapi-python-client",
     install_requires=install_requires,
```

