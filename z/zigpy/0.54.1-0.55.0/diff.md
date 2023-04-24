# Comparing `tmp/zigpy-0.54.1.tar.gz` & `tmp/zigpy-0.55.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.54.1.tar", last modified: Tue Apr 11 23:16:42 2023, max compression
+gzip compressed data, was "zigpy-0.55.0.tar", last modified: Mon Apr 24 17:30:04 2023, max compression
```

## Comparing `zigpy-0.54.1.tar` & `zigpy-0.55.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 23:16:39.000000 zigpy-0.54.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-11 23:16:39.000000 zigpy-0.54.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-11 23:16:42.214049 zigpy-0.54.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 23:16:39.000000 zigpy-0.54.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-11 23:16:42.214049 zigpy-0.54.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 23:16:39.000000 zigpy-0.54.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.206049 zigpy-0.54.1/zigpy/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (123)    41314 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/quirks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (123)    33225 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25260 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    82633 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.210049 zigpy-0.54.1/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-04-11 23:16:39.000000 zigpy-0.54.1/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:16:42.206049 zigpy-0.54.1/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 23:16:42.000000 zigpy-0.54.1/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 17:30:00.000000 zigpy-0.55.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 17:30:00.000000 zigpy-0.55.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-24 17:30:04.128014 zigpy-0.55.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-24 17:30:00.000000 zigpy-0.55.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-24 17:30:04.132014 zigpy-0.55.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-24 17:30:00.000000 zigpy-0.55.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.120014 zigpy-0.55.0/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43034 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    44010 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.124014 zigpy-0.55.0/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/quirks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (123)    33587 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25260 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82633 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15491 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.128014 zigpy-0.55.0/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-04-24 17:30:00.000000 zigpy-0.55.0/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:30:04.120014 zigpy-0.55.0/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 17:30:04.000000 zigpy-0.55.0/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.54.1/COPYING` & `zigpy-0.55.0/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/LICENSE` & `zigpy-0.55.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/PKG-INFO` & `zigpy-0.55.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.54.1
+Version: 0.55.0
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.54.1/README.md` & `zigpy-0.55.0/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/setup.cfg` & `zigpy-0.55.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 error_summary = True
 disable_error_code = 
 	type-arg,
 	return-value,
 	operator,
 	valid-type,
 	misc,
-	dict-item,
 	attr-defined,
 	assignment,
 	arg-type
 follow_imports = silent
 
 [tool:pytest]
 asyncio_mode = auto
```

### Comparing `zigpy-0.54.1/setup.py` & `zigpy-0.55.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "crccheck",
     "cryptography",
     'importlib_resources; python_version<"3.9"',
     'async-timeout; python_version<"3.11"',
     "voluptuous",
     'pyserial-asyncio; platform_system!="Windows"',
     'pyserial-asyncio!=0.5; platform_system=="Windows"',
+    "typing_extensions",
 ]
 
 setup(
     name="zigpy",
     version=zigpy.__version__,
     description="Library implementing a ZigBee stack",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
```

### Comparing `zigpy-0.54.1/zigpy/appdb.py` & `zigpy-0.55.0/zigpy/appdb.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.55.0/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/application.py` & `zigpy-0.55.0/zigpy/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,20 +44,23 @@
 TRANSIENT_CONNECTION_ERRORS = {
     errno.ENETUNREACH,
 }
 
 ENERGY_SCAN_WARN_THRESHOLD = 0.75 * 255
 _R = TypeVar("_R")
 
+CHANNEL_CHANGE_BROADCAST_DELAY_S = 1.0
+CHANNEL_CHANGE_SETTINGS_RELOAD_DELAY_S = 1.0
+
 
 class ControllerApplication(zigpy.util.ListenableMixin, abc.ABC):
     SCHEMA = conf.CONFIG_SCHEMA
     SCHEMA_DEVICE = conf.SCHEMA_DEVICE
 
-    def __init__(self, config: dict):
+    def __init__(self, config: dict) -> None:
         self.devices: dict[t.EUI64, zigpy.device.Device] = {}
         self.state: zigpy.state.State = zigpy.state.State()
         self._listeners = {}
         self._config = self.SCHEMA(config)
         self._dblistener = None
         self._groups = zigpy.group.Groups(self)
         self._listeners = {}
@@ -98,15 +101,15 @@
         self._dblistener = await zigpy.appdb.PersistingListener.new(database_file, self)
         self.add_listener(self._dblistener)
         self.groups.add_listener(self._dblistener)
         self.backups.add_listener(self._dblistener)
         self.topology.add_listener(self._dblistener)
         await self._dblistener.load()
 
-    async def initialize(self, *, auto_form: bool = False):
+    async def initialize(self, *, auto_form: bool = False) -> None:
         """Starts the network on a connected radio, optionally forming one with random
         settings if necessary.
         """
 
         last_backup = self.backups.most_recent_backup()
 
         try:
@@ -179,15 +182,15 @@
 
         if self.config[conf.CONF_TOPO_SCAN_ENABLED]:
             # Config specifies the period in minutes, not seconds
             self.topology.start_periodic_scans(
                 period=(60 * self.config[zigpy.config.CONF_TOPO_SCAN_PERIOD])
             )
 
-    async def startup(self, *, auto_form: bool = False):
+    async def startup(self, *, auto_form: bool = False) -> None:
         """Starts a network, optionally forming one with random settings if necessary."""
 
         try:
             await self.connect()
             await self.initialize(auto_form=auto_form)
         except Exception as e:
             LOGGER.error("Couldn't start application", exc_info=e)
@@ -238,14 +241,72 @@
             scanned_channels = channels
             energy_values = [0] * scanned_channels
         else:
             _, scanned_channels, _, _, energy_values = rsp
 
         return dict(zip(scanned_channels, energy_values))
 
+    async def _move_network_to_channel(
+        self, new_channel: int, new_nwk_update_id: int
+    ) -> None:
+        """Broadcasts the channel migration update request."""
+        # Default implementation for radios that migrate via a loopback ZDO request
+        await self._device.zdo.Mgmt_NWK_Update_req(
+            zigpy.zdo.types.NwkUpdate(
+                ScanChannels=zigpy.types.Channels.from_channel_list([new_channel]),
+                ScanDuration=zigpy.zdo.types.NwkUpdate.CHANNEL_CHANGE_REQ,
+                nwkUpdateId=new_nwk_update_id,
+            )
+        )
+
+    async def move_network_to_channel(
+        self, new_channel: int, *, num_broadcasts: int = 5
+    ) -> None:
+        """Moves the network to a new channel."""
+        if self.state.network_info.channel == new_channel:
+            return
+
+        new_nwk_update_id = (self.state.network_info.nwk_update_id + 1) % 0xFF
+
+        for attempt in range(num_broadcasts):
+            LOGGER.info(
+                "Broadcasting migration to channel %s (%s of %s)",
+                new_channel,
+                attempt + 1,
+                num_broadcasts,
+            )
+
+            await zigpy.zdo.broadcast(
+                app=self,
+                command=zigpy.zdo.types.ZDOCmd.Mgmt_NWK_Update_req,
+                grpid=None,
+                radius=30,  # Explicitly set the maximum radius
+                broadcast_address=zigpy.types.BroadcastAddress.ALL_DEVICES,
+                NwkUpdate=zigpy.zdo.types.NwkUpdate(
+                    ScanChannels=zigpy.types.Channels.from_channel_list([new_channel]),
+                    ScanDuration=zigpy.zdo.types.NwkUpdate.CHANNEL_CHANGE_REQ,
+                    nwkUpdateId=new_nwk_update_id,
+                ),
+            )
+
+            await asyncio.sleep(CHANNEL_CHANGE_BROADCAST_DELAY_S)
+
+        # Move the coordinator itself, if supported
+        await self._move_network_to_channel(
+            new_channel=new_channel, new_nwk_update_id=new_nwk_update_id
+        )
+
+        # Wait for settings to update
+        while self.state.network_info.channel != new_channel:
+            LOGGER.info("Waiting for channel change to take effect")
+            await self.load_network_info(load_devices=False)
+            await asyncio.sleep(CHANNEL_CHANGE_SETTINGS_RELOAD_DELAY_S)
+
+        LOGGER.info("Successfully migrated to channel %d", new_channel)
+
     async def form_network(self, *, fast: bool = False) -> None:
         """Writes random network settings to the coordinator."""
 
         # First, make the settings consistent and randomly generate missing values
         channel = self.config[conf.CONF_NWK][conf.CONF_NWK_CHANNEL]
         channels = self.config[conf.CONF_NWK][conf.CONF_NWK_CHANNELS]
         pan_id = self.config[conf.CONF_NWK][conf.CONF_NWK_PAN_ID]
@@ -338,25 +399,25 @@
         self.topology.stop_periodic_scans()
 
         if self._dblistener:
             await self._dblistener.shutdown()
 
         await self.disconnect()
 
-    def add_device(self, ieee: t.EUI64, nwk: t.NWK):
+    def add_device(self, ieee: t.EUI64, nwk: t.NWK) -> zigpy.device.Device:
         """Creates a zigpy `Device` object with the provided IEEE and NWK addresses."""
 
         assert isinstance(ieee, t.EUI64)
         # TODO: Shut down existing device
 
         dev = zigpy.device.Device(self, ieee, nwk)
         self.devices[ieee] = dev
         return dev
 
-    def device_initialized(self, device):
+    def device_initialized(self, device: zigpy.device.Device) -> None:
         """Used by a device to signal that it is initialized"""
         LOGGER.debug("Device is initialized %s", device)
 
         self.listener_event("raw_device_initialized", device)
         device = zigpy.quirks.get_device(device)
         self.devices[device.ieee] = device
         if self._dblistener is not None:
@@ -629,15 +690,15 @@
     @abc.abstractmethod
     async def add_endpoint(self, descriptor: zdo_types.SimpleDescriptor):
         """Registers a new endpoint on the controlled device. Not all radios will implement
         this.
         """
         raise NotImplementedError()  # pragma: no cover
 
-    async def register_endpoints(self):
+    async def register_endpoints(self) -> None:
         """Registers all necessary endpoints.
         The exact order in which this method is called depends on the radio module.
         """
 
         await self.add_endpoint(
             zdo_types.SimpleDescriptor(
                 endpoint=1,
@@ -722,15 +783,15 @@
         dst_ep: t.uint8_t,
         sequence: t.uint8_t,
         data: bytes,
         *,
         expect_reply: bool = True,
         use_ieee: bool = False,
         extended_timeout: bool = False,
-    ):
+    ) -> tuple[zigpy.zcl.foundation.Status, str]:
         """Submit and send data out as an unicast transmission.
         :param device: destination device
         :param profile: Zigbee Profile ID to use for outgoing message
         :param cluster: cluster id where the message is being sent
         :param src_ep: source endpoint id
         :param dst_ep: destination endpoint id
         :param sequence: transaction sequence number of the message
@@ -831,15 +892,15 @@
         src_ep: t.uint8_t,
         dst_ep: t.uint8_t,
         grpid: t.uint16_t,
         radius: int,
         sequence: t.uint8_t,
         data: bytes,
         broadcast_address: t.BroadcastAddress = t.BroadcastAddress.RX_ON_WHEN_IDLE,
-    ):
+    ) -> tuple[zigpy.zcl.foundation.Status, str]:
         """Submit and send data out as an unicast transmission.
         :param profile: Zigbee Profile ID to use for outgoing message
         :param cluster: cluster id where the message is being sent
         :param src_ep: source endpoint id
         :param dst_ep: destination endpoint id
         :param: grpid: group id to address the broadcast to
         :param radius: max radius of the broadcast
@@ -1011,15 +1072,15 @@
 
         try:
             yield listener.future
         finally:
             self._req_listeners[src].remove(listener)
 
     @abc.abstractmethod
-    async def permit_ncp(self, time_s: int = 60):
+    async def permit_ncp(self, time_s: int = 60) -> None:
         """Permit joining on NCP.
         Not all radios will require this method.
         """
         raise NotImplementedError()  # pragma: no cover
 
     @abc.abstractmethod
     async def permit_with_key(self, node: t.EUI64, code: bytes, time_s: int = 60):
@@ -1050,15 +1111,15 @@
 
     @abc.abstractmethod
     async def reset_network_info(self) -> None:
         """Leaves the current network."""
 
         raise NotImplementedError()  # pragma: no cover
 
-    async def permit(self, time_s: int = 60, node: t.EUI64 | str | None = None):
+    async def permit(self, time_s: int = 60, node: t.EUI64 | str | None = None) -> None:
         """Permit joining on a specific node or all router nodes."""
         assert 0 <= time_s <= 254
         if node is not None:
             if not isinstance(node, t.EUI64):
                 node = t.EUI64([t.uint8_t(p) for p in node])
             if node != self.state.node_info.ieee:
                 try:
@@ -1078,15 +1139,15 @@
             zdo_types.ZDOCmd.Mgmt_Permit_Joining_req,  # command
             0x0000,  # grpid
             0x00,  # radius
             time_s,
             0,
             broadcast_address=t.BroadcastAddress.ALL_ROUTERS_AND_COORDINATOR,
         )
