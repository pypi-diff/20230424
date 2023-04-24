# Comparing `tmp/graphql_service_framework-1.1.1.tar.gz` & `tmp/graphql_service_framework-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.1.1.tar", last modified: Mon Apr 24 09:04:20 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.2.tar", last modified: Mon Apr 24 14:58:52 2023, max compression
```

## Comparing `graphql_service_framework-1.1.1.tar` & `graphql_service_framework-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.072693 graphql_service_framework-1.1.1/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 09:04:20.073609 graphql_service_framework-1.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 09:04:19.000000 graphql_service_framework-1.1.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.069943 graphql_service_framework-1.1.1/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15905 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/query.graphql
--rw-rw-rw-   0 root         (0) root         (0)     8043 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7613 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     5105 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/service.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.071776 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 09:04:20.073609 graphql_service_framework-1.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.072693 graphql_service_framework-1.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6367 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/test_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 14:58:51.000000 graphql_service_framework-1.1.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.214325 graphql_service_framework-1.1.2/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15650 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/query.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.215325 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-24 14:58:52.000000 graphql_service_framework-1.1.2/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:58:52.217325 graphql_service_framework-1.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-24 14:58:43.000000 graphql_service_framework-1.1.2/tests/utils.py
```

### Comparing `graphql_service_framework-1.1.1/LICENSE` & `graphql_service_framework-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.1/PKG-INFO` & `graphql_service_framework-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.1.1
+Version: 1.1.2
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.1.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.2.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/conftest.py` & `graphql_service_framework-1.1.2/graphql_service_framework/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 def ctx():
     yield _ctx
 
 
 @pytest.fixture
 def services_ctx():
     class MockServicesManager:
-
         def __init__(self, services: Dict = None):
             self.services = services or {}
 
         def add_service(self, name: str, service):
             self.services[name] = service
 
         def __getattr__(self, service_name):
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/mesh.py` & `graphql_service_framework-1.1.2/graphql_service_framework/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,75 +34,73 @@
     ignore_service_manager_error: bool = True
     schema: Type = None
     state: ServiceConnectionState = ServiceConnectionState.UNKNOWN
 
     remote_name: Optional[str] = None
     remote_api_version: Optional[str] = None
     remote_service_version: Optional[str] = None
-    remote_service_manager: 'ServiceManager' = None
+    remote_service_manager: "ServiceManager" = None
     remote_service: GraphQLRemoteObject = None
 
     @classmethod
     def graphql_exclude_fields(cls) -> List[str]:
         return [
-            'schema',
-            'remote_service',
-            'remote_service_manager',
+            "schema",
+            "remote_service",
+            "remote_service_manager",
         ]
 
     def __post_init__(self):
         if self.schema:
             if hasattr(self.schema, "api_version"):
                 try:
                     schema_api_version = getattr(self.schema, "api_version")
-                    schema_api_version = packaging_version.Version(
-                        schema_api_version
-                    )
+                    schema_api_version = packaging_version.Version(schema_api_version)
                     if not self.api_version_specifier:
-                        self.api_version_specifier = \
-                            f"~={schema_api_version.major}" \
+                        self.api_version_specifier = (
+                            f"~={schema_api_version.major}"
                             f".{schema_api_version.minor}"
+                        )
                 except Exception:
                     logging.warning(
                         f"Could not identify the api_version for the "
                         f"connection to {self.name} at {self.service_url}"
                     )
 
         if self.service_url and self.schema:
             self.remote_service = GraphQLRemoteObject(
                 executor=GraphQLRemoteExecutor(
                     name=to_camel_case(self.name, title=True),
                     url=self.service_url,
-                    http_method=self.http_method
+                    http_method=self.http_method,
                 ),
-                api=GraphQLAPI(root=self.schema)
+                api=GraphQLAPI(root=self.schema),
             )
 
-    async def async_connect(
-            self,
-            logs: List = None,
-            timeout: int = 5
-    ) -> bool:
-
+    async def async_connect(self, logs: List = None, timeout: int = 5) -> bool:
         if logs is None:
             logs = []
 
         if not self.service_url:
             self.state = ServiceConnectionState.CONFIG_ERROR
-            logs.append(f"[{datetime.datetime.utcnow()}] ERROR: Missing URL"
-                        f" for service {self.name}")
+            logs.append(
+                f"[{datetime.datetime.utcnow()}] ERROR: Missing URL"
+                f" for service {self.name}"
+            )
 
             if self.raise_error:
                 raise TypeError(f"Missing URL for service {self.name}")
             return False
 
         if not self.schema:
             self.state = ServiceConnectionState.CONFIG_ERROR
-            logs.append(f"[{datetime.datetime.utcnow()}] ERROR: Missing schema"
-                        f" for service {self.name}")
+            logs.append(
+                f"[{datetime.datetime.utcnow()}] ERROR: Missing schema"
+                f" for service {self.name}"
+            )
 
             if self.raise_error:
                 raise TypeError(f"Missing schema for service {self.name}")
             return False
 
         name = to_camel_case(self.name, title=True) + "Service"
 
@@ -120,26 +118,26 @@
 
             # noinspection PyTypeChecker
             self.remote_service_manager: ServiceManager = GraphQLRemoteObject(
                 executor=GraphQLRemoteExecutor(
                     name=name,
                     url=self.service_manager_url,
                     http_method=self.http_method,
-                    http_timeout=timeout
+                    http_timeout=timeout,
                 ),
-                api=GraphQLAPI(root=ServiceManager)
+                api=GraphQLAPI(root=ServiceManager),
             )
 
             a = datetime.datetime.now()
             service_manager_error = False
             uptime = None
             try:
                 uptime = await self.remote_service_manager.call_async("uptime")
             except Exception as err:
-                msg = '' if self.ignore_service_manager_error else 'ERROR: '
+                msg = "" if self.ignore_service_manager_error else "ERROR: "
                 logs.append(
                     f"[{datetime.datetime.utcnow()}] {msg}unable to connect "
                     f"to {name} service manager, timed out after "
                     f"{timeout} seconds. {err}"
                 )
                 self.state = ServiceConnectionState.CONNECTION_ERROR
                 if self.ignore_service_manager_error:
@@ -152,30 +150,32 @@
                     )
                 else:
                     return False
 
             if not service_manager_error:
                 b = datetime.datetime.now()
 
