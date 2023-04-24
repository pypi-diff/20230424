# Comparing `tmp/chain-aide-1.0.4.tar.gz` & `tmp/chain-aide-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chain-aide-1.0.4.tar", last modified: Fri Apr 14 08:26:46 2023, max compression
+gzip compressed data, was "chain-aide-1.0.5.tar", last modified: Mon Apr 24 01:04:11 2023, max compression
```

## Comparing `chain-aide-1.0.4.tar` & `chain-aide-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:26:46.204867 chain-aide-1.0.4/
--rw-rw-rw-   0        0        0     1083 2023-03-23 06:13:36.000000 chain-aide-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3589 2023-04-14 08:26:46.189257 chain-aide-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2716 2023-03-31 09:03:39.000000 chain-aide-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 08:26:46.189257 chain-aide-1.0.4/chain_aide/
--rw-rw-rw-   0        0        0       65 2023-03-23 06:25:45.000000 chain-aide-1.0.4/chain_aide/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-03-31 06:26:42.000000 chain-aide-1.0.4/chain_aide/contract.py
--rw-rw-rw-   0        0        0     6176 2023-04-14 08:25:32.000000 chain-aide-1.0.4/chain_aide/main.py
--rw-rw-rw-   0        0        0     1635 2023-03-31 06:13:53.000000 chain-aide-1.0.4/chain_aide/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:26:46.189257 chain-aide-1.0.4/chain_aide.egg-info/
--rw-rw-rw-   0        0        0     3589 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 06:56:02.000000 chain-aide-1.0.4/chain_aide.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 08:26:46.207260 chain-aide-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1620 2023-04-14 08:25:58.000000 chain-aide-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:04:11.172767 chain-aide-1.0.5/
+-rw-rw-rw-   0        0        0     1083 2023-03-23 06:13:36.000000 chain-aide-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3589 2023-04-24 01:04:11.171767 chain-aide-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2716 2023-03-31 09:03:39.000000 chain-aide-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:04:11.161767 chain-aide-1.0.5/chain_aide/
+-rw-rw-rw-   0        0        0       65 2023-03-23 06:25:45.000000 chain-aide-1.0.5/chain_aide/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-03-31 06:26:42.000000 chain-aide-1.0.5/chain_aide/contract.py
+-rw-rw-rw-   0        0        0     6176 2023-04-14 08:25:32.000000 chain-aide-1.0.5/chain_aide/main.py
+-rw-rw-rw-   0        0        0     1595 2023-04-24 01:01:39.000000 chain-aide-1.0.5/chain_aide/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:04:11.169772 chain-aide-1.0.5/chain_aide.egg-info/
+-rw-rw-rw-   0        0        0     3589 2023-04-24 01:04:11.000000 chain-aide-1.0.5/chain_aide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-24 01:04:11.000000 chain-aide-1.0.5/chain_aide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:04:11.000000 chain-aide-1.0.5/chain_aide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 06:56:02.000000 chain-aide-1.0.5/chain_aide.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-04-24 01:04:11.000000 chain-aide-1.0.5/chain_aide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 01:04:11.000000 chain-aide-1.0.5/chain_aide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:04:11.172767 chain-aide-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2023-04-24 01:03:56.000000 chain-aide-1.0.5/setup.py
```

### Comparing `chain-aide-1.0.4/LICENSE` & `chain-aide-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.4/PKG-INFO` & `chain-aide-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain-aide
-Version: 1.0.4
+Version: 1.0.5
 Summary: An aide that helps you quickly access mainstream public chain and use its basic functions.
 Home-page: https://github.com/shinnng/chain-aide
 Author: Shinnng
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: chain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chain-aide-1.0.4/README.md` & `chain-aide-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.4/chain_aide/contract.py` & `chain-aide-1.0.5/chain_aide/contract.py`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.4/chain_aide/main.py` & `chain-aide-1.0.5/chain_aide/main.py`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.4/chain_aide/utils.py` & `chain-aide-1.0.5/chain_aide/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 
 from web3 import Web3, HTTPProvider, WebsocketProvider, IPCProvider
 from web3._utils.threads import Timeout
 
 
-def get_web3(uri, chain_id=None, hrp=None, timeout=10, modules=None) -> Web3:
+def get_web3(uri, timeout=10, modules=None) -> Web3:
     """ 通过rpc uri，获取web3对象
     """
     if uri.startswith('http'):
         provider = HTTPProvider
     elif uri.startswith('ws'):
         provider = WebsocketProvider
     elif uri.startswith('ipc'):
@@ -25,30 +25,32 @@
 
     return web3
 
 
 def contract_call(func):
     """ 合约调用的包装类
     """
+
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs).call()
 
     return wrapper
 
 
 def contract_transaction(func):
     """ 合约交易的包装类
     """
+
     @functools.wraps(func)
     def wrapper(self, *args, txn: dict = None, private_key=None, **kwargs):
         # 填充from地址，以免合约交易在预估gas时检验地址失败
         txn = txn or {}
         if not txn.get('from'):
-            account = self.aide.eth.account.from_key(private_key, hrp=self.aide.hrp) if private_key else self.aide.default_account
+            account = self.aide.eth.account.from_key(private_key) if private_key else self.aide.default_account
             if account:
                 txn['from'] = account.address
 
         txn = func(*args, **kwargs).build_transaction(txn)
         return self.aide.send_transaction(txn, private_key=private_key)
 
     return wrapper
```

### Comparing `chain-aide-1.0.4/chain_aide.egg-info/PKG-INFO` & `chain-aide-1.0.5/chain_aide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain-aide
-Version: 1.0.4
+Version: 1.0.5
 Summary: An aide that helps you quickly access mainstream public chain and use its basic functions.
 Home-page: https://github.com/shinnng/chain-aide
 Author: Shinnng
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: chain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chain-aide-1.0.4/setup.py` & `chain-aide-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open('./README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='chain-aide',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='1.0.4',
+    version='1.0.5',
     description="""An aide that helps you quickly access mainstream public chain and use its basic functions.""",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Shinnng',
     author_email='shinnng@outlook.com',
     url='https://github.com/shinnng/chain-aide',
     include_package_data=True,
```

