# Comparing `tmp/questdb-connect-0.0.8.tar.gz` & `tmp/questdb-connect-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.8.tar", last modified: Mon Apr 24 14:09:27 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.9.tar", last modified: Mon Apr 24 14:26:27 2023, max compression
```

## Comparing `questdb-connect-0.0.8.tar` & `questdb-connect-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.504159 questdb-connect-0.0.8/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.8/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 14:09:27.504013 questdb-connect-0.0.8/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.8/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 14:09:05.000000 questdb-connect-0.0.8/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 14:09:27.504195 questdb-connect-0.0.8/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.500859 questdb-connect-0.0.8/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.502544 questdb-connect-0.0.8/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.8/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    13236 2023-04-24 13:52:45.000000 questdb-connect-0.0.8/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     9115 2023-04-24 14:08:46.000000 questdb-connect-0.0.8/src/questdb_connect/superset.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.503527 questdb-connect-0.0.8/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.503667 questdb-connect-0.0.8/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.8/tests/test_dialect.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:26:27.839248 questdb-connect-0.0.9/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.9/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 14:26:27.839036 questdb-connect-0.0.9/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.9/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 14:22:58.000000 questdb-connect-0.0.9/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 14:26:27.839302 questdb-connect-0.0.9/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:26:27.836379 questdb-connect-0.0.9/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:26:27.837666 questdb-connect-0.0.9/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.9/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13289 2023-04-24 14:22:58.000000 questdb-connect-0.0.9/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9023 2023-04-24 14:22:58.000000 questdb-connect-0.0.9/src/questdb_connect/superset.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:26:27.838561 questdb-connect-0.0.9/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 14:26:27.000000 questdb-connect-0.0.9/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 14:26:27.000000 questdb-connect-0.0.9/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 14:26:27.000000 questdb-connect-0.0.9/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 14:26:27.000000 questdb-connect-0.0.9/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 14:26:27.000000 questdb-connect-0.0.9/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 14:26:27.000000 questdb-connect-0.0.9/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:26:27.838689 questdb-connect-0.0.9/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.9/tests/test_dialect.py
```

### Comparing `questdb-connect-0.0.8/LICENSE` & `questdb-connect-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.8/PKG-INFO` & `questdb-connect-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.8
+Version: 0.0.9
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.8/README.md` & `questdb-connect-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.8/pyproject.toml` & `questdb-connect-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.8/src/questdb_connect/__init__.py` & `questdb-connect-0.0.9/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.8/src/questdb_connect/dialect.py` & `questdb-connect-0.0.9/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
 
     return GeohashWithPrecision
 
 
 def resolve_type_from_name(type_name):
     if not type_name:
         return None
-    print(f'PAZUZU: {type_name}')
     name_u = type_name.upper()
     qdbc_type = None
     if name_u == 'BOOLEAN':
         qdbc_type = Boolean
     elif name_u == 'BYTE':
         qdbc_type = Byte
     elif name_u == 'SHORT':
@@ -183,14 +182,16 @@
         open_p = name_u.index('(')
         close_p = name_u.index(')')
         description = name_u[open_p + 1:close_p]
         bits = int(description[:-1])
         if description[-1].upper() == 'C':
             bits *= 5
         qdbc_type = geohash_type(bits)
+    if not qdbc_type:
+        raise ArgumentError(f'COCONUT.native_type: {type_name}')
     return qdbc_type() if qdbc_type else None
 
 
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
```

### Comparing `questdb-connect-0.0.8/src/questdb_connect/superset.py` & `questdb-connect-0.0.9/src/questdb_connect/superset.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,14 @@
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         if not native_type:
             return None
-        print(f'ULANKA native_type: {native_type}, source: {source}, db_extra: {db_extra}')
         sqla_type = qdbcd.resolve_type_from_name(native_type)
         name_u = sqla_type.__visit_name__.upper()
         generic_type = None
         if name_u == 'BOOLEAN':
             generic_type = GenericDataType.BOOLEAN
         elif name_u in ('BYTE', 'SHORT', 'INT', 'INTEGER', 'LONG', 'FLOAT', 'DOUBLE'):
             generic_type = GenericDataType.NUMERIC
```

### Comparing `questdb-connect-0.0.8/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.9/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.8
+Version: 0.0.9
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.8/tests/test_dialect.py` & `questdb-connect-0.0.9/tests/test_dialect.py`

 * *Files identical despite different names*