-                self.remote_name = await self.remote_service_manager \
-                    .call_async("name")
-                self.remote_api_version = await \
-                    self.remote_service_manager.call_async("api_version")
-                self.remote_service_version = await \
-                    self.remote_service_manager.call_async("service_version")
+                self.remote_name = await self.remote_service_manager.call_async("name")
+                self.remote_api_version = await self.remote_service_manager.call_async(
+                    "api_version"
+                )
+                self.remote_service_version = (
+                    await self.remote_service_manager.call_async("service_version")
+                )
 
                 delta = b - a
-                logs.append(f"[{datetime.datetime.utcnow()}] {name} "
-                            f"Response time {delta} Uptime {uptime}")
+                logs.append(
+                    f"[{datetime.datetime.utcnow()}] {name} "
+                    f"Response time {delta} Uptime {uptime}"
+                )
 
                 if self.api_version_specifier:
                     try:
                         specifier = specifiers.SpecifierSet(
-                            self.api_version_specifier,
-                            prereleases=True
+                            self.api_version_specifier, prereleases=True
                         )
                     except specifiers.InvalidSpecifier as err:
                         logs.append(
                             f"[{datetime.datetime.utcnow()}] "
                             f"ERROR: {name} malformed api version specifier "
                             f"{self.api_version_specifier}"
                         )
@@ -195,18 +195,15 @@
                             f"{self.remote_api_version}"
                         )
                         self.state = ServiceConnectionState.VALIDATION_ERROR
                         if self.raise_error:
                             raise err
                         return False
 
-                    if not specifier.contains(
-                            service_version,
-                            prereleases=True
-                    ):
+                    if not specifier.contains(service_version, prereleases=True):
                         logs.append(
                             f"[{datetime.datetime.utcnow()}] ERROR: "
                             f"api_version mismatch, found "
                             f"{self.remote_api_version}, required "
                             f"{self.api_version_specifier}"
                         )
                         self.state = ServiceConnectionState.VALIDATION_ERROR
