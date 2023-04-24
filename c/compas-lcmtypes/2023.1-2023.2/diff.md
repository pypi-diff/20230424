# Comparing `tmp/compas_lcmtypes-2023.1.tar.gz` & `tmp/compas_lcmtypes-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_lcmtypes-2023.1.tar", max compression
+gzip compressed data, was "compas_lcmtypes-2023.2.tar", max compression
```

## Comparing `compas_lcmtypes-2023.1.tar` & `compas_lcmtypes-2023.2.tar`

### file list

```diff
@@ -1,51 +1,43 @@
--rw-r--r--   0        0        0      109 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/__init__.py
--rw-r--r--   0        0        0      249 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/__init__.py
--rw-r--r--   0        0        0     2420 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/image_metadata_t.py
--rw-r--r--   0        0        0     1917 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/image_sync_t.py
--rw-r--r--   0        0        0     4566 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/image_t.py
--rw-r--r--   0        0        0     2065 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/raw_t.py
--rw-r--r--   0        0        0      218 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/__init__.py
--rw-r--r--   0        0        0      391 2023-02-17 00:28:30.209703 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2432 2023-02-17 00:28:30.209703 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/__pycache__/ctrl_mode_t.cpython-39.pyc
--rw-r--r--   0        0        0     3113 2023-02-17 00:28:30.213703 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/__pycache__/position_t.cpython-39.pyc
--rw-r--r--   0        0        0     3100 2023-02-17 00:28:30.213703 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/__pycache__/uuv_state_t.cpython-39.pyc
--rw-r--r--   0        0        0     1983 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/ctrl_mode_t.py
--rw-r--r--   0        0        0     2500 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/position_t.py
--rw-r--r--   0        0        0     3040 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/uuv_state_t.py
--rw-r--r--   0        0        0      208 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/oi/__init__.py
--rw-r--r--   0        0        0     2221 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/oi/double_t.py
--rw-r--r--   0        0        0     5303 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/oi/kearfott_t.py
--rw-r--r--   0        0        0     6311 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/oi/rdi_pd4_t.py
--rw-r--r--   0        0        0     1196 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/__init__.py
--rw-r--r--   0        0        0     3404 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/bno055_t.py
--rw-r--r--   0        0        0     2176 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/cmd_list_t.py
--rw-r--r--   0        0        0     2025 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/cmd_t.py
--rw-r--r--   0        0        0     2024 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/depth_t.py
--rw-r--r--   0        0        0     2166 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/enable_cmd_t.py
--rw-r--r--   0        0        0     2559 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/image_depth.py
--rw-r--r--   0        0        0     2413 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/image_float32.py
--rw-r--r--   0        0        0     2621 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/imu_t.py
--rw-r--r--   0        0        0     3936 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/joystick_t.py
--rw-r--r--   0        0        0     2618 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/multibeam_polar_t.py
--rw-r--r--   0        0        0     2311 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/multibeam_t.py
--rw-r--r--   0        0        0     2585 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/multibeam_xy_t.py
--rw-r--r--   0        0        0     2665 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/oculus_sonar_t.py
--rw-r--r--   0        0        0     2573 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/prosilica_attribute_t.py
--rw-r--r--   0        0        0     2877 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/prosilica_t.py
--rw-r--r--   0        0        0     2065 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/raw_t.py
--rw-r--r--   0        0        0     2414 2023-02-17 00:26:57.844785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rdi_bathy_t.py
--rw-r--r--   0        0        0     5270 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rdi_pd4_t.py
--rw-r--r--   0        0        0     3212 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rdi_pd5_t.py
--rw-r--r--   0        0        0     2534 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/relay_activation_t.py
--rw-r--r--   0        0        0     2512 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rph_angrate_t.py
--rw-r--r--   0        0        0     2017 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rph_t.py
--rw-r--r--   0        0        0     3170 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rtidvl_nmea_t.py
--rw-r--r--   0        0        0     2125 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/std_sensor_t.py
--rw-r--r--   0        0        0     2562 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/timedrift_t.py
--rw-r--r--   0        0        0     4534 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/vn_100_Carson2014_t.py
--rw-r--r--   0        0        0     3346 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/vn_100_extra_t.py
--rw-r--r--   0        0        0     4413 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/vn_100_t.py
--rw-r--r--   0        0        0     2361 2023-02-17 00:26:57.848785 compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/yun_info_t.py
--rw-r--r--   0        0        0      312 2023-02-17 00:29:58.942583 compas_lcmtypes-2023.1/pyproject.toml
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 compas_lcmtypes-2023.1/setup.py
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 compas_lcmtypes-2023.1/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/__init__.py
+-rw-r--r--   0        0        0     2420 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/image_metadata_t.py
+-rw-r--r--   0        0        0     1917 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/image_sync_t.py
+-rw-r--r--   0        0        0     4937 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/image_t.py
+-rw-r--r--   0        0        0      423 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/__init__.py
+-rw-r--r--   0        0        0     1965 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/point_t.py
+-rw-r--r--   0        0        0     2681 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/pose_t.py
+-rw-r--r--   0        0        0     2583 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/pose_with_covariance_t.py
+-rw-r--r--   0        0        0     2080 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/quaternion_t.py
+-rw-r--r--   0        0        0     2753 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/transform_t.py
+-rw-r--r--   0        0        0     2614 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/twist_t.py
+-rw-r--r--   0        0        0     2610 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/twist_with_covariance_t.py
+-rw-r--r--   0        0        0     1987 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/geometry/vector3_t.py
+-rw-r--r--   0        0        0      272 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/__init__.py
+-rw-r--r--   0        0        0     3281 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/odometry_t.py
+-rw-r--r--   0        0        0     2837 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/pose_t.py
+-rw-r--r--   0        0        0     2600 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/position_t.py
+-rw-r--r--   0        0        0     2864 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/twist_t.py
+-rw-r--r--   0        0        0     3040 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/uuv_state_t.py
+-rw-r--r--   0        0        0      674 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/__init__.py
+-rw-r--r--   0        0        0     2644 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/battery_t.py
+-rw-r--r--   0        0        0     2593 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/cmd_list_t.py
+-rw-r--r--   0        0        0     2832 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/ctd_t.py
+-rw-r--r--   0        0        0     2436 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/depth_t.py
+-rw-r--r--   0        0        0     2932 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/dvl_t.py
+-rw-r--r--   0        0        0     2724 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/effort_cmd_t.py
+-rw-r--r--   0        0        0     4295 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/gamepad_t.py
+-rw-r--r--   0        0        0     4980 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/generic_t.py
+-rw-r--r--   0        0        0     2560 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/gps_fix_t.py
+-rw-r--r--   0        0        0     2769 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/imu_t.py
+-rw-r--r--   0        0        0     2475 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/magnetometer_t.py
+-rw-r--r--   0        0        0     2727 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/multibeam_t.py
+-rw-r--r--   0        0        0     2636 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/rph_angrate_t.py
+-rw-r--r--   0        0        0     2347 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/rph_t.py
+-rw-r--r--   0        0        0     2251 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/sig_bool_t.py
+-rw-r--r--   0        0        0     2265 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/sig_double_t.py
+-rw-r--r--   0        0        0     2242 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/sig_long_t.py
+-rw-r--r--   0        0        0      140 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/standard/__init__.py
+-rw-r--r--   0        0        0     2357 2023-02-17 00:31:37.931564 compas_lcmtypes-2023.2/compas_lcmtypes/standard/header_t.py
+-rw-r--r--   0        0        0      312 2023-02-17 00:30:18.214774 compas_lcmtypes-2023.2/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 compas_lcmtypes-2023.2/setup.py
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 compas_lcmtypes-2023.2/PKG-INFO
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/image_metadata_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/image_metadata_t.py`

 * *Files identical despite different names*

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/image_sync_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/image_sync_t.py`

 * *Files identical despite different names*

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/image_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/bot_core/image_t.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,20 @@
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
 import compas_lcmtypes.bot_core.image_metadata_t
 
+import compas_lcmtypes.standard.header_t
+
 class image_t(object):
-    __slots__ = ["utime", "width", "height", "row_stride", "pixelformat", "size", "data", "nmetadata", "metadata"]
+    __slots__ = ["header", "width", "height", "row_stride", "pixelformat", "size", "data", "nmetadata", "metadata"]
 
-    __typenames__ = ["int64_t", "int32_t", "int32_t", "int32_t", "int32_t", "int32_t", "byte", "int32_t", "compas_lcmtypes.bot_core.image_metadata_t"]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "int32_t", "int32_t", "int32_t", "int32_t", "int32_t", "byte", "int32_t", "compas_lcmtypes.bot_core.image_metadata_t"]
 
     __dimensions__ = [None, None, None, None, None, None, ["size"], None, ["nmetadata"]]
 
     PIXEL_FORMAT_UYVY = 1498831189
     PIXEL_FORMAT_YUYV = 1448695129
     PIXEL_FORMAT_IYU1 = 827677001
     PIXEL_FORMAT_IYU2 = 844454217
@@ -51,15 +53,15 @@
     PIXEL_FORMAT_BE_SIGNED_GRAY16 = 359
     PIXEL_FORMAT_BE_SIGNED_RGB16 = 360
     PIXEL_FORMAT_FLOAT_GRAY32 = 842221382
     PIXEL_FORMAT_INVALID = -2
     PIXEL_FORMAT_ANY = -1
 
     def __init__(self):
-        self.utime = 0
+        self.header = compas_lcmtypes.standard.header_t()
         self.width = 0
         self.height = 0
         self.row_stride = 0
         self.pixelformat = 0
         self.size = 0
         self.data = b""
         self.nmetadata = 0
