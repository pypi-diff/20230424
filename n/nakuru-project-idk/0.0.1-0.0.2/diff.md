# Comparing `tmp/nakuru_project_idk-0.0.1.tar.gz` & `tmp/nakuru_project_idk-0.0.2.tar.gz`

## Comparing `nakuru_project_idk-0.0.1.tar` & `nakuru_project_idk-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0   280258 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/logo.png
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/setup.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/__init__.py
--rw-r--r--   0        0        0    14029 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/application.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/logger.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/misc.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/network.py
--rw-r--r--   0        0        0    29335 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/protocol.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/__init__.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/components.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/device.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/file.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/friend.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/group.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/guild.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/entities/others.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/event/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/event/builtins.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/event/enums.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/event/models.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/examples/forward_message.py
--rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/nakuru/examples/src/1.jpg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/LICENSE
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   280258 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/logo.png
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/setup.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/__init__.py
+-rw-r--r--   0        0        0    14029 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/application.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/logger.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/misc.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/network.py
+-rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/protocol.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/__init__.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/components.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/device.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/file.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/friend.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/group.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/guild.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/entities/others.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/builtins.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/enums.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/event/models.py
+-rw-r--r--   0        0        0    51695 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/examples/src/1.jpg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/nakuru/examples/src/forward_message.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 nakuru_project_idk-0.0.2/PKG-INFO
```

### Comparing `nakuru_project_idk-0.0.1/logo.png` & `nakuru_project_idk-0.0.2/logo.png`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/setup.py` & `nakuru_project_idk-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/application.py` & `nakuru_project_idk-0.0.2/nakuru/application.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/misc.py` & `nakuru_project_idk-0.0.2/nakuru/misc.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/network.py` & `nakuru_project_idk-0.0.2/nakuru/network.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/protocol.py` & `nakuru_project_idk-0.0.2/nakuru/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,29 @@
         result = await fetch.http_post(f"{self.baseurl_http}/send_group_forward_msg", {
             "group_id": group_id,
             "messages": messages
         }, params=self.protocol_params)
         if result["status"] == "ok":
             return BotMessage.parse_obj(result["data"])
         return False
+    
+    async def sendPrivateForwardMessage(self,
+                                        user_id: int,
+                                        messages: list) -> T.Union[BotMessage, bool]:
+        for i in range(len(messages)):
+            if isinstance(messages[i], Node):
+                messages[i] = messages[i].toDict()
+
+        result = await fetch.http_post(f"{self.baseurl_http}/send_private_forward_msg", {
+            "user_id": user_id,
+            "messages": messages
+        }, params=self.protocol_params)
+        if result["status"] == "ok":
+            return BotMessage.parse_obj(result["data"])
+        return False
 
     async def recall(self, message_id: int) -> bool:
         result = await fetch.http_post(f"{self.baseurl_http}/delete_msg", {
             "message_id": message_id
         }, params=self.protocol_params)
         if result["status"] == "ok":
             return True
@@ -251,15 +266,15 @@
             "reason": reason
         }, params=self.protocol_params)
         if result["status"] == "ok":
             return True
         return False
 
     async def getLoginInfo(self) -> T.Union[Bot, bool]:
-        result = await fetch.http_post(f"{self.baseurl_http}/get_login_info")
+        result = await fetch.http_post(f"{self.baseurl_http}/get_login_info", params=self.protocol_params)
         if result["status"] == "ok":
             return Bot.parse_obj(result["data"])
         return False
 
     async def getQiDianAccountInfo(self) -> T.Union[QiDianAccount, bool]:
         result = await fetch.http_post(f"{self.baseurl_http}/qidian_get_account_info")
         if result["status"] == "ok":
```

### Comparing `nakuru_project_idk-0.0.1/nakuru/entities/components.py` & `nakuru_project_idk-0.0.2/nakuru/entities/components.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/entities/file.py` & `nakuru_project_idk-0.0.2/nakuru/entities/file.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/entities/group.py` & `nakuru_project_idk-0.0.2/nakuru/entities/group.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/entities/guild.py` & `nakuru_project_idk-0.0.2/nakuru/entities/guild.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/entities/others.py` & `nakuru_project_idk-0.0.2/nakuru/entities/others.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/event/builtins.py` & `nakuru_project_idk-0.0.2/nakuru/event/builtins.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/event/enums.py` & `nakuru_project_idk-0.0.2/nakuru/event/enums.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/event/models.py` & `nakuru_project_idk-0.0.2/nakuru/event/models.py`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/nakuru/examples/forward_message.py` & `nakuru_project_idk-0.0.2/nakuru/examples/src/forward_message.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 from nakuru import (
     CQHTTP,
-    GroupMessage
+    GroupMessage,
+    FriendMessage
 )
 from nakuru.entities.components import Plain, Node, Image
 
 app = CQHTTP(
-    host="127.0.0.1",
+    host="8.9.15.33",
     port=6700,
-    http_port=5700
+    http_port=5700,
+    token="000112000112"
 )
 
+@app.receiver("FriendMessage")
+async def _(app: CQHTTP, source: FriendMessage):
+    await app.sendPrivateForwardMessage(source.user_id, [
+        Node(name="落雪ちゃん", uin=2941383730, content=[
+            Plain(text="nc什么时候cos小老师")
+        ]),
+        Node(name="盐焗雾喵", uin=2190945952, content=[
+            Plain(text="今晚就cos小老师")
+        ]),
+        Node(name="Rosemoe♪ ~ requiem ~", uin=2073412493, content=[
+            Plain(text="好耶"),
+            Image.fromFileSystem("./src/1.jpg")
+        ])
+    ])
+
 @app.receiver("GroupMessage")
 async def _(app: CQHTTP, source: GroupMessage):
     # 方法 1
     await app.sendGroupForwardMessage(source.group_id, [
         Node(name="落雪ちゃん", uin=2941383730, content=[
             Plain(text="nc什么时候cos小老师")
         ]),
```

### Comparing `nakuru_project_idk-0.0.1/nakuru/examples/src/1.jpg` & `nakuru_project_idk-0.0.2/nakuru/examples/src/1.jpg`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/LICENSE` & `nakuru_project_idk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/README.md` & `nakuru_project_idk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nakuru_project_idk-0.0.1/pyproject.toml` & `nakuru_project_idk-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nakuru-project-idk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lxns-Network", email="joinchang1206@gmail.com" },
+  { name="RockChinQ", email="junyan_qin@qq.com"}
 ]
 description = "一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `nakuru_project_idk-0.0.1/PKG-INFO` & `nakuru_project_idk-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nakuru-project-idk
-Version: 0.0.1
+Version: 0.0.2
 Summary: 一款为 go-cqhttp 的正向 WebSocket 设计的 Python SDK，支持纯 CQ 码与消息链的转换处理
 Project-URL: Homepage, https://github.com/idoknow/nakuru-project-idk
 Project-URL: Bug Tracker, https://github.com/idoknow/nakuru-project-idk/issues
-Author-email: Lxns-Network <joinchang1206@gmail.com>
+Author-email: Lxns-Network <joinchang1206@gmail.com>, RockChinQ <junyan_qin@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: async-lru
```

