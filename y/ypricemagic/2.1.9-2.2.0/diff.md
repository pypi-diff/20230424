# Comparing `tmp/ypricemagic-2.1.9.tar.gz` & `tmp/ypricemagic-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.1.9.tar", last modified: Wed Apr 19 14:09:35 2023, max compression
+gzip compressed data, was "ypricemagic-2.2.0.tar", last modified: Mon Apr 24 20:25:19 2023, max compression
```

## Comparing `ypricemagic-2.1.9.tar` & `ypricemagic-2.2.0.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.520710 ypricemagic-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.508710 ypricemagic-2.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-19 14:09:35.520710 ypricemagic-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-19 14:09:35.520710 ypricemagic-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    19779 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.512710 ypricemagic-2.1.9/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19656 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6131 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10454 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    21688 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4361 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7796 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.516710 ypricemagic-2.1.9/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-19 14:09:20.000000 ypricemagic-2.1.9/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:09:35.520710 ypricemagic-2.1.9/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-19 14:09:35.000000 ypricemagic-2.1.9/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-19 14:09:35.000000 ypricemagic-2.1.9/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:09:35.000000 ypricemagic-2.1.9/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-19 14:09:35.000000 ypricemagic-2.1.9/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-19 14:09:35.000000 ypricemagic-2.1.9/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.336266 ypricemagic-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.340266 ypricemagic-2.2.0/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20009 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.344266 ypricemagic-2.2.0/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19656 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21688 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.348266 ypricemagic-2.2.0/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3853 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-24 20:25:08.000000 ypricemagic-2.2.0/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 20:25:19.352266 ypricemagic-2.2.0/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-24 20:25:19.000000 ypricemagic-2.2.0/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.1.9/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/.github/workflows/pytest.yaml` & `ypricemagic-2.2.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/.github/workflows/release.yaml` & `ypricemagic-2.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/LICENSE.txt` & `ypricemagic-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/README.md` & `ypricemagic-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/setup.py` & `ypricemagic-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/classes/test_erc20.py` & `ypricemagic-2.2.0/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/classes/test_singleton.py` & `ypricemagic-2.2.0/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/fixtures.py` & `ypricemagic-2.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.2.0/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/lending/test_aave.py` & `ypricemagic-2.2.0/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/lending/test_compound.py` & `ypricemagic-2.2.0/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/test_chainlink.py` & `ypricemagic-2.2.0/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/test_magic.py` & `ypricemagic-2.2.0/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/test_popsicle.py` & `ypricemagic-2.2.0/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/test_synthetix.py` & `ypricemagic-2.2.0/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/test_yearn.py` & `ypricemagic-2.2.0/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/tests/prices/utils/test_buckets.py` & `ypricemagic-2.2.0/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/__init__.py` & `ypricemagic-2.2.0/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/classes/common.py` & `ypricemagic-2.2.0/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/classes/singleton.py` & `ypricemagic-2.2.0/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/constants.py` & `ypricemagic-2.2.0/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/contracts.py` & `ypricemagic-2.2.0/y/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 #yLazyLogger(logger)
 def contract_creation_block(address: AnyAddressType, when_no_history_return_0: bool = False) -> int:
     """
     Determine the block when a contract was created using binary search.
     NOTE Requires access to historical state. Doesn't account for CREATE2 or SELFDESTRUCT.
     """
     address = convert.to_address(address)
-    logger.info("contract creation block %s", address)
+    logger.debug(f"contract creation block {address}")
     height = chain.height
 
     if height == 0:
         raise NodeNotSynced(f'''
             `chain.height` returns 0 on your node, which means it is not fully synced.
             You can only use this function on a fully synced node.''')
 
@@ -100,31 +100,32 @@
                 if not warned:
                     logger.warning(str(e))
             else:
                 raise
             warned = True
             barrier = mid
             lo = mid
-    if hi == lo + 1 == barrier + 1:
-        if when_no_history_return_0:
-            logger.warning(f'could not determine creation block for {address} on {Network.name()} (deployed prior to barrier)')
-            return 0
+    if hi == lo + 1 == barrier + 1 and when_no_history_return_0:
+        logger.warning(f'could not determine creation block for {address} on {Network.name()} (deployed prior to barrier)')
+        logger.debug(f"contract creation block {address} -> 0")
+        return 0
     if hi != height:
+        logger.debug(f"contract creation block {address} -> {hi}")
         return hi
     raise ValueError(f"Unable to find deploy block for {address} on {Network.name()}")
 
 
 @a_sync.a_sync(cache_type='memory')
 async def contract_creation_block_async(address: AnyAddressType, when_no_history_return_0: bool = False) -> int:
     """
     Determine the block when a contract was created using binary search.
     NOTE Requires access to historical state. Doesn't account for CREATE2 or SELFDESTRUCT.
     """
     address = convert.to_address(address)
