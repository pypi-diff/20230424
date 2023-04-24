# Comparing `tmp/SocketSwap-0.1.2-py2.py3-none-any.whl.zip` & `tmp/SocketSwap-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5949 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      311 b- defN 23-Apr-21 14:15 SocketSwap/__init__.py
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Apr-20 14:11 SocketSwap/context_manager.py
--rw-rw-rw-  2.0 fat     7907 b- defN 23-Apr-18 19:59 SocketSwap/proxy.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      642 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/RECORD
-8 files, 13042 bytes uncompressed, 4831 bytes compressed:  63.0%
+Zip file size: 7294 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-23 10:17 SocketSwap/__init__.py
+-rw-rw-rw-  2.0 fat      815 b- defN 23-Apr-23 10:17 SocketSwap/context_manager.py
+-rw-rw-rw-  2.0 fat    12600 b- defN 23-Apr-23 12:25 SocketSwap/proxy.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-24 07:29 SocketSwap-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-24 07:29 SocketSwap-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-24 07:29 SocketSwap-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-24 07:29 SocketSwap-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      642 b- defN 23-Apr-24 07:29 SocketSwap-0.1.3.dist-info/RECORD
+8 files, 17476 bytes uncompressed, 6176 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: SocketSwap/context_manager.py
 Comment: 
 
 Filename: SocketSwap/proxy.py
 Comment: 
 
-Filename: SocketSwap-0.1.2.dist-info/LICENSE
+Filename: SocketSwap-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: SocketSwap-0.1.2.dist-info/METADATA
+Filename: SocketSwap-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: SocketSwap-0.1.2.dist-info/WHEEL
+Filename: SocketSwap-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: SocketSwap-0.1.2.dist-info/top_level.txt
+Filename: SocketSwap-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: SocketSwap-0.1.2.dist-info/RECORD
+Filename: SocketSwap-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SocketSwap/__init__.py

```diff
@@ -4,12 +4,15 @@
 SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 """
 
 __version__ = "0.1.0"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
-from SocketSwap.context_manager import SocketSwapContext
+from socketswap.context_manager import SocketSwapContext
+from socketswap.proxy import start_local_proxy
+
 
 __all__ = [
-    SocketSwapContext
+    SocketSwapContext,
+    start_local_proxy
 ]
```

## SocketSwap/context_manager.py

```diff
@@ -1,45 +1,31 @@
-
+"""
+Module to wrap the TCP proxy in a context manager daemon process
+"""
 import multiprocessing
-from socketswap.proxy import start_local_proxy
-import socket
+import socketswap.proxy as proxy
 import time
+import logging
 
-
-# def wrap_start_proxy(args):
-#     start_local_proxy(*args)
+logger = logging.getLogger("socketswap")
+logger.addHandler(logging.NullHandler())
 
 
 class SocketSwapContext:
     
     def __init__(self, *args):
         self.args = args
     
     def __enter__(self):
-        print("Starting Proxy Server")
-        self.proxy_process = multiprocessing.Process(target=start_local_proxy, args=(self.args))
+        logger.info("Starting Proxy Server")
+        self.proxy_process = multiprocessing.Process(target=proxy.start_local_proxy, args=(self.args))
         self.proxy_process.daemon = True
         self.proxy_process.start()
         time.sleep(1)
         return self
     
     def __exit__(self, exc_type, exc_value, traceback):
-        print("Exiting proxy server")
+        logger.info("Exiting proxy server")
         self.proxy_process.terminate()
         
 
-def conn_factory():
-    target_host = "localhost"
-    target_port = 5432
-    remote_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    remote_socket.connect((target_host, target_port))
-    return remote_socket
-
-if __name__ == '__main__':
-    # for testing
-    
-    
-    with SocketSwapContext(conn_factory, "127.0.0.1", 2222):
-        for i in range(1000):
-            print(i)
-            time.sleep(3)
```

## SocketSwap/proxy.py

