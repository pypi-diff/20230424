# Comparing `tmp/wellets_cli-1.2.0.tar.gz` & `tmp/wellets_cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellets_cli-1.2.0.tar", max compression
+gzip compressed data, was "wellets_cli-1.5.1.tar", max compression
```

## Comparing `wellets_cli-1.2.0.tar` & `wellets_cli-1.5.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1211 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/LICENSE
--rw-r--r--   0        0        0      949 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        6 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/VERSION
--rw-r--r--   0        0        0       46 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/__init__.py
--rw-r--r--   0        0        0      137 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/__main__.py
--rw-r--r--   0        0        0    13951 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/api.py
--rw-r--r--   0        0        0     1047 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/auth.py
--rw-r--r--   0        0        0      335 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/base.py
--rw-r--r--   0        0        0     1256 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/cli.py
--rw-r--r--   0        0        0        0 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/__init__.py
--rw-r--r--   0        0        0     8550 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/accumulation.py
--rw-r--r--   0        0        0     4992 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/asset.py
--rw-r--r--   0        0        0     1799 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/config.py
--rw-r--r--   0        0        0     1025 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/currency.py
--rw-r--r--   0        0        0     1896 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/investment.py
--rw-r--r--   0        0        0      646 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/login.py
--rw-r--r--   0        0        0     9365 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/portfolio.py
--rw-r--r--   0        0        0     1444 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/register.py
--rw-r--r--   0        0        0     6980 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/transaction.py
--rw-r--r--   0        0        0     3541 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/transfer.py
--rw-r--r--   0        0        0     6216 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/wallet.py
--rw-r--r--   0        0        0      187 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/commands/whoami.py
--rw-r--r--   0        0        0      194 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/config.py
--rw-r--r--   0        0        0     4100 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/model.py
--rw-r--r--   0        0        0      479 2022-12-04 13:04:20.854269 wellets_cli-1.2.0/wellets_cli/prompt.py
--rw-r--r--   0        0        0     8677 2022-12-04 13:04:20.858269 wellets_cli-1.2.0/wellets_cli/question.py
--rw-r--r--   0        0        0     4185 2022-12-04 13:04:20.858269 wellets_cli-1.2.0/wellets_cli/util.py
--rw-r--r--   0        0        0     5907 2022-12-04 13:04:20.858269 wellets_cli-1.2.0/wellets_cli/validator.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 wellets_cli-1.2.0/setup.py
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 wellets_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/LICENSE
+-rw-r--r--   0        0        0      990 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/VERSION
+-rw-r--r--   0        0        0       46 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/__main__.py
+-rw-r--r--   0        0        0    14811 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/api.py
+-rw-r--r--   0        0        0     1047 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/auth.py
+-rw-r--r--   0        0        0      335 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/base.py
+-rw-r--r--   0        0        0      973 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/chart.py
+-rw-r--r--   0        0        0     1281 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/cli.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/__init__.py
+-rw-r--r--   0        0        0     8501 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/accumulation.py
+-rw-r--r--   0        0        0     6479 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/asset.py
+-rw-r--r--   0        0        0     1333 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/currency.py
+-rw-r--r--   0        0        0     1896 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/investment.py
+-rw-r--r--   0        0        0      666 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/login.py
+-rw-r--r--   0        0        0    10997 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/portfolio.py
+-rw-r--r--   0        0        0     1394 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/register.py
+-rw-r--r--   0        0        0     6878 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/transaction.py
+-rw-r--r--   0        0        0     3571 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/transfer.py
+-rw-r--r--   0        0        0     6192 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/wallet.py
+-rw-r--r--   0        0        0      187 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/whoami.py
+-rw-r--r--   0        0        0      393 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/config.py
+-rw-r--r--   0        0        0     4176 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/model.py
+-rw-r--r--   0        0        0      479 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/prompt.py
+-rw-r--r--   0        0        0     9108 2023-04-24 20:39:50.756089 wellets_cli-1.5.1/wellets_cli/question.py
+-rw-r--r--   0        0        0     4250 2023-04-24 20:39:50.756089 wellets_cli-1.5.1/wellets_cli/util.py
+-rw-r--r--   0        0        0     6647 2023-04-24 20:39:50.756089 wellets_cli-1.5.1/wellets_cli/validator.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 wellets_cli-1.5.1/PKG-INFO
```

### Comparing `wellets_cli-1.2.0/LICENSE` & `wellets_cli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.2.0/pyproject.toml` & `wellets_cli-1.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "wellets_cli"
-version = "1.2.0"
+version = "1.5.1"
 description = "wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep under control your money."
 authors = ["lparolari"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dotenv = "^0.20.0"
 requests = "^2.28.1"
 pydantic = "^1.9.1"
 click = "^8.1.3"
 tabulate = "^0.8.10"
 python-dateutil = "^2.8.2"
 inquirerpy = "^0.3.4"
 numpy = "^1.23.5"
 matplotlib = "^3.6.2"
+dynaconf = "^3.1.12"
+codecov = "^2.1.13"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.4.2"
 pytest = "^7.1.2"
 flake8 = "^5.0.4"
 black = "^22.6.0"
 isort = "^5.10.1"
```

### Comparing `wellets_cli-1.2.0/wellets_cli/api.py` & `wellets_cli-1.5.1/wellets_cli/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 
 import requests
 
+from wellets_cli.config import settings
 from wellets_cli.auth import UserSession
-from wellets_cli.config import Config
 from wellets_cli.model import (
     Accumulation,
     Asset,
     AssetAllocation,
     AssetBalance,
     AverageLoadPrice,
     Balance,
@@ -20,55 +20,72 @@
     Transfer,
     User,
     UserCurrency,
     UserSettings,
     Wallet,
     WalletAverageLoadPrice,
     WalletHistory,
+    AssetHistory,
 )
 
-BASE_URL = Config.api_url
+base_url = lambda: settings.api_url
 
 
 class APIError(ValueError):
     pass
 
 
 def login(email: str, password: str) -> UserSession:
     response = requests.post(
-        f"{BASE_URL}/users/sessions",
+        f"{base_url()}/users/sessions",
         json={"email": email, "password": password},
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     user_session = response.json()
     user_session = UserSession(**user_session)
     return user_session
 
 
 def get_currencies(headers: dict) -> List[UserCurrency]:
     response = requests.get(
-        f"{BASE_URL}/currencies",
+        f"{base_url()}/currencies",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     currencies = response.json()
     currencies = map(lambda c: UserCurrency(**c), currencies)
     currencies = list(currencies)
     return currencies
 
 
+def sync_currencies(headers: dict) -> str:
+    response = requests.post(
+        f"{base_url()}/currencies/rate/sync",
+        headers=headers,
+    )
+
+    if not response.ok:
+        raise APIError(response.json())
+
+    if response.status_code == 201:
+        return "synced"
+    if response.status_code == 200:
+        return "already synced"
+    return "unknown"
+
+
 def get_wallets(headers: dict, params: Optional[dict] = None) -> List[Wallet]:
     response = requests.get(
-        f"{BASE_URL}/wallets",
+        f"{base_url()}/wallets",
         headers=headers,
         params=params,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
@@ -76,45 +93,45 @@
     wallets = map(lambda w: Wallet(**w), wallets)
     wallets = list(wallets)
     return wallets
 
 
 def create_wallet(data: dict, headers: dict) -> Wallet:
     response = requests.post(
-        f"{BASE_URL}/wallets",
+        f"{base_url()}/wallets",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     wallet = response.json()
     wallet = Wallet(**wallet)
     return wallet
 
 
 def update_wallet(wallet_id, data: dict, headers: dict) -> Wallet:
     response = requests.patch(
-        f"{BASE_URL}/wallets/{wallet_id}",
+        f"{base_url()}/wallets/{wallet_id}",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     wallet = response.json()
     wallet = Wallet(**wallet)
     return wallet
 
 
 def delete_wallet(wallet_id: str, headers: dict) -> Wallet:
     response = requests.delete(
-        f"{BASE_URL}/wallets/{wallet_id}",
+        f"{base_url()}/wallets/{wallet_id}",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     wallet = response.json()
@@ -122,30 +139,30 @@
     return wallet
 
 
 def get_wallet_average_load_price(
     params: dict, headers: dict
 ) -> WalletAverageLoadPrice:
     response = requests.get(
-        f"{BASE_URL}/wallets/average-load-price",
+        f"{base_url()}/wallets/average-load-price",
         params=params,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     avg_load_price = response.json()
     avg_load_price = WalletAverageLoadPrice(**avg_load_price)
     return avg_load_price
 
 
 def get_user_settings(headers: dict) -> UserSettings:
     response = requests.get(
-        f"{BASE_URL}/users/settings",
+        f"{base_url()}/users/settings",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     user_settings = response.json()
@@ -159,15 +176,15 @@
 
 
 def get_portfolios(params: dict, headers: dict) -> List[Portfolio]:
     portfolio_id = params.get("portfolio_id")
     show_all = params.get("show_all")
 
     response = requests.get(
-        f"{BASE_URL}/portfolios"
+        f"{base_url()}/portfolios"
         f"/{portfolio_id if portfolio_id else ''}"
         f"{'/all' if show_all else ''}",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
@@ -176,193 +193,191 @@
     portfolios = map(lambda w: Portfolio(**w), portfolios)
     portfolios = list(portfolios)
     return portfolios
 
 
 def get_portfolio(portfolio_id: str, headers: dict) -> Portfolio:
     response = requests.get(
-        f"{BASE_URL}/portfolios/{portfolio_id}/details",
+        f"{base_url()}/portfolios/{portfolio_id}/details",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     portfolio = response.json()
     portfolio = Portfolio(**portfolio)
     return portfolio
 
 
 def create_portfolio(data: dict, headers: dict) -> Portfolio:
     response = requests.post(
-        f"{BASE_URL}/portfolios",
+        f"{base_url()}/portfolios",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     portfolio = response.json()
     portfolio = Portfolio(**portfolio)
     return portfolio
 
 
 def edit_portfolio(portfolio_id: str, data: dict, headers: dict) -> Portfolio:
     response = requests.put(
-        f"{BASE_URL}/portfolios/{portfolio_id}",
+        f"{base_url()}/portfolios/{portfolio_id}",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     portfolio = response.json()
     portfolio = Portfolio(**portfolio)
     return portfolio
 
 
 def delete_portfolio(portfolio_id: str, headers: dict) -> Portfolio:
     response = requests.delete(
-        f"{BASE_URL}/portfolios/{portfolio_id}",
+        f"{base_url()}/portfolios/{portfolio_id}",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     portfolio = response.json()
     portfolio = Portfolio(**portfolio)
     return portfolio
 
 
 def get_wallet_balance(wallet_id: str, headers: dict) -> Balance:
     response = requests.get(
-        f"{BASE_URL}/wallets/balance",
+        f"{base_url()}/wallets/balance",
         params={"wallet_id": wallet_id},
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     balance = response.json()
     balance = Balance(**balance)
     return balance
 
 
 def get_total_balance(headers: dict) -> Balance:
     response = requests.get(
-        f"{BASE_URL}/wallets/total-balance",
+        f"{base_url()}/wallets/total-balance",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     balance = response.json()
     balance = Balance(**balance)
     return balance
 
 
 def get_wallets_total_balance(headers: dict) -> Balance:
     response = requests.get(
-        f"{BASE_URL}/wallets/total-balance",
+        f"{base_url()}/wallets/total-balance",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     balance = response.json()
     balance = Balance(**balance)
     return balance
 
 
 def get_portfolios_balance(params: dict, headers: dict) -> Balance:
     response = requests.get(
-        f"{BASE_URL}/portfolios/balance",
+        f"{base_url()}/portfolios/balance",
         params=params,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     balance = response.json()
     balance = Balance(**balance)
     return balance
 
 
-def get_portfolios_rebalance(
-    params: dict, headers: dict
-) -> PortfolioRebalance:
+def get_portfolios_rebalance(params: dict, headers: dict) -> PortfolioRebalance:
     portfolio_id = params["portfolio_id"]
 
     response = requests.get(
-        f"{BASE_URL}/portfolios/{portfolio_id}/rebalance",
+        f"{base_url()}/portfolios/{portfolio_id}/rebalance",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     rebalance = response.json()
     rebalance = PortfolioRebalance(**rebalance)
     return rebalance
 
 
 def get_transactions(params: dict, headers: dict) -> List[Transaction]:
     response = requests.get(
-        f"{BASE_URL}/transactions/",
+        f"{base_url()}/transactions/",
         params=params,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     transactions = response.json()["transactions"]
     transactions = [Transaction(**t) for t in transactions]
     return transactions
 
 
 def create_transaction(data: dict, headers: dict) -> Transaction:
     response = requests.post(
-        f"{BASE_URL}/transactions",
+        f"{base_url()}/transactions",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     transaction = response.json()
     transaction = Transaction(**transaction)
     return transaction
 
 
 def get_wallet(wallet_id: str, headers: dict) -> Wallet:
     response = requests.get(
-        f"{BASE_URL}/wallets/{wallet_id}",
+        f"{base_url()}/wallets/{wallet_id}",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     wallet = response.json()
     wallet = Wallet(**wallet)
     return wallet
 
 
 def get_accumulations(params: dict, headers: dict) -> List[Accumulation]:
     response = requests.get(
-        f"{BASE_URL}/accumulations/",
+        f"{base_url()}/accumulations/",
         headers=headers,
         params=params,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
@@ -371,224 +386,238 @@
     return accumulations
 
 
 def get_next_accumulation_entry(
     accumulation_id: str, headers: dict
 ) -> NextAccumulationEntry:
     response = requests.get(
-        f"{BASE_URL}/accumulations/{accumulation_id}/next-entry",
+        f"{base_url()}/accumulations/{accumulation_id}/next-entry",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     entry = response.json()
     entry = NextAccumulationEntry(**entry)
     return entry
 
 
 def create_accumulation(data: dict, headers: dict) -> Accumulation:
     response = requests.post(
-        f"{BASE_URL}/accumulations",
+        f"{base_url()}/accumulations",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     accumulation = response.json()
     accumulation = Accumulation(**accumulation)
     return accumulation
 
 
 def delete_accumulation(accumulation_id: str, headers: dict) -> Accumulation:
     response = requests.delete(
-        f"{BASE_URL}/accumulations/{accumulation_id}",
+        f"{base_url()}/accumulations/{accumulation_id}",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     accumulation = response.json()
     accumulation = Accumulation(**accumulation)
     return accumulation
 
 
 def create_transfer(data: dict, headers: dict) -> Transfer:
     response = requests.post(
-        f"{BASE_URL}/transfers",
+        f"{base_url()}/transfers",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     transfer = response.json()
     transfer = Transfer(**transfer)
     return transfer
 
 
 def get_assets(headers: dict) -> List[Asset]:
     response = requests.get(
-        f"{BASE_URL}/assets",
+        f"{base_url()}/assets",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     assets = response.json()
     assets = [Asset(**a) for a in assets]
     return assets
 
 
-def get_asset_average_load_price(
-    params: dict, headers: dict
-) -> AverageLoadPrice:
+def get_asset_average_load_price(params: dict, headers: dict) -> AverageLoadPrice:
     response = requests.get(
-        f"{BASE_URL}/assets/average-load-price",
+        f"{base_url()}/assets/average-load-price",
         params=params,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     avg_load_price = response.json()
     avg_load_price = AverageLoadPrice(**avg_load_price)
     return avg_load_price
 
 
 def get_asset_balance(params: dict, headers: dict) -> Balance:
     response = requests.get(
-        f"{BASE_URL}/assets/balance",
+        f"{base_url()}/assets/balance",
         params=params,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     asset_balance = response.json()
     asset_balance = AssetBalance(**asset_balance)
     return asset_balance
 
 
 def get_asset_allocations(headers: dict) -> List[AssetAllocation]:
     response = requests.get(
-        f"{BASE_URL}/assets/allocations",
+        f"{base_url()}/assets/allocations",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     allocations = response.json()
     allocations = [AssetAllocation(**a) for a in allocations]
     return allocations
 
 
 def get_total_asset_balance(headers: dict) -> Balance:
     response = requests.get(
-        f"{BASE_URL}/assets/total-balance",
+        f"{base_url()}/assets/total-balance",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     balance = response.json()
     balance = AssetBalance(**balance)
     return balance
 
 
 def revert_transaction(transaction_id: str, headers: dict) -> Transaction:
     response = requests.post(
-        f"{BASE_URL}/transactions/{transaction_id}/revert",
+        f"{base_url()}/transactions/{transaction_id}/revert",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     transaction = response.json()
     transaction = Transaction(**transaction)
     return transaction
 
 
 def set_preferred_currency(data: dict, headers: dict) -> UserSettings:
     response = requests.put(
-        f"{BASE_URL}/users/settings",
+        f"{base_url()}/users/settings",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     user_settings = response.json()
     user_settings = UserSettings(**user_settings)
     return user_settings
 
 
 def register(data: dict, headers: dict) -> User:
     response = requests.post(
-        f"{BASE_URL}/users",
+        f"{base_url()}/users",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     user = response.json()
     user = User(**user)
     return user
 
 
 def create_investment(data: dict, headers: dict) -> Investment:
     response = requests.post(
-        f"{BASE_URL}/investments",
+        f"{base_url()}/investments",
         json=data,
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     investment = response.json()
     investment = Investment(**investment)
     return investment
 
 
 def get_investments(headers: dict) -> List[Investment]:
     response = requests.get(
-        f"{BASE_URL}/investments",
+        f"{base_url()}/investments",
         headers=headers,
     )
 
     if not response.ok:
         raise APIError(response.json())
 
     investments = response.json()
     investments = [Investment(**i) for i in investments]
     return investments
 
 
 def get_wallet_history(params: dict, headers: dict) -> List[WalletHistory]:
     response = requests.get(
-        f"{BASE_URL}/wallets-balances/history",
+        f"{base_url()}/wallets-balances/history",
         params=params,
         headers=headers,
     )
 
     if not response.ok:
         print(response.status_code)
         raise APIError(response.json())
 
     history = response.json()
     history = [WalletHistory(**h) for h in history]
     return history
+
+
+def get_asset_history(params: dict, headers: dict) -> List[AssetHistory]:
+    response = requests.get(
+        f"{base_url()}/assets/history",
+        params=params,
+        headers=headers,
+    )
+
+    if not response.ok:
+        print(response.status_code)
+        raise APIError(response.json())
+
+    history = response.json()
+    history = [AssetHistory(**h) for h in history]
+    return history
```

### Comparing `wellets_cli-1.2.0/wellets_cli/auth.py` & `wellets_cli-1.5.1/wellets_cli/auth.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.2.0/wellets_cli/cli.py` & `wellets_cli-1.5.1/wellets_cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pathlib
 
 import click
 
 from wellets_cli.commands.accumulation import accumulation
 from wellets_cli.commands.asset import asset
-from wellets_cli.commands.config import config
 from wellets_cli.commands.currency import currency
 from wellets_cli.commands.investment import investment
 from wellets_cli.commands.login import login
 from wellets_cli.commands.portfolio import portfolio
 from wellets_cli.commands.register import register
 from wellets_cli.commands.transaction import transaction
 from wellets_cli.commands.transfer import transfer
@@ -25,21 +24,29 @@
 @click.group()
 @click.version_option(VERSION)
 def cli():
     pass
 
 
 def main():  # pragma: no cover
-    cli.add_command(wallet)
+
+    # user
     cli.add_command(login)
+    cli.add_command(register)
     cli.add_command(whoami)
-    cli.add_command(portfolio)
-    cli.add_command(config)
+
+    # wallets and transactions
+    cli.add_command(wallet)
     cli.add_command(transaction)
-    cli.add_command(currency)
-    cli.add_command(accumulation)
     cli.add_command(transfer)
+
+    # assets
     cli.add_command(asset)
-    cli.add_command(register)
-    cli.add_command(investment)
+    cli.add_command(portfolio)
+
+    # currency
+    cli.add_command(currency)
+
+    cli.add_command(accumulation)  # DEPRECATED
+    cli.add_command(investment)  # PREVIEW
 
     cli()
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/accumulation.py` & `wellets_cli-1.5.1/wellets_cli/commands/accumulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     AndValidator,
     EmptyInputValidator,
     GreaterThanValidator,
     NumberValidator,
 )
 
 
-@click.group()
+@click.group(deprecated=True)
 def accumulation():
     pass
 
 
 @accumulation.command(name="list")
 @click.option("--asset-id")
 @click.option("-i", "--interactive")
@@ -39,17 +39,15 @@
 
     wallets = api.get_wallets(headers=headers)
 
     asset_id = asset_id or (
         asset_question(wallets=wallets).execute() if interactive else None
     )
 
-    accumulations = api.get_accumulations(
-        {"asset_id": asset_id}, headers=headers
-    )
+    accumulations = api.get_accumulations({"asset_id": asset_id}, headers=headers)
 
     def get_accumulation_row(accumulation: Accumulation):
         return {
             "id": accumulation.id,
             "alias": accumulation.alias,
             "strategy": accumulation.strategy,
             "quote": accumulation.quote,
@@ -160,17 +158,15 @@
             message="Alias",
             validate=EmptyInputValidator(),
         ).execute()
     )
 
     strategy = (
         strategy
-        or inquirer.text(
-            message="Strategy", validate=EmptyInputValidator()
-        ).execute()
+        or inquirer.text(message="Strategy", validate=EmptyInputValidator()).execute()
     )
 
     quote = (
         quote
         or inquirer.number(
             message="Quote",
             float_allowed=True,
@@ -266,17 +262,15 @@
     headers = make_headers(auth_token)
 
     accumulation = __prompt_accumulation(accumulation_id, headers)
 
     if not accumulation:
         return
 
-    next_entry = api.get_next_accumulation_entry(
-        accumulation.id, headers=headers
-    )
+    next_entry = api.get_next_accumulation_entry(accumulation.id, headers=headers)
 
     description = (
         description
         or inquirer.text(
             message="Description",
             default=f"{accumulation.alias} entry #{next_entry.entry}",
             validate=EmptyInputValidator(),
@@ -288,23 +282,20 @@
         "accumulation_id": accumulation.id,
         "description": description,
     }
 
     ctx.invoke(create_transaction, **params)
 
 
-def __prompt_accumulation(
-    accumulation_id: str, headers
-) -> Optional[Accumulation]:
+def __prompt_accumulation(accumulation_id: str, headers) -> Optional[Accumulation]:
     accumulations = api.get_accumulations(params={}, headers=headers)
 
     if len(accumulations) == 0:
         return None
 
     accumulation_id = (
-        accumulation_id
-        or accumulation_question(accumulations=accumulations).execute()
+        accumulation_id or accumulation_question(accumulations=accumulations).execute()
     )
 
     accumulation = get_by_id(accumulations, accumulation_id)  # type: ignore
 
     return accumulation
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/config.py` & `wellets_cli-1.5.1/wellets_cli/commands/currency.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,47 @@
 import click
 from tabulate import tabulate
 
 import wellets_cli.api as api
 from wellets_cli.auth import get_auth_token
-from wellets_cli.config import Config
-from wellets_cli.question import currency_question
-from wellets_cli.util import make_headers
-
-CONFIG_API_URL = "api.url"
-CONFIG_API_USERNAME = "api.username"
-CONFIG_API_PASSWORD = "api.password"
-CONFIG_USER_PREFERRED_CURRENCY = "user-settings.preferred-currency"
-SETTABLE_CONFIGS = [CONFIG_USER_PREFERRED_CURRENCY]
+from wellets_cli.model import Currency
+from wellets_cli.util import change_value, make_headers
 
 
 @click.group()
-def config():
+def currency():
     pass
 
 
-@config.command(name="show")
+@currency.command(name="list")
 @click.option("--auth-token")
-def show_config(auth_token):
+def list_currencies(auth_token):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
-    preferred_currency = api.get_preferred_currency(headers=headers)
+    currencies = api.get_currencies(headers=headers)
 
-    data = [
-        {"config": CONFIG_API_URL, "value": Config.api_url},
-        {"config": CONFIG_API_USERNAME, "value": Config.api_username},
-        {"config": CONFIG_API_PASSWORD, "value": "<sensitive>"},
-        {
-            "config": CONFIG_USER_PREFERRED_CURRENCY,
-            "value": preferred_currency.acronym,
-        },
-    ]
+    def get_row_value(currency: Currency):
+        return {
+            "id": currency.id,
+            "acronym": currency.acronym,
+            "alias": currency.alias,
+            "dollar_rate": currency.dollar_rate,
+            "countervalue": change_value(currency.dollar_rate, 1, 1),
+            "updated_at": currency.updated_at.strftime("%Y-%m-%d %H:%M"),
+            "created_at": currency.created_at.strftime("%Y-%m-%d"),
+        }
+
+    data = list(map(get_row_value, currencies))
 
     print(tabulate(data, headers="keys"))
 
 
-@config.command(name="set")
-@click.argument("config")
+@currency.command(name="sync")
 @click.option("--auth-token")
-def set_config(config, auth_token):
+def sync_currencies(auth_token):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
-    if CONFIG_USER_PREFERRED_CURRENCY in config:
-        preferred_currency = api.get_preferred_currency(headers=headers)
-        currencies = api.get_currencies(headers=headers)
-
-        currency_id = currency_question(
-            currencies, default=preferred_currency
-        ).execute()
-
-        user_settings = api.set_preferred_currency(
-            data={"currency_id": currency_id}, headers=headers
-        )
+    sync_status = api.sync_currencies(headers=headers)
 
-    print(user_settings.id)
+    print(f"Currencies sync completed with status '{sync_status}'")
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/investment.py` & `wellets_cli-1.5.1/wellets_cli/commands/investment.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/login.py` & `wellets_cli-1.5.1/wellets_cli/commands/login.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Optional
 
 import click
 from InquirerPy import inquirer
 
 import wellets_cli.api as api
 from wellets_cli.auth import persist_auth
-from wellets_cli.config import Config
+from wellets_cli.config import settings
 
 
 @click.command()
 @click.option("--email")
 @click.option("--password")
 def login(email: Optional[str], password: Optional[str]):
     email = (
         email
-        or Config.api_username
+        or settings.get("api_username")
         or inquirer.text(message="Email").execute()
     )
     password = (
         password
-        or Config.api_password
+        or settings.get("api_password")
         or inquirer.secret(message="Password").execute()
     )
 
     user_session = api.login(email, password)
 
     persist_auth(user_session.json())
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/portfolio.py` & `wellets_cli-1.5.1/wellets_cli/commands/portfolio.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 
 @portfolio.command(name="list")
 @click.option("-id", "--portfolio-id", type=click.UUID)
 @click.option("-f", "--flatten", is_flag=True)
 @click.option("-a", "--all", "show_all", is_flag=True)
 @click.option("-i", "--interactive", is_flag=True)
+@click.option("-v", "--verbose", is_flag=True)
 @click.option("--auth-token")
-def list_portfolios(portfolio_id, flatten, show_all, interactive, auth_token):
+def list_portfolios(portfolio_id, flatten, show_all, interactive, verbose, auth_token):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
     portfolio_id = portfolio_id or (
         interactive
         and portfolio_question(
             portfolios=api.get_portfolios(
@@ -61,41 +62,93 @@
             for child in portfolio.children:
                 yield child
 
     if flatten:
         portfolios = [p for p in flatten_portfolios()]
 
     def get_row_value(portfolio: Portfolio):
+        if verbose:
+            children = ", ".join(sorted([child.alias for child in portfolio.children]))
+            wallets = ", ".join(sorted([wallet.alias for wallet in portfolio.wallets]))
+        else:
+            children = (
+                f"{len(portfolio.children)} children"
+                if len(portfolio.children) > 0
+                else ""
+            )
+            wallets = (
+                f"{len(portfolio.wallets)} wallets"
+                if len(portfolio.wallets) > 0
+                else ""
+            )
+
         return {
             "id": portfolio.id,
             "alias": portfolio.alias,
-            "weight": pp(portfolio.weight, percent=True, decimals=0),
+            "weight (%)": pp(portfolio.weight, 0, percent=True),
             "parent": portfolio.parent.alias if portfolio.parent else None,
-            "children": ", ".join(
-                [child.alias for child in portfolio.children]
-            ),
-            "wallets": ", ".join([w.alias for w in portfolio.wallets]),
+            "children": children,
+            "wallets": wallets,
         }
 
     data = list(map(get_row_value, portfolios))
 
     print(tabulate(data, headers="keys"))
 
 
+@portfolio.command(name="show")
+@click.option("-n", "--alias", type=str)
+@click.option("--auth-token")
+def show_portfolio(alias, auth_token):
+    auth_token = auth_token or get_auth_token()
+    headers = make_headers(auth_token)
+
+    alias = alias or ""
+
+    # TODO: replace with the proper API call
+    portfolios = api.get_portfolios(
+        params={"portfolio_id": None, "show_all": True},
+        headers=headers,
+    )
+
+    search = [p for p in portfolios if alias.lower() in p.alias.lower()]
+
+    if len(search) == 0:
+        print("No portfolio found")
+
+    portfolio = search[0]
+
+    data = [
+        {"key": "id", "value": portfolio.id},
+        {"key": "alias", "value": portfolio.alias},
+        {"key": "weight", "value": pp(portfolio.weight, 0, percent=True)},
+        {"key": "parent", "value": portfolio.parent.alias if portfolio.parent else "-"},
+        {
+            "key": "children",
+            "value": "\n".join(sorted([child.alias for child in portfolio.children]))
+            or "-",
+        },
+        {
+            "key": "wallets",
+            "value": "\n".join(sorted([w.alias for w in portfolio.wallets])) or "-",
+        },
+    ]
+
+    print(tabulate(data, headers="keys"))
+
+
 @portfolio.command(name="create")
 @click.option("--auth-token")
 @click.option("--alias", type=str)
 @click.option("--weight", type=click.FloatRange(0, 100))
 @click.option("--parent-id", type=click.UUID)
 @click.option(
     "--wallet-ids",
     multiple=True,
-    callback=lambda _1, _2, value: validate(
-        each_validator(uuid_validator), value
-    ),
+    callback=lambda _1, _2, value: validate(each_validator(uuid_validator), value),
 )
 @click.option("-y", "--yes", is_flag=True, type=bool)
 def create_portfolio(alias, weight, parent_id, wallet_ids, auth_token, yes):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
     weight = weight and float(weight) / 100
@@ -126,16 +179,15 @@
         or portfolio_question(
             portfolios=portfolios,
             message="Parent",
             allow_none=True,
         ).execute()
     )
     wallet_ids = (
-        wallet_ids
-        or wallets_question(wallets=wallets, allow_none=True).execute()
+        wallet_ids or wallets_question(wallets=wallets, allow_none=True).execute()
     )
 
     data = {
         "alias": alias,
         "weight": weight,
         "parent_id": parent_id,
         "wallet_ids": wallet_ids,
@@ -154,22 +206,18 @@
 @click.option("-id", "--portfolio-id", type=click.UUID)
 @click.option("--alias", type=str)
 @click.option("--weight", type=click.FloatRange(0, 100))
 @click.option("--parent-id", type=click.UUID)
 @click.option(
     "--wallet-ids",
     multiple=True,
-    callback=lambda _1, _2, value: validate(
-        each_validator(uuid_validator), value
-    ),
+    callback=lambda _1, _2, value: validate(each_validator(uuid_validator), value),
 )
 @click.option("-y", "--yes", is_flag=True, type=bool)
-def edit_portfolio(
-    portfolio_id, alias, weight, parent_id, wallet_ids, auth_token, yes
-):
+def edit_portfolio(portfolio_id, alias, weight, parent_id, wallet_ids, auth_token, yes):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
     weight = weight and float(weight) / 100
 
     portfolio_id = (
         portfolio_id
@@ -309,17 +357,17 @@
     result = api.get_portfolios_rebalance(
         params={"portfolio_id": portfolio_id}, headers=headers
     )
 
     def get_row_value(change: RebalanceChange):
         return {
             "portfolio": change.portfolio.alias,
-            "desired": f"{pp(change.portfolio.weight, percent=True, decimals=0)}",
-            "current": pp(change.weight, percent=True, decimals=2),
-            "off_by": pp(change.off_by, percent=True),
+            "desired (%)": f"{pp(change.portfolio.weight, 0, percent=True)}",
+            "current (%)": pp(change.weight, 1, percent=True),
+            "off_by (%)": pp(change.off_by, 1, percent=True),
             "target": pp(change.target),
             "actual": pp(change.actual),
             "rebalance": f"{change.action.type} {pp(change.action.amount)} {result.currency.acronym}",
         }
 
     data = list(map(get_row_value, result.changes))
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/register.py` & `wellets_cli-1.5.1/wellets_cli/commands/register.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,46 +15,40 @@
 )
 
 
 @click.command()
 @click.option("--email")
 @click.option("--password")
 @click.option("--auth-token")
-def register(
-    email: Optional[str], password: Optional[str], auth_token: Optional[str]
-):
+def register(email: Optional[str], password: Optional[str], auth_token: Optional[str]):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
     email = (
         email
         or inquirer.text(
             message="Email",
             validate=AndValidator([EmptyInputValidator(), EmailValidator()]),
         ).execute()
     )
     password = (
         password
         or inquirer.secret(
             message="Password",
-            validate=AndValidator(
-                [EmptyInputValidator(), TextLengthValidator(6)]
-            ),
+            validate=AndValidator([EmptyInputValidator(), TextLengthValidator(6)]),
         ).execute()
     )
 
     inquirer.secret(
         message="Confirm password",
         validate=AndValidator(
             [
                 EmptyInputValidator(),
                 TextLengthValidator(6),
                 PasswordMatchValidator(password),
             ]
         ),
     ).execute()
 
-    user = api.register(
-        data={"email": email, "password": password}, headers=headers
-    )
+    user = api.register(data={"email": email, "password": password}, headers=headers)
 
     print(user.id)
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/transaction.py` & `wellets_cli-1.5.1/wellets_cli/commands/transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,15 @@
 @transaction.command(name="list")
 @click.option("-id", "--wallet-id", type=click.UUID)
 @click.option("--auth-token")
 def list_transactions(wallet_id, auth_token):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
-    wallet_id = (
-        wallet_id
-        or wallet_question(api.get_wallets(headers=headers)).execute()
-    )
+    wallet_id = wallet_id or wallet_question(api.get_wallets(headers=headers)).execute()
 
     transactions = api.get_transactions(
         {"wallet_id": wallet_id, "limit": 25, "page": 1}, headers=headers
     )
     preferred_currency = api.get_preferred_currency(headers=headers)
 
     def get_row_value(transaction: Transaction):
@@ -134,23 +131,20 @@
         value
         or inquirer.number(
             message=f"{transaction_type} amount ({wallet_currency.acronym})",
             float_allowed=True,
             validate=AndValidator(
                 [EmptyInputValidator(), GreaterThanOrEqualValidator(0)]
             ),
-            filter=lambda x: float(x)
-            * (1 if transaction_type == "Income" else -1),
+            filter=lambda x: float(x) * (1 if transaction_type == "Income" else -1),
         ).execute()
     )
 
     if not dollar_rate:
-        usd_currency = get_currency_by_acronym(
-            currencies, acronym="USD", safe=True
-        )
+        usd_currency = get_currency_by_acronym(currencies, acronym="USD", safe=True)
 
         currency_id = (
             change_currency_id
             or currency_question(
                 currencies=currencies,
                 message="Change rate",
                 default=usd_currency,
@@ -210,34 +204,28 @@
 
 
 @transaction.command(name="revert")
 @click.option("--wallet-id", type=click.UUID)
 @click.option(
     "--transaction-ids",
     multiple=True,
-    callback=lambda _1, _2, value: validate(
-        each_validator(uuid_validator), value
-    ),
+    callback=lambda _1, _2, value: validate(each_validator(uuid_validator), value),
 )
 @click.option("--auth-token")
 @click.option("-y", "--yes", is_flag=True, type=bool, default=False)
 def revert_transaction(wallet_id, transaction_ids, auth_token, yes):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
     wallets = api.get_wallets(headers=headers)
     wallet_id = wallet_id or wallet_question(wallets).execute()
 
-    transactions = api.get_transactions(
-        {"wallet_id": wallet_id}, headers=headers
-    )
+    transactions = api.get_transactions({"wallet_id": wallet_id}, headers=headers)
 
-    transaction_ids = (
-        transaction_ids or transactions_question(transactions).execute()
-    )
+    transaction_ids = transaction_ids or transactions_question(transactions).execute()
 
     if not yes and not confirm_question().execute():
         return
 
     for transaction_id in transaction_ids:
         reverted = api.revert_transaction(transaction_id, headers=headers)
         print(reverted.id)
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/transfer.py` & `wellets_cli-1.5.1/wellets_cli/commands/transfer.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 @transfer.command(name="create")
 @click.option("--from-wallet-id", type=click.UUID)
 @click.option("--to-wallet-id", type=click.UUID)
 @click.option("--percentual-fee", type=float)
 @click.option("--static-fee", type=float)
 @click.option("--value", type=float)
-@click.option(
-    "-m", "--use-max-balance", type=bool, is_flag=True, default=False
-)
+@click.option("-m", "--use-max-balance", type=bool, is_flag=True, default=False)
 @click.option("-y", "--yes", is_flag=True, type=bool)
 @click.option("--auth-token")
 def create_transfer(
     from_wallet_id,
     to_wallet_id,
     percentual_fee,
     static_fee,
@@ -49,27 +47,25 @@
         or wallet_question(message="From wallet", wallets=wallets).execute()
     )
 
     to_wallet_id = (
         to_wallet_id
         or wallet_question(
             message="To wallet",
-            wallets=[
-                wallet for wallet in wallets if wallet.id != from_wallet_id
-            ],
+            wallets=[wallet for wallet in wallets if wallet.id != from_wallet_id],
         ).execute()
     )
 
     from_wallet = api.get_wallet(from_wallet_id, headers=headers)
 
     value = (
         value
         or inquirer.number(
             message=f"Value ({from_wallet.currency.alias})",
-            default=from_wallet.balance if use_max_balance else "",
+            default=from_wallet.balance if use_max_balance else 0,
             float_allowed=True,
             transformer=lambda x: pp(float(x), fixed=False),
             filter=lambda x: float(x),
             validate=AndValidator(
                 [
                     EmptyInputValidator(),
                     NumberValidator(float_allowed=True),
@@ -81,15 +77,18 @@
 
     percentual_fee = (
         percentual_fee
         or inquirer.number(
             message=f"Percentual fee ({from_wallet.currency.alias})",
             float_allowed=True,
             transformer=lambda x: pp(
-                float(x) / 100, percent=True, fixed=False
+                float(x) / 100,
+                percent=True,
+                fixed=False,
+                with_symbol=True,
             ),
             filter=lambda x: float(x) / 100,
             validate=AndValidator(
                 [
                     EmptyInputValidator(),
                     NumberValidator(float_allowed=True),
                 ]
```

### Comparing `wellets_cli-1.2.0/wellets_cli/commands/wallet.py` & `wellets_cli-1.5.1/wellets_cli/commands/wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,32 +173,28 @@
     result = api.get_wallets_total_balance(headers=headers)
 
     print(f"{result.balance} {result.currency.acronym}")
 
 
 @wallet.command(name="history")
 @click.option("--wallet-id")
-@click.option(
-    "--interval", type=click.Choice(["1d", "1w"], case_sensitive=True)
-)
+@click.option("--interval", type=click.Choice(["1d", "1w"], case_sensitive=True))
 @click.option("--start-date", type=click.DateTime())
 @click.option("--end-date", type=click.DateTime())
 @click.option("--path", type=click.Path())
 @click.option("--auth-token")
 def show_wallet_history(wallet_id, interval, start_date, end_date, path, auth_token):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
     wallets = api.get_wallets(headers=headers)
 
     wallet_id = wallet_id or wallet_question(wallets).execute()
     interval = interval or interval_question().execute()
-    start_date, end_date = (
-        start_date and end_date
-    ) or date_range_question().execute()
+    start_date, end_date = (start_date and end_date) or date_range_question().execute()
 
     params = {
         "wallet_id": wallet_id,
         "start": start_date,
         "end": end_date,
         "interval": interval,
     }
@@ -210,13 +206,13 @@
 
     xs = np.array([x.timestamp for x in history])
     ys = np.array([x.balance for x in history])
 
     fig, ax = plt.subplots()
     fig.autofmt_xdate()
     ax.plot(xs, ys)
-    
+
     if path:
         plt.savefig(path)
         print("Saved to", path)
     else:
         plt.show()
```

### Comparing `wellets_cli-1.2.0/wellets_cli/model.py` & `wellets_cli-1.5.1/wellets_cli/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,7 +210,12 @@
     def is_closed(self):
         return self.status == self.CLOSED
 
 
 class WalletHistory(BaseModel):
     timestamp: datetime
     balance: float
+
+
+class AssetHistory(BaseModel):
+    timestamp: datetime
+    balance: float
```

### Comparing `wellets_cli-1.2.0/wellets_cli/question.py` & `wellets_cli-1.5.1/wellets_cli/question.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from datetime import datetime, timedelta
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Tuple
 
 from InquirerPy import inquirer
-from InquirerPy.base import BaseComplexPrompt, BaseSimplePrompt
 from InquirerPy.base.control import Choice, Separator
-from InquirerPy.prompts import (
-    ConfirmPrompt,
-    InputPrompt,
-    ListPrompt,
-    NumberPrompt,
-)
+from InquirerPy.prompts import ConfirmPrompt, InputPrompt, ListPrompt, NumberPrompt
 from InquirerPy.validator import EmptyInputValidator, NumberValidator
 
 from wellets_cli.model import (
     Accumulation,
     Asset,
     Currency,
     Portfolio,
@@ -48,17 +42,15 @@
 def wallets_question(
     wallets: List[Wallet],
     message: str = "Wallets",
     default: List[Wallet] = None,
     allow_none: bool = False,
 ) -> ListPrompt:
     no_option = (
-        [Separator(), Choice(value=None, name="No wallets")]
-        if allow_none
-        else []
+        [Separator(), Choice(value=None, name="No wallets")] if allow_none else []
     )
 
     return inquirer.select(
         message=message,
         choices=[
             Choice(
                 w.id,
@@ -76,17 +68,15 @@
 def portfolio_question(
     portfolios: List[Portfolio],
     message: str = "Portfolio",
     default: Optional[Portfolio] = None,
     allow_none: bool = False,
 ) -> ListPrompt:
     no_option = (
-        [Separator(), Choice(value=None, name="No parent")]
-        if allow_none
-        else []
+        [Separator(), Choice(value=None, name="No parent")] if allow_none else []
     )
 
     return inquirer.select(
         message=message,
         choices=[
             Choice(
                 p.id,
@@ -120,17 +110,15 @@
 def currency_question(
     currencies: List[Currency],
     message: str = "Currency",
     default: Optional[Currency] = None,
     mandatory=True,
 ) -> ListPrompt:
     return inquirer.select(
-        choices=[
-            Choice(w.id, name=f"{w.acronym} - {w.alias}") for w in currencies
-        ],
+        choices=[Choice(w.id, name=f"{w.acronym} - {w.alias}") for w in currencies],
         default=default and default.id,
         message=message,
         mandatory=mandatory,
     )
 
 
 def change_value_question(
@@ -154,33 +142,29 @@
 
     return inquirer.number(
         message=message
         or f"Change value (1 {source_currency.acronym} equals ? {target_currency.acronym})",
         float_allowed=True,
         min_allowed=0,
         default=default
-        or change_value(
-            source_currency.dollar_rate, target_currency.dollar_rate, 1
-        ),
+        or change_value(source_currency.dollar_rate, target_currency.dollar_rate, 1),
         filter=lambda v: (1 / float(v)) * target_currency.dollar_rate,
         transformer=change_val_transformer,
         validate=EmptyInputValidator(),
     )
 
 
 def accumulation_question(
     accumulations: List[Accumulation],
     message: str = "Accumulation",
     default: Optional[Accumulation] = None,
     allow_none: bool = False,
 ) -> ListPrompt:
     no_option = (
-        [Separator(), Choice(value=None, name="No accumulation")]
-        if allow_none
-        else []
+        [Separator(), Choice(value=None, name="No accumulation")] if allow_none else []
     )
 
     return inquirer.select(
         message=message,
         choices=[Choice(a.id, name=a.alias) for a in accumulations]
         + no_option,  # type: ignore
         default=default and default.id,
@@ -240,79 +224,93 @@
         multiselect=True,
         choices=[Choice(t.id, name=t.description) for t in transactions],
     )
 
 
 def interval_question(
     message: str = "Interval",
+    choices: List[str] = ["1h", "1d", "1w", "1M", "1y"],
     default: Optional[str] = None,
 ) -> ListPrompt:
     return inquirer.select(
         message=message,
-        choices=[Choice(i, name=i) for i in ["1d", "1w"]],
+        choices=[Choice(i, name=i) for i in choices],
         default=default,
     )
 
 
 def date_range_question(
     message: str = "Range",
     now: Optional[datetime] = None,
+    default: Optional[Tuple[datetime, datetime]] = None,
     date_fmt: Optional[str] = None,
 ) -> Any:
     class DateRangePrompt:
-        def __init__(self, message: str, now: Optional[datetime] = None):
+        def __init__(
+            self,
+            message: str,
+            now: Optional[datetime] = None,
+            default: Optional[Tuple[datetime, datetime]] = None,
+            date_fmt: Optional[str] = None,
+        ):
             self._message = message
             self._now = now or datetime.now()
             self._date_fmt = "%Y-%m-%d" if date_fmt is None else date_fmt
+            self._default = default
+            self._make_predefined_ranges()
+            self._make_default()
 
         def execute(self) -> Any:
-            last_1d = (self._now - timedelta(days=1), self._now)
-            last_7d = (self._now - timedelta(days=7), self._now)
-            last_30d = (self._now - timedelta(days=30), self._now)
-            last_90d = (self._now - timedelta(days=90), self._now)
-            last_180d = (self._now - timedelta(days=180), self._now)
-            last_365d = (self._now - timedelta(days=365), self._now)
-
-            predefined_ranges = [
-                ("Last day", last_1d),
-                ("Last 7 days", last_7d),
-                ("Last 30 days", last_30d),
-                ("Last 90 days", last_90d),
-                ("Last 180 days", last_180d),
-                ("Last 365 days", last_365d),
-            ]
-
             choices = (
-                [Choice(value, name) for (name, value) in predefined_ranges]
-                + [Separator()]
-                + [
-                    Choice(None, "Custom"),
-                ]
+                [Choice(value, name) for (name, value) in self.predefined_ranges]
+                + [Separator()]  # type: ignore
+                + [Choice(None, "Custom")]
             )
 
             the_range = inquirer.select(
                 message,
                 choices,
-                default=last_1d,
+                default=self._default,
             ).execute()
 
             if the_range is None:
                 return self._custom_range()
 
             return the_range
 
         def _custom_range(self):
             start = date_question(
                 message="Start date",
                 default=self._now,
-                date_fmt=self.date_fmt,
+                date_fmt=self._date_fmt,
             ).execute()
 
             end = date_question(
                 message="End date",
                 default=self._now,
-                date_fmt=self.date_fmt,
+                date_fmt=self._date_fmt,
             ).execute()
 
             return (start, end)
 
-    return DateRangePrompt(message=message, now=now)
+        def _make_predefined_ranges(self):
+            self.last_1d = (self._now - timedelta(days=1), self._now)
+            self.last_7d = (self._now - timedelta(days=7), self._now)
+            self.last_30d = (self._now - timedelta(days=30), self._now)
+            self.last_90d = (self._now - timedelta(days=90), self._now)
+            self.last_180d = (self._now - timedelta(days=180), self._now)
+            self.last_365d = (self._now - timedelta(days=365), self._now)
+
+            self.predefined_ranges = [
+                ("Last day", self.last_1d),
+                ("Last 7 days", self.last_7d),
+                ("Last 30 days", self.last_30d),
+                ("Last 90 days", self.last_90d),
+                ("Last 180 days", self.last_180d),
+                ("Last 365 days", self.last_365d),
+            ]
+
+        def _make_default(self):
+            if self._default is None:
+                self._default = self.last_365d
+
+    return DateRangePrompt(message, now, default, date_fmt)
```

### Comparing `wellets_cli-1.2.0/wellets_cli/util.py` & `wellets_cli-1.5.1/wellets_cli/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from datetime import datetime
 from typing import List, Optional, TypeVar
 
 from dateutil.relativedelta import relativedelta
 
+import wellets_cli.api as api
 from wellets_cli.model import Duration
 
 
 class Resource:
     id: str
 
 
@@ -48,22 +49,27 @@
 
 
 def percent(x: float) -> float:
     return x * 100
 
 
 def pp(
-    x: float, percent=False, decimals=2, fixed=True, with_rounding=True
+    x: float,
+    decimals=2,
+    percent=False,
+    fixed=True,
+    with_symbol=False,
+    with_rounding=False,
 ) -> str:
     if x is None:
         return ""  # ignore None values
 
     # make percentage, if needed
     x = x * 100 if percent else x
-    p = "%" if percent else ""
+    p = "%" if percent and with_symbol else ""
 
     # round x to given number of decimals
     x_rounded = round(x, decimals)
 
     # if the number has been rounded, prefix the result with "~" symbol
     # with_rounding eventually disabled rounding indicator
     is_rounded = with_rounding and x_rounded != x
@@ -110,17 +116,15 @@
 
     if parts is None:
         raise ValueError(
             f"Could not parse duration from '{duration_str}'. Examples of valid strings: '8h', '2d 8h 5m 2s', '2m4.3s'"
         )
 
     duration_params = {
-        name: float(param)
-        for name, param in parts.groupdict().items()
-        if param
+        name: float(param) for name, param in parts.groupdict().items() if param
     }
 
     delta = relativedelta(**duration_params)  # type: ignore
 
     return {
         "years": delta.years,
         "months": delta.months,
@@ -135,17 +139,15 @@
 ### Converters
 
 
 def change_from(from_dollar_rate: float, to_dollar_rate: float) -> float:
     return from_dollar_rate / to_dollar_rate
 
 
-def change_value(
-    from_dollar_rate: float, to_dollar_rate: float, value: float
-) -> float:
+def change_value(from_dollar_rate: float, to_dollar_rate: float, value: float) -> float:
     return 1 / change_from(from_dollar_rate, to_dollar_rate) * value
 
 
 def change_val(from_currency, to_currency, value):
     from_dollar_rate = from_currency.dollar_rate
     to_dollar_rate = to_currency.dollar_rate
     return change_value(from_dollar_rate, to_dollar_rate, value)
```

### Comparing `wellets_cli-1.2.0/wellets_cli/validator.py` & `wellets_cli-1.5.1/wellets_cli/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,15 @@
     if value is not None:
         outcome = validator(value)
         if outcome != True:
             raise ValueError(outcome)
 
 
 def percent_validator(val: str):
-    return (
-        True
-        if float(val) >= 0 and float(val) <= 100
-        else "Should be a percentage"
-    )
+    return True if float(val) >= 0 and float(val) <= 100 else "Should be a percentage"
 
 
 def not_empty_validator(val: str):
     return True if val != "" else "Should not be empty"
 
 
 def number_validator(val: str):
@@ -205,20 +201,44 @@
             raise ValidationError(
                 message=self._message,
                 cursor_position=document.cursor_position,
             )
 
 
 class PasswordMatchValidator(Validator):
-    def __init__(
-        self, password: str, message: str = "Passwords do not match"
-    ) -> None:
+    def __init__(self, password: str, message: str = "Passwords do not match") -> None:
         self._password = password
         self._message = message
 
     def validate(self, document):
         confirm = document.text
         if confirm != self._password:
             raise ValidationError(
                 message=self._message,
                 cursor_position=document.cursor_position,
             )
+
+
+class UrlValidator(Validator):
+    def __init__(
+        self,
+        message: str = "Input should be a URL",
+        scheme: str = None,
+        message_scheme: str = None,
+    ) -> None:
+        self._message = message
+        self._scheme = scheme
+        self._message_scheme = message_scheme
+
+    def validate(self, document):
+        if "://" not in document.text:
+            raise ValidationError(
+                message=self._message,
+                cursor_position=document.cursor_position,
+            )
+
+        if self._scheme is not None:
+            if not document.text.startswith(self._scheme):
+                raise ValidationError(
+                    message=self._message_scheme,
+                    cursor_position=document.cursor_position,
+                )
```

### Comparing `wellets_cli-1.2.0/PKG-INFO` & `wellets_cli-1.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: wellets-cli
-Version: 1.2.0
+Version: 1.5.1
 Summary: wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep under control your money.
 Author: lparolari
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: codecov (>=2.1.13,<3.0.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

