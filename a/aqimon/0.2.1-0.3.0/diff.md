# Comparing `tmp/aqimon-0.2.1.tar.gz` & `tmp/aqimon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqimon-0.2.1.tar", max compression
+gzip compressed data, was "aqimon-0.3.0.tar", max compression
```

## Comparing `aqimon-0.2.1.tar` & `aqimon-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1065 2023-03-28 05:09:53.462436 aqimon-0.2.1/LICENSE
--rw-r--r--   0        0        0     4690 2023-03-28 05:09:53.462436 aqimon-0.2.1/README.md
--rw-r--r--   0        0        0       45 2023-03-28 05:09:53.462436 aqimon-0.2.1/aqimon/__init__.py
--rw-r--r--   0        0        0     1129 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/aqi_common.py
--rw-r--r--   0        0        0     1822 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/config.py
--rw-r--r--   0        0        0     2397 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/database.py
--rw-r--r--   0        0        0      865 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/read/__init__.py
--rw-r--r--   0        0        0     1539 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/read/mock.py
--rw-r--r--   0        0        0     2270 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/read/novapm.py
--rw-r--r--   0        0        0     5322 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/server.py
--rw-r--r--   0        0        0     6835 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/android-chrome-192x192.png
--rw-r--r--   0        0        0    20365 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/android-chrome-512x512.png
--rw-r--r--   0        0        0     6288 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/apple-touch-icon.png
--rw-r--r--   0        0        0   426477 2023-03-28 05:09:58.706537 aqimon-0.2.1/aqimon/static/elm.js
--rw-r--r--   0        0        0      351 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/favicon-16x16.png
--rw-r--r--   0        0        0      754 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/favicon.ico
--rw-r--r--   0        0        0     1799 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/images/failing.png
--rw-r--r--   0        0        0     2418 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/images/idle.png
--rw-r--r--   0        0        0    24380 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/images/loading.gif
--rw-r--r--   0        0        0      696 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/static/index.html
--rw-r--r--   0        0        0     5587 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/templates/index.html
--rw-r--r--   0        0        0     1329 2023-03-28 05:09:53.466436 aqimon-0.2.1/aqimon/usb.py
--rw-r--r--   0        0        0      803 2023-03-28 05:09:53.466436 aqimon-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 aqimon-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 23:22:03.569603 aqimon-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5828 2023-04-23 23:22:03.569603 aqimon-0.3.0/README.md
+-rw-r--r--   0        0        0       45 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/__init__.py
+-rw-r--r--   0        0        0     2449 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/aqi_common.py
+-rw-r--r--   0        0        0     2372 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/config.py
+-rw-r--r--   0        0        0     6988 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/database.py
+-rw-r--r--   0        0        0      881 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/mock.py
+-rw-r--r--   0        0        0     2113 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/novapm.py
+-rw-r--r--   0        0        0    12441 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/constants.py
+-rw-r--r--   0        0        0     1524 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/exceptions.py
+-rw-r--r--   0        0        0     4082 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/responses.py
+-rw-r--r--   0        0        0     7944 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/server.py
+-rw-r--r--   0        0        0     6835 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    20365 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0     6288 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/apple-touch-icon.png
+-rw-r--r--   0        0        0   437308 2023-04-23 23:22:33.441220 aqimon-0.3.0/aqimon/static/elm.js
+-rw-r--r--   0        0        0      351 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/favicon-16x16.png
+-rw-r--r--   0        0        0      754 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/favicon.ico
+-rw-r--r--   0        0        0     1799 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/images/failing.png
+-rw-r--r--   0        0        0     2418 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/images/idle.png
+-rw-r--r--   0        0        0    24380 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/images/loading.gif
+-rw-r--r--   0        0        0      696 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/index.html
+-rw-r--r--   0        0        0     5587 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/templates/index.html
+-rw-r--r--   0        0        0      968 2023-04-23 23:22:03.569603 aqimon-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 aqimon-0.3.0/PKG-INFO
```

### Comparing `aqimon-0.2.1/LICENSE` & `aqimon-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/README.md` & `aqimon-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 # AQIMON
 
 A simple Air Quality Index monitor, designed to work on the Raspberry Pi with the SDS011 Nova PM Sensor.
 
-## Installation
+- [AQIMON](#aqimon)
+  - [Installation](#installation)
+    - [Pre-Requisites](#pre-requisites)
+    - [Install](#install)
+  - [Running Aqimon](#running-aqimon)
+    - [Configure With Systemd](#configure-with-systemd)
+  - [Configuration](#configuration)
+  - [Contributing](#contributing)
+    - [Toolset](#toolset)
+    - [Quickstart](#quickstart)
+    - [Using the Mock Reader](#using-the-mock-reader)
+    - [Submitting a PR](#submitting-a-pr)
 
+## Installation
 
 ### Pre-Requisites
 
-* Python 3.9+
-* [uhubctl](https://github.com/mvp/uhubctl) must be installed and on your PATH.
+- Python 3.9+
 
 ### Install
 
 ```commandline
 pip install aqimon
 ```
 
 ## Running Aqimon
 
-Aqimon is a simple web server.  To start with all the defaults, you can just run:
+Aqimon is a simple web server.  To start with all the defaults (assuming available SDS011 hardware on `/dev/ttyUSB0`), you can just run:
 
 ```commandline
 aqimon
 ```
 
 And then go to your browser at `http://{serveraddress}:8000/` to view the UI.
 
+If you don't have the requisite SDS011 hardware, you can use a mock data source via a [mock reader](#using-the-mock-reader).
+
 ### Configure With Systemd
 
 Generally, you'd want to run `Aqimon` as an always-on service, using `systemd`.
 
 To do so, create a file at `/etc/systemd/system/aqimin.service` with the following contents:
 
-```
+```text
 [Unit]
 Description=AQIMON
 After=multi-user.target
 
 [Service]
 Type=simple
 Restart=always
@@ -53,38 +66,40 @@
 sudo systemctl start aqimon
 ```
 
 ## Configuration
 
 Aqimon uses environment variables for configuration, but all values should ship with sensible defaults.
 
-| Variable                         | Default             | Description                                                                                                                       |
-|----------------------------------|---------------------|-----------------------------------------------------------------------------------------------------------------------------------|
-| **AQIMON_DB_PATH**               | ~/.aqimon/db.sqlite | The path to the database file, where read information is stored. It should be an absolute path; user home expansion is supported. | 
-| **AQIMON_POLL_FREQUENCY_SEC**    | 900 (15 minutes)    | Sets how frequently to read from the device, in seconds.                                                                          |
-| **AQIMON_RETENTION_MINUTES**     | 10080 (1 week)      | Sets how long data will be kept in the database, in minutes.                                                                      |
-| **AQIMON_READER_TYPE**           | NOVAPM              | The reader type to use, either NOVAPM or MOCK.                                                                                    |
-| **AQIMON_USB_PATH**              | /dev/ttyUSB0        | The path to the USB device for the sensor.                                                                                        |
-| **AQIMON_SLEEP_TIME_SEC**        | 5                   | The number of seconds to wait for between each read in a set of reads.                                                            |
-| **AQIMON_SAMPLE_COUNT_PER_READ** | 5                   | The number of reads to take with each sample.                                                                                     |
-| **AQIMON_SERVER_PORT**           | 8000                | The port to run the server on.                                                                                                    |
-| **AQIMON_SERVER_HOST**           | 0.0.0.0             | The host to run the server on.                                                                                                    |
- 
+| Variable                           | Default             | Description                                                                                                                       |
+|------------------------------------|---------------------|-----------------------------------------------------------------------------------------------------------------------------------|
+| **AQIMON_DB_PATH**                 | ~/.aqimon/db.sqlite | The path to the database file, where read information is stored. It should be an absolute path; user home expansion is supported. |
+| **AQIMON_POLL_FREQUENCY_SEC**      | 900 (15 minutes)    | Sets how frequently to read from the device, in seconds.                                                                          |
+| **AQIMON_RETENTION_MINUTES**       | 10080 (1 week)      | Sets how long data will be kept in the database, in minutes.                                                                      |
+| **AQIMON_READER_TYPE**             | NOVAPM              | The reader type to use, either NOVAPM or MOCK.                                                                                    |
+| **AQIMON_USB_PATH**                | /dev/ttyUSB0        | The path to the USB device for the sensor.                                                                                        |
+| **AQIMON_SLEEP_SEC_BETWEEN_READS** | 5                   | The number of seconds to wait for between each read in a set of reads.                                                            |
+| **AQIMON_SAMPLE_COUNT_PER_READ**   | 5                   | The number of reads to take with each sample.                                                                                     |
+| **AQIMON_WARM_UP_SEC**             | 15                  | The number of seconds to wait for the device to warm up before reading.                                                           |
+| **AQIMON_COMMAND_WAIT_TIME**       | 1                   | The number of seconds to wait for the device respond to a command.                                                                |
+| **AQIMON_EPA_LOOKBACK_MIN**        | 60*8                | The number of minutes to look back at read data to calculate the EPA AQI.                                                         |
+| **AQIMON_SERVER_PORT**             | 8000                | The port to run the server on.                                                                                                    |
+| **AQIMON_SERVER_HOST**             | 0.0.0.0             | The host to run the server on.                                                                                                    |
 
 ## Contributing
 
 ### Toolset
 
 To start developing, you'll need to install the following tools:
 
-* [Python 3.9+](https://www.python.org/) - For API Code
-* [Elm 0.19](https://elm-lang.org/) - For client code
-* [poetry](https://python-poetry.org/) - For python package management
-* [justfile](https://github.com/casey/just) - For builds
-* [elm-format](https://github.com/avh4/elm-format) - For auto-formatting elm code.
+- [Python 3.9+](https://www.python.org/) - For API Code
+- [Elm 0.19](https://elm-lang.org/) - For client code
+- [poetry](https://python-poetry.org/) - For python package management
+- [justfile](https://github.com/casey/just) - For builds
+- [elm-format](https://github.com/avh4/elm-format) - For auto-formatting elm code.
 
 Optionally, we have [pre-commit](https://pre-commit.com/) hooks available as well.  To install hooks, just run
 `pre-commit install` and then linters and autoformatting will be applied automatically on commit.
 
 ### Quickstart
 
 To build the project, and install all dev-dependencies, run:
@@ -115,19 +130,18 @@
 
 ```commandline
 just format
 ```
 
 ### Using the Mock Reader
 
-Aqimon ships with a mock reader class that you can use in the event that you don't have a reader available on your 
+Aqimon ships with a mock reader class that you can use in the event that you don't have a reader available on your
 development computer.  The mock reader just returns randomized reads.  To use it, you can start the server like:
 
 ```commandline
 AQIMON_READER_TYPE=MOCK poetry run aqimon
 ```
 
 ### Submitting a PR
 
-Master branch is locked, but you can open a PR on the repo.  Build checks must pass, and changes approved by a code 
+Master branch is locked, but you can open a PR on the repo.  Build checks must pass, and changes approved by a code
 owner, before merging.
-
```

### Comparing `aqimon-0.2.1/aqimon/config.py` & `aqimon-0.3.0/aqimon/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,41 +13,54 @@
     poll_frequency_sec: int
     retention_minutes: int
 
     reader_type: str
 
     # Nova PM properties
     usb_path: str
-    usb_sleep_time_sec: int
+    sleep_sec_between_reads: int
     sample_count_per_read: int
+    warm_up_sec: int
+    command_wait_time: int
+
+    # EPA Properties
+    epa_lookback_minutes: int
 
     # Server properties
     server_port: int
     server_host: str
 
 
 DEFAULT_CONFIG = Config(
     database_path=os.path.expanduser(DEFAULT_DB_PATH),
     poll_frequency_sec=60 * 15,  # Every 15 minutes
     retention_minutes=60 * 24 * 7,  # 1 week
+    epa_lookback_minutes=60 * 8,  # 8 hours
     reader_type="NOVAPM",
     usb_path="/dev/ttyUSB0",
-    usb_sleep_time_sec=5,
+    sleep_sec_between_reads=5,
+    warm_up_sec=15,
+    command_wait_time=1,
     sample_count_per_read=5,
     server_port=8000,
     server_host="0.0.0.0",
 )
 
 
 def get_config_from_env() -> Config:
     """Get the config from environment variables."""
     return Config(
         database_path=os.path.expanduser(os.environ.get("AQIMON_DB_PATH", DEFAULT_CONFIG.database_path)),
         poll_frequency_sec=int(os.environ.get("AQIMON_POLL_FREQUENCY_SEC", DEFAULT_CONFIG.poll_frequency_sec)),
         retention_minutes=int(os.environ.get("AQIMON_RETENTION_MINUTES", DEFAULT_CONFIG.retention_minutes)),
         reader_type=os.environ.get("AQIMON_READER_TYPE", DEFAULT_CONFIG.reader_type),
         usb_path=os.environ.get("AQIMON_USB_PATH", DEFAULT_CONFIG.usb_path),
-        usb_sleep_time_sec=int(os.environ.get("AQIMON_USB_SLEEP_TIME_SEC", DEFAULT_CONFIG.usb_sleep_time_sec)),
+        sleep_sec_between_reads=int(
+            os.environ.get("AQIMON_SLEEP_SEC_BETWEEN_READS", DEFAULT_CONFIG.sleep_sec_between_reads)
+        ),
+        warm_up_sec=int(os.environ.get("AQIMON_WARM_UP_SEC", DEFAULT_CONFIG.warm_up_sec)),
+        command_wait_time=int(os.environ.get("AQIMON_COMMAND_WAIT_TIME", DEFAULT_CONFIG.command_wait_time)),
         sample_count_per_read=int(os.environ.get("AQIMON_SAMPLE_COUNT_PER_READ", DEFAULT_CONFIG.sample_count_per_read)),
         server_port=int(os.environ.get("AQIMON_SERVER_PORT", DEFAULT_CONFIG.server_port)),
         server_host=os.environ.get("AQIMON_SERVER_HOST", DEFAULT_CONFIG.server_host),
+        epa_lookback_minutes=int(os.environ.get("AQIMON_EPA_LOOKBACK_MIN", DEFAULT_CONFIG.epa_lookback_minutes)),
     )
```

### Comparing `aqimon-0.2.1/aqimon/read/__init__.py` & `aqimon-0.3.0/aqimon/read/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from enum import Enum
 
 
 class ReaderStatus(Enum):
     """Enum of possible reader states."""
 
     IDLE = 1
-    READING = 2
-    ERRORING = 3
+    WARM_UP = 2
+    READING = 3
+    ERRORING = 4
 
 
 @dataclass(frozen=True)
 class ReaderState:
     """State of a reader.
 
     Used to report status and errors to the user.
```

### Comparing `aqimon-0.2.1/aqimon/read/mock.py` & `aqimon-0.3.0/aqimon/read/mock.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/read/novapm.py` & `aqimon-0.3.0/aqimon/read/novapm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,65 @@
 """Nova PM SDS011 Reader module.
 
 https://www.amazon.com/SDS011-Quality-Detection-Conditioning-Monitor/dp/B07FSDMRR5
 """
-from aqimon import usb
-from . import AqiRead, ReaderState, ReaderStatus
 import asyncio
+
+from . import AqiRead, ReaderState, ReaderStatus
 import serial
+from typing import Union
+from .sds011 import QueryModeReader
 from statistics import mean
 
 
-class NovaPmReader:
+class OpinionatedReader:
     """NOVA PM SDS011 Reader."""
 
-    def __init__(self, usb_path: str, iterations: int = 5, sleep_time: int = 60):
+    def __init__(
+        self,
+        ser_dev: Union[str, serial.Serial],
+        warm_up_secs: int = 15,
+        iterations: int = 5,
+        sleep_time: int = 3,
+        command_wait_time: int = 15,
+    ):
         """Create the device."""
-        self.usb_path = usb_path
+        if isinstance(ser_dev, str):
+            ser_dev = serial.Serial(ser_dev, timeout=2)
+
+        self.reader = QueryModeReader(ser_dev=ser_dev, send_command_sleep=command_wait_time)
+
+        # Initial the reader to be in the mode we want.
+        self.reader.wake()
+        self.reader.set_working_period(0)
+
+        self.warm_up_secs = warm_up_secs
         self.iterations = iterations
         self.sleep_time = sleep_time
+
         self.state = ReaderState(ReaderStatus.IDLE, None)
 
     async def read(self) -> AqiRead:
         """Read from the device."""
         try:
+            self.reader.wake()
+            self.state = ReaderState(ReaderStatus.WARM_UP, None)
+            await asyncio.sleep(self.warm_up_secs)
             self.state = ReaderState(ReaderStatus.READING, None)
-            result = await self._power_saving_read()
+            pm25_reads = []
+            pm10_reads = []
+            for x in range(0, self.iterations):
+                await asyncio.sleep(self.sleep_time)
+                result = self.reader.query()
+                pm25_reads.append(result.pm25)
+                pm10_reads.append(result.pm10)
+            self.reader.sleep()
             self.state = ReaderState(ReaderStatus.IDLE, None)
-            return result
+            return AqiRead(pmtwofive=mean(pm25_reads), pmten=mean(pm10_reads))
         except Exception as e:
             self.state = ReaderState(ReaderStatus.ERRORING, e)
+            self.reader.sleep()
             raise e
 
     def get_state(self) -> ReaderState:
         """Get the current state of the reader."""
         return self.state
-
-    async def _power_saving_read(self) -> AqiRead:
-        try:
-            await usb.turn_on_usb()
-            await asyncio.sleep(5)
-        except usb.UhubCtlNotInstalled:
-            pass
-        result = await self._averaged_read()
-        try:
-            await usb.turn_off_usb()
-            await asyncio.sleep(5)
-        except usb.UhubCtlNotInstalled:
-            pass
-
-        return AqiRead(result.pmtwofive, result.pmten)
-
-    async def _averaged_read(self) -> AqiRead:
-        pm25_reads = []
-        pm10_reads = []
-
-        for x in range(self.iterations):
-            data = self._read()
-            pm25_reads.append(data.pmtwofive)
-            pm10_reads.append(data.pmten)
-            await asyncio.sleep(self.sleep_time)
-
-        avg_pm25 = mean(pm25_reads)
-        avg_pm10 = mean(pm10_reads)
-
-        return AqiRead(pmtwofive=avg_pm25, pmten=avg_pm10)
-
-    def _read(self) -> AqiRead:
-        ser = serial.Serial(self.usb_path)
-        data = ser.read(10)
-        pmtwofive = int.from_bytes(data[2:4], byteorder="little") / 10
-        pmten = int.from_bytes(data[4:6], byteorder="little") / 10
-        return AqiRead(pmtwofive, pmten)
```

### Comparing `aqimon-0.2.1/aqimon/static/android-chrome-192x192.png` & `aqimon-0.3.0/aqimon/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/android-chrome-512x512.png` & `aqimon-0.3.0/aqimon/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/apple-touch-icon.png` & `aqimon-0.3.0/aqimon/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/elm.js` & `aqimon-0.3.0/aqimon/static/elm.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -828,18 +828,18 @@
 
             case 11:
                 throw new Error('Cannot perform mod 0. Division by zero error.');
         }
     }
 
     function _Debug_regionToString(region) {
-        if (region.dt.aT === region.dR.aT) {
-            return 'on line ' + region.dt.aT;
+        if (region.dD.aY === region.d0.aY) {
+            return 'on line ' + region.dD.aY;
         }
-        return 'on lines ' + region.dt.aT + ' through ' + region.dR.aT;
+        return 'on lines ' + region.dD.aY + ' through ' + region.d0.aY;
     }
 
 
 
     // MATH
 
     var _Basics_add = F2(function(a, b) {
@@ -1822,17 +1822,17 @@
     // PROGRAMS
 
 
     var _Platform_worker = F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fu,
+            impl.fN,
+            impl.gr,
             impl.ga,
-            impl.fV,
             function() {
                 return function() {}
             }
         );
     });
 
 
@@ -2622,17 +2622,17 @@
 
     var _VirtualDom_mapEventTuple = F2(function(func, tuple) {
         return _Utils_Tuple2(func(tuple.a), tuple.b);
     });
 
     var _VirtualDom_mapEventRecord = F2(function(func, record) {
         return {
-            Z: func(record.Z),
-            dv: record.dv,
-            dg: record.dg
+            aa: func(record.aa),
+            dF: record.dF,
+            $7: record.$7
         }
     });
 
 
 
     // ORGANIZE FACTS
 
@@ -2864,19 +2864,19 @@
 
             // 0 = Normal
             // 1 = MayStopPropagation
             // 2 = MayPreventDefault
             // 3 = Custom
 
             var value = result.a;
-            var message = !tag ? value : tag < 3 ? value.a : value.Z;
-            var stopPropagation = tag == 1 ? value.b : tag == 3 && value.dv;
+            var message = !tag ? value : tag < 3 ? value.a : value.aa;
+            var stopPropagation = tag == 1 ? value.b : tag == 3 && value.dF;
             var currentEventNode = (
                 stopPropagation && event.stopPropagation(),
-                (tag == 2 ? value.b : tag == 3 && value.dg) && event.preventDefault(),
+                (tag == 2 ? value.b : tag == 3 && value.$7) && event.preventDefault(),
                 eventNode
             );
             var tagger;
             var i;
             while (tagger = currentEventNode.j) {
                 if (typeof tagger == 'function') {
                     message = tagger(message);
@@ -3717,19 +3717,19 @@
 
     var _Debugger_element;
 
     var _Browser_element = _Debugger_element || F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fu,
+            impl.fN,
+            impl.gr,
             impl.ga,
-            impl.fV,
             function(sendToApp, initialModel) {
-                var view = impl.gc;
+                var view = impl.gt;
                 /**/
                 var domNode = args['node'];
                 //*/
                 /**_UNUSED/
                 var domNode = args && args['node'] ? args['node'] : _Debug_crash(0);
                 //*/
                 var currNode = _VirtualDom_virtualize(domNode);
@@ -3751,32 +3751,32 @@
 
     var _Debugger_document;
 
     var _Browser_document = _Debugger_document || F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fu,
+            impl.fN,
+            impl.gr,
             impl.ga,
-            impl.fV,
             function(sendToApp, initialModel) {
-                var divertHrefToApp = impl.dm && impl.dm(sendToApp)
-                var view = impl.gc;
+                var divertHrefToApp = impl.dw && impl.dw(sendToApp)
+                var view = impl.gt;
                 var title = _VirtualDom_doc.title;
                 var bodyNode = _VirtualDom_doc.body;
                 var currNode = _VirtualDom_virtualize(bodyNode);
                 return _Browser_makeAnimator(initialModel, function(model) {
                     _VirtualDom_divertHrefToApp = divertHrefToApp;
                     var doc = view(model);
-                    var nextNode = _VirtualDom_node('body')(_List_Nil)(doc.e6);
+                    var nextNode = _VirtualDom_node('body')(_List_Nil)(doc.fp);
                     var patches = _VirtualDom_diff(currNode, nextNode);
                     bodyNode = _VirtualDom_applyPatches(bodyNode, currNode, patches, sendToApp);
                     currNode = nextNode;
                     _VirtualDom_divertHrefToApp = 0;
-                    (title !== doc.f_) && (_VirtualDom_doc.title = title = doc.f_);
+                    (title !== doc.gf) && (_VirtualDom_doc.title = title = doc.gf);
                 });
             }
         );
     });
 
 
 
@@ -3825,50 +3825,50 @@
 
 
 
     // APPLICATION
 
 
     function _Browser_application(impl) {
-        var onUrlChange = impl.fG;
-        var onUrlRequest = impl.fH;
+        var onUrlChange = impl.fX;
+        var onUrlRequest = impl.fY;
         var key = function() {
             key.a(onUrlChange(_Browser_getUrl()));
         };
 
         return _Browser_document({
-            dm: function(sendToApp) {
+            dw: function(sendToApp) {
                 key.a = sendToApp;
                 _Browser_window.addEventListener('popstate', key);
                 _Browser_window.navigator.userAgent.indexOf('Trident') < 0 || _Browser_window.addEventListener('hashchange', key);
 
                 return F2(function(domNode, event) {
                     if (!event.ctrlKey && !event.metaKey && !event.shiftKey && event.button < 1 && !domNode.target && !domNode.hasAttribute('download')) {
                         event.preventDefault();
                         var href = domNode.href;
                         var curr = _Browser_getUrl();
                         var next = $elm$url$Url$fromString(href).a;
                         sendToApp(onUrlRequest(
                             (next &&
-                                curr.et === next.et &&
-                                curr.d0 === next.d0 &&
-                                curr.eo.a === next.eo.a
+                                curr.eK === next.eK &&
+                                curr.ec === next.ec &&
+                                curr.eF.a === next.eF.a
                             ) ?
                             $elm$browser$Browser$Internal(next) :
                             $elm$browser$Browser$External(href)
                         ));
                     }
                 });
             },
-            fu: function(flags) {
-                return A3(impl.fu, flags, _Browser_getUrl(), key);
+            fN: function(flags) {
+                return A3(impl.fN, flags, _Browser_getUrl(), key);
             },
-            gc: impl.gc,
-            ga: impl.ga,
-            fV: impl.fV
+            gt: impl.gt,
+            gr: impl.gr,
+            ga: impl.ga
         });
     }
 
     function _Browser_getUrl() {
         return $elm$url$Url$fromString(_VirtualDom_doc.location.href).a || _Debug_crash(1);
     }
 
@@ -3928,35 +3928,35 @@
 
     // PAGE VISIBILITY
 
 
     function _Browser_visibilityInfo() {
         return (typeof _VirtualDom_doc.hidden !== 'undefined') ?
             {
-                fn: 'hidden',
-                e8: 'visibilitychange'
+                fG: 'hidden',
+                fr: 'visibilitychange'
             } :
             (typeof _VirtualDom_doc.mozHidden !== 'undefined') ?
             {
-                fn: 'mozHidden',
-                e8: 'mozvisibilitychange'
+                fG: 'mozHidden',
+                fr: 'mozvisibilitychange'
             } :
             (typeof _VirtualDom_doc.msHidden !== 'undefined') ?
             {
-                fn: 'msHidden',
-                e8: 'msvisibilitychange'
+                fG: 'msHidden',
+                fr: 'msvisibilitychange'
             } :
             (typeof _VirtualDom_doc.webkitHidden !== 'undefined') ?
             {
-                fn: 'webkitHidden',
-                e8: 'webkitvisibilitychange'
+                fG: 'webkitHidden',
+                fr: 'webkitvisibilitychange'
             } :
             {
-                fn: 'hidden',
-                e8: 'visibilitychange'
+                fG: 'hidden',
+                fr: 'visibilitychange'
             };
     }
 
 
 
     // ANIMATION FRAMES
 
@@ -4020,30 +4020,30 @@
 
 
     // WINDOW VIEWPORT
 
 
     function _Browser_getViewport() {
         return {
-            eC: _Browser_getScene(),
-            eV: {
-                eZ: _Browser_window.pageXOffset,
-                e_: _Browser_window.pageYOffset,
-                eY: _Browser_doc.documentElement.clientWidth,
-                d$: _Browser_doc.documentElement.clientHeight
+            eV: _Browser_getScene(),
+            fc: {
+                fg: _Browser_window.pageXOffset,
+                fh: _Browser_window.pageYOffset,
+                ff: _Browser_doc.documentElement.clientWidth,
+                eb: _Browser_doc.documentElement.clientHeight
             }
         };
     }
 
     function _Browser_getScene() {
         var body = _Browser_doc.body;
         var elem = _Browser_doc.documentElement;
         return {
-            eY: Math.max(body.scrollWidth, body.offsetWidth, elem.scrollWidth, elem.offsetWidth, elem.clientWidth),
-            d$: Math.max(body.scrollHeight, body.offsetHeight, elem.scrollHeight, elem.offsetHeight, elem.clientHeight)
+            ff: Math.max(body.scrollWidth, body.offsetWidth, elem.scrollWidth, elem.offsetWidth, elem.clientWidth),
+            eb: Math.max(body.scrollHeight, body.offsetHeight, elem.scrollHeight, elem.offsetHeight, elem.clientHeight)
         };
     }
 
     var _Browser_setViewport = F2(function(x, y) {
         return _Browser_withWindow(function() {
             _Browser_window.scroll(x, y);
             return _Utils_Tuple0;
@@ -4054,23 +4054,23 @@
 
     // ELEMENT VIEWPORT
 
 
     function _Browser_getViewportOf(id) {
         return _Browser_withNode(id, function(node) {
             return {
-                eC: {
-                    eY: node.scrollWidth,
-                    d$: node.scrollHeight
-                },
                 eV: {
-                    eZ: node.scrollLeft,
-                    e_: node.scrollTop,
-                    eY: node.clientWidth,
-                    d$: node.clientHeight
+                    ff: node.scrollWidth,
+                    eb: node.scrollHeight
+                },
+                fc: {
+                    fg: node.scrollLeft,
+                    fh: node.scrollTop,
+                    ff: node.clientWidth,
+                    eb: node.clientHeight
                 }
             };
         });
     }
 
 
     var _Browser_setViewportOf = F3(function(id, x, y) {
@@ -4088,26 +4088,26 @@
 
     function _Browser_getElement(id) {
         return _Browser_withNode(id, function(node) {
             var rect = node.getBoundingClientRect();
             var x = _Browser_window.pageXOffset;
             var y = _Browser_window.pageYOffset;
             return {
-                eC: _Browser_getScene(),
-                eV: {
-                    eZ: x,
-                    e_: y,
-                    eY: _Browser_doc.documentElement.clientWidth,
-                    d$: _Browser_doc.documentElement.clientHeight
+                eV: _Browser_getScene(),
+                fc: {
+                    fg: x,
+                    fh: y,
+                    ff: _Browser_doc.documentElement.clientWidth,
+                    eb: _Browser_doc.documentElement.clientHeight
                 },
-                fi: {
-                    eZ: x + rect.left,
-                    e_: y + rect.top,
-                    eY: rect.width,
-                    d$: rect.height
+                fB: {
+                    fg: x + rect.left,
+                    fh: y + rect.top,
+                    ff: rect.width,
+                    eb: rect.height
                 }
             };
         });
     }
 
 
 
@@ -4174,58 +4174,58 @@
 
 
     // SEND REQUEST
 
     var _Http_toTask = F3(function(router, toTask, request) {
         return _Scheduler_binding(function(callback) {
             function done(response) {
-                callback(toTask(request.dT.a(response)));
+                callback(toTask(request.d3.a(response)));
             }
 
             var xhr = new XMLHttpRequest();
             xhr.addEventListener('error', function() {
                 done($elm$http$Http$NetworkError_);
             });
             xhr.addEventListener('timeout', function() {
                 done($elm$http$Http$Timeout_);
             });
             xhr.addEventListener('load', function() {
-                done(_Http_toResponse(request.dT.b, xhr));
+                done(_Http_toResponse(request.d3.b, xhr));
             });
-            $elm$core$Maybe$isJust(request.eR) && _Http_track(router, xhr, request.eR.a);
+            $elm$core$Maybe$isJust(request.e8) && _Http_track(router, xhr, request.e8.a);
 
             try {
-                xhr.open(request.fC, request.eU, true);
+                xhr.open(request.fU, request.fb, true);
             } catch (e) {
-                return done($elm$http$Http$BadUrl_(request.eU));
+                return done($elm$http$Http$BadUrl_(request.fb));
             }
 
             _Http_configureRequest(xhr, request);
 
-            request.e6.a && xhr.setRequestHeader('Content-Type', request.e6.a);
-            xhr.send(request.e6.b);
+            request.fp.a && xhr.setRequestHeader('Content-Type', request.fp.a);
+            xhr.send(request.fp.b);
 
             return function() {
                 xhr.c = true;
                 xhr.abort();
             };
         });
     });
 
 
     // CONFIGURE
 
     function _Http_configureRequest(xhr, request) {
-        for (var headers = request.d_; headers.b; headers = headers.b) // WHILE_CONS
+        for (var headers = request.ea; headers.b; headers = headers.b) // WHILE_CONS
         {
             xhr.setRequestHeader(headers.a.a, headers.a.b);
         }
-        xhr.timeout = request.fY.a || 0;
-        xhr.responseType = request.dT.d;
-        xhr.withCredentials = request.e1;
+        xhr.timeout = request.gd.a || 0;
+        xhr.responseType = request.d3.d;
+        xhr.withCredentials = request.fk;
     }
 
 
     // RESPONSES
 
     function _Http_toResponse(toBody, xhr) {
         return A2(
@@ -4236,18 +4236,18 @@
     }
 
 
     // METADATA
 
     function _Http_toMetadata(xhr) {
         return {
-            eU: xhr.responseURL,
-            fT: xhr.status,
-            fU: xhr.statusText,
-            d_: _Http_parseHeaders(xhr.getAllResponseHeaders())
+            fb: xhr.responseURL,
+            f8: xhr.status,
+            f9: xhr.statusText,
+            ea: _Http_parseHeaders(xhr.getAllResponseHeaders())
         };
     }
 
 
     // HEADERS
 
     function _Http_parseHeaders(rawHeaders) {
@@ -4338,25 +4338,25 @@
         // TODO check out lengthComputable on loadstart event
 
         xhr.upload.addEventListener('progress', function(event) {
             if (xhr.c) {
                 return;
             }
             _Scheduler_rawSpawn(A2($elm$core$Platform$sendToSelf, router, _Utils_Tuple2(tracker, $elm$http$Http$Sending({
-                fQ: event.loaded,
-                eG: event.total
+                f5: event.loaded,
+                eZ: event.total
             }))));
         });
         xhr.addEventListener('progress', function(event) {
             if (xhr.c) {
                 return;
             }
             _Scheduler_rawSpawn(A2($elm$core$Platform$sendToSelf, router, _Utils_Tuple2(tracker, $elm$http$Http$Receiving({
-                fL: event.loaded,
-                eG: event.lengthComputable ? $elm$core$Maybe$Just(event.total) : $elm$core$Maybe$Nothing
+                f0: event.loaded,
+                eZ: event.lengthComputable ? $elm$core$Maybe$Just(event.total) : $elm$core$Maybe$Nothing
             }))));
         });
     }
 
 
     var _Bitwise_and = F2(function(a, b) {
         return a & b;
@@ -4926,20 +4926,20 @@
     };
     var $elm$browser$Browser$Dom$NotFound = $elm$core$Basics$identity;
     var $elm$url$Url$Http = 0;
     var $elm$url$Url$Https = 1;
     var $elm$url$Url$Url = F6(
         function(protocol, host, port_, path, query, fragment) {
             return {
-                dY: fragment,
-                d0: host,
-                em: path,
-                eo: port_,
-                et: protocol,
-                eu: query
+                d8: fragment,
+                ec: host,
+                eB: path,
+                eF: port_,
+                eK: protocol,
+                eL: query
             };
         });
     var $elm$core$String$contains = _String_contains;
     var $elm$core$String$length = _String_length;
     var $elm$core$String$slice = _String_slice;
     var $elm$core$String$dropLeft = F2(
         function(n, string) {
@@ -5217,15 +5217,15 @@
     var $author$project$Main$FetchData = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $author$project$Main$Hour = 1;
-    var $author$project$DeviceStatus$Idle = 1;
+    var $author$project$DeviceStatus$Idle = 2;
     var $elm$time$Time$Name = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $elm$time$Time$Offset = function(a) {
@@ -5244,35 +5244,46 @@
         });
     var $elm$time$Time$customZone = $elm$time$Time$Zone;
     var $elm$time$Time$Posix = $elm$core$Basics$identity;
     var $elm$time$Time$millisToPosix = $elm$core$Basics$identity;
     var $elm$time$Time$now = _Time_now($elm$time$Time$millisToPosix);
     var $author$project$Main$init = function(_v0) {
         return _Utils_Tuple2({
-                bm: _List_Nil,
-                bz: $elm$core$Maybe$Nothing,
-                dM: true,
-                bQ: _List_Nil,
-                az: {
-                    aM: 0,
-                    aY: 0.0,
-                    aZ: 0.0,
-                    cA: 0
+                bq: _List_Nil,
+                br: _List_Nil,
+                dW: $elm$core$Maybe$Nothing,
+                dX: true,
+                T: {
+                    ak: '',
+                    al: '',
+                    an: false
+                },
+                bW: _List_Nil,
+                bX: _List_Nil,
+                aE: {
+                    d1: 0.0,
+                    c_: 0,
+                    eD: 0.0,
+                    eE: 0.0,
+                    dq: 0
                 },
-                co: {
-                    ec: $elm$core$Maybe$Nothing,
-                    cy: 1
+                b$: $elm$core$Maybe$Nothing,
+                V: {
+                    dW: $elm$core$Maybe$Nothing,
+                    eo: $elm$core$Maybe$Nothing,
+                    ey: $elm$core$Maybe$Nothing,
+                    a2: 2
                 },
-                ac: 1
+                ae: 1
             },
             A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now));
     };
-    var $author$project$Main$FetchStatus = function(a) {
+    var $author$project$Main$Tick = function(a) {
         return {
-            $: 1,
+            $: 7,
             a: a
         };
     };
     var $elm$core$Platform$Sub$batch = _Platform_batch;
     var $elm$time$Time$Every = F2(
         function(a, b) {
             return {
@@ -5280,16 +5291,16 @@
                 a: a,
                 b: b
             };
         });
     var $elm$time$Time$State = F2(
         function(taggers, processes) {
             return {
-                es: processes,
-                eJ: taggers
+                eJ: processes,
+                e0: taggers
             };
         });
     var $elm$core$Dict$RBEmpty_elm_builtin = {
         $: -2
     };
     var $elm$core$Dict$empty = $elm$core$Dict$RBEmpty_elm_builtin;
     var $elm$time$Time$init = $elm$core$Task$succeed(
@@ -5569,15 +5580,15 @@
                         A3($elm$core$Dict$insert, interval, id, processes));
                 };
                 return A2($elm$core$Task$andThen, spawnRest, spawnTimer);
             }
         });
     var $elm$time$Time$onEffects = F3(
         function(router, subs, _v0) {
-            var processes = _v0.es;
+            var processes = _v0.eJ;
             var rightStep = F3(
                 function(_v6, id, _v7) {
                     var spawns = _v7.a;
                     var existing = _v7.b;
                     var kills = _v7.c;
                     return _Utils_Tuple3(
                         spawns,
@@ -5635,15 +5646,15 @@
                     function(_v2) {
                         return A3($elm$time$Time$spawnHelp, router, spawnList, existingDict);
                     },
                     killTask));
         });
     var $elm$time$Time$onSelfMsg = F3(
         function(router, interval, state) {
-            var _v0 = A2($elm$core$Dict$get, interval, state.eJ);
+            var _v0 = A2($elm$core$Dict$get, interval, state.e0);
             if (_v0.$ === 1) {
                 return $elm$core$Task$succeed(state);
             } else {
                 var taggers = _v0.a;
                 var tellTaggers = function(time) {
                     return $elm$core$Task$sequence(
                         A2(
@@ -5686,44 +5697,96 @@
                 A2($elm$time$Time$Every, interval, tagger));
         });
     var $author$project$Main$subscriptions = function(model) {
         return $elm$core$Platform$Sub$batch(
             _List_fromArray(
                 [
                     A2($elm$time$Time$every, 5000, $author$project$Main$FetchData),
-                    A2($elm$time$Time$every, 5000, $author$project$Main$FetchStatus)
+                    A2($elm$time$Time$every, 500, $author$project$Main$Tick)
                 ]));
     };
+    var $author$project$Main$FetchStatus = function(a) {
+        return {
+            $: 1,
+            a: a
+        };
+    };
+    var $author$project$Main$errorToString = function(error) {
+        switch (error.$) {
+            case 0:
+                var url = error.a;
+                return 'The URL ' + (url + ' was invalid');
+            case 1:
+                return 'Unable to reach the server, try again';
+            case 2:
+                return 'Unable to reach the server, check your network connection';
+            case 3:
+                switch (error.a) {
+                    case 500:
+                        return 'The server had a problem, try again later';
+                    case 400:
+                        return 'Verify your information and try again';
+                    default:
+                        return 'Unknown error';
+                }
+            default:
+                var errorMessage = error.a;
+                return errorMessage;
+        }
+    };
     var $author$project$Main$GotData = function(a) {
         return {
             $: 2,
             a: a
         };
     };
-    var $author$project$Main$ReadData = F4(
-        function(time, epa, pm25, pm10) {
+    var $author$project$Main$AllData = F2(
+        function(reads, epas) {
+            return {
+                c$: epas,
+                dr: reads
+            };
+        });
+    var $author$project$Main$EpaData = F2(
+        function(time, epa) {
             return {
-                aM: epa,
-                aY: pm10,
-                aZ: pm25,
-                cA: time
+                d1: epa,
+                cG: time
             };
         });
     var $elm$json$Json$Decode$field = _Json_decodeField;
     var $elm$json$Json$Decode$float = _Json_decodeFloat;
     var $elm$json$Json$Decode$list = _Json_decodeList;
-    var $elm$json$Json$Decode$map4 = _Json_map4;
-    var $author$project$Main$dataDecoder = $elm$json$Json$Decode$list(
-        A5(
-            $elm$json$Json$Decode$map4,
+    var $author$project$Main$epaDataDecoder = $elm$json$Json$Decode$list(
+        A3(
+            $elm$json$Json$Decode$map2,
+            $author$project$Main$EpaData,
+            A2($elm$json$Json$Decode$field, 't', $elm$json$Json$Decode$float),
+            A2($elm$json$Json$Decode$field, 'epa', $elm$json$Json$Decode$float)));
+    var $author$project$Main$ReadData = F3(
+        function(time, pm25, pm10) {
+            return {
+                eD: pm10,
+                eE: pm25,
+                cG: time
+            };
+        });
+    var $elm$json$Json$Decode$map3 = _Json_map3;
+    var $author$project$Main$readDataDecoder = $elm$json$Json$Decode$list(
+        A4(
+            $elm$json$Json$Decode$map3,
             $author$project$Main$ReadData,
             A2($elm$json$Json$Decode$field, 't', $elm$json$Json$Decode$float),
-            A2($elm$json$Json$Decode$field, 'epa', $elm$json$Json$Decode$float),
             A2($elm$json$Json$Decode$field, 'pm25', $elm$json$Json$Decode$float),
             A2($elm$json$Json$Decode$field, 'pm10', $elm$json$Json$Decode$float)));
+    var $author$project$Main$allDataDecoder = A3(
+        $elm$json$Json$Decode$map2,
+        $author$project$Main$AllData,
+        A2($elm$json$Json$Decode$field, 'reads', $author$project$Main$readDataDecoder),
+        A2($elm$json$Json$Decode$field, 'epas', $author$project$Main$epaDataDecoder));
     var $elm$json$Json$Decode$decodeString = _Json_runOnString;
     var $elm$http$Http$BadStatus_ = F2(
         function(a, b) {
             return {
                 $: 3,
                 a: a,
                 b: b
@@ -6197,15 +6260,15 @@
                 case 1:
                     return $elm$core$Result$Err($elm$http$Http$Timeout);
                 case 2:
                     return $elm$core$Result$Err($elm$http$Http$NetworkError);
                 case 3:
                     var metadata = response.a;
                     return $elm$core$Result$Err(
-                        $elm$http$Http$BadStatus(metadata.fT));
+                        $elm$http$Http$BadStatus(metadata.f8));
                 default:
                     var body = response.b;
                     return A2(
                         $elm$core$Result$mapError,
                         $elm$http$Http$BadBody,
                         toResult(body));
             }
@@ -6229,16 +6292,16 @@
             $: 1,
             a: a
         };
     };
     var $elm$http$Http$State = F2(
         function(reqs, subs) {
             return {
-                ew: reqs,
-                eI: subs
+                eP: reqs,
+                e$: subs
             };
         });
     var $elm$http$Http$init = $elm$core$Task$succeed(
         A2($elm$http$Http$State, $elm$core$Dict$empty, _List_Nil));
     var $elm$http$Http$updateReqs = F3(
         function(router, cmds, reqs) {
             updateReqs: while (true) {
@@ -6272,15 +6335,15 @@
                                 $elm$core$Process$kill(pid));
                         }
                     } else {
                         var req = cmd.a;
                         return A2(
                             $elm$core$Task$andThen,
                             function(pid) {
-                                var _v4 = req.eR;
+                                var _v4 = req.e8;
                                 if (_v4.$ === 1) {
                                     return A3($elm$http$Http$updateReqs, router, otherCmds, reqs);
                                 } else {
                                     var tracker = _v4.a;
                                     return A3(
                                         $elm$http$Http$updateReqs,
                                         router,
@@ -6302,15 +6365,15 @@
         function(router, cmds, subs, state) {
             return A2(
                 $elm$core$Task$andThen,
                 function(reqs) {
                     return $elm$core$Task$succeed(
                         A2($elm$http$Http$State, reqs, subs));
                 },
-                A3($elm$http$Http$updateReqs, router, cmds, state.ew));
+                A3($elm$http$Http$updateReqs, router, cmds, state.eP));
         });
     var $elm$core$List$maybeCons = F3(
         function(f, mx, xs) {
             var _v0 = f(mx);
             if (!_v0.$) {
                 var x = _v0.a;
                 return A2($elm$core$List$cons, x, xs);
@@ -6345,15 +6408,15 @@
                 function(_v1) {
                     return $elm$core$Task$succeed(state);
                 },
                 $elm$core$Task$sequence(
                     A2(
                         $elm$core$List$filterMap,
                         A3($elm$http$Http$maybeSend, router, tracker, progress),
-                        state.eI)));
+                        state.e$)));
         });
     var $elm$http$Http$Cancel = function(a) {
         return {
             $: 0,
             a: a
         };
     };
@@ -6361,22 +6424,22 @@
         function(func, cmd) {
             if (!cmd.$) {
                 var tracker = cmd.a;
                 return $elm$http$Http$Cancel(tracker);
             } else {
                 var r = cmd.a;
                 return $elm$http$Http$Request({
-                    e1: r.e1,
-                    e6: r.e6,
-                    dT: A2(_Http_mapExpect, func, r.dT),
-                    d_: r.d_,
-                    fC: r.fC,
-                    fY: r.fY,
-                    eR: r.eR,
-                    eU: r.eU
+                    fk: r.fk,
+                    fp: r.fp,
+                    d3: A2(_Http_mapExpect, func, r.d3),
+                    ea: r.ea,
+                    fU: r.fU,
+                    gd: r.gd,
+                    e8: r.e8,
+                    fb: r.fb
                 });
             }
         });
     var $elm$http$Http$MySub = F2(
         function(a, b) {
             return {
                 $: 0,
@@ -6395,33 +6458,33 @@
         });
     _Platform_effectManagers['Http'] = _Platform_createManager($elm$http$Http$init, $elm$http$Http$onEffects, $elm$http$Http$onSelfMsg, $elm$http$Http$cmdMap, $elm$http$Http$subMap);
     var $elm$http$Http$command = _Platform_leaf('Http');
     var $elm$http$Http$subscription = _Platform_leaf('Http');
     var $elm$http$Http$request = function(r) {
         return $elm$http$Http$command(
             $elm$http$Http$Request({
-                e1: false,
-                e6: r.e6,
-                dT: r.dT,
-                d_: r.d_,
-                fC: r.fC,
-                fY: r.fY,
-                eR: r.eR,
-                eU: r.eU
+                fk: false,
+                fp: r.fp,
+                d3: r.d3,
+                ea: r.ea,
+                fU: r.fU,
+                gd: r.gd,
+                e8: r.e8,
+                fb: r.fb
             }));
     };
     var $elm$http$Http$get = function(r) {
         return $elm$http$Http$request({
-            e6: $elm$http$Http$emptyBody,
-            dT: r.dT,
-            d_: _List_Nil,
-            fC: 'GET',
-            fY: $elm$core$Maybe$Nothing,
-            eR: $elm$core$Maybe$Nothing,
-            eU: r.eU
+            fp: $elm$http$Http$emptyBody,
+            d3: r.d3,
+            ea: _List_Nil,
+            fU: 'GET',
+            gd: $elm$core$Maybe$Nothing,
+            e8: $elm$core$Maybe$Nothing,
+            fb: r.fb
         });
     };
     var $author$project$Main$getData = function(windowDuration) {
         var stringDuration = function() {
             switch (windowDuration) {
                 case 0:
                     return 'all';
@@ -6430,192 +6493,1439 @@
                 case 2:
                     return 'day';
                 default:
                     return 'week';
             }
         }();
         return $elm$http$Http$get({
-            dT: A2($elm$http$Http$expectJson, $author$project$Main$GotData, $author$project$Main$dataDecoder),
-            eU: '/api/sensor_data?window=' + stringDuration
+            d3: A2($elm$http$Http$expectJson, $author$project$Main$GotData, $author$project$Main$allDataDecoder),
+            fb: '/api/sensor_data?window=' + stringDuration
         });
     };
     var $elm$core$List$head = function(list) {
         if (list.b) {
             var x = list.a;
             var xs = list.b;
             return $elm$core$Maybe$Just(x);
         } else {
             return $elm$core$Maybe$Nothing;
         }
     };
-    var $author$project$Main$getLastListItem = function(myList) {
-        var _v0 = $elm$core$List$head(
-            $elm$core$List$reverse(myList));
-        if (!_v0.$) {
-            var a = _v0.a;
-            return a;
-        } else {
-            return {
-                aM: 0,
-                aY: 0,
-                aZ: 0,
-                cA: 0
-            };
-        }
+    var $author$project$Main$getLastListItem = function(allData) {
+        var lastReads = function() {
+            var _v1 = $elm$core$List$head(
+                $elm$core$List$reverse(allData.dr));
+            if (!_v1.$) {
+                var a = _v1.a;
+                return a;
+            } else {
+                return {
+                    eD: 0,
+                    eE: 0,
+                    cG: 0
+                };
+            }
+        }();
+        var lastEpas = function() {
+            var _v0 = $elm$core$List$head(
+                $elm$core$List$reverse(allData.c$));
+            if (!_v0.$) {
+                var a = _v0.a;
+                return a;
+            } else {
+                return {
+                    d1: 0,
+                    cG: 0
+                };
+            }
+        }();
+        return {
+            d1: lastEpas.d1,
+            c_: lastEpas.cG,
+            eD: lastReads.eD,
+            eE: lastReads.eE,
+            dq: lastReads.cG
+        };
     };
     var $author$project$Main$GotStatus = function(a) {
         return {
             $: 3,
             a: a
         };
     };
-    var $author$project$DeviceStatus$DeviceInfo = F2(
-        function(state, lastException) {
+    var $author$project$Main$DeviceInfoResponse = F3(
+        function(readerStatus, readerException, nextSchedule) {
             return {
-                ec: lastException,
-                cy: state
+                ey: nextSchedule,
+                eM: readerException,
+                eN: readerStatus
             };
         });
+    var $elm$json$Json$Decode$int = _Json_decodeInt;
     var $elm$json$Json$Decode$oneOf = _Json_oneOf;
     var $elm$json$Json$Decode$maybe = function(decoder) {
         return $elm$json$Json$Decode$oneOf(
             _List_fromArray(
                 [
                     A2($elm$json$Json$Decode$map, $elm$core$Maybe$Just, decoder),
                     $elm$json$Json$Decode$succeed($elm$core$Maybe$Nothing)
                 ]));
     };
-    var $author$project$DeviceStatus$Failing = 2;
+    var $author$project$DeviceStatus$Failing = 3;
     var $author$project$DeviceStatus$Reading = 0;
+    var $author$project$DeviceStatus$WarmingUp = 1;
     var $elm$json$Json$Decode$andThen = _Json_andThen;
     var $elm$json$Json$Decode$fail = _Json_fail;
     var $elm$json$Json$Decode$string = _Json_decodeString;
     var $author$project$Main$stateDecoder = A2(
         $elm$json$Json$Decode$andThen,
         function(str) {
             switch (str) {
                 case 'IDLE':
+                    return $elm$json$Json$Decode$succeed(2);
+                case 'WARM_UP':
                     return $elm$json$Json$Decode$succeed(1);
                 case 'ERRORING':
-                    return $elm$json$Json$Decode$succeed(2);
+                    return $elm$json$Json$Decode$succeed(3);
                 case 'READING':
                     return $elm$json$Json$Decode$succeed(0);
                 default:
                     return $elm$json$Json$Decode$fail('Invalid DeviceState');
             }
         },
         $elm$json$Json$Decode$string);
-    var $author$project$Main$statusDecoder = A3(
-        $elm$json$Json$Decode$map2,
-        $author$project$DeviceStatus$DeviceInfo,
+    var $author$project$Main$statusDecoder = A4(
+        $elm$json$Json$Decode$map3,
+        $author$project$Main$DeviceInfoResponse,
         A2($elm$json$Json$Decode$field, 'reader_status', $author$project$Main$stateDecoder),
         $elm$json$Json$Decode$maybe(
-            A2($elm$json$Json$Decode$field, 'reader_exception', $elm$json$Json$Decode$string)));
+            A2($elm$json$Json$Decode$field, 'reader_exception', $elm$json$Json$Decode$string)),
+        $elm$json$Json$Decode$maybe(
+            A2($elm$json$Json$Decode$field, 'next_schedule', $elm$json$Json$Decode$int)));
     var $author$project$Main$getStatus = $elm$http$Http$get({
-        dT: A2($elm$http$Http$expectJson, $author$project$Main$GotStatus, $author$project$Main$statusDecoder),
-        eU: '/api/status'
+        d3: A2($elm$http$Http$expectJson, $author$project$Main$GotStatus, $author$project$Main$statusDecoder),
+        fb: '/api/status'
     });
+    var $elm$core$Maybe$map = F2(
+        function(f, maybe) {
+            if (!maybe.$) {
+                var value = maybe.a;
+                return $elm$core$Maybe$Just(
+                    f(value));
+            } else {
+                return $elm$core$Maybe$Nothing;
+            }
+        });
     var $elm$core$Platform$Cmd$batch = _Platform_batch;
     var $elm$core$Platform$Cmd$none = $elm$core$Platform$Cmd$batch(_List_Nil);
+    var $elm$time$Time$posixToMillis = function(_v0) {
+        var millis = _v0;
+        return millis;
+    };
+    var $author$project$Main$getDuration = F2(
+        function(currentTime, scheduledTime) {
+            var durationMillis = $elm$time$Time$posixToMillis(scheduledTime) - $elm$time$Time$posixToMillis(currentTime);
+            return durationMillis;
+        });
+    var $elm$core$Maybe$map2 = F3(
+        function(func, ma, mb) {
+            if (ma.$ === 1) {
+                return $elm$core$Maybe$Nothing;
+            } else {
+                var a = ma.a;
+                if (mb.$ === 1) {
+                    return $elm$core$Maybe$Nothing;
+                } else {
+                    var b = mb.a;
+                    return $elm$core$Maybe$Just(
+                        A2(func, a, b));
+                }
+            }
+        });
+    var $elm$core$Basics$negate = function(n) {
+        return -n;
+    };
+    var $elm$core$Maybe$withDefault = F2(
+        function(_default, maybe) {
+            if (!maybe.$) {
+                var value = maybe.a;
+                return value;
+            } else {
+                return _default;
+            }
+        });
+    var $author$project$Main$shouldFetchStatus = F2(
+        function(model, currentTime) {
+            var timeToNextRead = A2(
+                $elm$core$Maybe$withDefault,
+                1,
+                A3(
+                    $elm$core$Maybe$map2,
+                    $author$project$Main$getDuration,
+                    model.V.ey,
+                    $elm$core$Maybe$Just(currentTime)));
+            var maxTimeBetweenPolls = 15000;
+            var timeSinceLastPoll = A2(
+                $elm$core$Maybe$withDefault,
+                maxTimeBetweenPolls + 1,
+                A3(
+                    $elm$core$Maybe$map2,
+                    $author$project$Main$getDuration,
+                    model.b$,
+                    $elm$core$Maybe$Just(currentTime)));
+            return ((!model.V.a2) || (model.V.a2 === 1)) || ((_Utils_cmp(timeSinceLastPoll, maxTimeBetweenPolls) > 0) || (_Utils_cmp(timeToNextRead, -1) > 0));
+        });
     var $author$project$Main$update = F2(
         function(msg, model) {
             switch (msg.$) {
                 case 2:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    bm: data,
-                                    az: $author$project$Main$getLastListItem(data)
+                                    bq: data.c$,
+                                    br: data.dr,
+                                    T: {
+                                        ak: '',
+                                        al: '',
+                                        an: false
+                                    },
+                                    aE: $author$project$Main$getLastListItem(data)
                                 }),
                             $elm$core$Platform$Cmd$none);
                     } else {
                         var e = result.a;
-                        return _Utils_Tuple2(model, $elm$core$Platform$Cmd$none);
+                        return _Utils_Tuple2(
+                            _Utils_update(
+                                model, {
+                                    T: {
+                                        ak: $author$project$Main$errorToString(e),
+                                        al: 'Failed to retrieve read data',
+                                        an: true
+                                    }
+                                }),
+                            $elm$core$Platform$Cmd$none);
                     }
                 case 0:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bz: $elm$core$Maybe$Just(newTime)
+                                dW: $elm$core$Maybe$Just(newTime)
                             }),
-                        $author$project$Main$getData(model.ac));
+                        $author$project$Main$getData(model.ae));
                 case 3:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
+                        var deviceInfo = {
+                            dW: model.dW,
+                            eo: data.eM,
+                            ey: A2($elm$core$Maybe$map, $elm$time$Time$millisToPosix, data.ey),
+                            a2: data.eN
+                        };
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    co: data
+                                    T: {
+                                        ak: '',
+                                        al: '',
+                                        an: false
+                                    },
+                                    V: deviceInfo
                                 }),
                             $elm$core$Platform$Cmd$none);
                     } else {
                         var e = result.a;
-                        return _Utils_Tuple2(model, $elm$core$Platform$Cmd$none);
+                        return _Utils_Tuple2(
+                            _Utils_update(
+                                model, {
+                                    T: {
+                                        ak: $author$project$Main$errorToString(e),
+                                        al: 'Failed to retrieve device status',
+                                        an: true
+                                    }
+                                }),
+                            $elm$core$Platform$Cmd$none);
                     }
                 case 1:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bz: $elm$core$Maybe$Just(newTime)
+                                dW: $elm$core$Maybe$Just(newTime),
+                                b$: $elm$core$Maybe$Just(newTime)
                             }),
                         $author$project$Main$getStatus);
                 case 4:
                     var window = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                ac: window
+                                ae: window
                             }),
                         A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now));
-                default:
+                case 5:
+                    var hovering = msg.a;
+                    return _Utils_Tuple2(
+                        _Utils_update(
+                            model, {
+                                bX: hovering
+                            }),
+                        $elm$core$Platform$Cmd$none);
+                case 6:
                     var hovering = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bQ: hovering
+                                bW: hovering
                             }),
                         $elm$core$Platform$Cmd$none);
+                default:
+                    var newTime = msg.a;
+                    var readerState = model.V;
+                    var updatedReaderState = _Utils_update(
+                        readerState, {
+                            dW: $elm$core$Maybe$Just(newTime)
+                        });
+                    var cmd = A2($author$project$Main$shouldFetchStatus, model, newTime) ? A2($elm$core$Task$perform, $author$project$Main$FetchStatus, $elm$time$Time$now) : $elm$core$Platform$Cmd$none;
+                    return _Utils_Tuple2(
+                        _Utils_update(
+                            model, {
+                                dW: $elm$core$Maybe$Just(newTime),
+                                V: updatedReaderState
+                            }),
+                        cmd);
             }
         });
     var $author$project$Main$All = 0;
     var $author$project$Main$Day = 2;
-    var $author$project$Main$OnHover = function(a) {
+    var $author$project$Main$OnEpaHover = function(a) {
+        return {
+            $: 6,
+            a: a
+        };
+    };
+    var $author$project$Main$OnReadHover = function(a) {
         return {
             $: 5,
             a: a
         };
     };
     var $author$project$Main$Week = 3;
-    var $terezka$elm_charts$Internal$Svg$Start = 1;
-    var $terezka$elm_charts$Chart$Attributes$alignLeft = function(config) {
-        return _Utils_update(
-            config, {
-                i: $elm$core$Maybe$Just(1)
-            });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColAttrs = function(a) {
+        return {
+            $: 6,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs = function(attrs_) {
+        return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColAttrs(attrs_);
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowAttrs = function(a) {
         return {
             $: 2,
             a: a
         };
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs = function(attrs_) {
         return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowAttrs(attrs_);
     };
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$Center = 1;
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$MD = 2;
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$HAlign = F2(
+        function(screenSize, align) {
+            return {
+                dO: align,
+                eW: screenSize
+            };
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowHAlign = function(a) {
+        return {
+            $: 1,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowHAlign = F2(
+        function(size, align) {
+            return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowHAlign(
+                A2($rundis$elm_bootstrap$Bootstrap$General$Internal$HAlign, size, align));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowHAlign, 2, 1);
+    var $elm$json$Json$Encode$string = _Json_wrap;
+    var $elm$html$Html$Attributes$stringProperty = F2(
+        function(key, string) {
+            return A2(
+                _VirtualDom_property,
+                key,
+                $elm$json$Json$Encode$string(string));
+        });
+    var $elm$html$Html$Attributes$class = $elm$html$Html$Attributes$stringProperty('className');
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Column = function(a) {
+        return {
+            $: 0,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$col = F2(
+        function(options, children) {
+            return $rundis$elm_bootstrap$Bootstrap$Grid$Column({
+                dT: children,
+                dj: options
+            });
+        });
+    var $elm$html$Html$div = _VirtualDom_node('div');
+    var $rundis$elm_bootstrap$Bootstrap$Grid$container = F2(
+        function(attributes, children) {
+            return A2(
+                $elm$html$Html$div,
+                _Utils_ap(
+                    _List_fromArray(
+                        [
+                            $elm$html$Html$Attributes$class('container')
+                        ]),
+                    attributes),
+                children);
+        });
+    var $author$project$DeviceStatus$deviceStatusColor = function(deviceStatus) {
+        switch (deviceStatus) {
+            case 0:
+                return 'green';
+            case 1:
+                return 'orange';
+            case 2:
+                return 'gray';
+            default:
+                return 'red';
+        }
+    };
+    var $author$project$DeviceStatus$deviceStatusImage = function(deviceStatus) {
+        switch (deviceStatus) {
+            case 0:
+                return '/static/images/loading.gif';
+            case 1:
+                return '/static/images/loading.gif';
+            case 2:
+                return '/static/images/idle.png';
+            default:
+                return '/static/images/failing.png';
+        }
+    };
+    var $author$project$DeviceStatus$deviceStatusToString = function(deviceStatus) {
+        switch (deviceStatus) {
+            case 0:
+                return 'Reading';
+            case 1:
+                return 'Warming Up';
+            case 2:
+                return 'Idle';
+            default:
+                return 'Failing';
+        }
+    };
+    var $elm$core$Basics$modBy = _Basics_modBy;
+    var $elm$core$String$cons = _String_cons;
+    var $elm$core$String$fromChar = function(_char) {
+        return A2($elm$core$String$cons, _char, '');
+    };
+    var $elm$core$Bitwise$and = _Bitwise_and;
+    var $elm$core$Bitwise$shiftRightBy = _Bitwise_shiftRightBy;
+    var $elm$core$String$repeatHelp = F3(
+        function(n, chunk, result) {
+            return (n <= 0) ? result : A3(
+                $elm$core$String$repeatHelp,
+                n >> 1,
+                _Utils_ap(chunk, chunk),
+                (!(n & 1)) ? result : _Utils_ap(result, chunk));
+        });
+    var $elm$core$String$repeat = F2(
+        function(n, chunk) {
+            return A3($elm$core$String$repeatHelp, n, chunk, '');
+        });
+    var $elm$core$String$padLeft = F3(
+        function(n, _char, string) {
+            return _Utils_ap(
+                A2(
+                    $elm$core$String$repeat,
+                    n - $elm$core$String$length(string),
+                    $elm$core$String$fromChar(_char)),
+                string);
+        });
+    var $author$project$DeviceStatus$formatDuration = F2(
+        function(currentTime, scheduledTime) {
+            var durationMillis = $elm$time$Time$posixToMillis(scheduledTime) - $elm$time$Time$posixToMillis(currentTime);
+            var hour = (((((durationMillis / 1000) | 0) / 60) | 0) / 60) | 0;
+            var minute = A2($elm$core$Basics$modBy, 60, (((durationMillis / 1000) | 0) / 60) | 0);
+            var second = A2($elm$core$Basics$modBy, 60, (durationMillis / 1000) | 0);
+            return (durationMillis > 0) ? (A3(
+                $elm$core$String$padLeft,
+                2,
+                '0',
+                $elm$core$String$fromInt(hour)) + (':' + (A3(
+                $elm$core$String$padLeft,
+                2,
+                '0',
+                $elm$core$String$fromInt(minute)) + (':' + A3(
+                $elm$core$String$padLeft,
+                2,
+                '0',
+                $elm$core$String$fromInt(second)))))) : '00:00:00';
+        });
+    var $elm$html$Html$h5 = _VirtualDom_node('h5');
+    var $elm$virtual_dom$VirtualDom$text = _VirtualDom_text;
+    var $elm$html$Html$text = $elm$virtual_dom$VirtualDom$text;
+    var $author$project$DeviceStatus$htmlIf = F2(
+        function(el, cond) {
+            return cond ? el : $elm$html$Html$text('');
+        });
+    var $elm$html$Html$img = _VirtualDom_node('img');
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col = 0;
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width = F2(
+        function(screenSize, columnCount) {
+            return {
+                dV: columnCount,
+                eW: screenSize
+            };
+        });
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$XS = 0;
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign = F2(
+        function(align_, options) {
+            var _v0 = align_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            bp: $elm$core$Maybe$Just(align_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            bn: $elm$core$Maybe$Just(align_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            bm: $elm$core$Maybe$Just(align_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            bl: $elm$core$Maybe$Just(align_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            bo: $elm$core$Maybe$Just(align_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset = F2(
+        function(offset_, options) {
+            var _v0 = offset_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            ca: $elm$core$Maybe$Just(offset_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            b7: $elm$core$Maybe$Just(offset_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            b6: $elm$core$Maybe$Just(offset_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            b5: $elm$core$Maybe$Just(offset_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            b9: $elm$core$Maybe$Just(offset_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOrder = F2(
+        function(order_, options) {
+            var _v0 = order_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            ck: $elm$core$Maybe$Just(order_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            ci: $elm$core$Maybe$Just(order_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            ch: $elm$core$Maybe$Just(order_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            cg: $elm$core$Maybe$Just(order_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            cj: $elm$core$Maybe$Just(order_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPull = F2(
+        function(pull_, options) {
+            var _v0 = pull_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            cq: $elm$core$Maybe$Just(pull_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            co: $elm$core$Maybe$Just(pull_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            cn: $elm$core$Maybe$Just(pull_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            cm: $elm$core$Maybe$Just(pull_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            cp: $elm$core$Maybe$Just(pull_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPush = F2(
+        function(push_, options) {
+            var _v0 = push_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            cv: $elm$core$Maybe$Just(push_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            ct: $elm$core$Maybe$Just(push_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            cs: $elm$core$Maybe$Just(push_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            cr: $elm$core$Maybe$Just(push_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            cu: $elm$core$Maybe$Just(push_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth = F2(
+        function(width_, options) {
+            var _v0 = width_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            bd: $elm$core$Maybe$Just(width_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            bb: $elm$core$Maybe$Just(width_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            ba: $elm$core$Maybe$Just(width_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            a9: $elm$core$Maybe$Just(width_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            bc: $elm$core$Maybe$Just(width_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption = F2(
+        function(modifier, options) {
+            switch (modifier.$) {
+                case 6:
+                    var attrs = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bu: _Utils_ap(options.bu, attrs)
+                        });
+                case 0:
+                    var width_ = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth, width_, options);
+                case 1:
+                    var offset_ = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset, offset_, options);
+                case 2:
+                    var pull_ = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPull, pull_, options);
+                case 3:
+                    var push_ = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPush, push_, options);
+                case 4:
+                    var order_ = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOrder, order_, options);
+                case 5:
+                    var align = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign, align, options);
+                default:
+                    var align = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            cF: $elm$core$Maybe$Just(align)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$columnCountOption = function(size) {
+        switch (size) {
+            case 0:
+                return $elm$core$Maybe$Nothing;
+            case 1:
+                return $elm$core$Maybe$Just('1');
+            case 2:
+                return $elm$core$Maybe$Just('2');
+            case 3:
+                return $elm$core$Maybe$Just('3');
+            case 4:
+                return $elm$core$Maybe$Just('4');
+            case 5:
+                return $elm$core$Maybe$Just('5');
+            case 6:
+                return $elm$core$Maybe$Just('6');
+            case 7:
+                return $elm$core$Maybe$Just('7');
+            case 8:
+                return $elm$core$Maybe$Just('8');
+            case 9:
+                return $elm$core$Maybe$Just('9');
+            case 10:
+                return $elm$core$Maybe$Just('10');
+            case 11:
+                return $elm$core$Maybe$Just('11');
+            case 12:
+                return $elm$core$Maybe$Just('12');
+            default:
+                return $elm$core$Maybe$Just('auto');
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption = function(size) {
+        switch (size) {
+            case 0:
+                return $elm$core$Maybe$Nothing;
+            case 1:
+                return $elm$core$Maybe$Just('sm');
+            case 2:
+                return $elm$core$Maybe$Just('md');
+            case 3:
+                return $elm$core$Maybe$Just('lg');
+            default:
+                return $elm$core$Maybe$Just('xl');
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthClass = function(_v0) {
+        var screenSize = _v0.eW;
+        var columnCount = _v0.dV;
+        return $elm$html$Html$Attributes$class(
+            'col' + (A2(
+                $elm$core$Maybe$withDefault,
+                '',
+                A2(
+                    $elm$core$Maybe$map,
+                    function(v) {
+                        return '-' + v;
+                    },
+                    $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize))) + A2(
+                $elm$core$Maybe$withDefault,
+                '',
+                A2(
+                    $elm$core$Maybe$map,
+                    function(v) {
+                        return '-' + v;
+                    },
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$columnCountOption(columnCount)))));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthsToAttributes = function(widths) {
+        var width_ = function(w) {
+            return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthClass, w);
+        };
+        return A2(
+            $elm$core$List$filterMap,
+            $elm$core$Basics$identity,
+            A2($elm$core$List$map, width_, widths));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions = {
+        bl: $elm$core$Maybe$Nothing,
+        bm: $elm$core$Maybe$Nothing,
+        bn: $elm$core$Maybe$Nothing,
+        bo: $elm$core$Maybe$Nothing,
+        bp: $elm$core$Maybe$Nothing,
+        bu: _List_Nil,
+        b5: $elm$core$Maybe$Nothing,
+        b6: $elm$core$Maybe$Nothing,
+        b7: $elm$core$Maybe$Nothing,
+        b9: $elm$core$Maybe$Nothing,
+        ca: $elm$core$Maybe$Nothing,
+        cg: $elm$core$Maybe$Nothing,
+        ch: $elm$core$Maybe$Nothing,
+        ci: $elm$core$Maybe$Nothing,
+        cj: $elm$core$Maybe$Nothing,
+        ck: $elm$core$Maybe$Nothing,
+        cm: $elm$core$Maybe$Nothing,
+        cn: $elm$core$Maybe$Nothing,
+        co: $elm$core$Maybe$Nothing,
+        cp: $elm$core$Maybe$Nothing,
+        cq: $elm$core$Maybe$Nothing,
+        cr: $elm$core$Maybe$Nothing,
+        cs: $elm$core$Maybe$Nothing,
+        ct: $elm$core$Maybe$Nothing,
+        cu: $elm$core$Maybe$Nothing,
+        cv: $elm$core$Maybe$Nothing,
+        cF: $elm$core$Maybe$Nothing,
+        a9: $elm$core$Maybe$Nothing,
+        ba: $elm$core$Maybe$Nothing,
+        bb: $elm$core$Maybe$Nothing,
+        bc: $elm$core$Maybe$Nothing,
+        bd: $elm$core$Maybe$Nothing
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption = function(size) {
+        switch (size) {
+            case 0:
+                return '0';
+            case 1:
+                return '1';
+            case 2:
+                return '2';
+            case 3:
+                return '3';
+            case 4:
+                return '4';
+            case 5:
+                return '5';
+            case 6:
+                return '6';
+            case 7:
+                return '7';
+            case 8:
+                return '8';
+            case 9:
+                return '9';
+            case 10:
+                return '10';
+            default:
+                return '11';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString = function(screenSize) {
+        var _v0 = $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize);
+        if (!_v0.$) {
+            var s = _v0.a;
+            return '-' + (s + '-');
+        } else {
+            return '-';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass = function(_v0) {
+        var screenSize = _v0.eW;
+        var offsetCount = _v0.eA;
+        return $elm$html$Html$Attributes$class(
+            'offset' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption(offsetCount)));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes = function(offsets) {
+        var offset_ = function(m) {
+            return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass, m);
+        };
+        return A2(
+            $elm$core$List$filterMap,
+            $elm$core$Basics$identity,
+            A2($elm$core$List$map, offset_, offsets));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderColOption = function(size) {
+        switch (size) {
+            case 0:
+                return 'first';
+            case 1:
+                return '1';
+            case 2:
+                return '2';
+            case 3:
+                return '3';
+            case 4:
+                return '4';
+            case 5:
+                return '5';
+            case 6:
+                return '6';
+            case 7:
+                return '7';
+            case 8:
+                return '8';
+            case 9:
+                return '9';
+            case 10:
+                return '10';
+            case 11:
+                return '11';
+            case 12:
+                return '12';
+            default:
+                return 'last';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes = function(orders) {
+        var order_ = function(m) {
+            if (!m.$) {
+                var screenSize = m.a.eW;
+                var moveCount = m.a.aF;
+                return $elm$core$Maybe$Just(
+                    $elm$html$Html$Attributes$class(
+                        'order' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderColOption(moveCount))));
+            } else {
+                return $elm$core$Maybe$Nothing;
+            }
+        };
+        return A2(
+            $elm$core$List$filterMap,
+            $elm$core$Basics$identity,
+            A2($elm$core$List$map, order_, orders));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption = function(size) {
+        switch (size) {
+            case 0:
+                return '0';
+            case 1:
+                return '1';
+            case 2:
+                return '2';
+            case 3:
+                return '3';
+            case 4:
+                return '4';
+            case 5:
+                return '5';
+            case 6:
+                return '6';
+            case 7:
+                return '7';
+            case 8:
+                return '8';
+            case 9:
+                return '9';
+            case 10:
+                return '10';
+            case 11:
+                return '11';
+            default:
+                return '12';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes = function(pulls) {
+        var pull_ = function(m) {
+            if (!m.$) {
+                var screenSize = m.a.eW;
+                var moveCount = m.a.aF;
+                return $elm$core$Maybe$Just(
+                    $elm$html$Html$Attributes$class(
+                        'pull' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
+            } else {
+                return $elm$core$Maybe$Nothing;
+            }
+        };
+        return A2(
+            $elm$core$List$filterMap,
+            $elm$core$Basics$identity,
+            A2($elm$core$List$map, pull_, pulls));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes = function(pushes) {
+        var push_ = function(m) {
+            if (!m.$) {
+                var screenSize = m.a.eW;
+                var moveCount = m.a.aF;
+                return $elm$core$Maybe$Just(
+                    $elm$html$Html$Attributes$class(
+                        'push' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
+            } else {
+                return $elm$core$Maybe$Nothing;
+            }
+        };
+        return A2(
+            $elm$core$List$filterMap,
+            $elm$core$Basics$identity,
+            A2($elm$core$List$map, push_, pushes));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignDirOption = function(dir) {
+        switch (dir) {
+            case 1:
+                return 'center';
+            case 0:
+                return 'left';
+            default:
+                return 'right';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass = function(_v0) {
+        var dir = _v0.d_;
+        var size = _v0.eZ;
+        return $elm$html$Html$Attributes$class(
+            'text' + (A2(
+                $elm$core$Maybe$withDefault,
+                '-',
+                A2(
+                    $elm$core$Maybe$map,
+                    function(s) {
+                        return '-' + (s + '-');
+                    },
+                    $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(size))) + $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignDirOption(dir)));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$verticalAlignOption = function(align) {
+        switch (align) {
+            case 0:
+                return 'start';
+            case 1:
+                return 'center';
+            default:
+                return 'end';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignClass = F2(
+        function(prefix, _v0) {
+            var align = _v0.dO;
+            var screenSize = _v0.eW;
+            return $elm$html$Html$Attributes$class(
+                _Utils_ap(
+                    prefix,
+                    _Utils_ap(
+                        A2(
+                            $elm$core$Maybe$withDefault,
+                            '',
+                            A2(
+                                $elm$core$Maybe$map,
+                                function(v) {
+                                    return v + '-';
+                                },
+                                $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize))),
+                        $rundis$elm_bootstrap$Bootstrap$Grid$Internal$verticalAlignOption(align))));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes = F2(
+        function(prefix, aligns) {
+            var align = function(a) {
+                return A2(
+                    $elm$core$Maybe$map,
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignClass(prefix),
+                    a);
+            };
+            return A2(
+                $elm$core$List$filterMap,
+                $elm$core$Basics$identity,
+                A2($elm$core$List$map, align, aligns));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes = function(modifiers) {
+        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions, modifiers);
+        var shouldAddDefaultXs = !$elm$core$List$length(
+            A2(
+                $elm$core$List$filterMap,
+                $elm$core$Basics$identity,
+                _List_fromArray(
+                    [options.bd, options.bb, options.ba, options.a9, options.bc])));
+        return _Utils_ap(
+            $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthsToAttributes(
+                _List_fromArray(
+                    [
+                        shouldAddDefaultXs ? $elm$core$Maybe$Just(
+                            A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, 0, 0)) : options.bd,
+                        options.bb,
+                        options.ba,
+                        options.a9,
+                        options.bc
+                    ])),
+            _Utils_ap(
+                $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes(
+                    _List_fromArray(
+                        [options.ca, options.b7, options.b6, options.b5, options.b9])),
+                _Utils_ap(
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes(
+                        _List_fromArray(
+                            [options.cq, options.co, options.cn, options.cm, options.cp])),
+                    _Utils_ap(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes(
+                            _List_fromArray(
+                                [options.cv, options.ct, options.cs, options.cr, options.cu])),
+                        _Utils_ap(
+                            $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes(
+                                _List_fromArray(
+                                    [options.ck, options.ci, options.ch, options.cg, options.cj])),
+                            _Utils_ap(
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
+                                    'align-self-',
+                                    _List_fromArray(
+                                        [options.bp, options.bn, options.bm, options.bl, options.bo])),
+                                _Utils_ap(
+                                    function() {
+                                        var _v0 = options.cF;
+                                        if (!_v0.$) {
+                                            var a = _v0.a;
+                                            return _List_fromArray(
+                                                [
+                                                    $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass(a)
+                                                ]);
+                                        } else {
+                                            return _List_Nil;
+                                        }
+                                    }(),
+                                    options.bu)))))));
+    };
+    var $elm$virtual_dom$VirtualDom$keyedNode = function(tag) {
+        return _VirtualDom_keyedNode(
+            _VirtualDom_noScript(tag));
+    };
+    var $elm$html$Html$Keyed$node = $elm$virtual_dom$VirtualDom$keyedNode;
+    var $rundis$elm_bootstrap$Bootstrap$Grid$renderCol = function(column) {
+        switch (column.$) {
+            case 0:
+                var options = column.a.dj;
+                var children = column.a.dT;
+                return A2(
+                    $elm$html$Html$div,
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
+                    children);
+            case 1:
+                var e = column.a;
+                return e;
+            default:
+                var options = column.a.dj;
+                var children = column.a.dT;
+                return A3(
+                    $elm$html$Html$Keyed$node,
+                    'div',
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
+                    children);
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign = F2(
+        function(align, options) {
+            var _v0 = align.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            bT: $elm$core$Maybe$Just(align)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            bR: $elm$core$Maybe$Just(align)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            bQ: $elm$core$Maybe$Just(align)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            bP: $elm$core$Maybe$Just(align)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            bS: $elm$core$Maybe$Just(align)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign = F2(
+        function(align_, options) {
+            var _v0 = align_.eW;
+            switch (_v0) {
+                case 0:
+                    return _Utils_update(
+                        options, {
+                            cP: $elm$core$Maybe$Just(align_)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            cN: $elm$core$Maybe$Just(align_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            cM: $elm$core$Maybe$Just(align_)
+                        });
+                case 3:
+                    return _Utils_update(
+                        options, {
+                            cL: $elm$core$Maybe$Just(align_)
+                        });
+                default:
+                    return _Utils_update(
+                        options, {
+                            cO: $elm$core$Maybe$Just(align_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowOption = F2(
+        function(modifier, options) {
+            switch (modifier.$) {
+                case 2:
+                    var attrs = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bu: _Utils_ap(options.bu, attrs)
+                        });
+                case 0:
+                    var align = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign, align, options);
+                default:
+                    var align = modifier.a;
+                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign, align, options);
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultRowOptions = {
+        bu: _List_Nil,
+        bP: $elm$core$Maybe$Nothing,
+        bQ: $elm$core$Maybe$Nothing,
+        bR: $elm$core$Maybe$Nothing,
+        bS: $elm$core$Maybe$Nothing,
+        bT: $elm$core$Maybe$Nothing,
+        cL: $elm$core$Maybe$Nothing,
+        cM: $elm$core$Maybe$Nothing,
+        cN: $elm$core$Maybe$Nothing,
+        cO: $elm$core$Maybe$Nothing,
+        cP: $elm$core$Maybe$Nothing
+    };
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$horizontalAlignOption = function(align) {
+        switch (align) {
+            case 0:
+                return 'start';
+            case 1:
+                return 'center';
+            case 2:
+                return 'end';
+            case 3:
+                return 'around';
+            default:
+                return 'between';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$hAlignClass = function(_v0) {
+        var align = _v0.dO;
+        var screenSize = _v0.eW;
+        return $elm$html$Html$Attributes$class(
+            'justify-content-' + (A2(
+                $elm$core$Maybe$withDefault,
+                '',
+                A2(
+                    $elm$core$Maybe$map,
+                    function(v) {
+                        return v + '-';
+                    },
+                    $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize))) + $rundis$elm_bootstrap$Bootstrap$General$Internal$horizontalAlignOption(align)));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$hAlignsToAttributes = function(aligns) {
+        var align = function(a) {
+            return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$General$Internal$hAlignClass, a);
+        };
+        return A2(
+            $elm$core$List$filterMap,
+            $elm$core$Basics$identity,
+            A2($elm$core$List$map, align, aligns));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowAttributes = function(modifiers) {
+        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowOption, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultRowOptions, modifiers);
+        return _Utils_ap(
+            _List_fromArray(
+                [
+                    $elm$html$Html$Attributes$class('row')
+                ]),
+            _Utils_ap(
+                A2(
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
+                    'align-items-',
+                    _List_fromArray(
+                        [options.cP, options.cN, options.cM, options.cL, options.cO])),
+                _Utils_ap(
+                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$hAlignsToAttributes(
+                        _List_fromArray(
+                            [options.bT, options.bR, options.bQ, options.bP, options.bS])),
+                    options.bu)));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$row = F2(
+        function(options, cols) {
+            return A2(
+                $elm$html$Html$div,
+                $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowAttributes(options),
+                A2($elm$core$List$map, $rundis$elm_bootstrap$Bootstrap$Grid$renderCol, cols));
+        });
+    var $author$project$DeviceStatus$shouldShowTimer = function(deviceState) {
+        return (deviceState === 2) || (deviceState === 3);
+    };
+    var $elm$html$Html$Attributes$src = function(url) {
+        return A2(
+            $elm$html$Html$Attributes$stringProperty,
+            'src',
+            _VirtualDom_noJavaScriptOrHtmlUri(url));
+    };
+    var $elm$virtual_dom$VirtualDom$style = _VirtualDom_style;
+    var $elm$html$Html$Attributes$style = $elm$virtual_dom$VirtualDom$style;
+    var $author$project$DeviceStatus$getDeviceInfo = function(deviceInfo) {
+        return A2(
+            $rundis$elm_bootstrap$Bootstrap$Grid$container,
+            _List_Nil,
+            _List_fromArray(
+                [
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_fromArray(
+                            [
+                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$Attributes$class('align-items-center')
+                                        ]))
+                            ]),
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'max-width', '64px'),
+                                                        A2($elm$html$Html$Attributes$style, 'margin-right', '1em')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $elm$html$Html$img,
+                                                _List_fromArray(
+                                                    [
+                                                        $elm$html$Html$Attributes$src(
+                                                            $author$project$DeviceStatus$deviceStatusImage(deviceInfo.a2))
+                                                    ]),
+                                                _List_Nil)
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                                _List_Nil,
+                                                _List_fromArray(
+                                                    [
+                                                        A2(
+                                                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                            _List_Nil,
+                                                            _List_fromArray(
+                                                                [
+                                                                    A2(
+                                                                        $elm$html$Html$h5,
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                A2(
+                                                                                    $elm$html$Html$Attributes$style,
+                                                                                    'color',
+                                                                                    $author$project$DeviceStatus$deviceStatusColor(deviceInfo.a2))
+                                                                            ]),
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                $elm$html$Html$text(
+                                                                                    $author$project$DeviceStatus$deviceStatusToString(deviceInfo.a2))
+                                                                            ]))
+                                                                ]))
+                                                    ])),
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                                _List_Nil,
+                                                _List_fromArray(
+                                                    [
+                                                        A2(
+                                                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                            _List_Nil,
+                                                            _List_fromArray(
+                                                                [
+                                                                    $elm$html$Html$text(
+                                                                        A2($elm$core$Maybe$withDefault, '', deviceInfo.eo))
+                                                                ]))
+                                                    ])),
+                                            A2(
+                                                $author$project$DeviceStatus$htmlIf,
+                                                A2(
+                                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                                    _List_Nil,
+                                                    _List_fromArray(
+                                                        [
+                                                            A2(
+                                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                                _List_Nil,
+                                                                _List_fromArray(
+                                                                    [
+                                                                        $elm$html$Html$text(
+                                                                            'Next read in: ' + A2(
+                                                                                $elm$core$Maybe$withDefault,
+                                                                                '',
+                                                                                A3($elm$core$Maybe$map2, $author$project$DeviceStatus$formatDuration, deviceInfo.dW, deviceInfo.ey)))
+                                                                    ]))
+                                                        ])),
+                                                $author$project$DeviceStatus$shouldShowTimer(deviceInfo.a2))
+                                        ]))
+                            ]))
+                ]));
+    };
+    var $terezka$elm_charts$Internal$Svg$Start = 1;
+    var $terezka$elm_charts$Chart$Attributes$alignLeft = function(config) {
+        return _Utils_update(
+            config, {
+                i: $elm$core$Maybe$Just(1)
+            });
+    };
     var $terezka$elm_charts$Chart$Attributes$background = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    e4: v
+                    fn: v
                 });
         });
     var $terezka$elm_charts$Internal$Helpers$blue = '#12A5ED';
     var $terezka$elm_charts$Chart$Attributes$blue = $terezka$elm_charts$Internal$Helpers$blue;
     var $terezka$elm_charts$Chart$Attributes$border = F2(
         function(v, config) {
             return _Utils_update(
@@ -6626,40 +7936,19 @@
     var $terezka$elm_charts$Chart$Attributes$borderWidth = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
                     x: v
                 });
         });
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$Center = 1;
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$MD = 2;
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$HAlign = F2(
-        function(screenSize, align) {
-            return {
-                dE: align,
-                eD: screenSize
-            };
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowHAlign = function(a) {
-        return {
-            $: 1,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowHAlign = F2(
-        function(size, align) {
-            return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowHAlign(
-                A2($rundis$elm_bootstrap$Bootstrap$General$Internal$HAlign, size, align));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowHAlign, 2, 1);
     var $terezka$elm_charts$Internal$Svg$Event = F2(
         function(name, handler) {
             return {
-                dZ: handler,
-                fF: name
+                d9: handler,
+                fW: name
             };
         });
     var $elm$core$List$any = F2(
         function(isOkay, list) {
             any: while (true) {
                 if (!list.b) {
                     return false;
@@ -6682,28 +7971,19 @@
         function(funcs, _default) {
             var apply_ = F2(
                 function(f, a) {
                     return f(a);
                 });
             return A3($elm$core$List$foldl, apply_, _default, funcs);
         });
-    var $elm$json$Json$Encode$string = _Json_wrap;
-    var $elm$html$Html$Attributes$stringProperty = F2(
-        function(key, string) {
-            return A2(
-                _VirtualDom_property,
-                key,
-                $elm$json$Json$Encode$string(string));
-        });
-    var $elm$html$Html$Attributes$class = $elm$html$Html$Attributes$stringProperty('className');
     var $elm$svg$Svg$trustedNode = _VirtualDom_nodeNS('http://www.w3.org/2000/svg');
     var $elm$svg$Svg$clipPath = $elm$svg$Svg$trustedNode('clipPath');
-    var $elm$json$Json$Decode$map3 = _Json_map3;
     var $debois$elm_dom$DOM$offsetHeight = A2($elm$json$Json$Decode$field, 'offsetHeight', $elm$json$Json$Decode$float);
     var $debois$elm_dom$DOM$offsetWidth = A2($elm$json$Json$Decode$field, 'offsetWidth', $elm$json$Json$Decode$float);
+    var $elm$json$Json$Decode$map4 = _Json_map4;
     var $debois$elm_dom$DOM$offsetLeft = A2($elm$json$Json$Decode$field, 'offsetLeft', $elm$json$Json$Decode$float);
     var $elm$json$Json$Decode$null = _Json_decodeNull;
     var $debois$elm_dom$DOM$offsetParent = F2(
         function(x, decoder) {
             return $elm$json$Json$Decode$oneOf(
                 _List_fromArray(
                     [
@@ -6743,18 +8023,18 @@
     var $debois$elm_dom$DOM$boundingClientRect = A4(
         $elm$json$Json$Decode$map3,
         F3(
             function(_v0, width, height) {
                 var x = _v0.a;
                 var y = _v0.b;
                 return {
-                    d$: height,
-                    ed: x,
-                    eQ: y,
-                    eY: width
+                    eb: height,
+                    ep: x,
+                    e7: y,
+                    ff: width
                 };
             }),
         A2($debois$elm_dom$DOM$position, 0, 0),
         $debois$elm_dom$DOM$offsetWidth,
         $debois$elm_dom$DOM$offsetHeight);
     var $elm$json$Json$Decode$lazy = function(thunk) {
         return A2(
@@ -6779,92 +8059,91 @@
                 ]));
     }
     var $terezka$elm_charts$Internal$Svg$decodePosition = $terezka$elm_charts$Internal$Svg$cyclic$decodePosition();
     $terezka$elm_charts$Internal$Svg$cyclic$decodePosition = function() {
         return $terezka$elm_charts$Internal$Svg$decodePosition;
     };
     var $terezka$elm_charts$Internal$Coordinates$innerLength = function(axis) {
-        return A2($elm$core$Basics$max, 1, (axis.N - axis.fA) - axis.fz);
+        return A2($elm$core$Basics$max, 1, (axis.N - axis.fT) - axis.fS);
     };
     var $terezka$elm_charts$Internal$Coordinates$innerWidth = function(plane) {
-        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.eZ);
+        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fg);
     };
     var $terezka$elm_charts$Internal$Coordinates$range = function(axis) {
-        var diff = axis.fB - axis.fD;
+        var diff = axis.er - axis.et;
         return (diff > 0) ? diff : 1;
     };
     var $terezka$elm_charts$Internal$Coordinates$scaleCartesianX = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.eZ)) / $terezka$elm_charts$Internal$Coordinates$innerWidth(plane);
+            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fg)) / $terezka$elm_charts$Internal$Coordinates$innerWidth(plane);
         });
     var $terezka$elm_charts$Internal$Coordinates$toCartesianX = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, value - plane.eZ.fA) + plane.eZ.fD;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, value - plane.fg.fT) + plane.fg.et;
         });
     var $terezka$elm_charts$Internal$Coordinates$innerHeight = function(plane) {
-        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.e_);
+        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fh);
     };
     var $terezka$elm_charts$Internal$Coordinates$scaleCartesianY = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.e_)) / $terezka$elm_charts$Internal$Coordinates$innerHeight(plane);
+            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fh)) / $terezka$elm_charts$Internal$Coordinates$innerHeight(plane);
         });
     var $terezka$elm_charts$Internal$Coordinates$toCartesianY = F2(
         function(plane, value) {
-            return ($terezka$elm_charts$Internal$Coordinates$range(plane.e_) - A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, value - plane.e_.fA)) + plane.e_.fD;
+            return ($terezka$elm_charts$Internal$Coordinates$range(plane.fh) - A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, value - plane.fh.fT)) + plane.fh.et;
         });
     var $terezka$elm_charts$Internal$Svg$fromSvg = F2(
         function(plane, point) {
             return {
-                eZ: A2($terezka$elm_charts$Internal$Coordinates$toCartesianX, plane, point.eZ),
-                e_: A2($terezka$elm_charts$Internal$Coordinates$toCartesianY, plane, point.e_)
+                fg: A2($terezka$elm_charts$Internal$Coordinates$toCartesianX, plane, point.fg),
+                fh: A2($terezka$elm_charts$Internal$Coordinates$toCartesianY, plane, point.fh)
             };
         });
     var $debois$elm_dom$DOM$target = function(decoder) {
         return A2($elm$json$Json$Decode$field, 'target', decoder);
     };
     var $terezka$elm_charts$Internal$Svg$decoder = F2(
         function(plane, toMsg) {
             var handle = F3(
                 function(mouseX, mouseY, box) {
-                    var yPrev = plane.e_;
-                    var xPrev = plane.eZ;
-                    var widthPercent = box.eY / plane.eZ.N;
-                    var heightPercent = box.d$ / plane.e_.N;
+                    var yPrev = plane.fh;
+                    var xPrev = plane.fg;
+                    var widthPercent = box.ff / plane.fg.N;
+                    var heightPercent = box.eb / plane.fh.N;
                     var newPlane = _Utils_update(
                         plane, {
-                            eZ: _Utils_update(
+                            fg: _Utils_update(
                                 xPrev, {
-                                    N: box.eY,
-                                    fz: plane.eZ.fz * widthPercent,
-                                    fA: plane.eZ.fA * widthPercent
+                                    N: box.ff,
+                                    fS: plane.fg.fS * widthPercent,
+                                    fT: plane.fg.fT * widthPercent
                                 }),
-                            e_: _Utils_update(
+                            fh: _Utils_update(
                                 yPrev, {
-                                    N: box.d$,
-                                    fz: plane.e_.fz * heightPercent,
-                                    fA: plane.e_.fA * heightPercent
+                                    N: box.eb,
+                                    fS: plane.fh.fS * heightPercent,
+                                    fT: plane.fh.fT * heightPercent
                                 })
                         });
                     var searched = A2(
                         $terezka$elm_charts$Internal$Svg$fromSvg,
                         newPlane, {
-                            eZ: mouseX - box.ed,
-                            e_: mouseY - box.eQ
+                            fg: mouseX - box.ep,
+                            fh: mouseY - box.e7
                         });
                     return A2(toMsg, newPlane, searched);
                 });
             return A4(
                 $elm$json$Json$Decode$map3,
                 handle,
                 A2($elm$json$Json$Decode$field, 'pageX', $elm$json$Json$Decode$float),
                 A2($elm$json$Json$Decode$field, 'pageY', $elm$json$Json$Decode$float),
                 $debois$elm_dom$DOM$target($terezka$elm_charts$Internal$Svg$decodePosition));
         });
     var $elm$svg$Svg$defs = $elm$svg$Svg$trustedNode('defs');
-    var $elm$html$Html$div = _VirtualDom_node('div');
     var $elm$svg$Svg$Attributes$fill = _VirtualDom_attribute('fill');
     var $elm$core$String$fromFloat = _String_fromNumber;
     var $elm$svg$Svg$Attributes$height = _VirtualDom_attribute('height');
     var $elm$svg$Svg$Attributes$id = _VirtualDom_attribute('id');
     var $elm$virtual_dom$VirtualDom$Normal = function(a) {
         return {
             $: 0,
@@ -6877,16 +8156,14 @@
             return A2(
                 $elm$virtual_dom$VirtualDom$on,
                 event,
                 $elm$virtual_dom$VirtualDom$Normal(decoder));
         });
     var $elm$svg$Svg$Events$on = $elm$html$Html$Events$on;
     var $elm$svg$Svg$rect = $elm$svg$Svg$trustedNode('rect');
-    var $elm$virtual_dom$VirtualDom$style = _VirtualDom_style;
-    var $elm$html$Html$Attributes$style = $elm$virtual_dom$VirtualDom$style;
     var $elm$svg$Svg$svg = $elm$svg$Svg$trustedNode('svg');
     var $elm$core$String$replace = F3(
         function(before, after, string) {
             return A2(
                 $elm$core$String$join,
                 after,
                 A2($elm$core$String$split, before, string));
@@ -6898,79 +8175,79 @@
             A2($elm$core$String$replace, '.', '-'));
         return A2(
             $elm$core$String$join,
             '_',
             _List_fromArray(
                 [
                     'elm-charts__id',
-                    numToStr(plane.eZ.N),
-                    numToStr(plane.eZ.fD),
-                    numToStr(plane.eZ.fB),
-                    numToStr(plane.eZ.fA),
-                    numToStr(plane.eZ.fz),
-                    numToStr(plane.e_.N),
-                    numToStr(plane.e_.fD),
-                    numToStr(plane.e_.fB),
-                    numToStr(plane.e_.fA),
-                    numToStr(plane.e_.fz)
+                    numToStr(plane.fg.N),
+                    numToStr(plane.fg.et),
+                    numToStr(plane.fg.er),
+                    numToStr(plane.fg.fT),
+                    numToStr(plane.fg.fS),
+                    numToStr(plane.fh.N),
+                    numToStr(plane.fh.et),
+                    numToStr(plane.fh.er),
+                    numToStr(plane.fh.fT),
+                    numToStr(plane.fh.fS)
                 ]));
     };
     var $elm$svg$Svg$Attributes$viewBox = _VirtualDom_attribute('viewBox');
     var $elm$svg$Svg$Attributes$width = _VirtualDom_attribute('width');
     var $elm$svg$Svg$Attributes$x = _VirtualDom_attribute('x');
     var $elm$svg$Svg$Attributes$y = _VirtualDom_attribute('y');
     var $terezka$elm_charts$Internal$Svg$container = F5(
         function(plane, config, below, chartEls, above) {
             var toEvent = function(event) {
                 return A2(
                     $elm$svg$Svg$Events$on,
-                    event.fF,
-                    A2($terezka$elm_charts$Internal$Svg$decoder, plane, event.dZ));
+                    event.fW,
+                    A2($terezka$elm_charts$Internal$Svg$decoder, plane, event.d9));
             };
-            var svgAttrsSize = config.cq ? _List_fromArray(
+            var svgAttrsSize = config.cx ? _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$viewBox(
-                        '0 0 ' + ($elm$core$String$fromFloat(plane.eZ.N) + (' ' + $elm$core$String$fromFloat(plane.e_.N)))),
+                        '0 0 ' + ($elm$core$String$fromFloat(plane.fg.N) + (' ' + $elm$core$String$fromFloat(plane.fh.N)))),
                     A2($elm$html$Html$Attributes$style, 'display', 'block')
                 ]) : _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$width(
-                        $elm$core$String$fromFloat(plane.eZ.N)),
+                        $elm$core$String$fromFloat(plane.fg.N)),
                     $elm$svg$Svg$Attributes$height(
-                        $elm$core$String$fromFloat(plane.e_.N)),
+                        $elm$core$String$fromFloat(plane.fh.N)),
                     A2($elm$html$Html$Attributes$style, 'display', 'block')
                 ]);
-            var htmlAttrsSize = config.cq ? _List_fromArray(
+            var htmlAttrsSize = config.cx ? _List_fromArray(
                 [
                     A2($elm$html$Html$Attributes$style, 'width', '100%'),
                     A2($elm$html$Html$Attributes$style, 'height', '100%')
                 ]) : _List_fromArray(
                 [
                     A2(
                         $elm$html$Html$Attributes$style,
                         'width',
-                        $elm$core$String$fromFloat(plane.eZ.N) + 'px'),
+                        $elm$core$String$fromFloat(plane.fg.N) + 'px'),
                     A2(
                         $elm$html$Html$Attributes$style,
                         'height',
-                        $elm$core$String$fromFloat(plane.e_.N) + 'px')
+                        $elm$core$String$fromFloat(plane.fh.N) + 'px')
                 ]);
             var htmlAttrsDef = _List_fromArray(
                 [
                     $elm$html$Html$Attributes$class('elm-charts__container-inner')
                 ]);
             var htmlAttrs = _Utils_ap(
-                config.bR,
+                config.bY,
                 _Utils_ap(htmlAttrsDef, htmlAttrsSize));
             var chartPosition = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$x(
-                        $elm$core$String$fromFloat(plane.eZ.fA)),
+                        $elm$core$String$fromFloat(plane.fg.fT)),
                     $elm$svg$Svg$Attributes$y(
-                        $elm$core$String$fromFloat(plane.e_.fA)),
+                        $elm$core$String$fromFloat(plane.fh.fT)),
                     $elm$svg$Svg$Attributes$width(
                         $elm$core$String$fromFloat(
                             $terezka$elm_charts$Internal$Coordinates$innerWidth(plane))),
                     $elm$svg$Svg$Attributes$height(
                         $elm$core$String$fromFloat(
                             $terezka$elm_charts$Internal$Coordinates$innerHeight(plane))),
                     $elm$svg$Svg$Attributes$fill('transparent')
@@ -6992,19 +8269,19 @@
                                     A2($elm$svg$Svg$rect, chartPosition, _List_Nil)
                                 ]))
                     ]));
             var catcher = A2(
                 $elm$svg$Svg$rect,
                 _Utils_ap(
                     chartPosition,
-                    A2($elm$core$List$map, toEvent, config.bH)),
+                    A2($elm$core$List$map, toEvent, config.bM)),
                 _List_Nil);
             var chart = A2(
                 $elm$svg$Svg$svg,
-                _Utils_ap(svgAttrsSize, config.bq),
+                _Utils_ap(svgAttrsSize, config.bv),
                 _Utils_ap(
                     _List_fromArray(
                         [clipPathDefs]),
                     _Utils_ap(
                         chartEls,
                         _List_fromArray(
                             [catcher]))));
@@ -7027,56 +8304,47 @@
                                         [chart]),
                                     above)))
                     ]));
         });
     var $terezka$elm_charts$Internal$Coordinates$Position = F4(
         function(x1, x2, y1, y2) {
             return {
-                aF: x1,
-                bb: x2,
-                gg: y1,
-                dB: y2
+                aK: x1,
+                bf: x2,
+                gx: y1,
+                dL: y2
             };
         });
     var $elm$core$Basics$min = F2(
         function(x, y) {
             return (_Utils_cmp(x, y) < 0) ? x : y;
         });
-    var $elm$core$Maybe$withDefault = F2(
-        function(_default, maybe) {
-            if (!maybe.$) {
-                var value = maybe.a;
-                return value;
-            } else {
-                return _default;
-            }
-        });
     var $terezka$elm_charts$Internal$Coordinates$foldPosition = F2(
         function(func, data) {
             var fold = F2(
                 function(datum, posM) {
                     if (!posM.$) {
                         var pos = posM.a;
                         return $elm$core$Maybe$Just({
-                            aF: A2(
+                            aK: A2(
                                 $elm$core$Basics$min,
-                                func(datum).aF,
-                                pos.aF),
-                            bb: A2(
+                                func(datum).aK,
+                                pos.aK),
+                            bf: A2(
                                 $elm$core$Basics$max,
-                                func(datum).bb,
-                                pos.bb),
-                            gg: A2(
+                                func(datum).bf,
+                                pos.bf),
+                            gx: A2(
                                 $elm$core$Basics$min,
-                                func(datum).gg,
-                                pos.gg),
-                            dB: A2(
+                                func(datum).gx,
+                                pos.gx),
+                            dL: A2(
                                 $elm$core$Basics$max,
-                                func(datum).dB,
-                                pos.dB)
+                                func(datum).dL,
+                                pos.dL)
                         });
                     } else {
                         return $elm$core$Maybe$Just(
                             func(datum));
                     }
                 });
             return A2(
@@ -7084,41 +8352,41 @@
                 A4($terezka$elm_charts$Internal$Coordinates$Position, 0, 0, 0, 0),
                 A3($elm$core$List$foldl, fold, $elm$core$Maybe$Nothing, data));
         });
     var $terezka$elm_charts$Chart$Attributes$lowest = F3(
         function(v, edit, b) {
             return _Utils_update(
                 b, {
-                    fD: A3(edit, v, b.fD, b.fd)
+                    et: A3(edit, v, b.et, b.fw)
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$orLower = F3(
         function(least, real, _v0) {
             return (_Utils_cmp(real, least) > 0) ? least : real;
         });
     var $terezka$elm_charts$Chart$definePlane = F2(
         function(config, elements) {
-            var width = A2($elm$core$Basics$max, 1, (config.eY - config.R.ed) - config.R.a_);
+            var width = A2($elm$core$Basics$max, 1, (config.ff - config.R.ep) - config.R.a1);
             var toLimit = F5(
                 function(length, marginMin, marginMax, min, max) {
                     return {
-                        fc: max,
-                        fd: min,
+                        fv: max,
+                        fw: min,
                         N: length,
-                        fz: marginMax,
-                        fA: marginMin,
-                        fB: max,
-                        fD: min
+                        fS: marginMax,
+                        fT: marginMin,
+                        er: max,
+                        et: min
                     };
                 });
-            var height = A2($elm$core$Basics$max, 1, (config.d$ - config.R.aH) - config.R.eQ);
+            var height = A2($elm$core$Basics$max, 1, (config.eb - config.R.aM) - config.R.e7);
             var fixSingles = function(bs) {
-                return _Utils_eq(bs.fD, bs.fB) ? _Utils_update(
+                return _Utils_eq(bs.et, bs.er) ? _Utils_update(
                     bs, {
-                        fB: bs.fD + 10
+                        er: bs.et + 10
                     }) : bs;
             };
             var collectLimits = F2(
                 function(el, acc) {
                     switch (el.$) {
                         case 0:
                             return acc;
@@ -7151,83 +8419,83 @@
                             return acc;
                         default:
                             return acc;
                     }
                 });
             var limits_ = function(pos) {
                 return function(_v3) {
-                    var x = _v3.eZ;
-                    var y = _v3.e_;
+                    var x = _v3.fg;
+                    var y = _v3.fh;
                     return {
-                        eZ: fixSingles(x),
-                        e_: fixSingles(y)
+                        fg: fixSingles(x),
+                        fh: fixSingles(y)
                     };
                 }({
-                    eZ: A5(toLimit, width, config.aj.ed, config.aj.a_, pos.aF, pos.bb),
-                    e_: A5(toLimit, height, config.aj.eQ, config.aj.aH, pos.gg, pos.dB)
+                    fg: A5(toLimit, width, config.ao.ep, config.ao.a1, pos.aK, pos.bf),
+                    fh: A5(toLimit, height, config.ao.e7, config.ao.aM, pos.gx, pos.dL)
                 });
             }(
                 A2(
                     $terezka$elm_charts$Internal$Coordinates$foldPosition,
                     $elm$core$Basics$identity,
                     A3($elm$core$List$foldl, collectLimits, _List_Nil, elements)));
             var calcRange = function() {
-                var _v2 = config.dh;
+                var _v2 = config.dp;
                 if (!_v2.b) {
-                    return limits_.eZ;
+                    return limits_.fg;
                 } else {
                     var some = _v2;
                     return A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, b) {
                                 return f(b);
                             }),
-                        limits_.eZ,
+                        limits_.fg,
                         some);
                 }
             }();
             var calcDomain = function() {
-                var _v1 = config.cT;
+                var _v1 = config.cZ;
                 if (!_v1.b) {
-                    return A3($terezka$elm_charts$Chart$Attributes$lowest, 0, $terezka$elm_charts$Chart$Attributes$orLower, limits_.e_);
+                    return A3($terezka$elm_charts$Chart$Attributes$lowest, 0, $terezka$elm_charts$Chart$Attributes$orLower, limits_.fh);
                 } else {
                     var some = _v1;
                     return A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, b) {
                                 return f(b);
                             }),
-                        limits_.e_,
+                        limits_.fh,
                         some);
                 }
             }();
             var unpadded = {
-                eZ: calcRange,
-                e_: calcDomain
+                fg: calcRange,
+                fh: calcDomain
             };
             var scalePadX = $terezka$elm_charts$Internal$Coordinates$scaleCartesianX(unpadded);
-            var xMax = calcRange.fB + scalePadX(config.R.a_);
-            var xMin = calcRange.fD - scalePadX(config.R.ed);
+            var xMax = calcRange.er + scalePadX(config.R.a1);
+            var xMin = calcRange.et - scalePadX(config.R.ep);
             var scalePadY = $terezka$elm_charts$Internal$Coordinates$scaleCartesianY(unpadded);
-            var yMax = calcDomain.fB + scalePadY(config.R.eQ);
-            var yMin = calcDomain.fD - scalePadY(config.R.aH);
+            var yMax = calcDomain.er + scalePadY(config.R.e7);
+            var yMin = calcDomain.et - scalePadY(config.R.aM);
             return {
-                eZ: _Utils_update(
+                fg: _Utils_update(
                     calcRange, {
-                        N: config.eY,
-                        fB: A2($elm$core$Basics$max, xMin, xMax),
-                        fD: A2($elm$core$Basics$min, xMin, xMax)
+                        N: config.ff,
+                        er: A2($elm$core$Basics$max, xMin, xMax),
+                        et: A2($elm$core$Basics$min, xMin, xMax)
                     }),
-                e_: _Utils_update(
+                fh: _Utils_update(
                     calcDomain, {
-                        N: config.d$,
-                        fB: A2($elm$core$Basics$max, yMin, yMax),
-                        fD: A2($elm$core$Basics$min, yMin, yMax)
+                        N: config.eb,
+                        er: A2($elm$core$Basics$max, yMin, yMax),
+                        et: A2($elm$core$Basics$min, yMin, yMax)
                     })
             };
         });
     var $terezka$elm_charts$Chart$getItems = F2(
         function(plane, elements) {
             var toItems = F2(
                 function(el, acc) {
@@ -7310,17 +8578,17 @@
                 }
             });
         return A3($elm$core$List$foldl, toLegends, _List_Nil, elements);
     };
     var $terezka$elm_charts$Chart$TickValues = F4(
         function(xAxis, yAxis, xs, ys) {
             return {
-                bc: xAxis,
+                bg: xAxis,
                 A: xs,
-                bd: yAxis,
+                bh: yAxis,
                 I: ys
             };
         });
     var $terezka$elm_charts$Chart$getTickValues = F3(
         function(plane, items, elements) {
             var toValues = F2(
                 function(el, acc) {
@@ -7395,23 +8663,23 @@
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Svg$Circle = 0;
     var $terezka$elm_charts$Chart$Attributes$circle = function(config) {
         return _Utils_update(
             config, {
-                aB: $elm$core$Maybe$Just(0)
+                aG: $elm$core$Maybe$Just(0)
             });
     };
     var $elm$svg$Svg$Attributes$class = _VirtualDom_attribute('class');
     var $terezka$elm_charts$Chart$Attributes$color = F2(
         function(v, config) {
             return (v === '') ? config : _Utils_update(
                 config, {
-                    by: v
+                    bD: v
                 });
         });
     var $elm$core$List$append = F2(
         function(xs, ys) {
             if (!ys.b) {
                 return xs;
             } else {
@@ -7427,54 +8695,51 @@
                 A2($elm$core$List$map, f, list));
         });
     var $terezka$elm_charts$Internal$Helpers$darkGray = 'rgb(200 200 200)';
     var $terezka$elm_charts$Chart$Attributes$dashed = F2(
         function(value, config) {
             return _Utils_update(
                 config, {
-                    bB: value
+                    bG: value
                 });
         });
     var $terezka$elm_charts$Internal$Helpers$pink = '#ea60df';
     var $terezka$elm_charts$Internal$Svg$defaultDot = {
         v: '',
         x: 0,
-        by: $terezka$elm_charts$Internal$Helpers$pink,
+        bD: $terezka$elm_charts$Internal$Helpers$pink,
         l: false,
-        fo: 0,
-        fp: '',
-        fq: 5,
+        fH: 0,
+        fI: '',
+        fJ: 5,
         P: 1,
-        aB: $elm$core$Maybe$Nothing,
-        eG: 6
+        aG: $elm$core$Maybe$Nothing,
+        eZ: 6
     };
     var $elm$svg$Svg$circle = $elm$svg$Svg$trustedNode('circle');
     var $elm$svg$Svg$Attributes$cx = _VirtualDom_attribute('cx');
     var $elm$svg$Svg$Attributes$cy = _VirtualDom_attribute('cy');
     var $elm$svg$Svg$Attributes$d = _VirtualDom_attribute('d');
     var $elm$svg$Svg$Attributes$fillOpacity = _VirtualDom_attribute('fill-opacity');
     var $elm$svg$Svg$g = $elm$svg$Svg$trustedNode('g');
     var $elm$core$Basics$clamp = F3(
         function(low, high, number) {
             return (_Utils_cmp(number, low) < 0) ? low : ((_Utils_cmp(number, high) > 0) ? high : number);
         });
     var $terezka$elm_charts$Internal$Svg$isWithinPlane = F3(
         function(plane, x, y) {
             return _Utils_eq(
-                A3($elm$core$Basics$clamp, plane.eZ.fD, plane.eZ.fB, x),
+                A3($elm$core$Basics$clamp, plane.fg.et, plane.fg.er, x),
                 x) && _Utils_eq(
-                A3($elm$core$Basics$clamp, plane.e_.fD, plane.e_.fB, y),
+                A3($elm$core$Basics$clamp, plane.fh.et, plane.fh.er, y),
                 y);
         });
     var $elm$core$Basics$not = _Basics_not;
     var $elm$svg$Svg$path = $elm$svg$Svg$trustedNode('path');
     var $elm$core$Basics$pi = _Basics_pi;
-    var $elm$core$Basics$negate = function(n) {
-        return -n;
-    };
     var $elm$core$Basics$sqrt = _Basics_sqrt;
     var $terezka$elm_charts$Internal$Svg$plusPath = F4(
         function(area_, off, x_, y_) {
             var side = $elm$core$Basics$sqrt(area_ / 4) + off;
             var r6 = side / 2;
             var r3 = side;
             return A2(
@@ -7498,31 +8763,30 @@
                         'v' + $elm$core$String$fromFloat(r3 - off)
                     ]));
         });
     var $elm$svg$Svg$Attributes$r = _VirtualDom_attribute('r');
     var $elm$svg$Svg$Attributes$stroke = _VirtualDom_attribute('stroke');
     var $elm$svg$Svg$Attributes$strokeOpacity = _VirtualDom_attribute('stroke-opacity');
     var $elm$svg$Svg$Attributes$strokeWidth = _VirtualDom_attribute('stroke-width');
-    var $elm$virtual_dom$VirtualDom$text = _VirtualDom_text;
     var $elm$svg$Svg$text = $elm$virtual_dom$VirtualDom$text;
     var $terezka$elm_charts$Internal$Coordinates$scaleSVGX = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$innerWidth(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.eZ);
+            return (value * $terezka$elm_charts$Internal$Coordinates$innerWidth(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fg);
         });
     var $terezka$elm_charts$Internal$Coordinates$toSVGX = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, value - plane.eZ.fD) + plane.eZ.fA;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, value - plane.fg.et) + plane.fg.fT;
         });
     var $terezka$elm_charts$Internal$Coordinates$scaleSVGY = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$innerHeight(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.e_);
+            return (value * $terezka$elm_charts$Internal$Coordinates$innerHeight(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fh);
         });
     var $terezka$elm_charts$Internal$Coordinates$toSVGY = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGY, plane, plane.e_.fB - value) + plane.e_.fA;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGY, plane, plane.fh.er - value) + plane.fh.fT;
         });
     var $elm$svg$Svg$Attributes$transform = _VirtualDom_attribute('transform');
     var $elm$core$Basics$degrees = function(angleInDegrees) {
         return (angleInDegrees * $elm$core$Basics$pi) / 180;
     };
     var $elm$core$Basics$tan = _Basics_tan;
     var $terezka$elm_charts$Internal$Svg$trianglePath = F4(
@@ -7553,38 +8817,38 @@
             var yOrg = toY(datum_);
             var y_ = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, yOrg);
             var xOrg = toX(datum_);
             var x_ = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, xOrg);
             var styleAttrs = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$stroke(
-                        (config.v === '') ? config.by : config.v),
+                        (config.v === '') ? config.bD : config.v),
                     $elm$svg$Svg$Attributes$strokeWidth(
                         $elm$core$String$fromFloat(config.x)),
                     $elm$svg$Svg$Attributes$fillOpacity(
                         $elm$core$String$fromFloat(config.P)),
-                    $elm$svg$Svg$Attributes$fill(config.by),
+                    $elm$svg$Svg$Attributes$fill(config.bD),
                     $elm$svg$Svg$Attributes$class('elm-charts__dot'),
                     config.l ? $terezka$elm_charts$Internal$Svg$withinChartArea(plane) : $elm$svg$Svg$Attributes$class('')
                 ]);
             var showDot = A3($terezka$elm_charts$Internal$Svg$isWithinPlane, plane, xOrg, yOrg) || config.l;
-            var highlightColor = (config.fp === '') ? config.by : config.fp;
+            var highlightColor = (config.fI === '') ? config.bD : config.fI;
             var highlightAttrs = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$stroke(highlightColor),
                     $elm$svg$Svg$Attributes$strokeWidth(
-                        $elm$core$String$fromFloat(config.fq)),
+                        $elm$core$String$fromFloat(config.fJ)),
                     $elm$svg$Svg$Attributes$strokeOpacity(
-                        $elm$core$String$fromFloat(config.fo)),
+                        $elm$core$String$fromFloat(config.fH)),
                     $elm$svg$Svg$Attributes$fill('transparent'),
                     $elm$svg$Svg$Attributes$class('elm-charts__dot-highlight')
                 ]);
             var view = F3(
                 function(toEl, highlightOff, toAttrs) {
-                    return (config.fo > 0) ? A2(
+                    return (config.fH > 0) ? A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__dot-container')
                             ]),
                         _List_fromArray(
                             [
@@ -7603,29 +8867,29 @@
                             ])) : A2(
                         toEl,
                         _Utils_ap(
                             toAttrs(0),
                             styleAttrs),
                         _List_Nil);
                 });
-            var area_ = (2 * $elm$core$Basics$pi) * config.eG;
+            var area_ = (2 * $elm$core$Basics$pi) * config.eZ;
             if (!showDot) {
                 return $elm$svg$Svg$text('');
             } else {
-                var _v0 = config.aB;
+                var _v0 = config.aG;
                 if (_v0.$ === 1) {
                     return $elm$svg$Svg$text('');
                 } else {
                     switch (_v0.a) {
                         case 0:
                             var _v1 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$circle,
-                                config.fq / 2,
+                                config.fJ / 2,
                                 function(off) {
                                     var radius = $elm$core$Basics$sqrt(area_ / $elm$core$Basics$pi);
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$cx(
                                                 $elm$core$String$fromFloat(x_)),
                                             $elm$svg$Svg$Attributes$cy(
@@ -7635,28 +8899,28 @@
                                         ]);
                                 });
                         case 1:
                             var _v2 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fq,
+                                config.fJ,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$trianglePath, area_, off, x_, y_))
                                         ]);
                                 });
                         case 2:
                             var _v3 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$rect,
-                                config.fq,
+                                config.fJ,
                                 function(off) {
                                     var side = $elm$core$Basics$sqrt(area_);
                                     var sideOff = side + off;
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x(
                                                 $elm$core$String$fromFloat(x_ - (sideOff / 2))),
@@ -7669,15 +8933,15 @@
                                         ]);
                                 });
                         case 3:
                             var _v4 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$rect,
-                                config.fq,
+                                config.fJ,
                                 function(off) {
                                     var side = $elm$core$Basics$sqrt(area_);
                                     var sideOff = side + off;
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x(
                                                 $elm$core$String$fromFloat(x_ - (sideOff / 2))),
@@ -7692,30 +8956,30 @@
                                         ]);
                                 });
                         case 4:
                             var _v5 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fq,
+                                config.fJ,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$plusPath, area_, off, x_, y_)),
                                             $elm$svg$Svg$Attributes$transform(
                                                 'rotate(45 ' + ($elm$core$String$fromFloat(x_) + (' ' + ($elm$core$String$fromFloat(y_) + ')'))))
                                         ]);
                                 });
                         default:
                             var _v6 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fq,
+                                config.fJ,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$plusPath, area_, off, x_, y_))
                                         ]);
                                 });
@@ -7730,31 +8994,31 @@
                 plane,
                 toX,
                 toY,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultDot));
         });
     var $terezka$elm_charts$Internal$Helpers$gray = '#EFF2FA';
     var $terezka$elm_charts$Internal$Svg$defaultLine = {
-        bq: _List_Nil,
-        e7: false,
-        by: 'rgb(210, 210, 210)',
-        bB: _List_Nil,
+        bv: _List_Nil,
+        fq: false,
+        bD: 'rgb(210, 210, 210)',
+        bG: _List_Nil,
         e: false,
         l: false,
         P: 1,
-        fW: -90,
-        fX: 0,
-        eY: 1,
-        aF: $elm$core$Maybe$Nothing,
-        bb: $elm$core$Maybe$Nothing,
-        gf: $elm$core$Maybe$Nothing,
+        gb: -90,
+        gc: 0,
+        ff: 1,
+        aK: $elm$core$Maybe$Nothing,
+        bf: $elm$core$Maybe$Nothing,
+        gw: $elm$core$Maybe$Nothing,
         g: 0,
-        gg: $elm$core$Maybe$Nothing,
-        dB: $elm$core$Maybe$Nothing,
-        gh: $elm$core$Maybe$Nothing,
+        gx: $elm$core$Maybe$Nothing,
+        dL: $elm$core$Maybe$Nothing,
+        gy: $elm$core$Maybe$Nothing,
         h: 0
     };
     var $terezka$elm_charts$Internal$Commands$Line = F2(
         function(a, b) {
             return {
                 $: 1,
                 a: a,
@@ -8026,33 +9290,33 @@
                     A2(
                         $elm$core$List$map,
                         $elm$html$Html$Attributes$map($elm$core$Basics$never),
                         attrs)));
         });
     var $terezka$elm_charts$Internal$Svg$line = F2(
         function(plane, config) {
-            var angle = $elm$core$Basics$degrees(config.fW);
+            var angle = $elm$core$Basics$degrees(config.gb);
             var _v0 = function() {
                 var _v3 = _Utils_Tuple3(
-                    _Utils_Tuple2(config.aF, config.bb),
-                    _Utils_Tuple2(config.gg, config.dB),
-                    _Utils_Tuple2(config.gf, config.gh));
+                    _Utils_Tuple2(config.aK, config.bf),
+                    _Utils_Tuple2(config.gx, config.dL),
+                    _Utils_Tuple2(config.gw, config.gy));
                 if (!_v3.a.a.$) {
                     if (!_v3.a.b.$) {
                         if (_v3.b.a.$ === 1) {
                             if (_v3.b.b.$ === 1) {
                                 var _v4 = _v3.a;
                                 var a = _v4.a.a;
                                 var b = _v4.b.a;
                                 var _v5 = _v3.b;
                                 var _v6 = _v5.a;
                                 var _v7 = _v5.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, b),
-                                    _Utils_Tuple2(plane.e_.fD, plane.e_.fD));
+                                    _Utils_Tuple2(plane.fh.et, plane.fh.et));
                             } else {
                                 var _v38 = _v3.a;
                                 var a = _v38.a.a;
                                 var b = _v38.b.a;
                                 var _v39 = _v3.b;
                                 var _v40 = _v39.a;
                                 var c = _v39.b.a;
@@ -8070,33 +9334,33 @@
                                 var _v43 = _v42.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, b),
                                     _Utils_Tuple2(c, c));
                             } else {
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(
-                                        A2($elm$core$Maybe$withDefault, plane.eZ.fD, config.aF),
-                                        A2($elm$core$Maybe$withDefault, plane.eZ.fB, config.bb)),
+                                        A2($elm$core$Maybe$withDefault, plane.fg.et, config.aK),
+                                        A2($elm$core$Maybe$withDefault, plane.fg.er, config.bf)),
                                     _Utils_Tuple2(
-                                        A2($elm$core$Maybe$withDefault, plane.e_.fD, config.gg),
-                                        A2($elm$core$Maybe$withDefault, plane.e_.fB, config.dB)));
+                                        A2($elm$core$Maybe$withDefault, plane.fh.et, config.gx),
+                                        A2($elm$core$Maybe$withDefault, plane.fh.er, config.dL)));
                             }
                         }
                     } else {
                         if (_v3.b.a.$ === 1) {
                             if (_v3.b.b.$ === 1) {
                                 var _v8 = _v3.a;
                                 var a = _v8.a.a;
                                 var _v9 = _v8.b;
                                 var _v10 = _v3.b;
                                 var _v11 = _v10.a;
                                 var _v12 = _v10.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, a),
-                                    _Utils_Tuple2(plane.e_.fD, plane.e_.fB));
+                                    _Utils_Tuple2(plane.fh.et, plane.fh.er));
                             } else {
                                 if (!_v3.c.a.$) {
                                     if (!_v3.c.b.$) {
                                         var _v51 = _v3.a;
                                         var a = _v51.a.a;
                                         var _v52 = _v51.b;
                                         var _v53 = _v3.b;
@@ -8136,15 +9400,15 @@
                                         var _v46 = _v3.b;
                                         var _v47 = _v46.a;
                                         var b = _v46.b.a;
                                         var _v48 = _v3.c;
                                         var _v49 = _v48.a;
                                         var _v50 = _v48.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.eZ.fB),
+                                            _Utils_Tuple2(a, plane.fg.er),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v62 = _v3.a;
                                         var a = _v62.a.a;
                                         var _v63 = _v62.b;
                                         var _v64 = _v3.b;
                                         var _v65 = _v64.a;
@@ -8214,15 +9478,15 @@
                                         var _v70 = _v3.b;
                                         var b = _v70.a.a;
                                         var _v71 = _v70.b;
                                         var _v72 = _v3.c;
                                         var _v73 = _v72.a;
                                         var _v74 = _v72.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.eZ.fB),
+                                            _Utils_Tuple2(a, plane.fg.er),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v86 = _v3.a;
                                         var a = _v86.a.a;
                                         var _v87 = _v86.b;
                                         var _v88 = _v3.b;
                                         var b = _v88.a.a;
@@ -8248,15 +9512,15 @@
                                 var _v14 = _v13.a;
                                 var b = _v13.b.a;
                                 var _v15 = _v3.b;
                                 var _v16 = _v15.a;
                                 var _v17 = _v15.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(b, b),
-                                    _Utils_Tuple2(plane.e_.fD, plane.e_.fB));
+                                    _Utils_Tuple2(plane.fh.et, plane.fh.er));
                             } else {
                                 if (!_v3.c.a.$) {
                                     if (!_v3.c.b.$) {
                                         var _v99 = _v3.a;
                                         var _v100 = _v99.a;
                                         var a = _v99.b.a;
                                         var _v101 = _v3.b;
@@ -8296,15 +9560,15 @@
                                         var _v94 = _v3.b;
                                         var _v95 = _v94.a;
                                         var b = _v94.b.a;
                                         var _v96 = _v3.c;
                                         var _v97 = _v96.a;
                                         var _v98 = _v96.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.eZ.fB),
+                                            _Utils_Tuple2(a, plane.fg.er),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v110 = _v3.a;
                                         var _v111 = _v110.a;
                                         var a = _v110.b.a;
                                         var _v112 = _v3.b;
                                         var _v113 = _v112.a;
@@ -8374,15 +9638,15 @@
                                         var _v118 = _v3.b;
                                         var b = _v118.a.a;
                                         var _v119 = _v118.b;
                                         var _v120 = _v3.c;
                                         var _v121 = _v120.a;
                                         var _v122 = _v120.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.eZ.fB),
+                                            _Utils_Tuple2(a, plane.fg.er),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v134 = _v3.a;
                                         var _v135 = _v134.a;
                                         var a = _v134.b.a;
                                         var _v136 = _v3.b;
                                         var b = _v136.a.a;
@@ -8405,48 +9669,48 @@
                                 var _v18 = _v3.a;
                                 var _v19 = _v18.a;
                                 var _v20 = _v18.b;
                                 var _v21 = _v3.b;
                                 var a = _v21.a.a;
                                 var b = _v21.b.a;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.eZ.fD, plane.eZ.fD),
+                                    _Utils_Tuple2(plane.fg.et, plane.fg.et),
                                     _Utils_Tuple2(a, b));
                             } else {
                                 var _v22 = _v3.a;
                                 var _v23 = _v22.a;
                                 var _v24 = _v22.b;
                                 var _v25 = _v3.b;
                                 var a = _v25.a.a;
                                 var _v26 = _v25.b;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.eZ.fD, plane.eZ.fB),
+                                    _Utils_Tuple2(plane.fg.et, plane.fg.er),
                                     _Utils_Tuple2(a, a));
                             }
                         } else {
                             if (!_v3.b.b.$) {
                                 var _v27 = _v3.a;
                                 var _v28 = _v27.a;
                                 var _v29 = _v27.b;
                                 var _v30 = _v3.b;
                                 var _v31 = _v30.a;
                                 var b = _v30.b.a;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.eZ.fD, plane.eZ.fB),
+                                    _Utils_Tuple2(plane.fg.et, plane.fg.er),
                                     _Utils_Tuple2(b, b));
                             } else {
                                 var _v140 = _v3.a;
                                 var _v141 = _v140.a;
                                 var _v142 = _v140.b;
                                 var _v143 = _v3.b;
                                 var _v144 = _v143.a;
                                 var _v145 = _v143.b;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.eZ.fD, plane.eZ.fB),
-                                    _Utils_Tuple2(plane.e_.fD, plane.e_.fB));
+                                    _Utils_Tuple2(plane.fg.et, plane.fg.er),
+                                    _Utils_Tuple2(plane.fh.et, plane.fh.er));
                             }
                         }
                     }
                 }
             }();
             var _v1 = _v0.a;
             var x1 = _v1.a;
@@ -8454,86 +9718,86 @@
             var _v2 = _v0.b;
             var y1 = _v2.a;
             var y2 = _v2.b;
             var x1_ = x1 + A2($terezka$elm_charts$Internal$Svg$lengthInCartesianX, plane, config.g);
             var x2_ = x2 + A2($terezka$elm_charts$Internal$Svg$lengthInCartesianX, plane, config.g);
             var y1_ = y1 - A2($terezka$elm_charts$Internal$Svg$lengthInCartesianY, plane, config.h);
             var y2_ = y2 - A2($terezka$elm_charts$Internal$Svg$lengthInCartesianY, plane, config.h);
-            var _v146 = (config.fX > 0) ? _Utils_Tuple2(
+            var _v146 = (config.gc > 0) ? _Utils_Tuple2(
                 A2(
                     $terezka$elm_charts$Internal$Svg$lengthInCartesianX,
                     plane,
-                    $elm$core$Basics$cos(angle) * config.fX),
+                    $elm$core$Basics$cos(angle) * config.gc),
                 A2(
                     $terezka$elm_charts$Internal$Svg$lengthInCartesianY,
                     plane,
-                    $elm$core$Basics$sin(angle) * config.fX)) : _Utils_Tuple2(0, 0);
+                    $elm$core$Basics$sin(angle) * config.gc)) : _Utils_Tuple2(0, 0);
             var tickOffsetX = _v146.a;
             var tickOffsetY = _v146.b;
             var cmds = config.e ? _Utils_ap(
-                (config.fX > 0) ? _List_fromArray(
+                (config.gc > 0) ? _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x2_ + tickOffsetX, y2_ + tickOffsetY),
                         A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                     ]) : _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x2_, y2_)
                     ]),
                 _Utils_ap(
-                    config.e7 ? _List_fromArray(
+                    config.fq ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y1_),
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                         ]) : _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                         ]),
-                    (config.fX > 0) ? _List_fromArray(
+                    (config.gc > 0) ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_ + tickOffsetX, y1_ + tickOffsetY)
                         ]) : _List_Nil)) : _Utils_ap(
-                (config.fX > 0) ? _List_fromArray(
+                (config.gc > 0) ? _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x1_ + tickOffsetX, y1_ + tickOffsetY),
                         A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                     ]) : _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x1_, y1_)
                     ]),
                 _Utils_ap(
-                    config.e7 ? _List_fromArray(
+                    config.fq ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y2_),
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                         ]) : _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                         ]),
-                    (config.fX > 0) ? _List_fromArray(
+                    (config.gc > 0) ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_ + tickOffsetX, y2_ + tickOffsetY)
                         ]) : _List_Nil));
             return A4(
                 $terezka$elm_charts$Internal$Svg$withAttrs,
-                config.bq,
+                config.bv,
                 $elm$svg$Svg$path,
                 _List_fromArray(
                     [
                         $elm$svg$Svg$Attributes$class('elm-charts__line'),
                         $elm$svg$Svg$Attributes$fill('transparent'),
-                        $elm$svg$Svg$Attributes$stroke(config.by),
+                        $elm$svg$Svg$Attributes$stroke(config.bD),
                         $elm$svg$Svg$Attributes$strokeWidth(
-                            $elm$core$String$fromFloat(config.eY)),
+                            $elm$core$String$fromFloat(config.ff)),
                         $elm$svg$Svg$Attributes$strokeOpacity(
                             $elm$core$String$fromFloat(config.P)),
                         $elm$svg$Svg$Attributes$strokeDasharray(
                             A2(
                                 $elm$core$String$join,
                                 ' ',
-                                A2($elm$core$List$map, $elm$core$String$fromFloat, config.bB))),
+                                A2($elm$core$List$map, $elm$core$String$fromFloat, config.bG))),
                         $elm$svg$Svg$Attributes$d(
                             A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                         config.l ? $terezka$elm_charts$Internal$Svg$withinChartArea(plane) : $elm$svg$Svg$Attributes$class('')
                     ]),
                 _List_Nil);
         });
     var $terezka$elm_charts$Chart$Svg$line = F2(
@@ -8552,109 +9816,109 @@
                 },
                 xs);
         });
     var $terezka$elm_charts$Chart$Attributes$size = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    eG: v
+                    eZ: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$width = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    eY: v
+                    ff: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$x1 = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    aF: $elm$core$Maybe$Just(v)
+                    aK: $elm$core$Maybe$Just(v)
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$y1 = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    gg: $elm$core$Maybe$Just(v)
+                    gx: $elm$core$Maybe$Just(v)
                 });
         });
     var $terezka$elm_charts$Chart$grid = function(edits) {
         var config = A2(
             $terezka$elm_charts$Internal$Helpers$apply,
             edits, {
-                by: '',
-                bB: _List_Nil,
-                aK: false,
-                eY: 0
+                bD: '',
+                bG: _List_Nil,
+                aP: false,
+                ff: 0
             });
-        var width = (!config.eY) ? (config.aK ? 0.5 : 1) : config.eY;
-        var color = $elm$core$String$isEmpty(config.by) ? (config.aK ? $terezka$elm_charts$Internal$Helpers$darkGray : $terezka$elm_charts$Internal$Helpers$gray) : config.by;
+        var width = (!config.ff) ? (config.aP ? 0.5 : 1) : config.ff;
+        var color = $elm$core$String$isEmpty(config.bD) ? (config.aP ? $terezka$elm_charts$Internal$Helpers$darkGray : $terezka$elm_charts$Internal$Helpers$gray) : config.bD;
         var toDot = F4(
             function(vs, p, x, y) {
-                return (A2($elm$core$List$member, x, vs.bc) || A2($elm$core$List$member, y, vs.bd)) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return (A2($elm$core$List$member, x, vs.bg) || A2($elm$core$List$member, y, vs.bh)) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A5(
                         $terezka$elm_charts$Chart$Svg$dot,
                         p,
                         function($) {
-                            return $.eZ;
+                            return $.fg;
                         },
                         function($) {
-                            return $.e_;
+                            return $.fh;
                         },
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$size(width),
                                 $terezka$elm_charts$Chart$Attributes$circle
                             ]), {
-                            eZ: x,
-                            e_: y
+                            fg: x,
+                            fh: y
                         }));
             });
         var toXGrid = F3(
             function(vs, p, v) {
-                return A2($elm$core$List$member, v, vs.bc) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return A2($elm$core$List$member, v, vs.bg) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A2(
                         $terezka$elm_charts$Chart$Svg$line,
                         p,
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$width(width),
                                 $terezka$elm_charts$Chart$Attributes$x1(v),
-                                $terezka$elm_charts$Chart$Attributes$dashed(config.bB)
+                                $terezka$elm_charts$Chart$Attributes$dashed(config.bG)
                             ])));
             });
         var toYGrid = F3(
             function(vs, p, v) {
-                return A2($elm$core$List$member, v, vs.bd) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return A2($elm$core$List$member, v, vs.bh) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A2(
                         $terezka$elm_charts$Chart$Svg$line,
                         p,
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$width(width),
                                 $terezka$elm_charts$Chart$Attributes$y1(v),
-                                $terezka$elm_charts$Chart$Attributes$dashed(config.bB)
+                                $terezka$elm_charts$Chart$Attributes$dashed(config.bG)
                             ])));
             });
         return $terezka$elm_charts$Chart$GridElement(
             F2(
                 function(p, vs) {
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__grid')
                             ]),
-                        config.aK ? A2(
+                        config.aP ? A2(
                             $elm$core$List$concatMap,
                             function(x) {
                                 return A2(
                                     $elm$core$List$filterMap,
                                     A3(toDot, vs, p, x),
                                     vs.I);
                             },
@@ -8884,161 +10148,136 @@
                     $terezka$elm_charts$Chart$grid(_List_Nil),
                     indexedElements);
             }();
             var legends_ = $terezka$elm_charts$Chart$getLegends(elements);
             var config = A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
-                    bq: _List_fromArray(
+                    bv: _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$style('overflow: visible;')
                         ]),
-                    cT: _List_Nil,
-                    bH: _List_Nil,
-                    d$: 300,
-                    bR: _List_Nil,
-                    aj: {
-                        aH: 0,
-                        ed: 0,
-                        a_: 0,
-                        eQ: 0
+                    cZ: _List_Nil,
+                    bM: _List_Nil,
+                    eb: 300,
+                    bY: _List_Nil,
+                    ao: {
+                        aM: 0,
+                        ep: 0,
+                        a1: 0,
+                        e7: 0
                     },
                     R: {
-                        aH: 0,
-                        ed: 0,
-                        a_: 0,
-                        eQ: 0
+                        aM: 0,
+                        ep: 0,
+                        a1: 0,
+                        e7: 0
                     },
-                    dh: _List_Nil,
-                    cq: true,
-                    eY: 300
+                    dp: _List_Nil,
+                    cx: true,
+                    ff: 300
                 });
             var plane = A2($terezka$elm_charts$Chart$definePlane, config, elements);
             var items = A2($terezka$elm_charts$Chart$getItems, plane, elements);
             var toEvent = function(_v2) {
                 var event_ = _v2;
-                var _v1 = event_.ff;
+                var _v1 = event_.fy;
                 var decoder = _v1;
                 return A2(
                     $terezka$elm_charts$Internal$Svg$Event,
-                    event_.fF,
+                    event_.fW,
                     decoder(items));
             };
             var tickValues = A3($terezka$elm_charts$Chart$getTickValues, plane, items, elements);
             var _v0 = A6($terezka$elm_charts$Chart$viewElements, config, plane, tickValues, items, legends_, elements);
             var beforeEls = _v0.a;
             var chartEls = _v0.b;
             var afterEls = _v0.c;
             return A5(
                 $terezka$elm_charts$Internal$Svg$container,
                 plane, {
-                    bq: config.bq,
-                    bH: A2($elm$core$List$map, toEvent, config.bH),
-                    bR: config.bR,
-                    cq: config.cq
+                    bv: config.bv,
+                    bM: A2($elm$core$List$map, toEvent, config.bM),
+                    bY: config.bY,
+                    cx: config.cx
                 },
                 beforeEls,
                 chartEls,
                 afterEls);
         });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Column = function(a) {
-        return {
-            $: 0,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$col = F2(
-        function(options, children) {
-            return $rundis$elm_bootstrap$Bootstrap$Grid$Column({
-                dJ: children,
-                db: options
-            });
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$container = F2(
-        function(attributes, children) {
-            return A2(
-                $elm$html$Html$div,
-                _Utils_ap(
-                    _List_fromArray(
-                        [
-                            $elm$html$Html$Attributes$class('container')
-                        ]),
-                    attributes),
-                children);
-        });
     var $terezka$elm_charts$Internal$Many$Remodel = F2(
         function(a, b) {
             return {
                 $: 0,
                 a: a,
                 b: b
             };
         });
     var $terezka$elm_charts$Internal$Coordinates$center = function(pos) {
         return {
-            eZ: pos.aF + ((pos.bb - pos.aF) / 2),
-            e_: pos.gg + ((pos.dB - pos.gg) / 2)
+            fg: pos.aK + ((pos.bf - pos.aK) / 2),
+            fh: pos.gx + ((pos.dL - pos.gx) / 2)
         };
     };
     var $terezka$elm_charts$Internal$Many$fromPoint = function(point) {
         return {
-            aF: point.eZ,
-            bb: point.eZ,
-            gg: point.e_,
-            dB: point.e_
+            aK: point.fg,
+            bf: point.fg,
+            gx: point.fh,
+            dL: point.fh
         };
     };
     var $terezka$elm_charts$Internal$Item$getPosition = F2(
         function(plane, _v0) {
             var item = _v0;
-            return A2(item.f5, plane, item.e9);
+            return A2(item.gm, plane, item.fs);
         });
     var $terezka$elm_charts$Internal$Item$Dot = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Item$Rendered = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Item$isDot = function(_v0) {
         var item = _v0;
-        var _v1 = item.e9.fJ;
+        var _v1 = item.fs.f_;
         if (!_v1.$) {
             var dot = _v1.a;
             return $elm$core$Maybe$Just({
-                e9: {
-                    fJ: dot,
-                    f0: $terezka$elm_charts$Internal$Item$Dot,
-                    cC: item.e9.cC,
-                    gb: item.e9.gb
+                fs: {
+                    f_: dot,
+                    gh: $terezka$elm_charts$Internal$Item$Dot,
+                    cI: item.fs.cI,
+                    gs: item.fs.gs
                 },
-                f1: function(c) {
-                    return item.f1(item.e9);
+                gi: function(c) {
+                    return item.gi(item.fs);
                 },
-                f2: function(_v2) {
-                    return item.f2(item.e9);
+                gj: function(_v2) {
+                    return item.gj(item.fs);
                 },
-                f5: F2(
+                gm: F2(
                     function(plane, _v3) {
-                        return A2(item.f5, plane, item.e9);
+                        return A2(item.gm, plane, item.fs);
                     }),
-                f6: F3(
+                gn: F3(
                     function(plane, config, pos) {
-                        return config.gb.fx ? A5(
+                        return config.gs.fQ ? A5(
                             $terezka$elm_charts$Internal$Svg$dot,
                             plane,
                             function($) {
-                                return $.eZ;
+                                return $.fg;
                             },
                             function($) {
-                                return $.e_;
+                                return $.fh;
                             },
-                            config.fJ, {
-                                eZ: config.gb.aF,
-                                e_: config.gb.e_
+                            config.f_, {
+                                fg: config.gs.aK,
+                                fh: config.gs.fh
                             }) : $elm$svg$Svg$text('');
                     })
             });
         } else {
             return $elm$core$Maybe$Nothing;
         }
     };
@@ -9082,15 +10321,15 @@
     var $terezka$elm_charts$Chart$Attributes$format = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
                     F: $elm$core$Maybe$Just(v)
                 });
         });
-    var $author$project$Main$monthToString = function(month) {
+    var $author$project$Graph$monthToString = function(month) {
         switch (month) {
             case 0:
                 return '01';
             case 1:
                 return '02';
             case 2:
                 return '03';
@@ -9114,27 +10353,23 @@
                 return '12';
         }
     };
     var $elm$time$Time$flooredDiv = F2(
         function(numerator, denominator) {
             return $elm$core$Basics$floor(numerator / denominator);
         });
-    var $elm$time$Time$posixToMillis = function(_v0) {
-        var millis = _v0;
-        return millis;
-    };
     var $elm$time$Time$toAdjustedMinutesHelp = F3(
         function(defaultOffset, posixMinutes, eras) {
             toAdjustedMinutesHelp: while (true) {
                 if (!eras.b) {
                     return posixMinutes + defaultOffset;
                 } else {
                     var era = eras.a;
                     var olderEras = eras.b;
-                    if (_Utils_cmp(era.dt, posixMinutes) < 0) {
+                    if (_Utils_cmp(era.dD, posixMinutes) < 0) {
                         return posixMinutes + era.b;
                     } else {
                         var $temp$defaultOffset = defaultOffset,
                             $temp$posixMinutes = posixMinutes,
                             $temp$eras = olderEras;
                         defaultOffset = $temp$defaultOffset;
                         posixMinutes = $temp$posixMinutes;
@@ -9164,25 +10399,24 @@
         var dayOfEra = rawDay - (era * 146097);
         var yearOfEra = ((((dayOfEra - ((dayOfEra / 1460) | 0)) + ((dayOfEra / 36524) | 0)) - ((dayOfEra / 146096) | 0)) / 365) | 0;
         var dayOfYear = dayOfEra - (((365 * yearOfEra) + ((yearOfEra / 4) | 0)) - ((yearOfEra / 100) | 0));
         var mp = (((5 * dayOfYear) + 2) / 153) | 0;
         var month = mp + ((mp < 10) ? 3 : (-9));
         var year = yearOfEra + (era * 400);
         return {
-            dN: (dayOfYear - ((((153 * mp) + 2) / 5) | 0)) + 1,
-            eh: month,
-            e$: year + ((month <= 2) ? 1 : 0)
+            dY: (dayOfYear - ((((153 * mp) + 2) / 5) | 0)) + 1,
+            ev: month,
+            fi: year + ((month <= 2) ? 1 : 0)
         };
     };
     var $elm$time$Time$toDay = F2(
         function(zone, time) {
             return $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).dN;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).dY;
         });
-    var $elm$core$Basics$modBy = _Basics_modBy;
     var $elm$time$Time$toHour = F2(
         function(zone, time) {
             return A2(
                 $elm$core$Basics$modBy,
                 24,
                 A2(
                     $elm$time$Time$flooredDiv,
@@ -9207,15 +10441,15 @@
     var $elm$time$Time$May = 4;
     var $elm$time$Time$Nov = 10;
     var $elm$time$Time$Oct = 9;
     var $elm$time$Time$Sep = 8;
     var $elm$time$Time$toMonth = F2(
         function(zone, time) {
             var _v0 = $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).eh;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).ev;
             switch (_v0) {
                 case 1:
                     return 0;
                 case 2:
                     return 1;
                 case 3:
                     return 2;
@@ -9248,1016 +10482,59 @@
                     $elm$time$Time$flooredDiv,
                     $elm$time$Time$posixToMillis(time),
                     1000));
         });
     var $elm$time$Time$toYear = F2(
         function(zone, time) {
             return $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).e$;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).fi;
         });
     var $elm$time$Time$utc = A2($elm$time$Time$Zone, 0, _List_Nil);
-    var $author$project$Main$formatTime = function(time) {
+    var $author$project$Graph$formatTime = function(time) {
         var milliTime = $elm$time$Time$millisToPosix(
             $elm$core$Basics$floor(time) * 1000);
         var minute = $elm$core$String$fromInt(
             A2($elm$time$Time$toMinute, $elm$time$Time$utc, milliTime));
-        var month = $author$project$Main$monthToString(
+        var month = $author$project$Graph$monthToString(
             A2($elm$time$Time$toMonth, $elm$time$Time$utc, milliTime));
         var second = $elm$core$String$fromInt(
             A2($elm$time$Time$toSecond, $elm$time$Time$utc, milliTime));
         var year = $elm$core$String$fromInt(
             A2($elm$time$Time$toYear, $elm$time$Time$utc, milliTime));
         var hour = $elm$core$String$fromInt(
             A2($elm$time$Time$toHour, $elm$time$Time$utc, milliTime));
         var day = $elm$core$String$fromInt(
             A2($elm$time$Time$toDay, $elm$time$Time$utc, milliTime));
         return month + ('/' + (day + (' ' + (hour + (':' + (minute + (':' + second)))))));
     };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColAttrs = function(a) {
-        return {
-            $: 6,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs = function(attrs_) {
-        return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColAttrs(attrs_);
-    };
-    var $author$project$DeviceStatus$deviceStatusColor = function(deviceStatus) {
-        switch (deviceStatus) {
-            case 0:
-                return 'green';
-            case 1:
-                return 'gray';
-            default:
-                return 'red';
-        }
-    };
-    var $author$project$DeviceStatus$deviceStatusImage = function(deviceStatus) {
-        switch (deviceStatus) {
-            case 0:
-                return '/static/images/loading.gif';
-            case 1:
-                return '/static/images/idle.png';
-            default:
-                return '/static/images/failing.png';
-        }
-    };
-    var $author$project$DeviceStatus$deviceStatusToString = function(deviceStatus) {
-        switch (deviceStatus) {
-            case 0:
-                return 'Reading';
-            case 1:
-                return 'Idle';
-            default:
-                return 'Failing';
-        }
-    };
-    var $elm$html$Html$h5 = _VirtualDom_node('h5');
-    var $elm$html$Html$img = _VirtualDom_node('img');
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col = 0;
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width = F2(
-        function(screenSize, columnCount) {
-            return {
-                dL: columnCount,
-                eD: screenSize
-            };
-        });
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$XS = 0;
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign = F2(
-        function(align_, options) {
-            var _v0 = align_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            bl: $elm$core$Maybe$Just(align_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            bj: $elm$core$Maybe$Just(align_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            bi: $elm$core$Maybe$Just(align_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            bh: $elm$core$Maybe$Just(align_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            bk: $elm$core$Maybe$Just(align_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset = F2(
-        function(offset_, options) {
-            var _v0 = offset_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            b2: $elm$core$Maybe$Just(offset_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            b$: $elm$core$Maybe$Just(offset_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            b_: $elm$core$Maybe$Just(offset_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            bZ: $elm$core$Maybe$Just(offset_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            b1: $elm$core$Maybe$Just(offset_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOrder = F2(
-        function(order_, options) {
-            var _v0 = order_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            cc: $elm$core$Maybe$Just(order_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            ca: $elm$core$Maybe$Just(order_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            b9: $elm$core$Maybe$Just(order_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            b8: $elm$core$Maybe$Just(order_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            cb: $elm$core$Maybe$Just(order_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPull = F2(
-        function(pull_, options) {
-            var _v0 = pull_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            ci: $elm$core$Maybe$Just(pull_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            cg: $elm$core$Maybe$Just(pull_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            cf: $elm$core$Maybe$Just(pull_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            ce: $elm$core$Maybe$Just(pull_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            ch: $elm$core$Maybe$Just(pull_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPush = F2(
-        function(push_, options) {
-            var _v0 = push_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            cn: $elm$core$Maybe$Just(push_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            cl: $elm$core$Maybe$Just(push_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            ck: $elm$core$Maybe$Just(push_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            cj: $elm$core$Maybe$Just(push_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            cm: $elm$core$Maybe$Just(push_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth = F2(
-        function(width_, options) {
-            var _v0 = width_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            a9: $elm$core$Maybe$Just(width_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            a7: $elm$core$Maybe$Just(width_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            a6: $elm$core$Maybe$Just(width_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            a5: $elm$core$Maybe$Just(width_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            a8: $elm$core$Maybe$Just(width_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption = F2(
-        function(modifier, options) {
-            switch (modifier.$) {
-                case 6:
-                    var attrs = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            bp: _Utils_ap(options.bp, attrs)
-                        });
-                case 0:
-                    var width_ = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth, width_, options);
-                case 1:
-                    var offset_ = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset, offset_, options);
-                case 2:
-                    var pull_ = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPull, pull_, options);
-                case 3:
-                    var push_ = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPush, push_, options);
-                case 4:
-                    var order_ = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOrder, order_, options);
-                case 5:
-                    var align = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign, align, options);
-                default:
-                    var align = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            cz: $elm$core$Maybe$Just(align)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$columnCountOption = function(size) {
-        switch (size) {
-            case 0:
-                return $elm$core$Maybe$Nothing;
-            case 1:
-                return $elm$core$Maybe$Just('1');
-            case 2:
-                return $elm$core$Maybe$Just('2');
-            case 3:
-                return $elm$core$Maybe$Just('3');
-            case 4:
-                return $elm$core$Maybe$Just('4');
-            case 5:
-                return $elm$core$Maybe$Just('5');
-            case 6:
-                return $elm$core$Maybe$Just('6');
-            case 7:
-                return $elm$core$Maybe$Just('7');
-            case 8:
-                return $elm$core$Maybe$Just('8');
-            case 9:
-                return $elm$core$Maybe$Just('9');
-            case 10:
-                return $elm$core$Maybe$Just('10');
-            case 11:
-                return $elm$core$Maybe$Just('11');
-            case 12:
-                return $elm$core$Maybe$Just('12');
-            default:
-                return $elm$core$Maybe$Just('auto');
-        }
-    };
-    var $elm$core$Maybe$map = F2(
-        function(f, maybe) {
-            if (!maybe.$) {
-                var value = maybe.a;
-                return $elm$core$Maybe$Just(
-                    f(value));
-            } else {
-                return $elm$core$Maybe$Nothing;
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption = function(size) {
-        switch (size) {
-            case 0:
-                return $elm$core$Maybe$Nothing;
-            case 1:
-                return $elm$core$Maybe$Just('sm');
-            case 2:
-                return $elm$core$Maybe$Just('md');
-            case 3:
-                return $elm$core$Maybe$Just('lg');
-            default:
-                return $elm$core$Maybe$Just('xl');
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthClass = function(_v0) {
-        var screenSize = _v0.eD;
-        var columnCount = _v0.dL;
-        return $elm$html$Html$Attributes$class(
-            'col' + (A2(
-                $elm$core$Maybe$withDefault,
-                '',
-                A2(
-                    $elm$core$Maybe$map,
-                    function(v) {
-                        return '-' + v;
-                    },
-                    $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize))) + A2(
-                $elm$core$Maybe$withDefault,
-                '',
-                A2(
-                    $elm$core$Maybe$map,
-                    function(v) {
-                        return '-' + v;
-                    },
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$columnCountOption(columnCount)))));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthsToAttributes = function(widths) {
-        var width_ = function(w) {
-            return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthClass, w);
-        };
-        return A2(
-            $elm$core$List$filterMap,
-            $elm$core$Basics$identity,
-            A2($elm$core$List$map, width_, widths));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions = {
-        bh: $elm$core$Maybe$Nothing,
-        bi: $elm$core$Maybe$Nothing,
-        bj: $elm$core$Maybe$Nothing,
-        bk: $elm$core$Maybe$Nothing,
-        bl: $elm$core$Maybe$Nothing,
-        bp: _List_Nil,
-        bZ: $elm$core$Maybe$Nothing,
-        b_: $elm$core$Maybe$Nothing,
-        b$: $elm$core$Maybe$Nothing,
-        b1: $elm$core$Maybe$Nothing,
-        b2: $elm$core$Maybe$Nothing,
-        b8: $elm$core$Maybe$Nothing,
-        b9: $elm$core$Maybe$Nothing,
-        ca: $elm$core$Maybe$Nothing,
-        cb: $elm$core$Maybe$Nothing,
-        cc: $elm$core$Maybe$Nothing,
-        ce: $elm$core$Maybe$Nothing,
-        cf: $elm$core$Maybe$Nothing,
-        cg: $elm$core$Maybe$Nothing,
-        ch: $elm$core$Maybe$Nothing,
-        ci: $elm$core$Maybe$Nothing,
-        cj: $elm$core$Maybe$Nothing,
-        ck: $elm$core$Maybe$Nothing,
-        cl: $elm$core$Maybe$Nothing,
-        cm: $elm$core$Maybe$Nothing,
-        cn: $elm$core$Maybe$Nothing,
-        cz: $elm$core$Maybe$Nothing,
-        a5: $elm$core$Maybe$Nothing,
-        a6: $elm$core$Maybe$Nothing,
-        a7: $elm$core$Maybe$Nothing,
-        a8: $elm$core$Maybe$Nothing,
-        a9: $elm$core$Maybe$Nothing
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption = function(size) {
-        switch (size) {
-            case 0:
-                return '0';
-            case 1:
-                return '1';
-            case 2:
-                return '2';
-            case 3:
-                return '3';
-            case 4:
-                return '4';
-            case 5:
-                return '5';
-            case 6:
-                return '6';
-            case 7:
-                return '7';
-            case 8:
-                return '8';
-            case 9:
-                return '9';
-            case 10:
-                return '10';
-            default:
-                return '11';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString = function(screenSize) {
-        var _v0 = $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize);
-        if (!_v0.$) {
-            var s = _v0.a;
-            return '-' + (s + '-');
-        } else {
-            return '-';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass = function(_v0) {
-        var screenSize = _v0.eD;
-        var offsetCount = _v0.el;
-        return $elm$html$Html$Attributes$class(
-            'offset' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption(offsetCount)));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes = function(offsets) {
-        var offset_ = function(m) {
-            return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass, m);
-        };
-        return A2(
-            $elm$core$List$filterMap,
-            $elm$core$Basics$identity,
-            A2($elm$core$List$map, offset_, offsets));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderColOption = function(size) {
-        switch (size) {
-            case 0:
-                return 'first';
-            case 1:
-                return '1';
-            case 2:
-                return '2';
-            case 3:
-                return '3';
-            case 4:
-                return '4';
-            case 5:
-                return '5';
-            case 6:
-                return '6';
-            case 7:
-                return '7';
-            case 8:
-                return '8';
-            case 9:
-                return '9';
-            case 10:
-                return '10';
-            case 11:
-                return '11';
-            case 12:
-                return '12';
-            default:
-                return 'last';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes = function(orders) {
-        var order_ = function(m) {
-            if (!m.$) {
-                var screenSize = m.a.eD;
-                var moveCount = m.a.aA;
-                return $elm$core$Maybe$Just(
-                    $elm$html$Html$Attributes$class(
-                        'order' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderColOption(moveCount))));
-            } else {
-                return $elm$core$Maybe$Nothing;
-            }
-        };
-        return A2(
-            $elm$core$List$filterMap,
-            $elm$core$Basics$identity,
-            A2($elm$core$List$map, order_, orders));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption = function(size) {
-        switch (size) {
-            case 0:
-                return '0';
-            case 1:
-                return '1';
-            case 2:
-                return '2';
-            case 3:
-                return '3';
-            case 4:
-                return '4';
-            case 5:
-                return '5';
-            case 6:
-                return '6';
-            case 7:
-                return '7';
-            case 8:
-                return '8';
-            case 9:
-                return '9';
-            case 10:
-                return '10';
-            case 11:
-                return '11';
-            default:
-                return '12';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes = function(pulls) {
-        var pull_ = function(m) {
-            if (!m.$) {
-                var screenSize = m.a.eD;
-                var moveCount = m.a.aA;
-                return $elm$core$Maybe$Just(
-                    $elm$html$Html$Attributes$class(
-                        'pull' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
-            } else {
-                return $elm$core$Maybe$Nothing;
-            }
-        };
-        return A2(
-            $elm$core$List$filterMap,
-            $elm$core$Basics$identity,
-            A2($elm$core$List$map, pull_, pulls));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes = function(pushes) {
-        var push_ = function(m) {
-            if (!m.$) {
-                var screenSize = m.a.eD;
-                var moveCount = m.a.aA;
-                return $elm$core$Maybe$Just(
-                    $elm$html$Html$Attributes$class(
-                        'push' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
-            } else {
-                return $elm$core$Maybe$Nothing;
-            }
-        };
-        return A2(
-            $elm$core$List$filterMap,
-            $elm$core$Basics$identity,
-            A2($elm$core$List$map, push_, pushes));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignDirOption = function(dir) {
-        switch (dir) {
-            case 1:
-                return 'center';
-            case 0:
-                return 'left';
-            default:
-                return 'right';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass = function(_v0) {
-        var dir = _v0.dP;
-        var size = _v0.eG;
-        return $elm$html$Html$Attributes$class(
-            'text' + (A2(
-                $elm$core$Maybe$withDefault,
-                '-',
-                A2(
-                    $elm$core$Maybe$map,
-                    function(s) {
-                        return '-' + (s + '-');
-                    },
-                    $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(size))) + $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignDirOption(dir)));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$verticalAlignOption = function(align) {
-        switch (align) {
-            case 0:
-                return 'start';
-            case 1:
-                return 'center';
-            default:
-                return 'end';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignClass = F2(
-        function(prefix, _v0) {
-            var align = _v0.dE;
-            var screenSize = _v0.eD;
-            return $elm$html$Html$Attributes$class(
-                _Utils_ap(
-                    prefix,
-                    _Utils_ap(
-                        A2(
-                            $elm$core$Maybe$withDefault,
-                            '',
-                            A2(
-                                $elm$core$Maybe$map,
-                                function(v) {
-                                    return v + '-';
-                                },
-                                $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize))),
-                        $rundis$elm_bootstrap$Bootstrap$Grid$Internal$verticalAlignOption(align))));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes = F2(
-        function(prefix, aligns) {
-            var align = function(a) {
-                return A2(
-                    $elm$core$Maybe$map,
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignClass(prefix),
-                    a);
-            };
-            return A2(
-                $elm$core$List$filterMap,
-                $elm$core$Basics$identity,
-                A2($elm$core$List$map, align, aligns));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes = function(modifiers) {
-        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions, modifiers);
-        var shouldAddDefaultXs = !$elm$core$List$length(
-            A2(
-                $elm$core$List$filterMap,
-                $elm$core$Basics$identity,
-                _List_fromArray(
-                    [options.a9, options.a7, options.a6, options.a5, options.a8])));
-        return _Utils_ap(
-            $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthsToAttributes(
-                _List_fromArray(
-                    [
-                        shouldAddDefaultXs ? $elm$core$Maybe$Just(
-                            A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, 0, 0)) : options.a9,
-                        options.a7,
-                        options.a6,
-                        options.a5,
-                        options.a8
-                    ])),
-            _Utils_ap(
-                $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes(
-                    _List_fromArray(
-                        [options.b2, options.b$, options.b_, options.bZ, options.b1])),
-                _Utils_ap(
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes(
-                        _List_fromArray(
-                            [options.ci, options.cg, options.cf, options.ce, options.ch])),
-                    _Utils_ap(
-                        $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes(
-                            _List_fromArray(
-                                [options.cn, options.cl, options.ck, options.cj, options.cm])),
-                        _Utils_ap(
-                            $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes(
-                                _List_fromArray(
-                                    [options.cc, options.ca, options.b9, options.b8, options.cb])),
-                            _Utils_ap(
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
-                                    'align-self-',
-                                    _List_fromArray(
-                                        [options.bl, options.bj, options.bi, options.bh, options.bk])),
-                                _Utils_ap(
-                                    function() {
-                                        var _v0 = options.cz;
-                                        if (!_v0.$) {
-                                            var a = _v0.a;
-                                            return _List_fromArray(
-                                                [
-                                                    $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass(a)
-                                                ]);
-                                        } else {
-                                            return _List_Nil;
-                                        }
-                                    }(),
-                                    options.bp)))))));
-    };
-    var $elm$virtual_dom$VirtualDom$keyedNode = function(tag) {
-        return _VirtualDom_keyedNode(
-            _VirtualDom_noScript(tag));
-    };
-    var $elm$html$Html$Keyed$node = $elm$virtual_dom$VirtualDom$keyedNode;
-    var $rundis$elm_bootstrap$Bootstrap$Grid$renderCol = function(column) {
-        switch (column.$) {
-            case 0:
-                var options = column.a.db;
-                var children = column.a.dJ;
-                return A2(
-                    $elm$html$Html$div,
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
-                    children);
-            case 1:
-                var e = column.a;
-                return e;
-            default:
-                var options = column.a.db;
-                var children = column.a.dJ;
-                return A3(
-                    $elm$html$Html$Keyed$node,
-                    'div',
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
-                    children);
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign = F2(
-        function(align, options) {
-            var _v0 = align.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            bN: $elm$core$Maybe$Just(align)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            bL: $elm$core$Maybe$Just(align)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            bK: $elm$core$Maybe$Just(align)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            bJ: $elm$core$Maybe$Just(align)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            bM: $elm$core$Maybe$Just(align)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign = F2(
-        function(align_, options) {
-            var _v0 = align_.eD;
-            switch (_v0) {
-                case 0:
-                    return _Utils_update(
-                        options, {
-                            cJ: $elm$core$Maybe$Just(align_)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            cH: $elm$core$Maybe$Just(align_)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            cG: $elm$core$Maybe$Just(align_)
-                        });
-                case 3:
-                    return _Utils_update(
-                        options, {
-                            cF: $elm$core$Maybe$Just(align_)
-                        });
-                default:
-                    return _Utils_update(
-                        options, {
-                            cI: $elm$core$Maybe$Just(align_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowOption = F2(
-        function(modifier, options) {
-            switch (modifier.$) {
-                case 2:
-                    var attrs = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            bp: _Utils_ap(options.bp, attrs)
-                        });
-                case 0:
-                    var align = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign, align, options);
-                default:
-                    var align = modifier.a;
-                    return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign, align, options);
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultRowOptions = {
-        bp: _List_Nil,
-        bJ: $elm$core$Maybe$Nothing,
-        bK: $elm$core$Maybe$Nothing,
-        bL: $elm$core$Maybe$Nothing,
-        bM: $elm$core$Maybe$Nothing,
-        bN: $elm$core$Maybe$Nothing,
-        cF: $elm$core$Maybe$Nothing,
-        cG: $elm$core$Maybe$Nothing,
-        cH: $elm$core$Maybe$Nothing,
-        cI: $elm$core$Maybe$Nothing,
-        cJ: $elm$core$Maybe$Nothing
-    };
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$horizontalAlignOption = function(align) {
-        switch (align) {
-            case 0:
-                return 'start';
-            case 1:
-                return 'center';
-            case 2:
-                return 'end';
-            case 3:
-                return 'around';
-            default:
-                return 'between';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$hAlignClass = function(_v0) {
-        var align = _v0.dE;
-        var screenSize = _v0.eD;
-        return $elm$html$Html$Attributes$class(
-            'justify-content-' + (A2(
-                $elm$core$Maybe$withDefault,
-                '',
-                A2(
-                    $elm$core$Maybe$map,
-                    function(v) {
-                        return v + '-';
-                    },
-                    $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(screenSize))) + $rundis$elm_bootstrap$Bootstrap$General$Internal$horizontalAlignOption(align)));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$hAlignsToAttributes = function(aligns) {
-        var align = function(a) {
-            return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$General$Internal$hAlignClass, a);
-        };
-        return A2(
-            $elm$core$List$filterMap,
-            $elm$core$Basics$identity,
-            A2($elm$core$List$map, align, aligns));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowAttributes = function(modifiers) {
-        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowOption, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultRowOptions, modifiers);
-        return _Utils_ap(
-            _List_fromArray(
-                [
-                    $elm$html$Html$Attributes$class('row')
-                ]),
-            _Utils_ap(
-                A2(
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
-                    'align-items-',
-                    _List_fromArray(
-                        [options.cJ, options.cH, options.cG, options.cF, options.cI])),
-                _Utils_ap(
-                    $rundis$elm_bootstrap$Bootstrap$Grid$Internal$hAlignsToAttributes(
-                        _List_fromArray(
-                            [options.bN, options.bL, options.bK, options.bJ, options.bM])),
-                    options.bp)));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$row = F2(
-        function(options, cols) {
-            return A2(
-                $elm$html$Html$div,
-                $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowAttributes(options),
-                A2($elm$core$List$map, $rundis$elm_bootstrap$Bootstrap$Grid$renderCol, cols));
-        });
-    var $elm$html$Html$Attributes$src = function(url) {
-        return A2(
-            $elm$html$Html$Attributes$stringProperty,
-            'src',
-            _VirtualDom_noJavaScriptOrHtmlUri(url));
-    };
-    var $elm$html$Html$text = $elm$virtual_dom$VirtualDom$text;
-    var $author$project$DeviceStatus$getDeviceInfo = function(deviceInfo) {
-        return A2(
-            $rundis$elm_bootstrap$Bootstrap$Grid$container,
-            _List_Nil,
-            _List_fromArray(
-                [
-                    A2(
-                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                        _List_fromArray(
-                            [
-                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
-                                    _List_fromArray(
-                                        [
-                                            $elm$html$Html$Attributes$class('align-items-center')
-                                        ]))
-                            ]),
-                        _List_fromArray(
-                            [
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                    _List_fromArray(
-                                        [
-                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
-                                                _List_fromArray(
-                                                    [
-                                                        A2($elm$html$Html$Attributes$style, 'max-width', '64px'),
-                                                        A2($elm$html$Html$Attributes$style, 'margin-right', '1em')
-                                                    ]))
-                                        ]),
-                                    _List_fromArray(
-                                        [
-                                            A2(
-                                                $elm$html$Html$img,
-                                                _List_fromArray(
-                                                    [
-                                                        $elm$html$Html$Attributes$src(
-                                                            $author$project$DeviceStatus$deviceStatusImage(deviceInfo.cy))
-                                                    ]),
-                                                _List_Nil)
-                                        ])),
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                    _List_Nil,
-                                    _List_fromArray(
-                                        [
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                                _List_Nil,
-                                                _List_fromArray(
-                                                    [
-                                                        A2(
-                                                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                            _List_Nil,
-                                                            _List_fromArray(
-                                                                [
-                                                                    A2(
-                                                                        $elm$html$Html$h5,
-                                                                        _List_fromArray(
-                                                                            [
-                                                                                A2(
-                                                                                    $elm$html$Html$Attributes$style,
-                                                                                    'color',
-                                                                                    $author$project$DeviceStatus$deviceStatusColor(deviceInfo.cy))
-                                                                            ]),
-                                                                        _List_fromArray(
-                                                                            [
-                                                                                $elm$html$Html$text(
-                                                                                    $author$project$DeviceStatus$deviceStatusToString(deviceInfo.cy))
-                                                                            ]))
-                                                                ]))
-                                                    ])),
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                                _List_Nil,
-                                                _List_fromArray(
-                                                    [
-                                                        A2(
-                                                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                            _List_Nil,
-                                                            _List_fromArray(
-                                                                [
-                                                                    $elm$html$Html$text(
-                                                                        A2($elm$core$Maybe$withDefault, '', deviceInfo.ec))
-                                                                ]))
-                                                    ]))
-                                        ]))
-                            ]))
-                ]));
-    };
     var $terezka$elm_charts$Internal$Events$Decoder = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Many$apply = F2(
         function(_v0, items) {
             var func = _v0.b;
             return func(items);
         });
     var $terezka$elm_charts$Internal$Svg$closestPoint = F2(
         function(pos, searched) {
             return {
-                eZ: A3($elm$core$Basics$clamp, pos.aF, pos.bb, searched.eZ),
-                e_: A3($elm$core$Basics$clamp, pos.gg, pos.dB, searched.e_)
+                fg: A3($elm$core$Basics$clamp, pos.aK, pos.bf, searched.fg),
+                fh: A3($elm$core$Basics$clamp, pos.gx, pos.dL, searched.fh)
             };
         });
     var $elm$core$Basics$abs = function(n) {
         return (n < 0) ? (-n) : n;
     };
     var $terezka$elm_charts$Internal$Svg$distanceX = F3(
         function(plane, searched, point) {
             return $elm$core$Basics$abs(
-                A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, point.eZ) - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, searched.eZ));
+                A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, point.fg) - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, searched.fg));
         });
     var $terezka$elm_charts$Internal$Svg$distanceY = F3(
         function(plane, searched, point) {
             return $elm$core$Basics$abs(
-                A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, point.e_) - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, searched.e_));
+                A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, point.fh) - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, searched.fh));
         });
     var $elm$core$Basics$pow = _Basics_pow;
     var $terezka$elm_charts$Internal$Svg$distanceSquared = F3(
         function(plane, searched, point) {
             return A2(
                 $elm$core$Basics$pow,
                 A3($terezka$elm_charts$Internal$Svg$distanceX, plane, searched, point),
@@ -10265,15 +10542,15 @@
                 $elm$core$Basics$pow,
                 A3($terezka$elm_charts$Internal$Svg$distanceY, plane, searched, point),
                 2);
         });
     var $terezka$elm_charts$Internal$Svg$keepOne = function(toPosition) {
         var toArea = function(a) {
             return function(pos) {
-                return (pos.aF - pos.bb) * (pos.gg - pos.dB);
+                return (pos.aK - pos.bf) * (pos.gx - pos.dL);
             }(
                 toPosition(a));
         };
         var func = F2(
             function(one, acc) {
                 var _v0 = $elm$core$List$head(acc);
                 if (_v0.$ === 1) {
@@ -10336,341 +10613,60 @@
                     $terezka$elm_charts$Internal$Svg$getNearest,
                     toPos(plane),
                     groups,
                     plane);
             });
     };
     var $terezka$elm_charts$Chart$Events$getNearest = $terezka$elm_charts$Internal$Events$getNearest;
-    var $author$project$Main$ChangeWindow = function(a) {
-        return {
-            $: 4,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Attrs = function(a) {
-        return {
-            $: 4,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Button$attrs = function(attrs_) {
-        return $rundis$elm_bootstrap$Bootstrap$Internal$Button$Attrs(attrs_);
-    };
-    var $elm$virtual_dom$VirtualDom$MayPreventDefault = function(a) {
-        return {
-            $: 2,
-            a: a
-        };
-    };
-    var $elm$html$Html$Events$preventDefaultOn = F2(
-        function(event, decoder) {
-            return A2(
-                $elm$virtual_dom$VirtualDom$on,
-                event,
-                $elm$virtual_dom$VirtualDom$MayPreventDefault(decoder));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Button$onClick = function(message) {
-        return $rundis$elm_bootstrap$Bootstrap$Button$attrs(
-            _List_fromArray(
-                [
-                    A2(
-                        $elm$html$Html$Events$preventDefaultOn,
-                        'click',
-                        $elm$json$Json$Decode$succeed(
-                            _Utils_Tuple2(message, true)))
-                ]));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring = function(a) {
-        return {
-            $: 1,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined = function(a) {
-        return {
-            $: 1,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Primary = 0;
-    var $rundis$elm_bootstrap$Bootstrap$Button$outlinePrimary = $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring(
-        $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined(0));
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$RadioButtonItem = $elm$core$Basics$identity;
-    var $elm$virtual_dom$VirtualDom$attribute = F2(
-        function(key, value) {
-            return A2(
-                _VirtualDom_attribute,
-                _VirtualDom_noOnOrFormAction(key),
-                _VirtualDom_noJavaScriptOrHtmlUri(value));
-        });
-    var $elm$html$Html$Attributes$attribute = $elm$virtual_dom$VirtualDom$attribute;
-    var $elm$html$Html$Attributes$autocomplete = function(bool) {
-        return A2(
-            $elm$html$Html$Attributes$stringProperty,
-            'autocomplete',
-            bool ? 'on' : 'off');
-    };
-    var $elm$core$Maybe$andThen = F2(
-        function(callback, maybeValue) {
-            if (!maybeValue.$) {
-                var value = maybeValue.a;
-                return callback(value);
-            } else {
-                return $elm$core$Maybe$Nothing;
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$applyModifier = F2(
-        function(modifier, options) {
-            switch (modifier.$) {
-                case 0:
-                    var size = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            eG: $elm$core$Maybe$Just(size)
-                        });
-                case 1:
-                    var coloring = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            X: $elm$core$Maybe$Just(coloring)
-                        });
-                case 2:
-                    return _Utils_update(
-                        options, {
-                            bs: true
-                        });
-                case 3:
-                    var val = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            bE: val
-                        });
-                default:
-                    var attrs = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            bp: _Utils_ap(options.bp, attrs)
-                        });
-            }
-        });
-    var $elm$core$List$filter = F2(
-        function(isGood, list) {
-            return A3(
-                $elm$core$List$foldr,
-                F2(
-                    function(x, xs) {
-                        return isGood(x) ? A2($elm$core$List$cons, x, xs) : xs;
-                    }),
-                _List_Nil,
-                list);
-        });
-    var $elm$core$Tuple$second = function(_v0) {
-        var y = _v0.b;
-        return y;
-    };
-    var $elm$html$Html$Attributes$classList = function(classes) {
-        return $elm$html$Html$Attributes$class(
-            A2(
-                $elm$core$String$join,
-                ' ',
-                A2(
-                    $elm$core$List$map,
-                    $elm$core$Tuple$first,
-                    A2($elm$core$List$filter, $elm$core$Tuple$second, classes))));
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$defaultOptions = {
-        bp: _List_Nil,
-        bs: false,
-        X: $elm$core$Maybe$Nothing,
-        bE: false,
-        eG: $elm$core$Maybe$Nothing
-    };
-    var $elm$json$Json$Encode$bool = _Json_wrap;
-    var $elm$html$Html$Attributes$boolProperty = F2(
-        function(key, bool) {
-            return A2(
-                _VirtualDom_property,
-                key,
-                $elm$json$Json$Encode$bool(bool));
-        });
-    var $elm$html$Html$Attributes$disabled = $elm$html$Html$Attributes$boolProperty('disabled');
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass = function(role) {
-        switch (role) {
-            case 0:
-                return 'primary';
-            case 1:
-                return 'secondary';
-            case 2:
-                return 'success';
-            case 3:
-                return 'info';
-            case 4:
-                return 'warning';
-            case 5:
-                return 'danger';
-            case 6:
-                return 'dark';
-            case 7:
-                return 'light';
-            default:
-                return 'link';
-        }
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$buttonAttributes = function(modifiers) {
-        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Internal$Button$applyModifier, $rundis$elm_bootstrap$Bootstrap$Internal$Button$defaultOptions, modifiers);
-        return _Utils_ap(
-            _List_fromArray(
-                [
-                    $elm$html$Html$Attributes$classList(
-                        _List_fromArray(
-                            [
-                                _Utils_Tuple2('btn', true),
-                                _Utils_Tuple2('btn-block', options.bs),
-                                _Utils_Tuple2('disabled', options.bE)
-                            ])),
-                    $elm$html$Html$Attributes$disabled(options.bE)
-                ]),
-            _Utils_ap(
-                function() {
-                    var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.eG);
-                    if (!_v0.$) {
-                        var s = _v0.a;
-                        return _List_fromArray(
-                            [
-                                $elm$html$Html$Attributes$class('btn-' + s)
-                            ]);
-                    } else {
-                        return _List_Nil;
-                    }
-                }(),
-                _Utils_ap(
-                    function() {
-                        var _v1 = options.X;
-                        if (!_v1.$) {
-                            if (!_v1.a.$) {
-                                var role = _v1.a.a;
-                                return _List_fromArray(
-                                    [
-                                        $elm$html$Html$Attributes$class(
-                                            'btn-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
-                                    ]);
-                            } else {
-                                var role = _v1.a.a;
-                                return _List_fromArray(
-                                    [
-                                        $elm$html$Html$Attributes$class(
-                                            'btn-outline-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
-                                    ]);
-                            }
-                        } else {
-                            return _List_Nil;
-                        }
-                    }(),
-                    options.bp)));
-    };
-    var $elm$html$Html$Attributes$checked = $elm$html$Html$Attributes$boolProperty('checked');
-    var $elm$html$Html$input = _VirtualDom_node('input');
-    var $elm$html$Html$label = _VirtualDom_node('label');
-    var $elm$html$Html$Attributes$type_ = $elm$html$Html$Attributes$stringProperty('type');
-    var $rundis$elm_bootstrap$Bootstrap$Button$radioButton = F3(
-        function(checked, options, children) {
-            var hideRadio = A2($elm$html$Html$Attributes$attribute, 'data-toggle', 'button');
-            return A2(
-                $elm$html$Html$label,
-                A2(
-                    $elm$core$List$cons,
-                    $elm$html$Html$Attributes$classList(
-                        _List_fromArray(
-                            [
-                                _Utils_Tuple2('active', checked)
-                            ])),
-                    A2(
-                        $elm$core$List$cons,
-                        hideRadio,
-                        $rundis$elm_bootstrap$Bootstrap$Internal$Button$buttonAttributes(options))),
-                A2(
-                    $elm$core$List$cons,
-                    A2(
-                        $elm$html$Html$input,
-                        _List_fromArray(
-                            [
-                                $elm$html$Html$Attributes$type_('radio'),
-                                $elm$html$Html$Attributes$checked(checked),
-                                $elm$html$Html$Attributes$autocomplete(false)
-                            ]),
-                        _List_Nil),
-                    children));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButton = F3(
-        function(checked, options, children) {
-            return A3($rundis$elm_bootstrap$Bootstrap$Button$radioButton, checked, options, children);
-        });
-    var $author$project$Main$getSelector = F3(
-        function(windowDuration, textDuration, currentDuration) {
-            return A3(
-                $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButton,
-                _Utils_eq(windowDuration, currentDuration),
-                _List_fromArray(
-                    [
-                        $rundis$elm_bootstrap$Bootstrap$Button$outlinePrimary,
-                        $rundis$elm_bootstrap$Bootstrap$Button$onClick(
-                            $author$project$Main$ChangeWindow(windowDuration))
-                    ]),
-                _List_fromArray(
-                    [
-                        $elm$html$Html$text(textDuration)
-                    ]));
-        });
-    var $elm$html$Html$h1 = _VirtualDom_node('h1');
     var $terezka$elm_charts$Chart$Attributes$height = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    d$: v
+                    eb: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$htmlAttrs = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    bR: v
+                    bY: v
                 });
         });
     var $terezka$elm_charts$Internal$Svg$Linear = 0;
     var $terezka$elm_charts$Chart$Attributes$linear = function(config) {
         return _Utils_update(
             config, {
-                fC: $elm$core$Maybe$Just(0)
+                fU: $elm$core$Maybe$Just(0)
             });
     };
     var $terezka$elm_charts$Internal$Property$Property = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Property$property = F3(
         function(value, inter, attrs) {
             return $terezka$elm_charts$Internal$Property$Property({
-                bq: attrs,
-                dV: F5(
+                bv: attrs,
+                d5: F5(
                     function(_v0, _v1, _v2, _v3, _v4) {
                         return _List_Nil;
                     }),
                 F: A2(
                     $elm$core$Basics$composeR,
                     value,
                     A2(
                         $elm$core$Basics$composeR,
                         $elm$core$Maybe$map($elm$core$String$fromFloat),
                         $elm$core$Maybe$withDefault('N/A'))),
-                fv: inter,
-                ef: $elm$core$Maybe$Nothing,
-                U: value,
-                a4: value
+                fO: inter,
+                es: $elm$core$Maybe$Nothing,
+                W: value,
+                a8: value
             });
         });
     var $terezka$elm_charts$Chart$interpolated = F2(
         function(y, inter) {
             return A2(
                 $terezka$elm_charts$Internal$Property$property,
                 A2($elm$core$Basics$composeR, y, $elm$core$Maybe$Just),
@@ -10684,21 +10680,21 @@
             $: 13,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Coordinates$Axis = F7(
         function(length, marginMin, marginMax, dataMin, dataMax, min, max) {
             return {
-                fc: dataMax,
-                fd: dataMin,
+                fv: dataMax,
+                fw: dataMin,
                 N: length,
-                fz: marginMax,
-                fA: marginMin,
-                fB: max,
-                fD: min
+                fS: marginMax,
+                fT: marginMin,
+                er: max,
+                et: min
             };
         });
     var $terezka$elm_charts$Internal$Svg$apply = F2(
         function(funcs, _default) {
             var apply_ = F2(
                 function(f, a) {
                     return f(a);
@@ -10787,83 +10783,83 @@
             var _v0 = function() {
                 switch (design.$) {
                     case 0:
                         var edits = design.a;
                         var config = A2(
                             $terezka$elm_charts$Internal$Svg$apply,
                             edits, {
-                                by: defaultColor,
+                                bD: defaultColor,
                                 o: 45,
-                                fR: 4,
-                                eY: 3
+                                f6: 4,
+                                ff: 3
                             });
                         var theId = toPatternId(
                             _List_fromArray(
                                 [
-                                    config.by,
-                                    $elm$core$String$fromFloat(config.eY),
-                                    $elm$core$String$fromFloat(config.fR),
+                                    config.bD,
+                                    $elm$core$String$fromFloat(config.ff),
+                                    $elm$core$String$fromFloat(config.f6),
                                     $elm$core$String$fromFloat(config.o)
                                 ]));
                         return _Utils_Tuple2(
                             A4(
                                 toPatternDefs,
                                 theId,
-                                config.fR,
+                                config.f6,
                                 config.o,
                                 A2(
                                     $elm$svg$Svg$line,
                                     _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x1('0'),
                                             $elm$svg$Svg$Attributes$y('0'),
                                             $elm$svg$Svg$Attributes$x2('0'),
                                             $elm$svg$Svg$Attributes$y2(
-                                                $elm$core$String$fromFloat(config.fR)),
-                                            $elm$svg$Svg$Attributes$stroke(config.by),
+                                                $elm$core$String$fromFloat(config.f6)),
+                                            $elm$svg$Svg$Attributes$stroke(config.bD),
                                             $elm$svg$Svg$Attributes$strokeWidth(
-                                                $elm$core$String$fromFloat(config.eY))
+                                                $elm$core$String$fromFloat(config.ff))
                                         ]),
                                     _List_Nil)),
                             theId);
                     case 1:
                         var edits = design.a;
                         var config = A2(
                             $terezka$elm_charts$Internal$Svg$apply,
                             edits, {
-                                by: defaultColor,
+                                bD: defaultColor,
                                 o: 45,
-                                fR: 4,
-                                eY: 3
+                                f6: 4,
+                                ff: 3
                             });
                         var theId = toPatternId(
                             _List_fromArray(
                                 [
-                                    config.by,
-                                    $elm$core$String$fromFloat(config.eY),
-                                    $elm$core$String$fromFloat(config.fR),
+                                    config.bD,
+                                    $elm$core$String$fromFloat(config.ff),
+                                    $elm$core$String$fromFloat(config.f6),
                                     $elm$core$String$fromFloat(config.o)
                                 ]));
                         return _Utils_Tuple2(
                             A4(
                                 toPatternDefs,
                                 theId,
-                                config.fR,
+                                config.f6,
                                 config.o,
                                 A2(
                                     $elm$svg$Svg$circle,
                                     _List_fromArray(
                                         [
-                                            $elm$svg$Svg$Attributes$fill(config.by),
+                                            $elm$svg$Svg$Attributes$fill(config.bD),
                                             $elm$svg$Svg$Attributes$cx(
-                                                $elm$core$String$fromFloat(config.eY / 3)),
+                                                $elm$core$String$fromFloat(config.ff / 3)),
                                             $elm$svg$Svg$Attributes$cy(
-                                                $elm$core$String$fromFloat(config.eY / 3)),
+                                                $elm$core$String$fromFloat(config.ff / 3)),
                                             $elm$svg$Svg$Attributes$r(
-                                                $elm$core$String$fromFloat(config.eY / 3))
+                                                $elm$core$String$fromFloat(config.ff / 3))
                                         ]),
                                     _List_Nil)),
                             theId);
                     default:
                         var edits = design.a;
                         var colors = _Utils_eq(edits, _List_Nil) ? _List_fromArray(
                             [defaultColor, 'white']) : edits;
@@ -10912,15 +10908,15 @@
         });
     var $terezka$elm_charts$Internal$Svg$bar = F3(
         function(plane, config, point) {
             var viewBar = F6(
                 function(fill, fillOpacity, border, borderWidth, strokeOpacity, cmds) {
                     return A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bq,
+                        config.bv,
                         $elm$svg$Svg$path,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__bar'),
                                 $elm$svg$Svg$Attributes$fill(fill),
                                 $elm$svg$Svg$Attributes$fillOpacity(
                                     $elm$core$String$fromFloat(fillOpacity)),
@@ -10931,185 +10927,185 @@
                                     $elm$core$String$fromFloat(strokeOpacity)),
                                 $elm$svg$Svg$Attributes$d(
                                     A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                                 $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                             ]),
                         _List_Nil);
                 });
-            var highlightColor = (config.fp === '') ? config.by : config.fp;
+            var highlightColor = (config.fI === '') ? config.bD : config.fI;
             var borderWidthCarY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.x / 2);
-            var highlightWidthCarY = borderWidthCarY + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.fq / 2);
+            var highlightWidthCarY = borderWidthCarY + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.fJ / 2);
             var borderWidthCarX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.x / 2);
-            var highlightWidthCarX = borderWidthCarX + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.fq / 2);
+            var highlightWidthCarX = borderWidthCarX + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.fJ / 2);
             var pos = {
-                aF: A2($elm$core$Basics$min, point.aF, point.bb) + borderWidthCarX,
-                bb: A2($elm$core$Basics$max, point.aF, point.bb) - borderWidthCarX,
-                gg: A2($elm$core$Basics$min, point.gg, point.dB) + borderWidthCarY,
-                dB: A2($elm$core$Basics$max, point.gg, point.dB) - borderWidthCarY
+                aK: A2($elm$core$Basics$min, point.aK, point.bf) + borderWidthCarX,
+                bf: A2($elm$core$Basics$max, point.aK, point.bf) - borderWidthCarX,
+                gx: A2($elm$core$Basics$min, point.gx, point.dL) + borderWidthCarY,
+                dL: A2($elm$core$Basics$max, point.gx, point.dL) - borderWidthCarY
             };
-            var height = $elm$core$Basics$abs(pos.dB - pos.gg);
+            var height = $elm$core$Basics$abs(pos.dL - pos.gx);
             var highlightPos = {
-                aF: pos.aF - highlightWidthCarX,
-                bb: pos.bb + highlightWidthCarX,
-                gg: pos.gg - highlightWidthCarY,
-                dB: pos.dB + highlightWidthCarY
+                aK: pos.aK - highlightWidthCarX,
+                bf: pos.bf + highlightWidthCarX,
+                gx: pos.gx - highlightWidthCarY,
+                dL: pos.dL + highlightWidthCarY
             };
-            var width = $elm$core$Basics$abs(pos.bb - pos.aF);
-            var roundingBottom = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.fO);
+            var width = $elm$core$Basics$abs(pos.bf - pos.aK);
+            var roundingBottom = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f3);
             var radiusBottomX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, roundingBottom);
             var radiusBottomY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, roundingBottom);
-            var roundingTop = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.fP);
+            var roundingTop = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f4);
             var radiusTopX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, roundingTop);
             var radiusTopY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, roundingTop);
-            var _v0 = ((((height - (radiusTopY * 0.8)) - (radiusBottomY * 0.8)) <= 0) || (((width - (radiusTopX * 0.8)) - (radiusBottomX * 0.8)) <= 0)) ? _Utils_Tuple2(0, 0) : _Utils_Tuple2(config.fP, config.fO);
+            var _v0 = ((((height - (radiusTopY * 0.8)) - (radiusBottomY * 0.8)) <= 0) || (((width - (radiusTopX * 0.8)) - (radiusBottomX * 0.8)) <= 0)) ? _Utils_Tuple2(0, 0) : _Utils_Tuple2(config.f4, config.f3);
             var roundTop = _v0.a;
             var roundBottom = _v0.b;
             var _v1 = function() {
-                if (_Utils_eq(pos.gg, pos.dB)) {
+                if (_Utils_eq(pos.gx, pos.dL)) {
                     return _Utils_Tuple2(_List_Nil, _List_Nil);
                 } else {
                     var _v2 = _Utils_Tuple2(roundTop > 0, roundBottom > 0);
                     if (!_v2.a) {
                         if (!_v2.b) {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aF, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aF, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aF, highlightPos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb, highlightPos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
                                     ]));
                         } else {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aF + radiusBottomX, pos.gg),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aF, pos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bb - radiusBottomX, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF + radiusBottomX, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gx),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bf - radiusBottomX, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gx)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aF + radiusBottomX, highlightPos.gg),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aF, highlightPos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aF, highlightPos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb, highlightPos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb, highlightPos.gg + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bb - radiusBottomX, highlightPos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aF + radiusBottomX, highlightPos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb - radiusBottomX, pos.gg),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bb, pos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gx),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.gx + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bf - radiusBottomX, highlightPos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusBottomX, pos.gx),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bf, pos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx)
                                     ]));
                         }
                     } else {
                         if (!_v2.b) {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aF, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.dB - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aF + radiusTopX, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb - radiusTopX, pos.dB),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bb, pos.dB - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusTopX, pos.dL),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bf, pos.dL - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aF, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aF, highlightPos.dB - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aF + radiusTopX, highlightPos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb - radiusTopX, highlightPos.dB),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bb, highlightPos.dB - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.dB - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bb - radiusTopX, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF + radiusTopX, pos.dB),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aF, pos.dB - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf - radiusTopX, highlightPos.dL),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bf, highlightPos.dL - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bf - radiusTopX, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dL),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dL - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
                                     ]));
                         } else {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aF + radiusBottomX, pos.gg),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aF, pos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.dB - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aF + radiusTopX, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb - radiusTopX, pos.dB),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bb, pos.dB - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bb - radiusBottomX, pos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF + radiusBottomX, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gx),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusTopX, pos.dL),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bf, pos.dL - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bf - radiusBottomX, pos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gx)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aF + radiusBottomX, highlightPos.gg),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aF, highlightPos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aF, highlightPos.dB - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aF + radiusTopX, highlightPos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb - radiusTopX, highlightPos.dB),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bb, highlightPos.dB - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bb, highlightPos.gg + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bb - radiusBottomX, highlightPos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aF + radiusBottomX, highlightPos.gg),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb - radiusBottomX, pos.gg),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bb, pos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.dB - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bb - radiusTopX, pos.dB),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF + radiusTopX, pos.dB),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aF, pos.dB - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aF, pos.gg + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bb, pos.gg)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gx),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf - radiusTopX, highlightPos.dL),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bf, highlightPos.dL - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.gx + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bf - radiusBottomX, highlightPos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gx),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusBottomX, pos.gx),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bf, pos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bf - radiusTopX, pos.dL),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dL),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dL - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx)
                                     ]));
                         }
                     }
                 }
             }();
             var commands = _v1.a;
             var highlightCommands = _v1.b;
             var viewAuraBar = function(fill) {
-                return (!config.fo) ? A6(viewBar, fill, config.P, config.v, config.x, 1, commands) : A2(
+                return (!config.fH) ? A6(viewBar, fill, config.P, config.v, config.x, 1, commands) : A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__bar-with-highlight')
                         ]),
                     _List_fromArray(
                         [
-                            A6(viewBar, highlightColor, config.fo, 'transparent', 0, 0, highlightCommands),
+                            A6(viewBar, highlightColor, config.fH, 'transparent', 0, 0, highlightCommands),
                             A6(viewBar, fill, config.P, config.v, config.x, 1, commands)
                         ]));
             };
-            var _v3 = config.cR;
+            var _v3 = config.cX;
             if (_v3.$ === 1) {
-                return viewAuraBar(config.by);
+                return viewAuraBar(config.bD);
             } else {
                 var design = _v3.a;
-                var _v4 = A2($terezka$elm_charts$Internal$Svg$toPattern, config.by, design);
+                var _v4 = A2($terezka$elm_charts$Internal$Svg$toPattern, config.bD, design);
                 var patternDefs = _v4.a;
                 var fill = _v4.b;
                 return A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__bar-with-pattern')
@@ -11118,21 +11114,21 @@
                         [
                             patternDefs,
                             viewAuraBar(fill)
                         ]));
             }
         });
     var $terezka$elm_charts$Internal$Svg$defaultContainer = {
-        bq: _List_fromArray(
+        bv: _List_fromArray(
             [
                 $elm$svg$Svg$Attributes$style('overflow: visible;')
             ]),
-        bH: _List_Nil,
-        bR: _List_Nil,
-        cq: true
+        bM: _List_Nil,
+        bY: _List_Nil,
+        cx: true
     };
     var $terezka$elm_charts$Internal$Svg$barLegend = F2(
         function(config, barConfig) {
             var fontStyle = function() {
                 var _v0 = config.k;
                 if (!_v0.$) {
                     var size_ = _v0.a;
@@ -11141,118 +11137,118 @@
                         'font-size',
                         $elm$core$String$fromInt(size_) + 'px');
                 } else {
                     return A2($elm$html$Html$Attributes$style, '', '');
                 }
             }();
             var fakePlane = {
-                eZ: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eY, 0, 0, 0, 10, 0, 10),
-                e_: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.d$, 0, 0, 0, 10, 0, 10)
+                fg: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ff, 0, 0, 0, 10, 0, 10),
+                fh: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eb, 0, 0, 0, 10, 0, 10)
             };
             return A2(
                 $elm$html$Html$div,
                 _Utils_ap(
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('elm-charts__legend'),
                             A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                             A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                         ]),
-                    config.bR),
+                    config.bY),
                 _List_fromArray(
                     [
                         A5(
                             $terezka$elm_charts$Internal$Svg$container,
                             fakePlane,
                             _Utils_update(
                                 $terezka$elm_charts$Internal$Svg$defaultContainer, {
-                                    cq: false
+                                    cx: false
                                 }),
                             _List_Nil,
                             _List_fromArray(
                                 [
                                     A3(
                                         $terezka$elm_charts$Internal$Svg$bar,
                                         fakePlane,
                                         barConfig, {
-                                            aF: 0,
-                                            bb: 10,
-                                            gg: 0,
-                                            dB: 10
+                                            aK: 0,
+                                            bf: 10,
+                                            gx: 0,
+                                            dL: 10
                                         })
                                 ]),
                             _List_Nil),
                         A2(
                             $elm$html$Html$div,
                             _List_fromArray(
                                 [
                                     fontStyle,
                                     A2(
                                         $elm$html$Html$Attributes$style,
                                         'margin-left',
-                                        $elm$core$String$fromFloat(config.fR) + 'px')
+                                        $elm$core$String$fromFloat(config.f6) + 'px')
                                 ]),
                             _List_fromArray(
                                 [
-                                    $elm$html$Html$text(config.f_)
+                                    $elm$html$Html$text(config.gf)
                                 ]))
                     ]));
         });
     var $terezka$elm_charts$Internal$Svg$defaultBar = {
-        bq: _List_Nil,
+        bv: _List_Nil,
         v: 'white',
         x: 0,
-        by: $terezka$elm_charts$Internal$Helpers$pink,
-        cR: $elm$core$Maybe$Nothing,
-        fo: 0,
-        fp: '',
-        fq: 10,
+        bD: $terezka$elm_charts$Internal$Helpers$pink,
+        cX: $elm$core$Maybe$Nothing,
+        fH: 0,
+        fI: '',
+        fJ: 10,
         P: 1,
-        fO: 0,
-        fP: 0
+        f3: 0,
+        f4: 0
     };
     var $terezka$elm_charts$Internal$Svg$defaultBarLegend = {
-        by: '#808BAB',
+        bD: '#808BAB',
         k: $elm$core$Maybe$Nothing,
-        d$: 10,
-        bR: _List_Nil,
-        fR: 10,
-        f_: '',
-        eY: 10,
+        eb: 10,
+        bY: _List_Nil,
+        f6: 10,
+        gf: '',
+        ff: 10,
         g: 0,
         h: 0
     };
     var $terezka$elm_charts$Chart$Svg$barLegend = F2(
         function(edits, barAttrs) {
             return A2(
                 $terezka$elm_charts$Internal$Svg$barLegend,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultBarLegend),
                 A2($terezka$elm_charts$Internal$Helpers$apply, barAttrs, $terezka$elm_charts$Internal$Svg$defaultBar));
         });
     var $terezka$elm_charts$Internal$Svg$Row = 0;
     var $terezka$elm_charts$Internal$Svg$defaultLegends = {
-        dF: 0,
+        dP: 0,
         i: $elm$core$Maybe$Nothing,
-        e4: '',
+        fn: '',
         v: '',
         x: 0,
-        bR: _List_Nil,
-        fR: 10,
+        bY: _List_Nil,
+        f6: 10,
         g: 0,
         h: 0
     };
     var $elm$virtual_dom$VirtualDom$node = function(tag) {
         return _VirtualDom_node(
             _VirtualDom_noScript(tag));
     };
     var $elm$html$Html$node = $elm$virtual_dom$VirtualDom$node;
     var $terezka$elm_charts$Internal$Svg$positionHtml = F7(
         function(plane, x, y, xOff, yOff, attrs, content) {
-            var yPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y) - yOff) * 100) / plane.e_.N;
-            var xPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x) + xOff) * 100) / plane.eZ.N;
+            var yPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y) - yOff) * 100) / plane.fh.N;
+            var xPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x) + xOff) * 100) / plane.fg.N;
             var posititonStyles = _List_fromArray(
                 [
                     A2(
                         $elm$html$Html$Attributes$style,
                         'left',
                         $elm$core$String$fromFloat(xPercentage) + '%'),
                     A2(
@@ -11268,15 +11264,15 @@
                 content);
         });
     var $terezka$elm_charts$Internal$Svg$legendsAt = F5(
         function(plane, x, y, config, children) {
             var otherAttrs = _List_fromArray(
                 [
                     $elm$html$Html$Attributes$class('elm-charts__legends'),
-                    A2($elm$html$Html$Attributes$style, 'background', config.e4),
+                    A2($elm$html$Html$Attributes$style, 'background', config.fn),
                     A2($elm$html$Html$Attributes$style, 'border-color', config.v),
                     A2(
                         $elm$html$Html$Attributes$style,
                         'border-width',
                         $elm$core$String$fromFloat(config.x) + 'px'),
                     A2($elm$html$Html$Attributes$style, 'border-style', 'solid')
                 ]);
@@ -11307,15 +11303,15 @@
                                 [
                                     A2($elm$html$Html$Attributes$style, 'transform', 'translate(-50%, 0%)')
                                 ]);
                     }
                 }
             }();
             var _v0 = function() {
-                var _v1 = config.dF;
+                var _v1 = config.dP;
                 if (!_v1) {
                     return _Utils_Tuple2(
                         _List_fromArray(
                             [
                                 A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                                 A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                             ]),
@@ -11329,27 +11325,27 @@
                                 A2($elm$html$Html$Attributes$style, 'align-items', 'baseline')
                             ]),
                         'bottom');
                 }
             }();
             var alignmentAttrs = _v0.a;
             var direction = _v0.b;
-            var paddingStyle = ' .elm-charts__legends .elm-charts__legend {\n              margin-' + (direction + (':' + ($elm$core$String$fromFloat(config.fR) + ('px;\n            }\n\n            .elm-charts__legends .elm-charts__legend:last-child {\n              margin-' + (direction + ': 0px;\n            }\n        ')))));
+            var paddingStyle = ' .elm-charts__legends .elm-charts__legend {\n              margin-' + (direction + (':' + ($elm$core$String$fromFloat(config.f6) + ('px;\n            }\n\n            .elm-charts__legends .elm-charts__legend:last-child {\n              margin-' + (direction + ': 0px;\n            }\n        ')))));
             return A7(
                 $terezka$elm_charts$Internal$Svg$positionHtml,
                 plane,
                 x,
                 y,
                 config.g,
                 -config.h,
                 _Utils_ap(
                     anchorAttrs,
                     _Utils_ap(
                         alignmentAttrs,
-                        _Utils_ap(otherAttrs, config.bR))),
+                        _Utils_ap(otherAttrs, config.bY))),
                 A2(
                     $elm$core$List$cons,
                     A3(
                         $elm$html$Html$node,
                         'style',
                         _List_Nil,
                         _List_fromArray(
@@ -11364,84 +11360,84 @@
                 $terezka$elm_charts$Internal$Svg$legendsAt,
                 plane,
                 x,
                 y,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultLegends));
         });
     var $terezka$elm_charts$Internal$Svg$defaultInterpolation = {
-        bq: _List_Nil,
-        by: $terezka$elm_charts$Internal$Helpers$pink,
-        bB: _List_Nil,
-        cR: $elm$core$Maybe$Nothing,
-        fC: $elm$core$Maybe$Nothing,
+        bv: _List_Nil,
+        bD: $terezka$elm_charts$Internal$Helpers$pink,
+        bG: _List_Nil,
+        cX: $elm$core$Maybe$Nothing,
+        fU: $elm$core$Maybe$Nothing,
         P: 0,
-        eY: 1
+        ff: 1
     };
     var $terezka$elm_charts$Internal$Svg$defaultLineLegend = {
-        by: '#808BAB',
+        bD: '#808BAB',
         k: $elm$core$Maybe$Nothing,
-        d$: 16,
-        bR: _List_Nil,
-        fR: 10,
-        f_: '',
-        eY: 30,
+        eb: 16,
+        bY: _List_Nil,
+        f6: 10,
+        gf: '',
+        ff: 30,
         g: 0,
         h: 0
     };
     var $terezka$elm_charts$Internal$Svg$Point = F2(
         function(x, y) {
             return {
-                eZ: x,
-                e_: y
+                fg: x,
+                fh: y
             };
         });
     var $elm$svg$Svg$Attributes$fillRule = _VirtualDom_attribute('fill-rule');
     var $terezka$elm_charts$Internal$Interpolation$linear = $elm$core$List$map(
         $elm$core$List$map(
             function(_v0) {
-                var x = _v0.eZ;
-                var y = _v0.e_;
+                var x = _v0.fg;
+                var y = _v0.fh;
                 return A2($terezka$elm_charts$Internal$Commands$Line, x, y);
             }));
     var $terezka$elm_charts$Internal$Interpolation$First = {
         $: 0
     };
     var $terezka$elm_charts$Internal$Interpolation$Previous = function(a) {
         return {
             $: 1,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Interpolation$monotoneCurve = F4(
         function(point0, point1, tangent0, tangent1) {
-            var dx = (point1.eZ - point0.eZ) / 3;
-            return A6($terezka$elm_charts$Internal$Commands$CubicBeziers, point0.eZ + dx, point0.e_ + (dx * tangent0), point1.eZ - dx, point1.e_ - (dx * tangent1), point1.eZ, point1.e_);
+            var dx = (point1.fg - point0.fg) / 3;
+            return A6($terezka$elm_charts$Internal$Commands$CubicBeziers, point0.fg + dx, point0.fh + (dx * tangent0), point1.fg - dx, point1.fh - (dx * tangent1), point1.fg, point1.fh);
         });
     var $elm$core$Basics$neq = _Utils_notEqual;
     var $terezka$elm_charts$Internal$Interpolation$slope2 = F3(
         function(point0, point1, t) {
-            var h = point1.eZ - point0.eZ;
-            return (!(!h)) ? ((((3 * (point1.e_ - point0.e_)) / h) - t) / 2) : t;
+            var h = point1.fg - point0.fg;
+            return (!(!h)) ? ((((3 * (point1.fh - point0.fh)) / h) - t) / 2) : t;
         });
     var $elm$core$Basics$isNaN = _Basics_isNaN;
     var $terezka$elm_charts$Internal$Interpolation$sign = function(x) {
         return (x < 0) ? (-1) : 1;
     };
     var $terezka$elm_charts$Internal$Interpolation$toH = F2(
         function(h0, h1) {
             return (!h0) ? ((h1 < 0) ? (0 * (-1)) : h1) : h0;
         });
     var $terezka$elm_charts$Internal$Interpolation$slope3 = F3(
         function(point0, point1, point2) {
-            var h1 = point2.eZ - point1.eZ;
-            var h0 = point1.eZ - point0.eZ;
+            var h1 = point2.fg - point1.fg;
+            var h0 = point1.fg - point0.fg;
             var s0h = A2($terezka$elm_charts$Internal$Interpolation$toH, h0, h1);
-            var s0 = (point1.e_ - point0.e_) / s0h;
+            var s0 = (point1.fh - point0.fh) / s0h;
             var s1h = A2($terezka$elm_charts$Internal$Interpolation$toH, h1, h0);
-            var s1 = (point2.e_ - point1.e_) / s1h;
+            var s1 = (point2.fh - point1.fh) / s1h;
             var p = ((s0 * h1) + (s1 * h0)) / (h0 + h1);
             var slope = ($terezka$elm_charts$Internal$Interpolation$sign(s0) + $terezka$elm_charts$Internal$Interpolation$sign(s1)) * A2(
                 $elm$core$Basics$min,
                 A2(
                     $elm$core$Basics$min,
                     $elm$core$Basics$abs(s0),
                     $elm$core$Basics$abs(s1)),
@@ -11492,15 +11488,15 @@
                                 return _Utils_Tuple2(
                                     $terezka$elm_charts$Internal$Interpolation$Previous(t1),
                                     _Utils_ap(
                                         commands,
                                         _List_fromArray(
                                             [
                                                 A4($terezka$elm_charts$Internal$Interpolation$monotoneCurve, p0, p1, t1, t1),
-                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.eZ, p1.e_)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fg, p1.fh)
                                             ])));
                             }
                         } else {
                             break _v1$4;
                         }
                     } else {
                         if (_v1.b.b && _v1.b.b.b) {
@@ -11538,15 +11534,15 @@
                                 return _Utils_Tuple2(
                                     $terezka$elm_charts$Internal$Interpolation$Previous(t1),
                                     _Utils_ap(
                                         commands,
                                         _List_fromArray(
                                             [
                                                 A4($terezka$elm_charts$Internal$Interpolation$monotoneCurve, p0, p1, t0, t1),
-                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.eZ, p1.e_)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fg, p1.fh)
                                             ])));
                             }
                         } else {
                             break _v1$4;
                         }
                     }
                 }
@@ -11563,46 +11559,50 @@
                     return A2(
                         $terezka$elm_charts$Internal$Interpolation$monotonePart,
                         A2($elm$core$List$cons, p0, rest),
                         _Utils_Tuple2(
                             tangent,
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Line, p0.eZ, p0.e_)
+                                    A2($terezka$elm_charts$Internal$Commands$Line, p0.fg, p0.fh)
                                 ])));
                 } else {
                     return _Utils_Tuple2(tangent, _List_Nil);
                 }
             }();
             var t0 = _v1.a;
             var commands = _v1.b;
             return _Utils_Tuple2(
                 t0,
                 A2($elm$core$List$cons, commands, acc));
         });
+    var $elm$core$Tuple$second = function(_v0) {
+        var y = _v0.b;
+        return y;
+    };
     var $terezka$elm_charts$Internal$Interpolation$monotone = function(sections) {
         return A3(
             $elm$core$List$foldr,
             $terezka$elm_charts$Internal$Interpolation$monotoneSection,
             _Utils_Tuple2($terezka$elm_charts$Internal$Interpolation$First, _List_Nil),
             sections).b;
     };
     var $terezka$elm_charts$Internal$Interpolation$Point = F2(
         function(x, y) {
             return {
-                eZ: x,
-                e_: y
+                fg: x,
+                fh: y
             };
         });
     var $terezka$elm_charts$Internal$Interpolation$after = F2(
         function(a, b) {
             return _List_fromArray(
                 [
                     a,
-                    A2($terezka$elm_charts$Internal$Interpolation$Point, b.eZ, a.e_),
+                    A2($terezka$elm_charts$Internal$Interpolation$Point, b.fg, a.fh),
                     b
                 ]);
         });
     var $terezka$elm_charts$Internal$Interpolation$stepped = function(sections) {
         var expand = F2(
             function(result, section) {
                 expand: while (true) {
@@ -11631,16 +11631,16 @@
         return A2(
             $elm$core$List$map,
             A2(
                 $elm$core$Basics$composeR,
                 expand(_List_Nil),
                 $elm$core$List$map(
                     function(_v2) {
-                        var x = _v2.eZ;
-                        var y = _v2.e_;
+                        var x = _v2.fg;
+                        var y = _v2.fh;
                         return A2($terezka$elm_charts$Internal$Commands$Line, x, y);
                     })),
             sections);
     };
     var $elm$core$List$drop = F2(
         function(n, list) {
             drop: while (true) {
@@ -11707,25 +11707,25 @@
                             var rest = acc.b;
                             return A2(
                                 $elm$core$List$cons,
                                 _Utils_ap(
                                     latest,
                                     _List_fromArray(
                                         [{
-                                            eZ: toX(datum_),
-                                            e_: y_
+                                            fg: toX(datum_),
+                                            fh: y_
                                         }])),
                                 rest);
                         } else {
                             return A2(
                                 $elm$core$List$cons,
                                 _List_fromArray(
                                     [{
-                                        eZ: toX(datum_),
-                                        e_: y_
+                                        fg: toX(datum_),
+                                        fh: y_
                                     }]),
                                 acc);
                         }
                     } else {
                         return A2($elm$core$List$cons, _List_Nil, acc);
                     }
                 });
@@ -11745,30 +11745,30 @@
                 $elm$core$List$filterMap,
                 $elm$core$Basics$identity,
                 A3($elm$core$List$map2, toSets, points, commands));
         });
     var $terezka$elm_charts$Internal$Svg$area = F6(
         function(plane, toX, toY2M, toY, config, data) {
             var _v0 = function() {
-                var _v1 = config.cR;
+                var _v1 = config.cX;
                 if (_v1.$ === 1) {
                     return _Utils_Tuple2(
                         $elm$svg$Svg$text(''),
-                        config.by);
+                        config.bD);
                 } else {
                     var design = _v1.a;
-                    return A2($terezka$elm_charts$Internal$Svg$toPattern, config.by, design);
+                    return A2($terezka$elm_charts$Internal$Svg$toPattern, config.bD, design);
                 }
             }();
             var patternDefs = _v0.a;
             var fill = _v0.b;
             var view = function(cmds) {
                 return A4(
                     $terezka$elm_charts$Internal$Svg$withAttrs,
-                    config.bq,
+                    config.bv,
                     $elm$svg$Svg$path,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__area-section'),
                             $elm$svg$Svg$Attributes$fill(fill),
                             $elm$svg$Svg$Attributes$fillOpacity(
                                 $elm$core$String$fromFloat(config.P)),
@@ -11788,53 +11788,53 @@
                     var firstTop = _v6.a;
                     var cmdsTop = _v6.b;
                     var endTop = _v6.c;
                     return view(
                         _Utils_ap(
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.eZ, firstBottom.e_),
-                                    A2($terezka$elm_charts$Internal$Commands$Line, firstTop.eZ, firstTop.e_)
+                                    A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fg, firstBottom.fh),
+                                    A2($terezka$elm_charts$Internal$Commands$Line, firstTop.fg, firstTop.fh)
                                 ]),
                             _Utils_ap(
                                 cmdsTop,
                                 _Utils_ap(
                                     _List_fromArray(
                                         [
-                                            A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.eZ, firstBottom.e_)
+                                            A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fg, firstBottom.fh)
                                         ]),
                                     _Utils_ap(
                                         cmdsBottom,
                                         _List_fromArray(
                                             [
-                                                A2($terezka$elm_charts$Internal$Commands$Line, endTop.eZ, endTop.e_)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, endTop.fg, endTop.fh)
                                             ]))))));
                 });
             var withoutUnder = function(_v4) {
                 var first = _v4.a;
                 var cmds = _v4.b;
                 var end = _v4.c;
                 return view(
                     _Utils_ap(
                         _List_fromArray(
                             [
-                                A2($terezka$elm_charts$Internal$Commands$Move, first.eZ, 0),
-                                A2($terezka$elm_charts$Internal$Commands$Line, first.eZ, first.e_)
+                                A2($terezka$elm_charts$Internal$Commands$Move, first.fg, 0),
+                                A2($terezka$elm_charts$Internal$Commands$Line, first.fg, first.fh)
                             ]),
                         _Utils_ap(
                             cmds,
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Line, end.eZ, 0)
+                                    A2($terezka$elm_charts$Internal$Commands$Line, end.fg, 0)
                                 ]))));
             };
             if (config.P <= 0) {
                 return $elm$svg$Svg$text('');
             } else {
-                var _v2 = config.fC;
+                var _v2 = config.fU;
                 if (_v2.$ === 1) {
                     return $elm$svg$Svg$text('');
                 } else {
                     var method = _v2.a;
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
@@ -11868,41 +11868,41 @@
     var $terezka$elm_charts$Internal$Svg$interpolation = F5(
         function(plane, toX, toY, config, data) {
             var view = function(_v1) {
                 var first = _v1.a;
                 var cmds = _v1.b;
                 return A4(
                     $terezka$elm_charts$Internal$Svg$withAttrs,
-                    config.bq,
+                    config.bv,
                     $elm$svg$Svg$path,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__interpolation-section'),
                             $elm$svg$Svg$Attributes$fill('transparent'),
-                            $elm$svg$Svg$Attributes$stroke(config.by),
+                            $elm$svg$Svg$Attributes$stroke(config.bD),
                             $elm$svg$Svg$Attributes$strokeDasharray(
                                 A2(
                                     $elm$core$String$join,
                                     ' ',
-                                    A2($elm$core$List$map, $elm$core$String$fromFloat, config.bB))),
+                                    A2($elm$core$List$map, $elm$core$String$fromFloat, config.bG))),
                             $elm$svg$Svg$Attributes$strokeWidth(
-                                $elm$core$String$fromFloat(config.eY)),
+                                $elm$core$String$fromFloat(config.ff)),
                             $elm$svg$Svg$Attributes$d(
                                 A2(
                                     $terezka$elm_charts$Internal$Commands$description,
                                     plane,
                                     A2(
                                         $elm$core$List$cons,
-                                        A2($terezka$elm_charts$Internal$Commands$Move, first.eZ, first.e_),
+                                        A2($terezka$elm_charts$Internal$Commands$Move, first.fg, first.fh),
                                         cmds))),
                             $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                         ]),
                     _List_Nil);
             };
-            var _v0 = config.fC;
+            var _v0 = config.fU;
             if (_v0.$ === 1) {
                 return $elm$svg$Svg$text('');
             } else {
                 var method = _v0.a;
                 return A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
@@ -11934,18 +11934,18 @@
                 default:
                     return $elm$core$Basics$sqrt(area_ / 4);
             }
         });
     var $terezka$elm_charts$Internal$Svg$lineLegend = F3(
         function(config, interConfig, dotConfig) {
             var topMargin = function() {
-                var _v1 = dotConfig.aB;
+                var _v1 = dotConfig.aG;
                 if (!_v1.$) {
                     var shape = _v1.a;
-                    return A2($terezka$elm_charts$Internal$Svg$toRadius, dotConfig.eG, shape);
+                    return A2($terezka$elm_charts$Internal$Svg$toRadius, dotConfig.eZ, shape);
                 } else {
                     return 0;
                 }
             }();
             var fontStyle = function() {
                 var _v0 = config.k;
                 if (!_v0.$) {
@@ -11955,103 +11955,103 @@
                         'font-size',
                         $elm$core$String$fromInt(size_) + 'px');
                 } else {
                     return A2($elm$html$Html$Attributes$style, '', '');
                 }
             }();
             var fakePlane = {
-                eZ: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eY, 0, 0, 0, 10, 0, 10),
-                e_: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.d$, 0, 0, 0, 10, 0, 10)
+                fg: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ff, 0, 0, 0, 10, 0, 10),
+                fh: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eb, 0, 0, 0, 10, 0, 10)
             };
             var bottomMargin = (!interConfig.P) ? topMargin : 0;
             return A2(
                 $elm$html$Html$div,
                 _Utils_ap(
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('elm-charts__legend'),
                             A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                             A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                         ]),
-                    config.bR),
+                    config.bY),
                 _List_fromArray(
                     [
                         A5(
                             $terezka$elm_charts$Internal$Svg$container,
                             fakePlane,
                             _Utils_update(
                                 $terezka$elm_charts$Internal$Svg$defaultContainer, {
-                                    cq: false
+                                    cx: false
                                 }),
                             _List_Nil,
                             _List_fromArray(
                                 [
                                     A5(
                                         $terezka$elm_charts$Internal$Svg$interpolation,
                                         fakePlane,
                                         function($) {
-                                            return $.eZ;
+                                            return $.fg;
                                         },
                                         A2(
                                             $elm$core$Basics$composeR,
                                             function($) {
-                                                return $.e_;
+                                                return $.fh;
                                             },
                                             $elm$core$Maybe$Just),
                                         interConfig,
                                         _List_fromArray(
                                             [
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 0, 5),
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 10, 5)
                                             ])),
                                     A6(
                                         $terezka$elm_charts$Internal$Svg$area,
                                         fakePlane,
                                         function($) {
-                                            return $.eZ;
+                                            return $.fg;
                                         },
                                         $elm$core$Maybe$Nothing,
                                         A2(
                                             $elm$core$Basics$composeR,
                                             function($) {
-                                                return $.e_;
+                                                return $.fh;
                                             },
                                             $elm$core$Maybe$Just),
                                         interConfig,
                                         _List_fromArray(
                                             [
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 0, 5),
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 10, 5)
                                             ])),
                                     A5(
                                         $terezka$elm_charts$Internal$Svg$dot,
                                         fakePlane,
                                         function($) {
-                                            return $.eZ;
+                                            return $.fg;
                                         },
                                         function($) {
-                                            return $.e_;
+                                            return $.fh;
                                         },
                                         dotConfig,
                                         A2($terezka$elm_charts$Internal$Svg$Point, 5, 5))
                                 ]),
                             _List_Nil),
                         A2(
                             $elm$html$Html$div,
                             _List_fromArray(
                                 [
                                     fontStyle,
                                     A2(
                                         $elm$html$Html$Attributes$style,
                                         'margin-left',
-                                        $elm$core$String$fromFloat(config.fR) + 'px')
+                                        $elm$core$String$fromFloat(config.f6) + 'px')
                                 ]),
                             _List_fromArray(
                                 [
-                                    $elm$html$Html$text(config.f_)
+                                    $elm$html$Html$text(config.gf)
                                 ]))
                     ]));
         });
     var $terezka$elm_charts$Chart$Attributes$opacity = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
@@ -12061,19 +12061,19 @@
     var $terezka$elm_charts$Chart$Svg$lineLegend = F3(
         function(edits, interAttrsOrg, dotAttrsOrg) {
             var interpolationConfigOrg = A2($terezka$elm_charts$Internal$Helpers$apply, interAttrsOrg, $terezka$elm_charts$Internal$Svg$defaultInterpolation);
             var dotConfigOrg = A2($terezka$elm_charts$Internal$Helpers$apply, dotAttrsOrg, $terezka$elm_charts$Internal$Svg$defaultDot);
             var adjustWidth = function(config) {
                 return _Utils_update(
                     config, {
-                        eY: 10
+                        ff: 10
                     });
             };
             var _v0 = function() {
-                var _v1 = _Utils_Tuple2(interpolationConfigOrg.fC, dotConfigOrg.aB);
+                var _v1 = _Utils_Tuple2(interpolationConfigOrg.fU, dotConfigOrg.aG);
                 if (!_v1.a.$) {
                     if (_v1.b.$ === 1) {
                         var _v2 = _v1.b;
                         return _Utils_Tuple3(
                             dotAttrsOrg,
                             interAttrsOrg,
                             A2(
@@ -12121,15 +12121,15 @@
                 A2($terezka$elm_charts$Internal$Helpers$apply, interAttrs, $terezka$elm_charts$Internal$Svg$defaultInterpolation),
                 A2($terezka$elm_charts$Internal$Helpers$apply, dotAttrs, $terezka$elm_charts$Internal$Svg$defaultDot));
         });
     var $terezka$elm_charts$Chart$Attributes$title = F2(
         function(value, config) {
             return _Utils_update(
                 config, {
-                    f_: value
+                    gf: value
                 });
         });
     var $terezka$elm_charts$Chart$legendsAt = F4(
         function(toX, toY, attrs, children) {
             return $terezka$elm_charts$Chart$HtmlElement(
                 F2(
                     function(p, legends_) {
@@ -12157,40 +12157,25 @@
                                     interAttrs,
                                     dotAttrs);
                             }
                         };
                         return A5(
                             $terezka$elm_charts$Chart$Svg$legendsAt,
                             p,
-                            toX(p.eZ),
-                            toY(p.e_),
+                            toX(p.fg),
+                            toY(p.fh),
                             attrs,
                             A2($elm$core$List$map, viewLegend, legends_));
                     }));
         });
-    var $rundis$elm_bootstrap$Bootstrap$General$Internal$LG = 3;
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColWidth = function(a) {
-        return {
-            $: 0,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$width = F2(
-        function(size, count) {
-            return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColWidth(
-                A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, size, count));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$lg = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$width, 3, 0);
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col3 = 3;
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3 = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$width, 3, 3);
     var $terezka$elm_charts$Internal$Svg$Monotone = 1;
     var $terezka$elm_charts$Chart$Attributes$monotone = function(config) {
         return _Utils_update(
             config, {
-                fC: $elm$core$Maybe$Just(1)
+                fU: $elm$core$Maybe$Just(1)
             });
     };
     var $terezka$elm_charts$Chart$Attributes$moveDown = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
                     h: config.h + v
@@ -12205,25 +12190,25 @@
     var $terezka$elm_charts$Internal$Property$meta = F2(
         function(value, prop) {
             if (!prop.$) {
                 var con = prop.a;
                 return $terezka$elm_charts$Internal$Property$Property(
                     _Utils_update(
                         con, {
-                            ef: $elm$core$Maybe$Just(value)
+                            es: $elm$core$Maybe$Just(value)
                         }));
             } else {
                 var cons = prop.a;
                 return $terezka$elm_charts$Internal$Property$Stacked(
                     A2(
                         $elm$core$List$map,
                         function(con) {
                             return _Utils_update(
                                 con, {
-                                    ef: $elm$core$Maybe$Just(value)
+                                    es: $elm$core$Maybe$Just(value)
                                 });
                         },
                         cons));
             }
         });
     var $terezka$elm_charts$Chart$named = function(name) {
         return $terezka$elm_charts$Internal$Property$meta(name);
@@ -12248,20 +12233,20 @@
         });
     var $terezka$elm_charts$Chart$Events$map = $terezka$elm_charts$Internal$Events$map;
     var $terezka$elm_charts$Internal$Events$Event = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Events$on = F3(
         function(name, decoder, config) {
             return _Utils_update(
                 config, {
-                    bH: A2(
+                    bM: A2(
                         $elm$core$List$cons, {
-                            ff: decoder,
-                            fF: name
+                            fy: decoder,
+                            fW: name
                         },
-                        config.bH)
+                        config.bM)
                 });
         });
     var $terezka$elm_charts$Chart$Events$on = $terezka$elm_charts$Internal$Events$on;
     var $terezka$elm_charts$Chart$Events$onMouseLeave = function(onMsg) {
         return A2(
             $terezka$elm_charts$Chart$Events$on,
             'mouseleave',
@@ -12273,108 +12258,25 @@
     var $terezka$elm_charts$Chart$Events$onMouseMove = F2(
         function(onMsg, decoder) {
             return A2(
                 $terezka$elm_charts$Chart$Events$on,
                 'mousemove',
                 A2($terezka$elm_charts$Chart$Events$map, onMsg, decoder));
         });
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$GroupItem = $elm$core$Basics$identity;
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier = F2(
-        function(modifier, options) {
-            switch (modifier.$) {
-                case 0:
-                    var size = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            eG: $elm$core$Maybe$Just(size)
-                        });
-                case 1:
-                    return _Utils_update(
-                        options, {
-                            cL: true
-                        });
-                default:
-                    var attrs_ = modifier.a;
-                    return _Utils_update(
-                        options, {
-                            bp: _Utils_ap(options.bp, attrs_)
-                        });
-            }
-        });
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions = {
-        bp: _List_Nil,
-        eG: $elm$core$Maybe$Nothing,
-        cL: false
-    };
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes = F2(
-        function(toggle, modifiers) {
-            var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions, modifiers);
-            return _Utils_ap(
-                _List_fromArray(
-                    [
-                        A2($elm$html$Html$Attributes$attribute, 'role', 'group'),
-                        $elm$html$Html$Attributes$classList(
-                            _List_fromArray(
-                                [
-                                    _Utils_Tuple2('btn-group', true),
-                                    _Utils_Tuple2('btn-group-toggle', toggle),
-                                    _Utils_Tuple2('btn-group-vertical', options.cL)
-                                ])),
-                        A2($elm$html$Html$Attributes$attribute, 'data-toggle', 'buttons')
-                    ]),
-                _Utils_ap(
-                    function() {
-                        var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.eG);
-                        if (!_v0.$) {
-                            var s = _v0.a;
-                            return _List_fromArray(
-                                [
-                                    $elm$html$Html$Attributes$class('btn-group-' + s)
-                                ]);
-                        } else {
-                            return _List_Nil;
-                        }
-                    }(),
-                    options.bp));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem = F2(
-        function(options, items) {
-            return A2(
-                $elm$html$Html$div,
-                A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes, true, options),
-                A2(
-                    $elm$core$List$map,
-                    function(_v0) {
-                        var elem = _v0;
-                        return elem;
-                    },
-                    items));
-        });
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$renderGroup = function(_v0) {
-        var elem = _v0;
-        return elem;
-    };
-    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroup = F2(
-        function(options, items) {
-            return $rundis$elm_bootstrap$Bootstrap$ButtonGroup$renderGroup(
-                A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem, options, items));
-        });
-    var $terezka$elm_charts$Internal$Helpers$red = '#F5325B';
-    var $terezka$elm_charts$Chart$Attributes$red = $terezka$elm_charts$Internal$Helpers$red;
     var $terezka$elm_charts$Chart$Attributes$rotate = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
                     o: config.o + v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$row = function(config) {
         return _Utils_update(
             config, {
-                dF: 0
+                dP: 0
             });
     };
     var $terezka$elm_charts$Chart$Indexed = function(a) {
         return {
             $: 0,
             a: a
         };
@@ -12387,100 +12289,100 @@
                 b: b,
                 c: c,
                 d: d
             };
         });
     var $terezka$elm_charts$Internal$Item$toHtml = function(_v0) {
         var item = _v0;
-        return item.f1(item.e9);
+        return item.gi(item.fs);
     };
     var $terezka$elm_charts$Internal$Item$toSvg = F2(
         function(plane, _v0) {
             var item = _v0;
             return A3(
-                item.f6,
+                item.gn,
                 plane,
-                item.e9,
-                A2(item.f5, plane, item.e9));
+                item.fs,
+                A2(item.gm, plane, item.fs));
         });
     var $terezka$elm_charts$Internal$Item$generalize = F2(
         function(toAny, _v0) {
             var item = _v0;
             return {
-                e9: {
-                    fJ: toAny(item.e9.fJ),
-                    f0: $elm$core$Basics$identity,
-                    cC: item.e9.cC,
-                    gb: item.e9.gb
+                fs: {
+                    f_: toAny(item.fs.f_),
+                    gh: $elm$core$Basics$identity,
+                    cI: item.fs.cI,
+                    gs: item.fs.gs
                 },
-                f1: function(c) {
+                gi: function(c) {
                     return $terezka$elm_charts$Internal$Item$toHtml(item);
                 },
-                f2: function(_v1) {
-                    return item.f2(item.e9);
+                gj: function(_v1) {
+                    return item.gj(item.fs);
                 },
-                f5: F2(
+                gm: F2(
                     function(plane, _v2) {
-                        return A2(item.f5, plane, item.e9);
+                        return A2(item.gm, plane, item.fs);
                     }),
-                f6: F3(
+                gn: F3(
                     function(plane, _v3, _v4) {
                         return A2($terezka$elm_charts$Internal$Item$toSvg, plane, item);
                     })
             };
         });
     var $terezka$elm_charts$Internal$Many$getMembers = function(_v0) {
         var group_ = _v0;
         return function(_v1) {
             var x = _v1.a;
             var xs = _v1.b;
             return A2($elm$core$List$cons, x, xs);
-        }(group_.e9.d9);
+        }(group_.fs.el);
     };
     var $terezka$elm_charts$Internal$Many$getGenerals = function(group_) {
         var generalize = function(_v0) {
             var item = _v0;
-            return A2($terezka$elm_charts$Internal$Item$generalize, item.e9.f0, item);
+            return A2($terezka$elm_charts$Internal$Item$generalize, item.fs.gh, item);
         };
         return A2(
             $elm$core$List$map,
             generalize,
             $terezka$elm_charts$Internal$Many$getMembers(group_));
     };
     var $terezka$elm_charts$Internal$Item$getLimits = function(_v0) {
         var item = _v0;
-        return item.f2(item.e9);
+        return item.gj(item.fs);
     };
     var $terezka$elm_charts$Internal$Item$map = F2(
         function(func, _v0) {
             var item = _v0;
             return {
-                e9: {
-                    fJ: item.e9.fJ,
-                    f0: item.e9.f0,
-                    cC: item.e9.cC,
-                    gb: {
-                        fe: func(item.e9.gb.fe),
-                        fx: item.e9.gb.fx,
-                        aF: item.e9.gb.aF,
-                        bb: item.e9.gb.bb,
-                        e_: item.e9.gb.e_
+                fs: {
+                    f_: item.fs.f_,
+                    gh: item.fs.gh,
+                    cI: item.fs.cI,
+                    gs: {
+                        fx: func(item.fs.gs.fx),
+                        fQ: item.fs.gs.fQ,
+                        aK: item.fs.gs.aK,
+                        bf: item.fs.gs.bf,
+                        fh: item.fs.gs.fh
                     }
                 },
-                f1: function(_v1) {
+                gi: function(_v1) {
                     return $terezka$elm_charts$Internal$Item$toHtml(item);
                 },
-                f2: function(_v2) {
-                    return item.f2(item.e9);
+                gj: function(_v2) {
+                    return item.gj(item.fs);
                 },
-                f5: F2(
+                gm: F2(
                     function(plane, _v3) {
-                        return A2(item.f5, plane, item.e9);
+                        return A2(item.gm, plane, item.fs);
                     }),
-                f6: F3(
+                gn: F3(
                     function(plane, _v4, _v5) {
                         return A2($terezka$elm_charts$Internal$Item$toSvg, plane, item);
                     })
             };
         });
     var $elm$virtual_dom$VirtualDom$map = _VirtualDom_map;
     var $elm$svg$Svg$map = $elm$virtual_dom$VirtualDom$map;
@@ -12504,14 +12406,15 @@
             };
         });
     var $terezka$elm_charts$Internal$Helpers$brown = '#871c1c';
     var $terezka$elm_charts$Internal$Helpers$green = '#71c614';
     var $terezka$elm_charts$Internal$Helpers$moss = '#92b42c';
     var $terezka$elm_charts$Internal$Helpers$orange = '#FF8400';
     var $terezka$elm_charts$Internal$Helpers$purple = '#7b4dff';
+    var $terezka$elm_charts$Internal$Helpers$red = '#F5325B';
     var $elm$core$Dict$fromList = function(assocs) {
         return A3(
             $elm$core$List$foldl,
             F2(
                 function(_v0, dict) {
                     var key = _v0.a;
                     var value = _v0.b;
@@ -12572,27 +12475,27 @@
                     var interAttr = _Utils_ap(
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(
                                     $terezka$elm_charts$Internal$Helpers$toDefaultColor(colorIndex)),
                                 $terezka$elm_charts$Chart$Attributes$opacity(defaultOpacity)
                             ]),
-                        prop.fv);
+                        prop.fO);
                     var interConfig = toInterConfig(interAttr);
                     var defaultName = 'Property #' + $elm$core$String$fromInt(colorIndex + 1);
                     var defaultAttrs = _List_fromArray(
                         [
-                            $terezka$elm_charts$Chart$Attributes$color(interConfig.by),
-                            $terezka$elm_charts$Chart$Attributes$border(interConfig.by),
-                            _Utils_eq(interConfig.fC, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
+                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bD),
+                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bD),
+                            _Utils_eq(interConfig.fU, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
                         ]);
-                    var dotAttrs = _Utils_ap(defaultAttrs, prop.bq);
+                    var dotAttrs = _Utils_ap(defaultAttrs, prop.bv);
                     return A3(
                         $terezka$elm_charts$Internal$Legend$LineLegend,
-                        A2($elm$core$Maybe$withDefault, defaultName, prop.ef),
+                        A2($elm$core$Maybe$withDefault, defaultName, prop.es),
                         interAttr,
                         dotAttrs);
                 });
             return A2(
                 $elm$core$List$indexedMap,
                 F2(
                     function(propIndex, f) {
@@ -12604,29 +12507,14 @@
                         return A2(
                             $elm$core$List$map,
                             toDotLegend(ps),
                             ps);
                     },
                     A2($elm$core$List$map, $terezka$elm_charts$Internal$Property$toConfigs, properties)));
         });
-    var $elm$core$Maybe$map2 = F3(
-        function(func, ma, mb) {
-            if (ma.$ === 1) {
-                return $elm$core$Maybe$Nothing;
-            } else {
-                var a = ma.a;
-                if (mb.$ === 1) {
-                    return $elm$core$Maybe$Nothing;
-                } else {
-                    var b = mb.a;
-                    return $elm$core$Maybe$Just(
-                        A2(func, a, b));
-                }
-            }
-        });
     var $elm$html$Html$table = _VirtualDom_node('table');
     var $terezka$elm_charts$Internal$Produce$toDefaultName = F2(
         function(index, name) {
             return A2(
                 $elm$core$Maybe$withDefault,
                 'Property #' + $elm$core$String$fromInt(index + 1),
                 name);
@@ -12674,120 +12562,120 @@
                 return A2($terezka$elm_charts$Internal$Helpers$apply, attrs, $terezka$elm_charts$Internal$Svg$defaultDot);
             };
             var toDotItem = F7(
                 function(lineIndex, stackIndex, colorIndex, prop, interConfig, dataIndex, datum_) {
                     var y_ = A2(
                         $elm$core$Maybe$withDefault,
                         0,
-                        prop.a4(datum_));
+                        prop.a8(datum_));
                     var x_ = toX(datum_);
                     var defaultAttrs = _List_fromArray(
                         [
-                            $terezka$elm_charts$Chart$Attributes$color(interConfig.by),
-                            $terezka$elm_charts$Chart$Attributes$border(interConfig.by),
-                            _Utils_eq(interConfig.fC, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
+                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bD),
+                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bD),
+                            _Utils_eq(interConfig.fU, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
                         ]);
                     var dotAttrs = _Utils_ap(
                         defaultAttrs,
                         _Utils_ap(
-                            prop.bq,
-                            A5(prop.dV, lineIndex, stackIndex, dataIndex, prop.ef, datum_)));
+                            prop.bv,
+                            A5(prop.d5, lineIndex, stackIndex, dataIndex, prop.es, datum_)));
                     var config = toDotConfig(dotAttrs);
                     return {
-                        e9: {
-                            fJ: config,
-                            f0: $terezka$elm_charts$Internal$Item$Dot,
-                            cC: {
+                        fs: {
+                            f_: config,
+                            gh: $terezka$elm_charts$Internal$Item$Dot,
+                            cI: {
                                 v: config.v,
                                 x: config.x,
-                                by: function() {
-                                    var _v6 = config.by;
+                                bD: function() {
+                                    var _v6 = config.bD;
                                     if (_v6 === 'white') {
-                                        return interConfig.by;
+                                        return interConfig.bD;
                                     } else {
-                                        return config.by;
+                                        return config.bD;
                                     }
                                 }(),
-                                bC: dataIndex,
-                                fh: elIndex,
-                                dX: prop.F(datum_),
-                                ft: colorIndex,
-                                fF: prop.ef,
-                                fK: lineIndex,
-                                fS: stackIndex
+                                bH: dataIndex,
+                                fA: elIndex,
+                                d7: prop.F(datum_),
+                                fM: colorIndex,
+                                fW: prop.es,
+                                f$: lineIndex,
+                                f7: stackIndex
                             },
-                            gb: {
-                                fe: datum_,
-                                fx: function() {
-                                    var _v7 = prop.U(datum_);
+                            gs: {
+                                fx: datum_,
+                                fQ: function() {
+                                    var _v7 = prop.W(datum_);
                                     if (!_v7.$) {
                                         return true;
                                     } else {
                                         return false;
                                     }
                                 }(),
-                                aF: x_,
-                                bb: x_,
-                                e_: y_
+                                aK: x_,
+                                bf: x_,
+                                fh: y_
                             }
                         },
-                        f1: function(c) {
+                        gi: function(c) {
                             return _List_fromArray(
                                 [
                                     A3(
                                         $terezka$elm_charts$Internal$Produce$tooltipRow,
-                                        c.cC.by,
-                                        A2($terezka$elm_charts$Internal$Produce$toDefaultName, colorIndex, c.cC.fF),
+                                        c.cI.bD,
+                                        A2($terezka$elm_charts$Internal$Produce$toDefaultName, colorIndex, c.cI.fW),
                                         prop.F(datum_))
                                 ]);
                         },
-                        f2: function(_v8) {
+                        gj: function(_v8) {
                             return {
-                                aF: x_,
-                                bb: x_,
-                                gg: y_,
-                                dB: y_
+                                aK: x_,
+                                bf: x_,
+                                gx: y_,
+                                dL: y_
                             };
                         },
-                        f5: F2(
+                        gm: F2(
                             function(plane, _v9) {
                                 var radius = A2(
                                     $elm$core$Maybe$withDefault,
                                     0,
                                     A2(
                                         $elm$core$Maybe$map,
-                                        $terezka$elm_charts$Internal$Svg$toRadius(config.eG),
-                                        config.aB));
+                                        $terezka$elm_charts$Internal$Svg$toRadius(config.eZ),
+                                        config.aG));
                                 var radiusX_ = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, radius);
                                 var radiusY_ = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, radius);
                                 return {
-                                    aF: x_ - radiusX_,
-                                    bb: x_ + radiusX_,
-                                    gg: y_ - radiusY_,
-                                    dB: y_ + radiusY_
+                                    aK: x_ - radiusX_,
+                                    bf: x_ + radiusX_,
+                                    gx: y_ - radiusY_,
+                                    dL: y_ + radiusY_
                                 };
                             }),
-                        f6: F3(
+                        gn: F3(
                             function(plane, _v10, _v11) {
-                                var _v12 = prop.U(datum_);
+                                var _v12 = prop.W(datum_);
                                 if (_v12.$ === 1) {
                                     return $elm$svg$Svg$text('');
                                 } else {
                                     return A5(
                                         $terezka$elm_charts$Internal$Svg$dot,
                                         plane,
                                         function($) {
-                                            return $.eZ;
+                                            return $.fg;
                                         },
                                         function($) {
-                                            return $.e_;
+                                            return $.fh;
                                         },
                                         config, {
-                                            eZ: x_,
-                                            e_: y_
+                                            fg: x_,
+                                            fh: y_
                                         });
                                 }
                             })
                     };
                 });
             var toSeriesItem = F5(
                 function(lineIndex, stacks, stackIndex, prop, colorIndex) {
@@ -12795,30 +12683,30 @@
                     var interAttr = _Utils_ap(
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(
                                     $terezka$elm_charts$Internal$Helpers$toDefaultColor(colorIndex)),
                                 $terezka$elm_charts$Chart$Attributes$opacity(defaultOpacity)
                             ]),
-                        prop.fv);
+                        prop.fO);
                     var interConfig = toInterConfig(interAttr);
                     var dotItems = A2(
                         $elm$core$List$indexedMap,
                         A5(toDotItem, lineIndex, stackIndex, colorIndex, prop, interConfig),
                         data);
                     if (!dotItems.b) {
                         return $elm$core$Maybe$Nothing;
                     } else {
                         var first = dotItems.a;
                         var rest = dotItems.b;
                         return $elm$core$Maybe$Just({
-                            e9: {
-                                d9: _Utils_Tuple2(first, rest)
+                            fs: {
+                                el: _Utils_Tuple2(first, rest)
                             },
-                            f1: function(c) {
+                            gi: function(c) {
                                 return _List_fromArray(
                                     [
                                         A2(
                                             $elm$html$Html$table,
                                             _List_fromArray(
                                                 [
                                                     A2($elm$html$Html$Attributes$style, 'margin', '0')
@@ -12826,67 +12714,67 @@
                                             A2(
                                                 $elm$core$List$concatMap,
                                                 $terezka$elm_charts$Internal$Item$toHtml,
                                                 function(_v1) {
                                                     var x = _v1.a;
                                                     var xs = _v1.b;
                                                     return A2($elm$core$List$cons, x, xs);
-                                                }(c.d9)))
+                                                }(c.el)))
                                     ]);
                             },
-                            f2: function(c) {
+                            gj: function(c) {
                                 return A2(
                                     $terezka$elm_charts$Internal$Coordinates$foldPosition,
                                     $terezka$elm_charts$Internal$Item$getLimits,
                                     function(_v2) {
                                         var x = _v2.a;
                                         var xs = _v2.b;
                                         return A2($elm$core$List$cons, x, xs);
-                                    }(c.d9));
+                                    }(c.el));
                             },
-                            f5: F2(
+                            gm: F2(
                                 function(plane, c) {
                                     return A2(
                                         $terezka$elm_charts$Internal$Coordinates$foldPosition,
                                         $terezka$elm_charts$Internal$Item$getPosition(plane),
                                         function(_v3) {
                                             var x = _v3.a;
                                             var xs = _v3.b;
                                             return A2($elm$core$List$cons, x, xs);
-                                        }(c.d9));
+                                        }(c.el));
                                 }),
-                            f6: F3(
+                            gn: F3(
                                 function(plane, _v4, _v5) {
                                     var toBottom = function(datum_) {
                                         return A3(
                                             $elm$core$Maybe$map2,
                                             F2(
                                                 function(real, visual) {
                                                     return visual - real;
                                                 }),
-                                            prop.U(datum_),
-                                            prop.a4(datum_));
+                                            prop.W(datum_),
+                                            prop.a8(datum_));
                                     };
                                     return A2(
                                         $elm$svg$Svg$g,
                                         _List_fromArray(
                                             [
                                                 $elm$svg$Svg$Attributes$class('elm-charts__series')
                                             ]),
                                         _List_fromArray(
                                             [
                                                 A6(
                                                     $terezka$elm_charts$Internal$Svg$area,
                                                     plane,
                                                     toX,
                                                     $elm$core$Maybe$Just(toBottom),
-                                                    prop.a4,
+                                                    prop.a8,
                                                     interConfig,
                                                     data),
-                                                A5($terezka$elm_charts$Internal$Svg$interpolation, plane, toX, prop.a4, interConfig, data),
+                                                A5($terezka$elm_charts$Internal$Svg$interpolation, plane, toX, prop.a8, interConfig, data),
                                                 A2(
                                                     $elm$svg$Svg$g,
                                                     _List_fromArray(
                                                         [
                                                             $elm$svg$Svg$Attributes$class('elm-charts__dots')
                                                         ]),
                                                     A2(
@@ -12959,118 +12847,118 @@
         function(toX, properties, data) {
             return A4($terezka$elm_charts$Chart$seriesMap, $elm$core$Basics$identity, toX, properties, data);
         });
     var $terezka$elm_charts$Chart$Attributes$spacing = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    fR: v
+                    f6: v
                 });
         });
     var $terezka$elm_charts$Chart$html = function(func) {
         return $terezka$elm_charts$Chart$HtmlElement(
             F2(
                 function(p, _v0) {
                     return func(p);
                 }));
     };
     var $terezka$elm_charts$Internal$Svg$defaultTooltip = {
-        ar: true,
-        e4: 'white',
+        aw: true,
+        fn: 'white',
         v: '#D8D8D8',
-        Y: $elm$core$Maybe$Nothing,
-        fk: $elm$core$Maybe$Nothing,
-        d$: 0,
+        _: $elm$core$Maybe$Nothing,
+        fD: $elm$core$Maybe$Nothing,
+        eb: 0,
         b: 8,
-        eY: 0
+        ff: 0
     };
     var $terezka$elm_charts$Internal$Svg$Bottom = 3;
     var $terezka$elm_charts$Internal$Svg$Left = 1;
     var $terezka$elm_charts$Internal$Svg$Right = 2;
     var $terezka$elm_charts$Internal$Svg$Top = 0;
     var $elm$core$List$all = F2(
         function(isOkay, list) {
             return !A2(
                 $elm$core$List$any,
                 A2($elm$core$Basics$composeL, $elm$core$Basics$not, isOkay),
                 list);
         });
     var $terezka$elm_charts$Internal$Coordinates$bottom = function(pos) {
         return {
-            eZ: pos.aF + ((pos.bb - pos.aF) / 2),
-            e_: pos.gg
+            fg: pos.aK + ((pos.bf - pos.aK) / 2),
+            fh: pos.gx
         };
     };
     var $terezka$elm_charts$Internal$Coordinates$left = function(pos) {
         return {
-            eZ: pos.aF,
-            e_: pos.gg + ((pos.dB - pos.gg) / 2)
+            fg: pos.aK,
+            fh: pos.gx + ((pos.dL - pos.gx) / 2)
         };
     };
     var $elm$html$Html$map = $elm$virtual_dom$VirtualDom$map;
     var $terezka$elm_charts$Internal$Coordinates$right = function(pos) {
         return {
-            eZ: pos.bb,
-            e_: pos.gg + ((pos.dB - pos.gg) / 2)
+            fg: pos.bf,
+            fh: pos.gx + ((pos.dL - pos.gx) / 2)
         };
     };
     var $terezka$elm_charts$Internal$Svg$tooltipPointerStyle = F4(
         function(direction, className, background, borderColor) {
             var config = function() {
                 switch (direction) {
                     case 0:
                         return {
-                            ad: 'right', K: 'top', S: 'left'
+                            af: 'right', K: 'top', S: 'left'
                         };
                     case 3:
                         return {
-                            ad: 'right', K: 'bottom', S: 'left'
+                            af: 'right', K: 'bottom', S: 'left'
                         };
                     case 1:
                         return {
-                            ad: 'bottom', K: 'left', S: 'top'
+                            af: 'bottom', K: 'left', S: 'top'
                         };
                     case 2:
                         return {
-                            ad: 'bottom', K: 'right', S: 'top'
+                            af: 'bottom', K: 'right', S: 'top'
                         };
                     case 4:
                         return {
-                            ad: 'bottom', K: 'left', S: 'top'
+                            af: 'bottom', K: 'left', S: 'top'
                         };
                     default:
                         return {
-                            ad: 'right', K: 'top', S: 'left'
+                            af: 'right', K: 'top', S: 'left'
                         };
                 }
             }();
-            return '\n  .' + (className + (':before, .' + (className + (':after {\n    content: "";\n    position: absolute;\n    border-' + (config.S + (': 5px solid transparent;\n    border-' + (config.ad + (': 5px solid transparent;\n    ' + (config.K + (': 100%;\n    ' + (config.S + (': 50%;\n    margin-' + (config.S + (': -5px;\n  }\n\n  .' + (className + (':after {\n    border-' + (config.K + (': 5px solid ' + (background + (';\n    margin-' + (config.K + (': -1px;\n    z-index: 1;\n    height: 0px;\n  }\n\n  .' + (className + (':before {\n    border-' + (config.K + (': 5px solid ' + (borderColor + ';\n    height: 0px;\n  }\n  ')))))))))))))))))))))))))));
+            return '\n  .' + (className + (':before, .' + (className + (':after {\n    content: "";\n    position: absolute;\n    border-' + (config.S + (': 5px solid transparent;\n    border-' + (config.af + (': 5px solid transparent;\n    ' + (config.K + (': 100%;\n    ' + (config.S + (': 50%;\n    margin-' + (config.S + (': -5px;\n  }\n\n  .' + (className + (':after {\n    border-' + (config.K + (': 5px solid ' + (background + (';\n    margin-' + (config.K + (': -1px;\n    z-index: 1;\n    height: 0px;\n  }\n\n  .' + (className + (':before {\n    border-' + (config.K + (': 5px solid ' + (borderColor + ';\n    height: 0px;\n  }\n  ')))))))))))))))))))))))))));
         });
     var $terezka$elm_charts$Internal$Coordinates$top = function(pos) {
         return {
-            eZ: pos.aF + ((pos.bb - pos.aF) / 2),
-            e_: pos.dB
+            fg: pos.aK + ((pos.bf - pos.aK) / 2),
+            fh: pos.dL
         };
     };
     var $terezka$elm_charts$Internal$Svg$tooltip = F5(
         function(plane, pos, config, htmlAttrs, content) {
-            var distanceTop = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.dB);
-            var distanceRight = plane.eZ.N - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.aF);
-            var distanceLeft = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.bb);
-            var distanceBottom = plane.e_.N - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.gg);
+            var distanceTop = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.dL);
+            var distanceRight = plane.fg.N - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.aK);
+            var distanceLeft = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.bf);
+            var distanceBottom = plane.fh.N - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.gx);
             var direction = function() {
-                var _v5 = config.Y;
+                var _v5 = config._;
                 if (!_v5.$) {
                     switch (_v5.a) {
                         case 4:
                             var _v6 = _v5.a;
-                            return (config.eY > 0) ? ((_Utils_cmp(distanceLeft, config.eY + config.b) > 0) ? 1 : 2) : ((_Utils_cmp(distanceLeft, distanceRight) > 0) ? 1 : 2);
+                            return (config.ff > 0) ? ((_Utils_cmp(distanceLeft, config.ff + config.b) > 0) ? 1 : 2) : ((_Utils_cmp(distanceLeft, distanceRight) > 0) ? 1 : 2);
                         case 5:
                             var _v7 = _v5.a;
-                            return (config.d$ > 0) ? ((_Utils_cmp(distanceTop, config.d$ + config.b) > 0) ? 0 : 3) : ((_Utils_cmp(distanceTop, distanceBottom) > 0) ? 0 : 3);
+                            return (config.eb > 0) ? ((_Utils_cmp(distanceTop, config.eb + config.b) > 0) ? 0 : 3) : ((_Utils_cmp(distanceTop, distanceBottom) > 0) ? 0 : 3);
                         default:
                             var dir = _v5.a;
                             return dir;
                     }
                 } else {
                     var isLargest = function(a) {
                         return $elm$core$List$all(
@@ -13090,15 +12978,15 @@
                         isLargest,
                         distanceLeft,
                         _List_fromArray(
                             [distanceTop, distanceBottom, distanceRight])) ? 1 : 2));
                 }
             }();
             var focalPoint = function() {
-                var _v2 = config.fk;
+                var _v2 = config.fD;
                 if (!_v2.$) {
                     var focal = _v2.a;
                     switch (direction) {
                         case 0:
                             return $terezka$elm_charts$Internal$Coordinates$top(
                                 focal(pos));
                         case 3:
@@ -13130,75 +13018,75 @@
                         case 4:
                             return $terezka$elm_charts$Internal$Coordinates$left(pos);
                         default:
                             return $terezka$elm_charts$Internal$Coordinates$right(pos);
                     }
                 }
             }();
-            var arrowWidth = config.ar ? 4 : 0;
+            var arrowWidth = config.aw ? 4 : 0;
             var _v0 = function() {
                 switch (direction) {
                     case 0:
                         return {
-                            ae: 'elm-charts__tooltip-top', am: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
+                            ag: 'elm-charts__tooltip-top', ar: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
                         };
                     case 3:
                         return {
-                            ae: 'elm-charts__tooltip-bottom', am: 'translate(-50%, 0%)', g: 0, h: (-config.b) - arrowWidth
+                            ag: 'elm-charts__tooltip-bottom', ar: 'translate(-50%, 0%)', g: 0, h: (-config.b) - arrowWidth
                         };
                     case 1:
                         return {
-                            ae: 'elm-charts__tooltip-left', am: 'translate(-100%, -50%)', g: (-config.b) - arrowWidth, h: 0
+                            ag: 'elm-charts__tooltip-left', ar: 'translate(-100%, -50%)', g: (-config.b) - arrowWidth, h: 0
                         };
                     case 2:
                         return {
-                            ae: 'elm-charts__tooltip-right', am: 'translate(0, -50%)', g: config.b + arrowWidth, h: 0
+                            ag: 'elm-charts__tooltip-right', ar: 'translate(0, -50%)', g: config.b + arrowWidth, h: 0
                         };
                     case 4:
                         return {
-                            ae: 'elm-charts__tooltip-leftOrRight', am: 'translate(0, -50%)', g: (-config.b) - arrowWidth, h: 0
+                            ag: 'elm-charts__tooltip-leftOrRight', ar: 'translate(0, -50%)', g: (-config.b) - arrowWidth, h: 0
                         };
                     default:
                         return {
-                            ae: 'elm-charts__tooltip-topOrBottom', am: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
+                            ag: 'elm-charts__tooltip-topOrBottom', ar: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
                         };
                 }
             }();
             var xOff = _v0.g;
             var yOff = _v0.h;
-            var transformation = _v0.am;
-            var className = _v0.ae;
-            var children = config.ar ? A2(
+            var transformation = _v0.ar;
+            var className = _v0.ag;
+            var children = config.aw ? A2(
                 $elm$core$List$cons,
                 A3(
                     $elm$html$Html$node,
                     'style',
                     _List_Nil,
                     _List_fromArray(
                         [
                             $elm$html$Html$text(
-                                A4($terezka$elm_charts$Internal$Svg$tooltipPointerStyle, direction, className, config.e4, config.v))
+                                A4($terezka$elm_charts$Internal$Svg$tooltipPointerStyle, direction, className, config.fn, config.v))
                         ])),
                 content) : content;
             var attributes = _Utils_ap(
                 _List_fromArray(
                     [
                         $elm$html$Html$Attributes$class(className),
                         A2($elm$html$Html$Attributes$style, 'transform', transformation),
                         A2($elm$html$Html$Attributes$style, 'padding', '5px 8px'),
-                        A2($elm$html$Html$Attributes$style, 'background', config.e4),
+                        A2($elm$html$Html$Attributes$style, 'background', config.fn),
                         A2($elm$html$Html$Attributes$style, 'border', '1px solid ' + config.v),
                         A2($elm$html$Html$Attributes$style, 'border-radius', '3px'),
                         A2($elm$html$Html$Attributes$style, 'pointer-events', 'none')
                     ]),
                 htmlAttrs);
             return A2(
                 $elm$html$Html$map,
                 $elm$core$Basics$never,
-                A7($terezka$elm_charts$Internal$Svg$positionHtml, plane, focalPoint.eZ, focalPoint.e_, xOff, yOff, attributes, children));
+                A7($terezka$elm_charts$Internal$Svg$positionHtml, plane, focalPoint.fg, focalPoint.fh, xOff, yOff, attributes, children));
         });
     var $terezka$elm_charts$Chart$Svg$tooltip = F3(
         function(plane, pos, edits) {
             return A3(
                 $terezka$elm_charts$Internal$Svg$tooltip,
                 plane,
                 pos,
@@ -13206,112 +13094,23 @@
         });
     var $terezka$elm_charts$Chart$tooltip = F4(
         function(i, edits, attrs_, content) {
             return $terezka$elm_charts$Chart$html(
                 function(p) {
                     var pos = $terezka$elm_charts$Internal$Item$getLimits(i);
                     var content_ = _Utils_eq(content, _List_Nil) ? $terezka$elm_charts$Internal$Item$toHtml(i) : content;
-                    return A3($terezka$elm_charts$Internal$Svg$isWithinPlane, p, pos.aF, pos.dB) ? A5(
+                    return A3($terezka$elm_charts$Internal$Svg$isWithinPlane, p, pos.aK, pos.dL) ? A5(
                         $terezka$elm_charts$Chart$Svg$tooltip,
                         p,
                         A2($terezka$elm_charts$Internal$Item$getPosition, p, i),
                         edits,
                         attrs_,
                         content_) : $elm$html$Html$text('');
                 });
         });
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$Center = 1;
-    var $rundis$elm_bootstrap$Bootstrap$Text$alignMd = function(dir) {
-        return {
-            dP: dir,
-            eG: 2
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter = $rundis$elm_bootstrap$Bootstrap$Text$alignMd(1);
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$TextAlign = function(a) {
-        return {
-            $: 7,
-            a: a
-        };
-    };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign = function(align) {
-        return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$TextAlign(align);
-    };
-    var $author$project$Main$viewBigNumber = F2(
-        function(value, numberType) {
-            return A2(
-                $rundis$elm_bootstrap$Bootstrap$Grid$container,
-                _List_fromArray(
-                    [
-                        A2($elm$html$Html$Attributes$style, 'background-clip', 'border-box'),
-                        A2($elm$html$Html$Attributes$style, 'border', '1px solid darkgray'),
-                        A2($elm$html$Html$Attributes$style, 'padding', '0'),
-                        A2($elm$html$Html$Attributes$style, 'border-radius', '.25rem')
-                    ]),
-                _List_fromArray(
-                    [
-                        A2(
-                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                            _List_Nil,
-                            _List_fromArray(
-                                [
-                                    A2(
-                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                        _List_fromArray(
-                                            [
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign($rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter)
-                                            ]),
-                                        _List_fromArray(
-                                            [
-                                                A2(
-                                                    $elm$html$Html$h1,
-                                                    _List_fromArray(
-                                                        [
-                                                            A2($elm$html$Html$Attributes$style, 'padding', '.5em'),
-                                                            A2($elm$html$Html$Attributes$style, 'margin', '0'),
-                                                            A2($elm$html$Html$Attributes$style, 'color', 'white'),
-                                                            A2($elm$html$Html$Attributes$style, 'background-color', 'lightblue')
-                                                        ]),
-                                                    _List_fromArray(
-                                                        [
-                                                            $elm$html$Html$text(
-                                                                $elm$core$String$fromFloat(value))
-                                                        ]))
-                                            ]))
-                                ])),
-                        A2(
-                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                            _List_Nil,
-                            _List_fromArray(
-                                [
-                                    A2(
-                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                        _List_fromArray(
-                                            [
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign($rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter)
-                                            ]),
-                                        _List_fromArray(
-                                            [
-                                                A2(
-                                                    $elm$html$Html$h5,
-                                                    _List_fromArray(
-                                                        [
-                                                            A2($elm$html$Html$Attributes$style, 'padding', '.25em'),
-                                                            A2($elm$html$Html$Attributes$style, 'margin', '0'),
-                                                            A2($elm$html$Html$Attributes$style, 'color', 'darkblue'),
-                                                            A2($elm$html$Html$Attributes$style, 'background-color', 'lightgray')
-                                                        ]),
-                                                    _List_fromArray(
-                                                        [
-                                                            $elm$html$Html$text(numberType)
-                                                        ]))
-                                            ]))
-                                ]))
-                    ]));
-        });
     var $terezka$elm_charts$Chart$Attributes$withGrid = function(config) {
         return _Utils_update(
             config, {
                 f: true
             });
     };
     var $terezka$elm_charts$Internal$Svg$Floats = {
@@ -13324,18 +13123,18 @@
                 a: a,
                 b: b,
                 c: c
             };
         });
     var $terezka$elm_charts$Internal$Svg$defaultLabel = {
         i: $elm$core$Maybe$Nothing,
-        bq: _List_Nil,
+        bv: _List_Nil,
         v: 'white',
         x: 0,
-        by: '#808BAB',
+        bD: '#808BAB',
         j: $elm$core$Maybe$Nothing,
         k: $elm$core$Maybe$Nothing,
         l: false,
         o: 0,
         p: false,
         g: 0,
         h: 0
@@ -13372,15 +13171,14 @@
                     return (c !== '0') && (c !== '.');
                 },
                 $elm$core$String$toList(str));
             return _Utils_ap(
                 (signed && isNotZero) ? '-' : '',
                 str);
         });
-    var $elm$core$String$cons = _String_cons;
     var $elm$core$Char$fromCode = _Char_fromCode;
     var $myrho$elm_round$Round$increaseNum = function(_v0) {
         var head = _v0.a;
         var tail = _v0.b;
         if (head === '9') {
             var _v1 = $elm$core$String$uncons(tail);
             if (_v1.$ === 1) {
@@ -13397,31 +13195,14 @@
             return ((c >= 48) && (c < 57)) ? A2(
                 $elm$core$String$cons,
                 $elm$core$Char$fromCode(c + 1),
                 tail) : '0';
         }
     };
     var $elm$core$Basics$isInfinite = _Basics_isInfinite;
-    var $elm$core$String$fromChar = function(_char) {
-        return A2($elm$core$String$cons, _char, '');
-    };
-    var $elm$core$Bitwise$and = _Bitwise_and;
-    var $elm$core$Bitwise$shiftRightBy = _Bitwise_shiftRightBy;
-    var $elm$core$String$repeatHelp = F3(
-        function(n, chunk, result) {
-            return (n <= 0) ? result : A3(
-                $elm$core$String$repeatHelp,
-                n >> 1,
-                _Utils_ap(chunk, chunk),
-                (!(n & 1)) ? result : _Utils_ap(result, chunk));
-        });
-    var $elm$core$String$repeat = F2(
-        function(n, chunk) {
-            return A3($elm$core$String$repeatHelp, n, chunk, '');
-        });
     var $elm$core$String$padRight = F3(
         function(n, _char, string) {
             return _Utils_ap(
                 string,
                 A2(
                     $elm$core$String$repeat,
                     n - $elm$core$String$length(string),
@@ -13585,14 +13366,25 @@
             $elm$core$Basics$composeR,
             $myrho$elm_round$Round$round(prec),
             A2(
                 $elm$core$Basics$composeR,
                 $elm$core$String$toFloat,
                 $elm$core$Maybe$withDefault(0)));
     };
+    var $elm$core$List$filter = F2(
+        function(isGood, list) {
+            return A3(
+                $elm$core$List$foldr,
+                F2(
+                    function(x, xs) {
+                        return isGood(x) ? A2($elm$core$List$cons, x, xs) : xs;
+                    }),
+                _List_Nil,
+                list);
+        });
     var $terezka$intervals$Intervals$getMultiples = F3(
         function(magnitude, allowDecimals, hasTickAmount) {
             var defaults = hasTickAmount ? _List_fromArray(
                 [1, 1.2, 1.5, 2, 2.5, 3, 4, 5, 6, 8, 10]) : _List_fromArray(
                 [1, 2, 2.5, 5, 10]);
             return allowDecimals ? defaults : ((magnitude === 1) ? A2(
                 $elm$core$List$filter,
@@ -13701,15 +13493,15 @@
     var $terezka$intervals$Intervals$positions = F5(
         function(range, beginning, interval, m, acc) {
             positions: while (true) {
                 var nextPosition = A2(
                     $terezka$intervals$Intervals$correctFloat,
                     $terezka$intervals$Intervals$getPrecision(interval),
                     beginning + (m * interval));
-                if (_Utils_cmp(nextPosition, range.fB) > 0) {
+                if (_Utils_cmp(nextPosition, range.er) > 0) {
                     return acc;
                 } else {
                     var $temp$range = range,
                         $temp$beginning = beginning,
                         $temp$interval = interval,
                         $temp$m = m + 1,
                         $temp$acc = _Utils_ap(
@@ -13723,18 +13515,18 @@
                     acc = $temp$acc;
                     continue positions;
                 }
             }
         });
     var $terezka$intervals$Intervals$values = F4(
         function(allowDecimals, exact, amountRough, range) {
-            var intervalRough = (range.fB - range.fD) / amountRough;
+            var intervalRough = (range.er - range.et) / amountRough;
             var interval = A3($terezka$intervals$Intervals$getInterval, intervalRough, allowDecimals, exact);
             var intervalSafe = (!interval) ? 1 : interval;
-            var beginning = A2($terezka$intervals$Intervals$getBeginning, range.fD, intervalSafe);
+            var beginning = A2($terezka$intervals$Intervals$getBeginning, range.et, intervalSafe);
             var amountRoughSafe = (!amountRough) ? 1 : amountRough;
             return A5($terezka$intervals$Intervals$positions, range, beginning, intervalSafe, 0, _List_Nil);
         });
     var $terezka$intervals$Intervals$floats = function(amount) {
         if (!amount.$) {
             var number = amount.a;
             return A3($terezka$intervals$Intervals$values, true, true, number);
@@ -13744,28 +13536,28 @@
         }
     };
     var $terezka$elm_charts$Internal$Svg$floats = F2(
         function(i, b) {
             return A2(
                 $terezka$intervals$Intervals$floats,
                 $terezka$intervals$Intervals$around(i), {
-                    fB: b.fB,
-                    fD: b.fD
+                    er: b.er,
+                    et: b.et
                 });
         });
     var $terezka$elm_charts$Chart$Svg$floats = $terezka$elm_charts$Internal$Svg$floats;
     var $ryannhg$date_format$DateFormat$Language$Language = F6(
         function(toMonthName, toMonthAbbreviation, toWeekdayName, toWeekdayAbbreviation, toAmPm, toOrdinalSuffix) {
             return {
-                f$: toAmPm,
-                f3: toMonthAbbreviation,
-                f4: toMonthName,
-                aD: toOrdinalSuffix,
-                f7: toWeekdayAbbreviation,
-                f8: toWeekdayName
+                gg: toAmPm,
+                gk: toMonthAbbreviation,
+                gl: toMonthName,
+                aI: toOrdinalSuffix,
+                go: toWeekdayAbbreviation,
+                gp: toWeekdayName
             };
         });
     var $ryannhg$date_format$DateFormat$Language$toEnglishAmPm = function(hour) {
         return (hour > 11) ? 'pm' : 'am';
     };
     var $ryannhg$date_format$DateFormat$Language$toEnglishMonthName = function(month) {
         switch (month) {
@@ -13848,15 +13640,15 @@
             $elm$core$Basics$composeR,
             $ryannhg$date_format$DateFormat$Language$toEnglishWeekdayName,
             $elm$core$String$left(3)),
         $ryannhg$date_format$DateFormat$Language$toEnglishAmPm,
         $ryannhg$date_format$DateFormat$Language$toEnglishSuffix);
     var $ryannhg$date_format$DateFormat$amPm = F3(
         function(language, zone, posix) {
-            return language.f$(
+            return language.gg(
                 A2($elm$time$Time$toHour, zone, posix));
         });
     var $ryannhg$date_format$DateFormat$dayOfMonth = $elm$time$Time$toDay;
     var $elm$time$Time$Sun = 6;
     var $elm$time$Time$Fri = 4;
     var $elm$time$Time$Mon = 0;
     var $elm$time$Time$Sat = 5;
@@ -14187,92 +13979,92 @@
                 case 0:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 1:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aD(num));
+                            language.aI(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 2:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 3:
-                    return language.f3(
+                    return language.gk(
                         A2($elm$time$Time$toMonth, zone, posix));
                 case 4:
-                    return language.f4(
+                    return language.gl(
                         A2($elm$time$Time$toMonth, zone, posix));
                 case 17:
                     return $elm$core$String$fromInt(
                         1 + A2($ryannhg$date_format$DateFormat$quarter, zone, posix));
                 case 18:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aD(num));
+                            language.aI(num));
                     }(
                         1 + A2($ryannhg$date_format$DateFormat$quarter, zone, posix));
                 case 5:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$dayOfMonth, zone, posix));
                 case 6:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aD(num));
+                            language.aI(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfMonth, zone, posix));
                 case 7:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$dayOfMonth, zone, posix));
                 case 8:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$dayOfYear, zone, posix));
                 case 9:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aD(num));
+                            language.aI(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfYear, zone, posix));
                 case 10:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         3,
                         A2($ryannhg$date_format$DateFormat$dayOfYear, zone, posix));
                 case 11:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$dayOfWeek, zone, posix));
                 case 12:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aD(num));
+                            language.aI(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfWeek, zone, posix));
                 case 13:
-                    return language.f7(
+                    return language.go(
                         A2($elm$time$Time$toWeekday, zone, posix));
                 case 14:
-                    return language.f8(
+                    return language.gp(
                         A2($elm$time$Time$toWeekday, zone, posix));
                 case 19:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
                 case 20:
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
-                            language.aD(num));
+                            language.aI(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
                 case 21:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
@@ -14439,30 +14231,30 @@
     };
     var $ryannhg$date_format$DateFormat$yearNumber = $ryannhg$date_format$DateFormat$YearNumber;
     var $terezka$elm_charts$Internal$Svg$formatYear = $ryannhg$date_format$DateFormat$format(
         _List_fromArray(
             [$ryannhg$date_format$DateFormat$yearNumber]));
     var $terezka$elm_charts$Internal$Svg$formatTime = F2(
         function(zone, time) {
-            var _v0 = A2($elm$core$Maybe$withDefault, time.f9, time.e8);
+            var _v0 = A2($elm$core$Maybe$withDefault, time.gq, time.fr);
             switch (_v0) {
                 case 0:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClockMillis, zone, time.fZ);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClockMillis, zone, time.ge);
                 case 1:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClockSecond, zone, time.fZ);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClockSecond, zone, time.ge);
                 case 2:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.fZ);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.ge);
                 case 3:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.fZ);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.ge);
                 case 4:
-                    return (time.fE === 7) ? A2($terezka$elm_charts$Internal$Svg$formatWeekday, zone, time.fZ) : A2($terezka$elm_charts$Internal$Svg$formatDate, zone, time.fZ);
+                    return (time.fV === 7) ? A2($terezka$elm_charts$Internal$Svg$formatWeekday, zone, time.ge) : A2($terezka$elm_charts$Internal$Svg$formatDate, zone, time.ge);
                 case 5:
-                    return A2($terezka$elm_charts$Internal$Svg$formatMonth, zone, time.fZ);
+                    return A2($terezka$elm_charts$Internal$Svg$formatMonth, zone, time.ge);
                 default:
-                    return A2($terezka$elm_charts$Internal$Svg$formatYear, zone, time.fZ);
+                    return A2($terezka$elm_charts$Internal$Svg$formatYear, zone, time.ge);
             }
         });
     var $terezka$elm_charts$Chart$Svg$formatTime = $terezka$elm_charts$Internal$Svg$formatTime;
     var $terezka$elm_charts$Internal$Svg$generate = F3(
         function(amount, _v0, limits) {
             var func = _v0;
             return A2(func, amount, limits);
@@ -14484,16 +14276,16 @@
                 }());
         });
     var $terezka$elm_charts$Internal$Svg$ints = F2(
         function(i, b) {
             return A2(
                 $terezka$intervals$Intervals$ints,
                 $terezka$intervals$Intervals$around(i), {
-                    fB: b.fB,
-                    fD: b.fD
+                    er: b.er,
+                    et: b.et
                 });
         });
     var $terezka$elm_charts$Chart$Svg$ints = $terezka$elm_charts$Internal$Svg$ints;
     var $terezka$intervals$Intervals$Day = 4;
     var $terezka$intervals$Intervals$Hour = 3;
     var $terezka$intervals$Intervals$Millisecond = 0;
     var $terezka$intervals$Intervals$Minute = 2;
@@ -14645,17 +14437,17 @@
                         $temp$d = d - monthDays;
                     y = $temp$y;
                     m = $temp$m;
                     d = $temp$d;
                     continue toCalendarDateHelp;
                 } else {
                     return {
-                        dN: d,
-                        eh: m,
-                        e$: y
+                        dY: d,
+                        ev: m,
+                        fi: y
                     };
                 }
             }
         });
     var $justinmimbs$date$Date$divWithRemainder = F2(
         function(a, b) {
             return _Utils_Tuple2(
@@ -14679,38 +14471,38 @@
         var n = (!r1) ? 0 : 1;
         return ((((n400 * 400) + (n100 * 100)) + (n4 * 4)) + n1) + n;
     };
     var $justinmimbs$date$Date$toOrdinalDate = function(_v0) {
         var rd = _v0;
         var y = $justinmimbs$date$Date$year(rd);
         return {
-            dc: rd - $justinmimbs$date$Date$daysBeforeYear(y),
-            e$: y
+            dk: rd - $justinmimbs$date$Date$daysBeforeYear(y),
+            fi: y
         };
     };
     var $justinmimbs$date$Date$toCalendarDate = function(_v0) {
         var rd = _v0;
         var date = $justinmimbs$date$Date$toOrdinalDate(rd);
-        return A3($justinmimbs$date$Date$toCalendarDateHelp, date.e$, 0, date.dc);
+        return A3($justinmimbs$date$Date$toCalendarDateHelp, date.fi, 0, date.dk);
     };
     var $justinmimbs$date$Date$add = F3(
         function(unit, n, _v0) {
             var rd = _v0;
             switch (unit) {
                 case 0:
                     return A3($justinmimbs$date$Date$add, 1, 12 * n, rd);
                 case 1:
                     var date = $justinmimbs$date$Date$toCalendarDate(rd);
-                    var wholeMonths = ((12 * (date.e$ - 1)) + ($justinmimbs$date$Date$monthToNumber(date.eh) - 1)) + n;
+                    var wholeMonths = ((12 * (date.fi - 1)) + ($justinmimbs$date$Date$monthToNumber(date.ev) - 1)) + n;
                     var m = $justinmimbs$date$Date$numberToMonth(
                         A2($elm$core$Basics$modBy, 12, wholeMonths) + 1);
                     var y = A2($justinmimbs$date$Date$floorDiv, wholeMonths, 12) + 1;
                     return ($justinmimbs$date$Date$daysBeforeYear(y) + A2($justinmimbs$date$Date$daysBeforeMonth, y, m)) + A2(
                         $elm$core$Basics$min,
-                        date.dN,
+                        date.dY,
                         A2($justinmimbs$date$Date$daysInMonth, y, m));
                 case 2:
                     return rd + (7 * n);
                 default:
                     return rd + n;
             }
         });
@@ -14931,15 +14723,15 @@
     var $justinmimbs$date$Date$firstOfYear = function(y) {
         return $justinmimbs$date$Date$daysBeforeYear(y) + 1;
     };
     var $justinmimbs$date$Date$month = A2(
         $elm$core$Basics$composeR,
         $justinmimbs$date$Date$toCalendarDate,
         function($) {
-            return $.eh;
+            return $.ev;
         });
     var $justinmimbs$date$Date$monthToQuarter = function(m) {
         return (($justinmimbs$date$Date$monthToNumber(m) + 2) / 3) | 0;
     };
     var $justinmimbs$date$Date$quarter = A2($elm$core$Basics$composeR, $justinmimbs$date$Date$month, $justinmimbs$date$Date$monthToQuarter);
     var $justinmimbs$date$Date$quarterToMonth = function(q) {
         return $justinmimbs$date$Date$numberToMonth((q * 3) - 2);
@@ -15065,62 +14857,62 @@
     var $terezka$intervals$Intervals$Time$ceilingDay = F3(
         function(zone, mult, stamp) {
             return (mult === 7) ? A3($justinmimbs$time_extra$Time$Extra$ceiling, 3, zone, stamp) : A3($justinmimbs$time_extra$Time$Extra$ceiling, 11, zone, stamp);
         });
     var $justinmimbs$time_extra$Time$Extra$Hour = 12;
     var $justinmimbs$time_extra$Time$Extra$partsToPosix = F2(
         function(zone, _v0) {
-            var year = _v0.e$;
-            var month = _v0.eh;
-            var day = _v0.dN;
-            var hour = _v0.cW;
-            var minute = _v0.c7;
-            var second = _v0.dl;
-            var millisecond = _v0.c6;
+            var year = _v0.fi;
+            var month = _v0.ev;
+            var day = _v0.dY;
+            var hour = _v0.c2;
+            var minute = _v0.df;
+            var second = _v0.dv;
+            var millisecond = _v0.de;
             return A3(
                 $justinmimbs$time_extra$Time$Extra$posixFromDateTime,
                 zone,
                 A3($justinmimbs$date$Date$fromCalendarDate, year, month, day),
                 A4(
                     $justinmimbs$time_extra$Time$Extra$timeFromClock,
                     A3($elm$core$Basics$clamp, 0, 23, hour),
                     A3($elm$core$Basics$clamp, 0, 59, minute),
                     A3($elm$core$Basics$clamp, 0, 59, second),
                     A3($elm$core$Basics$clamp, 0, 999, millisecond)));
         });
     var $justinmimbs$time_extra$Time$Extra$posixToParts = F2(
         function(zone, posix) {
             return {
-                dN: A2($elm$time$Time$toDay, zone, posix),
-                cW: A2($elm$time$Time$toHour, zone, posix),
-                c6: A2($elm$time$Time$toMillis, zone, posix),
-                c7: A2($elm$time$Time$toMinute, zone, posix),
-                eh: A2($elm$time$Time$toMonth, zone, posix),
-                dl: A2($elm$time$Time$toSecond, zone, posix),
-                e$: A2($elm$time$Time$toYear, zone, posix)
+                dY: A2($elm$time$Time$toDay, zone, posix),
+                c2: A2($elm$time$Time$toHour, zone, posix),
+                de: A2($elm$time$Time$toMillis, zone, posix),
+                df: A2($elm$time$Time$toMinute, zone, posix),
+                ev: A2($elm$time$Time$toMonth, zone, posix),
+                dv: A2($elm$time$Time$toSecond, zone, posix),
+                fi: A2($elm$time$Time$toYear, zone, posix)
             };
         });
     var $terezka$intervals$Intervals$Time$ceilingHour = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 12, zone, stamp));
-            var rem = parts.cW % mult;
+            var rem = parts.c2 % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 12, mult - rem, zone, _new);
         });
     var $justinmimbs$time_extra$Time$Extra$Minute = 13;
     var $terezka$intervals$Intervals$Time$ceilingMinute = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 13, zone, stamp));
-            var rem = parts.c7 % mult;
+            var rem = parts.df % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 13, mult - rem, zone, _new);
         });
     var $terezka$intervals$Intervals$Time$intAsMonth = function(_int) {
         switch (_int) {
             case 1:
                 return 0;
@@ -15180,61 +14972,61 @@
     };
     var $terezka$intervals$Intervals$Time$ceilingMonth = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 2, zone, stamp));
-            var monthInt = $terezka$intervals$Intervals$Time$monthAsInt(parts.eh);
+            var monthInt = $terezka$intervals$Intervals$Time$monthAsInt(parts.ev);
             var rem = (monthInt - 1) % mult;
             var newMonth = (!rem) ? monthInt : ((monthInt - rem) + mult);
             return A2(
                 $justinmimbs$time_extra$Time$Extra$partsToPosix,
                 zone,
                 (newMonth > 12) ? _Utils_update(
                     parts, {
-                        eh: $terezka$intervals$Intervals$Time$intAsMonth(newMonth - 12),
-                        e$: parts.e$ + 1
+                        ev: $terezka$intervals$Intervals$Time$intAsMonth(newMonth - 12),
+                        fi: parts.fi + 1
                     }) : _Utils_update(
                     parts, {
-                        eh: $terezka$intervals$Intervals$Time$intAsMonth(newMonth)
+                        ev: $terezka$intervals$Intervals$Time$intAsMonth(newMonth)
                     }));
         });
     var $terezka$intervals$Intervals$Time$ceilingMs = F3(
         function(zone, mult, stamp) {
             var parts = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, stamp);
-            var rem = parts.c6 % mult;
+            var rem = parts.de % mult;
             return (!rem) ? A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts) : A4($justinmimbs$time_extra$Time$Extra$add, 15, mult - rem, zone, stamp);
         });
     var $justinmimbs$time_extra$Time$Extra$Second = 14;
     var $terezka$intervals$Intervals$Time$ceilingSecond = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 14, zone, stamp));
-            var rem = parts.dl % mult;
+            var rem = parts.dv % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 14, mult - rem, zone, _new);
         });
     var $justinmimbs$time_extra$Time$Extra$Year = 0;
     var $terezka$intervals$Intervals$Time$ceilingYear = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 0, zone, stamp));
-            var rem = parts.e$ % mult;
-            var newYear = (!rem) ? parts.e$ : ((parts.e$ - rem) + mult);
+            var rem = parts.fi % mult;
+            var newYear = (!rem) ? parts.fi : ((parts.fi - rem) + mult);
             return A2(
                 $justinmimbs$time_extra$Time$Extra$partsToPosix,
                 zone,
                 _Utils_update(
                     parts, {
-                        e$: newYear
+                        fi: newYear
                     }));
         });
     var $terezka$intervals$Intervals$Time$ceilingUnit = F3(
         function(zone, unit, mult) {
             switch (unit) {
                 case 0:
                     return A2($terezka$intervals$Intervals$Time$ceilingMs, zone, mult);
@@ -15259,15 +15051,15 @@
     var $terezka$intervals$Intervals$Time$Month = 5;
     var $terezka$intervals$Intervals$Time$Second = 1;
     var $terezka$intervals$Intervals$Time$Year = 6;
     var $terezka$intervals$Intervals$Time$getChange = F3(
         function(zone, a, b) {
             var bP = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b);
             var aP = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a);
-            return (!_Utils_eq(aP.e$, bP.e$)) ? 6 : ((!_Utils_eq(aP.eh, bP.eh)) ? 5 : ((!_Utils_eq(aP.dN, bP.dN)) ? 4 : ((!_Utils_eq(aP.cW, bP.cW)) ? 3 : ((!_Utils_eq(aP.c7, bP.c7)) ? 2 : ((!_Utils_eq(aP.dl, bP.dl)) ? 1 : 0)))));
+            return (!_Utils_eq(aP.fi, bP.fi)) ? 6 : ((!_Utils_eq(aP.ev, bP.ev)) ? 5 : ((!_Utils_eq(aP.dY, bP.dY)) ? 4 : ((!_Utils_eq(aP.c2, bP.c2)) ? 3 : ((!_Utils_eq(aP.df, bP.df)) ? 2 : ((!_Utils_eq(aP.dv, bP.dv)) ? 1 : 0)))));
         });
     var $danhandrea$elm_time_extra$Util$isLeapYear = function(year) {
         return (!A2($elm$core$Basics$modBy, 400, year)) || ((!(!A2($elm$core$Basics$modBy, 100, year))) && (!A2($elm$core$Basics$modBy, 4, year)));
     };
     var $danhandrea$elm_time_extra$Month$days = F2(
         function(year, month) {
             switch (month) {
@@ -15306,36 +15098,36 @@
                 $terezka$intervals$Intervals$Time$toMs(b)) < 0) ? _Utils_Tuple2(
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a),
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b)) : _Utils_Tuple2(
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b),
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a));
             var aP = _v0.a;
             var bP = _v0.b;
-            var dMsX = bP.c6 - aP.c6;
+            var dMsX = bP.de - aP.de;
             var dMs = (dMsX < 0) ? (1000 + dMsX) : dMsX;
-            var dSecondX = (bP.dl - aP.dl) + ((dMsX < 0) ? (-1) : 0);
-            var dMinuteX = (bP.c7 - aP.c7) + ((dSecondX < 0) ? (-1) : 0);
-            var dHourX = (bP.cW - aP.cW) + ((dMinuteX < 0) ? (-1) : 0);
-            var dDayX = (bP.dN - aP.dN) + ((dHourX < 0) ? (-1) : 0);
-            var dDay = (dDayX < 0) ? (A2($danhandrea$elm_time_extra$TimeExtra$daysInMonth, bP.e$, bP.eh) + dDayX) : dDayX;
-            var dMonthX = ($terezka$intervals$Intervals$Time$monthAsInt(bP.eh) - $terezka$intervals$Intervals$Time$monthAsInt(aP.eh)) + ((dDayX < 0) ? (-1) : 0);
+            var dSecondX = (bP.dv - aP.dv) + ((dMsX < 0) ? (-1) : 0);
+            var dMinuteX = (bP.df - aP.df) + ((dSecondX < 0) ? (-1) : 0);
+            var dHourX = (bP.c2 - aP.c2) + ((dMinuteX < 0) ? (-1) : 0);
+            var dDayX = (bP.dY - aP.dY) + ((dHourX < 0) ? (-1) : 0);
+            var dDay = (dDayX < 0) ? (A2($danhandrea$elm_time_extra$TimeExtra$daysInMonth, bP.fi, bP.ev) + dDayX) : dDayX;
+            var dMonthX = ($terezka$intervals$Intervals$Time$monthAsInt(bP.ev) - $terezka$intervals$Intervals$Time$monthAsInt(aP.ev)) + ((dDayX < 0) ? (-1) : 0);
             var dMonth = (dMonthX < 0) ? (12 + dMonthX) : dMonthX;
             var dHour = (dHourX < 0) ? (24 + dHourX) : dHourX;
             var dMinute = (dMinuteX < 0) ? (60 + dMinuteX) : dMinuteX;
             var dSecond = (dSecondX < 0) ? (60 + dSecondX) : dSecondX;
-            var dYearX = (bP.e$ - aP.e$) + ((dMonthX < 0) ? (-1) : 0);
-            var dYear = (dYearX < 0) ? ($terezka$intervals$Intervals$Time$monthAsInt(bP.eh) + dYearX) : dYearX;
+            var dYearX = (bP.fi - aP.fi) + ((dMonthX < 0) ? (-1) : 0);
+            var dYear = (dYearX < 0) ? ($terezka$intervals$Intervals$Time$monthAsInt(bP.ev) + dYearX) : dYearX;
             return {
-                dN: dDay,
-                cW: dHour,
-                c6: dMs,
-                c7: dMinute,
-                eh: dMonth,
-                dl: dSecond,
-                e$: dYear
+                dY: dDay,
+                c2: dHour,
+                de: dMs,
+                df: dMinute,
+                ev: dMonth,
+                dv: dSecond,
+                fi: dYear
             };
         });
     var $terezka$intervals$Intervals$Time$oneSecond = 1000;
     var $terezka$intervals$Intervals$Time$oneMinute = $terezka$intervals$Intervals$Time$oneSecond * 60;
     var $terezka$intervals$Intervals$Time$oneHour = $terezka$intervals$Intervals$Time$oneMinute * 60;
     var $terezka$intervals$Intervals$Time$oneDay = $terezka$intervals$Intervals$Time$oneHour * 24;
     var $terezka$intervals$Intervals$Time$oneMs = 1;
@@ -15377,20 +15169,20 @@
                 case 3:
                     return timeDiff($terezka$intervals$Intervals$Time$oneHour) + 1;
                 case 4:
                     return timeDiff($terezka$intervals$Intervals$Time$oneDay) + 1;
                 case 5:
                     return diff(
                         function(d) {
-                            return d.eh + (d.e$ * 12);
+                            return d.ev + (d.fi * 12);
                         }) + 1;
                 default:
                     return diff(
                         function($) {
-                            return $.e$;
+                            return $.fi;
                         }) + 1;
             }
         });
     var $terezka$intervals$Intervals$Time$largerUnit = function(unit) {
         switch (unit) {
             case 0:
                 return $elm$core$Maybe$Just(1);
@@ -15512,22 +15304,22 @@
             var mult = _v0.b;
             var amount = A5($terezka$intervals$Intervals$Time$getNumOfTicks, zone, unit, mult, min, max);
             var initial = A4($terezka$intervals$Intervals$Time$ceilingUnit, zone, unit, mult, min);
             var tUnit = $terezka$intervals$Intervals$Time$toExtraUnit(unit);
             var toTick = F3(
                 function(x, timestamp, change) {
                     return {
-                        e8: (_Utils_cmp(
+                        fr: (_Utils_cmp(
                             $terezka$intervals$Intervals$Time$unitToInt(change),
                             $terezka$intervals$Intervals$Time$unitToInt(unit)) > 0) ? $elm$core$Maybe$Just(change) : $elm$core$Maybe$Nothing,
-                        c4: !x,
-                        fE: mult,
-                        fZ: timestamp,
-                        f9: unit,
-                        dC: zone
+                        dc: !x,
+                        fV: mult,
+                        ge: timestamp,
+                        gq: unit,
+                        dM: zone
                     };
                 });
             var toTicks = F2(
                 function(xs, acc) {
                     toTicks: while (true) {
                         if (xs.b) {
                             var x = xs.a;
@@ -15572,66 +15364,66 @@
                         return 5;
                     default:
                         return 6;
                 }
             };
             var translateUnit = function(time) {
                 return {
-                    e8: A2($elm$core$Maybe$map, toUnit, time.e8),
-                    c4: time.c4,
-                    fE: time.fE,
-                    fZ: time.fZ,
-                    f9: toUnit(time.f9),
-                    dC: time.dC
+                    fr: A2($elm$core$Maybe$map, toUnit, time.fr),
+                    dc: time.dc,
+                    fV: time.fV,
+                    ge: time.ge,
+                    gq: toUnit(time.gq),
+                    dM: time.dM
                 };
             };
             var fromMs = function(ts) {
                 return $elm$time$Time$millisToPosix(
                     $elm$core$Basics$round(ts));
             };
             return A2(
                 $elm$core$List$map,
                 translateUnit,
                 A4(
                     $terezka$intervals$Intervals$Time$values,
                     zone,
                     amount,
-                    fromMs(range.fD),
-                    fromMs(range.fB)));
+                    fromMs(range.et),
+                    fromMs(range.er)));
         });
     var $terezka$elm_charts$Internal$Svg$times = function(zone) {
         return F2(
             function(i, b) {
                 return A3(
                     $terezka$intervals$Intervals$times,
                     zone,
                     i, {
-                        fB: b.fB,
-                        fD: b.fD
+                        er: b.er,
+                        et: b.et
                     });
             });
     };
     var $terezka$elm_charts$Chart$Svg$times = $terezka$elm_charts$Internal$Svg$times;
     var $terezka$elm_charts$Chart$generateValues = F4(
         function(amount, tick, maybeFormat, axis) {
             var toTickValues = F2(
                 function(toValue, toString) {
                     return $elm$core$List$map(
                         function(i) {
                             return {
-                                eb: function() {
+                                en: function() {
                                     if (!maybeFormat.$) {
                                         var formatter = maybeFormat.a;
                                         return formatter(
                                             toValue(i));
                                     } else {
                                         return toString(i);
                                     }
                                 }(),
-                                U: toValue(i)
+                                W: toValue(i)
                             };
                         });
                 });
             switch (tick.$) {
                 case 0:
                     return A3(
                         toTickValues,
@@ -15648,24 +15440,32 @@
                     var zone = tick.a;
                     return A3(
                         toTickValues,
                         A2(
                             $elm$core$Basics$composeL,
                             A2($elm$core$Basics$composeL, $elm$core$Basics$toFloat, $elm$time$Time$posixToMillis),
                             function($) {
-                                return $.fZ;
+                                return $.ge;
                             }),
                         $terezka$elm_charts$Chart$Svg$formatTime(zone),
                         A3(
                             $terezka$elm_charts$Chart$Svg$generate,
                             amount,
                             $terezka$elm_charts$Chart$Svg$times(zone),
                             axis));
             }
         });
+    var $elm$virtual_dom$VirtualDom$attribute = F2(
+        function(key, value) {
+            return A2(
+                _VirtualDom_attribute,
+                _VirtualDom_noOnOrFormAction(key),
+                _VirtualDom_noJavaScriptOrHtmlUri(value));
+        });
+    var $elm$html$Html$Attributes$attribute = $elm$virtual_dom$VirtualDom$attribute;
     var $elm$svg$Svg$foreignObject = $elm$svg$Svg$trustedNode('foreignObject');
     var $terezka$elm_charts$Internal$Svg$position = F6(
         function(plane, rotation, x_, y_, xOff_, yOff_) {
             return $elm$svg$Svg$Attributes$transform(
                 'translate(' + ($elm$core$String$fromFloat(
                     A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x_) + xOff_) + (',' + ($elm$core$String$fromFloat(
                     A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y_) + yOff_) + (') rotate(' + ($elm$core$String$fromFloat(rotation) + ')'))))));
@@ -15713,24 +15513,24 @@
                                 return 'text-anchor: middle;';
                         }
                     }
                 }();
                 return withOverflowWrap(
                     A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bq,
+                        config.bv,
                         $elm$svg$Svg$text_,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__label'),
                                 $elm$svg$Svg$Attributes$stroke(config.v),
                                 $elm$svg$Svg$Attributes$strokeWidth(
                                     $elm$core$String$fromFloat(config.x)),
-                                $elm$svg$Svg$Attributes$fill(config.by),
-                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.eZ, point.e_, config.g, config.h),
+                                $elm$svg$Svg$Attributes$fill(config.bD),
+                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fg, point.fh, config.g, config.h),
                                 $elm$svg$Svg$Attributes$style(
                                     A2(
                                         $elm$core$String$join,
                                         ' ',
                                         _List_fromArray(
                                             ['pointer-events: none;', fontStyle, anchorStyle, uppercaseStyle])))
                             ]),
@@ -15739,26 +15539,26 @@
                                 A2($elm$svg$Svg$tspan, _List_Nil, inner)
                             ])));
             } else {
                 var ellipsis = _v0.a;
                 var xOffWithAnchor = function() {
                     var _v11 = config.i;
                     if (_v11.$ === 1) {
-                        return config.g - (ellipsis.eY / 2);
+                        return config.g - (ellipsis.ff / 2);
                     } else {
                         switch (_v11.a) {
                             case 0:
                                 var _v12 = _v11.a;
-                                return config.g - ellipsis.eY;
+                                return config.g - ellipsis.ff;
                             case 1:
                                 var _v13 = _v11.a;
                                 return config.g;
                             default:
                                 var _v14 = _v11.a;
-                                return config.g - (ellipsis.eY / 2);
+                                return config.g - (ellipsis.ff / 2);
                         }
                     }
                 }();
                 var withOverflowWrap = function(el) {
                     return config.l ? A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
@@ -15798,49 +15598,49 @@
                                 return A2($elm$html$Html$Attributes$style, 'text-align', 'center');
                         }
                     }
                 }();
                 return withOverflowWrap(
                     A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bq,
+                        config.bv,
                         $elm$svg$Svg$foreignObject,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__label'),
                                 $elm$svg$Svg$Attributes$class('elm-charts__html-label'),
                                 $elm$svg$Svg$Attributes$width(
-                                    $elm$core$String$fromFloat(ellipsis.eY)),
+                                    $elm$core$String$fromFloat(ellipsis.ff)),
                                 $elm$svg$Svg$Attributes$height(
-                                    $elm$core$String$fromFloat(ellipsis.d$)),
-                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.eZ, point.e_, xOffWithAnchor, config.h - 10)
+                                    $elm$core$String$fromFloat(ellipsis.eb)),
+                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fg, point.fh, xOffWithAnchor, config.h - 10)
                             ]),
                         _List_fromArray(
                             [
                                 A2(
                                     $elm$html$Html$div,
                                     _List_fromArray(
                                         [
                                             A2($elm$html$Html$Attributes$attribute, 'xmlns', 'http://www.w3.org/1999/xhtml'),
                                             A2($elm$html$Html$Attributes$style, 'white-space', 'nowrap'),
                                             A2($elm$html$Html$Attributes$style, 'overflow', 'hidden'),
                                             A2($elm$html$Html$Attributes$style, 'text-overflow', 'ellipsis'),
                                             A2($elm$html$Html$Attributes$style, 'height', '100%'),
                                             A2($elm$html$Html$Attributes$style, 'pointer-events', 'none'),
-                                            A2($elm$html$Html$Attributes$style, 'color', config.by),
+                                            A2($elm$html$Html$Attributes$style, 'color', config.bD),
                                             fontStyle,
                                             uppercaseStyle,
                                             anchorStyle
                                         ]),
                                     inner)
                             ])));
             }
         });
     var $terezka$elm_charts$Chart$Attributes$zero = function(b) {
-        return A3($elm$core$Basics$clamp, b.fD, b.fB, 0);
+        return A3($elm$core$Basics$clamp, b.et, b.er, 0);
     };
     var $terezka$elm_charts$Chart$xLabels = function(edits) {
         var toTicks = F2(
             function(p, config) {
                 return A4(
                     $terezka$elm_charts$Chart$generateValues,
                     config.J,
@@ -15848,39 +15648,39 @@
                     config.F,
                     A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, x) {
                                 return f(x);
                             }),
-                        p.eZ,
+                        p.fg,
                         config.t));
             });
         var toTickValues = F3(
             function(p, config, ts) {
                 return (!config.f) ? ts : _Utils_update(
                     ts, {
                         A: _Utils_ap(
                             ts.A,
                             A2(
                                 $elm$core$List$map,
                                 function($) {
-                                    return $.U;
+                                    return $.W;
                                 },
                                 A2(toTicks, p, config)))
                     });
             });
         var toConfig = function(p) {
             return A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
                     J: 5,
                     i: $elm$core$Maybe$Nothing,
-                    bq: _List_Nil,
-                    by: '#808BAB',
+                    bv: _List_Nil,
+                    bD: '#808BAB',
                     j: $elm$core$Maybe$Nothing,
                     e: false,
                     k: $elm$core$Maybe$Nothing,
                     F: $elm$core$Maybe$Nothing,
                     M: $terezka$elm_charts$Internal$Svg$Floats,
                     f: false,
                     l: false,
@@ -15902,30 +15702,30 @@
                     var toLabel = function(item) {
                         return A4(
                             $terezka$elm_charts$Internal$Svg$label,
                             p,
                             _Utils_update(
                                 _default, {
                                     i: config.i,
-                                    bq: config.bq,
-                                    by: config.by,
+                                    bv: config.bv,
+                                    bD: config.bD,
                                     j: config.j,
                                     k: config.k,
                                     l: config.l,
                                     o: config.o,
                                     p: config.p,
                                     g: config.g,
                                     h: config.e ? ((-config.h) + 10) : config.h
                                 }),
                             _List_fromArray(
                                 [
-                                    $elm$svg$Svg$text(item.eb)
+                                    $elm$svg$Svg$text(item.en)
                                 ]), {
-                                eZ: item.U,
-                                e_: config.n(p.e_)
+                                fg: item.W,
+                                fh: config.n(p.fh)
                             });
                     };
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__x-labels')
@@ -15947,39 +15747,39 @@
                     config.F,
                     A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, y) {
                                 return f(y);
                             }),
-                        p.e_,
+                        p.fh,
                         config.t));
             });
         var toTickValues = F3(
             function(p, config, ts) {
                 return (!config.f) ? ts : _Utils_update(
                     ts, {
                         I: _Utils_ap(
                             ts.I,
                             A2(
                                 $elm$core$List$map,
                                 function($) {
-                                    return $.U;
+                                    return $.W;
                                 },
                                 A2(toTicks, p, config)))
                     });
             });
         var toConfig = function(p) {
             return A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
                     J: 5,
                     i: $elm$core$Maybe$Nothing,
-                    bq: _List_Nil,
-                    by: '#808BAB',
+                    bv: _List_Nil,
+                    bD: '#808BAB',
                     j: $elm$core$Maybe$Nothing,
                     e: false,
                     k: $elm$core$Maybe$Nothing,
                     F: $elm$core$Maybe$Nothing,
                     M: $terezka$elm_charts$Internal$Svg$Floats,
                     f: false,
                     l: false,
@@ -16010,45 +15810,698 @@
                                             return $elm$core$Maybe$Just(
                                                 config.e ? 1 : 0);
                                         } else {
                                             var anchor = _v0.a;
                                             return $elm$core$Maybe$Just(anchor);
                                         }
                                     }(),
-                                    bq: config.bq,
-                                    by: config.by,
+                                    bv: config.bv,
+                                    bD: config.bD,
                                     j: config.j,
                                     k: config.k,
                                     l: config.l,
                                     o: config.o,
                                     p: config.p,
                                     g: config.e ? (-config.g) : config.g,
                                     h: config.h
                                 }),
                             _List_fromArray(
                                 [
-                                    $elm$svg$Svg$text(item.eb)
+                                    $elm$svg$Svg$text(item.en)
                                 ]), {
-                                eZ: config.n(p.eZ),
-                                e_: item.U
+                                fg: config.n(p.fg),
+                                fh: item.W
                             });
                     };
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__y-labels')
                             ]),
                         A2(
                             $elm$core$List$map,
                             toLabel,
                             A2(toTicks, p, config)));
                 }));
     };
+    var $author$project$Graph$getEpaChart = F2(
+        function(graphModel, onHover) {
+            return A2(
+                $terezka$elm_charts$Chart$chart,
+                _List_fromArray(
+                    [
+                        $terezka$elm_charts$Chart$Attributes$height(300),
+                        $terezka$elm_charts$Chart$Attributes$width(1000),
+                        A2(
+                            $terezka$elm_charts$Chart$Events$onMouseMove,
+                            onHover,
+                            $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
+                        $terezka$elm_charts$Chart$Events$onMouseLeave(
+                            onHover(_List_Nil))
+                    ]),
+                _List_fromArray(
+                    [
+                        $terezka$elm_charts$Chart$xLabels(
+                            _List_fromArray(
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$moveDown(25),
+                                    $terezka$elm_charts$Chart$Attributes$withGrid,
+                                    $terezka$elm_charts$Chart$Attributes$rotate(60),
+                                    $terezka$elm_charts$Chart$Attributes$format($author$project$Graph$formatTime)
+                                ])),
+                        $terezka$elm_charts$Chart$yLabels(
+                            _List_fromArray(
+                                [$terezka$elm_charts$Chart$Attributes$withGrid])),
+                        A3(
+                            $terezka$elm_charts$Chart$series,
+                            function($) {
+                                return $.cG;
+                            },
+                            _List_fromArray(
+                                [
+                                    A2(
+                                        $terezka$elm_charts$Chart$named,
+                                        'EPA',
+                                        A3(
+                                            $terezka$elm_charts$Chart$interpolated,
+                                            function($) {
+                                                return $.d1;
+                                            },
+                                            _List_fromArray(
+                                                [
+                                                    $terezka$elm_charts$Chart$Attributes$monotone,
+                                                    $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$blue)
+                                                ]),
+                                            _List_fromArray(
+                                                [
+                                                    $terezka$elm_charts$Chart$Attributes$circle,
+                                                    $terezka$elm_charts$Chart$Attributes$size(3)
+                                                ])))
+                                ]),
+                            graphModel.bN),
+                        A2(
+                            $terezka$elm_charts$Chart$each,
+                            graphModel.bE,
+                            F2(
+                                function(p, item) {
+                                    return _List_fromArray(
+                                        [
+                                            A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
+                                        ]);
+                                })),
+                        A4(
+                            $terezka$elm_charts$Chart$legendsAt,
+                            function($) {
+                                return $.et;
+                            },
+                            function($) {
+                                return $.er;
+                            },
+                            _List_fromArray(
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$row,
+                                    $terezka$elm_charts$Chart$Attributes$alignLeft,
+                                    $terezka$elm_charts$Chart$Attributes$spacing(5),
+                                    $terezka$elm_charts$Chart$Attributes$background('Azure'),
+                                    $terezka$elm_charts$Chart$Attributes$border('gray'),
+                                    $terezka$elm_charts$Chart$Attributes$borderWidth(1),
+                                    $terezka$elm_charts$Chart$Attributes$htmlAttrs(
+                                        _List_fromArray(
+                                            [
+                                                A2($elm$html$Html$Attributes$style, 'padding', '0px 4px')
+                                            ]))
+                                ]),
+                            _List_fromArray(
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$fontSize(12)
+                                ]))
+                    ]));
+        });
+    var $terezka$elm_charts$Chart$Attributes$red = $terezka$elm_charts$Internal$Helpers$red;
     var $terezka$elm_charts$Chart$Attributes$yellow = $terezka$elm_charts$Internal$Helpers$yellow;
+    var $author$project$Graph$getReadChart = F2(
+        function(graphModel, onHover) {
+            return A2(
+                $terezka$elm_charts$Chart$chart,
+                _List_fromArray(
+                    [
+                        $terezka$elm_charts$Chart$Attributes$height(300),
+                        $terezka$elm_charts$Chart$Attributes$width(1000),
+                        A2(
+                            $terezka$elm_charts$Chart$Events$onMouseMove,
+                            onHover,
+                            $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
+                        $terezka$elm_charts$Chart$Events$onMouseLeave(
+                            onHover(_List_Nil))
+                    ]),
+                _List_fromArray(
+                    [
+                        $terezka$elm_charts$Chart$xLabels(
+                            _List_fromArray(
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$moveDown(25),
+                                    $terezka$elm_charts$Chart$Attributes$withGrid,
+                                    $terezka$elm_charts$Chart$Attributes$rotate(60),
+                                    $terezka$elm_charts$Chart$Attributes$format($author$project$Graph$formatTime)
+                                ])),
+                        $terezka$elm_charts$Chart$yLabels(
+                            _List_fromArray(
+                                [$terezka$elm_charts$Chart$Attributes$withGrid])),
+                        A3(
+                            $terezka$elm_charts$Chart$series,
+                            function($) {
+                                return $.cG;
+                            },
+                            _List_fromArray(
+                                [
+                                    A2(
+                                        $terezka$elm_charts$Chart$named,
+                                        'PM2.5',
+                                        A3(
+                                            $terezka$elm_charts$Chart$interpolated,
+                                            function($) {
+                                                return $.eE;
+                                            },
+                                            _List_fromArray(
+                                                [
+                                                    $terezka$elm_charts$Chart$Attributes$monotone,
+                                                    $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$yellow)
+                                                ]),
+                                            _List_fromArray(
+                                                [
+                                                    $terezka$elm_charts$Chart$Attributes$circle,
+                                                    $terezka$elm_charts$Chart$Attributes$size(3)
+                                                ]))),
+                                    A2(
+                                        $terezka$elm_charts$Chart$named,
+                                        'PM10',
+                                        A3(
+                                            $terezka$elm_charts$Chart$interpolated,
+                                            function($) {
+                                                return $.eD;
+                                            },
+                                            _List_fromArray(
+                                                [
+                                                    $terezka$elm_charts$Chart$Attributes$monotone,
+                                                    $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$red)
+                                                ]),
+                                            _List_fromArray(
+                                                [
+                                                    $terezka$elm_charts$Chart$Attributes$circle,
+                                                    $terezka$elm_charts$Chart$Attributes$size(3)
+                                                ])))
+                                ]),
+                            graphModel.bN),
+                        A2(
+                            $terezka$elm_charts$Chart$each,
+                            graphModel.bE,
+                            F2(
+                                function(p, item) {
+                                    return _List_fromArray(
+                                        [
+                                            A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
+                                        ]);
+                                })),
+                        A4(
+                            $terezka$elm_charts$Chart$legendsAt,
+                            function($) {
+                                return $.et;
+                            },
+                            function($) {
+                                return $.er;
+                            },
+                            _List_fromArray(
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$row,
+                                    $terezka$elm_charts$Chart$Attributes$alignLeft,
+                                    $terezka$elm_charts$Chart$Attributes$spacing(5),
+                                    $terezka$elm_charts$Chart$Attributes$background('Azure'),
+                                    $terezka$elm_charts$Chart$Attributes$border('gray'),
+                                    $terezka$elm_charts$Chart$Attributes$borderWidth(1),
+                                    $terezka$elm_charts$Chart$Attributes$htmlAttrs(
+                                        _List_fromArray(
+                                            [
+                                                A2($elm$html$Html$Attributes$style, 'padding', '0px 4px')
+                                            ]))
+                                ]),
+                            _List_fromArray(
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$fontSize(12)
+                                ]))
+                    ]));
+        });
+    var $author$project$Main$ChangeWindow = function(a) {
+        return {
+            $: 4,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Attrs = function(a) {
+        return {
+            $: 4,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Button$attrs = function(attrs_) {
+        return $rundis$elm_bootstrap$Bootstrap$Internal$Button$Attrs(attrs_);
+    };
+    var $elm$virtual_dom$VirtualDom$MayPreventDefault = function(a) {
+        return {
+            $: 2,
+            a: a
+        };
+    };
+    var $elm$html$Html$Events$preventDefaultOn = F2(
+        function(event, decoder) {
+            return A2(
+                $elm$virtual_dom$VirtualDom$on,
+                event,
+                $elm$virtual_dom$VirtualDom$MayPreventDefault(decoder));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Button$onClick = function(message) {
+        return $rundis$elm_bootstrap$Bootstrap$Button$attrs(
+            _List_fromArray(
+                [
+                    A2(
+                        $elm$html$Html$Events$preventDefaultOn,
+                        'click',
+                        $elm$json$Json$Decode$succeed(
+                            _Utils_Tuple2(message, true)))
+                ]));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring = function(a) {
+        return {
+            $: 1,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined = function(a) {
+        return {
+            $: 1,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Primary = 0;
+    var $rundis$elm_bootstrap$Bootstrap$Button$outlinePrimary = $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring(
+        $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined(0));
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$RadioButtonItem = $elm$core$Basics$identity;
+    var $elm$html$Html$Attributes$autocomplete = function(bool) {
+        return A2(
+            $elm$html$Html$Attributes$stringProperty,
+            'autocomplete',
+            bool ? 'on' : 'off');
+    };
+    var $elm$core$Maybe$andThen = F2(
+        function(callback, maybeValue) {
+            if (!maybeValue.$) {
+                var value = maybeValue.a;
+                return callback(value);
+            } else {
+                return $elm$core$Maybe$Nothing;
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$applyModifier = F2(
+        function(modifier, options) {
+            switch (modifier.$) {
+                case 0:
+                    var size = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            eZ: $elm$core$Maybe$Just(size)
+                        });
+                case 1:
+                    var coloring = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            Z: $elm$core$Maybe$Just(coloring)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            bx: true
+                        });
+                case 3:
+                    var val = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bJ: val
+                        });
+                default:
+                    var attrs = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bu: _Utils_ap(options.bu, attrs)
+                        });
+            }
+        });
+    var $elm$html$Html$Attributes$classList = function(classes) {
+        return $elm$html$Html$Attributes$class(
+            A2(
+                $elm$core$String$join,
+                ' ',
+                A2(
+                    $elm$core$List$map,
+                    $elm$core$Tuple$first,
+                    A2($elm$core$List$filter, $elm$core$Tuple$second, classes))));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$defaultOptions = {
+        bu: _List_Nil,
+        bx: false,
+        Z: $elm$core$Maybe$Nothing,
+        bJ: false,
+        eZ: $elm$core$Maybe$Nothing
+    };
+    var $elm$json$Json$Encode$bool = _Json_wrap;
+    var $elm$html$Html$Attributes$boolProperty = F2(
+        function(key, bool) {
+            return A2(
+                _VirtualDom_property,
+                key,
+                $elm$json$Json$Encode$bool(bool));
+        });
+    var $elm$html$Html$Attributes$disabled = $elm$html$Html$Attributes$boolProperty('disabled');
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass = function(role) {
+        switch (role) {
+            case 0:
+                return 'primary';
+            case 1:
+                return 'secondary';
+            case 2:
+                return 'success';
+            case 3:
+                return 'info';
+            case 4:
+                return 'warning';
+            case 5:
+                return 'danger';
+            case 6:
+                return 'dark';
+            case 7:
+                return 'light';
+            default:
+                return 'link';
+        }
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$buttonAttributes = function(modifiers) {
+        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Internal$Button$applyModifier, $rundis$elm_bootstrap$Bootstrap$Internal$Button$defaultOptions, modifiers);
+        return _Utils_ap(
+            _List_fromArray(
+                [
+                    $elm$html$Html$Attributes$classList(
+                        _List_fromArray(
+                            [
+                                _Utils_Tuple2('btn', true),
+                                _Utils_Tuple2('btn-block', options.bx),
+                                _Utils_Tuple2('disabled', options.bJ)
+                            ])),
+                    $elm$html$Html$Attributes$disabled(options.bJ)
+                ]),
+            _Utils_ap(
+                function() {
+                    var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.eZ);
+                    if (!_v0.$) {
+                        var s = _v0.a;
+                        return _List_fromArray(
+                            [
+                                $elm$html$Html$Attributes$class('btn-' + s)
+                            ]);
+                    } else {
+                        return _List_Nil;
+                    }
+                }(),
+                _Utils_ap(
+                    function() {
+                        var _v1 = options.Z;
+                        if (!_v1.$) {
+                            if (!_v1.a.$) {
+                                var role = _v1.a.a;
+                                return _List_fromArray(
+                                    [
+                                        $elm$html$Html$Attributes$class(
+                                            'btn-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
+                                    ]);
+                            } else {
+                                var role = _v1.a.a;
+                                return _List_fromArray(
+                                    [
+                                        $elm$html$Html$Attributes$class(
+                                            'btn-outline-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
+                                    ]);
+                            }
+                        } else {
+                            return _List_Nil;
+                        }
+                    }(),
+                    options.bu)));
+    };
+    var $elm$html$Html$Attributes$checked = $elm$html$Html$Attributes$boolProperty('checked');
+    var $elm$html$Html$input = _VirtualDom_node('input');
+    var $elm$html$Html$label = _VirtualDom_node('label');
+    var $elm$html$Html$Attributes$type_ = $elm$html$Html$Attributes$stringProperty('type');
+    var $rundis$elm_bootstrap$Bootstrap$Button$radioButton = F3(
+        function(checked, options, children) {
+            var hideRadio = A2($elm$html$Html$Attributes$attribute, 'data-toggle', 'button');
+            return A2(
+                $elm$html$Html$label,
+                A2(
+                    $elm$core$List$cons,
+                    $elm$html$Html$Attributes$classList(
+                        _List_fromArray(
+                            [
+                                _Utils_Tuple2('active', checked)
+                            ])),
+                    A2(
+                        $elm$core$List$cons,
+                        hideRadio,
+                        $rundis$elm_bootstrap$Bootstrap$Internal$Button$buttonAttributes(options))),
+                A2(
+                    $elm$core$List$cons,
+                    A2(
+                        $elm$html$Html$input,
+                        _List_fromArray(
+                            [
+                                $elm$html$Html$Attributes$type_('radio'),
+                                $elm$html$Html$Attributes$checked(checked),
+                                $elm$html$Html$Attributes$autocomplete(false)
+                            ]),
+                        _List_Nil),
+                    children));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButton = F3(
+        function(checked, options, children) {
+            return A3($rundis$elm_bootstrap$Bootstrap$Button$radioButton, checked, options, children);
+        });
+    var $author$project$Main$getSelector = F3(
+        function(windowDuration, textDuration, currentDuration) {
+            return A3(
+                $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButton,
+                _Utils_eq(windowDuration, currentDuration),
+                _List_fromArray(
+                    [
+                        $rundis$elm_bootstrap$Bootstrap$Button$outlinePrimary,
+                        $rundis$elm_bootstrap$Bootstrap$Button$onClick(
+                            $author$project$Main$ChangeWindow(windowDuration))
+                    ]),
+                _List_fromArray(
+                    [
+                        $elm$html$Html$text(textDuration)
+                    ]));
+        });
+    var $elm$html$Html$h1 = _VirtualDom_node('h1');
+    var $elm$html$Html$h2 = _VirtualDom_node('h2');
+    var $author$project$Main$htmlIf = F2(
+        function(el, cond) {
+            return cond ? el : $elm$html$Html$text('');
+        });
+    var $rundis$elm_bootstrap$Bootstrap$General$Internal$LG = 3;
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColWidth = function(a) {
+        return {
+            $: 0,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$width = F2(
+        function(size, count) {
+            return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColWidth(
+                A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, size, count));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$lg = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$width, 3, 0);
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col3 = 3;
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3 = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$width, 3, 3);
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$GroupItem = $elm$core$Basics$identity;
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier = F2(
+        function(modifier, options) {
+            switch (modifier.$) {
+                case 0:
+                    var size = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            eZ: $elm$core$Maybe$Just(size)
+                        });
+                case 1:
+                    return _Utils_update(
+                        options, {
+                            cR: true
+                        });
+                default:
+                    var attrs_ = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bu: _Utils_ap(options.bu, attrs_)
+                        });
+            }
+        });
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions = {
+        bu: _List_Nil,
+        eZ: $elm$core$Maybe$Nothing,
+        cR: false
+    };
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes = F2(
+        function(toggle, modifiers) {
+            var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions, modifiers);
+            return _Utils_ap(
+                _List_fromArray(
+                    [
+                        A2($elm$html$Html$Attributes$attribute, 'role', 'group'),
+                        $elm$html$Html$Attributes$classList(
+                            _List_fromArray(
+                                [
+                                    _Utils_Tuple2('btn-group', true),
+                                    _Utils_Tuple2('btn-group-toggle', toggle),
+                                    _Utils_Tuple2('btn-group-vertical', options.cR)
+                                ])),
+                        A2($elm$html$Html$Attributes$attribute, 'data-toggle', 'buttons')
+                    ]),
+                _Utils_ap(
+                    function() {
+                        var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.eZ);
+                        if (!_v0.$) {
+                            var s = _v0.a;
+                            return _List_fromArray(
+                                [
+                                    $elm$html$Html$Attributes$class('btn-group-' + s)
+                                ]);
+                        } else {
+                            return _List_Nil;
+                        }
+                    }(),
+                    options.bu));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem = F2(
+        function(options, items) {
+            return A2(
+                $elm$html$Html$div,
+                A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes, true, options),
+                A2(
+                    $elm$core$List$map,
+                    function(_v0) {
+                        var elem = _v0;
+                        return elem;
+                    },
+                    items));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$renderGroup = function(_v0) {
+        var elem = _v0;
+        return elem;
+    };
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroup = F2(
+        function(options, items) {
+            return $rundis$elm_bootstrap$Bootstrap$ButtonGroup$renderGroup(
+                A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem, options, items));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$Center = 1;
+    var $rundis$elm_bootstrap$Bootstrap$Text$alignMd = function(dir) {
+        return {
+            d_: dir,
+            eZ: 2
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter = $rundis$elm_bootstrap$Bootstrap$Text$alignMd(1);
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$TextAlign = function(a) {
+        return {
+            $: 7,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign = function(align) {
+        return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$TextAlign(align);
+    };
+    var $author$project$Main$viewBigNumber = F2(
+        function(value, numberType) {
+            return A2(
+                $rundis$elm_bootstrap$Bootstrap$Grid$container,
+                _List_fromArray(
+                    [
+                        A2($elm$html$Html$Attributes$style, 'background-clip', 'border-box'),
+                        A2($elm$html$Html$Attributes$style, 'border', '1px solid darkgray'),
+                        A2($elm$html$Html$Attributes$style, 'padding', '0'),
+                        A2($elm$html$Html$Attributes$style, 'border-radius', '.25rem')
+                    ]),
+                _List_fromArray(
+                    [
+                        A2(
+                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                            _List_Nil,
+                            _List_fromArray(
+                                [
+                                    A2(
+                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                        _List_fromArray(
+                                            [
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign($rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter)
+                                            ]),
+                                        _List_fromArray(
+                                            [
+                                                A2(
+                                                    $elm$html$Html$h1,
+                                                    _List_fromArray(
+                                                        [
+                                                            A2($elm$html$Html$Attributes$style, 'padding', '.5em'),
+                                                            A2($elm$html$Html$Attributes$style, 'margin', '0'),
+                                                            A2($elm$html$Html$Attributes$style, 'color', 'white'),
+                                                            A2($elm$html$Html$Attributes$style, 'background-color', 'lightblue')
+                                                        ]),
+                                                    _List_fromArray(
+                                                        [
+                                                            $elm$html$Html$text(
+                                                                $elm$core$String$fromFloat(value))
+                                                        ]))
+                                            ]))
+                                ])),
+                        A2(
+                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                            _List_Nil,
+                            _List_fromArray(
+                                [
+                                    A2(
+                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                        _List_fromArray(
+                                            [
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign($rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter)
+                                            ]),
+                                        _List_fromArray(
+                                            [
+                                                A2(
+                                                    $elm$html$Html$h5,
+                                                    _List_fromArray(
+                                                        [
+                                                            A2($elm$html$Html$Attributes$style, 'padding', '.25em'),
+                                                            A2($elm$html$Html$Attributes$style, 'margin', '0'),
+                                                            A2($elm$html$Html$Attributes$style, 'color', 'darkblue'),
+                                                            A2($elm$html$Html$Attributes$style, 'background-color', 'lightgray')
+                                                        ]),
+                                                    _List_fromArray(
+                                                        [
+                                                            $elm$html$Html$text(numberType)
+                                                        ]))
+                                            ]))
+                                ]))
+                    ]));
+        });
     var $author$project$Main$view = function(model) {
         return A2(
             $elm$html$Html$div,
             _List_Nil,
             _List_fromArray(
                 [
                     A2(
@@ -16089,19 +16542,56 @@
                                                                 ]))
                                                     ])),
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_Nil,
                                                 _List_fromArray(
                                                     [
-                                                        $author$project$DeviceStatus$getDeviceInfo(model.co)
+                                                        $author$project$DeviceStatus$getDeviceInfo(model.V)
                                                     ]))
                                         ]))
                             ])),
                     A2(
+                        $author$project$Main$htmlIf,
+                        A2(
+                            $rundis$elm_bootstrap$Bootstrap$Grid$container,
+                            _List_Nil,
+                            _List_fromArray(
+                                [
+                                    A2(
+                                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                        _List_Nil,
+                                        _List_fromArray(
+                                            [
+                                                A2(
+                                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                    _List_fromArray(
+                                                        [
+                                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                                _List_fromArray(
+                                                                    [
+                                                                        $elm$html$Html$Attributes$class('alert'),
+                                                                        $elm$html$Html$Attributes$class('alert-danger')
+                                                                    ]))
+                                                        ]),
+                                                    _List_fromArray(
+                                                        [
+                                                            A2(
+                                                                $elm$html$Html$h5,
+                                                                _List_Nil,
+                                                                _List_fromArray(
+                                                                    [
+                                                                        $elm$html$Html$text(model.T.al)
+                                                                    ])),
+                                                            $elm$html$Html$text(model.T.ak)
+                                                        ]))
+                                            ]))
+                                ])),
+                        model.T.an),
+                    A2(
                         $rundis$elm_bootstrap$Bootstrap$Grid$container,
                         _List_Nil,
                         _List_fromArray(
                             [
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                     _List_fromArray(
@@ -16110,31 +16600,31 @@
                                         [
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_fromArray(
                                                     [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
                                                 _List_fromArray(
                                                     [
-                                                        A2($author$project$Main$viewBigNumber, model.az.aM, 'EPA')
+                                                        A2($author$project$Main$viewBigNumber, model.aE.d1, 'EPA')
                                                     ])),
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_fromArray(
                                                     [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
                                                 _List_fromArray(
                                                     [
-                                                        A2($author$project$Main$viewBigNumber, model.az.aZ, 'PM2.5')
+                                                        A2($author$project$Main$viewBigNumber, model.aE.eE, 'PM2.5')
                                                     ])),
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_fromArray(
                                                     [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
                                                 _List_fromArray(
                                                     [
-                                                        A2($author$project$Main$viewBigNumber, model.az.aY, 'PM10')
+                                                        A2($author$project$Main$viewBigNumber, model.aE.eD, 'PM10')
                                                     ]))
                                         ])),
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                     _List_fromArray(
                                         [
                                             $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
@@ -16153,29 +16643,49 @@
                                                 _List_fromArray(
                                                     [
                                                         A2(
                                                             $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroup,
                                                             _List_Nil,
                                                             _List_fromArray(
                                                                 [
-                                                                    A3($author$project$Main$getSelector, 0, 'All', model.ac),
-                                                                    A3($author$project$Main$getSelector, 1, 'Hour', model.ac),
-                                                                    A3($author$project$Main$getSelector, 2, 'Day', model.ac),
-                                                                    A3($author$project$Main$getSelector, 3, 'Week', model.ac)
+                                                                    A3($author$project$Main$getSelector, 0, 'All', model.ae),
+                                                                    A3($author$project$Main$getSelector, 1, 'Hour', model.ae),
+                                                                    A3($author$project$Main$getSelector, 2, 'Day', model.ae),
+                                                                    A3($author$project$Main$getSelector, 3, 'Week', model.ae)
+                                                                ]))
+                                                    ]))
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                _List_Nil,
+                                                _List_fromArray(
+                                                    [
+                                                        A2(
+                                                            $elm$html$Html$h2,
+                                                            _List_Nil,
+                                                            _List_fromArray(
+                                                                [
+                                                                    $elm$html$Html$text('EPA AQI')
                                                                 ]))
                                                     ]))
                                         ])),
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                     _List_fromArray(
                                         [
                                             $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
                                                 _List_fromArray(
                                                     [
-                                                        A2($elm$html$Html$Attributes$style, 'padding-top', '1em')
+                                                        A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
+                                                        A2($elm$html$Html$Attributes$style, 'padding-bottom', '3em')
                                                     ])),
                                             $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd
                                         ]),
                                     _List_fromArray(
                                         [
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
@@ -16188,150 +16698,86 @@
                                                             _List_fromArray(
                                                                 [
                                                                     A2($elm$html$Html$Attributes$style, 'height', '400px')
                                                                 ]),
                                                             _List_fromArray(
                                                                 [
                                                                     A2(
-                                                                        $terezka$elm_charts$Chart$chart,
-                                                                        _List_fromArray(
-                                                                            [
-                                                                                $terezka$elm_charts$Chart$Attributes$height(300),
-                                                                                $terezka$elm_charts$Chart$Attributes$width(1000),
-                                                                                A2(
-                                                                                    $terezka$elm_charts$Chart$Events$onMouseMove,
-                                                                                    $author$project$Main$OnHover,
-                                                                                    $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
-                                                                                $terezka$elm_charts$Chart$Events$onMouseLeave(
-                                                                                    $author$project$Main$OnHover(_List_Nil))
-                                                                            ]),
-                                                                        _List_fromArray(
-                                                                            [
-                                                                                $terezka$elm_charts$Chart$xLabels(
-                                                                                    _List_fromArray(
-                                                                                        [
-                                                                                            $terezka$elm_charts$Chart$Attributes$moveDown(25),
-                                                                                            $terezka$elm_charts$Chart$Attributes$withGrid,
-                                                                                            $terezka$elm_charts$Chart$Attributes$rotate(60),
-                                                                                            $terezka$elm_charts$Chart$Attributes$format($author$project$Main$formatTime)
-                                                                                        ])),
-                                                                                $terezka$elm_charts$Chart$yLabels(
-                                                                                    _List_fromArray(
-                                                                                        [$terezka$elm_charts$Chart$Attributes$withGrid])),
-                                                                                A3(
-                                                                                    $terezka$elm_charts$Chart$series,
-                                                                                    function($) {
-                                                                                        return $.cA;
-                                                                                    },
-                                                                                    _List_fromArray(
-                                                                                        [
-                                                                                            A2(
-                                                                                                $terezka$elm_charts$Chart$named,
-                                                                                                'EPA',
-                                                                                                A3(
-                                                                                                    $terezka$elm_charts$Chart$interpolated,
-                                                                                                    function($) {
-                                                                                                        return $.aM;
-                                                                                                    },
-                                                                                                    _List_fromArray(
-                                                                                                        [
-                                                                                                            $terezka$elm_charts$Chart$Attributes$monotone,
-                                                                                                            $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$blue)
-                                                                                                        ]),
-                                                                                                    _List_fromArray(
-                                                                                                        [
-                                                                                                            $terezka$elm_charts$Chart$Attributes$circle,
-                                                                                                            $terezka$elm_charts$Chart$Attributes$size(3)
-                                                                                                        ]))),
-                                                                                            A2(
-                                                                                                $terezka$elm_charts$Chart$named,
-                                                                                                'PM2.5',
-                                                                                                A3(
-                                                                                                    $terezka$elm_charts$Chart$interpolated,
-                                                                                                    function($) {
-                                                                                                        return $.aZ;
-                                                                                                    },
-                                                                                                    _List_fromArray(
-                                                                                                        [
-                                                                                                            $terezka$elm_charts$Chart$Attributes$monotone,
-                                                                                                            $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$yellow)
-                                                                                                        ]),
-                                                                                                    _List_fromArray(
-                                                                                                        [
-                                                                                                            $terezka$elm_charts$Chart$Attributes$circle,
-                                                                                                            $terezka$elm_charts$Chart$Attributes$size(3)
-                                                                                                        ]))),
-                                                                                            A2(
-                                                                                                $terezka$elm_charts$Chart$named,
-                                                                                                'PM10',
-                                                                                                A3(
-                                                                                                    $terezka$elm_charts$Chart$interpolated,
-                                                                                                    function($) {
-                                                                                                        return $.aY;
-                                                                                                    },
-                                                                                                    _List_fromArray(
-                                                                                                        [
-                                                                                                            $terezka$elm_charts$Chart$Attributes$monotone,
-                                                                                                            $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$red)
-                                                                                                        ]),
-                                                                                                    _List_fromArray(
-                                                                                                        [
-                                                                                                            $terezka$elm_charts$Chart$Attributes$circle,
-                                                                                                            $terezka$elm_charts$Chart$Attributes$size(3)
-                                                                                                        ])))
-                                                                                        ]),
-                                                                                    model.bm),
-                                                                                A2(
-                                                                                    $terezka$elm_charts$Chart$each,
-                                                                                    model.bQ,
-                                                                                    F2(
-                                                                                        function(p, item) {
-                                                                                            return _List_fromArray(
-                                                                                                [
-                                                                                                    A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
-                                                                                                ]);
-                                                                                        })),
-                                                                                A4(
-                                                                                    $terezka$elm_charts$Chart$legendsAt,
-                                                                                    function($) {
-                                                                                        return $.fD;
-                                                                                    },
-                                                                                    function($) {
-                                                                                        return $.fB;
-                                                                                    },
-                                                                                    _List_fromArray(
-                                                                                        [
-                                                                                            $terezka$elm_charts$Chart$Attributes$row,
-                                                                                            $terezka$elm_charts$Chart$Attributes$alignLeft,
-                                                                                            $terezka$elm_charts$Chart$Attributes$spacing(5),
-                                                                                            $terezka$elm_charts$Chart$Attributes$background('Azure'),
-                                                                                            $terezka$elm_charts$Chart$Attributes$border('gray'),
-                                                                                            $terezka$elm_charts$Chart$Attributes$borderWidth(1),
-                                                                                            $terezka$elm_charts$Chart$Attributes$htmlAttrs(
-                                                                                                _List_fromArray(
-                                                                                                    [
-                                                                                                        A2($elm$html$Html$Attributes$style, 'padding', '0px 4px')
-                                                                                                    ]))
-                                                                                        ]),
-                                                                                    _List_fromArray(
-                                                                                        [
-                                                                                            $terezka$elm_charts$Chart$Attributes$fontSize(12)
-                                                                                        ]))
-                                                                            ]))
+                                                                        $author$project$Graph$getEpaChart, {
+                                                                            bE: model.bW,
+                                                                            bN: model.bq
+                                                                        },
+                                                                        $author$project$Main$OnEpaHover)
+                                                                ]))
+                                                    ]))
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                    _List_Nil,
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                _List_Nil,
+                                                _List_fromArray(
+                                                    [
+                                                        A2(
+                                                            $elm$html$Html$h2,
+                                                            _List_Nil,
+                                                            _List_fromArray(
+                                                                [
+                                                                    $elm$html$Html$text('PM2.5/PM10 Reads')
+                                                                ]))
+                                                    ]))
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
+                                                        A2($elm$html$Html$Attributes$style, 'padding-bottom', '3em')
+                                                    ])),
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                _List_fromArray(
+                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg]),
+                                                _List_fromArray(
+                                                    [
+                                                        A2(
+                                                            $elm$html$Html$div,
+                                                            _List_fromArray(
+                                                                [
+                                                                    A2($elm$html$Html$Attributes$style, 'height', '400px')
+                                                                ]),
+                                                            _List_fromArray(
+                                                                [
+                                                                    A2(
+                                                                        $author$project$Graph$getReadChart, {
+                                                                            bE: model.bX,
+                                                                            bN: model.br
+                                                                        },
+                                                                        $author$project$Main$OnReadHover)
                                                                 ]))
                                                     ]))
                                         ]))
                             ]))
                 ]));
     };
     var $author$project$Main$main = $elm$browser$Browser$element({
-        fu: $author$project$Main$init,
-        fV: $author$project$Main$subscriptions,
-        ga: $author$project$Main$update,
-        gc: $author$project$Main$view
+        fN: $author$project$Main$init,
+        ga: $author$project$Main$subscriptions,
+        gr: $author$project$Main$update,
+        gt: $author$project$Main$view
     });
     _Platform_export({
         'Main': {
             'init': $author$project$Main$main(
                 $elm$json$Json$Decode$succeed(0))(0)
         }
     });
```

### Comparing `aqimon-0.2.1/aqimon/static/favicon-32x32.png` & `aqimon-0.3.0/aqimon/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/favicon.ico` & `aqimon-0.3.0/aqimon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/images/failing.png` & `aqimon-0.3.0/aqimon/static/images/failing.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/images/idle.png` & `aqimon-0.3.0/aqimon/static/images/idle.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/images/loading.gif` & `aqimon-0.3.0/aqimon/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/static/index.html` & `aqimon-0.3.0/aqimon/static/index.html`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/aqimon/templates/index.html` & `aqimon-0.3.0/aqimon/templates/index.html`

 * *Files identical despite different names*

### Comparing `aqimon-0.2.1/pyproject.toml` & `aqimon-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aqimon"
-version = "0.2.1"
+version = "0.3.0"
 description = "Air Quality Index Monitor"
 authors = ["Tim Orme"]
 readme = "README.md"
 include = ["aqimon/static/elm.js"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -15,27 +15,32 @@
 fastapi-utils = "^0.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.256"
 black = "^23.1.0"
 mypy = "^1.1.1"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aqimon = "aqimon.server:start"
 aqimond = "aqimon.server:debug"
 
 [tool.ruff]
 select = ["E", "F", "D"]
 ignore = ["D203", "D213"]
 line-length = 120
 
+[tool.ruff.per-file-ignores]
+"tests/*" = ["D100", "D101", "D102", "D103", "D104" ]  # We dont need docstrings in tests
+
 [tool.black]
 line-length = 120
 
 [[tool.mypy.overrides]]
 module = "serial.*"
 ignore_missing_imports = true
```

### Comparing `aqimon-0.2.1/PKG-INFO` & `aqimon-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqimon
-Version: 0.2.1
+Version: 0.3.0
 Summary: Air Quality Index Monitor
 Author: Tim Orme
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,45 +15,58 @@
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # AQIMON
 
 A simple Air Quality Index monitor, designed to work on the Raspberry Pi with the SDS011 Nova PM Sensor.
 
-## Installation
+- [AQIMON](#aqimon)
+  - [Installation](#installation)
+    - [Pre-Requisites](#pre-requisites)
+    - [Install](#install)
+  - [Running Aqimon](#running-aqimon)
+    - [Configure With Systemd](#configure-with-systemd)
+  - [Configuration](#configuration)
+  - [Contributing](#contributing)
+    - [Toolset](#toolset)
+    - [Quickstart](#quickstart)
+    - [Using the Mock Reader](#using-the-mock-reader)
+    - [Submitting a PR](#submitting-a-pr)
 
+## Installation
 
 ### Pre-Requisites
 
-* Python 3.9+
-* [uhubctl](https://github.com/mvp/uhubctl) must be installed and on your PATH.
+- Python 3.9+
 
 ### Install
 
 ```commandline
 pip install aqimon
 ```
 
 ## Running Aqimon
 
-Aqimon is a simple web server.  To start with all the defaults, you can just run:
+Aqimon is a simple web server.  To start with all the defaults (assuming available SDS011 hardware on `/dev/ttyUSB0`), you can just run:
 
 ```commandline
 aqimon
 ```
 
 And then go to your browser at `http://{serveraddress}:8000/` to view the UI.
 
+If you don't have the requisite SDS011 hardware, you can use a mock data source via a [mock reader](#using-the-mock-reader).
+
 ### Configure With Systemd
 
 Generally, you'd want to run `Aqimon` as an always-on service, using `systemd`.
 
 To do so, create a file at `/etc/systemd/system/aqimin.service` with the following contents:
 
-```
+```text
 [Unit]
 Description=AQIMON
 After=multi-user.target
 
 [Service]
 Type=simple
 Restart=always
@@ -70,38 +83,40 @@
 sudo systemctl start aqimon
 ```
 
 ## Configuration
 
 Aqimon uses environment variables for configuration, but all values should ship with sensible defaults.
 
-| Variable                         | Default             | Description                                                                                                                       |
-|----------------------------------|---------------------|-----------------------------------------------------------------------------------------------------------------------------------|
-| **AQIMON_DB_PATH**               | ~/.aqimon/db.sqlite | The path to the database file, where read information is stored. It should be an absolute path; user home expansion is supported. | 
-| **AQIMON_POLL_FREQUENCY_SEC**    | 900 (15 minutes)    | Sets how frequently to read from the device, in seconds.                                                                          |
-| **AQIMON_RETENTION_MINUTES**     | 10080 (1 week)      | Sets how long data will be kept in the database, in minutes.                                                                      |
-| **AQIMON_READER_TYPE**           | NOVAPM              | The reader type to use, either NOVAPM or MOCK.                                                                                    |
-| **AQIMON_USB_PATH**              | /dev/ttyUSB0        | The path to the USB device for the sensor.                                                                                        |
-| **AQIMON_SLEEP_TIME_SEC**        | 5                   | The number of seconds to wait for between each read in a set of reads.                                                            |
-| **AQIMON_SAMPLE_COUNT_PER_READ** | 5                   | The number of reads to take with each sample.                                                                                     |
-| **AQIMON_SERVER_PORT**           | 8000                | The port to run the server on.                                                                                                    |
-| **AQIMON_SERVER_HOST**           | 0.0.0.0             | The host to run the server on.                                                                                                    |
- 
+| Variable                           | Default             | Description                                                                                                                       |
+|------------------------------------|---------------------|-----------------------------------------------------------------------------------------------------------------------------------|
+| **AQIMON_DB_PATH**                 | ~/.aqimon/db.sqlite | The path to the database file, where read information is stored. It should be an absolute path; user home expansion is supported. |
+| **AQIMON_POLL_FREQUENCY_SEC**      | 900 (15 minutes)    | Sets how frequently to read from the device, in seconds.                                                                          |
+| **AQIMON_RETENTION_MINUTES**       | 10080 (1 week)      | Sets how long data will be kept in the database, in minutes.                                                                      |
+| **AQIMON_READER_TYPE**             | NOVAPM              | The reader type to use, either NOVAPM or MOCK.                                                                                    |
+| **AQIMON_USB_PATH**                | /dev/ttyUSB0        | The path to the USB device for the sensor.                                                                                        |
+| **AQIMON_SLEEP_SEC_BETWEEN_READS** | 5                   | The number of seconds to wait for between each read in a set of reads.                                                            |
+| **AQIMON_SAMPLE_COUNT_PER_READ**   | 5                   | The number of reads to take with each sample.                                                                                     |
+| **AQIMON_WARM_UP_SEC**             | 15                  | The number of seconds to wait for the device to warm up before reading.                                                           |
+| **AQIMON_COMMAND_WAIT_TIME**       | 1                   | The number of seconds to wait for the device respond to a command.                                                                |
+| **AQIMON_EPA_LOOKBACK_MIN**        | 60*8                | The number of minutes to look back at read data to calculate the EPA AQI.                                                         |
+| **AQIMON_SERVER_PORT**             | 8000                | The port to run the server on.                                                                                                    |
+| **AQIMON_SERVER_HOST**             | 0.0.0.0             | The host to run the server on.                                                                                                    |
 
 ## Contributing
 
 ### Toolset
 
 To start developing, you'll need to install the following tools:
 
-* [Python 3.9+](https://www.python.org/) - For API Code
-* [Elm 0.19](https://elm-lang.org/) - For client code
-* [poetry](https://python-poetry.org/) - For python package management
-* [justfile](https://github.com/casey/just) - For builds
-* [elm-format](https://github.com/avh4/elm-format) - For auto-formatting elm code.
+- [Python 3.9+](https://www.python.org/) - For API Code
+- [Elm 0.19](https://elm-lang.org/) - For client code
+- [poetry](https://python-poetry.org/) - For python package management
+- [justfile](https://github.com/casey/just) - For builds
+- [elm-format](https://github.com/avh4/elm-format) - For auto-formatting elm code.
 
 Optionally, we have [pre-commit](https://pre-commit.com/) hooks available as well.  To install hooks, just run
 `pre-commit install` and then linters and autoformatting will be applied automatically on commit.
 
 ### Quickstart
 
 To build the project, and install all dev-dependencies, run:
@@ -132,20 +147,19 @@
 
 ```commandline
 just format
 ```
 
 ### Using the Mock Reader
 
-Aqimon ships with a mock reader class that you can use in the event that you don't have a reader available on your 
+Aqimon ships with a mock reader class that you can use in the event that you don't have a reader available on your
 development computer.  The mock reader just returns randomized reads.  To use it, you can start the server like:
 
 ```commandline
 AQIMON_READER_TYPE=MOCK poetry run aqimon
 ```
 
 ### Submitting a PR
 
-Master branch is locked, but you can open a PR on the repo.  Build checks must pass, and changes approved by a code 
+Master branch is locked, but you can open a PR on the repo.  Build checks must pass, and changes approved by a code
 owner, before merging.
 
-
```

