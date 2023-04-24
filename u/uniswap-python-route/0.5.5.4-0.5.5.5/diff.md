# Comparing `tmp/uniswap_python_route-0.5.5.4.tar.gz` & `tmp/uniswap_python_route-0.5.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswap_python_route-0.5.5.4.tar", max compression
+gzip compressed data, was "uniswap_python_route-0.5.5.5.tar", max compression
```

## Comparing `uniswap_python_route-0.5.5.4.tar` & `uniswap_python_route-0.5.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1080 2023-04-10 21:36:25.290516 uniswap_python_route-0.5.5.4/LICENSE
--rw-r--r--   0        0        0     5504 2023-04-10 21:36:25.290726 uniswap_python_route-0.5.5.4/README.md
--rw-r--r--   0        0        0     1253 2023-04-10 21:50:16.950222 uniswap_python_route-0.5.5.4/pyproject.toml
--rw-r--r--   0        0        0       90 2023-04-10 21:36:25.293632 uniswap_python_route-0.5.5.4/uniswap/__init__.py
--rw-r--r--   0        0        0     4376 2023-04-10 21:36:25.293775 uniswap_python_route-0.5.5.4/uniswap/assets/erc20.abi
--rw-r--r--   0        0        0     4378 2023-04-10 21:36:25.293849 uniswap_python_route-0.5.5.4/uniswap/assets/erc20b32.abi
--rw-r--r--   0        0        0    17154 2023-04-10 21:36:25.294013 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v1/exchange.abi
--rw-r--r--   0        0        0     1761 2023-04-10 21:36:25.294112 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v1/factory.abi
--rw-r--r--   0        0        0     3347 2023-04-10 21:36:25.294254 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v2/factory.abi
--rw-r--r--   0        0        0    15309 2023-04-10 21:36:25.294360 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v2/router02.abi
--rw-r--r--   0        0        0     4418 2023-04-10 21:36:25.294456 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/factory.abi
--rw-r--r--   0        0        0    19609 2023-04-10 21:36:25.294552 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/pool.abi
--rw-r--r--   0        0        0     2988 2023-04-10 21:36:25.294658 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/quoter.abi
--rw-r--r--   0        0        0     9265 2023-04-10 21:36:25.294728 uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/router.abi
--rw-r--r--   0        0        0     3229 2023-04-10 21:36:25.294817 uniswap_python_route-0.5.5.4/uniswap/cli.py
--rw-r--r--   0        0        0     2242 2023-04-10 21:36:25.294892 uniswap_python_route-0.5.5.4/uniswap/constants.py
--rw-r--r--   0        0        0     1760 2023-04-10 21:36:25.294970 uniswap_python_route-0.5.5.4/uniswap/decorators.py
--rw-r--r--   0        0        0      489 2023-04-10 21:36:25.295049 uniswap_python_route-0.5.5.4/uniswap/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-10 21:36:25.295079 uniswap_python_route-0.5.5.4/uniswap/py.typed
--rw-r--r--   0        0        0      677 2023-04-10 21:36:25.295156 uniswap_python_route-0.5.5.4/uniswap/token.py
--rw-r--r--   0        0        0      922 2023-04-10 21:36:25.295224 uniswap_python_route-0.5.5.4/uniswap/tokens.py
--rw-r--r--   0        0        0      165 2023-04-10 21:36:25.295303 uniswap_python_route-0.5.5.4/uniswap/types.py
--rw-r--r--   0        0        0    56200 2023-04-10 21:49:02.655830 uniswap_python_route-0.5.5.4/uniswap/uniswap.py
--rw-r--r--   0        0        0     1893 2023-04-10 21:36:25.295609 uniswap_python_route-0.5.5.4/uniswap/util.py
--rw-r--r--   0        0        0     6666 1970-01-01 00:00:00.000000 uniswap_python_route-0.5.5.4/setup.py
--rw-r--r--   0        0        0     6615 1970-01-01 00:00:00.000000 uniswap_python_route-0.5.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-10 21:36:25.290516 uniswap_python_route-0.5.5.5/LICENSE
+-rw-r--r--   0        0        0     5504 2023-04-10 21:36:25.290726 uniswap_python_route-0.5.5.5/README.md
+-rw-r--r--   0        0        0     1253 2023-04-24 20:23:54.164872 uniswap_python_route-0.5.5.5/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-04-10 21:36:25.293632 uniswap_python_route-0.5.5.5/uniswap/__init__.py
+-rw-r--r--   0        0        0     4376 2023-04-10 21:36:25.293775 uniswap_python_route-0.5.5.5/uniswap/assets/erc20.abi
+-rw-r--r--   0        0        0     4378 2023-04-10 21:36:25.293849 uniswap_python_route-0.5.5.5/uniswap/assets/erc20b32.abi
+-rw-r--r--   0        0        0    17154 2023-04-10 21:36:25.294013 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v1/exchange.abi
+-rw-r--r--   0        0        0     1761 2023-04-10 21:36:25.294112 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v1/factory.abi
+-rw-r--r--   0        0        0     3347 2023-04-10 21:36:25.294254 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v2/factory.abi
+-rw-r--r--   0        0        0    15309 2023-04-10 21:36:25.294360 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v2/router02.abi
+-rw-r--r--   0        0        0     4418 2023-04-10 21:36:25.294456 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/factory.abi
+-rw-r--r--   0        0        0    19609 2023-04-10 21:36:25.294552 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/pool.abi
+-rw-r--r--   0        0        0     2988 2023-04-10 21:36:25.294658 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/quoter.abi
+-rw-r--r--   0        0        0     9265 2023-04-10 21:36:25.294728 uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/router.abi
+-rw-r--r--   0        0        0     3229 2023-04-10 21:36:25.294817 uniswap_python_route-0.5.5.5/uniswap/cli.py
+-rw-r--r--   0        0        0     2242 2023-04-10 21:36:25.294892 uniswap_python_route-0.5.5.5/uniswap/constants.py
+-rw-r--r--   0        0        0     1760 2023-04-10 21:36:25.294970 uniswap_python_route-0.5.5.5/uniswap/decorators.py
+-rw-r--r--   0        0        0      489 2023-04-10 21:36:25.295049 uniswap_python_route-0.5.5.5/uniswap/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-10 21:36:25.295079 uniswap_python_route-0.5.5.5/uniswap/py.typed
+-rw-r--r--   0        0        0      677 2023-04-10 21:36:25.295156 uniswap_python_route-0.5.5.5/uniswap/token.py
+-rw-r--r--   0        0        0      922 2023-04-10 21:36:25.295224 uniswap_python_route-0.5.5.5/uniswap/tokens.py
+-rw-r--r--   0        0        0      165 2023-04-10 21:36:25.295303 uniswap_python_route-0.5.5.5/uniswap/types.py
+-rw-r--r--   0        0        0    56428 2023-04-24 20:22:29.685122 uniswap_python_route-0.5.5.5/uniswap/uniswap.py
+-rw-r--r--   0        0        0     1893 2023-04-10 21:36:25.295609 uniswap_python_route-0.5.5.5/uniswap/util.py
+-rw-r--r--   0        0        0     6666 1970-01-01 00:00:00.000000 uniswap_python_route-0.5.5.5/setup.py
+-rw-r--r--   0        0        0     6615 1970-01-01 00:00:00.000000 uniswap_python_route-0.5.5.5/PKG-INFO
```

### Comparing `uniswap_python_route-0.5.5.4/LICENSE` & `uniswap_python_route-0.5.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/README.md` & `uniswap_python_route-0.5.5.5/README.md`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/pyproject.toml` & `uniswap_python_route-0.5.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniswap-python-route"
-version = "0.5.5.4"
+version = "0.5.5.5"
 description = "An unofficial Python wrapper for the decentralized exchange Uniswap"
 repository = "https://github.com/starascendin/uniswap-python"
 readme = "README.md"
 keywords = ["uniswap", "ethereum", "exchange", "trading"]
 authors = ["Shane Fontaine <shane6fontaine@gmail.com>", "Erik Bjäreholt <erik@bjareho.lt>"]
 license = "MIT"
 packages = [
```

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/erc20.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/erc20.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/erc20b32.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/erc20b32.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v1/exchange.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v1/exchange.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v1/factory.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v1/factory.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v2/factory.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v2/factory.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v2/router02.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v2/router02.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/factory.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/factory.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/pool.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/pool.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/quoter.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/quoter.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/assets/uniswap-v3/router.abi` & `uniswap_python_route-0.5.5.5/uniswap/assets/uniswap-v3/router.abi`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/cli.py` & `uniswap_python_route-0.5.5.5/uniswap/cli.py`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/constants.py` & `uniswap_python_route-0.5.5.5/uniswap/constants.py`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/decorators.py` & `uniswap_python_route-0.5.5.5/uniswap/decorators.py`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/token.py` & `uniswap_python_route-0.5.5.5/uniswap/token.py`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/tokens.py` & `uniswap_python_route-0.5.5.5/uniswap/tokens.py`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/uniswap/uniswap.py` & `uniswap_python_route-0.5.5.5/uniswap/uniswap.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,14 +686,21 @@
             if not recipient:
                 function = token_funcs.tokenToTokenSwapInput(*func_params)
             else:
                 func_params.insert(len(func_params) - 1, recipient)
                 function = token_funcs.tokenToTokenTransferInput(*func_params)
             return self._build_and_send_tx(function)
         elif self.version == 2:
