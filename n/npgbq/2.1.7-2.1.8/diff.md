# Comparing `tmp/npgbq-2.1.7.tar.gz` & `tmp/npgbq-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npgbq-2.1.7.tar", last modified: Sat Mar 25 00:01:43 2023, max compression
+gzip compressed data, was "npgbq-2.1.8.tar", last modified: Mon Apr 24 10:57:29 2023, max compression
```

## Comparing `npgbq-2.1.7.tar` & `npgbq-2.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2023-03-25 00:01:43.107466 npgbq-2.1.7/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1062 2023-01-21 00:52:26.000000 npgbq-2.1.7/LICENSE
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1887 2023-03-25 00:01:43.107466 npgbq-2.1.7/PKG-INFO
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      954 2023-03-24 02:31:03.000000 npgbq-2.1.7/README.md
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2023-03-25 00:01:43.107466 npgbq-2.1.7/npgbq/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      653 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/__init__.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2023-03-25 00:01:43.107466 npgbq-2.1.7/npgbq/connectors/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        0 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/connectors/__init__.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     3958 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/connectors/dtype_mapper.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      461 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/connectors/mssql.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        0 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/connectors/mysql.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      367 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/connectors/postgres.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2023-03-25 00:01:43.107466 npgbq-2.1.7/npgbq/core/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        0 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/core/__init__.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     7560 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/core/helper_phone_number_th.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1240 2023-01-21 00:52:26.000000 npgbq-2.1.7/npgbq/core/log_table_schema.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)    38352 2023-03-24 23:36:47.000000 npgbq-2.1.7/npgbq/core/tools.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2023-03-25 00:01:43.107466 npgbq-2.1.7/npgbq.egg-info/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1887 2023-03-25 00:01:43.000000 npgbq-2.1.7/npgbq.egg-info/PKG-INFO
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      588 2023-03-25 00:01:43.000000 npgbq-2.1.7/npgbq.egg-info/SOURCES.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        1 2023-03-25 00:01:43.000000 npgbq-2.1.7/npgbq.egg-info/dependency_links.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      160 2023-03-25 00:01:43.000000 npgbq-2.1.7/npgbq.egg-info/requires.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        6 2023-03-25 00:01:43.000000 npgbq-2.1.7/npgbq.egg-info/top_level.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)       38 2023-03-25 00:01:43.107466 npgbq-2.1.7/setup.cfg
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1624 2023-03-24 23:35:15.000000 npgbq-2.1.7/setup.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2023-03-25 00:01:43.107466 npgbq-2.1.7/tests/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1893 2023-01-21 00:52:26.000000 npgbq-2.1.7/tests/test_insert_excel.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1628 2023-01-21 00:52:26.000000 npgbq-2.1.7/tests/test_load_scbpt_mediaperf.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     3252 2023-01-21 00:52:26.000000 npgbq-2.1.7/tests/test_load_scbpt_saleorder.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     5991 2023-01-21 00:52:26.000000 npgbq-2.1.7/tests/test_oracle_ingest.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1298 2023-01-21 00:52:26.000000 npgbq-2.1.7/tests/test_script.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.484221 npgbq-2.1.8/
+-rw-rw-rw-   0        0        0     1083 2023-04-12 05:59:51.000000 npgbq-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2771 2023-04-24 10:57:29.484221 npgbq-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2023-04-24 10:56:16.000000 npgbq-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.459718 npgbq-2.1.8/npgbq/
+-rw-rw-rw-   0        0        0      677 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.477718 npgbq-2.1.8/npgbq/connectors/
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/__init__.py
+-rw-rw-rw-   0        0        0     4052 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/dtype_mapper.py
+-rw-rw-rw-   0        0        0      475 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/mssql.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/mysql.py
+-rw-rw-rw-   0        0        0      386 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/connectors/postgres.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.480219 npgbq-2.1.8/npgbq/core/
+-rw-rw-rw-   0        0        0        0 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/core/__init__.py
+-rw-rw-rw-   0        0        0     7842 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/core/helper_phone_number_th.py
+-rw-rw-rw-   0        0        0     1298 2023-04-12 05:59:51.000000 npgbq-2.1.8/npgbq/core/log_table_schema.py
+-rw-rw-rw-   0        0        0    39415 2023-04-24 10:54:15.000000 npgbq-2.1.8/npgbq/core/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.474719 npgbq-2.1.8/npgbq.egg-info/
+-rw-rw-rw-   0        0        0     2771 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 10:57:29.000000 npgbq-2.1.8/npgbq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:57:29.484719 npgbq-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-04-24 10:54:37.000000 npgbq-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:57:29.483219 npgbq-2.1.8/tests/
+-rw-rw-rw-   0        0        0     1951 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_insert_excel.py
+-rw-rw-rw-   0        0        0     1674 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_load_scbpt_mediaperf.py
+-rw-rw-rw-   0        0        0     3342 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_load_scbpt_saleorder.py
+-rw-rw-rw-   0        0        0     6165 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_oracle_ingest.py
+-rw-rw-rw-   0        0        0     1334 2023-04-12 05:59:51.000000 npgbq-2.1.8/tests/test_script.py
```

### Comparing `npgbq-2.1.7/LICENSE` & `npgbq-2.1.8/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 NNOPP
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 NNOPP
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `npgbq-2.1.7/npgbq/__init__.py` & `npgbq-2.1.8/npgbq/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# flake8: noqa
-
-__docformat__ = "restructuredtext"
-
-# Let users know if they're missing any of our hard dependencies
-hard_dependencies = ("numpy", "pandas")
-missing_dependencies = []
-
-for dependency in hard_dependencies:
-    try:
-        __import__(dependency)
-    except ImportError as e:
-        missing_dependencies.append(f"{dependency}: {e}")
-
-if missing_dependencies:
-    raise ImportError(
-        "Unable to import required dependencies:\n"
-        + "\n".join(missing_dependencies)
-    )
-del hard_dependencies, dependency, missing_dependencies  # type: ignore
-
-# import main tool
-from npgbq import connectors
-from npgbq.core.tools import NPGBQ
+# flake8: noqa
+
+__docformat__ = "restructuredtext"
+
+# Let users know if they're missing any of our hard dependencies
+hard_dependencies = ("numpy", "pandas")
+missing_dependencies = []
+
+for dependency in hard_dependencies:
+    try:
+        __import__(dependency)
+    except ImportError as e:
+        missing_dependencies.append(f"{dependency}: {e}")
+
+if missing_dependencies:
+    raise ImportError(
+        "Unable to import required dependencies:\n"
+        + "\n".join(missing_dependencies)
+    )
+del hard_dependencies, dependency, missing_dependencies  # type: ignore
+
+# import main tool
+from npgbq import connectors
+from npgbq.core.tools import NPGBQ
```

