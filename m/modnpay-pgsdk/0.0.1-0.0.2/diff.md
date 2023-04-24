# Comparing `tmp/modnpay-pgsdk-0.0.1.tar.gz` & `tmp/modnpay-pgsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modnpay-pgsdk-0.0.1.tar", last modified: Fri Apr 21 10:00:36 2023, max compression
+gzip compressed data, was "modnpay-pgsdk-0.0.2.tar", last modified: Mon Apr 24 01:01:12 2023, max compression
```

## Comparing `modnpay-pgsdk-0.0.1.tar` & `modnpay-pgsdk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:00:36.249406 modnpay-pgsdk-0.0.1/
--rw-rw-rw-   0        0        0      425 2023-04-21 10:00:36.249406 modnpay-pgsdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-18 06:07:37.000000 modnpay-pgsdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 10:00:36.247413 modnpay-pgsdk-0.0.1/modnpay_pgsdk.egg-info/
--rw-rw-rw-   0        0        0      425 2023-04-21 10:00:36.000000 modnpay-pgsdk-0.0.1/modnpay_pgsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-04-21 10:00:36.000000 modnpay-pgsdk-0.0.1/modnpay_pgsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:00:36.000000 modnpay-pgsdk-0.0.1/modnpay_pgsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 10:00:36.000000 modnpay-pgsdk-0.0.1/modnpay_pgsdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 10:00:36.249406 modnpay-pgsdk-0.0.1/mpsdk/
--rw-rw-rw-   0        0        0     2088 2023-04-21 09:18:20.000000 modnpay-pgsdk-0.0.1/mpsdk/MPSDK.py
--rw-rw-rw-   0        0        0       62 2023-04-21 09:48:11.000000 modnpay-pgsdk-0.0.1/mpsdk/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-21 09:48:06.000000 modnpay-pgsdk-0.0.1/mpsdk/__version__.py
--rw-rw-rw-   0        0        0      104 2023-04-21 09:22:24.000000 modnpay-pgsdk-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-04-21 10:00:36.250402 modnpay-pgsdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-04-21 10:00:30.000000 modnpay-pgsdk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:01:12.247956 modnpay-pgsdk-0.0.2/
+-rw-rw-rw-   0        0        0      425 2023-04-24 01:01:12.247956 modnpay-pgsdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:07:37.000000 modnpay-pgsdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:01:12.245963 modnpay-pgsdk-0.0.2/modnpay_pgsdk.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-04-24 01:01:12.000000 modnpay-pgsdk-0.0.2/modnpay_pgsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-24 01:01:12.000000 modnpay-pgsdk-0.0.2/modnpay_pgsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:01:12.000000 modnpay-pgsdk-0.0.2/modnpay_pgsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 01:01:12.000000 modnpay-pgsdk-0.0.2/modnpay_pgsdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 01:01:12.247956 modnpay-pgsdk-0.0.2/mpsdk/
+-rw-rw-rw-   0        0        0     2211 2023-04-24 00:59:06.000000 modnpay-pgsdk-0.0.2/mpsdk/MPSDK.py
+-rw-rw-rw-   0        0        0       62 2023-04-21 09:48:11.000000 modnpay-pgsdk-0.0.2/mpsdk/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-21 09:48:06.000000 modnpay-pgsdk-0.0.2/mpsdk/__version__.py
+-rw-rw-rw-   0        0        0      104 2023-04-21 09:22:24.000000 modnpay-pgsdk-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-24 01:01:12.248953 modnpay-pgsdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-04-24 01:01:07.000000 modnpay-pgsdk-0.0.2/setup.py
```

### Comparing `modnpay-pgsdk-0.0.1/mpsdk/MPSDK.py` & `modnpay-pgsdk-0.0.2/mpsdk/MPSDK.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,58 +7,64 @@
 import rsa
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 
 
 class MPSDK:
 
-    def __init__(self, request, public_key):
-        self.public_key = public_key
-        self.requestParams = request.get_json()
+    def __init__(self, is_prod):
         self.byte_xid = os.urandom(16)
         self.xid = binascii.hexlify(self.byte_xid)
         self.iv = self.xid[0:16]
+        if is_prod:
+            self.url = "https://pg.modnpay.kr/api/v1/payments/order"
+        else:
+            self.url = "https://dpg.modnpay.kr/api/v1/payments/order"
+
+    def order(self, request, public_key):
+        public_key = public_key
+        requestParams = request.get_json()
 
-    def order(self):
-        e = self.encrypt(json.dumps(self.requestParams))
-        k = base64.b64encode(rsa.encrypt(self.xid, self.public_key)).decode('utf-8')
+        e = self.encrypt(json.dumps(requestParams))
+        k = base64.b64encode(rsa.encrypt(self.xid, public_key)).decode('utf-8')
 
         datas = {
-            "mid": self.requestParams['merchantId'],
+            "mid": requestParams['merchantId'],
             'e': e,
             'k': k
         }
 
-        url = "https://dpg.modnpay.kr/api/v1/payments/order"
         headers = {'Content-Type': 'application/json; charset=utf-8'}
 
-        response = requests.post(url, json=datas, headers=headers)
+        response = requests.post(self.url, json=datas, headers=headers)
 
         return response.json()
 
-    def refund(self):
+    def refund(self, request, public_key):
+        public_key = public_key
+        requestParams = request.get_json()
+
         refundParam = {
-            'merchantId': self.requestParams['merchantId'],
-            'traceNum': self.requestParams['tid'],
-            'refundAmount': self.requestParams['refundAmount']
+            'merchantId': requestParams['merchantId'],
+            'traceNum': requestParams['tid'],
+            'refundAmount': requestParams['refundAmount']
         }
 
         e = self.encrypt(json.dumps(refundParam))
-        k = base64.b64encode(rsa.encrypt(self.xid, self.public_key)).decode('utf-8')
+        k = base64.b64encode(rsa.encrypt(self.xid, public_key)).decode('utf-8')
 
         datas = {
-            "mid": self.requestParams['merchantId'],
+            "mid": requestParams['merchantId'],
             'e': e,
             'k': k
         }
 
-        url = "https://dpg.modnpay.kr/api/v1/payments/refund"
         headers = {'Content-Type': 'application/json; charset=utf-8'}
 
-        response = requests.post(url, json=datas, headers=headers)
+        response = requests.post(self.url, json=datas, headers=headers)
 
         return response.json()
 
     def encrypt(self, raw):
         cipher = AES.new(self.xid, AES.MODE_CBC, self.iv)
         return bytes.decode(base64.b64encode(cipher.encrypt(pad(raw.encode(), AES.block_size))))
```

### Comparing `modnpay-pgsdk-0.0.1/setup.py` & `modnpay-pgsdk-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="modnpay-pgsdk",
-    version="0.0.1",
+    version="0.0.2",
     author="seeroo",
     author_email="developers@seeroo.co.kr",
     description="modnpay-pgsdk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.seeroo.info/juyeol.jang/modnpay-pgsdk-python",
     classifiers=[
```

