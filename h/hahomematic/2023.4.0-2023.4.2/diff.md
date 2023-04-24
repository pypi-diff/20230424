# Comparing `tmp/hahomematic-2023.4.0.tar.gz` & `tmp/hahomematic-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.4.0.tar", last modified: Sun Apr 16 10:20:03 2023, max compression
+gzip compressed data, was "hahomematic-2023.4.2.tar", last modified: Mon Apr 24 18:05:07 2023, max compression
```

## Comparing `hahomematic-2023.4.0.tar` & `hahomematic-2023.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.098901 hahomematic-2023.4.0/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.098901 hahomematic-2023.4.0/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-16 10:20:03.000000 hahomematic-2023.4.0/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:20:01.000000 hahomematic-2023.4.0/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:05:07.331697 hahomematic-2023.4.2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-24 18:05:06.000000 hahomematic-2023.4.2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-24 18:05:07.000000 hahomematic-2023.4.2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:05:06.000000 hahomematic-2023.4.2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:05:05.000000 hahomematic-2023.4.2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-24 18:05:07.000000 hahomematic-2023.4.2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 18:05:07.000000 hahomematic-2023.4.2/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-24 18:04:28.000000 hahomematic-2023.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 18:05:07.335697 hahomematic-2023.4.2/setup.cfg
```

### Comparing `hahomematic-2023.4.0/LICENSE` & `hahomematic-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/PKG-INFO` & `hahomematic-2023.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.0
+Version: 2023.4.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.0/README.md` & `hahomematic-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/__init__.py` & `hahomematic-2023.4.2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/backport.py` & `hahomematic-2023.4.2/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/caches/dynamic.py` & `hahomematic-2023.4.2/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/caches/persistent.py` & `hahomematic-2023.4.2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/caches/visibility.py` & `hahomematic-2023.4.2/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/central_unit.py` & `hahomematic-2023.4.2/hahomematic/central_unit.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/client.py` & `hahomematic-2023.4.2/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/const.py` & `hahomematic-2023.4.2/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/decorators.py` & `hahomematic-2023.4.2/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/exceptions.py` & `hahomematic-2023.4.2/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/exporter.py` & `hahomematic-2023.4.2/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/hmcli.py` & `hahomematic-2023.4.2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/json_rpc_client.py` & `hahomematic-2023.4.2/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/__init__.py` & `hahomematic-2023.4.2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/const.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/cover.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         level: float | None = None,
         tilt_level: float | None = None,
         collector: CallParameterCollector | None = None,
     ) -> None:
         """Move the cover to a specific tilt level. Value range is 0.0 to 1.0."""
         _level = level if level is not None else self.current_position / 100.0
         _tilt_level = tilt_level if tilt_level is not None else self.current_tilt_position / 100.0
-        if self._e_combined and (
+        if self._e_combined.is_hmtype and (
             combined_parameter := self._get_combined_value(level=_level, tilt_level=_tilt_level)
         ):
             await self._e_combined.send_value(value=combined_parameter, collector=collector)
             return
 
         await self._e_level_2.send_value(value=_tilt_level, collector=collector)
         await super()._set_level(level=_level, collector=collector)
```

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Final, TypeVar, cast
 
 from hahomematic.const import INIT_DATETIME, MAX_CACHE_AGE, HmCallSource, HmEntityUsage
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import HmEntityDefinition
 from hahomematic.platforms.custom.support import ExtendedConfig
-from hahomematic.platforms.entity import BaseEntity
+from hahomematic.platforms.entity import BaseEntity, CallParameterCollector
 from hahomematic.platforms.generic import entity as hmge
 from hahomematic.platforms.support import (
     EntityNameData,
     check_channel_is_the_only_primary_channel,
     get_custom_entity_name,
     value_property,
 )
@@ -272,11 +272,16 @@
     max: Any = None
     min: Any = None
     unit: Any = None
     value: Any = None
     value_list: list[Any] = []
     visible: Any = None
     channel_operation_mode: str | None = None
+    is_hmtype = False
 
-    def send_value(self, value: Any) -> bool:
+    async def send_value(
+        self,
+        value: Any,
+        collector: CallParameterCollector | None = None,
+        do_validate: bool = True,
+    ) -> None:
         """Send value dummy method."""
-        return True  # pragma: no cover
```

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/light.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/support.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.4.2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/device.py` & `hahomematic-2023.4.2/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/entity.py` & `hahomematic-2023.4.2/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/event.py` & `hahomematic-2023.4.2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/action.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/button.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 class GenericEntity(hme.BaseParameterEntity[hme.ParameterT, hme.InputParameterT]):
     """Base class for generic entities."""
 
     _attr_validate_state_change: bool = True
+    is_hmtype: Final = True
 
     def __init__(
         self,
         device: hmd.HmDevice,
         unique_identifier: str,
         channel_address: str,
         paramset_key: str,
```

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/number.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/select.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.4.2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/button.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/number.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/select.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/hub/text.py` & `hahomematic-2023.4.2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/platforms/support.py` & `hahomematic-2023.4.2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.4.2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.4.2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.4.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/support.py` & `hahomematic-2023.4.2/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.4.2/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic/xml_rpc_server.py` & `hahomematic-2023.4.2/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.4.2/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.4.0
+Version: 2023.4.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.4.0/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.4.2/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.4.0/pyproject.toml` & `hahomematic-2023.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.4.0"
+version     = "2023.4.2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

