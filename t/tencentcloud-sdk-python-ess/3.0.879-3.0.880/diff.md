# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.879.tar", last modified: Fri Apr 21 00:44:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.880.tar", last modified: Mon Apr 24 03:04:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.879.tar` & `tencentcloud-sdk-python-ess-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49192 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219062 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49192 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219487 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.879/README.rst` & `tencentcloud-sdk-python-ess-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1585,39 +1585,39 @@
 
     def __init__(self):
         r"""
         :param FlowId: 流程编号
         :type FlowId: str
         :param FlowApproverInfos: 流程签署人，其中ApproverName，ApproverMobile和ApproverType必传，其他可不传，ApproverType目前只支持个人类型的签署人。还需注意签署人只能有手写签名和时间类型的签署控件，其他类型的填写控件和签署控件暂时都未支持。
         :type FlowApproverInfos: list of FlowCreateApprover
-        :param Organization: 机构信息，暂未开放
-        :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
         :param Operator: 用户信息，此结构体UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param Organization: 机构信息，暂未开放
+        :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
         """
         self.FlowId = None
         self.FlowApproverInfos = None
-        self.Organization = None
         self.Operator = None
+        self.Organization = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         if params.get("FlowApproverInfos") is not None:
             self.FlowApproverInfos = []
             for item in params.get("FlowApproverInfos"):
                 obj = FlowCreateApprover()
                 obj._deserialize(item)
                 self.FlowApproverInfos.append(obj)
-        if params.get("Organization") is not None:
-            self.Organization = OrganizationInfo()
-            self.Organization._deserialize(params.get("Organization"))
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
+        if params.get("Organization") is not None:
+            self.Organization = OrganizationInfo()
+            self.Organization._deserialize(params.get("Organization"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4047,32 +4047,37 @@
         :type FlowStatus: int
         :param CreatedOn: 流程创建的时间戳
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreatedOn: int
         :param FlowMessage: 拒签或者取消的原因描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowMessage: str
+        :param Creator:  合同发起人userId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Creator: str
         """
         self.FlowId = None
         self.FlowName = None
         self.FlowDescription = None
         self.FlowType = None
         self.FlowStatus = None
         self.CreatedOn = None
         self.FlowMessage = None
+        self.Creator = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.FlowName = params.get("FlowName")
         self.FlowDescription = params.get("FlowDescription")
         self.FlowType = params.get("FlowType")
         self.FlowStatus = params.get("FlowStatus")
         self.CreatedOn = params.get("CreatedOn")
         self.FlowMessage = params.get("FlowMessage")
+        self.Creator = params.get("Creator")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4211,24 +4216,28 @@
         :type FlowDescription: str
         :param CreatedOn: 合同(流程)的创建时间戳
         :type CreatedOn: int
         :param FlowApproverInfos: 合同(流程)的签署人数组
         :type FlowApproverInfos: list of FlowApproverDetail
         :param CcInfos: 合同(流程)的关注方信息列表
         :type CcInfos: list of FlowApproverDetail
+        :param Creator: 合同发起人UserId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Creator: str
         """
         self.FlowId = None
         self.FlowName = None
         self.FlowType = None
         self.FlowStatus = None
         self.FlowMessage = None
         self.FlowDescription = None
         self.CreatedOn = None
         self.FlowApproverInfos = None
         self.CcInfos = None
+        self.Creator = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.FlowName = params.get("FlowName")
         self.FlowType = params.get("FlowType")
         self.FlowStatus = params.get("FlowStatus")
@@ -4243,14 +4252,15 @@
                 self.FlowApproverInfos.append(obj)
         if params.get("CcInfos") is not None:
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = FlowApproverDetail()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
+        self.Creator = params.get("Creator")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.880/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.879/setup.py` & `tencentcloud-sdk-python-ess-3.0.880/setup.py`

 * *Files identical despite different names*

