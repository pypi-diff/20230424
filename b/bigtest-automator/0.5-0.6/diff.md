# Comparing `tmp/bigtest_automator-0.5.tar.gz` & `tmp/bigtest_automator-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtest_automator-0.5.tar", last modified: Sun Apr 23 16:28:26 2023, max compression
+gzip compressed data, was "bigtest_automator-0.6.tar", last modified: Sun Apr 23 16:32:08 2023, max compression
```

## Comparing `bigtest_automator-0.5.tar` & `bigtest_automator-0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.086609 bigtest_automator-0.5/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:28:26.086465 bigtest_automator-0.5/PKG-INFO
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.082526 bigtest_automator-0.5/bigtest_automator.egg-info/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:28:26.000000 bigtest_automator-0.5/bigtest_automator.egg-info/PKG-INFO
--rw-r--r--   0 shantharamp   (502) staff       (20)      871 2023-04-23 16:28:26.000000 bigtest_automator-0.5/bigtest_automator.egg-info/SOURCES.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-23 16:28:26.000000 bigtest_automator-0.5/bigtest_automator.egg-info/dependency_links.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       61 2023-04-23 16:28:26.000000 bigtest_automator-0.5/bigtest_automator.egg-info/entry_points.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-23 16:28:26.000000 bigtest_automator-0.5/bigtest_automator.egg-info/requires.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-23 16:28:26.000000 bigtest_automator-0.5/bigtest_automator.egg-info/top_level.txt
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.083245 bigtest_automator-0.5/core_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.5/core_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6620 2023-04-22 06:17:51.000000 bigtest_automator-0.5/core_utils/generate_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.5/core_utils/run_scp.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.5/core_utils/run_vmstat.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.5/core_utils/take_awr_snapshot.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.083665 bigtest_automator-0.5/entrypoint/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:17:21.000000 bigtest_automator-0.5/entrypoint/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1708 2023-04-23 15:23:40.000000 bigtest_automator-0.5/entrypoint/initialize.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      647 2023-04-23 16:24:30.000000 bigtest_automator-0.5/entrypoint/main_class.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.084657 bigtest_automator-0.5/internal_db_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.5/internal_db_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1236 2023-04-22 06:33:13.000000 bigtest_automator-0.5/internal_db_management/db_ops.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.5/internal_db_management/get_server_details.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1086 2023-04-03 11:48:57.000000 bigtest_automator-0.5/internal_db_management/pwd_handler.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.085175 bigtest_automator-0.5/oracle_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.5/oracle_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.5/oracle_utils/oracle_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.5/oracle_utils/remote_oracle_db_connector.py
--rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-23 16:28:26.086654 bigtest_automator-0.5/setup.cfg
--rw-r--r--   0 shantharamp   (502) staff       (20)      670 2023-04-23 16:27:33.000000 bigtest_automator-0.5/setup.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.085621 bigtest_automator-0.5/temp/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.5/temp/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.5/temp/initiator.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.5/temp/playground.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:28:26.086217 bigtest_automator-0.5/ui_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.5/ui_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.5/ui_management/dynamic_logger.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.5/ui_management/grid.py
--rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.5/ui_management/tk_page_layouts.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.347676 bigtest_automator-0.6/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:32:08.347517 bigtest_automator-0.6/PKG-INFO
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.340962 bigtest_automator-0.6/bigtest_automator.egg-info/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-23 16:32:08.000000 bigtest_automator-0.6/bigtest_automator.egg-info/PKG-INFO
+-rw-r--r--   0 shantharamp   (502) staff       (20)      871 2023-04-23 16:32:08.000000 bigtest_automator-0.6/bigtest_automator.egg-info/SOURCES.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-23 16:32:08.000000 bigtest_automator-0.6/bigtest_automator.egg-info/dependency_links.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       61 2023-04-23 16:32:08.000000 bigtest_automator-0.6/bigtest_automator.egg-info/entry_points.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-23 16:32:08.000000 bigtest_automator-0.6/bigtest_automator.egg-info/requires.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-23 16:32:08.000000 bigtest_automator-0.6/bigtest_automator.egg-info/top_level.txt
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.342346 bigtest_automator-0.6/core_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.6/core_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     6620 2023-04-22 06:17:51.000000 bigtest_automator-0.6/core_utils/generate_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.6/core_utils/run_scp.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.6/core_utils/run_vmstat.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.6/core_utils/take_awr_snapshot.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.343088 bigtest_automator-0.6/entrypoint/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:17:21.000000 bigtest_automator-0.6/entrypoint/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1729 2023-04-23 16:31:52.000000 bigtest_automator-0.6/entrypoint/initialize.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      647 2023-04-23 16:24:30.000000 bigtest_automator-0.6/entrypoint/main_class.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.344178 bigtest_automator-0.6/internal_db_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.6/internal_db_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1236 2023-04-22 06:33:13.000000 bigtest_automator-0.6/internal_db_management/db_ops.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.6/internal_db_management/get_server_details.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1086 2023-04-03 11:48:57.000000 bigtest_automator-0.6/internal_db_management/pwd_handler.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.345072 bigtest_automator-0.6/oracle_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.6/oracle_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.6/oracle_utils/oracle_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.6/oracle_utils/remote_oracle_db_connector.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-23 16:32:08.347723 bigtest_automator-0.6/setup.cfg
+-rw-r--r--   0 shantharamp   (502) staff       (20)      670 2023-04-23 16:32:00.000000 bigtest_automator-0.6/setup.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.346009 bigtest_automator-0.6/temp/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.6/temp/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.6/temp/initiator.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.6/temp/playground.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:32:08.346999 bigtest_automator-0.6/ui_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.6/ui_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.6/ui_management/dynamic_logger.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.6/ui_management/grid.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.6/ui_management/tk_page_layouts.py
```

### Comparing `bigtest_automator-0.5/bigtest_automator.egg-info/SOURCES.txt` & `bigtest_automator-0.6/bigtest_automator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/core_utils/generate_awr.py` & `bigtest_automator-0.6/core_utils/generate_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/core_utils/run_scp.py` & `bigtest_automator-0.6/core_utils/run_scp.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/core_utils/run_vmstat.py` & `bigtest_automator-0.6/core_utils/run_vmstat.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/core_utils/take_awr_snapshot.py` & `bigtest_automator-0.6/core_utils/take_awr_snapshot.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/entrypoint/initialize.py` & `bigtest_automator-0.6/entrypoint/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,10 +50,11 @@
         if con:
             con.close()
 
 def initialize_db():
     if not os.path.exists(os.path.join(os.getcwd(),"internal_db_management","serverdb.db")):
         db_file = os.path.join(os.getcwd(),"internal_db_management","serverdb.db")
         print("Creating database file: "+db_file)
