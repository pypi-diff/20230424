# Comparing `tmp/gpttui-0.4.0.tar.gz` & `tmp/gpttui-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpttui-0.4.0.tar", last modified: Mon Apr 24 21:23:49 2023, max compression
+gzip compressed data, was "gpttui-0.5.0.tar", last modified: Mon Apr 24 21:41:15 2023, max compression
```

## Comparing `gpttui-0.4.0.tar` & `gpttui-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.4.0/.gitignore
--rw-r--r--   0        0        0      185 2023-04-24 20:21:25.237725 gpttui-0.4.0/Makefile
--rw-r--r--   0        0        0     2164 2023-04-21 22:33:55.636511 gpttui-0.4.0/README.md
--rw-r--r--   0        0        0   999692 2023-04-21 22:33:55.649844 gpttui-0.4.0/docs/img/example.gif
--rw-r--r--   0        0        0      594 2023-04-24 21:23:45.239161 gpttui-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/database/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/database/base.py
--rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/database/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/models/__init__.py
--rw-r--r--   0        0        0     2027 2023-04-24 21:23:45.239161 gpttui-0.4.0/src/gpttui/models/base.py
--rw-r--r--   0        0        0     4447 2023-04-24 21:23:45.242494 gpttui-0.4.0/src/gpttui/models/chatsonic.py
--rw-r--r--   0        0        0     3783 2023-04-24 21:23:45.242494 gpttui-0.4.0/src/gpttui/models/openai.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/tui/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-21 22:33:55.649844 gpttui-0.4.0/src/gpttui/tui/app.py
--rw-r--r--   0        0        0     3271 2023-04-24 21:23:45.242494 gpttui-0.4.0/src/gpttui/tui/config.py
--rw-r--r--   0        0        0     2854 2023-04-24 21:23:45.245828 gpttui-0.4.0/src/gpttui/tui/front.py
--rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.4.0/src/gpttui/tui/main.py
--rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.4.0/test/main.sh
--rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.4.0/test/test_db.py
--rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.4.0/test/test_model.py
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 gpttui-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.5.0/.gitignore
+-rw-r--r--   0        0        0      185 2023-04-24 20:21:25.237725 gpttui-0.5.0/Makefile
+-rw-r--r--   0        0        0     2164 2023-04-21 22:33:55.636511 gpttui-0.5.0/README.md
+-rw-r--r--   0        0        0   999692 2023-04-21 22:33:55.649844 gpttui-0.5.0/docs/img/example.gif
+-rw-r--r--   0        0        0      594 2023-04-24 21:41:09.499816 gpttui-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/database/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/database/base.py
+-rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/database/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/models/__init__.py
+-rw-r--r--   0        0        0     2819 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/base.py
+-rw-r--r--   0        0        0     3728 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/chatsonic.py
+-rw-r--r--   0        0        0     4171 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/colossal.py
+-rw-r--r--   0        0        0     3054 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/openai.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/tui/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-21 22:33:55.649844 gpttui-0.5.0/src/gpttui/tui/app.py
+-rw-r--r--   0        0        0     3328 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/tui/config.py
+-rw-r--r--   0        0        0     3004 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/tui/front.py
+-rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.5.0/src/gpttui/tui/main.py
+-rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.5.0/test/main.sh
+-rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.5.0/test/test_db.py
+-rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.5.0/test/test_model.py
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 gpttui-0.5.0/PKG-INFO
```

### Comparing `gpttui-0.4.0/README.md` & `gpttui-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/docs/img/example.gif` & `gpttui-0.5.0/docs/img/example.gif`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/pyproject.toml` & `gpttui-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpttui"
-version = "0.4.0"
+version = "0.5.0"
 authors = [{name = "Juan Lara", email = "julara@unal.edu.co"}]
 description = "TUI to interact with gpt models."
 requires-python = ">3.8"
 dependencies = [
     "textual[dev]", "pydantic", "pyperclip"
 ]
```

