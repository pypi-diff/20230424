# Comparing `tmp/yumikogram-0.0.8.tar.gz` & `tmp/yumikogram-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yumikogram-0.0.8.tar", last modified: Mon Apr 24 12:59:06 2023, max compression
+gzip compressed data, was "yumikogram-0.0.9.tar", last modified: Mon Apr 24 13:14:53 2023, max compression
```

## Comparing `yumikogram-0.0.8.tar` & `yumikogram-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:06.905041 yumikogram-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:58:53.000000 yumikogram-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 12:59:06.905041 yumikogram-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 12:58:53.000000 yumikogram-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:59:06.905041 yumikogram-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-24 12:58:53.000000 yumikogram-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:06.901041 yumikogram-0.0.8/yumikogram/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 12:58:53.000000 yumikogram-0.0.8/yumikogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-24 12:58:53.000000 yumikogram-0.0.8/yumikogram/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:06.905041 yumikogram-0.0.8/yumikogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:58:53.000000 yumikogram-0.0.8/yumikogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:06.905041 yumikogram-0.0.8/yumikogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 12:59:06.000000 yumikogram-0.0.8/yumikogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 12:59:06.000000 yumikogram-0.0.8/yumikogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:59:06.000000 yumikogram-0.0.8/yumikogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:59:06.000000 yumikogram-0.0.8/yumikogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 12:59:06.000000 yumikogram-0.0.8/yumikogram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:53.232189 yumikogram-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:14:41.000000 yumikogram-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 13:14:53.232189 yumikogram-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 13:14:41.000000 yumikogram-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:14:53.232189 yumikogram-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-24 13:14:41.000000 yumikogram-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:53.232189 yumikogram-0.0.9/yumikogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 13:14:41.000000 yumikogram-0.0.9/yumikogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-24 13:14:41.000000 yumikogram-0.0.9/yumikogram/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:53.232189 yumikogram-0.0.9/yumikogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:14:41.000000 yumikogram-0.0.9/yumikogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:53.232189 yumikogram-0.0.9/yumikogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 13:14:53.000000 yumikogram-0.0.9/yumikogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 13:14:53.000000 yumikogram-0.0.9/yumikogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:14:53.000000 yumikogram-0.0.9/yumikogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 13:14:53.000000 yumikogram-0.0.9/yumikogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 13:14:53.000000 yumikogram-0.0.9/yumikogram.egg-info/top_level.txt
```

### Comparing `yumikogram-0.0.8/LICENSE` & `yumikogram-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yumikogram-0.0.8/PKG-INFO` & `yumikogram-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yumikogram
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package for telegram bots making and api making
 Home-page: https://github.com/yumiko-api/yumikogram
 Author: santhosh
 Author-email: yumikoapi@gmail.com
 Keywords: yumikogram,telegram,telegram-bots,yumikogram api,telegram bots library
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `yumikogram-0.0.8/setup.py` & `yumikogram-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `yumikogram-0.0.8/yumikogram/clients.py` & `yumikogram-0.0.9/yumikogram/clients.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,46 +81,45 @@
         updates = response.get('result', [])
         for update in updates:
             self.last_update_id = update['update_id']
         return updates
 
  
     async def _send_request(self, url: str, data: Dict) -> Dict:
-        """
-        Sends a request to the Telegram Bot API.
-
-        Args:
-            url (str): The URL of the Telegram Bot API endpoint.
-            data (Dict): The data to send to the Telegram Bot API.
-
-        Returns:
-            Dict: The response from the Telegram Bot API as a dictionary.
-        """
-        encoded_data = json.dumps(data).encode('utf-8')
-        headers = {
-            'Content-Type': 'application/json'
-        }
-        try:
-            async with asyncio.open_connection(self.server, self.port, ssl=self.ssl_context) as conn:
-                request = (f'POST {url} HTTP/1.1\r\n'
-                           f'Host: {self.server}\r\n'
-                           f'Content-Length: {len(encoded_data)}\r\n'
-                           f'Connection: close\r\n'
-                           f'{headers}\r\n').encode('utf-8') + encoded_data
-                conn.write(request)
-                response = await conn.read()
-        except (socket.gaierror, socket.error) as e:
-            logging.error(f'Error connecting to Telegram API: {e}')
-            return {}
-        try:
-            response = response.decode('utf-8')
-            response = json.loads(response)
-            return response
-        except ValueError:
-            return {}
+    """
+    Sends a request to the Telegram Bot API.
+    Args:
+        url (str): The URL of the Telegram Bot API endpoint.
+        data (Dict): The data to send to the Telegram Bot API.
+    Returns:
+        Dict: The response from the Telegram Bot API as a dictionary.
+    """
+    encoded_data = json.dumps(data).encode('utf-8')
+    headers = {
+        'Content-Type': 'application/json'
+    }
+    try:
+        reader, writer = await asyncio.create_connection((self.server, self.port), ssl=self.ssl_context)
+        request = (f'POST {url} HTTP/1.1\r\n'
+                   f'Host: {self.server}\r\n'
+                   f'Content-Length: {len(encoded_data)}\r\n'
+                   f'Connection: close\r\n'
+                   f'{headers}\r\n').encode('utf-8') + encoded_data
+        writer.write(request)
+        response = await reader.read()
+        writer.close()
+    except (socket.gaierror, socket.error) as e:
+        logging.error(f'Error connecting to Telegram API: {e}')
+        return {}
+    try:
+        response = response.decode('utf-8')
+        response = json.loads(response)
+        return response
+    except ValueError:
+        return {}
 
 async def get_dialogs(self) -> List[Dict]:
     """
     Gets the list of dialogs for the authorized user.
     Returns:
         List[Dict]: A list of dialogs as dictionaries.
     """
```

### Comparing `yumikogram-0.0.8/yumikogram.egg-info/PKG-INFO` & `yumikogram-0.0.9/yumikogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yumikogram
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package for telegram bots making and api making
 Home-page: https://github.com/yumiko-api/yumikogram
 Author: santhosh
 Author-email: yumikoapi@gmail.com
 Keywords: yumikogram,telegram,telegram-bots,yumikogram api,telegram bots library
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

