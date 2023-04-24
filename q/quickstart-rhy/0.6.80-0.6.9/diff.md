# Comparing `tmp/quickstart_rhy-0.6.80.tar.gz` & `tmp/QuickStart_Rhy-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart_rhy-0.6.80.tar", max compression
+gzip compressed data, was "QuickStart_Rhy-0.6.9.tar", last modified: Wed Mar  2 09:21:30 2022, max compression
```

## Comparing `quickstart_rhy-0.6.80.tar` & `QuickStart_Rhy-0.6.9.tar`

### file list

```diff
@@ -1,50 +1,62 @@
--rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.6.80/LICENSE
--rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.6.80/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.6.80/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0        0        0     3419 2023-04-15 03:33:34.034264 quickstart_rhy-0.6.80/QuickStart_Rhy/API/ChatGPT.py
--rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.6.80/QuickStart_Rhy/API/DeepL.py
--rw-r--r--   0        0        0      461 2023-03-03 03:25:06.035139 quickstart_rhy-0.6.80/QuickStart_Rhy/API/DeepLX.py
--rw-r--r--   0        0        0     1313 2023-01-23 15:27:56.468467 quickstart_rhy-0.6.80/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.6.80/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.6.80/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.6.80/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.6.80/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.6.80/QuickStart_Rhy/API/alapi.py
--rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/__init__.py
--rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0        0        0     9151 2023-04-24 09:10:36.431917 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/MultiSingleDL.py
--rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/__init__.py
--rw-r--r--   0        0        0     1076 2023-03-14 08:26:31.520529 quickstart_rhy-0.6.80/QuickStart_Rhy/NumbaTools/__init__.py
--rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/DiskMac.py
--rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/__init__.py
--rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.6.80/QuickStart_Rhy/ThreadTools/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.6.80/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.6.80/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.6.80/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.6.80/QuickStart_Rhy/TuiTools/__init__.py
--rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.6.80/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.6.80/QuickStart_Rhy/__cache__.py
--rw-r--r--   0        0        0     9777 2023-03-31 05:06:37.193966 quickstart_rhy-0.6.80/QuickStart_Rhy/__config__.py
--rw-r--r--   0        0        0    15748 2023-04-14 02:35:27.961149 quickstart_rhy-0.6.80/QuickStart_Rhy/__init__.py
--rw-r--r--   0        0        0    42307 2023-04-22 06:27:05.879972 quickstart_rhy-0.6.80/QuickStart_Rhy/apiTools.py
--rw-r--r--   0        0        0    14183 2023-03-16 03:04:25.939031 quickstart_rhy-0.6.80/QuickStart_Rhy/funcList.py
--rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.6.80/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0        0        0     2373 2023-01-22 08:07:59.504881 quickstart_rhy-0.6.80/QuickStart_Rhy/main.py
--rw-r--r--   0        0        0    11782 2023-02-16 12:55:15.000353 quickstart_rhy-0.6.80/QuickStart_Rhy/netTools.py
--rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.6.80/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.6.80/QuickStart_Rhy/system.py
--rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.6.80/README.md
--rw-r--r--   0        0        0      509 2023-04-24 13:54:34.768357 quickstart_rhy-0.6.80/pyproject.toml
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 quickstart_rhy-0.6.80/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 quickstart_rhy-0.6.80/PKG-INFO
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288929 QuickStart_Rhy-0.6.9/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1067 2019-09-20 01:32:29.000000 QuickStart_Rhy-0.6.9/LICENSE
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-03-02 09:21:30.289005 QuickStart_Rhy-0.6.9/PKG-INFO
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.283704 QuickStart_Rhy-0.6.9/QuickStart_Rhy/
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.285666 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5540 2021-06-02 09:40:32.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3312 2022-01-25 08:11:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1207 2022-01-14 15:40:03.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5783 2021-06-02 09:41:17.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     8909 2022-02-20 18:53:33.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     6365 2021-05-15 16:08:12.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1110 2021-02-23 18:02:37.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    20384 2022-01-31 06:47:25.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/alapi.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.286469 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     2307 2021-08-07 06:49:25.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    10325 2022-02-18 15:11:23.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      478 2021-08-07 06:47:43.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4005 2021-10-29 01:06:50.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       75 2021-01-14 15:40:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.287544 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1716 2021-04-14 06:04:07.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4934 2021-06-11 16:15:17.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3649 2022-03-02 09:15:49.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    11332 2022-03-02 05:36:33.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3673 2021-04-25 15:34:28.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3103 2021-01-27 06:50:19.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5763 2021-02-23 14:24:09.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288114 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     8861 2021-04-27 13:27:14.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4941 2021-04-30 07:48:42.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1127 2021-01-14 16:13:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1786 2021-04-04 02:34:42.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Monitor.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      623 2021-06-11 16:14:44.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288228 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     2794 2021-01-14 16:19:31.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288698 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4118 2022-03-02 05:29:22.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1292 2021-04-04 02:31:01.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      549 2021-04-25 15:17:49.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      102 2022-02-19 14:45:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/__init__.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.288813 QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4765 2021-01-25 08:16:22.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     9563 2022-02-19 14:36:18.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/__config__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     7076 2022-02-20 18:27:06.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    36966 2022-02-25 17:33:50.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/api.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)    12754 2022-02-24 10:06:39.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/funcList.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     5368 2021-10-27 04:35:12.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3648 2022-02-13 16:31:26.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/main.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     9085 2022-01-29 04:45:18.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/netTools.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     2288 2022-02-14 15:11:41.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     4882 2021-08-07 07:00:24.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy/system.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-03-02 09:21:30.284587 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      878 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/PKG-INFO
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1636 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/SOURCES.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/dependency_links.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       49 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/entry_points.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       56 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/requires.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       15 2022-03-02 09:21:30.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/top_level.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2020-04-02 18:40:53.000000 QuickStart_Rhy-0.6.9/QuickStart_Rhy.egg-info/zip-safe
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      425 2021-10-31 04:57:47.000000 QuickStart_Rhy-0.6.9/README.md
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      140 2022-03-02 09:21:30.289244 QuickStart_Rhy-0.6.9/setup.cfg
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-03-02 09:21:22.000000 QuickStart_Rhy-0.6.9/setup.py
```

### Comparing `quickstart_rhy-0.6.80/LICENSE` & `QuickStart_Rhy-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/API/AliCloud.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/AliCloud.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # coding=utf-8
 """
 阿里云相关API
 
 Alibaba cloud API
 """
-from . import pre_check, user_lang
+from . import pre_check, user_lang, dir_char
 from .. import requirePackage
+oss2 = requirePackage('oss2')
 
 
 class AliyunOSS:
-    def __init__(
-        self,
-        ac_id=pre_check("aliyun_oss_acid"),
-        ac_key=pre_check("aliyun_oss_ackey"),
-        bucket_url=pre_check("aliyun_oss_df_endpoint"),
-        df_bucket=pre_check("aliyun_oss_df_bucket"),
-    ):
+    def __init__(self, ac_id=pre_check('aliyun_oss_acid'), ac_key=pre_check('aliyun_oss_ackey'),
+                 bucket_url=pre_check('aliyun_oss_df_endpoint'), df_bucket=pre_check('aliyun_oss_df_bucket')):
         """
         初始化并登陆阿里云对象存储
 
         Initializes and logs into ali cloud object storage
 
         :param ac_id: Access id
         :param ac_key: Access key
@@ -27,125 +23,105 @@
         :param df_bucket: 桶名称
         """
         self.ac_id = ac_id
         self.ac_key = ac_key
         self.bucket_url = bucket_url
         self.df_bucket = df_bucket
         self.progress, self.trans_id, self._progress_file_name = None, None, None
-        self.auth = requirePackage("oss2", "Auth")(self.ac_id, self.ac_key)
+        self.auth = oss2.Auth(self.ac_id, self.ac_key)
 
     def get_func_table(self):
         """
         获取OSS类支持的操作
 
         Get the operations supported by the OSS class
 
         :return: 支持的函数字典
         """
         return {
-            "-up": self.upload,
-            "-rm": self.remove,
-            "-dl": self.download,
-            "-ls": self.list_bucket,
+            '-up': self.upload,
+            '-rm': self.remove,
+            '-dl': self.download,
+            '-ls': self.list_bucket
         }
 
     def _progress_bar(self, cur, total):
         """
         创建一个进度条并启动
 
         Create a progress bar and start
 
         :param cur: 当前完成量
         :param total: 总任务量
         :return: None
         """
         if not self.progress:
             from ..TuiTools.Bar import DataTransformBar
-
             self.progress = DataTransformBar(True if total else False)
-            self.trans_id = self.progress.add_task(
-                "Transform",
-                total=total if total else -1,
-                filename=self._progress_file_name,
-            )
+            self.trans_id = self.progress.add_task('Transform', total=total if total else -1,
+                                                   filename=self._progress_file_name)
             self.progress.start()
             self.progress.start_task(self.trans_id)
         self.progress.update(self.trans_id, completed=cur)
 
-    def upload(self, filePath: str, bucket: str = None, key: str = None):
+    def upload(self, filePath: str, bucket: str = None):
         """
         上传文件（支持断点续传）
 
         Upload file (support breakpoint continuation)
 
         :param filePath: 文件路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         import os
-        from .. import qs_default_console, qs_info_string, dir_char
+        from .. import qs_default_console, qs_info_string
         from ..SystemTools import get_core_num
-
         bucket = bucket if bucket else self.df_bucket
-        bucket = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
+        bucket = oss2.Bucket(self.auth, self.bucket_url, bucket)
         filePath = filePath.strip()
         self._progress_file_name = os.path.basename(filePath)
-        requirePackage("oss2", "resumable_upload")(
-            bucket,
-            key if key else filePath.replace(dir_char, "/"),
-            filePath,
-            num_threads=get_core_num() * 4,
-            progress_callback=self._progress_bar,
-        )
+        oss2.resumable_upload(bucket, filePath.replace(dir_char, '/'), filePath, num_threads=get_core_num() * 4,
+                              progress_callback=self._progress_bar)
         self.progress.stop()
-        qs_default_console.print(
-            qs_info_string, "Transform Completed!" if user_lang != "zh" else "传输完成!"
-        )
+        qs_default_console.print(qs_info_string, 'Transform Completed!' if user_lang != 'zh' else '传输完成!')
 
     def download(self, filename: str, bucket: str = None):
         """
         下载文件（支持断点续传）
 
         Download file (support breakpoint continuation)
 
         :param filename: 文件在bucket中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         import os
         from .. import qs_default_console, qs_info_string
         from ..SystemTools import get_core_num
-
         bucket = bucket if bucket else self.df_bucket
-        bucket = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
+        bucket = oss2.Bucket(self.auth, self.bucket_url, bucket)
         self._progress_file_name = os.path.basename(filename)
-        requirePackage("oss2", "resumable_download")(
-            bucket,
-            filename,
-            filename,
-            num_threads=get_core_num() * 4,
-            progress_callback=self._progress_bar,
-        )
+        oss2.resumable_download(bucket, filename, filename, num_threads=get_core_num() * 4,
+                                progress_callback=self._progress_bar)
         self.progress.stop()
-        qs_default_console.print(
-            qs_info_string, "Transform Completed!" if user_lang != "zh" else "传输完成!"
-        )
+        qs_default_console.print(qs_info_string, 'Transform Completed!' if user_lang != 'zh' else '传输完成!')
 
     def remove(self, filePath: str, bucket: str = None):
         """
         删除文件
 
         delete file
 
         :param filePath: 文件在bucket中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         bucket = bucket if bucket else self.df_bucket
-        bucket = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
+        bucket = oss2.Bucket(self.auth, self.bucket_url, bucket)
         bucket.delete_object(filePath)
 
     def list_bucket(self, bucket: str = None):
         """
         打印桶中的文件表
 
         Print the file table in the bucket
@@ -155,25 +131,20 @@
         """
         from .. import qs_default_console, qs_info_string
         from ..NetTools.NormalDL import size_format
         from ..TuiTools.Table import qs_default_table
         from rich.text import Text
 
         bucket = bucket if bucket else self.df_bucket
-        ls = requirePackage("oss2", "Bucket")(self.auth, self.bucket_url, bucket)
-        tb = qs_default_table(
-            ["File", "Size"] if user_lang != "zh" else ["文件", "体积"], title="Aliyun OSS"
-        )
+        ls = oss2.Bucket(self.auth, self.bucket_url, bucket)
+        tb = qs_default_table(['File', 'Size'] if user_lang != 'zh' else ['文件', '体积'], title='Aliyun OSS')
         prefix = dict()
-        for obj in requirePackage("oss2", "ObjectIterator")(ls):
-            if "/" in obj.key:
-                prefix[obj.key[obj.key[: obj.key.index("/")]]] = 0
-            tb.add_row(
-                Text(obj.key, justify="left"),
-                Text(size_format(obj.size, True), justify="right"),
-            )
+        for obj in oss2.ObjectIterator(ls):
+            if '/' in obj.key:
+                prefix[obj.key[obj.key[:obj.key.index('/')]]] = 0
+            tb.add_row(Text(obj.key, justify='left'), Text(size_format(obj.size, True), justify='right'))
         qs_default_console.print(
             qs_info_string,
-            "Bucket Url:" if user_lang != "zh" else "桶链接:",
-            "https://" + bucket + "." + self.bucket_url + "/",
+            'Bucket Url:' if user_lang != 'zh' else '桶链接:',
+            'https://' + bucket + '.' + self.bucket_url + '/'
         )
         qs_default_console.print(tb, justify="center")
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/API/BaiduCloud.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,104 +3,80 @@
 百度云相关API
 
 Baidu cloud API
 """
 import os
 from . import pre_check, user_lang
 from .. import qs_default_console, qs_error_string, qs_info_string, requirePackage
-
-imgp = requirePackage("aip", "imageprocess", real_name="baidu-aip")
-aip = requirePackage("aip", real_name="baidu-aip")
+aip = requirePackage('aip', real_name='baidu-aip')
 
 
 class ImageDeal:
     """
     百度图像处理类
 
     Baidu image processing class
     """
-
     import base64
 
-    def __init__(
-        self,
-        app_id: str = pre_check("AipImageAPP_ID"),
-        app_key: str = pre_check("AipImageAPP_KEY"),
-        secret_key: str = pre_check("AipImageSECRET_KEY"),
-    ):
+    def __init__(self, app_id: str = pre_check('AipImageAPP_ID'),
+                 app_key: str = pre_check('AipImageAPP_KEY'),
+                 secret_key: str = pre_check('AipImageSECRET_KEY')):
         """
         初始化并登陆百度图像处理
 
         Initialize and log in Baidu image processing
 
         :param app_id: 应用ID
         :param app_key: 应用key
         :param secret_key: 密钥
         """
-        self.client = imgp.AipImageProcess(app_id, app_key, secret_key)
+        self.client = aip.AipImageProcess(app_id, app_key, secret_key)
 
-    def largeImage(self, path: str):
+    def largeImage(self, path: str, st: qs_default_console.status = None):
         """
         放大图片 (图像效果增强)
 
         Enlarge image (Image Enhancement)
 
         :param st: console状态
         :param path: 图片路径
         :return: None
         """
         if not os.path.exists(path) or not os.path.isfile(path):
-            qs_default_console.log(
-                qs_error_string,
-                ("No file named: %s" if user_lang != "zh" else "没有文件: %s") % path,
-            )
+            qs_default_console.log(qs_error_string, ('No file named: %s' if user_lang != 'zh' else '没有文件: %s') % path)
             return
         img_name = os.path.basename(path)
-        img_name = (
-            img_name[: img_name.index(".")] + "_LG." + ".".join(img_name.split(".")[1:])
-        )
-
-        from .. import qs_default_status
-
-        with qs_default_status(
-            f'{"Reading Image" if user_lang != "zh" else "读取图片"}: {path}'
-        ) as status:
-            with open(path, "rb") as f:
+        img_name = img_name[:img_name.index('.')] + '_LG.' + '.'.join(img_name.split('.')[1:])
+
+        with qs_default_console.status(f'{"Reading Image" if user_lang != "zh" else "读取图片"}: {path}') if not st else st as status:
+            with open(path, 'rb') as f:
                 img = f.read()
-            status.update(
-                f'{qs_info_string} {"Dealing..." if user_lang != "zh" else "处理中..."}'
-            )
+            status.update(status=f'{qs_info_string} {"Dealing..." if user_lang != "zh" else "处理中..."}')
             img = self.client.imageQualityEnhance(img)
             try:
-                status.update(
-                    f'{qs_info_string} {"Write to" if user_lang != "zh" else "写入"}: {img_name}'
-                )
-                img = ImageDeal.base64.b64decode(img["image"])
-                with open(img_name, "wb") as f:
+                status.update(status=f'{qs_info_string} {"Write to" if user_lang != "zh" else "写入"}: {img_name}')
+                img = ImageDeal.base64.b64decode(img['image'])
+                with open(img_name, 'wb') as f:
                     f.write(img)
             except:
                 qs_default_console.print(qs_error_string, img)
-        qs_default_console.print(
-            qs_info_string, "Deal Done!" if user_lang != "zh" else "处理完成!"
-        )
+        qs_default_console.print(qs_info_string, "Deal Done!" if user_lang != "zh" else "处理完成!")
 
 
 class AipNLP:
     """
     百度语言处理类
 
     Baidu language processing class
     """
-
-    def __init__(
-        self,
-        appid: str = pre_check("AipNlpAPP_ID"),
-        appkey: str = pre_check("AipNlpAPP_KEY"),
-        sckey: str = pre_check("AipNlpSECRET_KEY"),
-    ):
+    def __init__(self,
+                 appid: str = pre_check("AipNlpAPP_ID"),
+                 appkey: str = pre_check("AipNlpAPP_KEY"),
+                 sckey: str = pre_check("AipNlpSECRET_KEY")):
         """
         初始化并登陆百度语言处理应用
 
         Initialize and log in baidu language processing application
 
         :param appid: 应用ID
         :param appkey: 应用Key
@@ -114,12 +90,12 @@
 
         Text error correction
 
         :param words: 待处理文本
         :return: 处理后的文本 | proceed words
         """
         try:
