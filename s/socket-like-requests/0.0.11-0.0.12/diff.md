# Comparing `tmp/socket_like_requests-0.0.11.tar.gz` & `tmp/socket_like_requests-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket_like_requests-0.0.11.tar", last modified: Thu Mar 30 17:54:02 2023, max compression
+gzip compressed data, was "socket_like_requests-0.0.12.tar", last modified: Mon Apr 24 11:54:41 2023, max compression
```

## Comparing `socket_like_requests-0.0.11.tar` & `socket_like_requests-0.0.12.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 17:54:02.427467 socket_like_requests-0.0.11/
--rw-rw-rw-   0        0        0     1072 2023-03-02 13:13:30.000000 socket_like_requests-0.0.11/LICENSE.txt
--rw-rw-rw-   0        0        0      641 2023-03-30 17:54:02.427467 socket_like_requests-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2216 2023-03-02 14:03:50.000000 socket_like_requests-0.0.11/README.md
--rw-rw-rw-   0        0        0      115 2023-03-30 17:54:02.428465 socket_like_requests-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-03-30 17:53:55.000000 socket_like_requests-0.0.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 17:54:02.413504 socket_like_requests-0.0.11/socket_like_requests/
--rw-rw-rw-   0        0        0       20 2023-03-03 16:29:48.000000 socket_like_requests-0.0.11/socket_like_requests/__init__.py
--rw-rw-rw-   0        0        0     7281 2023-03-30 17:53:38.000000 socket_like_requests-0.0.11/socket_like_requests/slr.py
-drwxrwxrwx   0        0        0        0 2023-03-30 17:54:02.425472 socket_like_requests-0.0.11/socket_like_requests.egg-info/
--rw-rw-rw-   0        0        0      641 2023-03-30 17:54:02.000000 socket_like_requests-0.0.11/socket_like_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-03-30 17:54:02.000000 socket_like_requests-0.0.11/socket_like_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 17:54:02.000000 socket_like_requests-0.0.11/socket_like_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-03-30 17:54:02.000000 socket_like_requests-0.0.11/socket_like_requests.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 11:54:41.532766 socket_like_requests-0.0.12/
+-rw-rw-rw-   0        0        0     1072 2023-03-02 13:13:30.000000 socket_like_requests-0.0.12/LICENSE.txt
+-rw-rw-rw-   0        0        0      641 2023-04-24 11:54:41.532766 socket_like_requests-0.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2216 2023-03-02 14:03:50.000000 socket_like_requests-0.0.12/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-24 11:54:41.534762 socket_like_requests-0.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-04-24 11:50:32.000000 socket_like_requests-0.0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:54:41.510826 socket_like_requests-0.0.12/socket_like_requests/
+-rw-rw-rw-   0        0        0       20 2023-03-03 16:29:48.000000 socket_like_requests-0.0.12/socket_like_requests/__init__.py
+-rw-rw-rw-   0        0        0     7795 2023-04-24 11:50:25.000000 socket_like_requests-0.0.12/socket_like_requests/slr.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:54:41.531802 socket_like_requests-0.0.12/socket_like_requests.egg-info/
+-rw-rw-rw-   0        0        0      641 2023-04-24 11:54:41.000000 socket_like_requests-0.0.12/socket_like_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-24 11:54:41.000000 socket_like_requests-0.0.12/socket_like_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 11:54:41.000000 socket_like_requests-0.0.12/socket_like_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-24 11:54:41.000000 socket_like_requests-0.0.12/socket_like_requests.egg-info/top_level.txt
```

### Comparing `socket_like_requests-0.0.11/LICENSE.txt` & `socket_like_requests-0.0.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socket_like_requests-0.0.11/PKG-INFO` & `socket_like_requests-0.0.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: socket_like_requests
-Version: 0.0.11
+Version: 0.0.12
 Summary: Use Socket Like Requests Module
 Home-page: https://github.com/zvhh/Socket-Like-Requests
-Download-URL: https://github.com/zvhh/Socket-Like-Requests/archive/refs/tags/0.0.11.tar.gz
+Download-URL: https://github.com/zvhh/Socket-Like-Requests/archive/refs/tags/0.0.12.tar.gz
 Author: Sami
 Author-email: sami2700@outlook.com
 License: MIT
 Keywords: Requests,TCP Request,Socket
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `socket_like_requests-0.0.11/README.md` & `socket_like_requests-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `socket_like_requests-0.0.11/setup.py` & `socket_like_requests-0.0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'socket_like_requests',
   packages = ['socket_like_requests'],
-  version = '0.0.11',
+  version = '0.0.12',
   license='MIT',
   description = 'Use Socket Like Requests Module',
   author = 'Sami',         
   author_email = 'sami2700@outlook.com', 
   url = 'https://github.com/zvhh/Socket-Like-Requests',
