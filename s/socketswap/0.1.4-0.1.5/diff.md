# Comparing `tmp/SocketSwap-0.1.4-py2.py3-none-any.whl.zip` & `tmp/socketswap-0.1.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7291 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-24 07:37 SocketSwap/__init__.py
--rw-rw-rw-  2.0 fat      815 b- defN 23-Apr-23 10:17 SocketSwap/context_manager.py
+Zip file size: 7292 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-24 07:39 SocketSwap/__init__.py
+-rw-rw-rw-  2.0 fat      815 b- defN 23-Apr-24 07:39 SocketSwap/context_manager.py
 -rw-rw-rw-  2.0 fat    12600 b- defN 23-Apr-23 12:25 SocketSwap/proxy.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 07:37 SocketSwap-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-24 07:37 SocketSwap-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 07:37 SocketSwap-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-24 07:37 SocketSwap-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      642 b- defN 23-Apr-24 07:37 SocketSwap-0.1.4.dist-info/RECORD
-8 files, 17476 bytes uncompressed, 6173 bytes compressed:  64.7%
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 07:40 socketswap-0.1.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-24 07:40 socketswap-0.1.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 07:40 socketswap-0.1.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-24 07:40 socketswap-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      642 b- defN 23-Apr-24 07:40 socketswap-0.1.5.dist-info/RECORD
+8 files, 17476 bytes uncompressed, 6174 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: SocketSwap/context_manager.py
 Comment: 
 
 Filename: SocketSwap/proxy.py
 Comment: 
 
-Filename: SocketSwap-0.1.4.dist-info/LICENSE
+Filename: socketswap-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: SocketSwap-0.1.4.dist-info/METADATA
+Filename: socketswap-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: SocketSwap-0.1.4.dist-info/WHEEL
+Filename: socketswap-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: SocketSwap-0.1.4.dist-info/top_level.txt
+Filename: socketswap-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: SocketSwap-0.1.4.dist-info/RECORD
+Filename: socketswap-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SocketSwap/__init__.py

```diff
@@ -1,18 +1,18 @@
 """
-SocketSwap
+socketswap
 
-SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
+socketswap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 """
 
 __version__ = "0.1.0"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
-from SocketSwap.context_manager import SocketSwapContext
-from SocketSwap.proxy import start_local_proxy
+from socketswap.context_manager import socketswapContext
+from socketswap.proxy import start_local_proxy
 
 
 __all__ = [
-    SocketSwapContext,
+    socketswapContext,
     start_local_proxy
 ]
```

## SocketSwap/context_manager.py

```diff
@@ -6,15 +6,15 @@
 import time
 import logging
 
 logger = logging.getLogger("socketswap")
 logger.addHandler(logging.NullHandler())
 
 
-class SocketSwapContext:
+class socketswapContext:
     
     def __init__(self, *args):
         self.args = args
     
     def __enter__(self):
         logger.info("Starting Proxy Server")
         self.proxy_process = multiprocessing.Process(target=proxy.start_local_proxy, args=(self.args))
```

## Comparing `SocketSwap-0.1.4.dist-info/LICENSE` & `socketswap-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SocketSwap-0.1.4.dist-info/METADATA` & `socketswap-0.1.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
-Name: SocketSwap
-Version: 0.1.4
-Summary: SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
-Home-page: https://github.com/fyx99/SocketSwap
+Name: socketswap
+Version: 0.1.5
+Summary: socketswap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
+Home-page: https://github.com/fyx99/socketswap
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SocketSwap
+# socketswap
 
-SocketSwap is a tool that allows to proxy any third-party libraries traffic through a TCP SOCKS5 Proxy.
+socketswap is a tool that allows to proxy any third-party libraries traffic through a TCP SOCKS5 Proxy.
 
 Some Python libaries support proxing out of the box like requests.
-For all other libaries especially ones not natively written in python, you can use SocketSwap to redirect traffic via a proxy.
+For all other libaries especially ones not natively written in python, you can use socketswap to redirect traffic via a proxy.
 
 ### Usage:
 
 There are two ways to use SwapSock. 
 
     - Via a Context Manager that starts the proxy in a daemon process
     - Directly as a blocking script
```

## Comparing `SocketSwap-0.1.4.dist-info/RECORD` & `socketswap-0.1.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-SocketSwap/__init__.py,sha256=STukqR19TaUKr-AaHDSwh2TCXy30a-OnlHPCkeuUmcU,385
-SocketSwap/context_manager.py,sha256=Bx7wh0Rwp3ekJlWJwseTMIHDKE0DB9n2rjRtGnY5AD4,815
+SocketSwap/__init__.py,sha256=CBuiop5iZVJbuWQXaQn0LU5W2ucK0L3q-T1Dm4c-QG4,385
+SocketSwap/context_manager.py,sha256=XC5mMHj9-mLXt9Disxn8o4K2LpE0faraZQiTzW27m68,815
 SocketSwap/proxy.py,sha256=Iy3-YtL-qbccNTKCfc7cn8s_RnMumLKK_wCIpWSRFFc,12600
-SocketSwap-0.1.4.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
-SocketSwap-0.1.4.dist-info/METADATA,sha256=auGxx7JQGMdhIMQAAyCsY07Xs2WUsdz3943nc_f8u4E,1857
-SocketSwap-0.1.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-SocketSwap-0.1.4.dist-info/top_level.txt,sha256=sGI9LWTAw3Bu2u37_lcKmZtgzwly_gHlFHYKhZTWVDM,11
-SocketSwap-0.1.4.dist-info/RECORD,,
+socketswap-0.1.5.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
+socketswap-0.1.5.dist-info/METADATA,sha256=a2kUX_sbiA2QC5tbmqoF9_ynjucLGXlYbK24jKiYHw0,1857
+socketswap-0.1.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+socketswap-0.1.5.dist-info/top_level.txt,sha256=MzFuGTZGmQe6YLuCVgk2-41gBGXF0knNQ_Bg3JYBYbo,11
+socketswap-0.1.5.dist-info/RECORD,,
```

