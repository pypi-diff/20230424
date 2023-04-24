# Comparing `tmp/SocketSwap-0.1.7-py2.py3-none-any.whl.zip` & `tmp/SocketSwap-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7288 bytes, number of entries: 8
+Zip file size: 7305 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-24 07:46 SocketSwap/__init__.py
--rw-rw-rw-  2.0 fat      815 b- defN 23-Apr-24 07:46 SocketSwap/context_manager.py
--rw-rw-rw-  2.0 fat    12600 b- defN 23-Apr-24 07:46 SocketSwap/proxy.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 07:49 SocketSwap-0.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-24 07:49 SocketSwap-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 07:49 SocketSwap-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-24 07:49 SocketSwap-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      642 b- defN 23-Apr-24 07:49 SocketSwap-0.1.7.dist-info/RECORD
-8 files, 17476 bytes uncompressed, 6170 bytes compressed:  64.7%
+-rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-24 08:20 SocketSwap/context_manager.py
+-rw-rw-rw-  2.0 fat    12640 b- defN 23-Apr-24 08:20 SocketSwap/proxy.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      642 b- defN 23-Apr-24 08:20 SocketSwap-0.1.8.dist-info/RECORD
+8 files, 17550 bytes uncompressed, 6187 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: SocketSwap/context_manager.py
 Comment: 
 
 Filename: SocketSwap/proxy.py
 Comment: 
 
-Filename: SocketSwap-0.1.7.dist-info/LICENSE
+Filename: SocketSwap-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: SocketSwap-0.1.7.dist-info/METADATA
+Filename: SocketSwap-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: SocketSwap-0.1.7.dist-info/WHEEL
+Filename: SocketSwap-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: SocketSwap-0.1.7.dist-info/top_level.txt
+Filename: SocketSwap-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: SocketSwap-0.1.7.dist-info/RECORD
+Filename: SocketSwap-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SocketSwap/context_manager.py

```diff
@@ -3,15 +3,16 @@
 """
 import multiprocessing
 import SocketSwap.proxy as proxy
 import time
 import logging
 
 logger = logging.getLogger("SocketSwap")
-logger.addHandler(logging.NullHandler())
+logger.addHandler(logging.StreamHandler())
+logger.setLevel(logging.DEBUG)
 
 
 class SocketSwapContext:
     
     def __init__(self, *args):
         self.args = args
```

## SocketSwap/proxy.py

```diff
@@ -7,15 +7,16 @@
 import ssl
 import select
 import errno
 import logging
 from typing import Callable, List
 
 logger = logging.getLogger("SocketSwap")
-logger.addHandler(logging.NullHandler())
+logger.addHandler(logging.StreamHandler())
+logger.setLevel(logging.DEBUG)
 
 
 proxy_socket = None
 
 def is_valid_ip4(ip):
     """Check if a string is a valid IPv4 address.
 
@@ -312,17 +313,17 @@
 
 
 if __name__ == '__main__':
     # for testing
     
     
     
-    logger = logging.getLogger("SocketSwap")
-    logger.addHandler(logging.StreamHandler())
-    logger.setLevel(logging.DEBUG)
+    # logger = logging.getLogger("SocketSwap")
+    # logger.addHandler(logging.StreamHandler())
+    # logger.setLevel(logging.DEBUG)
 
     import socket
     
 
     def conn_factory():
         target_host = "localhost"
         target_port = 5432
```

## Comparing `SocketSwap-0.1.7.dist-info/LICENSE` & `SocketSwap-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SocketSwap-0.1.7.dist-info/METADATA` & `SocketSwap-0.1.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SocketSwap
-Version: 0.1.7
+Version: 0.1.8
 Summary: SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 Home-page: https://github.com/fyx99/SocketSwap
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `SocketSwap-0.1.7.dist-info/RECORD` & `SocketSwap-0.1.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 SocketSwap/__init__.py,sha256=STukqR19TaUKr-AaHDSwh2TCXy30a-OnlHPCkeuUmcU,385
-SocketSwap/context_manager.py,sha256=czIJoLrqCLDAtXf32QY8EAmTKIwMhuIrIoBueg66iMQ,815
-SocketSwap/proxy.py,sha256=M2S0Qep9fqKmJILPkUf4o_iYM1g7OKU5WR08gp8kWTY,12600
-SocketSwap-0.1.7.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
-SocketSwap-0.1.7.dist-info/METADATA,sha256=lO2DellSdlUMmvXPGPsMQJg9k9wH93Big9HU0JRyf_Q,1857
-SocketSwap-0.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-SocketSwap-0.1.7.dist-info/top_level.txt,sha256=sGI9LWTAw3Bu2u37_lcKmZtgzwly_gHlFHYKhZTWVDM,11
-SocketSwap-0.1.7.dist-info/RECORD,,
+SocketSwap/context_manager.py,sha256=AQl0Y1qBpPMUmh-Cqa_W5Wiz4XiMHlmC9odxshuBD8E,849
+SocketSwap/proxy.py,sha256=6trydLnK0oPXSle7mWb7lRoC7njaUwn-shynup55rkI,12640
+SocketSwap-0.1.8.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
+SocketSwap-0.1.8.dist-info/METADATA,sha256=FQtWDPoX7NZzfLZmrjD3WWOtx3buT15oZZWDWukNQJk,1857
+SocketSwap-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+SocketSwap-0.1.8.dist-info/top_level.txt,sha256=sGI9LWTAw3Bu2u37_lcKmZtgzwly_gHlFHYKhZTWVDM,11
+SocketSwap-0.1.8.dist-info/RECORD,,
```

