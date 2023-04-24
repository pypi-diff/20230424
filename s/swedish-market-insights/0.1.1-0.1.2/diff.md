# Comparing `tmp/swedish_market_insights-0.1.1.tar.gz` & `tmp/swedish_market_insights-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swedish_market_insights-0.1.1.tar", max compression
+gzip compressed data, was "swedish_market_insights-0.1.2.tar", max compression
```

## Comparing `swedish_market_insights-0.1.1.tar` & `swedish_market_insights-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1301 2023-04-24 11:54:51.112113 swedish_market_insights-0.1.1/README.md
--rw-r--r--   0        0        0      444 2023-04-24 12:40:24.057779 swedish_market_insights-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-19 11:37:17.431866 swedish_market_insights-0.1.1/swedish_market_insights/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-24 12:40:05.310818 swedish_market_insights-0.1.1/swedish_market_insights/ficlient.py
--rw-r--r--   0        0        0      739 2023-04-24 12:40:32.707158 swedish_market_insights-0.1.1/swedish_market_insights/soup_utils.py
--rw-r--r--   0        0        0     1717 2023-04-24 12:40:47.136933 swedish_market_insights-0.1.1/swedish_market_insights/trade.py
--rw-r--r--   0        0        0      565 2023-04-23 08:16:33.495508 swedish_market_insights-0.1.1/swedish_market_insights/utils.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 swedish_market_insights-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-24 11:54:51.112113 swedish_market_insights-0.1.2/README.md
+-rw-r--r--   0        0        0      550 2023-04-24 12:49:57.525642 swedish_market_insights-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-19 11:37:17.431866 swedish_market_insights-0.1.2/swedish_market_insights/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-24 12:40:05.310818 swedish_market_insights-0.1.2/swedish_market_insights/ficlient.py
+-rw-r--r--   0        0        0      739 2023-04-24 12:40:32.707158 swedish_market_insights-0.1.2/swedish_market_insights/soup_utils.py
+-rw-r--r--   0        0        0     1717 2023-04-24 12:40:47.136933 swedish_market_insights-0.1.2/swedish_market_insights/trade.py
+-rw-r--r--   0        0        0      565 2023-04-23 08:16:33.495508 swedish_market_insights-0.1.2/swedish_market_insights/utils.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 swedish_market_insights-0.1.2/PKG-INFO
```

### Comparing `swedish_market_insights-0.1.1/README.md` & `swedish_market_insights-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.1/swedish_market_insights/ficlient.py` & `swedish_market_insights-0.1.2/swedish_market_insights/ficlient.py`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.1/swedish_market_insights/soup_utils.py` & `swedish_market_insights-0.1.2/swedish_market_insights/soup_utils.py`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.1/swedish_market_insights/trade.py` & `swedish_market_insights-0.1.2/swedish_market_insights/trade.py`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.1/swedish_market_insights/utils.py` & `swedish_market_insights-0.1.2/swedish_market_insights/utils.py`

 * *Files identical despite different names*

### Comparing `swedish_market_insights-0.1.1/PKG-INFO` & `swedish_market_insights-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: swedish-market-insights
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package to scrape the Finansinspektion's registers
+Home-page: https://github.com/fritjof-b/swedish-market-insights
 License: MIT
 Author: Fritjof Bengtsson
 Author-email: fritjof.folkeson@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: black (>=23.3.0,<24.0.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Repository, https://github.com/fritjof-b/swedish-market-insights
 Description-Content-Type: text/markdown
 
 # Swedish Market Insights
 
 SMI is a small package for fetching inside trades made in Sweden.
 The data is collected with `requests` and parsed with `BeautifulSoup4`.
 All data is publicly available on Finansinspektionen's [website](https://fi.se/).
```

