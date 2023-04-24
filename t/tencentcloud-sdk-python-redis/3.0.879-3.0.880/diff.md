# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.879.tar", last modified: Fri Apr 21 00:58:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.880.tar", last modified: Mon Apr 24 03:24:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.879.tar` & `tencentcloud-sdk-python-redis-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    86582 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   290895 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:58:10.000000 tencentcloud-sdk-python-redis-3.0.879/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    86631 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   291083 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-24 03:24:53.000000 tencentcloud-sdk-python-redis-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:24:54.000000 tencentcloud-sdk-python-redis-3.0.880/tencentcloud_sdk_python_redis.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-redis-3.0.879/README.rst` & `tencentcloud-sdk-python-redis-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1564,15 +1564,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyAutoBackupConfig(self, request):
-        """设置自动备份配置
+        """本接口（ModifyAutoBackupConfig）用于设置自动备份的配置。
 
         :param request: Request instance for ModifyAutoBackupConfig.
         :type request: :class:`tencentcloud.redis.v20180412.models.ModifyAutoBackupConfigRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.ModifyAutoBackupConfigResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.879/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.880/tencentcloud/redis/v20180412/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5828,21 +5828,22 @@
 class ModifyAutoBackupConfigRequest(AbstractModel):
     """ModifyAutoBackupConfig请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID。
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****。请登录[Redis控制台](https://console.cloud.tencent.com/redis)在实例列表复制实例 ID。
+
         :type InstanceId: str
         :param WeekDays: 设置自动备份周期。可设置为Monday，Tuesday，Wednesday，Thursday，Friday，Saturday，Sunday。该参数暂不支持修改。
         :type WeekDays: list of str
         :param TimePeriod: 备份时间段。可设置为每个整点。格式如：00:00-01:00, 01:00-02:00...... 23:00-00:00。
         :type TimePeriod: str
-        :param AutoBackupType: 自动备份类型： 1 “定时回档”。
+        :param AutoBackupType: 自动备份类型。目前仅能配置为：1 ，指定时备份。
         :type AutoBackupType: int
         """
         self.InstanceId = None
         self.WeekDays = None
         self.TimePeriod = None
         self.AutoBackupType = None
 
@@ -5864,19 +5865,19 @@
 class ModifyAutoBackupConfigResponse(AbstractModel):
     """ModifyAutoBackupConfig返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AutoBackupType: 自动备份类型： 1 “定时回档”
+        :param AutoBackupType: 自动备份类型。目前仅能配置为：1 ，指定时备份。
         :type AutoBackupType: int
         :param WeekDays: 自动备份周期。取值为：Monday，Tuesday，Wednesday，Thursday，Friday，Saturday，Sunday。
         :type WeekDays: list of str
-        :param TimePeriod: 自动备份时间段。格式如：00:00-01:00, 01:00-02:00...... 23:00-00:00。
+        :param TimePeriod: 自动定时备份时间段。格式如：00:00-01:00, 01:00-02:00...... 23:00-00:00。
         :type TimePeriod: str
         :param BackupStorageDays: 全量备份文件保存天数,单位：天。
         :type BackupStorageDays: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.AutoBackupType = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.880/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.879/setup.py` & `tencentcloud-sdk-python-redis-3.0.880/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.879/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.880/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