@@ -228,15 +225,15 @@
                             f" for {self.api_version_specifier}"
                         )
 
         executor = GraphQLRemoteExecutor(
             name=name,
             url=self.service_url,
             http_method=self.http_method,
-            http_timeout=timeout
+            http_timeout=timeout,
         )
 
         try:
             response = await executor.execute_async("query { __typename }")
         except Exception as err:
             logs.append(
                 f"[{datetime.datetime.utcnow()}] ERROR: {name} API error "
@@ -273,22 +270,22 @@
 class ServiceManager:
     """
     A manager for a service that advertises the status of the service and
     creates and maintains connections to other services.
     """
 
     def __init__(
-            self,
-            name: str,
-            schema: Any = None,
-            api_version: str = None,
-            service_version: str = None,
-            connections: List[ServiceConnection] = None,
-            connect_on_init: bool = True,
-            connect_timeout: int = 5
+        self,
+        name: str,
+        schema: Any = None,
+        api_version: str = None,
+        service_version: str = None,
+        connections: List[ServiceConnection] = None,
+        connect_on_init: bool = True,
+        connect_timeout: int = 5,
     ):
         if not connections:
             connections = []
 
         self._connections = connections
         self.connect_on_init = connect_on_init
         self.connect_timeout = connect_timeout
@@ -321,25 +318,24 @@
         self._name = name
         self._api_version = api_version
         self._service_version = service_version
         self._started_at = datetime.datetime.now()
         self._has_checked_connections = False
         self._logs = []
 
-        fp = os.path.dirname(
-            os.path.realpath(__file__)) + '/query.graphql'
-        with open(fp, 'r') as default_query:
+        fp = os.path.dirname(os.path.realpath(__file__)) + "/query.graphql"
+        with open(fp, "r") as default_query:
             default_query = default_query.read()
 
         self.manager_http_server = GraphQLHTTPServer.from_api(
             api=GraphQLAPI(root=ServiceManager),
             serve_graphiql=True,
             allow_cors=True,
             root_value=self,
-            graphiql_default_query=default_query
+            graphiql_default_query=default_query,
         )
 
         if self.connect_on_init:
             self.connect()
 
     def connect(self, timeout: int = None):
         if timeout is None:
@@ -348,18 +344,15 @@
         if not self._has_checked_connections and self._connections:
             self._has_checked_connections = True
 
             async def _check_connections(_timeout: int):
                 dependencies = []
                 for service in self._connections:
                     dependencies.append(
-                        service.async_connect(
-                            logs=self._logs,
-                            timeout=_timeout
-                        )
+                        service.async_connect(logs=self._logs, timeout=_timeout)
                     )
                 await asyncio.gather(*dependencies)
 
             try:
                 loop = asyncio.get_running_loop()
             except RuntimeError:
                 loop = None
@@ -369,16 +362,15 @@
             else:
                 asyncio.run(_check_connections(_timeout=timeout))
 
     def __getattr__(self, service_name):
         if self._connections:
             for service in self._connections:
                 if service.name == service_name:
-                    if service.state == \
-                            ServiceConnectionState.CONNECTION_ERROR:
+                    if service.state == ServiceConnectionState.CONNECTION_ERROR:
                         try:
                             loop = asyncio.get_running_loop()
                         except RuntimeError:
                             loop = None
 
                         if loop and loop.is_running():
                             loop.create_task(service.async_connect())
@@ -402,15 +394,15 @@
 
     @field
     def service_version(self) -> str:
         return self._service_version
 
     @field
     def started_at(self) -> str:
-        return self._started_at.strftime('%Y-%m-%d %H:%M:%S')
+        return self._started_at.strftime("%Y-%m-%d %H:%M:%S")
 
     @field
     def uptime(self) -> str:
         uptime = datetime.datetime.now() - self._started_at
         return str(uptime)
 
     @field
@@ -424,15 +416,17 @@
     @field
     def packages(self) -> List[str]:
         """
         All the Packages this service is dependent on.
         :return:
         """
         import pkg_resources
+
         installed_packages = pkg_resources.working_set
-        installed_packages_list = sorted(["%s==%s" % (i.key, i.version)
-                                          for i in installed_packages])
+        installed_packages_list = sorted(
+            ["%s==%s" % (i.key, i.version) for i in installed_packages]
+        )
         return installed_packages_list
 
     @field
     def logs(self) -> List[str]:
         return self._logs
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/middleware.py` & `graphql_service_framework-1.1.2/graphql_service_framework/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,29 @@
 from werkzeug import Request
 
 from graphql_service_framework.mesh import ServiceManager
 from graphql_service_framework.service import WSGIFramework
 
 
 class ServiceMeshMiddleware:
-
     def __init__(
-            self,
-            wsgi_app: WSGIFramework,
-            service_manager: 'ServiceManager',
-            service_manager_path: str = None,
-            check_connections_on_first_request: bool = True,
-            context_key: str = "services"
+        self,
+        wsgi_app: WSGIFramework,
+        service_manager: "ServiceManager",
+        service_manager_path: str = None,
+        check_connections_on_first_request: bool = True,
+        context_key: str = "services",
     ):
         self.wsgi_app = wsgi_app
         self.service_manager = service_manager
         self.service_manager_path = service_manager_path
         self.connect_on_first_request = check_connections_on_first_request
         self.context_key = context_key
 
-    def __call__(
-            self,
-            environ: Dict,
-            start_response: Callable
-    ) -> Iterable[bytes]:
+    def __call__(self, environ: Dict, start_response: Callable) -> Iterable[bytes]:
         if self.connect_on_first_request:
             self.service_manager.connect()
 
         request = Request(environ)
 
         if request.path == f"{self.service_manager_path}":
             # Expose the service manager HTTP server
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.2/graphql_service_framework/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from schemadiff import diff, format_diff
 from schemadiff.changes import CriticalityLevel
 
 from graphql_api.api import GraphQLRootTypeDelegate
 from graphql_api import GraphQLAPI
 from graphql_api.remote import GraphQLRemoteExecutor, GraphQLRemoteObject
 
-TClient = TypeVar("TClient", bound='Schema')
+TClient = TypeVar("TClient", bound="Schema")
 
 """
 Schema Provides Utilities to help with a Service
 
 Schema Class Attributes:
     api_version         The version of this schema, this must be defined
                         in the root controller.
@@ -32,28 +32,27 @@
                         If `validate_schema` is True and `criticality` is
                         set to `None` an exception will not be raised but
                         the changes will still be logged.
 """
 
 
 class APIVersion(type):
-
     @classmethod
     def __prepare__(mcs, name, bases, **kwargs):
         return super().__prepare__(name, bases, **kwargs)
 
     def __new__(mcs, name, bases, namespace, **kwargs):
         return super().__new__(mcs, name, bases, namespace)
 
     def __init__(cls, name, bases, namespace, api_version=None, **kwargs):
         if api_version:
             cls.api_version = api_version
         else:
             for base in bases:
-                if hasattr(base, 'api_version') and base.api_version:
+                if hasattr(base, "api_version") and base.api_version:
                     cls.api_version = base.api_version
 
         if not cls.api_version:
             cls.api_version = "0.0.1.dev"
         super().__init__(name, bases, namespace)
 
 
@@ -102,15 +101,15 @@
                 return schema
 
             if schema_class:
                 validate(
                     schema,
                     schema_class,
                     cls.criticality,
-                    cls.ignore_description_changes
+                    cls.ignore_description_changes,
                 )
 
         return schema
 
     @classmethod
     def client(cls: TClient, url: str = None) -> TClient:
         if not url:
@@ -121,85 +120,77 @@
                 raise ValueError(
                     f"A URL for client {cls.__name__} could not be found. "
                     f"Please set the `{env_var}` environment variable or "
                     f"specify a URL when creating the {cls.__name__} client"
                 )
         # noinspection PyTypeChecker
         return GraphQLRemoteObject(
-            executor=GraphQLRemoteExecutor(url),
-            api=GraphQLAPI(root=cls)
+            executor=GraphQLRemoteExecutor(url), api=GraphQLAPI(root=cls)
         )
 
     @classmethod
     def graphql_schema(cls) -> GraphQLSchema:
         return GraphQLAPI(root=cls).graphql_schema()[0]
 
     def create_service(self, config: Dict = None):
         from graphql_service_framework import Service
 
         return Service(root=self, config={**self.config, **(config or {})})
 
 
 def validate(
-        graphql_schema: GraphQLSchema,
-        service_schema: Type[Schema],
-        criticality: CriticalityLevel,
-        ignore_description_changes: bool = True
+    graphql_schema: GraphQLSchema,
+    service_schema: Type[Schema],
+    criticality: CriticalityLevel,
+    ignore_description_changes: bool = True,
 ):
-    generated_service_schema = \
-        GraphQLAPI(root=service_schema).graphql_schema()[0]
+    generated_service_schema = GraphQLAPI(root=service_schema).graphql_schema()[0]
 
     if not generated_service_schema:
-        raise ValueError(
-            f"Could not generate service schema for {service_schema}"
-        )
+        raise ValueError(f"Could not generate service schema for {service_schema}")
     query_a = generated_service_schema.query_type
     query_b = graphql_schema.query_type
 
     if query_a and query_b and query_a.name != query_b.name:
         query_a.name = query_b.name
 
     mutation_a = generated_service_schema.query_type
     mutation_b = graphql_schema.query_type
 
     if mutation_a and mutation_b and mutation_a.name != mutation_b.name:
         mutation_a.name = mutation_b.name
 
-    generated_service_schema_language = print_schema(
-        generated_service_schema
-    )
+    generated_service_schema_language = print_schema(generated_service_schema)
 
     schema_language = print_schema(graphql_schema)
 
     # There should be no changes for a perfect implementation
     changes = diff(generated_service_schema_language, schema_language)
 
     # Ignore description changes as often they are uncontrollable
     if ignore_description_changes:
         changes = [
-            change for change in changes
+            change
+            for change in changes
             if "DescriptionChanged" not in type(change).__name__
         ]
 
     if changes:
-
         raise_error_map = {
             None: [],
             CriticalityLevel.NonBreaking: [
                 CriticalityLevel.NonBreaking,
                 CriticalityLevel.Dangerous,
-                CriticalityLevel.Breaking
+                CriticalityLevel.Breaking,
             ],
             CriticalityLevel.Dangerous: [
                 CriticalityLevel.Dangerous,
-                CriticalityLevel.Breaking
+                CriticalityLevel.Breaking,
             ],
-            CriticalityLevel.Breaking: [
-                CriticalityLevel.Breaking
-            ]
+            CriticalityLevel.Breaking: [CriticalityLevel.Breaking],
         }
 
         raise_err = any(
             change.criticality.level in raise_error_map[criticality]
             for change in changes
         )
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.2/graphql_service_framework/schema_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,65 +10,63 @@
 from graphql import print_schema
 
 from schemadiff import diff
 from schemadiff.changes.field import FieldDescriptionChanged
 from schemadiff.formatting import format_change_by_criticality
 
 from graphql_service_framework.schema import Schema
-from graphql_service_framework.utils import \
-    increment_version, \
-    install_package, \
-    find_modules, \
-    find_schema, \
-    get_py_code_changes, \
-    set_api_version
+from graphql_service_framework.utils import (
+    increment_version,
+    install_package,
+    find_modules,
+    find_schema,
+    get_py_code_changes,
+    set_api_version,
+)
 
 
 @dataclass
 class SchemaTracker:
     name: str
     path: str
     schema: Type[Schema]
 
     @classmethod
-    def find_schemas(
-            cls,
-            path,
-            package_name,
-            index_url
-    ) -> List['SchemaTracker']:
-
+    def find_schemas(cls, path, package_name, index_url) -> List["SchemaTracker"]:
         schema_trackers = []
         for folder in os.listdir(path):
             full_path = os.path.join(path, folder)
-            if os.path.isdir(full_path) and not folder.startswith(".") and \
-                    folder not in ["tests"]:
+            if (
+                os.path.isdir(full_path)
+                and not folder.startswith(".")
+                and folder not in ["tests"]
+            ):
                 schema_name = folder
 
                 if modules := find_modules(full_path, schema_name):
                     if schema := find_schema(modules):
                         schema_trackers.append(
                             SchemaTracker(
                                 name=schema_name,
                                 path=full_path,
                                 schema=schema,
                                 package_name=package_name,
-                                index_url=index_url
+                                index_url=index_url,
                             )
                         )
 
         return schema_trackers
 
     def __init__(
-            self,
-            schema: Type[Schema],
-            name: str,
-            path: str,
-            package_name: str,
-            index_url: str
+        self,
+        schema: Type[Schema],
+        name: str,
+        path: str,
+        package_name: str,
+        index_url: str,
     ):
         self.schema = schema
         self.name = name
         self.path = path
         self.package_name = package_name
         self.index_url = index_url
 
@@ -77,106 +75,101 @@
 
     @functools.cache
     def previous_schema(self) -> Optional[Type[Schema]]:
         print(f"Checking for a previous version of {self.name}")
         _prev_report = install_package(self.name, index_url=self.index_url)
 
         if _prev_report:
-            v = _prev_report['install'][0]['metadata']['version']
+            v = _prev_report["install"][0]["metadata"]["version"]
 
-            install_location = _prev_report.get("pip_show").get('Location')
+            install_location = _prev_report.get("pip_show").get("Location")
             print(
-                f"Installed package "
-                f"{self.name} version {v} at {install_location}"
+                f"Installed package " f"{self.name} version {v} at {install_location}"
             )
 
             prev_modules = find_modules(
                 os.path.join(install_location, self.package_name, self.name),
-                f"{self.package_name}.{self.name}"
+                f"{self.package_name}.{self.name}",
             )
 
             return find_schema(prev_modules)
 
     @functools.cache
     def code_changes(self):
         if self.previous_schema():
             a_path = self.path
             b_path = os.path.dirname(
-                importlib.import_module(
-                    f"{self.package_name}.{self.name}"
-                ).__file__
+                importlib.import_module(f"{self.package_name}.{self.name}").__file__
             )
 
             print(
                 f"Comparing code for {self.name} with version "
                 f"{self.previous_schema().api_version}\n"
                 f"a_path={a_path}\nb_path={b_path}"
             )
             return get_py_code_changes(
-                a_path,
-                b_path,
-                self.previous_schema().api_version
+                a_path, b_path, self.previous_schema().api_version
             )
         return None
 
     def changes(self):
         if not self.previous_schema():
             return []
         else:
             new_schema_language = print_schema(self.schema.graphql_schema())
             previous_schema_language = print_schema(
                 self.previous_schema().graphql_schema()
             ).replace(f"{self.package_name}.", "")
 
-            return diff(
-                previous_schema_language,
-                new_schema_language
-            )
+            return diff(previous_schema_language, new_schema_language)
 
     def change_log(self):
-        prev_version = self.previous_schema().api_version \
-            if self.previous_schema() else None
+        prev_version = (
+            self.previous_schema().api_version if self.previous_schema() else None
+        )
 
-        version = f"**{self.version()}** (updated from *{prev_version}*)" \
-            if prev_version and prev_version != self.version() else \
-            f"*{self.version()}*"
+        version = (
+            f"**{self.version()}** (updated from *{prev_version}*)"
+            if prev_version and prev_version != self.version()
+            else f"*{self.version()}*"
+        )
 
         log = f"- {self.name} {version}\n"
         if not self.previous_schema():
             log += "  - *New Schema*\n"
         elif not self.changes() and self.code_changes():
             log += "  - *Code changes only* (No Schema changes)\n"
-        elif self.major_changes_count() or \
-                self.minor_changes_count() or \
-                self.micro_changes_count():
-            log += f"  - " \
-                   f"{self.major_changes_count()} breaking, " \
-                   f"{self.minor_changes_count()} safe, " \
-                   f"{self.micro_changes_count()} micro Schema changes \n"
+        elif (
+            self.major_changes_count()
+            or self.minor_changes_count()
+            or self.micro_changes_count()
+        ):
+            log += (
+                f"  - "
+                f"{self.major_changes_count()} breaking, "
+                f"{self.minor_changes_count()} safe, "
+                f"{self.micro_changes_count()} micro Schema changes \n"
+            )
             for change in self.changes():
                 log += f"    - {format_change_by_criticality(change)}\n"
 
         return log
 
     def major_changes_count(self):
-        return sum(
-            change.breaking or change.dangerous
-            for change in self.changes()
-        )
+        return sum(change.breaking or change.dangerous for change in self.changes())
 
     def minor_changes_count(self):
         return sum(
             change.safe and not isinstance(change, FieldDescriptionChanged)
             for change in self.changes()
         )
 
     def micro_changes_count(self):
         count = sum(
-            isinstance(change, FieldDescriptionChanged)
-            for change in self.changes()
+            isinstance(change, FieldDescriptionChanged) for change in self.changes()
         )
         if not count and (self.code_changes() or not self.previous_schema()):
             count = 1
 
         return count
 
     def version(self):
@@ -206,30 +199,34 @@
         if not release_reason:
             return
 
         print(f"Releasing {self.name} because {release_reason}")
         print(f"Schema: {print_schema(self.schema.graphql_schema())}")
         print(f"Creating setup.py in {self.path} for {self.name}")
 
-        setup_data = inspect.cleandoc("""
+        setup_data = (
+            inspect.cleandoc(
+                """
             from setuptools import setup
 
             setup(
                 name='SERVICE_NAME',
                 version='SERVICE_VERSION',
                 packages=['SERVICE_PACKAGE'],
                 install_requires=[
                     'packaging',
                     'graphql-service-framework'
                 ]
             )
-            """) \
-            .replace('SERVICE_NAME', self.name.replace("_", "-")) \
-            .replace('SERVICE_VERSION', self.version()) \
-            .replace('SERVICE_PACKAGE', f"{self.package_name}.{self.name}")
+            """
+            )
+            .replace("SERVICE_NAME", self.name.replace("_", "-"))
+            .replace("SERVICE_VERSION", self.version())
+            .replace("SERVICE_PACKAGE", f"{self.package_name}.{self.name}")
+        )
 
