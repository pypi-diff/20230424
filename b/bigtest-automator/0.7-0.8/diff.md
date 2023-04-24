# Comparing `tmp/bigtest_automator-0.7.tar.gz` & `tmp/bigtest_automator-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtest_automator-0.7.tar", last modified: Mon Apr 24 10:36:36 2023, max compression
+gzip compressed data, was "bigtest_automator-0.8.tar", last modified: Mon Apr 24 10:56:39 2023, max compression
```

## Comparing `bigtest_automator-0.7.tar` & `bigtest_automator-0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.199031 bigtest_automator-0.7/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-24 10:36:36.198882 bigtest_automator-0.7/PKG-INFO
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.194057 bigtest_automator-0.7/bigtest_automator.egg-info/
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-24 10:36:36.000000 bigtest_automator-0.7/bigtest_automator.egg-info/PKG-INFO
--rw-r--r--   0 shantharamp   (502) staff       (20)      871 2023-04-24 10:36:36.000000 bigtest_automator-0.7/bigtest_automator.egg-info/SOURCES.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-24 10:36:36.000000 bigtest_automator-0.7/bigtest_automator.egg-info/dependency_links.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       61 2023-04-24 10:36:36.000000 bigtest_automator-0.7/bigtest_automator.egg-info/entry_points.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-24 10:36:36.000000 bigtest_automator-0.7/bigtest_automator.egg-info/requires.txt
--rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-24 10:36:36.000000 bigtest_automator-0.7/bigtest_automator.egg-info/top_level.txt
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.194962 bigtest_automator-0.7/core_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.7/core_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6620 2023-04-22 06:17:51.000000 bigtest_automator-0.7/core_utils/generate_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.7/core_utils/run_scp.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.7/core_utils/run_vmstat.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.7/core_utils/take_awr_snapshot.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.195745 bigtest_automator-0.7/entrypoint/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:17:21.000000 bigtest_automator-0.7/entrypoint/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1784 2023-04-24 10:34:12.000000 bigtest_automator-0.7/entrypoint/initialize.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      647 2023-04-23 16:24:30.000000 bigtest_automator-0.7/entrypoint/main_class.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.196803 bigtest_automator-0.7/internal_db_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.7/internal_db_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1234 2023-04-24 10:34:58.000000 bigtest_automator-0.7/internal_db_management/db_ops.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.7/internal_db_management/get_server_details.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1132 2023-04-24 10:35:59.000000 bigtest_automator-0.7/internal_db_management/pwd_handler.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.197473 bigtest_automator-0.7/oracle_utils/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.7/oracle_utils/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.7/oracle_utils/oracle_awr.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.7/oracle_utils/remote_oracle_db_connector.py
--rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-24 10:36:36.199089 bigtest_automator-0.7/setup.cfg
--rw-r--r--   0 shantharamp   (502) staff       (20)      670 2023-04-24 10:36:16.000000 bigtest_automator-0.7/setup.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.197951 bigtest_automator-0.7/temp/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.7/temp/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.7/temp/initiator.py
--rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.7/temp/playground.py
-drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:36:36.198598 bigtest_automator-0.7/ui_management/
--rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.7/ui_management/__init__.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.7/ui_management/dynamic_logger.py
--rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.7/ui_management/grid.py
--rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.7/ui_management/tk_page_layouts.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.841570 bigtest_automator-0.8/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-24 10:56:39.841429 bigtest_automator-0.8/PKG-INFO
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.837599 bigtest_automator-0.8/bigtest_automator.egg-info/
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/PKG-INFO
+-rw-r--r--   0 shantharamp   (502) staff       (20)      871 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/SOURCES.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)        1 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/dependency_links.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       61 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/entry_points.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       22 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/requires.txt
+-rw-r--r--   0 shantharamp   (502) staff       (20)       77 2023-04-24 10:56:39.000000 bigtest_automator-0.8/bigtest_automator.egg-info/top_level.txt
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.838474 bigtest_automator-0.8/core_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:36:07.000000 bigtest_automator-0.8/core_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     7023 2023-04-24 10:55:23.000000 bigtest_automator-0.8/core_utils/generate_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     6198 2023-04-22 06:19:59.000000 bigtest_automator-0.8/core_utils/run_scp.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     5027 2023-04-22 06:21:16.000000 bigtest_automator-0.8/core_utils/run_vmstat.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     7817 2023-04-22 06:22:05.000000 bigtest_automator-0.8/core_utils/take_awr_snapshot.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.838952 bigtest_automator-0.8/entrypoint/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 16:17:21.000000 bigtest_automator-0.8/entrypoint/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1784 2023-04-24 10:34:12.000000 bigtest_automator-0.8/entrypoint/initialize.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      713 2023-04-24 10:51:17.000000 bigtest_automator-0.8/entrypoint/main_class.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.839606 bigtest_automator-0.8/internal_db_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:16.000000 bigtest_automator-0.8/internal_db_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1234 2023-04-24 10:34:58.000000 bigtest_automator-0.8/internal_db_management/db_ops.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2588 2023-04-22 06:25:51.000000 bigtest_automator-0.8/internal_db_management/get_server_details.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1132 2023-04-24 10:35:59.000000 bigtest_automator-0.8/internal_db_management/pwd_handler.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.840018 bigtest_automator-0.8/oracle_utils/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:20.000000 bigtest_automator-0.8/oracle_utils/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2680 2023-04-22 06:26:28.000000 bigtest_automator-0.8/oracle_utils/oracle_awr.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     2573 2023-04-22 06:23:15.000000 bigtest_automator-0.8/oracle_utils/remote_oracle_db_connector.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)       38 2023-04-24 10:56:39.841628 bigtest_automator-0.8/setup.cfg
+-rw-r--r--   0 shantharamp   (502) staff       (20)      670 2023-04-24 10:56:29.000000 bigtest_automator-0.8/setup.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.840448 bigtest_automator-0.8/temp/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:23.000000 bigtest_automator-0.8/temp/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      456 2022-12-06 06:14:16.000000 bigtest_automator-0.8/temp/initiator.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)     1929 2023-04-21 13:38:54.000000 bigtest_automator-0.8/temp/playground.py
+drwxr-xr-x   0 shantharamp   (502) staff       (20)        0 2023-04-24 10:56:39.841123 bigtest_automator-0.8/ui_management/
+-rw-r--r--   0 shantharamp   (502) staff       (20)        0 2023-04-23 15:37:27.000000 bigtest_automator-0.8/ui_management/__init__.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      225 2023-04-05 09:57:55.000000 bigtest_automator-0.8/ui_management/dynamic_logger.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)      320 2023-01-04 15:10:35.000000 bigtest_automator-0.8/ui_management/grid.py
+-rw-r--r--   0 shantharamp   (502) staff       (20)    23889 2023-04-23 06:00:54.000000 bigtest_automator-0.8/ui_management/tk_page_layouts.py
```

### Comparing `bigtest_automator-0.7/bigtest_automator.egg-info/SOURCES.txt` & `bigtest_automator-0.8/bigtest_automator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/core_utils/generate_awr.py` & `bigtest_automator-0.8/core_utils/generate_awr.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,18 @@
                 messagebox.showerror("Error", message="Please enter valid values")
             else:
                 full_server_detail = get_server_details.GetServerDetails.get_server_details(snap_list,"GEN_AWR")
                 if(full_server_detail[0][0] != full_server_detail[1][0]):
                     messagebox.showerror("Error",message="The begin and end snap ID are not from the same database!")
                 else:
 
