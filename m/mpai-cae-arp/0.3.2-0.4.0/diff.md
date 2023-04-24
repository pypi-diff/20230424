# Comparing `tmp/mpai_cae_arp-0.3.2.tar.gz` & `tmp/mpai_cae_arp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpai_cae_arp-0.3.2.tar", max compression
+gzip compressed data, was "mpai_cae_arp-0.4.0.tar", max compression
```

## Comparing `mpai_cae_arp-0.3.2.tar` & `mpai_cae_arp-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-04-03 21:35:54.975907 mpai_cae_arp-0.3.2/LICENSE
--rw-r--r--   0        0        0      491 2023-04-03 21:22:02.773309 mpai_cae_arp-0.3.2/README.md
--rw-r--r--   0        0        0      276 2023-04-04 08:31:02.533352 mpai_cae_arp-0.3.2/mpai_cae_arp/__init__.py
--rw-r--r--   0        0        0      176 2023-04-04 07:37:21.160932 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/__init__.py
--rw-r--r--   0        0        0    17904 2023-04-06 15:03:52.274016 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_audio.py
--rw-r--r--   0        0        0     2516 2023-04-04 07:38:52.008419 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_noise.py
--rw-r--r--   0        0        0      219 2023-04-03 21:48:20.943719 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/standards.py
--rw-r--r--   0        0        0     4211 2023-04-04 07:22:07.372604 mpai_cae_arp-0.3.2/mpai_cae_arp/audio/utils.py
--rw-r--r--   0        0        0     2055 2023-04-10 18:12:57.428996 mpai_cae_arp-0.3.2/mpai_cae_arp/files.py
--rw-r--r--   0        0        0     1304 2023-04-06 14:57:19.804922 mpai_cae_arp-0.3.2/mpai_cae_arp/io.py
--rw-r--r--   0        0        0     2246 2023-04-13 16:30:33.142293 mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2.py
--rw-r--r--   0        0        0     3679 2023-04-13 16:31:08.282079 mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2_grpc.py
--rw-r--r--   0        0        0     3100 2023-04-03 21:32:30.045143 mpai_cae_arp-0.3.2/mpai_cae_arp/time.py
--rw-r--r--   0        0        0        0 2023-04-03 21:25:06.272009 mpai_cae_arp-0.3.2/mpai_cae_arp/types/__init__.py
--rw-r--r--   0        0        0     7311 2023-04-13 11:52:35.097562 mpai_cae_arp-0.3.2/mpai_cae_arp/types/irregularity.py
--rw-r--r--   0        0        0     1668 2023-04-03 21:48:21.015718 mpai_cae_arp-0.3.2/mpai_cae_arp/types/schema.py
--rw-r--r--   0        0        0     1240 2023-04-13 16:33:06.769367 mpai_cae_arp-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.2/setup.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/LICENSE
+-rw-r--r--   0        0        0      491 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/README.md
+-rw-r--r--   0        0        0      276 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/__init__.py
+-rw-r--r--   0        0        0    18021 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_audio.py
+-rw-r--r--   0        0        0     2516 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_noise.py
+-rw-r--r--   0        0        0      231 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/standards.py
+-rw-r--r--   0        0        0     4211 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/utils.py
+-rw-r--r--   0        0        0     2065 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/files.py
+-rw-r--r--   0        0        0     1437 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/io.py
+-rw-r--r--   0        0        0     2307 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2.py
+-rw-r--r--   0        0        0     4041 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2_grpc.py
+-rw-r--r--   0        0        0     3182 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/time.py
+-rw-r--r--   0        0        0      314 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/__init__.py
+-rw-r--r--   0        0        0     8323 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/irregularity.py
+-rw-r--r--   0        0        0     2293 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/restoration.py
+-rw-r--r--   0        0        0     1632 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/schema.py
+-rw-r--r--   0        0        0     1236 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.4.0/setup.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.4.0/PKG-INFO
```

### Comparing `mpai_cae_arp-0.3.2/LICENSE` & `mpai_cae_arp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_audio.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,15 @@
     """
 
     array: np.ndarray
     bit: int
     samplerate: int
     channels: int
 
-    def __init__(self, data: np.ndarray, bit: int, channels: int,
-                 samplerate: int):
+    def __init__(self, data: np.ndarray, bit: int, channels: int, samplerate: int):
         if bit not in [8, 16, 24, 32]:
             raise ValueError("bit must be 8, 16, 24 or 32")
         if samplerate < 8000 or samplerate > 192000:
             raise ValueError("samplerate must be between 8 and 192 kHz")
         self.bit = bit
         self.channels = channels
         self.samplerate = samplerate
@@ -88,16 +87,15 @@
     def __len__(self):
         return len(self.array)
 
     def __iter__(self):
         return iter(self.array)
 
     def __getitem__(self, key):
-        return AudioWave(self.array[key], self.bit, self.channels,
-                         self.samplerate)
+        return AudioWave(self.array[key], self.bit, self.channels, self.samplerate)
 
     def __eq__(self, __o: object) -> bool:
         if isinstance(__o, AudioWave):
             return np.array_equal(
                 self.array, __o.array
             ) and self.bit == __o.bit and self.channels == __o.channels and self.samplerate == __o.samplerate
         raise TypeError(f"cannot compare AudioWave with {type(__o)}")
@@ -145,16 +143,15 @@
             samplerate = fp.getframerate()
             channels = fp.getnchannels()
             bit = fp.getsampwidth() * 8
 
         return bit, channels, samplerate
 
     @staticmethod
-    def buffer_generator_from_file(filepath: str,
-                                   buffer_size: int = 1024 * 1024 * 8):
+    def buffer_generator_from_file(filepath: str, buffer_size: int = 1024 * 1024 * 8):
         """Return a generator that yields AudioWave objects from a file. The generator will read the file in chunks of `buffer_size` bytes.
 
         Parameters
         ----------
         filepath: str
             The path to the file.
         buffer_size: int
