# Comparing `tmp/iseqresources-0.0.8.tar.gz` & `tmp/iseqresources-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iseqresources-0.0.8.tar", last modified: Wed Aug  3 12:24:54 2022, max compression
+gzip compressed data, was "iseqresources-0.0.9.tar", last modified: Wed Aug  3 12:59:12 2022, max compression
```

## Comparing `iseqresources-0.0.8.tar` & `iseqresources-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:24:54.877804 iseqresources-0.0.8/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1327 2022-07-29 13:46:59.000000 iseqresources-0.0.8/.gitignore
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1067 2022-07-29 13:46:59.000000 iseqresources-0.0.8/LICENSE
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3690 2022-08-03 12:24:54.877804 iseqresources-0.0.8/PKG-INFO
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3168 2022-07-29 13:46:59.000000 iseqresources-0.0.8/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:24:54.873804 iseqresources-0.0.8/json/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      103 2022-08-01 15:02:59.000000 iseqresources-0.0.8/json/info.json
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2854 2022-07-29 13:47:25.000000 iseqresources-0.0.8/json/tools_and_databases.json
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)      931 2022-08-03 12:24:54.877804 iseqresources-0.0.8/setup.cfg
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)       69 2022-07-29 13:46:59.000000 iseqresources-0.0.8/setup.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:24:54.873804 iseqresources-0.0.8/src/
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:24:54.873804 iseqresources-0.0.8/src/iseqresources/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)        0 2022-07-29 13:46:59.000000 iseqresources-0.0.8/src/iseqresources/__init__.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1691 2022-08-03 12:23:46.000000 iseqresources-0.0.8/src/iseqresources/add_new_tool_to_json.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2265 2022-08-01 12:09:35.000000 iseqresources-0.0.8/src/iseqresources/add_task_to_jira.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     8815 2022-08-03 12:23:35.000000 iseqresources-0.0.8/src/iseqresources/add_tool.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3059 2022-07-29 13:46:59.000000 iseqresources-0.0.8/src/iseqresources/check_version.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2990 2022-08-03 12:23:47.000000 iseqresources-0.0.8/src/iseqresources/check_versions_add_task.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1091 2022-07-29 13:48:39.000000 iseqresources-0.0.8/src/iseqresources/update_record.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2420 2022-08-03 12:23:48.000000 iseqresources-0.0.8/src/iseqresources/update_tool_record.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:24:54.877804 iseqresources-0.0.8/src/iseqresources.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3690 2022-08-03 12:24:54.000000 iseqresources-0.0.8/src/iseqresources.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      676 2022-08-03 12:24:54.000000 iseqresources-0.0.8/src/iseqresources.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2022-08-03 12:24:54.000000 iseqresources-0.0.8/src/iseqresources.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      183 2022-08-03 12:24:54.000000 iseqresources-0.0.8/src/iseqresources.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       50 2022-08-03 12:24:54.000000 iseqresources-0.0.8/src/iseqresources.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       20 2022-08-03 12:24:54.000000 iseqresources-0.0.8/src/iseqresources.egg-info/top_level.txt
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:24:54.877804 iseqresources-0.0.8/src/utils/
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)        0 2022-07-29 13:46:59.000000 iseqresources-0.0.8/src/utils/__init__.py
--rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2596 2022-08-02 08:36:05.000000 iseqresources-0.0.8/src/utils/utils.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:59:12.524620 iseqresources-0.0.9/
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1327 2022-07-29 13:46:59.000000 iseqresources-0.0.9/.gitignore
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1067 2022-07-29 13:46:59.000000 iseqresources-0.0.9/LICENSE
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3690 2022-08-03 12:59:12.524620 iseqresources-0.0.9/PKG-INFO
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3168 2022-07-29 13:46:59.000000 iseqresources-0.0.9/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:59:12.524620 iseqresources-0.0.9/json/
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)      103 2022-08-01 15:02:59.000000 iseqresources-0.0.9/json/info.json
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2159 2022-08-03 12:56:32.000000 iseqresources-0.0.9/json/tools_and_databases.json
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)      931 2022-08-03 12:59:12.524620 iseqresources-0.0.9/setup.cfg
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)       69 2022-07-29 13:46:59.000000 iseqresources-0.0.9/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:59:12.524620 iseqresources-0.0.9/src/
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:59:12.524620 iseqresources-0.0.9/src/iseqresources/
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)        0 2022-07-29 13:46:59.000000 iseqresources-0.0.9/src/iseqresources/__init__.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1691 2022-08-03 12:58:08.000000 iseqresources-0.0.9/src/iseqresources/add_new_tool_to_json.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2265 2022-08-01 12:09:35.000000 iseqresources-0.0.9/src/iseqresources/add_task_to_jira.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     8815 2022-08-03 12:23:35.000000 iseqresources-0.0.9/src/iseqresources/add_tool.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3059 2022-07-29 13:46:59.000000 iseqresources-0.0.9/src/iseqresources/check_version.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     3002 2022-08-03 12:58:04.000000 iseqresources-0.0.9/src/iseqresources/check_versions_add_task.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     1091 2022-07-29 13:48:39.000000 iseqresources-0.0.9/src/iseqresources/update_record.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2436 2022-08-03 12:58:01.000000 iseqresources-0.0.9/src/iseqresources/update_tool_record.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:59:12.524620 iseqresources-0.0.9/src/iseqresources.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3690 2022-08-03 12:59:12.000000 iseqresources-0.0.9/src/iseqresources.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      676 2022-08-03 12:59:12.000000 iseqresources-0.0.9/src/iseqresources.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2022-08-03 12:59:12.000000 iseqresources-0.0.9/src/iseqresources.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      183 2022-08-03 12:59:12.000000 iseqresources-0.0.9/src/iseqresources.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       50 2022-08-03 12:59:12.000000 iseqresources-0.0.9/src/iseqresources.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       20 2022-08-03 12:59:12.000000 iseqresources-0.0.9/src/iseqresources.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2022-08-03 12:59:12.524620 iseqresources-0.0.9/src/utils/
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)        0 2022-07-29 13:46:59.000000 iseqresources-0.0.9/src/utils/__init__.py
+-rw-r--r--   0 mateusz   (1000) mateusz   (1000)     2596 2022-08-02 08:36:05.000000 iseqresources-0.0.9/src/utils/utils.py
```

### Comparing `iseqresources-0.0.8/.gitignore` & `iseqresources-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/LICENSE` & `iseqresources-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/PKG-INFO` & `iseqresources-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqresources
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for adding new tools to json file, checking their versions and creating tasks in JIRA
 Home-page: https://gitlab.com/intelliseq/iseqresources
 Author: Mateusz Marynowski
 Author-email: mateusz.marynowski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iseqresources-0.0.8/README.md` & `iseqresources-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/setup.cfg` & `iseqresources-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iseqresources
