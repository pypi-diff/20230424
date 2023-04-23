# Comparing `tmp/dequeai-0.747.tar.gz` & `tmp/dequeai-0.748.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.747.tar", last modified: Sun Apr 23 23:32:24 2023, max compression
+gzip compressed data, was "dequeai-0.748.tar", last modified: Sun Apr 23 23:55:38 2023, max compression
```

## Comparing `dequeai-0.747.tar` & `dequeai-0.748.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:32:24.443527 dequeai-0.747/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:32:24.443527 dequeai-0.747/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:32:24.443527 dequeai-0.747/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.747/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.747/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.747/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.747/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-04-21 15:01:14.000000 dequeai-0.747/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29656 2023-04-23 23:31:37.000000 dequeai-0.747/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.747/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.747/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.747/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.747/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:32:24.443527 dequeai-0.747/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:32:23.000000 dequeai-0.747/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 23:32:24.443527 dequeai-0.747/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-23 23:32:10.000000 dequeai-0.747/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:55:38.442129 dequeai-0.748/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:55:38.442129 dequeai-0.748/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:55:38.442129 dequeai-0.748/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.748/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.748/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.748/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.748/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-21 15:01:14.000000 dequeai-0.748/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29655 2023-04-23 23:55:25.000000 dequeai-0.748/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.748/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.748/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.748/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.748/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:55:38.442129 dequeai-0.748/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:55:37.000000 dequeai-0.748/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-23 23:55:38.000000 dequeai-0.748/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 23:55:38.000000 dequeai-0.748/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-23 23:55:38.000000 dequeai-0.748/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 23:55:38.000000 dequeai-0.748/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 23:55:38.442129 dequeai-0.748/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-23 23:55:25.000000 dequeai-0.748/setup.py
```

### Comparing `dequeai-0.747/dequeai/datatypes.py` & `dequeai-0.748/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.747/dequeai/dequeai.py` & `dequeai-0.748/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.747/dequeai/dequeai_run.py` & `dequeai-0.748/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,24 +225,24 @@
         # let's add some System metadata to the data
         metadata = {}
         gpu_count = len(GPUtil.getGPUs())
         for i in range(gpu_count):
             gpu_free_memory = GPUtil.getGPUs()[i].memoryFree
             current_gpu_load = 100 * GPUtil.getGPUs()[i].load
             total_gpu_memory = GPUtil.getGPUs()[i].memoryTotal
-            metadata.update({"GPU": {str(i): {"total_gpu_memory": total_gpu_memory, "gpu_free_memory": gpu_free_memory,
-                                              "gpu_utilization": current_gpu_load}}})
+            metadata.update({"GPU": {str(i): {"total_memory": total_gpu_memory, "free_memory": gpu_free_memory,
+                                              "utilization": current_gpu_load}}})
 
-        metadata.update({"CPU": {"cpu_utilization": psutil.cpu_percent(interval=1)}})
-        metadata.update({"CPU": {"cpu_count": psutil.cpu_count()}})
+        metadata.update({"CPU": {"utilization": psutil.cpu_percent(interval=1)}})
+        metadata.update({"CPU": {"count": psutil.cpu_count()}})
         metadata.update({"Memory": {"available_memory": psutil.virtual_memory()[1]}})
         metadata.update({"Memory": {"total_memory": psutil.virtual_memory()[0]}})
         metadata.update({"Memory": {"memory_utilization": psutil.virtual_memory()[2]}})
         metadata.update({"Disk": {"free_disk_space": psutil.disk_usage(os.path.sep)[1]}})
-        data.update({"System": metadata})
+        data["experiment_data"].update({"System": metadata})
 
         pickled_data = pickle.dumps(data)
         self._rest.post_binary(url=TRACKING_ENDPOINT, data=pickled_data)
 
     def log_artifact(self, artifact_type, path):
         if self._run_meta_data is None:
             raise ValueError("Run not initialized. Please call init first")
```

### Comparing `dequeai-0.747/dequeai/parsing_service.py` & `dequeai-0.748/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.747/dequeai/rest_connect.py` & `dequeai-0.748/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.747/dequeai/util.py` & `dequeai-0.748/dequeai/util.py`

 * *Files identical despite different names*

