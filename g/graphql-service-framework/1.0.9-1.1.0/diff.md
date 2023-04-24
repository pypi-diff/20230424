# Comparing `tmp/graphql_service_framework-1.0.9.tar.gz` & `tmp/graphql_service_framework-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.0.9.tar", last modified: Thu Apr  6 09:41:55 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.0.tar", last modified: Mon Apr 24 07:51:02 2023, max compression
```

## Comparing `graphql_service_framework-1.0.9.tar` & `graphql_service_framework-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 09:41:55.702175 graphql_service_framework-1.0.9/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       99 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-06 09:41:55.702175 graphql_service_framework-1.0.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-06 09:41:55.000000 graphql_service_framework-1.0.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 09:41:55.701175 graphql_service_framework-1.0.9/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/context.py
--rw-rw-rw-   0 root         (0) root         (0)    14811 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     9496 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7650 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/service_manager_default.graphql
--rw-rw-rw-   0 root         (0) root         (0)     4888 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/graphql_service_framework/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 09:41:55.702175 graphql_service_framework-1.0.9/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-06 09:41:55.000000 graphql_service_framework-1.0.9/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-06 09:41:55.000000 graphql_service_framework-1.0.9/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 09:41:55.000000 graphql_service_framework-1.0.9/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-06 09:41:55.000000 graphql_service_framework-1.0.9/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-06 09:41:55.000000 graphql_service_framework-1.0.9/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-06 09:41:55.703175 graphql_service_framework-1.0.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1370 2023-04-06 09:41:46.000000 graphql_service_framework-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.263641 graphql_service_framework-1.1.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       99 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 07:51:02.263641 graphql_service_framework-1.1.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 07:51:01.000000 graphql_service_framework-1.1.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.260641 graphql_service_framework-1.1.0/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15511 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     8043 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7613 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5105 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/service_manager_default.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.261641 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 07:51:02.264641 graphql_service_framework-1.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.263641 graphql_service_framework-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6367 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/utils.py
```

### Comparing `graphql_service_framework-1.0.9/LICENSE` & `graphql_service_framework-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.0.9/PKG-INFO` & `graphql_service_framework-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.0.9
+Version: 1.1.0
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.0.9.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.0.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework/context.py` & `graphql_service_framework-1.1.0/graphql_service_framework/middleware.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from typing import Dict, Callable, Iterable
 
 from context_helper import Context
 from werkzeug import Request
 
-from graphql_service_framework.manager import ServiceManager
-from graphql_service_framework.wsgi import WSGIApp
+from graphql_service_framework.mesh import ServiceManager
+from graphql_service_framework.service import WSGIFramework
 
 
-class ServiceContextMiddleware:
+class ServiceMeshMiddleware:
 
     def __init__(
             self,
-            app: WSGIApp,
+            wsgi_app: WSGIFramework,
             service_manager: 'ServiceManager',
-            service_management_path: str = None,
+            service_manager_path: str = None,
             check_connections_on_first_request: bool = True,
             context_key: str = "services"
     ):
-        self.app = app
+        self.wsgi_app = wsgi_app
         self.service_manager = service_manager
-        self.service_management_path = service_management_path
+        self.service_manager_path = service_manager_path
         self.connect_on_first_request = check_connections_on_first_request
         self.context_key = context_key
 
     def __call__(
             self,
             environ: Dict,
             start_response: Callable
     ) -> Iterable[bytes]:
         if self.connect_on_first_request:
             self.service_manager.connect()
 
         request = Request(environ)
 