-            res = self.client.ecnet(words)["item"]["correct_query"]
+            res = self.client.ecnet(words)['item']['correct_query']
         except Exception as e:
             qs_default_console.log(qs_error_string, repr(e))
         else:
             return res
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/API/Lolicon.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/Lolicon.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-from ..NetTools import headers
-from .. import user_lang
+from .. import headers, user_lang
 from . import pre_check
 import requests
 import json
 
-lolicon_token = pre_check("lolicon_token", ext=False)
+lolicon_token = pre_check('lolicon_token', False)
 
 
-def loli_img(keyword: str = ""):
+def loli_img(keyword: str = ''):
     try:
         res = requests.get(
-            "https://api.lolicon.app/setu/",
-            headers=headers,
+            'https://api.lolicon.app/setu/', headers=headers,
             params={
-                "apikey": lolicon_token if lolicon_token else "",
-                "r18": "2",
-                "keyword": keyword,
-                "num": 1,
-                "proxy": "disable",
-            },
+                'apikey': lolicon_token if lolicon_token else '',
+                'r18': '2',
+                'keyword': keyword,
+                'num': 1,
+                'proxy': 'disable'
+            }
         )
     except Exception as e:
         return False, repr(e), False
     else:
         if res.status_code != requests.codes.ok:
-            return (
-                False,
-                ("Get Data Failed" if user_lang != "zh" else "获取图源数据失败"),
-                False,
-            )
+            return False, ("Get Data Failed" if user_lang != 'zh' else "获取图源数据失败"), False
         data = json.loads(res.text)
-        return data["code"] == 0, data["msg"], data["data"]
+        return data['code'] == 0, data['msg'], data['data']
 
 
 def magnet2torrent(hash: str):
     try:
         from ..NetTools import get_fileinfo
         from ..NetTools.NormalDL import normal_dl
-
-        infos = get_fileinfo("https://m2t.lolicon.app/m/" + hash)
+        infos = get_fileinfo('https://m2t.lolicon.app/m/' + hash)
         normal_dl(infos[0], set_name=f'{infos[-1].headers["torrent-name"]}.torrent')
-        return True, "Success"
+        return True, 'Success'
     except Exception as e:
         return False, repr(e)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/API/QiniuOSS.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 # coding=utf-8
 """
 七牛云对象存储API
 
 Qiniu cloud OSS API
 """
-from . import pre_check, user_lang
+from . import pre_check, dir_char, user_lang
 from .. import requirePackage
 
 
 class QiniuOSS:
-    qiniu = requirePackage("qiniu")
+    qiniu = requirePackage('qiniu')
 
-    def __init__(
-        self,
-        ac_key: str = None,
-        sc_key: str = None,
-        df_bucket: str = None,
-    ):
+    def __init__(self, ac_key: str = pre_check('qiniu_ac_key'),
+                 sc_key: str = pre_check('qiniu_sc_key'),
+                 df_bucket: str = pre_check('qiniu_bk_name')):
         """
         初始化并登陆七牛云对象存储
 
         Initializes and logs in qiniu cloud object storage
 
         :param ac_key: Access Key
         :param sc_key: Secret Key
         :param df_bucket: 默认桶名称
         """
-        if not (ac_key and sc_key and df_bucket):
-            ac_key, sc_key, df_bucket = pre_check(
-                "qiniu_ac_key", "qiniu_sc_key", "qiniu_bk_name"
-            )
         self.ac_key = ac_key
         self.sc_key = sc_key
         self.auth = QiniuOSS.qiniu.Auth(self.ac_key, self.sc_key)
         self.df_bucket = df_bucket
         self.bar, self.tid = None, None
 
     def get_func_table(self):
@@ -41,58 +34,46 @@
         获取对象支持的操作
 
         Gets the operations supported by the object
 
         :return: 函数表
         """
         return {
-            "-up": self.upload,
-            "-rm": self.remove,
-            "-cp": self.copy_url,
-            "-dl": self.download,
-            "-ls": self.list_bucket,
+            '-up': self.upload,
+            '-rm': self.remove,
+            '-cp': self.copy_url,
+            '-dl': self.download,
+            '-ls': self.list_bucket
         }
 
-    def upload(self, filePath: str, bucket: str = None, key: str = None):
+    def upload(self, filePath: str, bucket: str = None):
         """
         上传文件
 
         Upload file
 
         :param filePath: 文件路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         import os
-        from .. import dir_char
-
         filename = os.path.basename(filePath)
 
         def progress(cur, total):
             if not self.bar:
                 from ..TuiTools.Bar import DataTransformBar
-
                 self.bar = DataTransformBar()
-                self.tid = self.bar.add_task(
-                    "Transform" if user_lang != "zh" else "传输",
-                    filename=filename,
-                    total=total,
-                )
+                self.tid = self.bar.add_task('Transform' if user_lang != 'zh' else '传输', filename=filename, total=total)
                 self.bar.start()
                 self.bar.start_task(self.tid)
             self.bar.update(self.tid, completed=cur)
 
         filePath = filePath.strip()
         tk = self.auth.upload_token(bucket if bucket else self.df_bucket, filePath)
-        QiniuOSS.qiniu.put_file(
-            tk,
-            key if key else filePath.replace(dir_char, "/"),
-            filePath,
-            progress_handler=progress,
-        )
+        QiniuOSS.qiniu.put_file(tk, filePath.replace(dir_char, '/'), filePath, progress_handler=progress)
         self.bar.stop()
 
     def remove(self, filePath: str, bucket: str = None):
         """
         删除文件
 
         Delete file
@@ -111,38 +92,32 @@
         Copy files through URL (this interface seems to have no egg use, qiniu cloud will not work)
 
         :param filePath: 文件链接
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         bk = QiniuOSS.qiniu.BucketManager(self.auth)
-        bk.fetch(
-            filePath, bucket if bucket else self.df_bucket, filePath.split("/")[-1]
-        )
+        bk.fetch(filePath, bucket if bucket else self.df_bucket, filePath.split('/')[-1])
 
     def get_bucket_url(self, bucket: str = None):
         """
         获取当前桶的访问链接
 
         Gets the access link for the current bucket
 
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: 成功返回json，否则False
         """
         import requests
-
         bucket = bucket if bucket else self.df_bucket
-        url = "http://api.qiniu.com/v6/domain/list?tbl=%s" % bucket
-        res = requests.get(
-            url,
-            headers={
-                "Content-Type": "application/x-www-form-urlencoded",
-                "Authorization": "QBox %s" % self.auth.token_of_request(url),
-            },
-        )
+        url = 'http://api.qiniu.com/v6/domain/list?tbl=%s' % bucket
+        res = requests.get(url, headers={
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Authorization": "QBox %s" % self.auth.token_of_request(url)
+        })
         if res.status_code == requests.codes.ok:
             return res.json()
         else:
             return False
 
     def list_bucket(self, bucket: str = None):
         """
@@ -152,52 +127,42 @@
 
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from .. import qs_default_console, qs_info_string
         from ..TuiTools.Table import qs_default_table
         from rich.text import Text
-
         bk = QiniuOSS.qiniu.BucketManager(self.auth)
         ret = bk.list(bucket if bucket else self.df_bucket)
         if not ret[1]:
-            print("ERROR!" if user_lang != "zh" else "错误!")
+            print("ERROR!" if user_lang != 'zh' else '错误!')
             exit(0)
-        root_url = "http://" + self.get_bucket_url(bucket)[0] + "/"
-        ret = ret[0]["items"]
+        root_url = 'http://' + self.get_bucket_url(bucket)[0] + '/'
+        ret = ret[0]['items']
         from ..NetTools.NormalDL import size_format
-
-        tb = qs_default_table(
-            ["File", "Size"] if user_lang != "zh" else ["文件", "体积"], title="七牛 OSS"
-        )
+        tb = qs_default_table(['File', 'Size'] if user_lang != 'zh' else ['文件', '体积'], title='七牛 OSS')
         for i in ret:
-            tb.add_row(
-                Text(i["key"], justify="left"),
-                Text(size_format(i["fsize"], True), justify="right"),
-            )
-        qs_default_console.print(
-            qs_info_string, "Bucket url:" if user_lang != "zh" else "桶链接:", root_url
-        )
+            tb.add_row(Text(i['key'], justify="left"), Text(size_format(i['fsize'], True), justify='right'))
+        qs_default_console.print(qs_info_string, "Bucket url:" if user_lang != 'zh' else '桶链接:', root_url)
         qs_default_console.print(tb, justify="center")
 
     def download(self, filePath: str, bucket: str = None):
         """
         下载文件
 
         Download file
 
         :param filePath: 文件在桶中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from ..NetTools.NormalDL import normal_dl
-
         bucket = bucket if bucket else self.df_bucket
         root_url = self.get_bucket_url(bucket)[0]
         if root_url:
-            root_url = "http://" + root_url + "/"
+            root_url = 'http://' + root_url + '/'
         else:
-            exit("Get Bucket Url Failed!" if user_lang != "zh" else "获取桶链接失败!")
+            exit('Get Bucket Url Failed!' if user_lang != 'zh' else '获取桶链接失败!')
         dl_url = root_url + filePath
-        if bucket.startswith("admin"):
+        if bucket.startswith('admin'):
             dl_url = self.auth.private_download_url(dl_url)
         normal_dl(dl_url)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/API/SimpleAPI.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     删除图片背景
 
     Delete image background
 
     :param filePath: 图片的路径
     :return: None
     """
-    api_key = pre_check("rmbg")
+    api_key = pre_check('rmbg')
     res = requests.post(
-        "https://api.remove.bg/v1.0/removebg",
-        files={"image_file": open(filePath, "rb")},
-        data={"size": "auto"},
-        headers={"X-Api-Key": api_key},
+        'https://api.remove.bg/v1.0/removebg',
+        files={'image_file': open(filePath, 'rb')},
+        data={'size': 'auto'},
+        headers={'X-Api-Key': api_key},
     )
     if res.status_code == requests.codes.ok:
-        import os
-
-        img_name = os.path.basename(filePath).split(".")[0]
-        img_root = os.path.dirname(os.path.abspath(filePath))
-
-        with open(os.path.join(img_root, img_name + "_rmbg.png"), "wb") as imgfile:
+        img_name = filePath.split(dir_char)[-1].split('.')[0]
+        if dir_char in filePath:
+            img_root = dir_char.join(filePath.split(dir_char)[:-1]) + dir_char
+        else:
+            img_root = ''
+        with open(img_root + img_name + '_rmbg.png', 'wb') as imgfile:
             imgfile.write(res.content)
     else:
         qs_default_console.log(qs_error_string, res.status_code, res.text)
 
 
 def smms(filePath: str):
     """
@@ -44,212 +44,177 @@
 
     Upload images or all images from Markdown to SMMS
 
     :param filePath: 图片或Markdown文件的路径
     :return: None
     """
     import os
-    from .. import user_root
     from ..TuiTools.Table import qs_default_table
 
-    api_key = pre_check("smms")
-    res_tb = qs_default_table(
-        ["File", "Status", "url"] if user_lang != "zh" else ["文件", "状态", "链接"]
-    )
+    api_key = pre_check('smms')
+    res_tb = qs_default_table(['File', 'Status', 'url'] if user_lang != 'zh' else ['文件', '状态', '链接'])
 
     def post_img(path: str) -> dict:
         try:
-            data = {"smfile": (path.split("/")[-1], open(path, "rb")), "format": "json"}
+            data = {
+                'smfile': (path.split('/')[-1], open(path, 'rb')),
+                'format': 'json'
+            }
         except:
             return {}
-        res_json = requests.post(
-            "https://sm.ms/api/v2/upload",
-            headers={"Authorization": api_key},
-            files=data,
-        ).text
+        res_json = requests.post('https://sm.ms/api/v2/upload', headers={'Authorization': api_key}, files=data).text
         return json.loads(res_json)
 
     def get_path(rt, rel):
-        return os.path.abspath(os.path.join(rt, rel))
+        return os.path.abspath(rt + rel)
 
     def format_markdown(path):
         import re
-
-        rt_path = os.path.dirname(os.path.abspath(path))
+        _user_path = os.path.expanduser('~')
+        rt_path = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
         img_set = {}
-        with open(path, "r") as fp:
+        with open(path, 'r') as fp:
             ct = fp.read()
-        aims = re.findall("!\[.*?]\((.*?)\)", ct, re.M) + re.findall(
-            '<img.*?src="(.*?)".*?>', ct, re.M
-        )
+        aims = re.findall('!\[.*?]\((.*?)\)', ct, re.M) + re.findall('<img.*?src="(.*?)".*?>', ct, re.M)
         for aim in aims:
             raw_path = aim
-            aim = get_path(rt_path, aim.replace("~", user_root))
+            aim = aim.replace('~', _user_path)
+            aim = aim if aim.startswith(dir_char) else get_path(rt_path, aim)
             if aim not in img_set:
                 res_dict = post_img(aim)
                 if not res_dict:
-                    res_tb.add_row(os.path.basename(aim), "No File", "")
+                    res_tb.add_row(aim.split(dir_char)[-1], 'No File', '')
                     img_set[aim] = False
                 else:
                     res_tb.add_row(
-                        os.path.basename(aim),
-                        res_dict["success"],
-                        res_dict["message"]
-                        if not res_dict["success"]
-                        else res_dict["data"]["url"],
+                        aim.split(dir_char)[-1], res_dict['success'],
+                        res_dict['message'] if not res_dict['success'] else res_dict['data']['url']
                     )
-                    if not res_dict["success"] and res_dict["code"] == "unauthorized":
+                    if not res_dict['success'] and res_dict['code'] == 'unauthorized':
                         break
-                    img_set[aim] = (
-                        res_dict["data"]["url"] if res_dict["success"] else False
-                    )
+                    img_set[aim] = res_dict['data']['url'] if res_dict['success'] else False
             if img_set[aim]:
                 ct = ct.replace(raw_path, img_set[aim])
-        with open(path, "w") as fp:
+        with open(path, 'w') as fp:
             fp.write(ct)
         qs_default_console.print(res_tb, justify="center")
 
     try:
-        is_md = filePath.endswith(".md")
+        is_md = filePath.endswith('.md')
     except IndexError:
-        exit("Usage: qs {*.md} | {picture}")
+        exit('Usage: qs {*.md} | {picture}')
     else:
         if is_md:
             format_markdown(filePath)
         else:
             res = post_img(filePath)
             if not res:
-                res_tb.add_row(os.path.basename(filePath), "No File", "")
+                res_tb.add_row(filePath.split(dir_char)[-1], 'No File', '')
             else:
                 res_tb.add_row(
-                    os.path.basename(filePath),
-                    res["success"],
-                    "" if not res["success"] else res["data"]["url"],
-                )
+                    filePath.split(dir_char)[-1], res['success'], '' if not res['success'] else res['data']['url'])
             qs_default_console.print(res_tb, justify="center")
 
 
 def imgs_in_url(url: str, save: bool = False):
     """
     提取url中的img标签链接
 
     Extract img tag links from url
 
     :param url:
     :param save:
     :return:
     """
-    from ..NetTools import headers
-
+    from .. import headers
     html = requests.get(url, headers=headers)
     if html.status_code != requests.codes.ok:
-        qs_default_console.log(
-            qs_error_string, "Network Error" if user_lang != "zh" else "网络错误"
-        )
+        qs_default_console.log(qs_error_string, 'Network Error' if user_lang != 'zh' else '网络错误')
         return
     import re
     from ..ImageTools.ImagePreview import image_preview
-
     normal_dl = None
     if save:
         from ..NetTools.NormalDL import normal_dl
 
     imgs = re.findall('<img.*?src="(.*?)".*?>', html.text)
     a_ls = re.findall('<a.*?href="(.*?)".*?>', html.text)
     for i in a_ls:
         aim = i.lower()
-        for j in [".png", ".jpg", "jpeg"]:
+        for j in ['.png', '.jpg', 'jpeg']:
             if j in aim:
                 imgs.append(i)
                 break
     for url in imgs:
-        if not url.startswith("http") or url.endswith("svg"):
+        if not url.startswith('http') or url.endswith('svg'):
             continue
-        url = url.replace("&#46;", ".")
+        url = url.replace('&#46;', '.')
         qs_default_console.log(
-            qs_info_string,
-            "Link:" if user_lang != "zh" else "链接:",
-            url[:100] + ("" if len(url) <= 100 else "..."),
-        )
+            qs_info_string, 'Link:' if user_lang != 'zh' else '链接:', url[:100] + ('' if len(url) <= 100 else '...'))
         if save:
-            file_name = normal_dl(url)
-        else:
-            file_name = url
-        image_preview(file_name, True)
+            normal_dl(url)
+        if system == 'darwin':
+            try:
+                image_preview(url, True)
+            except Exception as e:
+                qs_default_console.log(qs_error_string, repr(e))
 
 
 def acg2():
     """
     随机获取一张acg图片链接
 
     Get a random link to an ACG image
 
     :return: 请求状态, 链接或报错, 宽度, 高度 | status, url or error, width, height
     """
     try:
-        res = requests.get("https://api.luvying.com/acgimg?return=json")
+        res = requests.get('https://api.luvying.com/acgimg?return=json')
     except Exception as e:
         return False, repr(e), None, None
     else:
         import json
-
         res = json.loads(res.text)
-        return (
-            res["code"] == "200",
-            (res["acgurl"] if res["code"] == "200" else "Error"),
-            res["width"],
-            res["height"],
-        )
+        return res['code'] == '200', (res['acgurl'] if res['code'] == '200' else 'Error'), res['width'], res['height']
 
 
-def wallhaven(
-    set_search_url: str = pre_check("wallhaven_aim_url", ext=False),
-    randomOne: bool = False,
-):
+def wallhaven(set_search_url: str = pre_check('wallhaven_aim_url', False), randomOne: bool = False):
     """
     获取wallhaven toplist或指定图片列表
 
     Get wallhaven toplist or specified picture list
 
     :param set_search_url: 用于搜索的URL
     :param randomOne: 随机抽一张返回
     :return: 包含链接的列表 | [link1, link2, ...]
     """
     from .. import qs_default_console, qs_error_string
