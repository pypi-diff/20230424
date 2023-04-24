# Comparing `tmp/databricks_sql_cli-0.3.0.tar.gz` & `tmp/databricks_sql_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_cli-0.3.0.tar", max compression
+gzip compressed data, was "databricks_sql_cli-0.3.1.tar", max compression
```

## Comparing `databricks_sql_cli-0.3.0.tar` & `databricks_sql_cli-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     3466 2023-03-31 18:09:19.470524 databricks_sql_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0     3512 2023-03-31 18:09:19.470524 databricks_sql_cli-0.3.0/README.md
--rw-r--r--   0        0        0       22 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/__init__.py
--rw-r--r--   0        0        0     1256 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/clibuffer.py
--rw-r--r--   0        0        0     4681 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/clistyle.py
--rw-r--r--   0        0        0     1504 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/clitoolbar.py
--rw-r--r--   0        0        0      137 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/compat.py
--rw-r--r--   0        0        0    15034 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/completer.py
--rw-r--r--   0        0        0     4332 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/completion_refresher.py
--rw-r--r--   0        0        0     2085 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/config.py
--rw-r--r--   0        0        0     3298 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/dbsqlclirc
--rw-r--r--   0        0        0     2254 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/key_bindings.py
--rw-r--r--   0        0        0      288 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/lexer.py
--rw-r--r--   0        0        0    26041 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/main.py
--rw-r--r--   0        0        0        0 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/__init__.py
--rw-r--r--   0        0        0    12639 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/completion_engine.py
--rw-r--r--   0        0        0     1713 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/filepaths.py
--rw-r--r--   0        0        0      892 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/format_utils.py
--rw-r--r--   0        0        0        0 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/literals/__init__.py
--rw-r--r--   0        0        0    10151 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/literals/main.py
--rw-r--r--   0        0        0     7976 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/parseutils.py
--rw-r--r--   0        0        0     1065 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/prompt_utils.py
--rw-r--r--   0        0        0      247 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/special/__init__.py
--rw-r--r--   0        0        0     1198 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/special/dbcommands.py
--rw-r--r--   0        0        0     2093 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/special/favoritequeries.py
--rw-r--r--   0        0        0    14399 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/special/iocommands.py
--rw-r--r--   0        0        0     4228 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/special/main.py
--rw-r--r--   0        0        0     1440 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/special/utils.py
--rw-r--r--   0        0        0        0 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/tabular_output/__init__.py
--rw-r--r--   0        0        0     1935 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/packages/tabular_output/sql_format.py
--rw-r--r--   0        0        0     6734 2023-03-31 18:09:19.486524 databricks_sql_cli-0.3.0/dbsqlcli/sqlexecute.py
--rw-r--r--   0        0        0      867 2023-03-31 18:09:44.739257 databricks_sql_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4585 1970-01-01 00:00:00.000000 databricks_sql_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3466 2023-04-24 20:44:11.649621 databricks_sql_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3512 2023-04-24 20:44:11.649621 databricks_sql_cli-0.3.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/__init__.py
+-rw-r--r--   0        0        0     1256 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/clibuffer.py
+-rw-r--r--   0        0        0     4681 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/clistyle.py
+-rw-r--r--   0        0        0     1504 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/clitoolbar.py
+-rw-r--r--   0        0        0      137 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/compat.py
+-rw-r--r--   0        0        0    15034 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/completer.py
+-rw-r--r--   0        0        0     4332 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/completion_refresher.py
+-rw-r--r--   0        0        0     2085 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/config.py
+-rw-r--r--   0        0        0     3298 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/dbsqlclirc
+-rw-r--r--   0        0        0     2254 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/key_bindings.py
+-rw-r--r--   0        0        0      288 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/lexer.py
+-rw-r--r--   0        0        0    26041 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/main.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/__init__.py
+-rw-r--r--   0        0        0    12595 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/completion_engine.py
+-rw-r--r--   0        0        0     1713 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/filepaths.py
+-rw-r--r--   0        0        0      892 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/format_utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/literals/__init__.py
+-rw-r--r--   0        0        0    10151 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/literals/main.py
+-rw-r--r--   0        0        0     7976 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/parseutils.py
+-rw-r--r--   0        0        0     1065 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/prompt_utils.py
+-rw-r--r--   0        0        0      247 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-24 20:44:11.665621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/dbcommands.py
+-rw-r--r--   0        0        0     2093 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/favoritequeries.py
+-rw-r--r--   0        0        0    14399 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/iocommands.py
+-rw-r--r--   0        0        0     4228 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/main.py
+-rw-r--r--   0        0        0     1440 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/special/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/tabular_output/__init__.py
+-rw-r--r--   0        0        0     1935 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/packages/tabular_output/sql_format.py
+-rw-r--r--   0        0        0     6734 2023-04-24 20:44:11.669621 databricks_sql_cli-0.3.1/dbsqlcli/sqlexecute.py
+-rw-r--r--   0        0        0      867 2023-04-24 20:44:37.525833 databricks_sql_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4585 1970-01-01 00:00:00.000000 databricks_sql_cli-0.3.1/PKG-INFO
```

### Comparing `databricks_sql_cli-0.3.0/LICENSE` & `databricks_sql_cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/README.md` & `databricks_sql_cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/clibuffer.py` & `databricks_sql_cli-0.3.1/dbsqlcli/clibuffer.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/clistyle.py` & `databricks_sql_cli-0.3.1/dbsqlcli/clistyle.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/clitoolbar.py` & `databricks_sql_cli-0.3.1/dbsqlcli/clitoolbar.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/completer.py` & `databricks_sql_cli-0.3.1/dbsqlcli/completer.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/completion_refresher.py` & `databricks_sql_cli-0.3.1/dbsqlcli/completion_refresher.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/config.py` & `databricks_sql_cli-0.3.1/dbsqlcli/config.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/dbsqlclirc` & `databricks_sql_cli-0.3.1/dbsqlcli/dbsqlclirc`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/key_bindings.py` & `databricks_sql_cli-0.3.1/dbsqlcli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/main.py` & `databricks_sql_cli-0.3.1/dbsqlcli/main.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/completion_engine.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/completion_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import sys
 import sqlparse
 import logging
 from collections import namedtuple
 from sqlparse.sql import Comparison, Identifier, Where
-from sqlparse.compat import text_type
 
 from dbsqlcli.packages.parseutils import last_word, extract_tables, find_prev_keyword
 from dbsqlcli.packages.special import parse_special_command
 
 _logger = logging.getLogger(__name__)
 
 Column = namedtuple("Column", ["tables", "drop_unique"])
@@ -74,15 +73,15 @@
         # Multiple statements being edited -- isolate the current one by
         # cumulatively summing statement lengths to find the one that bounds the
         # current position
         current_pos = len(text_before_cursor)
         stmt_start, stmt_end = 0, 0
 
         for statement in parsed:
-            stmt_len = len(text_type(statement))
+            stmt_len = len(str(statement))
             stmt_start, stmt_end = stmt_end, stmt_end + stmt_len
 
             if stmt_end >= current_pos:
                 text_before_cursor = full_text[stmt_start:current_pos]
                 full_text = full_text[stmt_start:]
                 break
```

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/filepaths.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/filepaths.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/format_utils.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/format_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/literals/main.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/literals/main.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/parseutils.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/parseutils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/prompt_utils.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/special/dbcommands.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/dbcommands.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/special/favoritequeries.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/favoritequeries.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/special/iocommands.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/iocommands.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/special/main.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/main.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/special/utils.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/special/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/packages/tabular_output/sql_format.py` & `databricks_sql_cli-0.3.1/dbsqlcli/packages/tabular_output/sql_format.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/dbsqlcli/sqlexecute.py` & `databricks_sql_cli-0.3.1/dbsqlcli/sqlexecute.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_cli-0.3.0/pyproject.toml` & `databricks_sql_cli-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = "A DBCLI client for Databricks SQL"
 authors = ["Databricks SQL CLI Maintainers <dbsqlcli-maintainers@databricks.com>"]
 packages = [{include = "dbsqlcli"}]
 readme = "README.md"
 license = "proprietary"
 
 [tool.poetry.dependencies]
```

### Comparing `databricks_sql_cli-0.3.0/PKG-INFO` & `databricks_sql_cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: A DBCLI client for Databricks SQL
 License: Proprietary
 Author: Databricks SQL CLI Maintainers
 Author-email: dbsqlcli-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

