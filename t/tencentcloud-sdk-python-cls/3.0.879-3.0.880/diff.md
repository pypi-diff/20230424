# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.879.tar", last modified: Fri Apr 21 00:40:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.880.tar", last modified: Mon Apr 24 02:56:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.879.tar` & `tencentcloud-sdk-python-cls-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248846 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67922 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:40:54.000000 tencentcloud-sdk-python-cls-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248744 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67922 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 02:56:09.000000 tencentcloud-sdk-python-cls-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.879/README.rst` & `tencentcloud-sdk-python-cls-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2894,45 +2894,34 @@
 class DescribeAlarmsRequest(AbstractModel):
     """DescribeAlarms请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: <br><li> name
-
-按照【告警策略名称】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> alarmId
-
-按照【告警策略ID】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> topicId
-
-按照【监控对象的日志主题ID】进行过滤。
-
-类型：String
-
-必选：否
-
-<br><li> enable
-
-按照【启用状态】进行过滤。
-
-类型：String
-
-备注：enable参数值范围: 1, t, T, TRUE, true, True, 0, f, F, FALSE, false, False。 其它值将返回参数错误信息.
-
-必选：否
+        :param Filters: name
+- 按照【告警策略名称】进行过滤。
+- 类型：String
+- 必选：否
+
+alarmId
+- 按照【告警策略ID】进行过滤。
+- 类型：String
+- 必选：否
+
+topicId
+- 按照【监控对象的日志主题ID】进行过滤。
+- 类型：String
+- 必选：否
+
+enable
+- 按照【启用状态】进行过滤。
+- 类型：String
+- 备注：enable参数值范围: 1, t, T, TRUE, true, True, 0, f, F, FALSE, false, False。 其它值将返回参数错误信息.
+- 必选：否
 
 每次请求的Filters的上限为10，Filter.Values的上限为5。
         :type Filters: list of Filter
         :param Offset: 分页的偏移量，默认值为0。
         :type Offset: int
         :param Limit: 分页单页限制数目，默认值为20，最大值100。
         :type Limit: int
@@ -3192,35 +3181,28 @@
 class DescribeConfigsRequest(AbstractModel):
     """DescribeConfigs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: <br><li> configName
-
-按照【采集配置名称】进行模糊匹配过滤。
-类型：String
-
-必选：否
-
-<br><li> configId
-
-按照【采集配置ID】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> topicId
-
-按照【日志主题】进行过滤。
-
-类型：String
-
-必选：否
+        :param Filters: configName
+- 按照【采集配置名称】进行模糊匹配过滤。
+- 类型：String
+- 必选：否
+
+configId
+- 按照【采集配置ID】进行过滤。
+- 类型：String
+- 必选：否
+
+topicId
+- 按照【日志主题】进行过滤。
+- 类型：String
+- 必选：否
 
 每次请求的Filters的上限为10，Filter.Values的上限为5。
         :type Filters: list of Filter
         :param Offset: 分页的偏移量，默认值为0
         :type Offset: int
         :param Limit: 分页单页的限制数目，默认值为20，最大值100
         :type Limit: int
@@ -3697,43 +3679,33 @@
 class DescribeLogsetsRequest(AbstractModel):
     """DescribeLogsets请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: <br><li> logsetName
-
-按照【日志集名称】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> logsetId
-
-按照【日志集ID】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> tagKey
-
-按照【标签键】进行过滤。
-
-类型：String
-
-必选：否
-
-<br><li> tag:tagKey
-
-按照【标签键值对】进行过滤。tagKey使用具体的标签键进行替换。
-类型：String
-
-必选：否
-
+        :param Filters: logsetName
+- 按照【日志集名称】进行过滤。
+- 类型：String
+- 必选：否
+
+logsetId
+- 按照【日志集ID】进行过滤。
+- 类型：String
+- 必选：否
+
+tagKey
+- 按照【标签键】进行过滤。
+- 类型：String
+- 必选：否
+
+tag:tagKey
+- 按照【标签键值对】进行过滤。tagKey使用具体的标签键进行替换。
+- 类型：String
+- 必选：否
 
 每次请求的Filters的上限为10，Filter.Values的上限为5。
         :type Filters: list of Filter
         :param Offset: 分页的偏移量，默认值为0
         :type Offset: int
         :param Limit: 分页单页的限制数目，默认值为20，最大值100
         :type Limit: int
@@ -3845,43 +3817,33 @@
 class DescribeMachineGroupsRequest(AbstractModel):
     """DescribeMachineGroups请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: <br><li> machineGroupName
-
-按照【机器组名称】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> machineGroupId
-
-按照【机器组ID】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> tagKey
-
-按照【标签键】进行过滤。
-
-类型：String
-
-必选：否
-
-<br><li> tag:tagKey
-
-按照【标签键值对】进行过滤。tagKey使用具体的标签键进行替换。
-类型：String
-
-必选：否
-
+        :param Filters: machineGroupName
+- 按照【机器组名称】进行过滤。
+- 类型：String
+- 必选：否
+
+machineGroupId
+- 按照【机器组ID】进行过滤。
+- 类型：String
+- 必选：否
+
+tagKey
+- 按照【标签键】进行过滤。
+- 类型：String
+- 必选：否
+
+tag:tagKey
+- 按照【标签键值对】进行过滤。tagKey使用具体的标签键进行替换。
+- 类型：String
+- 必选：否
 
 每次请求的Filters的上限为10，Filter.Values的上限为5。
         :type Filters: list of Filter
         :param Offset: 分页的偏移量，默认值为0
         :type Offset: int
         :param Limit: 分页单页的限制数目，默认值为20，最大值100
         :type Limit: int
@@ -4122,35 +4084,17 @@
 class DescribeShippersRequest(AbstractModel):
     """DescribeShippers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: <br><li> shipperName
-
-按照【投递规则名称】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> shipperId
-
-按照【投递规则ID】进行过滤。
-类型：String
-
-必选：否
-
-<br><li> topicId
-
-按照【日志主题】进行过滤。
-
-类型：String
-
-必选：否
+        :param Filters: - shipperName：按照【投递规则名称】进行过滤。类型：String。必选：否
+- shipperId：按照【投递规则ID】进行过滤。类型：String。必选：否
+- topicId：按照【日志主题】进行过滤。类型：String。必选：否
 
 每次请求的Filters的上限为10，Filter.Values的上限为5。
         :type Filters: list of Filter
         :param Offset: 分页的偏移量，默认值为0
         :type Offset: int
         :param Limit: 分页单页的限制数目，默认值为20，最大值100
         :type Limit: int
```

### Comparing `tencentcloud-sdk-python-cls-3.0.879/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.880/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.879/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.880/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.880/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.879/setup.py` & `tencentcloud-sdk-python-cls-3.0.880/setup.py`

 * *Files identical despite different names*

