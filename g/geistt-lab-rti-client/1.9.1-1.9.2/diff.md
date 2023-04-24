# Comparing `tmp/geistt-lab-rti-client-1.9.1.tar.gz` & `tmp/geistt-lab-rti-client-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geistt-lab-rti-client-1.9.1.tar", last modified: Fri Feb 17 06:36:15 2023, max compression
+gzip compressed data, was "dist/geistt-lab-rti-client-1.9.2.tar", last modified: Thu Feb 23 22:36:33 2023, max compression
```

## Comparing `geistt-lab-rti-client-1.9.1.tar` & `geistt-lab-rti-client-1.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/
--rw-r--r--   0 root         (0) root         (0)     1240 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    11356 2023-02-17 06:35:38.000000 geistt-lab-rti-client-1.9.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-02-17 06:35:38.000000 geistt-lab-rti-client-1.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/
--rw-rw-rw-   0 root         (0) root         (0)     6421 2023-02-17 06:35:38.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/rtiruntimecontrol.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-02-17 06:35:38.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/proto/
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-02-17 06:35:38.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/
--rw-r--r--   0 root         (0) root         (0)    18728 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityPosition_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28090 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Injections_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13335 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/LaunchConfigurations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16729 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Commands_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Scenarios_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20179 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityOperation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9050 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Injectables_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4432 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Parameter_pb2.py
--rw-r--r--   0 root         (0) root         (0)    12286 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Channels_pb2.py
--rw-r--r--   0 root         (0) root         (0)    54577 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/GeometryOperation_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18268 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/MeasurementBundle_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7838 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Measures_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2896 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Color_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28369 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Clients_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityCategory_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/IdMessage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/RuntimeState_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7380 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Measurement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2341 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/LVCCategory_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14772 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/MessageBundle_pb2.py
--rw-r--r--   0 root         (0) root         (0)    26184 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Logs_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityDomain_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39970 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/RuntimeControl_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10143 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/LaunchEvent_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    26323 2023-02-17 06:35:38.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/rticlient.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1670 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-17 06:36:15.000000 geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    11356 2023-02-23 22:35:52.000000 geistt-lab-rti-client-1.9.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-02-23 22:35:52.000000 geistt-lab-rti-client-1.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/
+-rw-rw-rw-   0 root         (0) root         (0)     6421 2023-02-23 22:35:52.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/rtiruntimecontrol.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-02-23 22:35:52.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/proto/
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-02-23 22:35:52.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/
+-rw-r--r--   0 root         (0) root         (0)    18728 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityPosition_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28090 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Injections_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13335 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/LaunchConfigurations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16729 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Commands_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Scenarios_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20179 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityOperation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9050 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Injectables_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Parameter_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    12286 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Channels_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    54577 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/GeometryOperation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18268 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/MeasurementBundle_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7838 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Measures_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Color_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28369 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Clients_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityCategory_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/IdMessage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/RuntimeState_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7380 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Measurement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/LVCCategory_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14772 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/MessageBundle_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    26184 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Logs_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityDomain_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39970 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/RuntimeControl_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10143 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/LaunchEvent_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    26323 2023-02-23 22:35:52.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/rticlient.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-02-23 22:36:33.000000 geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/requires.txt
```

### Comparing `geistt-lab-rti-client-1.9.1/PKG-INFO` & `geistt-lab-rti-client-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geistt-lab-rti-client
-Version: 1.9.1
+Version: 1.9.2
 Summary: GEISTT Lab RTI Client
 Home-page: https://gitlab.com/geistt/lab/rti
 Author: GEISTT AB
 Author-email: packages@geistt.com
 License: Apache license 2.0
 Keywords: RTI
 Platform: UNKNOWN
```

### Comparing `geistt-lab-rti-client-1.9.1/setup.py` & `geistt-lab-rti-client-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup(
     name='geistt-lab-rti-client',
     packages=[
         'geistt_lab_rti_client',
         'geistt_lab_rti_client.proto',
         'geistt_lab_rti_client.generated'
     ],
-    version='1.9.1',
+    version='1.9.2',
     license='Apache license 2.0',
     author='GEISTT AB',
     author_email='packages@geistt.com',
     url='https://gitlab.com/geistt/lab/rti',
     description='GEISTT Lab RTI Client',
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `geistt-lab-rti-client-1.9.1/LICENSE.txt` & `geistt-lab-rti-client-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/README.md` & `geistt-lab-rti-client-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/rtiruntimecontrol.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/rtiruntimecontrol.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/constants.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/constants.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/proto/__init__.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityPosition_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityPosition_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Injections_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Injections_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/LaunchConfigurations_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/LaunchConfigurations_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Commands_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Commands_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Scenarios_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Scenarios_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityOperation_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityOperation_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Injectables_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Injectables_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Parameter_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Channels_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Channels_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/GeometryOperation_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/GeometryOperation_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/MeasurementBundle_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/MeasurementBundle_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Measures_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Measures_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Color_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Color_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Clients_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Clients_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityCategory_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityCategory_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/IdMessage_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/IdMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/RuntimeState_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/RuntimeState_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Measurement_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Measurement_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/LVCCategory_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/LVCCategory_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/MessageBundle_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/MessageBundle_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/Logs_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/Logs_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/EntityDomain_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/EntityDomain_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/RuntimeControl_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/RuntimeControl_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/generated/LaunchEvent_pb2.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/generated/LaunchEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client/rticlient.py` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client/rticlient.py`

 * *Files identical despite different names*

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/PKG-INFO` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geistt-lab-rti-client
-Version: 1.9.1
+Version: 1.9.2
 Summary: GEISTT Lab RTI Client
 Home-page: https://gitlab.com/geistt/lab/rti
 Author: GEISTT AB
 Author-email: packages@geistt.com
 License: Apache license 2.0
 Keywords: RTI
 Platform: UNKNOWN
```

### Comparing `geistt-lab-rti-client-1.9.1/geistt_lab_rti_client.egg-info/SOURCES.txt` & `geistt-lab-rti-client-1.9.2/geistt_lab_rti_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

