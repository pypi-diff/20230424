# Comparing `tmp/yalexs-1.3.0.tar.gz` & `tmp/yalexs-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs-1.3.0.tar", last modified: Fri Apr 14 19:37:13 2023, max compression
+gzip compressed data, was "yalexs-1.3.1.tar", last modified: Mon Apr 24 17:14:58 2023, max compression
```

## Comparing `yalexs-1.3.0.tar` & `yalexs-1.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.450432 yalexs-1.3.0/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.440006 yalexs-1.3.0/.github/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.442274 yalexs-1.3.0/.github/workflows/
--rw-r--r--   0 bdraco     (501) staff       (20)     2383 2023-02-17 14:33:57.000000 yalexs-1.3.0/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.3.0/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.3.0/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.3.0/MANIFEST
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-14 19:37:13.450515 yalexs-1.3.0/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.3.0/README.md
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.3.0/build.sh
--rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.3.0/known_activities.md
--rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.3.0/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       46 2023-02-17 14:03:08.000000 yalexs-1.3.0/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.3.0/requirements_tests.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-14 19:37:13.450814 yalexs-1.3.0/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)      972 2023-04-14 19:36:50.000000 yalexs-1.3.0/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.443261 yalexs-1.3.0/tests/
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.447942 yalexs-1.3.0/tests/fixtures/
--rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/auto_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/auto_relock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/auto_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/bluetooth_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/door_closed_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/door_closed_activity_wrong_deviceid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/door_closed_activity_wrong_houseid.json
--rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/door_open_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/doorbell_motion_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/doorbell_motion_activity_no_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/doorbell_motion_activity_old.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/doorbell_motion_activity_wrong.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbell.battery_full.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbell.battery_low.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbell.battery_medium.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbell.json
--rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbell.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbell_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_doorbells.json
--rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_house_activities.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock.doorsense_init.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock.nostatus_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock.offline.json
--rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock.online_with_doorsense.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json
--rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_lock_v2.online.json
--rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_locks.json
--rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/get_pins.json
--rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/keypad_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/lock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/lock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/manual_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/manual_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/pin_unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/pin_unlock_activity_missing_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/pin_unlock_activity_with_image.json
--rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/remote_lock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/remote_lock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/remote_unlock_activity_v4.json
--rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/remote_unlock_activity_v4_2.json
--rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/unlock.json
--rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/unlock_activity.json
--rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/fixtures/unlock_without_doorstate.json
--rw-r--r--   0 bdraco     (501) staff       (20)    14610 2023-02-17 14:03:08.000000 yalexs-1.3.0/tests/test_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    31589 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/test_api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38166 2023-02-17 14:33:57.000000 yalexs-1.3.0/tests/test_api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/test_authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     8411 2023-02-17 14:03:08.000000 yalexs-1.3.0/tests/test_authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    14092 2023-04-14 19:36:42.000000 yalexs-1.3.0/tests/test_pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10482 2023-02-17 14:03:03.000000 yalexs-1.3.0/tests/test_util.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.3.0/tox.ini
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.449843 yalexs-1.3.0/yalexs/
--rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-04-14 19:36:50.000000 yalexs-1.3.0/yalexs/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    13856 2023-04-14 19:36:01.000000 yalexs-1.3.0/yalexs/activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     9792 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/api.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12351 2023-02-17 14:03:08.000000 yalexs-1.3.0/yalexs/api_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)    10480 2023-04-14 19:36:42.000000 yalexs-1.3.0/yalexs/api_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4740 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/authenticator.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5057 2023-02-17 14:03:08.000000 yalexs-1.3.0/yalexs/authenticator_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     5080 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/authenticator_common.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/bridge.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/device.py
--rw-r--r--   0 bdraco     (501) staff       (20)     4284 2023-02-17 14:03:08.000000 yalexs-1.3.0/yalexs/doorbell.py
--rw-r--r--   0 bdraco     (501) staff       (20)      273 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/keypad.py
--rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/lock.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.3.0/yalexs/pin.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3816 2023-04-14 19:36:42.000000 yalexs-1.3.0/yalexs/pubnub_activity.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/pubnub_async.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.3.0/yalexs/users.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2554 2023-02-17 14:03:08.000000 yalexs-1.3.0/yalexs/util.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-14 19:37:13.450323 yalexs-1.3.0/yalexs.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-14 19:37:13.000000 yalexs-1.3.0/yalexs.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     2799 2023-04-14 19:37:13.000000 yalexs-1.3.0/yalexs.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-14 19:37:13.000000 yalexs-1.3.0/yalexs.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-04-14 19:37:13.000000 yalexs-1.3.0/yalexs.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-04-14 19:37:13.000000 yalexs-1.3.0/yalexs.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.181164 yalexs-1.3.1/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.166974 yalexs-1.3.1/.github/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.169823 yalexs-1.3.1/.github/workflows/
+-rw-r--r--   0 bdraco     (501) staff       (20)     2383 2023-02-17 14:33:57.000000 yalexs-1.3.1/.github/workflows/ci.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)     1180 2023-02-17 14:03:03.000000 yalexs-1.3.1/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1063 2023-02-17 14:03:03.000000 yalexs-1.3.1/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      398 2023-02-17 14:03:03.000000 yalexs-1.3.1/MANIFEST
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-24 17:14:58.181235 yalexs-1.3.1/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4569 2023-02-17 14:03:03.000000 yalexs-1.3.1/README.md
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-02-17 14:03:03.000000 yalexs-1.3.1/build.sh
+-rw-r--r--   0 bdraco     (501) staff       (20)     4283 2023-02-17 14:03:03.000000 yalexs-1.3.1/known_activities.md
+-rw-r--r--   0 bdraco     (501) staff       (20)     1337 2023-02-17 14:03:03.000000 yalexs-1.3.1/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       46 2023-02-17 14:03:08.000000 yalexs-1.3.1/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      132 2023-02-17 14:33:57.000000 yalexs-1.3.1/requirements_tests.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-24 17:14:58.181516 yalexs-1.3.1/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)      972 2023-04-24 17:14:23.000000 yalexs-1.3.1/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.171048 yalexs-1.3.1/tests/
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.177302 yalexs-1.3.1/tests/fixtures/
+-rw-r--r--   0 bdraco     (501) staff       (20)      311 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/auto_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      926 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/auto_relock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      918 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/auto_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1331 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/bluetooth_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      774 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/door_closed_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      777 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/door_closed_activity_wrong_deviceid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      780 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/door_closed_activity_wrong_houseid.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      772 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/door_open_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1475 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/doorbell_motion_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      907 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/doorbell_motion_activity_no_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1501 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/doorbell_motion_activity_old.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1495 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/doorbell_motion_activity_wrong.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3198 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbell.battery_full.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3188 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbell.battery_low.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3197 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbell.battery_medium.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2488 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbell.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     3780 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbell.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1898 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbell_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2255 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_doorbells.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     9741 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_house_activities.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2744 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock.doorsense_init.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1182 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock.nostatus_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1680 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock.offline.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     2745 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1368 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock.online_with_doorsense.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1373 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock.online_with_doorsense_disabled.json
+-rw-r--r--   0 bdraco     (501) staff       (20)     1633 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_lock_v2.online.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      408 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_locks.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      664 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/get_pins.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      848 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/keypad_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      682 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/lock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      800 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      641 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/lock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      315 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/manual_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      321 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/manual_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      458 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/pin_unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/pin_unlock_activity_missing_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      479 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/pin_unlock_activity_with_image.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      827 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/remote_lock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      435 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/remote_lock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      441 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/remote_unlock_activity_v4.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      559 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/remote_unlock_activity_v4_2.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      686 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/unlock.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      732 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/unlock_activity.json
+-rw-r--r--   0 bdraco     (501) staff       (20)      648 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/fixtures/unlock_without_doorstate.json
+-rw-r--r--   0 bdraco     (501) staff       (20)    14702 2023-04-24 17:14:19.000000 yalexs-1.3.1/tests/test_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    31589 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/test_api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38166 2023-02-17 14:33:57.000000 yalexs-1.3.1/tests/test_api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7495 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/test_authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     8411 2023-02-17 14:03:08.000000 yalexs-1.3.1/tests/test_authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    14464 2023-04-24 17:14:19.000000 yalexs-1.3.1/tests/test_pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10482 2023-02-17 14:03:03.000000 yalexs-1.3.1/tests/test_util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1316 2023-02-17 14:33:57.000000 yalexs-1.3.1/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.180493 yalexs-1.3.1/yalexs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      114 2023-04-24 17:14:23.000000 yalexs-1.3.1/yalexs/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    13964 2023-04-24 17:14:19.000000 yalexs-1.3.1/yalexs/activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     9792 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/api.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    12351 2023-02-17 14:03:08.000000 yalexs-1.3.1/yalexs/api_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10480 2023-04-14 19:36:42.000000 yalexs-1.3.1/yalexs/api_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4740 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/authenticator.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5057 2023-02-17 14:03:08.000000 yalexs-1.3.1/yalexs/authenticator_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     5080 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/authenticator_common.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1852 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/bridge.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1399 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/device.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4284 2023-02-17 14:03:08.000000 yalexs-1.3.1/yalexs/doorbell.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      273 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1050 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/keypad.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     7977 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/lock.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2435 2023-02-20 05:39:04.000000 yalexs-1.3.1/yalexs/pin.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     4172 2023-04-24 17:14:19.000000 yalexs-1.3.1/yalexs/pubnub_activity.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3797 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/pubnub_async.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1088 2023-02-17 14:03:03.000000 yalexs-1.3.1/yalexs/users.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2554 2023-02-17 14:03:08.000000 yalexs-1.3.1/yalexs/util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-24 17:14:58.181074 yalexs-1.3.1/yalexs.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)      666 2023-04-24 17:14:58.000000 yalexs-1.3.1/yalexs.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     2799 2023-04-24 17:14:58.000000 yalexs-1.3.1/yalexs.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-24 17:14:58.000000 yalexs-1.3.1/yalexs.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       66 2023-04-24 17:14:58.000000 yalexs-1.3.1/yalexs.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        7 2023-04-24 17:14:58.000000 yalexs-1.3.1/yalexs.egg-info/top_level.txt
```

### Comparing `yalexs-1.3.0/.github/workflows/ci.yaml` & `yalexs-1.3.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/.gitignore` & `yalexs-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/LICENSE` & `yalexs-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/PKG-INFO` & `yalexs-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.3.0/README.md` & `yalexs-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/known_activities.md` & `yalexs-1.3.1/known_activities.md`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/pylintrc` & `yalexs-1.3.1/pylintrc`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/setup.cfg` & `yalexs-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.3.0
+current_version = 1.3.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `yalexs-1.3.0/setup.py` & `yalexs-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="yalexs",
-    version="1.3.0",
+    version="1.3.1",
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `yalexs-1.3.0/tests/fixtures/auto_relock_activity.json` & `yalexs-1.3.1/tests/fixtures/auto_relock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/auto_unlock_activity.json` & `yalexs-1.3.1/tests/fixtures/auto_unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/bluetooth_lock_activity.json` & `yalexs-1.3.1/tests/fixtures/bluetooth_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/door_closed_activity.json` & `yalexs-1.3.1/tests/fixtures/door_closed_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/door_closed_activity_wrong_deviceid.json` & `yalexs-1.3.1/tests/fixtures/door_closed_activity_wrong_deviceid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/door_closed_activity_wrong_houseid.json` & `yalexs-1.3.1/tests/fixtures/door_closed_activity_wrong_houseid.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/door_open_activity.json` & `yalexs-1.3.1/tests/fixtures/door_open_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/doorbell_motion_activity.json` & `yalexs-1.3.1/tests/fixtures/doorbell_motion_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/doorbell_motion_activity_no_image.json` & `yalexs-1.3.1/tests/fixtures/doorbell_motion_activity_no_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/doorbell_motion_activity_old.json` & `yalexs-1.3.1/tests/fixtures/doorbell_motion_activity_old.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/doorbell_motion_activity_wrong.json` & `yalexs-1.3.1/tests/fixtures/doorbell_motion_activity_wrong.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbell.battery_full.json` & `yalexs-1.3.1/tests/fixtures/get_doorbell.battery_full.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbell.battery_low.json` & `yalexs-1.3.1/tests/fixtures/get_doorbell.battery_low.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbell.battery_medium.json` & `yalexs-1.3.1/tests/fixtures/get_doorbell.battery_medium.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbell.json` & `yalexs-1.3.1/tests/fixtures/get_doorbell.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbell.offline.json` & `yalexs-1.3.1/tests/fixtures/get_doorbell.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbell_missing_image.json` & `yalexs-1.3.1/tests/fixtures/get_doorbell_missing_image.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_doorbells.json` & `yalexs-1.3.1/tests/fixtures/get_doorbells.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_house_activities.json` & `yalexs-1.3.1/tests/fixtures/get_house_activities.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock.doorsense_init.json` & `yalexs-1.3.1/tests/fixtures/get_lock.doorsense_init.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock.nostatus_with_doorsense.json` & `yalexs-1.3.1/tests/fixtures/get_lock.nostatus_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock.offline.json` & `yalexs-1.3.1/tests/fixtures/get_lock.offline.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock.online.json` & `yalexs-1.3.1/tests/fixtures/get_lock.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock.online_with_doorsense.json` & `yalexs-1.3.1/tests/fixtures/get_lock.online_with_doorsense.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock.online_with_doorsense_disabled.json` & `yalexs-1.3.1/tests/fixtures/get_lock.online_with_doorsense_disabled.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_lock_v2.online.json` & `yalexs-1.3.1/tests/fixtures/get_lock_v2.online.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/get_pins.json` & `yalexs-1.3.1/tests/fixtures/get_pins.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/keypad_lock_activity.json` & `yalexs-1.3.1/tests/fixtures/keypad_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/lock.json` & `yalexs-1.3.1/tests/fixtures/lock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/lock_activity.json` & `yalexs-1.3.1/tests/fixtures/lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/lock_without_doorstate.json` & `yalexs-1.3.1/tests/fixtures/lock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/remote_lock_activity.json` & `yalexs-1.3.1/tests/fixtures/remote_lock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/remote_unlock_activity_v4_2.json` & `yalexs-1.3.1/tests/fixtures/remote_unlock_activity_v4_2.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/unlock.json` & `yalexs-1.3.1/tests/fixtures/unlock.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/unlock_activity.json` & `yalexs-1.3.1/tests/fixtures/unlock_activity.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/fixtures/unlock_without_doorstate.json` & `yalexs-1.3.1/tests/fixtures/unlock_without_doorstate.json`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/test_activity.py` & `yalexs-1.3.1/tests/test_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     ACTION_DOORBELL_CALL_INITIATED,
     ACTION_DOORBELL_CALL_MISSED,
     ACTION_DOORBELL_IMAGE_CAPTURE,
     ACTION_DOORBELL_MOTION_DETECTED,
     ACTION_LOCK_AUTO_LOCK,
     ACTION_LOCK_BLE_LOCK,
     ACTION_LOCK_BLE_UNLOCK,
+    ACTION_LOCK_DOORBELL_BUTTON_PUSHED,
     ACTION_LOCK_JAMMED,
     ACTION_LOCK_LOCK,
     ACTION_LOCK_LOCKING,
     ACTION_LOCK_MANUAL_LOCK,
     ACTION_LOCK_MANUAL_UNLOCK,
     ACTION_LOCK_ONETOUCHLOCK,
     ACTION_LOCK_ONETOUCHLOCK_2,
@@ -76,14 +77,15 @@
     def test_activity_actions(self):
         self.assertCountEqual(
             ACTIVITY_ACTIONS_DOORBELL_DING,
             [
                 ACTION_DOORBELL_BUTTON_PUSHED,
                 ACTION_DOORBELL_CALL_MISSED,
                 ACTION_DOORBELL_CALL_HANGUP,
+                ACTION_LOCK_DOORBELL_BUTTON_PUSHED,
             ],
         )
         self.assertCountEqual(
             ACTIVITY_ACTIONS_DOORBELL_MOTION,
             [ACTION_DOORBELL_MOTION_DETECTED],
         )
         self.assertCountEqual(
```

