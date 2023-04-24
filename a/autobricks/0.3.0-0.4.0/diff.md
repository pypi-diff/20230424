# Comparing `tmp/autobricks-0.3.0.tar.gz` & `tmp/autobricks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobricks-0.3.0.tar", last modified: Mon Apr 24 18:04:07 2023, max compression
+gzip compressed data, was "autobricks-0.4.0.tar", last modified: Mon Apr 24 20:03:23 2023, max compression
```

## Comparing `autobricks-0.3.0.tar` & `autobricks-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 18:04:07.136608 autobricks-0.3.0/
--rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-04-24 18:04:07.136608 autobricks-0.3.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-04-24 18:03:36.000000 autobricks-0.3.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 18:04:07.132609 autobricks-0.3.0/autobricks/
--rw-r--r--   0 vsts      (1001) docker     (123)     9015 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/Cluster.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3558 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/Dbfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3946 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/Job.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/Library.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7638 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/SetupTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14308 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/Sql.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11141 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/Workspace.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1272 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/_decode_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 18:04:07.136608 autobricks-0.3.0/autobricks/api_service/
--rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5024 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/_auth.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1442 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/_auth_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/_base_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4367 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/api_service.py
--rw-r--r--   0 vsts      (1001) docker     (123)      313 2023-04-24 18:03:36.000000 autobricks-0.3.0/autobricks/api_service/autobricks_logging.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 18:04:07.132609 autobricks-0.3.0/autobricks.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-04-24 18:04:06.000000 autobricks-0.3.0/autobricks.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      701 2023-04-24 18:04:06.000000 autobricks-0.3.0/autobricks.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-24 18:04:06.000000 autobricks-0.3.0/autobricks.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-24 18:04:06.000000 autobricks-0.3.0/autobricks.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-04-24 18:04:06.000000 autobricks-0.3.0/autobricks.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-04-24 18:04:06.000000 autobricks-0.3.0/autobricks.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-24 18:04:07.136608 autobricks-0.3.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-04-24 18:03:36.000000 autobricks-0.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 20:03:23.744061 autobricks-0.4.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-04-24 20:03:23.740061 autobricks-0.4.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     7157 2023-04-24 20:02:48.000000 autobricks-0.4.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 20:03:23.740061 autobricks-0.4.0/autobricks/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9015 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/Cluster.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3558 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/Dbfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4661 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/Job.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/Library.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7638 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/SetupTools.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12863 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/Sql.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11141 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/Workspace.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/_common.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1272 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/_decode_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 20:03:23.740061 autobricks-0.4.0/autobricks/api_service/
+-rw-r--r--   0 vsts      (1001) docker     (123)      439 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5024 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/_auth.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1442 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/_auth_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/_base_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2876 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1146 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4367 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/api_service.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      313 2023-04-24 20:02:48.000000 autobricks-0.4.0/autobricks/api_service/autobricks_logging.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 20:03:23.740061 autobricks-0.4.0/autobricks.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      991 2023-04-24 20:03:23.000000 autobricks-0.4.0/autobricks.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      723 2023-04-24 20:03:23.000000 autobricks-0.4.0/autobricks.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-24 20:03:23.000000 autobricks-0.4.0/autobricks.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-24 20:03:23.000000 autobricks-0.4.0/autobricks.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-04-24 20:03:23.000000 autobricks-0.4.0/autobricks.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-04-24 20:03:23.000000 autobricks-0.4.0/autobricks.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-24 20:03:23.744061 autobricks-0.4.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-04-24 20:02:48.000000 autobricks-0.4.0/setup.py
```

### Comparing `autobricks-0.3.0/PKG-INFO` & `autobricks-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.3.0
+Version: 0.4.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.3.0/README.md` & `autobricks-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/Cluster.py` & `autobricks-0.4.0/autobricks/Cluster.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/Dbfs.py` & `autobricks-0.4.0/autobricks/Dbfs.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/Job.py` & `autobricks-0.4.0/autobricks/Job.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .api_service import ApiService, autobricks_logging
 from enum import Enum
-from typing import Union
+from typing import Union, List
+from ._common import get_metadata_format, load_format, tags_exist_in
+import os
 
 _logger = autobricks_logging.get_logger(__name__)
 
 endpoint = "jobs"
 _JOBS_API_VERSION = "2.1"
 _api_service = ApiService()
 
