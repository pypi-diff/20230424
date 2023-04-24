# Comparing `tmp/questdb-connect-0.0.4.tar.gz` & `tmp/questdb-connect-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.4.tar", last modified: Thu Apr 20 14:54:48 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.5.tar", last modified: Mon Apr 24 12:38:21 2023, max compression
```

## Comparing `questdb-connect-0.0.4.tar` & `questdb-connect-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-20 14:54:48.060020 questdb-connect-0.0.4/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.4/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-20 14:54:48.059844 questdb-connect-0.0.4/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-20 14:49:19.000000 questdb-connect-0.0.4/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2299 2023-04-20 14:54:25.000000 questdb-connect-0.0.4/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-20 14:54:48.060063 questdb-connect-0.0.4/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-20 14:54:48.055889 questdb-connect-0.0.4/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-20 14:54:48.058004 questdb-connect-0.0.4/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1284 2023-04-20 14:43:59.000000 questdb-connect-0.0.4/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     8853 2023-04-20 14:47:52.000000 questdb-connect-0.0.4/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     7378 2023-04-20 14:48:27.000000 questdb-connect-0.0.4/src/questdb_connect/superset.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-20 14:54:48.059279 questdb-connect-0.0.4/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-20 14:54:48.000000 questdb-connect-0.0.4/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-20 14:54:48.000000 questdb-connect-0.0.4/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-20 14:54:48.000000 questdb-connect-0.0.4/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-20 14:54:48.000000 questdb-connect-0.0.4/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-20 14:54:48.000000 questdb-connect-0.0.4/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-20 14:54:48.000000 questdb-connect-0.0.4/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-20 14:54:48.059428 questdb-connect-0.0.4/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     7989 2023-04-19 11:08:53.000000 questdb-connect-0.0.4/tests/test_dialect.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 12:38:21.437837 questdb-connect-0.0.5/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.5/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 12:38:21.437713 questdb-connect-0.0.5/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-20 14:49:19.000000 questdb-connect-0.0.5/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 12:36:29.000000 questdb-connect-0.0.5/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 12:38:21.437872 questdb-connect-0.0.5/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 12:38:21.435068 questdb-connect-0.0.5/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 12:38:21.436350 questdb-connect-0.0.5/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.5/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13177 2023-04-24 11:54:45.000000 questdb-connect-0.0.5/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7220 2023-04-24 11:48:04.000000 questdb-connect-0.0.5/src/questdb_connect/superset.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 12:38:21.437240 questdb-connect-0.0.5/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 12:38:21.000000 questdb-connect-0.0.5/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 12:38:21.000000 questdb-connect-0.0.5/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 12:38:21.000000 questdb-connect-0.0.5/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 12:38:21.000000 questdb-connect-0.0.5/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 12:38:21.000000 questdb-connect-0.0.5/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 12:38:21.000000 questdb-connect-0.0.5/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 12:38:21.437362 questdb-connect-0.0.5/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.5/tests/test_dialect.py
```

### Comparing `questdb-connect-0.0.4/LICENSE` & `questdb-connect-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.4/PKG-INFO` & `questdb-connect-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.4
+Version: 0.0.5
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.4/README.md` & `questdb-connect-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.4/pyproject.toml` & `questdb-connect-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -66,9 +66,13 @@
     ".pytest_cache",
     ".questdb_data",
     ".git",
     ".ruff_cache",
     "venv",
     "questdb_connect.egg-info",
 ]
+
+[tool.ruff.pylint]
+max-branches = 20
+
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
```

### Comparing `questdb-connect-0.0.4/src/questdb_connect/__init__.py` & `questdb-connect-0.0.5/src/questdb_connect/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 # ===== DBAPI =====
 
 apilevel = '2.0'
 threadsafety = 2
 paramstyle = 'pyformat'
 
 
