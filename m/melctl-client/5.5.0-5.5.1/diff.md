# Comparing `tmp/melctl_client-5.5.0.tar.gz` & `tmp/melctl_client-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melctl_client-5.5.0.tar", last modified: Mon Apr  3 12:51:53 2023, max compression
+gzip compressed data, was "melctl_client-5.5.1.tar", last modified: Mon Apr 24 09:18:38 2023, max compression
```

## Comparing `melctl_client-5.5.0.tar` & `melctl_client-5.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:51:53.685690 melctl_client-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-03 12:51:44.000000 melctl_client-5.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-03 12:51:53.685690 melctl_client-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-03 12:51:44.000000 melctl_client-5.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:51:53.685690 melctl_client-5.5.0/melctl_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:51:53.685690 melctl_client-5.5.0/melctl_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:51:53.685690 melctl_client-5.5.0/melctl_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-03 12:51:53.000000 melctl_client-5.5.0/melctl_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-03 12:51:53.000000 melctl_client-5.5.0/melctl_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:51:53.000000 melctl_client-5.5.0/melctl_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-03 12:51:53.000000 melctl_client-5.5.0/melctl_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-03 12:51:53.000000 melctl_client-5.5.0/melctl_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-03 12:51:53.000000 melctl_client-5.5.0/melctl_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:51:53.681690 melctl_client-5.5.0/melctl_client_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:51:53.685690 melctl_client-5.5.0/melctl_client_plugins/builtins/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client_plugins/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client_plugins/builtins/complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client_plugins/builtins/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client_plugins/builtins/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client_plugins/builtins/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-03 12:51:44.000000 melctl_client-5.5.0/melctl_client_plugins/builtins/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 12:51:53.685690 melctl_client-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-03 12:51:44.000000 melctl_client-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-24 09:18:19.000000 melctl_client-5.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 09:18:38.138778 melctl_client-5.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 09:18:19.000000 melctl_client-5.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 09:18:38.000000 melctl_client-5.5.1/melctl_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client_plugins/builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:18:38.138778 melctl_client-5.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 09:18:19.000000 melctl_client-5.5.1/setup.py
```

### Comparing `melctl_client-5.5.0/LICENSE` & `melctl_client-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/PKG-INFO` & `melctl_client-5.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melctl_client
-Version: 5.5.0
+Version: 5.5.1
 Summary: Command-line client for LuxProvide API (MelCtl)
 Home-page: https://github.com/LuxProvide/melctl-client
 Author: jpclipffel
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 This package provides the base MelCtl command-line client.
```

### Comparing `melctl_client-5.5.0/melctl_client/__init__.py` & `melctl_client-5.5.1/melctl_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 __email__      = 'jean-philippe.clipffel@lxp.lu'
 __author__     = 'Jean-Philippe Clipffel <jean-philippe.clipffel@lxp.lu>'
 __license__    = 'BSD-3-Clause'
 __copyright__  = 'Copyright (c) 2023 LuxProvide S.A.'
 __maintainer__ = 'Jean-Philippe Clipffel'
 
 
-__version__ = '5.5.0'
+__version__ = '5.5.1'
 __version_name__ = 'Pedantic Santa'
```

### Comparing `melctl_client-5.5.0/melctl_client/__main__.py` & `melctl_client-5.5.1/melctl_client/__main__.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client/commands.py` & `melctl_client-5.5.1/melctl_client/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,15 +204,16 @@
     def format_error(self, args, error: Exception):
         """Format and print an error.
 
         :param args: Parsed command line arguments
         :param error: Exception
         """
         data = {
-            'error': str(error)
+            'error': str(error),
+            'response': getattr(error, 'jsdata', None)
         }
         if args.traceback:
             data['traceback'] = traceback.format_exc()
         # Format and print
         self.format(args, data)
 
     def wait_task(self, task_id: str, frequency: int, timeout: int):
@@ -304,14 +305,29 @@
                 jsdata = {}
             # Enforce table fields
             self.headers = 'keys'
             # Print error
             self.format(args, jsdata)
             raise error
 
+    def raise_for_status(self, req, *args, **kwargs):
+        """Raise an error in case of invalid status with extra information.
+
+        :param req: Current request
+        """
+        try:
+            req.raise_for_status(*args, **kwargs)
+        except Exception as error:
+            try:
+                setattr(error, 'jsdata', req.json())
+            except Exception:
+                pass
+            raise error
+
+
 class SimpleCommand(Command):
     """Generic command, easier to extend.
     """
 
     def __init__(self, subparser, action: str, method: str, urn: str,
                     *args, **kwargs):
         super().__init__(subparser, action, *args, **kwargs)
@@ -322,9 +338,10 @@
         """Command entry point.
 
         :param args: Parsed command line arguments
         """
         req = self.session.request(
             self.method,
             f'{self.url}/{self.urn.format_map(args.__dict__)}')
-        req.raise_for_status()
+        # req.raise_for_status()
+        self.raise_for_status(req)
         return req.json()
```

### Comparing `melctl_client-5.5.0/melctl_client/config.py` & `melctl_client-5.5.1/melctl_client/config.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client/hints.py` & `melctl_client-5.5.1/melctl_client/hints.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client/utils/__init__.py` & `melctl_client-5.5.1/melctl_client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client.egg-info/PKG-INFO` & `melctl_client-5.5.1/melctl_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melctl-client
-Version: 5.5.0
+Version: 5.5.1
 Summary: Command-line client for LuxProvide API (MelCtl)
 Home-page: https://github.com/LuxProvide/melctl-client
 Author: jpclipffel
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 This package provides the base MelCtl command-line client.
```

### Comparing `melctl_client-5.5.0/melctl_client.egg-info/SOURCES.txt` & `melctl_client-5.5.1/melctl_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client_plugins/builtins/__init__.py` & `melctl_client-5.5.1/melctl_client_plugins/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client_plugins/builtins/complete.py` & `melctl_client-5.5.1/melctl_client_plugins/builtins/complete.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client_plugins/builtins/conf.py` & `melctl_client-5.5.1/melctl_client_plugins/builtins/conf.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client_plugins/builtins/login.py` & `melctl_client-5.5.1/melctl_client_plugins/builtins/login.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client_plugins/builtins/ping.py` & `melctl_client-5.5.1/melctl_client_plugins/builtins/ping.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/melctl_client_plugins/builtins/version.py` & `melctl_client-5.5.1/melctl_client_plugins/builtins/version.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.0/setup.py` & `melctl_client-5.5.1/setup.py`

 * *Files identical despite different names*

