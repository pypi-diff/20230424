# Comparing `tmp/elefantolib-0.8.1.tar.gz` & `tmp/elefantolib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib-0.8.1.tar", max compression
+gzip compressed data, was "elefantolib-0.9.1.tar", max compression
```

## Comparing `elefantolib-0.8.1.tar` & `elefantolib-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-04-22 10:03:44.969858 elefantolib-0.8.1/LICENSE
--rw-r--r--   0        0        0      154 2023-04-22 10:03:44.969858 elefantolib-0.8.1/README.rst
--rw-r--r--   0        0        0       22 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/__init__.py
--rw-r--r--   0        0        0       36 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/constants.py
--rw-r--r--   0        0        0     1572 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/context/__init__.py
--rw-r--r--   0        0        0      663 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/context/context_service.py
--rw-r--r--   0        0        0      460 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/exceptions.py
--rw-r--r--   0        0        0      577 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/http_client/__init__.py
--rw-r--r--   0        0        0     2367 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/http_client/httpx_client.py
--rw-r--r--   0        0        0      373 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/logger_config.py
--rw-r--r--   0        0        0      889 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/middleware.py
--rw-r--r--   0        0        0      542 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/provider/__init__.py
--rw-r--r--   0        0        0      392 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/provider/django_provider/__init__.py
--rw-r--r--   0        0        0      386 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/provider/fastapi_provider/__init__.py
--rw-r--r--   0        0        0      404 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/websocket_client/__init__.py
--rw-r--r--   0        0        0      380 2023-04-22 10:03:44.969858 elefantolib-0.8.1/elefantolib/websocket_client/websocket_client.py
--rw-r--r--   0        0        0     1258 2023-04-22 10:03:44.969858 elefantolib-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 elefantolib-0.8.1/setup.py
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 elefantolib-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-24 16:13:52.984495 elefantolib-0.9.1/LICENSE
+-rw-r--r--   0        0        0      146 2023-04-24 16:13:52.984495 elefantolib-0.9.1/README.rst
+-rw-r--r--   0        0        0       22 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/__init__.py
+-rw-r--r--   0        0        0     1776 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/auth/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/auth/user.py
+-rw-r--r--   0        0        0      210 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/constants.py
+-rw-r--r--   0        0        0     1849 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/context/__init__.py
+-rw-r--r--   0        0        0      663 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/context/context_service.py
+-rw-r--r--   0        0        0     1256 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/exceptions.py
+-rw-r--r--   0        0        0      577 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/http_client/__init__.py
+-rw-r--r--   0        0        0     2367 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/http_client/httpx_client.py
+-rw-r--r--   0        0        0      373 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/logger_config.py
+-rw-r--r--   0        0        0      889 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/middleware.py
+-rw-r--r--   0        0        0      542 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/provider/__init__.py
+-rw-r--r--   0        0        0      392 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/provider/django_provider/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/provider/fastapi_provider/__init__.py
+-rw-r--r--   0        0        0      404 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/websocket_client/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-24 16:13:52.984495 elefantolib-0.9.1/elefantolib/websocket_client/websocket_client.py
+-rw-r--r--   0        0        0     1429 2023-04-24 16:14:04.759355 elefantolib-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 elefantolib-0.9.1/setup.py
+-rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 elefantolib-0.9.1/PKG-INFO
```

### Comparing `elefantolib-0.8.1/LICENSE` & `elefantolib-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.1/elefantolib/context/__init__.py` & `elefantolib-0.9.1/elefantolib/context/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Iterable, NoReturn
 
 from elefantolib import exceptions, provider
+from elefantolib.auth import UserTokenService
 from elefantolib.context import context_service
 from elefantolib.http_client import httpx_client
 from elefantolib.websocket_client import websocket_client
 
 
 class BaseContext:
     HTTP_CLIENT = None
     WEBSOCKET_CLIENT = None
