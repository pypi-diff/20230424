# Comparing `tmp/era_5g_interface-0.1.0.tar.gz` & `tmp/era_5g_interface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_interface-0.1.0.tar", last modified: Fri Mar  3 13:27:23 2023, max compression
+gzip compressed data, was "era_5g_interface-0.2.0.tar", last modified: Mon Apr 24 11:45:28 2023, max compression
```

## Comparing `era_5g_interface-0.1.0.tar` & `era_5g_interface-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-03 13:27:23.894338 era_5g_interface-0.1.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-03-03 13:27:23.894338 era_5g_interface-0.1.0/PKG-INFO
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      625 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/backend_shim.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-03 13:27:23.890339 era_5g_interface-0.1.0/era_5g_interface/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface/py.typed
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1226 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface/task_handler.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2353 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface/task_handler_gstreamer.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      968 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface/task_handler_gstreamer_internal_q.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1418 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface/task_handler_internal_q.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-03-03 13:27:23.894338 era_5g_interface-0.1.0/era_5g_interface.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      513 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       24 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/era_5g_interface.egg-info/top_level.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-03-03 13:27:23.894338 era_5g_interface-0.1.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      873 2023-03-03 13:27:23.000000 era_5g_interface-0.1.0/setup.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/MANIFEST.in
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/PKG-INFO
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      625 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/backend_shim.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/era_5g_interface/
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/__init__.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/py.typed
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1251 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     2837 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      968 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer_internal_q.py
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)     1450 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface/task_handler_internal_q.py
+drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/era_5g_interface.egg-info/
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      427 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      513 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       24 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/requires.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       17 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/era_5g_interface.egg-info/top_level.txt
+-rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-04-24 11:45:28.890776 era_5g_interface-0.2.0/setup.cfg
+-rw-r--r--   0 zdenal    (1000) zdenal    (1000)      873 2023-04-24 11:45:28.000000 era_5g_interface-0.2.0/setup.py
```

### Comparing `era_5g_interface-0.1.0/backend_shim.py` & `era_5g_interface-0.2.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.1.0/era_5g_interface/task_handler.py` & `era_5g_interface-0.2.0/era_5g_interface/task_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import ABC, abstractmethod
 from threading import Event, Thread
 from typing import Optional
 
+import numpy as np
+
 
 class TaskHandlerInitializationFailed(Exception):
     pass
 
 
 class TaskHandler(Thread, ABC):
     """Abstract class.
@@ -27,15 +29,15 @@
     def run(self) -> None:
         """This method is run once the thread is started and could be used for
         periodical retrieval of images."""
 
         pass
 
     @abstractmethod
-    def store_image(self, metadata: dict, image: bytes) -> None:
+    def store_image(self, metadata: dict, image: np.ndarray) -> None:
         """This method is intended to pass the image to the worker (using
         internal queues, message broker or anything else).
 
         Args:
             metadata (dict): Arbitrary dictionary with metadata related to the image.
                 The format is NetApp-specific.
             image (_type_): The image to be processed.
```

### Comparing `era_5g_interface-0.1.0/era_5g_interface/task_handler_gstreamer.py` & `era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import time
 from abc import ABC
 
 import cv2
 
 from era_5g_interface.task_handler import TaskHandler, TaskHandlerInitializationFailed
 
 
@@ -33,32 +34,44 @@
 
         Raises:
             TaskHandlerInitializationFailed: Raised when the construction of
                 Gstreamer pipeline failed
         """
 
         # pipeline which decodes a h264 stream
-        camSet = (
-            f'udpsrc port={self.port} caps="application/x-rtp,media=(string)video,encoding-name=(string)H264,'
-            f'payload=(int)96" ! rtpjitterbuffer ! rtph264depay ! avdec_h264 ! videorate ! videoconvert ! '
-            f"appsink"
+        pipeline = (
+            f"udpsrc port={self.port} "
+            'caps="application/x-rtp,media=(string)video,encoding-name=(string)H264,'
+            'payload=(int)96" ! '
+            "rtph264depay ! avdec_h264 ! videoconvert ! appsink"
         )
 
         try:
             logging.info(f"Creating Gstreamer capture on port {self.port}")
             # standard OpenCV VideoCapture connected to the Gstreamer pipeline
-            cap = cv2.VideoCapture(camSet)
+            cap = cv2.VideoCapture(pipeline)
             if not cap.isOpened():
                 raise TaskHandlerInitializationFailed("VideoCapture was not opened")
             logging.info("Gstreamer capture created")
         except Exception as e:
             logging.error(f"Gstreamer capture failed. {str(e)}")
             # TODO: raise exception?
             exit(1)
 
         while not self.stop_event.is_set():
             ret, frame = cap.read()
             if ret:
-                # extract the timestamp from the frame
-                timestamp = cap.get(cv2.CAP_PROP_POS_MSEC)
-                self.store_image({"sid": self.sid, "websocket_id": self.websocket_id, "timestamp": timestamp}, frame)
+                recv_timestamp = time.time_ns()
+                # use frame number instead of unknown timestamp
+                logging.debug(f"CAP_PROP_POS_MSEC: {int(cap.get(cv2.CAP_PROP_POS_MSEC ))}")
+                logging.debug(f"CAP_PROP_POS_FRAMES: {int(cap.get(cv2.CAP_PROP_POS_FRAMES))} {recv_timestamp}")
+                timestamp = str(int(cap.get(cv2.CAP_PROP_POS_FRAMES)))
+                self.store_image(
+                    {
+                        "sid": self.sid,
+                        "websocket_id": self.websocket_id,
+                        "timestamp": timestamp,
+                        "recv_timestamp": recv_timestamp,
+                    },
+                    frame,
+                )
         cap.release()
```

### Comparing `era_5g_interface-0.1.0/era_5g_interface/task_handler_gstreamer_internal_q.py` & `era_5g_interface-0.2.0/era_5g_interface/task_handler_gstreamer_internal_q.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.1.0/era_5g_interface/task_handler_internal_q.py` & `era_5g_interface-0.2.0/era_5g_interface/task_handler_internal_q.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from queue import Full, Queue
 
+import numpy as np
+
 from era_5g_interface.task_handler import TaskHandler
 
 
 class TaskHandlerInternalQ(TaskHandler):
     """Task handler which takes care of passing the data to the python internal
     queue for future processing.
 
@@ -22,15 +24,15 @@
                 be passed to.
         """
 
         super().__init__(sid=sid, **kw)
         self._q = image_queue
         self.index = 0
 
-    def store_image(self, metadata: dict, image) -> None:
+    def store_image(self, metadata: dict, image: np.ndarray) -> None:
         """Method which will store the image to the queue for processing.
 
         Args:
             metadata (dict): Arbitrary dictionary with metadata related to the image.
                 The format is NetApp-specific.
             image (_type_): The image to be processed.
         """
```

### Comparing `era_5g_interface-0.1.0/era_5g_interface.egg-info/SOURCES.txt` & `era_5g_interface-0.2.0/era_5g_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.1.0/setup.py` & `era_5g_interface-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,9 +26,9 @@
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_interface',
     ),
     'python_requires': '>=3.8,<3.11',
-    'version': '0.1.0',
+    'version': '0.2.0',
 })
```

