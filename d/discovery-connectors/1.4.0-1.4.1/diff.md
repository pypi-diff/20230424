# Comparing `tmp/discovery-connectors-1.4.0.tar.gz` & `tmp/discovery-connectors-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-connectors-1.4.0.tar", last modified: Sat Apr  8 20:34:34 2023, max compression
+gzip compressed data, was "discovery-connectors-1.4.1.tar", last modified: Mon Apr 24 14:04:14 2023, max compression
```

## Comparing `discovery-connectors-1.4.0.tar` & `discovery-connectors-1.4.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.714393 discovery-connectors-1.4.0/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)     1330 2023-04-08 20:34:34.714627 discovery-connectors-1.4.0/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.702176 discovery-connectors-1.4.0/discovery_connectors.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)     1330 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)      987 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      195 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-04-08 20:34:34.000000 discovery-connectors-1.4.0/discovery_connectors.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.702492 discovery-connectors-1.4.0/ds_connectors/
--rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-04-08 20:34:13.000000 discovery-connectors-1.4.0/ds_connectors/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.707592 discovery-connectors-1.4.0/ds_connectors/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.0/ds_connectors/handlers/cortex_helpers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/hive_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.0/ds_connectors/handlers/mc_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5389 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/mongo_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.0/ds_connectors/handlers/mysql_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/postgres_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/redis_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15587 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/handlers/s3_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.708329 discovery-connectors-1.4.0/ds_connectors/parsers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/parsers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/ds_connectors/parsers/dsv.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-04-08 20:34:34.715484 discovery-connectors-1.4.0/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2352 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.699294 discovery-connectors-1.4.0/tests/
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.709034 discovery-connectors-1.4.0/tests/aws/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/tests/aws/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/tests/aws/s3_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.709581 discovery-connectors-1.4.0/tests/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.0/tests/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.710410 discovery-connectors-1.4.0/tests/managed_content/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.0/tests/managed_content/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.0/tests/managed_content/mc_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.712784 discovery-connectors-1.4.0/tests/mysql/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.0/tests/mysql/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1221 2023-04-08 19:04:25.000000 discovery-connectors-1.4.0/tests/mysql/mongo_handler_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8812 2023-04-08 20:11:13.000000 discovery-connectors-1.4.0/tests/mysql/mysql_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-08 20:34:34.713753 discovery-connectors-1.4.0/tests/po1/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.0/tests/po1/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.430725 discovery-connectors-1.4.1/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-24 14:04:14.430903 discovery-connectors-1.4.1/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      333 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.417939 discovery-connectors-1.4.1/discovery_connectors.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)     1332 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1019 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      197 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       20 2023-04-24 14:04:14.000000 discovery-connectors-1.4.1/discovery_connectors.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.418499 discovery-connectors-1.4.1/ds_connectors/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      111 2023-04-24 14:02:30.000000 discovery-connectors-1.4.1/ds_connectors/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.423198 discovery-connectors-1.4.1/ds_connectors/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1773 2022-05-17 19:58:17.000000 discovery-connectors-1.4.1/ds_connectors/handlers/cortex_helpers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3448 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/hive_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13669 2022-05-17 19:58:17.000000 discovery-connectors-1.4.1/ds_connectors/handlers/mc_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5089 2023-04-24 14:03:48.000000 discovery-connectors-1.4.1/ds_connectors/handlers/mongodb_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5754 2023-04-08 20:31:43.000000 discovery-connectors-1.4.1/ds_connectors/handlers/mysql_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3394 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/postgres_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5522 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/redis_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15587 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/handlers/s3_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.423872 discovery-connectors-1.4.1/ds_connectors/parsers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/parsers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3311 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/ds_connectors/parsers/dsv.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-04-24 14:04:14.431527 discovery-connectors-1.4.1/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2354 2023-04-24 14:03:48.000000 discovery-connectors-1.4.1/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.411323 discovery-connectors-1.4.1/tests/
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.425118 discovery-connectors-1.4.1/tests/aws/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/tests/aws/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      901 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/tests/aws/s3_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.426004 discovery-connectors-1.4.1/tests/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.1/tests/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.427015 discovery-connectors-1.4.1/tests/managed_content/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-05-11 14:11:47.000000 discovery-connectors-1.4.1/tests/managed_content/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2836 2022-05-11 14:11:47.000000 discovery-connectors-1.4.1/tests/managed_content/mc_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.428431 discovery-connectors-1.4.1/tests/mongodb/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-24 14:02:30.000000 discovery-connectors-1.4.1/tests/mongodb/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8334 2023-04-24 14:02:17.000000 discovery-connectors-1.4.1/tests/mongodb/mongodb_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.429697 discovery-connectors-1.4.1/tests/mysql/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-04-08 19:04:25.000000 discovery-connectors-1.4.1/tests/mysql/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8825 2023-04-24 14:02:30.000000 discovery-connectors-1.4.1/tests/mysql/mysql_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-04-24 14:04:14.430277 discovery-connectors-1.4.1/tests/po1/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2022-01-11 19:26:38.000000 discovery-connectors-1.4.1/tests/po1/__init__.py
```

### Comparing `discovery-connectors-1.4.0/LICENSE.txt` & `discovery-connectors-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/PKG-INFO` & `discovery-connectors-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.4.0
+Version: 1.4.1
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: postgress
 Provides-Extra: hive
