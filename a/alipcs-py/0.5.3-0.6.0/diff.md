# Comparing `tmp/alipcs_py-0.5.3.tar.gz` & `tmp/alipcs_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alipcs_py-0.5.3.tar", max compression
+gzip compressed data, was "alipcs_py-0.6.0.tar", max compression
```

## Comparing `alipcs_py-0.5.3.tar` & `alipcs_py-0.6.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1054 2021-08-22 03:34:43.538852 alipcs_py-0.5.3/LICENSE
--rw-r--r--   0        0        0    41449 2023-02-15 06:40:18.091581 alipcs_py-0.5.3/README.md
--rw-r--r--   0        0        0      106 2023-02-28 03:09:49.283441 alipcs_py-0.5.3/alipcs_py/__init__.py
--rw-r--r--   0        0        0      140 2023-02-15 16:28:39.315451 alipcs_py-0.5.3/alipcs_py/alipcs/__init__.py
--rw-r--r--   0        0        0    25991 2023-02-28 03:02:23.303669 alipcs_py-0.5.3/alipcs_py/alipcs/api.py
--rw-r--r--   0        0        0     1820 2023-02-25 05:07:10.262155 alipcs_py-0.5.3/alipcs_py/alipcs/errors.py
--rw-r--r--   0        0        0    17659 2022-10-26 04:22:42.847085 alipcs_py-0.5.3/alipcs_py/alipcs/inner.py
--rw-r--r--   0        0        0    29725 2023-02-28 02:56:07.877499 alipcs_py-0.5.3/alipcs_py/alipcs/pcs.py
--rw-r--r--   0        0        0    12095 2021-08-22 03:34:43.604109 alipcs_py-0.5.3/alipcs_py/alipcs/phone.py
--rw-r--r--   0        0        0     1460 2023-02-15 16:28:39.319727 alipcs_py-0.5.3/alipcs_py/alipcs/tree.py
--rw-r--r--   0        0        0      122 2021-09-18 06:46:25.830052 alipcs_py-0.5.3/alipcs_py/app/__init__.py
--rw-r--r--   0        0        0     5744 2023-02-28 03:00:41.141059 alipcs_py-0.5.3/alipcs_py/app/account.py
--rw-r--r--   0        0        0    47297 2023-02-15 16:28:39.321075 alipcs_py-0.5.3/alipcs_py/app/app.py
--rw-r--r--   0        0        0      825 2022-03-01 05:54:20.767866 alipcs_py-0.5.3/alipcs_py/app/config.py
--rw-r--r--   0        0        0        0 2021-08-22 03:34:43.630951 alipcs_py-0.5.3/alipcs_py/commands/__init__.py
--rw-r--r--   0        0        0      788 2022-12-04 09:09:43.288098 alipcs_py-0.5.3/alipcs_py/commands/cat.py
--rw-r--r--   0        0        0      659 2021-09-18 06:46:25.786441 alipcs_py-0.5.3/alipcs_py/commands/crypto.py
--rw-r--r--   0        0        0    14108 2023-02-19 02:46:52.312109 alipcs_py-0.5.3/alipcs_py/commands/display.py
--rw-r--r--   0        0        0    13621 2023-02-15 16:28:39.323579 alipcs_py-0.5.3/alipcs_py/commands/download.py
--rw-r--r--   0        0        0      494 2022-08-15 03:16:20.571025 alipcs_py-0.5.3/alipcs_py/commands/env.py
--rw-r--r--   0        0        0       40 2021-08-22 03:34:43.661676 alipcs_py-0.5.3/alipcs_py/commands/errors.py
--rw-r--r--   0        0        0     2557 2023-02-15 16:28:39.324554 alipcs_py-0.5.3/alipcs_py/commands/file_operators.py
--rw-r--r--   0        0        0    20246 2021-08-22 03:34:43.626482 alipcs_py-0.5.3/alipcs_py/commands/index.html
--rw-r--r--   0        0        0     5936 2023-02-15 05:59:32.859445 alipcs_py-0.5.3/alipcs_py/commands/list_files.py
--rw-r--r--   0        0        0      508 2022-12-04 07:57:21.765695 alipcs_py-0.5.3/alipcs_py/commands/log.py
--rw-r--r--   0        0        0     8671 2023-02-15 16:28:39.325348 alipcs_py-0.5.3/alipcs_py/commands/play.py
--rw-r--r--   0        0        0      805 2021-09-20 14:44:04.367772 alipcs_py-0.5.3/alipcs_py/commands/search.py
--rw-r--r--   0        0        0     6464 2023-02-15 16:28:39.326106 alipcs_py-0.5.3/alipcs_py/commands/server.py
--rw-r--r--   0        0        0     9571 2023-02-15 16:28:39.326798 alipcs_py-0.5.3/alipcs_py/commands/share.py
--rw-r--r--   0        0        0     2755 2022-11-11 09:35:07.589065 alipcs_py-0.5.3/alipcs_py/commands/sifter.py
--rw-r--r--   0        0        0     2958 2022-12-04 08:10:17.533008 alipcs_py-0.5.3/alipcs_py/commands/sync.py
--rw-r--r--   0        0        0    21566 2023-01-01 14:04:55.047139 alipcs_py-0.5.3/alipcs_py/commands/upload.py
--rw-r--r--   0        0        0      199 2022-08-15 05:04:44.362792 alipcs_py-0.5.3/alipcs_py/commands/user.py
--rw-r--r--   0        0        0     1317 2021-08-22 03:34:43.572027 alipcs_py-0.5.3/alipcs_py/common/cache.py
--rw-r--r--   0        0        0      941 2021-08-22 03:34:43.565972 alipcs_py-0.5.3/alipcs_py/common/concurrent.py
--rw-r--r--   0        0        0      188 2021-08-22 03:34:43.600492 alipcs_py-0.5.3/alipcs_py/common/constant.py
--rw-r--r--   0        0        0     8771 2023-02-15 06:08:25.455318 alipcs_py-0.5.3/alipcs_py/common/crypto.py
--rw-r--r--   0        0        0      785 2021-08-23 15:39:08.472441 alipcs_py-0.5.3/alipcs_py/common/date.py
--rw-r--r--   0        0        0     3328 2022-12-04 08:32:10.634459 alipcs_py-0.5.3/alipcs_py/common/downloader.py
--rw-r--r--   0        0        0     1160 2021-09-18 06:46:25.816885 alipcs_py-0.5.3/alipcs_py/common/event.py
--rw-r--r--   0        0        0     3179 2021-08-22 03:34:43.569872 alipcs_py-0.5.3/alipcs_py/common/file_type.py
--rw-r--r--   0        0        0    33904 2023-02-15 16:28:39.327729 alipcs_py-0.5.3/alipcs_py/common/io.py
--rw-r--r--   0        0        0     2810 2021-08-22 03:34:43.602159 alipcs_py-0.5.3/alipcs_py/common/keyboard.py
--rw-r--r--   0        0        0     1087 2022-12-04 07:54:57.943327 alipcs_py-0.5.3/alipcs_py/common/log.py
--rw-r--r--   0        0        0      700 2022-03-20 08:23:18.211962 alipcs_py-0.5.3/alipcs_py/common/net.py
--rw-r--r--   0        0        0      165 2021-08-22 03:34:43.568880 alipcs_py-0.5.3/alipcs_py/common/number.py
--rw-r--r--   0        0        0     1554 2022-12-04 07:52:11.933700 alipcs_py-0.5.3/alipcs_py/common/path.py
--rw-r--r--   0        0        0      143 2021-08-22 03:34:43.595732 alipcs_py-0.5.3/alipcs_py/common/platform.py
--rw-r--r--   0        0        0     1154 2022-12-03 16:04:42.948527 alipcs_py-0.5.3/alipcs_py/common/progress_bar.py
--rw-r--r--   0        0        0     1322 2021-08-22 03:34:43.598103 alipcs_py-0.5.3/alipcs_py/common/simple_cipher.pyx
--rw-r--r--   0        0        0       73 2021-08-22 03:34:43.596516 alipcs_py-0.5.3/alipcs_py/common/url.py
--rw-r--r--   0        0        0      451 2022-03-02 13:55:46.279575 alipcs_py-0.5.3/alipcs_py/common/util.py
--rw-r--r--   0        0        0     1208 2022-03-01 06:20:58.123489 alipcs_py-0.5.3/alipcs_py/config/__init__.py
--rw-r--r--   0        0        0        0 2022-03-06 15:08:01.483390 alipcs_py-0.5.3/alipcs_py/storage/__init__.py
--rw-r--r--   0        0        0     6225 2022-08-15 06:17:51.409475 alipcs_py-0.5.3/alipcs_py/storage/store.py
--rw-r--r--   0        0        0     5248 2023-02-15 16:28:39.328505 alipcs_py-0.5.3/alipcs_py/storage/tables.py
--rw-r--r--   0        0        0     1424 2021-08-22 03:34:43.602731 alipcs_py-0.5.3/alipcs_py/utils.py
--rw-r--r--   0        0        0      735 2021-09-18 06:47:25.953980 alipcs_py-0.5.3/build.py
--rw-r--r--   0        0        0     1251 2023-02-28 03:09:32.245850 alipcs_py-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    43736 1970-01-01 00:00:00.000000 alipcs_py-0.5.3/setup.py
--rw-r--r--   0        0        0    42978 1970-01-01 00:00:00.000000 alipcs_py-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1054 2021-08-22 03:34:43.538852 alipcs_py-0.6.0/LICENSE
+-rw-r--r--   0        0        0    43879 2023-04-24 09:44:53.678600 alipcs_py-0.6.0/README.md
+-rw-r--r--   0        0        0      106 2023-04-24 09:45:36.012429 alipcs_py-0.6.0/alipcs_py/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-24 04:55:07.710097 alipcs_py-0.6.0/alipcs_py/alipcs/__init__.py
+-rw-r--r--   0        0        0    38662 2023-04-24 04:55:07.710855 alipcs_py-0.6.0/alipcs_py/alipcs/api.py
+-rw-r--r--   0        0        0     1820 2023-02-25 05:07:10.262155 alipcs_py-0.6.0/alipcs_py/alipcs/errors.py
+-rw-r--r--   0        0        0    18578 2023-04-24 04:55:07.711733 alipcs_py-0.6.0/alipcs_py/alipcs/inner.py
+-rw-r--r--   0        0        0    43631 2023-04-24 04:55:07.712884 alipcs_py-0.6.0/alipcs_py/alipcs/pcs.py
+-rw-r--r--   0        0        0    12095 2021-08-22 03:34:43.604109 alipcs_py-0.6.0/alipcs_py/alipcs/phone.py
+-rw-r--r--   0        0        0     1446 2023-04-24 04:55:07.713710 alipcs_py-0.6.0/alipcs_py/alipcs/tree.py
+-rw-r--r--   0        0        0      122 2021-09-18 06:46:25.830052 alipcs_py-0.6.0/alipcs_py/app/__init__.py
+-rw-r--r--   0        0        0     8026 2023-04-24 04:55:07.714364 alipcs_py-0.6.0/alipcs_py/app/account.py
+-rw-r--r--   0        0        0    50217 2023-04-24 04:55:07.715041 alipcs_py-0.6.0/alipcs_py/app/app.py
+-rw-r--r--   0        0        0      825 2022-03-01 05:54:20.767866 alipcs_py-0.6.0/alipcs_py/app/config.py
+-rw-r--r--   0        0        0        0 2021-08-22 03:34:43.630951 alipcs_py-0.6.0/alipcs_py/commands/__init__.py
+-rw-r--r--   0        0        0      788 2022-12-04 09:09:43.288098 alipcs_py-0.6.0/alipcs_py/commands/cat.py
+-rw-r--r--   0        0        0      653 2023-04-24 04:55:07.715731 alipcs_py-0.6.0/alipcs_py/commands/crypto.py
+-rw-r--r--   0        0        0    14746 2023-04-24 04:55:07.716544 alipcs_py-0.6.0/alipcs_py/commands/display.py
+-rw-r--r--   0        0        0    13989 2023-04-24 04:55:07.717597 alipcs_py-0.6.0/alipcs_py/commands/download.py
+-rw-r--r--   0        0        0      494 2022-08-15 03:16:20.571025 alipcs_py-0.6.0/alipcs_py/commands/env.py
+-rw-r--r--   0        0        0       40 2021-08-22 03:34:43.661676 alipcs_py-0.6.0/alipcs_py/commands/errors.py
+-rw-r--r--   0        0        0     2557 2023-02-15 16:28:39.324554 alipcs_py-0.6.0/alipcs_py/commands/file_operators.py
+-rw-r--r--   0        0        0    20271 2023-03-03 16:42:13.787873 alipcs_py-0.6.0/alipcs_py/commands/index.html
+-rw-r--r--   0        0        0     5938 2023-04-24 04:55:07.718624 alipcs_py-0.6.0/alipcs_py/commands/list_files.py
+-rw-r--r--   0        0        0      508 2022-12-04 07:57:21.765695 alipcs_py-0.6.0/alipcs_py/commands/log.py
+-rw-r--r--   0        0        0     1250 2023-04-24 04:55:07.719052 alipcs_py-0.6.0/alipcs_py/commands/login.py
+-rw-r--r--   0        0        0     9030 2023-04-24 04:55:07.719536 alipcs_py-0.6.0/alipcs_py/commands/play.py
+-rw-r--r--   0        0        0      805 2021-09-20 14:44:04.367772 alipcs_py-0.6.0/alipcs_py/commands/search.py
+-rw-r--r--   0        0        0     6832 2023-04-24 04:55:07.720197 alipcs_py-0.6.0/alipcs_py/commands/server.py
+-rw-r--r--   0        0        0     9303 2023-04-24 04:55:07.720989 alipcs_py-0.6.0/alipcs_py/commands/share.py
+-rw-r--r--   0        0        0     2670 2023-04-24 04:55:07.722333 alipcs_py-0.6.0/alipcs_py/commands/sifter.py
+-rw-r--r--   0        0        0     2900 2023-04-24 04:55:07.723021 alipcs_py-0.6.0/alipcs_py/commands/sync.py
+-rw-r--r--   0        0        0    21434 2023-04-24 04:55:07.723636 alipcs_py-0.6.0/alipcs_py/commands/upload.py
+-rw-r--r--   0        0        0      199 2022-08-15 05:04:44.362792 alipcs_py-0.6.0/alipcs_py/commands/user.py
+-rw-r--r--   0        0        0     1317 2021-08-22 03:34:43.572027 alipcs_py-0.6.0/alipcs_py/common/cache.py
+-rw-r--r--   0        0        0      941 2021-08-22 03:34:43.565972 alipcs_py-0.6.0/alipcs_py/common/concurrent.py
+-rw-r--r--   0        0        0      188 2021-08-22 03:34:43.600492 alipcs_py-0.6.0/alipcs_py/common/constant.py
+-rw-r--r--   0        0        0     8745 2023-04-24 04:55:07.724749 alipcs_py-0.6.0/alipcs_py/common/crypto.py
+-rw-r--r--   0        0        0      751 2023-04-24 04:55:07.725914 alipcs_py-0.6.0/alipcs_py/common/date.py
+-rw-r--r--   0        0        0     3328 2022-12-04 08:32:10.634459 alipcs_py-0.6.0/alipcs_py/common/downloader.py
+-rw-r--r--   0        0        0     1160 2021-09-18 06:46:25.816885 alipcs_py-0.6.0/alipcs_py/common/event.py
+-rw-r--r--   0        0        0     3179 2021-08-22 03:34:43.569872 alipcs_py-0.6.0/alipcs_py/common/file_type.py
+-rw-r--r--   0        0        0    33495 2023-04-24 04:55:07.727448 alipcs_py-0.6.0/alipcs_py/common/io.py
+-rw-r--r--   0        0        0     2810 2021-08-22 03:34:43.602159 alipcs_py-0.6.0/alipcs_py/common/keyboard.py
+-rw-r--r--   0        0        0     1087 2022-12-04 07:54:57.943327 alipcs_py-0.6.0/alipcs_py/common/log.py
+-rw-r--r--   0        0        0      700 2022-03-20 08:23:18.211962 alipcs_py-0.6.0/alipcs_py/common/net.py
+-rw-r--r--   0        0        0      165 2021-08-22 03:34:43.568880 alipcs_py-0.6.0/alipcs_py/common/number.py
+-rw-r--r--   0        0        0     1554 2022-12-04 07:52:11.933700 alipcs_py-0.6.0/alipcs_py/common/path.py
+-rw-r--r--   0        0        0      143 2021-08-22 03:34:43.595732 alipcs_py-0.6.0/alipcs_py/common/platform.py
+-rw-r--r--   0        0        0     1154 2022-12-03 16:04:42.948527 alipcs_py-0.6.0/alipcs_py/common/progress_bar.py
+-rw-r--r--   0        0        0     1322 2021-08-22 03:34:43.598103 alipcs_py-0.6.0/alipcs_py/common/simple_cipher.pyx
+-rw-r--r--   0        0        0       73 2021-08-22 03:34:43.596516 alipcs_py-0.6.0/alipcs_py/common/url.py
+-rw-r--r--   0        0        0      451 2022-03-02 13:55:46.279575 alipcs_py-0.6.0/alipcs_py/common/util.py
+-rw-r--r--   0        0        0     1208 2022-03-01 06:20:58.123489 alipcs_py-0.6.0/alipcs_py/config/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-06 15:08:01.483390 alipcs_py-0.6.0/alipcs_py/storage/__init__.py
+-rw-r--r--   0        0        0     6121 2023-04-24 04:55:07.728382 alipcs_py-0.6.0/alipcs_py/storage/store.py
+-rw-r--r--   0        0        0     5188 2023-04-24 04:55:07.729402 alipcs_py-0.6.0/alipcs_py/storage/tables.py
+-rw-r--r--   0        0        0     1424 2021-08-22 03:34:43.602731 alipcs_py-0.6.0/alipcs_py/utils.py
+-rw-r--r--   0        0        0      735 2021-09-18 06:47:25.953980 alipcs_py-0.6.0/build.py
+-rw-r--r--   0        0        0     1366 2023-04-24 09:45:21.354430 alipcs_py-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    46242 1970-01-01 00:00:00.000000 alipcs_py-0.6.0/setup.py
+-rw-r--r--   0        0        0    45389 1970-01-01 00:00:00.000000 alipcs_py-0.6.0/PKG-INFO
```

### Comparing `alipcs_py-0.5.3/LICENSE` & `alipcs_py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/README.md` & `alipcs_py-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # AliPCS-Py
 
