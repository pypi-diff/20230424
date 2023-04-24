# Comparing `tmp/aiogram-ext-0.1.5.tar.gz` & `tmp/aiogram-ext-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.1.5.tar", last modified: Mon Apr 24 02:42:38 2023, max compression
+gzip compressed data, was "aiogram-ext-0.1.6.tar", last modified: Mon Apr 24 02:44:07 2023, max compression
```

## Comparing `aiogram-ext-0.1.5.tar` & `aiogram-ext-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1005 2023-04-24 02:27:10.112437 aiogram-ext-0.1.5/botty/__init__.py
--rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.5/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.5/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.5/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.5/botty/context.py
--rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.5/botty/deps.py
--rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.5/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.5/botty/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.5/botty/filters.py
--rw-r--r--   0        0        0      920 2023-04-24 02:42:34.728268 aiogram-ext-0.1.5/botty/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.5/botty/keyboards.py
--rw-r--r--   0        0        0      641 2023-04-24 02:27:10.075207 aiogram-ext-0.1.5/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.5/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.5/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.5/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.5/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.5/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      455 2023-04-24 02:42:34.736067 aiogram-ext-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.5/README.md
--rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.5/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-24 02:44:04.825894 aiogram-ext-0.1.6/botty/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.6/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.6/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.6/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.6/botty/context.py
+-rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.6/botty/deps.py
+-rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.6/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.6/botty/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.6/botty/filters.py
+-rw-r--r--   0        0        0      892 2023-04-24 02:43:07.706213 aiogram-ext-0.1.6/botty/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.6/botty/keyboards.py
+-rw-r--r--   0        0        0      641 2023-04-24 02:27:10.075207 aiogram-ext-0.1.6/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.6/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.6/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.6/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.6/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.6/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      455 2023-04-24 02:44:04.842949 aiogram-ext-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.6/README.md
+-rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.6/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.6/PKG-INFO
```

### Comparing `aiogram-ext-0.1.5/botty/__init__.py` & `aiogram-ext-0.1.6/botty/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     StatesGroup,
     SkipHandler,
     CancelHandler,
     TelegramAPIError,
 )
 from .dispatcher import Dispatcher
 from .env import env
-from .helpers import reply, is_group, is_private, is_channel
+from .helpers import reply, is_group, is_private, is_channel, ask
 from .keyboards import ReplyKeyboard, InlineKeyboard
 from .loader import bot, dp, logger, app, run
 
 __all__ = [
     "Dispatcher",
     "ReplyKeyboard",
     "InlineKeyboard",
@@ -44,8 +44,9 @@
     "CancelHandler",
     "TelegramAPIError",
     "is_private",
     "is_group",
     "is_channel",
     "app",
     "run",
+    "ask",
 ]
```

### Comparing `aiogram-ext-0.1.5/botty/buttons.py` & `aiogram-ext-0.1.6/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/context.py` & `aiogram-ext-0.1.6/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/deps.py` & `aiogram-ext-0.1.6/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/dispatcher.py` & `aiogram-ext-0.1.6/botty/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/env.py` & `aiogram-ext-0.1.6/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/filters.py` & `aiogram-ext-0.1.6/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/helpers.py` & `aiogram-ext-0.1.6/botty/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from aiogram.types import ChatType
 
 from .deps import ReplyKeyboardRemove, Message, ReplyMarkup, Query, Chat, State
 
 
 def reply(
-        msg: Message | Query,
-        text: str,
-        markup: ReplyMarkup | bool = None,
+    msg: Message | Query,
+    text: str,
+    markup: ReplyMarkup | bool = None,
 ) -> Awaitable[Message]:
     if isinstance(msg, Query):
         msg = msg.message
     if markup is False:
         markup = ReplyKeyboardRemove()
     return msg.answer(text, reply_markup=markup)
 
 
 async def ask(
-        state: State,
-        msg: Message,
-        text: str,
-        markup: ReplyMarkup = None,
+    state: State,
+    msg: Message,
+    text: str,
+    markup: ReplyMarkup = None,
 ):
     await state.set()
     await reply(msg, text, markup)
 
 
 def is_channel(chat: Chat) -> bool:
     return chat.type in [ChatType.CHANNEL]
```

### Comparing `aiogram-ext-0.1.5/botty/keyboards.py` & `aiogram-ext-0.1.6/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/loader.py` & `aiogram-ext-0.1.6/botty/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/middlewares/_conversation.py` & `aiogram-ext-0.1.6/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/middlewares/_membership.py` & `aiogram-ext-0.1.6/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/middlewares/misc.py` & `aiogram-ext-0.1.6/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.5/botty/middlewares/throttling.py` & `aiogram-ext-0.1.6/botty/middlewares/throttling.py`

 * *Files identical despite different names*

