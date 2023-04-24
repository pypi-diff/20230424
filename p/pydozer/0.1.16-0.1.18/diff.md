# Comparing `tmp/pydozer-0.1.16.tar.gz` & `tmp/pydozer-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydozer-0.1.16.tar", max compression
+gzip compressed data, was "pydozer-0.1.18.tar", max compression
```

## Comparing `pydozer-0.1.16.tar` & `pydozer-0.1.18.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1075 2023-03-08 02:19:48.717924 pydozer-0.1.16/LICENSE
--rw-r--r--   0        0        0     2938 2023-03-21 08:07:11.316734 pydozer-0.1.16/README.md
--rw-r--r--   0        0        0        0 2023-03-21 08:07:11.316892 pydozer-0.1.16/pydozer/__init__.py
--rw-r--r--   0        0        0     4799 2023-03-21 08:07:11.317319 pydozer-0.1.16/pydozer/api.py
--rw-r--r--   0        0        0     1328 2023-04-07 09:53:36.497225 pydozer-0.1.16/pydozer/auth_pb2.py
--rw-r--r--   0        0        0     2606 2023-04-07 09:53:36.497515 pydozer-0.1.16/pydozer/auth_pb2_grpc.py
--rw-r--r--   0        0        0     2986 2023-04-07 03:31:13.534198 pydozer-0.1.16/pydozer/common_pb2.py
--rw-r--r--   0        0        0     9824 2023-04-07 09:53:36.497873 pydozer-0.1.16/pydozer/common_pb2_grpc.py
--rw-r--r--   0        0        0     1774 2023-04-07 03:28:04.344688 pydozer-0.1.16/pydozer/health_pb2.py
--rw-r--r--   0        0        0     4418 2023-04-07 03:31:22.495001 pydozer-0.1.16/pydozer/health_pb2_grpc.py
--rw-r--r--   0        0        0     4584 2023-03-21 08:07:11.318436 pydozer-0.1.16/pydozer/helper.py
--rw-r--r--   0        0        0     3543 2023-03-21 08:07:11.318702 pydozer-0.1.16/pydozer/ingest.py
--rw-r--r--   0        0        0     3003 2023-04-07 03:31:43.195968 pydozer-0.1.16/pydozer/ingest_pb2.py
--rw-r--r--   0        0        0     7120 2023-04-07 03:31:49.763489 pydozer-0.1.16/pydozer/ingest_pb2_grpc.py
--rw-r--r--   0        0        0     4547 2023-04-07 09:53:36.498202 pydozer-0.1.16/pydozer/types_pb2.py
--rw-r--r--   0        0        0      159 2023-04-07 03:28:04.345106 pydozer-0.1.16/pydozer/types_pb2_grpc.py
--rw-r--r--   0        0        0      557 2023-04-07 09:53:36.498508 pydozer-0.1.16/pyproject.toml
--rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 pydozer-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-04-20 05:32:18.682544 pydozer-0.1.18/LICENSE
+-rw-r--r--   0        0        0     2938 2023-03-21 08:07:11.316734 pydozer-0.1.18/README.md
+-rw-r--r--   0        0        0        0 2023-03-21 08:07:11.316892 pydozer-0.1.18/pydozer/__init__.py
+-rw-r--r--   0        0        0     4993 2023-04-20 05:32:04.733813 pydozer-0.1.18/pydozer/api.py
+-rw-r--r--   0        0        0     2274 2023-04-20 05:32:04.734088 pydozer-0.1.18/pydozer/auth.py
+-rw-r--r--   0        0        0     1328 2023-04-07 09:53:36.497225 pydozer-0.1.18/pydozer/auth_pb2.py
+-rw-r--r--   0        0        0     2606 2023-04-07 09:53:36.497515 pydozer-0.1.18/pydozer/auth_pb2_grpc.py
+-rw-r--r--   0        0        0     2986 2023-04-07 03:31:13.534198 pydozer-0.1.18/pydozer/common_pb2.py
+-rw-r--r--   0        0        0     9824 2023-04-07 09:53:36.497873 pydozer-0.1.18/pydozer/common_pb2_grpc.py
+-rw-r--r--   0        0        0     1774 2023-04-07 03:28:04.344688 pydozer-0.1.18/pydozer/health_pb2.py
+-rw-r--r--   0        0        0     4418 2023-04-07 03:31:22.495001 pydozer-0.1.18/pydozer/health_pb2_grpc.py
+-rw-r--r--   0        0        0     4584 2023-03-21 08:07:11.318436 pydozer-0.1.18/pydozer/helper.py
+-rw-r--r--   0        0        0     3543 2023-03-21 08:07:11.318702 pydozer-0.1.18/pydozer/ingest.py
+-rw-r--r--   0        0        0     3003 2023-04-07 03:31:43.195968 pydozer-0.1.18/pydozer/ingest_pb2.py
+-rw-r--r--   0        0        0     7120 2023-04-07 03:31:49.763489 pydozer-0.1.18/pydozer/ingest_pb2_grpc.py
+-rw-r--r--   0        0        0     4547 2023-04-07 09:53:36.498202 pydozer-0.1.18/pydozer/types_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-07 03:28:04.345106 pydozer-0.1.18/pydozer/types_pb2_grpc.py
+-rw-r--r--   0        0        0      564 2023-04-20 05:32:18.683519 pydozer-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 pydozer-0.1.18/PKG-INFO
```

### Comparing `pydozer-0.1.16/README.md` & `pydozer-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/api.py` & `pydozer-0.1.18/pydozer/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     """Common API client for Dozer
 
     Args:
         endpoint (str): Endpoint to connect to.
         url (str, optional): Dozer gRPC URL. Defaults to Env variable DOZER_API_URL or `0.0.0.0:50051`.
         secure (bool, optional): Intialize a secure channel. Defaults to False.
     """