-        with open(os.path.join(self.path, "setup.py"), 'w') as file:
+        with open(os.path.join(self.path, "setup.py"), "w") as file:
             file.write(setup_data)
 
         print(f"Inserting api_version = {self.version()} into {self.name}")
         for file in Path(self.path).rglob("*.py"):
             file.write_text(set_api_version(file.read_text(), self.version()))
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/service.py` & `graphql_service_framework-1.1.2/graphql_service_framework/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,137 +12,130 @@
 from hypercorn import Config
 from hypercorn.asyncio import serve
 from hypercorn.typing import ASGIFramework, WSGIFramework
 from hypercorn.middleware import AsyncioWSGIMiddleware
 
 
 class Service:
-
     def __init__(self, root, config: Dict = None):
-        from graphql_service_framework import ServiceConnection, \
-            ServiceManager
+        from graphql_service_framework import ServiceConnection, ServiceManager
 
         if not config:
             config = {}
 
         self.config = config
 
         graphiql_default = self.config.get("graphiql_default", "")
         relative_path = self.config.get("http_relative_path", "")
 
         if not self.config.get("service_type"):
             self.config["service_type"] = "asgi"
 
         if not self.config.get("service_name"):
-            self.config["service_name"] = to_snake_case(
-                root.__class__.__name__
-            )
+            self.config["service_name"] = to_snake_case(root.__class__.__name__)
 
         if not self.config.get("api_version"):
             self.config["api_version"] = root.__class__.api_version
 
         if not self.config.get("http_health_path"):
             self.config["http_health_path"] = f"{relative_path}/health"
 
         health_path = self.config.get("http_health_path")
 
         if not graphiql_default:
             # noinspection PyBroadException
             try:
                 dirname = os.path.dirname(inspect.getfile(root.__class__))
                 graphiql_default = open(
-                    os.path.join(dirname, '../graphiql_default.graphql'),
-                    mode='r'
+                    os.path.join(dirname, "../graphiql_default.graphql"), mode="r"
                 ).read()
             except Exception:
                 # noinspection PyBroadException
                 try:
                     dirname = os.path.dirname(inspect.getfile(root.__class__))
                     graphiql_default = open(
-                        os.path.join(dirname, '../.graphql'),
-                        mode='r'
+                        os.path.join(dirname, "../.graphql"), mode="r"
                     ).read()
                 except Exception:
-                    pass
+                    try:
+                        dirname = os.path.dirname(inspect.getfile(root.__class__))
+                        graphiql_default = open(
+                            os.path.join(dirname, "./.graphql"), mode="r"
+                        ).read()
+                    except Exception:
+                        pass
 
         self.graphql_api = GraphQLAPI(root=root.__class__)
         self.graphql_http_server = GraphQLHTTPServer.from_api(
             api=self.graphql_api,
             root_value=root,
             graphiql_default_query=graphiql_default,
-            health_path=health_path
+            health_path=health_path,
         )
 
-        self.service_manager_path = self.config.get(
-            'service_manager_path', "/service"
-        )
+        self.service_manager_path = self.config.get("service_manager_path", "/service")
 
         connections = []
 
-        for key, service in self.config.get('services', {}).items():
+        for key, service in self.config.get("services", {}).items():
             from graphql_service_framework.schema import Schema
+
             valid_service = False
 
             if inspect.isclass(service) and issubclass(service, Schema):
                 service = service.client()
 
             if isinstance(service, GraphQLRemoteObject):
                 if issubclass(service.python_type, Schema):
-                    version = service.python_type.api_version.split('.')
+                    version = service.python_type.api_version.split(".")
 
                     if isinstance(service.executor, GraphQLRemoteExecutor):
                         if version[-1].lower() == "dev":
                             version_specifier = f">={'.'.join(version)}"
                         else:
                             version_specifier = f"~={version[0]}.{version[1]}"
 
                         url = service.executor.url + self.service_manager_path
                         connection = ServiceConnection(
                             name=key,
                             schema=service.python_type,
                             api_version_specifier=version_specifier,
                             service_url=service.executor.url,
-                            service_manager_url=url
+                            service_manager_url=url,
                         )
 
                         connections.append(connection)
                         valid_service = True
 
             if not valid_service:
                 raise TypeError(f"Invalid service {key} {service}.")
 
         self.service_manager = ServiceManager(
             name=config.get("service_name"),
             api_version=config.get("api_version"),
-            connections=connections
+            connections=connections,
         )
 
     def create_wsgi_app(self) -> WSGIFramework:
         from graphql_service_framework import ServiceMeshMiddleware
 
         wsgi_app = self.graphql_http_server.app(main=self.config.get("main"))
         return ServiceMeshMiddleware(
             wsgi_app=wsgi_app,
             service_manager=self.service_manager,
-            service_manager_path=self.service_manager_path
+            service_manager_path=self.service_manager_path,
         )
 
     def create_asgi_app(self) -> ASGIFramework:
         return AsyncioWSGIMiddleware(
-            wsgi_app=self.create_wsgi_app(),
-            max_body_size=2 ** 32
+            wsgi_app=self.create_wsgi_app(), max_body_size=2**32
         )
 
     def run(self, config: Dict = None):
