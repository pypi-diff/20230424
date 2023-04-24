# Comparing `tmp/authup-0.5.0.tar.gz` & `tmp/authup-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authup-0.5.0.tar", max compression
+gzip compressed data, was "authup-0.5.1.tar", max compression
```

## Comparing `authup-0.5.0.tar` & `authup-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      104 2023-01-19 17:18:07.679160 authup-0.5.0/authup/__init__.py
--rw-r--r--   0        0        0     6175 2023-01-20 08:19:18.560848 authup-0.5.0/authup/authup.py
--rw-r--r--   0        0        0       33 2023-01-19 17:18:07.680157 authup-0.5.0/authup/client/__init__.py
--rw-r--r--   0        0        0     2047 2023-01-19 17:18:07.681162 authup-0.5.0/authup/client/base_resource_client.py
--rw-r--r--   0        0        0     1137 2023-01-19 17:18:07.681162 authup-0.5.0/authup/client/client.py
--rw-r--r--   0        0        0        0 2023-01-19 17:18:07.681162 authup-0.5.0/authup/client/resource_clients/__init__.py
--rw-r--r--   0        0        0      206 2023-01-19 17:18:07.682161 authup-0.5.0/authup/client/resource_clients/realm.py
--rw-r--r--   0        0        0     2176 2023-01-19 17:18:07.682161 authup-0.5.0/authup/permissions.py
--rw-r--r--   0        0        0        0 2022-12-22 08:56:44.349909 authup-0.5.0/authup/plugins/__init__.py
--rw-r--r--   0        0        0     1918 2023-01-08 17:14:14.660937 authup-0.5.0/authup/plugins/asgi.py
--rw-r--r--   0        0        0     1532 2023-01-19 17:18:07.683161 authup-0.5.0/authup/plugins/fastapi.py
--rw-r--r--   0        0        0      263 2023-01-20 07:30:42.929885 authup-0.5.0/authup/plugins/flask.py
--rw-r--r--   0        0        0      822 2023-01-09 17:13:25.546622 authup-0.5.0/authup/plugins/httpx.py
--rw-r--r--   0        0        0      259 2023-01-03 06:46:03.750817 authup-0.5.0/authup/plugins/requests.py
--rw-r--r--   0        0        0        0 2023-01-19 17:18:07.683161 authup-0.5.0/authup/schemas/__init__.py
--rw-r--r--   0        0        0      430 2023-01-19 17:18:07.684162 authup-0.5.0/authup/schemas/realm.py
--rw-r--r--   0        0        0      880 2023-01-19 17:18:07.684162 authup-0.5.0/authup/schemas/token.py
--rw-r--r--   0        0        0      668 2023-01-19 17:18:07.684162 authup-0.5.0/authup/schemas/user.py
--rw-r--r--   0        0        0     2059 2023-01-09 21:20:22.458977 authup-0.5.0/authup/settings.py
--rw-r--r--   0        0        0        0 2023-01-03 16:48:05.993171 authup-0.5.0/authup/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 17:18:07.685162 authup-0.5.0/authup/tests/client/__init__.py
--rw-r--r--   0        0        0      733 2023-01-19 17:18:07.685162 authup-0.5.0/authup/tests/client/test_client.py
--rw-r--r--   0        0        0     2043 2023-01-19 17:18:07.685162 authup-0.5.0/authup/tests/client/test_realm_client.py
--rw-r--r--   0        0        0     1610 2023-01-19 17:18:07.686161 authup-0.5.0/authup/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-01-02 16:17:04.024297 authup-0.5.0/authup/tests/plugins/__init__.py
--rw-r--r--   0        0        0     2824 2023-01-09 17:13:25.547134 authup-0.5.0/authup/tests/plugins/test_asgi.py
--rw-r--r--   0        0        0     2521 2023-01-19 17:18:07.686161 authup-0.5.0/authup/tests/plugins/test_fastapi.py
--rw-r--r--   0        0        0     1018 2023-01-09 17:13:25.548143 authup-0.5.0/authup/tests/plugins/test_httpx.py
--rw-r--r--   0        0        0      382 2023-01-03 07:36:08.952423 authup-0.5.0/authup/tests/plugins/test_requests.py
--rw-r--r--   0        0        0     4077 2023-01-20 08:19:18.555849 authup-0.5.0/authup/tests/test_authup.py
--rw-r--r--   0        0        0     1886 2023-01-19 17:18:07.687161 authup-0.5.0/authup/tests/test_permissions.py
--rw-r--r--   0        0        0     3035 2023-01-08 21:25:11.744745 authup-0.5.0/authup/tests/test_settings.py
--rw-r--r--   0        0        0     8559 2023-01-20 08:09:02.996051 authup-0.5.0/authup/tests/test_token.py
--rw-r--r--   0        0        0     5440 2023-01-20 08:09:02.978053 authup-0.5.0/authup/token.py
--rw-r--r--   0        0        0     2033 2023-01-20 08:20:15.042706 authup-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10165 2023-01-19 17:18:07.679160 authup-0.5.0/README.md
--rw-r--r--   0        0        0    11617 1970-01-01 00:00:00.000000 authup-0.5.0/setup.py
--rw-r--r--   0        0        0    11352 1970-01-01 00:00:00.000000 authup-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0    10165 2023-03-27 18:22:36.072053 authup-0.5.1/README.md
+-rwxr-xr-x   0        0        0      104 2023-03-27 18:22:36.072053 authup-0.5.1/authup/__init__.py
+-rwxr-xr-x   0        0        0     6175 2023-03-27 18:22:36.072053 authup-0.5.1/authup/authup.py
+-rwxr-xr-x   0        0        0       33 2023-03-27 18:22:36.072053 authup-0.5.1/authup/client/__init__.py
+-rwxr-xr-x   0        0        0     2047 2023-03-27 18:22:36.072053 authup-0.5.1/authup/client/base_resource_client.py
+-rwxr-xr-x   0        0        0     1137 2023-03-27 18:22:36.072053 authup-0.5.1/authup/client/client.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 18:22:36.072053 authup-0.5.1/authup/client/resource_clients/__init__.py
+-rwxr-xr-x   0        0        0      206 2023-03-27 18:22:36.072053 authup-0.5.1/authup/client/resource_clients/realm.py
+-rwxr-xr-x   0        0        0     2176 2023-03-27 18:22:36.072053 authup-0.5.1/authup/permissions.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 18:22:36.072053 authup-0.5.1/authup/plugins/__init__.py
+-rwxr-xr-x   0        0        0     1863 2023-03-27 18:22:36.072053 authup-0.5.1/authup/plugins/asgi.py
+-rwxr-xr-x   0        0        0     1532 2023-03-27 18:22:36.072053 authup-0.5.1/authup/plugins/fastapi.py
+-rwxr-xr-x   0        0        0      263 2023-03-27 18:22:36.072053 authup-0.5.1/authup/plugins/flask.py
+-rwxr-xr-x   0        0        0      822 2023-03-27 18:22:36.072053 authup-0.5.1/authup/plugins/httpx.py
+-rwxr-xr-x   0        0        0      249 2023-03-27 18:22:36.072053 authup-0.5.1/authup/plugins/requests.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 18:22:36.072053 authup-0.5.1/authup/schemas/__init__.py
+-rwxr-xr-x   0        0        0      430 2023-03-27 18:22:36.072053 authup-0.5.1/authup/schemas/realm.py
+-rwxr-xr-x   0        0        0      880 2023-03-27 18:22:36.072053 authup-0.5.1/authup/schemas/token.py
+-rwxr-xr-x   0        0        0      668 2023-03-27 18:22:36.072053 authup-0.5.1/authup/schemas/user.py
+-rwxr-xr-x   0        0        0     1988 2023-03-27 18:22:36.072053 authup-0.5.1/authup/settings.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/client/__init__.py
+-rwxr-xr-x   0        0        0      733 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/client/test_client.py
+-rwxr-xr-x   0        0        0     2043 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/client/test_realm_client.py
+-rwxr-xr-x   0        0        0     1610 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/conftest.py
+-rwxr-xr-x   0        0        0        0 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/plugins/__init__.py
+-rwxr-xr-x   0        0        0     2824 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/plugins/test_asgi.py
+-rwxr-xr-x   0        0        0     2521 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/plugins/test_fastapi.py
+-rwxr-xr-x   0        0        0     1018 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/plugins/test_httpx.py
+-rwxr-xr-x   0        0        0      373 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/plugins/test_requests.py
+-rwxr-xr-x   0        0        0     4077 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/test_authup.py
+-rwxr-xr-x   0        0        0     1886 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/test_permissions.py
+-rwxr-xr-x   0        0        0     3035 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/test_settings.py
+-rwxr-xr-x   0        0        0     8559 2023-03-27 18:22:36.072053 authup-0.5.1/authup/tests/test_token.py
+-rwxr-xr-x   0        0        0     5440 2023-03-27 18:22:36.072053 authup-0.5.1/authup/token.py
+-rwxr-xr-x   0        0        0     2015 2023-04-24 09:38:25.822586 authup-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    11297 1970-01-01 00:00:00.000000 authup-0.5.1/PKG-INFO
```

### Comparing `authup-0.5.0/authup/authup.py` & `authup-0.5.1/authup/authup.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/client/base_resource_client.py` & `authup-0.5.1/authup/client/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/client/client.py` & `authup-0.5.1/authup/client/client.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/permissions.py` & `authup-0.5.1/authup/permissions.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/plugins/fastapi.py` & `authup-0.5.1/authup/plugins/fastapi.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/plugins/httpx.py` & `authup-0.5.1/authup/plugins/httpx.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/schemas/token.py` & `authup-0.5.1/authup/schemas/token.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/schemas/user.py` & `authup-0.5.1/authup/schemas/user.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/client/test_client.py` & `authup-0.5.1/authup/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/client/test_realm_client.py` & `authup-0.5.1/authup/tests/client/test_realm_client.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/conftest.py` & `authup-0.5.1/authup/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/plugins/test_asgi.py` & `authup-0.5.1/authup/tests/plugins/test_asgi.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/plugins/test_fastapi.py` & `authup-0.5.1/authup/tests/plugins/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/plugins/test_httpx.py` & `authup-0.5.1/authup/tests/plugins/test_httpx.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/test_authup.py` & `authup-0.5.1/authup/tests/test_authup.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/test_permissions.py` & `authup-0.5.1/authup/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/test_settings.py` & `authup-0.5.1/authup/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/tests/test_token.py` & `authup-0.5.1/authup/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/authup/token.py` & `authup-0.5.1/authup/token.py`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/pyproject.toml` & `authup-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "authup"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python plugins for the Authup authentication and authorization framework"
 authors = ["Michael Graf <michael.graf3110@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/migraf/authup-py.git"
 readme = "README.md"
 homepage = "https://authup.org"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-httpx = "^0.23.2"
-pydantic = "^1.10.4"
+httpx = "*"
+pydantic = "*"
 fastapi = { version=">= 0.87.0", optional=true}
-requests = {version="^2.26.0", optional=true}
+requests = {version="*", optional=true}
 flask = {version="^2.0.0", optional=true}
 asgiref = "^3.6.0"
 
 
 [tool.poetry.extras]
 fastapi = ["fastapi"]
 requests = ["requests"]
```

