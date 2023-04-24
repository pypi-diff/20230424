# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.879.tar", last modified: Fri Apr 21 01:08:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.880.tar", last modified: Mon Apr 24 03:47:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.879.tar` & `tencentcloud-sdk-python-trtc-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198942 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58202 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:08:26.000000 tencentcloud-sdk-python-trtc-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198942 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58535 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:47:44.000000 tencentcloud-sdk-python-trtc-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/README.rst` & `tencentcloud-sdk-python-trtc-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,14 +481,16 @@
     def DescribeTRTCRealTimeScaleMetricData(self, request):
         """查询TRTC监控仪表盘-实时监控规模指标（会返回下列指标）
         -userCount（在线用户数）
         -roomCount（在线房间数）
         注意：
         1.调用接口需开通监控仪表盘【基础版】和【进阶版】，监控仪表盘【免费版】不支持调用，监控仪表盘版本功能和计费说明：https://cloud.tencent.com/document/product/647/81331。
         2.查询时间范围根据监控仪表盘功能版本而定，基础版可查近3小时，进阶版可查近12小时。
+        xa0
+        3.除此之外您也可以通过订阅TRTC包月套餐(https://buy.cloud.tencent.com/trtc)尊享版或旗舰版解锁此接口（DescribeTRTCRealTimeScaleMetricData）的调用能力，请在开通包月套餐后，请提交工单联系售后解锁调用能力https://console.cloud.tencent.com/workorder/category
 
         :param request: Request instance for DescribeTRTCRealTimeScaleMetricData.
         :type request: :class:`tencentcloud.trtc.v20190722.models.DescribeTRTCRealTimeScaleMetricDataRequest`
         :rtype: :class:`tencentcloud.trtc.v20190722.models.DescribeTRTCRealTimeScaleMetricDataResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.880/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.879'
+__version__ = '3.0.880'
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.880/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.880/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.879/setup.py` & `tencentcloud-sdk-python-trtc-3.0.880/setup.py`

 * *Files identical despite different names*

