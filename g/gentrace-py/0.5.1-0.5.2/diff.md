# Comparing `tmp/gentrace_py-0.5.1.tar.gz` & `tmp/gentrace_py-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.5.1.tar", max compression
+gzip compressed data, was "gentrace_py-0.5.2.tar", max compression
```

## Comparing `gentrace_py-0.5.1.tar` & `gentrace_py-0.5.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      972 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-21 14:42:33.149020 gentrace_py-0.5.1/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      666 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    24193 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6399 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      695 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12220 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/gentrace/schemas.py
--rw-r--r--   0        0        0     1298 2023-04-21 14:42:33.153020 gentrace_py-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      972 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      766 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    24193 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6400 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      695 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12220 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/schemas.py
+-rw-r--r--   0        0        0     1571 2023-04-24 10:28:53.083036 gentrace_py-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.2/PKG-INFO
```

### Comparing `gentrace_py-0.5.1/gentrace/__init__.py` & `gentrace_py-0.5.2/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/api_client.py` & `gentrace_py-0.5.2/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/configuration.py` & `gentrace_py-0.5.2/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/exceptions.py` & `gentrace_py-0.5.2/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/feedback_request.py` & `gentrace_py-0.5.2/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/feedback_request.pyi` & `gentrace_py-0.5.2/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/feedback_response.py` & `gentrace_py-0.5.2/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/feedback_response.pyi` & `gentrace_py-0.5.2/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.5.2/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.5.2/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.5.2/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.5.2/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/models/__init__.py` & `gentrace_py-0.5.2/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/providers/getters.py` & `gentrace_py-0.5.2/gentrace/providers/getters.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,24 @@
 
 import openai
 
 from gentrace.configuration import Configuration as GentraceConfiguration
 
 openai.api_key = os.getenv("OPENAI_KEY")
 
+configured = False
+
 
 def configure_openai():
+    global configured
+
+    if configured:
+        return
+
+    configured = True
     from gentrace import api_key, host
 
     from .llms.openai import annotate_openai_module
 
     gentrace_config = GentraceConfiguration(host=host)
     gentrace_config.access_token = api_key
```

### Comparing `gentrace_py-0.5.1/gentrace/providers/llms/openai.py` & `gentrace_py-0.5.2/gentrace/providers/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/providers/pipeline.py` & `gentrace_py-0.5.2/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/providers/pipeline_run.py` & `gentrace_py-0.5.2/gentrace/providers/pipeline_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         except Exception as e:
             print(f"Error submitting to Gentrace: {e}")
             return {"pipelineRunId": None}
 
     def submit(self, wait_for_server=False) -> Dict:
         configuration = Configuration(host=self.pipeline.config.get("host"))
         configuration.access_token = self.pipeline.config.get("api_key")
+
         api_client = ApiClient(configuration=configuration)
         ingestion_api = IngestionApi(api_client=api_client)
 
         step_runs_data = [
             {
                 "provider": {
                     "name": step_run.provider,
```

### Comparing `gentrace_py-0.5.1/gentrace/providers/step_run.py` & `gentrace_py-0.5.2/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/providers/utils.py` & `gentrace_py-0.5.2/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.5.2/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/rest.py` & `gentrace_py-0.5.2/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/gentrace/schemas.py` & `gentrace_py-0.5.2/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.1/PKG-INFO` & `gentrace_py-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,11 +16,12 @@
 Provides-Extra: vectorstores
 Requires-Dist: aenum (>=3.1.11)
 Requires-Dist: frozendict (>=2.3.7,<3.0.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0) ; extra == "all" or extra == "llms"
 Requires-Dist: pinecone-client (>=2.2.1,<3.0.0) ; extra == "all" or extra == "vectorstores"
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: pystache (>=0.6.0,<0.7.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python_dateutil (>=2.5.3)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: urllib3 (>=1.25.3)
 Project-URL: Repository, https://github.com/gentrace/gentrace-python
```

