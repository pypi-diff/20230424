# Comparing `tmp/dequeai-0.745.tar.gz` & `tmp/dequeai-0.746.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.745.tar", last modified: Thu Apr 20 23:32:56 2023, max compression
+gzip compressed data, was "dequeai-0.746.tar", last modified: Sun Apr 23 23:14:35 2023, max compression
```

## Comparing `dequeai-0.745.tar` & `dequeai-0.746.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:32:56.131846 dequeai-0.745/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 23:32:56.131846 dequeai-0.745/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:32:56.131846 dequeai-0.745/dequeai/
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 21:04:18.000000 dequeai-0.745/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.745/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.745/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.745/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.745/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    28332 2023-04-20 23:31:17.000000 dequeai-0.745/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.745/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.745/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.745/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.745/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:32:56.131846 dequeai-0.745/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 23:32:55.000000 dequeai-0.745/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 23:32:56.000000 dequeai-0.745/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 23:32:55.000000 dequeai-0.745/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 23:32:55.000000 dequeai-0.745/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 23:32:56.000000 dequeai-0.745/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 23:32:56.131846 dequeai-0.745/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 23:32:42.000000 dequeai-0.745/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:14:35.490360 dequeai-0.746/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:14:35.490360 dequeai-0.746/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:14:35.490360 dequeai-0.746/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.746/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.746/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.746/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.746/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-21 15:01:14.000000 dequeai-0.746/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29653 2023-04-23 23:11:14.000000 dequeai-0.746/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.746/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.746/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.746/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.746/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 23:14:35.490360 dequeai-0.746/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 23:14:35.000000 dequeai-0.746/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 23:14:35.490360 dequeai-0.746/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-23 23:14:22.000000 dequeai-0.746/setup.py
```

### Comparing `dequeai-0.745/dequeai/datatypes.py` & `dequeai-0.746/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.745/dequeai/dequeai.py` & `dequeai-0.746/dequeai/dequeai.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dequeai.dequeai_run import Run
 
 run = Run()
 
 
-
 def init( user_name, project_name=None, api_key=None):
     run.init(user_name, project_name, api_key)
 
 def finish():
     run.finish()
 
 def log( data, step=None, commit=True):
@@ -18,21 +17,18 @@
 
 def log_artifact(artifact_type, path):
     run.log_artifact(artifact_type, path)
 
 def load_artifact(artifact_type, run_id):
     run.load_artifact(artifact_type, run_id)
 
-
 def register_artifacts(latest=True, label=None, tags=None):
     run.register_artifacts(latest, label, tags)
 
 def compare_runs(project_name, metric_key):
     run.compare_runs(project_name, metric_key)
 
-
 def read_best_run(project_name, metric_key):
     run.read_best_run(project_name, metric_key)
 
-def search_runs(filter_dict):
-    run.search_runs(filter_dict)
+
```

### Comparing `dequeai-0.745/dequeai/dequeai_run.py` & `dequeai-0.746/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 import traceback
 import coolname
 from dequeai.rest_connect import RestConnect
 from dequeai.deque_environment import AGENT_API_SERVICE_URL
 import pickle
 import multiprocessing
 from dequeai.parsing_service import ParsingService
-from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table #, Plot
-from dequeai.util import MODEL, CODE, DATA, ENVIRONMENT, RESOURCES,TRACKING_ENDPOINT
+from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table  # , Plot
+from dequeai.util import MODEL, CODE, DATA, ENVIRONMENT, RESOURCES, TRACKING_ENDPOINT
 import requests
 import glob
 import time
 import psutil
 import GPUtil
 import socket
 import types
-from IPython.display import display,HTML
+from IPython.display import display, HTML
 from tabulate import tabulate
 import numpy as np
 
-
-
 _RESOURCE_MONITORING_INTERVAL = 60
 
+
 class Run:
 
     def __init__(self):
         self.user_name = None
         self._workload_type = None
         self.project_id = None
         self._project_name = None
@@ -44,69 +43,70 @@
         self._run_meta_data = None
         self._model_logged = False
         self._code_logged = False
         self._running = False
         self._environment_logged = False
         self._resources_logged = False
         self._res_monitor = None
-        self._run_start_time =None
+        self._run_start_time = None
 
-    def init(self, user_name, api_key,project_name=None):
+    def init(self, user_name, api_key, project_name=None):
         os.environ["running"] = "yes"
         is_authenticated = self._authenticate(user_name=user_name, api_key=api_key)
         if is_authenticated:
             self.user_name = user_name
             self._api_key = api_key
         else:
             self.user_name = None
             raise ValueError("Invalid user and/or api key")
         self._run_start_time = datetime.datetime.now()
         self._running = True
         self._workload_type = os.getenv("workload_type")
         self._workload_id = os.getenv("workload_id")
