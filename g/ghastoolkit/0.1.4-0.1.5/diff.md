# Comparing `tmp/ghastoolkit-0.1.4.tar.gz` & `tmp/ghastoolkit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.4.tar", last modified: Mon Apr 24 16:16:40 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.5.tar", last modified: Mon Apr 24 18:35:30 2023, max compression
```

## Comparing `ghastoolkit-0.1.4.tar` & `ghastoolkit-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.642215 ghastoolkit-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.642215 ghastoolkit-0.1.4/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/src/ghastoolkit/octokit/octokit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-24 16:16:40.000000 ghastoolkit-0.1.4/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 16:16:40.000000 ghastoolkit-0.1.4/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:16:40.000000 ghastoolkit-0.1.4/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 16:16:40.000000 ghastoolkit-0.1.4/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 16:16:40.000000 ghastoolkit-0.1.4/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:16:40.646215 ghastoolkit-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 16:16:10.000000 ghastoolkit-0.1.4/tests/test_octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.770317 ghastoolkit-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.770317 ghastoolkit-0.1.5/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/src/ghastoolkit/octokit/octokit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 18:35:30.000000 ghastoolkit-0.1.5/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:35:30.774317 ghastoolkit-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 18:34:50.000000 ghastoolkit-0.1.5/tests/test_octokit.py
```

### Comparing `ghastoolkit-0.1.4/LICENSE` & `ghastoolkit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/PKG-INFO` & `ghastoolkit-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,7 +17,32 @@
 License-File: LICENSE
 
 
 [![Python Package](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml)
 
 # ghastoolkit
 GitHub Advanced Security Toolkit
+
+## Installing 
+
+**Pip:**
+
+```bash
+pip install ghastoolkit
+```
+
+**Pipenv:**
+
+``bach
+pipenv install ghastoolkit
+```
+
+## Usage 
+
+```python
+from ghastoolkit import GitHub
+
+
+GitHub.init("GeekMasher/ghastoolkit")
+
+```
+
```

### Comparing `ghastoolkit-0.1.4/pyproject.toml` & `ghastoolkit-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.5/src/ghastoolkit/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 arguments = parser.parse_args()
 
 
 def header(name: str):
     print("#" * 32)
     print(f"    {name}")
     print("#" * 32)
+    print("")
 
 
 # logger
 logging.basicConfig(
     level=logging.DEBUG if arguments.debug or os.environ.get("DEBUG") else logging.INFO,
     format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 )
@@ -69,14 +70,25 @@
     header("Code Scanning")
     codescanning = CodeScanning(GitHub.repository)
 
     alerts = codescanning.getAlerts()
 
     print(f"Total Alerts :: {len(alerts)}")
 
+    analyses = codescanning.getLatestAnalyses(GitHub.repository.reference)
+    print(f"\nTools:   ({len(analyses)})")
+
+    for analyse in analyses:
+        tool = analyse.get("tool", {}).get("name")
+        version = analyse.get("tool", {}).get("version")
+        created_at = analyse.get("created_at")
+
+        print(f" - {tool} v{version} ({created_at})")
+
+
 if arguments.mode in ["all", "dependencygraph"]:
     header("Dependency Graph")
 
     depgraph = DependencyGraph(GitHub.repository)
     bom = depgraph.exportBOM()
     packages = bom.get("sbom", {}).get("packages", [])
```

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.5/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.5/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.5/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.5/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.1.5/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,7 +17,32 @@
 License-File: LICENSE
 
 
 [![Python Package](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/GeekMasher/ghastoolkit/actions/workflows/python-package.yml)
 
 # ghastoolkit
 GitHub Advanced Security Toolkit
+
+## Installing 
+
+**Pip:**
+
+```bash
+pip install ghastoolkit
+```
+
+**Pipenv:**
+
+``bach
+pipenv install ghastoolkit
+```
+
+## Usage 
+
+```python
+from ghastoolkit import GitHub
+
+
+GitHub.init("GeekMasher/ghastoolkit")
+
+```
+
```

### Comparing `ghastoolkit-0.1.4/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.5/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/tests/test_codeqldb.py` & `ghastoolkit-0.1.5/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/tests/test_depgraph.py` & `ghastoolkit-0.1.5/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/tests/test_github.py` & `ghastoolkit-0.1.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.4/tests/test_octokit.py` & `ghastoolkit-0.1.5/tests/test_octokit.py`

 * *Files identical despite different names*

