# Comparing `tmp/pyiotown-0.4.3.dev7-py3-none-any.whl.zip` & `tmp/pyiotown-0.4.3.dev8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6660 bytes, number of entries: 10
+Zip file size: 6741 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-05 08:55 pyiotown/__init__.py
 -rw-r--r--  2.0 unx     3416 b- defN 23-Apr-18 05:32 pyiotown/get.py
--rw-r--r--  2.0 unx     3794 b- defN 23-Apr-18 05:32 pyiotown/post.py
--rw-r--r--  2.0 unx     6865 b- defN 23-Apr-22 06:39 pyiotown/post_process.py
--rw-r--r--  2.0 unx     1053 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/LICENSE
--rw-r--r--  2.0 unx      693 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/pbr.json
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      807 b- defN 23-Apr-22 06:41 pyiotown-0.4.3.dev7.dist-info/RECORD
-10 files, 16776 bytes uncompressed, 5274 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     4133 b- defN 23-Apr-22 07:21 pyiotown/post.py
+-rw-r--r--  2.0 unx     6951 b- defN 23-Apr-22 07:19 pyiotown/post_process.py
+-rw-r--r--  2.0 unx     1053 b- defN 23-Apr-22 07:22 pyiotown-0.4.3.dev8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      693 b- defN 23-Apr-22 07:22 pyiotown-0.4.3.dev8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 07:22 pyiotown-0.4.3.dev8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-22 07:22 pyiotown-0.4.3.dev8.dist-info/pbr.json
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-22 07:22 pyiotown-0.4.3.dev8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      807 b- defN 23-Apr-22 07:22 pyiotown-0.4.3.dev8.dist-info/RECORD
+10 files, 17201 bytes uncompressed, 5355 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pyiotown/post.py
 Comment: 
 
 Filename: pyiotown/post_process.py
 Comment: 
 
-Filename: pyiotown-0.4.3.dev7.dist-info/LICENSE
+Filename: pyiotown-0.4.3.dev8.dist-info/LICENSE
 Comment: 
 
-Filename: pyiotown-0.4.3.dev7.dist-info/METADATA
+Filename: pyiotown-0.4.3.dev8.dist-info/METADATA
 Comment: 
 
-Filename: pyiotown-0.4.3.dev7.dist-info/WHEEL
+Filename: pyiotown-0.4.3.dev8.dist-info/WHEEL
 Comment: 
 
-Filename: pyiotown-0.4.3.dev7.dist-info/pbr.json
+Filename: pyiotown-0.4.3.dev8.dist-info/pbr.json
 Comment: 
 
-Filename: pyiotown-0.4.3.dev7.dist-info/top_level.txt
+Filename: pyiotown-0.4.3.dev8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyiotown-0.4.3.dev7.dist-info/RECORD
+Filename: pyiotown-0.4.3.dev8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyiotown/post.py

```diff
@@ -1,76 +1,84 @@
 import sys
 import requests
 import json
 import ssl
 
-def uploadImage(url, token, payload, verify=True, timeout=60):
+def uploadImage(url, token, payload, group_id=None, verify=True, timeout=60):
     '''
     url : IoT.own Server Address
     token : IoT.own API Token
     payload : Image + Annotation Json Data (check format in README.md)
     '''
     apiaddr = url + "/api/v1.0/nn/image"
     header = {'Content-Type': 'application/json', 'Token': token}
+    if group_id is not None:
+        header['grpid'] = group_id
     try:
         r = requests.post(apiaddr, data=payload, headers=header, verify=verify, timeout=timeout)
         if r.status_code == 200:
             return True
         else:
             print(r.content)
             return False
     except Exception as e:
         print(e)
         return False
-def data(url, token, nid, data, upload="", verify=True, timeout=60):
+def data(url, token, nid, data, upload="", group_id=None, verify=True, timeout=60):
     '''
     url : IoT.own Server Address
     token : IoT.own API Token
     type: Message Type
     nid: Node ID
     data: data to send (JSON object)
     '''
     typenum = "2" # 2 static 
     apiaddr = url + "/api/v1.0/data"
     if upload == "":
-        header = {'Accept':'application/json', 'token':token } 
+        header = {'Accept':'application/json', 'token':token }
+        if group_id is not None:
+            header['grpid'] = group_id
         payload = { "type" : typenum, "nid" : nid, "data": data }
         try:
             r = requests.post(apiaddr, json=payload, headers=header, verify=verify, timeout=timeout)
             if r.status_code == 200:
                 return True
             else:
                 print(r.content)
                 return False
         except Exception as e:
             print(e)
             return False
     else:
-        header = {'Accept':'application/json', 'token':token } 
+        header = {'Accept':'application/json', 'token':token }
+        if group_id is not None:
+            header['grpid'] = group_id
         payload = { "type" : typenum, "nid" : nid, "meta": json.dumps(data) }
         try:
             r = requests.post(apiaddr, data=payload, headers=header, verify=verify, timeout=timeout, files=upload)
             if r.status_code == 200:
                 return True
             else:
                 print(r.content)
                 return False
         except Exception as e:
             print(e)
             return False
 
-def post_files(result, url, token, verify=True, timeout=60):
+def post_files(result, url, token, group_id=None, verify=True, timeout=60):
     if 'data' not in result.keys():
         return result
     
     for key in result['data'].keys():
         if type(result['data'][key]) is dict:
             resultkey = result['data'][key].keys()
             if ('raw' in resultkey) and ( 'file_type' in resultkey) :
                 header = {'Accept':'application/json', 'token':token }
+                if group_id is not None:
+                    header['grpid'] = group_id
                 upload = { key + "file": result['data'][key]['raw'] }
                 try:
                     r = requests.post( url + "/api/v1.0/file", headers=header, verify=verify, timeout=timeout, files=upload )
                     if r.status_code == 200:
                         del result['data'][key]['raw']
                         result['data'][key]['file_id'] = r.json()["files"][0]["file_id"]
                         result['data'][key]['file_ext'] = r.json()["files"][0]["file_ext"]
```