+        if self._workload_type is None or self._workload_id is None:
+            raise ValueError(
+                "Deque AI package is only supported wihtin the Creator's App. Download the app from https://deque.ai")
+
         self._submission_id = os.getenv("submission_id")
         self._agent_id = os.getenv("agent_id")
         if project_name is None:
             if self._workload_id is None:
                 raise ValueError("Project name cannot be empty")
             else:
                 self._project_name = self._workload_id
         else:
             self._project_name = project_name
         self._run_id = str(coolname.generate_slug(2))
         self._step = 1
-        p2 = multiprocessing.Process(target=self._start_parser)
-        p2.start()
+        # p2 = multiprocessing.Process(target=self._start_parser)
+        # p2.start()
         self._run_meta_data = {"submission_id": self._submission_id, "run_id": self._run_id,
                                "workload_type": self._workload_type, "workload_id": self._workload_id,
                                "project_name": self._project_name, "user_name": user_name}
         self._model_logged = False
         self._code_logged = False
         self._environment_logged = False
         self._resources_logged = False
-        print(f"Run initialized with project name as {self._project_name} for user {self.user_name} and run id {self._run_id}")
-
-    def _start_parser(self):
-        parser = ParsingService()
-        parser.receive()
+        print(
+            f"Run initialized with project name as {self._project_name} for user {self.user_name} and run id {self._run_id}")
 
     def finish(self):
         self._running = False
-        os.environ["running"]="no"
+        os.environ["running"] = "no"
         if self._res_monitor is not None:
             self._res_monitor.terminate()
 
     def _monitor_resources(self, agent_id, run_id, user_name, project_name, workload_id, submission_id,
                            workload_type, run_start_time):
         running = os.getenv("running")
-        step=os.getenv("step")
+        step = os.getenv("step")
         current = datetime.datetime.now()
-        duration_in_min = (current-run_start_time).total_seconds()/60
-        duration_in_hours = duration_in_min/60
-        while running=="yes":
+        duration_in_min = (current - run_start_time).total_seconds() / 60
+        duration_in_hours = duration_in_min / 60
+        while running == "yes":
             current = datetime.datetime.now()
             duration_in_min = (current - run_start_time).total_seconds() / 60
             duration_in_hours = duration_in_min / 60
             running = os.getenv("running")
             gpu_count = len(GPUtil.getGPUs())
             gpu_list = []
             for i in range(gpu_count):
@@ -140,34 +140,34 @@
                 'current_network_usage': 'unknown',
                 'current_gpu_usage': gpu_list,
                 'free_disk_space': psutil.disk_usage(os.path.sep)[1],
                 'ip_address': host_ip,
                 'gpu_list': gpu_list,
                 'gpu_count': len(gpu_list),
                 'agent_network_details': self._agent_network_details,
-                'create_datetime':current,
-                'update_datetime':current,
-                'duration_in_min':duration_in_min,
-                'duration_in_hours':duration_in_hours
+                'create_datetime': current,
+                'update_datetime': current,
+                'duration_in_min': duration_in_min,
+                'duration_in_hours': duration_in_hours
 
             }
             try:
                 resp = self._rest.post(
                     AGENT_API_SERVICE_URL + '/fex/experiment/monitor/',
                     json=monitoring_info, )
             except requests.exceptions.ConnectionError as e:
                 traceback.print_exc(e)
                 time.sleep(10)
                 self._monitor_resources(agent_id, run_id, user_name, project_name, workload_id, submission_id,
-                           workload_type)
+                                        workload_type)
             except Exception as ge:
                 traceback.print_exc(ge)
                 time.sleep(10)
                 self._monitor_resources(agent_id, run_id, user_name, project_name, workload_id, submission_id,
-                           workload_type)
+                                        workload_type)
             time.sleep(_RESOURCE_MONITORING_INTERVAL)
 
     def _get_network_details(self):
 
         interfaces = psutil.net_if_addrs()
         hostname = socket.gethostname()
         fqdn = socket.getfqdn()
@@ -200,15 +200,15 @@
         full_data = {"experiment_data": data}
         full_data.update(
             {"user_name": self.user_name, "run_id": self._run_id, "workload_type": self._workload_type,
              "workload_id": self._workload_id, "submission_id": self._submission_id,
              "project_name": self._project_name, "deque_log_time": datetime.datetime.now(), "step": self._step})
         p = multiprocessing.Process(target=self._log_task, args=(full_data, self._run_meta_data))
         p.start()
-        os.environ['step']=str(self._step)
+        os.environ['step'] = str(self._step)
         if commit:
             self._step += 1
 
     def log_hyperparams(self, hyperparams):
         self._validate_hyperparams(hyperparams=hyperparams)
         full_data = {"hyperparams": hyperparams}
         full_data.update(
@@ -218,14 +218,32 @@
 
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/experiment/hyperparams/create/",
                              json=full_data)
         res = resp.json()
         print(res)
 
     def _log_task(self, data, run_meta_data):
