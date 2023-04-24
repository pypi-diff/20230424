# Comparing `tmp/antchain_appex-1.3.3.tar.gz` & `tmp/antchain_appex-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_appex-1.3.3.tar", last modified: Tue Jul 19 02:26:34 2022, max compression
+gzip compressed data, was "dist/antchain_appex-1.3.8.tar", last modified: Fri Sep 23 03:33:54 2022, max compression
```

## Comparing `antchain_appex-1.3.3.tar` & `antchain_appex-1.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/
--rw-r--r--   0 root         (0) root         (0)      600 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2174 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      810 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      996 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_appex.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2174 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_appex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      339 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_appex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_appex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_appex.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_appex.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_sdk_appex/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_sdk_appex/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100250 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_sdk_appex/client.py
--rw-r--r--   0 root         (0) root         (0)   184136 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/antchain_sdk_appex/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2498 2022-07-19 02:26:34.000000 antchain_appex-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/
+-rw-r--r--   0 root         (0) root         (0)      600 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2174 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      810 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      996 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_appex.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2174 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_appex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      339 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_appex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_appex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_appex.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_appex.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_sdk_appex/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_sdk_appex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   102732 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_sdk_appex/client.py
+-rw-r--r--   0 root         (0) root         (0)   188254 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/antchain_sdk_appex/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2498 2022-09-23 03:33:54.000000 antchain_appex-1.3.8/setup.py
```

### Comparing `antchain_appex-1.3.3/LICENSE` & `antchain_appex-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_appex-1.3.3/PKG-INFO` & `antchain_appex-1.3.8/antchain_appex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_appex
-Version: 1.3.3
+Name: antchain-appex
+Version: 1.3.8
 Summary: Ant Chain APPEX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_appex-1.3.3/README-CN.md` & `antchain_appex-1.3.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_appex-1.3.3/README.md` & `antchain_appex-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `antchain_appex-1.3.3/antchain_appex.egg-info/PKG-INFO` & `antchain_appex-1.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-appex
-Version: 1.3.3
+Name: antchain_appex
+Version: 1.3.8
 Summary: Ant Chain APPEX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_appex-1.3.3/antchain_sdk_appex/client.py` & `antchain_appex-1.3.8/antchain_sdk_appex/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.3'
+                    'sdk_version': '1.3.8',
+                    '_prod_code': 'APPEX',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -233,15 +235,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.3'
+                    'sdk_version': '1.3.8',
+                    '_prod_code': 'APPEX',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -379,70 +383,14 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             appex_models.QueryMypocketChainaccountResponse(),
             await self.do_request_async('1.0', 'blockchain.appex.mypocket.chainaccount.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_mypocket_kmsaccount(
-        self,
-        request: appex_models.BindMypocketKmsaccountRequest,
-    ) -> appex_models.BindMypocketKmsaccountResponse:
-        """
-        Description: 外部DApp应用绑定链账户至did
-        Summary: 外部DApp应用绑定链账户至did
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.bind_mypocket_kmsaccount_ex(request, headers, runtime)
-
-    async def bind_mypocket_kmsaccount_async(
-        self,
-        request: appex_models.BindMypocketKmsaccountRequest,
-    ) -> appex_models.BindMypocketKmsaccountResponse:
-        """
-        Description: 外部DApp应用绑定链账户至did
-        Summary: 外部DApp应用绑定链账户至did
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.bind_mypocket_kmsaccount_ex_async(request, headers, runtime)
-
-    def bind_mypocket_kmsaccount_ex(
-        self,
-        request: appex_models.BindMypocketKmsaccountRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> appex_models.BindMypocketKmsaccountResponse:
-        """
-        Description: 外部DApp应用绑定链账户至did
-        Summary: 外部DApp应用绑定链账户至did
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            appex_models.BindMypocketKmsaccountResponse(),
-            self.do_request('1.0', 'blockchain.appex.mypocket.kmsaccount.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def bind_mypocket_kmsaccount_ex_async(
-        self,
-        request: appex_models.BindMypocketKmsaccountRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> appex_models.BindMypocketKmsaccountResponse:
-        """
-        Description: 外部DApp应用绑定链账户至did
-        Summary: 外部DApp应用绑定链账户至did
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            appex_models.BindMypocketKmsaccountResponse(),
-            await self.do_request_async('1.0', 'blockchain.appex.mypocket.kmsaccount.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def create_mypocket_didaccountbyalipay(
         self,
         request: appex_models.CreateMypocketDidaccountbyalipayRequest,
     ) -> appex_models.CreateMypocketDidaccountbyalipayResponse:
         """
         Description: 外部DApp应用通过支付宝UID创建普通用户did账户
         Summary: 创建普通用户DID账户（支付宝UID）
@@ -659,14 +607,126 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             appex_models.QueryMypocketEscrowchainaccountResponse(),
             await self.do_request_async('1.0', 'blockchain.appex.mypocket.escrowchainaccount.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def start_mypocket_appdidsignverify(
+        self,
+        request: appex_models.StartMypocketAppdidsignverifyRequest,
+    ) -> appex_models.StartMypocketAppdidsignverifyResponse:
+        """
+        Description: 验证app did签名
+        Summary: app did验签接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.start_mypocket_appdidsignverify_ex(request, headers, runtime)
+
+    async def start_mypocket_appdidsignverify_async(
+        self,
+        request: appex_models.StartMypocketAppdidsignverifyRequest,
+    ) -> appex_models.StartMypocketAppdidsignverifyResponse:
+        """
+        Description: 验证app did签名
+        Summary: app did验签接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.start_mypocket_appdidsignverify_ex_async(request, headers, runtime)
+
+    def start_mypocket_appdidsignverify_ex(
+        self,
+        request: appex_models.StartMypocketAppdidsignverifyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> appex_models.StartMypocketAppdidsignverifyResponse:
+        """
+        Description: 验证app did签名
+        Summary: app did验签接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            appex_models.StartMypocketAppdidsignverifyResponse(),
+            self.do_request('1.0', 'blockchain.appex.mypocket.appdidsignverify.start', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def start_mypocket_appdidsignverify_ex_async(
+        self,
+        request: appex_models.StartMypocketAppdidsignverifyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> appex_models.StartMypocketAppdidsignverifyResponse:
+        """
+        Description: 验证app did签名
+        Summary: app did验签接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            appex_models.StartMypocketAppdidsignverifyResponse(),
+            await self.do_request_async('1.0', 'blockchain.appex.mypocket.appdidsignverify.start', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def start_mypocket_userdidsignverify(
+        self,
+        request: appex_models.StartMypocketUserdidsignverifyRequest,
+    ) -> appex_models.StartMypocketUserdidsignverifyResponse:
+        """
+        Description: 验证user did签名
+        Summary: 验证user did签名
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.start_mypocket_userdidsignverify_ex(request, headers, runtime)
+
+    async def start_mypocket_userdidsignverify_async(
+        self,
+        request: appex_models.StartMypocketUserdidsignverifyRequest,
+    ) -> appex_models.StartMypocketUserdidsignverifyResponse:
+        """
+        Description: 验证user did签名
+        Summary: 验证user did签名
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.start_mypocket_userdidsignverify_ex_async(request, headers, runtime)
+
+    def start_mypocket_userdidsignverify_ex(
+        self,
+        request: appex_models.StartMypocketUserdidsignverifyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> appex_models.StartMypocketUserdidsignverifyResponse:
+        """
+        Description: 验证user did签名
+        Summary: 验证user did签名
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            appex_models.StartMypocketUserdidsignverifyResponse(),
+            self.do_request('1.0', 'blockchain.appex.mypocket.userdidsignverify.start', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def start_mypocket_userdidsignverify_ex_async(
+        self,
+        request: appex_models.StartMypocketUserdidsignverifyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> appex_models.StartMypocketUserdidsignverifyResponse:
+        """
+        Description: 验证user did签名
+        Summary: 验证user did签名
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            appex_models.StartMypocketUserdidsignverifyResponse(),
+            await self.do_request_async('1.0', 'blockchain.appex.mypocket.userdidsignverify.start', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_user_did(
         self,
         request: appex_models.CreateUserDidRequest,
     ) -> appex_models.CreateUserDidResponse:
         """
         Description: 区块链身份创建
         Summary: 区块链身份创建
```

