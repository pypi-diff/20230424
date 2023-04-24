# Comparing `tmp/mailparse-1.0.6.tar.gz` & `tmp/mailparse-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailparse-1.0.6.tar", last modified: Thu Apr  6 09:52:24 2023, max compression
+gzip compressed data, was "mailparse-1.0.7.tar", last modified: Mon Apr 24 10:00:14 2023, max compression
```

## Comparing `mailparse-1.0.6.tar` & `mailparse-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cx42      (1000) cx42      (1000)        0 2023-04-06 09:52:24.085016 mailparse-1.0.6/
--rw-r--r--   0 cx42      (1000) cx42      (1000)     1090 2022-10-13 08:35:16.000000 mailparse-1.0.6/LICENSE
--rw-r--r--   0 cx42      (1000) cx42      (1000)    17911 2023-04-06 09:52:24.085016 mailparse-1.0.6/PKG-INFO
--rw-r--r--   0 cx42      (1000) cx42      (1000)    16362 2022-10-13 10:18:33.000000 mailparse-1.0.6/README.md
-drwxr-xr-x   0 cx42      (1000) cx42      (1000)        0 2023-04-06 09:52:24.084016 mailparse-1.0.6/mailparse/
--rwxr-xr-x   0 cx42      (1000) cx42      (1000)      198 2022-10-25 12:35:32.000000 mailparse-1.0.6/mailparse/__init__.py
--rw-r--r--   0 cx42      (1000) cx42      (1000)       21 2023-04-06 09:51:43.000000 mailparse-1.0.6/mailparse/__version__.py
--rwxr-xr-x   0 cx42      (1000) cx42      (1000)    11239 2023-03-16 11:14:04.000000 mailparse-1.0.6/mailparse/decoder.py
--rwxr-xr-x   0 cx42      (1000) cx42      (1000)     8392 2023-04-06 09:51:36.000000 mailparse-1.0.6/mailparse/encoder.py
--rw-r--r--   0 cx42      (1000) cx42      (1000)      786 2022-10-24 14:23:49.000000 mailparse-1.0.6/mailparse/utils.py
-drwxr-xr-x   0 cx42      (1000) cx42      (1000)        0 2023-04-06 09:52:24.085016 mailparse-1.0.6/mailparse.egg-info/
--rw-r--r--   0 cx42      (1000) cx42      (1000)    17911 2023-04-06 09:52:24.000000 mailparse-1.0.6/mailparse.egg-info/PKG-INFO
--rw-r--r--   0 cx42      (1000) cx42      (1000)      276 2023-04-06 09:52:24.000000 mailparse-1.0.6/mailparse.egg-info/SOURCES.txt
--rw-r--r--   0 cx42      (1000) cx42      (1000)        1 2023-04-06 09:52:24.000000 mailparse-1.0.6/mailparse.egg-info/dependency_links.txt
--rw-r--r--   0 cx42      (1000) cx42      (1000)       10 2023-04-06 09:52:24.000000 mailparse-1.0.6/mailparse.egg-info/top_level.txt
--rw-r--r--   0 cx42      (1000) cx42      (1000)      102 2023-04-06 09:52:24.086016 mailparse-1.0.6/setup.cfg
--rw-rw-r--   0 cx42      (1000) cx42      (1000)     2820 2022-10-24 14:26:02.000000 mailparse-1.0.6/setup.py
+drwxr-xr-x   0 cx42      (1000) cx42      (1000)        0 2023-04-24 10:00:14.641093 mailparse-1.0.7/
+-rw-r--r--   0 cx42      (1000) cx42      (1000)     1090 2022-10-13 08:35:16.000000 mailparse-1.0.7/LICENSE
+-rw-r--r--   0 cx42      (1000) cx42      (1000)    17911 2023-04-24 10:00:14.641093 mailparse-1.0.7/PKG-INFO
+-rw-r--r--   0 cx42      (1000) cx42      (1000)    16362 2022-10-13 10:18:33.000000 mailparse-1.0.7/README.md
+drwxr-xr-x   0 cx42      (1000) cx42      (1000)        0 2023-04-24 10:00:14.640093 mailparse-1.0.7/mailparse/
+-rwxr-xr-x   0 cx42      (1000) cx42      (1000)      198 2022-10-25 12:35:32.000000 mailparse-1.0.7/mailparse/__init__.py
+-rw-r--r--   0 cx42      (1000) cx42      (1000)       21 2023-04-24 09:59:16.000000 mailparse-1.0.7/mailparse/__version__.py
+-rwxr-xr-x   0 cx42      (1000) cx42      (1000)    11578 2023-04-24 09:58:34.000000 mailparse-1.0.7/mailparse/decoder.py
+-rwxr-xr-x   0 cx42      (1000) cx42      (1000)     8392 2023-04-06 09:51:36.000000 mailparse-1.0.7/mailparse/encoder.py
+-rw-r--r--   0 cx42      (1000) cx42      (1000)      786 2022-10-24 14:23:49.000000 mailparse-1.0.7/mailparse/utils.py
+drwxr-xr-x   0 cx42      (1000) cx42      (1000)        0 2023-04-24 10:00:14.641093 mailparse-1.0.7/mailparse.egg-info/
+-rw-r--r--   0 cx42      (1000) cx42      (1000)    17911 2023-04-24 10:00:14.000000 mailparse-1.0.7/mailparse.egg-info/PKG-INFO
+-rw-r--r--   0 cx42      (1000) cx42      (1000)      276 2023-04-24 10:00:14.000000 mailparse-1.0.7/mailparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cx42      (1000) cx42      (1000)        1 2023-04-24 10:00:14.000000 mailparse-1.0.7/mailparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cx42      (1000) cx42      (1000)       10 2023-04-24 10:00:14.000000 mailparse-1.0.7/mailparse.egg-info/top_level.txt
+-rw-r--r--   0 cx42      (1000) cx42      (1000)      102 2023-04-24 10:00:14.641093 mailparse-1.0.7/setup.cfg
+-rw-rw-r--   0 cx42      (1000) cx42      (1000)     2820 2022-10-24 14:26:02.000000 mailparse-1.0.7/setup.py
```

### Comparing `mailparse-1.0.6/LICENSE` & `mailparse-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mailparse-1.0.6/PKG-INFO` & `mailparse-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailparse
-Version: 1.0.6
+Version: 1.0.7
 Summary: Encode raw emails into Python dict objects and build raw emails from Python dict.
 Home-page: https://github.com/cnicodeme/mailparse
 Author: Cyril Nicodeme
 Author-email: contact@cnicodeme.com
 License: MIT
 Project-URL: Source, https://github.com/cnicodeme/mailparse
 Keywords: mail email parse parser encode decode encoder decoder eml
