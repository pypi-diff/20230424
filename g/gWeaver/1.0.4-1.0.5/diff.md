# Comparing `tmp/gWeaver-1.0.4.tar.gz` & `tmp/gWeaver-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gWeaver-1.0.4.tar", last modified: Mon Apr 24 06:35:27 2023, max compression
+gzip compressed data, was "gWeaver-1.0.5.tar", last modified: Mon Apr 24 06:52:09 2023, max compression
```

## Comparing `gWeaver-1.0.4.tar` & `gWeaver-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.537186 gWeaver-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 06:34:08.000000 gWeaver-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 06:35:27.537186 gWeaver-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 06:34:08.000000 gWeaver-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.533186 gWeaver-1.0.4/gWeaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.533186 gWeaver-1.0.4/gWeaver/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/base/graph_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/base/graph_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/base/graph_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/base/node_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/base/response_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.533186 gWeaver-1.0.4/gWeaver/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.537186 gWeaver-1.0.4/gWeaver/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/management/commands/_private.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/management/commands/graph_migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.537186 gWeaver-1.0.4/gWeaver/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/managers/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.537186 gWeaver-1.0.4/gWeaver/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:34:08.000000 gWeaver-1.0.4/gWeaver/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:35:27.533186 gWeaver-1.0.4/gWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 06:35:27.000000 gWeaver-1.0.4/gWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-24 06:35:27.000000 gWeaver-1.0.4/gWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:35:27.000000 gWeaver-1.0.4/gWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:35:26.000000 gWeaver-1.0.4/gWeaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 06:35:27.000000 gWeaver-1.0.4/gWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 06:35:27.000000 gWeaver-1.0.4/gWeaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 06:35:27.537186 gWeaver-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-24 06:34:08.000000 gWeaver-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 06:51:38.000000 gWeaver-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 06:52:09.970904 gWeaver-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 06:51:38.000000 gWeaver-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/graph_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/graph_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/graph_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/node_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/response_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/gWeaver/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/commands/_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/commands/graph_migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/gWeaver/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/managers/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/gWeaver/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 06:52:09.970904 gWeaver-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-24 06:51:38.000000 gWeaver-1.0.5/setup.py
```

### Comparing `gWeaver-1.0.4/LICENSE.txt` & `gWeaver-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/PKG-INFO` & `gWeaver-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.4
+Version: 1.0.5
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.4/gWeaver/actions.py` & `gWeaver-1.0.5/gWeaver/actions.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/gWeaver/base/graph_actions.py` & `gWeaver-1.0.5/gWeaver/base/graph_actions.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/gWeaver/base/graph_models.py` & `gWeaver-1.0.5/gWeaver/base/graph_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..managers.client import dgraph_client
+# from ..managers.client import dgraph_client
 
 
 # client = dgraph_client().get_client()
 
 class SchemaGenerator:
     def __init__(self, graph_models: list) -> None:
         self.graph_models = graph_models
```

### Comparing `gWeaver-1.0.4/gWeaver/base/graph_views.py` & `gWeaver-1.0.5/gWeaver/base/graph_views.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/gWeaver/base/node_connector.py` & `gWeaver-1.0.5/gWeaver/base/node_connector.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/gWeaver/base/response_constructor.py` & `gWeaver-1.0.5/gWeaver/base/response_constructor.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/gWeaver/management/commands/graph_migrate.py` & `gWeaver-1.0.5/gWeaver/management/commands/graph_migrate.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/gWeaver/managers/client.py` & `gWeaver-1.0.5/gWeaver/managers/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 import pydgraph
 import time
 
 
 class dgraph_client:
     def __init__(self):
-        self.client = pydgraph.DgraphClient(
-            pydgraph.DgraphClientStub('localhost:9080'))
+        try:
+            self.client = pydgraph.DgraphClient(
+                pydgraph.DgraphClientStub('localhost:9080'))
+        except:
+            raise Exception("Dgraph server not running")
 
     def get_client(self):
         return self.client
 
     def read_data(self, query):
         # Create a new transaction.
         return self.client.txn(read_only=True).query(query)
```

### Comparing `gWeaver-1.0.4/gWeaver.egg-info/PKG-INFO` & `gWeaver-1.0.5/gWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.4
+Version: 1.0.5
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.4/gWeaver.egg-info/SOURCES.txt` & `gWeaver-1.0.5/gWeaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.4/setup.py` & `gWeaver-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     + extras_require["doc"]
     + extras_require["python-jose"]
 )
 
 
 setup(
     name="gWeaver",
-    version = "1.0.4",
+    version = "1.0.5",
     url="https://github.com/iamr2k/gWeaver",
     license="MIT",
     description="dgraph operation module for Django REST Framework",
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     author="Rahul Babu K",
     author_email="rahulbabu101@gmail.com",
     install_requires=[
```

