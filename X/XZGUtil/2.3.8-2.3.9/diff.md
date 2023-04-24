# Comparing `tmp/XZGUtil-2.3.8.tar.gz` & `tmp/XZGUtil-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\XZGUtil-2.3.8.tar", last modified: Fri Apr 14 12:17:45 2023, max compression
+gzip compressed data, was "dist\XZGUtil-2.3.9.tar", last modified: Mon Apr 24 02:21:25 2023, max compression
```

## Comparing `XZGUtil-2.3.8.tar` & `XZGUtil-2.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:17:45.000000 XZGUtil-2.3.8/
--rw-rw-rw-   0        0        0      608 2023-04-14 12:17:45.000000 XZGUtil-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2021-05-31 01:49:13.000000 XZGUtil-2.3.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-14 12:17:45.000000 XZGUtil-2.3.8/XZGUtil/
--rw-rw-rw-   0        0        0    77456 2023-04-14 12:16:37.000000 XZGUtil-2.3.8/XZGUtil/DBHelper.py
--rw-rw-rw-   0        0        0     1612 2023-02-15 10:08:17.000000 XZGUtil-2.3.8/XZGUtil/SYCMCryptUtil.py
--rw-rw-rw-   0        0        0      704 2023-03-10 08:44:13.000000 XZGUtil-2.3.8/XZGUtil/__init__.py
--rw-rw-rw-   0        0        0     4214 2023-02-15 07:41:00.000000 XZGUtil-2.3.8/XZGUtil/dealFile.py
--rw-rw-rw-   0        0        0     4893 2022-11-10 03:22:03.000000 XZGUtil-2.3.8/XZGUtil/downFile.py
--rw-rw-rw-   0        0        0   513760 2023-04-04 03:01:05.000000 XZGUtil-2.3.8/XZGUtil/dyXB.py
--rw-rw-rw-   0        0        0    37619 2022-09-21 03:07:37.000000 XZGUtil-2.3.8/XZGUtil/encAndDec.py
--rw-rw-rw-   0        0        0     2469 2022-01-12 08:39:02.000000 XZGUtil-2.3.8/XZGUtil/logger.py
--rw-rw-rw-   0        0        0     1439 2022-11-25 10:54:18.000000 XZGUtil-2.3.8/XZGUtil/messageUtil.py
--rw-rw-rw-   0        0        0     3579 2023-02-14 09:09:37.000000 XZGUtil-2.3.8/XZGUtil/raspberryScan.py
--rw-rw-rw-   0        0        0     1181 2021-06-02 10:25:57.000000 XZGUtil-2.3.8/XZGUtil/re_xzg.py
--rw-rw-rw-   0        0        0    14033 2022-11-25 10:50:05.000000 XZGUtil-2.3.8/XZGUtil/timeUtil.py
--rw-rw-rw-   0        0        0      858 2023-03-10 09:00:37.000000 XZGUtil-2.3.8/XZGUtil/timer.py
--rw-rw-rw-   0        0        0     3429 2023-04-07 02:20:06.000000 XZGUtil-2.3.8/XZGUtil/updateSpider.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:17:45.000000 XZGUtil-2.3.8/XZGUtil.egg-info/
--rw-rw-rw-   0        0        0      608 2023-04-14 12:17:44.000000 XZGUtil-2.3.8/XZGUtil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-04-14 12:17:44.000000 XZGUtil-2.3.8/XZGUtil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:17:44.000000 XZGUtil-2.3.8/XZGUtil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-14 12:17:44.000000 XZGUtil-2.3.8/XZGUtil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 12:17:44.000000 XZGUtil-2.3.8/XZGUtil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 12:17:45.000000 XZGUtil-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-04-14 12:17:20.000000 XZGUtil-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:21:25.000000 XZGUtil-2.3.9/
+-rw-rw-rw-   0        0        0      608 2023-04-24 02:21:25.000000 XZGUtil-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2021-05-31 01:49:13.000000 XZGUtil-2.3.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 02:21:25.000000 XZGUtil-2.3.9/XZGUtil/
+-rw-rw-rw-   0        0        0    77456 2023-04-14 12:16:37.000000 XZGUtil-2.3.9/XZGUtil/DBHelper.py
+-rw-rw-rw-   0        0        0     1612 2023-02-15 10:08:17.000000 XZGUtil-2.3.9/XZGUtil/SYCMCryptUtil.py
+-rw-rw-rw-   0        0        0      704 2023-03-10 08:44:13.000000 XZGUtil-2.3.9/XZGUtil/__init__.py
+-rw-rw-rw-   0        0        0     4214 2023-02-15 07:41:00.000000 XZGUtil-2.3.9/XZGUtil/dealFile.py
+-rw-rw-rw-   0        0        0     5092 2023-04-24 02:21:01.000000 XZGUtil-2.3.9/XZGUtil/downFile.py
+-rw-rw-rw-   0        0        0   513760 2023-04-04 03:01:05.000000 XZGUtil-2.3.9/XZGUtil/dyXB.py
+-rw-rw-rw-   0        0        0    37619 2022-09-21 03:07:37.000000 XZGUtil-2.3.9/XZGUtil/encAndDec.py
+-rw-rw-rw-   0        0        0     2469 2022-01-12 08:39:02.000000 XZGUtil-2.3.9/XZGUtil/logger.py
+-rw-rw-rw-   0        0        0     1439 2022-11-25 10:54:18.000000 XZGUtil-2.3.9/XZGUtil/messageUtil.py
+-rw-rw-rw-   0        0        0     3579 2023-02-14 09:09:37.000000 XZGUtil-2.3.9/XZGUtil/raspberryScan.py
+-rw-rw-rw-   0        0        0     1181 2021-06-02 10:25:57.000000 XZGUtil-2.3.9/XZGUtil/re_xzg.py
+-rw-rw-rw-   0        0        0    14033 2022-11-25 10:50:05.000000 XZGUtil-2.3.9/XZGUtil/timeUtil.py
+-rw-rw-rw-   0        0        0      858 2023-03-10 09:00:37.000000 XZGUtil-2.3.9/XZGUtil/timer.py
+-rw-rw-rw-   0        0        0     3429 2023-04-07 02:20:06.000000 XZGUtil-2.3.9/XZGUtil/updateSpider.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:21:25.000000 XZGUtil-2.3.9/XZGUtil.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-04-24 02:21:23.000000 XZGUtil-2.3.9/XZGUtil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-04-24 02:21:23.000000 XZGUtil-2.3.9/XZGUtil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 02:21:23.000000 XZGUtil-2.3.9/XZGUtil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-24 02:21:23.000000 XZGUtil-2.3.9/XZGUtil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 02:21:23.000000 XZGUtil-2.3.9/XZGUtil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 02:21:25.000000 XZGUtil-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2023-04-24 02:21:11.000000 XZGUtil-2.3.9/setup.py
```

### Comparing `XZGUtil-2.3.8/PKG-INFO` & `XZGUtil-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: XZGUtil
-Version: 2.3.8
+Version: 2.3.9
 Summary: xzgutil
 Home-page: UNKNOWN
 Author: xu-zhiguo
 Author-email: x_zg163@163.com
 License: BSD License
 Description: xzgutil
 Platform: all
