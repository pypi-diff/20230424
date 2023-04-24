# Comparing `tmp/zcbot-predict-sdk-0.0.1.tar.gz` & `tmp/zcbot-predict-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-predict-sdk-0.0.1.tar", last modified: Tue Apr 18 08:49:28 2023, max compression
+gzip compressed data, was "dist\zcbot-predict-sdk-0.0.2.tar", last modified: Mon Apr 24 13:05:13 2023, max compression
```

## Comparing `zcbot-predict-sdk-0.0.1.tar` & `zcbot-predict-sdk-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:49:28.898163 zcbot-predict-sdk-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      384 2023-04-18 08:49:28.897165 zcbot-predict-sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-18 08:49:28.898163 zcbot-predict-sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-04-18 08:49:16.000000 zcbot-predict-sdk-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:49:28.869164 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/__init__.py
--rw-rw-rw-   0        0        0     6559 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:49:28.882165 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/decator.py
--rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/exceptions.py
--rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/keys.py
--rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/thread_pool.py
--rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:49:28.886165 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/model/
--rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/model/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/model/callback.py
--rw-rw-rw-   0        0        0      814 2023-04-13 04:41:45.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/model/param.py
--rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/monitor.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:49:28.895165 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/
--rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/base.py
--rw-rw-rw-   0        0        0     1647 2023-03-24 12:37:57.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/catalog.py
--rw-rw-rw-   0        0        0      513 2023-04-13 01:36:51.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/info_extract.py
--rw-rw-rw-   0        0        0      458 2023-03-28 06:59:48.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/oss.py
--rw-rw-rw-   0        0        0     1690 2023-04-13 04:41:45.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/sku_search.py
--rw-rw-rw-   0        0        0      619 2023-03-24 06:26:54.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/tax.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:49:28.875165 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/
--rw-rw-rw-   0        0        0      384 2023-04-18 08:49:28.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-04-18 08:49:28.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 08:49:28.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 08:49:28.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-18 08:49:28.000000 zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.033677 zcbot-predict-sdk-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      384 2023-04-24 13:05:13.033677 zcbot-predict-sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:05:13.034676 zcbot-predict-sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-04-24 13:05:09.000000 zcbot-predict-sdk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.005678 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/__init__.py
+-rw-rw-rw-   0        0        0     7158 2023-04-23 02:14:35.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.019677 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/decator.py
+-rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/exceptions.py
+-rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/keys.py
+-rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/thread_pool.py
+-rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.024678 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/
+-rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/callback.py
+-rw-rw-rw-   0        0        0      404 2023-04-24 12:19:13.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/param.py
+-rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.031676 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/
+-rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/base.py
+-rw-rw-rw-   0        0        0      584 2023-04-24 13:01:27.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/info_extract.py
+-rw-rw-rw-   0        0        0     4066 2023-04-24 12:24:32.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/sku_tag.py
+-rw-rw-rw-   0        0        0      619 2023-03-24 06:26:54.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/tax.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:05:13.011676 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 13:05:12.000000 zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-predict-sdk-0.0.1/setup.py` & `zcbot-predict-sdk-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-predict-sdk',
-      version='0.0.1',
+      version='0.0.2',
       description='zcbot predict sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['celery', 'redis'],
       python_requires='>=3.7',
```

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/client.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # @singleton
 class CeleryClient(object):
     """
     Celery服务客户端
     注意：此类不建议手动初始化，可通过CeleryClientHolder初始化，方便各service类自动获取
     """
-
     def __init__(self, celery_broker_url: str, celery_result_backend: str, client_redis_uri: str, app_code: str):
         self.broker_url = celery_broker_url
         self.backend_uri = celery_result_backend
         self.client_redis_uri = client_redis_uri
         self.app_code = app_code
         self.default_expire_seconds = 12 * 3600
         self.celery_client = Celery(
@@ -30,35 +29,39 @@
             broker=self.broker_url,
             backend=self.backend_uri,
             task_acks_late=True
         )
         self.rds_client = Redis.from_url(url=client_redis_uri, decode_responses=True)
         self.task_map = dict()
 
-    def apply_group(self, task_name: str, task_params_list: List[Dict] = None, options: Dict = None, callback: Callback = None, timeout: float = None, **kwargs):
+    def apply_group(self, task_name: str, task_params_list: List[Dict] = None, options: Dict = None, callback: Callback = None, queue_name: str = None, timeout: float = None, **kwargs):
         """
         服务组调用
-        :param task_name:
-        :param task_params_list:
-        :param callback:
+        :param task_name: 任务名称
+        :param task_params_list: 任务参数清单
+        :param timeout: 【可选参数】超时时间
+        :param queue_name: 【可选参数】任务队列名称，默认`task.{task_name}`
+        :param options: 【可选参数】配置项
+        :param callback: 【可选参数】回调函数
         :param kwargs:
         :return:
         """
         try:
             # 同步/异步
             _headers = {'app_code': self.app_code}
             if callback and callback.app_code:
                 _headers['app_code'] = callback.app_code or self.app_code
 
             # 调用
             task_list = []
             for task_params in task_params_list:
                 task_list.append(self.get_task_by_name(task_name).signature(kwargs=task_params, options=options))
             task_group = group(task_list)
-            async_result = task_group.apply_async(queue=f'task.{task_name}', headers=_headers)
+            _queue_name = queue_name or f'task.{task_name}'
+            async_result = task_group.apply_async(queue=_queue_name, headers=_headers)
 
             # 结果
             if callback:
                 # 【异步】绑定回调处理函数
                 LOGGER.info(f'[服务组]异步调用 task={task_name}')
                 self._bind_callback(task_name, async_result, callback)
                 return async_result
@@ -72,31 +75,33 @@
                 rs = async_result.get(timeout=_timeout)
                 async_result.forget()
                 return rs
         except Exception as e:
             LOGGER.error(f'处理异常: task_name={task_name}, kwargs={len(task_params_list)}, e={e}')
             raise e
 
-    def apply(self, task_name: str, task_params: Dict = None, callback: Callback = None, timeout: float = None, **kwargs):
+    def apply(self, task_name: str, task_params: Dict = None, callback: Callback = None, queue_name: str = None, timeout: float = None, **kwargs):
         """
         单任务请求调用
-        :param task_name:
-        :param task_params:
-        :param callback:
-        :param timeout:
+        :param task_name: 任务名称
+        :param task_params: 任务参数字典
+        :param callback:【可选参数】回调函数
+        :param queue_name:【可选参数】任务队列名称，默认`task.{task_name}`
+        :param timeout:【可选参数】超时时间
         :param kwargs:
         :return:
         """
         try:
             # 同步/异步
             _headers = {'app_code': self.app_code}
             if callback and callback.app_code:
                 _headers['app_code'] = callback.app_code or self.app_code
             # 调用
-            async_result = self.get_task_by_name(task_name).apply_async(kwargs=task_params, queue=f'task.{task_name}', headers=_headers)
+            _queue_name = queue_name or f'task.{task_name}'
+            async_result = self.get_task_by_name(task_name).apply_async(kwargs=task_params, queue=_queue_name, headers=_headers)
             # 结果
             if callback:
                 # 【异步】绑定回调处理函数
                 LOGGER.info(f'[服务]异步调用 task={task_name}')
                 self._bind_callback(task_name, async_result, callback)
                 return async_result
             else:
```

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/exceptions.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/thread_pool.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/common/utils.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/model/callback.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/model/callback.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/monitor.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/catalog.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/tax.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,12 @@
-from typing import Dict
-
 from .base import BaseService
 from ..model.callback import Callback
