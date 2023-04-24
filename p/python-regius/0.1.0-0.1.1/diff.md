# Comparing `tmp/python_regius-0.1.0.tar.gz` & `tmp/python_regius-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_regius-0.1.0.tar", max compression
+gzip compressed data, was "python_regius-0.1.1.tar", max compression
```

## Comparing `python_regius-0.1.0.tar` & `python_regius-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       59 2023-04-23 23:35:15.384800 python_regius-0.1.0/README.md
--rw-r--r--   0        0        0      753 2023-04-23 23:39:54.042539 python_regius-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       94 2023-04-23 21:27:23.659621 python_regius-0.1.0/regius/__init__.py
--rw-r--r--   0        0        0      997 2023-04-23 23:04:52.162754 python_regius-0.1.0/regius/client.py
--rw-r--r--   0        0        0     3172 2023-04-23 23:20:02.386829 python_regius-0.1.0/regius/server.py
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 python_regius-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-23 23:35:15.384800 python_regius-0.1.1/README.md
+-rw-r--r--   0        0        0      728 2023-04-24 00:24:41.815654 python_regius-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-04-23 21:27:23.659621 python_regius-0.1.1/regius/__init__.py
+-rw-r--r--   0        0        0     1151 2023-04-24 00:21:25.420313 python_regius-0.1.1/regius/client.py
+-rw-r--r--   0        0        0     3185 2023-04-24 00:23:31.372352 python_regius-0.1.1/regius/server.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 python_regius-0.1.1/PKG-INFO
```

### Comparing `python_regius-0.1.0/pyproject.toml` & `python_regius-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "python-regius"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python Regius - A simple & friendly Python RPC framework."
 authors = ["王见充 <gerhut@sya.org.cn>"]
 license = "Proprietary"
 readme = "README.md"
 repository = "https://jihulab.com/Sya/Regius/regius.git"
 
 [[tool.poetry.packages]]
 include = "regius"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.23.0"
-python-dotenv = "^1.0.0"
 sanic = "^23.3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.3.1"
```

### Comparing `python_regius-0.1.0/regius/client.py` & `python_regius-0.1.1/regius/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from os import environ
 
 from httpx import AsyncClient
 
 __all__ = ["import_module", "RegiusModule"]
 
+_environ = environ.copy()
+
+try:
+    from dotenv import dotenv_values
+
+    _environ = {**dotenv_values(".env"), **_environ}
+except ImportError:
+    pass
+
 
 class RegiusModule(object):
     _endpoint_override: dict[str, str] = {}
-    _endpoint_template = environ.get("REGIUS_ENDPOINT_TEMPLATE", "http://{name}")
+    _endpoint_template = _environ.get("REGIUS_ENDPOINT_TEMPLATE", "http://{name}")
 
     def __init__(self, name: str):
         endpoint = self._endpoint_override.get(name)
         if endpoint is None:
             endpoint = self._endpoint_template.format(name=name)
 
         self._client = AsyncClient(base_url=endpoint)
```

### Comparing `python_regius-0.1.0/regius/server.py` & `python_regius-0.1.1/regius/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sanic.log import logger
 
 __all__ = ["app", "RegiusApp"]
 
 
 class RegiusApp(Sanic):
     def __init__(self, path: str, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super().__init__(name="regius_app", *args, **kwargs)
 
         path = os.path.join(path, "__init__.py")
         module = _load_module(path)
         _install_handlers(self, module.__dict__)
 
 
 def app(*args, **kwargs):
@@ -45,15 +45,15 @@
         if name.startswith("_"):
             continue
 
         if not isfunction(value):
             logger.warning("Skipping %s because it is not a function", name)
             continue
 
-        logger.info("Registering async function %s", name)
+        logger.info("Registering function %s", name)
         handler = _create_handler(value)
         app.add_route(handler, f"/{name}", methods=["POST"], name=name)
 
 
 def _create_handler(func: Callable):
     if iscoroutinefunction(func):
         return _handle_async(func)
```

### Comparing `python_regius-0.1.0/PKG-INFO` & `python_regius-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: python-regius
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Regius - A simple & friendly Python RPC framework.
 Home-page: https://jihulab.com/Sya/Regius/regius.git
 License: Proprietary
 Author: 王见充
 Author-email: gerhut@sya.org.cn
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sanic (>=23.3.0,<24.0.0)
 Project-URL: Repository, https://jihulab.com/Sya/Regius/regius.git
 Description-Content-Type: text/markdown
 
 # Python Regius
 
 A simple & friendly Python RPC framework.
```

