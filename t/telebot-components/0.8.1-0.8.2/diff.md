# Comparing `tmp/telebot_components-0.8.1.tar.gz` & `tmp/telebot_components-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_components-0.8.1.tar", max compression
+gzip compressed data, was "telebot_components-0.8.2.tar", max compression
```

## Comparing `telebot_components-0.8.1.tar` & `telebot_components-0.8.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35148 2023-04-23 21:57:54.755277 telebot_components-0.8.1/LICENSE
--rw-r--r--   0        0        0     2258 2023-04-23 21:57:54.755277 telebot_components-0.8.1/README.md
--rw-r--r--   0        0        0     1573 2023-04-23 21:58:33.356112 telebot_components-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/__init__.py
--rw-r--r--   0        0        0    13083 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/broadcast/__init__.py
--rw-r--r--   0        0        0     2835 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/broadcast/message_senders.py
--rw-r--r--   0        0        0      159 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/broadcast/subscriber.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/constants/__init__.py
--rw-r--r--   0        0        0    15212 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/constants/emoji.py
--rw-r--r--   0        0        0      168 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/constants/times.py
--rw-r--r--   0        0        0    50213 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/anti_spam.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/__init__.py
--rw-r--r--   0        0        0     8255 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/aux_feedback_handler.py
--rw-r--r--   0        0        0     3983 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/interface.py
--rw-r--r--   0        0        0    34435 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/integration/trello.py
--rw-r--r--   0        0        0      237 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/trello_integration.py
--rw-r--r--   0        0        0      493 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/feedback/types.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/__init__.py
--rw-r--r--   0        0        0    29347 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/field.py
--rw-r--r--   0        0        0    14757 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/form.py
--rw-r--r--   0        0        0    20318 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/handler.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.755277 telebot_components-0.8.1/telebot_components/form/helpers/__init__.py
--rw-r--r--   0        0        0     7572 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/form/helpers/calendar_keyboard.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/menu/__init__.py
--rw-r--r--   0        0        0    11976 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/menu/menu.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/py.typed
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/redis_utils/__init__.py
--rw-r--r--   0        0        0    10640 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/redis_utils/emulation.py
--rw-r--r--   0        0        0     6078 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/redis_utils/interface.py
--rw-r--r--   0        0        0        0 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/banned_users.py
--rw-r--r--   0        0        0     8229 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/category.py
--rw-r--r--   0        0        0     9203 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/forum_topics.py
--rw-r--r--   0        0        0     9845 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/generic.py
--rw-r--r--   0        0        0     8066 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/language.py
--rw-r--r--   0        0        0      397 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/types.py
--rw-r--r--   0        0        0     3914 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/user_group.py
--rw-r--r--   0        0        0      614 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/stores/utils.py
--rw-r--r--   0        0        0     8134 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/__init__.py
--rw-r--r--   0        0        0     5136 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/airtable.py
--rw-r--r--   0        0        0     2564 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/alerts.py
--rw-r--r--   0        0        0     1257 2023-04-23 21:57:54.759277 telebot_components-0.8.1/telebot_components/utils/strings.py
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-23 22:23:19.746289 telebot_components-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2258 2023-04-23 22:23:19.746289 telebot_components-0.8.2/README.md
+-rw-r--r--   0        0        0     1573 2023-04-23 22:24:06.466675 telebot_components-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/__init__.py
+-rw-r--r--   0        0        0    13083 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/broadcast/__init__.py
+-rw-r--r--   0        0        0     2835 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/broadcast/message_senders.py
+-rw-r--r--   0        0        0      159 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/broadcast/subscriber.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/constants/__init__.py
+-rw-r--r--   0        0        0    15212 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/constants/emoji.py
+-rw-r--r--   0        0        0      168 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/constants/times.py
+-rw-r--r--   0        0        0    50213 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/__init__.py
+-rw-r--r--   0        0        0     2075 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/anti_spam.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/integration/__init__.py
+-rw-r--r--   0        0        0     8255 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/integration/aux_feedback_handler.py
+-rw-r--r--   0        0        0     3983 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/integration/interface.py
+-rw-r--r--   0        0        0    34435 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/integration/trello.py
+-rw-r--r--   0        0        0      237 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/trello_integration.py
+-rw-r--r--   0        0        0      493 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/feedback/types.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/form/__init__.py
+-rw-r--r--   0        0        0    29347 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/form/field.py
+-rw-r--r--   0        0        0    14757 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/form/form.py
+-rw-r--r--   0        0        0    20318 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/form/handler.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/form/helpers/__init__.py
+-rw-r--r--   0        0        0     7572 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/form/helpers/calendar_keyboard.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/menu/__init__.py
+-rw-r--r--   0        0        0    11976 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/menu/menu.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/py.typed
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/redis_utils/__init__.py
+-rw-r--r--   0        0        0    10640 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/redis_utils/emulation.py
+-rw-r--r--   0        0        0     6078 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/redis_utils/interface.py
+-rw-r--r--   0        0        0        0 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/banned_users.py
+-rw-r--r--   0        0        0     8229 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/category.py
+-rw-r--r--   0        0        0     9306 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/forum_topics.py
+-rw-r--r--   0        0        0     9845 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/generic.py
+-rw-r--r--   0        0        0     8066 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/language.py
+-rw-r--r--   0        0        0      397 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/types.py
+-rw-r--r--   0        0        0     3914 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/user_group.py
+-rw-r--r--   0        0        0      614 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/stores/utils.py
+-rw-r--r--   0        0        0     8134 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/utils/__init__.py
+-rw-r--r--   0        0        0     5136 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/utils/airtable.py
+-rw-r--r--   0        0        0     2564 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/utils/alerts.py
+-rw-r--r--   0        0        0     1257 2023-04-23 22:23:19.750289 telebot_components-0.8.2/telebot_components/utils/strings.py
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 telebot_components-0.8.2/PKG-INFO
```

### Comparing `telebot_components-0.8.1/LICENSE` & `telebot_components-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/README.md` & `telebot_components-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/pyproject.toml` & `telebot_components-0.8.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telebot-components"
-version = "0.8.1"
+version = "0.8.2"
 description = "Framework/toolkit for building Telegram bots with telebot and redis"
 authors = ["Igor Vaiman <gosha.vaiman@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/bots-against-war/telebot-components"
 packages = [{include = "telebot_components"}]
 [tool.poetry.group.dev.dependencies]
```

### Comparing `telebot_components-0.8.1/telebot_components/broadcast/__init__.py` & `telebot_components-0.8.2/telebot_components/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/broadcast/message_senders.py` & `telebot_components-0.8.2/telebot_components/broadcast/message_senders.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/constants/emoji.py` & `telebot_components-0.8.2/telebot_components/constants/emoji.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/feedback/__init__.py` & `telebot_components-0.8.2/telebot_components/feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/feedback/anti_spam.py` & `telebot_components-0.8.2/telebot_components/feedback/anti_spam.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/feedback/integration/aux_feedback_handler.py` & `telebot_components-0.8.2/telebot_components/feedback/integration/aux_feedback_handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/feedback/integration/interface.py` & `telebot_components-0.8.2/telebot_components/feedback/integration/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/feedback/integration/trello.py` & `telebot_components-0.8.2/telebot_components/feedback/integration/trello.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/form/field.py` & `telebot_components-0.8.2/telebot_components/form/field.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/form/form.py` & `telebot_components-0.8.2/telebot_components/form/form.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/form/handler.py` & `telebot_components-0.8.2/telebot_components/form/handler.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/form/helpers/calendar_keyboard.py` & `telebot_components-0.8.2/telebot_components/form/helpers/calendar_keyboard.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/menu/menu.py` & `telebot_components-0.8.2/telebot_components/menu/menu.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/redis_utils/emulation.py` & `telebot_components-0.8.2/telebot_components/redis_utils/emulation.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/redis_utils/interface.py` & `telebot_components-0.8.2/telebot_components/redis_utils/interface.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/stores/banned_users.py` & `telebot_components-0.8.2/telebot_components/stores/banned_users.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/stores/category.py` & `telebot_components-0.8.2/telebot_components/stores/category.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/stores/forum_topics.py` & `telebot_components-0.8.2/telebot_components/stores/forum_topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,16 @@
             try:
                 for (topic_spec, default_color) in zip(self.topics, itertools.cycle(ForumTopicIconColor)):
                     existing_message_thread_id = await self.message_thread_id_by_topic.get_subkey(
                         self.admin_chat_id, topic_spec.id
                     )
                     if existing_message_thread_id is not None:
                         self.logger.info(
-                            f"Found saved message thread id for {topic_spec}, validating and syncing state"
+                            f"Found saved message thread id for {topic_spec}: "
+                            + f"{existing_message_thread_id}, trying to sync state"
                         )
                         success = False
                         try:
                             success = await self.bot.edit_forum_topic(
                                 chat_id=self.admin_chat_id,
                                 message_thread_id=existing_message_thread_id,
                                 name=topic_spec.name,
@@ -141,15 +142,16 @@
                         except ApiHTTPException as e:
                             if "TOPIC_NOT_MODIFIED" in e.error_description:
                                 success = True
                             else:
                                 self.logger.exception("Unexpected error syncing topic")
 
                         if success:
-                            self.logger.info(f"Forum topic synced: {topic_spec}")
+                            self.logger.info(f"Forum topic OK: {topic_spec}")
+                            await asyncio.sleep(5)
                             continue
                         else:
                             self.logger.info(f"Failed to sync {topic_spec}, will create new one")
 
                     self.logger.info(f"Creating new forum topic for {topic_spec}")
                     created_topic = await self.bot.create_forum_topic(
                         chat_id=self.admin_chat_id,
```

### Comparing `telebot_components-0.8.1/telebot_components/stores/generic.py` & `telebot_components-0.8.2/telebot_components/stores/generic.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/stores/language.py` & `telebot_components-0.8.2/telebot_components/stores/language.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/stores/user_group.py` & `telebot_components-0.8.2/telebot_components/stores/user_group.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/stores/utils.py` & `telebot_components-0.8.2/telebot_components/stores/utils.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/utils/__init__.py` & `telebot_components-0.8.2/telebot_components/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/utils/airtable.py` & `telebot_components-0.8.2/telebot_components/utils/airtable.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/utils/alerts.py` & `telebot_components-0.8.2/telebot_components/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/telebot_components/utils/strings.py` & `telebot_components-0.8.2/telebot_components/utils/strings.py`

 * *Files identical despite different names*

### Comparing `telebot_components-0.8.1/PKG-INFO` & `telebot_components-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebot-components
-Version: 0.8.1
+Version: 0.8.2
 Summary: Framework/toolkit for building Telegram bots with telebot and redis
 Home-page: https://github.com/bots-against-war/telebot-components
 License: GPLv3
 Author: Igor Vaiman
 Author-email: gosha.vaiman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