+**2023-04-24 支持 阿里云盘开放平台 api。**
+
 **2023-02-15 使用临时 API 接口，让下载可用。**
 
 **2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**
 
 [![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)
 ![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)
 
@@ -82,15 +84,15 @@
 
 #### HTTP 服务
 
 - [开启 HTTP 服务](#开启-HTTP-服务)
 
 ## 安装
 
-需要 Python 版本大于或等于 3.7
+需要 Python 版本大于或等于 3.8
 
 ```
 pip3 install Cython
 pip3 install AliPCS-Py
 ```
 
 ### Windows 依赖
@@ -202,15 +204,59 @@
 - save
 - server
 
 **注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。
 
 ## 添加用户
 
-AliPCS-Py 目前支持用`refresh_token`登录。需要使用者在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。
+**从 2023-02-14 开始，阿里云盘官方限制了 web 端 api 的调用。从 web 端 api 获取到的下载连接是限速的。但如果调用[阿里云盘开放平台](https://survey.alibaba.com/apps/zhiliao/I9Dd1Nl89)的 api 获取到的下载连接是不限速的。**
+
+AliPCS-Py (>= v0.6.0) 支持调用阿里云盘开放平台 api。但是由于一直没有拿到内测，没法提供默认登录操作。需要用户自己找其他应用提供的登录方式登录。
+
+### 使用 web `refresh_token` 和 第三方认证地址 登录
+
+第三方认证地址提供阿里云盘开放平台的认证服务。由于一直没有拿到内测，本项目目前没法提供。需要使用者自行寻找。
+
+交互添加：
+
+```
+AliPCS-Py useradd
+```
+
+或者直接添加：
+
+```
+AliPCS-Py useradd --web-refresh-token "..." --client-server "..."
+# 其他选项留空
+```
+
+之后用阿里云盘 APP 扫码登录。
+
+### 使用 web `refresh_token` 和 阿里云盘开放平台认证凭证 登录
+
+如果使用者拿到了阿里云盘开放平台认证，会获得 `client-id` 和 `client-secret`。使用这两个值可以直接登录。
+
+交互添加：
+
+```
+AliPCS-Py useradd
+```
+
+或者直接添加：
+
+```
+AliPCS-Py useradd --web-refresh-token "..." --client-id "..." --client-secret "..."
+# 其他选项留空
+```
+
+之后用阿里云盘 APP 扫码登录。
+
+### 使用 web `refresh_token` 登录
+
+使用者需要在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。`useradd` 其他参数留空就好。
 
 使用者可以用下面的方式获取用户的 `refresh_token` 值。
 
 1. 登录 https://www.aliyundrive.com/drive/
 2. 打开浏览器的开发者工具(如 Chrome DevTools)。
 3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。
 
@@ -223,19 +269,21 @@
 ```
 AliPCS-Py useradd
 ```
 
 或者直接添加：
 
 ```
-AliPCS-Py useradd --refresh-token "..."
+AliPCS-Py useradd --web-refresh-token "..."
 ```
 
 AliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。
 
+**注意：如果只用 `--web-refresh-token` 登录，下载文件时，服务器端会限速。**
+
 ## 显示当前用户的信息
 
 ```
 AliPCS-Py who
 ```
 
 或者：
@@ -244,17 +292,23 @@
 AliPCS-Py who user_id
 ```
 
 指明显示用户 id 为 `user_id` 的用户信息。
 
 ### 选项
 
-| Option                      | Description  |
-| --------------------------- | ------------ |
-| -K, --show-encrypt-password | 显示加密密码 |
+| Option                       | Description                |
+| ---------------------------- | -------------------------- |
+| -K, --show-encrypt-password  | 显示加密密码               |
+| --account-name TEXT          | 账号名 [默认为 user id]    |
+| --web-refresh-token TEXT     | 用户 web_refresh_token     |
+| --openapi-refresh-token TEXT | 用户 openapi_refresh_token |
+| --client-id TEXT             | openapi client id          |
+| --client-secret TEXT         | openapi client secret      |
+| --client-server TEXT         | openapi client server      |
 
 ## 更新用户信息
 
 默认更新当前用户信息。
 
 ```
 AliPCS-Py updateuser
@@ -569,14 +623,17 @@
 
 | Option        | Description  |
 | ------------- | ------------ |
 | -i, --file-id | TEXT 文件 ID |
 
 ## 下载文件或目录
 
+> 在使用了阿里云盘开放平台 api 时，如果下载他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中下载。
+> 下载结束后，会删除 `__alipcs_py_temp__` 中下载的文件。
+
 使用文件路径：
 
 ```
 AliPCS-Py download [OPTIONS] [REMOTEPATHS]...
 ```
 
 使用文件 ID：
@@ -605,14 +662,17 @@
 | -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | -d, --downloader [ me \| aget_py \| aget_rs \| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |
 | --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |
 
 ## 播放媒体文件
 
+> 在使用了阿里云盘开放平台 api 时，如果播放他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中播放。
+> 播放结束后，会删除 `__alipcs_py_temp__` 中播放的文件。
+
 使用文件路径：
 
 ```
 AliPCS-Py play [OPTIONS] [REMOTEPATHS]...
 ```
 
 使用文件 ID：
```

### Comparing `alipcs_py-0.5.3/alipcs_py/alipcs/api.py` & `alipcs_py-0.6.0/alipcs_py/alipcs/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,98 @@
-from typing import (
-    Optional,
-    List,
-    Tuple,
-    Dict,
-    DefaultDict,
-    Iterable,
-    Iterator,
-    Callable,
-    IO,
-)
+from typing import Optional, List, Tuple, Dict, Union, DefaultDict, Iterable, Iterator, Callable, IO
 from threading import Lock
 from collections import defaultdict
 from copy import deepcopy
 from functools import partial
 import logging
 
 from alipcs_py.alipcs.errors import AliPCSError
 from alipcs_py.common.io import RangeRequestIO, DEFAULT_MAX_CHUNK_SIZE
-from alipcs_py.alipcs.pcs import AliPCS, CheckNameMode
-from alipcs_py.alipcs.inner import (
-    PcsFile,
-    PcsPreparedFile,
-    PcsSharedLink,
-    PcsSharedLinkInfo,
-    PcsUser,
-    PcsDownloadUrl,
-)
+from alipcs_py.alipcs.pcs import AliPCS, AliOpenPCS, CheckNameMode
+from alipcs_py.alipcs.inner import PcsFile, PcsPreparedFile, PcsSharedLink, PcsSharedLinkInfo, PcsUser, PcsDownloadUrl
 from alipcs_py.common.path import split_posix_path, join_path, posix_path_dirname
 
 from requests_toolbelt import MultipartEncoderMonitor
 
 logger = logging.getLogger(__name__)
 
 
 _ALI_PCS_API_LOCK = Lock()
 
 
 class AliPCSApi:
-    """Ali PCS Api
+    """Aliyundrive PCS Api
 
     This is the wrapper of `AliPCS`. It parses the content of response of raw
     AliPCS requests to some inner data structions.
     """
 
     def __init__(
         self,
         refresh_token: str,
         access_token: str = "",
+        token_type: str = "",
         expire_time: int = 0,
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
-        token_type: str = "",
         device_id: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
     ):
         self._alipcs = AliPCS(
             refresh_token,
             access_token=access_token,
+            token_type=token_type,
             expire_time=expire_time,
             user_id=user_id,
             user_name=user_name,
             nick_name=nick_name,
-            token_type=token_type,
             device_id=device_id,
             default_drive_id=default_drive_id,
             role=role,
             status=status,
         )
 
         # The path tree is for user's own files
         self._path_tree = PathTree(self)
 
         # Map `share_id` to a `PathTree` for that shared link
-        self._shared_path_tree: DefaultDict[str, PathTree] = defaultdict(
-            partial(PathTree, self)
-        )
+        self._shared_path_tree: DefaultDict[str, PathTree] = defaultdict(partial(PathTree, self))
 
     @property
     def refresh_token(self) -> str:
         return self._alipcs.refresh_token
 
     @property
     def access_token(self) -> str:
         return self._alipcs.access_token
 
     @property
+    def token_type(self) -> str:
+        return self._alipcs.token_type
+
+    @property
+    def expire_time(self) -> int:
+        return self._alipcs.expire_time
+
+    @property
     def user_id(self) -> str:
         return self._alipcs.user_id
 
     @property
     def user_name(self) -> str:
         return self._alipcs.user_name
 
     @property
     def nick_name(self) -> str:
         return self._alipcs.nick_name
 
     @property
-    def token_type(self) -> str:
-        return self._alipcs.token_type
-
-    @property
-    def expire_time(self) -> int:
-        return self._alipcs.expire_time
-
-    @property
     def device_id(self) -> str:
         return self._alipcs.device_id
 
     @property
     def default_drive_id(self) -> str:
         return self._alipcs.default_drive_id
 
@@ -160,16 +141,16 @@
         file_id: str,
         share_id: str = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
-        limit: int = 100,
-        url_expire_sec: int = 7200,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
         next_marker: str = "",
     ) -> Tuple[List[PcsFile], str]:
         """List the directory's contents
 
         List files and directories in the given directory (which has the `file_id`).
         The return items size is limited by the `limit` parameter. If you want to list
         more, using the returned `next_marker` parameter for next `list` call.
@@ -195,16 +176,16 @@
         file_id: str,
         share_id: str = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
-        limit: int = 100,
-        url_expire_sec: int = 7200,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
         recursive: bool = False,
         include_dir: bool = True,
     ) -> Iterator[PcsFile]:
         """Iterate the directory by its `file_id`
 
         Iterate all files and directories at the directory (which has the `file_id`).
         """
@@ -253,17 +234,15 @@
             if not next_marker:
                 return
 
     def path(self, remotepath: str, share_id: str = None) -> Optional[PcsFile]:
         """Get the pcs file's info by the given absolute `remotepath`"""
 
         if share_id:
-            return self._shared_path_tree[share_id].search(
-                remotepath=remotepath, share_id=share_id
-            )
+            return self._shared_path_tree[share_id].search(remotepath=remotepath, share_id=share_id)
         else:
             return self._path_tree.search(remotepath=remotepath)
 
     def paths(self, *remotepaths: str, share_id: str = None) -> List[Optional[PcsFile]]:
         """Get the pcs files' info by the given absolute `remotepaths`"""
 
         return [self.path(rp, share_id=share_id) for rp in remotepaths]
@@ -274,16 +253,16 @@
         file_id: str = None,
         share_id: str = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
-        limit: int = 100,
-        url_expire_sec: int = 7200,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
         recursive: bool = False,
         include_dir: bool = True,
     ) -> Iterator[PcsFile]:
         """Iterate the `remotepath`"""
 
         if not file_id:
             pf = self.path(remotepath, share_id=share_id)
@@ -315,16 +294,16 @@
         file_id: str = None,
         share_id: str = None,
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
-        limit: int = 100,
-        url_expire_sec: int = 7200,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
     ) -> List[PcsFile]:
         return list(
             self.list_path_iter(
                 remotepath,
                 file_id=file_id,
                 share_id=share_id,
                 desc=desc,
@@ -391,46 +370,31 @@
         pre_hash: str,
         part_number: int = 1,
         check_name_mode: CheckNameMode = "auto_rename",
     ) -> PcsPreparedFile:
         """Create a prepared file with `pre_hash` for uploading"""
 
         return self.create_file(
-            filename,
-            dir_id,
-            size,
-            pre_hash=pre_hash,
-            part_number=part_number,
-            check_name_mode=check_name_mode,
+            filename, dir_id, size, pre_hash=pre_hash, part_number=part_number, check_name_mode=check_name_mode
         )
 
     def rapid_upload_file(
         self,
         filename: str,
         dir_id: str,
         size: int,
         content_hash: str,
         proof_code: str,
         check_name_mode: CheckNameMode = "auto_rename",
     ) -> PcsPreparedFile:
         return self.create_file(
-            filename,
-            dir_id,
-            size,
-            content_hash=content_hash,
-            proof_code=proof_code,
-            check_name_mode=check_name_mode,
+            filename, dir_id, size, content_hash=content_hash, proof_code=proof_code, check_name_mode=check_name_mode
         )
 
-    def upload_slice(
-        self,
-        io: IO,
-        url: str,
-        callback: Callable[[MultipartEncoderMonitor], None] = None,
-    ) -> None:
+    def upload_slice(self, io: IO, url: str, callback: Callable[[MultipartEncoderMonitor], None] = None) -> None:
         """Upload an io as a slice
 
         callable: the callback for monitoring uploading progress
         """
 
         self._alipcs.upload_slice(io, url, callback=callback)
 
@@ -455,22 +419,15 @@
         all: bool = False,
         limit: int = 100,
         next_marker: str = "",
     ) -> Tuple[List[PcsFile], str]:
         """Search with `keyword`"""
 
         info = self._alipcs.search(
-            keyword,
-            desc=desc,
-            name=name,
-            time=time,
-            size=size,
-            all=all,
-            limit=limit,
-            next_marker=next_marker,
+            keyword, desc=desc, name=name, time=time, size=size, all=all, limit=limit, next_marker=next_marker
         )
         next_marker = info["next_marker"]
         return [PcsFile.from_(v) for v in info.get("items", [])], next_marker
 
     def search_all(
         self,
         keyword: str,
@@ -564,38 +521,30 @@
 
         # Remove nodes from self._path_tree
         for file_id in file_ids[:-1]:
             self._path_tree.pop_by_file_id(file_id)
 
         return ["code" not in v for v in info["responses"]]
 
-    def share(
-        self, *file_ids: str, password: str = "", period: int = 0, description: str = ""
-    ) -> PcsSharedLink:
+    def share(self, *file_ids: str, password: str = "", period: int = 0, description: str = "") -> PcsSharedLink:
         """Share `remotepaths` to public with a optional password
 
         Args:
             period (int): The days for expiring. `0` means no expiring
         """
 
-        info = self._alipcs.share(
-            *file_ids, password=password, period=period, description=description
-        )
+        info = self._alipcs.share(*file_ids, password=password, period=period, description=description)
         return PcsSharedLink.from_(info)
 
     def is_shared_valid(self, share_id: str) -> bool:
         try:
             self.shared_info(share_id)
             return True
         except AliPCSError as err:
-            if err.error_code in (
-                "ShareLink.Forbidden",
-                "ShareLink.Cancelled",
-                "ShareLink.Expired",
-            ):
+            if err.error_code in ("ShareLink.Forbidden", "ShareLink.Cancelled", "ShareLink.Expired"):
                 return False
             raise
 
     def list_shared(self, next_marker: str = "") -> Tuple[List[PcsSharedLink], str]:
         """List shared link on a page"""
 
         info = self._alipcs.list_shared(next_marker=next_marker)
@@ -630,57 +579,45 @@
         while True:
             try:
                 info = self._alipcs.shared_info(share_id)
                 return PcsSharedLinkInfo.from_(info)
             except AliPCSError as err:
                 # XXX: What is the error?
                 if err.error_code == "ParamFlowException":
-                    logger.debug(
-                        "AliPCSApi.shared_info gets error: `ParamFlowException`"
-                    )
+                    logger.debug("AliPCSApi.shared_info gets error: `ParamFlowException`")
                     continue
                 else:
                     raise
 
     # list_shared_files is an alias of list
     list_shared_files = list
 
     def transfer_shared_files(
-        self,
-        shared_file_ids: List[str],
-        dest_id: str,
-        share_id: str,
-        auto_rename: bool = False,
+        self, shared_file_ids: List[str], dest_id: str, share_id: str, auto_rename: bool = False
     ) -> List[PcsFile]:
         """Save the `shared_file_ids` to `dest_id`"""
 
-        info = self._alipcs.transfer_shared_files(
-            shared_file_ids, dest_id, share_id, auto_rename=auto_rename
-        )
+        info = self._alipcs.transfer_shared_files(shared_file_ids, dest_id, share_id, auto_rename=auto_rename)
         return [PcsFile.from_(v["body"]) for v in info.get("responses", [])]
 
-    def shared_file_download_url(
-        self, shared_file_id: str, share_id: str, expire_duration: int = 10 * 60
-    ) -> str:
+    def shared_file_download_url(self, shared_file_id: str, share_id: str, expire_duration: int = 10 * 60) -> str:
         """Get shared file download link"""
 
-        return self._alipcs.shared_file_download_url(
-            shared_file_id, share_id, expire_duration=expire_duration
-        )
+        return self._alipcs.shared_file_download_url(shared_file_id, share_id, expire_duration=expire_duration)
 
     def user_info(self) -> PcsUser:
         """User's information"""
 
         info = self._alipcs.user_info()
 
         user_info = PcsUser.from_(info)
-        user_info.refresh_token = self.refresh_token
-        user_info.access_token = self.access_token
-        user_info.token_type = self.token_type
-        user_info.expire_time = self.expire_time
+        user_info.web_refresh_token = self.refresh_token
+        user_info.web_access_token = self.access_token
+        user_info.web_token_type = self.token_type
+        user_info.web_expire_time = self.expire_time
         user_info.device_id = self.device_id
         return user_info
 
     def download_link(self, file_id: str) -> Optional[PcsDownloadUrl]:
         """Get the download link of the `file_id`"""
 
         info = self._alipcs.download_link(file_id)
@@ -692,18 +629,15 @@
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
         callback: Callable[..., None] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
         """File stream as a normal io"""
 
         return self._alipcs.file_stream(
-            file_id,
-            max_chunk_size=max_chunk_size,
-            callback=callback,
-            encrypt_password=encrypt_password,
+            file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
         )
 
     def shared_file_stream(
         self,
         shared_file_id: str,
         share_id: str,
         expire_duration: int = 10 * 60,
@@ -719,14 +653,439 @@
             expire_duration=expire_duration,
             max_chunk_size=max_chunk_size,
             callback=callback,
             encrypt_password=encrypt_password,
         )
 
 
+class AliOpenPCSApi:
+    """Aliyundrive Open PCS Api
+
+    This is the wrapper of `AliPCS`. It parses the content of response of raw
+    AliPCS requests to some inner data structions.
+    """
+
+    def __init__(
+        self,
+        refresh_token: str,
+        access_token: str = "",
+        expire_time: int = 0,
+        client_id: str = "",
+        client_secret: str = "",
+        client_server: str = "",
+        user_id: str = "",
+        user_name: str = "",
+        nick_name: str = "",
+        token_type: str = "",
+        default_drive_id: str = "",
+        role: str = "",
+        status: str = "",
+    ):
+        self._aliopenpcs = AliOpenPCS(
+            refresh_token,
+            access_token=access_token,
+            expire_time=expire_time,
+            client_id=client_id,
+            client_secret=client_secret,
+            client_server=client_server,
+            user_id=user_id,
+            user_name=user_name,
+            nick_name=nick_name,
+            token_type=token_type,
+            default_drive_id=default_drive_id,
+            role=role,
+            status=status,
+        )
+
+        # The path tree is for user's own files
+        self._path_tree = PathTree(self)
+
+        # Map `share_id` to a `PathTree` for that shared link
+        self._shared_path_tree: DefaultDict[str, PathTree] = defaultdict(partial(PathTree, self))
+
+    @property
+    def refresh_token(self) -> str:
+        return self._aliopenpcs.refresh_token
+
+    @property
+    def access_token(self) -> str:
+        return self._aliopenpcs.access_token
+
+    @property
+    def token_type(self) -> str:
+        return self._aliopenpcs.token_type
+
+    @property
+    def client_id(self) -> str:
+        return self._aliopenpcs.client_id
+
+    @property
+    def client_secret(self) -> str:
+        return self._aliopenpcs.client_secret
+
+    @property
+    def client_server(self) -> str:
+        return self._aliopenpcs.client_server
+
+    @property
+    def user_id(self) -> str:
+        return self._aliopenpcs.user_id
+
+    @property
+    def user_name(self) -> str:
+        return self._aliopenpcs.user_name
+
+    @property
+    def nick_name(self) -> str:
+        return self._aliopenpcs.nick_name
+
+    @property
+    def expire_time(self) -> int:
+        return self._aliopenpcs.expire_time
+
+    @property
+    def default_drive_id(self) -> str:
+        return self._aliopenpcs.default_drive_id
+
+    @property
+    def role(self) -> str:
+        return self._aliopenpcs.role
+
+    @property
+    def status(self) -> str:
+        return self._aliopenpcs.status
+
+    def meta(self, *file_ids: str, share_id: str = None) -> List[PcsFile]:
+        """Meta data of `remotepaths`"""
+
+        pcs_files = [PcsFile.root() if fid == "root" else None for fid in file_ids]
+        fids = [fid for fid in file_ids if fid != "root"]
+
+        if fids:
+            info = self._aliopenpcs.meta(*fids, share_id=share_id)
+            pfs = [PcsFile.from_(v.get("body")) for v in info["responses"]]
+            j = 0
+            for i in range(len(pcs_files)):
+                if pcs_files[i] is None:
+                    pcs_files[i] = pfs[j]
+                    j += 1
+
+        return [pf for pf in pcs_files if pf is not None]
+
+    def exists(self, file_id: str) -> bool:
+        """Check whether `remotepath` exists"""
+
+        return self._aliopenpcs.exists(file_id)
+
+    def is_file(self, file_id: str) -> bool:
+        """Check whether `remotepath` is a file"""
+
+        return self._aliopenpcs.is_file(file_id)
+
+    def is_dir(self, file_id: str) -> bool:
+        """Check whether `remotepath` is a directory"""
+
+        return self._aliopenpcs.is_dir(file_id)
+
+    def list(
+        self,
+        file_id: str,
+        share_id: str = None,
+        desc: bool = False,
+        name: bool = False,
+        time: bool = False,
+        size: bool = False,
+        all: bool = False,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
+        next_marker: str = "",
+    ) -> Tuple[List[PcsFile], str]:
+        """List the directory's contents
+
+        List files and directories in the given directory (which has the `file_id`).
+        The return items size is limited by the `limit` parameter. If you want to list
+        more, using the returned `next_marker` parameter for next `list` call.
+        """
+
+        info = self._aliopenpcs.list(
+            file_id=file_id,
+            share_id=share_id,
+            desc=desc,
+            name=name,
+            time=time,
+            size=size,
+            all=all,
+            limit=limit,
+            url_expire_sec=url_expire_sec,
+            next_marker=next_marker,
+        )
+        next_marker = info["next_marker"]
+        return [PcsFile.from_(v) for v in info.get("items", [])], next_marker
+
+    def list_iter(
+        self,
+        file_id: str,
+        share_id: str = None,
+        desc: bool = False,
+        name: bool = False,
+        time: bool = False,
+        size: bool = False,
+        all: bool = False,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
+        recursive: bool = False,
+        include_dir: bool = True,
+    ) -> Iterator[PcsFile]:
+        """Iterate the directory by its `file_id`
+
+        Iterate all files and directories at the directory (which has the `file_id`).
+        """
+
+        next_marker = ""
+        pcs_file = self.meta(file_id, share_id=share_id)[0]
+        dirname = pcs_file.name
+        while True:
+            pcs_files, next_marker = self.list(
+                file_id,
+                share_id=share_id,
+                desc=desc,
+                name=name,
+                time=time,
+                size=size,
+                all=all,
+                limit=limit,
+                url_expire_sec=url_expire_sec,
+                next_marker=next_marker,
+            )
+            for pf in pcs_files:
+                pf.path = join_path(dirname, pf.name)
+
+                if pf.is_dir:
+                    if include_dir:
+                        yield pf
+                    if recursive:
+                        for sub_pf in self.list_iter(
+                            pf.file_id,
+                            share_id=share_id,
+                            desc=desc,
+                            name=name,
+                            time=time,
+                            size=size,
+                            all=all,
+                            limit=limit,
+                            url_expire_sec=url_expire_sec,
+                            recursive=recursive,
+                            include_dir=include_dir,
+                        ):
+                            sub_pf.path = join_path(dirname, sub_pf.path)
+                            yield sub_pf
+                else:
+                    yield pf
+
+            if not next_marker:
+                return
+
+    def path(self, remotepath: str, share_id: str = None) -> Optional[PcsFile]:
+        """Get the pcs file's info by the given absolute `remotepath`"""
+
+        if share_id:
+            return self._shared_path_tree[share_id].search(remotepath=remotepath, share_id=share_id)
+        else:
+            return self._path_tree.search(remotepath=remotepath)
+
+    def paths(self, *remotepaths: str, share_id: str = None) -> List[Optional[PcsFile]]:
+        """Get the pcs files' info by the given absolute `remotepaths`"""
+
+        return [self.path(rp, share_id=share_id) for rp in remotepaths]
+
+    def list_path_iter(
+        self,
+        remotepath: str,
+        file_id: str = None,
+        share_id: str = None,
+        desc: bool = False,
+        name: bool = False,
+        time: bool = False,
+        size: bool = False,
+        all: bool = False,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
+        recursive: bool = False,
+        include_dir: bool = True,
+    ) -> Iterator[PcsFile]:
+        """Iterate the `remotepath`"""
+
+        if not file_id:
+            pf = self.path(remotepath, share_id=share_id)
+            if not pf:
+                return
+            file_id = pf.file_id
+
+        dirname = posix_path_dirname(remotepath)
+
+        for p in self.list_iter(
+            file_id,
+            share_id=share_id,
+            desc=desc,
+            name=name,
+            time=time,
+            size=size,
+            all=all,
+            limit=limit,
+            url_expire_sec=url_expire_sec,
+            recursive=recursive,
+            include_dir=include_dir,
+        ):
+            p.path = join_path(dirname, p.path)
+            yield p
+
+    def list_path(
+        self,
+        remotepath: str,
+        file_id: str = None,
+        share_id: str = None,
+        desc: bool = False,
+        name: bool = False,
+        time: bool = False,
+        size: bool = False,
+        all: bool = False,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
+    ) -> List[PcsFile]:
+        return list(
+            self.list_path_iter(
+                remotepath,
+                file_id=file_id,
+                share_id=share_id,
+                desc=desc,
+                name=name,
+                time=time,
+                size=size,
+                all=all,
+                limit=limit,
+                url_expire_sec=url_expire_sec,
+            )
+        )
+
+    def download_link(self, file_id: str) -> Optional[PcsDownloadUrl]:
+        """Get the download link of the `file_id`"""
+
+        info = self._aliopenpcs.download_link(file_id)
+        return PcsDownloadUrl.from_(info)
+
+    def file_stream(
+        self,
+        file_id: str,
+        max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
+        callback: Callable[..., None] = None,
+        encrypt_password: bytes = b"",
+    ) -> Optional[RangeRequestIO]:
+        """File stream as a normal io"""
+
+        return self._aliopenpcs.file_stream(
+            file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
+        )
+
+
+class AliPCSApiMix(AliPCSApi):
+    def __init__(
+        self,
+        web_refresh_token: str,
+        web_access_token: str = "",
+        web_token_type: str = "",
+        web_expire_time: int = 0,
+        openapi_refresh_token: str = "",
+        openapi_access_token: str = "",
+        openapi_token_type: str = "",
+        openapi_expire_time: int = 0,
+        client_id: str = "",
+        client_secret: str = "",
+        client_server: str = "",
+        user_id: str = "",
+        user_name: str = "",
+        nick_name: str = "",
+        device_id: str = "",
+        default_drive_id: str = "",
+        role: str = "",
+        status: str = "",
+    ):
+        super().__init__(
+            refresh_token=web_refresh_token,
+            access_token=web_access_token,
+            token_type=web_token_type,
+            expire_time=web_expire_time,
+            user_id=user_id,
+            user_name=user_name,
+            nick_name=nick_name,
+            device_id=device_id,
+            default_drive_id=default_drive_id,
+            role=role,
+            status=status,
+        )
+
+        self._aliopenpcsapi: Optional[AliOpenPCSApi] = None
+        if openapi_refresh_token and ((client_id and client_secret) or client_server):
+            self._aliopenpcsapi = AliOpenPCSApi(
+                refresh_token=openapi_refresh_token,
+                access_token=openapi_access_token,
+                token_type=openapi_token_type,
+                expire_time=openapi_expire_time,
+                client_id=client_id,
+                client_secret=client_secret,
+                client_server=client_server,
+                user_id=user_id,
+                user_name=user_name,
+                nick_name=nick_name,
+                default_drive_id=default_drive_id,
+                role=role,
+                status=status,
+            )
+
+    def download_link(self, file_id: str) -> Optional[PcsDownloadUrl]:
+        """Get the download link of the `file_id`"""
+
+        if self._aliopenpcsapi:
+            return self._aliopenpcsapi.download_link(file_id)
+        else:
+            return super().download_link(file_id)
+
+    def file_stream(
+        self,
+        file_id: str,
+        max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
+        callback: Callable[..., None] = None,
+        encrypt_password: bytes = b"",
+    ) -> Optional[RangeRequestIO]:
+        """File stream as a normal io"""
+
+        if self._aliopenpcsapi:
+            return self._aliopenpcsapi.file_stream(
+                file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
+            )
+        else:
+            return super().file_stream(
+                file_id, max_chunk_size=max_chunk_size, callback=callback, encrypt_password=encrypt_password
+            )
+
+    def user_info(self) -> PcsUser:
+        pcs_user = super().user_info()
+
+        if self._aliopenpcsapi:
+            pcs_user.openapi_refresh_token = self._aliopenpcsapi.refresh_token
+            pcs_user.openapi_access_token = self._aliopenpcsapi.access_token
+            pcs_user.openapi_token_type = self._aliopenpcsapi.token_type
+            pcs_user.openapi_expire_time = self._aliopenpcsapi.expire_time
+
+            pcs_user.client_id = self._aliopenpcsapi.client_id
+            pcs_user.client_secret = self._aliopenpcsapi.client_secret
+            pcs_user.client_server = self._aliopenpcsapi.client_server
+
+        return pcs_user
+
+
 class _Node:
     def __init__(self, file_id: str, pcs_file: PcsFile):
         self.file_id = file_id
         self.pcs_file = pcs_file
 
         # Map path basename to node
         self.sub_nodes: Dict[str, _Node] = {}
@@ -761,15 +1120,15 @@
 class PathTree:
     """Path Tree
 
     Invite a file or directory by its path is not supported by aliyundrive.
     This class is aim to support to invite a file or directory by its path.
     """
 
-    def __init__(self, api: AliPCSApi):
+    def __init__(self, api: Union[AliPCSApi, AliOpenPCSApi]):
         self._api = api
         self.root = _Node("root", PcsFile.root())
         self._file_id_to_node: Dict[str, _Node] = {}
         self._file_id_to_node["root"] = self.root
 
     def __str__(self) -> str:
         return f"<PathTree {self.root} >"
@@ -783,34 +1142,30 @@
         """Pop a node from self._file_id_to_node"""
 
         try:
             return self._file_id_to_node.pop(file_id)
         except KeyError:
             return None
 
-    def search(
-        self, remotepath: str = "", topdown: Iterable[str] = [], share_id: str = None
-    ) -> Optional[PcsFile]:
+    def search(self, remotepath: str = "", topdown: Iterable[str] = [], share_id: str = None) -> Optional[PcsFile]:
         """Search the PcsFile which has remote path as `remotepath`
         or has the tree path `topdown`
         """
 
         if not topdown:
             assert remotepath.startswith("/")
             topdown = split_posix_path(remotepath)
 
         node = self._dfs(list(topdown), self.root, share_id=share_id)
         if node:
             return deepcopy(node.pcs_file)
         else:
             return None
 
-    def _dfs(
-        self, topdown: List[str], root: _Node, pull: bool = True, share_id: str = None
-    ) -> Optional[_Node]:
+    def _dfs(self, topdown: List[str], root: _Node, pull: bool = True, share_id: str = None) -> Optional[_Node]:
         """Search a node with the path `topdown` using depth first search"""
 
         if not topdown:
             return root
 
         next_key = topdown[0]
         if next_key == "/":
@@ -831,17 +1186,15 @@
                         break
 
             if next_key not in root.sub_nodes:
                 return None
 
         return self._dfs(topdown[1:], root.sub_nodes[next_key], share_id=share_id)
 
-    def pop(
-        self, remotepath: str = "", topdown: Iterable[str] = []
-    ) -> Optional[PcsFile]:
+    def pop(self, remotepath: str = "", topdown: Iterable[str] = []) -> Optional[PcsFile]:
         """Pop a node which is at the path of `remotepath` or `topdown`"""
 
         if not topdown:
             assert remotepath.startswith("/")
             topdown = split_posix_path(remotepath)
 
         parts = list(topdown)
```

### Comparing `alipcs_py-0.5.3/alipcs_py/alipcs/errors.py` & `alipcs_py-0.6.0/alipcs_py/alipcs/errors.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/alipcs/inner.py` & `alipcs_py-0.6.0/alipcs_py/alipcs/inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, List, Dict, Any, TYPE_CHECKING
 from dataclasses import dataclass
 from collections import namedtuple
 import time
 import re
 
-from alipcs_py.common.date import iso_8601_to_timestamp
+from alipcs_py.common.date import iso_8601_to_timestamp, now_timestamp
 
 if TYPE_CHECKING:
     from alipcs_py.alipcs.api import AliPCSApi
 
 
 @dataclass
 class PcsRapidUploadInfo:
@@ -173,19 +173,24 @@
                 if time.time() < expire_time - 5:
                     return False
         return True
 
     def update_download_url(self, api: "AliPCSApi"):
         """Update the download url if it expires"""
 
-        if self.download_url_expires():
-            pcs_url = api.download_link(self.file_id)
-            if not pcs_url:
-                return
-            self.download_url = pcs_url.url
+        if self.is_file:
+            if self.download_url_expires():
+                pcs_url = api.download_link(self.file_id)
+                if pcs_url:
+                    self.download_url = pcs_url.url
+            else:
+                if getattr(api, "_aliopenpcsapi"):
+                    pcs_url = api.download_link(self.file_id)
+                    if pcs_url:
+                        self.download_url = pcs_url.url
 
 
 @dataclass
 class PcsUploadUrl:
     upload_url: Optional[str] = None
     internal_upload_url: Optional[str] = None
     content_type: Optional[str] = None
@@ -217,17 +222,15 @@
     upload_id: Optional[str] = None
 
     encrypt_mode: Optional[str] = None
     location: Optional[str] = None
 
     @staticmethod
     def from_(info) -> "PcsPreparedFile":
-        part_info_list = [
-            PcsUploadUrl.from_(i) for i in info.get("part_info_list") or []
-        ]
+        part_info_list = [PcsUploadUrl.from_(i) for i in info.get("part_info_list") or []]
         return PcsPreparedFile(
             file_id=info.get("file_id"),
             parent_file_id=info.get("parent_file_id"),
             file_name=info.get("file_name"),
             type=info.get("type"),
             part_info_list=part_info_list,
             rapid_upload=info.get("rapid_upload"),
@@ -243,19 +246,15 @@
         return bool(self.pre_hash)
 
     def is_rapid_upload(self) -> bool:
         return bool(self.rapid_upload)
 
     def upload_urls(self, internal: bool = False) -> List[str]:
         if internal:
-            return [
-                p.internal_upload_url
-                for p in self.part_info_list or []
-                if p.internal_upload_url
-            ]
+            return [p.internal_upload_url for p in self.part_info_list or [] if p.internal_upload_url]
         else:
             return [p.upload_url for p in self.part_info_list or [] if p.upload_url]
 
 
 @dataclass
 class PcsSharedLink:
     """The shared link by the signin user"""
@@ -477,18 +476,27 @@
 @dataclass
 class PcsUser:
     user_id: str
     default_drive_id: Optional[str] = None
     device_id: Optional[str] = None
     domain_id: Optional[str] = None
 
-    refresh_token: Optional[str] = None
-    access_token: Optional[str] = None
-    token_type: Optional[str] = None
-    expire_time: Optional[int] = None
+    web_refresh_token: Optional[str] = None
+    web_access_token: Optional[str] = None
+    web_token_type: Optional[str] = None
+    web_expire_time: Optional[int] = None
+
+    openapi_refresh_token: Optional[str] = None
+    openapi_access_token: Optional[str] = None
+    openapi_token_type: Optional[str] = None
+    openapi_expire_time: Optional[int] = None
+
+    client_id: Optional[str] = None
+    client_secret: Optional[str] = None
+    client_server: Optional[str] = None
 
     user_name: Optional[str] = None
     nick_name: Optional[str] = None
     user_data: Optional[Dict[Any, Any]] = None
     phone: Optional[str] = None
     email: Optional[str] = None
     avatar: Optional[str] = None
@@ -523,17 +531,15 @@
             user_name=info.get("user_name"),
             nick_name=info.get("nick_name"),
             user_data=info.get("user_data"),
             phone=info.get("phone"),
             email=info.get("email"),
             avatar=info.get("avatar"),
             personal_space_info=PcsSpace.from_(info.get("personal_space_info") or {}),
-            personal_rights_info=PcsUserRights.from_(
-                info.get("personal_rights_info") or {}
-            ),
+            personal_rights_info=PcsUserRights.from_(info.get("personal_rights_info") or {}),
             user_vip_info=PcsUserVip.from_(info.get("user_vip_info") or {}),
             created_at=created_at,
             updated_at=updated_at,
             role=info.get("role"),
             status=info.get("status"),
             description=info.get("description"),
             deny_change_password_by_self=info.get("deny_change_password_by_self"),
@@ -576,7 +582,25 @@
             internal_url=info.get("internal_url"),
             cdn_url=info.get("cdn_url"),
             size=info.get("size"),
             method=info.get("method"),
             expiration=expiration,
             ratelimit=PcsRateLimit.from_(info.get("ratelimit") or {}),
         )
+
+
+@dataclass
+class AuthInfo:
+    refresh_token: str
+    access_token: str
+    token_type: str
+    expire_time: int
+
+    @staticmethod
+    def from_(info) -> "AuthInfo":
+        expire_time = now_timestamp() + info.get("expires_in", 7200)
+        return AuthInfo(
+            refresh_token=info.get("refresh_token"),
+            access_token=info.get("access_token"),
+            token_type=info.get("token_type"),
+            expire_time=expire_time,
+        )
```

### Comparing `alipcs_py-0.5.3/alipcs_py/alipcs/pcs.py` & `alipcs_py-0.6.0/alipcs_py/alipcs/pcs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 from typing import Optional, Dict, List, Union, Any, Callable, IO
 from enum import Enum
-import math
-import time
 import threading
+from urllib.parse import urljoin
 from typing_extensions import Literal
 
 import requests  # type: ignore
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
-from alipcs_py.common.date import (
-    now_timestamp,
-    iso_8601_to_timestamp,
-    timestamp_to_iso_8601,
-)
+from alipcs_py.common.date import now_timestamp, iso_8601_to_timestamp, timestamp_to_iso_8601
 from alipcs_py.common import constant
-from alipcs_py.common.io import (
-    RangeRequestIO,
-    DEFAULT_MAX_CHUNK_SIZE,
-    ChunkIO,
-    total_len,
-)
+from alipcs_py.common.io import RangeRequestIO, DEFAULT_MAX_CHUNK_SIZE, ChunkIO, total_len
 from alipcs_py.common.cache import timeout_cache
 from alipcs_py.common.crypto import generate_secp256k1_keys
 from alipcs_py.alipcs.errors import AliPCSError, parse_error, handle_error
 from alipcs_py.alipcs.errors import assert_ok
 from alipcs_py.alipcs.inner import SharedAuth
 
 
 UPLOAD_CHUNK_SIZE = 10 * constant.OneM
 
 APP_ID = "5dde4e1bdf9e4966b387ba58f4b3fdc3"
 
-PCS_BAIDU_COM = "https://api.aliyundrive.com"
-# PCS_BAIDU_COM = 'http://127.0.0.1:8888'
+ALIYUNDRIVE_COM = "https://www.aliyundrive.com"
+ALIYUNDRIVE_COM_API = "https://api.aliyundrive.com"
+ALIYUNDRIVE_OPENAPI_DOMAIN = "https://openapi.aliyundrive.com"
 
-PCS_UA = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/77.0.3865.75 Safari/537.36"
-PCS_HEADERS = {"User-Agent": PCS_UA}
+PCS_UA = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
+PCS_HEADERS = {"Origin": ALIYUNDRIVE_COM[:-1], "Referer": ALIYUNDRIVE_COM + "/", "User-Agent": PCS_UA}
 
 CheckNameMode = Literal[
     "overwrite",  # 直接覆盖，以后多版本有用
     "auto_rename",  # 自动换一个随机名称
     "refuse",  # 不会创建，告诉你已经存在
     "ignore",  # 会创建重名的
 ]
@@ -48,15 +39,15 @@
 class Method(Enum):
     Head = "HEAD"
     Get = "GET"
     Post = "POST"
 
 
 class PcsNode(Enum):
-    f"""PCS Nodes which use {PCS_BAIDU_COM}"""
+    f"""Aliyundrive PCS Nodes which use {ALIYUNDRIVE_COM_API}"""
 
     Token = "v2/account/token"
     Refresh = "token/refresh"
     CreateSession = "users/v1/users/device/create_session"
 
     FileList = "adrive/v3/file/list"
     Meta = "v2/file/get"
@@ -81,15 +72,15 @@
     SharedFileDownloadUrl = "v2/file/get_share_link_download_url"
 
     PersonalInfo = "v2/databox/get_personal_info"
     User = "v2/user/get"
     UserVip = "business/v1.0/users/vip/info"
 
     def url(self) -> str:
-        return f"{PCS_BAIDU_COM}/{self.value}"
+        return f"{ALIYUNDRIVE_COM_API}/{self.value}"
 
 
 # The Lock is used to refresh token
 _LOCK = threading.Lock()
 
 
 class AliPCS:
@@ -97,50 +88,52 @@
 
     SHARE_AUTHS: Dict[str, SharedAuth] = {}
 
     def __init__(
         self,
         refresh_token: str,
         access_token: str = "",
+        token_type: str = "Bearer",
         expire_time: int = 0,
         user_id: str = "",
         user_name: str = "",
         nick_name: str = "",
-        token_type: str = "",
         device_id: str = "",
         default_drive_id: str = "",
         role: str = "",
         status: str = "",
     ):
         self._session = requests.Session()
         self._refresh_token = refresh_token
         self._access_token = access_token
+        self._token_type = token_type
         self._expire_time = expire_time
 
         self._user_id = user_id
         self._user_name = user_name
         self._nick_name = nick_name
-        self._token_type = token_type
         self._device_id = device_id
         self._signature = ""
         self._default_drive_id = default_drive_id
         self._role = role
         self._status = status
         self._nonce = 0
 
     def __str__(self) -> str:
         return f"""AliPCS
 
     user_id: {self.user_id}
     user_name: {self.user_name}
     nick_name: {self.nick_name}
+
     refresh_token: {self.refresh_token}
     access_token: {self.access_token}
     token_type: {self.token_type}
     expire_time: {self.expire_time}
+
     device_id: {self.device_id}
     signature: {self.signature}
     default_drive_id: {self.default_drive_id}
     role: {self.role}
     status: {self.status}
     nonce: {self._nonce}
     """
@@ -152,19 +145,15 @@
         data = dict(refresh_token=self.refresh_token, grant_type="refresh_token")
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     @property
     def refresh_token(self) -> str:
         with _LOCK:
-            if (
-                not self._access_token
-                or (now_timestamp() - 1 * 60 * 60) >= self._expire_time
-                or not self._device_id
-            ):
+            if not self._access_token or (now_timestamp() - 1 * 60 * 60) >= self._expire_time or not self._device_id:
                 self.refresh()
             return self._refresh_token
 
     @property
     def access_token(self) -> str:
         self.refresh_token
         return self._access_token
@@ -233,31 +222,27 @@
         **kwargs,
     ) -> requests.Response:
         if not headers:
             headers = dict(PCS_HEADERS)
 
         if not refresh and "Authorization" not in headers:
             headers["Authorization"] = f"{self.token_type} {self.access_token}"
+            headers["x-device-id"] = self.device_id
 
         if json is not None:
             headers["Content-Type"] = "application/json;charset=UTF-8"
 
         if isinstance(data, (MultipartEncoder, MultipartEncoderMonitor)):
             headers["Content-Type"] = data.content_type
 
+        headers["x-canary"] = "client=web,app=adrive,version=v4.1.0"
+
         try:
             resp = self._session.request(
-                method.value,
-                url,
-                params=params,
-                headers=headers,
-                data=data,
-                json=json,
-                files=files,
-                **kwargs,
+                method.value, url, params=params, headers=headers, data=data, json=json, files=files, **kwargs
             )
             return resp
         except Exception as err:
             raise AliPCSError("AliPCS._request", cause=err)
 
     def refresh(self):
         """Refresh token"""
@@ -300,29 +285,29 @@
 
         private_key, public_key = generate_secp256k1_keys()
         message = f"{APP_ID}:{device_id}:{user_id}:{nonce}".encode()
         signature: str = private_key.sign(message).hex()
         sign = signature + "00"
 
         url = PcsNode.CreateSession.url()
-        data = dict(
-            deviceName="Chrome浏览器",
-            modelName="Windows网页版",
-            pubKey=public_key.to_string().hex(),
-        )
+        data = dict(deviceName="Chrome浏览器", modelName="Mac OS网页版", pubKey=public_key.to_string().hex())
 
         headers = dict(**PCS_HEADERS)
         headers.update({"x-device-id": device_id, "x-signature": sign})
 
-        resp = self._request(Method.Post, url, headers=headers, json=data)
-        info = resp.json()
+        @handle_error
+        def do(self):
+            resp = self._request(Method.Post, url, headers=headers, json=data)
+            return resp.json()
+
+        info = do(self)
         if info["result"] and info["success"]:
             self._signature = sign
 
-        return resp.json()
+        return info
 
     def meta(self, *file_ids: str, share_id: str = None):
         assert "root" not in file_ids, '"root" has NOT meta info'
 
         headers = dict(PCS_HEADERS)
         headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
 
@@ -333,17 +318,17 @@
             headers["x-share-token"] = share_token
 
         responses = []
         for file_id in file_ids:
             data = dict(
                 file_id=file_id,
                 fields="*",
-                # image_thumbnail_process="image/resize,w_400/format,jpeg",
-                # image_url_process="image/resize,w_375/format,jpeg",
-                # video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_375",
+                image_thumbnail_process="image/resize,w_400/format,jpeg",
+                image_url_process="image/resize,w_375/format,jpeg",
+                video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_375",
             )
 
             if share_id:
                 data["share_id"] = share_id
             else:
                 data["drive_id"] = self.default_drive_id
 
@@ -392,22 +377,22 @@
             return False
 
     @assert_ok
     @handle_error
     def list(
         self,
         file_id: str,
-        share_id: str = None,
+        share_id: str = "",
         desc: bool = False,
         name: bool = False,
         time: bool = False,
         size: bool = False,
         all: bool = False,
-        limit: int = 100,
-        url_expire_sec: int = 7200,
+        limit: int = 200,
+        url_expire_sec: int = 14400,
         next_marker: str = "",
     ):
         """List files at the directory which has `file_id`
 
         Args:
             file_id (str):
                 The file_id of the directory
@@ -429,21 +414,24 @@
             drive_id=self.default_drive_id,
             fields="*",
             limit=limit,
             order_by=orderby,
             order_direction="DESC" if desc else "ASC",
             parent_file_id=file_id,
             url_expire_sec=url_expire_sec,
-            marker=next_marker,
-            # image_thumbnail_process="image/resize,w_400/format,jpeg",
-            # image_url_process="image/resize,w_1920/format,jpeg",
-            # video_thumbnail_process="video/snapshot,t_0,f_jpg,ar_auto,w_300",
+            image_thumbnail_process="image/resize,w_256/format,jpeg",
+            image_url_process="image/resize,w_1920/format,jpeg/interlace,1",
+            video_thumbnail_process="video/snapshot,t_1000,f_jpg,ar_auto,w_256",
         )
 
+        if next_marker:
+            data["marker"] = next_marker
+
         headers = dict(PCS_HEADERS)
+        headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
         if share_id:
             share_token = self.share_token(share_id)
             assert share_token, "Need share_token"
 
             data["share_id"] = share_id
             data.pop("drive_id")
             headers["x-share-token"] = share_token
@@ -505,47 +493,29 @@
             proof_code=proof_code,
             proof_version="v1",
         )
 
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
-    def prepare_file(
-        self,
-        filename: str,
-        dir_id: str,
-        size: int,
-        pre_hash: str = "",
-        part_number: int = 1,
-    ):
-        return self.create_file(
-            filename, dir_id, size, pre_hash=pre_hash, part_number=part_number
-        )
+    def prepare_file(self, filename: str, dir_id: str, size: int, pre_hash: str = "", part_number: int = 1):
+        return self.create_file(filename, dir_id, size, pre_hash=pre_hash, part_number=part_number)
 
     @assert_ok
     @handle_error
-    def rapid_upload_file(
-        self, filename: str, dir_id: str, size: int, content_hash: str, proof_code: str
-    ):
+    def rapid_upload_file(self, filename: str, dir_id: str, size: int, content_hash: str, proof_code: str):
         """Rapid Upload File
 
         size (int): the length of total content.
         content_hash (str): the sha1 of total content.
         """
 
-        return self.create_file(
-            filename, dir_id, size, content_hash=content_hash, proof_code=proof_code
-        )
+        return self.create_file(filename, dir_id, size, content_hash=content_hash, proof_code=proof_code)
 
-    def upload_slice(
-        self,
-        io: IO,
-        url: str,
-        callback: Callable[[MultipartEncoderMonitor], None] = None,
-    ) -> None:
+    def upload_slice(self, io: IO, url: str, callback: Callable[[MultipartEncoderMonitor], None] = None) -> None:
         """Upload the content of io to remote url"""
 
         cio = ChunkIO(io, total_len(io))
         monitor = MultipartEncoderMonitor(cio, callback=callback)
 
         session = requests.Session()
         session.request(
@@ -556,19 +526,15 @@
             # timeout=(3, 9),  # (connect timeout, read timeout)
         )
 
     @assert_ok
     @handle_error
     def upload_complete(self, file_id: str, upload_id: str):
         url = PcsNode.UploadComplete.url()
-        data = dict(
-            drive_id=self.default_drive_id,
-            file_id=file_id,
-            upload_id=upload_id,
-        )
+        data = dict(drive_id=self.default_drive_id, file_id=file_id, upload_id=upload_id)
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     @assert_ok
     @handle_error
     def search(
         self,
@@ -595,17 +561,17 @@
         data = dict(
             all=all,
             drive_id=self.default_drive_id,
             limit=limit,
             order_by=orderby + " " + ("DESC" if desc else "ASC"),
             query=f'name match "{keyword}"',
             marker=next_marker,
-            # image_thumbnail_process="image/resize,w_160/format,jpeg",
-            # image_url_process="image/resize,w_1920/format,jpeg",
-            # video_thumbnail_process="video/snapshot,t_0,f_jpg,ar_auto,w_300",
+            image_thumbnail_process="image/resize,w_160/format,jpeg",
+            image_url_process="image/resize,w_1920/format,jpeg",
+            video_thumbnail_process="video/snapshot,t_0,f_jpg,ar_auto,w_300",
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     @assert_ok
     @handle_error
     def makedir(self, dir_id: str, name: str):
@@ -619,18 +585,15 @@
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     @assert_ok
     @handle_error
     def batch_operate(
-        self,
-        requests_: List[Dict[str, Any]],
-        resource: str = "file",
-        headers: Optional[Dict[str, str]] = None,
+        self, requests_: List[Dict[str, Any]], resource: str = "file", headers: Optional[Dict[str, str]] = None
     ):
         url = PcsNode.Batch.url()
         data = dict(resource=resource, requests=requests_)
         resp = self._request(Method.Post, url, headers=headers, json=data)
         return resp.json()
 
     def move(self, *file_ids: str):
@@ -668,18 +631,15 @@
     @assert_ok
     @handle_error
     def rename(self, file_id: str, name: str):
         """Rename the file to `name`"""
 
         url = PcsNode.Update.url()
         data = dict(
-            check_name_mode="refuse",  # or "auto_rename"
-            drive_id=self.default_drive_id,
-            file_id=file_id,
-            name=name,
+            check_name_mode="refuse", drive_id=self.default_drive_id, file_id=file_id, name=name  # or "auto_rename"
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     def copy(self, *file_ids: str):
         assert len(file_ids) > 1
 
@@ -706,18 +666,15 @@
         requests_ = []
         for file_id in file_ids:
             req = dict(
                 method="POST",
                 url="/recyclebin/trash",
                 id=file_id,
                 headers={"Content-Type": "application/json"},
-                body=dict(
-                    drive_id=self.default_drive_id,
-                    file_id=file_id,
-                ),
+                body=dict(drive_id=self.default_drive_id, file_id=file_id),
             )
             requests_.append(req)
         return self.batch_operate(requests_, resource="file")
 
     @assert_ok
     @handle_error
     def check_available(self, file_ids: str):
@@ -729,25 +686,23 @@
             file_id_list=list(file_ids),
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     @assert_ok
     @handle_error
-    def share(
-        self, *file_ids: str, password: str = "", period: int = 0, description: str = ""
-    ):
+    def share(self, *file_ids: str, password: str = "", period: int = 0, description: str = ""):
         """Share `remotepaths` to public
 
         period (int): The days for expiring. `0` means no expiring
         """
 
         expiration = ""  # Living forever
         if period > 0:
-            expiration = timestamp_to_iso_8601(int(time.time()) + period * 24 * 60 * 60)
+            expiration = timestamp_to_iso_8601(now_timestamp() + period * 24 * 60 * 60)
 
         url = PcsNode.Share.url()
         data = dict(
             drive_id=self.default_drive_id,
             expiration=expiration,
             file_id_list=list(file_ids),
             share_pwd=password,
@@ -776,17 +731,15 @@
         requests_ = []
         for share_id in share_ids:
             req = dict(
                 method="POST",
                 url="/share_link/cancel",
                 id=share_id,
                 headers={"Content-Type": "application/json"},
-                body=dict(
-                    share_id=share_id,
-                ),
+                body=dict(share_id=share_id),
             )
             requests_.append(req)
 
         return self.batch_operate(requests_, resource="file")
 
     @assert_ok
     @handle_error
@@ -801,17 +754,15 @@
         url = PcsNode.ShareToken.url()
         data = dict(share_id=share_id, share_pwd=share_password)
         resp = self._request(Method.Post, url, json=data)
 
         info = resp.json()
         if info.get("share_token"):
             # Store share password for refreshing share token
-            self.__class__.SHARE_AUTHS[share_id] = SharedAuth.from_(
-                share_id, share_password, info
-            )
+            self.__class__.SHARE_AUTHS[share_id] = SharedAuth.from_(share_id, share_password, info)
 
         return info
 
     def share_token(self, share_id: str) -> str:
         self.get_share_token(share_id)
 
         shared_auth = self.__class__.SHARE_AUTHS[share_id]
@@ -830,19 +781,15 @@
         info["share_id"] = share_id
         return info
 
     # list_shared_files is an alias of list
     list_shared_files = list
 
     def transfer_shared_files(
-        self,
-        shared_file_ids: List[str],
-        dest_id: str,
-        share_id: str,
-        auto_rename: bool = False,
+        self, shared_file_ids: List[str], dest_id: str, share_id: str, auto_rename: bool = False
     ):
         """Transfer shared files to destination directory"""
 
         requests_ = []
         for file_id in shared_file_ids:
             req = dict(
                 method="POST",
@@ -865,67 +812,51 @@
         headers = dict(PCS_HEADERS)
         headers["x-share-token"] = share_token
 
         return self.batch_operate(requests_, resource="file", headers=headers)
 
     @assert_ok
     @handle_error
-    def _get_shared_file_download_url(
-        self,
-        shared_file_id: str,
-        share_id: str,
-        expire_duration: int = 10 * 60,
-    ):
+    def _get_shared_file_download_url(self, shared_file_id: str, share_id: str, expire_duration: int = 10 * 60):
         url = PcsNode.SharedFileDownloadUrl.url()
-        data = dict(
-            expire_sec=expire_duration,
-            file_id=shared_file_id,
-            share_id=share_id,
-        )
+        data = dict(expire_sec=expire_duration, file_id=shared_file_id, share_id=share_id)
 
         share_token = self.share_token(share_id)
         assert share_token, "Need share_token"
 
         headers = dict(PCS_HEADERS)
         headers["x-share-token"] = share_token
 
         resp = self._request(Method.Post, url, headers=headers, json=data)
         return resp.json()
 
-    def shared_file_download_url(
-        self,
-        shared_file_id: str,
-        share_id: str,
-        expire_duration: int = 10 * 60,
-    ) -> str:
-        info = self._get_shared_file_download_url(
-            shared_file_id,
-            share_id,
-            expire_duration=expire_duration,
-        )
+    def shared_file_download_url(self, shared_file_id: str, share_id: str, expire_duration: int = 10 * 60) -> str:
+        info = self._get_shared_file_download_url(shared_file_id, share_id, expire_duration=expire_duration)
         url = info["url"]
 
         headers = dict(PCS_HEADERS)
         headers["Referer"] = "https://www.aliyundrive.com/"
         resp = requests.get(url, headers=headers, allow_redirects=False)
         return resp.headers["Location"]
 
     @assert_ok
     @handle_error
     def user_info(self):
-        url = PcsNode.PersonalInfo.url()
+        url = PcsNode.User.url()
         resp = self._request(Method.Post, url, json={})
         info1 = resp.json()
 
-        url = PcsNode.User.url()
-        resp = self._request(Method.Post, url, json={})
+        headers = dict(PCS_HEADERS)
+        headers.update({"x-device-id": self.device_id, "x-signature": self.signature})
+        url = PcsNode.PersonalInfo.url()
+        resp = self._request(Method.Post, url, headers=headers, json={})
         info2 = resp.json()
 
         url = PcsNode.UserVip.url()
-        resp = self._request(Method.Post, url, json={})
+        resp = self._request(Method.Post, url, headers=headers, json={})
         info3 = resp.json()
 
         return {**info1, **info2, "user_vip_info": info3}
 
     @timeout_cache(1 * 60 * 60)  # 1 hour timeout
     @assert_ok
     @handle_error
@@ -968,20 +899,413 @@
         shared_file_id: str,
         share_id: str,
         expire_duration: int = 10 * 60,
         max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
         callback: Callable[..., None] = None,
         encrypt_password: bytes = b"",
     ) -> Optional[RangeRequestIO]:
-        url = self.shared_file_download_url(
-            shared_file_id,
-            share_id,
-            expire_duration=expire_duration,
+        url = self.shared_file_download_url(shared_file_id, share_id, expire_duration=expire_duration)
+
+        headers = {
+            "User-Agent": PCS_UA,
+            "Connection": "Keep-Alive",
+            "Referer": "https://www.aliyundrive.com/",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,zh-TW;q=0.6",
+        }
+        return RangeRequestIO(
+            Method.Get.value,
+            url,
+            headers=headers,
+            max_chunk_size=max_chunk_size,
+            callback=callback,
+            encrypt_password=encrypt_password,
         )
 
+
+class OpenPcsNode(Enum):
+    f"""PCS Nodes which use {ALIYUNDRIVE_OPENAPI_DOMAIN}"""
+
+    UpdateRefreshToken = "oauth/access_token"
+    QrcodeLink = "oauth/authorize/qrcode"
+    QrcodeUrl = "o/oauth/authorize?sid={sid}"
+    QrcodeStatus = "oauth/qrcode/{sid}/status"
+
+    Token = "v2/account/token"
+    CreateSession = "users/v1/users/device/create_session"
+    DriveInfo = "adrive/v1.0/user/getDriveInfo"
+
+    Meta = "adrive/v1.0/openFile/get"
+    FileList = "adrive/v1.0/openFile/list"
+    Search = "adrive/v3/file/search"
+    DownloadUrl = "adrive/v1.0/openFile/getDownloadUrl"
+
+    CreateFile = "v2/file/create"
+    UploadComplete = "v2/file/complete"
+
+    Batch = "v3/batch"
+
+    CreateWithFolders = "adrive/v2/file/createWithFolders"
+    Move = "adrive/v3/file/move"
+    Update = "v3/file/update"
+    Trash = "v2/recyclebin/trash"
+
+    Available = "adrive/v2/share_link/check_avaliable"
+    Share = "adrive/v2/share_link/create"
+    ShareToken = "v2/share_link/get_share_token"
+    SharedInfo = "adrive/v3/share_link/get_share_by_anonymous"
+    SharedList = "adrive/v3/share_link/list"
+    SharedFileDownloadUrl = "v2/file/get_share_link_download_url"
+
+    SpaceInfo = "adrive/v1.0/user/getSpaceInfo"
+    # PersonalInfo = "v2/databox/get_personal_info"
+    PersonalInfo = "adrive/v1.0/user/get"
+    User = "v2/user/get"
+    UserVip = "adrive/v1.0/user/getVipInfo"
+
+    def url(self) -> str:
+        return f"{ALIYUNDRIVE_OPENAPI_DOMAIN}/{self.value}"
+
+
+class AliOpenPCS:
+    """`Aliyundrive Open PCS` provides pcs's apis which return raw json"""
+
+    SHARE_AUTHS: Dict[str, SharedAuth] = {}
+
+    def __init__(
+        self,
+        refresh_token: str,
+        access_token: str = "",
+        token_type: str = "Bearer",
+        expire_time: int = 0,
+        client_id: str = "",
+        client_secret: str = "",
+        client_server: str = "",
+        user_id: str = "",
+        user_name: str = "",
+        nick_name: str = "",
+        default_drive_id: str = "",
+        role: str = "",
+        status: str = "",
+    ):
+        assert (
+            client_id and client_secret
+        ) or client_server, "(client_id and client_secret) or client_server must be set"
+
+        self._session = requests.Session()
+
+        self._refresh_token = refresh_token
+        self._access_token = access_token
+        self._token_type = token_type
+        self._expire_time = expire_time
+
+        self._client_id = client_id
+        self._client_secret = client_secret
+        self._client_server = client_server
+
+        self._user_id = user_id
+        self._user_name = user_name
+        self._nick_name = nick_name
+        self._default_drive_id = default_drive_id
+        self._role = role
+        self._status = status
+        self._nonce = 0
+
+    def __str__(self) -> str:
+        return f"""AliPCS
+
+    user_id: {self.user_id}
+    user_name: {self.user_name}
+    nick_name: {self.nick_name}
+
+    refresh_token: {self.refresh_token}
+    access_token: {self.access_token}
+    token_type: {self.token_type}
+    expire_time: {self.expire_time}
+
+    client_id: {self._client_id}
+    client_secret: {self._client_secret}
+    client_server: {self._client_server}
+
+    default_drive_id: {self.default_drive_id}
+    role: {self.role}
+    status: {self.status}
+    nonce: {self._nonce}
+    """
+
+    @property
+    def refresh_token(self) -> str:
+        now = now_timestamp()
+        if self._expire_time - now < 200 or not self._access_token:
+            self._update_refresh_token()
+
+        if not self._default_drive_id:
+            self._get_drive_info()
+
+        return self._refresh_token
+
+    @property
+    def access_token(self) -> str:
+        self.refresh_token
+        return self._access_token
+
+    @property
+    def client_id(self) -> str:
+        return self._client_id
+
+    @property
+    def client_secret(self) -> str:
+        return self._client_secret
+
+    @property
+    def client_server(self) -> str:
+        return self._client_server
+
+    @property
+    def user_id(self) -> str:
+        self.refresh_token
+        return self._user_id
+
+    @property
+    def user_name(self) -> str:
+        self.refresh_token
+        return self._user_name
+
+    @property
+    def nick_name(self) -> str:
+        self.refresh_token
+        return self._nick_name
+
+    @property
+    def token_type(self) -> str:
+        self.refresh_token
+        return self._token_type
+
+    @property
+    def expire_time(self) -> int:
+        self.refresh_token
+        return self._expire_time
+
+    @property
+    def default_drive_id(self) -> str:
+        self.refresh_token
+        return self._default_drive_id
+
+    @property
+    def role(self) -> str:
+        self.refresh_token
+        return self._role
+
+    @property
+    def status(self) -> str:
+        self.refresh_token
+        return self._status
+
+    def _request(
+        self,
+        method: Method,
+        url: str,
+        params: Optional[Dict[str, str]] = None,
+        headers: Optional[Dict[str, str]] = None,
+        data: Union[str, bytes, Dict[str, str], Any] = None,
+        json: Any = None,
+        files: Optional[Dict[str, Any]] = None,
+        refresh: bool = False,
+        **kwargs,
+    ) -> requests.Response:
+        if not headers:
+            headers = dict(PCS_HEADERS)
+
+        if not refresh and "Authorization" not in headers:
+            headers["Authorization"] = f"{self._token_type} {self._access_token}"
+
+        if json is not None:
+            headers["Content-Type"] = "application/json;charset=UTF-8"
+
+        if isinstance(data, (MultipartEncoder, MultipartEncoderMonitor)):
+            headers["Content-Type"] = data.content_type
+
+        try:
+            resp = self._session.request(
+                method.value, url, params=params, headers=headers, data=data, json=json, files=files, **kwargs
+            )
+            return resp
+        except Exception as err:
+            raise AliPCSError("AliPCS._request", cause=err)
+
+    def _update_refresh_token(self):
+        """Update refresh token"""
+
+        data = dict(refresh_token=self._refresh_token, grant_type="refresh_token")
+        if self._client_id and self._client_secret:
+            url = OpenPcsNode.UpdateRefreshToken.url()
+            data["client_id"] = self._client_id
+            data["client_secret"] = self._client_secret
+        else:
+            url = urljoin(self._client_server, OpenPcsNode.UpdateRefreshToken.value)
+
+        resp = self._request(Method.Post, url, json=data, refresh=True)
+        info = resp.json()
+
+        if "code" in info:
+            err = parse_error(info["code"], info=info)
+            raise err
+
+        self._refresh_token = info["refresh_token"]
+        self._access_token = info["access_token"]
+        self._token_type = info["token_type"]
+        self._expire_time = now_timestamp() + info["expires_in"]
+
+        return info
+
+    def _get_drive_info(self):
+        """Get drive info"""
+
+        url = OpenPcsNode.DriveInfo.url()
+        data = dict()
+
+        resp = self._request(Method.Post, url, json=data)
+        info = resp.json()
+
+        if "code" in info:
+            err = parse_error(info["code"], info=info)
+            raise err
+
+        self._user_id = info["user_id"]
+        self._user_name = info["user_name"]
+        self._nick_name = info["nick_name"]
+        self._default_drive_id = info["default_drive_id"]
+        self._domain_id = info["domain_id"]
+        self._role = info["role"]
+        self._status = info["status"]
+
+        return info
+
+    def meta(self, *file_ids: str, share_id: str = None):
+        assert "root" not in file_ids, '"root" has NOT meta info'
+
+        responses = []
+        for file_id in file_ids:
+            data = dict(file_id=file_id, drive_id=self.default_drive_id)
+            url = PcsNode.Meta.url()
+            resp = self._request(Method.Post, url, json=data)
+            info = resp.json()
+            responses.append(dict(body=info))
+
+        return dict(responses=responses)
+
+    def exists(self, file_id: str) -> bool:
+        if file_id == "root":
+            return True
+
+        r = self.meta(file_id)
+        info = r["responses"][0]["body"]
+        if info.get("code") == "NotFound.File":
+            return False
+        else:
+            return True
+
+    def is_file(self, file_id: str) -> bool:
+        if file_id == "root":
+            return False
+
+        r = self.meta(file_id)
+        info = r["responses"][0]["body"]
+        if info.get("code") == "NotFound.File":
+            return False
+        if info["type"] == "file":
+            return True
+        else:
+            return False
+
+    def is_dir(self, file_id: str) -> bool:
+        if file_id == "root":
+            return True
+
+        r = self.meta(file_id)
+        info = r["responses"][0]["body"]
+        if info.get("code") == "NotFound.File":
+            return False
+        if info["type"] == "folder":
+            return True
+        else:
+            return False
+
+    @assert_ok
+    @handle_error
+    def list(
+        self,
+        file_id: str,
+        share_id: str = None,
+        desc: bool = False,
+        name: bool = False,
+        time: bool = False,
+        size: bool = False,
+        all: bool = False,
+        limit: int = 200,
+        url_expire_sec: int = 14200,
+        next_marker: str = "",
+    ):
+        """List files at the directory which has `file_id`
+
+        Args:
+            file_id (str):
+                The file_id of the directory
+        """
+
+        assert limit <= 200, "`limit` should be less than 200"
+
+        url = PcsNode.FileList.url()
+        orderby = "name"
+        if name:
+            orderby = "name"
+        elif time:
+            orderby = "updated_at"  # "created_at"  # 服务器最后修改时间
+        elif size:
+            orderby = "size"
+
+        data = dict(
+            all=all,
+            drive_id=self.default_drive_id,
+            fields="*",
+            limit=limit,
+            order_by=orderby,
+            order_direction="DESC" if desc else "ASC",
+            parent_file_id=file_id,
+            url_expire_sec=url_expire_sec,
+            marker=next_marker,
+        )
+
+        headers = dict(PCS_HEADERS)
+        resp = self._request(Method.Post, url, headers=headers, json=data)
+        return resp.json()
+
+    @staticmethod
+    def part_info_list(part_number: int) -> List[Dict[str, int]]:
+        return [dict(part_number=i) for i in range(1, part_number + 1)]
+
+    @timeout_cache(4 * 60 * 60)  # 4 hour timeout
+    @assert_ok
+    @handle_error
+    def download_link(self, file_id: str):
+        url = OpenPcsNode.DownloadUrl.url()
+        data = dict(drive_id=self.default_drive_id, file_id=file_id, expire_sec=14400)
+        resp = self._request(Method.Post, url, json=data)
+        return resp.json()
+
+    def file_stream(
+        self,
+        file_id: str,
+        max_chunk_size: int = DEFAULT_MAX_CHUNK_SIZE,
+        callback: Callable[..., None] = None,
+        encrypt_password: bytes = b"",
+    ) -> Optional[RangeRequestIO]:
+        info = self.download_link(file_id)
+        url = info["url"]
+
         headers = {
             "User-Agent": PCS_UA,
             "Connection": "Keep-Alive",
             "Referer": "https://www.aliyundrive.com/",
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-US,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,zh-TW;q=0.6",
         }
@@ -989,7 +1313,88 @@
             Method.Get.value,
             url,
             headers=headers,
             max_chunk_size=max_chunk_size,
             callback=callback,
             encrypt_password=encrypt_password,
         )