-    def __init__(self, endpoint, url=DOZER_API_URL, secure=False):
+    def __init__(self, endpoint, url=DOZER_API_URL, secure=False, token=None):
+
+        self.metadata = [('authorization', f'Bearer {token}')] if token else None
+
         if secure:
             channel = grpc.secure_channel(url)
         else:
             channel = grpc.insecure_channel(url)
         self.endpoint = endpoint
         self.channel = channel
         self.client = CommonGrpcServiceStub(channel)
@@ -44,15 +47,15 @@
                                     Eg: `pydozer.generated.trips.Trips` for endpoint `trips`
 
         Returns:
             HealthCheckResponse: _description_
         """
 
         health_client = HealthGrpcServiceStub(self.channel)
-        return health_client.healthCheck(HealthCheckRequest(service=service))
+        return health_client.healthCheck(HealthCheckRequest(service=service), metadata=self.metadata)
 
     def count(self, query: QueryRequest = {}) -> CountResponse:
         """Counts the number of records in Dozer cache.
 
         Args:
             query (dict, optional): Accepts a filter
             to query only a subset of records. 
@@ -65,16 +68,15 @@
             Defaults to {}.
 
         Returns:
             CountResponse: count of records
         """
 
         req = self.get_query_request(query)
-
-        return self.client.count(req)
+        return self.client.count(req, metadata=self.metadata)
 
     def query(self, query: dict = {}) -> QueryResponse:
         """Queries the Dozer cache for records. Response is in the common format.
 
         Args:
             query (dict, optional): Accepts a filter
             to query only a subset of records. 
@@ -89,26 +91,28 @@
         Returns:
             QueryResponse: {"fields": fields, "records": records}
                 fields: list of field definitions
                 records: list of records
         """
 
         req = self.get_query_request(query)
-        return self.client.query(req)
+
+        return self.client.query(req, metadata=self.metadata)
 
     def on_event(self, request={}):
         """Subscribes to events from Dozer.
 
         Args:
             request (OnEventRequest): Optionally accepts a filter
         """
         _req = OnEventRequest(endpoint=self.endpoint)
         for key, value in request.items():
             setattr(_req, key, value)
-        return self.client.OnEvent(_req)
+
+        return self.client.OnEvent(_req, metadata=self.metadata)
 
     def get_query_request(self, query: dict = {}) -> QueryRequest:
         """Returns a QueryRequest object
         Args:
             query (dict, optional): Accepts a filter
             to query only a subset of records. 
             Keys could be 