@@ -199,17 +196,15 @@
             >>> from audiohandler import AudioWave
             >>> audio = AudioWave.from_bytes(b'\\x00\\x00\\x00\\x00', 16, 2, 44100)
             >>> np.array_equal(audio.array, np.array([[0, 0]]))
             True
 
         """
         data = np.array([
-            int.from_bytes(raw_data[i:i + bit // 8],
-                           byteorder='little',
-                           signed=True)
+            int.from_bytes(raw_data[i:i + bit // 8], byteorder='little', signed=True)
             for i in range(0, len(raw_data), bit // 8)
         ])
         data = np.reshape(data, (-1, channels))
         return AudioWave(data, bit, channels, samplerate)
 
     def save(self, filepath: str, force: bool = False):
         """Save the audio as a wave file at the given path.
@@ -239,24 +234,36 @@
 
         """
 
         if not path.exists(path.dirname(filepath)):
             if force:
                 os.makedirs(path.dirname(filepath))
             else:
-                raise ValueError(
-                    f"Directory {path.dirname(filepath)} does not exist")
+                raise ValueError(f"Directory {path.dirname(filepath)} does not exist")
 
         with wave.open(filepath, 'wb') as fp:
             fp.setframerate(self.samplerate)
             fp.setnchannels(self.channels)
             fp.setsampwidth(self.bit // 8)
             fp.setnframes(self.number_of_frames())
             fp.writeframesraw(self.get_raw())
 
+    def set_sample_rate(self, samplerate: int):
+        """Set the sample rate of the audio.
+
+        .. versionadded:: 0.4.0
+
+        Parameters
+        ----------
+        samplerate: int
+            The new sample rate.
+        """
+        self.array = librosa.resample(self.array, self.samplerate, samplerate)
+        self.samplerate = samplerate
+
     def get_raw(self) -> bytes:
         """Get the raw data of the audio.
 
         Returns:
             A bytes stream in the form (left right left right ...), where left and right are the samples for the left and right channels respectively for each frame in little endian format and signed.
         """
         data: np.ndarray = np.reshape(self.array, (-1, ))
@@ -308,17 +315,15 @@
         """
 
         mfcc_per_ch = []
 
         for channel in range(self.channels):
             signal = self.get_channel(channel).array
             signal = signal / (2 ^ (self.bit - 1))  # normalize the signal
-            mfccs = librosa.feature.mfcc(y=signal,
-                                         sr=self.samplerate,
-                                         n_mfcc=n_mfcc)
+            mfccs = librosa.feature.mfcc(y=signal, sr=self.samplerate, n_mfcc=n_mfcc)
             mean_mfccs = []
             for e in mfccs:
                 mean_mfccs.append(np.mean(e))
             mfcc_per_ch.append(mean_mfccs)
 
         # return the mean of the mfcc of each channel
         return np.mean(mfcc_per_ch, axis=0)
