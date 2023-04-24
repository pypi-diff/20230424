# Comparing `tmp/ghastoolkit-0.1.1.tar.gz` & `tmp/ghastoolkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.1.tar", last modified: Sat Apr 22 00:30:38 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.2.tar", last modified: Mon Apr 24 13:19:11 2023, max compression
```

## Comparing `ghastoolkit-0.1.1.tar` & `ghastoolkit-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/src/ghastoolkit/octokit/octokit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 00:30:38.000000 ghastoolkit-0.1.1/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:30:38.157886 ghastoolkit-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-22 00:30:11.000000 ghastoolkit-0.1.1/tests/test_octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_octokit.py
```

### Comparing `ghastoolkit-0.1.1/LICENSE` & `ghastoolkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/PKG-INFO` & `ghastoolkit-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMaher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMaher/ghastoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+[![Python Package](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml)
+
 # ghastoolkit
 GitHub Advanced Security Toolkit
```

### Comparing `ghastoolkit-0.1.1/pyproject.toml` & `ghastoolkit-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.1.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.2/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.2/src/ghastoolkit/octokit/octokit.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,27 +95,33 @@
             if len(responce_json) < RestRequest.PER_PAGE:
                 break
 
             page += 1
 
         return result
 
-    def postJson(self, path: str, data: dict, expected: int = 200):
+    def postJson(self, path: str, data: dict, expected: int = 200) -> dict:
         repo = self.repository or GitHub.repository
         if not repo:
             raise Exception("Repository needs to be set")
 
         url = Octokit.route(path, repo, rtype="rest")
         logger.debug(f"Posting content from URL :: {url}")
 
         response = self.session.post(url, json=data)
 
         if response.status_code != expected:
+            logger.error(f"Error code from server :: {response.status_code}")
+            known_error = __OCTOKIT_ERRORS__.get(response.status_code)
+            if known_error:
+                raise Exception(known_error)
             raise Exception(f"Failed to post data")
 
+        return response.json()
+
 
 class GraphQLRequest:
     locations: list[str] = [os.path.join(__OCTOKIT_PATH__, "queries")]
 
     @staticmethod
     def query(name: str, **options):
         query_content = GraphQLRequest.loadQuery(name)
```

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.1.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMaher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMaher/ghastoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+[![Python Package](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml)
+
 # ghastoolkit
 GitHub Advanced Security Toolkit
```

### Comparing `ghastoolkit-0.1.1/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/tests/test_codeqldb.py` & `ghastoolkit-0.1.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/tests/test_depgraph.py` & `ghastoolkit-0.1.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/tests/test_github.py` & `ghastoolkit-0.1.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.1/tests/test_octokit.py` & `ghastoolkit-0.1.2/tests/test_octokit.py`

 * *Files identical despite different names*

