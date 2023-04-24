# Comparing `tmp/PyVkBot-1.0.5.tar.gz` & `tmp/pyvkbot-2.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVkBot-1.0.5.tar", last modified: Mon Dec  5 22:46:13 2022, max compression
+gzip compressed data, was "pyvkbot-2.0.0.1.tar", max compression
```

## Comparing `PyVkBot-1.0.5.tar` & `pyvkbot-2.0.0.1.tar`

### file list

```diff
@@ -1,17 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 22:46:13.282638 PyVkBot-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2022-12-05 22:46:13.282638 PyVkBot-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 22:46:13.282638 PyVkBot-1.0.5/PyVkBot/
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2022-12-05 22:45:59.000000 PyVkBot-1.0.5/PyVkBot/Bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-05 22:45:59.000000 PyVkBot-1.0.5/PyVkBot/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-05 22:45:59.000000 PyVkBot-1.0.5/PyVkBot/Keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-05 22:45:59.000000 PyVkBot-1.0.5/PyVkBot/Types.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-05 22:45:59.000000 PyVkBot-1.0.5/PyVkBot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 22:46:13.282638 PyVkBot-1.0.5/PyVkBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2022-12-05 22:46:13.000000 PyVkBot-1.0.5/PyVkBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-05 22:46:13.000000 PyVkBot-1.0.5/PyVkBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 22:46:13.000000 PyVkBot-1.0.5/PyVkBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 22:46:13.000000 PyVkBot-1.0.5/PyVkBot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-05 22:46:13.000000 PyVkBot-1.0.5/PyVkBot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-05 22:46:13.000000 PyVkBot-1.0.5/PyVkBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 22:46:13.286638 PyVkBot-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-05 22:45:59.000000 PyVkBot-1.0.5/setup.py
+-rw-r--r--   0        0        0     1063 2023-04-24 12:05:44.202220 pyvkbot-2.0.0.1/LICENSE.md
+-rw-r--r--   0        0        0     4626 2023-04-24 12:05:44.202220 pyvkbot-2.0.0.1/README.md
+-rw-r--r--   0        0        0      502 2023-04-24 12:23:43.484184 pyvkbot-2.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7896 2023-04-24 12:05:44.205554 pyvkbot-2.0.0.1/pyvkbot/Bot.py
+-rw-r--r--   0        0        0      154 2023-04-24 12:05:44.205554 pyvkbot-2.0.0.1/pyvkbot/Exceptions.py
+-rw-r--r--   0        0        0      506 2023-04-24 12:05:44.205554 pyvkbot-2.0.0.1/pyvkbot/Keyboard.py
+-rw-r--r--   0        0        0      776 2023-04-24 12:05:44.205554 pyvkbot-2.0.0.1/pyvkbot/Types.py
+-rw-r--r--   0        0        0      211 2023-04-24 12:05:44.205554 pyvkbot-2.0.0.1/pyvkbot/__init__.py
+-rw-r--r--   0        0        0      614 2023-04-24 12:05:44.205554 pyvkbot-2.0.0.1/pyvkbot/__main__.py
+-rw-r--r--   0        0        0     5467 1970-01-01 00:00:00.000000 pyvkbot-2.0.0.1/setup.py
+-rw-r--r--   0        0        0     5112 1970-01-01 00:00:00.000000 pyvkbot-2.0.0.1/PKG-INFO
```

### Comparing `PyVkBot-1.0.5/PKG-INFO` & `pyvkbot-2.0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
-Name: PyVkBot
-Version: 1.0.5
-Summary: Chat bot for vk.com
-Home-page: https://github.com/zeph1rrinc/pyvkbot
+Name: pyvkbot
+Version: 2.0.0.1
+Summary: Package for creating vk bots
 Author: zeph1rr
 Author-email: grianton535@gmail.com
-License: MIT
-Requires-Python: >3.10
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: vk-api (>=11.9.9,<12.0.0)
 Description-Content-Type: text/markdown
 
