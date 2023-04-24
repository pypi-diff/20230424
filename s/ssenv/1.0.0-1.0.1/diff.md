# Comparing `tmp/ssenv-1.0.0.tar.gz` & `tmp/ssenv-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssenv-1.0.0.tar", last modified: Mon Apr 24 17:09:53 2023, max compression
+gzip compressed data, was "ssenv-1.0.1.tar", last modified: Mon Apr 24 17:38:31 2023, max compression
```

## Comparing `ssenv-1.0.0.tar` & `ssenv-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:09:53.241269 ssenv-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-24 17:09:53.241269 ssenv-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-24 17:09:42.000000 ssenv-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:09:53.241269 ssenv-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-24 17:09:42.000000 ssenv-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:09:53.237269 ssenv-1.0.0/ssenv/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 17:09:42.000000 ssenv-1.0.0/ssenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-24 17:09:42.000000 ssenv-1.0.0/ssenv/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:09:53.237269 ssenv-1.0.0/ssenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-24 17:09:53.000000 ssenv-1.0.0/ssenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 17:09:53.000000 ssenv-1.0.0/ssenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:09:53.000000 ssenv-1.0.0/ssenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 17:09:53.000000 ssenv-1.0.0/ssenv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:09:53.237269 ssenv-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 17:09:42.000000 ssenv-1.0.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:38:31.941612 ssenv-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-24 17:38:18.000000 ssenv-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-24 17:38:31.941612 ssenv-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-24 17:38:18.000000 ssenv-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:38:31.941612 ssenv-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-24 17:38:18.000000 ssenv-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:38:31.937612 ssenv-1.0.1/ssenv/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 17:38:18.000000 ssenv-1.0.1/ssenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 17:38:18.000000 ssenv-1.0.1/ssenv/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:38:31.941612 ssenv-1.0.1/ssenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-24 17:38:31.000000 ssenv-1.0.1/ssenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 17:38:31.000000 ssenv-1.0.1/ssenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:38:31.000000 ssenv-1.0.1/ssenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 17:38:31.000000 ssenv-1.0.1/ssenv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:38:31.941612 ssenv-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 17:38:18.000000 ssenv-1.0.1/tests/test.py
```

### Comparing `ssenv-1.0.0/PKG-INFO` & `ssenv-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ssenv
-Version: 1.0.0
+Version: 1.0.1
 Summary: Super Duper Simple dotenv (.env) handler
 Home-page: https://github.com/asheswook/Environment
 Author: Jaewook Lee
 Author-email: me@jwlee.xyz
 Project-URL: Bug Tracker, https://github.com/asheswook/Environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Super Simple Environment
 
 ![Release](https://shields.io/github/v/release/asheswook/Environment?display_name=tag&sort=semver) ![build](https://img.shields.io/github/actions/workflow/status/asheswook/Environment/docker-workflow.yml?branch=main)
 
 Super Duper Simple, Super Duper Easy dotenv (.env) package in Python.
 
@@ -58,13 +59,7 @@
 **Use it!**
 
 You can use the dotenv file by using `get()` method. If you want to get the value of the dotenv, you can just use `get()` method with the key of the dotenv. If the dotenv file doesn't have the key, it will return `None`.
 
 ```python
 pwd = env.get('MY_PASSWORD')
 ```
-
-If you don't like to use `get()` method, you can also use the dotenv file by using `[]` operator.
-
-```python
-pwd = env['MY_PASSWORD']
-```
```

### Comparing `ssenv-1.0.0/README.md` & `ssenv-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -44,13 +44,7 @@
 **Use it!**
 
 You can use the dotenv file by using `get()` method. If you want to get the value of the dotenv, you can just use `get()` method with the key of the dotenv. If the dotenv file doesn't have the key, it will return `None`.
 
 ```python
 pwd = env.get('MY_PASSWORD')
 ```
-
-If you don't like to use `get()` method, you can also use the dotenv file by using `[]` operator.
-
-```python
-pwd = env['MY_PASSWORD']
-```
```

### Comparing `ssenv-1.0.0/setup.py` & `ssenv-1.0.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 requirements = [
 ]
 
 setuptools.setup(
     name='ssenv',
-    version='1.0.0',
+    version='1.0.1',
     author='Jaewook Lee',
     author_email='me@jwlee.xyz',
     description='Super Duper Simple dotenv (.env) handler',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/asheswook/Environment',
     project_urls={
```

### Comparing `ssenv-1.0.0/ssenv/main.py` & `ssenv-1.0.1/ssenv/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 class Environment:
     def __init__(self):
         self._dotenv_path = os.path.join(os.getcwd(), '.env')
         self._dotenv_dict = {}
         self.load_dotenv()
     
-    def __str__(self) -> dict:
-        return self._dotenv_dict
-
     def load_dotenv(self):
         with open(self._dotenv_path) as f:
             for line in f:
                 line = line.strip()
                 if not line or line.startswith('#'):
                     continue
                 k, v = line.split('=', 1)
-                self.dotenv_dict[k] = v
+                self._dotenv_dict[k] = v
 
     def get(self, key: str):
         return self._dotenv_dict[key] if key in self._dotenv_dict else None
```

### Comparing `ssenv-1.0.0/ssenv.egg-info/PKG-INFO` & `ssenv-1.0.1/ssenv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ssenv
-Version: 1.0.0
+Version: 1.0.1
 Summary: Super Duper Simple dotenv (.env) handler
 Home-page: https://github.com/asheswook/Environment
 Author: Jaewook Lee
 Author-email: me@jwlee.xyz
 Project-URL: Bug Tracker, https://github.com/asheswook/Environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Super Simple Environment
 
 ![Release](https://shields.io/github/v/release/asheswook/Environment?display_name=tag&sort=semver) ![build](https://img.shields.io/github/actions/workflow/status/asheswook/Environment/docker-workflow.yml?branch=main)
 
 Super Duper Simple, Super Duper Easy dotenv (.env) package in Python.
 
@@ -58,13 +59,7 @@
 **Use it!**
 
 You can use the dotenv file by using `get()` method. If you want to get the value of the dotenv, you can just use `get()` method with the key of the dotenv. If the dotenv file doesn't have the key, it will return `None`.
 
 ```python
 pwd = env.get('MY_PASSWORD')
 ```
-
-If you don't like to use `get()` method, you can also use the dotenv file by using `[]` operator.
-
-```python
-pwd = env['MY_PASSWORD']
-```
```