-from ..model.param import InfoPredictParam
-
-
-class StaplesCatalogService(BaseService):
-
-    def predict_catalog1(self, task_params: InfoPredictParam = None, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='catalog.staples1', task_params=task_params.dict(), callback=callback,
-                                        **kwargs)
-
-    def predict_catalog4(self, task_params: InfoPredictParam = None, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='catalog.staples4', task_params=task_params.dict(), callback=callback,
-                                        **kwargs)
-
-    def predict_catalog6(self, task_params: InfoPredictParam = None, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='catalog.staples6', task_params=task_params.dict(), callback=callback,
-                                        **kwargs)
+from ..model.param import TaxPredictParam
 
 
-class JslinkCatalogService(BaseService):
+class TaxService(BaseService):
 
-    def predict_catalog1(self, task_params: InfoPredictParam = None, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='catalog.jslink1', task_params=task_params.dict(), callback=callback,
-                                        **kwargs)
+    def get_tax_by_baiwang(self, task_params: TaxPredictParam = None, callback: Callback = None, **kwargs):
+        return self.celery_client.apply(task_name='tax.baiwang', task_params=task_params.dict(), callback=callback, **kwargs)
 
-    def predict_catalog4(self, task_params: InfoPredictParam = None, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='catalog.jslink4', task_params=task_params.dict(), callback=callback,
-                                        **kwargs)
+    def get_tax_by_demo(self, task_params: TaxPredictParam = None, callback: Callback = None, **kwargs):
+        return self.celery_client.apply(task_name='tax.demo', task_params=task_params.dict(), callback=callback, **kwargs)
```

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk/service/info_extract.py` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk/service/info_extract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Dict
-
+from typing import Union, Dict, List
 from .base import BaseService
 from ..model.callback import Callback
-from ..model.param import InfoPredictParam
+from ..model.param import InfoExtractParam
 
 
-class BrandNameModelExtractService(BaseService):
+class InfoExtractService(BaseService):
     """品牌、型号、通用名"""
 
-    def info_extract(self, task_params: InfoPredictParam = None, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='info_extract.bnm', task_params=task_params.dict(), callback=callback,
-                                        **kwargs)
+    def extract_sku(self, task_params: Union[Dict, InfoExtractParam] = None, callback: Callback = None, **kwargs):
+        _task_params = task_params.dict() if isinstance(task_params, InfoExtractParam) else task_params
+        return self.celery_client.apply(task_name='info_extract.sku', task_params=_task_params, callback=callback, **kwargs)
```

### Comparing `zcbot-predict-sdk-0.0.1/zcbot_predict_sdk.egg-info/SOURCES.txt` & `zcbot-predict-sdk-0.0.2/zcbot_predict_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,12 +16,10 @@
 zcbot_predict_sdk/common/thread_pool.py
 zcbot_predict_sdk/common/utils.py
 zcbot_predict_sdk/model/__init__.py
 zcbot_predict_sdk/model/callback.py
 zcbot_predict_sdk/model/param.py
 zcbot_predict_sdk/service/__init__.py
 zcbot_predict_sdk/service/base.py
-zcbot_predict_sdk/service/catalog.py
 zcbot_predict_sdk/service/info_extract.py
-zcbot_predict_sdk/service/oss.py
-zcbot_predict_sdk/service/sku_search.py
+zcbot_predict_sdk/service/sku_tag.py
 zcbot_predict_sdk/service/tax.py
```

