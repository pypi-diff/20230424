# Comparing `tmp/vidis_algorithms_api-0.4.5.tar.gz` & `tmp/vidis_algorithms_api-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidis_algorithms_api-0.4.5.tar", last modified: Sun Apr 23 10:56:32 2023, max compression
+gzip compressed data, was "vidis_algorithms_api-0.4.6.tar", last modified: Mon Apr 24 06:55:03 2023, max compression
```

## Comparing `vidis_algorithms_api-0.4.5.tar` & `vidis_algorithms_api-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-23 10:45:55.000000 vidis_algorithms_api-0.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/vidis_algorithms_api/
--rw-rw-rw-   0 root         (0) root         (0)     1952 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/Lifecycle.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-04-23 10:45:55.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/Task.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/vidis_algorithms_api/core/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/core/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 10:56:32.111338 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-23 10:56:32.000000 vidis_algorithms_api-0.4.5/vidis_algorithms_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:55:03.387088 vidis_algorithms_api-0.4.6/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-24 06:55:03.387088 vidis_algorithms_api-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 06:55:03.387088 vidis_algorithms_api-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-04-24 06:54:45.000000 vidis_algorithms_api-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:55:03.387088 vidis_algorithms_api-0.4.6/vidis_algorithms_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2023-04-21 13:43:32.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api/Lifecycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-24 06:26:42.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:55:03.387088 vidis_algorithms_api-0.4.6/vidis_algorithms_api/core/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api/core/Settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:55:03.387088 vidis_algorithms_api-0.4.6/vidis_algorithms_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-24 06:55:03.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-24 06:55:03.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 06:55:03.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-24 06:55:03.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 06:55:03.000000 vidis_algorithms_api-0.4.6/vidis_algorithms_api.egg-info/top_level.txt
```

### Comparing `vidis_algorithms_api-0.4.5/README.md` & `vidis_algorithms_api-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.5/vidis_algorithms_api/Lifecycle.py` & `vidis_algorithms_api-0.4.6/vidis_algorithms_api/Lifecycle.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.5/vidis_algorithms_api/Task.py` & `vidis_algorithms_api-0.4.6/vidis_algorithms_api/Task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import os.path
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 import numpy as np
+from PIL import Image
 
 from vidis_algorithms_api.core import settings
 
 
 class Task(ABC):
     
     @classmethod
     @property
     @abstractmethod
     def name(cls):
         raise NotImplementedError
    
     def _save_task_result(self, layer_data: np.ndarray, hypespecter_path: str):
-        path_to_save = os.path.join(settings.DATA_PATH, hypespecter_path,
-                                    settings.CUSTOM_LAYER_FOLDER, f'{self.name}_{datetime.now()}.npy')
-        os.makedirs(os.path.dirname(path_to_save), exist_ok=True)
-        np.save(path_to_save, layer_data)
-        return os.path.dirname(path_to_save)
+        basedir = os.path.join(settings.DATA_PATH, hypespecter_path,
+                                    settings.CUSTOM_LAYER_FOLDER)
+        os.makedirs(basedir, exist_ok=True)
+        
+        path_to_save_npy = os.path.join(basedir, f'{self.name}_{datetime.now()}.npy')
+        path_to_save_webp = os.path.join(basedir, f'{self.name}_{datetime.now()}.webp')
+        
+        np.save(path_to_save_npy, layer_data)
+        image = Image.fromarray(layer_data)
+        image.thumbnail((500, 500), Image.ANTIALIAS)
+        image.save(path_to_save_webp, "WEBP")
+        
+        return basedir
         
 
     def run(self, lname, hsi_id, hyperspecter_path, **kwargs):
         # Laye
         data = np.load(os.path.join(settings.DATA_PATH, hyperspecter_path, "hsi.npy"), mmap_mode="r")
         result = self.task(hyperspecter=data, **kwargs)
         assert result.ndim == 2, "Result should have two dimensions (height x width)"
```

