# Comparing `tmp/nonebug-0.3.2.tar.gz` & `tmp/nonebug-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebug-0.3.2.tar", max compression
+gzip compressed data, was "nonebug-0.3.3.tar", max compression
```

## Comparing `nonebug-0.3.2.tar` & `nonebug-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-03-31 11:18:43.774163 nonebug-0.3.2/LICENSE
--rw-r--r--   0        0        0     1673 2023-03-31 11:18:43.774163 nonebug-0.3.2/README.md
--rw-r--r--   0        0        0      137 2023-03-31 11:18:43.774163 nonebug-0.3.2/nonebug/__init__.py
--rw-r--r--   0        0        0      153 2023-03-31 11:18:43.774163 nonebug-0.3.2/nonebug/app.py
--rw-r--r--   0        0        0     1176 2023-03-31 11:18:43.774163 nonebug-0.3.2/nonebug/base.py
--rw-r--r--   0        0        0      706 2023-03-31 11:18:43.774163 nonebug-0.3.2/nonebug/fixture.py
--rw-r--r--   0        0        0      204 2023-03-31 11:18:43.774163 nonebug-0.3.2/nonebug/mixin/__init__.py
--rw-r--r--   0        0        0     6467 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/call_api/__init__.py
--rw-r--r--   0        0        0     1242 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/call_api/fake.py
--rw-r--r--   0        0        0      517 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/call_api/model.py
--rw-r--r--   0        0        0     1903 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/dependent.py
--rw-r--r--   0        0        0     1315 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/driver.py
--rw-r--r--   0        0        0    11098 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/process/__init__.py
--rw-r--r--   0        0        0     2783 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/process/fake.py
--rw-r--r--   0        0        0     1330 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/mixin/process/model.py
--rw-r--r--   0        0        0     2930 2023-03-31 11:18:43.778163 nonebug-0.3.2/nonebug/provider.py
--rw-r--r--   0        0        0     1838 2023-03-31 11:18:43.778163 nonebug-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 nonebug-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-24 08:05:01.258998 nonebug-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1673 2023-04-24 08:05:01.258998 nonebug-0.3.3/README.md
+-rw-r--r--   0        0        0      137 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/app.py
+-rw-r--r--   0        0        0     1176 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/base.py
+-rw-r--r--   0        0        0      706 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/fixture.py
+-rw-r--r--   0        0        0      204 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/__init__.py
+-rw-r--r--   0        0        0     7404 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/call_api/__init__.py
+-rw-r--r--   0        0        0     1738 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/call_api/fake.py
+-rw-r--r--   0        0        0      517 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/call_api/model.py
+-rw-r--r--   0        0        0     1903 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/dependent.py
+-rw-r--r--   0        0        0     1315 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/driver.py
+-rw-r--r--   0        0        0    11098 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/process/__init__.py
+-rw-r--r--   0        0        0     2783 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/process/fake.py
+-rw-r--r--   0        0        0     1330 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/process/model.py
+-rw-r--r--   0        0        0     2930 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/provider.py
+-rw-r--r--   0        0        0     1838 2023-04-24 08:05:01.262999 nonebug-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 nonebug-0.3.3/PKG-INFO
```

### Comparing `nonebug-0.3.2/LICENSE` & `nonebug-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/README.md` & `nonebug-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/base.py` & `nonebug-0.3.3/nonebug/base.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/fixture.py` & `nonebug-0.3.3/nonebug/fixture.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/mixin/call_api/__init__.py` & `nonebug-0.3.3/nonebug/mixin/call_api/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 import contextlib
 from queue import Queue
-from typing import TYPE_CHECKING, Any, Set, Dict, Type, Union, Optional
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Set,
+    Dict,
+    Type,
+    Union,
+    TypeVar,
+    Optional,
+    overload,
+)
 
 import pytest
 
 from nonebug.base import BaseApp, Context
 
 from .model import Api, Send, Model
 from .fake import make_fake_bot, make_fake_adapter
 
 if TYPE_CHECKING:
     from nonebot.adapters import Bot, Event, Adapter, Message, MessageSegment
 
