# Comparing `tmp/flow_py_sdk_legacy-1.1.2.tar.gz` & `tmp/flow_py_sdk_legacy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_py_sdk_legacy-1.1.2.tar", max compression
+gzip compressed data, was "flow_py_sdk_legacy-1.1.3.tar", max compression
```

## Comparing `flow_py_sdk_legacy-1.1.2.tar` & `flow_py_sdk_legacy-1.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1075 2023-04-24 18:54:56.329377 flow_py_sdk_legacy-1.1.2/LICENSE
--rw-r--r--   0        0        0      970 2023-04-24 18:54:56.329377 flow_py_sdk_legacy-1.1.2/README.md
--rw-r--r--   0        0        0      505 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/__init__.py
--rw-r--r--   0        0        0     6482 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/account_key.py
--rw-r--r--   0        0        0     2001 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/__init__.py
--rw-r--r--   0        0        0     2116 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/address.py
--rw-r--r--   0        0        0     2160 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/composite.py
--rw-r--r--   0        0        0     1495 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/constants.py
--rw-r--r--   0        0        0     1507 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/decode.py
--rw-r--r--   0        0        0     1600 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/encode.py
--rw-r--r--   0        0        0     1125 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/kind.py
--rw-r--r--   0        0        0    10018 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/kinds.py
--rw-r--r--   0        0        0     7019 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/simple_kinds.py
--rw-r--r--   0        0        0    16642 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/types.py
--rw-r--r--   0        0        0     1131 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/value.py
--rw-r--r--   0        0        0       43 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/client/__init__.py
--rw-r--r--   0        0        0    18652 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/client/client.py
--rw-r--r--   0        0        0     9839 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/client/entities.py
--rw-r--r--   0        0        0      689 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/exceptions.py
--rw-r--r--   0        0        0       37 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/frlp/__init__.py
--rw-r--r--   0        0        0      108 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/frlp/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/__init__.py
--rw-r--r--   0        0        0    14122 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/access.py
--rw-r--r--   0        0        0     4000 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/entities.py
--rw-r--r--   0        0        0     4702 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/execution.py
--rw-r--r--   0        0        0     1384 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/script.py
--rw-r--r--   0        0        0      361 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/__init__.py
--rw-r--r--   0        0        0      804 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/hash_algo.py
--rw-r--r--   0        0        0     1393 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/in_memory_signer.py
--rw-r--r--   0        0        0     1060 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/in_memory_verifier.py
--rw-r--r--   0        0        0     1015 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/sign_algo.py
--rw-r--r--   0        0        0     2042 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/signer.py
--rw-r--r--   0        0        0     1803 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/verifier.py
--rw-r--r--   0        0        0     4164 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/templates.py
--rw-r--r--   0        0        0     8118 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/tx.py
--rw-r--r--   0        0        0       77 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1549 2023-04-24 18:54:56.333377 flow_py_sdk_legacy-1.1.2/flow_py_sdk/utils/verify_user_signature.py
--rw-r--r--   0        0        0      947 2023-04-24 18:55:42.277659 flow_py_sdk_legacy-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.1.2/setup.py
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-24 19:07:42.336444 flow_py_sdk_legacy-1.1.3/LICENSE
+-rw-r--r--   0        0        0      970 2023-04-24 19:07:42.336444 flow_py_sdk_legacy-1.1.3/README.md
+-rw-r--r--   0        0        0      505 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/__init__.py
+-rw-r--r--   0        0        0     6482 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/account_key.py
+-rw-r--r--   0        0        0     2001 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/__init__.py
+-rw-r--r--   0        0        0     2116 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/address.py
+-rw-r--r--   0        0        0     2160 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/composite.py
+-rw-r--r--   0        0        0     1495 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/constants.py
+-rw-r--r--   0        0        0     1507 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/decode.py
+-rw-r--r--   0        0        0     1600 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/encode.py
+-rw-r--r--   0        0        0     1125 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/kind.py
+-rw-r--r--   0        0        0    10018 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/kinds.py
+-rw-r--r--   0        0        0     7019 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/simple_kinds.py
+-rw-r--r--   0        0        0    16642 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/types.py
+-rw-r--r--   0        0        0     1131 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/value.py
+-rw-r--r--   0        0        0       43 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/client/__init__.py
+-rw-r--r--   0        0        0    18652 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/client/client.py
+-rw-r--r--   0        0        0     9839 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/client/entities.py
+-rw-r--r--   0        0        0      689 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/exceptions.py
+-rw-r--r--   0        0        0       37 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/frlp/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/frlp/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/__init__.py
+-rw-r--r--   0        0        0    14122 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/access.py
+-rw-r--r--   0        0        0     4000 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/entities.py
+-rw-r--r--   0        0        0     4702 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/execution.py
+-rw-r--r--   0        0        0     1384 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/script.py
+-rw-r--r--   0        0        0      361 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/hash_algo.py
+-rw-r--r--   0        0        0     1393 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/in_memory_signer.py
+-rw-r--r--   0        0        0     1060 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/in_memory_verifier.py
+-rw-r--r--   0        0        0     1015 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/sign_algo.py
+-rw-r--r--   0        0        0     2042 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/signer.py
+-rw-r--r--   0        0        0     1803 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/verifier.py
+-rw-r--r--   0        0        0     4164 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/templates.py
+-rw-r--r--   0        0        0     8118 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/tx.py
+-rw-r--r--   0        0        0       77 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1549 2023-04-24 19:07:42.340444 flow_py_sdk_legacy-1.1.3/flow_py_sdk/utils/verify_user_signature.py
+-rw-r--r--   0        0        0      947 2023-04-24 19:08:33.616788 flow_py_sdk_legacy-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.1.3/setup.py
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.1.3/PKG-INFO
```

### Comparing `flow_py_sdk_legacy-1.1.2/LICENSE` & `flow_py_sdk_legacy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/README.md` & `flow_py_sdk_legacy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/account_key.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/account_key.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/__init__.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/address.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/address.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/composite.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/composite.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/constants.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/constants.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/decode.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/decode.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/encode.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/encode.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/kind.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/kind.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/kinds.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/kinds.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/simple_kinds.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/simple_kinds.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/types.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/types.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/cadence/value.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/cadence/value.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/client/client.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/client/client.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/client/entities.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/client/entities.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/exceptions.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/access.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/access.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/entities.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/entities.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/proto/flow/execution.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/proto/flow/execution.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/script.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/script.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/hash_algo.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/hash_algo.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/in_memory_signer.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/in_memory_signer.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/in_memory_verifier.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/in_memory_verifier.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/sign_algo.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/sign_algo.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/signer.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/signer.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/signer/verifier.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/signer/verifier.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/templates.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/templates.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/tx.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/tx.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/flow_py_sdk/utils/verify_user_signature.py` & `flow_py_sdk_legacy-1.1.3/flow_py_sdk/utils/verify_user_signature.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.1.2/pyproject.toml` & `flow_py_sdk_legacy-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "flow-py-sdk-legacy"
-version = "1.1.2"
+version = "1.1.3"
 description = "A python SDK for the flow blockchain"
 authors = ["Janez Podhostnik <janez.podhostnik@gmail.com>", "justin.kc.herrera@gmail.com"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/justinnout/flow-py-sdk"
 packages = [
     { include = "flow_py_sdk" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 betterproto = {extras = ["compiler"], version = "v2.0.0-beta5"}
 grpcio-tools = "^1.49.1"
 ecdsa = "^v0.15"
-rlp = "^1.2.0"
+rlp = "^3.0.0"
 grpclib = "^0.4"
 
 [tool.poetry.dev-dependencies]
 coloredlogs = "^15.0"
 toml = "^0.10"
 black = "^23.1"
 pytest = "^7.2"
```

### Comparing `flow_py_sdk_legacy-1.1.2/setup.py` & `flow_py_sdk_legacy-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 {'': ['*']}
 
 install_requires = \
 ['betterproto[compiler]==v2.0.0-beta5',
  'ecdsa>=v0.15,<0.16',
  'grpcio-tools>=1.49.1,<2.0.0',
  'grpclib>=0.4,<0.5',
- 'rlp>=1.2.0,<2.0.0']
+ 'rlp>=3.0.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['examples = examples.main:run']}
 
 setup_kwargs = {
     'name': 'flow-py-sdk-legacy',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'A python SDK for the flow blockchain',
     'long_description': 'The Flow Python SDK provides a set of packages for Python developers to build applications that interact with the Flow network.\n\n[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)\n[![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)\n\n\nSee the [guide](https://janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)!\n\n\nNote: This SDK is also fully compatible with the Flow Emulator and can be used for local development.\n\n## Installing\n\nTo start using the SDK, install Python 3.7 or higher and install package:\n\n```sh\npip install flow-py-sdk-legacy\n```\n\nor if using poetry:\n\n```sh\npoetry add flow-py-sdk-legacy\n```\n\n## Contributors\n\n<a href="https://github.com/justinnout/flow-py-sdk/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=justinnout/flow-py-sdk" />\n</a>\n\nMade with [contrib.rocks](https://contrib.rocks).',
     'author': 'Janez Podhostnik',
     'author_email': 'janez.podhostnik@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/justinnout/flow-py-sdk',
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['flow_py_sdk', 'flow_py_sdk.cadence', 'flow_py_sdk.client',
 'flow_py_sdk.frlp', 'flow_py_sdk.proto', 'flow_py_sdk.proto.flow',
 'flow_py_sdk.signer', 'flow_py_sdk.utils'] package_data = \ {'': ['*']}
 install_requires = \ ['betterproto[compiler]==v2.0.0-beta5',
 'ecdsa>=v0.15,<0.16', 'grpcio-tools>=1.49.1,<2.0.0', 'grpclib>=0.4,<0.5',
-'rlp>=1.2.0,<2.0.0'] entry_points = \ {'console_scripts': ['examples =
+'rlp>=3.0.0,<4.0.0'] entry_points = \ {'console_scripts': ['examples =
 examples.main:run']} setup_kwargs = { 'name': 'flow-py-sdk-legacy', 'version':
-'1.1.2', 'description': 'A python SDK for the flow blockchain',
+'1.1.3', 'description': 'A python SDK for the flow blockchain',
 'long_description': 'The Flow Python SDK provides a set of packages for Python
 developers to build applications that interact with the Flow network.\n\n[!
 [PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/
 project/flow-py-sdk-legacy/)\n[![codecov](https://codecov.io/gh/justinnout/
 flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/
 example-go)\n\n\nSee the [guide](https://janezpodhostnik.github.io/flow-py-sdk/
 python_SDK_guide/)!\n\n\nNote: This SDK is also fully compatible with the Flow
```

### Comparing `flow_py_sdk_legacy-1.1.2/PKG-INFO` & `flow_py_sdk_legacy-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow-py-sdk-legacy
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python SDK for the flow blockchain
 Home-page: https://github.com/justinnout/flow-py-sdk
 License: MIT
 Author: Janez Podhostnik
 Author-email: janez.podhostnik@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: betterproto[compiler] (==v2.0.0-beta5)
 Requires-Dist: ecdsa (>=v0.15,<0.16)
 Requires-Dist: grpcio-tools (>=1.49.1,<2.0.0)
 Requires-Dist: grpclib (>=0.4,<0.5)
-Requires-Dist: rlp (>=1.2.0,<2.0.0)
+Requires-Dist: rlp (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/justinnout/flow-py-sdk
 Description-Content-Type: text/markdown
 
 The Flow Python SDK provides a set of packages for Python developers to build applications that interact with the Flow network.
 
 [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)
 [![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: flow-py-sdk-legacy Version: 1.1.2 Summary: A python
+Metadata-Version: 2.1 Name: flow-py-sdk-legacy Version: 1.1.3 Summary: A python
 SDK for the flow blockchain Home-page: https://github.com/justinnout/flow-py-
 sdk License: MIT Author: Janez Podhostnik Author-email:
 janez.podhostnik@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: betterproto[compiler] (==v2.0.0-
 beta5) Requires-Dist: ecdsa (>=v0.15,<0.16) Requires-Dist: grpcio-tools
 (>=1.49.1,<2.0.0) Requires-Dist: grpclib (>=0.4,<0.5) Requires-Dist: rlp
-(>=1.2.0,<2.0.0) Project-URL: Repository, https://github.com/justinnout/flow-
+(>=3.0.0,<4.0.0) Project-URL: Repository, https://github.com/justinnout/flow-
 py-sdk Description-Content-Type: text/markdown The Flow Python SDK provides a
 set of packages for Python developers to build applications that interact with
 the Flow network. [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-
 legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/) [![codecov](https://
 codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://
 codecov.io/gh/codecov/example-go) See the [guide](https://
 janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)! Note: This SDK is
```