+                    def write_transaction_log():
+                        query = "DELETE FROM AWR WHERE SNAP_ID IN ('{}','{}')".format(full_server_detail[0][7],full_server_detail[1][7])
+                        db_ops.query_executor(query)
+
                     def exit_window():
                         answer = mb.askyesno(title='Are you sure?', message="Are you sure that you want to exit? Possible transaction loss if you proceed when a transaction is in progress.")
                         if answer:
                             root.quit()
 
                     for item in root.winfo_children():
                         item.destroy()
@@ -115,12 +119,14 @@
                         dynamic_logger.Logger(root,logtext,"Could not generate the AWR report")
                         for log in logger:
                             dynamic_logger.Logger(root,logtext,log)
                     
                     else:
                         for log in logger:
                             dynamic_logger.Logger(root,logtext,log)
-                        dynamic_logger.Logger(root,logtext,"Successfully generated the AWR:"+outfile)
+                        dynamic_logger.Logger(root,logtext,"Successfully generated the AWR at:"+outfile)
+                        dynamic_logger.Logger(root,logtext,"These snaps have been erased from the local table")
+                        write_transaction_log()
 
         button_grid_row = g.get_next_row()
         Button(root,text="Submit",command=submit_info).grid(row=button_grid_row,column=0)
         Button(root,text="Exit",command=root.quit).grid(row=button_grid_row,column=1)