-        asyncio_config = Config.from_mapping({
-            **(self.config or {}),
-            **(config or {})
-        })
-
-        return asyncio.run(serve(
-            self.create_asgi_app(), asyncio_config
-        ))
+        asyncio_config = Config.from_mapping({**(self.config or {}), **(config or {})})
+
+        return asyncio.run(serve(self.create_asgi_app(), asyncio_config))
 
     def client(self):
         from werkzeug.test import Client
 
         return Client(self.create_wsgi_app())
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.2/graphql_service_framework/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def set_api_version(code, new_version):
     from graphql_service_framework.schema import Schema
 
     schema_class_name = Schema.__name__
     if f"{schema_class_name}, api_version=" not in code.lower():
         old = f"{schema_class_name}):\n"
-        new = f'{schema_class_name}, api_version=\"{new_version}\"):\n'
+        new = f'{schema_class_name}, api_version="{new_version}"):\n'
         code = code.replace(old, new)
     return code
 
 
 def get_py_code_changes(a, b, _version):
     import glob
 
@@ -42,42 +42,40 @@
             a_data[_path.replace(a, "")] = set_api_version(f.read(), _version)
 
     for _path in glob.glob(os.path.join(b, "*.py")):
         with open(_path) as f:
             b_data[_path.replace(b, "")] = f.read()
 
     if a_data != b_data:
-        return '\n' + '\n'.join(
+        return "\n" + "\n".join(
             difflib.ndiff(
-                pprint.pformat(b_data).splitlines(),
-                pprint.pformat(a_data).splitlines()
+                pprint.pformat(b_data).splitlines(), pprint.pformat(a_data).splitlines()
             )
         )
 
     return None
 
 
 def increment_version(version, i=2, amount=1, reset=True):
-    version = version.split('.')
+    version = version.split(".")
     version[i] = str(int(version[i]) + amount)
     while reset and i != len(version) - 1:
         i += 1
         version[i] = "0"
-    return '.'.join(version)
+    return ".".join(version)
 
 
 def find_schema(modules):
     schemas = set()
 
     for module in modules:
         for name, obj in module.__dict__.items():
             from graphql_service_framework import Schema
-            if inspect.isclass(obj) \
-                    and issubclass(obj, Schema) \
-                    and obj != Schema:
+
+            if inspect.isclass(obj) and issubclass(obj, Schema) and obj != Schema:
                 schemas.add(obj)
 
     if len(schemas) > 1:
         raise TypeError(
             f"The {modules} folder defined multiple schemas '{schemas}'."
             f"Each schema should only have a single schema subclass."
         )
@@ -89,35 +87,43 @@
             f" Each schema should have a single schema subclass."
         )
 
 
 def install_package(package, index_url) -> Optional[dict]:
     # noinspection PyBroadException
     try:
-        print(
-            f"Installing package {package}"
-        )
+        print(f"Installing package {package}")
         report_path = f"{package}-report.json"
-        subprocess.check_call([
-            sys.executable, "-m", "pip", "install", package,
-            f"--index-url={index_url}", "--no-deps", "--ignore-installed",
-            f"--report={report_path}",
-            "--quiet", "--quiet", "--quiet"
-        ])
+        subprocess.check_call(
+            [
+                sys.executable,
+                "-m",
+                "pip",
+                "install",
+                package,
+                f"--index-url={index_url}",
+                "--no-deps",
+                "--ignore-installed",
+                f"--report={report_path}",
+                "--quiet",
+                "--quiet",
+                "--quiet",
+            ]
+        )
 
         _report = json.loads(open(report_path).read())
 
         # Edge case where we are being redirected by gitlab
-        if "pythonhosted.org" in _report['install'][0]['download_info']['url']:
+        if "pythonhosted.org" in _report["install"][0]["download_info"]["url"]:
             print(f"Ignoring gitlab redirect for package {package}")
             return None
 
-        pip_show_response = subprocess.check_output([
-            sys.executable, "-m", "pip", "show", package
-        ]).decode(sys.stdout.encoding)
+        pip_show_response = subprocess.check_output(
+            [sys.executable, "-m", "pip", "show", package]
+        ).decode(sys.stdout.encoding)
 
         pip_show = {}
 
         for line in pip_show_response.splitlines():
             split_line = line.split(": ", 1)
             if len(split_line) == 2:
                 pip_show[split_line[0]] = split_line[1]
@@ -127,44 +133,39 @@
         return _report
     except Exception:
         return None
 
 
 def find_modules(modules_path, package_name):
     print(
-        f"Searching for modules in {modules_path} with package name "
-        f"{package_name}"
+        f"Searching for modules in {modules_path} with package name " f"{package_name}"
     )
     _modules = []
     for root, dirs, files in os.walk(modules_path):
-        relative_path = root.replace(
-            modules_path + "/", ""
-        ).replace(
-            modules_path, ""
-        )
+        relative_path = root.replace(modules_path + "/", "").replace(modules_path, "")
 
         print(f" - Searching path {root}.")
 
         for _file in files:
             _file_name = os.path.join(relative_path, _file)
             print(f" - Found file {_file_name}")
-            if _file.endswith(".py") \
-                    and not _file.endswith("setup.py") \
-                    and not _file.endswith("__init__.py") \
-                    and not _file.endswith(".pyc") \
-                    and "__pycache__" not in _file:
+            if (
+                _file.endswith(".py")
+                and not _file.endswith("setup.py")
+                and not _file.endswith("__init__.py")
+                and not _file.endswith(".pyc")
+                and "__pycache__" not in _file
+            ):
                 print(f"    - Checking file {_file_name}")