@@ -117,14 +121,15 @@
                 `$skip`: `int`,
                 '$after`: `int`, cursor to start from. `$skip` and `$after` cannot be used in the same query
                 `$order_by`: `dict` eg: `{"name": "asc"}` or `{"id": "desc"}`
             Defaults to {}.
         Returns:
             QueryRequest: QueryRequest object
         """
+
         if query is None or len(query) == 0:
             query = {}
 
         data = {}
         for key, value in query.items():
             data[key] = value
         query_str = json.dumps(data)
```

### Comparing `pydozer-0.1.16/pydozer/auth_pb2.py` & `pydozer-0.1.18/pydozer/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/auth_pb2_grpc.py` & `pydozer-0.1.18/pydozer/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/common_pb2.py` & `pydozer-0.1.18/pydozer/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/common_pb2_grpc.py` & `pydozer-0.1.18/pydozer/common_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/health_pb2.py` & `pydozer-0.1.18/pydozer/health_pb2.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/health_pb2_grpc.py` & `pydozer-0.1.18/pydozer/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/helper.py` & `pydozer-0.1.18/pydozer/helper.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/ingest.py` & `pydozer-0.1.18/pydozer/ingest.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/ingest_pb2.py` & `pydozer-0.1.18/pydozer/ingest_pb2.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/ingest_pb2_grpc.py` & `pydozer-0.1.18/pydozer/ingest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pydozer/types_pb2.py` & `pydozer-0.1.18/pydozer/types_pb2.py`

 * *Files identical despite different names*

### Comparing `pydozer-0.1.16/pyproject.toml` & `pydozer-0.1.18/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pydozer"
-version = "0.1.16"
+version = "0.1.18"
 description = "Python wrapper for the Dozer API"
 authors = ["Dozer Team <api@getdozer.io>"]
-license = "MIT"
+license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 grpcio = "^1.51.3"
 protobuf = "^4.22.0"
 pyarrow = "^11.0.0"
```

### Comparing `pydozer-0.1.16/PKG-INFO` & `pydozer-0.1.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pydozer
-Version: 0.1.16
+Version: 0.1.18
 Summary: Python wrapper for the Dozer API
-License: MIT
+License: Apache-2.0
 Author: Dozer Team
 Author-email: api@getdozer.io
 Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.51.3,<2.0.0)
 Requires-Dist: grpcio-reflection (>=1.51.3,<2.0.0)
 Requires-Dist: polars (>=0.16.10,<0.17.0)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pydozer Version: 0.1.16 Summary: Python wrapper for
-the Dozer API License: MIT Author: Dozer Team Author-email: api@getdozer.io
-Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: grpcio
-(>=1.51.3,<2.0.0) Requires-Dist: grpcio-reflection (>=1.51.3,<2.0.0) Requires-
-Dist: polars (>=0.16.10,<0.17.0) Requires-Dist: protobuf (>=4.22.0,<5.0.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: pydozer Version: 0.1.18 Summary: Python wrapper for
+the Dozer API License: Apache-2.0 Author: Dozer Team Author-email:
+api@getdozer.io Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: grpcio (>=1.51.3,<2.0.0) Requires-Dist: grpcio-reflection
+(>=1.51.3,<2.0.0) Requires-Dist: polars (>=0.16.10,<0.17.0) Requires-Dist:
+protobuf (>=4.22.0,<5.0.0) Requires-Dist: pyarrow (>=11.0.0,<12.0.0) Requires-
+Dist: tqdm (>=4.65.0,<5.0.0) Description-Content-Type: text/markdown
 
      [https://dozer-assets.s3.ap-southeast-1.amazonaws.com/logo-blue.svg]
 
    Connect any data source, combine them in real-time and instantly get low-
                           latency gRPC and REST APIs.
                â¡ All with just a simple configuration! â¡ï¸
```