-Provides-Extra: mongo
+Provides-Extra: mongodb
 Provides-Extra: s3
 Provides-Extra: pandas
 Provides-Extra: yaml
 Provides-Extra: managed_content
 License-File: LICENSE.txt
 
 Discovery Connectors
```

### Comparing `discovery-connectors-1.4.0/discovery_connectors.egg-info/PKG-INFO` & `discovery-connectors-1.4.1/discovery_connectors.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-connectors
-Version: 1.4.0
+Version: 1.4.1
 Summary: an concrete implementation of the Discovery Foundation Project to hold a libary of connectors
 Home-page: http://github.com/gigas64/discovery-connectors
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Discovery connetors
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Provides-Extra: postgress
 Provides-Extra: hive
-Provides-Extra: mongo
+Provides-Extra: mongodb
 Provides-Extra: s3
 Provides-Extra: pandas
 Provides-Extra: yaml
 Provides-Extra: managed_content
 License-File: LICENSE.txt
 
 Discovery Connectors
```

### Comparing `discovery-connectors-1.4.0/discovery_connectors.egg-info/SOURCES.txt` & `discovery-connectors-1.4.1/discovery_connectors.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 discovery_connectors.egg-info/requires.txt
 discovery_connectors.egg-info/top_level.txt
 ds_connectors/__init__.py
 ds_connectors/handlers/__init__.py
 ds_connectors/handlers/cortex_helpers.py
 ds_connectors/handlers/hive_handlers.py
 ds_connectors/handlers/mc_handlers.py
-ds_connectors/handlers/mongo_handlers.py
+ds_connectors/handlers/mongodb_handlers.py
 ds_connectors/handlers/mysql_handlers.py
 ds_connectors/handlers/postgres_handlers.py
 ds_connectors/handlers/redis_handlers.py
 ds_connectors/handlers/s3_handlers.py
 ds_connectors/parsers/__init__.py
 ds_connectors/parsers/dsv.py
 tests/aws/__init__.py
 tests/aws/s3_handler_test.py
 tests/handlers/__init__.py
 tests/managed_content/__init__.py
 tests/managed_content/mc_handler_test.py
+tests/mongodb/__init__.py
+tests/mongodb/mongodb_handler_test.py
 tests/mysql/__init__.py
-tests/mysql/mongo_handler_test.py
 tests/mysql/mysql_handler_test.py
 tests/po1/__init__.py
