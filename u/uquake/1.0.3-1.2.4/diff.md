# Comparing `tmp/uquake-1.0.3.tar.gz` & `tmp/uquake-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uquake-1.0.3.tar", max compression
+gzip compressed data, was "uquake-1.2.4.tar", max compression
```

## Comparing `uquake-1.0.3.tar` & `uquake-1.2.4.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0     2419 2022-12-18 17:00:45.251852 uquake-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      106 2022-08-31 14:13:43.550987 uquake-1.0.3/uquake/__init__.py
--rw-r--r--   0        0        0      191 2022-08-31 14:13:43.551095 uquake-1.0.3/uquake/core/__init__.py
--rw-r--r--   0        0        0      658 2022-08-31 14:13:43.551173 uquake-1.0.3/uquake/core/decorators.py
--rw-r--r--   0        0        0    31389 2022-08-31 14:13:43.551326 uquake-1.0.3/uquake/core/event.py
--rw-r--r--   0        0        0     6233 2022-08-31 14:13:43.551440 uquake-1.0.3/uquake/core/focal_mechanism.py
--rw-r--r--   0        0        0    36615 2022-12-18 17:00:18.034148 uquake-1.0.3/uquake/core/inventory.py
--rw-r--r--   0        0        0      239 2022-08-31 14:13:43.551712 uquake-1.0.3/uquake/core/logging.py
--rw-r--r--   0        0        0    13628 2022-08-31 14:13:43.551824 uquake-1.0.3/uquake/core/stream.py
--rw-r--r--   0        0        0     5308 2022-08-31 14:13:43.551915 uquake-1.0.3/uquake/core/trace.py
--rw-r--r--   0        0        0       67 2022-08-31 14:13:43.552005 uquake-1.0.3/uquake/core/util/__init__.py
--rw-r--r--   0        0        0     4029 2022-08-31 14:13:43.552083 uquake-1.0.3/uquake/core/util/base.py
--rw-r--r--   0        0        0     5713 2022-08-31 14:13:43.552171 uquake-1.0.3/uquake/core/util/decorator.py
--rw-r--r--   0        0        0    13768 2022-08-31 14:13:43.552286 uquake-1.0.3/uquake/core/util/tools.py
--rw-r--r--   0        0        0       28 2022-08-31 14:13:43.552420 uquake-1.0.3/uquake/grid/__init__.py
--rw-r--r--   0        0        0    22979 2022-11-14 14:52:56.357648 uquake-1.0.3/uquake/grid/base.py
--rw-r--r--   0        0        0     4658 2022-08-31 14:13:43.552669 uquake-1.0.3/uquake/grid/hdf5.py
--rw-r--r--   0        0        0    46086 2022-11-14 14:50:34.766847 uquake-1.0.3/uquake/grid/nlloc.py
--rw-r--r--   0        0        0        0 2022-08-31 14:13:43.553016 uquake-1.0.3/uquake/imaging/__init__.py
--rw-r--r--   0        0        0     9674 2022-08-31 14:13:43.553148 uquake-1.0.3/uquake/imaging/plot.py
--rw-r--r--   0        0        0     2474 2022-08-31 14:13:43.553236 uquake-1.0.3/uquake/imaging/stereonet.py
--rw-r--r--   0        0        0    59743 2022-08-31 14:13:43.553480 uquake-1.0.3/uquake/imaging/waveform.py
--rw-r--r--   0        0        0      423 2022-08-31 14:13:43.553694 uquake-1.0.3/uquake/io/__init__.py
--rw-r--r--   0        0        0        0 2022-08-31 14:13:43.553754 uquake-1.0.3/uquake/io/event/__init__.py
--rw-r--r--   0        0        0     3417 2022-08-31 14:13:43.553841 uquake-1.0.3/uquake/io/event/core.py
--rw-r--r--   0        0        0       20 2022-08-31 14:13:43.553929 uquake-1.0.3/uquake/io/grid/__init__.py
--rw-r--r--   0        0        0     8496 2022-08-31 14:13:43.554020 uquake-1.0.3/uquake/io/grid/core.py
--rw-r--r--   0        0        0       20 2022-08-31 14:13:43.554104 uquake-1.0.3/uquake/io/waveform/__init__.py
--rw-r--r--   0        0        0     8944 2022-08-31 14:13:43.554205 uquake-1.0.3/uquake/io/waveform/core.py
--rw-r--r--   0        0        0       21 2022-08-31 14:13:43.554314 uquake-1.0.3/uquake/nlloc/__init__.py
--rw-r--r--   0        0        0    48293 2022-11-14 14:52:56.358096 uquake-1.0.3/uquake/nlloc/nlloc.py
--rw-r--r--   0        0        0        0 2022-08-31 14:13:43.554630 uquake-1.0.3/uquake/waveform/__init__.py
--rw-r--r--   0        0        0    34528 2022-08-31 14:13:43.554836 uquake-1.0.3/uquake/waveform/amp_measures.py
--rw-r--r--   0        0        0    15799 2022-08-31 14:13:43.554961 uquake-1.0.3/uquake/waveform/mag.py
--rw-r--r--   0        0        0     5354 2022-08-31 14:13:43.555065 uquake-1.0.3/uquake/waveform/mag_utils.py
--rw-r--r--   0        0        0     2827 2022-08-31 14:13:43.555144 uquake-1.0.3/uquake/waveform/parseval_utils.py
--rw-r--r--   0        0        0    23179 2022-08-31 14:13:43.555395 uquake-1.0.3/uquake/waveform/pick.py
--rw-r--r--   0        0        0    45455 2022-11-14 14:52:56.358512 uquake-1.0.3/uquake/waveform/simple_mag.py
--rw-r--r--   0        0        0    32225 2022-08-31 14:13:43.555829 uquake-1.0.3/uquake/waveform/smom_measure.py
--rw-r--r--   0        0        0    33065 2022-08-31 14:13:43.556056 uquake-1.0.3/uquake/waveform/smom_measure_legacy.py
--rw-r--r--   0        0        0     4456 2022-08-31 14:13:43.556159 uquake-1.0.3/uquake/waveform/transforms.py
--rw-r--r--   0        0        0     2901 2022-12-18 17:00:55.533447 uquake-1.0.3/setup.py
--rw-r--r--   0        0        0      953 2022-12-18 17:00:55.533665 uquake-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2345 2023-01-30 13:40:20.174805 uquake-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.2.4/uquake/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/__init__.py
+-rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/decorators.py
+-rw-r--r--   0        0        0    31807 2023-04-17 12:59:33.326538 uquake-1.2.4/uquake/core/event.py
+-rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/focal_mechanism.py
+-rw-r--r--   0        0        0    38774 2023-04-16 18:22:31.094780 uquake-1.2.4/uquake/core/inventory.py
+-rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/logging.py
+-rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.2.4/uquake/core/stream.py
+-rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/trace.py
+-rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/__init__.py
+-rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/base.py
+-rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/decorator.py
+-rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.2.4/uquake/core/util/requests.py
+-rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/core/util/tools.py
+-rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/grid/__init__.py
+-rw-r--r--   0        0        0    22963 2023-04-13 23:59:04.661740 uquake-1.2.4/uquake/grid/base.py
+-rw-r--r--   0        0        0     4658 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/grid/hdf5.py
+-rw-r--r--   0        0        0    47247 2023-04-14 00:12:47.864202 uquake-1.2.4/uquake/grid/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/imaging/__init__.py
+-rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.2.4/uquake/imaging/plot.py
+-rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.2.4/uquake/imaging/stereonet.py
+-rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/imaging/waveform.py
+-rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/event/__init__.py
+-rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/event/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/grid/__init__.py
+-rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/grid/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/inventory/__init__.py
+-rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/inventory/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/waveform/__init__.py
+-rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/io/waveform/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/nlloc/__init__.py
+-rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/nlloc/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/__init__.py
+-rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/amp_measures.py
+-rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/mag.py
+-rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/mag_utils.py
+-rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/parseval_utils.py
+-rw-r--r--   0        0        0    23179 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/pick.py
+-rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.2.4/uquake/waveform/simple_mag.py
+-rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/smom_measure.py
+-rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/smom_measure_legacy.py
+-rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.2.4/uquake/waveform/transforms.py
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 uquake-1.2.4/setup.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 uquake-1.2.4/PKG-INFO
```

### Comparing `uquake-1.0.3/pyproject.toml` & `uquake-1.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "uquake"
-version = "1.0.3"
+version = "1.2.4"
 description = "extension of the ObsPy library for local seismicity"
 authors = ["uQuake development team <dev@uQuake.org>"]
 license = "MIT"
 
 # poetry config virtualenvs.create false; poetry env info
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.10"
+python = "^3.9"
 numpy = "^1.18.0"
 loguru = "^0.5.3"
 pandas = "^1.2.1"
 jedi = "0.17.2"
 pytest = "^6.2.1"
 openpyxl = "^3.0.6"
 obspy = "^1.2.2"
