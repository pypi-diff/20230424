# Comparing `tmp/nonebot_plugin_datastore-0.6.2.tar.gz` & `tmp/nonebot_plugin_datastore-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_datastore-0.6.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_datastore-0.6.3.tar", max compression
```

## Comparing `nonebot_plugin_datastore-0.6.2.tar` & `nonebot_plugin_datastore-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/LICENSE
--rw-r--r--   0        0        0     7564 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/README.md
--rw-r--r--   0        0        0      259 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/__init__.py
--rw-r--r--   0        0        0     1772 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/config.py
--rw-r--r--   0        0        0     3597 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/db.py
--rw-r--r--   0        0        0      804 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py
--rw-r--r--   0        0        0     8844 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/plugin.py
--rw-r--r--   0        0        0     1487 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/__init__.py
--rw-r--r--   0        0        0     1226 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/database.py
--rw-r--r--   0        0        0     1530 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/json.py
--rw-r--r--   0        0        0     1635 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/toml.py
--rw-r--r--   0        0        0     1816 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/yaml.py
--rw-r--r--   0        0        0        0 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/py.typed
--rw-r--r--   0        0        0        0 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/__init__.py
--rw-r--r--   0        0        0     6755 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/cli.py
--rw-r--r--   0        0        0    12170 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/command.py
--rw-r--r--   0        0        0      510 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/migration/script.py.mako
--rw-r--r--   0        0        0     3921 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/utils.py
--rw-r--r--   0        0        0     1889 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/utils.py
--rw-r--r--   0        0        0     2074 2023-04-01 15:33:53.084289 nonebot_plugin_datastore-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     9023 1970-01-01 00:00:00.000000 nonebot_plugin_datastore-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/LICENSE
+-rw-r--r--   0        0        0     7564 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/README.md
+-rw-r--r--   0        0        0      259 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/__init__.py
+-rw-r--r--   0        0        0     1772 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/config.py
+-rw-r--r--   0        0        0     4093 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/db.py
+-rw-r--r--   0        0        0      804 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py
+-rw-r--r--   0        0        0     8844 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/plugin.py
+-rw-r--r--   0        0        0     1487 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/__init__.py
+-rw-r--r--   0        0        0     1226 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/database.py
+-rw-r--r--   0        0        0     1530 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/json.py
+-rw-r--r--   0        0        0     1635 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/toml.py
+-rw-r--r--   0        0        0     1816 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/yaml.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/py.typed
+-rw-r--r--   0        0        0        0 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/__init__.py
+-rw-r--r--   0        0        0     6372 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/cli.py
+-rw-r--r--   0        0        0    12170 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/command.py
+-rw-r--r--   0        0        0      510 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/migration/script.py.mako
+-rw-r--r--   0        0        0     3611 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/utils.py
+-rw-r--r--   0        0        0     1889 2023-04-24 14:44:07.039758 nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/utils.py
+-rw-r--r--   0        0        0     2085 2023-04-24 14:44:07.043758 nonebot_plugin_datastore-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     8994 1970-01-01 00:00:00.000000 nonebot_plugin_datastore-0.6.3/PKG-INFO
```

### Comparing `nonebot_plugin_datastore-0.6.2/LICENSE` & `nonebot_plugin_datastore-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/README.md` & `nonebot_plugin_datastore-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/config.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/db.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """ 数据库 """
-import asyncio
 from pathlib import Path
 from typing import TYPE_CHECKING, AsyncGenerator, Callable, Dict, List
 
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot.utils import is_coroutine_callable, run_sync
 from sqlalchemy.engine import make_url
@@ -62,45 +61,59 @@
 
 def post_db_init(func: Callable) -> Callable:
     """数据库初始化后执行的函数"""
     _post_db_init_funcs.append(func)
     return func
 
 
+async def run_funcs(funcs: List[Callable]) -> None:
+    """运行所有函数"""
+    for func in funcs:
+        if is_coroutine_callable(func):
+            await func()
+        else:
+            await run_sync(func)()
+
+
+async def run_pre_db_init_funcs(plugin: str) -> None:
+    """运行数据库初始化前执行的函数"""
+    funcs = _pre_db_init_funcs.get(plugin, [])
+    if funcs:
+        logger.debug(f"运行插件 {plugin} 的数据库初始化前执行的函数")
+        await run_funcs(funcs)
+
+
+async def run_post_db_init_funcs() -> None:
+    """运行数据库初始化后执行的函数"""
+    if _post_db_init_funcs:
+        logger.debug("运行数据库初始化后执行的函数")
+        await run_funcs(_post_db_init_funcs)
+
+
 async def init_db():
     """初始化数据库"""
-    from .script.utils import run_upgrade
-
-    # 执行数据库初始化前执行的函数
-    pre_db_init_funcs = [i for funcs in _pre_db_init_funcs.values() for i in funcs]
-    cors = [
-        func() if is_coroutine_callable(func) else run_sync(func)()
-        for func in pre_db_init_funcs
-    ]
-    if cors:
-        try:
-            await asyncio.gather(*cors)
-        except Exception as e:
-            logger.error("数据库初始化前执行的函数出错")
-            raise
+    from .script.command import upgrade
+    from .script.utils import Config, get_plugins
 
-    await run_upgrade()
+    plugins = get_plugins()
+    for plugin in plugins:
+        # 执行数据库初始化前执行的函数
+        await run_pre_db_init_funcs(plugin)
+        # 初始化数据库，升级到最新版本
+        logger.debug(f"初始化插件 {plugin} 的数据库")
+        config = Config(plugin)
+        await upgrade(config, "head")
 
     logger.info("数据库初始化完成")
 
     # 执行数据库初始化后执行的函数
