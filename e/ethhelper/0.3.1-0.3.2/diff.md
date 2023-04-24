# Comparing `tmp/ethhelper-0.3.1.tar.gz` & `tmp/ethhelper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethhelper-0.3.1.tar", max compression
+gzip compressed data, was "ethhelper-0.3.2.tar", max compression
```

## Comparing `ethhelper-0.3.1.tar` & `ethhelper-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-02-22 06:21:08.469634 ethhelper-0.3.1/LICENSE
--rw-r--r--   0        0        0     1280 2023-04-24 03:32:04.787997 ethhelper-0.3.1/README.md
--rw-r--r--   0        0        0     2137 2023-04-24 03:31:50.117968 ethhelper-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-23 08:08:41.740510 ethhelper-0.3.1/src/ethhelper/__init__.py
--rw-r--r--   0        0        0        0 2023-02-14 13:51:41.412513 ethhelper-0.3.1/src/ethhelper/connectors/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-23 08:02:20.007096 ethhelper-0.3.1/src/ethhelper/connectors/http/__init__.py
--rw-r--r--   0        0        0    13216 2023-04-23 05:49:16.346488 ethhelper-0.3.1/src/ethhelper/connectors/http/base.py
--rw-r--r--   0        0        0     7712 2023-04-23 05:51:14.599405 ethhelper-0.3.1/src/ethhelper/connectors/http/custom.py
--rw-r--r--   0        0        0    16281 2023-04-23 05:50:47.138676 ethhelper-0.3.1/src/ethhelper/connectors/http/eth.py
--rw-r--r--   0        0        0     1743 2023-04-23 05:51:00.189376 ethhelper-0.3.1/src/ethhelper/connectors/http/net.py
--rw-r--r--   0        0        0     3958 2023-04-23 05:28:50.118285 ethhelper-0.3.1/src/ethhelper/connectors/http/txpool.py
--rw-r--r--   0        0        0      159 2023-04-23 08:08:31.740563 ethhelper-0.3.1/src/ethhelper/connectors/ws/__init__.py
--rw-r--r--   0        0        0     5912 2023-04-23 05:48:37.045672 ethhelper-0.3.1/src/ethhelper/connectors/ws/base.py
--rw-r--r--   0        0        0     3505 2023-04-23 05:47:56.614878 ethhelper-0.3.1/src/ethhelper/connectors/ws/block.py
--rw-r--r--   0        0        0        0 2023-02-08 04:03:22.125975 ethhelper-0.3.1/src/ethhelper/datatypes/__init__.py
--rw-r--r--   0        0        0     7579 2023-04-23 06:13:59.638551 ethhelper-0.3.1/src/ethhelper/datatypes/base.py
--rw-r--r--   0        0        0    17501 2023-04-23 07:48:07.619936 ethhelper-0.3.1/src/ethhelper/datatypes/eth.py
--rw-r--r--   0        0        0     6824 2023-04-23 06:24:13.116631 ethhelper-0.3.1/src/ethhelper/datatypes/geth.py
--rw-r--r--   0        0        0     5135 2023-04-23 06:30:46.869030 ethhelper-0.3.1/src/ethhelper/datatypes/txpool.py
--rw-r--r--   0        0        0        0 2023-02-22 06:46:40.501121 ethhelper-0.3.1/src/ethhelper/py.typed
--rw-r--r--   0        0        0     1387 2023-04-23 08:27:20.706292 ethhelper-0.3.1/src/ethhelper/types.py
--rw-r--r--   0        0        0        0 2023-02-08 04:03:29.665985 ethhelper-0.3.1/src/ethhelper/utils/__init__.py
--rw-r--r--   0        0        0      927 2023-03-10 07:48:53.666281 ethhelper-0.3.1/src/ethhelper/utils/convert.py
--rw-r--r--   0        0        0      498 2023-03-02 06:44:48.060205 ethhelper-0.3.1/src/ethhelper/utils/json.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 ethhelper-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 03:45:33.880786 ethhelper-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1280 2023-04-24 03:45:33.880786 ethhelper-0.3.2/README.md
+-rw-r--r--   0        0        0     2137 2023-04-24 03:45:33.880786 ethhelper-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-24 03:45:33.880786 ethhelper-0.3.2/src/ethhelper/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:45:33.880786 ethhelper-0.3.2/src/ethhelper/connectors/__init__.py
+-rw-r--r--   0        0        0     1565 2023-04-24 03:45:33.880786 ethhelper-0.3.2/src/ethhelper/connectors/http/__init__.py
+-rw-r--r--   0        0        0    13216 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/base.py
+-rw-r--r--   0        0        0     7712 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/custom.py
+-rw-r--r--   0        0        0    16281 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/eth.py
+-rw-r--r--   0        0        0     1743 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/net.py
+-rw-r--r--   0        0        0     3958 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/http/txpool.py
+-rw-r--r--   0        0        0      159 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/ws/__init__.py
+-rw-r--r--   0        0        0     5912 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/ws/base.py
+-rw-r--r--   0        0        0     3505 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/connectors/ws/block.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/__init__.py
+-rw-r--r--   0        0        0     7579 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/base.py
+-rw-r--r--   0        0        0    17501 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/eth.py
+-rw-r--r--   0        0        0     6824 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/geth.py
+-rw-r--r--   0        0        0     5135 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/datatypes/txpool.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/py.typed
+-rw-r--r--   0        0        0     1387 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/types.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/utils/convert.py
+-rw-r--r--   0        0        0      498 2023-04-24 03:45:33.884786 ethhelper-0.3.2/src/ethhelper/utils/json.py
+-rw-r--r--   0        0        0     2419 1970-01-01 00:00:00.000000 ethhelper-0.3.2/setup.py
+-rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 ethhelper-0.3.2/PKG-INFO
```

### Comparing `ethhelper-0.3.1/LICENSE` & `ethhelper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/README.md` & `ethhelper-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/pyproject.toml` & `ethhelper-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ethhelper"
-version = "0.3.1"
+version = "0.3.2"
 description = "Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic."
 authors = ["XiaoHuiHui233 <1025184872@qq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/XiaoHuiHui233/ETHHelper"
 keywords = ["ethereum", "asyncio", "geth", "pydantic"]
```

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/http/__init__.py` & `ethhelper-0.3.2/src/ethhelper/connectors/http/__init__.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/http/base.py` & `ethhelper-0.3.2/src/ethhelper/connectors/http/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/http/custom.py` & `ethhelper-0.3.2/src/ethhelper/connectors/http/custom.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/http/eth.py` & `ethhelper-0.3.2/src/ethhelper/connectors/http/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/http/net.py` & `ethhelper-0.3.2/src/ethhelper/connectors/http/net.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/http/txpool.py` & `ethhelper-0.3.2/src/ethhelper/connectors/http/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/ws/base.py` & `ethhelper-0.3.2/src/ethhelper/connectors/ws/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/connectors/ws/block.py` & `ethhelper-0.3.2/src/ethhelper/connectors/ws/block.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/datatypes/base.py` & `ethhelper-0.3.2/src/ethhelper/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/datatypes/eth.py` & `ethhelper-0.3.2/src/ethhelper/datatypes/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/datatypes/geth.py` & `ethhelper-0.3.2/src/ethhelper/datatypes/geth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/datatypes/txpool.py` & `ethhelper-0.3.2/src/ethhelper/datatypes/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/types.py` & `ethhelper-0.3.2/src/ethhelper/types.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/src/ethhelper/utils/convert.py` & `ethhelper-0.3.2/src/ethhelper/utils/convert.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.1/PKG-INFO` & `ethhelper-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethhelper
-Version: 0.3.1
+Version: 0.3.2
 Summary: Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 Home-page: https://github.com/XiaoHuiHui233/ETHHelper
 License: Apache-2.0
 Keywords: ethereum,asyncio,geth,pydantic
 Author: XiaoHuiHui233
 Author-email: 1025184872@qq.com
 Requires-Python: >=3.10,<4.0
```

