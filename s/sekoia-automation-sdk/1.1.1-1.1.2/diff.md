# Comparing `tmp/sekoia_automation_sdk-1.1.1.tar.gz` & `tmp/sekoia_automation_sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.1.1.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.1.2.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.1.1.tar` & `sekoia_automation_sdk-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1066 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/LICENSE
--rw-r--r--   0        0        0     8422 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/README.md
--rw-r--r--   0        0        0     2114 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11220 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/action.py
--rw-r--r--   0        0        0     3795 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/config.py
--rw-r--r--   0        0        0     6469 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/connector.py
--rw-r--r--   0        0        0      426 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15477 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-03-28 12:36:00.637033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      647 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10005 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/openapi.py
--rw-r--r--   0        0        0     4626 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/storage.py
--rw-r--r--   0        0        0    10724 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-03-28 12:36:00.641033 sekoia_automation_sdk-1.1.1/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/LICENSE
+-rw-r--r--   0        0        0     8422 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/README.md
+-rw-r--r--   0        0        0     2114 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11220 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/action.py
+-rw-r--r--   0        0        0     3795 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6534 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/connector.py
+-rw-r--r--   0        0        0      426 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15477 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      647 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10005 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/openapi.py
+-rw-r--r--   0        0        0     4626 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    10724 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.1.2/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.1.1/LICENSE` & `sekoia_automation_sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/README.md` & `sekoia_automation_sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/pyproject.toml` & `sekoia_automation_sdk-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.1.1"
+version = "1.1.2"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/action.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/cli.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/config.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/connector.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,22 +80,24 @@
             self.log_exception(ex, message=f"Failed to forward {len(chunk)} events")
 
     def push_events_to_intakes(self, events: list[str]) -> list:
         # no event to push
         if not events:
             return []
 
-        self._last_events = datetime.utcnow()
+        self._last_events_time = datetime.utcnow()
         intake_host = self.configuration.intake_server
         batch_api = urljoin(intake_host, "/batch")
 
         # Dict to collect event_ids for the API
         collect_ids: dict[int, list] = {}
 
         # pushing the events
+        if self._stop_event.is_set():
+            return []
         chunks = self._chunk_events(events, self.configuration.chunk_size)
         futures = [
             self._executor.submit(
                 self._send_chunk, batch_api, chunk_index, chunk, collect_ids
             )
             for chunk_index, chunk in enumerate(chunks)
         ]
```

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/module.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/trigger.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.1.2/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.1/PKG-INFO` & `sekoia_automation_sdk-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