```

### Comparing `bigtest_automator-0.7/core_utils/run_scp.py` & `bigtest_automator-0.8/core_utils/run_scp.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/core_utils/run_vmstat.py` & `bigtest_automator-0.8/core_utils/run_vmstat.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/core_utils/take_awr_snapshot.py` & `bigtest_automator-0.8/core_utils/take_awr_snapshot.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/entrypoint/initialize.py` & `bigtest_automator-0.8/entrypoint/initialize.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/entrypoint/main_class.py` & `bigtest_automator-0.8/entrypoint/main_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from tkinter import *
-from ui_management import tk_page_layouts, grid
+import ui_management.tk_page_layouts as tk
+import ui_management.grid as grid
+# from ui_management import tk_page_layouts, grid
 import entrypoint.initialize as initialize
 
 
 g = grid.Grid() 
 
 def main():
     initialize.initialize_db()
@@ -17,13 +19,13 @@
 
     # root.geometry("2000x500")
     root.resizable(0, 0)
     root.title("VMSTAT Automator")
 
     Label(frm, text="Welcome to VMSTAT automator!", font=('calibre','20','bold')).grid(row=g.get_next_row(),column=0,columnspan=10)
 
-    tk_page_layouts.RecordActions(frm)
+    tk.RecordActions(frm)
 
     root.mainloop()
 
 if __name__ == "__main__":
     main()
```

### Comparing `bigtest_automator-0.7/internal_db_management/db_ops.py` & `bigtest_automator-0.8/internal_db_management/db_ops.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/internal_db_management/get_server_details.py` & `bigtest_automator-0.8/internal_db_management/get_server_details.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/internal_db_management/pwd_handler.py` & `bigtest_automator-0.8/internal_db_management/pwd_handler.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/oracle_utils/oracle_awr.py` & `bigtest_automator-0.8/oracle_utils/oracle_awr.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/oracle_utils/remote_oracle_db_connector.py` & `bigtest_automator-0.8/oracle_utils/remote_oracle_db_connector.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/setup.py` & `bigtest_automator-0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bigtest_automator',
-    version='0.7',
+    version='0.8',
     author='Shantharam Puranik M',
     author_email='shantharam.puranik@ellucian.com',
     description='A small tool that helps to run and collect performance related metrics such as VMSTAT and AWR. Highly specific to my ORG, might not be useful for general public. SORRY! - Noob.',
     packages=find_packages(),
     install_requires=[
         'scp',
         'paramiko',
```

### Comparing `bigtest_automator-0.7/temp/playground.py` & `bigtest_automator-0.8/temp/playground.py`

 * *Files identical despite different names*

### Comparing `bigtest_automator-0.7/ui_management/tk_page_layouts.py` & `bigtest_automator-0.8/ui_management/tk_page_layouts.py`

 * *Files identical despite different names*

