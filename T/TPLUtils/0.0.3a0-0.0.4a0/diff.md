# Comparing `tmp/TPLUtils-0.0.3a-.tar.gz` & `tmp/TPLUtils-0.0.4a-.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPLUtils-0.0.3a-.tar", last modified: Sun Apr 23 22:53:15 2023, max compression
+gzip compressed data, was "TPLUtils-0.0.4a-.tar", last modified: Mon Apr 24 00:43:25 2023, max compression
```

## Comparing `TPLUtils-0.0.3a-.tar` & `TPLUtils-0.0.4a-.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.693940 TPLUtils-0.0.3a-/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:53:15.693940 TPLUtils-0.0.3a-/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-23 22:53:06.000000 TPLUtils-0.0.3a-/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPL/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPL/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/website.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPL/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/utility/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/utility/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.436811 TPLUtils-0.0.4a-/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:43:25.436811 TPLUtils-0.0.4a-/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPL/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPL/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/website.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPL/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/utility/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/utility/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/top_level.txt
```

### Comparing `TPLUtils-0.0.3a-/src/TPL/db/config.py` & `TPLUtils-0.0.4a-/src/TPL/db/config.py`

 * *Files identical despite different names*

### Comparing `TPLUtils-0.0.3a-/src/TPL/db/user.py` & `TPLUtils-0.0.4a-/src/TPL/db/user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 
 from google.api_core.datetime_helpers import DatetimeWithNanoseconds
 from pydantic import BaseModel
 from fastapi import HTTPException, status
+from typing import Optional
 
 from src.TPL.db.config import db
 from src.TPL.utility.logging import logger
 
 class User(BaseModel):
     '''
     User class
     '''
     user_id: str
+    username: str
+
     allowed_deployments: int
     created_at: DatetimeWithNanoseconds
-    email: str
+    updated_at: Optional[DatetimeWithNanoseconds]
+    
     fname: str
+    lname: str
+
+    email: str
     github: str
     linkedin: str
-    lname: str
     phone: str
+
     photo_url: str
+    
     role: str
-    username: str
+    
+    # example:
+    # {
+    #    "<website_name>": "<website_id>",
+    #    "<website_name1>": "<website_id1>", 
+    #    ...
+    # }
     websites: dict
 
     @staticmethod
     def create(user_data: dict) -> 'User':
         user_data["created_at"] = DatetimeWithNanoseconds.now()
         new_user = User(**user_data)
         new_user.save()
```

### Comparing `TPLUtils-0.0.3a-/src/TPL/db/website.py` & `TPLUtils-0.0.4a-/src/TPL/db/website.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,23 +25,38 @@
     port_number: Optional[str] = None
     type: WebsiteType
 
 
 
 class Website(BaseModel):
     website_id: Optional[str]
+    owner_id: str
+
+    # website data structure creation date
     created_at: DatetimeWithNanoseconds
-    description: str
-    env: dict
+    # website data structure last update date, None if never updated
+    updated_at: Optional[DatetimeWithNanoseconds]
+    # website last deployment date, None if never deployed
+    deployed_at: Optional[DatetimeWithNanoseconds]
+
+    # information for profile card
     name: str
-    owner_id: str
+    description: str
+    profile_image: Optional[str] = None
+    profile_logo: Optional[str] = None
+
+    # information for deployment
+    env: dict    
     port_number: str
-    repo_name: str
-    type: WebsiteType
-    updated_at: Optional[DatetimeWithNanoseconds]
+    # full url of the repo
+    repo_url: str
+    template: WebsiteType
+    # path of the website: /user/<username>/<website_name>
+    path: str
+    
 
     def save(self):
         data = self.dict(exclude={'website_id'})
         website_ref = db.collection('websites').document(self.website_id)
         website_ref.set(data)
 
     def to_dict(self):
@@ -51,14 +66,16 @@
         website_ref = db.collection('websites').document(self.website_id)
         website_ref.delete()
 
     @staticmethod
     def create(website_data: dict) -> 'Website':
         new_website_id = str(uuid.uuid4())
         website_data["website_id"] = new_website_id
+        website_data["created_at"] = DatetimeWithNanoseconds.now()
+
         new_website = Website(**website_data)
         new_website.save()
         return new_website
     
     @staticmethod
     def get_from_id(website_id: str):
         website_ref = db.collection('websites').document(website_id)
```

### Comparing `TPLUtils-0.0.3a-/src/TPL/utility/security.py` & `TPLUtils-0.0.4a-/src/TPL/utility/security.py`

 * *Files identical despite different names*

