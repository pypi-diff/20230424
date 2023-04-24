# Comparing `tmp/hledger_lots-0.1.5.tar.gz` & `tmp/hledger_lots-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.1.5.tar", last modified: Tue Apr 18 19:32:28 2023, max compression
+gzip compressed data, was "hledger_lots-0.1.6.tar", last modified: Mon Apr 24 18:35:21 2023, max compression
```

## Comparing `hledger_lots-0.1.5.tar` & `hledger_lots-0.1.6.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.815543 hledger_lots-0.1.5/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4733 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.818543 hledger_lots-0.1.5/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3001 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2525 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    12828 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3776 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3040 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4313 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2780 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/lib.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3770 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/hledger_lots/prices_yahoo.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.819543 hledger_lots-0.1.5/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1003 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       66 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       34 2023-04-18 19:32:28.000000 hledger_lots-0.1.5/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1234 2023-04-18 19:27:41.000000 hledger_lots-0.1.5/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.820543 hledger_lots-0.1.5/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4601 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2612 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.1.5/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.814543 hledger_lots-0.1.5/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:32:28.822543 hledger_lots-0.1.5/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.1.5/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.094962 hledger_lots-0.1.6/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-24 18:35:21.094962 hledger_lots-0.1.6/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.084962 hledger_lots-0.1.6/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4733 2023-04-19 21:08:59.000000 hledger_lots-0.1.6/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.087962 hledger_lots-0.1.6/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2631 2023-04-23 18:16:23.000000 hledger_lots-0.1.6/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10816 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3157 2023-04-23 18:16:23.000000 hledger_lots-0.1.6/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4326 2023-04-24 13:24:22.000000 hledger_lots-0.1.6/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2758 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3749 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/prices_yahoo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9399 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/prompt.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.089962 hledger_lots-0.1.6/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1026 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-04-24 18:34:19.000000 hledger_lots-0.1.6/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-24 18:35:21.094962 hledger_lots-0.1.6/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.091962 hledger_lots-0.1.6/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.084962 hledger_lots-0.1.6/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.093962 hledger_lots-0.1.6/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.1.5/PKG-INFO` & `hledger_lots-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_lots
-Version: 0.1.5
+Version: 0.1.6
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hledger_lots-0.1.5/docs/README.md` & `hledger_lots-0.1.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/hledger_lots/avg.py` & `hledger_lots-0.1.6/hledger_lots/avg.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     qtty: float,
     cur: str,
     cash_account: str,
     revenue_account: str,
     comm_account: str,
     value: float,
     check: bool,
-    sell_cmd: str,
 ):
     adj_comm = adjust_commodity(cur)
     checks.check_short_sell_current(txns, qtty)
     checks.check_base_currency(txns)
     checks.check_available(txns, comm_account, qtty)
 
     sell_date = datetime.strptime(date, "%Y-%m-%d").date()
@@ -93,15 +92,14 @@
     base_curr = txns[0].base_cur
     price = value / qtty
     xirr = get_xirr(price, sell_date, txns) or 0 * 100
 
     txn_hl = f"""{date} Sold {cur}  ; cost_method:avg_cost
     ; commodity:{cur}, qtty:{qtty:,.2f}, price:{price:,.2f}
     ; xirr:{xirr:.2f}% annual percent rate 30/360US
-    ; command:{sell_cmd}
     {cash_account}    {value:.2f} {base_curr}
     {comm_account}    {qtty * -1} {adj_comm} @ {cost} {base_curr}
     {revenue_account}"""
 
     comm = ["hledger", "-f-", "print", "--explicit"]
     txn_proc = subprocess.run(comm, input=txn_hl.encode(), capture_output=True)
```

### Comparing `hledger_lots-0.1.5/hledger_lots/avg_info.py` & `hledger_lots-0.1.6/hledger_lots/avg_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from datetime import datetime
 from typing import Tuple
 
 from .avg import get_avg_cost
 from .info import AllInfo, Info, LotsInfo
+from .lib import dt_list2table
 
 
 class AvgInfo(Info):
     def __init__(self, journals: Tuple[str, ...], commodity: str, check: bool):
         super().__init__(journals, commodity)
         self.check = check
