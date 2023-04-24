# Comparing `tmp/questdb-connect-0.0.7.tar.gz` & `tmp/questdb-connect-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.7.tar", last modified: Mon Apr 24 13:53:37 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.8.tar", last modified: Mon Apr 24 14:09:27 2023, max compression
```

## Comparing `questdb-connect-0.0.7.tar` & `questdb-connect-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.795666 questdb-connect-0.0.7/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.7/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 13:53:37.795520 questdb-connect-0.0.7/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.7/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 13:52:45.000000 questdb-connect-0.0.7/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 13:53:37.795702 questdb-connect-0.0.7/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.791257 questdb-connect-0.0.7/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.793516 questdb-connect-0.0.7/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.7/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    13236 2023-04-24 13:52:45.000000 questdb-connect-0.0.7/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     8794 2023-04-24 13:52:45.000000 questdb-connect-0.0.7/src/questdb_connect/superset.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.795017 questdb-connect-0.0.7/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 13:53:37.000000 questdb-connect-0.0.7/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 13:53:37.795151 questdb-connect-0.0.7/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.7/tests/test_dialect.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.504159 questdb-connect-0.0.8/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.8/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 14:09:27.504013 questdb-connect-0.0.8/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.8/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2338 2023-04-24 14:09:05.000000 questdb-connect-0.0.8/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 14:09:27.504195 questdb-connect-0.0.8/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.500859 questdb-connect-0.0.8/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.502544 questdb-connect-0.0.8/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.8/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13236 2023-04-24 13:52:45.000000 questdb-connect-0.0.8/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9115 2023-04-24 14:08:46.000000 questdb-connect-0.0.8/src/questdb_connect/superset.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.503527 questdb-connect-0.0.8/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4002 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 14:09:27.000000 questdb-connect-0.0.8/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 14:09:27.503667 questdb-connect-0.0.8/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.8/tests/test_dialect.py
```

### Comparing `questdb-connect-0.0.7/LICENSE` & `questdb-connect-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.7/PKG-INFO` & `questdb-connect-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.7
+Version: 0.0.8
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.7/README.md` & `questdb-connect-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.7/pyproject.toml` & `questdb-connect-0.0.8/pyproject.toml`

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
-version = "0.0.7"
+version = "0.0.8"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.7/src/questdb_connect/__init__.py` & `questdb-connect-0.0.8/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.7/src/questdb_connect/dialect.py` & `questdb-connect-0.0.8/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.7/src/questdb_connect/superset.py` & `questdb-connect-0.0.8/src/questdb_connect/superset.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,14 +222,23 @@
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if target_type.upper() == 'DATETIME':
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
+    def get_datatype(cls, type_code: Any) -> Optional[str]:
+        """
+        Change column type code from cursor description to string representation.
+        :param type_code: Type code from cursor description
+        :return: String representation of type code
+        """
+        return type_code
+
+    @classmethod
     def get_column_spec(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
     ) -> Optional[utils.ColumnSpec]:
         """Get generic type related specs regarding a native column type.
```

### Comparing `questdb-connect-0.0.7/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.8/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.7
+Version: 0.0.8
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.7/tests/test_dialect.py` & `questdb-connect-0.0.8/tests/test_dialect.py`

 * *Files identical despite different names*

