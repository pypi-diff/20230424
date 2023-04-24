# Comparing `tmp/aiogram-ext-0.1.6.tar.gz` & `tmp/aiogram-ext-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.1.6.tar", last modified: Mon Apr 24 02:44:07 2023, max compression
+gzip compressed data, was "aiogram-ext-0.1.7.tar", last modified: Mon Apr 24 03:10:26 2023, max compression
```

## Comparing `aiogram-ext-0.1.6.tar` & `aiogram-ext-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1022 2023-04-24 02:44:04.825894 aiogram-ext-0.1.6/botty/__init__.py
--rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.6/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.6/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.6/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.6/botty/context.py
--rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.6/botty/deps.py
--rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.6/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.6/botty/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.6/botty/filters.py
--rw-r--r--   0        0        0      892 2023-04-24 02:43:07.706213 aiogram-ext-0.1.6/botty/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.6/botty/keyboards.py
--rw-r--r--   0        0        0      641 2023-04-24 02:27:10.075207 aiogram-ext-0.1.6/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.6/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.6/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.6/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.6/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.6/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      455 2023-04-24 02:44:04.842949 aiogram-ext-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.6/README.md
--rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.6/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-24 02:44:04.825894 aiogram-ext-0.1.7/botty/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.7/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.7/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.7/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.7/botty/context.py
+-rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.7/botty/deps.py
+-rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.7/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.7/botty/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.7/botty/filters.py
+-rw-r--r--   0        0        0      892 2023-04-24 02:43:07.706213 aiogram-ext-0.1.7/botty/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.7/botty/keyboards.py
+-rw-r--r--   0        0        0      669 2023-04-24 03:10:12.100277 aiogram-ext-0.1.7/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.7/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.7/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.7/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.7/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.7/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      455 2023-04-24 03:10:23.712589 aiogram-ext-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.7/README.md
+-rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.7/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.7/PKG-INFO
```

### Comparing `aiogram-ext-0.1.6/botty/__init__.py` & `aiogram-ext-0.1.7/botty/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/buttons.py` & `aiogram-ext-0.1.7/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/context.py` & `aiogram-ext-0.1.7/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/deps.py` & `aiogram-ext-0.1.7/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/dispatcher.py` & `aiogram-ext-0.1.7/botty/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/env.py` & `aiogram-ext-0.1.7/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/filters.py` & `aiogram-ext-0.1.7/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/helpers.py` & `aiogram-ext-0.1.7/botty/helpers.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/keyboards.py` & `aiogram-ext-0.1.7/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/loader.py` & `aiogram-ext-0.1.7/botty/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     db_name=MONGO.DB,
     host=MONGO.HOST,
     username=MONGO.USER,
     password=MONGO.PASSWORD,
 )
 
 dp = Dispatcher(bot, storage=storage)
+Dispatcher.set_current(dp)
 logger = logging.getLogger()
 
 
 @dp.errors_handler()
 async def _(update: Update, error: Exception):
     logger.exception(f"{error=} on {update=}")
     return True
```

### Comparing `aiogram-ext-0.1.6/botty/middlewares/_conversation.py` & `aiogram-ext-0.1.7/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/middlewares/_membership.py` & `aiogram-ext-0.1.7/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/middlewares/misc.py` & `aiogram-ext-0.1.7/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.6/botty/middlewares/throttling.py` & `aiogram-ext-0.1.7/botty/middlewares/throttling.py`

 * *Files identical despite different names*

