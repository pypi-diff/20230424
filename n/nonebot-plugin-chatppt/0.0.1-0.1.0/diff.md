# Comparing `tmp/nonebot_plugin_chatppt-0.0.1.tar.gz` & `tmp/nonebot_plugin_chatppt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chatppt-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_chatppt-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_chatppt-0.0.1.tar` & `nonebot_plugin_chatppt-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1742 2023-04-03 06:06:17.694939 nonebot_plugin_chatppt-0.0.1/README.md
--rw-r--r--   0        0        0     2603 2023-04-03 05:43:06.870365 nonebot_plugin_chatppt-0.0.1/nonebot_plugin_chatppt/__init__.py
--rw-r--r--   0        0        0      329 2023-04-03 04:12:32.473830 nonebot_plugin_chatppt-0.0.1/nonebot_plugin_chatppt/config.py
--rw-r--r--   0        0        0     7974 2023-04-03 05:38:49.124287 nonebot_plugin_chatppt-0.0.1/nonebot_plugin_chatppt/core.py
--rw-r--r--   0        0        0      593 2023-04-03 06:04:42.110335 nonebot_plugin_chatppt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2609 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.0.1/setup.py
--rw-r--r--   0        0        0     2531 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1918 2023-04-24 03:11:52.361828 nonebot_plugin_chatppt-0.1.0/README.md
+-rw-r--r--   0        0        0     6148 2023-04-24 03:08:30.860464 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/.DS_Store
+-rw-r--r--   0        0        0     3169 2023-04-24 02:42:56.609507 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-24 03:03:45.824081 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/config.py
+-rw-r--r--   0        0        0     7974 2023-04-24 03:03:45.824190 nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/core.py
+-rw-r--r--   0        0        0      593 2023-04-24 03:12:06.800026 nonebot_plugin_chatppt-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2789 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.1.0/setup.py
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 nonebot_plugin_chatppt-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_chatppt-0.0.1/README.md` & `nonebot_plugin_chatppt-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -43,29 +43,33 @@
 OPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 中国大陆/香港IP调用API请使用代理访问api,否则有几率会被封禁
 OPENAI_MODEL_NAME = "xxxxx"   # 使用的模型名称
 SLIDES_LIMIT = "xxxxx"   # 生成PPT页数的上限，不设置默认为10
 ```
 
 
 ## 使用方法
+- 配置PPT模版文件
 
-- 生成PPT
+ 在Bot目录下的data文件夹里面新建nonebot-plugin-chatppt/theme文件夹。把PPT主题模版文件放进里面，支持多文件。
+
+- 生成PPT命令
 ```
-chatppt 主题：XXXX，页数：XXXXX
+chatppt
 ```
-- 删除当前用户缓存文件
+- 删除当前用户缓存文件命令
 ```
 删除缓存PPT
 ```
-- 删除所有用户缓存文件
+- 删除所有用户缓存文件命令
 ```
 删除所有缓存PPT
 ```
 
 ## Todo
 
+- [x] 多模版支持
 - [ ] 优化生成内容
 - [ ] 完善插入图片功能
 
 ## 核心代码
 
 核心代码来源于：[Python-PPTX-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)
```

#### html2text {}

