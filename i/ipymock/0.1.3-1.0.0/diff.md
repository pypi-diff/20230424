# Comparing `tmp/ipymock-0.1.3.tar.gz` & `tmp/ipymock-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.1.3.tar", last modified: Fri Apr 21 22:21:57 2023, max compression
+gzip compressed data, was "ipymock-1.0.0.tar", last modified: Mon Apr 24 01:56:16 2023, max compression
```

## Comparing `ipymock-0.1.3.tar` & `ipymock-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.065845 ipymock-0.1.3/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.3/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.3/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-21 22:21:57.065544 ipymock-0.1.3/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-21 22:21:41.000000 ipymock-0.1.3/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.061982 ipymock-0.1.3/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-21 22:21:33.000000 ipymock-0.1.3/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-21 22:21:33.000000 ipymock-0.1.3/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     9912 2023-04-21 22:21:33.000000 ipymock-0.1.3/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.064025 ipymock-0.1.3/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.064887 ipymock-0.1.3/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.3/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.3/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.3/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-21 22:21:24.000000 ipymock-0.1.3/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-21 22:21:57.065964 ipymock-0.1.3/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.3/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.101354 ipymock-1.0.0/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.0/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.0/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-24 01:56:16.100237 ipymock-1.0.0/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-24 01:37:41.000000 ipymock-1.0.0/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.094857 ipymock-1.0.0/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1605 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     2306 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)    20991 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/agi.py
+-rw-r--r--   0 saintway   (501) staff       (20)    11200 2023-04-24 01:37:27.000000 ipymock-1.0.0/ipymock/browser.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.098230 ipymock-1.0.0/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-24 01:56:16.099401 ipymock-1.0.0/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.0/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.0/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      427 2023-04-24 01:56:16.000000 ipymock-1.0.0/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.0/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       62 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-24 01:56:15.000000 ipymock-1.0.0/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2519 2023-04-24 01:44:18.000000 ipymock-1.0.0/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-24 01:56:16.101551 ipymock-1.0.0/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.0/setup.py
```

### Comparing `ipymock-0.1.3/LICENSE` & `ipymock-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.3/PKG-INFO` & `ipymock-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.3
+Version: 1.0.0
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.1.3/README.md` & `ipymock-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.3/ipymock/__init__.py` & `ipymock-1.0.0/ipymock/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/core.ipynb (unless otherwise specified).
+# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/1_core.ipynb (unless otherwise specified).
 
 __all__ = ['get_test_funcs', 'print_result', 'do']
 
 # Cell
 import py
 import sys
 import traceback
```

### Comparing `ipymock-0.1.3/ipymock/mock.py` & `ipymock-1.0.0/ipymock/browser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/mock.ipynb (unless otherwise specified).
+# AUTOGENERATED! DO NOT EDIT! File to edit: nbs/2_browser.ipynb (unless otherwise specified).
 
-__all__ = ['get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
+__all__ = ['common', 'get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
            'generate_title', 'rename_title', 'delete_conversation', 'recover_conversation', 'clear_conversations',
-           'chat_gpt_base_url', 'common', 'attrdict', 'attributize', 'delta', 'mock_create', 'chat_delta',
-           'mock_chat_create', 'mock_openai']
+           'attrdict', 'attributize', 'delta', 'mock_create', 'chat_delta', 'mock_chat_create', 'mock_openai']
 
 # Internal Cell
 from queue import Queue
 
 class Common:
+    chat_gpt_base_url = 'http://127.0.0.1:8080'
+    access_token = None
+
     chat_gpt_model = 'gpt-3.5-turbo'
     role_user = 'user'
     role_assistant = 'assistant'
 
     question_answer_map = {}
     message_channel = Queue()
     exit_for_loop_channel = Queue()
     response_text_channel = Queue()
     conversation_done_channel = Queue()
     parent_message_id = ''
     conversation_id = ''
     reload_conversations_channel = Queue()
 
 # Internal Cell
-import json, os, requests, sys, uuid
+import json, os, requests, sys, time, uuid
 
 # Cell
-chat_gpt_base_url = 'http://127.0.0.1:8080'
-
-# open the JSON file and read the access_token
-with open(os.path.expanduser('~/.config/revChatGPT/config.json'), 'r') as f:
-    access_token = json.load(f).get('access_token', None)
-
 common = Common()
 