```

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/cortex_helpers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/cortex_helpers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/hive_handlers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/hive_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/mc_handlers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/mc_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/mongo_handlers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/redis_handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,131 @@
-# Developing Mongo Persist Handler
 import pandas as pd
-from aistac.handlers.abstract_handlers import AbstractSourceHandler, AbstractPersistHandler
-from aistac.handlers.abstract_handlers import HandlerFactory, ConnectorContract
+from aistac.handlers.abstract_handlers import AbstractSourceHandler, ConnectorContract, AbstractPersistHandler, \
+    HandlerFactory
 
-__author__ = 'Darryl Oatridge, Omar Eid'
+__author__ = 'Johan Gielstra'
 
 
-class MongoSourceHandler(AbstractSourceHandler):
+class RedisSourceHandler(AbstractSourceHandler):
     """ A mongoDB source handler"""
 
     def __init__(self, connector_contract: ConnectorContract):
         """ initialise the Hander passing the source_contract dictionary """
         # required module import
-        self.mongo = HandlerFactory.get_module('pymongo')
+        self.redis = HandlerFactory.get_module('redis')
         super().__init__(connector_contract)
-        database = self.connector_contract.kwargs.get("database")
-        self._mongo_database = self.mongo.MongoClient(self.connector_contract.uri)[database]
-        self._mongo_collection = self._mongo_database[self.connector_contract.kwargs.get("collection")]
         self._file_state = 0
         self._changed_flag = True
 
     def supported_types(self) -> list:
         """ The source types supported with this module"""
-        return ['mongo']
+        return ['redis']
 
-    def load_canonical(self, **kwargs) -> pd.DataFrame:
+    def load_canonical(self, **kwargs) -> dict:
         """ returns the canonical dataset based on the source contract
             The canonical in this instance is a dictionary that has the headers as the key and then
             the ordered list of values for that header
         """
+        conn = None
         if not isinstance(self.connector_contract, ConnectorContract):
-            raise ValueError("The PandasSource Connector Contract has not been set")
-
-        _cc = self.connector_contract
-
-        load_params = _cc.kwargs
-        load_params.update(_cc.query)  # Update kwargs with those in the uri query
-        load_params.update(kwargs)     # Update with any passed though the call
-        if load_params.get("aggregate") is not None:
-            return pd.DataFrame(list(self._mongo_collection.aggregate(_cc.kwargs.get("aggregate", []))))
-        elif load_params.get("query") is not None:
-            base_query = self._mongo_collection.find(_cc.kwargs.get("find", load_params.get("query", {})),
-                                                     _cc.kwargs.get("project"))
-            if _cc.kwargs.get("limit") is not None:
-                base_query.limit(_cc.kwargs.get("limit"))
-            if _cc.kwargs.get("skip") is not None:
-                base_query.skip(_cc.kwargs.get("skip"))
-            if _cc.kwargs.get("sort") is not None:
-                base_query.sort(_cc.kwargs.get("sort"))
-            return pd.DataFrame(list(base_query))
-        return pd.DataFrame()
+            raise ValueError("The Connector Contract is not valid")
+        # this supports redis hmap only...
+        cc_params = self.connector_contract.kwargs
+        cc_params.update(kwargs)     # Update with any passed though the call
+
+        match = cc_params.get('match', '*')
+        count = cc_params.get('count', 1000)
+        keys = cc_params.get('keys')
+        if not keys or len(keys) == 0:
+            raise ValueError("RedisConnector requires an array of 'keys'")
+        try:
+            conn = self.redis.from_url(self.connector_contract.uri)
+            rtn_dict = {'id': []}
+            for rowkey in conn.scan_iter(match, count):
+                """
+                {
+                    "col1" = [1,2,3],
+                    "col2" = ["a","b","c"]
+                }
+                """
+                rowdata = conn.hgetall(rowkey)
+                rtn_dict.get('id').append(rowkey.decode())
+                for colkey in keys:
+                    if colkey not in rtn_dict:
+                        rtn_dict[colkey] = []
+                    raw_col_val = rowdata.get(str.encode(colkey))
+                    if raw_col_val:
+                        col_val = raw_col_val.decode()
+                    else:
+                        col_val = None
+                    rtn_dict.get(colkey).append(col_val)
+            conn.close()
+            return rtn_dict
+        except Exception as error:
+            print(error)
+        finally:
+            if conn is not None:
+                conn.close()
+                print('Database connection closed.')
 
     def exists(self) -> bool:
-        """ returns True if the collection exists """
-        _cc = self.connector_contract
-        return _cc.kwargs.get("collection") in self._mongo_database.list_collection_names()
+        return True
 
     def has_changed(self) -> bool:
-        """ returns the amount of documents in the collection
-            ... if the counts change ... then the collection was probably modified ...
-            ... this assumes that records are never edited/updated ... nor deleted ...
-        """
-        _cc = self.connector_contract
-        state = self._mongo_collection.count_documents(_cc.kwargs.get("find", {}))
+        """ returns if the file has been modified"""
+        # TODO: Add in change logic here
+        state = None
         if state != self._file_state:
             self._changed_flag = True
             self._file_state = state
         return self._changed_flag
 
     def reset_changed(self, changed: bool = False):
         """ manual reset to say the file has been seen. This is automatically called if the file is loaded"""
         changed = changed if isinstance(changed, bool) else False
         self._changed_flag = changed
 
 
-class MongoPersistHandler(MongoSourceHandler, AbstractPersistHandler):
-    # a mongoDB persist handler
-
+class RedisPersistHandler(RedisSourceHandler, AbstractPersistHandler):
     def persist_canonical(self, canonical: pd.DataFrame, **kwargs) -> bool:
-        """ persists the canonical dataset
-        Extra Parameters in the ConnectorContract kwargs:
-            - file_type: (optional) the type of the source file. if not set, inferred from the file extension
-        """
+        """ persists the canonical dataset """
         if not isinstance(self.connector_contract, ConnectorContract):
             return False
-        _uri = self.connector_contract.uri
-        return self.backup_canonical(uri=_uri, canonical=canonical, **kwargs)
+        return self.backup_canonical(canonical=canonical, uri=self.connector_contract.uri, **kwargs)
 
-    def backup_canonical(self, canonical: pd.DataFrame, uri: str, **kwargs) -> bool:
-        """ creates a backup of the canonical to an alternative URI  """
+    def remove_canonical(self) -> bool:
         if not isinstance(self.connector_contract, ConnectorContract):
             return False
         _cc = self.connector_contract
-        _address = _cc.parse_address(uri=uri)
-        persist_params = kwargs if isinstance(kwargs, dict) else _cc.kwargs
-        persist_params.update(_cc.parse_query(uri=uri))
+        raise NotImplementedError("remove_canonical for RedisPersistHandler not yet implemented.")
 
-        if _cc.kwargs.get("ordered") is None:
-            resp = self._mongo_collection.insert_many(canonical.to_dict(orient="records"))
-        else:
-            resp = self._mongo_collection.insert_many(canonical.to_dict(orient="records"),
-                                                      ordered=_cc.kwargs.get("ordered"))
-        # print(dir(resp))
-        return len(resp.inserted_ids) == canonical.shape[0]
-
-    def remove_canonical(self) -> bool:
+    def backup_canonical(self, canonical: pd.DataFrame, uri: str, **kwargs) -> bool:
+        """ creates a backup of the canonical to an alternative URI  """
         if not isinstance(self.connector_contract, ConnectorContract):
             return False
         _cc = self.connector_contract
-        raise NotImplementedError("remove_canonical for MongoPersistHandler not yet implemented.")
+        persist_params = kwargs if isinstance(kwargs, dict) else _cc.kwargs
+        persist_params.update(_cc.parse_query(uri=uri))
+        hashprefix = persist_params.get('prefix')
+        if hashprefix is None:
+            raise ValueError("RedisPersistHandler requires a `prefix` to be provided")
+        # use `ifFieldName` to upsert records otherwise assume id is the index of the record in the data frame
+        id_field_name = persist_params.get('idFieldName')
+        use_index_for_id = False
+        to_dict_kwargs = {"orient": "records"}
+        if id_field_name is None:
+            use_index_for_id = True
+        if hashprefix is None:
+            raise ValueError("RedisPersistHandler requires a `prefix` to be provided")
+        conn = self.redis.from_url(self.connector_contract.uri)
+        # TODO if persist_params.get("ordered") is None:
+        # ` ordered=persist_params.get("ordered")` is this needed ?
+        count = 0
+        records = canonical.to_dict(**to_dict_kwargs)
+        for rec in records:
+            if use_index_for_id:
+                idx = count
+            else:
+                idx = rec[id_field_name]
+            conn.hmset(f'{hashprefix}.{idx}', rec)
+            count = count+1
+        return count == canonical.shape[0]
```

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/mysql_handlers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/mysql_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/postgres_handlers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/postgres_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/ds_connectors/handlers/s3_handlers.py` & `discovery-connectors-1.4.1/ds_connectors/handlers/s3_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/ds_connectors/parsers/dsv.py` & `discovery-connectors-1.4.1/ds_connectors/parsers/dsv.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/setup.py` & `discovery-connectors-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     python_requires='>=3.6',
     install_requires=[
         'aistac-foundation',
         'pandas >=0.25',
     ],
     extras_require={'postgress': ['psycopg2'],
                     'hive': ['pyhive'],
-                    'mongo': ['pymongo'],
+                    'mongodb': ['pymongo'],
                     's3': ['boto3', 'botocore'],
                     'pandas': ['pandas>0.25'],
                     'yaml': ['pyyaml'],
                     'managed_content': ['tenacity', 'pyyaml', 'requests', 'urllib3']
                     },
     test_suite='tests',
 )
