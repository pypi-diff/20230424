# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.879.tar", last modified: Fri Apr 21 01:08:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.880.tar", last modified: Mon Apr 24 03:47:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.879.tar` & `tencentcloud-sdk-python-trp-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139889 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)    43704 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:08:12.000000 tencentcloud-sdk-python-trp-3.0.879/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139995 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)    43764 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:47:30.000000 tencentcloud-sdk-python-trp-3.0.880/tencentcloud_sdk_python_trp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trp-3.0.879/README.rst` & `tencentcloud-sdk-python-trp-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1093,29 +1093,41 @@
         r"""
         :param BatchId: 批次ID
         :type BatchId: str
         :param CorpId: 企业ID
         :type CorpId: int
         :param Codes: 码
         :type Codes: list of CodeItem
+        :param CodeType: 码绑定激活策略，默认  0
+0: 传什么码就激活什么码
+1: 层级码 + 层级子码
+        :type CodeType: int
+        :param CheckType: 错误检查类型，默认 0
+0: 没有新导入码时正常返回
+1: 没有新导入码时报错，并返回没有导入成功的原因
+        :type CheckType: int
         """
         self.BatchId = None
         self.CorpId = None
         self.Codes = None
+        self.CodeType = None
+        self.CheckType = None
 
 
     def _deserialize(self, params):
         self.BatchId = params.get("BatchId")
         self.CorpId = params.get("CorpId")
         if params.get("Codes") is not None:
             self.Codes = []
             for item in params.get("Codes"):
                 obj = CodeItem()
                 obj._deserialize(item)
                 self.Codes.append(obj)