@@ -68,15 +70,17 @@
     def encode(self):
         buf = BytesIO()
         buf.write(image_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qiiiii", self.utime, self.width, self.height, self.row_stride, self.pixelformat, self.size))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">iiiii", self.width, self.height, self.row_stride, self.pixelformat, self.size))
         buf.write(bytearray(self.data[:self.size]))
         buf.write(struct.pack(">i", self.nmetadata))
         for i0 in range(self.nmetadata):
             assert self.metadata[i0]._get_packed_fingerprint() == compas_lcmtypes.bot_core.image_metadata_t._get_packed_fingerprint()
             self.metadata[i0]._encode_one(buf)
 
     def decode(data):
@@ -87,27 +91,28 @@
         if buf.read(8) != image_t._get_packed_fingerprint():
             raise ValueError("Decode error")
         return image_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
         self = image_t()
-        self.utime, self.width, self.height, self.row_stride, self.pixelformat, self.size = struct.unpack(">qiiiii", buf.read(28))
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.width, self.height, self.row_stride, self.pixelformat, self.size = struct.unpack(">iiiii", buf.read(20))
         self.data = buf.read(self.size)
         self.nmetadata = struct.unpack(">i", buf.read(4))[0]
         self.metadata = []
         for i0 in range(self.nmetadata):
             self.metadata.append(compas_lcmtypes.bot_core.image_metadata_t._decode_one(buf))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
         if image_t in parents: return 0
         newparents = parents + [image_t]
-        tmphash = (0x6fee6cb20472ff6a+ compas_lcmtypes.bot_core.image_metadata_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
+        tmphash = (0x5f0325a1392627aa+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)+ compas_lcmtypes.bot_core.image_metadata_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
         if image_t._packed_fingerprint is None:
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/bot_core/raw_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/dvl_t.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,64 +5,79 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class raw_t(object):
-    __slots__ = ["utime", "length", "data"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "int32_t", "byte"]
+class dvl_t(object):
+    __slots__ = ["header", "btv", "wtv", "range", "altitude"]
 
-    __dimensions__ = [None, None, ["length"]]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double", "double", "double"]
+
+    __dimensions__ = [None, [4], [4], [4], None]
+
+    BTV_SENTINAL = -32.768
+    WTV_SENTINAL = -32.768
 
     def __init__(self):
-        self.utime = 0
-        self.length = 0
-        self.data = b""
+        self.header = compas_lcmtypes.standard.header_t()
+        self.btv = [ 0.0 for dim0 in range(4) ]
+        self.wtv = [ 0.0 for dim0 in range(4) ]
+        self.range = [ 0.0 for dim0 in range(4) ]
+        self.altitude = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(raw_t._get_packed_fingerprint())
+        buf.write(dvl_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qi", self.utime, self.length))
-        buf.write(bytearray(self.data[:self.length]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack('>4d', *self.btv[:4]))
+        buf.write(struct.pack('>4d', *self.wtv[:4]))
+        buf.write(struct.pack('>4d', *self.range[:4]))
+        buf.write(struct.pack(">d", self.altitude))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != raw_t._get_packed_fingerprint():
+        if buf.read(8) != dvl_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return raw_t._decode_one(buf)
+        return dvl_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = raw_t()
-        self.utime, self.length = struct.unpack(">qi", buf.read(12))
-        self.data = buf.read(self.length)
+        self = dvl_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.btv = struct.unpack('>4d', buf.read(32))
+        self.wtv = struct.unpack('>4d', buf.read(32))
+        self.range = struct.unpack('>4d', buf.read(32))
+        self.altitude = struct.unpack(">d", buf.read(8))[0]
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if raw_t in parents: return 0
-        tmphash = (0x182b8da2dc0260c7) & 0xffffffffffffffff
+        if dvl_t in parents: return 0
+        newparents = parents + [dvl_t]
+        tmphash = (0xb7277a3bfaa904bf+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if raw_t._packed_fingerprint is None:
-            raw_t._packed_fingerprint = struct.pack(">Q", raw_t._get_hash_recursive([]))
-        return raw_t._packed_fingerprint
+        if dvl_t._packed_fingerprint is None:
+            dvl_t._packed_fingerprint = struct.pack(">Q", dvl_t._get_hash_recursive([]))
+        return dvl_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", raw_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", dvl_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/ctrl_mode_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/rph_t.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,63 +5,67 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class ctrl_mode_t(object):
-    __slots__ = ["control_mode"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int16_t"]
+class rph_t(object):
+    __slots__ = ["header", "rph"]
 
-    __dimensions__ = [None]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double"]
 
-    MODE_OPEN_LOOP = 1
-    MODE_CLOSED_LOOP = 2
+    __dimensions__ = [None, [3]]
 
     def __init__(self):
-        self.control_mode = 0
+        self.header = compas_lcmtypes.standard.header_t()
+        self.rph = [ 0.0 for dim0 in range(3) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(ctrl_mode_t._get_packed_fingerprint())
+        buf.write(rph_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">h", self.control_mode))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack('>3d', *self.rph[:3]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != ctrl_mode_t._get_packed_fingerprint():
+        if buf.read(8) != rph_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return ctrl_mode_t._decode_one(buf)
+        return rph_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = ctrl_mode_t()
-        self.control_mode = struct.unpack(">h", buf.read(2))[0]
+        self = rph_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.rph = struct.unpack('>3d', buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if ctrl_mode_t in parents: return 0
-        tmphash = (0xced89b662d1db860) & 0xffffffffffffffff
+        if rph_t in parents: return 0
+        newparents = parents + [rph_t]
+        tmphash = (0xab41f2db582f8e94+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if ctrl_mode_t._packed_fingerprint is None:
-            ctrl_mode_t._packed_fingerprint = struct.pack(">Q", ctrl_mode_t._get_hash_recursive([]))
-        return ctrl_mode_t._packed_fingerprint
+        if rph_t._packed_fingerprint is None:
+            rph_t._packed_fingerprint = struct.pack(">Q", rph_t._get_hash_recursive([]))
+        return rph_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", ctrl_mode_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", rph_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/position_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/geometry/vector3_t.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,69 +5,62 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class position_t(object):
-    __slots__ = ["utime", "xyzrph", "xyzrph_cov", "xyzrph_dot"]
+class vector3_t(object):
+    __slots__ = ["x", "y", "z"]
 
-    __typenames__ = ["int64_t", "double", "double", "double"]
+    __typenames__ = ["double", "double", "double"]
 
-    __dimensions__ = [None, [6], [36], [6]]
+    __dimensions__ = [None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.xyzrph = [ 0.0 for dim0 in range(6) ]
-        self.xyzrph_cov = [ 0.0 for dim0 in range(36) ]
-        self.xyzrph_dot = [ 0.0 for dim0 in range(6) ]
+        self.x = 0.0
+        self.y = 0.0
+        self.z = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(position_t._get_packed_fingerprint())
+        buf.write(vector3_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">q", self.utime))
-        buf.write(struct.pack('>6d', *self.xyzrph[:6]))
-        buf.write(struct.pack('>36d', *self.xyzrph_cov[:36]))
-        buf.write(struct.pack('>6d', *self.xyzrph_dot[:6]))
+        buf.write(struct.pack(">ddd", self.x, self.y, self.z))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != position_t._get_packed_fingerprint():
+        if buf.read(8) != vector3_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return position_t._decode_one(buf)
+        return vector3_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = position_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.xyzrph = struct.unpack('>6d', buf.read(48))
-        self.xyzrph_cov = struct.unpack('>36d', buf.read(288))
-        self.xyzrph_dot = struct.unpack('>6d', buf.read(48))
+        self = vector3_t()
+        self.x, self.y, self.z = struct.unpack(">ddd", buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if position_t in parents: return 0
-        tmphash = (0x102e605ad0830a12) & 0xffffffffffffffff
+        if vector3_t in parents: return 0
+        tmphash = (0x573f2fdd2f76508f) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if position_t._packed_fingerprint is None:
-            position_t._packed_fingerprint = struct.pack(">Q", position_t._get_hash_recursive([]))
-        return position_t._packed_fingerprint
+        if vector3_t._packed_fingerprint is None:
+            vector3_t._packed_fingerprint = struct.pack(">Q", vector3_t._get_hash_recursive([]))
+        return vector3_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", position_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", vector3_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/navlcm/uuv_state_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/uuv_state_t.py`

 * *Files identical despite different names*

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/oi/double_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/sig_double_t.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class double_t(object):
+class sig_double_t(object):
     __slots__ = ["name", "value"]
 
     __typenames__ = ["string", "double"]
 
     __dimensions__ = [None, None]
 
     def __init__(self):
         self.name = ""
         self.value = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(double_t._get_packed_fingerprint())
+        buf.write(sig_double_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
         __name_encoded = self.name.encode('utf-8')
         buf.write(struct.pack('>I', len(__name_encoded)+1))
         buf.write(__name_encoded)
@@ -34,38 +34,38 @@
         buf.write(struct.pack(">d", self.value))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != double_t._get_packed_fingerprint():
+        if buf.read(8) != sig_double_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return double_t._decode_one(buf)
+        return sig_double_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = double_t()
+        self = sig_double_t()
         __name_len = struct.unpack('>I', buf.read(4))[0]
         self.name = buf.read(__name_len)[:-1].decode('utf-8', 'replace')
         self.value = struct.unpack(">d", buf.read(8))[0]
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if double_t in parents: return 0
+        if sig_double_t in parents: return 0
         tmphash = (0x753ddee2f1cd978f) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if double_t._packed_fingerprint is None:
-            double_t._packed_fingerprint = struct.pack(">Q", double_t._get_hash_recursive([]))
-        return double_t._packed_fingerprint
+        if sig_double_t._packed_fingerprint is None:
+            sig_double_t._packed_fingerprint = struct.pack(">Q", sig_double_t._get_hash_recursive([]))
+        return sig_double_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", double_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", sig_double_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/oi/kearfott_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/generic_t.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,104 +5,111 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-import compas_lcmtypes.oi.double_t
+import compas_lcmtypes.senlcm.sig_bool_t
 
-class kearfott_t(object):
-    __slots__ = ["time_unix_sec", "count_publish", "sender_id", "cycles_uint", "mode", "monitor", "latitude_rad", "longitude_rad", "northing_m", "easting_m", "depth_m", "bheight_m", "roll_rad", "pitch_rad", "heading_rad", "vbodyx_ms", "vbodyy_ms", "vbodyz_ms", "accelx_ms2", "accely_ms2", "accelz_ms2", "prate_rads", "qrate_rads", "rrate_rads", "utcTime", "sampleTime", "num_doubles", "doubles"]
+import compas_lcmtypes.senlcm.sig_double_t
 
-    __typenames__ = ["double", "int64_t", "string", "int16_t", "byte", "byte", "double", "double", "double", "double", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "float", "int16_t", "compas_lcmtypes.oi.double_t"]
+import compas_lcmtypes.senlcm.sig_long_t
 
-    __dimensions__ = [None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, None, ["num_doubles"]]
+class generic_t(object):
+    __slots__ = ["publisher", "timestamp", "sentence", "num_doubles", "sig_doubles", "num_long", "sig_longs", "num_bools", "sig_bools"]
+
+    __typenames__ = ["string", "double", "string", "int16_t", "compas_lcmtypes.senlcm.sig_double_t", "int16_t", "compas_lcmtypes.senlcm.sig_long_t", "int16_t", "compas_lcmtypes.senlcm.sig_bool_t"]
+
+    __dimensions__ = [None, None, None, None, ["num_doubles"], None, ["num_long"], None, ["num_bools"]]
 
     def __init__(self):
-        self.time_unix_sec = 0.0
-        self.count_publish = 0
-        self.sender_id = ""
-        self.cycles_uint = 0
-        self.mode = 0
-        self.monitor = 0
-        self.latitude_rad = 0.0
-        self.longitude_rad = 0.0
-        self.northing_m = 0.0
-        self.easting_m = 0.0
-        self.depth_m = 0.0
-        self.bheight_m = 0.0
-        self.roll_rad = 0.0
-        self.pitch_rad = 0.0
-        self.heading_rad = 0.0
-        self.vbodyx_ms = 0.0
-        self.vbodyy_ms = 0.0
-        self.vbodyz_ms = 0.0
-        self.accelx_ms2 = 0.0
-        self.accely_ms2 = 0.0
-        self.accelz_ms2 = 0.0
-        self.prate_rads = 0.0
-        self.qrate_rads = 0.0
-        self.rrate_rads = 0.0
-        self.utcTime = 0.0
-        self.sampleTime = 0.0
+        self.publisher = ""
+        self.timestamp = 0.0
+        self.sentence = ""
         self.num_doubles = 0
-        self.doubles = []
+        self.sig_doubles = []
+        self.num_long = 0
+        self.sig_longs = []
+        self.num_bools = 0
+        self.sig_bools = []
 
     def encode(self):
         buf = BytesIO()
-        buf.write(kearfott_t._get_packed_fingerprint())
+        buf.write(generic_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">dq", self.time_unix_sec, self.count_publish))
-        __sender_id_encoded = self.sender_id.encode('utf-8')
-        buf.write(struct.pack('>I', len(__sender_id_encoded)+1))
-        buf.write(__sender_id_encoded)
+        __publisher_encoded = self.publisher.encode('utf-8')
+        buf.write(struct.pack('>I', len(__publisher_encoded)+1))
+        buf.write(__publisher_encoded)
+        buf.write(b"\0")
+        buf.write(struct.pack(">d", self.timestamp))
+        __sentence_encoded = self.sentence.encode('utf-8')
+        buf.write(struct.pack('>I', len(__sentence_encoded)+1))
+        buf.write(__sentence_encoded)
         buf.write(b"\0")
-        buf.write(struct.pack(">hBBddddffffffffffffffffh", self.cycles_uint, self.mode, self.monitor, self.latitude_rad, self.longitude_rad, self.northing_m, self.easting_m, self.depth_m, self.bheight_m, self.roll_rad, self.pitch_rad, self.heading_rad, self.vbodyx_ms, self.vbodyy_ms, self.vbodyz_ms, self.accelx_ms2, self.accely_ms2, self.accelz_ms2, self.prate_rads, self.qrate_rads, self.rrate_rads, self.utcTime, self.sampleTime, self.num_doubles))
+        buf.write(struct.pack(">h", self.num_doubles))
         for i0 in range(self.num_doubles):
-            assert self.doubles[i0]._get_packed_fingerprint() == compas_lcmtypes.oi.double_t._get_packed_fingerprint()
-            self.doubles[i0]._encode_one(buf)
+            assert self.sig_doubles[i0]._get_packed_fingerprint() == compas_lcmtypes.senlcm.sig_double_t._get_packed_fingerprint()
+            self.sig_doubles[i0]._encode_one(buf)
+        buf.write(struct.pack(">h", self.num_long))
+        for i0 in range(self.num_long):
+            assert self.sig_longs[i0]._get_packed_fingerprint() == compas_lcmtypes.senlcm.sig_long_t._get_packed_fingerprint()
+            self.sig_longs[i0]._encode_one(buf)
+        buf.write(struct.pack(">h", self.num_bools))
+        for i0 in range(self.num_bools):
+            assert self.sig_bools[i0]._get_packed_fingerprint() == compas_lcmtypes.senlcm.sig_bool_t._get_packed_fingerprint()
+            self.sig_bools[i0]._encode_one(buf)
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != kearfott_t._get_packed_fingerprint():
+        if buf.read(8) != generic_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return kearfott_t._decode_one(buf)
+        return generic_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = kearfott_t()
-        self.time_unix_sec, self.count_publish = struct.unpack(">dq", buf.read(16))
-        __sender_id_len = struct.unpack('>I', buf.read(4))[0]
-        self.sender_id = buf.read(__sender_id_len)[:-1].decode('utf-8', 'replace')
-        self.cycles_uint, self.mode, self.monitor, self.latitude_rad, self.longitude_rad, self.northing_m, self.easting_m, self.depth_m, self.bheight_m, self.roll_rad, self.pitch_rad, self.heading_rad, self.vbodyx_ms, self.vbodyy_ms, self.vbodyz_ms, self.accelx_ms2, self.accely_ms2, self.accelz_ms2, self.prate_rads, self.qrate_rads, self.rrate_rads, self.utcTime, self.sampleTime, self.num_doubles = struct.unpack(">hBBddddffffffffffffffffh", buf.read(102))
-        self.doubles = []
+        self = generic_t()
+        __publisher_len = struct.unpack('>I', buf.read(4))[0]
+        self.publisher = buf.read(__publisher_len)[:-1].decode('utf-8', 'replace')
+        self.timestamp = struct.unpack(">d", buf.read(8))[0]
+        __sentence_len = struct.unpack('>I', buf.read(4))[0]
+        self.sentence = buf.read(__sentence_len)[:-1].decode('utf-8', 'replace')
+        self.num_doubles = struct.unpack(">h", buf.read(2))[0]
+        self.sig_doubles = []
         for i0 in range(self.num_doubles):
-            self.doubles.append(compas_lcmtypes.oi.double_t._decode_one(buf))
+            self.sig_doubles.append(compas_lcmtypes.senlcm.sig_double_t._decode_one(buf))
+        self.num_long = struct.unpack(">h", buf.read(2))[0]
+        self.sig_longs = []
+        for i0 in range(self.num_long):
+            self.sig_longs.append(compas_lcmtypes.senlcm.sig_long_t._decode_one(buf))
+        self.num_bools = struct.unpack(">h", buf.read(2))[0]
+        self.sig_bools = []
+        for i0 in range(self.num_bools):
+            self.sig_bools.append(compas_lcmtypes.senlcm.sig_bool_t._decode_one(buf))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if kearfott_t in parents: return 0
-        newparents = parents + [kearfott_t]
-        tmphash = (0xb3fe10b7f94bb7a6+ compas_lcmtypes.oi.double_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
+        if generic_t in parents: return 0
+        newparents = parents + [generic_t]
+        tmphash = (0x1f28d7454bcebb69+ compas_lcmtypes.senlcm.sig_double_t._get_hash_recursive(newparents)+ compas_lcmtypes.senlcm.sig_long_t._get_hash_recursive(newparents)+ compas_lcmtypes.senlcm.sig_bool_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if kearfott_t._packed_fingerprint is None:
-            kearfott_t._packed_fingerprint = struct.pack(">Q", kearfott_t._get_hash_recursive([]))
-        return kearfott_t._packed_fingerprint
+        if generic_t._packed_fingerprint is None:
+            generic_t._packed_fingerprint = struct.pack(">Q", generic_t._get_hash_recursive([]))
+        return generic_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", kearfott_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", generic_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/bno055_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/battery_t.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,84 +5,70 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class bno055_t(object):
-    __slots__ = ["utime", "rph", "quaternion", "angRate", "accel", "magField", "gravity", "lin_accel", "temperature"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "double", "double", "double", "double", "double", "double", "double", "double"]
+class battery_t(object):
+    __slots__ = ["header", "voltage", "temperature", "current", "charge"]
 
-    __dimensions__ = [None, [3], [4], [3], [3], [3], [3], [3], None]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double", "double", "double"]
+
+    __dimensions__ = [None, None, None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.rph = [ 0.0 for dim0 in range(3) ]
-        self.quaternion = [ 0.0 for dim0 in range(4) ]
-        self.angRate = [ 0.0 for dim0 in range(3) ]
-        self.accel = [ 0.0 for dim0 in range(3) ]
-        self.magField = [ 0.0 for dim0 in range(3) ]
-        self.gravity = [ 0.0 for dim0 in range(3) ]
-        self.lin_accel = [ 0.0 for dim0 in range(3) ]
+        self.header = compas_lcmtypes.standard.header_t()
+        self.voltage = 0.0
         self.temperature = 0.0
+        self.current = 0.0
+        self.charge = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(bno055_t._get_packed_fingerprint())
+        buf.write(battery_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">q", self.utime))
-        buf.write(struct.pack('>3d', *self.rph[:3]))
-        buf.write(struct.pack('>4d', *self.quaternion[:4]))
-        buf.write(struct.pack('>3d', *self.angRate[:3]))
-        buf.write(struct.pack('>3d', *self.accel[:3]))
-        buf.write(struct.pack('>3d', *self.magField[:3]))
-        buf.write(struct.pack('>3d', *self.gravity[:3]))
-        buf.write(struct.pack('>3d', *self.lin_accel[:3]))
-        buf.write(struct.pack(">d", self.temperature))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">dddd", self.voltage, self.temperature, self.current, self.charge))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != bno055_t._get_packed_fingerprint():
+        if buf.read(8) != battery_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return bno055_t._decode_one(buf)
+        return battery_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = bno055_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.rph = struct.unpack('>3d', buf.read(24))
-        self.quaternion = struct.unpack('>4d', buf.read(32))
-        self.angRate = struct.unpack('>3d', buf.read(24))
-        self.accel = struct.unpack('>3d', buf.read(24))
-        self.magField = struct.unpack('>3d', buf.read(24))
-        self.gravity = struct.unpack('>3d', buf.read(24))
-        self.lin_accel = struct.unpack('>3d', buf.read(24))
-        self.temperature = struct.unpack(">d", buf.read(8))[0]
+        self = battery_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.voltage, self.temperature, self.current, self.charge = struct.unpack(">dddd", buf.read(32))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if bno055_t in parents: return 0
-        tmphash = (0xb95bfc2151bb1f23) & 0xffffffffffffffff
+        if battery_t in parents: return 0
+        newparents = parents + [battery_t]
+        tmphash = (0x8ebb4d983630afcf+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if bno055_t._packed_fingerprint is None:
-            bno055_t._packed_fingerprint = struct.pack(">Q", bno055_t._get_hash_recursive([]))
-        return bno055_t._packed_fingerprint
+        if battery_t._packed_fingerprint is None:
+            battery_t._packed_fingerprint = struct.pack(">Q", battery_t._get_hash_recursive([]))
+        return battery_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", bno055_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", battery_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/cmd_list_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/sig_bool_t.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,64 +5,67 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class cmd_list_t(object):
-    __slots__ = ["utime", "len", "commands"]
+class sig_bool_t(object):
+    __slots__ = ["name", "value"]
 
-    __typenames__ = ["int64_t", "int32_t", "double"]
+    __typenames__ = ["string", "boolean"]
 
-    __dimensions__ = [None, None, ["len"]]
+    __dimensions__ = [None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.len = 0
-        self.commands = []
+        self.name = ""
+        self.value = False
 
     def encode(self):
         buf = BytesIO()
-        buf.write(cmd_list_t._get_packed_fingerprint())
+        buf.write(sig_bool_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qi", self.utime, self.len))
-        buf.write(struct.pack('>%dd' % self.len, *self.commands[:self.len]))
+        __name_encoded = self.name.encode('utf-8')
+        buf.write(struct.pack('>I', len(__name_encoded)+1))
+        buf.write(__name_encoded)
+        buf.write(b"\0")
+        buf.write(struct.pack(">b", self.value))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != cmd_list_t._get_packed_fingerprint():
+        if buf.read(8) != sig_bool_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return cmd_list_t._decode_one(buf)
+        return sig_bool_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = cmd_list_t()
-        self.utime, self.len = struct.unpack(">qi", buf.read(12))
-        self.commands = struct.unpack('>%dd' % self.len, buf.read(self.len * 8))
+        self = sig_bool_t()
+        __name_len = struct.unpack('>I', buf.read(4))[0]
+        self.name = buf.read(__name_len)[:-1].decode('utf-8', 'replace')
+        self.value = bool(struct.unpack('b', buf.read(1))[0])
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if cmd_list_t in parents: return 0
-        tmphash = (0xa04d56805e537ee1) & 0xffffffffffffffff
+        if sig_bool_t in parents: return 0
+        tmphash = (0x3bdedce7d49bfde8) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if cmd_list_t._packed_fingerprint is None:
-            cmd_list_t._packed_fingerprint = struct.pack(">Q", cmd_list_t._get_hash_recursive([]))
-        return cmd_list_t._packed_fingerprint
+        if sig_bool_t._packed_fingerprint is None:
+            sig_bool_t._packed_fingerprint = struct.pack(">Q", sig_bool_t._get_hash_recursive([]))
+        return sig_bool_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", cmd_list_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", sig_bool_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/cmd_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/standard/header_t.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,63 +5,68 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class cmd_t(object):
-    __slots__ = ["utime", "force"]
+class header_t(object):
+    __slots__ = ["sequence", "timestamp", "frame_id"]
 
-    __typenames__ = ["int64_t", "double"]
+    __typenames__ = ["int32_t", "int64_t", "string"]
 
-    __dimensions__ = [None, [6]]
+    __dimensions__ = [None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.force = [ 0.0 for dim0 in range(6) ]
+        self.sequence = 0
+        self.timestamp = 0
+        self.frame_id = ""
 
     def encode(self):
         buf = BytesIO()
-        buf.write(cmd_t._get_packed_fingerprint())
+        buf.write(header_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">q", self.utime))
-        buf.write(struct.pack('>6d', *self.force[:6]))
+        buf.write(struct.pack(">iq", self.sequence, self.timestamp))
+        __frame_id_encoded = self.frame_id.encode('utf-8')
+        buf.write(struct.pack('>I', len(__frame_id_encoded)+1))
+        buf.write(__frame_id_encoded)
+        buf.write(b"\0")
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != cmd_t._get_packed_fingerprint():
+        if buf.read(8) != header_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return cmd_t._decode_one(buf)
+        return header_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = cmd_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.force = struct.unpack('>6d', buf.read(48))
+        self = header_t()
+        self.sequence, self.timestamp = struct.unpack(">iq", buf.read(12))
+        __frame_id_len = struct.unpack('>I', buf.read(4))[0]
+        self.frame_id = buf.read(__frame_id_len)[:-1].decode('utf-8', 'replace')
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if cmd_t in parents: return 0
-        tmphash = (0x27bd3380bfaa6b62) & 0xffffffffffffffff
+        if header_t in parents: return 0
+        tmphash = (0xa2111e7853888e66) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if cmd_t._packed_fingerprint is None:
-            cmd_t._packed_fingerprint = struct.pack(">Q", cmd_t._get_hash_recursive([]))
-        return cmd_t._packed_fingerprint
+        if header_t._packed_fingerprint is None:
+            header_t._packed_fingerprint = struct.pack(">Q", header_t._get_hash_recursive([]))
+        return header_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", cmd_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", header_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/depth_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/depth_t.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,54 +5,60 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
+import compas_lcmtypes.standard.header_t
+
 class depth_t(object):
-    __slots__ = ["utime", "depth", "pressure"]
+    __slots__ = ["header", "depth", "pressure"]
 
-    __typenames__ = ["int64_t", "double", "double"]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double"]
 
     __dimensions__ = [None, None, None]
 
     def __init__(self):
-        self.utime = 0
+        self.header = compas_lcmtypes.standard.header_t()
         self.depth = 0.0
         self.pressure = 0.0
 
     def encode(self):
         buf = BytesIO()
         buf.write(depth_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qdd", self.utime, self.depth, self.pressure))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">dd", self.depth, self.pressure))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
         if buf.read(8) != depth_t._get_packed_fingerprint():
             raise ValueError("Decode error")
         return depth_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
         self = depth_t()
-        self.utime, self.depth, self.pressure = struct.unpack(">qdd", buf.read(24))
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.depth, self.pressure = struct.unpack(">dd", buf.read(16))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
         if depth_t in parents: return 0
-        tmphash = (0xaed8e9fe70fca694) & 0xffffffffffffffff
+        newparents = parents + [depth_t]
+        tmphash = (0x16e44850c90dda6a+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
         if depth_t._packed_fingerprint is None:
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/enable_cmd_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/geometry/quaternion_t.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class enable_cmd_t(object):
-    __slots__ = ["utime", "enable_id", "enable_status"]
+class quaternion_t(object):
+    __slots__ = ["x", "y", "z", "w"]
 
-    __typenames__ = ["int64_t", "int16_t", "boolean"]
+    __typenames__ = ["double", "double", "double", "double"]
 
-    __dimensions__ = [None, None, None]
+    __dimensions__ = [None, None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.enable_id = 0
-        self.enable_status = False
+        self.x = 0.0
+        self.y = 0.0
+        self.z = 0.0
+        self.w = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(enable_cmd_t._get_packed_fingerprint())
+        buf.write(quaternion_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qhb", self.utime, self.enable_id, self.enable_status))
+        buf.write(struct.pack(">dddd", self.x, self.y, self.z, self.w))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != enable_cmd_t._get_packed_fingerprint():
+        if buf.read(8) != quaternion_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return enable_cmd_t._decode_one(buf)
+        return quaternion_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = enable_cmd_t()
-        self.utime, self.enable_id = struct.unpack(">qh", buf.read(10))
-        self.enable_status = bool(struct.unpack('b', buf.read(1))[0])
+        self = quaternion_t()
+        self.x, self.y, self.z, self.w = struct.unpack(">dddd", buf.read(32))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if enable_cmd_t in parents: return 0
-        tmphash = (0xe27d91846bae88bb) & 0xffffffffffffffff
+        if quaternion_t in parents: return 0
+        tmphash = (0x9b1dee9dfc8c0515) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if enable_cmd_t._packed_fingerprint is None:
-            enable_cmd_t._packed_fingerprint = struct.pack(">Q", enable_cmd_t._get_hash_recursive([]))
-        return enable_cmd_t._packed_fingerprint
+        if quaternion_t._packed_fingerprint is None:
+            quaternion_t._packed_fingerprint = struct.pack(">Q", quaternion_t._get_hash_recursive([]))
+        return quaternion_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", enable_cmd_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", quaternion_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/image_depth.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/twist_t.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,68 +5,73 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class image_depth(object):
-    __slots__ = ["utime", "width", "height", "range_min", "range", "image_size", "image"]
+import compas_lcmtypes.geometry.twist_t
 
-    __typenames__ = ["int64_t", "int32_t", "int32_t", "double", "double", "int32_t", "float"]
+import compas_lcmtypes.standard.header_t
 
-    __dimensions__ = [None, None, None, None, None, None, ["image_size"]]
+class twist_t(object):
+    __slots__ = ["header", "twist", "twist_covariance"]
+
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "compas_lcmtypes.geometry.twist_t", "double"]
+
+    __dimensions__ = [None, None, [36]]
 
     def __init__(self):
-        self.utime = 0
-        self.width = 0
-        self.height = 0
-        self.range_min = 0.0
-        self.range = 0.0
-        self.image_size = 0
-        self.image = []
+        self.header = compas_lcmtypes.standard.header_t()
+        self.twist = compas_lcmtypes.geometry.twist_t()
+        self.twist_covariance = [ 0.0 for dim0 in range(36) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(image_depth._get_packed_fingerprint())
+        buf.write(twist_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qiiddi", self.utime, self.width, self.height, self.range_min, self.range, self.image_size))
-        buf.write(struct.pack('>%df' % self.image_size, *self.image[:self.image_size]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        assert self.twist._get_packed_fingerprint() == compas_lcmtypes.geometry.twist_t._get_packed_fingerprint()
+        self.twist._encode_one(buf)
+        buf.write(struct.pack('>36d', *self.twist_covariance[:36]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != image_depth._get_packed_fingerprint():
+        if buf.read(8) != twist_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return image_depth._decode_one(buf)
+        return twist_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = image_depth()
-        self.utime, self.width, self.height, self.range_min, self.range, self.image_size = struct.unpack(">qiiddi", buf.read(36))
-        self.image = struct.unpack('>%df' % self.image_size, buf.read(self.image_size * 4))
+        self = twist_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.twist = compas_lcmtypes.geometry.twist_t._decode_one(buf)
+        self.twist_covariance = struct.unpack('>36d', buf.read(288))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if image_depth in parents: return 0
-        tmphash = (0xc1013eeae586c7ae) & 0xffffffffffffffff
+        if twist_t in parents: return 0
+        newparents = parents + [twist_t]
+        tmphash = (0x8807c70766588d61+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)+ compas_lcmtypes.geometry.twist_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if image_depth._packed_fingerprint is None:
-            image_depth._packed_fingerprint = struct.pack(">Q", image_depth._get_hash_recursive([]))
-        return image_depth._packed_fingerprint
+        if twist_t._packed_fingerprint is None:
+            twist_t._packed_fingerprint = struct.pack(">Q", twist_t._get_hash_recursive([]))
+        return twist_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", image_depth._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", twist_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/image_float32.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/geometry/twist_t.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,66 +5,68 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class image_float32(object):
-    __slots__ = ["utime", "width", "height", "image_size", "image"]
+import compas_lcmtypes.geometry.vector3_t
 
-    __typenames__ = ["int64_t", "int32_t", "int32_t", "int32_t", "float"]
+class twist_t(object):
+    __slots__ = ["linear", "angular"]
 
-    __dimensions__ = [None, None, None, None, ["image_size"]]
+    __typenames__ = ["compas_lcmtypes.geometry.vector3_t", "compas_lcmtypes.geometry.vector3_t"]
+
+    __dimensions__ = [None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.width = 0
-        self.height = 0
-        self.image_size = 0
-        self.image = []
+        self.linear = compas_lcmtypes.geometry.vector3_t()
+        self.angular = compas_lcmtypes.geometry.vector3_t()
 
     def encode(self):
         buf = BytesIO()
-        buf.write(image_float32._get_packed_fingerprint())
+        buf.write(twist_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qiii", self.utime, self.width, self.height, self.image_size))
-        buf.write(struct.pack('>%df' % self.image_size, *self.image[:self.image_size]))
+        assert self.linear._get_packed_fingerprint() == compas_lcmtypes.geometry.vector3_t._get_packed_fingerprint()
+        self.linear._encode_one(buf)
+        assert self.angular._get_packed_fingerprint() == compas_lcmtypes.geometry.vector3_t._get_packed_fingerprint()
+        self.angular._encode_one(buf)
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != image_float32._get_packed_fingerprint():
+        if buf.read(8) != twist_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return image_float32._decode_one(buf)
+        return twist_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = image_float32()
-        self.utime, self.width, self.height, self.image_size = struct.unpack(">qiii", buf.read(20))
-        self.image = struct.unpack('>%df' % self.image_size, buf.read(self.image_size * 4))
+        self = twist_t()
+        self.linear = compas_lcmtypes.geometry.vector3_t._decode_one(buf)
+        self.angular = compas_lcmtypes.geometry.vector3_t._decode_one(buf)
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if image_float32 in parents: return 0
-        tmphash = (0xbff98dd17a1f119e) & 0xffffffffffffffff
+        if twist_t in parents: return 0
+        newparents = parents + [twist_t]
+        tmphash = (0x3a4144772922add7+ compas_lcmtypes.geometry.vector3_t._get_hash_recursive(newparents)+ compas_lcmtypes.geometry.vector3_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if image_float32._packed_fingerprint is None:
-            image_float32._packed_fingerprint = struct.pack(">Q", image_float32._get_hash_recursive([]))
-        return image_float32._packed_fingerprint
+        if twist_t._packed_fingerprint is None:
+            twist_t._packed_fingerprint = struct.pack(">Q", twist_t._get_hash_recursive([]))
+        return twist_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", image_float32._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", twist_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/imu_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/geometry/point_t.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,75 +5,62 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class imu_t(object):
-    __slots__ = ["utime", "rph", "angRate", "xyz_ddot", "flags"]
+class point_t(object):
+    __slots__ = ["x", "y", "z"]
 
-    __typenames__ = ["int64_t", "double", "double", "double", "int16_t"]
+    __typenames__ = ["double", "double", "double"]
 
-    __dimensions__ = [None, [3], [3], [3], None]
-
-    FLAG_NEW_MEASUREMENT = 1
-    FLAG_OLD_MEASUREMENT = 0
+    __dimensions__ = [None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.rph = [ 0.0 for dim0 in range(3) ]
-        self.angRate = [ 0.0 for dim0 in range(3) ]
-        self.xyz_ddot = [ 0.0 for dim0 in range(3) ]
-        self.flags = 0
+        self.x = 0.0
+        self.y = 0.0
+        self.z = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(imu_t._get_packed_fingerprint())
+        buf.write(point_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">q", self.utime))
-        buf.write(struct.pack('>3d', *self.rph[:3]))
-        buf.write(struct.pack('>3d', *self.angRate[:3]))
-        buf.write(struct.pack('>3d', *self.xyz_ddot[:3]))
-        buf.write(struct.pack(">h", self.flags))
+        buf.write(struct.pack(">ddd", self.x, self.y, self.z))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != imu_t._get_packed_fingerprint():
+        if buf.read(8) != point_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return imu_t._decode_one(buf)
+        return point_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = imu_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.rph = struct.unpack('>3d', buf.read(24))
-        self.angRate = struct.unpack('>3d', buf.read(24))
-        self.xyz_ddot = struct.unpack('>3d', buf.read(24))
-        self.flags = struct.unpack(">h", buf.read(2))[0]
+        self = point_t()
+        self.x, self.y, self.z = struct.unpack(">ddd", buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if imu_t in parents: return 0
-        tmphash = (0xc6be45f481db0d58) & 0xffffffffffffffff
+        if point_t in parents: return 0
+        tmphash = (0x573f2fdd2f76508f) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if imu_t._packed_fingerprint is None:
-            imu_t._packed_fingerprint = struct.pack(">Q", imu_t._get_hash_recursive([]))
-        return imu_t._packed_fingerprint
+        if point_t._packed_fingerprint is None:
+            point_t._packed_fingerprint = struct.pack(">Q", point_t._get_hash_recursive([]))
+        return point_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", imu_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", point_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/joystick_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/gamepad_t.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class joystick_t(object):
-    __slots__ = ["utime", "button_a", "button_b", "button_x", "button_y", "button_select", "button_start", "button_trigger_r", "button_trigger_l", "axis_r", "axis_l", "trigger_r", "trigger_l", "hats"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "boolean", "boolean", "boolean", "boolean", "boolean", "boolean", "boolean", "boolean", "double", "double", "double", "double", "double"]
+class gamepad_t(object):
+    __slots__ = ["header", "button_a", "button_b", "button_x", "button_y", "button_select", "button_start", "button_trigger_r", "button_trigger_l", "axis_r", "axis_l", "trigger_r", "trigger_l", "hats"]
+
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "boolean", "boolean", "boolean", "boolean", "boolean", "boolean", "boolean", "boolean", "double", "double", "double", "double", "double"]
 
     __dimensions__ = [None, None, None, None, None, None, None, None, None, [2], [2], None, None, [2]]
 
     def __init__(self):
-        self.utime = 0
+        self.header = compas_lcmtypes.standard.header_t()
         self.button_a = False
         self.button_b = False
         self.button_x = False
         self.button_y = False
         self.button_select = False
         self.button_start = False
         self.button_trigger_r = False
@@ -30,38 +32,40 @@
         self.axis_l = [ 0.0 for dim0 in range(2) ]
         self.trigger_r = 0.0
         self.trigger_l = 0.0
         self.hats = [ 0.0 for dim0 in range(2) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(joystick_t._get_packed_fingerprint())
+        buf.write(gamepad_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qbbbbbbbb", self.utime, self.button_a, self.button_b, self.button_x, self.button_y, self.button_select, self.button_start, self.button_trigger_r, self.button_trigger_l))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">bbbbbbbb", self.button_a, self.button_b, self.button_x, self.button_y, self.button_select, self.button_start, self.button_trigger_r, self.button_trigger_l))
         buf.write(struct.pack('>2d', *self.axis_r[:2]))
         buf.write(struct.pack('>2d', *self.axis_l[:2]))
         buf.write(struct.pack(">dd", self.trigger_r, self.trigger_l))
         buf.write(struct.pack('>2d', *self.hats[:2]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != joystick_t._get_packed_fingerprint():
+        if buf.read(8) != gamepad_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return joystick_t._decode_one(buf)
+        return gamepad_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = joystick_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
+        self = gamepad_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
         self.button_a = bool(struct.unpack('b', buf.read(1))[0])
         self.button_b = bool(struct.unpack('b', buf.read(1))[0])
         self.button_x = bool(struct.unpack('b', buf.read(1))[0])
         self.button_y = bool(struct.unpack('b', buf.read(1))[0])
         self.button_select = bool(struct.unpack('b', buf.read(1))[0])
         self.button_start = bool(struct.unpack('b', buf.read(1))[0])
         self.button_trigger_r = bool(struct.unpack('b', buf.read(1))[0])
@@ -70,24 +74,25 @@
         self.axis_l = struct.unpack('>2d', buf.read(16))
         self.trigger_r, self.trigger_l = struct.unpack(">dd", buf.read(16))
         self.hats = struct.unpack('>2d', buf.read(16))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if joystick_t in parents: return 0
-        tmphash = (0xa80557971a4c037a) & 0xffffffffffffffff
+        if gamepad_t in parents: return 0
+        newparents = parents + [gamepad_t]
+        tmphash = (0xa2323731c07047db+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if joystick_t._packed_fingerprint is None:
-            joystick_t._packed_fingerprint = struct.pack(">Q", joystick_t._get_hash_recursive([]))
-        return joystick_t._packed_fingerprint
+        if gamepad_t._packed_fingerprint is None:
+            gamepad_t._packed_fingerprint = struct.pack(">Q", gamepad_t._get_hash_recursive([]))
+        return gamepad_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", joystick_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", gamepad_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/multibeam_polar_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/sig_long_t.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,73 +5,67 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class multibeam_polar_t(object):
-    __slots__ = ["utime", "npoints", "quality", "data"]
+class sig_long_t(object):
+    __slots__ = ["name", "value"]
 
-    __typenames__ = ["int64_t", "int32_t", "int32_t", "double"]
+    __typenames__ = ["string", "int32_t"]
 
-    __dimensions__ = [None, None, ["npoints"], ["npoints", 2]]
-
-    QUALITY_INVALID = 0
-    QUALITY_VALID = 1
+    __dimensions__ = [None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.npoints = 0
-        self.quality = []
-        self.data = []
+        self.name = ""
+        self.value = 0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(multibeam_polar_t._get_packed_fingerprint())
+        buf.write(sig_long_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qi", self.utime, self.npoints))
-        buf.write(struct.pack('>%di' % self.npoints, *self.quality[:self.npoints]))
-        for i0 in range(self.npoints):
-            buf.write(struct.pack('>2d', *self.data[i0][:2]))
+        __name_encoded = self.name.encode('utf-8')
+        buf.write(struct.pack('>I', len(__name_encoded)+1))
+        buf.write(__name_encoded)
+        buf.write(b"\0")
+        buf.write(struct.pack(">i", self.value))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != multibeam_polar_t._get_packed_fingerprint():
+        if buf.read(8) != sig_long_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return multibeam_polar_t._decode_one(buf)
+        return sig_long_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = multibeam_polar_t()
-        self.utime, self.npoints = struct.unpack(">qi", buf.read(12))
-        self.quality = struct.unpack('>%di' % self.npoints, buf.read(self.npoints * 4))
-        self.data = []
-        for i0 in range(self.npoints):
-            self.data.append(struct.unpack('>2d', buf.read(16)))
+        self = sig_long_t()
+        __name_len = struct.unpack('>I', buf.read(4))[0]
+        self.name = buf.read(__name_len)[:-1].decode('utf-8', 'replace')
+        self.value = struct.unpack(">i", buf.read(4))[0]
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if multibeam_polar_t in parents: return 0
-        tmphash = (0x609531075d71a838) & 0xffffffffffffffff
+        if sig_long_t in parents: return 0
+        tmphash = (0x42dfe221079e03e8) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if multibeam_polar_t._packed_fingerprint is None:
-            multibeam_polar_t._packed_fingerprint = struct.pack(">Q", multibeam_polar_t._get_hash_recursive([]))
-        return multibeam_polar_t._packed_fingerprint
+        if sig_long_t._packed_fingerprint is None:
+            sig_long_t._packed_fingerprint = struct.pack(">Q", sig_long_t._get_hash_recursive([]))
+        return sig_long_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", multibeam_polar_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", sig_long_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/multibeam_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/multibeam_t.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,57 +5,63 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
+import compas_lcmtypes.standard.header_t
+
 class multibeam_t(object):
-    __slots__ = ["utime", "n_pings", "angle_range", "pings"]
+    __slots__ = ["header", "n_pings", "angle_range", "pings"]
 
-    __typenames__ = ["int64_t", "int16_t", "double", "double"]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "int16_t", "double", "double"]
 
     __dimensions__ = [None, None, None, ["n_pings"]]
 
     def __init__(self):
-        self.utime = 0
+        self.header = compas_lcmtypes.standard.header_t()
         self.n_pings = 0
         self.angle_range = 0.0
         self.pings = []
 
     def encode(self):
         buf = BytesIO()
         buf.write(multibeam_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qhd", self.utime, self.n_pings, self.angle_range))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">hd", self.n_pings, self.angle_range))
         buf.write(struct.pack('>%dd' % self.n_pings, *self.pings[:self.n_pings]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
         if buf.read(8) != multibeam_t._get_packed_fingerprint():
             raise ValueError("Decode error")
         return multibeam_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
         self = multibeam_t()
-        self.utime, self.n_pings, self.angle_range = struct.unpack(">qhd", buf.read(18))
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.n_pings, self.angle_range = struct.unpack(">hd", buf.read(10))
         self.pings = struct.unpack('>%dd' % self.n_pings, buf.read(self.n_pings * 8))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
         if multibeam_t in parents: return 0
-        tmphash = (0x7eba7acc00ea708c) & 0xffffffffffffffff
+        newparents = parents + [multibeam_t]
+        tmphash = (0x7cad524b0e945351+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
         if multibeam_t._packed_fingerprint is None:
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/multibeam_xy_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/effort_cmd_t.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,73 +5,72 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class multibeam_xy_t(object):
-    __slots__ = ["utime", "npoints", "quality", "data"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "int32_t", "int32_t", "double"]
+class effort_cmd_t(object):
+    __slots__ = ["header", "x", "y", "z", "phi", "theta", "psi"]
 
-    __dimensions__ = [None, None, ["npoints"], ["npoints", 3]]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double", "double", "double", "double", "double"]
 
-    QUALITY_INVALID = 0
-    QUALITY_VALID = 1
+    __dimensions__ = [None, None, None, None, None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.npoints = 0
-        self.quality = []
-        self.data = []
+        self.header = compas_lcmtypes.standard.header_t()
+        self.x = 0.0
+        self.y = 0.0
+        self.z = 0.0
+        self.phi = 0.0
+        self.theta = 0.0
+        self.psi = 0.0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(multibeam_xy_t._get_packed_fingerprint())
+        buf.write(effort_cmd_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qi", self.utime, self.npoints))
-        buf.write(struct.pack('>%di' % self.npoints, *self.quality[:self.npoints]))
-        for i0 in range(self.npoints):
-            buf.write(struct.pack('>3d', *self.data[i0][:3]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">dddddd", self.x, self.y, self.z, self.phi, self.theta, self.psi))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != multibeam_xy_t._get_packed_fingerprint():
+        if buf.read(8) != effort_cmd_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return multibeam_xy_t._decode_one(buf)
+        return effort_cmd_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = multibeam_xy_t()
-        self.utime, self.npoints = struct.unpack(">qi", buf.read(12))
-        self.quality = struct.unpack('>%di' % self.npoints, buf.read(self.npoints * 4))
-        self.data = []
-        for i0 in range(self.npoints):
-            self.data.append(struct.unpack('>3d', buf.read(24)))
+        self = effort_cmd_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.x, self.y, self.z, self.phi, self.theta, self.psi = struct.unpack(">dddddd", buf.read(48))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if multibeam_xy_t in parents: return 0
-        tmphash = (0x609531075d71a839) & 0xffffffffffffffff
+        if effort_cmd_t in parents: return 0
+        newparents = parents + [effort_cmd_t]
+        tmphash = (0xba86a0c54fd80a1f+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if multibeam_xy_t._packed_fingerprint is None:
-            multibeam_xy_t._packed_fingerprint = struct.pack(">Q", multibeam_xy_t._get_hash_recursive([]))
-        return multibeam_xy_t._packed_fingerprint
+        if effort_cmd_t._packed_fingerprint is None:
+            effort_cmd_t._packed_fingerprint = struct.pack(">Q", effort_cmd_t._get_hash_recursive([]))
+        return effort_cmd_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", multibeam_xy_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", effort_cmd_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/oculus_sonar_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/cmd_list_t.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,70 +5,70 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class oculus_sonar_t(object):
-    __slots__ = ["utime", "nBeams", "nRanges", "range", "image_size", "image", "bearings"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "int32_t", "int32_t", "double", "int32_t", "byte", "int16_t"]
+class cmd_list_t(object):
+    __slots__ = ["header", "len", "commands"]
 
-    __dimensions__ = [None, None, None, None, None, ["image_size"], ["nBeams"]]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "int32_t", "double"]
+
+    __dimensions__ = [None, None, ["len"]]
 
     def __init__(self):
-        self.utime = 0
-        self.nBeams = 0
-        self.nRanges = 0
-        self.range = 0.0
-        self.image_size = 0
-        self.image = b""
-        self.bearings = []
+        self.header = compas_lcmtypes.standard.header_t()
+        self.len = 0
+        self.commands = []
 
     def encode(self):
         buf = BytesIO()
-        buf.write(oculus_sonar_t._get_packed_fingerprint())
+        buf.write(cmd_list_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qiidi", self.utime, self.nBeams, self.nRanges, self.range, self.image_size))
-        buf.write(bytearray(self.image[:self.image_size]))
-        buf.write(struct.pack('>%dh' % self.nBeams, *self.bearings[:self.nBeams]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">i", self.len))
+        buf.write(struct.pack('>%dd' % self.len, *self.commands[:self.len]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != oculus_sonar_t._get_packed_fingerprint():
+        if buf.read(8) != cmd_list_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return oculus_sonar_t._decode_one(buf)
+        return cmd_list_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = oculus_sonar_t()
-        self.utime, self.nBeams, self.nRanges, self.range, self.image_size = struct.unpack(">qiidi", buf.read(28))
-        self.image = buf.read(self.image_size)
-        self.bearings = struct.unpack('>%dh' % self.nBeams, buf.read(self.nBeams * 2))
+        self = cmd_list_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.len = struct.unpack(">i", buf.read(4))[0]
+        self.commands = struct.unpack('>%dd' % self.len, buf.read(self.len * 8))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if oculus_sonar_t in parents: return 0
-        tmphash = (0x826975d8961d653) & 0xffffffffffffffff
+        if cmd_list_t in parents: return 0
+        newparents = parents + [cmd_list_t]
+        tmphash = (0x119a6401e6709630+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if oculus_sonar_t._packed_fingerprint is None:
-            oculus_sonar_t._packed_fingerprint = struct.pack(">Q", oculus_sonar_t._get_hash_recursive([]))
-        return oculus_sonar_t._packed_fingerprint
+        if cmd_list_t._packed_fingerprint is None:
+            cmd_list_t._packed_fingerprint = struct.pack(">Q", cmd_list_t._get_hash_recursive([]))
+        return cmd_list_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", oculus_sonar_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", cmd_list_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/prosilica_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/rph_angrate_t.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,74 +5,70 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-import compas_lcmtypes.senlcm.prosilica_attribute_t
+import compas_lcmtypes.standard.header_t
 
-class prosilica_t(object):
-    __slots__ = ["utime", "self", "n_attributes", "PvAttributes"]
+class rph_angrate_t(object):
+    __slots__ = ["header", "rph", "angRate"]
 
-    __typenames__ = ["int64_t", "boolean", "int32_t", "compas_lcmtypes.senlcm.prosilica_attribute_t"]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double"]
 
-    __dimensions__ = [None, None, None, ["n_attributes"]]
+    __dimensions__ = [None, [3], [3]]
 
     def __init__(self):
-        self.utime = 0
-        self.self = False
-        self.n_attributes = 0
-        self.PvAttributes = []
+        self.header = compas_lcmtypes.standard.header_t()
+        self.rph = [ 0.0 for dim0 in range(3) ]
+        self.angRate = [ 0.0 for dim0 in range(3) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(prosilica_t._get_packed_fingerprint())
+        buf.write(rph_angrate_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qbi", self.utime, self.self, self.n_attributes))
-        for i0 in range(self.n_attributes):
-            assert self.PvAttributes[i0]._get_packed_fingerprint() == compas_lcmtypes.senlcm.prosilica_attribute_t._get_packed_fingerprint()
-            self.PvAttributes[i0]._encode_one(buf)
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack('>3d', *self.rph[:3]))
+        buf.write(struct.pack('>3d', *self.angRate[:3]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != prosilica_t._get_packed_fingerprint():
+        if buf.read(8) != rph_angrate_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return prosilica_t._decode_one(buf)
+        return rph_angrate_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = prosilica_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.self = bool(struct.unpack('b', buf.read(1))[0])
-        self.n_attributes = struct.unpack(">i", buf.read(4))[0]
-        self.PvAttributes = []
-        for i0 in range(self.n_attributes):
-            self.PvAttributes.append(compas_lcmtypes.senlcm.prosilica_attribute_t._decode_one(buf))
+        self = rph_angrate_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.rph = struct.unpack('>3d', buf.read(24))
+        self.angRate = struct.unpack('>3d', buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if prosilica_t in parents: return 0
-        newparents = parents + [prosilica_t]
-        tmphash = (0x84aedcc25441391a+ compas_lcmtypes.senlcm.prosilica_attribute_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
+        if rph_angrate_t in parents: return 0
+        newparents = parents + [rph_angrate_t]
+        tmphash = (0x2aa5eb76897e5606+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if prosilica_t._packed_fingerprint is None:
-            prosilica_t._packed_fingerprint = struct.pack(">Q", prosilica_t._get_hash_recursive([]))
-        return prosilica_t._packed_fingerprint
+        if rph_angrate_t._packed_fingerprint is None:
+            rph_angrate_t._packed_fingerprint = struct.pack(">Q", rph_angrate_t._get_hash_recursive([]))
+        return rph_angrate_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", prosilica_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", rph_angrate_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/raw_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/position_t.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,64 +5,70 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class raw_t(object):
-    __slots__ = ["utime", "length", "data"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "int32_t", "byte"]
+class position_t(object):
+    __slots__ = ["header", "xyz", "xyz_cov"]
 
-    __dimensions__ = [None, None, ["length"]]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double"]
+
+    __dimensions__ = [None, [3], [9]]
 
     def __init__(self):
-        self.utime = 0
-        self.length = 0
-        self.data = b""
+        self.header = compas_lcmtypes.standard.header_t()
+        self.xyz = [ 0.0 for dim0 in range(3) ]
+        self.xyz_cov = [ 0.0 for dim0 in range(9) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(raw_t._get_packed_fingerprint())
+        buf.write(position_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qi", self.utime, self.length))
-        buf.write(bytearray(self.data[:self.length]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack('>3d', *self.xyz[:3]))
+        buf.write(struct.pack('>9d', *self.xyz_cov[:9]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != raw_t._get_packed_fingerprint():
+        if buf.read(8) != position_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return raw_t._decode_one(buf)
+        return position_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = raw_t()
-        self.utime, self.length = struct.unpack(">qi", buf.read(12))
-        self.data = buf.read(self.length)
+        self = position_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.xyz = struct.unpack('>3d', buf.read(24))
+        self.xyz_cov = struct.unpack('>9d', buf.read(72))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if raw_t in parents: return 0
-        tmphash = (0x182b8da2dc0260c7) & 0xffffffffffffffff
+        if position_t in parents: return 0
+        newparents = parents + [position_t]
+        tmphash = (0x4ad0f080677f06f1+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if raw_t._packed_fingerprint is None:
-            raw_t._packed_fingerprint = struct.pack(">Q", raw_t._get_hash_recursive([]))
-        return raw_t._packed_fingerprint
+        if position_t._packed_fingerprint is None:
+            position_t._packed_fingerprint = struct.pack(">Q", position_t._get_hash_recursive([]))
+        return position_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", raw_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", position_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rdi_bathy_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/imu_t.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,71 +5,73 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class rdi_bathy_t(object):
-    __slots__ = ["utime", "range", "xyz"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "float", "float"]
+class imu_t(object):
+    __slots__ = ["header", "orientation", "angRate", "xyz_ddot"]
 
-    __dimensions__ = [None, [4], [4, 3]]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double", "double"]
 
-    RANGE_SENTINAL = 0
+    __dimensions__ = [None, [4], [3], [3]]
 
     def __init__(self):
-        self.utime = 0
-        self.range = [ 0.0 for dim0 in range(4) ]
-        self.xyz = [ [ 0.0 for dim1 in range(3) ] for dim0 in range(4) ]
+        self.header = compas_lcmtypes.standard.header_t()
+        self.orientation = [ 0.0 for dim0 in range(4) ]
+        self.angRate = [ 0.0 for dim0 in range(3) ]
+        self.xyz_ddot = [ 0.0 for dim0 in range(3) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(rdi_bathy_t._get_packed_fingerprint())
+        buf.write(imu_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">q", self.utime))
-        buf.write(struct.pack('>4f', *self.range[:4]))
-        for i0 in range(4):
-            buf.write(struct.pack('>3f', *self.xyz[i0][:3]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack('>4d', *self.orientation[:4]))
+        buf.write(struct.pack('>3d', *self.angRate[:3]))
+        buf.write(struct.pack('>3d', *self.xyz_ddot[:3]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != rdi_bathy_t._get_packed_fingerprint():
+        if buf.read(8) != imu_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return rdi_bathy_t._decode_one(buf)
+        return imu_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = rdi_bathy_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.range = struct.unpack('>4f', buf.read(16))
-        self.xyz = []
-        for i0 in range(4):
-            self.xyz.append(struct.unpack('>3f', buf.read(12)))
+        self = imu_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.orientation = struct.unpack('>4d', buf.read(32))
+        self.angRate = struct.unpack('>3d', buf.read(24))
+        self.xyz_ddot = struct.unpack('>3d', buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if rdi_bathy_t in parents: return 0
-        tmphash = (0xb573265d6b32ac19) & 0xffffffffffffffff
+        if imu_t in parents: return 0
+        newparents = parents + [imu_t]
+        tmphash = (0xf72bd2d311e44505+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if rdi_bathy_t._packed_fingerprint is None:
-            rdi_bathy_t._packed_fingerprint = struct.pack(">Q", rdi_bathy_t._get_hash_recursive([]))
-        return rdi_bathy_t._packed_fingerprint
+        if imu_t._packed_fingerprint is None:
+            imu_t._packed_fingerprint = struct.pack(">Q", imu_t._get_hash_recursive([]))
+        return imu_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", rdi_bathy_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", imu_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rdi_pd5_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/navlcm/pose_t.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,80 +5,73 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-import compas_lcmtypes.senlcm.rdi_pd4_t
+import compas_lcmtypes.geometry.pose_t
 
-class rdi_pd5_t(object):
-    __slots__ = ["utime", "pd4", "salinity", "depth", "pitch", "roll", "heading", "dmg_btv", "dmg_wtv"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "compas_lcmtypes.senlcm.rdi_pd4_t", "double", "double", "double", "double", "double", "double", "double"]
+class pose_t(object):
+    __slots__ = ["header", "pose", "pose_covariance"]
 
-    __dimensions__ = [None, None, None, None, None, None, None, [4], [4]]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "compas_lcmtypes.geometry.pose_t", "double"]
+
+    __dimensions__ = [None, None, [36]]
 
     def __init__(self):
-        self.utime = 0
-        self.pd4 = compas_lcmtypes.senlcm.rdi_pd4_t()
-        self.salinity = 0.0
-        self.depth = 0.0
-        self.pitch = 0.0
-        self.roll = 0.0
-        self.heading = 0.0
-        self.dmg_btv = [ 0.0 for dim0 in range(4) ]
-        self.dmg_wtv = [ 0.0 for dim0 in range(4) ]
+        self.header = compas_lcmtypes.standard.header_t()
+        self.pose = compas_lcmtypes.geometry.pose_t()
+        self.pose_covariance = [ 0.0 for dim0 in range(36) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(rdi_pd5_t._get_packed_fingerprint())
+        buf.write(pose_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">q", self.utime))
-        assert self.pd4._get_packed_fingerprint() == compas_lcmtypes.senlcm.rdi_pd4_t._get_packed_fingerprint()
-        self.pd4._encode_one(buf)
-        buf.write(struct.pack(">ddddd", self.salinity, self.depth, self.pitch, self.roll, self.heading))
-        buf.write(struct.pack('>4d', *self.dmg_btv[:4]))
-        buf.write(struct.pack('>4d', *self.dmg_wtv[:4]))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        assert self.pose._get_packed_fingerprint() == compas_lcmtypes.geometry.pose_t._get_packed_fingerprint()
+        self.pose._encode_one(buf)
+        buf.write(struct.pack('>36d', *self.pose_covariance[:36]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != rdi_pd5_t._get_packed_fingerprint():
+        if buf.read(8) != pose_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return rdi_pd5_t._decode_one(buf)
+        return pose_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = rdi_pd5_t()
-        self.utime = struct.unpack(">q", buf.read(8))[0]
-        self.pd4 = compas_lcmtypes.senlcm.rdi_pd4_t._decode_one(buf)
-        self.salinity, self.depth, self.pitch, self.roll, self.heading = struct.unpack(">ddddd", buf.read(40))
-        self.dmg_btv = struct.unpack('>4d', buf.read(32))
-        self.dmg_wtv = struct.unpack('>4d', buf.read(32))
+        self = pose_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.pose = compas_lcmtypes.geometry.pose_t._decode_one(buf)
+        self.pose_covariance = struct.unpack('>36d', buf.read(288))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if rdi_pd5_t in parents: return 0
-        newparents = parents + [rdi_pd5_t]
-        tmphash = (0x94c4660b03ed5183+ compas_lcmtypes.senlcm.rdi_pd4_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
+        if pose_t in parents: return 0
+        newparents = parents + [pose_t]
+        tmphash = (0x423ec15e5fc94cf9+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)+ compas_lcmtypes.geometry.pose_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if rdi_pd5_t._packed_fingerprint is None:
-            rdi_pd5_t._packed_fingerprint = struct.pack(">Q", rdi_pd5_t._get_hash_recursive([]))
-        return rdi_pd5_t._packed_fingerprint
+        if pose_t._packed_fingerprint is None:
+            pose_t._packed_fingerprint = struct.pack(">Q", pose_t._get_hash_recursive([]))
+        return pose_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", rdi_pd5_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", pose_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/relay_activation_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/magnetometer_t.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,70 +5,67 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class relay_activation_t(object):
-    __slots__ = ["utime", "cam_1", "cam_2", "dvl", "bp_oculus", "laser", "led", "odroid"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "int16_t", "int16_t", "int16_t", "int16_t", "int16_t", "int16_t", "int16_t"]
+class magnetometer_t(object):
+    __slots__ = ["header", "magfield"]
 
-    __dimensions__ = [None, None, None, None, None, None, None, None]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double"]
 
-    ON = 1
-    OFF = 0
+    __dimensions__ = [None, [3]]
 
     def __init__(self):
-        self.utime = 0
-        self.cam_1 = 0
-        self.cam_2 = 0
-        self.dvl = 0
-        self.bp_oculus = 0
-        self.laser = 0
-        self.led = 0
-        self.odroid = 0
+        self.header = compas_lcmtypes.standard.header_t()
+        self.magfield = [ 0.0 for dim0 in range(3) ]
 
     def encode(self):
         buf = BytesIO()
-        buf.write(relay_activation_t._get_packed_fingerprint())
+        buf.write(magnetometer_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qhhhhhhh", self.utime, self.cam_1, self.cam_2, self.dvl, self.bp_oculus, self.laser, self.led, self.odroid))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack('>3d', *self.magfield[:3]))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != relay_activation_t._get_packed_fingerprint():
+        if buf.read(8) != magnetometer_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return relay_activation_t._decode_one(buf)
+        return magnetometer_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = relay_activation_t()
-        self.utime, self.cam_1, self.cam_2, self.dvl, self.bp_oculus, self.laser, self.led, self.odroid = struct.unpack(">qhhhhhhh", buf.read(22))
+        self = magnetometer_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.magfield = struct.unpack('>3d', buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if relay_activation_t in parents: return 0
-        tmphash = (0xce51f04b6f7132fd) & 0xffffffffffffffff
+        if magnetometer_t in parents: return 0
+        newparents = parents + [magnetometer_t]
+        tmphash = (0x850646cd720587aa+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if relay_activation_t._packed_fingerprint is None:
-            relay_activation_t._packed_fingerprint = struct.pack(">Q", relay_activation_t._get_hash_recursive([]))
-        return relay_activation_t._packed_fingerprint
+        if magnetometer_t._packed_fingerprint is None:
+            magnetometer_t._packed_fingerprint = struct.pack(">Q", magnetometer_t._get_hash_recursive([]))
+        return magnetometer_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", relay_activation_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", magnetometer_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/rtidvl_nmea_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/senlcm/gps_fix_t.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,78 +5,69 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class rtidvl_nmea_t(object):
-    __slots__ = ["utime", "timeStartup", "sample", "temperature", "btv", "altitude", "wtv", "wtv_layer", "bit", "subsystem", "subsystem_index"]
+import compas_lcmtypes.standard.header_t
 
-    __typenames__ = ["int64_t", "int64_t", "int32_t", "double", "double", "double", "double", "double", "double", "int32_t", "int32_t"]
+class gps_fix_t(object):
+    __slots__ = ["header", "latitude", "longitud", "altitude"]
 
-    __dimensions__ = [None, None, None, None, [4], None, [4], None, None, None, None]
+    __typenames__ = ["compas_lcmtypes.standard.header_t", "double", "double", "double"]
+
+    __dimensions__ = [None, None, None, None]
 
     def __init__(self):
-        self.utime = 0
-        self.timeStartup = 0
-        self.sample = 0
-        self.temperature = 0.0
-        self.btv = [ 0.0 for dim0 in range(4) ]
+        self.header = compas_lcmtypes.standard.header_t()
+        self.latitude = 0.0
+        self.longitud = 0.0
         self.altitude = 0.0
-        self.wtv = [ 0.0 for dim0 in range(4) ]
-        self.wtv_layer = 0.0
-        self.bit = 0.0
-        self.subsystem = 0
-        self.subsystem_index = 0
 
     def encode(self):
         buf = BytesIO()
-        buf.write(rtidvl_nmea_t._get_packed_fingerprint())
+        buf.write(gps_fix_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qqid", self.utime, self.timeStartup, self.sample, self.temperature))
-        buf.write(struct.pack('>4d', *self.btv[:4]))
-        buf.write(struct.pack(">d", self.altitude))
-        buf.write(struct.pack('>4d', *self.wtv[:4]))
-        buf.write(struct.pack(">ddii", self.wtv_layer, self.bit, self.subsystem, self.subsystem_index))
+        assert self.header._get_packed_fingerprint() == compas_lcmtypes.standard.header_t._get_packed_fingerprint()
+        self.header._encode_one(buf)
+        buf.write(struct.pack(">ddd", self.latitude, self.longitud, self.altitude))
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != rtidvl_nmea_t._get_packed_fingerprint():
+        if buf.read(8) != gps_fix_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return rtidvl_nmea_t._decode_one(buf)
+        return gps_fix_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = rtidvl_nmea_t()
-        self.utime, self.timeStartup, self.sample, self.temperature = struct.unpack(">qqid", buf.read(28))
-        self.btv = struct.unpack('>4d', buf.read(32))
-        self.altitude = struct.unpack(">d", buf.read(8))[0]
-        self.wtv = struct.unpack('>4d', buf.read(32))
-        self.wtv_layer, self.bit, self.subsystem, self.subsystem_index = struct.unpack(">ddii", buf.read(24))
+        self = gps_fix_t()
+        self.header = compas_lcmtypes.standard.header_t._decode_one(buf)
+        self.latitude, self.longitud, self.altitude = struct.unpack(">ddd", buf.read(24))
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if rtidvl_nmea_t in parents: return 0
-        tmphash = (0x2a793dd9726e2227) & 0xffffffffffffffff
+        if gps_fix_t in parents: return 0
+        newparents = parents + [gps_fix_t]
+        tmphash = (0x34d70df50a971e8b+ compas_lcmtypes.standard.header_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if rtidvl_nmea_t._packed_fingerprint is None:
-            rtidvl_nmea_t._packed_fingerprint = struct.pack(">Q", rtidvl_nmea_t._get_hash_recursive([]))
-        return rtidvl_nmea_t._packed_fingerprint
+        if gps_fix_t._packed_fingerprint is None:
+            gps_fix_t._packed_fingerprint = struct.pack(">Q", gps_fix_t._get_hash_recursive([]))
+        return gps_fix_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", rtidvl_nmea_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", gps_fix_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/compas_lcmtypes/senlcm/timedrift_t.py` & `compas_lcmtypes-2023.2/compas_lcmtypes/geometry/pose_t.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,67 +5,70 @@
 
 try:
     import cStringIO.StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 import struct
 
-class timedrift_t(object):
-    __slots__ = ["sync_host", "sync_ticks", "ticks_sec", "host_before", "host_after", "ticks", "host_utime", "cam_utime"]
+import compas_lcmtypes.geometry.point_t
 
-    __typenames__ = ["int64_t", "int64_t", "double", "int64_t", "int64_t", "int64_t", "int64_t", "int64_t"]
+import compas_lcmtypes.geometry.quaternion_t
 
-    __dimensions__ = [None, None, None, None, None, None, None, None]
+class pose_t(object):
+    __slots__ = ["position", "orientation"]
+
+    __typenames__ = ["compas_lcmtypes.geometry.point_t", "compas_lcmtypes.geometry.quaternion_t"]
+
+    __dimensions__ = [None, None]
 
     def __init__(self):
-        self.sync_host = 0
-        self.sync_ticks = 0
-        self.ticks_sec = 0.0
-        self.host_before = 0
-        self.host_after = 0
-        self.ticks = 0
-        self.host_utime = 0
-        self.cam_utime = 0
+        self.position = compas_lcmtypes.geometry.point_t()
+        self.orientation = compas_lcmtypes.geometry.quaternion_t()
 
     def encode(self):
         buf = BytesIO()
-        buf.write(timedrift_t._get_packed_fingerprint())
+        buf.write(pose_t._get_packed_fingerprint())
         self._encode_one(buf)
         return buf.getvalue()
 
     def _encode_one(self, buf):
-        buf.write(struct.pack(">qqdqqqqq", self.sync_host, self.sync_ticks, self.ticks_sec, self.host_before, self.host_after, self.ticks, self.host_utime, self.cam_utime))
+        assert self.position._get_packed_fingerprint() == compas_lcmtypes.geometry.point_t._get_packed_fingerprint()
+        self.position._encode_one(buf)
+        assert self.orientation._get_packed_fingerprint() == compas_lcmtypes.geometry.quaternion_t._get_packed_fingerprint()
+        self.orientation._encode_one(buf)
 
     def decode(data):
         if hasattr(data, 'read'):
             buf = data
         else:
             buf = BytesIO(data)
-        if buf.read(8) != timedrift_t._get_packed_fingerprint():
+        if buf.read(8) != pose_t._get_packed_fingerprint():
             raise ValueError("Decode error")
-        return timedrift_t._decode_one(buf)
+        return pose_t._decode_one(buf)
     decode = staticmethod(decode)
 
     def _decode_one(buf):
-        self = timedrift_t()
-        self.sync_host, self.sync_ticks, self.ticks_sec, self.host_before, self.host_after, self.ticks, self.host_utime, self.cam_utime = struct.unpack(">qqdqqqqq", buf.read(64))
+        self = pose_t()
+        self.position = compas_lcmtypes.geometry.point_t._decode_one(buf)
+        self.orientation = compas_lcmtypes.geometry.quaternion_t._decode_one(buf)
         return self
     _decode_one = staticmethod(_decode_one)
 
     def _get_hash_recursive(parents):
-        if timedrift_t in parents: return 0
-        tmphash = (0x3144eb295ac5e503) & 0xffffffffffffffff
+        if pose_t in parents: return 0
+        newparents = parents + [pose_t]
+        tmphash = (0x2d70dd60bd541272+ compas_lcmtypes.geometry.point_t._get_hash_recursive(newparents)+ compas_lcmtypes.geometry.quaternion_t._get_hash_recursive(newparents)) & 0xffffffffffffffff
         tmphash  = (((tmphash<<1)&0xffffffffffffffff) + (tmphash>>63)) & 0xffffffffffffffff
         return tmphash
     _get_hash_recursive = staticmethod(_get_hash_recursive)
     _packed_fingerprint = None
 
     def _get_packed_fingerprint():
-        if timedrift_t._packed_fingerprint is None:
-            timedrift_t._packed_fingerprint = struct.pack(">Q", timedrift_t._get_hash_recursive([]))
-        return timedrift_t._packed_fingerprint
+        if pose_t._packed_fingerprint is None:
+            pose_t._packed_fingerprint = struct.pack(">Q", pose_t._get_hash_recursive([]))
+        return pose_t._packed_fingerprint
     _get_packed_fingerprint = staticmethod(_get_packed_fingerprint)
 
     def get_hash(self):
         """Get the LCM hash of the struct"""
-        return struct.unpack(">Q", timedrift_t._get_packed_fingerprint())[0]
+        return struct.unpack(">Q", pose_t._get_packed_fingerprint())[0]
```

### Comparing `compas_lcmtypes-2023.1/setup.py` & `compas_lcmtypes-2023.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['compas_lcmtypes',
  'compas_lcmtypes.bot_core',
+ 'compas_lcmtypes.geometry',
  'compas_lcmtypes.navlcm',
- 'compas_lcmtypes.oi',
- 'compas_lcmtypes.senlcm']
+ 'compas_lcmtypes.senlcm',
+ 'compas_lcmtypes.standard']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'compas-lcmtypes',
-    'version': '2023.1',
+    'version': '2023.2',
     'description': 'CoMPAS LCM types',
     'long_description': 'None',
     'author': 'Kevin Barnard',
     'author_email': 'kbarnard@mbari.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