-        if request.path == f"{self.service_management_path}":
-            # Expose the service management HTTP server
-            return self.service_manager.management_http_server.app()(
+        if request.path == f"{self.service_manager_path}":
+            # Expose the service manager HTTP server
+            return self.service_manager.manager_http_server.app()(
                 environ, start_response
             )
 
         with Context(**{self.context_key: self.service_manager}):
-            return self.app(environ, start_response)
+            return self.wsgi_app(environ, start_response)
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework/manager.py` & `graphql_service_framework-1.1.0/graphql_service_framework/mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     OK = "OK"
 
 
 @dataclass
 class ServiceConnection:
     name: str
     api_version_specifier: Optional[str] = None
-    service_url: str = None
+    service_url: Optional[str] = None
     service_manager_url: Optional[str] = None
     http_method: str = "POST"
     raise_error: bool = True
+    ignore_service_manager_error: bool = True
     schema: Type = None
     state: ServiceConnectionState = ServiceConnectionState.UNKNOWN
 
     remote_name: Optional[str] = None
     remote_api_version: Optional[str] = None
     remote_service_version: Optional[str] = None
     remote_service_manager: 'ServiceManager' = None
-    remote_service_manager_api: GraphQLRemoteObject = None
+    remote_service: GraphQLRemoteObject = None
 
     @classmethod
     def graphql_exclude_fields(cls) -> List[str]:
         return [
             'schema',
             'remote_service',
             'remote_service_manager',
-            'remote_service_manager_api'
         ]
 
     def __post_init__(self):
         if self.schema:
             if hasattr(self.schema, "api_version"):
                 try:
                     schema_api_version = getattr(self.schema, "api_version")
@@ -64,15 +64,15 @@
                 except Exception:
                     logging.warning(
                         f"Could not identify the api_version for the "
                         f"connection to {self.name} at {self.service_url}"
                     )
 
         if self.service_url and self.schema:
-            self.remote_service_manager_api = GraphQLRemoteObject(
+            self.remote_service = GraphQLRemoteObject(
                 executor=GraphQLRemoteExecutor(
                     name=to_camel_case(self.name, title=True),
                     url=self.service_url,
                     http_method=self.http_method
                 ),
                 api=GraphQLAPI(root=self.schema)
             )
@@ -108,18 +108,17 @@
 
         logs.append(
             f"[{datetime.datetime.utcnow()}] "
             f"connecting to {name} {self.service_url}"
         )
 
         if self.service_manager_url:
-
             # Attempt to connect to a Service Directory
             logs.append(
-                f"[{datetime.datetime.utcnow()}]  Connecting to Service "
+                f"[{datetime.datetime.utcnow()}] connecting to Service "
                 f"Manager for {name} {self.service_manager_url}"
             )
 
             # noinspection PyTypeChecker
             self.remote_service_manager: ServiceManager = GraphQLRemoteObject(
                 executor=GraphQLRemoteExecutor(
                     name=name,
@@ -127,148 +126,158 @@
                     http_method=self.http_method,
                     http_timeout=timeout
                 ),
                 api=GraphQLAPI(root=ServiceManager)
             )
 
             a = datetime.datetime.now()
-
+            service_manager_error = False
+            uptime = None
             try:
                 uptime = await self.remote_service_manager.call_async("uptime")
             except Exception as err:
+                msg = '' if self.ignore_service_manager_error else 'ERROR: '
                 logs.append(
-                    f"[{datetime.datetime.utcnow()}] ERROR: Unable to connect "
-                    f"to {name}, timed out after "
-                    f"{timeout} seconds, error {err}"
+                    f"[{datetime.datetime.utcnow()}] {msg}unable to connect "
+                    f"to {name} service manager, timed out after "
+                    f"{timeout} seconds. {err}"
                 )
                 self.state = ServiceConnectionState.CONNECTION_ERROR
+                if self.ignore_service_manager_error:
+                    service_manager_error = True
 
-                if self.raise_error:
+                elif self.raise_error:
                     raise ConnectionError(
-                        f"Unable to connect to {name}, timed out after "
+                        f"unable to connect to {name}, timed out after "
                         f"{timeout} seconds, error {err}"
                     )
-                return False
-
-            b = datetime.datetime.now()
-
-            self.remote_name = await self.remote_service_manager \
-                .call_async("name")
-            self.remote_api_version = await \
-                self.remote_service_manager.call_async("api_version")
-            self.remote_service_version = await \
-                self.remote_service_manager.call_async("service_version")
-
-            delta = b - a
-            logs.append(f"[{datetime.datetime.utcnow()}] {name} "
-                        f"Response time {delta} Uptime {uptime}")
-
-            if self.api_version_specifier:
-                try:
-                    specifier = specifiers.Specifier(
-                        self.api_version_specifier
-                    )
-                except specifiers.InvalidSpecifier as err:
-                    logs.append(
-                        f"[{datetime.datetime.utcnow()}] "
-                        f"ERROR: {name} malformed api version specifier "
-                        f"{self.api_version_specifier}"
-                    )
-                    self.state = ServiceConnectionState.VALIDATION_ERROR
-                    if self.raise_error:
-                        raise err
+                else:
                     return False
 
-                try:
-                    service_version = packaging_version.Version(
-                        self.remote_api_version
-                    )
-                except packaging_version.InvalidVersion as err:
-                    logs.append(
-                        f"[{datetime.datetime.utcnow()}] "
-                        f"ERROR: {name} malformed api version found "
-                        f"{self.remote_api_version}"
-                    )
-                    self.state = ServiceConnectionState.VALIDATION_ERROR
-                    if self.raise_error:
-                        raise err
-                    return False
+            if not service_manager_error:
+                b = datetime.datetime.now()
 
-                if not specifier.contains(service_version):
-                    logs.append(
-                        f"[{datetime.datetime.utcnow()}] ERROR: Api version "
-                        f"mismatch, found {self.remote_api_version}, "
-                        f"required {self.api_version_specifier}"
-                    )
-                    self.state = ServiceConnectionState.VALIDATION_ERROR
-                    if self.raise_error:
-                        raise TypeError(
+                self.remote_name = await self.remote_service_manager \
+                    .call_async("name")
+                self.remote_api_version = await \
+                    self.remote_service_manager.call_async("api_version")
+                self.remote_service_version = await \
+                    self.remote_service_manager.call_async("service_version")
+
+                delta = b - a
+                logs.append(f"[{datetime.datetime.utcnow()}] {name} "
+                            f"Response time {delta} Uptime {uptime}")
+
+                if self.api_version_specifier:
+                    try:
+                        specifier = specifiers.SpecifierSet(
+                            self.api_version_specifier,
+                            prereleases=True
+                        )
+                    except specifiers.InvalidSpecifier as err:
+                        logs.append(
+                            f"[{datetime.datetime.utcnow()}] "
+                            f"ERROR: {name} malformed api version specifier "
+                            f"{self.api_version_specifier}"
+                        )
+                        self.state = ServiceConnectionState.VALIDATION_ERROR
+                        if self.raise_error:
+                            raise err
+                        return False
+
+                    try:
+                        service_version = packaging_version.Version(
+                            self.remote_api_version.replace(".dev", "")
+                        )
+                    except packaging_version.InvalidVersion as err:
+                        logs.append(
+                            f"[{datetime.datetime.utcnow()}] "
+                            f"ERROR: {name} malformed api version found "
+                            f"{self.remote_api_version}"
+                        )
+                        self.state = ServiceConnectionState.VALIDATION_ERROR
+                        if self.raise_error:
+                            raise err
+                        return False
+
+                    if not specifier.contains(
+                            service_version,
+                            prereleases=True
+                    ):
+                        logs.append(
+                            f"[{datetime.datetime.utcnow()}] ERROR: "
+                            f"api_version mismatch, found "
+                            f"{self.remote_api_version}, required "
+                            f"{self.api_version_specifier}"
+                        )
+                        self.state = ServiceConnectionState.VALIDATION_ERROR
+                        if self.raise_error:
+                            raise TypeError(
+                                f"[{datetime.datetime.utcnow()}] {name} "
+                                f"api_version mismatch at {self.service_url}, "
+                                f"expecting version "
+                                f"{self.api_version_specifier} "
+                                f"but {self.service_url} identified as "
+                                f"{self.remote_name} version "
+                                f"{self.remote_api_version}."
+                            )
+                        return False
+                    else:
+                        logs.append(
                             f"[{datetime.datetime.utcnow()}] {name} api "
-                            f"version mismatch at {self.service_url}, "
-                            f"expecting version {self.api_version_specifier} "
-                            f"but {self.service_url} identified as "
-                            f"{self.remote_name} version "
-                            f"{self.remote_api_version}."
+                            f"version match {self.remote_api_version} is valid"
+                            f" for {self.api_version_specifier}"
                         )
-                    return False
-                else:
-                    logs.append(
-                        f"[{datetime.datetime.utcnow()}] {name} api version "
-                        f"match {self.remote_api_version} is valid for "
-                        f"{self.api_version_specifier}"
-                    )
 
         executor = GraphQLRemoteExecutor(
             name=name,
             url=self.service_url,
             http_method=self.http_method,
             http_timeout=timeout
         )
 
         try:
             response = await executor.execute_async("query { __typename }")
         except Exception as err:
             logs.append(
                 f"[{datetime.datetime.utcnow()}] ERROR: {name} API error "
-                f"from {self.service_url}, {err}"
+                f"from {self.service_url}. {err}"
             )
             self.state = ServiceConnectionState.CONNECTION_ERROR
             if self.raise_error:
                 raise err
             return False
         else:
             if response.errors:
                 logs.append(
                     f"[{datetime.datetime.utcnow()}] ERROR: {name} API "
-                    f"Response error from {self.service_url}, "
+                    f"Response error from {self.service_url}. "
                     f"{response.errors}"
                 )
                 self.state = ServiceConnectionState.CONNECTION_ERROR
                 if self.raise_error:
                     raise ConnectionError(
                         f"[{datetime.datetime.utcnow()}] ERROR: {name} API "
-                        f"Response error from {self.service_url}, "
+                        f"Response error from {self.service_url}. "
                         f"{response.errors}"
                     )
                 return False
 
         self.state = ServiceConnectionState.OK
         logs.append(
             f"[{datetime.datetime.utcnow()}] ServiceState = OK "
             f"for {name} {self.service_url}"
         )
         return True
 
 
 class ServiceManager:
     """
-    The Service Manager is a management api for a service that advertises
-    the service and creates and maintains connections to other services.
-
-    The Service Manager GraphQL API is accessible at '/service'
+    A manager for a service that advertises the status of the service and
+    creates and maintains connections to other services.
     """
 
     def __init__(
             self,
             name: str,
             schema: Any = None,
             api_version: str = None,
@@ -296,15 +305,15 @@
             else:
                 raise TypeError(f"Invalid schema {schema}")
 
         if api_version:
             packaging_version.Version(api_version)
 
         if not service_version:
-            service_version = os.getenv("SERVICE_VERSION") or "0.0.1dev"
+            service_version = os.getenv("SERVICE_VERSION") or "0.0.0.dev"
 
         if "dev" in service_version:
             logging.warning(
                 f"The {name} Service is using the development Service "
                 f"version {service_version}, ignore this if this"
                 f" is a development build."
             )
@@ -317,15 +326,15 @@
         self._logs = []
 
         fp = os.path.dirname(
             os.path.realpath(__file__)) + '/service_manager_default.graphql'
         with open(fp, 'r') as default_query:
             default_query = default_query.read()
 
-        self.management_http_server = GraphQLHTTPServer.from_api(
+        self.manager_http_server = GraphQLHTTPServer.from_api(
             api=GraphQLAPI(root=ServiceManager),
             serve_graphiql=True,
             allow_cors=True,
             root_value=self,
             graphiql_default_query=default_query
         )
 
@@ -372,15 +381,15 @@
                             loop = None
 
                         if loop and loop.is_running():
                             loop.create_task(service.async_connect())
                         else:
                             asyncio.run(service.async_connect())
 
-                    return service.remote_service_manager_api
+                    return service.remote_service
 
         raise KeyError(f"Service '{service_name}' is not available.")
 
     def __getitem__(self, item):
         return self.__getattr__(item)
 
     @field
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.0/graphql_service_framework/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 from schemadiff import diff, format_diff
 from schemadiff.changes import CriticalityLevel
 
 from graphql_api.api import GraphQLRootTypeDelegate
 from graphql_api import GraphQLAPI
 from graphql_api.remote import GraphQLRemoteExecutor, GraphQLRemoteObject
 
-from graphql_http_server import GraphQLHTTPServer
-
-from graphql_service_framework.context import ServiceContextMiddleware
-from graphql_service_framework.manager import ServiceManager
-from graphql_service_framework.wsgi import WSGIApp
-
 TClient = TypeVar("TClient", bound='Schema')
 
 """
 Schema Provides Utilities to help with a Service
 
 Schema Class Attributes:
     api_version         The version of this schema, this must be defined
@@ -50,26 +44,32 @@
     def __new__(mcs, name, bases, namespace, **kwargs):
         return super().__new__(mcs, name, bases, namespace)
 
     def __init__(cls, name, bases, namespace, api_version=None, **kwargs):
         if api_version:
             cls.api_version = api_version
         else:
-            cls.api_version = "0.0.dev1"
+            for base in bases:
+                if hasattr(base, 'api_version') and base.api_version:
+                    cls.api_version = base.api_version
+
+        if not cls.api_version:
+            cls.api_version = "0.0.1.dev"
         super().__init__(name, bases, namespace)
 
 
-# noinspection PyBroadException
 class Schema(GraphQLRootTypeDelegate, metaclass=APIVersion):
     api_version: str = None
     validate_schema: bool = True
     criticality: Optional[CriticalityLevel] = CriticalityLevel.NonBreaking
     ignore_description_changes: bool = True
 
     def __init__(self, config: Dict = None, url: str = None):
+        if not config:
+            config = {}
         self.config = config
         self.url = url
 
     def __new__(cls, config: Dict = None, url: str = None, *args, **kwargs):
         schema_class = cls.get_schema_class()
         if cls == schema_class:
             return cls.client(url=url)
@@ -111,75 +111,36 @@
 
         return schema
 
     @classmethod
     def client(cls: TClient, url: str = None) -> TClient:
         if not url:
             name = to_snake_case(cls.__name__).upper()
-            url = os.getenv(f"{name}_URL")
+            env_var = f"{name}_URL"
+            url = os.getenv(env_var)
             if not url:
                 raise ValueError(
-                    f"A URL for client {cls.__name__} could not be found"
+                    f"A URL for client {cls.__name__} could not be found. "
+                    f"Please set the `{env_var}` environment variable or "
+                    f"specify a URL when creating the {cls.__name__} client"
                 )
         # noinspection PyTypeChecker
         return GraphQLRemoteObject(
             executor=GraphQLRemoteExecutor(url),
             api=GraphQLAPI(root=cls)
         )
 
     @classmethod
     def graphql_schema(cls) -> GraphQLSchema:
         return GraphQLAPI(root=cls).graphql_schema()[0]
 
-    def create_app(self, config: Dict = None) -> WSGIApp:
-        if not config:
-            config = {}
-
-        config = {**self.config, **config}
-
-        service_name = config.get(
-            "service_name", to_snake_case(self.__class__.__name__)
-        )
-        graphiql_default = config.get("graphiql_default", "")
-        relative_path = config.get("http_relative_path", "")
-        health_path = config.get("http_health_path", f"{relative_path}/health")
-        api_version = config.get("api_version", self.__class__.api_version)
-        service_management_path = config.get(
-            "http_service_management_path", f"{relative_path}/service")
-
-        if not graphiql_default:
-            try:
-                dirname = os.path.dirname(inspect.getfile(self.__class__))
-                graphiql_default = open(
-                    os.path.join(dirname, '../graphiql_default.graphql'),
-                    mode='r'
-                ).read()
-            except Exception:
-                try:
-                    dirname = os.path.dirname(inspect.getfile(self.__class__))
-                    graphiql_default = open(
-                        os.path.join(dirname, '../.graphql'),
-                        mode='r'
-                    ).read()
-                except Exception:
-                    pass
-
-        graphql_http_server = GraphQLHTTPServer.from_api(
-            api=GraphQLAPI(root=self.__class__),
-            root_value=self,
-            graphiql_default_query=graphiql_default,
-            health_path=health_path
-        )
+    def create_service(self, config: Dict = None):
+        from graphql_service_framework import Service
 
-        app = ServiceContextMiddleware(
-            graphql_http_server.app(),
-            ServiceManager(name=service_name, api_version=api_version),
-            service_management_path=service_management_path
-        )
-        return app
+        return Service(root=self, config={**self.config, **(config or {})})
 
 
 def validate(
         graphql_schema: GraphQLSchema,
         service_schema: Type[Schema],
         criticality: CriticalityLevel,
         ignore_description_changes: bool = True
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.0/graphql_service_framework/schema_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     def changes(self):
         if not self.previous_schema():
             return []
         else:
             new_schema_language = print_schema(self.schema.graphql_schema())
             previous_schema_language = print_schema(
                 self.previous_schema().graphql_schema()
-            ).replace(f" {self.package_name}.", " ")
+            ).replace(f"{self.package_name}.", "")
 
             return diff(
                 previous_schema_language,
                 new_schema_language
             )
 
     def change_log(self):
@@ -215,15 +215,14 @@
 
             setup(
                 name='SERVICE_NAME',
                 version='SERVICE_VERSION',
                 packages=['SERVICE_PACKAGE'],
                 install_requires=[
                     'packaging',
-                    'graphql-api',
                     'graphql-service-framework'
                 ]
             )
             """) \
             .replace('SERVICE_NAME', self.name.replace("_", "-")) \
             .replace('SERVICE_VERSION', self.version()) \
             .replace('SERVICE_PACKAGE', f"{self.package_name}.{self.name}")
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.0/graphql_service_framework/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+import dataclasses
 import difflib
 import importlib
 import inspect
 import json
 import os
 import pprint
 import subprocess
 import sys
 
 from typing import Optional
 
-from graphql_service_framework.schema import Schema
+
+def dataclass_from_dict(klass, d):
+    # noinspection PyBroadException
+    try:
+        f_types = {f.name: f.type for f in dataclasses.fields(klass)}
+        return klass(**{f: dataclass_from_dict(f_types[f], d[f]) for f in d})
+    except Exception:
+        return d
 
 
 def set_api_version(code, new_version):
+    from graphql_service_framework.schema import Schema
+
     schema_class_name = Schema.__name__
     if f"{schema_class_name}, api_version=" not in code.lower():
         old = f"{schema_class_name}):\n"
         new = f'{schema_class_name}, api_version=\"{new_version}\"):\n'
         code = code.replace(old, new)
     return code
 
@@ -56,14 +66,15 @@
 
 
 def find_schema(modules):
     schemas = set()
 
     for module in modules:
         for name, obj in module.__dict__.items():
+            from graphql_service_framework import Schema
             if inspect.isclass(obj) \
                     and issubclass(obj, Schema) \
                     and obj != Schema:
                 schemas.add(obj)
 
     if len(schemas) > 1:
         raise TypeError(
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.0/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.0.9
+Version: 1.1.0
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.0.9.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.0.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.0.9/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.0/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 setup.cfg
 setup.py
 graphql_service_framework/__init__.py
-graphql_service_framework/context.py
-graphql_service_framework/manager.py
+graphql_service_framework/conftest.py
+graphql_service_framework/mesh.py
+graphql_service_framework/middleware.py
 graphql_service_framework/schema.py
 graphql_service_framework/schema_tracker.py
+graphql_service_framework/service.py
 graphql_service_framework/service_manager_default.graphql
 graphql_service_framework/utils.py
-graphql_service_framework/wsgi.py
 graphql_service_framework.egg-info/PKG-INFO
 graphql_service_framework.egg-info/SOURCES.txt
 graphql_service_framework.egg-info/dependency_links.txt
 graphql_service_framework.egg-info/requires.txt
-graphql_service_framework.egg-info/top_level.txt
+graphql_service_framework.egg-info/top_level.txt
+tests/__init__.py
+tests/test_schema.py
+tests/test_service_manager.py
+tests/utils.py
```

### Comparing `graphql_service_framework-1.0.9/setup.py` & `graphql_service_framework-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,20 +23,25 @@
                  f'archive/master/graphql-service-framework-v{version}.zip',
     keywords=['GraphQL'],
     description='GraphQL Service Framework.',
     long_description=readme,
     long_description_content_type='text/markdown',
     install_requires=[
         "graphql-core>=3.2.0",
-        "graphql-api>=1.2.28",
+        "graphql-api>=1.3.0",
         "werkzeug>=2.2.2",
         "context-helper>=1.0.2",
         "packaging>=21.3",
         "graphql-schema-diff>=1.2.4",
-        "graphql-http-server>=1.3.36"
+        "graphql-http-server>=1.4.3",
+        "hypercorn>=0.14.3",
+        "pytest",
+        "pytest-cov",
+        "coverage",
+        "flake8"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
```