@@ -26,25 +26,32 @@
 future = "^0.18.2"
 
 [tool.poetry.dev-dependencies]
 ipdb = "^0.13.9"
 ipython = "^8.1.0"
 
 [tool.poetry.plugins] # Optional super table
+
+[tool.poetry.plugins."uquake.io.inventory"]
+ESG_SENSOR = 'uquake.io.inventory'
+
+[tool.poetry.plugins."uquake.io.inventory.ESG_SENSOR"]
+readFormat = "uquake.io.inventory:read_esg_sensor_file"
+
+[tool.poetry.plugins."uquake.io.event"]
+QUAKEML = "uquake.io.quakeml"
+NLLOC = "uquake.io.nlloc"
+
 [tool.poetry.plugins."uquake.io.waveform"]
 ESG_SEGY = "uquake.io.waveform"
-HSF = "micorquake.io.waveform"
+HSF = "uquake.io.waveform"
 TEXCEL_CSV = "uquake.io.waveform"
 IMS_CONTINUOUS = "uquake.io.waveform"
 IMS_ASCII = "uquake.io.waveform"
 
-[tool.poetry.plugins."uquake.io.event"]
-QUAKEML = "uquake.io.quakeml"
-NLLOC = "uquake.io.nlloc"
-
 [tool.poetry.plugins."uquake.io.waveform.ESG_SEGY"]
 readFormat = "uquake.io.waveform:read_ESG_SEGY"
 
 [tool.poetry.plugins."uquake.io.waveform.TEXCEL_CSV"]
 readFormat = "uquake.io.waveform:read_TEXCEL_CSV"
 
 [tool.poetry.plugins."uquake.io.waveform.IMS_ASCII"]
@@ -72,19 +79,12 @@
 readFormat = "uquake.io.grid:read_pickle"
 writeFormat = "uquake.io.grid:write_pickle"
 
 [tool.poetry.plugins."uquake.io.grid.CSV"]
 writeFormat = "uquake.io.grid:write_csv"
 readFormat = "uquake.io.grid:read_csv"
 
-[tool.poetry.plugins."uquake.io.site.CSV"]
-readFormat = "uquake.io.site:read_csv"
-writeFormat = "uquake.io.site:write_csv"
-
-[tool.poetry.plugins."uquake.io.site.PICKLE"]
-readFormat = "uquake.io.site:read_pickle"
-writeFormat = "uquake.io.site:write_pickle"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `uquake-1.0.3/uquake/core/decorators.py` & `uquake-1.2.4/uquake/core/decorators.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/core/event.py` & `uquake-1.2.4/uquake/core/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,15 +387,15 @@
                 app_stress = 2 * self.energy_joule / self.potency_m3
         return app_stress
 
     @property
     def seismic_moment(self):
         seismic_moment = None
         if self.magnitude_type == 'Mw':
-            seismic_moment = 10 ** (3 * (self.mag + 6.02) / 2)
+            seismic_moment = 10 ** (3 * (self.mag + 6.03) / 2)
         return seismic_moment
 
     # @seismic_moment.setter
     # def seismic_moment(self, val):
     #     self.mag = val
     #     self.magnitude_type = 'Mw'
 
@@ -564,14 +564,34 @@
     def site_code(self):
         return self.pick.site
 
     @property
     def site(self):
         return self.pick.site
 
+    @property
+    def time(self):
+        return self.pick.time
+
+    @property
+    def channel(self):
+        return self.pick.waveform_id.channel_code
+
+    @property
+    def location(self):
+        return self.pick.waveform_id.location_code
+
+    @property
+    def station(self):
+        return self.pick.waveform_id.station_code
+
+    @property
+    def network(self):
+        return self.pick.waveform_id.network_code
+
     def get_pick(self):
         if self.pick_id is not None:
             return self.pick_id.get_referred_object()
 
     def get_sta(self):
         if self.pick_id is not None:
             pick = self.pick_id.get_referred_object()
@@ -917,15 +937,14 @@
 
         method_id = ResourceIdentifier('predicted from rays')
         return Pick(time=time, waveform_id=waveform_id, method_id=method_id,
                     back_azimuth=self.back_azimuth, phase_hint=self.phase,
                     evaluation_mode='automatic',
                     evaluation_status='preliminary')
 
-
     def __len__(self):
         return len(self.nodes)
 
     def __str__(self):
 
         site_code = f'{self.network}.{self.site_code[0:4]}.' \
                     f'{self.site_code[4:]}'
```