-    from ..NetTools import headers
+    from . import headers
     import requests
     import re
 
     if not set_search_url:
-        set_search_url = "https://wallhaven.cc/search?categories=010&purity=011&topRange=1M&sorting=toplist&order=desc"
+        set_search_url = 'https://wallhaven.cc/search?categories=010&purity=011&topRange=1M&sorting=toplist&order=desc'
 
-    urlTemplate = "https://w.wallhaven.cc/full/{}/wallhaven-{}"
+    urlTemplate = 'https://w.wallhaven.cc/full/{}/wallhaven-{}'
     html = requests.get(set_search_url, headers=headers)
     if html.status_code != requests.codes.ok:
-        qs_default_console.print(qs_error_string, f"Http Status: {html.status_code}")
+        qs_default_console.print(qs_error_string, f'Http Status: {html.status_code}')
         return None
-    html = re.findall("<section.*?>(.*?)</section", html.text, re.S)[0]
-    lis = re.findall("<li>(.*?)</li", html, re.S)
+    html = re.findall('<section.*?>(.*?)</section', html.text, re.S)[0]
+    lis = re.findall('<li>(.*?)</li', html, re.S)
     res = []
     for i in lis:
-        url, size = re.findall(
-            '<img.*?data-src="(.*?)".*?<span.*?class="wall-res".*?>(.*?)<', i, re.S
-        )[0]
-        url = url.split("/")[-2:]
+        url, size = re.findall('<img.*?data-src="(.*?)".*?<span.*?class="wall-res".*?>(.*?)<', i, re.S)[0]
+        url = url.split('/')[-2:]
         if '<span class="png">' in i:
-            url[-1] = url[-1].replace(".jpg", ".png")
-        res.append(
-            {
-                "url": urlTemplate.format(*url),
-                "size": [int(i) for i in re.findall("\d+\.?\d*", size)],
-            }
-        )
+            url[-1] = url[-1].replace('.jpg', '.png')
+        res.append({'url': urlTemplate.format(*url), 'size': [int(i) for i in re.findall('\d+\.?\d*', size)]})
     if randomOne:
         import random
-
         return [random.choice(res)]
     return res
 
 
 def lmgtfy(keyword: str):
     """
     让我帮你Google一下
@@ -257,64 +222,47 @@
     Let me google that for you
 
     :param keyword: 关键词
     :return: 目标链接 | http link
     """
     import random
     import base64
-
-    supportLs = ["https://moedog.org/tools/google/?q="]
-    return random.choice(supportLs) + base64.b64encode(bytes(keyword, "utf-8")).decode(
-        "utf-8"
-    )
+    supportLs = [
+        'https://moedog.org/tools/google/?q='
+    ]
+    return random.choice(supportLs) + base64.b64encode(bytes(keyword, 'utf-8')).decode('utf-8')
 
 
 class Designation2magnet:
     import re
 
     def __init__(self, description):
-        self.rt_url = "https://18mag.net"
-        self.cover_url = "https://www5.javmost.com/search/{designation}/"
+        self.rt_url = 'https://3mag.net'
         self.description = description
 
     def search_designation(self):
         """
         番号搜索
 
         :return:
         """
         infos = [
-            Designation2magnet.re.findall(
-                '<a.*?href="(.*?)".*?>(.*?)<.*?td-size.*?>(.*?)<',
-                item,
-                Designation2magnet.re.S,
-            )
-            for item in Designation2magnet.re.findall(
-                "<tr>(.*?)</tr>",
-                requests.get(self.rt_url + "/search?q={}".format(self.description))
-                .text.replace("<b>", "")
-                .replace("</b>", ""),
-                Designation2magnet.re.S,
-            )
+            Designation2magnet.re.findall('<a.*?href="(.*?)".*?>(.*?)<.*?td-size.*?>(.*?)<', item, Designation2magnet.re.S) for item in
+            Designation2magnet.re.findall('<tr>(.*?)</tr>', requests.get(self.rt_url + '/search?q={}'.format(self.description)).text.replace('<b>', '').replace('</b>', ''), Designation2magnet.re.S)
         ]
         if [] in infos:
-            return [
-                (i[0][0], i[0][1].strip(), i[0][2]) for i in infos[: infos.index([])]
-            ]
+            return [(i[0][0], i[0][1].strip(), i[0][2]) for i in infos[:infos.index([])]]
         else:
             return [(i[0][0], i[0][1].strip(), i[0][2]) for i in infos]
 
     def get_magnet(self, info: str):
         """
         将选定的信息转为磁力链
 
         :param info:
         :return:
         """
-        return (
-            "magnet:?xt=urn:btih:"
-            + Designation2magnet.re.findall(
-                "种子特征码.*?<dd>(.*?)<",
-                requests.get(self.rt_url + info).text,
-                Designation2magnet.re.S,
-            )[0]
-        )
+        return 'magnet:?xt=urn:btih:' + Designation2magnet.re.findall(
+            '种子特征码.*?<dd>(.*?)<',
+            requests.get(self.rt_url + info).text,
+            Designation2magnet.re.S
+        )[0]
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/API/TencentCloud.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/API/TencentCloud.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,84 @@
 # coding=utf-8
 """
 腾讯云相关API
 
 Tencent cloud API
 """
 import json
-from .. import requirePackage, user_lang
-from . import pre_check
+from .. import requirePackage
+from . import pre_check, user_lang, dir_char
 
 
 class TxCOS:
-    def __init__(self, scid=None, sckey=None, region=None, bucket=None, cdn_url=None):
+    qcloud_cos = requirePackage('qcloud_cos', real_name='cos-python-sdk-v5')
+
+    def __init__(self):
         """
         初始化并登陆腾讯云对象存储
 
         Initialize and log in Tencent Cloud object storage
-
-        :param scid: SecretId
-        :param sckey: SecretKey
-        :param region: 地区
-        :param bucket: 桶名称
-        :param cdn_url: CDN地址
-
-        :return: None
         """
-        if not (scid and sckey and region and bucket):
-            scid, sckey, self.region, self.df_bucket = pre_check(
-                "txyun_scid", "txyun_sckey", "txyun_df_region", "txyun_cos_df_bucket"
-            )
-        self.cdn_url = (
-            pre_check("txyun_df_cdn_url", ext=False) if not cdn_url else cdn_url
-        )
-        if self.cdn_url and not self.cdn_url.endswith("/"):
-            self.cdn_url += "/"
-
-        qcloud_cos = requirePackage("qcloud_cos", real_name="cos-python-sdk-v5")
-
-        config = qcloud_cos.CosConfig(
-            Region=self.region, SecretId=scid, SecretKey=sckey
-        )
-        self.client = qcloud_cos.CosS3Client(config)
+        scid = pre_check('txyun_scid')
+        sckey = pre_check('txyun_sckey')
+        self.region = pre_check('txyun_df_region')
+        self.df_bucket = pre_check('txyun_cos_df_bucket')
+        self.cdn_url = pre_check('txyun_df_cdn_url', ext=False)
+        if self.cdn_url and not self.cdn_url.endswith('/'):
+            self.cdn_url += '/'
+        config = TxCOS.qcloud_cos.CosConfig(Region=self.region,
+                                            SecretId=scid,
+                                            SecretKey=sckey)
+        self.client = TxCOS.qcloud_cos.CosS3Client(config)
 
     def get_func_table(self):
         """
         获取对象支持的函数表
 
         Gets a table of functions supported by the object
 
         :return: 函数表
         """
         return {
-            "-up": self.upload,
-            "-rm": self.remove,
-            "-dl": self.download,
-            "-ls": self.list_bucket,
+            '-up': self.upload,
+            '-rm': self.remove,
+            '-dl': self.download,
+            '-ls': self.list_bucket
         }
 
-    def upload(self, filePath: str, bucket: str = None, key: str = None):
+    def upload(self, filePath: str, bucket: str = None):
         """
         上传文件
 
         Upload file
 
-        :param key: 在COS上的文件路径
         :param filePath: 文件地址
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
-        from .. import dir_char
-
         bucket = bucket if bucket else self.df_bucket
         filename = filePath.strip()
-        self.client.upload_file(
-            Bucket=bucket,
-            LocalFilePath=filename,
-            Key=key if key else filename.replace(dir_char, "/"),
-        )
+        self.client.upload_file(Bucket=bucket, LocalFilePath=filename, Key=filename.replace(dir_char, '/'))
 
     def download(self, filename: str, bucket: str = None):
         """
         下载文件
 
         Download file
 
         :param filename: 文件在桶中的路径
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from ..NetTools.NormalDL import normal_dl
-
         bucket = bucket if bucket else self.df_bucket
 
-        url = (
-            self.cdn_url + filename
-            if bucket == self.df_bucket and self.cdn_url
-            else "https://"
-            + bucket
-            + ".cos."
-            + self.region
-            + ".myqcloud.com/"
-            + filename
-        )
+        url = self.cdn_url + filename \
+            if bucket == self.df_bucket and self.cdn_url else \
+            'https://' + bucket + '.cos.' + self.region + '.myqcloud.com/' + filename
         normal_dl(url)  # * 由于腾讯云没有提供可调用的下载sdk，因此使用qs下载引擎下载
 
     def remove(self, filePath: str, bucket: str = None):
         """
         删除桶中的文件
 
         Delete files in the bucket
@@ -125,111 +99,82 @@
         :param bucket: 桶名称，缺省使用self.df_bucket
         :return: None
         """
         from .. import qs_default_console, qs_info_string
         from ..NetTools.NormalDL import size_format
         from ..TuiTools.Table import qs_default_table
         from rich.text import Text
-
         bucket = bucket if bucket else self.df_bucket
-        ls = self.client.list_objects(Bucket=bucket)["Contents"]
-        tb = qs_default_table(
-            ["File", "Size"] if user_lang != "zh" else ["文件", "体积"], title="Tencnet COS"
-        )
+        ls = self.client.list_objects(Bucket=bucket)['Contents']
+        tb = qs_default_table(['File', 'Size'] if user_lang != 'zh' else ['文件', '体积'], title='Tencnet COS')
         for obj in ls:
-            tb.add_row(
-                Text(obj["Key"], justify="left"),
-                Text(size_format(int(obj["Size"]), align=True), justify="right"),
-            )
-        qs_default_console.print(
-            qs_info_string,
-            "Bucket Url:" if user_lang != "zh" else "桶链接:",
-            self.cdn_url
-            if bucket == self.df_bucket and self.cdn_url
-            else "https://" + bucket + ".cos." + self.region + ".myqcloud.com/",
-        )
+            tb.add_row(Text(obj['Key'], justify='left'), Text(size_format(int(obj['Size']), align=True), justify='right'))
+        qs_default_console.print(qs_info_string, 'Bucket Url:' if user_lang != 'zh' else '桶链接:',
+                                 self.cdn_url if bucket == self.df_bucket and self.cdn_url else
+                                 'https://' + bucket + '.cos.' + self.region + '.myqcloud.com/')
         qs_default_console.print(tb, justify="center")
 
 
 class Translate:
+    requirePackage('tencentcloud', real_name='tencentcloud-sdk-python')
+    detect = requirePackage('langdetect', 'detect')
+    DetectorFactory = requirePackage('langdetect', 'DetectorFactory')
+
+    from tencentcloud.common import credential
+    from tencentcloud.common.profile.client_profile import ClientProfile
+    from tencentcloud.common.profile.http_profile import HttpProfile
+    from tencentcloud.tmt.v20180321 import tmt_client, models
 
-    from tencentcloud.tmt.v20180321 import models
-
-    def __init__(self, scid, sckey, region):
+    def __init__(self, scid: str = pre_check('txyun_scid'), sckey: str = pre_check('txyun_sckey'),
+                 region: str = pre_check('txyun_df_region')):
         """
         初始化并登陆腾讯翻译接口
 
         Initialize and log in Tencent translation interface
 
         :param scid: secret id
         :param sckey: secret key
         :param region: 地区
         """
-        if not (scid and sckey and region):
-            scid, sckey, region = pre_check(
-                "txyun_scid", "txyun_sckey", "txyun_df_region"
-            )
-        requirePackage("langdetect", "DetectorFactory").seed = 0
-        cred = requirePackage(
-            "tencentcloud.common", "credential", real_name="tencentcloud-sdk-python"
-        )
-        http_profile = requirePackage(
-            "tencentcloud.common.profile.http_profile",
-            "HttpProfile",
-            real_name="tencentcloud-sdk-python",
-        )()
+        Translate.DetectorFactory.seed = 0
+        cred = Translate.credential.Credential(scid, sckey)
+        http_profile = Translate.HttpProfile()
         http_profile.endpoint = "tmt.tencentcloudapi.com"
-        clientProfile = requirePackage(
-            "tencentcloud.common.profile.client_profile",
-            "ClientProfile",
-            real_name="tencentcloud-sdk-python",
-        )()
+        clientProfile = Translate.ClientProfile()
         clientProfile.httpProfile = http_profile
-        self.client = requirePackage(
-            "tencentcloud.tmt.v20180321.tmt_client",
-            "TmtClient",
-            real_name="tencentcloud-sdk-python",
-        )(cred, region, clientProfile)
+        self.client = Translate.tmt_client.TmtClient(cred, region, clientProfile)
 
     @staticmethod
     def langdetect(text: str) -> str:
         """
         获取文本的语言类型
 
         Gets the language type of the text
 
         :param text: 待识别文本
         :return: 语言类型
         """
-        return requirePackage("langid", "classify")(text)[0]
+        return Translate.detect(text)
 
-    def translate(
-        self, text: str, from_lang: str = None, target_lang: str = user_lang
-    ) -> str:
+    def translate(self, text: str, from_lang: str = None, to_lang: str = user_lang) -> str:
         """
         翻译文本至默认语言
 
         Translate text to the default language
 
         :param from_lang: 文本语言
-        :param target_lang: 目标语言
+        :param to_lang: 目标语言
         :param text: 文本
         :return: 翻译结果
         """
-        req = requirePackage(
-            "tencentcloud.tmt.v20180321.models", "TextTranslateRequest"
-        )()
-        req.from_json_string(
-            json.dumps(
-                {
-                    "SourceText": text,
-                    "Source": self.langdetect(text) if not from_lang else from_lang,
-                    "Target": target_lang,
-                    "ProjectId": 0,
-                }
-            )
-        )
-        return json.loads(self.client.TextTranslate(req).to_json_string())["TargetText"]
+        req = Translate.models.TextTranslateRequest()
+        req.from_json_string(json.dumps({
+            "SourceText": text,
+            "Source": self.langdetect(text) if not from_lang else from_lang,
+            "Target": to_lang,
+            "ProjectId": 0
+        }))
+        return json.loads(self.client.TextTranslate(req).to_json_string())['TargetText']
 
 
-def translate(text: str, from_lang: str = None, target_lang: str = user_lang) -> str:
-    return Translate().translate(text, from_lang, target_lang)
+def translate(text: str, from_lang: str = None, to_lang: str = user_lang) -> str:
+    return Translate().translate(text, from_lang, to_lang)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/ColorTools.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # coding=utf-8
 """
 修改图像颜色工具
 
 Modify image color tool
 """
-from .. import requirePackage
+from PIL import Image
 
-Image = requirePackage("PIL", "Image")
 
-
-def transport_back(
-    src: str, to_color: tuple, from_color: tuple = (0, 0, 0, 0)
-) -> Image.Image:
+def transport_back(src: str, to_color: tuple, from_color: tuple = (0, 0, 0, 0)) -> Image.Image:
     """
     图片颜色替换
 
     Image color replacement
 
     :param src: 图片路径
     :param to_color: RGBA四元组 -> 转换至目标颜色
     :param from_color: RGBA四元组 -> 需要被转换的颜色
     :return:
     """
     src = Image.open(src)
-    src = src.convert("RGBA")
+    src = src.convert('RGBA')
     L, H = src.size
     color_0 = from_color
     transparency_flag = False if color_0[-1] else True
     for h_indx in range(H):
         for l_indx in range(L):
             dot = (l_indx, h_indx)
             color_1 = src.getpixel(dot)
@@ -48,15 +44,15 @@
     :param to_color: RGBA四元组 -> 转换至目标颜色
     :param except_color: RGBA四元组 -> 忽略的颜色
     :return:
     """
     if except_color is None:
         except_color = [(0, 0, 0, 0)]
     src = Image.open(src)
-    src = src.convert("RGBA")
+    src = src.convert('RGBA')
     L, H = src.size
     for h_indx in range(H):
         for l_indx in range(L):
             color_1 = src.getpixel(dot := (l_indx, h_indx))
             if color_1 not in except_color:
                 src.putpixel(dot, to_color)
     return src
@@ -67,22 +63,17 @@
     解析字符串为RGBA四元组
 
     Parse strings for RGBA quaternions
 
     :param str_color: 表示颜色的字符串(支持16进制、RGB或RGBA) | String representing color (hex, RGB, or RGBA support)
     :return: RGBA四元组 | RGBA quad
     """
-    if "," in str_color:
-        str_color = [int(i) for i in str_color.split(",")]
+    if ',' in str_color:
+        str_color = [int(i) for i in str_color.split(',')]
         if len(str_color) == 3:
             str_color.append(255)
         str_color = tuple(str_color)
     elif len(str_color) == 6:
-        str_color = (
-            int(str_color[:2], 16),
-            int(str_color[2:4], 16),
-            int(str_color[4:], 16),
-            255,
-        )
+        str_color = (int(str_color[:2], 16), int(str_color[2:4], 16), int(str_color[4:], 16), 255)
     else:
-        exit("ERROR COLOR!")
+        exit('ERROR COLOR!')
     return str_color
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/ImageTools/VideoTools.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 # coding=utf-8
 """
 视频处理库, 你需要额外安装moviepy库
 
 Video processing library, you need to install additional moviepy library
 """
 import os
