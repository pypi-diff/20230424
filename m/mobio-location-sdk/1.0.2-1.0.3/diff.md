# Comparing `tmp/mobio-location-sdk-1.0.2.tar.gz` & `tmp/mobio-location-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-location-sdk-1.0.2.tar", last modified: Fri Apr 21 09:26:07 2023, max compression
+gzip compressed data, was "mobio-location-sdk-1.0.3.tar", last modified: Mon Apr 24 12:16:30 2023, max compression
```

## Comparing `mobio-location-sdk-1.0.2.tar` & `mobio-location-sdk-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.661254 mobio-location-sdk-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-04-21 09:26:07.661254 mobio-location-sdk-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.645254 mobio-location-sdk-1.0.2/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.649254 mobio-location-sdk-1.0.2/mobio/sdks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.650254 mobio-location-sdk-1.0.2/mobio/sdks/location/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.652254 mobio-location-sdk-1.0.2/mobio/sdks/location/helpers/
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/helpers/function.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/helpers/redis_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.656254 mobio-location-sdk-1.0.2/mobio/sdks/location/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/models/address_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/models/base_model.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/models/country_configs.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/mobio/sdks/location/models/db_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:26:07.660254 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-04-21 09:26:07.000000 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-21 09:26:07.000000 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:26:07.000000 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-21 09:26:07.000000 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-21 09:26:07.000000 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-21 09:26:07.000000 mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 09:26:07.662254 mobio-location-sdk-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8880 2023-04-21 09:26:06.000000 mobio-location-sdk-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.759672 mobio-location-sdk-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-24 12:16:30.759672 mobio-location-sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.747671 mobio-location-sdk-1.0.3/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.750671 mobio-location-sdk-1.0.3/mobio/sdks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.750671 mobio-location-sdk-1.0.3/mobio/sdks/location/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.752671 mobio-location-sdk-1.0.3/mobio/sdks/location/helpers/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-04-24 12:13:48.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/helpers/function.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/helpers/redis_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.755672 mobio-location-sdk-1.0.3/mobio/sdks/location/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/models/address_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/models/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/models/country_configs.py
+-rw-r--r--   0 root         (0) root         (0)      882 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/mobio/sdks/location/models/db_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:30.758672 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-21 09:19:51.000000 mobio-location-sdk-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 12:16:30.759672 mobio-location-sdk-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-04-24 12:16:30.000000 mobio-location-sdk-1.0.3/setup.py
```

### Comparing `mobio-location-sdk-1.0.2/PKG-INFO` & `mobio-location-sdk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-location-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Mobio Location SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: # Thư viện Mobio Location SDK
```

### Comparing `mobio-location-sdk-1.0.2/mobio/sdks/location/helpers/function.py` & `mobio-location-sdk-1.0.3/mobio/sdks/location/helpers/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import unicodedata
+
 from ..models.country_configs import CountryConfigModel, CountryConfigStructure, RankConfigStructure
 from ..models.address_mapping import AddressMappingModel
 
+FIELD_MAPPING_NORMALIZE = ["country", "state", "county", "city", "district", "subdistrict"]
+
 
 class MappingInput:
     COUNTRY = "country"
 
 
 class CountryConfig:
     TYPE = "COUNTRY"
@@ -20,14 +24,16 @@
     def get_location_by_mapping(self, merchant_id, mapping):
         try:
             print("="*20)
             log_fuction = f'{LOG_HEADER} get_location_by_mapping():::'
             print(f'{log_fuction} INFO: input merchant_id: {merchant_id}')
             print(f'{log_fuction} INFO: input mapping: {mapping}')
 
+            mapping = self.normalize_unicode(mapping)
+            print('{} INFO: normalize_unicode input mapping: {}'.format(log_fuction, mapping))
             country_input = mapping.get(MappingInput.COUNTRY)
             if not country_input:
                 print(f'{log_fuction} ERROR: country_input is empty')
                 return False, None
 
             # get country first
             mapping_value = self._build_mapping_value([], country_input)
@@ -114,7 +120,20 @@
     @staticmethod
     def _build_mapping_value(mapping_codes, current_mapping_value):
         mapping_value = ""
         for item in mapping_codes:
             mapping_value = mapping_value + str(item) + "#"
         mapping_value = mapping_value + current_mapping_value + "#"
         return mapping_value
+
+    def normalize_unicode(self, mapping):
+        new_mapping = {}
+        for key, value in mapping.items():
+            if key in FIELD_MAPPING_NORMALIZE:
+                print("OLD: {} {}".format(key, bytearray(value, "utf-8")))
+                new_value = unicodedata.normalize("NFC", value)
+                print("NEW: {} {}".format(key, bytearray(new_value, "utf-8")))
+                new_mapping[key] = new_value
+            else:
+                new_mapping[key] = value
+        return new_mapping
+
```

### Comparing `mobio-location-sdk-1.0.2/mobio/sdks/location/helpers/redis_helper.py` & `mobio-location-sdk-1.0.3/mobio/sdks/location/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-1.0.2/mobio/sdks/location/models/address_mapping.py` & `mobio-location-sdk-1.0.3/mobio/sdks/location/models/address_mapping.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-1.0.2/mobio/sdks/location/models/base_model.py` & `mobio-location-sdk-1.0.3/mobio/sdks/location/models/base_model.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-1.0.2/mobio/sdks/location/models/country_configs.py` & `mobio-location-sdk-1.0.3/mobio/sdks/location/models/country_configs.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-1.0.2/mobio/sdks/location/models/db_manager.py` & `mobio-location-sdk-1.0.3/mobio/sdks/location/models/db_manager.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/PKG-INFO` & `mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-location-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Mobio Location SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: # Thư viện Mobio Location SDK
```

### Comparing `mobio-location-sdk-1.0.2/mobio_location_sdk.egg-info/SOURCES.txt` & `mobio-location-sdk-1.0.3/mobio_location_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-1.0.2/setup.py` & `mobio-location-sdk-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         :param filename:
         :return:
         """
         requirements = ["m-singleton", "redis", "pymongo"]
         return requirements
 
 
-version_dev='1.0.6'
-version_prod='1.0.2'
+version_dev='1.0.7'
+version_prod='1.0.3'
 
 run_mode=''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="mobio-location-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.2',  # Required, Phần này cũng không được format file.
+    version='1.0.3',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Location SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

