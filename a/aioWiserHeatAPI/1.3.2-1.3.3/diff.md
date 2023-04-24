# Comparing `tmp/aioWiserHeatAPI-1.3.2.tar.gz` & `tmp/aioWiserHeatAPI-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioWiserHeatAPI-1.3.2.tar", last modified: Fri Apr 14 17:03:43 2023, max compression
+gzip compressed data, was "aioWiserHeatAPI-1.3.3.tar", last modified: Mon Apr 24 14:57:47 2023, max compression
```

## Comparing `aioWiserHeatAPI-1.3.2.tar` & `aioWiserHeatAPI-1.3.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4339 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.349615 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating_actuator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/extra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/opentherm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/special_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/zigbee.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/hot_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/rest_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    24883 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/roomstat.py
--rw-r--r--   0 runner    (1001) docker     (123)    40806 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartvalve.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/ufh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/wiserhub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.349615 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4460 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating_actuator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/extra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/opentherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/special_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/zigbee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/hot_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/rest_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24805 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/roomstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40806 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartvalve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/ufh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/wiserhub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 14:57:47.000000 aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 14:57:47.361543 aioWiserHeatAPI-1.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-04-24 14:57:36.000000 aioWiserHeatAPI-1.3.3/setup.py
```

### Comparing `aioWiserHeatAPI-1.3.2/LICENSE` & `aioWiserHeatAPI-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/PKG-INFO` & `aioWiserHeatAPI-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.3.2
+Version: 1.3.3
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Drayton Wiser Hub API Async v1.3.2
+# Drayton Wiser Hub API Async v1.3.3
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -64,14 +64,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.3
+
+* Fixed issue in passive mode so that it works with 3 channel hub and different rooms on different channels
+
 ### v1.3.2
 
 * Fixed issue ot maintaining some parameters after hub update
 * Improved handling of extra config json errors
 * Amended current_target_temp to use DisplayedSetPoint instead of CurrentSetPoint as this displays incorrectly in Eco mode
 
 ### 1.3.1
```

### Comparing `aioWiserHeatAPI-1.3.2/README.md` & `aioWiserHeatAPI-1.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Drayton Wiser Hub API Async v1.3.2
+# Drayton Wiser Hub API Async v1.3.3
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -48,14 +48,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.3
+
+* Fixed issue in passive mode so that it works with 3 channel hub and different rooms on different channels
+
 ### v1.3.2
 
 * Fixed issue ot maintaining some parameters after hub update
 * Improved handling of extra config json errors
 * Amended current_target_temp to use DisplayedSetPoint instead of CurrentSetPoint as this displays incorrectly in Eco mode
 
 ### 1.3.1
```

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/cli.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/cli.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/const.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/const.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/devices.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/devices.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/discovery.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/discovery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating_actuator.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/heating_actuator.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/battery.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/battery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/capabilities.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/capabilities.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/cloud.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/device.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/device.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/extra_config.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/extra_config.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/firmware.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/firmware.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/network.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/network.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/opentherm.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/opentherm.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/signal.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/signal.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/special_times.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/special_times.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/temp.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/temp.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/zigbee.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/helpers/zigbee.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/hot_water.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/hot_water.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/light.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/light.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/moments.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/moments.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/rest_controller.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/rest_controller.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/room.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from datetime import datetime
 from typing import Union
 
 
 from . import _LOGGER
 
 from .devices import _WiserDeviceCollection
-from .helpers.automations import _WiserRoomAutomations
 from .helpers.misc import is_value_in_list
 from .helpers.temp import _WiserTemperatureFunctions as tf
 from .rest_controller import _WiserRestController, WiserRestActionEnum
 from .schedule import _WiserSchedule, _WiserScheduleCollection
 
 from .const import (
     DEFAULT_BOOST_DELTA,
@@ -623,15 +622,15 @@
         """
         Cancel all overrides and set room schedule to the current temperature setting for the mode
         return: boolean
         """
         return await self._send_command({"RequestOverride": {"Type": "None"}})
 
 
-class _WiserRoomCollection(_WiserRoomAutomations):
+class _WiserRoomCollection:
     """Class holding all wiser room objects"""
 
     def __init__(
         self,
         wiser_rest_controller: _WiserRestController,
         room_data: dict,
         schedules: _WiserScheduleCollection,
```

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/roomstat.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/roomstat.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/schedule.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/shutter.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/shutter.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartplug.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartplug.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartvalve.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/smartvalve.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/system.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/system.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/ufh.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/ufh.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/wiserhub.py` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI/wiserhub.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # TODO: Update entity values after commend issued to get current values
 import asyncio
 from dataclasses import dataclass
 import aiohttp
 import pathlib
 from typing import Optional
 
+from .helpers.automations import _WiserHeatingChannelAutomations
+
 
 from . import _LOGGER, __VERSION__
 
 from .const import (
     DEFAULT_AWAY_MODE_TEMP,
     DEFAULT_DEGRADED_TEMP,
     MAX_BOOST_INCREASE,
@@ -126,15 +128,18 @@
             )
 
     async def read_hub_data(self):
         await self._build_objects()
 
         # Run automations
         if self._enable_automations:
-            if await self._rooms.run_automations():
+            automations = _WiserHeatingChannelAutomations(
+                self._wiser_rest_controller, self.heating_channels
+            )
+            if await automations.run_automations():
                 await self._build_objects()
 
     async def _build_objects(self):
         """Read all data from hub and populate objects"""
 
         # Read data from hub
         self._domain_data = await self._wiser_rest_controller._get_hub_data(
```

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/PKG-INFO` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.3.2
+Version: 1.3.3
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Drayton Wiser Hub API Async v1.3.2
+# Drayton Wiser Hub API Async v1.3.3
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -64,14 +64,18 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.3
+
+* Fixed issue in passive mode so that it works with 3 channel hub and different rooms on different channels
+
 ### v1.3.2
 
 * Fixed issue ot maintaining some parameters after hub update
 * Improved handling of extra config json errors
 * Amended current_target_temp to use DisplayedSetPoint instead of CurrentSetPoint as this displays incorrectly in Eco mode
 
 ### 1.3.1
```

### Comparing `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/SOURCES.txt` & `aioWiserHeatAPI-1.3.3/aioWiserHeatAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.2/setup.py` & `aioWiserHeatAPI-1.3.3/setup.py`

 * *Files identical despite different names*