### Comparing `yalexs-1.3.0/tests/test_api.py` & `yalexs-1.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/test_api_async.py` & `yalexs-1.3.1/tests/test_api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/test_authenticator.py` & `yalexs-1.3.1/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/test_authenticator_async.py` & `yalexs-1.3.1/tests/test_authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tests/test_pubnub_activity.py` & `yalexs-1.3.1/tests/test_pubnub_activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import unittest
 
 import dateutil.parser
+from dateutil.tz import tzlocal
 
 from yalexs.activity import (
     ActivityType,
     BridgeOperationActivity,
     DoorbellDingActivity,
     DoorbellImageCaptureActivity,
     DoorbellMotionActivity,
@@ -113,14 +114,17 @@
                     "wlanRSSI": -55,
                     "wlanSNR": 44,
                     "duration": 2534,
                 },
             },
         )
         assert isinstance(activities[0], LockOperationActivity)
+        assert activities[0].activity_start_time == dateutil.parser.parse(
+            "2021-03-20T18:19:06.372Z"
+        ).astimezone(tz=tzlocal()).replace(tzinfo=None)
         assert "LockOperationActivity" in str(activities[0])
         assert activities[0].action == "jammed"
 
         activities = activities_from_pubnub_message(
             lock,
             dateutil.parser.parse("2017-12-10T05:48:31.273Z"),
             {
@@ -141,14 +145,17 @@
                     "wlanSNR": 44,
                     "duration": 2534,
                 },
             },
         )
         assert isinstance(activities[0], LockOperationActivity)
         assert "LockOperationActivity" in str(activities[0])
