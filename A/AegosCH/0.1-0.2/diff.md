# Comparing `tmp/AegosCH-0.1.tar.gz` & `tmp/AegosCH-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AegosCH-0.1.tar", last modified: Mon Apr 24 00:14:27 2023, max compression
+gzip compressed data, was "AegosCH-0.2.tar", last modified: Mon Apr 24 01:06:37 2023, max compression
```

## Comparing `AegosCH-0.1.tar` & `AegosCH-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 00:14:27.638616 AegosCH-0.1/
-drwxrwxrwx   0        0        0        0 2023-04-24 00:14:27.566974 AegosCH-0.1/AegosCH/
--rw-rw-rw-   0        0        0       55 2023-04-24 00:12:01.000000 AegosCH-0.1/AegosCH/__init__.py
--rw-rw-rw-   0        0        0     3421 2023-04-24 00:09:27.000000 AegosCH-0.1/AegosCH/ch_ti.py
-drwxrwxrwx   0        0        0        0 2023-04-24 00:14:27.634626 AegosCH-0.1/AegosCH.egg-info/
--rw-rw-rw-   0        0        0      348 2023-04-24 00:14:27.000000 AegosCH-0.1/AegosCH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-04-24 00:14:27.000000 AegosCH-0.1/AegosCH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 00:14:27.000000 AegosCH-0.1/AegosCH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 00:14:27.000000 AegosCH-0.1/AegosCH.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-24 00:14:27.000000 AegosCH-0.1/AegosCH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      348 2023-04-24 00:14:27.637619 AegosCH-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 00:14:27.639613 AegosCH-0.1/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-04-24 00:13:56.000000 AegosCH-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:06:37.446601 AegosCH-0.2/
+drwxrwxrwx   0        0        0        0 2023-04-24 01:06:37.396733 AegosCH-0.2/AegosCH/
+-rw-rw-rw-   0        0        0       55 2023-04-24 00:12:01.000000 AegosCH-0.2/AegosCH/__init__.py
+-rw-rw-rw-   0        0        0     3408 2023-04-24 01:04:39.000000 AegosCH-0.2/AegosCH/ch_ti.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:06:37.436627 AegosCH-0.2/AegosCH.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-04-24 01:06:37.000000 AegosCH-0.2/AegosCH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-24 01:06:37.000000 AegosCH-0.2/AegosCH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:06:37.000000 AegosCH-0.2/AegosCH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 01:06:37.000000 AegosCH-0.2/AegosCH.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-04-24 01:06:37.000000 AegosCH-0.2/AegosCH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      348 2023-04-24 01:06:37.444606 AegosCH-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:06:37.447598 AegosCH-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-04-24 01:06:13.000000 AegosCH-0.2/setup.py
```

### Comparing `AegosCH-0.1/AegosCH/ch_ti.py` & `AegosCH-0.2/AegosCH/ch_ti.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
             'accept-Encoding':'gzip',
             'user-agent':'com.zhiliaoapp.musically/2018101933 (Linux; U; Android 11; ar_IQ; SM-A022F; Build/RP1A.200720.012; Cronet/58.0.2991.0)',
             'connection': 'close'        
     }
     data = f"app_language=ar&manifest_version_code=2018101933&_rticket=1656747775754&iid=7115676682581247750&channel=googleplay&language=ar&fp=&device_type=SM-A022F&resolution=720*1471&openudid=8c05dec470c7b7d5&update_version_code=2018101933&sys_region=IQ&os_api=30&is_my_cn=0&timezone_name=Asia%2FBaghdad&dpi=280&email={email}&retry_type=no_retry&carrier_region=IQ&ac=wifi&device_id=7023349253125604869&mcc_mnc=41805&timezone_offset=10800&os_version=11&version_code=880&carrier_region_v2=418&app_name=musical_ly&ab_version=8.8.0&version_name=8.8.0&device_brand=samsung&ssmix=a&pass-region=1&build_number=8.8.0&device_platform=android&region=SA&aid=1233"
     res = requests.post(url,headers=headers,data=data).text
     if 'Sent successfully' in res:
-        return {'status':'Available','BY':'@G_4_2'}
+        return {'status':'OK','BY':'@G_4_2'}
     else :
-        return {'status':'Unavailable','BY':'@G_4_2'}
+        return {'status':'FALSE','BY':'@G_4_2'}
 def Instagram(email):
     url2 = 'https://i.instagram.com/api/v1/accounts/login/'
     headers2 = {
         'User-Agent':str(hd),
         'Accept':'*/*',
         'Cookie':'missing',
         'Accept-Encoding':'gzip, deflate',
```

