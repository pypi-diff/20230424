# Comparing `tmp/cujirax-0.6.0.tar.gz` & `tmp/cujirax-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.6.0.tar", last modified: Thu Apr 13 07:43:17 2023, max compression
+gzip compressed data, was "cujirax-0.7.0.tar", last modified: Mon Apr 24 15:46:57 2023, max compression
```

## Comparing `cujirax-0.6.0.tar` & `cujirax-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.6.0/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.6.0/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.6.0/README.md
--rw-r--r--   0        0        0    10469 2023-04-13 06:38:24.586970 cujirax-0.6.0/cujirax/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.6.0/cujirax/cucumber.py
--rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.6.0/cujirax/jira.py
--rw-r--r--   0        0        0     2485 2023-04-13 02:16:47.949068 cujirax-0.6.0/cujirax/xray/__init__.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.6.0/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.6.0/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.0/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.0/README.md
+-rw-r--r--   0        0        0    10469 2023-04-24 15:46:15.240638 cujirax-0.7.0/cujirax/__init__.py
+-rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.7.0/cujirax/cucumber.py
+-rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.0/cujirax/jira.py
+-rw-r--r--   0        0        0     2564 2023-04-24 15:45:21.596828 cujirax-0.7.0/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.0/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.0/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.7.0/PKG-INFO
```

### Comparing `cujirax-0.6.0/.gitignore` & `cujirax-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/LICENSE` & `cujirax-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/README.md` & `cujirax-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/cujirax/__init__.py` & `cujirax-0.7.0/cujirax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
```

### Comparing `cujirax-0.6.0/cujirax/cucumber.py` & `cujirax-0.7.0/cujirax/cucumber.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/cujirax/jira.py` & `cujirax-0.7.0/cujirax/jira.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/cujirax/xray/__init__.py` & `cujirax-0.7.0/cujirax/xray/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 import json
-from typing import List, Union
+from typing import List, Union, AnyStr
 from pydantic import BaseModel, Field
 import os
 import requests
 import time
 import functools
 
 
@@ -50,20 +50,22 @@
     header = Header()
     response = post(Endpoint.AUTHENTICATE.value, Authentication(), header)
     if response.status_code == 200:
         header.Authorization = "Bearer " + eval(response.text)
         return header
     raise Exception("Authentication error: Invalid credentials")
 
-def post(endpoint: str, payload: Union[BaseModel, List[BaseModel]], headers: Header)-> requests.Response:
+def post(endpoint: str, payload: Union[BaseModel, List[BaseModel], AnyStr], headers: Header)-> requests.Response:
     url = f"{xray_url}{endpoint}"
     if isinstance(payload, list):
         _payload = [p.dict(by_alias=True, exclude_none=True) for p in payload]
         _payload = json.dumps(_payload)
         # print("payload", _payload)
+    elif isinstance(payload, str): 
+        _payload = payload
     else:
         _payload = payload.json(by_alias=True, exclude_none=True)
 
     parameters = {
         "url": url,
         "method": "POST", 
         "headers": headers.dict(by_alias=True, exclude_none=True),
```

### Comparing `cujirax-0.6.0/cujirax/xray/import_results.py` & `cujirax-0.7.0/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/cujirax/xray/import_tests.py` & `cujirax-0.7.0/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.6.0/PKG-INFO` & `cujirax-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
```