-    cors = [
-        func() if is_coroutine_callable(func) else run_sync(func)()
-        for func in _post_db_init_funcs
-    ]
-    if cors:
-        try:
-            await asyncio.gather(*cors)
-        except Exception as e:
-            logger.error(f"数据库初始化后执行的函数出错: {e}")
+    try:
+        await run_post_db_init_funcs()
+    except Exception as e:
+        logger.error(f"数据库初始化后执行的函数出错: {e}")
 
 
 if plugin_config.datastore_enable_database:
     _engine = _make_engine()
     get_driver().on_startup(init_db)
```

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/plugin.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/__init__.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/database.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/database.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/json.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/toml.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/toml.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/providers/yaml.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/providers/yaml.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/cli.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-import asyncio
-from argparse import Namespace
-from functools import partial, wraps
-from typing import Any, Callable, Coroutine, Optional, TypeVar
-
-from nonebot.log import logger
-from nonebot.utils import is_coroutine_callable
-
 try:
     import anyio
     import click
     from typing_extensions import ParamSpec
 except ImportError as e:  # pragma: no cover
     raise ImportError("请使用 `pip install nonebot-plugin-datastore[cli]` 安装所需依赖") from e
 
+from argparse import Namespace
+from functools import partial, wraps
+from typing import Any, Callable, Coroutine, Optional, TypeVar
+
+from nonebot.log import logger
 
 from ..config import plugin_config
-from ..db import _pre_db_init_funcs
+from ..db import run_pre_db_init_funcs
 from ..plugin import PluginData
 from . import command
 from .utils import Config, get_plugins
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
@@ -86,24 +83,15 @@
 @run_async
 async def upgrade(name: Optional[str], revision: str):
     """升级数据库版本"""
     # 执行数据库初始化前执行的函数
     # 比如 bison 需要在迁移之前把 alembic_version 表重命名
     plugins = get_plugins(name)
     for plugin in plugins:
-        cors = [
-            func() if is_coroutine_callable(func) else run_sync(func)()
-            for func in _pre_db_init_funcs.get(plugin, [])
-        ]
-        if cors:
-            try:
-                await asyncio.gather(*cors)
-            except Exception as e:
-                click.echo("数据库初始化前执行的函数出错")
-                raise
+        await run_pre_db_init_funcs(plugin)
         logger.info(f"升级插件 {plugin} 的数据库")
         config = Config(plugin)
         await command.upgrade(config, revision)
 
 
 @cli.command()
 @click.option("--name", "-n", default=None, help="插件名")
```

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/command.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/script/utils.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/script/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,19 +103,7 @@
 
 async def run_migration(plugin_name: Optional[str] = None):
     """运行迁移"""
     connectable = get_engine()
 
     async with connectable.connect() as connection:
         await connection.run_sync(do_run_migrations, plugin_name)
-
-
-async def run_upgrade():
-    """初始化数据库"""
-    from .command import upgrade
-
-    plugins = get_plugins()
-    for plugin in plugins:
-        logger.debug(f"初始化插件 {plugin} 的数据库")
-        config = Config(plugin)
-        # 升级到最新版本
-        await upgrade(config, "head")
```

### Comparing `nonebot_plugin_datastore-0.6.2/nonebot_plugin_datastore/utils.py` & `nonebot_plugin_datastore-0.6.3/nonebot_plugin_datastore/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-0.6.2/pyproject.toml` & `nonebot_plugin_datastore-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-datastore"
-version = "0.6.2"
+version = "0.6.3"
 description = "适用于 Nonebot2 的数据存储插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-datastore"
 repository = "https://github.com/he0119/nonebot-plugin-datastore"
 documentation = "https://github.com/he0119/nonebot-plugin-datastore#readme"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = { extras = ["httpx"], version = "^2.0.0-rc.1" }
 nonebot-plugin-localstore = ">=0.2.0,!=0.3.0,!=0.4.0,<0.5.0"
-sqlalchemy = "^2.0.3"
-aiosqlite = ">=0.17,<0.19"
+sqlalchemy = { extras = ["aiosqlite"], version = "^2.0.0" }
 alembic = "^1.9.1"
 
 anyio = { version = ">=3.6", optional = true }
 click = { version = ">=8.0", optional = true }
 typing-extensions = { version = ">=4.4", optional = true }
 rtoml = { version = "^0.9.0", optional = true }
 pyyaml = { version = "^6.0", optional = true }
```

### Comparing `nonebot_plugin_datastore-0.6.2/PKG-INFO` & `nonebot_plugin_datastore-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-datastore
-Version: 0.6.2
+Version: 0.6.3
 Summary: 适用于 Nonebot2 的数据存储插件
 Home-page: https://github.com/he0119/nonebot-plugin-datastore
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,23 +13,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: toml
 Provides-Extra: yaml
-Requires-Dist: aiosqlite (>=0.17,<0.19)
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: anyio (>=3.6) ; extra == "cli" or extra == "all"
 Requires-Dist: click (>=8.0) ; extra == "cli" or extra == "all"
 Requires-Dist: nonebot-plugin-localstore (>=0.2.0,!=0.3.0,!=0.4.0,<0.5.0)
 Requires-Dist: nonebot2[httpx] (>=2.0.0-rc.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml" or extra == "all"
 Requires-Dist: rtoml (>=0.9.0,<0.10.0) ; extra == "toml" or extra == "all"
-Requires-Dist: sqlalchemy (>=2.0.3,<3.0.0)
+Requires-Dist: sqlalchemy[aiosqlite] (>=2.0.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4) ; extra == "cli" or extra == "all"
 Project-URL: Documentation, https://github.com/he0119/nonebot-plugin-datastore#readme
 Project-URL: Repository, https://github.com/he0119/nonebot-plugin-datastore
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
```

