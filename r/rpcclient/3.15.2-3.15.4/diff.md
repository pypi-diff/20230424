# Comparing `tmp/rpcclient-3.15.2.tar.gz` & `tmp/rpcclient-3.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-3.15.2.tar", last modified: Wed Mar 29 23:00:34 2023, max compression
+gzip compressed data, was "rpcclient-3.15.4.tar", last modified: Mon Apr 24 06:57:29 2023, max compression
```

## Comparing `rpcclient-3.15.2.tar` & `rpcclient-3.15.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.896152 rpcclient-3.15.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-29 23:00:22.000000 rpcclient-3.15.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-29 23:00:34.896152 rpcclient-3.15.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-29 23:00:22.000000 rpcclient-3.15.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.888152 rpcclient-3.15.2/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.892151 rpcclient-3.15.2/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    35778 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.892151 rpcclient-3.15.2/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.892151 rpcclient-3.15.2/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.892151 rpcclient-3.15.2/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.892151 rpcclient-3.15.2/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-03-29 23:00:22.000000 rpcclient-3.15.2/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 23:00:34.888152 rpcclient-3.15.2/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-29 23:00:34.000000 rpcclient-3.15.2/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-29 23:00:34.000000 rpcclient-3.15.2/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 23:00:34.000000 rpcclient-3.15.2/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 23:00:34.000000 rpcclient-3.15.2/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-29 23:00:34.000000 rpcclient-3.15.2/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 23:00:34.000000 rpcclient-3.15.2/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 23:00:34.896152 rpcclient-3.15.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-29 23:00:22.000000 rpcclient-3.15.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-24 06:57:20.000000 rpcclient-3.15.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-24 06:57:29.719548 rpcclient-3.15.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-24 06:57:20.000000 rpcclient-3.15.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.715548 rpcclient-3.15.4/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37668 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.719548 rpcclient-3.15.4/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-04-24 06:57:20.000000 rpcclient-3.15.4/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:57:29.715548 rpcclient-3.15.4/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 06:57:29.000000 rpcclient-3.15.4/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:57:29.719548 rpcclient-3.15.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-24 06:57:20.000000 rpcclient-3.15.4/setup.py
```

### Comparing `rpcclient-3.15.2/LICENSE` & `rpcclient-3.15.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/PKG-INFO` & `rpcclient-3.15.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.15.2
+Version: 3.15.4
 Summary: rpcclient for connecting with the rpcserver
 Home-page: https://github.com/doronz88/rpc-project
 Author: DoronZ
 Author-email: doron88@gmail.com
 License: GNU GENERAL PUBLIC LICENSE - Version 3, 29 June 2007
 Project-URL: rpc-project, https://github.com/doronz88/rpc-project
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `rpcclient-3.15.2/rpcclient/__main__.py` & `rpcclient-3.15.4/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/client.py` & `rpcclient-3.15.4/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/client_factory.py` & `rpcclient-3.15.4/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/bluetooth.py` & `rpcclient-3.15.4/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/cfpreferences.py` & `rpcclient-3.15.4/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/client.py` & `rpcclient-3.15.4/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/consts.py` & `rpcclient-3.15.4/rpcclient/darwin/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -918,7 +918,60 @@
 
     OFF = 0
     NONE = 0
     UNDEFINED = 1  # no such plist key
     DEFAULT = 2
     INFO = 3
     DEBUG = 4
+
+
+# Definitions of flags stored in file flags word.
+# Super-user and owner changeable flags.
+
+UF_SETTABLE = 0x0000ffff  # mask of owner changeable flags
+UF_NODUMP = 0x00000001  # do not dump file
+UF_IMMUTABLE = 0x00000002  # file may not be changed
+UF_APPEND = 0x00000004  # writes to file may only append
+UF_OPAQUE = 0x00000008  # directory is opaque wrt. union
+
+# The following bit is reserved for FreeBSD.  It is not implemented
+# in Mac OS X.
+
+# UF_NOUNLINK =  0x00000010  # file may not be removed or renamed
+UF_COMPRESSED = 0x00000020  # file is compressed (some file-systems)
+
+# UF_TRACKED is used for dealing with document IDs.  We no longer issue
+#  notifications for deletes or renames for files which have UF_TRACKED set.
+UF_TRACKED = 0x00000040
+
+UF_DATAVAULT = 0x00000080  # entitlement required for reading
+# and writing
+
+# Bits 0x0100 through 0x4000 are currently undefined.
+UF_HIDDEN = 0x00008000  # hint that this item should not be
+# displayed in a GUI
+#
+# Super-user changeable flags.
+
+SF_SUPPORTED = 0x009f0000  # mask of superuser supported flags
+SF_SETTABLE = 0x3fff0000  # mask of superuser changeable flags
+SF_SYNTHETIC = 0xc0000000  # mask of system read-only synthetic flags
+SF_ARCHIVED = 0x00010000  # file is archived
+SF_IMMUTABLE = 0x00020000  # file may not be changed
+SF_APPEND = 0x00040000  # writes to file may only append
+SF_RESTRICTED = 0x00080000  # entitlement required for writing
+SF_NOUNLINK = 0x00100000  # Item may not be removed, renamed or mounted on
+
+# The following two bits are reserved for FreeBSD.  They are not
+# implemented in Mac OS X.
+
+# SF_SNAPSHOT =  0x00200000  # snapshot inode
+# NOTE: There is no SF_HIDDEN bit.
+
+SF_FIRMLINK = 0x00800000  # file is a firmlink
+
+# Synthetic flags.
+#
+# These are read-only.  We keep them out of SF_SUPPORTED so that
+# attempts to set them will fail.
+
+SF_DATALESS = 0x40000000  # file is dataless object
```

