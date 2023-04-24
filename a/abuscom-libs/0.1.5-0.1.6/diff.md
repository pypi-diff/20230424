# Comparing `tmp/abuscom-libs-0.1.5.tar.gz` & `tmp/abuscom-libs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuscom-libs-0.1.5.tar", last modified: Wed Apr 19 09:18:34 2023, max compression
+gzip compressed data, was "abuscom-libs-0.1.6.tar", last modified: Mon Apr 24 10:03:14 2023, max compression
```

## Comparing `abuscom-libs-0.1.5.tar` & `abuscom-libs-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.939946 abuscom-libs-0.1.5/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-19 09:18:34.939512 abuscom-libs-0.1.5/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.5/README.md
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.928371 abuscom-libs-0.1.5/abuscom/
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.935422 abuscom-libs-0.1.5/abuscom/connectors/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.5/abuscom/connectors/__init__.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     1887 2023-04-19 09:17:07.000000 abuscom-libs-0.1.5/abuscom/connectors/compass.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     8401 2023-04-13 12:20:45.000000 abuscom-libs-0.1.5/abuscom/connectors/hubspot.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5983 2023-04-07 09:46:30.000000 abuscom-libs-0.1.5/abuscom/connectors/oracle.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.5/abuscom/connectors/planio.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.5/abuscom/connectors/postgres.py
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-19 09:18:34.938708 abuscom-libs-0.1.5/abuscom_libs.egg-info/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/SOURCES.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/dependency_links.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/requires.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-19 09:18:34.000000 abuscom-libs-0.1.5/abuscom_libs.egg-info/top_level.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-19 09:18:34.940172 abuscom-libs-0.1.5/setup.cfg
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-19 09:17:30.000000 abuscom-libs-0.1.5/setup.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.772857 abuscom-libs-0.1.6/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-24 10:03:14.772381 abuscom-libs-0.1.6/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.6/README.md
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.759965 abuscom-libs-0.1.6/abuscom/
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.767988 abuscom-libs-0.1.6/abuscom/connectors/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.6/abuscom/connectors/__init__.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     1887 2023-04-19 09:17:07.000000 abuscom-libs-0.1.6/abuscom/connectors/compass.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     8401 2023-04-13 12:20:45.000000 abuscom-libs-0.1.6/abuscom/connectors/hubspot.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6017 2023-04-24 10:02:05.000000 abuscom-libs-0.1.6/abuscom/connectors/oracle.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.6/abuscom/connectors/planio.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.6/abuscom/connectors/postgres.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-04-24 10:03:14.771789 abuscom-libs-0.1.6/abuscom_libs.egg-info/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/requires.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-04-24 10:03:14.000000 abuscom-libs-0.1.6/abuscom_libs.egg-info/top_level.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-04-24 10:03:14.772991 abuscom-libs-0.1.6/setup.cfg
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-04-24 10:02:05.000000 abuscom-libs-0.1.6/setup.py
```

### Comparing `abuscom-libs-0.1.5/README.md` & `abuscom-libs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.5/abuscom/connectors/compass.py` & `abuscom-libs-0.1.6/abuscom/connectors/compass.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.5/abuscom/connectors/hubspot.py` & `abuscom-libs-0.1.6/abuscom/connectors/hubspot.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.5/abuscom/connectors/oracle.py` & `abuscom-libs-0.1.6/abuscom/connectors/oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         :return: 0 if successful.
         """
         # If clear is True, then clear the table before inserting the rows.
         if clear:
             self.clear_table(tableName=tableName)
         # If there are rows to insert, then bulk-insert them using the OracleHook.
         if tuples:
-            self.ora_hook.bulk_insert_rows(tableName, tuples)
+            self.ora_hook.bulk_insert_rows(table=tableName, rows=tuples, target_fields=columns)
         # Return 0 to indicate success.
         return 0
 
     def load_to_tuples(self, tableName, colNames,where=[]):
         """
         Reads data from an Oracle table and returns it as a list of tuples.
```

### Comparing `abuscom-libs-0.1.5/abuscom/connectors/planio.py` & `abuscom-libs-0.1.6/abuscom/connectors/planio.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.5/abuscom/connectors/postgres.py` & `abuscom-libs-0.1.6/abuscom/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.5/setup.py` & `abuscom-libs-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='abuscom-libs',
-    version='0.1.5',
+    version='0.1.6',
     description='Utility classes for airflow DAGs',
     url='https://abuscom.com',
     author='Leonhard Holzer',
     author_email='leonhard.holzer@abuscom.com',
     license='BSD 2-clause',
     packages=['abuscom.connectors'],
     install_requires=['apache-airflow>=2.4.3',
```

