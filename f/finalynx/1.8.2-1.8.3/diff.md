# Comparing `tmp/finalynx-1.8.2.tar.gz` & `tmp/finalynx-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalynx-1.8.2.tar", max compression
+gzip compressed data, was "finalynx-1.8.3.tar", max compression
```

## Comparing `finalynx-1.8.2.tar` & `finalynx-1.8.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    35149 2023-04-21 20:18:01.257602 finalynx-1.8.2/LICENSE
--rw-r--r--   0        0        0     6890 2023-04-21 20:18:01.257602 finalynx-1.8.2/README.md
--rw-r--r--   0        0        0     1345 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/__init__.py
--rw-r--r--   0        0        0      770 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/__main__.py
--rw-r--r--   0        0        0      662 2023-04-21 20:18:02.581629 finalynx-1.8.2/finalynx/__meta__.py
--rw-r--r--   0        0        0      993 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/analyzer/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/analyzer/analyzer.py
--rw-r--r--   0        0        0     3187 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/analyzer/asset_class.py
--rw-r--r--   0        0        0     2398 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/analyzer/envelopes.py
--rw-r--r--   0        0        0     2858 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/analyzer/investment_state.py
--rw-r--r--   0        0        0     8047 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/assistant.py
--rw-r--r--   0        0        0      273 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/console.py
--rw-r--r--   0        0        0      424 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/copilot/__init__.py
--rw-r--r--   0        0        0      593 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/copilot/copilot.py
--rw-r--r--   0        0        0      427 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/dashboard/__init__.py
--rw-r--r--   0        0        0    11713 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/dashboard/dashboard.py
--rw-r--r--   0        0        0      891 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/fetch/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/fetch/fetch.py
--rw-r--r--   0        0        0    16256 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/fetch/fetch_finary.py
--rw-r--r--   0        0        0       47 2023-04-21 20:18:01.661610 finalynx-1.8.2/finalynx/finary_api/.git
--rw-r--r--   0        0        0      222 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/.github/dependabot.yml
--rw-r--r--   0        0        0     1905 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/.gitignore
--rw-r--r--   0        0        0     1064 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/LICENSE
--rw-r--r--   0        0        0     5099 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/README.md
--rwxr-xr-x   0        0        0      170 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/check.sh
--rw-r--r--   0        0        0       32 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/credentials.json.tpl
--rw-r--r--   0        0        0      691 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/__init__.py
--rw-r--r--   0        0        0    15625 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/__main__.py
--rw-r--r--   0        0        0      323 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/auth.py
--rw-r--r--   0        0        0      694 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/bank_account_types.py
--rw-r--r--   0        0        0      118 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/constants.py
--rw-r--r--   0        0        0      241 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/crypto_chains.py
--rw-r--r--   0        0        0      824 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/currencies.py
--rw-r--r--   0        0        0      308 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/institutions.py
--rw-r--r--   0        0        0      511 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/precious_metals.py
--rw-r--r--   0        0        0      494 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/scpis.py
--rw-r--r--   0        0        0     3276 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/securities.py
--rw-r--r--   0        0        0     2308 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/signin.py
--rw-r--r--   0        0        0     4177 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_cryptos.py
--rw-r--r--   0        0        0      246 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_me.py
--rw-r--r--   0        0        0     1670 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_portfolio.py
--rw-r--r--   0        0        0     1865 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_precious_metals.py
--rw-r--r--   0        0        0      222 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_real_estates.py
--rw-r--r--   0        0        0      208 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_scpis.py
--rw-r--r--   0        0        0     5680 2023-04-21 20:18:01.669611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_securities.py
--rw-r--r--   0        0        0      221 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/finary_api/user_startups.py
--rw-r--r--   0        0        0      196 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/finary_api/utils.py
--rw-r--r--   0        0        0     3253 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/finary_api/views.py
--rw-r--r--   0        0        0      478 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/mypy.ini
--rw-r--r--   0        0        0      195 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/requirements-tests.txt
--rw-r--r--   0        0        0       60 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/requirements.txt
--rw-r--r--   0        0        0      224 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/setup.cfg
--rw-r--r--   0        0        0       50 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/tests/data/cryptos.csv
--rw-r--r--   0        0        0      172 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/tests/data/stocks.csv
--rw-r--r--   0        0        0      340 2023-04-21 20:18:01.673611 finalynx-1.8.2/finalynx/finary_api/tests/data/stocks.json
--rw-r--r--   0        0        0      153 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/parse/__init__.py
--rw-r--r--   0        0        0      739 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/parse/json.py
--rw-r--r--   0        0        0     1007 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/parse/parser.py
--rw-r--r--   0        0        0     2016 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/__init__.py
--rw-r--r--   0        0        0     4675 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/bucket.py
--rw-r--r--   0        0        0      860 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/constants.py
--rw-r--r--   0        0        0     2427 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/envelope.py
--rw-r--r--   0        0        0     7703 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/folder.py
--rw-r--r--   0        0        0      422 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/hierarchy.py
--rw-r--r--   0        0        0     2436 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/line.py
--rw-r--r--   0        0        0     8333 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/node.py
--rw-r--r--   0        0        0     1195 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/portfolio.py
--rw-r--r--   0        0        0     3624 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/render.py
--rw-r--r--   0        0        0    11976 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/portfolio/targets.py
--rw-r--r--   0        0        0      419 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/simulator/__init__.py
--rw-r--r--   0        0        0     2385 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/simulator/simulator.py
--rw-r--r--   0        0        0     2088 2023-04-21 20:18:01.273602 finalynx-1.8.2/finalynx/usage.py
--rw-r--r--   0        0        0     1713 2023-04-21 20:18:02.581629 finalynx-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 finalynx-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 08:19:00.351602 finalynx-1.8.3/LICENSE
+-rw-r--r--   0        0        0     6890 2023-04-24 08:19:00.351602 finalynx-1.8.3/README.md
+-rw-r--r--   0        0        0     1345 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/__init__.py
+-rw-r--r--   0        0        0      770 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/__main__.py
+-rw-r--r--   0        0        0      662 2023-04-24 08:19:01.599645 finalynx-1.8.3/finalynx/__meta__.py
+-rw-r--r--   0        0        0      993 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/__init__.py
+-rw-r--r--   0        0        0     1101 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3187 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/asset_class.py
+-rw-r--r--   0        0        0     2398 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/envelopes.py
+-rw-r--r--   0        0        0     2858 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/analyzer/investment_state.py
+-rw-r--r--   0        0        0     8096 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/assistant.py
+-rw-r--r--   0        0        0      273 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/console.py
+-rw-r--r--   0        0        0      424 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/copilot/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/copilot/copilot.py
+-rw-r--r--   0        0        0      427 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/dashboard/__init__.py
+-rw-r--r--   0        0        0    11713 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/dashboard/dashboard.py
+-rw-r--r--   0        0        0      891 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/fetch/__init__.py
+-rw-r--r--   0        0        0     1095 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/fetch/fetch.py
+-rw-r--r--   0        0        0    16256 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/fetch/fetch_finary.py
+-rw-r--r--   0        0        0       47 2023-04-24 08:19:00.715614 finalynx-1.8.3/finalynx/finary_api/.git
+-rw-r--r--   0        0        0      222 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/.github/dependabot.yml
+-rw-r--r--   0        0        0     1905 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/.gitignore
+-rw-r--r--   0        0        0     1064 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/LICENSE
+-rw-r--r--   0        0        0     5099 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/README.md
+-rwxr-xr-x   0        0        0      170 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/check.sh
+-rw-r--r--   0        0        0       32 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/credentials.json.tpl
+-rw-r--r--   0        0        0      691 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/__init__.py
+-rw-r--r--   0        0        0    15625 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/__main__.py
+-rw-r--r--   0        0        0      323 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/auth.py
+-rw-r--r--   0        0        0      694 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/bank_account_types.py
+-rw-r--r--   0        0        0      118 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/constants.py
+-rw-r--r--   0        0        0      241 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/crypto_chains.py
+-rw-r--r--   0        0        0      824 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/currencies.py
+-rw-r--r--   0        0        0      308 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/institutions.py
+-rw-r--r--   0        0        0      511 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/precious_metals.py
+-rw-r--r--   0        0        0      494 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/scpis.py
+-rw-r--r--   0        0        0     3276 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/securities.py
+-rw-r--r--   0        0        0     2308 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/signin.py
+-rw-r--r--   0        0        0     4177 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_cryptos.py
+-rw-r--r--   0        0        0      246 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_holdings_accounts.py
+-rw-r--r--   0        0        0      411 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_me.py
+-rw-r--r--   0        0        0     1670 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_real_estates.py
+-rw-r--r--   0        0        0      208 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_scpis.py
+-rw-r--r--   0        0        0     5680 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_securities.py
+-rw-r--r--   0        0        0      221 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/user_startups.py
+-rw-r--r--   0        0        0      196 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/utils.py
+-rw-r--r--   0        0        0     3253 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/finary_api/views.py
+-rw-r--r--   0        0        0      478 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/mypy.ini
+-rw-r--r--   0        0        0      195 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/requirements.txt
+-rw-r--r--   0        0        0      224 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/setup.cfg
+-rw-r--r--   0        0        0       50 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/tests/data/cryptos.csv
+-rw-r--r--   0        0        0      172 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/tests/data/stocks.csv
+-rw-r--r--   0        0        0      340 2023-04-24 08:19:00.723615 finalynx-1.8.3/finalynx/finary_api/tests/data/stocks.json
+-rw-r--r--   0        0        0      153 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/parse/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/parse/json.py
+-rw-r--r--   0        0        0     1007 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/parse/parser.py
+-rw-r--r--   0        0        0     2016 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/bucket.py
+-rw-r--r--   0        0        0      860 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/constants.py
+-rw-r--r--   0        0        0     2427 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/envelope.py
+-rw-r--r--   0        0        0     7703 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/folder.py
+-rw-r--r--   0        0        0      422 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/hierarchy.py
+-rw-r--r--   0        0        0     2436 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/line.py
+-rw-r--r--   0        0        0     8333 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/node.py
+-rw-r--r--   0        0        0     1195 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/portfolio.py
+-rw-r--r--   0        0        0     3624 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/render.py
+-rw-r--r--   0        0        0    11976 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/portfolio/targets.py
+-rw-r--r--   0        0        0      419 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/simulator/__init__.py
+-rw-r--r--   0        0        0     2385 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/simulator/simulator.py
+-rw-r--r--   0        0        0     2088 2023-04-24 08:19:00.367602 finalynx-1.8.3/finalynx/usage.py
+-rw-r--r--   0        0        0     1713 2023-04-24 08:19:01.599645 finalynx-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     7777 1970-01-01 00:00:00.000000 finalynx-1.8.3/PKG-INFO
```

### Comparing `finalynx-1.8.2/LICENSE` & `finalynx-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/README.md` & `finalynx-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/__init__.py` & `finalynx-1.8.3/finalynx/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/__main__.py` & `finalynx-1.8.3/finalynx/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/__meta__.py` & `finalynx-1.8.3/finalynx/__meta__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ```{warning}
 Do not manually change this information.
 ```
 
 Metadata information about Finalynx. This file is used by Fynalinx and updated by the CI/CD pipeline.
 """
 
-__version__ = "1.8.2"
+__version__ = "1.8.3"
 
 __author__ = "Pierre Laclau (MadeInPierre)"
 
 __copyright__ = """
 Copyright (c) 2023, MadeInPierre
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
```

### Comparing `finalynx-1.8.2/finalynx/analyzer/__init__.py` & `finalynx-1.8.3/finalynx/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/analyzer/analyzer.py` & `finalynx-1.8.3/finalynx/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/analyzer/asset_class.py` & `finalynx-1.8.3/finalynx/analyzer/asset_class.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/analyzer/envelopes.py` & `finalynx-1.8.3/finalynx/analyzer/envelopes.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/analyzer/investment_state.py` & `finalynx-1.8.3/finalynx/analyzer/investment_state.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/assistant.py` & `finalynx-1.8.3/finalynx/assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         # Display deltas only if not already printed in the main tree
         if not self.hide_deltas and "delta" not in self.output_format:
             render.append(self.portfolio.tree_delta())
 
         # Final set of results to be displayed
         panels: List[ConsoleRenderable] = [
             Columns([Text("  ")] + render),  # type: ignore
-            Panel(self.render_envelopes(), title="Envelope investments", padding=(1, 2), expand=False),
+            Panel(self.render_envelopes(), title="Investments Summary", padding=(1, 2), expand=False),
         ]
 
         # Show the data fetched from Finary if specified
         if self.show_data:
             panels.append(Panel(finary_tree, title="Finary data"))
 
         # Display the entire portfolio and associated recommendations