### Comparing `authup-0.5.0/README.md` & `authup-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `authup-0.5.0/setup.py` & `authup-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,347 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: authup
+Version: 0.5.1
+Summary: Python plugins for the Authup authentication and authorization framework
+Home-page: https://authup.org
+License: MIT
+Author: Michael Graf
+Author-email: michael.graf3110@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: asgi
+Provides-Extra: fastapi
+Provides-Extra: flask
+Provides-Extra: requests
+Requires-Dist: asgiref (>=3.6.0,<4.0.0)
+Requires-Dist: fastapi (>=0.87.0) ; extra == "fastapi" or extra == "all"
+Requires-Dist: flask (>=2.0.0,<3.0.0) ; extra == "flask" or extra == "all"
+Requires-Dist: httpx
+Requires-Dist: pydantic
+Requires-Dist: requests ; extra == "requests" or extra == "all"
+Project-URL: Repository, https://github.com/migraf/authup-py.git
+Description-Content-Type: text/markdown
 
-packages = \
-['authup',
- 'authup.client',
- 'authup.client.resource_clients',
- 'authup.plugins',
- 'authup.schemas',
- 'authup.tests',
- 'authup.tests.client',
- 'authup.tests.plugins']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['asgiref>=3.6.0,<4.0.0', 'httpx>=0.23.2,<0.24.0', 'pydantic>=1.10.4,<2.0.0']
-
-extras_require = \
-{'all': ['fastapi>=0.87.0', 'requests>=2.26.0,<3.0.0', 'flask>=2.0.0,<3.0.0'],
- 'fastapi': ['fastapi>=0.87.0'],
- 'flask': ['flask>=2.0.0,<3.0.0'],
- 'requests': ['requests>=2.26.0,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'authup',
-    'version': '0.5.0',
-    'description': 'Python plugins for the Authup authentication and authorization framework',
-    'long_description': '[![CI](https://github.com/migraf/authup-py/actions/workflows/main.yml/badge.svg)](https://github.com/migraf/authup-py/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/migraf/authup-py/branch/main/graph/badge.svg?token=qILJEFdh8I)](https://codecov.io/gh/migraf/authup-py)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/authup)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/authup)\n[![Maintainability](https://api.codeclimate.com/v1/badges/520401d6c07170a6e413/maintainability)](https://codeclimate.com/github/migraf/authup-py/maintainability)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# Authup Python Plugins\n\nThis repository contains python plugins for using the [Authup](https://authup.org) authentication and authorization\nframework in the python language.\nThe plugins are used to integrate Authup with different python frameworks and libraries.\n\n## Supported Python frameworks\n\n### Client\n| Plugin                                      | Extra        | Sync | Async |\n|---------------------------------------------|--------------|:----:|------:|\n| [httpx](https://github.com/encode/httpx)    |              |  ✅   |     ✅ |\n| [requests](https://github.com/psf/requests) | `[requests]` |  ✅   |     ❌ |\n\n### Server\n\n| Plugin                                                        | Extra       | Sync | Async | Middleware | User |\n|---------------------------------------------------------------|-------------|:----:|------:|------------|------|\n| [FastApi](https://fastapi.tiangolo.com/)                      | `[fastapi]` |  ✅   |     ✅ | ✅          | ✅    |\n| [ASGI](https://asgi.readthedocs.io/en/latest/specs/main.html) | `[asgi]`    |  ❌   |     ✅ | ✅          | ✅    |\n| [Flask](https://flask.palletsprojects.com/en/2.2.x/)          | `[flask]`   |  ⏳   |     ⏳ | ⏳          | ⏳    |\n\nTable of Contents\n=================\n\n* [Authup Python Plugins](#authup-python-plugins)\n   * [Supported Python frameworks](#supported-python-frameworks)\n      * [Client](#client)\n      * [Server](#server)\n   * [Installation](#installation)\n      * [Extra dependencies](#extra-dependencies)\n   * [How to use](#how-to-use)\n      * [httpx](#httpx)\n      * [requests](#requests)\n      * [ASGI Middleware](#asgi-middleware)\n         * [Optional user injection](#optional-user-injection)\n      * [FastAPI Dependency](#fastapi-dependency)\n         * [Basic user dependency](#basic-user-dependency)\n         * [Require permissions](#require-permissions)\n   * [How to develop](#how-to-develop)\n      * [Install](#install)\n      * [Test](#test)\n\n\n## Installation\n\nThe plugins are available via [PyPi](https://pypi.org/project/authup-py/).\n\n```bash\npip install authup-py\n```\n\n### Extra dependencies\nThe plugin for the project\'s base library [httpx](https://github.com/encode/httpx) needs no extra dependencies. To\nuse the additional plugins for other libraries, you need to install with the corresponding extra i.e. for `requests`:\n\n```bash\npip install authup-py[requests]\n```\n\n## How to use\nAll the plugins share the underlying `Authup` class. The class is initialized with the url of the Authup server and\nthe credentials you would like to use (username/password or robot_id/secret).    \nThe class provides both sync and async methods for the different authentication and authorization flows.\n\n```python\n\nfrom authup import Authup\n\nauthup = Authup(\n    url="https://authup.org",\n    username="username",\n    password="password"\n)\n\nauthup_robot = Authup(\n    url="https://authup.org",\n    robot_id="robot",\n    robot_secret="secret"\n)\n\n```\n\nThe following plugins all expect the same arguments as the `Authup` class with the addition of the\napp as a first argument for server side libraries (e.g. FastApi, Flask).\n\n### httpx\nFor synchronously using the plugin with [httpx](https://github.com/encode/httpx) , you can use the `AuthupHttpx` class and pass an instance to your\n`httpx.Client` or a basic `httpx.Request` as the `auth` parameter:\n\n```python\nimport httpx\nfrom authup.plugins.httpx import AuthupHttpx\n\nauthup = AuthupHttpx(\n    url="https://authup.org",\n    username="username",\n    password="password",\n)\n\n# Use the authup instance as the auth parameter for the httpx client\nclient = httpx.Client(auth=authup)\n\nwith client:\n    response = client.get("https://authup.org")\n    print(response.status_code)\n\n\n# Use the authup instance as the auth parameter for a top level request function\nrequest = httpx.get("https://authup.org", auth=authup)\n\n```\n\nIt works the same way for the asynchronous httpx client:\n\n```python\nimport httpx\nfrom authup.plugins.httpx import AuthupHttpxAsync\n\nauthup = AuthupHttpxAsync(\n    url="https://authup.org",\n    username="username",\n    password="password",\n)\n\nasync with httpx.AsyncClient(auth=authup) as client:\n    response = await client.get("https://authup.org")\n    print(response.status_code)\n\n```\n\n### requests\nSince [requests](https://github.com/psf/requests) is a synchronous library, the plugin is also synchronous. You can use the `AuthupRequests` class and\nuse it with the `requests.Session` or the `requests.request` functions:\n> **Note**\n> Requires the `requests` extra to be installed. `pip install authup-py[requests]`\n\n```python\nimport requests\nfrom authup.plugins.requests import AuthupRequests\n\nauthup = AuthupRequests(\n    url="https://authup.org",\n    username="username",\n    password="password",\n)\n\n# Use the authup instance as the auth parameter for the requests session\nwith requests.Session() as session:\n    session.auth = authup\n    response = session.get("https://authup.org")\n    print(response.status_code)\n\n# Use the authup instance as the auth parameter for a top level request function\nresponse = requests.get("https://authup.org", auth=authup)\nprint(response.status_code)\n\n```\n\n### ASGI Middleware\n\nThe `AuthupASGIMiddleware` class can be used as an ASGI middleware for any ASGI framework (i.e. FastAPI, Starlette). \nThe middleware will check the incoming requests for a valid token and otherwise return a 401 response. If you pass the\noptional `user` parameter, the middleware will inject the user object into the request scope (`r.state.user`).\n\nThe first argument is the ASGI application and the second argument is the URL of the authup instance.\n> **Note**\n> Requires the `asgi` extra to be installed. `pip install authup-py[asgi]`\n\nThe following shows a simple example for using the middleware with a FastAPI application but it should work with any ASGI framework.\n\n> **Note**\n> Expects a running authup instance available at the given URL.\n> \n```python\nfrom fastapi import FastAPI\nfrom authup.plugins.asgi import AuthupASGIMiddleware\n\napp = FastAPI()\n\nauthup_url = "https://authup.org"  # change to your authup instance\n@app.get("/test")\nasync def test():\n    return {"message": "Hello World"}\n\n# register the middleware pass the authup url as argument\napp.add_middleware(AuthupASGIMiddleware, authup_url=authup_url)\n\n```\nNow you can access the `/test` endpoint without a token and will receive a 401 response. When using a valid token, you will receive the expected response.\n\n```python\nimport httpx\nfrom authup.plugins.httpx import AuthupHttpx\n\n# no token or invalid token raises 401\nresponse = httpx.get("http://localhost:8000/test") # 401\nprint(response.status_code)\n\n# valid token receives the expected response\nauthup = AuthupHttpx(\n    url="https://authup.org",\n    username="username",\n    password="password",\n)\n\nresponse = httpx.get("http://localhost:8000/test", auth=authup) # 200\nprint(response.status_code)\n\n```\n\n#### Optional user injection\nSet the `user` parameter to `True` when adding the middleware to your ASGI application:\n\n```python\nfrom fastapi import FastAPI, Request\nfrom authup.plugins.asgi import AuthupASGIMiddleware\n\napp = FastAPI()\n\nauthup_url = "https://authup.org"  # change to your authup instance\n@app.get("/test-user")\nasync def test(request: Request):\n    return {"user": request.state.user}\n\n# register the middleware pass the authup url as argument\napp.add_middleware(AuthupASGIMiddleware, authup_url=authup_url, user=True)\n\n```\n\nCalling the `/test-user` endpoint without a token will return a 401 response. When using a valid token, the user object \nwill be injected into the request scope, and you will receive the expected response containing your user.\n\n### FastAPI Dependency\nThe `AuthupUser` class can be used as a FastAPI dependency. \nIt will check the incoming requests for a valid token and otherwise return a 401 response. If the token is valid a user object\nwill be available in the dependency call.\n\n#### Basic user dependency\nThe following shows a simple example for using the dependency with a FastAPI application that will return the user\nobject obtained from the token.\n\n```python\nfrom fastapi import FastAPI, Depends\nfrom authup.plugins.fastapi import AuthupUser\nfrom authup import User\n\n\napp = FastAPI()\n\nuser_dependency = AuthupUser(url="http://localhost:3010")\n\n@app.get("/test")\nasync def user_test(user: User = Depends(user_dependency)):\n    return {"user": user.dict()}\n\n```\n\n#### Require permissions\nYou can also require specific permissions for the user. The following example will only allow users with the \n`client_add` permission and a power level of over `100`. Otherwise, a 401 response will be returned.\n\n```python\nfrom fastapi import FastAPI, Depends\nfrom authup.plugins.fastapi import AuthupUser\nfrom authup import User\nfrom authup.permissions import Permission\n\npermissions = [\n        Permission(name="client_add", inverse=False, power=100),\n    ]\n\nrequired_permissions = AuthupUser(\n    url="http://localhost:3010",\n    permissions=permissions,\n)\n\napp = FastAPI()\n\n@app.get("/test")\nasync def user_test(user: User = Depends(required_permissions)):\n    return {"user": user.dict()}\n\n```\n\n\n\n## How to develop\n\n### Install\n\nRequires [poetry](https://python-poetry.org/) and [pre-commit](https://pre-commit.com/) and python 3.7+.\n\n```shell\npoetry install --with dev --all-extras\n```\n\nInstall pre-commit hooks\n\n```shell\npoetry run pre-commit install\n```\n\n### Test\n\n```shell\npoetry run pytest\n```\n\n',
-    'author': 'Michael Graf',
-    'author_email': 'michael.graf3110@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://authup.org',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+[![CI](https://github.com/migraf/authup-py/actions/workflows/main.yml/badge.svg)](https://github.com/migraf/authup-py/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/migraf/authup-py/branch/main/graph/badge.svg?token=qILJEFdh8I)](https://codecov.io/gh/migraf/authup-py)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/authup)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/authup)
+[![Maintainability](https://api.codeclimate.com/v1/badges/520401d6c07170a6e413/maintainability)](https://codeclimate.com/github/migraf/authup-py/maintainability)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# Authup Python Plugins
+
+This repository contains python plugins for using the [Authup](https://authup.org) authentication and authorization
+framework in the python language.
+The plugins are used to integrate Authup with different python frameworks and libraries.
+
+## Supported Python frameworks
+
+### Client
+| Plugin                                      | Extra        | Sync | Async |
+|---------------------------------------------|--------------|:----:|------:|
+| [httpx](https://github.com/encode/httpx)    |              |  ✅   |     ✅ |
+| [requests](https://github.com/psf/requests) | `[requests]` |  ✅   |     ❌ |
+
+### Server
+
+| Plugin                                                        | Extra       | Sync | Async | Middleware | User |
+|---------------------------------------------------------------|-------------|:----:|------:|------------|------|
+| [FastApi](https://fastapi.tiangolo.com/)                      | `[fastapi]` |  ✅   |     ✅ | ✅          | ✅    |
+| [ASGI](https://asgi.readthedocs.io/en/latest/specs/main.html) | `[asgi]`    |  ❌   |     ✅ | ✅          | ✅    |
+| [Flask](https://flask.palletsprojects.com/en/2.2.x/)          | `[flask]`   |  ⏳   |     ⏳ | ⏳          | ⏳    |
+
+Table of Contents
+=================
+
+* [Authup Python Plugins](#authup-python-plugins)
+   * [Supported Python frameworks](#supported-python-frameworks)
+      * [Client](#client)
+      * [Server](#server)
+   * [Installation](#installation)
+      * [Extra dependencies](#extra-dependencies)
+   * [How to use](#how-to-use)
+      * [httpx](#httpx)
+      * [requests](#requests)
+      * [ASGI Middleware](#asgi-middleware)
+         * [Optional user injection](#optional-user-injection)
+      * [FastAPI Dependency](#fastapi-dependency)
+         * [Basic user dependency](#basic-user-dependency)
+         * [Require permissions](#require-permissions)
+   * [How to develop](#how-to-develop)
+      * [Install](#install)
+      * [Test](#test)
+
+
+## Installation
+
+The plugins are available via [PyPi](https://pypi.org/project/authup-py/).
+
+```bash
+pip install authup-py
+```
+
+### Extra dependencies
+The plugin for the project's base library [httpx](https://github.com/encode/httpx) needs no extra dependencies. To
+use the additional plugins for other libraries, you need to install with the corresponding extra i.e. for `requests`:
+
+```bash
+pip install authup-py[requests]
+```
+
+## How to use
+All the plugins share the underlying `Authup` class. The class is initialized with the url of the Authup server and
+the credentials you would like to use (username/password or robot_id/secret).    
+The class provides both sync and async methods for the different authentication and authorization flows.
+
+```python
+
+from authup import Authup
+
+authup = Authup(
+    url="https://authup.org",
+    username="username",
+    password="password"
+)
+
+authup_robot = Authup(
+    url="https://authup.org",
+    robot_id="robot",
+    robot_secret="secret"
+)
+
+```
+
+The following plugins all expect the same arguments as the `Authup` class with the addition of the
+app as a first argument for server side libraries (e.g. FastApi, Flask).
+
+### httpx
+For synchronously using the plugin with [httpx](https://github.com/encode/httpx) , you can use the `AuthupHttpx` class and pass an instance to your
+`httpx.Client` or a basic `httpx.Request` as the `auth` parameter:
+
+```python
+import httpx
+from authup.plugins.httpx import AuthupHttpx
+
+authup = AuthupHttpx(
+    url="https://authup.org",
+    username="username",
+    password="password",
+)
+
+# Use the authup instance as the auth parameter for the httpx client
+client = httpx.Client(auth=authup)
+
+with client:
+    response = client.get("https://authup.org")
+    print(response.status_code)
+
+
+# Use the authup instance as the auth parameter for a top level request function
+request = httpx.get("https://authup.org", auth=authup)
+
+```
+
+It works the same way for the asynchronous httpx client:
+
+```python
+import httpx
+from authup.plugins.httpx import AuthupHttpxAsync
+
+authup = AuthupHttpxAsync(
+    url="https://authup.org",
+    username="username",
+    password="password",
+)
+
+async with httpx.AsyncClient(auth=authup) as client:
+    response = await client.get("https://authup.org")
+    print(response.status_code)
+
+```
+
+### requests
+Since [requests](https://github.com/psf/requests) is a synchronous library, the plugin is also synchronous. You can use the `AuthupRequests` class and
+use it with the `requests.Session` or the `requests.request` functions:
+> **Note**
+> Requires the `requests` extra to be installed. `pip install authup-py[requests]`
+
+```python
+import requests
+from authup.plugins.requests import AuthupRequests
+
+authup = AuthupRequests(
+    url="https://authup.org",
+    username="username",
+    password="password",
+)
+
+# Use the authup instance as the auth parameter for the requests session
+with requests.Session() as session:
+    session.auth = authup
+    response = session.get("https://authup.org")
+    print(response.status_code)
+
+# Use the authup instance as the auth parameter for a top level request function
+response = requests.get("https://authup.org", auth=authup)
+print(response.status_code)
+
+```
+
+### ASGI Middleware
+
+The `AuthupASGIMiddleware` class can be used as an ASGI middleware for any ASGI framework (i.e. FastAPI, Starlette). 
+The middleware will check the incoming requests for a valid token and otherwise return a 401 response. If you pass the
+optional `user` parameter, the middleware will inject the user object into the request scope (`r.state.user`).
+
+The first argument is the ASGI application and the second argument is the URL of the authup instance.
+> **Note**
+> Requires the `asgi` extra to be installed. `pip install authup-py[asgi]`
+
+The following shows a simple example for using the middleware with a FastAPI application but it should work with any ASGI framework.
+
+> **Note**
+> Expects a running authup instance available at the given URL.
+> 
+```python
+from fastapi import FastAPI
+from authup.plugins.asgi import AuthupASGIMiddleware
+
+app = FastAPI()
+
+authup_url = "https://authup.org"  # change to your authup instance
+@app.get("/test")
+async def test():
+    return {"message": "Hello World"}
+
+# register the middleware pass the authup url as argument
+app.add_middleware(AuthupASGIMiddleware, authup_url=authup_url)
+
+```
+Now you can access the `/test` endpoint without a token and will receive a 401 response. When using a valid token, you will receive the expected response.
+
+```python
+import httpx
+from authup.plugins.httpx import AuthupHttpx
+
+# no token or invalid token raises 401
+response = httpx.get("http://localhost:8000/test") # 401
+print(response.status_code)
+
+# valid token receives the expected response
+authup = AuthupHttpx(
+    url="https://authup.org",
+    username="username",
+    password="password",
+)
+
+response = httpx.get("http://localhost:8000/test", auth=authup) # 200
+print(response.status_code)
+
+```
+
+#### Optional user injection
+Set the `user` parameter to `True` when adding the middleware to your ASGI application:
+
+```python
+from fastapi import FastAPI, Request
+from authup.plugins.asgi import AuthupASGIMiddleware
+
+app = FastAPI()
+
+authup_url = "https://authup.org"  # change to your authup instance
+@app.get("/test-user")
+async def test(request: Request):
+    return {"user": request.state.user}
+
+# register the middleware pass the authup url as argument
+app.add_middleware(AuthupASGIMiddleware, authup_url=authup_url, user=True)
+
+```
+
+Calling the `/test-user` endpoint without a token will return a 401 response. When using a valid token, the user object 
+will be injected into the request scope, and you will receive the expected response containing your user.
+
+### FastAPI Dependency
+The `AuthupUser` class can be used as a FastAPI dependency. 
+It will check the incoming requests for a valid token and otherwise return a 401 response. If the token is valid a user object
+will be available in the dependency call.
+
+#### Basic user dependency
+The following shows a simple example for using the dependency with a FastAPI application that will return the user
+object obtained from the token.
+
+```python
+from fastapi import FastAPI, Depends
+from authup.plugins.fastapi import AuthupUser
+from authup import User
+
+
+app = FastAPI()
+
+user_dependency = AuthupUser(url="http://localhost:3010")
+
+@app.get("/test")
+async def user_test(user: User = Depends(user_dependency)):
+    return {"user": user.dict()}
+
+```
+
+#### Require permissions
+You can also require specific permissions for the user. The following example will only allow users with the 
+`client_add` permission and a power level of over `100`. Otherwise, a 401 response will be returned.
+
+```python
+from fastapi import FastAPI, Depends
+from authup.plugins.fastapi import AuthupUser
+from authup import User
+from authup.permissions import Permission
+
+permissions = [
+        Permission(name="client_add", inverse=False, power=100),
+    ]
+
+required_permissions = AuthupUser(
+    url="http://localhost:3010",
+    permissions=permissions,
+)
+
+app = FastAPI()
+
+@app.get("/test")
+async def user_test(user: User = Depends(required_permissions)):
+    return {"user": user.dict()}
+
+```
+
+
+
+## How to develop
+
+### Install
+
+Requires [poetry](https://python-poetry.org/) and [pre-commit](https://pre-commit.com/) and python 3.7+.
+
+```shell
+poetry install --with dev --all-extras
+```
+
+Install pre-commit hooks
+
+```shell
+poetry run pre-commit install
+```
+
+### Test
+
+```shell
+poetry run pytest
+```
 
 
-setup(**setup_kwargs)
```

