# Comparing `tmp/sapcloudconnectorpythonsocket-0.1.2-py2.py3-none-any.whl.zip` & `tmp/sapcloudconnectorpythonsocket-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7033 bytes, number of entries: 9
+Zip file size: 7288 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 14:00 sap-cloud-connector-python-socket/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-12 14:01 sap-cloud-connector-python-socket/sap-cloud-connector-python-socket.py
--rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket/__init__.py
--rw-rw-rw-  2.0 fat     9419 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2402 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      936 b- defN 23-Apr-12 17:23 sapcloudconnectorpythonsocket-0.1.2.dist-info/RECORD
-9 files, 14297 bytes uncompressed, 5353 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-24 12:22 sapcloudconnectorpythonsocket/__init__.py
+-rw-rw-rw-  2.0 fat    10358 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2401 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      937 b- defN 23-Apr-24 12:23 sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD
+9 files, 15230 bytes uncompressed, 5608 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: sapcloudconnectorpythonsocket/__init__.py
 Comment: 
 
 Filename: sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.2.dist-info/LICENSE
+Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.2.dist-info/METADATA
+Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.2.dist-info/WHEEL
+Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.2.dist-info/top_level.txt
+Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sapcloudconnectorpythonsocket-0.1.2.dist-info/RECORD
+Filename: sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sapcloudconnectorpythonsocket/__init__.py

```diff
@@ -1,14 +1,14 @@
 """
 sap-cloud-connector-python-socket
 
 Python Socket to connect to the SAP Cloud Connector via Connectivity Service
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
 from sapcloudconnectorpythonsocket.sapcloudconnectorpythonsocket import CloudConnectorSocket
 
 __all__ = [
     CloudConnectorSocket
```

## sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py