```

### Comparing `mailparse-1.0.6/README.md` & `mailparse-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mailparse-1.0.6/mailparse/decoder.py` & `mailparse-1.0.7/mailparse/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,19 @@
                     'type': payload.get_content_type(),
                     'name': self._decode_str(payload.get_filename(), charset)
                 }
 
                 if payload.get('content-description') is not None:
                     attachment['description'] = self._decode_str(str(payload.get('content-description')), charset)
 
+                if payload.get('Content-Transfer-Encoding') is not None:
+                    encoding = str(payload.get('Content-Transfer-Encoding')).lower()
+                    if encoding in ('base64', 'quoted-printable', '7bit', '8bit', 'binary') or encoding.startswith('x-'):
+                        attachment['encoding'] = encoding
+
                 if str(payload.get('Content-Transfer-Encoding')) == 'base64':
                     attachment['content'] = self._merge_multiple_payload(payload, charset, decode=False)
                 elif payload.get_content_maintype().lower() in ('text', 'message'):
                     content = self._merge_multiple_payload(payload, charset)
                     attachment['content'] = self._decode_str(content, charset)
                 else:
                     attachment['content'] = base64.b64encode(self._decode_str(payload.get_payload(decode=True), charset).encode('utf-8')).decode('utf-8')
```

### Comparing `mailparse-1.0.6/mailparse/encoder.py` & `mailparse-1.0.7/mailparse/encoder.py`

 * *Files identical despite different names*

### Comparing `mailparse-1.0.6/mailparse/utils.py` & `mailparse-1.0.7/mailparse/utils.py`

 * *Files identical despite different names*

### Comparing `mailparse-1.0.6/mailparse.egg-info/PKG-INFO` & `mailparse-1.0.7/mailparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailparse
-Version: 1.0.6
+Version: 1.0.7
 Summary: Encode raw emails into Python dict objects and build raw emails from Python dict.
 Home-page: https://github.com/cnicodeme/mailparse
 Author: Cyril Nicodeme
 Author-email: contact@cnicodeme.com
 License: MIT
 Project-URL: Source, https://github.com/cnicodeme/mailparse
 Keywords: mail email parse parser encode decode encoder decoder eml
```

### Comparing `mailparse-1.0.6/setup.py` & `mailparse-1.0.7/setup.py`

 * *Files identical despite different names*