```

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/audio/_noise.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_noise.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/audio/utils.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/audio/utils.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/files.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from io import TextIOWrapper
 from enum import Enum
 import json
 import yaml
 from pydantic import BaseModel
 
 
-class FileAction(Enum):
+class FileAction(str, Enum):
     READ = "r"
     WRITE = "w"
     APPEND = "a"
 
 
-class FileType(Enum):
+class FileType(str, Enum):
     YAML = "yaml"
     JSON = "json"
 
 
 class File(BaseModel):
     encoding: str
     format: FileType
```

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/io.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/io.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains functions to print and format text in the console. Consider it as deprecated, use instead rich library.
+"""
 from enum import Enum
 
 END = '\033[0m'
 
 
 class Style(Enum):
     """
```

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,32 +6,31 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tarp.proto\x12\x03\x61rp\"+\n\x0bInfoRequest\x12\x12\n\x05\x66ield\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_field\"S\n\nJobRequest\x12\x13\n\x0bworking_dir\x18\x01 \x01(\t\x12\x12\n\nfiles_name\x18\x02 \x01(\t\x12\x12\n\x05index\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_index\".\n\x0bJobResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\"&\n\x07\x43ontact\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"$\n\x07License\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\"\x81\x01\n\x0cInfoResponse\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1d\n\x07\x63ontact\x18\x04 \x01(\x0b\x32\x0c.arp.Contact\x12\x1d\n\x07license\x18\x05 \x01(\x0b\x32\x0c.arp.License2f\n\x03\x41IM\x12\x30\n\x07getInfo\x12\x10.arp.InfoRequest\x1a\x11.arp.InfoResponse\"\x00\x12-\n\x04work\x12\x0f.arp.JobRequest\x1a\x10.arp.JobResponse\"\x00\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\tarp.proto\x12\x03\x61rp\"+\n\x0bInfoRequest\x12\x12\n\x05\x66ield\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_field\"S\n\nJobRequest\x12\x13\n\x0bworking_dir\x18\x01 \x01(\t\x12\x12\n\nfiles_name\x18\x02 \x01(\t\x12\x12\n\x05index\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_index\".\n\x0bJobResponse\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\"&\n\x07\x43ontact\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\"$\n\x07License\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\"\x81\x01\n\x0cInfoResponse\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x1d\n\x07\x63ontact\x18\x04 \x01(\x0b\x32\x0c.arp.Contact\x12\x1d\n\x07license\x18\x05 \x01(\x0b\x32\x0c.arp.License2f\n\x03\x41IM\x12\x30\n\x07getInfo\x12\x10.arp.InfoRequest\x1a\x11.arp.InfoResponse\"\x00\x12-\n\x04work\x12\x0f.arp.JobRequest\x1a\x10.arp.JobResponse\"\x00\x30\x01\x62\x06proto3'
+)
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arp_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-  DESCRIPTOR._options = None
-  _INFOREQUEST._serialized_start=18
-  _INFOREQUEST._serialized_end=61
-  _JOBREQUEST._serialized_start=63
-  _JOBREQUEST._serialized_end=146
-  _JOBRESPONSE._serialized_start=148
-  _JOBRESPONSE._serialized_end=194
-  _CONTACT._serialized_start=196
-  _CONTACT._serialized_end=234
-  _LICENSE._serialized_start=236
-  _LICENSE._serialized_end=272
-  _INFORESPONSE._serialized_start=275
-  _INFORESPONSE._serialized_end=404
-  _AIM._serialized_start=406
-  _AIM._serialized_end=508
+    DESCRIPTOR._options = None
+    _INFOREQUEST._serialized_start = 18
+    _INFOREQUEST._serialized_end = 61
+    _JOBREQUEST._serialized_start = 63
+    _JOBREQUEST._serialized_end = 146
+    _JOBRESPONSE._serialized_start = 148
+    _JOBRESPONSE._serialized_end = 194
+    _CONTACT._serialized_start = 196
+    _CONTACT._serialized_end = 234
+    _LICENSE._serialized_start = 236
+    _LICENSE._serialized_end = 272
+    _INFORESPONSE._serialized_start = 275
+    _INFORESPONSE._serialized_end = 404
+    _AIM._serialized_start = 406
+    _AIM._serialized_end = 508
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/network/arp_pb2_grpc.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,23 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.getInfo = channel.unary_unary(
-                '/arp.AIM/getInfo',
-                request_serializer=arp__pb2.InfoRequest.SerializeToString,
-                response_deserializer=arp__pb2.InfoResponse.FromString,
-                )
+            '/arp.AIM/getInfo',
+            request_serializer=arp__pb2.InfoRequest.SerializeToString,
+            response_deserializer=arp__pb2.InfoResponse.FromString,
+        )
         self.work = channel.unary_stream(
-                '/arp.AIM/work',
-                request_serializer=arp__pb2.JobRequest.SerializeToString,
-                response_deserializer=arp__pb2.JobResponse.FromString,
-                )
+            '/arp.AIM/work',
+            request_serializer=arp__pb2.JobRequest.SerializeToString,
+            response_deserializer=arp__pb2.JobResponse.FromString,
+        )
 
 
 class AIMServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def getInfo(self, request, context):
         """
@@ -44,60 +44,64 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_AIMServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'getInfo': grpc.unary_unary_rpc_method_handler(
-                    servicer.getInfo,
-                    request_deserializer=arp__pb2.InfoRequest.FromString,
-                    response_serializer=arp__pb2.InfoResponse.SerializeToString,
-            ),
-            'work': grpc.unary_stream_rpc_method_handler(
-                    servicer.work,
-                    request_deserializer=arp__pb2.JobRequest.FromString,
-                    response_serializer=arp__pb2.JobResponse.SerializeToString,
-            ),
+        'getInfo':
+        grpc.unary_unary_rpc_method_handler(
+            servicer.getInfo,
+            request_deserializer=arp__pb2.InfoRequest.FromString,
+            response_serializer=arp__pb2.InfoResponse.SerializeToString,
+        ),
+        'work':
+        grpc.unary_stream_rpc_method_handler(
+            servicer.work,
+            request_deserializer=arp__pb2.JobRequest.FromString,
+            response_serializer=arp__pb2.JobResponse.SerializeToString,
+        ),
     }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'arp.AIM', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
+    generic_handler = grpc.method_handlers_generic_handler('arp.AIM',
+                                                           rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler, ))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class AIM(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def getInfo(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                target,
+                options=(),
+                channel_credentials=None,
+                call_credentials=None,
+                insecure=False,
+                compression=None,
+                wait_for_ready=None,
+                timeout=None,
+                metadata=None):
         return grpc.experimental.unary_unary(request, target, '/arp.AIM/getInfo',
-            arp__pb2.InfoRequest.SerializeToString,
-            arp__pb2.InfoResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             arp__pb2.InfoRequest.SerializeToString,
+                                             arp__pb2.InfoResponse.FromString, options,
+                                             channel_credentials, insecure,
+                                             call_credentials, compression,
+                                             wait_for_ready, timeout, metadata)
 
     @staticmethod
     def work(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+             target,
+             options=(),
+             channel_credentials=None,
+             call_credentials=None,
+             insecure=False,
+             compression=None,
+             wait_for_ready=None,
+             timeout=None,
+             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/arp.AIM/work',
-            arp__pb2.JobRequest.SerializeToString,
-            arp__pb2.JobResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                              arp__pb2.JobRequest.SerializeToString,
+                                              arp__pb2.JobResponse.FromString, options,
+                                              channel_credentials, insecure,
+                                              call_credentials, compression,
+                                              wait_for_ready, timeout, metadata)
```

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/time.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/time.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module contains functions to convert time formats. The agreed time format is hh:mm:ss.msc as a string in MPAI standards.
+"""
 import datetime
 
 
 def seconds_to_string(seconds: float) -> str:
     """Converts seconds to a human readable time format (hh:mm:ss.msc).
 
     Parameters
