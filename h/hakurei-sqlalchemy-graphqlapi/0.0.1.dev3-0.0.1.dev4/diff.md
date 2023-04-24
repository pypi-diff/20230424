# Comparing `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev3.tar.gz` & `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev3.tar", last modified: Mon Apr 24 08:22:12 2023, max compression
+gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev4.tar", last modified: Mon Apr 24 09:33:28 2023, max compression
```

## Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3.tar` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:22:12.274018 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/
--rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/LICENSE
--rw-rw-rw-   0        0        0     3115 2023-04-24 08:22:12.274018 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 08:22:12.267036 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/__init__.py
--rw-rw-rw-   0        0        0     3153 2023-04-24 08:20:59.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/adapter.py
--rw-rw-rw-   0        0        0      599 2023-04-24 08:12:54.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/db_engine_specs.py
--rw-rw-rw-   0        0        0     2957 2023-04-24 08:12:54.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/dialect.py
--rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/lib.py
--rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/types.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:22:12.273020 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-04-24 08:22:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-04-24 08:22:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:22:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-24 08:22:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-04-24 08:22:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 08:22:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 08:22:12.274018 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/setup.cfg
--rw-rw-rw-   0        0        0     4284 2023-04-24 08:22:05.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:28.093856 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/
+-rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/LICENSE
+-rw-rw-rw-   0        0        0     3115 2023-04-24 09:33:28.092858 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:28.075932 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/__init__.py
+-rw-rw-rw-   0        0        0    16697 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/adapter.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/db_engine_specs.py
+-rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/dialect.py
+-rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/lib.py
+-rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/types.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:33:28.092858 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/
+-rw-rw-rw-   0        0        0     3115 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:33:28.093856 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     4257 2023-04-24 09:33:27.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/setup.py
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/LICENSE` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei_sqlalchemy-graphqlapi
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/README.md` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/db_engine_specs.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/db_engine_specs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Taken from: https://github.com/apache/superset/blob/master/superset/db_engine_specs/gsheets.py  # noqa: E501
 from superset.db_engine_specs.sqlite import SqliteEngineSpec
 
 
 class GraphQLEngineSpec(SqliteEngineSpec):
     """Engine for GraphQL API tables"""
 
-    engine = "my_graphql"
-    engine_name = "My_GraphQL"
+    engine = "graphql"
+    engine_name = "GraphQL"
     allows_joins = True
     allows_subqueries = True
 
     default_driver = "apsw"
-    sqlalchemy_uri_placeholder = "my_graphql://"
+    sqlalchemy_uri_placeholder = "graphql://"
 
     # TODO(cancan101): figure out what other spec items make sense here
     # See: https://preset.io/blog/building-database-connector/
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/dialect.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sqlalchemy.engine import Connection
 from sqlalchemy.engine.url import URL
 
 from .lib import extract_query, get_last_query, run_query
 
 # -----------------------------------------------------------------------------
 
-ADAPTER_NAME = "my_graphql"
+ADAPTER_NAME = "graphql"
 
 # -----------------------------------------------------------------------------
 
 
 class APSWGraphQLDialect(APSWDialect):
     supports_statement_cache = True
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/lib.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/lib.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei-sqlalchemy-graphqlapi
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev3/setup.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for GraphQL APIs."
-VERSION = "0.0.1.dev3"
+VERSION = "0.0.1.dev4"
 
 # -----------------------------------------------------------------------------
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type = "text/markdown; charset=UTF-8; variant=GFM"
@@ -99,25 +99,24 @@
     long_description_content_type=long_description_content_type,
     author="Alex Rothberg",
     author_email="agrothberg@gmail.com",
     url="https://github.com/cancan101/graphql-db-api",
     packages=find_packages(exclude=("tests",)),
     entry_points={
         "sqlalchemy.dialects": [
-            "my_graphql = graphqldb.dialect:APSWGraphQLDialect",
+            "graphql = graphqldb.dialect:APSWGraphQLDialect",
         ],
         "shillelagh.adapter": [
-            "my_graphql = graphqldb.adapter:SystemAPIAdapter",
+            "graphql = graphqldb.adapter:GraphQLAdapter",
         ],
     },
     install_requires=(
         "shillelagh >= 1.0.6",
         "sqlalchemy >= 1.3.0",
         "requests >= 2.20.0",
-        "psutil",
         "typing-extensions",
     ),
     license="MIT",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 2 - Pre-Alpha",
```

