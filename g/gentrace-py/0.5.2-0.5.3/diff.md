# Comparing `tmp/gentrace_py-0.5.2.tar.gz` & `tmp/gentrace_py-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.5.2.tar", max compression
+gzip compressed data, was "gentrace_py-0.5.3.tar", max compression
```

## Comparing `gentrace_py-0.5.2.tar` & `gentrace_py-0.5.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      972 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      766 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    24193 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6400 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      695 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12220 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-24 10:28:53.079036 gentrace_py-0.5.2/gentrace/schemas.py
--rw-r--r--   0        0        0     1571 2023-04-24 10:28:53.083036 gentrace_py-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      968 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    25461 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6400 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      695 2023-04-24 15:48:58.139451 gentrace_py-0.5.3/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-24 15:48:58.143451 gentrace_py-0.5.3/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12220 2023-04-24 15:48:58.143451 gentrace_py-0.5.3/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-24 15:48:58.143451 gentrace_py-0.5.3/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-24 15:48:58.143451 gentrace_py-0.5.3/gentrace/schemas.py
+-rw-r--r--   0        0        0     1571 2023-04-24 15:48:58.143451 gentrace_py-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.3/PKG-INFO
```

### Comparing `gentrace_py-0.5.2/gentrace/__init__.py` & `gentrace_py-0.5.3/gentrace/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 
 # flake8: noqa
 
-"""
-    Gentrace API
+""" Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
     The version of the OpenAPI document: 0.4.8
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `gentrace_py-0.5.2/gentrace/api_client.py` & `gentrace_py-0.5.3/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/configuration.py` & `gentrace_py-0.5.3/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/exceptions.py` & `gentrace_py-0.5.3/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/feedback_request.py` & `gentrace_py-0.5.3/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/feedback_request.pyi` & `gentrace_py-0.5.3/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/feedback_response.py` & `gentrace_py-0.5.3/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/feedback_response.pyi` & `gentrace_py-0.5.3/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.5.3/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.5.3/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.5.3/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.5.3/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/models/__init__.py` & `gentrace_py-0.5.3/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.5.3/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.5.3/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/providers/getters.py` & `gentrace_py-0.5.3/gentrace/providers/getters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-import importlib.util
 import os
-from typing import Any, Dict, Optional, cast
 
 import openai
 
 from gentrace.configuration import Configuration as GentraceConfiguration
 
 openai.api_key = os.getenv("OPENAI_KEY")
 
-configured = False
-
 
 def configure_openai():
-    global configured
-
-    if configured:
-        return
-
-    configured = True
     from gentrace import api_key, host
 
     from .llms.openai import annotate_openai_module
 
+    if not api_key:
+        raise ValueError("Gentrace API key not set")
+
     gentrace_config = GentraceConfiguration(host=host)
     gentrace_config.access_token = api_key
 
     annotate_openai_module(gentrace_config=gentrace_config)
 
 
 def configure_pinecone():
```

### Comparing `gentrace_py-0.5.2/gentrace/providers/llms/openai.py` & `gentrace_py-0.5.3/gentrace/providers/llms/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -637,32 +637,46 @@
                 )
 
         return completion
 
     return wrapper
 
 
+def swap_methods(cls, attribute: str, gentrace_config: Configuration, intercept_fn):
+    has_old_sync_saved = hasattr(cls, attribute + "_old")
+    original_create = getattr(cls, attribute)
+    if has_old_sync_saved:
+        original_create = getattr(cls, attribute + "_old")
+    else:
+        setattr(cls, attribute + "_old", getattr(cls, attribute))
+
+    setattr(cls, attribute, intercept_fn(original_create, gentrace_config))
+
+
 def annotate_openai_module(
     gentrace_config: Configuration,
 ):
     import openai
 
     for name, cls in vars(openai.api_resources).items():
         if isinstance(cls, type):
             if name == "Completion":
