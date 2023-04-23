# Comparing `tmp/TPLUtils-0.0.2a-.tar.gz` & `tmp/TPLUtils-0.0.3a-.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPLUtils-0.0.2a-.tar", last modified: Sat Apr 22 03:57:38 2023, max compression
+gzip compressed data, was "TPLUtils-0.0.3a-.tar", last modified: Sun Apr 23 22:53:15 2023, max compression
```

## Comparing `TPLUtils-0.0.2a-.tar` & `TPLUtils-0.0.3a-.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:38.299248 TPLUtils-0.0.2a-/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/src/TPL/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/src/TPL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/src/TPL/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/src/TPL/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/src/TPL/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/src/TPL/db/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/src/TPL/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/src/TPL/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-22 03:57:28.000000 TPLUtils-0.0.2a-/src/TPL/utility/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 03:57:38.303248 TPLUtils-0.0.2a-/src/TPLUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-22 03:57:38.000000 TPLUtils-0.0.2a-/src/TPLUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-22 03:57:38.000000 TPLUtils-0.0.2a-/src/TPLUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 03:57:38.000000 TPLUtils-0.0.2a-/src/TPLUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 03:57:38.000000 TPLUtils-0.0.2a-/src/TPLUtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 03:57:38.000000 TPLUtils-0.0.2a-/src/TPLUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.693940 TPLUtils-0.0.3a-/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:53:15.693940 TPLUtils-0.0.3a-/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-23 22:53:06.000000 TPLUtils-0.0.3a-/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPL/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPL/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/db/website.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPL/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/utility/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-23 22:53:05.000000 TPLUtils-0.0.3a-/src/TPL/utility/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:53:15.689940 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 22:53:15.000000 TPLUtils-0.0.3a-/src/TPLUtils.egg-info/top_level.txt
```

### Comparing `TPLUtils-0.0.2a-/src/TPL/db/config.py` & `TPLUtils-0.0.3a-/src/TPL/db/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from firebase_admin import credentials, initialize_app, firestore
 import os
 
 from src.TPL.utility.logging import logger
 
-
 # initialize firebase auth and db
 try :
     key_file_path = os.environ.get("TPL_FIREBASE_AUTH")
     cred = credentials.Certificate(key_file_path)
     initialize_app(cred)
     db = firestore.client()
     logger.info("Firebase initialized")
```

### Comparing `TPLUtils-0.0.2a-/src/TPL/db/user.py` & `TPLUtils-0.0.3a-/src/TPL/db/user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,65 @@
+
 from google.api_core.datetime_helpers import DatetimeWithNanoseconds
 from pydantic import BaseModel
 from fastapi import HTTPException, status
 
-from db.config import db
-from utility.logging import logger
+from src.TPL.db.config import db
+from src.TPL.utility.logging import logger
 
 class User(BaseModel):
+    '''
+    User class
+    '''
     user_id: str
     allowed_deployments: int
     created_at: DatetimeWithNanoseconds
     email: str
     fname: str
     github: str
     linkedin: str
     lname: str
     phone: str
     photo_url: str
     role: str
     username: str
     websites: dict
 
+    @staticmethod
+    def create(user_data: dict) -> 'User':
+        user_data["created_at"] = DatetimeWithNanoseconds.now()
+        new_user = User(**user_data)
+        new_user.save()
+        return new_user
+
     def save(self) -> None:
+        '''
+        Save user to database
+        '''
         data = self.dict(exclude={'user_id'})
         user_ref = db.collection('users').document(self.user_id)
         user_ref.set(data)
 
     @staticmethod
     def get(user_id: str) -> 'User':
+        '''
+        Get user by user_id
+        '''
         user_ref = db.collection('users').document(user_id)
         try:
             user = user_ref.get().to_dict()
             user["user_id"] = user_id
         except Exception as e:
             logger.error(e)
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="User not found")
         return User(**user)
     
     @staticmethod
     def get_from_username(username: str) -> 'User':
+        '''
+        Get user by username
+        '''
         users_ref = db.collection('users')
         users = users_ref.where('username', '==', username).stream()
         for user in users:
             return User.get(user.id)
         raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="User not found")
```

