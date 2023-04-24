# Comparing `tmp/py-jama-rest-client-1.9.1.tar.gz` & `tmp/py-jama-rest-client-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-jama-rest-client-1.9.1.tar", last modified: Wed Dec  4 19:00:41 2019, max compression
+gzip compressed data, was "dist/py-jama-rest-client-1.9.2.tar", last modified: Mon Jan 13 20:26:09 2020, max compression
```

## Comparing `py-jama-rest-client-1.9.1.tar` & `py-jama-rest-client-1.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/
--rw-r--r--   0 nmchale  (72603470) 598265605     6363 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/PKG-INFO
--rw-r--r--   0 nmchale  (72603470) 598265605     4425 2019-08-06 21:14:29.000000 py-jama-rest-client-1.9.1/README.md
-drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client/
--rw-r--r--   0 nmchale  (72603470) 598265605        0 2019-01-12 20:00:15.000000 py-jama-rest-client-1.9.1/py_jama_rest_client/__init__.py
--rw-r--r--   0 nmchale  (72603470) 598265605    33377 2019-12-04 18:56:12.000000 py-jama-rest-client-1.9.1/py_jama_rest_client/client.py
--rw-r--r--   0 nmchale  (72603470) 598265605     4929 2019-07-24 20:22:00.000000 py-jama-rest-client-1.9.1/py_jama_rest_client/core.py
-drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/
--rw-r--r--   0 nmchale  (72603470) 598265605     6363 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/PKG-INFO
--rw-r--r--   0 nmchale  (72603470) 598265605      384 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/SOURCES.txt
--rw-r--r--   0 nmchale  (72603470) 598265605        1 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/dependency_links.txt
--rw-r--r--   0 nmchale  (72603470) 598265605        9 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/requires.txt
--rw-r--r--   0 nmchale  (72603470) 598265605       20 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/top_level.txt
--rw-r--r--   0 nmchale  (72603470) 598265605      107 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/setup.cfg
--rw-r--r--   0 nmchale  (72603470) 598265605     7877 2019-12-04 19:00:37.000000 py-jama-rest-client-1.9.1/setup.py
-drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2019-12-04 19:00:41.000000 py-jama-rest-client-1.9.1/test/
--rw-r--r--   0 nmchale  (72603470) 598265605    18295 2019-12-04 18:56:12.000000 py-jama-rest-client-1.9.1/test/test_jamaClient.py
--rw-r--r--   0 nmchale  (72603470) 598265605     1055 2019-04-05 16:31:08.000000 py-jama-rest-client-1.9.1/test/test_jamaClientCore.py
+drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/
+-rw-r--r--   0 nmchale  (72603470) 598265605     6388 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/PKG-INFO
+-rw-r--r--   0 nmchale  (72603470) 598265605     4442 2019-12-04 19:07:54.000000 py-jama-rest-client-1.9.2/README.md
+drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/py_jama_rest_client/
+-rw-r--r--   0 nmchale  (72603470) 598265605        0 2019-01-12 20:00:15.000000 py-jama-rest-client-1.9.2/py_jama_rest_client/__init__.py
+-rw-r--r--   0 nmchale  (72603470) 598265605    33670 2020-01-13 20:19:11.000000 py-jama-rest-client-1.9.2/py_jama_rest_client/client.py
+-rw-r--r--   0 nmchale  (72603470) 598265605     4929 2019-07-24 20:22:00.000000 py-jama-rest-client-1.9.2/py_jama_rest_client/core.py
+drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/
+-rw-r--r--   0 nmchale  (72603470) 598265605     6388 2020-01-13 20:26:08.000000 py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/PKG-INFO
+-rw-r--r--   0 nmchale  (72603470) 598265605      384 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nmchale  (72603470) 598265605        1 2020-01-13 20:26:08.000000 py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nmchale  (72603470) 598265605        9 2020-01-13 20:26:08.000000 py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/requires.txt
+-rw-r--r--   0 nmchale  (72603470) 598265605       20 2020-01-13 20:26:08.000000 py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/top_level.txt
+-rw-r--r--   0 nmchale  (72603470) 598265605      107 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/setup.cfg
+-rw-r--r--   0 nmchale  (72603470) 598265605     7877 2020-01-13 20:23:00.000000 py-jama-rest-client-1.9.2/setup.py
+drwxr-xr-x   0 nmchale  (72603470) 598265605        0 2020-01-13 20:26:09.000000 py-jama-rest-client-1.9.2/test/
+-rw-r--r--   0 nmchale  (72603470) 598265605    18295 2019-12-04 18:56:12.000000 py-jama-rest-client-1.9.2/test/test_jamaClient.py
+-rw-r--r--   0 nmchale  (72603470) 598265605     1055 2019-04-05 16:31:08.000000 py-jama-rest-client-1.9.2/test/test_jamaClientCore.py
```

### Comparing `py-jama-rest-client-1.9.1/PKG-INFO` & `py-jama-rest-client-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jama-rest-client
-Version: 1.9.1
+Version: 1.9.2
 Summary: A client for the Jama Connect REST API
 Home-page: https://github.com/JamaSoftware/py-jama-rest-client
 Author: Nick McHale
 Author-email: nmchale@jamasoftware.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/JamaSoftware/py-jama-rest-client/issues
 Project-URL: Source, https://github.com/JamaSoftware/py-jama-rest-client
