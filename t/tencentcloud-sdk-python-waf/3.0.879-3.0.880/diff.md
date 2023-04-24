# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.879.tar", last modified: Fri Apr 21 01:09:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.880.tar", last modified: Mon Apr 24 03:49:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.879.tar` & `tencentcloud-sdk-python-waf-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46564 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177630 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:09:50.000000 tencentcloud-sdk-python-waf-3.0.879/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46564 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179442 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:49:28.000000 tencentcloud-sdk-python-waf-3.0.880/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.879/README.rst` & `tencentcloud-sdk-python-waf-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.879/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.880/tencentcloud/waf/v20180125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
     def __init__(self):
         r"""
         :param Name: 规则名称
         :type Name: str
         :param SortId: 优先级
         :type SortId: str
-        :param ExpireTime: 过期时间
+        :param ExpireTime: 过期时间，单位为秒级时间戳，例如1677254399表示过期时间为2023-02-24 23:59:59. 0表示永不过期
         :type ExpireTime: str
         :param Strategies: 策略详情
         :type Strategies: list of Strategy
         :param Domain: 需要添加策略的域名
         :type Domain: str
         :param ActionType: 动作类型，1代表阻断，2代表人机识别，3代表观察，4代表重定向
         :type ActionType: str
@@ -1723,31 +1723,35 @@
         :type AttackCount: int
         :param ACLCount: 访问控制总数
         :type ACLCount: int
         :param CCCount: CC攻击总数
         :type CCCount: int
         :param BotCount: Bot攻击总数
         :type BotCount: int
+        :param ApiAssetsCount: api资产总数
+        :type ApiAssetsCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.AccessCount = None
         self.AttackCount = None
         self.ACLCount = None
         self.CCCount = None
         self.BotCount = None
+        self.ApiAssetsCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.AccessCount = params.get("AccessCount")
         self.AttackCount = params.get("AttackCount")
         self.ACLCount = params.get("ACLCount")
         self.CCCount = params.get("CCCount")
         self.BotCount = params.get("BotCount")
+        self.ApiAssetsCount = params.get("ApiAssetsCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeAutoDenyIPRequest(AbstractModel):
     """DescribeAutoDenyIP请求参数结构体
 
     """
@@ -1861,25 +1865,29 @@
         :type RuleId: str
         :param SortId: 优先级
         :type SortId: str
         :param Status: 状态
         :type Status: str
         :param Strategies: 策略详情
         :type Strategies: list of Strategy
+        :param EventId: 事件id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EventId: str
         """
         self.ActionType = None
         self.Bypass = None
         self.CreateTime = None
         self.ExpireTime = None
         self.Name = None
         self.Redirect = None
         self.RuleId = None
         self.SortId = None
         self.Status = None
         self.Strategies = None
+        self.EventId = None
 
 
     def _deserialize(self, params):
         self.ActionType = params.get("ActionType")
         self.Bypass = params.get("Bypass")
         self.CreateTime = params.get("CreateTime")
         self.ExpireTime = params.get("ExpireTime")
@@ -1890,14 +1898,15 @@
         self.Status = params.get("Status")
         if params.get("Strategies") is not None:
             self.Strategies = []
             for item in params.get("Strategies"):
                 obj = Strategy()
                 obj._deserialize(item)
                 self.Strategies.append(obj)
+        self.EventId = params.get("EventId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3440,15 +3449,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class FiltersItemNew(AbstractModel):
-    """实例入参过滤器
+    """过滤数组
 
     """
 
     def __init__(self):
         r"""
         :param Name: 字段名
         :type Name: str
@@ -3669,15 +3678,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceId: id
         :type InstanceId: str
-        :param InstanceName: name
+        :param InstanceName: Name
         :type InstanceName: str
         :param ResourceIds: 资源id
         :type ResourceIds: str
         :param Region: 地域
         :type Region: str
         :param PayMode: 付费模式
         :type PayMode: int
@@ -3723,14 +3732,28 @@
         :type ElasticBilling: int
         :param AttackLogPost: 攻击日志投递开关
 注意：此字段可能返回 null，表示取不到有效值。
         :type AttackLogPost: int
         :param MaxBandwidth: 带宽峰值
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxBandwidth: int
+        :param APISecurity: api安全是否购买
+        :type APISecurity: int
+        :param QpsStandard: 购买的qps规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QpsStandard: int
+        :param BandwidthStandard: 购买的带宽规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BandwidthStandard: int
+        :param Status: 实例状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param SandboxQps: 实例沙箱值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SandboxQps: int
         """
         self.InstanceId = None
         self.InstanceName = None
         self.ResourceIds = None
         self.Region = None
         self.PayMode = None
         self.RenewFlag = None
@@ -3749,14 +3772,19 @@
         self.Edition = None
         self.FraudPkg = None
         self.BotPkg = None
         self.BotQPS = None
         self.ElasticBilling = None
         self.AttackLogPost = None
         self.MaxBandwidth = None
+        self.APISecurity = None
+        self.QpsStandard = None
+        self.BandwidthStandard = None
+        self.Status = None
+        self.SandboxQps = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.ResourceIds = params.get("ResourceIds")
         self.Region = params.get("Region")
@@ -3787,14 +3815,19 @@
             self.BotPkg._deserialize(params.get("BotPkg"))
         if params.get("BotQPS") is not None:
             self.BotQPS = BotQPS()
             self.BotQPS._deserialize(params.get("BotQPS"))
         self.ElasticBilling = params.get("ElasticBilling")
         self.AttackLogPost = params.get("AttackLogPost")
         self.MaxBandwidth = params.get("MaxBandwidth")
+        self.APISecurity = params.get("APISecurity")
+        self.QpsStandard = params.get("QpsStandard")
+        self.BandwidthStandard = params.get("BandwidthStandard")
+        self.Status = params.get("Status")
+        self.SandboxQps = params.get("SandboxQps")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5083,20 +5116,24 @@
     """自定义规则的匹配条件结构体
 
     """
 
     def __init__(self):
         r"""
         :param Field: 匹配字段
+注意：此字段可能返回 null，表示取不到有效值。
         :type Field: str
         :param CompareFunc: 逻辑符号
+注意：此字段可能返回 null，表示取不到有效值。
         :type CompareFunc: str
         :param Content: 匹配内容
+注意：此字段可能返回 null，表示取不到有效值。
         :type Content: str
         :param Arg: 匹配参数
+注意：此字段可能返回 null，表示取不到有效值。
         :type Arg: str
         """
         self.Field = None
         self.CompareFunc = None
         self.Content = None
         self.Arg = None
```

### Comparing `tencentcloud-sdk-python-waf-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.880/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.879/setup.py` & `tencentcloud-sdk-python-waf-3.0.880/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.879/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.880/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