@@ -89,19 +92,17 @@
     -------
     float
         The number of seconds
 
     """
 
     if fps <= 0:
-        raise ValueError(
-            "The number of frames per second must be greater than 0")
+        raise ValueError("The number of frames per second must be greater than 0")
     if frames < 0:
-        raise ValueError(
-            "The number of frames must be greater than or equal to 0")
+        raise ValueError("The number of frames must be greater than or equal to 0")
 
     return frames / fps
 
 
 def seconds_to_frames(seconds: float, fps: int) -> int:
     """
     Converts a number of seconds in frames.
@@ -122,14 +123,12 @@
     -------
     int
         The number of frames
 
     """
 
     if fps <= 0:
-        raise ValueError(
-            "The number of frames per second must be greater than 0")
+        raise ValueError("The number of frames per second must be greater than 0")
     if seconds < 0:
-        raise ValueError(
-            "The number of seconds must be greater than or equal to 0")
+        raise ValueError("The number of seconds must be greater than or equal to 0")
 
     return int(seconds * fps)
```

### Comparing `mpai_cae_arp-0.3.2/mpai_cae_arp/types/schema.py` & `mpai_cae_arp-0.4.0/mpai_cae_arp/types/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,17 @@
+# pylint: disable=too-few-public-methods
 from pydantic import BaseModel, Field
 
 
 class Contact(BaseModel):
     name: str = Field(..., description="Name of the contact person.")
     email: str = Field(..., description="Email of the contact person.")
 
     class Config:
-        schema_extra = {
-            "example": {
-                "name": "John Doe",
-                "email": "email@email.com"
-            }
-        }
+        schema_extra = {"example": {"name": "John Doe", "email": "email@email.com"}}
 
 
 class License(BaseModel):
     name: str = Field(..., description="Name of the license.")
     url: str = Field(..., description="URL of the license.")
 
     class Config:
@@ -29,16 +25,15 @@
 
 class Info(BaseModel):
     title: str = Field(..., description="The title of the API.")
     description: str = Field(..., description="A short description of the API.")
     version: str = Field(..., description="The version of the API.")
     contact: Contact = Field(
         ..., description="Contact information for the owners of the API.")
-    license_info: License = Field(
-        ..., description="License information for the API.")
+    license_info: License = Field(..., description="License information for the API.")
 
     class Config:
         schema_extra = {
             "example": {
                 "title": "API title",
                 "description": "A very nice API",
                 "version": "0.1.0",
```

### Comparing `mpai_cae_arp-0.3.2/pyproject.toml` & `mpai_cae_arp-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpai-cae-arp"
-version = "0.3.2"
+version = "0.4.0"
 description = "The MPAI CAE-ARP software API"
 authors = ["Matteo Spanio <dev2@audioinnova.com>"]
 readme = "README.md"
 packages = [{include = "mpai_cae_arp"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -19,15 +19,14 @@
 pylint = "^2.17.2"
 yapf = "^0.32.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.2.1"
 toml = "^0.10.2"
 
-
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -37,20 +36,20 @@
 testpaths = ["tests"]
 
 [tool.coverage.run]
 relative_files = true
 
 [tool.yapf]
 blank_line_before_nested_class_or_def = true
-column_limit = 80
+column_limit = 88
 
 [tool.pylint]
-max-line-length = 80
+max-line-length = 88
+extension-pkg-whitelist=['pydantic']
 disable = [
     "C0103",  # Invalid name
     "C0114",  # Missing module docstring
     "C0115",  # Missing class docstring
     "C0116",  # Missing function or method docstring
     "C0301",  # Line too long
-    "W0102",  # Dangerous default value
     "E1101",  # Module has no member
 ]
```

### Comparing `mpai_cae_arp-0.3.2/setup.py` & `mpai_cae_arp-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'llvmlite>=0.39.1,<0.40.0',
  'numpy==1.23.3',
  'pydantic>=1.10.7,<2.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'mpai-cae-arp',
-    'version': '0.3.2',
+    'version': '0.4.0',
     'description': 'The MPAI CAE-ARP software API',
     'long_description': '# MPAI CAE-ARP API\n\n[![LICENSE](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://img.shields.io/badge/license-GPLv3-blue.svg)\n\n## Description\n\nThis package provides a set of tools for common task in MPAI CAE-ARP standard. It is usend in the official implementation of the standard and can be used as well to develop your own.\n\n## License\n\nThis software is licensed under the GPLv3 license. See the [official site](http://www.gnu.org/licenses/gpl-3.0.html) for more information.\n',
     'author': 'Matteo Spanio',
     'author_email': 'dev2@audioinnova.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mpai_cae_arp-0.3.2/PKG-INFO` & `mpai_cae_arp-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpai-cae-arp
-Version: 0.3.2
+Version: 0.4.0
 Summary: The MPAI CAE-ARP software API
 Author: Matteo Spanio
 Author-email: dev2@audioinnova.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

