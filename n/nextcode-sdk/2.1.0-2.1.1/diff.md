# Comparing `tmp/nextcode_sdk-2.1.0.tar.gz` & `tmp/nextcode_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode_sdk-2.1.0.tar", max compression
+gzip compressed data, was "nextcode_sdk-2.1.1.tar", max compression
```

## Comparing `nextcode_sdk-2.1.0.tar` & `nextcode_sdk-2.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1070 2023-04-18 15:04:38.684354 nextcode_sdk-2.1.0/LICENSE
--rw-r--r--   0        0        0     2393 2023-04-18 15:04:38.684354 nextcode_sdk-2.1.0/README.md
--rw-r--r--   0        0        0      647 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/__init__.py
--rw-r--r--   0        0        0     8570 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/client.py
--rw-r--r--   0        0        0     6482 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/config.py
--rw-r--r--   0        0        0     3327 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/credentials.py
--rw-r--r--   0        0        0     6746 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/csa.py
--rw-r--r--   0        0        0     1302 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/exceptions.py
--rw-r--r--   0        0        0    15309 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/keycloak.py
--rw-r--r--   0        0        0     1150 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/nextcode.py
--rw-r--r--   0        0        0     4292 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/packagelocal.py
--rw-r--r--   0        0        0     3081 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/__init__.py
--rw-r--r--   0        0        0      134 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenoteke/__init__.py
--rw-r--r--   0        0        0     1895 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenoteke/service.py
--rw-r--r--   0        0        0      167 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/__init__.py
--rw-r--r--   0        0        0     1789 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog.py
--rw-r--r--   0        0        0     1554 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog_run.py
--rw-r--r--   0        0        0      127 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/exceptions.py
--rw-r--r--   0        0        0     8034 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype.py
--rw-r--r--   0        0        0     3604 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype_matrix.py
--rw-r--r--   0        0        0     3803 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/playlist.py
--rw-r--r--   0        0        0    30337 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/service.py
--rw-r--r--   0        0        0      669 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/__init__.py
--rw-r--r--   0        0        0      224 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/exceptions.py
--rw-r--r--   0        0        0     5881 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/job.py
--rw-r--r--   0        0        0     3838 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/service.py
--rw-r--r--   0        0        0      214 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/project/__init__.py
--rw-r--r--   0        0        0      227 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/project/exceptions.py
--rw-r--r--   0        0        0    12632 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/project/service.py
--rw-r--r--   0        0        0      154 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/__init__.py
--rw-r--r--   0        0        0      481 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/exceptions.py
--rw-r--r--   0        0        0    16226 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/jupyter.py
--rw-r--r--   0        0        0    12837 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/query.py
--rw-r--r--   0        0        0    15851 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/service.py
--rw-r--r--   0        0        0     2142 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/utils.py
--rw-r--r--   0        0        0      135 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/queryserver/__init__.py
--rw-r--r--   0        0        0     6151 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/queryserver/result.py
--rw-r--r--   0        0        0     3842 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/queryserver/service.py
--rw-r--r--   0        0        0      310 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/__init__.py
--rw-r--r--   0        0        0      223 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/exceptions.py
--rw-r--r--   0        0        0    10501 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/job.py
--rw-r--r--   0        0        0     9159 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/pytest_plugin.py
--rw-r--r--   0        0        0    12238 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/service.py
--rw-r--r--   0        0        0     1574 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/weblog.py
--rw-r--r--   0        0        0     8172 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/session.py
--rw-r--r--   0        0        0     4350 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/utils.py
--rw-r--r--   0        0        0     2199 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 nextcode_sdk-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2393 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/README.md
+-rw-r--r--   0        0        0      647 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/__init__.py
+-rw-r--r--   0        0        0     8570 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/client.py
+-rw-r--r--   0        0        0     6482 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/config.py
+-rw-r--r--   0        0        0     3327 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/credentials.py
+-rw-r--r--   0        0        0     6746 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/csa.py
+-rw-r--r--   0        0        0     1302 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/exceptions.py
+-rw-r--r--   0        0        0    15309 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/keycloak.py
+-rw-r--r--   0        0        0     1150 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/nextcode.py
+-rw-r--r--   0        0        0     4292 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/packagelocal.py
+-rw-r--r--   0        0        0     3081 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/__init__.py
+-rw-r--r--   0        0        0      134 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenoteke/__init__.py
+-rw-r--r--   0        0        0     1895 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenoteke/service.py
+-rw-r--r--   0        0        0      167 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/__init__.py
+-rw-r--r--   0        0        0     1789 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/analysis_catalog.py
+-rw-r--r--   0        0        0     1554 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/analysis_catalog_run.py
+-rw-r--r--   0        0        0      127 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/exceptions.py
+-rw-r--r--   0        0        0     8034 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/phenotype.py
+-rw-r--r--   0        0        0     3604 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/phenotype_matrix.py
+-rw-r--r--   0        0        0     3803 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/playlist.py
+-rw-r--r--   0        0        0    30337 2023-04-24 16:45:38.261293 nextcode_sdk-2.1.1/nextcode/services/phenotype/service.py
+-rw-r--r--   0        0        0      669 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/pipelines/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/pipelines/exceptions.py
+-rw-r--r--   0        0        0     5881 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/pipelines/job.py
+-rw-r--r--   0        0        0     3838 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/pipelines/service.py
+-rw-r--r--   0        0        0      214 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/project/__init__.py
+-rw-r--r--   0        0        0      227 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/project/exceptions.py
+-rw-r--r--   0        0        0    12632 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/project/service.py
+-rw-r--r--   0        0        0      154 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/query/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/query/exceptions.py
+-rw-r--r--   0        0        0    16226 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/query/jupyter.py
+-rw-r--r--   0        0        0    12837 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/query/query.py
+-rw-r--r--   0        0        0    15851 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/query/service.py
+-rw-r--r--   0        0        0     2142 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/query/utils.py
+-rw-r--r--   0        0        0      135 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/queryserver/__init__.py
+-rw-r--r--   0        0        0     6151 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/queryserver/result.py
+-rw-r--r--   0        0        0     3842 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/queryserver/service.py
+-rw-r--r--   0        0        0      310 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/workflow/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/workflow/exceptions.py
+-rw-r--r--   0        0        0    10501 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/workflow/job.py
+-rw-r--r--   0        0        0     9159 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/workflow/pytest_plugin.py
+-rw-r--r--   0        0        0    12238 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/workflow/service.py
+-rw-r--r--   0        0        0     1574 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/services/workflow/weblog.py
+-rw-r--r--   0        0        0     8172 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/session.py
+-rw-r--r--   0        0        0     4350 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/nextcode/utils.py
+-rw-r--r--   0        0        0     2199 2023-04-24 16:45:38.265293 nextcode_sdk-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 nextcode_sdk-2.1.1/PKG-INFO
```

### Comparing `nextcode_sdk-2.1.0/LICENSE` & `nextcode_sdk-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/README.md` & `nextcode_sdk-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/__init__.py` & `nextcode_sdk-2.1.1/nextcode/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/client.py` & `nextcode_sdk-2.1.1/nextcode/client.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/config.py` & `nextcode_sdk-2.1.1/nextcode/config.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/credentials.py` & `nextcode_sdk-2.1.1/nextcode/credentials.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/csa.py` & `nextcode_sdk-2.1.1/nextcode/csa.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/exceptions.py` & `nextcode_sdk-2.1.1/nextcode/exceptions.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/keycloak.py` & `nextcode_sdk-2.1.1/nextcode/keycloak.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/nextcode.py` & `nextcode_sdk-2.1.1/nextcode/nextcode.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/packagelocal.py` & `nextcode_sdk-2.1.1/nextcode/packagelocal.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/__init__.py` & `nextcode_sdk-2.1.1/nextcode/services/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenoteke/service.py` & `nextcode_sdk-2.1.1/nextcode/services/phenoteke/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog.py` & `nextcode_sdk-2.1.1/nextcode/services/phenotype/analysis_catalog.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog_run.py` & `nextcode_sdk-2.1.1/nextcode/services/phenotype/analysis_catalog_run.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype.py` & `nextcode_sdk-2.1.1/nextcode/services/phenotype/phenotype.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype_matrix.py` & `nextcode_sdk-2.1.1/nextcode/services/phenotype/phenotype_matrix.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenotype/playlist.py` & `nextcode_sdk-2.1.1/nextcode/services/phenotype/playlist.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/phenotype/service.py` & `nextcode_sdk-2.1.1/nextcode/services/phenotype/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/pipelines/__init__.py` & `nextcode_sdk-2.1.1/nextcode/services/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/pipelines/job.py` & `nextcode_sdk-2.1.1/nextcode/services/pipelines/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/pipelines/service.py` & `nextcode_sdk-2.1.1/nextcode/services/pipelines/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/project/service.py` & `nextcode_sdk-2.1.1/nextcode/services/project/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/query/jupyter.py` & `nextcode_sdk-2.1.1/nextcode/services/query/jupyter.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/query/query.py` & `nextcode_sdk-2.1.1/nextcode/services/query/query.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/query/service.py` & `nextcode_sdk-2.1.1/nextcode/services/query/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/query/utils.py` & `nextcode_sdk-2.1.1/nextcode/services/query/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/queryserver/result.py` & `nextcode_sdk-2.1.1/nextcode/services/queryserver/result.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/queryserver/service.py` & `nextcode_sdk-2.1.1/nextcode/services/queryserver/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/workflow/job.py` & `nextcode_sdk-2.1.1/nextcode/services/workflow/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/workflow/pytest_plugin.py` & `nextcode_sdk-2.1.1/nextcode/services/workflow/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/workflow/service.py` & `nextcode_sdk-2.1.1/nextcode/services/workflow/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/services/workflow/weblog.py` & `nextcode_sdk-2.1.1/nextcode/services/workflow/weblog.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/session.py` & `nextcode_sdk-2.1.1/nextcode/session.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/nextcode/utils.py` & `nextcode_sdk-2.1.1/nextcode/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.1.0/pyproject.toml` & `nextcode_sdk-2.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nextcode-sdk"
-version = "2.1.0"
+version = "2.1.1"
 description = "Python SDK for Genuity Science Services"
 license = "MIT"
 authors = ["WUXI NextCODE <support@wuxinextcode.com>"]
 maintainers = ["Genuity Science Software Development <sdev@genuitysci.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/wuxi-nextcode/nextcode-python-sdk"
 repository = "https://www.github.com/wuxi-nextcode/nextcode-python-sdk"
@@ -30,34 +30,34 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dateutil = "^2.8.2"
 PyYAML = "^6.0"
 requests = "^2.28.2"
 hjson = "^3.1.0"
-boto3 = "^1.26.115"
-pandas = {version = "^2.0.0", optional = true}
+boto3 = "^1.26.118"
+pandas = {version = "^2.0.1", optional = true}
 ipython = {version = "^8.12.0", optional = true}
 termcolor = {version = "^2.2.0", optional = true}
 tqdm = {version = "^4.65.0", optional = true}
 ipywidgets = {version = "^8.0.6", optional = true}
-plotly = {version = "^5.14.0", optional = true}
+plotly = {version = "^5.14.1", optional = true}
 PyJWT = "^2.6.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 responses = "^0.23.1"
 pytest-cov = "^4.0.0"
 asserts = "^0.12.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^6.1.3"
 sphinx-bootstrap-theme = "^0.8.1"
 sphinx-rtd-theme = "^1.2.0"
-sphinx-autodoc-typehints = "^1.19.5"
+sphinx-autodoc-typehints = "^1.23.0"
 nbsphinx = "^0.9.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.12.0"
 
 [tool.poetry.extras]
 jupyter = ["pandas", "ipython", "termcolor", "tqdm", "ipywidgets", "plotly"]
```

### Comparing `nextcode_sdk-2.1.0/PKG-INFO` & `nextcode_sdk-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python SDK for Genuity Science Services
 Home-page: https://www.github.com/wuxi-nextcode/nextcode-python-sdk
 License: MIT
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 Maintainer: Genuity Science Software Development
 Maintainer-email: sdev@genuitysci.com
@@ -27,20 +27,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: jupyter
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: boto3 (>=1.26.115,<2.0.0)
+Requires-Dist: boto3 (>=1.26.118,<2.0.0)
 Requires-Dist: hjson (>=3.1.0,<4.0.0)
 Requires-Dist: ipython (>=8.12.0,<9.0.0) ; extra == "jupyter"
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0) ; extra == "jupyter"
-Requires-Dist: pandas (>=2.0.0,<3.0.0) ; extra == "jupyter"
-Requires-Dist: plotly (>=5.14.0,<6.0.0) ; extra == "jupyter"
+Requires-Dist: pandas (>=2.0.1,<3.0.0) ; extra == "jupyter"
+Requires-Dist: plotly (>=5.14.1,<6.0.0) ; extra == "jupyter"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0) ; extra == "jupyter"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0) ; extra == "jupyter"
 Project-URL: Documentation, https://wuxi-nextcode.github.io/nextcode-python-sdk/
 Project-URL: Repository, https://www.github.com/wuxi-nextcode/nextcode-python-sdk
 Description-Content-Type: text/markdown
```

