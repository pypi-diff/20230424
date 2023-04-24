# Comparing `tmp/gokyuzu-2.0.1.tar.gz` & `tmp/gokyuzu-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gokyuzu-2.0.1.tar", last modified: Mon Apr 24 18:02:41 2023, max compression
+gzip compressed data, was "gokyuzu-2.0.2.tar", last modified: Mon Apr 24 18:17:09 2023, max compression
```

## Comparing `gokyuzu-2.0.1.tar` & `gokyuzu-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:02:41.081216 gokyuzu-2.0.1/
--rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-2.0.1/LICENSE
--rw-r--r--   0 kilic      (501) staff       (20)     6343 2023-04-24 18:02:41.081095 gokyuzu-2.0.1/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)     5567 2023-04-24 17:58:52.000000 gokyuzu-2.0.1/README.md
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:02:41.079416 gokyuzu-2.0.1/gokyuzu/
--rw-r--r--   0 kilic      (501) staff       (20)     8586 2023-04-24 18:01:58.000000 gokyuzu-2.0.1/gokyuzu/BlueskyEndpoints.py
--rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-2.0.1/gokyuzu/BlueskyHelper.py
--rw-r--r--   0 kilic      (501) staff       (20)      224 2023-04-24 17:33:31.000000 gokyuzu-2.0.1/gokyuzu/BlueskyRecords.py
--rw-r--r--   0 kilic      (501) staff       (20)     4015 2023-04-24 17:31:55.000000 gokyuzu-2.0.1/gokyuzu/BlueskySession.py
--rw-r--r--   0 kilic      (501) staff       (20)    30303 2023-04-24 18:02:03.000000 gokyuzu-2.0.1/gokyuzu/__init__.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:02:41.080509 gokyuzu-2.0.1/gokyuzu.egg-info/
--rw-r--r--   0 kilic      (501) staff       (20)     6343 2023-04-24 18:02:41.000000 gokyuzu-2.0.1/gokyuzu.egg-info/PKG-INFO
--rw-r--r--   0 kilic      (501) staff       (20)      357 2023-04-24 18:02:41.000000 gokyuzu-2.0.1/gokyuzu.egg-info/SOURCES.txt
--rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-24 18:02:41.000000 gokyuzu-2.0.1/gokyuzu.egg-info/dependency_links.txt
--rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-24 18:02:41.000000 gokyuzu-2.0.1/gokyuzu.egg-info/requires.txt
--rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-24 18:02:41.000000 gokyuzu-2.0.1/gokyuzu.egg-info/top_level.txt
--rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-24 18:02:18.000000 gokyuzu-2.0.1/pyproject.toml
--rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-24 18:02:41.081252 gokyuzu-2.0.1/setup.cfg
--rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-24 18:02:09.000000 gokyuzu-2.0.1/setup.py
-drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:02:41.080763 gokyuzu-2.0.1/tests/
--rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-2.0.1/tests/__init__.py
--rw-r--r--   0 kilic      (501) staff       (20)     4706 2023-04-22 19:03:38.000000 gokyuzu-2.0.1/tests/test_main.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.049122 gokyuzu-2.0.2/
+-rw-r--r--   0 kilic      (501) staff       (20)       50 2023-04-22 15:30:32.000000 gokyuzu-2.0.2/LICENSE
+-rw-r--r--   0 kilic      (501) staff       (20)     6380 2023-04-24 18:17:09.049015 gokyuzu-2.0.2/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)     5604 2023-04-24 18:16:49.000000 gokyuzu-2.0.2/README.md
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.047634 gokyuzu-2.0.2/gokyuzu/
+-rw-r--r--   0 kilic      (501) staff       (20)     8586 2023-04-24 18:05:45.000000 gokyuzu-2.0.2/gokyuzu/BlueskyEndpoints.py
+-rw-r--r--   0 kilic      (501) staff       (20)      178 2023-04-22 16:36:29.000000 gokyuzu-2.0.2/gokyuzu/BlueskyHelper.py
+-rw-r--r--   0 kilic      (501) staff       (20)      224 2023-04-24 17:33:31.000000 gokyuzu-2.0.2/gokyuzu/BlueskyRecords.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4015 2023-04-24 17:31:55.000000 gokyuzu-2.0.2/gokyuzu/BlueskySession.py
+-rw-r--r--   0 kilic      (501) staff       (20)    30565 2023-04-24 18:16:31.000000 gokyuzu-2.0.2/gokyuzu/__init__.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.048481 gokyuzu-2.0.2/gokyuzu.egg-info/
+-rw-r--r--   0 kilic      (501) staff       (20)     6380 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/PKG-INFO
+-rw-r--r--   0 kilic      (501) staff       (20)      357 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 kilic      (501) staff       (20)        1 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       17 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/requires.txt
+-rw-r--r--   0 kilic      (501) staff       (20)       14 2023-04-24 18:17:09.000000 gokyuzu-2.0.2/gokyuzu.egg-info/top_level.txt
+-rw-r--r--   0 kilic      (501) staff       (20)      475 2023-04-24 18:16:57.000000 gokyuzu-2.0.2/pyproject.toml
+-rw-r--r--   0 kilic      (501) staff       (20)       38 2023-04-24 18:17:09.049157 gokyuzu-2.0.2/setup.cfg
+-rw-r--r--   0 kilic      (501) staff       (20)     1029 2023-04-24 18:16:58.000000 gokyuzu-2.0.2/setup.py
+drwxr-xr-x   0 kilic      (501) staff       (20)        0 2023-04-24 18:17:09.048700 gokyuzu-2.0.2/tests/
+-rw-r--r--   0 kilic      (501) staff       (20)        0 2023-04-22 15:30:32.000000 gokyuzu-2.0.2/tests/__init__.py
+-rw-r--r--   0 kilic      (501) staff       (20)     4706 2023-04-22 19:03:38.000000 gokyuzu-2.0.2/tests/test_main.py
```

### Comparing `gokyuzu-2.0.1/PKG-INFO` & `gokyuzu-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.1
+Version: 2.0.2
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -97,14 +97,15 @@
 - `def listAppPassword()`
 - `def getAccountInviteCodes( limit=10, includeUsed=True, create_available=True)` 
 - `def getSession()` 
 - `def requestAccountDelete()` 
 - `def requestPasswordReset( email)` 
 - `def resetPassword( email, password)` 
 - `def refreshSession()` 