-from .. import user_lang, qs_default_console, qs_error_string, requirePackage
+from .. import dir_char, user_lang, qs_default_console, qs_error_string, requirePackage
 
 
 def VideoWrapper(func):
     """
     视频处理的函数装饰器
 
     Video processing function decorator
 
     :param func: 函数
     :return: wrapper
     """
-
     def wrapper(path, *args, **kwargs):
         if not os.path.exists(path):
-            qs_default_console.log(
-                qs_error_string,
-                f'{"No such file" if user_lang != "zh" else "文件不存在"}: {path}',
-            )
+            qs_default_console.log(qs_error_string, f'{"No such file" if user_lang != "zh" else "文件不存在"}: {path}')
             return
         if not os.path.isfile(path):
-            qs_default_console.log(
-                qs_error_string,
-                f'{"No a file" if user_lang != "zh" else "不是文件"}: {path}',
-            )
-        mpy = requirePackage("moviepy", "editor")
+            qs_default_console.log(qs_error_string, f'{"No a file" if user_lang != "zh" else "不是文件"}: {path}')
+        mpy = requirePackage('moviepy', 'editor')
         func(path, *args, **kwargs, mpy=mpy)
 
     return wrapper
 
 
 @VideoWrapper
 def video_2_gif(path: str, size: tuple = (480, 320), fps: int = None, mpy=None):
@@ -45,83 +38,75 @@
 
     :param mpy: moviepy.editor
     :param path: 视频路径
     :param size: gif尺寸
     :param fps: fps
     :return: None
     """
-    file_name = ".".join(os.path.basename(path).split(".")[:-1]) + ".gif"
-    dir_name = os.path.abspath(os.path.dirname(path))
+    file_name = '.'.join(os.path.basename(path).split('.')[:-1]) + '.gif'
+    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
     ct = mpy.VideoFileClip(path) if not size else mpy.VideoFileClip(path).resize(size)
-    ct.write_gif(os.path.join(dir_name, file_name), fps=fps)
+    ct.write_gif(dir_name + file_name, fps=fps) if fps else ct.write_gif(dir_name + file_name)
 
 
 @VideoWrapper
 def rm_audio(path: str, mpy=None):
     """
     删除视频的音频
 
     Delete the audio of the video
 
     :param mpy: moviepy.editor
     :param path: 视频路径
     :return: None
     """
     file_name = os.path.basename(path)
-    if "." in file_name:
-        indx = file_name.index(".")
-        file_name = file_name[:indx] + "_rm_audio" + file_name[indx:]
-        file_name = file_name.split(".")
-        file_name = ".".join(file_name[:-1]) + ".mp4"
+    if '.' in file_name:
+        indx = file_name.index('.')
+        file_name = file_name[:indx] + '_rm_audio' + file_name[indx:]
+        file_name = file_name.split('.')
+        file_name = '.'.join(file_name[:-1]) + '.mp4'
     else:
-        file_name += "_rm_audio"
-    dir_name = os.path.abspath(os.path.dirname(path))
+        file_name += '_rm_audio'
+    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
     ct = mpy.VideoFileClip(path).set_audio(None)
-    ct.write_videofile(os.path.join(dir_name, file_name))
+    ct.write_videofile(dir_name + file_name)
 
 
 @VideoWrapper
 def tomp4(path: str, mpy=None):
     """
     将视频转为mp4
 
     Convert the video to MP4
 
     :param mpy: moviepy.editor
     :param path: 视频路径
     :return: None
     """
     file_name = os.path.basename(path)
-    file_name = (
-        ".".join(file_name.split(".")[:-1]) + ".mp4"
-        if "." in file_name
-        else file_name + ".mp4"
-    )
-    dir_name = os.path.abspath(os.path.dirname(path))
+    file_name = '.'.join(file_name.split('.')[:-1]) + '.mp4' if '.' in file_name else file_name + '.mp4'
+    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
     ct = mpy.VideoFileClip(path)
-    ct.write_videofile(os.path.join(dir_name, file_name))
+    ct.write_videofile(dir_name + file_name, audio_codec='aac')
 
 
 @VideoWrapper
 def video_2_mp3(path: str, mpy=None):
     """
     提取视频的音频并保存为mp3格式
 
     Extract the audio from the video and save it in MP3 format
 
     :return:
     """
     file_name = os.path.basename(path)
-    file_name = (
-        ".".join(file_name[:-1].split(".")) + ".mp3"
-        if "." in file_name
-        else file_name + ".mp3"
-    )
-    dir_name = os.path.abspath(os.path.dirname(path))
-    mpy.VideoFileClip(path).audio.write_audiofile(os.path.join(dir_name, file_name))
+    file_name = '.'.join(file_name[:-1].split('.')) + '.mp3' if '.' in file_name else file_name + '.mp3'
+    dir_name = dir_char.join(os.path.abspath(path).split(dir_char)[:-1]) + dir_char
+    mpy.VideoFileClip(path).audio.write_audiofile(dir_name + file_name)
 
 
 @VideoWrapper
 def set_video_audio(v_path: str, a_path: str, mpy=None):
     """
     设置视频的音频
 
@@ -129,17 +114,13 @@
 
     :param v_path: 视频路径 | video path
     :param a_path: 音频路径 | audio path
     :param mpy: None, DO NOT SET IT
     :return:
     """
     file_name = os.path.basename(v_path)
-    file_name = (
-        ".".join(file_name.split(".")[:-1]) + "_sta.mp4"
-        if "." in file_name
-        else file_name + "_sta.mp4"
-    )
-    dir_name = os.path.abspath(os.path.dirname(v_path))
+    file_name = '.'.join(file_name.split('.')[:-1]) + '_sta.mp4' if '.' in file_name else file_name + '_sta.mp4'
+    dir_name = dir_char.join(os.path.abspath(v_path).split(dir_char)[:-1]) + dir_char
     v = mpy.VideoFileClip(v_path)
     a = mpy.AudioFileClip(a_path)
     v = v.set_audio(a)
-    v.write_videofile(os.path.join(dir_name, file_name), audio_codec="aac")
+    v.write_videofile(dir_name + file_name, audio_codec='aac')
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/HttpServer.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from socketserver import ThreadingMixIn
 from http.server import SimpleHTTPRequestHandler
 from http.server import HTTPServer
 from .. import qs_default_console, qs_info_string, requirePackage
 
 
 class HttpServers:
-    qrcode_terminal = requirePackage("qrcode_terminal", real_name="qrcode-terminal")
+    qrcode_terminal = requirePackage('qrcode_terminal')
     import signal
 
-    def __init__(self, ip="localhost", port=8000, url=""):
+    def __init__(self, ip='localhost', port=8000, url=''):
         """
         http服务类初始化
 
         HTTP service class initialization
 
         :param ip: 绑定的ip
         :param port: 端口
@@ -37,29 +37,26 @@
         开启http服务
 
         Start the HTTP service
 
         :return: None
         """
         HttpServers.signal.signal(HttpServers.signal.SIGINT, self.shutdown)
-        self.httpd = HttpServers.Server(
-            (self.web_address, self.web_port), SimpleHTTPRequestHandler
-        )
+        self.httpd = HttpServers.Server((self.web_address, self.web_port), SimpleHTTPRequestHandler)
         if not self.bind_url:
-            self.bind_url = "http://" + self.web_address + ":" + str(self.web_port)
+            self.bind_url = 'http://' + self.web_address + ':' + str(self.web_port)
         qs_default_console.print(qs_info_string, self.bind_url)  # * 展示待访问的url
         HttpServers.qrcode_terminal.draw(self.bind_url)  # * 为待访问的url绘制二维码
         try:
             self.httpd.serve_forever()
         except TypeError:
             self.shutdown()
 
     def shutdown(self):
         """
         Ctrl C
         :return: None
         """
         import os
-
         self.httpd.shutdown()
-        qs_default_console.print(qs_info_string, "HTTP Server: Closed.")
+        qs_default_console.print(qs_info_string, 'HTTP Server: Closed.')
         os._exit(0)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/M3u8DL.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,76 +5,71 @@
 The downloader of m3u8 file
 """
 import urllib3
 from concurrent.futures import ThreadPoolExecutor, wait
 import requests
 import os
 import queue
-from .. import (
-    remove,
-    user_lang,
-    qs_default_console,
-    qs_error_string,
-    qs_info_string,
-)
-from . import headers
-
+from .. import dir_char, remove, headers, user_lang, qs_default_console, qs_error_string, qs_info_string
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def merge_file(path, ts_ls, name):
     """
     将全部ts文件合并
 
     Merge all TS files
 
     :param path: 文件夹路径
     :param ts_ls: ts文件路径列表
     :param name: 合并后的ts文件名
     :return:
     """
-    with open(name + ".ts", "wb") as f:
+    if not path.endswith(dir_char):
+        path += dir_char
+    with open(name + '.ts', 'wb') as f:
         for ts in ts_ls:
-            with open(os.path.join(path, ts), "rb") as ff:
+            with open(path + ts, 'rb') as ff:
                 f.write(ff.read())
 
 
 class M3U8DL:
     from rich.progress import Progress, TimeRemainingColumn, TextColumn, BarColumn
 
     proxies = {}
 
-    def __init__(self, target, name, proxy: str = ""):
+    def __init__(self, target, name, proxy: str = ''):
         """
         初始化M3U8下载引擎
 
         Initialize the M3U8 download engine
 
         :param target: 目标url
         :param name: 文件名
         """
-        self.path = ""
+        self.path = ''
         self._cur = 0
         self._all = 0
         self.target = target
         self.name = name
         self.job_queue = queue.Queue()
         if proxy:
-            M3U8DL.proxies = {"http": "http://" + proxy, "https": "https://" + proxy}
+            M3U8DL.proxies = {
+                'http': 'http://'+proxy,
+                'https': 'https://'+proxy
+            }
         self.main_progress = M3U8DL.Progress(
             M3U8DL.TextColumn("[bold blue]{task.fields[taskName]}", justify="right"),
             M3U8DL.BarColumn(bar_width=None),
             "[progress.percentage]{task.percentage:>3.1f}%",
             "•",
             M3U8DL.TimeRemainingColumn(),
-            console=qs_default_console,
-        )
-        self.dl_id = self.main_progress.add_task(
-            "Download", taskName="Downloading" if user_lang != "zh" else "下载中"
+            console=qs_default_console
         )
+        self.dl_id = self.main_progress.add_task("Download", taskName='Downloading' if user_lang != 'zh' else '下载中')
 
     def _dl_one(self, job):
         """
         下载一个ts文件
 
         Download a TS file
 
@@ -83,64 +78,54 @@
         """
         try:
             if job[-1]:
                 pd_url = job[0]
                 c_fule_name = job[1]
                 if not os.path.exists(os.path.join(self.path, c_fule_name)):
                     res = requests.get(pd_url, verify=False, proxies=M3U8DL.proxies)
-                    with open(os.path.join(self.path, c_fule_name), "ab") as f:
+                    with open(os.path.join(self.path, c_fule_name), 'ab') as f:
                         f.write(res.content)
                         f.flush()
             self.main_progress.advance(self.dl_id, 1)
         except Exception as e:
             qs_default_console.log(qs_error_string, repr(e))
             self.job_queue.put(job)
 
     def download(self):
         """
         下载
 
         :return: None
         """
         target = self.target
-        download_path = os.path.join(os.getcwd(), self.name)
+        download_path = os.getcwd() + dir_char + self.name
         self.path = download_path
         if not os.path.exists(download_path):
             os.mkdir(download_path)
         try:
-            all_content = requests.get(
-                target, verify=False, headers=headers, proxies=M3U8DL.proxies
-            ).text
+            all_content = requests.get(target, verify=False, headers=headers, proxies=M3U8DL.proxies).text
         except Exception as e:
             qs_default_console.log(qs_error_string, repr(e))
             return
         if "#EXTM3U" not in all_content:
-            raise Exception("Not M3U8 Link" if user_lang != "zh" else "非M3U8的链接")
+            raise Exception("Not M3U8 Link" if user_lang != 'zh' else "非M3U8的链接")
         if "EXT-X-STREAM-INF" in all_content:
             file_line = all_content.split("\n")
             for line in file_line:
-                if ".m3u8" in line:
+                if '.m3u8' in line:
                     target = target.rsplit("/", 1)[0] + "/" + line
-                    all_content = requests.get(
-                        target, verify=False, headers=headers, proxies=M3U8DL.proxies
-                    ).text
+                    all_content = requests.get(target, verify=False, headers=headers, proxies=M3U8DL.proxies).text
         file_line = all_content.split("\n")
         _rt = target.rsplit("/", 1)[0] + "/"
         tmp = []
         for index, line in enumerate(file_line):
             if "#EXT-X-KEY" in line:
                 tmp.append((_rt, line, 0))
             if "EXTINF" in line:
-                tmp.append(
-                    (
-                        _rt + file_line[index + 1],
-                        file_line[index + 1].rsplit("/", 1)[-1],
-                        1,
-                    )
-                )
+                tmp.append((_rt + file_line[index + 1], file_line[index + 1].rsplit("/", 1)[-1], 1))
         file_line = tmp[::-1]
         self._all = len(file_line)
         tmp = [jb[1] for jb in file_line]
 
         self.main_progress.update(self.dl_id, total=len(file_line))
         for i in file_line:
             self.job_queue.put(i)
@@ -150,15 +135,11 @@
         while not self.job_queue.empty():
             cur_work = []
             while not self.job_queue.empty():
                 cur_work.append(pool.submit(self._dl_one, self.job_queue.get()))
             wait(cur_work)
         self.main_progress.stop()
 
-        qs_default_console.print(
-            qs_info_string,
-            "Download completed! Start merge.."
-            if user_lang != "zh"
-            else "下载完成! 开始合并..",
-        )
+        qs_default_console.print(qs_info_string, "Download completed! Start merge.."
+                                 if user_lang != 'zh' else '下载完成! 开始合并..')
         merge_file(download_path, tmp, self.name)
         remove(download_path)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/MultiSingleDL.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,260 +1,284 @@
-from . import size_format, get_fileinfo, headers
+# coding=utf-8
+"""
+qs的普通文件下载器！干翻迅雷，并且支持设置代理，设置referer，好看的命令行交互，啥j8文件都能下；(仅支持http[s]协议)
+
+QS ordinary file downloader! Dry out Thunder, and support to set the proxy, set the Referer,
+good-looking command line interaction, and it can download fuck any files; (only supports HTTP[S])
+
+Author: RhythmLian (https://rhythmlian.cn)
+"""
+from . import size_format, get_fileinfo
 from concurrent.futures import ThreadPoolExecutor, wait
+from ..ThreadTools import FileWriters
 from ..SystemTools import get_core_num
-from ..TuiTools.Bar import NormalProgressBar
-from .. import (
-    user_lang,
-    qs_default_console,
-    qs_default_status,
-    qs_error_string,
-    qs_info_string,
-    qs_warning_string,
-)
+from .. import user_lang, qs_default_console, qs_error_string, qs_info_string, qs_warning_string, headers
 from threading import Lock
 from requests import get
+import signal
 import queue
 import time
+import sys
 import os
 
-core_num = min(get_core_num() * 4, 16)
+core_num = get_core_num()
+maxBlockSize = int(5e6)
+minBlockSize = int(5e5)
 
 
-class MultiSingleDL:
-    def __init__(
-        self,
-        urls: list,
-        rt_dir: str,
-        proxy: str = "",
-        referer: str = "",
-        failed2exit: bool = False,
-        save_to_mem: bool = False,
-    ):
-        self.proxy = proxy
-        self.referer = referer
-        self.proxies = (
-            {"http": "http://" + proxy, "https": "https://" + proxy} if proxy else {}
-        )
-        self.headers = headers
-        if referer:
-            self.headers["Referer"] = referer
-        self.rt_dir = rt_dir
-        self.failed2exit = failed2exit
-        self.save_to_mem = save_to_mem
-        self.status_dict = {}
-        self.infos = {}
-        self.urls = set(urls)
-        self.task_num = len(self.urls)
-        if self.save_to_mem:
-            self.content_ls = [b""] * self.task_num
-        self.cur_task_num = 0
-        self.task_num_lock = Lock()
-        self.max_retry = 3
-        self.job_queue = queue.Queue()
-        self.pool = None
-        self.status = qs_default_status("获取文件信息中...")
-        self.progress, self.task_id = NormalProgressBar("多文件下载", self.task_num)
-
-    def _info(self, url):
-        retry = 3
-        while retry:
-            real_url, name, r = get_fileinfo(url, self.proxy, self.referer)
-            if all([real_url, name, r]):
-                break
-            retry -= 1
+def GetBlockSize(sz):
+    """
+    自动规划块大小
+
+    Automatically program the block size
+
+    :param sz: 文件大小
+    :return: 块大小
+    """
+    if sz >= maxBlockSize << 10:
+        return maxBlockSize
+    elif sz <= minBlockSize << 3:
+        return minBlockSize
+    else:
+        return max(sz >> 9, minBlockSize)
+
+
+def ask_overwrite(path: str):
+    from PyInquirer import prompt
+
+    return prompt({
+        'type': 'confirm',
+        'name': 'overwrite',
+        'message': f'"{path}" 已存在, 是否覆盖?' if user_lang == 'zh' else f'"{path}" already exists, overwrite?',
+        'default': False
+    })['overwrite']
+
+
+class Downloader:
+    from ..TuiTools.Bar import DataTransformBar
+
+    def __init__(self, url: str, num: int, name: str = '', proxy: str = '',
+                 referer: str = '', output_error: bool = False, failed2exit: bool = False, exit_if_exist: bool = False,
+                 disableStatus: bool = False, disableParallel: bool = False):
+        """
+        qs普通文件下载引擎
+
+        Qs general file download engine
 
+        :param url: 文件url
+        :param num: 线程数量
+        """
+        signal.signal(signal.SIGINT, self._kill_self)
         info_flag = True
