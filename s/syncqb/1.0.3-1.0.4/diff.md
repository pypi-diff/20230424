# Comparing `tmp/syncqb-1.0.3.tar.gz` & `tmp/syncqb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.3.tar", last modified: Thu Apr 13 17:32:09 2023, max compression
+gzip compressed data, was "syncqb-1.0.4.tar", last modified: Mon Apr 24 16:01:08 2023, max compression
```

## Comparing `syncqb-1.0.3.tar` & `syncqb-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.397101 syncqb-1.0.3/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.3/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-13 17:32:09.387101 syncqb-1.0.3/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.3/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-04-13 17:29:22.000000 syncqb-1.0.3/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-13 17:32:09.397101 syncqb-1.0.3/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.3/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.377101 syncqb-1.0.3/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.377101 syncqb-1.0.3/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.3/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.3/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    15814 2023-04-13 17:16:51.000000 syncqb-1.0.3/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11313 2023-04-13 17:00:56.000000 syncqb-1.0.3/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-04-13 17:15:37.000000 syncqb-1.0.3/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.3/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.3/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.3/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2639 2023-04-13 17:16:03.000000 syncqb-1.0.3/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.3/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-04-13 17:16:23.000000 syncqb-1.0.3/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.3/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.387101 syncqb-1.0.3/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-13 17:32:09.000000 syncqb-1.0.3/src/syncqb.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-13 17:32:09.387101 syncqb-1.0.3/tests/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1296 2023-04-13 17:21:46.000000 syncqb-1.0.3/tests/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.4/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 16:01:08.288570 syncqb-1.0.4/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.4/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-04-24 16:00:32.000000 syncqb-1.0.4/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-24 16:01:08.288570 syncqb-1.0.4/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.4/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.4/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.4/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16238 2023-04-21 17:31:28.000000 syncqb-1.0.4/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11395 2023-04-21 14:13:40.000000 syncqb-1.0.4/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-04-13 17:15:37.000000 syncqb-1.0.4/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.4/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.4/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.4/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2799 2023-04-21 17:29:58.000000 syncqb-1.0.4/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.4/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-04-13 17:16:23.000000 syncqb-1.0.4/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.4/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/tests/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1428 2023-04-13 17:50:02.000000 syncqb-1.0.4/tests/test.py
```

### Comparing `syncqb-1.0.3/LICENSE` & `syncqb-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/PKG-INFO` & `syncqb-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.3/README.md` & `syncqb-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/pyproject.toml` & `syncqb-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",'requests>=2.25.1','lxml>=4.6.3','chardet>=3.0.4']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syncqb"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Jacob Gearhardt", email="jacob@synctivate.com" },
 ]
 description = "A Python SDK for quickbase"
 readme = "README.md"
 license = { file="LICENSE" }
 dependencies = [
```

### Comparing `syncqb-1.0.3/src/syncqb/json_quickbase.py` & `syncqb-1.0.4/src/syncqb/json_quickbase.py`

 * *Files 9% similar despite different names*

```diff
@@ -232,60 +232,62 @@
 
         if safemode:
             pk = self.get_primary_key(database)
             if pk in fields.keys():
                 raise ValueError(f'Primary key fid: {pk} cannot be set in safemode')
 
         response = self._insert_update_record(fields, uploads, return_fields, database=database)
+        response_metadata = response.get('metadata', {})
 
-        if len(response["metadata"]["createdRecordIds"]) > 1:
-            rids = response["metadata"]["createdRecordIds"]
+        if len(response_metadata.get('createdRecordIds')) > 1:
+            rids = response_metadata.get('createdRecordIds')
             raise QuickbaseError(f"More than one record created, record ids: {rids}")
 
-        if len(response['metadata']['updatedRecordIds']) > 0:
-            rids = response["metadata"]["updatedRecordIds"]
+        if len(response_metadata.get('updatedRecordIds')) > 0:
+            rids = response_metadata.get('updatedRecordIds')
             raise QuickbaseError(f'Record updated instead of created, record ids: {rids}')
         
         if return_fields:
             return self.denest(response['data'])[0]
         else:
-            return response["metadata"]["createdRecordIds"][0]
+            return response_metadata.get('createdRecordIds')[0]
 
     def edit_record(self, rid=None, key=None, fields=None, database=None, uploads=None, return_fields=None):
         if not fields:
             fields = {}
 
         if not rid and not key:
             raise ValueError('Must provide either a rid or a key')
         if rid:
             fields.update({'3': rid})
         elif key:
             fields.update({self.get_primary_key(database): key or rid})
         
 
         response = self._insert_update_record(fields, uploads, return_fields, database=database)
+        response_metadata = response.get('metadata', {})
 
         try:
-            if len(response["metadata"]["createdRecordIds"]) > 0:
-                rids = response["metadata"]["createdRecordIds"]
+            if len(response_metadata.get('createdRecordIds')) > 0:
+                rids = response_metadata.get('createdRecordIds')
                 raise QuickbaseError(f"Created instead of updated a record, record ids: {rids}", response)
             
-            if len(response['metadata']['updatedRecordIds']) > 1:
-                rids = response["metadata"]["updatedRecordIds"]
+            if len(response_metadata.get('updatedRecordIds')) > 1:
+                rids = response_metadata.get('updatedRecordIds')
                 raise QuickbaseError(f'More than one record updated, record ids: {rids}', response)
-        except:
-            raise QuickbaseError('Error Attempting to update records', response)
+        except Exception as e:
+            raise QuickbaseError('Error Attempting to update records', response) from e
         
         if return_fields:
             return self.denest(response['data'])[0]
         else:
             try:
-                return response["metadata"]["updatedRecordIds"][0]
+                return response_metadata.get('updatedRecordIds')[0]
             except IndexError:
-                return response["metadata"]["unchangedRecordIds"][0]
+                return response_metadata.get('unchangedRecordIds')[0]
 
     def _insert_update_record(self, body, uploads, return_fields, database=None):
  
         if uploads:
             for upload in uploads:
                 body.update({upload['field']: {
                     'fileName': upload['filename'],
@@ -345,14 +347,18 @@
         url = 'https://api.quickbase.com/v1/records'
         body = {
             'to': database or self.database,
             'data': records,
             'fieldsToReturn': return_fields
         }
         response = self._request(url, 'post', self.headers, data=body, json=True)
+        response_metadata = response.get('metadata', {})
+        if response_metadata.get('lineErrors'):
+            key = list(response_metadata['lineErrors'].keys())[0]
+            raise QuickbaseError(f'Your record has invalid data: {response_metadata["lineErrors"][key]}')
 
         return response
 
     def purge_records(self, database=None, rids=None, query=None):
         if not rids and not query:
             raise ValueError('Must provide either a list of rids or a query')
```

### Comparing `syncqb-1.0.3/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.4/src/syncqb/json_quickbase.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -122,34 +122,34 @@
         Delete a record from a Quickbase table.
         :param rid: (str or int) Quickbase record ID
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :return: (dict) The response
         """
         ...
     def add_multiple_records(self, data: list[dict[str, Any]], database: str | None = None, return_fields: list[str | int] | None = None, 
-                             round_ints: bool = False, safemode: bool = False) -> dict[str, Any]:
+                             round_ints: bool = False, safemode: bool = False) -> list[dict[str, Any]]:
         """
         Add multiple records to a Quickbase table.
         :param data: (list of dict) List of dictionaries of field IDs and values
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :param return_fields: (None or list of str or int) List of fields to return (default None)
         :param round_ints: (bool) Whether to round integers (default False)
         :param safemode: (bool) Whether to raise an error if you might edit a record (default False)
-        :return: (dict) The response
+        :return: (list) Returned data about the records added or edited
         """
         ...
     def edit_multiple_records(self, data: list[dict[str, Any]], database: str | None = None, 
-                              return_fields: list[str | int] | None = None, round_ints: bool = False) -> dict[str, Any]:
+                              return_fields: list[str | int] | None = None, round_ints: bool = False) -> list[dict[str, Any]]:
         """
         Edit multiple records in a Quickbase table.
         :param data: (list of dict) List of dictionaries of field IDs and values
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :param return_fields: (None or list of str or int) List of fields to return (default None)
         :param round_ints: (bool) Whether to round integers (default False)
-        :return: (dict) The response
+        :return: (list) Returned data about the records added or edited
         """
         ...
     def purge_records(self, database: str | None = None, rids: list[str | int] | None = None, query: str | None = None) -> dict[str, int]:
         """
         Purge records from a Quickbase table.
         :param database: (str or None) Quickbase Table ID (default None, uses self.database)
         :param rids: (None or list of str or int) List of record IDs to purge (default None)
```

### Comparing `syncqb-1.0.3/src/syncqb/qb_client.py` & `syncqb-1.0.4/src/syncqb/qb_client.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb/qb_client.pyi` & `syncqb-1.0.4/src/syncqb/qb_client.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb/qb_errors.py` & `syncqb-1.0.4/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb/qb_errors.pyi` & `syncqb-1.0.4/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb/quickbase.py` & `syncqb-1.0.4/src/syncqb/quickbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,18 @@
             raise QBResponseError('Response Error: Invalid request', response)
         elif response.status_code == 429:
             raise QBResponseError('Response Error: Too many requests', response)
         elif response.status_code == 500:
             raise QBResponseError('Response Error: Internal Quickbase Server Error', response)
         
         if json:
-            return response.json()
+            try:
+                return response.json()
+            except Exception as e:
+                raise QBResponseError('Response Error: Invalid JSON or no data given', response) from e
         else:
             return response
         
     def _request(self, url, action, headers, data=None, params=None, json=False):
         tries = 0
 
         while tries < 10:
```

### Comparing `syncqb-1.0.3/src/syncqb/quickbase.pyi` & `syncqb-1.0.4/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb/xml_quickbase.py` & `syncqb-1.0.4/src/syncqb/xml_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.4/src/syncqb/xml_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.4/src/syncqb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.3/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.4/src/syncqb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.3/tests/test.py` & `syncqb-1.0.4/tests/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,21 +30,27 @@
             'field': '19',
             'filename': 'test.txt',
             'value': 'MjM='
         }
     ]
 
     client = qb_client.get_xml_client()
-    client2 = qb_client.get_json_client(default='NOT APPLICABLE')
+    client2 = qb_client.get_json_client()
 
-    # xml_res = client.get_f
-    xml_res = 'N/A'
-    json_res = client2.do_query(
-        qid=13, database="bpxua87ct", sort=[22], ascending=False)
-    # json_res = 'N/A'
+    xml_res = client.do_query(
+        query='{3.EX.128}',
+        # qid=10, 
+        columns=[3, 6, 9], 
+        database='bnsucj684', 
+        # structured=True,
+        # qid_custom_headers=True
+    )
+    # xml_res = 'N/A'
+    # json_res = client2.get_file(database='bnsucj684', field=19, record=69036)
+    json_res = 'N/A'
 
     print('xml_res:', xml_res)
     print('json_res:', json_res)
```

