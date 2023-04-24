# Comparing `tmp/inhandtest-0.0.35.tar.gz` & `tmp/inhandtest-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.35.tar", last modified: Tue Apr 18 07:47:11 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.36.tar", last modified: Mon Apr 24 03:19:28 2023, max compression
```

## Comparing `inhandtest-0.0.35.tar` & `inhandtest-0.0.36.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:47:11.000000 inhandtest-0.0.35/
--rw-rw-rw-   0        0        0      535 2023-04-18 07:47:11.000000 inhandtest-0.0.35/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.35/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 07:47:11.000000 inhandtest-0.0.35/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.35/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:47:11.000000 inhandtest-0.0.35/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.35/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.35/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.35/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.35/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.35/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.35/inhandtest/file.py
--rw-rw-rw-   0        0        0    11858 2023-04-04 07:39:23.000000 inhandtest-0.0.35/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.35/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    38857 2023-03-31 08:19:19.000000 inhandtest-0.0.35/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.35/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.35/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.35/inhandtest/ip.py
--rw-rw-rw-   0        0        0     3628 2023-04-18 01:11:21.000000 inhandtest-0.0.35/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1222 2023-04-18 01:10:09.000000 inhandtest-0.0.35/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32231 2023-04-17 06:31:22.000000 inhandtest-0.0.35/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    22481 2023-04-17 01:30:47.000000 inhandtest-0.0.35/inhandtest/tools.py
--rw-rw-rw-   0        0        0       98 2023-04-18 02:40:30.000000 inhandtest-0.0.35/requirements.txt
--rw-rw-rw-   0        0        0     1407 2023-04-18 07:46:10.000000 inhandtest-0.0.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:19:28.000000 inhandtest-0.0.36/
+-rw-rw-rw-   0        0        0      535 2023-04-24 03:19:28.000000 inhandtest-0.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.36/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 03:19:28.000000 inhandtest-0.0.36/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.36/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:19:28.000000 inhandtest-0.0.36/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.36/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.36/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.36/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.36/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.36/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.36/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11858 2023-04-04 07:39:23.000000 inhandtest-0.0.36/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     2605 2023-04-23 10:26:25.000000 inhandtest-0.0.36/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.36/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    45323 2023-04-23 10:35:33.000000 inhandtest-0.0.36/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.36/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.36/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.36/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     3628 2023-04-23 10:47:45.000000 inhandtest-0.0.36/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1222 2023-04-18 01:10:09.000000 inhandtest-0.0.36/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.36/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    22700 2023-04-24 03:15:39.000000 inhandtest-0.0.36/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      115 2023-04-24 03:15:39.000000 inhandtest-0.0.36/requirements.txt
+-rw-rw-rw-   0        0        0     1419 2023-04-24 03:18:46.000000 inhandtest-0.0.36/setup.py
```

### Comparing `inhandtest-0.0.35/PKG-INFO` & `inhandtest-0.0.36/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inhandtest
-Version: 0.0.35
+Version: 0.0.36
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 License: UNKNOWN
 Description: 方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；
         映翰通出品，追尾必究！
```

### Comparing `inhandtest-0.0.35/README.md` & `inhandtest-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.36/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/base_page/base_page.py` & `inhandtest-0.0.36/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.36/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/exception.py` & `inhandtest-0.0.36/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/file.py` & `inhandtest-0.0.36/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/inmodbus.py` & `inhandtest-0.0.36/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/inmqtt.py` & `inhandtest-0.0.36/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/inrequest.py` & `inhandtest-0.0.36/inhandtest/inrequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 import base64
 import logging
 import os
 import re
 import sys
 import time
 from typing import List
-
 import urllib3
 import requests
 from inhandtest.exception import ParameterValueError, UsernameOrPasswordError, TimeOutError, UpgradeFailedError, \
     ResourceNotFoundError
 from inhandtest.file import file_hash