-        if not (real_url and name and r):
+        self.url, self.num, self.output_error, self.proxies = url, num, output_error, {}
+        self.exit_if_exist = exit_if_exist
+        self.enabled = True
+        if not disableStatus:
+            with qs_default_console.status('Getting file info..' if user_lang != 'zh' else '获取文件信息中..'):
+                self.url, self.name, r = get_fileinfo(url, proxy, referer)
+        else:
+            self.url, self.name, r = get_fileinfo(url, proxy, referer)
+        if not (self.url and self.name and r):
             info_flag = False
-            qs_default_console.print(
-                qs_error_string if self.failed2exit else qs_warning_string,
-                f"{url}: Get File information failed, please check network!"
-                if user_lang != "zh"
-                else "获取文件信息失败，请检查网络!",
-                (real_url, name, r)
-            )
-            if self.failed2exit:
+            qs_default_console.print(qs_error_string if failed2exit else qs_warning_string,
+                                     'Get File information failed, please check network!'
+                                     if user_lang != 'zh' else '获取文件信息失败，请检查网络!')
+            if failed2exit:
                 self.enabled = False
                 return
+        if self.name and '.' not in self.name:
+            self.name = os.path.basename(url)
+        if name:
+            self.name = name
+
+        if os.path.exists(self.name) and self.exit_if_exist:
+            self.enabled = False
+            return
+
+        if proxy:
+            self.proxies = {
+                'http': 'http://'+proxy,
+                'https': 'https://'+proxy
+            }
+        self.headers = headers
+        if referer:
+            self.headers['Referer'] = referer
+        if not self.url:
+            qs_default_console.print(qs_error_string, self.name)
+            raise Exception('Connection Error!' if user_lang != 'zh' else '连接失败!')
+        try:
+            if not info_flag:
+                raise KeyError
+            self.size = int(r.headers['content-length'])
+            self.main_progress = Downloader.DataTransformBar()
+            self.dl_id = self.main_progress.add_task('Download', filename=self.name, start=False)
+            self.main_progress.update(self.dl_id, total=self.size)
+            if self.size < 5e6 or disableParallel:
+                qs_default_console.print(qs_info_string, 'FILE SIZE' if user_lang != 'zh' else '文件大小'
+                                         , size_format(self.size))
+                self.size = -self.size
+            else:
+                self.fileBlock = GetBlockSize(self.size)
+        except KeyError:
+            self.size = -1
+            self.main_progress = Downloader.DataTransformBar(False)
+            self.dl_id = self.main_progress.add_task('Download', filename=self.name, start=False)
+        if self.size > 0:
+            self.pool = ThreadPoolExecutor(max_workers=self.num)
+            self.futures, self.fileLock = [], Lock()
+            self.job_queue = queue.Queue()
+            if os.path.exists(self.name + '.qs_dl'):
+                self.ctn_file = open(self.name + '.qs_dl', 'r+')
+                self.ctn = [int(i) for i in self.ctn_file.read().strip().split()]
+            else:
+                self.ctn_file = open(self.name + '.qs_dl', 'w')
+                self.ctn = []
+            self.writers = FileWriters(self.name, max(2, int(core_num / 2)), "rb+" if self.ctn else "wb")
+            qs_default_console.print(qs_info_string, 'FILE  SIZE' if user_lang != 'zh' else '文件大小'
+                                     , size_format(self.size, align=True))
+            qs_default_console.print(qs_info_string, 'THRAED NUM' if user_lang != 'zh' else '线程数量'
+                                     , '%7d' % num)
+
+    def _kill_self(self, signum, frame):
+        """
+        终止下载任务，保存断点
+
+        Terminate the download and save the breakpoint
+
+        :param signum: 信号
+        :param frame: frame
+        :return: None
+        """
+        if self.size > 0:
+            self.main_progress.stop_task(self.dl_id)
+            self.main_progress.stop()
+            qs_default_console.print(qs_info_string,
+                                     'Get Ctrl-C, exiting...' if user_lang != 'zh' else '捕获Ctrl-C, 正在退出...')
+            self.ctn_file.close()
+            self.pool.shutdown(wait=False)
+            self.writers.wait()
+            qs_default_console.print(qs_info_string, 'Deal Done!' if user_lang != 'zh' else '处理完成!')
+        os._exit(0)
 
-        self.infos[url] = {
-            "url": real_url,
-            "name": os.path.basename(url) if name and "." not in name else name,
-            "size": -1
-            if not info_flag
-            else int(r.headers["content-length"])
-            if "content-length" in r.headers
-            else -1,
-        }
-
-        self.task_num_lock.acquire()
-        self.cur_task_num += 1
-        total = sum([self.infos[i]["size"] for i in self.infos if self.infos[i]["size"] != -1])
-        self.status.update(f"获取文件信息中 [bold cyan]{self.cur_task_num}[/]/[bold]{self.task_num}[/]: [bold green]{size_format(total)}[/]")
-        self.task_num_lock.release()
+    def _dl(self, start):
+        """
+        执行文件块下载任务
+
+        Perform the file block download task
 
-    def _dl(self, url, filename, job_id, retry=0):
+        :param start: 文件块起始偏移量
+        :return: None
+        """
         try:
-            r = get(
-                self.infos[url]["url"],
-                stream=True,
-                proxies=self.proxies,
-                headers=self.headers,
-            )
-            if not self.save_to_mem:
-                with open(os.path.join(self.rt_dir, filename), "wb") as f:
-                    for chunk in r.iter_content(32768):
-                        f.write(chunk)
-            else:
-                for chunk in r.iter_content(32768):
-                    self.content_ls[job_id] += chunk
-            self.progress.advance(self.task_id, 1)
+            _sz = min(start + self.fileBlock, self.size - 1)
+            _headers = self.headers.copy()
+            _headers['Range'] = 'bytes={}-{}'.format(start, _sz)
+            _content = b''
+            for chunk in get(self.url, headers=_headers, timeout=50, proxies=self.proxies).iter_content(65536):
+                _content += chunk
+                self.main_progress.advance(self.dl_id, sys.getsizeof(chunk))
+            self.writers.new_job(_content, start)
         except Exception as e:
-            if retry < self.max_retry:
-                self.progress.print(
-                    qs_warning_string,
-                    f'"{url}": task anomaly, ' if user_lang != "zh" else f'"{url}": 任务异常, ',
-                    "retrying..." if user_lang != "zh" else "正在重试...",
-                )
-                self.job_queue.put(
-                    {
-                        "url": url,
-                        "filename": filename,
-                        "job_id": job_id,
-                        "retry": retry + 1,
-                    }
-                )
-            else:
-                self.progress.print(
-                    qs_error_string,
-                    f'"{url}":',
-                    "Download failed!" if user_lang != "zh" else "下载失败！",
-                )
-                self.status_dict[url] = "failed"
-                self.progress.advance(self.task_id, 1)
+            if self.output_error:
+                qs_default_console.print(qs_error_string, repr(e))
+            self.job_queue.put(start)
+        else:
+            self.fileLock.acquire()
+            self.ctn.append(start)
+            self.ctn_file.write('%d\n' % start)
+            self.fileLock.release()
 
-    def run(self, name_map: dict = None, qps: int = None, qps_info:int = None, qps_download: int = None, without_output: bool = False, without_info: bool = False):
+    def _single_dl(self):
         """
-        :param name_map: {url: filename}
-        :param qps: qps for download
-        :param qps_info: qps for get file info
-        :param qps_download: qps for download
-        :param without_output: without output
-        :param without_info: without get file info
+        无法并行下载或无需并行下载时采用串行下载
+
+        Parallel downloads are not possible or serial downloads are not required
+
+        :return: None
         """
-        self.qps = qps
-        qps_info = qps_info if qps_info else qps
-        qps_download = qps_download if qps_download else qps
-
-        self.status.start()
-        if qps_info:
-            self.pool = ThreadPoolExecutor(max_workers=qps_info)
-            wait([self.pool.submit(self._info, item) for item in self.urls])
+        r = get(self.url, stream=True, proxies=self.proxies, headers=self.headers)
+        flag = self.size != -1
+
+        if flag:
+            self.main_progress.start_task(self.dl_id)
         else:
-            self.pool = ThreadPoolExecutor(max_workers=core_num)
-            wait([self.pool.submit(self._info, item) for item in self.urls])
-        self.pool.shutdown(wait=True)
-
-        if name_map:
-            from .. import requirePackage
-            file_suffix = requirePackage('.SystemTools', 'file_suffix')
-
-        total = sum([self.infos[i]["size"] for i in self.infos])
-        failed_num = [self.infos[i]["size"] for i in self.infos].count(-1)
-        if not without_output:
-            qs_default_console.print(
-                qs_info_string,
-                f"获取文件信息完毕! 文件总大小: {size_format(total)} | 未获取到详细信息条数为: {failed_num}",
-            )
-        self.status.stop()
-
-        for _id, item in enumerate(self.urls):
-            self.job_queue.put(
-                {"url": item,
-                    "filename": self.infos[item]["name"], "job_id": _id}
-                if not name_map
-                else {"url": item, "filename": f'{name_map[item]}.{file_suffix(self.infos[item]["name"])}', "job_id": _id}
-            )
-
-        self.progress.start()
-        wait_list = []
-        self.pool = ThreadPoolExecutor(max_workers=qps_download) if qps_download else ThreadPoolExecutor(max_workers=core_num)
-        while not self.job_queue.empty():
-            while not self.job_queue.empty():
-                job = self.job_queue.get()
-                wait_list.append(self.pool.submit(self._dl, **job))
-            wait(wait_list)
-        self.progress.stop()
-        return (
-            [os.path.join(self.rt_dir, self.infos[i]["name"])
-             for i in self.infos]
-            if not name_map
-            else [os.path.join(self.rt_dir, f'{name_map[i]}.{file_suffix(self.infos[i]["name"])}') for i in self.infos]
-        )
-
-    def get_content_ls(self):
-        return self.content_ls
-
-
-def multi_single_dl(
-    urls: list,
-    rt_dir: str = "./",
-    proxy: str = "",
-    referer: str = "",
-    failed2exit: bool = False,
-    name_map: dict = None,
-    qps: int = 0,
-    qps_info: int = 0,
-    qps_download: int = 0,
-    without_output: bool = False,
-):
-    """
-    并行多个小文件下载
+            self.main_progress.update(self.dl_id, total=-1)
+        with open(self.name, 'wb') as f:
+            for chunk in r.iter_content(32768):
+                f.write(chunk)
+                self.main_progress.advance(self.dl_id, sys.getsizeof(chunk))
 
-    :param urls: 小文件的URL
-    :param rt_dir: 文件下载目录
-    :param proxy: 代理
-    :param referer: referer
-    :param failed2exit: 信息获取失败立即退出
-    :param name_map: 文件命名映射{URL: filename}, 后缀名会自动获取并添加
-    :param qps: 限制每秒请求次数, qps_info和qps_download默认为qps
-    :param qps_info: 限制每秒获取信息次数
-    :param qps_download: 限制每秒下载次数
-    :param without_output: 不输出信息
-    :return: 下载好的文件路径列表
-    """
-    return MultiSingleDL(
-        urls=urls, rt_dir=rt_dir, proxy=proxy, referer=referer, failed2exit=failed2exit
-    ).run(name_map=name_map, qps=qps, qps_info=qps_info, qps_download=qps_download, without_output=without_output)
+    def run(self):
+        """
+        规划下载任务并开始下载
+
+        qs可以有效应对网络问题对下载任务造成的影响，如：
+          1.下载过程中切换代理
+
+          2.链路异常
+        并确保下载任务顺利完成
 
+        :return: None
+        """
+        if not self.enabled:
+            return self.name if self.exit_if_exist else ''
+        self.main_progress.start()
+        if self.size > 0:
+            self.main_progress.start_task(self.dl_id)
+            if not self.ctn:
+                with open(self.name, "wb") as fp:
+                    fp.truncate(self.size)
+            self.main_progress.advance(self.dl_id, self.fileBlock*len(self.ctn))
+            for i in range(0, self.size, self.fileBlock):
+                if self.ctn and i in self.ctn:
+                    continue
+                else:
+                    self.job_queue.put(i)
+            retry_cnt = 0
+            while not self.job_queue.empty():
+                self.futures.clear()
+                while not self.job_queue.empty():
+                    cur = self.job_queue.get()
+                    if cur not in self.ctn:
+                        self.futures.append(self.pool.submit(self._dl, cur))
+                wait(self.futures)
+                if not self.job_queue.empty() and retry_cnt > 2:
+                    qs_default_console.print(qs_warning_string, 'Exists File Block Lost, Retrying after 0.5 sec'
+                                             if user_lang != 'zh' else '存在文件块丢失，0.5秒后重试')
+                    time.sleep(0.5)
+                retry_cnt += 1
+            self.writers.wait()
+            self.ctn_file.close()
+            os.remove(self.name + '.qs_dl')
+        else:
+            self._single_dl()
+        self.main_progress.stop()
+        qs_default_console.print(qs_info_string, self.name, 'download done!' if user_lang != 'zh' else '下载完成!')
+        return self.name
 
-def multi_single_dl_content_ls(
-    urls: list,
-    rt_dir: str = "./",
-    proxy: str = "",
-    referer: str = "",
-    failed2exit: bool = False,
-    qps: int = 0,
-    without_output: bool = False,
-):
+
+def normal_dl(url, set_name: str = '', set_proxy: str = '', set_referer: str = '',
+              thread_num: int = min(16, core_num * 4), output_error: bool = False, failed2exit: bool = False, exit_if_exist: bool = False,
+              disableStatus: bool = False, disableParallel: bool = False):
     """
-    并行多个小文件下载
+    自动规划下载线程数量并开始并行下载
+
+    Automatically schedule the number of download threads and begin parallel downloads
 
-    :param urls: 小文件的URL
-    :param rt_dir: 文件下载目录
-    :param proxy: 代理
-    :param referer: referer
-    :param failed2exit: 信息获取失败立即退出
-    :param qps: 限制每秒请求次数
-    :param without_output: 不输出信息
-    :return: 存储在内存中的文件内容列表
+    :param disableStatus:
+    :param url: 文件url
+    :param set_name: 设置文件名（默认采用url所指向的资源名）
+    :param set_proxy: 设置代理（默认无代理）
+    :param set_referer: 设置referer
+    :param thread_num: 线程数
+    :param output_error: 输出报错信息
+    :param failed2exit: 获取文件信息失败则不下载，否则qs将继续尝试下载
+    :param disableStatus: 是否显示当前任务状态
+    :return: file name
     """
-    dl = MultiSingleDL(
-        urls=urls,
-        rt_dir=rt_dir,
-        proxy=proxy,
-        referer=referer,
-        failed2exit=failed2exit,
-        save_to_mem=True,
-    )
-    dl.run(qps=qps, without_output=without_output)
-    return dl.get_content_ls()
+    if set_name and os.path.exists(set_name) and not ask_overwrite(set_name):
+        return ''
+    return Downloader(
+        url=url, num=thread_num, name=set_name, proxy=set_proxy,
+        referer=set_referer, output_error=output_error, failed2exit=failed2exit, exit_if_exist=exit_if_exist,
+        disableStatus=disableStatus, disableParallel=disableParallel
+    ).run()
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/WiFi.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 qs的WIFI模块, 协助连接WIFI, 但不支持机构WIFI自动登录
 
 The WiFi module of QS helps to connect WiFi, but does not support the automatic login of institutional WiFi
 """
 import time
 from .. import user_lang, qs_default_console, qs_error_string, requirePackage
 
-const = requirePackage("pywifi", "const")
-PyWiFi = requirePackage("pywifi", "PyWiFi")
+const = requirePackage('pywifi', 'const')
+PyWiFi = requirePackage('pywifi', 'PyWiFi')
 
 
 class WiFi:
     def __init__(self) -> None:
         """
         qs的wifi工具 (Windows 或 Linux)
         """
@@ -25,15 +25,15 @@
         判断当前wifi连接状态
 
         Determine the current wifi connection status
 
         :return: 连接的wifi名 | The name of the connecting wifi
         """
         flag = self.iface.status() in [const.IFACE_CONNECTED, const.IFACE_CONNECTING]
-        return self.iface.name if flag else ""
+        return self.iface.name if flag else ''
 
     def scan(self):
         """
         扫描附近可连接的wifi
 
         Scan for nearby wifi connections
 
@@ -55,57 +55,47 @@
         Set Network port
 
         :return: None
         """
         num = len(self.ifaces)
         if num <= 0:
             qs_default_console.log(
-                qs_error_string,
-                "There is no recognizable network card interface"
-                if user_lang != "zh"
-                else "没有可识别的网卡接口",
-            )
+                qs_error_string, "There is no recognizable network card interface"
+                if user_lang != 'zh' else '没有可识别的网卡接口')
             return
         elif num != 1:
             from ..TuiTools.Table import qs_default_table
-
-            table = qs_default_table(
-                ["id", "interface"] if user_lang != "zh" else ["序号", "网卡"]
-            )
+            table = qs_default_table(['id', 'interface'] if user_lang != 'zh' else ['序号', '网卡'])
             for i, w in enumerate(self.ifaces):
                 table.add_row(str(i), w.name())
             qs_default_console.print(table)
             while True:
-                iface_no = input(
-                    "请选择网卡接口序号: " if user_lang != "zh" else "Select interface by id: "
-                )
+                iface_no = input('请选择网卡接口序号: ' if user_lang != 'zh' else 'Select interface by id: ')
                 try:
                     no = int(iface_no)
                     if 0 <= no < num:
                         self.iface = self.ifaces[no]
                         break
                 except:
                     continue
         else:
-            qs_default_console.print(
-                f"{'Only one' if user_lang != 'zh' else '仅有可用'}: {self.iface.name()}"
-            )
+            qs_default_console.print(f"{'Only one' if user_lang != 'zh' else '仅有可用'}: {self.iface.name()}")
 
     def conn(self, ssid, password):
         """
         连接WiFi
 
         connect WiFi
 
         :param ssid: wifi名称
         :param password: 密码
         :return: status
         """
         # from pywifi import Profile
