# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.879.tar", last modified: Fri Apr 21 00:58:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.880.tar", last modified: Mon Apr 24 03:25:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.879.tar` & `tencentcloud-sdk-python-scf-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    42711 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)    31630 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190870 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:58:45.000000 tencentcloud-sdk-python-scf-3.0.879/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)    31630 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191185 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:25:32.000000 tencentcloud-sdk-python-scf-3.0.880/tencentcloud_sdk_python_scf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-scf-3.0.879/README.rst` & `tencentcloud-sdk-python-scf-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.879/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.880/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3275,16 +3275,17 @@
         :type Offset: int
         :param Limit: 返回数据长度，默认值为 20
         :type Limit: int
         :param OrderBy: 根据哪个字段进行返回结果排序,支持以下字段：add_time，mod_time，默认mod_time
         :type OrderBy: str
         :param Order: 以升序还是降序的方式返回结果，可选值 ASC 和 DESC，默认DESC
         :type Order: str
-        :param Filters: * Qualifier:
-函数版本，别名
+        :param Filters: * Qualifier: 函数版本，别名
+* TriggerName: 函数触发器名称
+* Description: 函数触发器描述
         :type Filters: list of Filter
         """
         self.FunctionName = None
         self.Namespace = None
         self.Offset = None
         self.Limit = None
         self.OrderBy = None
@@ -4584,27 +4585,31 @@
         :type ModTime: str
         :param ResourceId: 触发器最小资源ID
         :type ResourceId: str
         :param BindStatus: 触发器和云函数绑定状态
         :type BindStatus: str
         :param TriggerAttribute: 触发器类型，双向表示两侧控制台均可操作，单向表示SCF控制台单向创建
         :type TriggerAttribute: str
+        :param Description: 客户自定义触发器描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
         """
         self.Enable = None
         self.Qualifier = None
         self.TriggerName = None
         self.Type = None
         self.TriggerDesc = None
         self.AvailableStatus = None
         self.CustomArgument = None
         self.AddTime = None
         self.ModTime = None
         self.ResourceId = None
         self.BindStatus = None
         self.TriggerAttribute = None
+        self.Description = None
 
 
     def _deserialize(self, params):
         self.Enable = params.get("Enable")
         self.Qualifier = params.get("Qualifier")
         self.TriggerName = params.get("TriggerName")
         self.Type = params.get("Type")
@@ -4612,14 +4617,15 @@
         self.AvailableStatus = params.get("AvailableStatus")
         self.CustomArgument = params.get("CustomArgument")
         self.AddTime = params.get("AddTime")
         self.ModTime = params.get("ModTime")
         self.ResourceId = params.get("ResourceId")
         self.BindStatus = params.get("BindStatus")
         self.TriggerAttribute = params.get("TriggerAttribute")
+        self.Description = params.get("Description")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-scf-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.880/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.879/setup.py` & `tencentcloud-sdk-python-scf-3.0.880/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.879/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.880/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