+
+
+class AliOpenAuth:
+    def __init__(self, client_id: str = "", client_secret: str = "", client_server: str = ""):
+        assert (
+            client_id and client_secret
+        ) or client_server, "(client_id and client_secret) or client_server must be set"
+
+        self._session = requests.Session()
+
+        self._client_id = client_id
+        self._client_secret = client_secret
+        self._client_server = client_server
+
+    def _request(
+        self,
+        method: Method,
+        url: str,
+        params: Optional[Dict[str, str]] = None,
+        headers: Optional[Dict[str, str]] = None,
+        data: Union[str, bytes, Dict[str, str], Any] = None,
+        json: Any = None,
+        files: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ) -> requests.Response:
+        if not headers:
+            headers = dict(PCS_HEADERS)
+
+        try:
+            resp = self._session.request(
+                method.value, url, params=params, headers=headers, data=data, json=json, files=files, **kwargs
+            )
+            return resp
+        except Exception as err:
+            raise AliPCSError("AliOpenAuth._request", cause=err)
+
+    @staticmethod
+    def qrcode_url(sid: str) -> str:
+        return OpenPcsNode.QrcodeUrl.url().format(sid)
+
+    @handle_error
+    def get_qrcode_info(self):
+        data: Dict[str, Any] = dict(
+            scopes=[
+                "user:base",
+                "file:all:read",
+                "file:all:write",
+            ],
+            width=None,
+            height=None,
+        )
+
+        if self._client_server:
+            url = self._client_server.strip("/") + "/" + OpenPcsNode.QrcodeLink.value
+        else:
+            data["client_id"] = self._client_id
+            data["client_secret"] = self._client_secret
+            url = OpenPcsNode.QrcodeLink.url()
+
+        resp = self._request(Method.Post, url, json=data)
+        return resp.json()
+
+    @handle_error
+    def scan_status(self, sid: str):
+        url = OpenPcsNode.QrcodeStatus.url().format(sid=sid)
+        resp = self._request(Method.Get, url)
+        return resp.json()
+
+    @handle_error
+    def get_refresh_token(self, auth_code: str):
+        data = dict(grant_type="authorization_code", code=auth_code)
+
+        if self._client_server:
+            url = self._client_server.strip("/") + "/" + OpenPcsNode.UpdateRefreshToken.value
+        else:
+            data["client_id"] = self._client_id
+            data["client_secret"] = self._client_secret
+            url = OpenPcsNode.UpdateRefreshToken.url()
+
+        resp = self._request(Method.Post, url, json=data)
+        return resp.json()
```

### Comparing `alipcs_py-0.5.3/alipcs_py/alipcs/phone.py` & `alipcs_py-0.6.0/alipcs_py/alipcs/phone.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/alipcs/tree.py` & `alipcs_py-0.6.0/alipcs_py/alipcs/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
 
 class PathTree:
     def __init__(self, api: AliPCSApi):
         self._api = api
         self.root = _Node("root", PcsFile.root())
 
