# Comparing `tmp/oaas_sdk_py-0.1.6.tar.gz` & `tmp/oaas_sdk_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaas_sdk_py-0.1.6.tar", last modified: Mon Apr 24 10:45:31 2023, max compression
+gzip compressed data, was "oaas_sdk_py-0.1.7.tar", last modified: Mon Apr 24 11:03:18 2023, max compression
```

## Comparing `oaas_sdk_py-0.1.6.tar` & `oaas_sdk_py-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:45:31.934728 oaas_sdk_py-0.1.6/
--rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      258 2023-04-24 10:45:31.933510 oaas_sdk_py-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.6/README.md
--rw-rw-rw-   0        0        0      495 2023-04-24 10:44:39.000000 oaas_sdk_py-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 10:45:31.934728 oaas_sdk_py-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 10:45:31.918788 oaas_sdk_py-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 10:45:31.924520 oaas_sdk_py-0.1.6/src/oaas_sdk_py/
--rw-rw-rw-   0        0        0     8948 2023-04-24 10:44:39.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py/__init__.py
--rw-rw-rw-   0        0        0     1740 2023-04-14 09:02:39.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py/model.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:45:31.932503 oaas_sdk_py-0.1.6/src/oaas_sdk_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-04-24 10:45:31.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-24 10:45:31.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:45:31.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-24 10:45:31.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 10:45:31.000000 oaas_sdk_py-0.1.6/src/oaas_sdk_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.235846 oaas_sdk_py-0.1.7/
+-rw-rw-rw-   0        0        0    11557 2023-02-10 20:57:09.000000 oaas_sdk_py-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      258 2023-04-24 11:03:18.234846 oaas_sdk_py-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-02-10 20:52:55.000000 oaas_sdk_py-0.1.7/README.md
+-rw-rw-rw-   0        0        0      495 2023-04-24 11:01:50.000000 oaas_sdk_py-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 11:03:18.235846 oaas_sdk_py-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.221095 oaas_sdk_py-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.226097 oaas_sdk_py-0.1.7/src/oaas_sdk_py/
+-rw-rw-rw-   0        0        0     8948 2023-04-24 10:44:39.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-04-24 11:01:38.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py/model.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:03:18.233847 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 11:03:18.000000 oaas_sdk_py-0.1.7/src/oaas_sdk_py.egg-info/top_level.txt
```

### Comparing `oaas_sdk_py-0.1.6/LICENSE` & `oaas_sdk_py-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.6/src/oaas_sdk_py/__init__.py` & `oaas_sdk_py-0.1.7/src/oaas_sdk_py/__init__.py`

 * *Files identical despite different names*

### Comparing `oaas_sdk_py-0.1.6/src/oaas_sdk_py/model.py` & `oaas_sdk_py-0.1.7/src/oaas_sdk_py/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,39 +12,41 @@
 
     @property
     def func(self):
         return self.json_dict['funcName']
 
 
 class OaasObject:
-    updated_keys: [str] = []
 
     def __init__(self, json_dict):
         self.json_dict = json_dict
         self.origin = OaasObjectOrigin(self.json_dict["origin"])
         self.data = self.json_dict.get("data", {})
+        self.updated_keys: [str] = []
 
     @property
     def id(self):
         return self.json_dict["id"]
 
 
 class OaasTask:
-    input: [OaasObject] = []
+    input: [OaasObject]
     output_obj: OaasObject = None
 
     def __init__(self, json_dict):
         self.json_dict = json_dict
         if 'output' in json_dict:
             self.output_obj = OaasObject(json_dict['output'])
         self.main_obj = OaasObject(json_dict['main'])
         self.alloc_url = json_dict.get('allocOutputUrl', {})
         self.alloc_main_url = json_dict.get('allocMainUrl', {})
         if 'inputs' in json_dict:
             self.inputs = [OaasObject(input_dict) for input_dict in json_dict['inputs']]
+        else:
+            self.inputs = []
         self.main_keys = json_dict.get('mainKeys', {})
         self.input_keys = json_dict.get('inputKeys', [])
         if 'args' in json_dict:
             self.args = json_dict['args']
         else:
             self.args = {}
```