@@ -167,16 +167,16 @@
         a summary of transfers to make."""
         tree = Tree("Envelopes", hide_root=True)
 
         for env in self.envelopes:
             children, env_delta = [], 0.0
             for line in env.lines:
                 delta = line.get_delta()
-                env_delta += delta
                 if delta != 0 and line.target.check() not in [Target.RESULT_NONE, Target.RESULT_OK]:
+                    env_delta += delta
                     children.append(line.render(output_format="[delta] [name]"))
 
             if children:
                 env_delta = round(env_delta)
                 render_delta = f"[{'green' if env_delta > 0 else 'red'}]{'+' if env_delta > 0 else ''}{env_delta} €"
                 node = tree.add(f"{render_delta} [dodger_blue2 bold]{env.name}")
                 for child in children:
@@ -189,14 +189,15 @@
                 if isinstance(child, Folder):
                     if child.display == FolderDisplay.EXPANDED:
                         found += _get_collapsed_folders(child)
                     else:
                         found.append(child)
             return found
 
-        node = tree.add("[dodger_blue2 bold]Collapsed folders")
         collapsed_folders = _get_collapsed_folders(self.portfolio)
-        for f in collapsed_folders:
-            if f.get_delta() != 0:
-                node.add(f.render(output_format="[delta] [name]"))
+        if collapsed_folders:
+            node = tree.add("[dodger_blue2 bold]Collapsed folders")
+            for f in collapsed_folders:
+                if f.get_delta() != 0:
+                    node.add(f.render(output_format="[delta] [name]"))
 
         return tree
```

### Comparing `finalynx-1.8.2/finalynx/copilot/copilot.py` & `finalynx-1.8.3/finalynx/copilot/copilot.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/dashboard/dashboard.py` & `finalynx-1.8.3/finalynx/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/fetch/__init__.py` & `finalynx-1.8.3/finalynx/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/fetch/fetch.py` & `finalynx-1.8.3/finalynx/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/fetch/fetch_finary.py` & `finalynx-1.8.3/finalynx/fetch/fetch_finary.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/.gitignore` & `finalynx-1.8.3/finalynx/finary_api/.gitignore`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/LICENSE` & `finalynx-1.8.3/finalynx/finary_api/LICENSE`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/README.md` & `finalynx-1.8.3/finalynx/finary_api/README.md`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/__init__.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/__main__.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/__main__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/bank_account_types.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/currencies.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/currencies.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/importers/cryptocom.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/securities.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/signin.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/signin.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/user_cryptos.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/user_generic_assets.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/user_holdings_accounts.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/user_portfolio.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/user_portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/user_precious_metals.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/user_securities.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/user_securities.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/finary_api/finary_api/views.py` & `finalynx-1.8.3/finalynx/finary_api/finary_api/views.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/parse/json.py` & `finalynx-1.8.3/finalynx/parse/json.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/parse/parser.py` & `finalynx-1.8.3/finalynx/parse/parser.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/__init__.py` & `finalynx-1.8.3/finalynx/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/bucket.py` & `finalynx-1.8.3/finalynx/portfolio/bucket.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/constants.py` & `finalynx-1.8.3/finalynx/portfolio/constants.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/envelope.py` & `finalynx-1.8.3/finalynx/portfolio/envelope.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/folder.py` & `finalynx-1.8.3/finalynx/portfolio/folder.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/line.py` & `finalynx-1.8.3/finalynx/portfolio/line.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/node.py` & `finalynx-1.8.3/finalynx/portfolio/node.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/portfolio.py` & `finalynx-1.8.3/finalynx/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/render.py` & `finalynx-1.8.3/finalynx/portfolio/render.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/portfolio/targets.py` & `finalynx-1.8.3/finalynx/portfolio/targets.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/simulator/simulator.py` & `finalynx-1.8.3/finalynx/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/finalynx/usage.py` & `finalynx-1.8.3/finalynx/usage.py`

 * *Files identical despite different names*

### Comparing `finalynx-1.8.2/pyproject.toml` & `finalynx-1.8.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finalynx"
-version = "1.8.2"
+version = "1.8.3"
 description = "A command line investment assistant to organize your portfolio and simulate its future to reach your life goals."
 authors = ["MadeInPierre <pielaclau@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "finalynx"}]
 include = [{ path = "finalynx/finary_api/**/*" }]
 
@@ -48,15 +48,15 @@
 upload_to_pypi = true
 upload_to_release = true
 commit_subject = "chore(release): auto bump version to {version}"
 build_command = "pip install poetry && poetry build"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.8.2"
+version = "1.8.3"
 tag_format = "v$version"
 
 [tool.mypy]
 exclude = [
     "finary_api/*",
     "docs/*",
     "tests/*.py"
```

### Comparing `finalynx-1.8.2/PKG-INFO` & `finalynx-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalynx
-Version: 1.8.2
+Version: 1.8.3
 Summary: A command line investment assistant to organize your portfolio and simulate its future to reach your life goals.
 License: GPLv3
 Author: MadeInPierre
 Author-email: pielaclau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finalynx Version: 1.8.2 Summary: A command line
+Metadata-Version: 2.1 Name: finalynx Version: 1.8.3 Summary: A command line
 investment assistant to organize your portfolio and simulate its future to
 reach your life goals. License: GPLv3 Author: MadeInPierre Author-email:
 pielaclau@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: docopt (==0.6.2)
```

