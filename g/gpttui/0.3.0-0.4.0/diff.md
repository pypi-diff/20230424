# Comparing `tmp/gpttui-0.3.0.tar.gz` & `tmp/gpttui-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpttui-0.3.0.tar", last modified: Fri Apr 21 22:34:14 2023, max compression
+gzip compressed data, was "gpttui-0.4.0.tar", last modified: Mon Apr 24 21:23:49 2023, max compression
```

## Comparing `gpttui-0.3.0.tar` & `gpttui-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.3.0/.gitignore
--rw-r--r--   0        0        0      176 2023-04-11 01:50:25.100205 gpttui-0.3.0/Makefile
--rw-r--r--   0        0        0     2164 2023-04-21 22:33:55.636511 gpttui-0.3.0/README.md
--rw-r--r--   0        0        0   999692 2023-04-21 22:33:55.649844 gpttui-0.3.0/docs/img/example.gif
--rw-r--r--   0        0        0      531 2023-04-21 22:33:55.649844 gpttui-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/database/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/database/base.py
--rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/database/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/models/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-21 22:33:55.649844 gpttui-0.3.0/src/gpttui/models/base.py
--rw-r--r--   0        0        0     3377 2023-04-21 22:33:55.649844 gpttui-0.3.0/src/gpttui/models/openai.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.3.0/src/gpttui/tui/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-21 22:33:55.649844 gpttui-0.3.0/src/gpttui/tui/app.py
--rw-r--r--   0        0        0     2644 2023-04-21 22:14:51.392110 gpttui-0.3.0/src/gpttui/tui/config.py
--rw-r--r--   0        0        0     2391 2023-04-11 01:50:25.103539 gpttui-0.3.0/src/gpttui/tui/front.py
--rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.3.0/src/gpttui/tui/main.py
--rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.3.0/test/main.sh
--rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.3.0/test/test_db.py
--rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.3.0/test/test_model.py
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 gpttui-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.4.0/.gitignore
+-rw-r--r--   0        0        0      185 2023-04-24 20:21:25.237725 gpttui-0.4.0/Makefile
+-rw-r--r--   0        0        0     2164 2023-04-21 22:33:55.636511 gpttui-0.4.0/README.md
+-rw-r--r--   0        0        0   999692 2023-04-21 22:33:55.649844 gpttui-0.4.0/docs/img/example.gif
+-rw-r--r--   0        0        0      594 2023-04-24 21:23:45.239161 gpttui-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/database/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/database/base.py
+-rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/database/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/models/__init__.py
+-rw-r--r--   0        0        0     2027 2023-04-24 21:23:45.239161 gpttui-0.4.0/src/gpttui/models/base.py
+-rw-r--r--   0        0        0     4447 2023-04-24 21:23:45.242494 gpttui-0.4.0/src/gpttui/models/chatsonic.py
+-rw-r--r--   0        0        0     3783 2023-04-24 21:23:45.242494 gpttui-0.4.0/src/gpttui/models/openai.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.4.0/src/gpttui/tui/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-21 22:33:55.649844 gpttui-0.4.0/src/gpttui/tui/app.py
+-rw-r--r--   0        0        0     3271 2023-04-24 21:23:45.242494 gpttui-0.4.0/src/gpttui/tui/config.py
+-rw-r--r--   0        0        0     2854 2023-04-24 21:23:45.245828 gpttui-0.4.0/src/gpttui/tui/front.py
+-rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.4.0/src/gpttui/tui/main.py
+-rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.4.0/test/main.sh
+-rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.4.0/test/test_db.py
+-rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.4.0/test/test_model.py
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 gpttui-0.4.0/PKG-INFO
```

### Comparing `gpttui-0.3.0/README.md` & `gpttui-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gpttui-0.3.0/docs/img/example.gif` & `gpttui-0.4.0/docs/img/example.gif`

 * *Files identical despite different names*

### Comparing `gpttui-0.3.0/src/gpttui/database/base.py` & `gpttui-0.4.0/src/gpttui/database/base.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.3.0/src/gpttui/database/sqlite.py` & `gpttui-0.4.0/src/gpttui/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.3.0/src/gpttui/models/base.py` & `gpttui-0.4.0/src/gpttui/models/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 This module defines the general classes required to integrate different models.
 """
 from abc import ABC, abstractmethod
+
+from pydantic import BaseModel
 from gpttui.database.base import AbstractDB
-from typing import Any
 from enum import Enum
 
 class ModelsEnum(Enum):
     """
     This enum defines the available models.
     """
     OPENAI = "OPENAI"
+    CHATSONIC = "CHATSONIC"
 
 class AbstractModel(ABC):
     """
     This abstract class defines any generative model.
 
     Attributes
     ----------