-        return await self.permit_ncp(time_s)
+        await self.permit_ncp(time_s)
 
     def get_sequence(self) -> t.uint8_t:
         self._send_sequence = (self._send_sequence + 1) % 256
         return self._send_sequence
 
     def get_device(
         self, ieee: t.EUI64 = None, nwk: t.NWK | int = None
@@ -1111,15 +1172,15 @@
 
         raise KeyError(f"Device not found: nwk={nwk!r}, ieee={ieee!r}")
 
     def get_endpoint_id(self, cluster_id: int, is_server_cluster: bool = False) -> int:
         """Returns coordinator endpoint id for specified cluster id."""
         return DEFAULT_ENDPOINT_ID
 
-    def get_dst_address(self, cluster) -> zdo_types.MultiAddress:
+    def get_dst_address(self, cluster: zigpy.zcl.Cluster) -> zdo_types.MultiAddress:
         """Helper to get a dst address for bind/unbind operations.
 
         Allows radios to provide correct information especially for radios which listen
         on specific endpoints only.
         :param cluster: cluster instance to be bound to coordinator
         :returns: returns a "destination address"
         """
@@ -1140,18 +1201,18 @@
 
     @config.setter
     def config(self, new_config) -> None:
         """Configuration setter."""
         self._config = self.SCHEMA(new_config)
 
     @property
-    def groups(self):
+    def groups(self) -> zigpy.group.Groups:
         return self._groups
 
     @property
-    def ota(self):
+    def ota(self) -> zigpy.ota.OTA:
         return self._ota
 
     @property
     def _device(self):
         """The device being controlled."""
         return self.get_device(ieee=self.state.node_info.ieee)
```

### Comparing `zigpy-0.54.1/zigpy/backups.py` & `zigpy-0.55.0/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/config/__init__.py` & `zigpy-0.55.0/zigpy/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Config schemas and validation."""
 
+from __future__ import annotations
+
 import voluptuous as vol
 
 from zigpy.config.defaults import (
     CONF_MAX_CONCURRENT_REQUESTS_DEFAULT,
     CONF_NWK_BACKUP_ENABLED_DEFAULT,
     CONF_NWK_BACKUP_PERIOD_DEFAULT,
     CONF_NWK_CHANNEL_DEFAULT,
```

### Comparing `zigpy-0.54.1/zigpy/config/defaults.py` & `zigpy-0.55.0/zigpy/config/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import zigpy.types as t
 
 CONF_STARTUP_ENERGY_SCAN_DEFAULT = True
 CONF_MAX_CONCURRENT_REQUESTS_DEFAULT = 8
 CONF_NWK_BACKUP_ENABLED_DEFAULT = True
 CONF_NWK_BACKUP_PERIOD_DEFAULT = 24 * 60  # 24 hours
 CONF_NWK_CHANNEL_DEFAULT = None
```

### Comparing `zigpy-0.54.1/zigpy/config/validators.py` & `zigpy-0.55.0/zigpy/config/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/const.py` & `zigpy-0.55.0/zigpy/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 """Zigpy Constants."""
 
 SIG_ENDPOINTS = "endpoints"
 SIG_EP_INPUT = "input_clusters"
 SIG_EP_OUTPUT = "output_clusters"
 SIG_EP_PROFILE = "profile_id"
 SIG_EP_TYPE = "device_type"
```

### Comparing `zigpy-0.54.1/zigpy/device.py` & `zigpy-0.55.0/zigpy/device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/endpoint.py` & `zigpy-0.55.0/zigpy/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import asyncio
 import enum
 import logging
 from typing import Any
 
 import zigpy.exceptions
 import zigpy.profiles
-from zigpy.types.named import EUI64
+import zigpy.types as t
 from zigpy.typing import AddressingMode, DeviceType
 import zigpy.util
 import zigpy.zcl
-from zigpy.zcl.clusters.general import Basic
-from zigpy.zcl.foundation import Status as ZCLStatus, ZCLHeader
-from zigpy.zdo.types import Status as zdo_status
+from zigpy.zcl.foundation import (
+    CommandSchema,
+    GeneralCommand,
+    Status as ZCLStatus,
+    ZCLHeader,
+)
+from zigpy.zdo.types import Status as ZDOStatus
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Status(enum.IntEnum):
     """The status of an Endpoint"""
 
@@ -28,15 +32,15 @@
     # Endpoint Inactive
     ENDPOINT_INACTIVE = 3
 
 
 class Endpoint(zigpy.util.LocalLogMixin, zigpy.util.ListenableMixin):
     """An endpoint on a device on the network"""
 
-    def __init__(self, device: DeviceType, endpoint_id: int):
+    def __init__(self, device: DeviceType, endpoint_id: int) -> None:
         self._device: DeviceType = device
         self._endpoint_id: int = endpoint_id
         self._listeners: dict = {}
 
         self.status: Status = Status.NEW
         self.profile_id: int | None = None
         self.device_type: zigpy.profiles.zha.DeviceType | None = None
@@ -55,19 +59,19 @@
         if self.profile_id is not None or self.status == Status.ENDPOINT_INACTIVE:
             self.info("Endpoint descriptor already queried")
         else:
             status, _, sd = await self._device.zdo.Simple_Desc_req(
                 self._device.nwk, self._endpoint_id, tries=3, delay=2
             )
 
-            if status == zdo_status.NOT_ACTIVE:
+            if status == ZDOStatus.NOT_ACTIVE:
                 # These endpoints are essentially junk but this lets the device join
                 self.status = Status.ENDPOINT_INACTIVE
                 return
-            elif status != zdo_status.SUCCESS:
+            elif status != ZDOStatus.SUCCESS:
                 raise zigpy.exceptions.InvalidResponse(
                     "Failed to retrieve service descriptor: %s", status
                 )
 
             self.info("Discovered endpoint information: %s", sd)
             self.profile_id = sd.profile
             self.device_type = sd.device_type
@@ -167,15 +171,15 @@
             self.debug("Failed to sync-up group membership")
             return
 
         groups = set(res[1])
         self.device.application.groups.update_group_membership(self, groups)
 
     async def get_model_info(self) -> tuple[str | None, str | None]:
-        if Basic.cluster_id not in self.in_clusters:
+        if zigpy.zcl.clusters.general.Basic.cluster_id not in self.in_clusters:
             return None, None
 
         # Some devices can't handle multiple attributes in the same read request
         for names in (["manufacturer", "model"], ["manufacturer"], ["model"]):
             try:
                 success, failure = await self.basic.read_attributes(
                     names, allow_cache=True
@@ -191,15 +195,17 @@
                 self._model = success["model"]
 
             if "manufacturer" in success:
                 self._manufacturer = success["manufacturer"]
 
         return self._model, self._manufacturer
 
-    def deserialize(self, cluster_id, data):
+    def deserialize(
+        self, cluster_id: t.ClusterId, data: bytes
+    ) -> tuple[ZCLHeader, CommandSchema]:
         """Deserialize data for ZCL"""
         if cluster_id not in self.in_clusters and cluster_id not in self.out_clusters:
             raise KeyError(f"No cluster ID 0x{cluster_id:04x} on {self.unique_id}")
 
         cluster = self.in_clusters.get(cluster_id, self.out_clusters.get(cluster_id))
         return cluster.deserialize(data)
 
@@ -220,15 +226,20 @@
             self.debug("Message on unknown cluster 0x%04x", cluster)
             self.listener_event("unknown_cluster_message", hdr.command_id, args)
             return
 
         handler(hdr, args, dst_addressing=dst_addressing)
 
     async def request(
-        self, cluster, sequence, data, expect_reply=True, command_id=0x00
+        self,
+        cluster: t.ClusterId,
+        sequence: t.uint8_t,
+        data: bytes,
+        expect_reply: bool = True,
+        command_id: GeneralCommand | t.uint8_t = 0x00,
     ):
         if self.profile_id == zigpy.profiles.zll.PROFILE_ID and not (
             cluster == zigpy.zcl.clusters.lightlink.LightLink.cluster_id
             and command_id < 0x40
         ):
             profile_id = zigpy.profiles.zha.PROFILE_ID
         else:
@@ -240,15 +251,21 @@
             self._endpoint_id,
             self._endpoint_id,
             sequence,
             data,
             expect_reply=expect_reply,
         )
 
-    async def reply(self, cluster, sequence, data, command_id=0x00):
+    async def reply(
+        self,
+        cluster: t.ClusterId,
+        sequence: t.uint8_t,
+        data: bytes,
+        command_id: GeneralCommand | t.uint8_t = 0x00,
+    ) -> None:
         if self.profile_id == zigpy.profiles.zll.PROFILE_ID and not (
             cluster == zigpy.zcl.clusters.lightlink.LightLink.cluster_id
             and command_id < 0x40
         ):
             profile_id = zigpy.profiles.zha.PROFILE_ID
         else:
             profile_id = self.profile_id
@@ -304,18 +321,18 @@
         self.warning(
             "Overriding model from quirks is not supported and "
             "will be removed in the next version"
         )
         self._model = value
 
     @property
-    def unique_id(self) -> tuple[EUI64, int]:
+    def unique_id(self) -> tuple[t.EUI64, int]:
         return self.device.ieee, self.endpoint_id
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> zigpy.zcl.Cluster:
         try:
             return self._cluster_attr[name]
         except KeyError:
             raise AttributeError
 
     def __repr__(self) -> str:
         def cluster_repr(clusters):
```

### Comparing `zigpy-0.54.1/zigpy/exceptions.py` & `zigpy-0.55.0/zigpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/group.py` & `zigpy-0.55.0/zigpy/group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/listeners.py` & `zigpy-0.55.0/zigpy/listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/ota/__init__.py` & `zigpy-0.55.0/zigpy/ota/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """OTA support for Zigbee devices."""
+from __future__ import annotations
+
 import datetime
 import logging
-from typing import Optional
 
 import attr
 
 from zigpy.config import (
     CONF_OTA,
     CONF_OTA_DIR,
     CONF_OTA_IKEA,
@@ -34,15 +35,15 @@
     DEFAULT_EXPIRATION = datetime.timedelta(hours=18)
 
     image = attr.ib(default=None)
     expires_on = attr.ib(default=None)
     cached_data = attr.ib(default=None)
 
     @classmethod
-    def new(cls, img: BaseOTAImage) -> "CachedImage":
+    def new(cls, img: BaseOTAImage) -> CachedImage:
         expiration = datetime.datetime.now() + cls.DEFAULT_EXPIRATION
         return cls(img, expiration)
 
     @property
     def expired(self) -> bool:
         if self.expires_on is None:
             return False
@@ -56,15 +57,21 @@
     def header(self) -> OTAImageHeader:
         return self.image.header
 
     @property
     def version(self) -> int:
         return self.image.header.file_version
 
-    def should_update(self, manufacturer_id, img_type, ver, hw_ver=None) -> bool:
+    def should_update(
+        self,
+        manufacturer_id: t.uint16_t,
+        img_type: t.uint16_t,
+        ver: t.uint32_t,
+        hw_ver: None = None,
+    ) -> bool:
         """Check if it should upgrade"""
 
         if self.key != ImageKey(manufacturer_id, img_type):
             return False
 
         if ver >= self.version:
             return False
@@ -78,15 +85,15 @@
                 <= self.image.header.maximum_hardware_version
             )
         ):
             return False
 
         return True
 
-    def get_image_block(self, offset: t.uint32_t, size: t.uint8_t) -> bytes:
+    def get_image_block(self, offset: t.t.uint32_t, size: t.uint8_t) -> bytes:
         if (
             self.expires_on is not None
             and self.expires_on - datetime.datetime.now() < DELAY_EXPIRATION
         ):
             self.expires_on += DELAY_EXPIRATION
 
         if self.cached_data is None:
@@ -97,15 +104,15 @@
 
         return self.cached_data[offset : offset + min(self.MAXIMUM_DATA_SIZE, size)]
 
 
 class OTA(zigpy.util.ListenableMixin):
     """OTA Manager."""
 
-    def __init__(self, app: ControllerApplicationType, *args, **kwargs):
+    def __init__(self, app: ControllerApplicationType, *args, **kwargs) -> None:
         self._app: ControllerApplicationType = app
         self._image_cache: dict[ImageKey, CachedImage] = {}
         self._not_initialized = True
         self._listeners = {}
         ota_config = app.config[CONF_OTA]
         if ota_config[CONF_OTA_DIR]:
             self.add_listener(zigpy.ota.provider.FileStore())
@@ -123,16 +130,19 @@
             self.add_listener(zigpy.ota.provider.ThirdReality())
 
     async def initialize(self) -> None:
         await self.async_event("initialize_provider", self._app.config[CONF_OTA])
         self._not_initialized = False
 
     async def get_ota_image(
-        self, manufacturer_id, image_type, model=None
-    ) -> Optional[CachedImage]:
+        self,
+        manufacturer_id: t.uint16_t,
+        image_type: t.uint16_t,
+        model: str | None = None,
+    ) -> CachedImage | None:
         if manufacturer_id in (
             zigpy.ota.provider.Salus.MANUFACTURER_ID,
         ):  # Salus/computime do not pass a useful image_type
             # in the message from the device. So construct key based on model name.
             key = ImageKey(manufacturer_id, model)
         else:
             key = ImageKey(manufacturer_id, image_type)
```

### Comparing `zigpy-0.54.1/zigpy/ota/image.py` & `zigpy-0.55.0/zigpy/ota/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,21 @@
         )
 
 
 class HeaderString(str):
     _size = 32
 
     @classmethod
-    def deserialize(cls, data):
+    def deserialize(cls, data: bytes) -> tuple[HeaderString, bytes]:
         if len(data) < cls._size:
             raise ValueError(f"Data is too short. Should be at least {cls._size}")
         raw = data[: cls._size].split(b"\x00")[0]
         return cls(raw.decode("utf8", errors="replace")), data[cls._size :]
 
-    def serialize(self):
+    def serialize(self) -> bytes:
         return self.encode("utf8").ljust(self._size, b"\x00")
 
 
 class FieldControl(t.bitmap16):
     SECURITY_CREDENTIAL_VERSION_PRESENT = 0b001
     DEVICE_SPECIFIC_FILE_PRESENT = 0b010
     HARDWARE_VERSIONS_PRESENT = 0b100
@@ -98,19 +98,19 @@
     @property
     def hardware_versions_present(self) -> bool:
         if self.field_control is None:
             return None
         return bool(self.field_control & FieldControl.HARDWARE_VERSIONS_PRESENT)
 
     @property
-    def key(self):
+    def key(self) -> ImageKey:
         return ImageKey(self.manufacturer_id, self.image_type)
 
     @classmethod
-    def deserialize(cls, data) -> tuple[OTAImageHeader, bytes]:
+    def deserialize(cls, data: bytes) -> tuple[OTAImageHeader, bytes]:
         hdr, data = super().deserialize(data)
         if hdr.upgrade_file_id != cls.MAGIC_VALUE:
             raise ValueError(
                 f"Wrong magic number for OTA Image: {hdr.upgrade_file_id!r}"
             )
 
         return hdr, data
@@ -154,15 +154,15 @@
 class OTAImage(t.Struct, BaseOTAImage):
     """Zigbee OTA image according to 11.4 of the ZCL specification."""
 
     header: OTAImageHeader
     subelements: t.List[SubElement]
 
     @classmethod
-    def deserialize(cls, data) -> tuple[OTAImage, bytes]:
+    def deserialize(cls, data: bytes) -> tuple[OTAImage, bytes]:
         hdr, data = OTAImageHeader.deserialize(data)
         elements_len = hdr.image_size - hdr.header_length
 
         if elements_len > len(data):
             raise ValueError(f"Data is too short for {cls}")
 
         image = cls(header=hdr, subelements=[])
@@ -170,15 +170,15 @@
 
         while element_data:
             element, element_data = SubElement.deserialize(element_data)
             image.subelements.append(element)
 
         return image, data
 
-    def serialize(self):
+    def serialize(self) -> bytes:
         res = super().serialize()
         assert len(res) == self.header.image_size
 
         return res
 
 
 @attr.s
@@ -192,15 +192,15 @@
     header = attr.ib(default=None)
     data = attr.ib(default=None)
 
     def serialize(self) -> bytes:
         return self.header.serialize() + self.data
 
     @classmethod
-    def deserialize(cls, data) -> tuple[HueSBLOTAImage, bytes]:
+    def deserialize(cls, data: bytes) -> tuple[HueSBLOTAImage, bytes]:
         header, remaining_data = OTAImageHeader.deserialize(data)
         firmware = remaining_data[: header.image_size - len(header.serialize())]
 
         if len(data) < header.image_size:
             raise ValueError(
                 f"Data is too short to contain image: {len(data)} < {header.image_size}"
             )
```

### Comparing `zigpy-0.54.1/zigpy/ota/provider.py` & `zigpy-0.55.0/zigpy/ota/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
 
 class Basic(zigpy.util.LocalLogMixin, ABC):
     """Skeleton OTA Firmware provider."""
 
     REFRESH = datetime.timedelta(hours=12)
 
-    def __init__(self):
-        self.config = {}
-        self._cache = {}
+    def __init__(self) -> None:
+        self.config: dict[str, str | int] = {}
+        self._cache: dict[ImageKey, BaseOTAImage] = {}
         self._is_enabled = False
-        self._locks = defaultdict(asyncio.Semaphore)
+        self._locks: defaultdict[asyncio.Semaphore] = defaultdict(asyncio.Semaphore)
         self._last_refresh = None
 
     @abstractmethod
     async def initialize_provider(self, ota_config: dict) -> None:
         """Initialize OTA provider."""
 
     @abstractmethod
@@ -73,54 +73,54 @@
 
     def disable(self) -> None:
         self._is_enabled = False
 
     def enable(self) -> None:
         self._is_enabled = True
 
-    def update_expiration(self):
+    def update_expiration(self) -> None:
         self._last_refresh = datetime.datetime.now()
 
     @property
     def is_enabled(self) -> bool:
         return self._is_enabled
 
     @property
     def expired(self) -> bool:
         """Return True if firmware list needs refreshing."""
         if self._last_refresh is None:
             return True
 
         return datetime.datetime.now() - self._last_refresh > self.REFRESH
 
-    def log(self, lvl, msg, *args, **kwargs):
+    def log(self, lvl: int, msg: str, *args, **kwargs) -> None:
         """Log a message"""
         msg = f"{self.__class__.__name__}: {msg}"
         return LOGGER.log(lvl, msg, *args, **kwargs)
 
 
 @attr.s
 class IKEAImage:
     manufacturer_id = attr.ib()
     image_type = attr.ib()
     version = attr.ib(default=None)
     image_size = attr.ib(default=None)
     url = attr.ib(default=None)
 
     @classmethod
-    def new(cls, data):
+    def new(cls, data: dict[str, str | int]) -> IKEAImage:
         res = cls(data["fw_manufacturer_id"], data["fw_image_type"])
         res.file_version = data["fw_file_version_MSB"] << 16
         res.file_version |= data["fw_file_version_LSB"]
         res.image_size = data["fw_filesize"]
         res.url = data["fw_binary_url"]
         return res
 
     @property
-    def key(self):
+    def key(self) -> ImageKey:
         return ImageKey(self.manufacturer_id, self.image_type)
 
     async def fetch_image(self) -> BaseOTAImage | None:
         async with aiohttp.ClientSession() as req:
             LOGGER.debug("Downloading %s for %s", self.url, self.key)
             async with req.get(self.url) as rsp:
                 data = await rsp.read()
@@ -545,15 +545,15 @@
                 return img
         except (OSError, ValueError):
             LOGGER.debug("Couldn't load '%s' OTA image", self.file_name, exc_info=True)
         return None
 
 
 class FileStore(Basic):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self._ota_dir = None
 
     @staticmethod
     def validate_ota_dir(ota_dir: str) -> str | None:
         """Return True if exists and is a dir."""
         if ota_dir is None:
@@ -623,30 +623,30 @@
 class INOVELLIImage:
     manufacturer_id = attr.ib()
     image_type = attr.ib()
     version = attr.ib()
     url = attr.ib()
 
     @classmethod
-    def from_json(cls, obj):
+    def from_json(cls, obj: dict[str, str | int]) -> INOVELLIImage:
         version = int(obj["version"], 16)
 
         # Old Inovelli OTA JSON versions were in hex, they then switched back to decimal
         if version > 0x10:
             version = int(obj["version"])
 
         return cls(
             manufacturer_id=obj["manufacturer_id"],
             image_type=obj["image_type"],
             version=version,
             url=obj["firmware"],
         )
 
     @property
-    def key(self):
+    def key(self) -> ImageKey:
         return ImageKey(self.manufacturer_id, self.image_type)
 
     async def fetch_image(self) -> BaseOTAImage | None:
         async with aiohttp.ClientSession() as req:
             LOGGER.debug("Downloading %s for %s", self.url, self.key)
             async with req.get(self.url) as rsp:
                 data = await rsp.read()
```

### Comparing `zigpy-0.54.1/zigpy/ota/validators.py` & `zigpy-0.55.0/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/profiles/zha.py` & `zigpy-0.55.0/zigpy/profiles/zha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import zigpy.types as t
 
 PROFILE_ID = 260
 
 
 class DeviceType(t.enum16):
     # Generic
```

### Comparing `zigpy-0.54.1/zigpy/profiles/zll.py` & `zigpy-0.55.0/zigpy/profiles/zll.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import zigpy.types as t
 
 PROFILE_ID = 49246
 
 
 class DeviceType(t.enum16):
     ON_OFF_LIGHT = 0x0000
```

### Comparing `zigpy-0.54.1/zigpy/quirks/__init__.py` & `zigpy-0.55.0/zigpy/quirks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import Any, Callable, Coroutine, Iterable
+import typing
 
 from zigpy.const import (  # noqa: F401
     SIG_ENDPOINTS,
     SIG_EP_INPUT,
     SIG_EP_OUTPUT,
     SIG_EP_PROFILE,
     SIG_EP_TYPE,
@@ -15,24 +15,30 @@
     SIG_NODE_DESC,
     SIG_SKIP_CONFIG,
 )
 import zigpy.device
 import zigpy.endpoint
 from zigpy.quirks.registry import DeviceRegistry  # noqa: F401
 import zigpy.types as t
+from zigpy.types.basic import uint16_t
 import zigpy.zcl
 import zigpy.zcl.foundation as foundation
 
+if typing.TYPE_CHECKING:
+    from zigpy.application import ControllerApplication
+
 _LOGGER = logging.getLogger(__name__)
 
 _DEVICE_REGISTRY = DeviceRegistry()
 _uninitialized_device_message_handlers = []
 
 
-def get_device(device: zigpy.device.Device, registry: DeviceRegistry | None = None):
+def get_device(
+    device: zigpy.device.Device, registry: DeviceRegistry | None = None
+) -> zigpy.device.Device:
     """Get a CustomDevice object, if one is available"""
     if registry is None:
         return _DEVICE_REGISTRY.get_device(device)
 
     return registry.get_device(device)
 
 
@@ -42,33 +48,39 @@
     """Get the Quirk list for a given manufacturer and model."""
     if registry is None:
         return _DEVICE_REGISTRY.registry[manufacturer][model]
 
     return registry.registry[manufacturer][model]
 
 
-def register_uninitialized_device_message_handler(handler: Callable) -> None:
+def register_uninitialized_device_message_handler(handler: typing.Callable) -> None:
     """Register an handler for messages received by uninitialized devices.
 
     each handler is passed same parameters as
     zigpy.application.ControllerApplication.handle_message
     """
     if handler not in _uninitialized_device_message_handlers:
         _uninitialized_device_message_handlers.append(handler)
 
 
 class CustomDevice(zigpy.device.Device):
-    replacement: dict[str, Any] = {}
+    replacement: dict[str, typing.Any] = {}
     signature = None
 
-    def __init_subclass__(cls):
+    def __init_subclass__(cls) -> None:
         if getattr(cls, "signature", None) is not None:
             _DEVICE_REGISTRY.add_to_registry(cls)
 
-    def __init__(self, application, ieee, nwk, replaces):
+    def __init__(
+        self,
+        application: ControllerApplication,
+        ieee: t.EUI64,
+        nwk: t.NWK,
+        replaces: zigpy.device.Device,
+    ) -> None:
         super().__init__(application, ieee, nwk)
 
         def set_device_attr(attr):
             if attr in self.replacement:
                 setattr(self, attr, self.replacement[attr])
             else:
                 setattr(self, attr, getattr(replaces, attr))
@@ -80,15 +92,17 @@
         set_device_attr(SIG_NODE_DESC)
         set_device_attr(SIG_MANUFACTURER)
         set_device_attr(SIG_MODEL)
         set_device_attr(SIG_SKIP_CONFIG)
         for endpoint_id, endpoint in self.replacement.get(SIG_ENDPOINTS, {}).items():
             self.add_endpoint(endpoint_id, replace_device=replaces)
 
-    def add_endpoint(self, endpoint_id, replace_device=None) -> zigpy.endpoint.Endpoint:
+    def add_endpoint(
+        self, endpoint_id: int, replace_device: zigpy.device.Device | None = None
+    ) -> zigpy.endpoint.Endpoint:
         if endpoint_id not in self.replacement.get(SIG_ENDPOINTS, {}):
             return super().add_endpoint(endpoint_id)
 
         endpoints = self.replacement[SIG_ENDPOINTS]
 
         if isinstance(endpoints[endpoint_id], tuple):
             custom_ep_type = endpoints[endpoint_id][0]
@@ -99,15 +113,21 @@
 
         ep = custom_ep_type(self, endpoint_id, replacement_data, replace_device)
         self.endpoints[endpoint_id] = ep
         return ep
 
 
 class CustomEndpoint(zigpy.endpoint.Endpoint):
-    def __init__(self, device, endpoint_id, replacement_data, replace_device):
+    def __init__(
+        self,
+        device: CustomDevice,
+        endpoint_id: int,
+        replacement_data: dict[str, typing.Any],
+        replace_device: zigpy.device.Device,
+    ) -> None:
         super().__init__(device, endpoint_id)
 
         def set_device_attr(attr):
             if attr in replacement_data:
                 setattr(self, attr, replacement_data[attr])
             else:
                 setattr(self, attr, getattr(replace_device[endpoint_id], attr))
@@ -133,24 +153,24 @@
                 cluster = c(self, is_server=False)
                 cluster_id = cluster.cluster_id
             self.add_output_cluster(cluster_id, cluster)
 
 
 class CustomCluster(zigpy.zcl.Cluster):
     _skip_registry = True
-    _CONSTANT_ATTRIBUTES: dict[int, Any] | None = None
+    _CONSTANT_ATTRIBUTES: dict[int, typing.Any] | None = None
 
     manufacturer_id_override: t.uint16_t | None = None
 
     @property
     def _is_manuf_specific(self) -> bool:
         """Return True if cluster_id is within manufacturer specific range."""
         return 0xFC00 <= self.cluster_id <= 0xFFFF
 
-    def _has_manuf_attr(self, attrs_to_process: Iterable | list | dict) -> bool:
+    def _has_manuf_attr(self, attrs_to_process: typing.Iterable | list | dict) -> bool:
         """Return True if contains a manufacturer specific attribute."""
         if self._is_manuf_specific:
             return True
 
         for attr_id in attrs_to_process:
             if (
                 attr_id in self.attributes
@@ -164,16 +184,16 @@
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         *args,
         manufacturer: int | t.uint16_t | None = None,
         expect_reply: bool = True,
         tries: int = 1,
         tsn: int | t.uint8_t | None = None,
-        **kwargs: Any,
-    ) -> Coroutine:
+        **kwargs: typing.Any,
+    ) -> typing.Coroutine:
         command = self.server_commands[command_id]
 
         if manufacturer is None and (
             self._is_manuf_specific or command.is_manufacturer_specific
         ):
             manufacturer = self.endpoint.manufacturer_id
 
@@ -191,16 +211,16 @@
 
     async def client_command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         *args,
         manufacturer: int | t.uint16_t | None = None,
         tsn: int | t.uint8_t | None = None,
-        **kwargs: Any,
-    ) -> Coroutine:
+        **kwargs: typing.Any,
+    ):
         command = self.client_commands[command_id]
 
         if manufacturer is None and (
             self._is_manuf_specific or command.is_manufacturer_specific
         ):
             manufacturer = self.endpoint.manufacturer_id
 
@@ -210,15 +230,17 @@
             command.schema,
             *args,
             manufacturer=manufacturer,
             tsn=tsn,
             **kwargs,
         )
 
-    async def read_attributes_raw(self, attributes, manufacturer=None):
+    async def read_attributes_raw(
+        self, attributes: list[uint16_t], manufacturer: uint16_t | None = None
+    ):
         if not self._CONSTANT_ATTRIBUTES:
             return await super().read_attributes_raw(
                 attributes, manufacturer=manufacturer
             )
 
         succeeded = [
             foundation.ReadAttributeRecord(
@@ -314,14 +336,32 @@
             [a.attrid for a in attributes]
         ):
             manufacturer = self.endpoint.manufacturer_id
         return await super()._write_attributes_undivided(
             attributes, *args, manufacturer=manufacturer, **kwargs
         )
 
+    def get(self, key: int | str, default: typing.Any | None = None) -> typing.Any:
+        """Get cached attribute."""
+
+        try:
+            attr_def = self.find_attribute(key)
+        except KeyError:
+            return super().get(key, default)
+
+        # Ensure we check the constant attributes dictionary first, since their values
+        # will not be in the attribute cache but can be read immediately.
+        if (
+            self._CONSTANT_ATTRIBUTES is not None
+            and attr_def.id in self._CONSTANT_ATTRIBUTES
+        ):
+            return self._CONSTANT_ATTRIBUTES[attr_def.id]
+
+        return super().get(key, default)
+
 
 def handle_message_from_uninitialized_sender(
     sender: zigpy.device.Device,
     profile: int,
     cluster: int,
     src_ep: int,
     dst_ep: int,
```

### Comparing `zigpy-0.54.1/zigpy/quirks/registry.py` & `zigpy-0.55.0/zigpy/quirks/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import collections
 import itertools
 import logging
-from typing import Dict, List, Optional, Union
+import typing
 
 from zigpy.const import (
     SIG_ENDPOINTS,
     SIG_EP_INPUT,
     SIG_EP_OUTPUT,
     SIG_EP_PROFILE,
     SIG_EP_TYPE,
@@ -14,16 +16,18 @@
     SIG_MODELS_INFO,
 )
 import zigpy.quirks
 from zigpy.typing import CustomDeviceType, DeviceType
 
 _LOGGER = logging.getLogger(__name__)
 
-TYPE_MODEL_QUIRKS_LIST = Dict[Optional[str], List["zigpy.quirks.CustomDevice"]]
-TYPE_MANUF_QUIRKS_DICT = Dict[Optional[str], TYPE_MODEL_QUIRKS_LIST]
+TYPE_MANUF_QUIRKS_DICT = typing.Dict[
+    typing.Optional[str],
+    typing.Dict[typing.Optional[str], typing.List["zigpy.quirks.CustomDevice"]],
+]
 
 
 class DeviceRegistry:
     def __init__(self, *args, **kwargs) -> None:
         self._registry: TYPE_MANUF_QUIRKS_DICT = collections.defaultdict(
             lambda: collections.defaultdict(list)
         )
@@ -47,15 +51,15 @@
             for manuf, model in models_info:
                 self.registry[manuf][model].remove(custom_device)
         else:
             manufacturer = custom_device.signature.get(SIG_MANUFACTURER)
             model = custom_device.signature.get(SIG_MODEL)
             self.registry[manufacturer][model].remove(custom_device)
 
-    def get_device(self, device: DeviceType) -> Union[CustomDeviceType, DeviceType]:
+    def get_device(self, device: DeviceType) -> CustomDeviceType | DeviceType:
         """Get a CustomDevice object, if one is available"""
         if isinstance(device, zigpy.quirks.CustomDevice):
             return device
         dev_ep = set(device.endpoints) - {0}
         _LOGGER.debug(
             "Checking quirks for %s %s (%s)",
             device.manufacturer,
@@ -146,19 +150,19 @@
             )
             device = candidate(device._application, device.ieee, device.nwk, device)
             break
 
         return device
 
     @staticmethod
-    def _match(a, b):
+    def _match(a: dict | typing.Iterable, b: dict | typing.Iterable) -> bool:
         return set(a) == set(b)
 
     @property
-    def registry(self):
+    def registry(self) -> TYPE_MANUF_QUIRKS_DICT:
         return self._registry
 
     def __contains__(self, device: CustomDeviceType) -> bool:
         manufacturer, model = device.signature.get(
             SIG_MODELS_INFO,
             [(device.signature.get(SIG_MANUFACTURER), device.signature.get(SIG_MODEL))],
         )[0]
```

### Comparing `zigpy-0.54.1/zigpy/serial.py` & `zigpy-0.55.0/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/state.py` & `zigpy-0.55.0/zigpy/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
         return self.value == other
 
     def __int__(self) -> int:
         """Return int of the current value."""
         return self.value
 
-    def __post_init__(self, initial_value) -> None:
+    def __post_init__(self, initial_value: int) -> None:
         """Initialize instance."""
         self._raw_value = initial_value
 
     def __str__(self) -> str:
         """String representation."""
         return f"{self.name} = {self.value}"
```

### Comparing `zigpy-0.54.1/zigpy/topology.py` & `zigpy-0.55.0/zigpy/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     t.EUI64.convert("ff:ff:ff:ff:ff:ff:ff:ff"),
 }
 
 
 class Topology(zigpy.util.ListenableMixin):
     """Topology scanner."""
 
-    def __init__(self, app: zigpy.application.ControllerApplication):
+    def __init__(self, app: zigpy.application.ControllerApplication) -> None:
         """Instantiate."""
         self._app: zigpy.application.ControllerApplication = app
         self._listeners: dict = {}
         self._scan_task: asyncio.Task | None = None
         self._scan_loop_task: asyncio.Task | None = None
 
         # Keep track of devices that do not support scanning
@@ -51,15 +51,15 @@
         )
         self.routes: dict[t.EUI64, list[zdo_t.Route]] = collections.defaultdict(list)
 
     def start_periodic_scans(self, period: int | float) -> None:
         self.stop_periodic_scans()
         self._scan_loop_task = asyncio.create_task(self._scan_loop(period))
 
-    def stop_periodic_scans(self):
+    def stop_periodic_scans(self) -> None:
         if self._scan_loop_task is not None:
             self._scan_loop_task.cancel()
 
     async def _scan_loop(self, period: int | float) -> None:
         """Delay scan by creating a task."""
 
         while True:
```

### Comparing `zigpy-0.54.1/zigpy/types/basic.py` & `zigpy-0.55.0/zigpy/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/types/named.py` & `zigpy-0.55.0/zigpy/types/named.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
-from typing import Iterable
+import typing
 
 from . import basic
 from .struct import Struct
 
+if typing.TYPE_CHECKING:
+    from typing_extensions import Self
+
 
 class BaseDataclassMixin:
-    def replace(self, **kwargs):
+    def replace(self, **kwargs) -> Self:
         return dataclasses.replace(self, **kwargs)
 
 
 def _hex_string_to_bytes(hex_string: str) -> bytes:
     """Parses a hex string with optional colon delimiters and whitespace into bytes."""
 
     # Strips out whitespace and colons
@@ -33,15 +36,15 @@
 
 
 class EUI64(basic.FixedList, item_type=basic.uint8_t, length=8):
     # EUI 64-bit ID (an IEEE address).
     def __repr__(self) -> str:
         return ":".join("%02x" % i for i in self[::-1])
 
-    def __hash__(self):
+    def __hash__(self) -> int:  # type: ignore
         return hash(repr(self))
 
     @classmethod
     def convert(cls, ieee: str) -> EUI64:
         if ieee is None:
             return None
         ieee = [basic.uint8_t(p) for p in _hex_string_to_bytes(ieee)[::-1]]
@@ -98,15 +101,15 @@
     CHANNEL_22 = 0x00400000
     CHANNEL_23 = 0x00800000
     CHANNEL_24 = 0x01000000
     CHANNEL_25 = 0x02000000
     CHANNEL_26 = 0x04000000
 
     @classmethod
-    def from_channel_list(cls: Channels, channels: Iterable[int]) -> Channels:
+    def from_channel_list(cls: Channels, channels: typing.Iterable[int]) -> Channels:
         mask = cls.NO_CHANNELS
 
         for channel in channels:
             if not 11 <= channel <= 26:
                 raise ValueError(
                     f"Invalid channel number {channel}. Must be between 11 and 26."
                 )
@@ -534,15 +537,15 @@
 @dataclasses.dataclass
 class AddrModeAddress(BaseDataclassMixin):
     """Address mode and address."""
 
     addr_mode: AddrMode
     address: NWK | Group | EUI64 | BroadcastAddress | None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.addr_mode is not None and self.address is not None:
             self.address = {
                 AddrMode.Group: Group,
                 AddrMode.NWK: NWK,
                 AddrMode.IEEE: EUI64,
                 AddrMode.Broadcast: BroadcastAddress,
             }[self.addr_mode](self.address)
```

### Comparing `zigpy-0.54.1/zigpy/types/struct.py` & `zigpy-0.55.0/zigpy/types/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 class Struct:
     @classmethod
     def _real_cls(cls) -> type:
         # The "Optional" subclass is dynamically created and breaks types.
         # We have to use a little introspection to find our real class.
         return next(c for c in cls.__mro__ if c.__name__ != "Optional")
 
-    def __init_subclass__(cls):
+    def __init_subclass__(cls) -> None:
         super().__init_subclass__()
 
         # Explicitly check for old-style structs
         if hasattr(cls, "_fields"):
             raise TypeError(
                 "Struct subclasses do not use `_fields` anymore."
                 " Use class attributes with type annotations."
```

### Comparing `zigpy-0.54.1/zigpy/typing.py` & `zigpy-0.55.0/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/util.py` & `zigpy-0.55.0/zigpy/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import abc
 import asyncio
 import collections
 import functools
 import inspect
 import logging
 import traceback
+import types
 import typing
 import warnings
 
 from crccheck.crc import CrcX25
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import ECB
@@ -22,28 +23,28 @@
 
 
 class ListenableMixin:
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._listeners: dict[int, tuple[typing.Callable, bool]] = {}
 
-    def _add_listener(self, listener, include_context):
+    def _add_listener(self, listener: typing.Any, include_context: bool) -> int:
         id_ = id(listener)
         while id_ in self._listeners:
             id_ += 1
         self._listeners[id_] = (listener, include_context)
         return id_
 
-    def add_listener(self, listener):
+    def add_listener(self, listener: typing.Any) -> int:
         return self._add_listener(listener, include_context=False)
 
-    def add_context_listener(self, listener):
+    def add_context_listener(self, listener: CatchingTaskMixin) -> int:
         return self._add_listener(listener, include_context=True)
 
-    def listener_event(self, method_name, *args):
+    def listener_event(self, method_name: str, *args) -> list[typing.Any | None]:
         result = []
         for listener, include_context in self._listeners.values():
             method = getattr(listener, method_name, None)
 
             if not method:
                 continue
 
@@ -57,15 +58,15 @@
                     "Error calling listener %r with args %r: %r", method, args, e
                 )
                 LOGGER.debug(
                     "Error calling listener %r with args %r", method, args, exc_info=e
                 )
         return result
 
-    async def async_event(self, method_name, *args):
+    async def async_event(self, method_name: str, *args) -> list[typing.Any]:
         tasks = []
         for listener, include_context in self._listeners.values():
             method = getattr(listener, method_name, None)
 
             if not method:
                 continue
 
@@ -92,60 +93,64 @@
 
 
 class LocalLogMixin:
     @abc.abstractmethod
     def log(self, lvl: int, msg: str, *args, **kwargs):  # pragma: no cover
         pass
 
-    def _log(self, lvl: int, msg: str, *args, **kwargs):
+    def _log(self, lvl: int, msg: str, *args, **kwargs) -> None:
         return self.log(lvl, msg, *args, stacklevel=4, **kwargs)
 
-        return self.log(lvl, msg, *args, **kwargs)
-
     def exception(self, msg, *args, **kwargs):
         return self._log(logging.ERROR, msg, *args, **kwargs)
 
-    def debug(self, msg, *args, **kwargs):
+    def debug(self, msg: str, *args, **kwargs) -> None:
         return self._log(logging.DEBUG, msg, *args, **kwargs)
 
-    def info(self, msg, *args, **kwargs):
+    def info(self, msg: str, *args, **kwargs) -> None:
         return self._log(logging.INFO, msg, *args, **kwargs)
 
-    def warning(self, msg, *args, **kwargs):
+    def warning(self, msg: str, *args, **kwargs) -> None:
         return self._log(logging.WARNING, msg, *args, **kwargs)
 
     def error(self, msg, *args, **kwargs):
         return self._log(logging.ERROR, msg, *args, **kwargs)
 
 
-async def retry(func, retry_exceptions, tries=3, delay=0.1):
+async def retry(
+    func: typing.Callable[[], typing.Awaitable[typing.Any]],
+    retry_exceptions: typing.Iterable[BaseException],
+    tries: int = 3,
+    delay: int | float = 0.1,
+) -> typing.Any:
     """Retry a function in case of exception
 
     Only exceptions in `retry_exceptions` will be retried.
     """
     while True:
         LOGGER.debug("Tries remaining: %s", tries)
         try:
-            r = await func()
-            return r
+            return await func()
         except retry_exceptions:
             if tries <= 1:
                 raise
             tries -= 1
             await asyncio.sleep(delay)
 
 
-def retryable(retry_exceptions, tries=1, delay=0.1):
+def retryable(
+    retry_exceptions: typing.Iterable[BaseException], tries: int = 1, delay: float = 0.1
+) -> typing.Callable:
     """Return a decorator which makes a function able to be retried
 
     This adds "tries" and "delay" keyword arguments to the function. Only
     exceptions in `retry_exceptions` will be retried.
     """
 
-    def decorator(func):
+    def decorator(func: typing.Callable) -> typing.Callable:
         nonlocal tries, delay
 
         @functools.wraps(func)
         def wrapper(*args, tries=tries, delay=delay, **kwargs):
             if tries <= 1:
                 return func(*args, **kwargs)
             return retry(
@@ -258,20 +263,20 @@
         return self._result
 
     @property
     def sequence(self) -> t.uint8_t:
         """Send Future."""
         return self._sequence
 
-    def __enter__(self):
+    def __enter__(self) -> Request:
         """Return context manager."""
         self._pending[self.sequence] = self
         return self
 
-    def __exit__(self, exc_type, exc_value, exc_traceback):
+    def __exit__(self, exc_type: None, exc_value: None, exc_traceback: None) -> bool:
         """Clean up pending on exit."""
         if not self.result.done():
             self.result.cancel()
         self._pending.pop(self.sequence)
 
         return not exc_type
 
@@ -376,15 +381,15 @@
     def num_waiting(self) -> int:
         return len(self._waiters)
 
     def locked(self) -> bool:
         """Returns True if semaphore cannot be acquired immediately."""
         return self._value <= 0
 
-    async def acquire(self):
+    async def acquire(self) -> typing.Literal[True]:
         """Acquire a semaphore.
 
         If the internal counter is larger than zero on entry, decrement it by one and
         return True immediately.  If it is zero on entry, block, waiting until some
         other coroutine has called release() to make it larger than 0, and then return
         True.
         """
@@ -419,15 +424,20 @@
         self._value += 1
         self._wake_up_next()
 
     async def __aenter__(self) -> None:
         await self.acquire()
         return None
 
-    async def __aexit__(self, exc_type, exc, tb):
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        traceback: types.TracebackType | None,
+    ) -> None:
         self.release()
 
     def __repr__(self) -> str:
         if self.locked():
             extra = f"locked, max value:{self._max_value}, waiters:{len(self._waiters)}"
         else:
             extra = f"unlocked, value:{self._value}, max value:{self._max_value}"
```

### Comparing `zigpy-0.54.1/zigpy/zcl/__init__.py` & `zigpy-0.55.0/zigpy/zcl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
 
 import enum
 import functools
 import logging
-from typing import Any, Sequence
+from typing import TYPE_CHECKING, Any, Sequence
 import warnings
 
 from zigpy import util
 import zigpy.types as t
 from zigpy.typing import AddressingMode, EndpointType
 from zigpy.zcl import foundation
 
+if TYPE_CHECKING:
+    from zigpy.appdb import PersistingListener
+    from zigpy.endpoint import Endpoint
+
+
 LOGGER = logging.getLogger(__name__)
 
 
 def convert_list_schema(
     schema: Sequence[type], command_id: int, direction: foundation.Direction
 ) -> type[t.Struct]:
     schema_dict = {}
@@ -153,15 +158,15 @@
 
         if cls.cluster_id is not None:
             cls._registry[cls.cluster_id] = cls
 
         if cls.cluster_id_range is not None:
             cls._registry_range[cls.cluster_id_range] = cls
 
-    def __init__(self, endpoint: EndpointType, is_server: bool = True):
+    def __init__(self, endpoint: EndpointType, is_server: bool = True) -> None:
         self._endpoint: EndpointType = endpoint
         self._attr_cache: dict[int, Any] = {}
         self.unsupported_attributes: set[int | str] = set()
         self._listeners = {}
         self._type: ClusterType = (
             ClusterType.Server if is_server else ClusterType.Client
         )
@@ -336,15 +341,15 @@
         general: bool,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
         schema: dict | t.Struct,
         *args,
         manufacturer: int | t.uint16_t | None = None,
         tsn: int | t.uint8_t | None = None,
         **kwargs,
-    ):
+    ) -> None:
         hdr, request = self._create_request(
             general=general,
             command_id=command_id,
             schema=schema,
             manufacturer=manufacturer,
             tsn=tsn,
             disable_default_response=True,
@@ -363,15 +368,15 @@
 
     def handle_message(
         self,
         hdr: foundation.ZCLHeader,
         args: list[Any],
         *,
         dst_addressing: AddressingMode | None = None,
-    ):
+    ) -> None:
         self.debug(
             "Received command 0x%02X (TSN %d): %s", hdr.command_id, hdr.tsn, args
         )
         if hdr.frame_control.is_cluster:
             self.handle_cluster_request(hdr, args, dst_addressing=dst_addressing)
             self.listener_event("cluster_command", hdr.tsn, hdr.command_id, args)
             return
@@ -436,15 +441,15 @@
 
     async def read_attributes(
         self,
         attributes: list[int | str],
         allow_cache: bool = False,
         only_cache: bool = False,
         manufacturer: int | t.uint16_t | None = None,
-    ):
+    ) -> Any:
         success, failure = {}, {}
         attribute_ids: list[int] = []
         orig_attributes: dict[int, int | str] = {}
 
         for attribute in attributes:
             if isinstance(attribute, str):
                 attrid = self.attributes_by_name[attribute].id
@@ -742,43 +747,43 @@
 
     @property
     def is_server(self) -> bool:
         """Return True if this is a server cluster."""
         return self._type == ClusterType.Server
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.__class__.__name__
 
     @property
-    def endpoint(self):
+    def endpoint(self) -> Endpoint:
         return self._endpoint
 
     @property
     def commands(self):
         return list(self._server_commands_idx.keys())
 
-    def update_attribute(self, attrid, value):
+    def update_attribute(self, attrid: int | t.uint16_t, value: Any) -> None:
         """Update specified attribute with specified value"""
         self._update_attribute(attrid, value)
 
-    def _update_attribute(self, attrid, value):
+    def _update_attribute(self, attrid: int | t.uint16_t, value: Any) -> None:
         self._attr_cache[attrid] = value
         self.listener_event("attribute_updated", attrid, value)
 
-    def log(self, lvl, msg, *args, **kwargs):
+    def log(self, lvl: int, msg: str, *args, **kwargs) -> None:
         msg = "[%s:%s:0x%04x] " + msg
         args = (
             self._endpoint.device.name,
             self._endpoint.endpoint_id,
             self.cluster_id,
         ) + args
         return LOGGER.log(lvl, msg, *args, **kwargs)
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> functools.partial:
         if name in self._client_commands_idx:
             return functools.partial(
                 self.client_command, self._client_commands_idx[name]
             )
         elif name in self._server_commands_idx:
             return functools.partial(self.command, self._server_commands_idx[name])
         else:
@@ -926,25 +931,25 @@
             if isinstance(attr, int):
                 self.remove_unsupported_attribute(attrdef.name, inhibit_events)
             else:
                 self.remove_unsupported_attribute(attrdef.id, inhibit_events)
 
 
 class ClusterPersistingListener:
-    def __init__(self, applistener, cluster):
+    def __init__(self, applistener: PersistingListener, cluster: Cluster) -> None:
         self._applistener = applistener
         self._cluster = cluster
 
-    def attribute_updated(self, attrid, value):
+    def attribute_updated(self, attrid: int | t.uint16_t, value: Any) -> None:
         self._applistener.attribute_updated(self._cluster, attrid, value)
 
-    def cluster_command(self, *args, **kwargs):
+    def cluster_command(self, *args, **kwargs) -> None:
         pass
 
-    def general_command(self, *args, **kwargs):
+    def general_command(self, *args, **kwargs) -> None:
         pass
 
     def unsupported_attribute_added(self, attrid: int) -> None:
         """An unsupported attribute was added."""
         self._applistener.unsupported_attribute_added(self._cluster, attrid)
 
     def unsupported_attribute_removed(self, attrid: int) -> None:
```

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/__init__.py` & `zigpy-0.55.0/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/closures.py` & `zigpy-0.55.0/zigpy/zcl/clusters/closures.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/general.py` & `zigpy-0.55.0/zigpy/zcl/clusters/general.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/homeautomation.py` & `zigpy-0.55.0/zigpy/zcl/clusters/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/hvac.py` & `zigpy-0.55.0/zigpy/zcl/clusters/hvac.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/lighting.py` & `zigpy-0.55.0/zigpy/zcl/clusters/lighting.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.55.0/zigpy/zcl/clusters/lightlink.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/measurement.py` & `zigpy-0.55.0/zigpy/zcl/clusters/measurement.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/protocol.py` & `zigpy-0.55.0/zigpy/zcl/clusters/protocol.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/security.py` & `zigpy-0.55.0/zigpy/zcl/clusters/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.55.0/zigpy/zcl/clusters/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zcl/foundation.py` & `zigpy-0.55.0/zigpy/zcl/foundation.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,19 +94,19 @@
             other = type
             type = other.type
             value = other.value
 
         self.type = type
         self.value = value
 
-    def serialize(self):
+    def serialize(self) -> bytes:
         return self.type.to_bytes(1, "little") + self.value.serialize()
 
     @classmethod
-    def deserialize(cls, data):
+    def deserialize(cls, data: bytes) -> tuple[TypeValue, bytes]:
         type, data = t.uint8_t.deserialize(data)
         python_type = DATA_TYPES[type][1]
         value, data = python_type.deserialize(data)
 
         return cls(type=type, value=value), data
 
     def __repr__(self) -> str:
@@ -138,21 +138,34 @@
 class Set(TypedCollection):
     pass  # ToDo: Make this a real set?
 
 
 class DataTypes(dict):
     """DataTypes container."""
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        data_types: dict[
+            int,
+            tuple[
+                str,
+                typing.Any,
+                typing.Literal[Null]
+                | typing.Literal[Discrete]
+                | typing.Literal[Analog]
+                | typing.Literal[None],
+            ],
+        ],
+    ) -> None:
+        super().__init__(data_types)
         self._idx_by_class = {
             _type: type_id for type_id, (name, _type, ad) in self.items()
         }
 
-    def pytype_to_datatype_id(self, python_type) -> int:
+    def pytype_to_datatype_id(self, python_type: typing.Any) -> int:
         """Return Zigbee Datatype ID for a give python type."""
 
         # We return the most specific parent class
         for cls in python_type.__mro__:
             if cls in self._idx_by_class:
                 return self._idx_by_class[cls]
 
@@ -390,15 +403,15 @@
 
 class ConfigureReportingResponseRecord(t.Struct):
     status: Status
     direction: ReportingDirection
     attrid: t.uint16_t = t.StructField(repr=_hex_uint16_repr)
 
     @classmethod
-    def deserialize(cls, data):
+    def deserialize(cls, data: bytes) -> tuple[ConfigureReportingResponseRecord, bytes]:
         r = cls()
         r.status, data = Status.deserialize(data)
         if r.status == Status.SUCCESS:
             r.direction, data = t.Optional(t.uint8_t).deserialize(data)
             if r.direction is not None:
                 r.direction = ReportingDirection(r.direction)
             r.attrid, data = t.Optional(t.uint16_t).deserialize(data)
@@ -411,15 +424,15 @@
     def serialize(self):
         r = Status(self.status).serialize()
         if self.status != Status.SUCCESS:
             r += ReportingDirection(self.direction).serialize()
             r += t.uint16_t(self.attrid).serialize()
         return r
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         r = f"{self.__class__.__name__}(status={self.status}"
         if self.status != Status.SUCCESS:
             r += f", direction={self.direction}, attrid={self.attrid}"
         r += ")"
         return r
 
 
@@ -543,15 +556,19 @@
     manufacturer: t.uint16_t = t.StructField(
         requires=lambda hdr: hdr.frame_control.is_manufacturer_specific
     )
     tsn: t.uint8_t
     command_id: t.uint8_t
 
     def __new__(
-        cls, frame_control=None, manufacturer=None, tsn=None, command_id=None
+        cls: type[ZCLHeader],
+        frame_control: FrameControl | None = None,
+        manufacturer: t.uint16_t | None = None,
+        tsn: int | t.uint8_t | None = None,
+        command_id: int | GeneralCommand | None = None,
     ) -> ZCLHeader:
         # Allow "auto manufacturer ID" to be disabled in higher layers
         if manufacturer is cls.NO_MANUFACTURER_ID:
             manufacturer = None
 
         if frame_control is not None and manufacturer is not None:
             frame_control.is_manufacturer_specific = True
@@ -559,15 +576,19 @@
         return super().__new__(cls, frame_control, manufacturer, tsn, command_id)
 
     @property
     def direction(self) -> bool:
         """Return direction of Frame Control."""
         return self.frame_control.direction
 
-    def __setattr__(self, name, value) -> None:
+    def __setattr__(
+        self,
+        name: str,
+        value: t.uint16_t | FrameControl | t.uint8_t | GeneralCommand | None,
+    ) -> None:
         if name == "manufacturer" and value is self.NO_MANUFACTURER_ID:
             value = None
 
         super().__setattr__(name, value)
 
         if name == "manufacturer" and self.frame_control is not None:
             self.frame_control.is_manufacturer_specific = value is not None
@@ -613,23 +634,23 @@
 class ZCLCommandDef(t.BaseDataclassMixin):
     name: str = None
     schema: CommandSchema = None
     direction: Direction = None
     id: t.uint8_t = None
     is_manufacturer_specific: bool = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         ensure_valid_name(self.name)
 
         if isinstance(self.direction, bool):
             object.__setattr__(
                 self, "direction", Direction._from_is_reply(self.direction)
             )
 
-    def with_compiled_schema(self):
+    def with_compiled_schema(self) -> ZCLCommandDef:
         """Return a copy of the ZCL command definition object with its dictionary command
         schema converted into a `CommandSchema` subclass.
         """
 
         if isinstance(self.schema, tuple):
             raise ValueError(
                 f"Tuple schemas are deprecated: {self.schema!r}. Use a dictionary or a"
@@ -683,15 +704,17 @@
     """Struct subclass that behaves more like a tuple."""
 
     command: ZCLCommandDef = None
 
     def __iter__(self):
         return iter(self.as_tuple())
 
-    def __getitem__(self, item):
+    def __getitem__(
+        self, item: slice | typing.SupportsIndex
+    ) -> typing.Any | tuple[typing.Any, ...]:
         return self.as_tuple()[item]
 
     def __len__(self) -> int:
         return len(self.as_tuple())
 
     def __eq__(self, other) -> bool:
         if isinstance(other, tuple) and not isinstance(other, type(self)):
@@ -750,15 +773,15 @@
     )
     mandatory: bool = False
     is_manufacturer_specific: bool = False
 
     # The ID will be specified later
     id: t.uint16_t = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.id is not None and not isinstance(self.id, t.uint16_t):
             object.__setattr__(self, "id", t.uint16_t(self.id))
 
         if isinstance(self.access, str):
             ZCLAttributeAccess.NONE
             object.__setattr__(self, "access", ZCLAttributeAccess.from_str(self.access))
```

### Comparing `zigpy-0.54.1/zigpy/zdo/__init__.py` & `zigpy-0.55.0/zigpy/zdo/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy/zdo/types.py` & `zigpy-0.55.0/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.54.1/zigpy.egg-info/PKG-INFO` & `zigpy-0.55.0/zigpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.54.1
+Version: 0.55.0
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.54.1/zigpy.egg-info/SOURCES.txt` & `zigpy-0.55.0/zigpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

