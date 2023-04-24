# Comparing `tmp/connexion-3.0.0a5.tar.gz` & `tmp/connexion-3.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connexion-3.0.0a5.tar", max compression
+gzip compressed data, was "connexion-3.0.0a6.tar", max compression
```

## Comparing `connexion-3.0.0a5.tar` & `connexion-3.0.0a6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     3091 2023-04-22 20:10:31.091928 connexion-3.0.0a5/ARCHITECTURE.rst
--rw-r--r--   0        0        0      878 2023-04-22 20:10:31.091928 connexion-3.0.0a5/CONTRIBUTING.rst
--rw-r--r--   0        0        0      556 2023-04-22 20:10:31.091928 connexion-3.0.0a5/LICENSE.txt
--rw-r--r--   0        0        0    25923 2023-04-22 20:10:31.091928 connexion-3.0.0a5/README.rst
--rwxr-xr-x   0        0        0     1351 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/__init__.py
--rw-r--r--   0        0        0      144 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/__main__.py
--rw-r--r--   0        0        0      250 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/__init__.py
--rw-r--r--   0        0        0    12633 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/abstract.py
--rw-r--r--   0        0        0     7794 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/asynchronous.py
--rw-r--r--   0        0        0    10558 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/apps/flask.py
--rw-r--r--   0        0        0     5332 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/cli.py
--rw-r--r--   0        0        0      981 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/context.py
--rw-r--r--   0        0        0     1081 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/datastructures.py
--rw-r--r--   0        0        0      174 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/__init__.py
--rw-r--r--   0        0        0     6489 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/main.py
--rw-r--r--   0        0        0    15027 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/parameter.py
--rw-r--r--   0        0        0     7026 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/decorators/response.py
--rw-r--r--   0        0        0     5541 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/__init__.py
--rw-r--r--   0        0        0     1069 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/abstract.py
--rw-r--r--   0        0        0     4096 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/flask.py
--rw-r--r--   0        0        0     2795 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/frameworks/starlette.py
--rw-r--r--   0        0        0     1259 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/handlers.py
--rw-r--r--   0        0        0      227 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/http_facts.py
--rw-r--r--   0        0        0     4661 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/json_schema.py
--rw-r--r--   0        0        0     2856 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/jsonifier.py
--rw-r--r--   0        0        0     6973 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/lifecycle.py
--rw-r--r--   0        0        0      111 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/__init__.py
--rw-r--r--   0        0        0     9843 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/abstract.py
--rw-r--r--   0        0        0     1407 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/context.py
--rw-r--r--   0        0        0     2394 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/exceptions.py
--rw-r--r--   0        0        0      940 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/lifespan.py
--rw-r--r--   0        0        0    17217 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/main.py
--rw-r--r--   0        0        0     6591 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/request_validation.py
--rw-r--r--   0        0        0     5598 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/response_validation.py
--rw-r--r--   0        0        0     4908 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/routing.py
--rw-r--r--   0        0        0     4659 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/security.py
--rw-r--r--   0        0        0     8198 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/middleware/swagger_ui.py
--rw-r--r--   0        0        0     1828 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/mock.py
--rw-r--r--   0        0        0      531 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/__init__.py
--rw-r--r--   0        0        0     6666 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/abstract.py
--rw-r--r--   0        0        0     8983 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/openapi.py
--rw-r--r--   0        0        0    11327 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/operations/swagger2.py
--rw-r--r--   0        0        0     4376 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/options.py
--rw-r--r--   0        0        0     2255 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/problem.py
--rw-r--r--   0        0        0    12118 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/resolver.py
--rw-r--r--   0        0        0    40020 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/resources/schemas/v2.0/schema.json
--rw-r--r--   0        0        0    35456 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/resources/schemas/v3.0/schema.json
--rw-r--r--   0        0        0    21402 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/security.py
--rw-r--r--   0        0        0     9537 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/spec.py
--rw-r--r--   0        0        0     2153 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/testing.py
--rw-r--r--   0        0        0    11661 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/uri_parsing.py
--rw-r--r--   0        0        0    12674 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/utils.py
--rw-r--r--   0        0        0      892 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/__init__.py
--rw-r--r--   0        0        0     7075 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/abstract.py
--rw-r--r--   0        0        0     3280 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/form_data.py
--rw-r--r--   0        0        0     4753 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/json.py
--rw-r--r--   0        0        0     5181 2023-04-22 20:10:31.091928 connexion-3.0.0a5/connexion/validators/parameter.py
--rw-r--r--   0        0        0     2874 2023-04-22 20:10:32.479941 connexion-3.0.0a5/pyproject.toml
--rw-r--r--   0        0        0    28529 1970-01-01 00:00:00.000000 connexion-3.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     3091 2023-04-24 16:58:46.116016 connexion-3.0.0a6/ARCHITECTURE.rst
+-rw-r--r--   0        0        0      878 2023-04-24 16:58:46.116016 connexion-3.0.0a6/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      556 2023-04-24 16:58:46.116016 connexion-3.0.0a6/LICENSE.txt
+-rw-r--r--   0        0        0    25923 2023-04-24 16:58:46.116016 connexion-3.0.0a6/README.rst
+-rwxr-xr-x   0        0        0     1351 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/__main__.py
+-rw-r--r--   0        0        0      250 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/apps/__init__.py
+-rw-r--r--   0        0        0    12633 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/apps/abstract.py
+-rw-r--r--   0        0        0     7794 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/apps/asynchronous.py
+-rw-r--r--   0        0        0    10558 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/apps/flask.py
+-rw-r--r--   0        0        0     5332 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/cli.py
+-rw-r--r--   0        0        0      981 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/context.py
+-rw-r--r--   0        0        0     1081 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/datastructures.py
+-rw-r--r--   0        0        0      174 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/decorators/__init__.py
+-rw-r--r--   0        0        0     6489 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/decorators/main.py
+-rw-r--r--   0        0        0    15027 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/decorators/parameter.py
+-rw-r--r--   0        0        0     7026 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/decorators/response.py
+-rw-r--r--   0        0        0     5541 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/frameworks/__init__.py
+-rw-r--r--   0        0        0     1069 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/frameworks/abstract.py
+-rw-r--r--   0        0        0     4096 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/frameworks/flask.py
+-rw-r--r--   0        0        0     2795 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/frameworks/starlette.py
+-rw-r--r--   0        0        0     1259 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/handlers.py
+-rw-r--r--   0        0        0      227 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/http_facts.py
+-rw-r--r--   0        0        0     4661 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/json_schema.py
+-rw-r--r--   0        0        0     2856 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/jsonifier.py
+-rw-r--r--   0        0        0     6973 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/lifecycle.py
+-rw-r--r--   0        0        0      111 2023-04-24 16:58:46.116016 connexion-3.0.0a6/connexion/middleware/__init__.py
+-rw-r--r--   0        0        0     9843 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/abstract.py
+-rw-r--r--   0        0        0     1407 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/context.py
+-rw-r--r--   0        0        0     2382 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/exceptions.py
+-rw-r--r--   0        0        0      940 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/lifespan.py
+-rw-r--r--   0        0        0    17485 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/main.py
+-rw-r--r--   0        0        0     6591 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/request_validation.py
+-rw-r--r--   0        0        0     5598 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/response_validation.py
+-rw-r--r--   0        0        0     4908 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/routing.py
+-rw-r--r--   0        0        0     4659 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/security.py
+-rw-r--r--   0        0        0     8198 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/middleware/swagger_ui.py
+-rw-r--r--   0        0        0     1828 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/mock.py
+-rw-r--r--   0        0        0      531 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/operations/__init__.py
+-rw-r--r--   0        0        0     6666 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/operations/abstract.py
+-rw-r--r--   0        0        0     8983 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/operations/openapi.py
+-rw-r--r--   0        0        0    11327 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/operations/swagger2.py
+-rw-r--r--   0        0        0     4376 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/options.py
+-rw-r--r--   0        0        0     2255 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/problem.py
+-rw-r--r--   0        0        0    12118 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/resolver.py
+-rw-r--r--   0        0        0    40020 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/resources/schemas/v2.0/schema.json
+-rw-r--r--   0        0        0    35456 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/resources/schemas/v3.0/schema.json
+-rw-r--r--   0        0        0    21402 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/security.py
+-rw-r--r--   0        0        0     9537 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/spec.py
+-rw-r--r--   0        0        0     2153 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/testing.py
+-rw-r--r--   0        0        0    11661 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/uri_parsing.py
+-rw-r--r--   0        0        0    12674 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/utils.py
+-rw-r--r--   0        0        0      892 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/validators/__init__.py
+-rw-r--r--   0        0        0     7075 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/validators/abstract.py
+-rw-r--r--   0        0        0     3280 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/validators/form_data.py
+-rw-r--r--   0        0        0     4753 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/validators/json.py
+-rw-r--r--   0        0        0     5181 2023-04-24 16:58:46.120016 connexion-3.0.0a6/connexion/validators/parameter.py
+-rw-r--r--   0        0        0     2874 2023-04-24 16:58:46.424020 connexion-3.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0    28529 1970-01-01 00:00:00.000000 connexion-3.0.0a6/PKG-INFO
```

### Comparing `connexion-3.0.0a5/ARCHITECTURE.rst` & `connexion-3.0.0a6/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/CONTRIBUTING.rst` & `connexion-3.0.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/LICENSE.txt` & `connexion-3.0.0a6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/README.rst` & `connexion-3.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/__init__.py` & `connexion-3.0.0a6/connexion/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/apps/abstract.py` & `connexion-3.0.0a6/connexion/apps/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/apps/asynchronous.py` & `connexion-3.0.0a6/connexion/apps/asynchronous.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/apps/flask.py` & `connexion-3.0.0a6/connexion/apps/flask.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/cli.py` & `connexion-3.0.0a6/connexion/cli.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/context.py` & `connexion-3.0.0a6/connexion/context.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/datastructures.py` & `connexion-3.0.0a6/connexion/datastructures.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/decorators/main.py` & `connexion-3.0.0a6/connexion/decorators/main.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/decorators/parameter.py` & `connexion-3.0.0a6/connexion/decorators/parameter.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/decorators/response.py` & `connexion-3.0.0a6/connexion/decorators/response.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/exceptions.py` & `connexion-3.0.0a6/connexion/exceptions.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/frameworks/abstract.py` & `connexion-3.0.0a6/connexion/frameworks/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/frameworks/flask.py` & `connexion-3.0.0a6/connexion/frameworks/flask.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/frameworks/starlette.py` & `connexion-3.0.0a6/connexion/frameworks/starlette.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/handlers.py` & `connexion-3.0.0a6/connexion/handlers.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/json_schema.py` & `connexion-3.0.0a6/connexion/json_schema.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/jsonifier.py` & `connexion-3.0.0a6/connexion/jsonifier.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/lifecycle.py` & `connexion-3.0.0a6/connexion/lifecycle.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/abstract.py` & `connexion-3.0.0a6/connexion/middleware/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/context.py` & `connexion-3.0.0a6/connexion/middleware/context.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/exceptions.py` & `connexion-3.0.0a6/connexion/middleware/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,28 @@
     def __init__(self, next_app: ASGIApp):
         super().__init__(next_app)
         self.add_exception_handler(ProblemException, self.problem_handler)
         self.add_exception_handler(Exception, self.common_error_handler)
 
     @staticmethod
     def problem_handler(_request: StarletteRequest, exc: ProblemException):