### Comparing `antchain_appex-1.3.3/antchain_sdk_appex/models.py` & `antchain_appex-1.3.8/antchain_sdk_appex/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -881,92 +881,71 @@
         if m.get('chain_accounts') is not None:
             for k in m.get('chain_accounts'):
                 temp_model = AccountEntry()
                 self.chain_accounts.append(temp_model.from_map(k))
         return self
 
 
-class BindMypocketKmsaccountRequest(TeaModel):
+class CreateMypocketDidaccountbyalipayRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        did: str = None,
-        chain_id: str = None,
-        chain_account: str = None,
-        kms_id: str = None,
+        alipay_uid: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 用户的DID
-        self.did = did
-        # 区块链ID
-        self.chain_id = chain_id
-        # 用户的链上账户
-        self.chain_account = chain_account
-        # 该链账户在BaaS服务的KMS ID
-        self.kms_id = kms_id
+        # 支付宝Uid
+        self.alipay_uid = alipay_uid
 
     def validate(self):
-        self.validate_required(self.did, 'did')
-        self.validate_required(self.chain_id, 'chain_id')
-        self.validate_required(self.chain_account, 'chain_account')
-        self.validate_required(self.kms_id, 'kms_id')
+        self.validate_required(self.alipay_uid, 'alipay_uid')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.did is not None:
-            result['did'] = self.did
-        if self.chain_id is not None:
-            result['chain_id'] = self.chain_id
-        if self.chain_account is not None:
-            result['chain_account'] = self.chain_account
-        if self.kms_id is not None:
-            result['kms_id'] = self.kms_id
+        if self.alipay_uid is not None:
+            result['alipay_uid'] = self.alipay_uid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('did') is not None:
-            self.did = m.get('did')
-        if m.get('chain_id') is not None:
-            self.chain_id = m.get('chain_id')
-        if m.get('chain_account') is not None:
-            self.chain_account = m.get('chain_account')
-        if m.get('kms_id') is not None:
-            self.kms_id = m.get('kms_id')
+        if m.get('alipay_uid') is not None:
+            self.alipay_uid = m.get('alipay_uid')
         return self
 
 
