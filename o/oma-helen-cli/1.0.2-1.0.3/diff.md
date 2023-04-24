# Comparing `tmp/oma-helen-cli-1.0.2.tar.gz` & `tmp/oma-helen-cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oma-helen-cli-1.0.2.tar", last modified: Mon Jan 23 20:06:52 2023, max compression
+gzip compressed data, was "oma-helen-cli-1.0.3.tar", last modified: Mon Apr 24 19:09:42 2023, max compression
```

## Comparing `oma-helen-cli-1.0.2.tar` & `oma-helen-cli-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-01-23 20:06:52.530577 oma-helen-cli-1.0.2/
--rw-r--r--   0 caro       (501) staff       (20)     1079 2022-09-09 11:17:34.000000 oma-helen-cli-1.0.2/LICENSE
--rw-r--r--   0 caro       (501) staff       (20)     6476 2023-01-23 20:06:52.530454 oma-helen-cli-1.0.2/PKG-INFO
--rw-r--r--   0 caro       (501) staff       (20)     5674 2023-01-14 21:51:15.000000 oma-helen-cli-1.0.2/README.md
-drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-01-23 20:06:52.525362 oma-helen-cli-1.0.2/helenservice/
--rw-r--r--   0 caro       (501) staff       (20)        0 2022-09-18 16:57:21.000000 oma-helen-cli-1.0.2/helenservice/__init__.py
--rw-r--r--   0 caro       (501) staff       (20)    12250 2023-01-17 18:10:03.000000 oma-helen-cli-1.0.2/helenservice/api_client.py
--rw-r--r--   0 caro       (501) staff       (20)     1038 2023-01-17 18:10:03.000000 oma-helen-cli-1.0.2/helenservice/api_response.py
--rwxr-xr-x   0 caro       (501) staff       (20)     6457 2023-01-14 21:51:15.000000 oma-helen-cli-1.0.2/helenservice/cli.py
--rw-r--r--   0 caro       (501) staff       (20)       22 2022-09-19 18:41:34.000000 oma-helen-cli-1.0.2/helenservice/const.py
--rw-r--r--   0 caro       (501) staff       (20)     5538 2022-09-20 16:14:21.000000 oma-helen-cli-1.0.2/helenservice/helen_session.py
--rw-r--r--   0 caro       (501) staff       (20)     6590 2023-01-14 21:51:15.000000 oma-helen-cli-1.0.2/helenservice/price_client.py
--rw-r--r--   0 caro       (501) staff       (20)      447 2023-01-14 21:51:15.000000 oma-helen-cli-1.0.2/helenservice/utils.py
-drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-01-23 20:06:52.530317 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/
--rw-r--r--   0 caro       (501) staff       (20)     6476 2023-01-23 20:06:52.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/PKG-INFO
--rw-r--r--   0 caro       (501) staff       (20)      490 2023-01-23 20:06:52.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/SOURCES.txt
--rw-r--r--   0 caro       (501) staff       (20)        1 2023-01-23 20:06:52.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/dependency_links.txt
--rw-r--r--   0 caro       (501) staff       (20)       56 2023-01-23 20:06:52.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/entry_points.txt
--rw-r--r--   0 caro       (501) staff       (20)        1 2023-01-14 22:28:51.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/not-zip-safe
--rw-r--r--   0 caro       (501) staff       (20)      121 2023-01-23 20:06:52.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/requires.txt
--rw-r--r--   0 caro       (501) staff       (20)       13 2023-01-23 20:06:52.000000 oma-helen-cli-1.0.2/oma_helen_cli.egg-info/top_level.txt
--rw-r--r--   0 caro       (501) staff       (20)       38 2023-01-23 20:06:52.530612 oma-helen-cli-1.0.2/setup.cfg
--rw-r--r--   0 caro       (501) staff       (20)     1562 2023-01-23 19:57:08.000000 oma-helen-cli-1.0.2/setup.py
+drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-04-24 19:09:42.323016 oma-helen-cli-1.0.3/
+-rw-r--r--   0 caro       (501) staff       (20)     1079 2022-09-09 11:17:34.000000 oma-helen-cli-1.0.3/LICENSE
+-rw-r--r--   0 caro       (501) staff       (20)     6648 2023-04-24 19:09:42.322884 oma-helen-cli-1.0.3/PKG-INFO
+-rw-r--r--   0 caro       (501) staff       (20)     5846 2023-04-24 19:04:33.000000 oma-helen-cli-1.0.3/README.md
+drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-04-24 19:09:42.310481 oma-helen-cli-1.0.3/helenservice/
+-rw-r--r--   0 caro       (501) staff       (20)        0 2022-09-18 16:57:21.000000 oma-helen-cli-1.0.3/helenservice/__init__.py
+-rw-r--r--   0 caro       (501) staff       (20)    13751 2023-04-24 18:00:21.000000 oma-helen-cli-1.0.3/helenservice/api_client.py
+-rw-r--r--   0 caro       (501) staff       (20)       54 2023-04-24 17:38:45.000000 oma-helen-cli-1.0.3/helenservice/api_exceptions.py
+-rw-r--r--   0 caro       (501) staff       (20)     1038 2023-01-17 18:10:03.000000 oma-helen-cli-1.0.3/helenservice/api_response.py
+-rwxr-xr-x   0 caro       (501) staff       (20)     6486 2023-04-24 18:48:11.000000 oma-helen-cli-1.0.3/helenservice/cli.py
+-rw-r--r--   0 caro       (501) staff       (20)       22 2022-09-19 18:41:34.000000 oma-helen-cli-1.0.3/helenservice/const.py
+-rw-r--r--   0 caro       (501) staff       (20)     5538 2022-09-20 16:14:21.000000 oma-helen-cli-1.0.3/helenservice/helen_session.py
+-rw-r--r--   0 caro       (501) staff       (20)     5324 2023-04-24 17:25:36.000000 oma-helen-cli-1.0.3/helenservice/price_client.py
+-rw-r--r--   0 caro       (501) staff       (20)      447 2023-01-14 21:51:15.000000 oma-helen-cli-1.0.3/helenservice/utils.py
+drwxr-xr-x   0 caro       (501) staff       (20)        0 2023-04-24 19:09:42.322728 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/
+-rw-r--r--   0 caro       (501) staff       (20)     6648 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/PKG-INFO
+-rw-r--r--   0 caro       (501) staff       (20)      521 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 caro       (501) staff       (20)        1 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 caro       (501) staff       (20)       56 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/entry_points.txt
+-rw-r--r--   0 caro       (501) staff       (20)        1 2023-01-14 22:28:51.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/not-zip-safe
+-rw-r--r--   0 caro       (501) staff       (20)      121 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/requires.txt
+-rw-r--r--   0 caro       (501) staff       (20)       13 2023-04-24 19:09:42.000000 oma-helen-cli-1.0.3/oma_helen_cli.egg-info/top_level.txt
+-rw-r--r--   0 caro       (501) staff       (20)       38 2023-04-24 19:09:42.323050 oma-helen-cli-1.0.3/setup.cfg
+-rw-r--r--   0 caro       (501) staff       (20)     1562 2023-04-24 19:08:01.000000 oma-helen-cli-1.0.3/setup.py
```

### Comparing `oma-helen-cli-1.0.2/LICENSE` & `oma-helen-cli-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.2/PKG-INFO` & `oma-helen-cli-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oma-helen-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Oma Helen API library and CLI
 Home-page: https://github.com/carohauta/oma-helen-cli
 Author: carohauta
 Author-email: carosoft.dev@gmail.com
 License: MIT license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,23 @@
 
 ### What is Oma Helen?
 
 Oma Helen is the user portal for a Finnish electricity company, Helen Oy.
 
 ### How to use and develop
 
