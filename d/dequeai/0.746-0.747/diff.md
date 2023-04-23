# Comparing `tmp/dequeai-0.746.tar.gz` & `tmp/dequeai-0.747.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.746.tar", last modified: Sun Apr 23 23:14:35 2023, max compression
+gzip compressed data, was "dequeai-0.747.tar", last modified: Sun Apr 23 23:32:24 2023, max compression
```

## Comparing `dequeai-0.746.tar` & `dequeai-0.747.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:14:35.490360 dequeai-0.746/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:14:35.490360 dequeai-0.746/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:14:35.490360 dequeai-0.746/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.746/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.746/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.746/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.746/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-04-21 15:01:14.000000 dequeai-0.746/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29653 2023-04-23 23:11:14.000000 dequeai-0.746/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.746/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.746/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.746/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.746/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:14:35.490360 dequeai-0.746/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 23:14:35.490360 dequeai-0.746/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-23 23:14:22.000000 dequeai-0.746/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:32:24.443527 dequeai-0.747/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:32:24.443527 dequeai-0.747/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:32:24.443527 dequeai-0.747/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.747/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.747/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.747/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.747/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-21 15:01:14.000000 dequeai-0.747/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29656 2023-04-23 23:31:37.000000 dequeai-0.747/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.747/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.747/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.747/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.747/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:32:24.443527 dequeai-0.747/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:32:23.000000 dequeai-0.747/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 23:32:24.000000 dequeai-0.747/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 23:32:24.443527 dequeai-0.747/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-23 23:32:10.000000 dequeai-0.747/setup.py
```

### Comparing `dequeai-0.746/dequeai/datatypes.py` & `dequeai-0.747/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.746/dequeai/dequeai.py` & `dequeai-0.747/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.746/dequeai/dequeai_run.py` & `dequeai-0.747/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         else:
             self.user_name = None
             raise ValueError("Invalid user and/or api key")
         self._run_start_time = datetime.datetime.now()
         self._running = True
         self._workload_type = os.getenv("workload_type")
         self._workload_id = os.getenv("workload_id")
-        if self._workload_type is None or self._workload_id is None:
-            raise ValueError(
-                "Deque AI package is only supported wihtin the Creator's App. Download the app from https://deque.ai")
+        #if self._workload_type is None or self._workload_id is None:
+            #raise ValueError(
+               # "Deque AI package is only supported wihtin the Creator's App. Download the app from https://deque.ai")
 
         self._submission_id = os.getenv("submission_id")
         self._agent_id = os.getenv("agent_id")
         if project_name is None:
             if self._workload_id is None:
                 raise ValueError("Project name cannot be empty")
             else:
```

### Comparing `dequeai-0.746/dequeai/parsing_service.py` & `dequeai-0.747/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.746/dequeai/rest_connect.py` & `dequeai-0.747/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.746/dequeai/util.py` & `dequeai-0.747/dequeai/util.py`

 * *Files identical despite different names*

