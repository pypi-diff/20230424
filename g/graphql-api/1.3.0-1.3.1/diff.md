# Comparing `tmp/graphql-api-1.3.0.tar.gz` & `tmp/graphql-api-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.0.tar", last modified: Sat Apr 22 10:50:39 2023, max compression
+gzip compressed data, was "graphql-api-1.3.1.tar", last modified: Mon Apr 24 14:17:59 2023, max compression
```

## Comparing `graphql-api-1.3.0.tar` & `graphql-api-1.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.418552 graphql-api-1.3.0/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-22 10:50:30.000000 graphql-api-1.3.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-22 10:50:30.000000 graphql-api-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1945 2023-04-22 10:50:39.418552 graphql-api-1.3.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1269 2023-04-22 10:50:30.000000 graphql-api-1.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-22 10:50:38.000000 graphql-api-1.3.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.413557 graphql-api-1.3.0/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8046 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      560 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3693 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      592 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     6166 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    24401 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3073 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6915 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3161 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    34111 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     3492 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5635 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.414556 graphql-api-1.3.0/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1945 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-22 10:50:39.418552 graphql-api-1.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1483 2023-04-22 10:50:30.000000 graphql-api-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.418552 graphql-api-1.3.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5443 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_custom_types.py
--rwxrwxrwx   0 root         (0) root         (0)     5766 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     7401 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    36924 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4347 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    19028 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3722 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.895662 graphql-api-1.3.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 14:17:50.000000 graphql-api-1.3.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-24 14:17:50.000000 graphql-api-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-04-24 14:17:59.895662 graphql-api-1.3.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-04-24 14:17:50.000000 graphql-api-1.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 14:17:59.000000 graphql-api-1.3.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.890662 graphql-api-1.3.1/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3382 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    23879 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3070 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32840 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     3372 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5612 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.891662 graphql-api-1.3.1/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 14:17:59.895662 graphql-api-1.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-04-24 14:17:50.000000 graphql-api-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.894662 graphql-api-1.3.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5129 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_custom_types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5183 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    17896 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.0/LICENSE` & `graphql-api-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.0/PKG-INFO` & `graphql-api-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.0
+Version: 1.3.1
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.0/graphql-api-v1.3.0.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.1/graphql-api-v1.3.1.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,15 @@
 Framework for building a GraphQL API with Python
 
 [![coverage report](https://gitlab.com/parob/graphql-api/badges/master/coverage.svg)](https://gitlab.com/parob/graphql-api/commits/master)
 
 [![pipeline status](https://gitlab.com/parob/graphql-api/badges/master/pipeline.svg)](https://gitlab.com/parob/graphql-api/commits/master)
 
 
+
 ## Installation
 
 ##### Pip
 ```
 pip install graphql-api
 ```
```

### Comparing `graphql-api-1.3.0/README.md` & `graphql-api-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Framework for building a GraphQL API with Python
 
 [![coverage report](https://gitlab.com/parob/graphql-api/badges/master/coverage.svg)](https://gitlab.com/parob/graphql-api/commits/master)
 
 [![pipeline status](https://gitlab.com/parob/graphql-api/badges/master/pipeline.svg)](https://gitlab.com/parob/graphql-api/commits/master)
 
 
+
 ## Installation
 
 ##### Pip
 ```
 pip install graphql-api
 ```
```

### Comparing `graphql-api-1.3.0/graphql_api/api.py` & `graphql-api-1.3.1/graphql_api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,93 +4,74 @@
 from graphql import (
     GraphQLSchema,
     GraphQLObjectType,
     GraphQLField,
     GraphQLString,
     is_named_type,
     ExecutionResult,
-    GraphQLType
+    GraphQLType,
 )
 
 from graphql_api import GraphQLError
 
 from graphql_api.executor import GraphQLExecutor, GraphQLBaseExecutor
 from graphql_api.context import GraphQLContext
 from graphql_api.reduce import GraphQLSchemaReducer, GraphQLFilter
 from graphql_api.mapper import GraphQLTypeMapper
 
 
 class GraphQLFieldContext:
-
     def __init__(self, meta, query=None):
         self.meta = meta
         self.query = query
 
     def __str__(self):
         query_str = ""
         if self.query:
-            query_str = f', query: {query_str}' if self.query else ''
+            query_str = f", query: {query_str}" if self.query else ""
         return f"<Node meta: {self.meta}{query_str}>"
 
 
 class GraphQLRequestContext:
-
     def __init__(self, args, info):
         self.args = args
         self.info = info
 
 
 def decorate(
-        func: Callable,
-        _type: str,
-        schema: "GraphQLAPI" = None,
-        meta: Dict = None
+    func: Callable, _type: str, schema: "GraphQLAPI" = None, meta: Dict = None
 ):
     func.graphql = True
     func.defined_on = func
 
     if not meta:
         meta = {}
 
-    api = {
-        "defined_on": func,
-        "meta": meta,
-        "type": _type,
-        "schema": schema
-    }
+    api = {"defined_on": func, "meta": meta, "type": _type, "schema": schema}
 
     if not hasattr(func, "schemas"):
         func.schemas = {}
 
     if hasattr(func, "schemas"):
         func.schemas[schema] = api
 
     return func
 
 
 def decorator(a, b, _type):
     func = a if callable(a) else b if callable(b) else None
     meta = a if isinstance(a, dict) else b if isinstance(b, dict) else None
-    schema = a if isinstance(a, GraphQLAPI) else \
-        b if isinstance(b, GraphQLAPI) else None
+    schema = (
+        a if isinstance(a, GraphQLAPI) else b if isinstance(b, GraphQLAPI) else None
+    )
 
     if func:
-        return decorate(
-            func=func,
-            _type=_type,
-            schema=schema,
-            meta=meta
-        )
+        return decorate(func=func, _type=_type, schema=schema, meta=meta)
 
-    return lambda _func: decorate(
-        func=_func,
-        _type=_type,
-        schema=schema,
-        meta=meta
-    )
+    return lambda _func: decorate(func=_func, _type=_type, schema=schema, meta=meta)
 
 
 class GraphQLRootTypeDelegate:
     infer_subclass_fields = True
 
     @classmethod
     def validate_graphql_schema(cls, schema: GraphQLSchema) -> GraphQLSchema:
@@ -100,29 +81,22 @@
         :param schema: The GraphQL schema that is generated by
         :return:schema: The validated and updated GraphQL schema.
         """
         return schema
 
 
 class GraphQLAPI(GraphQLBaseExecutor):
-
     def field(self=None, meta=None, mutable=False):
         _type = "query"
         if mutable:
             _type = "mutation"
 
         return decorator(self, meta, _type=_type)
 
-    def type(
-            self=None,
-            meta=None,
-            abstract=False,
-            interface=False,
-            root=False
-    ):
+    def type(self=None, meta=None, abstract=False, interface=False, root=False):
         _type = "object"
         if interface:
             _type = "interface"
         elif abstract:
             _type = "abstract"
         elif root:
             return self.set_root
@@ -130,19 +104,19 @@
         return decorator(self, meta, _type=_type)
 
     def set_root(self, root_type):
         self.root_type = root_type
         return root_type
 
     def __init__(
-            self,
-            root: Type = None,
-            middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
-            filters: List[GraphQLFilter] = None,
-            error_protection=True
+        self,
+        root: Type = None,
+        middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
+        filters: List[GraphQLFilter] = None,
+        error_protection=True,
     ):
         super().__init__()
         if middleware is None:
             middleware = []
 
         self.root_type = root
         self.middleware = middleware
@@ -157,127 +131,110 @@
 
         if self.root_type:
             # Create the root query
             query_mapper = GraphQLTypeMapper(schema=self)
             query: GraphQLType = query_mapper.map(self.root_type)
 
             if not isinstance(query, GraphQLObjectType):
-                raise GraphQLError(
-                    f"Query {query} was not a valid ObjectType."
-                )
+                raise GraphQLError(f"Query {query} was not a valid ObjectType.")
 
             # Filter the root query
             filtered_query = GraphQLSchemaReducer.reduce_query(
-                query_mapper,
-                query,
-                filters=self.filters
+                query_mapper, query, filters=self.filters
             )
 
             if query_mapper.validate(filtered_query, evaluate=True):
-                schema_args['query'] = filtered_query
+                schema_args["query"] = filtered_query
                 query_types = query_mapper.types()
                 registry = query_mapper.registry
 
             else:
                 query_types = set()
                 registry = None
 
             # Create the root mutation
             mutation_mapper = GraphQLTypeMapper(
-                as_mutable=True,
-                suffix="Mutable",
-                registry=registry,
-                schema=self
+                as_mutable=True, suffix="Mutable", registry=registry, schema=self
             )
             mutation: GraphQLType = mutation_mapper.map(self.root_type)
 
             if not isinstance(mutation, GraphQLObjectType):
-                raise GraphQLError(
-                    f"Mutation {mutation} was not a valid ObjectType."
-                )
+                raise GraphQLError(f"Mutation {mutation} was not a valid ObjectType.")
 
             # Filter the root mutation
             filtered_mutation = GraphQLSchemaReducer.reduce_mutation(
-                mutation_mapper,
-                mutation
+                mutation_mapper, mutation
             )
 
             if mutation_mapper.validate(filtered_mutation, evaluate=True):
-                schema_args['mutation'] = filtered_mutation
+                schema_args["mutation"] = filtered_mutation
                 mutation_types = mutation_mapper.types()
             else:
                 mutation_types = set()
 
-            schema_args['types'] = list(query_types | mutation_types)
-            schema_args['types'] = [
-                type_
-                for type_ in schema_args['types'] if is_named_type(type_)
+            schema_args["types"] = list(query_types | mutation_types)
+            schema_args["types"] = [
+                type_ for type_ in schema_args["types"] if is_named_type(type_)
             ]
 
             meta = {**query_mapper.meta, **mutation_mapper.meta}
 
             self.query_mapper = query_mapper
             self.mutation_mapper = mutation_mapper
 
         # Create a placeholder query (every GraphQL schema must have a query)
-        if 'query' not in schema_args:
-            placeholder = GraphQLField(
-                type_=GraphQLString,
-                resolve=lambda *_: ''
-            )
-            schema_args['query'] = GraphQLObjectType(
-                name='PlaceholderQuery',
-                fields={'placeholder': placeholder}
+        if "query" not in schema_args:
+            placeholder = GraphQLField(type_=GraphQLString, resolve=lambda *_: "")
+            schema_args["query"] = GraphQLObjectType(
+                name="PlaceholderQuery", fields={"placeholder": placeholder}
             )
 
         schema = GraphQLSchema(**schema_args)
 
-        if self.root_type and issubclass(
-                self.root_type,
-                GraphQLRootTypeDelegate
-        ):
+        if self.root_type and issubclass(self.root_type, GraphQLRootTypeDelegate):
             schema = self.root_type.validate_graphql_schema(schema)
 
         return schema, meta
 
     def execute(
         self,
         query,
         variables=None,
         operation_name=None,
         root_value: Any = None,
         middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
         middleware_on_introspection: bool = False,
-        error_protection: bool = None
+        error_protection: bool = None,
     ) -> ExecutionResult:
         return self.executor(
             root_value=root_value,
             middleware=middleware,
             middleware_on_introspection=middleware_on_introspection,
-            error_protection=error_protection
+            error_protection=error_protection,
         ).execute(
             query=query,
             variables=variables,
             operation_name=operation_name,
         )
 
     def executor(
         self,
         root_value: Any = None,
         middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
         middleware_on_introspection: bool = False,
-        error_protection: bool = None
+        error_protection: bool = None,
     ) -> GraphQLExecutor:
         schema, meta = self.graphql_schema()
 
         if callable(self.root_type) and root_value is None:
             root_value = self.root_type()
 
         return GraphQLExecutor(
             schema=schema,
             meta=meta,
             root_value=root_value,
             middleware=middleware,
             middleware_on_introspection=middleware_on_introspection,
-            error_protection=error_protection if error_protection is not None
-            else self.error_protection
+            error_protection=error_protection
+            if error_protection is not None
+            else self.error_protection,
         )
```

### Comparing `graphql-api-1.3.0/graphql_api/context.py` & `graphql-api-1.3.1/graphql_api/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 class GraphQLContext:
-
     def __init__(self, schema=None, meta=None, executor=None):
-
         if not meta:
             meta = {}
 
         # Server specific
         self.schema = schema
         self.meta = meta
         self.executor = executor
```

### Comparing `graphql-api-1.3.0/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.1/graphql_api/dataclass_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Type, get_type_hints
 import typing_inspect
 from docstring_parser import parse_from_object
 
-from graphql.type.definition import \
-    GraphQLType, \
-    GraphQLObjectType, \
-    GraphQLField, \
-    GraphQLInputField, \
-    GraphQLNonNull
+from graphql.type.definition import (
+    GraphQLType,
+    GraphQLObjectType,
+    GraphQLField,
+    GraphQLInputField,
+    GraphQLNonNull,
+)
 
 from graphql_api.utils import to_camel_case
 
 
 def type_is_dataclass(_class: Type):
     try:
         from dataclasses import is_dataclass
@@ -24,22 +25,25 @@
 def type_from_dataclass(_class: Type, mapper) -> GraphQLType:
     dataclass_fields = dict(_class.__dataclass_fields__)
     dataclass_types = get_type_hints(_class)
     base_type: GraphQLObjectType = mapper.map(_class, use_graphql_type=False)
     docstrings = parse_from_object(_class)
 
     # Remove any modifiers
-    while hasattr(base_type, 'of_type'):
+    while hasattr(base_type, "of_type"):
         base_type = base_type.of_type
 
     if mapper.as_input:
         return base_type
 
-    exclude_fields = _class.graphql_exclude_fields() \
-        if hasattr(_class, 'graphql_exclude_fields') else []
+    exclude_fields = (
+        _class.graphql_exclude_fields()
+        if hasattr(_class, "graphql_exclude_fields")
+        else []
+    )
 
     properties = {
         name: (field, dataclass_types.get(name))
         for name, field in dataclass_fields.items()
         if not name.startswith("_") and name not in exclude_fields
     }
 
@@ -55,66 +59,54 @@
             local_fields = {}
 
             for prop_name, (field, field_type) in local_properties.items():
 
                 def local_resolver():
                     local_prop_name = prop_name
 
-                    def resolver(
-                        self,
-                        info=None,
-                        context=None,
-                        *args,
-                        **kwargs
-                    ):
+                    def resolver(self, info=None, context=None, *args, **kwargs):
                         return getattr(self, local_prop_name)
+
                     return resolver
 
                 description = None
 
                 for docstring_param in docstrings.params:
                     if docstring_param.arg_name == prop_name:
                         description = docstring_param.description
 
                 type_: GraphQLType = local_mapper.map(type_=field_type)
 
                 nullable = False
 
                 if typing_inspect.is_union_type(field_type):
-                    union_args = typing_inspect.get_args(
-                        field_type,
-                        evaluate=True
-                    )
+                    union_args = typing_inspect.get_args(field_type, evaluate=True)
                     if type(None) in union_args:
                         nullable = True
 
                 if not nullable:
                     type_: GraphQLType = GraphQLNonNull(type_)
 
                 if local_mapper.as_input:
-                    field = GraphQLInputField(
-                        type_=type_,
-                        description=description
-                    )
+                    field = GraphQLInputField(type_=type_, description=description)
                 else:
                     field = GraphQLField(
-                        type_=type_,
-                        resolve=local_resolver(),
-                        description=description
+                        type_=type_, resolve=local_resolver(), description=description
                     )
 
                 local_fields[to_camel_case(prop_name)] = field
 
             if local_type_fields:
                 try:
                     fields_ = local_type_fields()
                     for name, field in fields_.items():
                         if name not in local_fields:
                             local_fields[name] = field
                 except AssertionError:
                     pass
 
             return local_fields
+
         return fields_callback
 
     base_type._fields = local_fields_callback()
     return base_type
```

### Comparing `graphql-api-1.3.0/graphql_api/error.py` & `graphql-api-1.3.1/graphql_api/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from graphql import GraphQLError as GraphQLCoreError
 
 
 class GraphQLError(GraphQLCoreError):
-
     def __init__(
         self,
         message,
         nodes=None,
         source=None,
         positions=None,
         path=None,
         original_error=None,
-        extensions=None
+        extensions=None,
     ):
         super(GraphQLError, self).__init__(
             message=message,
             nodes=nodes,
             source=source,
             positions=positions,
             path=path,
             original_error=original_error,
-            extensions=extensions
+            extensions=extensions,
         )
         self.extensions = extensions
```

### Comparing `graphql-api-1.3.0/graphql_api/executor.py` & `graphql-api-1.3.1/graphql_api/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 import inspect
 
 from typing import Any, List, Dict, Callable
 
-from graphql import graphql, graphql_sync, ExecutionContext, GraphQLError, \
-    GraphQLOutputType
+from graphql import (
+    graphql,
+    graphql_sync,
+    ExecutionContext,
+    GraphQLError,
+    GraphQLOutputType,
+)
 
 from graphql.execution import ExecutionResult
 from graphql.type.schema import GraphQLSchema
 
 from graphql_api.context import GraphQLContext
-from graphql_api.middleware import \
-    middleware_field_context, \
-    middleware_request_context, \
-    middleware_local_proxy, \
-    middleware_adapt_enum, middleware_catch_exception
+from graphql_api.middleware import (
+    middleware_field_context,
+    middleware_request_context,
+    middleware_local_proxy,
+    middleware_adapt_enum,
+    middleware_catch_exception,
+)
 
 
 class GraphQLBaseExecutor:
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.validate()
 
     def validate(self):
         pass
 
-    def execute(
-            self,
-            query,
-            variables=None,
-            operation_name=None
-    ) -> ExecutionResult:
+    def execute(self, query, variables=None, operation_name=None) -> ExecutionResult:
         pass
 
     async def execute_async(
-            self,
-            query,
-            variables=None,
-            operation_name=None
+        self, query, variables=None, operation_name=None
     ) -> ExecutionResult:
         pass
 
 
 class ErrorProtectionExecutionContext(ExecutionContext):
     default_error_protection = True
 
     error_protection = "ERROR_PROTECTION"
 
     def handle_field_error(
-            self,
-            error: GraphQLError,
-            return_type: GraphQLOutputType,
+        self,
+        error: GraphQLError,
+        return_type: GraphQLOutputType,
     ) -> None:
-
         error_protection = self.default_error_protection
         original_error = error.original_error
         if hasattr(error, self.error_protection):
             error_protection = getattr(error, self.error_protection)
 
         elif hasattr(original_error, self.error_protection):
             error_protection = getattr(original_error, self.error_protection)
@@ -68,23 +65,22 @@
 
 
 class NoErrorProtectionExecutionContext(ErrorProtectionExecutionContext):
     default_error_protection = False
 
 
 class GraphQLExecutor(GraphQLBaseExecutor):
-
     def __init__(
-            self,
-            schema: GraphQLSchema,
-            meta: Dict = None,
-            root_value: Any = None,
-            middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
-            middleware_on_introspection: bool = False,
-            error_protection: bool = True
+        self,
+        schema: GraphQLSchema,
+        meta: Dict = None,
+        root_value: Any = None,
+        middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
+        middleware_on_introspection: bool = False,
+        error_protection: bool = True,
     ):
         super().__init__()
 
         if meta is None:
             meta = {}
 
         if middleware is None:
@@ -97,101 +93,82 @@
         middleware.insert(0, middleware_adapt_enum)
 
         self.meta = meta
         self.schema = schema
         self.middleware = middleware
         self.root_value = root_value
         self.middleware_on_introspection = middleware_on_introspection
-        self.execution_context_class = ErrorProtectionExecutionContext \
-            if error_protection else NoErrorProtectionExecutionContext
+        self.execution_context_class = (
+            ErrorProtectionExecutionContext
+            if error_protection
+            else NoErrorProtectionExecutionContext
+        )
 
     def execute(
-            self,
-            query,
-            variables=None,
-            operation_name=None,
-            root_value=None,
-            context=None
+        self, query, variables=None, operation_name=None, root_value=None, context=None
     ) -> ExecutionResult:
-
-        context = GraphQLContext(
-            schema=self.schema,
-            meta=self.meta,
-            executor=self
-        )
+        context = GraphQLContext(schema=self.schema, meta=self.meta, executor=self)
 
         if root_value is None:
             root_value = self.root_value
 
         value = graphql_sync(
             self.schema,
             query,
             context_value=context,
             variable_values=variables,
             operation_name=operation_name,
             middleware=self.adapt_middleware(self.middleware),
             root_value=root_value,
-            execution_context_class=self.execution_context_class
+            execution_context_class=self.execution_context_class,
         )
         return value
 
     async def execute_async(
-            self,
-            query,
-            variables=None,
-            operation_name=None,
-            root_value=None,
-            context=None
+        self, query, variables=None, operation_name=None, root_value=None, context=None
     ) -> ExecutionResult:
-
-        context = GraphQLContext(
-            schema=self.schema,
-            meta=self.meta,
-            executor=self
-        )
+        context = GraphQLContext(schema=self.schema, meta=self.meta, executor=self)
 
         if root_value is None:
             root_value = self.root_value
 
         value = await graphql(
             self.schema,
             query,
             context_value=context,
             variable_values=variables,
             operation_name=operation_name,
             middleware=self.adapt_middleware(self.middleware),
             root_value=root_value,
-            execution_context_class=self.execution_context_class
+            execution_context_class=self.execution_context_class,
         )
         return value
 
     @staticmethod
-    def adapt_middleware(
-            middleware,
-            middleware_on_introspection: bool = False
-    ):
-
+    def adapt_middleware(middleware, middleware_on_introspection: bool = False):
         def simplify(_middleware: Callable[[Callable, GraphQLContext], Any]):
             def graphql_middleware(next, root, info, **args):
                 kwargs = {}
                 if "context" in inspect.signature(_middleware).parameters:
                     context: GraphQLContext = info.context
                     kwargs["context"] = context
-                    context.resolve_args['root'] = root
-                    context.resolve_args['info'] = info
-                    context.resolve_args['args'] = args
+                    context.resolve_args["root"] = root
+                    context.resolve_args["info"] = info
+                    context.resolve_args["args"] = args
 
                 return _middleware(lambda: next(root, info, **args), **kwargs)
 
             return graphql_middleware
 
         def skip_if_introspection(_middleware):
             def middleware_with_skip(next, root, info, **args):
-                skip = info.operation.name and \
-                       info.operation.name.value == 'IntrospectionQuery'
+                skip = (
+                    info.operation.name
+                    and info.operation.name.value == "IntrospectionQuery"
+                )
                 if skip:
                     return next(root, info, **args)
                 return _middleware(next, root, info, **args)
 
             return middleware_with_skip
 
         adapters = [simplify]
```

### Comparing `graphql-api-1.3.0/graphql_api/mapper.py` & `graphql-api-1.3.1/graphql_api/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 from graphql import (
     GraphQLObjectType,
     GraphQLField,
     GraphQLString,
     GraphQLList,
     GraphQLBoolean,
     GraphQLInt,
-    GraphQLFloat
+    GraphQLFloat,
 )
 
 from graphql.type.definition import (
     GraphQLType,
     GraphQLUnionType,
     GraphQLInterfaceType,
     GraphQLArgument,
     GraphQLInputObjectType,
     is_input_type,
     GraphQLEnumType,
     GraphQLScalarType,
     GraphQLNonNull,
-    GraphQLInputField
+    GraphQLInputField,
 )
 
 from graphql.pyutils import Undefined, UndefinedType
 
 from graphql_api.context import GraphQLContext
 from graphql_api.types import (
     GraphQLBytes,
     GraphQLUUID,
     GraphQLDateTime,
-    GraphQLJSON, JsonType, GraphQLMappedEnumType
+    GraphQLJSON,
+    JsonType,
+    GraphQLMappedEnumType,
 )
 
 from graphql_api.utils import to_camel_case, to_snake_case, to_input_value
 from graphql_api.exception import GraphQLBaseException
-from graphql_api.dataclass_mapping import \
-    type_is_dataclass, \
-    type_from_dataclass
+from graphql_api.dataclass_mapping import type_is_dataclass, type_from_dataclass
 
 """
 class AnyObject:
 
 
     @classmethod
     def graphql_from_input(cls, age: int):
@@ -72,15 +72,14 @@
 
 
 class GraphQLTypeMapError(GraphQLBaseException):
     pass
 
 
 class GraphQLTypeWrapper:
-
     @classmethod
     def graphql_type(cls, mapper: "GraphQLTypeMapper") -> GraphQLType:
         pass
 
 
 class GraphQLMetaKey(enum.Enum):
     resolve_to_mutable = "RESOLVE_TO_MUTABLE"
@@ -90,46 +89,40 @@
 
 
 class GraphQLMutableField(GraphQLField):
     pass
 
 
 class GraphQLTypeMapper:
-
     def __init__(
-            self,
-            as_mutable=False,
-            as_input=False,
-            registry=None,
-            reverse_registry=None,
-            suffix="",
-            schema=None
+        self,
+        as_mutable=False,
+        as_input=False,
+        registry=None,
+        reverse_registry=None,
+        suffix="",
+        schema=None,
     ):
         self.as_mutable = as_mutable
         self.as_input = as_input
         self.registry = registry or {}
         self.reverse_registry = reverse_registry or {}
         self.suffix = suffix
         self.meta = {}
         self.input_type_mapper = None
         self.schema = schema
 
     def types(self) -> Set[GraphQLType]:
         return set(self.registry.values())
 
-    def map_to_field(
-            self,
-            function_type: Callable,
-            name="",
-            key=""
-    ) -> GraphQLField:
+    def map_to_field(self, function_type: Callable, name="", key="") -> GraphQLField:
         type_hints = typing.get_type_hints(function_type)
         description = inspect.getdoc(function_type)
 
-        return_type = type_hints.pop('return', None)
+        return_type = type_hints.pop("return", None)
 
         if not return_type:
             raise GraphQLTypeMapInvalid(
                 f"Field '{name}.{key}' with function ({function_type}) did "
                 f"not specify a valid return type."
             )
 
@@ -151,17 +144,15 @@
 
         enum_return = None
 
         if isinstance(return_graphql_type, GraphQLEnumType):
             enum_return = return_type
 
         if not nullable:
-            return_graphql_type: GraphQLType = GraphQLNonNull(
-                return_graphql_type
-            )
+            return_graphql_type: GraphQLType = GraphQLNonNull(return_graphql_type)
 
         signature = inspect.signature(function_type)
 
         default_args = {
             key: value.default
             for key, value in signature.parameters.items()
             if value.default is not inspect.Parameter.empty
@@ -169,49 +160,50 @@
 
         input_type_mapper = GraphQLTypeMapper(
             as_mutable=self.as_mutable,
             as_input=True,
             registry=self.registry,
             reverse_registry=self.reverse_registry,
             suffix=self.suffix,
-            schema=self.schema
+            schema=self.schema,
         )
         self.input_type_mapper = input_type_mapper
         arguments = {}
         enum_arguments = {}
 
         include_context = False
 
         for key, hint in type_hints.items():
-            if key == 'context' and \
-                    inspect.isclass(hint) and \
-                    issubclass(hint, GraphQLContext):
+            if (
+                key == "context"
+                and inspect.isclass(hint)
+                and issubclass(hint, GraphQLContext)
+            ):
                 include_context = True
                 continue
 
             arg_type = input_type_mapper.map(hint)
 
             if isinstance(arg_type, GraphQLEnumType):
                 enum_arguments[key] = hint
 
             nullable = key in default_args
             if not nullable:
                 arg_type = GraphQLNonNull(arg_type)
 
             arguments[to_camel_case(key)] = GraphQLArgument(
-                type_=arg_type,
-                default_value=default_args.get(key, Undefined)
+                type_=arg_type, default_value=default_args.get(key, Undefined)
             )
 
         # noinspection PyUnusedLocal
         def resolve(_self, info=None, context=None, *args, **kwargs):
             _args = {to_snake_case(_key): arg for _key, arg in kwargs.items()}
 
             if include_context:
-                _args['context'] = info.context
+                _args["context"] = info.context
 
             function_name = function_type.__name__
             parent_type = _self.__class__
             class_attribute = getattr(parent_type, function_name, None)
             is_property = isinstance(class_attribute, property)
             response = None
 
@@ -237,31 +229,27 @@
             if enum_return:
                 if isinstance(response, enum.Enum):
                     response = response.value
 
             return response
 
         field_class = GraphQLField
-        func_type = get_value(function_type, self.schema, 'type')
+        func_type = get_value(function_type, self.schema, "type")
         if func_type == "mutation":
             field_class = GraphQLMutableField
 
         return field_class(
-            return_graphql_type,
-            arguments,
-            resolve,
-            description=description
+            return_graphql_type, arguments, resolve, description=description
         )
 
     def map_to_union(self, union_type: Union) -> GraphQLType:
         union_args = typing_inspect.get_args(union_type, evaluate=True)
         none_type = type(None)
         union_map: Dict[type, GraphQLType] = {
-            arg: self.map(arg)
-            for arg in union_args if arg and arg != none_type
+            arg: self.map(arg) for arg in union_args if arg and arg != none_type
         }
 
         if len(union_map) == 1:
             _, mapped_type = union_map.popitem()
             return mapped_type
 
         # noinspection PyUnusedLocal
@@ -270,25 +258,22 @@
 
             value_type = type(value)
 
             if isinstance(value, GraphQLRemoteObject):
                 value_type = value.python_type
 
             for arg, _mapped_type in union_map.items():
-                if issubclass(value_type, arg) \
-                        and hasattr(_mapped_type, 'name'):
+                if issubclass(value_type, arg) and hasattr(_mapped_type, "name"):
                     return _mapped_type.name
 
         names = [arg.__name__ for arg in union_args]
         name = f"{''.join(names)}{self.suffix}Union"
 
         return GraphQLUnionType(
-            name,
-            types=[*union_map.values()],
-            resolve_type=resolve_type
+            name, types=[*union_map.values()], resolve_type=resolve_type
         )
 
     def map_to_list(self, type_: List) -> GraphQLList:
         list_subtype = typing_inspect.get_args(type_)[0]
 
         list_type = GraphQLList(type_=self.map(list_subtype))
 
@@ -307,17 +292,15 @@
         enum_type = type_
         name = f"{type_.__name__}Enum"
         # Enums don't include a suffix as they are immutable
 
         description = inspect.getdoc(enum_type)
 
         enum_type = GraphQLMappedEnumType(
-            name=name,
-            values=enum_type,
-            description=description
+            name=name, values=enum_type, description=description
         )
 
         enum_type.enum_type = type_
 
         def serialize(_self, value) -> Union[str, None, UndefinedType]:
             if value and isinstance(value, collections.abc.Hashable):
                 if isinstance(value, enum.Enum):
@@ -341,15 +324,15 @@
         ([str], GraphQLString),
         ([bytes], GraphQLBytes),
         ([bool], GraphQLBoolean),
         ([int], GraphQLInt),
         ([dict, list, set], GraphQLJSON),
         ([float], GraphQLFloat),
         ([datetime], GraphQLDateTime),
-        ([type(None)], None)
+        ([type(None)], None),
     ]
 
     def scalar_classes(self):
         classes = []
         for scalar_class_map in self.scalar_map:
             for scalar_class in scalar_class_map[0]:
                 classes.append(scalar_class)
@@ -357,15 +340,18 @@
 
     def map_to_scalar(self, class_type: Type) -> GraphQLScalarType:
         for test_types, graphql_type in self.scalar_map:
             for test_type in test_types:
                 if issubclass(class_type, test_type):
                     return graphql_type
 
-    def map_to_interface(self, class_type: Type, ) -> GraphQLType:
+    def map_to_interface(
+        self,
+        class_type: Type,
+    ) -> GraphQLType:
         subclasses = class_type.__subclasses__()
         name = class_type.__name__
 
         for subclass in subclasses:
             if not is_abstract(subclass, self.schema):
                 self.map(subclass)
 
@@ -376,49 +362,49 @@
 
         def local_resolve_type():
             local_self = self
 
             # noinspection PyUnusedLocal
             def resolve_type(value, info, _type):
                 value = local_self.map(type(value))
-                if hasattr(value, 'name'):
+                if hasattr(value, "name"):
                     return value.name
+
             return resolve_type
 
         def local_fields():
             local_self = self
             local_class_funcs = class_funcs
             local_class_type = class_type
             local_name = name
 
             def fields():
                 fields_ = {}
                 for key_, func_ in local_class_funcs:
                     local_class_name = local_class_type.__name__
                     func_.__globals__[local_class_name] = local_class_type
                     fields_[to_camel_case(key_)] = local_self.map_to_field(
-                        func_,
-                        local_name,
-                        key_
+                        func_, local_name, key_
                     )
 
                 return fields_
+
             return fields
 
         return GraphQLInterfaceType(
             interface_name,
             fields=local_fields(),
             resolve_type=local_resolve_type(),
-            description=description
+            description=description,
         )
 
     def map_to_input(self, class_type: Type) -> GraphQLType:
         name = f"{class_type.__name__}{self.suffix}Input"
 
-        if hasattr(class_type, 'graphql_from_input'):
+        if hasattr(class_type, "graphql_from_input"):
             creator = class_type.graphql_from_input
             func = creator
 
         else:
             creator = class_type
             # noinspection PyTypeChecker
             func = class_type.__init__
@@ -440,25 +426,23 @@
         default_args = {
             key: value.default
             for key, value in signature.parameters.items()
             if value.default is not inspect.Parameter.empty
         }
 
         def local_fields():
-
             local_name = name
             local_self = self
             local_type_hints = type_hints
             local_default_args = default_args
 
             def fields():
                 arguments = {}
 
                 for key, hint in local_type_hints.items():
-
                     input_arg_type = local_self.map(hint)
 
                     nullable = key in local_default_args
                     if not nullable:
                         # noinspection PyTypeChecker
                         input_arg_type = GraphQLNonNull(input_arg_type)
 
@@ -469,49 +453,45 @@
                             default_value = to_input_value(default_value)
                         except ValueError as _err:
                             raise ValueError(
                                 f"Unable to map {local_name}.{key}, {_err}."
                             )
 
                     arguments[to_camel_case(key)] = GraphQLInputField(
-                        type_=input_arg_type,
-                        default_value=default_value
+                        type_=input_arg_type, default_value=default_value
                     )
                 return arguments
 
             return fields
 
         def local_container_type():
             local_creator = creator
 
             def container_type(data):
-                data = {
-                    to_snake_case(key): value
-                    for key, value in data.items()
-                }
+                data = {to_snake_case(key): value for key, value in data.items()}
                 return local_creator(**data)
 
             return container_type
 
         return GraphQLInputObjectType(
             name,
             fields=local_fields(),
             out_type=local_container_type(),
-            description=description
+            description=description,
         )
 
     def map_to_object(self, class_type: Type) -> GraphQLType:
         name = f"{class_type.__name__}{self.suffix}"
         description = inspect.getdoc(class_type)
 
         class_funcs = get_class_funcs(class_type, self.schema, self.as_mutable)
 
         for key, func in class_funcs:
-            func_meta = get_value(func, self.schema, 'meta')
-            func_meta['type'] = get_value(func, self.schema, 'type')
+            func_meta = get_value(func, self.schema, "meta")
+            func_meta["type"] = get_value(func, self.schema, "type")
 
             self.meta[(name, to_snake_case(key))] = func_meta
 
         def local_interfaces():
             local_class_type = class_type
             local_self = self
 
@@ -539,42 +519,35 @@
             def fields():
                 fields_ = {}
 
                 for key_, func_ in local_class_funcs:
                     local_class_type_name = local_class_type.__name__
                     func_.__globals__[local_class_type_name] = local_class_type
                     fields_[to_camel_case(key_)] = local_self.map_to_field(
-                        func_,
-                        local_name,
-                        key_
+                        func_, local_name, key_
                     )
 
                 return fields_
 
             return fields
 
         obj = GraphQLObjectType(
-            name,
-            local_fields(),
-            local_interfaces(),
-            description=description
+            name, local_fields(), local_interfaces(), description=description
         )
 
         return obj
 
     def rmap(self, graphql_type: GraphQLType) -> Type:
-        while hasattr(graphql_type, 'of_type'):
+        while hasattr(graphql_type, "of_type"):
             graphql_type = graphql_type.of_type
 
         return self.reverse_registry.get(graphql_type)
 
     def map(self, type_, use_graphql_type=True) -> GraphQLType:
-
         def _map(type__) -> GraphQLType:
-
             if type_ == JsonType:
                 return GraphQLJSON
 
             if use_graphql_type and inspect.isclass(type__):
                 if issubclass(type__, GraphQLTypeWrapper):
                     return type__.graphql_type(mapper=self)
 
@@ -585,16 +558,17 @@
                 return self.map_to_union(type__)
 
             if typing_inspect.is_literal_type(type__):
                 return self.map_to_literal(type__)
 
             origin_type = get_origin(type__)
 
-            if inspect.isclass(origin_type) and \
-                    issubclass(get_origin(type__), (List, Set)):
+            if inspect.isclass(origin_type) and issubclass(
+                get_origin(type__), (List, Set)
+            ):
                 return self.map_to_list(type__)
 
             if inspect.isclass(type__):
                 if issubclass(type__, GraphQLType):
                     return type__()
 
                 if issubclass(type__, tuple(self.scalar_classes())):
@@ -610,18 +584,19 @@
                     return self.map_to_input(type__)
                 else:
                     return self.map_to_object(type__)
 
             if isinstance(type__, GraphQLType):
                 return type__
 
-        key_hash = abs(hash(str(type_))) % (10 ** 8)
-        suffix = {'|' + self.suffix if self.suffix else ''}
-        generic_key = f"Registry({key_hash})" \
-                      f"{suffix}|{self.as_input}|{self.as_mutable}"
+        key_hash = abs(hash(str(type_))) % (10**8)
+        suffix = {"|" + self.suffix if self.suffix else ""}
+        generic_key = (
+            f"Registry({key_hash})" f"{suffix}|{self.as_input}|{self.as_mutable}"
+        )
 
         generic_registry_value = self.registry.get(generic_key, None)
 
         if generic_registry_value:
             return generic_registry_value
 
         value: GraphQLType = _map(type_)
@@ -665,30 +640,23 @@
 
             elif not callable(type_._fields) and len(type_._fields) == 0:
                 return False
 
         return True
 
 
-def get_class_funcs(
-        class_type,
-        schema,
-        mutable=False
-) -> List[Tuple[Any, Any]]:
+def get_class_funcs(class_type, schema, mutable=False) -> List[Tuple[Any, Any]]:
     members = []
     for _class_type in class_type.mro():
         for key, member in inspect.getmembers(_class_type):
             if not (key.startswith("__") and key.endswith("__")):
                 members.append((key, member))
 
-    if hasattr(class_type, 'graphql_fields'):
-        members += [
-            (func.__name__, func)
-            for func in class_type.graphql_fields()
-        ]
+    if hasattr(class_type, "graphql_fields"):
+        members += [(func.__name__, func) for func in class_type.graphql_fields()]
     func_members = []
 
     for key, member in reversed(members):
         if isinstance(member, property):
             getter = member.fget
             if getter:
                 func_members.append((key, getter))
@@ -696,36 +664,33 @@
 
             if setter:
                 func_members.append((key, setter))
         else:
             func_members.append((key, member))
 
     def matches_criterion(func):
-        func_type = get_value(func, schema, 'type')
+        func_type = get_value(func, schema, "type")
         return func_type == "query" or (mutable and func_type == "mutation")
 
     callable_funcs = []
 
     inherited_fields = {}
     for key, member in func_members:
-        if getattr(member, 'graphql', None) and key != "test_property":
+        if getattr(member, "graphql", None) and key != "test_property":
             inherited_fields[key] = {**member.__dict__}
         elif key in inherited_fields:
-            member.__dict__ = {
-                **inherited_fields[key],
-                'defined_on': member
-            }
+            member.__dict__ = {**inherited_fields[key], "defined_on": member}
 
     done = []
 
     for key, member in reversed(func_members):
         if is_graphql(member, schema=schema) and matches_criterion(member):
             if not callable(member):
                 type_hints = typing.get_type_hints(member)
-                return_type = type_hints.pop('return', None)
+                return_type = type_hints.pop("return", None)
 
                 def local_func():
                     local_key = key
                     local_member = member
 
                     def func(self) -> return_type:
                         return getattr(self, local_key)
@@ -733,15 +698,15 @@
                     func.graphql = local_member.graphql
                     func.defined_on = local_member.defined_on
                     func.schemas = {
                         schema: {
                             "meta": local_member.meta,
                             "type": local_member.type,
                             "defined_on": local_member.defined_on,
-                            "schema": schema
+                            "schema": schema,
                         }
                     }
 
                     return func
 
                 func = local_func()
 
@@ -757,33 +722,33 @@
 
 def get_value(type_, schema, key):
     if is_graphql(type_, schema):
         return type_.schemas.get(schema, type_.schemas.get(None)).get(key)
 
 
 def is_graphql(type_, schema):
-    graphql = getattr(type_, 'graphql', None)
-    schemas = getattr(type_, 'schemas', {})
+    graphql = getattr(type_, "graphql", None)
+    schemas = getattr(type_, "schemas", {})
     valid_schema = schema in schemas.keys() or None in schemas.keys()
 
     return graphql and schemas and valid_schema
 
 
 def is_interface(type_, schema):
     if is_graphql(type_, schema):
-        type_type = get_value(type_, schema, 'type')
-        type_defined_on = get_value(type_, schema, 'defined_on')
+        type_type = get_value(type_, schema, "type")
+        type_defined_on = get_value(type_, schema, "defined_on")
 
         return type_type == "interface" and type_defined_on == type_
 
 
 def is_abstract(type_, schema):
     if is_graphql(type_, schema):
-        type_type = get_value(type_, schema, 'type')
-        type_defined_on = get_value(type_, schema, 'defined_on')
+        type_type = get_value(type_, schema, "type")
+        type_defined_on = get_value(type_, schema, "defined_on")
 
         return type_type == "abstract" and type_defined_on == type_
 
 
 def is_scalar(type_):
     for test_types, graphql_type in GraphQLTypeMapper.scalar_map:
         for test_type in test_types:
```

### Comparing `graphql-api-1.3.0/graphql_api/middleware.py` & `graphql-api-1.3.1/graphql_api/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,43 +11,44 @@
 
 
 def middleware_catch_exception(next, context: GraphQLContext):
     try:
         value = next()
     except Exception as err:
         from graphql_api.executor import ErrorProtectionExecutionContext
+
         info: GraphQLResolveInfo = context.resolve_args.get("info")
 
         field_meta = context.field.meta
         if field_meta.get(GraphQLMetaKey.error_protection) is not None:
             setattr(
                 err,
                 ErrorProtectionExecutionContext.error_protection,
-                field_meta.get(GraphQLMetaKey.error_protection)
+                field_meta.get(GraphQLMetaKey.error_protection),
             )
 
         return_type = info.return_type
         ignored = isinstance(return_type, GraphQLNonNull)
 
         print(
             f"GraphQLField '{info.field_name}' on '{info.parent_type.name}' "
             f"resolver {'(ignored) ' if ignored else ''}Exception: {err} ",
-            file=sys.stderr
+            file=sys.stderr,
         )
         traceback.print_exc()
         raise err
 
     return value
 
 
 def middleware_local_proxy(next):
     value = next()
 
     # Compatibility with LocalProxy from Werkzeug
-    if hasattr(value, '_get_current_object'):
+    if hasattr(value, "_get_current_object"):
         value = value._get_current_object()
 
     if isinstance(value, Exception):
         raise value
 
     return value
 
@@ -62,16 +63,16 @@
 
     return value
 
 
 def middleware_request_context(next, context: GraphQLContext):
     from graphql_api.api import GraphQLRequestContext
 
-    info = context.resolve_args.get('info')
-    args = context.resolve_args.get('args')
+    info = context.resolve_args.get("info")
+    args = context.resolve_args.get("args")
 
     if info.context.request:
         return next()
 
     args = {to_snake_case(key): arg for key, arg in args.items()}
     graphql_request = GraphQLRequestContext(args=args, info=info)
 
@@ -84,32 +85,31 @@
 
     return value
 
 
 def middleware_field_context(next, context: GraphQLContext):
     from graphql_api.api import GraphQLFieldContext
 
-    info = context.resolve_args.get('info')
+    info = context.resolve_args.get("info")
 
     field_meta = info.context.meta.get(
-        (info.parent_type.name, to_snake_case(info.field_name)),
-        {}
+        (info.parent_type.name, to_snake_case(info.field_name)), {}
     )
     return_type = info.return_type
 
     if field_meta is None:
         field_meta = {}
 
     if return_type and isinstance(return_type, GraphQLNonNull):
         return_type = return_type.of_type
 
     kwargs = {}
     if return_type and isinstance(return_type, GraphQLObjectType):
         sub_loc = info.field_nodes[0].selection_set.loc
-        kwargs['query'] = sub_loc.source.body[sub_loc.start:sub_loc.end]
+        kwargs["query"] = sub_loc.source.body[sub_loc.start : sub_loc.end]
 
     info.context.field = GraphQLFieldContext(meta=field_meta, **kwargs)
 
     try:
         value = next()
     finally:
         info.context.field = None
```

### Comparing `graphql-api-1.3.0/graphql_api/reduce.py` & `graphql-api-1.3.1/graphql_api/reduce.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from typing import List
 
 from graphql import GraphQLNonNull, GraphQLList, GraphQLObjectType
 from graphql.type.definition import GraphQLInterfaceType
 
-from graphql_api.mapper import \
-    GraphQLMutableField, \
-    GraphQLTypeMapError, \
-    GraphQLMetaKey
+from graphql_api.mapper import GraphQLMutableField, GraphQLTypeMapError, GraphQLMetaKey
 from graphql_api.utils import has_mutable, iterate_fields, to_snake_case
 
 
 class GraphQLFilter:
-
     def filter_field(self, name, meta: dict) -> bool:
         """
         Return True to filter (remove) a field from the schema
         """
         raise NotImplementedError()
 
 
 class TagFilter(GraphQLFilter):
-
     def __init__(self, tags: List[str] = None):
         """
         Remove any fields that are tagged with a tag in tags
         """
         self.tags = tags
 
     def filter_field(self, name: str, meta: dict) -> bool:
@@ -34,25 +29,22 @@
             if tag in self.tags:
                 return True
 
         return False
 
 
 class GraphQLSchemaReducer:
-
     @staticmethod
     def reduce_query(mapper, root, filters=None):
         query: GraphQLObjectType = mapper.map(root)
 
         # Remove any types that have no fields
         # (and remove any fields that returned that type)
         invalid_types, invalid_fields = GraphQLSchemaReducer.invalid(
-            root_type=query,
-            filters=filters,
-            meta=mapper.meta
+            root_type=query, filters=filters, meta=mapper.meta
         )
 
         for type_, key in invalid_fields:
             del type_.fields[key]
 
         for key, value in dict(mapper.registry).items():
             if value in invalid_types:
@@ -76,28 +68,30 @@
 
         # Replace fields that have no mutable
         # subtypes with their non-mutable equivalents
 
         for type_, key, field in iterate_fields(mutation):
             field_type = field.type
             meta = mapper.meta.get((type_.name, to_snake_case(key)), {})
-            field_definition_type = meta.get('type', 'query')
+            field_definition_type = meta.get("type", "query")
 
             wraps = []
             while isinstance(field_type, (GraphQLNonNull, GraphQLList)):
                 wraps.append(field_type.__class__)
                 field_type = field_type.of_type
 
             if meta.get(GraphQLMetaKey.resolve_to_mutable):
                 # Flagged as mutable
                 continue
 
             if field_definition_type == "query":
-                if mapper.suffix in str(field_type) or \
-                        field_type in filtered_mutation_types:
+                if (
+                    mapper.suffix in str(field_type)
+                    or field_type in filtered_mutation_types
+                ):
                     # Calculated as it as mutable
                     continue
 
             # convert it to immutable
             query_type_name = str(field_type).replace(mapper.suffix, "", 1)
             query_type = mapper.registry.get(query_type_name)
 
@@ -110,37 +104,36 @@
         fields_to_remove = set()
         for type_ in filtered_mutation_types:
             while isinstance(type_, (GraphQLNonNull, GraphQLList)):
                 type_ = type_.of_type
             if isinstance(type_, GraphQLObjectType):
                 interface_fields = []
                 for interface in type_.interfaces:
-                    interface_fields += [
-                        key
-                        for key, field in interface.fields.items()
-                    ]
+                    interface_fields += [key for key, field in interface.fields.items()]
                 for key, field in type_.fields.items():
-                    if key not in interface_fields and \
-                            not isinstance(field, GraphQLMutableField) and \
-                            not has_mutable(field.type):
+                    if (
+                        key not in interface_fields
+                        and not isinstance(field, GraphQLMutableField)
+                        and not has_mutable(field.type)
+                    ):
                         fields_to_remove.add((type_, key))
 
         for type_, key in fields_to_remove:
             del type_.fields[key]
 
         return mutation
 
     @staticmethod
     def invalid(
         root_type,
         filters=None,
         meta=None,
         checked_types=None,
         invalid_types=None,
-        invalid_fields=None
+        invalid_fields=None,
     ):
         if not checked_types:
             checked_types = set()
 
         if not invalid_types:
             invalid_types = set()
 
@@ -156,24 +149,21 @@
             fields = root_type.fields
         except (AssertionError, GraphQLTypeMapError):
             invalid_types.add(root_type)
             return invalid_types, invalid_fields
 
         interfaces = []
 
-        if hasattr(root_type, 'interfaces'):
+        if hasattr(root_type, "interfaces"):
             interfaces = root_type.interfaces
 
         interface_fields = []
         for interface in interfaces:
             try:
-                interface_fields += [
-                    key
-                    for key, field in interface.fields.items()
-                ]
+                interface_fields += [key for key, field in interface.fields.items()]
             except (AssertionError, GraphQLTypeMapError):
                 invalid_types.add(interface)
 
         for key, field in fields.items():
             if key not in interface_fields:
                 type_ = field.type
 
@@ -185,27 +175,24 @@
                 field_meta = meta.get((root_type.name, field_name), {})
 
                 if filters:
                     for field_filter in filters:
                         if field_filter.filter_field(field_name, field_meta):
                             invalid_fields.add((root_type, key))
 
-                if isinstance(
-                    type_,
-                    (GraphQLInterfaceType, GraphQLObjectType)
-                ):
+                if isinstance(type_, (GraphQLInterfaceType, GraphQLObjectType)):
                     try:
                         assert type_.fields
                         sub_invalid = GraphQLSchemaReducer.invalid(
                             root_type=type_,
                             filters=filters,
                             meta=meta,
                             checked_types=checked_types,
                             invalid_types=invalid_types,
-                            invalid_fields=invalid_fields
+                            invalid_fields=invalid_fields,
                         )
 
                         invalid_types.update(sub_invalid[0])
                         invalid_fields.update(sub_invalid[1])
 
                     except (AssertionError, GraphQLTypeMapError):
                         invalid_types.add(type_)
```

### Comparing `graphql-api-1.3.0/graphql_api/relay.py` & `graphql-api-1.3.1/graphql_api/relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,16 @@
     def __init__(
         self,
         has_previous_page: bool,
         has_next_page: bool,
         start_cursor: str,
         end_cursor: str,
         *args,
-        **kwargs
+        **kwargs,
     ):
-
         super().__init__(*args, **kwargs)
 
         self._has_previous_page = has_previous_page
         self._has_next_page = has_next_page
         self._start_cursor = start_cursor
         self._end_cursor = end_cursor
 
@@ -108,28 +107,28 @@
     """
 
     def __init__(
         self,
         before: str = None,
         after: str = None,
         first: int = None,
-        last: int = None, *args, **kwargs
+        last: int = None,
+        *args,
+        **kwargs,
     ):
         self._before = before
         self._after = after
         self._first = first
         self._last = last
         super().__init__(*args, **kwargs)
 
     @GraphQLAPI.field
     def edges(self) -> List[Edge]:
         raise NotImplementedError(
-            f"{self.__class__.__name__} has not "
-            f"implemented 'Connection.edges'"
+            f"{self.__class__.__name__} has not " f"implemented 'Connection.edges'"
         )
 
     @GraphQLAPI.field
     def page_info(self) -> PageInfo:
         raise NotImplementedError(
-            f"{self.__class__.__name__} has not "
-            f"implemented 'Connection.page_info'"
+            f"{self.__class__.__name__} has not " f"implemented 'Connection.page_info'"
         )
```

### Comparing `graphql-api-1.3.0/graphql_api/remote.py` & `graphql-api-1.3.1/graphql_api/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,219 +15,194 @@
     GraphQLEnumType,
     GraphQLInterfaceType,
     GraphQLUnionType,
     GraphQLID,
     GraphQLString,
     GraphQLFloat,
     GraphQLBoolean,
-    GraphQLInt
+    GraphQLInt,
 )
 from graphql.execution import ExecutionResult
 from graphql.type.definition import (
     GraphQLField,
     GraphQLScalarType,
     GraphQLNonNull,
     GraphQLList,
     GraphQLType,
-    is_enum_type
+    is_enum_type,
 )
 
 from graphql_api.error import GraphQLError
 from graphql_api.executor import GraphQLBaseExecutor
 from graphql_api.mapper import GraphQLTypeMapper, GraphQLMetaKey
 from graphql_api.api import GraphQLAPI
 from graphql_api.types import serialize_bytes
-from graphql_api.utils import \
-    to_camel_case, \
-    url_to_ast, \
-    to_snake_case, \
-    http_query
+from graphql_api.utils import to_camel_case, url_to_ast, to_snake_case, http_query
 
 
 class GraphQLRemoteExecutor(GraphQLBaseExecutor, GraphQLObjectType):
-
     def __init__(
-            self,
-            url,
-            name="Remote",
-            description=None,
-            http_method="GET",
-            http_headers=None,
-            http_timeout=None,
-            verify=True,
-            ignore_unsupported=True
+        self,
+        url,
+        name="Remote",
+        description=None,
+        http_method="GET",
+        http_headers=None,
+        http_timeout=None,
+        verify=True,
+        ignore_unsupported=True,
     ):
-
         if not description:
-            description = f'The `{name}` object type forwards all ' \
-                          f'requests to the GraphQL executor at {url}'
+            description = (
+                f"The `{name}` object type forwards all "
+                f"requests to the GraphQL executor at {url}"
+            )
 
         if http_headers is None:
             http_headers = {}
 
         self.url = url
         self.http_method = http_method
         self.http_headers = http_headers
         self.http_timeout = http_timeout
         self.verify = verify
         self.ignore_unsupported = ignore_unsupported
 
-        super().__init__(name=name,
-                         fields=self.build_fields,
-                         description=description)
+        super().__init__(name=name, fields=self.build_fields, description=description)
 
     def build_fields(self):
         ast_schema = url_to_ast(
-            self.url,
-            http_method=self.http_method,
-            http_headers=self.http_headers
+            self.url, http_method=self.http_method, http_headers=self.http_headers
         )
 
         def resolver(info=None, context=None, *args, **kwargs):
             field_ = context.field_nodes[0]
             if field_.alias:
                 key_ = field_.alias.value
             else:
                 key_ = field_.name.value
 
             return info[key_]
 
         # noinspection PyProtectedMember
         for name, type in ast_schema.type_map.items():
-            if (isinstance(type, GraphQLObjectType) or
-                isinstance(type, GraphQLInputObjectType)) and \
-                    not type.name.startswith("__"):
+            if (
+                isinstance(type, GraphQLObjectType)
+                or isinstance(type, GraphQLInputObjectType)
+            ) and not type.name.startswith("__"):
                 for key, field in type.fields.items():
                     field.resolver = resolver
             elif isinstance(type, GraphQLEnumType):
                 if not self.ignore_unsupported:
                     raise GraphQLError(
                         f"GraphQLScalarType '{type}' type is not supported "
                         f"in a remote executor '{self.url}'."
                     )
             elif isinstance(type, (GraphQLInterfaceType, GraphQLUnionType)):
-
-                super_type = 'GraphQLInterface' \
-                    if isinstance(type, GraphQLInterfaceType) \
-                    else 'GraphQLUnionType'
+                super_type = (
+                    "GraphQLInterface"
+                    if isinstance(type, GraphQLInterfaceType)
+                    else "GraphQLUnionType"
+                )
 
                 if not self.ignore_unsupported:
                     raise GraphQLError(
                         f"{super_type} '{type}' type is not supported"
                         f" from remote executor '{self.url}'."
                     )
             elif isinstance(type, GraphQLScalarType):
                 if type not in [
                     GraphQLID,
                     GraphQLString,
                     GraphQLFloat,
                     GraphQLBoolean,
-                    GraphQLInt
+                    GraphQLInt,
                 ]:
                     if not self.ignore_unsupported:
                         raise GraphQLError(
                             f"GraphQLScalarType '{type}' type is not "
                             f"supported in a remote executor '{self.url}'."
                         )
-            elif str(type).startswith('__'):
+            elif str(type).startswith("__"):
                 continue
             else:
                 raise GraphQLError(
                     f"Unknown GraphQLType '{type}' type is not supported in "
                     f"a remote executor '{self.url}'."
                 )
 
         # noinspection PyProtectedMember
         return ast_schema.query_type.fields
 
     async def execute_async(
-            self,
-            query,
-            variable_values=None,
-            operation_name=None,
-            http_headers=None
+        self, query, variable_values=None, operation_name=None, http_headers=None
     ) -> ExecutionResult:
-
         if http_headers is None:
             http_headers = self.http_headers
         else:
             http_headers = {**self.http_headers, **http_headers}
 
         try:
             json_ = await http_query(
                 url=self.url,
                 query=query,
                 variable_values=variable_values,
                 operation_name=operation_name,
                 http_method=self.http_method,
                 http_headers=http_headers,
                 http_timeout=self.http_timeout,
-                verify=self.verify
+                verify=self.verify,
             )
         except RequestException as e:
             import sys
+
             err_msg = f"{e}, remote service '{self.name}' is unavailable."
             raise type(e)(err_msg).with_traceback(sys.exc_info()[2])
 
         except ValueError as e:
-            raise ValueError(
-                f"{e}, from remote service '{self.name}'."
-            )
+            raise ValueError(f"{e}, from remote service '{self.name}'.")
 
-        return ExecutionResult(
-            data=json_.get('data'),
-            errors=json_.get('errors')
-        )
+        return ExecutionResult(data=json_.get("data"), errors=json_.get("errors"))
 
     def execute(
-            self,
-            query,
-            variable_values=None,
-            operation_name=None,
-            http_headers=None
+        self, query, variable_values=None, operation_name=None, http_headers=None
     ) -> ExecutionResult:
-
         if http_headers is None:
             http_headers = self.http_headers
         else:
             http_headers = {**self.http_headers, **http_headers}
 
         try:
-            json_ = asyncio.run(http_query(
-                url=self.url,
-                query=query,
-                variable_values=variable_values,
-                operation_name=operation_name,
-                http_method=self.http_method,
-                http_headers=http_headers,
-                http_timeout=self.http_timeout,
-                verify=self.verify
-            ))
+            json_ = asyncio.run(
+                http_query(
+                    url=self.url,
+                    query=query,
+                    variable_values=variable_values,
+                    operation_name=operation_name,
+                    http_method=self.http_method,
+                    http_headers=http_headers,
+                    http_timeout=self.http_timeout,
+                    verify=self.verify,
+                )
+            )
         except RequestException as e:
             import sys
+
             err_msg = f"{e}, remote service '{self.name}' is unavailable."
             raise type(e)(err_msg).with_traceback(sys.exc_info()[2])
 
         except ValueError as e:
-            raise ValueError(
-                f"{e}, from remote service '{self.name}'."
-            )
+            raise ValueError(f"{e}, from remote service '{self.name}'.")
 
-        return ExecutionResult(
-            data=json_.get('data'),
-            errors=json_.get('errors')
-        )
+        return ExecutionResult(data=json_.get("data"), errors=json_.get("errors"))
 
 
 class GraphQLMappers:
-
     def __init__(
-            self,
-            query_mapper: GraphQLTypeMapper,
-            mutable_mapper: GraphQLTypeMapper
+        self, query_mapper: GraphQLTypeMapper, mutable_mapper: GraphQLTypeMapper
     ):
         self.query_mapper = query_mapper
         self.mutable_mapper = mutable_mapper
 
     def map(self, type, reverse=False):
         if reverse:
             query_type = self.query_mapper.rmap(type)
@@ -246,52 +221,46 @@
 
 
 class NullResponse(BaseException):
     pass
 
 
 class GraphQLRemoteError(GraphQLError):
-
     def __init__(self, query=None, result=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.query = query
         self.result = result
 
 
 class GraphQLAsyncStub:
-
     async def call_async(self, name, *args, **kwargs):
         pass
 
 
 class GraphQLRemoteObject:
-
     def get_labels(self) -> List[str]:
         return self.python_type.get_labels()
 
     @classmethod
     def from_url(
-            cls,
-            url: str,
-            api: GraphQLAPI,
-            http_method: str = "GET"
-    ) -> 'GraphQLRemoteObject':
+        cls, url: str, api: GraphQLAPI, http_method: str = "GET"
+    ) -> "GraphQLRemoteObject":
         executor = GraphQLRemoteExecutor(url=url, http_method=http_method)
 
         return GraphQLRemoteObject(executor=executor, api=api)
 
     # noinspection PyProtectedMember
     def __init__(
-            self,
-            executor: GraphQLBaseExecutor,
-            api: GraphQLAPI = None,
-            mappers: GraphQLMappers = None,
-            python_type: Type = None,
-            call_history: List[Tuple['GraphQLRemoteField', Dict]] = None,
-            delay_mapping: bool = True
+        self,
+        executor: GraphQLBaseExecutor,
+        api: GraphQLAPI = None,
+        mappers: GraphQLMappers = None,
+        python_type: Type = None,
+        call_history: List[Tuple["GraphQLRemoteField", Dict]] = None,
+        delay_mapping: bool = True,
     ):
         if not call_history:
             call_history = []
 
         if not api and python_type:
             api = GraphQLAPI(root=python_type)
 
@@ -317,40 +286,36 @@
     def _map(self, force=False):
         if self.mappers is None:
             api = self.api
 
             api.graphql_schema()
 
             self.mappers = GraphQLMappers(
-                query_mapper=api.query_mapper,
-                mutable_mapper=api.mutation_mapper
+                query_mapper=api.query_mapper, mutable_mapper=api.mutation_mapper
             )
 
         if not self.mapped_types:
             self.mapped_types = True
             graphql_types = self.mappers.map(self.python_type)
             self.graphql_query_type, self.graphql_mutable_type = graphql_types
 
-    def fetch(self, fields: List[Tuple['GraphQLRemoteField', Dict]] = None):
+    def fetch(self, fields: List[Tuple["GraphQLRemoteField", Dict]] = None):
         if fields is None:
             fields = self._fields()
 
         field_values = self._fetch(fields=fields)
 
         for field, args in fields:
             field_value = field_values.get(to_camel_case(field.name))
 
             arg_hash = self.hash(args)
 
             self.values[(field, arg_hash)] = field_value
 
-    async def fetch_async(
-            self,
-            fields: List[Tuple['GraphQLRemoteField', Dict]] = None
-    ):
+    async def fetch_async(self, fields: List[Tuple["GraphQLRemoteField", Dict]] = None):
         if fields is None:
             fields = self._fields()
 
         field_values = await self._fetch_async(fields=fields)
 
         for field, args in fields:
             field_value = field_values.get(to_camel_case(field.name))
@@ -376,132 +341,115 @@
             name
             for name, field in self.graphql_query_type.fields.items()
             if is_valid_field(field)
         ]
 
         return [(self.get_field(name), {}) for name in valid_fields]
 
-    def _fetch(self, fields: List[Tuple['GraphQLRemoteField', Dict]] = None):
+    def _fetch(self, fields: List[Tuple["GraphQLRemoteField", Dict]] = None):
         """
         Load all the scalar values for this object into the values dictionary
         :return:
         """
         if fields is None:
             fields = self._fields()
 
         query = self._fetch_build_query(fields=fields)
 
         result = self.executor.execute(query=query)
 
         return self._fetch_process(query, result, fields)
 
     async def _fetch_async(
-            self,
-            fields: List[Tuple['GraphQLRemoteField', Dict]] = None
+        self, fields: List[Tuple["GraphQLRemoteField", Dict]] = None
     ):
         """
         Load all the scalar values for this object into the values dictionary
         :return:
         """
         if fields is None:
             fields = self._fields()
 
         query = self._fetch_build_query(fields=fields)
 
         result = await self.executor.execute_async(query=query)
 
         return self._fetch_process(query, result, fields)
 
-    def _fetch_build_query(
-            self,
-            fields: List[Tuple['GraphQLRemoteField', Dict]]
-    ):
+    def _fetch_build_query(self, fields: List[Tuple["GraphQLRemoteField", Dict]]):
         self._map()
 
-        mutable = any([
-            field.mutable
-            for field, args in self.call_history + fields])
+        mutable = any([field.mutable for field, args in self.call_history + fields])
 
         query_builder = GraphQLRemoteQueryBuilder(
             call_stack=self.call_history,
             fields=fields,
             mappers=self.mappers,
-            mutable=mutable
+            mutable=mutable,
         )
 
         return query_builder.build()
 
     def _fetch_process(
-            self,
-            query,
-            result: ExecutionResult,
-            fields: List[Tuple['GraphQLRemoteField', Dict]]
+        self,
+        query,
+        result: ExecutionResult,
+        fields: List[Tuple["GraphQLRemoteField", Dict]],
     ):
-
         if result.errors:
             raise GraphQLRemoteError(
-                query=query,
-                result=result,
-                message=result.errors[0]["message"]
+                query=query, result=result, message=result.errors[0]["message"]
             )
 
         field_values = result.data
         for field, args in self.call_history:
             camel_name = to_camel_case(field.name)
 
             if isinstance(field_values, list):
-                raise ValueError(
-                    "GraphQLLists can only contain scalar values."
-                )
+                raise ValueError("GraphQLLists can only contain scalar values.")
 
             if field_values is None:
                 raise NullResponse()
 
             field_values = field_values.get(camel_name)
 
         if field_values is None:
             raise NullResponse()
 
         def parse_field(key, value):
-
             field: GraphQLRemoteField = None
 
             for _field, _field_dict in fields:
                 if _field.name == key:
                     field = _field
                     break
 
             if not field:
-                raise KeyError(
-                    f"Could not find field for key {key}"
-                )
+                raise KeyError(f"Could not find field for key {key}")
 
             field_type = field.graphql_type()
 
             if value is None:
                 if not field.nullable:
                     raise TypeError(
                         f"Unable to parse None type for non nullable field, "
                         f"'{key}'. Expected type: {field_type}"
                     )
                 return None
 
             if not is_scalar(field_type):
-                raise TypeError(
-                    f"Unable to parse non-scalar type {field_type}"
-                )
+                raise TypeError(f"Unable to parse non-scalar type {field_type}")
 
             def _to_value(value):
                 ast_value = to_ast_value(value, field_type)
 
-                if hasattr(field_type, 'parse_literal'):
+                if hasattr(field_type, "parse_literal"):
                     value = field_type.parse_literal(ast_value)
 
-                    if is_enum_type(field_type) and \
-                            hasattr(field_type, 'enum_type'):
+                    if is_enum_type(field_type) and hasattr(field_type, "enum_type"):
                         enum_type = field_type.enum_type
                         value = enum_type(value)
 
                     return value
 
             if field.list:
                 values = []
@@ -517,57 +465,55 @@
                     key: parse_field(key, value)
                     for key, value in field_values_list_item.items()
                 }
                 for field_values_list_item in field_values
             ]
         else:
             field_values = {
-                key: parse_field(key, value)
-                for key, value in field_values.items()
+                key: parse_field(key, value) for key, value in field_values.items()
             }
 
         return field_values
 
     def hash(self, args: Dict):
         hashable_args = {}
 
         for key, value in args.items():
-
             if isinstance(value, list):
                 value = tuple(value)
 
             hashable_args[key] = value
 
         return hash(frozenset(hashable_args.items()))
 
-    def _get_value_cached(self, field: 'GraphQLRemoteField', args: Dict):
+    def _get_value_cached(self, field: "GraphQLRemoteField", args: Dict):
         try:
             arg_hash = self.hash(args)
         except TypeError:
             arg_hash = hash(uuid.uuid4())
 
         if field.mutable:
             self.values.clear()
 
-        for ((_field, _arg_hash), value) in self.values.items():
+        for (_field, _arg_hash), value in self.values.items():
             if field.name == _field.name and arg_hash == _arg_hash:
                 return value, True, arg_hash
 
         return None, False, arg_hash
 
     def _get_value_check_mutated(self, field):
         mutated = any([field.mutable for field, args in self.call_history])
 
         if mutated and (field.scalar or field.mutable or field.nullable):
             raise GraphQLError(
                 f"Cannot fetch {field.name} from {self.python_type}, "
                 f"mutated objects cannot be re-fetched."
             )
 
-    async def get_value_async(self, field: 'GraphQLRemoteField', args: Dict):
+    async def get_value_async(self, field: "GraphQLRemoteField", args: Dict):
         self._map()
         value, result, arg_hash = self._get_value_cached(field, args)
 
         if result:
             return value
 
         if (field, arg_hash) in self.values.keys():
@@ -576,45 +522,40 @@
         self._get_value_check_mutated(field)
 
         if field.scalar:
             await self.fetch_async(fields=[(field, args)])
             return self.values.get((field, arg_hash), None)
 
         else:
-            python_type = self.mappers.map(
-                field.graphql_field.type,
-                reverse=True
-            )
+            python_type = self.mappers.map(field.graphql_field.type, reverse=True)
 
             obj = GraphQLRemoteObject(
                 executor=self.executor,
                 api=self.api,
                 python_type=python_type,
                 mappers=self.mappers,
-                call_history=[*self.call_history, (field, args)]
+                call_history=[*self.call_history, (field, args)],
             )
 
             if field.list:
                 data = await obj._fetch_async()
                 fields = obj._fields()
                 remote_objects = []
 
                 for remote_object_data in data:
                     remote_object = GraphQLRemoteObject(
                         executor=self.executor,
                         api=self.api,
                         python_type=python_type,
                         mappers=self.mappers,
-                        call_history=[*self.call_history, (field, args)]
+                        call_history=[*self.call_history, (field, args)],
                     )
 
                     for field, args in fields:
-                        field_value = remote_object_data.get(
-                            to_camel_case(field.name)
-                        )
+                        field_value = remote_object_data.get(to_camel_case(field.name))
                         arg_hash = self.hash(args)
                         field_key = (field, arg_hash)
                         remote_object.values[field_key] = field_value
 
                     remote_objects.append(remote_object)
                 return remote_objects
 
@@ -626,23 +567,25 @@
                         return None
 
                 if field.mutable:
                     meta = self.mappers.mutable_mapper.meta.get(
                         (self.graphql_mutable_type.name, field.name)
                     )
 
-                    if field.recursive and \
-                            meta and \
-                            meta.get(GraphQLMetaKey.resolve_to_self, True):
+                    if (
+                        field.recursive
+                        and meta
+                        and meta.get(GraphQLMetaKey.resolve_to_self, True)
+                    ):
                         self.values.update(obj.values)
                         return self
 
                 return obj
 
-    def get_value(self, field: 'GraphQLRemoteField', args: Dict):
+    def get_value(self, field: "GraphQLRemoteField", args: Dict):
         self._map()
         value, result, arg_hash = self._get_value_cached(field, args)
 
         if result:
             return value
 
         if (field, arg_hash) in self.values.keys():
@@ -651,45 +594,40 @@
         self._get_value_check_mutated(field)
 
         if field.scalar:
             self.fetch(fields=[(field, args)])
             return self.values.get((field, arg_hash), None)
 
         else:
-            python_type = self.mappers.map(
-                field.graphql_field.type,
-                reverse=True
-            )
+            python_type = self.mappers.map(field.graphql_field.type, reverse=True)
 
             obj = GraphQLRemoteObject(
                 executor=self.executor,
                 api=self.api,
                 python_type=python_type,
                 mappers=self.mappers,
-                call_history=[*self.call_history, (field, args)]
+                call_history=[*self.call_history, (field, args)],
             )
 
             if field.list:
                 data = obj._fetch()
                 fields = obj._fields()
                 remote_objects = []
 
                 for remote_object_data in data:
                     remote_object = GraphQLRemoteObject(
                         executor=self.executor,
                         api=self.api,
                         python_type=python_type,
                         mappers=self.mappers,
-                        call_history=[*self.call_history, (field, args)]
+                        call_history=[*self.call_history, (field, args)],
                     )
 
                     for field, args in fields:
-                        field_value = remote_object_data.get(
-                            to_camel_case(field.name)
-                        )
+                        field_value = remote_object_data.get(to_camel_case(field.name))
                         arg_hash = self.hash(args)
                         field_key = (field, arg_hash)
                         remote_object.values[field_key] = field_value
 
                     remote_objects.append(remote_object)
                 return remote_objects
 
@@ -701,17 +639,19 @@
                         return None
 
                 if field.mutable:
                     meta = self.mappers.mutable_mapper.meta.get(
                         (self.graphql_mutable_type.name, field.name)
                     )
 
-                    if field.recursive and \
-                            meta and \
-                            meta.get(GraphQLMetaKey.resolve_to_self, True):
+                    if (
+                        field.recursive
+                        and meta
+                        and meta.get(GraphQLMetaKey.resolve_to_self, True)
+                    ):
                         self.values.update(obj.values)
                         return self
 
                 return obj
 
     def get_field(self, name):
         self._map()
@@ -732,23 +672,20 @@
             except AssertionError:
                 pass
 
         if not field:
             raise GraphQLError(f"Field {name} on {self} does not exist")
 
         return GraphQLRemoteField(
-            name=camel_name,
-            mutable=mutable,
-            graphql_field=field,
-            parent=self
+            name=camel_name, mutable=mutable, graphql_field=field, parent=self
         )
 
     def __getattr__(self, name):
         if name == "__await__":
-            raise AttributeError('Not Awaitable')
+            raise AttributeError("Not Awaitable")
 
         field, auto_call = self.getattr(name)
 
         if auto_call:
             return field()
 
         return field
@@ -766,18 +703,15 @@
 
         try:
             # noinspection PyUnresolvedReferences
             from dataclasses import fields, is_dataclass
 
             if is_dataclass(self.python_type):
                 # noinspection PyDataclass
-                field_names = [
-                    field.name
-                    for field in fields(self.python_type)
-                ]
+                field_names = [field.name for field in fields(self.python_type)]
 
                 is_dataclass_field = name in field_names
 
         except ImportError:
             pass
 
         is_property = isinstance(attribute_type, property)
@@ -785,14 +719,15 @@
 
         auto_call = is_dataclass_field or is_property
 
         if not auto_call:
             try:
                 # noinspection PyPackageRequirements
                 from sqlalchemy.orm.attributes import InstrumentedAttribute
+
                 auto_call = isinstance(attribute_type, InstrumentedAttribute)
             except ImportError:
                 pass
 
         try:
             field = self.get_field(name)
 
@@ -800,67 +735,60 @@
             if not pass_through:
                 raise err
 
             if "does not exist" in err.message:
                 if is_callable:
                     func = getattr(self.python_type, name)
                     _is_method = inspect.ismethod(func)
-                    _is_static_method = is_static_method(
-                        self.python_type,
-                        name
-                    )
+                    _is_static_method = is_static_method(self.python_type, name)
 
                     if _is_method or _is_static_method:
                         return func, False
                     else:
-                        return (lambda *args, **kwargs: func(
-                            self,
-                            *args, **kwargs
-                        )), False
+                        return (
+                            lambda *args, **kwargs: func(self, *args, **kwargs)
+                        ), False
 
                 if is_property:
                     prop = getattr(self.python_type, name)
                     return prop.fget(self), False
             raise
 
         return field, auto_call
 
     def __str__(self):
         self._map()
 
-        return f"<RemoteObject({self.graphql_query_type.name}) " \
-               f"at {hex(id(self))}>"
+        return f"<RemoteObject({self.graphql_query_type.name}) " f"at {hex(id(self))}>"
 
 
 class GraphQLRemoteField:
-
     # noinspection PyProtectedMember
     def __init__(
-            self,
-            name: str,
-            mutable: bool,
-            graphql_field: GraphQLField,
-            parent: GraphQLRemoteObject
+        self,
+        name: str,
+        mutable: bool,
+        graphql_field: GraphQLField,
+        parent: GraphQLRemoteObject,
     ):
         self.name = name
         self.mutable = mutable
         self.graphql_field = graphql_field
         self.parent = parent
         self.nullable = is_nullable(self.graphql_field.type)
         self.scalar = is_scalar(self.graphql_field.type)
         self.list = is_list(self.graphql_field.type)
 
         self.recursive = self.parent.python_type == self.parent.mappers.map(
-            self.graphql_field.type,
-            reverse=True
+            self.graphql_field.type, reverse=True
         )
 
     def graphql_type(self) -> GraphQLType:
         graphql_type = self.graphql_field.type
-        while hasattr(graphql_type, 'of_type'):
+        while hasattr(graphql_type, "of_type"):
             graphql_type = graphql_type.of_type
 
         return graphql_type
 
     def remap_args_to_kwargs(self, args, kwargs):
         arg_names = list(self.graphql_field.args.keys())
         arg_names_count = len(arg_names)
@@ -893,120 +821,109 @@
     def __eq__(self, other):
         if isinstance(other, GraphQLRemoteField):
             if other.parent == self.parent and other.name == self.name:
                 return True
 
 
 class GraphQLRemoteQueryBuilder:
-
     def __init__(
-            self,
-            call_stack: List[Tuple['GraphQLRemoteField', Dict]],
-            fields: List[Tuple['GraphQLRemoteField', Dict]],
-            mappers: GraphQLMappers,
-            mutable=False
+        self,
+        call_stack: List[Tuple["GraphQLRemoteField", Dict]],
+        fields: List[Tuple["GraphQLRemoteField", Dict]],
+        mappers: GraphQLMappers,
+        mutable=False,
     ):
         self.call_stack = call_stack
         self.fields = fields
         self.mappers = mappers
         self.mutable = mutable
 
     def build(self):
         if self.mutable:
-            query = 'mutation'
+            query = "mutation"
         else:
-            query = 'query'
+            query = "query"
 
         def to_field_call(field, args=None):
             name = field.name
             field_call = to_camel_case(name)
             if args:
                 values = []
                 for key, value in args.items():
                     camel_key = to_camel_case(key)
                     graphql_arg = field.graphql_field.args[camel_key]
                     graphql_type = graphql_arg.type
 
                     str_value = self.map_to_input_value(
                         value=value,
                         expected_graphql_type=graphql_type,
-                        mappers=self.mappers
+                        mappers=self.mappers,
                     )
 
                     if str_value is not None:
                         values.append(f"{camel_key}:{str_value}")
 
                 field_call += f"({','.join(values)})"
             return field_call
 
         for field, args in self.call_stack:
             query += "{" + to_field_call(field, args=args)
 
-        field_calls = [
-            to_field_call(field, args=args)
-            for field, args in self.fields
-        ]
+        field_calls = [to_field_call(field, args=args) for field, args in self.fields]
 
         query += "{" + ",".join(field_calls) + "}"
         query += "}" * len(self.call_stack)
 
         return query
 
     # noinspection PyMethodMayBeStatic
     def map_to_input_value(
-            self,
-            value,
-            mappers: GraphQLMappers,
-            expected_graphql_type=None
+        self, value, mappers: GraphQLMappers, expected_graphql_type=None
     ):
         from graphql_api.mapper import is_scalar
 
         if value is None:
             return None
 
         python_type = type(value)
 
         if is_scalar(python_type):
             if isinstance(value, (list, set)):
                 values = [
                     self.map_to_input_value(
                         item,
                         mappers=mappers,
-                        expected_graphql_type=expected_graphql_type
+                        expected_graphql_type=expected_graphql_type,
                     )
                     for item in value
                 ]
-                return '[' + ','.join(values) + ']'
+                return "[" + ",".join(values) + "]"
 
             if isinstance(value, str):
                 return json.dumps(value)
             if isinstance(value, bool):
-                return 'true' if value else 'false'
+                return "true" if value else "false"
             if isinstance(value, (float, int)):
                 return str(value)
             if isinstance(value, bytes):
                 return '"' + serialize_bytes(value) + '"'
             else:
                 return '"' + str(value) + '"'
 
         if isinstance(value, enum.Enum):
             return str(value.value)
 
         if isinstance(value, object):
-
             if expected_graphql_type is not None:
-
-                while hasattr(expected_graphql_type, 'of_type'):
+                while hasattr(expected_graphql_type, "of_type"):
                     expected_graphql_type = expected_graphql_type.of_type
 
                 graphql_type = expected_graphql_type
             else:
-                graphql_type = mappers.query_mapper.input_type_mapper.map(
-                    type(value)
-                )
+                graphql_type = mappers.query_mapper.input_type_mapper.map(type(value))
 
             input_dict = {}
 
             for key, field in graphql_type.fields.items():
                 try:
                     raw_input_value = getattr(value, to_snake_case(key))
 
@@ -1018,26 +935,20 @@
                         raise GraphQLError(
                             f"InputObject error, '{type(value)}' object has"
                             f" no attribute {to_snake_case(key)}, nested"
                             f" inputs must have matching attribute "
                             f"to field names"
                         )
                 else:
-                    _value = self.map_to_input_value(
-                        raw_input_value,
-                        mappers=mappers
-                    )
+                    _value = self.map_to_input_value(raw_input_value, mappers=mappers)
 
                     if _value is not None:
                         input_dict[key] = _value
 
-            input_values = [
-                f"{key}:{value}"
-                for key, value in input_dict.items()
-            ]
+            input_values = [f"{key}:{value}" for key, value in input_dict.items()]
 
             input_value = "{" + ",".join(input_values) + "}"
 
             return input_value
 
 
 def remote_execute(executor: GraphQLBaseExecutor, context):
@@ -1050,37 +961,37 @@
     if result.errors:
         raise GraphQLError(str(result.errors))
 
     return result.data
 
 
 def is_list(graphql_type):
-    while hasattr(graphql_type, 'of_type'):
+    while hasattr(graphql_type, "of_type"):
         if isinstance(graphql_type, GraphQLList):
             return True
         graphql_type = graphql_type.of_type
 
     return False
 
 
 def is_scalar(graphql_type):
-    while hasattr(graphql_type, 'of_type'):
+    while hasattr(graphql_type, "of_type"):
         graphql_type = graphql_type.of_type
 
     if isinstance(graphql_type, GraphQLScalarType):
         return True
 
     if isinstance(graphql_type, GraphQLEnumType):
         return True
 
     return False
 
 
 def is_nullable(graphql_type):
-    while hasattr(graphql_type, 'of_type'):
+    while hasattr(graphql_type, "of_type"):
         if isinstance(graphql_type, GraphQLNonNull):
             return False
         graphql_type = graphql_type.of_type
 
     return True
 
 
@@ -1103,15 +1014,15 @@
     if value is None:
         return None
 
     type_map = {
         (bool,): ast.BooleanValueNode,
         (str,): ast.StringValueNode,
         (float,): ast.FloatValueNode,
-        (int,): ast.IntValueNode
+        (int,): ast.IntValueNode,
     }
     ast_type = None
     ast_value = None
 
     for types, ast_type in type_map.items():
         if isinstance(value, types):
             ast_value = ast_type(value=value)
```

### Comparing `graphql-api-1.3.0/graphql_api/types.py` & `graphql-api-1.3.1/graphql_api/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 import binascii
 import datetime
 import json
 import uuid
 from typing import Dict, Union, List
 
-from graphql import GraphQLScalarType, StringValueNode, Undefined, \
-    GraphQLEnumType
+from graphql import GraphQLScalarType, StringValueNode, Undefined, GraphQLEnumType
 from graphql.language import ast
 
 
 class GraphQLMappedEnumType(GraphQLEnumType):
-
     def parse_literal(self, *args, **kwargs):
         result = super().parse_literal(*args, **kwargs)
 
-        return self.enum_type(result) \
-            if hasattr(self, 'enum_type') else result
+        return self.enum_type(result) if hasattr(self, "enum_type") else result
 
 
 def parse_uuid_literal(ast):
     if isinstance(ast, StringValueNode):
         try:
             return uuid.UUID(ast.value)
         except ValueError:
             return Undefined
 
 
 GraphQLUUID = GraphQLScalarType(
-    name='UUID',
-    description='The `UUID` scalar type represents a unique identifer.',
+    name="UUID",
+    description="The `UUID` scalar type represents a unique identifer.",
     serialize=str,
     parse_value=str,
-    parse_literal=parse_uuid_literal)
+    parse_literal=parse_uuid_literal,
+)
 
 
 def serialize_datetime(dt):
     return dt.isoformat(sep=" ")
 
 
 def parse_datetime_value(value):
-    datetime_formats = [
-        "%Y-%m-%d %H:%M:%S.%f",
-        "%Y-%m-%dT%H:%M:%S.%f"
-    ]
+    datetime_formats = ["%Y-%m-%d %H:%M:%S.%f", "%Y-%m-%dT%H:%M:%S.%f"]
 
     for datetime_format in datetime_formats:
         try:
             return datetime.datetime.strptime(value, datetime_format)
         except ValueError:
             pass
 
-    raise ValueError(f"Datetime {value} did not fit any "
-                     f"of the formats {datetime_formats}.")
+    raise ValueError(
+        f"Datetime {value} did not fit any " f"of the formats {datetime_formats}."
+    )
 
 
 def parse_datetime_literal(node):
     if isinstance(node, StringValueNode):
         return parse_datetime_value(node.value)
 
 
 GraphQLDateTime = GraphQLScalarType(
-    name='DateTime',
-    description='The `DateTime` scalar type represents a datetime, '
-                'the datetime should be in the format `2018-01-22 17:46:32`',
+    name="DateTime",
+    description="The `DateTime` scalar type represents a datetime, "
+    "the datetime should be in the format `2018-01-22 17:46:32`",
     serialize=serialize_datetime,
     parse_value=parse_datetime_value,
-    parse_literal=parse_datetime_literal)
+    parse_literal=parse_datetime_literal,
+)
 
 
 JsonType = Union[None, int, float, str, bool, List, Dict]
 
 
 def serialize_json(data: JsonType) -> str:
     return json.dumps(data)
@@ -85,44 +82,44 @@
     if isinstance(node, ast.BooleanValueNode):
         return node.value
     if isinstance(node, ast.FloatValueNode):
         return node.value
 
 
 GraphQLJSON = GraphQLScalarType(
-    name='JSON',
-    description='The `JSON` scalar type represents JSON values as specified by'
-                ' [ECMA-404](http://www.ecma-international.org/'
-                'publications/files/ECMA-ST/ECMA-404.pdf).',
+    name="JSON",
+    description="The `JSON` scalar type represents JSON values as specified by"
+    " [ECMA-404](http://www.ecma-international.org/"
+    "publications/files/ECMA-ST/ECMA-404.pdf).",
     serialize=serialize_json,
     parse_value=parse_json_value,
-    parse_literal=parse_json_literal)
+    parse_literal=parse_json_literal,
+)
 
 
 def serialize_bytes(bytes: bytes) -> str:
     try:
-        data = bytes.decode('utf-8')
+        data = bytes.decode("utf-8")
     except (binascii.Error, UnicodeDecodeError, Exception):
-        data = "UTF-8 ENCODED PREVIEW: " + \
-               bytes.decode('utf-8', errors="ignore")
+        data = "UTF-8 ENCODED PREVIEW: " + bytes.decode("utf-8", errors="ignore")
     return data
 
 
 def parse_bytes_value(value: str) -> bytes:
-    data = bytes(value, 'utf-8')
+    data = bytes(value, "utf-8")
     return data
 
 
 def parse_bytes_literal(node):
     if isinstance(node, ast.StringValueNode):
         return parse_bytes_value(node.value)
 
 
 GraphQLBytes = GraphQLScalarType(
-    name='Bytes',
-    description='The `Bytes` scalar type expects and returns a '
-                'Byte array in UTF-8 string format that represents the Bytes. '
-                'If the data is not UTF-encodable the erros will be ignored',
+    name="Bytes",
+    description="The `Bytes` scalar type expects and returns a "
+    "Byte array in UTF-8 string format that represents the Bytes. "
+    "If the data is not UTF-encodable the erros will be ignored",
     serialize=serialize_bytes,
     parse_value=parse_bytes_value,
-    parse_literal=parse_bytes_literal
+    parse_literal=parse_bytes_literal,
 )
```

### Comparing `graphql-api-1.3.0/graphql_api/utils.py` & `graphql-api-1.3.1/graphql_api/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,92 +9,88 @@
 from graphql import (
     GraphQLNonNull,
     GraphQLList,
     GraphQLObjectType,
     GraphQLSchema,
     GraphQLError,
     build_client_schema,
-    get_introspection_query)
+    get_introspection_query,
+)
 
 from graphql.type.definition import GraphQLType, GraphQLInterfaceType
 
 
 # From this response in Stackoverflow
 # http://stackoverflow.com/a/19053800/1072990
 def to_camel_case(snake_str, title=False):
-    if snake_str.startswith('_'):
+    if snake_str.startswith("_"):
         snake_str = snake_str[1:]
 
-    components = snake_str.split('_')
+    components = snake_str.split("_")
     # We capitalize the first letter of each component except the first one
     # with the 'title' method and join them together.
     if not snake_str:
         return ""
     prefix = components[0].title() if title else components[0]
-    value = prefix + "".join(x.title() if x else '_' for x in components[1:])
+    value = prefix + "".join(x.title() if x else "_" for x in components[1:])
     return value
 
 
 # From this response in Stackoverflow
 # http://stackoverflow.com/a/1176023/1072990
 def to_snake_case(name):
-    s1 = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
-    return re.sub('([a-z0-9])([A-Z])', r'\1_\2', s1).lower()
+    s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
+    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
 
 def to_input_value(value):
     from graphql_api.mapper import is_scalar
 
     if value is None:
         return None
 
     python_type = type(value)
 
     if is_scalar(python_type):
         if isinstance(value, str):
             return '"' + value + '"'
         if isinstance(value, bool):
-            return 'true' if value else 'false'
+            return "true" if value else "false"
         else:
             return str(value)
 
     if isinstance(value, enum.Enum):
         return str(value.value)
 
-    raise ValueError(f'Cannot map {value} to GraphQLInput')
+    raise ValueError(f"Cannot map {value} to GraphQLInput")
 
 
 def has_mutable(type, checked_types=None, interfaces_default_mutable=True):
     from .mapper import GraphQLMutableField, GraphQLTypeMapError
 
     while isinstance(type, (GraphQLNonNull, GraphQLList)):
         type = type.of_type
 
     if isinstance(type, (GraphQLObjectType, GraphQLInterfaceType)):
-        if interfaces_default_mutable and \
-                isinstance(type, GraphQLInterfaceType):
+        if interfaces_default_mutable and isinstance(type, GraphQLInterfaceType):
             return True
 
         if not checked_types:
             checked_types = set()
         try:
             fields = type.fields
         except (AssertionError, GraphQLTypeMapError):
             return False
 
         for key, field in fields.items():
             if isinstance(field, GraphQLMutableField):
                 return True
             if field.type not in checked_types:
                 checked_types.add(field.type)
-                if has_mutable(
-                    field.type,
-                    checked_types,
-                    interfaces_default_mutable
-                ):
+                if has_mutable(field.type, checked_types, interfaces_default_mutable):
                     return True
 
     return False
 
 
 def iterate_fields(type: GraphQLType, done_fields=None):
     from .mapper import GraphQLTypeMapError
@@ -115,37 +111,32 @@
                 field_id = type.name + "." + key
                 if field_id not in done_fields:
                     done_fields.add(field_id)
                     yield type, key, field
                     yield from iterate_fields(field.type, done_fields)
 
 
-def url_to_ast(
-    url,
-    http_method="GET",
-    http_headers=None,
-    verify=True
-) -> GraphQLSchema:
+def url_to_ast(url, http_method="GET", http_headers=None, verify=True) -> GraphQLSchema:
     _introspect_query = get_introspection_query()
 
     response = asyncio.run(
         http_query(
             url=url,
             query=_introspect_query,
             http_method=http_method,
             http_headers=http_headers,
-            verify=verify
+            verify=verify,
         )
     )
-    errors = response.get('errors')
+    errors = response.get("errors")
 
     if errors:
         raise GraphQLError(f"RemoteSchema {url} Error: {str(errors)}")
 
-    introspect_schema = response.get('data')
+    introspect_schema = response.get("data")
     return build_client_schema(introspect_schema)
 
 
 def executor_to_ast(executor) -> GraphQLSchema:
     _introspect_query = get_introspection_query()
     response = executor.execute(_introspect_query)
     introspect_schema = response.data
@@ -157,15 +148,15 @@
     url,
     query,
     variable_values=None,
     operation_name=None,
     http_method="GET",
     http_headers=None,
     http_timeout=10,
-    verify=True
+    verify=True,
 ):
     params = {"query": query}
 
     if http_headers is None:
         http_headers = {}
 
     if variable_values:
@@ -176,31 +167,33 @@
 
     async with aiohttp.ClientSession() as session:
         if http_method == "GET":
             r = await session.get(
                 url,
                 params=params,
                 ssl=verify,
-                headers={'Accept': 'application/json', **http_headers},
-                timeout=ClientTimeout(total=http_timeout)
+                headers={"Accept": "application/json", **http_headers},
+                timeout=ClientTimeout(total=http_timeout),
             )
 
         elif http_method == "POST":
             r = await session.post(
                 url,
                 json=params,
                 ssl=verify,
-                headers={'Accept': 'application/json', **http_headers},
-                timeout=ClientTimeout(total=http_timeout)
+                headers={
+                    "Accept": "application/json",
+                    "Content-Type": "application/json",
+                    **http_headers,
+                },
+                timeout=ClientTimeout(total=http_timeout),
             )
 
         else:
             raise AttributeError(f"Invalid HTTP method {http_method}")
 
         try:
             json = await r.json(content_type=None)
         except JSONDecodeError as e:
-            raise ValueError(
-                f"{e}, unable to decode JSON"
-            )
+            raise ValueError(f"{e}, unable to decode JSON")
 
     return json
```

### Comparing `graphql-api-1.3.0/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.1/graphql_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.0
+Version: 1.3.1
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.0/graphql-api-v1.3.0.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.1/graphql-api-v1.3.1.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,15 @@
 Framework for building a GraphQL API with Python
 
 [![coverage report](https://gitlab.com/parob/graphql-api/badges/master/coverage.svg)](https://gitlab.com/parob/graphql-api/commits/master)
 
 [![pipeline status](https://gitlab.com/parob/graphql-api/badges/master/pipeline.svg)](https://gitlab.com/parob/graphql-api/commits/master)
 
 
+
 ## Installation
 
 ##### Pip
 ```
 pip install graphql-api
 ```
```

### Comparing `graphql-api-1.3.0/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.1/graphql_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.0/tests/test_custom_types.py` & `graphql-api-1.3.1/tests/test_custom_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,53 +3,47 @@
 from uuid import UUID
 
 from graphql_api.api import GraphQLAPI
 from graphql_api.types import JsonType
 
 
 class TestCustomTypes:
-
     def test_uuid_type(self):
         api = GraphQLAPI()
 
         user_id = uuid.uuid4()
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def name(self, id: UUID) -> str:
                 assert isinstance(id, UUID)
                 assert id == user_id
                 return "rob"
 
             @api.field
             def id(self) -> UUID:
                 return user_id
 
         executor = api.executor()
 
-        test_name_query = f"query GetName {{ name(id: \"{user_id}\") }}"
+        test_name_query = f'query GetName {{ name(id: "{user_id}") }}'
 
         result = executor.execute(test_name_query)
 
-        expected = {
-            "name": "rob"
-        }
+        expected = {"name": "rob"}
         assert not result.errors
         assert result.data == expected
 
         test_id_query = "query GetId { id }"
 
         result = executor.execute(test_id_query)
 
-        expected = {
-            "id": str(user_id)
-        }
+        expected = {"id": str(user_id)}
 
         assert not result.errors
         assert result.data == expected
 
         test_invalid_name_query = 'query GetName { name(id: "INVALID_UUID") }'
 
         result = executor.execute(test_invalid_name_query)
@@ -59,132 +53,125 @@
     def test_datetime_type(self):
         api = GraphQLAPI()
 
         now = datetime.now()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def add_one_hour(self, time: datetime) -> datetime:
                 return time + timedelta(hours=1)
 
         executor = api.executor()
 
-        test_time_query = f"query GetTimeInOneHour {{ addOneHour(time: \"{now}\") }}"
+        test_time_query = f'query GetTimeInOneHour {{ addOneHour(time: "{now}") }}'
 
         result = executor.execute(test_time_query)
 
-        expected = {
-            "addOneHour": str(now + timedelta(hours=1))
-        }
+        expected = {"addOneHour": str(now + timedelta(hours=1))}
         assert not result.errors
         assert result.data == expected
 
     def test_json_type(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def adapt_profile(self, profile: dict) -> dict:
                 return {**profile, "location": "london"}
 
             @api.field
             def add_number(self, numbers: list) -> list:
                 return [*numbers, 5]
 
             @api.field
             def send_json(self, json: JsonType) -> str:
                 return str(type(json)) + str(json)
 
         executor = api.executor()
 
-        test_profile_query = r'query GetAdaptProfile {' \
-                             r'     adaptProfile(profile: ' \
-                             r'     "{ \"name\": \"rob\", \"age\": 26 }") ' \
-                             r'}'
+        test_profile_query = (
+            r"query GetAdaptProfile {"
+            r"     adaptProfile(profile: "
+            r'     "{ \"name\": \"rob\", \"age\": 26 }") '
+            r"}"
+        )
 
         result = executor.execute(test_profile_query)
 
-        expected = {
-            "adaptProfile": '{"name": "rob", "age": 26, "location": "london"}'
-        }
+        expected = {"adaptProfile": '{"name": "rob", "age": 26, "location": "london"}'}
         assert not result.errors
         assert result.data == expected
 
-        test_number_query = r'query GetAddNumber {' \
-                            r'     addNumber(numbers: "[1, 2, 3, 4]") ' \
-                            r'}'
+        test_number_query = (
+            r"query GetAddNumber {" r'     addNumber(numbers: "[1, 2, 3, 4]") ' r"}"
+        )
 
         result = executor.execute(test_number_query)
 
-        expected = {
-            "addNumber": '[1, 2, 3, 4, 5]'
-        }
+        expected = {"addNumber": "[1, 2, 3, 4, 5]"}
         assert not result.errors
         assert result.data == expected
 
-        test_json_query = 'query SendJson {' \
-                          '     a: sendJson(json: "1") ' \
-                          '     b: sendJson(json: true) ' \
-                          '     c: sendJson(json: "true") ' \
-                          '     d: sendJson(json: "\\"test\\"") ' \
-                          '     e: sendJson(json: "{ \\"a\\": 1 }") ' \
-                          '     f: sendJson(json: "[ 1, 2, 3 ]") ' \
-                          '     g: sendJson(json: "1.01") ' \
-                          '}'
+        test_json_query = (
+            "query SendJson {"
+            '     a: sendJson(json: "1") '
+            "     b: sendJson(json: true) "
+            '     c: sendJson(json: "true") '
+            '     d: sendJson(json: "\\"test\\"") '
+            '     e: sendJson(json: "{ \\"a\\": 1 }") '
+            '     f: sendJson(json: "[ 1, 2, 3 ]") '
+            '     g: sendJson(json: "1.01") '
+            "}"
+        )
 
         result = executor.execute(test_json_query)
 
         expected = {
-            'a': "<class 'int'>1",
-            'b': "<class 'bool'>True",
-            'c': "<class 'bool'>True",
-            'd': "<class 'str'>test",
-            'e': "<class 'dict'>{'a': 1}",
-            'f': "<class 'list'>[1, 2, 3]",
-            'g': "<class 'float'>1.01"
+            "a": "<class 'int'>1",
+            "b": "<class 'bool'>True",
+            "c": "<class 'bool'>True",
+            "d": "<class 'str'>test",
+            "e": "<class 'dict'>{'a': 1}",
+            "f": "<class 'list'>[1, 2, 3]",
+            "g": "<class 'float'>1.01",
         }
         assert not result.errors
         assert result.data == expected
 
     def test_bytes_type(self):
         api = GraphQLAPI()
 
-        data_input = b'aW5wdXRfYnl0ZXM='
-        data_output = b'b3V0cHV0X2J5dGVz'
+        data_input = b"aW5wdXRfYnl0ZXM="
+        data_output = b"b3V0cHV0X2J5dGVz"
         non_utf_output = "A".encode("utf-32")
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def byte_data(self, value: bytes) -> bytes:
                 assert value == data_input
                 return data_output
 
             @api.field
             def non_utf_byte_data(self) -> bytes:
                 return non_utf_output
 
         executor = api.executor()
 
-        test_bytes_query = f"query GetByteData {{ byteData(value: \"{data_input.decode('utf-8')}\") }}"
+        test_bytes_query = (
+            f"query GetByteData {{ byteData(value: \"{data_input.decode('utf-8')}\") }}"
+        )
 
         result = executor.execute(test_bytes_query)
 
-        expected = {
-            "byteData": data_output.decode('utf-8')
-        }
+        expected = {"byteData": data_output.decode("utf-8")}
         assert not result.errors
         assert result.data == expected
 
-        test_non_utf_bytes_query = f"query GetNonUtfByteData {{ nonUtfByteData }}"
+        test_non_utf_bytes_query = "query GetNonUtfByteData { nonUtfByteData }"
         result = executor.execute(test_non_utf_bytes_query)
 
-        expected = {
-            'nonUtfByteData': 'UTF-8 ENCODED PREVIEW: \x00\x00A\x00\x00\x00'
-        }
+        expected = {"nonUtfByteData": "UTF-8 ENCODED PREVIEW: \x00\x00A\x00\x00\x00"}
         assert not result.errors
         assert result.data == expected
```

### Comparing `graphql-api-1.3.0/tests/test_docstrings.py` & `graphql-api-1.3.1/tests/test_docstrings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-import enum
-import sys
-
-import pytest
-
 from dataclasses import dataclass
-from typing import Union, Optional
+from typing import Optional
 
-from graphql import GraphQLSchema
-from requests.api import request
-from requests.exceptions import ConnectionError, ConnectTimeout, ReadTimeout
-
-# noinspection PyPackageRequirements
-from graphql.utilities import print_schema
-
-from graphql_api.utils import executor_to_ast
-from graphql_api.error import GraphQLError
-from graphql_api.context import GraphQLContext
-from graphql_api.api import GraphQLAPI, GraphQLRootTypeDelegate
-from graphql_api.reduce import TagFilter
-from graphql_api.remote import GraphQLRemoteExecutor, remote_execute
-from graphql_api.decorators import field
+from graphql_api.api import GraphQLAPI
 
 
 class TestGraphQL:
-
     def test_basic_docstring(self):
         api = GraphQLAPI()
 
         class Node:
             """
             NODE_DOCSTRING
             """
@@ -52,15 +33,15 @@
                 """
                 return Node()
 
         schema = api.graphql_schema()[0]
 
         assert schema.query_type.description == "ROOT_DOCSTRING"
 
-        root_field = schema.query_type.fields['rootField']
+        root_field = schema.query_type.fields["rootField"]
 
         assert root_field.description == "ROOT_FIELD_DOCSTRING"
 
         root_field_type = root_field.type.of_type
 
         assert root_field_type.description == "NODE_DOCSTRING"
 
@@ -72,14 +53,15 @@
         api = GraphQLAPI()
 
         @dataclass
         class Node:
             """
             NODE_DOCSTRING
             """
+
             string_field: Optional[str] = None
             int_field: Optional[int] = None
 
             @api.field
             def node_field(self, test: int) -> int:
                 """
                 NODE_FIELD_DOCSTRING
@@ -99,15 +81,15 @@
                 """
                 return Node()
 
         schema = api.graphql_schema()[0]
 
         assert schema.query_type.description == "ROOT_DOCSTRING"
 
-        root_field = schema.query_type.fields['rootField']
+        root_field = schema.query_type.fields["rootField"]
 
         assert root_field.description == "ROOT_FIELD_DOCSTRING"
 
         root_field_type = root_field.type.of_type
 
         assert root_field_type.description == "NODE_DOCSTRING"
 
@@ -119,14 +101,15 @@
         api = GraphQLAPI()
 
         @dataclass
         class Node:
             """
             NODE_DOCSTRING
             """
+
             string_field: Optional[str] = None
             """STRING_FIELD_DOCSTRING"""
             int_field: Optional[int] = None
             """INT_FIELD_DOCSTRING"""
 
             @api.field
             def node_field(self, test: int) -> int:
@@ -148,15 +131,15 @@
                 """
                 return Node()
 
         schema = api.graphql_schema()[0]
 
         assert schema.query_type.description == "ROOT_DOCSTRING"
 
-        root_field = schema.query_type.fields['rootField']
+        root_field = schema.query_type.fields["rootField"]
 
         assert root_field.description == "ROOT_FIELD_DOCSTRING"
 
         root_field_type = root_field.type.of_type
 
         assert root_field_type.description == "NODE_DOCSTRING"
 
@@ -176,33 +159,33 @@
             """
             NODE_DOCSTRING
 
             Args:
                 string_field: STRING_FIELD_DOCSTRING
                 int_field: INT_FIELD_DOCSTRING
             """
+
             string_field: Optional[str] = None
             int_field: Optional[int] = None
 
             @api.field
             def node_field(self, test: int) -> int:
                 """
                 NODE_FIELD_DOCSTRING
                 """
                 return test * test
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def root_field(self) -> Node:
                 return Node()
 
         schema = api.graphql_schema()[0]
-        root_field = schema.query_type.fields['rootField']
+        root_field = schema.query_type.fields["rootField"]
         root_field_type = root_field.type.of_type
 
         string_field = root_field_type.fields["stringField"]
         int_field = root_field_type.fields["intField"]
         node_field = root_field_type.fields["nodeField"]
 
         assert string_field.description == "STRING_FIELD_DOCSTRING"
```

### Comparing `graphql-api-1.3.0/tests/test_filtering.py` & `graphql-api-1.3.1/tests/test_filtering.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,116 +1,103 @@
 from graphql_api.mapper import GraphQLMetaKey
 from graphql_api.api import GraphQLAPI
 
 
 class TestSchemaFiltering:
-
     def test_query_remove_invalid(self):
         api = GraphQLAPI()
 
         class Person:
-
             def __init__(self):
                 self.name = ""
 
             @api.field(mutable=True)
-            def update_name(self, name: str) -> 'Person':
+            def update_name(self, name: str) -> "Person":
                 self.name = name
                 return self
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def person(self) -> Person:
                 return Person()
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query PersonName {
                 person {
                     updateName(name:"phil") {
                         name
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
         assert result.errors
-        assert 'Cannot query field' in result.errors[0].message
+        assert "Cannot query field" in result.errors[0].message
 
     def test_mutation_return_query(self):
         """
         Mutation fields by default should return queries
         :return:
         """
         api = GraphQLAPI()
 
         class Person:
-
             def __init__(self):
                 self._name = ""
 
             @api.field
             def name(self) -> str:
                 return self._name
 
             @api.field(mutable=True)
-            def update_name(self, name: str) -> 'Person':
+            def update_name(self, name: str) -> "Person":
                 self._name = name
                 return self
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def person(self) -> Person:
                 return Person()
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             mutation PersonName {
                 person {
                     updateName(name:"phil") {
                         name
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
         assert not result.errors
 
-        expected = {
-            "person": {
-                "updateName": {
-                    "name": "phil"
-                }
-            }
-        }
+        expected = {"person": {"updateName": {"name": "phil"}}}
 
         assert result.data == expected
 
     def test_keep_interface(self):
         api = GraphQLAPI()
 
         @api.type(interface=True)
         class Person:
-
             @api.field
             def name(self) -> str:
                 pass
 
         class Employee(Person):
-
             def __init__(self):
                 self._name = "Bob"
 
             @api.field
             def name(self) -> str:
                 return self._name
 
@@ -124,57 +111,46 @@
                 return name
 
         bob_employee = Employee()
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def person(self) -> Person:
                 return bob_employee
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query PersonName {
                 person {
                     name
                     ... on Employee {
                         department
                     }
                 }
             }
-        '''
+        """
 
-        test_mutation = '''
+        test_mutation = """
             mutation SetPersonName {
                 person {
                     ... on EmployeeMutable {
                         setName(name: "Tom")
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "person": {
-                "name": "Bob",
-                "department": "Human Resources"
-            }
-        }
+        expected = {"person": {"name": "Bob", "department": "Human Resources"}}
 
-        expected_2 = {
-            "person": {
-                "name": "Tom",
-                "department": "Human Resources"
-            }
-        }
+        expected_2 = {"person": {"name": "Tom", "department": "Human Resources"}}
 
         assert result.data == expected
 
         result = executor.execute(test_mutation)
 
         assert not result.errors
 
@@ -183,114 +159,98 @@
         assert result.data == expected_2
 
     def test_mutation_return_mutable_flag(self):
         api = GraphQLAPI()
 
         @api.type
         class Person:
-
             def __init__(self):
                 self._name = ""
 
             @api.field
             def name(self) -> str:
                 return self._name
 
             @api.field(mutable=True)
-            def update_name(self, name: str) -> 'Person':
+            def update_name(self, name: str) -> "Person":
                 self._name = name
                 return self
 
             @api.field({GraphQLMetaKey.resolve_to_mutable: True}, mutable=True)
-            def update_name_mutable(self, name: str) -> 'Person':
+            def update_name_mutable(self, name: str) -> "Person":
                 self._name = name
                 return self
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def person(self) -> Person:
                 return Person()
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
                     mutation PersonName {
                         person {
                             updateName(name:"phil") {
                                 name
                             }
                         }
                     }
-                '''
+                """
 
         result = executor.execute(test_query)
         assert not result.errors
 
-        expected = {
-            "person": {
-                "updateName": {
-                    "name": "phil"
-                }
-            }
-        }
+        expected = {"person": {"updateName": {"name": "phil"}}}
 
         assert result.data == expected
 
-        test_mutable_query = '''
+        test_mutable_query = """
                     mutation PersonName {
                         person {
                             updateNameMutable(name:"tom") {
                                 updateName(name:"phil") {
                                     name
                                 }
                             }
                         }
                     }
-                '''
+                """
 
         result = executor.execute(test_mutable_query)
         assert not result.errors
 
-        expected = {
-            "person": {
-                "updateNameMutable": {
-                    "updateName": {
-                        "name": "phil"
-                    }
-                }
-            }
-        }
+        expected = {"person": {"updateNameMutable": {"updateName": {"name": "phil"}}}}
 
         assert result.data == expected
 
-        test_invalid_query = '''
+        test_invalid_query = """
                     mutation PersonName {
                         person {
                             updateName(name:"tom") {
                                 updateName(name:"phil") {
                                     name
                                 }
                             }
                         }
                     }
-                '''
+                """
 
         result = executor.execute(test_invalid_query)
         assert result.errors
         assert "Cannot query field 'updateName'" in result.errors[0].message
 
-        test_invalid_mutable_query = '''
+        test_invalid_mutable_query = """
                     mutation PersonName {
                         person {
                             updateNameMutable(name:"tom") {
                                 name
                             }
                         }
                     }
-                '''
+                """
 
         result = executor.execute(test_invalid_mutable_query)
         assert result.errors
         assert "Cannot query field 'name'" in result.errors[0].message
```

### Comparing `graphql-api-1.3.0/tests/test_graphql.py` & `graphql-api-1.3.1/tests/test_graphql.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,167 +26,156 @@
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
 
     return False
 
 
 # noinspection PyPep8Naming,DuplicatedCode
 class TestGraphQL:
-
     def test_multiple_apis(self):
         api_1 = GraphQLAPI()
         api_2 = GraphQLAPI()
 
         @api_1.type
         class Math:
-
             @api_1.field
             def test_square(self, number: int) -> int:
                 return number * number
 
             @api_2.field
             def test_cube(self, number: int) -> int:
                 return number * number * number
 
         # noinspection PyUnusedLocal
         @api_1.type(root=True)
         @api_2.type(root=True)
         class Root:
-
             @api_1.field
             @api_2.field
             def math(self) -> Math:
                 return Math()
 
-        result_1 = api_1.execute('''
+        result_1 = api_1.execute(
+            """
             query GetTestSquare {
                 math {
                     square: testSquare(number: %d)
                 }
             }
-        ''' % 5)
+        """
+            % 5
+        )
 
-        expected = {
-            "math": {
-                "square": 25
-            }
-        }
+        expected = {"math": {"square": 25}}
         assert not result_1.errors
         assert result_1.data == expected
 
-        result_2 = api_2.execute('''
+        result_2 = api_2.execute(
+            """
             query GetTestCube {
                 math {
                     square: testCube(number: %d)
                 }
             }
-        ''' % 5)
+        """
+            % 5
+        )
 
-        expected = {
-            "math": {
-                "square": 125
-            }
-        }
+        expected = {"math": {"square": 125}}
         assert not result_2.errors
         assert result_2.data == expected
 
-        result_3 = api_2.execute('''
+        result_3 = api_2.execute(
+            """
             query GetTestSquare {
                 math {
                     square: testSquare(number: %d)
                 }
             }
-        ''' % 5)
+        """
+            % 5
+        )
 
         assert result_3.errors
 
     def test_deep_query(self):
         api = GraphQLAPI()
 
         class Math:
-
             @api.field
             def test_square(self, number: int) -> int:
                 return number * number
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def math(self) -> Math:
                 return Math()
 
-        result = api.execute('''
+        result = api.execute(
+            """
             query GetTestSquare {
                 math {
                     square: testSquare(number: %d)
                 }
             }
-        ''' % 5)
+        """
+            % 5
+        )
 
-        expected = {
-            "math": {
-                "square": 25
-            }
-        }
+        expected = {"math": {"square": 25}}
         assert not result.errors
         assert result.data == expected
 
     def test_query_object_input(self):
         api = GraphQLAPI()
 
         class Person:
-
             def __init__(self, name: str):
                 self.name = name
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def get_name(self, person: Person) -> str:
                 return person.name
 
-        test_query = '''
+        test_query = """
             query GetTestSquare {
                 getName(person: { name: "steve" })
             }
-        '''
+        """
 
         result = api.execute(test_query)
 
-        expected = {
-            "getName": "steve"
-        }
+        expected = {"getName": "steve"}
         assert not result.errors
         assert result.data == expected
 
     def test_custom_query_input(self):
         api = GraphQLAPI()
 
         class Person:
-
             @classmethod
             def graphql_from_input(cls, age: int):
                 person = Person(name="hugh")
                 person.age = age
                 return person
 
             def __init__(self, name: str):
@@ -198,121 +187,102 @@
                 return self.name
 
             @api.field
             def age(self) -> int:
                 return self.age
 
         class Root:
-
             @api.field
             def person_info(self, person: Person) -> str:
                 return person.name + " is " + str(person.age)
 
         api.root_type = Root
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetPersonInfo {
                 personInfo(person: { age: 30 })
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "personInfo": "hugh is 30"
-        }
+        expected = {"personInfo": "hugh is 30"}
         assert not result.errors
         assert result.data == expected
 
     def test_runtime_field(self):
         api = GraphQLAPI()
 
         class Person:
-
             @classmethod
             def graphql_fields(cls):
-
                 @api.field
                 def age(_self) -> int:
                     return _self.hidden_age
 
                 return [age]
 
             def __init__(self, age: int):
                 self.hidden_age = age
 
         class Root:
-
             @api.field
             def thomas(self) -> Person:
                 return Person(age=2)
 
         api.root_type = Root
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetThomasAge {
                 thomas { age }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "thomas": {
-                "age": 2
-            }
-        }
+        expected = {"thomas": {"age": 2}}
         assert not result.errors
         assert result.data == expected
 
     def test_recursive_query(self):
         api = GraphQLAPI()
 
         class Root:
-
             @api.field
-            def root(self) -> 'Root':
+            def root(self) -> "Root":
                 return Root()
 
             @api.field
             def value(self) -> int:
                 return 5
 
         api.root_type = Root
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetRecursiveRoot {
                 root {
                     root {
                         value
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "root": {
-                "root":  {
-                    "value": 5
-                }
-            }
-        }
+        expected = {"root": {"root": {"value": 5}}}
         assert not result.errors
         assert result.data == expected
 
     def test_field_filter(self):
-
         # noinspection PyUnusedLocal
         class Root:
-
             @field
             def name(self) -> str:
                 return "rob"
 
             @field({"tags": ["admin"]})
             def social_security_number(self) -> int:
                 return 56
@@ -342,15 +312,14 @@
 
     def test_property(self):
         api = GraphQLAPI()
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             def __init__(self):
                 self._test_property = 5
 
             @property
             @api.field
             def test_property(self) -> int:
                 return self._test_property
@@ -360,194 +329,165 @@
             @api.field(mutable=True)
             def test_property(self, value: int) -> int:
                 self._test_property = value
                 return self._test_property
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetTestProperty {
                 testProperty
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "testProperty": 5
-        }
+        expected = {"testProperty": 5}
         assert not result.errors
         assert result.data == expected
 
-        test_mutation = '''
+        test_mutation = """
             mutation SetTestProperty {
                 testProperty(value: 10)
             }
-        '''
+        """
 
         result = executor.execute(test_mutation)
 
-        expected = {
-            "testProperty": 10
-        }
+        expected = {"testProperty": 10}
         assert not result.errors
         assert result.data == expected
 
     def test_interface(self):
         api = GraphQLAPI()
 
         @api.type(interface=True)
         class Animal:
-
             @api.field
             def planet(self) -> str:
                 return "Earth"
 
             @api.field
             def name(self) -> str:
                 return "GenericAnimalName"
 
         class Dog(Animal):
-
             @api.field
             def name(self) -> str:
                 return "Floppy"
 
         class Human(Animal):
-
             @api.field
             def name(self) -> str:
                 return "John"
 
             @api.field
             def pet(self) -> Dog:
                 return Dog()
 
         class Root:
-
             @api.field
             def best_animal(self, task: str = "bark") -> Animal:
                 if task == "bark":
                     return Dog()
                 return Human()
 
         api.root_type = Root
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetAnimal {
                 bestAnimal(task: "%s") {
                     planet
                     name
                     ... on Human {
                         pet {
                             name
                         }
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query % "bark")
 
-        expected = {
-            "bestAnimal": {
-                "planet": "Earth",
-                "name": "Floppy"
-            }
-        }
+        expected = {"bestAnimal": {"planet": "Earth", "name": "Floppy"}}
 
         assert not result.errors
         assert result.data == expected
 
         result = executor.execute(test_query % "making a cake")
 
         expected = {
-            "bestAnimal": {
-                "planet": "Earth",
-                "name": "John",
-                "pet": {
-                    "name": "Floppy"
-                }
-            }
+            "bestAnimal": {"planet": "Earth", "name": "John", "pet": {"name": "Floppy"}}
         }
         assert not result.errors
         assert result.data == expected
 
     def test_multiple_interfaces(self):
         api = GraphQLAPI()
 
         @api.type(interface=True)
         class Animal:
-
             @api.field
             def name(self) -> str:
                 return "GenericAnimalName"
 
         @api.type(interface=True)
         class Object:
-
             @api.field
             def weight(self) -> int:
                 return 100
 
         @api.type(interface=True)
         class Responds:
-
             # noinspection PyUnusedLocal
             @api.field
             def ask_question(self, text: str) -> str:
                 return "GenericResponse"
 
         class BasicRespondMixin(Responds, Animal):
-
             @api.field
             def ask_question(self, text: str) -> str:
                 return f"Hello, im {self.name()}!"
 
         class Dog(BasicRespondMixin, Animal, Object):
-
             @api.field
             def name(self) -> str:
                 return "Floppy"
 
             @api.field
             def weight(self) -> int:
                 return 20
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def animal(self) -> Animal:
                 return Dog()
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetDog {
                 animal {
                     name
                     ... on Dog {
                         weight
                         response: askQuestion(text: "Whats your name?")
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         expected = {
-            "animal": {
-                "name": "Floppy",
-                "weight": 20,
-                "response": "Hello, im Floppy!"
-            }
+            "animal": {"name": "Floppy", "weight": 20, "response": "Hello, im Floppy!"}
         }
 
         assert not result.errors
         assert result.data == expected
 
     def test_dataclass(self):
         api = GraphQLAPI()
@@ -557,126 +497,114 @@
         @dataclass
         class Root:
             hello_world: str = "hello world"
             hello_world_optional: Optional[str] = None
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query HelloWorld {
                 helloWorld
                 helloWorldOptional
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "helloWorld": "hello world",
-            'helloWorldOptional': None
-        }
+        expected = {"helloWorld": "hello world", "helloWorldOptional": None}
         assert not result.errors
         assert result.data == expected
 
     def test_mutation(self):
         api = GraphQLAPI()
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field(mutable=True)
             def hello_world(self) -> str:
                 return "hello world"
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             mutation HelloWorld {
                 helloWorld
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "helloWorld": "hello world"
-        }
+        expected = {"helloWorld": "hello world"}
         assert not result.errors
         assert result.data == expected
 
     def test_deep_mutation(self):
         api = GraphQLAPI()
 
         class Math:
-
             @api.field
             def square(self, number: int) -> int:
                 return number * number
 
             @api.field(mutable=True)
             def create_square(self, number: int) -> int:
                 return number * number
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def math(self) -> Math:
                 return Math()
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = (
+            """
         mutation GetTestSquare {
             math {
                 square: createSquare(number: %d)
             }
         }
-        ''' % 5
+        """
+            % 5
+        )
 
         result = executor.execute(test_query)
 
-        expected = {
-            "math": {
-                "square": 25
-            }
-        }
+        expected = {"math": {"square": 25}}
         assert not result.errors
         assert result.data == expected
 
     def test_print(self):
-
         api = GraphQLAPI()
 
         class Math:
-
             @api.field
             def square(self, number: int) -> int:
                 return number * number
 
             @api.field(mutable=True)
             def create_square(self, number: int) -> int:
                 return number * number
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def math(self) -> Math:
                 return Math()
 
         schema, _ = api.graphql_schema()
 
         schema_str = print_schema(schema)
         schema_str = schema_str.strip().replace(" ", "")
 
-        expected_schema_str = '''
+        expected_schema_str = """
             schema {
                 query: Root
                 mutation: RootMutable
             }
 
             type Root {
                 math: Math!
@@ -689,77 +617,71 @@
             type Math {
                 square(number: Int!): Int!
             }
 
             type MathMutable {
                 createSquare(number: Int!): Int!
             }
-        '''.strip().replace(" ", "")
+        """.strip().replace(
+            " ", ""
+        )
 
         assert set(schema_str.split("}")) == set(expected_schema_str.split("}"))
 
     # noinspection PyUnusedLocal
     def test_middleware(self):
         api = GraphQLAPI()
 
         was_called = []
 
         @api.type(root=True)
         class Root:
-
             @api.field({"test_meta": "hello_meta"})
             def test_query(self, test_string: str = None) -> str:
                 if test_string == "hello":
                     return "world"
                 return "not_possible"
 
         def test_middleware(next_, context):
             if context.field.meta.get("test_meta") == "hello_meta":
-                if context.request.args.get('test_string') == "hello":
+                if context.request.args.get("test_string") == "hello":
                     return next_()
             return "possible"
 
         def test_simple_middleware(next_):
             was_called.append(True)
             return next_()
 
-        middleware = [
-            test_middleware,
-            test_simple_middleware
-        ]
+        middleware = [test_middleware, test_simple_middleware]
 
         executor = api.executor(middleware=middleware)
 
-        test_mutation = '''
+        test_mutation = """
             query TestMiddlewareQuery {
                 testQuery(testString: "hello")
             }
-        '''
+        """
 
         result = executor.execute(test_mutation)
 
         assert was_called
 
-        expected = {
-            "testQuery": "world"
-        }
+        expected = {"testQuery": "world"}
         assert not result.errors
         assert result.data == expected
 
-        test_mutation = '''
+        test_mutation = """
             query TestMisddlewareQuery {
                 testQuery(testString: "not_hello")
             }
-        '''
+        """
 
         result = executor.execute(test_mutation)
 
-        expected = {
-            "testQuery": "possible"
-        }
+        expected = {"testQuery": "possible"}
         assert not result.errors
         assert result.data == expected
 
     # noinspection PyUnusedLocal
     def test_input(self):
         api = GraphQLAPI()
 
@@ -774,66 +696,60 @@
 
             @api.field
             def value_squared(self) -> int:
                 return self._value * self._value
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def square(self, value: TestInputObject) -> TestInputObject:
                 return value
 
         executor = api.executor()
 
-        test_input_query = '''
+        test_input_query = """
             query TestInputQuery {
                 square(value: {aValue: 14}){
                     valueSquared
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_input_query)
 
-        expected = {
-            "square": {
-                "valueSquared": 196
-            }
-        }
+        expected = {"square": {"valueSquared": 196}}
         assert not result.errors
         assert result.data == expected
 
     # noinspection PyUnusedLocal
     def test_enum(self):
         api = GraphQLAPI()
 
         class AnimalType(enum.Enum):
             dog = "dog"
             cat = "cat"
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def opposite(self, animal: AnimalType) -> AnimalType:
                 assert isinstance(animal, AnimalType)
 
                 if animal == AnimalType.dog:
                     return AnimalType.cat
 
                 return AnimalType.dog
 
         executor = api.executor()
 
-        test_enum_query = '''
+        test_enum_query = """
             query TestEnum {
                 opposite(animal: dog)
             }
-        '''
+        """
 
         result = executor.execute(test_enum_query)
         expected = {"opposite": "cat"}
 
         assert result.data == expected
 
     # noinspection PyUnusedLocal
@@ -842,65 +758,61 @@
 
         class AnimalType(enum.Enum):
             dog = "dog"
             cat = "cat"
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def all(self, animals: List[AnimalType]) -> List[AnimalType]:
-                assert all(
-                    isinstance(animal, AnimalType) for animal in animals
-                )
+                assert all(isinstance(animal, AnimalType) for animal in animals)
 
                 return animals
 
         executor = api.executor()
 
-        test_enum_query = '''
+        test_enum_query = """
             query TestEnum {
                 all(animals: [dog, cat])
             }
-        '''
+        """
 
         result = executor.execute(test_enum_query)
-        expected = {"all": ["dog","cat"]}
+        expected = {"all": ["dog", "cat"]}
 
         assert result.data == expected
 
     def test_optional_enum(self):
         api = GraphQLAPI()
 
         class AnimalType(enum.Enum):
             dog = "dog"
             cat = "cat"
 
         @api.type(root=True)
         class Root:
-
             @api.field
-            def opposite(self, animal: Optional[AnimalType] = None) \
-                    -> Optional[AnimalType]:
-
+            def opposite(
+                self, animal: Optional[AnimalType] = None
+            ) -> Optional[AnimalType]:
                 if animal is None:
                     return None
 
                 if animal == AnimalType.dog:
                     return AnimalType.cat
 
                 return AnimalType.dog
 
         executor = api.executor()
 
-        test_enum_query = '''
+        test_enum_query = """
                 query TestEnum {
                     opposite
                 }
-            '''
+            """
 
         result = executor.execute(test_enum_query)
         expected = {"opposite": None}
         assert not result.errors
 
         assert result.data == expected
 
@@ -908,360 +820,342 @@
     def test_functional_enum(self):
         api = GraphQLAPI()
 
         AnimalType = enum.Enum("AnimalType", ["dog", "cat"])
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def opposite(self, animal: AnimalType) -> AnimalType:
                 assert isinstance(animal, AnimalType)
 
                 if animal == AnimalType.dog:
                     return AnimalType.cat
 
                 return AnimalType.dog
 
         executor = api.executor()
 
-        test_enum_query = '''
+        test_enum_query = """
             query TestEnum {
                 opposite(animal: dog)
             }
-        '''
+        """
 
         result = executor.execute(test_enum_query)
         expected = {"opposite": "cat"}
 
         assert result.data == expected
 
     # noinspection PyUnusedLocal
     def test_literal(self):
         api = GraphQLAPI()
 
         Period = Literal["1d", "5d", "1mo", "3mo", "6mo", "1y"]
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def get_count(self, period: Period) -> int:
                 if period == "1d":
                     return 365
 
                 return 0
 
         executor = api.executor()
 
-        test_literal_query = '''
+        test_literal_query = """
             query TestEnum {
                 getCount(period: "1d")
             }
-        '''
+        """
 
         result = executor.execute(test_literal_query)
         expected = {"getCount": 365}
 
         assert result.data == expected
 
     # noinspection PyUnusedLocal
     def test_required(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def value(self, a_int: int) -> Optional[int]:
                 return a_int
 
         executor = api.executor()
 
-        test_input_query = '''
+        test_input_query = """
             query TestOptionalQuery {
                 value
             }
-        '''
+        """
 
         result = executor.execute(test_input_query)
 
-        assert result.errors and "is required, but it was not provided" in result.errors[0].message
+        assert (
+            result.errors
+            and "is required, but it was not provided" in result.errors[0].message
+        )
 
     # noinspection PyUnusedLocal
     def test_optional(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def value(self, a_int: int = 50) -> int:
                 return a_int
 
         executor = api.executor()
 
-        test_input_query = '''
+        test_input_query = """
             query TestOptionalQuery {
                 value
             }
-        '''
+        """
 
         result = executor.execute(test_input_query)
 
-        expected = {
-            "value": 50
-        }
+        expected = {"value": 50}
         assert not result.errors
         assert result.data == expected
 
-    @pytest.mark.skipif(
-        sys.version_info < (3, 10), reason="requires python3.10"
-    )
+    @pytest.mark.skipif(sys.version_info < (3, 10), reason="requires python3.10")
     def test_optional_311(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def value(self, a_int: int | None = 50) -> Optional[int]:
                 return a_int
 
         executor = api.executor()
 
-        test_input_query = '''
+        test_input_query = """
             query TestOptionalQuery {
                 value
             }
-        '''
+        """
 
         result = executor.execute(test_input_query)
 
-        expected = {
-            "value": 50
-        }
+        expected = {"value": 50}
         assert not result.errors
         assert result.data == expected
 
     # noinspection PyUnusedLocal
     def test_union(self):
         api = GraphQLAPI()
 
         class Customer:
-
             @api.field
             def id(self) -> int:
                 return 5
 
         class Owner:
-
             @api.field
             def name(self) -> str:
                 return "rob"
 
         @api.type(root=True)
         class Bank:
-
             @api.field
-            def owner_or_customer(self, owner: bool = True, none: bool = False) -> Optional[Union[Owner, Customer]]:
+            def owner_or_customer(
+                self, owner: bool = True, none: bool = False
+            ) -> Optional[Union[Owner, Customer]]:
                 if owner:
                     return Owner()
 
                 if none:
                     return None
 
                 return Customer()
 
         executor = api.executor()
 
-        test_owner_query = '''
+        test_owner_query = """
             query TestOwnerUnion {
                 ownerOrCustomer {
                     ... on Owner {
                       name
                     }
                 }
             }
-        '''
+        """
 
-        owner_expected = {
-            "ownerOrCustomer": {
-                "name": "rob"
-            }
-        }
+        owner_expected = {"ownerOrCustomer": {"name": "rob"}}
 
         owner_result = executor.execute(test_owner_query)
         assert not owner_result.errors
         assert owner_result.data == owner_expected
 
-        test_customer_query = '''
+        test_customer_query = """
             query TestCustomerUnion {
                 ownerOrCustomer(owner: false) {
                     ... on Customer {
                       id
                     }
                 }
             }
-        '''
+        """
 
-        customer_expected = {
-            "ownerOrCustomer": {
-                "id": 5
-            }
-        }
+        customer_expected = {"ownerOrCustomer": {"id": 5}}
 
         customer_result = executor.execute(test_customer_query)
         assert not customer_result.errors
         assert customer_result.data == customer_expected
 
-        test_none_query = '''
+        test_none_query = """
             query TestCustomerUnion {
                 ownerOrCustomer(owner: false, none: true) {
                     ... on Customer {
                       id
                     }
                 }
             }
-        '''
+        """
 
-        none_expected = {
-            "ownerOrCustomer": None
-        }
+        none_expected = {"ownerOrCustomer": None}
 
         none_result = executor.execute(test_none_query)
         assert not none_result.errors
         assert none_result.data == none_expected
 
     # noinspection PyUnusedLocal
     def test_non_null(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def non_nullable(self) -> int:
                 # noinspection PyTypeChecker
                 return None
 
             @api.field
             def nullable(self) -> Optional[int]:
                 return None
 
         executor = api.executor()
 
-        test_non_null_query = '''
+        test_non_null_query = """
             query TestNonNullQuery {
                 nonNullable
             }
-        '''
+        """
 
         non_null_result = executor.execute(test_non_null_query)
 
         assert non_null_result.errors
 
-        test_null_query = '''
+        test_null_query = """
             query TestNullQuery {
                 nullable
             }
-        '''
+        """
 
-        expected = {
-            "nullable": None
-        }
+        expected = {"nullable": None}
 
         null_result = executor.execute(test_null_query)
         assert not null_result.errors
         assert null_result.data == expected
 
     # noinspection PyUnusedLocal
     def test_context(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def has_context(self, context: GraphQLContext) -> bool:
                 return bool(context)
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query HasContext {
                 hasContext
             }
-        '''
+        """
 
-        expected = {
-            "hasContext": True
-        }
+        expected = {"hasContext": True}
 
         result = executor.execute(test_query)
 
         assert not result.errors
         assert result.data == expected
 
     star_wars_api_url = "https://swapi-graphql.netlify.app/.netlify/functions/index"
 
     # noinspection DuplicatedCode,PyUnusedLocal
-    @pytest.mark.skipif(not available(star_wars_api_url),
-                        reason=f"The star wars API '{star_wars_api_url}' is unavailable")
+    @pytest.mark.skipif(
+        not available(star_wars_api_url),
+        reason=f"The star wars API '{star_wars_api_url}' is unavailable",
+    )
     def test_remote_get(self):
         api = GraphQLAPI()
 
         RemoteAPI = GraphQLRemoteExecutor(url=self.star_wars_api_url)
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def star_wars(self, context: GraphQLContext) -> RemoteAPI:
                 operation = context.request.info.operation.operation
                 query = context.field.query
                 redirected_query = operation.value + " " + query
                 _result = RemoteAPI.execute(query=redirected_query)
 
                 if _result.errors:
                     raise GraphQLError(str(_result.errors))
 
                 return _result.data
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetAllFilms {
                 starWars {
                   allFilms {
                      totalCount
                   }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data.get("starWars", {}).get("allFilms", {}).get("totalCount", {}) >= 6
+        assert (
+            result.data.get("starWars", {}).get("allFilms", {}).get("totalCount", {})
+            >= 6
+        )
 
     pokemon_graphql_url = "https://graphqlpokemon.favware.tech/"
 
     # noinspection DuplicatedCode
-    @pytest.mark.skipif(not available(pokemon_graphql_url),
-                        reason=f"The Pokemon API '{pokemon_graphql_url}' is unavailable")
+    @pytest.mark.skipif(
+        not available(pokemon_graphql_url),
+        reason=f"The Pokemon API '{pokemon_graphql_url}' is unavailable",
+    )
     def test_remote_post(self):
         api = GraphQLAPI()
 
-        RemoteAPI = GraphQLRemoteExecutor(url=self.pokemon_graphql_url, http_method="POST")
+        RemoteAPI = GraphQLRemoteExecutor(
+            url=self.pokemon_graphql_url, http_method="POST"
+        )
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def graphql(self, context: GraphQLContext) -> RemoteAPI:
                 operation = context.request.info.operation.operation
                 query = context.field.query
                 redirected_query = operation.value + " " + query
 
                 result_ = RemoteAPI.execute(query=redirected_query)
@@ -1269,63 +1163,61 @@
                 if result_.errors:
                     raise GraphQLError(str(result_.errors))
 
                 return result_.data
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query getPokemon {
                 graphql {
                     getPokemon(pokemon: pikachu) {
                         types
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
 
         pokemon = result.data.get("graphql").get("getPokemon")
 
         assert pokemon.get("types") == ["Electric"]
 
     @pytest.mark.skipif(
         not available(pokemon_graphql_url),
-        reason=f"The pokemon API '{pokemon_graphql_url}' is unavailable"
+        reason=f"The pokemon API '{pokemon_graphql_url}' is unavailable",
     )
     def test_remote_post_helper(self):
         api = GraphQLAPI()
 
         RemoteAPI = GraphQLRemoteExecutor(
-            url=self.pokemon_graphql_url,
-            http_method="POST"
+            url=self.pokemon_graphql_url, http_method="POST"
         )
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def graphql(self, context: GraphQLContext) -> RemoteAPI:
                 return remote_execute(executor=RemoteAPI, context=context)
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query getPokemon {
                 graphql {
                     getPokemon(pokemon: pikachu) {
                         types
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
 
         pokemon = result.data.get("graphql").get("getPokemon")
 
@@ -1333,15 +1225,14 @@
 
     # noinspection PyUnusedLocal
     def test_executor_to_ast(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Root:
-
             @api.field
             def hello(self) -> str:
                 return "hello world"
 
         executor = api.executor()
 
         schema = executor_to_ast(executor)
@@ -1356,18 +1247,15 @@
 
         @api.type(root=True)
         class Root(GraphQLRootTypeDelegate):
             was_called = False
             input_schema = None
 
             @classmethod
-            def validate_graphql_schema(
-                cls,
-                schema: GraphQLSchema
-            ) -> GraphQLSchema:
+            def validate_graphql_schema(cls, schema: GraphQLSchema) -> GraphQLSchema:
                 cls.was_called = True
                 cls.input_schema = schema
 
                 return updated_schema
 
             @api.field
             def hello(self) -> str:
@@ -1376,17 +1264,15 @@
         schema = api.graphql_schema()[0]
 
         assert Root.was_called
         assert Root.input_schema
         assert schema == updated_schema
 
     def test_schema_subclass(self):
-
         class Interface:
-
             @field
             def hello(self) -> str:
                 raise NotImplementedError()
 
             @field(mutable=True)
             def hello_mutable(self) -> str:
                 raise NotImplementedError()
@@ -1409,114 +1295,105 @@
             def hello_changed(self) -> str:
                 return "hello world"
 
         api = GraphQLAPI(root=Implementation)
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query {
                 hello
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data['hello'] == "hello world"
+        assert result.data["hello"] == "hello world"
 
-        test_query = '''
+        test_query = """
             mutation {
                 helloMutable
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data['helloMutable'] == "hello 1"
+        assert result.data["helloMutable"] == "hello 1"
 
-        test_query = '''
+        test_query = """
             query {
                 helloChanged
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data['helloChanged'] == "hello world"
+        assert result.data["helloChanged"] == "hello world"
 
     def test_class_update(self):
-
         @dataclass
         class Person:
             name: str
 
         class GreetInterface:
-
             @field
             def hello(self, person: Person) -> str:
                 raise NotImplementedError()
 
         class HashablePerson(Person):
-
             def __hash__(self):
                 return hash(self.name)
 
         class Implementation(GreetInterface):
-
             def hello(self, person: HashablePerson) -> str:
                 return f"hello {hash(person)}"
 
         api = GraphQLAPI(root=Implementation)
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query {
                 hello(person:{name:"rob"})
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data['hello'] == f"hello {hash('rob')}"
+        assert result.data["hello"] == f"hello {hash('rob')}"
 
     def test_class_update_same_name(self):
-
         @dataclass
         class Person:
             name: str
 
         class GreetInterface:
-
             @field
             def hello(self, person: Person) -> str:
                 raise NotImplementedError()
 
         class Person(Person):
-
             def __hash__(self):
                 return hash(self.name)
 
         class Implementation(GreetInterface):
-
             def hello(self, person: Person) -> str:
                 return f"hello {hash(person)}"
 
         api = GraphQLAPI(root=Implementation)
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query {
                 hello(person:{name:"rob"})
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
         assert not result.errors
-        assert result.data['hello'] == f"hello {hash('rob')}"
-
+        assert result.data["hello"] == f"hello {hash('rob')}"
```

### Comparing `graphql-api-1.3.0/tests/test_relay.py` & `graphql-api-1.3.1/tests/test_relay.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 from typing import List
 
 from graphql_api.relay import Node, Connection, Edge, PageInfo
 from graphql_api.api import GraphQLAPI
 
 
 class TestRelay:
-
     def test_relay_query(self):
         api = GraphQLAPI()
 
         class Person(Node):
-
             def __init__(self, name: str = None, *args, **kwargs):
                 super().__init__(*args, **kwargs)
                 self._name = name
 
             @property
             @api.field
             def name(self) -> str:
                 return self._name
 
         class PersonConnection(Connection):
-
             def __init__(self, people, *args, **kwargs):
                 super().__init__(*args, **kwargs)
 
                 cursors = list(people.keys())
                 start_index = 0
                 end_index = len(cursors) - 1
 
@@ -40,114 +37,93 @@
                         self.has_previous_page = True
 
                 if self._before is not None:
                     end_index = cursors.index(self._before)
                     if end_index < len(cursors) - 1:
                         self.has_next_page = True
 
-                self.filtered_cursors = cursors[start_index: end_index + 1]
+                self.filtered_cursors = cursors[start_index : end_index + 1]
 
                 self.people = people
 
                 if self._first is not None:
-                    self.filtered_cursors = self.filtered_cursors[:self._first]
+                    self.filtered_cursors = self.filtered_cursors[: self._first]
 
                 elif self._last is not None:
-                    self.filtered_cursors = self.filtered_cursors[-self._last:]
+                    self.filtered_cursors = self.filtered_cursors[-self._last :]
 
             @api.field
             def edges(self) -> List[Edge]:
                 return [
-                    Edge(
-                        cursor=cursor,
-                        node=self.people[cursor]
-                    )
+                    Edge(cursor=cursor, node=self.people[cursor])
                     for cursor in self.filtered_cursors
                 ]
 
             @api.field
             def page_info(self) -> PageInfo:
                 return PageInfo(
                     start_cursor=self.filtered_cursors[0],
                     end_cursor=self.filtered_cursors[-1],
                     has_previous_page=self.has_previous_page,
-                    has_next_page=self.has_next_page
+                    has_next_page=self.has_next_page,
                 )
 
         # noinspection PyUnusedLocal
         @api.type(root=True)
         class Root:
-
             @api.field
             def people(
                 self,
                 before: str = None,
                 after: str = None,
                 first: int = None,
-                last: int = None
+                last: int = None,
             ) -> Connection:
-
-                _people = collections.OrderedDict([
-                    ("a", Person(name="rob")),
-                    ("b", Person(name="dan")),
-                    ("c", Person(name="lily"))
-                ])
+                _people = collections.OrderedDict(
+                    [
+                        ("a", Person(name="rob")),
+                        ("b", Person(name="dan")),
+                        ("c", Person(name="lily")),
+                    ]
+                )
 
                 return PersonConnection(
-                    _people,
-                    before=before,
-                    after=after,
-                    first=first,
-                    last=last
+                    _people, before=before, after=after, first=first, last=last
                 )
 
         executor = api.executor()
 
-        test_query = '''
+        test_query = """
             query GetPeopleNextPage {
                 people {
                     pageInfo {
                         hasNextPage
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "people": {
-                "pageInfo": {
-                    "hasNextPage": False
-                }
-            }
-        }
+        expected = {"people": {"pageInfo": {"hasNextPage": False}}}
         assert not result.errors
         assert result.data == expected
 
-        test_query = '''
+        test_query = """
             query GetPeopleNames {
                 people(first: 1, after: "a")  {
                     edges {
                         node {
                         ... on Person {
                                 name
                             }
                         }
                     }
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_query)
 
-        expected = {
-            "people": {
-                "edges": [{
-                    "node": {
-                        "name": "rob"
-                    }
-                }]
-            }
-        }
+        expected = {"people": {"edges": [{"node": {"name": "rob"}}]}}
         assert not result.errors
         assert result.data == expected
```

### Comparing `graphql-api-1.3.0/tests/test_remote.py` & `graphql-api-1.3.1/tests/test_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
-import base64
 import enum
 import uuid
+
 from typing import Optional, List
 from uuid import UUID
 
 import time
 import pytest
 
 from graphql_api.error import GraphQLError
@@ -14,60 +14,50 @@
 from graphql_api.remote import GraphQLRemoteObject, GraphQLRemoteExecutor
 
 # noinspection PyTypeChecker
 from tests.test_graphql import available
 
 
 class TestGraphQLRemote:
-
     def test_remote_query(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class House:
-
             @api.field
             def number_of_doors(self) -> int:
                 return 5
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert house.number_of_doors() == 5
 
     def test_remote_query_list(self):
         api = GraphQLAPI()
 
         class Door:
-
             def __init__(self, height: int):
                 self._height = height
 
             @api.field
             def height(self) -> int:
                 return self._height
 
             @property
             @api.field
             def wood(self) -> str:
                 return "oak"
 
         @api.type(root=True)
         class House:
-
             @api.field
             def doors(self) -> List[Door]:
                 return [Door(height=3), Door(height=5)]
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         doors = house.doors()
         heights = {door.height() for door in doors}
 
         assert heights == {3, 5}
 
         doors_2 = house.doors()
@@ -77,46 +67,40 @@
         assert heights_2 == {3, 5}
         assert woods_2 == {"oak"}
 
     def test_remote_query_list_nested(self):
         api = GraphQLAPI()
 
         class Person:
-
             def __init__(self, name: str):
                 self._name = name
 
             @api.field
             def name(self) -> str:
                 return self._name
 
         class Door:
-
             def __init__(self, height: int):
                 self._height = height
 
             @api.field
             def height(self) -> int:
                 return self._height
 
             @api.field
             def owner(self) -> Person:
                 return Person(name="Rob")
 
         @api.type(root=True)
         class House:
-
             @api.field
             def doors(self) -> List[Door]:
                 return [Door(height=3), Door(height=5)]
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         doors = house.doors()
 
         with pytest.raises(ValueError, match="can only contain scalar values"):
             assert {door.owner().name() for door in doors}
 
     def test_remote_query_enum(self):
@@ -124,145 +108,120 @@
 
         class HouseType(enum.Enum):
             bungalow = "bungalow"
             flat = "flat"
 
         @api.type(root=True)
         class House:
-
             @api.field
             def type(self) -> HouseType:
                 return HouseType.bungalow
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert house.type() == HouseType.bungalow
 
     def test_remote_query_send_enum(self):
         api = GraphQLAPI()
 
         class RoomType(enum.Enum):
             bedroom = "bedroom"
             kitchen = "kitchen"
 
         class Room:
-
             def __init__(self, name: str, room_type: RoomType):
                 self._name = name
                 self._room_type = room_type
 
             @api.field
             def name(self) -> str:
                 return self._name
 
             @api.field
             def room_type(self) -> RoomType:
                 return self._room_type
 
         @api.type(root=True)
         class House:
-
             @api.field
             def get_room(self) -> Room:
                 return Room(name="robs_room", room_type=RoomType.bedroom)
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert house.get_room().room_type() == RoomType.bedroom
 
     def test_remote_query_uuid(self):
         api = GraphQLAPI()
 
         person_id = uuid.uuid4()
 
         @api.type(root=True)
         class Person:
-
             @api.field
             def id(self) -> UUID:
                 return person_id
 
-        person: Person = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        person: Person = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert person.id() == person_id
 
     def test_query_bytes(self):
         api = GraphQLAPI()
 
-        a_value = b'hello '
-        b_value = b'world'
+        a_value = b"hello "
+        b_value = b"world"
 
         @api.type(root=True)
         class BytesUtils:
-
             @api.field
             def add_bytes(self, a: bytes, b: bytes) -> bytes:
-                return b''.join([a, b])
+                return b"".join([a, b])
 
         executor = api.executor()
 
-        bytes_utils: BytesUtils = GraphQLRemoteObject(
-            executor=executor,
-            api=api
-        )
+        bytes_utils: BytesUtils = GraphQLRemoteObject(executor=executor, api=api)
         test_bytes = bytes_utils.add_bytes(a_value, b_value)
 
-        assert test_bytes == b''.join([a_value, b_value])
+        assert test_bytes == b"".join([a_value, b_value])
 
     def test_remote_query_list_parameter(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Tags:
-
             @api.field
             def join_tags(self, tags: List[str] = None) -> str:
                 return "".join(tags) if tags else ""
 
-        tags: Tags = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        tags: Tags = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert tags.join_tags() == ""
         assert tags.join_tags(tags=[]) == ""
         assert tags.join_tags(tags=["a", "b"]) == "ab"
 
     def test_remote_mutation(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Counter:
-
             def __init__(self):
                 self._value = 0
 
             @api.field(mutable=True)
             def increment(self) -> int:
                 self._value += 1
                 return self._value
 
             @property
             @api.field
             def value(self) -> int:
                 return self._value
 
-        counter: Counter = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        counter: Counter = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert counter.value == 0
         assert counter.increment() == 1
         assert counter.value == 1
 
         for x in range(10):
             counter.increment()
@@ -270,167 +229,134 @@
         assert counter.value == 11
 
     def test_remote_positional_args(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Multiplier:
-
             @api.field
             def calculate(self, value_one: int = 1, value_two: int = 1) -> int:
                 return value_one * value_two
 
-        multiplier: Multiplier = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        multiplier: Multiplier = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert multiplier.calculate(4, 2) == 8
 
     def test_remote_query_optional(self):
         api = GraphQLAPI()
 
         class Person:
-
             @property
             @api.field
             def age(self) -> int:
                 return 25
 
             @api.field
             def name(self) -> str:
                 return "rob"
 
         @api.type(root=True)
         class Bank:
-
             @api.field
             def owner(self, respond_none: bool = False) -> Optional[Person]:
                 if respond_none:
                     return None
 
                 return Person()
 
-        bank: Bank = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        bank: Bank = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert bank.owner().age == 25
-        assert bank.owner().name() == 'rob'
+        assert bank.owner().name() == "rob"
         assert bank.owner(respond_none=True) is None
 
     def test_remote_mutation_with_input(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Counter:
-
             def __init__(self):
                 self.value = 0
 
             @api.field(mutable=True)
             def add(self, value: int = 0) -> int:
                 self.value += value
                 return self.value
 
-        counter: Counter = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        counter: Counter = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert counter.add(value=5) == 5
         assert counter.add(value=10) == 15
 
     def test_remote_query_with_input(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Calculator:
-
             @api.field
             def square(self, value: int) -> int:
                 return value * value
 
-        calculator: Calculator = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        calculator: Calculator = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert calculator.square(value=5) == 25
 
     def test_remote_query_with_enumerable_input(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Calculator:
-
             @api.field
             def add(self, values: List[int]) -> int:
                 total = 0
 
                 for value in values:
                     total += value
 
                 return total
 
-        calculator: Calculator = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        calculator: Calculator = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert calculator.add(values=[5, 2, 7]) == 14
 
     def test_remote_input_object(self):
         api = GraphQLAPI()
 
         class Garden:
-
             def __init__(self, size: int):
                 self._size = size
 
             @property
             @api.field
             def size(self) -> int:
                 return self._size
 
         @api.type(root=True)
         class House:
-
             @api.field
             def value(self, garden: Garden, rooms: int = 7) -> int:
                 return (garden.size * 2) + (rooms * 10)
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
         assert house.value(garden=Garden(size=10)) == 90
 
     def test_remote_input_object_nested(self):
         api = GraphQLAPI()
 
         class Animal:
-
             def __init__(self, age: int):
                 self._age = age
 
             @property
             @api.field
             def age(self) -> int:
                 return self._age
 
         class Garden:
-
-            def __init__(
-                    self,
-                    size: int,
-                    animal: Animal,
-                    set_animal: bool = False
-            ):
+            def __init__(self, size: int, animal: Animal, set_animal: bool = False):
                 self.set_animal = set_animal
                 if set_animal:
                     self.animal = animal
                 self._size = size
 
             @property
             @api.field
@@ -440,97 +366,79 @@
             @property
             @api.field
             def animal_age(self) -> int:
                 return self.animal.age
 
         @api.type(root=True)
         class House:
-
             @api.field
             def value(self, garden: Garden, rooms: int = 7) -> int:
                 return ((garden.size * 2) + (rooms * 10)) - garden.animal_age
 
-        house: House = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         with pytest.raises(
-                GraphQLError,
-                match="nested inputs must have matching attribute to field names"
+            GraphQLError,
+            match="nested inputs must have matching attribute to field names",
         ):
-            assert house.value(
-                garden=Garden(
-                    animal=Animal(age=5),
-                    size=10)
-            ) == 85
-
-        assert house.value(
-            garden=Garden(
-                animal=Animal(age=5),
-                set_animal=True,
-                size=10)
-        ) == 85
+            assert house.value(garden=Garden(animal=Animal(age=5), size=10)) == 85
+
+        assert (
+            house.value(garden=Garden(animal=Animal(age=5), set_animal=True, size=10))
+            == 85
+        )
 
     def test_remote_recursive_mutated(self):
         api = GraphQLAPI()
 
         class Flopper:
-
             def __init__(self):
                 self._flop = True
 
             @api.field
             def value(self) -> bool:
                 return self._flop
 
             @api.field(mutable=True)
-            def flop(self) -> 'Flopper':
+            def flop(self) -> "Flopper":
                 self._flop = not self._flop
                 return self
 
         global_flopper = Flopper()
 
         @api.type(root=True)
         class Flipper:
-
             def __init__(self):
                 self._flip = True
 
             @api.field
             def value(self) -> bool:
                 return self._flip
 
             @api.field(mutable=True)
-            def flip(self) -> 'Flipper':
+            def flip(self) -> "Flipper":
                 self._flip = not self._flip
                 return self
 
             @api.field
             def flopper(self) -> Flopper:
                 return global_flopper
 
             @api.field({GraphQLMetaKey.resolve_to_self: False}, mutable=True)
-            def flagged_flip(self) -> 'Flipper':
+            def flagged_flip(self) -> "Flipper":
                 self._flip = not self._flip
                 return self
 
-        flipper: Flipper = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        flipper: Flipper = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert flipper.value()
         flipped_flipper = flipper.flagged_flip()
         assert not flipped_flipper.value()
 
-        with pytest.raises(
-                GraphQLError,
-                match="mutated objects cannot be re-fetched"
-        ):
+        with pytest.raises(GraphQLError, match="mutated objects cannot be re-fetched"):
             flipped_flipper.flagged_flip()
 
         safe_flipped_flipper = flipper.flip()
 
         assert safe_flipped_flipper.value()
 
         safe_flipped_flipper.flip()
@@ -551,15 +459,14 @@
         assert mutated_flopper.value()
         assert mutated_mutated_flopper.value()
 
     def test_remote_nested(self):
         api = GraphQLAPI()
 
         class Person:
-
             def __init__(self, name: str, age: int, height: float):
                 self._name = name
                 self._age = age
                 self._height = height
 
             @api.field
             def age(self) -> int:
@@ -571,43 +478,34 @@
 
             @property
             @api.field
             def height(self) -> float:
                 return self._height
 
             @api.field(mutable=True)
-            def update(
-                    self,
-                    name: str = None,
-                    height: float = None
-            ) -> 'Person':
-
+            def update(self, name: str = None, height: float = None) -> "Person":
                 if name:
                     self._name = name
 
                 if height:
                     self._height = height
 
                 return self
 
         @api.type(root=True)
         class Root:
-
             def __init__(self):
                 self._rob = Person(name="rob", age=10, height=183.0)
                 self._counter = 0
 
             @api.field
             def rob(self) -> Person:
                 return self._rob
 
-        root: Root = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        root: Root = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         person: Person = root.rob()
 
         assert person.name() == "rob"
         assert person.age() == 10
         assert person.height == 183.0
 
@@ -623,118 +521,102 @@
         assert person.name() == "pete"
 
     def test_remote_with_local_property(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Person:
-
             @api.field
             def age(self) -> int:
                 return 50
 
             @property
             def height(self):
                 return 183
 
-        person: Person = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        person: Person = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert person.age() == 50
         assert person.height == 183
 
     def test_remote_with_local_method(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Person:
-
             @api.field
             def age(self) -> int:
                 return 50
 
             # noinspection PyMethodMayBeStatic
             def hello(self):
                 return "hello"
 
-        person: Person = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        person: Person = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert person.age() == 50
         assert person.hello() == "hello"
 
     def test_remote_with_local_static_method(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Person:
-
             @api.field
             def age(self) -> int:
                 return 50
 
             @staticmethod
             def hello():
                 return "hello"
 
-        person: Person = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        person: Person = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert person.age() == 50
         assert person.hello() == "hello"
 
     def test_remote_with_local_class_method(self):
         api = GraphQLAPI()
 
         @api.type(root=True)
         class Person:
-
             @api.field
             def age(self) -> int:
                 return 50
 
             @classmethod
             def hello(cls):
                 assert cls == Person
                 return "hello"
 
-        person: Person = GraphQLRemoteObject(
-            executor=api.executor(),
-            api=api
-        )
+        person: Person = GraphQLRemoteObject(executor=api.executor(), api=api)
 
         assert person.age() == 50
         assert person.hello() == "hello"
 
     utc_time_api_url = "https://europe-west2-parob-297412.cloudfunctions.net/utc_time"
 
     # noinspection DuplicatedCode,PyUnusedLocal
-    @pytest.mark.skipif(not available(utc_time_api_url),
-                        reason=f"The UTCTime API '{utc_time_api_url}' is unavailable")
+    @pytest.mark.skipif(
+        not available(utc_time_api_url),
+        reason=f"The UTCTime API '{utc_time_api_url}' is unavailable",
+    )
     def test_remote_get_async(self):
         utc_time_api = GraphQLAPI()
 
         remote_executor = GraphQLRemoteExecutor(url=self.utc_time_api_url)
 
         @utc_time_api.type(root=True)
         class UTCTimeAPI:
-
             @utc_time_api.field
             def now(self) -> str:
                 pass
 
         api: UTCTimeAPI = GraphQLRemoteObject(
-            executor=remote_executor,
-            api=utc_time_api
+            executor=remote_executor, api=utc_time_api
         )
 
         request_count = 100
 
         # Async test
         async_start = time.time()
```

### Comparing `graphql-api-1.3.0/tests/test_schema.py` & `graphql-api-1.3.1/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # noinspection PyPep8Naming,DuplicatedCode
 from graphql_api import GraphQLAPI, type, field
 
 
 class TestGraphQL:
-
     def test_decorators_no_schema(self):
-
         @type
         class ObjectNoSchema:
-
             @field
             def test_query_no_schema(self, a: int) -> int:
                 pass
 
             @field(mutable=True)
             def test_mutation_no_schema(self, a: int) -> int:
                 pass
 
         @type(abstract=True)
         class AbstractNoSchema:
-
             @field
             def test_abstract_query_no_schema(self, a: int) -> int:
                 pass
 
             @field(mutable=True)
             def test_abstract_mutation_no_schema(self, a: int) -> int:
                 pass
 
         @type(interface=True)
         class InterfaceNoSchema:
-
             @field
             def test_interface_query_no_schema(self, a: int) -> int:
                 pass
 
             @field(mutable=True)
             def test_interface_mutation_no_schema(self, a: int) -> int:
                 pass
@@ -52,32 +47,29 @@
         assert InterfaceNoSchema.test_interface_mutation_no_schema.graphql
 
     def test_decorators_schema(self):
         api_1 = GraphQLAPI()
 
         @api_1.type
         class ObjectSchema:
-
             @api_1.field
             def test_query_schema(self, a: int) -> int:
                 pass
 
             @api_1.field(mutable=True)
             def test_mutation_schema(self, a: int) -> int:
                 pass
 
         assert ObjectSchema.graphql
         assert ObjectSchema.test_query_schema.graphql
         assert ObjectSchema.test_mutation_schema.graphql
 
     def test_decorators_no_schema_meta(self):
-
         @type(meta={"test": "test"})
         class ObjectNoSchemaMeta:
-
             @field(meta={"test": "test"})
             def test_query_no_schema_meta(self, a: int) -> int:
                 pass
 
             @field(meta={"test": "test"}, mutable=True)
             def test_mutation_no_schema_meta(self, a: int) -> int:
                 pass
@@ -87,20 +79,18 @@
         assert ObjectNoSchemaMeta.test_mutation_no_schema_meta.graphql
 
     def test_decorators_schema_meta(self):
         api_1 = GraphQLAPI()
 
         @api_1.type(meta={"test": "test"})
         class ObjectSchemaMeta:
-
             @api_1.field(meta={"test": "test"})
             def test_query_schema_meta(self, a: int) -> int:
                 pass
 
             @api_1.field(meta={"test": "test"}, mutable=True)
             def test_mutation_schema_meta(self, a: int) -> int:
                 pass
 
         assert ObjectSchemaMeta.graphql
         assert ObjectSchemaMeta.test_query_schema_meta.graphql
         assert ObjectSchemaMeta.test_mutation_schema_meta.graphql
-
```

### Comparing `graphql-api-1.3.0/tests/test_subscriptions.py` & `graphql-api-1.3.1/tests/test_subscriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from asyncio import sleep, create_task, wait
 from dataclasses import dataclass
-from inspect import isawaitable
-from typing import AsyncIterator, Optional
 
 import pytest
-from graphql import GraphQLSchema, GraphQLObjectType, GraphQLField, \
-    GraphQLInt, subscribe, parse, MapAsyncIterator, graphql
+from graphql import (
+    GraphQLSchema,
+    GraphQLObjectType,
+    GraphQLField,
+    GraphQLInt,
+    subscribe,
+    parse,
+    MapAsyncIterator,
+    graphql,
+)
 from graphql.pyutils import SimplePubSub
 
 from graphql_api import GraphQLAPI
 
 count = 0
 pubsub = SimplePubSub()
 
@@ -28,26 +34,19 @@
 def subscribe_count(_root, info):
     return pubsub.get_subscriber()
 
 
 schema = GraphQLSchema(
     query=GraphQLObjectType(
         "RootQueryType",
-        {
-            "count": GraphQLField(GraphQLInt, resolve=resolve_count)
-        },
+        {"count": GraphQLField(GraphQLInt, resolve=resolve_count)},
     ),
     mutation=GraphQLObjectType(
         "RootMutationType",
-        {
-            "increaseCount": GraphQLField(
-                GraphQLInt,
-                resolve=resolve_increase_count
-            )
-        },
+        {"increaseCount": GraphQLField(GraphQLInt, resolve=resolve_increase_count)},
     ),
     subscription=GraphQLObjectType(
         "RootSubscriptionType",
         {
             "count": GraphQLField(
                 GraphQLInt,
                 subscribe=subscribe_count,
@@ -55,18 +54,16 @@
             )
         },
     ),
 )
 
 
 class TestSubscriptions:
-
     @pytest.mark.asyncio
     async def test_subscribe_to_count(self):
-
         a = await graphql(schema, "query {count}")
         b = await graphql(schema, "mutation {increaseCount}")
         c = await graphql(schema, "query {count}")
 
         query = "subscription {count}"
 
         subscription = await subscribe(schema, parse(query))
@@ -88,53 +85,50 @@
 
         subscription = subscribe(schema, parse(query))
 
         async def receive_count():
             async for result in await subscription:
                 received_count.append(result)
 
-        done, pending = await wait([
-            create_task(receive_count()), create_task(mutate_count())
-        ], timeout=1)
-
-        assert len(received_count) == 4 \
-               and all(result.data["count"] for result in received_count)
+        done, pending = await wait(
+            [create_task(receive_count()), create_task(mutate_count())], timeout=1
+        )
+
+        assert len(received_count) == 4 and all(
+            result.data["count"] for result in received_count
+        )
 
     @pytest.mark.asyncio
     async def test_graphql_api_subscribe(self):
         api = GraphQLAPI()
 
         @dataclass
         class Comment:
             user: str
             comment: str
 
         @api.type(root=True)
         class Root:
-
             @api.field
             # async
             def on_comment_added(
-                    self,
-                    by_user: str = None
-            ) -> Comment:   # AsyncIterator[Comment]:
+                self, by_user: str = None
+            ) -> Comment:  # AsyncIterator[Comment]:
                 return Comment(user="rob", comment="test comment")
                 # comment_pub_sub = SimplePubSub()
                 # return comment_pub_sub.get_subscriber()
 
         executor = api.executor()
 
-        test_input_query = '''
+        test_input_query = """
             query {
                 onCommentAdded {
                     comment
                 }
             }
-        '''
+        """
 
         result = executor.execute(test_input_query)
 
-        expected = {
-            "onCommentAdded": {"comment": "test comment"}
-        }
+        expected = {"onCommentAdded": {"comment": "test comment"}}
         assert not result.errors
         assert result.data == expected
```

