# Comparing `tmp/conductor_py-0.0.0.tar.gz` & `tmp/conductor_py-0.0.1.tar.gz`

## Comparing `conductor_py-0.0.0.tar` & `conductor_py-0.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 conductor_py-0.0.0/operations.graphql
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 conductor_py-0.0.0/schema.graphql
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 conductor_py-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/async_base_client.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/base_model.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/client.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/create_integration_connection.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/enums.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/exceptions.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/get_integration_connection.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/get_integration_connections.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/input_types.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/ping_integration_connection.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/scalars.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/graphql_client/send_integration_request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/netsuite/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 conductor_py-0.0.0/conductor_py/netsuite/invoice.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 conductor_py-0.0.0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 conductor_py-0.0.0/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 conductor_py-0.0.0/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conductor_py-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 conductor_py-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 conductor_py-0.0.1/operations.graphql
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 conductor_py-0.0.1/schema.graphql
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 conductor_py-0.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 conductor_py-0.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/__init__.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/base_model.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/client.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/create_integration_connection.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/enums.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connection.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connections.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/input_types.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/ping_integration_connection.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/scalars.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/graphql_client/send_integration_request.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/netsuite/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 conductor_py-0.0.1/conductor_py/netsuite/invoice.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 conductor_py-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 conductor_py-0.0.1/LICENSE
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 conductor_py-0.0.1/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 conductor_py-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 conductor_py-0.0.1/PKG-INFO
```

### Comparing `conductor_py-0.0.0/operations.graphql` & `conductor_py-0.0.1/operations.graphql`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/schema.graphql` & `conductor_py-0.0.1/schema.graphql`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/.github/workflows/python-publish.yml` & `conductor_py-0.0.1/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,12 @@
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
         run: python -m build
-      - name: Publish package
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      - name: Publish package to PyPi
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/__init__.py` & `conductor_py-0.0.1/conductor_py/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/async_base_client.py` & `conductor_py-0.0.1/conductor_py/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/base_model.py` & `conductor_py-0.0.1/conductor_py/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/client.py` & `conductor_py-0.0.1/conductor_py/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/create_integration_connection.py` & `conductor_py-0.0.1/conductor_py/graphql_client/create_integration_connection.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/exceptions.py` & `conductor_py-0.0.1/conductor_py/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/get_integration_connection.py` & `conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connection.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/get_integration_connections.py` & `conductor_py-0.0.1/conductor_py/graphql_client/get_integration_connections.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/input_types.py` & `conductor_py-0.0.1/conductor_py/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/ping_integration_connection.py` & `conductor_py-0.0.1/conductor_py/graphql_client/ping_integration_connection.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/conductor_py/graphql_client/send_integration_request.py` & `conductor_py-0.0.1/conductor_py/graphql_client/send_integration_request.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/.gitignore` & `conductor_py-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/LICENSE` & `conductor_py-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.0/pyproject.toml` & `conductor_py-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "conductor-py"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Danny Nemer", email="hi@dannynemer.com" },
 ]
 description = "Python bindings for the Conductor API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

