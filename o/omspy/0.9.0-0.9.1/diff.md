# Comparing `tmp/omspy-0.9.0.tar.gz` & `tmp/omspy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omspy-0.9.0.tar", max compression
+gzip compressed data, was "omspy-0.9.1.tar", max compression
```

## Comparing `omspy-0.9.0.tar` & `omspy-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1076 2021-12-31 13:47:58.134124 omspy-0.9.0/LICENSE
--rw-r--r--   0        0        0      109 2021-12-31 13:47:58.134124 omspy-0.9.0/README.md
--rw-r--r--   0        0        0       22 2021-12-31 13:47:58.134124 omspy-0.9.0/omspy/__init__.py
--rw-r--r--   0        0        0      215 2022-05-03 13:56:12.928580 omspy-0.9.0/omspy/algos/README.md
--rw-r--r--   0        0        0     7670 2022-11-01 16:42:57.099765 omspy-0.9.0/omspy/algos/straddle.py
--rw-r--r--   0        0        0    10724 2022-11-05 15:05:39.145365 omspy-0.9.0/omspy/base.py
--rw-r--r--   0        0        0     2748 2022-11-01 16:42:55.223804 omspy-0.9.0/omspy/brokers/api_helper.py
--rw-r--r--   0        0        0     6031 2022-11-18 03:14:43.933558 omspy-0.9.0/omspy/brokers/finvasia.py
--rw-r--r--   0        0        0      775 2022-11-05 08:29:42.521928 omspy-0.9.0/omspy/brokers/finvasia.yaml
--rw-r--r--   0        0        0     6653 2021-12-31 13:47:58.134124 omspy-0.9.0/omspy/brokers/fyers.py
--rw-r--r--   0        0        0      543 2021-12-31 13:47:58.134124 omspy-0.9.0/omspy/brokers/fyers.yaml
--rw-r--r--   0        0        0    11538 2022-11-17 15:44:48.879614 omspy-0.9.0/omspy/brokers/kotak.py
--rw-r--r--   0        0        0      275 2022-11-17 15:44:49.483607 omspy-0.9.0/omspy/brokers/kotak.yaml
--rw-r--r--   0        0        0    25471 2022-10-25 15:16:28.775080 omspy-0.9.0/omspy/brokers/master_trust.py
--rw-r--r--   0        0        0      577 2021-12-31 13:47:58.134124 omspy-0.9.0/omspy/brokers/master_trust.yaml
--rw-r--r--   0        0        0     1162 2022-03-19 13:33:23.146972 omspy-0.9.0/omspy/brokers/paper.py
--rw-r--r--   0        0        0      116 2021-12-31 13:47:58.138124 omspy-0.9.0/omspy/brokers/paper.yaml
--rw-r--r--   0        0        0     7707 2022-08-24 15:44:48.608120 omspy-0.9.0/omspy/brokers/zerodha.py
--rw-r--r--   0        0        0      186 2021-12-31 13:47:58.138124 omspy-0.9.0/omspy/brokers/zerodha.yaml
--rw-r--r--   0        0        0    12255 2022-11-01 16:42:59.775709 omspy-0.9.0/omspy/models.py
--rw-r--r--   0        0        0     4253 2022-10-27 06:05:20.631405 omspy-0.9.0/omspy/multi.py
--rw-r--r--   0        0        0    21744 2022-11-05 12:06:26.403067 omspy-0.9.0/omspy/order.py
--rw-r--r--   0        0        0     1006 2022-10-27 06:05:20.631405 omspy-0.9.0/omspy/orders/depth.py
--rw-r--r--   0        0        0    11114 2022-11-05 14:34:46.750028 omspy-0.9.0/omspy/orders/peg.py
--rw-r--r--   0        0        0     4380 2022-11-17 14:44:10.611206 omspy-0.9.0/omspy/orders/stop.py
--rw-r--r--   0        0        0     3008 2022-04-27 11:30:28.255509 omspy-0.9.0/omspy/utils.py
--rw-r--r--   0        0        0      826 2022-11-18 03:18:31.252314 omspy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 omspy-0.9.0/setup.py
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 omspy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-12-31 13:47:58.134124 omspy-0.9.1/LICENSE
+-rw-r--r--   0        0        0      109 2021-12-31 13:47:58.134124 omspy-0.9.1/README.md
+-rw-r--r--   0        0        0       22 2021-12-31 13:47:58.134124 omspy-0.9.1/omspy/__init__.py
+-rw-r--r--   0        0        0      215 2022-05-03 13:56:12.928580 omspy-0.9.1/omspy/algos/README.md
+-rw-r--r--   0        0        0     7670 2022-11-01 16:42:57.099765 omspy-0.9.1/omspy/algos/straddle.py
+-rw-r--r--   0        0        0    10724 2022-11-05 15:05:39.145365 omspy-0.9.1/omspy/base.py
+-rw-r--r--   0        0        0     2748 2022-11-01 16:42:55.223804 omspy-0.9.1/omspy/brokers/api_helper.py
+-rw-r--r--   0        0        0     6705 2022-11-30 11:26:34.224135 omspy-0.9.1/omspy/brokers/finvasia.py
+-rw-r--r--   0        0        0      865 2022-11-30 13:08:26.780299 omspy-0.9.1/omspy/brokers/finvasia.yaml
+-rw-r--r--   0        0        0     6653 2021-12-31 13:47:58.134124 omspy-0.9.1/omspy/brokers/fyers.py
+-rw-r--r--   0        0        0      543 2021-12-31 13:47:58.134124 omspy-0.9.1/omspy/brokers/fyers.yaml
+-rw-r--r--   0        0        0    11749 2022-11-30 13:08:29.012274 omspy-0.9.1/omspy/brokers/kotak.py
+-rw-r--r--   0        0        0      353 2022-11-30 12:50:06.560487 omspy-0.9.1/omspy/brokers/kotak.yaml
+-rw-r--r--   0        0        0    25471 2022-10-25 15:16:28.775080 omspy-0.9.1/omspy/brokers/master_trust.py
+-rw-r--r--   0        0        0      577 2021-12-31 13:47:58.134124 omspy-0.9.1/omspy/brokers/master_trust.yaml
+-rw-r--r--   0        0        0     1162 2022-03-19 13:33:23.146972 omspy-0.9.1/omspy/brokers/paper.py
+-rw-r--r--   0        0        0      116 2021-12-31 13:47:58.138124 omspy-0.9.1/omspy/brokers/paper.yaml
+-rw-r--r--   0        0        0     7707 2022-08-24 15:44:48.608120 omspy-0.9.1/omspy/brokers/zerodha.py
+-rw-r--r--   0        0        0      186 2021-12-31 13:47:58.138124 omspy-0.9.1/omspy/brokers/zerodha.yaml
+-rw-r--r--   0        0        0    12255 2022-11-01 16:42:59.775709 omspy-0.9.1/omspy/models.py
+-rw-r--r--   0        0        0     4253 2022-10-27 06:05:20.631405 omspy-0.9.1/omspy/multi.py
+-rw-r--r--   0        0        0    21744 2022-11-05 12:06:26.403067 omspy-0.9.1/omspy/order.py
+-rw-r--r--   0        0        0     1006 2022-10-27 06:05:20.631405 omspy-0.9.1/omspy/orders/depth.py
+-rw-r--r--   0        0        0    11114 2022-11-05 14:34:46.750028 omspy-0.9.1/omspy/orders/peg.py
+-rw-r--r--   0        0        0     4380 2022-11-17 14:44:10.611206 omspy-0.9.1/omspy/orders/stop.py
+-rw-r--r--   0        0        0     3008 2022-04-27 11:30:28.255509 omspy-0.9.1/omspy/utils.py
+-rw-r--r--   0        0        0      826 2022-11-30 13:10:51.786692 omspy-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 omspy-0.9.1/setup.py
+-rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 omspy-0.9.1/PKG-INFO
```

### Comparing `omspy-0.9.0/LICENSE` & `omspy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/algos/straddle.py` & `omspy-0.9.1/omspy/algos/straddle.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/base.py` & `omspy-0.9.1/omspy/base.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/api_helper.py` & `omspy-0.9.1/omspy/brokers/api_helper.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/finvasia.py` & `omspy-0.9.1/omspy/brokers/finvasia.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,18 +45,21 @@
         """
         return self.login()
 
     def _convert_symbol(self, symbol: str, exchange: str = "NSE") -> str:
         """
         Convert raw symbol to finvasia
         """
-        if symbol.endswith("-EQ") or symbol.endswith("-eq"):
-            return symbol
+        if exchange == "NSE":
+            if symbol.endswith("-EQ") or symbol.endswith("-eq"):
+                return symbol
+            else:
+                return f"{symbol}-EQ"
         else:
-            return f"{symbol}-EQ"
+            return symbol
 
     @property
     @post
     def orders(self) -> List[Dict]:
         orderbook = self.finvasia.get_order_book()
         if len(orderbook) == 0:
             return orderbook
@@ -67,36 +70,58 @@
         for order in orderbook:
             try:
                 for int_col in int_cols:
                     order[int_col] = int(order.get(int_col, 0))
                 for float_col in float_cols:
                     order[float_col] = float(order.get(float_col, 0))
                 ts = order["exch_tm"]
-                order["exchange_timestamp"] = pendulum.from_format(
-                    ts, fmt="DD-MM-YYYY HH:mm:ss", tz="Asia/Kolkata"
+                # Timestamp converted to str to facilitate loading into pandas dataframe
+                order["exchange_timestamp"] = str(
+                    pendulum.from_format(
+                        ts, fmt="DD-MM-YYYY HH:mm:ss", tz="Asia/Kolkata"
+                    )
                 )
                 ts2 = order["norentm"]
-                order["broker_timestamp"] = pendulum.from_format(
-                    ts2, fmt="HH:mm:ss DD-MM-YYYY", tz="Asia/Kolkata"
+                order["broker_timestamp"] = str(
+                    pendulum.from_format(
+                        ts2, fmt="HH:mm:ss DD-MM-YYYY", tz="Asia/Kolkata"
+                    )
                 )
             except Exception as e:
                 logging.error(e)
             order_list.append(order)
         return order_list
 
     @property
     @post
     def positions(self) -> List[Dict]:
         positionbook = self.finvasia.get_positions()
         if len(positionbook) == 0:
             return positionbook
 
         position_list = []
-        int_cols = ["netqty", "daybuyqty", "daysellqty"]
-        float_cols = ["daybuyamt", "daysellamt"]
+        int_cols = [
+            "netqty",
+            "daybuyqty",
+            "daysellqty",
+            "cfbuyqty",
+            "cfsellqty",
+            "openbuyqty",
+            "opensellqty",
+        ]
+        float_cols = [
+            "daybuyamt",
+            "daysellamt",
+            "lp",
+            "rpnl",
+            "dayavgprc",
+            "daybuyavgprc",
+            "daysellavgprc",
+            "urmtom",
+        ]
         for position in positionbook:
             try:
                 for int_col in int_cols:
                     position[int_col] = int(position.get(int_col, 0))
                 for float_col in float_cols:
                     position[float_col] = float(position.get(float_col, 0))
             except Exception as e:
@@ -136,29 +161,30 @@
         )
         order_types["SL-M"] = "SL-MKT"
         order_types["SL-L"] = "SL-LMT"
         return order_types.get(order_type.upper(), "MKT")
 
     @pre
     def order_place(self, **kwargs) -> Union[str, None]:
-        symbol = kwargs.pop("symbol")
-        symbol = self._convert_symbol(symbol)
         side = kwargs.pop("side")
         order_type = kwargs.pop("order_type", "MKT")
+        exchange = kwargs.pop("exchange", "NSE")
+        symbol = kwargs.pop("symbol")
+        symbol = self._convert_symbol(symbol, exchange=exchange)
         if order_type:
             order_type = self.get_order_type(order_type)
         if side:
             side = side.upper()[0]
         if symbol:
             symbol = symbol.upper()
         order_args = dict(
             tradingsymbol=symbol,
             buy_or_sell=side,
             price_type=order_type,
-            exchange="NSE",
+            exchange=exchange,
             retention="DAY",
             product_type="I",
             discloseqty=0,
         )
         order_args.update(kwargs)
         return self.finvasia.place_order(**order_args)
```

### Comparing `omspy-0.9.0/omspy/brokers/finvasia.yaml` & `omspy-0.9.1/omspy/brokers/finvasia.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,18 @@
   quantity: newquantity
   price: newprice
   trigger_price: newtrigger_price
   symbol: tradingsymbol
 positions:
   tsym: symbol
   netqty: quantity
+  lp: last_price
+  exch: exchange
+  daybuyamt: day_buy_value
+  daysellamt: day_sell_value
 orders:
   tsym: symbol
   qty: quantity
   trantype: side
   ret: validity
   prc: price
   trgprc: trigger_price
```

### Comparing `omspy-0.9.0/omspy/brokers/fyers.py` & `omspy-0.9.1/omspy/brokers/fyers.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/fyers.yaml` & `omspy-0.9.1/omspy/brokers/fyers.yaml`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/kotak.py` & `omspy-0.9.1/omspy/brokers/kotak.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,33 +146,42 @@
             )
         ]
         return data
     else:
         return data
 
 
+def _create_instrument_dataframe() -> pd.DataFrame:
+    """
+    Create the instrument dataframe
+    """
+    # TODO: Handle error in case of no instruments
+    cash = download_file(get_url(segment="cash"))
+    fno = download_file(get_url(segment="fno"))
+    cash = add_name(cash, segment="cash")
+    fno = add_name(fno, segment="fno")
+    df = pd.concat([cash, fno]).drop_duplicates(subset=["instrumenttoken"])
+    return df
+
+
 def create_instrument_master(
     name: str = "inst_name", token: str = "instrumenttoken"
 ) -> Dict[str, int]:
     """
     Create the instrument master
     name
         column name representing the symbol column
     token
         column name representing the token
     Note
     ----
     Takes no arguments by default and returns the entire instrument_master as a dictionary with key as name and values as instrument token
     """
     # TODO: Handle error in case of no instruments
-    cash = download_file(get_url(segment="cash"))
-    fno = download_file(get_url(segment="fno"))
-    cash = add_name(cash, segment="cash")
-    fno = add_name(fno, segment="fno")
-    df = pd.concat([cash, fno]).drop_duplicates(subset=["instrumenttoken"])
+    df = _create_instrument_dataframe()
     return {k: int(v) for k, v in zip(df[name].values, df[token].values)}
 
 
 class Kotak(Broker):
     """
     Automated Trading class
     """
```

### Comparing `omspy-0.9.0/omspy/brokers/master_trust.py` & `omspy-0.9.1/omspy/brokers/master_trust.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/master_trust.yaml` & `omspy-0.9.1/omspy/brokers/master_trust.yaml`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/paper.py` & `omspy-0.9.1/omspy/brokers/paper.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/brokers/zerodha.py` & `omspy-0.9.1/omspy/brokers/zerodha.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/models.py` & `omspy-0.9.1/omspy/models.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/multi.py` & `omspy-0.9.1/omspy/multi.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/order.py` & `omspy-0.9.1/omspy/order.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/orders/depth.py` & `omspy-0.9.1/omspy/orders/depth.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/orders/peg.py` & `omspy-0.9.1/omspy/orders/peg.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/orders/stop.py` & `omspy-0.9.1/omspy/orders/stop.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/omspy/utils.py` & `omspy-0.9.1/omspy/utils.py`

 * *Files identical despite different names*

### Comparing `omspy-0.9.0/pyproject.toml` & `omspy-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omspy"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 license = "MIT"
 authors = ["Ubermensch <uberdeveloper001@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/uberdeveloper/omspy"
 
 [tool.poetry.dependencies]
```

### Comparing `omspy-0.9.0/setup.py` & `omspy-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['PyYAML>=5.4.1,<6.0.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'sqlite-utils>=3.22.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'omspy',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': '',
     'long_description': '# Omspy\n\nomspy is a broker agnostic order management system with a common api, advanced order types and more\n',
     'author': 'Ubermensch',
     'author_email': 'uberdeveloper001@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/uberdeveloper/omspy',
```

### Comparing `omspy-0.9.0/PKG-INFO` & `omspy-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omspy
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Home-page: https://github.com/uberdeveloper/omspy
 License: MIT
 Author: Ubermensch
 Author-email: uberdeveloper001@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

