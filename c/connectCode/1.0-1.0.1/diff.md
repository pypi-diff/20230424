# Comparing `tmp/connectCode-1.0.tar.gz` & `tmp/connectCode-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectCode-1.0.tar", last modified: Sun Apr 23 07:18:33 2023, max compression
+gzip compressed data, was "dist\connectCode-1.0.1.tar", last modified: Mon Apr 24 02:19:12 2023, max compression
```

## Comparing `connectCode-1.0.tar` & `connectCode-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:18:33.794483 connectCode-1.0/
--rw-rw-rw-   0        0        0    34520 2023-04-23 07:06:12.000000 connectCode-1.0/LICENSE
--rw-rw-rw-   0        0        0       96 2023-04-23 07:18:33.793483 connectCode-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 07:18:33.790483 connectCode-1.0/connectCode/
--rw-rw-rw-   0        0        0       49 2023-04-23 07:11:22.000000 connectCode-1.0/connectCode/__init__.py
--rw-rw-rw-   0        0        0     1776 2023-04-19 08:15:55.000000 connectCode-1.0/connectCode/connectCode.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:18:33.793483 connectCode-1.0/connectCode.egg-info/
--rw-rw-rw-   0        0        0       96 2023-04-23 07:18:33.000000 connectCode-1.0/connectCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-23 07:18:33.000000 connectCode-1.0/connectCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:18:33.000000 connectCode-1.0/connectCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-23 07:18:33.000000 connectCode-1.0/connectCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:18:33.794483 connectCode-1.0/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-04-23 07:17:40.000000 connectCode-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:19:12.000000 connectCode-1.0.1/
+-rw-rw-rw-   0        0        0    34520 2023-04-23 07:06:12.000000 connectCode-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-04-24 02:19:12.000000 connectCode-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2023-04-24 01:33:02.000000 connectCode-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 02:19:12.000000 connectCode-1.0.1/connectCode/
+-rw-rw-rw-   0        0        0       49 2023-04-23 07:11:22.000000 connectCode-1.0.1/connectCode/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-04-24 01:23:40.000000 connectCode-1.0.1/connectCode/connectCode.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:19:12.000000 connectCode-1.0.1/connectCode.egg-info/
+-rw-rw-rw-   0        0        0      186 2023-04-24 02:19:12.000000 connectCode-1.0.1/connectCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-24 02:19:12.000000 connectCode-1.0.1/connectCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 02:19:12.000000 connectCode-1.0.1/connectCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 02:19:12.000000 connectCode-1.0.1/connectCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 02:19:12.000000 connectCode-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-04-24 02:16:53.000000 connectCode-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `connectCode-1.0/LICENSE` & `connectCode-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectCode-1.0/connectCode/connectCode.py` & `connectCode-1.0.1/connectCode/connectCode.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 
 import requests
 from fake_useragent import UserAgent
 import os
 import hashlib
 
 def getExtermalCode():
-    location = os.getcwd() + '\\fake_useragent.json'
+    # location = os.getcwd() + '\\fake_useragent.json'
+    location = os.sep.join([os.getcwd(), r'fake_useragent.json'])
     print(location)
-    ua = UserAgent()
-    # url = 'http://139.9.218.64/Software.txt'
-    # url = r'http://222.186.141.155:8866/Software.txt'
-    url = r'https://meta-3.cn/Software.txt'
+    # ua = UserAgent(cache_path='fake_useragent.json')
+    # url = r'https://meta-3.cn/Software.txt'
+    url = r'http://222.186.141.155:8866/Software.txt'
     headers = {
-        "user-agent": ua.chrome
+        "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2840.99 Safari/537.36"
     }
+
+
+    print(headers)
     response = requests.get(url=url, headers=headers)
     resStr = response.text
     #print(resStr)
-    #print('编码格式：{}'.format(response.apparent_encoding))
+
     return resStr
 
 def fileExists(filePath):
     flag = False
 
     if os.path.exists(filePath):
         #print('文件存在')
@@ -51,25 +54,27 @@
     #print(res)
     return res
 
 
 if __name__ == '__main__':
     resStr = getExtermalCode()
 
-    pathStr = os.path.dirname(os.path.abspath(__file__))
+    pathStr = os.path.dirname(os.path.dirname(__file__))
     filePath = 'CONNECT-KEY.txt'
     filePath = pathStr + '\\' + filePath
+    # filePath = os.sep.join([pathStr, filePath])
     print(filePath)
     flag = fileExists(filePath)
 
     if flag:
         strLocal = getFileValue(filePath)
     else:
         print('文件不存在')
 
+
     strSha256 = getSha256(resStr)
 
     flag2 = False
     if strLocal == strSha256:
         print('通过')
         flag2 = True
     else:
```