```diff
@@ -1,35 +1,37 @@
-"""main module"""
+"""
+CloudConnectorSocket instance of Pythons socket class overriding the connect function to open a socket via SAP Cloud Connector.
+"""
 import functools
 import socket
 import struct
 import base64
 import logging
 
 logger = logging.getLogger('sapcloudconnectorpythonsocket')
 logger.addHandler(logging.NullHandler())
 
 
-
-
-def format_status_byte(byte):
-    codes = {
+def format_status_byte(status_byte) -> str:
+    """helper function to log the CC specific error bytes"""
+    status_byte_messages = {
         b"\x00": "SUCCESS: Success",
         b"\x01": "FAILURE: Connection closed by backend or general scenario failure.",
         b"\x02": "FORBIDDEN: Connection not allowed by ruleset. No matching host mapping found in Cloud Connector access control settings, see Configure Access Control (TCP).",
         b"\x03": "NETWORK_UNREACHABLE: The Cloud Connector is not connected to the subaccount and the Cloud Connector Location ID that is used by the cloud application can't be identified. See Connect and Disconnect a Cloud Subaccount and Managing Subaccounts, section Procedure.",
         b"\x04": "HOST_UNREACHABLE: Cannot open connection to the backend, that is, the host is unreachable.",
         b"\x05": "CONNECTION_REFUSED: Authentication failure",
         b"\x06": "TTL_EXPIRED: Not used",
         b"\x07": "COMMAND_UNSUPPORTED: Only the SOCKS5 CONNECT command is supported.",
         b"\x08": "ADDRESS_UNSUPPORTED: Only the SOCKS5 DOMAIN and IPv4 commands are supported."
     }
-    return codes[byte] if byte in codes else "Other Unexpected Error byte"
+    return status_byte_messages[status_byte] if status_byte in status_byte_messages else "Other Unexpected Error byte"
 
 def set_self_blocking(function):
+    """helper to use blocking on socket object"""
     @functools.wraps(function)
     def wrapper(*args, **kwargs):
         self = args[0]
         try:
             _is_blocking = self.gettimeout()
             if _is_blocking == 0:
                 self.setblocking(True)
@@ -38,47 +40,56 @@
             raise e
         finally:
             if _is_blocking == 0:
                 self.setblocking(False)
     return wrapper
 
 
-# Cloud Connector socket based on SOCKS 5
+
 class CloudConnectorSocket(socket.socket):
+    """Cloud Connector socket based on SOCKS5 standard"""
 
     def __init__(self, family=socket.AF_INET, type=socket.SOCK_STREAM, proto=0, *args, **kwargs):
-        # some default params for the socket class
+        """set default params for TCP socket"""
         super(CloudConnectorSocket, self).__init__(family, type, proto, *args, **kwargs)
     
     timeout = 30 # default
 
     @set_self_blocking
-    def connect(self, dest_host, dest_port, proxy_host, proxy_port, token, location_id=None, catch_errors=None):
-
+    def connect(self, dest_host: str, dest_port: int, proxy_host: str, proxy_port: int, token: str, location_id: str=None):
+        """
+        Connect to the destination host via the proxy host
+
+        :param dest_host: The host of the destination
+        :param dest_port: The (int) port of the destination
+        :param proxy_host: The host of the proxy
+        :param proxy_port: The port of the proxy
+        :param token: The token from the connectivity-service instance
+        :param location_id: (Optional) specify the Cloud Connector location_id to connect to (if set in cloud connector config else leave empty)
+        """
         super(CloudConnectorSocket, self).settimeout(self.timeout)
         
         try:
             # Initial connection to proxy server
             super(CloudConnectorSocket, self).connect((proxy_host, proxy_port))
-           
         except Exception as e:
             self.close()
             raise Exception(f"EXCEPTION AT INITIAL CONNECT: {e}")
             
         
-        # Connected to proxy server, now negotiate
         try:                
+            # Connected to proxy server, now negotiate authentication
             self.negotiate_auth(dest_host, dest_port, token, location_id)
         except Exception as e:
             self.close()
             raise Exception(f"EXCEPTION NEGOTIATIONG {e}")
 
                 
     def negotiate_auth(self, dest_host, dest_port, token, location_id):
-        
+        """SAP Cloud Connector specific authentication scheme"""
         self.settimeout(None)   # apparently needed for make file to set to blocking https://stackoverflow.com/questions/3432102/python-socket-connection-timeout
         writer = self.makefile("wb")
         reader = self.makefile("rb", 0)  # buffering=0 renamed in Python 3
         try:
             # 5 is for command, 1 for length of auth list, 80 is custom auth type of cc
             writer.write(b"\x05\x01\x80")
             writer.flush()
@@ -88,34 +99,35 @@
 
             if chosen_auth[0:1] != b"\x05":
                 raise Exception("SOCKS5 PROXY SERVER SENT UNEXPECTED DATA FOR CHOSE AUTH")
 
             # Check if 80 method is confirmed
 
             if chosen_auth[1:2] == b"\x80":
-                encoded_location_id = base64.b64encode(location_id.encode())
-                location_id_part = (len(encoded_location_id).to_bytes(1, byteorder="big") + encoded_location_id) if location_id else b"\x00"
+                location_id_part = b"\x00"
+                if location_id:
+                    encoded_location_id = base64.b64encode(location_id.encode())
+                    location_id_part = len(encoded_location_id).to_bytes(1, byteorder="big") + encoded_location_id
                 auth_message = b"\x01" + len(token.encode()).to_bytes(4, byteorder="big") + token.encode() + location_id_part
                 logger.info(auth_message)
                 writer.write(auth_message)
                 writer.flush()
 
                 auth_status = self.readAll(reader, 2)
                 logger.info(f"Auth Status: {auth_status[0:1]} Success: {auth_status[1:2]}")
            
                 
                 if auth_status[0:1] != b"\x01":
-                    raise Exception("SOCKS5 PROXY SERVER SENT UNEXPECTED DATA FOR AUTH")
+                    raise Exception("CLOUD CONNECTOR SENT UNEXPECTED DATA FOR AUTH")
                 if auth_status[1:2] != b"\x00":
                     # Authentication failed
                     raise Exception("SOCKS5 AUTH FAILED " + format_status_byte(auth_status[1:2]))
             
             else:
-                raise Exception("SOCKS5 PROXY SERVER SENT UNEXPECTED CHOSEN AUTH TYPE NOT x80")    
-                
+                raise Exception("CLOUD CONNECTOR SENT UNEXPECTED CHOSEN AUTH TYPE NOT x80")    
                 
             # authentication succeeded and can request actual connection
             # x05 start of message x01 command x00 standard end of command
 
             writer.write(b"\x05\x01\x00")
             resolved = self.writeSOCKS5address(dest_host, dest_port, writer)
             logger.info("flush")
```