-class BindMypocketKmsaccountResponse(TeaModel):
+class CreateMypocketDidaccountbyalipayResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        did: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 用户的DID
+        self.did = did
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -975,28 +954,32 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.did is not None:
+            result['did'] = self.did
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('did') is not None:
+            self.did = m.get('did')
         return self
 
 
-class CreateMypocketDidaccountbyalipayRequest(TeaModel):
+class QueryMypocketDidaccountbyalipayRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         alipay_uid: str = None,
     ):
         # OAuth模式下的授权token
@@ -1029,29 +1012,29 @@
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('alipay_uid') is not None:
             self.alipay_uid = m.get('alipay_uid')
         return self
 
 
-class CreateMypocketDidaccountbyalipayResponse(TeaModel):
+class QueryMypocketDidaccountbyalipayResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         did: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 用户的DID
+        # 外部DApp应用通过支付宝UID查询普通用户did
         self.did = did
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1078,71 +1061,82 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('did') is not None:
             self.did = m.get('did')
         return self
 
 
-class QueryMypocketDidaccountbyalipayRequest(TeaModel):
+class CreateMypocketEscrowchainaccountRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        alipay_uid: str = None,
+        did: str = None,
+        chain_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 支付宝Uid
-        self.alipay_uid = alipay_uid
+        # 用户did
+        self.did = did
+        # 链id
+        self.chain_id = chain_id
 
     def validate(self):