+        self.avg_lots = get_avg_cost(self.txns, self.check)
+        self.table = dt_list2table(self.avg_lots)
 
     @property
     def info(self):
         commodity = self.commodity
         cur = self.txns[0].base_cur
-        avg_lots = get_avg_cost(self.txns, self.check)
-        qtty = avg_lots[-1].total_qtty
-        amount = avg_lots[-1].total_amount
-        avg_cost = avg_lots[-1].avg_cost
-        last_buy_date = datetime.strptime(avg_lots[-1].date, "%Y-%m-%d").date()
+        qtty = self.avg_lots[-1].total_qtty
+        amount = self.avg_lots[-1].total_amount
+        avg_cost = self.avg_lots[-1].avg_cost
+        last_buy_date = datetime.strptime(self.avg_lots[-1].date, "%Y-%m-%d").date()
         xirr = self.get_lots_xirr(last_buy_date)
 
         if self.market_price and self.market_date and xirr:
             market_price_str = f"{self.market_price:,.4f}"
             market_amount = self.market_price * qtty
             market_amount_str = f"{market_amount:,.2f}"
             market_profit = market_amount - amount
```

### Comparing `hledger_lots-0.1.5/hledger_lots/checks.py` & `hledger_lots-0.1.6/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/hledger_lots/cli.py` & `hledger_lots-0.1.6/hledger_lots/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import functools
 import os
 from pathlib import Path
 from typing import Literal, Tuple
 
 import rich_click as click
 
-from .avg import avg_sell, get_avg_cost
 from .avg_info import AllAvgInfo, AvgInfo
-from .fifo import get_lots, get_sell_lots, txn2hl
 from .fifo_info import AllFifoInfo, FifoInfo
-from .files import get_default_file, get_file_path
-from .hl import hledger2txn
-from .info import AllInfo, get_commodities
-from .lib import default_fn_bool, dt_list2table, get_sell_comm
+from .files import get_default_file, get_file_path, get_files_comm
+from .info import AllInfo
+from .lib import default_fn_bool
 from .prices_yahoo import get_hledger_prices
+from .prompt import PromptSell, get_append_file
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 click.rich_click.USE_MARKDOWN = True
 click.rich_click.SHOW_ARGUMENTS = True
 click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
 click.rich_click.MAX_WIDTH = 80
@@ -85,15 +82,14 @@
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
     help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. Inthe future it will default to true",
 )
-# TODO: fill help
 @click.option(
     "-p",
     "--append-prices-to",
     type=click.Path(),
     default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
     prompt=False,
     required=False,
@@ -109,37 +105,28 @@
 ):
     """
     Report lots for a commodity.\r
 
     Show a report with lots for a commodity considering eventual past sale using FIFO or AVERAGE COST accounting principles.
 
     Also show some indicators about the lots and performance if there is prices in the journal after the last purchase. See the docs for details
-
-    All flags, except '--file' will be interactively prompted if absent, much like 'hledger-add'.
     """
 
     journals = file or get_default_file()
-    adj_txn = hledger2txn(journals, commodity, no_desc)
 
     if append_prices_to:
         get_hledger_prices(file, append_prices_to)
 
     if avg_cost:
-        buy_lots = get_avg_cost(adj_txn, check)
-        table = dt_list2table(buy_lots)
-        click.echo(table)
-        avg_info = AvgInfo(journals, commodity, check)
-        click.echo(avg_info.info_txt)
-
+        info = AvgInfo(journals, commodity, check)
     else:
-        buy_lots = get_lots(adj_txn, check)
-        table = dt_list2table(buy_lots)
-        click.echo(table)
-        fifo_info = FifoInfo(journals, commodity, check)
-        click.echo(fifo_info.info_txt)
+        info = FifoInfo(journals, commodity, check)
+
+    click.echo(info.table)
+    click.echo(info.info_txt)
 
 
 @click.command()
 @click.option(
     "-f",
     "--file",
     type=click.Path(),
@@ -152,154 +139,74 @@
     "-g",
     "--avg-cost",
     is_flag=True,
     default=default_fn_bool("HLEDGER_LOTS_AVG_COST", False),
     help='Change cost method to "average cost"". Can be set with env HLEDGER_LOTS_IS_AVG_COST=true|false. Default to false',
 )
 @click.option(
-    "-c",
-    "--commodity",
-    type=click.STRING,
-    prompt=True,
-    help="Commodity you are selling",
-)
-@click.option(
     "-n",
     "--no-desc",
     type=click.STRING,
     default=lambda: os.environ.get("HLEDGER_LOTS_NO_DESC", None),
-    prompt=False,
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
-    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=tru|false. Default to false. Inthe future it will default to true",
-)
-@click.option(
-    "-s",
-    "--commodity-account",
-    type=click.STRING,
-    prompt=False,
-    required=False,
-    help="What account holds product of the sale. Only used with --avg-cost",
-)
-@click.option(
-    "-a",
-    "--cash-account",
-    type=click.STRING,
-    prompt=True,
-    help="What account entered the product of the sell",
-)
-@click.option(
-    "-r",
-    "--revenue-account",
-    type=click.STRING,
-    prompt=True,
-    help="Account that represent capital gain/loss",
-)
-@click.option(
-    "-d",
-    "--date",
-    type=click.STRING,
-    prompt=True,
-    help="Date of the transaction (YYYY-mm-dd)",
-)
-@click.option(
-    "-q",
-    "--quantity",
-    help="Quantity being sold",
-    type=click.FLOAT,
-    prompt=True,
-)
-@click.option(
-    "-p",
-    "--price",
-    help="Price being sold",
-    type=click.FLOAT,
-    prompt=True,
+    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. In the future it will default to true",
 )
 @click.pass_context
 def sell(
     ctx: click.Context,  # pyright:ignore
     file: Tuple[str, ...],
     avg_cost: bool,
-    commodity: str,
     no_desc: str,
-    commodity_account: str,
-    cash_account: str,
-    revenue_account: str,
-    date: str,
-    quantity: float,
-    price: float,
     check: bool,
 ):
     """
-    Create a transaction with automatic FIFO or AVERAGE COST for a commodity.\r
+    Create a transaction with automatic FIFO or AVERAGE COST for a commodity by answering some prompts that tries to avoid errors with validation and using current journal data to filter possible answers give informations that guides the user thru the process.\r
+
+    > This command also add transaction's comment with some indicators. See an example on "Output examples" page of the docs.
 
-    Generate a transaction that represents a sale of a commodity with the following postings:
+    ## Transaction postings
 
     - First posting: Positive amount on the 'base-currency' in the account that receives the product of the sale.
 
-    - Multiple lot postings: Each posting is a different lot you are selling for the cost price on purchasing date, calculated according to FIFO accounting principles.
+    - Multiple lot postings: Each posting represents a lot you are selling for the cost price on purchasing date, according to FIFO accounting principles or one postings in case of AVERAGE COST method.
 
     - Revenue posting: posting that represent Capital Gain or Loss as the difference between the total cost and the amount received on the base-currency.
-
-    This command also add transaction's comment with some indicators. See the docs for more info.
-
-    All flags, except '--file' will be interactively prompted if absent, much like 'hledger-add'.
     """
 
     journals = file or get_default_file()
-    adj_txns = hledger2txn(journals, commodity, no_desc)
-    value = quantity * price
+    prompt_sell = PromptSell(journals, avg_cost, check, no_desc)
 
-    sell_comm_fn = functools.partial(
-        get_sell_comm,
-        commodity,
-        no_desc,
-        commodity_account,
-        cash_account,
-        revenue_account,
-        date,
-        quantity,
-        price,
-    )
+    txn_print = prompt_sell.get_hl_txn()
+    click.echo("\n" + txn_print)
 
-    if avg_cost and not commodity_account:
-        commodity_account = input("Commodity account: ")
+    append_file = get_append_file(journals[0])
+    if append_file:
+        with open(append_file, "a") as f:
+            f.write("\n" + txn_print)
+    else:
+        click.echo("\n" + "Transaction not saved.")
 