-version = 0.0.8
+version = 0.0.9
 author = Mateusz Marynowski
 author_email = mateusz.marynowski@intelliseq.pl
 description = Package for adding new tools to json file, checking their versions and creating tasks in JIRA
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/intelliseq/iseqresources
 classifiers =
```

### Comparing `iseqresources-0.0.8/src/iseqresources/add_new_tool_to_json.py` & `iseqresources-0.0.9/src/iseqresources/add_new_tool_to_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 from iseqresources.add_tool import AddTool
 from utils import utils
 import os
 
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 GITLAB_TOKEN=os.environ.get("GITLAB_TOKEN")
 
 
 def info_text():
     return '''Press 0 to exit
```

### Comparing `iseqresources-0.0.8/src/iseqresources/add_task_to_jira.py` & `iseqresources-0.0.9/src/iseqresources/add_task_to_jira.py`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/src/iseqresources/add_tool.py` & `iseqresources-0.0.9/src/iseqresources/add_tool.py`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/src/iseqresources/check_version.py` & `iseqresources-0.0.9/src/iseqresources/check_version.py`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/src/iseqresources/check_versions_add_task.py` & `iseqresources-0.0.9/src/iseqresources/check_versions_add_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tqdm import tqdm
 from utils import utils
 from iseqresources.check_version import CheckVersion
 from iseqresources.add_task_to_jira import AddTaskToJira
 import os
 
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 GITHUB_TOKEN=os.environ.get("GITHUB_TOKEN")
 GITLAB_TOKEN=os.environ.get("GITLAB_TOKEN")
 JIRA_EMAIL=os.environ.get("JIRA_EMAIL")
 JIRA_TOKEN=os.environ.get("JIRA_TOKEN")
 
@@ -34,16 +34,17 @@
     for tool_or_database in tqdm(resources_dict):
         obj = CheckVersion(tool_or_database, github_token)
         create_task_in_jira = test_name.get(tool_or_database["test"], lambda : "ERROR: Invalid test")()
         # create task in jira if there is new version of tool/database
         if create_task_in_jira:
             jira = AddTaskToJira(tool_or_database, jira_email, jira_token, jira_project_info=jira_project_info)
             jira.add_task_to_jira()
-    if not gitlab_token and json_file.startswith("https://"):
-        gitlab_token = utils.get_gitlab_token()
+    if json_file.startswith("https://"):
+        if not gitlab_token:
+            gitlab_token = utils.get_gitlab_token()
         utils.save_json_to_gitlab(resources_dict, gitlab_token)
     else:
         utils.save_json(json_file, resources_dict)
     return create_task_in_jira
 
 
 def main():
```

### Comparing `iseqresources-0.0.8/src/iseqresources/update_record.py` & `iseqresources-0.0.9/src/iseqresources/update_record.py`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/src/iseqresources/update_tool_record.py` & `iseqresources-0.0.9/src/iseqresources/update_tool_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 from utils import utils
 from iseqresources.update_record import UpdateRecord
 import json
 import os
 
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 GITLAB_TOKEN=os.environ.get("GITLAB_TOKEN")
 
 
 def info_text():
     utils.clear_screen()
@@ -42,16 +42,17 @@
                 tool_found = True
                 break
         if not tool_found:
             print("Tool/database not found")
             input("Press enter to continue")
         choice = info_text()
     if (input_dict != resources_dict):
-        if not gitlab_token and json_file.startswith("https://"):
-            gitlab_token = utils.get_gitlab_token()
+        if json_file.startswith("https://"):
+            if not gitlab_token:
+                gitlab_token = utils.get_gitlab_token()
             utils.save_json_to_gitlab(resources_dict, gitlab_token)
         else:
             utils.save_json(json_file, resources_dict)
 
 
 def main():
     parser = argparse.ArgumentParser(description='Add new tool to json file')
```

### Comparing `iseqresources-0.0.8/src/iseqresources.egg-info/PKG-INFO` & `iseqresources-0.0.9/src/iseqresources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqresources
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for adding new tools to json file, checking their versions and creating tasks in JIRA
 Home-page: https://gitlab.com/intelliseq/iseqresources
 Author: Mateusz Marynowski
 Author-email: mateusz.marynowski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iseqresources-0.0.8/src/iseqresources.egg-info/SOURCES.txt` & `iseqresources-0.0.9/src/iseqresources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iseqresources-0.0.8/src/utils/utils.py` & `iseqresources-0.0.9/src/utils/utils.py`

 * *Files identical despite different names*