-        self.validate_required(self.alipay_uid, 'alipay_uid')
+        self.validate_required(self.did, 'did')
+        self.validate_required(self.chain_id, 'chain_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.alipay_uid is not None:
-            result['alipay_uid'] = self.alipay_uid
+        if self.did is not None:
+            result['did'] = self.did
+        if self.chain_id is not None:
+            result['chain_id'] = self.chain_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('alipay_uid') is not None:
-            self.alipay_uid = m.get('alipay_uid')
+        if m.get('did') is not None:
+            self.did = m.get('did')
+        if m.get('chain_id') is not None:
+            self.chain_id = m.get('chain_id')
         return self
 
 
-class QueryMypocketDidaccountbyalipayResponse(TeaModel):
+class CreateMypocketEscrowchainaccountResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        did: str = None,
+        account_name: str = None,
+        account_id: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 外部DApp应用通过支付宝UID查询普通用户did
-        self.did = did
+        # 账户名称
+        self.account_name = account_name
+        # 链上id
+        self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1151,32 +1145,36 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.did is not None:
-            result['did'] = self.did
+        if self.account_name is not None:
+            result['account_name'] = self.account_name
+        if self.account_id is not None:
+            result['account_id'] = self.account_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('did') is not None:
-            self.did = m.get('did')
+        if m.get('account_name') is not None:
+            self.account_name = m.get('account_name')
+        if m.get('account_id') is not None:
+            self.account_id = m.get('account_id')
         return self
 
 
-class CreateMypocketEscrowchainaccountRequest(TeaModel):
+class QueryMypocketEscrowchainaccountRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         did: str = None,
         chain_id: str = None,
     ):
@@ -1217,33 +1215,152 @@
         if m.get('did') is not None:
             self.did = m.get('did')
         if m.get('chain_id') is not None:
             self.chain_id = m.get('chain_id')
         return self
 
 
