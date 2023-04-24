# Comparing `tmp/mpai_cae_arp-0.4.0.tar.gz` & `tmp/mpai_cae_arp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpai_cae_arp-0.4.0.tar", max compression
+gzip compressed data, was "mpai_cae_arp-0.4.1.tar", max compression
```

## Comparing `mpai_cae_arp-0.4.0.tar` & `mpai_cae_arp-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/LICENSE
--rw-r--r--   0        0        0      491 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/README.md
--rw-r--r--   0        0        0      276 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/__init__.py
--rw-r--r--   0        0        0      172 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/__init__.py
--rw-r--r--   0        0        0    18021 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_audio.py
--rw-r--r--   0        0        0     2516 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_noise.py
--rw-r--r--   0        0        0      231 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/standards.py
--rw-r--r--   0        0        0     4211 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/audio/utils.py
--rw-r--r--   0        0        0     2065 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/files.py
--rw-r--r--   0        0        0     1437 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/io.py
--rw-r--r--   0        0        0     2307 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2.py
--rw-r--r--   0        0        0     4041 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2_grpc.py
--rw-r--r--   0        0        0     3182 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/time.py
--rw-r--r--   0        0        0      314 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/__init__.py
--rw-r--r--   0        0        0     8323 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/irregularity.py
--rw-r--r--   0        0        0     2293 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/restoration.py
--rw-r--r--   0        0        0     1632 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/mpai_cae_arp/types/schema.py
--rw-r--r--   0        0        0     1236 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.4.0/setup.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/LICENSE
+-rw-r--r--   0        0        0      491 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/README.md
+-rw-r--r--   0        0        0      276 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/audio/__init__.py
+-rw-r--r--   0        0        0    18021 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/audio/_audio.py
+-rw-r--r--   0        0        0     2516 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/audio/_noise.py
+-rw-r--r--   0        0        0      231 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/audio/standards.py
+-rw-r--r--   0        0        0     4211 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/audio/utils.py
+-rw-r--r--   0        0        0     2065 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/files.py
+-rw-r--r--   0        0        0     1437 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/io.py
+-rw-r--r--   0        0        0     2307 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/network/arp_pb2.py
+-rw-r--r--   0        0        0     4041 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/network/arp_pb2_grpc.py
+-rw-r--r--   0        0        0     3182 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/time.py
+-rw-r--r--   0        0        0      314 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/types/__init__.py
+-rw-r--r--   0        0        0     8323 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/types/irregularity.py
+-rw-r--r--   0        0        0     2291 2023-04-24 17:26:35.835286 mpai_cae_arp-0.4.1/mpai_cae_arp/types/restoration.py
+-rw-r--r--   0        0        0     1632 2023-04-24 16:04:56.069432 mpai_cae_arp-0.4.1/mpai_cae_arp/types/schema.py
+-rw-r--r--   0        0        0     1236 2023-04-24 17:27:56.814948 mpai_cae_arp-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 mpai_cae_arp-0.4.1/setup.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 mpai_cae_arp-0.4.1/PKG-INFO
```

### Comparing `mpai_cae_arp-0.4.0/LICENSE` & `mpai_cae_arp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_audio.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/audio/_audio.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/audio/_noise.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/audio/_noise.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/audio/utils.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/audio/utils.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/files.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/files.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/io.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/io.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/network/arp_pb2.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/network/arp_pb2_grpc.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/network/arp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/time.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/time.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/types/irregularity.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/types/irregularity.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/types/restoration.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/types/restoration.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     id: uuid.UUID = Field(default_factory=uuid.uuid4, alias="RestorationID")
     preservation_audio_file_start: str = Field(alias="PreservationAudioFileStart")
     preservation_audio_file_end: str = Field(alias="PreservationAudioFileEnd")
     restored_audio_file_URI: str = Field(alias="RestoredAudioFileURI")
     reading_backwards: bool = Field(alias="ReadingBackwards")
     applied_speed_standard: SpeedStandard = Field(alias="AppliedSpeedStandard")
     applied_sample_frequency: int = Field(alias="AppliedSampleFrequency")
-    original_equalization_standard: EqualizationStandard = Field(
-        alias="OriginalEqualizationStandard")
+    applied_equalization_standard: EqualizationStandard = Field(
+        alias="AppliedEqualisationStandard")
 
 
 Self = TypeVar("Self", bound="EditingList")
 
 
 class EditingList(BaseModel):
     """
@@ -34,15 +34,15 @@
     """
 
     class Config:
         allow_population_by_field_name = True
 
     original_speed_standard: SpeedStandard = Field(alias="OriginalSpeedStandard")
     original_equalization_standard: EqualizationStandard = Field(
-        alias="OriginalEqualizationStandard")
+        alias="OriginalEqualisationStandard")
     original_sample_frequency: int = Field(alias="OriginalSampleFrequency")
     restorations: list[Restoration] = Field(alias="Restorations")
 
     def add(self, restoration: Restoration) -> Self:
         self.restorations.append(restoration)
         return self
```

### Comparing `mpai_cae_arp-0.4.0/mpai_cae_arp/types/schema.py` & `mpai_cae_arp-0.4.1/mpai_cae_arp/types/schema.py`

 * *Files identical despite different names*

### Comparing `mpai_cae_arp-0.4.0/pyproject.toml` & `mpai_cae_arp-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpai-cae-arp"
-version = "0.4.0"
+version = "0.4.1"
 description = "The MPAI CAE-ARP software API"
 authors = ["Matteo Spanio <dev2@audioinnova.com>"]
 readme = "README.md"
 packages = [{include = "mpai_cae_arp"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `mpai_cae_arp-0.4.0/setup.py` & `mpai_cae_arp-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'llvmlite>=0.39.1,<0.40.0',
  'numpy==1.23.3',
  'pydantic>=1.10.7,<2.0.0',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'mpai-cae-arp',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'The MPAI CAE-ARP software API',
     'long_description': '# MPAI CAE-ARP API\n\n[![LICENSE](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://img.shields.io/badge/license-GPLv3-blue.svg)\n\n## Description\n\nThis package provides a set of tools for common task in MPAI CAE-ARP standard. It is usend in the official implementation of the standard and can be used as well to develop your own.\n\n## License\n\nThis software is licensed under the GPLv3 license. See the [official site](http://www.gnu.org/licenses/gpl-3.0.html) for more information.\n',
     'author': 'Matteo Spanio',
     'author_email': 'dev2@audioinnova.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mpai_cae_arp-0.4.0/PKG-INFO` & `mpai_cae_arp-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpai-cae-arp
-Version: 0.4.0
+Version: 0.4.1
 Summary: The MPAI CAE-ARP software API
 Author: Matteo Spanio
 Author-email: dev2@audioinnova.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

