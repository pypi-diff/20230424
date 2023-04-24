# Comparing `tmp/syncqb-1.0.4.tar.gz` & `tmp/syncqb-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.4.tar", last modified: Mon Apr 24 16:01:08 2023, max compression
+gzip compressed data, was "syncqb-1.0.5.tar", last modified: Mon Apr 24 19:19:19 2023, max compression
```

## Comparing `syncqb-1.0.4.tar` & `syncqb-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.4/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 16:01:08.288570 syncqb-1.0.4/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.4/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-04-24 16:00:32.000000 syncqb-1.0.4/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-24 16:01:08.288570 syncqb-1.0.4/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.4/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.4/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.4/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    16238 2023-04-21 17:31:28.000000 syncqb-1.0.4/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    11395 2023-04-21 14:13:40.000000 syncqb-1.0.4/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-04-13 17:15:37.000000 syncqb-1.0.4/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.4/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.4/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.4/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2799 2023-04-21 17:29:58.000000 syncqb-1.0.4/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.4/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-04-13 17:16:23.000000 syncqb-1.0.4/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.4/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-24 16:01:08.000000 syncqb-1.0.4/src/syncqb.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 16:01:08.288570 syncqb-1.0.4/tests/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1428 2023-04-13 17:50:02.000000 syncqb-1.0.4/tests/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.691053 syncqb-1.0.5/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.5/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 19:19:19.691053 syncqb-1.0.5/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.5/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-04-24 19:18:47.000000 syncqb-1.0.5/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-04-24 19:19:19.691053 syncqb-1.0.5/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.5/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.669386 syncqb-1.0.5/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.669386 syncqb-1.0.5/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.5/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.5/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    16238 2023-04-21 17:31:28.000000 syncqb-1.0.5/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    11395 2023-04-21 14:13:40.000000 syncqb-1.0.5/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-04-13 17:15:37.000000 syncqb-1.0.5/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.5/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.5/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.5/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2797 2023-04-24 18:59:22.000000 syncqb-1.0.5/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.5/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-04-13 17:16:23.000000 syncqb-1.0.5/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.5/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.680220 syncqb-1.0.5/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-04-24 19:19:19.000000 syncqb-1.0.5/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-04-24 19:19:19.691053 syncqb-1.0.5/tests/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1570 2023-04-24 16:41:50.000000 syncqb-1.0.5/tests/test.py
```

### Comparing `syncqb-1.0.4/LICENSE` & `syncqb-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/PKG-INFO` & `syncqb-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.4/README.md` & `syncqb-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/pyproject.toml` & `syncqb-1.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",'requests>=2.25.1','lxml>=4.6.3','chardet>=3.0.4']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syncqb"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Jacob Gearhardt", email="jacob@synctivate.com" },
 ]
 description = "A Python SDK for quickbase"
 readme = "README.md"
 license = { file="LICENSE" }
 dependencies = [
```

### Comparing `syncqb-1.0.4/src/syncqb/json_quickbase.py` & `syncqb-1.0.5/src/syncqb/json_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.5/src/syncqb/json_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/qb_client.py` & `syncqb-1.0.5/src/syncqb/qb_client.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/qb_client.pyi` & `syncqb-1.0.5/src/syncqb/qb_client.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/qb_errors.py` & `syncqb-1.0.5/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/qb_errors.pyi` & `syncqb-1.0.5/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/quickbase.py` & `syncqb-1.0.5/src/syncqb/quickbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,25 +40,25 @@
             raise ValueError('invalid action')
         
         if response.status_code == 401 or response.status_code == 403:
             raise QBAuthError('Invalid credentials')
         elif response.status_code == 404:
             raise QBConnectionError('Connection Error: Invalid URL')
         elif response.status_code == 400:
-            raise QBResponseError('Response Error: Invalid request', response)
+            raise QuickbaseError('Response Error: Invalid request', response)
         elif response.status_code == 429:
             raise QBResponseError('Response Error: Too many requests', response)
         elif response.status_code == 500:
             raise QBResponseError('Response Error: Internal Quickbase Server Error', response)
         
         if json:
             try:
                 return response.json()
             except Exception as e:
-                raise QBResponseError('Response Error: Invalid JSON or no data given', response) from e
+                raise QuickbaseError('Response Error: Invalid JSON or no data given', response) from e
         else:
             return response
         
     def _request(self, url, action, headers, data=None, params=None, json=False):
         tries = 0
 
         while tries < 10:
```

### Comparing `syncqb-1.0.4/src/syncqb/quickbase.pyi` & `syncqb-1.0.5/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/xml_quickbase.py` & `syncqb-1.0.5/src/syncqb/xml_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.5/src/syncqb/xml_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.5/src/syncqb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `syncqb-1.0.4/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.5/src/syncqb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.4/tests/test.py` & `syncqb-1.0.5/tests/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,25 +32,32 @@
             'value': 'MjM='
         }
     ]
 
     client = qb_client.get_xml_client()
     client2 = qb_client.get_json_client()
 
-    xml_res = client.do_query(
+    # xml_res = client.do_query(
+    #     query='{3.EX.128}',
+    #     # qid=10, 
+    #     columns=[3, 6, 9], 
+    #     database='bnsucj684', 
+    #     # structured=True,
+    #     # qid_custom_headers=True
+    # )
+    xml_res = 'N/A'
+    json_res = client2.do_query(
         query='{3.EX.128}',
         # qid=10, 
         columns=[3, 6, 9], 
         database='bnsucj684', 
         # structured=True,
         # qid_custom_headers=True
     )
-    # xml_res = 'N/A'
-    # json_res = client2.get_file(database='bnsucj684', field=19, record=69036)
-    json_res = 'N/A'
+    # json_res = 'N/A'
 
     print('xml_res:', xml_res)
     print('json_res:', json_res)
```