-    def search(
-        self, remotepath: str = "", topdown: Iterable[str] = [], root: _Node = None
-    ) -> Optional[PcsFile]:
+    def search(self, remotepath: str = "", topdown: Iterable[str] = [], root: _Node = None) -> Optional[PcsFile]:
         if not topdown:
             assert remotepath.startswith("/")
             topdown = split_posix_path(remotepath)
 
         root = root or self.root
         return self._dfs(list(topdown), root)
```

### Comparing `alipcs_py-0.5.3/alipcs_py/app/app.py` & `alipcs_py-0.6.0/alipcs_py/app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Optional, List, Tuple, Union
+from typing import Optional, List, Dict, Tuple, Union, final
 import os
 
+
 # Enable UTF-8 Mode for Windows
 # https://www.python.org/dev/peps/pep-0540/
 if os.name == "nt":
     os.environ["PYTHONUTF8"] = "1"
 
 from collections import OrderedDict
 from functools import wraps
@@ -15,20 +16,21 @@
 import logging
 import traceback
 
 from alipcs_py import __version__
 from alipcs_py.alipcs import AliPCSApi, AliPCSError
 from alipcs_py.app import account as account_module
 from alipcs_py.app.account import Account, AccountManager
-from alipcs_py.commands.env import CONFIG_PATH, ACCOUNT_DATA_PATH, SHARED_STORE_PATH
 from alipcs_py.common.progress_bar import _progress, init_progress_bar
 from alipcs_py.common.path import join_path
 from alipcs_py.common.net import random_avail_port
 from alipcs_py.common.io import EncryptType
 from alipcs_py.common.event import keyboard_listener_start
+from alipcs_py.commands.login import openapi_qrcode_login
+from alipcs_py.commands.env import CONFIG_PATH, ACCOUNT_DATA_PATH
 from alipcs_py.commands.sifter import (
     IncludeSifter,
     ExcludeSifter,
     IsFileSifter,
     IsDirSifter,
 )
 from alipcs_py.commands.display import (
@@ -52,15 +54,15 @@
 )
 from alipcs_py.commands.play import play as _play, Player, DEFAULT_PLAYER
 from alipcs_py.commands.upload import upload as _upload, from_tos, CPU_NUM, UploadType
 from alipcs_py.commands.sync import sync as _sync
 from alipcs_py.commands import share as _share
 from alipcs_py.commands.server import start_server
 from alipcs_py.commands.log import get_logger
-from alipcs_py.storage.store import AliPCSApiWithSharedStore, SharedStore
+from alipcs_py.storage.store import AliPCSApiMixWithSharedStore, SharedStore
 from alipcs_py.config import AppConfig
 from alipcs_py.app.config import init_config
 
 import click
 
 from rich import print
 from rich.console import Console
@@ -135,14 +137,39 @@
         finally:
             _exit_progress_bar()
             _teardown()
 
     return wrap
 
 
+def save_modified_user_data(func):
+    """Save modified user data after some commands is finished"""
+
+    @wraps(func)
+    def wrap(ctx, *args, **kwargs):
+        pre_account_data_path_mtime = ctx.obj.pre_account_data_path_mtime
+
+        try:
+            result = func(ctx, *args, **kwargs)
+            return result
+        except:
+            raise
+        finally:
+            now_account_data_path_mtime = Path(ctx.obj.account_data_path).stat().st_mtime
+            # If the account_data had saved, we ignore to save it
+            if now_account_data_path_mtime == pre_account_data_path_mtime:
+                am = ctx.obj.account_manager
+                used_user_ids = ctx.obj.used_user_ids
+                for user_id in used_user_ids:
+                    am.update(user_id)
+                am.save()
+
+    return wrap
+
+
 def _app_config(ctx):
     """App Configuration"""
 
     return ctx.obj.app_config
 
 
 def _user_ids(ctx) -> Optional[List[int]]:
@@ -170,34 +197,33 @@
 
 def multi_user_do(func):
     """Run command on multi users"""
 
     @wraps(func)
     def wrap(*args, **kwargs):
         ctx = args[0]
+        used_user_ids = ctx.obj.used_user_ids
         user_ids = _user_ids(ctx)
         if not user_ids:
             return func(*args, **kwargs)
 
         am = ctx.obj.account_manager
         for user_id in user_ids:
             accout = am.who(user_id)
             if not accout:
                 continue
 
             user_name = accout.user.user_name
-            print(
-                "[i yellow]@Do[/i yellow]: "
-                f"user_name: [b]{user_name}[/b], "
-                f"user_id: [b]{user_id}[/b]"
-            )
+            print("[i yellow]@Do[/i yellow]: " f"user_name: [b]{user_name}[/b], " f"user_id: [b]{user_id}[/b]")
             _change_account(ctx, user_id)
             func(*args, **kwargs)
             print()
 
+            used_user_ids.add(user_id)
+
     return wrap
 
 
 def _recent_account(ctx) -> Optional[Account]:
     """Return recent user's `AliPCSApi`"""
 
     am = ctx.obj.account_manager
@@ -205,21 +231,26 @@
     if account:
         return account
     else:
         print("[italic red]No recent user, please adding or selecting one[/]")
         return None
 
 
-def _recent_api(ctx) -> Union[AliPCSApi, AliPCSApiWithSharedStore, None]:
+def _recent_api(ctx) -> Union[AliPCSApi, AliPCSApiMixWithSharedStore, None]:
     """Return recent user's `AliPCSApi`"""
 
+    am = ctx.obj.account_manager
     app_config = _app_config(ctx)
     account = _recent_account(ctx)
     if account:
-        api = account.pcsapi()
+        # Record used user_id for save_modified_user_data
+        used_user_ids = ctx.obj.used_user_ids
+        used_user_ids.add(account.user.user_id)
+
+        api = am.get_api()
         if app_config.share.store:
             api._sharedstore = SharedStore()  # type: ignore
         return api
     else:
         return None
 
 
@@ -303,43 +334,45 @@
 _APP_DOC = f"""AliPCS App v{__version__}
 
     \b
     如果第一次使用，你需要运行 `AliPCS-Py useradd` 添加 `refresh_token`。
     如何获取 `refresh_token` 见 https://github.com/PeterDing/AliPCS-Py#%E6%B7%BB%E5%8A%A0%E7%94%A8%E6%88%B7
     用 `AliPCS-Py {{command}} --help` 查看具体的用法。"""
 
-_ALIAS_DOC = "Command 别名:\n\n\b\n" + "\n".join(
-    [f"{alias: >3} : {cmd}" for alias, cmd in ALIAS.items()]
-)
+_ALIAS_DOC = "Command 别名:\n\n\b\n" + "\n".join([f"{alias: >3} : {cmd}" for alias, cmd in ALIAS.items()])
 
 
 @click.group(cls=AliasedGroup, help=_APP_DOC, epilog=_ALIAS_DOC)
-@click.option(
-    "--config", "-c", type=str, default=CONFIG_PATH, help="Configuration file"
-)
+@click.option("--config", "-c", type=str, default=CONFIG_PATH, help="Configuration file")
 @click.option(
     "--account-data-path",
     "--adp",
     type=str,
     default=ACCOUNT_DATA_PATH,
     help="Account data file",
 )
 @click.option("--accounts", "-u", type=str, default=None, help="帐号名片段，用“,”分割")
 @click.pass_context
 def app(ctx, config, account_data_path, accounts):
+    ctx.obj.account_data_path = account_data_path
+    ad_path = Path(account_data_path)
+    ctx.obj.pre_account_data_path_mtime = 0
+    if ad_path.exists():
+        ctx.obj.pre_account_data_path_mtime = ad_path.stat().st_mtime
     ctx.obj.account_manager = AccountManager.load_data(account_data_path)
     ctx.obj.accounts = [] if accounts is None else accounts.split(",")
+    ctx.obj.used_user_ids = set()
 
     # Load app config
     app_config = AppConfig.load(config)
     ctx.obj.app_config = app_config
     init_config(app_config)
 
     if app_config.share.store:
-        account_module.AliPCSApi = AliPCSApiWithSharedStore
+        account_module.AliPCSApiMix = AliPCSApiMixWithSharedStore
 
 
 # Account
 # {{{
 @app.command()
 @click.argument("user_id", type=int, default=None, required=False)
 @click.option("--show-encrypt-password", "-K", is_flag=True, help="显示加密密码")
@@ -428,35 +461,55 @@
         [(a.user, a.pwd, a.account_name) for a in am.accounts],
         key=lambda x: x[0].user_id,
     )
     display_user_infos(*ls, recent_user_id=am._who)
 
 
 @app.command()
+@click.option("--account-name", prompt="Account Name", hide_input=False, default="", help="账号名 [默认为 user id]")
+@click.option("--web-refresh-token", prompt="web refresh token", hide_input=True, help="用户 web_refresh_token")
 @click.option(
-    "--account_name",
-    prompt="Account Name",
-    hide_input=False,
-    default="",
-    help="账号名 [默认为 user id]",
-)
-@click.option(
-    "--refresh-token",
-    prompt="refresh token",
+    "--openapi-refresh-token",
+    prompt="openapi refresh token",
     hide_input=True,
-    help="用户 refresh_token",
+    default="",
+    help="用户 openapi_refresh_token",
 )
+@click.option("--client-id", prompt="open client id", default="", help="openapi client id")
+@click.option("--client-secret", prompt="open client secret", default="", help="openapi client secret")
+@click.option("--client-server", prompt="open client server", default="", help="openapi client server")
 @click.pass_context
 @handle_error
-def useradd(ctx, account_name, refresh_token):
+def useradd(ctx, account_name, web_refresh_token, openapi_refresh_token, client_id, client_secret, client_server):
     """添加一个用户并设置为当前用户"""
 
-    assert refresh_token, "No `refresh_token`"
+    assert web_refresh_token, "No `web_refresh_token`"
 
-    account = Account.from_refresh_token(refresh_token, account_name=account_name)
+    openapi_access_token = ""
+    openapi_token_type = "Bearer"
+    openapi_expire_time = 0
+    if (client_id and client_secret) or client_server:
+        if not openapi_refresh_token:
+            auth_info = openapi_qrcode_login(client_id, client_secret, client_server)
+            openapi_refresh_token = auth_info.refresh_token
+            openapi_access_token = auth_info.access_token
+            openapi_token_type = auth_info.token_type
+            openapi_expire_time = auth_info.expire_time
+
+    account = Account.from_refresh_token(
+        web_refresh_token,
+        openapi_refresh_token=openapi_refresh_token,
+        openapi_access_token=openapi_access_token,
+        openapi_token_type=openapi_token_type,
+        openapi_expire_time=openapi_expire_time,
+        client_id=client_id or "",
+        client_secret=client_secret or "",
+        client_server=client_server or "",
+        account_name=account_name,
+    )
     am = ctx.obj.account_manager
     am.add_account(account)
     am.su(account.user.user_id)
     am.save()
 
 
 @app.command()
@@ -525,14 +578,15 @@
 
     pwd = _pwd(ctx)
     print(pwd)
 
 
 # }}}
 
+
 # File Operations
 # {{{
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--file-id", "-i", multiple=True, type=str, help="文件 ID")
 @click.option("--share-id", "--si", nargs=1, type=str, help="列出这个分享ID下的文件")
 @click.option("--share-url", "--su", nargs=1, type=str, help="列出这个分享url下的文件")