```diff
@@ -9,14 +9,17 @@
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-chatppt"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-chatppt ``` ##
 éç½®æä»¶ å¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼ ```
 OPENAI_API_KEY = key ``` å¯éåå®¹ï¼ ``` OPENAI_HTTP_PROXY = "http://
 127.0.0.1:8001" # ä¸­å½å¤§é/
 é¦æ¸¯IPè°ç¨APIè¯·ä½¿ç¨ä»£çè®¿é®api,å¦åæå çä¼è¢«å°ç¦
 OPENAI_MODEL_NAME = "xxxxx" # ä½¿ç¨çæ¨¡ååç§° SLIDES_LIMIT = "xxxxx" #
-çæPPTé¡µæ°çä¸éï¼ä¸è®¾ç½®é»è®¤ä¸º10 ``` ## ä½¿ç¨æ¹æ³ - çæPPT
-``` chatppt ä¸»é¢ï¼XXXXï¼é¡µæ°ï¼XXXXX ``` - å é¤å½åç¨æ·ç¼å­æä»¶
-``` å é¤ç¼å­PPT ``` - å é¤ææç¨æ·ç¼å­æä»¶ ```
-å é¤ææç¼å­PPT ``` ## Todo - [ ] ä¼åçæåå®¹ - [ ]
-å®åæå¥å¾çåè½ ## æ ¸å¿ä»£ç  æ ¸å¿ä»£ç æ¥æºäºï¼[Python-PPTX-
-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-
-ChatGPT-Presentation-Generator)
+çæPPTé¡µæ°çä¸éï¼ä¸è®¾ç½®é»è®¤ä¸º10 ``` ## ä½¿ç¨æ¹æ³ -
+éç½®PPTæ¨¡çæä»¶ å¨Botç®å½ä¸çdataæä»¶å¤¹éé¢æ°å»ºnonebot-
+plugin-chatppt/
+themeæä»¶å¤¹ãæPPTä¸»é¢æ¨¡çæä»¶æ¾è¿éé¢ï¼æ¯æå¤æä»¶ã -
+çæPPTå½ä»¤ ``` chatppt ``` - å é¤å½åç¨æ·ç¼å­æä»¶å½ä»¤ ```
+å é¤ç¼å­PPT ``` - å é¤ææç¨æ·ç¼å­æä»¶å½ä»¤ ```
+å é¤ææç¼å­PPT ``` ## Todo - [x] å¤æ¨¡çæ¯æ - [ ]
+ä¼åçæåå®¹ - [ ] å®åæå¥å¾çåè½ ## æ ¸å¿ä»£ç 
+æ ¸å¿ä»£ç æ¥æºäºï¼[Python-PPTX-ChatGPT-Presentation-Generator](https://
+github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)
```

### Comparing `nonebot_plugin_chatppt-0.0.1/nonebot_plugin_chatppt/__init__.py` & `nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import shutil
 from pathlib import Path
 
 import nonebot
-from nonebot import on_command, on_notice
-from nonebot.adapters.onebot.v11 import (Message, MessageSegment)
-from nonebot.adapters.onebot.v11 import MessageEvent, Bot, GroupMessageEvent, GroupUploadNoticeEvent
-from nonebot.params import CommandArg
+from nonebot import on_command
+from nonebot.adapters.onebot.v11 import MessageEvent, Bot
+from nonebot.adapters.onebot.v11 import (MessageSegment)
+from nonebot.params import ArgPlainText
 
 from .config import Config
 from .core import generate_ppt
 
 plugin_config = Config.parse_obj(nonebot.get_driver().config.dict())
 
 if not plugin_config.slides_limit:
@@ -21,15 +21,14 @@
 
 def delete_file(dir):
     if os.path.exists(dir):
         shutil.rmtree(dir)
 
 
 cache_folder = Path() / "data" / "nonebot-plugin-chatppt" / "caches"
-delete_file(cache_folder)
 
 delete_request = on_command("删除所有缓存PPT", block=True, priority=1)
 
 
 @delete_request.handle()
 async def _():
     delete_file(cache_folder)
@@ -45,33 +44,46 @@
     await delete_user_request.finish(MessageSegment.text("成功删除你在该群的缓存文件！"), at_sender=True)
 
 
 start_request = on_command("chatppt", block=True, priority=1)
 
 
 @start_request.handle()
-async def _(bot: Bot, event: MessageEvent, msg: Message = CommandArg()):
-    delete_file(os.path.join(cache_folder, event.get_session_id()))
+async def handle_function():
+    directory = './data/nonebot-plugin-chatppt/theme'
+    files_string = ''
+
+    for root, dirs, files in os.walk(directory):
+        for filename in files:
+            files_string += filename + '\n'
 
-    # if api_key == "":
-    #     await start_request.finish(MessageSegment.text("请先配置openai_api_key"), at_sender=True)
+    print(files_string)
+    await start_request.send(MessageSegment.text(f"当前可用PPT模版有:\n{files_string}"), at_sender=True)
 
-    content = msg.extract_plain_text()
 
+@start_request.got("content", prompt="请输入选择的PPT模版（需要带后缀名）、PPT主题、生成页数。示例：模版：xxxxxx，主题：xxxxx，页数：5")
+async def _(bot: Bot, event: MessageEvent, content: str = ArgPlainText()):
     if content == "" or content is None:
         await start_request.finish(MessageSegment.text("内容不能为空！"), at_sender=True)
 
