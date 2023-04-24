# Comparing `tmp/yumikogram-0.0.6.tar.gz` & `tmp/yumikogram-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yumikogram-0.0.6.tar", last modified: Fri Mar 31 12:54:36 2023, max compression
+gzip compressed data, was "yumikogram-0.0.7.tar", last modified: Mon Apr 24 12:43:34 2023, max compression
```

## Comparing `yumikogram-0.0.6.tar` & `yumikogram-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:54:36.221440 yumikogram-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 12:54:21.000000 yumikogram-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-31 12:54:36.217440 yumikogram-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-31 12:54:21.000000 yumikogram-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 12:54:36.221440 yumikogram-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-31 12:54:21.000000 yumikogram-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:54:36.217440 yumikogram-0.0.6/yumikogram/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-31 12:54:21.000000 yumikogram-0.0.6/yumikogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-03-31 12:54:21.000000 yumikogram-0.0.6/yumikogram/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:54:36.217440 yumikogram-0.0.6/yumikogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:54:21.000000 yumikogram-0.0.6/yumikogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:54:36.217440 yumikogram-0.0.6/yumikogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-31 12:54:36.000000 yumikogram-0.0.6/yumikogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-31 12:54:36.000000 yumikogram-0.0.6/yumikogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:54:36.000000 yumikogram-0.0.6/yumikogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-31 12:54:36.000000 yumikogram-0.0.6/yumikogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 12:54:36.000000 yumikogram-0.0.6/yumikogram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:43:34.838072 yumikogram-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:43:24.000000 yumikogram-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 12:43:34.838072 yumikogram-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 12:43:24.000000 yumikogram-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:43:34.838072 yumikogram-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-24 12:43:24.000000 yumikogram-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:43:34.838072 yumikogram-0.0.7/yumikogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 12:43:24.000000 yumikogram-0.0.7/yumikogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-24 12:43:24.000000 yumikogram-0.0.7/yumikogram/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:43:34.838072 yumikogram-0.0.7/yumikogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:43:24.000000 yumikogram-0.0.7/yumikogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:43:34.838072 yumikogram-0.0.7/yumikogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 12:43:34.000000 yumikogram-0.0.7/yumikogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 12:43:34.000000 yumikogram-0.0.7/yumikogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:43:34.000000 yumikogram-0.0.7/yumikogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:43:34.000000 yumikogram-0.0.7/yumikogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 12:43:34.000000 yumikogram-0.0.7/yumikogram.egg-info/top_level.txt
```

### Comparing `yumikogram-0.0.6/LICENSE` & `yumikogram-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yumikogram-0.0.6/PKG-INFO` & `yumikogram-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yumikogram
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package for telegram bots making and api making
 Home-page: https://github.com/yumiko-api/yumikogram
 Author: santhosh
 Author-email: yumikoapi@gmail.com
 Keywords: yumikogram,telegram,telegram-bots,yumikogram api,telegram bots library
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yumikogram-0.0.6/setup.py` & `yumikogram-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `yumikogram-0.0.6/yumikogram/clients.py` & `yumikogram-0.0.7/yumikogram/clients.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,51 +79,48 @@
         data.update(kwargs)
         response = await self._send_request(url, data)
         updates = response.get('result', [])
         for update in updates:
             self.last_update_id = update['update_id']
         return updates
 
+ 
     async def _send_request(self, url: str, data: Dict) -> Dict:
         """
         Sends a request to the Telegram Bot API.
 
         Args:
             url (str): The URL of the Telegram Bot API endpoint.
             data (Dict): The data to send to the Telegram Bot API.
 
         Returns:
             Dict: The response from the Telegram Bot API as a dictionary.
         """
         encoded_data = json.dumps(data).encode('utf-8')
         headers = {
-            'Content-Type': 'application/json
+            'Content-Type': 'application/json'
         }
-    try:
-        async with asyncio.open_connection(self.server, self.port, ssl=self.ssl_context) as conn:
-            request = (f'POST {url} HTTP/1.1\r\n'
-                       f'Host: {self.server}\r\n'
-                       f'Content-Length: {len(encoded_data)}\r\n'
-                       f'Connection: close\r\n\r\n').encode('utf-8') + encoded_data
-            conn.write(request)
-            response = await conn.read()
-    except (socket.gaierror, socket.error) as e:
-        logging.error(f'Error connecting to Telegram API: {e}')
-        return {}
-    try:
-        response = response.decode('utf-8')
-        headers, body = response.split('\r\n\r\n', 1)
-        status_code = int(headers.split()[1])
-        if status_code != 200:
-            logging.error(f'Request failed with status code {status_code}: {body}')
+        try:
+            async with asyncio.open_connection(self.server, self.port, ssl=self.ssl_context) as conn:
+                request = (f'POST {url} HTTP/1.1\r\n'
+                           f'Host: {self.server}\r\n'
+                           f'Content-Length: {len(encoded_data)}\r\n'
+                           f'Connection: close\r\n'
+                           f'{headers}\r\n').encode('utf-8') + encoded_data
+                conn.write(request)
+                response = await conn.read()
+        except (socket.gaierror, socket.error) as e:
+            logging.error(f'Error connecting to Telegram API: {e}')
+            return {}
+        try:
+            response = response.decode('utf-8')
+            response = json.loads(response)
+            return response
+        except ValueError:
             return {}
-        return json.loads(body)
-    except Exception as e:
-        logging.error(f'Error parsing response from Telegram API: {e}')
-        return {}
 
 async def get_dialogs(self) -> List[Dict]:
     """
     Gets the list of dialogs for the authorized user.
     Returns:
         List[Dict]: A list of dialogs as dictionaries.
     """
```

### Comparing `yumikogram-0.0.6/yumikogram.egg-info/PKG-INFO` & `yumikogram-0.0.7/yumikogram.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yumikogram
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package for telegram bots making and api making
 Home-page: https://github.com/yumiko-api/yumikogram
 Author: santhosh
 Author-email: yumikoapi@gmail.com
 Keywords: yumikogram,telegram,telegram-bots,yumikogram api,telegram bots library
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