### Comparing `npgbq-2.1.7/npgbq/connectors/dtype_mapper.py` & `npgbq-2.1.8/npgbq/connectors/dtype_mapper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-mssql_to_gbq = {
-    "bigint": "INT64",
-    "bit": "BOOL",
-    "char": "STRING",
-    "date": "DATE",
-    "datetime": "TIMESTAMP",
-    "decimal": "FLOAT64",
-    "int": "INT64",
-    "money": "FLOAT64",
-    "nchar": "STRING",
-    "numeric": "FLOAT64",
-    "nvarchar": "STRING",
-    "real": "FLOAT64",
-    "smalldatetime": "TIMESTAMP",
-    "smallint": "INT64",
-    "time": "TIME",
-    "varchar": "STRING",
-    "float": "FLOAT64",
-}
-
-mysql_to_gbq = {
-    "bigint": "INT64",
-    "bit": "BOOL",
-    "char": "STRING",
-    "date": "DATE",
-    "datetime": "TIMESTAMP",
-    "decimal": "FLOAT64",
-    "int": "INT64",
-    "money": "FLOAT64",
-    "nchar": "STRING",
-    "numeric": "FLOAT64",
-    "nvarchar": "STRING",
-    "real": "FLOAT64",
-    "smalldatetime": "TIMESTAMP",
-    "smallint": "INT64",
-    "time": "TIME",
-    "varchar": "STRING",
-    "float": "FLOAT64",
-}
-
-postgres_to_gbq = {
-    "bigint": "INT64",
-    "bit": "BOOL",
-    "char": "STRING",
-    "date": "DATE",
-    "datetime": "TIMESTAMP",
-    "decimal": "FLOAT64",
-    "int": "INT64",
-    "money": "FLOAT64",
-    "nchar": "STRING",
-    "numeric": "FLOAT64",
-    "nvarchar": "STRING",
-    "real": "FLOAT64",
-    "smalldatetime": "TIMESTAMP",
-    "smallint": "INT64",
-    "time": "TIME",
-    "varchar": "STRING",
-    "float": "FLOAT64",
-}
-
-
-oracle_to_gbq = {
-    # https://cloud.google.com/static/architecture/dw2bq/oracle/oracle-bq-sql-translation-reference.pdf
-    "VARCHAR2": "STRING",
-    "NVARCHAR2": "STRING",
-    "CHAR": "STRING",
-    "NCHAR": "STRING",
-    "CLOB": "STRING",
-    "NCLOB": "STRING",
-    # integer
-    "INTEGER": "INT64",
-    "SHORTINTEGER": "INT64",
-    "LONGINTEGER": "INT64",
-    # BigQuery does not allow user specification of custom values for precision or scale. As a result, a column in Oracle might be defined so that it has a bigger scale than BigQuery supports. Additionally, before storing a decimal number, Oracle rounds up if that number has more digits after the decimal point than are specified for the corresponding column. In BigQuery, you can implement this feature by using the ROUND() function.
-    "NUMBER": "NUMERIC",
-    # FLOAT is an exact data type, and it’s a NUMBER subtype in Oracle. In BitQuery, FLOAT64 is an approximate data type. NUMERIC is often a better match for FLOAT type in BigQuery
-    "FLOAT": "FLOAT64",
-    "BINARY_DOUBLE": "FLOAT64",
-    "BINARY_FLOAT": "FLOAT64",
-    # The LONG data type is used in earlier versions and is not suggested in new versions of Oracle Database. The BYTES data type in BigQuery can be used if it is necessary to hold LONG data in BigQuery. A better approach is putting binary objects in Cloud Storage and holding references in BigQuery.
-    "LONG": "BYTES",
-    # The BYTES data type can be used to store variable-length binary data. If this field is not queried and not used in analytics, a better option is to store binary data in Cloud Storage.
-    "BLOB": "STRING",
-    # Binary files can be stored in Cloud Storage, and the STRING data type can be used for referencing files in a BigQuery table.
-    "BFILE": "STRING",
-    "DATE": "DATE",
-    # BigQuery supports microsecond precision (10 -6 ), in comparison to Oracle, which supports precision ranging from 0 to 9. BigQuery supports a time zone region name from a TZ database and time zone offset from UTC. In BigQuery, use a manual time zone conversion to match Oracle’s TIMESTAMP WITH LOCAL TIME ZONE feature.
-    "TIMESTAMP": "TIMESTAMP",
-    # The BYTES data type can be used to store variable-length binary data. If this field is not queried and used in analytics, a LONG RAW better option is to store binary data on Cloud Storage.
-    "RAW": "BYTES",
-    "LONG RAW": "STRING",
-    # These data types are used by Oracle internally to specify unique addresses to rows in a table. Normally ROWID or UROWID fields should not be used in applications. But if this is the case, the STRING data type can be used to hold this data.
-    "ROWID": "STRING",
-}
+mssql_to_gbq = {
+    "bigint": "INT64",
+    "bit": "BOOL",
+    "char": "STRING",
+    "date": "DATE",
+    "datetime": "TIMESTAMP",
+    "decimal": "FLOAT64",
+    "int": "INT64",
+    "money": "FLOAT64",
+    "nchar": "STRING",
+    "numeric": "FLOAT64",
+    "nvarchar": "STRING",
+    "real": "FLOAT64",
+    "smalldatetime": "TIMESTAMP",
+    "smallint": "INT64",
+    "time": "TIME",
+    "varchar": "STRING",
+    "float": "FLOAT64",
+}
+
+mysql_to_gbq = {
+    "bigint": "INT64",
+    "bit": "BOOL",
+    "char": "STRING",
+    "date": "DATE",
+    "datetime": "TIMESTAMP",
+    "decimal": "FLOAT64",
+    "int": "INT64",
+    "money": "FLOAT64",
+    "nchar": "STRING",
+    "numeric": "FLOAT64",
+    "nvarchar": "STRING",
+    "real": "FLOAT64",
+    "smalldatetime": "TIMESTAMP",
+    "smallint": "INT64",
+    "time": "TIME",
+    "varchar": "STRING",
+    "float": "FLOAT64",
+}
+
+postgres_to_gbq = {
+    "bigint": "INT64",
+    "bit": "BOOL",
+    "char": "STRING",
+    "date": "DATE",
+    "datetime": "TIMESTAMP",
+    "decimal": "FLOAT64",
+    "int": "INT64",
+    "money": "FLOAT64",
+    "nchar": "STRING",
+    "numeric": "FLOAT64",
+    "nvarchar": "STRING",
+    "real": "FLOAT64",
+    "smalldatetime": "TIMESTAMP",
+    "smallint": "INT64",
+    "time": "TIME",
+    "varchar": "STRING",
+    "float": "FLOAT64",
+}
+
+
+oracle_to_gbq = {
+    # https://cloud.google.com/static/architecture/dw2bq/oracle/oracle-bq-sql-translation-reference.pdf
+    "VARCHAR2": "STRING",
+    "NVARCHAR2": "STRING",
+    "CHAR": "STRING",
+    "NCHAR": "STRING",
+    "CLOB": "STRING",
+    "NCLOB": "STRING",
+    # integer
+    "INTEGER": "INT64",
+    "SHORTINTEGER": "INT64",
+    "LONGINTEGER": "INT64",
+    # BigQuery does not allow user specification of custom values for precision or scale. As a result, a column in Oracle might be defined so that it has a bigger scale than BigQuery supports. Additionally, before storing a decimal number, Oracle rounds up if that number has more digits after the decimal point than are specified for the corresponding column. In BigQuery, you can implement this feature by using the ROUND() function.
+    "NUMBER": "NUMERIC",
+    # FLOAT is an exact data type, and it’s a NUMBER subtype in Oracle. In BitQuery, FLOAT64 is an approximate data type. NUMERIC is often a better match for FLOAT type in BigQuery
+    "FLOAT": "FLOAT64",
+    "BINARY_DOUBLE": "FLOAT64",
+    "BINARY_FLOAT": "FLOAT64",
+    # The LONG data type is used in earlier versions and is not suggested in new versions of Oracle Database. The BYTES data type in BigQuery can be used if it is necessary to hold LONG data in BigQuery. A better approach is putting binary objects in Cloud Storage and holding references in BigQuery.
+    "LONG": "BYTES",
+    # The BYTES data type can be used to store variable-length binary data. If this field is not queried and not used in analytics, a better option is to store binary data in Cloud Storage.
+    "BLOB": "STRING",
+    # Binary files can be stored in Cloud Storage, and the STRING data type can be used for referencing files in a BigQuery table.
+    "BFILE": "STRING",
+    "DATE": "DATE",
+    # BigQuery supports microsecond precision (10 -6 ), in comparison to Oracle, which supports precision ranging from 0 to 9. BigQuery supports a time zone region name from a TZ database and time zone offset from UTC. In BigQuery, use a manual time zone conversion to match Oracle’s TIMESTAMP WITH LOCAL TIME ZONE feature.
+    "TIMESTAMP": "TIMESTAMP",
+    # The BYTES data type can be used to store variable-length binary data. If this field is not queried and used in analytics, a LONG RAW better option is to store binary data on Cloud Storage.
+    "RAW": "BYTES",
+    "LONG RAW": "STRING",
+    # These data types are used by Oracle internally to specify unique addresses to rows in a table. Normally ROWID or UROWID fields should not be used in applications. But if this is the case, the STRING data type can be used to hold this data.
+    "ROWID": "STRING",
+}
```

### Comparing `npgbq-2.1.7/npgbq/core/helper_phone_number_th.py` & `npgbq-2.1.8/npgbq/core/helper_phone_number_th.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-import numpy as np
-import pandas as pd
-import re
-
-thai_area_code = {
-    "02": "Bangkok (Krung Thep Maha Nakhon), Nonthaburi, Pathum Thani, Samut Prakan, Phutthamonthon (Nakhon Pathom)",
-    "032": "Phetchaburi, Prachuap Khiri Khan, Ratchaburi",
-    "034": "Kanchanaburi, Nakhon Pathom (except Phutthamonthon), Samut Sakhon, Samut Songkhram",
-    "035": "Ang Thong, Phra Nakhon Si Ayutthaya, Suphan Buri",
-    "036": "Lop Buri, Saraburi, Sing Buri",
-    "037": "Nakhon Nayok, Prachin Buri, Sa Kaeo",
-    "038": "Chachoengsao, Chon Buri, Rayong",
-    "039": "Chanthaburi, Trat",
-    "042": "Bueng Kan, Loei, Mukdahan, Nakhon Phanom, Nong Bua Lamphu, Nong Khai, Sakon Nakhon, Udon Thani",
-    "043": "Kalasin, Khon Kaen, Maha Sarakham, Roi Et, Nam Nao (Phetchabun)",
-    "044": "Buri Ram, Chaiyaphum, Nakhon Ratchasima, Surin",
-    "045": "Amnat Charoen, Si Sa Ket, Ubon Ratchathani, Yasothon",
-    "052": "Chiang Mai, Chiang Rai, Lamphun, Mae Hong Son",
-    "053": "Chiang Mai, Chiang Rai, Lamphun, Mae Hong Son",
-    "054": "Lampang, Nan, Phayao, Phrae",
-    "055": "Kamphaeng Phet, Phitsanulok, Sukhothai, Tak, Uttaradit, Sam Ngam, Wachirabarami (Phichit)",
-    "056": "Chai Nat, Nakhon Sawan, Phetchabun (except Nam Nao), Phichit (except Sam Ngam & Wachirabarami), Uthai Thani",
-    "073": "Narathiwat, Pattani, Yala",
-    "074": "Phatthalung, Satun, Songkhla",
-    "075": "Krabi, Nakhon Si Thammarat, Trang",
-    "076": "Phang Nga, Phuket",
-    "077": "Chumphon, Ranong, Surat Thani",
-}
-
-phone_list_bkk = ["02"]
-phone_list_nonbkk = [k for k, v in thai_area_code.items() if k != "02"]
-phone_list_mobile = [
-    "060",
-    "061",
-    "062",
-    "063",
-    "064",
-    "065",
-    "066",
-    "068",
-    "080",
-    "081",
-    "082",
-    "083",
-    "084",
-    "085",
-    "086",
-    "087",
-    "088",
-    "089",
-    "090",
-    "091",
-    "092",
-    "093",
-    "094",
-    "095",
-    "096",
-    "097",
-    "098",
-    "099",
-    "099 ",
-]
-
-
-def get_possible_extension(text):
-    non_mobile = text[:9]
-    if is_bkk_office_number(non_mobile) or is_nonbkk_office_number(non_mobile):
-        ext = text[9:]
-        return ext
-    else:
-        return ""
-
-
-def prepare_phone_out(phone_no_extension, extension):
-    if len(extension) > 0:
-        return f"{phone_no_extension}-{extension}"
-    else:
-        return phone_no_extension
-
-
-def add_leading_zero(text):
-    if ((len(text) == 9) or (len(text) == 8)) and (text[0] != "0"):
-        return f"0{text}"
-    else:
-        return text
-
-
-def update_old_mobile(text):
-    leading = "08"
-    num = text[1:]
-    return f"{leading}{num}"
-
-
-def keep_only_number(text):
-    txt = re.sub("[^0-9.]+", "", text)
-    return txt
-
-
-def remove_66(txt):
-    if is_phone_with66(txt):
-        txt = txt.replace("66", "", 1)
-        return txt
-    else:
-        return txt
-
-
-def finalize_phone(text, extension):
-    num_extension = len(extension)
-    if has_extension(num_extension):
-        phone_no_extension = text[:-num_extension]
-    else:
-        phone_no_extension = text
-    if is_bkk_office_number(phone_no_extension):
-        phone_type = "office"
-        phone_num = prepare_phone_out(phone_no_extension, extension)
-    elif is_nonbkk_office_number(phone_no_extension):
-        phone_type = "office"
-        phone_num = prepare_phone_out(phone_no_extension, extension)
-    elif is_mobile_number(text):
-        phone_type = "mobile"
-        phone_num = text
-    elif is_old_mobile_number(text):
-        phone_type = "mobile"
-        phone_num = update_old_mobile(text)
-    else:
-        phone_type = "other"
-        phone_num = np.nan
-    return phone_type, phone_num
-
-
-def is_old_mobile_number(text):
-    old_nums = ["09", "01"]
-    if (text[:2] in old_nums) and (len(text) == 9):
-        return True
-    else:
-        return False
-
-
-def is_mobile_number(text):
-    if (text[:3] in phone_list_mobile) and (len(text) == 10):
-        return True
-    else:
-        return False
-
-
-def is_nonbkk_office_number(text):
-    if (text[:3] in phone_list_nonbkk) and (len(text) == 9):
-        return True
-    else:
-        return False
-
-
-def is_bkk_office_number(text):
-    if (text[:2] == "02") and (len(text) == 9):
-        return True
-    else:
-        return False
-
-
-def is_phone_with66(text):
-    if (text[:2] == "66") and (len(text) == 11):
-        return True
-    elif (text[:2] == "66") and (len(text) == 10):
-        return True
-    else:
-        return False
-
-
-def has_extension(n):
-    if n > 0:
-        return True
-    else:
-        return False
-
-
-def try_convert_as_int(x):
-    try:
-        output = str(int(float(x)))
-    except Exception as e:
-        print(f"failed to convert {x} to float>int>str")
-        return ""
-    else:
-        return output
-
-
-def format_phone(col):
-    phone_type, phone_num = "other", np.nan
-    if pd.isna(col):
-        return phone_type, phone_num
-
-    text = str(col).strip()
-    text = keep_only_number(text)
-    text = remove_66(text)
-    text = try_convert_as_int(text)
-    if len(text) < 7:
-        return phone_type, phone_num
-    text = add_leading_zero(text)
-    ext = get_possible_extension(text)
-    phone_type, phone_num = finalize_phone(text, ext)
-    return phone_type, phone_num
-
-
-if __name__ == "__main__":
-    input_val = 943350770
-    print(f"Input {input_val}",format_phone(943350770))
-    
-    input_val = "09-4597386"
-    print(f"Input {input_val}",format_phone("09-4597386"))
-    
-    input_val = "01-3636342"
-    print(f"Input {input_val}",format_phone("01-3636342"))
-    
-    input_val = "05-1622430"
-    print(f"Input {input_val}",format_phone("05-1622430"))
-
-    
-    input_val = "0231531447128"
-    print(f"Input {input_val}",format_phone("0231531447128"))
-    
-    input_val = " "
-    print(f"Input {input_val}",format_phone(" "))
-    
-    input_val = None
-    print(f"Input {input_val}",format_phone(None))
-    
-    input_val = "02-7205978-87"
-    print(f"Input {input_val}",format_phone("02-7205978-87"))
-    
-    input_val = "022482000 160"
-    print(f"Input {input_val}",format_phone("022482000 160"))
-    # bad one
-    
-    input_val = "6683ฮ091545"
-    print(f"Input {input_val}",format_phone("6683ฮ091545"))
-    # mobile
-    
-    input_val = "66830091545"
-    print(f"Input {input_val}",format_phone("66830091545"))
-    
-    input_val = "+66830091545"
-    print(f"Input {input_val}",format_phone("+66830091545"))
-    
-    input_val = "083-009-1545"
-    print(f"Input {input_val}",format_phone("083-009-1545"))
-    
-    input_val = "83-009-1545"
-    print(f"Input {input_val}",format_phone("83-009-1545"))
-    
-    input_val = "+830091545"
-    print(f"Input {input_val}",format_phone("+830091545"))
-    # bkk
-    
-    input_val = "6625377653"
-    print(f"Input {input_val}",format_phone("6625377653"))
-    
-    input_val = "+6625377653"
-    print(f"Input {input_val}",format_phone("+6625377653"))
-    
-    input_val = "02-537-7653"
-    print(f"Input {input_val}",format_phone("02-537-7653"))
-    
-    input_val = "2-537-7653"
-    print(f"Input {input_val}",format_phone("2-537-7653"))
-    
-    input_val = "+25377653"
-    print(f"Input {input_val}",format_phone("+25377653"))
-    # non-bkk
-    
-    input_val = "6635343240"
-    print(f"Input {input_val}",format_phone("6635343240"))
-    
-    input_val = "+6635343240"
-    print(f"Input {input_val}",format_phone("+6635343240"))
-    
-    input_val = "03-534-3240"
-    print(f"Input {input_val}",format_phone("03-534-3240"))
-    
-    input_val = "3-534-3240"
-    print(f"Input {input_val}",format_phone("3-534-3240"))
-    
-    input_val = "+35343240"
-    print(f"Input {input_val}",format_phone("+35343240"))
+import numpy as np
+import pandas as pd
+import re
+
+thai_area_code = {
+    "02": "Bangkok (Krung Thep Maha Nakhon), Nonthaburi, Pathum Thani, Samut Prakan, Phutthamonthon (Nakhon Pathom)",
+    "032": "Phetchaburi, Prachuap Khiri Khan, Ratchaburi",
+    "034": "Kanchanaburi, Nakhon Pathom (except Phutthamonthon), Samut Sakhon, Samut Songkhram",
+    "035": "Ang Thong, Phra Nakhon Si Ayutthaya, Suphan Buri",
+    "036": "Lop Buri, Saraburi, Sing Buri",
+    "037": "Nakhon Nayok, Prachin Buri, Sa Kaeo",
+    "038": "Chachoengsao, Chon Buri, Rayong",
+    "039": "Chanthaburi, Trat",
+    "042": "Bueng Kan, Loei, Mukdahan, Nakhon Phanom, Nong Bua Lamphu, Nong Khai, Sakon Nakhon, Udon Thani",
+    "043": "Kalasin, Khon Kaen, Maha Sarakham, Roi Et, Nam Nao (Phetchabun)",
+    "044": "Buri Ram, Chaiyaphum, Nakhon Ratchasima, Surin",
+    "045": "Amnat Charoen, Si Sa Ket, Ubon Ratchathani, Yasothon",
+    "052": "Chiang Mai, Chiang Rai, Lamphun, Mae Hong Son",
+    "053": "Chiang Mai, Chiang Rai, Lamphun, Mae Hong Son",
+    "054": "Lampang, Nan, Phayao, Phrae",
+    "055": "Kamphaeng Phet, Phitsanulok, Sukhothai, Tak, Uttaradit, Sam Ngam, Wachirabarami (Phichit)",
+    "056": "Chai Nat, Nakhon Sawan, Phetchabun (except Nam Nao), Phichit (except Sam Ngam & Wachirabarami), Uthai Thani",
+    "073": "Narathiwat, Pattani, Yala",
+    "074": "Phatthalung, Satun, Songkhla",
+    "075": "Krabi, Nakhon Si Thammarat, Trang",
+    "076": "Phang Nga, Phuket",
+    "077": "Chumphon, Ranong, Surat Thani",
+}
+
+phone_list_bkk = ["02"]
+phone_list_nonbkk = [k for k, v in thai_area_code.items() if k != "02"]
+phone_list_mobile = [
+    "060",
+    "061",
+    "062",
+    "063",
+    "064",
+    "065",
+    "066",
+    "068",
+    "080",
+    "081",
+    "082",
+    "083",
+    "084",
+    "085",
+    "086",
+    "087",
+    "088",
+    "089",
+    "090",
+    "091",
+    "092",
+    "093",
+    "094",
+    "095",
+    "096",
+    "097",
+    "098",
+    "099",
+    "099 ",
+]
+
+
+def get_possible_extension(text):
+    non_mobile = text[:9]
+    if is_bkk_office_number(non_mobile) or is_nonbkk_office_number(non_mobile):
+        ext = text[9:]
+        return ext
+    else:
+        return ""
+
+
+def prepare_phone_out(phone_no_extension, extension):
+    if len(extension) > 0:
+        return f"{phone_no_extension}-{extension}"
+    else:
+        return phone_no_extension
+
+
+def add_leading_zero(text):
+    if ((len(text) == 9) or (len(text) == 8)) and (text[0] != "0"):
+        return f"0{text}"
+    else:
+        return text
+
+
+def update_old_mobile(text):
+    leading = "08"
+    num = text[1:]
+    return f"{leading}{num}"
+
+
+def keep_only_number(text):
+    txt = re.sub("[^0-9.]+", "", text)
+    return txt
+
+
+def remove_66(txt):
+    if is_phone_with66(txt):
+        txt = txt.replace("66", "", 1)
+        return txt
+    else:
+        return txt
+
+
+def finalize_phone(text, extension):
+    num_extension = len(extension)
+    if has_extension(num_extension):
+        phone_no_extension = text[:-num_extension]
+    else:
+        phone_no_extension = text
+    if is_bkk_office_number(phone_no_extension):
+        phone_type = "office"
+        phone_num = prepare_phone_out(phone_no_extension, extension)
+    elif is_nonbkk_office_number(phone_no_extension):
+        phone_type = "office"
+        phone_num = prepare_phone_out(phone_no_extension, extension)
+    elif is_mobile_number(text):
+        phone_type = "mobile"
+        phone_num = text
+    elif is_old_mobile_number(text):
+        phone_type = "mobile"
+        phone_num = update_old_mobile(text)
+    else:
+        phone_type = "other"
+        phone_num = np.nan
+    return phone_type, phone_num
+
+
+def is_old_mobile_number(text):
+    old_nums = ["09", "01"]
+    if (text[:2] in old_nums) and (len(text) == 9):
+        return True
+    else:
+        return False
+
+
+def is_mobile_number(text):
+    if (text[:3] in phone_list_mobile) and (len(text) == 10):
+        return True
+    else:
+        return False
+
+
+def is_nonbkk_office_number(text):
+    if (text[:3] in phone_list_nonbkk) and (len(text) == 9):
+        return True
+    else:
+        return False
+
+
+def is_bkk_office_number(text):
+    if (text[:2] == "02") and (len(text) == 9):
+        return True
+    else:
+        return False
+
+
+def is_phone_with66(text):
+    if (text[:2] == "66") and (len(text) == 11):
+        return True
+    elif (text[:2] == "66") and (len(text) == 10):
+        return True
+    else:
+        return False
+
+
+def has_extension(n):
+    if n > 0:
+        return True
+    else:
+        return False
+
+
+def try_convert_as_int(x):
+    try:
+        output = str(int(float(x)))
+    except Exception as e:
+        print(f"failed to convert {x} to float>int>str")
+        return ""
+    else:
+        return output
+
+
+def format_phone(col):
+    phone_type, phone_num = "other", np.nan
+    if pd.isna(col):
+        return phone_type, phone_num
+
+    text = str(col).strip()
+    text = keep_only_number(text)
+    text = remove_66(text)
+    text = try_convert_as_int(text)
+    if len(text) < 7:
+        return phone_type, phone_num
+    text = add_leading_zero(text)
+    ext = get_possible_extension(text)
+    phone_type, phone_num = finalize_phone(text, ext)
+    return phone_type, phone_num
+
+
+if __name__ == "__main__":
+    input_val = 943350770
+    print(f"Input {input_val}",format_phone(943350770))
+    
+    input_val = "09-4597386"
+    print(f"Input {input_val}",format_phone("09-4597386"))
+    
+    input_val = "01-3636342"
+    print(f"Input {input_val}",format_phone("01-3636342"))
+    
+    input_val = "05-1622430"
+    print(f"Input {input_val}",format_phone("05-1622430"))
+
+    
+    input_val = "0231531447128"
+    print(f"Input {input_val}",format_phone("0231531447128"))
+    
+    input_val = " "
+    print(f"Input {input_val}",format_phone(" "))
+    
+    input_val = None
+    print(f"Input {input_val}",format_phone(None))
+    
+    input_val = "02-7205978-87"
+    print(f"Input {input_val}",format_phone("02-7205978-87"))
+    
+    input_val = "022482000 160"
+    print(f"Input {input_val}",format_phone("022482000 160"))
+    # bad one
+    
+    input_val = "6683ฮ091545"
+    print(f"Input {input_val}",format_phone("6683ฮ091545"))
+    # mobile
+    
+    input_val = "66830091545"
+    print(f"Input {input_val}",format_phone("66830091545"))
+    
+    input_val = "+66830091545"
+    print(f"Input {input_val}",format_phone("+66830091545"))
+    
+    input_val = "083-009-1545"
+    print(f"Input {input_val}",format_phone("083-009-1545"))
+    
+    input_val = "83-009-1545"
+    print(f"Input {input_val}",format_phone("83-009-1545"))
+    
+    input_val = "+830091545"
+    print(f"Input {input_val}",format_phone("+830091545"))
+    # bkk
+    
+    input_val = "6625377653"
+    print(f"Input {input_val}",format_phone("6625377653"))
+    
+    input_val = "+6625377653"
+    print(f"Input {input_val}",format_phone("+6625377653"))
+    
+    input_val = "02-537-7653"
+    print(f"Input {input_val}",format_phone("02-537-7653"))
+    
+    input_val = "2-537-7653"
+    print(f"Input {input_val}",format_phone("2-537-7653"))
+    
+    input_val = "+25377653"
+    print(f"Input {input_val}",format_phone("+25377653"))
+    # non-bkk
+    
+    input_val = "6635343240"
+    print(f"Input {input_val}",format_phone("6635343240"))
+    
+    input_val = "+6635343240"
+    print(f"Input {input_val}",format_phone("+6635343240"))
+    
+    input_val = "03-534-3240"
+    print(f"Input {input_val}",format_phone("03-534-3240"))
+    
+    input_val = "3-534-3240"
+    print(f"Input {input_val}",format_phone("3-534-3240"))
+    
+    input_val = "+35343240"
+    print(f"Input {input_val}",format_phone("+35343240"))
```

### Comparing `npgbq-2.1.7/npgbq/core/tools.py` & `npgbq-2.1.8/npgbq/core/tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1032 +1,1032 @@
-"""
-referencecs:
-BigQuery: https://github.com/googleapis/python-bigquery/blob/a3f4351633f006b3132d8a8625ad7921b3d57699/samples/snippets/create_table_external_hive_partitioned.py
-BgiQuery: https://github.com/googleapis/python-bigquery/blob/35627d145a41d57768f19d4392ef235928e00f72/samples/load_table_uri_parquet.py
-
-Oracle:
-- ORA-29275: partial multibyte character
-    - solution 1: `SELECT CONVERT(COLUMN NAME, 'UTF8', 'US7ASCII')` do this for all string based 
-    - solution 2: Loop through the row to find the row that has error
-    - readmore: https://stackoverflow.com/questions/37964728/biztalk-wcf-custom-raised-an-error-ora-29275-partial-multibyte-character
-
-"""
-import decimal
-import json
-import logging
-import os
-import platform
-import re
-import uuid
-from datetime import datetime
-from typing import List, Optional, Union
-
-import google.cloud.logging
-import numpy as np
-import pandas as pd
-from google.cloud import bigquery
-from pytz import timezone
-
-from npgbq.core.helper_phone_number_th import format_phone
-
-from ..connectors.dtype_mapper import oracle_to_gbq
-
-# from ..connectors.mssql import get_conn_mssql # disabled in 2.0.5
-from ..connectors.postgres import get_conn_pg
-from .log_table_schema import gbq_log_schema
-
-
-class NPGBQ(object):
-    def __init__(self, project_id, gcp_service_account_path: Optional[str] = None):
-        self.project_id = project_id
-        self.path_json_key = gcp_service_account_path
-        self.__add_environment()
-
-        # var default
-        self.__log_dataset = "data_log"
-        self.__log_table = "logs"
-        self.job_uuid = None
-        self.dataset_id = None
-        self.table_name = None
-
-        # create client
-        self.client = self.__get_bq_client()
-
-    def __add_environment(self):
-        if self.path_json_key:
-            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = self.path_json_key
-
-    def __get_bq_client(self):
-
-        client = google.cloud.logging.Client(project=self.project_id)
-        client.setup_logging(log_level=logging.INFO)
-        return bigquery.Client(self.project_id)
-
-    @staticmethod
-    def get_valid_colname(text: str):
-        val = re.sub("[^A-Za-z0-9_]+", "_", text)
-        val = NPGBQ.remove_double_underscores(val)
-        val = NPGBQ.remove_double_space(val)
-        val = val.upper().rstrip("_").lstrip("_")
-        if re.search(r"^\d", val):
-            val = f"_{val}"
-        return val
-
-    @staticmethod
-    def remove_double_space(text: str) -> str:
-        regex = re.compile(r"\s+")
-        return re.sub(regex, " ", text)
-
-    @staticmethod
-    def remove_double_underscores(text: str) -> str:
-        regex = re.compile(r"__+")
-        return re.sub(regex, "_", text)
-
-    def format_deciaml_cols(self, df, col_decimal):
-        for col in col_decimal:
-            df[col] = df[col].astype(str).map(decimal.Decimal)
-        return df
-
-    def __validate_col_type(self, col_type: str) -> bool:
-        valid_col_type = [
-            "ARRAY",
-            "BIGNUMERIC",
-            "BOOL",
-            "BOOLEAN",
-            "DATE",
-            "DATES",
-            "FLOAT",
-            "FLOAT64",
-            "GEOGRAPHY",
-            "INT64",
-            "INTEGER",
-            "INTERVAL",
-            "NUMERIC",
-            "STRING",
-            "TIME",
-            "TIMESTAMP",
-        ]
-        if col_type not in valid_col_type:
-            raise ValueError(f"the input column datatype {  col_type} is not valid")
-        return True
-
-    @staticmethod
-    def get_full_qualified_table_name(project_id, dataset_id, table_id):
-        full_qualified_id = f"{project_id}.{dataset_id}.{table_id}"
-        return full_qualified_id
-
-    def __get_full_qualified_table_name(self, dataset_id, table_id):
-        full_qualified_id = f"{self.client.project}.{dataset_id}.{table_id}"
-        return full_qualified_id
-
-    def update_schema(self, table_obj: bigquery.Table, mapping: dict, desc: str):
-        """
-        Usage:
-        table_id = "central-cto-cds-data-hub-prd.rbs_mdc.customer_entity"
-        table_obj = gbq.client.get_table(table_id)
-        mapping = {"default_billing": "INTEGER", "default_shipping": "INTEGER",'gender':'INTEGER'}
-        gbq.update_schema(table_obj, mapping)
-        """
-        schema = table_obj.schema
-        _schema = []
-        for field in schema:
-            if field.name in mapping:
-                new_field = bigquery.SchemaField(field.name, mapping[field.name], mode=field.mode, description=desc)  # type: ignore
-                _schema.append(new_field)
-            else:
-                _schema.append(field)
-        table_obj.schema = _schema
-        self.client.update_table(table_obj, ["schema"])
-        print(f"Schema updated for {table_obj.full_table_id}")
-
-    def get_col_rename_dict(self, dict_org: dict, dict_gbq: dict) -> dict:
-        res = {}
-        for (k1, v2), (k2, v2) in zip(dict_org.items(), dict_gbq.items()):
-            if k1 != k2:
-                res[k1] = k2
-        return res
-
-    def __get_db_connection(
-        self,
-        db_hostname_or_ip,
-        db_port_number,
-        db_database_name,
-        db_username,
-        db_password,
-        engine="postgres",
-    ):
-        self.log2bq(message=f"Making connection to database: {db_database_name}")
-        conn = None
-        if engine == "postgres":
-            conn = get_conn_pg(
-                db_hostname_or_ip,
-                db_port_number,
-                db_database_name,
-                db_username,
-                db_password,
-            )
-        # disabled in 2.0.5
-        # elif engine == "mssql":
-        #     conn = get_conn_mssql(
-        #         db_hostname_or_ip,
-        #         db_port_number,
-        #         db_database_name,
-        #         db_username,
-        #         db_password,
-        #     )
-        else:
-            raise NotImplementedError(
-                f"your engine {engine} is invalid please contact the administrator"
-            )
-        self.log2bq(message=f"The connection is ready: {db_database_name}")
-        return conn
-
-    # ====================================== Public method ======================================
-
-    def create_bq_dataset(self, dataset_id):
-        try:
-            dataset_id = f"{self.client.project}.{dataset_id}"
-            dataset = bigquery.Dataset(dataset_id)
-            dataset.location = "asia-southeast1"
-            dataset = self.client.create_dataset(dataset, timeout=30)
-        except Exception as e:
-            print(f"Can not create the dataset: {e}")
-        else:
-            print(f"Created dataset name {dataset_id}")
-
-    def delete_bq_dataset(self, dataset_name: str = "DATASET_ABC"):
-        # need to remove all tables from the dataset first
-        tables = self.list_tables(dataset_name)
-        for table in tables:
-            table_name = table.split(".")[-1]
-            self.delete_bq_table(dataset_name, table_name)
-        try:
-            dataset_name = f"{self.client.project}.{dataset_name}"
-            dataset = bigquery.Dataset(dataset_name)
-            dataset.location = "asia-southeast1"
-            dataset = self.client.delete_dataset(dataset, timeout=30)
-        except Exception as e:
-            print(f"Can not create the dataset: {e}")
-        else:
-            print(f"Deleted dataset: {dataset_name}")
-
-    def create_bq_table(self, dataset_id, table_id, schema):
-        try:
-            full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
-            table = bigquery.Table(full_qualified_id, schema=schema)
-            table = self.client.create_table(table)
-        except Exception as e:
-            print(f"Can not create table: {e}")
-        else:
-            print(f"Created the table name {table_id}")
-
-    def create_log_table(self):
-        schema_dict = gbq_log_schema
-        schema = self.generate_bq_schema_from_dict(schema_dict)
-        self.create_bq_dataset(self.__log_dataset)
-        self.create_bq_table(self.__log_dataset, table_id=self.__log_table, schema=schema)
-
-    def create_backup_table(self, dataset_id, table_name):
-        now_th = datetime.now(timezone("Asia/Bangkok"))
-        now_th_text = now_th.strftime("%Y%m%d_%H%M%S")
-        table_name_src = self.__get_full_qualified_table_name(
-            dataset_id=dataset_id, table_id=table_name
-        )
-        table_name_backup = f"{table_name}_bkp_{now_th_text}"
-        table_name_backup = self.__get_full_qualified_table_name(
-            dataset_id=dataset_id, table_id=table_name_backup
-        )
-        sql = f"""
-		CREATE TABLE `{table_name_backup}`
-		AS SELECT * FROM `{table_name_src}`
-		;
-		"""
-        self.run_sql(sql)
-
-    def merge_table(self, dataset_id, table_src, table_dst, col_key, columns):
-        table_src = self.__get_full_qualified_table_name(
-            dataset_id=dataset_id, table_id=table_src
-        )
-        table_dst = self.__get_full_qualified_table_name(
-            dataset_id=dataset_id, table_id=table_dst
-        )
-        on_key = self.generate_merge_on_key(col_key)
-        col_update_set = self.generate_sql_merge_update_set(columns, col_key)
-        col_insert_set = self.generate_sql_merge_insert_set(columns)
-        sql = f"""
-		MERGE `{table_dst}` as t
-		USING `{table_src}` as s
-			ON (
-				{on_key}
-			)
-			WHEN MATCHED THEN
-				UPDATE SET 
-					{col_update_set}
-			WHEN NOT MATCHED THEN
-				{col_insert_set}
-		"""
-        self.run_sql(sql)
-
-    def __get_is_nullable(self, args: str) -> str:
-        # todo handle REPEATED type
-        if args in ("Yes", "YES", "yes", "Y", "y"):
-            return "NULLABLE"
-        return "REQUIRED"
-
-    def generate_dummy_schema_from_df(self, df: pd.DataFrame, output_path=None):
-        data = {}
-        for index, col in enumerate(df.columns):
-            data[col] = {
-                "data_type": "STRING",
-                "precision": 0,
-                "scale": 0,
-                "is_nullable": "YES",
-                "col_id": index,
-                "description": "column description",
-            }
-        if output_path:
-            with open(output_path, "w", encoding="utf8") as json_file:
-                json.dump(data, json_file, ensure_ascii=False, indent=4)
-
-    def read_schema_from_file(self, file_path: str) -> dict:
-        with open(file_path, "r", encoding="utf8") as json_file:
-            data = json.load(json_file)
-        return data
-
-    def generate_bq_schema_from_dict(
-        self, schema_dict, add_etl_cols=False, add_etl_filename=False
-    ):
-        """
-        Example:
-        {
-            'column_name': {
-                'data_type': 'STRING',
-                'precision': 0,
-                'scale': 0,
-                'is_nullable': 'YES',
-                'col_id': 1,
-                'description': 'column description'
-            },
-            'column_name2': {
-                'data_type': 'STRING',
-                'precision': 0,
-                'scale': 0,
-                'is_nullable': 'YES',
-                'col_id': 1,
-                'description': 'column description'
-            }
-        }
-        """
-        schema = []
-        for k, v in schema_dict.items():
-            col_name = k
-            col_type = v.get("data_type")
-            col_mode = self.__get_is_nullable(v.get("is_nullable"))
-            desc = v.get("description")
-            schema.append(
-                bigquery.SchemaField(col_name, col_type, mode=col_mode, description=desc)
-            )
-        # add the etl extra columns if needed
-        if add_etl_cols:
-            if add_etl_filename:
-                schema.append(
-                    bigquery.SchemaField("etl_sourcefilename", "STRING", mode="REQUIRED")
-                )
-            schema.append(
-                bigquery.SchemaField("etl_updatetime", "TIMESTAMP", mode="REQUIRED")
-            )
-            schema.append(
-                bigquery.SchemaField("etl_updatemode", "STRING", mode="REQUIRED")
-            )
-        return schema
-
-    def add_etl_to_data(
-        self, df: pd.DataFrame, add_etl_src_file=False, etl_filename=None
-    ):
-        now_th = datetime.now(timezone("Asia/Bangkok"))
-        df["etl_updatetime"] = now_th
-        df["etl_updatemode"] = "insert"
-        if add_etl_src_file:
-            if etl_filename is None:
-                raise ValueError(
-                    f"Please provide the input filename when set add_etl_src_file=True"
-                )
-            df["etl_sourcefilename"] = etl_filename
-        return df
-
-    def delete_bq_table(self, dataset_id, table_id):
-        """
-        Remove the target table from your dataset
-        """
-        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
-        try:
-            self.client.delete_table(full_qualified_id, not_found_ok=True)
-        except Exception as e:
-            print(f"Failed to delete the table {full_qualified_id} with error {e}")
-        else:
-            print(f"Deleted table: {full_qualified_id}")
-
-    def fix_none_null_value(self, df):
-        df = df.where(pd.notnull(df), None)
-        return df
-
-    def get_mode_bq(self, mode):
-        if mode in ("append", "incremental"):
-            return "WRITE_APPEND"
-        elif mode in ("truncate", "initial"):
-            return "WRITE_TRUNCATE"
-        else:
-            raise ValueError(f"Invalid mode for inserting data to BigQuery: {mode}")
-
-    def insert_row(self, rows, dataset_id, table_name):
-        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_name)
-        table = self.client.get_table(full_qualified_id)
-        errors = self.client.insert_rows(table, rows)
-        if errors:
-            print(f"failed to insert the input row: {errors}")
-
-    def __update_instance(self, dataset_id, table_id):
-        self.dataset_id = dataset_id
-        self.table_name = table_id
-        self.job_uuid = str(uuid.uuid4())
-
-    def log2bq(self, message="no input message", is_error=0):
-        if self.job_uuid is None:
-            self.__update_instance(dataset_id="no_dataset_id", table_id="no_table_name")
-        value = {
-            "hostname": platform.uname().node,
-            "job_uuid": self.job_uuid,
-            "dataset_name": self.dataset_id,
-            "table_name": self.table_name,
-            "message": message,
-            "is_error": is_error,
-            "create_timestamp": datetime.now(),
-        }
-        value = [value]
-        self.insert_row(value, self.__log_dataset, self.__log_table)
-
-    def insert_dataframe_to_bq_table(
-        self, df, dataset_id, table_id, schema, mode, update_instance=True
-    ):
-        """
-        Insert the whole dataframe into BigQuery with proper schema
-
-        mode['append','truncate']
-        'append' = append data to the table
-        'truncate' = remove all data from the table and write
-        """
-        # update value to the instace
-        if update_instance:
-            self.__update_instance(dataset_id, table_id)
-        # ensure the data is good for bigquery
-        df = self.fix_none_null_value(df)
-        mode_bq = self.get_mode_bq(mode)
-        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
-        self.log2bq(message="loading data from input dataframe to the target table")
-        try:
-            job_config = bigquery.LoadJobConfig(schema=schema, write_disposition=mode_bq)
-            print(f"Inserting data to the table {full_qualified_id}")
-            job = self.client.load_table_from_dataframe(
-                df, full_qualified_id, job_config=job_config
-            )
-            job.result()
-        except Exception as e:
-            raise ValueError(f"failed to insert data: {e}")
-        else:
-            print(f"successfully insert data to {full_qualified_id}")
-            self.log2bq(message=f"successfully insert data to {full_qualified_id}")
-            return True
-
-    def prepare_sql_query(self, sql, schema_name_src, table_name_src):
-        if sql is None:
-            sql = f"SELECT * FROM {schema_name_src}.{table_name_src}"
-        print(f"Using the SQL command below")
-        print(sql)
-        return sql
-
-    def clean_thai_phone(self, df: pd.DataFrame, col_phone):
-        df.reset_index(drop=True, inplace=True)
-        if col_phone:
-            for c in col_phone:
-                val = df[c].apply(format_phone).to_list()
-                val = pd.DataFrame(val, columns=["phone_type", "phone_number"])
-                df.loc[:, c] = val["phone_number"]
-        return df
-
-    def __getcsize(self, num):
-        if num is None:
-            return 100000
-        else:
-            return num
-
-    # def load_table_from_db(
-    #     self,
-    #     schema_name_src,
-    #     table_name_src,
-    #     dataset_id,
-    #     table_name,
-    #     schema_dict,
-    #     loading_mode,
-    #     db_engine,
-    #     db_hostname_or_ip,
-    #     db_port_number,
-    #     db_database_name,
-    #     db_username,
-    #     db_password,
-    #     sql=None,
-    #     add_etl_cols=False,
-    #     rename_dict=None,
-    #     col_phone=None,
-    #     csize=None,
-    # ):
-    #     self.__update_instance(dataset_id, table_name)
-    #     self.db = self.__get_db_connection(
-    #         db_hostname_or_ip,
-    #         db_port_number,
-    #         db_database_name,
-    #         db_username,
-    #         db_password,
-    #         engine=db_engine,
-    #     )
-    #     if loading_mode.lower() == "truncate":
-    #         self.clear_table(dataset_id, table_name)
-    #     sql = self.prepare_sql_query(sql, schema_name_src, table_name_src)
-    #     self.log2bq(message="making a request to the target database")
-    #     self.log2bq(message=sql)
-    #     schema = self.generate_bq_schema_from_dict(
-    #         schema_dict, add_etl_cols=add_etl_cols, add_etl_filename=False
-    #     )
-    #     dbcsize = self.__getcsize(csize)
-    #     chunk_count = 0
-    #     for df in pd.read_sql(sql, self.db, chunksize=dbcsize):  # type: ignore
-    #         df = self.remove_nulls(df)
-    #         msg = f"found records of requested data: {df.shape[0]} for the chunk [{chunk_count}]"
-    #         print(msg)
-    #         self.log2bq(message=msg)
-    #         if add_etl_cols:
-    #             df["etl_updatetime"] = datetime.now()
-    #             df["etl_updatemode"] = "INSERT"
-    #             msg = f"added `etl_updatetime`, `etl_updatemode` to df"
-    #             self.log2bq(message=msg)
-    #         df = self.rename_columns(df, rename_col=rename_dict)
-    #         dtype_config = self.generate_dtype_from_schema(schema_dict)
-    #         df = self.clean_thai_phone(df, col_phone)
-    #         df = self.convert_dtype(df, dtype_config)
-    #         self.insert_dataframe_to_bq_table(
-    #             df,
-    #             dataset_id,
-    #             table_name,
-    #             schema,
-    #             mode="append",
-    #             update_instance=False,
-    #         )
-    #         chunk_count += 1
-
-    def remove_nulls(self, df):
-        df.fillna(np.nan, inplace=True)
-        return df
-
-    def load_table_from_postgres(
-        self,
-        schema_name_src,
-        table_name_src,
-        dataset_id,
-        table_name,
-        schema,
-        loading_mode,
-        db_hostname_or_ip,
-        db_port_number,
-        db_database_name,
-        db_username,
-        db_password,
-        sql=None,
-        add_etl_cols=False,
-    ):
-        self.__update_instance(dataset_id, table_name)
-        self.db = self.__get_db_connection(
-            db_hostname_or_ip,
-            db_port_number,
-            db_database_name,
-            db_username,
-            db_password,
-            engine="postgres",
-        )
-        if sql is None:
-            sql = f"SELECT * FROM {schema_name_src}.{table_name_src}"
-        self.log2bq(message="making a request to the target database")
-        self.log2bq(message=sql)
-        df = pd.read_sql(sql, self.db)  # type: ignore
-        print(f"found records of requested data: {df.shape[0]}")
-        self.log2bq(message=f"found records of requested data: {df.shape[0]}")
-        if add_etl_cols:
-            df["etl_updatetime"] = datetime.now()
-            df["etl_updatemode"] = "INSERT"
-            self.log2bq(message=f"added 2 etl_updatetime, etl_updatemode to the data")
-        print(df.head())
-        self.insert_dataframe_to_bq_table(
-            df,
-            dataset_id,
-            table_name,
-            schema,
-            loading_mode,
-            update_instance=False,
-        )
-
-    def rename_columns(self, df: pd.DataFrame, rename_dict: dict):
-        if rename_dict:
-            return df.rename(columns=rename_dict)
-        return df
-
-    def get_schema_dict_from_db(self, df: pd.DataFrame, db_engine=None) -> dict:
-        """Generate a schema dictionary from a dataframe
-        https://cloud.google.com/static/architecture/dw2bq/oracle/oracle-bq-sql-translation-reference.pdf
-
-        Args:
-            df (pd.DataFrame): the input information schema dataframe
-
-        Returns:
-            dict: a dictionary of schema
-
-        Example:
-        {
-            'column_name': {
-                'data_type': 'STRING',
-                'precision': 0,
-                'scale': 0,
-                'is_nullable': 'YES',
-                'col_id': 1
-            },
-            'column_name2': {
-                'data_type': 'STRING',
-                'precision': 0,
-                'scale': 0,
-                'is_nullable': 'YES',
-                'col_id': 1
-            }
-        }
-        """
-        if db_engine is None:
-            raise ValueError(
-                "db_engine is required to select the right data type mapping"
-            )
-        res = None
-        if db_engine.lower() == "oracle":
-            res = self.convert_oracle_dict(df)
-        else:
-            raise ValueError(f"db_engine {db_engine} is not supported yet")
-        return res
-
-    def convert_oracle_dict(
-        self,
-        df,
-    ):
-        res = {}
-        for i, r in df.iterrows():
-            gbq_col_name = self.get_valid_colname(r["COLUMN_NAME"])
-            res[gbq_col_name] = {
-                "data_type": self.get_gbq_type_from_oracle_type(
-                    r["DATA_TYPE"], r["DATA_PRECISION"], r["DATA_SCALE"]
-                ),
-                "precision": r["DATA_PRECISION"],
-                "scale": r["DATA_SCALE"],
-                "length": r["DATA_LENGTH"],
-                "is_nullable": r["NULLABLE"],
-                "col_id": r["COLUMN_ID"],
-            }
-        return res
-
-    def get_str_schema_from_list(self, columns, output_filename=None) -> dict:
-        res = {}
-        for col in columns:
-            res[col] = {
-                "data_type": "STRING",
-                "precision": 0,
-                "scale": 0,
-                "length": 0,
-                "is_nullable": "YES",
-                "col_id": 0,
-            }
-        if output_filename:
-            with open(output_filename, "w", encoding="utf-8") as json_file:
-                json.dump(res, json_file, indent=4, ensure_ascii=False)
-        return res
-
-    def get_gbq_type_from_oracle_type(
-        self, data_type: str, precision: int, scale: int
-    ) -> str:
-        if data_type.lower() in ("numeric", "decimal", "number"):
-            data_type = self.choose_num_bignum(precision, scale)
-        elif "timestamp(" in data_type.lower():
-            return "TIMESTAMP"
-        else:
-            data_type = oracle_to_gbq.get(data_type)  # type: ignore
-        if data_type is None:
-            raise ValueError(f"cannot find the mapping for {data_type}")
-        return data_type
-
-    # def load_table_from_s3(
-    #     self,
-    #     access_key,
-    #     secret_key,
-    #     bucket_name,
-    #     dataset_id,
-    #     table_name,
-    #     schema_dict,
-    #     s3_prefix,
-    #     loading_mode,
-    #     add_etl_cols,
-    #     add_etl_filename,
-    #     lower_colname=True,
-    #     rename_col=None,
-    # ):
-    #     self.__update_instance(dataset_id, table_name)
-    #     schema = self.generate_bq_schema_from_dict(
-    #         schema_dict,
-    #         add_etl_cols=add_etl_cols,
-    #         add_etl_filename=add_etl_filename,
-    #     )
-    #     self.create_bq_dataset(dataset_id)
-    #     self.create_bq_table(dataset_id, table_id=table_name, schema=schema)
-    #     self.s3 = self.get_s3_object(access_key, secret_key, bucket_name)  # type: ignore
-    #     s3_files = self.s3.list_file(s3_prefix)
-    #     for s3_file in s3_files:
-    #         df = self.read_data_from_s3(s3_filepath=s3_file)
-    #         df = self.rename_columns(df, lower_colname, rename_col)
-    #         df = self.manage_etl_columns(
-    #             df, s3_file, add_etl_cols, add_etl_filename
-    #         )
-    #         dtype_config = self.generate_dtype_from_schema(schema_dict)
-    #         df = self.convert_dtype(df, dtype_config)
-    #         self.insert_dataframe_to_bq_table(
-    #             df,
-    #             dataset_id,
-    #             table_name,
-    #             schema,
-    #             loading_mode,
-    #             update_instance=False,
-    #         )
-
-    def manage_etl_columns(
-        self, df, s3_file=None, add_etl_cols=True, add_etl_filename=False
-    ):
-        if add_etl_cols:
-            if add_etl_filename:
-                if s3_file is not None:
-                    df["etl_sourcefilename"] = s3_file
-                else:
-                    raise ValueError(f"There is no input filename")
-            df["etl_updatetime"] = datetime.now()
-            df["etl_updatemode"] = "INSERT"
-        return df
-
-    # def generate_dtype_from_schema(self, schema_dict):
-    #     config = {
-    #         "col_str": [],
-    #         "col_bool": [],
-    #         "col_ts": [],
-    #         "col_dt": [],
-    #         "col_int": [],
-    #         "col_decimal": [],
-    #         "col_float": [],
-    #         "col_time": [],
-    #     }
-    #     for k, v in schema_dict.items():
-    #         if v["data_type"] in ["STRING"]:
-    #             config["col_str"].append(k)
-    #         elif v["data_type"] in ["DATE"]:
-    #             config["col_dt"].append(k)
-    #         elif v["data_type"] in ["TIMESTAMP"]:
-    #             config["col_ts"].append(k)
-    #         elif v["data_type"] in ["INTEGER", "INT64"]:
-    #             config["col_int"].append(k)
-    #         elif v["data_type"] in ["NUMERIC", "DECIMAL"]:
-    #             config["col_decimal"].append(self.choose_num_bignum(v))
-    #         elif v["data_type"] in ["BOOLEAN", "BOOL"]:
-    #             config["col_bool"].append(k)
-    #         elif v["data_type"] in ["FLOAT64", "FLOAT"]:
-    #             config["col_float"].append(k)
-    #         elif v["data_type"] in ["TIME"]:
-    #             config["col_time"].append(k)
-    #         else:
-    #             raise NotImplementedError(
-    #                 f"the value [{v}] is not implemented yet"
-    #             )
-    #     return config
-
-    def choose_num_bignum(self, precision, scale):
-        if (scale is None) and (precision is None):
-            return "NUMERIC"
-        if scale <= 9 and precision <= 38:
-            return "NUMERIC"
-        else:
-            return "BIGNUMERIC"
-
-    def convert_time(self, val):
-        if pd.isna(val):
-            return None
-        else:
-            return val
-
-    def get_row_counts(self, table_id: str):
-        table = self.client.get_table(table_id)
-        return table.num_rows
-
-    def list_tables(self, dataset_name: str = "DATASET_ABC"):
-        tables = []
-        for table in self.client.list_tables(dataset_name):
-            tables.append(table.full_table_id.replace(":", "."))
-        return tables
-
-    def list_datasets(self) -> List[bigquery.Dataset]:
-        datasets = list(self.client.list_datasets())  # Make an API request.
-        return datasets
-
-    def convert_dtype(self, df: pd.DataFrame, schema_bq: List[bigquery.SchemaField]):
-        for sch in schema_bq:
-            print(f"Converting: {sch.name}")
-            data_type = sch.field_type
-            if data_type in ("NUMERIC", "BIGNUMERIC"):
-                df[sch.name] = df[sch.name].apply(self.convert_to_decimal)  # type: ignore it can handle None
-            elif data_type in ("TIMESTAMP"):
-                df[sch.name] = pd.to_datetime(df[sch.name], errors="coerce")
-            elif data_type in ("DATE"):
-                # https://stackoverflow.com/questions/64317195/python-google-cloud-bigquery-parquet-column-date-has-type-int64-which-does-not
-                df[sch.name] = pd.to_datetime(df[sch.name], errors="coerce").dt.date
-            elif data_type in ("TIME"):
-                df[sch.name] = df[sch.name].apply(self.convert_time)  # type: ignore it can handle None
-            elif data_type in ("STRING"):
-                df[sch.name] = df[sch.name].astype(str)
-            elif data_type in ("INTEGER"):
-                df[sch.name] = df[sch.name].astype("float")
-                df[sch.name] = df[sch.name].astype("Int64")
-            elif data_type in ("FLOAT"):
-                df = self.convert_float_cols(df, sch.name)
-            elif data_type in ("BOOLEAN"):
-                df = self.convert_boolean_cols(df, sch.name)
-            else:
-                raise NotImplementedError(
-                    f"the value [{data_type}] is not implemented yet"
-                )
-        df.replace({"nan": None, "NaN": None}, inplace=True)
-        df.replace({pd.NaT: None}, inplace=True)
-        return df
-
-    def convert_to_decimal(self, val):
-        """This is updated method to solve the issue of converting to decimal
-        previously I use the method below, but it will cause the precision issue
-        df[c] = df[c].astype(str).map(decimal.Decimal)
-
-        Args:
-            val (Any): the input value from table
-
-        Returns:
-            Decimal: Decimal value to pass into bigquery
-        """
-        if pd.isna(val):
-            return None
-        if isinstance(val, float):
-            return decimal.Decimal(str(val))
-        else:
-            return decimal.Decimal(val)
-
-    def convert_boolean_cols(self, df, col):
-        try:
-            df[col] = df[col].astype(int)
-        except Exception as e:
-            pass
-        df[col] = df[col].astype("bool")
-        return df
-
-    def convert_float_cols(self, df, col):
-        try:
-            df[col] = df[col].astype(float)
-        except Exception as e:
-            pass
-        return df
-
-    # def read_data_from_s3(self, s3_filepath):
-    #     _temp_file_path = f"./{uuid.uuid4().hex}.tempfile"
-    #     self.s3.download_file(s3_filepath, _temp_file_path)
-    #     if s3_filepath.endswith(".csv"):
-    #         df = pd.read_csv(_temp_file_path, dtype=str)
-    #     elif s3_filepath.endswith(".xlsx"):
-    #         df = pd.read_excel(_temp_file_path, dtype=str, engine="openpyxl")
-    #     else:
-    #         raise NotImplementedError(
-    #             f"the input file is not supported yet: {s3_filepath}"
-    #         )
-    #     os.remove(_temp_file_path)
-    #     print(f"data size {df.shape}")
-    #     return df
-
-    def run_sql(self, sql):
-        query_job = self.client.query(sql)
-        results = query_job.result()
-        return results
-
-    def clear_table(self, dataset_id, table_id):
-        """remove all records from the table, the target table must exists to run this
-
-        Args:
-                dataset_id (str): schema_name/dataset_id
-                table_id (str): table_name/table_id
-        """
-        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
-        sql = f"TRUNCATE TABLE {full_qualified_id}"
-        self.run_sql(sql)
-
-    def get_schema_from_existing_table(self, dataset_id, table_id):
-        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
-        table = self.client.get_table(full_qualified_id)
-        return table.schema
-
-    def generate_merge_on_key(self, col_key):
-        txt = ""
-        for col in col_key:
-            _t = f"t.{col} = s.{col}"
-            if col != col_key[-1]:
-                _t = f"{_t} AND "
-            txt += _t
-        return txt
-
-    def generate_sql_merge_update_set(self, columns, col_key):
-        columns = [c for c in columns if c.lower() not in col_key]
-        n_col = len(columns)
-        txt = ""
-        for index, col in enumerate(columns):
-            if col == "update_mode":
-                txt += f"t.{col} = 'UPDATE',\n"
-            elif not (index + 1) == n_col:
-                txt += f"t.{col} = s.{col},\n"
-            else:
-                txt += f"t.{col} = s.{col}\n"
-        return txt
-
-    def generate_sql_merge_insert_set(self, columns):
-        col_txt = ",".join(columns)
-        col_txt_value = ""
-        for col in columns:
-            col_txt_value += f"s.{col},"
-        col_txt_value = col_txt_value[:-1]
-        # final text to output
-        txt_final = f"""
-		INSERT({col_txt})
-		VALUES({col_txt_value})
-		"""
-        return txt_final
-
-    def create_external_table_from_gcs(
-        self,
-        table_id: str,
-        gcs_uri: str,
-        file_type: str,
-        connection_id: Union[str, None] = None,
-        is_hive_partition: bool = False,
-        schema: Union[List[bigquery.SchemaField], None] = None,
-    ) -> "bigquery.Table":  # type: ignore
-        # table_id = "your-project.your_dataset.your_table_name"
-        # gcs_uri = "gs://cto-ris-cds-prd_converted/test/cds/jda/outbound/JDASKU/*"
-        # source_uri_prefix = "gs://cto-ris-cds-prd_converted/test/cds/jda/outbound/JDASKU/"
-        # Example usage: gbq.create_external_table_from_gcs(table_id=table_id,schema=None,gcs_uri=gcs_uri,avro_or_parquet='AVRO',is_hive_partition=True)
-        # ================================= Choose file format =================================
-        if file_type.upper() == "AVRO":
-            external_config = bigquery.ExternalConfig("AVRO")
-        elif file_type.upper() == "PARQUET":
-            external_config = bigquery.ExternalConfig("PARQUET")
-        elif file_type.upper() == "NEWLINE_DELIMITED_JSON":
-            external_config = bigquery.ExternalConfig("NEWLINE_DELIMITED_JSON")
-        else:
-            raise NotImplementedError(f"The {file_type} type is not supported yet")
-        external_config.source_uris = [gcs_uri]
-        if connection_id:
-            external_config.connection_id = connection_id
-        source_uri_prefix = gcs_uri[:-1]
-        # ================================= Set Hive partition config =================================
-        if is_hive_partition:
-            hive_partitioning_opts = bigquery.HivePartitioningOptions()
-            hive_partitioning_opts.mode = "AUTO"
-            hive_partitioning_opts.require_partition_filter = False
-            hive_partitioning_opts.source_uri_prefix = source_uri_prefix
-            external_config.hive_partitioning = hive_partitioning_opts
-        # ================================= Set external table config =================================
-        if schema is None:
-            external_config.autodetect = True
-            table = bigquery.Table(table_id)
-        else:
-            table = bigquery.Table(table_id, schema=schema)
-        table.external_data_configuration = external_config
-        # ================================= Create table =================================
-        try:
-            table = self.client.create_table(table)  # Make an API request.
-        except Exception as e:
-            if "Already Exists: Table" in e.args[0]:
-                print(f"Table already exists: {table_id}")
-            else:
-                raise ValueError(e)
-        else:
-            return table
-
-    def get_schema_policy_tag(
-        self,
-        col_name,
-        col_type,
-        col_mode,
-        policy_tag_id: Union[str, None] = None,
-        fields: Union[List[bigquery.SchemaField], None] = None,
-        desc: str = "No description",
-    ):
-        """Add policy tag to the BigQuery table schema
-        Args:
-            col_name (tr): the name of the column
-            col_type (str): the type of the column, e.g. STRING, INTEGER, FLOAT, etc.
-            col_mode (str): the mode of the column, e.g. NULLABLE, REQUIRED, REPEATED
-            policy_tag_id (str, optional): The policy tag full id. Defaults to None. example: projects/myproject/locations/asia-southeast1/taxonomies/11111111111111111111/policyTags/22222222222222222
-        Returns:
-            bigquery.SchemaField: the schema field with policy tag or without it
-        """
-        bq_policy = bigquery.PolicyTagList(names=[policy_tag_id])  # type: ignore
-        if fields is None:
-            fields = []
-        if policy_tag_id:
-            return bigquery.SchemaField(
-                name=col_name,
-                field_type=col_type,
-                mode=col_mode,
-                description=desc,
-                fields=fields,
-                policy_tags=bq_policy,
-            )
-        else:
-            return bigquery.SchemaField(
-                name=col_name,
-                field_type=col_type,
-                mode=col_mode,
-                description=desc,
-                fields=fields,
-            )
-
-    def create_external_table_from_google_sheets(
-        self,
-        table_id: str,
-        ext_config: Union[bigquery.ExternalConfig, None] = None,
-        uri: str = "",
-        schema: Union[List[bigquery.SchemaField], None] = None,
-    ) -> None:
-        table = bigquery.Table(table_id, schema=schema)
-        if ext_config:
-            table.external_data_configuration = ext_config
-        else:
-            external_cfg = bigquery.ExternalConfig("GOOGLE_SHEETS")
-            external_cfg.source_uris = [uri]
-            external_cfg.options.skip_leading_rows = 1  # type: ignore
-            # external_cfg.autodetect = True
-            # external_cfg.max_bad_records = 2
-            external_cfg.ignore_unknown_values = False
-            table.external_data_configuration = external_cfg
-        table = self.client.create_table(table)
-        print(table)
-
-    # ================================= Get data from GBQ =================================
-    def get_data_from_gbq(self, sql: str) -> pd.DataFrame:
-        # sql = "SELECT * FROM `bigquery-public-data.irs_990.irs_990_2012`"
-        # need package: google-cloud-bigquery-storage, pyarrow
-        return self.client.query(sql).to_dataframe()
+"""
+referencecs:
+BigQuery: https://github.com/googleapis/python-bigquery/blob/a3f4351633f006b3132d8a8625ad7921b3d57699/samples/snippets/create_table_external_hive_partitioned.py
+BgiQuery: https://github.com/googleapis/python-bigquery/blob/35627d145a41d57768f19d4392ef235928e00f72/samples/load_table_uri_parquet.py
+
+Oracle:
+- ORA-29275: partial multibyte character
+    - solution 1: `SELECT CONVERT(COLUMN NAME, 'UTF8', 'US7ASCII')` do this for all string based 
+    - solution 2: Loop through the row to find the row that has error
+    - readmore: https://stackoverflow.com/questions/37964728/biztalk-wcf-custom-raised-an-error-ora-29275-partial-multibyte-character
+
+"""
+import decimal
+import json
+import logging
+import os
+import platform
+import re
+import uuid
+from datetime import datetime
+from typing import List, Optional, Union
+
+import google.cloud.logging
+import numpy as np
+import pandas as pd
+from google.cloud import bigquery
+from pytz import timezone
+
+from npgbq.core.helper_phone_number_th import format_phone
+
+from ..connectors.dtype_mapper import oracle_to_gbq
+
+# from ..connectors.mssql import get_conn_mssql # disabled in 2.0.5
+from ..connectors.postgres import get_conn_pg
+from .log_table_schema import gbq_log_schema
+
+
+class NPGBQ(object):
+    def __init__(self, project_id, gcp_service_account_path: Optional[str] = None):
+        self.project_id = project_id
+        self.path_json_key = gcp_service_account_path
+        self.__add_environment()
+
+        # var default
+        self.__log_dataset = "data_log"
+        self.__log_table = "logs"
+        self.job_uuid = None
+        self.dataset_id = None
+        self.table_name = None
+
+        # create client
+        self.client = self.__get_bq_client()
+
+    def __add_environment(self):
+        if self.path_json_key:
+            os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = self.path_json_key
+
+    def __get_bq_client(self):
+
+        client = google.cloud.logging.Client(project=self.project_id)
+        client.setup_logging(log_level=logging.INFO)
+        return bigquery.Client(self.project_id)
+
+    @staticmethod
+    def get_valid_colname(text: str):
+        val = re.sub("[^A-Za-z0-9_]+", "_", text)
+        val = NPGBQ.remove_double_underscores(val)
+        val = NPGBQ.remove_double_space(val)
+        val = val.upper().rstrip("_").lstrip("_")
+        if re.search(r"^\d", val):
+            val = f"_{val}"
+        return val
+
+    @staticmethod
+    def remove_double_space(text: str) -> str:
+        regex = re.compile(r"\s+")
+        return re.sub(regex, " ", text)
+
+    @staticmethod
+    def remove_double_underscores(text: str) -> str:
+        regex = re.compile(r"__+")
+        return re.sub(regex, "_", text)
+
+    def format_deciaml_cols(self, df, col_decimal):
+        for col in col_decimal:
+            df[col] = df[col].astype(str).map(decimal.Decimal)
+        return df
+
+    def __validate_col_type(self, col_type: str) -> bool:
+        valid_col_type = [
+            "ARRAY",
+            "BIGNUMERIC",
+            "BOOL",
+            "BOOLEAN",
+            "DATE",
+            "DATES",
+            "FLOAT",
+            "FLOAT64",
+            "GEOGRAPHY",
+            "INT64",
+            "INTEGER",
+            "INTERVAL",
+            "NUMERIC",
+            "STRING",
+            "TIME",
+            "TIMESTAMP",
+        ]
+        if col_type not in valid_col_type:
+            raise ValueError(f"the input column datatype {  col_type} is not valid")
+        return True
+
+    @staticmethod
+    def get_full_qualified_table_name(project_id, dataset_id, table_id):
+        full_qualified_id = f"{project_id}.{dataset_id}.{table_id}"
+        return full_qualified_id
+
+    def __get_full_qualified_table_name(self, dataset_id, table_id):
+        full_qualified_id = f"{self.client.project}.{dataset_id}.{table_id}"
+        return full_qualified_id
+
+    def update_schema(self, table_obj: bigquery.Table, mapping: dict, desc: str):
+        """
+        Usage:
+        table_id = "central-cto-cds-data-hub-prd.rbs_mdc.customer_entity"
+        table_obj = gbq.client.get_table(table_id)
+        mapping = {"default_billing": "INTEGER", "default_shipping": "INTEGER",'gender':'INTEGER'}
+        gbq.update_schema(table_obj, mapping)
+        """
+        schema = table_obj.schema
+        _schema = []
+        for field in schema:
+            if field.name in mapping:
+                new_field = bigquery.SchemaField(field.name, mapping[field.name], mode=field.mode, description=desc)  # type: ignore
+                _schema.append(new_field)
+            else:
+                _schema.append(field)
+        table_obj.schema = _schema
+        self.client.update_table(table_obj, ["schema"])
+        print(f"Schema updated for {table_obj.full_table_id}")
+
+    def get_col_rename_dict(self, dict_org: dict, dict_gbq: dict) -> dict:
+        res = {}
+        for (k1, v2), (k2, v2) in zip(dict_org.items(), dict_gbq.items()):
+            if k1 != k2:
+                res[k1] = k2
+        return res
+
+    def __get_db_connection(
+        self,
+        db_hostname_or_ip,
+        db_port_number,
+        db_database_name,
+        db_username,
+        db_password,
+        engine="postgres",
+    ):
+        # self.log2bq(message=f"Making connection to database: {db_database_name}")
+        conn = None
+        if engine == "postgres":
+            conn = get_conn_pg(
+                db_hostname_or_ip,
+                db_port_number,
+                db_database_name,
+                db_username,
+                db_password,
+            )
+        # disabled in 2.0.5
+        # elif engine == "mssql":
+        #     conn = get_conn_mssql(
+        #         db_hostname_or_ip,
+        #         db_port_number,
+        #         db_database_name,
+        #         db_username,
+        #         db_password,
+        #     )
+        else:
+            raise NotImplementedError(
+                f"your engine {engine} is invalid please contact the administrator"
+            )
+        # self.log2bq(message=f"The connection is ready: {db_database_name}")
+        return conn
+
+    # ====================================== Public method ======================================
+
+    def create_bq_dataset(self, dataset_id):
+        try:
+            dataset_id = f"{self.client.project}.{dataset_id}"
+            dataset = bigquery.Dataset(dataset_id)
+            dataset.location = "asia-southeast1"
+            dataset = self.client.create_dataset(dataset, timeout=30)
+        except Exception as e:
+            print(f"Can not create the dataset: {e}")
+        else:
+            print(f"Created dataset name {dataset_id}")
+
+    def delete_bq_dataset(self, dataset_name: str = "DATASET_ABC"):
+        # need to remove all tables from the dataset first
+        tables = self.list_tables(dataset_name)
+        for table in tables:
+            table_name = table.split(".")[-1]
+            self.delete_bq_table(dataset_name, table_name)
+        try:
+            dataset_name = f"{self.client.project}.{dataset_name}"
+            dataset = bigquery.Dataset(dataset_name)
+            dataset.location = "asia-southeast1"
+            dataset = self.client.delete_dataset(dataset, timeout=30)
+        except Exception as e:
+            print(f"Can not create the dataset: {e}")
+        else:
+            print(f"Deleted dataset: {dataset_name}")
+
+    def create_bq_table(self, dataset_id, table_id, schema):
+        try:
+            full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
+            table = bigquery.Table(full_qualified_id, schema=schema)
+            table = self.client.create_table(table)
+        except Exception as e:
+            print(f"Can not create table: {e}")
+        else:
+            print(f"Created the table name {table_id}")
+
+    def create_log_table(self):
+        schema_dict = gbq_log_schema
+        schema = self.generate_bq_schema_from_dict(schema_dict)
+        self.create_bq_dataset(self.__log_dataset)
+        self.create_bq_table(self.__log_dataset, table_id=self.__log_table, schema=schema)
+
+    def create_backup_table(self, dataset_id, table_name):
+        now_th = datetime.now(timezone("Asia/Bangkok"))
+        now_th_text = now_th.strftime("%Y%m%d_%H%M%S")
+        table_name_src = self.__get_full_qualified_table_name(
+            dataset_id=dataset_id, table_id=table_name
+        )
+        table_name_backup = f"{table_name}_bkp_{now_th_text}"
+        table_name_backup = self.__get_full_qualified_table_name(
+            dataset_id=dataset_id, table_id=table_name_backup
+        )
+        sql = f"""
+		CREATE TABLE `{table_name_backup}`
+		AS SELECT * FROM `{table_name_src}`
+		;
+		"""
+        self.run_sql(sql)
+
+    def merge_table(self, dataset_id, table_src, table_dst, col_key, columns):
+        table_src = self.__get_full_qualified_table_name(
+            dataset_id=dataset_id, table_id=table_src
+        )
+        table_dst = self.__get_full_qualified_table_name(
+            dataset_id=dataset_id, table_id=table_dst
+        )
+        on_key = self.generate_merge_on_key(col_key)
+        col_update_set = self.generate_sql_merge_update_set(columns, col_key)
+        col_insert_set = self.generate_sql_merge_insert_set(columns)
+        sql = f"""
+		MERGE `{table_dst}` as t
+		USING `{table_src}` as s
+			ON (
+				{on_key}
+			)
+			WHEN MATCHED THEN
+				UPDATE SET 
+					{col_update_set}
+			WHEN NOT MATCHED THEN
+				{col_insert_set}
+		"""
+        self.run_sql(sql)
+
+    def __get_is_nullable(self, args: str) -> str:
+        # todo handle REPEATED type
+        if args in ("Yes", "YES", "yes", "Y", "y"):
+            return "NULLABLE"
+        return "REQUIRED"
+
+    def generate_dummy_schema_from_df(self, df: pd.DataFrame, output_path=None):
+        data = {}
+        for index, col in enumerate(df.columns):
+            data[col] = {
+                "data_type": "STRING",
+                "precision": 0,
+                "scale": 0,
+                "is_nullable": "YES",
+                "col_id": index,
+                "description": "column description",
+            }
+        if output_path:
+            with open(output_path, "w", encoding="utf8") as json_file:
+                json.dump(data, json_file, ensure_ascii=False, indent=4)
+
+    def read_schema_from_file(self, file_path: str) -> dict:
+        with open(file_path, "r", encoding="utf8") as json_file:
+            data = json.load(json_file)
+        return data
+
+    def generate_bq_schema_from_dict(
+        self, schema_dict, add_etl_cols=False, add_etl_filename=False
+    ):
+        """
+        Example:
+        {
+            'column_name': {
+                'data_type': 'STRING',
+                'precision': 0,
+                'scale': 0,
+                'is_nullable': 'YES',
+                'col_id': 1,
+                'description': 'column description'
+            },
+            'column_name2': {
+                'data_type': 'STRING',
+                'precision': 0,
+                'scale': 0,
+                'is_nullable': 'YES',
+                'col_id': 1,
+                'description': 'column description'
+            }
+        }
+        """
+        schema = []
+        for k, v in schema_dict.items():
+            col_name = k
+            col_type = v.get("data_type")
+            col_mode = self.__get_is_nullable(v.get("is_nullable"))
+            desc = v.get("description")
+            schema.append(
+                bigquery.SchemaField(col_name, col_type, mode=col_mode, description=desc)
+            )
+        # add the etl extra columns if needed
+        if add_etl_cols:
+            if add_etl_filename:
+                schema.append(
+                    bigquery.SchemaField("etl_sourcefilename", "STRING", mode="REQUIRED")
+                )
+            schema.append(
+                bigquery.SchemaField("etl_updatetime", "TIMESTAMP", mode="REQUIRED")
+            )
+            schema.append(
+                bigquery.SchemaField("etl_updatemode", "STRING", mode="REQUIRED")
+            )
+        return schema
+
+    def add_etl_to_data(
+        self, df: pd.DataFrame, add_etl_src_file=False, etl_filename=None
+    ):
+        now_th = datetime.now(timezone("Asia/Bangkok"))
+        df["etl_updatetime"] = now_th
+        df["etl_updatemode"] = "insert"
+        if add_etl_src_file:
+            if etl_filename is None:
+                raise ValueError(
+                    f"Please provide the input filename when set add_etl_src_file=True"
+                )
+            df["etl_sourcefilename"] = etl_filename
+        return df
+
+    def delete_bq_table(self, dataset_id, table_id):
+        """
+        Remove the target table from your dataset
+        """
+        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
+        try:
+            self.client.delete_table(full_qualified_id, not_found_ok=True)
+        except Exception as e:
+            print(f"Failed to delete the table {full_qualified_id} with error {e}")
+        else:
+            print(f"Deleted table: {full_qualified_id}")
+
+    def fix_none_null_value(self, df):
+        df = df.where(pd.notnull(df), None)
+        return df
+
+    def get_mode_bq(self, mode):
+        if mode in ("append", "incremental"):
+            return "WRITE_APPEND"
+        elif mode in ("truncate", "initial"):
+            return "WRITE_TRUNCATE"
+        else:
+            raise ValueError(f"Invalid mode for inserting data to BigQuery: {mode}")
+
+    def insert_row(self, rows, dataset_id, table_name):
+        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_name)
+        table = self.client.get_table(full_qualified_id)
+        errors = self.client.insert_rows(table, rows)
+        if errors:
+            print(f"failed to insert the input row: {errors}")
+
+    def __update_instance(self, dataset_id, table_id):
+        self.dataset_id = dataset_id
+        self.table_name = table_id
+        self.job_uuid = str(uuid.uuid4())
+
+    def log2bq(self, message="no input message", is_error=0):
+        if self.job_uuid is None:
+            self.__update_instance(dataset_id="no_dataset_id", table_id="no_table_name")
+        value = {
+            "hostname": platform.uname().node,
+            "job_uuid": self.job_uuid,
+            "dataset_name": self.dataset_id,
+            "table_name": self.table_name,
+            "message": message,
+            "is_error": is_error,
+            "create_timestamp": datetime.now(),
+        }
+        value = [value]
+        self.insert_row(value, self.__log_dataset, self.__log_table)
+
+    def insert_dataframe_to_bq_table(
+        self, df, dataset_id, table_id, schema, mode, update_instance=True
+    ):
+        """
+        Insert the whole dataframe into BigQuery with proper schema
+
+        mode['append','truncate']
+        'append' = append data to the table
+        'truncate' = remove all data from the table and write
+        """
+        # update value to the instace
+        if update_instance:
+            self.__update_instance(dataset_id, table_id)
+        # ensure the data is good for bigquery
+        df = self.fix_none_null_value(df)
+        mode_bq = self.get_mode_bq(mode)
+        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
+        # self.log2bq(message="loading data from input dataframe to the target table")
+        try:
+            job_config = bigquery.LoadJobConfig(schema=schema, write_disposition=mode_bq)
+            print(f"Inserting data to the table {full_qualified_id}")
+            job = self.client.load_table_from_dataframe(
+                df, full_qualified_id, job_config=job_config
+            )
+            job.result()
+        except Exception as e:
+            raise ValueError(f"failed to insert data: {e}")
+        else:
+            print(f"successfully insert data to {full_qualified_id}")
+            # self.log2bq(message=f"successfully insert data to {full_qualified_id}")
+            return True
+
+    def prepare_sql_query(self, sql, schema_name_src, table_name_src):
+        if sql is None:
+            sql = f"SELECT * FROM {schema_name_src}.{table_name_src}"
+        print(f"Using the SQL command below")
+        print(sql)
+        return sql
+
+    def clean_thai_phone(self, df: pd.DataFrame, col_phone):
+        df.reset_index(drop=True, inplace=True)
+        if col_phone:
+            for c in col_phone:
+                val = df[c].apply(format_phone).to_list()
+                val = pd.DataFrame(val, columns=["phone_type", "phone_number"])
+                df.loc[:, c] = val["phone_number"]
+        return df
+
+    def __getcsize(self, num):
+        if num is None:
+            return 100000
+        else:
+            return num
+
+    # def load_table_from_db(
+    #     self,
+    #     schema_name_src,
+    #     table_name_src,
+    #     dataset_id,
+    #     table_name,
+    #     schema_dict,
+    #     loading_mode,
+    #     db_engine,
+    #     db_hostname_or_ip,
+    #     db_port_number,
+    #     db_database_name,
+    #     db_username,
+    #     db_password,
+    #     sql=None,
+    #     add_etl_cols=False,
+    #     rename_dict=None,
+    #     col_phone=None,
+    #     csize=None,
+    # ):
+    #     self.__update_instance(dataset_id, table_name)
+    #     self.db = self.__get_db_connection(
+    #         db_hostname_or_ip,
+    #         db_port_number,
+    #         db_database_name,
+    #         db_username,
+    #         db_password,
+    #         engine=db_engine,
+    #     )
+    #     if loading_mode.lower() == "truncate":
+    #         self.clear_table(dataset_id, table_name)
+    #     sql = self.prepare_sql_query(sql, schema_name_src, table_name_src)
+    #     self.log2bq(message="making a request to the target database")
+    #     self.log2bq(message=sql)
+    #     schema = self.generate_bq_schema_from_dict(
+    #         schema_dict, add_etl_cols=add_etl_cols, add_etl_filename=False
+    #     )
+    #     dbcsize = self.__getcsize(csize)
+    #     chunk_count = 0
+    #     for df in pd.read_sql(sql, self.db, chunksize=dbcsize):  # type: ignore
+    #         df = self.remove_nulls(df)
+    #         msg = f"found records of requested data: {df.shape[0]} for the chunk [{chunk_count}]"
+    #         print(msg)
+    #         self.log2bq(message=msg)
+    #         if add_etl_cols:
+    #             df["etl_updatetime"] = datetime.now()
+    #             df["etl_updatemode"] = "INSERT"
+    #             msg = f"added `etl_updatetime`, `etl_updatemode` to df"
+    #             self.log2bq(message=msg)
+    #         df = self.rename_columns(df, rename_col=rename_dict)
+    #         dtype_config = self.generate_dtype_from_schema(schema_dict)
+    #         df = self.clean_thai_phone(df, col_phone)
+    #         df = self.convert_dtype(df, dtype_config)
+    #         self.insert_dataframe_to_bq_table(
+    #             df,
+    #             dataset_id,
+    #             table_name,
+    #             schema,
+    #             mode="append",
+    #             update_instance=False,
+    #         )
+    #         chunk_count += 1
+
+    def remove_nulls(self, df):
+        df.fillna(np.nan, inplace=True)
+        return df
+
+    def load_table_from_postgres(
+        self,
+        schema_name_src,
+        table_name_src,
+        dataset_id,
+        table_name,
+        schema,
+        loading_mode,
+        db_hostname_or_ip,
+        db_port_number,
+        db_database_name,
+        db_username,
+        db_password,
+        sql=None,
+        add_etl_cols=False,
+    ):
+        self.__update_instance(dataset_id, table_name)
+        self.db = self.__get_db_connection(
+            db_hostname_or_ip,
+            db_port_number,
+            db_database_name,
+            db_username,
+            db_password,
+            engine="postgres",
+        )
+        if sql is None:
+            sql = f"SELECT * FROM {schema_name_src}.{table_name_src}"
+        # self.log2bq(message="making a request to the target database")
+        # self.log2bq(message=sql)
+        df = pd.read_sql(sql, self.db)  # type: ignore
+        print(f"found records of requested data: {df.shape[0]}")
+        # self.log2bq(message=f"found records of requested data: {df.shape[0]}")
+        if add_etl_cols:
+            df["etl_updatetime"] = datetime.now()
+            df["etl_updatemode"] = "INSERT"
+            # self.log2bq(message=f"added 2 etl_updatetime, etl_updatemode to the data")
+        print(df.head())
+        self.insert_dataframe_to_bq_table(
+            df,
+            dataset_id,
+            table_name,
+            schema,
+            loading_mode,
+            update_instance=False,
+        )
+
+    def rename_columns(self, df: pd.DataFrame, rename_dict: dict):
+        if rename_dict:
+            return df.rename(columns=rename_dict)
+        return df
+
+    def get_schema_dict_from_db(self, df: pd.DataFrame, db_engine=None) -> dict:
+        """Generate a schema dictionary from a dataframe
+        https://cloud.google.com/static/architecture/dw2bq/oracle/oracle-bq-sql-translation-reference.pdf
+
+        Args:
+            df (pd.DataFrame): the input information schema dataframe
+
+        Returns:
+            dict: a dictionary of schema
+
+        Example:
+        {
+            'column_name': {
+                'data_type': 'STRING',
+                'precision': 0,
+                'scale': 0,
+                'is_nullable': 'YES',
+                'col_id': 1
+            },
+            'column_name2': {
+                'data_type': 'STRING',
+                'precision': 0,
+                'scale': 0,
+                'is_nullable': 'YES',
+                'col_id': 1
+            }
+        }
+        """
+        if db_engine is None:
+            raise ValueError(
+                "db_engine is required to select the right data type mapping"
+            )
+        res = None
+        if db_engine.lower() == "oracle":
+            res = self.convert_oracle_dict(df)
+        else:
+            raise ValueError(f"db_engine {db_engine} is not supported yet")
+        return res
+
+    def convert_oracle_dict(
+        self,
+        df,
+    ):
+        res = {}
+        for i, r in df.iterrows():
+            gbq_col_name = self.get_valid_colname(r["COLUMN_NAME"])
+            res[gbq_col_name] = {
+                "data_type": self.get_gbq_type_from_oracle_type(
+                    r["DATA_TYPE"], r["DATA_PRECISION"], r["DATA_SCALE"]
+                ),
+                "precision": r["DATA_PRECISION"],
+                "scale": r["DATA_SCALE"],
+                "length": r["DATA_LENGTH"],
+                "is_nullable": r["NULLABLE"],
+                "col_id": r["COLUMN_ID"],
+            }
+        return res
+
+    def get_str_schema_from_list(self, columns, output_filename=None) -> dict:
+        res = {}
+        for col in columns:
+            res[col] = {
+                "data_type": "STRING",
+                "precision": 0,
+                "scale": 0,
+                "length": 0,
+                "is_nullable": "YES",
+                "col_id": 0,
+            }
+        if output_filename:
+            with open(output_filename, "w", encoding="utf-8") as json_file:
+                json.dump(res, json_file, indent=4, ensure_ascii=False)
+        return res
+
+    def get_gbq_type_from_oracle_type(
+        self, data_type: str, precision: int, scale: int
+    ) -> str:
+        if data_type.lower() in ("numeric", "decimal", "number"):
+            data_type = self.choose_num_bignum(precision, scale)
+        elif "timestamp(" in data_type.lower():
+            return "TIMESTAMP"
+        else:
+            data_type = oracle_to_gbq.get(data_type)  # type: ignore
+        if data_type is None:
+            raise ValueError(f"cannot find the mapping for {data_type}")
+        return data_type
+
+    # def load_table_from_s3(
+    #     self,
+    #     access_key,
+    #     secret_key,
+    #     bucket_name,
+    #     dataset_id,
+    #     table_name,
+    #     schema_dict,
+    #     s3_prefix,
+    #     loading_mode,
+    #     add_etl_cols,
+    #     add_etl_filename,
+    #     lower_colname=True,
+    #     rename_col=None,
+    # ):
+    #     self.__update_instance(dataset_id, table_name)
+    #     schema = self.generate_bq_schema_from_dict(
+    #         schema_dict,
+    #         add_etl_cols=add_etl_cols,
+    #         add_etl_filename=add_etl_filename,
+    #     )
+    #     self.create_bq_dataset(dataset_id)
+    #     self.create_bq_table(dataset_id, table_id=table_name, schema=schema)
+    #     self.s3 = self.get_s3_object(access_key, secret_key, bucket_name)  # type: ignore
+    #     s3_files = self.s3.list_file(s3_prefix)
+    #     for s3_file in s3_files:
+    #         df = self.read_data_from_s3(s3_filepath=s3_file)
+    #         df = self.rename_columns(df, lower_colname, rename_col)
+    #         df = self.manage_etl_columns(
+    #             df, s3_file, add_etl_cols, add_etl_filename
+    #         )
+    #         dtype_config = self.generate_dtype_from_schema(schema_dict)
+    #         df = self.convert_dtype(df, dtype_config)
+    #         self.insert_dataframe_to_bq_table(
+    #             df,
+    #             dataset_id,
+    #             table_name,
+    #             schema,
+    #             loading_mode,
+    #             update_instance=False,
+    #         )
+
+    def manage_etl_columns(
+        self, df, s3_file=None, add_etl_cols=True, add_etl_filename=False
+    ):
+        if add_etl_cols:
+            if add_etl_filename:
+                if s3_file is not None:
+                    df["etl_sourcefilename"] = s3_file
+                else:
+                    raise ValueError(f"There is no input filename")
+            df["etl_updatetime"] = datetime.now()
+            df["etl_updatemode"] = "INSERT"
+        return df
+
+    # def generate_dtype_from_schema(self, schema_dict):
+    #     config = {
+    #         "col_str": [],
+    #         "col_bool": [],
+    #         "col_ts": [],
+    #         "col_dt": [],
+    #         "col_int": [],
+    #         "col_decimal": [],
+    #         "col_float": [],
+    #         "col_time": [],
+    #     }
+    #     for k, v in schema_dict.items():
+    #         if v["data_type"] in ["STRING"]:
+    #             config["col_str"].append(k)
+    #         elif v["data_type"] in ["DATE"]:
+    #             config["col_dt"].append(k)
+    #         elif v["data_type"] in ["TIMESTAMP"]:
+    #             config["col_ts"].append(k)
+    #         elif v["data_type"] in ["INTEGER", "INT64"]:
+    #             config["col_int"].append(k)
+    #         elif v["data_type"] in ["NUMERIC", "DECIMAL"]:
+    #             config["col_decimal"].append(self.choose_num_bignum(v))
+    #         elif v["data_type"] in ["BOOLEAN", "BOOL"]:
+    #             config["col_bool"].append(k)
+    #         elif v["data_type"] in ["FLOAT64", "FLOAT"]:
+    #             config["col_float"].append(k)
+    #         elif v["data_type"] in ["TIME"]:
+    #             config["col_time"].append(k)
+    #         else:
+    #             raise NotImplementedError(
+    #                 f"the value [{v}] is not implemented yet"
+    #             )
+    #     return config
+
+    def choose_num_bignum(self, precision, scale):
+        if (scale is None) and (precision is None):
+            return "NUMERIC"
+        if scale <= 9 and precision <= 38:
+            return "NUMERIC"
+        else:
+            return "BIGNUMERIC"
+
+    def convert_time(self, val):
+        if pd.isna(val):
+            return None
+        else:
+            return val
+
+    def get_row_counts(self, table_id: str):
+        table = self.client.get_table(table_id)
+        return table.num_rows
+
+    def list_tables(self, dataset_name: str = "DATASET_ABC"):
+        tables = []
+        for table in self.client.list_tables(dataset_name):
+            tables.append(table.full_table_id.replace(":", "."))
+        return tables
+
+    def list_datasets(self) -> List[bigquery.Dataset]:
+        datasets = list(self.client.list_datasets())  # Make an API request.
+        return datasets
+
+    def convert_dtype(self, df: pd.DataFrame, schema_bq: List[bigquery.SchemaField]):
+        for sch in schema_bq:
+            print(f"Converting: {sch.name}")
+            data_type = sch.field_type
+            if data_type in ("NUMERIC", "BIGNUMERIC"):
+                df[sch.name] = df[sch.name].apply(self.convert_to_decimal)  # type: ignore it can handle None
+            elif data_type in ("TIMESTAMP"):
+                df[sch.name] = pd.to_datetime(df[sch.name], errors="coerce")
+            elif data_type in ("DATE"):
+                # https://stackoverflow.com/questions/64317195/python-google-cloud-bigquery-parquet-column-date-has-type-int64-which-does-not
+                df[sch.name] = pd.to_datetime(df[sch.name], errors="coerce").dt.date
+            elif data_type in ("TIME"):
+                df[sch.name] = df[sch.name].apply(self.convert_time)  # type: ignore it can handle None
+            elif data_type in ("STRING"):
+                df[sch.name] = df[sch.name].astype(str)
+            elif data_type in ("INTEGER"):
+                df[sch.name] = df[sch.name].astype("float")
+                df[sch.name] = df[sch.name].astype("Int64")
+            elif data_type in ("FLOAT"):
+                df = self.convert_float_cols(df, sch.name)
+            elif data_type in ("BOOLEAN"):
+                df = self.convert_boolean_cols(df, sch.name)
+            else:
+                raise NotImplementedError(
+                    f"the value [{data_type}] is not implemented yet"
+                )
+        df.replace({"nan": None, "NaN": None}, inplace=True)
+        df.replace({pd.NaT: None}, inplace=True)
+        return df
+
+    def convert_to_decimal(self, val):
+        """This is updated method to solve the issue of converting to decimal
+        previously I use the method below, but it will cause the precision issue
+        df[c] = df[c].astype(str).map(decimal.Decimal)
+
+        Args:
+            val (Any): the input value from table
+
+        Returns:
+            Decimal: Decimal value to pass into bigquery
+        """
+        if pd.isna(val):
+            return None
+        if isinstance(val, float):
+            return decimal.Decimal(str(val))
+        else:
+            return decimal.Decimal(val)
+
+    def convert_boolean_cols(self, df, col):
+        try:
+            df[col] = df[col].astype(int)
+        except Exception as e:
+            pass
+        df[col] = df[col].astype("bool")
+        return df
+
+    def convert_float_cols(self, df, col):
+        try:
+            df[col] = df[col].astype(float)
+        except Exception as e:
+            pass
+        return df
+
+    # def read_data_from_s3(self, s3_filepath):
+    #     _temp_file_path = f"./{uuid.uuid4().hex}.tempfile"
+    #     self.s3.download_file(s3_filepath, _temp_file_path)
+    #     if s3_filepath.endswith(".csv"):
+    #         df = pd.read_csv(_temp_file_path, dtype=str)
+    #     elif s3_filepath.endswith(".xlsx"):
+    #         df = pd.read_excel(_temp_file_path, dtype=str, engine="openpyxl")
+    #     else:
+    #         raise NotImplementedError(
+    #             f"the input file is not supported yet: {s3_filepath}"
+    #         )
+    #     os.remove(_temp_file_path)
+    #     print(f"data size {df.shape}")
+    #     return df
+
+    def run_sql(self, sql):
+        query_job = self.client.query(sql)
+        results = query_job.result()
+        return results
+
+    def clear_table(self, dataset_id, table_id):
+        """remove all records from the table, the target table must exists to run this
+
+        Args:
+                dataset_id (str): schema_name/dataset_id
+                table_id (str): table_name/table_id
+        """
+        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
+        sql = f"TRUNCATE TABLE {full_qualified_id}"
+        self.run_sql(sql)
+
+    def get_schema_from_existing_table(self, dataset_id, table_id):
+        full_qualified_id = self.__get_full_qualified_table_name(dataset_id, table_id)
+        table = self.client.get_table(full_qualified_id)
+        return table.schema
+
+    def generate_merge_on_key(self, col_key):
+        txt = ""
+        for col in col_key:
+            _t = f"t.{col} = s.{col}"
+            if col != col_key[-1]:
+                _t = f"{_t} AND "
+            txt += _t
+        return txt
+
+    def generate_sql_merge_update_set(self, columns, col_key):
+        columns = [c for c in columns if c.lower() not in col_key]
+        n_col = len(columns)
+        txt = ""
+        for index, col in enumerate(columns):
+            if col == "update_mode":
+                txt += f"t.{col} = 'UPDATE',\n"
+            elif not (index + 1) == n_col:
+                txt += f"t.{col} = s.{col},\n"
+            else:
+                txt += f"t.{col} = s.{col}\n"
+        return txt
+
+    def generate_sql_merge_insert_set(self, columns):
+        col_txt = ",".join(columns)
+        col_txt_value = ""
+        for col in columns:
+            col_txt_value += f"s.{col},"
+        col_txt_value = col_txt_value[:-1]
+        # final text to output
+        txt_final = f"""
+		INSERT({col_txt})
+		VALUES({col_txt_value})
+		"""
+        return txt_final
+
+    def create_external_table_from_gcs(
+        self,
+        table_id: str,
+        gcs_uri: str,
+        file_type: str,
+        connection_id: Union[str, None] = None,
+        is_hive_partition: bool = False,
+        schema: Union[List[bigquery.SchemaField], None] = None,
+    ) -> "bigquery.Table":  # type: ignore
+        # table_id = "your-project.your_dataset.your_table_name"
+        # gcs_uri = "gs://cto-ris-cds-prd_converted/test/cds/jda/outbound/JDASKU/*"
+        # source_uri_prefix = "gs://cto-ris-cds-prd_converted/test/cds/jda/outbound/JDASKU/"
+        # Example usage: gbq.create_external_table_from_gcs(table_id=table_id,schema=None,gcs_uri=gcs_uri,avro_or_parquet='AVRO',is_hive_partition=True)
+        # ================================= Choose file format =================================
+        if file_type.upper() == "AVRO":
+            external_config = bigquery.ExternalConfig("AVRO")
+        elif file_type.upper() == "PARQUET":
+            external_config = bigquery.ExternalConfig("PARQUET")
+        elif file_type.upper() == "NEWLINE_DELIMITED_JSON":
+            external_config = bigquery.ExternalConfig("NEWLINE_DELIMITED_JSON")
+        else:
+            raise NotImplementedError(f"The {file_type} type is not supported yet")
+        external_config.source_uris = [gcs_uri]
+        if connection_id:
+            external_config.connection_id = connection_id
+        source_uri_prefix = gcs_uri[:-1]
+        # ================================= Set Hive partition config =================================
+        if is_hive_partition:
+            hive_partitioning_opts = bigquery.HivePartitioningOptions() # type: ignore
+            hive_partitioning_opts.mode = "AUTO"
+            hive_partitioning_opts.require_partition_filter = False
+            hive_partitioning_opts.source_uri_prefix = source_uri_prefix
+            external_config.hive_partitioning = hive_partitioning_opts
+        # ================================= Set external table config =================================
+        if schema is None:
+            external_config.autodetect = True
+            table = bigquery.Table(table_id)
+        else:
+            table = bigquery.Table(table_id, schema=schema)
+        table.external_data_configuration = external_config
+        # ================================= Create table =================================
+        try:
+            table = self.client.create_table(table)  # Make an API request.
+        except Exception as e:
+            if "Already Exists: Table" in e.args[0]:
+                print(f"Table already exists: {table_id}")
+            else:
+                raise ValueError(e)
+        else:
+            return table
+
+    def get_schema_policy_tag(
+        self,
+        col_name,
+        col_type,
+        col_mode,
+        policy_tag_id: Union[str, None] = None,
+        fields: Union[List[bigquery.SchemaField], None] = None,
+        desc: str = "No description",
+    ):
+        """Add policy tag to the BigQuery table schema
+        Args:
+            col_name (tr): the name of the column
+            col_type (str): the type of the column, e.g. STRING, INTEGER, FLOAT, etc.
+            col_mode (str): the mode of the column, e.g. NULLABLE, REQUIRED, REPEATED
+            policy_tag_id (str, optional): The policy tag full id. Defaults to None. example: projects/myproject/locations/asia-southeast1/taxonomies/11111111111111111111/policyTags/22222222222222222
+        Returns:
+            bigquery.SchemaField: the schema field with policy tag or without it
+        """
+        bq_policy = bigquery.PolicyTagList(names=[policy_tag_id])  # type: ignore
+        if fields is None:
+            fields = []
+        if policy_tag_id:
+            return bigquery.SchemaField(
+                name=col_name,
+                field_type=col_type,
+                mode=col_mode,
+                description=desc,
+                fields=fields,
+                policy_tags=bq_policy,
+            )
+        else:
+            return bigquery.SchemaField(
+                name=col_name,
+                field_type=col_type,
+                mode=col_mode,
+                description=desc,
+                fields=fields,
+            )
+
+    def create_external_table_from_google_sheets(
+        self,
+        table_id: str,
+        ext_config: Union[bigquery.ExternalConfig, None] = None,
+        uri: str = "",
+        schema: Union[List[bigquery.SchemaField], None] = None,
+    ) -> None:
+        table = bigquery.Table(table_id, schema=schema)
+        if ext_config:
+            table.external_data_configuration = ext_config
+        else:
+            external_cfg = bigquery.ExternalConfig("GOOGLE_SHEETS")
+            external_cfg.source_uris = [uri]
+            external_cfg.options.skip_leading_rows = 1  # type: ignore
+            # external_cfg.autodetect = True
+            # external_cfg.max_bad_records = 2
+            external_cfg.ignore_unknown_values = False
+            table.external_data_configuration = external_cfg
+        table = self.client.create_table(table)
+        print(table)
+
+    # ================================= Get data from GBQ =================================
+    def get_data_from_gbq(self, sql: str) -> pd.DataFrame:
+        # sql = "SELECT * FROM `bigquery-public-data.irs_990.irs_990_2012`"
+        # need package: google-cloud-bigquery-storage, pyarrow
+        return self.client.query(sql).to_dataframe()
```

### Comparing `npgbq-2.1.7/npgbq.egg-info/SOURCES.txt` & `npgbq-2.1.8/npgbq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `npgbq-2.1.7/setup.py` & `npgbq-2.1.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import pathlib
-
-from setuptools import find_packages, setup
-
-here = pathlib.Path(__file__).parent.resolve()
-
-# Read long description from the readme.md file
-with open("README.md") as f:
-    readme = f.read()
-
-with open("LICENSE") as f:
-    license = f.read()
-
-setup(
-    name="npgbq",
-    version="2.1.7",
-    description="A package designed for helping everyone in the team to work with data ingestion",
-    long_description_content_type="text/markdown",
-    long_description=readme,
-    author="Nopporn Phantawee",
-    author_email="n.phantawee@gmail.com",
-    url="https://github.com/noppGithub/npgbq",
-    license="MIT",
-    packages=find_packages(exclude=("tests", "docs")),
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-    ],
-    install_requires=[
-        "fastparquet",
-        "google-cloud-bigquery",
-        "google-cloud-logging",
-        "openpyxl",
-        "pandas",
-        "pyarrow",
-        "requests",
-        "psycopg2-binary",
-        "pyodbc",
-        "db-dtypes",
-    ],
-    extras_require={
-        "dev": ["check-manifest"],
-        "test": ["coverage"],
-    },
-    python_requires=">=3.6, <4",
-)
+import pathlib
+
+from setuptools import find_packages, setup
+
+here = pathlib.Path(__file__).parent.resolve()
+
+# Read long description from the readme.md file
+with open("README.md") as f:
+    readme = f.read()
+
+with open("LICENSE") as f:
+    license = f.read()
+
+setup(
+    name="npgbq",
+    version="2.1.8",
+    description="A package designed for helping everyone in the team to work with data ingestion",
+    long_description_content_type="text/markdown",
+    long_description=readme,
+    author="Nopporn Phantawee",
+    author_email="n.phantawee@gmail.com",
+    url="https://github.com/noppGithub/npgbq",
+    license="MIT",
+    packages=find_packages(exclude=("tests", "docs")),
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+    ],
+    install_requires=[
+        "fastparquet",
+        "google-cloud-bigquery",
+        "google-cloud-logging",
+        "openpyxl",
+        "pandas",
+        "pyarrow",
+        "requests",
+        "psycopg2-binary",
+        "pyodbc",
+        "db-dtypes",
+    ],
+    extras_require={
+        "dev": ["check-manifest"],
+        "test": ["coverage"],
+    },
+    python_requires=">=3.6, <4",
+)
```