@@ -23,15 +25,15 @@
     session_name : str
         Session name.
     context : str
         Context given to the model.
     database : AbstractDB
         Database to store the messages.
     """
-    model_name: str
+    config: BaseModel
     session_name: str
     context: str
     database: AbstractDB
 
     def add_context(self, context: str) -> "AbstractModel":
         """
         Sets the context.
@@ -46,24 +48,26 @@
         AbstractModel
             Instance of the model to use as a builder.
         """
         self.context = context
         return self
 
     @abstractmethod
-    def setup(self, *args: Any, **kwargs: Any) -> "AbstractModel":
+    def setup(self, config: BaseModel, session_name: str, database: AbstractDB) -> "AbstractModel":
         """
         This method is used to setup any model.
 
         Parameters
         ----------
-        args : Any
-            Any positional argument.
-        kwargs : Any
-            Any keyword argument.
+        config : BaseModel
+            Dataclass with the model's config options.
+        session_name : str
+            Session name.
+        database : AbstractDB
+            Database to store the messages.
 
         Returns
         -------
         AbstractModel
             Instance of the model to use as a builder.
         """
         ...
```

### Comparing `gpttui-0.3.0/src/gpttui/models/openai.py` & `gpttui-0.4.0/src/gpttui/models/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 """
 This module contains the integration with OpenAI models.
 """
-import openai, os, time
-from openai.error import Timeout
+try:
+    import openai, time
+    from openai.error import Timeout
+except ImportError:
+    raise ImportError("Could not import openai library, please install it with:\n\tpip install gpttui[openai]")
+from pydantic import BaseModel
 from gpttui.models.base import AbstractModel
-from gpttui.database.base import Messages, Message, MessageWithTime
-from typing import Any
+from gpttui.database.base import AbstractDB, Messages, Message, MessageWithTime
+
+class OpenAIConf(BaseModel):
+    """
+    Dataclass to setup OpenAI models.
+    """
+    timeout : int = 30
+    max_retries : int = 3
+    model_name : str = "gpt-3.5-turbo"
+    organization : str = ""
+    api_key : str = ""
 
 class OpenAIModel(AbstractModel):
     """
     This class allows loading and interacting with any openai model through its API.
     """
-    timeout = 0
-    max_retries = 3
+    config : OpenAIConf
 
-    def setup(self, **kwargs: Any) -> "OpenAIModel":
+    def setup(self, config: OpenAIConf, session_name: str, database: AbstractDB) -> "OpenAIModel":
         """
         Initializes the model and collects credentials for OpenAI.
 
         Parameters
         ----------
         model_name : str
             Model name.
@@ -28,19 +40,19 @@
             Database to store the messages.
 
         Returns
         -------
         OpenAIModel
             Instance of the model to be used as a builder.
         """
-        self.model_name = kwargs["model_name"]
-        self.session_name = kwargs["session_name"]
-        self.database = kwargs["database"]
-        openai.organization = os.getenv("OPENAI_ORG")
-        openai.api_key = os.getenv("OPENAI_API_KEY")
+        self.config = config
+        self.session_name = session_name
+        self.database = database
+        openai.organization = config.organization
+        openai.api_key = config.api_key
         return self
 
     def last_messages(self) -> Messages:
         """
         Extracts the most recent messages from the database.
 
         Returns
@@ -78,25 +90,25 @@
                 message=Message(role="user", content=message),
                 timestamp=int(time.time())
                 )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         last_msgs = self.last_messages()
         response = ""
         retries = 0
-        while not response and retries < self.max_retries:
+        while not response and retries < self.config.max_retries:
             try:
                 response = await openai.ChatCompletion.acreate(
-                            model = self.model_name,
+                            model = self.config.model_name,
                             messages = last_msgs.dict()["values"],
-                            request_timeout = self.timeout
+                            request_timeout = self.config.timeout
                             )
             except Timeout:
                 retries += 1
-        response = str(response.choices[0].message.content) # type: ignore
-        if retries == 3:
+        if retries == self.config.max_retries:
             raise Timeout("Maximum number of retries achieved.")
+        response = str(response.choices[0].message.content) # type: ignore
         new_msg = MessageWithTime(
                 message=Message(role="assistant", content=response),
                 timestamp=int(time.time())
                 )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         return response
