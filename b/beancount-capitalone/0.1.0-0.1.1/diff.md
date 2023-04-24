# Comparing `tmp/beancount-capitalone-0.1.0.tar.gz` & `tmp/beancount-capitalone-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-capitalone-0.1.0.tar", last modified: Fri Mar 10 14:47:36 2023, max compression
+gzip compressed data, was "beancount-capitalone-0.1.1.tar", last modified: Mon Apr 24 12:17:09 2023, max compression
```

## Comparing `beancount-capitalone-0.1.0.tar` & `beancount-capitalone-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-10 14:47:36.158178 beancount-capitalone-0.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2667 2023-03-10 14:47:36.158178 beancount-capitalone-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1865 2023-03-10 14:47:26.000000 beancount-capitalone-0.1.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-10 14:47:36.158178 beancount-capitalone-0.1.0/beancount_capitalone/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-03-10 14:47:26.000000 beancount-capitalone-0.1.0/beancount_capitalone/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3835 2023-03-10 14:47:26.000000 beancount-capitalone-0.1.0/beancount_capitalone/credit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2511 2023-03-10 14:47:26.000000 beancount-capitalone-0.1.0/beancount_capitalone/credit_test.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-10 14:47:36.158178 beancount-capitalone-0.1.0/beancount_capitalone.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2667 2023-03-10 14:47:36.000000 beancount-capitalone-0.1.0/beancount_capitalone.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2023-03-10 14:47:36.000000 beancount-capitalone-0.1.0/beancount_capitalone.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-10 14:47:36.000000 beancount-capitalone-0.1.0/beancount_capitalone.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-03-10 14:47:36.000000 beancount-capitalone-0.1.0/beancount_capitalone.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-10 14:47:36.158178 beancount-capitalone-0.1.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      658 2023-03-10 14:47:26.000000 beancount-capitalone-0.1.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-24 12:17:09.268375 beancount-capitalone-0.1.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2667 2023-04-24 12:17:09.268375 beancount-capitalone-0.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1865 2023-04-24 12:17:02.000000 beancount-capitalone-0.1.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-24 12:17:09.268375 beancount-capitalone-0.1.1/beancount_capitalone/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-04-24 12:17:02.000000 beancount-capitalone-0.1.1/beancount_capitalone/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4152 2023-04-24 12:17:02.000000 beancount-capitalone-0.1.1/beancount_capitalone/credit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3255 2023-04-24 12:17:02.000000 beancount-capitalone-0.1.1/beancount_capitalone/credit_test.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-24 12:17:09.268375 beancount-capitalone-0.1.1/beancount_capitalone.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2667 2023-04-24 12:17:09.000000 beancount-capitalone-0.1.1/beancount_capitalone.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      294 2023-04-24 12:17:09.000000 beancount-capitalone-0.1.1/beancount_capitalone.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-24 12:17:09.000000 beancount-capitalone-0.1.1/beancount_capitalone.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-04-24 12:17:09.000000 beancount-capitalone-0.1.1/beancount_capitalone.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-24 12:17:09.268375 beancount-capitalone-0.1.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      658 2023-04-24 12:17:02.000000 beancount-capitalone-0.1.1/setup.py
```

### Comparing `beancount-capitalone-0.1.0/PKG-INFO` & `beancount-capitalone-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-capitalone
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import CapitalOne banking transactions into beancount format
 Home-page: https://github.com/mtlynch/beancount-capitalone.git
 Author: Michael Lynch
 License: MIT
 Description: # beancount-capitalone
         
         [![PyPI](https://img.shields.io/pypi/v/beancount-capitalone)](https://pypi.org/project/beancount-capitalone/)
```

### Comparing `beancount-capitalone-0.1.0/README.md` & `beancount-capitalone-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `beancount-capitalone-0.1.0/beancount_capitalone/credit.py` & `beancount-capitalone-0.1.1/beancount_capitalone/credit.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from beancount.core import data
 from beancount.core import flags
 from beancount.core import number as beancount_number
 from beancount.ingest import importer
 
 _COLUMN_DATE = 'Posted Date'
 _COLUMN_PAYEE = 'Description'
-_COLUMN_AMOUNT = 'Debit'
+_COLUMN_DEBIT_AMOUNT = 'Debit'
+_COLUMN_CREDIT_AMOUNT = 'Credit'
 
 _FILENAME_PATTERN = re.compile(r'\d{4}-\d{2}-\d{2}_transaction_download.csv')
 
 
 class CreditImporter(importer.ImporterProtocol):
 
     def __init__(self,
@@ -67,16 +68,20 @@
     def _extract_transaction_from_row(self, row, metadata):
         transaction_date = datetime.datetime.strptime(row[_COLUMN_DATE],
                                                       '%Y-%m-%d').date()
 
         payee = row[_COLUMN_PAYEE]
         transaction_description = titlecase.titlecase(payee)
 
-        if row[_COLUMN_AMOUNT]:
-            transaction_amount = self._parse_amount(row[_COLUMN_AMOUNT])
+        if row[_COLUMN_DEBIT_AMOUNT]:
+            transaction_amount = self._parse_amount(row[_COLUMN_DEBIT_AMOUNT])
+        elif row[_COLUMN_CREDIT_AMOUNT]:
+            # Negate the credit column so that it has opposite sign from debits.
+            negated_credit_amount = '-' + row[_COLUMN_CREDIT_AMOUNT]
+            transaction_amount = self._parse_amount(negated_credit_amount)
         else:
             return None  # 0 dollar transaction
 
         if transaction_amount == amount.Amount(beancount_number.D(0),
                                                self._currency):
             return None
```

### Comparing `beancount-capitalone-0.1.0/beancount_capitalone/credit_test.py` & `beancount-capitalone-0.1.1/beancount_capitalone/credit_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,7 +66,26 @@
             ]).extract(f)
 
     assert _unindent("""
         2023-02-22 * "Shopify* 169483256"
           Liabilities:Credit-Cards:CapitalOne  -528.55 USD
           Expenses:Cloud-Services:Shopify       528.55 USD
         """.rstrip()) == _stringify_directives(directives).strip()