+class Error(Exception):
+    pass
+
+
 def connect(**kwargs):
     host = kwargs.get('host') or '127.0.0.1'
     port = kwargs.get('port') or 8812
     user = kwargs.get('username') or 'admin'
     passwd = kwargs.get('password') or 'quest'
     database = kwargs.get('database') or 'main'
     return psycopg2.connect(host=host, port=port, user=user, password=passwd, database=database)
```

### Comparing `questdb-connect-0.0.4/src/questdb_connect/dialect.py` & `questdb-connect-0.0.5/src/questdb_connect/dialect.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,134 +21,190 @@
 #  limitations under the License.
 #
 import abc
 import enum
 
 import sqlalchemy as sqla
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
+from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.exc import ArgumentError
+from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
+from sqlalchemy.sql.visitors import Traversible
 
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
+# ===== SQLAlchemy Dialect ======
+
+def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
+    return f'questdb://{username}:{password}@{host}:{port}/{database}'
+
+
+def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
+    return sqla.create_engine(connection_uri(host, port, username, password, database))
+
+
 # ===== QUESTDB PARTITION TYPE =====
 
 class PartitionBy(enum.Enum):
     DAY = 0
     MONTH = 1
     YEAR = 2
     NONE = 3
     HOUR = 4
     WEEK = 5
 
 
 # ===== QUESTDB DATA TYPES =====
 
-class QDBType:
+class QDBTypeMixin:
     """Base class for all questdb_connect types"""
     __visit_name__ = 'QuestDBType'
 
     def column_spec(self, column_name: str):
         return f"'{column_name}' {self.__visit_name__}"
 
 
-class Boolean(sqla.Boolean, QDBType):
+class Boolean(sqla.Boolean, QDBTypeMixin):
     __visit_name__ = 'BOOLEAN'
 
 
-class Byte(sqla.Integer, QDBType):
+class Byte(sqla.Integer, QDBTypeMixin):
     __visit_name__ = 'BYTE'
 
 
-class Short(sqla.Integer, QDBType):
+class Short(sqla.Integer, QDBTypeMixin):
     __visit_name__ = 'SHORT'
 
 
-class Int(sqla.Integer, QDBType):
+class Int(sqla.Integer, QDBTypeMixin):
     __visit_name__ = 'INT'
 
 
 class Integer(Int):
     pass
 
 
-class Long(sqla.Integer, QDBType):
+class Long(sqla.Integer, QDBTypeMixin):
     __visit_name__ = 'LONG'
 
 
-class Float(sqla.Float, QDBType):
+class Float(sqla.Float, QDBTypeMixin):
     __visit_name__ = 'FLOAT'
 
 
-class Double(sqla.Float, QDBType):
+class Double(sqla.Float, QDBTypeMixin):
     __visit_name__ = 'DOUBLE'
 
 
-class Symbol(sqla.String, QDBType):
+class Symbol(sqla.String, QDBTypeMixin):
     __visit_name__ = 'SYMBOL'
 
 
-class String(sqla.String, QDBType):
+class String(sqla.String, QDBTypeMixin):
     __visit_name__ = 'STRING'
 
 
-class Char(sqla.String, QDBType):
+class Char(sqla.String, QDBTypeMixin):
     __visit_name__ = 'CHAR'
 
 
-class Long256(sqla.String, QDBType):
+class Long256(sqla.String, QDBTypeMixin):
     __visit_name__ = 'LONG256'
 
 
-class UUID(sqla.String, QDBType):
+class UUID(sqla.String, QDBTypeMixin):
     __visit_name__ = 'UUID'
 
 
-class Date(sqla.Date, QDBType):
+class Date(sqla.Date, QDBTypeMixin):
     __visit_name__ = 'DATE'
 
 
-class Timestamp(sqla.DateTime, QDBType):
+class Timestamp(sqla.DateTime, QDBTypeMixin):
     __visit_name__ = 'TIMESTAMP'
 
 
 _GEOHASH_MAX_BITS = 60
 
 
 def geohash_type(bits: int):
     """Factory for Geohash(<bits>b) types"""
     if not isinstance(bits, int) or bits < 0 or bits > _GEOHASH_MAX_BITS:
         raise AttributeError(f'bits should be of type int [0, {_GEOHASH_MAX_BITS}]')
 