```diff
@@ -1,49 +1,131 @@
+"""
+Module to start a TCP proxy
+"""
 import sys
 import threading
 import socket
 import ssl
 import select
 import errno
+import logging
+from typing import Callable, List
+
+logger = logging.getLogger("socketswap")
+logger.addHandler(logging.NullHandler())
+
 
 proxy_socket = None
 
 def is_valid_ip4(ip):
-    # some rudimentary checks if ip is actually a valid IP
-    octets = ip.split('.')
+    """Check if a string is a valid IPv4 address.
+
+    Args:
+        ip (str): A string representing an IPv4 address in the format "X.X.X.X".
+
+    Returns:
+        bool: True if the input string is a valid IPv4 address, False otherwise.
+
+    Raises:
+        None.
+
+    This function splits the input string by periods and checks if it contains exactly 4 octets. It then verifies that each
+    octet is an integer between 0 and 255 inclusive. Returns True if the input string is a valid IPv4 address, False otherwise.
+    """
+    octets = ip.split(".")
     if len(octets) != 4:
         return False
     return octets[0] != 0 and all(0 <= int(octet) <= 255 for octet in octets)
 
 
-def receive_from(s):
-    # receive data from a socket until no more data is there
+def receive_from(sock):
+    """
+    Receive data from a socket until no more data is available.
+
+    Parameters:
+    - sock (socket.socket): a socket object representing a network connection.
+
+    Returns:
+    - A bytes object containing all the data received from the socket.
+
+    Notes:
+    - This function receives data from the socket in chunks of 4096 bytes at a time, and concatenates them to a single bytes object.
+    - The function stops receiving data from the socket when either the socket connection is closed or the last chunk of data received is less than 4096 bytes.
+    - This function blocks until data is available from the socket or the socket is closed.
+
+    Example:
+    >>> import socket
+    >>> sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    >>> sock.connect(("www.google.com", 80))
+    >>> sock.sendall(b"GET / HTTP/1.1\r\nHost: www.google.com\r\n\r\n")
+    >>> response = receive_from(sock)
+    >>> print(response)
+    b'HTTP/1.1 200 OK\r\nDate: Fri, 23 Apr 2023 22:12:17 GMT\r\nServer: gws\r\nContent-Type: text/html; charset=ISO-8859-1\r\n...
+    """
     b = b""
     while True:
-        data = s.recv(4096)
+        data = sock.recv(4096)
         b += data
         if not data or len(data) < 4096:
             break
     return b
 
 
-
 def is_client_hello(sock):
+    """
+    Check if a given socket contains a ClientHello message for SSL/TLS.
+
+    Parameters:
+    - sock (socket.socket): a socket object representing a network connection.
+
+    Returns:
+    - True if the socket's first bytes represent a ClientHello message for SSL/TLS, False otherwise.
+
+    Notes:
+    - This function does not consume any data from the socket, but only peeks at its first bytes with a maximum size of 128.
+    - The function checks if the first byte is 0x16, which is the SSL/TLS handshake message type for ClientHello.
+    - The function checks if the next two bytes represent the SSL/TLS protocol version and can be one of [b"\x03\x00", b"\x03\x01", b"\x03\x02", b"\x03\x03", b"\x02\x00"].
+
+    Example:
+    >>> import socket
+    >>> sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    >>> sock.connect(("www.google.com", 443))
+    >>> is_client_hello(sock)
+    True
+    """
     firstbytes = sock.recv(128, socket.MSG_PEEK)
     return (len(firstbytes) >= 3 and
             firstbytes[0] == 0x16 and
             firstbytes[1:3] in [b"\x03\x00",
                                 b"\x03\x01",
                                 b"\x03\x02",
                                 b"\x03\x03",
                                 b"\x02\x00"]
             )
 
 
 def enable_ssl(server_key, server_certificate, client_key, client_certificate, remote_socket, local_socket):
+    """
+    Enable SSL/TLS encryption for a given connection.
+
+    Parameters:
+    - server_key (str): path to the private key file for the server-side SSL/TLS connection
+    - server_certificate (str): path to the certificate file for the server-side SSL/TLS connection
+    - client_key (str): path to the private key file for the client-side SSL/TLS connection (optional)
+    - client_certificate (str): path to the certificate file for the client-side SSL/TLS connection (optional)
+    - remote_socket (socket.socket): socket object representing the remote endpoint of the connection
+    - local_socket (socket.socket): socket object representing the local endpoint of the connection
+
+    Returns:
+    - A list of two socket objects representing the wrapped remote and local sockets, respectively, with SSL/TLS encryption layers.
+
+    Raises:
+    - ssl.SSLError: if an SSL/TLS handshake error occurs during the setup process.
+    """
+
     sni = None
 
     def sni_callback(sock, name, ctx):
         nonlocal sni
         sni = name
 
     try:
@@ -52,176 +134,196 @@
         ctx.load_cert_chain(certfile=server_certificate,
                             keyfile=server_key,
                             )
         local_socket = ctx.wrap_socket(local_socket,
                                        server_side=True,
                                        )
     except ssl.SSLError as e:
-        print("SSL handshake failed for listening socket", str(e))
+        logger.error(f"SSL handshake failed for listening socket: {e}")
         raise
 
     try:
         ctx = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
         ctx.check_hostname = False
         ctx.verify_mode = ssl.CERT_NONE
+        
         if client_certificate and client_key:
-            ctx.load_cert_chain(certfile=client_certificate,
-                                keyfile=client_key,
-                                )
-        remote_socket = ctx.wrap_socket(remote_socket,
-                                        server_hostname=sni,
-                                        )
+            ctx.load_cert_chain(certfile=client_certificate, keyfile=client_key)
+            
+        remote_socket = ctx.wrap_socket(remote_socket, server_hostname=sni)
+        
     except ssl.SSLError as e:
-        print("SSL handshake failed for remote socket", str(e))
+        logger.error(f"SSL handshake failed for remote socket: {e}")
         raise
 
     return [remote_socket, local_socket]
 
 
-def starttls(use_ssl, local_socket, read_sockets):
+def starttls(use_ssl: bool, local_socket: socket.socket, read_sockets: List[socket.socket]) -> bool:
+    """Check if a socket should start a TLS handshake (STARTTLS).
+
+    Args:
+        use_ssl (bool): A boolean indicating if STARTTLS should be used.
+        local_socket (socket.socket): A local socket to be checked for the STARTTLS handshake.
+        read_sockets (List[socket.socket]): A list of sockets that the server is listening to.
+
+    Returns:
+        bool: True if the local socket should start a TLS handshake, False otherwise.
+
+    Raises:
+        None.
+
+    This function checks if the STARTTLS option is enabled, if the local socket is ready to read, if it is not already an
+    SSL socket, and if it is sending a Client Hello message. If all conditions are met, the function returns True indicating
+    that a STARTTLS handshake should be initiated.
+
+    """
     return (use_ssl and
             local_socket in read_sockets and
             not isinstance(local_socket, ssl.SSLSocket) and
             is_client_hello(local_socket)
             )
 
 
-def proxy_thread(connect_socket, local_socket, use_ssl, server_key, server_certificate, client_key, client_certificate):
-
+def proxy_thread(socket_factory: Callable[[], socket.socket], local_socket: socket.socket, use_ssl: bool, server_key: str, server_certificate: str, client_key: str, client_certificate: str):
+    """handles each connection read/write in a seperate thread"""
     try:
-        remote_socket = connect_socket()
-    except socket.error as serr:
-        if serr.errno == errno.ECONNREFUSED:
-            for s in [remote_socket, local_socket]:
-                s.close()
-            print("connect socket - Connection refused")
-            return None
-        elif serr.errno == errno.ETIMEDOUT:
-            for s in [remote_socket, local_socket]:
-                s.close()
-            print("connect socket - Connection timed out")
-            return None
-        else:
-            for s in [remote_socket, local_socket]:
-                s.close()
-            raise serr
+        remote_socket = socket_factory()
+    except socket.error as socket_error:
+        
+        logger.error(f"SOCKET ERROR connecting remote socket: {socket_error}")
+        for s in [remote_socket, local_socket]:
+            s.close()
+            
+        # TODO braucht man hier den noch? (errno.errorcode[errnumber], os.strerror(errnumber))
+        if socket_error.errno not in (errno.ETIMEDOUT, errno.ECONNREFUSED):
+            raise socket_error
+        return None
+        
     
     running = True
     while running:
         read_sockets, _, _ = select.select([remote_socket, local_socket], [], [])
 
         if starttls(use_ssl, local_socket, read_sockets):
             try:
                 ssl_sockets = enable_ssl(server_key, server_certificate, client_key, client_certificate, remote_socket, local_socket)
                 remote_socket, local_socket = ssl_sockets
-                print( "SSL enabled")
+                logger.info("SSL enabled")
             except ssl.SSLError as e:
-                print("SSL handshake failed", str(e))
+                logger.error(f"SSL handshake failed: {e}")
                 break
 
             read_sockets, _, _ = select.select(ssl_sockets, [], [])
 
         for sock in read_sockets:
             try:
                 peer = sock.getpeername()
-            except socket.error as serr:
-                if serr.errno == errno.ENOTCONN:
+            except socket.error as socket_error:
+                if socket_error.errno == errno.ENOTCONN:
                     # kind of a blind shot at fixing issue #15
                     # I don't yet understand how this error can happen, but if it happens I'll just shut down the thread
                     # the connection is not in a useful state anymore
                     for s in [remote_socket, local_socket]:
                         s.close()
                     running = False
                     break
                 else:
-                    print(f" Socket exception in start_proxy_thread")
-                    raise serr
+                    logger.info(f"Socket exception in start_proxy_thread")
+                    raise socket_error
 
             data = receive_from(sock)
-            print( 'Received %d bytes' % len(data))
+            logger.info(f"Received {len(data)} bytes")
 
             if sock == local_socket:
                 if len(data):
-                    print( b'< < < out\n' + data)
+                    logger.info( b'< < < out\n' + data)
                     remote_socket.send(data.encode() if isinstance(data, str) else data)
                 else:
-                    print( "Connection from local client %s:%d closed" % peer)
+                    logger.info( "Connection from local client %s:%d closed" % peer)
                     remote_socket.close()
                     running = False
                     break
             elif sock == remote_socket:
                 if len(data):
-                    print( b'> > > in\n' + data)
+                    logger.info( b'> > > in\n' + data)
                     local_socket.send(data)
                 else:
-                    print( "Connection to remote server %s:%d closed" % peer)
+                    logger.info( "Connection to remote server %s:%d closed" % peer)
                     local_socket.close()
                     running = False
                     break
            
 
 
 def start_local_proxy(connect_socket, local_host, local_port, server_key=None, server_certificate=None, client_key=None, client_certificate=None, use_ssl=False):
-    
-    print("hey")
+    """starts a local proxy server"""
     global proxy_socket
+    logger.info("Starting local proxy server")
+    
     if ((client_key is None) ^ (client_certificate is None)):
-        print("You must either specify both the client certificate and client key or leave both empty")
+        logger.error("You must either specify both the client certificate and client key or leave both empty")
         sys.exit(8)
 
     if local_host != '0.0.0.0' and not is_valid_ip4(local_host):
         try:
             ip = socket.gethostbyname(local_host)
         except socket.gaierror:
             ip = False
         if ip is False:
-            print('%s is not a valid IP address or host name' % local_host)
+            logger.error(f"Provided listening host is not a valid IP address or host name: {local_host}")
             sys.exit(1)
         else:
             local_host = ip
 
 
     # local proxy socket
     proxy_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     proxy_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
     try:
         proxy_socket.bind((local_host, local_port))
     except socket.error as e:
-        print(e.strerror)
+        logger.error(e.strerror)
         sys.exit(5)
 
     proxy_socket.listen(100)
     try:
         while True:
             in_socket, in_addrinfo = proxy_socket.accept()
-            print( 'Connection from %s:%d' % in_addrinfo)
+            logger.info( 'Connection from %s:%d' % in_addrinfo)
             pthread = threading.Thread(
                 target=proxy_thread, 
                 args=(connect_socket, in_socket, use_ssl, server_key, server_certificate, client_key, client_certificate)
             )
-            print( "Starting proxy thread " + pthread.name)
+            logger.info(f"Starting proxy thread {pthread.name}")
             pthread.start()
-    except KeyboardInterrupt:
-        print( 'Ctrl+C detected, exiting...')
+    except KeyboardInterrupt as e:
+        logger.info(e)
         sys.exit(0)
 
 
 def stop_local_proxy():
     global proxy_socket
     try:
         if proxy_socket:
             proxy_socket.close()
-    except:
-        print("close exception")
+    except Exception as e:
+        logger.error(f"Exception on closing listening socket: {e}")
 
 
 if __name__ == '__main__':
     # for testing
     
+    
+    
+    logger = logging.getLogger("socketswap")
+    logger.addHandler(logging.StreamHandler())
+    logger.setLevel(logging.DEBUG)
+
     import socket
     
 
     def conn_factory():
         target_host = "localhost"
         target_port = 5432
         remote_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
```

## Comparing `SocketSwap-0.1.2.dist-info/LICENSE` & `SocketSwap-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SocketSwap-0.1.2.dist-info/METADATA` & `SocketSwap-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SocketSwap
-Version: 0.1.2
+Version: 0.1.3
 Summary: SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 Home-page: https://github.com/fyx99/SocketSwap
 Author: fxy99
 Author-email: 
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

