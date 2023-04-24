# Comparing `tmp/oatk-0.0.6.tar.gz` & `tmp/oatk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oatk-0.0.6.tar", last modified: Mon Apr 24 10:46:18 2023, max compression
+gzip compressed data, was "oatk-0.0.7.tar", last modified: Mon Apr 24 12:00:30 2023, max compression
```

## Comparing `oatk-0.0.6.tar` & `oatk-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.757566 oatk-0.0.6/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.751095 oatk-0.0.6/.github/
--rw-r--r--   0 xtof       (501) staff       (20)    21159 2023-04-24 10:45:00.000000 oatk-0.0.6/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2022-09-21 15:35:49.000000 oatk-0.0.6/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      154 2022-10-15 17:50:41.000000 oatk-0.0.6/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 10:46:18.757431 oatk-0.0.6/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.751558 oatk-0.0.6/examples/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-13 18:35:36.000000 oatk-0.0.6/examples/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      404 2022-10-15 11:27:46.000000 oatk-0.0.6/examples/create-and-validate.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.751939 oatk-0.0.6/examples/google/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-03-25 10:56:05.000000 oatk-0.0.6/examples/google/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1538 2023-04-24 10:45:04.000000 oatk-0.0.6/examples/google/app.py
--rw-r--r--   0 xtof       (501) staff       (20)      911 2022-10-15 14:53:02.000000 oatk-0.0.6/examples/web.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.752166 oatk-0.0.6/oatk/
--rw-r--r--   0 xtof       (501) staff       (20)     5538 2023-04-24 10:45:34.000000 oatk-0.0.6/oatk/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      751 2023-04-24 09:58:16.000000 oatk-0.0.6/oatk/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.753901 oatk-0.0.6/oatk/fake/
--rw-r--r--   0 xtof       (501) staff       (20)      907 2022-10-15 13:14:16.000000 oatk-0.0.6/oatk/fake/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1300 2022-10-15 13:16:23.000000 oatk-0.0.6/oatk/fake/db.py
--rw-r--r--   0 xtof       (501) staff       (20)     7971 2022-10-16 09:03:05.000000 oatk-0.0.6/oatk/fake/routes.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.754736 oatk-0.0.6/oatk/fake/static/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.6/oatk/fake/static/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)    12980 2022-10-15 14:45:31.000000 oatk-0.0.6/oatk/fake/static/oatk.js
--rw-r--r--   0 xtof       (501) staff       (20)     1341 2022-10-16 14:49:57.000000 oatk-0.0.6/oatk/fake/static/style.css
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.756660 oatk-0.0.6/oatk/fake/templates/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.6/oatk/fake/templates/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      459 2022-10-16 14:32:06.000000 oatk-0.0.6/oatk/fake/templates/authorize.html
--rw-r--r--   0 xtof       (501) staff       (20)      206 2022-10-16 14:31:57.000000 oatk-0.0.6/oatk/fake/templates/base.html
--rw-r--r--   0 xtof       (501) staff       (20)     1514 2022-10-16 14:51:49.000000 oatk-0.0.6/oatk/fake/templates/create_client.html
--rw-r--r--   0 xtof       (501) staff       (20)      249 2022-10-16 14:31:48.000000 oatk-0.0.6/oatk/fake/templates/dialog.html
--rw-r--r--   0 xtof       (501) staff       (20)      343 2022-10-16 14:49:16.000000 oatk-0.0.6/oatk/fake/templates/home.html
--rw-r--r--   0 xtof       (501) staff       (20)      254 2022-10-16 14:30:22.000000 oatk-0.0.6/oatk/fake/templates/login.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.757020 oatk-0.0.6/oatk/js/
--rw-r--r--   0 xtof       (501) staff       (20)      169 2023-04-15 12:40:08.000000 oatk-0.0.6/oatk/js/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 10:46:18.753013 oatk-0.0.6/oatk.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      762 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       44 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       94 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       14 2023-04-24 10:46:18.000000 oatk-0.0.6/oatk.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-04-24 10:46:18.757605 oatk-0.0.6/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1582 2023-04-15 08:19:14.000000 oatk-0.0.6/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.355230 oatk-0.0.7/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.348534 oatk-0.0.7/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)    21159 2023-04-24 10:48:41.000000 oatk-0.0.7/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2022-09-21 15:35:49.000000 oatk-0.0.7/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      154 2022-10-15 17:50:41.000000 oatk-0.0.7/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 12:00:30.355083 oatk-0.0.7/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.348981 oatk-0.0.7/examples/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-24 11:18:52.000000 oatk-0.0.7/examples/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      404 2022-10-15 11:27:46.000000 oatk-0.0.7/examples/create-and-validate.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.349376 oatk-0.0.7/examples/google/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-03-25 10:56:05.000000 oatk-0.0.7/examples/google/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1538 2023-04-24 11:19:17.000000 oatk-0.0.7/examples/google/app.py
+-rw-r--r--   0 xtof       (501) staff       (20)      911 2022-10-15 14:53:02.000000 oatk-0.0.7/examples/web.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.349735 oatk-0.0.7/oatk/
+-rw-r--r--   0 xtof       (501) staff       (20)     5538 2023-04-24 11:55:28.000000 oatk-0.0.7/oatk/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      751 2023-04-24 09:58:16.000000 oatk-0.0.7/oatk/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.351320 oatk-0.0.7/oatk/fake/
+-rw-r--r--   0 xtof       (501) staff       (20)      907 2022-10-15 13:14:16.000000 oatk-0.0.7/oatk/fake/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1300 2022-10-15 13:16:23.000000 oatk-0.0.7/oatk/fake/db.py
+-rw-r--r--   0 xtof       (501) staff       (20)     7971 2022-10-16 09:03:05.000000 oatk-0.0.7/oatk/fake/routes.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.352094 oatk-0.0.7/oatk/fake/static/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.7/oatk/fake/static/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)    12980 2022-10-15 14:45:31.000000 oatk-0.0.7/oatk/fake/static/oatk.js
+-rw-r--r--   0 xtof       (501) staff       (20)     1341 2022-10-16 14:49:57.000000 oatk-0.0.7/oatk/fake/static/style.css
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.354306 oatk-0.0.7/oatk/fake/templates/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2022-10-15 17:51:00.000000 oatk-0.0.7/oatk/fake/templates/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      459 2022-10-16 14:32:06.000000 oatk-0.0.7/oatk/fake/templates/authorize.html
+-rw-r--r--   0 xtof       (501) staff       (20)      206 2022-10-16 14:31:57.000000 oatk-0.0.7/oatk/fake/templates/base.html
+-rw-r--r--   0 xtof       (501) staff       (20)     1514 2022-10-16 14:51:49.000000 oatk-0.0.7/oatk/fake/templates/create_client.html
+-rw-r--r--   0 xtof       (501) staff       (20)      249 2022-10-16 14:31:48.000000 oatk-0.0.7/oatk/fake/templates/dialog.html
+-rw-r--r--   0 xtof       (501) staff       (20)      343 2022-10-16 14:49:16.000000 oatk-0.0.7/oatk/fake/templates/home.html
+-rw-r--r--   0 xtof       (501) staff       (20)      254 2022-10-16 14:30:22.000000 oatk-0.0.7/oatk/fake/templates/login.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.354669 oatk-0.0.7/oatk/js/
+-rw-r--r--   0 xtof       (501) staff       (20)      169 2023-04-15 12:40:08.000000 oatk-0.0.7/oatk/js/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-04-24 12:00:30.350460 oatk-0.0.7/oatk.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)    25748 2023-04-24 12:00:30.000000 oatk-0.0.7/oatk.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      762 2023-04-24 12:00:30.000000 oatk-0.0.7/oatk.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-04-24 12:00:30.000000 oatk-0.0.7/oatk.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       44 2023-04-24 12:00:30.000000 oatk-0.0.7/oatk.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       94 2023-04-24 12:00:30.000000 oatk-0.0.7/oatk.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       14 2023-04-24 12:00:30.000000 oatk-0.0.7/oatk.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-04-24 12:00:30.355283 oatk-0.0.7/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1582 2023-04-24 11:19:11.000000 oatk-0.0.7/setup.py
```

### Comparing `oatk-0.0.6/.github/README.md` & `oatk-0.0.7/.github/README.md`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/LICENSE.txt` & `oatk-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/PKG-INFO` & `oatk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oatk
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of useful functions for dealing with OAuth
 Home-page: https://github.com/christophevg/oatk
 Author: Christophe VG
 License: MIT
 Description: # OAuthToolKit
         
         > A collection of useful functions for dealing with OAuth
```

