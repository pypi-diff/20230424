# Comparing `tmp/tdmclient-ty-0.1.8.tar.gz` & `tmp/tdmclient-ty-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdmclient-ty-0.1.8.tar", last modified: Thu Mar  2 22:29:34 2023, max compression
+gzip compressed data, was "tdmclient-ty-0.1.9.tar", last modified: Mon Apr 24 06:30:03 2023, max compression
```

## Comparing `tdmclient-ty-0.1.8.tar` & `tdmclient-ty-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 22:29:34.775166 tdmclient-ty-0.1.8/
--rw-rw-rw-   0        0        0     1895 2023-03-02 22:25:47.000000 tdmclient-ty-0.1.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1529 2021-10-20 08:38:54.000000 tdmclient-ty-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       58 2021-10-20 08:38:58.000000 tdmclient-ty-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5269 2023-03-02 22:29:34.775166 tdmclient-ty-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2022-06-22 07:33:33.000000 tdmclient-ty-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 22:29:34.741163 tdmclient-ty-0.1.8/doc/
--rw-rw-rw-   0        0        0     4770 2022-04-05 12:33:37.000000 tdmclient-ty-0.1.8/doc/help.md
--rw-rw-rw-   0        0        0       42 2023-03-02 22:29:34.776165 tdmclient-ty-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1033 2023-03-02 22:24:30.000000 tdmclient-ty-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 22:29:34.769163 tdmclient-ty-0.1.8/tdmclient_ty.egg-info/
--rw-rw-rw-   0        0        0     5269 2023-03-02 22:29:34.000000 tdmclient-ty-0.1.8/tdmclient_ty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-03-02 22:29:34.000000 tdmclient-ty-0.1.8/tdmclient_ty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 22:29:34.000000 tdmclient-ty-0.1.8/tdmclient_ty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-02 22:29:34.000000 tdmclient-ty-0.1.8/tdmclient_ty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-02 22:29:34.000000 tdmclient-ty-0.1.8/tdmclient_ty.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-02 22:29:34.731181 tdmclient-ty-0.1.8/thonnycontrib/
-drwxrwxrwx   0        0        0        0 2023-03-02 22:29:34.770164 tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/
--rw-rw-rw-   0        0        0    16259 2023-03-02 22:24:41.000000 tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-02 22:29:34.773166 tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/res/
--rw-rw-rw-   0        0        0     5012 2022-06-22 07:18:21.000000 tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/res/thymio.run.png
--rw-rw-rw-   0        0        0     4968 2022-06-22 07:18:21.000000 tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/res/thymio.stop.png
+drwxrwxrwx   0        0        0        0 2023-04-24 06:30:03.534647 tdmclient-ty-0.1.9/
+-rw-rw-rw-   0        0        0     2115 2023-04-23 10:03:24.000000 tdmclient-ty-0.1.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1529 2021-10-20 08:38:54.000000 tdmclient-ty-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       58 2021-10-20 08:38:58.000000 tdmclient-ty-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5269 2023-04-24 06:30:03.534647 tdmclient-ty-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2022-06-22 07:33:33.000000 tdmclient-ty-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:30:03.496542 tdmclient-ty-0.1.9/doc/
+-rw-rw-rw-   0        0        0     4770 2022-04-05 12:33:37.000000 tdmclient-ty-0.1.9/doc/help.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:30:03.534647 tdmclient-ty-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-04-23 10:03:45.000000 tdmclient-ty-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:30:03.524575 tdmclient-ty-0.1.9/tdmclient_ty.egg-info/
+-rw-rw-rw-   0        0        0     5269 2023-04-24 06:30:03.000000 tdmclient-ty-0.1.9/tdmclient_ty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-24 06:30:03.000000 tdmclient-ty-0.1.9/tdmclient_ty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:30:03.000000 tdmclient-ty-0.1.9/tdmclient_ty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 06:30:03.000000 tdmclient-ty-0.1.9/tdmclient_ty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 06:30:03.000000 tdmclient-ty-0.1.9/tdmclient_ty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 06:30:03.480471 tdmclient-ty-0.1.9/thonnycontrib/
+drwxrwxrwx   0        0        0        0 2023-04-24 06:30:03.534647 tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/
+-rw-rw-rw-   0        0        0    16410 2023-04-12 22:10:34.000000 tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:30:03.534647 tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/res/
+-rw-rw-rw-   0        0        0     5012 2022-06-22 07:18:21.000000 tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/res/thymio.run.png
+-rw-rw-rw-   0        0        0     4968 2022-06-22 07:18:21.000000 tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/res/thymio.stop.png
```

### Comparing `tdmclient-ty-0.1.8/CHANGELOG.md` & `tdmclient-ty-0.1.9/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 Notable changes of tdmclient-ty. Release versions refer to [https://pypi.org/project/tdmclient-ty/].
 
 ## [Unreleased]
 
+## [0.1.9] - 2023-04-24
+
+### Fixed
+
+- When the automatic connection on launch fails, usually because the TDM isn't running and Thonny is started for plain Python without robot, an error message isn't displayed anymore.
+
 ## [0.1.8] - 2023-03-02
 
 ### Fixed
 
 - When the connection to the TDM fails at launch, periodic attempt to reconnect has been suppressed. It froze the GUI for 2 seconds. It has been replaced with a menu entry "Connect to Thymio" in the "Thymio" menu.
 
 ## [0.1.7] - 2022-10-17
```

### Comparing `tdmclient-ty-0.1.8/LICENSE` & `tdmclient-ty-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tdmclient-ty-0.1.8/PKG-INFO` & `tdmclient-ty-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdmclient-ty
-Version: 0.1.8
+Version: 0.1.9
 Summary: Communication with Thymio II robot from Thonny via the Thymio Device Manager
 Home-page: https://github.com/epfl-mobots/tdmclient-ty
 Author: Yves Piguet
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tdmclient-ty-0.1.8/README.md` & `tdmclient-ty-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tdmclient-ty-0.1.8/doc/help.md` & `tdmclient-ty-0.1.9/doc/help.md`

 * *Files identical despite different names*

### Comparing `tdmclient-ty-0.1.8/setup.py` & `tdmclient-ty-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import find_packages, setup
 
 with open("doc/help.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="tdmclient-ty",
-    version="0.1.8",
+    version="0.1.9",
     author="Yves Piguet",
     packages=["thonnycontrib.tdmclient_ty"],
     description="Communication with Thymio II robot from Thonny via the Thymio Device Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/epfl-mobots/tdmclient-ty",
     install_requires=[
```

### Comparing `tdmclient-ty-0.1.8/tdmclient_ty.egg-info/PKG-INFO` & `tdmclient-ty-0.1.9/tdmclient_ty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdmclient-ty
-Version: 0.1.8
+Version: 0.1.9
 Summary: Communication with Thymio II robot from Thonny via the Thymio Device Manager
 Home-page: https://github.com/epfl-mobots/tdmclient-ty
 Author: Yves Piguet
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/__init__.py` & `tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,22 @@
         except ConnectionRefusedError:
             print("ConnectionRefusedError")
             client = None
             node_default = None
             node = None
 
 
-def connect(lock=True):
+def connect(lock=True, hide_connection_error=False):
     connect_tdm()
     global node
     node = None if client is None else node_default if robot_view is None else client.first_node(node_id=robot_view.selected_node_id)
     if lock:
         if node is None:
-            print_error("Cannot connect to robot\n")
+            if not hide_connection_error:
+                print_error("Cannot connect to robot\n")
             return
         try:
             aw(node.lock())
             get_workbench().after(100, process_incoming_messages)  # schedule after 100 ms
         except NodeLockError:
             node = None
     get_workbench()._update_toolbar()
@@ -446,14 +447,16 @@
     def patched_restart(c):
         filename = get_filename()
         if filename is not None and filename.endswith(".pythii"):
             stop()
         else:
             c["handler"]()
 
-    get_workbench().after(1000, connect)  # schedule after 1 s
+    # schedule connection after 1 s
+    get_workbench().after(1000,
+                          lambda: connect(hide_connection_error=True))
 
 def unload_plugin(event=None):
     global client
     if client is not None:
         client.disconnect()
         client = None
```

### Comparing `tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/res/thymio.run.png` & `tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/res/thymio.run.png`

 * *Files identical despite different names*

### Comparing `tdmclient-ty-0.1.8/thonnycontrib/tdmclient_ty/res/thymio.stop.png` & `tdmclient-ty-0.1.9/thonnycontrib/tdmclient_ty/res/thymio.stop.png`

 * *Files identical despite different names*