### Comparing `uquake-1.0.3/uquake/core/focal_mechanism.py` & `uquake-1.2.4/uquake/core/focal_mechanism.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/core/inventory.py` & `uquake-1.2.4/uquake/core/inventory.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,81 +17,158 @@
     (http://www.gnu.org/copyleft/lesser.html)
 """
 import io
 from obspy.core import inventory, AttribDict, UTCDateTime
 from obspy.core.inventory import Network
 from obspy.signal.invsim import corn_freq_2_paz
 from obspy.core.inventory import (Response, InstrumentSensitivity,
-                                  PolesZerosResponseStage)
+                                  PolesZerosResponseStage, ResponseStage)
 import numpy as np
 from obspy.core.inventory.util import (Equipment, Operator, Person,
                                        PhoneNumber, Site, _textwrap,
                                        _unified_content_strings)
 from pathlib import Path
 
-from obspy.clients.nrl import NRL
 from .logging import logger
 from uquake import __package_name__ as ns
 
 import pandas as pd
 from io import BytesIO
 from .util.tools import lon_lat_x_y
 
-nrl = NRL()
+from typing import List
+from .util import ENTRY_POINTS
+from pkg_resources import load_entry_point
+import requests
+from tqdm import tqdm
+from tempfile import NamedTemporaryFile
+import os
+from .util.requests import download_file_from_url
+
+
+class SystemResponse(object):
+    def __init__(self, sensitivity=1, frequency=1):
+        self.stage_sequence_number = 0
+        self.response_stages = []
+        self.sensitivity = sensitivity
+        self.frequency = frequency
+
+    def add_geophone(self, resonance_frequency, gain, damping=0.707,
+                     output_resistance=np.inf,
+                     cable_length=np.inf, cable_capacitance=np.inf):
+
+        resp = geophone_response(resonance_frequency, gain, damping=damping,
+                                 output_resistance=output_resistance,
+                                 cable_length=cable_length,
+                                 cable_capacitance=cable_capacitance,
+                                 stage_sequence_number=
+                                 self.stage_sequence_number)
+
+        self.stage_sequence_number += 1
+
+        self.response_stages.append(resp)
+
+    def add_accelerometer(self, resonance_frequency, gain, sensitivity=1,
+                          damping=0.707):
+
+        resp = accelerometer_response(resonance_frequency, gain,
+                                      sensitivity=sensitivity,
+                                      stage_sequence_number=
+                                      self.stage_sequence_number,
+                                      damping=damping)
+
+        self.stage_sequence_number += 1
+
+        self.response_stages.append(resp)
+
+    def add_digitizer(self, max_voltage=2.5, resolution_bit=24,
+                      stage_gain_frequency=1, digitizer_name=None):
+
+        stage_gain = 2 ** resolution_bit / max_voltage
+        resp = ResponseStage(self.stage_sequence_number, stage_gain,
+                             stage_gain_frequency,
+                             input_units='V', output_units='COUNT',
+                             input_units_description='voltage',
+                             output_units_description='ADC Count',
+                             name=digitizer_name)
+        self.stage_sequence_number += 1
+
+        self.response_stages.append(resp)
+
+    @property
+    def response(self):
+        if len(self.response_stages) == 0:
+            return
+
+        input_units = self.response_stages[0].input_units
+        i_s = InstrumentSensitivity(self.sensitivity,
+                                    self.frequency,
+                                    input_units=input_units,
+                                    output_units='COUNT',
+                                    input_units_description='Velocity',
+                                    output_units_description='ADC Count')
+
+        return Response(instrument_sensitivity=i_s,
+                        response_stages=self.response_stages)
 
 
 def geophone_response(resonance_frequency, gain, damping=0.707,
                       output_resistance=np.inf,
                       cable_length=np.inf, cable_capacitance=np.inf,
-                      sensitivity=1, stage_sequence_number=1):
+                      stage_sequence_number=0):
+
     paz = corn_freq_2_paz(resonance_frequency,
                           damp=damping)
 
     l = cable_length
     R = output_resistance
     C = cable_capacitance
 
     if ((R * l * C) != np.inf) and ((R * l * C) != 0):
         pole_cable = -1 / (R * l * C)
         paz['poles'].append(pole_cable)
 
-    i_s = InstrumentSensitivity(sensitivity, resonance_frequency,
-                                input_units='M/S',
-                                output_units='M/S',
-                                input_units_description='velocity',
-                                output_units_description='velocity')
+    # i_s = InstrumentSensitivity(sensitivity, resonance_frequency,
+    #                             input_units='M/S',
+    #                             output_units='COUNT',
+    #                             input_units_description='Velocity',
+    #                             output_units_description='ADC Count')
 
     pzr = PolesZerosResponseStage(stage_sequence_number, gain,
-                                  resonance_frequency, 'M/S', 'M/S',
+                                  resonance_frequency, 'M/S', 'V',
                                   'LAPLACE (RADIANT/SECOND)',
                                   resonance_frequency, paz['zeros'],
                                   paz['poles'])
 
-    return Response(instrument_sensitivity=i_s,
-                    response_stages=[pzr])
+    return pzr
+
+    # return Response(instrument_sensitivity=i_s,
+    #                 response_stages=[pzr])
 
 
 def accelerometer_response(resonance_frequency, gain, sensitivity=1,
-                           stage_sequence_number=1, damping=0.707):
+                           stage_sequence_number=0, damping=0.707):
     i_s = InstrumentSensitivity(sensitivity, resonance_frequency,
                                 input_units='M/S/S', output_units='M/S/S',
-                                input_units_description='acceleration',
-                                output_units_description='acceleration')
+                                input_units_description='ACC',
+                                output_units_description='ACC')
 
     paz = corn_freq_2_paz(resonance_frequency, damp=damping)
 
     paz['zeros'] = []
 
-    pzr = PolesZerosResponseStage(1, 1, 14, 'M/S/S', 'M/S',
+    pzr = PolesZerosResponseStage(stage_sequence_number, 1, 14, 'M/S/S', 'V',
                                   'LAPLACE (RADIANT/SECOND)',
                                   1, [],
                                   paz['poles'])
 
-    return Response(instrument_sensitivity=i_s,
-                    response_stages=[pzr])
+    return pzr
+
+    # return Response(instrument_sensitivity=i_s,
+    #                 response_stages=[pzr])
 
 
 def get_response_from_nrl(datalogger_keys, sensor_keys):
     pass
 
 
 # class Inventory(inventory.Inventory):
@@ -124,14 +201,43 @@
                                                            input_projection=
                                                            input_projection,
                                                            output_projection=
                                                            output_projection))
 
         return inv
 
+
+    @staticmethod
+    def from_url(url):
+        """
+        Load an ObsPy inventory object from a URL.
+
+        :param url: The URL to download the inventory file from.
+        :type url: str
+        :return: The loaded ObsPy inventory object.
+        :rtype: obspy.core.inventory.Inventory
+        """
+        # Download the inventory file from the URL
+
+        inventory_data = download_file_from_url(url)
+
+        # Save the inventory data to a temporary file
+        with NamedTemporaryFile(delete=False) as temp_file:
+            temp_file.write(inventory_data.read())
+            temp_file.flush()
+
+            # Load the inventory from the temporary file
+            file_format = 'STATIONXML'  # Replace with the correct format
+            inventory = read_inventory(temp_file.name, format=file_format)
+
+        # Remove the temporary file after reading the inventory
+        os.remove(temp_file.name)
+
+        return inventory
+
     @staticmethod
     def from_bytes(byte_string):
         file_in = io.BytesIO(byte_string)
         file_in.read()
         file_in.seek(0)
         return read_inventory(file_in)
 
@@ -243,15 +349,16 @@
             for site in station.sites:
                 if site.code in ignore_sites:
                     continue
                 coordinates.append(site.loc)
 
         min = np.min(coordinates, axis=0)
         max = np.max(coordinates, axis=0)
-        center = min + (max - min) / 2
+        # center = min + (max - min) / 2
+        center = (min + max) / 2
         d = (max - min) * (1 + padding_fraction)
 
         c1 = center - d / 2
         c2 = center + d / 2
 
         return c1, c2
 
@@ -363,87 +470,14 @@
                                                            input_projection=
                                                            input_projection,
                                                            output_projection=
                                                            output_projection))
 
         return stn
 
-    @classmethod
-    def from_station_dict(cls, station_dict, site):
-        stn = station_dict
-
-        equipments = []
-        if 'manufacturer_sensor' in stn:
-            equipments = [Equipment(type='Site',
-                                    manufacturer=stn['manufacturer_sensor'],
-                                    model=stn['model'])]
-
-        sta = cls(stn['station_code'], latitude=0., longitude=0.,
-                  elevation=0., site=Site(name=site),
-                  equipments=equipments,
-                  historical_code=stn['long_name'],
-                  creation_date=UTCDateTime("2015-12-31T12:23:34.5"),
-                  start_date=UTCDateTime("2015-12-31T12:23:34.5"),
-                  end_date=UTCDateTime("2599-12-31T12:23:34.5"))
-
-        non_extras_keys = {'code', 'long_name', 'channels', 'start_date',
-                           'end_date'}
-
-        sta.channels = []
-
-        for cha in stn['channels']:
-
-            response = None
-            if stn['nrl_sensor_keys']:
-                sensor_keys = [key.strip() for key in
-                               stn['nrl_sensor_keys'].split(',')]
-                response = nrl.get_sensor_response(sensor_keys)
-
-            elif stn['motion'].upper() == 'ACCELERATION':
-                response = accelerometer_response(stn['resonance_frequency'],
-                                                  stn['gain'])
-
-            elif stn['motion'].upper() == 'VELOCITY':
-                response = geophone_response(stn['resonance_frequency'],
-                                             stn['gain'],
-                                             damping=stn['damping'],
-                                             output_resistance=stn[
-                                                 'coil_resistance'],
-                                             cable_length=stn['cable_length'],
-                                             cable_capacitance=stn['c'])
-            else:
-                print("Unknown motion=[%s]" % stn['motion'])
-                exit()
-
-            channel_code = f'{stn["channel_base_code"].upper()}' \
-                           f'{cha["cmp"].upper()}'
-
-            channel = Channel(code=channel_code,  # required
-                              location_code=f'{stn["location_code"]:02d}',
-                              # required
-                              latitude=0.,  # required
-                              longitude=0.,  # required
-                              elevation=0.,  # required
-                              depth=0.,  # required
-                              start_date=UTCDateTime("1999-12-31T12:23:34.5"),
-                              end_date=UTCDateTime("2599-12-31T12:23:34.5"),
-                              azimuth=0,
-                              dip=0,
-                              response=response)
-
-            sta.channels.append(channel)
-
-            channel.x = cha['x']
-            channel.y = cha['y']
-            channel.z = cha['z']
-            channel.set_orientation(cha['orientation'])
-            channel.alternative_code = stn['code']
-
-        return sta
-
     def __setattr__(self, key, value):
         if key in self.extra_keys:
             if not hasattr(self, 'extra'):
                 self.extra = {}
 
             self.extra[key] = {'value': value, 'namespace': ns}
         else:
@@ -1029,19 +1063,55 @@
                          'from latitude-longitude to UTM')
 
     if type(path_or_file_object) is Path:
         path_or_file_object = str(path_or_file_object)
 
     # del kwargs['xy_from_lat_lon']
 
-    obspy_inv = inventory.read_inventory(str(path_or_file_object),
-                                         format=format,
-                                         *args, **kwargs)
-
-    return Inventory.from_obspy_inventory_object(obspy_inv,
-                    xy_from_lat_lon=xy_from_lat_lon,
-                    output_projection=output_projection,
-                    input_projection=input_projection)
+    if (format not in ENTRY_POINTS['inventory'].keys()) or \
+            (format.upper() == 'STATIONXML'):
+
+        obspy_inv = inventory.read_inventory(str(path_or_file_object),
+                                             format=format,
+                                             *args, **kwargs)
+
+        return Inventory.from_obspy_inventory_object(obspy_inv,
+                                        xy_from_lat_lon=xy_from_lat_lon,
+                                        output_projection=output_projection,
+                                        input_projection=input_projection)
+
+    else:
+        format_ep = ENTRY_POINTS['inventory'][format]
+
+        read_format = load_entry_point(format_ep.dist.key,
+                                       'obspy.io.%s' %
+                                       format_ep.name, 'readFormat')
+
+        # kwargs_obspy = kwargs.copy()
+        # kwargs_obspy.pop('xy_from_lat_lon')
+        # kwargs_obspy.pop('input_projection')
+        # kwargs_obspy.pop('output_projection')
+
+        return read_format(str(path_or_file_object), **kwargs)
+
+    # else:
+
+
+# def read_inventory(filename, format='STATIONXML', **kwargs):
+#     if isinstance(filename, Path):
+#         filename = str(filename)
+#
+#     if format in ENTRY_POINTS['inventory'].keys():
+#         format_ep = ENTRY_POINTS['inventory'][format]
+#         read_format = load_entry_point(format_ep.dist.key,
+#                                        'obspy.plugin.inventory.%s' %
+#                                        format_ep.name, 'readFormat')
+#
+#         return Inventory(inventory=read_format(filename, **kwargs))
+#
+#     else:
+#         return inventory.read_inventory(filename, format=format,
+#                                                **kwargs)
 
 
 read_inventory.__doc__ = inventory.read_inventory.__doc__.replace(
     'obspy', ns)
```

### Comparing `uquake-1.0.3/uquake/core/stream.py` & `uquake-1.2.4/uquake/core/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,17 +438,21 @@
 
 def read(filename, format='MSEED', **kwargs):
     if isinstance(filename, Path):
         filename = str(filename)
 
     if format in ENTRY_POINTS['waveform'].keys():
         format_ep = ENTRY_POINTS['waveform'][format]
-        read_format = load_entry_point(format_ep.dist.key,
-                                       'obspy.plugin.waveform.%s' %
-                                       format_ep.name, 'readFormat')
+        try:
+            read_format = load_entry_point(format_ep.dist.key,
+                                           'uquake.io.waveform.%s' %
+                                           format_ep.name, 'readFormat')
+        except Exception as e:
+            return Stream(
+                stream=obsstream.read(filename, format=format, **kwargs))
 
         st = Stream(stream=read_format(filename, **kwargs))
 
         # making sure the channel names are upper case
         trs = []
         for tr in st:
             tr.stats.channel = tr.stats.channel.upper()
```

### Comparing `uquake-1.0.3/uquake/core/trace.py` & `uquake-1.2.4/uquake/core/trace.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/core/util/base.py` & `uquake-1.2.4/uquake/core/util/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # appending elements to the obspy ENTRY_POINTS
 ENTRY_POINTS['grid'] = _get_entry_points('uquake.io.grid', 'readFormat')
 ENTRY_POINTS['grid_write'] = _get_entry_points('uquake.io.grid',
                                                'writeFormat')
 
 gfr_entry_points = _get_entry_points('uquake.io.waveform', 'readFormat')
-gfw_entry_points = _get_entry_points('uquake.io.waveform', 'writeformat')
+gfw_entry_points = _get_entry_points('uquake.io.waveform', 'writeFormat')
 
 wf_entry_points = _get_entry_points('uquake.io.waveform', 'readFormat')
 
 for key in wf_entry_points.keys():
     ENTRY_POINTS['waveform'][key] = wf_entry_points[key]
 
 wfw_entry_points = _get_entry_points('uquake.io.waveform', 'writeFormat')
@@ -22,14 +22,18 @@
     ENTRY_POINTS['waveform_write'][key] = wfw_entry_points[key]
 
 evt_entry_points = _get_entry_points('uquake.io.event', 'readFormat')
 
 for key in evt_entry_points.keys():
     ENTRY_POINTS['event'][key] = evt_entry_points[key]
 
+invr_entry_points = _get_entry_points('uquake.io.inventory', 'readFormat')
+for key in invr_entry_points.keys():
+    ENTRY_POINTS['inventory'][key] = invr_entry_points[key]
+
 
 def proc(cmd, cwd='.', silent=True):
     from ..logging import logger
 
     try:
         if silent:
             cmd = '%s > /dev/null 2>&1' % cmd
@@ -56,19 +60,19 @@
 
 
 def np_array(arr):
     new_arr = np.empty(shape=(len(arr),), dtype=object)
 
     for i, el in enumerate(arr):
         new_arr[i] = el
-
+    plugin_
     return new_arr
 
 
-def _read_from_plugin(plugin_type, filename, format=None, **kwargs):
+def _read_from_plugin(type, filename, format=None, **kwargs):
     """
     Reads a single file from a plug-in's readFormat function.
     """
     eps = ENTRY_POINTS[plugin_type]
     # get format entry point
     format_ep = None
```

### Comparing `uquake-1.0.3/uquake/core/util/decorator.py` & `uquake-1.2.4/uquake/core/util/decorator.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/core/util/tools.py` & `uquake-1.2.4/uquake/core/util/tools.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/grid/base.py` & `uquake-1.2.4/uquake/grid/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         :type dimensions: tuple
         :param spacing: spacing between the grid nodes
         :type spacing: float
         :param val: constant value with which to fill the grid
         """
 
         data = np.ones(tuple(dimensions)) * val
-        cls.grid = cls.__init__(data, spacing=spacing, origin=origin)
+        cls.grid = cls(data, spacing=spacing, origin=origin)
 
     @classmethod
     def from_ocs(cls, origin, corner, spacing, val=0):
         """
         create a grid from origin, corner and spacing
         :param origin: grid origin (e.g., lower left corner for 2D grid)
         :type origin: tuple or list or numpy.array
@@ -139,35 +139,35 @@
         :type spacing: float
         :param val: constant value with which to fill the grid
         :param buf: buffer around the grid in fraction of grid size
         """
         origin2 = origin
         corner2 = corner
 
-        gshape = tuple([int(np.ceil((c - o) / spacing))
-                        for o, c in zip(origin2, corner2)])
+        gshape = tuple([int(np.ceil((c - o) / s))
+                        for o, c, s in zip(origin2, corner2, spacing)])
         data = np.ones(gshape) * val
-        cls.__init__(data, spacing=spacing, origin=origin)
-        cls.fill_homogeneous(val)
-        return cls
+        out = cls(data, spacing=spacing, origin=origin)
+        out.fill_homogeneous(val)
+        return out
 
     @classmethod
     def from_ocd(cls, origin, corner, dimensions, val=0):
         """
         create a grid from origin, corner and dimensions
         :param origin: grid origin (e.g., lower left corner for 2D grid)
         :param corner: grid upper (e.g., upper right corner for 2D grid)
         :param dimensions: grid dimensions
         :param val: constant value with which to fill the grid
         :return:
         """
 
         data = np.ones(dimensions) * val
         spacing = (corner - origin) / (dimensions - 1)
-        cls.__init__(data, spacing, spacing=spacing, origin=origin)
+        cls(data, spacing, spacing=spacing, origin=origin)
         return cls
 
     def __repr__(self):
         repr_str = """
         spacing: %s
         origin : %s
         shape  : %s
@@ -555,15 +555,14 @@
 
     def smooth(self, sigma: np.array, grid_space=False):
         if not grid_space:
             sigma = sigma / self.spacing
 
         self.data = gaussian_filter(self.data, sigma)
 
-
     @property
     def ndim(self):
         return self.data.ndim
 
     @property
     def shape(self):
         return list(self.data.shape)
```

### Comparing `uquake-1.0.3/uquake/grid/hdf5.py` & `uquake-1.2.4/uquake/grid/hdf5.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/grid/nlloc.py` & `uquake-1.2.4/uquake/grid/nlloc.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 
     def __init__(self, data_or_dims, origin, spacing, phase,
                  value=0, grid_type='VELOCITY_METERS',
                  grid_units=__default_grid_units__,
                  float_type="FLOAT", model_id=None):
         """
         :param data_or_dims: data or data dimensions. If dimensions are
-        provided the a homogeneous gris is created with value=value
+        provided the a homogeneous grid is created with value=value
         :param origin: origin of the grid
         :type origin: list
         :param spacing: the spacing between grid nodes
         :type spacing: list
         :param phase: the uquake phase (value 'P' or 'S')
         :type phase: str
         :param value:
@@ -388,14 +388,29 @@
         """
 
         self.write(base_name, destination)
         for ext in self.extensions:
             shutil.move(f'{origin}/{base_name}.{ext}',
                         f'{destination}/{base_name}.{ext}')
 
+    @classmethod
+    def from_ods(cls, origin, dimensions, spacing, phase, val=0):
+        grid = super().from_ods(origin, dimensions, spacing, val=val)
+        return cls_(grid.data, origin, spacing, phase)
+
+    @classmethod
+    def from_ocs(cls, origin, corner, spacing, phase, val=0):
+        grid = super().from_ocs(origin, corner, spacing, val=val)
+        return cls_(grid.data, grid.origin, grid.spacing, phase)
+
+    @classmethod
+    def from_ocd(cls, origin, corner, dimensions, phase, val=0):
+        grid = super().from_ocd(origin, corner, dimensions, val=val)
+        return cls_(grid.data, grid.origin, grid.spacing, phase)
+
     @property
     def model_id(self):
         return self.resource_id
 
 
 class ModelLayer:
     """
@@ -889,14 +904,31 @@
                                                         cpu_utilisation,
                                                         *args, **kwargs)
 
             tt_grid_ensemble += tt_grids
 
         return tt_grid_ensemble
 