+        # let's add some System metadata to the data
+        metadata = {}
+        gpu_count = len(GPUtil.getGPUs())
+        for i in range(gpu_count):
+            gpu_free_memory = GPUtil.getGPUs()[i].memoryFree
+            current_gpu_load = 100 * GPUtil.getGPUs()[i].load
+            total_gpu_memory = GPUtil.getGPUs()[i].memoryTotal
+            metadata.update({"GPU": {str(i): {"total_gpu_memory": total_gpu_memory, "gpu_free_memory": gpu_free_memory,
+                                              "gpu_utilization": current_gpu_load}}})
+
+        metadata.update({"CPU": {"cpu_utilization": psutil.cpu_percent(interval=1)}})
+        metadata.update({"CPU": {"cpu_count": psutil.cpu_count()}})
+        metadata.update({"Memory": {"available_memory": psutil.virtual_memory()[1]}})
+        metadata.update({"Memory": {"total_memory": psutil.virtual_memory()[0]}})
+        metadata.update({"Memory": {"memory_utilization": psutil.virtual_memory()[2]}})
+        metadata.update({"Disk": {"free_disk_space": psutil.disk_usage(os.path.sep)[1]}})
+        data.update({"System": metadata})
+
         pickled_data = pickle.dumps(data)
         self._rest.post_binary(url=TRACKING_ENDPOINT, data=pickled_data)
 
     def log_artifact(self, artifact_type, path):
         if self._run_meta_data is None:
             raise ValueError("Run not initialized. Please call init first")
         if artifact_type == MODEL:
@@ -240,29 +258,30 @@
         p2.start()
 
     def _log_artifact_task(self, artifact_type, path, run_meta_data):
 
         file_name = os.path.basename(path)
         if artifact_type == MODEL:
             dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/model/" + file_name
-            valid_extensions = [".h5", ".hdf5", ".pt", ".pth", ".pkl", ".pklz", ".pkl.gz", ".pkl.bz2", ".pkl.xz", ".joblib"]
+            valid_extensions = [".h5", ".hdf5", ".pt", ".pth", ".pkl", ".pklz", ".pkl.gz", ".pkl.bz2", ".pkl.xz",
+                                ".joblib"]
             if not any(file_name.lower().endswith(ext) for ext in valid_extensions):
                 raise ValueError("Model file must be one of the following extensions: " + str(valid_extensions))
         elif artifact_type == CODE:
-            dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/code/"+ file_name
+            dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/code/" + file_name
             valid_extensions = [".ipynb", ".py"]
             if not any(file_name.lower().endswith(ext) for ext in valid_extensions):
                 raise ValueError("Code file must be one of the following extensions: " + str(valid_extensions))
         elif artifact_type == ENVIRONMENT:
             dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/environment/" + file_name
             if not file_name.lower().endswith("yml"):
                 raise ValueError("Environment file must be a .yml file")
         else:
             raise ValueError(
-                "artifact_type must be model (file), environment (file), code (file) ")#or resources (directory)")
+                "artifact_type must be model (file), environment (file), code (file) ")  # or resources (directory)")
 
         if os.path.isdir(path):
             artifact_uris = []
             for filename in glob.iglob(path + '**/**', recursive=True):
                 if os.path.isdir(filename):
                     continue
                 dest_path = dest_path + filename
@@ -318,15 +337,15 @@
         req_data = {"user_name": self.user_name, "latest": latest, "label": label,
                     "project_name": self._project_name, "run_id": self._run_id, "tags": tags}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/artifacts/register/",
                              json=req_data)
         res = resp.json()
         print(res)
 
-    def load_artifact(self,  artifact_type, run_id):
+    def load_artifact(self, artifact_type, run_id):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling load_artifact")
         req_data = {
             "user_name": self.user_name,
             "run_id": run_id,
             "artifact_type": artifact_type
         }
@@ -356,15 +375,15 @@
             print(f"Downloaded artifact '{file_name}'")
 
     def _validate_data(self, data):
         for key, value in data.items():
             if type(value) is dict:
                 self._validate_data(value)
             else:
