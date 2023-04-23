# Comparing `tmp/telebot_components-0.8.0.tar.gz` & `tmp/telebot_components-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.0.tar", max compression
+gzip compressed data, was "telebot_components-0.8.1.tar", max compression
```

## Comparing `telebot_components-0.8.0.tar` & `telebot_components-0.8.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-04-20 21:06:42.150375 telebot_components-0.8.0/LICENSE
--rw-r--r--   0        0        0     2258 2023-04-20 21:06:42.150375 telebot_components-0.8.0/README.md
--rw-r--r--   0        0        0     1573 2023-04-20 21:07:29.130652 telebot_components-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/constants/times.py
--rw-r--r--   0        0        0    50122 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8255 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    29347 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/field.py
--rw-r--r--   0        0        0    14757 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    11976 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-04-20 21:06:42.154375 telebot_components-0.8.0/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6078 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/category.py
--rw-r--r--   0        0        0     8786 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8066 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8134 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5136 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-04-20 21:06:42.158375 telebot_components-0.8.0/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-23 21:57:54.755277 telebot_components-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2258 2023-04-23 21:57:54.755277 telebot_components-0.8.1/README.md
+-rw-r--r--   0        0        0     1573 2023-04-23 21:58:33.356112 telebot_components-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    50213 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8255 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    29347 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/field.py
+-rw-r--r--   0        0        0    14757 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    11976 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9203 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8066 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8134 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5136 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.1/PKG-INFO
```

### Comparing `telebot_components-0.8.0/LICENSE` & `telebot_components-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/README.md` & `telebot_components-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/pyproject.toml` & `telebot_components-0.8.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.0"
+version = "0.8.1"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
 [tool.poetry.group.dev.dependencies]
```

### Comparing `telebot_components-0.8.0/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.1/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.1/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/constants/emoji.py` & `telebot_components-0.8.1/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/feedback/__init__.py` & `telebot_components-0.8.1/telebot_components/feedback/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,18 +636,19 @@
         method can be used in such cases.
 
         If the message has been successfully sent to the admin chat, this method returns its id.
         """
 
         async def message_forwarder(message_thread_id: Optional[int]) -> MessageForwarderResult:
             if attachment is None:
+                if "message_thread_id" not in send_message_kwargs:
+                    send_message_kwargs["message_thread_id"] = message_thread_id
                 sent_msg = await bot.send_message(
                     self.admin_chat_id,
                     text=text,
-                    message_thread_id=message_thread_id,
                     **send_message_kwargs,
                 )
             else:
                 sent_msg = await send_attachment(
                     bot,
                     self.admin_chat_id,
                     attachment,
```

### Comparing `telebot_components-0.8.0/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.1/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.1/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.1/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.1/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/form/field.py` & `telebot_components-0.8.1/telebot_components/form/field.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/form/form.py` & `telebot_components-0.8.1/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/form/handler.py` & `telebot_components-0.8.1/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.1/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/menu/menu.py` & `telebot_components-0.8.1/telebot_components/menu/menu.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.1/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.1/telebot_components/redis_utils/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/stores/banned_users.py` & `telebot_components-0.8.1/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/stores/category.py` & `telebot_components-0.8.1/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/stores/forum_topics.py` & `telebot_components-0.8.1/telebot_components/stores/forum_topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional
 
 from async_lru import alru_cache
 from telebot import AsyncTeleBot
+from telebot.api import ApiHTTPException
 
 from telebot_components.redis_utils.interface import RedisInterface
 from telebot_components.stores.category import Category
 from telebot_components.stores.generic import KeyDictStore
 
 
 @dataclass
@@ -125,25 +126,33 @@
                     existing_message_thread_id = await self.message_thread_id_by_topic.get_subkey(
                         self.admin_chat_id, topic_spec.id
                     )
                     if existing_message_thread_id is not None:
                         self.logger.info(
                             f"Found saved message thread id for {topic_spec}, validating and syncing state"
                         )
-                        success = await self.bot.edit_forum_topic(
-                            chat_id=self.admin_chat_id,
-                            message_thread_id=existing_message_thread_id,
-                            name=topic_spec.name,
-                            icon_custom_emoji_id=topic_spec.icon_custom_emoji_id,
-                        )
+                        success = False
+                        try:
+                            success = await self.bot.edit_forum_topic(
+                                chat_id=self.admin_chat_id,
+                                message_thread_id=existing_message_thread_id,
+                                name=topic_spec.name,
+                                icon_custom_emoji_id=topic_spec.icon_custom_emoji_id,
+                            )
+                        except ApiHTTPException as e:
+                            if "TOPIC_NOT_MODIFIED" in e.error_description:
+                                success = True
+                            else:
+                                self.logger.exception("Unexpected error syncing topic")
+
                         if success:
-                            self.logger.info(f"Forum topic updated for {topic_spec}")
+                            self.logger.info(f"Forum topic synced: {topic_spec}")
                             continue
                         else:
-                            self.logger.info(f"Forum topic not updated for {topic_spec}, will create new one")
+                            self.logger.info(f"Failed to sync {topic_spec}, will create new one")
 
                     self.logger.info(f"Creating new forum topic for {topic_spec}")
                     created_topic = await self.bot.create_forum_topic(
                         chat_id=self.admin_chat_id,
                         name=topic_spec.name,
                         icon_color=(topic_spec.icon_color or default_color).value,
                         icon_custom_emoji_id=topic_spec.icon_custom_emoji_id,
```

### Comparing `telebot_components-0.8.0/telebot_components/stores/generic.py` & `telebot_components-0.8.1/telebot_components/stores/generic.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/stores/language.py` & `telebot_components-0.8.1/telebot_components/stores/language.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/stores/user_group.py` & `telebot_components-0.8.1/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/stores/utils.py` & `telebot_components-0.8.1/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/utils/__init__.py` & `telebot_components-0.8.1/telebot_components/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/utils/airtable.py` & `telebot_components-0.8.1/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/utils/alerts.py` & `telebot_components-0.8.1/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/telebot_components/utils/strings.py` & `telebot_components-0.8.1/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.0/PKG-INFO` & `telebot_components-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.0
+Version: 0.8.1
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