-class CreateMypocketEscrowchainaccountResponse(TeaModel):
+class QueryMypocketEscrowchainaccountResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        account_name: str = None,
-        account_id: str = None,
+        chain_accounts: List[AccountEntry] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 账户名称
-        self.account_name = account_name
-        # 链上id
-        self.account_id = account_id
+        # DID对应的所有链上账户
+        self.chain_accounts = chain_accounts
+
+    def validate(self):
+        if self.chain_accounts:
+            for k in self.chain_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['chain_accounts'] = []
+        if self.chain_accounts is not None:
+            for k in self.chain_accounts:
+                result['chain_accounts'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.chain_accounts = []
+        if m.get('chain_accounts') is not None:
+            for k in m.get('chain_accounts'):
+                temp_model = AccountEntry()
+                self.chain_accounts.append(temp_model.from_map(k))
+        return self
+
+
+class StartMypocketAppdidsignverifyRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        did_sign: str = None,
+        payload: str = None,
+        dapp_id: str = None,
+        timestamp: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 签名
+        self.did_sign = did_sign
+        # 签名原文
+        self.payload = payload
+        # 分配的dapp id，uuid v4格式
+        self.dapp_id = dapp_id
+        # epoch时间，毫秒
+        self.timestamp = timestamp
+
+    def validate(self):
+        self.validate_required(self.did_sign, 'did_sign')
+        self.validate_required(self.payload, 'payload')
+        self.validate_required(self.dapp_id, 'dapp_id')
+        self.validate_required(self.timestamp, 'timestamp')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.did_sign is not None:
+            result['did_sign'] = self.did_sign
+        if self.payload is not None:
+            result['payload'] = self.payload
+        if self.dapp_id is not None:
+            result['dapp_id'] = self.dapp_id
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('did_sign') is not None:
+            self.did_sign = m.get('did_sign')
+        if m.get('payload') is not None:
+            self.payload = m.get('payload')
+        if m.get('dapp_id') is not None:
+            self.dapp_id = m.get('dapp_id')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        return self
+
+
+class StartMypocketAppdidsignverifyResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        is_valid: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 签名是否合法
+        self.is_valid = is_valid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1252,138 +1369,143 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.account_name is not None:
-            result['account_name'] = self.account_name
-        if self.account_id is not None:
-            result['account_id'] = self.account_id
+        if self.is_valid is not None:
+            result['is_valid'] = self.is_valid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('account_name') is not None:
-            self.account_name = m.get('account_name')
-        if m.get('account_id') is not None:
-            self.account_id = m.get('account_id')
+        if m.get('is_valid') is not None:
+            self.is_valid = m.get('is_valid')
         return self
 
 
-class QueryMypocketEscrowchainaccountRequest(TeaModel):
+class StartMypocketUserdidsignverifyRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        did: str = None,
-        chain_id: str = None,
+        did_sign: str = None,
+        payload: str = None,
+        user_did: str = None,
+        timestamp: int = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 用户did
-        self.did = did
-        # 链id
-        self.chain_id = chain_id
+        # 签名
+        self.did_sign = did_sign
+        # 签名原文
+        self.payload = payload
+        # mychain did信息
+        self.user_did = user_did
+        # epoch时间，毫秒
+        self.timestamp = timestamp
 
     def validate(self):
-        self.validate_required(self.did, 'did')
-        self.validate_required(self.chain_id, 'chain_id')
+        self.validate_required(self.did_sign, 'did_sign')
+        self.validate_required(self.payload, 'payload')
+        self.validate_required(self.user_did, 'user_did')
+        self.validate_required(self.timestamp, 'timestamp')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.did is not None:
-            result['did'] = self.did
-        if self.chain_id is not None:
-            result['chain_id'] = self.chain_id
+        if self.did_sign is not None:
+            result['did_sign'] = self.did_sign
+        if self.payload is not None:
+            result['payload'] = self.payload
+        if self.user_did is not None:
+            result['user_did'] = self.user_did
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('did') is not None:
-            self.did = m.get('did')
-        if m.get('chain_id') is not None:
-            self.chain_id = m.get('chain_id')
+        if m.get('did_sign') is not None:
+            self.did_sign = m.get('did_sign')
+        if m.get('payload') is not None:
+            self.payload = m.get('payload')
+        if m.get('user_did') is not None:
+            self.user_did = m.get('user_did')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
         return self
 
 
-class QueryMypocketEscrowchainaccountResponse(TeaModel):
+class StartMypocketUserdidsignverifyResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        chain_accounts: List[AccountEntry] = None,
+        is_valid: bool = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # DID对应的所有链上账户
-        self.chain_accounts = chain_accounts
+        # 
+        # 签名是否合法
+        self.is_valid = is_valid
 
     def validate(self):
-        if self.chain_accounts:
-            for k in self.chain_accounts:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        result['chain_accounts'] = []
-        if self.chain_accounts is not None:
-            for k in self.chain_accounts:
-                result['chain_accounts'].append(k.to_map() if k else None)
+        if self.is_valid is not None:
+            result['is_valid'] = self.is_valid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        self.chain_accounts = []
-        if m.get('chain_accounts') is not None:
-            for k in m.get('chain_accounts'):
-                temp_model = AccountEntry()
-                self.chain_accounts.append(temp_model.from_map(k))
+        if m.get('is_valid') is not None:
+            self.is_valid = m.get('is_valid')
         return self
 
 
 class CreateUserDidRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_appex-1.3.3/setup.py` & `antchain_appex-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_appex.
 
-Created on 19/07/2022
+Created on 23/09/2022
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_appex"
 NAME = "antchain_appex" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain APPEX SDK Library for Python"
```