@@ -555,14 +609,15 @@
 @click.option("--show-hash", "-H", is_flag=True, help="显示文件 sha1")
 @click.option("--show-absolute-path", "-A", is_flag=True, help="显示文件绝对路径")
 @click.option("--show-dl-link", "--DL", is_flag=True, help="显示文件下载连接")
 @click.option("--csv", is_flag=True, help="用 csv 格式显示，单行显示，推荐和 --DL 或 --HL 一起用")
 @click.option("--only-dl-link", "--ODL", is_flag=True, help="只显示文件下载连接")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def ls(
     ctx,
     remotepaths,
     file_id,
     share_id,
     share_url,
@@ -675,14 +730,15 @@
 @click.option("--no-highlight", "--NH", is_flag=True, help="取消匹配高亮")
 @click.option("--show-size", "-S", is_flag=True, help="显示文件大小")
 @click.option("--show-date", "-D", is_flag=True, help="显示文件创建时间")
 @click.option("--show-hash", "-H", is_flag=True, help="显示文件 sha1")
 @click.option("--csv", is_flag=True, help="用 csv 格式显示")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def search(
     ctx,
     keyword,
     include,
     include_regex,
     exclude,
@@ -728,19 +784,18 @@
     )
 
 
 @app.command()
 @click.argument("remotepath", nargs=1, type=str)
 @click.option("--encoding", "-e", type=str, help="文件编码，默认自动解码")
 @click.option("--no-decrypt", "--ND", is_flag=True, help="不解密")
-@click.option(
-    "--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的"
-)
+@click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def cat(ctx, remotepath, encoding, no_decrypt, encrypt_password):
     """显示文件内容"""
 
     api = _recent_api(ctx)
     if not api:
         return
@@ -757,14 +812,15 @@
 
 
 @app.command()
 @click.argument("remotedirs", nargs=-1, type=str)
 @click.option("--show", "-S", is_flag=True, help="显示目录")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def mkdir(ctx, remotedirs, show):
     """创建目录"""
 
     api = _recent_api(ctx)
     if not api:
         return
@@ -776,14 +832,15 @@
 
 
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--show", "-S", is_flag=True, help="显示结果")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def move(ctx, remotepaths, show):
     """移动文件
 
     \b
     examples:
         move /file1 /file2 /to/dir
@@ -803,14 +860,15 @@
 
 @app.command()
 @click.argument("remotepath", nargs=1, type=str)
 @click.argument("new_name", nargs=1, type=str)
 @click.option("--show", "-S", is_flag=True, help="显示结果")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def rename(ctx, remotepath, new_name, show):
     """文件重命名
 
     \b
     examples:
         rename /path/to/far new_name_foo
@@ -828,14 +886,15 @@
 
 
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--show", "-S", is_flag=True, help="显示结果")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def copy(ctx, remotepaths, show):
     """拷贝文件
 
     \b
     examples:
         copy /file1 /file2 /to/dir
@@ -854,14 +913,15 @@
 
 
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--file-id", "-i", multiple=True, type=str, help="文件 ID")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def remove(ctx, remotepaths, file_id):
     """删除文件"""
 
     api = _recent_api(ctx)
     if not api:
         return
@@ -879,17 +939,15 @@
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--file-id", "-i", multiple=True, type=str, help="文件 ID")
 @click.option("--outdir", "-o", nargs=1, type=str, default=".", help="指定下载本地目录，默认为当前目录")
 @click.option("--share-id", "--si", nargs=1, type=str, help="下载这个分享ID下的文件")
 @click.option("--share-url", "--su", nargs=1, type=str, help="下载这个分享url下的文件")
 @click.option("--password", "-p", type=str, help="分享链接密码，如果没有不用设置")
 @click.option("--recursive", "-R", is_flag=True, help="递归下载")
-@click.option(
-    "--from-index", "-f", type=int, default=0, help="从所有目录中的第几个文件开始下载，默认为0（第一个）"
-)
+@click.option("--from-index", "-f", type=int, default=0, help="从所有目录中的第几个文件开始下载，默认为0（第一个）")
 @click.option("--include", "-I", type=str, help="筛选包含这个字符串的文件")
 @click.option("--include-regex", "--IR", type=str, help="筛选包含这个正则表达式的文件")
 @click.option("--exclude", "-E", type=str, help="筛选 不 包含这个字符串的文件")
 @click.option("--exclude-regex", "--ER", type=str, help="筛选 不 包含这个正则表达式的文件")
 @click.option(
     "-d",
     "--downloader",
@@ -912,25 +970,22 @@
 @click.option(
     "--concurrency",
     "-s",
     type=int,
     default=DEFAULT_CONCURRENCY,
     help=f"下载同步链接数，默认为{DEFAULT_CONCURRENCY}。建议小于 10",
 )
-@click.option(
-    "--chunk-size", "-k", type=str, default=DEFAULT_CHUNK_SIZE, help="同步链接分块大小"
-)
+@click.option("--chunk-size", "-k", type=str, default=DEFAULT_CHUNK_SIZE, help="同步链接分块大小")
 @click.option("--no-decrypt", "--ND", is_flag=True, help="不解密")
 @click.option("--quiet", "-q", is_flag=True, help="取消第三方下载应用输出")
 @click.option("--out-cmd", "--OC", is_flag=True, help="输出第三方下载应用命令")
-@click.option(
-    "--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的"
-)
+@click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def download(
     ctx,
     remotepaths,
     file_id,
     outdir,
     share_id,
@@ -988,17 +1043,15 @@
             share_id=share_id,
             share_url=share_url,
             password=password,
             sifters=sifters,
             recursive=recursive,
             from_index=from_index,
             downloader=getattr(Downloader, downloader),
-            downloadparams=DownloadParams(
-                concurrency=concurrency, chunk_size=chunk_size, quiet=quiet
-            ),
+            downloadparams=DownloadParams(concurrency=concurrency, chunk_size=chunk_size, quiet=quiet),
             out_cmd=out_cmd,
             encrypt_password=encrypt_password,
         )
     else:
         pwd = _pwd(ctx)
         remotepaths = [join_path(pwd, r) for r in remotepaths]
         _download(
@@ -1006,32 +1059,28 @@
             remotepaths,
             file_id,
             outdir,
             sifters=sifters,
             recursive=recursive,
             from_index=from_index,
             downloader=getattr(Downloader, downloader),
-            downloadparams=DownloadParams(
-                concurrency=concurrency, chunk_size=chunk_size, quiet=quiet
-            ),
+            downloadparams=DownloadParams(concurrency=concurrency, chunk_size=chunk_size, quiet=quiet),
             out_cmd=out_cmd,
             encrypt_password=encrypt_password,
         )
 
 
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--file-id", "-i", multiple=True, type=str, help="文件 ID")
 @click.option("--share-id", "--si", nargs=1, type=str, help="播放这个分享ID下的文件")
 @click.option("--share-url", "--su", nargs=1, type=str, help="播放这个分享url下的文件")
 @click.option("--password", "-p", type=str, help="分享链接密码，如果没有不用设置")
 @click.option("--recursive", "-R", is_flag=True, help="递归播放")
-@click.option(
-    "--from-index", "-f", type=int, default=0, help="从所有目录中的第几个文件开始播放，默认为0（第一个）"
-)
+@click.option("--from-index", "-f", type=int, default=0, help="从所有目录中的第几个文件开始播放，默认为0（第一个）")
 @click.option("--include", "-I", type=str, help="筛选包含这个字符串的文件")
 @click.option("--include-regex", "--IR", type=str, help="筛选包含这个正则表达式的文件")
 @click.option("--exclude", "-E", type=str, help="筛选 不 包含这个字符串的文件")
 @click.option("--exclude-regex", "--ER", type=str, help="筛选 不 包含这个正则表达式的文件")
 @click.option(
     "--player",
     "--pl",
@@ -1045,19 +1094,18 @@
 )
 @click.option("--player-params", "--PP", multiple=True, type=str, help="第三方播放器参数")
 @click.option("--quiet", "-q", is_flag=True, help="取消第三方播放器输出")
 @click.option("--shuffle", "--sf", is_flag=True, help="随机播放")
 @click.option("--ignore-ext", "--IE", is_flag=True, help="不用文件名后缀名来判断媒体文件")
 @click.option("--out-cmd", "--OC", is_flag=True, help="输出第三方播放器命令")
 @click.option("--use-local-server", "-s", is_flag=True, help="使用本地服务器播放。")
-@click.option(
-    "--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的"
-)
+@click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def play(
     ctx,
     remotepaths,
     file_id,
     share_id,
     share_url,
@@ -1092,17 +1140,15 @@
         sifters.append(ExcludeSifter(exclude, regex=False))
     if exclude_regex:
         sifters.append(ExcludeSifter(exclude_regex, regex=True))
 
     local_server = ""
     if use_local_server:
         if share_id or file_id:
-            assert ValueError(
-                "Recently local server can't play others shared items and using `file_id`"
-            )
+            assert ValueError("Recently local server can't play others shared items and using `file_id`")
 
         encrypt_password = encrypt_password or _encrypt_password(ctx)
 
         host = "localhost"
         port = random_avail_port()
 
         local_server = f"http://{host}:{port}"
@@ -1172,37 +1218,30 @@
 @click.argument("localpaths", nargs=-1, type=str)
 @click.argument("remotedir", nargs=1, type=str)
 @click.option(
     "--upload-type",
     "-t",
     type=click.Choice([t.name for t in UploadType]),
     default=UploadType.Many.name,
-    help=(
-        "上传方式，Many: 同时上传多个文件，"
-        "One: 一次只上传一个文件，但同时上传文件的多个分片 "
-        "(阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效)"
-    ),
-)
-@click.option(
-    "--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的"
+    help=("上传方式，Many: 同时上传多个文件，" "One: 一次只上传一个文件，但同时上传文件的多个分片 " "(阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效)"),
 )
+@click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.option(
     "--encrypt-type",
     "-e",
     type=click.Choice([t.name for t in EncryptType]),
     default=EncryptType.No.name,
     help="文件加密方法，默认为 No 不加密",
 )
-@click.option(
-    "--max-workers", "-w", type=int, default=CPU_NUM, help="同时上传连接数量，默认为 CPU 核数"
-)
+@click.option("--max-workers", "-w", type=int, default=CPU_NUM, help="同时上传连接数量，默认为 CPU 核数")
 @click.option("--no-ignore-existing", "--NI", is_flag=True, help="上传已经存在的文件")
 @click.option("--no-show-progress", "--NP", is_flag=True, help="不显示上传进度")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def upload(
     ctx,
     localpaths,
     remotedir,
     upload_type,
     encrypt_password,
@@ -1248,28 +1287,27 @@
         show_progress=not no_show_progress,
     )
 
 
 @app.command()
 @click.argument("localdir", nargs=1, type=str)
 @click.argument("remotedir", nargs=1, type=str)
-@click.option(
-    "--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的"
-)
+@click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.option(
     "--encrypt-type",
     "-e",
     type=click.Choice([t.name for t in EncryptType]),
     default=EncryptType.No.name,
     help="文件加密方法，默认为 No 不加密",
 )
 @click.option("--max-workers", "-w", type=int, default=CPU_NUM, help="同时上传文件数")
 @click.option("--no-show-progress", "--NP", is_flag=True, help="不显示上传进度")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def sync(
     ctx,
     localdir,
     remotedir,
     encrypt_password,
     encrypt_type,
@@ -1310,14 +1348,15 @@
 # {{{
 @app.command()
 @click.argument("remotepaths", nargs=-1, type=str)
 @click.option("--password", "-p", type=str, default="", help="设置秘密，默认没有秘密")
 @click.option("--period-time", "--pt", type=int, default=0, help="设置分享有效期，单位为天")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def share(ctx, remotepaths, password, period_time):
     """分享文件
 
     \b
     examples:
         share /path1 path2
@@ -1333,14 +1372,15 @@
     _share.share_files(api, *remotepaths, password=password, period=period_time or 0)
 
 
 @app.command()
 @click.option("--show-all", "-A", is_flag=True, help="显示所有分享的链接，默认只显示有效的分享链接")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def shared(ctx, show_all):
     """列出分享链接"""
 
     api = _recent_api(ctx)
     if not api:
         return
@@ -1348,14 +1388,15 @@
     _share.list_shared(api, show_all=show_all)
 
 
 @app.command()
 @click.argument("share_ids", nargs=-1, type=str)
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def cancelshared(ctx, share_ids):
     """取消分享链接"""
 
     api = _recent_api(ctx)
     if not api:
         return
@@ -1366,14 +1407,15 @@
 @app.command()
 @click.argument("share_url_or_id", nargs=1, type=str)
 @click.argument("remotedir", nargs=1, type=str)
 @click.option("--file-id", "-i", multiple=True, type=str, help="文件 ID")
 @click.option("--password", "-p", type=str, help="分享链接密码，如果没有不用设置")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
 def save(ctx, share_url_or_id, file_id, remotedir, password):
     """保存其他用户分享的链接"""
 
     api = _recent_api(ctx)
     if not api:
         return
@@ -1399,42 +1441,39 @@
 
 
 @app.command()
 @click.argument("share_urls_or_ids", nargs=-1, type=str)
 @click.option("--password", "-p", type=str, help="分享链接密码，如果没有不用设置")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 def storesharedlinks(ctx, share_urls_or_ids, password):
     """保存分享连接至本地
 
     注意: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true
     """
 
     app_config = _app_config(ctx)
     if not app_config.share.store:
-        print(
-            "App configuration `[share] store is false`. So the command does not work"
-        )
+        print("App configuration `[share] store is false`. So the command does not work")
         return
 
     api = _recent_api(ctx)
     if not api:
         return
 
     for share_url_or_id in share_urls_or_ids:
         share_url = ""
         share_id = ""
         if "/s/" in share_url_or_id:
             share_url = share_url_or_id
         else:
             share_id = share_url_or_id
 
-        _share.get_share_token(
-            api, share_id=share_id, share_url=share_url, password=password
-        )
+        _share.get_share_token(api, share_id=share_id, share_url=share_url, password=password)
 
 
 @app.command()
 @click.pass_context
 @handle_error
 def listsharedlinks(ctx):
     """显示本地保存的分享连接
@@ -1493,17 +1532,15 @@
 
     注意: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true
     """
 
     _find_shared_links(keywords)
 
 
-def _find_shared_files(
-    keywords: List[str], share_ids: List[str] = [], verbose: bool = False
-):
+def _find_shared_files(keywords: List[str], share_ids: List[str] = [], verbose: bool = False):
     shared_store = SharedStore()
     shared_files = shared_store.search_shared_files(*keywords, share_ids=share_ids)
     display_shared_files(*shared_files, verbose=verbose)
 
 
 @app.command()
 @click.argument("keywords", nargs=-1, type=str)
@@ -1534,19 +1571,18 @@
     _find_shared_links(keywords)
     print()
     _find_shared_files(keywords, verbose=verbose)
 
 
 @app.command()
 @click.argument("share_ids", nargs=-1, type=str)
-@click.option(
-    "--keyword", "-k", multiple=True, type=str, help="要删除文件名的关键字，如果为空则删除share_id下的所有文件"
-)
+@click.option("--keyword", "-k", multiple=True, type=str, help="要删除文件名的关键字，如果为空则删除share_id下的所有文件")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 def deletestoredshared(ctx, share_ids, keyword):
     """删除本地保存的分享连接或文件
 
     注意: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true
     """
 
     if not share_ids:
@@ -1588,20 +1624,18 @@
     """清理本地保存的无效分享连接
 
     注意: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true
     """
 
     app_config = _app_config(ctx)
     if not app_config.share.store:
-        print(
-            "App configuration `[share] store is false`. So the command does not work"
-        )
+        print("App configuration `[share] store is false`. So the command does not work")
         return
 
-    api: AliPCSApiWithSharedStore = _recent_api(ctx)
+    api: AliPCSApiMixWithSharedStore = _recent_api(ctx)
     if not api:
         return
 
     store = api.sharedstore
     if not store:
         return
 
@@ -1610,33 +1644,31 @@
         if not api.is_shared_valid(shared_link.share_id):
             store.delete_shared_links(shared_link.share_id)
             display_invalid_shared_link_infos(shared_link)
 
 
 # }}}
 
+
 # Server
 # {{{
 @app.command()
 @click.argument("root_dir", type=str, default="/", required=False)
 @click.option("--path", type=str, default="/", help="服务路径，默认为 “/”")
 @click.option("--host", "-h", type=str, default="localhost", help="监听 host")
 @click.option("--port", "-p", type=int, default=8000, help="监听 port")
 @click.option("--workers", "-w", type=int, default=CPU_NUM, help="进程数")
-@click.option(
-    "--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的"
-)
+@click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.option("--username", type=str, default=None, help="HTTP Basic Auth 用户名")
 @click.option("--password", type=str, default=None, help="HTTP Basic Auth 密钥")
 @click.pass_context
 @handle_error
+@save_modified_user_data
 @multi_user_do
-def server(
-    ctx, root_dir, path, host, port, workers, encrypt_password, username, password
-):
+def server(ctx, root_dir, path, host, port, workers, encrypt_password, username, password):
     """开启 HTTP 服务"""
 
     api = _recent_api(ctx)
     if not api:
         return
 
     encrypt_password = encrypt_password or _encrypt_password(ctx)
```

### Comparing `alipcs_py-0.5.3/alipcs_py/app/config.py` & `alipcs_py-0.6.0/alipcs_py/app/config.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/cat.py` & `alipcs_py-0.6.0/alipcs_py/commands/cat.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/crypto.py` & `alipcs_py-0.6.0/alipcs_py/commands/crypto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from os import PathLike
 from pathlib import Path
 
 from alipcs_py.common.io import to_decryptio, READ_SIZE
 from alipcs_py.common.path import exists
 
 
-def decrypt_file(
-    from_encrypted: PathLike, to_decrypted: PathLike, encrypt_password: bytes = b""
-):
+def decrypt_file(from_encrypted: PathLike, to_decrypted: PathLike, encrypt_password: bytes = b""):
     assert exists(from_encrypted)
 
     dio = to_decryptio(open(from_encrypted, "rb"), encrypt_password=encrypt_password)
 
     dpath = Path(to_decrypted)
     dir_ = dpath.parent
     if not dir_.exists():
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/display.py` & `alipcs_py-0.6.0/alipcs_py/commands/display.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,17 +133,15 @@
                 row[0] = "d"
             else:
                 tp._text = ["d"]
                 background.style = "blue"
 
         if highlight and sifters:
             pats: List[Union[Pattern, str]] = list(
-                filter(
-                    None, [sifter.pattern() for sifter in sifters if sifter.include()]
-                )
+                filter(None, [sifter.pattern() for sifter in sifters if sifter.include()])
             )
             highlighter = Highlighter(pats, "yellow")
             _path = highlighter(path)
         else:
             _path = Text(path)
 
         if csv:
@@ -226,28 +224,24 @@
 
     console = Console()
     console.print(*panels)
 
 
 def display_invalid_shared_link_infos(*shared_links: PcsSharedLinkInfo):
     for shared_link in shared_links:
-        print(
-            f"[i yellow]Remove[/i yellow]: {shared_link.share_url}\t{shared_link.share_name}"
-        )
+        print(f"[i yellow]Remove[/i yellow]: {shared_link.share_url}\t{shared_link.share_name}")
 
 
 def display_shared_paths(*shared_paths):
     table = Table(box=SIMPLE, padding=0, show_edge=False)
     table.add_column()
     table.add_column("Size", justify="right")
     table.add_column("Path", justify="left", overflow="fold")
 
-    max_size_str_len = max(
-        [len(str(shared_path.size or 0)) for shared_path in shared_paths]
-    )
+    max_size_str_len = max([len(str(shared_path.size or 0)) for shared_path in shared_paths])
     for shared_path in shared_paths:
         row: List[Union[str, Text]] = []
 
         # Is file
         tp = Text("-", style="bold red")
         row.append(tp)
 
@@ -277,17 +271,15 @@
     table.add_column("Expiration", justify="left", overflow="fold")
 
     for shared_link_info in shared_link_infos:
         table.add_row(
             f"https://www.aliyundrive.com/s/{shared_link_info.share_id}",
             shared_link_info.share_pwd or "",
             shared_link_info.share_name or shared_link_info.display_name or "",
-            format_date(shared_link_info.expiration)
-            if shared_link_info.expiration
-            else "Never",
+            format_date(shared_link_info.expiration) if shared_link_info.expiration else "Never",
         )
 
     console = Console()
     console.print(table)
 
 
 _SHARED_FILE_FORMAT = (
@@ -298,31 +290,27 @@
     "Size: {size}\n"
     "File ID: {file_id}\n"
     "Name: {name}\n"
     "Share URL Directory: {share_url_directory}"
 )
 
 
-def display_shared_files(
-    *shared_file_and_links: Tuple[PcsFile, PcsSharedLinkInfo], verbose: bool = False
-):
+def display_shared_files(*shared_file_and_links: Tuple[PcsFile, PcsSharedLinkInfo], verbose: bool = False):
     if verbose:
         panels = []
         for shared_file, shared_link_info in shared_file_and_links:
             if shared_file.is_dir:
                 share_url = f"https://www.aliyundrive.com/s/{shared_link_info.share_id}/folder/{shared_file.file_id}"
             else:
                 share_url = f"https://www.aliyundrive.com/s/{shared_link_info.share_id}"
             panel = Panel(
                 _SHARED_FILE_FORMAT.format(
                     share_url=share_url,
                     password=shared_link_info.share_pwd or "",
-                    share_name=shared_link_info.share_name
-                    or shared_link_info.display_name
-                    or "",
+                    share_name=shared_link_info.share_name or shared_link_info.display_name or "",
                     type=shared_file.type,
                     size=human_size(shared_file.size or 0),
                     file_id=shared_file.file_id,
                     name=shared_file.name,
                     share_url_directory=f"https://www.aliyundrive.com/s/{shared_link_info.share_id}/folder/{shared_file.parent_file_id}",
                 ),
                 highlight=True,
@@ -361,46 +349,60 @@
     default_drive_id = user_info.default_drive_id
     domain_id = user_info.domain_id
     user_name = user_info.user_name
     nick_name = user_info.nick_name
     phone = user_info.phone
     personal_space_info = user_info.personal_space_info
 
-    refresh_token = user_info.refresh_token
-    access_token = user_info.access_token
-    expire_time = format_date(user_info.expire_time or 0)
+    web_refresh_token = user_info.web_refresh_token
+    web_access_token = user_info.web_access_token
+    web_token_type = user_info.web_token_type
+    web_expire_time = format_date(user_info.web_expire_time or 0)
+
+    openapi_refresh_token = user_info.openapi_refresh_token
+    openapi_access_token = user_info.openapi_access_token
+    openapi_token_type = user_info.openapi_token_type
+    openapi_expire_time = format_date(user_info.openapi_expire_time or 0)
+
+    client_id = user_info.client_id
+    client_secret = user_info.client_secret
+    client_server = user_info.client_server
 
     assert personal_space_info
-    quota_str = (
-        human_size(personal_space_info.used_size)
-        + "/"
-        + human_size(personal_space_info.total_size)
-    )
+    quota_str = human_size(personal_space_info.used_size) + "/" + human_size(personal_space_info.total_size)
 
     _tempt = (
         f"user id: {user_id}\n"
         f"user name: {user_name}\n"
         f"nick name: {nick_name}\n"
         f"user phone: {phone}\n"
         f"default drive id: {default_drive_id}\n"
         f"domain id: {domain_id}\n"
         f"quota: {quota_str}\n"
         "\n"
-        f"refresh token: {refresh_token}\n"
-        f"access token: {access_token}\n"
-        f"expire time: {expire_time}\n"
+        f"web_refresh token: {web_refresh_token}\n"
+        f"web_access token: {web_access_token}\n"
+        f"web_token_type: {web_token_type}\n"
+        f"web_expire time: {web_expire_time}\n"
+        "\n"
+        f"openapi_refresh token: {openapi_refresh_token}\n"
+        f"openapi_access token: {openapi_access_token}\n"
+        f"openapi_token_type: {openapi_token_type}\n"
+        f"openapi_expire time: {openapi_expire_time}\n"
+        "\n"
+        f"client_id: {client_id}\n"
+        f"client_secret: {client_secret}\n"
+        f"client_server: {client_server}\n"
     )
 
     console = Console()
     console.print(_tempt, highlight=True)
 
 
-def display_user_infos(
-    *user_infos: Tuple[PcsUser, str, str], recent_user_id: Optional[int] = None
-):
+def display_user_infos(*user_infos: Tuple[PcsUser, str, str], recent_user_id: Optional[int] = None):
     """
     Args:
         user_infos (*Tuple[PcsUser, pwd: str])
     """
 
     table = Table(box=SIMPLE, show_edge=False, highlight=True)
     table.add_column("Index", justify="left")
@@ -419,23 +421,17 @@
         nick_name = user_info.nick_name
         personal_space_info = user_info.personal_space_info
         vip = ""
         if user_info.user_vip_info:
             vip = f"[b red]{user_info.user_vip_info.identity}[/b red]"
 
         assert personal_space_info
-        quota_str = (
-            human_size(personal_space_info.used_size)
-            + "/"
-            + human_size(personal_space_info.total_size)
-        )
+        quota_str = human_size(personal_space_info.used_size) + "/" + human_size(personal_space_info.total_size)
 
-        table.add_row(
-            str(idx), is_recent, account_name, user_name, nick_name, quota_str, vip, pwd
-        )
+        table.add_row(str(idx), is_recent, account_name, user_name, nick_name, quota_str, vip, pwd)
 
     console = Console()
     console.print(table)
 
 
 def display_blocked_remotepath(remotepath: str):
     print(f"[i yellow]Remote path is blocked[/i yellow]: {remotepath}")
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/download.py` & `alipcs_py-0.6.0/alipcs_py/commands/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, List, Dict, Any, Callable
 from types import SimpleNamespace
 from enum import Enum
 from pathlib import Path
 import os
+import time
 import shutil
 import subprocess
 from concurrent.futures import Future
 
 from alipcs_py.alipcs import AliPCSApi, PcsFile
 from alipcs_py.alipcs.pcs import PCS_UA
 from alipcs_py.utils import human_size_to_int
@@ -106,17 +107,15 @@
             return
 
         returncode = self.spawn(cmd, downloadparams.quiet)
 
         logger.debug("`download`: cmd returncode: %s", returncode)
 
         if returncode != 0:
-            print(
-                f"[italic]{self.value}[/italic] fails. return code: [red]{returncode}[/red]"
-            )
+            print(f"[italic]{self.value}[/italic] fails. return code: [red]{returncode}[/red]")
         else:
             if encrypt_password:
                 dio = to_decryptio(open(localpath_tmp, "rb"), encrypt_password)
                 if isinstance(dio, DecryptIO):
                     with open(localpath, "wb") as fd:
                         while True:
                             buf = dio.read(READ_SIZE)
@@ -287,35 +286,47 @@
         print(f"[yellow]{localpath}[/yellow] is ready existed.")
         return
 
     if not pcs_file:
         return
 
     if downloader != Downloader.me:
-        print(
-            f"[italic blue]Download[/italic blue]: {pcs_file.path or pcs_file.name} to {localpath}"
-        )
+        print(f"[italic blue]Download[/italic blue]: {pcs_file.path or pcs_file.name} to {localpath}")
 
     download_url: Optional[str]
     if share_id:
-        download_url = api.shared_file_download_url(pcs_file.file_id, share_id)
-    else:
-        pcs_file.update_download_url(api)
-        download_url = pcs_file.download_url
+        remote_temp_dir = "/__alipcs_py_temp__"
+        pcs_temp_dir = api.path(remote_temp_dir) or api.makedir_path(remote_temp_dir)
+        pcs_file = api.transfer_shared_files([pcs_file.file_id], pcs_temp_dir.file_id, share_id)[0]
+
+        while True:
+            pcs_file = api.meta(pcs_file.file_id)[0]
+            if pcs_file.download_url:
+                break
+            time.sleep(2)
+
+    if not pcs_file or pcs_file.is_dir:
+        return
+
+    pcs_file.update_download_url(api)
+    download_url = pcs_file.download_url
 
     assert download_url
 
     downloader.download(
         download_url,
         str(localpath),
         downloadparams=downloadparams,
         out_cmd=out_cmd,
         encrypt_password=encrypt_password,
     )
 
+    if share_id:
+        api.remove(pcs_file.file_id)
+
 
 def download_dir(
     api: AliPCSApi,
     pcs_file: PcsFile,
     localdir: str,
     share_id: str = None,
     sifters: List[Sifter] = [],
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/file_operators.py` & `alipcs_py-0.6.0/alipcs_py/commands/file_operators.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/index.html` & `alipcs_py-0.6.0/alipcs_py/commands/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,15 @@
                                 <span class="goup">Go up</span>
                             </a>
                         </td>
                         <td>&mdash;</td>
                         <td class="hideable">&mdash;</td>
                         <td class="hideable"></td>
                     </tr>
-                    {% for is_dir, name, escaped_name, size, local_mtime in entries %}
+                    {% for file_id, is_dir, name, escaped_name, size, local_mtime in entries %}
                     <tr class="file">
                         <td>
                         </td>
                         <td>
                             {% if is_dir %}
                             <svg width="1.5em" height="1em" version="1.1" viewBox="0 0 317 259">
                                 <use xlink:href="#folder"></use>
@@ -347,15 +347,15 @@
                             <svg width="1.5em" height="1em" version="1.1" viewBox="0 0 265 323">
                                 <use xlink:href="#file"></use>
                             </svg>
                             {% endif %}
                             {% if is_dir %}
                             <span class="name"><a href="{{ escaped_name }}/">{{ name }}</a></span>
                             {% else %}
-                            <span class="name"><a href="{{ escaped_name }}">{{ name }}</a></span>
+                            <span class="name"><a href="/__fileid__/?file_id={{ file_id }}">{{ name }}</a></span>
                             {% endif %}
                         </td>
                         {% if is_dir %}
                         <td data-order="-1">&mdash;</td>
                         {% else %}
                         <td data-order="{{ size }}">
                             <size>{{ size }}</size>
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/list_files.py` & `alipcs_py-0.6.0/alipcs_py/commands/list_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     file_id: str = None,
     share_id: str = None,
     desc: bool = False,
     name: bool = False,
     time: bool = False,
     size: bool = False,
     all: bool = False,
-    limit: int = 100,
-    url_expire_sec: int = 7200,
+    limit: int = 200,
+    url_expire_sec: int = 14400,
     recursive: bool = False,
     sifters: List[Sifter] = [],
     highlight: bool = False,
     rapiduploadinfo_file: Optional[str] = None,
     user_id: Optional[str] = None,
     user_name: Optional[str] = None,
     show_size: bool = False,
@@ -128,16 +128,16 @@
     file_ids: List[str] = [],
     share_id: str = None,
     desc: bool = False,
     name: bool = False,
     time: bool = False,
     size: bool = False,
     all: bool = False,
-    limit: int = 100,
-    url_expire_sec: int = 7200,
+    limit: int = 200,
+    url_expire_sec: int = 14400,
     recursive: bool = False,
     sifters: List[Sifter] = [],
     highlight: bool = False,
     rapiduploadinfo_file: Optional[str] = None,
     user_id: Optional[str] = None,
     user_name: Optional[str] = None,
     show_size: bool = False,
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/play.py` & `alipcs_py-0.6.0/alipcs_py/commands/play.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         quiet: bool = False,
         player_params: List[str] = [],
         out_cmd: bool = False,
         use_local_server: bool = False,
     ):
         global DEFAULT_PLAYER
         if not self.which():
-            print(
-                f"[yellow]No player {self.name}[/yellow], using default player: {DEFAULT_PLAYER.name}"
-            )
+            print(f"[yellow]No player {self.name}[/yellow], using default player: {DEFAULT_PLAYER.name}")
             self = DEFAULT_PLAYER
         if not self.which():
             raise CommandError(f"No player: {self.name}")
 
         if self == Player.mpv:
             cmd = self._mpv_cmd(
                 url,
@@ -70,17 +68,15 @@
         # Print out command
         if out_cmd:
             _print(" ".join((repr(c) for c in cmd)))
             return
 
         returncode = self.spawn(cmd)
         if returncode != 0:
-            print(
-                f"[italic]{self.value}[/italic] fails. return code: [red]{returncode}[/red]"
-            )
+            print(f"[italic]{self.value}[/italic] fails. return code: [red]{returncode}[/red]")
 
     def spawn(self, cmd: List[str], quiet: bool = False):
         child = subprocess.run(
             cmd,
             stdout=subprocess.DEVNULL if quiet else None,
         )
         return child.returncode
@@ -130,18 +126,27 @@
     # For typing
     download_url: Optional[str] = None
 
     use_local_server = bool(local_server)
 
     if share_id:
         use_local_server = False
-        download_url = api.shared_file_download_url(pcs_file.file_id, share_id)
-    elif use_local_server:
-        remotepath = join_path("/", quote(pcs_file.path))
-        download_url = f"{local_server}{remotepath}"
+        remote_temp_dir = "/__alipcs_py_temp__"
+        pcs_temp_dir = api.path(remote_temp_dir) or api.makedir_path(remote_temp_dir)
+        pcs_file = api.transfer_shared_files([pcs_file.file_id], pcs_temp_dir.file_id, share_id)[0]
+        # download_url = api.shared_file_download_url(pcs_file.file_id, share_id)
+
+        while True:
+            pcs_file = api.meta(pcs_file.file_id)[0]
+            if pcs_file.download_url:
+                break
+            time.sleep(2)
+
+    if use_local_server:
+        download_url = f"{local_server}/__fileid__/?file_id={pcs_file.file_id}"
         print("url:", download_url)
     else:
         if not pcs_file or pcs_file.is_dir:
             return
         pcs_file.update_download_url(api)
         download_url = pcs_file.download_url
 
@@ -150,14 +155,17 @@
             download_url,
             quiet=quiet,
             player_params=player_params,
             out_cmd=out_cmd,
             use_local_server=use_local_server,
         )
 
+    if share_id:
+        api.remove(pcs_file.file_id)
+
 
 def play_dir(
     api: AliPCSApi,
     pcs_file: PcsFile,
     share_id: str = None,
     sifters: List[Sifter] = [],
     recursive: bool = False,
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/search.py` & `alipcs_py-0.6.0/alipcs_py/commands/search.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/server.py` & `alipcs_py-0.6.0/alipcs_py/commands/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Dict
+from typing import Optional, Dict, Union
 from pathlib import Path
 import os
 import mimetypes
 import asyncio
 import secrets
 import copy
 from urllib.parse import quote
@@ -31,116 +31,119 @@
 _encrypt_password: bytes = b""
 
 # For Auth
 _username: Optional[str] = None
 _password: Optional[str] = None
 
 # This template is from https://github.com/rclone/rclone/blob/master/cmd/serve/httplib/serve/data/templates/index.html
-_html_tempt: Template = Template(
-    (Path(__file__).parent / "index.html").open(encoding="utf-8").read()
-)
+_html_tempt: Template = Template((Path(__file__).parent / "index.html").open(encoding="utf-8").read())
 
 
 def fake_io(io: RangeRequestIO, start: int = 0, end: int = -1):
     for b in io._auto_decrypt_request.read((start, end)):
         yield b
 
 
+def get_file(file_id: str, remotepath: str, _range: Optional[str]):
+    global _api
+    assert _api
+
+    try:
+        fs = _api.file_stream(file_id, encrypt_password=_encrypt_password)
+    except Exception as err:
+        raise HTTPException(status_code=500, detail=f"Error: {err}, remotepath: {remotepath}")
+
+    if not fs:
+        raise HTTPException(status_code=404, detail=f"No download link: {remotepath}")
+
+    length = len(fs)
+
+    headers: Dict[str, str] = {
+        "accept-ranges": "bytes",
+        "connection": "Keep-Alive",
+        "access-control-allow-origin": "*",
+    }
+
+    ext = os.path.splitext(remotepath)[-1]
+    content_type = mimetypes.types_map.get(ext)
+
+    if content_type:
+        headers["content-type"] = content_type
+
+    if _range and fs.seekable():
+        assert _range.startswith("bytes=")
+
+        status_code = 206
+        start, end = _range[6:].split("-")
+        _s, _e = int(start or 0), int(end or length - 1) + 1
+        _iter_io = fake_io(fs, _s, _e)
+        headers["content-range"] = f"bytes {_s}-{_e-1}/{length}"
+        headers["content-length"] = str(_e - _s)
+    else:
+        status_code = 200
+        _iter_io = fake_io(fs)
+        headers["content-length"] = str(length)
+    return StreamingResponse(_iter_io, status_code=status_code, headers=headers)
+
+
 async def handle_request(
     request: Request,
     remotepath: str,
     order: str = "asc",  # desc , asc
     sort: str = "name",  # name, time, size
+    file_id: str = "",
 ):
     desc = order == "desc"
     name = sort == "name"
     time = sort == "time"
     size = sort == "size"
 
     global _root_dir
     global _api
     assert _api
 
+    _range = request.headers.get("range")
+
+    if file_id:
+        return get_file(file_id, remotepath, _range)
+
     remotepath = remotepath.strip("/")
 
     _rp = join_path(_root_dir, remotepath)
 
     # Anti path traversal attack
     if not _rp.startswith(_root_dir):
         raise HTTPException(status_code=404, detail="Item not found")
 
-    _range = request.headers.get("range")
-
     rpf = _api.path(_rp)
     if not rpf:
         raise HTTPException(status_code=404, detail="Item not found")
 
     is_dir = rpf.is_dir
     if is_dir:
         chunks = ["/"] + (remotepath.split("/") if remotepath != "" else [])
-        navigation = [
-            (i - 1, "../" * (len(chunks) - i), name) for i, name in enumerate(chunks, 1)
-        ]
+        navigation = [(i - 1, "../" * (len(chunks) - i), name) for i, name in enumerate(chunks, 1)]
         pcs_files = _api.list_path_iter(_rp, desc=desc, name=name, time=time, size=size)
         entries = []
         for f in pcs_files:
             p = Path(f.path)
             entries.append(
                 (
+                    f.file_id,
                     f.is_dir,
                     p.name,
                     quote(p.name),
                     f.size,
                     format_date(f.updated_at or 0),
                 )
             )
-        cn = _html_tempt.render(
-            root_dir=remotepath, navigation=navigation, entries=entries
-        )
+        cn = _html_tempt.render(root_dir=remotepath, navigation=navigation, entries=entries)
         return HTMLResponse(cn)
     else:
-        try:
-            fs = _api.file_stream(rpf.file_id, encrypt_password=_encrypt_password)
-        except Exception as err:
-            print("Error:", err)
-            raise HTTPException(
-                status_code=500, detail=f"Error: {err}, remotepath: {_rp}"
-            )
-
-        if not fs:
-            raise HTTPException(status_code=404, detail=f"No download link: {_rp}")
-
-        length = len(fs)
-
-        headers: Dict[str, str] = {
-            "accept-ranges": "bytes",
-            "connection": "Keep-Alive",
-            "access-control-allow-origin": "*",
-        }
-
-        ext = os.path.splitext(remotepath)[-1]
-        content_type = mimetypes.types_map.get(ext)
-
-        if content_type:
-            headers["content-type"] = content_type
-
-        if _range and fs.seekable():
-            assert _range.startswith("bytes=")
-
-            status_code = 206
-            start, end = _range[6:].split("-")
-            _s, _e = int(start or 0), int(end or length - 1) + 1
-            _iter_io = fake_io(fs, _s, _e)
-            headers["content-range"] = f"bytes {_s}-{_e-1}/{length}"
-            headers["content-length"] = str(_e - _s)
-        else:
-            status_code = 200
-            _iter_io = fake_io(fs)
-            headers["content-length"] = str(length)
-        return StreamingResponse(_iter_io, status_code=status_code, headers=headers)
+        return get_file(rpf.file_id, remotepath, _range)
 
 
 _security = HTTPBasic()
 
 
 def to_auth(credentials: HTTPBasicCredentials = Depends(_security)) -> str:
     correct_username = secrets.compare_digest(credentials.username, _username or "")
@@ -152,26 +155,33 @@
             headers={"WWW-Authenticate": "Basic"},
         )
     return credentials.username
 
 
 def make_auth_http_server(path: str = ""):
     @app.get("%s/{remotepath:path}" % path)
-    async def auth_http_server(
-        username: str = Depends(to_auth), response: Response = Depends(handle_request)
-    ):
+    async def auth_http_server(username: str = Depends(to_auth), response: Response = Depends(handle_request)):
+        if username:
+            return response
+
+    @app.get("/__fileid__/")
+    async def auth_file_id(username: str = Depends(to_auth), response: Response = Depends(handle_request)):
         if username:
             return response
 
 
 def make_http_server(path: str = ""):
     @app.get("%s/{remotepath:path}" % path)
     async def http_server(response: Response = Depends(handle_request)):
         return response
 
+    @app.get("/__fileid__/")
+    async def file_id(response: Response = Depends(handle_request)):
+        return response
+
 
 def start_server(
     api: AliPCSApi,
     root_dir: str = "/",
     path: str = "",
     host: str = "localhost",
     port: int = 8000,
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/share.py` & `alipcs_py-0.6.0/alipcs_py/commands/share.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     download,
     Downloader,
     DEFAULT_DOWNLOADER,
     DownloadParams,
     DEFAULT_DOWNLOADPARAMS,
 )
 from alipcs_py.commands.play import play, Player, DEFAULT_PLAYER
-from alipcs_py.storage.store import AliPCSApiWithSharedStore, SharedStore
 
 import requests  # type: ignore
 
 from rich import print
 
 
 def share_files(api: AliPCSApi, *remotepaths: str, password: str = "", period: int = 0):
@@ -62,17 +61,15 @@
 
 
 def _extract_file_id(share_url: str) -> str:
     m = re.search(r"/folder/(\w+)", share_url)
     return m.group(1) if m else ""
 
 
-def save_shared_by_url(
-    api: AliPCSApi, remotedir: str, share_url: str, password: str = ""
-):
+def save_shared_by_url(api: AliPCSApi, remotedir: str, share_url: str, password: str = ""):
     share_url = _redirect(share_url)
     share_id = _extract_share_id(share_url)
     file_id = _extract_file_id(share_url)
     file_ids = [file_id] if file_id else []
 
     assert share_id
 
@@ -111,35 +108,29 @@
         rd = _remotedirs[shared_file.file_id]
 
         # Make sure remote dir exists
         if rd not in dest_pcs_files:
             dest_pcs_files[rd] = api.makedir_path(rd)
         dest_pcs_file = dest_pcs_files[rd]
 
-        if not shared_file.is_root() and not remotepath_exists(
-            api, shared_file.name, rd
-        ):
+        if not shared_file.is_root() and not remotepath_exists(api, shared_file.name, rd):
             api.transfer_shared_files(
                 [shared_file.file_id],
                 dest_pcs_file.file_id,
                 share_id,
                 auto_rename=False,
             )
             print(f"save: `{shared_file.path}` to `{rd}`")
         else:
             # Ignore existed file
             if shared_file.is_file:
                 print(f"[yellow]WARNING[/]: `{shared_file.path}` has be in `{rd}`")
                 continue
             else:  # shared_file.is_dir
-                sub_files = list(
-                    api.list_path_iter(
-                        shared_file.path, file_id=shared_file.file_id, share_id=share_id
-                    )
-                )
+                sub_files = list(api.list_path_iter(shared_file.path, file_id=shared_file.file_id, share_id=share_id))
 
                 rd = (PurePosixPath(rd) / shared_file.name).as_posix()
                 for sp in sub_files:
                     _remotedirs[sp.file_id] = rd
                 shared_files.extendleft(sub_files[::-1])
 
 
@@ -149,17 +140,15 @@
     share_id: str = "",
     share_url: str = "",
     file_ids: List[str] = [],
     password: str = "",
 ):
     assert remotedir.startswith("/"), "`remotedir` must be an absolute path"
 
-    assert int(bool(share_id)) ^ int(
-        bool(share_url)
-    ), "`share_id` and `share_url` only can be given one"
+    assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     if share_url:
         save_shared_by_url(api, remotedir, share_url, password=password)
     else:
         save_shared_by_file_ids(api, remotedir, share_id, file_ids, password=password)
 
 
@@ -171,28 +160,26 @@
     password: str = "",
     file_ids: List[str] = [],
     desc: bool = False,
     name: bool = False,
     time: bool = False,
     size: bool = False,
     all: bool = True,
-    limit: int = 100,
+    limit: int = 200,
     recursive: bool = False,
     sifters: List[Sifter] = [],
     highlight: bool = False,
     show_size: bool = False,
     show_date: bool = False,
     show_file_id: bool = False,
     show_hash: bool = False,
     show_absolute_path: bool = False,
     csv: bool = False,
 ):
