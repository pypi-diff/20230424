# Comparing `tmp/ethhelper-0.3.2.tar.gz` & `tmp/ethhelper-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethhelper-0.3.2.tar", max compression
+gzip compressed data, was "ethhelper-0.3.3.tar", max compression
```

## Comparing `ethhelper-0.3.2.tar` & `ethhelper-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-04-24 03:45:33.880786 ethhelper-0.3.2/LICENSE
--rw-r--r--   0        0        0     1280 2023-04-24 03:45:33.880786 ethhelper-0.3.2/README.md
--rw-r--r--   0        0        0     2137 2023-04-24 03:45:33.880786 ethhelper-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-24 03:45:33.880786 ethhelper-0.3.2/src/ethhelper/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 03:45:33.880786 ethhelper-0.3.2/src/ethhelper/connectors/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-24 03:45:33.880786 ethhelper-0.3.2/src/ethhelper/connectors/http/__init__.py
--rw-r--r--   0        0        0    13216 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/base.py
--rw-r--r--   0        0        0     7712 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/custom.py
--rw-r--r--   0        0        0    16281 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/eth.py
--rw-r--r--   0        0        0     1743 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/net.py
--rw-r--r--   0        0        0     3958 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/txpool.py
--rw-r--r--   0        0        0      159 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/ws/__init__.py
--rw-r--r--   0        0        0     5912 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/ws/base.py
--rw-r--r--   0        0        0     3505 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/ws/block.py
--rw-r--r--   0        0        0        0 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/__init__.py
--rw-r--r--   0        0        0     7579 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/base.py
--rw-r--r--   0        0        0    17501 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/eth.py
--rw-r--r--   0        0        0     6824 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/geth.py
--rw-r--r--   0        0        0     5135 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/txpool.py
--rw-r--r--   0        0        0        0 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/py.typed
--rw-r--r--   0        0        0     1387 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/types.py
--rw-r--r--   0        0        0        0 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/utils/__init__.py
--rw-r--r--   0        0        0      927 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/utils/convert.py
--rw-r--r--   0        0        0      498 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/utils/json.py
--rw-r--r--   0        0        0     2419 1970-01-01 00:00:00.000000 ethhelper-0.3.2/setup.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 ethhelper-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 04:03:12.106765 ethhelper-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-24 04:03:12.106765 ethhelper-0.3.3/README.md
+-rw-r--r--   0        0        0     2137 2023-04-24 04:03:12.110765 ethhelper-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/__init__.py
+-rw-r--r--   0        0        0     1565 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/http/__init__.py
+-rw-r--r--   0        0        0    13216 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/http/base.py
+-rw-r--r--   0        0        0     7712 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/http/custom.py
+-rw-r--r--   0        0        0    16281 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/http/eth.py
+-rw-r--r--   0        0        0     1743 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/http/net.py
+-rw-r--r--   0        0        0     3958 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/http/txpool.py
+-rw-r--r--   0        0        0      159 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/ws/__init__.py
+-rw-r--r--   0        0        0     5912 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/ws/base.py
+-rw-r--r--   0        0        0     3505 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/connectors/ws/block.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/datatypes/__init__.py
+-rw-r--r--   0        0        0     7579 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/datatypes/base.py
+-rw-r--r--   0        0        0    17501 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/datatypes/eth.py
+-rw-r--r--   0        0        0     6824 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/datatypes/geth.py
+-rw-r--r--   0        0        0     5135 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/datatypes/txpool.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/py.typed
+-rw-r--r--   0        0        0     1387 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/types.py
+-rw-r--r--   0        0        0        0 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/utils/convert.py
+-rw-r--r--   0        0        0      498 2023-04-24 04:03:12.110765 ethhelper-0.3.3/src/ethhelper/utils/json.py
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 ethhelper-0.3.3/setup.py
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 ethhelper-0.3.3/PKG-INFO
```

### Comparing `ethhelper-0.3.2/LICENSE` & `ethhelper-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/README.md` & `ethhelper-0.3.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # ETHHelper
 
