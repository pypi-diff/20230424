# Comparing `tmp/smpplib-2.2.2.tar.gz` & `tmp/smpplib-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpplib-2.2.2.tar", last modified: Thu Mar  9 18:50:11 2023, max compression
+gzip compressed data, was "smpplib-2.2.3.tar", last modified: Mon Apr 24 16:56:34 2023, max compression
```

## Comparing `smpplib-2.2.2.tar` & `smpplib-2.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-03-09 18:50:11.147783 smpplib-2.2.2/
--rw-r--r--   0 eigenein   (501) staff       (20)     7652 2020-03-10 17:46:00.000000 smpplib-2.2.2/LICENSE
--rw-r--r--   0 eigenein   (501) staff       (20)     4186 2023-03-09 18:50:11.147475 smpplib-2.2.2/PKG-INFO
--rw-r--r--   0 eigenein   (501) staff       (20)     3111 2021-10-19 19:01:17.000000 smpplib-2.2.2/README.md
--rw-r--r--   0 eigenein   (501) staff       (20)       38 2023-03-09 18:50:11.147831 smpplib-2.2.2/setup.cfg
--rw-r--r--   0 eigenein   (501) staff       (20)     1494 2023-03-09 18:49:30.000000 smpplib-2.2.2/setup.py
-drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-03-09 18:50:11.135480 smpplib-2.2.2/smpplib/
--rw-r--r--   0 eigenein   (501) staff       (20)      876 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/__init__.py
--rw-r--r--   0 eigenein   (501) staff       (20)    14214 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/client.py
--rw-r--r--   0 eigenein   (501) staff       (20)    34169 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/command.py
--rw-r--r--   0 eigenein   (501) staff       (20)     1633 2018-10-15 14:01:29.000000 smpplib-2.2.2/smpplib/command_codes.py
--rw-r--r--   0 eigenein   (501) staff       (20)    13991 2020-03-10 17:46:00.000000 smpplib-2.2.2/smpplib/consts.py
--rw-r--r--   0 eigenein   (501) staff       (20)      311 2018-02-19 11:31:03.000000 smpplib-2.2.2/smpplib/exceptions.py
--rw-r--r--   0 eigenein   (501) staff       (20)     3504 2021-11-22 10:59:21.000000 smpplib-2.2.2/smpplib/gsm.py
--rw-r--r--   0 eigenein   (501) staff       (20)     3929 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/pdu.py
--rw-r--r--   0 eigenein   (501) staff       (20)     1026 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/ptypes.py
--rw-r--r--   0 eigenein   (501) staff       (20)     1235 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/smpp.py
-drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-03-09 18:50:11.146764 smpplib-2.2.2/smpplib/tests/
--rw-r--r--   0 eigenein   (501) staff       (20)        0 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/tests/__init__.py
--rw-r--r--   0 eigenein   (501) staff       (20)     1358 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/tests/test_client.py
--rw-r--r--   0 eigenein   (501) staff       (20)     2196 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/tests/test_command.py
--rw-r--r--   0 eigenein   (501) staff       (20)     2197 2021-10-19 19:16:36.000000 smpplib-2.2.2/smpplib/tests/test_gsm.py
-drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-03-09 18:50:11.142989 smpplib-2.2.2/smpplib.egg-info/
--rw-r--r--   0 eigenein   (501) staff       (20)     4186 2023-03-09 18:50:11.000000 smpplib-2.2.2/smpplib.egg-info/PKG-INFO
--rw-r--r--   0 eigenein   (501) staff       (20)      503 2023-03-09 18:50:11.000000 smpplib-2.2.2/smpplib.egg-info/SOURCES.txt
--rw-r--r--   0 eigenein   (501) staff       (20)        1 2023-03-09 18:50:11.000000 smpplib-2.2.2/smpplib.egg-info/dependency_links.txt
--rw-r--r--   0 eigenein   (501) staff       (20)       64 2023-03-09 18:50:11.000000 smpplib-2.2.2/smpplib.egg-info/requires.txt
--rw-r--r--   0 eigenein   (501) staff       (20)        8 2023-03-09 18:50:11.000000 smpplib-2.2.2/smpplib.egg-info/top_level.txt
--rw-r--r--   0 eigenein   (501) staff       (20)        1 2019-02-06 13:13:18.000000 smpplib-2.2.2/smpplib.egg-info/zip-safe
+drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-04-24 16:56:34.920524 smpplib-2.2.3/
+-rw-r--r--   0 eigenein   (501) staff       (20)     7652 2020-03-10 17:46:00.000000 smpplib-2.2.3/LICENSE
+-rw-r--r--   0 eigenein   (501) staff       (20)     4191 2023-04-24 16:56:34.920196 smpplib-2.2.3/PKG-INFO
+-rw-r--r--   0 eigenein   (501) staff       (20)     3111 2021-10-19 19:01:17.000000 smpplib-2.2.3/README.md
+-rw-r--r--   0 eigenein   (501) staff       (20)       38 2023-04-24 16:56:34.920567 smpplib-2.2.3/setup.cfg
+-rw-r--r--   0 eigenein   (501) staff       (20)     1499 2023-04-24 16:53:52.000000 smpplib-2.2.3/setup.py
+drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-04-24 16:56:34.913625 smpplib-2.2.3/smpplib/
+-rw-r--r--   0 eigenein   (501) staff       (20)      876 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/__init__.py
+-rw-r--r--   0 eigenein   (501) staff       (20)    14016 2023-04-24 16:47:29.000000 smpplib-2.2.3/smpplib/client.py
+-rw-r--r--   0 eigenein   (501) staff       (20)    34085 2023-04-24 16:47:29.000000 smpplib-2.2.3/smpplib/command.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     1633 2018-10-15 14:01:29.000000 smpplib-2.2.3/smpplib/command_codes.py
+-rw-r--r--   0 eigenein   (501) staff       (20)    13992 2023-04-24 16:51:08.000000 smpplib-2.2.3/smpplib/consts.py
+-rw-r--r--   0 eigenein   (501) staff       (20)      311 2018-02-19 11:31:03.000000 smpplib-2.2.3/smpplib/exceptions.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     3504 2021-11-22 10:59:21.000000 smpplib-2.2.3/smpplib/gsm.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     3929 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/pdu.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     1026 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/ptypes.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     1235 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/smpp.py
+drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-04-24 16:56:34.919793 smpplib-2.2.3/smpplib/tests/
+-rw-r--r--   0 eigenein   (501) staff       (20)        0 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/tests/__init__.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     1358 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/tests/test_client.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     2353 2023-04-24 16:47:29.000000 smpplib-2.2.3/smpplib/tests/test_command.py
+-rw-r--r--   0 eigenein   (501) staff       (20)     2197 2021-10-19 19:16:36.000000 smpplib-2.2.3/smpplib/tests/test_gsm.py
+drwxr-xr-x   0 eigenein   (501) staff       (20)        0 2023-04-24 16:56:34.916823 smpplib-2.2.3/smpplib.egg-info/
+-rw-r--r--   0 eigenein   (501) staff       (20)     4191 2023-04-24 16:56:34.000000 smpplib-2.2.3/smpplib.egg-info/PKG-INFO
+-rw-r--r--   0 eigenein   (501) staff       (20)      503 2023-04-24 16:56:34.000000 smpplib-2.2.3/smpplib.egg-info/SOURCES.txt
+-rw-r--r--   0 eigenein   (501) staff       (20)        1 2023-04-24 16:56:34.000000 smpplib-2.2.3/smpplib.egg-info/dependency_links.txt
+-rw-r--r--   0 eigenein   (501) staff       (20)       64 2023-04-24 16:56:34.000000 smpplib-2.2.3/smpplib.egg-info/requires.txt
+-rw-r--r--   0 eigenein   (501) staff       (20)        8 2023-04-24 16:56:34.000000 smpplib-2.2.3/smpplib.egg-info/top_level.txt
+-rw-r--r--   0 eigenein   (501) staff       (20)        1 2019-02-06 13:13:18.000000 smpplib-2.2.3/smpplib.egg-info/zip-safe
```

### Comparing `smpplib-2.2.2/LICENSE` & `smpplib-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/PKG-INFO` & `smpplib-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smpplib
-Version: 2.2.2
+Version: 2.2.3
 Summary: SMPP library for python