-    assert int(bool(share_id)) ^ int(
-        bool(share_url)
-    ), "`share_id` and `share_url` only can be given one"
+    assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
         if not file_ids:
             file_id = _extract_file_id(share_url)
@@ -224,17 +211,15 @@
         show_file_id=show_file_id,
         show_hash=show_hash,
         show_absolute_path=show_absolute_path,
         csv=csv,
     )
 
 
-def remotepath_exists(
-    api: AliPCSApi, name: str, rd: str, _cache: Dict[str, Set[str]] = {}
-) -> bool:
+def remotepath_exists(api: AliPCSApi, name: str, rd: str, _cache: Dict[str, Set[str]] = {}) -> bool:
     names = _cache.get(rd)
     if not names:
         names = set([sp.name for sp in api.list_path_iter(rd)])
         _cache[rd] = names
     return name in names
 
 
@@ -250,17 +235,15 @@
     recursive: bool = False,
     from_index: int = 0,
     downloader: Downloader = DEFAULT_DOWNLOADER,
     downloadparams: DownloadParams = DEFAULT_DOWNLOADPARAMS,
     out_cmd: bool = False,
     encrypt_password: bytes = b"",
 ):
-    assert int(bool(share_id)) ^ int(
-        bool(share_url)
-    ), "`share_id` and `share_url` only can be given one"
+    assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
         if not file_ids:
             file_id = _extract_file_id(share_url)
@@ -303,17 +286,15 @@
     player_params: List[str] = [],
     quiet: bool = False,
     shuffle: bool = False,
     ignore_ext: bool = False,
     out_cmd: bool = False,
     local_server: str = "",
 ):
-    assert int(bool(share_id)) ^ int(
-        bool(share_url)
-    ), "`share_id` and `share_url` only can be given one"
+    assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
         if not file_ids:
             file_id = _extract_file_id(share_url)
@@ -340,20 +321,16 @@
         shuffle=shuffle,
         ignore_ext=ignore_ext,
         out_cmd=out_cmd,
         local_server=local_server,
     )
 
 
-def get_share_token(
-    api: AliPCSApi, share_id: str, share_url: str = "", password: str = ""
-) -> str:
-    assert int(bool(share_id)) ^ int(
-        bool(share_url)
-    ), "`share_id` and `share_url` only can be given one"
+def get_share_token(api: AliPCSApi, share_id: str, share_url: str = "", password: str = "") -> str:
+    assert int(bool(share_id)) ^ int(bool(share_url)), "`share_id` and `share_url` only can be given one"
 
     share_url = _redirect(share_url)
 
     if share_url:
         share_id = _extract_share_id(share_url)
 
     assert share_id
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/sifter.py` & `alipcs_py-0.6.0/alipcs_py/commands/sifter.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,24 +85,17 @@
 
 
 T = TypeVar("T", PcsFile, str)
 
 
 def sift(objs: List[T], sifters: List[Sifter], recursive: bool = False) -> List[T]:
     if sifters:
-
         obj_dirs: List[T]
         if recursive:
             # If it is recursive, we ignore to sift dirs.
             obj_dirs = [o for o in objs if isinstance(o, PcsFile) and o.is_dir]
-            objs = [
-                o
-                for o in objs
-                if not isinstance(o, PcsFile) or isinstance(o, PcsFile) and o.is_file
-            ]
+            objs = [o for o in objs if not isinstance(o, PcsFile) or isinstance(o, PcsFile) and o.is_file]
         else:
             obj_dirs = []
 
-        objs = obj_dirs + [
-            obj for obj in objs if all([sifter(obj) for sifter in sifters])
-        ]
+        objs = obj_dirs + [obj for obj in objs if all([sifter(obj) for sifter in sifters])]
     return objs
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/sync.py` & `alipcs_py-0.6.0/alipcs_py/commands/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,29 +54,24 @@
             fts.append(FromTo(localpath, join_path(remotedir, path)))
         else:
             check_list.append((localpath, all_pcs_files[path]))
 
     for lp, pf in check_list:
         sha1 = calc_sha1(Path(lp).open("rb"))
 
-        if (
-            pf.rapid_upload_info
-            and sha1.lower() != pf.rapid_upload_info.content_hash.lower()
-        ):
+        if pf.rapid_upload_info and sha1.lower() != pf.rapid_upload_info.content_hash.lower():
             fts.append(FromTo(lp, pf.path))
 
     need_deleted_file_ids = []
     for rp in all_pcs_files.keys():
         if rp not in all_localpaths:
             need_deleted_file_ids.append(all_pcs_files[rp].file_id)
 
     logger.debug(
-        "`sync`: all localpaths: %s, "
-        "localpaths needed to upload: %s, "
-        "remotepaths needed to delete: %s",
+        "`sync`: all localpaths: %s, localpaths needed to upload: %s, remotepaths needed to delete: %s",
         len(all_localpaths),
         len(fts),
         len(need_deleted_file_ids),
     )
 
     _upload(
         api,
```

### Comparing `alipcs_py-0.5.3/alipcs_py/commands/upload.py` & `alipcs_py-0.6.0/alipcs_py/commands/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,17 +186,15 @@
             slice_size=slice_size,
             show_progress=show_progress,
             user_id=user_id,
             user_name=user_name,
         )
 
 
-def _need_to_upload(
-    api: AliPCSApi, remotepath: str, check_name_mode: CheckNameMode
-) -> bool:
+def _need_to_upload(api: AliPCSApi, remotepath: str, check_name_mode: CheckNameMode) -> bool:
     """Check wether the `remotepath` needs to be uploaded
 
     If `check_name_mode` is `refuse` and the `remotepath` exists, then it does not need to be uploaded.
     """
 
     try:
         pcs_file = api.path(remotepath)
@@ -338,17 +336,15 @@
 
     filename = posix_path_basename(remotepath)
 
     if not _need_to_upload(api, remotepath, check_name_mode):
         remove_progress_task(task_id)
         return
 
-    info = _init_encrypt_io(
-        localpath, encrypt_password=encrypt_password, encrypt_type=encrypt_type
-    )
+    info = _init_encrypt_io(localpath, encrypt_password=encrypt_password, encrypt_type=encrypt_type)
     encrypt_io, encrypt_io_len, local_ctime, local_mtime = info
     slice_size = adjust_slice_size(slice_size, encrypt_io_len)
     part_number = math.ceil(encrypt_io_len / slice_size)
 
     # Progress bar
     if task_id is not None and progress_task_exists(task_id):
         _progress.update(task_id, total=encrypt_io_len)
@@ -455,17 +451,15 @@
                 size = min(slice_size, encrypt_io_len - i)
                 if size == 0:
                     break
 
                 data = encrypt_io.read(size)
                 io = BytesIO(data or b"")
 
-                fut = executor.submit(
-                    sure_release, semaphore, _upload_slice, (io, upload_url)
-                )
+                fut = executor.submit(sure_release, semaphore, _upload_slice, (io, upload_url))
                 futs.append(fut)
 
                 i += size
 
             as_completed(futs)
 
         file_id = pcs_prepared_file.file_id
@@ -583,17 +577,15 @@
 
     filename = posix_path_basename(remotepath)
 
     if not _need_to_upload(api, remotepath, check_name_mode):
         remove_progress_task(task_id)
         return
 
-    info = _init_encrypt_io(
-        localpath, encrypt_password=encrypt_password, encrypt_type=encrypt_type
-    )
+    info = _init_encrypt_io(localpath, encrypt_password=encrypt_password, encrypt_type=encrypt_type)
     encrypt_io, encrypt_io_len, local_ctime, local_mtime = info
     slice_size = adjust_slice_size(slice_size, encrypt_io_len)
     part_number = math.ceil(encrypt_io_len / slice_size)
 
     # Progress bar
     if task_id is not None and progress_task_exists(task_id):
         _progress.update(task_id, total=encrypt_io_len)
@@ -656,28 +648,24 @@
             )
 
         reset_encrypt_io(encrypt_io)
 
         for upload_url in pcs_prepared_file.upload_urls():
             _wait_start()
 
-            logger.debug(
-                "`upload_file`: upload_slice: slice_completed: %s", slice_completed
-            )
+            logger.debug("`upload_file`: upload_slice: slice_completed: %s", slice_completed)
 
             size = min(slice_size, encrypt_io_len - slice_completed)
             if size == 0:
                 break
 
             data = encrypt_io.read(size) or b""
             io = BytesIO(data)
 