### Comparing `gpttui-0.4.0/src/gpttui/database/base.py` & `gpttui-0.5.0/src/gpttui/database/base.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/src/gpttui/database/sqlite.py` & `gpttui-0.5.0/src/gpttui/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/src/gpttui/models/base.py` & `gpttui-0.5.0/src/gpttui/models/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 This module defines the general classes required to integrate different models.
 """
+import time
 from abc import ABC, abstractmethod
-
 from pydantic import BaseModel
-from gpttui.database.base import AbstractDB
+from gpttui.database.base import AbstractDB, Messages, Message, MessageWithTime
 from enum import Enum
 
 class ModelsEnum(Enum):
     """
     This enum defines the available models.
     """
     OPENAI = "OPENAI"
     CHATSONIC = "CHATSONIC"
+    COLOSSAL = "COLOSSAL"
 
 class AbstractModel(ABC):
     """
     This abstract class defines any generative model.
 
     Attributes
     ----------
@@ -47,14 +48,34 @@
         -------
         AbstractModel
             Instance of the model to use as a builder.
         """
         self.context = context
         return self
 
+    def last_messages(self) -> Messages:
+        """
+        Extracts the most recent messages from the database.
+
+        Returns
+        -------
+        Messages
+            Most recent messages.
+        """
+        self.database.create_session(session_name=self.session_name)
+        last_msgs = self.database.get_messages(session_name=self.session_name)
+        if not len(last_msgs.values):
+            msg = MessageWithTime(
+                    message=Message(role="system", content=self.context),
+                    timestamp=int(time.time())
+                    )
+            self.database.add_message(msg=msg, session_name=self.session_name)
+            return self.last_messages()
+        return last_msgs
+
     @abstractmethod
     def setup(self, config: BaseModel, session_name: str, database: AbstractDB) -> "AbstractModel":
         """
         This method is used to setup any model.
 
         Parameters
         ----------
```

### Comparing `gpttui-0.4.0/src/gpttui/models/chatsonic.py` & `gpttui-0.5.0/src/gpttui/models/chatsonic.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,34 +45,14 @@
             Instance of the model to be used as a builder.
         """
         self.config = config
         self.session_name = session_name
         self.database = database
         return self
 
-    def last_messages(self) -> Messages:
-        """
-        Extracts the most recent messages from the database.
-
-        Returns
-        -------
-        Messages
-            Most recent messages.
-        """
-        self.database.create_session(session_name=self.session_name)
-        last_msgs = self.database.get_messages(session_name=self.session_name)
-        if not len(last_msgs.values):
-            msg = MessageWithTime(
-                    message=Message(role="system", content=self.context),
-                    timestamp=int(time.time())
-                    )
-            self.database.add_message(msg=msg, session_name=self.session_name)
-            return self.last_messages()
-        return last_msgs
-
     @staticmethod
     def parse_messages(msgs: Messages) -> ChatSonicMessages:
         """
         This method parses general messages into chatsonic specific messages.
 
         Parameters
         ----------
```

### Comparing `gpttui-0.4.0/src/gpttui/models/openai.py` & `gpttui-0.5.0/src/gpttui/models/openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 try:
     import openai, time
     from openai.error import Timeout
 except ImportError:
     raise ImportError("Could not import openai library, please install it with:\n\tpip install gpttui[openai]")
 from pydantic import BaseModel
 from gpttui.models.base import AbstractModel
-from gpttui.database.base import AbstractDB, Messages, Message, MessageWithTime
+from gpttui.database.base import AbstractDB, Message, MessageWithTime
 
 class OpenAIConf(BaseModel):
     """
     Dataclass to setup OpenAI models.
     """
     timeout : int = 30
     max_retries : int = 3
@@ -47,34 +47,14 @@
         self.config = config
         self.session_name = session_name
         self.database = database
         openai.organization = config.organization
         openai.api_key = config.api_key
         return self
 