+
+
+def test_extracts_cashback(tmp_path):
+    capitalone_file = tmp_path / '2023-03-10_transaction_download.csv'
+    capitalone_file.write_text(
+        _unindent("""
+            Transaction Date,Posted Date,Card No.,Description,Category,Debit,Credit
+            2023-03-03,2023-03-03,1234,CREDIT-CASH BACK REWARD,Payment/Credit,,32.42
+            """))
+
+    with capitalone_file.open() as f:
+        directives = CreditImporter(
+            account='Income:Credit-Card-Rewards:CapitalOne-Rewards',
+            lastfour='1234').extract(f)
+
+    assert _unindent("""
+        2023-03-03 * "Credit-Cash Back Reward"
+          Income:Credit-Card-Rewards:CapitalOne-Rewards  32.42 USD
+        """.rstrip()) == _stringify_directives(directives).strip()
```

### Comparing `beancount-capitalone-0.1.0/beancount_capitalone.egg-info/PKG-INFO` & `beancount-capitalone-0.1.1/beancount_capitalone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-capitalone
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import CapitalOne banking transactions into beancount format
 Home-page: https://github.com/mtlynch/beancount-capitalone.git
 Author: Michael Lynch
 License: MIT
 Description: # beancount-capitalone
         
         [![PyPI](https://img.shields.io/pypi/v/beancount-capitalone)](https://pypi.org/project/beancount-capitalone/)
```

### Comparing `beancount-capitalone-0.1.0/setup.py` & `beancount-capitalone-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     name='beancount-capitalone',
     long_description=open(
         os.path.join(os.path.abspath(os.path.dirname(__file__)),
                      'README.md')).read(),
     long_description_content_type="text/markdown",
-    version='0.1.0',
+    version='0.1.1',
     description='Import CapitalOne banking transactions into beancount format',
     author='Michael Lynch',
     license="MIT",
     keywords="capitalone beancount bookkeeping finance",
     url='https://github.com/mtlynch/beancount-capitalone.git',
     packages=['beancount_capitalone'],
     install_requires=[],
```