```

### Comparing `XZGUtil-2.3.8/XZGUtil/DBHelper.py` & `XZGUtil-2.3.9/XZGUtil/DBHelper.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/SYCMCryptUtil.py` & `XZGUtil-2.3.9/XZGUtil/SYCMCryptUtil.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/__init__.py` & `XZGUtil-2.3.9/XZGUtil/__init__.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/dealFile.py` & `XZGUtil-2.3.9/XZGUtil/dealFile.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/downFile.py` & `XZGUtil-2.3.9/XZGUtil/downFile.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 from XZGUtil.logger import conlog
 from retrying import retry
 from faker import Faker
 
 faker = Faker()
 
 
-def dl_file(name: str, type: str, save_path: str, url: str, cookie=None, header=None, data=None, params=None, method='GET'):
+def dl_file(name: str, type: str, save_path: str, url: str, cookie=None, header=None, data=None, params=None, method='GET', check:int=999999):
     """
     发送请求
     :param name:  文件名
     :param type:  文件类型 ： jpg/gif/excel/xls
     :param save_path:  文件保存路径
     :param url:   下载地址
     :param cookie:  登录信息，str类型
     :param header:  请求头
     :param data:
     :param params:
     :param method:
+    :param check:如果传递此参数，图片小于这个值将会重试
     :return:
     """
     if header:
         pass
     else:
         header = {'cache-control': 'max-age=0',
                   'sec-ch-ua': '".Not/A)Brand";v="99", "Google Chrome";v="103", "Chromium";v="103"',
@@ -39,14 +40,16 @@
                   'sec-ch-ua-platform': '"Windows"',
                   'upgrade-insecure-requests': '1',
                   'user-agent': faker.user_agent(),
                   'accept-language': 'zh-CN,zh;q=0.9'}
     if cookie:
         header['cookie'] = deal_cookie(cookie) if isinstance(cookie, dict) else cookie
     res = __send_req(data, params, method, url, header)
+    if len(res.text) < check:
+        assert False, "文件下载失败，下载大小小于给定值"
     conlog(f'开始下载文件：{name}，大小：{len(res.text)}')
     with open(f'{save_path}{name}.{type}', 'wb') as w:
         w.write(res.content)
     state = check_file_isexist_local(f'{name}.{type}', save_path)
     return state
```

### Comparing `XZGUtil-2.3.8/XZGUtil/dyXB.py` & `XZGUtil-2.3.9/XZGUtil/dyXB.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/encAndDec.py` & `XZGUtil-2.3.9/XZGUtil/encAndDec.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/logger.py` & `XZGUtil-2.3.9/XZGUtil/logger.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/messageUtil.py` & `XZGUtil-2.3.9/XZGUtil/messageUtil.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/raspberryScan.py` & `XZGUtil-2.3.9/XZGUtil/raspberryScan.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/re_xzg.py` & `XZGUtil-2.3.9/XZGUtil/re_xzg.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/timeUtil.py` & `XZGUtil-2.3.9/XZGUtil/timeUtil.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/timer.py` & `XZGUtil-2.3.9/XZGUtil/timer.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil/updateSpider.py` & `XZGUtil-2.3.9/XZGUtil/updateSpider.py`

 * *Files identical despite different names*

### Comparing `XZGUtil-2.3.8/XZGUtil.egg-info/PKG-INFO` & `XZGUtil-2.3.9/XZGUtil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: XZGUtil
-Version: 2.3.8
+Version: 2.3.9
 Summary: xzgutil
 Home-page: UNKNOWN
 Author: xu-zhiguo
 Author-email: x_zg163@163.com
 License: BSD License
 Description: xzgutil
 Platform: all
```

### Comparing `XZGUtil-2.3.8/setup.py` & `XZGUtil-2.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 setup(name='XZGUtil',  # 包名
-      version='2.3.8',  # 版本号
+      version='2.3.9',  # 版本号
       description='xzgutil',
       long_description='xzgutil',
       author='xu-zhiguo',
       author_email='x_zg163@163.com',
       url='',
       install_requires=['postcard', 'retrying', 'python-dateutil'],
       license='BSD License',
```

