# Comparing `tmp/tfrecord-1.8.tar.gz` & `tmp/tfrecord-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tfrecord-1.8.tar", last modified: Thu Jan 23 07:19:54 2020, max compression
+gzip compressed data, was "dist/tfrecord-1.9.tar", last modified: Sun Feb 23 01:51:57 2020, max compression
```

## Comparing `tfrecord-1.8.tar` & `tfrecord-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2020-01-23 07:19:54.000000 tfrecord-1.8/
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2020-01-23 07:19:54.000000 tfrecord-1.8/tfrecord/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     2213 2019-12-13 06:09:55.000000 tfrecord-1.8/tfrecord/writer.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)    17910 2019-11-23 18:51:39.000000 tfrecord-1.8/tfrecord/example_pb2.py
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2020-01-23 07:19:54.000000 tfrecord-1.8/tfrecord/tools/
--rw-r--r--   0 vahid     (1000) vahid     (1000)      881 2020-01-19 21:50:57.000000 tfrecord-1.8/tfrecord/tools/tfrecord2idx.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        0 2019-11-27 04:36:26.000000 tfrecord-1.8/tfrecord/tools/__init__.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1172 2019-12-13 06:08:11.000000 tfrecord-1.8/tfrecord/iterator_utils.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     4830 2019-12-13 06:09:20.000000 tfrecord-1.8/tfrecord/reader.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       95 2019-12-13 06:10:24.000000 tfrecord-1.8/tfrecord/__init__.py
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2020-01-23 07:19:54.000000 tfrecord-1.8/tfrecord/torch/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        0 2019-11-26 03:57:38.000000 tfrecord-1.8/tfrecord/torch/__init__.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1811 2019-12-13 06:11:11.000000 tfrecord-1.8/tfrecord/torch/dataset.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      227 2020-01-23 07:19:54.000000 tfrecord-1.8/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      388 2020-01-23 07:19:48.000000 tfrecord-1.8/setup.py
+drwxr-xr-x   0 vahid      (501) staff       (20)        0 2020-02-23 01:51:57.000000 tfrecord-1.9/
+-rw-r--r--   0 vahid      (501) staff       (20)      227 2020-02-23 01:51:57.000000 tfrecord-1.9/PKG-INFO
+-rw-r--r--   0 vahid      (501) staff       (20)      388 2020-02-23 01:51:06.000000 tfrecord-1.9/setup.py
+drwxr-xr-x   0 vahid      (501) staff       (20)        0 2020-02-23 01:51:57.000000 tfrecord-1.9/tfrecord/
+-rw-r--r--   0 vahid      (501) staff       (20)       95 2020-02-13 05:41:22.000000 tfrecord-1.9/tfrecord/__init__.py
+-rw-r--r--   0 vahid      (501) staff       (20)    17910 2019-11-26 08:49:17.000000 tfrecord-1.9/tfrecord/example_pb2.py
+-rw-r--r--   0 vahid      (501) staff       (20)     1172 2019-11-26 08:49:17.000000 tfrecord-1.9/tfrecord/iterator_utils.py
+-rw-r--r--   0 vahid      (501) staff       (20)     4899 2020-02-13 05:41:22.000000 tfrecord-1.9/tfrecord/reader.py
+drwxr-xr-x   0 vahid      (501) staff       (20)        0 2020-02-23 01:51:57.000000 tfrecord-1.9/tfrecord/tools/
+-rw-r--r--   0 vahid      (501) staff       (20)        0 2019-11-26 08:49:17.000000 tfrecord-1.9/tfrecord/tools/__init__.py
+-rw-r--r--   0 vahid      (501) staff       (20)      881 2020-02-13 05:41:22.000000 tfrecord-1.9/tfrecord/tools/tfrecord2idx.py
+drwxr-xr-x   0 vahid      (501) staff       (20)        0 2020-02-23 01:51:57.000000 tfrecord-1.9/tfrecord/torch/
+-rw-r--r--   0 vahid      (501) staff       (20)        0 2019-11-26 08:49:17.000000 tfrecord-1.9/tfrecord/torch/__init__.py
+-rw-r--r--   0 vahid      (501) staff       (20)     1811 2020-02-13 05:41:22.000000 tfrecord-1.9/tfrecord/torch/dataset.py
+-rw-r--r--   0 vahid      (501) staff       (20)     2213 2020-02-13 05:41:22.000000 tfrecord-1.9/tfrecord/writer.py
```

### Comparing `tfrecord-1.8/tfrecord/writer.py` & `tfrecord-1.9/tfrecord/writer.py`

 * *Files identical despite different names*

### Comparing `tfrecord-1.8/tfrecord/example_pb2.py` & `tfrecord-1.9/tfrecord/example_pb2.py`

 * *Files identical despite different names*

### Comparing `tfrecord-1.8/tfrecord/tools/tfrecord2idx.py` & `tfrecord-1.9/tfrecord/tools/tfrecord2idx.py`

 * *Files identical despite different names*

### Comparing `tfrecord-1.8/tfrecord/iterator_utils.py` & `tfrecord-1.9/tfrecord/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `tfrecord-1.8/tfrecord/reader.py` & `tfrecord-1.9/tfrecord/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,28 @@
     file = io.open(data_path, "rb")
 
     length_bytes = bytearray(8)
     crc_bytes = bytearray(4)
     datum_bytes = bytearray(1024*1024)
 
     def read_records(start_offset=None, end_offset=None):
+        nonlocal length_bytes, crc_bytes, datum_bytes
+
         if start_offset is not None:
             file.seek(start_offset)
         if end_offset is None:
             end_offset = os.path.getsize(data_path)
         while file.tell() < end_offset:
             if file.readinto(length_bytes) != 8:
                 raise RuntimeError("Failed to read the record size.")
             if file.readinto(crc_bytes) != 4:
                 raise RuntimeError("Failed to read the start token.")
             length, = struct.unpack("<Q", length_bytes)
             if length > len(datum_bytes):
-                datum_bytes.zfill(int(length * 1.5))
+                datum_bytes = datum_bytes.zfill(int(length * 1.5))
             datum_bytes_view = memoryview(datum_bytes)[:length]
             if file.readinto(datum_bytes_view) != length:
                 raise RuntimeError("Failed to read the record.")
             if file.readinto(crc_bytes) != 4:
                 raise RuntimeError("Failed to read the end token.")
             yield datum_bytes_view
```

### Comparing `tfrecord-1.8/tfrecord/torch/dataset.py` & `tfrecord-1.9/tfrecord/torch/dataset.py`

 * *Files identical despite different names*