+A = TypeVar("A", bound="Adapter")
+B = TypeVar("B", bound="Bot")
+
 
 class ApiContext(Context):
     """API testing context.
 
     This context is used to test the api calling behavior of the bot.
     You may inherit this class to make api testing available in other context.
 
@@ -34,33 +47,75 @@
 
     def _connect_bot(self, bot: "Bot") -> None:
         from nonebot import get_driver
 
         get_driver()._bot_connect(bot)
         self.connected_bot.add(bot)
 
+    @overload
     def create_adapter(
         self,
         *,
-        base: Optional[Type["Adapter"]] = None,
+        base: None = None,
         **kwargs: Any,
     ) -> "Adapter":
+        ...
+
+    @overload
+    def create_adapter(
+        self,
+        *,
+        base: Optional[Type[A]] = None,
+        **kwargs: Any,
+    ) -> A:
+        ...
+
+    def create_adapter(
+        self,
+        *,
+        base: Optional[Type[A]] = None,
+        **kwargs: Any,
+    ) -> Union[A, "Adapter"]:
         from nonebot import get_driver
 
         return make_fake_adapter(self, base=base)(get_driver(), **kwargs)
 
+    @overload
     def create_bot(
         self,
         *,
-        base: Optional[Type["Bot"]] = None,
+        base: None = None,
         adapter: Optional["Adapter"] = None,
         self_id: str = "test",
         auto_connect: bool = True,
         **kwargs: Any,
     ) -> "Bot":
+        ...
+
+    @overload
+    def create_bot(
+        self,
+        *,
+        base: Optional[Type[B]] = None,
+        adapter: Optional["Adapter"] = None,
+        self_id: str = "test",
+        auto_connect: bool = True,
+        **kwargs: Any,
+    ) -> B:
+        ...
+
+    def create_bot(
+        self,
+        *,
+        base: Optional[Type[B]] = None,
+        adapter: Optional["Adapter"] = None,
+        self_id: str = "test",
+        auto_connect: bool = True,
+        **kwargs: Any,
+    ) -> Union[B, "Bot"]:
         adapter = adapter or self.create_adapter()
         bot = make_fake_bot(self, base=base)(adapter, self_id, **kwargs)
         if auto_connect:
             self._connect_bot(bot)
         return bot
 
     def patch_adapter(
```

### Comparing `nonebug-0.3.2/nonebug/mixin/call_api/fake.py` & `nonebug-0.3.3/nonebug/mixin/call_api/fake.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,68 @@
-from typing import TYPE_CHECKING, Any, Type, Union, Optional
+from typing import TYPE_CHECKING, Any, Type, Union, TypeVar, Optional, overload
 
 if TYPE_CHECKING:
     from nonebot.adapters import Bot, Event, Adapter, Message, MessageSegment
 
     from . import ApiContext
 
+A = TypeVar("A", bound=Type["Adapter"])
+B = TypeVar("B", bound=Type["Bot"])
+
+
+@overload
+def make_fake_adapter(ctx: "ApiContext", base: None = None) -> Type["Adapter"]:
+    ...
+
+
+@overload
+def make_fake_adapter(ctx: "ApiContext", base: A) -> A:
+    ...
+
 
 # fake class should be created every init
-def make_fake_adapter(ctx: "ApiContext", base: Optional[Type["Adapter"]] = None):
+def make_fake_adapter(
+    ctx: "ApiContext", base: Optional[A] = None
+) -> Union[A, Type["Adapter"]]:
     from nonebot.adapters import Adapter
     from nonebot.typing import overrides
 
-    base = base or Adapter
+    _base = base or Adapter
 
-    class FakeAdapter(base):
+    class FakeAdapter(_base):  # type: ignore
         @classmethod
-        @overrides(base)
+        @overrides(_base)
         def get_name(cls) -> str:
             return "fake"
 
-        @overrides(base)
+        @overrides(_base)
         async def _call_api(self, bot: "Bot", api: str, **data) -> Any:
             return ctx.got_call_api(self, api, **data)
 
     return FakeAdapter
 
 
-def make_fake_bot(ctx: "ApiContext", base: Optional[Type["Bot"]] = None) -> Type["Bot"]:
+@overload
+def make_fake_bot(ctx: "ApiContext", base: None = None) -> Type["Bot"]:
+    ...
+
+
+@overload
+def make_fake_bot(ctx: "ApiContext", base: B) -> B:
+    ...
+
+
+def make_fake_bot(ctx: "ApiContext", base: Optional[B] = None) -> Union[B, Type["Bot"]]:
     from nonebot.adapters import Bot
     from nonebot.typing import overrides
 
-    base = base or Bot
+    _base = base or Bot
 
-    class FakeBot(base):
-        @overrides(base)
+    class FakeBot(_base):  # type: ignore
+        @overrides(_base)
         async def send(
             self,
             event: "Event",
             message: Union[str, "Message", "MessageSegment"],
             **kwargs,
         ) -> Any:
             return ctx.got_call_send(self, event, message, **kwargs)
```

### Comparing `nonebug-0.3.2/nonebug/mixin/call_api/model.py` & `nonebug-0.3.3/nonebug/mixin/call_api/model.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/mixin/dependent.py` & `nonebug-0.3.3/nonebug/mixin/dependent.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/mixin/driver.py` & `nonebug-0.3.3/nonebug/mixin/driver.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/mixin/process/__init__.py` & `nonebug-0.3.3/nonebug/mixin/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/mixin/process/fake.py` & `nonebug-0.3.3/nonebug/mixin/process/fake.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/mixin/process/model.py` & `nonebug-0.3.3/nonebug/mixin/process/model.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/nonebug/provider.py` & `nonebug-0.3.3/nonebug/provider.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.2/pyproject.toml` & `nonebug-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebug"
-version = "0.3.2"
+version = "0.3.3"
 description = "nonebot2 test framework"
 authors = ["AkiraXie <l997460364@outlook.com>", "yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://v2.nonebot.dev/"
 repository = "https://github.com/nonebot/nonebug"
 documentation = "https://v2.nonebot.dev/"
@@ -24,15 +24,15 @@
 black = "^23.1.0"
 nonemoji = "^0.1.3"
 pre-commit = "^3.0.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
-pytest-asyncio = "^0.20.0"
+pytest-asyncio = "^0.21.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", extras = ["fastapi"] }
 
 [tool.poetry.plugins.pytest11]
 nonebug = "nonebug.fixture"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
```

### Comparing `nonebug-0.3.2/PKG-INFO` & `nonebug-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebug
-Version: 0.3.2
+Version: 0.3.3
 Summary: nonebot2 test framework
 Home-page: https://v2.nonebot.dev/
 License: MIT
 Keywords: nonebot,pytest,test,bot,onebot,cqhttp
 Author: AkiraXie
 Author-email: l997460364@outlook.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebug Version: 0.3.2 Summary: nonebot2 test
+Metadata-Version: 2.1 Name: nonebug Version: 0.3.3 Summary: nonebot2 test
 framework Home-page: https://v2.nonebot.dev/ License: MIT Keywords:
 nonebot,pytest,test,bot,onebot,cqhttp Author: AkiraXie Author-email:
 l997460364@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Framework ::
 Pytest Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