-        Profile = requirePackage("pywifi", "Profile")
+        Profile = requirePackage('pywifi', 'Profile')
         self.iface.disconnect()
         time.sleep(1)
         pinfo = Profile()
         pinfo.ssid = ssid
         pinfo.auth = const.AUTH_ALG_OPEN
         pinfo.akm.append(const.AKM_TYPE_WPA2PSK)
         pinfo.cipher = const.CIPHER_TYPE_CCMP
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,70 +12,67 @@
 class WiFi:
     def __init__(self) -> None:
         """
         适用于Mac OS X的wifi工具
 
         Wifi tools for Mac OS X
         """
-        with os.popen("networksetup -listallhardwareports") as pipe:
+        with os.popen('networksetup -listallhardwareports') as pipe:
             ifaces = pipe.read()
-        ifaces = [i.split("\n") for i in ifaces.strip().split("\n\n")]
-        ifaces.remove(["VLAN Configurations", "==================="])
+        ifaces = [i.split('\n') for i in ifaces.strip().split('\n\n')]
+        ifaces.remove(['VLAN Configurations', '==================='])
         self.ifaces = ifaces
         for i in self.ifaces:
-            if i[0].endswith("Wi-Fi"):
+            if i[0].endswith('Wi-Fi'):
                 self.iface = [j.split()[-1] for j in i[1:]]
                 return
 
     def status(self) -> str:
         """
         判断当前wifi连接状态
 
         Determine the current wifi connection status
 
         :return: 连接的wifi名 | The name of the connecting wifi
         """
-        with os.popen("networksetup -getairportnetwork %s" % self.iface[0]) as pipe:
+        with os.popen('networksetup -getairportnetwork %s' % self.iface[0]) as pipe:
             res = pipe.read().strip()
-            res = re.sub(".*?:", "", res).strip()
-        qs_default_console.print(
-            qs_info_string, f"{'已' if res else '未'}连接", res if res else ""
-        )
+            res = re.sub('.*?:', '', res).strip()
+        qs_default_console.print(qs_info_string, f"{'已' if res else '未'}连接", res if res else '')
         return res
 
     @staticmethod
     def scan():
         """
         扫描附近可连接的wifi
 
         Scan for nearby wifi connections
 
         :return: 按信号强度排序好的可连接wifi列表 | A list of available wifi connections sorted by signal strength
         """
+        from . import is_mac
         with os.popen(
-            "/System/Library/PrivateFrameworks/Apple80211.framework/Versions/A/Resources/airport scan"
-        ) as pipe:
-            res = pipe.read().strip().split("\n")[1:]
+                '/System/Library/PrivateFrameworks/Apple80211.framework/Versions/A/Resources/airport scan') as pipe:
+            res = pipe.read().strip().split('\n')[1:]
             tmp_ls = [i.strip().split() for i in res]
             has_add = set()
             res = []
             for i in tmp_ls:
-                # mac_index = 0
-                # while mac_index < len(i):
-                #     if is_mac(i[mac_index]):
-                #         break
-                #     else:
-                #         mac_index += 1
-                # if mac_index >= len(i):
-                #     qs_default_console.log(qs_warning_string, "Failed to get info with:", i)
-                #     continue
-                index = i.index("--") - 3
-                ssid = " ".join(i[:index])
-                if ssid not in has_add:
-                    res.append([ssid, int(i[index]), i[-1]])
+                mac_index = 0
+                while mac_index < len(i):
+                    if is_mac(i[mac_index]):
+                        break
+                    else:
+                        mac_index += 1
+                if mac_index >= len(i):
+                    qs_default_console.log(qs_warning_string, "Failed to get info with:", i)
+                    continue
+                ssid = ' '.join(i[:mac_index])
+                if i[0] not in has_add:
+                    res.append([ssid, int(i[mac_index+1]), i[-1]])
                     has_add.add(ssid)
         return sorted(res, key=lambda x: x[1], reverse=True)
 
     def set_iface(self):
         raise NotImplementedError
 
     def conn(self, ssid: list, password: str):
@@ -84,17 +81,12 @@
 
         connect WiFi
 
         :param ssid: wifi名称
         :param password: 密码
         :return: status
         """
-        from .. import external_exec
-
-        external_exec(
-            'networksetup -setairportnetwork %s %s "%s"'
-            % (self.iface[0], ssid[0], password)
-        )
+        os.system('networksetup -setairportnetwork %s %s "%s"' % (self.iface[0], ssid[0], password))
         return self.status()
 
     def disconn(self):
         return NotImplementedError
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/NetTools/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/NetTools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 qs的网络工具库
 
 The network tool library of QS
 """
 import socket
 import requests
 from requests.exceptions import RequestException
-from typing import Tuple
 
 
 headers = {
-    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/604.4.7 (KHTML, like Gecko) "
-    "Version/11.0.2 Safari/604.4.7"
-}
+    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_2) AppleWebKit/604.4.7 (KHTML, like Gecko) '
+                  'Version/11.0.2 Safari/604.4.7'}
 
 
 def is_ipv4(ip: str) -> bool:
     """
     判断ip是否为可连接的ipv4
 
     Determine whether the IP is a connectable IPv4
@@ -27,15 +25,15 @@
     try:
         socket.inet_pton(socket.AF_INET, ip)
     except AttributeError:  # no inet_pton here, sorry
         try:
             socket.inet_aton(ip)
         except socket.error:
             return False
-        return ip.count(".") == 3
+        return ip.count('.') == 3
     except socket.error:  # not a valid ip
         return False
     return True
 
 
 def is_ipv6(ip: str) -> bool:
     """
@@ -56,36 +54,36 @@
     """
     判断ip是否为可连接的
 
     Determine whether the IP is a connectable
     :param ip: like fe80::1862:5a79:a8a0:aae5, 8.8.8.8 etc.
     :return: bool
     """
-    if ip == "localhost":
+    if ip == 'localhost':
         return True
     return is_ipv4(ip) or is_ipv6(ip)
 
 
 def is_mac(addr: str) -> bool:
     """
     检查addr是否为mac地址
 
     Check whether addr is a mac address
 
     :param addr: string like '80:8f:1d:e2:f2:f5'
     :return: bool
     """
-    part = addr.split(":")
+    part = addr.split(':')
     if len(part) != 6:
         return False
     for i in part:
         if len(i) != 2:
             return False
         for j in i:
-            if j not in "0123456789abcdefABCDEF":
+            if j not in '0123456789abcdefABCDEF':
                 return False
     return True
 
 
 def check_one_page(url: str) -> bool:
     """
     检查url是否可访问
@@ -107,52 +105,50 @@
     为url添加https或http使其能被访问
 
     Add HTTPS or HTTP to the URL to make it accessible
 
     :param try_url: 待尝试的url
     :return: 能被成功访问的url
     """
-    if try_url.startswith("http://") or try_url.startswith("https://"):
+    if try_url.startswith('http://') or try_url.startswith('https://'):
         return try_url
     res_url = try_url
     if not check_one_page(res_url):
-        res_url = "https://" + try_url
+        res_url = 'https://' + try_url
         if not check_one_page(res_url):
-            res_url = "http://" + try_url
+            res_url = 'http://' + try_url
     return res_url
 
 
 def open_url(url: str):
     """
     使用默认浏览器打开url
 
     Open url using the default browser
 
     :param url:
     :return:
     """
     import webbrowser as wb
-
     url = formatUrl(url)
     wb.open_new_tab(url)
 
 
 def get_ip() -> str:
     """
     获取本机ip
 
     Get native IP
 
     :return: ip
     """
     import socket
-
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
-        s.connect(("8.8.8.8", 80))
+        s.connect(('8.8.8.8', 80))
         ip = s.getsockname()[0]
         return ip
     except Exception:
         s.close()
         return socket.gethostbyname(socket.gethostname())
 
 
@@ -163,80 +159,69 @@
     Format file size display
 
     :param sz: 整数，表示文件大小
     :param align: 是否对齐
     :return: 文件大小字符串
     """
     if sz >= 1e9:
-        return (
-            "%.3f GB" % (sz / 1024**3) if not align else "%7.3f GB" % (sz / 1024**3)
-        )
+        return '%.3f GB' % (sz / 1e9) if not align else '%7.3f GB' % (sz / 1e9)
     elif sz >= 1e6:
-        return (
-            "%.3f MB" % (sz / 1024**2) if not align else "%7.3f MB" % (sz / 1024**2)
-        )
+        return '%.3f MB' % (sz / 1e6) if not align else '%7.3f MB' % (sz / 1e6)
     elif sz >= 1e3:
-        return "%.3f KB" % (sz / 1024) if not align else "%7.3f KB" % (sz / 1024)
+        return '%.3f KB' % (sz / 1e3) if not align else '%7.3f KB' % (sz / 1e3)
     else:
-        return "%.2f B" % sz if not align else "%7.2f B" % sz
+        return '%.2f B' % sz if not align else '%7.2f B' % sz
 
 
 def get_ip_info() -> dict:
     """
     通过ip-api获取本机ip信息
 
     Get native IP information through IP-API
 
     :return: ip信息的dict，失败返回None
     """
     import json
-
-    res = requests.get("http://ip-api.com/json/", headers=headers)
+    res = requests.get('http://ip-api.com/json/', headers=headers)
     if res.status_code == requests.codes.ok:
         return json.loads(res.text)
     else:
         return {}
 
 
-def get_fileinfo(
-    url: str, proxy: str = "", referer: str = ""
-) -> Tuple[str, str, requests.Response]:
+def get_fileinfo(url: str, proxy: str = '', referer: str = '') -> (str, str, requests.Response):
     """
     获取待下载的文件信息
 
     Gets information about the file to be downloaded
 
     :param url: 文件url
     :param proxy: 代理
     :param referer: 绕反爬
     :return: 真实url，文件名，http头部信息 (headers中键值均为小写)
     """
     import re
     import os
-
-    proxies = {"http": "http://" + proxy, "https": "https://" + proxy} if proxy else {}
+    proxies = {
+        'http': 'http://'+proxy,
+        'https': 'https://'+proxy
+    } if proxy else {}
     if referer:
-        headers["referer"] = referer
+        headers['referer'] = referer
     try:
         res = requests.head(url, headers=headers, proxies=proxies)
-        if res.status_code == 404:
-            return url, "", res  # 某些网站会返回404，但是文件还是可以下载的
     except Exception as e:
-        return "", repr(e), None
+        return '', repr(e), None
     while res.status_code in [301, 302]:
-        url = {i[0]: i[1] for i in res.headers.lower_items()}["location"]
+        url = {i[0]: i[1] for i in res.headers.lower_items()}['location']
         res = requests.head(url, headers=headers, proxies=proxies)
     res.headers = {i[0]: i[1] for i in res.headers.lower_items()}
-    if "content-disposition" in res.headers:
+    if 'content-disposition' in res.headers:
         try:
-            filename = re.findall(
-                "filename=(.*?);", res.headers["content-disposition"]
-            )[0]
+            filename = re.findall('filename=(.*?);', res.headers['content-disposition'])[0]
         except IndexError:
             from urllib.parse import urlparse
-
-            filename = os.path.basename(urlparse(url).path.strip("/"))
+            filename = os.path.basename(urlparse(url).path.strip('/'))
     else:
         from urllib.parse import urlparse
-
-        filename = os.path.basename(urlparse(url).path.strip("/"))
+        filename = os.path.basename(urlparse(url).path.strip('/'))
     return url, re.sub(r"^\W+|\W+$", "", filename), res
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/Compress.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,166 +3,149 @@
 压缩与解压缩各种文件
 
 Compress and decompress all kinds of files
 """
 import io
 import os
 import sys
-
-from .. import (
-    user_lang,
-    qs_default_console,
-    qs_warning_string,
-    requirePackage,
-)
+import tarfile
+import zipfile
+import rarfile
+import py7zr
+from .. import dir_char, user_lang, qs_default_console, qs_warning_string
 
 
 def get_compress_package_name():
     """
     从命令行参数中，解析并返回压缩包名称
 
     From the command line arguments, the package name is parsed and returned.
 
     :return: 压缩包名称，合法的文件列表 | Compressed package name, a list of legitimate files.
     """
     file_names = sys.argv[2:]
     if not file_names:
-        exit("No enough parameters")
+        exit('No enough parameters')
     if len(file_names) > 1:
-        name = "pigeonhole"
+        tar_name = 'pigeonhole'
     else:
-        name = os.path.basename(file_names[0]).split(".")[0]
+        ls = file_names[0].split(dir_char)
+        while not ls[-1]:
+            ls.pop()
+        tar_name = ls[-1].split('.')[0]
     ls = []
     for file_name in file_names:
         if os.path.exists(file_name):
             ls.append(file_name)
         else:
-            qs_default_console.print(
-                qs_warning_string,
-                f"{file_name} not found" if user_lang != "zh" else f"{file_name} 未找到",
-            )
-    return name, ls
+            print("No such file or dictionary:%s" % file_name)
+    return tar_name, ls
 
 
-def checkIsProtocolFile(protocol, verify_func, path):
+def checkIsProtocolFile(protocol, path):
     """
     验证压缩包文件
 
     Verify compressed package file
-
     :param protocol: 压缩协议 | compress protocol
     :param path: 文件路径 | File Path
     :return:
     """
-
-    protocol_name = {
-        "tarfile": "tar",
-        "zipfile": "zip",
-        "rarfile": "rar",
-        "py7zr": "7z",
-    }
-
     if os.path.exists(path):
-        if not requirePackage(protocol, verify_func)(path):
-            raise TypeError(
-                f"{path} "
-                + (
-                    f"Not recognized by {protocol_name[protocol]} protocol"
-                    if user_lang != "zh"
-                    else f"无法被{protocol_name[protocol]}协议识别"
-                )
-            )
+        if protocol == tarfile and not tarfile.is_tarfile(path):
+            raise TypeError(f"{path} " + ('Not recognized by tar protocol' if user_lang != 'zh' else '无法被tar协议识别'))
+        elif protocol == zipfile and not zipfile.is_zipfile(path):
+            raise TypeError(f"{path} " + ('Not recognized by zip protocol' if user_lang != 'zh' else '无法被zip协议识别'))
+        elif protocol == rarfile and not rarfile.is_rarfile(path):
+            raise TypeError(f"{path} " + ('Not recognized by rar protocol' if user_lang != 'zh' else '无法被rar协议识别'))
+        elif protocol == py7zr and not py7zr.is_7zfile(path):
+            raise TypeError(f"{path} " + ('Not recognized by 7z protocol' if user_lang != 'zh' else '无法被7z协议识别'))
     else:
         raise FileNotFoundError
 
 
 class _NormalCompressedPackage:
     """
     通用压缩协议类，如果你不懂它是做什么的，请不要调用它
 
     General compression protocol class, if you do not understand what it does, please do not call it
     """
-
-    def __init__(self, protocol, verify_func, obj_name, path: str, mode="r"):
+    def __init__(self, _protocol, path: str, mode='r'):
         """
         通用压缩协议类初始化
 
         General compression protocol class initialization
 
-        :param protocol: 压缩协议包 | General compression protocol packages
-        :param verify_func: 验证函数 | Verification function
-        :param obj_name: 对象名称 | Object name
+        :param _protocol: 压缩协议包 | General compression protocol packages
         :param path: 压缩包路径 | compression package path
         :param mode: 读写模式 | 'r' or 'w', which 'r' means read and 'w' means write
         """
-        self._protocol = protocol
+        self._protocol = _protocol
         self.path = path
-        if mode not in ("r", "w"):
+        if mode not in ('r', 'w'):
             raise ValueError("Requires mode 'r', 'w'")
-        if mode == "r":
-            checkIsProtocolFile(protocol, verify_func, path)
-            if protocol != "rarfile":
-                self.src = requirePackage(protocol, obj_name)(path, "r")
+        if mode == 'r':
+            checkIsProtocolFile(_protocol, path)
+            if _protocol == zipfile:
+                self.src = zipfile.ZipFile(path, 'r')
+            elif _protocol == rarfile:
+                self.src = rarfile.RarFile(path)
+            elif _protocol == py7zr:
+                self.src = py7zr.SevenZipFile(path, 'r')
             else:
-                self.src = requirePackage(protocol, obj_name)(path)
+                self.src = _protocol.open(path, 'r')
             self.mode = True
-        elif mode == "w":
-            if protocol != "rarfile":
-                self.src = requirePackage(protocol, obj_name)(path, "w")
-            else:
-                raise NotImplementedError(
-                    "qs not support to create rar file because `RarFile`"
-                )
+        elif mode == 'w':
+            if _protocol == tarfile:
+                self.src = _protocol.open(path, 'x:gz')
+            elif _protocol == zipfile:
+                self.src = _protocol.ZipFile(path, 'w')
+            elif _protocol == rarfile:
+                raise NotImplementedError('qs not support to create rar file because `RarFile`')
+            elif _protocol == py7zr:
+                self.src = _protocol.SevenZipFile(path, 'w')
             self.mode = False
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add file to the compressed package (works in 'w' mode)
 
         :param path: 文件路径 | File path
         :return: None
         """
         if self.mode:
             raise io.UnsupportedOperation
-        if not os.path.exists(path):
-            raise FileNotFoundError
-        if os.path.isdir(path):
-            for root, dirs, files in os.walk(path):
-                for file in files:
-                    if self._protocol == "tarfile":
-                        self.src.add(os.path.join(root, file))
-                    elif self._protocol in ["zipfile", "py7zr"]:
-                        self.src.write(os.path.join(root, file))
-        else:
-            if self._protocol == "tarfile":
+        if os.path.exists(path):
+            if self._protocol == tarfile:
                 self.src.add(path)
-            elif self._protocol in ["zipfile", "py7zr"]:
+            elif self._protocol in [zipfile, py7zr]:
                 self.src.write(path)
+        else:
+            raise FileNotFoundError
 
     def extract(self):
         """
         解压缩 | extract
 
         :return: None
         """
         if self.mode:
-            if self._protocol in ["tarfile", "rarfile", "py7zr"]:
+            if self._protocol in [tarfile, rarfile, py7zr]:
                 self.src.extractall()
-            elif self._protocol == "zipfile":
+            elif self._protocol in [zipfile]:
                 from pathlib import Path
-
                 for fn in self.src.namelist():
                     path = Path(self.src.extract(fn))
                     try:
-                        path.rename(fn.encode("cp437").decode("utf-8"))
+                        path.rename(fn.encode('cp437').decode('utf-8'))
                     except:
                         try:
-                            path.rename(fn.encode("cp437").decode("gbk"))
+                            path.rename(fn.encode('cp437').decode('gbk'))
                         except Exception as e:
                             qs_default_console.log(qs_warning_string, repr(e))
 
             else:
                 raise NotImplementedError
             self.save()
         else:
@@ -174,24 +157,24 @@
 
         :return: None
         """
         self.src.close()
 
 
 class Tar(_NormalCompressedPackage):