### Comparing `npgbq-2.1.7/tests/test_load_scbpt_saleorder.py` & `npgbq-2.1.8/tests/test_load_scbpt_saleorder.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from npgbq import NPGBQ
-import pandas as pd
-
-
-if __name__ == "__main__":
-    gbq_service_account_path = r"D:\np\npgbq\scbpt_bq_admin.json"
-
-    # ====================================== create instance ======================================
-    gbq = NPGBQ(gbq_service_account_path=gbq_service_account_path)
-
-    # ====================================== 0. create log table and insert some log ======================================
-    # gbq.create_log_table()
-    # gbq.log2bq(message="hello test")
-
-    # ====================================== 1. sale order ======================================
-    dataset_name = "scbpt_dataset"
-    table_name = "order_campaign"
-    loading_mode = "truncate"
-
-    fp = "./data/sale_order_province_url.xlsx"
-    df = pd.read_excel(fp, engine="openpyxl", dtype=str)
-
-    schema_dict = {
-        "applicationformid": "STRING",
-        "paymentmethod": "STRING",
-        "insurer": "STRING",
-        "producttype": "STRING",
-        "producttemplatename": "STRING",
-        "packagename": "STRING",
-        "packagepackagecode": "STRING",
-        "paymentmode": "STRING",
-        "maintotalpremium": "FLOAT",
-        "mainvatpremium": "FLOAT",
-        "mainnetpremium": "FLOAT",
-        "mainstamppremium": "FLOAT",
-        "addontotalpremium": "FLOAT",
-        "addonnetpremium": "FLOAT",
-        "addonvatpremium": "FLOAT",
-        "addonstamppremium": "FLOAT",
-        "coupondiscount": "FLOAT",
-        "discount": "FLOAT",
-        "status": "STRING",
-        "status1": "STRING",
-        "upfrontdiscount": "FLOAT",
-        "totalpremium": "FLOAT",
-        "discountcode": "STRING",
-        "absorbinterest": "STRING",
-        "installmentperiod": "INTEGER",
-        "installmenttype": "STRING",
-        "installmentrate": "FLOAT",
-        "age": "INTEGER",
-        "applicationformcode": "STRING",
-        "province": "STRING",
-        "district": "STRING",
-        "subdistrict": "STRING",
-        "addresstype": "STRING",
-        "payment_year": "INTEGER",
-        "payment_month": "INTEGER",
-        "payment_day": "INTEGER",
-        "payment_timestamp": "TIMESTAMP",
-        "payment_yearmonth": "STRING",
-        "payment_hour": "INTEGER",
-        "payment_weekday": "STRING",
-        "campaign_name": "STRING",
-        "campaign_start_date_sitecore": "DATE",
-        "campaign_end_date_sitecore": "DATE",
-        "facet1_medium": "STRING",
-        "facet2_traffic_src": "STRING",
-        "facet4_product_type": "STRING",
-        "facet5_objectives": "STRING",
-        "campaign_channel": "STRING",
-        "campaign_group": "STRING",
-        "campaign_id_from_sitecore": "STRING",
-        "lat": "FLOAT",
-        "long": "FLOAT",
-        "province_eng": "STRING",
-        "payment_date": "DATE",
-        "producttype_group": "INTEGER",
-    }
-    rename_dict = {}
-
-    dtype_config = gbq.generate_dtype_from_schema(schema_dict)
-    df = gbq.convert_dtype(df, dtype_config)
-    schema = gbq.generate_bq_schema_from_dict(schema_dict)
-    gbq.create_bq_dataset(dataset_name)
-    # gbq.delete_bq_table(dataset_name, table_name)
-    gbq.create_bq_table(dataset_name, table_id=table_name, schema=schema)
-    gbq.insert_dataframe_to_bq_table(
-        df, dataset_name, table_name, schema, mode=loading_mode
-    )
+from npgbq import NPGBQ
+import pandas as pd
+
+
+if __name__ == "__main__":
+    gbq_service_account_path = r"D:\np\npgbq\scbpt_bq_admin.json"
+
+    # ====================================== create instance ======================================
+    gbq = NPGBQ(gbq_service_account_path=gbq_service_account_path)
+
+    # ====================================== 0. create log table and insert some log ======================================
+    # gbq.create_log_table()
+    # gbq.log2bq(message="hello test")
+
+    # ====================================== 1. sale order ======================================
+    dataset_name = "scbpt_dataset"
+    table_name = "order_campaign"
+    loading_mode = "truncate"
+
+    fp = "./data/sale_order_province_url.xlsx"
+    df = pd.read_excel(fp, engine="openpyxl", dtype=str)
+
+    schema_dict = {
+        "applicationformid": "STRING",
+        "paymentmethod": "STRING",
+        "insurer": "STRING",
+        "producttype": "STRING",
+        "producttemplatename": "STRING",
+        "packagename": "STRING",
+        "packagepackagecode": "STRING",
+        "paymentmode": "STRING",
+        "maintotalpremium": "FLOAT",
+        "mainvatpremium": "FLOAT",
+        "mainnetpremium": "FLOAT",
+        "mainstamppremium": "FLOAT",
+        "addontotalpremium": "FLOAT",
+        "addonnetpremium": "FLOAT",
+        "addonvatpremium": "FLOAT",
+        "addonstamppremium": "FLOAT",
+        "coupondiscount": "FLOAT",
+        "discount": "FLOAT",
+        "status": "STRING",
+        "status1": "STRING",
+        "upfrontdiscount": "FLOAT",
+        "totalpremium": "FLOAT",
+        "discountcode": "STRING",
+        "absorbinterest": "STRING",
+        "installmentperiod": "INTEGER",
+        "installmenttype": "STRING",
+        "installmentrate": "FLOAT",
+        "age": "INTEGER",
+        "applicationformcode": "STRING",
+        "province": "STRING",
+        "district": "STRING",
+        "subdistrict": "STRING",
+        "addresstype": "STRING",
+        "payment_year": "INTEGER",
+        "payment_month": "INTEGER",
+        "payment_day": "INTEGER",
+        "payment_timestamp": "TIMESTAMP",
+        "payment_yearmonth": "STRING",
+        "payment_hour": "INTEGER",
+        "payment_weekday": "STRING",
+        "campaign_name": "STRING",
+        "campaign_start_date_sitecore": "DATE",
+        "campaign_end_date_sitecore": "DATE",
+        "facet1_medium": "STRING",
+        "facet2_traffic_src": "STRING",
+        "facet4_product_type": "STRING",
+        "facet5_objectives": "STRING",
+        "campaign_channel": "STRING",
+        "campaign_group": "STRING",
+        "campaign_id_from_sitecore": "STRING",
+        "lat": "FLOAT",
+        "long": "FLOAT",
+        "province_eng": "STRING",
+        "payment_date": "DATE",
+        "producttype_group": "INTEGER",
+    }
+    rename_dict = {}
+
+    dtype_config = gbq.generate_dtype_from_schema(schema_dict)
+    df = gbq.convert_dtype(df, dtype_config)
+    schema = gbq.generate_bq_schema_from_dict(schema_dict)
+    gbq.create_bq_dataset(dataset_name)
+    # gbq.delete_bq_table(dataset_name, table_name)
+    gbq.create_bq_table(dataset_name, table_id=table_name, schema=schema)
+    gbq.insert_dataframe_to_bq_table(
+        df, dataset_name, table_name, schema, mode=loading_mode
+    )
```

### Comparing `npgbq-2.1.7/tests/test_oracle_ingest.py` & `npgbq-2.1.8/tests/test_oracle_ingest.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import logging
-import os
-import platform
-from io import BytesIO
-from pathlib import Path
-
-import cx_Oracle
-import pandas as pd
-from npgcs import NPGCS
-
-from npgbq import NPGBQ
-
-log_dir = "./log"
-Path(log_dir).mkdir(exist_ok=True, parents=True)
-log_path = str(Path(log_dir).joinpath(Path(__file__).stem)) + ".log"
-
-logger = logging.getLogger(__name__)
-logger.propagate = False  # remove duplicated log
-logger.setLevel(logging.DEBUG)
-formatter = logging.Formatter("%(asctime)s:%(levelname)s:%(name)s:%(message)s")
-stream_handler = logging.StreamHandler()
-stream_handler.setLevel(logging.INFO)
-stream_handler.setFormatter(formatter)
-logger.addHandler(stream_handler)
-file_handler = logging.FileHandler(
-    log_path, mode="a", encoding="utf-8", delay=False
-)
-file_handler.setLevel(logging.DEBUG)
-file_handler.setFormatter(formatter)
-logger.addHandler(file_handler)
-# ================================= Oracle settings =================================
-# provide the path contain Oracle client manually
-LOCATION = r"D:\np\central-crv\oracle_client\instantclient_19_5"
-LOCATION = "./oracle_client/instantclient_21_7"
-print("ARCH:", platform.architecture())
-files_at_location = []
-for name in os.listdir(LOCATION):
-    files_at_location.append(name)
-os.environ["PATH"] = LOCATION + ";" + os.environ["PATH"]
-
-# credentails
-username = "pocmigration"
-password = "RaQ7075RI6"
-dsn = "GOLD"
-
-# create DNS_TNS with particular users
-dsn_tns = cx_Oracle.makedsn("192.168.200.130", "1521", service_name="GOLD")
-conn = cx_Oracle.connect(
-    user="pocmigration",
-    password="RaQ7075RI6",
-    dsn=dsn_tns,
-    encoding="US-ASCII",
-    nencoding="utf-8",
-)
-
-
-tables = [
-    "REPLACEME_LOL",
-    # "HUONGNGUYEN.SC_STR_SUP_062022_CURRENT_VIZ",
-]
-
-table_completed = [
-    # "HUONGNGUYEN.SC_WH_SUP_102021_052022_VIZ",
-    # "QUYENNGUYEN.SC_STORE_WH_SKU",
-]
-
-# ================================= Functions =================================
-def get_columns_info(conn, schema_name=None, table_name=None) -> pd.DataFrame:
-    if schema_name is not None:
-        sql = f"SELECT * FROM all_tab_cols where OWNER='{schema_name}' and TABLE_NAME='{table_name}'"
-        sql = f"""
-        SELECT * 
-        FROM all_tab_cols 
-        where OWNER='{schema_name}' 
-        and TABLE_NAME='{table_name}'
-        and COLUMN_ID is not null order by OWNER, TABLE_NAME,COLUMN_ID
-        """
-    else:
-        sql = f"SELECT * FROM all_tab_cols WHERE COLUMN_ID is not null order by OWNER, TABLE_NAME,COLUMN_ID"
-    return pd.read_sql(sql, conn)
-
-
-def get_schema_dict(df: pd.DataFrame):
-    schema_dict = {}
-    for index, row in df.iterrows():
-        schema_dict[row["object_name"]] = row["schema_name"]
-    return schema_dict
-
-
-def get_schema_org_dict(df: pd.DataFrame) -> dict:
-    output = {}
-    for index, row in df[["COLUMN_NAME", "DATA_TYPE"]].iterrows():
-        output[row["COLUMN_NAME"]] = row["DATA_TYPE"]
-    return output
-
-
-if __name__ == "__main__":
-    # chunksize = 100000
-    CHUNK_SIZE = 100000
-    # gcs
-    project_id = "cto-crv-dev"
-    bucket_name = "crv_gold"
-    dataset_id = "gold"
-    gcs = NPGCS(project_id=project_id)
-    gbq = NPGBQ(project_id=project_id)
-
-    # filter only the table that not completed
-    tables = [table for table in tables if table not in table_completed]
-
-    # loop over tables
-    for table in tables:
-        logger.info(f"Start {table}")
-        # count number of rows
-        sql = f"SELECT COUNT(*) FROM {table}"
-        df_count = pd.read_sql(sql, conn)
-        logger.info(f"Total number of rows {table}: {df_count.iloc[0,0]:,}")
-
-        # get schema and table name from the table
-        schema_name, table_name = table.split(".")
-
-        # in each table get the information schema from oracle
-        _df = get_columns_info(conn, schema_name, table_name)
-        schema_original = get_schema_org_dict(_df)
-        logger.info(f"Schema original {schema_original}")
-
-        # generate schema_dict from the information schema
-        schema_dict = gbq.get_schema_dict_from_db(_df, db_engine="oracle")
-        schema_bq = gbq.generate_bq_schema_from_dict(schema_dict)
-        rename_dict = gbq.get_col_rename_dict(schema_original, schema_dict)
-        logger.info(f"Schema_dict {schema_dict}")
-
-        # iterate over the table with chunksize
-        file_count, n_recs = 0, 0
-        blob_path = None
-        logger.info(f"Extracting from table {table}")
-        sql_table = f"""
-        SELECT * FROM {table}
-        """
-        for df in pd.read_sql(
-            sql_table,
-            conn,
-            chunksize=CHUNK_SIZE,
-        ):
-            # convert the data type to the correct type
-            logger.info(f"Converting data type {df.shape}")
-            df = gbq.rename_columns(df, rename_dict)
-            df = gbq.convert_dtype(df, schema_bq)
-
-            # upload to gcs
-            logger.info(f"Saving as byte")
-            fo = BytesIO()
-            df.to_parquet(fo, engine="pyarrow", compression="gzip")
-            fo.seek(0)
-            blob_path = f"{schema_name}/{table_name}"
-            blob_name = f"{blob_path}/{schema_name}_{table_name}_part_{file_count:09d}.parquet"
-            logger.info(f"Uploading to GCS {blob_name}")
-            gcs.upload_blob_from_stream(
-                bucket_name, file_obj=fo, destination_blob_name=blob_name
-            )
-
-            # update file_count
-            file_count += 1
-            n_recs += df.shape[0]
-            logger.info(f"Part done {file_count} : {n_recs} records")
-        logger.info(
-            f"Extracted data from {table} to GCS, Total {file_count} files, {n_recs} records"
-        )
-        # create external table in BigQuery
-        if blob_path is not None:
-            table_id = f"{project_id}.{dataset_id}.{schema_name}_{table_name}"
-            logger.info(f"Creating table {table_id}")
-            gcs_uri = f"gs://{bucket_name}/{blob_path}/*.parquet"
-            gbq.create_external_table_from_gcs(table_id, schema_bq, gcs_uri)
-        logger.info(f"Completed {table}")
+import logging
+import os
+import platform
+from io import BytesIO
+from pathlib import Path
+
+import cx_Oracle
+import pandas as pd
+from npgcs import NPGCS
+
+from npgbq import NPGBQ
+
+log_dir = "./log"
+Path(log_dir).mkdir(exist_ok=True, parents=True)
+log_path = str(Path(log_dir).joinpath(Path(__file__).stem)) + ".log"
+
+logger = logging.getLogger(__name__)
+logger.propagate = False  # remove duplicated log
+logger.setLevel(logging.DEBUG)
+formatter = logging.Formatter("%(asctime)s:%(levelname)s:%(name)s:%(message)s")
+stream_handler = logging.StreamHandler()
+stream_handler.setLevel(logging.INFO)
+stream_handler.setFormatter(formatter)
+logger.addHandler(stream_handler)
+file_handler = logging.FileHandler(
+    log_path, mode="a", encoding="utf-8", delay=False
+)
+file_handler.setLevel(logging.DEBUG)
+file_handler.setFormatter(formatter)
+logger.addHandler(file_handler)
+# ================================= Oracle settings =================================
+# provide the path contain Oracle client manually
+LOCATION = r"D:\np\central-crv\oracle_client\instantclient_19_5"
+LOCATION = "./oracle_client/instantclient_21_7"
+print("ARCH:", platform.architecture())
+files_at_location = []
+for name in os.listdir(LOCATION):
+    files_at_location.append(name)
+os.environ["PATH"] = LOCATION + ";" + os.environ["PATH"]
+
+# credentails
+username = "pocmigration"
+password = "RaQ7075RI6"
+dsn = "GOLD"
+
+# create DNS_TNS with particular users
+dsn_tns = cx_Oracle.makedsn("192.168.200.130", "1521", service_name="GOLD")
+conn = cx_Oracle.connect(
+    user="pocmigration",
+    password="RaQ7075RI6",
+    dsn=dsn_tns,
+    encoding="US-ASCII",
+    nencoding="utf-8",
+)
+
+
+tables = [
+    "REPLACEME_LOL",
+    # "HUONGNGUYEN.SC_STR_SUP_062022_CURRENT_VIZ",
+]
+
+table_completed = [
+    # "HUONGNGUYEN.SC_WH_SUP_102021_052022_VIZ",
+    # "QUYENNGUYEN.SC_STORE_WH_SKU",
+]
+
+# ================================= Functions =================================
+def get_columns_info(conn, schema_name=None, table_name=None) -> pd.DataFrame:
+    if schema_name is not None:
+        sql = f"SELECT * FROM all_tab_cols where OWNER='{schema_name}' and TABLE_NAME='{table_name}'"
+        sql = f"""
+        SELECT * 
+        FROM all_tab_cols 
+        where OWNER='{schema_name}' 
+        and TABLE_NAME='{table_name}'
+        and COLUMN_ID is not null order by OWNER, TABLE_NAME,COLUMN_ID
+        """
+    else:
+        sql = f"SELECT * FROM all_tab_cols WHERE COLUMN_ID is not null order by OWNER, TABLE_NAME,COLUMN_ID"
+    return pd.read_sql(sql, conn)
+
+
+def get_schema_dict(df: pd.DataFrame):
+    schema_dict = {}
+    for index, row in df.iterrows():
+        schema_dict[row["object_name"]] = row["schema_name"]
+    return schema_dict
+
+
+def get_schema_org_dict(df: pd.DataFrame) -> dict:
+    output = {}
+    for index, row in df[["COLUMN_NAME", "DATA_TYPE"]].iterrows():
+        output[row["COLUMN_NAME"]] = row["DATA_TYPE"]
+    return output
+
+
+if __name__ == "__main__":
+    # chunksize = 100000
+    CHUNK_SIZE = 100000
+    # gcs
+    project_id = "cto-crv-dev"
+    bucket_name = "crv_gold"
+    dataset_id = "gold"
+    gcs = NPGCS(project_id=project_id)
+    gbq = NPGBQ(project_id=project_id)
+
+    # filter only the table that not completed
+    tables = [table for table in tables if table not in table_completed]
+
+    # loop over tables
+    for table in tables:
+        logger.info(f"Start {table}")
+        # count number of rows
+        sql = f"SELECT COUNT(*) FROM {table}"
+        df_count = pd.read_sql(sql, conn)
+        logger.info(f"Total number of rows {table}: {df_count.iloc[0,0]:,}")
+
+        # get schema and table name from the table
+        schema_name, table_name = table.split(".")
+
+        # in each table get the information schema from oracle
+        _df = get_columns_info(conn, schema_name, table_name)
+        schema_original = get_schema_org_dict(_df)
+        logger.info(f"Schema original {schema_original}")
+
+        # generate schema_dict from the information schema
+        schema_dict = gbq.get_schema_dict_from_db(_df, db_engine="oracle")
+        schema_bq = gbq.generate_bq_schema_from_dict(schema_dict)
+        rename_dict = gbq.get_col_rename_dict(schema_original, schema_dict)
+        logger.info(f"Schema_dict {schema_dict}")
+
+        # iterate over the table with chunksize
+        file_count, n_recs = 0, 0
+        blob_path = None
+        logger.info(f"Extracting from table {table}")
+        sql_table = f"""
+        SELECT * FROM {table}
+        """
+        for df in pd.read_sql(
+            sql_table,
+            conn,
+            chunksize=CHUNK_SIZE,
+        ):
+            # convert the data type to the correct type
+            logger.info(f"Converting data type {df.shape}")
+            df = gbq.rename_columns(df, rename_dict)
+            df = gbq.convert_dtype(df, schema_bq)
+
+            # upload to gcs
+            logger.info(f"Saving as byte")
+            fo = BytesIO()
+            df.to_parquet(fo, engine="pyarrow", compression="gzip")
+            fo.seek(0)
+            blob_path = f"{schema_name}/{table_name}"
+            blob_name = f"{blob_path}/{schema_name}_{table_name}_part_{file_count:09d}.parquet"
+            logger.info(f"Uploading to GCS {blob_name}")
+            gcs.upload_blob_from_stream(
+                bucket_name, file_obj=fo, destination_blob_name=blob_name
+            )
+
+            # update file_count
+            file_count += 1
+            n_recs += df.shape[0]
+            logger.info(f"Part done {file_count} : {n_recs} records")
+        logger.info(
+            f"Extracted data from {table} to GCS, Total {file_count} files, {n_recs} records"
+        )
+        # create external table in BigQuery
+        if blob_path is not None:
+            table_id = f"{project_id}.{dataset_id}.{schema_name}_{table_name}"
+            logger.info(f"Creating table {table_id}")
+            gcs_uri = f"gs://{bucket_name}/{blob_path}/*.parquet"
+            gbq.create_external_table_from_gcs(table_id, schema_bq, gcs_uri)
+        logger.info(f"Completed {table}")
```

### Comparing `npgbq-2.1.7/tests/test_script.py` & `npgbq-2.1.8/tests/test_script.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from npgbq import NPGBQ
-import pandas as pd
-
-
-if __name__ == "__main__":
-    gbq_service_account_path = r"D:\np\npgbq\scbpt_bq_admin.json"
-
-    # ====================================== create instance ======================================
-    gbq = NPGBQ(gbq_service_account_path=gbq_service_account_path)
-
-    # ====================================== 0. create log table and insert some log ======================================
-    gbq.create_log_table()
-    gbq.log2bq(message="hello test")
-
-    # ====================================== 1. load from dataframe ======================================
-    dataset_name = "zz_test"
-    table_name = "from_dataframe"
-    loading_mode = "truncate"
-    data = [
-        {"firstname": "nopporn1", "lastname": "phantawee", "age": 33},
-        {"firstname": "nopporn2", "lastname": "phantawee2", "age": 34},
-    ]
-    df = pd.DataFrame(data)
-    schema_dict = {
-        "firstname": "STRING",
-        "lastname": "STRING",
-        "age": "INT64",
-    }
-    schema = gbq.generate_bq_schema_from_dict(schema_dict)
-    gbq.create_bq_dataset(dataset_name)
-    gbq.create_bq_table(dataset_name, table_id=table_name, schema=schema)
-
-    # insert data
-    gbq.insert_dataframe_to_bq_table(
-        df, dataset_name, table_name, schema, mode=loading_mode
-    )
+from npgbq import NPGBQ
+import pandas as pd
+
+
+if __name__ == "__main__":
+    gbq_service_account_path = r"D:\np\npgbq\scbpt_bq_admin.json"
+
+    # ====================================== create instance ======================================
+    gbq = NPGBQ(gbq_service_account_path=gbq_service_account_path)
+
+    # ====================================== 0. create log table and insert some log ======================================
+    gbq.create_log_table()
+    gbq.log2bq(message="hello test")
+
+    # ====================================== 1. load from dataframe ======================================
+    dataset_name = "zz_test"
+    table_name = "from_dataframe"
+    loading_mode = "truncate"
+    data = [
+        {"firstname": "nopporn1", "lastname": "phantawee", "age": 33},
+        {"firstname": "nopporn2", "lastname": "phantawee2", "age": 34},
+    ]
+    df = pd.DataFrame(data)
+    schema_dict = {
+        "firstname": "STRING",
+        "lastname": "STRING",
+        "age": "INT64",
+    }
+    schema = gbq.generate_bq_schema_from_dict(schema_dict)
+    gbq.create_bq_dataset(dataset_name)
+    gbq.create_bq_table(dataset_name, table_id=table_name, schema=schema)
+
+    # insert data
+    gbq.insert_dataframe_to_bq_table(
+        df, dataset_name, table_name, schema, mode=loading_mode
+    )
```