+# open the JSON file and read the access_token and conversation_id
+with open(os.path.expanduser('~/.config/ipymock/config.json'), 'r') as f:
+    config = json.load(f)
+    common.access_token = config.get('access_token', None)
+    common.conversation_id = config.get('conversation_id', None)
 
+# Cell
 def get_conversations():
-    response = requests.get(f'{chat_gpt_base_url}/conversations?offset=0&limit=100', headers = {'Authorization': access_token})
+    response = requests.get(f'{common.chat_gpt_base_url}/conversations?offset=0&limit=100', headers = {'Authorization': common.access_token})
     return response.json()
 
 def get_conversation(conversation_id):
-    response = requests.get(f'{chat_gpt_base_url}/conversation/{conversation_id}', headers = {'Authorization': access_token})
+    response = requests.get(f'{common.chat_gpt_base_url}/conversation/{conversation_id}', headers = {'Authorization': common.access_token})
     conversation = response.json()
     current_node = conversation['current_node']
-    common.parent_message_id = current_node
-    handle_conversation_detail(current_node, conversation['mapping'])
+    try:
+        handle_conversation_detail(current_node, conversation['mapping'])
+    except RecursionError as errr:
+        sys.stderr.write(f'Error Recursing: {errr}\n')
     common.exit_for_loop_channel.put(True)
+    return current_node
 
 def handle_conversation_detail(current_node, mapping):
     conversation_detail = mapping[current_node]
     parent_id = conversation_detail.get('parent', '')
     if parent_id != '':
-        common.question_answer_map[parent_id] = conversation_detail['message']['content']['parts'][0].strip()
         handle_conversation_detail(parent_id, mapping)
+        common.question_answer_map[parent_id] = conversation_detail['message']['content']['parts'][0].strip()
     if 'message' not in conversation_detail:
         return
     message = conversation_detail['message']
     parts = message['content']['parts']
-    if len(parts) > 0 and parts[0] != '':
-        if message['author']['role'] == common.role_user:
-            common.message_channel.put(message)
+    if len(parts) > 0 and parts[0] != '' and message['author']['role'] == common.role_user:
+        common.message_channel.put(message)
 
 def start_conversation(content):
     if common.conversation_id != '' and common.parent_message_id == '':
         try:
-            # set common.parent_message_id
-            get_conversation(common.conversation_id)
+            common.parent_message_id = get_conversation(common.conversation_id)
         except requests.exceptions.ConnectionError as errc:
             sys.stderr.write(f'Error Connecting: {errc}\n')
-        except RecursionError as errr:
-            sys.stderr.write(f'Error Recursion: {errr}\n')
 
     if common.conversation_id == '' or common.parent_message_id == '':
         common.conversation_id = ''
         common.parent_message_id = str(uuid.uuid4())
 
     post_data = {
         'action': 'next',
@@ -93,17 +94,17 @@
     }
     if common.conversation_id != '':
         post_data['conversation_id'] = common.conversation_id
     if common.parent_message_id != '':
         post_data['parent_message_id'] = common.parent_message_id
 
     response = requests.post(
-        f'{chat_gpt_base_url}/conversation',
+        f'{common.chat_gpt_base_url}/conversation',
         headers = {
-            'Authorization': access_token,
+            'Authorization': common.access_token,
             'Content-Type': 'application/json',
             'Accept': 'text/event-stream'
         },
         data = json.dumps(post_data),
         stream=True
     )
 
@@ -130,80 +131,80 @@
         if common.conversation_id == '':
             temp_conversation_id = make_conversation_response['conversation_id']
         common.parent_message_id = make_conversation_response['message']['id']
         if make_conversation_response['message']['end_turn'] == True:
             common.conversation_done_channel.put(True)
             continue
 
