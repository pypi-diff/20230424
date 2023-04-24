# Comparing `tmp/weatherly-0.2.0-py3.11.egg` & `tmp/weatherly-0.3.0-py3.10.egg`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 40223 bytes, number of entries: 24
--rw-rw-rw-  2.0 fat     3022 b- defN 23-Apr-21 08:50 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      383 b- defN 23-Apr-21 08:50 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-21 08:50 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat       39 b- defN 23-Apr-21 08:50 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-21 08:50 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-21 08:50 EGG-INFO/zip-safe
--rw-rw-rw-  2.0 fat      813 b- defN 23-Apr-21 08:47 weatherly/__init__.py
--rw-rw-rw-  2.0 fat     5297 b- defN 23-Apr-21 08:27 weatherly/abc.py
--rw-rw-rw-  2.0 fat     4647 b- defN 23-Apr-17 09:10 weatherly/enums.py
--rw-rw-rw-  2.0 fat     3854 b- defN 23-Apr-21 08:18 weatherly/errors.py
--rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-21 08:25 weatherly/responses.py
--rw-rw-rw-  2.0 fat     2855 b- defN 23-Apr-21 08:41 weatherly/utils.py
--rw-rw-rw-  2.0 fat     1359 b- defN 23-Apr-21 08:50 weatherly/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat     6514 b- defN 23-Apr-21 08:50 weatherly/__pycache__/abc.cpython-311.pyc
--rw-rw-rw-  2.0 fat     5906 b- defN 23-Apr-21 08:50 weatherly/__pycache__/enums.cpython-311.pyc
--rw-rw-rw-  2.0 fat     5249 b- defN 23-Apr-21 08:50 weatherly/__pycache__/errors.cpython-311.pyc
--rw-rw-rw-  2.0 fat     8392 b- defN 23-Apr-21 08:50 weatherly/__pycache__/responses.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3648 b- defN 23-Apr-21 08:50 weatherly/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-  2.0 fat     1258 b- defN 23-Apr-17 09:10 weatherly/api/__init__.py
--rw-rw-rw-  2.0 fat     9793 b- defN 23-Apr-21 08:45 weatherly/api/client.py
--rw-rw-rw-  2.0 fat     2752 b- defN 23-Apr-21 08:18 weatherly/api/core.py
--rw-rw-rw-  2.0 fat     1419 b- defN 23-Apr-21 08:50 weatherly/api/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat    11907 b- defN 23-Apr-21 08:50 weatherly/api/__pycache__/client.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3661 b- defN 23-Apr-21 08:50 weatherly/api/__pycache__/core.cpython-311.pyc
-24 files, 89590 bytes uncompressed, 36943 bytes compressed:  58.8%
+Zip file size: 47123 bytes, number of entries: 24
+-rw-rw-r--  2.0 unx     2958 b- defN 23-Apr-24 22:40 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx      383 b- defN 23-Apr-24 22:40 EGG-INFO/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-24 22:40 EGG-INFO/dependency_links.txt
+-rw-rw-r--  2.0 unx       64 b- defN 23-Apr-24 22:40 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-24 22:40 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 22:40 EGG-INFO/zip-safe
+-rw-r--r--  2.0 unx      783 b- defN 23-Apr-24 22:37 weatherly/__init__.py
+-rw-rw-r--  2.0 unx    15185 b- defN 23-Apr-24 21:44 weatherly/abc.py
+-rw-rw-r--  2.0 unx     4488 b- defN 23-Apr-16 23:05 weatherly/enums.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Apr-23 21:25 weatherly/errors.py
+-rw-rw-r--  2.0 unx    21609 b- defN 23-Apr-24 21:47 weatherly/responses.py
+-rw-rw-r--  2.0 unx     2762 b- defN 23-Apr-22 23:27 weatherly/utils.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-24 22:40 weatherly/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx    16172 b- defN 23-Apr-24 22:40 weatherly/__pycache__/abc.cpython-310.pyc
+-rw-r--r--  2.0 unx     5124 b- defN 23-Apr-24 22:40 weatherly/__pycache__/enums.cpython-310.pyc
+-rw-r--r--  2.0 unx     4342 b- defN 23-Apr-24 22:40 weatherly/__pycache__/errors.cpython-310.pyc
+-rw-r--r--  2.0 unx    20450 b- defN 23-Apr-24 22:40 weatherly/__pycache__/responses.cpython-310.pyc
+-rw-r--r--  2.0 unx     2897 b- defN 23-Apr-24 22:40 weatherly/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--  2.0 unx     1228 b- defN 23-Apr-16 21:16 weatherly/api/__init__.py
+-rw-rw-r--  2.0 unx    12850 b- defN 23-Apr-24 21:52 weatherly/api/client.py
+-rw-rw-r--  2.0 unx     2657 b- defN 23-Apr-23 21:24 weatherly/api/core.py
+-rw-r--r--  2.0 unx     1388 b- defN 23-Apr-24 22:40 weatherly/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx    12258 b- defN 23-Apr-24 22:40 weatherly/api/__pycache__/client.cpython-310.pyc
+-rw-r--r--  2.0 unx     3003 b- defN 23-Apr-24 22:40 weatherly/api/__pycache__/core.cpython-310.pyc
+24 files, 135398 bytes uncompressed, 43843 bytes compressed:  67.6%
```

## zipnote «TEMP»/diffoscope_2q64d1ry_/tmpdcii7y4w_.zip

```diff
@@ -30,44 +30,44 @@
 
 Filename: weatherly/responses.py
 Comment: 
 
 Filename: weatherly/utils.py
 Comment: 
 
-Filename: weatherly/__pycache__/__init__.cpython-311.pyc
+Filename: weatherly/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/__pycache__/abc.cpython-311.pyc
+Filename: weatherly/__pycache__/abc.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/__pycache__/enums.cpython-311.pyc
+Filename: weatherly/__pycache__/enums.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/__pycache__/errors.cpython-311.pyc
+Filename: weatherly/__pycache__/errors.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/__pycache__/responses.cpython-311.pyc
+Filename: weatherly/__pycache__/responses.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/__pycache__/utils.cpython-311.pyc
+Filename: weatherly/__pycache__/utils.cpython-310.pyc
 Comment: 
 
 Filename: weatherly/api/__init__.py
 Comment: 
 
 Filename: weatherly/api/client.py
 Comment: 
 
 Filename: weatherly/api/core.py
 Comment: 
 
-Filename: weatherly/api/__pycache__/__init__.cpython-311.pyc
+Filename: weatherly/api/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/api/__pycache__/client.cpython-311.pyc
+Filename: weatherly/api/__pycache__/client.cpython-310.pyc
 Comment: 
 
-Filename: weatherly/api/__pycache__/core.cpython-311.pyc
+Filename: weatherly/api/__pycache__/core.cpython-310.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,74 +1,77 @@
-Metadata-Version: 2.1
-Name: weatherly
-Version: 0.2.0
-Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
-Home-page: https://github.com/konradsic/weatherly
-Author: konradsic
-License: MIT
-Project-URL: Issues, https://github.com/konradsic/weatherly/issues
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Classifier: Typing :: Typed
-Requires-Python: >=3.10.0
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-License-File: LICENSE
-
-⛅ weatherly
-====================
-.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
-    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
-    :alt: Weatherly license
-.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Weatherly version on PyPI
-.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
-    :target: https://pypi.python.org/project/weatherly
-    :alt: Supported Python versions
-.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
-    :target: https://github.com/konradsic/weatherly
-    :alt: Build status
-
-Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
-
-📜 Features
----------------
-* Easy to use,
-* Intuitive design,
-* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
-* Modern and typed Python package,
-* Support for languages (provided by WeatherAPI)
-
-💻 Code example
----------------------
-
-.. code:: python
-
-    import weatherly
-    
-    client = weatherly.WeatherAPIClient(api_key="your WeatherAPi key")
-    # you can set language to all request, or pass it manually
-    client.set_language("fr")     # lang code
-    client.set_language("German") # language full name
-
-    # getting weather info
-    current_weather = client.get_current_weather(query="London")
-
-    # getting forecast info
-    forecast = client.get_forecast_data(query="Paris")
-
-    # historical data
-    history = client.get_historical_data(query="48.8567,2.3508") # query could also be latitude,longitude
-
-    # marine data
-    marine = client.get_marine_data(query="Madrid")
+Metadata-Version: 2.1
+Name: weatherly
+Version: 0.3.0
+Summary: A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more...
+Home-page: https://github.com/konradsic/weatherly
+Author: konradsic
+License: MIT
+Project-URL: Issues, https://github.com/konradsic/weatherly/issues
+Platform: UNKNOWN
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Classifier: Typing :: Typed
+Requires-Python: >=3.10.0
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+License-File: LICENSE
+
+⛅ weatherly
+====================
+.. image:: https://img.shields.io/github/license/konradsic/weatherly?color=blue&style=for-the-badge
+    :target: https://github.com/konradsic/weatherly/blob/master/LICENSE
+    :alt: Weatherly license
+.. image:: https://img.shields.io/pypi/v/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Weatherly version on PyPI
+.. image:: https://img.shields.io/pypi/pyversions/weatherly?color=blue&style=for-the-badge
+    :target: https://pypi.python.org/project/weatherly
+    :alt: Supported Python versions
+.. image:: https://img.shields.io/github/actions/workflow/status/konradsic/weatherly/build.yml?style=for-the-badge
+    :target: https://github.com/konradsic/weatherly
+    :alt: Build status
+
+Weatherly is a simple package that retrieves weather data from WeatherAPI.com. It provides an easy to use interface to access current and historical weather data for a specific location.
+
+📜 Features
+---------------
+* Easy to use,
+* Intuitive design,
+* Can provide current weather data aswell as forecast, historical data, future predictions and even more!
+* Modern and typed Python package,
+* Support for languages (provided by WeatherAPI)
+
+💻 Code example
+---------------------
+
+.. code:: python
+
+    import weatherly
+    
+    client = weatherly.Client(api_key="your WeatherAPI key")
+    # you can set language to all request, or pass it manually
+    client.set_language("fr")     # lang code
+    client.set_language("German") # language full name
+
+    # getting weather info
+    current_weather = client.get_current_weather(query="London")
+
+    # getting forecast info
+    forecast = client.get_forecast_data(query="Paris")
+
+    # historical data
+    history = client.get_historical_data(query="48.8567,2.3508") # query could also be latitude,longitude
+
+    # marine data
+    marine = client.get_marine_data(query="Madrid")
+
+
```

## EGG-INFO/requires.txt

```diff
@@ -1,4 +1,5 @@
 requests==2.28.2
 
 [docs]
 sphinx==5.3.0
+sphinx_book_theme==1.0.1
```

## EGG-INFO/zip-safe

```diff
@@ -1 +1 @@
-00000000: 0d0a                                     ..
+00000000: 0a                                       .
```

## weatherly/__init__.py

```diff
@@ -1,35 +1,34 @@
-"""
-weatherly
-===============
-A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more.
-
-:copyright: (c) 2023-present @konradsic
-:license: MIT license, see LICENSE for details
-"""
-
-__title__ = 'weatherly'
-__author__ = 'konradsic'
-__license__ = 'MIT'
-__copyright__ = 'Copyright 2023-present konradsic'
-__version__ = '0.2.0'
-
-from typing import NamedTuple, Literal
-
-from .api import *
-from .errors import *
-from .enums import *
-from .responses import *
-from . import (
-    utils as utils
-)
-
-class VersionInfo(NamedTuple):
-    major: int
-    minor: int
-    micro: int
-    release_type: Literal["alpha", "beta", "pre", "final"]
-    
-version_info = VersionInfo(major=0, minor=2, micro=0, release_type="final")
-
-
-del NamedTuple, Literal, VersionInfo
+"""
+weatherly
+===============
+A simple Python wrapper around WeatherAPI. Get current weather, forecast, history and more.
+
+:copyright: (c) 2023-present @konradsic
+:license: MIT license, see LICENSE for details
+"""
+
+__title__ = 'weatherly'
+__author__ = 'konradsic'
+__license__ = 'MIT'
+__copyright__ = 'Copyright 2023-present konradsic'
+__version__ = '0.3.0'
+
+from typing import NamedTuple, Literal
+
+from .api import *
+from .errors import *
+from .enums import *
+from .responses import *
+from . import (
+    utils as utils
+)
+
+class VersionInfo(NamedTuple):
+    major: int
+    minor: int
+    micro: int
+    release_type: Literal["alpha", "beta", "candidate", "final"]
+    
+version_info = VersionInfo(major=0, minor=3, micro=0, release_type="final")
+
+del NamedTuple, Literal, VersionInfo
```

## weatherly/abc.py

```diff
@@ -1,161 +1,514 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from typing import (
-    Any,
-    Literal,
-    Dict,
-    Optional
-)
-from abc import ABC
-
-__all__ = (
-    "ResponseModel",
-    "CurrentWeather",
-)
-
-class ResponseModel(ABC):
-    """
-    ResponseModel is an ABC that defines a basic response model from WeatherAPI.
-    Almost all models inherit from this class.
-    
-    Attributes
-    ----------
-    raw: Dict[:class:`str`, Any]
-        Raw response in a JSON-like format (converted to a python dictionary)
-    status: :class:`int`
-        HTTP status of the response. 200 is OK, and is the most common status.
-    code: Union[:class:`int`, None]
-        Response code. In some cases this can be ``None``
-    """
-    raw: Dict[str, Any]
-    status: int
-    code: int | None
-
-class CurrentWeather(ResponseModel):
-    """
-    An ABC defining current weather data.
-
-    The following classes implement this ABC:
-    - :class:`~weatherly.CurrentWeatherData`
-
-    Attributes
-    ------------
-    location: :class:`~weatherly.LocationData`
-        Location of the requested weather data
-    last_updated_epoch: :class:`int`
-        The timestamp when the weather data was last updated.
-    temp_c: :class:`float`
-        Weather temperature in Celsius
-    temp_f: :class:`float`
-        Weather temperature in Fahrenheit
-    is_day: :class:`bool`
-        Wherever the current time is considered day time.
-    condition_text: :class:`str`
-        Weather condition text
-    condition_icon: :class:`str`
-        Link to the weather condition icon
-    condition_code: :class:`int`
-        Code of current weather condition
-    wind_mph: :class:`float`
-        Current wind speed in miles per hour (mph)
-    wind_kph: :class:`float`
-        Current wind speed in kilometers per hour (kph)
-    wind_degree: :class:`int`
-        Direction of wind in degrees
-    wind_dir: :class:`str`
-        Direction of wind as a string (e.g. "W")
-    pressure_mb: :class:`float`
-        Pressure in millibars (mb)
-    pressure_in: :class:`float`
-        Pressure in inches (in)
-    precip_mm: :class:`float`
-        Precipation (water that is falling out of the sky) in millimeters (mm)
-    precip_in: :class:`float`
-        Precipation (water that is falling in the sky) in inches (in)
-    humidity: :class:`int`
-        Humidity in integer percentage
-    cloud: :class:`int`
-        Cloud cover as percentage
-    feelslike_c: :class:`float`
-        Feels like temperature in Celsius
-    feelslike_f: :class:`float`
-        Feels like temperature in Fahrenheit
-    uv: :class:`float`
-        UV Index
-    """
-    last_updated_epoch: int
-    temp_c: float
-    temp_f: float
-    is_day: bool
-    condition_text: str
-    condition_icon: str
-    condition_code: int
-    wind_mph: float
-    wind_kph: float
-    wind_degree: int
-    wind_dir: str
-    pressure_mb: float
-    pressure_in: float
-    precip_mm: float
-    precip_in: float
-    humidity: int
-    cloud: int
-    feelslike_c: float
-    feelslike_f: float
-    uv: float
-
-class LocationModel(ResponseModel):
-    """An ABC that provides information about a location
-
-    Attributes
-    --------------
-    id: :class:`int`
-        A specific ID of the location. Can be ``None``
-    name: :class:`str`
-        Name of the location (e.g. London)
-    region: :class:`str`
-        A region of the location
-    country: :class:`str`
-        Country where the location is
-    latitude: :class:`float`
-        Latitude coordinate of the location
-    longitude: :class:`float`
-        Longitude coordinate of the location
-    timezone_id: Optional[:class:`str`]
-        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.
-    localtime_epoch: Optional[:class:`int`]
-        Local time of the location as a timestamp
-    localtime_formatted: Optional[:class:`str`]
-        Formatted local time of the location
-    """
-    id: Optional[int]
-    name: str
-    region: str
-    country: str
-    latitude: float
-    longitude: float
-    timezone_id: Optional[str]
-    localtime_epoch: Optional[int]
-    localtime_formatted: Optional[str]
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import (
+    Any,
+    Literal,
+    Dict,
+    Optional,
+    List
+)
+from abc import ABC
+
+__all__ = (
+    "ResponseModel",
+    "CurrentWeather",
+)
+
+class ResponseModel(ABC):
+    """
+    ResponseModel is an ABC that defines a basic response model from WeatherAPI.
+    Almost all models inherit from this class.
+    
+    Attributes
+    ----------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Union[:class:`int`, None]
+        Response code. In some cases this can be ``None``
+    """
+    raw: Dict[str, Any]
+    status: int
+    code: int | None
+
+class CurrentWeather(ResponseModel):
+    """
+    An ABC defining current weather data.
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.CurrentWeatherData`
+
+    Attributes
+    ------------
+    location: :class:`~weatherly.LocationData`
+        Location of the requested weather data
+    last_updated_epoch: :class:`int`
+        The timestamp when the weather data was last updated.
+    temp_c: :class:`float`
+        Weather temperature in Celsius
+    temp_f: :class:`float`
+        Weather temperature in Fahrenheit
+    is_day: :class:`bool`
+        Wherever the current time is considered day time.
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Link to the weather condition icon
+    condition_code: :class:`int`
+        Code of current weather condition
+    wind_mph: :class:`float`
+        Current wind speed in miles per hour (mph)
+    wind_kph: :class:`float`
+        Current wind speed in kilometers per hour (kph)
+    wind_degree: :class:`int`
+        Direction of wind in degrees
+    wind_dir: :class:`str`
+        Direction of wind as a string (e.g. "W")
+    pressure_mb: :class:`float`
+        Pressure in millibars (mb)
+    pressure_in: :class:`float`
+        Pressure in inches (in)
+    precip_mm: :class:`float`
+        Precipation (water that is falling out of the sky) in millimeters (mm)
+    precip_in: :class:`float`
+        Precipation (water that is falling in the sky) in inches (in)
+    humidity: :class:`int`
+        Humidity in integer percentage
+    cloud: :class:`int`
+        Cloud cover as percentage
+    feelslike_c: :class:`float`
+        Feels like temperature in Celsius
+    feelslike_f: :class:`float`
+        Feels like temperature in Fahrenheit
+    uv: :class:`float`
+        UV Index
+    """
+    location: ResponseModel # should inherit from this, actually its "weatherly.LocationData"
+    last_updated_epoch: int
+    temp_c: float
+    temp_f: float
+    is_day: bool
+    condition_text: str
+    condition_icon: str
+    condition_code: int
+    wind_mph: float
+    wind_kph: float
+    wind_degree: int
+    wind_dir: str
+    pressure_mb: float
+    pressure_in: float
+    precip_mm: float
+    precip_in: float
+    humidity: int
+    cloud: int
+    feelslike_c: float
+    feelslike_f: float
+    uv: float
+
+class LocationModel(ResponseModel):
+    """An ABC that provides information about a location
+    
+    The following classes implement this ABC:
+    - :class:`~weatherly.LocationData`
+
+    Attributes
+    --------------
+    id: :class:`int`
+        A specific ID of the location. Can be ``None``
+    name: :class:`str`
+        Name of the location (e.g. London)
+    region: :class:`str`
+        A region of the location
+    country: :class:`str`
+        Country where the location is
+    latitude: :class:`float`
+        Latitude coordinate of the location
+    longitude: :class:`float`
+        Longitude coordinate of the location
+    timezone_id: Optional[:class:`str`]
+        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.
+    localtime_epoch: Optional[:class:`int`]
+        Local time of the location as a timestamp
+    localtime_formatted: Optional[:class:`str`]
+        Formatted local time of the location
+    """
+    id: Optional[int]
+    name: str
+    region: str
+    country: str
+    latitude: float
+    longitude: float
+    timezone_id: Optional[str]
+    localtime_epoch: Optional[int]
+    localtime_formatted: Optional[str]
+    
+class AirQuality(ResponseModel):
+    """An ABC that provides information about air quality for a specific location.
+    
+    The following classes implement this ABC:
+    - :class:`~weatherly.AirQualityData`
+    
+    Attributes
+    --------------
+    co: :class:`float`
+        Carbon Monoxide (μg/m3)
+    o3: :class`float`
+        Ozone (μg/m3)
+    no2: :class`float`	
+        Nitrogen dioxide (μg/m3)
+    so2: :class`float`
+        Sulphur dioxide (μg/m3)
+    pm2_5: :class`float`
+        PM2.5 (μg/m3)
+    pm10: :class`float`
+        PM10 (μg/m3)
+    us_epa_index: :class`int`
+        US - EPA standard.
+        * 1 means Good
+        * 2 means Moderate
+        * 3 means Unhealthy for sensitive group
+        * 4 means Unhealthy
+        * 5 means Very Unhealthy
+        * 6 means Hazardous
+    gb_defra_index: :class:`int`
+        UK Defra Index
+        
+        +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+        | Index  | 1    | 2     | 3     | 4        | 5        | 6        | 7     | 8     | 9     | 10         |
+        +========+======+=======+=======+==========+==========+==========+=======+=======+=======+============+
+        | Band   | Low  | Low   | Low   | Moderate | Moderate | Moderate | High  | High  | High  | Very High  |
+        +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+        | µgm^-3 | 0-11 | 12-23 | 24-35 | 36-41    | 42-47    | 48-53    | 54-58 | 59-64 | 65-70 | 71 or more |
+        +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+    """
+    co: float
+    o3: float
+    no2: float
+    so2: float
+    pm2_5: float
+    pm10: float
+    us_epa_index: int
+    gb_defra_index: int
+
+class ForecastHourModel(ResponseModel):
+    """
+    An ABC defining a base forecast hour model from WeatherAPI
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.ForecastHour`
+
+    Attributes
+    -------------
+    time_epoch: :class:`int`
+        Time as epoch
+    time: :class:`str`
+        Date and time
+    temp_c: :class:`float`
+        Temperature in celsius
+    temp_f: :class:`float`
+        Temperature in fahrenheit
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icons
+    condition_code: :class:`int`
+        Weather condition code
+    wind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    wind_kph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    wind_degree: :class:`int`
+        Wind direction in degrees
+    wind_dir: :class:`str`
+        Wind direction as 16 point compass. e.g.: NSW
+    pressure_mb: :class:`float`
+        Pressure in millibars
+    pressure_in: :class:`float`
+        Pressure in inches
+    precip_mm: :class:`float`
+        Precipitation amount in millimeters
+    precip_in: :class:`float`
+        Precipitation amount in inches
+    humidity: :class:`int`
+        Humidity as percentage
+    cloud: :class:`int`
+        Cloud cover as percentage
+    feelslike_c: :class:`float`
+        Feels like temperature as celcius
+    feelslike_f: :class:`float`
+        Feels like temperature as fahrenheit
+    windchill_c: :class:`float`
+        Windchill temperature in celcius
+    windchill_f: :class:`float`
+        Windchill temperature in fahrenheit
+    headindex_c: :class:`float`
+        Heat index in celcius
+    headindex_f: :class:`float`
+        Heat index in fahrenheit
+    dewpoint_c: :class:`float`
+        Dew point in celcius
+    dewpoint_f: :class:`float`
+        Dew point in fahrenheit
+    will_it_rain: :class:`bool`
+        Will it will rain or not
+    will_it_snow: :class:`bool`
+        Will it will snow or not
+    is_day: :class:`bool`
+        Whether to show day condition icon or night icon
+    vis_km: :class:`float`
+        Visibility in kilometer
+    vis_miles: :class:`float`
+        Visibility in miles
+    chance_of_rain: :class:`int`
+        Chance of rain as percentage
+    chance_of_snow: :class:`int`
+        Chance of snow as percentage
+    gust_mph: :class:`float`
+        Wind gust in miles per hour
+    gust_kph: :class:`float`
+        Wind gust in kilometer per hour
+    uv: :class:`float`
+        UV Index
+    aqi: Optional[:class:`AirQuality`]
+        Air Quality data. See :class:`AirQualityData` for more info.
+    """
+    time_epoch: int
+    time: str
+    temp_c: float
+    temp_f: float
+    condition_text: str
+    condition_icon: str
+    condition_code: int
+    wind_mph: float
+    wind_kph: float
+    wind_degree: int
+    wind_dir: str
+    pressure_mb: float
+    pressure_in: float
+    precip_mm: float
+    precip_in: float
+    humidity: int
+    cloud: int
+    feelslike_c: float
+    feelslike_f: float
+    windchill_c: float
+    windchill_f: float
+    headindex_c: float
+    headindex_f: float
+    dewpoint_c: float
+    dewpoint_f: float
+    will_it_rain: bool
+    will_it_snow: bool
+    is_day: bool
+    vis_km: float
+    vis_miles: float
+    chance_of_rain: int
+    chance_of_snow: int
+    gust_mph: float
+    gust_kph: float
+    uv: float
+
+    aqi: Optional[AirQuality]
+    
+
+class ForecastDayModel(ResponseModel):
+    """
+    An ABC defining a base forecast day model from WeatherAPI
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.ForecastDay`
+
+    Attributes
+    -------------
+    date: :class:`str`
+        Forecast date
+    date_epoch: :class:`int`
+        Forecast date as unix time.
+    maxtemp_c: :class:`float`
+        Maximum temperature in celsius for the day.
+    maxtemp_f: :class:`float`
+        Maximum temperature in fahrenheit for the day
+    mintemp_c: :class:`float`
+        Minimum temperature in celsius for the day
+    mintemp_f: :class:`float`
+        Minimum temperature in fahrenheit for the day
+    avgtemp_c: :class:`float`
+        Average temperature in celsius for the day
+    avgtemp_f: :class:`float`
+        Average temperature in fahrenheit for the day
+    maxwind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    maxwind_mph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    totalprecip_mm: :class:`float`
+        Total precipitation in milimeter
+    totalprecip_in: :class:`float`
+        Total precipitation in inches
+    avgvis_km: :class:`float`
+        Average visibility in kilometer
+    avgvis_miles: :class:`float`
+        Average visibility in miles
+    avghumidity: :class:`int`
+        Average humidity as percentage
+    uv: :class:`int`
+        UV Index
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icon
+    condition_code: :class:`int`
+        Weather condition code
+    hour_data: List[:class:`ForecastHourModel`]
+        A list of :class:`ForecastHourModel` objects representing hourly weather data.
+    sunrise: :class:`str`
+        Sunrise time
+    sunset: :class:`str`
+        Sunset time
+    moonrise: :class:`str`
+        Moonrise time
+    moonset: :class:`str`
+        Moonset time
+    moon_phase: :class:`str`
+        Moon phases. Value returned:
+        * New Moon
+        * Waxing Crescent
+        * First Quarter
+        * Waxing Gibbous
+        * Full Moon
+        * Waning Gibbous
+        * Last Quarter
+        * Waning Crescent
+    moon_illumination: :class:`float`
+        Moon illumination as %
+    aqi: Optional[:class:`AirQuality`]
+        Air Quality data as :class:`AirQuality` object. Can be ``None``
+    """
+    date: str
+    date_epoch: int
+    # day
+    maxtemp_c: float
+    maxtemp_f: float
+    mintemp_c: float
+    mintemp_f: float
+    avgtemp_c: float
+    avgtemp_f: float
+
+    maxwind_mph: float
+    maxwind_mph: float
+
+    totalprecip_mm: float
+    totalprecip_in: float
+
+    avgvis_km: float
+    avgvis_miles: float
+    avghumidity: int
+    uv: int
+
+    condition_text: str
+    condition_icon: str
+    condition_code: int
+    # astro data
+    sunrise: Optional[str]
+    sunset: Optional[str]
+    moonrise: Optional[str]
+    moonset: Optional[str]
+    moon_phase: Optional[str]
+    moon_illumination: Optional[float]
+    # aqi
+    aqi: Optional[AirQuality]
+
+    hour_data: List[ForecastHourModel]
+
+
+class AlertModel(ResponseModel):
+    """
+    An ABC defining a base alert model from WeatherAPI
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.AlertData`
+
+    Attributes
+    -------------
+    headline: :class:`str`
+        Alert headline
+    msg_type: :class:`str`
+        Type of alert
+    severity: :class:`str`
+        Severity of alert
+    urgency: :class:`str`
+        Urgency
+    areas: :class:`str`
+        Areas covered
+    category: :class:`str`
+        Category
+    certainty: :class:`str`
+        Certainty
+    event: :class:`str`
+        Event
+    note: :class:`str`
+        Note
+    effective: :class:`str`
+        Effective
+    expires: :class:`str`
+        Expires
+    description: :class:`str`
+        Description
+    instruction: :class:`str`
+        Instruction
+    """
+    headline: str
+    msg_type: str
+    severity: str
+    urgency: str
+    areas: str
+    category: str
+    certainty: str
+    event: str
+    note: str
+    effective: str
+    expires: str
+    description: str
+    instruction: str
+
+class ForecastModel(ResponseModel):
+    """
+    An ABC defining a base response from Forecast API.
+
+    The following classes implement this ABC:
+    - :class:`~weatherly.ForecastData`
+    
+    Attributes
+    -------------
+    location: :class:`LocationModel`
+        Location of the forecast data.
+    forecast_days: List[:class:`ForecastDayModel`]
+        A list of forecast days
+    alerts: List[:class:`AlertModel`]
+        A list of alerts, this list can be empty
+    """
+    location: LocationModel
+    forecast_days: List[ForecastDayModel]
+    alerts: List[AlertModel]
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## weatherly/enums.py

 * *Ordering differences only*

```diff
@@ -1,159 +1,159 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from enum import Enum
-
-__all__ = (
-    "Languages",
-)
-
-class Languages(Enum):
-    """
-    Languages - an enum representing languages available for use in the WeatherAPI requests.
-    
-    Attributes are languages and language codes
-    
-    Attributes
-    ----------
-    Arabic: :class:`str`
-        Language code: ar
-    Bengali: :class:`str`
-        Language code: bn
-    Bulgarian: :class:`str`
-        Language code: bg
-    ChineseSimplified: :class:`str`
-        Language code: zh
-    ChineseTraditional: :class:`str`
-        Language code: zh_tw
-    Czech: :class:`str`
-        Language code: cs
-    Danish: :class:`str`
-        Language code: da
-    Dutch: :class:`str`
-        Language code: nl
-    Finnish: :class:`str`
-        Language code: fi
-    French: :class:`str`
-        Language code: fr
-    German: :class:`str`
-        Language code: de
-    Greek: :class:`str`
-        Language code: el
-    Hindi: :class:`str`
-        Language code: hi
-    Hungarian: :class:`str`
-        Language code: hu
-    Italian: :class:`str`
-        Language code: it
-    Japanese: :class:`str`
-        Language code: ja
-    Javanese: :class:`str`
-        Language code: jv
-    Korean: :class:`str`
-        Language code: ko
-    Mandarin: :class:`str`
-        Language code: zh_cmn
-    Marathi: :class:`str`
-        Language code: mr
-    Polish: :class:`str`
-        Language code: pl
-    Portuguese: :class:`str`
-        Language code: pt
-    Punjabi: :class:`str`
-        Language code: pa
-    Romanian: :class:`str`
-        Language code: ro
-    Russian: :class:`str`
-        Language code: ru
-    Serbian: :class:`str`
-        Language code: sr
-    Sinhalese: :class:`str`
-        Language code: si
-    Slovak: :class:`str`
-        Language code: sk
-    Spanish: :class:`str`
-        Language code: es
-    Swedish: :class:`str`
-        Language code: sv
-    Tamil: :class:`str`
-        Language code: ta
-    Telugu: :class:`str`
-        Language code: te
-    Turkish: :class:`str`
-        Language code: tr
-    Ukrainian: :class:`str`
-        Language code: uk
-    Urdu: :class:`str`
-        Language code: ur
-    Vietnamese: :class:`str`
-        Language code: vi
-    WuShanghainese: :class:`str`
-        Language code: zh_wuu
-    Xiang: :class:`str`
-        Language code: zh_hsn
-    YueCantonese: :class:`str`
-        Language code: zh_yue
-    Zulu: :class:`str`
-        Language code: zu
-    """
-    Arabic: str = "ar"
-    Bengali: str = "bn"
-    Bulgarian: str = "bg"
-    ChineseSimplified: str = "zh"
-    ChineseTraditional: str = "zh_tw"
-    Czech: str = "cs"
-    Danish: str = "da"
-    Dutch: str = "nl"
-    Finnish: str = "fi"
-    French: str = "fr"
-    German: str = "de"
-    Greek: str = "el"
-    Hindi: str = "hi"
-    Hungarian: str = "hu"
-    Italian: str = "it"
-    Japanese: str = "ja"
-    Javanese: str = "jv"
-    Korean: str = "ko"
-    Mandarin: str = "zh_cmn"
-    Marathi: str = "mr"
-    Polish: str = "pl"
-    Portuguese: str = "pt"
-    Punjabi: str = "pa"
-    Romanian: str = "ro"
-    Russian: str = "ru"
-    Serbian: str = "sr"
-    Sinhalese: str = "si"
-    Slovak: str = "sk"
-    Spanish: str = "es"
-    Swedish: str = "sv"
-    Tamil: str = "ta"
-    Telugu: str = "te"
-    Turkish: str =	"tr"
-    Ukrainian: str = "uk"
-    Urdu: str = "ur"
-    Vietnamese: str = "vi"
-    WuShanghainese: str = "zh_wuu"
-    Xiang: str = "zh_hsn"
-    YueCantonese: str =	"zh_yue"
-    Zulu: str = "zu"
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from enum import Enum
+
+__all__ = (
+    "Languages",
+)
+
+class Languages(Enum):
+    """
+    Languages - an enum representing languages available for use in the WeatherAPI requests.
+    
+    Attributes are languages and language codes
+    
+    Attributes
+    ----------
+    Arabic: :class:`str`
+        Language code: ar
+    Bengali: :class:`str`
+        Language code: bn
+    Bulgarian: :class:`str`
+        Language code: bg
+    ChineseSimplified: :class:`str`
+        Language code: zh
+    ChineseTraditional: :class:`str`
+        Language code: zh_tw
+    Czech: :class:`str`
+        Language code: cs
+    Danish: :class:`str`
+        Language code: da
+    Dutch: :class:`str`
+        Language code: nl
+    Finnish: :class:`str`
+        Language code: fi
+    French: :class:`str`
+        Language code: fr
+    German: :class:`str`
+        Language code: de
+    Greek: :class:`str`
+        Language code: el
+    Hindi: :class:`str`
+        Language code: hi
+    Hungarian: :class:`str`
+        Language code: hu
+    Italian: :class:`str`
+        Language code: it
+    Japanese: :class:`str`
+        Language code: ja
+    Javanese: :class:`str`
+        Language code: jv
+    Korean: :class:`str`
+        Language code: ko
+    Mandarin: :class:`str`
+        Language code: zh_cmn
+    Marathi: :class:`str`
+        Language code: mr
+    Polish: :class:`str`
+        Language code: pl
+    Portuguese: :class:`str`
+        Language code: pt
+    Punjabi: :class:`str`
+        Language code: pa
+    Romanian: :class:`str`
+        Language code: ro
+    Russian: :class:`str`
+        Language code: ru
+    Serbian: :class:`str`
+        Language code: sr
+    Sinhalese: :class:`str`
+        Language code: si
+    Slovak: :class:`str`
+        Language code: sk
+    Spanish: :class:`str`
+        Language code: es
+    Swedish: :class:`str`
+        Language code: sv
+    Tamil: :class:`str`
+        Language code: ta
+    Telugu: :class:`str`
+        Language code: te
+    Turkish: :class:`str`
+        Language code: tr
+    Ukrainian: :class:`str`
+        Language code: uk
+    Urdu: :class:`str`
+        Language code: ur
+    Vietnamese: :class:`str`
+        Language code: vi
+    WuShanghainese: :class:`str`
+        Language code: zh_wuu
+    Xiang: :class:`str`
+        Language code: zh_hsn
+    YueCantonese: :class:`str`
+        Language code: zh_yue
+    Zulu: :class:`str`
+        Language code: zu
+    """
+    Arabic: str = "ar"
+    Bengali: str = "bn"
+    Bulgarian: str = "bg"
+    ChineseSimplified: str = "zh"
+    ChineseTraditional: str = "zh_tw"
+    Czech: str = "cs"
+    Danish: str = "da"
+    Dutch: str = "nl"
+    Finnish: str = "fi"
+    French: str = "fr"
+    German: str = "de"
+    Greek: str = "el"
+    Hindi: str = "hi"
+    Hungarian: str = "hu"
+    Italian: str = "it"
+    Japanese: str = "ja"
+    Javanese: str = "jv"
+    Korean: str = "ko"
+    Mandarin: str = "zh_cmn"
+    Marathi: str = "mr"
+    Polish: str = "pl"
+    Portuguese: str = "pt"
+    Punjabi: str = "pa"
+    Romanian: str = "ro"
+    Russian: str = "ru"
+    Serbian: str = "sr"
+    Sinhalese: str = "si"
+    Slovak: str = "sk"
+    Spanish: str = "es"
+    Swedish: str = "sv"
+    Tamil: str = "ta"
+    Telugu: str = "te"
+    Turkish: str =	"tr"
+    Ukrainian: str = "uk"
+    Urdu: str = "ur"
+    Vietnamese: str = "vi"
+    WuShanghainese: str = "zh_wuu"
+    Xiang: str = "zh_hsn"
+    YueCantonese: str =	"zh_yue"
+    Zulu: str = "zu"
```

## weatherly/errors.py