+- `def revokeAppPassword( app_name)`
 
 #### com.atproto.sync
 
 - `def getBlob( repo_did, blob_cid)` 
 - `def getBlocks( did, cids)` 
 - `def getCheckout( did, commit=None)` 
 - `def getCommitPath( did, latest=None, earliest=None)`
```

### Comparing `gokyuzu-2.0.1/README.md` & `gokyuzu-2.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 - `def listAppPassword()`
 - `def getAccountInviteCodes( limit=10, includeUsed=True, create_available=True)` 
 - `def getSession()` 
 - `def requestAccountDelete()` 
 - `def requestPasswordReset( email)` 
 - `def resetPassword( email, password)` 
 - `def refreshSession()` 
+- `def revokeAppPassword( app_name)`
 
 #### com.atproto.sync
 
 - `def getBlob( repo_did, blob_cid)` 
 - `def getBlocks( did, cids)` 
 - `def getCheckout( did, commit=None)` 
 - `def getCommitPath( did, latest=None, earliest=None)`
```

### Comparing `gokyuzu-2.0.1/gokyuzu/BlueskyEndpoints.py` & `gokyuzu-2.0.2/gokyuzu/BlueskyEndpoints.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.1/gokyuzu/BlueskySession.py` & `gokyuzu-2.0.2/gokyuzu/BlueskySession.py`

 * *Files identical despite different names*

### Comparing `gokyuzu-2.0.1/gokyuzu/__init__.py` & `gokyuzu-2.0.2/gokyuzu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,14 +447,22 @@
         request_data = {
             "refresh_token": self.SESSION.getRefreshToken()
         } 
         response = self.SESSION.postJson(request_url, json=request_data)
         self.SESSION.useResponseBody(response.content)
         return response
 
+    def revokeAppPassword(self, app_name):
+        request_url = self.ENDPOINTS.revokeAppPassword()
+        request_data = {
+            "name": app_name
+        }
+        response = self.SESSION.postJson(request_url, json=request_data)
+        return response
+
     #endregion
 
     #region com.atproto.sync
     def getBlob(self, repo_did, blob_cid):
         request_url = self.ENDPOINTS.getBlob() + "?did={}&cid={}".format(repo_did, blob_cid)
         response = self.SESSION.get(request_url)
         return response
```

### Comparing `gokyuzu-2.0.1/gokyuzu.egg-info/PKG-INFO` & `gokyuzu-2.0.2/gokyuzu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gokyuzu
-Version: 2.0.1
+Version: 2.0.2
 Summary: bsky.social client library
 Home-page: https://github.com/kiliczsh/gokyuzu
 Author: Muhammed Kılıç
 Author-email: muhammeddkilicc@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -97,14 +97,15 @@
 - `def listAppPassword()`
 - `def getAccountInviteCodes( limit=10, includeUsed=True, create_available=True)` 
 - `def getSession()` 
 - `def requestAccountDelete()` 
 - `def requestPasswordReset( email)` 
 - `def resetPassword( email, password)` 
 - `def refreshSession()` 
+- `def revokeAppPassword( app_name)`
 
 #### com.atproto.sync
 
 - `def getBlob( repo_did, blob_cid)` 
 - `def getBlocks( did, cids)` 
 - `def getCheckout( did, commit=None)` 
 - `def getCommitPath( did, latest=None, earliest=None)`
```

### Comparing `gokyuzu-2.0.1/setup.py` & `gokyuzu-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gokyuzu',
-    version='2.0.1',
+    version='2.0.2',
     description='bsky.social client library',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Muhammed Kılıç',
     author_email='muhammeddkilicc@gmail.com',
     url='https://github.com/kiliczsh/gokyuzu',
     packages=find_packages(),
```

### Comparing `gokyuzu-2.0.1/tests/test_main.py` & `gokyuzu-2.0.2/tests/test_main.py`

 * *Files identical despite different names*