-                if type(value) in [Audio, BoundingBox2D, Histogram,Table,
+                if type(value) in [Audio, BoundingBox2D, Histogram, Table,
                                    Image] or type(value) in types.__builtins__.values():
                     pass
                 else:
                     raise ValueError(
                         "Invalid type in dictionary. Allowed values include builtin types and Deque data types " + str(
                             type(value)) + " " + str(value.__class__.__module__))
 
@@ -390,29 +409,29 @@
         res = resp.json()
         print(res)
         if "authenticated" in res:
             return res["authenticated"]
         else:
             return False
 
-    def compare_runs(self, project_name,metric_key):
+    def compare_runs(self, project_name, metric_key):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling compare_runs")
 
         if project_name is None:
             project_name = self._project_name
 
         req_data = {
             "user_name": self.user_name,
             "project_name": project_name,
             "metric_key": metric_key
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/compare/", json=req_data)
         data_list = resp.json()
-        #print(data_list)
+        # print(data_list)
         # Extract header names
         first_run_data_keys = list(data_list['runs'][0]['best_experiment_data']['data'].keys())
         headers = ['Run ID', 'Best Metric Key', 'Best Metric'] + [f'{key}.{sub_key}' for key in first_run_data_keys for
                                                                   sub_key in
                                                                   data_list['runs'][0]['best_experiment_data']['data'][
                                                                       key]]
 
@@ -475,15 +494,15 @@
         req_data = {
             "user_name": self.user_name,
             "project_name": project_name,
             "metric_key": metric_key
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/best/read/", json=req_data)
         data_list = resp.json()
-        #print(data_list)
+        # print(data_list)
         # Extract header names
         first_run_data_keys = list(data_list['run'][0]['best_experiment_data']['data'].keys())
         headers = ['Run ID', 'Best Metric Key', 'Best Metric'] + [f'{key}.{sub_key}' for key in first_run_data_keys for
                                                                   sub_key in
                                                                   data_list['run'][0]['best_experiment_data']['data'][
                                                                       key]]
 
@@ -531,16 +550,15 @@
 
         # Wrap the table in a scrollable div
         scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{styled_table}</div>'
 
         # Display the scrollable table in the notebook
         display(HTML(scrollable_table))
 
-
-    def search_runs(self,filter_dict):
+    def search_runs(self, filter_dict):
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling search_runs")
         req_data = {
             "user_name": self.user_name,
             "filter_dict": filter_dict
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/search/", json=req_data)
@@ -557,16 +575,15 @@
             "file_format": file_format,
         }
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/report/create/", json=req_data)
         res = resp.json()
         print(res)
         return res
 
-
-    def _filter_dicts_by_keys(self,dicts_list, keys, values=None, operators=None):
+    def _filter_dicts_by_keys(self, dicts_list, keys, values=None, operators=None):
         filtered_dicts = []
 
         if not values:
             values = [None] * len(keys)
 
         if not operators:
             operators = ['=='] * len(keys)
@@ -590,16 +607,15 @@
                         break
 
             if match:
                 filtered_dicts.append(d)
 
         return filtered_dicts
 
-
-    def _get_nested_value(self,nested_dict, key):
+    def _get_nested_value(self, nested_dict, key):
         keys = key.split('.')
         current_dict = nested_dict
 
         for k in keys:
             if k in current_dict:
                 current_dict = current_dict[k]
             else:
@@ -616,17 +632,15 @@
                 self._log_histogram(f"{module_name}_input_{idx}_grad", grad.cpu().numpy())
 
         # Handling multiple output gradients
         for idx, grad in enumerate(grad_output):
             if grad is not None:
                 self._log_histogram(f"{module_name}_output_{idx}_grad", grad.cpu().numpy())
 
-
-
-    def _log_histogram(self,values, bins, min_value=None, max_value=None, density=True):
+    def _log_histogram(self, values, bins, min_value=None, max_value=None, density=True):
         """
         Log histogram data from the given values.
 
         Args:
             values (list or np.array): The values to create the histogram from.
             bins (int): The number of bins to divide the data into.
             min_value (float, optional): The lower bound of the histogram range. Defaults to the minimum value in the dataset.
@@ -646,17 +660,18 @@
 
         return bin_edges, hist
 
     def log_gradients(self, model):
         for module_name, module in model.named_modules():
             module.register_backward_hook(self._gradient_hook)
 
+
 if __name__ == "__main__":
     deque = Run()
     deque._validate_hyperparams({"train": {"accuracy": "1.3", "loss": "2.2"}})
-    #deque.log_artifact_task(artifact_type=RESOURCES, path="//dequeapp.egg-info",
-       #                     run_meta_data=None)
+    # deque.log_artifact_task(artifact_type=RESOURCES, path="//dequeapp.egg-info",
+    #                     run_meta_data=None)
     # deque.init(user_name="riju@deque.app", project_name="awesome-dude")
     # for i in range(100):
     # deque.log(data={"train": {"accuracy": i, "loss": i - 100}, "image": deque.im})
 
     # deque.log(data={"image":deque.im})
```

### Comparing `dequeai-0.745/dequeai/parsing_service.py` & `dequeai-0.746/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.745/dequeai/rest_connect.py` & `dequeai-0.746/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.745/dequeai/util.py` & `dequeai-0.746/dequeai/util.py`

 * *Files identical despite different names*