-from inhandtest.tools import dict_in, dict_merge, replace_str
+from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict
 
 
 class DmInterface:
 
     def __init__(self, username, password, host='iot.inhand.com.cn'):
         """
         :param username  平台用户名
         :param password  平台密码
         :param host: 'iot.inhand.com.cn'|'iot.inhandnetworks.com' 平台是哪个环境,
         """
         self.host = host
         self.username = username
-        type_ = 'iot' if 'iot' in self.host else 'ics'
+        type_ = 'iot' if ('iot' in self.host) or ('elms' in self.host) else 'ics'
         self.api = InRequest(self.host, username, password, type_)
 
     def device_exist(self, sn: str, timeout=120, interval=5) -> None:
         """检查设备在平台账号下存在，如果超时都不存在就抛异常
 
         :param sn:
         :param timeout:
@@ -81,15 +80,15 @@
                     {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('info').get('iccid'),
                      'imei': res.get('info').get('imei'), 'imsi': res.get('info').get('imsi'),
                      'version': res.get('info').get('swVersion'), 'hwVersion': res.get('info').get('hwVersion'),
                      'bootVersion': res.get('info').get('bootVersion'), 'address': res.get('address'),
                      'id': res.get('_id'), 'name': res.get('name')})
             else:
                 result.append(
-                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'swVersion': None,
+                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
                      'hwVersion': None, 'bootVersion': None, 'address': None, 'id': None, 'name': None})
         return result
 
     def add_device(self, sn: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
@@ -504,15 +503,15 @@
                     {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('metadata').get('iccid'),
                      'imei': res.get('metadata').get('imei'), 'imsi': res.get('metadata').get('imsi'),
                      'version': res.get('metadata').get('swVersion'), 'hwVersion': res.get('metadata').get('hwVersion'),
                      'bootVersion': res.get('metadata').get('bootVersion'),
                      'id': res.get('id'), 'connected': res.get('connected'), 'name': res.get('name')})
             else:
                 result.append(
-                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'swVersion': None,
+                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
                      'hwVersion': None, 'bootVersion': None, 'id': None, 'connected': None, 'name': None})
         return result
 
     def send_openvpn_config(self, sn: str) -> None:
         """每次把设备添加到平台上线后，openvpn要连半天，可以主动推送下配置让openvpn连接的更快，
            如果设备已经连接上了openvpn就不在下发了
 
@@ -539,14 +538,146 @@
         device = list(filter(lambda x: x.get('id'), self.device_state(sn)))
         if device:
             for device_ in device:
                 self.api.send_request(f'api/invpn/router/{device_.get("id")}', 'delete', {'oid': self.oid})
                 logging.info(f'the {device_.get("sn")} delete success')
 
 