```diff
@@ -1,122 +1,122 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-__all__ = (
-    "WeatherlyException",
-    "WeatherAPIException",
-    "NoLocationFound",
-    "InvalidAPIKey",
-    "APILimitExceeded",
-    "APIKeyDisabled",
-    "AccessDenied",
-    "InternalApplicationError",
-)
-
-class WeatherlyException(Exception):
-    """
-    A base class for all ``weatherly`` exceptions. Almost all exceptions of this module inherit from this class.
-
-    Inherits from :class:`Exception`.
-    """
-    pass
-
-class WeatherAPIException(WeatherlyException): 
-    """
-    The base class for :class:`weatherly.WeatherAPIClient` weather requests exceptions.
-    
-    Parameters
-    ----------
-    status: :class:`int`
-        HTTP status code
-    code: :class:`int`
-        Error code
-    message: :class:`str`
-        Message provided with the error
-    """
-    def __init__(self, status: int, code: int, message: str, *args):
-        self.status = status
-        self.code = code
-        self.message = message
-        self.formatted_message = f"{self.status} (error code {self.code}): {message}"
-        super().__init__(self.formatted_message, *args)
-
-class NoLocationFound(WeatherAPIException): 
-    """
-    Exception like this is raised when no location was found when searching for weather data.
-
-    Usually has status code  400 and error code 1006.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class InvalidAPIKey(WeatherAPIException): 
-    """
-    Exception like this is raised when provided API key is invalid
-
-    Usually has status code 401 and error code 2006.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class APILimitExceeded(WeatherAPIException): 
-    """
-    Exception like this is raised when API key has exceeded monthly calls limit.
-
-    Usually has status code 400 and error code 2007.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class APIKeyDisabled(WeatherAPIException): 
-    """
-    Exception like this is raised when API key has been disabled.
-
-    Usually has status code 403 and error code 2008.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class AccessDenied(WeatherAPIException): 
-    """
-    Exception like this is raised when API key does not have access to requested resource.
-
-    Usually has status code 403 and error code 2009.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
-    pass
-
-class InternalApplicationError(WeatherAPIException): 
-    """
-    Exception like this is raised when an internal application error occured. There is nothing to do about it.
-
-    Usually has status code 400 and error code 9999.
-    
-    Inherits from :class:`WeatherAPIException`.
-    """
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+__all__ = (
+    "WeatherlyException",
+    "WeatherAPIException",
+    "NoLocationFound",
+    "InvalidAPIKey",
+    "APILimitExceeded",
+    "APIKeyDisabled",
+    "AccessDenied",
+    "InternalApplicationError",
+)
+
+class WeatherlyException(Exception):
+    """
+    A base class for all ``weatherly`` exceptions. Almost all exceptions of this module inherit from this class.
+
+    Inherits from :class:`Exception`.
+    """
+    pass
+
+class WeatherAPIException(WeatherlyException): 
+    """
+    The base class for :class:`Client` weather requests exceptions.
+    
+    Parameters
+    ----------
+    status: :class:`int`
+        HTTP status code
+    code: :class:`int`
+        Error code
+    message: :class:`str`
+        Message provided with the error
+    """
+    def __init__(self, status: int, code: int, message: str, *args):
+        self.status = status
+        self.code = code
+        self.message = message
+        self.formatted_message = f"{self.status} (error code {self.code}): {message}"
+        super().__init__(self.formatted_message, *args)
+
+class NoLocationFound(WeatherAPIException): 
+    """
+    Exception like this is raised when no location was found when searching for weather data.
+
+    Usually has status code  400 and error code 1006.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class InvalidAPIKey(WeatherAPIException): 
+    """
+    Exception like this is raised when provided API key is invalid
+
+    Usually has status code 401 and error code 2006.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class APILimitExceeded(WeatherAPIException): 
+    """
+    Exception like this is raised when API key has exceeded monthly calls limit.
+
+    Usually has status code 400 and error code 2007.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class APIKeyDisabled(WeatherAPIException): 
+    """
+    Exception like this is raised when API key has been disabled.
+
+    Usually has status code 403 and error code 2008.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class AccessDenied(WeatherAPIException): 
+    """
+    Exception like this is raised when API key does not have access to requested resource.
+
+    Usually has status code 403 and error code 2009.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
+    pass
+
+class InternalApplicationError(WeatherAPIException): 
+    """
+    Exception like this is raised when an internal application error occured. There is nothing to do about it.
+
+    Usually has status code 400 and error code 9999.
+    
+    Inherits from :class:`WeatherAPIException`.
+    """
     pass
```

## weatherly/responses.py

```diff
@@ -1,182 +1,623 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from .abc import CurrentWeather, LocationModel
-from typing import (
-    Dict,
-    Any,
-    Union
-)
-
-__all__ = (
-    "CurrentWeatherData",
-    "LocationData",
-)
-
-class CurrentWeatherData(CurrentWeather):
-    """
-    Current weather data, a common return type from methods that requests this from WeatherAPI.com.
-    
-    Please note, that only ``condition_text`` is translated into requested language.
-    
-    .. note::
-        This class should not be created manually, instead it will be returned from methods like ``get_current_weather`` of the :class:`WeatherAPIClient` class.
-
-    Attributes
-    ----------
-    raw: Dict[:class:`str`, Any]
-        Raw response in a JSON-like format (converted to a python dictionary)
-    status: :class:`int`
-        HTTP status of the response. 200 is OK, and is the most common status.
-    code: Union[:class:`int`, None]
-        Response code. In some cases this can be ``None``
-    location: :class:`LocationData`
-        Location of the requested weather data
-    last_updated_epoch: :class:`int`
-        The timestamp when the weather data was last updated.
-    temp_c: :class:`float`
-        Weather temperature in Celsius
-    temp_f: :class:`float`
-        Weather temperature in Fahrenheit
-    is_day: :class:`bool`
-        Wherever the current time is considered day time.
-    condition_text: :class:`str`
-        Weather condition text
-    condition_icon: :class:`str`
-        Link to the weather condition icon
-    condition_code: :class:`int`
-        Code of current weather condition
-    wind_mph: :class:`float`
-        Current wind speed in miles per hour (mph)
-    wind_kph: :class:`float`
-        Current wind speed in kilometers per hour (kph)
-    wind_degree: :class:`int`
-        Direction of wind in degrees
-    wind_dir: :class:`str`
-        Direction of wind as a string (e.g. "W")
-    pressure_mb: :class:`float`
-        Pressure in millibars (mb)
-    pressure_in: :class:`float`
-        Pressure in inches (in)
-    precip_mm: :class:`float`
-        Precipation (water that is falling out of the sky) in millimeters (mm)
-    precip_in: :class:`float`
-        Precipation (water that is falling in the sky) in inches (in)
-    humidity: :class:`int`
-        Humidity in integer percentage
-    cloud: :class:`int`
-        Cloud cover as percentage
-    feelslike_c: :class:`float`
-        Feels like temperature in Celsius
-    feelslike_f: :class:`float`
-        Feels like temperature in Fahrenheit
-    uv: :class:`float`
-        UV Index
-    """
-    def __init__(
-        self,
-        raw: Dict[str, Any],
-        status: int,
-        code: Union[int, None]
-    ) -> None:
-        super().__init__()
-        
-        self.status = status
-        self.code = code
-        self.raw = raw
-        
-        self.location = LocationData(raw["location"], status, code)
-        raw = raw["current"]
-        
-        self.last_updated_epoch = raw["last_updated_epoch"]
-        self.temp_c = raw["temp_c"]
-        self.temp_f = raw["temp_f"]
-        self.is_day = bool(raw["is_day"])
-        self.condition_text = raw["condition"]["text"]
-        self.condition_icon = raw["condition"]["icon"]
-        self.condition_code = raw["condition"]["code"]
-        self.wind_mph = raw["wind_mph"]
-        self.wind_kph = raw["wind_kph"]
-        self.wind_degree = raw["wind_degree"]
-        self.wind_dir = raw["wind_dir"]
-        self.pressure_mb = raw["pressure_mb"]
-        self.pressure_in = raw["pressure_in"]
-        self.precip_mm = raw["precip_mm"]
-        self.precip_in = raw["precip_in"]
-        self.humidity = raw["humidity"]
-        self.cloud = raw["cloud"]
-        self.feelslike_c = raw["feelslike_c"]
-        self.feelslike_f = raw["feelslike_f"]
-        self.uv = raw["uv"]
-
-class LocationData(LocationModel):
-    """
-    Location data, returned with most requests.
-    
-    Attributes
-    --------------
-    raw: Dict[:class:`str`, Any]
-        Raw response in a JSON-like format (converted to a python dictionary)
-    status: :class:`int`
-        HTTP status of the response. 200 is OK, and is the most common status.
-    code: Union[:class:`int`, None]
-        Response code. In some cases this can be ``None``
-    id: Optional[:class:`int`]
-        A specific ID of the location. Can be ``None``
-    name: :class:`str`
-        Name of the location (e.g. London)
-    region: :class:`str`
-        A region of the location
-    country: :class:`str`
-        Country where the location is
-    latitude: :class:`float`
-        Latitude coordinate of the location
-    longitude: :class:`float`
-        Longitude coordinate of the location
-    timezone_id: Optional[:class:`str`]
-        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.
-    localtime_epoch: Optional[:class:`int`]
-        Local time of the location as a timestamp
-    localtime_formatted: Optional[:class:`str`]
-        Formatted local time of the location
-    """
-    def __init__(
-        self, 
-        raw: Dict[str, Any],
-        status: int,
-        code: Union[int, None]
-    ) -> None:
-        self.raw = raw
-        self.status = status
-        self.code = code
-
-        self.id = raw.get('id', None)
-        self.name = raw['name']
-        self.region = raw['region']
-        self.country = raw['country']
-        self.latitude = raw['lat']
-        self.longitude = raw['lon']
-        self.timezone_id = raw.get('tz_id', None)
-        self.localtime_epoch = raw.get('localtime_epoch')
-        self.localtime_formatted = raw.get('localtime', None)
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from .abc import (
+    CurrentWeather, 
+    LocationModel, 
+    AirQuality, 
+    ForecastDayModel, 
+    ForecastHourModel, 
+    ForecastModel,
+    AlertModel,
+)
+from typing import (
+    Dict,
+    Any,
+    Union,
+    Optional,
+)
+
+__all__ = (
+    "CurrentWeatherData",
+    "LocationData",
+    "AirQualityData",
+    "ForecastData",
+    "ForecastDay",
+    "ForecastHour",
+    "AlertData",
+)
+
+GB_DEFRA_BAND = ("Low", "Low", "Low", "Moderate", "Moderate", "Moderate", "High", "High", "High", "Very High")
+
+class CurrentWeatherData(CurrentWeather):
+    """
+    Current weather data, a common return type from methods that requests this from WeatherAPI.com.
+    
+    Please note, that only ``condition_text`` is translated into requested language.
+    
+    Attributes
+    ----------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    location: :class:`LocationData`
+        Location of the requested weather data
+    last_updated_epoch: :class:`int`
+        The timestamp when the weather data was last updated.
+    temp_c: :class:`float`
+        Weather temperature in Celsius
+    temp_f: :class:`float`
+        Weather temperature in Fahrenheit
+    is_day: :class:`bool`
+        Wherever the current time is considered day time.
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Link to the weather condition icon
+    condition_code: :class:`int`
+        Code of current weather condition
+    wind_mph: :class:`float`
+        Current wind speed in miles per hour (mph)
+    wind_kph: :class:`float`
+        Current wind speed in kilometers per hour (kph)
+    wind_degree: :class:`int`
+        Direction of wind in degrees
+    wind_dir: :class:`str`
+        Direction of wind as a string (e.g. "W")
+    pressure_mb: :class:`float`
+        Pressure in millibars (mb)
+    pressure_in: :class:`float`
+        Pressure in inches (in)
+    precip_mm: :class:`float`
+        Precipation (water that is falling out of the sky) in millimeters (mm)
+    precip_in: :class:`float`
+        Precipation (water that is falling in the sky) in inches (in)
+    humidity: :class:`int`
+        Humidity in integer percentage
+    cloud: :class:`int`
+        Cloud cover as percentage
+    feelslike_c: :class:`float`
+        Feels like temperature in Celsius
+    feelslike_f: :class:`float`
+        Feels like temperature in Fahrenheit
+    uv: :class:`float`
+        UV Index
+    aqi: Optional[:class:`AirQualityData`]
+        Air quality data. Can be ``None`` (if this field of data was not requested)
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        super().__init__()
+        
+        self.status = status
+        self.code = code
+        self.raw = raw
+        
+        self.location = LocationData(raw["location"], status, code)
+        raw = raw["current"]
+        
+        self.aqi = AirQualityData(raw["air_quality"], status, code) if raw.get("air_quality") else None
+        self.last_updated_epoch = raw["last_updated_epoch"]
+        self.temp_c = raw["temp_c"]
+        self.temp_f = raw["temp_f"]
+        self.is_day = bool(raw["is_day"])
+        self.condition_text = raw["condition"]["text"]
+        self.condition_icon = raw["condition"]["icon"]
+        self.condition_code = raw["condition"]["code"]
+        self.wind_mph = raw["wind_mph"]
+        self.wind_kph = raw["wind_kph"]
+        self.wind_degree = raw["wind_degree"]
+        self.wind_dir = raw["wind_dir"]
+        self.pressure_mb = raw["pressure_mb"]
+        self.pressure_in = raw["pressure_in"]
+        self.precip_mm = raw["precip_mm"]
+        self.precip_in = raw["precip_in"]
+        self.humidity = raw["humidity"]
+        self.cloud = raw["cloud"]
+        self.feelslike_c = raw["feelslike_c"]
+        self.feelslike_f = raw["feelslike_f"]
+        self.uv = raw["uv"]
+
+class LocationData(LocationModel):
+    """
+    Location data, returned with most requests.
+    
+    Attributes
+    --------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    id: Optional[:class:`int`]
+        A specific ID of the location. Can be ``None``
+    name: :class:`str`
+        Name of the location (e.g. London)
+    region: :class:`str`
+        A region of the location
+    country: :class:`str`
+        Country where the location is
+    latitude: :class:`float`
+        Latitude coordinate of the location
+    longitude: :class:`float`
+        Longitude coordinate of the location
+    timezone_id: Optional[:class:`str`]
+        Timezone ID of the location (e.g. Europe/London). Could be ``None`` when using the Search/Autocomplete API.
+    localtime_epoch: Optional[:class:`int`]
+        Local time of the location as a timestamp
+    localtime_formatted: Optional[:class:`str`]
+        Formatted local time of the location
+    """
+    def __init__(
+        self, 
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+
+        self.id = raw.get('id', None)
+        self.name = raw['name']
+        self.region = raw['region']
+        self.country = raw['country']
+        self.latitude = raw['lat']
+        self.longitude = raw['lon']
+        self.timezone_id = raw.get('tz_id', None)
+        self.localtime_epoch = raw.get('localtime_epoch')
+        self.localtime_formatted = raw.get('localtime', None)
+
+
+class AirQualityData(AirQuality):
+    """
+    Attributes
+    --------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    co: :class:`float`
+        Carbon Monoxide (μg/m3)
+    o3: :class:`float`
+        Ozone (μg/m3)
+    no2: :class`float`	
+        Nitrogen dioxide (μg/m3)
+    so2: :class:`float`
+        Sulphur dioxide (μg/m3)
+    pm2_5: :class`float`
+        PM2.5 (μg/m3)
+    pm10: :class:`float`
+        PM10 (μg/m3)
+    us_epa_index: :class:`int`
+        US - EPA standard.
+        * 1 means Good
+        * 2 means Moderate
+        * 3 means Unhealthy for sensitive group
+        * 4 means Unhealthy
+        * 5 means Very Unhealthy
+        * 6 means Hazardous
+    gb_defra_index: :class:`int`
+        UK Defra Index
+        
+        +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+        | Index  | 1    | 2     | 3     | 4        | 5        | 6        | 7     | 8     | 9     | 10         |
+        +========+======+=======+=======+==========+==========+==========+=======+=======+=======+============+
+        | Band   | Low  | Low   | Low   | Moderate | Moderate | Moderate | High  | High  | High  | Very High  |
+        +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+        | µgm^-3 | 0-11 | 12-23 | 24-35 | 36-41    | 42-47    | 48-53    | 54-58 | 59-64 | 65-70 | 71 or more |
+        +--------+------+-------+-------+----------+----------+----------+-------+-------+-------+------------+
+    gb_defra_band: :class:`str`
+        A band corresponding to the :ref:`gb_defra_index`
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+        
+        self.co = raw["co"]
+        self.o3 = raw["o3"]
+        self.no2 = raw["no2"]
+        self.so2 = raw["so2"]
+        self.pm2_5 = raw["pm2_5"]
+        self.pm10 = raw["pm10"]
+        self.us_epa_index = raw["us-epa-index"]
+        self.gb_defra_index = raw["gb-defra-index"]
+
+        self.gb_defra_band = GB_DEFRA_BAND[self.gb_defra_index-1]
+
+class AlertData(AlertModel):
+    """
+    An alert from WeatherAPI
+
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    headline: :class:`str`
+        Alert headline
+    msg_type: :class:`str`
+        Type of alert
+    severity: :class:`str`
+        Severity of alert
+    urgency: :class:`str`
+        Urgency
+    areas: :class:`str`
+        Areas covered
+    category: :class:`str`
+        Category
+    certainty: :class:`str`
+        Certainty
+    event: :class:`str`
+        Event
+    note: :class:`str`
+        Note
+    effective: :class:`str`
+        Effective
+    expires: :class:`str`
+        Expires
+    description: :class:`str`
+        Description
+    instruction: :class:`str`
+        Instruction
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+        
+        self.headline = raw["headline"]
+        self.msg_type = raw["msgType"]
+        self.severity = raw["severity"]
+        self.urgency = raw["urgency"]
+        self.areas = raw["areas"]
+        self.category = raw["category"]
+        self.certainty = raw["certainty"]
+        self.event = raw["event"]
+        self.note = raw["note"]
+        self.effective = raw["effective"]
+        self.expires = raw["expires"]
+        self.description = raw["desc"]
+        self.instruction = raw["instruction"]
+
+class ForecastHour(ForecastHourModel):
+    """
+    Forecast hour, an element of :class:`ForecastDay`
+    
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    time_epoch: :class:`int`
+        Time as epoch
+    time: :class:`str`
+        Date and time
+    temp_c: :class:`float`
+        Temperature in celsius
+    temp_f: :class:`float`
+        Temperature in fahrenheit
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icons
+    condition_code: :class:`int`
+        Weather condition code
+    wind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    wind_kph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    wind_degree: :class:`int`
+        Wind direction in degrees
+    wind_dir: :class:`str`
+        Wind direction as 16 point compass. e.g.: NSW
+    pressure_mb: :class:`float`
+        Pressure in millibars
+    pressure_in: :class:`float`
+        Pressure in inches
+    precip_mm: :class:`float`
+        Precipitation amount in millimeters
+    precip_in: :class:`float`
+        Precipitation amount in inches
+    humidity: :class:`int`
+        Humidity as percentage
+    cloud: :class:`int`
+        Cloud cover as percentage
+    feelslike_c: :class:`float`
+        Feels like temperature as celcius
+    feelslike_f: :class:`float`
+        Feels like temperature as fahrenheit
+    windchill_c: :class:`float`
+        Windchill temperature in celcius
+    windchill_f: :class:`float`
+        Windchill temperature in fahrenheit
+    headindex_c: :class:`float`
+        Heat index in celcius
+    headindex_f: :class:`float`
+        Heat index in fahrenheit
+    dewpoint_c: :class:`float`
+        Dew point in celcius
+    dewpoint_f: :class:`float`
+        Dew point in fahrenheit
+    will_it_rain: :class:`bool`
+        Will it will rain or not
+    will_it_snow: :class:`bool`
+        Will it will snow or not
+    is_day: :class:`bool`
+        Whether to show day condition icon or night icon
+    vis_km: :class:`float`
+        Visibility in kilometer
+    vis_miles: :class:`float`
+        Visibility in miles
+    chance_of_rain: :class:`int`
+        Chance of rain as percentage
+    chance_of_snow: :class:`int`
+        Chance of snow as percentage
+    gust_mph: :class:`float`
+        Wind gust in miles per hour
+    gust_kph: :class:`float`
+        Wind gust in kilometer per hour
+    uv: :class:`float`
+        UV Index
+    aqi: Optional[:class:`AirQualityData`]
+        Air Quality data. See :class:`AirQualityData` for more info.
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+
+        self.time_epoch = raw["time_epoch"]
+        self.time = raw["time"]
+        self.temp_c = raw["temp_c"]
+        self.temp_f = raw["temp_f"]
+        self.condition_text = raw["condition"]["text"]
+        self.condition_icon = raw["condition"]["icon"]
+        self.condition_code = raw["condition"]["code"]
+        self.wind_mph = raw["wind_mph"]
+        self.wind_kph = raw["wind_kph"]
+        self.wind_degree = raw["wind_degree"]
+        self.wind_dir = raw["wind_dir"]
+        self.pressure_mb = raw["pressure_mb"]
+        self.pressure_in = raw["pressure_in"]
+        self.precip_mm = raw["precip_mm"]
+        self.precip_in = raw["precip_in"]
+        self.humidity = raw["humidity"]
+        self.cloud = raw["cloud"]
+        self.feelslike_c = raw["feelslike_c"]
+        self.feelslike_f = raw["feelslike_f"]
+        self.windchill_c = raw["windchill_c"]
+        self.windchill_f = raw["windchill_f"]
+        self.heatindex_c = raw["heatindex_c"]
+        self.heatindex_f = raw["heatindex_f"]
+        self.dewpoint_c = raw["dewpoint_c"]
+        self.dewpoint_f = raw["dewpoint_f"]
+        self.will_it_rain = bool(raw["will_it_rain"])
+        self.will_it_snow = bool(raw["will_it_snow"])
+        self.is_day = bool(raw["is_day"])
+        self.vis_km = raw["vis_km"]
+        self.vis_miles = raw["vis_miles"]
+        self.chance_of_rain = raw["chance_of_rain"]
+        self.chance_of_snow = raw["chance_of_snow"]
+        self.gust_mph = raw["gust_mph"]
+        self.gust_kph = raw["gust_kph"]
+        self.uv = raw["uv"]
+        
+        if raw.get("air_quality"): self.aqi = AirQualityData(raw["air_quality"], status, code)
+        else: self.aqi = None
+    
+class ForecastDay(ForecastDayModel):
+    """
+    A forecast day, element of :class:`ForecastData`
+
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    date: :class:`str`
+        Forecast date
+    date_epoch: :class:`int`
+        Forecast date as unix time.
+    maxtemp_c: :class:`float`
+        Maximum temperature in celsius for the day.
+    maxtemp_f: :class:`float`
+        Maximum temperature in fahrenheit for the day
+    mintemp_c: :class:`float`
+        Minimum temperature in celsius for the day
+    mintemp_f: :class:`float`
+        Minimum temperature in fahrenheit for the day
+    avgtemp_c: :class:`float`
+        Average temperature in celsius for the day
+    avgtemp_f: :class:`float`
+        Average temperature in fahrenheit for the day
+    maxwind_mph: :class:`float`
+        Maximum wind speed in miles per hour
+    maxwind_kph: :class:`float`
+        Maximum wind speed in kilometer per hour
+    totalprecip_mm: :class:`float`
+        Total precipitation in milimeter
+    totalprecip_in: :class:`float`
+        Total precipitation in inches
+    avgvis_km: :class:`float`
+        Average visibility in kilometer
+    avgvis_miles: :class:`float`
+        Average visibility in miles
+    avghumidity: :class:`int`
+        Average humidity as percentage
+    uv: :class:`int`
+        UV Index
+    condition_text: :class:`str`
+        Weather condition text
+    condition_icon: :class:`str`
+        Weather condition icon
+    condition_code: :class:`int`
+        Weather condition code
+    hour_data: List[:class:`ForecastHour`]
+        A list of :class:`ForecastHour` objects representing hourly weather data.
+    sunrise: :class:`str`
+        Sunrise time
+    sunset: :class:`str`
+        Sunset time
+    moonrise: :class:`str`
+        Moonrise time
+    moonset: :class:`str`
+        Moonset time
+    moon_phase: :class:`str`
+        Moon phases. Value returned:
+            * New Moon
+            * Waxing Crescent
+            * First Quarter
+            * Waxing Gibbous
+            * Full Moon
+            * Waning Gibbous
+            * Last Quarter
+            * Waning Crescent
+    moon_illumination: :class:`float`
+        Moon illumination as %
+    aqi: Optional[:class:`AirQualityData`]
+        Air Quality data as :class:`AirQualityData` object. Can be ``None``
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+        self.date = raw["date"]
+        self.date_epoch = raw["date_epoch"]
+        
+        before_raw = raw.copy()
+        raw = raw["day"]
+        
+        self.maxtemp_c = raw["maxtemp_c"]
+        self.maxtemp_f = raw["maxtemp_f"]
+        self.mintemp_c = raw["mintemp_c"]
+        self.mintemp_f = raw["mintemp_f"]
+        self.avgtemp_c = raw["avgtemp_c"]
+        self.avgtemp_f = raw["avgtemp_f"]
+        self.maxwind_mph = raw["maxwind_mph"]
+        self.maxwind_kph = raw["maxwind_kph"]
+        self.totalprecip_in = raw["totalprecip_in"]
+        self.totalprecip_mm = raw["totalprecip_mm"]
+        self.avgvis_km = raw["avgvis_km"]
+        self.avgvis_miles = raw["avgvis_miles"]
+        self.avghumidity = raw["avghumidity"]
+        self.uv = raw["uv"]
+        self.condition_text = raw["condition"]["text"]
+        self.condition_icon = raw["condition"]["icon"]
+        self.condition_code = raw["condition"]["code"]
+        if raw.get("air_quality"): self.aqi = AirQualityData(raw["air_quality"], status, code)
+        else: self.aqi = None
+        
+        raw = before_raw
+        self.hour_data = list([
+            ForecastHour(elem, status, code) for elem in raw["hour"]
+        ])
+        self.sunrise = raw["astro"]["sunrise"]
+        self.sunset = raw["astro"]["sunset"]
+        self.moonrise = raw["astro"]["moonrise"]
+        self.moonset = raw["astro"]["moonset"]
+        self.moon_phase = raw["astro"]["moon_phase"]
+        self.moon_illumination = raw["astro"]["moon_illumination"]
+
+    
+class ForecastData(ForecastModel):
+    """
+    Forecast data returned from Forecast API
+    
+    Attributes
+    -------------
+    raw: Dict[:class:`str`, Any]
+        Raw response in a JSON-like format (converted to a python dictionary)
+    status: :class:`int`
+        HTTP status of the response. 200 is OK, and is the most common status.
+    code: Optional[:class:`int`]
+        Response code. In some cases this can be ``None``
+    location: :class:`LocationData`
+        Location of the forecast data.
+    forecast_days: List[:class:`ForecastDay`]
+        A list of forecast days
+    alerts: List[:class:`AlertData`]
+        A list of alerts, this list can be empty. List is also empty, when the user disabled alerts in the request.
+    """
+    def __init__(
+        self,
+        raw: Dict[str, Any],
+        status: int,
+        code: Optional[int]
+    ) -> None:
+        self.raw = raw
+        self.status = status
+        self.code = code
+        
+        self.location = LocationData(raw["location"], status, code)
+        self.forecast_days = list([ForecastDay(elem, status, code) for elem in raw["forecast"]["forecastday"]])
+        self.alerts = []
+        alert_data = raw.get("alerts", {})
+        
+        for k,v in alert_data.items():
+            if v is not []:
+                self.alerts.extend(list([
+                    AlertData(elem, status, code) for elem in v
+                ]))
+
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## weatherly/utils.py

 * *Ordering differences only*

```diff
@@ -1,94 +1,94 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from typing import (
-    Dict,
-    Any,
-    overload
-)
-from .enums import Languages
-
-def parse_kwargs_to_urlargs(kwargs: Dict[str, Any]) -> str:
-    """
-    Parses keyword arguments (kwargs) to format fitting URLs
-    Example: ``{"some_key": "some value", "yes": "no"}`` -> ``?some_key=some_value&yes=no``
-    
-    Parameters
-    ----------
-    kwargs: Dict[:class:`str`, Any]
-        A dictionary of keyword arguments to be parsed.
-        
-    Returns
-    -------
-    args_string: :class:`str`
-        A string - formatted keyword arguments
-    """
-    if not kwargs: return ""
-    
-    args_string = ""
-    first = True
-    
-    for k,v in kwargs.items():
-        args_string += f"{'?' if first else '&'}{k}={v}"
-        first = False
-    return args_string
-
-@overload
-def find_language(lang: str, asobj: bool=False) -> None:
-    ...
-    
-@overload
-def find_language(lang: str, asobj: bool=False) -> Languages:
-    ...
-
-def find_language(lang: str, asobj: bool=False) -> str:
-    """
-    Used to find language code from available languages.
-
-    Paremeters
-    ----------
-    lang: :class:`str`
-        A language you want to search for
-
-    Returns
-    -------
-    Union[:class:`str`, :class:`Languages`, None]
-        Language code, could be ``None``, could be a :class:`Languages` enum.
-    """
-
-    if isinstance(lang, Languages):
-        try:
-            if asobj: return lang
-            return lang.value
-        except: 
-            return None
-
-    lang = lang.lower()
-
-    for language in Languages:
-        if language.name.lower() == lang or language.value == lang:
-            if asobj: return language
-            return language.value
-        
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import (
+    Dict,
+    Any,
+    overload
+)
+from .enums import Languages
+
+def parse_kwargs_to_urlargs(kwargs: Dict[str, Any]) -> str:
+    """
+    Parses keyword arguments (kwargs) to format fitting URLs
+    Example: ``{"some_key": "some value", "yes": "no"}`` -> ``?some_key=some_value&yes=no``
+    
+    Parameters
+    ----------
+    kwargs: Dict[:class:`str`, Any]
+        A dictionary of keyword arguments to be parsed.
+        
+    Returns
+    -------
+    args_string: :class:`str`
+        A string - formatted keyword arguments
+    """
+    if not kwargs: return ""
+    
+    args_string = ""
+    first = True
+    
+    for k,v in kwargs.items():
+        args_string += f"{'?' if first else '&'}{k}={v}"
+        first = False
+    return args_string
+
+@overload
+def find_language(lang: str, asobj: bool=False) -> None:
+    ...
+    
+@overload
+def find_language(lang: str, asobj: bool=False) -> Languages:
+    ...
+
+def find_language(lang: str, asobj: bool=False) -> str:
+    """
+    Used to find language code from available languages.
+
+    Paremeters
+    ----------
+    lang: :class:`str`
+        A language you want to search for
+
+    Returns
+    -------
+    Union[:class:`str`, :class:`Languages`, None]
+        Language code, could be ``None``, could be a :class:`Languages` enum.
+    """
+
+    if isinstance(lang, Languages):
+        try:
+            if asobj: return lang
+            return lang.value
+        except: 
+            return None
+
+    lang = lang.lower()
+
+    for language in Languages:
+        if language.name.lower() == lang or language.value == lang:
+            if asobj: return language
+            return language.value
+        
     return None
