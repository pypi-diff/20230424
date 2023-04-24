# Comparing `tmp/asyncpgdb-0.0.2.tar.gz` & `tmp/asyncpgdb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpgdb-0.0.2.tar", max compression
+gzip compressed data, was "asyncpgdb-0.0.3.tar", max compression
```

## Comparing `asyncpgdb-0.0.2.tar` & `asyncpgdb-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2023-01-25 13:04:40.809165 asyncpgdb-0.0.2/README.md
--rw-r--r--   0        0        0      827 2023-04-24 16:40:12.525993 asyncpgdb-0.0.2/asyncpgdb/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 13:45:42.124801 asyncpgdb-0.0.2/asyncpgdb/types/__init__.py
--rw-r--r--   0        0        0      172 2023-04-24 13:55:34.429438 asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5716 2023-04-24 16:47:30.589020 asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc
--rw-r--r--   0        0        0     1074 2023-04-24 16:29:11.125800 asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc
--rw-r--r--   0        0        0     4740 2023-04-24 14:06:39.702336 asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc
--rw-r--r--   0        0        0     6435 2023-04-24 17:00:15.915915 asyncpgdb-0.0.2/asyncpgdb/types/connectionpool.py
--rw-r--r--   0        0        0     1072 2023-04-24 15:46:54.657895 asyncpgdb-0.0.2/asyncpgdb/types/dsn.py
--rw-r--r--   0        0        0     1995 2023-04-24 17:00:15.830233 asyncpgdb-0.0.2/asyncpgdb/types/maps/__init__.py
--rw-r--r--   0        0        0     3135 2023-04-24 16:51:16.562586 asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      427 2023-04-24 15:40:06.471910 asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     2282 2023-04-24 16:52:44.454854 asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc
--rw-r--r--   0        0        0     5910 2023-04-24 16:50:41.379740 asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0      281 2023-04-24 15:32:16.634327 asyncpgdb-0.0.2/asyncpgdb/types/maps/base.py
--rw-r--r--   0        0        0     1475 2023-04-24 17:00:15.822654 asyncpgdb-0.0.2/asyncpgdb/types/maps/jsonifier.py
--rw-r--r--   0        0        0     6109 2023-04-24 17:00:15.902858 asyncpgdb-0.0.2/asyncpgdb/types/maps/util.py
--rw-r--r--   0        0        0        0 2023-04-24 14:10:13.542655 asyncpgdb-0.0.2/asyncpgdb/types/sql/__init__.py
--rw-r--r--   0        0        0      176 2023-04-24 14:16:23.734081 asyncpgdb-0.0.2/asyncpgdb/types/sql/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3168 2023-04-24 16:59:46.710316 asyncpgdb-0.0.2/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc
--rw-r--r--   0        0        0     4745 2023-04-24 16:47:13.027161 asyncpgdb-0.0.2/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc
--rw-r--r--   0        0        0     2334 2023-04-24 17:00:15.838172 asyncpgdb-0.0.2/asyncpgdb/types/sql/metadata.py
--rw-r--r--   0        0        0     4225 2023-04-24 17:00:15.882178 asyncpgdb-0.0.2/asyncpgdb/types/sql/stmt.py
--rw-r--r--   0        0        0      474 2023-04-24 17:00:21.622064 asyncpgdb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 asyncpgdb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-25 13:04:40.809165 asyncpgdb-0.0.3/README.md
+-rw-r--r--   0        0        0      827 2023-04-24 16:40:12.525993 asyncpgdb-0.0.3/asyncpgdb/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 13:45:42.124801 asyncpgdb-0.0.3/asyncpgdb/types/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-24 13:55:34.429438 asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5716 2023-04-24 16:47:30.589020 asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc
+-rw-r--r--   0        0        0     1074 2023-04-24 16:29:11.125800 asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc
+-rw-r--r--   0        0        0     4740 2023-04-24 14:06:39.702336 asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc
+-rw-r--r--   0        0        0     6395 2023-04-24 17:00:52.196366 asyncpgdb-0.0.3/asyncpgdb/types/connectionpool.py
+-rw-r--r--   0        0        0     1072 2023-04-24 15:46:54.657895 asyncpgdb-0.0.3/asyncpgdb/types/dsn.py
+-rw-r--r--   0        0        0     1995 2023-04-24 17:00:15.830233 asyncpgdb-0.0.3/asyncpgdb/types/maps/__init__.py
+-rw-r--r--   0        0        0     3135 2023-04-24 16:51:16.562586 asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      427 2023-04-24 15:40:06.471910 asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2282 2023-04-24 16:52:44.454854 asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc
+-rw-r--r--   0        0        0     5910 2023-04-24 16:50:41.379740 asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0      281 2023-04-24 15:32:16.634327 asyncpgdb-0.0.3/asyncpgdb/types/maps/base.py
+-rw-r--r--   0        0        0     1430 2023-04-24 17:00:44.146569 asyncpgdb-0.0.3/asyncpgdb/types/maps/jsonifier.py
+-rw-r--r--   0        0        0     6109 2023-04-24 17:00:15.902858 asyncpgdb-0.0.3/asyncpgdb/types/maps/util.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:10:13.542655 asyncpgdb-0.0.3/asyncpgdb/types/sql/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-24 14:16:23.734081 asyncpgdb-0.0.3/asyncpgdb/types/sql/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3168 2023-04-24 16:59:46.710316 asyncpgdb-0.0.3/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc
+-rw-r--r--   0        0        0     4745 2023-04-24 16:47:13.027161 asyncpgdb-0.0.3/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc
+-rw-r--r--   0        0        0     2302 2023-04-24 17:00:55.297663 asyncpgdb-0.0.3/asyncpgdb/types/sql/metadata.py
+-rw-r--r--   0        0        0     4274 2023-04-24 17:01:22.301514 asyncpgdb-0.0.3/asyncpgdb/types/sql/stmt.py
+-rw-r--r--   0        0        0      474 2023-04-24 17:01:39.020173 asyncpgdb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 asyncpgdb-0.0.3/PKG-INFO
```

### Comparing `asyncpgdb-0.0.2/asyncpgdb/__init__.py` & `asyncpgdb-0.0.3/asyncpgdb/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/connectionpool.py` & `asyncpgdb-0.0.3/asyncpgdb/types/connectionpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,14 @@
         vars: Optional[Union[list[dict], list[SomeSchema]]] = None,
         timeout: Optional[float] = None,
     ):
 
         query = self.compile_stmt(stmt)
         if vars:
             vars = stmt.format_vars(vars=vars)