-    class GeohashWithPrecision(sqla.String, QDBType):
+    class GeohashWithPrecision(sqla.String, QDBTypeMixin):
         __visit_name__ = f'GEOHASH({bits}b)'
         bit_precision = bits
 
     return GeohashWithPrecision
 
 
-# ===== SQLAlchemy Dialect ======
-
-def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
-    return f'questdb://{username}:{password}@{host}:{port}/{database}'
-
+def resolve_type_from_name(type_name):
+    if not type_name:
+        return None
+    name_u = type_name.upper()
+    qdbc_type = None
+    if name_u == 'BOOLEAN':
+        qdbc_type = Boolean
+    elif name_u == 'BYTE':
+        qdbc_type = Byte
+    elif name_u == 'SHORT':
+        qdbc_type = Short
+    elif name_u == 'INT' or name_u == 'INTEGER':
+        qdbc_type = Int
+    elif name_u == 'LONG':
+        qdbc_type = Long
+    elif name_u == 'FLOAT':
+        qdbc_type = Float
+    elif name_u == 'DOUBLE':
+        qdbc_type = Double
+    elif name_u == 'SYMBOL':
+        qdbc_type = Symbol
+    elif name_u == 'STRING':
+        qdbc_type = String
+    elif name_u == 'TEXT':
+        qdbc_type = String
+    elif name_u == 'VARCHAR':
+        qdbc_type = String
+    elif name_u == 'CHAR':
+        qdbc_type = Char
+    elif name_u == 'LONG256':
+        qdbc_type = Long256
+    elif name_u == 'UUID':
+        qdbc_type = UUID
+    elif name_u == 'DATE':
+        qdbc_type = Date
+    elif name_u == 'TIMESTAMP':
+        qdbc_type = Timestamp
+    elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+        open_p = name_u.index('(')
+        close_p = name_u.index(')')
+        description = name_u[open_p + 1:close_p]
+        bits = int(description[:-1])
+        if description[-1].upper() == 'C':
+            bits *= 5
+        qdbc_type = geohash_type(bits)
+    return qdbc_type
 
-def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
-    return sqla.create_engine(connection_uri(host, port, username, password, database))
 
+# ===== QUESTDB ENGINE =====
 
-class QDBEngine(SchemaEventTarget):
+class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
+            table_name: str,
             ts_col_name: str = None,
             partition_by: PartitionBy = PartitionBy.DAY,
             is_wal: bool = True
     ):
+        Traversible.__init__(self)
+        self.name = table_name
         self.ts_col_name = ts_col_name
         self.partition_by = partition_by
         self.is_wal = is_wal
         self.compiled = None
 
     def get_table_suffix(self):
         if self.compiled is None:
@@ -170,14 +226,17 @@
                     self.compiled += ' BYPASS WAL'
         return self.compiled
 
     def _set_parent(self, parent, **_kwargs):
         parent.engine = self
 
 
+# ===== QUESTDB DIALECT TYPES =====
+
+
 _QUOTES = ("'", '"')
 
 
 def _quote_identifier(identifier: str):
     if not identifier:
         return None
     first = 0
@@ -207,41 +266,108 @@
     def visit_create_table(self, create, **kw):
         table = create.element
         create_table = f"CREATE TABLE '{table.fullname}' ("
         create_table += ', '.join([self.get_column_specification(c.element) for c in create.columns])
         return create_table + ') ' + table.engine.get_table_suffix()
 
     def get_column_specification(self, column: sqla.Column, **_):
-        if not isinstance(column.type, QDBType):
+        if not isinstance(column.type, QDBTypeMixin):
             raise ArgumentError('Column type is not a valid QuestDB type')
         return column.type.column_spec(column.name)
 
 
 class QDBSQLCompiler(SQLCompiler):
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
 
