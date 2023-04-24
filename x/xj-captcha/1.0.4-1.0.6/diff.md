# Comparing `tmp/xj_captcha-1.0.4.tar.gz` & `tmp/xj_captcha-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_captcha-1.0.4.tar", last modified: Wed Dec  7 09:51:18 2022, max compression
+gzip compressed data, was "dist\xj_captcha-1.0.6.tar", last modified: Mon Apr 24 01:12:55 2023, max compression
```

## Comparing `xj_captcha-1.0.4.tar` & `xj_captcha-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/
--rw-rw-rw-   0        0        0     1438 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      946 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2017 2022-12-07 09:51:10.000000 xj_captcha-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha/
--rw-rw-rw-   0        0        0        0 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha/apis/
--rw-rw-rw-   0        0        0        0 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/apis/__init__.py
--rw-rw-rw-   0        0        0      923 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/apis/send_short_message.py
--rw-rw-rw-   0        0        0      190 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/apps.py
--rw-rw-rw-   0        0        0     1661 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/common.py
--rw-rw-rw-   0        0        0        0 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/models.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha/services/
--rw-rw-rw-   0        0        0        0 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/services/__init__.py
--rw-rw-rw-   0        0        0     5625 2022-12-07 09:47:50.000000 xj_captcha-1.0.4/xj_captcha/services/send_short_message_service.py
--rw-rw-rw-   0        0        0      220 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/urls.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha/utils/
--rw-rw-rw-   0        0        0        0 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/__init__.py
--rw-rw-rw-   0        0        0     1661 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/common.py
--rw-rw-rw-   0        0        0     1350 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/custom_response.py
--rw-rw-rw-   0        0        0      988 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/j_dict.py
--rw-rw-rw-   0        0        0     7311 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/model_handle.py
--rw-rw-rw-   0        0        0     2460 2022-12-07 06:27:38.000000 xj_captcha-1.0.4/xj_captcha/utils/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha.egg-info/
--rw-rw-rw-   0        0        0     1438 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-12-07 09:51:18.000000 xj_captcha-1.0.4/xj_captcha.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/
+-rw-rw-rw-   0        0        0     1438 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2022-09-29 07:15:08.000000 xj_captcha-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2023-04-23 07:23:34.000000 xj_captcha-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/apis/
+-rw-rw-rw-   0        0        0     1397 2023-04-23 01:35:57.000000 xj_captcha-1.0.6/xj_captcha/apis/SmsApis.py
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/apis/__init__.py
+-rw-rw-rw-   0        0        0      923 2022-10-15 09:54:41.000000 xj_captcha-1.0.6/xj_captcha/apis/send_short_message.py
+-rw-rw-rw-   0        0        0      190 2022-09-29 07:08:39.000000 xj_captcha-1.0.6/xj_captcha/apps.py
+-rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/common.py
+-rw-rw-rw-   0        0        0        0 2022-08-26 07:39:01.000000 xj_captcha-1.0.6/xj_captcha/models.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/services/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/services/__init__.py
+-rw-rw-rw-   0        0        0     5625 2022-12-08 07:39:37.000000 xj_captcha-1.0.6/xj_captcha/services/send_short_message_service.py
+-rw-rw-rw-   0        0        0     6126 2023-04-23 07:23:45.000000 xj_captcha-1.0.6/xj_captcha/services/sms_service.py
+-rw-rw-rw-   0        0        0      411 2023-04-23 01:40:00.000000 xj_captcha-1.0.6/xj_captcha/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 06:25:46.000000 xj_captcha-1.0.6/xj_captcha/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/utils/common.py
+-rw-rw-rw-   0        0        0     1350 2022-08-22 01:46:29.000000 xj_captcha-1.0.6/xj_captcha/utils/custom_response.py
+-rw-rw-rw-   0        0        0    23527 2023-04-17 01:01:06.000000 xj_captcha-1.0.6/xj_captcha/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_captcha-1.0.6/xj_captcha/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-08-29 07:52:36.000000 xj_captcha-1.0.6/xj_captcha/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7311 2022-10-15 09:47:02.000000 xj_captcha-1.0.6/xj_captcha/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_captcha-1.0.6/xj_captcha/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     2460 2022-08-26 02:08:41.000000 xj_captcha-1.0.6/xj_captcha/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/
+-rw-rw-rw-   0        0        0     1438 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 01:12:55.000000 xj_captcha-1.0.6/xj_captcha.egg-info/top_level.txt
```

### Comparing `xj_captcha-1.0.4/PKG-INFO` & `xj_captcha-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_captcha
-Version: 1.0.4
+Version: 1.0.6
 Summary: 短信模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_captcha
         
         #### 介绍
         短信模块
```

### Comparing `xj_captcha-1.0.4/README.md` & `xj_captcha-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/setup.py` & `xj_captcha-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_captcha',  # 模块名称
-    version='1.0.4',  # 模块版本
+    version='1.0.6',  # 模块版本
     description='短信模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_payment'],  # 系指定安装模块
     license="apache 3.0",
```

### Comparing `xj_captcha-1.0.4/xj_captcha/apis/send_short_message.py` & `xj_captcha-1.0.6/xj_captcha/apis/send_short_message.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/common.py` & `xj_captcha-1.0.6/xj_captcha/common.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/services/send_short_message_service.py` & `xj_captcha-1.0.6/xj_captcha/services/send_short_message_service.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/utils/common.py` & `xj_captcha-1.0.6/xj_captcha/utils/common.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/utils/custom_response.py` & `xj_captcha-1.0.6/xj_captcha/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/utils/j_config.py` & `xj_captcha-1.0.6/xj_captcha/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/utils/model_handle.py` & `xj_captcha-1.0.6/xj_captcha/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha/utils/utils.py` & `xj_captcha-1.0.6/xj_captcha/utils/utils.py`

 * *Files identical despite different names*

### Comparing `xj_captcha-1.0.4/xj_captcha.egg-info/PKG-INFO` & `xj_captcha-1.0.6/xj_captcha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-captcha
-Version: 1.0.4
+Version: 1.0.6
 Summary: 短信模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_captcha
         
         #### 介绍
         短信模块
```

