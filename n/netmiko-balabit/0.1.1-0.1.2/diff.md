# Comparing `tmp/netmiko_balabit-0.1.1-py3-none-any.whl.zip` & `tmp/netmiko_balabit-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7980 bytes, number of entries: 7
--rw-r--r--  2.0 unx       88 b- defN 22-Aug-23 13:32 netmiko_balabit/__init__.py
--rw-r--r--  2.0 unx     4998 b- defN 22-Aug-23 13:32 netmiko_balabit/balabit_scb_ssh.py
--rwxr-xr-x  2.0 unx    11357 b- defN 22-Aug-23 13:37 netmiko_balabit-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1658 b- defN 22-Aug-23 13:37 netmiko_balabit-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-23 13:37 netmiko_balabit-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 22-Aug-23 13:37 netmiko_balabit-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      600 b- defN 22-Aug-23 13:37 netmiko_balabit-0.1.1.dist-info/RECORD
-7 files, 18809 bytes uncompressed, 6906 bytes compressed:  63.3%
+Zip file size: 7998 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       88 b- defN 22-Aug-23 13:49 netmiko_balabit/__init__.py
+-rw-r--r--  2.0 unx     5038 b- defN 23-Apr-24 20:33 netmiko_balabit/balabit_scb_ssh.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Apr-24 20:35 netmiko_balabit-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1677 b- defN 23-Apr-24 20:35 netmiko_balabit-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 20:35 netmiko_balabit-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-24 20:35 netmiko_balabit-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      600 b- defN 23-Apr-24 20:35 netmiko_balabit-0.1.2.dist-info/RECORD
+7 files, 18868 bytes uncompressed, 6924 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: netmiko_balabit/__init__.py
 Comment: 
 
 Filename: netmiko_balabit/balabit_scb_ssh.py
 Comment: 
 
-Filename: netmiko_balabit-0.1.1.dist-info/LICENSE
+Filename: netmiko_balabit-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: netmiko_balabit-0.1.1.dist-info/METADATA
+Filename: netmiko_balabit-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: netmiko_balabit-0.1.1.dist-info/WHEEL
+Filename: netmiko_balabit-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: netmiko_balabit-0.1.1.dist-info/top_level.txt
+Filename: netmiko_balabit-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: netmiko_balabit-0.1.1.dist-info/RECORD
+Filename: netmiko_balabit-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netmiko_balabit/balabit_scb_ssh.py

```diff
@@ -32,15 +32,16 @@
         """Removes secrets (no_log) from messages"""
         if self.no_log:
             for hidden_data in self.no_log.values():
                 if isinstance(hidden_data, list):
                     for item in hidden_data:
                         record.msg = record.msg.replace(item, "********")
                 else:
-                    record.msg = record.msg.replace(hidden_data, "********")
+                    if hidden_data:
+                        record.msg = record.msg.replace(hidden_data, "********")
         return True
 
 
 import netmiko
 
 netmiko.base_connection.SecretsFilter = SecretsFilter
```

## Comparing `netmiko_balabit-0.1.1.dist-info/LICENSE` & `netmiko_balabit-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netmiko_balabit-0.1.1.dist-info/METADATA` & `netmiko_balabit-0.1.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: netmiko-balabit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Out of tree netmiko driver for balabit scb
 Home-page: https://github.com/jinjamator/netmiko_balabit
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
@@ -58,7 +59,8 @@
 - Issue Tracker: https://github.com/jinjamator/netmiko_balabit/issues
 - Source Code: https://github.com/jinjamator/netmiko_balabit
 
 License
 -----------------
 
 This project is licensed under the Apache License Version 2.0
+
```