-        open(db_file, 'a').close()
+        with open(db_file, 'w') as fp:
+            pass
         create_tables(db_file)
```

### Comparing `bigtest_automator-0.5/entrypoint/main_class.py` & `bigtest_automator-0.6/entrypoint/main_class.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/internal_db_management/db_ops.py` & `bigtest_automator-0.6/internal_db_management/db_ops.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/internal_db_management/get_server_details.py` & `bigtest_automator-0.6/internal_db_management/get_server_details.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/internal_db_management/pwd_handler.py` & `bigtest_automator-0.6/internal_db_management/pwd_handler.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/oracle_utils/oracle_awr.py` & `bigtest_automator-0.6/oracle_utils/oracle_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/oracle_utils/remote_oracle_db_connector.py` & `bigtest_automator-0.6/oracle_utils/remote_oracle_db_connector.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/setup.py` & `bigtest_automator-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bigtest_automator',
-    version='0.5',
+    version='0.6',
     author='Shantharam Puranik M',
     author_email='shantharam.puranik@ellucian.com',
     description='A small tool that helps to run and collect performance related metrics such as VMSTAT and AWR. Highly specific to my ORG, might not be useful for general public. SORRY! - Noob.',
     packages=find_packages(),
     install_requires=[
         'scp',
         'paramiko',
```

### Comparing `bigtest_automator-0.5/temp/playground.py` & `bigtest_automator-0.6/temp/playground.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.5/ui_management/tk_page_layouts.py` & `bigtest_automator-0.6/ui_management/tk_page_layouts.py`

 * *Files identical despite different names*