### Comparing `rpcclient-3.15.2/rpcclient/darwin/core_graphics.py` & `rpcclient-3.15.4/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/crash_reports.py` & `rpcclient-3.15.4/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/darwin_lief.py` & `rpcclient-3.15.4/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/fs.py` & `rpcclient-3.15.4/rpcclient/darwin/fs.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,7 +70,13 @@
 
     @path_to_str('path')
     def statfs(self, path: str):
         with self._client.safe_malloc(statfs64.sizeof()) as buf:
             if 0 != self._client.symbols.statfs64(path, buf):
                 self._client.raise_errno_exception(f'statfs failed for: {path}')
             return statfs64.parse_stream(buf)
+
+    @path_to_str('path')
+    def chflags(self, path: str, flags: int) -> None:
+        """ call chflags(path, flags) at remote. see manpage for more info """
+        if 0 != self._client.symbols.chflags(path, flags):
+            self._client.raise_errno_exception(f'chflags failed for: {path}')
```

### Comparing `rpcclient-3.15.2/rpcclient/darwin/hid.py` & `rpcclient-3.15.4/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/ioregistry.py` & `rpcclient-3.15.4/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/location.py` & `rpcclient-3.15.4/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/media.py` & `rpcclient-3.15.4/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/network.py` & `rpcclient-3.15.4/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/objc.py` & `rpcclient-3.15.4/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/objective_c_class.py` & `rpcclient-3.15.4/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-3.15.4/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/processes.py` & `rpcclient-3.15.4/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/reports.py` & `rpcclient-3.15.4/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/scpreferences.py` & `rpcclient-3.15.4/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/structs.py` & `rpcclient-3.15.4/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/symbol.py` & `rpcclient-3.15.4/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/syslog.py` & `rpcclient-3.15.4/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/darwin/time.py` & `rpcclient-3.15.4/rpcclient/darwin/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,11 @@
         """ opt-in automatic time settings """
         self._client.symbols.TMSetAutomaticTimeZoneEnabled(1)
 
     @property
     def is_set_automatically(self):
         """ tell is time settings are set to automatic """
         return bool(self._client.symbols.TMIsAutomaticTimeZoneEnabled())
+
+    def boot_time(self) -> datetime:
+        timestamp = timeval.parse(self._client.sysctl.get_by_name('kern.boottime')).tv_sec
+        return datetime.fromtimestamp(timestamp)
```

### Comparing `rpcclient-3.15.2/rpcclient/darwin/xpc.py` & `rpcclient-3.15.4/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/exceptions.py` & `rpcclient-3.15.4/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/fs.py` & `rpcclient-3.15.4/rpcclient/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/accessibility.py` & `rpcclient-3.15.4/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/backlight.py` & `rpcclient-3.15.4/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/client.py` & `rpcclient-3.15.4/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/lockdown.py` & `rpcclient-3.15.4/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/mobile_gestalt.py` & `rpcclient-3.15.4/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/screen_capture.py` & `rpcclient-3.15.4/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/sprinboard.py` & `rpcclient-3.15.4/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/telephony.py` & `rpcclient-3.15.4/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/ios/wifi.py` & `rpcclient-3.15.4/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/lief.py` & `rpcclient-3.15.4/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/linux/client.py` & `rpcclient-3.15.4/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/linux/structs.py` & `rpcclient-3.15.4/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/macos/apple_script.py` & `rpcclient-3.15.4/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/macos/client.py` & `rpcclient-3.15.4/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/network.py` & `rpcclient-3.15.4/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/processes.py` & `rpcclient-3.15.4/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/protocol.py` & `rpcclient-3.15.4/rpcclient/protocol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/structs/consts.py` & `rpcclient-3.15.4/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/structs/generic.py` & `rpcclient-3.15.4/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/symbol.py` & `rpcclient-3.15.4/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/symbols_jar.py` & `rpcclient-3.15.4/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/sysctl.py` & `rpcclient-3.15.4/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient/xonshrc.py` & `rpcclient-3.15.4/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/rpcclient.egg-info/PKG-INFO` & `rpcclient-3.15.4/rpcclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.15.2
+Version: 3.15.4
 Summary: rpcclient for connecting with the rpcserver
 Home-page: https://github.com/doronz88/rpc-project
 Author: DoronZ
 Author-email: doron88@gmail.com
 License: GNU GENERAL PUBLIC LICENSE - Version 3, 29 June 2007
 Project-URL: rpc-project, https://github.com/doronz88/rpc-project
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `rpcclient-3.15.2/rpcclient.egg-info/SOURCES.txt` & `rpcclient-3.15.4/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-3.15.2/setup.py` & `rpcclient-3.15.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 BASE_DIR = Path(__file__).parent.resolve(strict=True)
-VERSION = '3.15.2'
+VERSION = '3.15.4'
 PACKAGE_NAME = 'rpcclient'
 PACKAGES = [p for p in find_packages() if not p.startswith('tests')]
 
 
 def parse_requirements():
     reqs = []
     with open(BASE_DIR / 'requirements.txt', 'r') as fd:
```