## pyiotown/post_process.py

```diff
@@ -40,15 +40,16 @@
             client.publish('iotown/proc-done', json.dumps(message), 1)
         return
 
     if userdata['dry'] == True:
         result = None
     
     if type(result) is dict and 'data' in result.keys():
-        result = post_files(result, userdata['url'], userdata['token'], userdata['verify'])
+        group_id = data['grpid'] if userdata['group'] == 'common' else None
+        result = post_files(result, userdata['url'], userdata['token'], group_id, userdata['verify'])
         message['data'] = result['data']
         client.publish('iotown/proc-done', json.dumps(message), 1)
     elif result is None:
         print(f"Discard the message")
     else:
         print(f"CALLBACK FUNCTION TYPE ERROR {type(result)} must [ dict ]", file=sys.stderr)
         client.publish('iotown/proc-done', msg.payload, 1)
```

## Comparing `pyiotown-0.4.3.dev7.dist-info/LICENSE` & `pyiotown-0.4.3.dev8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyiotown-0.4.3.dev7.dist-info/METADATA` & `pyiotown-0.4.3.dev8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiotown
-Version: 0.4.3.dev7
+Version: 0.4.3.dev8
 Summary: IoT.own Library
 Home-page: https://github.com/CoXlabInc/pyiotow
 Author: CoXlab Inc.
 Author-email: support@coxlab.kr
 Maintainer: Jongsoo Jeong
 Maintainer-email: jsjeong@coxlab.k
 License: MIT
```

## Comparing `pyiotown-0.4.3.dev7.dist-info/RECORD` & `pyiotown-0.4.3.dev8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyiotown/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyiotown/get.py,sha256=025Eg17ZnS2VttWiaNgc-6lz1eaKRFsj5kz6hJxMh3U,3416
-pyiotown/post.py,sha256=qdeb2G74anHc8ceymjSSQ7ZnNpO1iQMFghbWYjbj2ms,3794
-pyiotown/post_process.py,sha256=p4_XO0NDPd0Q3csHIbsXh4_XO3splFI8gMy33li6n9U,6865
-pyiotown-0.4.3.dev7.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
-pyiotown-0.4.3.dev7.dist-info/METADATA,sha256=x77a64d3itDnT3PzvbK6GwBWbKw4I8kLC18SUrRgv74,693
-pyiotown-0.4.3.dev7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyiotown-0.4.3.dev7.dist-info/pbr.json,sha256=kc6ciLY88_Yu39zFSPymNBFrUwpb9p90BPvr6VtpTyo,47
-pyiotown-0.4.3.dev7.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
-pyiotown-0.4.3.dev7.dist-info/RECORD,,
+pyiotown/post.py,sha256=usPMeZf_v3rzFTwo4EKJSxg0Z6FneCROITuyeNRnifM,4133
+pyiotown/post_process.py,sha256=bA2Z3LLu2ee9thhORVvx1whUiWeMqKOYcNRdTD43LvY,6951
+pyiotown-0.4.3.dev8.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
+pyiotown-0.4.3.dev8.dist-info/METADATA,sha256=uzsXVSLgeQgA7eil7PFPwcNVpSGmudJKeSyLrqGQ7cs,693
+pyiotown-0.4.3.dev8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyiotown-0.4.3.dev8.dist-info/pbr.json,sha256=cqbZm2EU5qg6CAAOi_OVVF0geM1iTbn8_Z7MNJ8Z-b8,47
+pyiotown-0.4.3.dev8.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
+pyiotown-0.4.3.dev8.dist-info/RECORD,,
```