-    topic = content.split("：")[1].split("，")[0]
-    length = content.split("：")[2]
-    if slides_limit < int(length):
+    theme = content.split("：")[1].split("，")[0]
+    topic = content.split("：")[2].split("，")[0]
+    length = content.split("：")[3].split("，")[0]
+    filepath = './data/nonebot-plugin-chatppt/theme/' + theme
+
+    if not os.path.exists(filepath):
+        await start_request.reject(f"PPT模版 {theme} 不存在，请重新输入！")
+
+    if int(slides_limit) < int(length):
         await start_request.finish(MessageSegment.text(f"生成的PPT不能超过{slides_limit}页！"), at_sender=True)
 
     await start_request.send(MessageSegment.text("生成中......."))
 
     try:
-        res = await generate_ppt(topic, length, event.get_session_id())
+        res = await generate_ppt(filepath, topic, length, event.get_session_id())
     except Exception as error:
         await start_request.finish(str(error), at_sender=True)
 
     await bot.upload_group_file(group_id=event.group_id,
                                 file=res,
                                 name=event.get_session_id() + topic + ".pptx")
+    start_request.finish("生成完成！", at_sender=True)
```

### Comparing `nonebot_plugin_chatppt-0.0.1/nonebot_plugin_chatppt/core.py` & `nonebot_plugin_chatppt-0.1.0/nonebot_plugin_chatppt/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatppt-0.0.1/pyproject.toml` & `nonebot_plugin_chatppt-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-chatppt"
-version = "0.0.1"
+version = "0.1.0"
 description = "A nonebot plugin for generating PPT slides from ChatGPT"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_chatppt-0.0.1/setup.py` & `nonebot_plugin_chatppt-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'openai>=0.27.1,<0.28.0',
  'python-pptx>=0.6.21,<0.7.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-chatppt',