-            print("UPSERT VARS:", vars)
 
             await self.connect()
 
             try:
 
                 result = await self.connection.executemany(
                     query, args=vars, timeout=timeout
```

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/dsn.py` & `asyncpgdb-0.0.3/asyncpgdb/types/dsn.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/maps/__init__.py` & `asyncpgdb-0.0.3/asyncpgdb/types/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/maps/jsonifier.py` & `asyncpgdb-0.0.3/asyncpgdb/types/maps/jsonifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         }
 
     def jsonify_vars(
         self, __data: Union[dict, SomeModel, SomeSchema], include_null: bool = True
     ):
         getter = dict.get if isinstance(__data, dict) else getattr
         vars = []
-        print("INCLUDE_NULL:", include_null)
         for field in self.field_jsonifiers:
             name = field.name
             value = getter(__data, name, None)
             if value is None:
                 if include_null:
                     vars.append(value)
             else:
```

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/maps/util.py` & `asyncpgdb-0.0.3/asyncpgdb/types/maps/util.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc` & `asyncpgdb-0.0.3/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/sql/metadata.py` & `asyncpgdb-0.0.3/asyncpgdb/types/sql/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             columns.append(column_sql)
 
         columns = ",\n".join(columns)
 
         while ",," in columns:
             columns = columns.replace(",,", ",")
         result = cls(f"CREATE TABLE IF NOT EXISTS {table.name} (\n{columns}\n);")
-        print("RESULT:", result)
+
         return result
 
 
 class DropTableSQL(str):
     @classmethod
     def parse_table(cls, table):
         return cls(f"DROP TABLE IF EXISTS {table.name};")
```

### Comparing `asyncpgdb-0.0.2/asyncpgdb/types/sql/stmt.py` & `asyncpgdb-0.0.3/asyncpgdb/types/sql/stmt.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,18 +54,18 @@
                 result = self.dtype.row2dict_serializer()
             else:
                 result = self.dtype.row2schema_serializer()
         else:
             result = None
         return result
 
-    def format_vars(self, vars: Union[list[dict], list[SomeSchema]]):
+    def format_vars(self, vars: Union[list[dict], list[SomeSchema]],include_null:bool=True):
         if self.dtype:
 
-            result = self.dtype.format_upsert_vars(vars=vars)
+            result = self.dtype.format_upsert_vars(vars=vars,include_null=include_null)
         else:
             print("UNABLE TO FORMAT VARS: UNKNOWN DTYPE:")
             result = vars
         return result
 
 
 def select(
```

### Comparing `asyncpgdb-0.0.2/PKG-INFO` & `asyncpgdb-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpgdb
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: wayfaring-stranger
 Author-email: zw6p226m@duck.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