+class StarInterface:
+
+    def __init__(self, username, password, host='star.inhandcloud.cn'):
+        """ 须确保用户关闭了多因素认证
+
+        :param username  平台用户名
+        :param password  平台密码
+        :param host: 'star.inhandcloud.cn'|'star.inhandcloud.cn'|'star.nezha.inhand.dev'|'star.nezha.inhand.design' 平台是哪个环境,
+        """
+        self.host = host
+        self.username = username
+        self.api = InRequest(self.host, username, password, 'star')
+        self.me = self.__get_me()
+
+    def __get_me(self) -> DotDict:
+        """ 获取me的各种信息 包括oid
+
+        :return:
+        """
+        response = DotDict(
+            self.api.send_request('/api/v1/users/me', method='get', param={"expand": 'org'}).json().get('result'))
+        return response
+
+    def device_state(self, sn: list) -> List[dict]:
+        """根据sn 转换属性 属性值有：  online: 在线|离线   True|False
+                                       iccid:
+                                       imei:
+                                       imsi:
+                                       version: 固件版本
+                                       licenseStatus: 'licensed'
+                                       sn: 序列号
+                                       address
+                                       id: 设备id
+                                       name: 设备名字
+        :param sn: 列表
+        :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
+        """
+        result = []
+        for sn_ in sn:
+            response = self.api.send_request('/api/v1/devices', method='get',
+                                             param={"expand": 'firmwareUpgradeStatus,compatibilities,org', "limit": 10,
+                                                    "compatibilities": 'nezha_device_config,nezha_device_webui',
+                                                    'serialNumber': sn_}).json()
+            if response.get('total') == 1:
+                res = response.get('result')[0]
+                result.append(
+                    {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('state').get('iccid'),
+                     'imei': res.get('state').get('imei'), 'imsi': res.get('state').get('imsi'),
+                     'version': res.get('firmware'), 'licenseStatus': res.get('licenseStatus'),
+                     'address': res.get('address'), 'id': res.get('_id'), 'name': res.get('name')})
+            else:
+                result.append(
+                    {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None,
+                     'version': None, 'licenseStatus': None, 'address': None, 'id': None, 'name': None})
+        return result
+
+    def add_device(self, sn: str, mac_or_imei: str) -> None:
+        """添加设备，
+
+        :param sn: 设备序列号
+        :param mac_or_imei: 添加设备时需要依赖设备的mac地址或者IMEI号，去生产库查询该设备是否是映翰通设备
+        :return:
+        """
+        while True:
+            validated_field = self.api.send_request(f'api/v1/serialnumber/{sn}/validate', method='post').json().get(
+                'result').get('validatedField')
+            if not list(filter(lambda x: x.get('id'), self.device_state([sn]))):
+                self.api.send_request('api/v1/devices', 'post',
+                                      body={"name": sn + str(int(time.time())), "serialNumber": sn, 'oid': self.me.oid,
+                                            validated_field: mac_or_imei})
+                logging.info(f"the {sn} device add success")
+            else:
+                break
+
+    def assert_device_state(self, sn: str, state: dict, timeout=120, interval=5) -> None:
+        """校验设备基本状态
+
+        :param sn: 序列号
+        :param state:   支持表达式${value} ex: {'version': "'${value}' in 'V1.1.3.r4956'"}
+                        online: 在线|离线   True|False
+                        iccid:
+                        imei:
+                        imsi:
+                        version: 固件版本
+                        licenseStatus: 'licensed'
+                        sn: 序列号
+                        address
+        :param timeout: 校验信息，最大超时时间
+        :param interval: 校验信息，校验间隔时间
+        :return: True or False
+        """
+        if state:
+            for i in range(0, timeout, interval):
+                result = self.device_state([sn])[0]
+                for key, value in state.items():
+                    if '${value}' in value:
+                        value = replace_str(value, {'${value}': result.get(key)})
+                        logging.info(f'start assert {sn} state {key} {value}')
+                        try:
+                            if not eval(value):
+                                logging.info(f'the {sn} device {key} info eval {value} is false')
+                                break
+                        except Exception as e:
+                            logging.error(e)
+                            break
+                    else:
+                        logging.info(f'start assert {sn} state {key} {value}')
+                        if result.get(key) != value:
+                            logging.info(f'the {sn} device {key} info value is {result.get(key)} not {value}')
+                            break
+                else:
+                    logging.info(f"check {sn} device all state success")
+                    break
+                logging.info(f"check {sn} device state failed, please wait for {interval}s")
+                time.sleep(interval)
+            else:
+                raise TimeOutError(f"the {sn} state {state} check failed")
+
+    def delete_device(self, sn: str or list) -> None:
+        """
+
+        :param sn: 设备序列号，一个或多个
+        :return:
+        """
+        sn = [sn] if isinstance(sn, str) else sn
+        device = list(filter(lambda x: x.get('id'), self.device_state(sn)))
+        if device:
+            for device_ in device:
+                self.api.send_request(f'api/devices/{device_.get("id")}', 'delete')
+                logging.info(f'the {device_.get("sn")} delete success')
+
+
 class InRequest:
 
     def __init__(self, host: str, username: str, password: str, type_='device', protocol='https', port=443):
         """支持设备，平台登录及操作API, 自动识别地址
 
         :param host:  主机地址，如果是平台的就填写平台server，如果是设备就填写设备的地址
         :param username:  用户名
@@ -604,15 +735,15 @@
                 'client_secret': res_setting['result']['authProvider']['clientSecret'],
                 'grant_type': 'password',
                 'scope': 'offline',
                 "username": self.username,
                 "password": self.password,
                 # "type": 'account'
             }
-            response = self.send_request('/oauth2/token', method='post', param=param, params_type='form')
+            response = self.send_request('/oauth2/token', method='post', param=param, params_type='form').json()
             self.headers = {'Authorization': 'Bearer ' + response['access_token']}
             self.protocol = protocol_re
             self.host = host_re
         elif self.type_ == 'device':
             username_password = '%s:%s' % (self.username, self.password)
             base_auth = base64.b64encode(username_password.encode()).decode()
             self.headers = {'Authorization': 'Basic %s' % base_auth}
@@ -712,16 +843,17 @@
             else:
                 raise ValueError('expect param type error！')
         return res
 
 
 if __name__ == "__main__":
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
-    testApi = IcsInterface('guofang@inhand.com.cn', '123456')
-    testApi.remote_maintenance_online('RF3052213006490', )
+    testApi = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.dev')
+    print(testApi.me.oid)
+    # testApi.remote_maintenance_online('RF3052213006490', )
     # testApi.add_device({'RF3052213006490': 'IR305'})
     # print(testApi.web_remote_online('RF3052213006490'))
     # testApi.device_exist('VG7512022009918')
     # testApi.get_config_online('VG7512022009918', 'hello\r\nword')
     # testApi.send_config_online('VG7512022009918', 'hello\nword')
     # testApi.send_openvpn_config('RF3022206089272')
     # print(testApi.remote_maintenance_online('RF3052213006490', action='delete'))
```

### Comparing `inhandtest-0.0.35/inhandtest/insocket.py` & `inhandtest-0.0.36/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/inssh.py` & `inhandtest-0.0.36/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/ip.py` & `inhandtest-0.0.36/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/mail.py` & `inhandtest-0.0.36/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/pytest_email.html` & `inhandtest-0.0.36/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.35/inhandtest/telnet.py` & `inhandtest-0.0.36/inhandtest/telnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,21 +367,22 @@
         if kwargs.get('key_replace') and 'last_read' in key_replace_type:
             result = replace_str(result, kwargs.get('key_replace'))
         if self.interface_replace and 'last_read' in interface_replace_type:  # 替换接口的关键字
             result = replace_str(result, self.interface_replace)
         return result
 
     @__auto_login
-    def assert_cli(self, cli=None, expect=None, timeout=20, interval=5, type_='super',
-                   key_replace=None, key_replace_type='last_read', interface_replace_type='cli') -> None:
+    def assert_cli(self, cli=None, expect=None, timeout=20, interval=5, type_='super', key_replace=None,
+                   key_replace_type='last_read', interface_replace_type='cli', read_until=None) -> None:
 
         """在某个模式下支持输入一条或多条命令, 且支持对执行时最后一条命令返回的结果做断言
            该方法对ping tcpdump命令 无效
 
         :param cli: str or list, 发送的命令 一条或者多条