+    def to_time(self, seeds, seed_labels, multi_threaded=False, *args, **kwargs):
+        if multi_threaded:
+            return self.to_time_multi_threaded(seeds, seed_labels)
+
+        else:
+            tt_grid_ensemble = TravelTimeEnsemble([])
+            for key in self.keys():
+                for seed, seed_labels in zip(seeds, seed_labels):
+                    tt_grid_ensemble += self[key].to_time(seed, seed_label)
+
+
+    @property
+    def p(self):
+        return self['p']
+
+    def s(self):
+        return self['s']
 
 class SeededGrid(NLLocGrid):
     """
     container for seeded grids (e.g., travel time, azimuth and take off angle)
     """
     __valid_grid_type__ = ['TIME', 'TIME2D', 'ANGLE', 'ANGLE2D']
```

### Comparing `uquake-1.0.3/uquake/imaging/plot.py` & `uquake-1.2.4/uquake/imaging/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.text import Text
 from matplotlib.transforms import offset_copy
 from uquake.core import event
+from datetime import timedelta
+from matplotlib.ticker import ScalarFormatter
 
 from uquake.core.logging import logger
 
 
 def guttenberg_richter(magnitudes, dates, bin_size=0.05, b_range=[-2.0, -0.5],
                        magnitude_type='Moment magnitude', xlim=[-2.0, 1.0],
                        **kwargs):