+    user = None
     CONTEXT_ATTRIBUTES = (
         'auth_token',
         'correlation_id',
         'locale',
     )
     REQUIRED_ATTRIBUTES = (
         'auth_token',
@@ -30,14 +32,19 @@
     def context(self):
         return {a: getattr(self, a) for a in self.CONTEXT_ATTRIBUTES}
 
     def validate(self, required_attrs: Iterable = None) -> None | NoReturn:
         required_attrs = required_attrs or self.REQUIRED_ATTRIBUTES
 
         for required_attr in required_attrs:
+            if required_attr == 'auth_token' and (token := getattr(self, required_attr, None)):
+                uts = UserTokenService()
+                self.user = uts.extract_user(token)
+                continue
+
             if getattr(self, required_attr, None) is not None:
                 continue
 
             raise exceptions.ClientError(f'{required_attr} must be set for this request.')
 
         return None
```

### Comparing `elefantolib-0.8.1/elefantolib/context/context_service.py` & `elefantolib-0.9.1/elefantolib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.1/elefantolib/http_client/__init__.py` & `elefantolib-0.9.1/elefantolib/http_client/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.1/elefantolib/http_client/httpx_client.py` & `elefantolib-0.9.1/elefantolib/http_client/httpx_client.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.1/elefantolib/middleware.py` & `elefantolib-0.9.1/elefantolib/middleware.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.1/elefantolib/provider/__init__.py` & `elefantolib-0.9.1/elefantolib/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `elefantolib-0.8.1/pyproject.toml` & `elefantolib-0.9.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "elefantolib"
-version = "0.8.1"
 description = "Elefanto lib"
+version = "0.9.1"
 authors = ["Elefanto <elefanto@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/elefanto-organization/elefantolib"
 repository = "https://github.com/elefanto-organization/elefantolib"
 classifiers = [
     "Operating System :: OS Independent",
@@ -16,34 +16,44 @@
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.23.3"
+pyjwt = "^2.6.0"
+pytest-env = "^0.8.1"
 websockets = "^11.0"
 exceptiongroup = "^1.1.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-flake8 = "^1.1.1"
 pytest-mock = "^3.10.0"
 flake8-quotes = "^3.3.2"
 flake8-import-order = "^0.18.2"
 flake8-commas = "^2.1.0"
 flake8 = "4.0.1"
 pytest-asyncio = "^0.21.0"
 
+[tool.hatch.version]
+path = "elefantolib/__init__.py"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = "elefantolib"
 python_files = "tests.py test_*.py"
 python_classes = "*Test"
 addopts = "--cov=elefantolib --cov-report term-missing --flake8"
 testpaths = [
     "tests"
 ]
+env = [
+    "SECRET=Secret",
+    "ALGORITHM=HS256",
+    "ISSUER=Consumer",
+]
 flake8-max-line-length = 99
```

### Comparing `elefantolib-0.8.1/setup.py` & `elefantolib-0.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['elefantolib',
+ 'elefantolib.auth',
  'elefantolib.context',
  'elefantolib.http_client',
  'elefantolib.provider',
  'elefantolib.provider.django_provider',
  'elefantolib.provider.fastapi_provider',
  'elefantolib.websocket_client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['exceptiongroup>=1.1.1,<2.0.0',
  'httpx>=0.23.3,<0.24.0',
+ 'pyjwt>=2.6.0,<3.0.0',
+ 'pytest-env>=0.8.1,<0.9.0',
  'websockets>=11.0,<12.0']
 
 setup_kwargs = {
     'name': 'elefantolib',
-    'version': '0.8.1',
+    'version': '0.9.1',
     'description': 'Elefanto lib',
-    'long_description': 'Elefantolib\n-----------------------\n\n   **NOTE:** After clone this repository you should run command:\n\n   ``console git config core.hooksPath .githooks``\n',
+    'long_description': 'Elefantolib\n-----------------------\n\n   **NOTE:** After clone this repository you should run command:\n\n   ``git config core.hooksPath .githooks``\n',
     'author': 'Elefanto',
     'author_email': 'elefanto@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/elefanto-organization/elefantolib',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `elefantolib-0.8.1/PKG-INFO` & `elefantolib-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefantolib
-Version: 0.8.1
+Version: 0.9.1
 Summary: Elefanto lib
 Home-page: https://github.com/elefanto-organization/elefantolib
 License: MIT
 Author: Elefanto
 Author-email: elefanto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,18 +13,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
+Requires-Dist: pytest-env (>=0.8.1,<0.9.0)
 Requires-Dist: websockets (>=11.0,<12.0)
 Project-URL: Repository, https://github.com/elefanto-organization/elefantolib
 Description-Content-Type: text/x-rst
 
 Elefantolib
 -----------------------
 
    **NOTE:** After clone this repository you should run command:
 
-   ``console git config core.hooksPath .githooks``
+   ``git config core.hooksPath .githooks``
```

