# Comparing `tmp/ws_cli_chat-0.3.1.tar.gz` & `tmp/ws_cli_chat-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.3.1.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.3.5.tar", max compression
```

## Comparing `ws_cli_chat-0.3.1.tar` & `ws_cli_chat-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      582 2023-04-23 22:38:57.030007 ws_cli_chat-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.1/README.md
--rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.3.1/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0     3283 2023-04-23 22:38:40.250507 ws_cli_chat-0.3.1/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0     2901 2023-04-23 22:38:40.280494 ws_cli_chat-0.3.1/ws_cli_chat/myconsole.py
--rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.3.1/ws_cli_chat/render.py
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      582 2023-04-24 21:32:24.101063 ws_cli_chat-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.5/README.md
+-rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.3.5/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     3296 2023-04-24 21:25:40.373180 ws_cli_chat-0.3.5/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.3.5/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.3.5/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.5/PKG-INFO
```

### Comparing `ws_cli_chat-0.3.1/pyproject.toml` & `ws_cli_chat-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ws_cli_chat"
-version = "0.3.1"
+version = "0.3.5"
 description = "simple cli-websocket-ws-cli-chat"
 authors = ["__coelho__ <109885900+MikalROn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "ws_cli_chat"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ws_cli_chat-0.3.1/README.md` & `ws_cli_chat-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.1/ws_cli_chat/cli_chat.py` & `ws_cli_chat-0.3.5/ws_cli_chat/cli_chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 app = typer.Typer()
 MESSAGES: list[str] = []
 
 
 def rederizar_menssagens(lista_menssagens: list) -> None:
     MyConsole.clear()
     [print(menssagen) for menssagen in lista_menssagens]
-    MyConsole.br(300)
+    MyConsole.br(30)
 
 
 async def recive_message(socket) -> None:
     try:
         while True:
             msg: str = await socket.recv()
             if msg:
@@ -30,15 +30,15 @@
         return None
 
 
 def send_message(socket) -> None:
     while True:
         try:
             msg: str = input()
-            if msg:
+            if msg and msg != '':
                 asyncio.run(socket.send(msg))
         except KeyboardInterrupt:
             return None
 
 
 def winded_send_message(socket) -> None:
     loop = EventSimpleGUI()
```

### Comparing `ws_cli_chat-0.3.1/ws_cli_chat/myconsole.py` & `ws_cli_chat-0.3.5/ws_cli_chat/myconsole.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,23 @@
 import subprocess
 from rich.console import Console
 
 
 console = Console(record=True)
 
 
-
 class MyConsole:
     
-
-    
     def __init__(self):
         raise NotImplementedError
 
     @staticmethod
-    def clear() -> str:
+    def clear():
         """ Gerado pelo chat gpt"""
-        past = console.export_text()
-        console.clear()
-        return past
+        os.system('cls' if os.name == 'nt' else 'clear')
 
 
     @staticmethod
     def clear_line():
         """Limpa a linha atual do console"""
         sys.stdout.write("\033[K")
```

### Comparing `ws_cli_chat-0.3.1/ws_cli_chat/render.py` & `ws_cli_chat-0.3.5/ws_cli_chat/render.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.1/PKG-INFO` & `ws_cli_chat-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.3.1
+Version: 0.3.5
 Summary: simple cli-websocket-ws-cli-chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