+        self.CodeType = params.get("CodeType")
+        self.CheckType = params.get("CheckType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3504,85 +3516,85 @@
         :type BatchId: str
         :param TaskId: 生产溯源任务ID
         :type TaskId: str
         :param TraceItems: 溯源信息
         :type TraceItems: list of TraceItem
         :param PhaseName: 溯源阶段名称
         :type PhaseName: str
+        :param PhaseData: 环节数据
+        :type PhaseData: :class:`tencentcloud.trp.v20210515.models.PhaseData`
+        :param Status: 溯源状态 0: 无效, 1: 有效
+        :type Status: int
+        :param Rank: 排序
+        :type Rank: int
         :param Type: [无效] 类型
         :type Type: int
         :param Code: [无效] 溯源码
         :type Code: str
-        :param Rank: [无效] 排序
-        :type Rank: int
         :param Phase: [无效] 溯源阶段 0:商品 1:通用 2:生产溯源 3:销售溯源
         :type Phase: int
         :param TraceTime: [无效] 溯源时间
         :type TraceTime: str
         :param CreateTime: [无效] 创建时间
         :type CreateTime: str
         :param ChainStatus: [无效] 上链状态
         :type ChainStatus: int
         :param ChainTime: [无效] 上链时间
         :type ChainTime: str
         :param ChainData: [无效] 上链数据
         :type ChainData: :class:`tencentcloud.trp.v20210515.models.ChainData`
         :param CorpId: 企业ID
         :type CorpId: int
-        :param Status: 溯源状态 0: 无效, 1: 有效
-        :type Status: int
-        :param PhaseData: 环节数据
-        :type PhaseData: :class:`tencentcloud.trp.v20210515.models.PhaseData`
         """
         self.TraceId = None
         self.BatchId = None
         self.TaskId = None
         self.TraceItems = None
         self.PhaseName = None
+        self.PhaseData = None
+        self.Status = None
+        self.Rank = None
         self.Type = None
         self.Code = None
-        self.Rank = None
         self.Phase = None
         self.TraceTime = None
         self.CreateTime = None
         self.ChainStatus = None
         self.ChainTime = None
         self.ChainData = None
         self.CorpId = None
-        self.Status = None
-        self.PhaseData = None
 
 
     def _deserialize(self, params):
         self.TraceId = params.get("TraceId")
         self.BatchId = params.get("BatchId")
         self.TaskId = params.get("TaskId")
         if params.get("TraceItems") is not None:
             self.TraceItems = []
             for item in params.get("TraceItems"):
                 obj = TraceItem()
                 obj._deserialize(item)
                 self.TraceItems.append(obj)
         self.PhaseName = params.get("PhaseName")
+        if params.get("PhaseData") is not None:
+            self.PhaseData = PhaseData()
+            self.PhaseData._deserialize(params.get("PhaseData"))
+        self.Status = params.get("Status")
+        self.Rank = params.get("Rank")
         self.Type = params.get("Type")
         self.Code = params.get("Code")
-        self.Rank = params.get("Rank")
         self.Phase = params.get("Phase")
         self.TraceTime = params.get("TraceTime")
         self.CreateTime = params.get("CreateTime")
         self.ChainStatus = params.get("ChainStatus")
         self.ChainTime = params.get("ChainTime")
         if params.get("ChainData") is not None:
             self.ChainData = ChainData()
             self.ChainData._deserialize(params.get("ChainData"))
         self.CorpId = params.get("CorpId")
-        self.Status = params.get("Status")
-        if params.get("PhaseData") is not None:
-            self.PhaseData = PhaseData()
-            self.PhaseData._deserialize(params.get("PhaseData"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4183,39 +4195,32 @@
     """溯源数据
 
     """
 
     def __init__(self):
         r"""
         :param TraceId: 溯源ID
-注意：此字段可能返回 null，表示取不到有效值。
         :type TraceId: str
         :param CorpId: 企业ID
-注意：此字段可能返回 null，表示取不到有效值。
         :type CorpId: int
         :param Type: 码类型 0: 批次, 1: 码, 2: 生产任务
-注意：此字段可能返回 null，表示取不到有效值。
         :type Type: int
         :param Code: 码值，跟码类型一一对应
 注意：此字段可能返回 null，表示取不到有效值。
         :type Code: str
         :param Rank: 排序，在Phase相同情况下，值越小排名靠前
-注意：此字段可能返回 null，表示取不到有效值。
         :type Rank: int
         :param Phase: 溯源阶段 0:商品 1:通用 2:生产溯源 3:销售溯源
-注意：此字段可能返回 null，表示取不到有效值。
         :type Phase: int
         :param PhaseName: 溯源环节名称
-注意：此字段可能返回 null，表示取不到有效值。
         :type PhaseName: str
         :param TraceTime: 溯源时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type TraceTime: str
         :param TraceItems: 无
-注意：此字段可能返回 null，表示取不到有效值。
         :type TraceItems: list of TraceItem
         :param CreateTime: 创建时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateTime: str
         :param ChainStatus: 上链状态 0: 未上链 1: 上链中 2: 已上链 -1: 异常
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChainStatus: int
@@ -4225,15 +4230,14 @@
         :param ChainData: 上链数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChainData: :class:`tencentcloud.trp.v20210515.models.ChainData`
         :param PhaseData: 溯源阶段配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type PhaseData: :class:`tencentcloud.trp.v20210515.models.PhaseData`
         :param Status: 溯源阶段状态 0: 无效, 1: 有效
-注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         """
         self.TraceId = None
         self.CorpId = None
         self.Type = None
         self.Code = None
         self.Rank = None
@@ -4280,73 +4284,88 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TraceItem(AbstractModel):
-    """溯源数据项
-    Type的枚举值
+    """溯源数据项 Type 的枚举值
+
     text:文本类型, longtext:长文本类型, banner:单图片类型, image:多图片类型, video:视频类型, mp:小程序类型
+
     具体组合如下
-    Type: "text" 文本类型, 对应值 Value: "文本字符串"
-    Type: "longtext" 长文本类型, 对应值 Value: "长文本字符串, 支持换行\n"
-    Type: "banner" 单图片类型, 对应图片地址 Value: "https://sample.cdn.com/xxx.jpg"
-    Type: "image" 多图片类型, 对应图片地址 Values: ["https://sample.cdn.com/1.jpg", "https://sample.cdn.com/2.jpg"]
-    Type: "video" 视频类型, 对应视频地址 Value: "https://sample.cdn.com/xxx.mp4"
-    Type: "mp" 小程序类型, 对应配置 Values: ["WXAPPID", "WXAPP_PATH", "跳转说明"]
+    - Type: "text" 文本类型, 对应值 Value: "文本字符串"
+    - Type: "longtext" 长文本类型, 对应值 Value: "长文本字符串, 支持换行\n"
+    - Type: "banner" 单图片类型, 对应图片地址 Value: "https://sample.cdn.com/xxx.jpg"
+    - Type: "image" 多图片类型, 对应图片地址 Values: ["https://sample.cdn.com/1.jpg", "https://sample.cdn.com/2.jpg"]
+    - Type: "video" 视频类型, 对应视频地址 Value: "https://sample.cdn.com/xxx.mp4"
+    - Type: "mp" 小程序类型, 对应配置 Values: ["WXAPPID", "WXAPP_PATH", "跳转说明"]
 
     """
 
     def __init__(self):
         r"""
         :param Name: 字段名称
-注意：此字段可能返回 null，表示取不到有效值。
         :type Name: str
         :param Value: 字段值
-注意：此字段可能返回 null，表示取不到有效值。
         :type Value: str
-        :param Type: 类型 text:文本类型, longtext:长文本类型, banner:单图片类型, image:多图片类型, video:视频类型, mp:小程序类型
-注意：此字段可能返回 null，表示取不到有效值。
+        :param Type: 字段类型
+text:文本类型, 
+longtext:长文本类型, banner:单图片类型, image:多图片类型,
+video:视频类型,
+mp:小程序类型
         :type Type: str
         :param ReadOnly: 只读
-注意：此字段可能返回 null，表示取不到有效值。
         :type ReadOnly: bool
         :param Hidden: 扫码展示
-注意：此字段可能返回 null，表示取不到有效值。
         :type Hidden: bool
         :param Values: 多个值
-注意：此字段可能返回 null，表示取不到有效值。
         :type Values: list of str
         :param Key: 类型标识
-注意：此字段可能返回 null，表示取不到有效值。
         :type Key: str
         :param Ext: 扩展字段
-注意：此字段可能返回 null，表示取不到有效值。
         :type Ext: str
+        :param Attrs: 额外属性
+        :type Attrs: list of TraceItem
+        :param List: 子页面，只读
+        :type List: list of TraceData
         """
         self.Name = None
         self.Value = None
         self.Type = None
         self.ReadOnly = None
         self.Hidden = None
         self.Values = None
         self.Key = None
         self.Ext = None
+        self.Attrs = None
+        self.List = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Value = params.get("Value")
         self.Type = params.get("Type")
         self.ReadOnly = params.get("ReadOnly")
         self.Hidden = params.get("Hidden")
         self.Values = params.get("Values")
         self.Key = params.get("Key")
         self.Ext = params.get("Ext")
+        if params.get("Attrs") is not None:
+            self.Attrs = []
+            for item in params.get("Attrs"):
+                obj = TraceItem()
+                obj._deserialize(item)
+                self.Attrs.append(obj)
+        if params.get("List") is not None:
+            self.List = []
+            for item in params.get("List"):
+                obj = TraceData()
+                obj._deserialize(item)
+                self.List.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-trp-3.0.879/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.880/tencentcloud/trp/v20210515/trp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTraceCodes(self, request):
-        """批量导入二维码，只支持平台发的码
+        """批量绑定指定批次并激活二维码，只支持平台发的码，且只会激活没有使用过的码
 
         :param request: Request instance for CreateTraceCodes.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateTraceCodesRequest`
         :rtype: :class:`tencentcloud.trp.v20210515.models.CreateTraceCodesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-trp-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trp-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.880/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.879/setup.py` & `tencentcloud-sdk-python-trp-3.0.880/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.879/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.880/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

