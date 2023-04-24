# Comparing `tmp/python_ember_mug-0.7.0b1.tar.gz` & `tmp/python_ember_mug-0.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b1.tar", max compression
+gzip compressed data, was "python_ember_mug-0.7.0b2.tar", max compression
```

## Comparing `python_ember_mug-0.7.0b1.tar` & `python_ember_mug-0.7.0b2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/LICENSE
--rw-r--r--   0        0        0     5219 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/README.md
--rwxr-xr-x   0        0        0      189 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8471 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     4890 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/consts.py
--rw-r--r--   0        0        0     7776 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/formatting.py
--rw-r--r--   0        0        0    16978 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/mug.py
--rw-r--r--   0        0        0     2112 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/scanner.py
--rw-r--r--   0        0        0     1963 2023-04-23 18:10:40.292760 python_ember_mug-0.7.0b1/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/conftest.py
--rw-r--r--   0        0        0    19254 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_consts.py
--rw-r--r--   0        0        0     2343 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_formatting.py
--rw-r--r--   0        0        0     3338 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-23 18:10:40.296760 python_ember_mug-0.7.0b1/tests/test_utils.py
--rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/LICENSE
+-rw-r--r--   0        0        0     5282 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/README.md
+-rwxr-xr-x   0        0        0      189 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8471 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     4875 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/consts.py
+-rw-r--r--   0        0        0     8198 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/formatting.py
+-rw-r--r--   0        0        0    17544 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/mug.py
+-rw-r--r--   0        0        0     2112 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/scanner.py
+-rw-r--r--   0        0        0     1973 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/ember_mug/utils.py
+-rw-r--r--   0        0        0     2896 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-24 00:31:08.017132 python_ember_mug-0.7.0b2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_connection.py
+-rw-r--r--   0        0        0      776 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_consts.py
+-rw-r--r--   0        0        0     2383 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_formatting.py
+-rw-r--r--   0        0        0     3366 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-24 00:31:08.021132 python_ember_mug-0.7.0b2/tests/test_utils.py
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b2/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b1/LICENSE` & `python_ember_mug-0.7.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/README.md` & `python_ember_mug-0.7.0b2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ## Summary
 
 This is an *unofficial* library to attempt to interact with Ember Mugs via Bluetooth.
 This was created for use with my [Home Assistant integration](https://github.com/sopelj/hass-ember-mug-component),
 but could be useful separately and has a simple CLI interface too.
 
-**Note**: Works with the standard Ember Mug (1 and 2). The Cup and Thermos may work, but have not been tested.
+**Note**: Confirmed working with the standard Ember Mug (1 and 2), Ember Cup (2) and Travel Mug (1). If you have another device, and it works or doesn't, please let me know.
 
 ## Features
 
 * Finding devices
 * Connecting to devices
 * Reading Information (Colour, temp, liquid level, etc.)
 * Writing (Desired temp, colour, temperature unit)*
```

### Comparing `python_ember_mug-0.7.0b1/ember_mug/cli/commands.py` & `python_ember_mug-0.7.0b2/ember_mug/cli/commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/ember_mug/cli/helpers.py` & `python_ember_mug-0.7.0b2/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/ember_mug/consts.py` & `python_ember_mug-0.7.0b2/ember_mug/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     'current_temp': 'Current Temp',
     'target_temp': 'Target Temp',
     'use_metric': 'Use Metric',
     'dsk': 'DSK',
     'udsk': 'UDSK',
     'date_time_zone': 'Date Time + Time Zone',
     'battery_voltage': 'Voltage',
+    'volume': 'Volume',
 }
 
 # Attributes
 INITIAL_ATTRS = {
     "meta",
     "udsk",
     "dsk",
@@ -177,15 +178,14 @@
     "current_temp",
     "target_temp",
     "temperature_unit",
     "battery",
     "liquid_level",
     "liquid_state",
 }
-TRAVEL_MUG_ATTRS = {"battery_voltage"}
 EXTRA_ATTRS = {'dsk', 'udsk', 'battery_voltage', 'date_time_zone'}
 
 # Validation
 MUG_NAME_REGEX = re.compile(r"^[A-Za-z0-9,.\[\]#()!\"\';:|\-_+<>%= ]{1,16}$")
 MAC_ADDRESS_REGEX = re.compile(r"^([0-9A-Fa-f]{2}:){5}([0-9A-Fa-f]{2})$")
 
 IS_LINUX = platform.system() == "Linux"
