# Comparing `tmp/ws_cli_chat-0.3.5.tar.gz` & `tmp/ws_cli_chat-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.3.5.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.3.7.tar", max compression
```

## Comparing `ws_cli_chat-0.3.5.tar` & `ws_cli_chat-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      582 2023-04-24 21:32:24.101063 ws_cli_chat-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.5/README.md
--rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.3.5/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0     3296 2023-04-24 21:25:40.373180 ws_cli_chat-0.3.5/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.3.5/ws_cli_chat/myconsole.py
--rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.3.5/ws_cli_chat/render.py
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      597 2023-04-24 21:39:12.188084 ws_cli_chat-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.7/README.md
+-rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.3.7/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     3296 2023-04-24 21:25:40.373180 ws_cli_chat-0.3.7/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.3.7/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.3.7/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.7/PKG-INFO
```

### Comparing `ws_cli_chat-0.3.5/pyproject.toml` & `ws_cli_chat-0.3.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "ws_cli_chat"
-version = "0.3.5"
+version = "0.3.7"
 description = "simple cli-websocket-ws-cli-chat"
 authors = ["__coelho__ <109885900+MikalROn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "ws_cli_chat"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.7.0"}
 websockets = "^11.0.2"
 colorama = "^0.4.6"
 eventsimplegui = "^0.3.0"
 pysimplegui = "^4.60.4"
+tk = "^0.1.0"
 
 [tool.poetry.scripts]
 chat = "ws_cli_chat.cli_chat:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ws_cli_chat-0.3.5/README.md` & `ws_cli_chat-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.5/ws_cli_chat/cli_chat.py` & `ws_cli_chat-0.3.7/ws_cli_chat/cli_chat.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.5/ws_cli_chat/myconsole.py` & `ws_cli_chat-0.3.7/ws_cli_chat/myconsole.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.5/ws_cli_chat/render.py` & `ws_cli_chat-0.3.7/ws_cli_chat/render.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.5/PKG-INFO` & `ws_cli_chat-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.3.5
+Version: 0.3.7
 Summary: simple cli-websocket-ws-cli-chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: eventsimplegui (>=0.3.0,<0.4.0)
 Requires-Dist: pysimplegui (>=4.60.4,<5.0.0)
+Requires-Dist: tk (>=0.1.0,<0.2.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Description-Content-Type: text/markdown
 
 # Chat Application
 This is a command-line chat application built with Python that allows users to connect to a websocket server and chat with other users in real-time.
```