+class QDBInspector(Inspector):
+    def reflecttable(
+            self,
+            table,
+            include_columns,
+            exclude_columns=(),
+            resolve_fks=True,
+            _extend_on=None,
+    ):
+        # backward compatibility SQLAlchemy 1.3
+        return self.reflect_table(table, include_columns, exclude_columns, resolve_fks, _extend_on)
+
+    def reflect_table(
+            self,
+            table,
+            include_columns=None,
+            exclude_columns=None,
+            resolve_fks=False,
+            _extend_on=None,
+    ):
+        table_name = table.name
+        result_set = self.bind.execute(f"tables() WHERE name = '{table_name}'")
+        if not result_set:
+            raise NoResultFound(f"Table '{table_name}' does not exist")
+        table_attrs = result_set.first()
+        col_ts_name = table_attrs['designatedTimestamp']
+        partition_by = PartitionBy[table_attrs['partitionBy']]
+        is_wal = table_attrs['walEnabled'] == True
+        for row in self.bind.execute(f"table_columns('{table_name}')"):
+            col_name = row[0]
+            if include_columns and col_name not in include_columns:
+                continue
+            if exclude_columns and col_name in exclude_columns:
+                continue
+            col_type = resolve_type_from_name(row[1])
+            if col_ts_name and col_ts_name.upper() == col_name.upper():
+                table.append_column(sqla.Column(col_name, col_type, primary_key=True))
+            else:
+                table.append_column(sqla.Column(col_name, col_type))
+        table.engine = QDBTableEngine(table_name, col_ts_name, partition_by, is_wal)
+        table.metadata = sqla.MetaData()
+
+    def get_columns(self, table_name, schema=None, **kw):
+        result_set = self.bind.execute(f"table_columns('{table_name}')")
+        if not result_set:
+            raise NoResultFound(f"Table '{table_name}' does not exist")
+        return [{
+            'name': row[0],
+            'type': resolve_type_from_name(row[1]),
+            'nullable': True,
+            'autoincrement': False,
+            'persisted': True
+        } for row in result_set]
+
+
+# class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
 class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
     type_compiler = GenericTypeCompiler
+    inspector = QDBInspector
     preparer = QDBIdentifierPreparer
     supports_schemas = False
     supports_statement_cache = False
     supports_server_side_cursors = False
     supports_views = False
     supports_empty_insert = False
     supports_multivalues_insert = True
+    supports_comments = True
     inline_comments = False
     postfetch_lastrowid = False
+    non_native_boolean_check_constraint = False
     max_identifier_length = 255
+    _user_defined_max_identifier_length = 255
+    supports_multivalues_insert = True
+    supports_is_distinct_from = False
+
+    @classmethod
+    def dbapi(cls):
+        import questdb_connect as dbapi
+        return dbapi
 
     def get_schema_names(self, connection, **kw):
         return ['public']
 
     def get_table_names(self, connection, schema=None, **kw):
         return [row.table for row in connection.execute(sqla.text('SHOW TABLES'))]
```

### Comparing `questdb-connect-0.0.4/src/questdb_connect/superset.py` & `questdb-connect-0.0.5/src/questdb_connect/superset.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,39 +21,37 @@
 #  limitations under the License.
 #
 import logging
 import re
 from datetime import datetime
 from typing import Dict, Optional
 
-from superset.db_engine_specs.base import BasicParametersMixin, BasicParametersType
-from superset.db_engine_specs.postgres import PostgresBaseEngineSpec
+from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
 from superset.utils.core import GenericDataType
 
 import questdb_connect as qdbc
 from questdb_connect.dialect import connection_uri
 
 logger = logging.getLogger(__name__)
 
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
-class QDBEngineSpec(PostgresBaseEngineSpec, BasicParametersMixin):
+class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
-    engine_aliases = {}
-    # https://www.postgresql.org/docs/9.1/libpq-ssl.html#LIBQ-SSL-CERTIFICATES
     encryption_parameters = {"sslmode": "require"}
-    max_column_name_length = 250
+    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
     time_secondary_columns = True