-                cls.create = intercept_completion(cls.create, gentrace_config)
-                cls.acreate = intercept_completion_async(cls.acreate, gentrace_config)
+                swap_methods(cls, "create", gentrace_config, intercept_completion)
+                swap_methods(
+                    cls, "acreate", gentrace_config, intercept_completion_async
+                )
             elif name == "ChatCompletion":
-                cls.create = intercept_chat_completion(cls.create, gentrace_config)
-                cls.acreate = intercept_chat_completion_async(
-                    cls.acreate, gentrace_config
+                swap_methods(cls, "create", gentrace_config, intercept_chat_completion)
+                swap_methods(
+                    cls, "acreate", gentrace_config, intercept_chat_completion_async
                 )
+
             elif name == "Embedding":
-                cls.create = intercept_embedding(cls.create, gentrace_config)
-                cls.acreate = intercept_embedding_async(cls.acreate, gentrace_config)
+                swap_methods(cls, "create", gentrace_config, intercept_embedding)
+                swap_methods(cls, "acreate", gentrace_config, intercept_embedding_async)
 
             setattr(openai.api_resources, name, cls)
 
 
 def annotate_pipeline_handler(
     handler: OpenAIPipelineHandler,
     gentrace_config: Configuration,
@@ -672,33 +686,49 @@
 
     for name, cls in vars(openai.api_resources).items():
         if isinstance(cls, type):
             # Create new class that inherits from the original class, don't directly monkey patch
             # the original class
             new_class = type(name, (cls,), {})
             if name == "Completion":
+                original_create = (
+                    cls.create_old if hasattr(cls, "create_old") else cls.create
+                )
                 new_class.create = intercept_completion(
-                    new_class.create, gentrace_config
+                    original_create, gentrace_config
+                )
+                original_acreate = (
+                    cls.acreate_old if hasattr(cls, "acreate_old") else cls.acreate
                 )
                 new_class.acreate = intercept_completion_async(
-                    new_class.acreate, gentrace_config
+                    original_acreate, gentrace_config
                 )
             elif name == "ChatCompletion":
+                original_create = (
+                    cls.create_old if hasattr(cls, "create_old") else cls.create
+                )
                 new_class.create = intercept_chat_completion(
-                    new_class.create, gentrace_config
+                    original_create, gentrace_config
+                )
+                original_acreate = (
+                    cls.acreate_old if hasattr(cls, "acreate_old") else cls.acreate
                 )
                 new_class.acreate = intercept_chat_completion_async(
-                    new_class.acreate, gentrace_config
+                    original_acreate, gentrace_config
                 )
             elif name == "Embedding":
-                new_class.create = intercept_embedding(
-                    new_class.create, gentrace_config
+                original_create = (
+                    cls.create_old if hasattr(cls, "create_old") else cls.create
+                )
+                new_class.create = intercept_embedding(original_create, gentrace_config)
+                original_acreate = (
+                    cls.acreate_old if hasattr(cls, "acreate_old") else cls.acreate
                 )
                 new_class.acreate = intercept_embedding_async(
-                    new_class.acreate, gentrace_config
+                    original_acreate, gentrace_config
                 )
 
             new_class.pipeline_run = pipeline_run
             setattr(handler, name, new_class)
 
     return handler
```

### Comparing `gentrace_py-0.5.2/gentrace/providers/pipeline.py` & `gentrace_py-0.5.3/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/providers/pipeline_run.py` & `gentrace_py-0.5.3/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/providers/step_run.py` & `gentrace_py-0.5.3/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/providers/utils.py` & `gentrace_py-0.5.3/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.5.3/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/rest.py` & `gentrace_py-0.5.3/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/gentrace/schemas.py` & `gentrace_py-0.5.3/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.2/pyproject.toml` & `gentrace_py-0.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.5.2"
+version = "0.5.3"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
```

### Comparing `gentrace_py-0.5.2/PKG-INFO` & `gentrace_py-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

