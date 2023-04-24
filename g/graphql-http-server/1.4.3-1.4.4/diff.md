# Comparing `tmp/graphql_http_server-1.4.3.tar.gz` & `tmp/graphql_http_server-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.4.3.tar", last modified: Sun Apr 23 08:31:36 2023, max compression
+gzip compressed data, was "graphql_http_server-1.4.4.tar", last modified: Mon Apr 24 08:59:01 2023, max compression
```

## Comparing `graphql_http_server-1.4.3.tar` & `graphql_http_server-1.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.559430 graphql_http_server-1.4.3/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-23 08:31:36.559430 graphql_http_server-1.4.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-23 08:31:35.000000 graphql_http_server-1.4.3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.556429 graphql_http_server-1.4.3/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.558430 graphql_http_server-1.4.3/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)     3060 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9295 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/graphql_http_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.557429 graphql_http_server-1.4.3/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-23 08:31:36.000000 graphql_http_server-1.4.3/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-23 08:31:36.560430 graphql_http_server-1.4.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 08:31:36.559430 graphql_http_server-1.4.3/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     2246 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/test_app.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-23 08:31:27.000000 graphql_http_server-1.4.3/tests/test_graphql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:59:01.480842 graphql_http_server-1.4.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-24 08:59:01.480842 graphql_http_server-1.4.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 08:59:00.000000 graphql_http_server-1.4.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:59:01.476842 graphql_http_server-1.4.4/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:59:01.478842 graphql_http_server-1.4.4/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9295 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:59:01.478842 graphql_http_server-1.4.4/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-24 08:59:01.000000 graphql_http_server-1.4.4/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-24 08:59:01.000000 graphql_http_server-1.4.4/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:59:01.000000 graphql_http_server-1.4.4/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-24 08:59:01.000000 graphql_http_server-1.4.4/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-24 08:59:01.000000 graphql_http_server-1.4.4/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 08:59:01.481842 graphql_http_server-1.4.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:59:01.480842 graphql_http_server-1.4.4/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     2246 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2770 2023-04-24 08:58:51.000000 graphql_http_server-1.4.4/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.4.3/LICENSE` & `graphql_http_server-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/PKG-INFO` & `graphql_http_server-1.4.4/graphql_http_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: graphql_http_server
-Version: 1.4.3
+Name: graphql-http-server
+Version: 1.4.4
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.3.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.4.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.3/graphql_http_server/error.py` & `graphql_http_server-1.4.4/graphql_http_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/graphql_http_server/graphiql/index.html` & `graphql_http_server-1.4.4/graphql_http_server/graphiql/index.html`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/graphql_http_server/helpers.py` & `graphql_http_server-1.4.4/graphql_http_server/helpers.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/graphql_http_server/server.py` & `graphql_http_server-1.4.4/graphql_http_server/server.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: graphql-http-server
-Version: 1.4.3
+Name: graphql_http_server
+Version: 1.4.4
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.3.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.4.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.3/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.4/graphql_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/setup.py` & `graphql_http_server-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/tests/test_app.py` & `graphql_http_server-1.4.4/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.3/tests/test_graphql_api.py` & `graphql_http_server-1.4.4/tests/test_graphql_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,8 +102,7 @@
         assert "data" in response.json
         assert "errors" in response.json
 
         with pytest.raises(Exception):
             server.client().get(
                 '/?query={raiseHello}'
             )
-
```