-                module_name = _file_name.replace("/", ".").rsplit('.', 1)[0]
+                module_name = _file_name.replace("/", ".").rsplit(".", 1)[0]
                 print(f"    - Found module {module_name} in {_file_name}")
                 try:
-                    _modules.append(importlib.import_module(
-                        f"{package_name}.{module_name}"
-                    ))
-                    print(
-                        f"    - Imported module {module_name} in {_file_name}"
+                    _modules.append(
+                        importlib.import_module(f"{package_name}.{module_name}")
                     )
+                    print(f"    - Imported module {module_name} in {_file_name}")
                 except Exception as err:
                     print(
                         f"    - Unable to import module {module_name} in "
                         f"{_file_name}, {err}"
                     )
     return _modules
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.2/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.1.1
+Version: 1.1.2
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.1.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.2.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.1/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.2/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.1/setup.py` & `graphql_service_framework-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import io
 
 from setuptools import setup, find_packages
 
-with io.open('README.md', 'rt', encoding='utf8') as f:
+with io.open("README.md", "rt", encoding="utf8") as f:
     readme = f.read()
 
-with io.open('VERSION') as version_file:
+with io.open("VERSION") as version_file:
     version = version_file.read().strip().lower()
     if version.startswith("v"):
         version = version[1:]
 
 setup(
-    name='graphql_service_framework',
+    name="graphql_service_framework",
     version=version,
-    license='MIT',
+    license="MIT",
     packages=find_packages(),
     include_package_data=True,
-    author='Robert Parker',
-    author_email='rob@parob.com',
-    url='https://gitlab.com/parob/graphql-service-framework',
-    download_url=f'https://gitlab.com/parob/graphql-service-framework/-/'
-                 f'archive/master/graphql-service-framework-v{version}.zip',
-    keywords=['GraphQL'],
-    description='GraphQL Service Framework.',
+    author="Robert Parker",
+    author_email="rob@parob.com",
+    url="https://gitlab.com/parob/graphql-service-framework",
+    download_url=f"https://gitlab.com/parob/graphql-service-framework/-/"
+    f"archive/master/graphql-service-framework-v{version}.zip",
+    keywords=["GraphQL"],
+    description="GraphQL Service Framework.",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     install_requires=[
         "graphql-core>=3.2.0",
         "graphql-api>=1.3.0",
         "werkzeug>=2.2.2",
         "context-helper>=1.0.2",
         "packaging>=21.3",
         "graphql-schema-diff>=1.2.4",
         "graphql-http-server>=1.4.4",
         "hypercorn>=0.14.3",
         "pytest",
         "pytest-cov",
         "coverage",
-        "flake8"
+        "flake8",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent"
-    ]
+        "Operating System :: OS Independent",
+    ],
 )
```

### Comparing `graphql_service_framework-1.1.1/tests/test_schema.py` & `graphql_service_framework-1.1.2/tests/test_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,43 +12,37 @@
 
 from graphql_service_framework.schema import Schema
 from tests.utils import available
 
 
 # noinspection DuplicatedCode
 class TestSchema:
-
     def test_schema_validation(self):
         from graphql_api import GraphQLAPI
 
         class UTCTime(Schema):
-
             @field
             def now(self) -> Optional[str]:
                 raise NotImplementedError()
 
         class UTCTimeService(UTCTime):
-
             @field
             def now(self) -> Optional[str]:
                 return str(datetime.datetime.now())
 
-        server = GraphQLHTTPServer.from_api(
-            api=GraphQLAPI(root=UTCTimeService)
-        )
+        server = GraphQLHTTPServer.from_api(api=GraphQLAPI(root=UTCTimeService))
 
         client = Client(server.app())
 
-        response = client.get('/?query={now}')
+        response = client.get("/?query={now}")
 
         assert response.status_code == 200
         assert "now" in response.text
 
         class InvalidUTCTimeService(UTCTime):
-
             @field
             def now(self) -> str:
                 return str(datetime.datetime.now())
 
         with pytest.raises(TypeError, match="Validation Error"):
             GraphQLAPI(root=InvalidUTCTimeService).graphql_schema()
 
@@ -63,37 +57,32 @@
 
         assert GraphQLAPI(root=InvalidUTCTimeService).graphql_schema()
 
     def test_schema_validation_no_field(self):
         from graphql_api import GraphQLAPI
 
         class UTCTime(Schema):
-
             @field
             def now(self) -> Optional[str]:
                 raise NotImplementedError()
 
         class UTCTimeService(UTCTime):
-
             def now(self) -> Optional[str]:
                 return str(datetime.datetime.now())
 
-        server = GraphQLHTTPServer.from_api(
-            api=GraphQLAPI(root=UTCTimeService)
-        )
+        server = GraphQLHTTPServer.from_api(api=GraphQLAPI(root=UTCTimeService))
 
         client = Client(server.app())
 
-        response = client.get('/?query={now}')
+        response = client.get("/?query={now}")
 
         assert response.status_code == 200
         assert "now" in response.text
 
         class InvalidUTCTimeService(UTCTime):
-
             def now(self) -> str:
                 return str(datetime.datetime.now())
 
         with pytest.raises(TypeError, match="Validation Error"):
             GraphQLAPI(root=InvalidUTCTimeService).graphql_schema()
 
         InvalidUTCTimeService.validate_schema = False
@@ -105,21 +94,19 @@
 
         InvalidUTCTimeService.criticality = CriticalityLevel.Breaking
 
         assert GraphQLAPI(root=InvalidUTCTimeService).graphql_schema()
 
     def test_schema_client(self):
         class UTCTime(Schema):
-
             @field
             def now(self) -> Optional[str]:
                 raise NotImplementedError()
 
         class UTCTimeService(UTCTime):
-
             @field
             def now(self) -> Optional[str]:
                 return str(datetime.datetime.now())
 
         with pytest.raises(ValueError):
             client = UTCTime()
             assert client
@@ -128,94 +115,87 @@
         assert client
 
         local_client = UTCTimeService()
         assert local_client.now()
 
     def test_create_service(self):
         class UTCTime(Schema):
-
             @field
             def now(self) -> Optional[str]:
                 raise NotImplementedError()
 
         class UTCTimeService(UTCTime):
