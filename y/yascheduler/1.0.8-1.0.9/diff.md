# Comparing `tmp/yascheduler-1.0.8.tar.gz` & `tmp/yascheduler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yascheduler-1.0.8.tar", last modified: Sun Apr 16 16:14:21 2023, max compression
+gzip compressed data, was "yascheduler-1.0.9.tar", last modified: Mon Apr 24 19:43:08 2023, max compression
```

## Comparing `yascheduler-1.0.8.tar` & `yascheduler-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.667817 yascheduler-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-16 16:14:21.667817 yascheduler-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10424 2023-03-08 16:11:57.000000 yascheduler-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-16 16:14:21.667817 yascheduler-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1972 2022-08-17 12:59:28.000000 yascheduler-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.659817 yascheduler-1.0.8/yascheduler/
--rw-r--r--   0 root         (0) root         (0)      228 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-10 23:58:05.000000 yascheduler-1.0.8/yascheduler/__version__.py
--rw-r--r--   0 root         (0) root         (0)     4747 2022-09-26 15:10:05.000000 yascheduler-1.0.8/yascheduler/aiida_plugin.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-08-01 14:38:59.000000 yascheduler-1.0.8/yascheduler/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.659817 yascheduler-1.0.8/yascheduler/clouds/
--rw-r--r--   0 root         (0) root         (0)      170 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/clouds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2981 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/adapters.py
--rw-r--r--   0 root         (0) root         (0)     8736 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/az.py
--rw-r--r--   0 root         (0) root         (0)     6867 2022-08-16 14:53:47.000000 yascheduler-1.0.8/yascheduler/clouds/cloud_api.py
--rw-r--r--   0 root         (0) root         (0)     6821 2022-08-16 14:53:47.000000 yascheduler-1.0.8/yascheduler/clouds/cloud_api_manager.py
--rw-r--r--   0 root         (0) root         (0)     3282 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/hetzner.py
--rw-r--r--   0 root         (0) root         (0)     5802 2022-08-16 14:53:47.000000 yascheduler-1.0.8/yascheduler/clouds/protocols.py
--rw-r--r--   0 root         (0) root         (0)     2831 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/upcloud.py
--rw-r--r--   0 root         (0) root         (0)      763 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/clouds/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.663817 yascheduler-1.0.8/yascheduler/config/
--rw-r--r--   0 root         (0) root         (0)      731 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6408 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/config/cloud.py
--rw-r--r--   0 root         (0) root         (0)     2438 2022-08-17 12:59:28.000000 yascheduler-1.0.8/yascheduler/config/config.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/db.py
--rw-r--r--   0 root         (0) root         (0)     4917 2022-08-01 15:25:53.000000 yascheduler-1.0.8/yascheduler/config/engine.py
--rw-r--r--   0 root         (0) root         (0)     2635 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/engine_repository.py
--rw-r--r--   0 root         (0) root         (0)     2844 2022-08-02 17:38:08.000000 yascheduler-1.0.8/yascheduler/config/local.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/remote.py
--rw-r--r--   0 root         (0) root         (0)      484 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/config/utils.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-30 22:43:26.000000 yascheduler-1.0.8/yascheduler/daemon_systemd.py
--rw-r--r--   0 root         (0) root         (0)      864 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/daemon_sysv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.663817 yascheduler-1.0.8/yascheduler/data/
--rw-r--r--   0 root         (0) root         (0)      360 2023-02-09 18:58:39.000000 yascheduler-1.0.8/yascheduler/data/schema.sql
--rw-r--r--   0 root         (0) root         (0)     1493 2022-07-30 22:43:26.000000 yascheduler-1.0.8/yascheduler/data/yascheduler.conf
--rw-r--r--   0 root         (0) root         (0)      664 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/data/yascheduler.service
--rwxr-xr-x   0 root         (0) root         (0)     1832 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/data/yascheduler.sh
--rw-r--r--   0 root         (0) root         (0)    12108 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/db.py
--rw-r--r--   0 root         (0) root         (0)     1651 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.667817 yascheduler-1.0.8/yascheduler/remote_machine/
--rw-r--r--   0 root         (0) root         (0)      417 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/remote_machine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3271 2022-08-17 12:59:28.000000 yascheduler-1.0.8/yascheduler/remote_machine/adapters.py
--rw-r--r--   0 root         (0) root         (0)     2338 2022-08-17 12:59:28.000000 yascheduler-1.0.8/yascheduler/remote_machine/checks.py
--rw-r--r--   0 root         (0) root         (0)     1213 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/remote_machine/common.py
--rw-r--r--   0 root         (0) root         (0)       72 2022-07-30 22:43:26.000000 yascheduler-1.0.8/yascheduler/remote_machine/exc.py
--rw-r--r--   0 root         (0) root         (0)     6980 2022-08-03 22:43:25.000000 yascheduler-1.0.8/yascheduler/remote_machine/linux_methods.py
--rw-r--r--   0 root         (0) root         (0)     8641 2022-08-16 21:24:49.000000 yascheduler-1.0.8/yascheduler/remote_machine/protocol.py
--rw-r--r--   0 root         (0) root         (0)    13207 2023-03-10 23:58:05.000000 yascheduler-1.0.8/yascheduler/remote_machine/remote_machine.py
--rw-r--r--   0 root         (0) root         (0)     2655 2022-07-30 22:43:35.000000 yascheduler-1.0.8/yascheduler/remote_machine/remote_machine_repository.py
--rw-r--r--   0 root         (0) root         (0)     7288 2022-08-03 22:43:25.000000 yascheduler-1.0.8/yascheduler/remote_machine/windows_methods.py
--rwxr-xr-x   0 root         (0) root         (0)    26345 2023-03-10 23:59:11.000000 yascheduler-1.0.8/yascheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)      435 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/time.py
--rw-r--r--   0 root         (0) root         (0)    15688 2023-03-08 16:11:57.000000 yascheduler-1.0.8/yascheduler/utils.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-08-01 13:33:43.000000 yascheduler-1.0.8/yascheduler/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:21.659817 yascheduler-1.0.8/yascheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      235 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 16:14:21.000000 yascheduler-1.0.8/yascheduler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.812351 yascheduler-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-24 19:43:01.000000 yascheduler-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-24 19:43:08.812351 yascheduler-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10424 2023-03-08 16:11:57.000000 yascheduler-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-24 19:43:08.812351 yascheduler-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1576 2022-07-30 22:43:35.000000 yascheduler-1.0.9/setup.json
+-rw-r--r--   0 root         (0) root         (0)     1972 2022-08-17 12:59:28.000000 yascheduler-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/
+-rw-r--r--   0 root         (0) root         (0)      228 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-24 19:38:14.000000 yascheduler-1.0.9/yascheduler/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2022-09-26 15:10:05.000000 yascheduler-1.0.9/yascheduler/aiida_plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2022-08-01 14:38:59.000000 yascheduler-1.0.9/yascheduler/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/clouds/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/clouds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/adapters.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/az.py
+-rw-r--r--   0 root         (0) root         (0)     6867 2022-08-16 14:53:47.000000 yascheduler-1.0.9/yascheduler/clouds/cloud_api.py
+-rw-r--r--   0 root         (0) root         (0)     6821 2022-08-16 14:53:47.000000 yascheduler-1.0.9/yascheduler/clouds/cloud_api_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/hetzner.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2022-08-16 14:53:47.000000 yascheduler-1.0.9/yascheduler/clouds/protocols.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/upcloud.py
+-rw-r--r--   0 root         (0) root         (0)      763 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/clouds/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/config/
+-rw-r--r--   0 root         (0) root         (0)      731 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/config/cloud.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2022-08-17 12:59:28.000000 yascheduler-1.0.9/yascheduler/config/config.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/db.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2022-08-01 15:25:53.000000 yascheduler-1.0.9/yascheduler/config/engine.py
+-rw-r--r--   0 root         (0) root         (0)     2635 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/engine_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2022-08-02 17:38:08.000000 yascheduler-1.0.9/yascheduler/config/local.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/remote.py
+-rw-r--r--   0 root         (0) root         (0)      484 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/config/utils.py
+-rw-r--r--   0 root         (0) root         (0)      200 2022-07-30 22:43:26.000000 yascheduler-1.0.9/yascheduler/daemon_systemd.py
+-rw-r--r--   0 root         (0) root         (0)      864 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/daemon_sysv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler/data/
+-rw-r--r--   0 root         (0) root         (0)      360 2023-02-09 18:58:39.000000 yascheduler-1.0.9/yascheduler/data/schema.sql
+-rw-r--r--   0 root         (0) root         (0)     1493 2022-07-30 22:43:26.000000 yascheduler-1.0.9/yascheduler/data/yascheduler.conf
+-rw-r--r--   0 root         (0) root         (0)      664 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/data/yascheduler.service
+-rwxr-xr-x   0 root         (0) root         (0)     1832 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/data/yascheduler.sh
+-rw-r--r--   0 root         (0) root         (0)    12108 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/db.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.812351 yascheduler-1.0.9/yascheduler/remote_machine/
+-rw-r--r--   0 root         (0) root         (0)      417 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/remote_machine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-08-17 12:59:28.000000 yascheduler-1.0.9/yascheduler/remote_machine/adapters.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2022-08-17 12:59:28.000000 yascheduler-1.0.9/yascheduler/remote_machine/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/remote_machine/common.py
+-rw-r--r--   0 root         (0) root         (0)       72 2022-07-30 22:43:26.000000 yascheduler-1.0.9/yascheduler/remote_machine/exc.py
+-rw-r--r--   0 root         (0) root         (0)     6980 2022-08-03 22:43:25.000000 yascheduler-1.0.9/yascheduler/remote_machine/linux_methods.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2022-08-16 21:24:49.000000 yascheduler-1.0.9/yascheduler/remote_machine/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    13207 2023-03-10 23:58:05.000000 yascheduler-1.0.9/yascheduler/remote_machine/remote_machine.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2022-07-30 22:43:35.000000 yascheduler-1.0.9/yascheduler/remote_machine/remote_machine_repository.py
+-rw-r--r--   0 root         (0) root         (0)     7288 2022-08-03 22:43:25.000000 yascheduler-1.0.9/yascheduler/remote_machine/windows_methods.py
+-rwxr-xr-x   0 root         (0) root         (0)    26345 2023-03-10 23:59:11.000000 yascheduler-1.0.9/yascheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)      435 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/time.py
+-rw-r--r--   0 root         (0) root         (0)    15688 2023-03-08 16:11:57.000000 yascheduler-1.0.9/yascheduler/utils.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-08-01 13:33:43.000000 yascheduler-1.0.9/yascheduler/variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:43:08.808351 yascheduler-1.0.9/yascheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      235 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 19:43:08.000000 yascheduler-1.0.9/yascheduler.egg-info/top_level.txt
```

### Comparing `yascheduler-1.0.8/PKG-INFO` & `yascheduler-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yascheduler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Yet another computing scheduler and cloud orchestration engine
 Home-page: https://github.com/tilde-lab/yascheduler
 Author: Sergey Korolev, Evgeny Blokhin, Andrey Sobolev
 Author-email: eb@tilde.pro
 License: MIT
 Description: *Yascheduler* is a job scheduler designed for submitting scientific simulations to the VM clouds and copying back their results.
 Platform: UNKNOWN