-    def __init__(self, path, mode="r"):
+    def __init__(self, path, mode='r'):
         """
         Tar协议初始化
 
         Tar protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__("tarfile", "is_tarfile", "TarFile", path, mode)
+        super().__init__(tarfile, path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'write'模式下）
 
         Add files to the compressed package (works in 'write' mode)
 
@@ -212,24 +195,24 @@
 
     def save(self):
         """保存 | save"""
         return super().save()
 
 
 class Zip(_NormalCompressedPackage):
-    def __init__(self, path, mode="r"):
+    def __init__(self, path, mode='r'):
         """
         Zip协议初始化
 
         Zip protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__("zipfile", "is_zipfile", "ZipFile", path, mode)
+        super().__init__(zipfile, path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add files to the compressed package (works in 'write' mode)
 
@@ -250,24 +233,24 @@
 
     def save(self):
         """保存 | save"""
         return super().save()
 
 
 class Rar(_NormalCompressedPackage):
-    def __init__(self, path, mode="r"):
+    def __init__(self, path, mode='r'):
         """
         Rar协议初始化
 
         Rar protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__("rarfile", "is_rarfile", "RarFile", path, mode)
+        super().__init__(rarfile, path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add files to the compressed package (works in 'write' mode)
 
@@ -288,24 +271,24 @@
 
     def save(self):
         """保存 | save"""
         return super().save()
 
 
 class SevenZip(_NormalCompressedPackage):
-    def __init__(self, path, mode="r"):
+    def __init__(self, path, mode='r'):
         """
         7z协议初始化
 
         7z protocol initialization.
 
         :param path: 压缩包路径 | The package path is compressed.
         :param mode: 工作模式 | Working mode ('read' or 'write')
         """
-        super().__init__("py7zr", "is_7zfile", "SevenZipFile", path, mode)
+        super().__init__(py7zr, path, mode)
 
     def add_file(self, path):
         """
         向压缩包添加文件（工作在'w'模式下）
 
         Add files to the compressed package (works in 'write' mode)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/Diff.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-from .. import (
-    qs_default_console,
-    qs_error_string,
-    qs_warning_string,
-    user_lang,
-    dir_char,
-)
+from .. import dir_char, qs_default_console, qs_error_string, qs_warning_string, user_lang
 from ..SystemTools.FileHash import md5
 import os
 import re
 
 
 class DictionaryFiles(set):
     def __init__(self, rt: str, ignorePatterns: list = None):
@@ -17,19 +11,19 @@
         """
         super().__init__()
         if ignorePatterns is None:
             ignorePatterns = []
         if not (os.path.exists(rt) or os.path.isdir(rt)):
             qs_default_console.log(
                 qs_error_string,
-                f'"{rt}" {"Not exist or Not a dictionary!" if user_lang != "zh" else "不存在或不是文件夹"}',
+                f'"{rt}" {"Not exist or Not a dictionary!" if user_lang != "zh" else "不存在或不是文件夹"}'
             )
             self.available = False
             return
-        self.name = os.path.basename(rt)
+        self.name = rt.strip(dir_char).split(dir_char)[-1]
         self.rt = os.path.abspath(rt)
         self.available = True
         self.ignored = set(ignorePatterns) if ignorePatterns else None
         self.__getAllPaths()
 
     def checkIgnore(self, path):
         if self.ignored:
@@ -37,15 +31,15 @@
                 if re.findall(item, path):
                     return True
         return False
 
     def __getAllPaths(self):
         for rt, sonDir, files in os.walk(self.rt):
             for file in files:
-                filePath = os.path.join(rt, file).replace(self.rt, "")
+                filePath = os.path.join(rt, file).replace(self.rt, '')
                 if self.checkIgnore(filePath):
                     continue
                 self.add(filePath)
 
     def getMd5ByFileItem(self, item: str):
         return md5(self.rt + item)
 
@@ -57,43 +51,42 @@
     from concurrent.futures import ThreadPoolExecutor, wait
     from rich.progress import Progress
     from difflib import HtmlDiff
 
     def __init__(self, d1: DictionaryFiles, d2: DictionaryFiles):
         self.d1 = d1
         self.d2 = d2
-        self.rt = os.path.join(os.getcwd(), d1.name + "-vs-" + d2.name + ".qs_diff")
+        self.rt = os.getcwd() + dir_char + d1.name + '-vs-' + d2.name + '.qs_diff'
         self.pool = DiffFilesToStructHtml.ThreadPoolExecutor(max_workers=8)
         self.jobLs = []
         self.progress = DiffFilesToStructHtml.Progress(console=qs_default_console)
-        self.pid = self.progress.add_task("compare" if user_lang != "zh" else "对比")
+        self.pid = self.progress.add_task('compare' if user_lang != 'zh' else '对比')
 
     def _run(self, item: str):
         pathLs = item.strip(dir_char).split(dir_char)[:-1]
         for i in range(len(pathLs)):
-            dirName = os.path.join(self.rt, *pathLs[: i + 1])
+            dirName = self.rt + dir_char + dir_char.join(pathLs[:i+1])
             if not os.path.exists(dirName):
                 os.mkdir(dirName)
-        with open(self.d1.getFilepathByItem(item), "r") as f:
+        with open(self.d1.getFilepathByItem(item), 'r') as f:
             _d1 = f.readlines()
-        with open(self.d2.getFilepathByItem(item), "r") as f:
+        with open(self.d2.getFilepathByItem(item), 'r') as f:
             _d2 = f.readlines()
         _diff = DiffFilesToStructHtml.HtmlDiff().make_file(_d1, _d2)
-        with open(self.rt + item + ".html", "w") as f:
+        with open(self.rt + item + '.html', 'w') as f:
             f.write(_diff)
         self.progress.advance(self.pid, 1)
 
     def generate(self):
         if os.path.exists(self.rt):
             qs_default_console.log(
                 qs_warning_string,
-                f'"{self.rt}" {"Already exists! QS will delete it and regenerate." if user_lang != "zh" else "已经存在! QS将删除它并重新生成."}',
+                f'"{self.rt}" {"Already exists! QS will delete it and regenerate." if user_lang != "zh" else "已经存在! QS将删除它并重新生成."}'
             )
             from .. import remove
-
             remove(self.rt)
 
         os.mkdir(self.rt)
         _tmpLs = []
         for item in list(self.d1 & self.d2):
             if self.d1.getMd5ByFileItem(item) != self.d2.getMd5ByFileItem(item):
                 _tmpLs.append(item)
@@ -103,42 +96,31 @@
 
         for item in _tmpLs:
             self.jobLs.append(self.pool.submit(self._run, item))
 
         DiffFilesToStructHtml.wait(self.jobLs)
         self.progress.stop()
 
-        with open(os.path.join(self.rt, "README.md"), "w") as f:
-            print("# Diff Results | 目录对比结果", file=f, end="\n\n")
+        with open(self.rt + dir_char + 'README.md', 'w') as f:
+            print("# Diff Results | 目录对比结果", file=f, end='\n\n')
 
             print(
                 "## Several documents with differences as shown in the table below"
-                if user_lang != "zh"
-                else "## 存在若干有差异的文件如下表",
+                if user_lang != 'zh' else '## 存在若干有差异的文件如下表',
                 file=f,
-                end="\n\n",
+                end='\n\n'
             )
 
-            print(
-                f'|{"Path" if user_lang != "zh" else "路径"}|{"Results Link" if user_lang != "zh" else "结果链接"}|\n|---|:---:|',
-                file=f,
-            )
+            print(f'|{"Path" if user_lang != "zh" else "路径"}|{"Results Link" if user_lang != "zh" else "结果链接"}|\n|---|:---:|', file=f)
             for item in sorted(_tmpLs):
-                print(
-                    f'|{item}|[{"result" if user_lang != "zh" else "结果"}](file://{self.rt + item + ".html"})|',
-                    file=f,
-                )
+                print(f'|{item}|[{"result" if user_lang != "zh" else "结果"}](file://{self.rt + item + ".html"})|', file=f)
 
             print(
                 "## There are several non-shared documents as shown in the table below"
-                if user_lang != "zh"
-                else "## 存在若干非共有文件如下表",
+                if user_lang != 'zh' else '## 存在若干非共有文件如下表',
                 file=f,
-                end="\n\n",
+                end='\n\n'
             )
 
-            print(f"|{self.d1.name}|{self.d2.name}|\n|---|---|", file=f)
+            print(f'|{self.d1.name}|{self.d2.name}|\n|---|---|', file=f)
             for item in sorted(list(self.d1 ^ self.d2)):
-                print(
-                    f'|{item if item in self.d1 else " "}|{item if item in self.d2 else " "}|',
-                    file=f,
-                )
+                print(f'|{item if item in self.d1 else " "}|{item if item in self.d2 else " "}|', file=f)
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/SystemTools/FileHash.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,47 +12,44 @@
 def hashWrapper(algorithm):
     """
     计算文件哈希值(通用)
 
     :param algorithm: 算法名 [md5, sha1, sha256, sha512]
     :return:
     """
-
     def Wrapper(func):
         def wrapper(filePath: str) -> str:
             global cal
             if not os.path.exists(filePath):
-                return "No such file: " + filePath
+                return 'No such file: ' + filePath
             if not os.path.isfile(filePath):
-                return "Not a file: " + filePath
+                return 'Not a file: ' + filePath
             cal = func()
-            with open(filePath, "rb") as f:
+            with open(filePath, 'rb') as f:
                 while True:
                     data = f.read(BlockSize)
                     if not data:
                         break
                     cal.update(data)
             return cal.hexdigest()
-
         return wrapper
-
     return Wrapper
 
 
-@hashWrapper("md5")
+@hashWrapper('md5')
 def md5():
     return hashlib.md5()
 
 
-@hashWrapper("sha1")
+@hashWrapper('sha1')
 def sha1():
     return hashlib.sha1()
 
 
-@hashWrapper("sha256")
+@hashWrapper('sha256')
 def sha256():
     return hashlib.sha256()
 
 
-@hashWrapper("sha512")
+@hashWrapper('sha512')
 def sha512():
     return hashlib.sha512()
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/ThreadTools/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         (Multiple file pointer acceleration)
 
         :param filename: 文件名
         :param workers: 线程数
         :param mode: 读写模式，如'wb', 'rb+'
         """
         self.workers = workers
-        self.handles = [open(filename, mode) for _ in range(workers)]
-        self.handles_lock = [threading.Lock() for _ in range(workers)]
+        self.handles = [open(filename, mode) for i in range(workers)]
+        self.handles_lock = [threading.Lock() for i in range(workers)]
         self.pool = ThreadPoolExecutor(max_workers=workers)
         self.job_q = []
         self.cur_handle = 0
 
     def wait(self):
         """
         等待完全完成任务
@@ -88,45 +88,20 @@
 
         Write a new file block
 
         :param content: 文件内容
         :param index: 起始位置
         :return:
         """
-        self.job_q.append(
-            self.pool.submit(self._write, self.cur_handle, content, index)
-        )
-        self.cur_handle = (self.cur_handle + 1) % self.workers
+        self.job_q.append(self.pool.submit(self._write, self.cur_handle, content, index))
+        self.cur_handle = (self.cur_handle+1) % self.workers
 
     def __del__(self):
         """
         删除对象，必须等待线程池工作结束
 
         To delete an object, you must wait for the thread pool to finish working
 
         :return:
         """
         self.wait()
         self.pool.shutdown()
-
-
-class MemWriter:
-    def __init__(self):
-        """
-        线程安全的写内存。
-        """
-        from io import BytesIO
-
-        self.q = BytesIO()
-
-    def new_job(self, content: bytes, index: int):
-        # 将内容写入内存
-        self.q.seek(index)
-        self.q.write(content)
-
-    @property
-    def content(self):
-        # 获取内存内容
-        return self.q.getvalue()
-
-    def wait(self):
-        pass
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/TuiTools/Line.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/TuiTools/Line.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 曲线图
 
 Line Graph
 """
 import io
 from .. import requirePackage
 
-diagram = requirePackage("diagram")
+diagram = requirePackage('diagram')
 
 
 class Line:
     def __init__(self, values: list, height: int, width: int):
         """
         折线图
 
@@ -31,18 +31,20 @@
 
         Draw and return a string
 
         :return: 折线图的字符串
         """
         opt = diagram.DOption()
         opt.size = diagram.Point([self.height, self.width])
-        opt.mode = "g"
+        opt.mode = 'g'
         stream = io.BytesIO()
         gram = diagram.DGWrapper(
-            data=[self.values, range(len(self.values))], dg_option=opt, ostream=stream
+            data=[self.values, range(len(self.values))],
+            dg_option=opt,
+            ostream=stream
         )
         gram.show()
         return str(stream.getvalue(), encoding="utf-8")
 
     def push(self, x: float):
         """
         尾部添加值
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/Wrapper/__init__.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 # coding=utf-8
 """
 qs用到的函数装饰器, 在使用它们前, 请确保你理解注释描述的内容
 
 Before using function decorators used by QS, please make sure that you understand the content described by the annotation.
 """
-from QuickProject.__config__ import set_timeout
+
+
+def set_timeout(num: int):
+    """
+    定时函数装饰器
+
+    Timing function decorator
+
+    :param num: 时间（秒）
+    :return: wrapper
+    """
+    def wrapper(func):
+        def handle(signum, frame):
+            raise RuntimeError
+
+        def run(*args, **kwargs):
+            import signal
+            try:
+                signal.signal(signal.SIGALRM, handle)
+                signal.alarm(num)
+                res = func(*args, **kwargs)
+                signal.alarm(0)
+                return res
+            except RuntimeError:
+                return False
+        return run
+    return wrapper
 
 
 def mkCompressPackageWrap(func):
     """
     创建压缩文件的通用函数装饰器, 被装饰的函数将被传递压缩文件名, 你需要返回:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     的子类对象, 并将读写状态设为 写 状态
@@ -17,25 +43,34 @@
     name, which you need to return:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     's sub object, and set read-write mode as write
 
     :param func: func(filePath: str = '') -> QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     :return: 装饰器 | wrapper
     """
-
     def wrapper():
+        import os
+        from .. import dir_char
         from ..SystemTools.Compress import get_compress_package_name
-
         packages_name, ls = get_compress_package_name()
         packages = func(packages_name)
 
+        def dfs(cur_p):
+            if os.path.isfile(cur_p):
+                packages.add_file(cur_p)
+                return
+            file_ls = os.listdir(cur_p)
+            flag_ch = '' if cur_p.endswith(dir_char) else dir_char
+            for fp in file_ls:
+                fp = cur_p + flag_ch + fp
+                dfs(fp)
+
         for i in ls:
-            packages.add_file(i)
+            dfs(i)
         packages.save()
-
     return wrapper
 
 
 def unCompressPackageWrap(func):
     """
     解压缩文件的通用函数装饰器, 被装饰的函数将被传递压缩文件名, 你需要返回:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
@@ -45,71 +80,61 @@
     name, which you need to return:
         QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     's sub object, and set read-write mode as read
 
     :param func: func(filePath: str = '') -> QuickStart_Rhy.SystemTools.Compress._NormalCompressedPackage
     :return: 装饰器 | wrapper
     """
-
     def wrapper():
         import os
         import sys
 
         file_names = sys.argv[2:]
         if not file_names:
             exit("No enough parameters")
         from .. import qs_default_console, qs_error_string
         from ..NetTools.NormalDL import core_num
         from ..ThreadTools import ThreadPoolExecutor, wait
-
         pool = ThreadPoolExecutor(max_workers=max(core_num // 2, 4))
         job_q = []
 
         def run(path):
             if os.path.exists(path):
                 try:
                     cur_tar = func(path)
                     cur_tar.extract()
                 except Exception as e:
                     qs_default_console.log(qs_error_string, repr(e))
             else:
-                qs_default_console.log(
-                    qs_error_string, "No such file or dictionary: %s" % path
-                )
+                qs_default_console.log(qs_error_string, "No such file or dictionary: %s" % path)
 
         for file_name in file_names:
             job_q.append(pool.submit(run, file_name))
         wait(job_q)
-
     return wrapper
 
 
-def HashWrapper():
+def HashWrapper(algorithm: str):
     """
     文件哈希值计算(通用函数)
+
+    :param algorithm: 算法名称 [md5, sha1, sha256, sha512]
     :return:
     """
-
     def Wrapper(func):
-        algorithm = func.__name__
-
         def _wrapper():
             import sys, os
-            from .. import qs_default_console, qs_info_string, requirePackage
+            from .. import qs_default_console, qs_info_string, user_lang
 
             ls = sys.argv[2:]
             if not ls:
-                qs_default_console.print(
-                    qs_info_string, "Usage: qs %s file1 file2 ..." % algorithm
-                )
+                qs_default_console.print(qs_info_string, 'Usage: qs %s file1 file2 ...' % algorithm)
                 return
 
-            func = requirePackage(".SystemTools.FileHash", algorithm)
+            exec('from QuickStart_Rhy.SystemTools.FileHash import %s' % algorithm)
             for file in ls:
                 qs_default_console.print(
-                    f"\[[bold magenta]{algorithm}[/]]",
-                    f"[underline]{os.path.basename(file)}[/]: '{func(file)}'",
+                    qs_info_string, 'Calculate:' if user_lang != 'zh' else '计算:', os.path.basename(file)
                 )
-
+                exec(f'qs_default_console.print(qs_info_string, "{algorithm}" + ":", {algorithm}("{file}"))')
         return _wrapper
-
     return Wrapper
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/imageDeal.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/imageDeal.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,196 +11,162 @@
 
 def set_img_background():
     """替换图片颜色 | Replace color in image"""
     from .ImageTools.ColorTools import transport_back, get_color_from_str
 
     try:
         img = sys.argv[2]
-        if img == "-help":
+        if img == '-help':
             raise IndexError
         if not os.path.exists(img):
-            qs_default_console.log(qs_error_string, "No Such File: %s" % img)
+            qs_default_console.log(qs_error_string, 'No Such File: %s' % img)
             return
         to = sys.argv[3]
         try:
             frm = sys.argv[4]
         except IndexError:
-            frm = "0,0,0,0"
+            frm = '0,0,0,0'
     except IndexError:
-        qs_default_console.log(
-            qs_error_string,
-            "Usage: qs stbg <picture> <to_color> [from_color: default transparency]",
-        )
+        qs_default_console.log(qs_error_string, 'Usage: qs stbg <picture> <to_color> [from_color: default transparency]')
         return
     else:
         to = get_color_from_str(to)
         frm = get_color_from_str(frm)
         img = transport_back(img, to, frm)
-        iname = sys.argv[2].split(".")
-        iname = iname[0] + "_stbg." + "".join(iname[1:])
+        iname = sys.argv[2].split('.')
+        iname = iname[0] + '_stbg.' + ''.join(iname[1:])
         img.save(iname)
 
 
 def fmt_img_color():
     from .ImageTools.ColorTools import formatOneColor, get_color_from_str
 
     try:
         img = sys.argv[2]
-        if img == "-help":
+        if img == '-help':
             raise IndexError
         if not os.path.exists(img):
-            qs_default_console.log(qs_error_string, "No Such File: %s" % img)
+            qs_default_console.log(qs_error_string, 'No Such File: %s' % img)
             return
         to = sys.argv[3]
         try:
             exp = sys.argv[4:]
         except IndexError:
-            exp = "0,0,0,0"
+            exp = '0,0,0,0'
     except IndexError:
-        qs_default_console.log(
-            qs_error_string,
-            "Usage: qs fmti <picture> <to_color> [except_color: default transparency]",
-        )
+        qs_default_console.log(qs_error_string,
+                               'Usage: qs fmti <picture> <to_color> [except_color: default transparency]')
         return
     else:
         to = get_color_from_str(to)
         exp = [get_color_from_str(i) for i in exp]
         img = formatOneColor(img, to, exp)
-        iname = sys.argv[2].split(".")
-        iname = iname[0] + "_fmt." + "".join(iname[1:])
+        iname = sys.argv[2].split('.')
+        iname = iname[0] + '_fmt.' + ''.join(iname[1:])
         img.save(iname)
 
 
 def v2gif():
     """视频转gif | video to gif"""
     from .ImageTools.VideoTools import video_2_gif
 
     try:
         video = sys.argv[2]
         sz, fps = None, None
         if len(sys.argv) > 3:
             for i in sys.argv[3:]:
                 try:
-                    if "," in i:
-                        sz = tuple([int(j) for j in i.split(",")])
+                    if ',' in i:
+                        sz = tuple([int(j) for j in i.split(',')])
                     else:
                         fps = int(i)
                 except:
                     raise IndexError
-        sz = (
-            tuple([int(i) for i in sys.argv[3].split(",")])
-            if len(sys.argv) > 3 and "," in sys.argv[3]
-            else None
-        )
-    except IndexError:
-        qs_default_console.log(
-            qs_error_string, "Usage: qs v2gif <*.mp4> [width,height] [fps]"
-        )
+        sz = tuple([int(i) for i in sys.argv[3].split(',')]) if len(sys.argv) > 3 and ',' in sys.argv[3] else None
+    except IndexError:
+        qs_default_console.log(qs_error_string, 'Usage: qs v2gif <*.mp4> [width,height] [fps]')
         return
     else:
-        video_2_gif(video, sz, fps) if sz and fps else video_2_gif(
-            video, sz
-        ) if sz else video_2_gif(video, fps=fps) if fps else video_2_gif(video)
+        video_2_gif(video, sz, fps) if sz and fps else video_2_gif(video, sz) \
+            if sz else video_2_gif(video, fps=fps) if fps else video_2_gif(video)
 
 
 def remove_audio():
     """删除视频的音频 | remove audio in mp4"""
     from .ImageTools.VideoTools import rm_audio
-
     try:
         videos = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, "Usage: qs rmaudio <video...>")
+        qs_default_console.log(qs_error_string, 'Usage: qs rmaudio <video...>')
     else:
         for video in videos:
             rm_audio(video)
 
 
 def v2mp4():
     """视频转mp4 | transfer video to mp4"""
     from .ImageTools.VideoTools import tomp4
-
     try:
         videos = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, "Usage: qs v2mp4 <video...>")
+        qs_default_console.log(qs_error_string, 'Usage: qs v2mp4 <video...>')
     else:
         for video in videos:
             tomp4(video)
 
 
 def v2mp3():
     """提取视频音频为mp3 | Extract the audio from the video and save it in MP3 format"""
     from .ImageTools.VideoTools import video_2_mp3
-
     try:
         videos = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, "Usage: qs v2mp3 <video...>")