+            # BL: if route is non, set route to TOKEN0 TOKEN1.
+            path_route = None
+            if route is None:
+                path_route = [input_token, output_token]
+            
+            path_route = [input_token, output_token] if route is None else route
+            
             min_tokens_bought = int(
                 (1 - slippage)
                 * self._get_token_token_input_price(
                     input_token, output_token, qty, fee=fee, route=route
                 )
             )
             if fee_on_transfer:
@@ -706,26 +713,26 @@
             camelot_dex_arbitrum_router_addr = "0xc873fEcbd354f5A56E00E710B90EF4201db2448d"
             if self.router.address == camelot_dex_arbitrum_router_addr:
                 logger.info("Using CamelotDex Arbitrum Router....")
                 return self._build_and_send_tx(
                     func(
                         qty,
                         min_tokens_bought,
-                        [input_token, output_token],
+                        path_route,
                         recipient,
                         '0x0000000000000000000000000000000000000000',
                         self._deadline(),
                     ),
                 )
             
             return self._build_and_send_tx(
                 func(
                     qty,
                     min_tokens_bought,
-                    [input_token, self.get_weth_address(), output_token],
+                    path_route,
                     recipient,
                     self._deadline(),
                 ),
             )
         elif self.version == 3:
             if fee_on_transfer:
                 raise Exception("fee on transfer not supported by Uniswap v3")
