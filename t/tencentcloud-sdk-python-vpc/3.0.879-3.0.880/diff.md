# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.879.tar", last modified: Fri Apr 21 01:09:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.880.tar", last modified: Mon Apr 24 03:49:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.879.tar` & `tencentcloud-sdk-python-vpc-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   327723 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    40141 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   834744 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   327723 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    40141 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   836460 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:49:16.000000 tencentcloud-sdk-python-vpc-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.880/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/README.rst` & `tencentcloud-sdk-python-vpc-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2328,14 +2328,43 @@
 
 
 class CcnRegionBandwidthLimitInfo(AbstractModel):
     """云联网（CCN）地域出带宽上限。
 
     """
 
+    def __init__(self):
+        r"""
+        :param SourceRegion: 源地域，例如：ap-shanghai
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SourceRegion: str
+        :param DestinationRegion: 目的地域， 例如：ap-shanghai
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DestinationRegion: str
+        :param BandwidthLimit: 出带宽上限，单位：Mbps。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BandwidthLimit: int
+        """
+        self.SourceRegion = None
+        self.DestinationRegion = None
+        self.BandwidthLimit = None
+
+
+    def _deserialize(self, params):
+        self.SourceRegion = params.get("SourceRegion")
+        self.DestinationRegion = params.get("DestinationRegion")
+        self.BandwidthLimit = params.get("BandwidthLimit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
 
 class CcnRoute(AbstractModel):
     """CCN路由策略对象
 
     """
 
     def __init__(self):
@@ -5231,15 +5260,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param VpnGatewayId: VPN网关实例ID。
         :type VpnGatewayId: str
-        :param CustomerGatewayId: 对端网关ID，例如：cgw-2wqq41m9，可通过DescribeCustomerGateways接口查询对端网关。
+        :param CustomerGatewayId: 对端网关ID。例如：cgw-2wqq41m9，可通过[DescribeCustomerGateways](https://cloud.tencent.com/document/product/215/17516)接口查询对端网关。
         :type CustomerGatewayId: str
         :param VpnConnectionName: 通道名称，可任意命名，但不得超过60个字符。
         :type VpnConnectionName: str
         :param PreShareKey: 预共享密钥。
         :type PreShareKey: str
         :param VpcId: VPC实例ID。可通过[DescribeVpcs](https://cloud.tencent.com/document/product/215/15778)接口返回值中的VpcId获取。
 CCN VPN 形的通道 可以不传VPCID
@@ -5248,19 +5277,19 @@
         :type SecurityPolicyDatabases: list of SecurityPolicyDatabase
         :param IKEOptionsSpecification: IKE配置（Internet Key Exchange，因特网密钥交换），IKE具有一套自我保护机制，用户配置网络安全协议
         :type IKEOptionsSpecification: :class:`tencentcloud.vpc.v20170312.models.IKEOptionsSpecification`
         :param IPSECOptionsSpecification: IPSec配置，腾讯云提供IPSec安全会话设置
         :type IPSECOptionsSpecification: :class:`tencentcloud.vpc.v20170312.models.IPSECOptionsSpecification`
         :param Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]
         :type Tags: list of Tag
-        :param EnableHealthCheck: 是否支持隧道内健康检查
+        :param EnableHealthCheck: 是否支持隧道内健康检查，默认为False。
         :type EnableHealthCheck: bool
-        :param HealthCheckLocalIp: 健康检查本端地址
+        :param HealthCheckLocalIp: 健康检查本端地址，默认值为随机在169.254.128.0/17分配一个IP。
         :type HealthCheckLocalIp: str
-        :param HealthCheckRemoteIp: 健康检查对端地址
+        :param HealthCheckRemoteIp: 健康检查对端地址，默认值为随机在169.254.128.0/17分配一个IP。
         :type HealthCheckRemoteIp: str
         :param RouteType: 通道类型, 例如:["STATIC", "StaticRoute", "Policy"]
         :type RouteType: str
         :param NegotiationType: 协商类型，默认为active（主动协商）。可选值：active（主动协商），passive（被动协商），flowTrigger（流量协商）
         :type NegotiationType: str
         :param DpdEnable: DPD探测开关。默认为0，表示关闭DPD探测。可选值：0（关闭），1（开启）
         :type DpdEnable: int
@@ -6179,15 +6208,15 @@
 class DeleteCustomerGatewayRequest(AbstractModel):
     """DeleteCustomerGateway请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param CustomerGatewayId: 对端网关ID，例如：cgw-2wqq41m9，可通过DescribeCustomerGateways接口查询对端网关。
+        :param CustomerGatewayId: 对端网关ID，例如：cgw-2wqq41m9，可通过[DescribeCustomerGateways](https://cloud.tencent.com/document/api/215/17516)接口查询对端网关。
         :type CustomerGatewayId: str
         """
         self.CustomerGatewayId = None
 
 
     def _deserialize(self, params):
         self.CustomerGatewayId = params.get("CustomerGatewayId")
@@ -16720,15 +16749,15 @@
 class ModifyCustomerGatewayAttributeRequest(AbstractModel):
     """ModifyCustomerGatewayAttribute请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param CustomerGatewayId: 对端网关ID，例如：cgw-2wqq41m9，可通过DescribeCustomerGateways接口查询对端网关。
+        :param CustomerGatewayId: 对端网关ID，例如：cgw-2wqq41m9，可通过[DescribeCustomerGateways](https://cloud.tencent.com/document/api/215/17516)接口查询对端网关。
         :type CustomerGatewayId: str
         :param CustomerGatewayName: 对端网关名称，可任意命名，但不得超过60个字符。
         :type CustomerGatewayName: str
         """
         self.CustomerGatewayId = None
         self.CustomerGatewayName = None
 
@@ -18428,48 +18457,51 @@
         r"""
         :param VpnConnectionId: VPN通道实例ID。形如：vpnx-f49l6u0z。
         :type VpnConnectionId: str
         :param VpnConnectionName: VPN通道名称，可任意命名，但不得超过60个字符。
         :type VpnConnectionName: str
         :param PreShareKey: 预共享密钥。
         :type PreShareKey: str
-        :param SecurityPolicyDatabases: SPD策略组，例如：{"10.0.0.5/24":["172.123.10.5/16"]}，10.0.0.5/24是vpc内网段172.123.10.5/16是IDC网段。用户指定VPC内哪些网段可以和您IDC中哪些网段通信。
+        :param SecurityPolicyDatabases: SPD策略组，例如：{"10.0.0.5/24":["172.123.10.5/16"]}，10.0.0.5/24是vpc内网段，172.123.10.5/16是IDC网段。用户指定VPC内哪些网段可以和您IDC中哪些网段通信。
         :type SecurityPolicyDatabases: list of SecurityPolicyDatabase
         :param IKEOptionsSpecification: IKE配置（Internet Key Exchange，因特网密钥交换），IKE具有一套自我保护机制，用户配置网络安全协议。
         :type IKEOptionsSpecification: :class:`tencentcloud.vpc.v20170312.models.IKEOptionsSpecification`
         :param IPSECOptionsSpecification: IPSec配置，腾讯云提供IPSec安全会话设置。
         :type IPSECOptionsSpecification: :class:`tencentcloud.vpc.v20170312.models.IPSECOptionsSpecification`
-        :param EnableHealthCheck: 是否启用通道健康检查
+        :param EnableHealthCheck: 是否启用通道健康检查，默认为False。
         :type EnableHealthCheck: bool
-        :param HealthCheckLocalIp: 本端通道探测ip
+        :param HealthCheckLocalIp: 本端通道探测IP。
         :type HealthCheckLocalIp: str
-        :param HealthCheckRemoteIp: 对端通道探测ip
+        :param HealthCheckRemoteIp: 对端通道探测IP。
         :type HealthCheckRemoteIp: str
         :param NegotiationType: 协商类型，默认为active（主动协商）。可选值：active（主动协商），passive（被动协商），flowTrigger（流量协商）
         :type NegotiationType: str
         :param DpdEnable: DPD探测开关。默认为0，表示关闭DPD探测。可选值：0（关闭），1（开启）
         :type DpdEnable: int
         :param DpdTimeout: DPD超时时间。即探测确认对端不存在需要的时间。dpdEnable为1（开启）时有效。默认30，单位为秒
         :type DpdTimeout: str
         :param DpdAction: DPD超时后的动作。默认为clear。dpdEnable为1（开启）时有效。可取值为clear（断开）和restart（重试）
         :type DpdAction: str
+        :param CustomerGatewayId: 对端网关ID，4.0及以上网关下的通道支持更新。
+        :type CustomerGatewayId: str
         """
         self.VpnConnectionId = None
         self.VpnConnectionName = None
         self.PreShareKey = None
         self.SecurityPolicyDatabases = None
         self.IKEOptionsSpecification = None
         self.IPSECOptionsSpecification = None
         self.EnableHealthCheck = None
         self.HealthCheckLocalIp = None
         self.HealthCheckRemoteIp = None
         self.NegotiationType = None
         self.DpdEnable = None
         self.DpdTimeout = None
         self.DpdAction = None
+        self.CustomerGatewayId = None
 
 
     def _deserialize(self, params):
         self.VpnConnectionId = params.get("VpnConnectionId")
         self.VpnConnectionName = params.get("VpnConnectionName")
         self.PreShareKey = params.get("PreShareKey")
         if params.get("SecurityPolicyDatabases") is not None:
@@ -18487,14 +18519,15 @@
         self.EnableHealthCheck = params.get("EnableHealthCheck")
         self.HealthCheckLocalIp = params.get("HealthCheckLocalIp")
         self.HealthCheckRemoteIp = params.get("HealthCheckRemoteIp")
         self.NegotiationType = params.get("NegotiationType")
         self.DpdEnable = params.get("DpdEnable")
         self.DpdTimeout = params.get("DpdTimeout")
         self.DpdAction = params.get("DpdAction")
+        self.CustomerGatewayId = params.get("CustomerGatewayId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.880/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.879/setup.py` & `tencentcloud-sdk-python-vpc-3.0.880/setup.py`

 * *Files identical despite different names*

