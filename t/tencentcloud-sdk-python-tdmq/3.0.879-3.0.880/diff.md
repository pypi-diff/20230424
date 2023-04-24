# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.879.tar", last modified: Fri Apr 21 01:02:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.880.tar", last modified: Mon Apr 24 03:39:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.879.tar` & `tencentcloud-sdk-python-tdmq-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)    99909 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   372127 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:02:38.000000 tencentcloud-sdk-python-tdmq-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   101085 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   374030 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2199,14 +2199,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyRocketMQInstanceSpec(self, request):
+        """本API用于修改RocketMQ专享实例配置，可以支持实例规格、节点数和存储的升配和实例规格的降配。本API发起订单并成功支付后进入实例配置变更的流程，可通过DescribeRocketMQVipInstances查询实例是否已变更完成。
+
+        :param request: Request instance for ModifyRocketMQInstanceSpec.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQInstanceSpecRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQInstanceSpecResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyRocketMQInstanceSpec", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyRocketMQInstanceSpecResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyRocketMQNamespace(self, request):
         """更新RocketMQ命名空间
 
         :param request: Request instance for ModifyRocketMQNamespace.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQNamespaceRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.ModifyRocketMQNamespaceResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 # CAM鉴权不通过。
 AUTHFAILURE_UNAUTHORIZEDOPERATION = 'AuthFailure.UnauthorizedOperation'
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
+# 调用交易服务发生异常。
+FAILEDOPERATION_CALLTRADE = 'FailedOperation.CallTrade'
+
 # CMQ 后台服务错误。
 FAILEDOPERATION_CMQBACKENDERROR = 'FailedOperation.CmqBackendError'
 
 # 创建vpc绑定关系失败。
 FAILEDOPERATION_CREATEBINDVPC = 'FailedOperation.CreateBindVpc'
 
 # 创建集群失败。
@@ -82,14 +85,17 @@
 
 # 获取环境属性失败。
 FAILEDOPERATION_GETENVIRONMENTATTRIBUTESFAILED = 'FailedOperation.GetEnvironmentAttributesFailed'
 
 # 获取主题分区数失败。
 FAILEDOPERATION_GETTOPICPARTITIONSFAILED = 'FailedOperation.GetTopicPartitionsFailed'
 
+# 实例尚未就绪，请稍后再试。
+FAILEDOPERATION_INSTANCENOTREADY = 'FailedOperation.InstanceNotReady'
+
 # 最大消息超过1MB。
 FAILEDOPERATION_MAXMESSAGESIZEERROR = 'FailedOperation.MaxMessageSizeError'
 
 # 上传的msgID错误。
 FAILEDOPERATION_MESSAGEIDERROR = 'FailedOperation.MessageIDError'
 
 # 必须先清除关联命名空间才能继续操作。
@@ -309,7 +315,10 @@
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# 该实例不支持降配操作。
+UNSUPPORTEDOPERATION_INSTANCEDOWNGRADE = 'UnsupportedOperation.InstanceDowngrade'
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7487,14 +7487,76 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyRocketMQInstanceSpecRequest(AbstractModel):
+    """ModifyRocketMQInstanceSpec请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 专享实例ID
+        :type InstanceId: str
+        :param Specification: 实例规格，
+rocket-vip-basic-1 基础型
+rocket-vip-basic-2 标准型
+rocket-vip-basic-3 高阶Ⅰ型
+rocket-vip-basic-4 高阶Ⅱ型
+        :type Specification: str
+        :param NodeCount: 节点数量
+        :type NodeCount: int
+        :param StorageSize: 存储空间，GB为单位
+        :type StorageSize: int
+        """
+        self.InstanceId = None
+        self.Specification = None
+        self.NodeCount = None
+        self.StorageSize = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.Specification = params.get("Specification")
+        self.NodeCount = params.get("NodeCount")
+        self.StorageSize = params.get("StorageSize")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyRocketMQInstanceSpecResponse(AbstractModel):
+    """ModifyRocketMQInstanceSpec返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OrderId: 订单号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OrderId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.OrderId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.OrderId = params.get("OrderId")
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyRocketMQNamespaceRequest(AbstractModel):
     """ModifyRocketMQNamespace请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.880/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.879/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.880/setup.py`

 * *Files identical despite different names*