-    'version': '0.0.1',
+    'version': '0.1.0',
     'description': 'A nonebot plugin for generating PPT slides from ChatGPT',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-chatppt\n</div>\n\n## 介绍\n- 本插件基于OpenAI的API开发，在nonebot框架下实现一个AI生成指定主题PPT的文件并上传到群文件中。\n\n![](demo.png)\n## 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot-plugin-chatppt.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-chatppt"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-chatppt\n  ```\n\n## 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n```\nOPENAI_API_KEY = key\n```\n\n可选内容：\n```\nOPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 中国大陆/香港IP调用API请使用代理访问api,否则有几率会被封禁\nOPENAI_MODEL_NAME = "xxxxx"   # 使用的模型名称\nSLIDES_LIMIT = "xxxxx"   # 生成PPT页数的上限，不设置默认为10\n```\n\n\n## 使用方法\n\n- 生成PPT\n```\nchatppt 主题：XXXX，页数：XXXXX\n```\n- 删除当前用户缓存文件\n```\n删除缓存PPT\n```\n- 删除所有用户缓存文件\n```\n删除所有缓存PPT\n```\n\n## Todo\n\n- [ ] 优化生成内容\n- [ ] 完善插入图片功能\n\n## 核心代码\n\n核心代码来源于：[Python-PPTX-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-chatppt\n</div>\n\n## 介绍\n- 本插件基于OpenAI的API开发，在nonebot框架下实现一个AI生成指定主题PPT的文件并上传到群文件中。\n\n![](demo.png)\n## 安装\n\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot-plugin-chatppt.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-chatppt"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-chatppt\n  ```\n\n## 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n```\nOPENAI_API_KEY = key\n```\n\n可选内容：\n```\nOPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 中国大陆/香港IP调用API请使用代理访问api,否则有几率会被封禁\nOPENAI_MODEL_NAME = "xxxxx"   # 使用的模型名称\nSLIDES_LIMIT = "xxxxx"   # 生成PPT页数的上限，不设置默认为10\n```\n\n\n## 使用方法\n- 配置PPT模版文件\n\n 在Bot目录下的data文件夹里面新建nonebot-plugin-chatppt/theme文件夹。把PPT主题模版文件放进里面，支持多文件。\n\n- 生成PPT命令\n```\nchatppt\n```\n- 删除当前用户缓存文件命令\n```\n删除缓存PPT\n```\n- 删除所有用户缓存文件命令\n```\n删除所有缓存PPT\n```\n\n## Todo\n\n- [x] 多模版支持\n- [ ] 优化生成内容\n- [ ] 完善插入图片功能\n\n## 核心代码\n\n核心代码来源于：[Python-PPTX-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_chatppt'] package_data = \ {'': ['*']} install_requires = \
 ['icrawler>=0.6.6,<0.7.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
 'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=0.27.1,<0.28.0', 'python-
 pptx>=0.6.21,<0.7.0'] setup_kwargs = { 'name': 'nonebot-plugin-chatppt',
-'version': '0.0.1', 'description': 'A nonebot plugin for generating PPT slides
+'version': '0.1.0', 'description': 'A nonebot plugin for generating PPT slides
 from ChatGPT', 'long_description': '
                            \n [NoneBotPluginLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
                         \n\n# nonebot-plugin-chatppt\n
@@ -20,18 +20,21 @@
 nonebot-plugin-chatppt"]\n ```\n* ä½¿ç¨ pip\n ```\n pip install nonebot-
 plugin-chatppt\n ```\n\n##
 éç½®æä»¶\n\nå¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼\n\n```\nOPENAI_API_KEY
 = key\n```\n\nå¯éåå®¹ï¼\n```\nOPENAI_HTTP_PROXY = "http://127.0.0.1:8001"
 # ä¸­å½å¤§é/
 é¦æ¸¯IPè°ç¨APIè¯·ä½¿ç¨ä»£çè®¿é®api,å¦åæå çä¼è¢«å°ç¦\nOPENAI_MODEL_NAME
 = "xxxxx" # ä½¿ç¨çæ¨¡ååç§°\nSLIDES_LIMIT = "xxxxx" #
-çæPPTé¡µæ°çä¸éï¼ä¸è®¾ç½®é»è®¤ä¸º10\n```\n\n\n## ä½¿ç¨æ¹æ³\n\n-
-çæPPT\n```\nchatppt ä¸»é¢ï¼XXXXï¼é¡µæ°ï¼XXXXX\n```\n-
-å é¤å½åç¨æ·ç¼å­æä»¶\n```\nå é¤ç¼å­PPT\n```\n-
-å é¤ææç¨æ·ç¼å­æä»¶\n```\nå é¤ææç¼å­PPT\n```\n\n## Todo\n\n-
-[ ] ä¼åçæåå®¹\n- [ ] å®åæå¥å¾çåè½\n\n##
-æ ¸å¿ä»£ç \n\næ ¸å¿ä»£ç æ¥æºäºï¼[Python-PPTX-ChatGPT-Presentation-
-Generator](https://github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-
-Generator)\n', 'author': 'Alpaca', 'author_email': 'alpaca@bupt.edu.cn',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+çæPPTé¡µæ°çä¸éï¼ä¸è®¾ç½®é»è®¤ä¸º10\n```\n\n\n## ä½¿ç¨æ¹æ³\n-
+éç½®PPTæ¨¡çæä»¶\n\n å¨Botç®å½ä¸çdataæä»¶å¤¹éé¢æ°å»ºnonebot-
+plugin-chatppt/
+themeæä»¶å¤¹ãæPPTä¸»é¢æ¨¡çæä»¶æ¾è¿éé¢ï¼æ¯æå¤æä»¶ã\n\n-
+çæPPTå½ä»¤\n```\nchatppt\n```\n-
+å é¤å½åç¨æ·ç¼å­æä»¶å½ä»¤\n```\nå é¤ç¼å­PPT\n```\n-
+å é¤ææç¨æ·ç¼å­æä»¶å½ä»¤\n```\nå é¤ææç¼å­PPT\n```\n\n##
+Todo\n\n- [x] å¤æ¨¡çæ¯æ\n- [ ] ä¼åçæåå®¹\n- [ ]
+å®åæå¥å¾çåè½\n\n## æ ¸å¿ä»£ç \n\næ ¸å¿ä»£ç æ¥æºäºï¼[Python-
+PPTX-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-
+PPTX-ChatGPT-Presentation-Generator)\n', 'author': 'Alpaca', 'author_email':
+'alpaca@bupt.edu.cn', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
+'None', 'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_chatppt-0.0.1/PKG-INFO` & `nonebot_plugin_chatppt-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatppt
-Version: 0.0.1
+Version: 0.1.0
 Summary: A nonebot plugin for generating PPT slides from ChatGPT
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,30 +64,34 @@
 OPENAI_HTTP_PROXY = "http://127.0.0.1:8001"    # 中国大陆/香港IP调用API请使用代理访问api,否则有几率会被封禁
 OPENAI_MODEL_NAME = "xxxxx"   # 使用的模型名称
 SLIDES_LIMIT = "xxxxx"   # 生成PPT页数的上限，不设置默认为10
 ```
 
 
 ## 使用方法
+- 配置PPT模版文件
 
-- 生成PPT
+ 在Bot目录下的data文件夹里面新建nonebot-plugin-chatppt/theme文件夹。把PPT主题模版文件放进里面，支持多文件。
+
+- 生成PPT命令
 ```
-chatppt 主题：XXXX，页数：XXXXX
+chatppt
 ```
-- 删除当前用户缓存文件
+- 删除当前用户缓存文件命令
 ```
 删除缓存PPT
 ```
-- 删除所有用户缓存文件
+- 删除所有用户缓存文件命令
 ```
 删除所有缓存PPT
 ```
 
 ## Todo
 
+- [x] 多模版支持
 - [ ] 优化生成内容
 - [ ] 完善插入图片功能
 
 ## 核心代码
 
 核心代码来源于：[Python-PPTX-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatppt Version: 0.0.1 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-chatppt Version: 0.1.0 Summary: A
 nonebot plugin for generating PPT slides from ChatGPT License: MIT Author:
 Alpaca Author-email: alpaca@bupt.edu.cn Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: icrawler (>=0.6.6,<0.7.0) Requires-Dist: nonebot-adapter-onebot
@@ -20,14 +20,17 @@
 plugin_dirs = ["xxxxxx","xxxxxx",......,"ä¸è½½å®æçæä»¶è·¯å¾/nonebot-
 plugin-chatppt"] ``` * ä½¿ç¨ pip ``` pip install nonebot-plugin-chatppt ``` ##
 éç½®æä»¶ å¨Botæ ¹ç®å½ä¸ç.envæä»¶ä¸­è¿½å å¦ä¸åå®¹ï¼ ```
 OPENAI_API_KEY = key ``` å¯éåå®¹ï¼ ``` OPENAI_HTTP_PROXY = "http://
 127.0.0.1:8001" # ä¸­å½å¤§é/
 é¦æ¸¯IPè°ç¨APIè¯·ä½¿ç¨ä»£çè®¿é®api,å¦åæå çä¼è¢«å°ç¦
 OPENAI_MODEL_NAME = "xxxxx" # ä½¿ç¨çæ¨¡ååç§° SLIDES_LIMIT = "xxxxx" #
-çæPPTé¡µæ°çä¸éï¼ä¸è®¾ç½®é»è®¤ä¸º10 ``` ## ä½¿ç¨æ¹æ³ - çæPPT
-``` chatppt ä¸»é¢ï¼XXXXï¼é¡µæ°ï¼XXXXX ``` - å é¤å½åç¨æ·ç¼å­æä»¶
-``` å é¤ç¼å­PPT ``` - å é¤ææç¨æ·ç¼å­æä»¶ ```
-å é¤ææç¼å­PPT ``` ## Todo - [ ] ä¼åçæåå®¹ - [ ]
-å®åæå¥å¾çåè½ ## æ ¸å¿ä»£ç  æ ¸å¿ä»£ç æ¥æºäºï¼[Python-PPTX-
-ChatGPT-Presentation-Generator](https://github.com/AmNotAGoose/Python-PPTX-
-ChatGPT-Presentation-Generator)
+çæPPTé¡µæ°çä¸éï¼ä¸è®¾ç½®é»è®¤ä¸º10 ``` ## ä½¿ç¨æ¹æ³ -
+éç½®PPTæ¨¡çæä»¶ å¨Botç®å½ä¸çdataæä»¶å¤¹éé¢æ°å»ºnonebot-
+plugin-chatppt/
+themeæä»¶å¤¹ãæPPTä¸»é¢æ¨¡çæä»¶æ¾è¿éé¢ï¼æ¯æå¤æä»¶ã -
+çæPPTå½ä»¤ ``` chatppt ``` - å é¤å½åç¨æ·ç¼å­æä»¶å½ä»¤ ```
+å é¤ç¼å­PPT ``` - å é¤ææç¨æ·ç¼å­æä»¶å½ä»¤ ```
+å é¤ææç¼å­PPT ``` ## Todo - [x] å¤æ¨¡çæ¯æ - [ ]
+ä¼åçæåå®¹ - [ ] å®åæå¥å¾çåè½ ## æ ¸å¿ä»£ç 
+æ ¸å¿ä»£ç æ¥æºäºï¼[Python-PPTX-ChatGPT-Presentation-Generator](https://
+github.com/AmNotAGoose/Python-PPTX-ChatGPT-Presentation-Generator)
```