-    def last_messages(self) -> Messages:
-        """
-        Extracts the most recent messages from the database.
-
-        Returns
-        -------
-        Messages
-            Most recent messages.
-        """
-        self.database.create_session(session_name=self.session_name)
-        last_msgs = self.database.get_messages(session_name=self.session_name)
-        if not len(last_msgs.values):
-            msg = MessageWithTime(
-                    message=Message(role="system", content=self.context),
-                    timestamp=int(time.time())
-                    )
-            self.database.add_message(msg=msg, session_name=self.session_name)
-            return self.last_messages()
-        return last_msgs
-
     async def get_answer(self, message: str) -> str:
         """
         Obtains an answer form any message.
 
         Parameters
         ----------
         message : str
```

### Comparing `gpttui-0.4.0/src/gpttui/tui/app.py` & `gpttui-0.5.0/src/gpttui/tui/app.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/src/gpttui/tui/config.py` & `gpttui-0.5.0/src/gpttui/tui/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This file defines the main configuration options for the TUI.
 """
 import os
 from pathlib import Path
 from pydantic import BaseModel
 from typing import TypeVar, Type
+from gpttui.models.chatsonic import ChatSonicConf
+from gpttui.models.colossal import ColossalConf
 from gpttui.models.openai import OpenAIConf
 
-ConfT = TypeVar("ConfT", OpenAIConf, BaseModel)
-
 __CSS_CONFIG = """
 Prompt {
     dock: bottom;
     layout: horizontal;
     padding: 0;
     margin: 0;
 }
@@ -104,15 +104,15 @@
     """
     home_path = os.environ["HOME"]
     cfg_path = Path(os.path.join(home_path, ".config/gpttui"))
     if not cfg_path.exists():
         cfg_path.mkdir()
     return cfg_path
 
-def config_file(path: Path, type: Type[ConfT]) -> ConfT:
+def config_file(path: Path, type: Type[BaseModel]) -> BaseModel:
     """
     Setups the config file given any configuration type.
 
     Parameters
     ----------
     path : str
         Configuration path.
```

### Comparing `gpttui-0.4.0/src/gpttui/tui/front.py` & `gpttui-0.5.0/src/gpttui/tui/front.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from pathlib import Path
 from click import option, command
 from pydantic import BaseModel
 from gpttui.database.base import AbstractDB, DatabasesEnum
 from gpttui.database.sqlite import SqliteDB
 from gpttui.models.base import AbstractModel, ModelsEnum
 from gpttui.models.chatsonic import ChatSonicConf, ChatSonicModel
+from gpttui.models.colossal import ColossalConf, ColossalModel
 from gpttui.models.openai import OpenAIModel, OpenAIConf
 from gpttui.tui.app import GptApp
 from gpttui.tui.config import config_file
 from typing import Dict, Type
 
 DBS: Dict[DatabasesEnum, Type[AbstractDB]] = {
         DatabasesEnum.SQLITE: SqliteDB
         }
 MODELS: Dict[ModelsEnum, Type[AbstractModel]] = {
         ModelsEnum.OPENAI: OpenAIModel,
-        ModelsEnum.CHATSONIC: ChatSonicModel
+        ModelsEnum.CHATSONIC: ChatSonicModel,
+        ModelsEnum.COLOSSAL: ColossalModel
         }
 CONFS: Dict[ModelsEnum, Type[BaseModel]] = {
         ModelsEnum.OPENAI: OpenAIConf,
-        ModelsEnum.CHATSONIC: ChatSonicConf
+        ModelsEnum.CHATSONIC: ChatSonicConf,
+        ModelsEnum.COLOSSAL: ColossalConf
         }
 
 @command()
 @option(
     "--database_kind",
     type=DatabasesEnum,
     default=DatabasesEnum.SQLITE,
```

### Comparing `gpttui-0.4.0/test/test_db.py` & `gpttui-0.5.0/test/test_db.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/test/test_model.py` & `gpttui-0.5.0/test/test_model.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.4.0/PKG-INFO` & `gpttui-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpttui
-Version: 0.4.0
+Version: 0.5.0
 Summary: TUI to interact with gpt models.
 Author-email: Juan Lara <julara@unal.edu.co>
 Requires-Python: >3.8
 Requires-Dist: textual[dev]
 Requires-Dist: pydantic
 Requires-Dist: pyperclip
 Requires-Dist: httpx ; extra == "chatsonic"
```