-  download_url = 'https://github.com/zvhh/Socket-Like-Requests/archive/refs/tags/0.0.11.tar.gz',   
+  download_url = 'https://github.com/zvhh/Socket-Like-Requests/archive/refs/tags/0.0.12.tar.gz',   
   keywords = ['Requests', 'TCP Request', 'Socket'],
   install_requires=[          
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
```

### Comparing `socket_like_requests-0.0.11/socket_like_requests/slr.py` & `socket_like_requests-0.0.12/socket_like_requests/slr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import socket, ssl, base64, struct
 
-
-# For Any Help Contact Me :
-# instagram : zvhk
-# email : sami2700@outlook.com
-# discord : zvhk#0007
-
 class REQ:
     
     def __init__(self):
         #print('test')
         pass
     
     
     def data(self, data=None):
         
-        if not len(data) < 1:
+        if data != None:
         
             ls = []
 
             for m, n in data.items():
                 ls.append(f'{m}={n}')
                 
             zx = '&'.join(ls)
@@ -28,14 +22,23 @@
             
             return zx
         
     def hed(self, hed=None):
         
         a = []
         
+        if hed == None:
+            
+            hed = {}
+            hed['User-Agent'] = f'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36'
+            hed['Accept-Language'] = 'en-US'
+            hed['Accept'] = '*/*'
+            hed['Connection'] = 'close'
+            hed['Content-Type'] = 'application/x-www-form-urlencoded'
+
         for k, v in hed.items():
             if 'Content-Length' in k or 'Host' in k:
                 pass
             
             else:
                 a.append(f'{k}: {v}\r\n')
 
@@ -91,15 +94,15 @@
         
     #     if not response.__contains__(b'200'): # Need Test Again
     #         raise Exception('Proxy Failed')
         
     #     return s
     def https(self, s, auth):
         
-        s.sendall(f'CONNECT {self.path}:{self.port} HTTP/1.1\r\n\r\n{auth}'.encode())
+        s.sendall(f'CONNECT {self.path}:{self.port} HTTP/1.1\r\n{auth}\r\n\r\n'.encode())
         response = s.recv(70)
         
         return s
         
     def socks4(self, s):
         
         s.sendall(b'\x04\x01' + struct.pack('>H', self.port) + socket.inet_aton(socket.gethostbyname(f'{self.path}')) + b'\x00')
@@ -144,16 +147,17 @@
         
         return s
     
     
     def verify(self, s):
         
         if self.port == 443:
-        
-            s = ssl.create_default_context().wrap_socket(s, server_hostname=f'{self.path}')
+
+            #s = ssl.create_default_context().wrap_socket(s, server_hostname=f'{self.path}')
+            s = ssl.wrap_socket(s)
     
         return s
 
     def path_de(self, path, hh=None, po=None):
         
         ho, xz = path.split('://')
         
@@ -243,64 +247,75 @@
         return s, hh
         
         
     def send(self, path, method=None, hed=None, data=None, proxy=None, verify=None, proxy_type=None, auth=None, timeout=5):
         
         self.path, hh, self.port = self.path_de(path)
 
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM, 0)
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         socket.setdefaulttimeout(timeout)
         
         s, hh = self.conf(s, path, proxy, proxy_type, auth, verify, hh)
         
         hed = f'{method} {hh} HTTP/1.1\r\nHost: {self.path}\r\n{self.hed(hed)}{self.data(data)}'.encode()
         
         #print(hed, '\n\n')
-
-        s.sendall(hed)
-        
         lst = []
         
+        s.sendall(hed)
+
         while True:
+            
             data = s.recv(1024)
             if (len(data) < 1):
                 break
             lst.append(data.decode())
-            
     
         qz = ' '.join(lst)
-        
+
         s.close()
 
         return Response(qz)
-        
     
     
 class Response:
     
     def __init__(self, qz):
         self.qz = qz
+
+        
     
     @property
     def text(self):
-    
-            
+
         q = self.qz.split('\r\n\r\n')[1]
 
         return q
-    
-    
+
     @property
     def sc(self):
         
-        status_code = int(self.qz.splitlines()[0].split(' ')[1])
+        try:
 
-        return status_code
-    
+            status_code = int(self.qz.splitlines()[0].split(' ')[1])
+
+            return status_code
+        
+        except:
+
+            if 'Too many open connections' in self.qz:
+                
+                return 421
+
+            elif 'Bad Request' in self.qz:
+
+                return 400
+
+        
     @property
     def headers(self):
         
         cont = self.qz.split('\r\n\r\n')[0]
         
         return cont
```

### Comparing `socket_like_requests-0.0.11/socket_like_requests.egg-info/PKG-INFO` & `socket_like_requests-0.0.12/socket_like_requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: socket-like-requests
-Version: 0.0.11
+Version: 0.0.12
 Summary: Use Socket Like Requests Module
 Home-page: https://github.com/zvhh/Socket-Like-Requests
-Download-URL: https://github.com/zvhh/Socket-Like-Requests/archive/refs/tags/0.0.11.tar.gz
+Download-URL: https://github.com/zvhh/Socket-Like-Requests/archive/refs/tags/0.0.12.tar.gz
 Author: Sami
 Author-email: sami2700@outlook.com
 License: MIT
 Keywords: Requests,TCP Request,Socket
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

