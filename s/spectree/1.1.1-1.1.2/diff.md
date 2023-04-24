# Comparing `tmp/spectree-1.1.1.tar.gz` & `tmp/spectree-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectree-1.1.1.tar", last modified: Sun Apr 23 04:48:59 2023, max compression
+gzip compressed data, was "spectree-1.1.2.tar", last modified: Mon Apr 24 13:26:47 2023, max compression
```

## Comparing `spectree-1.1.1.tar` & `spectree-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.398696 spectree-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-23 04:48:45.000000 spectree-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 04:48:45.000000 spectree-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-23 04:48:59.398696 spectree-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-23 04:48:45.000000 spectree-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 04:48:45.000000 spectree-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 04:48:59.398696 spectree-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-23 04:48:45.000000 spectree-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.394696 spectree-1.1.1/spectree/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.394696 spectree-1.1.1/spectree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/falcon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/flask_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/quart_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/plugins/starlette_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-23 04:48:45.000000 spectree-1.1.1/spectree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.394696 spectree-1.1.1/spectree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 04:48:59.000000 spectree-1.1.1/spectree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:48:59.398696 spectree-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_falcon_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_flask_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_flask_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_quart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_plugin_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-23 04:48:45.000000 spectree-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.396857 spectree-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-24 13:26:32.000000 spectree-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 13:26:32.000000 spectree-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-24 13:26:47.396857 spectree-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-04-24 13:26:32.000000 spectree-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-24 13:26:32.000000 spectree-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:26:47.396857 spectree-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:26:32.000000 spectree-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.392857 spectree-1.1.2/spectree/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.392857 spectree-1.1.2/spectree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/falcon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/flask_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/quart_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/plugins/starlette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-24 13:26:32.000000 spectree-1.1.2/spectree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.392857 spectree-1.1.2/spectree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:26:47.000000 spectree-1.1.2/spectree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:26:47.396857 spectree-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_falcon_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_flask_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_flask_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_quart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_plugin_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-24 13:26:32.000000 spectree-1.1.2/tests/test_utils.py
```

### Comparing `spectree-1.1.1/LICENSE` & `spectree-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/PKG-INFO` & `spectree-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.1
+Version: 1.1.2
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
```

### Comparing `spectree-1.1.1/README.md` & `spectree-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/pyproject.toml` & `spectree-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spectree"
-version = "1.1.1"
+version = "1.1.2"
 dynamic = []
 description = "generate OpenAPI document and validate request&response with Python annotations."
 readme = "README.md"
 license = {text = "Apache-2.0"}
 requires-python = ">=3.6"
 authors = [
     { name = "Keming Yang", email = "kemingy94@gmail.com" },
```

### Comparing `spectree-1.1.1/setup.py` & `spectree-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/_types.py` & `spectree-1.1.2/spectree/_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from pydantic import BaseModel
 from typing_extensions import Protocol
 
 ModelType = Type[BaseModel]
 OptionalModelType = Optional[ModelType]
 NamingStrategy = Callable[[ModelType], str]
+NestedNamingStrategy = Callable[[str, str], str]
 
 
 class MultiDict(Protocol):
     def get(self, key: str) -> Optional[str]:
         ...
 
     def getlist(self, key: str) -> List[str]:
```

### Comparing `spectree-1.1.1/spectree/config.py` & `spectree-1.1.2/spectree/config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/models.py` & `spectree-1.1.2/spectree/models.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/page.py` & `spectree-1.1.2/spectree/page.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/plugins/__init__.py` & `spectree-1.1.2/spectree/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/plugins/base.py` & `spectree-1.1.2/spectree/plugins/base.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/plugins/falcon_plugin.py` & `spectree-1.1.2/spectree/plugins/falcon_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/plugins/flask_plugin.py` & `spectree-1.1.2/spectree/plugins/flask_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/plugins/quart_plugin.py` & `spectree-1.1.2/spectree/plugins/quart_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/plugins/starlette_plugin.py` & `spectree-1.1.2/spectree/plugins/starlette_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/response.py` & `spectree-1.1.2/spectree/response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/spectree/spec.py` & `spectree-1.1.2/spectree/spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,25 @@
     Mapping,
     Optional,
     Sequence,
     Type,
     get_type_hints,
 )
 
-from ._types import FunctionDecorator, ModelType, NamingStrategy
+from ._types import FunctionDecorator, ModelType, NamingStrategy, NestedNamingStrategy
 from .config import Configuration, ModeEnum
 from .models import Tag, ValidationError
 from .plugins import PLUGINS, BasePlugin
 from .response import Response
 from .utils import (
     default_after_handler,
     default_before_handler,
     get_model_key,
     get_model_schema,
+    get_nested_key,
     get_security,
     parse_comments,
     parse_name,
     parse_params,
     parse_request,
     parse_resp,
 )