@@ -27,15 +29,21 @@
     :param xlim: limits of the x axis
     :type xlim: list containing two floats
     """
 
     mag = np.array(magnitudes)
 
     wdt = 15
-    num_years = (np.max(dates) - np.min(dates)) / (24 * 3600 * 365.25)
+    delta = (np.max(dates) - np.min(dates))
+    if isinstance(delta, np.timedelta64):
+        total_seconds = delta.item() * 1e-9
+    else:
+        total_seconds = delta.total_seconds()
+    total_days = total_seconds / (24 * 60 * 60)
+    num_years = total_days / 365.25
 
     bins = np.arange(xlim[0], xlim[1], bin_size)
     hist = np.histogram(mag, bins=bins)
     hist = hist[0][::-1]
     bins = bins[::-1]
     bins = bins[1::]
     cum_hist = hist.cumsum()
@@ -54,20 +62,23 @@
     indices = np.nonzero((bins >= min_mag) & (bins <= max_mag))[0]
     b, a = np.polyfit(bins[indices], log_cum_sum[indices], 1)
 
     mg = np.arange(min_mag, max_mag, 0.1)
     fitmg = b * mg + a
 
     # Tracer()()
-    plt.semilogy(bins, new_cum_yearly_rate, 'k.', **kwargs)
-    plt.semilogy(mg, 10 ** fitmg, 'k--',
+    plt.clf()
+    fig, ax = plt.subplots()
+    ax.semilogy(bins, new_cum_yearly_rate, 'k.', **kwargs)
+    ax.semilogy(mg, 10 ** fitmg, 'k--',
                  label='best fit ($%0.1f\,M_w + %0.1f$)' % (b, a), **kwargs)
     plt.xlabel('%s' % magnitude_type)
     plt.ylabel('Number of events/year')
     plt.xlim(xlim)
+    ax.yaxis.set_major_formatter(ScalarFormatter())
     plt.legend()
 
 
 # ylim = plt.ylim()
 # plt.ylim([0, 10**0])
 
 # plt.show()
```

### Comparing `uquake-1.0.3/uquake/imaging/stereonet.py` & `uquake-1.2.4/uquake/imaging/stereonet.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/imaging/waveform.py` & `uquake-1.2.4/uquake/imaging/waveform.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/io/event/core.py` & `uquake-1.2.4/uquake/io/event/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/io/grid/core.py` & `uquake-1.2.4/uquake/io/grid/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/io/waveform/core.py` & `uquake-1.2.4/uquake/io/waveform/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,88 +115,101 @@
     for k, dt in enumerate(data.T):
         stats.channel = '%s' % (component[k])
         traces.append(Trace(data=np.array(dt), header=stats))
 
     return Stream(traces=traces)
 
 
+# def write_ims_ascii(stream, filename, **kwargs):
+#     """
+#     write IMS ASCII format
+#     :param stream: data stream
+#     :type stream: ~uquake.core.Stream.stream
+#     :param filename: filename/path
+#     :type filename: str
+#     """
+#
+#
+#     for tr in stream:
+#
+#         decimated_sampling = tr.stats.sampling_rate
+#         sampling_rate = tr.stats.sampling_rate
+#         decimation_factor = 0
+#         trigger_time = tr.stats.starttime.datetime.timestamp
+#         trigger_time_second = np.floor(trigger_time)
+#         trigger_time_usecond = (trigger_time - trigger_time_second) * 1e6
+#
+#     header_line = f'x_24,{decimated_sampling},{sampling_rate},' \
+#                   f'{decimation_factor},100.0,{trigger_time_second},' \
+#                   f'{trigger_time_usecond},0,}'
+#
+#
+#
+
+
 @uncompress