@@ -67,14 +67,15 @@
         - GET all synced items
         - GET synced item sync status
         - GET Locked state of an item
         - DELETE an Item by ID
         - PATCH an Item
         - POST an item to a project
         - POST item attachment
+        - POST item sync
         - POST a tag to an item
         - PUT an item
         - PUT item lock
         
         ##### Relationship Types
         - GET all relationship types
         - GET a specific relationship type by ID
```

### Comparing `py-jama-rest-client-1.9.1/README.md` & `py-jama-rest-client-1.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 - GET all synced items
 - GET synced item sync status
 - GET Locked state of an item
 - DELETE an Item by ID
 - PATCH an Item
 - POST an item to a project
 - POST item attachment
+- POST item sync
 - POST a tag to an item
 - PUT an item
 - PUT item lock
 
 ##### Relationship Types
 - GET all relationship types
 - GET a specific relationship type by ID
```

### Comparing `py-jama-rest-client-1.9.1/py_jama_rest_client/client.py` & `py-jama-rest-client-1.9.2/py_jama_rest_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,16 +606,17 @@
         # Make the API Call
         response = self.__core.post(resource_path, data=json.dumps(body), headers=headers)
 
         # Validate response
         JamaClient.__handle_response_status(response)
         return response.json()['meta']['id']
 
-    def post_item(self, project, item_type_id, child_item_type_id, location, fields):
+    def post_item(self, project, item_type_id, child_item_type_id, location, fields, global_id=None):
         """ This method will post a new item to Jama Connect.
+        :param global_id: optional param to post the item with a custom global id
         :param project integer representing the project to which this item is to be posted
         :param item_type_id integer ID of an Item Type.
         :param child_item_type_id integer ID of an Item Type.
         :param location dictionary with integer ID of the parent item or project.
         :param fields dictionary item field data.
         :return integer ID of the successfully posted item or None if there was an error."""
 
@@ -625,16 +626,23 @@
             "childItemType": child_item_type_id,
             "location": {
                 "parent": location
             },
             "fields": fields
         }
         resource_path = 'items/'
+        params = {}
+
+        # we setting a global ID?
+        if global_id is not None:
+            body['globalId'] = global_id
+            params['setGlobalIdManually'] = True
+
         headers = {'content-type': 'application/json'}
-        response = self.__core.post(resource_path, data=json.dumps(body), headers=headers)
+        response = self.__core.post(resource_path, data=json.dumps(body), headers=headers, params=params)
         JamaClient.__handle_response_status(response)
         return response.json()['meta']['id']
 
     def post_item_tag(self, item_id, tag_id):
         """
         Add an existing tag to the item with the specified ID
         Args:
```

### Comparing `py-jama-rest-client-1.9.1/py_jama_rest_client/core.py` & `py-jama-rest-client-1.9.2/py_jama_rest_client/core.py`

 * *Files identical despite different names*

### Comparing `py-jama-rest-client-1.9.1/py_jama_rest_client.egg-info/PKG-INFO` & `py-jama-rest-client-1.9.2/py_jama_rest_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jama-rest-client
-Version: 1.9.1
+Version: 1.9.2
 Summary: A client for the Jama Connect REST API
 Home-page: https://github.com/JamaSoftware/py-jama-rest-client
 Author: Nick McHale
 Author-email: nmchale@jamasoftware.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/JamaSoftware/py-jama-rest-client/issues
 Project-URL: Source, https://github.com/JamaSoftware/py-jama-rest-client
@@ -67,14 +67,15 @@
         - GET all synced items
         - GET synced item sync status
         - GET Locked state of an item
         - DELETE an Item by ID
         - PATCH an Item
         - POST an item to a project
         - POST item attachment
+        - POST item sync
         - POST a tag to an item
         - PUT an item
         - PUT item lock
         
         ##### Relationship Types
         - GET all relationship types
         - GET a specific relationship type by ID
```

### Comparing `py-jama-rest-client-1.9.1/setup.py` & `py-jama-rest-client-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.9.1',  # Required
+    version='1.9.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A client for the Jama Connect REST API',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `py-jama-rest-client-1.9.1/test/test_jamaClient.py` & `py-jama-rest-client-1.9.2/test/test_jamaClient.py`

 * *Files identical despite different names*

### Comparing `py-jama-rest-client-1.9.1/test/test_jamaClientCore.py` & `py-jama-rest-client-1.9.2/test/test_jamaClientCore.py`

 * *Files identical despite different names*