-        logger.exception(exc)
+        logger.error(exc)
 
         response = exc.to_problem()
 
         return Response(
             content=response.body,
             status_code=response.status_code,
             media_type=response.mimetype,
             headers=response.headers,
         )
 
     @staticmethod
     def http_exception(_request: StarletteRequest, exc: HTTPException) -> Response:
-        logger.exception(exc)
+        logger.error(exc)
 
         headers = exc.headers
 
         connexion_response = problem(
             title=exc.detail, detail=exc.detail, status=exc.status_code, headers=headers
         )
 
@@ -48,15 +48,15 @@
             status_code=connexion_response.status_code,
             media_type=connexion_response.mimetype,
             headers=connexion_response.headers,
         )
 
     @staticmethod
     def common_error_handler(_request: StarletteRequest, exc: Exception) -> Response:
-        logger.exception(exc)
+        logger.error(exc)
 
         response = InternalServerError().to_problem()
 
         return Response(
             content=response.body,
             status_code=response.status_code,
             media_type=response.mimetype,
```

### Comparing `connexion-3.0.0a5/connexion/middleware/lifespan.py` & `connexion-3.0.0a6/connexion/middleware/lifespan.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/main.py` & `connexion-3.0.0a6/connexion/middleware/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import dataclasses
 import enum
 import logging
 import pathlib
 import typing as t
 from dataclasses import dataclass, field
 from functools import partial
@@ -176,15 +177,17 @@
         self.specification_dir = (
             spec_dir if spec_dir.is_absolute() else self.root_path / spec_dir
         )
 
         self.app = app
         self.lifespan = lifespan
         self.middlewares = (
-            middlewares if middlewares is not None else self.default_middlewares
+            middlewares
+            if middlewares is not None
+            else copy.copy(self.default_middlewares)
         )
         self.middleware_stack: t.Optional[t.Iterable[ASGIApp]] = None
         self.apis: t.List[API] = []
         self.error_handlers: t.List[tuple] = []
 
         self.options = _Options(
             arguments=arguments,
@@ -219,19 +222,24 @@
         if self.middleware_stack is not None:
             raise RuntimeError("Cannot add middleware after an application has started")
 
         for m, middleware in enumerate(self.middlewares):
             if isinstance(middleware, partial):
                 middleware = middleware.func
 
-            if middleware == position:
+            if middleware == position.value:
                 self.middlewares.insert(
                     m, t.cast(ASGIApp, partial(middleware_class, **options))
                 )
                 break
+        else:
+            raise ValueError(
+                f"Could not insert middleware at position {position.name}. "
+                f"Please make sure you have a {position.value} in your stack."
+            )
 
     def _build_middleware_stack(self) -> t.Tuple[ASGIApp, t.Iterable[ASGIApp]]:
         """Apply all middlewares to the provided app.
 
         :return: Tuple of the outer middleware wrapping the application and a list of the wrapped
             middlewares, including the wrapped application.
         """
@@ -253,15 +261,15 @@
                         api.specification,
                         base_path=api.base_path,
                         **api.kwargs,
                     )
 
             if isinstance(app, ExceptionMiddleware):
                 for error_handler in self.error_handlers:
-                    app.add_exception_handler(error_handler)
+                    app.add_exception_handler(*error_handler)
 
         return app, list(reversed(apps))
 
     def add_api(
         self,
         specification: t.Union[pathlib.Path, str, dict],
         *,
```

### Comparing `connexion-3.0.0a5/connexion/middleware/request_validation.py` & `connexion-3.0.0a6/connexion/middleware/request_validation.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/response_validation.py` & `connexion-3.0.0a6/connexion/middleware/response_validation.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/routing.py` & `connexion-3.0.0a6/connexion/middleware/routing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/security.py` & `connexion-3.0.0a6/connexion/middleware/security.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/middleware/swagger_ui.py` & `connexion-3.0.0a6/connexion/middleware/swagger_ui.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/mock.py` & `connexion-3.0.0a6/connexion/mock.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/operations/__init__.py` & `connexion-3.0.0a6/connexion/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/operations/abstract.py` & `connexion-3.0.0a6/connexion/operations/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/operations/openapi.py` & `connexion-3.0.0a6/connexion/operations/openapi.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/operations/swagger2.py` & `connexion-3.0.0a6/connexion/operations/swagger2.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/options.py` & `connexion-3.0.0a6/connexion/options.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/problem.py` & `connexion-3.0.0a6/connexion/problem.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/resolver.py` & `connexion-3.0.0a6/connexion/resolver.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/resources/schemas/v2.0/schema.json` & `connexion-3.0.0a6/connexion/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/resources/schemas/v3.0/schema.json` & `connexion-3.0.0a6/connexion/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/security.py` & `connexion-3.0.0a6/connexion/security.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/spec.py` & `connexion-3.0.0a6/connexion/spec.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/testing.py` & `connexion-3.0.0a6/connexion/testing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/uri_parsing.py` & `connexion-3.0.0a6/connexion/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/utils.py` & `connexion-3.0.0a6/connexion/utils.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/validators/__init__.py` & `connexion-3.0.0a6/connexion/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/validators/abstract.py` & `connexion-3.0.0a6/connexion/validators/abstract.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/validators/form_data.py` & `connexion-3.0.0a6/connexion/validators/form_data.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/validators/json.py` & `connexion-3.0.0a6/connexion/validators/json.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/connexion/validators/parameter.py` & `connexion-3.0.0a6/connexion/validators/parameter.py`

 * *Files identical despite different names*

### Comparing `connexion-3.0.0a5/pyproject.toml` & `connexion-3.0.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connexion"
-version = '3.0.0a5'
+version = '3.0.0a6'
 description = "Connexion - API first applications with OpenAPI/Swagger"
 readme = "README.rst"
 keywords = ["api", "swagger", "openapi"]
 license = "Apache-2.0"
 authors = [
     "Daniel Grossmann-Kavanagh <me@danielgk.com>",
     "Henning Jacobs <henning.jacobs@zalando.de>",
```

### Comparing `connexion-3.0.0a5/PKG-INFO` & `connexion-3.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connexion
-Version: 3.0.0a5
+Version: 3.0.0a6
 Summary: Connexion - API first applications with OpenAPI/Swagger
 Home-page: https://github.com/spec-first/connexion
 License: Apache-2.0
 Keywords: api,swagger,openapi
 Author: Daniel Grossmann-Kavanagh
 Author-email: me@danielgk.com
 Maintainer: Robbe Sneyders
```