-def read_ESG_SEGY(fname, site=None, **kwargs):
+def read_ESG_SEGY(fname, inventory=None, **kwargs):
     """
     read data produced by ESG and turn them into a valid stream with network,
     station and component information properly filled
     :param fname: the filename
-    :param site: a site object containing site information
-    :type site: ~uquake.core.station.Site
+    :param inventory: a site object containing site information
+    :type inventory: ~uquake.core.inventory.Inventory
     :return: ~uquake.core.stream.Stream
     """
 
-    if not site:
-        logger.warning('A site object should be provided for the information '
-                       'on the system to be properly added to the traces '
-                       'header. The file will be read but information such as '
-                       'the site, network, station or component information '
-                       'will not be appended')
-
-        return read(fname, format='SEGY', unpack_trace_headers=True)
-
-    st = read(fname, format='SEGY', unpack_trace_headers=True)
-
-    stations = site.stations()
-    traces = []
-
-    for k, tr in enumerate(st):
-        x = tr.stats.segy.trace_header.group_coordinate_x
-        y = tr.stats.segy.trace_header.group_coordinate_y
-
-        hdist_min = 1e10
-        station = None
-        network = None
-
-        for net in site:
-            for sta in net:
-                hdist = np.linalg.norm([sta.x - x, sta.y - y])
-
-                if hdist < hdist_min:
-                    hdist_min = hdist
-                    station = sta
-                    network = net
-
-        tr.stats.station = station.code
-        tr.stats.network = network.code
-        traces.append(Trace(trace=tr))
+    if inventory is None:
+        return
 
