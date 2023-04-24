# Comparing `tmp/zcbot-predict-sdk-0.0.2.tar.gz` & `tmp/zcbot-predict-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-predict-sdk-0.0.2.tar", last modified: Mon Apr 24 13:05:13 2023, max compression
+gzip compressed data, was "dist\zcbot-predict-sdk-0.0.3.tar", last modified: Mon Apr 24 14:13:37 2023, max compression
```

## Comparing `zcbot-predict-sdk-0.0.2.tar` & `zcbot-predict-sdk-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.033677 zcbot-predict-sdk-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      384 2023-04-24 13:05:13.033677 zcbot-predict-sdk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-24 13:05:13.034676 zcbot-predict-sdk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-04-24 13:05:09.000000 zcbot-predict-sdk-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.005678 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/__init__.py
--rw-rw-rw-   0        0        0     7158 2023-04-23 02:14:35.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.019677 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/decator.py
--rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/exceptions.py
--rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/keys.py
--rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/thread_pool.py
--rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.024678 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/
--rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/callback.py
--rw-rw-rw-   0        0        0      404 2023-04-24 12:19:13.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/param.py
--rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/monitor.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.031676 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/
--rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/base.py
--rw-rw-rw-   0        0        0      584 2023-04-24 13:01:27.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/info_extract.py
--rw-rw-rw-   0        0        0     4066 2023-04-24 12:24:32.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/sku_tag.py
--rw-rw-rw-   0        0        0      619 2023-03-24 06:26:54.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/tax.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.011676 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/
--rw-rw-rw-   0        0        0      384 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:13:37.245029 zcbot-predict-sdk-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      384 2023-04-24 14:13:37.244029 zcbot-predict-sdk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:13:37.245029 zcbot-predict-sdk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-04-24 14:13:36.000000 zcbot-predict-sdk-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:13:37.215028 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/__init__.py
+-rw-rw-rw-   0        0        0     7158 2023-04-23 02:14:35.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:13:37.231028 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/decator.py
+-rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/exceptions.py
+-rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/keys.py
+-rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/thread_pool.py
+-rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:13:37.235030 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/model/
+-rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/model/callback.py
+-rw-rw-rw-   0        0        0      205 2023-04-24 14:12:16.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/model/param.py
+-rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:13:37.242028 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/
+-rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/base.py
+-rw-rw-rw-   0        0        0      563 2023-04-24 14:12:11.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/info_extract.py
+-rw-rw-rw-   0        0        0     3916 2023-04-24 14:12:11.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/sku_tag.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:13:37.221029 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-04-24 14:13:36.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2023-04-24 14:13:37.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:13:36.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 14:13:36.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 14:13:36.000000 zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-predict-sdk-0.0.2/setup.py` & `zcbot-predict-sdk-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-predict-sdk',
-      version='0.0.2',
+      version='0.0.3',
       description='zcbot predict sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['celery', 'redis'],
       python_requires='>=3.7',
```

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/client.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/client.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/exceptions.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/thread_pool.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/utils.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/callback.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/model/callback.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/monitor.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/info_extract.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/info_extract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union, Dict, List
 from .base import BaseService
 from ..model.callback import Callback
-from ..model.param import InfoExtractParam
+from ..model.param import TextParam
 
 
 class InfoExtractService(BaseService):
     """品牌、型号、通用名"""
 
-    def extract_sku(self, task_params: Union[Dict, InfoExtractParam] = None, callback: Callback = None, **kwargs):
-        _task_params = task_params.dict() if isinstance(task_params, InfoExtractParam) else task_params
+    def extract_sku(self, task_params: Union[Dict, TextParam] = None, callback: Callback = None, **kwargs):
+        _task_params = task_params.dict() if isinstance(task_params, TextParam) else task_params
         return self.celery_client.apply(task_name='info_extract.sku', task_params=_task_params, callback=callback, **kwargs)
```

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/sku_tag.py` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk/service/sku_tag.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 from typing import Dict, List, Union
 
 from .base import BaseService
 from ..model.callback import Callback
-from ..model.param import TaxPredictParam
+from ..model.param import TextParam
 
 
-def _params_convert(task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]]):
+def _params_convert(task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]]):
     text_list = list()
     # 单个
     if isinstance(task_params, Dict):
-        if isinstance(task_params, TaxPredictParam):
+        if isinstance(task_params, TextParam):
             text_list.append(task_params.dict())
         else:
             text_list.append(task_params)
     # 批量
     for task_param in task_params:
-        if isinstance(task_param, TaxPredictParam):
+        if isinstance(task_param, TextParam):
             text_list.append(task_param.dict())
         else:
             text_list.append(task_param)
 
     return text_list
 
 
 class StaplesSkuTagService(BaseService):
 
-    def predict_catalog1(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog1(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.catalog1', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_catalog4(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog4(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.catalog4', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_catalog6(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog6(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.catalog6', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_brand(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_brand(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.brand', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
 
 class JslinkSkuTagService(BaseService):
 
-    def predict_catalog1(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog1(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.catalog1', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_catalog4(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog4(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.catalog4', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_brand(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_brand(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.brand', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
 
 class ZjmiSkuTagService(BaseService):
 
-    def predict_catalog1(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog1(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.zjmi.catalog1', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_catalog3(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_catalog3(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.zjmi.catalog3', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
 
-    def predict_brand(self, task_params: Union[Dict, TaxPredictParam, List[Union[TaxPredictParam, Dict]]] = None, callback: Callback = None, **kwargs):
+    def predict_brand(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.brand', task_params={'text_list': _params_convert(task_params)}, callback=callback, **kwargs)
```

### Comparing `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/SOURCES.txt` & `zcbot-predict-sdk-0.0.3/zcbot_predict_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 zcbot_predict_sdk/common/utils.py
 zcbot_predict_sdk/model/__init__.py
 zcbot_predict_sdk/model/callback.py
 zcbot_predict_sdk/model/param.py
 zcbot_predict_sdk/service/__init__.py
 zcbot_predict_sdk/service/base.py
 zcbot_predict_sdk/service/info_extract.py
-zcbot_predict_sdk/service/sku_tag.py
-zcbot_predict_sdk/service/tax.py
+zcbot_predict_sdk/service/sku_tag.py
```