-    logger.info("contract creation block %s", address)
+    logger.debug(f"contract creation block {address}")
     height = await dank_w3.eth.block_number
 
     if height == 0:
         raise NodeNotSynced(f'''
             `chain.height` returns 0 on your node, which means it is not fully synced.
             You can only use this function on a fully synced node.''')
 
@@ -150,19 +151,20 @@
                 if not warned:
                     logger.warning(str(e))
             else:
                 raise
             warned = True
             barrier = mid
             lo = mid
-    if hi == lo + 1 == barrier + 1:
-        if when_no_history_return_0:
-            logger.warning(f'could not determine creation block for {address} on {Network.name()} (deployed prior to barrier)')
-            return 0
+    if hi == lo + 1 == barrier + 1 and when_no_history_return_0:
+        logger.warning(f'could not determine creation block for {address} on {Network.name()} (deployed prior to barrier)')
+        logger.debug(f"contract creation block {address} -> 0")
+        return 0
     if hi != height:
+        logger.debug(f"contract creation block {address} -> {hi}")
         return hi
     raise ValueError(f"Unable to find deploy block for {address} on {Network.name()}")
 
 # this defaultdict prevents congestion in the contracts thread pool
 address_semaphores = defaultdict(lambda: ThreadsafeSemaphore(1))
 
 class Contract(brownie.Contract, metaclass=ChecksumAddressSingletonMeta):
```

### Comparing `ypricemagic-2.1.9/y/datatypes.py` & `ypricemagic-2.2.0/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/decorators.py` & `ypricemagic-2.2.0/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/erc20.py` & `ypricemagic-2.2.0/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/exceptions.py` & `ypricemagic-2.2.0/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/ERC20.py` & `ypricemagic-2.2.0/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.2.0/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/compound/unitroller.py` & `ypricemagic-2.2.0/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.2.0/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/multicall2.py` & `ypricemagic-2.2.0/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.2.0/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.2.0/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/networks.py` & `ypricemagic-2.2.0/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/band.py` & `ypricemagic-2.2.0/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/chainlink.py` & `ypricemagic-2.2.0/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/convex.py` & `ypricemagic-2.2.0/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.2.0/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/balancer/v1.py` & `ypricemagic-2.2.0/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/balancer/v2.py` & `ypricemagic-2.2.0/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/genericamm.py` & `ypricemagic-2.2.0/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/mooniswap.py` & `ypricemagic-2.2.0/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.2.0/y/prices/dex/uniswap/uniswap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+import os
 import threading
 from typing import Dict, Optional
 
 import a_sync
 from brownie import ZERO_ADDRESS, chain
 from multicall import Call
 
@@ -82,21 +83,25 @@
                 return price
         
         if chain.id == Network.Mainnet:
             return await self.get_price_v1(token_in, block, sync=False)
         
         return None
     
+    # NOTE: This uses mad memory so we arbitrarily cut it off at 50.
+    #       Feel free to implement your own limit with the env var. 
+    @a_sync.a_sync(semaphore=int(os.environ.get("YPM_DEEPEST_ROUTER_SEMAPHORE", 50)))
     async def deepest_router(self, token_in: AnyAddressType, block: Optional[Block] = None) -> Optional[UniswapRouterV2]:
         token_in = convert.to_address(token_in)
 
         for router in await self.routers_by_depth(token_in, block=block, sync=False):
             return router # will return first router in the dict, or None if no supported routers
         return None
 
+    
     async def routers_by_depth(self, token_in: AnyAddressType, block: Optional[Block] = None) -> Dict[UniswapRouterV2,str]:
         '''
         Returns a dict {router: pool} ordered by liquidity depth, greatest to least
         '''
         token_in = convert.to_address(token_in)
         routers = self.routers.values()
         pools_per_router = await asyncio.gather(*[router.pools_for_token(token_in, sync=False) for router in routers])
