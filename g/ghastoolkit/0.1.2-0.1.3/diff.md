# Comparing `tmp/ghastoolkit-0.1.2.tar.gz` & `tmp/ghastoolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.2.tar", last modified: Mon Apr 24 13:19:11 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.3.tar", last modified: Mon Apr 24 15:36:13 2023, max compression
```

## Comparing `ghastoolkit-0.1.2.tar` & `ghastoolkit-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/src/ghastoolkit/octokit/octokit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 13:19:11.000000 ghastoolkit-0.1.2/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:19:11.444428 ghastoolkit-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 13:18:43.000000 ghastoolkit-0.1.2/tests/test_octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.727196 ghastoolkit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-24 15:36:13.727196 ghastoolkit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:36:13.727196 ghastoolkit-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.723196 ghastoolkit-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.723196 ghastoolkit-0.1.3/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.723196 ghastoolkit-0.1.3/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.727196 ghastoolkit-0.1.3/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/src/ghastoolkit/octokit/octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.723196 ghastoolkit-0.1.3/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-24 15:36:13.000000 ghastoolkit-0.1.3/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 15:36:13.000000 ghastoolkit-0.1.3/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:36:13.000000 ghastoolkit-0.1.3/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 15:36:13.000000 ghastoolkit-0.1.3/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:36:13.727196 ghastoolkit-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 15:35:45.000000 ghastoolkit-0.1.3/tests/test_octokit.py
```

### Comparing `ghastoolkit-0.1.2/LICENSE` & `ghastoolkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/PKG-INFO` & `ghastoolkit-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
-Project-URL: Homepage, https://github.com/GeekMaher/ghastoolkit
-Project-URL: Bug Tracker, https://github.com/GeekMaher/ghastoolkit/issues
+Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
+Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ghastoolkit-0.1.2/pyproject.toml` & `ghastoolkit-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/GeekMaher/ghastoolkit"
-"Bug Tracker" = "https://github.com/GeekMaher/ghastoolkit/issues"
+"Homepage" = "https://github.com/GeekMasher/ghastoolkit"
+"Bug Tracker" = "https://github.com/GeekMasher/ghastoolkit/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.3/src/ghastoolkit/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,31 @@
     DependencyGraph,
 )
 
 # Arguments
 parser = argparse.ArgumentParser(name)
 parser.add_argument("--debug", action="store_true")
 
-parser.add_argument("mode", choices=["codescanning", "codeql", "dependencygraph"])
+parser.add_argument(
+    "mode", choices=["all", "codescanning", "codeql", "dependencygraph"]
+)
 
 parser.add_argument("-sha", default=os.environ.get("GITHUB_SHA"), help="Commit SHA")
 parser.add_argument("-ref", default=os.environ.get("GITHUB_REF"), help="Commit ref")
 
 parser_github = parser.add_argument_group("GitHub")
 parser_github.add_argument(
     "-r",
     "--github-repository",
     default=os.environ.get("GITHUB_REPOSITORY"),
     help="GitHub Repository",
 )
 parser_github.add_argument(
     "--github-instance",
-    default=os.environ.get("GITHUB_API_URL", "https://api.github.com"),
+    default=os.environ.get("GITHUB_SERVER_URL", "https://github.com"),
     help="GitHub Instance",
 )
 parser_github.add_argument(
     "-t",
     "--github-token",
     default=os.environ.get("GITHUB_TOKEN"),
     help="GitHub API Token",
@@ -50,26 +52,32 @@
 # logger
 logging.basicConfig(
     level=logging.DEBUG if arguments.debug or os.environ.get("DEBUG") else logging.INFO,
     format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 )
 
 # GitHub Init
-GitHub.init(repository=arguments.github_repository, token=arguments.github_token)
+GitHub.init(
+    repository=arguments.github_repository,
+    instance=arguments.github_instance,
+    token=arguments.github_token,
+)
 
+if not GitHub.repository:
+    raise Exception(f"GitHub Repository must be set")
 
-if arguments.mode == "codescanning":
+if arguments.mode in ["all", "codescanning"]:
     header("Code Scanning")
     codescanning = CodeScanning(GitHub.repository)
 
     alerts = codescanning.getAlerts()
 
     print(f"Total Alerts :: {len(alerts)}")
 
-elif arguments.mode == "dependencygraph":
+if arguments.mode in ["all", "dependencygraph"]:
     header("Dependency Graph")
 
     depgraph = DependencyGraph(GitHub.repository)
     bom = depgraph.exportBOM()
     packages = bom.get("sbom", {}).get("packages", [])
 
     print(f"Total Dependencies :: {len(packages)}")
```

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.3/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.1.3/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.3/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.3/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.3/src/ghastoolkit/octokit/octokit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import logging
 from string import Template
-from typing import Optional
+from typing import Optional, Union
 from requests import Session
 
 from ghastoolkit.octokit.github import GitHub, Repository
 
 
 logger = logging.getLogger("ghastoolkit.octokit")
 
@@ -49,15 +49,15 @@
 
     def get(
         self,
         path: str,
         parameters: dict = {},
         expected: int = 200,
         authenticated: bool = False,
-    ) -> dict | list[dict]:
+    ) -> Union[dict, list[dict]]:
         repo = self.repository or GitHub.repository
         if not repo:
             raise Exception("Repository needs to be set")
 
         url = Octokit.route(path, repo, rtype="rest", **parameters)
         logger.debug(f"Fetching content from URL :: {url}")
 
@@ -74,14 +74,15 @@
             params["page"] = page
 
             responce = self.session.get(url, params=params)
             responce_json = responce.json()
 
             if responce.status_code != expected:
                 logger.error(f"Error code from server :: {responce.status_code}")
+                logger.error(f"Content :: {responce_json}")
                 known_error = __OCTOKIT_ERRORS__.get(responce.status_code)
                 if known_error:
                     raise Exception(known_error)
                 raise Exception("REST Request failed :: non-expected server error")
 
             if isinstance(responce_json, dict) and responce_json.get("errors"):
                 logger.error(responce_json.get("message"))
```

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.1.3/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
-Project-URL: Homepage, https://github.com/GeekMaher/ghastoolkit
-Project-URL: Bug Tracker, https://github.com/GeekMaher/ghastoolkit/issues
+Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
+Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ghastoolkit-0.1.2/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.3/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/tests/test_codeqldb.py` & `ghastoolkit-0.1.3/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/tests/test_depgraph.py` & `ghastoolkit-0.1.3/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/tests/test_github.py` & `ghastoolkit-0.1.3/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.2/tests/test_octokit.py` & `ghastoolkit-0.1.3/tests/test_octokit.py`

 * *Files identical despite different names*