```

### Comparing `discovery-connectors-1.4.0/tests/aws/s3_handler_test.py` & `discovery-connectors-1.4.1/tests/aws/s3_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/tests/managed_content/mc_handler_test.py` & `discovery-connectors-1.4.1/tests/managed_content/mc_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-connectors-1.4.0/tests/mysql/mysql_handler_test.py` & `discovery-connectors-1.4.1/tests/mysql/mysql_handler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import os
 from pathlib import Path
 import shutil
 import pandas as pd
 from aistac.handlers.abstract_handlers import ConnectorContract
-from ds_discovery import SyntheticBuilder
+from ds_discovery import SyntheticBuilder, Controller
 from aistac.properties.property_manager import PropertyManager
 
 # Pandas setup
 pd.set_option('max_colwidth', 320)
 pd.set_option('display.max_rows', 100)
 pd.set_option('display.max_columns', 99)
 pd.set_option('expand_frame_repr', True)
@@ -47,14 +47,15 @@
 
     def tearDown(self):
         try:
             shutil.rmtree('working')
         except OSError:
             pass
 
+
     def test_handler_default(self):
         sb = SyntheticBuilder.from_memory()
         df = self.data(size=1_000)
         sb.set_persist_uri("mysql://user:pass@localhost:3306/mydb")
         sb.remove_canonical(sb.CONNECTOR_PERSIST)
         self.assertFalse(sb.pm.get_connector_handler(sb.CONNECTOR_PERSIST).exists())
         sb.save_persist_canonical(df)
```

