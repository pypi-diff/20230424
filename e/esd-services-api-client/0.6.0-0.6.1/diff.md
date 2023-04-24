# Comparing `tmp/esd_services_api_client-0.6.0.tar.gz` & `tmp/esd_services_api_client-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-0.6.0.tar", max compression
+gzip compressed data, was "esd_services_api_client-0.6.1.tar", max compression
```

## Comparing `esd_services_api_client-0.6.0.tar` & `esd_services_api_client-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10693 2023-03-14 09:56:50.442982 esd_services_api_client-0.6.0/LICENSE
--rw-r--r--   0        0        0      120 2023-03-14 09:56:50.442982 esd_services_api_client-0.6.0/README.md
--rw-r--r--   0        0        0      598 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2023-03-14 09:57:16.507092 esd_services_api_client-0.6.0/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      791 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/arcane/__init__.py
--rw-r--r--   0        0        0     1163 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/arcane/_api_versions.py
--rw-r--r--   0        0        0     7197 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/arcane/_connector.py
--rw-r--r--   0        0        0     5919 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/arcane/_models.py
--rw-r--r--   0        0        0      743 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0     2666 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/beast/_auth.py
--rw-r--r--   0        0        0    10369 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/beast/_connector.py
--rw-r--r--   0        0        0     9442 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/beast/_models.py
--rw-r--r--   0        0        0     2221 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      780 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     5214 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      976 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8272 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1736 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/_helpers.py
--rw-r--r--   0        0        0     3105 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      598 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      787 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      832 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0     9493 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4025 2023-03-14 09:56:50.446982 esd_services_api_client-0.6.0/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0      949 2023-03-14 09:57:16.507092 esd_services_api_client-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 esd_services_api_client-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/LICENSE
+-rw-r--r--   0        0        0      120 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/README.md
+-rw-r--r--   0        0        0      598 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-24 15:55:57.578765 esd_services_api_client-0.6.1/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      791 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/__init__.py
+-rw-r--r--   0        0        0     1163 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/_api_versions.py
+-rw-r--r--   0        0        0     7197 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/_connector.py
+-rw-r--r--   0        0        0     5919 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/arcane/_models.py
+-rw-r--r--   0        0        0      743 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0     2666 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/_auth.py
+-rw-r--r--   0        0        0    10369 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/_connector.py
+-rw-r--r--   0        0        0     9442 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/beast/_models.py
+-rw-r--r--   0        0        0     2221 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      780 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     5214 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      976 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8272 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1736 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_helpers.py
+-rw-r--r--   0        0        0     3105 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      598 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      787 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      832 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0     9493 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4025 2023-04-24 15:55:40.294283 esd_services_api_client-0.6.1/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0      949 2023-04-24 15:55:57.578765 esd_services_api_client-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 esd_services_api_client-0.6.1/PKG-INFO
```

### Comparing `esd_services_api_client-0.6.0/LICENSE` & `esd_services_api_client-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/__init__.py` & `esd_services_api_client-0.6.1/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/arcane/__init__.py` & `esd_services_api_client-0.6.1/esd_services_api_client/arcane/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/arcane/_api_versions.py` & `esd_services_api_client-0.6.1/esd_services_api_client/arcane/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/arcane/_connector.py` & `esd_services_api_client-0.6.1/esd_services_api_client/arcane/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/arcane/_models.py` & `esd_services_api_client-0.6.1/esd_services_api_client/arcane/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-0.6.1/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/beast/_auth.py` & `esd_services_api_client-0.6.1/esd_services_api_client/beast/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/beast/_connector.py` & `esd_services_api_client-0.6.1/esd_services_api_client/beast/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/beast/_models.py` & `esd_services_api_client-0.6.1/esd_services_api_client/beast/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/README.md` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/_helpers.py` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_helpers.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-0.6.1/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/common/__init__.py` & `esd_services_api_client-0.6.1/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-0.6.1/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-0.6.1/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-0.6.1/esd_services_api_client/crystal/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-0.6.1/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-0.6.0/pyproject.toml` & `esd_services_api_client-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "0.6.0"
+version = "0.6.1"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-adapta = { version="^2.0.0", extras = ["azure"] }
+python = ">=3.9,<3.12"
+adapta = { version="^2.2.0", extras = ["azure"] }
 dataclasses-json = "~0.5.7"
 pycryptodome = "~3.15"
 azure-identity = { version = "~1.7", optional = true }
 pyjwt = "~2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2"
```

### Comparing `esd_services_api_client-0.6.0/PKG-INFO` & `esd_services_api_client-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: azure
-Requires-Dist: adapta[azure] (>=2.0.0,<3.0.0)
+Requires-Dist: adapta[azure] (>=2.2.0,<3.0.0)
 Requires-Dist: azure-identity (>=1.7,<1.8) ; extra == "azure"
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: pycryptodome (>=3.15,<3.16)
 Requires-Dist: pyjwt (>=2.4.0,<2.5.0)
 Project-URL: Repository, https://github.com/SneaksAndData/esd-services-api-client
 Description-Content-Type: text/markdown
```

