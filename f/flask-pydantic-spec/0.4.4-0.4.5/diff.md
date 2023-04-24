# Comparing `tmp/flask_pydantic_spec-0.4.4.tar.gz` & `tmp/flask_pydantic_spec-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_pydantic_spec-0.4.4.tar", last modified: Mon Apr 17 10:03:22 2023, max compression
+gzip compressed data, was "flask_pydantic_spec-0.4.5.tar", last modified: Mon Apr 24 12:17:13 2023, max compression
```

## Comparing `flask_pydantic_spec-0.4.4.tar` & `flask_pydantic_spec-0.4.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:03:22.383046 flask_pydantic_spec-0.4.4/flask_pydantic_spec/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/flask_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/page.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 10:03:22.000000 flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 10:03:22.387046 flask_pydantic_spec-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-17 10:03:13.000000 flask_pydantic_spec-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:17:13.587450 flask_pydantic_spec-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-24 12:17:13.587450 flask_pydantic_spec-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:17:13.587450 flask_pydantic_spec-0.4.5/flask_pydantic_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/flask_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:17:13.587450 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 12:17:13.000000 flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 12:17:13.587450 flask_pydantic_spec-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-24 12:17:02.000000 flask_pydantic_spec-0.4.5/setup.py
```

### Comparing `flask_pydantic_spec-0.4.4/LICENSE` & `flask_pydantic_spec-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.4/PKG-INFO` & `flask_pydantic_spec-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_pydantic_spec
-Version: 0.4.4
+Version: 0.4.5
 Summary: generate OpenAPI document and validate request & response with Python annotations.
 Home-page: https://github.com/turner-townsend/flask-pydantic-spec
 Author: Chris Gearing, Simon Hayward, Rob Young, Donald Fleming, Saurabh Jha
 Author-email: chris.gearing@turntown.digital
 License: UNKNOWN
 Description: # Flask Pydantic Spec
```

### Comparing `flask_pydantic_spec-0.4.4/README.md` & `flask_pydantic_spec-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec/config.py` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec/config.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec/flask_backend.py` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec/flask_backend.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec/page.py` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec/page.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec/spec.py` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from collections import defaultdict
-from copy import copy, deepcopy
+from copy import deepcopy
 from functools import wraps
 from typing import Mapping, Optional, Type, Union, Callable, Iterable, Any, Dict, List
 
 from flask import Flask, Response as FlaskResponse
 from pydantic import BaseModel
 from inflection import camelize
 
 from . import Request
 from .config import Config
+from .constants import OPENAPI_SCHEMA_TEMPLATE
 from .flask_backend import FlaskBackend
 from .types import RequestBase, ResponseBase
 from .utils import (
     parse_comments,
     parse_request,
     parse_params,
     parse_resp,
     parse_name,
     default_before_handler,
     default_after_handler,
 )
 
-OPENAPI_SCHEMA_TEMPLATE = "#/components/schemas/{model}"
-
 
 def _move_schema_reference(reference: str) -> str:
     if "/definitions" in reference:
         return f"#/components/schemas/{reference.split('/definitions/')[-1]}"
     return reference
```

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec/types.py` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 from typing import Optional, Type, Iterable, Mapping, Any, Dict
 
 from pydantic import BaseModel
 
+from flask_pydantic_spec.constants import OPENAPI_SCHEMA_TEMPLATE
+
 
 class ResponseBase:
     """
     Base Class for Response Types
     """
 
     def has_model(self) -> bool:
@@ -176,15 +178,15 @@
         self.file_key = file_key
         self.encoding = encoding
 
     def has_model(self) -> bool:
         return self.model is not None
 
     def generate_spec(self) -> Mapping[str, Any]:
-        model_spec = self.model.schema() if self.model else None
+        model_spec = self.model.schema(ref_template=OPENAPI_SCHEMA_TEMPLATE) if self.model else None
         if model_spec:
             additional_properties = model_spec["properties"]
         else:
             additional_properties = {}
 
         return {
             "content": {
```

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec/utils.py` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec/utils.py`

 * *Files identical despite different names*

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/PKG-INFO` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-pydantic-spec
-Version: 0.4.4
+Version: 0.4.5
 Summary: generate OpenAPI document and validate request & response with Python annotations.
 Home-page: https://github.com/turner-townsend/flask-pydantic-spec
 Author: Chris Gearing, Simon Hayward, Rob Young, Donald Fleming, Saurabh Jha
 Author-email: chris.gearing@turntown.digital
 License: UNKNOWN
 Description: # Flask Pydantic Spec
```

### Comparing `flask_pydantic_spec-0.4.4/flask_pydantic_spec.egg-info/SOURCES.txt` & `flask_pydantic_spec-0.4.5/flask_pydantic_spec.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 flask_pydantic_spec/__init__.py
 flask_pydantic_spec/config.py
+flask_pydantic_spec/constants.py
 flask_pydantic_spec/flask_backend.py
 flask_pydantic_spec/page.py
 flask_pydantic_spec/spec.py
 flask_pydantic_spec/types.py
 flask_pydantic_spec/utils.py
 flask_pydantic_spec.egg-info/PKG-INFO
 flask_pydantic_spec.egg-info/SOURCES.txt
```

### Comparing `flask_pydantic_spec-0.4.4/setup.py` & `flask_pydantic_spec-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open(path.join(here, "requirements/production.txt"), encoding="utf-8") as f:
     requires = [req.strip() for req in f if req]
 
 
 setup(
     name="flask_pydantic_spec",
-    version="0.4.4",
+    version="0.4.5",
     author="Chris Gearing, Simon Hayward, Rob Young, Donald Fleming, Saurabh Jha",
     author_email="chris.gearing@turntown.digital",
     description=(
         "generate OpenAPI document and validate request & response "
         "with Python annotations."
     ),
     long_description=readme,
```

