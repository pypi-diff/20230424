# Comparing `tmp/ixcom-1.3.0.tar.gz` & `tmp/ixcom-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixcom-1.3.0.tar", last modified: Thu Apr 20 13:18:24 2023, max compression
+gzip compressed data, was "ixcom-1.3.1.tar", last modified: Mon Apr 24 15:34:41 2023, max compression
```

## Comparing `ixcom-1.3.0.tar` & `ixcom-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-20 13:18:24.358921 ixcom-1.3.0/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-04-20 13:09:22.000000 ixcom-1.3.0/LICENSE
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-20 13:18:24.358921 ixcom-1.3.0/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-04-20 13:09:22.000000 ixcom-1.3.0/README.md
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-20 13:18:24.354921 ixcom-1.3.0/ixcom/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/__init__.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/cmdline.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/commands.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/crc16.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/data.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/exceptions.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/grep.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/parameters.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    70844 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/parser.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/plugin_messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42100 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/protocol.py
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-20 13:18:24.354921 ixcom-1.3.0/ixcom.egg-info/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      415 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/SOURCES.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/dependency_links.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/entry_points.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/requires.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/top_level.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-04-20 13:18:24.358921 ixcom-1.3.0/setup.cfg
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1890 2023-04-20 13:09:22.000000 ixcom-1.3.0/setup.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-24 15:34:41.770173 ixcom-1.3.1/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-04-24 15:31:45.000000 ixcom-1.3.1/LICENSE
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-24 15:34:41.770173 ixcom-1.3.1/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-04-24 15:31:45.000000 ixcom-1.3.1/README.md
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-24 15:34:41.770173 ixcom-1.3.1/ixcom/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/__init__.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/cmdline.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/commands.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/crc16.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/data.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/exceptions.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/grep.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/parameters.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71125 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/parser.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/plugin_messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42100 2023-04-24 15:31:45.000000 ixcom-1.3.1/ixcom/protocol.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-24 15:34:41.770173 ixcom-1.3.1/ixcom.egg-info/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      415 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/entry_points.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/requires.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-04-24 15:34:41.000000 ixcom-1.3.1/ixcom.egg-info/top_level.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-04-24 15:34:41.770173 ixcom-1.3.1/setup.cfg
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1890 2023-04-24 15:31:45.000000 ixcom-1.3.1/setup.py
```

### Comparing `ixcom-1.3.0/LICENSE` & `ixcom-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/PKG-INFO` & `ixcom-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.0/README.md` & `ixcom-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/cmdline.py` & `ixcom-1.3.1/ixcom/cmdline.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/commands.py` & `ixcom-1.3.1/ixcom/commands.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/crc16.py` & `ixcom-1.3.1/ixcom/crc16.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/grep.py` & `ixcom-1.3.1/ixcom/grep.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/messages.py` & `ixcom-1.3.1/ixcom/messages.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/parameters.py` & `ixcom-1.3.1/ixcom/parameters.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom/parser.py` & `ixcom-1.3.1/ixcom/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,15 @@
     '''
 
     def __init__(self, host, port=GENERAL_PORT, timeout = WAIT_TIME_FOR_RESPONSE):
         MessageParser.__init__(self)
         self.timeout = timeout
         self.host = host
         self.port = port
+        self._open_channel = -1
         self._create_socket_and_connect()
         self._stop_event = threading.Event()
         self._response_event = threading.Event()
         self._response_event.response = None
         self._parameter_event = threading.Event()
         self._parameter_event.parameter = None
         self._message_event = threading.Event()
@@ -274,14 +275,17 @@
         self._comm_thread.join()
     
     def get_commthread_handler(self):
         return self._comm_thread
 
     def get_callbackthread_handler(self):
         return self._callback_thread
+    
+    def get_open_channel(self):
+        return self._open_channel
 
     def stop(self):
         self._stop_event.set()
         self._comm_thread.join()
         self._callback_thread.join()
 
     def publish(self, message):
@@ -339,14 +343,15 @@
             ResponseError: The response from the system was not 'OK'
         
         '''
         msgToSend = data.getCommandWithID(data.XcomCommandPayload.command_id)
         msgToSend.payload.data['mode'] = data.XcomCommandParameter.channel_open
         msgToSend.payload.data['channelNumber'] = channelNumber
         self.send_msg_and_waitfor_okay(msgToSend)
+        self._open_channel = channelNumber
 
     def _update_data(self):
         while not self._stop_event.is_set():
             inputready, _, _ = select.select([self.sock], [],[], 0.1)
             for _ in inputready:
                 if self.sock.fileno() != -1:
                     try:
@@ -377,14 +382,15 @@
         msgToSend.payload.data['mode'] = data.XcomCommandParameter.channel_open
         channelNumber = LAST_CHANNEL_NUMBER
         while channelNumber >= 0:
             msgToSend.payload.data['channelNumber'] = channelNumber
             try:
                 self.send_msg_and_waitfor_okay(msgToSend)
                 self.clear_all()
+                self._open_channel = channelNumber
                 return channelNumber
             except (ResponseError, ConnectionError):
                 channelNumber -= 1
                 self._create_socket_and_connect()
             finally:
                 if channelNumber == 0:
                     raise RuntimeError('No free channel on the system!')
@@ -416,14 +422,15 @@
         msgToSend.payload.data['mode'] = data.XcomCommandParameter.channel_open
         channelNumber = 0
         while channelNumber <= LAST_CHANNEL_NUMBER:
             msgToSend.payload.data['channelNumber'] = channelNumber
             try:
                 self.send_msg_and_waitfor_okay(msgToSend)
                 self.clear_all()
+                self._open_channel = channelNumber
                 return channelNumber
             except (ResponseError, ConnectionError):
                 channelNumber += 1
                 self._create_socket_and_connect()
             finally:
                 if channelNumber > LAST_CHANNEL_NUMBER:
                     raise RuntimeError('No free channel on the system!')
@@ -438,14 +445,16 @@
             ResponseError: The response from the system was not 'OK'
         
         '''
         msgToSend = data.getCommandWithID(data.XcomCommandPayload.command_id)
         msgToSend.payload.data['mode'] = data.XcomCommandParameter.channel_close
         msgToSend.payload.data['channelNumber'] = 0
         self.send_msg_and_waitfor_okay(msgToSend)
+        self._open_channel = -1
+
 
     def reboot(self):
         '''Reboots the system
 
         Sends an XCOM reboot command on the associated socket and waits for an 'OK' response.
 
         Raises:
```

### Comparing `ixcom-1.3.0/ixcom/protocol.py` & `ixcom-1.3.1/ixcom/protocol.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.0/ixcom.egg-info/PKG-INFO` & `ixcom-1.3.1/ixcom.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.0/setup.py` & `ixcom-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 if __name__ == '__main__':
 
     readmePath = os.path.join(os.path.dirname(__file__), 'README.md')
     long_description = open(readmePath, "rt").read()
 
     setup(name='ixcom',
-          version='1.3.0',
+          version='1.3.1',
           description='Library for communicating with xcom devices over network',
           author='iMAR Navigation GmbH',
           author_email='support@imar-navigation.de',
           url='http://www.imar-navigation.de',
           keywords=['XCOM', 'Inertial navigation', 'INS', 'iMAR', 'iNAT', 'GNSS', 'GPS', 'AHRS'],
           packages=['ixcom'],
           entry_points={
```

