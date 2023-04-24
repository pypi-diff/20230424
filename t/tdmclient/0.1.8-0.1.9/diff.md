# Comparing `tmp/tdmclient-0.1.8.tar.gz` & `tmp/tdmclient-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdmclient-0.1.8.tar", last modified: Wed Oct 13 13:54:57 2021, max compression
+gzip compressed data, was "tdmclient-0.1.9.tar", last modified: Wed Oct 20 13:32:36 2021, max compression
```

## Comparing `tdmclient-0.1.8.tar` & `tdmclient-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.398844 tdmclient-0.1.8/
--rw-rw-rw-   0        0        0     4705 2021-10-13 13:45:14.000000 tdmclient-0.1.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1529 2021-03-16 09:02:40.000000 tdmclient-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      680 2021-10-13 13:32:21.000000 tdmclient-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    65119 2021-10-13 13:54:57.398844 tdmclient-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2021-02-11 10:02:03.000000 tdmclient-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.290761 tdmclient-0.1.8/doc/
--rw-rw-rw-   0        0        0    15266 2021-10-13 11:56:00.000000 tdmclient-0.1.8/doc/help.md
--rw-rw-rw-   0        0        0    18526 2021-10-13 13:05:17.000000 tdmclient-0.1.8/doc/notebooks.md
--rw-rw-rw-   0        0        0     7527 2021-09-28 07:55:29.000000 tdmclient-0.1.8/doc/repl.md
--rw-rw-rw-   0        0        0    21966 2021-10-07 15:07:06.000000 tdmclient-0.1.8/doc/transpiler.md
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.260795 tdmclient-0.1.8/examples/
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.294757 tdmclient-0.1.8/examples/host/
--rw-rw-rw-   0        0        0     1373 2021-04-08 08:59:47.000000 tdmclient-0.1.8/examples/host/events.py
--rw-rw-rw-   0        0        0      960 2021-03-16 09:02:50.000000 tdmclient-0.1.8/examples/host/runprogram.py
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.310838 tdmclient-0.1.8/examples/robot/
--rw-rw-rw-   0        0        0      161 2021-09-13 09:18:08.000000 tdmclient-0.1.8/examples/robot/acquisition.py
--rw-rw-rw-   0        0        0      214 2021-04-12 09:26:01.000000 tdmclient-0.1.8/examples/robot/backward.py
--rw-rw-rw-   0        0        0      163 2021-03-15 08:08:23.000000 tdmclient-0.1.8/examples/robot/blink.aseba
--rw-rw-rw-   0        0        0      179 2021-04-12 09:26:27.000000 tdmclient-0.1.8/examples/robot/blink.py
--rw-rw-rw-   0        0        0       22 2021-03-15 08:03:07.000000 tdmclient-0.1.8/examples/robot/blue.aseba
--rw-rw-rw-   0        0        0      290 2021-10-07 14:07:09.000000 tdmclient-0.1.8/examples/robot/clock.py
--rw-rw-rw-   0        0        0      209 2021-09-08 08:37:12.000000 tdmclient-0.1.8/examples/robot/exit.py
--rw-rw-rw-   0        0        0      319 2021-09-08 08:34:34.000000 tdmclient-0.1.8/examples/robot/print.py
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.319754 tdmclient-0.1.8/notebooks/
--rw-rw-rw-   0        0        0     9397 2021-08-26 09:25:41.000000 tdmclient-0.1.8/notebooks/tdmclient_intro.ipynb
--rw-rw-rw-   0        0        0    13271 2021-10-13 12:44:06.000000 tdmclient-0.1.8/notebooks/tdmclient_sync.ipynb
--rw-rw-rw-   0        0        0     9486 2021-10-12 17:03:11.000000 tdmclient-0.1.8/notebooks/tdmclient_sync_adv.ipynb
--rw-rw-rw-   0        0        0    14117 2021-10-13 13:04:47.000000 tdmclient-0.1.8/notebooks/tdmclient_sync_interact.ipynb
--rw-rw-rw-   0        0        0    20844 2021-09-27 12:09:38.000000 tdmclient-0.1.8/notebooks/tdmclient_sync_nf.ipynb
--rw-rw-rw-   0        0        0       42 2021-10-13 13:54:57.399842 tdmclient-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1139 2021-10-13 13:45:39.000000 tdmclient-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.346353 tdmclient-0.1.8/tdmclient/
--rw-rw-rw-   0        0        0      795 2021-04-27 21:10:39.000000 tdmclient-0.1.8/tdmclient/__init__.py
--rw-rw-rw-   0        0        0    56444 2021-10-13 08:43:40.000000 tdmclient-0.1.8/tdmclient/atranspiler.py
--rw-rw-rw-   0        0        0     4017 2021-04-16 08:21:12.000000 tdmclient-0.1.8/tdmclient/client.py
--rw-rw-rw-   0        0        0     5126 2021-09-09 13:24:01.000000 tdmclient-0.1.8/tdmclient/clientasync.py
--rw-rw-rw-   0        0        0     5331 2021-10-05 08:50:20.000000 tdmclient-0.1.8/tdmclient/clientasynccachenode.py
--rw-rw-rw-   0        0        0     5259 2021-04-16 08:12:20.000000 tdmclient-0.1.8/tdmclient/clientasyncnode.py
--rw-rw-rw-   0        0        0     3104 2021-04-29 15:56:31.000000 tdmclient-0.1.8/tdmclient/clientnode.py
--rw-rw-rw-   0        0        0    23562 2021-06-24 09:00:38.000000 tdmclient-0.1.8/tdmclient/fb.py
--rw-rw-rw-   0        0        0     1036 2021-10-13 08:33:13.000000 tdmclient-0.1.8/tdmclient/module_clock.py
--rw-rw-rw-   0        0        0    17130 2021-10-07 12:16:30.000000 tdmclient-0.1.8/tdmclient/module_thymio.py
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.374009 tdmclient-0.1.8/tdmclient/notebook/
--rw-rw-rw-   0        0        0     7459 2021-10-13 12:44:56.000000 tdmclient-0.1.8/tdmclient/notebook/__init__.py
--rw-rw-rw-   0        0        0    27758 2021-10-13 07:31:06.000000 tdmclient-0.1.8/tdmclient/repl.py
--rw-rw-rw-   0        0        0    19095 2021-10-04 07:23:47.000000 tdmclient-0.1.8/tdmclient/server.py
--rw-rw-rw-   0        0        0     5250 2021-04-12 07:14:16.000000 tdmclient-0.1.8/tdmclient/tcp.py
--rw-rw-rw-   0        0        0    29445 2021-10-07 07:57:10.000000 tdmclient-0.1.8/tdmclient/thymio.py
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.395844 tdmclient-0.1.8/tdmclient/tools/
--rw-rw-rw-   0        0        0       70 2021-04-27 08:41:09.000000 tdmclient-0.1.8/tdmclient/tools/__init__.py
--rw-rw-rw-   0        0        0    21407 2021-05-05 14:09:44.000000 tdmclient-0.1.8/tdmclient/tools/gui.py
--rw-rw-rw-   0        0        0     3386 2021-05-05 16:03:41.000000 tdmclient-0.1.8/tdmclient/tools/list.py
--rw-rw-rw-   0        0        0     2433 2021-10-04 07:23:47.000000 tdmclient-0.1.8/tdmclient/tools/repl.py
--rw-rw-rw-   0        0        0     9011 2021-10-07 12:18:54.000000 tdmclient-0.1.8/tdmclient/tools/run.py
--rw-rw-rw-   0        0        0     1440 2021-09-08 08:20:25.000000 tdmclient-0.1.8/tdmclient/tools/server.py
--rw-rw-rw-   0        0        0      545 2021-03-16 08:53:29.000000 tdmclient-0.1.8/tdmclient/tools/tdmdiscovery.py
--rw-rw-rw-   0        0        0     2683 2021-10-07 12:22:31.000000 tdmclient-0.1.8/tdmclient/tools/transpile.py
--rw-rw-rw-   0        0        0      535 2021-03-23 13:32:51.000000 tdmclient-0.1.8/tdmclient/tools/watch.py
--rw-rw-rw-   0        0        0      662 2021-05-04 08:45:18.000000 tdmclient-0.1.8/tdmclient/ws.py
--rw-rw-rw-   0        0        0     1765 2021-09-22 14:49:28.000000 tdmclient-0.1.8/tdmclient/zeroconf.py
-drwxrwxrwx   0        0        0        0 2021-10-13 13:54:57.374009 tdmclient-0.1.8/tdmclient.egg-info/
--rw-rw-rw-   0        0        0    65119 2021-10-13 13:54:57.000000 tdmclient-0.1.8/tdmclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1329 2021-10-13 13:54:57.000000 tdmclient-0.1.8/tdmclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-13 13:54:57.000000 tdmclient-0.1.8/tdmclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-10-13 13:54:57.000000 tdmclient-0.1.8/tdmclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-10-13 13:54:57.000000 tdmclient-0.1.8/tdmclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.518096 tdmclient-0.1.9/
+-rw-rw-rw-   0        0        0     5037 2021-10-20 13:30:24.000000 tdmclient-0.1.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1529 2021-03-16 09:02:40.000000 tdmclient-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      680 2021-10-13 13:32:21.000000 tdmclient-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    65119 2021-10-20 13:32:36.517094 tdmclient-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2021-02-11 10:02:03.000000 tdmclient-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.422100 tdmclient-0.1.9/doc/
+-rw-rw-rw-   0        0        0    15266 2021-10-13 11:56:00.000000 tdmclient-0.1.9/doc/help.md
+-rw-rw-rw-   0        0        0    18526 2021-10-13 13:05:17.000000 tdmclient-0.1.9/doc/notebooks.md
+-rw-rw-rw-   0        0        0     7527 2021-09-28 07:55:29.000000 tdmclient-0.1.9/doc/repl.md
+-rw-rw-rw-   0        0        0    21966 2021-10-07 15:07:06.000000 tdmclient-0.1.9/doc/transpiler.md
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.404093 tdmclient-0.1.9/examples/
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.425094 tdmclient-0.1.9/examples/host/
+-rw-rw-rw-   0        0        0     1373 2021-04-08 08:59:47.000000 tdmclient-0.1.9/examples/host/events.py
+-rw-rw-rw-   0        0        0      960 2021-03-16 09:02:50.000000 tdmclient-0.1.9/examples/host/runprogram.py
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.436094 tdmclient-0.1.9/examples/robot/
+-rw-rw-rw-   0        0        0      161 2021-09-13 09:18:08.000000 tdmclient-0.1.9/examples/robot/acquisition.py
+-rw-rw-rw-   0        0        0      214 2021-04-12 09:26:01.000000 tdmclient-0.1.9/examples/robot/backward.py
+-rw-rw-rw-   0        0        0      163 2021-03-15 08:08:23.000000 tdmclient-0.1.9/examples/robot/blink.aseba
+-rw-rw-rw-   0        0        0      179 2021-04-12 09:26:27.000000 tdmclient-0.1.9/examples/robot/blink.py
+-rw-rw-rw-   0        0        0       22 2021-03-15 08:03:07.000000 tdmclient-0.1.9/examples/robot/blue.aseba
+-rw-rw-rw-   0        0        0      290 2021-10-07 14:07:09.000000 tdmclient-0.1.9/examples/robot/clock.py
+-rw-rw-rw-   0        0        0      209 2021-09-08 08:37:12.000000 tdmclient-0.1.9/examples/robot/exit.py
+-rw-rw-rw-   0        0        0      319 2021-09-08 08:34:34.000000 tdmclient-0.1.9/examples/robot/print.py
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.444095 tdmclient-0.1.9/notebooks/
+-rw-rw-rw-   0        0        0     9397 2021-08-26 09:25:41.000000 tdmclient-0.1.9/notebooks/tdmclient_intro.ipynb
+-rw-rw-rw-   0        0        0    13271 2021-10-13 12:44:06.000000 tdmclient-0.1.9/notebooks/tdmclient_sync.ipynb
+-rw-rw-rw-   0        0        0     9486 2021-10-12 17:03:11.000000 tdmclient-0.1.9/notebooks/tdmclient_sync_adv.ipynb
+-rw-rw-rw-   0        0        0     7297 2021-10-20 13:29:51.000000 tdmclient-0.1.9/notebooks/tdmclient_sync_interact.ipynb
+-rw-rw-rw-   0        0        0    20844 2021-09-27 12:09:38.000000 tdmclient-0.1.9/notebooks/tdmclient_sync_nf.ipynb
+-rw-rw-rw-   0        0        0       42 2021-10-20 13:32:36.518096 tdmclient-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2021-10-20 13:30:44.000000 tdmclient-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.470094 tdmclient-0.1.9/tdmclient/
+-rw-rw-rw-   0        0        0      795 2021-04-27 21:10:39.000000 tdmclient-0.1.9/tdmclient/__init__.py
+-rw-rw-rw-   0        0        0    56457 2021-10-18 10:16:32.000000 tdmclient-0.1.9/tdmclient/atranspiler.py
+-rw-rw-rw-   0        0        0     4017 2021-04-16 08:21:12.000000 tdmclient-0.1.9/tdmclient/client.py
+-rw-rw-rw-   0        0        0     5126 2021-09-09 13:24:01.000000 tdmclient-0.1.9/tdmclient/clientasync.py
+-rw-rw-rw-   0        0        0     5331 2021-10-05 08:50:20.000000 tdmclient-0.1.9/tdmclient/clientasynccachenode.py
+-rw-rw-rw-   0        0        0     5259 2021-04-16 08:12:20.000000 tdmclient-0.1.9/tdmclient/clientasyncnode.py
+-rw-rw-rw-   0        0        0     3104 2021-04-29 15:56:31.000000 tdmclient-0.1.9/tdmclient/clientnode.py
+-rw-rw-rw-   0        0        0    23562 2021-06-24 09:00:38.000000 tdmclient-0.1.9/tdmclient/fb.py
+-rw-rw-rw-   0        0        0     1036 2021-10-13 08:33:13.000000 tdmclient-0.1.9/tdmclient/module_clock.py
+-rw-rw-rw-   0        0        0    17130 2021-10-07 12:16:30.000000 tdmclient-0.1.9/tdmclient/module_thymio.py
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.501094 tdmclient-0.1.9/tdmclient/notebook/
+-rw-rw-rw-   0        0        0     7587 2021-10-20 13:14:24.000000 tdmclient-0.1.9/tdmclient/notebook/__init__.py
+-rw-rw-rw-   0        0        0    28676 2021-10-20 13:18:01.000000 tdmclient-0.1.9/tdmclient/repl.py
+-rw-rw-rw-   0        0        0    19095 2021-10-04 07:23:47.000000 tdmclient-0.1.9/tdmclient/server.py
+-rw-rw-rw-   0        0        0     5250 2021-04-12 07:14:16.000000 tdmclient-0.1.9/tdmclient/tcp.py
+-rw-rw-rw-   0        0        0    29445 2021-10-07 07:57:10.000000 tdmclient-0.1.9/tdmclient/thymio.py
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.515093 tdmclient-0.1.9/tdmclient/tools/
+-rw-rw-rw-   0        0        0       70 2021-04-27 08:41:09.000000 tdmclient-0.1.9/tdmclient/tools/__init__.py
+-rw-rw-rw-   0        0        0    21407 2021-05-05 14:09:44.000000 tdmclient-0.1.9/tdmclient/tools/gui.py
+-rw-rw-rw-   0        0        0     3386 2021-05-05 16:03:41.000000 tdmclient-0.1.9/tdmclient/tools/list.py
+-rw-rw-rw-   0        0        0     2595 2021-10-18 14:20:06.000000 tdmclient-0.1.9/tdmclient/tools/repl.py
+-rw-rw-rw-   0        0        0     9011 2021-10-18 10:07:42.000000 tdmclient-0.1.9/tdmclient/tools/run.py
+-rw-rw-rw-   0        0        0     1440 2021-09-08 08:20:25.000000 tdmclient-0.1.9/tdmclient/tools/server.py
+-rw-rw-rw-   0        0        0      545 2021-03-16 08:53:29.000000 tdmclient-0.1.9/tdmclient/tools/tdmdiscovery.py
+-rw-rw-rw-   0        0        0     2683 2021-10-07 12:22:31.000000 tdmclient-0.1.9/tdmclient/tools/transpile.py
+-rw-rw-rw-   0        0        0      535 2021-03-23 13:32:51.000000 tdmclient-0.1.9/tdmclient/tools/watch.py
+-rw-rw-rw-   0        0        0      662 2021-05-04 08:45:18.000000 tdmclient-0.1.9/tdmclient/ws.py
+-rw-rw-rw-   0        0        0     1765 2021-09-22 14:49:28.000000 tdmclient-0.1.9/tdmclient/zeroconf.py
+drwxrwxrwx   0        0        0        0 2021-10-20 13:32:36.499095 tdmclient-0.1.9/tdmclient.egg-info/
+-rw-rw-rw-   0        0        0    65119 2021-10-20 13:32:35.000000 tdmclient-0.1.9/tdmclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2021-10-20 13:32:35.000000 tdmclient-0.1.9/tdmclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-10-20 13:32:35.000000 tdmclient-0.1.9/tdmclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2021-10-20 13:32:35.000000 tdmclient-0.1.9/tdmclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-10-20 13:32:35.000000 tdmclient-0.1.9/tdmclient.egg-info/top_level.txt
```

### Comparing `tdmclient-0.1.8/CHANGELOG.md` & `tdmclient-0.1.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # Changelog
 
 Notable changes of tdmclient. Release versions refer to [https://pypi.org/project/tdmclient/].
 
 ## [Unreleased]
 
+## [0.1.9] - 2021-10-20
+
+### Added
+
+- In `tdmclient.tools.repl`, launch code moved to a function `main(argv=None)` so that it can be called from the Python shell
+- In repl and notebooks, shortened message when interrupting program
+
+### Fixed
+
+- In transpiler, module "clock" fixed
+- In repl, better support for Python 3.6 and 3.10
+
 ## [0.1.8] - 2021-10-13
 
 ### Added
 
 - In transpiler:
 	- module `clock` with functions `seconds()`, `ticks_50Hz()` and `reset()`
 - In repl:
```

### Comparing `tdmclient-0.1.8/LICENSE` & `tdmclient-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/MANIFEST.in` & `tdmclient-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/PKG-INFO` & `tdmclient-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdmclient
-Version: 0.1.8
+Version: 0.1.9
 Summary: Communication with Thymio II robot via the Thymio Device Manager
 Home-page: https://github.com/epfl-mobots/tdm-python
 Author: Yves Piguet
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tdmclient-0.1.8/README.md` & `tdmclient-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/doc/help.md` & `tdmclient-0.1.9/doc/help.md`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/doc/notebooks.md` & `tdmclient-0.1.9/doc/notebooks.md`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/doc/repl.md` & `tdmclient-0.1.9/doc/repl.md`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/doc/transpiler.md` & `tdmclient-0.1.9/doc/transpiler.md`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/examples/host/events.py` & `tdmclient-0.1.9/examples/host/events.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/examples/host/runprogram.py` & `tdmclient-0.1.9/examples/host/runprogram.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/notebooks/tdmclient_intro.ipynb` & `tdmclient-0.1.9/notebooks/tdmclient_intro.ipynb`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/notebooks/tdmclient_sync.ipynb` & `tdmclient-0.1.9/notebooks/tdmclient_sync.ipynb`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/notebooks/tdmclient_sync_adv.ipynb` & `tdmclient-0.1.9/notebooks/tdmclient_sync_adv.ipynb`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/notebooks/tdmclient_sync_nf.ipynb` & `tdmclient-0.1.9/notebooks/tdmclient_sync_nf.ipynb`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/setup.py` & `tdmclient-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 with open("doc/repl.md", "r") as f:
     long_description += f.read()
 with open("doc/notebooks.md", "r") as f:
     long_description += f.read()
 
 setup(
     name="tdmclient",
-    version="0.1.8",
+    version="0.1.9",
     author="Yves Piguet",
     packages=["tdmclient", "tdmclient.tools", "tdmclient.notebook", ],
     description="Communication with Thymio II robot via the Thymio Device Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/epfl-mobots/tdm-python",
     install_requires=[
```

### Comparing `tdmclient-0.1.8/tdmclient/__init__.py` & `tdmclient-0.1.9/tdmclient/__init__.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/atranspiler.py` & `tdmclient-0.1.9/tdmclient/atranspiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1201,16 +1201,16 @@
 
         # variable declarations
         var_decl = context_top.var_declarations()
         var_decl += "".join([
             context_top.functions[fun_name].var_declarations()
             for fun_name in context_top.functions
         ])
-        for var_name, var_val0 in enumerate(self.additional_var_declarations):
-            var_decl += f"""var {var_name} = {var_val0}
+        for var_name in self.additional_var_declarations:
+            var_decl += f"""var {var_name} = {self.additional_var_declarations[var_name]}
 """
         if len(var_decl) > 0:
             self.output_src = var_decl + "\n" + self.output_src
 
     def get_print_statements(self):
         """Get the python source code of a list of print statements
         where each element is a tuple with a format string and the number of numeric
```

### Comparing `tdmclient-0.1.8/tdmclient/client.py` & `tdmclient-0.1.9/tdmclient/client.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/clientasync.py` & `tdmclient-0.1.9/tdmclient/clientasync.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/clientasynccachenode.py` & `tdmclient-0.1.9/tdmclient/clientasynccachenode.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/clientasyncnode.py` & `tdmclient-0.1.9/tdmclient/clientasyncnode.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/clientnode.py` & `tdmclient-0.1.9/tdmclient/clientnode.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/fb.py` & `tdmclient-0.1.9/tdmclient/fb.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/module_clock.py` & `tdmclient-0.1.9/tdmclient/module_clock.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/module_thymio.py` & `tdmclient-0.1.9/tdmclient/module_thymio.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/notebook/__init__.py` & `tdmclient-0.1.9/tdmclient/notebook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,19 @@
     args = line.split()
     wait = "--wait" in args
     clear_event_data = "--clear-event-data" in args
     import_thymio = "--nothymio" not in args
 
     if clear_event_data:
         _interactive_console.clear_event_data()
-    _interactive_console.run_program(cell, "python", wait=wait, import_thymio=import_thymio)
+    try:
+        _interactive_console.run_program(cell, "python", wait=wait, import_thymio=import_thymio)
+    except KeyboardInterrupt:
+        # avoid long exception message with stack trace
+        print("Interrupted")
 
 @register_cell_magic
 def run_aseba(line, cell):
     _interactive_console.run_program(cell, "aseba")
 
 @register_cell_magic
 def transpile_to_aseba(line, cell):
```

### Comparing `tdmclient-0.1.8/tdmclient/repl.py` & `tdmclient-0.1.9/tdmclient/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,19 @@
             """Run program obtained by robot_code on the robot. By default, wait
             to process events until "_exit" is received (call to "exit()" in the
             robot's program), or return immediately if the program doesn't send
             any event.
             """
             src_p = robot_code()
             # compile, load, run, and set scratchpad without checking the result
-            self.run_program(src_p, language="python", wait=wait)
+            try:
+                self.run_program(src_p, language="python", wait=wait)
+            except KeyboardInterrupt:
+                # avoid long exception message with stack trace
+                print("Interrupted")
 
         def stop():
             """Stop the program running on the robot.
             """
             self.stop_program(discard_output=True)
 
         def get_var(*args):
@@ -458,14 +462,20 @@
         var_set = set()
         var_global = set()
         fun_called = set()
 
         def do_node(node):
             nonlocal globals, var_got, var_set, var_global
 
+            # alternative to direct use of isinstance for node types
+            # which aren't defined in Python 3.6
+            def isinst(obj, ast_name):
+                return (hasattr(ast, ast_name)
+                        and isinstance(obj, getattr(ast, ast_name)))
+
             if isinstance(node, ast.Assign):
                 for target in node.targets:
                     if isinstance(target, ast.Tuple):
                         for elt in target.elts:
                             do_target(elt)
                     else:
                         do_target(target)
@@ -477,16 +487,16 @@
                 do_node(node.value)
             elif isinstance(node, ast.BinOp):
                 do_node(node.left)
                 do_node(node.right)
             elif isinstance(node, ast.BoolOp):
                 do_nodes(node.values)
             elif isinstance(node, ast.Call):
+                do_node(node.func)
                 do_nodes(node.args)
-                ast.dump(node)
                 if isinstance(node.func, ast.Name):
                     fun_name = node.func.id
                     if (fun_name not in ATranspiler.PREDEFINED_FUNCTIONS
                         or fun_name in self.fun_defs):
                         fun_called.add(fun_name)
                     if fun_name in self.fun_defs:
                         # call to a user-defined function
@@ -535,19 +545,29 @@
                 do_node(node.test)
                 do_node(node.body)
                 do_node(node.orelse)
             elif isinstance(node, ast.Index):
                 do_node(node.value)
             elif isinstance(node, ast.JoinedStr):
                 do_nodes(node.values)
+            elif isinstance(node, ast.Lambda):
+                do_node(node.body)
             elif isinstance(node, ast.List):
                 do_nodes(node.elts)
             elif isinstance(node, ast.ListComp):
                 do_node(node.elt)
                 do_nodes(node.generators)
+            elif isinst(node, "Match"):
+                do_node(node.subject)
+                for c in node.cases:
+                    do_node(c.pattern)
+                    do_node(c.guard)
+                    do_nodes(c.body)
+            elif isinst(node, "MatchValue"):
+                do_node(node.value)
             elif isinstance(node, ast.Name):
                 if node.id in globals:
                     var_got.add(node.id)
             elif isinstance(node, ast.Return):
                 do_node(node.value)
             elif isinstance(node, ast.Set):
                 do_nodes(node.elts)
@@ -582,19 +602,20 @@
                 do_node(node.value)
             elif isinstance(node, ast.YieldFrom):
                 do_node(node.value)
             elif isinstance(node,
                             (ast.AsyncFunctionDef, ast.Attribute,
                              ast.Break,
                              ast.ClassDef, ast.Constant, ast.Continue,
-                             ast.Delete, ast.FunctionDef,
+                             ast.Delete,
+                             ast.FunctionDef,
                              ast.Import, ast.ImportFrom,
-                             ast.Lambda,
                              ast.NameConstant, ast.Nonlocal, ast.Num,
-                             ast.Pass)):
+                             ast.Pass,
+                             ast.Str)):
                 pass
             elif node is not None:
                 print("Unchecked", ast.dump(node))
 
         def do_nodes(nodes):
             for node in nodes:
                 do_node(node)
@@ -627,15 +648,15 @@
             self.var_got &= self.sync_var
             self.var_set &= self.sync_var
             self.fetch_variables(self.var_got)
         except Exception as e:
             # print("pre_run error", e)
             pass
 
-    def get_function_def_src(self, node):
+    def get_function_def_src(self, node, next_node):
         # use bytes b/c col_offset is in bytes
         src_b = bytes(self.cmd_src, "utf-8")
 
         def index(lineno, col_offset):
             i = 0
             for _ in range(1, lineno):
                 # start of next line
@@ -649,40 +670,39 @@
                 index_from = min(index_from,
                                  index(decorator.lineno, decorator.col_offset))
             # as well as first "@"
             while index_from > 0 and src_b[index_from - 1] in b" \t":
                 index_from -= 1
             if src_b[index_from - 1] == ord("@"):
                 index_from -= 1
-            else:
-                raise SyntaxError("Internal error",
-                                  ("<stdin>",
-                                   node.decorator_list[0].lineno,
-                                   node.decorator_list[0].col_offset,
-                                   self.cmd_src))
 
-        index_to = index(node.end_lineno, node.end_col_offset)
+        index_to = (index(next_node.lineno, next_node.col_offset)
+                    if next_node is not None
+                    else len(src_b))
 
         return str(src_b[index_from : index_to], "utf-8") + "\n"
 
     def post_run(self):
         """Analyze a complete command after it has been executed,
         with or without error.
         """
         self.send_variables(self.var_set)
         try:
             if (self.cmd_tree is not None and
                 self.cmd_tree.body is not None):
-                for statement in self.cmd_tree.body:
+                for i, statement in enumerate(self.cmd_tree.body):
                     if isinstance(statement, ast.FunctionDef):
                         # keep function source code
                         var_got, var_set, var_gl, fun_called = self.find_global_var(statement.body,
                                                                                     globals=set())
                         self.fun_defs[statement.name] = {
-                            "src": self.get_function_def_src(statement),
+                            "src": self.get_function_def_src(statement,
+                                                             self.cmd_tree.body[i + 1]
+                                                             if i + 1 < len(self.cmd_tree.body)
+                                                             else None),
                             "in": var_got,
                             "out": var_set,
                             "global": var_gl,
                             "calls": fun_called,
                         }
                     elif isinstance(statement, ast.Delete):
                         # discard function source code
```

### Comparing `tdmclient-0.1.8/tdmclient/server.py` & `tdmclient-0.1.9/tdmclient/server.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tcp.py` & `tdmclient-0.1.9/tdmclient/tcp.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/thymio.py` & `tdmclient-0.1.9/tdmclient/thymio.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/gui.py` & `tdmclient-0.1.9/tdmclient/tools/gui.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/list.py` & `tdmclient-0.1.9/tdmclient/tools/list.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/repl.py` & `tdmclient-0.1.9/tdmclient/tools/repl.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,52 +29,56 @@
   --robotid=I    robot id; default=any
   --robotname=N  robot name; default=any
   --tdmaddr=H    tdm address (default: localhost or from zeroconf)
   --tdmport=P    tdm port (default: from zeroconf)
 """)
 
 
-if __name__ == "__main__":
-
+def main(argv=None):
     tdm_addr = None
     tdm_port = None
     robot_id = None
     robot_name = None
 
-    try:
-        arguments, values = getopt.getopt(sys.argv[1:],
-                                          "",
-                                          [
-                                              "help",
-                                              "robotid=",
-                                              "robotname=",
-                                              "tdmaddr=",
-                                              "tdmport=",
-                                          ])
-    except getopt.error as err:
-        print(str(err))
-        sys.exit(1)
-    for arg, val in arguments:
-        if arg == "--help":
-            help()
-            sys.exit(0)
-        elif arg == "--robotid":
-            robot_id = val
-        elif arg == "--robotname":
-            robot_name = val
-        elif arg == "--tdmaddr":
-            tdm_addr = val
-        elif arg == "--tdmport":
-            tdm_port = int(val)
+    if argv is not None:
+        try:
+            arguments, values = getopt.getopt(argv[1:],
+                                              "",
+                                              [
+                                                  "help",
+                                                  "robotid=",
+                                                  "robotname=",
+                                                  "tdmaddr=",
+                                                  "tdmport=",
+                                              ])
+        except getopt.error as err:
+            print(str(err))
+            sys.exit(1)
+        for arg, val in arguments:
+            if arg == "--help":
+                help()
+                sys.exit(0)
+            elif arg == "--robotid":
+                robot_id = val
+            elif arg == "--robotname":
+                robot_name = val
+            elif arg == "--tdmaddr":
+                tdm_addr = val
+            elif arg == "--tdmport":
+                tdm_port = int(val)
 
     with ClientAsync(tdm_addr=tdm_addr, tdm_port=tdm_port) as client:
 
         async def co_init():
             with await client.lock(node_id=robot_id, node_name=robot_name) as node:
                 interactive_console = TDMConsole(user_functions={
                     "get_client": lambda: client,
                     "get_node": lambda: node,
                 })
                 await interactive_console.init(client, node)
                 interactive_console.interact()
 
         client.run_async_program(co_init)
+
+
+if __name__ == "__main__":
+    main(sys.argv)
```

### Comparing `tdmclient-0.1.8/tdmclient/tools/run.py` & `tdmclient-0.1.9/tdmclient/tools/run.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/server.py` & `tdmclient-0.1.9/tdmclient/tools/server.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/tdmdiscovery.py` & `tdmclient-0.1.9/tdmclient/tools/tdmdiscovery.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/transpile.py` & `tdmclient-0.1.9/tdmclient/tools/transpile.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/tools/watch.py` & `tdmclient-0.1.9/tdmclient/tools/watch.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/ws.py` & `tdmclient-0.1.9/tdmclient/ws.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient/zeroconf.py` & `tdmclient-0.1.9/tdmclient/zeroconf.py`

 * *Files identical despite different names*

### Comparing `tdmclient-0.1.8/tdmclient.egg-info/PKG-INFO` & `tdmclient-0.1.9/tdmclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdmclient
-Version: 0.1.8
+Version: 0.1.9
 Summary: Communication with Thymio II robot via the Thymio Device Manager
 Home-page: https://github.com/epfl-mobots/tdm-python
 Author: Yves Piguet
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tdmclient-0.1.8/tdmclient.egg-info/SOURCES.txt` & `tdmclient-0.1.9/tdmclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

