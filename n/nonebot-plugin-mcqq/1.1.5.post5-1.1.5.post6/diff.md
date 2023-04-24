# Comparing `tmp/nonebot-plugin-mcqq-1.1.5.post5.tar.gz` & `tmp/nonebot-plugin-mcqq-1.1.5.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post5.tar", last modified: Sun Apr 23 10:04:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post6.tar", last modified: Mon Apr 24 08:39:17 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.1.5.post5.tar` & `nonebot-plugin-mcqq-1.1.5.post6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:04:49.023323 nonebot-plugin-mcqq-1.1.5.post5/
--rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post5/LICENSE
--rw-rw-rw-   0        0        0     3004 2023-04-23 10:04:49.023323 nonebot-plugin-mcqq-1.1.5.post5/PKG-INFO
--rw-rw-rw-   0        0        0     2503 2023-04-23 10:04:21.000000 nonebot-plugin-mcqq-1.1.5.post5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 10:04:49.018319 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/
--rw-rw-rw-   0        0        0     1786 2023-04-23 07:24:20.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/__init__.py
--rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/data_source.py
--rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:04:49.022321 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/
--rw-rw-rw-   0        0        0     3004 2023-04-23 10:04:48.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-23 10:04:49.000000 nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 10:04:49.023323 nonebot-plugin-mcqq-1.1.5.post5/setup.cfg
--rw-rw-rw-   0        0        0     1244 2023-04-23 10:03:54.000000 nonebot-plugin-mcqq-1.1.5.post5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:39:17.881507 nonebot-plugin-mcqq-1.1.5.post6/
+-rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post6/LICENSE
+-rw-rw-rw-   0        0        0     3004 2023-04-24 08:39:17.881507 nonebot-plugin-mcqq-1.1.5.post6/PKG-INFO
+-rw-rw-rw-   0        0        0     2503 2023-04-23 10:04:21.000000 nonebot-plugin-mcqq-1.1.5.post6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:39:17.872924 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/
+-rw-rw-rw-   0        0        0     1746 2023-04-23 16:18:39.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/__init__.py
+-rw-rw-rw-   0        0        0     2847 2023-04-23 06:12:28.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/data_source.py
+-rw-rw-rw-   0        0        0     1024 2023-04-22 05:52:16.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:39:17.879931 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/
+-rw-rw-rw-   0        0        0     3004 2023-04-24 08:39:17.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-04-24 08:39:17.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:39:17.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-04-24 08:39:17.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-24 08:39:17.000000 nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:39:17.881507 nonebot-plugin-mcqq-1.1.5.post6/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2023-04-24 08:38:31.000000 nonebot-plugin-mcqq-1.1.5.post6/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/LICENSE` & `nonebot-plugin-mcqq-1.1.5.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post5
+Version: 1.1.5.post6
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/README.md` & `nonebot-plugin-mcqq-1.1.5.post6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Union
 
-from mcqq_tool import GUILD_ADMIN
+from mcqq_tool.common import GUILD_ADMIN
+from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
 from nonebot import on_message, on_command, get_driver
 from nonebot.adapters import Message
-from nonebot.exception import FinishedException
 from nonebot.params import CommandArg
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP_ADMIN, GROUP_OWNER
 from nonebot.permission import SUPERUSER
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, GROUP_ADMIN, GROUP_OWNER
 from nonebot_plugin_guild_patch import GuildMessageEvent
-from mcqq_tool.utils import send_msg_to_mc, send_cmd_to_mc
+
 from .data_source import start_ws_server, stop_ws_server
 from .utils import msg_rule
 
 mc_qq = on_message(priority=2, rule=msg_rule)
 
 mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post6/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.5.post5
+Version: 1.1.5.post6
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.1.5.post5/setup.py` & `nonebot-plugin-mcqq-1.1.5.post6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.5-post5",  # 程序版本
+    version="1.1.5-post6",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

