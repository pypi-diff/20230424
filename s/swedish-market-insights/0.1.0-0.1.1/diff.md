# Comparing `tmp/swedish_market_insights-0.1.0.tar.gz` & `tmp/swedish_market_insights-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swedish_market_insights-0.1.0.tar", max compression
+gzip compressed data, was "swedish_market_insights-0.1.1.tar", max compression
```

## Comparing `swedish_market_insights-0.1.0.tar` & `swedish_market_insights-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1301 2023-04-24 11:54:51.112113 swedish_market_insights-0.1.0/README.md
--rw-r--r--   0        0        0      444 2023-04-24 11:56:08.170821 swedish_market_insights-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-19 11:37:17.431866 swedish_market_insights-0.1.0/swedish_market_insights/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-24 12:00:57.790938 swedish_market_insights-0.1.0/swedish_market_insights/ficlient.py
--rw-r--r--   0        0        0      738 2023-04-23 08:12:34.525937 swedish_market_insights-0.1.0/swedish_market_insights/soup_utils.py
--rw-r--r--   0        0        0     1740 2023-04-24 11:51:19.962106 swedish_market_insights-0.1.0/swedish_market_insights/trade.py
--rw-r--r--   0        0        0      565 2023-04-23 08:16:33.495508 swedish_market_insights-0.1.0/swedish_market_insights/utils.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 swedish_market_insights-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-24 11:54:51.112113 swedish_market_insights-0.1.1/README.md
+-rw-r--r--   0        0        0      444 2023-04-24 12:40:24.057779 swedish_market_insights-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-19 11:37:17.431866 swedish_market_insights-0.1.1/swedish_market_insights/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-24 12:40:05.310818 swedish_market_insights-0.1.1/swedish_market_insights/ficlient.py
+-rw-r--r--   0        0        0      739 2023-04-24 12:40:32.707158 swedish_market_insights-0.1.1/swedish_market_insights/soup_utils.py
+-rw-r--r--   0        0        0     1717 2023-04-24 12:40:47.136933 swedish_market_insights-0.1.1/swedish_market_insights/trade.py
+-rw-r--r--   0        0        0      565 2023-04-23 08:16:33.495508 swedish_market_insights-0.1.1/swedish_market_insights/utils.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 swedish_market_insights-0.1.1/PKG-INFO
```

### Comparing `swedish_market_insights-0.1.0/README.md` & `swedish_market_insights-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.0/swedish_market_insights/ficlient.py` & `swedish_market_insights-0.1.1/swedish_market_insights/ficlient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from datetime import date
 
 import requests
 
-from soup_utils import get_trade_entries_from_page, find_href_for_next_page
-from trade import TradeEntry
+from .soup_utils import get_trade_entries_from_page, find_href_for_next_page
+from .trade import TradeEntry
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 BASE_URL = "https://marknadssok.fi.se/Publiceringsklient/sv-SE/Search/Search?"
```

### Comparing `swedish_market_insights-0.1.0/swedish_market_insights/soup_utils.py` & `swedish_market_insights-0.1.1/swedish_market_insights/soup_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bs4 import BeautifulSoup
 
-from trade import TradeEntry
+from .trade import TradeEntry
 
 
 def get_trade_entries_from_page(page: bytes) -> list[TradeEntry]:
     trade_entries = []
     soup = BeautifulSoup(page, "html.parser")
     table_rows = soup.find_all("tr")
     for row in table_rows[1:]:
```

### Comparing `swedish_market_insights-0.1.0/swedish_market_insights/trade.py` & `swedish_market_insights-0.1.1/swedish_market_insights/trade.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from datetime import date
 
-from swedish_market_insights.utils import (
+from .utils import (
     date_from_string,
     is_relative,
     parse_price_from_string,
     parse_volume_from_string,
 )
```

### Comparing `swedish_market_insights-0.1.0/swedish_market_insights/utils.py` & `swedish_market_insights-0.1.1/swedish_market_insights/utils.py`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.0/PKG-INFO` & `swedish_market_insights-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swedish-market-insights
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package to scrape the Finansinspektion's registers
 License: MIT
 Author: Fritjof Bengtsson
 Author-email: fritjof.folkeson@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