+        assert activities[0].activity_start_time == dateutil.parser.parse(
+            "2021-03-20T18:19:06.372Z"
+        ).astimezone(tz=tzlocal()).replace(tzinfo=None)
         assert activities[0].action == "unlock"
 
         activities = activities_from_pubnub_message(
             lock,
             dateutil.parser.parse("2017-12-10T05:48:30.272Z"),
             {
                 "status": "locked",
```

### Comparing `yalexs-1.3.0/tests/test_util.py` & `yalexs-1.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/tox.ini` & `yalexs-1.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/activity.py` & `yalexs-1.3.1/yalexs/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,28 @@
 ACTION_DOOR_CLOSE_2 = "door_close"
 
 
 ACTION_DOORBELL_CALL_INITIATED = "doorbell_call_initiated"
 ACTION_DOORBELL_MOTION_DETECTED = "doorbell_motion_detected"
 ACTION_DOORBELL_CALL_MISSED = "doorbell_call_missed"
 ACTION_DOORBELL_CALL_HANGUP = "doorbell_call_hangup"
+ACTION_LOCK_DOORBELL_BUTTON_PUSHED = "lock_accessory_motion_detect"
 
 ACTION_BRIDGE_ONLINE = "associated_bridge_online"  # pubnub only
 ACTION_BRIDGE_OFFLINE = "associated_bridge_offline"  # pubnub only
 ACTION_DOORBELL_IMAGE_CAPTURE = "imagecapture"  # pubnub only
 ACTION_DOORBELL_BUTTON_PUSHED = "buttonpush"  # pubnub only
 
 ACTIVITY_ACTIONS_BRIDGE_OPERATION = {ACTION_BRIDGE_ONLINE, ACTION_BRIDGE_OFFLINE}
 
 ACTIVITY_ACTIONS_DOORBELL_DING = {
     ACTION_DOORBELL_BUTTON_PUSHED,
     ACTION_DOORBELL_CALL_MISSED,
     ACTION_DOORBELL_CALL_HANGUP,
+    ACTION_LOCK_DOORBELL_BUTTON_PUSHED,
 }
 ACTIVITY_ACTIONS_DOORBELL_IMAGE_CAPTURE = {ACTION_DOORBELL_IMAGE_CAPTURE}
 ACTIVITY_ACTIONS_DOORBELL_MOTION = {ACTION_DOORBELL_MOTION_DETECTED}
 ACTIVITY_ACTIONS_DOORBELL_VIEW = {ACTION_DOORBELL_CALL_INITIATED}
 ACTIVITY_ACTIONS_LOCK_OPERATION = {
     ACTION_RF_SECURE,
     ACTION_RF_LOCK,
```

### Comparing `yalexs-1.3.0/yalexs/api.py` & `yalexs-1.3.1/yalexs/api.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/api_async.py` & `yalexs-1.3.1/yalexs/api_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/api_common.py` & `yalexs-1.3.1/yalexs/api_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/authenticator.py` & `yalexs-1.3.1/yalexs/authenticator.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/authenticator_async.py` & `yalexs-1.3.1/yalexs/authenticator_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/authenticator_common.py` & `yalexs-1.3.1/yalexs/authenticator_common.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/bridge.py` & `yalexs-1.3.1/yalexs/bridge.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/device.py` & `yalexs-1.3.1/yalexs/device.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/doorbell.py` & `yalexs-1.3.1/yalexs/doorbell.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/keypad.py` & `yalexs-1.3.1/yalexs/keypad.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/lock.py` & `yalexs-1.3.1/yalexs/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/pin.py` & `yalexs-1.3.1/yalexs/pin.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/pubnub_activity.py` & `yalexs-1.3.1/yalexs/pubnub_activity.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,31 +24,40 @@
     LockDetail,
     LockDoorStatus,
     LockStatus,
     determine_door_state,
     determine_lock_status,
 )
 
+from .api_common import _datetime_string_to_epoch
 from .device import Device
 
 
 def activities_from_pubnub_message(
     device: Device, date_time: datetime, message: Dict[str, Any]
 ):
     """Create activities from pubnub."""
     activities = []
     activity_dict = {
         "deviceID": device.device_id,
         "house": device.house_id,
-        "dateTime": date_time.timestamp() * 1000,
         "deviceName": device.device_name,
     }
+    info = message.get("info", {})
+    context = info.get("context", {})
+    if "startDate" in context:
+        activity_dict["dateTime"] = _datetime_string_to_epoch(context["startDate"])
+    elif "startTime" in info:
+        activity_dict["dateTime"] = _datetime_string_to_epoch(info["startTime"])
+    else:
+        activity_dict["dateTime"] = date_time.timestamp() * 1000
+
     if isinstance(device, LockDetail):
         activity_dict["deviceType"] = "lock"
-        activity_dict["info"] = message.get("info", {})
+        activity_dict["info"] = info
         calling_user_id = message.get("callingUserID")
         if calling_user_id:
             activity_dict["callingUser"] = {"UserID": calling_user_id}
         if "remoteEvent" in message:
             activity_dict["info"]["remote"] = True
 
         if LOCK_STATUS_KEY in message:
```

### Comparing `yalexs-1.3.0/yalexs/pubnub_async.py` & `yalexs-1.3.1/yalexs/pubnub_async.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/users.py` & `yalexs-1.3.1/yalexs/users.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs/util.py` & `yalexs-1.3.1/yalexs/util.py`

 * *Files identical despite different names*

### Comparing `yalexs-1.3.0/yalexs.egg-info/PKG-INFO` & `yalexs-1.3.1/yalexs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API for Yale Access (formerly August) Smart Lock and Doorbell
 Home-page: https://github.com/bdraco/yalexs
 Author: bdraco
 Author-email: nick@koston.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yalexs-1.3.0/yalexs.egg-info/SOURCES.txt` & `yalexs-1.3.1/yalexs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

