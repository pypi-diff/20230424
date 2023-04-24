# Comparing `tmp/graphql_service_framework-1.1.0.tar.gz` & `tmp/graphql_service_framework-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.1.0.tar", last modified: Mon Apr 24 07:51:02 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.1.tar", last modified: Mon Apr 24 09:04:20 2023, max compression
```

## Comparing `graphql_service_framework-1.1.0.tar` & `graphql_service_framework-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.263641 graphql_service_framework-1.1.0/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       99 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 07:51:02.263641 graphql_service_framework-1.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 07:51:01.000000 graphql_service_framework-1.1.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.260641 graphql_service_framework-1.1.0/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15511 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     8043 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7613 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     5105 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/service_manager_default.graphql
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/graphql_service_framework/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.261641 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-24 07:51:02.000000 graphql_service_framework-1.1.0/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 07:51:02.264641 graphql_service_framework-1.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:51:02.263641 graphql_service_framework-1.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6367 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/test_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-24 07:50:53.000000 graphql_service_framework-1.1.0/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.072693 graphql_service_framework-1.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 09:04:20.073609 graphql_service_framework-1.1.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 09:04:19.000000 graphql_service_framework-1.1.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.069943 graphql_service_framework-1.1.1/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15905 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/query.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     8043 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7613 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5105 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.071776 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-24 09:04:20.000000 graphql_service_framework-1.1.1/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 09:04:20.073609 graphql_service_framework-1.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:04:20.072693 graphql_service_framework-1.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6367 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-24 09:04:09.000000 graphql_service_framework-1.1.1/tests/utils.py
```

### Comparing `graphql_service_framework-1.1.0/LICENSE` & `graphql_service_framework-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/PKG-INFO` & `graphql_service_framework-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.1.0
+Version: 1.1.1
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.0.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.1.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/conftest.py` & `graphql_service_framework-1.1.1/graphql_service_framework/conftest.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/mesh.py` & `graphql_service_framework-1.1.1/graphql_service_framework/mesh.py`

 * *Files 7% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         self._api_version = api_version
         self._service_version = service_version
         self._started_at = datetime.datetime.now()
         self._has_checked_connections = False
         self._logs = []
 
         fp = os.path.dirname(
-            os.path.realpath(__file__)) + '/service_manager_default.graphql'
+            os.path.realpath(__file__)) + '/query.graphql'
         with open(fp, 'r') as default_query:
             default_query = default_query.read()
 
         self.manager_http_server = GraphQLHTTPServer.from_api(
             api=GraphQLAPI(root=ServiceManager),
             serve_graphiql=True,
             allow_cors=True,
@@ -418,9 +418,21 @@
         """
         All the Services this service is dependent on.
         :return:
         """
         return self._connections or []
 
     @field
+    def packages(self) -> List[str]:
+        """
+        All the Packages this service is dependent on.
+        :return:
+        """
+        import pkg_resources
+        installed_packages = pkg_resources.working_set
+        installed_packages_list = sorted(["%s==%s" % (i.key, i.version)
+                                          for i in installed_packages])
+        return installed_packages_list
+
+    @field
     def logs(self) -> List[str]:
         return self._logs
```

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/middleware.py` & `graphql_service_framework-1.1.1/graphql_service_framework/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.1/graphql_service_framework/schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.1/graphql_service_framework/schema_tracker.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/service.py` & `graphql_service_framework-1.1.1/graphql_service_framework/service.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.1/graphql_service_framework/utils.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.1/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.1.0
+Version: 1.1.1
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.0.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.1.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.0/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.1/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 VERSION
 setup.cfg
 setup.py
 graphql_service_framework/__init__.py
 graphql_service_framework/conftest.py
 graphql_service_framework/mesh.py
 graphql_service_framework/middleware.py
+graphql_service_framework/query.graphql
 graphql_service_framework/schema.py
 graphql_service_framework/schema_tracker.py
 graphql_service_framework/service.py
-graphql_service_framework/service_manager_default.graphql
 graphql_service_framework/utils.py
 graphql_service_framework.egg-info/PKG-INFO
 graphql_service_framework.egg-info/SOURCES.txt
 graphql_service_framework.egg-info/dependency_links.txt
 graphql_service_framework.egg-info/requires.txt
 graphql_service_framework.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `graphql_service_framework-1.1.0/setup.py` & `graphql_service_framework-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     install_requires=[
         "graphql-core>=3.2.0",
         "graphql-api>=1.3.0",
         "werkzeug>=2.2.2",
         "context-helper>=1.0.2",
         "packaging>=21.3",
         "graphql-schema-diff>=1.2.4",
-        "graphql-http-server>=1.4.3",
+        "graphql-http-server>=1.4.4",
         "hypercorn>=0.14.3",
         "pytest",
         "pytest-cov",
         "coverage",
         "flake8"
     ],
     classifiers=[
```

### Comparing `graphql_service_framework-1.1.0/tests/test_schema.py` & `graphql_service_framework-1.1.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/tests/test_service_manager.py` & `graphql_service_framework-1.1.1/tests/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.0/tests/utils.py` & `graphql_service_framework-1.1.1/tests/utils.py`

 * *Files identical despite different names*