-[![license](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)]
 [![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)
+[![Python Version](https://img.shields.io/pypi/pyversions/ethhelper)]
+[![Wheel Status](https://img.shields.io/pypi/wheel/ethhelper)]
+[![Latest Version](https://img.shields.io/github/v/release/XiaoHuiHui233/ETHHelper)]
+[![License](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)
 
 Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 
 Quickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).
 
 [中文](docs/README_cn.md) | English
```

### Comparing `ethhelper-0.3.2/pyproject.toml` & `ethhelper-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ethhelper"
-version = "0.3.2"
+version = "0.3.3"
 description = "Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic."
 authors = ["XiaoHuiHui233 <1025184872@qq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/XiaoHuiHui233/ETHHelper"
 keywords = ["ethereum", "asyncio", "geth", "pydantic"]
```

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/http/__init__.py` & `ethhelper-0.3.3/src/ethhelper/connectors/http/__init__.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/http/base.py` & `ethhelper-0.3.3/src/ethhelper/connectors/http/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/http/custom.py` & `ethhelper-0.3.3/src/ethhelper/connectors/http/custom.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/http/eth.py` & `ethhelper-0.3.3/src/ethhelper/connectors/http/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/http/net.py` & `ethhelper-0.3.3/src/ethhelper/connectors/http/net.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/http/txpool.py` & `ethhelper-0.3.3/src/ethhelper/connectors/http/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/ws/base.py` & `ethhelper-0.3.3/src/ethhelper/connectors/ws/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/connectors/ws/block.py` & `ethhelper-0.3.3/src/ethhelper/connectors/ws/block.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/datatypes/base.py` & `ethhelper-0.3.3/src/ethhelper/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/datatypes/eth.py` & `ethhelper-0.3.3/src/ethhelper/datatypes/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/datatypes/geth.py` & `ethhelper-0.3.3/src/ethhelper/datatypes/geth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/datatypes/txpool.py` & `ethhelper-0.3.3/src/ethhelper/datatypes/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/types.py` & `ethhelper-0.3.3/src/ethhelper/types.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/src/ethhelper/utils/convert.py` & `ethhelper-0.3.3/src/ethhelper/utils/convert.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.2/setup.py` & `ethhelper-0.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'orjson>=3.8.10,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'web3>=6.2.0,<7.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'ethhelper',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.',
-    'long_description': "# ETHHelper\n\n[![license](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)\n\nAsynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.\n\nQuickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).\n\n[中文](docs/README_cn.md) | English\n\n## Usage\n\n### pypi\n\nIf you prefer to use pypi to install this package, you can just run the following command:\n\n```bash\npip install ethhelper\n```\n\n### git\n\nThe project is managed by poetry. If you prefer to use git to install this package, you can use poetry to directly add a reference to the project's build package through git.\n\nThe command is as follow:\n\n```bash\npoetry add git+ssh://git@github.com:XiaoHuiHui233/ETHHelper.git\n```\n\n## Build\n\nYou can use poetry's tools to generate a build of this project (pure Python).\n\nThe command is as follow:\n\n```bash\npoetry build\n```\n\n## Author and License\n\nETHHelper was written by [XiaoHuiHui233](https://github.com/XiaoHuiHui233/), licensed under the Apache 2.0.\n",
+    'long_description': "# ETHHelper\n\n[![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)]\n[![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)\n[![Python Version](https://img.shields.io/pypi/pyversions/ethhelper)]\n[![Wheel Status](https://img.shields.io/pypi/wheel/ethhelper)]\n[![Latest Version](https://img.shields.io/github/v/release/XiaoHuiHui233/ETHHelper)]\n[![License](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)\n\nAsynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.\n\nQuickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).\n\n[中文](docs/README_cn.md) | English\n\n## Usage\n\n### pypi\n\nIf you prefer to use pypi to install this package, you can just run the following command:\n\n```bash\npip install ethhelper\n```\n\n### git\n\nThe project is managed by poetry. If you prefer to use git to install this package, you can use poetry to directly add a reference to the project's build package through git.\n\nThe command is as follow:\n\n```bash\npoetry add git+ssh://git@github.com:XiaoHuiHui233/ETHHelper.git\n```\n\n## Build\n\nYou can use poetry's tools to generate a build of this project (pure Python).\n\nThe command is as follow:\n\n```bash\npoetry build\n```\n\n## Author and License\n\nETHHelper was written by [XiaoHuiHui233](https://github.com/XiaoHuiHui233/), licensed under the Apache 2.0.\n",
     'author': 'XiaoHuiHui233',
     'author_email': '1025184872@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/XiaoHuiHui233/ETHHelper',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `ethhelper-0.3.2/PKG-INFO` & `ethhelper-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethhelper
-Version: 0.3.2
+Version: 0.3.3
 Summary: Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 Home-page: https://github.com/XiaoHuiHui233/ETHHelper
 License: Apache-2.0
 Keywords: ethereum,asyncio,geth,pydantic
 Author: XiaoHuiHui233
 Author-email: 1025184872@qq.com
 Requires-Python: >=3.10,<4.0
@@ -19,16 +19,20 @@
 Requires-Dist: web3 (>=6.2.0,<7.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Repository, https://github.com/XiaoHuiHui233/ETHHelper
 Description-Content-Type: text/markdown
 
 # ETHHelper
 
-[![license](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)]
 [![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)
+[![Python Version](https://img.shields.io/pypi/pyversions/ethhelper)]
+[![Wheel Status](https://img.shields.io/pypi/wheel/ethhelper)]
+[![Latest Version](https://img.shields.io/github/v/release/XiaoHuiHui233/ETHHelper)]
+[![License](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)
 
 Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 
 Quickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).
 
 [中文](docs/README_cn.md) | English
```