```

### Comparing `ypricemagic-2.1.9/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.2.0/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.2.0/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.2.0/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.2.0/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/eth_derivs/creth.py` & `ypricemagic-2.2.0/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.2.0/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/gearbox.py` & `ypricemagic-2.2.0/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/lending/aave.py` & `ypricemagic-2.2.0/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/lending/compound.py` & `ypricemagic-2.2.0/y/prices/lending/compound.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 TROLLERS = {
     Network.Mainnet: {
         "comp":             "0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B",
         "cream":            "0x3d5BC3c8d13dcB8bF317092d84783c2697AE9258",
         "ironbank":         "0xAB1c342C7bf5Ec5F02ADEA1c2270670bCa144CbB",
         "inverse":          "0x4dCf7407AE5C07f8681e1659f626E114A7667339",
         "unfederalreserve": "0x3105D328c66d8d55092358cF595d54608178E9B5",
+        "flux":             "0x95Af143a021DF745bc78e845b54591C53a8B3A51",
     },
     Network.BinanceSmartChain: {
         "venus":            "0xfD36E2c2a6789Db23113685031d7F16329158384",
     },
     Network.Polygon: {
         "easyfi":           "0xcb3fA413B23b12E402Cfcd8FA120f983FB70d8E8",
         "apple":            "0x46220a07F071D1a821D68fA7C769BCcdA3C65430",
```

### Comparing `ypricemagic-2.1.9/y/prices/lending/ib.py` & `ypricemagic-2.2.0/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/magic.py` & `ypricemagic-2.2.0/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/one_to_one.py` & `ypricemagic-2.2.0/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/popsicle.py` & `ypricemagic-2.2.0/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/stable_swap/belt.py` & `ypricemagic-2.2.0/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/stable_swap/curve.py` & `ypricemagic-2.2.0/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.2.0/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/stable_swap/froyo.py` & `ypricemagic-2.2.0/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.2.0/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/stable_swap/saddle.py` & `ypricemagic-2.2.0/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/synthetix.py` & `ypricemagic-2.2.0/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.2.0/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.2.0/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.2.0/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.2.0/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/utils/buckets.py` & `ypricemagic-2.2.0/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/utils/sense_check.py` & `ypricemagic-2.2.0/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/utils/ypriceapi.py` & `ypricemagic-2.2.0/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/prices/yearn.py` & `ypricemagic-2.2.0/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/time.py` & `ypricemagic-2.2.0/y/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     while wait_for_block_if_needed:
         try:
             return await closest_block_after_timestamp_async(timestamp)
         except NoBlockFound:
             await asyncio.sleep(0.2)
 
     height = await dank_w3.eth.block_number
-    print(height)
     lo, hi = 0, height
     while hi - lo > 1:
         mid = lo + (hi - lo) // 2
         if await get_block_timestamp_async(mid) > timestamp:
             hi = mid
         else:
             lo = mid
```

### Comparing `ypricemagic-2.1.9/y/utils/client.py` & `ypricemagic-2.2.0/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/utils/events.py` & `ypricemagic-2.2.0/y/utils/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,27 +139,31 @@
     end: Block
     ) -> List[LogReceipt]:
     if end - start == BATCH_SIZE - 1:
         response = _get_logs_batch_cached(address, topics, start, end)
     else:
         response = _get_logs_no_cache(address, topics, start, end)
     for log in response:
-        if log.address != address:
+        if address and log.address != address:
             ''' I have this due to a corrupt cache on my local box that I would prefer not to lose. '''
             ''' It will not impact your scripts. ''' 
             response.remove(log)
     return response
 
-address_semaphores = defaultdict(lambda: ThreadsafeSemaphore(16))
+get_logs_semaphores = defaultdict(lambda: ThreadsafeSemaphore(16))
 
-async def _get_logs_async(address, topics, start, end) -> List[LogReceipt]:
+def _get_semaphore_key(address, topics) -> tuple:
     if isinstance(address, list):
         address.sort()
-    semaphores_key = (tuple(address) if isinstance(address, list) else address, tuple(topics) if isinstance(topics, list) else topics)
-    async with address_semaphores[semaphores_key]:
+    addr_key = tuple(address) if isinstance(address, list) else address
+    topics_key = tuple(tuple(t) if isinstance(t, list) else t for t in topics) if isinstance(topics, list) else topics
+    return addr_key, topics_key
+
+async def _get_logs_async(address, topics, start, end) -> List[LogReceipt]:
+    async with get_logs_semaphores[_get_semaphore_key(address, topics)]:
         return await _get_logs(address, topics, start, end, asynchronous=True)
 
 @eth_retry.auto_retry
 def _get_logs_no_cache(
     address: Optional[ChecksumAddress],
     topics: Optional[List[str]],
     start: Block,
```

### Comparing `ypricemagic-2.1.9/y/utils/fakes.py` & `ypricemagic-2.2.0/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/utils/logging.py` & `ypricemagic-2.2.0/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/utils/middleware.py` & `ypricemagic-2.2.0/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/utils/multicall.py` & `ypricemagic-2.2.0/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/y/utils/raw_calls.py` & `ypricemagic-2.2.0/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/ypricemagic/magic.py` & `ypricemagic-2.2.0/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.1.9/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.2.0/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