-    st2 = Stream(traces=traces)
-    traces = []
+    st = read(fname, format='SEGY', unpack_trace_headers=True, **kwargs)
 
-    for station in site.stations():
-        if np.all(station.loc == [1000, 1000, 1000]):
+    trs = []
+    missed_traces = 0
+    for tr in st:
+        tr_y = tr.stats.segy.trace_header.group_coordinate_x
+        tr_x = tr.stats.segy.trace_header.group_coordinate_y
+
+        h_distances = []
+        sites = inventory.networks[0].sites
+
+        component = np.abs(tr.stats.segy.trace_header.trace_identification_code
+                           - 14)
+
+        if component == 13:
+            component = 0
+
+        for site in inventory.networks[0].sites:
+            h_distance = np.linalg.norm([site.x - tr_x, site.y - tr_y])
+            h_distances.append(h_distance)
+        if np.min(h_distances) > 1:
+            missed_traces += 1
             continue
-        sttmp = st2.copy().select(station=station.code)
 
-        for k, tr in enumerate(sttmp):
-            if k == 0:
-                if len(sttmp) == 3:
-                    tr.stats.channel = 'X'
-                else:
-                    tr.stats.channel = 'Z'
-            elif k == 1:
-                tr.stats.channel = 'Y'
-            else:
-                tr.stats.channel = 'Z'
+        i = np.argmin(h_distances)
+        site = sites[i]
 
-            msec_starttime = tr.stats.segy.trace_header.lag_time_A
-            usec_starttime = tr.stats.segy.trace_header.lag_time_B
+        channel_code = f'{site.channels[0].code[0:2]}{component:0.0f}'
 
-            usecs = msec_starttime / 1000. + usec_starttime / 1.0e6
-            tr.stats.starttime = tr.stats.starttime + usecs
+        tr_stats = Stats()
+        tr_stats.network = network
+        tr_stats.station = site.station.code
+        tr_stats.location = site.location_code
+        tr_stats.channel = channel_code
+        tr_stats.sampling_rate = tr.stats.sampling_rate
 