```

## weatherly/api/__init__.py

 * *Ordering differences only*

```diff
@@ -1,30 +1,30 @@
-"""
-weatherly/api
---------------
-An package extension to weatherly providing access to WeatherAPI (requests, client, etc.)
-
-
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from .client import *
+"""
+weatherly/api
+--------------
+An package extension to weatherly providing access to WeatherAPI (requests, client, etc.)
+
+
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from .client import *
```

## weatherly/api/client.py

```diff
@@ -1,260 +1,344 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from .core import BaseAPIClient
-from ..enums import Languages
-from ..responses import CurrentWeatherData, LocationData
-from ..errors import (
-    WeatherAPIException,
-    NoLocationFound,
-    InvalidAPIKey,
-    APILimitExceeded,
-    APIKeyDisabled,
-    AccessDenied,
-    InternalApplicationError
-)
-from .. import (
-    utils as utils
-)
-
-from typing import (
-    Any,
-    Literal,
-    Dict,
-    Optional,
-    Union,
-    List
-)
-
-WEATHERAPI_BASE_URL = "http://api.weatherapi.com/v1/"
-
-__all__ = (
-    "WeatherAPIClient",
-)
-
-class WeatherAPIClient(BaseAPIClient):
-    """
-    A WeatherAPI.com client for fetching various weather information
-
-    Parameters
-    ----------
-    api_key: :class:`str`
-        API Key used to authenticate when sending requests
-    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]
-        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
-    dt: Optional[:class:`int`]
-        Restrict date output for Forecast and History API method. (Required for History and Future API)
-    end_dt: Optional[:class:`int`]
-        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)
-    hour: Optional[:class:`int`]
-        Restricting forecast or history output to a specific hour in a given day.
-    aqi: Literal["yes", "no"]
-        Enable/Disable Air Quality data in forecast API output. Defaults to "no".
-    tides: Literal["yes", "no"]
-        Enable/Disable Tide data in Marine API output. Defaults to "no".
-    kwargs: Dict[:class:`str`, Any]
-        Additional keyword arguments passed by default to requests made by the client
-    """
-    def __init__(
-        self,
-        api_key: str,
-        lang: Optional[Union[str, Languages]] = None,
-        dt: Optional[int] = None,
-        end_dt: Optional[int] = None,
-        hour: Optional[int] = None,
-        aqi: Literal["yes", "no"] = "no",
-        tides: Literal["yes", "no"] = "no",
-        **kwargs: Dict[str, Any]
-    ) -> None:
-        lang_code = None
-        if lang is not None: 
-            lang_code = utils.find_language(lang, asobj=True)
-        opts = {
-            "key": api_key,
-            **kwargs
-        }
-        if lang_code: opts.update(lang = lang_code.value if lang_code is not None else None)
-
-        super().__init__(base_url=WEATHERAPI_BASE_URL,
-                         default_options=opts)
-        
-        self.dt = dt
-        self.end_dt = end_dt
-        self.hour = hour
-        self.aqi = aqi
-        self.tides = tides
-        self.kwargs = kwargs
-        self.lang = Languages(lang_code) if lang_code else None
-    
-    
-    def _call_request(self, endpoint: str, options: Dict[str, Any]) -> Dict[str, Any]:
-        """Private method used to make requests to WeatherAPI"""
-        final_options = self.default_options.copy()
-
-        for k,v in final_options.items(): # check - remove NoneType values
-            if v is None: del final_options[k]
-        # add options to final_options
-        for k,v in options.items():
-            if v is not None: final_options[k] = v
-
-        resp = self._request(endpoint, **final_options)
-
-        if not resp[1].status_code < 400:
-            # raise errors yay
-            error_data = resp[0]["error"]
-            code = error_data["code"]
-            status = resp[1].status_code
-            msg = error_data["message"]
-
-            if code == 1006: raise NoLocationFound(status, code, msg)
-            elif code == 2006: raise InvalidAPIKey(status, code, msg)
-            elif code == 2007: raise APILimitExceeded(status, code, msg)
-            elif code == 2008: raise APIKeyDisabled(status, code, msg)
-            elif code == 2009: raise AccessDenied(status, code, msg)
-            elif code == 9999: raise InternalApplicationError(status, code, msg)
-            else: raise WeatherAPIException(status, code, msg)
-
-        return resp
-
-    def set_language(self, lang: Union[str, Languages]) -> Union[Languages, None]:
-        """
-        Set client's language when requesting data.
-        
-        Parameters
-        -----------
-        lang: Union[:class:`str`, :class:`Languages`]
-            Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.
-            
-        Returns
-        ---------
-        :class:`bool`
-            A boolean indicating whether the language was successfully set. If it's ``False``, then something went wrong, probably because of the wrong ``lang`` value.
-        """
-        lang_class = utils.find_language(lang, asobj=True)
-        if not lang_class:
-            self.lang = None
-            return False
-
-        self.lang = lang_class 
-        return True
-
-    def get_current_weather(self, 
-        query: str,
-        lang: Optional[Union[str, Languages]] = None,
-        aqi: Literal["yes", "no", None] = None,
-        **kwargs: Dict[str, Any]
-    ) -> CurrentWeatherData:
-        """
-        Get current weather data
-
-        Parameters
-        ----------
-        query: :class:`str`
-            Query string - location you want to get weather data for
-        lang: Optional[Union[:class:`str`, Languages]]
-            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
-            To get a list of languages visit :class:`Languages`.
-        aqi: Literal["yes", "no", None]
-            Enable/Disable Air Quality data in forecast API output. If nothing is passes, then it defaults to client default value.
-        kwargs: Dict[:class:`str`, Any]
-            Additional keyword arguments to request
-
-        Returns
-        -------
-        :class:`CurrentWeatherData`
-            Current weather data class
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        options = {
-            "aqi": aqi or self.aqi,
-            "q": query,
-            **kwargs
-        }
-        if lang is not None: options["lang"] = lang
-        resp = self._call_request("current.json", options)
-
-        weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
-        return weather
-
-    def get_locations(self, query: str):
-        """
-        Get locations for given query
-
-        Parameters
-        ---------------
-        query: :class:`str`
-            Query string, a location you are searching for
-
-        Returns
-        -----------
-        List[:class:`LocationData`]
-            A list of :class:`LocationData` classes.
-
-        Raises
-        ---------
-        :exc:`NoLocationFound`
-            Raised when no location for given query was found
-        :exc:`InvalidAPIKey`
-            Raised when the API key is invalid
-        :exc:`APILimitExceeded`
-            Raised when API key calls limit was exceeded
-        :exc:`APIKeyDisabled`
-            Raised when API key is disabled
-        :exc:`AccessDenied`
-            Raised when access to given resource was denied
-        :exc:`InternalApplicationError`
-            Raised when there was a very rare internal application error
-        :exc:`WeatherAPIException`
-            Raised when something else went wrong, that does not have a specific exception class.
-        """
-        resp = self._call_request("search.json",{"q": query})
-
-        locations = []
-        for loc in resp[0]:
-            locations.append(LocationData(loc, resp[1].status_code, None))
-        return locations
-    
-    def __str__(self):
-        return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
-    
-    def __repr__(self):
-        return repr(f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>")
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from .core import BaseAPIClient
+from ..enums import Languages
+from ..responses import (
+    CurrentWeatherData, 
+    LocationData, 
+    ForecastData
+)
+from ..errors import (
+    WeatherAPIException,
+    NoLocationFound,
+    InvalidAPIKey,
+    APILimitExceeded,
+    APIKeyDisabled,
+    AccessDenied,
+    InternalApplicationError
+)
+from .. import (
+    utils as utils
+)
+
+from typing import (
+    Any,
+    Literal,
+    Dict,
+    Optional,
+    Union,
+    List
+)
+
+WEATHERAPI_BASE_URL = "http://api.weatherapi.com/v1/"
+BOOL_REPLACE = {True: "yes", False: "no"}
+
+__all__ = (
+    "Client",
+)
+
+class Client(BaseAPIClient):
+    """
+    A WeatherAPI.com client for fetching various weather information
+
+    Parameters
+    ----------
+    api_key: :class:`str`
+        API Key used to authenticate when sending requests
+    lang: Optional[ Union[:class:`str`, :class:`Languages`] ]
+        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
+    dt: Optional[:class:`int`]
+        Restrict date output for Forecast and History API method. (Required for History and Future API)
+    end_dt: Optional[:class:`int`]
+        Restrict date output for History API method. Only works for API on Pro plan and above. (Available for History API)
+    hour: Optional[:class:`int`]
+        Restricting forecast or history output to a specific hour in a given day.
+    aqi: :class:`bool`
+        Enable/Disable Air Quality data in forecast API output. Defaults to "no".
+    tides: :class:`bool`
+        Enable/Disable Tide data in Marine API output. Defaults to "no".
+    kwargs: Dict[:class:`str`, Any]
+        Additional keyword arguments passed by default to requests made by the client
+        
+    Attributes
+    -------------
+    lang: Optional[:class:`Languages`]
+        Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+        To get a list of languages visit :class:`Languages`. If ``None`` then the default language is used (English)
+    dt: Optional[:class:`int`]
+        Restricted date output for Forecast and History API method. (Required for History and Future API)
+    end_dt: Optional[:class:`int`]
+        Restricted date output for History API method. Only works for API on Pro plan and above.
+    hour: Optional[:class:`int`]
+        Restricted forecast or history output to a specific hour in a given day.
+    aqi: :class:`bool`
+        Indicates if Air Quality data has been enabled
+    tides: :class:`bool`
+        Indicates if tides data in the Marine API has been enabled
+    kwargs: Dict[:class:`str`, Any]
+        Additional keyword arguments passed by default to requests made by the client
+    """
+    def __init__(
+        self,
+        api_key: str,
+        lang: Optional[Union[str, Languages]] = None,
+        dt: Optional[int] = None,
+        end_dt: Optional[int] = None,
+        hour: Optional[int] = None,
+        aqi: bool = False,
+        tides: bool = False,
+        **kwargs: Dict[str, Any]
+    ) -> None:
+        lang_code = None
+        if lang is not None: 
+            lang_code = utils.find_language(lang, asobj=True)
+        opts = {
+            "key": api_key,
+            **kwargs
+        }
+        if lang_code: opts.update(lang = lang_code.value if lang_code is not None else None)
+
+        super().__init__(base_url=WEATHERAPI_BASE_URL,
+                         default_options=opts)
+        
+        self.dt = dt
+        self.end_dt = end_dt
+        self.hour = hour
+        self.aqi = aqi
+        self.tides = tides
+        self.kwargs = kwargs
+        self.lang = Languages(lang_code) if lang_code else None
+    
+    
+    def _call_request(self, endpoint: str, options: Dict[str, Any]) -> Dict[str, Any]:
+        """Private method used to make requests to WeatherAPI"""
+        final_options = self.default_options.copy()
+
+        for k,v in final_options.items(): # check - remove NoneType values
+            if v is None: del final_options[k]
+        # add options to final_options
+        for k,v in options.items():
+            # also - replace bool with "yes"/"no"
+            if v is not None: final_options[k] = BOOL_REPLACE.get(v, v)
+
+        resp = self._request(endpoint, **final_options)
+
+        if not resp[1].status_code < 400:
+            # raise errors yay
+            error_data = resp[0]["error"]
+            code = error_data["code"]
+            status = resp[1].status_code
+            msg = error_data["message"]
+
+            if code == 1006: raise NoLocationFound(status, code, msg)
+            elif code == 2006: raise InvalidAPIKey(status, code, msg)
+            elif code == 2007: raise APILimitExceeded(status, code, msg)
+            elif code == 2008: raise APIKeyDisabled(status, code, msg)
+            elif code == 2009: raise AccessDenied(status, code, msg)
+            elif code == 9999: raise InternalApplicationError(status, code, msg)
+            else: raise WeatherAPIException(status, code, msg)
+
+        return resp
+
+    def set_language(self, lang: Union[str, Languages]) -> Optional[Languages]:
+        """
+        Set client's language when requesting data.
+        
+        Parameters
+        -----------
+        lang: Union[:class:`str`, :class:`Languages`]
+            Language to set. Can be either a string that is lanuage's name or code or a :class:`Languages` enum object.
+            
+        Returns
+        ---------
+        Optional[:class:`Languages`]
+            An enum class representing the language of the client. Is ``None`` when something went wrong and the language was not set.
+        """
+        lang_class = utils.find_language(lang, asobj=True)
+        if not lang_class:
+            return None
+
+        self.lang = lang_class 
+        return self.lang
+
+    def get_current_weather(self, 
+        query: str, 
+        *,
+        lang: Optional[Union[str, Languages]] = None,
+        aqi: Optional[bool] = None,
+        **kwargs: Dict[str, Any]
+    ) -> CurrentWeatherData:
+        """
+        Get current weather data
+
+        Parameters
+        ----------
+        query: :class:`str`
+            Query string - location you want to get weather data for
+        lang: Optional[Union[:class:`str`, Languages]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        aqi: Optional[:class:`bool`]
+            Enable/Disable Air Quality data in forecast API output. If nothing is passed, then it defaults to client default value.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments to request
+
+        Returns
+        -------
+        :class:`CurrentWeatherData`
+            Current weather data class
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "aqi": aqi or self.aqi,
+            "q": query,
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+        resp = self._call_request("current.json", options)
+
+        weather = CurrentWeatherData(resp[0], resp[1].status_code, None)
+        return weather
+
+    def get_locations(self, query: str):
+        """
+        Get locations for given query
+
+        Parameters
+        ---------------
+        query: :class:`str`
+            Query string, a location you are searching for
+
+        Returns
+        -----------
+        List[:class:`LocationData`]
+            A list of :class:`LocationData` classes.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        resp = self._call_request("search.json",{"q": query})
+
+        locations = []
+        for loc in resp[0]:
+            locations.append(LocationData(loc, resp[1].status_code, None))
+        return locations
+
+    def get_forecast_data(
+        self,
+        query: str, 
+        *,
+        aqi: Optional[bool] = None,
+        alerts: Optional[bool] = None,
+        lang: Optional[Union[str, Languages]] = None,
+        **kwargs: Dict[str, Any]
+    ) -> ForecastData:
+        """
+        Get forecast data from Forecast API
+
+        Parameters
+        -------------
+        query: :class:`str`
+            Query string, location you want to get forecast data for
+        aqi: Optional[:class:`bool`]
+            Enable/Disable Air Quality data. Defaults to ``None`` (will use client's default)
+        alerts: Optional[:class:`bool`]
+            Enable/Disable alerts data. Defaults to ``None`` (will use client's default)
+        lang: Optional[Union[:class`str`, :class`Languages`]]
+            Language from the :class:`Languages` enum or a string representing the language or language code (preferably).
+            To get a list of languages visit :class:`Languages`.
+        kwargs: Dict[:class:`str`, Any]
+            Additional keyword arguments that will be passed to the request.
+            
+        Returns
+        ----------
+        :class:`ForecastData`
+            Fetched forecast data as a class.
+
+        Raises
+        ---------
+        :exc:`NoLocationFound`
+            Raised when no location for given query was found
+        :exc:`InvalidAPIKey`
+            Raised when the API key is invalid
+        :exc:`APILimitExceeded`
+            Raised when API key calls limit was exceeded
+        :exc:`APIKeyDisabled`
+            Raised when API key is disabled
+        :exc:`AccessDenied`
+            Raised when access to given resource was denied
+        :exc:`InternalApplicationError`
+            Raised when there was a very rare internal application error
+        :exc:`WeatherAPIException`
+            Raised when something else went wrong, that does not have a specific exception class.
+        """
+        options = {
+            "aqi": aqi or self.aqi,
+            "q": query,
+            "alerts": alerts or self.kwargs.get("alerts"),
+            **kwargs
+        }
+        if lang is not None: options["lang"] = lang
+
+        resp = self._call_request("forecast.json", options)
+        forecast = ForecastData(resp[0], resp[1].status_code, None)
+        return forecast
+    
+    def __str__(self):
+        return f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>"
+    
+    def __repr__(self):
+        return repr(f"<{self.__class__.__name__} api_key={self.default_options['key']} lang={self.lang}>")
```

## weatherly/api/core.py

```diff
@@ -1,86 +1,86 @@
-"""
-MIT License
-
-Copyright (c) 2023 Konrad (@konradsic)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-
-from typing import (
-    Any,
-    Optional,
-    List,
-    Tuple,
-    Literal,
-    Dict,
-    TypeVar
-)
-import urllib
-import requests
-from ..utils import parse_kwargs_to_urlargs
-import json
-
-T = TypeVar("T")
-
-__all__ = (
-    "BaseAPIClient",
-)
-
-class BaseAPIClient():
-    """
-    Represents a base API client that can handle requests. Used as a base class for ``WeatherAPIClient``
-    
-    Parameters
-    ----------
-    base_url: :class:`str`
-        An URL that will be used as a base for requests.
-    default_options: Optional[Dict[:class:`str`, Any]]
-        Default options for requests made by the client that will be automatically added.
-    """
-    def __init__(
-        self,
-        base_url: str,
-        default_options: Optional[Dict[str, Any]]
-    ) -> None:
-        self.url = base_url
-        self.default_options = default_options or {}
-        
-    def _request(
-        self,
-        path: str,
-        **kwargs: Optional[Dict[str, str]]
-    ) -> Tuple[Dict[Any, Any], requests.Response]:
-        """
-        Request data from the base URL + path.
-        Private function, use ``WeatherAPIClient`` methods instead
-        
-        Parameters
-        ----------
-        path: :class:`str`
-            A path that will be used as an endpoint for the request.
-        kwargs: Optional[Dict[str, str]]
-            Additional parameters for the request.
-        """
-        full_url = self.url + path + parse_kwargs_to_urlargs({**self.default_options, **kwargs})
-
-        response = requests.get(full_url)
-        return response.json(), response
-        
-        
+"""
+MIT License
+
+Copyright (c) 2023 Konrad (@konradsic)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
+from typing import (
+    Any,
+    Optional,
+    List,
+    Tuple,
+    Literal,
+    Dict,
+    TypeVar
+)
+import urllib
+import requests
+from ..utils import parse_kwargs_to_urlargs
+import json
+
+T = TypeVar("T")
+
+__all__ = (
+    "BaseAPIClient",
+)
+
+class BaseAPIClient():
+    """
+    Represents a base API client that can handle requests. Used as a base class for :class:`Client`
+    
+    Parameters
+    ----------
+    base_url: :class:`str`
+        An URL that will be used as a base for requests.
+    default_options: Optional[Dict[:class:`str`, Any]]
+        Default options for requests made by the client that will be automatically added.
+    """
+    def __init__(
+        self,
+        base_url: str,
+        default_options: Optional[Dict[str, Any]]
+    ) -> None:
+        self.url = base_url
+        self.default_options = default_options or {}
+        
+    def _request(
+        self,
+        path: str,
+        **kwargs: Optional[Dict[str, str]]
+    ) -> Tuple[Dict[Any, Any], requests.Response]:
+        """
+        Request data from the base URL + path.
+        Private function, use :class:`Client` methods instead
+        
+        Parameters
+        ----------
+        path: :class:`str`
+            A path that will be used as an endpoint for the request.
+        kwargs: Optional[Dict[str, str]]
+            Additional parameters for the request.
+        """
+        full_url = self.url + path + parse_kwargs_to_urlargs({**self.default_options, **kwargs})
+
+        response = requests.get(full_url)
+        return response.json(), response
+        
+
```

## Comparing `weatherly/__pycache__/enums.cpython-311.pyc` & `weatherly/__pycache__/enums.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Mon Apr 17 07:10:18 2023 UTC, .py size: 4647 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,370 +1,321 @@
-00000000: a70d 0d0a 0000 0000 daf0 3c64 2712 0000  ..........<d'...
-00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 3600 0000 9700 6400 5a00  ......6.....d.Z.
-00000030: 6401 6402 6c01 6d02 5a02 0100 6403 5a03  d.d.l.m.Z...d.Z.
-00000040: 0200 4700 6404 8400 6405 6502 a603 0000  ..G.d...d.e.....
-00000050: ab03 0000 0000 0000 0000 5a04 6406 5300  ..........Z.d.S.
-00000060: 2907 6135 0400 000a 4d49 5420 4c69 6365  ).a5....MIT Lice
-00000070: 6e73 650a 0a43 6f70 7972 6967 6874 2028  nse..Copyright (
-00000080: 6329 2032 3032 3320 4b6f 6e72 6164 2028  c) 2023 Konrad (
-00000090: 406b 6f6e 7261 6473 6963 290a 0a50 6572  @konradsic)..Per
-000000a0: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
-000000b0: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
-000000c0: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
-000000d0: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
-000000e0: 6e67 2061 2063 6f70 790a 6f66 2074 6869  ng a copy.of thi
-000000f0: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
-00000100: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
-00000110: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
-00000120: 6865 2022 536f 6674 7761 7265 2229 2c20  he "Software"), 
-00000130: 746f 2064 6561 6c0a 696e 2074 6865 2053  to deal.in the S
-00000140: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
-00000150: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
-00000160: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
-00000170: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
-00000180: 6768 7473 0a74 6f20 7573 652c 2063 6f70  ghts.to use, cop
-00000190: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
-000001a0: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
-000001b0: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
-000001c0: 652c 2061 6e64 2f6f 7220 7365 6c6c 0a63  e, and/or sell.c
-000001d0: 6f70 6965 7320 6f66 2074 6865 2053 6f66  opies of the Sof
-000001e0: 7477 6172 652c 2061 6e64 2074 6f20 7065  tware, and to pe
-000001f0: 726d 6974 2070 6572 736f 6e73 2074 6f20  rmit persons to 
-00000200: 7768 6f6d 2074 6865 2053 6f66 7477 6172  whom the Softwar
-00000210: 6520 6973 0a66 7572 6e69 7368 6564 2074  e is.furnished t
-00000220: 6f20 646f 2073 6f2c 2073 7562 6a65 6374  o do so, subject
-00000230: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
-00000240: 6720 636f 6e64 6974 696f 6e73 3a0a 0a54  g conditions:..T
-00000250: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
-00000260: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
-00000270: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
-00000280: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
-00000290: 636c 7564 6564 2069 6e20 616c 6c0a 636f  cluded in all.co
-000002a0: 7069 6573 206f 7220 7375 6273 7461 6e74  pies or substant
-000002b0: 6961 6c20 706f 7274 696f 6e73 206f 6620  ial portions of 
-000002c0: 7468 6520 536f 6674 7761 7265 2e0a 0a54  the Software...T
-000002d0: 4845 2053 4f46 5457 4152 4520 4953 2050  HE SOFTWARE IS P
-000002e0: 524f 5649 4445 4420 2241 5320 4953 222c  ROVIDED "AS IS",
-000002f0: 2057 4954 484f 5554 2057 4152 5241 4e54   WITHOUT WARRANT
-00000300: 5920 4f46 2041 4e59 204b 494e 442c 2045  Y OF ANY KIND, E
-00000310: 5850 5245 5353 204f 520a 494d 504c 4945  XPRESS OR.IMPLIE
-00000320: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
-00000330: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
-00000340: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
-00000350: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-00000360: 592c 0a46 4954 4e45 5353 2046 4f52 2041  Y,.FITNESS FOR A
-00000370: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
-00000380: 4f53 4520 414e 4420 4e4f 4e49 4e46 5249  OSE AND NONINFRI
-00000390: 4e47 454d 454e 542e 2049 4e20 4e4f 2045  NGEMENT. IN NO E
-000003a0: 5645 4e54 2053 4841 4c4c 2054 4845 0a41  VENT SHALL THE.A
-000003b0: 5554 484f 5253 204f 5220 434f 5059 5249  UTHORS OR COPYRI
-000003c0: 4748 5420 484f 4c44 4552 5320 4245 204c  GHT HOLDERS BE L
-000003d0: 4941 424c 4520 464f 5220 414e 5920 434c  IABLE FOR ANY CL
-000003e0: 4149 4d2c 2044 414d 4147 4553 204f 5220  AIM, DAMAGES OR 
-000003f0: 4f54 4845 520a 4c49 4142 494c 4954 592c  OTHER.LIABILITY,
-00000400: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
-00000410: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
-00000420: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
-00000430: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
-00000440: 4f4d 2c0a 4f55 5420 4f46 204f 5220 494e  OM,.OUT OF OR IN
-00000450: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
-00000460: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
-00000470: 2054 4845 2055 5345 204f 5220 4f54 4845   THE USE OR OTHE
-00000480: 5220 4445 414c 494e 4753 2049 4e20 5448  R DEALINGS IN TH
-00000490: 450a 534f 4654 5741 5245 2e0a e900 0000  E.SOFTWARE......
-000004a0: 0029 01da 0445 6e75 6d29 01da 094c 616e  .)...Enum)...Lan
-000004b0: 6775 6167 6573 6300 0000 0000 0000 0000  guagesc.........
-000004c0: 0000 0003 0000 0000 0000 00f3 4402 0000  ............D...
-000004d0: 9700 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-000004e0: 6402 5a04 6505 6506 6403 3c00 0000 6404  d.Z.e.e.d.<...d.
-000004f0: 5a07 6505 6506 6405 3c00 0000 6406 5a08  Z.e.e.d.<...d.Z.
-00000500: 6505 6506 6407 3c00 0000 6408 5a09 6505  e.e.d.<...d.Z.e.
-00000510: 6506 6409 3c00 0000 640a 5a0a 6505 6506  e.d.<...d.Z.e.e.
-00000520: 640b 3c00 0000 640c 5a0b 6505 6506 640d  d.<...d.Z.e.e.d.
-00000530: 3c00 0000 640e 5a0c 6505 6506 640f 3c00  <...d.Z.e.e.d.<.
-00000540: 0000 6410 5a0d 6505 6506 6411 3c00 0000  ..d.Z.e.e.d.<...
-00000550: 6412 5a0e 6505 6506 6413 3c00 0000 6414  d.Z.e.e.d.<...d.
-00000560: 5a0f 6505 6506 6415 3c00 0000 6416 5a10  Z.e.e.d.<...d.Z.
-00000570: 6505 6506 6417 3c00 0000 6418 5a11 6505  e.e.d.<...d.Z.e.
-00000580: 6506 6419 3c00 0000 641a 5a12 6505 6506  e.d.<...d.Z.e.e.
-00000590: 641b 3c00 0000 641c 5a13 6505 6506 641d  d.<...d.Z.e.e.d.
-000005a0: 3c00 0000 641e 5a14 6505 6506 641f 3c00  <...d.Z.e.e.d.<.
-000005b0: 0000 6420 5a15 6505 6506 6421 3c00 0000  ..d Z.e.e.d!<...
-000005c0: 6422 5a16 6505 6506 6423 3c00 0000 6424  d"Z.e.e.d#<...d$
-000005d0: 5a17 6505 6506 6425 3c00 0000 6426 5a18  Z.e.e.d%<...d&Z.
-000005e0: 6505 6506 6427 3c00 0000 6428 5a19 6505  e.e.d'<...d(Z.e.
-000005f0: 6506 6429 3c00 0000 642a 5a1a 6505 6506  e.d)<...d*Z.e.e.
-00000600: 642b 3c00 0000 642c 5a1b 6505 6506 642d  d+<...d,Z.e.e.d-
-00000610: 3c00 0000 642e 5a1c 6505 6506 642f 3c00  <...d.Z.e.e.d/<.
-00000620: 0000 6430 5a1d 6505 6506 6431 3c00 0000  ..d0Z.e.e.d1<...
-00000630: 6432 5a1e 6505 6506 6433 3c00 0000 6434  d2Z.e.e.d3<...d4
-00000640: 5a1f 6505 6506 6435 3c00 0000 6436 5a20  Z.e.e.d5<...d6Z 
-00000650: 6505 6506 6437 3c00 0000 6438 5a21 6505  e.e.d7<...d8Z!e.
-00000660: 6506 6439 3c00 0000 643a 5a22 6505 6506  e.d9<...d:Z"e.e.
-00000670: 643b 3c00 0000 643c 5a23 6505 6506 643d  d;<...d<Z#e.e.d=
-00000680: 3c00 0000 643e 5a24 6505 6506 643f 3c00  <...d>Z$e.e.d?<.
-00000690: 0000 6440 5a25 6505 6506 6441 3c00 0000  ..d@Z%e.e.dA<...
-000006a0: 6442 5a26 6505 6506 6443 3c00 0000 6444  dBZ&e.e.dC<...dD
-000006b0: 5a27 6505 6506 6445 3c00 0000 6446 5a28  Z'e.e.dE<...dFZ(
-000006c0: 6505 6506 6447 3c00 0000 6448 5a29 6505  e.e.dG<...dHZ)e.
-000006d0: 6506 6449 3c00 0000 644a 5a2a 6505 6506  e.dI<...dJZ*e.e.
-000006e0: 644b 3c00 0000 644c 5a2b 6505 6506 644d  dK<...dLZ+e.e.dM
-000006f0: 3c00 0000 644e 5a2c 6505 6506 644f 3c00  <...dNZ,e.e.dO<.
-00000700: 0000 6450 5a2d 6505 6506 6451 3c00 0000  ..dPZ-e.e.dQ<...
-00000710: 6452 5300 2953 7204 0000 0061 0609 0000  dRS.)Sr....a....
-00000720: 0a20 2020 204c 616e 6775 6167 6573 202d  .    Languages -
-00000730: 2061 6e20 656e 756d 2072 6570 7265 7365   an enum represe
-00000740: 6e74 696e 6720 6c61 6e67 7561 6765 7320  nting languages 
-00000750: 6176 6169 6c61 626c 6520 666f 7220 7573  available for us
-00000760: 6520 696e 2074 6865 2057 6561 7468 6572  e in the Weather
-00000770: 4150 4920 7265 7175 6573 7473 2e0a 2020  API requests..  
-00000780: 2020 0a20 2020 2041 7474 7269 6275 7465    .    Attribute
-00000790: 7320 6172 6520 6c61 6e67 7561 6765 7320  s are languages 
-000007a0: 616e 6420 6c61 6e67 7561 6765 2063 6f64  and language cod
-000007b0: 6573 0a20 2020 200a 2020 2020 4174 7472  es.    .    Attr
-000007c0: 6962 7574 6573 0a20 2020 202d 2d2d 2d2d  ibutes.    -----
-000007d0: 2d2d 2d2d 2d0a 2020 2020 4172 6162 6963  -----.    Arabic
-000007e0: 3a20 3a63 6c61 7373 3a60 7374 7260 0a20  : :class:`str`. 
-000007f0: 2020 2020 2020 204c 616e 6775 6167 6520         Language 
-00000800: 636f 6465 3a20 6172 0a20 2020 2042 656e  code: ar.    Ben
-00000810: 6761 6c69 3a20 3a63 6c61 7373 3a60 7374  gali: :class:`st
-00000820: 7260 0a20 2020 2020 2020 204c 616e 6775  r`.        Langu
-00000830: 6167 6520 636f 6465 3a20 626e 0a20 2020  age code: bn.   
-00000840: 2042 756c 6761 7269 616e 3a20 3a63 6c61   Bulgarian: :cla
-00000850: 7373 3a60 7374 7260 0a20 2020 2020 2020  ss:`str`.       
-00000860: 204c 616e 6775 6167 6520 636f 6465 3a20   Language code: 
-00000870: 6267 0a20 2020 2043 6869 6e65 7365 5369  bg.    ChineseSi
-00000880: 6d70 6c69 6669 6564 3a20 3a63 6c61 7373  mplified: :class
-00000890: 3a60 7374 7260 0a20 2020 2020 2020 204c  :`str`.        L
-000008a0: 616e 6775 6167 6520 636f 6465 3a20 7a68  anguage code: zh
-000008b0: 0a20 2020 2043 6869 6e65 7365 5472 6164  .    ChineseTrad
-000008c0: 6974 696f 6e61 6c3a 203a 636c 6173 733a  itional: :class:
-000008d0: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
-000008e0: 6e67 7561 6765 2063 6f64 653a 207a 685f  nguage code: zh_
-000008f0: 7477 0a20 2020 2043 7a65 6368 3a20 3a63  tw.    Czech: :c
-00000900: 6c61 7373 3a60 7374 7260 0a20 2020 2020  lass:`str`.     
-00000910: 2020 204c 616e 6775 6167 6520 636f 6465     Language code
-00000920: 3a20 6373 0a20 2020 2044 616e 6973 683a  : cs.    Danish:
-00000930: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
-00000940: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
-00000950: 6f64 653a 2064 610a 2020 2020 4475 7463  ode: da.    Dutc
-00000960: 683a 203a 636c 6173 733a 6073 7472 600a  h: :class:`str`.
-00000970: 2020 2020 2020 2020 4c61 6e67 7561 6765          Language
-00000980: 2063 6f64 653a 206e 6c0a 2020 2020 4669   code: nl.    Fi
-00000990: 6e6e 6973 683a 203a 636c 6173 733a 6073  nnish: :class:`s
-000009a0: 7472 600a 2020 2020 2020 2020 4c61 6e67  tr`.        Lang
-000009b0: 7561 6765 2063 6f64 653a 2066 690a 2020  uage code: fi.  
-000009c0: 2020 4672 656e 6368 3a20 3a63 6c61 7373    French: :class
-000009d0: 3a60 7374 7260 0a20 2020 2020 2020 204c  :`str`.        L
-000009e0: 616e 6775 6167 6520 636f 6465 3a20 6672  anguage code: fr
-000009f0: 0a20 2020 2047 6572 6d61 6e3a 203a 636c  .    German: :cl
-00000a00: 6173 733a 6073 7472 600a 2020 2020 2020  ass:`str`.      
-00000a10: 2020 4c61 6e67 7561 6765 2063 6f64 653a    Language code:
-00000a20: 2064 650a 2020 2020 4772 6565 6b3a 203a   de.    Greek: :
-00000a30: 636c 6173 733a 6073 7472 600a 2020 2020  class:`str`.    
-00000a40: 2020 2020 4c61 6e67 7561 6765 2063 6f64      Language cod
-00000a50: 653a 2065 6c0a 2020 2020 4869 6e64 693a  e: el.    Hindi:
-00000a60: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
-00000a70: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
-00000a80: 6f64 653a 2068 690a 2020 2020 4875 6e67  ode: hi.    Hung
-00000a90: 6172 6961 6e3a 203a 636c 6173 733a 6073  arian: :class:`s
-00000aa0: 7472 600a 2020 2020 2020 2020 4c61 6e67  tr`.        Lang
-00000ab0: 7561 6765 2063 6f64 653a 2068 750a 2020  uage code: hu.  
-00000ac0: 2020 4974 616c 6961 6e3a 203a 636c 6173    Italian: :clas
-00000ad0: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
-00000ae0: 4c61 6e67 7561 6765 2063 6f64 653a 2069  Language code: i
-00000af0: 740a 2020 2020 4a61 7061 6e65 7365 3a20  t.    Japanese: 
-00000b00: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
-00000b10: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
-00000b20: 6465 3a20 6a61 0a20 2020 204a 6176 616e  de: ja.    Javan
-00000b30: 6573 653a 203a 636c 6173 733a 6073 7472  ese: :class:`str
-00000b40: 600a 2020 2020 2020 2020 4c61 6e67 7561  `.        Langua
-00000b50: 6765 2063 6f64 653a 206a 760a 2020 2020  ge code: jv.    
-00000b60: 4b6f 7265 616e 3a20 3a63 6c61 7373 3a60  Korean: :class:`
-00000b70: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
-00000b80: 6775 6167 6520 636f 6465 3a20 6b6f 0a20  guage code: ko. 
-00000b90: 2020 204d 616e 6461 7269 6e3a 203a 636c     Mandarin: :cl
-00000ba0: 6173 733a 6073 7472 600a 2020 2020 2020  ass:`str`.      
-00000bb0: 2020 4c61 6e67 7561 6765 2063 6f64 653a    Language code:
-00000bc0: 207a 685f 636d 6e0a 2020 2020 4d61 7261   zh_cmn.    Mara
-00000bd0: 7468 693a 203a 636c 6173 733a 6073 7472  thi: :class:`str
-00000be0: 600a 2020 2020 2020 2020 4c61 6e67 7561  `.        Langua
-00000bf0: 6765 2063 6f64 653a 206d 720a 2020 2020  ge code: mr.    
-00000c00: 506f 6c69 7368 3a20 3a63 6c61 7373 3a60  Polish: :class:`
-00000c10: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
-00000c20: 6775 6167 6520 636f 6465 3a20 706c 0a20  guage code: pl. 
-00000c30: 2020 2050 6f72 7475 6775 6573 653a 203a     Portuguese: :
-00000c40: 636c 6173 733a 6073 7472 600a 2020 2020  class:`str`.    
-00000c50: 2020 2020 4c61 6e67 7561 6765 2063 6f64      Language cod
-00000c60: 653a 2070 740a 2020 2020 5075 6e6a 6162  e: pt.    Punjab
-00000c70: 693a 203a 636c 6173 733a 6073 7472 600a  i: :class:`str`.
-00000c80: 2020 2020 2020 2020 4c61 6e67 7561 6765          Language
-00000c90: 2063 6f64 653a 2070 610a 2020 2020 526f   code: pa.    Ro
-00000ca0: 6d61 6e69 616e 3a20 3a63 6c61 7373 3a60  manian: :class:`
-00000cb0: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
-00000cc0: 6775 6167 6520 636f 6465 3a20 726f 0a20  guage code: ro. 
-00000cd0: 2020 2052 7573 7369 616e 3a20 3a63 6c61     Russian: :cla
-00000ce0: 7373 3a60 7374 7260 0a20 2020 2020 2020  ss:`str`.       
-00000cf0: 204c 616e 6775 6167 6520 636f 6465 3a20   Language code: 
-00000d00: 7275 0a20 2020 2053 6572 6269 616e 3a20  ru.    Serbian: 
-00000d10: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
-00000d20: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
-00000d30: 6465 3a20 7372 0a20 2020 2053 696e 6861  de: sr.    Sinha
-00000d40: 6c65 7365 3a20 3a63 6c61 7373 3a60 7374  lese: :class:`st
-00000d50: 7260 0a20 2020 2020 2020 204c 616e 6775  r`.        Langu
-00000d60: 6167 6520 636f 6465 3a20 7369 0a20 2020  age code: si.   
-00000d70: 2053 6c6f 7661 6b3a 203a 636c 6173 733a   Slovak: :class:
-00000d80: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
-00000d90: 6e67 7561 6765 2063 6f64 653a 2073 6b0a  nguage code: sk.
-00000da0: 2020 2020 5370 616e 6973 683a 203a 636c      Spanish: :cl
-00000db0: 6173 733a 6073 7472 600a 2020 2020 2020  ass:`str`.      
-00000dc0: 2020 4c61 6e67 7561 6765 2063 6f64 653a    Language code:
-00000dd0: 2065 730a 2020 2020 5377 6564 6973 683a   es.    Swedish:
-00000de0: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
-00000df0: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
-00000e00: 6f64 653a 2073 760a 2020 2020 5461 6d69  ode: sv.    Tami
-00000e10: 6c3a 203a 636c 6173 733a 6073 7472 600a  l: :class:`str`.
-00000e20: 2020 2020 2020 2020 4c61 6e67 7561 6765          Language
-00000e30: 2063 6f64 653a 2074 610a 2020 2020 5465   code: ta.    Te
-00000e40: 6c75 6775 3a20 3a63 6c61 7373 3a60 7374  lugu: :class:`st
-00000e50: 7260 0a20 2020 2020 2020 204c 616e 6775  r`.        Langu
-00000e60: 6167 6520 636f 6465 3a20 7465 0a20 2020  age code: te.   
-00000e70: 2054 7572 6b69 7368 3a20 3a63 6c61 7373   Turkish: :class
-00000e80: 3a60 7374 7260 0a20 2020 2020 2020 204c  :`str`.        L
-00000e90: 616e 6775 6167 6520 636f 6465 3a20 7472  anguage code: tr
-00000ea0: 0a20 2020 2055 6b72 6169 6e69 616e 3a20  .    Ukrainian: 
-00000eb0: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
-00000ec0: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
-00000ed0: 6465 3a20 756b 0a20 2020 2055 7264 753a  de: uk.    Urdu:
-00000ee0: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
-00000ef0: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
-00000f00: 6f64 653a 2075 720a 2020 2020 5669 6574  ode: ur.    Viet
-00000f10: 6e61 6d65 7365 3a20 3a63 6c61 7373 3a60  namese: :class:`
-00000f20: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
-00000f30: 6775 6167 6520 636f 6465 3a20 7669 0a20  guage code: vi. 
-00000f40: 2020 2057 7553 6861 6e67 6861 696e 6573     WuShanghaines
-00000f50: 653a 203a 636c 6173 733a 6073 7472 600a  e: :class:`str`.
-00000f60: 2020 2020 2020 2020 4c61 6e67 7561 6765          Language
-00000f70: 2063 6f64 653a 207a 685f 7775 750a 2020   code: zh_wuu.  
-00000f80: 2020 5869 616e 673a 203a 636c 6173 733a    Xiang: :class:
-00000f90: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
-00000fa0: 6e67 7561 6765 2063 6f64 653a 207a 685f  nguage code: zh_
-00000fb0: 6873 6e0a 2020 2020 5975 6543 616e 746f  hsn.    YueCanto
-00000fc0: 6e65 7365 3a20 3a63 6c61 7373 3a60 7374  nese: :class:`st
-00000fd0: 7260 0a20 2020 2020 2020 204c 616e 6775  r`.        Langu
-00000fe0: 6167 6520 636f 6465 3a20 7a68 5f79 7565  age code: zh_yue
-00000ff0: 0a20 2020 205a 756c 753a 203a 636c 6173  .    Zulu: :clas
-00001000: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
-00001010: 4c61 6e67 7561 6765 2063 6f64 653a 207a  Language code: z
-00001020: 750a 2020 2020 da02 6172 da06 4172 6162  u.    ..ar..Arab
-00001030: 6963 da02 626e da07 4265 6e67 616c 69da  ic..bn..Bengali.
-00001040: 0262 67da 0942 756c 6761 7269 616e da02  .bg..Bulgarian..
-00001050: 7a68 da11 4368 696e 6573 6553 696d 706c  zh..ChineseSimpl
-00001060: 6966 6965 64da 057a 685f 7477 da12 4368  ified..zh_tw..Ch
-00001070: 696e 6573 6554 7261 6469 7469 6f6e 616c  ineseTraditional
-00001080: da02 6373 da05 437a 6563 68da 0264 61da  ..cs..Czech..da.
-00001090: 0644 616e 6973 68da 026e 6cda 0544 7574  .Danish..nl..Dut
-000010a0: 6368 da02 6669 da07 4669 6e6e 6973 68da  ch..fi..Finnish.
-000010b0: 0266 72da 0646 7265 6e63 68da 0264 65da  .fr..French..de.
-000010c0: 0647 6572 6d61 6eda 0265 6cda 0547 7265  .German..el..Gre
-000010d0: 656b da02 6869 da05 4869 6e64 69da 0268  ek..hi..Hindi..h
-000010e0: 75da 0948 756e 6761 7269 616e da02 6974  u..Hungarian..it
-000010f0: da07 4974 616c 6961 6eda 026a 61da 084a  ..Italian..ja..J
-00001100: 6170 616e 6573 65da 026a 76da 084a 6176  apanese..jv..Jav
-00001110: 616e 6573 65da 026b 6fda 064b 6f72 6561  anese..ko..Korea
-00001120: 6eda 067a 685f 636d 6eda 084d 616e 6461  n..zh_cmn..Manda
-00001130: 7269 6eda 026d 72da 074d 6172 6174 6869  rin..mr..Marathi
-00001140: da02 706c da06 506f 6c69 7368 da02 7074  ..pl..Polish..pt
-00001150: da0a 506f 7274 7567 7565 7365 da02 7061  ..Portuguese..pa
-00001160: da07 5075 6e6a 6162 69da 0272 6fda 0852  ..Punjabi..ro..R
-00001170: 6f6d 616e 6961 6eda 0272 75da 0752 7573  omanian..ru..Rus
-00001180: 7369 616e da02 7372 da07 5365 7262 6961  sian..sr..Serbia
-00001190: 6eda 0273 69da 0953 696e 6861 6c65 7365  n..si..Sinhalese
-000011a0: da02 736b da06 536c 6f76 616b da02 6573  ..sk..Slovak..es
-000011b0: da07 5370 616e 6973 68da 0273 76da 0753  ..Spanish..sv..S
-000011c0: 7765 6469 7368 da02 7461 da05 5461 6d69  wedish..ta..Tami
-000011d0: 6cda 0274 65da 0654 656c 7567 75da 0274  l..te..Telugu..t
-000011e0: 72da 0754 7572 6b69 7368 da02 756b da09  r..Turkish..uk..
-000011f0: 556b 7261 696e 6961 6eda 0275 72da 0455  Ukrainian..ur..U
-00001200: 7264 75da 0276 69da 0a56 6965 746e 616d  rdu..vi..Vietnam
-00001210: 6573 65da 067a 685f 7775 75da 0e57 7553  ese..zh_wuu..WuS
-00001220: 6861 6e67 6861 696e 6573 65da 067a 685f  hanghainese..zh_
-00001230: 6873 6eda 0558 6961 6e67 da06 7a68 5f79  hsn..Xiang..zh_y
-00001240: 7565 da0c 5975 6543 616e 746f 6e65 7365  ue..YueCantonese
-00001250: da02 7a75 da04 5a75 6c75 4e29 2eda 085f  ..zu..ZuluN)..._
-00001260: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00001270: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00001280: 5fda 075f 5f64 6f63 5f5f 7207 0000 00da  _..__doc__r.....
-00001290: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-000012a0: 6f6e 735f 5f72 0900 0000 720b 0000 0072  ons__r....r....r
-000012b0: 0d00 0000 720f 0000 0072 1100 0000 7213  ....r....r....r.
-000012c0: 0000 0072 1500 0000 7217 0000 0072 1900  ...r....r....r..
-000012d0: 0000 721b 0000 0072 1d00 0000 721f 0000  ..r....r....r...
-000012e0: 0072 2100 0000 7223 0000 0072 2500 0000  .r!...r#...r%...
-000012f0: 7227 0000 0072 2900 0000 722b 0000 0072  r'...r)...r+...r
-00001300: 2d00 0000 722f 0000 0072 3100 0000 7233  -...r/...r1...r3
-00001310: 0000 0072 3500 0000 7237 0000 0072 3900  ...r5...r7...r9.
-00001320: 0000 723b 0000 0072 3d00 0000 723f 0000  ..r;...r=...r?..
-00001330: 0072 4100 0000 7243 0000 0072 4500 0000  .rA...rC...rE...
-00001340: 7247 0000 0072 4900 0000 724b 0000 0072  rG...rI...rK...r
-00001350: 4d00 0000 724f 0000 0072 5100 0000 7253  M...rO...rQ...rS
-00001360: 0000 0072 5500 0000 a900 f300 0000 00fa  ...rU...........
-00001370: 2c62 7569 6c64 5c62 6469 7374 2e77 696e  ,build\bdist.win
-00001380: 2d61 6d64 3634 5c65 6767 5c77 6561 7468  -amd64\egg\weath
-00001390: 6572 6c79 5c65 6e75 6d73 2e70 7972 0400  erly\enums.pyr..
-000013a0: 0000 7204 0000 001f 0000 0073 a302 0000  ..r........s....
-000013b0: 8000 8000 8000 8000 8000 8000 f002 5701  ..............W.
-000013c0: 0508 f000 5701 0508 f070 0200 1317 8046  ....W....p.....F
-000013d0: 8843 d004 16d0 0416 d104 16d8 1317 8047  .C.............G
-000013e0: 8853 d004 17d0 0417 d104 17d8 1519 8049  .S.............I
-000013f0: 8873 d004 19d0 0419 d104 19d8 1d21 d004  .s...........!..
-00001400: 1590 73d0 0421 d004 21d1 0421 d81e 25d0  ..s..!..!..!..%.
-00001410: 0416 9803 d004 25d0 0425 d104 25d8 1115  ......%..%..%...
-00001420: 8045 8833 d004 15d0 0415 d104 15d8 1216  .E.3............
-00001430: 8046 8843 d004 16d0 0416 d104 16d8 1115  .F.C............
-00001440: 8045 8833 d004 15d0 0415 d104 15d8 1317  .E.3............
-00001450: 8047 8853 d004 17d0 0417 d104 17d8 1216  .G.S............
-00001460: 8046 8843 d004 16d0 0416 d104 16d8 1216  .F.C............
-00001470: 8046 8843 d004 16d0 0416 d104 16d8 1115  .F.C............
-00001480: 8045 8833 d004 15d0 0415 d104 15d8 1115  .E.3............
-00001490: 8045 8833 d004 15d0 0415 d104 15d8 1519  .E.3............
-000014a0: 8049 8873 d004 19d0 0419 d104 19d8 1317  .I.s............
-000014b0: 8047 8853 d004 17d0 0417 d104 17d8 1418  .G.S............
-000014c0: 8048 8863 d004 18d0 0418 d104 18d8 1418  .H.c............
-000014d0: 8048 8863 d004 18d0 0418 d104 18d8 1216  .H.c............
-000014e0: 8046 8843 d004 16d0 0416 d104 16d8 141c  .F.C............
-000014f0: 8048 8863 d004 1cd0 041c d104 1cd8 1317  .H.c............
-00001500: 8047 8853 d004 17d0 0417 d104 17d8 1216  .G.S............
-00001510: 8046 8843 d004 16d0 0416 d104 16d8 161a  .F.C............
-00001520: 804a 9003 d004 1ad0 041a d104 1ad8 1317  .J..............
-00001530: 8047 8853 d004 17d0 0417 d104 17d8 1418  .G.S............
-00001540: 8048 8863 d004 18d0 0418 d104 18d8 1317  .H.c............
-00001550: 8047 8853 d004 17d0 0417 d104 17d8 1317  .G.S............
-00001560: 8047 8853 d004 17d0 0417 d104 17d8 1519  .G.S............
-00001570: 8049 8873 d004 19d0 0419 d104 19d8 1216  .I.s............
-00001580: 8046 8843 d004 16d0 0416 d104 16d8 1317  .F.C............
-00001590: 8047 8853 d004 17d0 0417 d104 17d8 1317  .G.S............
-000015a0: 8047 8853 d004 17d0 0417 d104 17d8 1115  .G.S............
-000015b0: 8045 8833 d004 15d0 0415 d104 15d8 1216  .E.3............
-000015c0: 8046 8843 d004 16d0 0416 d104 16d8 1317  .F.C............
-000015d0: 8047 8853 d004 17d0 0417 d104 17d8 1519  .G.S............
-000015e0: 8049 8873 d004 19d0 0419 d104 19d8 1014  .I.s............
-000015f0: 8044 8823 d004 14d0 0414 d104 14d8 161a  .D.#............
-00001600: 804a 9003 d004 1ad0 041a d104 1ad8 1a22  .J............."
-00001610: 804e 9043 d004 22d0 0422 d104 22d8 1119  .N.C.."..".."...
-00001620: 8045 8833 d004 19d0 0419 d104 19d8 1820  .E.3........... 
-00001630: 804c 9023 d004 20d0 0420 d104 20d8 1014  .L.#.. .. .. ...
-00001640: 8044 8823 d004 14d0 0414 d104 14d0 0414  .D.#............
-00001650: d004 1472 5d00 0000 7204 0000 004e 2905  ...r]...r....N).
-00001660: 7259 0000 00da 0465 6e75 6d72 0300 0000  rY.....enumr....
-00001670: da07 5f5f 616c 6c5f 5f72 0400 0000 725c  ..__all__r....r\
-00001680: 0000 0072 5d00 0000 725e 0000 00fa 083c  ...r]...r^.....<
-00001690: 6d6f 6475 6c65 3e72 6100 0000 0100 0000  module>ra.......
-000016a0: 7368 0000 00f0 0301 0101 f002 1601 04f0  sh..............
-000016b0: 0016 0104 f030 0001 16d0 0015 d000 15d0  .....0..........
-000016c0: 0015 d000 15d0 0015 f004 020b 0280 07f0  ................
-000016d0: 0840 0201 15f0 0040 0201 15f0 0040 0201  .@.....@.....@..
-000016e0: 15f0 0040 0201 15f0 0040 0201 1590 04f1  ...@.....@......
-000016f0: 0040 0201 15f4 0040 0201 15f0 0040 0201  .@.....@.....@..
-00001700: 15f0 0040 0201 15f0 0040 0201 1572 5d00  ...@.....@...r].
-00001710: 0000                                     ..
+00000000: 6f0d 0d0a 0000 0000 2a63 3c64 8811 0000  o.......*c<d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
+00000040: 5a03 4700 6404 6405 8400 6405 6502 8303  Z.G.d.d...d.e...
+00000050: 5a04 6406 5300 2907 6135 0400 000a 4d49  Z.d.S.).a5....MI
+00000060: 5420 4c69 6365 6e73 650a 0a43 6f70 7972  T License..Copyr
+00000070: 6967 6874 2028 6329 2032 3032 3320 4b6f  ight (c) 2023 Ko
+00000080: 6e72 6164 2028 406b 6f6e 7261 6473 6963  nrad (@konradsic
+00000090: 290a 0a50 6572 6d69 7373 696f 6e20 6973  )..Permission is
+000000a0: 2068 6572 6562 7920 6772 616e 7465 642c   hereby granted,
+000000b0: 2066 7265 6520 6f66 2063 6861 7267 652c   free of charge,
+000000c0: 2074 6f20 616e 7920 7065 7273 6f6e 206f   to any person o
+000000d0: 6274 6169 6e69 6e67 2061 2063 6f70 790a  btaining a copy.
+000000e0: 6f66 2074 6869 7320 736f 6674 7761 7265  of this software
+000000f0: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
+00000100: 646f 6375 6d65 6e74 6174 696f 6e20 6669  documentation fi
+00000110: 6c65 7320 2874 6865 2022 536f 6674 7761  les (the "Softwa
+00000120: 7265 2229 2c20 746f 2064 6561 6c0a 696e  re"), to deal.in
+00000130: 2074 6865 2053 6f66 7477 6172 6520 7769   the Software wi
+00000140: 7468 6f75 7420 7265 7374 7269 6374 696f  thout restrictio
+00000150: 6e2c 2069 6e63 6c75 6469 6e67 2077 6974  n, including wit
+00000160: 686f 7574 206c 696d 6974 6174 696f 6e20  hout limitation 
+00000170: 7468 6520 7269 6768 7473 0a74 6f20 7573  the rights.to us
+00000180: 652c 2063 6f70 792c 206d 6f64 6966 792c  e, copy, modify,
+00000190: 206d 6572 6765 2c20 7075 626c 6973 682c   merge, publish,
+000001a0: 2064 6973 7472 6962 7574 652c 2073 7562   distribute, sub
+000001b0: 6c69 6365 6e73 652c 2061 6e64 2f6f 7220  license, and/or 
+000001c0: 7365 6c6c 0a63 6f70 6965 7320 6f66 2074  sell.copies of t
+000001d0: 6865 2053 6f66 7477 6172 652c 2061 6e64  he Software, and
+000001e0: 2074 6f20 7065 726d 6974 2070 6572 736f   to permit perso
+000001f0: 6e73 2074 6f20 7768 6f6d 2074 6865 2053  ns to whom the S
+00000200: 6f66 7477 6172 6520 6973 0a66 7572 6e69  oftware is.furni
+00000210: 7368 6564 2074 6f20 646f 2073 6f2c 2073  shed to do so, s
+00000220: 7562 6a65 6374 2074 6f20 7468 6520 666f  ubject to the fo
+00000230: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
+00000240: 6e73 3a0a 0a54 6865 2061 626f 7665 2063  ns:..The above c
+00000250: 6f70 7972 6967 6874 206e 6f74 6963 6520  opyright notice 
+00000260: 616e 6420 7468 6973 2070 6572 6d69 7373  and this permiss
+00000270: 696f 6e20 6e6f 7469 6365 2073 6861 6c6c  ion notice shall
+00000280: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
+00000290: 616c 6c0a 636f 7069 6573 206f 7220 7375  all.copies or su
+000002a0: 6273 7461 6e74 6961 6c20 706f 7274 696f  bstantial portio
+000002b0: 6e73 206f 6620 7468 6520 536f 6674 7761  ns of the Softwa
+000002c0: 7265 2e0a 0a54 4845 2053 4f46 5457 4152  re...THE SOFTWAR
+000002d0: 4520 4953 2050 524f 5649 4445 4420 2241  E IS PROVIDED "A
+000002e0: 5320 4953 222c 2057 4954 484f 5554 2057  S IS", WITHOUT W
+000002f0: 4152 5241 4e54 5920 4f46 2041 4e59 204b  ARRANTY OF ANY K
+00000300: 494e 442c 2045 5850 5245 5353 204f 520a  IND, EXPRESS OR.
+00000310: 494d 504c 4945 442c 2049 4e43 4c55 4449  IMPLIED, INCLUDI
+00000320: 4e47 2042 5554 204e 4f54 204c 494d 4954  NG BUT NOT LIMIT
+00000330: 4544 2054 4f20 5448 4520 5741 5252 414e  ED TO THE WARRAN
+00000340: 5449 4553 204f 4620 4d45 5243 4841 4e54  TIES OF MERCHANT
+00000350: 4142 494c 4954 592c 0a46 4954 4e45 5353  ABILITY,.FITNESS
+00000360: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
+00000370: 5220 5055 5250 4f53 4520 414e 4420 4e4f  R PURPOSE AND NO
+00000380: 4e49 4e46 5249 4e47 454d 454e 542e 2049  NINFRINGEMENT. I
+00000390: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
+000003a0: 2054 4845 0a41 5554 484f 5253 204f 5220   THE.AUTHORS OR 
+000003b0: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
+000003c0: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
+000003d0: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
+000003e0: 4553 204f 5220 4f54 4845 520a 4c49 4142  ES OR OTHER.LIAB
+000003f0: 494c 4954 592c 2057 4845 5448 4552 2049  ILITY, WHETHER I
+00000400: 4e20 414e 2041 4354 494f 4e20 4f46 2043  N AN ACTION OF C
+00000410: 4f4e 5452 4143 542c 2054 4f52 5420 4f52  ONTRACT, TORT OR
+00000420: 204f 5448 4552 5749 5345 2c20 4152 4953   OTHERWISE, ARIS
+00000430: 494e 4720 4652 4f4d 2c0a 4f55 5420 4f46  ING FROM,.OUT OF
+00000440: 204f 5220 494e 2043 4f4e 4e45 4354 494f   OR IN CONNECTIO
+00000450: 4e20 5749 5448 2054 4845 2053 4f46 5457  N WITH THE SOFTW
+00000460: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
+00000470: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
+00000480: 2049 4e20 5448 450a 534f 4654 5741 5245   IN THE.SOFTWARE
+00000490: 2e0a e900 0000 0029 01da 0445 6e75 6d29  .......)...Enum)
+000004a0: 01da 094c 616e 6775 6167 6573 6300 0000  ...Languagesc...
+000004b0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000004c0: 0040 0000 0073 f201 0000 6500 5a01 6400  .@...s....e.Z.d.
+000004d0: 5a02 5500 6401 5a03 6402 5a04 6505 6506  Z.U.d.Z.d.Z.e.e.
+000004e0: 6403 3c00 6404 5a07 6505 6506 6405 3c00  d.<.d.Z.e.e.d.<.
+000004f0: 6406 5a08 6505 6506 6407 3c00 6408 5a09  d.Z.e.e.d.<.d.Z.
+00000500: 6505 6506 6409 3c00 640a 5a0a 6505 6506  e.e.d.<.d.Z.e.e.
+00000510: 640b 3c00 640c 5a0b 6505 6506 640d 3c00  d.<.d.Z.e.e.d.<.
+00000520: 640e 5a0c 6505 6506 640f 3c00 6410 5a0d  d.Z.e.e.d.<.d.Z.
+00000530: 6505 6506 6411 3c00 6412 5a0e 6505 6506  e.e.d.<.d.Z.e.e.
+00000540: 6413 3c00 6414 5a0f 6505 6506 6415 3c00  d.<.d.Z.e.e.d.<.
+00000550: 6416 5a10 6505 6506 6417 3c00 6418 5a11  d.Z.e.e.d.<.d.Z.
+00000560: 6505 6506 6419 3c00 641a 5a12 6505 6506  e.e.d.<.d.Z.e.e.
+00000570: 641b 3c00 641c 5a13 6505 6506 641d 3c00  d.<.d.Z.e.e.d.<.
+00000580: 641e 5a14 6505 6506 641f 3c00 6420 5a15  d.Z.e.e.d.<.d Z.
+00000590: 6505 6506 6421 3c00 6422 5a16 6505 6506  e.e.d!<.d"Z.e.e.
+000005a0: 6423 3c00 6424 5a17 6505 6506 6425 3c00  d#<.d$Z.e.e.d%<.
+000005b0: 6426 5a18 6505 6506 6427 3c00 6428 5a19  d&Z.e.e.d'<.d(Z.
+000005c0: 6505 6506 6429 3c00 642a 5a1a 6505 6506  e.e.d)<.d*Z.e.e.
+000005d0: 642b 3c00 642c 5a1b 6505 6506 642d 3c00  d+<.d,Z.e.e.d-<.
+000005e0: 642e 5a1c 6505 6506 642f 3c00 6430 5a1d  d.Z.e.e.d/<.d0Z.
+000005f0: 6505 6506 6431 3c00 6432 5a1e 6505 6506  e.e.d1<.d2Z.e.e.
+00000600: 6433 3c00 6434 5a1f 6505 6506 6435 3c00  d3<.d4Z.e.e.d5<.
+00000610: 6436 5a20 6505 6506 6437 3c00 6438 5a21  d6Z e.e.d7<.d8Z!
+00000620: 6505 6506 6439 3c00 643a 5a22 6505 6506  e.e.d9<.d:Z"e.e.
+00000630: 643b 3c00 643c 5a23 6505 6506 643d 3c00  d;<.d<Z#e.e.d=<.
+00000640: 643e 5a24 6505 6506 643f 3c00 6440 5a25  d>Z$e.e.d?<.d@Z%
+00000650: 6505 6506 6441 3c00 6442 5a26 6505 6506  e.e.dA<.dBZ&e.e.
+00000660: 6443 3c00 6444 5a27 6505 6506 6445 3c00  dC<.dDZ'e.e.dE<.
+00000670: 6446 5a28 6505 6506 6447 3c00 6448 5a29  dFZ(e.e.dG<.dHZ)
+00000680: 6505 6506 6449 3c00 644a 5a2a 6505 6506  e.e.dI<.dJZ*e.e.
+00000690: 644b 3c00 644c 5a2b 6505 6506 644d 3c00  dK<.dLZ+e.e.dM<.
+000006a0: 644e 5a2c 6505 6506 644f 3c00 6450 5a2d  dNZ,e.e.dO<.dPZ-
+000006b0: 6505 6506 6451 3c00 6452 5300 2953 7203  e.e.dQ<.dRS.)Sr.
+000006c0: 0000 0061 0609 0000 0a20 2020 204c 616e  ...a.....    Lan
+000006d0: 6775 6167 6573 202d 2061 6e20 656e 756d  guages - an enum
+000006e0: 2072 6570 7265 7365 6e74 696e 6720 6c61   representing la
+000006f0: 6e67 7561 6765 7320 6176 6169 6c61 626c  nguages availabl
+00000700: 6520 666f 7220 7573 6520 696e 2074 6865  e for use in the
+00000710: 2057 6561 7468 6572 4150 4920 7265 7175   WeatherAPI requ
+00000720: 6573 7473 2e0a 2020 2020 0a20 2020 2041  ests..    .    A
+00000730: 7474 7269 6275 7465 7320 6172 6520 6c61  ttributes are la
+00000740: 6e67 7561 6765 7320 616e 6420 6c61 6e67  nguages and lang
+00000750: 7561 6765 2063 6f64 6573 0a20 2020 200a  uage codes.    .
+00000760: 2020 2020 4174 7472 6962 7574 6573 0a20      Attributes. 
+00000770: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000780: 2020 4172 6162 6963 3a20 3a63 6c61 7373    Arabic: :class
+00000790: 3a60 7374 7260 0a20 2020 2020 2020 204c  :`str`.        L
+000007a0: 616e 6775 6167 6520 636f 6465 3a20 6172  anguage code: ar
+000007b0: 0a20 2020 2042 656e 6761 6c69 3a20 3a63  .    Bengali: :c
+000007c0: 6c61 7373 3a60 7374 7260 0a20 2020 2020  lass:`str`.     
+000007d0: 2020 204c 616e 6775 6167 6520 636f 6465     Language code
+000007e0: 3a20 626e 0a20 2020 2042 756c 6761 7269  : bn.    Bulgari
+000007f0: 616e 3a20 3a63 6c61 7373 3a60 7374 7260  an: :class:`str`
+00000800: 0a20 2020 2020 2020 204c 616e 6775 6167  .        Languag
+00000810: 6520 636f 6465 3a20 6267 0a20 2020 2043  e code: bg.    C
+00000820: 6869 6e65 7365 5369 6d70 6c69 6669 6564  hineseSimplified
+00000830: 3a20 3a63 6c61 7373 3a60 7374 7260 0a20  : :class:`str`. 
+00000840: 2020 2020 2020 204c 616e 6775 6167 6520         Language 
+00000850: 636f 6465 3a20 7a68 0a20 2020 2043 6869  code: zh.    Chi
+00000860: 6e65 7365 5472 6164 6974 696f 6e61 6c3a  neseTraditional:
+00000870: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
+00000880: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
+00000890: 6f64 653a 207a 685f 7477 0a20 2020 2043  ode: zh_tw.    C
+000008a0: 7a65 6368 3a20 3a63 6c61 7373 3a60 7374  zech: :class:`st
+000008b0: 7260 0a20 2020 2020 2020 204c 616e 6775  r`.        Langu
+000008c0: 6167 6520 636f 6465 3a20 6373 0a20 2020  age code: cs.   
+000008d0: 2044 616e 6973 683a 203a 636c 6173 733a   Danish: :class:
+000008e0: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
+000008f0: 6e67 7561 6765 2063 6f64 653a 2064 610a  nguage code: da.
+00000900: 2020 2020 4475 7463 683a 203a 636c 6173      Dutch: :clas
+00000910: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
+00000920: 4c61 6e67 7561 6765 2063 6f64 653a 206e  Language code: n
+00000930: 6c0a 2020 2020 4669 6e6e 6973 683a 203a  l.    Finnish: :
+00000940: 636c 6173 733a 6073 7472 600a 2020 2020  class:`str`.    
+00000950: 2020 2020 4c61 6e67 7561 6765 2063 6f64      Language cod
+00000960: 653a 2066 690a 2020 2020 4672 656e 6368  e: fi.    French
+00000970: 3a20 3a63 6c61 7373 3a60 7374 7260 0a20  : :class:`str`. 
+00000980: 2020 2020 2020 204c 616e 6775 6167 6520         Language 
+00000990: 636f 6465 3a20 6672 0a20 2020 2047 6572  code: fr.    Ger
+000009a0: 6d61 6e3a 203a 636c 6173 733a 6073 7472  man: :class:`str
+000009b0: 600a 2020 2020 2020 2020 4c61 6e67 7561  `.        Langua
+000009c0: 6765 2063 6f64 653a 2064 650a 2020 2020  ge code: de.    
+000009d0: 4772 6565 6b3a 203a 636c 6173 733a 6073  Greek: :class:`s
+000009e0: 7472 600a 2020 2020 2020 2020 4c61 6e67  tr`.        Lang
+000009f0: 7561 6765 2063 6f64 653a 2065 6c0a 2020  uage code: el.  
+00000a00: 2020 4869 6e64 693a 203a 636c 6173 733a    Hindi: :class:
+00000a10: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
+00000a20: 6e67 7561 6765 2063 6f64 653a 2068 690a  nguage code: hi.
+00000a30: 2020 2020 4875 6e67 6172 6961 6e3a 203a      Hungarian: :
+00000a40: 636c 6173 733a 6073 7472 600a 2020 2020  class:`str`.    
+00000a50: 2020 2020 4c61 6e67 7561 6765 2063 6f64      Language cod
+00000a60: 653a 2068 750a 2020 2020 4974 616c 6961  e: hu.    Italia
+00000a70: 6e3a 203a 636c 6173 733a 6073 7472 600a  n: :class:`str`.
+00000a80: 2020 2020 2020 2020 4c61 6e67 7561 6765          Language
+00000a90: 2063 6f64 653a 2069 740a 2020 2020 4a61   code: it.    Ja
+00000aa0: 7061 6e65 7365 3a20 3a63 6c61 7373 3a60  panese: :class:`
+00000ab0: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
+00000ac0: 6775 6167 6520 636f 6465 3a20 6a61 0a20  guage code: ja. 
+00000ad0: 2020 204a 6176 616e 6573 653a 203a 636c     Javanese: :cl
+00000ae0: 6173 733a 6073 7472 600a 2020 2020 2020  ass:`str`.      
+00000af0: 2020 4c61 6e67 7561 6765 2063 6f64 653a    Language code:
+00000b00: 206a 760a 2020 2020 4b6f 7265 616e 3a20   jv.    Korean: 
+00000b10: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
+00000b20: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
+00000b30: 6465 3a20 6b6f 0a20 2020 204d 616e 6461  de: ko.    Manda
+00000b40: 7269 6e3a 203a 636c 6173 733a 6073 7472  rin: :class:`str
+00000b50: 600a 2020 2020 2020 2020 4c61 6e67 7561  `.        Langua
+00000b60: 6765 2063 6f64 653a 207a 685f 636d 6e0a  ge code: zh_cmn.
+00000b70: 2020 2020 4d61 7261 7468 693a 203a 636c      Marathi: :cl
+00000b80: 6173 733a 6073 7472 600a 2020 2020 2020  ass:`str`.      
+00000b90: 2020 4c61 6e67 7561 6765 2063 6f64 653a    Language code:
+00000ba0: 206d 720a 2020 2020 506f 6c69 7368 3a20   mr.    Polish: 
+00000bb0: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
+00000bc0: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
+00000bd0: 6465 3a20 706c 0a20 2020 2050 6f72 7475  de: pl.    Portu
+00000be0: 6775 6573 653a 203a 636c 6173 733a 6073  guese: :class:`s
+00000bf0: 7472 600a 2020 2020 2020 2020 4c61 6e67  tr`.        Lang
+00000c00: 7561 6765 2063 6f64 653a 2070 740a 2020  uage code: pt.  
+00000c10: 2020 5075 6e6a 6162 693a 203a 636c 6173    Punjabi: :clas
+00000c20: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
+00000c30: 4c61 6e67 7561 6765 2063 6f64 653a 2070  Language code: p
+00000c40: 610a 2020 2020 526f 6d61 6e69 616e 3a20  a.    Romanian: 
+00000c50: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
+00000c60: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
+00000c70: 6465 3a20 726f 0a20 2020 2052 7573 7369  de: ro.    Russi
+00000c80: 616e 3a20 3a63 6c61 7373 3a60 7374 7260  an: :class:`str`
+00000c90: 0a20 2020 2020 2020 204c 616e 6775 6167  .        Languag
+00000ca0: 6520 636f 6465 3a20 7275 0a20 2020 2053  e code: ru.    S
+00000cb0: 6572 6269 616e 3a20 3a63 6c61 7373 3a60  erbian: :class:`
+00000cc0: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
+00000cd0: 6775 6167 6520 636f 6465 3a20 7372 0a20  guage code: sr. 
+00000ce0: 2020 2053 696e 6861 6c65 7365 3a20 3a63     Sinhalese: :c
+00000cf0: 6c61 7373 3a60 7374 7260 0a20 2020 2020  lass:`str`.     
+00000d00: 2020 204c 616e 6775 6167 6520 636f 6465     Language code
+00000d10: 3a20 7369 0a20 2020 2053 6c6f 7661 6b3a  : si.    Slovak:
+00000d20: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
+00000d30: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
+00000d40: 6f64 653a 2073 6b0a 2020 2020 5370 616e  ode: sk.    Span
+00000d50: 6973 683a 203a 636c 6173 733a 6073 7472  ish: :class:`str
+00000d60: 600a 2020 2020 2020 2020 4c61 6e67 7561  `.        Langua
+00000d70: 6765 2063 6f64 653a 2065 730a 2020 2020  ge code: es.    
+00000d80: 5377 6564 6973 683a 203a 636c 6173 733a  Swedish: :class:
+00000d90: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
+00000da0: 6e67 7561 6765 2063 6f64 653a 2073 760a  nguage code: sv.
+00000db0: 2020 2020 5461 6d69 6c3a 203a 636c 6173      Tamil: :clas
+00000dc0: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
+00000dd0: 4c61 6e67 7561 6765 2063 6f64 653a 2074  Language code: t
+00000de0: 610a 2020 2020 5465 6c75 6775 3a20 3a63  a.    Telugu: :c
+00000df0: 6c61 7373 3a60 7374 7260 0a20 2020 2020  lass:`str`.     
+00000e00: 2020 204c 616e 6775 6167 6520 636f 6465     Language code
+00000e10: 3a20 7465 0a20 2020 2054 7572 6b69 7368  : te.    Turkish
+00000e20: 3a20 3a63 6c61 7373 3a60 7374 7260 0a20  : :class:`str`. 
+00000e30: 2020 2020 2020 204c 616e 6775 6167 6520         Language 
+00000e40: 636f 6465 3a20 7472 0a20 2020 2055 6b72  code: tr.    Ukr
+00000e50: 6169 6e69 616e 3a20 3a63 6c61 7373 3a60  ainian: :class:`
+00000e60: 7374 7260 0a20 2020 2020 2020 204c 616e  str`.        Lan
+00000e70: 6775 6167 6520 636f 6465 3a20 756b 0a20  guage code: uk. 
+00000e80: 2020 2055 7264 753a 203a 636c 6173 733a     Urdu: :class:
+00000e90: 6073 7472 600a 2020 2020 2020 2020 4c61  `str`.        La
+00000ea0: 6e67 7561 6765 2063 6f64 653a 2075 720a  nguage code: ur.
+00000eb0: 2020 2020 5669 6574 6e61 6d65 7365 3a20      Vietnamese: 
+00000ec0: 3a63 6c61 7373 3a60 7374 7260 0a20 2020  :class:`str`.   
+00000ed0: 2020 2020 204c 616e 6775 6167 6520 636f       Language co
+00000ee0: 6465 3a20 7669 0a20 2020 2057 7553 6861  de: vi.    WuSha
+00000ef0: 6e67 6861 696e 6573 653a 203a 636c 6173  nghainese: :clas
+00000f00: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
+00000f10: 4c61 6e67 7561 6765 2063 6f64 653a 207a  Language code: z
+00000f20: 685f 7775 750a 2020 2020 5869 616e 673a  h_wuu.    Xiang:
+00000f30: 203a 636c 6173 733a 6073 7472 600a 2020   :class:`str`.  
+00000f40: 2020 2020 2020 4c61 6e67 7561 6765 2063        Language c
+00000f50: 6f64 653a 207a 685f 6873 6e0a 2020 2020  ode: zh_hsn.    
+00000f60: 5975 6543 616e 746f 6e65 7365 3a20 3a63  YueCantonese: :c
+00000f70: 6c61 7373 3a60 7374 7260 0a20 2020 2020  lass:`str`.     
+00000f80: 2020 204c 616e 6775 6167 6520 636f 6465     Language code
+00000f90: 3a20 7a68 5f79 7565 0a20 2020 205a 756c  : zh_yue.    Zul
+00000fa0: 753a 203a 636c 6173 733a 6073 7472 600a  u: :class:`str`.
+00000fb0: 2020 2020 2020 2020 4c61 6e67 7561 6765          Language
+00000fc0: 2063 6f64 653a 207a 750a 2020 2020 da02   code: zu.    ..
+00000fd0: 6172 da06 4172 6162 6963 da02 626e da07  ar..Arabic..bn..
+00000fe0: 4265 6e67 616c 69da 0262 67da 0942 756c  Bengali..bg..Bul
+00000ff0: 6761 7269 616e da02 7a68 da11 4368 696e  garian..zh..Chin
+00001000: 6573 6553 696d 706c 6966 6965 64da 057a  eseSimplified..z
+00001010: 685f 7477 da12 4368 696e 6573 6554 7261  h_tw..ChineseTra
+00001020: 6469 7469 6f6e 616c da02 6373 da05 437a  ditional..cs..Cz
+00001030: 6563 68da 0264 61da 0644 616e 6973 68da  ech..da..Danish.
+00001040: 026e 6cda 0544 7574 6368 da02 6669 da07  .nl..Dutch..fi..
+00001050: 4669 6e6e 6973 68da 0266 72da 0646 7265  Finnish..fr..Fre
+00001060: 6e63 68da 0264 65da 0647 6572 6d61 6eda  nch..de..German.
+00001070: 0265 6cda 0547 7265 656b da02 6869 da05  .el..Greek..hi..
+00001080: 4869 6e64 69da 0268 75da 0948 756e 6761  Hindi..hu..Hunga
+00001090: 7269 616e da02 6974 da07 4974 616c 6961  rian..it..Italia
+000010a0: 6eda 026a 61da 084a 6170 616e 6573 65da  n..ja..Japanese.
+000010b0: 026a 76da 084a 6176 616e 6573 65da 026b  .jv..Javanese..k
+000010c0: 6fda 064b 6f72 6561 6eda 067a 685f 636d  o..Korean..zh_cm
+000010d0: 6eda 084d 616e 6461 7269 6eda 026d 72da  n..Mandarin..mr.
+000010e0: 074d 6172 6174 6869 da02 706c da06 506f  .Marathi..pl..Po
+000010f0: 6c69 7368 da02 7074 da0a 506f 7274 7567  lish..pt..Portug
+00001100: 7565 7365 da02 7061 da07 5075 6e6a 6162  uese..pa..Punjab
+00001110: 69da 0272 6fda 0852 6f6d 616e 6961 6eda  i..ro..Romanian.
+00001120: 0272 75da 0752 7573 7369 616e da02 7372  .ru..Russian..sr
+00001130: da07 5365 7262 6961 6eda 0273 69da 0953  ..Serbian..si..S
+00001140: 696e 6861 6c65 7365 da02 736b da06 536c  inhalese..sk..Sl
+00001150: 6f76 616b da02 6573 da07 5370 616e 6973  ovak..es..Spanis
+00001160: 68da 0273 76da 0753 7765 6469 7368 da02  h..sv..Swedish..
+00001170: 7461 da05 5461 6d69 6cda 0274 65da 0654  ta..Tamil..te..T
+00001180: 656c 7567 75da 0274 72da 0754 7572 6b69  elugu..tr..Turki
+00001190: 7368 da02 756b da09 556b 7261 696e 6961  sh..uk..Ukrainia
+000011a0: 6eda 0275 72da 0455 7264 75da 0276 69da  n..ur..Urdu..vi.
+000011b0: 0a56 6965 746e 616d 6573 65da 067a 685f  .Vietnamese..zh_
+000011c0: 7775 75da 0e57 7553 6861 6e67 6861 696e  wuu..WuShanghain
+000011d0: 6573 65da 067a 685f 6873 6eda 0558 6961  ese..zh_hsn..Xia
+000011e0: 6e67 da06 7a68 5f79 7565 da0c 5975 6543  ng..zh_yue..YueC
+000011f0: 616e 746f 6e65 7365 da02 7a75 da04 5a75  antonese..zu..Zu
+00001200: 6c75 4e29 2eda 085f 5f6e 616d 655f 5fda  luN)...__name__.
+00001210: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00001220: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00001230: 5f5f 7205 0000 00da 0373 7472 da0f 5f5f  __r......str..__
+00001240: 616e 6e6f 7461 7469 6f6e 735f 5f72 0700  annotations__r..
+00001250: 0000 7209 0000 0072 0b00 0000 720d 0000  ..r....r....r...
+00001260: 0072 0f00 0000 7211 0000 0072 1300 0000  .r....r....r....
+00001270: 7215 0000 0072 1700 0000 7219 0000 0072  r....r....r....r
+00001280: 1b00 0000 721d 0000 0072 1f00 0000 7221  ....r....r....r!
+00001290: 0000 0072 2300 0000 7225 0000 0072 2700  ...r#...r%...r'.
+000012a0: 0000 7229 0000 0072 2b00 0000 722d 0000  ..r)...r+...r-..
+000012b0: 0072 2f00 0000 7231 0000 0072 3300 0000  .r/...r1...r3...
+000012c0: 7235 0000 0072 3700 0000 7239 0000 0072  r5...r7...r9...r
+000012d0: 3b00 0000 723d 0000 0072 3f00 0000 7241  ;...r=...r?...rA
+000012e0: 0000 0072 4300 0000 7245 0000 0072 4700  ...rC...rE...rG.
+000012f0: 0000 7249 0000 0072 4b00 0000 724d 0000  ..rI...rK...rM..
+00001300: 0072 4f00 0000 7251 0000 0072 5300 0000  .rO...rQ...rS...
+00001310: a900 725a 0000 0072 5a00 0000 fa2f 6275  ..rZ...rZ..../bu
+00001320: 696c 642f 6264 6973 742e 6c69 6e75 782d  ild/bdist.linux-
+00001330: 7838 365f 3634 2f65 6767 2f77 6561 7468  x86_64/egg/weath
+00001340: 6572 6c79 2f65 6e75 6d73 2e70 7972 0300  erly/enums.pyr..
+00001350: 0000 1f00 0000 7354 0000 000a 0004 010c  ......sT........
+00001360: 580c 010c 010c 010c 010c 010c 010c 010c  X...............
+00001370: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001380: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00001390: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+000013a0: 010c 010c 010c 010c 010c 010c 0110 0172  ...............r
+000013b0: 0300 0000 4e29 0572 5700 0000 da04 656e  ....N).rW.....en
+000013c0: 756d 7202 0000 00da 075f 5f61 6c6c 5f5f  umr......__all__
+000013d0: 7203 0000 0072 5a00 0000 725a 0000 0072  r....rZ...rZ...r
+000013e0: 5a00 0000 725b 0000 00da 083c 6d6f 6475  Z...r[.....<modu
+000013f0: 6c65 3e01 0000 0073 0800 0000 0400 0c18  le>....s........
+00001400: 0402 1404                                ....
```

## Comparing `weatherly/api/__pycache__/__init__.cpython-311.pyc` & `weatherly/api/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Mon Apr 17 07:10:18 2023 UTC, .py size: 1258 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,87 @@
-00000000: a70d 0d0a 0000 0000 daf0 3c64 ea04 0000  ..........<d....
-00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
-00000020: 0000 0000 00f3 1200 0000 9700 6400 5a00  ............d.Z.
-00000030: 6401 6402 6c01 5400 6403 5300 2904 61ae  d.d.l.T.d.S.).a.
-00000040: 0400 000a 7765 6174 6865 726c 792f 6170  ....weatherly/ap
-00000050: 690a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  i.--------------
-00000060: 0a41 6e20 7061 636b 6167 6520 6578 7465  .An package exte
-00000070: 6e73 696f 6e20 746f 2077 6561 7468 6572  nsion to weather
-00000080: 6c79 2070 726f 7669 6469 6e67 2061 6363  ly providing acc
-00000090: 6573 7320 746f 2057 6561 7468 6572 4150  ess to WeatherAP
-000000a0: 4920 2872 6571 7565 7374 732c 2063 6c69  I (requests, cli
-000000b0: 656e 742c 2065 7463 2e29 0a0a 0a4d 4954  ent, etc.)...MIT
-000000c0: 204c 6963 656e 7365 0a0a 436f 7079 7269   License..Copyri
-000000d0: 6768 7420 2863 2920 3230 3233 204b 6f6e  ght (c) 2023 Kon
-000000e0: 7261 6420 2840 6b6f 6e72 6164 7369 6329  rad (@konradsic)
-000000f0: 0a0a 5065 726d 6973 7369 6f6e 2069 7320  ..Permission is 
-00000100: 6865 7265 6279 2067 7261 6e74 6564 2c20  hereby granted, 
-00000110: 6672 6565 206f 6620 6368 6172 6765 2c20  free of charge, 
-00000120: 746f 2061 6e79 2070 6572 736f 6e20 6f62  to any person ob
-00000130: 7461 696e 696e 6720 6120 636f 7079 0a6f  taining a copy.o
-00000140: 6620 7468 6973 2073 6f66 7477 6172 6520  f this software 
-00000150: 616e 6420 6173 736f 6369 6174 6564 2064  and associated d
-00000160: 6f63 756d 656e 7461 7469 6f6e 2066 696c  ocumentation fil
-00000170: 6573 2028 7468 6520 2253 6f66 7477 6172  es (the "Softwar
-00000180: 6522 292c 2074 6f20 6465 616c 0a69 6e20  e"), to deal.in 
-00000190: 7468 6520 536f 6674 7761 7265 2077 6974  the Software wit
-000001a0: 686f 7574 2072 6573 7472 6963 7469 6f6e  hout restriction
-000001b0: 2c20 696e 636c 7564 696e 6720 7769 7468  , including with
-000001c0: 6f75 7420 6c69 6d69 7461 7469 6f6e 2074  out limitation t
-000001d0: 6865 2072 6967 6874 730a 746f 2075 7365  he rights.to use
-000001e0: 2c20 636f 7079 2c20 6d6f 6469 6679 2c20  , copy, modify, 
-000001f0: 6d65 7267 652c 2070 7562 6c69 7368 2c20  merge, publish, 
-00000200: 6469 7374 7269 6275 7465 2c20 7375 626c  distribute, subl
-00000210: 6963 656e 7365 2c20 616e 642f 6f72 2073  icense, and/or s
-00000220: 656c 6c0a 636f 7069 6573 206f 6620 7468  ell.copies of th
-00000230: 6520 536f 6674 7761 7265 2c20 616e 6420  e Software, and 
-00000240: 746f 2070 6572 6d69 7420 7065 7273 6f6e  to permit person
-00000250: 7320 746f 2077 686f 6d20 7468 6520 536f  s to whom the So
-00000260: 6674 7761 7265 2069 730a 6675 726e 6973  ftware is.furnis
-00000270: 6865 6420 746f 2064 6f20 736f 2c20 7375  hed to do so, su
-00000280: 626a 6563 7420 746f 2074 6865 2066 6f6c  bject to the fol
-00000290: 6c6f 7769 6e67 2063 6f6e 6469 7469 6f6e  lowing condition
-000002a0: 733a 0a0a 5468 6520 6162 6f76 6520 636f  s:..The above co
-000002b0: 7079 7269 6768 7420 6e6f 7469 6365 2061  pyright notice a
-000002c0: 6e64 2074 6869 7320 7065 726d 6973 7369  nd this permissi
-000002d0: 6f6e 206e 6f74 6963 6520 7368 616c 6c20  on notice shall 
-000002e0: 6265 2069 6e63 6c75 6465 6420 696e 2061  be included in a
-000002f0: 6c6c 0a63 6f70 6965 7320 6f72 2073 7562  ll.copies or sub
-00000300: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
-00000310: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
-00000320: 652e 0a0a 5448 4520 534f 4654 5741 5245  e...THE SOFTWARE
-00000330: 2049 5320 5052 4f56 4944 4544 2022 4153   IS PROVIDED "AS
-00000340: 2049 5322 2c20 5749 5448 4f55 5420 5741   IS", WITHOUT WA
-00000350: 5252 414e 5459 204f 4620 414e 5920 4b49  RRANTY OF ANY KI
-00000360: 4e44 2c20 4558 5052 4553 5320 4f52 0a49  ND, EXPRESS OR.I
-00000370: 4d50 4c49 4544 2c20 494e 434c 5544 494e  MPLIED, INCLUDIN
-00000380: 4720 4255 5420 4e4f 5420 4c49 4d49 5445  G BUT NOT LIMITE
-00000390: 4420 544f 2054 4845 2057 4152 5241 4e54  D TO THE WARRANT
-000003a0: 4945 5320 4f46 204d 4552 4348 414e 5441  IES OF MERCHANTA
-000003b0: 4249 4c49 5459 2c0a 4649 544e 4553 5320  BILITY,.FITNESS 
-000003c0: 464f 5220 4120 5041 5254 4943 554c 4152  FOR A PARTICULAR
-000003d0: 2050 5552 504f 5345 2041 4e44 204e 4f4e   PURPOSE AND NON
-000003e0: 494e 4652 494e 4745 4d45 4e54 2e20 494e  INFRINGEMENT. IN
-000003f0: 204e 4f20 4556 454e 5420 5348 414c 4c20   NO EVENT SHALL 
-00000400: 5448 450a 4155 5448 4f52 5320 4f52 2043  THE.AUTHORS OR C
-00000410: 4f50 5952 4947 4854 2048 4f4c 4445 5253  OPYRIGHT HOLDERS
-00000420: 2042 4520 4c49 4142 4c45 2046 4f52 2041   BE LIABLE FOR A
-00000430: 4e59 2043 4c41 494d 2c20 4441 4d41 4745  NY CLAIM, DAMAGE
-00000440: 5320 4f52 204f 5448 4552 0a4c 4941 4249  S OR OTHER.LIABI
-00000450: 4c49 5459 2c20 5748 4554 4845 5220 494e  LITY, WHETHER IN
-00000460: 2041 4e20 4143 5449 4f4e 204f 4620 434f   AN ACTION OF CO
-00000470: 4e54 5241 4354 2c20 544f 5254 204f 5220  NTRACT, TORT OR 
-00000480: 4f54 4845 5257 4953 452c 2041 5249 5349  OTHERWISE, ARISI
-00000490: 4e47 2046 524f 4d2c 0a4f 5554 204f 4620  NG FROM,.OUT OF 
-000004a0: 4f52 2049 4e20 434f 4e4e 4543 5449 4f4e  OR IN CONNECTION
-000004b0: 2057 4954 4820 5448 4520 534f 4654 5741   WITH THE SOFTWA
-000004c0: 5245 204f 5220 5448 4520 5553 4520 4f52  RE OR THE USE OR
-000004d0: 204f 5448 4552 2044 4541 4c49 4e47 5320   OTHER DEALINGS 
-000004e0: 494e 2054 4845 0a53 4f46 5457 4152 452e  IN THE.SOFTWARE.
-000004f0: 0ae9 0100 0000 2901 da01 2a4e 2902 da07  ......)...*N)...
-00000500: 5f5f 646f 635f 5fda 0663 6c69 656e 74a9  __doc__..client.
-00000510: 00f3 0000 0000 fa33 6275 696c 645c 6264  .......3build\bd
-00000520: 6973 742e 7769 6e2d 616d 6436 345c 6567  ist.win-amd64\eg
-00000530: 675c 7765 6174 6865 726c 795c 6170 695c  g\weatherly\api\
-00000540: 5f5f 696e 6974 5f5f 2e70 79fa 083c 6d6f  __init__.py..<mo
-00000550: 6475 6c65 3e72 0900 0000 0100 0000 7323  dule>r........s#
-00000560: 0000 00f0 0301 0101 f002 1b01 04f0 001b  ................
-00000570: 0104 f03a 0001 16d0 0015 d000 15d0 0015  ...:............
-00000580: d000 15d0 0015 7207 0000 00              ......r....
+00000000: 6f0d 0d0a 0000 0000 7a49 3c64 cc04 0000  o.......zI<d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0002 0000 0040 0000 0073 1000 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5400 6403 5300 2904  Z.d.d.l.T.d.S.).
+00000040: 61ae 0400 000a 7765 6174 6865 726c 792f  a.....weatherly/
+00000050: 6170 690a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  api.------------
+00000060: 2d2d 0a41 6e20 7061 636b 6167 6520 6578  --.An package ex
+00000070: 7465 6e73 696f 6e20 746f 2077 6561 7468  tension to weath
+00000080: 6572 6c79 2070 726f 7669 6469 6e67 2061  erly providing a
+00000090: 6363 6573 7320 746f 2057 6561 7468 6572  ccess to Weather
+000000a0: 4150 4920 2872 6571 7565 7374 732c 2063  API (requests, c
+000000b0: 6c69 656e 742c 2065 7463 2e29 0a0a 0a4d  lient, etc.)...M
+000000c0: 4954 204c 6963 656e 7365 0a0a 436f 7079  IT License..Copy
+000000d0: 7269 6768 7420 2863 2920 3230 3233 204b  right (c) 2023 K
+000000e0: 6f6e 7261 6420 2840 6b6f 6e72 6164 7369  onrad (@konradsi
+000000f0: 6329 0a0a 5065 726d 6973 7369 6f6e 2069  c)..Permission i
+00000100: 7320 6865 7265 6279 2067 7261 6e74 6564  s hereby granted
+00000110: 2c20 6672 6565 206f 6620 6368 6172 6765  , free of charge
+00000120: 2c20 746f 2061 6e79 2070 6572 736f 6e20  , to any person 
+00000130: 6f62 7461 696e 696e 6720 6120 636f 7079  obtaining a copy
+00000140: 0a6f 6620 7468 6973 2073 6f66 7477 6172  .of this softwar
+00000150: 6520 616e 6420 6173 736f 6369 6174 6564  e and associated
+00000160: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
+00000170: 696c 6573 2028 7468 6520 2253 6f66 7477  iles (the "Softw
+00000180: 6172 6522 292c 2074 6f20 6465 616c 0a69  are"), to deal.i
+00000190: 6e20 7468 6520 536f 6674 7761 7265 2077  n the Software w
+000001a0: 6974 686f 7574 2072 6573 7472 6963 7469  ithout restricti
+000001b0: 6f6e 2c20 696e 636c 7564 696e 6720 7769  on, including wi
+000001c0: 7468 6f75 7420 6c69 6d69 7461 7469 6f6e  thout limitation
+000001d0: 2074 6865 2072 6967 6874 730a 746f 2075   the rights.to u
+000001e0: 7365 2c20 636f 7079 2c20 6d6f 6469 6679  se, copy, modify
+000001f0: 2c20 6d65 7267 652c 2070 7562 6c69 7368  , merge, publish
+00000200: 2c20 6469 7374 7269 6275 7465 2c20 7375  , distribute, su
+00000210: 626c 6963 656e 7365 2c20 616e 642f 6f72  blicense, and/or
+00000220: 2073 656c 6c0a 636f 7069 6573 206f 6620   sell.copies of 
+00000230: 7468 6520 536f 6674 7761 7265 2c20 616e  the Software, an
+00000240: 6420 746f 2070 6572 6d69 7420 7065 7273  d to permit pers
+00000250: 6f6e 7320 746f 2077 686f 6d20 7468 6520  ons to whom the 
+00000260: 536f 6674 7761 7265 2069 730a 6675 726e  Software is.furn
+00000270: 6973 6865 6420 746f 2064 6f20 736f 2c20  ished to do so, 
+00000280: 7375 626a 6563 7420 746f 2074 6865 2066  subject to the f
+00000290: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
+000002a0: 6f6e 733a 0a0a 5468 6520 6162 6f76 6520  ons:..The above 
+000002b0: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
+000002c0: 2061 6e64 2074 6869 7320 7065 726d 6973   and this permis
+000002d0: 7369 6f6e 206e 6f74 6963 6520 7368 616c  sion notice shal
+000002e0: 6c20 6265 2069 6e63 6c75 6465 6420 696e  l be included in
+000002f0: 2061 6c6c 0a63 6f70 6965 7320 6f72 2073   all.copies or s
+00000300: 7562 7374 616e 7469 616c 2070 6f72 7469  ubstantial porti
+00000310: 6f6e 7320 6f66 2074 6865 2053 6f66 7477  ons of the Softw
+00000320: 6172 652e 0a0a 5448 4520 534f 4654 5741  are...THE SOFTWA
+00000330: 5245 2049 5320 5052 4f56 4944 4544 2022  RE IS PROVIDED "
+00000340: 4153 2049 5322 2c20 5749 5448 4f55 5420  AS IS", WITHOUT 
+00000350: 5741 5252 414e 5459 204f 4620 414e 5920  WARRANTY OF ANY 
+00000360: 4b49 4e44 2c20 4558 5052 4553 5320 4f52  KIND, EXPRESS OR
+00000370: 0a49 4d50 4c49 4544 2c20 494e 434c 5544  .IMPLIED, INCLUD
+00000380: 494e 4720 4255 5420 4e4f 5420 4c49 4d49  ING BUT NOT LIMI
+00000390: 5445 4420 544f 2054 4845 2057 4152 5241  TED TO THE WARRA
+000003a0: 4e54 4945 5320 4f46 204d 4552 4348 414e  NTIES OF MERCHAN
+000003b0: 5441 4249 4c49 5459 2c0a 4649 544e 4553  TABILITY,.FITNES
+000003c0: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
+000003d0: 4152 2050 5552 504f 5345 2041 4e44 204e  AR PURPOSE AND N
+000003e0: 4f4e 494e 4652 494e 4745 4d45 4e54 2e20  ONINFRINGEMENT. 
+000003f0: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
+00000400: 4c20 5448 450a 4155 5448 4f52 5320 4f52  L THE.AUTHORS OR
+00000410: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
+00000420: 5253 2042 4520 4c49 4142 4c45 2046 4f52  RS BE LIABLE FOR
+00000430: 2041 4e59 2043 4c41 494d 2c20 4441 4d41   ANY CLAIM, DAMA
+00000440: 4745 5320 4f52 204f 5448 4552 0a4c 4941  GES OR OTHER.LIA
+00000450: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
+00000460: 494e 2041 4e20 4143 5449 4f4e 204f 4620  IN AN ACTION OF 
+00000470: 434f 4e54 5241 4354 2c20 544f 5254 204f  CONTRACT, TORT O
+00000480: 5220 4f54 4845 5257 4953 452c 2041 5249  R OTHERWISE, ARI
+00000490: 5349 4e47 2046 524f 4d2c 0a4f 5554 204f  SING FROM,.OUT O
+000004a0: 4620 4f52 2049 4e20 434f 4e4e 4543 5449  F OR IN CONNECTI
+000004b0: 4f4e 2057 4954 4820 5448 4520 534f 4654  ON WITH THE SOFT
+000004c0: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
+000004d0: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
+000004e0: 5320 494e 2054 4845 0a53 4f46 5457 4152  S IN THE.SOFTWAR
+000004f0: 452e 0ae9 0100 0000 2901 da01 2a4e 2902  E.......)...*N).
+00000500: da07 5f5f 646f 635f 5fda 0663 6c69 656e  ..__doc__..clien
+00000510: 74a9 0072 0500 0000 7205 0000 00fa 3662  t..r....r.....6b
+00000520: 7569 6c64 2f62 6469 7374 2e6c 696e 7578  uild/bdist.linux
+00000530: 2d78 3836 5f36 342f 6567 672f 7765 6174  -x86_64/egg/weat
+00000540: 6865 726c 792f 6170 692f 5f5f 696e 6974  herly/api/__init
+00000550: 5f5f 2e70 79da 083c 6d6f 6475 6c65 3e01  __.py..<module>.
+00000560: 0000 0073 0400 0000 0400 0c1d            ...s........
```

## Comparing `weatherly/api/__pycache__/client.cpython-311.pyc` & `weatherly/api/__pycache__/client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Fri Apr 21 06:45:42 2023 UTC, .py size: 9793 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,745 +1,767 @@
-00000000: a70d 0d0a 0000 0000 1631 4264 4126 0000  .........1BdA&..
-00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 a600 0000 9700 6400 5a00  ............d.Z.
-00000030: 6401 6402 6c01 6d02 5a02 0100 6403 6404  d.d.l.m.Z...d.d.
-00000040: 6c03 6d04 5a04 0100 6403 6405 6c05 6d06  l.m.Z...d.d.l.m.
-00000050: 5a06 6d07 5a07 0100 6403 6406 6c08 6d09  Z.m.Z...d.d.l.m.
-00000060: 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d  Z.m.Z.m.Z.m.Z.m.
-00000070: 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6403 6407  Z.m.Z.m.Z...d.d.
-00000080: 6c10 6d11 5a11 0100 6408 6409 6c12 6d13  l.m.Z...d.d.l.m.
-00000090: 5a13 6d14 5a14 6d15 5a15 6d16 5a16 6d17  Z.m.Z.m.Z.m.Z.m.
-000000a0: 5a17 6d18 5a18 0100 640a 5a19 640b 5a1a  Z.m.Z...d.Z.d.Z.
-000000b0: 0200 4700 640c 8400 640d 6502 a603 0000  ..G.d...d.e.....
-000000c0: ab03 0000 0000 0000 0000 5a1b 640e 5300  ..........Z.d.S.
-000000d0: 290f 6135 0400 000a 4d49 5420 4c69 6365  ).a5....MIT Lice
-000000e0: 6e73 650a 0a43 6f70 7972 6967 6874 2028  nse..Copyright (
-000000f0: 6329 2032 3032 3320 4b6f 6e72 6164 2028  c) 2023 Konrad (
-00000100: 406b 6f6e 7261 6473 6963 290a 0a50 6572  @konradsic)..Per
-00000110: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
-00000120: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
-00000130: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
-00000140: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
-00000150: 6e67 2061 2063 6f70 790a 6f66 2074 6869  ng a copy.of thi
-00000160: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
-00000170: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
-00000180: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
-00000190: 6865 2022 536f 6674 7761 7265 2229 2c20  he "Software"), 
-000001a0: 746f 2064 6561 6c0a 696e 2074 6865 2053  to deal.in the S
-000001b0: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
-000001c0: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
-000001d0: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
-000001e0: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
-000001f0: 6768 7473 0a74 6f20 7573 652c 2063 6f70  ghts.to use, cop
-00000200: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
-00000210: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
-00000220: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
-00000230: 652c 2061 6e64 2f6f 7220 7365 6c6c 0a63  e, and/or sell.c
-00000240: 6f70 6965 7320 6f66 2074 6865 2053 6f66  opies of the Sof
-00000250: 7477 6172 652c 2061 6e64 2074 6f20 7065  tware, and to pe
-00000260: 726d 6974 2070 6572 736f 6e73 2074 6f20  rmit persons to 
-00000270: 7768 6f6d 2074 6865 2053 6f66 7477 6172  whom the Softwar
-00000280: 6520 6973 0a66 7572 6e69 7368 6564 2074  e is.furnished t
-00000290: 6f20 646f 2073 6f2c 2073 7562 6a65 6374  o do so, subject
-000002a0: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
-000002b0: 6720 636f 6e64 6974 696f 6e73 3a0a 0a54  g conditions:..T
-000002c0: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
-000002d0: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
-000002e0: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
-000002f0: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
-00000300: 636c 7564 6564 2069 6e20 616c 6c0a 636f  cluded in all.co
-00000310: 7069 6573 206f 7220 7375 6273 7461 6e74  pies or substant
-00000320: 6961 6c20 706f 7274 696f 6e73 206f 6620  ial portions of 
-00000330: 7468 6520 536f 6674 7761 7265 2e0a 0a54  the Software...T
-00000340: 4845 2053 4f46 5457 4152 4520 4953 2050  HE SOFTWARE IS P
-00000350: 524f 5649 4445 4420 2241 5320 4953 222c  ROVIDED "AS IS",
-00000360: 2057 4954 484f 5554 2057 4152 5241 4e54   WITHOUT WARRANT
-00000370: 5920 4f46 2041 4e59 204b 494e 442c 2045  Y OF ANY KIND, E
-00000380: 5850 5245 5353 204f 520a 494d 504c 4945  XPRESS OR.IMPLIE
-00000390: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
-000003a0: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
-000003b0: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
-000003c0: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-000003d0: 592c 0a46 4954 4e45 5353 2046 4f52 2041  Y,.FITNESS FOR A
-000003e0: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
-000003f0: 4f53 4520 414e 4420 4e4f 4e49 4e46 5249  OSE AND NONINFRI
-00000400: 4e47 454d 454e 542e 2049 4e20 4e4f 2045  NGEMENT. IN NO E
-00000410: 5645 4e54 2053 4841 4c4c 2054 4845 0a41  VENT SHALL THE.A
-00000420: 5554 484f 5253 204f 5220 434f 5059 5249  UTHORS OR COPYRI
-00000430: 4748 5420 484f 4c44 4552 5320 4245 204c  GHT HOLDERS BE L
-00000440: 4941 424c 4520 464f 5220 414e 5920 434c  IABLE FOR ANY CL
-00000450: 4149 4d2c 2044 414d 4147 4553 204f 5220  AIM, DAMAGES OR 
-00000460: 4f54 4845 520a 4c49 4142 494c 4954 592c  OTHER.LIABILITY,
-00000470: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
-00000480: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
-00000490: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
-000004a0: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
-000004b0: 4f4d 2c0a 4f55 5420 4f46 204f 5220 494e  OM,.OUT OF OR IN
-000004c0: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
-000004d0: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
-000004e0: 2054 4845 2055 5345 204f 5220 4f54 4845   THE USE OR OTHE
-000004f0: 5220 4445 414c 494e 4753 2049 4e20 5448  R DEALINGS IN TH
-00000500: 450a 534f 4654 5741 5245 2e0a e901 0000  E.SOFTWARE......
-00000510: 0029 01da 0d42 6173 6541 5049 436c 6965  .)...BaseAPIClie
-00000520: 6e74 e902 0000 0029 01da 094c 616e 6775  nt.....)...Langu
-00000530: 6167 6573 2902 da12 4375 7272 656e 7457  ages)...CurrentW
-00000540: 6561 7468 6572 4461 7461 da0c 4c6f 6361  eatherData..Loca
-00000550: 7469 6f6e 4461 7461 2907 da13 5765 6174  tionData)...Weat
-00000560: 6865 7241 5049 4578 6365 7074 696f 6eda  herAPIException.
-00000570: 0f4e 6f4c 6f63 6174 696f 6e46 6f75 6e64  .NoLocationFound
-00000580: da0d 496e 7661 6c69 6441 5049 4b65 79da  ..InvalidAPIKey.
-00000590: 1041 5049 4c69 6d69 7445 7863 6565 6465  .APILimitExceede
-000005a0: 64da 0e41 5049 4b65 7944 6973 6162 6c65  d..APIKeyDisable
-000005b0: 64da 0c41 6363 6573 7344 656e 6965 64da  d..AccessDenied.
-000005c0: 1849 6e74 6572 6e61 6c41 7070 6c69 6361  .InternalApplica
-000005d0: 7469 6f6e 4572 726f 7229 01da 0575 7469  tionError)...uti
-000005e0: 6c73 e900 0000 0029 06da 0341 6e79 da07  ls.....)...Any..
-000005f0: 4c69 7465 7261 6cda 0444 6963 74da 084f  Literal..Dict..O
-00000600: 7074 696f 6e61 6cda 0555 6e69 6f6e da04  ptional..Union..
-00000610: 4c69 7374 7a1d 6874 7470 3a2f 2f61 7069  Listz.http://api
-00000620: 2e77 6561 7468 6572 6170 692e 636f 6d2f  .weatherapi.com/
-00000630: 7631 2f29 01da 1057 6561 7468 6572 4150  v1/)...WeatherAP
-00000640: 4943 6c69 656e 7463 0000 0000 0000 0000  IClientc........
-00000650: 0000 0000 1300 0000 0000 0000 f394 0100  ................
-00000660: 0087 0097 0065 005a 0164 005a 0264 015a  .....e.Z.d.Z.d.Z
-00000670: 0309 0009 0009 0009 0009 0009 0064 1964  .............d.d
-00000680: 0465 0464 0565 0565 0665 0465 0766 0219  .e.d.e.e.e.e.f..
-00000690: 0000 0000 0000 0000 0019 0000 0000 0000  ................
-000006a0: 0000 0064 0665 0565 0819 0000 0000 0000  ...d.e.e........
-000006b0: 0000 0064 0765 0565 0819 0000 0000 0000  ...d.e.e........
-000006c0: 0000 0064 0865 0565 0819 0000 0000 0000  ...d.e.e........
-000006d0: 0000 0064 0965 0964 0a19 0000 0000 0000  ...d.e.d........
-000006e0: 0000 0064 0b65 0964 0a19 0000 0000 0000  ...d.e.d........
-000006f0: 0000 0064 0c65 0a65 0465 0b66 0219 0000  ...d.e.e.e.f....
-00000700: 0000 0000 0000 0064 0d64 0266 1288 0066  .......d.d.f...f
-00000710: 0164 0e84 0d5a 0c64 0f65 0464 1065 0a65  .d...Z.d.e.d.e.e
-00000720: 0465 0b66 0219 0000 0000 0000 0000 0064  .e.f...........d
-00000730: 0d65 0a65 0465 0b66 0219 0000 0000 0000  .e.e.e.f........
-00000740: 0000 0066 0664 1184 045a 0d64 0565 0665  ...f.d...Z.d.e.e
-00000750: 0465 0766 0219 0000 0000 0000 0000 0064  .e.f...........d
-00000760: 0d65 0665 0764 0266 0219 0000 0000 0000  .e.e.d.f........
-00000770: 0000 0066 0464 1284 045a 0e09 0009 0064  ...f.d...Z.....d
-00000780: 1a64 1365 0464 0565 0565 0665 0465 0766  .d.e.d.e.e.e.e.f
-00000790: 0219 0000 0000 0000 0000 0019 0000 0000  ................
-000007a0: 0000 0000 0064 0965 0964 1419 0000 0000  .....d.e.d......
-000007b0: 0000 0000 0064 0c65 0a65 0465 0b66 0219  .....d.e.e.e.f..
-000007c0: 0000 0000 0000 0000 0064 0d65 0f66 0a64  .........d.e.f.d
-000007d0: 1584 055a 1064 1365 0466 0264 1684 045a  ...Z.d.e.f.d...Z
-000007e0: 1164 1784 005a 1264 1884 005a 1388 0078  .d...Z.d...Z...x
-000007f0: 015a 1453 0029 1b72 1700 0000 61d3 0400  .Z.S.).r....a...
-00000800: 000a 2020 2020 4120 5765 6174 6865 7241  ..    A WeatherA
-00000810: 5049 2e63 6f6d 2063 6c69 656e 7420 666f  PI.com client fo
-00000820: 7220 6665 7463 6869 6e67 2076 6172 696f  r fetching vario
-00000830: 7573 2077 6561 7468 6572 2069 6e66 6f72  us weather infor
-00000840: 6d61 7469 6f6e 0a0a 2020 2020 5061 7261  mation..    Para
-00000850: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00000860: 2d2d 2d2d 2d0a 2020 2020 6170 695f 6b65  -----.    api_ke
-00000870: 793a 203a 636c 6173 733a 6073 7472 600a  y: :class:`str`.
-00000880: 2020 2020 2020 2020 4150 4920 4b65 7920          API Key 
-00000890: 7573 6564 2074 6f20 6175 7468 656e 7469  used to authenti
-000008a0: 6361 7465 2077 6865 6e20 7365 6e64 696e  cate when sendin
-000008b0: 6720 7265 7175 6573 7473 0a20 2020 206c  g requests.    l
-000008c0: 616e 673a 204f 7074 696f 6e61 6c5b 2055  ang: Optional[ U
-000008d0: 6e69 6f6e 5b3a 636c 6173 733a 6073 7472  nion[:class:`str
-000008e0: 602c 203a 636c 6173 733a 604c 616e 6775  `, :class:`Langu
-000008f0: 6167 6573 605d 205d 0a20 2020 2020 2020  ages`] ].       
-00000900: 204c 616e 6775 6167 6520 6672 6f6d 2074   Language from t
-00000910: 6865 203a 636c 6173 733a 604c 616e 6775  he :class:`Langu
-00000920: 6167 6573 6020 656e 756d 206f 7220 6120  ages` enum or a 
-00000930: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-00000940: 696e 6720 7468 6520 6c61 6e67 7561 6765  ing the language
-00000950: 206f 7220 6c61 6e67 7561 6765 2063 6f64   or language cod
-00000960: 6520 2870 7265 6665 7261 626c 7929 2e0a  e (preferably)..
-00000970: 2020 2020 2020 2020 546f 2067 6574 2061          To get a
-00000980: 206c 6973 7420 6f66 206c 616e 6775 6167   list of languag
-00000990: 6573 2076 6973 6974 203a 636c 6173 733a  es visit :class:
-000009a0: 604c 616e 6775 6167 6573 602e 2049 6620  `Languages`. If 
-000009b0: 6060 4e6f 6e65 6060 2074 6865 6e20 7468  ``None`` then th
-000009c0: 6520 6465 6661 756c 7420 6c61 6e67 7561  e default langua
-000009d0: 6765 2069 7320 7573 6564 2028 456e 676c  ge is used (Engl
-000009e0: 6973 6829 0a20 2020 2064 743a 204f 7074  ish).    dt: Opt
-000009f0: 696f 6e61 6c5b 3a63 6c61 7373 3a60 696e  ional[:class:`in
-00000a00: 7460 5d0a 2020 2020 2020 2020 5265 7374  t`].        Rest
-00000a10: 7269 6374 2064 6174 6520 6f75 7470 7574  rict date output
-00000a20: 2066 6f72 2046 6f72 6563 6173 7420 616e   for Forecast an
-00000a30: 6420 4869 7374 6f72 7920 4150 4920 6d65  d History API me
-00000a40: 7468 6f64 2e20 2852 6571 7569 7265 6420  thod. (Required 
-00000a50: 666f 7220 4869 7374 6f72 7920 616e 6420  for History and 
-00000a60: 4675 7475 7265 2041 5049 290a 2020 2020  Future API).    
-00000a70: 656e 645f 6474 3a20 4f70 7469 6f6e 616c  end_dt: Optional
-00000a80: 5b3a 636c 6173 733a 6069 6e74 605d 0a20  [:class:`int`]. 
-00000a90: 2020 2020 2020 2052 6573 7472 6963 7420         Restrict 
-00000aa0: 6461 7465 206f 7574 7075 7420 666f 7220  date output for 
-00000ab0: 4869 7374 6f72 7920 4150 4920 6d65 7468  History API meth
-00000ac0: 6f64 2e20 4f6e 6c79 2077 6f72 6b73 2066  od. Only works f
-00000ad0: 6f72 2041 5049 206f 6e20 5072 6f20 706c  or API on Pro pl
-00000ae0: 616e 2061 6e64 2061 626f 7665 2e20 2841  an and above. (A
-00000af0: 7661 696c 6162 6c65 2066 6f72 2048 6973  vailable for His
-00000b00: 746f 7279 2041 5049 290a 2020 2020 686f  tory API).    ho
-00000b10: 7572 3a20 4f70 7469 6f6e 616c 5b3a 636c  ur: Optional[:cl
-00000b20: 6173 733a 6069 6e74 605d 0a20 2020 2020  ass:`int`].     
-00000b30: 2020 2052 6573 7472 6963 7469 6e67 2066     Restricting f
-00000b40: 6f72 6563 6173 7420 6f72 2068 6973 746f  orecast or histo
-00000b50: 7279 206f 7574 7075 7420 746f 2061 2073  ry output to a s
-00000b60: 7065 6369 6669 6320 686f 7572 2069 6e20  pecific hour in 
-00000b70: 6120 6769 7665 6e20 6461 792e 0a20 2020  a given day..   
-00000b80: 2061 7169 3a20 4c69 7465 7261 6c5b 2279   aqi: Literal["y
-00000b90: 6573 222c 2022 6e6f 225d 0a20 2020 2020  es", "no"].     
-00000ba0: 2020 2045 6e61 626c 652f 4469 7361 626c     Enable/Disabl
-00000bb0: 6520 4169 7220 5175 616c 6974 7920 6461  e Air Quality da
-00000bc0: 7461 2069 6e20 666f 7265 6361 7374 2041  ta in forecast A
-00000bd0: 5049 206f 7574 7075 742e 2044 6566 6175  PI output. Defau
-00000be0: 6c74 7320 746f 2022 6e6f 222e 0a20 2020  lts to "no"..   
-00000bf0: 2074 6964 6573 3a20 4c69 7465 7261 6c5b   tides: Literal[
-00000c00: 2279 6573 222c 2022 6e6f 225d 0a20 2020  "yes", "no"].   
-00000c10: 2020 2020 2045 6e61 626c 652f 4469 7361       Enable/Disa
-00000c20: 626c 6520 5469 6465 2064 6174 6120 696e  ble Tide data in
-00000c30: 204d 6172 696e 6520 4150 4920 6f75 7470   Marine API outp
-00000c40: 7574 2e20 4465 6661 756c 7473 2074 6f20  ut. Defaults to 
-00000c50: 226e 6f22 2e0a 2020 2020 6b77 6172 6773  "no"..    kwargs
-00000c60: 3a20 4469 6374 5b3a 636c 6173 733a 6073  : Dict[:class:`s
-00000c70: 7472 602c 2041 6e79 5d0a 2020 2020 2020  tr`, Any].      
-00000c80: 2020 4164 6469 7469 6f6e 616c 206b 6579    Additional key
-00000c90: 776f 7264 2061 7267 756d 656e 7473 2070  word arguments p
-00000ca0: 6173 7365 6420 6279 2064 6566 6175 6c74  assed by default
-00000cb0: 2074 6f20 7265 7175 6573 7473 206d 6164   to requests mad
-00000cc0: 6520 6279 2074 6865 2063 6c69 656e 740a  e by the client.
-00000cd0: 2020 2020 4eda 026e 6fda 0761 7069 5f6b      N..no..api_k
-00000ce0: 6579 da04 6c61 6e67 da02 6474 da06 656e  ey..lang..dt..en
-00000cf0: 645f 6474 da04 686f 7572 da03 6171 6929  d_dt..hour..aqi)
-00000d00: 02da 0379 6573 7219 0000 00da 0574 6964  ...yesr......tid
-00000d10: 6573 da06 6b77 6172 6773 da06 7265 7475  es..kwargs..retu
-00000d20: 726e 6308 0000 0000 0000 0000 0000 0004  rnc.............
-00000d30: 0000 000b 0000 00f3 5e01 0000 9501 9700  ........^.......
-00000d40: 6400 7d09 7c02 8116 7401 0000 0000 0000  d.}.|...t.......
-00000d50: 0000 0000 6a01 0000 0000 0000 0000 7c02  ....j.........|.
-00000d60: 6401 ac02 a602 0000 ab02 0000 0000 0000  d...............
-00000d70: 0000 7d09 6403 7c01 6901 7c08 a501 7d0a  ..}.d.|.i.|...}.
-00000d80: 7c09 721f 7c0a a002 0000 0000 0000 0000  |.r.|...........
-00000d90: 0000 0000 0000 0000 0000 0000 7c09 8107  ............|...
-00000da0: 7c09 6a03 0000 0000 0000 0000 6e01 6400  |.j.........n.d.
-00000db0: ac04 a601 0000 ab01 0000 0000 0000 0000  ................
-00000dc0: 0100 7409 0000 0000 0000 0000 0000 a600  ..t.............
-00000dd0: 0000 ab00 0000 0000 0000 0000 a005 0000  ................
-00000de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000df0: 0000 740c 0000 0000 0000 0000 0000 7c0a  ..t...........|.
-00000e00: ac05 a602 0000 ab02 0000 0000 0000 0000  ................
-00000e10: 0100 7c03 7c00 5f07 0000 0000 0000 0000  ..|.|._.........
-00000e20: 7c04 7c00 5f08 0000 0000 0000 0000 7c05  |.|._.........|.
-00000e30: 7c00 5f09 0000 0000 0000 0000 7c06 7c00  |._.........|.|.
-00000e40: 5f0a 0000 0000 0000 0000 7c07 7c00 5f0b  _.........|.|._.
-00000e50: 0000 0000 0000 0000 7c08 7c00 5f0c 0000  ........|.|._...
-00000e60: 0000 0000 0000 7c09 720f 741b 0000 0000  ......|.r.t.....
-00000e70: 0000 0000 0000 7c09 a601 0000 ab01 0000  ......|.........
-00000e80: 0000 0000 0000 6e01 6400 7c00 5f0e 0000  ......n.d.|._...
-00000e90: 0000 0000 0000 6400 5300 2906 4e54 a901  ......d.S.).NT..
-00000ea0: da05 6173 6f62 6ada 036b 6579 2901 721b  ..asobj..key).r.
-00000eb0: 0000 0029 02da 0862 6173 655f 7572 6cda  ...)...base_url.
-00000ec0: 0f64 6566 6175 6c74 5f6f 7074 696f 6e73  .default_options
-00000ed0: 290f 720f 0000 00da 0d66 696e 645f 6c61  ).r......find_la
-00000ee0: 6e67 7561 6765 da06 7570 6461 7465 da05  nguage..update..
-00000ef0: 7661 6c75 65da 0573 7570 6572 da08 5f5f  value..super..__
-00000f00: 696e 6974 5f5f da13 5745 4154 4845 5241  init__..WEATHERA
-00000f10: 5049 5f42 4153 455f 5552 4c72 1c00 0000  PI_BASE_URLr....
-00000f20: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000f30: 2100 0000 7222 0000 0072 0500 0000 721b  !...r"...r....r.
-00000f40: 0000 0029 0cda 0473 656c 6672 1a00 0000  ...)...selfr....
-00000f50: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000f60: 1e00 0000 721f 0000 0072 2100 0000 7222  ....r....r!...r"
-00000f70: 0000 00da 096c 616e 675f 636f 6465 da04  .....lang_code..
-00000f80: 6f70 7473 da09 5f5f 636c 6173 735f 5f73  opts..__class__s
-00000f90: 0c00 0000 2020 2020 2020 2020 2020 2080  ....           .
-00000fa0: fa31 6275 696c 645c 6264 6973 742e 7769  .1build\bdist.wi
-00000fb0: 6e2d 616d 6436 345c 6567 675c 7765 6174  n-amd64\egg\weat
-00000fc0: 6865 726c 795c 6170 695c 636c 6965 6e74  herly\api\client
-00000fd0: 2e70 7972 2e00 0000 7a19 5765 6174 6865  .pyr....z.Weathe
-00000fe0: 7241 5049 436c 6965 6e74 2e5f 5f69 6e69  rAPIClient.__ini
-00000ff0: 745f 5f50 0000 0073 d000 0000 f880 00f0  t__P...s........
-00001000: 1600 1519 8809 d80b 0fd0 0b1b dd18 1dd4  ................
-00001010: 182b a844 b804 d018 3dd1 183d d418 3d88  .+.D....=..=..=.
-00001020: 49e0 0c11 9037 f003 0310 0ae0 0e14 f005  I....7..........
-00001030: 0310 0a88 04f0 0800 0c15 d008 5c90 6497  ............\.d.
-00001040: 6b92 6bb8 49d0 3c51 a819 ac1f a81f d057  k.k.I.<Q.......W
-00001050: 5b90 6bd1 165c d416 5cd0 165c e508 0d89  [.k..\..\..\....
-00001060: 078c 07d7 0818 d208 18d5 2235 d829 2df0  .........."5.)-.
-00001070: 0300 0919 f100 0109 2ff4 0001 092f f000  ......../..../..
-00001080: 0109 2ff0 0600 1315 8804 8c07 d816 1c88  ../.............
-00001090: 048c 0bd8 1418 8804 8c09 d813 1688 048c  ................
-000010a0: 08d8 151a 8804 8c0a d816 1c88 048c 0bd8  ................
-000010b0: 2c35 d014 3f95 4998 69d1 1428 d414 28d0  ,5..?.I.i..(..(.
-000010c0: 1428 b834 8804 8c09 8809 8809 f300 0000  .(.4............
-000010d0: 00da 0865 6e64 706f 696e 74da 076f 7074  ...endpoint..opt
-000010e0: 696f 6e73 6303 0000 0000 0000 0000 0000  ionsc...........
-000010f0: 0005 0000 0003 0000 00f3 8202 0000 9700  ................
-00001100: 7c00 6a00 0000 0000 0000 0000 a001 0000  |.j.............
-00001110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001120: 0000 a600 0000 ab00 0000 0000 0000 0000  ................
-00001130: 7d03 7c03 a002 0000 0000 0000 0000 0000  }.|.............
-00001140: 0000 0000 0000 0000 0000 a600 0000 ab00  ................
-00001150: 0000 0000 0000 0000 4400 5d0a 5c02 0000  ........D.].\...
-00001160: 7d04 7d05 7c05 8003 7c03 7c04 3d00 8c0b  }.}.|...|.|.=...
-00001170: 7c02 a002 0000 0000 0000 0000 0000 0000  |...............
-00001180: 0000 0000 0000 0000 a600 0000 ab00 0000  ................
-00001190: 0000 0000 0000 4400 5d0c 5c02 0000 7d04  ......D.].\...}.
-000011a0: 7d05 7c05 8105 7c05 7c03 7c04 3c00 0000  }.|...|.|.|.<...
-000011b0: 8c0d 0200 7c00 6a03 0000 0000 0000 0000  ....|.j.........
-000011c0: 7c01 6601 6900 7c03 a401 8e01 7d06 7c06  |.f.i.|.....}.|.
-000011d0: 6402 1900 0000 0000 0000 0000 6a04 0000  d...........j...
-000011e0: 0000 0000 0000 6403 6b00 0000 0000 73c6  ......d.k.....s.
-000011f0: 7c06 6404 1900 0000 0000 0000 0000 6405  |.d...........d.
-00001200: 1900 0000 0000 0000 0000 7d07 7c07 6406  ..........}.|.d.
-00001210: 1900 0000 0000 0000 0000 7d08 7c06 6402  ..........}.|.d.
-00001220: 1900 0000 0000 0000 0000 6a04 0000 0000  ..........j.....
-00001230: 0000 0000 7d09 7c07 6407 1900 0000 0000  ....}.|.d.......
-00001240: 0000 0000 7d0a 7c08 6408 6b02 0000 0000  ....}.|.d.k.....
-00001250: 7211 740b 0000 0000 0000 0000 0000 7c09  r.t...........|.
-00001260: 7c08 7c0a a603 0000 ab03 0000 0000 0000  |.|.............
-00001270: 0000 8201 7c08 6409 6b02 0000 0000 7211  ....|.d.k.....r.
-00001280: 740d 0000 0000 0000 0000 0000 7c09 7c08  t...........|.|.
-00001290: 7c0a a603 0000 ab03 0000 0000 0000 0000  |...............
-000012a0: 8201 7c08 640a 6b02 0000 0000 7211 740f  ..|.d.k.....r.t.
-000012b0: 0000 0000 0000 0000 0000 7c09 7c08 7c0a  ..........|.|.|.
-000012c0: a603 0000 ab03 0000 0000 0000 0000 8201  ................
-000012d0: 7c08 640b 6b02 0000 0000 7211 7411 0000  |.d.k.....r.t...
-000012e0: 0000 0000 0000 0000 7c09 7c08 7c0a a603  ........|.|.|...
-000012f0: 0000 ab03 0000 0000 0000 0000 8201 7c08  ..............|.
-00001300: 640c 6b02 0000 0000 7211 7413 0000 0000  d.k.....r.t.....
-00001310: 0000 0000 0000 7c09 7c08 7c0a a603 0000  ......|.|.|.....
-00001320: ab03 0000 0000 0000 0000 8201 7c08 640d  ............|.d.
-00001330: 6b02 0000 0000 7211 7415 0000 0000 0000  k.....r.t.......
-00001340: 0000 0000 7c09 7c08 7c0a a603 0000 ab03  ....|.|.|.......
-00001350: 0000 0000 0000 0000 8201 7417 0000 0000  ..........t.....
-00001360: 0000 0000 0000 7c09 7c08 7c0a a603 0000  ......|.|.|.....
-00001370: ab03 0000 0000 0000 0000 8201 7c06 5300  ............|.S.
-00001380: 290e 7a32 5072 6976 6174 6520 6d65 7468  ).z2Private meth
-00001390: 6f64 2075 7365 6420 746f 206d 616b 6520  od used to make 
-000013a0: 7265 7175 6573 7473 2074 6f20 5765 6174  requests to Weat
-000013b0: 6865 7241 5049 4e72 0200 0000 6990 0100  herAPINr....i...
-000013c0: 0072 1000 0000 da05 6572 726f 72da 0463  .r......error..c
-000013d0: 6f64 65da 076d 6573 7361 6765 69ee 0300  ode..messagei...
-000013e0: 0069 d607 0000 69d7 0700 0069 d807 0000  .i....i....i....
-000013f0: 69d9 0700 0069 0f27 0000 290c 7229 0000  i....i.'..).r)..
-00001400: 00da 0463 6f70 79da 0569 7465 6d73 da08  ...copy..items..
-00001410: 5f72 6571 7565 7374 da0b 7374 6174 7573  _request..status
-00001420: 5f63 6f64 6572 0900 0000 720a 0000 0072  _coder....r....r
-00001430: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-00001440: 0000 0072 0800 0000 290b 7230 0000 0072  ...r....).r0...r
-00001450: 3600 0000 7237 0000 00da 0d66 696e 616c  6...r7.....final
-00001460: 5f6f 7074 696f 6e73 da01 6bda 0176 da04  _options..k..v..
-00001470: 7265 7370 da0a 6572 726f 725f 6461 7461  resp..error_data
-00001480: 723a 0000 00da 0673 7461 7475 73da 036d  r:.....status..m
-00001490: 7367 730b 0000 0020 2020 2020 2020 2020  sgs....         
-000014a0: 2020 7234 0000 00da 0d5f 6361 6c6c 5f72    r4....._call_r
-000014b0: 6571 7565 7374 7a1e 5765 6174 6865 7241  equestz.WeatherA
-000014c0: 5049 436c 6965 6e74 2e5f 6361 6c6c 5f72  PIClient._call_r
-000014d0: 6571 7565 7374 7000 0000 737a 0100 0080  equestp...sz....
-000014e0: 00e0 181c d418 2cd7 1831 d218 31d1 1833  ......,..1..1..3
-000014f0: d418 3388 0de0 1320 d713 26d2 1326 d113  ..3.... ..&..&..
-00001500: 28d4 1328 f000 0109 2ff0 0001 092f 8943  (..(..../..../.C
-00001510: 8841 8861 d80f 1088 7998 6da8 41d0 1e2e  .A.a....y.m.A...
-00001520: f8e0 131a 973d 923d 913f 943f f000 0109  .....=.=.?.?....
-00001530: 33f0 0001 0933 8943 8841 8861 d80f 1088  3....3.C.A.a....
-00001540: 7db0 1198 6da8 41d1 1e2e f8e0 0f1c 8874  }...m.A........t
-00001550: 8c7d 9858 d00f 37d0 0f37 a81d d00f 37d0  .}.X..7..7....7.
-00001560: 0f37 8804 e00f 1390 418c 77d4 0f22 a053  .7......A.w..".S
-00001570: d20f 28d0 0f28 e019 1d98 619c 17a0 17d4  ..(..(....a.....
-00001580: 1929 884a d813 1d98 66d4 1325 8844 d815  .).J....f..%.D..
-00001590: 1998 2194 57d4 1528 8846 d812 1c98 59d4  ..!.W..(.F....Y.
-000015a0: 1227 8843 e00f 1390 748a 7c88 7ca5 3fb0  .'.C....t.|.|.?.
-000015b0: 36b8 34c0 13d1 2345 d423 45d0 1d45 d811  6.4...#E.#E..E..
-000015c0: 1598 1492 1c90 1ca5 5db0 36b8 34c0 13d1  ........].6.4...
-000015d0: 2545 d425 45d0 1f45 d811 1598 1492 1c90  %E.%E..E........
-000015e0: 1cd5 2535 b066 b864 c043 d125 48d4 2548  ..%5.f.d.C.%H.%H
-000015f0: d01f 48d8 1115 9814 921c 901c a55e b046  ..H..........^.F
-00001600: b844 c023 d125 46d4 2546 d01f 46d8 1115  .D.#.%F.%F..F...
-00001610: 9814 921c 901c a55c b026 b824 c003 d125  .......\.&.$...%
-00001620: 44d4 2544 d01f 44d8 1115 9814 921c 901c  D.%D..D.........
-00001630: d525 3db8 66c0 64c8 43d1 2550 d425 50d0  .%=.f.d.C.%P.%P.
-00001640: 1f50 dd18 2ba8 46b0 44b8 23d1 183e d418  .P..+.F.D.#..>..
-00001650: 3ed0 123e e00f 1388 0b72 3500 0000 6302  >..>.....r5...c.
-00001660: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00001670: 0000 00f3 5600 0000 9700 7401 0000 0000  ....V.....t.....
-00001680: 0000 0000 0000 6a01 0000 0000 0000 0000  ......j.........
-00001690: 7c01 6401 ac02 a602 0000 ab02 0000 0000  |.d.............
-000016a0: 0000 0000 7d02 7c02 7309 6403 7c00 5f02  ....}.|.s.d.|._.
-000016b0: 0000 0000 0000 0000 6404 5300 7c02 7c00  ........d.S.|.|.
-000016c0: 5f02 0000 0000 0000 0000 6401 5300 2905  _.........d.S.).
-000016d0: 6108 0200 000a 2020 2020 2020 2020 5365  a.....        Se
-000016e0: 7420 636c 6965 6e74 2773 206c 616e 6775  t client's langu
-000016f0: 6167 6520 7768 656e 2072 6571 7565 7374  age when request
-00001700: 696e 6720 6461 7461 2e0a 2020 2020 2020  ing data..      
-00001710: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-00001720: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00001730: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00001740: 2020 6c61 6e67 3a20 556e 696f 6e5b 3a63    lang: Union[:c
-00001750: 6c61 7373 3a60 7374 7260 2c20 3a63 6c61  lass:`str`, :cla
-00001760: 7373 3a60 4c61 6e67 7561 6765 7360 5d0a  ss:`Languages`].
-00001770: 2020 2020 2020 2020 2020 2020 4c61 6e67              Lang
-00001780: 7561 6765 2074 6f20 7365 742e 2043 616e  uage to set. Can
-00001790: 2062 6520 6569 7468 6572 2061 2073 7472   be either a str
-000017a0: 696e 6720 7468 6174 2069 7320 6c61 6e75  ing that is lanu
-000017b0: 6167 6527 7320 6e61 6d65 206f 7220 636f  age's name or co
-000017c0: 6465 206f 7220 6120 3a63 6c61 7373 3a60  de or a :class:`
-000017d0: 4c61 6e67 7561 6765 7360 2065 6e75 6d20  Languages` enum 
-000017e0: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-000017f0: 2020 2020 0a20 2020 2020 2020 2052 6574      .        Ret
-00001800: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00001810: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 203a  ------.        :
-00001820: 636c 6173 733a 6062 6f6f 6c60 0a20 2020  class:`bool`.   
-00001830: 2020 2020 2020 2020 2041 2062 6f6f 6c65           A boole
-00001840: 616e 2069 6e64 6963 6174 696e 6720 7768  an indicating wh
-00001850: 6574 6865 7220 7468 6520 6c61 6e67 7561  ether the langua
-00001860: 6765 2077 6173 2073 7563 6365 7373 6675  ge was successfu
-00001870: 6c6c 7920 7365 742e 2049 6620 6974 2773  lly set. If it's
-00001880: 2060 6046 616c 7365 6060 2c20 7468 656e   ``False``, then
-00001890: 2073 6f6d 6574 6869 6e67 2077 656e 7420   something went 
-000018a0: 7772 6f6e 672c 2070 726f 6261 626c 7920  wrong, probably 
-000018b0: 6265 6361 7573 6520 6f66 2074 6865 2077  because of the w
-000018c0: 726f 6e67 2060 606c 616e 6760 6020 7661  rong ``lang`` va
-000018d0: 6c75 652e 0a20 2020 2020 2020 2054 7225  lue..        Tr%
-000018e0: 0000 004e 4629 0372 0f00 0000 722a 0000  ...NF).r....r*..
-000018f0: 0072 1b00 0000 2903 7230 0000 0072 1b00  .r....).r0...r..
-00001900: 0000 da0a 6c61 6e67 5f63 6c61 7373 7303  ....lang_classs.
-00001910: 0000 0020 2020 7234 0000 00da 0c73 6574  ...   r4.....set
-00001920: 5f6c 616e 6775 6167 657a 1d57 6561 7468  _languagez.Weath
-00001930: 6572 4150 4943 6c69 656e 742e 7365 745f  erAPIClient.set_
-00001940: 6c61 6e67 7561 6765 8d00 0000 7339 0000  language....s9..
-00001950: 0080 00f5 1c00 161b d415 28a8 14b0 54d0  ..........(...T.
-00001960: 153a d115 3ad4 153a 880a d80f 19f0 0002  .:..:..:........
-00001970: 0919 d818 1c88 448c 49d8 1318 9035 e014  ......D.I....5..
-00001980: 1e88 048c 09d8 0f13 8874 7235 0000 00da  .........tr5....
-00001990: 0571 7565 7279 2903 7220 0000 0072 1900  .query).r ...r..
-000019a0: 0000 4e63 0400 0000 0000 0000 0000 0000  ..Nc............
-000019b0: 0500 0000 0b00 0000 f3a0 0000 0097 007c  ...............|
-000019c0: 0370 067c 006a 0000 0000 0000 0000 007c  .p.|.j.........|
-000019d0: 0164 019c 027c 04a5 017d 057c 0281 057c  .d...|...}.|...|
-000019e0: 027c 0564 033c 0000 007c 00a0 0100 0000  .|.d.<...|......
-000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a00: 0064 047c 05a6 0200 00ab 0200 0000 0000  .d.|............
-00001a10: 0000 007d 0674 0500 0000 0000 0000 0000  ...}.t..........
-00001a20: 007c 0664 0519 0000 0000 0000 0000 007c  .|.d...........|
-00001a30: 0664 0619 0000 0000 0000 0000 006a 0300  .d...........j..
-00001a40: 0000 0000 0000 0064 02a6 0300 00ab 0300  .......d........
-00001a50: 0000 0000 0000 007d 077c 0753 0029 0761  .......}.|.S.).a
-00001a60: d505 0000 0a20 2020 2020 2020 2047 6574  .....        Get
-00001a70: 2063 7572 7265 6e74 2077 6561 7468 6572   current weather
-00001a80: 2064 6174 610a 0a20 2020 2020 2020 2050   data..        P
-00001a90: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00001aa0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00001ab0: 2020 2020 2071 7565 7279 3a20 3a63 6c61       query: :cla
-00001ac0: 7373 3a60 7374 7260 0a20 2020 2020 2020  ss:`str`.       
-00001ad0: 2020 2020 2051 7565 7279 2073 7472 696e       Query strin
-00001ae0: 6720 2d20 6c6f 6361 7469 6f6e 2079 6f75  g - location you
-00001af0: 2077 616e 7420 746f 2067 6574 2077 6561   want to get wea
-00001b00: 7468 6572 2064 6174 6120 666f 720a 2020  ther data for.  
-00001b10: 2020 2020 2020 6c61 6e67 3a20 4f70 7469        lang: Opti
-00001b20: 6f6e 616c 5b55 6e69 6f6e 5b3a 636c 6173  onal[Union[:clas
-00001b30: 733a 6073 7472 602c 204c 616e 6775 6167  s:`str`, Languag
-00001b40: 6573 5d5d 0a20 2020 2020 2020 2020 2020  es]].           
-00001b50: 204c 616e 6775 6167 6520 6672 6f6d 2074   Language from t
-00001b60: 6865 203a 636c 6173 733a 604c 616e 6775  he :class:`Langu
-00001b70: 6167 6573 6020 656e 756d 206f 7220 6120  ages` enum or a 
-00001b80: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-00001b90: 696e 6720 7468 6520 6c61 6e67 7561 6765  ing the language
-00001ba0: 206f 7220 6c61 6e67 7561 6765 2063 6f64   or language cod
-00001bb0: 6520 2870 7265 6665 7261 626c 7929 2e0a  e (preferably)..
-00001bc0: 2020 2020 2020 2020 2020 2020 546f 2067              To g
-00001bd0: 6574 2061 206c 6973 7420 6f66 206c 616e  et a list of lan
-00001be0: 6775 6167 6573 2076 6973 6974 203a 636c  guages visit :cl
-00001bf0: 6173 733a 604c 616e 6775 6167 6573 602e  ass:`Languages`.
-00001c00: 0a20 2020 2020 2020 2061 7169 3a20 4c69  .        aqi: Li
-00001c10: 7465 7261 6c5b 2279 6573 222c 2022 6e6f  teral["yes", "no
-00001c20: 222c 204e 6f6e 655d 0a20 2020 2020 2020  ", None].       
-00001c30: 2020 2020 2045 6e61 626c 652f 4469 7361       Enable/Disa
-00001c40: 626c 6520 4169 7220 5175 616c 6974 7920  ble Air Quality 
-00001c50: 6461 7461 2069 6e20 666f 7265 6361 7374  data in forecast
-00001c60: 2041 5049 206f 7574 7075 742e 2049 6620   API output. If 
-00001c70: 6e6f 7468 696e 6720 6973 2070 6173 7365  nothing is passe
-00001c80: 732c 2074 6865 6e20 6974 2064 6566 6175  s, then it defau
-00001c90: 6c74 7320 746f 2063 6c69 656e 7420 6465  lts to client de
-00001ca0: 6661 756c 7420 7661 6c75 652e 0a20 2020  fault value..   
-00001cb0: 2020 2020 206b 7761 7267 733a 2044 6963       kwargs: Dic
-00001cc0: 745b 3a63 6c61 7373 3a60 7374 7260 2c20  t[:class:`str`, 
-00001cd0: 416e 795d 0a20 2020 2020 2020 2020 2020  Any].           
-00001ce0: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
-00001cf0: 6f72 6420 6172 6775 6d65 6e74 7320 746f  ord arguments to
-00001d00: 2072 6571 7565 7374 0a0a 2020 2020 2020   request..      
-00001d10: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00001d20: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00001d30: 2020 3a63 6c61 7373 3a60 4375 7272 656e    :class:`Curren
-00001d40: 7457 6561 7468 6572 4461 7461 600a 2020  tWeatherData`.  
-00001d50: 2020 2020 2020 2020 2020 4375 7272 656e            Curren
-00001d60: 7420 7765 6174 6865 7220 6461 7461 2063  t weather data c
-00001d70: 6c61 7373 0a0a 2020 2020 2020 2020 5261  lass..        Ra
-00001d80: 6973 6573 0a20 2020 2020 2020 202d 2d2d  ises.        ---
-00001d90: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 203a  ------.        :
-00001da0: 6578 633a 604e 6f4c 6f63 6174 696f 6e46  exc:`NoLocationF
-00001db0: 6f75 6e64 600a 2020 2020 2020 2020 2020  ound`.          
-00001dc0: 2020 5261 6973 6564 2077 6865 6e20 6e6f    Raised when no
-00001dd0: 206c 6f63 6174 696f 6e20 666f 7220 6769   location for gi
-00001de0: 7665 6e20 7175 6572 7920 7761 7320 666f  ven query was fo
-00001df0: 756e 640a 2020 2020 2020 2020 3a65 7863  und.        :exc
-00001e00: 3a60 496e 7661 6c69 6441 5049 4b65 7960  :`InvalidAPIKey`
-00001e10: 0a20 2020 2020 2020 2020 2020 2052 6169  .            Rai
-00001e20: 7365 6420 7768 656e 2074 6865 2041 5049  sed when the API
-00001e30: 206b 6579 2069 7320 696e 7661 6c69 640a   key is invalid.
-00001e40: 2020 2020 2020 2020 3a65 7863 3a60 4150          :exc:`AP
-00001e50: 494c 696d 6974 4578 6365 6564 6564 600a  ILimitExceeded`.
-00001e60: 2020 2020 2020 2020 2020 2020 5261 6973              Rais
-00001e70: 6564 2077 6865 6e20 4150 4920 6b65 7920  ed when API key 
-00001e80: 6361 6c6c 7320 6c69 6d69 7420 7761 7320  calls limit was 
-00001e90: 6578 6365 6564 6564 0a20 2020 2020 2020  exceeded.       
-00001ea0: 203a 6578 633a 6041 5049 4b65 7944 6973   :exc:`APIKeyDis
-00001eb0: 6162 6c65 6460 0a20 2020 2020 2020 2020  abled`.         
-00001ec0: 2020 2052 6169 7365 6420 7768 656e 2041     Raised when A
-00001ed0: 5049 206b 6579 2069 7320 6469 7361 626c  PI key is disabl
-00001ee0: 6564 0a20 2020 2020 2020 203a 6578 633a  ed.        :exc:
-00001ef0: 6041 6363 6573 7344 656e 6965 6460 0a20  `AccessDenied`. 
-00001f00: 2020 2020 2020 2020 2020 2052 6169 7365             Raise
-00001f10: 6420 7768 656e 2061 6363 6573 7320 746f  d when access to
-00001f20: 2067 6976 656e 2072 6573 6f75 7263 6520   given resource 
-00001f30: 7761 7320 6465 6e69 6564 0a20 2020 2020  was denied.     
-00001f40: 2020 203a 6578 633a 6049 6e74 6572 6e61     :exc:`Interna
-00001f50: 6c41 7070 6c69 6361 7469 6f6e 4572 726f  lApplicationErro
-00001f60: 7260 0a20 2020 2020 2020 2020 2020 2052  r`.            R
-00001f70: 6169 7365 6420 7768 656e 2074 6865 7265  aised when there
-00001f80: 2077 6173 2061 2076 6572 7920 7261 7265   was a very rare
-00001f90: 2069 6e74 6572 6e61 6c20 6170 706c 6963   internal applic
-00001fa0: 6174 696f 6e20 6572 726f 720a 2020 2020  ation error.    
-00001fb0: 2020 2020 3a65 7863 3a60 5765 6174 6865      :exc:`Weathe
-00001fc0: 7241 5049 4578 6365 7074 696f 6e60 0a20  rAPIException`. 
-00001fd0: 2020 2020 2020 2020 2020 2052 6169 7365             Raise
-00001fe0: 6420 7768 656e 2073 6f6d 6574 6869 6e67  d when something
-00001ff0: 2065 6c73 6520 7765 6e74 2077 726f 6e67   else went wrong
-00002000: 2c20 7468 6174 2064 6f65 7320 6e6f 7420  , that does not 
-00002010: 6861 7665 2061 2073 7065 6369 6669 6320  have a specific 
-00002020: 6578 6365 7074 696f 6e20 636c 6173 732e  exception class.
-00002030: 0a20 2020 2020 2020 2029 0272 1f00 0000  .        ).r....
-00002040: da01 714e 721b 0000 007a 0c63 7572 7265  ..qNr....z.curre
-00002050: 6e74 2e6a 736f 6e72 1000 0000 7202 0000  nt.jsonr....r...
-00002060: 0029 0472 1f00 0000 7247 0000 0072 0600  .).r....rG...r..
-00002070: 0000 723f 0000 0029 0872 3000 0000 724b  ..r?...).r0...rK
-00002080: 0000 0072 1b00 0000 721f 0000 0072 2200  ...r....r....r".
-00002090: 0000 7237 0000 0072 4300 0000 da07 7765  ..r7...rC.....we
-000020a0: 6174 6865 7273 0800 0000 2020 2020 2020  athers....      
-000020b0: 2020 7234 0000 00da 1367 6574 5f63 7572    r4.....get_cur
-000020c0: 7265 6e74 5f77 6561 7468 6572 7a24 5765  rent_weatherz$We
-000020d0: 6174 6865 7241 5049 436c 6965 6e74 2e67  atherAPIClient.g
-000020e0: 6574 5f63 7572 7265 6e74 5f77 6561 7468  et_current_weath
-000020f0: 6572 a300 0000 736d 0000 0080 00f0 5801  er....sm......X.
-00002100: 0014 1790 3f98 249c 28d8 1116 f005 0413  ....?.$.(.......
-00002110: 0af0 0004 130a f006 000f 15f0 0704 130a  ................
-00002120: 8807 f00a 000c 10d0 0b1b a874 9857 a056  ...........t.W.V
-00002130: 995f d80f 13d7 0f21 d20f 21a0 2eb0 27d1  ._.....!..!...'.
-00002140: 0f3a d40f 3a88 04e5 1224 a054 a821 a457  .:..:....$.T.!.W
-00002150: a864 b031 ac67 d42e 41c0 34d1 1248 d412  .d.1.g..A.4..H..
-00002160: 4888 07d8 0f16 880e 7235 0000 0063 0200  H.......r5...c..
-00002170: 0000 0000 0000 0000 0000 0800 0000 0300  ................
-00002180: 0000 f3ae 0000 0097 007c 00a0 0000 0000  .........|......
-00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021a0: 0064 0164 027c 0169 01a6 0200 00ab 0200  .d.d.|.i........
-000021b0: 0000 0000 0000 007d 0267 007d 037c 0264  .......}.g.}.|.d
-000021c0: 0319 0000 0000 0000 0000 0044 005d 317d  ...........D.]1}
-000021d0: 047c 03a0 0100 0000 0000 0000 0000 0000  .|..............
-000021e0: 0000 0000 0000 0000 0074 0500 0000 0000  .........t......
-000021f0: 0000 0000 007c 047c 0264 0419 0000 0000  .....|.|.d......
-00002200: 0000 0000 006a 0300 0000 0000 0000 0064  .....j.........d
-00002210: 05a6 0300 00ab 0300 0000 0000 0000 00a6  ................
-00002220: 0100 00ab 0100 0000 0000 0000 0001 008c  ................
-00002230: 327c 0353 0029 0661 ec03 0000 0a20 2020  2|.S.).a.....   
-00002240: 2020 2020 2047 6574 206c 6f63 6174 696f       Get locatio
-00002250: 6e73 2066 6f72 2067 6976 656e 2071 7565  ns for given que
-00002260: 7279 0a0a 2020 2020 2020 2020 5061 7261  ry..        Para
-00002270: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00002280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00002290: 2020 2020 2020 2071 7565 7279 3a20 3a63         query: :c
-000022a0: 6c61 7373 3a60 7374 7260 0a20 2020 2020  lass:`str`.     
-000022b0: 2020 2020 2020 2051 7565 7279 2073 7472         Query str
-000022c0: 696e 672c 2061 206c 6f63 6174 696f 6e20  ing, a location 
-000022d0: 796f 7520 6172 6520 7365 6172 6368 696e  you are searchin
-000022e0: 6720 666f 720a 0a20 2020 2020 2020 2052  g for..        R
-000022f0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00002300: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00002310: 2020 204c 6973 745b 3a63 6c61 7373 3a60     List[:class:`
-00002320: 4c6f 6361 7469 6f6e 4461 7461 605d 0a20  LocationData`]. 
-00002330: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
-00002340: 7420 6f66 203a 636c 6173 733a 604c 6f63  t of :class:`Loc
-00002350: 6174 696f 6e44 6174 6160 2063 6c61 7373  ationData` class
-00002360: 6573 2e0a 0a20 2020 2020 2020 2052 6169  es...        Rai
-00002370: 7365 730a 2020 2020 2020 2020 2d2d 2d2d  ses.        ----
-00002380: 2d2d 2d2d 2d0a 2020 2020 2020 2020 3a65  -----.        :e
-00002390: 7863 3a60 4e6f 4c6f 6361 7469 6f6e 466f  xc:`NoLocationFo
-000023a0: 756e 6460 0a20 2020 2020 2020 2020 2020  und`.           
-000023b0: 2052 6169 7365 6420 7768 656e 206e 6f20   Raised when no 
-000023c0: 6c6f 6361 7469 6f6e 2066 6f72 2067 6976  location for giv
-000023d0: 656e 2071 7565 7279 2077 6173 2066 6f75  en query was fou
-000023e0: 6e64 0a20 2020 2020 2020 203a 6578 633a  nd.        :exc:
-000023f0: 6049 6e76 616c 6964 4150 494b 6579 600a  `InvalidAPIKey`.
-00002400: 2020 2020 2020 2020 2020 2020 5261 6973              Rais
-00002410: 6564 2077 6865 6e20 7468 6520 4150 4920  ed when the API 
-00002420: 6b65 7920 6973 2069 6e76 616c 6964 0a20  key is invalid. 
-00002430: 2020 2020 2020 203a 6578 633a 6041 5049         :exc:`API
-00002440: 4c69 6d69 7445 7863 6565 6465 6460 0a20  LimitExceeded`. 
-00002450: 2020 2020 2020 2020 2020 2052 6169 7365             Raise
-00002460: 6420 7768 656e 2041 5049 206b 6579 2063  d when API key c
-00002470: 616c 6c73 206c 696d 6974 2077 6173 2065  alls limit was e
-00002480: 7863 6565 6465 640a 2020 2020 2020 2020  xceeded.        
-00002490: 3a65 7863 3a60 4150 494b 6579 4469 7361  :exc:`APIKeyDisa
-000024a0: 626c 6564 600a 2020 2020 2020 2020 2020  bled`.          
-000024b0: 2020 5261 6973 6564 2077 6865 6e20 4150    Raised when AP
-000024c0: 4920 6b65 7920 6973 2064 6973 6162 6c65  I key is disable
-000024d0: 640a 2020 2020 2020 2020 3a65 7863 3a60  d.        :exc:`
-000024e0: 4163 6365 7373 4465 6e69 6564 600a 2020  AccessDenied`.  
-000024f0: 2020 2020 2020 2020 2020 5261 6973 6564            Raised
-00002500: 2077 6865 6e20 6163 6365 7373 2074 6f20   when access to 
-00002510: 6769 7665 6e20 7265 736f 7572 6365 2077  given resource w
-00002520: 6173 2064 656e 6965 640a 2020 2020 2020  as denied.      
-00002530: 2020 3a65 7863 3a60 496e 7465 726e 616c    :exc:`Internal
-00002540: 4170 706c 6963 6174 696f 6e45 7272 6f72  ApplicationError
-00002550: 600a 2020 2020 2020 2020 2020 2020 5261  `.            Ra
-00002560: 6973 6564 2077 6865 6e20 7468 6572 6520  ised when there 
-00002570: 7761 7320 6120 7665 7279 2072 6172 6520  was a very rare 
-00002580: 696e 7465 726e 616c 2061 7070 6c69 6361  internal applica
-00002590: 7469 6f6e 2065 7272 6f72 0a20 2020 2020  tion error.     
-000025a0: 2020 203a 6578 633a 6057 6561 7468 6572     :exc:`Weather
-000025b0: 4150 4945 7863 6570 7469 6f6e 600a 2020  APIException`.  
-000025c0: 2020 2020 2020 2020 2020 5261 6973 6564            Raised
-000025d0: 2077 6865 6e20 736f 6d65 7468 696e 6720   when something 
-000025e0: 656c 7365 2077 656e 7420 7772 6f6e 672c  else went wrong,
-000025f0: 2074 6861 7420 646f 6573 206e 6f74 2068   that does not h
-00002600: 6176 6520 6120 7370 6563 6966 6963 2065  ave a specific e
-00002610: 7863 6570 7469 6f6e 2063 6c61 7373 2e0a  xception class..
-00002620: 2020 2020 2020 2020 7a0b 7365 6172 6368          z.search
-00002630: 2e6a 736f 6e72 4d00 0000 7210 0000 0072  .jsonrM...r....r
-00002640: 0200 0000 4e29 0472 4700 0000 da06 6170  ....N).rG.....ap
-00002650: 7065 6e64 7207 0000 0072 3f00 0000 2905  pendr....r?...).
-00002660: 7230 0000 0072 4b00 0000 7243 0000 00da  r0...rK...rC....
-00002670: 096c 6f63 6174 696f 6e73 da03 6c6f 6373  .locations..locs
-00002680: 0500 0000 2020 2020 2072 3400 0000 da0d  ....     r4.....
-00002690: 6765 745f 6c6f 6361 7469 6f6e 737a 1e57  get_locationsz.W
-000026a0: 6561 7468 6572 4150 4943 6c69 656e 742e  eatherAPIClient.
-000026b0: 6765 745f 6c6f 6361 7469 6f6e 73d9 0000  get_locations...
-000026c0: 0073 6700 0000 8000 f03e 0010 14d7 0f21  .sg......>.....!
-000026d0: d20f 21a0 2db0 13b0 65b0 0cd1 0f3d d40f  ..!.-...e....=..
-000026e0: 3d88 04e0 1416 8809 d813 1798 0194 37f0  =.............7.
-000026f0: 0001 094b 01f0 0001 094b 0188 43d8 0c15  ...K.....K..C...
-00002700: d70c 1cd2 0c1c 9d5c a823 a874 b041 ac77  .......\.#.t.A.w
-00002710: d42f 42c0 44d1 1d49 d41d 49d1 0c4a d40c  ./B.D..I..I..J..
-00002720: 4ad0 0c4a d00c 4ad8 0f18 d008 1872 3500  J..J..J......r5.
-00002730: 0000 6301 0000 0000 0000 0000 0000 0007  ..c.............
-00002740: 0000 0003 0000 00f3 4e00 0000 9700 6401  ........N.....d.
-00002750: 7c00 6a00 0000 0000 0000 0000 6a01 0000  |.j.........j...
-00002760: 0000 0000 0000 9b00 6402 7c00 6a02 0000  ........d.|.j...
-00002770: 0000 0000 0000 6403 1900 0000 0000 0000  ......d.........
-00002780: 0000 9b00 6404 7c00 6a03 0000 0000 0000  ....d.|.j.......
-00002790: 0000 9b00 6405 9d07 5300 a906 4efa 013c  ....d...S...N..<
-000027a0: 7a09 2061 7069 5f6b 6579 3d72 2700 0000  z. api_key=r'...
-000027b0: 7a06 206c 616e 673d fa01 3e29 0472 3300  z. lang=..>).r3.
-000027c0: 0000 da08 5f5f 6e61 6d65 5f5f 7229 0000  ....__name__r)..
-000027d0: 0072 1b00 0000 a901 7230 0000 0073 0100  .r......r0...s..
-000027e0: 0000 2072 3400 0000 da07 5f5f 7374 725f  .. r4.....__str_
-000027f0: 5f7a 1857 6561 7468 6572 4150 4943 6c69  _z.WeatherAPICli
-00002800: 656e 742e 5f5f 7374 725f 5fff 0000 0073  ent.__str__....s
-00002810: 3400 0000 8000 d80f 6490 3494 3ed4 132a  4.......d.4.>..*
-00002820: d00f 64d0 0f64 b054 d435 49c8 25d4 3550  ..d..d.T.5I.%.5P
-00002830: d00f 64d0 0f64 d058 5cd4 5861 d00f 64d0  ..d..d.X\.Xa..d.
-00002840: 0f64 d00f 64d0 0864 7235 0000 0063 0100  .d..d..dr5...c..
-00002850: 0000 0000 0000 0000 0000 0900 0000 0300  ................
-00002860: 0000 f368 0000 0097 0074 0100 0000 0000  ...h.....t......
-00002870: 0000 0000 0064 017c 006a 0100 0000 0000  .....d.|.j......
-00002880: 0000 006a 0200 0000 0000 0000 009b 0064  ...j...........d
-00002890: 027c 006a 0300 0000 0000 0000 0064 0319  .|.j.........d..
-000028a0: 0000 0000 0000 0000 009b 0064 047c 006a  ...........d.|.j
-000028b0: 0400 0000 0000 0000 009b 0064 059d 07a6  ...........d....
-000028c0: 0100 00ab 0100 0000 0000 0000 0053 0072  .............S.r
-000028d0: 5600 0000 2905 da04 7265 7072 7233 0000  V...)...reprr3..
-000028e0: 0072 5900 0000 7229 0000 0072 1b00 0000  .rY...r)...r....
-000028f0: 725a 0000 0073 0100 0000 2072 3400 0000  rZ...s.... r4...
-00002900: da08 5f5f 7265 7072 5f5f 7a19 5765 6174  ..__repr__z.Weat
-00002910: 6865 7241 5049 436c 6965 6e74 2e5f 5f72  herAPIClient.__r
-00002920: 6570 725f 5f02 0100 0073 3d00 0000 8000  epr__....s=.....
-00002930: dd0f 13d0 1469 9804 9c0e d418 2fd0 1469  .....i....../..i
-00002940: d014 69b8 24d4 3a4e c875 d43a 55d0 1469  ..i.$.:N.u.:U..i
-00002950: d014 69d0 5d61 d45d 66d0 1469 d014 69d0  ..i.]a.]f..i..i.
-00002960: 1469 d10f 6ad4 0f6a d008 6a72 3500 0000  .i..j..j..jr5...
-00002970: 2906 4e4e 4e4e 7219 0000 0072 1900 0000  ).NNNNr....r....
-00002980: 2902 4e4e 2915 7259 0000 00da 0a5f 5f6d  ).NN).rY.....__m
-00002990: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000029a0: 616d 655f 5fda 075f 5f64 6f63 5f5f da03  ame__..__doc__..
-000029b0: 7374 7272 1400 0000 7215 0000 0072 0500  strr....r....r..
-000029c0: 0000 da03 696e 7472 1200 0000 7213 0000  ....intr....r...
-000029d0: 0072 1100 0000 722e 0000 0072 4700 0000  .r....r....rG...
-000029e0: 724a 0000 0072 0600 0000 724f 0000 0072  rJ...r....rO...r
-000029f0: 5400 0000 725b 0000 0072 5e00 0000 da0d  T...r[...r^.....
-00002a00: 5f5f 636c 6173 7363 656c 6c5f 5f29 0172  __classcell__).r
-00002a10: 3300 0000 7301 0000 0040 7234 0000 0072  3...s....@r4...r
-00002a20: 1700 0000 7217 0000 0038 0000 0073 1302  ....r....8...s..
-00002a30: 0000 f880 0080 0080 0080 0080 00f0 0216  ................
-00002a40: 0508 f000 1605 08f0 3400 3135 d81c 20d8  ........4.15.. .
-00002a50: 2024 d81e 22d8 2428 d826 2af0 111d 0540   $..".$(.&*....@
-00002a60: 01f0 001d 0540 01e0 1114 f005 1d05 4001  .....@........@.
-00002a70: f006 000f 1790 7598 53a0 2998 5ed4 172c  ......u.S.).^..,
-00002a80: d40e 2df0 071d 0540 01f0 0800 0d15 9053  ..-....@.......S
-00002a90: 8c4d f009 1d05 4001 f00a 0011 1998 1394  .M....@.........
-00002aa0: 0df0 0b1d 0540 01f0 0c00 0f17 9073 8c6d  .....@.......s.m
-00002ab0: f00d 1d05 4001 f00e 000e 1590 5bd4 0d21  ....@.......[..!
-00002ac0: f00f 1d05 4001 f010 0010 1790 7bd4 0f23  ....@.......{..#
-00002ad0: f011 1d05 4001 f012 0013 1790 7398 4390  ....@.......s.C.
-00002ae0: 7894 2ef0 131d 0540 01f0 1400 0a0e f015  x......@........
-00002af0: 1d05 4001 f000 1d05 4001 f000 1d05 4001  ..@.....@.....@.
-00002b00: f000 1d05 4001 f000 1d05 4001 f000 1d05  ....@.....@.....
-00002b10: 4001 f040 011b 0514 a063 f000 1b05 14b0  @..@.....c......
-00002b20: 44b8 13b8 63b8 18b4 4ef0 001b 0514 c074  D...c...N......t
-00002b30: c843 d051 54c8 48c4 7ef0 001b 0514 f000  .C.QT.H.~.......
-00002b40: 1b05 14f0 001b 0514 f000 1b05 14f0 3a14  ..............:.
-00002b50: 0514 a015 a073 a849 a07e d421 36f0 0014  .....s.I.~.!6...
-00002b60: 0514 b835 c019 c844 c01f d43b 51f0 0014  ...5...D...;Q...
-00002b70: 0514 f000 1405 14f0 0014 0514 f000 1405  ................
-00002b80: 14f0 3000 3135 d82a 2ef0 0734 0517 f000  ..0.15.*...4....
-00002b90: 3405 17d8 0f12 f003 3405 17e0 0e16 9075  4.......4......u
-00002ba0: 9853 a029 985e d417 2cd4 0e2d f005 3405  .S.).^..,..-..4.
-00002bb0: 17f0 0600 0e15 d015 26d4 0d27 f007 3405  ........&..'..4.
-00002bc0: 17f0 0800 1317 9073 9843 9078 942e f009  .......s.C.x....
-00002bd0: 3405 17f0 0a00 0a1c f00b 3405 17f0 0034  4.........4....4
-00002be0: 0517 f000 3405 17f0 0034 0517 f06c 0124  ....4....4...l.$
-00002bf0: 0519 a033 f000 2405 19f0 0024 0519 f000  ...3..$....$....
-00002c00: 2405 19f0 0024 0519 f04c 0101 0565 01f0  $....$...L...e..
-00002c10: 0001 0565 01f0 0001 0565 01f0 0601 056b  ...e.....e.....k
-00002c20: 01f0 0001 056b 01f0 0001 056b 01f0 0001  .....k.....k....
-00002c30: 056b 01f0 0001 056b 01f0 0001 056b 01f0  .k.....k.....k..
-00002c40: 0001 056b 0172 3500 0000 7217 0000 004e  ...k.r5...r....N
-00002c50: 291c 7261 0000 00da 0463 6f72 6572 0300  ).ra.....corer..
-00002c60: 0000 da05 656e 756d 7372 0500 0000 da09  ....enumsr......
-00002c70: 7265 7370 6f6e 7365 7372 0600 0000 7207  responsesr....r.
-00002c80: 0000 00da 0665 7272 6f72 7372 0800 0000  .....errorsr....
-00002c90: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00002ca0: 0c00 0000 720d 0000 0072 0e00 0000 da00  ....r....r......
-00002cb0: 720f 0000 00da 0674 7970 696e 6772 1100  r......typingr..
-00002cc0: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00002cd0: 0072 1500 0000 7216 0000 0072 2f00 0000  .r....r....r/...
-00002ce0: da07 5f5f 616c 6c5f 5f72 1700 0000 a900  ..__all__r......
-00002cf0: 7235 0000 0072 3400 0000 fa08 3c6d 6f64  r5...r4.....<mod
-00002d00: 756c 653e 726d 0000 0001 0000 0073 6c01  ule>rm.......sl.
-00002d10: 0000 f003 0101 01f0 0216 0104 f000 1601  ................
-00002d20: 04f0 3000 0120 d000 1fd0 001f d000 1fd0  ..0.. ..........
-00002d30: 001f d000 1fd8 001d d000 1dd0 001d d000  ................
-00002d40: 1dd0 001d d000 1dd8 0038 d000 38d0 0038  .........8..8..8
-00002d50: d000 38d0 0038 d000 38d0 0038 d000 38f0  ..8..8..8..8..8.
-00002d60: 0208 0102 f000 0801 02f0 0008 0102 f000  ................
-00002d70: 0801 02f0 0008 0102 f000 0801 02f0 0008  ................
-00002d80: 0102 f000 0801 02f0 0008 0102 f000 0801  ................
-00002d90: 02f0 0008 0102 f000 0801 02f0 0008 0102  ................
-00002da0: f000 0801 02f0 0008 0102 f000 0801 02f0  ................
-00002db0: 0008 0102 f000 0801 02f0 1202 0102 f000  ................
-00002dc0: 0201 02f0 0002 0102 f000 0201 02f0 0002  ................
-00002dd0: 0102 f000 0201 02f0 0807 0102 f000 0701  ................
-00002de0: 02f0 0007 0102 f000 0701 02f0 0007 0102  ................
-00002df0: f000 0701 02f0 0007 0102 f000 0701 02f0  ................
-00002e00: 0007 0102 f000 0701 02f0 0007 0102 f000  ................
-00002e10: 0701 02f0 0007 0102 f000 0701 02f0 0007  ................
-00002e20: 0102 f000 0701 02f0 1200 1736 d000 13f0  ...........6....
-00002e30: 0402 0b02 8007 f008 4b03 016b 01f0 004b  ........K..k...K
-00002e40: 0301 6b01 f000 4b03 016b 01f0 004b 0301  ..k...K..k...K..
-00002e50: 6b01 f000 4b03 016b 0190 7df1 004b 0301  k...K..k..}..K..
-00002e60: 6b01 f400 4b03 016b 01f0 004b 0301 6b01  k...K..k...K..k.
-00002e70: f000 4b03 016b 01f0 004b 0301 6b01 7235  ..K..k...K..k.r5
-00002e80: 0000 00                                  ...
+00000000: 6f0d 0d0a 0000 0000 e4dd 4664 3232 0000  o.........Fd22..
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
+00000040: 6404 6c03 6d04 5a04 0100 6403 6405 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6403  m.Z.m.Z.m.Z...d.
+00000060: 6406 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
+00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
+00000080: 0100 6403 6407 6c11 6d12 5a12 0100 6408  ..d.d.l.m.Z...d.
+00000090: 6409 6c13 6d14 5a14 6d15 5a15 6d16 5a16  d.l.m.Z.m.Z.m.Z.
+000000a0: 6d17 5a17 6d18 5a18 6d19 5a19 0100 640a  m.Z.m.Z.m.Z...d.
+000000b0: 5a1a 640b 640c 640d 9c02 5a1b 640e 5a1c  Z.d.d.d...Z.d.Z.
+000000c0: 4700 640f 6410 8400 6410 6502 8303 5a1d  G.d.d...d.e...Z.
+000000d0: 6411 5300 2912 6135 0400 000a 4d49 5420  d.S.).a5....MIT 
+000000e0: 4c69 6365 6e73 650a 0a43 6f70 7972 6967  License..Copyrig
+000000f0: 6874 2028 6329 2032 3032 3320 4b6f 6e72  ht (c) 2023 Konr
+00000100: 6164 2028 406b 6f6e 7261 6473 6963 290a  ad (@konradsic).
+00000110: 0a50 6572 6d69 7373 696f 6e20 6973 2068  .Permission is h
+00000120: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
+00000130: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
+00000140: 6f20 616e 7920 7065 7273 6f6e 206f 6274  o any person obt
+00000150: 6169 6e69 6e67 2061 2063 6f70 790a 6f66  aining a copy.of
+00000160: 2074 6869 7320 736f 6674 7761 7265 2061   this software a
+00000170: 6e64 2061 7373 6f63 6961 7465 6420 646f  nd associated do
+00000180: 6375 6d65 6e74 6174 696f 6e20 6669 6c65  cumentation file
+00000190: 7320 2874 6865 2022 536f 6674 7761 7265  s (the "Software
+000001a0: 2229 2c20 746f 2064 6561 6c0a 696e 2074  "), to deal.in t
+000001b0: 6865 2053 6f66 7477 6172 6520 7769 7468  he Software with
+000001c0: 6f75 7420 7265 7374 7269 6374 696f 6e2c  out restriction,
+000001d0: 2069 6e63 6c75 6469 6e67 2077 6974 686f   including witho
+000001e0: 7574 206c 696d 6974 6174 696f 6e20 7468  ut limitation th
+000001f0: 6520 7269 6768 7473 0a74 6f20 7573 652c  e rights.to use,
+00000200: 2063 6f70 792c 206d 6f64 6966 792c 206d   copy, modify, m
+00000210: 6572 6765 2c20 7075 626c 6973 682c 2064  erge, publish, d
+00000220: 6973 7472 6962 7574 652c 2073 7562 6c69  istribute, subli
+00000230: 6365 6e73 652c 2061 6e64 2f6f 7220 7365  cense, and/or se
+00000240: 6c6c 0a63 6f70 6965 7320 6f66 2074 6865  ll.copies of the
+00000250: 2053 6f66 7477 6172 652c 2061 6e64 2074   Software, and t
+00000260: 6f20 7065 726d 6974 2070 6572 736f 6e73  o permit persons
+00000270: 2074 6f20 7768 6f6d 2074 6865 2053 6f66   to whom the Sof
+00000280: 7477 6172 6520 6973 0a66 7572 6e69 7368  tware is.furnish
+00000290: 6564 2074 6f20 646f 2073 6f2c 2073 7562  ed to do so, sub
+000002a0: 6a65 6374 2074 6f20 7468 6520 666f 6c6c  ject to the foll
+000002b0: 6f77 696e 6720 636f 6e64 6974 696f 6e73  owing conditions
+000002c0: 3a0a 0a54 6865 2061 626f 7665 2063 6f70  :..The above cop
+000002d0: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
+000002e0: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
+000002f0: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
+00000300: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
+00000310: 6c0a 636f 7069 6573 206f 7220 7375 6273  l.copies or subs
+00000320: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
+00000330: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
+00000340: 2e0a 0a54 4845 2053 4f46 5457 4152 4520  ...THE SOFTWARE 
+00000350: 4953 2050 524f 5649 4445 4420 2241 5320  IS PROVIDED "AS 
+00000360: 4953 222c 2057 4954 484f 5554 2057 4152  IS", WITHOUT WAR
+00000370: 5241 4e54 5920 4f46 2041 4e59 204b 494e  RANTY OF ANY KIN
+00000380: 442c 2045 5850 5245 5353 204f 520a 494d  D, EXPRESS OR.IM
+00000390: 504c 4945 442c 2049 4e43 4c55 4449 4e47  PLIED, INCLUDING
+000003a0: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
+000003b0: 2054 4f20 5448 4520 5741 5252 414e 5449   TO THE WARRANTI
+000003c0: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
+000003d0: 494c 4954 592c 0a46 4954 4e45 5353 2046  ILITY,.FITNESS F
+000003e0: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
+000003f0: 5055 5250 4f53 4520 414e 4420 4e4f 4e49  PURPOSE AND NONI
+00000400: 4e46 5249 4e47 454d 454e 542e 2049 4e20  NFRINGEMENT. IN 
+00000410: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
+00000420: 4845 0a41 5554 484f 5253 204f 5220 434f  HE.AUTHORS OR CO
+00000430: 5059 5249 4748 5420 484f 4c44 4552 5320  PYRIGHT HOLDERS 
+00000440: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
+00000450: 5920 434c 4149 4d2c 2044 414d 4147 4553  Y CLAIM, DAMAGES
+00000460: 204f 5220 4f54 4845 520a 4c49 4142 494c   OR OTHER.LIABIL
+00000470: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
+00000480: 414e 2041 4354 494f 4e20 4f46 2043 4f4e  AN ACTION OF CON
+00000490: 5452 4143 542c 2054 4f52 5420 4f52 204f  TRACT, TORT OR O
+000004a0: 5448 4552 5749 5345 2c20 4152 4953 494e  THERWISE, ARISIN
+000004b0: 4720 4652 4f4d 2c0a 4f55 5420 4f46 204f  G FROM,.OUT OF O
+000004c0: 5220 494e 2043 4f4e 4e45 4354 494f 4e20  R IN CONNECTION 
+000004d0: 5749 5448 2054 4845 2053 4f46 5457 4152  WITH THE SOFTWAR
+000004e0: 4520 4f52 2054 4845 2055 5345 204f 5220  E OR THE USE OR 
+000004f0: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
+00000500: 4e20 5448 450a 534f 4654 5741 5245 2e0a  N THE.SOFTWARE..
+00000510: e901 0000 0029 01da 0d42 6173 6541 5049  .....)...BaseAPI
+00000520: 436c 6965 6e74 e902 0000 0029 01da 094c  Client.....)...L
+00000530: 616e 6775 6167 6573 2903 da12 4375 7272  anguages)...Curr
+00000540: 656e 7457 6561 7468 6572 4461 7461 da0c  entWeatherData..
+00000550: 4c6f 6361 7469 6f6e 4461 7461 da0c 466f  LocationData..Fo
+00000560: 7265 6361 7374 4461 7461 2907 da13 5765  recastData)...We
+00000570: 6174 6865 7241 5049 4578 6365 7074 696f  atherAPIExceptio
+00000580: 6eda 0f4e 6f4c 6f63 6174 696f 6e46 6f75  n..NoLocationFou
+00000590: 6e64 da0d 496e 7661 6c69 6441 5049 4b65  nd..InvalidAPIKe
+000005a0: 79da 1041 5049 4c69 6d69 7445 7863 6565  y..APILimitExcee
+000005b0: 6465 64da 0e41 5049 4b65 7944 6973 6162  ded..APIKeyDisab
+000005c0: 6c65 64da 0c41 6363 6573 7344 656e 6965  led..AccessDenie
+000005d0: 64da 1849 6e74 6572 6e61 6c41 7070 6c69  d..InternalAppli
+000005e0: 6361 7469 6f6e 4572 726f 7229 01da 0575  cationError)...u
+000005f0: 7469 6c73 e900 0000 0029 06da 0341 6e79  tils.....)...Any
+00000600: da07 4c69 7465 7261 6cda 0444 6963 74da  ..Literal..Dict.
+00000610: 084f 7074 696f 6e61 6cda 0555 6e69 6f6e  .Optional..Union
+00000620: da04 4c69 7374 7a1d 6874 7470 3a2f 2f61  ..Listz.http://a
+00000630: 7069 2e77 6561 7468 6572 6170 692e 636f  pi.weatherapi.co
+00000640: 6d2f 7631 2fda 0379 6573 da02 6e6f 2902  m/v1/..yes..no).
+00000650: 5446 2901 da06 436c 6965 6e74 6300 0000  TF)...Clientc...
+00000660: 0000 0000 0000 0000 0000 0000 0013 0000  ................
+00000670: 0000 0000 0073 5c01 0000 6500 5a01 6400  .....s\...e.Z.d.
+00000680: 5a02 6401 5a03 0902 0902 0902 0902 0903  Z.d.Z...........
+00000690: 0903 6423 6404 6504 6405 6505 6506 6504  ..d#d.e.d.e.e.e.
+000006a0: 6507 6602 1900 1900 6406 6505 6508 1900  e.f.....d.e.e...
+000006b0: 6407 6505 6508 1900 6408 6505 6508 1900  d.e.e...d.e.e...
+000006c0: 6409 6509 640a 6509 640b 650a 6504 650b  d.e.d.e.d.e.e.e.
+000006d0: 6602 1900 640c 6402 6612 8700 6601 640d  f...d.d.f...f.d.
+000006e0: 640e 840d 5a0c 640f 6504 6410 650a 6504  d...Z.d.e.d.e.e.
+000006f0: 650b 6602 1900 640c 650a 6504 650b 6602  e.f...d.e.e.e.f.
+00000700: 1900 6606 6411 6412 8404 5a0d 6405 6506  ..f.d.d...Z.d.e.
+00000710: 6504 6507 6602 1900 640c 6505 6507 1900  e.e.f...d.e.e...
+00000720: 6604 6413 6414 8404 5a0e 6402 6402 6415  f.d.d...Z.d.d.d.
+00000730: 9c02 6416 6504 6405 6505 6506 6504 6507  ..d.e.d.e.e.e.e.
+00000740: 6602 1900 1900 6409 6505 6509 1900 640b  f.....d.e.e...d.
+00000750: 650a 6504 650b 6602 1900 640c 650f 660a  e.e.e.f...d.e.f.
+00000760: 6417 6418 8406 5a10 6416 6504 6602 6419  d.d...Z.d.e.f.d.
+00000770: 641a 8404 5a11 6402 6402 6402 641b 9c03  d...Z.d.d.d.d...
+00000780: 6416 6504 6409 6505 6509 1900 641c 6505  d.e.d.e.e...d.e.
+00000790: 6509 1900 6405 6505 6506 6504 6507 6602  e...d.e.e.e.e.f.
+000007a0: 1900 1900 640b 650a 6504 650b 6602 1900  ....d.e.e.e.f...
+000007b0: 640c 6512 660c 641d 641e 8406 5a13 641f  d.e.f.d.d...Z.d.
+000007c0: 6420 8400 5a14 6421 6422 8400 5a15 8700  d ..Z.d!d"..Z...
+000007d0: 0400 5a16 5300 2924 7219 0000 0061 a508  ..Z.S.)$r....a..
+000007e0: 0000 0a20 2020 2041 2057 6561 7468 6572  ...    A Weather
+000007f0: 4150 492e 636f 6d20 636c 6965 6e74 2066  API.com client f
+00000800: 6f72 2066 6574 6368 696e 6720 7661 7269  or fetching vari
+00000810: 6f75 7320 7765 6174 6865 7220 696e 666f  ous weather info
+00000820: 726d 6174 696f 6e0a 0a20 2020 2050 6172  rmation..    Par
+00000830: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00000840: 2d2d 2d2d 2d2d 0a20 2020 2061 7069 5f6b  ------.    api_k
+00000850: 6579 3a20 3a63 6c61 7373 3a60 7374 7260  ey: :class:`str`
+00000860: 0a20 2020 2020 2020 2041 5049 204b 6579  .        API Key
+00000870: 2075 7365 6420 746f 2061 7574 6865 6e74   used to authent
+00000880: 6963 6174 6520 7768 656e 2073 656e 6469  icate when sendi
+00000890: 6e67 2072 6571 7565 7374 730a 2020 2020  ng requests.    
+000008a0: 6c61 6e67 3a20 4f70 7469 6f6e 616c 5b20  lang: Optional[ 
+000008b0: 556e 696f 6e5b 3a63 6c61 7373 3a60 7374  Union[:class:`st
+000008c0: 7260 2c20 3a63 6c61 7373 3a60 4c61 6e67  r`, :class:`Lang
+000008d0: 7561 6765 7360 5d20 5d0a 2020 2020 2020  uages`] ].      
+000008e0: 2020 4c61 6e67 7561 6765 2066 726f 6d20    Language from 
+000008f0: 7468 6520 3a63 6c61 7373 3a60 4c61 6e67  the :class:`Lang
+00000900: 7561 6765 7360 2065 6e75 6d20 6f72 2061  uages` enum or a
+00000910: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+00000920: 7469 6e67 2074 6865 206c 616e 6775 6167  ting the languag
+00000930: 6520 6f72 206c 616e 6775 6167 6520 636f  e or language co
+00000940: 6465 2028 7072 6566 6572 6162 6c79 292e  de (preferably).
+00000950: 0a20 2020 2020 2020 2054 6f20 6765 7420  .        To get 
+00000960: 6120 6c69 7374 206f 6620 6c61 6e67 7561  a list of langua
+00000970: 6765 7320 7669 7369 7420 3a63 6c61 7373  ges visit :class
+00000980: 3a60 4c61 6e67 7561 6765 7360 2e20 4966  :`Languages`. If
+00000990: 2060 604e 6f6e 6560 6020 7468 656e 2074   ``None`` then t
+000009a0: 6865 2064 6566 6175 6c74 206c 616e 6775  he default langu
+000009b0: 6167 6520 6973 2075 7365 6420 2845 6e67  age is used (Eng
+000009c0: 6c69 7368 290a 2020 2020 6474 3a20 4f70  lish).    dt: Op
+000009d0: 7469 6f6e 616c 5b3a 636c 6173 733a 6069  tional[:class:`i
+000009e0: 6e74 605d 0a20 2020 2020 2020 2052 6573  nt`].        Res
+000009f0: 7472 6963 7420 6461 7465 206f 7574 7075  trict date outpu
+00000a00: 7420 666f 7220 466f 7265 6361 7374 2061  t for Forecast a
+00000a10: 6e64 2048 6973 746f 7279 2041 5049 206d  nd History API m
+00000a20: 6574 686f 642e 2028 5265 7175 6972 6564  ethod. (Required
+00000a30: 2066 6f72 2048 6973 746f 7279 2061 6e64   for History and
+00000a40: 2046 7574 7572 6520 4150 4929 0a20 2020   Future API).   
+00000a50: 2065 6e64 5f64 743a 204f 7074 696f 6e61   end_dt: Optiona
+00000a60: 6c5b 3a63 6c61 7373 3a60 696e 7460 5d0a  l[:class:`int`].
+00000a70: 2020 2020 2020 2020 5265 7374 7269 6374          Restrict
+00000a80: 2064 6174 6520 6f75 7470 7574 2066 6f72   date output for
+00000a90: 2048 6973 746f 7279 2041 5049 206d 6574   History API met
+00000aa0: 686f 642e 204f 6e6c 7920 776f 726b 7320  hod. Only works 
+00000ab0: 666f 7220 4150 4920 6f6e 2050 726f 2070  for API on Pro p
+00000ac0: 6c61 6e20 616e 6420 6162 6f76 652e 2028  lan and above. (
+00000ad0: 4176 6169 6c61 626c 6520 666f 7220 4869  Available for Hi
+00000ae0: 7374 6f72 7920 4150 4929 0a20 2020 2068  story API).    h
+00000af0: 6f75 723a 204f 7074 696f 6e61 6c5b 3a63  our: Optional[:c
+00000b00: 6c61 7373 3a60 696e 7460 5d0a 2020 2020  lass:`int`].    
+00000b10: 2020 2020 5265 7374 7269 6374 696e 6720      Restricting 
+00000b20: 666f 7265 6361 7374 206f 7220 6869 7374  forecast or hist
+00000b30: 6f72 7920 6f75 7470 7574 2074 6f20 6120  ory output to a 
+00000b40: 7370 6563 6966 6963 2068 6f75 7220 696e  specific hour in
+00000b50: 2061 2067 6976 656e 2064 6179 2e0a 2020   a given day..  
+00000b60: 2020 6171 693a 203a 636c 6173 733a 6062    aqi: :class:`b
+00000b70: 6f6f 6c60 0a20 2020 2020 2020 2045 6e61  ool`.        Ena
+00000b80: 626c 652f 4469 7361 626c 6520 4169 7220  ble/Disable Air 
+00000b90: 5175 616c 6974 7920 6461 7461 2069 6e20  Quality data in 
+00000ba0: 666f 7265 6361 7374 2041 5049 206f 7574  forecast API out
+00000bb0: 7075 742e 2044 6566 6175 6c74 7320 746f  put. Defaults to
+00000bc0: 2022 6e6f 222e 0a20 2020 2074 6964 6573   "no"..    tides
+00000bd0: 3a20 3a63 6c61 7373 3a60 626f 6f6c 600a  : :class:`bool`.
+00000be0: 2020 2020 2020 2020 456e 6162 6c65 2f44          Enable/D
+00000bf0: 6973 6162 6c65 2054 6964 6520 6461 7461  isable Tide data
+00000c00: 2069 6e20 4d61 7269 6e65 2041 5049 206f   in Marine API o
+00000c10: 7574 7075 742e 2044 6566 6175 6c74 7320  utput. Defaults 
+00000c20: 746f 2022 6e6f 222e 0a20 2020 206b 7761  to "no"..    kwa
+00000c30: 7267 733a 2044 6963 745b 3a63 6c61 7373  rgs: Dict[:class
+00000c40: 3a60 7374 7260 2c20 416e 795d 0a20 2020  :`str`, Any].   
+00000c50: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+00000c60: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00000c70: 7320 7061 7373 6564 2062 7920 6465 6661  s passed by defa
+00000c80: 756c 7420 746f 2072 6571 7565 7374 7320  ult to requests 
+00000c90: 6d61 6465 2062 7920 7468 6520 636c 6965  made by the clie
+00000ca0: 6e74 0a20 2020 2020 2020 200a 2020 2020  nt.        .    
+00000cb0: 4174 7472 6962 7574 6573 0a20 2020 202d  Attributes.    -
+00000cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00000cd0: 206c 616e 673a 204f 7074 696f 6e61 6c5b   lang: Optional[
+00000ce0: 3a63 6c61 7373 3a60 4c61 6e67 7561 6765  :class:`Language
+00000cf0: 7360 5d0a 2020 2020 2020 2020 4c61 6e67  s`].        Lang
+00000d00: 7561 6765 2066 726f 6d20 7468 6520 3a63  uage from the :c
+00000d10: 6c61 7373 3a60 4c61 6e67 7561 6765 7360  lass:`Languages`
+00000d20: 2065 6e75 6d20 6f72 2061 2073 7472 696e   enum or a strin
+00000d30: 6720 7265 7072 6573 656e 7469 6e67 2074  g representing t
+00000d40: 6865 206c 616e 6775 6167 6520 6f72 206c  he language or l
+00000d50: 616e 6775 6167 6520 636f 6465 2028 7072  anguage code (pr
+00000d60: 6566 6572 6162 6c79 292e 0a20 2020 2020  eferably)..     
+00000d70: 2020 2054 6f20 6765 7420 6120 6c69 7374     To get a list
+00000d80: 206f 6620 6c61 6e67 7561 6765 7320 7669   of languages vi
+00000d90: 7369 7420 3a63 6c61 7373 3a60 4c61 6e67  sit :class:`Lang
+00000da0: 7561 6765 7360 2e20 4966 2060 604e 6f6e  uages`. If ``Non
+00000db0: 6560 6020 7468 656e 2074 6865 2064 6566  e`` then the def
+00000dc0: 6175 6c74 206c 616e 6775 6167 6520 6973  ault language is
+00000dd0: 2075 7365 6420 2845 6e67 6c69 7368 290a   used (English).
+00000de0: 2020 2020 6474 3a20 4f70 7469 6f6e 616c      dt: Optional
+00000df0: 5b3a 636c 6173 733a 6069 6e74 605d 0a20  [:class:`int`]. 
+00000e00: 2020 2020 2020 2052 6573 7472 6963 7465         Restricte
+00000e10: 6420 6461 7465 206f 7574 7075 7420 666f  d date output fo
+00000e20: 7220 466f 7265 6361 7374 2061 6e64 2048  r Forecast and H
+00000e30: 6973 746f 7279 2041 5049 206d 6574 686f  istory API metho
+00000e40: 642e 2028 5265 7175 6972 6564 2066 6f72  d. (Required for
+00000e50: 2048 6973 746f 7279 2061 6e64 2046 7574   History and Fut
+00000e60: 7572 6520 4150 4929 0a20 2020 2065 6e64  ure API).    end
+00000e70: 5f64 743a 204f 7074 696f 6e61 6c5b 3a63  _dt: Optional[:c
+00000e80: 6c61 7373 3a60 696e 7460 5d0a 2020 2020  lass:`int`].    
+00000e90: 2020 2020 5265 7374 7269 6374 6564 2064      Restricted d
+00000ea0: 6174 6520 6f75 7470 7574 2066 6f72 2048  ate output for H
+00000eb0: 6973 746f 7279 2041 5049 206d 6574 686f  istory API metho
+00000ec0: 642e 204f 6e6c 7920 776f 726b 7320 666f  d. Only works fo
+00000ed0: 7220 4150 4920 6f6e 2050 726f 2070 6c61  r API on Pro pla
+00000ee0: 6e20 616e 6420 6162 6f76 652e 0a20 2020  n and above..   
+00000ef0: 2068 6f75 723a 204f 7074 696f 6e61 6c5b   hour: Optional[
+00000f00: 3a63 6c61 7373 3a60 696e 7460 5d0a 2020  :class:`int`].  
+00000f10: 2020 2020 2020 5265 7374 7269 6374 6564        Restricted
+00000f20: 2066 6f72 6563 6173 7420 6f72 2068 6973   forecast or his
+00000f30: 746f 7279 206f 7574 7075 7420 746f 2061  tory output to a
+00000f40: 2073 7065 6369 6669 6320 686f 7572 2069   specific hour i
+00000f50: 6e20 6120 6769 7665 6e20 6461 792e 0a20  n a given day.. 
+00000f60: 2020 2061 7169 3a20 3a63 6c61 7373 3a60     aqi: :class:`
+00000f70: 626f 6f6c 600a 2020 2020 2020 2020 496e  bool`.        In
+00000f80: 6469 6361 7465 7320 6966 2041 6972 2051  dicates if Air Q
+00000f90: 7561 6c69 7479 2064 6174 6120 6861 7320  uality data has 
+00000fa0: 6265 656e 2065 6e61 626c 6564 0a20 2020  been enabled.   
+00000fb0: 2074 6964 6573 3a20 3a63 6c61 7373 3a60   tides: :class:`
+00000fc0: 626f 6f6c 600a 2020 2020 2020 2020 496e  bool`.        In
+00000fd0: 6469 6361 7465 7320 6966 2074 6964 6573  dicates if tides
+00000fe0: 2064 6174 6120 696e 2074 6865 204d 6172   data in the Mar
+00000ff0: 696e 6520 4150 4920 6861 7320 6265 656e  ine API has been
+00001000: 2065 6e61 626c 6564 0a20 2020 206b 7761   enabled.    kwa
+00001010: 7267 733a 2044 6963 745b 3a63 6c61 7373  rgs: Dict[:class
+00001020: 3a60 7374 7260 2c20 416e 795d 0a20 2020  :`str`, Any].   
+00001030: 2020 2020 2041 6464 6974 696f 6e61 6c20       Additional 
+00001040: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00001050: 7320 7061 7373 6564 2062 7920 6465 6661  s passed by defa
+00001060: 756c 7420 746f 2072 6571 7565 7374 7320  ult to requests 
+00001070: 6d61 6465 2062 7920 7468 6520 636c 6965  made by the clie
+00001080: 6e74 0a20 2020 204e 46da 0761 7069 5f6b  nt.    NF..api_k
+00001090: 6579 da04 6c61 6e67 da02 6474 da06 656e  ey..lang..dt..en
+000010a0: 645f 6474 da04 686f 7572 da03 6171 69da  d_dt..hour..aqi.
+000010b0: 0574 6964 6573 da06 6b77 6172 6773 da06  .tides..kwargs..
+000010c0: 7265 7475 726e 6308 0000 0000 0000 0000  returnc.........
+000010d0: 0000 000b 0000 0004 0000 000b 0000 0073  ...............s
+000010e0: 9400 0000 6400 7d09 7c02 6400 7501 720d  ....d.}.|.d.u.r.
+000010f0: 7400 6a01 7c02 6401 6402 8d02 7d09 6403  t.j.|.d.d...}.d.
+00001100: 7c01 6901 7c08 a501 7d0a 7c09 7222 7c0a  |.i.|...}.|.r"|.
+00001110: 6a02 7c09 6400 7501 721e 7c09 6a03 6e01  j.|.d.u.r.|.j.n.
+00001120: 6400 6404 8d01 0100 7404 8300 6a05 7406  d.d.....t...j.t.
+00001130: 7c0a 6405 8d02 0100 7c03 7c00 5f07 7c04  |.d.....|.|._.|.
+00001140: 7c00 5f08 7c05 7c00 5f09 7c06 7c00 5f0a  |._.|.|._.|.|._.
+00001150: 7c07 7c00 5f0b 7c08 7c00 5f0c 7c09 7245  |.|._.|.|._.|.rE
+00001160: 740d 7c09 8301 7c00 5f0e 6400 5300 6400  t.|...|._.d.S.d.
+00001170: 7c00 5f0e 6400 5300 2906 4e54 a901 da05  |._.d.S.).NT....
+00001180: 6173 6f62 6ada 036b 6579 2901 721b 0000  asobj..key).r...
+00001190: 0029 02da 0862 6173 655f 7572 6cda 0f64  .)...base_url..d
+000011a0: 6566 6175 6c74 5f6f 7074 696f 6e73 290f  efault_options).
+000011b0: 720f 0000 00da 0d66 696e 645f 6c61 6e67  r......find_lang
+000011c0: 7561 6765 da06 7570 6461 7465 da05 7661  uage..update..va
+000011d0: 6c75 65da 0573 7570 6572 da08 5f5f 696e  lue..super..__in
+000011e0: 6974 5f5f da13 5745 4154 4845 5241 5049  it__..WEATHERAPI
+000011f0: 5f42 4153 455f 5552 4c72 1c00 0000 721d  _BASE_URLr....r.
+00001200: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00001210: 0000 7221 0000 0072 0400 0000 721b 0000  ..r!...r....r...
+00001220: 0029 0bda 0473 656c 6672 1a00 0000 721b  .)...selfr....r.
+00001230: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00001240: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
+00001250: 00da 096c 616e 675f 636f 6465 da04 6f70  ...lang_code..op
+00001260: 7473 a901 da09 5f5f 636c 6173 735f 5fa9  ts....__class__.
+00001270: 00fa 3462 7569 6c64 2f62 6469 7374 2e6c  ..4build/bdist.l
+00001280: 696e 7578 2d78 3836 5f36 342f 6567 672f  inux-x86_64/egg/
+00001290: 7765 6174 6865 726c 792f 6170 692f 636c  weatherly/api/cl
+000012a0: 6965 6e74 2e70 7972 2c00 0000 6700 0000  ient.pyr,...g...
+000012b0: 7324 0000 0004 0b08 010e 0104 0202 ff02  s$..............
+000012c0: 0204 fe1e 0408 0202 0106 ff06 0306 0106  ................
+000012d0: 0106 0106 0106 011c 017a 0f43 6c69 656e  .........z.Clien
+000012e0: 742e 5f5f 696e 6974 5f5f da08 656e 6470  t.__init__..endp
+000012f0: 6f69 6e74 da07 6f70 7469 6f6e 7363 0300  oint..optionsc..
+00001300: 0000 0000 0000 0000 0000 0b00 0000 0500  ................
+00001310: 0000 4300 0000 7322 0100 007c 006a 00a0  ..C...s"...|.j..
+00001320: 01a1 007d 037c 03a0 02a1 0044 005d 0b5c  ...}.|.....D.].\
+00001330: 027d 047d 057c 0564 0175 0072 147c 037c  .}.}.|.d.u.r.|.|
+00001340: 043d 0071 097c 02a0 02a1 0044 005d 105c  .=.q.|.....D.].\
+00001350: 027d 047d 057c 0564 0175 0172 2974 03a0  .}.}.|.d.u.r)t..
+00001360: 047c 057c 05a1 027c 037c 043c 0071 197c  .|.|...|.|.<.q.|
+00001370: 006a 057c 0166 0169 007c 03a4 018e 017d  .j.|.f.i.|.....}
+00001380: 067c 0664 0219 006a 0664 036b 0073 8f7c  .|.d...j.d.k.s.|
+00001390: 0664 0419 0064 0519 007d 077c 0764 0619  .d...d...}.|.d..
+000013a0: 007d 087c 0664 0219 006a 067d 097c 0764  .}.|.d...j.}.|.d
+000013b0: 0719 007d 0a7c 0864 086b 0272 5774 077c  ...}.|.d.k.rWt.|
+000013c0: 097c 087c 0a83 0382 017c 0864 096b 0272  .|.|.....|.d.k.r
+000013d0: 6174 087c 097c 087c 0a83 0382 017c 0864  at.|.|.|.....|.d
+000013e0: 0a6b 0272 6b74 097c 097c 087c 0a83 0382  .k.rkt.|.|.|....
+000013f0: 017c 0864 0b6b 0272 7574 0a7c 097c 087c  .|.d.k.rut.|.|.|
+00001400: 0a83 0382 017c 0864 0c6b 0272 7f74 0b7c  .....|.d.k.r.t.|
+00001410: 097c 087c 0a83 0382 017c 0864 0d6b 0272  .|.|.....|.d.k.r
+00001420: 8974 0c7c 097c 087c 0a83 0382 0174 0d7c  .t.|.|.|.....t.|
+00001430: 097c 087c 0a83 0382 017c 0653 0029 0e7a  .|.|.....|.S.).z
+00001440: 3250 7269 7661 7465 206d 6574 686f 6420  2Private method 
+00001450: 7573 6564 2074 6f20 6d61 6b65 2072 6571  used to make req
+00001460: 7565 7374 7320 746f 2057 6561 7468 6572  uests to Weather
+00001470: 4150 494e 7201 0000 0069 9001 0000 7210  APINr....i....r.
+00001480: 0000 00da 0565 7272 6f72 da04 636f 6465  .....error..code
+00001490: da07 6d65 7373 6167 6569 ee03 0000 69d6  ..messagei....i.
+000014a0: 0700 0069 d707 0000 69d8 0700 0069 d907  ...i....i....i..
+000014b0: 0000 690f 2700 0029 0e72 2700 0000 da04  ..i.'..).r'.....
+000014c0: 636f 7079 da05 6974 656d 73da 0c42 4f4f  copy..items..BOO
+000014d0: 4c5f 5245 504c 4143 45da 0367 6574 da08  L_REPLACE..get..
+000014e0: 5f72 6571 7565 7374 da0b 7374 6174 7573  _request..status
+000014f0: 5f63 6f64 6572 0900 0000 720a 0000 0072  _coder....r....r
+00001500: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
+00001510: 0000 0072 0800 0000 290b 722e 0000 0072  ...r....).r....r
+00001520: 3500 0000 7236 0000 00da 0d66 696e 616c  5...r6.....final
+00001530: 5f6f 7074 696f 6e73 da01 6bda 0176 da04  _options..k..v..
+00001540: 7265 7370 da0a 6572 726f 725f 6461 7461  resp..error_data
+00001550: 7238 0000 00da 0673 7461 7475 73da 036d  r8.....status..m
+00001560: 7367 7233 0000 0072 3300 0000 7234 0000  sgr3...r3...r4..
+00001570: 00da 0d5f 6361 6c6c 5f72 6571 7565 7374  ..._call_request
+00001580: 8700 0000 732a 0000 000a 0210 020e 0102  ....s*..........
+00001590: 8010 0218 0202 8012 020e 020c 0208 010a  ................
+000015a0: 0108 0114 0214 0114 0114 0114 0114 010c  ................
+000015b0: 0104 027a 1443 6c69 656e 742e 5f63 616c  ...z.Client._cal
+000015c0: 6c5f 7265 7175 6573 7463 0200 0000 0000  l_requestc......
+000015d0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+000015e0: 0000 7322 0000 0074 006a 017c 0164 0164  ..s"...t.j.|.d.d
+000015f0: 028d 027d 027c 0273 0b64 0353 007c 027c  ...}.|.s.d.S.|.|
+00001600: 005f 027c 006a 0253 0029 0461 f601 0000  ._.|.j.S.).a....
+00001610: 0a20 2020 2020 2020 2053 6574 2063 6c69  .        Set cli
+00001620: 656e 7427 7320 6c61 6e67 7561 6765 2077  ent's language w
+00001630: 6865 6e20 7265 7175 6573 7469 6e67 2064  hen requesting d
+00001640: 6174 612e 0a20 2020 2020 2020 200a 2020  ata..        .  
+00001650: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00001660: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001670: 2d2d 2d2d 0a20 2020 2020 2020 206c 616e  ----.        lan
+00001680: 673a 2055 6e69 6f6e 5b3a 636c 6173 733a  g: Union[:class:
+00001690: 6073 7472 602c 203a 636c 6173 733a 604c  `str`, :class:`L
+000016a0: 616e 6775 6167 6573 605d 0a20 2020 2020  anguages`].     
+000016b0: 2020 2020 2020 204c 616e 6775 6167 6520         Language 
+000016c0: 746f 2073 6574 2e20 4361 6e20 6265 2065  to set. Can be e
+000016d0: 6974 6865 7220 6120 7374 7269 6e67 2074  ither a string t
+000016e0: 6861 7420 6973 206c 616e 7561 6765 2773  hat is lanuage's
+000016f0: 206e 616d 6520 6f72 2063 6f64 6520 6f72   name or code or
+00001700: 2061 203a 636c 6173 733a 604c 616e 6775   a :class:`Langu
+00001710: 6167 6573 6020 656e 756d 206f 626a 6563  ages` enum objec
+00001720: 742e 0a20 2020 2020 2020 2020 2020 200a  t..            .
+00001730: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00001740: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00001750: 2d0a 2020 2020 2020 2020 4f70 7469 6f6e  -.        Option
+00001760: 616c 5b3a 636c 6173 733a 604c 616e 6775  al[:class:`Langu
+00001770: 6167 6573 605d 0a20 2020 2020 2020 2020  ages`].         
+00001780: 2020 2041 6e20 656e 756d 2063 6c61 7373     An enum class
+00001790: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+000017a0: 6520 6c61 6e67 7561 6765 206f 6620 7468  e language of th
+000017b0: 6520 636c 6965 6e74 2e20 4973 2060 604e  e client. Is ``N
+000017c0: 6f6e 6560 6020 7768 656e 2073 6f6d 6574  one`` when somet
+000017d0: 6869 6e67 2077 656e 7420 7772 6f6e 6720  hing went wrong 
+000017e0: 616e 6420 7468 6520 6c61 6e67 7561 6765  and the language
+000017f0: 2077 6173 206e 6f74 2073 6574 2e0a 2020   was not set..  
+00001800: 2020 2020 2020 5472 2300 0000 4e29 0372        Tr#...N).r
+00001810: 0f00 0000 7228 0000 0072 1b00 0000 2903  ....r(...r....).
+00001820: 722e 0000 0072 1b00 0000 da0a 6c61 6e67  r....r......lang
+00001830: 5f63 6c61 7373 7233 0000 0072 3300 0000  _classr3...r3...
+00001840: 7234 0000 00da 0c73 6574 5f6c 616e 6775  r4.....set_langu
+00001850: 6167 65a5 0000 0073 0a00 0000 0e0e 0401  age....s........
+00001860: 0401 0602 0601 7a13 436c 6965 6e74 2e73  ......z.Client.s
+00001870: 6574 5f6c 616e 6775 6167 6529 0272 1b00  et_language).r..
+00001880: 0000 721f 0000 00da 0571 7565 7279 6302  ..r......queryc.
+00001890: 0000 0000 0000 0002 0000 0008 0000 0004  ................
+000018a0: 0000 004b 0000 0073 4a00 0000 7c03 7004  ...K...sJ...|.p.
+000018b0: 7c00 6a00 7c01 6401 9c02 7c04 a501 7d05  |.j.|.d...|...}.
+000018c0: 7c02 6402 7501 7212 7c02 7c05 6403 3c00  |.d.u.r.|.|.d.<.
+000018d0: 7c00 a001 6404 7c05 a102 7d06 7402 7c06  |...d.|...}.t.|.
+000018e0: 6405 1900 7c06 6406 1900 6a03 6402 8303  d...|.d...j.d...
+000018f0: 7d07 7c07 5300 2907 61d2 0500 000a 2020  }.|.S.).a.....  
+00001900: 2020 2020 2020 4765 7420 6375 7272 656e        Get curren
+00001910: 7420 7765 6174 6865 7220 6461 7461 0a0a  t weather data..
+00001920: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00001930: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00001940: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7175  -----.        qu
+00001950: 6572 793a 203a 636c 6173 733a 6073 7472  ery: :class:`str
+00001960: 600a 2020 2020 2020 2020 2020 2020 5175  `.            Qu
+00001970: 6572 7920 7374 7269 6e67 202d 206c 6f63  ery string - loc
+00001980: 6174 696f 6e20 796f 7520 7761 6e74 2074  ation you want t
+00001990: 6f20 6765 7420 7765 6174 6865 7220 6461  o get weather da
+000019a0: 7461 2066 6f72 0a20 2020 2020 2020 206c  ta for.        l
+000019b0: 616e 673a 204f 7074 696f 6e61 6c5b 556e  ang: Optional[Un
+000019c0: 696f 6e5b 3a63 6c61 7373 3a60 7374 7260  ion[:class:`str`
+000019d0: 2c20 4c61 6e67 7561 6765 735d 5d0a 2020  , Languages]].  
+000019e0: 2020 2020 2020 2020 2020 4c61 6e67 7561            Langua
+000019f0: 6765 2066 726f 6d20 7468 6520 3a63 6c61  ge from the :cla
+00001a00: 7373 3a60 4c61 6e67 7561 6765 7360 2065  ss:`Languages` e
+00001a10: 6e75 6d20 6f72 2061 2073 7472 696e 6720  num or a string 
+00001a20: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
+00001a30: 206c 616e 6775 6167 6520 6f72 206c 616e   language or lan
+00001a40: 6775 6167 6520 636f 6465 2028 7072 6566  guage code (pref
+00001a50: 6572 6162 6c79 292e 0a20 2020 2020 2020  erably)..       
+00001a60: 2020 2020 2054 6f20 6765 7420 6120 6c69       To get a li
+00001a70: 7374 206f 6620 6c61 6e67 7561 6765 7320  st of languages 
+00001a80: 7669 7369 7420 3a63 6c61 7373 3a60 4c61  visit :class:`La
+00001a90: 6e67 7561 6765 7360 2e0a 2020 2020 2020  nguages`..      
+00001aa0: 2020 6171 693a 204f 7074 696f 6e61 6c5b    aqi: Optional[
+00001ab0: 3a63 6c61 7373 3a60 626f 6f6c 605d 0a20  :class:`bool`]. 
+00001ac0: 2020 2020 2020 2020 2020 2045 6e61 626c             Enabl
+00001ad0: 652f 4469 7361 626c 6520 4169 7220 5175  e/Disable Air Qu
+00001ae0: 616c 6974 7920 6461 7461 2069 6e20 666f  ality data in fo
+00001af0: 7265 6361 7374 2041 5049 206f 7574 7075  recast API outpu
+00001b00: 742e 2049 6620 6e6f 7468 696e 6720 6973  t. If nothing is
+00001b10: 2070 6173 7365 642c 2074 6865 6e20 6974   passed, then it
+00001b20: 2064 6566 6175 6c74 7320 746f 2063 6c69   defaults to cli
+00001b30: 656e 7420 6465 6661 756c 7420 7661 6c75  ent default valu
+00001b40: 652e 0a20 2020 2020 2020 206b 7761 7267  e..        kwarg
+00001b50: 733a 2044 6963 745b 3a63 6c61 7373 3a60  s: Dict[:class:`
+00001b60: 7374 7260 2c20 416e 795d 0a20 2020 2020  str`, Any].     
+00001b70: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
+00001b80: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
+00001b90: 6e74 7320 746f 2072 6571 7565 7374 0a0a  nts to request..
+00001ba0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00001bb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00001bc0: 2020 2020 2020 2020 3a63 6c61 7373 3a60          :class:`
+00001bd0: 4375 7272 656e 7457 6561 7468 6572 4461  CurrentWeatherDa
+00001be0: 7461 600a 2020 2020 2020 2020 2020 2020  ta`.            
+00001bf0: 4375 7272 656e 7420 7765 6174 6865 7220  Current weather 
+00001c00: 6461 7461 2063 6c61 7373 0a0a 2020 2020  data class..    
+00001c10: 2020 2020 5261 6973 6573 0a20 2020 2020      Raises.     
+00001c20: 2020 202d 2d2d 2d2d 2d2d 2d2d 0a20 2020     ---------.   
+00001c30: 2020 2020 203a 6578 633a 604e 6f4c 6f63       :exc:`NoLoc
+00001c40: 6174 696f 6e46 6f75 6e64 600a 2020 2020  ationFound`.    
+00001c50: 2020 2020 2020 2020 5261 6973 6564 2077          Raised w
+00001c60: 6865 6e20 6e6f 206c 6f63 6174 696f 6e20  hen no location 
+00001c70: 666f 7220 6769 7665 6e20 7175 6572 7920  for given query 
+00001c80: 7761 7320 666f 756e 640a 2020 2020 2020  was found.      
+00001c90: 2020 3a65 7863 3a60 496e 7661 6c69 6441    :exc:`InvalidA
+00001ca0: 5049 4b65 7960 0a20 2020 2020 2020 2020  PIKey`.         
+00001cb0: 2020 2052 6169 7365 6420 7768 656e 2074     Raised when t
+00001cc0: 6865 2041 5049 206b 6579 2069 7320 696e  he API key is in
+00001cd0: 7661 6c69 640a 2020 2020 2020 2020 3a65  valid.        :e
+00001ce0: 7863 3a60 4150 494c 696d 6974 4578 6365  xc:`APILimitExce
+00001cf0: 6564 6564 600a 2020 2020 2020 2020 2020  eded`.          
+00001d00: 2020 5261 6973 6564 2077 6865 6e20 4150    Raised when AP
+00001d10: 4920 6b65 7920 6361 6c6c 7320 6c69 6d69  I key calls limi
+00001d20: 7420 7761 7320 6578 6365 6564 6564 0a20  t was exceeded. 
+00001d30: 2020 2020 2020 203a 6578 633a 6041 5049         :exc:`API
+00001d40: 4b65 7944 6973 6162 6c65 6460 0a20 2020  KeyDisabled`.   
+00001d50: 2020 2020 2020 2020 2052 6169 7365 6420           Raised 
+00001d60: 7768 656e 2041 5049 206b 6579 2069 7320  when API key is 
+00001d70: 6469 7361 626c 6564 0a20 2020 2020 2020  disabled.       
+00001d80: 203a 6578 633a 6041 6363 6573 7344 656e   :exc:`AccessDen
+00001d90: 6965 6460 0a20 2020 2020 2020 2020 2020  ied`.           
+00001da0: 2052 6169 7365 6420 7768 656e 2061 6363   Raised when acc
+00001db0: 6573 7320 746f 2067 6976 656e 2072 6573  ess to given res
+00001dc0: 6f75 7263 6520 7761 7320 6465 6e69 6564  ource was denied
+00001dd0: 0a20 2020 2020 2020 203a 6578 633a 6049  .        :exc:`I
+00001de0: 6e74 6572 6e61 6c41 7070 6c69 6361 7469  nternalApplicati
+00001df0: 6f6e 4572 726f 7260 0a20 2020 2020 2020  onError`.       
+00001e00: 2020 2020 2052 6169 7365 6420 7768 656e       Raised when
+00001e10: 2074 6865 7265 2077 6173 2061 2076 6572   there was a ver
+00001e20: 7920 7261 7265 2069 6e74 6572 6e61 6c20  y rare internal 
+00001e30: 6170 706c 6963 6174 696f 6e20 6572 726f  application erro
+00001e40: 720a 2020 2020 2020 2020 3a65 7863 3a60  r.        :exc:`
+00001e50: 5765 6174 6865 7241 5049 4578 6365 7074  WeatherAPIExcept
+00001e60: 696f 6e60 0a20 2020 2020 2020 2020 2020  ion`.           
+00001e70: 2052 6169 7365 6420 7768 656e 2073 6f6d   Raised when som
+00001e80: 6574 6869 6e67 2065 6c73 6520 7765 6e74  ething else went
+00001e90: 2077 726f 6e67 2c20 7468 6174 2064 6f65   wrong, that doe
+00001ea0: 7320 6e6f 7420 6861 7665 2061 2073 7065  s not have a spe
+00001eb0: 6369 6669 6320 6578 6365 7074 696f 6e20  cific exception 
+00001ec0: 636c 6173 732e 0a20 2020 2020 2020 2029  class..        )
+00001ed0: 0272 1f00 0000 da01 714e 721b 0000 007a  .r......qNr....z
+00001ee0: 0c63 7572 7265 6e74 2e6a 736f 6e72 1000  .current.jsonr..
+00001ef0: 0000 7201 0000 0029 0472 1f00 0000 7247  ..r....).r....rG
+00001f00: 0000 0072 0500 0000 723f 0000 0029 0872  ...r....r?...).r
+00001f10: 2e00 0000 724a 0000 0072 1b00 0000 721f  ....rJ...r....r.
+00001f20: 0000 0072 2100 0000 7236 0000 0072 4300  ...r!...r6...rC.
+00001f30: 0000 da07 7765 6174 6865 7272 3300 0000  ....weatherr3...
+00001f40: 7233 0000 0072 3400 0000 da13 6765 745f  r3...r4.....get_
+00001f50: 6375 7272 656e 745f 7765 6174 6865 72ba  current_weather.
+00001f60: 0000 0073 1200 0000 082d 0201 04fe 0203  ...s.....-......
+00001f70: 04fd 1005 0c01 1602 0401 7a1a 436c 6965  ..........z.Clie
+00001f80: 6e74 2e67 6574 5f63 7572 7265 6e74 5f77  nt.get_current_w
+00001f90: 6561 7468 6572 6302 0000 0000 0000 0000  eatherc.........
+00001fa0: 0000 0005 0000 0007 0000 0043 0000 0073  ...........C...s
+00001fb0: 3e00 0000 7c00 a000 6401 6402 7c01 6901  >...|...d.d.|.i.
+00001fc0: a102 7d02 6700 7d03 7c02 6403 1900 4400  ..}.g.}.|.d...D.
+00001fd0: 5d0e 7d04 7c03 a001 7402 7c04 7c02 6404  ].}.|...t.|.|.d.
+00001fe0: 1900 6a03 6405 8303 a101 0100 710e 7c03  ..j.d.......q.|.
+00001ff0: 5300 2906 61ec 0300 000a 2020 2020 2020  S.).a.....      
+00002000: 2020 4765 7420 6c6f 6361 7469 6f6e 7320    Get locations 
+00002010: 666f 7220 6769 7665 6e20 7175 6572 790a  for given query.
+00002020: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00002030: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00002040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00002050: 2020 2020 7175 6572 793a 203a 636c 6173      query: :clas
+00002060: 733a 6073 7472 600a 2020 2020 2020 2020  s:`str`.        
+00002070: 2020 2020 5175 6572 7920 7374 7269 6e67      Query string
+00002080: 2c20 6120 6c6f 6361 7469 6f6e 2079 6f75  , a location you
+00002090: 2061 7265 2073 6561 7263 6869 6e67 2066   are searching f
+000020a0: 6f72 0a0a 2020 2020 2020 2020 5265 7475  or..        Retu
+000020b0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+000020c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000020d0: 4c69 7374 5b3a 636c 6173 733a 604c 6f63  List[:class:`Loc
+000020e0: 6174 696f 6e44 6174 6160 5d0a 2020 2020  ationData`].    
+000020f0: 2020 2020 2020 2020 4120 6c69 7374 206f          A list o
+00002100: 6620 3a63 6c61 7373 3a60 4c6f 6361 7469  f :class:`Locati
+00002110: 6f6e 4461 7461 6020 636c 6173 7365 732e  onData` classes.
+00002120: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00002130: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002140: 2d2d 0a20 2020 2020 2020 203a 6578 633a  --.        :exc:
+00002150: 604e 6f4c 6f63 6174 696f 6e46 6f75 6e64  `NoLocationFound
+00002160: 600a 2020 2020 2020 2020 2020 2020 5261  `.            Ra
+00002170: 6973 6564 2077 6865 6e20 6e6f 206c 6f63  ised when no loc
+00002180: 6174 696f 6e20 666f 7220 6769 7665 6e20  ation for given 
+00002190: 7175 6572 7920 7761 7320 666f 756e 640a  query was found.
+000021a0: 2020 2020 2020 2020 3a65 7863 3a60 496e          :exc:`In
+000021b0: 7661 6c69 6441 5049 4b65 7960 0a20 2020  validAPIKey`.   
+000021c0: 2020 2020 2020 2020 2052 6169 7365 6420           Raised 
+000021d0: 7768 656e 2074 6865 2041 5049 206b 6579  when the API key
+000021e0: 2069 7320 696e 7661 6c69 640a 2020 2020   is invalid.    
+000021f0: 2020 2020 3a65 7863 3a60 4150 494c 696d      :exc:`APILim
+00002200: 6974 4578 6365 6564 6564 600a 2020 2020  itExceeded`.    
+00002210: 2020 2020 2020 2020 5261 6973 6564 2077          Raised w
+00002220: 6865 6e20 4150 4920 6b65 7920 6361 6c6c  hen API key call
+00002230: 7320 6c69 6d69 7420 7761 7320 6578 6365  s limit was exce
+00002240: 6564 6564 0a20 2020 2020 2020 203a 6578  eded.        :ex
+00002250: 633a 6041 5049 4b65 7944 6973 6162 6c65  c:`APIKeyDisable
+00002260: 6460 0a20 2020 2020 2020 2020 2020 2052  d`.            R
+00002270: 6169 7365 6420 7768 656e 2041 5049 206b  aised when API k
+00002280: 6579 2069 7320 6469 7361 626c 6564 0a20  ey is disabled. 
+00002290: 2020 2020 2020 203a 6578 633a 6041 6363         :exc:`Acc
+000022a0: 6573 7344 656e 6965 6460 0a20 2020 2020  essDenied`.     
+000022b0: 2020 2020 2020 2052 6169 7365 6420 7768         Raised wh
+000022c0: 656e 2061 6363 6573 7320 746f 2067 6976  en access to giv
+000022d0: 656e 2072 6573 6f75 7263 6520 7761 7320  en resource was 
+000022e0: 6465 6e69 6564 0a20 2020 2020 2020 203a  denied.        :
+000022f0: 6578 633a 6049 6e74 6572 6e61 6c41 7070  exc:`InternalApp
+00002300: 6c69 6361 7469 6f6e 4572 726f 7260 0a20  licationError`. 
+00002310: 2020 2020 2020 2020 2020 2052 6169 7365             Raise
+00002320: 6420 7768 656e 2074 6865 7265 2077 6173  d when there was
+00002330: 2061 2076 6572 7920 7261 7265 2069 6e74   a very rare int
+00002340: 6572 6e61 6c20 6170 706c 6963 6174 696f  ernal applicatio
+00002350: 6e20 6572 726f 720a 2020 2020 2020 2020  n error.        
+00002360: 3a65 7863 3a60 5765 6174 6865 7241 5049  :exc:`WeatherAPI
+00002370: 4578 6365 7074 696f 6e60 0a20 2020 2020  Exception`.     
+00002380: 2020 2020 2020 2052 6169 7365 6420 7768         Raised wh
+00002390: 656e 2073 6f6d 6574 6869 6e67 2065 6c73  en something els
+000023a0: 6520 7765 6e74 2077 726f 6e67 2c20 7468  e went wrong, th
+000023b0: 6174 2064 6f65 7320 6e6f 7420 6861 7665  at does not have
+000023c0: 2061 2073 7065 6369 6669 6320 6578 6365   a specific exce
+000023d0: 7074 696f 6e20 636c 6173 732e 0a20 2020  ption class..   
+000023e0: 2020 2020 207a 0b73 6561 7263 682e 6a73       z.search.js
+000023f0: 6f6e 724b 0000 0072 1000 0000 7201 0000  onrK...r....r...
+00002400: 004e 2904 7247 0000 00da 0661 7070 656e  .N).rG.....appen
+00002410: 6472 0600 0000 723f 0000 0029 0572 2e00  dr....r?...).r..
+00002420: 0000 724a 0000 0072 4300 0000 da09 6c6f  ..rJ...rC.....lo
+00002430: 6361 7469 6f6e 73da 036c 6f63 7233 0000  cations..locr3..
+00002440: 0072 3300 0000 7234 0000 00da 0d67 6574  .r3...r4.....get
+00002450: 5f6c 6f63 6174 696f 6e73 f100 0000 730a  _locations....s.
+00002460: 0000 0010 1f04 020c 011a 0104 017a 1443  .............z.C
+00002470: 6c69 656e 742e 6765 745f 6c6f 6361 7469  lient.get_locati
+00002480: 6f6e 7329 0372 1f00 0000 da06 616c 6572  ons).r......aler
+00002490: 7473 721b 0000 0072 5200 0000 6302 0000  tsr....rR...c...
+000024a0: 0000 0000 0003 0000 0009 0000 0005 0000  ................
+000024b0: 004b 0000 0073 5800 0000 7c02 7004 7c00  .K...sX...|.p.|.
+000024c0: 6a00 7c01 7c03 700c 7c00 6a01 a002 6401  j.|.|.p.|.j...d.
+000024d0: a101 6402 9c03 7c05 a501 7d06 7c04 6403  ..d...|...}.|.d.
+000024e0: 7501 7219 7c04 7c06 6404 3c00 7c00 a003  u.r.|.|.d.<.|...
+000024f0: 6405 7c06 a102 7d07 7404 7c07 6406 1900  d.|...}.t.|.d...
+00002500: 7c07 6407 1900 6a05 6403 8303 7d08 7c08  |.d...j.d...}.|.
+00002510: 5300 2908 616b 0600 000a 2020 2020 2020  S.).ak....      
+00002520: 2020 4765 7420 666f 7265 6361 7374 2064    Get forecast d
+00002530: 6174 6120 6672 6f6d 2046 6f72 6563 6173  ata from Forecas
+00002540: 7420 4150 490a 0a20 2020 2020 2020 2050  t API..        P
+00002550: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00002560: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a    -------------.
+00002570: 2020 2020 2020 2020 7175 6572 793a 203a          query: :
+00002580: 636c 6173 733a 6073 7472 600a 2020 2020  class:`str`.    
+00002590: 2020 2020 2020 2020 5175 6572 7920 7374          Query st
+000025a0: 7269 6e67 2c20 6c6f 6361 7469 6f6e 2079  ring, location y
+000025b0: 6f75 2077 616e 7420 746f 2067 6574 2066  ou want to get f
+000025c0: 6f72 6563 6173 7420 6461 7461 2066 6f72  orecast data for
+000025d0: 0a20 2020 2020 2020 2061 7169 3a20 4f70  .        aqi: Op
+000025e0: 7469 6f6e 616c 5b3a 636c 6173 733a 6062  tional[:class:`b
+000025f0: 6f6f 6c60 5d0a 2020 2020 2020 2020 2020  ool`].          
+00002600: 2020 456e 6162 6c65 2f44 6973 6162 6c65    Enable/Disable
+00002610: 2041 6972 2051 7561 6c69 7479 2064 6174   Air Quality dat
+00002620: 612e 2044 6566 6175 6c74 7320 746f 2060  a. Defaults to `
+00002630: 604e 6f6e 6560 6020 2877 696c 6c20 7573  `None`` (will us
+00002640: 6520 636c 6965 6e74 2773 2064 6566 6175  e client's defau
+00002650: 6c74 290a 2020 2020 2020 2020 616c 6572  lt).        aler
+00002660: 7473 3a20 4f70 7469 6f6e 616c 5b3a 636c  ts: Optional[:cl
+00002670: 6173 733a 6062 6f6f 6c60 5d0a 2020 2020  ass:`bool`].    
+00002680: 2020 2020 2020 2020 456e 6162 6c65 2f44          Enable/D
+00002690: 6973 6162 6c65 2061 6c65 7274 7320 6461  isable alerts da
+000026a0: 7461 2e20 4465 6661 756c 7473 2074 6f20  ta. Defaults to 
+000026b0: 6060 4e6f 6e65 6060 2028 7769 6c6c 2075  ``None`` (will u
+000026c0: 7365 2063 6c69 656e 7427 7320 6465 6661  se client's defa
+000026d0: 756c 7429 0a20 2020 2020 2020 206c 616e  ult).        lan
+000026e0: 673a 204f 7074 696f 6e61 6c5b 556e 696f  g: Optional[Unio
+000026f0: 6e5b 3a63 6c61 7373 6073 7472 602c 203a  n[:class`str`, :
+00002700: 636c 6173 7360 4c61 6e67 7561 6765 7360  class`Languages`
+00002710: 5d5d 0a20 2020 2020 2020 2020 2020 204c  ]].            L
+00002720: 616e 6775 6167 6520 6672 6f6d 2074 6865  anguage from the
+00002730: 203a 636c 6173 733a 604c 616e 6775 6167   :class:`Languag
+00002740: 6573 6020 656e 756d 206f 7220 6120 7374  es` enum or a st
+00002750: 7269 6e67 2072 6570 7265 7365 6e74 696e  ring representin
+00002760: 6720 7468 6520 6c61 6e67 7561 6765 206f  g the language o
+00002770: 7220 6c61 6e67 7561 6765 2063 6f64 6520  r language code 
+00002780: 2870 7265 6665 7261 626c 7929 2e0a 2020  (preferably)..  
+00002790: 2020 2020 2020 2020 2020 546f 2067 6574            To get
+000027a0: 2061 206c 6973 7420 6f66 206c 616e 6775   a list of langu
+000027b0: 6167 6573 2076 6973 6974 203a 636c 6173  ages visit :clas
+000027c0: 733a 604c 616e 6775 6167 6573 602e 0a20  s:`Languages`.. 
+000027d0: 2020 2020 2020 206b 7761 7267 733a 2044         kwargs: D
+000027e0: 6963 745b 3a63 6c61 7373 3a60 7374 7260  ict[:class:`str`
+000027f0: 2c20 416e 795d 0a20 2020 2020 2020 2020  , Any].         
+00002800: 2020 2041 6464 6974 696f 6e61 6c20 6b65     Additional ke
+00002810: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00002820: 7468 6174 2077 696c 6c20 6265 2070 6173  that will be pas
+00002830: 7365 6420 746f 2074 6865 2072 6571 7565  sed to the reque
+00002840: 7374 2e0a 2020 2020 2020 2020 2020 2020  st..            
+00002850: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00002860: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002870: 2d2d 2d0a 2020 2020 2020 2020 3a63 6c61  ---.        :cla
+00002880: 7373 3a60 466f 7265 6361 7374 4461 7461  ss:`ForecastData
+00002890: 600a 2020 2020 2020 2020 2020 2020 4665  `.            Fe
+000028a0: 7463 6865 6420 666f 7265 6361 7374 2064  tched forecast d
+000028b0: 6174 6120 6173 2061 2063 6c61 7373 2e0a  ata as a class..
+000028c0: 0a20 2020 2020 2020 2052 6169 7365 730a  .        Raises.
+000028d0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000028e0: 2d0a 2020 2020 2020 2020 3a65 7863 3a60  -.        :exc:`
+000028f0: 4e6f 4c6f 6361 7469 6f6e 466f 756e 6460  NoLocationFound`
+00002900: 0a20 2020 2020 2020 2020 2020 2052 6169  .            Rai
+00002910: 7365 6420 7768 656e 206e 6f20 6c6f 6361  sed when no loca
+00002920: 7469 6f6e 2066 6f72 2067 6976 656e 2071  tion for given q
+00002930: 7565 7279 2077 6173 2066 6f75 6e64 0a20  uery was found. 
+00002940: 2020 2020 2020 203a 6578 633a 6049 6e76         :exc:`Inv
+00002950: 616c 6964 4150 494b 6579 600a 2020 2020  alidAPIKey`.    
+00002960: 2020 2020 2020 2020 5261 6973 6564 2077          Raised w
+00002970: 6865 6e20 7468 6520 4150 4920 6b65 7920  hen the API key 
+00002980: 6973 2069 6e76 616c 6964 0a20 2020 2020  is invalid.     
+00002990: 2020 203a 6578 633a 6041 5049 4c69 6d69     :exc:`APILimi
+000029a0: 7445 7863 6565 6465 6460 0a20 2020 2020  tExceeded`.     
+000029b0: 2020 2020 2020 2052 6169 7365 6420 7768         Raised wh
+000029c0: 656e 2041 5049 206b 6579 2063 616c 6c73  en API key calls
+000029d0: 206c 696d 6974 2077 6173 2065 7863 6565   limit was excee
+000029e0: 6465 640a 2020 2020 2020 2020 3a65 7863  ded.        :exc
+000029f0: 3a60 4150 494b 6579 4469 7361 626c 6564  :`APIKeyDisabled
+00002a00: 600a 2020 2020 2020 2020 2020 2020 5261  `.            Ra
+00002a10: 6973 6564 2077 6865 6e20 4150 4920 6b65  ised when API ke
+00002a20: 7920 6973 2064 6973 6162 6c65 640a 2020  y is disabled.  
+00002a30: 2020 2020 2020 3a65 7863 3a60 4163 6365        :exc:`Acce
+00002a40: 7373 4465 6e69 6564 600a 2020 2020 2020  ssDenied`.      
+00002a50: 2020 2020 2020 5261 6973 6564 2077 6865        Raised whe
+00002a60: 6e20 6163 6365 7373 2074 6f20 6769 7665  n access to give
+00002a70: 6e20 7265 736f 7572 6365 2077 6173 2064  n resource was d
+00002a80: 656e 6965 640a 2020 2020 2020 2020 3a65  enied.        :e
+00002a90: 7863 3a60 496e 7465 726e 616c 4170 706c  xc:`InternalAppl
+00002aa0: 6963 6174 696f 6e45 7272 6f72 600a 2020  icationError`.  
+00002ab0: 2020 2020 2020 2020 2020 5261 6973 6564            Raised
+00002ac0: 2077 6865 6e20 7468 6572 6520 7761 7320   when there was 
+00002ad0: 6120 7665 7279 2072 6172 6520 696e 7465  a very rare inte
+00002ae0: 726e 616c 2061 7070 6c69 6361 7469 6f6e  rnal application
+00002af0: 2065 7272 6f72 0a20 2020 2020 2020 203a   error.        :
+00002b00: 6578 633a 6057 6561 7468 6572 4150 4945  exc:`WeatherAPIE
+00002b10: 7863 6570 7469 6f6e 600a 2020 2020 2020  xception`.      
+00002b20: 2020 2020 2020 5261 6973 6564 2077 6865        Raised whe
+00002b30: 6e20 736f 6d65 7468 696e 6720 656c 7365  n something else
+00002b40: 2077 656e 7420 7772 6f6e 672c 2074 6861   went wrong, tha
+00002b50: 7420 646f 6573 206e 6f74 2068 6176 6520  t does not have 
+00002b60: 6120 7370 6563 6966 6963 2065 7863 6570  a specific excep
+00002b70: 7469 6f6e 2063 6c61 7373 2e0a 2020 2020  tion class..    
+00002b80: 2020 2020 7252 0000 0029 0372 1f00 0000      rR...).r....
+00002b90: 724b 0000 0072 5200 0000 4e72 1b00 0000  rK...rR...Nr....
+00002ba0: 7a0d 666f 7265 6361 7374 2e6a 736f 6e72  z.forecast.jsonr
+00002bb0: 1000 0000 7201 0000 0029 0672 1f00 0000  ....r....).r....
+00002bc0: 7221 0000 0072 3d00 0000 7247 0000 0072  r!...r=...rG...r
+00002bd0: 0700 0000 723f 0000 0029 0972 2e00 0000  ....r?...).r....
+00002be0: 724a 0000 0072 1f00 0000 7252 0000 0072  rJ...r....rR...r
+00002bf0: 1b00 0000 7221 0000 0072 3600 0000 7243  ....r!...r6...rC
+00002c00: 0000 00da 0866 6f72 6563 6173 7472 3300  .....forecastr3.
+00002c10: 0000 7233 0000 0072 3400 0000 da11 6765  ..r3...r4.....ge
+00002c20: 745f 666f 7265 6361 7374 5f64 6174 6117  t_forecast_data.
+00002c30: 0100 0073 1400 0000 0831 0201 0e01 04fd  ...s.....1......
+00002c40: 0204 04fc 1006 0c02 1601 0401 7a18 436c  ............z.Cl
+00002c50: 6965 6e74 2e67 6574 5f66 6f72 6563 6173  ient.get_forecas
+00002c60: 745f 6461 7461 6301 0000 0000 0000 0000  t_datac.........
+00002c70: 0000 0001 0000 0007 0000 0043 0000 0073  ...........C...s
+00002c80: 2400 0000 6401 7c00 6a00 6a01 9b00 6402  $...d.|.j.j...d.
+00002c90: 7c00 6a02 6403 1900 9b00 6404 7c00 6a03  |.j.d.....d.|.j.
+00002ca0: 9b00 6405 9d07 5300 a906 4efa 013c 7a09  ..d...S...N..<z.
+00002cb0: 2061 7069 5f6b 6579 3d72 2500 0000 7a06   api_key=r%...z.
+00002cc0: 206c 616e 673d fa01 3e29 0472 3200 0000   lang=..>).r2...
+00002cd0: da08 5f5f 6e61 6d65 5f5f 7227 0000 0072  ..__name__r'...r
+00002ce0: 1b00 0000 a901 722e 0000 0072 3300 0000  ......r....r3...
+00002cf0: 7233 0000 0072 3400 0000 da07 5f5f 7374  r3...r4.....__st
+00002d00: 725f 5f53 0100 0073 0200 0000 2401 7a0e  r__S...s....$.z.
+00002d10: 436c 6965 6e74 2e5f 5f73 7472 5f5f 6301  Client.__str__c.
+00002d20: 0000 0000 0000 0000 0000 0001 0000 0008  ................
+00002d30: 0000 0043 0000 0073 2800 0000 7400 6401  ...C...s(...t.d.
+00002d40: 7c00 6a01 6a02 9b00 6402 7c00 6a03 6403  |.j.j...d.|.j.d.
+00002d50: 1900 9b00 6404 7c00 6a04 9b00 6405 9d07  ....d.|.j...d...
+00002d60: 8301 5300 7255 0000 0029 05da 0472 6570  ..S.rU...)...rep
+00002d70: 7272 3200 0000 7258 0000 0072 2700 0000  rr2...rX...r'...
+00002d80: 721b 0000 0072 5900 0000 7233 0000 0072  r....rY...r3...r
+00002d90: 3300 0000 7234 0000 00da 085f 5f72 6570  3...r4.....__rep
+00002da0: 725f 5f56 0100 0073 0200 0000 2801 7a0f  r__V...s....(.z.
+00002db0: 436c 6965 6e74 2e5f 5f72 6570 725f 5f29  Client.__repr__)
+00002dc0: 064e 4e4e 4e46 4629 1772 5800 0000 da0a  .NNNNFF).rX.....
+00002dd0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00002de0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00002df0: 5fda 0373 7472 7214 0000 0072 1500 0000  _..strr....r....
+00002e00: 7204 0000 00da 0369 6e74 da04 626f 6f6c  r......int..bool
+00002e10: 7213 0000 0072 1100 0000 722c 0000 0072  r....r....r,...r
+00002e20: 4700 0000 7249 0000 0072 0500 0000 724d  G...rI...r....rM
+00002e30: 0000 0072 5100 0000 7207 0000 0072 5400  ...rQ...r....rT.
+00002e40: 0000 725a 0000 0072 5c00 0000 da0d 5f5f  ..rZ...r\.....__
+00002e50: 636c 6173 7363 656c 6c5f 5f72 3300 0000  classcell__r3...
+00002e60: 7233 0000 0072 3100 0000 7234 0000 0072  r3...r1...r4...r
+00002e70: 1900 0000 3d00 0000 737a 0000 0008 0004  ....=...sz......
+00002e80: 0102 2c02 0102 0102 0102 0102 0104 f802  ..,.............
+00002e90: 0202 fe0e 0302 fd06 0402 fc06 0502 fb06  ................
+00002ea0: 0602 fa02 0702 f902 0802 f80a 0902 f702  ................
+00002eb0: 0a0e f626 201e 1e02 1802 0106 fc02 0102  ...& ...........
+00002ec0: ff0e 0302 fd06 0402 fc0a 0502 fb02 060a  ................
+00002ed0: fa0e 3702 2a02 0102 0106 fa02 0202 fe06  ..7.*...........
+00002ee0: 0402 fc06 0502 fb0e 0602 fa0a 0702 f902  ................
+00002ef0: 080a f808 3c10 0372 1900 0000 4e29 1e72  ....<..r....N).r
+00002f00: 5f00 0000 da04 636f 7265 7202 0000 00da  _.....corer.....
+00002f10: 0565 6e75 6d73 7204 0000 00da 0972 6573  .enumsr......res
+00002f20: 706f 6e73 6573 7205 0000 0072 0600 0000  ponsesr....r....
+00002f30: 7207 0000 00da 0665 7272 6f72 7372 0800  r......errorsr..
+00002f40: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00002f50: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00002f60: da00 720f 0000 00da 0674 7970 696e 6772  ..r......typingr
+00002f70: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00002f80: 0000 0072 1500 0000 7216 0000 0072 2d00  ...r....r....r-.
+00002f90: 0000 723c 0000 00da 075f 5f61 6c6c 5f5f  ..r<.....__all__
+00002fa0: 7219 0000 0072 3300 0000 7233 0000 0072  r....r3...r3...r
+00002fb0: 3300 0000 7234 0000 00da 083c 6d6f 6475  3...r4.....<modu
+00002fc0: 6c65 3e01 0000 0073 1600 0000 0400 0c18  le>....s........
+00002fd0: 0c01 1401 2405 0c09 2004 0409 0a01 0402  ....$... .......
+00002fe0: 1404                                     ..
```