+    max_column_name_length = 120
     _time_grain_expressions = {
         None: '{col}',
         'PT1S': "date_trunc('second', {col})",
         'PT5S': "date_trunc('second', {col}) + 5000000",
         'PT30S': "date_trunc('second', {col}) + 30000000",
         'PT1M': "date_trunc('minute', {col})",
         'PT5M': "date_trunc('minute', {col}) + 300000000",
@@ -195,28 +193,25 @@
             GenericDataType.TEMPORAL,
         ),
         (
             re.compile(r"^date", re.IGNORECASE),
             qdbc.Date(),
             GenericDataType.TEMPORAL,
         ),
-
     )
 
-    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
-
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
         return connection_uri(
-            parameters["host"],
-            int(parameters["port"]),
+            parameters.get("host"),
+            int(parameters.get("port")),
             parameters.get("username"),
             parameters.get("password"),
             parameters.get("database"))
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
         return '{col} * 1000'
```

### Comparing `questdb-connect-0.0.4/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.5/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.4
+Version: 0.0.5
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.4/tests/test_dialect.py` & `questdb-connect-0.0.5/tests/test_dialect.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import datetime
 
+import questdb_connect.dialect as qdbc
 import sqlalchemy as sqla
 from sqlalchemy.orm import Session
 
-from tests.conftest import collect_select_all, collect_select_all_raw_connection
+from tests.conftest import TEST_TABLE_NAME, collect_select_all, collect_select_all_raw_connection
 
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
-        assert test_engine.dialect.has_table(conn, 'all_types_table', 'public')
+        assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME, 'public')
         assert not test_engine.dialect.has_table(conn, 'scorchio', 'public')
         now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
         now_date = now.date()
         expected = ("(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                     "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                     "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
                     "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
@@ -78,14 +79,62 @@
             'col_geohash': 'dfvgsj2vptwu',
             'col_long256': '0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a'
         })
         assert collect_select_all(conn, expected_rows=2) == expected
     assert collect_select_all_raw_connection(test_engine, expected_rows=2) == expected
 
 
+def test_inspect(test_engine, test_model):
+    now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
+    now_date = now.date()
+    session = Session(test_engine)
+    try:
+        session.add(test_model(
+            col_boolean=True,
+            col_byte=8,
+            col_short=12,
+            col_int=0,
+            col_long=14,
+            col_float=15.234,
+            col_double=16.88993244,
+            col_symbol='coconut',
+            col_string='banana',
+            col_char='C',
+            col_uuid='6d5eb038-63d1-4971-8484-30c16e13de5b',
+            col_date=now_date,
+            col_ts=now,
+            col_geohash='dfvgsj2vptwu',
+            col_long256='0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a'
+        ))
+        session.commit()
+    finally:
+        if session:
+            session.close()
+    metadata = sqla.MetaData()
+    table = sqla.Table(TEST_TABLE_NAME, metadata, autoload_with=test_engine)
+    table_columns = str([(col.name, col.type, col.primary_key) for col in table.columns])
+    assert table_columns == str([
+        ('col_boolean', qdbc.Boolean(), False),
+        ('col_byte', qdbc.Byte(), False),
+        ('col_short', qdbc.Short(), False),
+        ('col_int', qdbc.Int(), False),
+        ('col_long', qdbc.Long(), False),
+        ('col_float', qdbc.Float(), False),
+        ('col_double', qdbc.Double(), False),
+        ('col_symbol', qdbc.Symbol(), False),
+        ('col_string', qdbc.String(), False),
+        ('col_char', qdbc.Char(), False),
+        ('col_uuid', qdbc.UUID(), False),
+        ('col_date', qdbc.Date(), False),
+        ('col_ts', qdbc.Timestamp(), True),
+        ('col_geohash', qdbc.geohash_type(40)(), False),
+        ('col_long256', qdbc.Long256(), False)
+    ])
+
+
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
     num_rows = 3
     expected = ("(True, 8, 12, 0, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                 "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
```