```

### Comparing `python_ember_mug-0.7.0b1/ember_mug/data.py` & `python_ember_mug-0.7.0b2/ember_mug/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Classes for representing data from the mug."""
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, is_dataclass
+from datetime import datetime
 from functools import cached_property
 from typing import Any, NamedTuple
 
 from .consts import (
     ATTR_LABELS,
     EMBER_CUP,
+    EMBER_TRAVEL_MUG,
     EMBER_TRAVEL_MUG_SHORT,
     EXTRA_ATTRS,
     INITIAL_ATTRS,
-    TRAVEL_MUG_ATTRS,
     UPDATE_ATTRS,
     LiquidState,
     TemperatureUnit,
 )
 from .formatting import format_led_colour, format_liquid_level, format_temp
 from .utils import bytes_to_little_int, decode_byte_string
 
@@ -102,21 +103,29 @@
                 f'Version: {self.version}',
                 f'Hardware: {self.hardware}',
                 f'Bootloader: {self.bootloader}',
             ),
         )
 
 
-@dataclass
+@dataclass(init=False)
 class Model:
     """Model name and attributes based on mode."""
 
     name: str
     include_extra: bool = False
 
+    def __init__(self, name: str, include_extra: bool = False) -> None:
+        """Override init to set long name for travel mug."""
+        if name == EMBER_TRAVEL_MUG_SHORT:
+            # Replace with full name for aesthetics
+            name = EMBER_TRAVEL_MUG
+        self.name = name
+        self.include_extra = include_extra
+
     @cached_property
     def is_cup(self) -> bool:
         """Check if the model is a Cup."""
         return self.name.startswith(EMBER_CUP)
 
     @cached_property
     def is_travel_mug(self) -> bool:
@@ -141,15 +150,15 @@
         """Attributes to update based on model and extra."""
         attributes = UPDATE_ATTRS
         if self.include_extra is False:
             attributes = attributes - EXTRA_ATTRS
         if self.is_cup:
             attributes = attributes - {'name'}
         elif self.is_travel_mug:
-            attributes = (attributes - {'led_colour', 'liquid_level'}) | TRAVEL_MUG_ATTRS
+            attributes = (attributes - {'led_colour', 'liquid_level'}) | {'volume'}
         return attributes
 
 
 @dataclass
 class MugMeta:
     """Meta data for mug."""
 
@@ -186,16 +195,17 @@
     liquid_state: LiquidState = LiquidState.UNKNOWN
     liquid_level: int = 0
     temperature_unit: TemperatureUnit = TemperatureUnit.CELSIUS
     current_temp: float = 0.0
     target_temp: float = 0.0
     dsk: str = ""
     udsk: str = ""
-    date_time_zone: str = ""
-    battery_voltage: str = ""
+    volume: int | None = None
+    date_time_zone: datetime | None = None
+    battery_voltage: int | None = None
 
     @property
     def meta_display(self) -> str:
         """Return Meta infor based on preference."""
         if self.meta and not self.model.include_extra:
             return f'Serial Number: {self.meta.serial_number}'
         return str(self.meta)
```

### Comparing `python_ember_mug-0.7.0b1/ember_mug/formatting.py` & `python_ember_mug-0.7.0b2/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/ember_mug/mug.py` & `python_ember_mug-0.7.0b2/ember_mug/mug.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,14 +213,27 @@
         return temp_from_bytes(temp_bytes, self.data.use_metric)
 
     async def get_liquid_level(self) -> int:
         """Get liquid level from mug gatt."""
         liquid_level_bytes = await self._read(MugCharacteristic.LIQUID_LEVEL)
         return bytes_to_little_int(liquid_level_bytes)
 
+    async def get_volume(self) -> int | None:
+        """Get volume from mug gatt."""
+        try:
+            volume_bytes = await self._read(MugCharacteristic.VOLUME)
+        except (BleakError, ValueError, TypeError) as e:
+            logger.error('Failed to read volume attribute.  Error was: %s', e)
+            return None
+        try:
+            return bytes_to_little_int(volume_bytes)
+        except (TypeError, ValueError) as e:
+            logger.error('Failed to decode volume value. Values was %s, Error was: %s', volume_bytes, e)
+        return None
+
     async def get_liquid_state(self) -> LiquidState:
         """Get liquid state from mug gatt."""
         liquid_state_bytes = await self._read(MugCharacteristic.LIQUID_STATE)
         state = bytes_to_little_int(liquid_state_bytes)
         return LiquidState(state)
 
     async def get_name(self) -> str:
```

### Comparing `python_ember_mug-0.7.0b1/ember_mug/scanner.py` & `python_ember_mug-0.7.0b2/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/ember_mug/utils.py` & `python_ember_mug-0.7.0b2/ember_mug/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def bytes_to_little_int(data: bytearray | bytes) -> int:
     """Convert bytes to little int."""
     return int.from_bytes(data, byteorder="little", signed=False)
 
 
 def bytes_to_big_int(data: bytearray | bytes) -> int:
     """Convert bytes to big int."""
-    return int.from_bytes(data, "big")
+    return int.from_bytes(data, byteorder="big")
 
 
 def temp_from_bytes(temp_bytes: bytearray, metric: bool = True) -> float:
     """Get temperature from bytearray and convert to Fahrenheit if needed."""
     temp = float(bytes_to_little_int(temp_bytes)) * 0.01
     if metric is False:
         # Convert to fahrenheit
```

### Comparing `python_ember_mug-0.7.0b1/pyproject.toml` & `python_ember_mug-0.7.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.7.0b1"
+version = "0.7.0b2"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.7.0b1/tests/cli/test_commands.py` & `python_ember_mug-0.7.0b2/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/cli/test_helpers.py` & `python_ember_mug-0.7.0b2/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/conftest.py` & `python_ember_mug-0.7.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/test_connection.py` & `python_ember_mug-0.7.0b2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/test_consts.py` & `python_ember_mug-0.7.0b2/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/test_data.py` & `python_ember_mug-0.7.0b2/tests/test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,21 +46,22 @@
     assert mug.is_travel_mug is False
     assert 'udsk' not in mug.initial_attributes
     assert 'name' in mug.update_attributes
     assert 'name' in mug.attribute_labels
     assert 'battery_voltage' not in mug.update_attributes
     mug_with_extra = Model(EMBER_MUG, include_extra=True)
     assert 'udsk' in mug_with_extra.initial_attributes
+    assert 'battery_voltage' not in mug.update_attributes
 
     travel_mug = Model(EMBER_TRAVEL_MUG)
     assert travel_mug.is_travel_mug is True
     assert travel_mug.is_cup is False
     assert 'name' in travel_mug.update_attributes
     assert 'name' in travel_mug.attribute_labels
-    assert 'battery_voltage' in travel_mug.attribute_labels
+    assert 'volume' in travel_mug.attribute_labels
 
     cup = Model(EMBER_CUP)
     assert cup.is_cup is True
     assert cup.is_travel_mug is False
     assert 'name' not in cup.update_attributes
     assert 'name' not in cup.attribute_labels
-    assert 'battery_voltage' not in cup.update_attributes
+    assert 'volume' not in cup.update_attributes
```

### Comparing `python_ember_mug-0.7.0b1/tests/test_formatting.py` & `python_ember_mug-0.7.0b2/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/test_mug_data.py` & `python_ember_mug-0.7.0b2/tests/test_mug_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,26 +75,27 @@
 
 def test_mug_dict(mug_data: MugData) -> None:
     mug_data.update_info(meta=MugMeta('test_id', 'serial number'))
     assert mug_data.as_dict() == {
         'model': {'include_extra': False, 'name': 'Ember Ceramic Mug'},
         'use_metric': True,
         'battery': None,
-        'battery_voltage': '',
+        'battery_voltage': None,
         'current_temp': 0.0,
         'current_temp_display': '0.00°C',
-        'date_time_zone': '',
+        'date_time_zone': None,
         'dsk': '',
         'firmware': None,
         'led_colour': Colour(red=255, green=255, blue=255),
         'led_colour_display': '#ffffff',
         'liquid_level': 0,
         'liquid_level_display': '0.00%',
         'liquid_state': LiquidState.UNKNOWN,
         'liquid_state_display': 'Unknown',
         'meta': {'mug_id': 'test_id', 'serial_number': 'serial number'},
         'name': '',
         'target_temp': 0.0,
         'target_temp_display': '0.00°C',
         'temperature_unit': TemperatureUnit.CELSIUS,
         'udsk': '',
+        'volume': None,
     }
```

### Comparing `python_ember_mug-0.7.0b1/tests/test_scanner.py` & `python_ember_mug-0.7.0b2/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/tests/test_utils.py` & `python_ember_mug-0.7.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b1/PKG-INFO` & `python_ember_mug-0.7.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.7.0b1
+Version: 0.7.0b2
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -46,15 +46,15 @@
 
 ## Summary
 
 This is an *unofficial* library to attempt to interact with Ember Mugs via Bluetooth.
 This was created for use with my [Home Assistant integration](https://github.com/sopelj/hass-ember-mug-component),
 but could be useful separately and has a simple CLI interface too.
 
-**Note**: Works with the standard Ember Mug (1 and 2). The Cup and Thermos may work, but have not been tested.
+**Note**: Confirmed working with the standard Ember Mug (1 and 2), Ember Cup (2) and Travel Mug (1). If you have another device, and it works or doesn't, please let me know.
 
 ## Features
 
 * Finding devices
 * Connecting to devices
 * Reading Information (Colour, temp, liquid level, etc.)
 * Writing (Desired temp, colour, temperature unit)*
```

