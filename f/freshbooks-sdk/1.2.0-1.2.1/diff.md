# Comparing `tmp/freshbooks-sdk-1.2.0.tar.gz` & `tmp/freshbooks-sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freshbooks-sdk-1.2.0.tar", last modified: Sat Mar 25 20:29:29 2023, max compression
+gzip compressed data, was "freshbooks-sdk-1.2.1.tar", last modified: Mon Apr 24 13:15:04 2023, max compression
```

## Comparing `freshbooks-sdk-1.2.0.tar` & `freshbooks-sdk-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:29:29.061589 freshbooks-sdk-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-03-25 20:29:29.061589 freshbooks-sdk-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:29:29.057589 freshbooks-sdk-1.2.0/freshbooks/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:29:29.057589 freshbooks-sdk-1.2.0/freshbooks/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/accounting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/timetracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/api/uploads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:29:29.061589 freshbooks-sdk-1.2.0/freshbooks/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/builders/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/builders/includes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/builders/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/builders/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    18384 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/freshbooks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:29:29.061589 freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-03-25 20:29:29.000000 freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-25 20:29:29.000000 freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 20:29:29.000000 freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-25 20:29:29.000000 freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-25 20:29:29.000000 freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-25 20:29:29.061589 freshbooks-sdk-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-25 20:29:14.000000 freshbooks-sdk-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/freshbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/freshbooks/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/timetracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/api/uploads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/freshbooks/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/builders/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/builders/includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/builders/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/builders/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18486 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/freshbooks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-24 13:15:04.000000 freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-24 13:15:04.000000 freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:15:04.000000 freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 13:15:04.000000 freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 13:15:04.000000 freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 13:15:04.691446 freshbooks-sdk-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-24 13:14:54.000000 freshbooks-sdk-1.2.1/setup.py
```

### Comparing `freshbooks-sdk-1.2.0/LICENSE` & `freshbooks-sdk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/PKG-INFO` & `freshbooks-sdk-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: freshbooks-sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: API client for FreshBooks
 Home-page: https://github.com/freshbooks/freshbooks-python-sdk
-Download-URL: https://github.com/freshbooks/freshbooks-python-sdk/archive/release/1.2.0.tar.gz
+Download-URL: https://github.com/freshbooks/freshbooks-python-sdk/archive/release/1.2.1.tar.gz
 Author: Andrew McIntosh
 Author-email: andrew@amcintosh.net
 Maintainer: FreshBooks
 Maintainer-email: dev@freshbooks.com
 License: MIT
 Keywords: FreshBooks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freshbooks-sdk-1.2.0/README.md` & `freshbooks-sdk-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/__init__.py` & `freshbooks-sdk-1.2.1/freshbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/accounting.py` & `freshbooks-sdk-1.2.1/freshbooks/api/accounting.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/auth.py` & `freshbooks-sdk-1.2.1/freshbooks/api/auth.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/comments.py` & `freshbooks-sdk-1.2.1/freshbooks/api/comments.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/events.py` & `freshbooks-sdk-1.2.1/freshbooks/api/events.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/payments.py` & `freshbooks-sdk-1.2.1/freshbooks/api/payments.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/projects.py` & `freshbooks-sdk-1.2.1/freshbooks/api/projects.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/resource.py` & `freshbooks-sdk-1.2.1/freshbooks/api/resource.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/timetracking.py` & `freshbooks-sdk-1.2.1/freshbooks/api/timetracking.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/api/uploads.py` & `freshbooks-sdk-1.2.1/freshbooks/api/uploads.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/builders/filter.py` & `freshbooks-sdk-1.2.1/freshbooks/builders/filter.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/builders/includes.py` & `freshbooks-sdk-1.2.1/freshbooks/builders/includes.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/builders/paginator.py` & `freshbooks-sdk-1.2.1/freshbooks/builders/paginator.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/builders/sort.py` & `freshbooks-sdk-1.2.1/freshbooks/builders/sort.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/client.py` & `freshbooks-sdk-1.2.1/freshbooks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,23 +148,27 @@
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "grant_type": grant_type,
             "redirect_uri": self.redirect_uri,
             code_type: code
         }
         response = requests.post(self.token_url, payload, timeout=self.timeout)
-        content = response.json()
         try:
+            content = response.json()
             self.access_token = content["access_token"]
             self.refresh_token = content["refresh_token"]
             created_at = datetime.utcfromtimestamp(content["created_at"])
             expires_in = timedelta(seconds=content["expires_in"])
             self.access_token_expires_at = created_at + expires_in
         except KeyError:
-            raise FreshBooksError(response.status_code, "Failed to fetch access_token", raw_response=response.text)
+            raise FreshBooksError(
+                response.status_code,
+                content.get("error_description") or "Failed to fetch access_token",
+                raw_response=response.text
+            )
         return SimpleNamespace(
             access_token=self.access_token,
             refresh_token=self.refresh_token,
             access_token_expires_at=self.access_token_expires_at
         )
 
     def get_access_token(self, code: str) -> SimpleNamespace:
```

### Comparing `freshbooks-sdk-1.2.0/freshbooks/errors.py` & `freshbooks-sdk-1.2.1/freshbooks/errors.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks/models.py` & `freshbooks-sdk-1.2.1/freshbooks/models.py`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/PKG-INFO` & `freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: freshbooks-sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: API client for FreshBooks
 Home-page: https://github.com/freshbooks/freshbooks-python-sdk
-Download-URL: https://github.com/freshbooks/freshbooks-python-sdk/archive/release/1.2.0.tar.gz
+Download-URL: https://github.com/freshbooks/freshbooks-python-sdk/archive/release/1.2.1.tar.gz
 Author: Andrew McIntosh
 Author-email: andrew@amcintosh.net
 Maintainer: FreshBooks
 Maintainer-email: dev@freshbooks.com
 License: MIT
 Keywords: FreshBooks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `freshbooks-sdk-1.2.0/freshbooks_sdk.egg-info/SOURCES.txt` & `freshbooks-sdk-1.2.1/freshbooks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freshbooks-sdk-1.2.0/setup.cfg` & `freshbooks-sdk-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0
+current_version = 1.2.1
 commit = True
 tag = True
 tag_name = release/{new_version}
 message = 🔖 Bump version: {current_version} → {new_version}
 
 [wheel]
 universal = 1
```

### Comparing `freshbooks-sdk-1.2.0/setup.py` & `freshbooks-sdk-1.2.1/setup.py`

 * *Files identical despite different names*