@@ -171,7 +173,26 @@
     name = job.get("name", "Unknown")
 
     job_id = job_get_id(name)
     if job_id:
         job_delete(job_id=job_id)
 
     job_create(job=job)
+
+
+def job_import_jobs(from_path: str, tags: Union[str, List[str], None] = None):
+
+    for root, _, files in os.walk(from_path):
+
+        config_files = [f for f in files if get_metadata_format(f)]
+
+        for f in config_files:
+            filename = os.path.join(root, f)
+            filename = os.path.abspath(filename)
+            with open(filename, "r", encoding="utf-8") as f:
+                metadata_format = get_metadata_format(filename)
+                data: dict = load_format(f, metadata_format)
+
+            in_tags = data.get("tags")
+
+            if tags_exist_in(tags, in_tags):
+                job_recreate(data)
```

### Comparing `autobricks-0.3.0/autobricks/Library.py` & `autobricks-0.4.0/autobricks/Library.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/SetupTools.py` & `autobricks-0.4.0/autobricks/SetupTools.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/Sql.py` & `autobricks-0.4.0/autobricks/Sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from .. import _logging
 from .api_service import ApiService
 import math
 import os
 import yaml
 import json
 from enum import Enum
-from io import TextIOWrapper
+
 from typing import Union, List
 from .Workspace import (
     workspace_dir_exists,
     workspace_mkdirs,
     workspace_get_folder_id,
     workspace_find_paths,
 )
+from ._common import MetadataFormat, get_metadata_format, load_format, tags_exist_in
 
 
 _logger = _logging.get_logger(__name__)
 endpoint = "sql"
 _PREVIEW = True
 _API_VERSION = "2.0"
 _FOLDERS = "folders/"
@@ -43,19 +44,14 @@
 
 
 class AclCredential(Enum):
     user_acl = "user_name"
     group_acl = "group_name"
 
 
-class MetadataFormat(Enum):
-    yaml = "yaml"
-    json = "json"
-
-
 def _get_credential_type(name: str):
     """
     name: str   name o the credential
 
     If it contains an @ sign then determine it's an email address
     and therefore a users. TODO: change to regex pattern match
     """
@@ -122,31 +118,14 @@
         page += 1
 
     _logger.debug(f"exported {len(results)}")
 
     return results
 
 
-def _tags_exist_in(tags: Union[str, List[str], None], in_tags: List[str]):
-    """
-    tags: Union[str, List[str], None]   Tags that want to check are in the superset list. If there are no tags returns true
-    in_tags: List[str]                  The target superset of tags you want to check if the tags are in
-
-    This is a utility function to check is a set of tags are in a superset of tags.
-    If the tags are none then it assumes that no tag filtered is being applied and
-    therefore returns true.
-    """
-    if isinstance(tags, str):
-        return tags in in_tags
-    elif isinstance(tags, list):
-        return set(tags).issubset(set(in_tags))
-    else:
-        return True
-
-
 def set_acl(
     acl_name: Union[str, List[str]],
     permission: PermissionLevel,
     object_id: str,
     object_type: ObjectType = ObjectType.query,
 ):
     """
@@ -200,30 +179,30 @@
         path = workspace_paths.get(id, "")
         return path
 
     sql_queries = queries(page_size, order=order, q=q)
     folder_ids = [
         s["options"]["parent"].replace(_FOLDERS, "")
         for s in sql_queries
-        if _tags_exist_in(tags, s["tags"])
+        if tags_exist_in(tags, s["tags"])
     ]
     workspace_paths = workspace_find_paths(folder_ids, root_folders)
     name_sql = {
         s["name"]: {
             "id": s["id"],
             "name": s["name"],
             "query": s["query"],
             "options": {"parameters": s["options"].get("parameters")},
             "workspace_path": _lookup_workspace_path(
                 s["options"]["parent"], workspace_paths
             ),
             "tags": s["tags"],
         }
         for s in sql_queries
-        if _tags_exist_in(tags, s["tags"])
+        if tags_exist_in(tags, s["tags"])
     }
 
     _logger.debug(f"matched {len(name_sql.keys())} queries")
     return name_sql
 
 
 def queries_export_sql_files(
@@ -343,42 +322,14 @@
         function,
         data=metadata,
         preview=_PREVIEW,
         api_version=_API_VERSION,
     )
 
 
-def _get_metadata_format(filename: str):
-    """
-    filename:str name of the file with the extension
-
-    determines the supported format of the metadata files.
-    """
-    _, ext = os.path.splitext(filename)
-    try:
-        ext = MetadataFormat(ext[1:])
-        return ext
-    except Exception:
-        return None
-
-
-def _load_format(f: TextIOWrapper, format: MetadataFormat):
-    """
-    f: TextIOWrapper        file stream from an open command
-    format: MetadataFormat  metadata format
-
-    reads the filestream using the correct library to parse the file format type
-    """
-    if format == MetadataFormat.yaml:
-        data = yaml.safe_load(f)
-    elif format == MetadataFormat.json:
-        data = json.load(f)
-    return data
-
-
 def _get_folder_id(workspace_path: str):
     if not workspace_dir_exists(workspace_path):
         workspace_mkdirs(workspace_path)
     folder_object_id = workspace_get_folder_id(workspace_path)
     return folder_object_id
 
 
@@ -398,27 +349,27 @@
     If share_with is supplied then it will set ACLS on those groups.
     """
 
     sql_queries = []
     exceptions = []
     for root, _, files in os.walk(from_path):
 
