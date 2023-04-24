# Comparing `tmp/mtsql-1.4.202304230628-py3-none-any.whl.zip` & `tmp/mtsql-1.4.202304241627-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19131 bytes, number of entries: 11
+Zip file size: 19248 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
 -rw-r--r--  2.0 unx     9989 b- defN 23-Apr-23 06:23 mt/sql/base.py
 -rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
--rw-r--r--  2.0 unx    64376 b- defN 23-Apr-23 06:28 mt/sql/psql.py
+-rw-r--r--  2.0 unx    65289 b- defN 23-Apr-24 16:26 mt/sql/psql.py
 -rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 23-Apr-23 06:28 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/LICENSE
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/RECORD
-11 files, 91002 bytes uncompressed, 17677 bytes compressed:  80.6%
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-24 16:27 mt/sql/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-24 16:27 mtsql-1.4.202304241627.dist-info/LICENSE
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-24 16:27 mtsql-1.4.202304241627.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 16:27 mtsql-1.4.202304241627.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Apr-24 16:27 mtsql-1.4.202304241627.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-Apr-24 16:27 mtsql-1.4.202304241627.dist-info/RECORD
+11 files, 91915 bytes uncompressed, 17794 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.4.202304230628.dist-info/LICENSE
+Filename: mtsql-1.4.202304241627.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.4.202304230628.dist-info/METADATA
+Filename: mtsql-1.4.202304241627.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.4.202304230628.dist-info/WHEEL
+Filename: mtsql-1.4.202304241627.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.4.202304230628.dist-info/top_level.txt
+Filename: mtsql-1.4.202304241627.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.4.202304230628.dist-info/RECORD
+Filename: mtsql-1.4.202304241627.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/psql.py

```diff
@@ -28,14 +28,15 @@
     "list_foreign_tables",
     "list_frames",
     "list_all_frames",
     "get_frame_length",
     "get_frame_dependencies",
     "get_view_sql_code",
     "rename_table",
+    "vacuum_table",
     "drop_table",
     "rename_view",
     "drop_view",
     "rename_matview",
     "refresh_matview",
     "drop_matview",
     "frame_exists",
@@ -699,22 +700,54 @@
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns
     """
     frame_sql_str = frame_sql(old_table_name, schema=schema)
-    exec_sql(
+    return exec_sql(
         'ALTER TABLE {} RENAME TO "{}";'.format(frame_sql_str, new_table_name),
         engine,
         nb_trials=nb_trials,
         logger=logger,
     )
 
 
+def vacuum_table(
+    table_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+):
+    """Vacuums a table of a schema.
+
+    Parameters
+    ----------
+    table_name: str
+    engine: sqlalchemy.engine.Engine
+        an sqlalchemy connection engine created by function `create_engine()`
+    schema: str or None
+        a valid schema name returned from `list_schemas()`
+    nb_trials: int
+        number of query trials
+    logger: mt.logg.IndentedLoggerAdapter, optional
+        logger for debugging
+
+    Returns
+    -------
+    whatever exec_sql() returns
+    """
+    frame_sql_str = frame_sql(table_name, schema=schema)
+    engine2 = engine.execution_options(isolation_level="AUTOCOMMIT")
+    return exec_sql(
+        f"VACUUM {frame_sql_str};", engine2, nb_trials=nb_trials, logger=logger
+    )
+
+
 def drop_table(
     table_name,
     engine,
     schema: tp.Optional[str] = None,
     restrict=True,
     nb_trials: int = 3,
     logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('04')
-VERSION_DAY = int('23')
-VERSION_HOUR = int('06')
-VERSION_MINUTE = int('28')
+VERSION_DAY = int('24')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('27')
 MAJOR_VERSION = 1
 MINOR_VERSION = 4
-PATCH_VERSION = 202304230628
-version_date = '2023/04/23 06:28'
+PATCH_VERSION = 202304241627
+version_date = '2023/04/24 16:27'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.4.202304230628.dist-info/LICENSE` & `mtsql-1.4.202304241627.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.4.202304230628.dist-info/METADATA` & `mtsql-1.4.202304241627.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.4.202304230628
+Version: 1.4.202304241627
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

## Comparing `mtsql-1.4.202304230628.dist-info/RECORD` & `mtsql-1.4.202304241627.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mt/sql/__init__.py,sha256=b7zO50apZxt9Hg2eOkJhRLrXgACR8eS5b-Rphdn5qNQ,44
 mt/sql/base.py,sha256=I5ZcfcWKY7Bg6NmZJDCq94xSuXFA5qFO6GWneBGVStA,9989
 mt/sql/mysql.py,sha256=n2ENDctdUqZuSaDAcrqZYtPtawq3Wx4dOPCRsCB5Q4w,4894
-mt/sql/psql.py,sha256=SJ5mK3DpyGa-vOG_Yt3TzzpYqU_6kkZ-fP12xaQ66Kg,64376
+mt/sql/psql.py,sha256=k4hSZUe46yTI1ZDvDgPxwrxk-i8x32CGBjvrrSX4PE4,65289
 mt/sql/sqlite.py,sha256=T2ak_hhNi_zRfpg_gp8JhNHn7D2kl4i-Ey6-9ANMtz0,8678
-mt/sql/version.py,sha256=9Aez7g_XA84pYtaOlyJZW4AEAUlBHNUWuJOKMXEJ_4M,396
-mtsql-1.4.202304230628.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtsql-1.4.202304230628.dist-info/METADATA,sha256=E1Dg1hzxKB-N81mLwdGOB_A3UnGAFHRMN870tTer1HE,597
-mtsql-1.4.202304230628.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtsql-1.4.202304230628.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtsql-1.4.202304230628.dist-info/RECORD,,
+mt/sql/version.py,sha256=W-dGNcI8G_gb7QgAa3vvEEu7v3MNRbDSVksTXVK5g9c,396
+mtsql-1.4.202304241627.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtsql-1.4.202304241627.dist-info/METADATA,sha256=akBcFZt5oewswC1FIzi2yQD-LZd7xE3qsbNHFbDEvkk,597
+mtsql-1.4.202304241627.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtsql-1.4.202304241627.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtsql-1.4.202304241627.dist-info/RECORD,,
```