```

### Comparing `uniswap_python_route-0.5.5.4/uniswap/util.py` & `uniswap_python_route-0.5.5.5/uniswap/util.py`

 * *Files identical despite different names*

### Comparing `uniswap_python_route-0.5.5.4/setup.py` & `uniswap_python_route-0.5.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ['click>=8.0.3,<9.0.0', 'python-dotenv', 'web3>=5.23.0,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['unipy = uniswap:main']}
 
 setup_kwargs = {
     'name': 'uniswap-python-route',
-    'version': '0.5.5.4',
+    'version': '0.5.5.5',
     'description': 'An unofficial Python wrapper for the decentralized exchange Uniswap',
     'long_description': '<p align="center">\n  <img width="350" height="350" src="https://user-images.githubusercontent.com/9441295/107376524-d96b5880-6a9e-11eb-9eba-094c439cfb07.png">\n</p>\n\n# uniswap-python\n\n[![GitHub Actions](https://github.com/shanefontaine/uniswap-python/workflows/Test/badge.svg)](https://github.com/shanefontaine/uniswap-python/actions)\n[![codecov](https://codecov.io/gh/uniswap-python/uniswap-python/branch/master/graph/badge.svg?token=VHAZHHLFX8)](https://codecov.io/gh/uniswap-python/uniswap-python)\n[![Downloads](https://pepy.tech/badge/uniswap-python)](https://pepy.tech/project/uniswap-python)\n[![License](http://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/shanefontaine/uniswap-python/master/LICENSE)\n[![PyPI](https://img.shields.io/pypi/v/uniswap-python)](https://pypi.org/project/uniswap-python/)\n[![Typechecking: Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n[![GitHub Repo stars](https://img.shields.io/github/stars/uniswap-python/uniswap-python?style=social)](https://github.com/uniswap-python/uniswap-python/stargazers)\n[![Twitter Follow](https://img.shields.io/twitter/follow/UniswapPython?label=Follow&style=social)](https://twitter.com/UniswapPython)\n\nThe unofficial Python client for [Uniswap](https://uniswap.io/).\n\nDocumentation is available at https://uniswap-python.com/\n\n## Functionality\n\n*  A simple to use Python wrapper for all available contract functions and variables\n*  A basic CLI to get prices and token metadata\n*  Simple parsing of data returned from the Uniswap contract\n\n### Supports\n\n - Uniswap v3 (as of v0.5.0)\n    - Including beta support for Arbitrum & Optimism deployments (as of v0.5.4)\n - Uniswap v2 (as of v0.4.0)\n - Uniswap v1 (deprecated)\n - Various forks (untested, but should work)\n   - Honeyswap (xDai)\n   - Pancakeswap (BSC)\n   - Sushiswap (mainnet)\n\n## Getting Started\n\nSee our [Getting started guide](https://uniswap-python.com/getting-started.html) in the documentation.\n\n## Testing\n\nUnit tests are under development using the pytest framework. Contributions are welcome!\n\nTest are run on a fork of the main net using ganache-cli. You need to install it with `npm install -g ganache-cli` before running tests.\n\nTo run the full test suite, in the project directory set the `PROVIDER` env variable to a mainnet provider, and run:\n\n```sh\npoetry install\nexport PROVIDER= # URL of provider, e.g. https://mainnet.infura.io/v3/...\nmake test\n# or...\npoetry run pytest --capture=no  # doesn\'t capture output (verbose)\n```\n\n## Support our continued work!\n\nYou can support us on [Gitcoin Grants](https://gitcoin.co/grants/2631/uniswap-python).\n\n## Authors\n\n* [Shane Fontaine](https://twitter.com/shanecoin)\n* [Erik Bjäreholt](https://twitter.com/ErikBjare)\n* [@liquid-8](https://github.com/liquid-8)\n* ...and [others](https://github.com/uniswap-python/uniswap-python/graphs/contributors)\n\n*Want to help out with development? We have funding to those that do! See [#181](https://github.com/uniswap-python/uniswap-python/discussions/181)*\n\n## Changelog\n\n_0.5.4_\n\n* added use of gas estimation instead of a fixed gas limit (to support Arbitrum)\n* added `use_estimate_gas` constructor argument (used in testing)\n* added constants/basic support for Arbitrum, Optimism, Polygon, and Fantom. (untested)\n* incomplete changelog\n\n_0.5.3_\n\n* incomplete changelog\n\n_0.5.2_\n\n* incomplete changelog\n\n_0.5.1_\n\n* Updated dependencies\n* Fixed minor typing issues\n\n_0.5.0_\n\n* Basic support for Uniswap V3\n* Added new methods `get_price_input` and `get_price_output`\n* Made a lot of previously public methods private\n* Added documentation site\n* Removed ENS support (which was probably broken to begin with)\n\n_0.4.6_\n\n* Bug fix: Update bleach package from 3.1.4 to 3.3.0\n\n_0.4.5_\n* Bug fix: Use .eth instead of .ens\n\n_0.4.4_\n\n* General: Add new logo for Uniswap V2\n* Bug fix: Invalid balance check (#25)\n* Bug fix: Fixed error when passing WETH as token\n\n_0.4.3_\n\n* Allow kwargs in `approved` decorator.\n\n_0.4.2_\n\n* Add note about Uniswap V2 support\n\n_0.4.1_\n\n* Update changelog for PyPi and clean up\n\n_0.4.0_\n\n_A huge thank you [Erik Bjäreholt](https://github.com/ErikBjare) for adding Uniswap V2 support, as well as all changes in this version!_\n\n* Added support for Uniswap v2\n* Handle arbitrary tokens (by address) using the factory contract\n* Switched from setup.py to pyproject.toml/poetry\n* Switched from Travis to GitHub Actions\n* For CI to work in your repo, you need to set the secret MAINNET_PROVIDER. I use Infura.\n* Running tests on a local fork of mainnet using ganache-cli (started as a fixture)\n* Fixed tests for make_trade and make_trade_output\n* Added type annotations to the entire codebase and check them with mypy in CI\n* Formatted entire codebase with black\n* Moved stuff around such that the basic import becomes from uniswap import Uniswap (instead of from uniswap.uniswap import UniswapWrapper)\n* Fixed misc bugs\n\n_0.3.3_\n*  Provide token inputs as addresses instead of names\n\n_0.3.2_\n*  Add ability to transfer tokens after a trade\n*  Add tests for this new functionality\n\n_0.3.1_\n*  Add tests for all types of trades\n\n_0.3.0_\n*  Add ability to make all types of trades\n*  Add example to README\n\n_0.2.1_\n*  Add liquidity tests\n\n_0.2.0_\n*  Add liquidity and ERC20 pool methods\n\n_0.1.1_\n*  Major README update\n\n_0.1.0_\n*  Add market endpoints\n*  Add tests for market endpoints\n',
     'author': 'Shane Fontaine',
     'author_email': 'shane6fontaine@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/starascendin/uniswap-python',
```

### Comparing `uniswap_python_route-0.5.5.4/PKG-INFO` & `uniswap_python_route-0.5.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniswap-python-route
-Version: 0.5.5.4
+Version: 0.5.5.5
 Summary: An unofficial Python wrapper for the decentralized exchange Uniswap
 Home-page: https://github.com/starascendin/uniswap-python
 License: MIT
 Keywords: uniswap,ethereum,exchange,trading
 Author: Shane Fontaine
 Author-email: shane6fontaine@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
```