-            traces.append(Trace(trace=tr))
+        msec_starttime = tr.stats.segy.trace_header.lag_time_A
+        usec_starttime = tr.stats.segy.trace_header.lag_time_B
 
-    return Stream(traces=traces)
+        usecs = msec_starttime / 1000. + usec_starttime / 1.0e6
+        tr_stats.starttime = tr.stats.starttime + usecs
+        tr_stats.npts = len(tr.data)
+
+        trs.append(Trace(data=tr.data, header=tr_stats))
+
+    return Stream(traces=trs)
 
 
 @uncompress
 def read_TEXCEL_CSV(filename, **kwargs):
     """
     Reads a texcel csv file and returns a uquake Stream object.
```

### Comparing `uquake-1.0.3/uquake/nlloc/nlloc.py` & `uquake-1.2.4/uquake/nlloc/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/amp_measures.py` & `uquake-1.2.4/uquake/waveform/amp_measures.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/mag.py` & `uquake-1.2.4/uquake/waveform/mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/mag_utils.py` & `uquake-1.2.4/uquake/waveform/mag_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/parseval_utils.py` & `uquake-1.2.4/uquake/waveform/parseval_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/pick.py` & `uquake-1.2.4/uquake/waveform/pick.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/simple_mag.py` & `uquake-1.2.4/uquake/waveform/simple_mag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,20 +1177,20 @@
             # filter the pulse using the corner frequency of the sensor
 
             sensor_min_freq = np.min(poles) / (2 * np.pi)
             window_min_freq = 1 / win_length
 
             low_bp_freq = np.max([sensor_min_freq, window_min_freq])
             high_bp_freq = np.max(poles) / (2 * np.pi)
-            if high_bp_freq > pulse[0].stats.sampling_rate / 2:
-                high_bp_freq = pulse[0].stats.sampling_rate / 2.5
+            # if high_bp_freq > pulse[0].stats.sampling_rate / 2:
+            #     high_bp_freq = pulse[0].stats.sampling_rate / 2.5
 
             high_bp_freq = max_frequency
             pulse = pulse.taper(max_percentage=0.05, type='cosine')
-            pulse.filter('bandpass', freqmin=low_bp_freq, freqmax=high_bp_freq)
+            # pulse.filter('bandpass', freqmin=low_bp_freq, freqmax=high_bp_freq)
             low_bp_freq1 = 10 ** (np.log10(low_bp_freq) - 0.2)
             low_bp_freq2 = low_bp_freq
             high_bp_freq1 = high_bp_freq
             high_bp_freq2 = 10 ** (np.log10(high_bp_freq) + 0.2)
             pre_filt = [low_bp_freq1, low_bp_freq2, high_bp_freq1,
                         high_bp_freq2]
             pulse.attach_response(inventory)
```

### Comparing `uquake-1.0.3/uquake/waveform/smom_measure.py` & `uquake-1.2.4/uquake/waveform/smom_measure.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/smom_measure_legacy.py` & `uquake-1.2.4/uquake/waveform/smom_measure_legacy.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/uquake/waveform/transforms.py` & `uquake-1.2.4/uquake/waveform/transforms.py`

 * *Files identical despite different names*

### Comparing `uquake-1.0.3/setup.py` & `uquake-1.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
  'uquake.core',
  'uquake.core.util',
  'uquake.grid',
  'uquake.imaging',
  'uquake.io',
  'uquake.io.event',
  'uquake.io.grid',
+ 'uquake.io.inventory',
  'uquake.io.waveform',
  'uquake.nlloc',
  'uquake.waveform']
 
 package_data = \
 {'': ['*']}
 
@@ -43,42 +44,41 @@
  'uquake.io.grid.CSV': ['readFormat = uquake.io.grid:read_csv',
                         'writeFormat = uquake.io.grid:write_csv'],
  'uquake.io.grid.NLLOC': ['readFormat = uquake.io.grid:read_nlloc'],
  'uquake.io.grid.PICKLE': ['readFormat = uquake.io.grid:read_pickle',
                            'writeFormat = uquake.io.grid:write_pickle'],
  'uquake.io.grid.VTK': ['readFormat = uquake.io.grid:read_vtk',
                         'writeFormat = uquake.io.grid:write_vtk'],
- 'uquake.io.site.CSV': ['readFormat = uquake.io.site:read_csv',
-                        'writeFormat = uquake.io.site:write_csv'],
- 'uquake.io.site.PICKLE': ['readFormat = uquake.io.site:read_pickle',
-                           'writeFormat = uquake.io.site:write_pickle'],
+ 'uquake.io.inventory': ['ESG_SENSOR = uquake.io.inventory'],
+ 'uquake.io.inventory.ESG_SENSOR': ['readFormat = '
+                                    'uquake.io.inventory:read_esg_sensor_file'],
  'uquake.io.waveform': ['ESG_SEGY = uquake.io.waveform',
-                        'HSF = micorquake.io.waveform',
+                        'HSF = uquake.io.waveform',
                         'IMS_ASCII = uquake.io.waveform',
                         'IMS_CONTINUOUS = uquake.io.waveform',
                         'TEXCEL_CSV = uquake.io.waveform'],
  'uquake.io.waveform.ESG_SEGY': ['readFormat = '
                                  'uquake.io.waveform:read_ESG_SEGY'],
  'uquake.io.waveform.IMS_ASCII': ['readFormat = '
                                   'uquake.io.waveform:read_IMS_ASCII'],
  'uquake.io.waveform.TEXCEL_CSV': ['readFormat = '
                                    'uquake.io.waveform:read_TEXCEL_CSV']}
 
 setup_kwargs = {
     'name': 'uquake',
-    'version': '1.0.3',
+    'version': '1.2.4',
     'description': 'extension of the ObsPy library for local seismicity',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'uQuake development team',
     'author_email': 'dev@uQuake.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.10',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `uquake-1.0.3/PKG-INFO` & `uquake-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: uquake
-Version: 1.0.3
+Version: 1.2.4
 Summary: extension of the ObsPy library for local seismicity
 License: MIT
 Author: uQuake development team
 Author-email: dev@uQuake.org
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.4,<4.0.0)
 Requires-Dist: future (>=0.18.2,<0.19.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: jedi (==0.17.2)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: numpy (>=1.18.0,<2.0.0)
 Requires-Dist: obspy (>=1.2.2,<2.0.0)
```