-
             @field
             def now(self) -> Optional[str]:
                 return str(datetime.datetime.now())
 
         service = UTCTimeService(config={"test": "test"}).create_service()
 
         assert service
 
     def test_create_service_init(self):
         class UTCTime(Schema):
-
             @field
             def now(self) -> Optional[str]:
                 raise NotImplementedError()
 
         class UTCTimeService(UTCTime):
-
             def __init__(self, offset: int, config: Dict = None):
                 super().__init__(config=config)
                 self.offset = offset
 
             @field
             def now(self) -> Optional[str]:
                 return str(
-                    datetime.datetime.now() +
-                    datetime.timedelta(seconds=self.offset)
+                    datetime.datetime.now() + datetime.timedelta(seconds=self.offset)
                 )
 
-        service = UTCTimeService(
-            offset=1, config={"test": "test"}
-        ).create_service()
+        service = UTCTimeService(offset=1, config={"test": "test"}).create_service()
 
         client = service.client()
 
-        response = client.get('?query={now}')
+        response = client.get("?query={now}")
 
         assert response.status_code == 200 and "now" in response.text
 
-    utc_time_api_url = "https://europe-west2-parob-297412.cloudfunctions." \
-                       "net/utc_time"
+    utc_time_api_url = (
+        "https://europe-west2-parob-297412.cloudfunctions." "net/utc_time"
+    )
 
     # noinspection DuplicatedCode,PyUnusedLocal
     @pytest.mark.skipif(
         not available(utc_time_api_url),
-        reason=f"The UTCTime API '{utc_time_api_url}' is unavailable"
+        reason=f"The UTCTime API '{utc_time_api_url}' is unavailable",
     )
     def test_create_service_mesh(self):
         class UTCTime(Schema):
-
             @field
             def now(self) -> Optional[str]:
                 raise NotImplementedError()
 
         class TimeOffset(Schema):
-
             @field
             def now(self, offset: int) -> Optional[str]:
                 raise NotImplementedError()
 
         class TimeOffsetService(TimeOffset):
-
             @field
             def now(self, offset: int) -> Optional[str]:
                 utc_time: UTCTime = ctx.services.utc_time
                 now = datetime.datetime.fromisoformat(utc_time.now())
                 return str(now + datetime.timedelta(seconds=offset))
 
-        service = TimeOffsetService(config={
-            "services": {
-                "utc_time": UTCTime(
-                    url="https://europe-west2-parob-297412.cloudfunctions.net/"
+        service = TimeOffsetService(
+            config={
+                "services": {
+                    "utc_time": UTCTime(
+                        url="https://europe-west2-parob-297412.cloudfunctions.net/"
                         "utc_time"
-                )
+                    )
+                }
             }
-        }).create_service()
+        ).create_service()
 
         client = service.client()
 
-        response = client.get('?query={now(offset:7200)}')
+        response = client.get("?query={now(offset:7200)}")
         assert response
```

### Comparing `graphql_service_framework-1.1.1/tests/test_service_manager.py` & `graphql_service_framework-1.1.2/tests/test_service_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,74 +3,61 @@
 from context_helper import ctx
 from graphql_api import field
 from werkzeug import Response
 from werkzeug.test import Client
 
 from graphql_http_server import GraphQLHTTPServer
 from graphql_service_framework.middleware import ServiceMeshMiddleware
-from graphql_service_framework.mesh import \
-    ServiceConnection, \
-    ServiceManager
+from graphql_service_framework.mesh import ServiceConnection, ServiceManager
 from tests.utils import available
 
 
 class TestServiceManager:
-
-    utc_time_url = \
-        "https://europe-west2-parob-297412.cloudfunctions.net/utc_time"
+    utc_time_url = "https://europe-west2-parob-297412.cloudfunctions.net/utc_time"
 
     # noinspection DuplicatedCode,PyUnusedLocal
     @pytest.mark.skipif(
         not available(utc_time_url),
-        reason=f"The UTCTime API '{utc_time_url}' is unavailable"
+        reason=f"The UTCTime API '{utc_time_url}' is unavailable",
     )
     def test_service_manager(self):
         from graphql_api import GraphQLAPI
 
         class UTCTimeSchema:
-
             @field
             def now(self) -> str:
                 pass
 
-        connections = [ServiceConnection(
-            name="utc_time",
-            service_url=self.utc_time_url,
-            schema=UTCTimeSchema
-        )]
+        connections = [
+            ServiceConnection(
+                name="utc_time", service_url=self.utc_time_url, schema=UTCTimeSchema
+            )
+        ]
 
         service_manager = ServiceManager(
-            name="gateway",
-            api_version="0.0.1",
-            connections=connections
+            name="gateway", api_version="0.0.1", connections=connections
         )
 
         api = GraphQLAPI()
 
         @api.type(root=True)
         class RootQueryType:
-
             @api.field
             def hello(self, name: str) -> str:
                 utc_time: UTCTimeSchema = ctx.services["utc_time"]
 
                 return f"hey {name}, the time is {utc_time.now()}"
 
         server = GraphQLHTTPServer.from_api(api=api)
 
         client = Client(
-            ServiceMeshMiddleware(
-                server.app(),
-                service_manager,
-                "/service"
-            ),
-            Response
+            ServiceMeshMiddleware(server.app(), service_manager, "/service"), Response
         )
 
-        response = client.get('/service?query={logs}')
+        response = client.get("/service?query={logs}")
 
         assert response.status_code == 200
         assert "ServiceState = OK" in response.text
 
         response = client.get('/?query={hello(name:"rob")}')
 
         assert response.status_code == 200
```

### Comparing `graphql_service_framework-1.1.1/tests/utils.py` & `graphql_service_framework-1.1.2/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,18 @@
     try:
         response = request(
             method,
             url,
             timeout=5,
             verify=False,
             headers={
-                "accept":
-                    "text/html,application/xhtml+xml,application/xml;q=0.9,"
-                    "image/avif,image/webp,image/apng,*/*;q=0.8,"
-                    "application/signed-exchange;v=b3;q=0.7"
-            }
+                "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,"
+                "image/avif,image/webp,image/apng,*/*;q=0.8,"
+                "application/signed-exchange;v=b3;q=0.7"
+            },
         )
     except (ConnectionError, ConnectTimeout, ReadTimeout):
         return False
 
     if response.status_code == 400 or response.status_code == 200:
         return True
```