-﻿# PYVKBOT
+# PYVKBOT
 
 ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=black)
 
 [![tests&build](https://img.shields.io/github/workflow/status/zeph1rrinc/pyvkbot/tests/master?label=test%26build&logo=github&logoColor=white)](https://github.com/zeph1rrinc/pyvkbot/actions)
 [![LICENCE](https://img.shields.io/badge/License-MIT-yellow.svg?logo=ReadtheDocs&logoColor=white)](/LICENSE.md)
 [![Version](https://img.shields.io/pypi/v/pyvkbot?logo=pypi&logoColor=white)](https://pypi.org/project/PyVkBot/)
 
@@ -26,16 +30,16 @@
 ## Bot
 ### Methods
 ### init
 Creating instance for future working
 
 Params:
 - token: str - access token of your group
+- group_id: int - id of your group
 - main_chat: int - [OPTIONAL] main chat for bot
-- group_id: int - [OPTIONAL] id of your group
 - logging: bool - [OPTIONAL. DEFAULT: True] if True - logging in stdout by loguru.logger
 
 Example:
 
 ```python
 import os
 from PyVkBot import Bot
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyVkBot-1.0.5/PyVkBot/Bot.py` & `pyvkbot-2.0.0.1/pyvkbot/Bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 class Bot:
     """
     Main class for working with vk bot
 
     :param token: VK access token
     :type token: str
 
-    :param main_chat: id of main chat for bot
-    :type main_chat: int
-
     :param group_id: id of your group
     :type group_id: int
 
+    :param main_chat: id of main chat for bot
+    :type main_chat: int
+
     :param logging: if True - logging in stdout by loguru.logger
     :type logging: bool
     """
 
-    def __init__(self, token: str, main_chat: int = None, group_id: int = None, logging: bool = True):
+    def __init__(self, token: str, group_id: int, main_chat: int = None, logging: bool = True):
         self.main_chat = main_chat
         self.vk_session = vk_api.VkApi(token=token)
         self.longpoll = VkBotLongPoll(self.vk_session, group_id=group_id)
 
         self.events = {
             EventTypes.MESSAGE: {},
             EventTypes.ACTION: {},
@@ -162,14 +162,15 @@
         """
         response = self.vk_session.method(method, payload)
         logger.debug(
             f"Sent api method '{method}'. "
             f"With payload {json.dumps(payload, ensure_ascii=False).encode('utf-8').decode()}. "
             f"Response: {json.dumps(response, ensure_ascii=False).encode('utf-8').decode()}"
         )
+        return response
 
     def send_message(self, peer_id: int, text: str, keyboard: Union[str, Keyboard] = None):
         """
         Sending message in chat
 
         :param peer_id: id of chat, where you want to send message
         :type peer_id: int
```

### Comparing `PyVkBot-1.0.5/PyVkBot/Types.py` & `pyvkbot-2.0.0.1/pyvkbot/Types.py`

 * *Files identical despite different names*

### Comparing `PyVkBot-1.0.5/PyVkBot.egg-info/PKG-INFO` & `pyvkbot-2.0.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: PyVkBot
-Version: 1.0.5
-Summary: Chat bot for vk.com
-Home-page: https://github.com/zeph1rrinc/pyvkbot
-Author: zeph1rr
-Author-email: grianton535@gmail.com
-License: MIT
-Requires-Python: >3.10
-Description-Content-Type: text/markdown
-
-﻿# PYVKBOT
+# PYVKBOT
 
 ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=black)
 
 [![tests&build](https://img.shields.io/github/workflow/status/zeph1rrinc/pyvkbot/tests/master?label=test%26build&logo=github&logoColor=white)](https://github.com/zeph1rrinc/pyvkbot/actions)
 [![LICENCE](https://img.shields.io/badge/License-MIT-yellow.svg?logo=ReadtheDocs&logoColor=white)](/LICENSE.md)
 [![Version](https://img.shields.io/pypi/v/pyvkbot?logo=pypi&logoColor=white)](https://pypi.org/project/PyVkBot/)
 
@@ -26,16 +15,16 @@
 ## Bot
 ### Methods
 ### init
 Creating instance for future working
 
 Params:
 - token: str - access token of your group
+- group_id: int - id of your group
 - main_chat: int - [OPTIONAL] main chat for bot
-- group_id: int - [OPTIONAL] id of your group
 - logging: bool - [OPTIONAL. DEFAULT: True] if True - logging in stdout by loguru.logger
 
 Example:
 
 ```python
 import os
 from PyVkBot import Bot
@@ -170,8 +159,8 @@
 # Simple one time vk keyboard
 one_time_keyboard = Keyboard(one_time=True)
 
 # Inline vk keyboard
 inline_keyboard = Keyboard(inline=True)
 ```
 
-All keyboard methods you can see in [doc](https://vk-api.readthedocs.io/en/latest/keyboard.html). Callback methods are not implemented.
+All keyboard methods you can see in [doc](https://vk-api.readthedocs.io/en/latest/keyboard.html). Callback methods are not implemented.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

