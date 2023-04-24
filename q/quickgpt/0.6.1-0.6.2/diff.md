# Comparing `tmp/quickgpt-0.6.1.tar.gz` & `tmp/quickgpt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgpt-0.6.1.tar", last modified: Mon Apr 17 02:41:32 2023, max compression
+gzip compressed data, was "quickgpt-0.6.2.tar", last modified: Mon Apr 24 15:35:03 2023, max compression
```

## Comparing `quickgpt-0.6.1.tar` & `quickgpt-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.166690 quickgpt-0.6.1/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-17 02:41:32.166690 quickgpt-0.6.1/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-04-17 02:41:07.000000 quickgpt-0.6.1/README.rst
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/bin/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.6.1/bin/quickgpt
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/quickgpt/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-17 02:41:25.000000 quickgpt-0.6.1/quickgpt/__init__.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/quickgpt/thread/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     5932 2023-04-17 00:33:22.000000 quickgpt-0.6.1/quickgpt/thread/__init__.py
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      643 2023-03-27 17:04:18.000000 quickgpt-0.6.1/quickgpt/thread/messagetypes.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2552 2023-04-17 02:40:43.000000 quickgpt-0.6.1/quickgpt/thread/response.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/quickgpt.egg-info/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/requires.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/top_level.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-17 02:41:32.166690 quickgpt-0.6.1/setup.cfg
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      805 2023-04-17 02:41:18.000000 quickgpt-0.6.1/setup.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-24 15:35:03.884707 quickgpt-0.6.2/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-04-17 02:41:32.000000 quickgpt-0.6.2/README.rst
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/bin/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.6.2/bin/quickgpt
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/quickgpt/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-24 15:28:50.000000 quickgpt-0.6.2/quickgpt/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/quickgpt/thread/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     6593 2023-04-24 15:30:08.000000 quickgpt-0.6.2/quickgpt/thread/__init__.py
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      935 2023-04-24 15:32:21.000000 quickgpt-0.6.2/quickgpt/thread/messagetypes.py
+-rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2772 2023-04-24 15:32:27.000000 quickgpt-0.6.2/quickgpt/thread/response.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-24 15:35:03.884707 quickgpt-0.6.2/quickgpt.egg-info/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/requires.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-24 15:35:03.000000 quickgpt-0.6.2/quickgpt.egg-info/top_level.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-24 15:35:03.884707 quickgpt-0.6.2/setup.cfg
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      805 2023-04-24 15:24:28.000000 quickgpt-0.6.2/setup.py
```

### Comparing `quickgpt-0.6.1/PKG-INFO` & `quickgpt-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.6.1
+Version: 0.6.2
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
```

### Comparing `quickgpt-0.6.1/README.rst` & `quickgpt-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6.1/bin/quickgpt` & `quickgpt-0.6.2/bin/quickgpt`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6.1/quickgpt/__init__.py` & `quickgpt-0.6.2/quickgpt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from quickgpt.thread import Thread
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 import os
 
 class QuickGPT:
     def __init__(self, api_key=None, retry_count=3):
         """ Main QuickGPT object
```

### Comparing `quickgpt-0.6.1/quickgpt/thread/__init__.py` & `quickgpt-0.6.2/quickgpt/thread/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import openai
 import time
 import json
+import tiktoken
 
 from uuid import uuid4
 
 from quickgpt.thread.messagetypes import *
 from quickgpt.thread.response import Response
 
 class Thread:
@@ -13,14 +14,16 @@
         self.model = model
 
         openai.api_key = quickgpt.api_key
 
         self.thread = []
         self.id = str(uuid4())
 
+        self.tokenizer = None
+
     def __len__(self):
         """ Returns the length of the Thread, by message count
 
         Returns:
             int: Length of thread by message count
         """
 
@@ -31,14 +34,36 @@
             raise TypeError("list indices must be integers or slices, not %s" % type(index))
 
         return self.thread[index]
 
     def __setitem__(self, index, value):
         self.thread[index] = value
 
+    def get_tokens(self):
+        """ Returns the tokens of the current thread, using OpenAI's tiktoken
+
+        Currently hard-coded to use cl100k_base only for now.
+        """
+
+        if not self.tokenizer:
+            self.tokenizer = tiktoken.get_encoding("cl100k_base")
+
+        tokens = []
+
+        for message in self.thread:
+            _token = self.tokenizer.encode(message.message)
+            tokens += _token
+
+        return tokens
+
+    def get_tokens_length(self):
+        """ Returns the length of the current thread, in tokens """
+
+        return len(self.get_tokens())
+
     def serialize(self):
         """ Returns a serializable, JSON-friendly dict with all of the
         thread's data. Can be restored to a new Thread object later.
 
         Returns:
             dict: A JSON-safe representation of this thread, to be restored
                 later using thread.restore()
```

### Comparing `quickgpt-0.6.1/quickgpt/thread/response.py` & `quickgpt-0.6.2/quickgpt/thread/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import tiktoken
 
 class Response:
     def __init__(self, response_obj, stream=False):
         self._ = response_obj
         self.stream = stream
         self.complete = False
         self._message = ""
@@ -19,14 +20,20 @@
     def __str__(self):
         return "<assistant> %s" % self.message
 
     def __len__(self):
         """ Returns the length of the text, in characters """
         return len(self.message)
 
+    def get_tokens(self):
+        """ Returns the length of the content, in tokens """
+        tokenizer = tiktoken.get_encoding("cl100k_base")
+
+        return len(tokenizer.encode(self.message))
+
     @property
     def rsp(self):
         if self.stream:
             return self.gathered
         else:
             return self._
```

### Comparing `quickgpt-0.6.1/quickgpt.egg-info/PKG-INFO` & `quickgpt-0.6.2/quickgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.6.1
+Version: 0.6.2
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
```

### Comparing `quickgpt-0.6.1/setup.py` & `quickgpt-0.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='quickgpt',
-    version='0.6.1',
+    version='0.6.2',
     description='A barebones library to make interacting with OpenAI\'s ChatGPT API much simpler.',
     long_description=open("README.rst", "r").read(),
     author='Ben Baptist',
     author_email='me@benbaptist.com',
     url='https://github.com/benbaptist/quickgpt',
     packages=find_packages(),
     scripts=['bin/quickgpt'],
```