-        config_files = [f for f in files if _get_metadata_format(f)]
+        config_files = [f for f in files if get_metadata_format(f)]
 
         for f in config_files:
 
             filename = os.path.join(root, f)
             filename = os.path.abspath(filename)
             with open(filename, "r", encoding="utf-8") as f:
-                metadata_format = _get_metadata_format(filename)
-                data: dict = _load_format(f, metadata_format)
+                metadata_format = get_metadata_format(filename)
+                data: dict = load_format(f, metadata_format)
 
             in_tags = data["tags"]
 
-            if _tags_exist_in(tags, in_tags):
+            if tags_exist_in(tags, in_tags):
 
                 filename = data["query"]
                 sql_file_path = os.path.abspath(root)
                 sql_file_path = os.path.join(sql_file_path, filename)
                 with open(sql_file_path, "r", encoding="utf-8") as f:
                     data["query"] = f.read()
```

### Comparing `autobricks-0.3.0/autobricks/Workspace.py` & `autobricks-0.4.0/autobricks/Workspace.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/_decode_utils.py` & `autobricks-0.4.0/autobricks/_decode_utils.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/api_service/_auth.py` & `autobricks-0.4.0/autobricks/api_service/_auth.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/api_service/_auth_factory.py` & `autobricks-0.4.0/autobricks/api_service/_auth_factory.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/api_service/_base_api.py` & `autobricks-0.4.0/autobricks/api_service/_base_api.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/api_service/_configuration.py` & `autobricks-0.4.0/autobricks/api_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/api_service/_exceptions.py` & `autobricks-0.4.0/autobricks/api_service/_exceptions.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks/api_service/api_service.py` & `autobricks-0.4.0/autobricks/api_service/api_service.py`

 * *Files identical despite different names*

### Comparing `autobricks-0.3.0/autobricks.egg-info/PKG-INFO` & `autobricks-0.4.0/autobricks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobricks
-Version: 0.3.0
+Version: 0.4.0
 Summary: Databricks Deployment Utils
 Home-page: https://autobricks.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/autobricks
 Project-URL: Documentation, https://autobricks.readthedocs.io/en/latest/
```

### Comparing `autobricks-0.3.0/autobricks.egg-info/SOURCES.txt` & `autobricks-0.4.0/autobricks.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 autobricks/Cluster.py
 autobricks/Dbfs.py
 autobricks/Job.py
 autobricks/Library.py
 autobricks/SetupTools.py
 autobricks/Sql.py
 autobricks/Workspace.py
+autobricks/_common.py
 autobricks/_decode_utils.py
 autobricks.egg-info/PKG-INFO
 autobricks.egg-info/SOURCES.txt
 autobricks.egg-info/dependency_links.txt
 autobricks.egg-info/not-zip-safe
 autobricks.egg-info/requires.txt
 autobricks.egg-info/top_level.txt
```

### Comparing `autobricks-0.3.0/setup.py` & `autobricks-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "PYPI.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="autobricks",
-    version="0.3.0",
+    version="0.4.0",
     description="Databricks Deployment Utils",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://autobricks.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/autobricks',
         'Documentation': 'https://autobricks.readthedocs.io/en/latest/'
```