+    if response.status_code >= 400:
+        sys.stderr.write(f'Error Status Code: {response.status_code}\n')
+    response.raise_for_status()
+
     if common.conversation_id == '' and temp_conversation_id != '':
         common.conversation_id = temp_conversation_id
         generate_title(common.conversation_id)
     else:
         common.reload_conversations_channel.put(True)
 
 def generate_title(conversation_id):
     requests.post(
-        f'{chat_gpt_base_url}/conversation/gen_title/{conversation_id}',
+        f'{common.chat_gpt_base_url}/conversation/gen_title/{conversation_id}',
         headers = {
-            'Authorization': access_token,
+            'Authorization': common.access_token,
             'Content-Type': 'application/json'
         },
         data = json.dumps({
-            'message_id': common.parent_message_id,
+            'message_id': get_conversation(conversation_id),
             'model': common.chat_gpt_model
         })
     )
 
 def rename_title(conversation_id, title):
     requests.patch(
-        f'{chat_gpt_base_url}/conversation/{conversation_id}',
+        f'{common.chat_gpt_base_url}/conversation/{conversation_id}',
         headers={
-            'Authorization': access_token,
+            'Authorization': common.access_token,
             'Content-Type': 'application/json'
         },
         data = json.dumps({
             'title': title
         })
     )
 
 def delete_conversation(conversation_id):
     requests.patch(
-        f'{chat_gpt_base_url}/conversation/{conversation_id}',
+        f'{common.chat_gpt_base_url}/conversation/{conversation_id}',
         headers={
-            'Authorization': access_token,
+            'Authorization': common.access_token,
             'Content-Type': 'application/json'
         },
         data=json.dumps({
             'is_visible': False
         })
     )
 
 def recover_conversation(conversation_id):
     requests.patch(
-        f'{chat_gpt_base_url}/conversation/{conversation_id}',
+        f'{common.chat_gpt_base_url}/conversation/{conversation_id}',
         headers={
-            'Authorization': access_token,
+            'Authorization': common.access_token,
             'Content-Type': 'application/json'
         },
         data=json.dumps({
             'is_visible': True
         })
     )
 
 def clear_conversations():
-    requests.patch(f'{chat_gpt_base_url}/conversations', headers = {'Authorization': access_token}, data = {'is_visible': False})
+    requests.patch(f'{common.chat_gpt_base_url}/conversations', headers = {'Authorization': common.access_token}, data = {'is_visible': False})
 
     common.conversation_id = ''
+    common.parent_message_id = ''
     common.reload_conversations_channel.put(True)
 
-# Internal Cell
-# open the JSON file and read the conversation_id
-with open(os.path.expanduser('~/.config/revChatGPT/config.json'), 'r') as f:
-    common.conversation_id = json.load(f).get('conversation_id', None)
-
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
 def attributize(obj):
     '''Add attributes to a dictionary and its sub-dictionaries.'''
@@ -239,16 +240,45 @@
 
     if kwargs.get('stream', False):
         return delta('\n'.join(prompts))
 
     choices = []
     for prompt in prompts:
         response = ''
-        for response in start_conversation(prompt):
-            pass
+        wait_second = 1
+        while True:
+            try:
+                for response in start_conversation(prompt):
+                    pass
+            except requests.exceptions.HTTPError as err:
+                sys.stderr.write(
+                    f'{err}\n'
+                    f'response = {repr(response)}\n'
+                    f'Retrying...\n'
+                )
+                status_code = err.response.status_code
+                if status_code == 413:
+                    # todo: split the prompt
+                    break
+                if status_code == 429:
+                    break
+                if status_code >= 400 and status_code != 500:
+                    time.sleep(wait_second)
+                    wait_second *= 2
+                    continue
+                break
+            if response == '':
+                sys.stderr.write(
+                    f'Error Responding: response = {repr(response)}\n'
+                    f'Retrying...\n'
+                )
+                time.sleep(wait_second)
+                wait_second *= 2
+                continue
+            break
         choices.append({
             'finish_reason': 'stop',
             'index': 0,
             'logprobs': None,
             'text': response,
         })
     return attributize({
@@ -283,14 +313,16 @@
 
     if kwargs.get('stream', False):
         return chat_delta(summarized_prompt)
 
     response = ''
     for response in start_conversation(summarized_prompt):
         pass
+    if response == '':
+        sys.stderr.write(f'Error Responding: {repr(response)}\n')
     return attributize({
         'choices': [
             {
                 'finish_reason': 'stop',
                 'index': 0,
                 'message': {
                     'content': response,
```

### Comparing `ipymock-0.1.3/ipymock.egg-info/PKG-INFO` & `ipymock-1.0.0/ipymock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.3
+Version: 1.0.0
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ipymock-0.1.3/settings.ini` & `ipymock-1.0.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.1.3
+version = 1.0.0
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
 status = 2
 
 # Optional. Same format as setuptools requirements
-requirements = pytest==6.* nbdev==1.* openai==0.*
+requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.*
 # Optional. Same format as setuptools console_scripts
 # console_scripts = 
 # Optional. Same format as setuptools dependency-links
 # dep_links = 
 
 ###
 # You probably won't need to change anything under here,
```

### Comparing `ipymock-0.1.3/setup.py` & `ipymock-1.0.0/setup.py`

 * *Files identical despite different names*