## Comparing `sapcloudconnectorpythonsocket-0.1.2.dist-info/LICENSE` & `sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Felix
+Copyright (c) 2023
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `sapcloudconnectorpythonsocket-0.1.2.dist-info/METADATA` & `sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapcloudconnectorpythonsocket
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Package to open socket to SAP Cloud Connector via Connectivity Proxy
 Home-page: https://github.com/fyx99/sap-cloud-connector-python-socket
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,35 +13,35 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sap-cloud-connector-python-socket
+# sapcloudconnectorpythonsocket
 Python Socket to connect to the SAP Cloud Connector via Connectivity Service
 
 The SAP BTP Connectivity Proxy allows to connect to on-prem systems. It can act as a SOCKS5 Proxy to establish TCP connections. 
 Due to its custom authentication scheme one can not use standard SOCKS5 client libaries. For details on how to authenticate against the Connectivity Proxy see the official Documentation. https://help.sap.com/docs/connectivity/sap-btp-connectivity-cf/using-tcp-protocol-for-cloud-applications
 
-Sample Usage:
+##Sample Usage:
 ```python 
 from sapcloudconnectorpythonsocket import CloudConnectorSocket
 
 cc_socket = CloudConnectorSocket()
 cc_socket.connect(
     dest_host="virtualhost", 
     dest_port=3333, 
     proxy_host="connectivity-proxy", 
     proxy_port=20003, 
     token="<token>",
     location_id="CLOUD_CONNECTOR_LOCATION_ID"
 )
 ```
-Opens a socket in python using the SAP Cloud Connector as proxy. The standard socket object from python can be used in a various applications. Often times useful in connectig to TCP based protocols using python packages. The LocationId is optional.
+Opens a socket in python using the SAP Cloud Connector as proxy. The standard socket object from python can be used in a various applications. Often times useful in connectig to TCP based protocols using python packages. The location_id is optional.
 The destination host and port are the virtualhost and virtualport configured in the Cloud Connector configuration.
 The proxy_host and the proxy_port are the host and port of the BTP Cloud Foundry Connectivity Proxy. The token is the authentication token to the Connectivity Proxy. They can be obtained from the Credentials of an BTP Connectivity Service instance.
 
 To open a TCP based connection the proxy_port needs to be the port to the socks5 proxy. This is usually 20004 in the connectivity service.
```

## Comparing `sapcloudconnectorpythonsocket-0.1.2.dist-info/RECORD` & `sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sap-cloud-connector-python-socket/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sap-cloud-connector-python-socket/sap-cloud-connector-python-socket.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sapcloudconnectorpythonsocket/__init__.py,sha256=6tftekR7BlLQte8jPD3X5j26FBzYenxb3hXta1Fd4bY,338
-sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py,sha256=qR5_O8S3ho8Kqe_dMdaNvMBgMjZlZDRAZLOqUYIaIrg,9419
-sapcloudconnectorpythonsocket-0.1.2.dist-info/LICENSE,sha256=oXTItccfzyUudck6ObY-GItzzZwngLzQ403XSpITg0U,1062
-sapcloudconnectorpythonsocket-0.1.2.dist-info/METADATA,sha256=WCnz6e5tuoPVBtMj50CaIn4ghkdYsohMk3WL4QB5qLI,2402
-sapcloudconnectorpythonsocket-0.1.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-sapcloudconnectorpythonsocket-0.1.2.dist-info/top_level.txt,sha256=Sr63qbSm-90o-CQ-qwd4EKcLFznczAzm416CC87q0pA,30
-sapcloudconnectorpythonsocket-0.1.2.dist-info/RECORD,,
+sapcloudconnectorpythonsocket/__init__.py,sha256=RA6VspWt6kfqEeTOlBITEEg6i2y4mxQVmUHNNOxj9H0,338
+sapcloudconnectorpythonsocket/sapcloudconnectorpythonsocket.py,sha256=80MrhtLdNfPb6HYwEYCS9f2YZCKbOXloRiXlg33YMxg,10358
+sapcloudconnectorpythonsocket-0.1.3.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
+sapcloudconnectorpythonsocket-0.1.3.dist-info/METADATA,sha256=U7RXSZENOwKjULSArDJvwWevPo4fd82NcMURNXXZ6oI,2401
+sapcloudconnectorpythonsocket-0.1.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+sapcloudconnectorpythonsocket-0.1.3.dist-info/top_level.txt,sha256=Sr63qbSm-90o-CQ-qwd4EKcLFznczAzm416CC87q0pA,30
+sapcloudconnectorpythonsocket-0.1.3.dist-info/RECORD,,
```

