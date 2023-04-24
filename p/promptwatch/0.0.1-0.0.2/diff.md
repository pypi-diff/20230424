# Comparing `tmp/promptwatch-0.0.1.tar.gz` & `tmp/promptwatch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.1.tar", last modified: Mon Apr 24 13:19:14 2023, max compression
+gzip compressed data, was "promptwatch-0.0.2.tar", last modified: Mon Apr 24 20:11:04 2023, max compression
```

## Comparing `promptwatch-0.0.1.tar` & `promptwatch-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 13:19:14.808258 promptwatch-0.0.1/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-04-24 13:19:14.808096 promptwatch-0.0.1/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3781 2023-04-21 05:55:12.000000 promptwatch-0.0.1/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.1/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-04-24 13:19:14.808301 promptwatch-0.0.1/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1137 2023-04-24 13:18:48.000000 promptwatch-0.0.1/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 13:19:14.803615 promptwatch-0.0.1/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 13:19:14.806375 promptwatch-0.0.1/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      206 2023-04-24 13:03:04.000000 promptwatch-0.0.1/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2284 2023-04-22 17:25:04.000000 promptwatch-0.0.1/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.1/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1506 2023-04-22 10:56:22.000000 promptwatch-0.0.1/src/promptwatch/decorators.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16765 2023-04-22 20:40:51.000000 promptwatch-0.0.1/src/promptwatch/langchain_handler.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15224 2023-04-23 21:00:16.000000 promptwatch-0.0.1/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      559 2023-04-22 10:49:03.000000 promptwatch-0.0.1/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 13:19:14.807883 promptwatch-0.0.1/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-04-24 13:19:14.000000 promptwatch-0.0.1/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      480 2023-04-24 13:19:14.000000 promptwatch-0.0.1/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-24 13:19:14.000000 promptwatch-0.0.1/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.1/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       19 2023-04-24 13:19:14.000000 promptwatch-0.0.1/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-04-24 13:19:14.000000 promptwatch-0.0.1/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.342497 promptwatch-0.0.2/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-04-24 20:11:04.342336 promptwatch-0.0.2/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3781 2023-04-21 05:55:12.000000 promptwatch-0.0.2/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.2/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-04-24 20:11:04.342541 promptwatch-0.0.2/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1137 2023-04-24 13:18:48.000000 promptwatch-0.0.2/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.338345 promptwatch-0.0.2/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.340617 promptwatch-0.0.2/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      206 2023-04-24 20:10:51.000000 promptwatch-0.0.2/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2284 2023-04-22 17:25:04.000000 promptwatch-0.0.2/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.2/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1506 2023-04-22 10:56:22.000000 promptwatch-0.0.2/src/promptwatch/decorators.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16765 2023-04-22 20:40:51.000000 promptwatch-0.0.2/src/promptwatch/langchain_handler.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15224 2023-04-24 20:09:25.000000 promptwatch-0.0.2/src/promptwatch/promptwatch_context.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      559 2023-04-22 10:49:03.000000 promptwatch-0.0.2/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-04-24 20:11:04.342121 promptwatch-0.0.2/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4154 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      480 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.2/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       19 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-04-24 20:11:04.000000 promptwatch-0.0.2/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.1/PKG-INFO` & `promptwatch-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.1
+Version: 0.0.2
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.1/README.md` & `promptwatch-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/setup.py` & `promptwatch-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/src/promptwatch/client.py` & `promptwatch-0.0.2/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/src/promptwatch/data_model.py` & `promptwatch-0.0.2/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/src/promptwatch/decorators.py` & `promptwatch-0.0.2/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/src/promptwatch/langchain_handler.py` & `promptwatch-0.0.2/src/promptwatch/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/src/promptwatch/promptwatch_context.py` & `promptwatch-0.0.2/src/promptwatch/promptwatch_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             if tenant_id.startswith("temp_"):
                 if session_id:
                     self.logger.warn("Setting up session_id with a temporary PromptWatch API Key is not allowed. You session_id will be ignored")
                 self.session_id = tenant_id[5:]
                 GREEN = '\033[32m'
                 RESET = '\033[0m'
                 print(f"{GREEN}You are using a temporary API key. Do not use in production.")
-                print(f"Visit the the detail of this session at https://app.promptwatch.io/sessions?temp-api-key={api_key} {RESET}")
+                print(f"Visit the the detail of this session at https://www.promptwatch.io/sessions?temp-api-key={api_key} {RESET}")
                 
 
 
 
         self.client = Client(api_key=api_key)
```

### Comparing `promptwatch-0.0.1/src/promptwatch/utils.py` & `promptwatch-0.0.2/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.1/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.0.2/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.1
+Version: 0.0.2
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