```

### Comparing `yascheduler-1.0.8/README.md` & `yascheduler-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/setup.py` & `yascheduler-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/aiida_plugin.py` & `yascheduler-1.0.9/yascheduler/aiida_plugin.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/client.py` & `yascheduler-1.0.9/yascheduler/client.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/adapters.py` & `yascheduler-1.0.9/yascheduler/clouds/adapters.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/az.py` & `yascheduler-1.0.9/yascheduler/clouds/az.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/cloud_api.py` & `yascheduler-1.0.9/yascheduler/clouds/cloud_api.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/cloud_api_manager.py` & `yascheduler-1.0.9/yascheduler/clouds/cloud_api_manager.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/hetzner.py` & `yascheduler-1.0.9/yascheduler/clouds/hetzner.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/protocols.py` & `yascheduler-1.0.9/yascheduler/clouds/protocols.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/upcloud.py` & `yascheduler-1.0.9/yascheduler/clouds/upcloud.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/clouds/utils.py` & `yascheduler-1.0.9/yascheduler/clouds/utils.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/__init__.py` & `yascheduler-1.0.9/yascheduler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/cloud.py` & `yascheduler-1.0.9/yascheduler/config/cloud.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/config.py` & `yascheduler-1.0.9/yascheduler/config/config.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/db.py` & `yascheduler-1.0.9/yascheduler/config/db.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/engine.py` & `yascheduler-1.0.9/yascheduler/config/engine.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/engine_repository.py` & `yascheduler-1.0.9/yascheduler/config/engine_repository.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/local.py` & `yascheduler-1.0.9/yascheduler/config/local.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/config/remote.py` & `yascheduler-1.0.9/yascheduler/config/remote.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/daemon_sysv.py` & `yascheduler-1.0.9/yascheduler/daemon_sysv.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/data/yascheduler.conf` & `yascheduler-1.0.9/yascheduler/data/yascheduler.conf`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/data/yascheduler.service` & `yascheduler-1.0.9/yascheduler/data/yascheduler.service`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/data/yascheduler.sh` & `yascheduler-1.0.9/yascheduler/data/yascheduler.sh`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/db.py` & `yascheduler-1.0.9/yascheduler/db.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/queue.py` & `yascheduler-1.0.9/yascheduler/queue.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/adapters.py` & `yascheduler-1.0.9/yascheduler/remote_machine/adapters.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/checks.py` & `yascheduler-1.0.9/yascheduler/remote_machine/checks.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/common.py` & `yascheduler-1.0.9/yascheduler/remote_machine/common.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/linux_methods.py` & `yascheduler-1.0.9/yascheduler/remote_machine/linux_methods.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/protocol.py` & `yascheduler-1.0.9/yascheduler/remote_machine/protocol.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/remote_machine.py` & `yascheduler-1.0.9/yascheduler/remote_machine/remote_machine.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/remote_machine_repository.py` & `yascheduler-1.0.9/yascheduler/remote_machine/remote_machine_repository.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/remote_machine/windows_methods.py` & `yascheduler-1.0.9/yascheduler/remote_machine/windows_methods.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/scheduler.py` & `yascheduler-1.0.9/yascheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler/utils.py` & `yascheduler-1.0.9/yascheduler/utils.py`

 * *Files identical despite different names*

### Comparing `yascheduler-1.0.8/yascheduler.egg-info/PKG-INFO` & `yascheduler-1.0.9/yascheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yascheduler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Yet another computing scheduler and cloud orchestration engine
 Home-page: https://github.com/tilde-lab/yascheduler
 Author: Sergey Korolev, Evgeny Blokhin, Andrey Sobolev
 Author-email: eb@tilde.pro
 License: MIT
 Description: *Yascheduler* is a job scheduler designed for submitting scientific simulations to the VM clouds and copying back their results.
 Platform: UNKNOWN
```

### Comparing `yascheduler-1.0.8/yascheduler.egg-info/SOURCES.txt` & `yascheduler-1.0.9/yascheduler.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+MANIFEST.in
 README.md
 setup.cfg
+setup.json
 setup.py
 yascheduler/__init__.py
 yascheduler/__version__.py
 yascheduler/aiida_plugin.py
 yascheduler/client.py
 yascheduler/daemon_systemd.py
 yascheduler/daemon_sysv.py
```