+    commodity = prompt_sell.info["comm"]
     if avg_cost:
-        sell_cmd = sell_comm_fn(True)
-        sell_avg = avg_sell(
-            txns=adj_txns,
-            date=date,
-            qtty=quantity,
-            cur=commodity,
-            cash_account=cash_account,
-            revenue_account=revenue_account,
-            comm_account=commodity_account,
-            value=value,
-            check=check,
-            sell_cmd=sell_cmd,
-        )
-        click.echo(sell_avg)
+        info = AvgInfo(journals, commodity, check)
     else:
-        sell_fifo = get_sell_lots(adj_txns, date, quantity, check)
-        sell_cmd = sell_comm_fn(False)
-        txn_print = txn2hl(
-            txns=sell_fifo,
-            date=date,
-            cur=commodity,
-            cash_account=cash_account,
-            revenue_account=revenue_account,
-            value=value,
-            sell_cmd=sell_cmd,
+        info = FifoInfo(journals, commodity, check)
+
+    click.echo(info.table)
+    click.echo(info.info_txt)
+
+    if commodity.startswith("y."):
+        files_comm_str = " ".join(get_files_comm(journals))
+        click.echo(
+            f"To update prices from Yahoo finance, run:\n\n hledger-lots {files_comm_str} view -c {commodity} -p {journals[0]}"
         )
-        click.echo(txn_print)
 
 
 @click.command(name="list")
 @click.option(
     "-f",
     "--file",
     type=click.Path(),
@@ -378,9 +285,9 @@
     else:
         table = lots_info.infos_table("plain")
 
     click.echo(table)
 
 
 cli.add_command(view)
-cli.add_command(sell)
 cli.add_command(list_commodities)
+cli.add_command(sell)
```

### Comparing `hledger_lots-0.1.5/hledger_lots/fifo.py` & `hledger_lots-0.1.6/hledger_lots/fifo.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,29 +87,27 @@
 def txn2hl(
     txns: List[AdjustedTxn],
     date: str,
     cur: str,
     cash_account: str,
     revenue_account: str,
     value: float,
-    sell_cmd: str,
 ):
     adj_comm = adjust_commodity(cur)
     base_curr = txns[0].base_cur
     avg_cost = get_avg_fifo(txns)
     sum_qtty = sum(txn.qtty for txn in txns)
     price = value / sum_qtty
     dt = datetime.strptime(date, "%Y-%m-%d").date()
     xirr = get_xirr(price, dt, txns) or 0 * 100
 
     txn_hl = f"""
 {date} Sold {cur}  ; cost_method:fifo
     ; commodity:{cur}, qtty:{sum_qtty:,.2f}, price:{price:,.2f}
     ; avg_cost:{avg_cost:,.4f}, xirr:{xirr:.2f}% annual percent rate 30/360US
-    ; command:{sell_cmd}
     {cash_account}  {value:.2f} {base_curr}
 """
 
     for txn in txns:
         txn_hl += f"    {txn.acct}    {txn.qtty * -1} {adj_comm} @ {txn.price} {base_curr}  ; buy_date:{txn.date}, base_cur:{txn.base_cur}\n"
 
     txn_hl += f"    {revenue_account}   "
```

### Comparing `hledger_lots-0.1.5/hledger_lots/fifo_info.py` & `hledger_lots-0.1.6/hledger_lots/fifo_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from datetime import datetime
 from typing import Tuple
 
 from .checks import MultipleBaseCurrencies
 from .fifo import get_lots
 from .hl import hledger2txn
 from .info import AllInfo, Info, LotsInfo
-from .lib import get_avg_fifo
+from .lib import dt_list2table, get_avg_fifo
 
 
 class FifoInfo(Info):
     def __init__(self, journals: Tuple[str, ...], commodity: str, check: bool):
         super().__init__(journals, commodity)
         self.check = check
 
         self.lots = get_lots(self.txns, check)
         self.last_buy_date = self.lots[-1].date if len(self.lots) > 0 else None
 
+        self.buy_lots = get_lots(self.txns, check)
+        self.table = dt_list2table(self.buy_lots)
+
     @property
     def info(self):
         commodity = self.commodity
 
         cur = self.lots[0].base_cur
         qtty = sum(lot.qtty for lot in self.lots)
         amount = sum(lot.price * lot.qtty for lot in self.lots)
```

### Comparing `hledger_lots-0.1.5/hledger_lots/files.py` & `hledger_lots-0.1.6/hledger_lots/files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/hledger_lots/hl.py` & `hledger_lots-0.1.6/hledger_lots/hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/hledger_lots/info.py` & `hledger_lots-0.1.6/hledger_lots/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 def get_commodities(journals: Tuple[str, ...]):
     files_comm = get_files_comm(journals)
     comm = ["hledger", *files_comm, "commodities"]
     commodities_proc = subprocess.run(comm, capture_output=True)
     commodities_str = commodities_proc.stdout.decode("utf8")
 
-    commodities_list = [com for com in commodities_str.split("\n")]
+    commodities_list = [com for com in commodities_str.split("\n") if com != ""]
     return commodities_list
 
 
 class Info:
     def __init__(
         self, journals: Tuple[str, ...], commodity: str, no_desc: Optional[str] = None
     ) -> None:
```

### Comparing `hledger_lots-0.1.5/hledger_lots/lib.py` & `hledger_lots-0.1.6/hledger_lots/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 import re
 import shlex
 from dataclasses import asdict, dataclass
 from datetime import date
 from typing import List, Optional
 
+import click
 from pyxirr import DayCount, xirr
 from tabulate import tabulate
 
-from .files import get_files_comm
-
 
 @dataclass
 class AdjustedTxn:
     date: str
     price: float
     base_cur: str
     qtty: float
```

### Comparing `hledger_lots-0.1.5/hledger_lots/prices_yahoo.py` & `hledger_lots-0.1.6/hledger_lots/prices_yahoo.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import yfinance as yf
 from requests.exceptions import HTTPError
 from requests_cache import CachedSession
 
+from .files import get_files_comm
 from .hl import hledger2txn
 from .info import get_commodities, get_last_price
-from .lib import adjust_commodity, get_files_comm
 
 
 @dataclass
 class Price:
     name: str
     date: date
     price: float
@@ -109,14 +109,14 @@
                     prices = get_yahoo_prices(
                         ticker, start_date, yesterday_str, session
                     )
                     prices_hledger = prices2hledger(prices)
                     f.write(prices_hledger + "\n")
                 except HTTPError:
                     print(f"stderr: {ticker} not found", file=sys.stderr)
-                except Exception as e:
+                except Exception:
                     print(
                         f"stderr: Nothing downloaded for {ticker} between {start_date} and {yesterday_str}",
                         file=sys.stderr,
                     )
 
         f.write("\n")
```

### Comparing `hledger_lots-0.1.5/hledger_lots.egg-info/PKG-INFO` & `hledger_lots-0.1.6/hledger_lots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-lots
-Version: 0.1.5
+Version: 0.1.6
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hledger_lots-0.1.5/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.1.6/hledger_lots.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 hledger_lots/fifo.py
 hledger_lots/fifo_info.py
 hledger_lots/files.py
 hledger_lots/hl.py
 hledger_lots/info.py
 hledger_lots/lib.py
 hledger_lots/prices_yahoo.py
+hledger_lots/prompt.py
 hledger_lots.egg-info/PKG-INFO
 hledger_lots.egg-info/SOURCES.txt
 hledger_lots.egg-info/dependency_links.txt
 hledger_lots.egg-info/entry_points.txt
 hledger_lots.egg-info/requires.txt
 hledger_lots.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `hledger_lots-0.1.5/pyproject.toml` & `hledger_lots-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,27 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.1.5"
+version = "0.1.6"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
 	     "pyxirr",
 	     "yfinance",
 	     "requests",
-	     "requests-cache"
+	     "requests-cache",
+	     "questionary"
 ]
 
 [project.urls]
 homepage = "https://github.com/edkedk99/hledger-lots"
 documentation = "https://edkedk99.github.io/hledger-lots/"
 repository = "https://github.com/edkedk99/hledger-lots"
 # changelog = ""
```

### Comparing `hledger_lots-0.1.5/tests/lots_data.py` & `hledger_lots-0.1.6/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/tests/test_avg.py` & `hledger_lots-0.1.6/tests/test_avg.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,19 @@
             qtty=50,
             cur="AAPL",
             cash_account="Asset:Bank",
             revenue_account="Revenue:Capital Gain",
             comm_account="Acct1",
             value=1000,
             check=False,
-            sell_cmd=""
         )
 
         expected = """2022-02-01 Sold AAPL  ; cost_method:avg_cost
     ; commodity:AAPL, qtty:50.00, price:20.00
     ; xirr:3.56% annual percent rate 30/360US
-    ; command:
     Asset:Bank                                    1000.00 USD
     Acct1                   -50 AAPL @ 17.848837209302324 USD
     Revenue:Capital Gain               -107.5581395348838 USD
 
 """
 
         assert test == expected
```

### Comparing `hledger_lots-0.1.5/tests/test_checks.py` & `hledger_lots-0.1.6/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/tests/test_fifo.py` & `hledger_lots-0.1.6/tests/test_fifo.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,40 +48,37 @@
     date = "2022-02-01"
     cash_account = "Bank"
     revenue_account = "Revenue"
 
     def test_txn2hl_profit(self):
         cur = "USD"
         test = fifo.txn2hl(
-            self.txns, self.date, cur, self.cash_account, self.revenue_account, 160, ""
-        )
+            self.txns, self.date, cur, self.cash_account, self.revenue_account, 160)
 
         expected = """2022-02-01 Sold USD  ; cost_method:fifo
     ; commodity:USD, qtty:5.00, price:32.00
     ; avg_cost:26.0000, xirr:61.42% annual percent rate 30/360US
-    ; command:
     Bank                 160.00 USD
     Acct1      -2.00 USD @ 35.0 USD  ; buy_date:2022-01-12, base_cur:USD
     Acct1      -3.00 USD @ 20.0 USD  ; buy_date:2022-01-14, base_cur:USD
     Revenue              -30.00 USD
 
 """
 
         assert test == expected
 
     def test_txn2hl_loss(self):
         cur = "USD"
         test = fifo.txn2hl(
-            self.txns, self.date, cur, self.cash_account, self.revenue_account, 80, ""
+            self.txns, self.date, cur, self.cash_account, self.revenue_account, 80
         )
 
         expected = """2022-02-01 Sold USD  ; cost_method:fifo
     ; commodity:USD, qtty:5.00, price:16.00
     ; avg_cost:26.0000, xirr:-1.00% annual percent rate 30/360US
-    ; command:
     Bank                  80.00 USD
     Acct1      -2.00 USD @ 35.0 USD  ; buy_date:2022-01-12, base_cur:USD
     Acct1      -3.00 USD @ 20.0 USD  ; buy_date:2022-01-14, base_cur:USD
     Revenue               50.00 USD
 
 """
```

### Comparing `hledger_lots-0.1.5/tests/test_files.py` & `hledger_lots-0.1.6/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/tests/test_hl.py` & `hledger_lots-0.1.6/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/tests/test_info.py` & `hledger_lots-0.1.6/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/tests/test_lib.py` & `hledger_lots-0.1.6/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2html.py` & `hledger_lots-0.1.6/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2html4.py` & `hledger_lots-0.1.6/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2html5.py` & `hledger_lots-0.1.6/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2latex.py` & `hledger_lots-0.1.6/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2man.py` & `hledger_lots-0.1.6/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2odt.py` & `hledger_lots-0.1.6/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.1.6/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.1.6/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2s5.py` & `hledger_lots-0.1.6/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2xetex.py` & `hledger_lots-0.1.6/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rst2xml.py` & `hledger_lots-0.1.6/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.5/venv/bin/rstpep2html.py` & `hledger_lots-0.1.6/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