+        qs_default_console.log(qs_error_string, 'Usage: qs v2mp3 <video...>')
     else:
         for video in videos:
             video_2_mp3(video)
 
 
 def icat():
     """Mac::iTerm下预览图片 | Preview the picture under Mac::iTerm"""
     try:
         path = sys.argv[2]
-        is_url = "-u" in sys.argv or (
-            not os.path.exists(path)
-            and (path.startswith("http://") or path.startswith("https://"))
-        )
-        is_in_rc_file = "--rc" in sys.argv
-        if is_in_rc_file:
-            rc_width = int(sys.argv[sys.argv.index("--rc") + 1])
-        else:
-            rc_width = 0
+        is_url = '-open_url' in sys.argv or \
+                 (not os.path.exists(path) and (path.startswith('http://') or path.startswith('https://')))
         if not os.path.exists(path) and not is_url:
-            qs_default_console.log(qs_error_string, "No such file:", path)
+            qs_default_console.log(qs_error_string, 'No such file:', path)
             raise FileNotFoundError
     except:
-        qs_default_console.log(
-            qs_error_string, "Usage: qs icat <img path/url> [-u if is url]"
-        )
+        qs_default_console.log(qs_error_string, 'Usage: qs icat <img path/url> [-open_url if is url]')
     else:
         from .ImageTools.ImagePreview import image_preview
-
-        image_preview(
-            path, set_width_in_rc_file=rc_width, force_show=True
-        ) if not is_url else image_preview(
-            path, is_url, set_width_in_rc_file=rc_width, force_show=True
-        )
+        image_preview(open(path)) if not is_url else image_preview(path, is_url)
 
 
 def i2png():
     try:
         imgs = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, "Usage: qs i2png <imgs...>")
+        qs_default_console.log(qs_error_string, 'Usage: qs i2png <imgs...>')
     else:
         from .ImageTools.ImageTools import topng
-
         for imgPath in imgs:
             topng(imgPath)
 
 
 def i2jpg():
     try:
         imgs = sys.argv[2:]
     except IndexError:
-        qs_default_console.log(qs_error_string, "Usage: qs i2jpg <imgs...>")
+        qs_default_console.log(qs_error_string, 'Usage: qs i2jpg <imgs...>')
     else:
         from .ImageTools.ImageTools import tojpg
-
         for imgPath in imgs:
             tojpg(imgPath)
 
 
 def vsta():
     from .ImageTools.VideoTools import set_video_audio
-
     try:
         set_video_audio(*sys.argv[2:])
     except Exception as e:
-        qs_default_console.log(
-            qs_error_string, f"{repr(e)}\nUsage: qs vsta <video> <audio>"
-        )
+        qs_default_console.log(qs_error_string, f'{repr(e)}\nUsage: qs vsta <video> <audio>')
```

### Comparing `quickstart_rhy-0.6.80/QuickStart_Rhy/system.py` & `QuickStart_Rhy-0.6.9/QuickStart_Rhy/system.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,309 +2,255 @@
 """
 调用各种系统工具
 
 Call various system tools
 """
 import QuickStart_Rhy.Wrapper as _wrapper
 
-miss_file = [".DS_Store"]
+miss_file = ['.DS_Store']
 
 
 def __latest_filename(name):
     import os
+    from . import dir_char
 
     cur = os.getcwd()
-    while cur != os.path.dirname(cur):
-        if os.path.exists(os.path.join(cur, name)):
-            return os.path.join(cur, name)
-        cur = os.path.dirname(cur)
-    return os.path.join(cur, name) if os.path.exists(os.path.join(cur, name)) else ""
+    rec = cur
+    while cur != dir_char:
+        if os.path.exists(name):
+            os.chdir(rec)
+            return cur + dir_char + name
+        os.chdir('..')
+        cur = os.getcwd()
+    os.chdir(rec)
+    return ''
 
 
 def top():
     """
     CPU和内存监测
 
     CPU and memory monitoring
 
     :return: None
     """
-    import sys
-
-    sys.argv = ["bpytop"] + sys.argv[2:]
-
-    from . import requirePackage
+    from . import dir_char
+    if dir_char == '\\':
+        from .SystemTools.Monitor import top
+        top()
+    else:
+        import sys
+        sys.argv = ['bpytop'] + sys.argv[2:]
 
-    requirePackage("bpytop", "main")()
+        from . import requirePackage
+        requirePackage('bpytop', 'main')()
 
 
 def clear_mem():
     """
     清理系统内存
 
     Clean system memory
 
     :return: None
     """
     from .SystemTools import clear_mem
-
     clear_mem()
 
 
 def go_github():
     """
     自动识别当前文件夹.git/config中的地址，并通过浏览器打开
 
     Automatically recognize the address in the current folder .git/config and open it through a browser
     """
     import os
-    from . import (
-        qs_default_console,
-        qs_error_string,
-        user_lang,
-        open_url,
-        requirePackage,
-    )
+    from . import qs_default_console, qs_error_string, user_lang, open_url, requirePackage
 
-    config_path = __latest_filename(".git/config")
+    config_path = __latest_filename('.git/config')
     if not os.path.exists(config_path):
-        qs_default_console.print(
-            qs_error_string,
-            "No a git dictionary" if user_lang != "zh" else "不是 git 文件夹",
-        )
+        qs_default_console.print(qs_error_string, 'No a git dictionary' if user_lang != 'zh' else '不是 git 文件夹')
         return
-    config = requirePackage("configparser", "ConfigParser")()
+    config = requirePackage('configparser', 'ConfigParser')()
     config.read(filenames=config_path)
     url_ls = []
     for section in config.sections():
-        if section.startswith("remote"):
-            url_ls.append(config[section]["url"].replace(".git", ""))
+        if section.startswith('remote'):
+            url_ls.append(config[section]['url'].replace('.git', ''))
     open_url(url_ls)
 
 
+@_wrapper.mkCompressPackageWrap
+def _mktar(file_path: str = ''):
+    from .SystemTools.Compress import Tar
+    return Tar(file_path + '.tar.gz', 'w')
+
+
 def mktar():
     """
     创建tar包
 
     Create a tar packages
 
     :return: None
     """
+    return _mktar()
 
-    @_wrapper.mkCompressPackageWrap
-    def _mktar(file_path: str = ""):
-        from .SystemTools.Compress import Tar
 
-        return Tar(file_path + ".tar.gz", "w")
-
-    return _mktar()
+@_wrapper.unCompressPackageWrap
+def _untar(file_path: str = ''):
+    from .SystemTools.Compress import Tar
+    return Tar(file_path)
 
 
 def untar():
     """
     解压tar包
 
     Unpack the tar packages
 
     :return: None
     """
+    return _untar()
 
-    @_wrapper.unCompressPackageWrap
-    def _untar(file_path: str = ""):
-        from .SystemTools.Compress import Tar
-
-        return Tar(file_path)
 
-    return _untar()
+@_wrapper.mkCompressPackageWrap
+def _mkzip(file_path: str = ''):
+    from .SystemTools.Compress import Zip
+    return Zip(file_path + '.zip', 'w')
 
 
 def mkzip():
     """
     创建ZIP包
 
     Create a ZIP package
 
     :return: None
     """
+    return _mkzip()
 
-    @_wrapper.mkCompressPackageWrap
-    def _mkzip(file_path: str = ""):
-        from .SystemTools.Compress import Zip
-
-        return Zip(file_path + ".zip", "w")
 
-    return _mkzip()
+@_wrapper.unCompressPackageWrap
+def _unzip(file_path: str = ''):
+    from .SystemTools.Compress import Zip
+    return Zip(file_path, 'r')
 
 
 def unzip():
     """
     解压ZIP包
 
     Unpack the ZIP package
 
     :return: None
     """
+    return _unzip()
 
-    @_wrapper.unCompressPackageWrap
-    def _unzip(file_path: str = ""):
-        from .SystemTools.Compress import Zip
-
-        return Zip(file_path, "r")
 
-    return _unzip()
+@_wrapper.unCompressPackageWrap
+def _unrar(file_path: str = ''):
+    from .SystemTools.Compress import Rar
+    return Rar(file_path)
 
 
 def unrar():
     """
     解压RAR包
 
     Extract RAR package
 
     :return: None
     """
+    return _unrar()
 
-    @_wrapper.unCompressPackageWrap
-    def _unrar(file_path: str = ""):
-        from .SystemTools.Compress import Rar
 
-        return Rar(file_path)
-
-    return _unrar()
+@_wrapper.mkCompressPackageWrap
+def _mk7z(file_path: str = ''):
+    from .SystemTools.Compress import SevenZip
+    return SevenZip(file_path + '.7z', 'w')
 
 
 def mk7z():
     """
     创建7z包
 
     Create 7z package
 
     :return: None
     """
+    return _mk7z()
 
-    @_wrapper.mkCompressPackageWrap
-    def _mk7z(file_path: str = ""):
-        from .SystemTools.Compress import SevenZip
 
-        return SevenZip(file_path + ".7z", "w")
-
-    return _mk7z()
+@_wrapper.unCompressPackageWrap
+def _un7z(file_path: str = ''):
+    from .SystemTools.Compress import SevenZip
+    return SevenZip(file_path)
 
 
 def un7z():
     """
     解压7z包
 
     Extract 7z package
 
     :return:
     """
-
-    @_wrapper.unCompressPackageWrap
-    def _un7z(file_path: str = ""):
-        from .SystemTools.Compress import SevenZip
-
-        return SevenZip(file_path)
-
     return _un7z()
 
 
-@_wrapper.HashWrapper()
+@_wrapper.HashWrapper('md5')
 def md5():
     """
     获取文件md5值
     :return:
     """
 
 
-@_wrapper.HashWrapper()
+@_wrapper.HashWrapper('sha1')
 def sha1():
     """
     获取文件sha1值
     :return:
     """
 
 
-@_wrapper.HashWrapper()
+@_wrapper.HashWrapper('sha256')
 def sha256():
     """
     获取文件sha256值
     :return:
     """
 
 
-@_wrapper.HashWrapper()
+@_wrapper.HashWrapper('sha512')
 def sha512():
     """
     获取文件sha512值
     :return:
     """
 
 
 def diff_dir():
     """
     对比两个文件夹差异，并生成相应html对比结果
     :return:
     """
-    from . import user_lang, qs_default_console, qs_info_string, qs_default_status
+    from . import user_lang, qs_default_console, qs_info_string
     from .SystemTools.Diff import DictionaryFiles
     import sys
 
-    if "-h" in sys.argv:
-        qs_default_console.print(
-            qs_info_string, "Usage: qs diff <dir1> <dir2> [-x <name or regex pattern>]"
-        )
+    if '-h' in sys.argv:
+        qs_default_console.print(qs_info_string, 'Usage: qs diff <dir1> <dir2> [-x <name or regex pattern>]')
 
     d1, d2 = sys.argv[2:4]
-    apply_ignore = sys.argv[sys.argv.index("-x") + 1 :] if "-x" in sys.argv else None
+    apply_ignore = sys.argv[sys.argv.index('-x') + 1:] if '-x' in sys.argv else None
     d1 = DictionaryFiles(d1, apply_ignore)
     d2 = DictionaryFiles(d2, apply_ignore)
 
     if not (d1.available and d2.available):
         return
 
-    with qs_default_status(
-        "Generating diff result.." if user_lang != "zh" else "生成对比结果中.."
-    ):
+    with qs_default_console.status('Generating diff result..' if user_lang != 'zh' else '生成对比结果中..'):
         from .SystemTools.Diff import DiffFilesToStructHtml
 
         DiffFilesToStructHtml(d1, d2).generate()
-
-
-def mount_dmg():
-    """
-    挂载镜像 
-
-    :return:
-    """
-    from .SystemTools.DiskMac import DMG
-    import sys
-
-    DMG().mount(sys.argv[2])
-
-
-def unmount_dmg():
-    """
-    卸载镜像
-    """
-    from .SystemTools.DiskMac import DMG
-    from .TuiTools.Table import qs_default_table
-    from . import qs_default_console, user_lang, qs_info_string, _ask
-
-    disks = DMG()
-    _ls = disks.get_disk_list()[2:]
-    if not _ls:
-        return qs_default_console.print(
-            qs_info_string, "No DMG disk found" if user_lang != "zh" else "没有找到 dmg 磁盘"
-        )
-    table = qs_default_table(["Disk", "Type", "Size"])
-    for disk in _ls:
-        table.add_row(disk["path"], disk["type"], disk["size"])
-    qs_default_console.print(table, justify="center")
-    disk_paths = _ask(
-        {
-            "type": "checkbox",
-            "message": "Select a disk to umount" if user_lang != "zh" else "选择要卸载的磁盘",
-            "choices": [{'name': disk["path"], 'checked': True} for disk in _ls],
-        }
-    )
-    for disk_path in disk_paths:
-        disks.unmount(disk_path)
```