-Home-page: https://github.com/podshumok/python-smpplib
+Home-page: https://github.com/python-smpplib/python-smpplib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smpplib-2.2.2/README.md` & `smpplib-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/setup.py` & `smpplib-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
         long_description_content_type='text/markdown',
     )
 except OSError:
     long_description_kwd=dict()
 
 setup(
     name='smpplib',
-    version='2.2.2',
-    url='https://github.com/podshumok/python-smpplib',
+    version='2.2.3',
+    url='https://github.com/python-smpplib/python-smpplib',
     description='SMPP library for python',
     packages=find_packages(),
     install_requires=['six'],
     extras_require=dict(
         tests=('typing; python_version < "3.5"', 'pytest', 'mock'),
     ),
     zip_safe=True,
```

### Comparing `smpplib-2.2.2/smpplib/__init__.py` & `smpplib-2.2.3/smpplib/__init__.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/client.py` & `smpplib-2.2.3/smpplib/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,66 +203,59 @@
         if self.state not in consts.COMMAND_STATES[p.command]:
             raise exceptions.PDUError("Command %s failed: %s" % (
                 p.command,
                 consts.DESCRIPTIONS[consts.SMPP_ESME_RINVBNDSTS],
             ))
 
         self.logger.debug('Sending %s PDU', p.command)
-
         generated = p.generate()
-
         self.logger.debug('>>%s (%d bytes)', binascii.b2a_hex(generated), len(generated))
 
-        sent = 0
+        try:
+            self._socket.sendall(generated)
+        except socket.error as e:
+            self.logger.warning(e)
+            raise exceptions.ConnectionError()
+
+        return True
 
-        while sent < len(generated):
+    def _recv_exact(self, exact_size):
+        """
+        Keep reading from self._socket until exact_size bytes have been read
+        """
+        parts = []
+        received = 0
+        while received < exact_size:
             try:
-                sent_last = self._socket.send(generated[sent:])
+                part = self._socket.recv(exact_size - received)
+            except socket.timeout:
+                raise
             except socket.error as e:
                 self.logger.warning(e)
                 raise exceptions.ConnectionError()
-            if sent_last == 0:
+            if not part:
                 raise exceptions.ConnectionError()
-            sent += sent_last
-
-        return True
+            received += len(part)
+            parts.append(part)
+        return b"".join(parts)
 
     def read_pdu(self):
         """Read PDU from the SMSC"""
 
         self.logger.debug('Waiting for PDU...')
 
-        try:
-            raw_len = self._socket.recv(4)
-        except socket.timeout:
-            raise
-        except socket.error as e:
-            self.logger.warning(e)
-            raise exceptions.ConnectionError()
-        if not raw_len:
-            raise exceptions.ConnectionError()
+        raw_len = self._recv_exact(4)
 
         try:
             length = struct.unpack('>L', raw_len)[0]
         except struct.error:
             self.logger.warning('Receive broken pdu... %s', repr(raw_len))
             raise exceptions.PDUError('Broken PDU')
 
-        raw_pdu = raw_len
-        while len(raw_pdu) < length:
-            try:
-                raw_pdu_part = self._socket.recv(length - len(raw_pdu))
-            except socket.timeout:
-                raise
-            except socket.error as e:
-                self.logger.warning(e)
-                raise exceptions.ConnectionError()
-            if not raw_pdu:
-                raise exceptions.ConnectionError()
-            raw_pdu += raw_pdu_part
+        raw_pdu = raw_len + self._recv_exact(length - 4)
 
         self.logger.debug('<<%s (%d bytes)', binascii.b2a_hex(raw_pdu), len(raw_pdu))
 
         pdu = smpp.parse_pdu(
             raw_pdu,
             client=self,
             allow_unknown_opt_params=self.allow_unknown_opt_params,
```

### Comparing `smpplib-2.2.2/smpplib/command.py` & `smpplib-2.2.3/smpplib/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
     # Order is important, but params dictionary is unordered
     params_order = (
         'system_id', 'password', 'system_type',
         'interface_version', 'addr_ton', 'addr_npi', 'address_range',
     )
 
     def __init__(self, command, **kwargs):
-        super(BindTransmitter, self).__init__(command, need_sequence=False, **kwargs)
+        super(BindTransmitter, self).__init__(command, **kwargs)
 
         self._set_vars(**(dict.fromkeys(self.params)))
         self.interface_version = consts.SMPP_VERSION_34
 
 
 class BindReceiver(BindTransmitter):
     """Bind as a receiver command"""
@@ -813,15 +813,15 @@
         'callback_num', 'source_subaddress',
         'dest_subaddress', 'language_indicator', 'its_session_info',
         'network_error_code', 'message_state', 'receipted_message_id',
         'source_network_type', 'dest_network_type', 'more_messages_to_send',
     )
 
     def __init__(self, command, **kwargs):
-        super(DeliverSM, self).__init__(command, need_sequence=False, **kwargs)
+        super(DeliverSM, self).__init__(command, **kwargs)
         self._set_vars(**(dict.fromkeys(self.params)))
 
 
 class DeliverSMResp(SubmitSMResp):
     """deliver_sm_response response class, same as submit_sm"""
     message_id = None
 
@@ -896,15 +896,15 @@
 class Unbind(Command):
     """Unbind command"""
 
     params = {}
     params_order = ()
 
     def __init__(self, command, **kwargs):
-        super(Unbind, self).__init__(command, need_sequence=False, **kwargs)
+        super(Unbind, self).__init__(command, **kwargs)
 
 
 class UnbindResp(Command):
     """Unbind response command"""
 
     params = {}
     params_order = ()
@@ -915,15 +915,15 @@
 
 class EnquireLink(Command):
     """Enquire link command"""
     params = {}
     params_order = ()
 
     def __init__(self, command, **kwargs):
-        super(EnquireLink, self).__init__(command, need_sequence=False, **kwargs)
+        super(EnquireLink, self).__init__(command, **kwargs)
 
 
 class EnquireLinkResp(Command):
     """Enquire link command response"""
     params = {}
     params_order = ()
```

### Comparing `smpplib-2.2.2/smpplib/command_codes.py` & `smpplib-2.2.3/smpplib/command_codes.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/consts.py` & `smpplib-2.2.3/smpplib/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 NULL_STRING = b'\0'
 
 
 # Message part lengths in different encodings.
 # SMPP 3.4, 2.2.1.2
 SEVENBIT_LENGTH = 160
 EIGHTBIT_LENGTH = 140
-UCS2_LENGTH = 70
+UCS2_LENGTH = 140
 
 MULTIPART_HEADER_SIZE = 6
 
 SEVENBIT_PART_SIZE = SEVENBIT_LENGTH - 7  # TODO: where does 7 come from?
 EIGHTBIT_PART_SIZE = 140 - MULTIPART_HEADER_SIZE
 UCS2_PART_SIZE = 140 - MULTIPART_HEADER_SIZE  # must be an even number anyway
```

### Comparing `smpplib-2.2.2/smpplib/gsm.py` & `smpplib-2.2.3/smpplib/gsm.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/pdu.py` & `smpplib-2.2.3/smpplib/pdu.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/ptypes.py` & `smpplib-2.2.3/smpplib/ptypes.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/smpp.py` & `smpplib-2.2.3/smpplib/smpp.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/tests/test_client.py` & `smpplib-2.2.3/smpplib/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib/tests/test_command.py` & `smpplib-2.2.3/smpplib/tests/test_command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from smpplib import consts, exceptions
+from smpplib.client import Client
 from smpplib.command import DeliverSM
 
 import pytest
 
 
 def test_parse_deliver_sm():
-    pdu = DeliverSM('deliver_sm')
+    client = Client("localhost", 5679)
+    pdu = DeliverSM('deliver_sm', client=client)
     pdu.parse(
         b"\x00\x00\x00\xcb\x00\x00\x00\x05\x00\x00\x00\x00\x00\x00\x00\x01\x00"
         b"\x01\x0131600000000\x00\x05\x00XXX YYYY\x00\x04\x00\x00\x00\x00\x00"
         b"\x00\x00\x00\x00\x00\x0e\x00\x01\x01\x00\x06\x00\x01\x01\x00\x1e\x00"
         b"\t1d305b4c\x00\x04'\x00\x01\x02\x04$\x00rid:0489708364 sub:001"
         b" dlvrd:001 submit date:1810151907 done date:1810151907 stat:DELIVRD"
         b" err:000 text:\x04\x1f\x04@\x048\x042\x045\x04B\x04&\x00\x01\x01"
@@ -22,25 +24,26 @@
     assert pdu.receipted_message_id == b'1d305b4c'
     assert pdu.source_network_type == consts.SMPP_NETWORK_TYPE_GSM
     assert pdu.message_state == consts.SMPP_MESSAGE_STATE_DELIVERED
     assert pdu.user_message_reference is None
 
 
 def test_unrecognised_optional_parameters():
-    pdu = DeliverSM("deliver_sm", allow_unknown_opt_params=True)
+    client = Client("localhost", 5679)
+    pdu = DeliverSM("deliver_sm", client=client, allow_unknown_opt_params=True)
     pdu.parse(b'\x00\x00\x00\xa8\x00\x00\x00\x05\x00\x00\x00\x00/p\xc6'
               b'\x9a\x00\x00\x0022549909028\x00\x01\x00\x00\x04\x00\x00'
               b'\x00\x00\x00\x00\x00\x00iid:795920026 sub:001 dlvrd:001 '
               b'submit date:200319131913 done date:200319131913 stat:DELIVRD err:000 text:'
               b'\x14\x03\x00\x07(null)\x00\x14\x02\x00\x04612\x00'
     )
 
     # This is only to avoid a breaking change, at some point the other behaviour
     # should become the default.
     with pytest.raises(exceptions.UnknownCommandError):
-        pdu2 = DeliverSM("deliver_sm")
+        pdu2 = DeliverSM("deliver_sm", client=client)
         pdu2.parse(b'\x00\x00\x00\xa8\x00\x00\x00\x05\x00\x00\x00\x00/p\xc6'
                   b'\x9a\x00\x00\x0022549909028\x00\x01\x00\x00\x04\x00\x00'
                   b'\x00\x00\x00\x00\x00\x00iid:795920026 sub:001 dlvrd:001 '
                   b'submit date:200319131913 done date:200319131913 stat:DELIVRD err:000 text:'
                   b'\x14\x03\x00\x07(null)\x00\x14\x02\x00\x04612\x00'
         )
```

### Comparing `smpplib-2.2.2/smpplib/tests/test_gsm.py` & `smpplib-2.2.3/smpplib/tests/test_gsm.py`

 * *Files identical despite different names*

### Comparing `smpplib-2.2.2/smpplib.egg-info/PKG-INFO` & `smpplib-2.2.3/smpplib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smpplib
-Version: 2.2.2
+Version: 2.2.3
 Summary: SMPP library for python
-Home-page: https://github.com/podshumok/python-smpplib
+Home-page: https://github.com/python-smpplib/python-smpplib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