```

### Comparing `gpttui-0.3.0/src/gpttui/tui/app.py` & `gpttui-0.4.0/src/gpttui/tui/app.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.3.0/src/gpttui/tui/config.py` & `gpttui-0.4.0/src/gpttui/tui/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 This file defines the main configuration options for the TUI.
 """
 import os
 from pathlib import Path
 from pydantic import BaseModel
+from typing import TypeVar, Type
+from gpttui.models.openai import OpenAIConf
+
+ConfT = TypeVar("ConfT", OpenAIConf, BaseModel)
 
 __CSS_CONFIG = """
 Prompt {
     dock: bottom;
     layout: horizontal;
     padding: 0;
     margin: 0;
@@ -100,14 +104,38 @@
     """
     home_path = os.environ["HOME"]
     cfg_path = Path(os.path.join(home_path, ".config/gpttui"))
     if not cfg_path.exists():
         cfg_path.mkdir()
     return cfg_path
 
+def config_file(path: Path, type: Type[ConfT]) -> ConfT:
+    """
+    Setups the config file given any configuration type.
+
+    Parameters
+    ----------
+    path : str
+        Configuration path.
+    type : Type[ConfT]
+        Configuration dataclass.
+
+    Returns
+    -------
+    ConfT
+        Loaded configuration.
+    """
+    if not path.exists():
+        obj = type()
+        with open(path, "w") as f:
+            f.write(obj.json())
+    else:
+        obj = type.parse_file(path)
+    return obj
+
 def css_config():
     """
     Initializes the CSS configuration file.
     """
     cfg_path = config_folder()
     filename = cfg_path / "style.css"
     if not filename.exists():
```

### Comparing `gpttui-0.3.0/src/gpttui/tui/front.py` & `gpttui-0.4.0/src/gpttui/tui/front.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 This file defines the CLI options in the front subcommand.
 """
 import os
 from pathlib import Path
 from click import option, command
+from pydantic import BaseModel
 from gpttui.database.base import AbstractDB, DatabasesEnum
 from gpttui.database.sqlite import SqliteDB
 from gpttui.models.base import AbstractModel, ModelsEnum
-from gpttui.models.openai import OpenAIModel
+from gpttui.models.chatsonic import ChatSonicConf, ChatSonicModel
+from gpttui.models.openai import OpenAIModel, OpenAIConf
 from gpttui.tui.app import GptApp
+from gpttui.tui.config import config_file
 from typing import Dict, Type
 
 DBS: Dict[DatabasesEnum, Type[AbstractDB]] = {
         DatabasesEnum.SQLITE: SqliteDB
         }
 MODELS: Dict[ModelsEnum, Type[AbstractModel]] = {
-        ModelsEnum.OPENAI: OpenAIModel
+        ModelsEnum.OPENAI: OpenAIModel,
+        ModelsEnum.CHATSONIC: ChatSonicModel
+        }
+CONFS: Dict[ModelsEnum, Type[BaseModel]] = {
+        ModelsEnum.OPENAI: OpenAIConf,
+        ModelsEnum.CHATSONIC: ChatSonicConf
         }
 
 @command()
 @option(
     "--database_kind",
     type=DatabasesEnum,
     default=DatabasesEnum.SQLITE,
@@ -40,32 +48,32 @@
 @option(
     "--model_kind",
     type=ModelsEnum,
     default=ModelsEnum.OPENAI,
     help="Which model to use."
     )
 @option(
-    "--model_name",
-    type=str,
-    default="gpt-3.5-turbo",
-    help="Model's name."
-    )
-@option(
     "--context",
     type=str,
     default="You are an AI assistant",
     help="Context for the model."
     )
+@option(
+    "--config",
+    type=Path,
+    default=Path(os.environ["HOME"]) / ".config/gpttui/openai.json",
+    help="Context for the model."
+    )
 def front(
     database_kind: DatabasesEnum,
     database_name: str,
     session: str,
     model_kind: ModelsEnum,
-    model_name: str,
-    context: str
+    context: str,
+    config: Path
     ) -> None:
     """
     Determines what to do when the front subcommand is launched.
 
     Parameters
     ----------
     database_kind : DatabasesEnum
@@ -76,23 +84,27 @@
         Session name.
     model_kind : ModelsEnum
         Which model to use.
     model_name : str
         Model name.
     context : str
         Context for the model.
+    config : Path
+        Configuration file.
     """
     db = (
             DBS[database_kind]()
             .setup(database=database_name)
             )
     db.create_session(session_name=session)
+    cfg = config_file(config, CONFS[model_kind])
+
     model = (
             MODELS[model_kind]()
             .add_context(context=context)
-            .setup(model_name=model_name, database=db, session_name=session)
+            .setup(config=cfg, database=db, session_name=session)
             )
     app = (
             GptApp()
             .setup(model=model)
             )
     app.run()
```

### Comparing `gpttui-0.3.0/test/test_db.py` & `gpttui-0.4.0/test/test_db.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.3.0/test/test_model.py` & `gpttui-0.4.0/test/test_model.py`

 * *Files identical despite different names*