+        :param read_until: str or list, 直至返回结果终止， 与cli相呼应，如None的情况表示输入命令后等待1s， ['/www', None]
         :param expect: str or list or dict, 一条或多条希望校验的存在的结果，如需要判断不存在时，可以使用字典{$expect: False}
                        同时校验时可以是{$expect1: True, $expect: False}, str或者list时都是判断存在
         :param timeout: 检测超时时间  秒
         :param interval: 检测间隔时间 秒
         :param type_: 'super'|'config'|'user'|'normal'|'factory'|None
         :param key_replace: 字典, 需将固定字符替换为另一字符则填写该参数, 例: {'\r\n': '', ' ': ''}等 默认去掉换行
         :param key_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在key_replace 有值时生效，默认last_read
@@ -391,26 +392,27 @@
                                  'cli_last_read'|'cli_expect'|'last_read_expect' 任意两种组合
                                  'cli_expect_last_read': 既要替换cli 也要替换最后读取到的内容还有校验的值
         :param interface_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在interface_replace 有值时生效，默认cli
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'expect': 仅替换期望校验的值
                                  'cli_last_read'|'cli_expect'|'last_read_expect' 任意两种组合
+
                                  'cli_expect_last_read': 既要替换cli 也要替换最后读取到的内容还有校验的值
         :return: None|Exception
         """
 
         if key_replace is None:
             key_replace = {'\r\n': ''}
         if cli is not None:
             for i in range(0, timeout, interval):
                 if key_replace and 'cli' in key_replace_type:
                     cli = replace_str(cli, key_replace)
                     key_replace_type = key_replace_type.replace('cli', '')
-                result = self.send_cli(cli, type_=type_, key_replace=key_replace, key_replace_type=key_replace_type,
+                result = self.send_cli(cli, read_until, type_=type_, key_replace=key_replace, key_replace_type=key_replace_type,
                                        interface_replace_type=interface_replace_type)
                 expect = str(expect) if isinstance(expect, int) else expect
                 check_ = True
                 if expect:
                     if 'expect' in key_replace_type:
                         expect = replace_str(expect, key_replace)
                     if 'expect' in interface_replace_type:
```

### Comparing `inhandtest-0.0.35/inhandtest/tools.py` & `inhandtest-0.0.36/inhandtest/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,28 +177,27 @@
 
 def kill_windows_port(ip_, port: int or list) -> None:
     """ 杀死windows 相关端口服务
 
     :param ip_: 本机IP地址
     :param port: int|list, 端口号，可以是多个
     """
-    import socket
+    import psutil
 
     def kill_one_port(one_port: int):
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        for proc in psutil.process_iter(['pid', 'name']):
             try:
-                s.bind((ip_, one_port))
-            except socket.error as e:
-                command = f"taskkill /F /PID {one_port}"
-                p = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                                     encoding='gbk')
-                task_result = p.communicate()[0].strip()
-                logging.info(f'port {one_port} is already in use, and kill result is {task_result}')
-            else:
-                s.close()
+                conn_list = proc.connections()
+            except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+                continue
+            for conn in conn_list:
+                if conn.status == psutil.CONN_LISTEN and conn.laddr.port == one_port:
+                    logging.info(f"进程 {proc.pid} 正在占用端口 {one_port}")
+                    # 终止进程
+                    proc.kill()
 
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
 
 
 def windows_cmd(command: str or list, expect: str or list or dict = None, last_read_replace: dict = None):
     """输入一条或多条命令, 且支持对执行时最后一条命令返回的结果做断言
 
@@ -514,14 +513,29 @@
 
     try:
         _async_raise(thread.ident, SystemExit)
     except Exception as e:
         logging.warning(e)
 
 
+class DotDict(dict):
+    """使用点号深度获取字典key的值
+
+    """
+
+    def __getattr__(self, key):
+        try:
+            return self[key]
+        except KeyError:
+            raise AttributeError(key)
+
+    def __setattr__(self, key, value):
+        self[key] = value
+
+
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
     print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
```

### Comparing `inhandtest-0.0.35/setup.py` & `inhandtest-0.0.36/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.35',
+    version='0.0.36',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
@@ -23,11 +23,11 @@
     package_data={'inhandtest': ['pytest_email.html']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'serial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
-                      'emails', 'Jinja2'
+                      'emails', 'Jinja2', 'pymongo',
                       # 这里是依赖列表，表示运行这个包的运行某些功能还需要你安装其他的包
                       ],
 )
```

