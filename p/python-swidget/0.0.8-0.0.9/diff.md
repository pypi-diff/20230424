# Comparing `tmp/python_swidget-0.0.8.tar.gz` & `tmp/python_swidget-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_swidget-0.0.8.tar", max compression
+gzip compressed data, was "python_swidget-0.0.9.tar", max compression
```

## Comparing `python_swidget-0.0.8.tar` & `python_swidget-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       59 2023-01-11 19:11:12.359430 python_swidget-0.0.8/README.md
--rw-r--r--   0        0        0     2112 2023-01-11 19:47:29.469449 python_swidget-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1264 2023-01-11 19:11:12.359430 python_swidget-0.0.8/swidget/__init__.py
--rw-r--r--   0        0        0     6327 2023-01-11 19:11:12.359430 python_swidget-0.0.8/swidget/cli.py
--rw-r--r--   0        0        0     3483 2023-01-11 19:37:08.299444 python_swidget-0.0.8/swidget/discovery.py
--rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-0.0.8/swidget/exceptions.py
--rw-r--r--   0        0        0      595 2023-01-11 19:17:05.439433 python_swidget-0.0.8/swidget/provision.py
--rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-0.0.8/swidget/py.typed
--rw-r--r--   0        0        0    12659 2023-01-11 19:18:20.139434 python_swidget-0.0.8/swidget/swidgetdevice.py
--rw-r--r--   0        0        0     1525 2023-01-11 19:46:28.219448 python_swidget-0.0.8/swidget/swidgetdimmer.py
--rw-r--r--   0        0        0      384 2023-01-11 19:46:48.669448 python_swidget-0.0.8/swidget/swidgetoutlet.py
--rw-r--r--   0        0        0      574 2023-01-11 19:46:59.259448 python_swidget-0.0.8/swidget/swidgetswitch.py
--rw-r--r--   0        0        0      649 2023-01-11 19:47:08.599449 python_swidget-0.0.8/swidget/swidgettimerswitch.py
--rw-r--r--   0        0        0     4519 2023-01-11 19:18:26.769434 python_swidget-0.0.8/swidget/websocket.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 python_swidget-0.0.8/setup.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 python_swidget-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-01-11 19:11:12.359430 python_swidget-0.0.9/README.md
+-rw-r--r--   0        0        0     2112 2023-01-11 22:03:19.879384 python_swidget-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1264 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/__init__.py
+-rw-r--r--   0        0        0     6327 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/cli.py
+-rw-r--r--   0        0        0     3483 2023-01-11 19:37:08.299444 python_swidget-0.0.9/swidget/discovery.py
+-rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/exceptions.py
+-rw-r--r--   0        0        0      595 2023-01-11 19:17:05.439433 python_swidget-0.0.9/swidget/provision.py
+-rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-0.0.9/swidget/py.typed
+-rw-r--r--   0        0        0    12739 2023-01-11 22:02:31.839384 python_swidget-0.0.9/swidget/swidgetdevice.py
+-rw-r--r--   0        0        0     1525 2023-01-11 19:46:28.219448 python_swidget-0.0.9/swidget/swidgetdimmer.py
+-rw-r--r--   0        0        0      384 2023-01-11 19:46:48.669448 python_swidget-0.0.9/swidget/swidgetoutlet.py
+-rw-r--r--   0        0        0      574 2023-01-11 19:46:59.259448 python_swidget-0.0.9/swidget/swidgetswitch.py
+-rw-r--r--   0        0        0      649 2023-01-11 19:47:08.599449 python_swidget-0.0.9/swidget/swidgettimerswitch.py
+-rw-r--r--   0        0        0     4521 2023-01-11 20:18:00.769464 python_swidget-0.0.9/swidget/websocket.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 python_swidget-0.0.9/setup.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 python_swidget-0.0.9/PKG-INFO
```

### Comparing `python_swidget-0.0.8/pyproject.toml` & `python_swidget-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-swidget"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python API for Swidget smart devices"
 license = "GPL-3.0-or-later"
 authors = ["Swidget"]
 repository = "https://github.com/swidget/python-swidget"
 readme = "README.md"
 packages = [
   { include = "swidget" }
```

### Comparing `python_swidget-0.0.8/swidget/__init__.py` & `python_swidget-0.0.9/swidget/__init__.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/cli.py` & `python_swidget-0.0.9/swidget/cli.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/discovery.py` & `python_swidget-0.0.9/swidget/discovery.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/provision.py` & `python_swidget-0.0.9/swidget/provision.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/swidgetdevice.py` & `python_swidget-0.0.9/swidget/swidgetdevice.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             self._websocket = SwidgetWebsocket(
                 host=self.ip_address,
                 token_name=self.token_name,
                 secret_key=self.secret_key,
                 callback=self.message_callback,
                 session=self._session)
 
+    def set_countdown_timer(self, minutes):
+        raise NotImplementedError()
 
     def stop(self):
         """Stop the websocket."""
         if self._websocket is not None:
             self._websocket.stop()
 
     async def message_callback(self, message):
```

### Comparing `python_swidget-0.0.8/swidget/swidgetdimmer.py` & `python_swidget-0.0.9/swidget/swidgetdimmer.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/swidgetswitch.py` & `python_swidget-0.0.9/swidget/swidgetswitch.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/swidgettimerswitch.py` & `python_swidget-0.0.9/swidget/swidgettimerswitch.py`

 * *Files identical despite different names*

### Comparing `python_swidget-0.0.8/swidget/websocket.py` & `python_swidget-0.0.9/swidget/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         else:
             if self.state != STATE_STOPPED:
                 self.state = STATE_DISCONNECTED
 
                 await asyncio.sleep(5)
 
     async def send_str(self, message):
-        _LOGGER.error(f"Sending Message: {message}")
+        # _LOGGER.error(f"Sending Message: {message}")
         message = str(message)
         await self.ws_client.send_str(f'{message}')
 
     async def listen(self):
         """Close the listening websocket."""
         self.failed_attempts = 0
         while self.state != STATE_STOPPED:
```

### Comparing `python_swidget-0.0.8/setup.py` & `python_swidget-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
           'sphinxcontrib-programoutput>=0,<1']}
 
 entry_points = \
 {'console_scripts': ['swidget = swidget.cli:cli']}
 
 setup_kwargs = {
     'name': 'python-swidget',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Python API for Swidget smart devices',
     'long_description': '# python-swidget\nA library to manage Swidget smart devices\n',
     'author': 'Swidget',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/swidget/python-swidget',
```

### Comparing `python_swidget-0.0.8/PKG-INFO` & `python_swidget-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-swidget
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python API for Swidget smart devices
 Home-page: https://github.com/swidget/python-swidget
 License: GPL-3.0-or-later
 Author: Swidget
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

