# Comparing `tmp/yuanfen-2023.4.24.1.tar.gz` & `tmp/yuanfen-2023.4.24.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuanfen-2023.4.24.1.tar", last modified: Mon Apr 24 07:00:29 2023, max compression
+gzip compressed data, was "yuanfen-2023.4.24.9.tar", last modified: Mon Apr 24 12:57:02 2023, max compression
```

## Comparing `yuanfen-2023.4.24.1.tar` & `yuanfen-2023.4.24.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:00:29.736481 yuanfen-2023.4.24.1/
--rw-r--r--   0 root         (0) root         (0)     1019 2023-04-24 07:00:29.735481 yuanfen-2023.4.24.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-23 10:54:21.000000 yuanfen-2023.4.24.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 07:00:29.736481 yuanfen-2023.4.24.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.24.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:00:29.734481 yuanfen-2023.4.24.1/yuanfen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 07:00:28.000000 yuanfen-2023.4.24.1/yuanfen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1912 2023-04-24 07:00:28.000000 yuanfen-2023.4.24.1/yuanfen/config.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.24.1/yuanfen/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:00:29.735481 yuanfen-2023.4.24.1/yuanfen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1019 2023-04-24 07:00:29.000000 yuanfen-2023.4.24.1/yuanfen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-04-24 07:00:29.000000 yuanfen-2023.4.24.1/yuanfen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 07:00:29.000000 yuanfen-2023.4.24.1/yuanfen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-24 07:00:29.000000 yuanfen-2023.4.24.1/yuanfen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-24 07:00:29.000000 yuanfen-2023.4.24.1/yuanfen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:57:02.919557 yuanfen-2023.4.24.9/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-24 12:57:02.919557 yuanfen-2023.4.24.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-23 10:54:21.000000 yuanfen-2023.4.24.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 12:57:02.919557 yuanfen-2023.4.24.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.24.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:57:02.918557 yuanfen-2023.4.24.9/yuanfen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 12:57:01.000000 yuanfen-2023.4.24.9/yuanfen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-24 11:13:41.000000 yuanfen-2023.4.24.9/yuanfen/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.24.9/yuanfen/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:57:02.918557 yuanfen-2023.4.24.9/yuanfen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/top_level.txt
```

### Comparing `yuanfen-2023.4.24.1/PKG-INFO` & `yuanfen-2023.4.24.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.24.1
+Version: 2023.4.24.9
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yuanfen-2023.4.24.1/README.md` & `yuanfen-2023.4.24.9/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.1/setup.py` & `yuanfen-2023.4.24.9/setup.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.1/yuanfen/config.py` & `yuanfen-2023.4.24.9/yuanfen/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import configparser
 import json
 import os
 import threading
 
 import yaml
 from watchdog.events import FileSystemEventHandler
+from watchdog.observers.polling import PollingObserver
 from watchdog.observers import Observer
 
 from . import logger
 
 
 class Config:
     observer = None
     observer_lock = threading.Lock()
 
-    def __init__(self, _path):
-        self._path = _path
+    def __init__(self, path, poll=True):
+        self._path = path
         self._data = {}
         self._load()
 
         with Config.observer_lock:
             if Config.observer is None:
-                Config.observer = Observer()
+                Config.observer = PollingObserver() if poll else Observer()
                 Config.observer.start()
 
             self.observer = Config.observer
-            self.observer.schedule(ConfigChangeHandler(self), os.path.dirname(_path), recursive=False)
+            self.observer.schedule(ConfigChangeHandler(self), os.path.dirname(path), recursive=False)
 
     def __getitem__(self, key):
         return self._data[key]
 
     def _load(self):
         with open(self._path, "r") as f:
             if self._path.endswith(".json"):
@@ -49,11 +50,10 @@
 
 class ConfigChangeHandler(FileSystemEventHandler):
     def __init__(self, config):
         super().__init__()
         self.config = config
 
     def on_modified(self, event):
-        logger.info(f"{event.src_path} modified, {os.path.abspath(event.src_path)}, {os.path.abspath(self.config._path)}"  )
         if os.path.abspath(event.src_path) == os.path.abspath(self.config._path):
             self.config._load()
             logger.info(f"{event.src_path} reloaded")
```

### Comparing `yuanfen-2023.4.24.1/yuanfen/logger.py` & `yuanfen-2023.4.24.9/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.1/yuanfen.egg-info/PKG-INFO` & `yuanfen-2023.4.24.9/yuanfen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.24.1
+Version: 2023.4.24.9
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