+Install from [pypi](https://pypi.org/project/oma-helen-cli/): 
+```sh
+pip install oma-helen-cli
+```
+
+#### Installing from sources and running the project
+
+First clone this repo.
+
 Use virtual env to keep the project isolated. Developed using Python 3.9.9
 
 1. In the project root folder run `python -m venv .venv`
 2. Activate the venv with `source .venv/bin/activate`
 3. Install requirements `pip install -r requirements.txt`
 4. Launch the CLI as a python module `python -m helenservice.cli`
 5. Enter your username and password as they are prompted
@@ -53,15 +62,15 @@
 | get_contract_delivery_site_id | Get the delivery site id from the contract data |
 | get_daily_measurements_json   | Returns your daily energy consumption for the on-going month of the on-going year as JSON |
 | get_market_prices_json        | Returns the prices for the Market Price Electricity contract as JSON. The JSON includes the price for last month, the current month and next month if available |
 | get_monthly_measurements_json | Returns your monthly energy consumption for the on-going year as JSON |
 | calculate_the_impact_of_usage_between_dates | Calculates your impact of usage between given dates for the Helen Smart Electricity Guarantee |
 | calculate_spot_cost_between_dates | Calculates the total costs between given dates of a spot price contract in an hourly precision |
 | get_exchange_margin_price_json | Get the margin price of the Exchange Electricity contract |
-| get_smart_guarantee_price_json | Get the c/kwh price of the Smart Guarantee Electricity contract |
+| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data |
 
 ### Oma Helen API example
 
 In this example, in addition to the `access-token`, you are going to need your delivery site id (`Consumption` or `Käyttöpaikka`) from Oma Helen. You can get it with the CLI tool's `get_contract_delivery_site_id` function.
 
 #### Making a request
```

### Comparing `oma-helen-cli-1.0.2/README.md` & `oma-helen-cli-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 
 ### What is Oma Helen?
 
 Oma Helen is the user portal for a Finnish electricity company, Helen Oy.
 
 ### How to use and develop
 
+Install from [pypi](https://pypi.org/project/oma-helen-cli/): 
+```sh
+pip install oma-helen-cli
+```
+
+#### Installing from sources and running the project
+
+First clone this repo.
+
 Use virtual env to keep the project isolated. Developed using Python 3.9.9
 
 1. In the project root folder run `python -m venv .venv`
 2. Activate the venv with `source .venv/bin/activate`
 3. Install requirements `pip install -r requirements.txt`
 4. Launch the CLI as a python module `python -m helenservice.cli`
 5. Enter your username and password as they are prompted
@@ -31,15 +40,15 @@
 | get_contract_delivery_site_id | Get the delivery site id from the contract data |
 | get_daily_measurements_json   | Returns your daily energy consumption for the on-going month of the on-going year as JSON |
 | get_market_prices_json        | Returns the prices for the Market Price Electricity contract as JSON. The JSON includes the price for last month, the current month and next month if available |
 | get_monthly_measurements_json | Returns your monthly energy consumption for the on-going year as JSON |
 | calculate_the_impact_of_usage_between_dates | Calculates your impact of usage between given dates for the Helen Smart Electricity Guarantee |
 | calculate_spot_cost_between_dates | Calculates the total costs between given dates of a spot price contract in an hourly precision |
 | get_exchange_margin_price_json | Get the margin price of the Exchange Electricity contract |
-| get_smart_guarantee_price_json | Get the c/kwh price of the Smart Guarantee Electricity contract |
+| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data |
 
 ### Oma Helen API example
 
 In this example, in addition to the `access-token`, you are going to need your delivery site id (`Consumption` or `Käyttöpaikka`) from Oma Helen. You can get it with the CLI tool's `get_contract_delivery_site_id` function.
 
 #### Making a request
```

### Comparing `oma-helen-cli-1.0.2/helenservice/api_client.py` & `oma-helen-cli-1.0.3/helenservice/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from cachetools import cached, TTLCache
-import json
+import json, logging
 from datetime import date, datetime, timedelta
+
+from helenservice.api_exceptions import InvalidApiResponseException
 from .api_response import MeasurementResponse, SpotPricesResponse
 from .const import HTTP_READ_TIMEOUT
 from .helen_session import HelenSession
 from requests import get
 from dateutil.relativedelta import relativedelta
 
 
@@ -223,17 +225,37 @@
 
         return self.get_contract_data_json()[0]["delivery_site"]["id"]
 
     def get_contract_base_price(self) -> int:
         """Get the contract base price from your contract data."""
         
         contract_data = self.get_contract_data_json()
-        contract_components = contract_data[0]["products"][0]["components"]
-        base_price_component = next(filter(lambda component: component["is_base_price"], contract_components))
+        contract = contract_data[0] if contract_data else None
+        if not contract: raise InvalidApiResponseException("Contract data is empty or None")
+        products = contract["products"] if contract else []
+        product = products[0] if products else None
+        if not product: raise InvalidApiResponseException("Product data is empty or None")
+        components = product["components"] if product else []
+        base_price_component = next(filter(lambda component: component["is_base_price"], components), None)
+        if base_price_component is None: raise InvalidApiResponseException("Could not resolve contract base price from Helen API response")
         return base_price_component["price"]
+    
+    def get_contract_energy_unit_price(self) -> int:
+        """Get the unit price for electricity from your contract data."""
+        
+        contract_data = self.get_contract_data_json()
+        contract = contract_data[0] if contract_data else None
+        if not contract: raise InvalidApiResponseException("Contract data is empty or None")
+        products = contract["products"] if contract else []
+        product = products[0] if products else None
+        if not product: raise InvalidApiResponseException("Product data is empty or None")
+        components = product["components"] if product else []
+        energy_unit_price_component = next(filter(lambda component: component["name"] == "Energia", components), None)
+        if energy_unit_price_component is None: raise InvalidApiResponseException("Could not resolve energy unit price from Helen API contract response")
+        return energy_unit_price_component["price"]
 
     def get_api_access_token(self):
         return self._session.get_access_token()
 
     def _api_request_headers(self):
         return {
             "Authorization": f"Bearer {self.get_api_access_token()}",
```

### Comparing `oma-helen-cli-1.0.2/helenservice/api_response.py` & `oma-helen-cli-1.0.3/helenservice/api_response.py`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.2/helenservice/cli.py` & `oma-helen-cli-1.0.3/helenservice/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,21 +109,14 @@
     def do_get_market_prices_json(self, input=None):
         """Get prices for the Market Price contract type as JSON"""
 
         price = self.helen_price_client.get_market_price_prices()
         price_json = json.dumps(price, default=_json_serializer, indent=2)
         print(price_json)
 
-    def do_get_smart_guarantee_price_json(self, input=None):
-        """Get price for the Smart Guarantee contract type as JSON"""
-
-        price = self.helen_price_client.get_smart_guarantee_prices()
-        price_json = json.dumps(price, default=_json_serializer, indent=2)
-        print(price_json)
-
     def do_get_exchange_margin_price_json(self, input=None):
         """Get margin price for the Exchange Electricity contract type as JSON"""
 
         price = self.helen_price_client.get_exchange_prices()
         price_json = json.dumps(price, default=_json_serializer, indent=2)
         print(price_json)
 
@@ -141,14 +134,19 @@
 
     def do_get_api_access_token(self, input=None):
         """Get your access token for the Oma Helen API."""
         
         access_token = self.api_client.get_api_access_token()
         print(access_token)
 
+    def do_get_contract_energy_unit_price(self, input=None):
+        """Helper to get the energy unit price from your contract data. To see the whole contract data as JSON, use get_contract_data_json"""
+
+        contract_energy_unit_price = self.api_client.get_contract_energy_unit_price()
+        print(contract_energy_unit_price)
 
 def main():
     print("Log in to Oma Helen")
     username = input("Username: ")
     password = getpass()
     HelenCLIPrompt(username, password).cmdloop()
```

### Comparing `oma-helen-cli-1.0.2/helenservice/helen_session.py` & `oma-helen-cli-1.0.3/helenservice/helen_session.py`

 * *Files identical despite different names*

### Comparing `oma-helen-cli-1.0.2/helenservice/price_client.py` & `oma-helen-cli-1.0.3/helenservice/price_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,44 +35,32 @@
     def __init__(self, last_month, current_month, next_month):
         super().__init__()
         self.last_month: float = last_month
         self.current_month: float = current_month
         self.next_month: float = next_month
 
 
-class HelenSmartGuaranteePrices(HelenPrices):
-    def __init__(self, price):
-        super().__init__()
-        self.price: float = price
-
-
 class HelenExchangePrices(HelenPrices):
     def __init__(self, margin):
         super().__init__()
         self.margin: float = margin
 
 
 class HelenPriceClient:
     MARKET_PRICE_ELECTRICITY_URL = "https://www.helen.fi/sahko/sahkosopimus/markkinahinta"
-    SMART_ELECTRICITY_GUARANTEE_URL = "https://www.helen.fi/sahko/sahkosopimus/fiksusahko-takuu"
     EXCHANGE_ELECTRICITY_URL = "https://www.helen.fi/sahko/sahkosopimus/porssisahko"
 
     _helen_market_price_prices: HelenMarketPrices = None
-    _helen_smart_guarantee_prices: HelenSmartGuaranteePrices = None
     _helen_exchange_prices: HelenExchangePrices = None
         
 
     def _are_market_price_prices_valid(self):
         return self._is_helen_prices_valid(self._helen_market_price_prices)
 
 
-    def _are_smart_guarantee_prices_valid(self):
-        return self._is_helen_prices_valid(self._helen_smart_guarantee_prices)
-
-
     def _are_exchange_prices_valid(self):
         return self._is_helen_prices_valid(self._helen_exchange_prices)
 
     
     def _is_helen_prices_valid(self, helen_prices: HelenPrices):
         """If the latest price scrape has happened within the last hour, then use cache"""
 
@@ -118,34 +106,14 @@
             return self._helen_market_price_prices
         last_month_price, current_month_price, next_month_price = self._scrape_market_price_prices()
 
         self._helen_market_price_prices = HelenMarketPrices(last_month_price, current_month_price, next_month_price)
         return self._helen_market_price_prices
 
 
-    def _scrape_smart_guarantee_prices(self):
-        price_site_response = get(self.SMART_ELECTRICITY_GUARANTEE_URL, timeout=HTTP_READ_TIMEOUT)
-        price_site_soup = BeautifulSoup(price_site_response.text, "html.parser")
-
-        element = price_site_soup.select_one(f'span.product-info-block__data--price')
-        price = element.text
-
-        return float(price.replace(",", "."))
-
-
-    def get_smart_guarantee_prices(self) -> HelenSmartGuaranteePrices:
-        """Get the current price (c/kwh) for the Smart Guarantee contract"""
-        if self._are_smart_guarantee_prices_valid():
-            return self._helen_smart_guarantee_prices
-        price = self._scrape_smart_guarantee_prices()
-
-        self._helen_smart_guarantee_prices = HelenSmartGuaranteePrices(price)
-        return self._helen_smart_guarantee_prices
-
-
     def _scrape_exchange_prices(self):
         price_site_response = get(self.EXCHANGE_ELECTRICITY_URL, timeout=HTTP_READ_TIMEOUT)
         price_site_soup = BeautifulSoup(price_site_response.text, "html.parser")
 
         element = price_site_soup.select_one(f'span.product-info-block__data--price')
         margin = element.text
```

### Comparing `oma-helen-cli-1.0.2/oma_helen_cli.egg-info/PKG-INFO` & `oma-helen-cli-1.0.3/oma_helen_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oma-helen-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Oma Helen API library and CLI
 Home-page: https://github.com/carohauta/oma-helen-cli
 Author: carohauta
 Author-email: carosoft.dev@gmail.com
 License: MIT license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,23 @@
 
 ### What is Oma Helen?
 
 Oma Helen is the user portal for a Finnish electricity company, Helen Oy.
 
 ### How to use and develop
 
+Install from [pypi](https://pypi.org/project/oma-helen-cli/): 
+```sh
+pip install oma-helen-cli
+```
+
+#### Installing from sources and running the project
+
+First clone this repo.
+
 Use virtual env to keep the project isolated. Developed using Python 3.9.9
 
 1. In the project root folder run `python -m venv .venv`
 2. Activate the venv with `source .venv/bin/activate`
 3. Install requirements `pip install -r requirements.txt`
 4. Launch the CLI as a python module `python -m helenservice.cli`
 5. Enter your username and password as they are prompted
@@ -53,15 +62,15 @@
 | get_contract_delivery_site_id | Get the delivery site id from the contract data |
 | get_daily_measurements_json   | Returns your daily energy consumption for the on-going month of the on-going year as JSON |
 | get_market_prices_json        | Returns the prices for the Market Price Electricity contract as JSON. The JSON includes the price for last month, the current month and next month if available |
 | get_monthly_measurements_json | Returns your monthly energy consumption for the on-going year as JSON |
 | calculate_the_impact_of_usage_between_dates | Calculates your impact of usage between given dates for the Helen Smart Electricity Guarantee |
 | calculate_spot_cost_between_dates | Calculates the total costs between given dates of a spot price contract in an hourly precision |
 | get_exchange_margin_price_json | Get the margin price of the Exchange Electricity contract |
-| get_smart_guarantee_price_json | Get the c/kwh price of the Smart Guarantee Electricity contract |
+| get_contract_energy_unit_price | Get the energy unit price (c/kwh) from your contract data |
 
 ### Oma Helen API example
 
 In this example, in addition to the `access-token`, you are going to need your delivery site id (`Consumption` or `Käyttöpaikka`) from Oma Helen. You can get it with the CLI tool's `get_contract_delivery_site_id` function.
 
 #### Making a request
```

### Comparing `oma-helen-cli-1.0.2/setup.py` & `oma-helen-cli-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     install_requires=requirements,
     license="MIT license",
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(include=['helenservice', 'helenservice.*']),
     url='https://github.com/carohauta/oma-helen-cli',
-    version='1.0.2',
+    version='1.0.3',
     zip_safe=False,
 )
```

