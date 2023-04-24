# Comparing `tmp/datasette-explain-0.1a1.tar.gz` & `tmp/datasette-explain-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-explain-0.1a1.tar", last modified: Tue Apr  4 19:11:05 2023, max compression
+gzip compressed data, was "datasette-explain-0.1a2.tar", last modified: Mon Apr 24 03:58:09 2023, max compression
```

## Comparing `datasette-explain-0.1a1.tar` & `datasette-explain-0.1a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:11:05.883195 datasette-explain-0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 19:10:48.000000 datasette-explain-0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-04 19:11:05.883195 datasette-explain-0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-04 19:10:48.000000 datasette-explain-0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:11:05.879195 datasette-explain-0.1a1/datasette_explain/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-04 19:10:48.000000 datasette-explain-0.1a1/datasette_explain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:11:05.883195 datasette-explain-0.1a1/datasette_explain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-04 19:11:05.000000 datasette-explain-0.1a1/datasette_explain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-04 19:11:05.000000 datasette-explain-0.1a1/datasette_explain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:11:05.000000 datasette-explain-0.1a1/datasette_explain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 19:11:05.000000 datasette-explain-0.1a1/datasette_explain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 19:11:05.000000 datasette-explain-0.1a1/datasette_explain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 19:11:05.000000 datasette-explain-0.1a1/datasette_explain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:11:05.883195 datasette-explain-0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-04 19:10:48.000000 datasette-explain-0.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:11:05.883195 datasette-explain-0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-04 19:10:48.000000 datasette-explain-0.1a1/tests/test_explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:58:09.196109 datasette-explain-0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 03:57:54.000000 datasette-explain-0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-24 03:58:09.196109 datasette-explain-0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 03:57:54.000000 datasette-explain-0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:58:09.196109 datasette-explain-0.1a2/datasette_explain/
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-24 03:57:54.000000 datasette-explain-0.1a2/datasette_explain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:58:09.196109 datasette-explain-0.1a2/datasette_explain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-24 03:58:09.000000 datasette-explain-0.1a2/datasette_explain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 03:58:09.000000 datasette-explain-0.1a2/datasette_explain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 03:58:09.000000 datasette-explain-0.1a2/datasette_explain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 03:58:09.000000 datasette-explain-0.1a2/datasette_explain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 03:58:09.000000 datasette-explain-0.1a2/datasette_explain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 03:58:09.000000 datasette-explain-0.1a2/datasette_explain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 03:58:09.196109 datasette-explain-0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 03:57:54.000000 datasette-explain-0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:58:09.196109 datasette-explain-0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-24 03:57:54.000000 datasette-explain-0.1a2/tests/test_explain.py
```

### Comparing `datasette-explain-0.1a1/LICENSE` & `datasette-explain-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-explain-0.1a1/PKG-INFO` & `datasette-explain-0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-explain
-Version: 0.1a1
+Version: 0.1a2
 Summary: Explain SQL queries executed using Datasette
 Home-page: https://github.com/simonw/datasette-explain
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-explain/issues
 Project-URL: CI, https://github.com/simonw/datasette-explain/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-explain/releases
```

### Comparing `datasette-explain-0.1a1/README.md` & `datasette-explain-0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `datasette-explain-0.1a1/datasette_explain/__init__.py` & `datasette-explain-0.1a2/datasette_explain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from datasette import hookimpl, Response
+from datasette.utils import derive_named_parameters
 
 
 async def explain(request, datasette):
     sql = request.args.get("sql")
-    params = dict([(k, request.args[k]) for k in request.args if k != "sql"])
     if not sql:
         return Response.json({"ok": False, "error": "No SQL query"})
     database = request.url_vars["database"]
     try:
         db = datasette.get_database(database)
     except KeyError:
         return Response.json({"ok": False, "error": "No such database"})
+    params = {name: "" for name in await derive_named_parameters(db, sql)}
     try:
         explain_result = await db.execute("explain " + sql, params)
         explain_query_result = await db.execute("explain query plan " + sql, params)
     except Exception as e:
         return Response.json({"ok": False, "error": str(e)})
 
     # Build the explain_tree
```

### Comparing `datasette-explain-0.1a1/datasette_explain.egg-info/PKG-INFO` & `datasette-explain-0.1a2/datasette_explain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-explain
-Version: 0.1a1
+Version: 0.1a2
 Summary: Explain SQL queries executed using Datasette
 Home-page: https://github.com/simonw/datasette-explain
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-explain/issues
 Project-URL: CI, https://github.com/simonw/datasette-explain/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-explain/releases
```

### Comparing `datasette-explain-0.1a1/setup.py` & `datasette-explain-0.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1a1"
+VERSION = "0.1a2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-explain-0.1a1/tests/test_explain.py` & `datasette-explain-0.1a2/tests/test_explain.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,37 +10,47 @@
     await db.execute_write("create table if not exists t1 (id integer primary key)")
     await db.execute_write("create table if not exists t2 (id integer primary key)")
     return datasette
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "sql,params,expected",
+    "sql,expected",
     (
         (
             "select 1",
-            {},
             {
                 "ok": True,
                 "explain_tree": [{"detail": "SCAN CONSTANT ROW", "children": []}],
                 "tables": [],
             },
         ),
         (
             "select * from t1",
-            {},
             {
                 "ok": True,
                 "explain_tree": [{"detail": "SCAN t1", "children": []}],
                 "tables": [{"name": "t1", "columns": ["id"]}],
             },
         ),
         (
+            "select * from t1 where id > :id",
+            {
+                "ok": True,
+                "explain_tree": [
+                    {
+                        "detail": "SEARCH t1 USING INTEGER PRIMARY KEY (rowid>?)",
+                        "children": [],
+                    }
+                ],
+                "tables": [{"name": "t1", "columns": ["id"]}],
+            },
+        ),
+        (
             "select id, (select id from t2 where t2.id = t1.id) from t1",
-            {},
             {
                 "ok": True,
                 "explain_tree": [
                     {"detail": "SCAN t1", "children": []},
                     {
                         "detail": "CORRELATED SCALAR SUBQUERY 1",
                         "children": [
@@ -55,27 +65,26 @@
                     {"name": "t1", "columns": ["id"]},
                     {"name": "t2", "columns": ["id"]},
                 ],
             },
         ),
         (
             "select count(*) from t1 where id > :id",
-            {"id": 1},
             {
                 "ok": True,
                 "explain_tree": [
                     {
                         "detail": "SEARCH t1 USING INTEGER PRIMARY KEY (rowid>?)",
                         "children": [],
                     }
                 ],
                 "tables": [{"name": "t1", "columns": ["id"]}],
             },
         ),
     ),
 )
-async def test_explain(ds, sql, params, expected):
-    params["sql"] = sql
+async def test_explain(ds, sql, expected):
+    params = {"sql": sql}
     response = await ds.client.get("/test/-/explain", params=params)
     assert response.status_code == 200
     data = response.json()
     assert data == expected
```

