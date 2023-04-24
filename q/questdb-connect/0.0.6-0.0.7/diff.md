# Comparing `tmp/questdb-connect-0.0.6.tar.gz` & `tmp/questdb-connect-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.6.tar", last modified: Mon Apr 24 13:45:29 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.7.tar", last modified: Mon Apr 24 13:53:37 2023, max compression
```

## Comparing `questdb-connect-0.0.6.tar` & `questdb-connect-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:45:29.446885 questdb-connect-0.0.6/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.6/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 13:45:29.446723 questdb-connect-0.0.6/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.6/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 13:41:26.000000 questdb-connect-0.0.6/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 13:45:29.446930 questdb-connect-0.0.6/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:45:29.444267 questdb-connect-0.0.6/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:45:29.445392 questdb-connect-0.0.6/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.6/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    13202 2023-04-24 13:39:58.000000 questdb-connect-0.0.6/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     8702 2023-04-24 13:44:24.000000 questdb-connect-0.0.6/src/questdb_connect/superset.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:45:29.446201 questdb-connect-0.0.6/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 13:45:29.000000 questdb-connect-0.0.6/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 13:45:29.000000 questdb-connect-0.0.6/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 13:45:29.000000 questdb-connect-0.0.6/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 13:45:29.000000 questdb-connect-0.0.6/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 13:45:29.000000 questdb-connect-0.0.6/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 13:45:29.000000 questdb-connect-0.0.6/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:45:29.446321 questdb-connect-0.0.6/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.6/tests/test_dialect.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.795666 questdb-connect-0.0.7/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.7/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 13:53:37.795520 questdb-connect-0.0.7/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.7/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 13:52:45.000000 questdb-connect-0.0.7/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 13:53:37.795702 questdb-connect-0.0.7/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.791257 questdb-connect-0.0.7/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.793516 questdb-connect-0.0.7/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.7/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13236 2023-04-24 13:52:45.000000 questdb-connect-0.0.7/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     8794 2023-04-24 13:52:45.000000 questdb-connect-0.0.7/src/questdb_connect/superset.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.795017 questdb-connect-0.0.7/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.795151 questdb-connect-0.0.7/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.7/tests/test_dialect.py
```

### Comparing `questdb-connect-0.0.6/LICENSE` & `questdb-connect-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.6/PKG-INFO` & `questdb-connect-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.6
+Version: 0.0.7
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.6/README.md` & `questdb-connect-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.6/pyproject.toml` & `questdb-connect-0.0.7/pyproject.toml`

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
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.6/src/questdb_connect/__init__.py` & `questdb-connect-0.0.7/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.6/src/questdb_connect/dialect.py` & `questdb-connect-0.0.7/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 
     return GeohashWithPrecision
 
 
 def resolve_type_from_name(type_name):
     if not type_name:
         return None
+    print(f'PAZUZU: {type_name}')
     name_u = type_name.upper()
     qdbc_type = None
     if name_u == 'BOOLEAN':
         qdbc_type = Boolean
     elif name_u == 'BYTE':
         qdbc_type = Byte
     elif name_u == 'SHORT':
```

### Comparing `questdb-connect-0.0.6/src/questdb_connect/superset.py` & `questdb-connect-0.0.7/src/questdb_connect/superset.py`

 * *Files 5% similar despite different names*

```diff
@@ -236,14 +236,15 @@
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         if not native_type:
             return None
+        print(f'ULANKA native_type: {native_type}, source: {source}, db_extra: {db_extra}')
         sqla_type = qdbcd.resolve_type_from_name(native_type)
         name_u = sqla_type.__visit_name__.upper()
         generic_type = None
         if name_u == 'BOOLEAN':
             generic_type = GenericDataType.BOOLEAN
         elif name_u in ('BYTE', 'SHORT', 'INT', 'INTEGER', 'LONG', 'FLOAT', 'DOUBLE'):
             generic_type = GenericDataType.NUMERIC
```

### Comparing `questdb-connect-0.0.6/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.7/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.6
+Version: 0.0.7
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.6/tests/test_dialect.py` & `questdb-connect-0.0.7/tests/test_dialect.py`

 * *Files identical despite different names*