-            logger.debug(
-                "`upload_file`: upload_slice: size should be %s == %s", size, len(data)
-            )
+            logger.debug("`upload_file`: upload_slice: size should be %s == %s", size, len(data))
 
             # Retry upload until success
             retry(
                 -1,
                 except_callback=lambda err, fail_count: (
                     io.seek(0, 0),
                     logger.warning(
```

### Comparing `alipcs_py-0.5.3/alipcs_py/common/cache.py` & `alipcs_py-0.6.0/alipcs_py/common/cache.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/concurrent.py` & `alipcs_py-0.6.0/alipcs_py/common/concurrent.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/crypto.py` & `alipcs_py-0.6.0/alipcs_py/common/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         cmd = ["md5sum", localpath]
     else:  # windows
         cmd = ["CertUtil", "-hashfile", localpath, "MD5"]
     return cmd
 
 
 def calc_file_md5(localpath: str) -> str:
-    cp = subprocess.run(
-        _md5_cmd(localpath), universal_newlines=True, stdout=subprocess.PIPE
-    )
+    cp = subprocess.run(_md5_cmd(localpath), universal_newlines=True, stdout=subprocess.PIPE)
 
     output = cp.stdout.strip()
     if IS_MACOS:
         return re.split(r"\s+", output)[-1]
     elif IS_LINUX:
         return re.split(r"\s+", output)[0]
     else:  # windows
@@ -62,17 +60,15 @@
             md5_v.update(buf)
             crc32_v = crc32(buf, crc32_v).conjugate()
         else:
             break
     return crc32_v.conjugate() & 0xFFFFFFFF, md5_v.hexdigest()
 
 
-def calc_hash(
-    hash_method: Callable, buf: Union[str, bytes, IO, BufferedReader], encoding="utf-8"
-) -> str:
+def calc_hash(hash_method: Callable, buf: Union[str, bytes, IO, BufferedReader], encoding="utf-8") -> str:
     assert isinstance(buf, (str, bytes, IO, BufferedReader))
 
     if isinstance(buf, str):
         buf = buf.encode(encoding)
         return hash_method(buf).hexdigest()
     elif isinstance(buf, bytes):
         return hash_method(buf).hexdigest()
@@ -118,17 +114,15 @@
 
 def random_sys_bytes(size: int) -> bytes:
     """Generate random bytes with `os.urandom`"""
 
     return os.urandom(size)
 
 
-def padding_key(
-    key: Union[str, bytes], length: int = 0, value: bytes = b"\xff"
-) -> bytes:
+def padding_key(key: Union[str, bytes], length: int = 0, value: bytes = b"\xff") -> bytes:
     """padding key with `value`"""
 
     assert len(value) < 2
 
     if isinstance(key, str):
         key = key.encode("utf-8")
```

### Comparing `alipcs_py-0.5.3/alipcs_py/common/date.py` & `alipcs_py-0.6.0/alipcs_py/common/date.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,12 +19,8 @@
     if len(date_string) == 20:
         return int(datetime.strptime(date_string, "%Y-%m-%dT%H:%M:%S%z").timestamp())
     else:
         return int(datetime.strptime(date_string, "%Y-%m-%dT%H:%M:%S.%f%z").timestamp())
 
 
 def timestamp_to_iso_8601(timestamp: int) -> str:
-    return (
-        datetime.fromtimestamp(timestamp, timezone.utc)
-        .isoformat()
-        .replace("+00:00", ".000Z")
-    )
+    return datetime.fromtimestamp(timestamp, timezone.utc).isoformat().replace("+00:00", ".000Z")
```

### Comparing `alipcs_py-0.5.3/alipcs_py/common/downloader.py` & `alipcs_py-0.6.0/alipcs_py/common/downloader.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/event.py` & `alipcs_py-0.6.0/alipcs_py/common/event.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/file_type.py` & `alipcs_py-0.6.0/alipcs_py/common/file_type.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/io.py` & `alipcs_py-0.6.0/alipcs_py/common/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,23 +232,19 @@
         #
         # Only define it at __init__
         self._total_origin_len = total_origin_len
 
         self._encrypt_password = encrypt_password
 
         self._salt_for_head = generate_salt()
-        self._encrypt_key_for_head, self._iv_for_head = generate_key_iv(
-            encrypt_password, self._salt_for_head, 32, 16
-        )
+        self._encrypt_key_for_head, self._iv_for_head = generate_key_iv(encrypt_password, self._salt_for_head, 32, 16)
 
         # `self._encrypt_key`,`self._nonce_or_iv` is for cryptography
         self._salt = generate_salt()
-        self._encrypt_key, self._nonce_or_iv = generate_key_iv(
-            encrypt_password, self._salt, 32, 16
-        )
+        self._encrypt_key, self._nonce_or_iv = generate_key_iv(encrypt_password, self._salt, 32, 16)
 
         # Cryptography
         #
         # Instantiated at each subclass, here is for mypy
         self._crypto: Cryptography
 
         self._total_head: bytes
@@ -307,16 +303,15 @@
             + u64_to_u8x8(self._total_origin_len),
             PADDED_ENCRYPT_HEAD_LEN,
             value=b"",
         )
 
         # AES256CBC Encrypt head
         self._total_head = (
-            aes256cbc_encrypt(ori_head, self._encrypt_key_for_head, self._iv_for_head)
-            + self._salt_for_head
+            aes256cbc_encrypt(ori_head, self._encrypt_key_for_head, self._iv_for_head) + self._salt_for_head
         )
         return self._total_head
 
     def __len__(self) -> int:
         return self._total_head_len + self._io_len
 
     def read(self, size: int = -1) -> Optional[bytes]:
@@ -336,29 +331,22 @@
         else:
             io_buf = self._io.read(size)
             data = self._crypto.encrypt(io_buf)
         self._offset += len(data)
         return data
 
     def seek(self, offset: int, whence: int = 0) -> int:
-        if (
-            not self.seekable()
-            and offset == 0
-            and whence == 0
-            and self._total_head_len > 0
-        ):
+        if not self.seekable() and offset == 0 and whence == 0 and self._total_head_len > 0:
             self._crypto.reset()
             self._io.seek(0, 0)
             self._offset = 0
             return self._offset
 
         if not self.seekable():
-            raise ValueError(
-                f"{self._crypto.__class__.__name__} is not support seeking"
-            )
+            raise ValueError(f"{self._crypto.__class__.__name__} is not support seeking")
 
         if whence == 0:
             if offset < 0:
                 raise ValueError(f"Negative seek position {offset}")
             pass
         elif whence == 1:
             offset += self._offset
@@ -481,26 +469,23 @@
         data = self._io.read(size) or b""
         if not data:
             return
 
         self._origin_io_offset += len(data)
         self._origin_cache.extend(data)
 
-        avail_ori_len = padding_size(
-            len(self._origin_cache), self.BLOCK_SIZE, ceil=False
-        )
+        avail_ori_len = padding_size(len(self._origin_cache), self.BLOCK_SIZE, ceil=False)
         if avail_ori_len > 0:
             ori_cn = self._origin_cache[:avail_ori_len]
             self._origin_cache = self._origin_cache[avail_ori_len:]
         else:
             ori_cn = b""
 
         # The end encryption
         if self._origin_io_offset == self._total_origin_len:
-
             # Take all remainder
             if self._origin_cache:
                 ori_cn += bytes(self._origin_cache)
                 self._origin_cache.clear()
 
             # Padding
             if self._need_data_padded:
@@ -542,17 +527,15 @@
         return data
 
     def seekable(self) -> bool:
         return False
 
 
 class DecryptIO(IO):
-    def __init__(
-        self, io: IO, encrypt_key: bytes, nonce_or_iv: bytes, total_origin_len: int
-    ):
+    def __init__(self, io: IO, encrypt_key: bytes, nonce_or_iv: bytes, total_origin_len: int):
         self._io = io
 
         # The offset after ENCRYPT_HEAD_LEN
         # Must be equal ENCRYPT_HEAD_LEN
         #
         # When `self.set_io` be called, the `_io_init_offset` must be set to `io.tell()`
         self._io_init_offset = io.tell()
@@ -680,17 +663,15 @@
 
         self._encrypted_cache = bytearray()
         self._decrypted_cache = bytearray()
 
     def __len__(self) -> int:
         """The decrypted content length of `self._io`"""
 
-        avail_enc_len = padding_size(
-            self._io_len - self._io_init_offset, self.BLOCK_SIZE, ceil=False
-        )
+        avail_enc_len = padding_size(self._io_len - self._io_init_offset, self.BLOCK_SIZE, ceil=False)
         return avail_enc_len
 
     def _read_block(self, size: int = -1):
         """Read encrypted block to cache"""
 
         # `self._decrypted_cache` has remains.
         if size > 0 and len(self._decrypted_cache) > size:
@@ -703,17 +684,15 @@
         data = self._io.read(size)
         if not data:
             return
 
         self._encrypted_io_offset += len(data)
         self._encrypted_cache.extend(data)
 
-        avail_enc_len = padding_size(
-            len(self._encrypted_cache), self.BLOCK_SIZE, ceil=False
-        )
+        avail_enc_len = padding_size(len(self._encrypted_cache), self.BLOCK_SIZE, ceil=False)
         if avail_enc_len > 0:
             enc_cn = bytes(self._encrypted_cache[:avail_enc_len])
             self._encrypted_cache = self._encrypted_cache[avail_enc_len:]
         else:
             enc_cn = b""
 
         # The end decryption
@@ -755,17 +734,15 @@
         head[:i],
         head[i : i + 1],  # magic_code
         head[i + 1 : i + 1 + 16],  # salt + random padding
         head[i + 1 + 16 : i + 1 + 16 + 8],  # total_origin_len
     )
 
 
-def _decryptio_version1(
-    total_head: bytes, io: IO, encrypt_password: bytes
-) -> Optional[DecryptIO]:
+def _decryptio_version1(total_head: bytes, io: IO, encrypt_password: bytes) -> Optional[DecryptIO]:
     encrypt_password = padding_key(encrypt_password, 32)
 
     if len(total_head) < ENCRYPT_HEAD_LEN:
         return None
 
     # Version 1
     b_mc, magic_code, nonce_or_iv, total_origin_len_ = parse_head(total_head)
@@ -782,28 +759,24 @@
     elif magic_code == AES256CBCEncryptIO.MAGIC_CODE:
         return AES256CBCDecryptIO(io, encrypt_password, nonce_or_iv, total_origin_len)
     else:
         logging.warning(f"Unknown magic_code: {magic_code!r}")
         return None
 
 
-def _decryptio_version3(
-    total_head: bytes, io: IO, encrypt_password: bytes
-) -> Optional[DecryptIO]:
+def _decryptio_version3(total_head: bytes, io: IO, encrypt_password: bytes) -> Optional[DecryptIO]:
     if len(total_head) < PADDED_ENCRYPT_HEAD_WITH_SALT_LEN:
         return None
 
     enc_head, salt_for_head = (
         total_head[:PADDED_ENCRYPT_HEAD_LEN],
         total_head[PADDED_ENCRYPT_HEAD_LEN:],
     )
 
-    encrypt_key_for_head, iv_for_head = generate_key_iv(
-        encrypt_password, salt_for_head, 32, 16
-    )
+    encrypt_key_for_head, iv_for_head = generate_key_iv(encrypt_password, salt_for_head, 32, 16)
 
     head = aes256cbc_decrypt(enc_head, encrypt_key_for_head, iv_for_head)
 
     b_mc, magic_code, padding_salt, total_origin_len_ = parse_head(head)
     total_origin_len = u8x8_to_u64(total_origin_len_)
 
     salt = padding_salt[:8]
@@ -933,30 +906,24 @@
     def _parse_crypto(self):
         if self._encrypt_password:
             with self._request((0, PADDED_ENCRYPT_HEAD_WITH_SALT_LEN - 1)) as resp:
                 raw_data = resp.raw.read()
                 if len(raw_data) == PADDED_ENCRYPT_HEAD_WITH_SALT_LEN:
                     self._dio = to_decryptio(BytesIO(raw_data), self._encrypt_password)
                     self._has_encrypted = isinstance(self._dio, DecryptIO)
-                    self._total_head_len = (
-                        cast(DecryptIO, self._dio)._total_head_len
-                        if self._has_encrypted
-                        else 0
-                    )
+                    self._total_head_len = cast(DecryptIO, self._dio)._total_head_len if self._has_encrypted else 0
         self._parsed = True
 
     def _request(self, _range: Tuple[int, int]) -> Response:
         headers = dict(self._headers or {})
         headers["Range"] = "bytes={}-{}".format(*_range)
 
         while True:
             try:
-                resp = self._session.request(
-                    self._method, self._url, headers=headers, **self._kwargs
-                )
+                resp = self._session.request(self._method, self._url, headers=headers, **self._kwargs)
                 if not resp.ok:
                     logger.warning(
                         "`%s._request` request error: status_code: %s, body: %s",
                         self.__class__.__name__,
                         resp.status_code,
                         resp.content[:1000],
                     )
@@ -1009,17 +976,15 @@
 
         if start != self._decrypted_count and not self.rangeable():
             raise IndexError(
                 "ChaCha20 must decoded data with continue data."
                 f"start: {start}, decrypted count: {self._decrypted_count}"
             )
 
-        ranges = self._split_chunk(
-            start + self._total_head_len, end + self._total_head_len
-        )
+        ranges = self._split_chunk(start + self._total_head_len, end + self._total_head_len)
         for _rg in ranges:
             with self._request(_rg) as resp:
                 stream = resp.raw
                 while True:
                     buf = stream.read(READ_SIZE)
                     if not buf:
                         break
```

### Comparing `alipcs_py-0.5.3/alipcs_py/common/keyboard.py` & `alipcs_py-0.6.0/alipcs_py/common/keyboard.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/log.py` & `alipcs_py-0.6.0/alipcs_py/common/log.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/net.py` & `alipcs_py-0.6.0/alipcs_py/common/net.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/path.py` & `alipcs_py-0.6.0/alipcs_py/common/path.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/progress_bar.py` & `alipcs_py-0.6.0/alipcs_py/common/progress_bar.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/common/simple_cipher.pyx` & `alipcs_py-0.6.0/alipcs_py/common/simple_cipher.pyx`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/config/__init__.py` & `alipcs_py-0.6.0/alipcs_py/config/__init__.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/alipcs_py/storage/store.py` & `alipcs_py-0.6.0/alipcs_py/storage/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Tuple, List, Any
 
 from peewee import SQL
 
-from alipcs_py.alipcs.api import AliPCSApi
+from alipcs_py.alipcs.api import AliPCSApiMix
 from alipcs_py.alipcs.inner import PcsSharedLinkInfo, PcsFile
 from alipcs_py.storage.tables import PcsSharedLinkInfoTable, PcsFileTable
 
 
 class SharedStore:
     def __init__(self) -> None:
         pass
@@ -16,18 +16,15 @@
         if ins:
             return ins.to_pcs()
         else:
             return None
 
     def add_shared_link_info(self, pcs_shared_link_info: PcsSharedLinkInfo) -> Any:
         pcs_shared_link_info_ins, _ = PcsSharedLinkInfoTable.get_or_create(
-            **{
-                k: getattr(pcs_shared_link_info, k)
-                for k in pcs_shared_link_info.__dataclass_fields__
-            }
+            **{k: getattr(pcs_shared_link_info, k) for k in pcs_shared_link_info.__dataclass_fields__}
         )
         return pcs_shared_link_info_ins
 
     def add_shared_file(self, share_id: str, pcs_file: PcsFile) -> Any:
         if PcsFileTable.get_or_none(file_id=pcs_file.file_id):
             # The file exists
             return
@@ -37,28 +34,24 @@
         pcs_file_ins, _ = PcsFileTable.get_or_create(
             **{k: getattr(pcs_file, k) for k in pcs_file.__dataclass_fields__},
             shared_link_info_id=pcs_shared_link_info_ins.id,
         )
         return pcs_file_ins
 
     def delete_shared_links(self, *share_ids: str) -> None:
-        PcsSharedLinkInfoTable.delete().where(
-            PcsSharedLinkInfoTable.share_id.in_(share_ids)
-        ).execute()
+        PcsSharedLinkInfoTable.delete().where(PcsSharedLinkInfoTable.share_id.in_(share_ids)).execute()
 
     def delete_shared_files(self, *file_ids: str) -> None:
         PcsFileTable.delete().where(PcsFileTable.file_id.in_(file_ids)).execute()
 
     def search_shared_links(
         self, *keywords: str, fields: List[str] = ["share_name", "display_name"]
     ) -> List[PcsSharedLinkInfo]:
         sql = " OR ".join([f"`{f}` like ?" for f in fields * len(keywords)])
-        query = PcsSharedLinkInfoTable.select().where(
-            SQL(sql, [f"%{keyword}%" for keyword in keywords] * len(fields))
-        )
+        query = PcsSharedLinkInfoTable.select().where(SQL(sql, [f"%{keyword}%" for keyword in keywords] * len(fields)))
         return [item.to_pcs() for item in query]
 
     def search_shared_files(
         self,
         *keywords: str,
         fields: List[str] = ["name", "path"],
         share_ids: List[str] = [],
@@ -70,17 +63,15 @@
         )
         if share_ids:
             query = query.where(
                 PcsSharedLinkInfoTable.share_id.in_(share_ids)
                 & SQL(sql, [f"%{keyword}%" for keyword in keywords] * len(fields))
             )
         else:
-            query = query.where(
-                SQL(sql, [f"%{keyword}%" for keyword in keywords] * len(fields))
-            )
+            query = query.where(SQL(sql, [f"%{keyword}%" for keyword in keywords] * len(fields)))
         return [(item.to_pcs(), item.shared_link_info_id.to_pcs()) for item in query]
 
     def list_shared_links(
         self,
         by_id: bool = False,
         by_name: bool = False,
         limit: int = 100,
@@ -123,18 +114,18 @@
         # If limit is 0, selecting all items
         if limit > 0:
             query = query.limit(limit).offset(offset)
 
         return [(item.to_pcs(), item.shared_link_info_id.to_pcs()) for item in query]
 
 
-class AliPCSApiWithSharedStore(AliPCSApi):
-    """AliPCS API with SharedStore
+class AliPCSApiMixWithSharedStore(AliPCSApiMix):
+    """AliPCS API Mix with SharedStore
 
-    Hooking the `AliPCSApi.list` to store the shared file infos
+    Hooking the `AliPCSApiMix.list` to store the shared file infos
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._sharedstore: Optional[SharedStore] = None
```

### Comparing `alipcs_py-0.5.3/alipcs_py/storage/tables.py` & `alipcs_py-0.6.0/alipcs_py/storage/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,15 @@
         pcs_item = self.pcs_item()
         data: Dict[str, Any] = {}
         columns = self.__class__._meta.columns  # type: ignore
         pcs_fields = pcs_item.__dataclass_fields__
         for col in columns.keys():
             if col in pcs_fields:
                 val = getattr(self, col)
-                if (
-                    pcs_fields[col].type == typing.Optional[bool]
-                    or pcs_fields[col].type == bool
-                ):
+                if pcs_fields[col].type == typing.Optional[bool] or pcs_fields[col].type == bool:
                     if val == None:
                         data[col] = None
                     else:
                         data[col] = bool(val)
                 else:
                     data[col] = val
         return pcs_item(**data)
```

### Comparing `alipcs_py-0.5.3/alipcs_py/utils.py` & `alipcs_py-0.6.0/alipcs_py/utils.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/build.py` & `alipcs_py-0.6.0/build.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.5.3/pyproject.toml` & `alipcs_py-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 [tool.poetry]
 name = "AliPCS-Py"
 homepage = "https://github.com/PeterDing/AliPCS-Py"
-version = "0.5.3"
+version = "0.6.0"
 description = "Ali Pcs Api and App"
 authors = ["PeterDing <dfhayst@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 build = "build.py"
 
+[tool.black]
+line-length = 119
+
+[tool.ruff]
+ignore = ["E501", "F401", "F841"]
+line-length = 119
+
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = ">=2.28"
 requests-toolbelt = ">=0.10"
 peewee = ">=3.15"
 toml = ">=0.10"
+qrcode = ">=7.4"
 rich = ">=12.6"
 pillow = ">=9.3"
 click = ">=8.1"
 typing-extensions = ">=4.4"
 aget = ">=0.1"
 chardet = ">=5.0"
 fastapi = ">=0.87"
```

### Comparing `alipcs_py-0.5.3/setup.py` & `alipcs_py-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,37 +21,38 @@
  'cython>=0.29',
  'ecdsa>=0.18',
  'fastapi>=0.87',
  'jinja2>=3.1',
  'passlib>=1.7',
  'peewee>=3.15',
  'pillow>=9.3',
+ 'qrcode>=7.4',
  'requests-toolbelt>=0.10',
  'requests>=2.28',
  'rich>=12.6',
  'toml>=0.10',
  'typing-extensions>=4.4',
  'uvicorn>=0.19']
 
 entry_points = \
 {'console_scripts': ['AliPCS-Py = alipcs_py.app:main']}
 
 setup_kwargs = {
     'name': 'alipcs-py',
-    'version': '0.5.3',
+    'version': '0.6.0',
     'description': 'Ali Pcs Api and App',
-    'long_description': '# AliPCS-Py\n\n**2023-02-15 使用临时 API 接口，让下载可用。**\n\n**2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**\n\n[![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)\n![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)\n\nAn AliPCS API and An App\n\nAliPCS-Py 是阿里云盘的非官方 api 和一个命令行运用程序。\n\n---\n\n## 百度云盘 api 和 命令行客户端在 https://github.com/PeterDing/BaiduPCS-Py\n\n---\n\n- [安装](#安装)\n- [更新](#更新)\n- [API](#API)\n- [用法](#用法)\n- [命令别名](#命令别名)\n- [对多个帐号进行相同操作](#对多个帐号进行相同操作)\n\n#### 用户相关命令\n\n- [添加用户](#添加用户)\n- [显示当前用户的信息](#显示当前用户的信息)\n- [更新用户信息](#更新用户信息)\n- [显示所有用户](#显示所有用户)\n- [切换当前用户](#切换当前用户)\n- [删除一个用户](#删除一个用户)\n- [显示当前工作目录](#显示当前工作目录)\n- [切换当前工作目录](#切换当前工作目录)\n\n#### 无感加密解密文件\n\n- [设置文件加密密码](#设置文件加密密码)\n\n#### 文件操作相关命令\n\n- [文件操作](#文件操作)\n- [列出网盘路径下的文件](#列出网盘路径下的文件)\n- [搜索文件](#搜索文件)\n- [显示文件内容](#显示文件内容)\n- [创建目录](#创建目录)\n- [移动文件](#移动文件)\n- [文件重命名](#文件重命名)\n- [拷贝文件](#拷贝文件)\n- [删除文件](#删除文件)\n- [下载文件或目录](#下载文件或目录)\n- [播放媒体文件](#播放媒体文件)\n- [上传文件](#上传文件)\n- [同步本地目录到远端](#同步本地目录到远端)\n\n#### 秒传\n\n- [关于秒传连接](#关于秒传连接)\n\n#### 分享相关命令\n\n- [分享文件](#分享文件)\n- [列出分享链接](#列出分享链接)\n- [取消分享链接](#取消分享链接)\n- [列出其他用户分享链接中的文件](#列出其他用户分享链接中的文件)\n- [下载他人分享的文件](#下载他人分享的文件)\n- [播放他人分享的文件](#播放他人分享的文件)\n- [保存其他用户分享的链接](#保存其他用户分享的链接)\n\n#### 本地保存分享连接\n\n- [保存分享连接至本地](#保存分享连接至本地)\n- [显示本地保存的分享连接](#显示本地保存的分享连接)\n- [显示本地保存的分享文件](#显示本地保存的分享文件)\n- [查找本地保存的分享连接](#查找本地保存的分享连接)\n- [查找本地保存的分享文件](#查找本地保存的分享文件)\n- [查找本地保存的分享连接和文件](#查找本地保存的分享连接和文件)\n- [删除本地保存的分享连接或文件](#删除本地保存的分享连接或文件)\n- [清理本地保存的无效分享连接](#清理本地保存的无效分享连接)\n\n#### HTTP 服务\n\n- [开启 HTTP 服务](#开启-HTTP-服务)\n\n## 安装\n\n需要 Python 版本大于或等于 3.7\n\n```\npip3 install Cython\npip3 install AliPCS-Py\n```\n\n### Windows 依赖\n\n在 Windows 上，AliPCS-Py 依赖 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)。\n\n在安装 AliPCS-Py 前，请先安装 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)，再在其中勾选 `C++ 生成工具` 并安装。完成后即可安装 AliPCS-Py。\n\n## 更新\n\n```\npip3 install AliPCS-Py --upgrade\n```\n\n## API\n\nAliPCS-Py 的阿里云盘 API 只依赖 requests，方便用户开发自己的运用。\n\n```python\nfrom alipcs_py.alipcs import AliPCSApi\n\napi = AliPCSApi(refresh_token)\n```\n\n## 用法\n\n```\nAliPCS-Py --help\n```\n\n## 命令别名\n\n可以用下面的命令别名代替原来的命令名。\n\n| 别名 | 原名         |\n| ---- | ------------ |\n| w    | who          |\n| uu   | updateuser   |\n| su   | su           |\n| ul   | userlist     |\n| ua   | useradd      |\n| ep   | encryptpwd   |\n| ud   | userdel      |\n| l    | ls           |\n| f    | search       |\n| md   | mkdir        |\n| mv   | move         |\n| rn   | rename       |\n| cp   | copy         |\n| rm   | remove       |\n| d    | download     |\n| p    | play         |\n| u    | upload       |\n| sn   | sync         |\n| S    | share        |\n| sl   | shared       |\n| cs   | cancelshared |\n| s    | save         |\n| sv   | server       |\n\n## 对多个帐号进行相同操作\n\nAliPCS-Py 支持对多个帐号进行相同操作。比如，用相同关键字搜索多个帐号，上传相同的文件/目录到多个帐号，等等。\n\n使用者只需用 `--users` 选项来指定要操作的帐号名即可。\n\n`--users` 接受一个参数，这个参数是用“,”连接的要进行操作帐号名的部分字符。假设我们现在有 3 个帐号，帐号名分别是 `Tom`，`Peter`，`Joy`。\n现在我要同时对`Tom`和`Joy`进行关键字搜索。我们可以用下面的命令进行：\n\n```\nAliPCS-Py --users \'Tom,Joy\' search \'keyword\' / -R\n```\n\n或者给出帐号名的部分片段：\n\n```\nAliPCS-Py --users \'om,oy\' search \'keyword\' / -R\n```\n\n更简单可以用：\n\n```\n# Tom, Joy 都包含字符 "o"\nAliPCS-Py --users \'o\' search \'keyword\' / -R\n```\n\n如果要对所有帐号进行操作用 `--users \'\'`。\n\n如果不使用 `--users` 选项，默认只对当前帐号进行操作。\n\n以下命令支持对多个帐号进行操作：\n\n- pwd\n- ls\n- search\n- cat\n- mkdir\n- move\n- rename\n- copy\n- remove\n- download\n- play\n- upload\n- sync\n- share\n- shared\n- cancelshared\n- save\n- server\n\n**注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。\n\n## 添加用户\n\nAliPCS-Py 目前支持用`refresh_token`登录。需要使用者在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。\n\n使用者可以用下面的方式获取用户的 `refresh_token` 值。\n\n1. 登录 https://www.aliyundrive.com/drive/\n2. 打开浏览器的开发者工具(如 Chrome DevTools)。\n3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。\n\n![refresh_token](./imgs/refresh_token.png)\n\n现在找到了 `refresh_token` 值，我们可以用下面的命令添加一个用户。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --refresh-token "..."\n```\n\nAliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。\n\n## 显示当前用户的信息\n\n```\nAliPCS-Py who\n```\n\n或者：\n\n```\nAliPCS-Py who user_id\n```\n\n指明显示用户 id 为 `user_id` 的用户信息。\n\n### 选项\n\n| Option                      | Description  |\n| --------------------------- | ------------ |\n| -K, --show-encrypt-password | 显示加密密码 |\n\n## 更新用户信息\n\n默认更新当前用户信息。\n\n```\nAliPCS-Py updateuser\n```\n\n也可指定多个 `user_id`\n\n```\nAliPCS-Py updateuser user_id\n```\n\n## 显示所有用户\n\n```\nAliPCS-Py userlist\n```\n\n## 切换当前用户\n\n```\nAliPCS-Py su\n```\n\n或者指定用户列表中用户所在的位置：\n\n```\nAliPCS-Py su 2\n```\n\n## 删除一个用户\n\n```\nAliPCS-Py userdel\n```\n\n## 设置文件加密密码\n\nAliPCS-Py 支持“无感的”文件加密。\n\nAliPCS-Py 可以加密上传文件，在下载的时候自动解密，让使用者感觉不到加密解密的过程。\n\n如果使用者需要将保密文件上传至阿里云盘保存，可以使用这个方法。即使帐号被盗，攻击者也无法还原文件内容。\n\nAliPCS-Py 支持以下加密方法：\n\n- **Simple** 一种简单的加密算法。根据密钥生成一个字节对照表来加密解密文件。\n  速度快，但**不安全**，不建议加密重要文件。\n  因为这种算法加解密不需要知道上下文信息，所以，下载时支持分段下载，如果是媒体文件则支持拖动播放。\n  推荐用于加密不重要的媒体文件。\n- **ChaCha20** 工业级加密算法，速度快，推荐用于加密重要文件。不支持分段下载。\n- **AES256CBC** 工业级加密算法，推荐用于加密重要文件。不支持分段下载。\n\n**注意**：用命令 `encryptpwd` 设置的密码**只是为当前用户**的。\n\n为当前用户设置加密密码:\n\n交互添加：\n\n```\nAliPCS-Py encryptpwd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py encryptpwd --encrypt-password \'my-encrypt-password\'\n```\n\n上传并加密文件：\n\n上传和同步文件时只需要指定加密算法就可。如果不指定就不加密。\n\n```\n# 默认使用上面设置的 `encrypt-password`\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type AES256CBC\n```\n\n下载并用上面设置的 `encrypt-password` 自动解密文件：\n\n```\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/\n```\n\n也可以使用临时的 `encrypt-password`：\n\n```\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type Simple --encrypt-password \'onlyyou\'\n```\n\n但在使用临时的 `encrypt-password` 后，`cat`、下载和播放这些文件时需要指定 `encrypt-password`，但不需要指定加密算法，程序会自动检查加密算法：\n\n```\n# 下载\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/  --encrypt-password \'onlyyou\'\n\n# 开启本地服务并播放\nAliPCS-Py play /to/here/some-file.mp4 --encrypt-password \'onlyyou\' --use-local-server\n```\n\n显示当前用户的密钥：\n\n```\nAliPCS-Py who --show-encrypt-password\n```\n\nAliPCS-Py 下载时默认会解密文件，如果想要下载但不解密文件，需要加 `--no-decrypt`\n\n```\nAliPCS-Py download some-file --no-decrypt\n```\n\n## 文件操作\n\nAliPCS-Py 操作网盘中的文件可以使用文件的绝对路径或相对路径（相对与当前目录 pwd）。\n\n每一个用户都有自己的当前工作目录（pwd），默认为 `/` 根目录。\n\n使用者可以用 `cd` 命令来切换当前的工作目录（pwd）。\n\n下面所有涉及网盘路径的命令，其中如果网盘路径用的是相对路径，那么是相对于当前工作目录（pwd）的。\n如果是网盘路径用的是绝对路径，那么就是这个绝对路径。\n\n## 显示当前工作目录\n\n```\nAliPCS-Py pwd\n```\n\n## 切换当前工作目录\n\n切换到绝对路径：\n\n```\nAliPCS-Py cd /to/some/path\n```\n\n切换到相对路径：\n\n```\n# 切换到 (pwd)/../path\nAliPCS-Py cd ../path\n```\n\n## 列出网盘路径下的文件\n\n使用文件路径：\n\n```\nAliPCS-Py ls [OPTIONS] [REMOTEPATHS]...\n\nAliPCS-Py ls /absolute/path\n\n# or\nAliPCS-Py ls relative/path\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py ls -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                     | Description                                           |\n| -------------------------- | ----------------------------------------------------- |\n| -i, --file-id TEXT         | 文件 ID                                               |\n| --share-id, --si TEXT      | 列出这个分享 ID 下的文件                              |\n| --share-url, --su TEXT     | 列出这个分享 url 下的文件                             |\n| -p, --password TEXT        | 分享链接密码，如果没有不用设置                        |\n| -r, --desc                 | 逆序排列文件                                          |\n| -n, --name                 | 依名字排序                                            |\n| -t, --time                 | 依时间排序                                            |\n| -s, --size                 | 依文件大小排序                                        |\n| -R, --recursive            | 递归列出文件                                          |\n| -I, --include TEXT         | 筛选包含这个字符串的文件                              |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件                          |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件                      |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件                  |\n| -f, --is-file              | 筛选 **非** 目录文件                                  |\n| -d, --is-dir               | 筛选目录文件                                          |\n| --no-highlight, --NH       | 取消匹配高亮                                          |\n| -S, --show-size            | 显示文件大小                                          |\n| -D, --show-date            | 显示文件创建时间                                      |\n| --show-file-id, --ID       | 显示文件 ID                                           |\n| -M, --show-hash            | 显示文件 sha1                                         |\n| -A, --show-absolute-path   | 显示文件绝对路径                                      |\n| --show-dl-link, --DL       | 显示文件下载连接                                      |\n| --csv                      | 用 csv 格式显示，单行显示，推荐和 --DL 或 --HL 一起用 |\n| --only-dl-link, --ODL      | 只显示文件下载连接                                    |\n\n## 搜索文件\n\n搜索包含 `keyword` 的文件\n\n```\nAliPCS-Py search [OPTIONS] KEYWORD [REMOTEDIR]\n\n# 在当前工作目录中搜索\nAliPCS-Py search keyword\n\n# or\nAliPCS-Py search keyword /absolute/path\n\n# or\nAliPCS-Py search keyword relative/path\n```\n\n### 选项\n\n| Option                     | Description                          |\n| -------------------------- | ------------------------------------ |\n| -R, --recursive            | 递归搜索文件                         |\n| -I, --include TEXT         | 筛选包含这个字符串的文件             |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件         |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件     |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件 |\n| -f, --is-file              | 筛选 **非** 目录文件                 |\n| -d, --is-dir               | 筛选目录文件                         |\n| --no-highlight, --NH       | 取消匹配高亮                         |\n| -S, --show-size            | 显示文件大小                         |\n| -D, --show-date            | 显示文件创建时间                     |\n| -M, --show-hash            | 显示文件 sha1                        |\n| --csv                      | 用 csv 格式显示                      |\n\n## 显示文件内容\n\n```\nAliPCS-Py cat [OPTIONS] REMOTEPATH\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| -e, --encoding TEXT           | 文件编码，默认自动解码       |\n| --no-decrypt, --ND            | 不解密                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n\n## 创建目录\n\n```\nAliPCS-Py mkdir [OPTIONS] [REMOTEDIRS]...\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示目录    |\n\n## 移动文件\n\n移动一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 文件重命名\n\n```\nAliPCS-Py rename [OPTIONS] REMOTEPATH NEW_NAME\n```\n\ne.g.\n\n重命名 `/path/to/far` to `/path/to/foo`\n\n```\nAliPCS-Py rename /path/to/far foo\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 拷贝文件\n\n拷贝一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 删除文件\n\n```\nAliPCS-Py remove [OPTIONS] [REMOTEPATHS]...\n\n# 指定 路径\nAliPCS-Py remove /some/path\n# 指定 file-id\nAliPCS-Py remove --file-id ...\n```\n\n### 选项\n\n| Option        | Description  |\n| ------------- | ------------ |\n| -i, --file-id | TEXT 文件 ID |\n\n## 下载文件或目录\n\n使用文件路径：\n\n```\nAliPCS-Py download [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py download -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                                                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                    |\n| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| -i, --file-id TEXT                                     | 文件 ID                                                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| --share-id, --si TEXT                                  | 下载这个分享 ID 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --share-url, --su TEXT                                 | 下载这个分享 url 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                      |\n| -p, --password TEXT                                    | 分享链接密码，如果没有不用设置                                                                                                                                                                                                                                                                                                                                                                                                                                 |\n| -o, --outdir TEXT                                      | 指定下载本地目录，默认为当前目录                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -R, --recursive                                        | 递归下载                                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| -f, --from-index INTEGER                               | 从所有目录中的第几个文件开始下载，默认为 0（第一个）                                                                                                                                                                                                                                                                                                                                                                                                           |\n| -I, --include TEXT                                     | 筛选包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --include-regex, --IR TEXT                             | 筛选包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| -E, --exclude TEXT                                     | 筛选 不 包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| --exclude-regex, --ER TEXT                             | 筛选 不 包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -s, --concurrency INTEGER                              | 下载同步链接数，默认为 5。建议小于 10。                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| -k, --chunk-size TEXT                                  | 同步链接分块大小，默认为 50MB                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| -d, --downloader [ me \\| aget_py \\| aget_rs \\| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |\n| --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n\n## 播放媒体文件\n\n使用文件路径：\n\n```\nAliPCS-Py play [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n**注意：目前，使用 `--share-id` 或 `--file-id` 时，无法使用 `--use-local-server`**\n\n```\nAliPCS-Py play -i file_id1 -i file_id2 -i ...\n```\n\n`play` 命令默认播放带有媒体后缀的文件，如 `abc.mp4`, `abc.mp3`。如果需要播放的媒体文件没有用常规的媒体文件后缀，则需要加选项 `--ignore-ext`。\n\n### 选项\n\n| Option                        | Description                                          |\n| ----------------------------- | ---------------------------------------------------- |\n| -i, --file-id TEXT            | 文件 ID                                              |\n| --share-id, --si TEXT         | 播放这个分享 ID 下的文件                             |\n| --share-url, --su TEXT        | 播放这个分享 url 下的文件                            |\n| -p, --password TEXT           | 链接密码，如果没有不用设置                           |\n| -R, --recursive               | 递归播放                                             |\n| -f, --from-index INTEGER      | 从所有目录中的第几个文件开始播放，默认为 0（第一个） |\n| -I, --include TEXT            | 筛选包含这个字符串的文件                             |\n| --include-regex, --IR TEXT    | 筛选包含这个正则表达式的文件                         |\n| -E, --exclude TEXT            | 筛选 不 包含这个字符串的文件                         |\n| --exclude-regex, --ER TEXT    | 筛选 不 包含这个正则表达式的文件                     |\n| --player-params, --PP TEXT    | 第三方播放器参数                                     |\n| -q, --quiet                   | 取消第三方播放器输出                                 |\n| --shuffle, --sf               | 随机播放                                             |\n| --ignore-ext, --IE            | 不用文件名后缀名来判断媒体文件                       |\n| --out-cmd, --OC               | 输出第三方播放器命令                                 |\n| --pl, --player [mpv]          | 指定第三方播放器<br><br>默认为 mpv (https://mpv.io)  |\n| -s, --use-local-server        | 使用本地服务器播放。                                 |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的                         |\n\n## 上传文件\n\n上传一些本地文件或目录到网盘目录。\n\nAliPCS-Py 首先会尝试秒传。如果秒传失败，会使用分片上传上传文件。\n\n上传过程中，按 “p” 可以暂停或继续上传。\n\n```\nAliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定上传方式：\n\n`--upload-type Many`: 同时上传多个文件。\n\n适合大多数文件长度小于 100M 以下的情况。\n\n```\nAliPCS-Py upload --upload-type Many [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n<del>`--upload-type One`: 一次只上传一个文件，但同时上传文件的多个分片。</del>\n\n<del>适合大多数文件长度大于 1G 以上的情况。</del>\n\n**阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效**\n\n```\nAliPCS-Py upload --upload-type One [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定同时上传连接数量:\n\n`--max-workers` 默认为 CPU 核数。\n\n```\nAliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n如果上传本地目录 `localdir` 到远端目录 `remotedir`，AliPCS-Py 是将 `localdir` 这个目录上传到远端目录 `remotedir` 下。\n\n比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。\n\n如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`\n\n### 选项\n\n| Option                                                     | Description                             |\n| ---------------------------------------------------------- | --------------------------------------- |\n| -t, --upload-type [One \\| Many]                            | 上传方式，Many (默认): 同时上传多个文件 |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的            |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密          |\n| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数   |\n| --no-ignore-existing, --NI                                 | 上传已经存在的文件                      |\n| --no-show-progress, --NP                                   | 不显示上传进度                          |\n\n## 同步本地目录到远端\n\n同步本地目录到远端。\n\n如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。\n\n```\nAliPCS-Py sync [OPTIONS] LOCALDIR REMOTEDIR\n```\n\n### 选项\n\n| Option                                                     | Description                    |\n| ---------------------------------------------------------- | ------------------------------ |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的   |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密 |\n| -w, --max-workers INTEGER                                  | 同时上传文件数                 |\n| --no-show-progress, --NP                                   | 不显示上传进度                 |\n\n## 关于秒传连接\n\n**阿里云盘已经不能实现用秒传连接上传。**\n\n## 分享文件\n\n```\nAliPCS-Py share [OPTIONS] [REMOTEPATHS]...\n```\n\n### 选项\n\n| Option                      | Description                      |\n| --------------------------- | -------------------------------- |\n| -p, --password TEXT         | 设置秘密，4 个字符。默认没有秘密 |\n| --period-time, --pt INTEGER | 设置分享有效期，单位为天         |\n\n## 列出分享链接\n\n```\nAliPCS-Py shared\n```\n\n### 选项\n\n| Option         | Description                                  |\n| -------------- | -------------------------------------------- |\n| -A, --show-all | 显示所有分享的链接，默认只显示有效的分享链接 |\n\n## 取消分享链接\n\n```\nAliPCS-Py cancelshared [OPTIONS] [SHARE_IDS]...\n```\n\n## 列出其他用户分享链接中的文件\n\n给 `ls` 命令加参数，我们可以列出其他用户分享链接中的文件。\n\n**注意: 这里 `remotepaths` 只能是绝对路径。**\n\n如果有分享密码，加上 `--password PASSWORD`。\n\n- 使用分享连接\n\n  ```\n  AliPCS-Py ls --share-url SHARE_URL\n\n  # e.g.\n\n  # 列出这个分享url的根目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归列出这个分享url的文件\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 列出这个分享url的指定目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  分享 ID 是 https://www.aliyundrive.com/s/DaNNsdvi9bi 中的 `DaNNsdvi9bi`\n\n  ```\n  AliPCS-Py ls /path --share-id SHARE_ID\n\n  # e.g.\n\n  # 列出这个分享ID的根目录\n  AliPCS-Py ls / --share-id DaNNsdvi9bi\n\n  # 列出这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py ls --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `ls` 命令。\n\n## 下载他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`download` 命令可以直接下载他人分享的文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py download /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py download /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py download --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 下载这个分享url的指定目录\n  AliPCS-Py download --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi -R\n\n  # 下载这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py download --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `download` 命令。\n\n## 播放他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`play` 命令可以直接播放他人分享的媒体文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py play /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py play /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py play --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 播放这个分享url的指定目录\n  AliPCS-Py play --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi -R\n\n  # 播放这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py play --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `play` 命令。\n\n## 保存其他用户分享的链接\n\n保存其他用户分享的链接到远端目录。\n\n```\nAliPCS-Py save [OPTIONS] SHARE_URL_OR_ID REMOTEDIR\n```\n\n指定 `--file-id` 可以保存指定的文件。\n\n### 选项\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -i, --file-id TEXT  | 文件 ID                        |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 本地保存分享连接\n\n可以将他人分享了连接保存至本地，而不需要保存在网盘。这只作为一个记录。在需要是提供查看搜索功能。\n\n使用这个功能，需要使用者在本地配置文件(`~/.alipcs-py/config.toml`)中配置:\n\n```toml\n[share]\nstore = true\n```\n\n这个功能开启后，所有与他人分享连接的操作，都会将连接和其中访问过的文件信息保存在本地文件 `~/.alipcs-py/shared-store.sqlite3` 中。\n\n使用者可以用下面的命令来查看或搜索保存的分享连接。\n\n## 保存分享连接至本地\n\n```\nAliPCS-Py storesharedlinks [OPTIONS] [SHARE_URLS_OR_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 显示本地保存的分享连接\n\n```\nAliPCS-Py listsharedlinks\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 显示本地保存的分享文件\n\n```\nAliPCS-Py listsharedfiles [OPTIONS]\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description                |\n| --------------------- | -------------------------- |\n| --share-id, --si TEXT | 指定显示 share id 下的文件 |\n\n## 查找本地保存的分享连接\n\n```\nAliPCS-Py findsharedlinks [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 查找本地保存的分享文件\n\n```\nAliPCS-Py findsharedfiles [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description       |\n| --------------------- | ----------------- |\n| --share-id, --si TEXT | 要搜索的 share id |\n| -v, --verbose         | 显示细节          |\n\n## 查找本地保存的分享连接和文件\n\n```\nAliPCS-Py findshared [OPTIONS] [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option        | Description |\n| ------------- | ----------- |\n| -v, --verbose | 显示细节    |\n\n## 删除本地保存的分享连接或文件\n\n```\nAliPCS-Py deletestoredshared [OPTIONS] [SHARE_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option             | Description                                                |\n| ------------------ | ---------------------------------------------------------- |\n| -k, --keyword TEXT | 要删除文件名的关键字，如果为空则删除 share_id 下的所有文件 |\n\n## 清理本地保存的无效分享连接\n\n```\nAliPCS-Py cleanstore\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 开启 HTTP 服务\n\n在远端 `ROOT_DIR` 目录下开启 HTTP 服务。\n\n`ROOT_DIR` 默认为 `/`\n\n```\nAliPCS-Py AliPCS-Py server [OPTIONS] [ROOT_DIR]\n```\n\n如果需要设置认证，使用下面的选项设置用户名和密钥：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --username \'foo\' --password \'bar\'\n```\n\n也可以指定服务路径：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --path \'/my/pan\'\n\n# 访问 http://localhost:8000/my/pan/\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| --path TEXT                   | 服务路径，默认为 “/”         |\n| -h, --host TEXT               | 监听 host                    |\n| -p, --port INTEGER            | 监听 port                    |\n| -w, --workers INTEGER         | 进程数                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n| --username TEXT               | HTTP Basic Auth 用户名       |\n| --password TEXT               | HTTP Basic Auth 密钥         |\n',
+    'long_description': '# AliPCS-Py\n\n**2023-04-24 支持 阿里云盘开放平台 api。**\n\n**2023-02-15 使用临时 API 接口，让下载可用。**\n\n**2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**\n\n[![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)\n![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)\n\nAn AliPCS API and An App\n\nAliPCS-Py 是阿里云盘的非官方 api 和一个命令行运用程序。\n\n---\n\n## 百度云盘 api 和 命令行客户端在 https://github.com/PeterDing/BaiduPCS-Py\n\n---\n\n- [安装](#安装)\n- [更新](#更新)\n- [API](#API)\n- [用法](#用法)\n- [命令别名](#命令别名)\n- [对多个帐号进行相同操作](#对多个帐号进行相同操作)\n\n#### 用户相关命令\n\n- [添加用户](#添加用户)\n- [显示当前用户的信息](#显示当前用户的信息)\n- [更新用户信息](#更新用户信息)\n- [显示所有用户](#显示所有用户)\n- [切换当前用户](#切换当前用户)\n- [删除一个用户](#删除一个用户)\n- [显示当前工作目录](#显示当前工作目录)\n- [切换当前工作目录](#切换当前工作目录)\n\n#### 无感加密解密文件\n\n- [设置文件加密密码](#设置文件加密密码)\n\n#### 文件操作相关命令\n\n- [文件操作](#文件操作)\n- [列出网盘路径下的文件](#列出网盘路径下的文件)\n- [搜索文件](#搜索文件)\n- [显示文件内容](#显示文件内容)\n- [创建目录](#创建目录)\n- [移动文件](#移动文件)\n- [文件重命名](#文件重命名)\n- [拷贝文件](#拷贝文件)\n- [删除文件](#删除文件)\n- [下载文件或目录](#下载文件或目录)\n- [播放媒体文件](#播放媒体文件)\n- [上传文件](#上传文件)\n- [同步本地目录到远端](#同步本地目录到远端)\n\n#### 秒传\n\n- [关于秒传连接](#关于秒传连接)\n\n#### 分享相关命令\n\n- [分享文件](#分享文件)\n- [列出分享链接](#列出分享链接)\n- [取消分享链接](#取消分享链接)\n- [列出其他用户分享链接中的文件](#列出其他用户分享链接中的文件)\n- [下载他人分享的文件](#下载他人分享的文件)\n- [播放他人分享的文件](#播放他人分享的文件)\n- [保存其他用户分享的链接](#保存其他用户分享的链接)\n\n#### 本地保存分享连接\n\n- [保存分享连接至本地](#保存分享连接至本地)\n- [显示本地保存的分享连接](#显示本地保存的分享连接)\n- [显示本地保存的分享文件](#显示本地保存的分享文件)\n- [查找本地保存的分享连接](#查找本地保存的分享连接)\n- [查找本地保存的分享文件](#查找本地保存的分享文件)\n- [查找本地保存的分享连接和文件](#查找本地保存的分享连接和文件)\n- [删除本地保存的分享连接或文件](#删除本地保存的分享连接或文件)\n- [清理本地保存的无效分享连接](#清理本地保存的无效分享连接)\n\n#### HTTP 服务\n\n- [开启 HTTP 服务](#开启-HTTP-服务)\n\n## 安装\n\n需要 Python 版本大于或等于 3.8\n\n```\npip3 install Cython\npip3 install AliPCS-Py\n```\n\n### Windows 依赖\n\n在 Windows 上，AliPCS-Py 依赖 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)。\n\n在安装 AliPCS-Py 前，请先安装 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)，再在其中勾选 `C++ 生成工具` 并安装。完成后即可安装 AliPCS-Py。\n\n## 更新\n\n```\npip3 install AliPCS-Py --upgrade\n```\n\n## API\n\nAliPCS-Py 的阿里云盘 API 只依赖 requests，方便用户开发自己的运用。\n\n```python\nfrom alipcs_py.alipcs import AliPCSApi\n\napi = AliPCSApi(refresh_token)\n```\n\n## 用法\n\n```\nAliPCS-Py --help\n```\n\n## 命令别名\n\n可以用下面的命令别名代替原来的命令名。\n\n| 别名 | 原名         |\n| ---- | ------------ |\n| w    | who          |\n| uu   | updateuser   |\n| su   | su           |\n| ul   | userlist     |\n| ua   | useradd      |\n| ep   | encryptpwd   |\n| ud   | userdel      |\n| l    | ls           |\n| f    | search       |\n| md   | mkdir        |\n| mv   | move         |\n| rn   | rename       |\n| cp   | copy         |\n| rm   | remove       |\n| d    | download     |\n| p    | play         |\n| u    | upload       |\n| sn   | sync         |\n| S    | share        |\n| sl   | shared       |\n| cs   | cancelshared |\n| s    | save         |\n| sv   | server       |\n\n## 对多个帐号进行相同操作\n\nAliPCS-Py 支持对多个帐号进行相同操作。比如，用相同关键字搜索多个帐号，上传相同的文件/目录到多个帐号，等等。\n\n使用者只需用 `--users` 选项来指定要操作的帐号名即可。\n\n`--users` 接受一个参数，这个参数是用“,”连接的要进行操作帐号名的部分字符。假设我们现在有 3 个帐号，帐号名分别是 `Tom`，`Peter`，`Joy`。\n现在我要同时对`Tom`和`Joy`进行关键字搜索。我们可以用下面的命令进行：\n\n```\nAliPCS-Py --users \'Tom,Joy\' search \'keyword\' / -R\n```\n\n或者给出帐号名的部分片段：\n\n```\nAliPCS-Py --users \'om,oy\' search \'keyword\' / -R\n```\n\n更简单可以用：\n\n```\n# Tom, Joy 都包含字符 "o"\nAliPCS-Py --users \'o\' search \'keyword\' / -R\n```\n\n如果要对所有帐号进行操作用 `--users \'\'`。\n\n如果不使用 `--users` 选项，默认只对当前帐号进行操作。\n\n以下命令支持对多个帐号进行操作：\n\n- pwd\n- ls\n- search\n- cat\n- mkdir\n- move\n- rename\n- copy\n- remove\n- download\n- play\n- upload\n- sync\n- share\n- shared\n- cancelshared\n- save\n- server\n\n**注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。\n\n## 添加用户\n\n**从 2023-02-14 开始，阿里云盘官方限制了 web 端 api 的调用。从 web 端 api 获取到的下载连接是限速的。但如果调用[阿里云盘开放平台](https://survey.alibaba.com/apps/zhiliao/I9Dd1Nl89)的 api 获取到的下载连接是不限速的。**\n\nAliPCS-Py (>= v0.6.0) 支持调用阿里云盘开放平台 api。但是由于一直没有拿到内测，没法提供默认登录操作。需要用户自己找其他应用提供的登录方式登录。\n\n### 使用 web `refresh_token` 和 第三方认证地址 登录\n\n第三方认证地址提供阿里云盘开放平台的认证服务。由于一直没有拿到内测，本项目目前没法提供。需要使用者自行寻找。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-server "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 和 阿里云盘开放平台认证凭证 登录\n\n如果使用者拿到了阿里云盘开放平台认证，会获得 `client-id` 和 `client-secret`。使用这两个值可以直接登录。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-id "..." --client-secret "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 登录\n\n使用者需要在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。`useradd` 其他参数留空就好。\n\n使用者可以用下面的方式获取用户的 `refresh_token` 值。\n\n1. 登录 https://www.aliyundrive.com/drive/\n2. 打开浏览器的开发者工具(如 Chrome DevTools)。\n3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。\n\n![refresh_token](./imgs/refresh_token.png)\n\n现在找到了 `refresh_token` 值，我们可以用下面的命令添加一个用户。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..."\n```\n\nAliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。\n\n**注意：如果只用 `--web-refresh-token` 登录，下载文件时，服务器端会限速。**\n\n## 显示当前用户的信息\n\n```\nAliPCS-Py who\n```\n\n或者：\n\n```\nAliPCS-Py who user_id\n```\n\n指明显示用户 id 为 `user_id` 的用户信息。\n\n### 选项\n\n| Option                       | Description                |\n| ---------------------------- | -------------------------- |\n| -K, --show-encrypt-password  | 显示加密密码               |\n| --account-name TEXT          | 账号名 [默认为 user id]    |\n| --web-refresh-token TEXT     | 用户 web_refresh_token     |\n| --openapi-refresh-token TEXT | 用户 openapi_refresh_token |\n| --client-id TEXT             | openapi client id          |\n| --client-secret TEXT         | openapi client secret      |\n| --client-server TEXT         | openapi client server      |\n\n## 更新用户信息\n\n默认更新当前用户信息。\n\n```\nAliPCS-Py updateuser\n```\n\n也可指定多个 `user_id`\n\n```\nAliPCS-Py updateuser user_id\n```\n\n## 显示所有用户\n\n```\nAliPCS-Py userlist\n```\n\n## 切换当前用户\n\n```\nAliPCS-Py su\n```\n\n或者指定用户列表中用户所在的位置：\n\n```\nAliPCS-Py su 2\n```\n\n## 删除一个用户\n\n```\nAliPCS-Py userdel\n```\n\n## 设置文件加密密码\n\nAliPCS-Py 支持“无感的”文件加密。\n\nAliPCS-Py 可以加密上传文件，在下载的时候自动解密，让使用者感觉不到加密解密的过程。\n\n如果使用者需要将保密文件上传至阿里云盘保存，可以使用这个方法。即使帐号被盗，攻击者也无法还原文件内容。\n\nAliPCS-Py 支持以下加密方法：\n\n- **Simple** 一种简单的加密算法。根据密钥生成一个字节对照表来加密解密文件。\n  速度快，但**不安全**，不建议加密重要文件。\n  因为这种算法加解密不需要知道上下文信息，所以，下载时支持分段下载，如果是媒体文件则支持拖动播放。\n  推荐用于加密不重要的媒体文件。\n- **ChaCha20** 工业级加密算法，速度快，推荐用于加密重要文件。不支持分段下载。\n- **AES256CBC** 工业级加密算法，推荐用于加密重要文件。不支持分段下载。\n\n**注意**：用命令 `encryptpwd` 设置的密码**只是为当前用户**的。\n\n为当前用户设置加密密码:\n\n交互添加：\n\n```\nAliPCS-Py encryptpwd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py encryptpwd --encrypt-password \'my-encrypt-password\'\n```\n\n上传并加密文件：\n\n上传和同步文件时只需要指定加密算法就可。如果不指定就不加密。\n\n```\n# 默认使用上面设置的 `encrypt-password`\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type AES256CBC\n```\n\n下载并用上面设置的 `encrypt-password` 自动解密文件：\n\n```\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/\n```\n\n也可以使用临时的 `encrypt-password`：\n\n```\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type Simple --encrypt-password \'onlyyou\'\n```\n\n但在使用临时的 `encrypt-password` 后，`cat`、下载和播放这些文件时需要指定 `encrypt-password`，但不需要指定加密算法，程序会自动检查加密算法：\n\n```\n# 下载\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/  --encrypt-password \'onlyyou\'\n\n# 开启本地服务并播放\nAliPCS-Py play /to/here/some-file.mp4 --encrypt-password \'onlyyou\' --use-local-server\n```\n\n显示当前用户的密钥：\n\n```\nAliPCS-Py who --show-encrypt-password\n```\n\nAliPCS-Py 下载时默认会解密文件，如果想要下载但不解密文件，需要加 `--no-decrypt`\n\n```\nAliPCS-Py download some-file --no-decrypt\n```\n\n## 文件操作\n\nAliPCS-Py 操作网盘中的文件可以使用文件的绝对路径或相对路径（相对与当前目录 pwd）。\n\n每一个用户都有自己的当前工作目录（pwd），默认为 `/` 根目录。\n\n使用者可以用 `cd` 命令来切换当前的工作目录（pwd）。\n\n下面所有涉及网盘路径的命令，其中如果网盘路径用的是相对路径，那么是相对于当前工作目录（pwd）的。\n如果是网盘路径用的是绝对路径，那么就是这个绝对路径。\n\n## 显示当前工作目录\n\n```\nAliPCS-Py pwd\n```\n\n## 切换当前工作目录\n\n切换到绝对路径：\n\n```\nAliPCS-Py cd /to/some/path\n```\n\n切换到相对路径：\n\n```\n# 切换到 (pwd)/../path\nAliPCS-Py cd ../path\n```\n\n## 列出网盘路径下的文件\n\n使用文件路径：\n\n```\nAliPCS-Py ls [OPTIONS] [REMOTEPATHS]...\n\nAliPCS-Py ls /absolute/path\n\n# or\nAliPCS-Py ls relative/path\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py ls -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                     | Description                                           |\n| -------------------------- | ----------------------------------------------------- |\n| -i, --file-id TEXT         | 文件 ID                                               |\n| --share-id, --si TEXT      | 列出这个分享 ID 下的文件                              |\n| --share-url, --su TEXT     | 列出这个分享 url 下的文件                             |\n| -p, --password TEXT        | 分享链接密码，如果没有不用设置                        |\n| -r, --desc                 | 逆序排列文件                                          |\n| -n, --name                 | 依名字排序                                            |\n| -t, --time                 | 依时间排序                                            |\n| -s, --size                 | 依文件大小排序                                        |\n| -R, --recursive            | 递归列出文件                                          |\n| -I, --include TEXT         | 筛选包含这个字符串的文件                              |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件                          |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件                      |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件                  |\n| -f, --is-file              | 筛选 **非** 目录文件                                  |\n| -d, --is-dir               | 筛选目录文件                                          |\n| --no-highlight, --NH       | 取消匹配高亮                                          |\n| -S, --show-size            | 显示文件大小                                          |\n| -D, --show-date            | 显示文件创建时间                                      |\n| --show-file-id, --ID       | 显示文件 ID                                           |\n| -M, --show-hash            | 显示文件 sha1                                         |\n| -A, --show-absolute-path   | 显示文件绝对路径                                      |\n| --show-dl-link, --DL       | 显示文件下载连接                                      |\n| --csv                      | 用 csv 格式显示，单行显示，推荐和 --DL 或 --HL 一起用 |\n| --only-dl-link, --ODL      | 只显示文件下载连接                                    |\n\n## 搜索文件\n\n搜索包含 `keyword` 的文件\n\n```\nAliPCS-Py search [OPTIONS] KEYWORD [REMOTEDIR]\n\n# 在当前工作目录中搜索\nAliPCS-Py search keyword\n\n# or\nAliPCS-Py search keyword /absolute/path\n\n# or\nAliPCS-Py search keyword relative/path\n```\n\n### 选项\n\n| Option                     | Description                          |\n| -------------------------- | ------------------------------------ |\n| -R, --recursive            | 递归搜索文件                         |\n| -I, --include TEXT         | 筛选包含这个字符串的文件             |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件         |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件     |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件 |\n| -f, --is-file              | 筛选 **非** 目录文件                 |\n| -d, --is-dir               | 筛选目录文件                         |\n| --no-highlight, --NH       | 取消匹配高亮                         |\n| -S, --show-size            | 显示文件大小                         |\n| -D, --show-date            | 显示文件创建时间                     |\n| -M, --show-hash            | 显示文件 sha1                        |\n| --csv                      | 用 csv 格式显示                      |\n\n## 显示文件内容\n\n```\nAliPCS-Py cat [OPTIONS] REMOTEPATH\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| -e, --encoding TEXT           | 文件编码，默认自动解码       |\n| --no-decrypt, --ND            | 不解密                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n\n## 创建目录\n\n```\nAliPCS-Py mkdir [OPTIONS] [REMOTEDIRS]...\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示目录    |\n\n## 移动文件\n\n移动一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 文件重命名\n\n```\nAliPCS-Py rename [OPTIONS] REMOTEPATH NEW_NAME\n```\n\ne.g.\n\n重命名 `/path/to/far` to `/path/to/foo`\n\n```\nAliPCS-Py rename /path/to/far foo\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 拷贝文件\n\n拷贝一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 删除文件\n\n```\nAliPCS-Py remove [OPTIONS] [REMOTEPATHS]...\n\n# 指定 路径\nAliPCS-Py remove /some/path\n# 指定 file-id\nAliPCS-Py remove --file-id ...\n```\n\n### 选项\n\n| Option        | Description  |\n| ------------- | ------------ |\n| -i, --file-id | TEXT 文件 ID |\n\n## 下载文件或目录\n\n> 在使用了阿里云盘开放平台 api 时，如果下载他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中下载。\n> 下载结束后，会删除 `__alipcs_py_temp__` 中下载的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py download [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py download -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                                                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                    |\n| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| -i, --file-id TEXT                                     | 文件 ID                                                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| --share-id, --si TEXT                                  | 下载这个分享 ID 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --share-url, --su TEXT                                 | 下载这个分享 url 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                      |\n| -p, --password TEXT                                    | 分享链接密码，如果没有不用设置                                                                                                                                                                                                                                                                                                                                                                                                                                 |\n| -o, --outdir TEXT                                      | 指定下载本地目录，默认为当前目录                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -R, --recursive                                        | 递归下载                                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| -f, --from-index INTEGER                               | 从所有目录中的第几个文件开始下载，默认为 0（第一个）                                                                                                                                                                                                                                                                                                                                                                                                           |\n| -I, --include TEXT                                     | 筛选包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --include-regex, --IR TEXT                             | 筛选包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| -E, --exclude TEXT                                     | 筛选 不 包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| --exclude-regex, --ER TEXT                             | 筛选 不 包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -s, --concurrency INTEGER                              | 下载同步链接数，默认为 5。建议小于 10。                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| -k, --chunk-size TEXT                                  | 同步链接分块大小，默认为 50MB                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| -d, --downloader [ me \\| aget_py \\| aget_rs \\| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |\n| --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n\n## 播放媒体文件\n\n> 在使用了阿里云盘开放平台 api 时，如果播放他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中播放。\n> 播放结束后，会删除 `__alipcs_py_temp__` 中播放的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py play [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n**注意：目前，使用 `--share-id` 或 `--file-id` 时，无法使用 `--use-local-server`**\n\n```\nAliPCS-Py play -i file_id1 -i file_id2 -i ...\n```\n\n`play` 命令默认播放带有媒体后缀的文件，如 `abc.mp4`, `abc.mp3`。如果需要播放的媒体文件没有用常规的媒体文件后缀，则需要加选项 `--ignore-ext`。\n\n### 选项\n\n| Option                        | Description                                          |\n| ----------------------------- | ---------------------------------------------------- |\n| -i, --file-id TEXT            | 文件 ID                                              |\n| --share-id, --si TEXT         | 播放这个分享 ID 下的文件                             |\n| --share-url, --su TEXT        | 播放这个分享 url 下的文件                            |\n| -p, --password TEXT           | 链接密码，如果没有不用设置                           |\n| -R, --recursive               | 递归播放                                             |\n| -f, --from-index INTEGER      | 从所有目录中的第几个文件开始播放，默认为 0（第一个） |\n| -I, --include TEXT            | 筛选包含这个字符串的文件                             |\n| --include-regex, --IR TEXT    | 筛选包含这个正则表达式的文件                         |\n| -E, --exclude TEXT            | 筛选 不 包含这个字符串的文件                         |\n| --exclude-regex, --ER TEXT    | 筛选 不 包含这个正则表达式的文件                     |\n| --player-params, --PP TEXT    | 第三方播放器参数                                     |\n| -q, --quiet                   | 取消第三方播放器输出                                 |\n| --shuffle, --sf               | 随机播放                                             |\n| --ignore-ext, --IE            | 不用文件名后缀名来判断媒体文件                       |\n| --out-cmd, --OC               | 输出第三方播放器命令                                 |\n| --pl, --player [mpv]          | 指定第三方播放器<br><br>默认为 mpv (https://mpv.io)  |\n| -s, --use-local-server        | 使用本地服务器播放。                                 |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的                         |\n\n## 上传文件\n\n上传一些本地文件或目录到网盘目录。\n\nAliPCS-Py 首先会尝试秒传。如果秒传失败，会使用分片上传上传文件。\n\n上传过程中，按 “p” 可以暂停或继续上传。\n\n```\nAliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定上传方式：\n\n`--upload-type Many`: 同时上传多个文件。\n\n适合大多数文件长度小于 100M 以下的情况。\n\n```\nAliPCS-Py upload --upload-type Many [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n<del>`--upload-type One`: 一次只上传一个文件，但同时上传文件的多个分片。</del>\n\n<del>适合大多数文件长度大于 1G 以上的情况。</del>\n\n**阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效**\n\n```\nAliPCS-Py upload --upload-type One [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定同时上传连接数量:\n\n`--max-workers` 默认为 CPU 核数。\n\n```\nAliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n如果上传本地目录 `localdir` 到远端目录 `remotedir`，AliPCS-Py 是将 `localdir` 这个目录上传到远端目录 `remotedir` 下。\n\n比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。\n\n如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`\n\n### 选项\n\n| Option                                                     | Description                             |\n| ---------------------------------------------------------- | --------------------------------------- |\n| -t, --upload-type [One \\| Many]                            | 上传方式，Many (默认): 同时上传多个文件 |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的            |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密          |\n| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数   |\n| --no-ignore-existing, --NI                                 | 上传已经存在的文件                      |\n| --no-show-progress, --NP                                   | 不显示上传进度                          |\n\n## 同步本地目录到远端\n\n同步本地目录到远端。\n\n如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。\n\n```\nAliPCS-Py sync [OPTIONS] LOCALDIR REMOTEDIR\n```\n\n### 选项\n\n| Option                                                     | Description                    |\n| ---------------------------------------------------------- | ------------------------------ |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的   |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密 |\n| -w, --max-workers INTEGER                                  | 同时上传文件数                 |\n| --no-show-progress, --NP                                   | 不显示上传进度                 |\n\n## 关于秒传连接\n\n**阿里云盘已经不能实现用秒传连接上传。**\n\n## 分享文件\n\n```\nAliPCS-Py share [OPTIONS] [REMOTEPATHS]...\n```\n\n### 选项\n\n| Option                      | Description                      |\n| --------------------------- | -------------------------------- |\n| -p, --password TEXT         | 设置秘密，4 个字符。默认没有秘密 |\n| --period-time, --pt INTEGER | 设置分享有效期，单位为天         |\n\n## 列出分享链接\n\n```\nAliPCS-Py shared\n```\n\n### 选项\n\n| Option         | Description                                  |\n| -------------- | -------------------------------------------- |\n| -A, --show-all | 显示所有分享的链接，默认只显示有效的分享链接 |\n\n## 取消分享链接\n\n```\nAliPCS-Py cancelshared [OPTIONS] [SHARE_IDS]...\n```\n\n## 列出其他用户分享链接中的文件\n\n给 `ls` 命令加参数，我们可以列出其他用户分享链接中的文件。\n\n**注意: 这里 `remotepaths` 只能是绝对路径。**\n\n如果有分享密码，加上 `--password PASSWORD`。\n\n- 使用分享连接\n\n  ```\n  AliPCS-Py ls --share-url SHARE_URL\n\n  # e.g.\n\n  # 列出这个分享url的根目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归列出这个分享url的文件\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 列出这个分享url的指定目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  分享 ID 是 https://www.aliyundrive.com/s/DaNNsdvi9bi 中的 `DaNNsdvi9bi`\n\n  ```\n  AliPCS-Py ls /path --share-id SHARE_ID\n\n  # e.g.\n\n  # 列出这个分享ID的根目录\n  AliPCS-Py ls / --share-id DaNNsdvi9bi\n\n  # 列出这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py ls --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `ls` 命令。\n\n## 下载他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`download` 命令可以直接下载他人分享的文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py download /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py download /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py download --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 下载这个分享url的指定目录\n  AliPCS-Py download --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi -R\n\n  # 下载这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py download --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `download` 命令。\n\n## 播放他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`play` 命令可以直接播放他人分享的媒体文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py play /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py play /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py play --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 播放这个分享url的指定目录\n  AliPCS-Py play --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi -R\n\n  # 播放这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py play --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `play` 命令。\n\n## 保存其他用户分享的链接\n\n保存其他用户分享的链接到远端目录。\n\n```\nAliPCS-Py save [OPTIONS] SHARE_URL_OR_ID REMOTEDIR\n```\n\n指定 `--file-id` 可以保存指定的文件。\n\n### 选项\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -i, --file-id TEXT  | 文件 ID                        |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 本地保存分享连接\n\n可以将他人分享了连接保存至本地，而不需要保存在网盘。这只作为一个记录。在需要是提供查看搜索功能。\n\n使用这个功能，需要使用者在本地配置文件(`~/.alipcs-py/config.toml`)中配置:\n\n```toml\n[share]\nstore = true\n```\n\n这个功能开启后，所有与他人分享连接的操作，都会将连接和其中访问过的文件信息保存在本地文件 `~/.alipcs-py/shared-store.sqlite3` 中。\n\n使用者可以用下面的命令来查看或搜索保存的分享连接。\n\n## 保存分享连接至本地\n\n```\nAliPCS-Py storesharedlinks [OPTIONS] [SHARE_URLS_OR_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 显示本地保存的分享连接\n\n```\nAliPCS-Py listsharedlinks\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 显示本地保存的分享文件\n\n```\nAliPCS-Py listsharedfiles [OPTIONS]\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description                |\n| --------------------- | -------------------------- |\n| --share-id, --si TEXT | 指定显示 share id 下的文件 |\n\n## 查找本地保存的分享连接\n\n```\nAliPCS-Py findsharedlinks [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 查找本地保存的分享文件\n\n```\nAliPCS-Py findsharedfiles [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description       |\n| --------------------- | ----------------- |\n| --share-id, --si TEXT | 要搜索的 share id |\n| -v, --verbose         | 显示细节          |\n\n## 查找本地保存的分享连接和文件\n\n```\nAliPCS-Py findshared [OPTIONS] [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option        | Description |\n| ------------- | ----------- |\n| -v, --verbose | 显示细节    |\n\n## 删除本地保存的分享连接或文件\n\n```\nAliPCS-Py deletestoredshared [OPTIONS] [SHARE_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option             | Description                                                |\n| ------------------ | ---------------------------------------------------------- |\n| -k, --keyword TEXT | 要删除文件名的关键字，如果为空则删除 share_id 下的所有文件 |\n\n## 清理本地保存的无效分享连接\n\n```\nAliPCS-Py cleanstore\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 开启 HTTP 服务\n\n在远端 `ROOT_DIR` 目录下开启 HTTP 服务。\n\n`ROOT_DIR` 默认为 `/`\n\n```\nAliPCS-Py AliPCS-Py server [OPTIONS] [ROOT_DIR]\n```\n\n如果需要设置认证，使用下面的选项设置用户名和密钥：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --username \'foo\' --password \'bar\'\n```\n\n也可以指定服务路径：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --path \'/my/pan\'\n\n# 访问 http://localhost:8000/my/pan/\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| --path TEXT                   | 服务路径，默认为 “/”         |\n| -h, --host TEXT               | 监听 host                    |\n| -p, --port INTEGER            | 监听 port                    |\n| -w, --workers INTEGER         | 进程数                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n| --username TEXT               | HTTP Basic Auth 用户名       |\n| --password TEXT               | HTTP Basic Auth 密钥         |\n',
     'author': 'PeterDing',
     'author_email': 'dfhayst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/PeterDing/AliPCS-Py',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 from build import *
 build(setup_kwargs)
 
 setup(**setup_kwargs)
```

### Comparing `alipcs_py-0.5.3/PKG-INFO` & `alipcs_py-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 Metadata-Version: 2.1
 Name: alipcs-py
-Version: 0.5.3
+Version: 0.6.0
 Summary: Ali Pcs Api and App
 Home-page: https://github.com/PeterDing/AliPCS-Py
 License: MIT
 Author: PeterDing
 Author-email: dfhayst@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aget (>=0.1)
 Requires-Dist: chardet (>=5.0)
 Requires-Dist: click (>=8.1)
 Requires-Dist: cryptography (>=38.0)
 Requires-Dist: cython (>=0.29)
 Requires-Dist: ecdsa (>=0.18)
 Requires-Dist: fastapi (>=0.87)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: passlib (>=1.7)
 Requires-Dist: peewee (>=3.15)
 Requires-Dist: pillow (>=9.3)
+Requires-Dist: qrcode (>=7.4)
 Requires-Dist: requests (>=2.28)
 Requires-Dist: requests-toolbelt (>=0.10)
 Requires-Dist: rich (>=12.6)
 Requires-Dist: toml (>=0.10)
 Requires-Dist: typing-extensions (>=4.4)
 Requires-Dist: uvicorn (>=0.19)
 Description-Content-Type: text/markdown
 
 # AliPCS-Py
 
+**2023-04-24 支持 阿里云盘开放平台 api。**
+
 **2023-02-15 使用临时 API 接口，让下载可用。**
 
 **2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**
 
 [![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)
 ![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)
 
@@ -125,15 +127,15 @@
 
 #### HTTP 服务
 
 - [开启 HTTP 服务](#开启-HTTP-服务)
 
 ## 安装
 
-需要 Python 版本大于或等于 3.7
+需要 Python 版本大于或等于 3.8
 
 ```
 pip3 install Cython
 pip3 install AliPCS-Py
 ```
 
 ### Windows 依赖
@@ -245,15 +247,59 @@
 - save
 - server
 
 **注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。
 
 ## 添加用户
 
-AliPCS-Py 目前支持用`refresh_token`登录。需要使用者在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。
+**从 2023-02-14 开始，阿里云盘官方限制了 web 端 api 的调用。从 web 端 api 获取到的下载连接是限速的。但如果调用[阿里云盘开放平台](https://survey.alibaba.com/apps/zhiliao/I9Dd1Nl89)的 api 获取到的下载连接是不限速的。**
+
+AliPCS-Py (>= v0.6.0) 支持调用阿里云盘开放平台 api。但是由于一直没有拿到内测，没法提供默认登录操作。需要用户自己找其他应用提供的登录方式登录。
+
+### 使用 web `refresh_token` 和 第三方认证地址 登录
+
+第三方认证地址提供阿里云盘开放平台的认证服务。由于一直没有拿到内测，本项目目前没法提供。需要使用者自行寻找。
+
+交互添加：
+
+```
+AliPCS-Py useradd
+```
+
+或者直接添加：
+
+```
+AliPCS-Py useradd --web-refresh-token "..." --client-server "..."
+# 其他选项留空
+```
+
+之后用阿里云盘 APP 扫码登录。
+
+### 使用 web `refresh_token` 和 阿里云盘开放平台认证凭证 登录
+
+如果使用者拿到了阿里云盘开放平台认证，会获得 `client-id` 和 `client-secret`。使用这两个值可以直接登录。
+
+交互添加：
+
+```
+AliPCS-Py useradd
+```
+
+或者直接添加：
+
+```
+AliPCS-Py useradd --web-refresh-token "..." --client-id "..." --client-secret "..."
+# 其他选项留空
+```
+
+之后用阿里云盘 APP 扫码登录。
+
+### 使用 web `refresh_token` 登录
+
+使用者需要在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。`useradd` 其他参数留空就好。
 
 使用者可以用下面的方式获取用户的 `refresh_token` 值。
 
 1. 登录 https://www.aliyundrive.com/drive/
 2. 打开浏览器的开发者工具(如 Chrome DevTools)。
 3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。
 
@@ -266,19 +312,21 @@
 ```
 AliPCS-Py useradd
 ```
 
 或者直接添加：
 
 ```
-AliPCS-Py useradd --refresh-token "..."
+AliPCS-Py useradd --web-refresh-token "..."
 ```
 
 AliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。
 
+**注意：如果只用 `--web-refresh-token` 登录，下载文件时，服务器端会限速。**
+
 ## 显示当前用户的信息
 
 ```
 AliPCS-Py who
 ```
 
 或者：
@@ -287,17 +335,23 @@
 AliPCS-Py who user_id
 ```
 
 指明显示用户 id 为 `user_id` 的用户信息。
 
 ### 选项
 
-| Option                      | Description  |
-| --------------------------- | ------------ |
-| -K, --show-encrypt-password | 显示加密密码 |
+| Option                       | Description                |
+| ---------------------------- | -------------------------- |
+| -K, --show-encrypt-password  | 显示加密密码               |
+| --account-name TEXT          | 账号名 [默认为 user id]    |
+| --web-refresh-token TEXT     | 用户 web_refresh_token     |
+| --openapi-refresh-token TEXT | 用户 openapi_refresh_token |
+| --client-id TEXT             | openapi client id          |
+| --client-secret TEXT         | openapi client secret      |
+| --client-server TEXT         | openapi client server      |
 
 ## 更新用户信息
 
 默认更新当前用户信息。
 
 ```
 AliPCS-Py updateuser
@@ -612,14 +666,17 @@
 
 | Option        | Description  |
 | ------------- | ------------ |
 | -i, --file-id | TEXT 文件 ID |
 
 ## 下载文件或目录
 
+> 在使用了阿里云盘开放平台 api 时，如果下载他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中下载。
+> 下载结束后，会删除 `__alipcs_py_temp__` 中下载的文件。
+
 使用文件路径：
 
 ```
 AliPCS-Py download [OPTIONS] [REMOTEPATHS]...
 ```
 
 使用文件 ID：
@@ -648,14 +705,17 @@
 | -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | -d, --downloader [ me \| aget_py \| aget_rs \| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |
 | --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |
 
 ## 播放媒体文件
 
+> 在使用了阿里云盘开放平台 api 时，如果播放他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中播放。
+> 播放结束后，会删除 `__alipcs_py_temp__` 中播放的文件。
+
 使用文件路径：
 
 ```
 AliPCS-Py play [OPTIONS] [REMOTEPATHS]...
 ```
 
 使用文件 ID：
```