@@ -61,17 +62,19 @@
         backend: Optional[Type[BasePlugin]] = None,
         app: Any = None,
         before: Callable = default_before_handler,
         after: Callable = default_after_handler,
         validation_error_status: int = 422,
         validation_error_model: Optional[ModelType] = None,
         naming_strategy: NamingStrategy = get_model_key,
+        nested_naming_strategy: NestedNamingStrategy = get_nested_key,
         **kwargs: Any,
     ):
         self.naming_strategy = naming_strategy
+        self.nested_naming_strategy = nested_naming_strategy
         self.before = before
         self.after = after
         self.validation_error_status = validation_error_status
         self.validation_error_model = validation_error_model or ValidationError
         self.config: Configuration = Configuration.parse_obj(kwargs)
         self.backend_name = backend_name
         if backend:
@@ -257,15 +260,19 @@
     def _add_model(self, model: ModelType) -> str:
         """
         unified model processing
         """
 
         model_key = self.naming_strategy(model)
         self.models[model_key] = deepcopy(
-            get_model_schema(model=model, naming_strategy=self.naming_strategy)
+            get_model_schema(
+                model=model,
+                naming_strategy=self.naming_strategy,
+                nested_naming_strategy=self.nested_naming_strategy,
+            )
         )
 
         return model_key
 
     def _generate_spec(self) -> Dict[str, Any]:
         """
         generate OpenAPI spec according to routes and decorators
@@ -346,11 +353,13 @@
         """
         handle nested models
         """
         definitions = {}
         for name, schema in self.models.items():
             if "definitions" in schema:
                 for key, value in schema["definitions"].items():
-                    definitions[f"{name}.{key}"] = value
+                    composed_key = self.nested_naming_strategy(name, key)
+                    if composed_key not in definitions:
+                        definitions[composed_key] = value
                 del schema["definitions"]
 
         return definitions
```

### Comparing `spectree-1.1.1/spectree/utils.py` & `spectree-1.1.2/spectree/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Tuple,
     Type,
     Union,
 )
 
 from pydantic import BaseModel, ValidationError
 
-from ._types import ModelType, MultiDict, NamingStrategy
+from ._types import ModelType, MultiDict, NamingStrategy, NestedNamingStrategy
 
 # parse HTTP status code to get the code
 HTTP_CODE = re.compile(r"^HTTP_(?P<code>\d{3})$")
 
 RE_FLASK_RULE = re.compile(
     r"""
     (?P<static>[^<]*)                           # static rule data
@@ -225,27 +225,42 @@
     :param model: `pydantic.BaseModel` query, json, headers or cookies from
         request or response
     """
 
     return f"{model.__name__}.{hash_module_path(module_path=model.__module__)}"
 
 
-def get_model_schema(model: ModelType, naming_strategy: NamingStrategy = get_model_key):
+def get_nested_key(parent: str, child: str) -> str:
+    """
+    generate nested model reference name suffixed by parent model name
+
+    :param parent: string of parent name
+    :param child: string of child name
+    """
+
+    return f"{parent}.{child}"
+
+
+def get_model_schema(
+    model: ModelType,
+    naming_strategy: NamingStrategy = get_model_key,
+    nested_naming_strategy: NestedNamingStrategy = get_nested_key,
+):
     """
     return a dictionary representing the model as JSON Schema with a hashed
     infix in ref to ensure name uniqueness
 
     :param model: `pydantic.BaseModel` query, json, headers or cookies from
         request or response
     """
     assert issubclass(model, BaseModel)
 
-    return model.schema(
-        ref_template=f"#/components/schemas/{naming_strategy(model)}.{{model}}"
-    )
+    nested_key = nested_naming_strategy(naming_strategy(model), "{model}")
+
+    return model.schema(ref_template=f"#/components/schemas/{nested_key}")
 
 
 def get_security(security: Union[None, Mapping, Sequence[Any]]) -> List[Any]:
     """
     return the correct format of security
     """
     if security is None or not security:
```

### Comparing `spectree-1.1.1/spectree.egg-info/PKG-INFO` & `spectree-1.1.2/spectree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.1
+Version: 1.1.2
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
```

### Comparing `spectree-1.1.1/spectree.egg-info/SOURCES.txt` & `spectree-1.1.2/spectree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_config.py` & `spectree-1.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin.py` & `spectree-1.1.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_falcon.py` & `spectree-1.1.2/tests/test_plugin_falcon.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_falcon_asgi.py` & `spectree-1.1.2/tests/test_plugin_falcon_asgi.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_flask.py` & `spectree-1.1.2/tests/test_plugin_flask.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_flask_blueprint.py` & `spectree-1.1.2/tests/test_plugin_flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_flask_view.py` & `spectree-1.1.2/tests/test_plugin_flask_view.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_quart.py` & `spectree-1.1.2/tests/test_plugin_quart.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_plugin_starlette.py` & `spectree-1.1.2/tests/test_plugin_starlette.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_response.py` & `spectree-1.1.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_spec.py` & `spectree-1.1.2/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.1/tests/test_utils.py` & `spectree-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

