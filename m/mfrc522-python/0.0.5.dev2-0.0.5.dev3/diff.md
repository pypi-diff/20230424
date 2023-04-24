# Comparing `tmp/mfrc522-python-0.0.5.dev2.tar.gz` & `tmp/mfrc522-python-0.0.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.5.dev2.tar", last modified: Mon Apr 24 08:02:59 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.5.dev3.tar", last modified: Mon Apr 24 08:16:37 2023, max compression
```

## Comparing `mfrc522-python-0.0.5.dev2.tar` & `mfrc522-python-0.0.5.dev3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.545494 mfrc522-python-0.0.5.dev2/
--rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev2/LICENSE
--rw-rw-rw-   0        0        0     3018 2023-04-24 08:02:59.543495 mfrc522-python-0.0.5.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev2/README.md
--rw-rw-rw-   0        0        0      665 2023-04-24 07:59:38.000000 mfrc522-python-0.0.5.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 08:02:59.546562 mfrc522-python-0.0.5.dev2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.349629 mfrc522-python-0.0.5.dev2/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.497467 mfrc522-python-0.0.5.dev2/src/mfrc522/
--rw-rw-rw-   0        0        0     5617 2023-04-24 07:58:49.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/BasicMFRC522.py
--rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0     3368 2023-04-19 16:18:45.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/SimpleMFRC522.py
--rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev2/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:02:59.540496 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0     3018 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 08:02:59.000000 mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 08:16:37.216541 mfrc522-python-0.0.5.dev3/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev3/LICENSE
+-rw-rw-rw-   0        0        0     3018 2023-04-24 08:16:37.207886 mfrc522-python-0.0.5.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev3/README.md
+-rw-rw-rw-   0        0        0      665 2023-04-24 08:15:30.000000 mfrc522-python-0.0.5.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:16:37.216541 mfrc522-python-0.0.5.dev3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 08:16:35.339265 mfrc522-python-0.0.5.dev3/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:16:37.158364 mfrc522-python-0.0.5.dev3/src/mfrc522/
+-rw-rw-rw-   0        0        0     5688 2023-04-24 08:14:25.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/BasicMFRC522.py
+-rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0     3281 2023-04-24 08:12:53.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/SimpleMFRC522.py
+-rw-rw-rw-   0        0        0      130 2023-04-24 08:10:04.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:16:37.207886 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3018 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.5.dev2/LICENSE` & `mfrc522-python-0.0.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev2/PKG-INFO` & `mfrc522-python-0.0.5.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.5.dev2
+Version: 0.0.5.dev3
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mfrc522-python-0.0.5.dev2/README.md` & `mfrc522-python-0.0.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev2/pyproject.toml` & `mfrc522-python-0.0.5.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.5.dev2"
+version = "0.0.5.dev3"
 authors = [
   { name="Aditya"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mfrc522-python-0.0.5.dev2/src/mfrc522/BasicMFRC522.py` & `mfrc522-python-0.0.5.dev3/src/mfrc522/BasicMFRC522.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from . import MFRC522
 
+
 class BasicMFRC522:
     def __init__(self, KEY=[0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]):
         self.MFRC522 = MFRC522()
         self.KEY = KEY
-    
+
     def read_sector(self, trailer_block=11):
-        id, text = self.read_no_block(trailer_block, (trailer_block-3, trailer_block-2, trailer_block-1))
+        id, text = self.read_no_block(
+            trailer_block, (trailer_block-3, trailer_block-2, trailer_block-1))
         while not id:
-            id, text = self.read_no_block(trailer_block, (trailer_block-3, trailer_block-2, trailer_block-1))
+            id, text = self.read_no_block(
+                trailer_block, (trailer_block-3, trailer_block-2, trailer_block-1))
         return id, text
-    
+
     def read_sectors(self, trailer_blocks=[11]):
         text_all = ''
         for trailer_block in trailer_blocks:
             id, text = self.read_sector(trailer_block)
             text_all += text
         return id, text_all
 
@@ -68,30 +71,32 @@
         return id, text_in
 
     def write_sectors(self, text, trailer_blocks=[11]):
         text_formated_list = self.split_string(text)
         text_all = ''
         for i in range(0, len(trailer_blocks)):
             try:
-                id, text = self.write_sector(text_formated_list[i], trailer_blocks[i])
+                id, text = self.write_sector(
+                    text_formated_list[i], trailer_blocks[i])
                 text_all += text
             except IndexError:
                 pass
         return id, text_all
 
     def write_no_block(self, text, trailer_block, block_addr):
         (status, TagType) = self.MFRC522.Request(self.MFRC522.PICC_REQIDL)
         if status != self.MFRC522.MI_OK:
             return None, None
         (status, uid) = self.MFRC522.Anticoll()
         if status != self.MFRC522.MI_OK:
             return None, None
         id = self.uid_to_num(uid)
         self.MFRC522.SelectTag(uid)
-        status = self.MFRC522.Authenticate(self.MFRC522.PICC_AUTHENT1A, trailer_block, self.KEY, uid)
+        status = self.MFRC522.Authenticate(
+            self.MFRC522.PICC_AUTHENT1A, trailer_block, self.KEY, uid)
         self.MFRC522.ReadTag(trailer_block)
         try:
             if status == self.MFRC522.MI_OK:
                 data = bytearray()
                 data.extend(bytearray(text.ljust(
                     len(block_addr) * 16).encode('ascii')))
                 i = 0
@@ -100,38 +105,25 @@
                     i += 1
             self.MFRC522.StopCrypto1()
             return id, text[0:(len(block_addr) * 16)]
         except:
             self.MFRC522.StopCrypto1()
             return None, None
 
-    def uid_to_num(self, uid):
-        n = 0
-        for i in range(0, 5):
-            n = n * 256 + uid[i]
-        return n
-
-    def split_string(self, s):
-        l = list()
-        for i in range(0, len(s), 48):
-            l.append(s[i:i+48]) 
-        if len(l[-1]) < 48:
-            l[-1] += '\0'*(48-len(l[-1]))
-        return l
-    
     def clear_no_sector(self, trailer_block):
         (status, TagType) = self.MFRC522.Request(self.MFRC522.PICC_REQIDL)
         if status != self.MFRC522.MI_OK:
             return None
         (status, uid) = self.MFRC522.Anticoll()
         if status != self.MFRC522.MI_OK:
             return None
         id = self.uid_to_num(uid)
         self.MFRC522.SelectTag(uid)
-        status = self.MFRC522.Authenticate(self.MFRC522.PICC_AUTHENT1A, trailer_block, self.KEY, uid)
+        status = self.MFRC522.Authenticate(
+            self.MFRC522.PICC_AUTHENT1A, trailer_block, self.KEY, uid)
         self.MFRC522.ReadTag(trailer_block)
         block_addr = [trailer_block-3, trailer_block-2, trailer_block-1]
         try:
             if status == self.MFRC522.MI_OK:
                 data = [0x00]*16
                 for block_num in block_addr:
                     self.MFRC522.WriteTag(block_num, data)
@@ -142,7 +134,21 @@
             return None
 
     def clear_sector(self, trailer_block):
         id = self.clear_no_sector(trailer_block)
         while not id:
             id = self.clear_no_sector(trailer_block)
         return id
+
+    def uid_to_num(self, uid):
+        n = 0
+        for i in range(0, 5):
+            n = n * 256 + uid[i]
+        return n
+
+    def split_string(self, s):
+        l = list()
+        for i in range(0, len(s), 48):
+            l.append(s[i:i+48])
+        if len(l[-1]) < 48:
+            l[-1] += '\0'*(48-len(l[-1]))
+        return l
```

### Comparing `mfrc522-python-0.0.5.dev2/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.5.dev3/src/mfrc522/MFRC522.py`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev2/src/mfrc522/SimpleMFRC522.py` & `mfrc522-python-0.0.5.dev3/src/mfrc522/SimpleMFRC522.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from . import MFRC522
 
+
 class SimpleMFRC522:
     def __init__(self):
-        self.READER = MFRC522()
+        self.MFRC522 = MFRC522()
         self.KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
         self.BLOCK_ADDRS = [8, 9, 10]
 
     def read(self):
         id, text = self.read_no_block()
         while not id:
             id, text = self.read_no_block()
@@ -15,80 +16,80 @@
     def read_id(self):
         id = self.read_id_no_block()
         while not id:
             id = self.read_id_no_block()
         return id
 
     def read_id_no_block(self):
-        (status, TagType) = self.READER.MFRC522_Request(self.READER.PICC_REQIDL)
-        if status != self.READER.MI_OK:
+        (status, TagType) = self.MFRC522.Request(self.MFRC522.PICC_REQIDL)
+        if status != self.MFRC522.MI_OK:
             return None
-        (status, uid) = self.READER.MFRC522_Anticoll()
-        if status != self.READER.MI_OK:
+        (status, uid) = self.MFRC522.Anticoll()
+        if status != self.MFRC522.MI_OK:
             return None
         return self.uid_to_num(uid)
 
     def read_no_block(self):
-        (status, TagType) = self.READER.MFRC522_Request(self.READER.PICC_REQIDL)
-        if status != self.READER.MI_OK:
+        (status, TagType) = self.MFRC522.Request(self.MFRC522.PICC_REQIDL)
+        if status != self.MFRC522.MI_OK:
             return None, None
-        (status, uid) = self.READER.MFRC522_Anticoll()
-        if status != self.READER.MI_OK:
+        (status, uid) = self.MFRC522.Anticoll()
+        if status != self.MFRC522.MI_OK:
             return None, None
         id = self.uid_to_num(uid)
-        self.READER.MFRC522_SelectTag(uid)
-        status = self.READER.MFRC522_Auth(
-            self.READER.PICC_AUTHENT1A, 11, self.KEY, uid)
+        self.MFRC522.SelectTag(uid)
+        status = self.MFRC522.Authenticate(
+            self.MFRC522.PICC_AUTHENT1A, 11, self.KEY, uid)
         try:
             data = []
             text_read = ''
-            if status == self.READER.MI_OK:
+            if status == self.MFRC522.MI_OK:
                 for block_num in self.BLOCK_ADDRS:
-                    block = self.READER.MFRC522_Read(block_num)
+                    block = self.MFRC522.Read(block_num)
                     if block:
                         data += block
                 if data:
                     text_read = ''.join(chr(i) for i in data)
-            self.READER.MFRC522_StopCrypto1()
+            self.MFRC522.StopCrypto1()
             return id, text_read
         except:
-            self.READER.MFRC522_StopCrypto1()
+            self.MFRC522.StopCrypto1()
             return None, None
 
     def write(self, text):
         id, text_in = self.write_no_block(text)
         while not id:
             id, text_in = self.write_no_block(text)
         return id, text_in
 
     def write_no_block(self, text):
-        (status, TagType) = self.READER.MFRC522_Request(self.READER.PICC_REQIDL)
-        if status != self.READER.MI_OK:
+        (status, TagType) = self.MFRC522.Request(self.MFRC522.PICC_REQIDL)
+        if status != self.MFRC522.MI_OK:
             return None, None
-        (status, uid) = self.READER.MFRC522_Anticoll()
-        if status != self.READER.MI_OK:
+        (status, uid) = self.MFRC522.Anticoll()
+        if status != self.MFRC522.MI_OK:
             return None, None
         id = self.uid_to_num(uid)
-        self.READER.MFRC522_SelectTag(uid)
-        status = self.READER.MFRC522_Auth(
-            self.READER.PICC_AUTHENT1A, 11, self.KEY, uid)
+        self.MFRC522.SelectTag(uid)
+        status = self.MFRC522.Authenticate(
+            self.MFRC522.PICC_AUTHENT1A, 11, self.KEY, uid)
         try:
-            self.READER.MFRC522_Read(11)
-            if status == self.READER.MI_OK:
+            self.MFRC522.Read(11)
+            if status == self.MFRC522.MI_OK:
                 data = bytearray()
                 data.extend(bytearray(text.ljust(
                     len(self.BLOCK_ADDRS) * 16).encode('ascii')))
                 i = 0
                 for block_num in self.BLOCK_ADDRS:
-                    self.READER.MFRC522_Write(block_num, data[(i*16):(i+1)*16])
+                    self.MFRC522.Write(block_num, data[(i*16):(i+1)*16])
                     i += 1
-            self.READER.MFRC522_StopCrypto1()
+            self.MFRC522.StopCrypto1()
             return id, text[0:(len(self.BLOCK_ADDRS) * 16)]
         except:
-            self.READER.MFRC522_StopCrypto1()
+            self.MFRC522.StopCrypto1()
             return None, None
 
     def uid_to_num(self, uid):
         n = 0
         for i in range(0, 5):
             n = n * 256 + uid[i]
         return n
```

### Comparing `mfrc522-python-0.0.5.dev2/src/mfrc522_python.egg-info/PKG-INFO` & `mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.5.dev2
+Version: 0.0.5.dev3
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

