# Comparing `tmp/seven2one-4.1.1.tar.gz` & `tmp/seven2one-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven2one-4.1.1.tar", last modified: Wed Apr 19 07:46:56 2023, max compression
+gzip compressed data, was "seven2one-4.1.2.tar", last modified: Mon Apr 24 07:01:43 2023, max compression
```

## Comparing `seven2one-4.1.1.tar` & `seven2one-4.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:46:56.289813 seven2one-4.1.1/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-04-14 08:32:42.000000 seven2one-4.1.1/LICENSE
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-14 08:32:42.000000 seven2one-4.1.1/MANIFEST.in
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-19 07:46:56.289813 seven2one-4.1.1/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1771 2023-04-14 08:32:42.000000 seven2one-4.1.1/README.md
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-04-19 07:46:56.289813 seven2one-4.1.1/setup.cfg
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-04-19 07:45:51.000000 seven2one-4.1.1/setup.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:46:56.285813 seven2one-4.1.1/seven2one/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-04-19 07:46:51.000000 seven2one-4.1.1/seven2one/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-04-19 07:30:12.000000 seven2one-4.1.1/seven2one/authorization.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/automation.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    63376 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/core.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/email.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/fileImportService.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/fileimport.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:46:56.289813 seven2one-4.1.1/seven2one/logging_loki/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/logging_loki/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/logging_loki/const.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/logging_loki/emitter.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/logging_loki/handlers.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/programming.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/schedule.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61487 2023-04-19 07:30:12.000000 seven2one-4.1.1/seven2one/timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:46:56.289813 seven2one-4.1.1/seven2one/utils/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-04-19 07:46:51.000000 seven2one-4.1.1/seven2one/utils/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35310 2023-04-19 07:30:12.000000 seven2one-4.1.1/seven2one/utils/ut.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/utils/ut_autprog.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/utils/ut_fileimport.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/utils/ut_init.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-04-19 07:30:12.000000 seven2one-4.1.1/seven2one/utils/ut_log.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/utils/ut_meta.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/utils/ut_time.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6584 2023-04-14 08:32:42.000000 seven2one-4.1.1/seven2one/utils/ut_timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:46:56.285813 seven2one-4.1.1/seven2one.egg-info/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-19 07:46:56.000000 seven2one-4.1.1/seven2one.egg-info/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-04-19 07:46:56.000000 seven2one-4.1.1/seven2one.egg-info/SOURCES.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-19 07:46:56.000000 seven2one-4.1.1/seven2one.egg-info/dependency_links.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-19 07:46:56.000000 seven2one-4.1.1/seven2one.egg-info/not-zip-safe
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-04-19 07:46:56.000000 seven2one-4.1.1/seven2one.egg-info/requires.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-04-19 07:46:56.000000 seven2one-4.1.1/seven2one.egg-info/top_level.txt
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-24 07:01:43.052679 seven2one-4.1.2/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-04-14 08:32:42.000000 seven2one-4.1.2/LICENSE
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-14 08:32:42.000000 seven2one-4.1.2/MANIFEST.in
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-24 07:01:43.052679 seven2one-4.1.2/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1771 2023-04-14 08:32:42.000000 seven2one-4.1.2/README.md
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-04-24 07:01:43.052679 seven2one-4.1.2/setup.cfg
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-04-19 07:45:51.000000 seven2one-4.1.2/setup.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-24 07:01:43.052679 seven2one-4.1.2/seven2one/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-04-24 07:01:38.000000 seven2one-4.1.2/seven2one/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-04-19 07:30:12.000000 seven2one-4.1.2/seven2one/authorization.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/automation.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    63376 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/core.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/email.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/fileImportService.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/fileimport.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-24 07:01:43.052679 seven2one-4.1.2/seven2one/logging_loki/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/logging_loki/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/logging_loki/const.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/logging_loki/emitter.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/logging_loki/handlers.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/programming.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/schedule.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61487 2023-04-19 07:30:12.000000 seven2one-4.1.2/seven2one/timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-24 07:01:43.052679 seven2one-4.1.2/seven2one/utils/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-04-24 07:01:38.000000 seven2one-4.1.2/seven2one/utils/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35310 2023-04-19 07:30:12.000000 seven2one-4.1.2/seven2one/utils/ut.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/utils/ut_autprog.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/utils/ut_fileimport.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/utils/ut_init.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-04-19 07:30:12.000000 seven2one-4.1.2/seven2one/utils/ut_log.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/utils/ut_meta.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-04-14 08:32:42.000000 seven2one-4.1.2/seven2one/utils/ut_time.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-04-24 06:02:28.000000 seven2one-4.1.2/seven2one/utils/ut_timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-24 07:01:43.052679 seven2one-4.1.2/seven2one.egg-info/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-24 07:01:43.000000 seven2one-4.1.2/seven2one.egg-info/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-04-24 07:01:43.000000 seven2one-4.1.2/seven2one.egg-info/SOURCES.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-24 07:01:43.000000 seven2one-4.1.2/seven2one.egg-info/dependency_links.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-24 07:01:42.000000 seven2one-4.1.2/seven2one.egg-info/not-zip-safe
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-04-24 07:01:43.000000 seven2one-4.1.2/seven2one.egg-info/requires.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-04-24 07:01:43.000000 seven2one-4.1.2/seven2one.egg-info/top_level.txt
```

### Comparing `seven2one-4.1.1/LICENSE` & `seven2one-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/PKG-INFO` & `seven2one-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.1.1
+Version: 4.1.2
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.1.1/README.md` & `seven2one-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/setup.py` & `seven2one-4.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/authorization.py` & `seven2one-4.1.2/seven2one/authorization.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/automation.py` & `seven2one-4.1.2/seven2one/automation.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/core.py` & `seven2one-4.1.2/seven2one/core.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/email.py` & `seven2one-4.1.2/seven2one/email.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/fileImportService.py` & `seven2one-4.1.2/seven2one/fileImportService.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/fileimport.py` & `seven2one-4.1.2/seven2one/fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/logging_loki/const.py` & `seven2one-4.1.2/seven2one/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/logging_loki/emitter.py` & `seven2one-4.1.2/seven2one/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/logging_loki/handlers.py` & `seven2one-4.1.2/seven2one/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/programming.py` & `seven2one-4.1.2/seven2one/programming.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/schedule.py` & `seven2one-4.1.2/seven2one/schedule.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/timeseries.py` & `seven2one-4.1.2/seven2one/timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut.py` & `seven2one-4.1.2/seven2one/utils/ut.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_autprog.py` & `seven2one-4.1.2/seven2one/utils/ut_autprog.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_fileimport.py` & `seven2one-4.1.2/seven2one/utils/ut_fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_init.py` & `seven2one-4.1.2/seven2one/utils/ut_init.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_log.py` & `seven2one-4.1.2/seven2one/utils/ut_log.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_meta.py` & `seven2one-4.1.2/seven2one/utils/ut_meta.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_time.py` & `seven2one-4.1.2/seven2one/utils/ut_time.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.1.1/seven2one/utils/ut_timeseries.py` & `seven2one-4.1.2/seven2one/utils/ut_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from itertools import islice
 import pandas as pd
-from numpy import nan
 import pytz
 from loguru import logger
 from .ut import Utils
 import math
 
 gq = Utils._toGraphQL
 
@@ -74,15 +73,15 @@
         """
         Creates a time Series DataFrame for different time series data methods
         """
         df = dataFrame
         if df.empty:
             logger.info('The query did not produce results.')
             return df
-        df.loc[(df.flag == 'MISSING'), 'value'] = nan
+        df.loc[(df.flag == 'MISSING'), 'value'] = math.nan
         
         if displayMode == 'pivot':
             if includeMissing == False:
                 df = df.pivot_table(index='timestamp', columns=fields, values='value', dropna=True)
             else:
                 df = df.pivot_table(index='timestamp', columns=fields, values='value', dropna=False)
```

### Comparing `seven2one-4.1.1/seven2one.egg-info/PKG-INFO` & `seven2one-4.1.2/seven2one.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.1.1
+Version: 4.1.2
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.1.1/seven2one.egg-info/SOURCES.txt` & `seven2one-4.1.2/seven2one.egg-info/SOURCES.txt`

 * *Files identical despite different names*