### Comparing `oatk-0.0.6/examples/google/app.py` & `oatk-0.0.7/examples/google/app.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/examples/web.py` & `oatk-0.0.7/examples/web.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/__init__.py` & `oatk-0.0.7/oatk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 import logging
 logger = logging.getLogger(__name__)
 
 import json
 import uuid
```

### Comparing `oatk-0.0.6/oatk/__main__.py` & `oatk-0.0.7/oatk/__main__.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/fake/__init__.py` & `oatk-0.0.7/oatk/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/fake/db.py` & `oatk-0.0.7/oatk/fake/db.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/fake/routes.py` & `oatk-0.0.7/oatk/fake/routes.py`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/fake/static/oatk.js` & `oatk-0.0.7/oatk/fake/static/oatk.js`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/fake/static/style.css` & `oatk-0.0.7/oatk/fake/static/style.css`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk/fake/templates/create_client.html` & `oatk-0.0.7/oatk/fake/templates/create_client.html`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/oatk.egg-info/PKG-INFO` & `oatk-0.0.7/oatk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oatk
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of useful functions for dealing with OAuth
 Home-page: https://github.com/christophevg/oatk
 Author: Christophe VG
 License: MIT
 Description: # OAuthToolKit
         
         > A collection of useful functions for dealing with OAuth
```

### Comparing `oatk-0.0.6/oatk.egg-info/SOURCES.txt` & `oatk-0.0.7/oatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oatk-0.0.6/setup.py` & `oatk-0.0.7/setup.py`

 * *Files identical despite different names*

