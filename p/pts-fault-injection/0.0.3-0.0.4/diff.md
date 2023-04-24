# Comparing `tmp/pts_fault_injection-0.0.3.tar.gz` & `tmp/pts_fault_injection-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fault_injection-0.0.3.tar", last modified: Thu Jan 26 15:10:50 2023, max compression
+gzip compressed data, was "dist/pts_fault_injection-0.0.4.tar", last modified: Mon Apr 24 18:33:37 2023, max compression
```

## Comparing `pts_fault_injection-0.0.3.tar` & `pts_fault_injection-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3470 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/pts_fault_injection/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/pts_fault_injection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3083 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/pts_fault_injection/fault_injection_box.py
--rw-rw-rw-   0 root         (0) root         (0)     8209 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/pts_fault_injection/signal_card_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7764 2023-01-26 15:10:40.000000 pts_fault_injection-0.0.3/pts_fault_injection/CANFWupdate.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-26 15:10:50.000000 pts_fault_injection-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3083 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/fault_injection_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     8204 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/signal_card_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7764 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/CANFWupdate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/setup.cfg
```

### Comparing `pts_fault_injection-0.0.3/PKG-INFO` & `pts_fault_injection-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fault_injection
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.3/setup.py` & `pts_fault_injection-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fault_injection",
-    version="0.0.3",
+    version="0.0.4",
     author="Pass testing Solutions GmbH",
     description="Fault Injection box Diagnostics package Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/pts-fault-injection-box",
     license="MIT",
```

### Comparing `pts_fault_injection-0.0.3/pts_fault_injection.egg-info/PKG-INFO` & `pts_fault_injection-0.0.4/pts_fault_injection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fault-injection
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.3/LICENSE.txt` & `pts_fault_injection-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.3/README.md` & `pts_fault_injection-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.3/pts_fault_injection/fault_injection_box.py` & `pts_fault_injection-0.0.4/pts_fault_injection/fault_injection_box.py`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.3/pts_fault_injection/signal_card_controller.py` & `pts_fault_injection-0.0.4/pts_fault_injection/signal_card_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class SignalCardController:
     """
     Base class to control all signal card relays inside a HiL
     """
 
     def __init__(self, dbc_dir):
-        self.can0 = None
+        self.bus = None
         self.can_db = cantools.database.Database()
         self.dbc_dir = dbc_dir
         print(f"Searching for DBCs in {self.dbc_dir}")
         for file in os.listdir(self.dbc_dir):
             if file.endswith(".dbc"):
                 print(f"adding {file}")
                 self.can_db.add_dbc_file(os.path.join(os.getcwd(), self.dbc_dir + file))
@@ -40,16 +40,16 @@
         Establishes a CAN connection
         :return:
         """
         # Usage with PEAK CAN Dongle
         can.rc['interface'] = interface
         can.rc['channel'] = channel
         can.rc['bitrate'] = bitrate
-        self.can0 = can.interface.Bus()
-        self.can0.flush_tx_buffer()  # Reset transmit after start
+        self.bus = can.interface.Bus()
+        self.bus.flush_tx_buffer()  # Reset transmit after start
 
     def send_can_message(self, msg_name, commands):
         try:
             cmd_message = self.can_db.get_message_by_name(msg_name)
         except Exception as e:
             print(f"ERROR: Message {msg_name} not found in Databases")
             print(e)
@@ -63,15 +63,15 @@
             else:
                 signals[signal.name] = 0
 
         message = can.Message(arbitration_id=cmd_message.frame_id,
                               data=cmd_message.encode(signals, strict=False),
                               is_extended_id=False)
         # print(f"sending message {message}")
-        self.can0.send(message)
+        self.bus.send(message)
 
     @staticmethod
     def print_bin(num):
         x = []
         for b in num:
             x.append(bin(b))
         print(x)
@@ -114,15 +114,15 @@
         cmd = {'RC_mux': card, mux_name: data}
         self.send_can_message("RC_Cntrl", cmd)
 
     def send_relay_can_message_raw(self, card, data):
         message = can.Message(arbitration_id=528,
                               data=self.create_payload(card, data),
                               is_extended_id=False)
-        self.can0.send(message)
+        self.bus.send(message)
 
     def send_cmb_relay_can_message(self, cell, type, val):
         cmd = {f'RCCMBCntrl_CV{cell}_{type}': val}
         self.send_can_message("RCCMBCntrl", cmd)
 
     def check_card(self, card, relays=None):
         if card > 16:
```

### Comparing `pts_fault_injection-0.0.3/pts_fault_injection/CANFWupdate.py` & `pts_fault_injection-0.0.4/pts_fault_injection/CANFWupdate.py`

 * *Files identical despite different names*

