# Comparing `tmp/kavk_api-0.9.7.4.tar.gz` & `tmp/kavk_api-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kavk_api-0.9.7.4.tar", max compression
+gzip compressed data, was "kavk_api-0.9.9.tar", max compression
```

## Comparing `kavk_api-0.9.7.4.tar` & `kavk_api-0.9.9.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1066 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/LICENSE
--rw-r--r--   0        0        0     1251 2023-04-08 11:46:12.307389 kavk_api-0.9.7.4/README.rst
--rw-r--r--   0        0        0       51 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/__init__.py
--rw-r--r--   0        0        0     3192 2023-04-08 15:49:21.388876 kavk_api-0.9.7.4/kavk_api/bot_longpoll.py
--rw-r--r--   0        0        0    10766 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/enums.py
--rw-r--r--   0        0        0      341 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/exceptions.py
--rw-r--r--   0        0        0     4037 2023-04-08 11:31:33.141480 kavk_api-0.9.7.4/kavk_api/kavk_api.py
--rw-r--r--   0        0        0     8287 2023-04-09 08:41:13.287542 kavk_api-0.9.7.4/kavk_api/longpoll.py
--rw-r--r--   0        0        0     3609 2023-04-10 10:30:26.347957 kavk_api-0.9.7.4/kavk_api/types/base.py
--rw-r--r--   0        0        0     8143 2023-04-09 07:57:29.029583 kavk_api-0.9.7.4/kavk_api/types/bot_events.py
--rw-r--r--   0        0        0     5024 2023-04-09 07:57:45.848583 kavk_api-0.9.7.4/kavk_api/types/event_objects.py
--rw-r--r--   0        0        0   261659 2023-04-09 19:27:05.290321 kavk_api-0.9.7.4/kavk_api/types/methods.py
--rw-r--r--   0        0        0   144553 2023-04-08 11:31:33.144480 kavk_api-0.9.7.4/kavk_api/types/objects.py
--rw-r--r--   0        0        0    43571 2023-04-10 10:34:30.165969 kavk_api-0.9.7.4/kavk_api/types/responses.py
--rw-r--r--   0        0        0      123 2023-04-08 11:31:33.145480 kavk_api-0.9.7.4/kavk_api/utils.py
--rw-r--r--   0        0        0      423 2023-04-10 10:35:46.812972 kavk_api-0.9.7.4/pyproject.toml
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kavk_api-0.9.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-24 13:58:38.368151 kavk_api-0.9.9/LICENSE
+-rw-r--r--   0        0        0     1073 2023-04-24 13:58:38.368151 kavk_api-0.9.9/README.rst
+-rw-r--r--   0        0        0       51 2023-04-24 13:58:38.368151 kavk_api-0.9.9/kavk_api/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-24 13:58:38.368151 kavk_api-0.9.9/kavk_api/bot.py
+-rw-r--r--   0        0        0      342 2023-04-24 13:58:38.368151 kavk_api-0.9.9/kavk_api/exceptions.py
+-rw-r--r--   0        0        0     4037 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/kavk_api.py
+-rw-r--r--   0        0        0      100 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/longpoll/__init__.py
+-rw-r--r--   0        0        0     3182 2023-04-24 13:59:22.617152 kavk_api-0.9.9/kavk_api/longpoll/bot_longpoll.py
+-rw-r--r--   0        0        0     5196 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/longpoll/enums.py
+-rw-r--r--   0        0        0     2585 2023-04-24 14:07:46.826164 kavk_api-0.9.9/kavk_api/longpoll/user_longpoll.py
+-rw-r--r--   0        0        0     3609 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/types/base.py
+-rw-r--r--   0        0        0     8143 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/types/bot_events.py
+-rw-r--r--   0        0        0     5024 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/types/event_objects.py
+-rw-r--r--   0        0        0   261659 2023-04-24 13:58:38.369151 kavk_api-0.9.9/kavk_api/types/methods.py
+-rw-r--r--   0        0        0   144579 2023-04-24 13:58:38.370151 kavk_api-0.9.9/kavk_api/types/objects.py
+-rw-r--r--   0        0        0    43571 2023-04-24 13:58:38.370151 kavk_api-0.9.9/kavk_api/types/responses.py
+-rw-r--r--   0        0        0     9698 2023-04-24 15:00:02.407235 kavk_api-0.9.9/kavk_api/types/user_events.py
+-rw-r--r--   0        0        0      102 2023-04-24 13:58:38.370151 kavk_api-0.9.9/kavk_api/user.py
+-rw-r--r--   0        0        0      123 2023-04-24 13:58:38.370151 kavk_api-0.9.9/kavk_api/utils.py
+-rw-r--r--   0        0        0      421 2023-04-24 13:58:38.370151 kavk_api-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 kavk_api-0.9.9/PKG-INFO
```

### Comparing `kavk_api-0.9.7.4/LICENSE` & `kavk_api-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/kavk_api/bot_longpoll.py` & `kavk_api-0.9.9/kavk_api/longpoll/bot_longpoll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .kavk_api import Vk
-from .types import bot_events as BotEvents
+from ..kavk_api import Vk
+from ..types import bot_events as BotEvent
 
 
 class BotLongPoll:
-    def __init__(self, vk:Vk, wait:int=25) -> None:
-        '''
+    '''
         Класс для работы с BotLongPoll
 
         ...
         
         vk:Vk
             Объект kavk_api.Vk
         wait:int = 25
             Время ожидания
-        '''
+    '''
+    def __init__(self, vk:Vk, wait:int=25) -> None:
         self._vk:Vk = vk
         self._wait:int = wait
         self._server:str = ''
         self._params:dict = {}
         self._updates:list = []
 
     async def listen(self):
@@ -62,15 +62,15 @@
     # Она же в свою очередь просто получает наш новый ивент и обрабатывает его
 
     def __aiter__(self): return self
 
     async def __anext__(self):
         if self._updates != []:
             u:dict = self._updates.pop(0)
-            event = BotEvents._get_event(u.get('type',''))
+            event = BotEvent._get_event(u.get('type',''))
             return event(**u, raw=u)
             
         updates = []
         while updates == []:
             '''
             Если событий за время self._wait не произойдёт, мы получим в ответ пустой список.
             Т.к. делать ивент из такого ответа хз как, мы просто ждем когда прийдет нормальный
@@ -78,11 +78,11 @@
             updates = await self.get_event() 
         
         if len(updates) > 0:
             self._updates = updates[1:]
             update:dict = updates[0]
         else: update:dict = updates[0]
         event_type = str(update.get('type', ''))
-        event = BotEvents._get_event(event_type)
+        event = BotEvent._get_event(event_type)
         return event(**update, raw=update)
 
-__all__ = ("BotLongPoll", 'BotEvents')
+__all__ = ("BotLongPoll", 'BotEvent')
```

### Comparing `kavk_api-0.9.7.4/kavk_api/kavk_api.py` & `kavk_api-0.9.9/kavk_api/kavk_api.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/kavk_api/types/base.py` & `kavk_api-0.9.9/kavk_api/types/base.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/kavk_api/types/bot_events.py` & `kavk_api-0.9.9/kavk_api/types/bot_events.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/kavk_api/types/event_objects.py` & `kavk_api-0.9.9/kavk_api/types/event_objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/kavk_api/types/methods.py` & `kavk_api-0.9.9/kavk_api/types/methods.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/kavk_api/types/objects.py` & `kavk_api-0.9.9/kavk_api/types/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -3801,5235 +3801,5237 @@
 0000ed80: 5669 6465 6f56 6964 656f 225d 203d 204e  VideoVideo"] = N
 0000ed90: 6f6e 650a 0977 616c 6c3a 4f70 7469 6f6e  one..wall:Option
 0000eda0: 616c 5b22 5761 6c6c 5761 6c6c 706f 7374  al["WallWallpost
 0000edb0: 4675 6c6c 225d 203d 204e 6f6e 650a 0a0a  Full"] = None...
 0000edc0: 636c 6173 7320 4d65 7373 6167 6573 4b65  class MessagesKe
 0000edd0: 7962 6f61 7264 2842 4d29 3a0a 096f 6e65  yboard(BM):..one
 0000ede0: 5f74 696d 653a 626f 6f6c 0a09 6275 7474  _time:bool..butt
-0000edf0: 6f6e 733a 6c69 7374 5b6c 6973 745d 0a09  ons:list[list]..
-0000ee00: 6175 7468 6f72 5f69 643a 4f70 7469 6f6e  author_id:Option
-0000ee10: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-0000ee20: 696e 6c69 6e65 3a4f 7074 696f 6e61 6c5b  inline:Optional[
-0000ee30: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 0a63  bool] = None...c
-0000ee40: 6c61 7373 204d 6573 7361 6765 734b 6579  lass MessagesKey
-0000ee50: 626f 6172 6442 7574 746f 6e28 424d 293a  boardButton(BM):
-0000ee60: 0a09 6163 7469 6f6e 3a22 4d65 7373 6167  ..action:"Messag
-0000ee70: 6573 4b65 7962 6f61 7264 4275 7474 6f6e  esKeyboardButton
-0000ee80: 5072 6f70 6572 7479 4163 7469 6f6e 220a  PropertyAction".
-0000ee90: 0963 6f6c 6f72 3a4f 7074 696f 6e61 6c5b  .color:Optional[
-0000eea0: 7374 725d 203d 204e 6f6e 650a 0a0a 636c  str] = None...cl
-0000eeb0: 6173 7320 4d65 7373 6167 6573 4b65 7962  ass MessagesKeyb
-0000eec0: 6f61 7264 4275 7474 6f6e 4163 7469 6f6e  oardButtonAction
-0000eed0: 4361 6c6c 6261 636b 2842 4d29 3a0a 096c  Callback(BM):..l
-0000eee0: 6162 656c 3a73 7472 0a09 7061 796c 6f61  abel:str..payloa
-0000eef0: 643a 4f70 7469 6f6e 616c 5b73 7472 5d20  d:Optional[str] 
-0000ef00: 3d20 4e6f 6e65 0a09 7479 7065 3a73 7472  = None..type:str
-0000ef10: 0a0a 0a63 6c61 7373 204d 6573 7361 6765  ...class Message
-0000ef20: 734b 6579 626f 6172 6442 7574 746f 6e41  sKeyboardButtonA
-0000ef30: 6374 696f 6e4c 6f63 6174 696f 6e28 424d  ctionLocation(BM
-0000ef40: 293a 0a09 7061 796c 6f61 643a 4f70 7469  ):..payload:Opti
-0000ef50: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000ef60: 0a09 7479 7065 3a73 7472 0a0a 0a63 6c61  ..type:str...cla
-0000ef70: 7373 204d 6573 7361 6765 734b 6579 626f  ss MessagesKeybo
-0000ef80: 6172 6442 7574 746f 6e41 6374 696f 6e4f  ardButtonActionO
-0000ef90: 7065 6e41 7070 2842 4d29 3a0a 0961 7070  penApp(BM):..app
-0000efa0: 5f69 643a 696e 740a 0968 6173 683a 4f70  _id:int..hash:Op
-0000efb0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000efc0: 6e65 0a09 6c61 6265 6c3a 7374 720a 096f  ne..label:str..o
-0000efd0: 776e 6572 5f69 643a 696e 740a 0970 6179  wner_id:int..pay
-0000efe0: 6c6f 6164 3a4f 7074 696f 6e61 6c5b 7374  load:Optional[st
-0000eff0: 725d 203d 204e 6f6e 650a 0974 7970 653a  r] = None..type:
-0000f000: 7374 720a 0a0a 636c 6173 7320 4d65 7373  str...class Mess
-0000f010: 6167 6573 4b65 7962 6f61 7264 4275 7474  agesKeyboardButt
-0000f020: 6f6e 4163 7469 6f6e 4f70 656e 4c69 6e6b  onActionOpenLink
-0000f030: 2842 4d29 3a0a 096c 6162 656c 3a73 7472  (BM):..label:str
-0000f040: 0a09 6c69 6e6b 3a73 7472 0a09 7061 796c  ..link:str..payl
-0000f050: 6f61 643a 4f70 7469 6f6e 616c 5b73 7472  oad:Optional[str
-0000f060: 5d20 3d20 4e6f 6e65 0a09 7479 7065 3a73  ] = None..type:s
-0000f070: 7472 0a0a 0a63 6c61 7373 204d 6573 7361  tr...class Messa
-0000f080: 6765 734b 6579 626f 6172 6442 7574 746f  gesKeyboardButto
-0000f090: 6e41 6374 696f 6e4f 7065 6e50 686f 746f  nActionOpenPhoto
-0000f0a0: 2842 4d29 3a0a 0974 7970 653a 7374 720a  (BM):..type:str.
-0000f0b0: 0a0a 636c 6173 7320 4d65 7373 6167 6573  ..class Messages
-0000f0c0: 4b65 7962 6f61 7264 4275 7474 6f6e 4163  KeyboardButtonAc
-0000f0d0: 7469 6f6e 5465 7874 2842 4d29 3a0a 096c  tionText(BM):..l
-0000f0e0: 6162 656c 3a73 7472 0a09 7061 796c 6f61  abel:str..payloa
-0000f0f0: 643a 4f70 7469 6f6e 616c 5b73 7472 5d20  d:Optional[str] 
-0000f100: 3d20 4e6f 6e65 0a09 7479 7065 3a73 7472  = None..type:str
-0000f110: 0a0a 0a63 6c61 7373 204d 6573 7361 6765  ...class Message
-0000f120: 734b 6579 626f 6172 6442 7574 746f 6e41  sKeyboardButtonA
-0000f130: 6374 696f 6e56 6b70 6179 2842 4d29 3a0a  ctionVkpay(BM):.
-0000f140: 0968 6173 683a 7374 720a 0970 6179 6c6f  .hash:str..paylo
-0000f150: 6164 3a4f 7074 696f 6e61 6c5b 7374 725d  ad:Optional[str]
-0000f160: 203d 204e 6f6e 650a 0974 7970 653a 7374   = None..type:st
-0000f170: 720a 0a0a 636c 6173 7320 4d65 7373 6167  r...class Messag
-0000f180: 6573 4b65 7962 6f61 7264 4275 7474 6f6e  esKeyboardButton
-0000f190: 5072 6f70 6572 7479 4163 7469 6f6e 2842  PropertyAction(B
-0000f1a0: 4d29 3a0a 0970 6173 730a 0a63 6c61 7373  M):..pass..class
-0000f1b0: 204d 6573 7361 6765 734c 6173 7441 6374   MessagesLastAct
-0000f1c0: 6976 6974 7928 424d 293a 0a09 6f6e 6c69  ivity(BM):..onli
-0000f1d0: 6e65 3a62 6f6f 6c0a 0974 696d 653a 696e  ne:bool..time:in
-0000f1e0: 740a 0a0a 636c 6173 7320 4d65 7373 6167  t...class Messag
-0000f1f0: 6573 4c6f 6e67 706f 6c6c 4d65 7373 6167  esLongpollMessag
-0000f200: 6573 2842 4d29 3a0a 0963 6f75 6e74 3a4f  es(BM):..count:O
-0000f210: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0000f220: 6f6e 650a 0969 7465 6d73 3a4f 7074 696f  one..items:Optio
-0000f230: 6e61 6c5b 6c69 7374 5b22 4d65 7373 6167  nal[list["Messag
-0000f240: 6573 4d65 7373 6167 6522 5d5d 203d 204e  esMessage"]] = N
-0000f250: 6f6e 650a 0a0a 636c 6173 7320 4d65 7373  one...class Mess
-0000f260: 6167 6573 4c6f 6e67 706f 6c6c 5061 7261  agesLongpollPara
-0000f270: 6d73 2842 4d29 3a0a 0973 6572 7665 723a  ms(BM):..server:
-0000f280: 7374 720a 096b 6579 3a73 7472 0a09 7473  str..key:str..ts
-0000f290: 3a69 6e74 0a09 7074 733a 4f70 7469 6f6e  :int..pts:Option
-0000f2a0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
-0000f2b0: 0a63 6c61 7373 204d 6573 7361 6765 734d  .class MessagesM
-0000f2c0: 6573 7361 6765 2842 4d29 3a0a 0961 6374  essage(BM):..act
-0000f2d0: 696f 6e3a 4f70 7469 6f6e 616c 5b22 4d65  ion:Optional["Me
-0000f2e0: 7373 6167 6573 4d65 7373 6167 6541 6374  ssagesMessageAct
-0000f2f0: 696f 6e22 5d20 3d20 4e6f 6e65 0a09 6164  ion"] = None..ad
-0000f300: 6d69 6e5f 6175 7468 6f72 5f69 643a 4f70  min_author_id:Op
-0000f310: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0000f320: 6e65 0a09 6174 7461 6368 6d65 6e74 733a  ne..attachments:
-0000f330: 4f70 7469 6f6e 616c 5b6c 6973 745b 224d  Optional[list["M
-0000f340: 6573 7361 6765 734d 6573 7361 6765 4174  essagesMessageAt
-0000f350: 7461 6368 6d65 6e74 225d 5d20 3d20 4e6f  tachment"]] = No
-0000f360: 6e65 0a09 636f 6e76 6572 7361 7469 6f6e  ne..conversation
-0000f370: 5f6d 6573 7361 6765 5f69 643a 4f70 7469  _message_id:Opti
-0000f380: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-0000f390: 0a09 6461 7465 3a69 6e74 0a09 6465 6c65  ..date:int..dele
-0000f3a0: 7465 643a 4f70 7469 6f6e 616c 5b62 6f6f  ted:Optional[boo
-0000f3b0: 6c5d 203d 204e 6f6e 650a 0966 726f 6d5f  l] = None..from_
-0000f3c0: 6964 3a69 6e74 0a09 6677 645f 6d65 7373  id:int..fwd_mess
-0000f3d0: 6167 6573 3a4f 7074 696f 6e61 6c5b 6c69  ages:Optional[li
-0000f3e0: 7374 5b22 4d65 7373 6167 6573 466f 7265  st["MessagesFore
-0000f3f0: 6967 6e4d 6573 7361 6765 225d 5d20 3d20  ignMessage"]] = 
-0000f400: 4e6f 6e65 0a09 6765 6f3a 4f70 7469 6f6e  None..geo:Option
-0000f410: 616c 5b22 4261 7365 4765 6f22 5d20 3d20  al["BaseGeo"] = 
-0000f420: 4e6f 6e65 0a09 6964 3a69 6e74 0a09 696d  None..id:int..im
-0000f430: 706f 7274 616e 743a 4f70 7469 6f6e 616c  portant:Optional
-0000f440: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0969  [bool] = None..i
-0000f450: 735f 6869 6464 656e 3a4f 7074 696f 6e61  s_hidden:Optiona
-0000f460: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0000f470: 6973 5f63 726f 7070 6564 3a4f 7074 696f  is_cropped:Optio
-0000f480: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0000f490: 0a09 6b65 7962 6f61 7264 3a4f 7074 696f  ..keyboard:Optio
-0000f4a0: 6e61 6c5b 224d 6573 7361 6765 734b 6579  nal["MessagesKey
-0000f4b0: 626f 6172 6422 5d20 3d20 4e6f 6e65 0a09  board"] = None..
-0000f4c0: 6d65 6d62 6572 735f 636f 756e 743a 4f70  members_count:Op
-0000f4d0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0000f4e0: 6e65 0a09 6f75 743a 626f 6f6c 0a09 7061  ne..out:bool..pa
-0000f4f0: 796c 6f61 643a 4f70 7469 6f6e 616c 5b73  yload:Optional[s
-0000f500: 7472 5d20 3d20 4e6f 6e65 0a09 7065 6572  tr] = None..peer
-0000f510: 5f69 643a 696e 740a 0972 616e 646f 6d5f  _id:int..random_
-0000f520: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-0000f530: 203d 204e 6f6e 650a 0972 6566 3a4f 7074   = None..ref:Opt
-0000f540: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000f550: 650a 0972 6566 5f73 6f75 7263 653a 4f70  e..ref_source:Op
-0000f560: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000f570: 6e65 0a09 7265 706c 795f 6d65 7373 6167  ne..reply_messag
-0000f580: 653a 4f70 7469 6f6e 616c 5b22 4d65 7373  e:Optional["Mess
-0000f590: 6167 6573 466f 7265 6967 6e4d 6573 7361  agesForeignMessa
-0000f5a0: 6765 225d 203d 204e 6f6e 650a 0974 6578  ge"] = None..tex
-0000f5b0: 743a 7374 720a 0975 7064 6174 655f 7469  t:str..update_ti
-0000f5c0: 6d65 3a4f 7074 696f 6e61 6c5b 696e 745d  me:Optional[int]
-0000f5d0: 203d 204e 6f6e 650a 0977 6173 5f6c 6973   = None..was_lis
-0000f5e0: 7465 6e65 643a 4f70 7469 6f6e 616c 5b62  tened:Optional[b
-0000f5f0: 6f6f 6c5d 203d 204e 6f6e 650a 0970 696e  ool] = None..pin
-0000f600: 6e65 645f 6174 3a4f 7074 696f 6e61 6c5b  ned_at:Optional[
-0000f610: 696e 745d 203d 204e 6f6e 650a 0969 735f  int] = None..is_
-0000f620: 7369 6c65 6e74 3a4f 7074 696f 6e61 6c5b  silent:Optional[
-0000f630: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 0a63  bool] = None...c
-0000f640: 6c61 7373 204d 6573 7361 6765 734d 6573  lass MessagesMes
-0000f650: 7361 6765 4163 7469 6f6e 2842 4d29 3a0a  sageAction(BM):.
-0000f660: 0963 6f6e 7665 7273 6174 696f 6e5f 6d65  .conversation_me
-0000f670: 7373 6167 655f 6964 3a4f 7074 696f 6e61  ssage_id:Optiona
-0000f680: 6c5b 696e 745d 203d 204e 6f6e 650a 0965  l[int] = None..e
-0000f690: 6d61 696c 3a4f 7074 696f 6e61 6c5b 7374  mail:Optional[st
-0000f6a0: 725d 203d 204e 6f6e 650a 096d 656d 6265  r] = None..membe
-0000f6b0: 725f 6964 3a4f 7074 696f 6e61 6c5b 696e  r_id:Optional[in
-0000f6c0: 745d 203d 204e 6f6e 650a 096d 6573 7361  t] = None..messa
-0000f6d0: 6765 3a4f 7074 696f 6e61 6c5b 7374 725d  ge:Optional[str]
-0000f6e0: 203d 204e 6f6e 650a 0970 686f 746f 3a4f   = None..photo:O
-0000f6f0: 7074 696f 6e61 6c5b 224d 6573 7361 6765  ptional["Message
-0000f700: 734d 6573 7361 6765 4163 7469 6f6e 5068  sMessageActionPh
-0000f710: 6f74 6f22 5d20 3d20 4e6f 6e65 0a09 7465  oto"] = None..te
-0000f720: 7874 3a4f 7074 696f 6e61 6c5b 7374 725d  xt:Optional[str]
-0000f730: 203d 204e 6f6e 650a 0974 7970 653a 224d   = None..type:"M
-0000f740: 6573 7361 6765 734d 6573 7361 6765 4163  essagesMessageAc
-0000f750: 7469 6f6e 5374 6174 7573 220a 0a0a 636c  tionStatus"...cl
-0000f760: 6173 7320 4d65 7373 6167 6573 4d65 7373  ass MessagesMess
-0000f770: 6167 6541 6374 696f 6e50 686f 746f 2842  ageActionPhoto(B
-0000f780: 4d29 3a0a 0970 686f 746f 5f35 303a 7374  M):..photo_50:st
-0000f790: 720a 0970 686f 746f 5f31 3030 3a73 7472  r..photo_100:str
-0000f7a0: 0a09 7068 6f74 6f5f 3230 303a 7374 720a  ..photo_200:str.
-0000f7b0: 0a0a 636c 6173 7320 4d65 7373 6167 6573  ..class Messages
-0000f7c0: 4d65 7373 6167 6541 7474 6163 686d 656e  MessageAttachmen
-0000f7d0: 7428 424d 293a 0a09 6175 6469 6f3a 4f70  t(BM):..audio:Op
-0000f7e0: 7469 6f6e 616c 5b22 4175 6469 6f41 7564  tional["AudioAud
-0000f7f0: 696f 225d 203d 204e 6f6e 650a 0961 7564  io"] = None..aud
-0000f800: 696f 5f6d 6573 7361 6765 3a4f 7074 696f  io_message:Optio
-0000f810: 6e61 6c5b 224d 6573 7361 6765 7341 7564  nal["MessagesAud
-0000f820: 696f 4d65 7373 6167 6522 5d20 3d20 4e6f  ioMessage"] = No
-0000f830: 6e65 0a09 6361 6c6c 3a4f 7074 696f 6e61  ne..call:Optiona
-0000f840: 6c5b 2243 616c 6c73 4361 6c6c 225d 203d  l["CallsCall"] =
-0000f850: 204e 6f6e 650a 0964 6f63 3a4f 7074 696f   None..doc:Optio
-0000f860: 6e61 6c5b 2244 6f63 7344 6f63 225d 203d  nal["DocsDoc"] =
-0000f870: 204e 6f6e 650a 0967 6966 743a 4f70 7469   None..gift:Opti
-0000f880: 6f6e 616c 5b22 4769 6674 734c 6179 6f75  onal["GiftsLayou
-0000f890: 7422 5d20 3d20 4e6f 6e65 0a09 6772 6166  t"] = None..graf
-0000f8a0: 6669 7469 3a4f 7074 696f 6e61 6c5b 224d  fiti:Optional["M
-0000f8b0: 6573 7361 6765 7347 7261 6666 6974 6922  essagesGraffiti"
-0000f8c0: 5d20 3d20 4e6f 6e65 0a09 6d61 726b 6574  ] = None..market
-0000f8d0: 3a4f 7074 696f 6e61 6c5b 224d 6172 6b65  :Optional["Marke
-0000f8e0: 744d 6172 6b65 7449 7465 6d22 5d20 3d20  tMarketItem"] = 
-0000f8f0: 4e6f 6e65 0a09 6d61 726b 6574 5f6d 6172  None..market_mar
-0000f900: 6b65 745f 616c 6275 6d3a 4f70 7469 6f6e  ket_album:Option
-0000f910: 616c 5b22 4d61 726b 6574 4d61 726b 6574  al["MarketMarket
-0000f920: 416c 6275 6d22 5d20 3d20 4e6f 6e65 0a09  Album"] = None..
-0000f930: 7068 6f74 6f3a 4f70 7469 6f6e 616c 5b22  photo:Optional["
-0000f940: 5068 6f74 6f73 5068 6f74 6f22 5d20 3d20  PhotosPhoto"] = 
-0000f950: 4e6f 6e65 0a09 7374 6963 6b65 723a 4f70  None..sticker:Op
-0000f960: 7469 6f6e 616c 5b22 4261 7365 5374 6963  tional["BaseStic
-0000f970: 6b65 7222 5d20 3d20 4e6f 6e65 0a09 7374  ker"] = None..st
-0000f980: 6f72 793a 4f70 7469 6f6e 616c 5b22 5374  ory:Optional["St
-0000f990: 6f72 6965 7353 746f 7279 225d 203d 204e  oriesStory"] = N
-0000f9a0: 6f6e 650a 0974 7970 653a 224d 6573 7361  one..type:"Messa
-0000f9b0: 6765 734d 6573 7361 6765 4174 7461 6368  gesMessageAttach
-0000f9c0: 6d65 6e74 5479 7065 220a 0976 6964 656f  mentType"..video
-0000f9d0: 3a4f 7074 696f 6e61 6c5b 2256 6964 656f  :Optional["Video
-0000f9e0: 5669 6465 6f46 756c 6c22 5d20 3d20 4e6f  VideoFull"] = No
-0000f9f0: 6e65 0a09 7761 6c6c 5f72 6570 6c79 3a4f  ne..wall_reply:O
-0000fa00: 7074 696f 6e61 6c5b 2257 616c 6c57 616c  ptional["WallWal
-0000fa10: 6c43 6f6d 6d65 6e74 225d 203d 204e 6f6e  lComment"] = Non
-0000fa20: 650a 0970 6f6c 6c3a 4f70 7469 6f6e 616c  e..poll:Optional
-0000fa30: 5b22 506f 6c6c 7350 6f6c 6c22 5d20 3d20  ["PollsPoll"] = 
-0000fa40: 4e6f 6e65 0a0a 0a63 6c61 7373 204d 6573  None...class Mes
-0000fa50: 7361 6765 734d 6573 7361 6765 5265 7175  sagesMessageRequ
-0000fa60: 6573 7444 6174 6128 424d 293a 0a09 7374  estData(BM):..st
-0000fa70: 6174 7573 3a4f 7074 696f 6e61 6c5b 7374  atus:Optional[st
-0000fa80: 725d 203d 204e 6f6e 650a 0969 6e76 6974  r] = None..invit
-0000fa90: 6572 5f69 643a 4f70 7469 6f6e 616c 5b69  er_id:Optional[i
-0000faa0: 6e74 5d20 3d20 4e6f 6e65 0a09 7265 7175  nt] = None..requ
-0000fab0: 6573 745f 6461 7465 3a4f 7074 696f 6e61  est_date:Optiona
-0000fac0: 6c5b 696e 745d 203d 204e 6f6e 650a 0a0a  l[int] = None...
-0000fad0: 636c 6173 7320 4d65 7373 6167 6573 4d65  class MessagesMe
-0000fae0: 7373 6167 6573 4172 7261 7928 424d 293a  ssagesArray(BM):
-0000faf0: 0a09 636f 756e 743a 4f70 7469 6f6e 616c  ..count:Optional
-0000fb00: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6974  [int] = None..it
-0000fb10: 656d 733a 4f70 7469 6f6e 616c 5b6c 6973  ems:Optional[lis
-0000fb20: 745b 224d 6573 7361 6765 734d 6573 7361  t["MessagesMessa
-0000fb30: 6765 225d 5d20 3d20 4e6f 6e65 0a0a 0a63  ge"]] = None...c
-0000fb40: 6c61 7373 204d 6573 7361 6765 734f 7574  lass MessagesOut
-0000fb50: 5265 6164 4279 2842 4d29 3a0a 0963 6f75  ReadBy(BM):..cou
-0000fb60: 6e74 3a4f 7074 696f 6e61 6c5b 696e 745d  nt:Optional[int]
-0000fb70: 203d 204e 6f6e 650a 096d 656d 6265 725f   = None..member_
-0000fb80: 6964 733a 4f70 7469 6f6e 616c 5b6c 6973  ids:Optional[lis
-0000fb90: 745b 696e 745d 5d20 3d20 4e6f 6e65 0a0a  t[int]] = None..
-0000fba0: 0a63 6c61 7373 204d 6573 7361 6765 7350  .class MessagesP
-0000fbb0: 696e 6e65 644d 6573 7361 6765 2842 4d29  innedMessage(BM)
-0000fbc0: 3a0a 0961 7474 6163 686d 656e 7473 3a4f  :..attachments:O
-0000fbd0: 7074 696f 6e61 6c5b 6c69 7374 5b22 4d65  ptional[list["Me
-0000fbe0: 7373 6167 6573 4d65 7373 6167 6541 7474  ssagesMessageAtt
-0000fbf0: 6163 686d 656e 7422 5d5d 203d 204e 6f6e  achment"]] = Non
-0000fc00: 650a 0963 6f6e 7665 7273 6174 696f 6e5f  e..conversation_
-0000fc10: 6d65 7373 6167 655f 6964 3a4f 7074 696f  message_id:Optio
-0000fc20: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-0000fc30: 0969 643a 696e 740a 0964 6174 653a 696e  .id:int..date:in
-0000fc40: 740a 0966 726f 6d5f 6964 3a69 6e74 0a09  t..from_id:int..
-0000fc50: 6677 645f 6d65 7373 6167 6573 3a4f 7074  fwd_messages:Opt
-0000fc60: 696f 6e61 6c5b 6c69 7374 5b22 4d65 7373  ional[list["Mess
-0000fc70: 6167 6573 466f 7265 6967 6e4d 6573 7361  agesForeignMessa
-0000fc80: 6765 225d 5d20 3d20 4e6f 6e65 0a09 6765  ge"]] = None..ge
-0000fc90: 6f3a 4f70 7469 6f6e 616c 5b22 4261 7365  o:Optional["Base
-0000fca0: 4765 6f22 5d20 3d20 4e6f 6e65 0a09 7065  Geo"] = None..pe
-0000fcb0: 6572 5f69 643a 696e 740a 0972 6570 6c79  er_id:int..reply
-0000fcc0: 5f6d 6573 7361 6765 3a4f 7074 696f 6e61  _message:Optiona
-0000fcd0: 6c5b 224d 6573 7361 6765 7346 6f72 6569  l["MessagesForei
-0000fce0: 676e 4d65 7373 6167 6522 5d20 3d20 4e6f  gnMessage"] = No
-0000fcf0: 6e65 0a09 7465 7874 3a73 7472 0a09 6b65  ne..text:str..ke
-0000fd00: 7962 6f61 7264 3a4f 7074 696f 6e61 6c5b  yboard:Optional[
-0000fd10: 224d 6573 7361 6765 734b 6579 626f 6172  "MessagesKeyboar
-0000fd20: 6422 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  d"] = None...cla
-0000fd30: 7373 204d 6573 7361 6765 7350 7573 6853  ss MessagesPushS
-0000fd40: 6574 7469 6e67 7328 424d 293a 0a09 6469  ettings(BM):..di
-0000fd50: 7361 626c 6564 5f66 6f72 6576 6572 3a62  sabled_forever:b
-0000fd60: 6f6f 6c0a 0964 6973 6162 6c65 645f 756e  ool..disabled_un
-0000fd70: 7469 6c3a 4f70 7469 6f6e 616c 5b69 6e74  til:Optional[int
-0000fd80: 5d20 3d20 4e6f 6e65 0a09 6e6f 5f73 6f75  ] = None..no_sou
-0000fd90: 6e64 3a62 6f6f 6c0a 0964 6973 6162 6c65  nd:bool..disable
-0000fda0: 645f 6d65 6e74 696f 6e73 3a4f 7074 696f  d_mentions:Optio
-0000fdb0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0000fdc0: 0a09 6469 7361 626c 6564 5f6d 6173 735f  ..disabled_mass_
-0000fdd0: 6d65 6e74 696f 6e73 3a4f 7074 696f 6e61  mentions:Optiona
-0000fde0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a  l[bool] = None..
-0000fdf0: 0a63 6c61 7373 204d 6573 7361 6765 7353  .class MessagesS
-0000fe00: 656e 6455 7365 7249 6473 5265 7370 6f6e  endUserIdsRespon
-0000fe10: 7365 4974 656d 2842 4d29 3a0a 0970 6565  seItem(BM):..pee
-0000fe20: 725f 6964 3a69 6e74 0a09 6d65 7373 6167  r_id:int..messag
-0000fe30: 655f 6964 3a69 6e74 0a09 636f 6e76 6572  e_id:int..conver
-0000fe40: 7361 7469 6f6e 5f6d 6573 7361 6765 5f69  sation_message_i
-0000fe50: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-0000fe60: 3d20 4e6f 6e65 0a09 6572 726f 723a 4f70  = None..error:Op
-0000fe70: 7469 6f6e 616c 5b22 4261 7365 4d65 7373  tional["BaseMess
-0000fe80: 6167 6545 7272 6f72 225d 203d 204e 6f6e  ageError"] = Non
-0000fe90: 650a 0a0a 0a0a 636c 6173 7320 4e65 7773  e.....class News
-0000fea0: 6665 6564 436f 6d6d 656e 7473 4669 6c74  feedCommentsFilt
-0000feb0: 6572 7328 456e 756d 293a 0a09 504f 5354  ers(Enum):..POST
-0000fec0: 203d 2022 706f 7374 220a 0950 484f 544f   = "post"..PHOTO
-0000fed0: 203d 2022 7068 6f74 6f22 0a09 5649 4445   = "photo"..VIDE
-0000fee0: 4f20 3d20 2276 6964 656f 220a 0954 4f50  O = "video"..TOP
-0000fef0: 4943 203d 2022 746f 7069 6322 0a09 4e4f  IC = "topic"..NO
-0000ff00: 5445 203d 2022 6e6f 7465 220a 0a63 6c61  TE = "note"..cla
-0000ff10: 7373 204e 6577 7366 6565 6449 676e 6f72  ss NewsfeedIgnor
-0000ff20: 6549 7465 6d54 7970 6528 456e 756d 293a  eItemType(Enum):
-0000ff30: 0a09 504f 5354 5f4f 4e5f 5448 455f 5741  ..POST_ON_THE_WA
-0000ff40: 4c4c 203d 2022 7761 6c6c 220a 0954 4147  LL = "wall"..TAG
-0000ff50: 5f4f 4e5f 415f 5048 4f54 4f20 3d20 2274  _ON_A_PHOTO = "t
-0000ff60: 6167 220a 0950 524f 4649 4c45 5f50 484f  ag"..PROFILE_PHO
-0000ff70: 544f 203d 2022 7072 6f66 696c 6570 686f  TO = "profilepho
-0000ff80: 746f 220a 0956 4944 454f 203d 2022 7669  to"..VIDEO = "vi
-0000ff90: 6465 6f22 0a09 5048 4f54 4f20 3d20 2270  deo"..PHOTO = "p
-0000ffa0: 686f 746f 220a 0941 5544 494f 203d 2022  hoto"..AUDIO = "
-0000ffb0: 6175 6469 6f22 0a0a 636c 6173 7320 4e65  audio"..class Ne
-0000ffc0: 7773 6665 6564 4974 656d 5761 6c6c 706f  wsfeedItemWallpo
-0000ffd0: 7374 4665 6564 6261 636b 5479 7065 2845  stFeedbackType(E
-0000ffe0: 6e75 6d29 3a0a 0942 5554 544f 4e53 203d  num):..BUTTONS =
-0000fff0: 2022 6275 7474 6f6e 7322 0a09 5354 4152   "buttons"..STAR
-00010000: 5320 3d20 2273 7461 7273 220a 0a63 6c61  S = "stars"..cla
-00010010: 7373 204e 6577 7366 6565 644e 6577 7366  ss NewsfeedNewsf
-00010020: 6565 6449 7465 6d54 7970 6528 456e 756d  eedItemType(Enum
-00010030: 293a 0a09 504f 5354 203d 2022 706f 7374  ):..POST = "post
-00010040: 220a 0950 484f 544f 203d 2022 7068 6f74  "..PHOTO = "phot
-00010050: 6f22 0a09 5048 4f54 4f5f 5441 4720 3d20  o"..PHOTO_TAG = 
-00010060: 2270 686f 746f 5f74 6167 220a 0957 414c  "photo_tag"..WAL
-00010070: 4c5f 5048 4f54 4f20 3d20 2277 616c 6c5f  L_PHOTO = "wall_
-00010080: 7068 6f74 6f22 0a09 4652 4945 4e44 203d  photo"..FRIEND =
-00010090: 2022 6672 6965 6e64 220a 0941 5544 494f   "friend"..AUDIO
-000100a0: 203d 2022 6175 6469 6f22 0a09 5649 4445   = "audio"..VIDE
-000100b0: 4f20 3d20 2276 6964 656f 220a 0954 4f50  O = "video"..TOP
-000100c0: 4943 203d 2022 746f 7069 6322 0a09 4449  IC = "topic"..DI
-000100d0: 4745 5354 203d 2022 6469 6765 7374 220a  GEST = "digest".
-000100e0: 0953 544f 5249 4553 203d 2022 7374 6f72  .STORIES = "stor
-000100f0: 6965 7322 0a09 4e4f 5445 203d 2022 6e6f  ies"..NOTE = "no
-00010100: 7465 220a 0941 5544 494f 5f50 4c41 594c  te"..AUDIO_PLAYL
-00010110: 4953 5420 3d20 2261 7564 696f 5f70 6c61  IST = "audio_pla
-00010120: 796c 6973 7422 0a09 434c 4950 203d 2022  ylist"..CLIP = "
-00010130: 636c 6970 220a 0a63 6c61 7373 204e 6577  clip"..class New
-00010140: 7366 6565 6449 7465 6d41 7564 696f 4175  sfeedItemAudioAu
-00010150: 6469 6f28 424d 293a 0a09 636f 756e 743a  dio(BM):..count:
-00010160: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00010170: 4e6f 6e65 0a09 6974 656d 733a 4f70 7469  None..items:Opti
-00010180: 6f6e 616c 5b6c 6973 745b 2241 7564 696f  onal[list["Audio
-00010190: 4175 6469 6f22 5d5d 203d 204e 6f6e 650a  Audio"]] = None.
-000101a0: 0a0a 636c 6173 7320 4e65 7773 6665 6564  ..class Newsfeed
-000101b0: 4974 656d 4261 7365 2842 4d29 3a0a 0974  ItemBase(BM):..t
-000101c0: 7970 653a 224e 6577 7366 6565 644e 6577  ype:"NewsfeedNew
-000101d0: 7366 6565 6449 7465 6d54 7970 6522 0a09  sfeedItemType"..
-000101e0: 736f 7572 6365 5f69 643a 696e 740a 0964  source_id:int..d
-000101f0: 6174 653a 696e 740a 0a0a 636c 6173 7320  ate:int...class 
-00010200: 4e65 7773 6665 6564 4974 656d 4469 6765  NewsfeedItemDige
-00010210: 7374 4275 7474 6f6e 2842 4d29 3a0a 0974  stButton(BM):..t
-00010220: 6974 6c65 3a73 7472 0a09 7374 796c 653a  itle:str..style:
-00010230: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00010240: 4e6f 6e65 0a0a 0a63 6c61 7373 204e 6577  None...class New
-00010250: 7366 6565 6449 7465 6d44 6967 6573 7446  sfeedItemDigestF
-00010260: 6f6f 7465 7228 424d 293a 0a09 7374 796c  ooter(BM):..styl
-00010270: 653a 7374 720a 0974 6578 743a 7374 720a  e:str..text:str.
-00010280: 0962 7574 746f 6e3a 4f70 7469 6f6e 616c  .button:Optional
-00010290: 5b22 4e65 7773 6665 6564 4974 656d 4469  ["NewsfeedItemDi
-000102a0: 6765 7374 4275 7474 6f6e 225d 203d 204e  gestButton"] = N
-000102b0: 6f6e 650a 0a0a 636c 6173 7320 4e65 7773  one...class News
-000102c0: 6665 6564 4974 656d 4469 6765 7374 4675  feedItemDigestFu
-000102d0: 6c6c 4974 656d 2842 4d29 3a0a 0974 6578  llItem(BM):..tex
-000102e0: 743a 4f70 7469 6f6e 616c 5b73 7472 5d20  t:Optional[str] 
-000102f0: 3d20 4e6f 6e65 0a09 736f 7572 6365 5f6e  = None..source_n
-00010300: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
-00010310: 5d20 3d20 4e6f 6e65 0a09 6174 7461 6368  ] = None..attach
-00010320: 6d65 6e74 5f69 6e64 6578 3a4f 7074 696f  ment_index:Optio
-00010330: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00010340: 0961 7474 6163 686d 656e 743a 4f70 7469  .attachment:Opti
-00010350: 6f6e 616c 5b22 5761 6c6c 5761 6c6c 706f  onal["WallWallpo
-00010360: 7374 4174 7461 6368 6d65 6e74 225d 203d  stAttachment"] =
-00010370: 204e 6f6e 650a 0973 7479 6c65 3a4f 7074   None..style:Opt
-00010380: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00010390: 650a 0970 6f73 743a 2257 616c 6c57 616c  e..post:"WallWal
-000103a0: 6c70 6f73 7422 0a0a 0a63 6c61 7373 204e  lpost"...class N
-000103b0: 6577 7366 6565 6449 7465 6d44 6967 6573  ewsfeedItemDiges
-000103c0: 7448 6561 6465 7228 424d 293a 0a09 7469  tHeader(BM):..ti
-000103d0: 746c 653a 7374 720a 0973 7562 7469 746c  tle:str..subtitl
-000103e0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-000103f0: 3d20 4e6f 6e65 0a09 7374 796c 653a 7374  = None..style:st
-00010400: 720a 0962 7574 746f 6e3a 4f70 7469 6f6e  r..button:Option
-00010410: 616c 5b22 4e65 7773 6665 6564 4974 656d  al["NewsfeedItem
-00010420: 4469 6765 7374 4275 7474 6f6e 225d 203d  DigestButton"] =
-00010430: 204e 6f6e 650a 0a0a 636c 6173 7320 4e65   None...class Ne
-00010440: 7773 6665 6564 4974 656d 4469 6765 7374  wsfeedItemDigest
-00010450: 4974 656d 2842 4d29 3a0a 0970 6173 730a  Item(BM):..pass.
-00010460: 0a63 6c61 7373 204e 6577 7366 6565 6449  .class NewsfeedI
-00010470: 7465 6d46 7269 656e 6446 7269 656e 6473  temFriendFriends
-00010480: 2842 4d29 3a0a 0963 6f75 6e74 3a4f 7074  (BM):..count:Opt
-00010490: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-000104a0: 650a 0969 7465 6d73 3a4f 7074 696f 6e61  e..items:Optiona
-000104b0: 6c5b 6c69 7374 5b22 4261 7365 5573 6572  l[list["BaseUser
-000104c0: 4964 225d 5d20 3d20 4e6f 6e65 0a0a 0a63  Id"]] = None...c
-000104d0: 6c61 7373 204e 6577 7366 6565 6449 7465  lass NewsfeedIte
-000104e0: 6d48 6f6c 6964 6179 5265 636f 6d6d 656e  mHolidayRecommen
-000104f0: 6461 7469 6f6e 7342 6c6f 636b 4865 6164  dationsBlockHead
-00010500: 6572 2842 4d29 3a0a 0974 6974 6c65 3a4f  er(BM):..title:O
-00010510: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00010520: 6f6e 650a 0973 7562 7469 746c 653a 4f70  one..subtitle:Op
-00010530: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00010540: 6e65 0a09 696d 6167 653a 4f70 7469 6f6e  ne..image:Option
-00010550: 616c 5b6c 6973 745b 2242 6173 6549 6d61  al[list["BaseIma
-00010560: 6765 225d 5d20 3d20 4e6f 6e65 0a09 6163  ge"]] = None..ac
-00010570: 7469 6f6e 3a4f 7074 696f 6e61 6c5b 2242  tion:Optional["B
-00010580: 6173 654c 696e 6b42 7574 746f 6e41 6374  aseLinkButtonAct
-00010590: 696f 6e22 5d20 3d20 4e6f 6e65 0a0a 0a63  ion"] = None...c
-000105a0: 6c61 7373 204e 6577 7366 6565 6449 7465  lass NewsfeedIte
-000105b0: 6d50 686f 746f 5068 6f74 6f73 2842 4d29  mPhotoPhotos(BM)
-000105c0: 3a0a 0963 6f75 6e74 3a4f 7074 696f 6e61  :..count:Optiona
-000105d0: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
-000105e0: 7465 6d73 3a4f 7074 696f 6e61 6c5b 6c69  tems:Optional[li
-000105f0: 7374 5b22 4e65 7773 6665 6564 4e65 7773  st["NewsfeedNews
-00010600: 6665 6564 5068 6f74 6f22 5d5d 203d 204e  feedPhoto"]] = N
-00010610: 6f6e 650a 0a0a 636c 6173 7320 4e65 7773  one...class News
-00010620: 6665 6564 4974 656d 5068 6f74 6f54 6167  feedItemPhotoTag
-00010630: 5068 6f74 6f54 6167 7328 424d 293a 0a09  PhotoTags(BM):..
-00010640: 636f 756e 743a 4f70 7469 6f6e 616c 5b69  count:Optional[i
-00010650: 6e74 5d20 3d20 4e6f 6e65 0a09 6974 656d  nt] = None..item
-00010660: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-00010670: 224e 6577 7366 6565 644e 6577 7366 6565  "NewsfeedNewsfee
-00010680: 6450 686f 746f 225d 5d20 3d20 4e6f 6e65  dPhoto"]] = None
-00010690: 0a0a 0a63 6c61 7373 204e 6577 7366 6565  ...class Newsfee
-000106a0: 6449 7465 6d50 726f 6d6f 4275 7474 6f6e  dItemPromoButton
-000106b0: 4163 7469 6f6e 2842 4d29 3a0a 0975 726c  Action(BM):..url
-000106c0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-000106d0: 204e 6f6e 650a 0974 7970 653a 4f70 7469   None..type:Opti
-000106e0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-000106f0: 0a09 7461 7267 6574 3a4f 7074 696f 6e61  ..target:Optiona
-00010700: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
-00010710: 636c 6173 7320 4e65 7773 6665 6564 4974  class NewsfeedIt
-00010720: 656d 5072 6f6d 6f42 7574 746f 6e49 6d61  emPromoButtonIma
-00010730: 6765 2842 4d29 3a0a 0977 6964 7468 3a4f  ge(BM):..width:O
-00010740: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00010750: 6f6e 650a 0968 6569 6768 743a 4f70 7469  one..height:Opti
-00010760: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00010770: 0a09 7572 6c3a 4f70 7469 6f6e 616c 5b73  ..url:Optional[s
-00010780: 7472 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  tr] = None...cla
-00010790: 7373 204e 6577 7366 6565 6449 7465 6d56  ss NewsfeedItemV
-000107a0: 6964 656f 5669 6465 6f28 424d 293a 0a09  ideoVideo(BM):..
-000107b0: 636f 756e 743a 4f70 7469 6f6e 616c 5b69  count:Optional[i
-000107c0: 6e74 5d20 3d20 4e6f 6e65 0a09 6974 656d  nt] = None..item
-000107d0: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-000107e0: 2256 6964 656f 5669 6465 6f22 5d5d 203d  "VideoVideo"]] =
-000107f0: 204e 6f6e 650a 0a0a 636c 6173 7320 4e65   None...class Ne
-00010800: 7773 6665 6564 4974 656d 5761 6c6c 706f  wsfeedItemWallpo
-00010810: 7374 4665 6564 6261 636b 2842 4d29 3a0a  stFeedback(BM):.
-00010820: 0974 7970 653a 224e 6577 7366 6565 6449  .type:"NewsfeedI
-00010830: 7465 6d57 616c 6c70 6f73 7446 6565 6462  temWallpostFeedb
-00010840: 6163 6b54 7970 6522 0a09 7175 6573 7469  ackType"..questi
-00010850: 6f6e 3a73 7472 0a09 616e 7377 6572 733a  on:str..answers:
-00010860: 4f70 7469 6f6e 616c 5b6c 6973 745b 224e  Optional[list["N
-00010870: 6577 7366 6565 6449 7465 6d57 616c 6c70  ewsfeedItemWallp
-00010880: 6f73 7446 6565 6462 6163 6b41 6e73 7765  ostFeedbackAnswe
-00010890: 7222 5d5d 203d 204e 6f6e 650a 0973 7461  r"]] = None..sta
-000108a0: 7273 5f63 6f75 6e74 3a4f 7074 696f 6e61  rs_count:Optiona
-000108b0: 6c5b 696e 745d 203d 204e 6f6e 650a 0967  l[int] = None..g
-000108c0: 7261 7469 7475 6465 3a4f 7074 696f 6e61  ratitude:Optiona
-000108d0: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
-000108e0: 636c 6173 7320 4e65 7773 6665 6564 4974  class NewsfeedIt
-000108f0: 656d 5761 6c6c 706f 7374 4665 6564 6261  emWallpostFeedba
-00010900: 636b 416e 7377 6572 2842 4d29 3a0a 0974  ckAnswer(BM):..t
-00010910: 6974 6c65 3a73 7472 0a09 6964 3a73 7472  itle:str..id:str
-00010920: 0a0a 0a63 6c61 7373 204e 6577 7366 6565  ...class Newsfee
-00010930: 644c 6973 7428 424d 293a 0a09 6964 3a69  dList(BM):..id:i
-00010940: 6e74 0a09 7469 746c 653a 7374 720a 0a0a  nt..title:str...
-00010950: 636c 6173 7320 4e65 7773 6665 6564 4e65  class NewsfeedNe
-00010960: 7773 6665 6564 4974 656d 2842 4d29 3a0a  wsfeedItem(BM):.
-00010970: 0970 6173 730a 0a0a 0a63 6c61 7373 204e  .pass....class N
-00010980: 6f74 6573 4e6f 7465 2842 4d29 3a0a 0972  otesNote(BM):..r
-00010990: 6561 645f 636f 6d6d 656e 7473 3a4f 7074  ead_comments:Opt
-000109a0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-000109b0: 650a 0963 616e 5f63 6f6d 6d65 6e74 3a4f  e..can_comment:O
-000109c0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-000109d0: 4e6f 6e65 0a09 636f 6d6d 656e 7473 3a69  None..comments:i
-000109e0: 6e74 0a09 6461 7465 3a69 6e74 0a09 6964  nt..date:int..id
-000109f0: 3a69 6e74 0a09 6f77 6e65 725f 6964 3a69  :int..owner_id:i
-00010a00: 6e74 0a09 7465 7874 3a4f 7074 696f 6e61  nt..text:Optiona
-00010a10: 6c5b 7374 725d 203d 204e 6f6e 650a 0974  l[str] = None..t
-00010a20: 6578 745f 7769 6b69 3a4f 7074 696f 6e61  ext_wiki:Optiona
-00010a30: 6c5b 7374 725d 203d 204e 6f6e 650a 0974  l[str] = None..t
-00010a40: 6974 6c65 3a73 7472 0a09 7669 6577 5f75  itle:str..view_u
-00010a50: 726c 3a73 7472 0a09 7072 6976 6163 795f  rl:str..privacy_
-00010a60: 7669 6577 3a4f 7074 696f 6e61 6c5b 6c69  view:Optional[li
-00010a70: 7374 5b73 7472 5d5d 203d 204e 6f6e 650a  st[str]] = None.
-00010a80: 0970 7269 7661 6379 5f63 6f6d 6d65 6e74  .privacy_comment
-00010a90: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b73  :Optional[list[s
-00010aa0: 7472 5d5d 203d 204e 6f6e 650a 0a0a 636c  tr]] = None...cl
-00010ab0: 6173 7320 4e6f 7465 734e 6f74 6543 6f6d  ass NotesNoteCom
-00010ac0: 6d65 6e74 2842 4d29 3a0a 0964 6174 653a  ment(BM):..date:
-00010ad0: 696e 740a 0969 643a 696e 740a 096d 6573  int..id:int..mes
-00010ae0: 7361 6765 3a73 7472 0a09 6e69 643a 696e  sage:str..nid:in
-00010af0: 740a 096f 6964 3a69 6e74 0a09 7265 706c  t..oid:int..repl
-00010b00: 795f 746f 3a4f 7074 696f 6e61 6c5b 696e  y_to:Optional[in
-00010b10: 745d 203d 204e 6f6e 650a 0975 6964 3a69  t] = None..uid:i
-00010b20: 6e74 0a0a 0a0a 0a63 6c61 7373 204e 6f74  nt.....class Not
-00010b30: 6966 6963 6174 696f 6e73 4665 6564 6261  ificationsFeedba
-00010b40: 636b 2842 4d29 3a0a 0961 7474 6163 686d  ck(BM):..attachm
-00010b50: 656e 7473 3a4f 7074 696f 6e61 6c5b 6c69  ents:Optional[li
-00010b60: 7374 5b22 5761 6c6c 5761 6c6c 706f 7374  st["WallWallpost
-00010b70: 4174 7461 6368 6d65 6e74 225d 5d20 3d20  Attachment"]] = 
-00010b80: 4e6f 6e65 0a09 6672 6f6d 5f69 643a 4f70  None..from_id:Op
-00010b90: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00010ba0: 6e65 0a09 6765 6f3a 4f70 7469 6f6e 616c  ne..geo:Optional
-00010bb0: 5b22 4261 7365 4765 6f22 5d20 3d20 4e6f  ["BaseGeo"] = No
-00010bc0: 6e65 0a09 6964 3a4f 7074 696f 6e61 6c5b  ne..id:Optional[
-00010bd0: 696e 745d 203d 204e 6f6e 650a 096c 696b  int] = None..lik
-00010be0: 6573 3a4f 7074 696f 6e61 6c5b 2242 6173  es:Optional["Bas
-00010bf0: 654c 696b 6573 496e 666f 225d 203d 204e  eLikesInfo"] = N
-00010c00: 6f6e 650a 0974 6578 743a 4f70 7469 6f6e  one..text:Option
-00010c10: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00010c20: 746f 5f69 643a 4f70 7469 6f6e 616c 5b69  to_id:Optional[i
-00010c30: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  nt] = None...cla
-00010c40: 7373 204e 6f74 6966 6963 6174 696f 6e73  ss Notifications
-00010c50: 4e6f 7469 6669 6361 7469 6f6e 2842 4d29  Notification(BM)
-00010c60: 3a0a 0964 6174 653a 4f70 7469 6f6e 616c  :..date:Optional
-00010c70: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6665  [int] = None..fe
-00010c80: 6564 6261 636b 3a4f 7074 696f 6e61 6c5b  edback:Optional[
-00010c90: 224e 6f74 6966 6963 6174 696f 6e73 4665  "NotificationsFe
-00010ca0: 6564 6261 636b 225d 203d 204e 6f6e 650a  edback"] = None.
-00010cb0: 0970 6172 656e 743a 4f70 7469 6f6e 616c  .parent:Optional
-00010cc0: 5b22 4e6f 7469 6669 6361 7469 6f6e 734e  ["NotificationsN
-00010cd0: 6f74 6966 6963 6174 696f 6e22 5d20 3d20  otification"] = 
-00010ce0: 4e6f 6e65 0a09 7265 706c 793a 4f70 7469  None..reply:Opti
-00010cf0: 6f6e 616c 5b22 4e6f 7469 6669 6361 7469  onal["Notificati
-00010d00: 6f6e 7352 6570 6c79 225d 203d 204e 6f6e  onsReply"] = Non
-00010d10: 650a 0974 7970 653a 4f70 7469 6f6e 616c  e..type:Optional
-00010d20: 5b73 7472 5d20 3d20 4e6f 6e65 0a0a 0a63  [str] = None...c
-00010d30: 6c61 7373 204e 6f74 6966 6963 6174 696f  lass Notificatio
-00010d40: 6e73 4e6f 7469 6669 6361 7469 6f6e 4974  nsNotificationIt
-00010d50: 656d 2842 4d29 3a0a 0970 6173 730a 0a63  em(BM):..pass..c
-00010d60: 6c61 7373 204e 6f74 6966 6963 6174 696f  lass Notificatio
-00010d70: 6e73 4e6f 7469 6669 6361 7469 6f6e 7343  nsNotificationsC
-00010d80: 6f6d 6d65 6e74 2842 4d29 3a0a 0964 6174  omment(BM):..dat
-00010d90: 653a 4f70 7469 6f6e 616c 5b69 6e74 5d20  e:Optional[int] 
-00010da0: 3d20 4e6f 6e65 0a09 6964 3a4f 7074 696f  = None..id:Optio
-00010db0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00010dc0: 096f 776e 6572 5f69 643a 4f70 7469 6f6e  .owner_id:Option
-00010dd0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00010de0: 7068 6f74 6f3a 4f70 7469 6f6e 616c 5b22  photo:Optional["
-00010df0: 5068 6f74 6f73 5068 6f74 6f22 5d20 3d20  PhotosPhoto"] = 
-00010e00: 4e6f 6e65 0a09 706f 7374 3a4f 7074 696f  None..post:Optio
-00010e10: 6e61 6c5b 2257 616c 6c57 616c 6c70 6f73  nal["WallWallpos
-00010e20: 7422 5d20 3d20 4e6f 6e65 0a09 7465 7874  t"] = None..text
-00010e30: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00010e40: 204e 6f6e 650a 0974 6f70 6963 3a4f 7074   None..topic:Opt
-00010e50: 696f 6e61 6c5b 2242 6f61 7264 546f 7069  ional["BoardTopi
-00010e60: 6322 5d20 3d20 4e6f 6e65 0a09 7669 6465  c"] = None..vide
-00010e70: 6f3a 4f70 7469 6f6e 616c 5b22 5669 6465  o:Optional["Vide
-00010e80: 6f56 6964 656f 225d 203d 204e 6f6e 650a  oVideo"] = None.
-00010e90: 0a0a 636c 6173 7320 4e6f 7469 6669 6361  ..class Notifica
-00010ea0: 7469 6f6e 7352 6570 6c79 2842 4d29 3a0a  tionsReply(BM):.
-00010eb0: 0964 6174 653a 4f70 7469 6f6e 616c 5b69  .date:Optional[i
-00010ec0: 6e74 5d20 3d20 4e6f 6e65 0a09 6964 3a4f  nt] = None..id:O
-00010ed0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00010ee0: 6f6e 650a 0974 6578 743a 4f70 7469 6f6e  one..text:Option
-00010ef0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
-00010f00: 0a63 6c61 7373 204e 6f74 6966 6963 6174  .class Notificat
-00010f10: 696f 6e73 5365 6e64 4d65 7373 6167 6545  ionsSendMessageE
-00010f20: 7272 6f72 2842 4d29 3a0a 0963 6f64 653a  rror(BM):..code:
-00010f30: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00010f40: 4e6f 6e65 0a09 6465 7363 7269 7074 696f  None..descriptio
-00010f50: 6e3a 4f70 7469 6f6e 616c 5b73 7472 5d20  n:Optional[str] 
-00010f60: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204e  = None...class N
-00010f70: 6f74 6966 6963 6174 696f 6e73 5365 6e64  otificationsSend
-00010f80: 4d65 7373 6167 6549 7465 6d28 424d 293a  MessageItem(BM):
-00010f90: 0a09 7573 6572 5f69 643a 4f70 7469 6f6e  ..user_id:Option
-00010fa0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00010fb0: 7374 6174 7573 3a4f 7074 696f 6e61 6c5b  status:Optional[
-00010fc0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6572  bool] = None..er
-00010fd0: 726f 723a 4f70 7469 6f6e 616c 5b22 4e6f  ror:Optional["No
-00010fe0: 7469 6669 6361 7469 6f6e 7353 656e 644d  tificationsSendM
-00010ff0: 6573 7361 6765 4572 726f 7222 5d20 3d20  essageError"] = 
-00011000: 4e6f 6e65 0a0a 0a0a 0a63 6c61 7373 204f  None.....class O
-00011010: 6175 7468 4572 726f 7228 424d 293a 0a09  authError(BM):..
-00011020: 6572 726f 723a 7374 720a 0965 7272 6f72  error:str..error
-00011030: 5f64 6573 6372 6970 7469 6f6e 3a73 7472  _description:str
-00011040: 0a09 7265 6469 7265 6374 5f75 7269 3a4f  ..redirect_uri:O
-00011050: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00011060: 6f6e 650a 0a0a 0a0a 636c 6173 7320 4f72  one.....class Or
-00011070: 6465 7273 416d 6f75 6e74 2842 4d29 3a0a  dersAmount(BM):.
-00011080: 0961 6d6f 756e 7473 3a4f 7074 696f 6e61  .amounts:Optiona
-00011090: 6c5b 6c69 7374 5b22 4f72 6465 7273 416d  l[list["OrdersAm
-000110a0: 6f75 6e74 4974 656d 225d 5d20 3d20 4e6f  ountItem"]] = No
-000110b0: 6e65 0a09 6375 7272 656e 6379 3a4f 7074  ne..currency:Opt
-000110c0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-000110d0: 650a 0a0a 636c 6173 7320 4f72 6465 7273  e...class Orders
-000110e0: 416d 6f75 6e74 4974 656d 2842 4d29 3a0a  AmountItem(BM):.
-000110f0: 0961 6d6f 756e 743a 4f70 7469 6f6e 616c  .amount:Optional
-00011100: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6465  [int] = None..de
-00011110: 7363 7269 7074 696f 6e3a 4f70 7469 6f6e  scription:Option
-00011120: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00011130: 766f 7465 733a 4f70 7469 6f6e 616c 5b73  votes:Optional[s
-00011140: 7472 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  tr] = None...cla
-00011150: 7373 204f 7264 6572 734f 7264 6572 2842  ss OrdersOrder(B
-00011160: 4d29 3a0a 0961 6d6f 756e 743a 7374 720a  M):..amount:str.
-00011170: 0961 7070 5f6f 7264 6572 5f69 643a 7374  .app_order_id:st
-00011180: 720a 0963 616e 6365 6c5f 7472 616e 7361  r..cancel_transa
-00011190: 6374 696f 6e5f 6964 3a4f 7074 696f 6e61  ction_id:Optiona
-000111a0: 6c5b 7374 725d 203d 204e 6f6e 650a 0964  l[str] = None..d
-000111b0: 6174 653a 7374 720a 0969 643a 7374 720a  ate:str..id:str.
-000111c0: 0969 7465 6d3a 7374 720a 0972 6563 6569  .item:str..recei
-000111d0: 7665 725f 6964 3a73 7472 0a09 7374 6174  ver_id:str..stat
-000111e0: 7573 3a73 7472 0a09 7472 616e 7361 6374  us:str..transact
-000111f0: 696f 6e5f 6964 3a4f 7074 696f 6e61 6c5b  ion_id:Optional[
-00011200: 7374 725d 203d 204e 6f6e 650a 0975 7365  str] = None..use
-00011210: 725f 6964 3a73 7472 0a0a 0a63 6c61 7373  r_id:str...class
-00011220: 204f 7264 6572 7353 7562 7363 7269 7074   OrdersSubscript
-00011230: 696f 6e28 424d 293a 0a09 6361 6e63 656c  ion(BM):..cancel
-00011240: 5f72 6561 736f 6e3a 4f70 7469 6f6e 616c  _reason:Optional
-00011250: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6372  [str] = None..cr
-00011260: 6561 7465 5f74 696d 653a 696e 740a 0969  eate_time:int..i
-00011270: 643a 696e 740a 0969 7465 6d5f 6964 3a73  d:int..item_id:s
-00011280: 7472 0a09 6e65 7874 5f62 696c 6c5f 7469  tr..next_bill_ti
-00011290: 6d65 3a4f 7074 696f 6e61 6c5b 696e 745d  me:Optional[int]
-000112a0: 203d 204e 6f6e 650a 0965 7870 6972 655f   = None..expire_
-000112b0: 7469 6d65 3a4f 7074 696f 6e61 6c5b 696e  time:Optional[in
-000112c0: 745d 203d 204e 6f6e 650a 0970 656e 6469  t] = None..pendi
-000112d0: 6e67 5f63 616e 6365 6c3a 4f70 7469 6f6e  ng_cancel:Option
-000112e0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-000112f0: 0970 6572 696f 643a 696e 740a 0970 6572  .period:int..per
-00011300: 696f 645f 7374 6172 745f 7469 6d65 3a69  iod_start_time:i
-00011310: 6e74 0a09 7072 6963 653a 696e 740a 0974  nt..price:int..t
-00011320: 6974 6c65 3a4f 7074 696f 6e61 6c5b 7374  itle:Optional[st
-00011330: 725d 203d 204e 6f6e 650a 0961 7070 5f69  r] = None..app_i
-00011340: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-00011350: 3d20 4e6f 6e65 0a09 6170 706c 6963 6174  = None..applicat
-00011360: 696f 6e5f 6e61 6d65 3a4f 7074 696f 6e61  ion_name:Optiona
-00011370: 6c5b 7374 725d 203d 204e 6f6e 650a 0970  l[str] = None..p
-00011380: 686f 746f 5f75 726c 3a4f 7074 696f 6e61  hoto_url:Optiona
-00011390: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
-000113a0: 7461 7475 733a 7374 720a 0974 6573 745f  tatus:str..test_
-000113b0: 6d6f 6465 3a4f 7074 696f 6e61 6c5b 626f  mode:Optional[bo
-000113c0: 6f6c 5d20 3d20 4e6f 6e65 0a09 7472 6961  ol] = None..tria
-000113d0: 6c5f 6578 7069 7265 5f74 696d 653a 4f70  l_expire_time:Op
-000113e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000113f0: 6e65 0a09 7570 6461 7465 5f74 696d 653a  ne..update_time:
-00011400: 696e 740a 0a0a 0a0a 636c 6173 7320 4f77  int.....class Ow
-00011410: 6e65 7253 7461 7465 2842 4d29 3a0a 0973  nerState(BM):..s
-00011420: 7461 7465 3a4f 7074 696f 6e61 6c5b 696e  tate:Optional[in
-00011430: 745d 203d 204e 6f6e 650a 0964 6573 6372  t] = None..descr
-00011440: 6970 7469 6f6e 3a4f 7074 696f 6e61 6c5b  iption:Optional[
-00011450: 7374 725d 203d 204e 6f6e 650a 0a0a 0a0a  str] = None.....
-00011460: 636c 6173 7320 5061 6765 7350 7269 7661  class PagesPriva
-00011470: 6379 5365 7474 696e 6773 2845 6e75 6d29  cySettings(Enum)
-00011480: 3a0a 0943 4f4d 4d55 4e49 5459 5f4d 414e  :..COMMUNITY_MAN
-00011490: 4147 4552 535f 4f4e 4c59 203d 2030 0a09  AGERS_ONLY = 0..
-000114a0: 434f 4d4d 554e 4954 595f 4d45 4d42 4552  COMMUNITY_MEMBER
-000114b0: 535f 4f4e 4c59 203d 2031 0a09 4556 4552  S_ONLY = 1..EVER
-000114c0: 594f 4e45 203d 2032 0a0a 636c 6173 7320  YONE = 2..class 
-000114d0: 5061 6765 7357 696b 6970 6167 6528 424d  PagesWikipage(BM
-000114e0: 293a 0a09 6372 6561 746f 725f 6964 3a4f  ):..creator_id:O
-000114f0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00011500: 6f6e 650a 0963 7265 6174 6f72 5f6e 616d  one..creator_nam
-00011510: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-00011520: 3d20 4e6f 6e65 0a09 6564 6974 6f72 5f69  = None..editor_i
-00011530: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-00011540: 3d20 4e6f 6e65 0a09 6564 6974 6f72 5f6e  = None..editor_n
-00011550: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
-00011560: 5d20 3d20 4e6f 6e65 0a09 6772 6f75 705f  ] = None..group_
-00011570: 6964 3a69 6e74 0a09 6964 3a69 6e74 0a09  id:int..id:int..
-00011580: 7469 746c 653a 7374 720a 0976 6965 7773  title:str..views
-00011590: 3a69 6e74 0a09 7768 6f5f 6361 6e5f 6564  :int..who_can_ed
-000115a0: 6974 3a22 5061 6765 7350 7269 7661 6379  it:"PagesPrivacy
-000115b0: 5365 7474 696e 6773 220a 0977 686f 5f63  Settings"..who_c
-000115c0: 616e 5f76 6965 773a 2250 6167 6573 5072  an_view:"PagesPr
-000115d0: 6976 6163 7953 6574 7469 6e67 7322 0a0a  ivacySettings"..
-000115e0: 0a63 6c61 7373 2050 6167 6573 5769 6b69  .class PagesWiki
-000115f0: 7061 6765 4675 6c6c 2842 4d29 3a0a 0963  pageFull(BM):..c
-00011600: 7265 6174 6564 3a69 6e74 0a09 6372 6561  reated:int..crea
-00011610: 746f 725f 6964 3a4f 7074 696f 6e61 6c5b  tor_id:Optional[
-00011620: 696e 745d 203d 204e 6f6e 650a 0963 7572  int] = None..cur
-00011630: 7265 6e74 5f75 7365 725f 6361 6e5f 6564  rent_user_can_ed
-00011640: 6974 3a4f 7074 696f 6e61 6c5b 626f 6f6c  it:Optional[bool
-00011650: 5d20 3d20 4e6f 6e65 0a09 6375 7272 656e  ] = None..curren
-00011660: 745f 7573 6572 5f63 616e 5f65 6469 745f  t_user_can_edit_
-00011670: 6163 6365 7373 3a4f 7074 696f 6e61 6c5b  access:Optional[
-00011680: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6564  bool] = None..ed
-00011690: 6974 6564 3a69 6e74 0a09 6564 6974 6f72  ited:int..editor
-000116a0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-000116b0: 5d20 3d20 4e6f 6e65 0a09 6772 6f75 705f  ] = None..group_
-000116c0: 6964 3a69 6e74 0a09 6874 6d6c 3a4f 7074  id:int..html:Opt
-000116d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-000116e0: 650a 0969 643a 696e 740a 0973 6f75 7263  e..id:int..sourc
-000116f0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-00011700: 3d20 4e6f 6e65 0a09 7469 746c 653a 7374  = None..title:st
-00011710: 720a 0976 6965 775f 7572 6c3a 7374 720a  r..view_url:str.
-00011720: 0976 6965 7773 3a69 6e74 0a09 7768 6f5f  .views:int..who_
-00011730: 6361 6e5f 6564 6974 3a22 5061 6765 7350  can_edit:"PagesP
-00011740: 7269 7661 6379 5365 7474 696e 6773 220a  rivacySettings".
-00011750: 0977 686f 5f63 616e 5f76 6965 773a 2250  .who_can_view:"P
-00011760: 6167 6573 5072 6976 6163 7953 6574 7469  agesPrivacySetti
-00011770: 6e67 7322 0a09 7572 6c3a 4f70 7469 6f6e  ngs"..url:Option
-00011780: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00011790: 7061 7265 6e74 3a4f 7074 696f 6e61 6c5b  parent:Optional[
-000117a0: 7374 725d 203d 204e 6f6e 650a 0970 6172  str] = None..par
-000117b0: 656e 7432 3a4f 7074 696f 6e61 6c5b 7374  ent2:Optional[st
-000117c0: 725d 203d 204e 6f6e 650a 096f 776e 6572  r] = None..owner
-000117d0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-000117e0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
-000117f0: 2050 6167 6573 5769 6b69 7061 6765 4869   PagesWikipageHi
-00011800: 7374 6f72 7928 424d 293a 0a09 6964 3a69  story(BM):..id:i
-00011810: 6e74 0a09 6c65 6e67 7468 3a69 6e74 0a09  nt..length:int..
-00011820: 6461 7465 3a69 6e74 0a09 6564 6974 6f72  date:int..editor
-00011830: 5f69 643a 696e 740a 0965 6469 746f 725f  _id:int..editor_
-00011840: 6e61 6d65 3a73 7472 0a0a 0a0a 0a63 6c61  name:str.....cla
-00011850: 7373 2050 686f 746f 7349 6d61 6765 5479  ss PhotosImageTy
-00011860: 7065 2845 6e75 6d29 3a0a 0953 203d 2022  pe(Enum):..S = "
-00011870: 7322 0a09 4d20 3d20 226d 220a 0958 203d  s"..M = "m"..X =
-00011880: 2022 7822 0a09 4c20 3d20 226c 220a 094f   "x"..L = "l"..O
-00011890: 203d 2022 6f22 0a09 5020 3d20 2270 220a   = "o"..P = "p".
-000118a0: 0951 203d 2022 7122 0a09 5220 3d20 2272  .Q = "q"..R = "r
-000118b0: 220a 0959 203d 2022 7922 0a09 5a20 3d20  "..Y = "y"..Z = 
-000118c0: 227a 220a 0957 203d 2022 7722 0a0a 636c  "z"..W = "w"..cl
-000118d0: 6173 7320 5068 6f74 6f73 5068 6f74 6f53  ass PhotosPhotoS
-000118e0: 697a 6573 5479 7065 2845 6e75 6d29 3a0a  izesType(Enum):.
-000118f0: 0953 203d 2022 7322 0a09 4d20 3d20 226d  .S = "s"..M = "m
-00011900: 220a 0958 203d 2022 7822 0a09 4f20 3d20  "..X = "x"..O = 
-00011910: 226f 220a 0950 203d 2022 7022 0a09 5120  "o"..P = "p"..Q 
-00011920: 3d20 2271 220a 0952 203d 2022 7222 0a09  = "q"..R = "r"..
-00011930: 4b20 3d20 226b 220a 094c 203d 2022 6c22  K = "k"..L = "l"
-00011940: 0a09 5920 3d20 2279 220a 095a 203d 2022  ..Y = "y"..Z = "
-00011950: 7a22 0a09 4320 3d20 2263 220a 0957 203d  z"..C = "c"..W =
-00011960: 2022 7722 0a09 4120 3d20 2261 220a 0942   "w"..A = "a"..B
-00011970: 203d 2022 6222 0a09 4520 3d20 2265 220a   = "b"..E = "e".
-00011980: 0949 203d 2022 6922 0a09 4420 3d20 2264  .I = "i"..D = "d
-00011990: 220a 094a 203d 2022 6a22 0a09 5445 4d50  "..J = "j"..TEMP
-000119a0: 203d 2022 7465 6d70 220a 0948 203d 2022   = "temp"..H = "
-000119b0: 6822 0a09 4720 3d20 2267 220a 094e 203d  h"..G = "g"..N =
-000119c0: 2022 6e22 0a09 4620 3d20 2266 220a 094d   "n"..F = "f"..M
-000119d0: 4158 203d 2022 6d61 7822 0a0a 636c 6173  AX = "max"..clas
-000119e0: 7320 5068 6f74 6f73 496d 6167 6528 424d  s PhotosImage(BM
-000119f0: 293a 0a09 6865 6967 6874 3a4f 7074 696f  ):..height:Optio
-00011a00: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00011a10: 0974 7970 653a 4f70 7469 6f6e 616c 5b22  .type:Optional["
-00011a20: 5068 6f74 6f73 496d 6167 6554 7970 6522  PhotosImageType"
-00011a30: 5d20 3d20 4e6f 6e65 0a09 7572 6c3a 4f70  ] = None..url:Op
-00011a40: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00011a50: 6e65 0a09 7769 6474 683a 4f70 7469 6f6e  ne..width:Option
-00011a60: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
-00011a70: 0a63 6c61 7373 2050 686f 746f 7350 686f  .class PhotosPho
-00011a80: 746f 2842 4d29 3a0a 0961 6363 6573 735f  to(BM):..access_
-00011a90: 6b65 793a 4f70 7469 6f6e 616c 5b73 7472  key:Optional[str
-00011aa0: 5d20 3d20 4e6f 6e65 0a09 616c 6275 6d5f  ] = None..album_
-00011ab0: 6964 3a69 6e74 0a09 6461 7465 3a69 6e74  id:int..date:int
-00011ac0: 0a09 6865 6967 6874 3a4f 7074 696f 6e61  ..height:Optiona
-00011ad0: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
-00011ae0: 643a 696e 740a 0969 6d61 6765 733a 4f70  d:int..images:Op
-00011af0: 7469 6f6e 616c 5b6c 6973 745b 2250 686f  tional[list["Pho
-00011b00: 746f 7349 6d61 6765 225d 5d20 3d20 4e6f  tosImage"]] = No
-00011b10: 6e65 0a09 6c61 743a 4f70 7469 6f6e 616c  ne..lat:Optional
-00011b20: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6c6f  [int] = None..lo
-00011b30: 6e67 3a4f 7074 696f 6e61 6c5b 696e 745d  ng:Optional[int]
-00011b40: 203d 204e 6f6e 650a 096f 776e 6572 5f69   = None..owner_i
-00011b50: 643a 696e 740a 0970 686f 746f 5f32 3536  d:int..photo_256
-00011b60: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00011b70: 204e 6f6e 650a 0963 616e 5f63 6f6d 6d65   None..can_comme
-00011b80: 6e74 3a4f 7074 696f 6e61 6c5b 626f 6f6c  nt:Optional[bool
-00011b90: 5d20 3d20 4e6f 6e65 0a09 706c 6163 653a  ] = None..place:
-00011ba0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00011bb0: 4e6f 6e65 0a09 706f 7374 5f69 643a 4f70  None..post_id:Op
-00011bc0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00011bd0: 6e65 0a09 7369 7a65 733a 4f70 7469 6f6e  ne..sizes:Option
-00011be0: 616c 5b6c 6973 745b 2250 686f 746f 7350  al[list["PhotosP
-00011bf0: 686f 746f 5369 7a65 7322 5d5d 203d 204e  hotoSizes"]] = N
-00011c00: 6f6e 650a 0974 6578 743a 4f70 7469 6f6e  one..text:Option
-00011c10: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00011c20: 7573 6572 5f69 643a 4f70 7469 6f6e 616c  user_id:Optional
-00011c30: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7769  [int] = None..wi
-00011c40: 6474 683a 4f70 7469 6f6e 616c 5b69 6e74  dth:Optional[int
-00011c50: 5d20 3d20 4e6f 6e65 0a09 6861 735f 7461  ] = None..has_ta
-00011c60: 6773 3a62 6f6f 6c0a 096c 696b 6573 3a4f  gs:bool..likes:O
-00011c70: 7074 696f 6e61 6c5b 2242 6173 654c 696b  ptional["BaseLik
-00011c80: 6573 225d 203d 204e 6f6e 650a 0963 6f6d  es"] = None..com
-00011c90: 6d65 6e74 733a 4f70 7469 6f6e 616c 5b22  ments:Optional["
-00011ca0: 4261 7365 4f62 6a65 6374 436f 756e 7422  BaseObjectCount"
-00011cb0: 5d20 3d20 4e6f 6e65 0a09 7265 706f 7374  ] = None..repost
-00011cc0: 733a 4f70 7469 6f6e 616c 5b22 4261 7365  s:Optional["Base
-00011cd0: 5265 706f 7374 7349 6e66 6f22 5d20 3d20  RepostsInfo"] = 
-00011ce0: 4e6f 6e65 0a09 7461 6773 3a4f 7074 696f  None..tags:Optio
-00011cf0: 6e61 6c5b 2242 6173 654f 626a 6563 7443  nal["BaseObjectC
-00011d00: 6f75 6e74 225d 203d 204e 6f6e 650a 0a0a  ount"] = None...
-00011d10: 636c 6173 7320 5068 6f74 6f73 5068 6f74  class PhotosPhot
-00011d20: 6f41 6c62 756d 2842 4d29 3a0a 0963 7265  oAlbum(BM):..cre
-00011d30: 6174 6564 3a69 6e74 0a09 6465 7363 7269  ated:int..descri
-00011d40: 7074 696f 6e3a 4f70 7469 6f6e 616c 5b73  ption:Optional[s
-00011d50: 7472 5d20 3d20 4e6f 6e65 0a09 6964 3a69  tr] = None..id:i
-00011d60: 6e74 0a09 6f77 6e65 725f 6964 3a69 6e74  nt..owner_id:int
-00011d70: 0a09 7369 7a65 3a69 6e74 0a09 7468 756d  ..size:int..thum
-00011d80: 623a 4f70 7469 6f6e 616c 5b22 5068 6f74  b:Optional["Phot
-00011d90: 6f73 5068 6f74 6f22 5d20 3d20 4e6f 6e65  osPhoto"] = None
-00011da0: 0a09 7469 746c 653a 7374 720a 0975 7064  ..title:str..upd
-00011db0: 6174 6564 3a69 6e74 0a0a 0a63 6c61 7373  ated:int...class
-00011dc0: 2050 686f 746f 7350 686f 746f 416c 6275   PhotosPhotoAlbu
-00011dd0: 6d46 756c 6c28 424d 293a 0a09 6361 6e5f  mFull(BM):..can_
-00011de0: 7570 6c6f 6164 3a4f 7074 696f 6e61 6c5b  upload:Optional[
-00011df0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 636f  bool] = None..co
-00011e00: 6d6d 656e 7473 5f64 6973 6162 6c65 643a  mments_disabled:
-00011e10: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00011e20: 204e 6f6e 650a 0963 7265 6174 6564 3a69   None..created:i
-00011e30: 6e74 0a09 6465 7363 7269 7074 696f 6e3a  nt..description:
-00011e40: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00011e50: 4e6f 6e65 0a09 6361 6e5f 6465 6c65 7465  None..can_delete
-00011e60: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-00011e70: 3d20 4e6f 6e65 0a09 6964 3a69 6e74 0a09  = None..id:int..
-00011e80: 6f77 6e65 725f 6964 3a69 6e74 0a09 7369  owner_id:int..si
-00011e90: 7a65 3a69 6e74 0a09 7369 7a65 733a 4f70  ze:int..sizes:Op
-00011ea0: 7469 6f6e 616c 5b6c 6973 745b 2250 686f  tional[list["Pho
-00011eb0: 746f 7350 686f 746f 5369 7a65 7322 5d5d  tosPhotoSizes"]]
-00011ec0: 203d 204e 6f6e 650a 0974 6875 6d62 5f69   = None..thumb_i
-00011ed0: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-00011ee0: 3d20 4e6f 6e65 0a09 7468 756d 625f 6973  = None..thumb_is
-00011ef0: 5f6c 6173 743a 4f70 7469 6f6e 616c 5b62  _last:Optional[b
-00011f00: 6f6f 6c5d 203d 204e 6f6e 650a 0974 6875  ool] = None..thu
-00011f10: 6d62 5f73 7263 3a4f 7074 696f 6e61 6c5b  mb_src:Optional[
-00011f20: 7374 725d 203d 204e 6f6e 650a 0974 6974  str] = None..tit
-00011f30: 6c65 3a73 7472 0a09 7570 6461 7465 643a  le:str..updated:
-00011f40: 696e 740a 0975 706c 6f61 645f 6279 5f61  int..upload_by_a
-00011f50: 646d 696e 735f 6f6e 6c79 3a4f 7074 696f  dmins_only:Optio
-00011f60: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00011f70: 0a0a 0a63 6c61 7373 2050 686f 746f 7350  ...class PhotosP
-00011f80: 686f 746f 4661 6c73 6561 626c 6528 424d  hotoFalseable(BM
-00011f90: 293a 0a09 7061 7373 0a0a 636c 6173 7320  ):..pass..class 
-00011fa0: 5068 6f74 6f73 5068 6f74 6f46 756c 6c58  PhotosPhotoFullX
-00011fb0: 7472 5265 616c 4f66 6673 6574 2842 4d29  trRealOffset(BM)
-00011fc0: 3a0a 0961 6363 6573 735f 6b65 793a 4f70  :..access_key:Op
-00011fd0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00011fe0: 6e65 0a09 616c 6275 6d5f 6964 3a69 6e74  ne..album_id:int
-00011ff0: 0a09 6361 6e5f 636f 6d6d 656e 743a 4f70  ..can_comment:Op
-00012000: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-00012010: 6f6e 650a 0963 6f6d 6d65 6e74 733a 4f70  one..comments:Op
-00012020: 7469 6f6e 616c 5b22 4261 7365 4f62 6a65  tional["BaseObje
-00012030: 6374 436f 756e 7422 5d20 3d20 4e6f 6e65  ctCount"] = None
-00012040: 0a09 6461 7465 3a69 6e74 0a09 6865 6967  ..date:int..heig
-00012050: 6874 3a4f 7074 696f 6e61 6c5b 696e 745d  ht:Optional[int]
-00012060: 203d 204e 6f6e 650a 0968 6964 6465 6e3a   = None..hidden:
-00012070: 4f70 7469 6f6e 616c 5b22 4261 7365 5072  Optional["BasePr
-00012080: 6f70 6572 7479 4578 6973 7473 225d 203d  opertyExists"] =
-00012090: 204e 6f6e 650a 0969 643a 696e 740a 096c   None..id:int..l
-000120a0: 6174 3a4f 7074 696f 6e61 6c5b 696e 745d  at:Optional[int]
-000120b0: 203d 204e 6f6e 650a 096c 696b 6573 3a4f   = None..likes:O
-000120c0: 7074 696f 6e61 6c5b 2242 6173 654c 696b  ptional["BaseLik
-000120d0: 6573 225d 203d 204e 6f6e 650a 096c 6f6e  es"] = None..lon
-000120e0: 673a 4f70 7469 6f6e 616c 5b69 6e74 5d20  g:Optional[int] 
-000120f0: 3d20 4e6f 6e65 0a09 6f77 6e65 725f 6964  = None..owner_id
-00012100: 3a69 6e74 0a09 7068 6f74 6f5f 3132 3830  :int..photo_1280
-00012110: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00012120: 204e 6f6e 650a 0970 686f 746f 5f31 3330   None..photo_130
-00012130: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00012140: 204e 6f6e 650a 0970 686f 746f 5f32 3536   None..photo_256
-00012150: 303a 4f70 7469 6f6e 616c 5b73 7472 5d20  0:Optional[str] 
-00012160: 3d20 4e6f 6e65 0a09 7068 6f74 6f5f 3630  = None..photo_60
-00012170: 343a 4f70 7469 6f6e 616c 5b73 7472 5d20  4:Optional[str] 
-00012180: 3d20 4e6f 6e65 0a09 7068 6f74 6f5f 3735  = None..photo_75
-00012190: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-000121a0: 204e 6f6e 650a 0970 686f 746f 5f38 3037   None..photo_807
-000121b0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-000121c0: 204e 6f6e 650a 0970 6f73 745f 6964 3a4f   None..post_id:O
-000121d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000121e0: 6f6e 650a 0972 6561 6c5f 6f66 6673 6574  one..real_offset
-000121f0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00012200: 204e 6f6e 650a 0972 6570 6f73 7473 3a4f   None..reposts:O
-00012210: 7074 696f 6e61 6c5b 2242 6173 654f 626a  ptional["BaseObj
-00012220: 6563 7443 6f75 6e74 225d 203d 204e 6f6e  ectCount"] = Non
-00012230: 650a 0973 697a 6573 3a4f 7074 696f 6e61  e..sizes:Optiona
-00012240: 6c5b 6c69 7374 5b22 5068 6f74 6f73 5068  l[list["PhotosPh
-00012250: 6f74 6f53 697a 6573 225d 5d20 3d20 4e6f  otoSizes"]] = No
-00012260: 6e65 0a09 7461 6773 3a4f 7074 696f 6e61  ne..tags:Optiona
-00012270: 6c5b 2242 6173 654f 626a 6563 7443 6f75  l["BaseObjectCou
-00012280: 6e74 225d 203d 204e 6f6e 650a 0974 6578  nt"] = None..tex
-00012290: 743a 4f70 7469 6f6e 616c 5b73 7472 5d20  t:Optional[str] 
-000122a0: 3d20 4e6f 6e65 0a09 7573 6572 5f69 643a  = None..user_id:
-000122b0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000122c0: 4e6f 6e65 0a09 7769 6474 683a 4f70 7469  None..width:Opti
-000122d0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000122e0: 0a0a 0a63 6c61 7373 2050 686f 746f 7350  ...class PhotosP
-000122f0: 686f 746f 5369 7a65 7328 424d 293a 0a09  hotoSizes(BM):..
-00012300: 6865 6967 6874 3a69 6e74 0a09 7572 6c3a  height:int..url:
-00012310: 7374 720a 0973 7263 3a4f 7074 696f 6e61  str..src:Optiona
-00012320: 6c5b 7374 725d 203d 204e 6f6e 650a 0974  l[str] = None..t
-00012330: 7970 653a 2250 686f 746f 7350 686f 746f  ype:"PhotosPhoto
-00012340: 5369 7a65 7354 7970 6522 0a09 7769 6474  SizesType"..widt
-00012350: 683a 696e 740a 0a0a 636c 6173 7320 5068  h:int...class Ph
-00012360: 6f74 6f73 5068 6f74 6f54 6167 2842 4d29  otosPhotoTag(BM)
-00012370: 3a0a 0964 6174 653a 696e 740a 0969 643a  :..date:int..id:
-00012380: 696e 740a 0970 6c61 6365 725f 6964 3a69  int..placer_id:i
-00012390: 6e74 0a09 7461 6767 6564 5f6e 616d 653a  nt..tagged_name:
-000123a0: 7374 720a 0964 6573 6372 6970 7469 6f6e  str..description
-000123b0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-000123c0: 204e 6f6e 650a 0975 7365 725f 6964 3a69   None..user_id:i
-000123d0: 6e74 0a09 7669 6577 6564 3a62 6f6f 6c0a  nt..viewed:bool.
-000123e0: 0978 3a69 6e74 0a09 7832 3a69 6e74 0a09  .x:int..x2:int..
-000123f0: 793a 696e 740a 0979 323a 696e 740a 0a0a  y:int..y2:int...
-00012400: 636c 6173 7320 5068 6f74 6f73 5068 6f74  class PhotosPhot
-00012410: 6f55 706c 6f61 6428 424d 293a 0a09 616c  oUpload(BM):..al
-00012420: 6275 6d5f 6964 3a69 6e74 0a09 7570 6c6f  bum_id:int..uplo
-00012430: 6164 5f75 726c 3a73 7472 0a09 6661 6c6c  ad_url:str..fall
-00012440: 6261 636b 5f75 706c 6f61 645f 7572 6c3a  back_upload_url:
-00012450: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00012460: 4e6f 6e65 0a09 7573 6572 5f69 643a 696e  None..user_id:in
-00012470: 740a 0967 726f 7570 5f69 643a 4f70 7469  t..group_id:Opti
-00012480: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00012490: 0a0a 0a63 6c61 7373 2050 686f 746f 7350  ...class PhotosP
-000124a0: 686f 746f 5874 7252 6561 6c4f 6666 7365  hotoXtrRealOffse
-000124b0: 7428 424d 293a 0a09 6163 6365 7373 5f6b  t(BM):..access_k
-000124c0: 6579 3a4f 7074 696f 6e61 6c5b 7374 725d  ey:Optional[str]
-000124d0: 203d 204e 6f6e 650a 0961 6c62 756d 5f69   = None..album_i
-000124e0: 643a 696e 740a 0964 6174 653a 696e 740a  d:int..date:int.
-000124f0: 0968 6569 6768 743a 4f70 7469 6f6e 616c  .height:Optional
-00012500: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6869  [int] = None..hi
-00012510: 6464 656e 3a4f 7074 696f 6e61 6c5b 2242  dden:Optional["B
-00012520: 6173 6550 726f 7065 7274 7945 7869 7374  asePropertyExist
-00012530: 7322 5d20 3d20 4e6f 6e65 0a09 6964 3a69  s"] = None..id:i
-00012540: 6e74 0a09 6c61 743a 4f70 7469 6f6e 616c  nt..lat:Optional
-00012550: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6c6f  [int] = None..lo
-00012560: 6e67 3a4f 7074 696f 6e61 6c5b 696e 745d  ng:Optional[int]
-00012570: 203d 204e 6f6e 650a 096f 776e 6572 5f69   = None..owner_i
-00012580: 643a 696e 740a 0970 686f 746f 5f31 3238  d:int..photo_128
-00012590: 303a 4f70 7469 6f6e 616c 5b73 7472 5d20  0:Optional[str] 
-000125a0: 3d20 4e6f 6e65 0a09 7068 6f74 6f5f 3133  = None..photo_13
-000125b0: 303a 4f70 7469 6f6e 616c 5b73 7472 5d20  0:Optional[str] 
-000125c0: 3d20 4e6f 6e65 0a09 7068 6f74 6f5f 3235  = None..photo_25
-000125d0: 3630 3a4f 7074 696f 6e61 6c5b 7374 725d  60:Optional[str]
-000125e0: 203d 204e 6f6e 650a 0970 686f 746f 5f36   = None..photo_6
-000125f0: 3034 3a4f 7074 696f 6e61 6c5b 7374 725d  04:Optional[str]
-00012600: 203d 204e 6f6e 650a 0970 686f 746f 5f37   = None..photo_7
-00012610: 353a 4f70 7469 6f6e 616c 5b73 7472 5d20  5:Optional[str] 
-00012620: 3d20 4e6f 6e65 0a09 7068 6f74 6f5f 3830  = None..photo_80
-00012630: 373a 4f70 7469 6f6e 616c 5b73 7472 5d20  7:Optional[str] 
-00012640: 3d20 4e6f 6e65 0a09 706f 7374 5f69 643a  = None..post_id:
-00012650: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00012660: 4e6f 6e65 0a09 7265 616c 5f6f 6666 7365  None..real_offse
-00012670: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
-00012680: 3d20 4e6f 6e65 0a09 7369 7a65 733a 4f70  = None..sizes:Op
-00012690: 7469 6f6e 616c 5b6c 6973 745b 2250 686f  tional[list["Pho
-000126a0: 746f 7350 686f 746f 5369 7a65 7322 5d5d  tosPhotoSizes"]]
-000126b0: 203d 204e 6f6e 650a 0974 6578 743a 4f70   = None..text:Op
-000126c0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-000126d0: 6e65 0a09 7573 6572 5f69 643a 4f70 7469  ne..user_id:Opti
-000126e0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000126f0: 0a09 7769 6474 683a 4f70 7469 6f6e 616c  ..width:Optional
-00012700: 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63  [int] = None...c
-00012710: 6c61 7373 2050 686f 746f 7350 686f 746f  lass PhotosPhoto
-00012720: 5874 7254 6167 496e 666f 2842 4d29 3a0a  XtrTagInfo(BM):.
-00012730: 0961 6363 6573 735f 6b65 793a 4f70 7469  .access_key:Opti
-00012740: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00012750: 0a09 616c 6275 6d5f 6964 3a69 6e74 0a09  ..album_id:int..
-00012760: 6461 7465 3a69 6e74 0a09 6865 6967 6874  date:int..height
-00012770: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00012780: 204e 6f6e 650a 0969 643a 696e 740a 096c   None..id:int..l
-00012790: 6174 3a4f 7074 696f 6e61 6c5b 696e 745d  at:Optional[int]
-000127a0: 203d 204e 6f6e 650a 096c 6f6e 673a 4f70   = None..long:Op
-000127b0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000127c0: 6e65 0a09 6f77 6e65 725f 6964 3a69 6e74  ne..owner_id:int
-000127d0: 0a09 7068 6f74 6f5f 3132 3830 3a4f 7074  ..photo_1280:Opt
-000127e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-000127f0: 650a 0970 686f 746f 5f31 3330 3a4f 7074  e..photo_130:Opt
-00012800: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00012810: 650a 0970 686f 746f 5f32 3536 303a 4f70  e..photo_2560:Op
-00012820: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00012830: 6e65 0a09 7068 6f74 6f5f 3630 343a 4f70  ne..photo_604:Op
-00012840: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00012850: 6e65 0a09 7068 6f74 6f5f 3735 3a4f 7074  ne..photo_75:Opt
-00012860: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00012870: 650a 0970 686f 746f 5f38 3037 3a4f 7074  e..photo_807:Opt
-00012880: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00012890: 650a 0970 6c61 6365 725f 6964 3a4f 7074  e..placer_id:Opt
-000128a0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-000128b0: 650a 0970 6f73 745f 6964 3a4f 7074 696f  e..post_id:Optio
-000128c0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-000128d0: 0973 697a 6573 3a4f 7074 696f 6e61 6c5b  .sizes:Optional[
-000128e0: 6c69 7374 5b22 5068 6f74 6f73 5068 6f74  list["PhotosPhot
-000128f0: 6f53 697a 6573 225d 5d20 3d20 4e6f 6e65  oSizes"]] = None
-00012900: 0a09 7461 675f 6372 6561 7465 643a 4f70  ..tag_created:Op
-00012910: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00012920: 6e65 0a09 7461 675f 6964 3a4f 7074 696f  ne..tag_id:Optio
-00012930: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00012940: 0974 6578 743a 4f70 7469 6f6e 616c 5b73  .text:Optional[s
-00012950: 7472 5d20 3d20 4e6f 6e65 0a09 7573 6572  tr] = None..user
-00012960: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-00012970: 5d20 3d20 4e6f 6e65 0a09 7769 6474 683a  ] = None..width:
-00012980: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00012990: 4e6f 6e65 0a0a 0a63 6c61 7373 2050 686f  None...class Pho
-000129a0: 746f 7354 6167 7353 7567 6765 7374 696f  tosTagsSuggestio
-000129b0: 6e49 7465 6d28 424d 293a 0a09 7469 746c  nItem(BM):..titl
-000129c0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-000129d0: 3d20 4e6f 6e65 0a09 6361 7074 696f 6e3a  = None..caption:
-000129e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000129f0: 4e6f 6e65 0a09 7479 7065 3a4f 7074 696f  None..type:Optio
-00012a00: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00012a10: 0962 7574 746f 6e73 3a4f 7074 696f 6e61  .buttons:Optiona
-00012a20: 6c5b 6c69 7374 5b22 5068 6f74 6f73 5461  l[list["PhotosTa
-00012a30: 6773 5375 6767 6573 7469 6f6e 4974 656d  gsSuggestionItem
-00012a40: 4275 7474 6f6e 225d 5d20 3d20 4e6f 6e65  Button"]] = None
-00012a50: 0a09 7068 6f74 6f3a 4f70 7469 6f6e 616c  ..photo:Optional
-00012a60: 5b22 5068 6f74 6f73 5068 6f74 6f22 5d20  ["PhotosPhoto"] 
-00012a70: 3d20 4e6f 6e65 0a09 7461 6773 3a4f 7074  = None..tags:Opt
-00012a80: 696f 6e61 6c5b 6c69 7374 5b22 5068 6f74  ional[list["Phot
-00012a90: 6f73 5068 6f74 6f54 6167 225d 5d20 3d20  osPhotoTag"]] = 
-00012aa0: 4e6f 6e65 0a09 7472 6163 6b5f 636f 6465  None..track_code
-00012ab0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00012ac0: 204e 6f6e 650a 0a0a 636c 6173 7320 5068   None...class Ph
-00012ad0: 6f74 6f73 5461 6773 5375 6767 6573 7469  otosTagsSuggesti
-00012ae0: 6f6e 4974 656d 4275 7474 6f6e 2842 4d29  onItemButton(BM)
-00012af0: 3a0a 0974 6974 6c65 3a4f 7074 696f 6e61  :..title:Optiona
-00012b00: 6c5b 7374 725d 203d 204e 6f6e 650a 0961  l[str] = None..a
-00012b10: 6374 696f 6e3a 4f70 7469 6f6e 616c 5b73  ction:Optional[s
-00012b20: 7472 5d20 3d20 4e6f 6e65 0a09 7374 796c  tr] = None..styl
-00012b30: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-00012b40: 3d20 4e6f 6e65 0a0a 0a0a 0a63 6c61 7373  = None.....class
-00012b50: 2050 6f64 6361 7374 436f 7665 7228 424d   PodcastCover(BM
-00012b60: 293a 0a09 7369 7a65 733a 4f70 7469 6f6e  ):..sizes:Option
-00012b70: 616c 5b6c 6973 745b 2250 686f 746f 7350  al[list["PhotosP
-00012b80: 686f 746f 5369 7a65 7322 5d5d 203d 204e  hotoSizes"]] = N
-00012b90: 6f6e 650a 0a0a 636c 6173 7320 506f 6463  one...class Podc
-00012ba0: 6173 7445 7874 6572 6e61 6c44 6174 6128  astExternalData(
-00012bb0: 424d 293a 0a09 7572 6c3a 4f70 7469 6f6e  BM):..url:Option
-00012bc0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00012bd0: 6f77 6e65 725f 7572 6c3a 4f70 7469 6f6e  owner_url:Option
-00012be0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00012bf0: 7469 746c 653a 4f70 7469 6f6e 616c 5b73  title:Optional[s
-00012c00: 7472 5d20 3d20 4e6f 6e65 0a09 6f77 6e65  tr] = None..owne
-00012c10: 725f 6e61 6d65 3a4f 7074 696f 6e61 6c5b  r_name:Optional[
-00012c20: 7374 725d 203d 204e 6f6e 650a 0963 6f76  str] = None..cov
-00012c30: 6572 3a4f 7074 696f 6e61 6c5b 2250 6f64  er:Optional["Pod
-00012c40: 6361 7374 436f 7665 7222 5d20 3d20 4e6f  castCover"] = No
-00012c50: 6e65 0a0a 0a0a 0a63 6c61 7373 2050 6f6c  ne.....class Pol
-00012c60: 6c73 416e 7377 6572 2842 4d29 3a0a 0969  lsAnswer(BM):..i
-00012c70: 643a 696e 740a 0972 6174 653a 696e 740a  d:int..rate:int.
-00012c80: 0974 6578 743a 7374 720a 0976 6f74 6573  .text:str..votes
-00012c90: 3a69 6e74 0a0a 0a63 6c61 7373 2050 6f6c  :int...class Pol
-00012ca0: 6c73 4261 636b 6772 6f75 6e64 2842 4d29  lsBackground(BM)
-00012cb0: 3a0a 0961 6e67 6c65 3a4f 7074 696f 6e61  :..angle:Optiona
-00012cc0: 6c5b 696e 745d 203d 204e 6f6e 650a 0963  l[int] = None..c
-00012cd0: 6f6c 6f72 3a4f 7074 696f 6e61 6c5b 7374  olor:Optional[st
-00012ce0: 725d 203d 204e 6f6e 650a 0968 6569 6768  r] = None..heigh
-00012cf0: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
-00012d00: 3d20 4e6f 6e65 0a09 6964 3a4f 7074 696f  = None..id:Optio
-00012d10: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00012d20: 096e 616d 653a 4f70 7469 6f6e 616c 5b73  .name:Optional[s
-00012d30: 7472 5d20 3d20 4e6f 6e65 0a09 696d 6167  tr] = None..imag
-00012d40: 6573 3a4f 7074 696f 6e61 6c5b 6c69 7374  es:Optional[list
-00012d50: 5b22 4261 7365 496d 6167 6522 5d5d 203d  ["BaseImage"]] =
-00012d60: 204e 6f6e 650a 0970 6f69 6e74 733a 4f70   None..points:Op
-00012d70: 7469 6f6e 616c 5b6c 6973 745b 2242 6173  tional[list["Bas
-00012d80: 6547 7261 6469 656e 7450 6f69 6e74 225d  eGradientPoint"]
-00012d90: 5d20 3d20 4e6f 6e65 0a09 7479 7065 3a4f  ] = None..type:O
-00012da0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00012db0: 6f6e 650a 0977 6964 7468 3a4f 7074 696f  one..width:Optio
-00012dc0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00012dd0: 0a0a 636c 6173 7320 506f 6c6c 7346 7269  ..class PollsFri
-00012de0: 656e 6428 424d 293a 0a09 6964 3a69 6e74  end(BM):..id:int
-00012df0: 0a0a 0a63 6c61 7373 2050 6f6c 6c73 506f  ...class PollsPo
-00012e00: 6c6c 2842 4d29 3a0a 0961 6e6f 6e79 6d6f  ll(BM):..anonymo
-00012e10: 7573 3a4f 7074 696f 6e61 6c5b 2250 6f6c  us:Optional["Pol
-00012e20: 6c73 506f 6c6c 416e 6f6e 796d 6f75 7322  lsPollAnonymous"
-00012e30: 5d20 3d20 4e6f 6e65 0a09 6672 6965 6e64  ] = None..friend
-00012e40: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-00012e50: 2250 6f6c 6c73 4672 6965 6e64 225d 5d20  "PollsFriend"]] 
-00012e60: 3d20 4e6f 6e65 0a09 6d75 6c74 6970 6c65  = None..multiple
-00012e70: 3a62 6f6f 6c0a 0961 6e73 7765 725f 6964  :bool..answer_id
-00012e80: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00012e90: 204e 6f6e 650a 0965 6e64 5f64 6174 653a   None..end_date:
-00012ea0: 696e 740a 0961 6e73 7765 725f 6964 733a  int..answer_ids:
-00012eb0: 4f70 7469 6f6e 616c 5b6c 6973 745b 696e  Optional[list[in
-00012ec0: 745d 5d20 3d20 4e6f 6e65 0a09 636c 6f73  t]] = None..clos
-00012ed0: 6564 3a62 6f6f 6c0a 0969 735f 626f 6172  ed:bool..is_boar
-00012ee0: 643a 626f 6f6c 0a09 6361 6e5f 6564 6974  d:bool..can_edit
-00012ef0: 3a62 6f6f 6c0a 0963 616e 5f76 6f74 653a  :bool..can_vote:
-00012f00: 626f 6f6c 0a09 6361 6e5f 7265 706f 7274  bool..can_report
-00012f10: 3a62 6f6f 6c0a 0963 616e 5f73 6861 7265  :bool..can_share
-00012f20: 3a62 6f6f 6c0a 0965 6d62 6564 5f68 6173  :bool..embed_has
-00012f30: 683a 4f70 7469 6f6e 616c 5b73 7472 5d20  h:Optional[str] 
-00012f40: 3d20 4e6f 6e65 0a09 7068 6f74 6f3a 4f70  = None..photo:Op
-00012f50: 7469 6f6e 616c 5b22 506f 6c6c 7342 6163  tional["PollsBac
-00012f60: 6b67 726f 756e 6422 5d20 3d20 4e6f 6e65  kground"] = None
-00012f70: 0a09 616e 7377 6572 733a 6c69 7374 5b22  ..answers:list["
-00012f80: 506f 6c6c 7341 6e73 7765 7222 5d0a 0963  PollsAnswer"]..c
-00012f90: 7265 6174 6564 3a69 6e74 0a09 6964 3a69  reated:int..id:i
-00012fa0: 6e74 0a09 6f77 6e65 725f 6964 3a69 6e74  nt..owner_id:int
-00012fb0: 0a09 6175 7468 6f72 5f69 643a 4f70 7469  ..author_id:Opti
-00012fc0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00012fd0: 0a09 7175 6573 7469 6f6e 3a73 7472 0a09  ..question:str..
-00012fe0: 6261 636b 6772 6f75 6e64 3a4f 7074 696f  background:Optio
-00012ff0: 6e61 6c5b 2250 6f6c 6c73 4261 636b 6772  nal["PollsBackgr
-00013000: 6f75 6e64 225d 203d 204e 6f6e 650a 0976  ound"] = None..v
-00013010: 6f74 6573 3a69 6e74 0a09 6469 7361 626c  otes:int..disabl
-00013020: 655f 756e 766f 7465 3a62 6f6f 6c0a 0a0a  e_unvote:bool...
-00013030: 636c 6173 7320 506f 6c6c 7350 6f6c 6c41  class PollsPollA
-00013040: 6e6f 6e79 6d6f 7573 2842 4d29 3a0a 0970  nonymous(BM):..p
-00013050: 6173 730a 0a63 6c61 7373 2050 6f6c 6c73  ass..class Polls
-00013060: 566f 7465 7273 2842 4d29 3a0a 0961 6e73  Voters(BM):..ans
-00013070: 7765 725f 6964 3a4f 7074 696f 6e61 6c5b  wer_id:Optional[
-00013080: 696e 745d 203d 204e 6f6e 650a 0975 7365  int] = None..use
-00013090: 7273 3a4f 7074 696f 6e61 6c5b 2250 6f6c  rs:Optional["Pol
-000130a0: 6c73 566f 7465 7273 5573 6572 7322 5d20  lsVotersUsers"] 
-000130b0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2050  = None...class P
-000130c0: 6f6c 6c73 566f 7465 7273 5573 6572 7328  ollsVotersUsers(
-000130d0: 424d 293a 0a09 636f 756e 743a 4f70 7469  BM):..count:Opti
-000130e0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000130f0: 0a09 6974 656d 733a 4f70 7469 6f6e 616c  ..items:Optional
-00013100: 5b6c 6973 745b 696e 745d 5d20 3d20 4e6f  [list[int]] = No
-00013110: 6e65 0a0a 0a0a 0a63 6c61 7373 2050 7265  ne.....class Pre
-00013120: 7474 7943 6172 6473 5072 6574 7479 4361  ttyCardsPrettyCa
-00013130: 7264 2842 4d29 3a0a 0962 7574 746f 6e3a  rd(BM):..button:
-00013140: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
-00013150: 7472 2c22 4261 7365 4c69 6e6b 4275 7474  tr,"BaseLinkButt
-00013160: 6f6e 225d 5d20 3d20 4e6f 6e65 0a09 6275  on"]] = None..bu
-00013170: 7474 6f6e 5f74 6578 743a 4f70 7469 6f6e  tton_text:Option
-00013180: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00013190: 6361 7264 5f69 643a 7374 720a 0969 6d61  card_id:str..ima
-000131a0: 6765 733a 4f70 7469 6f6e 616c 5b6c 6973  ges:Optional[lis
-000131b0: 745b 2242 6173 6549 6d61 6765 225d 5d20  t["BaseImage"]] 
-000131c0: 3d20 4e6f 6e65 0a09 6c69 6e6b 5f75 726c  = None..link_url
-000131d0: 3a73 7472 0a09 7068 6f74 6f3a 7374 720a  :str..photo:str.
-000131e0: 0970 7269 6365 3a4f 7074 696f 6e61 6c5b  .price:Optional[
-000131f0: 7374 725d 203d 204e 6f6e 650a 0970 7269  str] = None..pri
-00013200: 6365 5f6f 6c64 3a4f 7074 696f 6e61 6c5b  ce_old:Optional[
-00013210: 7374 725d 203d 204e 6f6e 650a 0974 6974  str] = None..tit
-00013220: 6c65 3a73 7472 0a0a 0a63 6c61 7373 2050  le:str...class P
-00013230: 7265 7474 7943 6172 6473 5072 6574 7479  rettyCardsPretty
-00013240: 4361 7264 4f72 4572 726f 7228 424d 293a  CardOrError(BM):
-00013250: 0a09 7061 7373 0a0a 0a0a 636c 6173 7320  ..pass....class 
-00013260: 5365 6172 6368 4869 6e74 5365 6374 696f  SearchHintSectio
-00013270: 6e28 456e 756d 293a 0a09 4752 4f55 5053  n(Enum):..GROUPS
-00013280: 203d 2022 6772 6f75 7073 220a 0945 5645   = "groups"..EVE
-00013290: 4e54 5320 3d20 2265 7665 6e74 7322 0a09  NTS = "events"..
-000132a0: 5055 424c 4943 5320 3d20 2270 7562 6c69  PUBLICS = "publi
-000132b0: 6373 220a 0943 4f52 5245 5350 4f4e 4445  cs"..CORRESPONDE
-000132c0: 4e54 5320 3d20 2263 6f72 7265 7370 6f6e  NTS = "correspon
-000132d0: 6465 6e74 7322 0a09 5045 4f50 4c45 203d  dents"..PEOPLE =
-000132e0: 2022 7065 6f70 6c65 220a 0946 5249 454e   "people"..FRIEN
-000132f0: 4453 203d 2022 6672 6965 6e64 7322 0a09  DS = "friends"..
-00013300: 4d55 5455 414c 5f46 5249 454e 4453 203d  MUTUAL_FRIENDS =
-00013310: 2022 6d75 7475 616c 5f66 7269 656e 6473   "mutual_friends
-00013320: 220a 0950 524f 4d4f 203d 2022 7072 6f6d  "..PROMO = "prom
-00013330: 6f22 0a0a 636c 6173 7320 5365 6172 6368  o"..class Search
-00013340: 4869 6e74 5479 7065 2845 6e75 6d29 3a0a  HintType(Enum):.
-00013350: 0947 524f 5550 203d 2022 6772 6f75 7022  .GROUP = "group"
-00013360: 0a09 5052 4f46 494c 4520 3d20 2270 726f  ..PROFILE = "pro
-00013370: 6669 6c65 220a 0956 4b5f 4150 5020 3d20  file"..VK_APP = 
-00013380: 2276 6b5f 6170 7022 0a09 4150 5020 3d20  "vk_app"..APP = 
-00013390: 2261 7070 220a 0948 544d 4c35 5f47 414d  "app"..HTML5_GAM
-000133a0: 4520 3d20 2268 746d 6c35 5f67 616d 6522  E = "html5_game"
-000133b0: 0a09 4c49 4e4b 203d 2022 6c69 6e6b 220a  ..LINK = "link".
-000133c0: 0a63 6c61 7373 2053 6561 7263 6848 696e  .class SearchHin
-000133d0: 7428 424d 293a 0a09 6170 703a 4f70 7469  t(BM):..app:Opti
-000133e0: 6f6e 616c 5b22 4170 7073 4170 7022 5d20  onal["AppsApp"] 
-000133f0: 3d20 4e6f 6e65 0a09 6465 7363 7269 7074  = None..descript
-00013400: 696f 6e3a 7374 720a 095f 676c 6f62 616c  ion:str.._global
-00013410: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-00013420: 3d20 4e6f 6e65 0a09 6772 6f75 703a 4f70  = None..group:Op
-00013430: 7469 6f6e 616c 5b22 4772 6f75 7073 4772  tional["GroupsGr
-00013440: 6f75 7022 5d20 3d20 4e6f 6e65 0a09 7072  oup"] = None..pr
-00013450: 6f66 696c 653a 4f70 7469 6f6e 616c 5b22  ofile:Optional["
-00013460: 5573 6572 7355 7365 724d 696e 225d 203d  UsersUserMin"] =
-00013470: 204e 6f6e 650a 0973 6563 7469 6f6e 3a4f   None..section:O
-00013480: 7074 696f 6e61 6c5b 2253 6561 7263 6848  ptional["SearchH
-00013490: 696e 7453 6563 7469 6f6e 225d 203d 204e  intSection"] = N
-000134a0: 6f6e 650a 0974 7970 653a 2253 6561 7263  one..type:"Searc
-000134b0: 6848 696e 7454 7970 6522 0a09 6c69 6e6b  hHintType"..link
-000134c0: 3a4f 7074 696f 6e61 6c5b 2242 6173 654c  :Optional["BaseL
-000134d0: 696e 6b22 5d20 3d20 4e6f 6e65 0a0a 0a0a  ink"] = None....
-000134e0: 0a63 6c61 7373 2053 6563 7572 6547 6976  .class SecureGiv
-000134f0: 6545 7665 6e74 5374 6963 6b65 7249 7465  eEventStickerIte
-00013500: 6d28 424d 293a 0a09 7573 6572 5f69 643a  m(BM):..user_id:
-00013510: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00013520: 4e6f 6e65 0a09 7374 6174 7573 3a4f 7074  None..status:Opt
-00013530: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00013540: 650a 0a0a 636c 6173 7320 5365 6375 7265  e...class Secure
-00013550: 4c65 7665 6c28 424d 293a 0a09 6c65 7665  Level(BM):..leve
-00013560: 6c3a 4f70 7469 6f6e 616c 5b69 6e74 5d20  l:Optional[int] 
-00013570: 3d20 4e6f 6e65 0a09 7569 643a 4f70 7469  = None..uid:Opti
+0000edf0: 6f6e 733a 6c69 7374 5b6c 6973 745b 224d  ons:list[list["M
+0000ee00: 6573 7361 6765 734b 6579 626f 6172 6442  essagesKeyboardB
+0000ee10: 7574 746f 6e22 5d5d 0a09 6175 7468 6f72  utton"]]..author
+0000ee20: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
+0000ee30: 5d20 3d20 4e6f 6e65 0a09 696e 6c69 6e65  ] = None..inline
+0000ee40: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0000ee50: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204d  = None...class M
+0000ee60: 6573 7361 6765 734b 6579 626f 6172 6442  essagesKeyboardB
+0000ee70: 7574 746f 6e28 424d 293a 0a09 6163 7469  utton(BM):..acti
+0000ee80: 6f6e 3a22 4d65 7373 6167 6573 4b65 7962  on:"MessagesKeyb
+0000ee90: 6f61 7264 4275 7474 6f6e 5072 6f70 6572  oardButtonProper
+0000eea0: 7479 4163 7469 6f6e 220a 0963 6f6c 6f72  tyAction"..color
+0000eeb0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+0000eec0: 204e 6f6e 650a 0a0a 636c 6173 7320 4d65   None...class Me
+0000eed0: 7373 6167 6573 4b65 7962 6f61 7264 4275  ssagesKeyboardBu
+0000eee0: 7474 6f6e 4163 7469 6f6e 4361 6c6c 6261  ttonActionCallba
+0000eef0: 636b 2842 4d29 3a0a 096c 6162 656c 3a73  ck(BM):..label:s
+0000ef00: 7472 0a09 7061 796c 6f61 643a 4f70 7469  tr..payload:Opti
+0000ef10: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000ef20: 0a09 7479 7065 3a73 7472 0a0a 0a63 6c61  ..type:str...cla
+0000ef30: 7373 204d 6573 7361 6765 734b 6579 626f  ss MessagesKeybo
+0000ef40: 6172 6442 7574 746f 6e41 6374 696f 6e4c  ardButtonActionL
+0000ef50: 6f63 6174 696f 6e28 424d 293a 0a09 7061  ocation(BM):..pa
+0000ef60: 796c 6f61 643a 4f70 7469 6f6e 616c 5b73  yload:Optional[s
+0000ef70: 7472 5d20 3d20 4e6f 6e65 0a09 7479 7065  tr] = None..type
+0000ef80: 3a73 7472 0a0a 0a63 6c61 7373 204d 6573  :str...class Mes
+0000ef90: 7361 6765 734b 6579 626f 6172 6442 7574  sagesKeyboardBut
+0000efa0: 746f 6e41 6374 696f 6e4f 7065 6e41 7070  tonActionOpenApp
+0000efb0: 2842 4d29 3a0a 0961 7070 5f69 643a 696e  (BM):..app_id:in
+0000efc0: 740a 0968 6173 683a 4f70 7469 6f6e 616c  t..hash:Optional
+0000efd0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6c61  [str] = None..la
+0000efe0: 6265 6c3a 7374 720a 096f 776e 6572 5f69  bel:str..owner_i
+0000eff0: 643a 696e 740a 0970 6179 6c6f 6164 3a4f  d:int..payload:O
+0000f000: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000f010: 6f6e 650a 0974 7970 653a 7374 720a 0a0a  one..type:str...
+0000f020: 636c 6173 7320 4d65 7373 6167 6573 4b65  class MessagesKe
+0000f030: 7962 6f61 7264 4275 7474 6f6e 4163 7469  yboardButtonActi
+0000f040: 6f6e 4f70 656e 4c69 6e6b 2842 4d29 3a0a  onOpenLink(BM):.
+0000f050: 096c 6162 656c 3a73 7472 0a09 6c69 6e6b  .label:str..link
+0000f060: 3a73 7472 0a09 7061 796c 6f61 643a 4f70  :str..payload:Op
+0000f070: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000f080: 6e65 0a09 7479 7065 3a73 7472 0a0a 0a63  ne..type:str...c
+0000f090: 6c61 7373 204d 6573 7361 6765 734b 6579  lass MessagesKey
+0000f0a0: 626f 6172 6442 7574 746f 6e41 6374 696f  boardButtonActio
+0000f0b0: 6e4f 7065 6e50 686f 746f 2842 4d29 3a0a  nOpenPhoto(BM):.
+0000f0c0: 0974 7970 653a 7374 720a 0a0a 636c 6173  .type:str...clas
+0000f0d0: 7320 4d65 7373 6167 6573 4b65 7962 6f61  s MessagesKeyboa
+0000f0e0: 7264 4275 7474 6f6e 4163 7469 6f6e 5465  rdButtonActionTe
+0000f0f0: 7874 2842 4d29 3a0a 096c 6162 656c 3a73  xt(BM):..label:s
+0000f100: 7472 0a09 7061 796c 6f61 643a 4f70 7469  tr..payload:Opti
+0000f110: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000f120: 0a09 7479 7065 3a73 7472 0a0a 0a63 6c61  ..type:str...cla
+0000f130: 7373 204d 6573 7361 6765 734b 6579 626f  ss MessagesKeybo
+0000f140: 6172 6442 7574 746f 6e41 6374 696f 6e56  ardButtonActionV
+0000f150: 6b70 6179 2842 4d29 3a0a 0968 6173 683a  kpay(BM):..hash:
+0000f160: 7374 720a 0970 6179 6c6f 6164 3a4f 7074  str..payload:Opt
+0000f170: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000f180: 650a 0974 7970 653a 7374 720a 0a0a 636c  e..type:str...cl
+0000f190: 6173 7320 4d65 7373 6167 6573 4b65 7962  ass MessagesKeyb
+0000f1a0: 6f61 7264 4275 7474 6f6e 5072 6f70 6572  oardButtonProper
+0000f1b0: 7479 4163 7469 6f6e 2842 4d29 3a0a 0970  tyAction(BM):..p
+0000f1c0: 6173 730a 0a63 6c61 7373 204d 6573 7361  ass..class Messa
+0000f1d0: 6765 734c 6173 7441 6374 6976 6974 7928  gesLastActivity(
+0000f1e0: 424d 293a 0a09 6f6e 6c69 6e65 3a62 6f6f  BM):..online:boo
+0000f1f0: 6c0a 0974 696d 653a 696e 740a 0a0a 636c  l..time:int...cl
+0000f200: 6173 7320 4d65 7373 6167 6573 4c6f 6e67  ass MessagesLong
+0000f210: 706f 6c6c 4d65 7373 6167 6573 2842 4d29  pollMessages(BM)
+0000f220: 3a0a 0963 6f75 6e74 3a4f 7074 696f 6e61  :..count:Optiona
+0000f230: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
+0000f240: 7465 6d73 3a4f 7074 696f 6e61 6c5b 6c69  tems:Optional[li
+0000f250: 7374 5b22 4d65 7373 6167 6573 4d65 7373  st["MessagesMess
+0000f260: 6167 6522 5d5d 203d 204e 6f6e 650a 0a0a  age"]] = None...
+0000f270: 636c 6173 7320 4d65 7373 6167 6573 4c6f  class MessagesLo
+0000f280: 6e67 706f 6c6c 5061 7261 6d73 2842 4d29  ngpollParams(BM)
+0000f290: 3a0a 0973 6572 7665 723a 7374 720a 096b  :..server:str..k
+0000f2a0: 6579 3a73 7472 0a09 7473 3a69 6e74 0a09  ey:str..ts:int..
+0000f2b0: 7074 733a 4f70 7469 6f6e 616c 5b69 6e74  pts:Optional[int
+0000f2c0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+0000f2d0: 204d 6573 7361 6765 734d 6573 7361 6765   MessagesMessage
+0000f2e0: 2842 4d29 3a0a 0961 6374 696f 6e3a 4f70  (BM):..action:Op
+0000f2f0: 7469 6f6e 616c 5b22 4d65 7373 6167 6573  tional["Messages
+0000f300: 4d65 7373 6167 6541 6374 696f 6e22 5d20  MessageAction"] 
+0000f310: 3d20 4e6f 6e65 0a09 6164 6d69 6e5f 6175  = None..admin_au
+0000f320: 7468 6f72 5f69 643a 4f70 7469 6f6e 616c  thor_id:Optional
+0000f330: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6174  [int] = None..at
+0000f340: 7461 6368 6d65 6e74 733a 4f70 7469 6f6e  tachments:Option
+0000f350: 616c 5b6c 6973 745b 224d 6573 7361 6765  al[list["Message
+0000f360: 734d 6573 7361 6765 4174 7461 6368 6d65  sMessageAttachme
+0000f370: 6e74 225d 5d20 3d20 4e6f 6e65 0a09 636f  nt"]] = None..co
+0000f380: 6e76 6572 7361 7469 6f6e 5f6d 6573 7361  nversation_messa
+0000f390: 6765 5f69 643a 4f70 7469 6f6e 616c 5b69  ge_id:Optional[i
+0000f3a0: 6e74 5d20 3d20 4e6f 6e65 0a09 6461 7465  nt] = None..date
+0000f3b0: 3a69 6e74 0a09 6465 6c65 7465 643a 4f70  :int..deleted:Op
+0000f3c0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0000f3d0: 6f6e 650a 0966 726f 6d5f 6964 3a69 6e74  one..from_id:int
+0000f3e0: 0a09 6677 645f 6d65 7373 6167 6573 3a4f  ..fwd_messages:O
+0000f3f0: 7074 696f 6e61 6c5b 6c69 7374 5b22 4d65  ptional[list["Me
+0000f400: 7373 6167 6573 466f 7265 6967 6e4d 6573  ssagesForeignMes
+0000f410: 7361 6765 225d 5d20 3d20 4e6f 6e65 0a09  sage"]] = None..
+0000f420: 6765 6f3a 4f70 7469 6f6e 616c 5b22 4261  geo:Optional["Ba
+0000f430: 7365 4765 6f22 5d20 3d20 4e6f 6e65 0a09  seGeo"] = None..
+0000f440: 6964 3a69 6e74 0a09 696d 706f 7274 616e  id:int..importan
+0000f450: 743a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  t:Optional[bool]
+0000f460: 203d 204e 6f6e 650a 0969 735f 6869 6464   = None..is_hidd
+0000f470: 656e 3a4f 7074 696f 6e61 6c5b 626f 6f6c  en:Optional[bool
+0000f480: 5d20 3d20 4e6f 6e65 0a09 6973 5f63 726f  ] = None..is_cro
+0000f490: 7070 6564 3a4f 7074 696f 6e61 6c5b 626f  pped:Optional[bo
+0000f4a0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6b65 7962  ol] = None..keyb
+0000f4b0: 6f61 7264 3a4f 7074 696f 6e61 6c5b 224d  oard:Optional["M
+0000f4c0: 6573 7361 6765 734b 6579 626f 6172 6422  essagesKeyboard"
+0000f4d0: 5d20 3d20 4e6f 6e65 0a09 6d65 6d62 6572  ] = None..member
+0000f4e0: 735f 636f 756e 743a 4f70 7469 6f6e 616c  s_count:Optional
+0000f4f0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6f75  [int] = None..ou
+0000f500: 743a 626f 6f6c 0a09 7061 796c 6f61 643a  t:bool..payload:
+0000f510: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000f520: 4e6f 6e65 0a09 7065 6572 5f69 643a 696e  None..peer_id:in
+0000f530: 740a 0972 616e 646f 6d5f 6964 3a4f 7074  t..random_id:Opt
+0000f540: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0000f550: 650a 0972 6566 3a4f 7074 696f 6e61 6c5b  e..ref:Optional[
+0000f560: 7374 725d 203d 204e 6f6e 650a 0972 6566  str] = None..ref
+0000f570: 5f73 6f75 7263 653a 4f70 7469 6f6e 616c  _source:Optional
+0000f580: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7265  [str] = None..re
+0000f590: 706c 795f 6d65 7373 6167 653a 4f70 7469  ply_message:Opti
+0000f5a0: 6f6e 616c 5b22 4d65 7373 6167 6573 466f  onal["MessagesFo
+0000f5b0: 7265 6967 6e4d 6573 7361 6765 225d 203d  reignMessage"] =
+0000f5c0: 204e 6f6e 650a 0974 6578 743a 7374 720a   None..text:str.
+0000f5d0: 0975 7064 6174 655f 7469 6d65 3a4f 7074  .update_time:Opt
+0000f5e0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0000f5f0: 650a 0977 6173 5f6c 6973 7465 6e65 643a  e..was_listened:
+0000f600: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0000f610: 204e 6f6e 650a 0970 696e 6e65 645f 6174   None..pinned_at
+0000f620: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+0000f630: 204e 6f6e 650a 0969 735f 7369 6c65 6e74   None..is_silent
+0000f640: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0000f650: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204d  = None...class M
+0000f660: 6573 7361 6765 734d 6573 7361 6765 4163  essagesMessageAc
+0000f670: 7469 6f6e 2842 4d29 3a0a 0963 6f6e 7665  tion(BM):..conve
+0000f680: 7273 6174 696f 6e5f 6d65 7373 6167 655f  rsation_message_
+0000f690: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
+0000f6a0: 203d 204e 6f6e 650a 0965 6d61 696c 3a4f   = None..email:O
+0000f6b0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000f6c0: 6f6e 650a 096d 656d 6265 725f 6964 3a4f  one..member_id:O
+0000f6d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0000f6e0: 6f6e 650a 096d 6573 7361 6765 3a4f 7074  one..message:Opt
+0000f6f0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000f700: 650a 0970 686f 746f 3a4f 7074 696f 6e61  e..photo:Optiona
+0000f710: 6c5b 224d 6573 7361 6765 734d 6573 7361  l["MessagesMessa
+0000f720: 6765 4163 7469 6f6e 5068 6f74 6f22 5d20  geActionPhoto"] 
+0000f730: 3d20 4e6f 6e65 0a09 7465 7874 3a4f 7074  = None..text:Opt
+0000f740: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000f750: 650a 0974 7970 653a 224d 6573 7361 6765  e..type:"Message
+0000f760: 734d 6573 7361 6765 4163 7469 6f6e 5374  sMessageActionSt
+0000f770: 6174 7573 220a 0a0a 636c 6173 7320 4d65  atus"...class Me
+0000f780: 7373 6167 6573 4d65 7373 6167 6541 6374  ssagesMessageAct
+0000f790: 696f 6e50 686f 746f 2842 4d29 3a0a 0970  ionPhoto(BM):..p
+0000f7a0: 686f 746f 5f35 303a 7374 720a 0970 686f  hoto_50:str..pho
+0000f7b0: 746f 5f31 3030 3a73 7472 0a09 7068 6f74  to_100:str..phot
+0000f7c0: 6f5f 3230 303a 7374 720a 0a0a 636c 6173  o_200:str...clas
+0000f7d0: 7320 4d65 7373 6167 6573 4d65 7373 6167  s MessagesMessag
+0000f7e0: 6541 7474 6163 686d 656e 7428 424d 293a  eAttachment(BM):
+0000f7f0: 0a09 6175 6469 6f3a 4f70 7469 6f6e 616c  ..audio:Optional
+0000f800: 5b22 4175 6469 6f41 7564 696f 225d 203d  ["AudioAudio"] =
+0000f810: 204e 6f6e 650a 0961 7564 696f 5f6d 6573   None..audio_mes
+0000f820: 7361 6765 3a4f 7074 696f 6e61 6c5b 224d  sage:Optional["M
+0000f830: 6573 7361 6765 7341 7564 696f 4d65 7373  essagesAudioMess
+0000f840: 6167 6522 5d20 3d20 4e6f 6e65 0a09 6361  age"] = None..ca
+0000f850: 6c6c 3a4f 7074 696f 6e61 6c5b 2243 616c  ll:Optional["Cal
+0000f860: 6c73 4361 6c6c 225d 203d 204e 6f6e 650a  lsCall"] = None.
+0000f870: 0964 6f63 3a4f 7074 696f 6e61 6c5b 2244  .doc:Optional["D
+0000f880: 6f63 7344 6f63 225d 203d 204e 6f6e 650a  ocsDoc"] = None.
+0000f890: 0967 6966 743a 4f70 7469 6f6e 616c 5b22  .gift:Optional["
+0000f8a0: 4769 6674 734c 6179 6f75 7422 5d20 3d20  GiftsLayout"] = 
+0000f8b0: 4e6f 6e65 0a09 6772 6166 6669 7469 3a4f  None..graffiti:O
+0000f8c0: 7074 696f 6e61 6c5b 224d 6573 7361 6765  ptional["Message
+0000f8d0: 7347 7261 6666 6974 6922 5d20 3d20 4e6f  sGraffiti"] = No
+0000f8e0: 6e65 0a09 6d61 726b 6574 3a4f 7074 696f  ne..market:Optio
+0000f8f0: 6e61 6c5b 224d 6172 6b65 744d 6172 6b65  nal["MarketMarke
+0000f900: 7449 7465 6d22 5d20 3d20 4e6f 6e65 0a09  tItem"] = None..
+0000f910: 6d61 726b 6574 5f6d 6172 6b65 745f 616c  market_market_al
+0000f920: 6275 6d3a 4f70 7469 6f6e 616c 5b22 4d61  bum:Optional["Ma
+0000f930: 726b 6574 4d61 726b 6574 416c 6275 6d22  rketMarketAlbum"
+0000f940: 5d20 3d20 4e6f 6e65 0a09 7068 6f74 6f3a  ] = None..photo:
+0000f950: 4f70 7469 6f6e 616c 5b22 5068 6f74 6f73  Optional["Photos
+0000f960: 5068 6f74 6f22 5d20 3d20 4e6f 6e65 0a09  Photo"] = None..
+0000f970: 7374 6963 6b65 723a 4f70 7469 6f6e 616c  sticker:Optional
+0000f980: 5b22 4261 7365 5374 6963 6b65 7222 5d20  ["BaseSticker"] 
+0000f990: 3d20 4e6f 6e65 0a09 7374 6f72 793a 4f70  = None..story:Op
+0000f9a0: 7469 6f6e 616c 5b22 5374 6f72 6965 7353  tional["StoriesS
+0000f9b0: 746f 7279 225d 203d 204e 6f6e 650a 0974  tory"] = None..t
+0000f9c0: 7970 653a 224d 6573 7361 6765 734d 6573  ype:"MessagesMes
+0000f9d0: 7361 6765 4174 7461 6368 6d65 6e74 5479  sageAttachmentTy
+0000f9e0: 7065 220a 0976 6964 656f 3a4f 7074 696f  pe"..video:Optio
+0000f9f0: 6e61 6c5b 2256 6964 656f 5669 6465 6f46  nal["VideoVideoF
+0000fa00: 756c 6c22 5d20 3d20 4e6f 6e65 0a09 7761  ull"] = None..wa
+0000fa10: 6c6c 5f72 6570 6c79 3a4f 7074 696f 6e61  ll_reply:Optiona
+0000fa20: 6c5b 2257 616c 6c57 616c 6c43 6f6d 6d65  l["WallWallComme
+0000fa30: 6e74 225d 203d 204e 6f6e 650a 0970 6f6c  nt"] = None..pol
+0000fa40: 6c3a 4f70 7469 6f6e 616c 5b22 506f 6c6c  l:Optional["Poll
+0000fa50: 7350 6f6c 6c22 5d20 3d20 4e6f 6e65 0a0a  sPoll"] = None..
+0000fa60: 0a63 6c61 7373 204d 6573 7361 6765 734d  .class MessagesM
+0000fa70: 6573 7361 6765 5265 7175 6573 7444 6174  essageRequestDat
+0000fa80: 6128 424d 293a 0a09 7374 6174 7573 3a4f  a(BM):..status:O
+0000fa90: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000faa0: 6f6e 650a 0969 6e76 6974 6572 5f69 643a  one..inviter_id:
+0000fab0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0000fac0: 4e6f 6e65 0a09 7265 7175 6573 745f 6461  None..request_da
+0000fad0: 7465 3a4f 7074 696f 6e61 6c5b 696e 745d  te:Optional[int]
+0000fae0: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
+0000faf0: 4d65 7373 6167 6573 4d65 7373 6167 6573  MessagesMessages
+0000fb00: 4172 7261 7928 424d 293a 0a09 636f 756e  Array(BM):..coun
+0000fb10: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
+0000fb20: 3d20 4e6f 6e65 0a09 6974 656d 733a 4f70  = None..items:Op
+0000fb30: 7469 6f6e 616c 5b6c 6973 745b 224d 6573  tional[list["Mes
+0000fb40: 7361 6765 734d 6573 7361 6765 225d 5d20  sagesMessage"]] 
+0000fb50: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204d  = None...class M
+0000fb60: 6573 7361 6765 734f 7574 5265 6164 4279  essagesOutReadBy
+0000fb70: 2842 4d29 3a0a 0963 6f75 6e74 3a4f 7074  (BM):..count:Opt
+0000fb80: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0000fb90: 650a 096d 656d 6265 725f 6964 733a 4f70  e..member_ids:Op
+0000fba0: 7469 6f6e 616c 5b6c 6973 745b 696e 745d  tional[list[int]
+0000fbb0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+0000fbc0: 204d 6573 7361 6765 7350 696e 6e65 644d   MessagesPinnedM
+0000fbd0: 6573 7361 6765 2842 4d29 3a0a 0961 7474  essage(BM):..att
+0000fbe0: 6163 686d 656e 7473 3a4f 7074 696f 6e61  achments:Optiona
+0000fbf0: 6c5b 6c69 7374 5b22 4d65 7373 6167 6573  l[list["Messages
+0000fc00: 4d65 7373 6167 6541 7474 6163 686d 656e  MessageAttachmen
+0000fc10: 7422 5d5d 203d 204e 6f6e 650a 0963 6f6e  t"]] = None..con
+0000fc20: 7665 7273 6174 696f 6e5f 6d65 7373 6167  versation_messag
+0000fc30: 655f 6964 3a4f 7074 696f 6e61 6c5b 696e  e_id:Optional[in
+0000fc40: 745d 203d 204e 6f6e 650a 0969 643a 696e  t] = None..id:in
+0000fc50: 740a 0964 6174 653a 696e 740a 0966 726f  t..date:int..fro
+0000fc60: 6d5f 6964 3a69 6e74 0a09 6677 645f 6d65  m_id:int..fwd_me
+0000fc70: 7373 6167 6573 3a4f 7074 696f 6e61 6c5b  ssages:Optional[
+0000fc80: 6c69 7374 5b22 4d65 7373 6167 6573 466f  list["MessagesFo
+0000fc90: 7265 6967 6e4d 6573 7361 6765 225d 5d20  reignMessage"]] 
+0000fca0: 3d20 4e6f 6e65 0a09 6765 6f3a 4f70 7469  = None..geo:Opti
+0000fcb0: 6f6e 616c 5b22 4261 7365 4765 6f22 5d20  onal["BaseGeo"] 
+0000fcc0: 3d20 4e6f 6e65 0a09 7065 6572 5f69 643a  = None..peer_id:
+0000fcd0: 696e 740a 0972 6570 6c79 5f6d 6573 7361  int..reply_messa
+0000fce0: 6765 3a4f 7074 696f 6e61 6c5b 224d 6573  ge:Optional["Mes
+0000fcf0: 7361 6765 7346 6f72 6569 676e 4d65 7373  sagesForeignMess
+0000fd00: 6167 6522 5d20 3d20 4e6f 6e65 0a09 7465  age"] = None..te
+0000fd10: 7874 3a73 7472 0a09 6b65 7962 6f61 7264  xt:str..keyboard
+0000fd20: 3a4f 7074 696f 6e61 6c5b 224d 6573 7361  :Optional["Messa
+0000fd30: 6765 734b 6579 626f 6172 6422 5d20 3d20  gesKeyboard"] = 
+0000fd40: 4e6f 6e65 0a0a 0a63 6c61 7373 204d 6573  None...class Mes
+0000fd50: 7361 6765 7350 7573 6853 6574 7469 6e67  sagesPushSetting
+0000fd60: 7328 424d 293a 0a09 6469 7361 626c 6564  s(BM):..disabled
+0000fd70: 5f66 6f72 6576 6572 3a62 6f6f 6c0a 0964  _forever:bool..d
+0000fd80: 6973 6162 6c65 645f 756e 7469 6c3a 4f70  isabled_until:Op
+0000fd90: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0000fda0: 6e65 0a09 6e6f 5f73 6f75 6e64 3a62 6f6f  ne..no_sound:boo
+0000fdb0: 6c0a 0964 6973 6162 6c65 645f 6d65 6e74  l..disabled_ment
+0000fdc0: 696f 6e73 3a4f 7074 696f 6e61 6c5b 626f  ions:Optional[bo
+0000fdd0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6469 7361  ol] = None..disa
+0000fde0: 626c 6564 5f6d 6173 735f 6d65 6e74 696f  bled_mass_mentio
+0000fdf0: 6e73 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ns:Optional[bool
+0000fe00: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+0000fe10: 204d 6573 7361 6765 7353 656e 6455 7365   MessagesSendUse
+0000fe20: 7249 6473 5265 7370 6f6e 7365 4974 656d  rIdsResponseItem
+0000fe30: 2842 4d29 3a0a 0970 6565 725f 6964 3a69  (BM):..peer_id:i
+0000fe40: 6e74 0a09 6d65 7373 6167 655f 6964 3a69  nt..message_id:i
+0000fe50: 6e74 0a09 636f 6e76 6572 7361 7469 6f6e  nt..conversation
+0000fe60: 5f6d 6573 7361 6765 5f69 643a 4f70 7469  _message_id:Opti
+0000fe70: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0000fe80: 0a09 6572 726f 723a 4f70 7469 6f6e 616c  ..error:Optional
+0000fe90: 5b22 4261 7365 4d65 7373 6167 6545 7272  ["BaseMessageErr
+0000fea0: 6f72 225d 203d 204e 6f6e 650a 0a0a 0a0a  or"] = None.....
+0000feb0: 636c 6173 7320 4e65 7773 6665 6564 436f  class NewsfeedCo
+0000fec0: 6d6d 656e 7473 4669 6c74 6572 7328 456e  mmentsFilters(En
+0000fed0: 756d 293a 0a09 504f 5354 203d 2022 706f  um):..POST = "po
+0000fee0: 7374 220a 0950 484f 544f 203d 2022 7068  st"..PHOTO = "ph
+0000fef0: 6f74 6f22 0a09 5649 4445 4f20 3d20 2276  oto"..VIDEO = "v
+0000ff00: 6964 656f 220a 0954 4f50 4943 203d 2022  ideo"..TOPIC = "
+0000ff10: 746f 7069 6322 0a09 4e4f 5445 203d 2022  topic"..NOTE = "
+0000ff20: 6e6f 7465 220a 0a63 6c61 7373 204e 6577  note"..class New
+0000ff30: 7366 6565 6449 676e 6f72 6549 7465 6d54  sfeedIgnoreItemT
+0000ff40: 7970 6528 456e 756d 293a 0a09 504f 5354  ype(Enum):..POST
+0000ff50: 5f4f 4e5f 5448 455f 5741 4c4c 203d 2022  _ON_THE_WALL = "
+0000ff60: 7761 6c6c 220a 0954 4147 5f4f 4e5f 415f  wall"..TAG_ON_A_
+0000ff70: 5048 4f54 4f20 3d20 2274 6167 220a 0950  PHOTO = "tag"..P
+0000ff80: 524f 4649 4c45 5f50 484f 544f 203d 2022  ROFILE_PHOTO = "
+0000ff90: 7072 6f66 696c 6570 686f 746f 220a 0956  profilephoto"..V
+0000ffa0: 4944 454f 203d 2022 7669 6465 6f22 0a09  IDEO = "video"..
+0000ffb0: 5048 4f54 4f20 3d20 2270 686f 746f 220a  PHOTO = "photo".
+0000ffc0: 0941 5544 494f 203d 2022 6175 6469 6f22  .AUDIO = "audio"
+0000ffd0: 0a0a 636c 6173 7320 4e65 7773 6665 6564  ..class Newsfeed
+0000ffe0: 4974 656d 5761 6c6c 706f 7374 4665 6564  ItemWallpostFeed
+0000fff0: 6261 636b 5479 7065 2845 6e75 6d29 3a0a  backType(Enum):.
+00010000: 0942 5554 544f 4e53 203d 2022 6275 7474  .BUTTONS = "butt
+00010010: 6f6e 7322 0a09 5354 4152 5320 3d20 2273  ons"..STARS = "s
+00010020: 7461 7273 220a 0a63 6c61 7373 204e 6577  tars"..class New
+00010030: 7366 6565 644e 6577 7366 6565 6449 7465  sfeedNewsfeedIte
+00010040: 6d54 7970 6528 456e 756d 293a 0a09 504f  mType(Enum):..PO
+00010050: 5354 203d 2022 706f 7374 220a 0950 484f  ST = "post"..PHO
+00010060: 544f 203d 2022 7068 6f74 6f22 0a09 5048  TO = "photo"..PH
+00010070: 4f54 4f5f 5441 4720 3d20 2270 686f 746f  OTO_TAG = "photo
+00010080: 5f74 6167 220a 0957 414c 4c5f 5048 4f54  _tag"..WALL_PHOT
+00010090: 4f20 3d20 2277 616c 6c5f 7068 6f74 6f22  O = "wall_photo"
+000100a0: 0a09 4652 4945 4e44 203d 2022 6672 6965  ..FRIEND = "frie
+000100b0: 6e64 220a 0941 5544 494f 203d 2022 6175  nd"..AUDIO = "au
+000100c0: 6469 6f22 0a09 5649 4445 4f20 3d20 2276  dio"..VIDEO = "v
+000100d0: 6964 656f 220a 0954 4f50 4943 203d 2022  ideo"..TOPIC = "
+000100e0: 746f 7069 6322 0a09 4449 4745 5354 203d  topic"..DIGEST =
+000100f0: 2022 6469 6765 7374 220a 0953 544f 5249   "digest"..STORI
+00010100: 4553 203d 2022 7374 6f72 6965 7322 0a09  ES = "stories"..
+00010110: 4e4f 5445 203d 2022 6e6f 7465 220a 0941  NOTE = "note"..A
+00010120: 5544 494f 5f50 4c41 594c 4953 5420 3d20  UDIO_PLAYLIST = 
+00010130: 2261 7564 696f 5f70 6c61 796c 6973 7422  "audio_playlist"
+00010140: 0a09 434c 4950 203d 2022 636c 6970 220a  ..CLIP = "clip".
+00010150: 0a63 6c61 7373 204e 6577 7366 6565 6449  .class NewsfeedI
+00010160: 7465 6d41 7564 696f 4175 6469 6f28 424d  temAudioAudio(BM
+00010170: 293a 0a09 636f 756e 743a 4f70 7469 6f6e  ):..count:Option
+00010180: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00010190: 6974 656d 733a 4f70 7469 6f6e 616c 5b6c  items:Optional[l
+000101a0: 6973 745b 2241 7564 696f 4175 6469 6f22  ist["AudioAudio"
+000101b0: 5d5d 203d 204e 6f6e 650a 0a0a 636c 6173  ]] = None...clas
+000101c0: 7320 4e65 7773 6665 6564 4974 656d 4261  s NewsfeedItemBa
+000101d0: 7365 2842 4d29 3a0a 0974 7970 653a 224e  se(BM):..type:"N
+000101e0: 6577 7366 6565 644e 6577 7366 6565 6449  ewsfeedNewsfeedI
+000101f0: 7465 6d54 7970 6522 0a09 736f 7572 6365  temType"..source
+00010200: 5f69 643a 696e 740a 0964 6174 653a 696e  _id:int..date:in
+00010210: 740a 0a0a 636c 6173 7320 4e65 7773 6665  t...class Newsfe
+00010220: 6564 4974 656d 4469 6765 7374 4275 7474  edItemDigestButt
+00010230: 6f6e 2842 4d29 3a0a 0974 6974 6c65 3a73  on(BM):..title:s
+00010240: 7472 0a09 7374 796c 653a 4f70 7469 6f6e  tr..style:Option
+00010250: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a0a  al[str] = None..
+00010260: 0a63 6c61 7373 204e 6577 7366 6565 6449  .class NewsfeedI
+00010270: 7465 6d44 6967 6573 7446 6f6f 7465 7228  temDigestFooter(
+00010280: 424d 293a 0a09 7374 796c 653a 7374 720a  BM):..style:str.
+00010290: 0974 6578 743a 7374 720a 0962 7574 746f  .text:str..butto
+000102a0: 6e3a 4f70 7469 6f6e 616c 5b22 4e65 7773  n:Optional["News
+000102b0: 6665 6564 4974 656d 4469 6765 7374 4275  feedItemDigestBu
+000102c0: 7474 6f6e 225d 203d 204e 6f6e 650a 0a0a  tton"] = None...
+000102d0: 636c 6173 7320 4e65 7773 6665 6564 4974  class NewsfeedIt
+000102e0: 656d 4469 6765 7374 4675 6c6c 4974 656d  emDigestFullItem
+000102f0: 2842 4d29 3a0a 0974 6578 743a 4f70 7469  (BM):..text:Opti
+00010300: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00010310: 0a09 736f 7572 6365 5f6e 616d 653a 4f70  ..source_name:Op
+00010320: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00010330: 6e65 0a09 6174 7461 6368 6d65 6e74 5f69  ne..attachment_i
+00010340: 6e64 6578 3a4f 7074 696f 6e61 6c5b 696e  ndex:Optional[in
+00010350: 745d 203d 204e 6f6e 650a 0961 7474 6163  t] = None..attac
+00010360: 686d 656e 743a 4f70 7469 6f6e 616c 5b22  hment:Optional["
+00010370: 5761 6c6c 5761 6c6c 706f 7374 4174 7461  WallWallpostAtta
+00010380: 6368 6d65 6e74 225d 203d 204e 6f6e 650a  chment"] = None.
+00010390: 0973 7479 6c65 3a4f 7074 696f 6e61 6c5b  .style:Optional[
+000103a0: 7374 725d 203d 204e 6f6e 650a 0970 6f73  str] = None..pos
+000103b0: 743a 2257 616c 6c57 616c 6c70 6f73 7422  t:"WallWallpost"
+000103c0: 0a0a 0a63 6c61 7373 204e 6577 7366 6565  ...class Newsfee
+000103d0: 6449 7465 6d44 6967 6573 7448 6561 6465  dItemDigestHeade
+000103e0: 7228 424d 293a 0a09 7469 746c 653a 7374  r(BM):..title:st
+000103f0: 720a 0973 7562 7469 746c 653a 4f70 7469  r..subtitle:Opti
+00010400: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00010410: 0a09 7374 796c 653a 7374 720a 0962 7574  ..style:str..but
+00010420: 746f 6e3a 4f70 7469 6f6e 616c 5b22 4e65  ton:Optional["Ne
+00010430: 7773 6665 6564 4974 656d 4469 6765 7374  wsfeedItemDigest
+00010440: 4275 7474 6f6e 225d 203d 204e 6f6e 650a  Button"] = None.
+00010450: 0a0a 636c 6173 7320 4e65 7773 6665 6564  ..class Newsfeed
+00010460: 4974 656d 4469 6765 7374 4974 656d 2842  ItemDigestItem(B
+00010470: 4d29 3a0a 0970 6173 730a 0a63 6c61 7373  M):..pass..class
+00010480: 204e 6577 7366 6565 6449 7465 6d46 7269   NewsfeedItemFri
+00010490: 656e 6446 7269 656e 6473 2842 4d29 3a0a  endFriends(BM):.
+000104a0: 0963 6f75 6e74 3a4f 7074 696f 6e61 6c5b  .count:Optional[
+000104b0: 696e 745d 203d 204e 6f6e 650a 0969 7465  int] = None..ite
+000104c0: 6d73 3a4f 7074 696f 6e61 6c5b 6c69 7374  ms:Optional[list
+000104d0: 5b22 4261 7365 5573 6572 4964 225d 5d20  ["BaseUserId"]] 
+000104e0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204e  = None...class N
+000104f0: 6577 7366 6565 6449 7465 6d48 6f6c 6964  ewsfeedItemHolid
+00010500: 6179 5265 636f 6d6d 656e 6461 7469 6f6e  ayRecommendation
+00010510: 7342 6c6f 636b 4865 6164 6572 2842 4d29  sBlockHeader(BM)
+00010520: 3a0a 0974 6974 6c65 3a4f 7074 696f 6e61  :..title:Optiona
+00010530: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
+00010540: 7562 7469 746c 653a 4f70 7469 6f6e 616c  ubtitle:Optional
+00010550: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 696d  [str] = None..im
+00010560: 6167 653a 4f70 7469 6f6e 616c 5b6c 6973  age:Optional[lis
+00010570: 745b 2242 6173 6549 6d61 6765 225d 5d20  t["BaseImage"]] 
+00010580: 3d20 4e6f 6e65 0a09 6163 7469 6f6e 3a4f  = None..action:O
+00010590: 7074 696f 6e61 6c5b 2242 6173 654c 696e  ptional["BaseLin
+000105a0: 6b42 7574 746f 6e41 6374 696f 6e22 5d20  kButtonAction"] 
+000105b0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204e  = None...class N
+000105c0: 6577 7366 6565 6449 7465 6d50 686f 746f  ewsfeedItemPhoto
+000105d0: 5068 6f74 6f73 2842 4d29 3a0a 0963 6f75  Photos(BM):..cou
+000105e0: 6e74 3a4f 7074 696f 6e61 6c5b 696e 745d  nt:Optional[int]
+000105f0: 203d 204e 6f6e 650a 0969 7465 6d73 3a4f   = None..items:O
+00010600: 7074 696f 6e61 6c5b 6c69 7374 5b22 4e65  ptional[list["Ne
+00010610: 7773 6665 6564 4e65 7773 6665 6564 5068  wsfeedNewsfeedPh
+00010620: 6f74 6f22 5d5d 203d 204e 6f6e 650a 0a0a  oto"]] = None...
+00010630: 636c 6173 7320 4e65 7773 6665 6564 4974  class NewsfeedIt
+00010640: 656d 5068 6f74 6f54 6167 5068 6f74 6f54  emPhotoTagPhotoT
+00010650: 6167 7328 424d 293a 0a09 636f 756e 743a  ags(BM):..count:
+00010660: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00010670: 4e6f 6e65 0a09 6974 656d 733a 4f70 7469  None..items:Opti
+00010680: 6f6e 616c 5b6c 6973 745b 224e 6577 7366  onal[list["Newsf
+00010690: 6565 644e 6577 7366 6565 6450 686f 746f  eedNewsfeedPhoto
+000106a0: 225d 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  "]] = None...cla
+000106b0: 7373 204e 6577 7366 6565 6449 7465 6d50  ss NewsfeedItemP
+000106c0: 726f 6d6f 4275 7474 6f6e 4163 7469 6f6e  romoButtonAction
+000106d0: 2842 4d29 3a0a 0975 726c 3a4f 7074 696f  (BM):..url:Optio
+000106e0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000106f0: 0974 7970 653a 4f70 7469 6f6e 616c 5b73  .type:Optional[s
+00010700: 7472 5d20 3d20 4e6f 6e65 0a09 7461 7267  tr] = None..targ
+00010710: 6574 3a4f 7074 696f 6e61 6c5b 7374 725d  et:Optional[str]
+00010720: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
+00010730: 4e65 7773 6665 6564 4974 656d 5072 6f6d  NewsfeedItemProm
+00010740: 6f42 7574 746f 6e49 6d61 6765 2842 4d29  oButtonImage(BM)
+00010750: 3a0a 0977 6964 7468 3a4f 7074 696f 6e61  :..width:Optiona
+00010760: 6c5b 696e 745d 203d 204e 6f6e 650a 0968  l[int] = None..h
+00010770: 6569 6768 743a 4f70 7469 6f6e 616c 5b69  eight:Optional[i
+00010780: 6e74 5d20 3d20 4e6f 6e65 0a09 7572 6c3a  nt] = None..url:
+00010790: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000107a0: 4e6f 6e65 0a0a 0a63 6c61 7373 204e 6577  None...class New
+000107b0: 7366 6565 6449 7465 6d56 6964 656f 5669  sfeedItemVideoVi
+000107c0: 6465 6f28 424d 293a 0a09 636f 756e 743a  deo(BM):..count:
+000107d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000107e0: 4e6f 6e65 0a09 6974 656d 733a 4f70 7469  None..items:Opti
+000107f0: 6f6e 616c 5b6c 6973 745b 2256 6964 656f  onal[list["Video
+00010800: 5669 6465 6f22 5d5d 203d 204e 6f6e 650a  Video"]] = None.
+00010810: 0a0a 636c 6173 7320 4e65 7773 6665 6564  ..class Newsfeed
+00010820: 4974 656d 5761 6c6c 706f 7374 4665 6564  ItemWallpostFeed
+00010830: 6261 636b 2842 4d29 3a0a 0974 7970 653a  back(BM):..type:
+00010840: 224e 6577 7366 6565 6449 7465 6d57 616c  "NewsfeedItemWal
+00010850: 6c70 6f73 7446 6565 6462 6163 6b54 7970  lpostFeedbackTyp
+00010860: 6522 0a09 7175 6573 7469 6f6e 3a73 7472  e"..question:str
+00010870: 0a09 616e 7377 6572 733a 4f70 7469 6f6e  ..answers:Option
+00010880: 616c 5b6c 6973 745b 224e 6577 7366 6565  al[list["Newsfee
+00010890: 6449 7465 6d57 616c 6c70 6f73 7446 6565  dItemWallpostFee
+000108a0: 6462 6163 6b41 6e73 7765 7222 5d5d 203d  dbackAnswer"]] =
+000108b0: 204e 6f6e 650a 0973 7461 7273 5f63 6f75   None..stars_cou
+000108c0: 6e74 3a4f 7074 696f 6e61 6c5b 696e 745d  nt:Optional[int]
+000108d0: 203d 204e 6f6e 650a 0967 7261 7469 7475   = None..gratitu
+000108e0: 6465 3a4f 7074 696f 6e61 6c5b 7374 725d  de:Optional[str]
+000108f0: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
+00010900: 4e65 7773 6665 6564 4974 656d 5761 6c6c  NewsfeedItemWall
+00010910: 706f 7374 4665 6564 6261 636b 416e 7377  postFeedbackAnsw
+00010920: 6572 2842 4d29 3a0a 0974 6974 6c65 3a73  er(BM):..title:s
+00010930: 7472 0a09 6964 3a73 7472 0a0a 0a63 6c61  tr..id:str...cla
+00010940: 7373 204e 6577 7366 6565 644c 6973 7428  ss NewsfeedList(
+00010950: 424d 293a 0a09 6964 3a69 6e74 0a09 7469  BM):..id:int..ti
+00010960: 746c 653a 7374 720a 0a0a 636c 6173 7320  tle:str...class 
+00010970: 4e65 7773 6665 6564 4e65 7773 6665 6564  NewsfeedNewsfeed
+00010980: 4974 656d 2842 4d29 3a0a 0970 6173 730a  Item(BM):..pass.
+00010990: 0a0a 0a63 6c61 7373 204e 6f74 6573 4e6f  ...class NotesNo
+000109a0: 7465 2842 4d29 3a0a 0972 6561 645f 636f  te(BM):..read_co
+000109b0: 6d6d 656e 7473 3a4f 7074 696f 6e61 6c5b  mments:Optional[
+000109c0: 696e 745d 203d 204e 6f6e 650a 0963 616e  int] = None..can
+000109d0: 5f63 6f6d 6d65 6e74 3a4f 7074 696f 6e61  _comment:Optiona
+000109e0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
+000109f0: 636f 6d6d 656e 7473 3a69 6e74 0a09 6461  comments:int..da
+00010a00: 7465 3a69 6e74 0a09 6964 3a69 6e74 0a09  te:int..id:int..
+00010a10: 6f77 6e65 725f 6964 3a69 6e74 0a09 7465  owner_id:int..te
+00010a20: 7874 3a4f 7074 696f 6e61 6c5b 7374 725d  xt:Optional[str]
+00010a30: 203d 204e 6f6e 650a 0974 6578 745f 7769   = None..text_wi
+00010a40: 6b69 3a4f 7074 696f 6e61 6c5b 7374 725d  ki:Optional[str]
+00010a50: 203d 204e 6f6e 650a 0974 6974 6c65 3a73   = None..title:s
+00010a60: 7472 0a09 7669 6577 5f75 726c 3a73 7472  tr..view_url:str
+00010a70: 0a09 7072 6976 6163 795f 7669 6577 3a4f  ..privacy_view:O
+00010a80: 7074 696f 6e61 6c5b 6c69 7374 5b73 7472  ptional[list[str
+00010a90: 5d5d 203d 204e 6f6e 650a 0970 7269 7661  ]] = None..priva
+00010aa0: 6379 5f63 6f6d 6d65 6e74 3a4f 7074 696f  cy_comment:Optio
+00010ab0: 6e61 6c5b 6c69 7374 5b73 7472 5d5d 203d  nal[list[str]] =
+00010ac0: 204e 6f6e 650a 0a0a 636c 6173 7320 4e6f   None...class No
+00010ad0: 7465 734e 6f74 6543 6f6d 6d65 6e74 2842  tesNoteComment(B
+00010ae0: 4d29 3a0a 0964 6174 653a 696e 740a 0969  M):..date:int..i
+00010af0: 643a 696e 740a 096d 6573 7361 6765 3a73  d:int..message:s
+00010b00: 7472 0a09 6e69 643a 696e 740a 096f 6964  tr..nid:int..oid
+00010b10: 3a69 6e74 0a09 7265 706c 795f 746f 3a4f  :int..reply_to:O
+00010b20: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00010b30: 6f6e 650a 0975 6964 3a69 6e74 0a0a 0a0a  one..uid:int....
+00010b40: 0a63 6c61 7373 204e 6f74 6966 6963 6174  .class Notificat
+00010b50: 696f 6e73 4665 6564 6261 636b 2842 4d29  ionsFeedback(BM)
+00010b60: 3a0a 0961 7474 6163 686d 656e 7473 3a4f  :..attachments:O
+00010b70: 7074 696f 6e61 6c5b 6c69 7374 5b22 5761  ptional[list["Wa
+00010b80: 6c6c 5761 6c6c 706f 7374 4174 7461 6368  llWallpostAttach
+00010b90: 6d65 6e74 225d 5d20 3d20 4e6f 6e65 0a09  ment"]] = None..
+00010ba0: 6672 6f6d 5f69 643a 4f70 7469 6f6e 616c  from_id:Optional
+00010bb0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6765  [int] = None..ge
+00010bc0: 6f3a 4f70 7469 6f6e 616c 5b22 4261 7365  o:Optional["Base
+00010bd0: 4765 6f22 5d20 3d20 4e6f 6e65 0a09 6964  Geo"] = None..id
+00010be0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00010bf0: 204e 6f6e 650a 096c 696b 6573 3a4f 7074   None..likes:Opt
+00010c00: 696f 6e61 6c5b 2242 6173 654c 696b 6573  ional["BaseLikes
+00010c10: 496e 666f 225d 203d 204e 6f6e 650a 0974  Info"] = None..t
+00010c20: 6578 743a 4f70 7469 6f6e 616c 5b73 7472  ext:Optional[str
+00010c30: 5d20 3d20 4e6f 6e65 0a09 746f 5f69 643a  ] = None..to_id:
+00010c40: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00010c50: 4e6f 6e65 0a0a 0a63 6c61 7373 204e 6f74  None...class Not
+00010c60: 6966 6963 6174 696f 6e73 4e6f 7469 6669  ificationsNotifi
+00010c70: 6361 7469 6f6e 2842 4d29 3a0a 0964 6174  cation(BM):..dat
+00010c80: 653a 4f70 7469 6f6e 616c 5b69 6e74 5d20  e:Optional[int] 
+00010c90: 3d20 4e6f 6e65 0a09 6665 6564 6261 636b  = None..feedback
+00010ca0: 3a4f 7074 696f 6e61 6c5b 224e 6f74 6966  :Optional["Notif
+00010cb0: 6963 6174 696f 6e73 4665 6564 6261 636b  icationsFeedback
+00010cc0: 225d 203d 204e 6f6e 650a 0970 6172 656e  "] = None..paren
+00010cd0: 743a 4f70 7469 6f6e 616c 5b22 4e6f 7469  t:Optional["Noti
+00010ce0: 6669 6361 7469 6f6e 734e 6f74 6966 6963  ficationsNotific
+00010cf0: 6174 696f 6e22 5d20 3d20 4e6f 6e65 0a09  ation"] = None..
+00010d00: 7265 706c 793a 4f70 7469 6f6e 616c 5b22  reply:Optional["
+00010d10: 4e6f 7469 6669 6361 7469 6f6e 7352 6570  NotificationsRep
+00010d20: 6c79 225d 203d 204e 6f6e 650a 0974 7970  ly"] = None..typ
+00010d30: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
+00010d40: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 204e  = None...class N
+00010d50: 6f74 6966 6963 6174 696f 6e73 4e6f 7469  otificationsNoti
+00010d60: 6669 6361 7469 6f6e 4974 656d 2842 4d29  ficationItem(BM)
+00010d70: 3a0a 0970 6173 730a 0a63 6c61 7373 204e  :..pass..class N
+00010d80: 6f74 6966 6963 6174 696f 6e73 4e6f 7469  otificationsNoti
+00010d90: 6669 6361 7469 6f6e 7343 6f6d 6d65 6e74  ficationsComment
+00010da0: 2842 4d29 3a0a 0964 6174 653a 4f70 7469  (BM):..date:Opti
+00010db0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00010dc0: 0a09 6964 3a4f 7074 696f 6e61 6c5b 696e  ..id:Optional[in
+00010dd0: 745d 203d 204e 6f6e 650a 096f 776e 6572  t] = None..owner
+00010de0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
+00010df0: 5d20 3d20 4e6f 6e65 0a09 7068 6f74 6f3a  ] = None..photo:
+00010e00: 4f70 7469 6f6e 616c 5b22 5068 6f74 6f73  Optional["Photos
+00010e10: 5068 6f74 6f22 5d20 3d20 4e6f 6e65 0a09  Photo"] = None..
+00010e20: 706f 7374 3a4f 7074 696f 6e61 6c5b 2257  post:Optional["W
+00010e30: 616c 6c57 616c 6c70 6f73 7422 5d20 3d20  allWallpost"] = 
+00010e40: 4e6f 6e65 0a09 7465 7874 3a4f 7074 696f  None..text:Optio
+00010e50: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00010e60: 0974 6f70 6963 3a4f 7074 696f 6e61 6c5b  .topic:Optional[
+00010e70: 2242 6f61 7264 546f 7069 6322 5d20 3d20  "BoardTopic"] = 
+00010e80: 4e6f 6e65 0a09 7669 6465 6f3a 4f70 7469  None..video:Opti
+00010e90: 6f6e 616c 5b22 5669 6465 6f56 6964 656f  onal["VideoVideo
+00010ea0: 225d 203d 204e 6f6e 650a 0a0a 636c 6173  "] = None...clas
+00010eb0: 7320 4e6f 7469 6669 6361 7469 6f6e 7352  s NotificationsR
+00010ec0: 6570 6c79 2842 4d29 3a0a 0964 6174 653a  eply(BM):..date:
+00010ed0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00010ee0: 4e6f 6e65 0a09 6964 3a4f 7074 696f 6e61  None..id:Optiona
+00010ef0: 6c5b 696e 745d 203d 204e 6f6e 650a 0974  l[int] = None..t
+00010f00: 6578 743a 4f70 7469 6f6e 616c 5b69 6e74  ext:Optional[int
+00010f10: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+00010f20: 204e 6f74 6966 6963 6174 696f 6e73 5365   NotificationsSe
+00010f30: 6e64 4d65 7373 6167 6545 7272 6f72 2842  ndMessageError(B
+00010f40: 4d29 3a0a 0963 6f64 653a 4f70 7469 6f6e  M):..code:Option
+00010f50: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00010f60: 6465 7363 7269 7074 696f 6e3a 4f70 7469  description:Opti
+00010f70: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00010f80: 0a0a 0a63 6c61 7373 204e 6f74 6966 6963  ...class Notific
+00010f90: 6174 696f 6e73 5365 6e64 4d65 7373 6167  ationsSendMessag
+00010fa0: 6549 7465 6d28 424d 293a 0a09 7573 6572  eItem(BM):..user
+00010fb0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
+00010fc0: 5d20 3d20 4e6f 6e65 0a09 7374 6174 7573  ] = None..status
+00010fd0: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+00010fe0: 3d20 4e6f 6e65 0a09 6572 726f 723a 4f70  = None..error:Op
+00010ff0: 7469 6f6e 616c 5b22 4e6f 7469 6669 6361  tional["Notifica
+00011000: 7469 6f6e 7353 656e 644d 6573 7361 6765  tionsSendMessage
+00011010: 4572 726f 7222 5d20 3d20 4e6f 6e65 0a0a  Error"] = None..
+00011020: 0a0a 0a63 6c61 7373 204f 6175 7468 4572  ...class OauthEr
+00011030: 726f 7228 424d 293a 0a09 6572 726f 723a  ror(BM):..error:
+00011040: 7374 720a 0965 7272 6f72 5f64 6573 6372  str..error_descr
+00011050: 6970 7469 6f6e 3a73 7472 0a09 7265 6469  iption:str..redi
+00011060: 7265 6374 5f75 7269 3a4f 7074 696f 6e61  rect_uri:Optiona
+00011070: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
+00011080: 0a0a 636c 6173 7320 4f72 6465 7273 416d  ..class OrdersAm
+00011090: 6f75 6e74 2842 4d29 3a0a 0961 6d6f 756e  ount(BM):..amoun
+000110a0: 7473 3a4f 7074 696f 6e61 6c5b 6c69 7374  ts:Optional[list
+000110b0: 5b22 4f72 6465 7273 416d 6f75 6e74 4974  ["OrdersAmountIt
+000110c0: 656d 225d 5d20 3d20 4e6f 6e65 0a09 6375  em"]] = None..cu
+000110d0: 7272 656e 6379 3a4f 7074 696f 6e61 6c5b  rrency:Optional[
+000110e0: 7374 725d 203d 204e 6f6e 650a 0a0a 636c  str] = None...cl
+000110f0: 6173 7320 4f72 6465 7273 416d 6f75 6e74  ass OrdersAmount
+00011100: 4974 656d 2842 4d29 3a0a 0961 6d6f 756e  Item(BM):..amoun
+00011110: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
+00011120: 3d20 4e6f 6e65 0a09 6465 7363 7269 7074  = None..descript
+00011130: 696f 6e3a 4f70 7469 6f6e 616c 5b73 7472  ion:Optional[str
+00011140: 5d20 3d20 4e6f 6e65 0a09 766f 7465 733a  ] = None..votes:
+00011150: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00011160: 4e6f 6e65 0a0a 0a63 6c61 7373 204f 7264  None...class Ord
+00011170: 6572 734f 7264 6572 2842 4d29 3a0a 0961  ersOrder(BM):..a
+00011180: 6d6f 756e 743a 7374 720a 0961 7070 5f6f  mount:str..app_o
+00011190: 7264 6572 5f69 643a 7374 720a 0963 616e  rder_id:str..can
+000111a0: 6365 6c5f 7472 616e 7361 6374 696f 6e5f  cel_transaction_
+000111b0: 6964 3a4f 7074 696f 6e61 6c5b 7374 725d  id:Optional[str]
+000111c0: 203d 204e 6f6e 650a 0964 6174 653a 7374   = None..date:st
+000111d0: 720a 0969 643a 7374 720a 0969 7465 6d3a  r..id:str..item:
+000111e0: 7374 720a 0972 6563 6569 7665 725f 6964  str..receiver_id
+000111f0: 3a73 7472 0a09 7374 6174 7573 3a73 7472  :str..status:str
+00011200: 0a09 7472 616e 7361 6374 696f 6e5f 6964  ..transaction_id
+00011210: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00011220: 204e 6f6e 650a 0975 7365 725f 6964 3a73   None..user_id:s
+00011230: 7472 0a0a 0a63 6c61 7373 204f 7264 6572  tr...class Order
+00011240: 7353 7562 7363 7269 7074 696f 6e28 424d  sSubscription(BM
+00011250: 293a 0a09 6361 6e63 656c 5f72 6561 736f  ):..cancel_reaso
+00011260: 6e3a 4f70 7469 6f6e 616c 5b73 7472 5d20  n:Optional[str] 
+00011270: 3d20 4e6f 6e65 0a09 6372 6561 7465 5f74  = None..create_t
+00011280: 696d 653a 696e 740a 0969 643a 696e 740a  ime:int..id:int.
+00011290: 0969 7465 6d5f 6964 3a73 7472 0a09 6e65  .item_id:str..ne
+000112a0: 7874 5f62 696c 6c5f 7469 6d65 3a4f 7074  xt_bill_time:Opt
+000112b0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000112c0: 650a 0965 7870 6972 655f 7469 6d65 3a4f  e..expire_time:O
+000112d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000112e0: 6f6e 650a 0970 656e 6469 6e67 5f63 616e  one..pending_can
+000112f0: 6365 6c3a 4f70 7469 6f6e 616c 5b62 6f6f  cel:Optional[boo
+00011300: 6c5d 203d 204e 6f6e 650a 0970 6572 696f  l] = None..perio
+00011310: 643a 696e 740a 0970 6572 696f 645f 7374  d:int..period_st
+00011320: 6172 745f 7469 6d65 3a69 6e74 0a09 7072  art_time:int..pr
+00011330: 6963 653a 696e 740a 0974 6974 6c65 3a4f  ice:int..title:O
+00011340: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00011350: 6f6e 650a 0961 7070 5f69 643a 4f70 7469  one..app_id:Opti
+00011360: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00011370: 0a09 6170 706c 6963 6174 696f 6e5f 6e61  ..application_na
+00011380: 6d65 3a4f 7074 696f 6e61 6c5b 7374 725d  me:Optional[str]
+00011390: 203d 204e 6f6e 650a 0970 686f 746f 5f75   = None..photo_u
+000113a0: 726c 3a4f 7074 696f 6e61 6c5b 7374 725d  rl:Optional[str]
+000113b0: 203d 204e 6f6e 650a 0973 7461 7475 733a   = None..status:
+000113c0: 7374 720a 0974 6573 745f 6d6f 6465 3a4f  str..test_mode:O
+000113d0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+000113e0: 4e6f 6e65 0a09 7472 6961 6c5f 6578 7069  None..trial_expi
+000113f0: 7265 5f74 696d 653a 4f70 7469 6f6e 616c  re_time:Optional
+00011400: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7570  [int] = None..up
+00011410: 6461 7465 5f74 696d 653a 696e 740a 0a0a  date_time:int...
+00011420: 0a0a 636c 6173 7320 4f77 6e65 7253 7461  ..class OwnerSta
+00011430: 7465 2842 4d29 3a0a 0973 7461 7465 3a4f  te(BM):..state:O
+00011440: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00011450: 6f6e 650a 0964 6573 6372 6970 7469 6f6e  one..description
+00011460: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00011470: 204e 6f6e 650a 0a0a 0a0a 636c 6173 7320   None.....class 
+00011480: 5061 6765 7350 7269 7661 6379 5365 7474  PagesPrivacySett
+00011490: 696e 6773 2845 6e75 6d29 3a0a 0943 4f4d  ings(Enum):..COM
+000114a0: 4d55 4e49 5459 5f4d 414e 4147 4552 535f  MUNITY_MANAGERS_
+000114b0: 4f4e 4c59 203d 2030 0a09 434f 4d4d 554e  ONLY = 0..COMMUN
+000114c0: 4954 595f 4d45 4d42 4552 535f 4f4e 4c59  ITY_MEMBERS_ONLY
+000114d0: 203d 2031 0a09 4556 4552 594f 4e45 203d   = 1..EVERYONE =
+000114e0: 2032 0a0a 636c 6173 7320 5061 6765 7357   2..class PagesW
+000114f0: 696b 6970 6167 6528 424d 293a 0a09 6372  ikipage(BM):..cr
+00011500: 6561 746f 725f 6964 3a4f 7074 696f 6e61  eator_id:Optiona
+00011510: 6c5b 696e 745d 203d 204e 6f6e 650a 0963  l[int] = None..c
+00011520: 7265 6174 6f72 5f6e 616d 653a 4f70 7469  reator_name:Opti
+00011530: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00011540: 0a09 6564 6974 6f72 5f69 643a 4f70 7469  ..editor_id:Opti
+00011550: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00011560: 0a09 6564 6974 6f72 5f6e 616d 653a 4f70  ..editor_name:Op
+00011570: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00011580: 6e65 0a09 6772 6f75 705f 6964 3a69 6e74  ne..group_id:int
+00011590: 0a09 6964 3a69 6e74 0a09 7469 746c 653a  ..id:int..title:
+000115a0: 7374 720a 0976 6965 7773 3a69 6e74 0a09  str..views:int..
+000115b0: 7768 6f5f 6361 6e5f 6564 6974 3a22 5061  who_can_edit:"Pa
+000115c0: 6765 7350 7269 7661 6379 5365 7474 696e  gesPrivacySettin
+000115d0: 6773 220a 0977 686f 5f63 616e 5f76 6965  gs"..who_can_vie
+000115e0: 773a 2250 6167 6573 5072 6976 6163 7953  w:"PagesPrivacyS
+000115f0: 6574 7469 6e67 7322 0a0a 0a63 6c61 7373  ettings"...class
+00011600: 2050 6167 6573 5769 6b69 7061 6765 4675   PagesWikipageFu
+00011610: 6c6c 2842 4d29 3a0a 0963 7265 6174 6564  ll(BM):..created
+00011620: 3a69 6e74 0a09 6372 6561 746f 725f 6964  :int..creator_id
+00011630: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00011640: 204e 6f6e 650a 0963 7572 7265 6e74 5f75   None..current_u
+00011650: 7365 725f 6361 6e5f 6564 6974 3a4f 7074  ser_can_edit:Opt
+00011660: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00011670: 6e65 0a09 6375 7272 656e 745f 7573 6572  ne..current_user
+00011680: 5f63 616e 5f65 6469 745f 6163 6365 7373  _can_edit_access
+00011690: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+000116a0: 3d20 4e6f 6e65 0a09 6564 6974 6564 3a69  = None..edited:i
+000116b0: 6e74 0a09 6564 6974 6f72 5f69 643a 4f70  nt..editor_id:Op
+000116c0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000116d0: 6e65 0a09 6772 6f75 705f 6964 3a69 6e74  ne..group_id:int
+000116e0: 0a09 6874 6d6c 3a4f 7074 696f 6e61 6c5b  ..html:Optional[
+000116f0: 7374 725d 203d 204e 6f6e 650a 0969 643a  str] = None..id:
+00011700: 696e 740a 0973 6f75 7263 653a 4f70 7469  int..source:Opti
+00011710: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00011720: 0a09 7469 746c 653a 7374 720a 0976 6965  ..title:str..vie
+00011730: 775f 7572 6c3a 7374 720a 0976 6965 7773  w_url:str..views
+00011740: 3a69 6e74 0a09 7768 6f5f 6361 6e5f 6564  :int..who_can_ed
+00011750: 6974 3a22 5061 6765 7350 7269 7661 6379  it:"PagesPrivacy
+00011760: 5365 7474 696e 6773 220a 0977 686f 5f63  Settings"..who_c
+00011770: 616e 5f76 6965 773a 2250 6167 6573 5072  an_view:"PagesPr
+00011780: 6976 6163 7953 6574 7469 6e67 7322 0a09  ivacySettings"..
+00011790: 7572 6c3a 4f70 7469 6f6e 616c 5b73 7472  url:Optional[str
+000117a0: 5d20 3d20 4e6f 6e65 0a09 7061 7265 6e74  ] = None..parent
+000117b0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+000117c0: 204e 6f6e 650a 0970 6172 656e 7432 3a4f   None..parent2:O
+000117d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000117e0: 6f6e 650a 096f 776e 6572 5f69 643a 4f70  one..owner_id:Op
+000117f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00011800: 6e65 0a0a 0a63 6c61 7373 2050 6167 6573  ne...class Pages
+00011810: 5769 6b69 7061 6765 4869 7374 6f72 7928  WikipageHistory(
+00011820: 424d 293a 0a09 6964 3a69 6e74 0a09 6c65  BM):..id:int..le
+00011830: 6e67 7468 3a69 6e74 0a09 6461 7465 3a69  ngth:int..date:i
+00011840: 6e74 0a09 6564 6974 6f72 5f69 643a 696e  nt..editor_id:in
+00011850: 740a 0965 6469 746f 725f 6e61 6d65 3a73  t..editor_name:s
+00011860: 7472 0a0a 0a0a 0a63 6c61 7373 2050 686f  tr.....class Pho
+00011870: 746f 7349 6d61 6765 5479 7065 2845 6e75  tosImageType(Enu
+00011880: 6d29 3a0a 0953 203d 2022 7322 0a09 4d20  m):..S = "s"..M 
+00011890: 3d20 226d 220a 0958 203d 2022 7822 0a09  = "m"..X = "x"..
+000118a0: 4c20 3d20 226c 220a 094f 203d 2022 6f22  L = "l"..O = "o"
+000118b0: 0a09 5020 3d20 2270 220a 0951 203d 2022  ..P = "p"..Q = "
+000118c0: 7122 0a09 5220 3d20 2272 220a 0959 203d  q"..R = "r"..Y =
+000118d0: 2022 7922 0a09 5a20 3d20 227a 220a 0957   "y"..Z = "z"..W
+000118e0: 203d 2022 7722 0a0a 636c 6173 7320 5068   = "w"..class Ph
+000118f0: 6f74 6f73 5068 6f74 6f53 697a 6573 5479  otosPhotoSizesTy
+00011900: 7065 2845 6e75 6d29 3a0a 0953 203d 2022  pe(Enum):..S = "
+00011910: 7322 0a09 4d20 3d20 226d 220a 0958 203d  s"..M = "m"..X =
+00011920: 2022 7822 0a09 4f20 3d20 226f 220a 0950   "x"..O = "o"..P
+00011930: 203d 2022 7022 0a09 5120 3d20 2271 220a   = "p"..Q = "q".
+00011940: 0952 203d 2022 7222 0a09 4b20 3d20 226b  .R = "r"..K = "k
+00011950: 220a 094c 203d 2022 6c22 0a09 5920 3d20  "..L = "l"..Y = 
+00011960: 2279 220a 095a 203d 2022 7a22 0a09 4320  "y"..Z = "z"..C 
+00011970: 3d20 2263 220a 0957 203d 2022 7722 0a09  = "c"..W = "w"..
+00011980: 4120 3d20 2261 220a 0942 203d 2022 6222  A = "a"..B = "b"
+00011990: 0a09 4520 3d20 2265 220a 0949 203d 2022  ..E = "e"..I = "
+000119a0: 6922 0a09 4420 3d20 2264 220a 094a 203d  i"..D = "d"..J =
+000119b0: 2022 6a22 0a09 5445 4d50 203d 2022 7465   "j"..TEMP = "te
+000119c0: 6d70 220a 0948 203d 2022 6822 0a09 4720  mp"..H = "h"..G 
+000119d0: 3d20 2267 220a 094e 203d 2022 6e22 0a09  = "g"..N = "n"..
+000119e0: 4620 3d20 2266 220a 094d 4158 203d 2022  F = "f"..MAX = "
+000119f0: 6d61 7822 0a0a 636c 6173 7320 5068 6f74  max"..class Phot
+00011a00: 6f73 496d 6167 6528 424d 293a 0a09 6865  osImage(BM):..he
+00011a10: 6967 6874 3a4f 7074 696f 6e61 6c5b 696e  ight:Optional[in
+00011a20: 745d 203d 204e 6f6e 650a 0974 7970 653a  t] = None..type:
+00011a30: 4f70 7469 6f6e 616c 5b22 5068 6f74 6f73  Optional["Photos
+00011a40: 496d 6167 6554 7970 6522 5d20 3d20 4e6f  ImageType"] = No
+00011a50: 6e65 0a09 7572 6c3a 4f70 7469 6f6e 616c  ne..url:Optional
+00011a60: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7769  [str] = None..wi
+00011a70: 6474 683a 4f70 7469 6f6e 616c 5b69 6e74  dth:Optional[int
+00011a80: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+00011a90: 2050 686f 746f 7350 686f 746f 2842 4d29   PhotosPhoto(BM)
+00011aa0: 3a0a 0961 6363 6573 735f 6b65 793a 4f70  :..access_key:Op
+00011ab0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00011ac0: 6e65 0a09 616c 6275 6d5f 6964 3a69 6e74  ne..album_id:int
+00011ad0: 0a09 6461 7465 3a69 6e74 0a09 6865 6967  ..date:int..heig
+00011ae0: 6874 3a4f 7074 696f 6e61 6c5b 696e 745d  ht:Optional[int]
+00011af0: 203d 204e 6f6e 650a 0969 643a 696e 740a   = None..id:int.
+00011b00: 0969 6d61 6765 733a 4f70 7469 6f6e 616c  .images:Optional
+00011b10: 5b6c 6973 745b 2250 686f 746f 7349 6d61  [list["PhotosIma
+00011b20: 6765 225d 5d20 3d20 4e6f 6e65 0a09 6c61  ge"]] = None..la
+00011b30: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
+00011b40: 3d20 4e6f 6e65 0a09 6c6f 6e67 3a4f 7074  = None..long:Opt
+00011b50: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00011b60: 650a 096f 776e 6572 5f69 643a 696e 740a  e..owner_id:int.
+00011b70: 0970 686f 746f 5f32 3536 3a4f 7074 696f  .photo_256:Optio
+00011b80: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00011b90: 0963 616e 5f63 6f6d 6d65 6e74 3a4f 7074  .can_comment:Opt
+00011ba0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00011bb0: 6e65 0a09 706c 6163 653a 4f70 7469 6f6e  ne..place:Option
+00011bc0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00011bd0: 706f 7374 5f69 643a 4f70 7469 6f6e 616c  post_id:Optional
+00011be0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7369  [int] = None..si
+00011bf0: 7a65 733a 4f70 7469 6f6e 616c 5b6c 6973  zes:Optional[lis
+00011c00: 745b 2250 686f 746f 7350 686f 746f 5369  t["PhotosPhotoSi
+00011c10: 7a65 7322 5d5d 203d 204e 6f6e 650a 0974  zes"]] = None..t
+00011c20: 6578 743a 4f70 7469 6f6e 616c 5b73 7472  ext:Optional[str
+00011c30: 5d20 3d20 4e6f 6e65 0a09 7573 6572 5f69  ] = None..user_i
+00011c40: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+00011c50: 3d20 4e6f 6e65 0a09 7769 6474 683a 4f70  = None..width:Op
+00011c60: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00011c70: 6e65 0a09 6861 735f 7461 6773 3a62 6f6f  ne..has_tags:boo
+00011c80: 6c0a 096c 696b 6573 3a4f 7074 696f 6e61  l..likes:Optiona
+00011c90: 6c5b 2242 6173 654c 696b 6573 225d 203d  l["BaseLikes"] =
+00011ca0: 204e 6f6e 650a 0963 6f6d 6d65 6e74 733a   None..comments:
+00011cb0: 4f70 7469 6f6e 616c 5b22 4261 7365 4f62  Optional["BaseOb
+00011cc0: 6a65 6374 436f 756e 7422 5d20 3d20 4e6f  jectCount"] = No
+00011cd0: 6e65 0a09 7265 706f 7374 733a 4f70 7469  ne..reposts:Opti
+00011ce0: 6f6e 616c 5b22 4261 7365 5265 706f 7374  onal["BaseRepost
+00011cf0: 7349 6e66 6f22 5d20 3d20 4e6f 6e65 0a09  sInfo"] = None..
+00011d00: 7461 6773 3a4f 7074 696f 6e61 6c5b 2242  tags:Optional["B
+00011d10: 6173 654f 626a 6563 7443 6f75 6e74 225d  aseObjectCount"]
+00011d20: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
+00011d30: 5068 6f74 6f73 5068 6f74 6f41 6c62 756d  PhotosPhotoAlbum
+00011d40: 2842 4d29 3a0a 0963 7265 6174 6564 3a69  (BM):..created:i
+00011d50: 6e74 0a09 6465 7363 7269 7074 696f 6e3a  nt..description:
+00011d60: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00011d70: 4e6f 6e65 0a09 6964 3a69 6e74 0a09 6f77  None..id:int..ow
+00011d80: 6e65 725f 6964 3a69 6e74 0a09 7369 7a65  ner_id:int..size
+00011d90: 3a69 6e74 0a09 7468 756d 623a 4f70 7469  :int..thumb:Opti
+00011da0: 6f6e 616c 5b22 5068 6f74 6f73 5068 6f74  onal["PhotosPhot
+00011db0: 6f22 5d20 3d20 4e6f 6e65 0a09 7469 746c  o"] = None..titl
+00011dc0: 653a 7374 720a 0975 7064 6174 6564 3a69  e:str..updated:i
+00011dd0: 6e74 0a0a 0a63 6c61 7373 2050 686f 746f  nt...class Photo
+00011de0: 7350 686f 746f 416c 6275 6d46 756c 6c28  sPhotoAlbumFull(
+00011df0: 424d 293a 0a09 6361 6e5f 7570 6c6f 6164  BM):..can_upload
+00011e00: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+00011e10: 3d20 4e6f 6e65 0a09 636f 6d6d 656e 7473  = None..comments
+00011e20: 5f64 6973 6162 6c65 643a 4f70 7469 6f6e  _disabled:Option
+00011e30: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+00011e40: 0963 7265 6174 6564 3a69 6e74 0a09 6465  .created:int..de
+00011e50: 7363 7269 7074 696f 6e3a 4f70 7469 6f6e  scription:Option
+00011e60: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00011e70: 6361 6e5f 6465 6c65 7465 3a4f 7074 696f  can_delete:Optio
+00011e80: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00011e90: 0a09 6964 3a69 6e74 0a09 6f77 6e65 725f  ..id:int..owner_
+00011ea0: 6964 3a69 6e74 0a09 7369 7a65 3a69 6e74  id:int..size:int
+00011eb0: 0a09 7369 7a65 733a 4f70 7469 6f6e 616c  ..sizes:Optional
+00011ec0: 5b6c 6973 745b 2250 686f 746f 7350 686f  [list["PhotosPho
+00011ed0: 746f 5369 7a65 7322 5d5d 203d 204e 6f6e  toSizes"]] = Non
+00011ee0: 650a 0974 6875 6d62 5f69 643a 4f70 7469  e..thumb_id:Opti
+00011ef0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00011f00: 0a09 7468 756d 625f 6973 5f6c 6173 743a  ..thumb_is_last:
+00011f10: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00011f20: 204e 6f6e 650a 0974 6875 6d62 5f73 7263   None..thumb_src
+00011f30: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00011f40: 204e 6f6e 650a 0974 6974 6c65 3a73 7472   None..title:str
+00011f50: 0a09 7570 6461 7465 643a 696e 740a 0975  ..updated:int..u
+00011f60: 706c 6f61 645f 6279 5f61 646d 696e 735f  pload_by_admins_
+00011f70: 6f6e 6c79 3a4f 7074 696f 6e61 6c5b 626f  only:Optional[bo
+00011f80: 6f6c 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  ol] = None...cla
+00011f90: 7373 2050 686f 746f 7350 686f 746f 4661  ss PhotosPhotoFa
+00011fa0: 6c73 6561 626c 6528 424d 293a 0a09 7061  lseable(BM):..pa
+00011fb0: 7373 0a0a 636c 6173 7320 5068 6f74 6f73  ss..class Photos
+00011fc0: 5068 6f74 6f46 756c 6c58 7472 5265 616c  PhotoFullXtrReal
+00011fd0: 4f66 6673 6574 2842 4d29 3a0a 0961 6363  Offset(BM):..acc
+00011fe0: 6573 735f 6b65 793a 4f70 7469 6f6e 616c  ess_key:Optional
+00011ff0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 616c  [str] = None..al
+00012000: 6275 6d5f 6964 3a69 6e74 0a09 6361 6e5f  bum_id:int..can_
+00012010: 636f 6d6d 656e 743a 4f70 7469 6f6e 616c  comment:Optional
+00012020: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0963  [bool] = None..c
+00012030: 6f6d 6d65 6e74 733a 4f70 7469 6f6e 616c  omments:Optional
+00012040: 5b22 4261 7365 4f62 6a65 6374 436f 756e  ["BaseObjectCoun
+00012050: 7422 5d20 3d20 4e6f 6e65 0a09 6461 7465  t"] = None..date
+00012060: 3a69 6e74 0a09 6865 6967 6874 3a4f 7074  :int..height:Opt
+00012070: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00012080: 650a 0968 6964 6465 6e3a 4f70 7469 6f6e  e..hidden:Option
+00012090: 616c 5b22 4261 7365 5072 6f70 6572 7479  al["BaseProperty
+000120a0: 4578 6973 7473 225d 203d 204e 6f6e 650a  Exists"] = None.
+000120b0: 0969 643a 696e 740a 096c 6174 3a4f 7074  .id:int..lat:Opt
+000120c0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000120d0: 650a 096c 696b 6573 3a4f 7074 696f 6e61  e..likes:Optiona
+000120e0: 6c5b 2242 6173 654c 696b 6573 225d 203d  l["BaseLikes"] =
+000120f0: 204e 6f6e 650a 096c 6f6e 673a 4f70 7469   None..long:Opti
+00012100: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00012110: 0a09 6f77 6e65 725f 6964 3a69 6e74 0a09  ..owner_id:int..
+00012120: 7068 6f74 6f5f 3132 3830 3a4f 7074 696f  photo_1280:Optio
+00012130: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00012140: 0970 686f 746f 5f31 3330 3a4f 7074 696f  .photo_130:Optio
+00012150: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00012160: 0970 686f 746f 5f32 3536 303a 4f70 7469  .photo_2560:Opti
+00012170: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00012180: 0a09 7068 6f74 6f5f 3630 343a 4f70 7469  ..photo_604:Opti
+00012190: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000121a0: 0a09 7068 6f74 6f5f 3735 3a4f 7074 696f  ..photo_75:Optio
+000121b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000121c0: 0970 686f 746f 5f38 3037 3a4f 7074 696f  .photo_807:Optio
+000121d0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000121e0: 0970 6f73 745f 6964 3a4f 7074 696f 6e61  .post_id:Optiona
+000121f0: 6c5b 696e 745d 203d 204e 6f6e 650a 0972  l[int] = None..r
+00012200: 6561 6c5f 6f66 6673 6574 3a4f 7074 696f  eal_offset:Optio
+00012210: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00012220: 0972 6570 6f73 7473 3a4f 7074 696f 6e61  .reposts:Optiona
+00012230: 6c5b 2242 6173 654f 626a 6563 7443 6f75  l["BaseObjectCou
+00012240: 6e74 225d 203d 204e 6f6e 650a 0973 697a  nt"] = None..siz
+00012250: 6573 3a4f 7074 696f 6e61 6c5b 6c69 7374  es:Optional[list
+00012260: 5b22 5068 6f74 6f73 5068 6f74 6f53 697a  ["PhotosPhotoSiz
+00012270: 6573 225d 5d20 3d20 4e6f 6e65 0a09 7461  es"]] = None..ta
+00012280: 6773 3a4f 7074 696f 6e61 6c5b 2242 6173  gs:Optional["Bas
+00012290: 654f 626a 6563 7443 6f75 6e74 225d 203d  eObjectCount"] =
+000122a0: 204e 6f6e 650a 0974 6578 743a 4f70 7469   None..text:Opti
+000122b0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000122c0: 0a09 7573 6572 5f69 643a 4f70 7469 6f6e  ..user_id:Option
+000122d0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+000122e0: 7769 6474 683a 4f70 7469 6f6e 616c 5b69  width:Optional[i
+000122f0: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  nt] = None...cla
+00012300: 7373 2050 686f 746f 7350 686f 746f 5369  ss PhotosPhotoSi
+00012310: 7a65 7328 424d 293a 0a09 6865 6967 6874  zes(BM):..height
+00012320: 3a69 6e74 0a09 7572 6c3a 7374 720a 0973  :int..url:str..s
+00012330: 7263 3a4f 7074 696f 6e61 6c5b 7374 725d  rc:Optional[str]
+00012340: 203d 204e 6f6e 650a 0974 7970 653a 2250   = None..type:"P
+00012350: 686f 746f 7350 686f 746f 5369 7a65 7354  hotosPhotoSizesT
+00012360: 7970 6522 0a09 7769 6474 683a 696e 740a  ype"..width:int.
+00012370: 0a0a 636c 6173 7320 5068 6f74 6f73 5068  ..class PhotosPh
+00012380: 6f74 6f54 6167 2842 4d29 3a0a 0964 6174  otoTag(BM):..dat
+00012390: 653a 696e 740a 0969 643a 696e 740a 0970  e:int..id:int..p
+000123a0: 6c61 6365 725f 6964 3a69 6e74 0a09 7461  lacer_id:int..ta
+000123b0: 6767 6564 5f6e 616d 653a 7374 720a 0964  gged_name:str..d
+000123c0: 6573 6372 6970 7469 6f6e 3a4f 7074 696f  escription:Optio
+000123d0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000123e0: 0975 7365 725f 6964 3a69 6e74 0a09 7669  .user_id:int..vi
+000123f0: 6577 6564 3a62 6f6f 6c0a 0978 3a69 6e74  ewed:bool..x:int
+00012400: 0a09 7832 3a69 6e74 0a09 793a 696e 740a  ..x2:int..y:int.
+00012410: 0979 323a 696e 740a 0a0a 636c 6173 7320  .y2:int...class 
+00012420: 5068 6f74 6f73 5068 6f74 6f55 706c 6f61  PhotosPhotoUploa
+00012430: 6428 424d 293a 0a09 616c 6275 6d5f 6964  d(BM):..album_id
+00012440: 3a69 6e74 0a09 7570 6c6f 6164 5f75 726c  :int..upload_url
+00012450: 3a73 7472 0a09 6661 6c6c 6261 636b 5f75  :str..fallback_u
+00012460: 706c 6f61 645f 7572 6c3a 4f70 7469 6f6e  pload_url:Option
+00012470: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00012480: 7573 6572 5f69 643a 696e 740a 0967 726f  user_id:int..gro
+00012490: 7570 5f69 643a 4f70 7469 6f6e 616c 5b69  up_id:Optional[i
+000124a0: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  nt] = None...cla
+000124b0: 7373 2050 686f 746f 7350 686f 746f 5874  ss PhotosPhotoXt
+000124c0: 7252 6561 6c4f 6666 7365 7428 424d 293a  rRealOffset(BM):
+000124d0: 0a09 6163 6365 7373 5f6b 6579 3a4f 7074  ..access_key:Opt
+000124e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+000124f0: 650a 0961 6c62 756d 5f69 643a 696e 740a  e..album_id:int.
+00012500: 0964 6174 653a 696e 740a 0968 6569 6768  .date:int..heigh
+00012510: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
+00012520: 3d20 4e6f 6e65 0a09 6869 6464 656e 3a4f  = None..hidden:O
+00012530: 7074 696f 6e61 6c5b 2242 6173 6550 726f  ptional["BasePro
+00012540: 7065 7274 7945 7869 7374 7322 5d20 3d20  pertyExists"] = 
+00012550: 4e6f 6e65 0a09 6964 3a69 6e74 0a09 6c61  None..id:int..la
+00012560: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
+00012570: 3d20 4e6f 6e65 0a09 6c6f 6e67 3a4f 7074  = None..long:Opt
+00012580: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00012590: 650a 096f 776e 6572 5f69 643a 696e 740a  e..owner_id:int.
+000125a0: 0970 686f 746f 5f31 3238 303a 4f70 7469  .photo_1280:Opti
+000125b0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000125c0: 0a09 7068 6f74 6f5f 3133 303a 4f70 7469  ..photo_130:Opti
+000125d0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000125e0: 0a09 7068 6f74 6f5f 3235 3630 3a4f 7074  ..photo_2560:Opt
+000125f0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00012600: 650a 0970 686f 746f 5f36 3034 3a4f 7074  e..photo_604:Opt
+00012610: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00012620: 650a 0970 686f 746f 5f37 353a 4f70 7469  e..photo_75:Opti
+00012630: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00012640: 0a09 7068 6f74 6f5f 3830 373a 4f70 7469  ..photo_807:Opti
+00012650: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00012660: 0a09 706f 7374 5f69 643a 4f70 7469 6f6e  ..post_id:Option
+00012670: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00012680: 7265 616c 5f6f 6666 7365 743a 4f70 7469  real_offset:Opti
+00012690: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000126a0: 0a09 7369 7a65 733a 4f70 7469 6f6e 616c  ..sizes:Optional
+000126b0: 5b6c 6973 745b 2250 686f 746f 7350 686f  [list["PhotosPho
+000126c0: 746f 5369 7a65 7322 5d5d 203d 204e 6f6e  toSizes"]] = Non
+000126d0: 650a 0974 6578 743a 4f70 7469 6f6e 616c  e..text:Optional
+000126e0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7573  [str] = None..us
+000126f0: 6572 5f69 643a 4f70 7469 6f6e 616c 5b69  er_id:Optional[i
+00012700: 6e74 5d20 3d20 4e6f 6e65 0a09 7769 6474  nt] = None..widt
+00012710: 683a 4f70 7469 6f6e 616c 5b69 6e74 5d20  h:Optional[int] 
+00012720: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2050  = None...class P
+00012730: 686f 746f 7350 686f 746f 5874 7254 6167  hotosPhotoXtrTag
+00012740: 496e 666f 2842 4d29 3a0a 0961 6363 6573  Info(BM):..acces
+00012750: 735f 6b65 793a 4f70 7469 6f6e 616c 5b73  s_key:Optional[s
+00012760: 7472 5d20 3d20 4e6f 6e65 0a09 616c 6275  tr] = None..albu
+00012770: 6d5f 6964 3a69 6e74 0a09 6461 7465 3a69  m_id:int..date:i
+00012780: 6e74 0a09 6865 6967 6874 3a4f 7074 696f  nt..height:Optio
+00012790: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+000127a0: 0969 643a 696e 740a 096c 6174 3a4f 7074  .id:int..lat:Opt
+000127b0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000127c0: 650a 096c 6f6e 673a 4f70 7469 6f6e 616c  e..long:Optional
+000127d0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6f77  [int] = None..ow
+000127e0: 6e65 725f 6964 3a69 6e74 0a09 7068 6f74  ner_id:int..phot
+000127f0: 6f5f 3132 3830 3a4f 7074 696f 6e61 6c5b  o_1280:Optional[
+00012800: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
+00012810: 746f 5f31 3330 3a4f 7074 696f 6e61 6c5b  to_130:Optional[
+00012820: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
+00012830: 746f 5f32 3536 303a 4f70 7469 6f6e 616c  to_2560:Optional
+00012840: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7068  [str] = None..ph
+00012850: 6f74 6f5f 3630 343a 4f70 7469 6f6e 616c  oto_604:Optional
+00012860: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7068  [str] = None..ph
+00012870: 6f74 6f5f 3735 3a4f 7074 696f 6e61 6c5b  oto_75:Optional[
+00012880: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
+00012890: 746f 5f38 3037 3a4f 7074 696f 6e61 6c5b  to_807:Optional[
+000128a0: 7374 725d 203d 204e 6f6e 650a 0970 6c61  str] = None..pla
+000128b0: 6365 725f 6964 3a4f 7074 696f 6e61 6c5b  cer_id:Optional[
+000128c0: 696e 745d 203d 204e 6f6e 650a 0970 6f73  int] = None..pos
+000128d0: 745f 6964 3a4f 7074 696f 6e61 6c5b 696e  t_id:Optional[in
+000128e0: 745d 203d 204e 6f6e 650a 0973 697a 6573  t] = None..sizes
+000128f0: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
+00012900: 5068 6f74 6f73 5068 6f74 6f53 697a 6573  PhotosPhotoSizes
+00012910: 225d 5d20 3d20 4e6f 6e65 0a09 7461 675f  "]] = None..tag_
+00012920: 6372 6561 7465 643a 4f70 7469 6f6e 616c  created:Optional
+00012930: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7461  [int] = None..ta
+00012940: 675f 6964 3a4f 7074 696f 6e61 6c5b 696e  g_id:Optional[in
+00012950: 745d 203d 204e 6f6e 650a 0974 6578 743a  t] = None..text:
+00012960: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00012970: 4e6f 6e65 0a09 7573 6572 5f69 643a 4f70  None..user_id:Op
+00012980: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00012990: 6e65 0a09 7769 6474 683a 4f70 7469 6f6e  ne..width:Option
+000129a0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
+000129b0: 0a63 6c61 7373 2050 686f 746f 7354 6167  .class PhotosTag
+000129c0: 7353 7567 6765 7374 696f 6e49 7465 6d28  sSuggestionItem(
+000129d0: 424d 293a 0a09 7469 746c 653a 4f70 7469  BM):..title:Opti
+000129e0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000129f0: 0a09 6361 7074 696f 6e3a 4f70 7469 6f6e  ..caption:Option
+00012a00: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00012a10: 7479 7065 3a4f 7074 696f 6e61 6c5b 7374  type:Optional[st
+00012a20: 725d 203d 204e 6f6e 650a 0962 7574 746f  r] = None..butto
+00012a30: 6e73 3a4f 7074 696f 6e61 6c5b 6c69 7374  ns:Optional[list
+00012a40: 5b22 5068 6f74 6f73 5461 6773 5375 6767  ["PhotosTagsSugg
+00012a50: 6573 7469 6f6e 4974 656d 4275 7474 6f6e  estionItemButton
+00012a60: 225d 5d20 3d20 4e6f 6e65 0a09 7068 6f74  "]] = None..phot
+00012a70: 6f3a 4f70 7469 6f6e 616c 5b22 5068 6f74  o:Optional["Phot
+00012a80: 6f73 5068 6f74 6f22 5d20 3d20 4e6f 6e65  osPhoto"] = None
+00012a90: 0a09 7461 6773 3a4f 7074 696f 6e61 6c5b  ..tags:Optional[
+00012aa0: 6c69 7374 5b22 5068 6f74 6f73 5068 6f74  list["PhotosPhot
+00012ab0: 6f54 6167 225d 5d20 3d20 4e6f 6e65 0a09  oTag"]] = None..
+00012ac0: 7472 6163 6b5f 636f 6465 3a4f 7074 696f  track_code:Optio
+00012ad0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00012ae0: 0a0a 636c 6173 7320 5068 6f74 6f73 5461  ..class PhotosTa
+00012af0: 6773 5375 6767 6573 7469 6f6e 4974 656d  gsSuggestionItem
+00012b00: 4275 7474 6f6e 2842 4d29 3a0a 0974 6974  Button(BM):..tit
+00012b10: 6c65 3a4f 7074 696f 6e61 6c5b 7374 725d  le:Optional[str]
+00012b20: 203d 204e 6f6e 650a 0961 6374 696f 6e3a   = None..action:
+00012b30: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00012b40: 4e6f 6e65 0a09 7374 796c 653a 4f70 7469  None..style:Opti
+00012b50: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00012b60: 0a0a 0a0a 0a63 6c61 7373 2050 6f64 6361  .....class Podca
+00012b70: 7374 436f 7665 7228 424d 293a 0a09 7369  stCover(BM):..si
+00012b80: 7a65 733a 4f70 7469 6f6e 616c 5b6c 6973  zes:Optional[lis
+00012b90: 745b 2250 686f 746f 7350 686f 746f 5369  t["PhotosPhotoSi
+00012ba0: 7a65 7322 5d5d 203d 204e 6f6e 650a 0a0a  zes"]] = None...
+00012bb0: 636c 6173 7320 506f 6463 6173 7445 7874  class PodcastExt
+00012bc0: 6572 6e61 6c44 6174 6128 424d 293a 0a09  ernalData(BM):..
+00012bd0: 7572 6c3a 4f70 7469 6f6e 616c 5b73 7472  url:Optional[str
+00012be0: 5d20 3d20 4e6f 6e65 0a09 6f77 6e65 725f  ] = None..owner_
+00012bf0: 7572 6c3a 4f70 7469 6f6e 616c 5b73 7472  url:Optional[str
+00012c00: 5d20 3d20 4e6f 6e65 0a09 7469 746c 653a  ] = None..title:
+00012c10: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00012c20: 4e6f 6e65 0a09 6f77 6e65 725f 6e61 6d65  None..owner_name
+00012c30: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00012c40: 204e 6f6e 650a 0963 6f76 6572 3a4f 7074   None..cover:Opt
+00012c50: 696f 6e61 6c5b 2250 6f64 6361 7374 436f  ional["PodcastCo
+00012c60: 7665 7222 5d20 3d20 4e6f 6e65 0a0a 0a0a  ver"] = None....
+00012c70: 0a63 6c61 7373 2050 6f6c 6c73 416e 7377  .class PollsAnsw
+00012c80: 6572 2842 4d29 3a0a 0969 643a 696e 740a  er(BM):..id:int.
+00012c90: 0972 6174 653a 696e 740a 0974 6578 743a  .rate:int..text:
+00012ca0: 7374 720a 0976 6f74 6573 3a69 6e74 0a0a  str..votes:int..
+00012cb0: 0a63 6c61 7373 2050 6f6c 6c73 4261 636b  .class PollsBack
+00012cc0: 6772 6f75 6e64 2842 4d29 3a0a 0961 6e67  ground(BM):..ang
+00012cd0: 6c65 3a4f 7074 696f 6e61 6c5b 696e 745d  le:Optional[int]
+00012ce0: 203d 204e 6f6e 650a 0963 6f6c 6f72 3a4f   = None..color:O
+00012cf0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00012d00: 6f6e 650a 0968 6569 6768 743a 4f70 7469  one..height:Opti
+00012d10: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00012d20: 0a09 6964 3a4f 7074 696f 6e61 6c5b 696e  ..id:Optional[in
+00012d30: 745d 203d 204e 6f6e 650a 096e 616d 653a  t] = None..name:
+00012d40: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00012d50: 4e6f 6e65 0a09 696d 6167 6573 3a4f 7074  None..images:Opt
+00012d60: 696f 6e61 6c5b 6c69 7374 5b22 4261 7365  ional[list["Base
+00012d70: 496d 6167 6522 5d5d 203d 204e 6f6e 650a  Image"]] = None.
+00012d80: 0970 6f69 6e74 733a 4f70 7469 6f6e 616c  .points:Optional
+00012d90: 5b6c 6973 745b 2242 6173 6547 7261 6469  [list["BaseGradi
+00012da0: 656e 7450 6f69 6e74 225d 5d20 3d20 4e6f  entPoint"]] = No
+00012db0: 6e65 0a09 7479 7065 3a4f 7074 696f 6e61  ne..type:Optiona
+00012dc0: 6c5b 7374 725d 203d 204e 6f6e 650a 0977  l[str] = None..w
+00012dd0: 6964 7468 3a4f 7074 696f 6e61 6c5b 696e  idth:Optional[in
+00012de0: 745d 203d 204e 6f6e 650a 0a0a 636c 6173  t] = None...clas
+00012df0: 7320 506f 6c6c 7346 7269 656e 6428 424d  s PollsFriend(BM
+00012e00: 293a 0a09 6964 3a69 6e74 0a0a 0a63 6c61  ):..id:int...cla
+00012e10: 7373 2050 6f6c 6c73 506f 6c6c 2842 4d29  ss PollsPoll(BM)
+00012e20: 3a0a 0961 6e6f 6e79 6d6f 7573 3a4f 7074  :..anonymous:Opt
+00012e30: 696f 6e61 6c5b 2250 6f6c 6c73 506f 6c6c  ional["PollsPoll
+00012e40: 416e 6f6e 796d 6f75 7322 5d20 3d20 4e6f  Anonymous"] = No
+00012e50: 6e65 0a09 6672 6965 6e64 733a 4f70 7469  ne..friends:Opti
+00012e60: 6f6e 616c 5b6c 6973 745b 2250 6f6c 6c73  onal[list["Polls
+00012e70: 4672 6965 6e64 225d 5d20 3d20 4e6f 6e65  Friend"]] = None
+00012e80: 0a09 6d75 6c74 6970 6c65 3a62 6f6f 6c0a  ..multiple:bool.
+00012e90: 0961 6e73 7765 725f 6964 3a4f 7074 696f  .answer_id:Optio
+00012ea0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00012eb0: 0965 6e64 5f64 6174 653a 696e 740a 0961  .end_date:int..a
+00012ec0: 6e73 7765 725f 6964 733a 4f70 7469 6f6e  nswer_ids:Option
+00012ed0: 616c 5b6c 6973 745b 696e 745d 5d20 3d20  al[list[int]] = 
+00012ee0: 4e6f 6e65 0a09 636c 6f73 6564 3a62 6f6f  None..closed:boo
+00012ef0: 6c0a 0969 735f 626f 6172 643a 626f 6f6c  l..is_board:bool
+00012f00: 0a09 6361 6e5f 6564 6974 3a62 6f6f 6c0a  ..can_edit:bool.
+00012f10: 0963 616e 5f76 6f74 653a 626f 6f6c 0a09  .can_vote:bool..
+00012f20: 6361 6e5f 7265 706f 7274 3a62 6f6f 6c0a  can_report:bool.
+00012f30: 0963 616e 5f73 6861 7265 3a62 6f6f 6c0a  .can_share:bool.
+00012f40: 0965 6d62 6564 5f68 6173 683a 4f70 7469  .embed_hash:Opti
+00012f50: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00012f60: 0a09 7068 6f74 6f3a 4f70 7469 6f6e 616c  ..photo:Optional
+00012f70: 5b22 506f 6c6c 7342 6163 6b67 726f 756e  ["PollsBackgroun
+00012f80: 6422 5d20 3d20 4e6f 6e65 0a09 616e 7377  d"] = None..answ
+00012f90: 6572 733a 6c69 7374 5b22 506f 6c6c 7341  ers:list["PollsA
+00012fa0: 6e73 7765 7222 5d0a 0963 7265 6174 6564  nswer"]..created
+00012fb0: 3a69 6e74 0a09 6964 3a69 6e74 0a09 6f77  :int..id:int..ow
+00012fc0: 6e65 725f 6964 3a69 6e74 0a09 6175 7468  ner_id:int..auth
+00012fd0: 6f72 5f69 643a 4f70 7469 6f6e 616c 5b69  or_id:Optional[i
+00012fe0: 6e74 5d20 3d20 4e6f 6e65 0a09 7175 6573  nt] = None..ques
+00012ff0: 7469 6f6e 3a73 7472 0a09 6261 636b 6772  tion:str..backgr
+00013000: 6f75 6e64 3a4f 7074 696f 6e61 6c5b 2250  ound:Optional["P
+00013010: 6f6c 6c73 4261 636b 6772 6f75 6e64 225d  ollsBackground"]
+00013020: 203d 204e 6f6e 650a 0976 6f74 6573 3a69   = None..votes:i
+00013030: 6e74 0a09 6469 7361 626c 655f 756e 766f  nt..disable_unvo
+00013040: 7465 3a62 6f6f 6c0a 0a0a 636c 6173 7320  te:bool...class 
+00013050: 506f 6c6c 7350 6f6c 6c41 6e6f 6e79 6d6f  PollsPollAnonymo
+00013060: 7573 2842 4d29 3a0a 0970 6173 730a 0a63  us(BM):..pass..c
+00013070: 6c61 7373 2050 6f6c 6c73 566f 7465 7273  lass PollsVoters
+00013080: 2842 4d29 3a0a 0961 6e73 7765 725f 6964  (BM):..answer_id
+00013090: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+000130a0: 204e 6f6e 650a 0975 7365 7273 3a4f 7074   None..users:Opt
+000130b0: 696f 6e61 6c5b 2250 6f6c 6c73 566f 7465  ional["PollsVote
+000130c0: 7273 5573 6572 7322 5d20 3d20 4e6f 6e65  rsUsers"] = None
+000130d0: 0a0a 0a63 6c61 7373 2050 6f6c 6c73 566f  ...class PollsVo
+000130e0: 7465 7273 5573 6572 7328 424d 293a 0a09  tersUsers(BM):..
+000130f0: 636f 756e 743a 4f70 7469 6f6e 616c 5b69  count:Optional[i
+00013100: 6e74 5d20 3d20 4e6f 6e65 0a09 6974 656d  nt] = None..item
+00013110: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
+00013120: 696e 745d 5d20 3d20 4e6f 6e65 0a0a 0a0a  int]] = None....
+00013130: 0a63 6c61 7373 2050 7265 7474 7943 6172  .class PrettyCar
+00013140: 6473 5072 6574 7479 4361 7264 2842 4d29  dsPrettyCard(BM)
+00013150: 3a0a 0962 7574 746f 6e3a 4f70 7469 6f6e  :..button:Option
+00013160: 616c 5b55 6e69 6f6e 5b73 7472 2c22 4261  al[Union[str,"Ba
+00013170: 7365 4c69 6e6b 4275 7474 6f6e 225d 5d20  seLinkButton"]] 
+00013180: 3d20 4e6f 6e65 0a09 6275 7474 6f6e 5f74  = None..button_t
+00013190: 6578 743a 4f70 7469 6f6e 616c 5b73 7472  ext:Optional[str
+000131a0: 5d20 3d20 4e6f 6e65 0a09 6361 7264 5f69  ] = None..card_i
+000131b0: 643a 7374 720a 0969 6d61 6765 733a 4f70  d:str..images:Op
+000131c0: 7469 6f6e 616c 5b6c 6973 745b 2242 6173  tional[list["Bas
+000131d0: 6549 6d61 6765 225d 5d20 3d20 4e6f 6e65  eImage"]] = None
+000131e0: 0a09 6c69 6e6b 5f75 726c 3a73 7472 0a09  ..link_url:str..
+000131f0: 7068 6f74 6f3a 7374 720a 0970 7269 6365  photo:str..price
+00013200: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00013210: 204e 6f6e 650a 0970 7269 6365 5f6f 6c64   None..price_old
+00013220: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00013230: 204e 6f6e 650a 0974 6974 6c65 3a73 7472   None..title:str
+00013240: 0a0a 0a63 6c61 7373 2050 7265 7474 7943  ...class PrettyC
+00013250: 6172 6473 5072 6574 7479 4361 7264 4f72  ardsPrettyCardOr
+00013260: 4572 726f 7228 424d 293a 0a09 7061 7373  Error(BM):..pass
+00013270: 0a0a 0a0a 636c 6173 7320 5365 6172 6368  ....class Search
+00013280: 4869 6e74 5365 6374 696f 6e28 456e 756d  HintSection(Enum
+00013290: 293a 0a09 4752 4f55 5053 203d 2022 6772  ):..GROUPS = "gr
+000132a0: 6f75 7073 220a 0945 5645 4e54 5320 3d20  oups"..EVENTS = 
+000132b0: 2265 7665 6e74 7322 0a09 5055 424c 4943  "events"..PUBLIC
+000132c0: 5320 3d20 2270 7562 6c69 6373 220a 0943  S = "publics"..C
+000132d0: 4f52 5245 5350 4f4e 4445 4e54 5320 3d20  ORRESPONDENTS = 
+000132e0: 2263 6f72 7265 7370 6f6e 6465 6e74 7322  "correspondents"
+000132f0: 0a09 5045 4f50 4c45 203d 2022 7065 6f70  ..PEOPLE = "peop
+00013300: 6c65 220a 0946 5249 454e 4453 203d 2022  le"..FRIENDS = "
+00013310: 6672 6965 6e64 7322 0a09 4d55 5455 414c  friends"..MUTUAL
+00013320: 5f46 5249 454e 4453 203d 2022 6d75 7475  _FRIENDS = "mutu
+00013330: 616c 5f66 7269 656e 6473 220a 0950 524f  al_friends"..PRO
+00013340: 4d4f 203d 2022 7072 6f6d 6f22 0a0a 636c  MO = "promo"..cl
+00013350: 6173 7320 5365 6172 6368 4869 6e74 5479  ass SearchHintTy
+00013360: 7065 2845 6e75 6d29 3a0a 0947 524f 5550  pe(Enum):..GROUP
+00013370: 203d 2022 6772 6f75 7022 0a09 5052 4f46   = "group"..PROF
+00013380: 494c 4520 3d20 2270 726f 6669 6c65 220a  ILE = "profile".
+00013390: 0956 4b5f 4150 5020 3d20 2276 6b5f 6170  .VK_APP = "vk_ap
+000133a0: 7022 0a09 4150 5020 3d20 2261 7070 220a  p"..APP = "app".
+000133b0: 0948 544d 4c35 5f47 414d 4520 3d20 2268  .HTML5_GAME = "h
+000133c0: 746d 6c35 5f67 616d 6522 0a09 4c49 4e4b  tml5_game"..LINK
+000133d0: 203d 2022 6c69 6e6b 220a 0a63 6c61 7373   = "link"..class
+000133e0: 2053 6561 7263 6848 696e 7428 424d 293a   SearchHint(BM):
+000133f0: 0a09 6170 703a 4f70 7469 6f6e 616c 5b22  ..app:Optional["
+00013400: 4170 7073 4170 7022 5d20 3d20 4e6f 6e65  AppsApp"] = None
+00013410: 0a09 6465 7363 7269 7074 696f 6e3a 7374  ..description:st
+00013420: 720a 095f 676c 6f62 616c 3a4f 7074 696f  r.._global:Optio
+00013430: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+00013440: 0a09 6772 6f75 703a 4f70 7469 6f6e 616c  ..group:Optional
+00013450: 5b22 4772 6f75 7073 4772 6f75 7022 5d20  ["GroupsGroup"] 
+00013460: 3d20 4e6f 6e65 0a09 7072 6f66 696c 653a  = None..profile:
+00013470: 4f70 7469 6f6e 616c 5b22 5573 6572 7355  Optional["UsersU
+00013480: 7365 724d 696e 225d 203d 204e 6f6e 650a  serMin"] = None.
+00013490: 0973 6563 7469 6f6e 3a4f 7074 696f 6e61  .section:Optiona
+000134a0: 6c5b 2253 6561 7263 6848 696e 7453 6563  l["SearchHintSec
+000134b0: 7469 6f6e 225d 203d 204e 6f6e 650a 0974  tion"] = None..t
+000134c0: 7970 653a 2253 6561 7263 6848 696e 7454  ype:"SearchHintT
+000134d0: 7970 6522 0a09 6c69 6e6b 3a4f 7074 696f  ype"..link:Optio
+000134e0: 6e61 6c5b 2242 6173 654c 696e 6b22 5d20  nal["BaseLink"] 
+000134f0: 3d20 4e6f 6e65 0a0a 0a0a 0a63 6c61 7373  = None.....class
+00013500: 2053 6563 7572 6547 6976 6545 7665 6e74   SecureGiveEvent
+00013510: 5374 6963 6b65 7249 7465 6d28 424d 293a  StickerItem(BM):
+00013520: 0a09 7573 6572 5f69 643a 4f70 7469 6f6e  ..user_id:Option
+00013530: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00013540: 7374 6174 7573 3a4f 7074 696f 6e61 6c5b  status:Optional[
+00013550: 7374 725d 203d 204e 6f6e 650a 0a0a 636c  str] = None...cl
+00013560: 6173 7320 5365 6375 7265 4c65 7665 6c28  ass SecureLevel(
+00013570: 424d 293a 0a09 6c65 7665 6c3a 4f70 7469  BM):..level:Opti
 00013580: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00013590: 0a0a 0a63 6c61 7373 2053 6563 7572 6553  ...class SecureS
-000135a0: 6574 436f 756e 7465 7249 7465 6d28 424d  etCounterItem(BM
-000135b0: 293a 0a09 6964 3a69 6e74 0a09 7265 7375  ):..id:int..resu
-000135c0: 6c74 3a62 6f6f 6c0a 0a0a 636c 6173 7320  lt:bool...class 
-000135d0: 5365 6375 7265 536d 734e 6f74 6966 6963  SecureSmsNotific
-000135e0: 6174 696f 6e28 424d 293a 0a09 6170 705f  ation(BM):..app_
-000135f0: 6964 3a4f 7074 696f 6e61 6c5b 7374 725d  id:Optional[str]
-00013600: 203d 204e 6f6e 650a 0964 6174 653a 4f70   = None..date:Op
-00013610: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00013620: 6e65 0a09 6964 3a4f 7074 696f 6e61 6c5b  ne..id:Optional[
-00013630: 7374 725d 203d 204e 6f6e 650a 096d 6573  str] = None..mes
-00013640: 7361 6765 3a4f 7074 696f 6e61 6c5b 7374  sage:Optional[st
-00013650: 725d 203d 204e 6f6e 650a 0975 7365 725f  r] = None..user_
-00013660: 6964 3a4f 7074 696f 6e61 6c5b 7374 725d  id:Optional[str]
-00013670: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
-00013680: 5365 6375 7265 546f 6b65 6e43 6865 636b  SecureTokenCheck
-00013690: 6564 2842 4d29 3a0a 0964 6174 653a 4f70  ed(BM):..date:Op
-000136a0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000136b0: 6e65 0a09 6578 7069 7265 3a4f 7074 696f  ne..expire:Optio
-000136c0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-000136d0: 0973 7563 6365 7373 3a4f 7074 696f 6e61  .success:Optiona
-000136e0: 6c5b 696e 745d 203d 204e 6f6e 650a 0975  l[int] = None..u
-000136f0: 7365 725f 6964 3a4f 7074 696f 6e61 6c5b  ser_id:Optional[
-00013700: 696e 745d 203d 204e 6f6e 650a 0a0a 636c  int] = None...cl
-00013710: 6173 7320 5365 6375 7265 5472 616e 7361  ass SecureTransa
-00013720: 6374 696f 6e28 424d 293a 0a09 6461 7465  ction(BM):..date
-00013730: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00013740: 204e 6f6e 650a 0969 643a 4f70 7469 6f6e   None..id:Option
-00013750: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00013760: 7569 645f 6672 6f6d 3a4f 7074 696f 6e61  uid_from:Optiona
-00013770: 6c5b 696e 745d 203d 204e 6f6e 650a 0975  l[int] = None..u
-00013780: 6964 5f74 6f3a 4f70 7469 6f6e 616c 5b69  id_to:Optional[i
-00013790: 6e74 5d20 3d20 4e6f 6e65 0a09 766f 7465  nt] = None..vote
-000137a0: 733a 4f70 7469 6f6e 616c 5b69 6e74 5d20  s:Optional[int] 
-000137b0: 3d20 4e6f 6e65 0a0a 0a0a 0a63 6c61 7373  = None.....class
-000137c0: 2053 7461 7473 4163 7469 7669 7479 2842   StatsActivity(B
-000137d0: 4d29 3a0a 0963 6f6d 6d65 6e74 733a 4f70  M):..comments:Op
-000137e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000137f0: 6e65 0a09 636f 7069 6573 3a4f 7074 696f  ne..copies:Optio
-00013800: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00013810: 0968 6964 6465 6e3a 4f70 7469 6f6e 616c  .hidden:Optional
-00013820: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6c69  [int] = None..li
-00013830: 6b65 733a 4f70 7469 6f6e 616c 5b69 6e74  kes:Optional[int
-00013840: 5d20 3d20 4e6f 6e65 0a09 7375 6273 6372  ] = None..subscr
-00013850: 6962 6564 3a4f 7074 696f 6e61 6c5b 696e  ibed:Optional[in
-00013860: 745d 203d 204e 6f6e 650a 0975 6e73 7562  t] = None..unsub
-00013870: 7363 7269 6265 643a 4f70 7469 6f6e 616c  scribed:Optional
-00013880: 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63  [int] = None...c
-00013890: 6c61 7373 2053 7461 7473 4369 7479 2842  lass StatsCity(B
-000138a0: 4d29 3a0a 0963 6f75 6e74 3a4f 7074 696f  M):..count:Optio
-000138b0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-000138c0: 096e 616d 653a 4f70 7469 6f6e 616c 5b73  .name:Optional[s
-000138d0: 7472 5d20 3d20 4e6f 6e65 0a09 7661 6c75  tr] = None..valu
-000138e0: 653a 4f70 7469 6f6e 616c 5b69 6e74 5d20  e:Optional[int] 
-000138f0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2053  = None...class S
-00013900: 7461 7473 436f 756e 7472 7928 424d 293a  tatsCountry(BM):
-00013910: 0a09 636f 6465 3a4f 7074 696f 6e61 6c5b  ..code:Optional[
-00013920: 7374 725d 203d 204e 6f6e 650a 0963 6f75  str] = None..cou
-00013930: 6e74 3a4f 7074 696f 6e61 6c5b 696e 745d  nt:Optional[int]
-00013940: 203d 204e 6f6e 650a 096e 616d 653a 4f70   = None..name:Op
-00013950: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00013960: 6e65 0a09 7661 6c75 653a 4f70 7469 6f6e  ne..value:Option
-00013970: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
-00013980: 0a63 6c61 7373 2053 7461 7473 5065 7269  .class StatsPeri
-00013990: 6f64 2842 4d29 3a0a 0961 6374 6976 6974  od(BM):..activit
-000139a0: 793a 4f70 7469 6f6e 616c 5b22 5374 6174  y:Optional["Stat
-000139b0: 7341 6374 6976 6974 7922 5d20 3d20 4e6f  sActivity"] = No
-000139c0: 6e65 0a09 7065 7269 6f64 5f66 726f 6d3a  ne..period_from:
-000139d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000139e0: 4e6f 6e65 0a09 7065 7269 6f64 5f74 6f3a  None..period_to:
-000139f0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00013a00: 4e6f 6e65 0a09 7265 6163 683a 4f70 7469  None..reach:Opti
-00013a10: 6f6e 616c 5b22 5374 6174 7352 6561 6368  onal["StatsReach
-00013a20: 225d 203d 204e 6f6e 650a 0976 6973 6974  "] = None..visit
-00013a30: 6f72 733a 4f70 7469 6f6e 616c 5b22 5374  ors:Optional["St
-00013a40: 6174 7356 6965 7773 225d 203d 204e 6f6e  atsViews"] = Non
-00013a50: 650a 0a0a 636c 6173 7320 5374 6174 7352  e...class StatsR
-00013a60: 6561 6368 2842 4d29 3a0a 0961 6765 3a4f  each(BM):..age:O
-00013a70: 7074 696f 6e61 6c5b 6c69 7374 5b22 5374  ptional[list["St
-00013a80: 6174 7353 6578 4167 6522 5d5d 203d 204e  atsSexAge"]] = N
-00013a90: 6f6e 650a 0963 6974 6965 733a 4f70 7469  one..cities:Opti
-00013aa0: 6f6e 616c 5b6c 6973 745b 2253 7461 7473  onal[list["Stats
-00013ab0: 4369 7479 225d 5d20 3d20 4e6f 6e65 0a09  City"]] = None..
-00013ac0: 636f 756e 7472 6965 733a 4f70 7469 6f6e  countries:Option
-00013ad0: 616c 5b6c 6973 745b 2253 7461 7473 436f  al[list["StatsCo
-00013ae0: 756e 7472 7922 5d5d 203d 204e 6f6e 650a  untry"]] = None.
-00013af0: 096d 6f62 696c 655f 7265 6163 683a 4f70  .mobile_reach:Op
-00013b00: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00013b10: 6e65 0a09 7265 6163 683a 4f70 7469 6f6e  ne..reach:Option
-00013b20: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00013b30: 7265 6163 685f 7375 6273 6372 6962 6572  reach_subscriber
-00013b40: 733a 4f70 7469 6f6e 616c 5b69 6e74 5d20  s:Optional[int] 
-00013b50: 3d20 4e6f 6e65 0a09 7365 783a 4f70 7469  = None..sex:Opti
-00013b60: 6f6e 616c 5b6c 6973 745b 2253 7461 7473  onal[list["Stats
-00013b70: 5365 7841 6765 225d 5d20 3d20 4e6f 6e65  SexAge"]] = None
-00013b80: 0a09 7365 785f 6167 653a 4f70 7469 6f6e  ..sex_age:Option
-00013b90: 616c 5b6c 6973 745b 2253 7461 7473 5365  al[list["StatsSe
-00013ba0: 7841 6765 225d 5d20 3d20 4e6f 6e65 0a0a  xAge"]] = None..
-00013bb0: 0a63 6c61 7373 2053 7461 7473 5365 7841  .class StatsSexA
-00013bc0: 6765 2842 4d29 3a0a 0963 6f75 6e74 3a4f  ge(BM):..count:O
-00013bd0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00013be0: 6f6e 650a 0976 616c 7565 3a73 7472 0a09  one..value:str..
-00013bf0: 7265 6163 683a 4f70 7469 6f6e 616c 5b69  reach:Optional[i
-00013c00: 6e74 5d20 3d20 4e6f 6e65 0a09 7265 6163  nt] = None..reac
-00013c10: 685f 7375 6273 6372 6962 6572 733a 4f70  h_subscribers:Op
-00013c20: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00013c30: 6e65 0a09 636f 756e 745f 7375 6273 6372  ne..count_subscr
-00013c40: 6962 6572 733a 4f70 7469 6f6e 616c 5b69  ibers:Optional[i
-00013c50: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  nt] = None...cla
-00013c60: 7373 2053 7461 7473 5669 6577 7328 424d  ss StatsViews(BM
-00013c70: 293a 0a09 6167 653a 4f70 7469 6f6e 616c  ):..age:Optional
-00013c80: 5b6c 6973 745b 2253 7461 7473 5365 7841  [list["StatsSexA
-00013c90: 6765 225d 5d20 3d20 4e6f 6e65 0a09 6369  ge"]] = None..ci
-00013ca0: 7469 6573 3a4f 7074 696f 6e61 6c5b 6c69  ties:Optional[li
-00013cb0: 7374 5b22 5374 6174 7343 6974 7922 5d5d  st["StatsCity"]]
-00013cc0: 203d 204e 6f6e 650a 0963 6f75 6e74 7269   = None..countri
-00013cd0: 6573 3a4f 7074 696f 6e61 6c5b 6c69 7374  es:Optional[list
-00013ce0: 5b22 5374 6174 7343 6f75 6e74 7279 225d  ["StatsCountry"]
-00013cf0: 5d20 3d20 4e6f 6e65 0a09 6d6f 6269 6c65  ] = None..mobile
-00013d00: 5f76 6965 7773 3a4f 7074 696f 6e61 6c5b  _views:Optional[
-00013d10: 696e 745d 203d 204e 6f6e 650a 0973 6578  int] = None..sex
-00013d20: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
-00013d30: 5374 6174 7353 6578 4167 6522 5d5d 203d  StatsSexAge"]] =
-00013d40: 204e 6f6e 650a 0973 6578 5f61 6765 3a4f   None..sex_age:O
-00013d50: 7074 696f 6e61 6c5b 6c69 7374 5b22 5374  ptional[list["St
-00013d60: 6174 7353 6578 4167 6522 5d5d 203d 204e  atsSexAge"]] = N
-00013d70: 6f6e 650a 0976 6965 7773 3a4f 7074 696f  one..views:Optio
-00013d80: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00013d90: 0976 6973 6974 6f72 733a 4f70 7469 6f6e  .visitors:Option
-00013da0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
-00013db0: 0a63 6c61 7373 2053 7461 7473 5761 6c6c  .class StatsWall
-00013dc0: 706f 7374 5374 6174 2842 4d29 3a0a 0970  postStat(BM):..p
-00013dd0: 6f73 745f 6964 3a4f 7074 696f 6e61 6c5b  ost_id:Optional[
-00013de0: 696e 745d 203d 204e 6f6e 650a 0968 6964  int] = None..hid
-00013df0: 653a 4f70 7469 6f6e 616c 5b69 6e74 5d20  e:Optional[int] 
-00013e00: 3d20 4e6f 6e65 0a09 6a6f 696e 5f67 726f  = None..join_gro
-00013e10: 7570 3a4f 7074 696f 6e61 6c5b 696e 745d  up:Optional[int]
-00013e20: 203d 204e 6f6e 650a 096c 696e 6b73 3a4f   = None..links:O
-00013e30: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00013e40: 6f6e 650a 0972 6561 6368 5f73 7562 7363  one..reach_subsc
-00013e50: 7269 6265 7273 3a4f 7074 696f 6e61 6c5b  ribers:Optional[
-00013e60: 696e 745d 203d 204e 6f6e 650a 0972 6561  int] = None..rea
-00013e70: 6368 5f73 7562 7363 7269 6265 7273 5f63  ch_subscribers_c
-00013e80: 6f75 6e74 3a4f 7074 696f 6e61 6c5b 696e  ount:Optional[in
-00013e90: 745d 203d 204e 6f6e 650a 0972 6561 6368  t] = None..reach
-00013ea0: 5f74 6f74 616c 3a4f 7074 696f 6e61 6c5b  _total:Optional[
-00013eb0: 696e 745d 203d 204e 6f6e 650a 0972 6561  int] = None..rea
-00013ec0: 6368 5f74 6f74 616c 5f63 6f75 6e74 3a4f  ch_total_count:O
-00013ed0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00013ee0: 6f6e 650a 0972 6561 6368 5f76 6972 616c  one..reach_viral
-00013ef0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00013f00: 204e 6f6e 650a 0972 6561 6368 5f61 6473   None..reach_ads
-00013f10: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00013f20: 204e 6f6e 650a 0972 6570 6f72 743a 4f70   None..report:Op
-00013f30: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00013f40: 6e65 0a09 746f 5f67 726f 7570 3a4f 7074  ne..to_group:Opt
-00013f50: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00013f60: 650a 0975 6e73 7562 7363 7269 6265 3a4f  e..unsubscribe:O
-00013f70: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00013f80: 6f6e 650a 0973 6578 5f61 6765 3a4f 7074  one..sex_age:Opt
-00013f90: 696f 6e61 6c5b 6c69 7374 5b22 5374 6174  ional[list["Stat
-00013fa0: 7353 6578 4167 6522 5d5d 203d 204e 6f6e  sSexAge"]] = Non
-00013fb0: 650a 0a0a 0a0a 636c 6173 7320 5374 6174  e.....class Stat
-00013fc0: 7573 5374 6174 7573 2842 4d29 3a0a 0974  usStatus(BM):..t
-00013fd0: 6578 743a 7374 720a 0961 7564 696f 3a4f  ext:str..audio:O
-00013fe0: 7074 696f 6e61 6c5b 2241 7564 696f 4175  ptional["AudioAu
-00013ff0: 6469 6f22 5d20 3d20 4e6f 6e65 0a0a 0a0a  dio"] = None....
-00014000: 0a63 6c61 7373 2053 7469 636b 6572 7349  .class StickersI
-00014010: 6d61 6765 5365 7428 424d 293a 0a09 6261  mageSet(BM):..ba
-00014020: 7365 5f75 726c 3a73 7472 0a09 7665 7273  se_url:str..vers
-00014030: 696f 6e3a 4f70 7469 6f6e 616c 5b69 6e74  ion:Optional[int
-00014040: 5d20 3d20 4e6f 6e65 0a0a 0a0a 0a63 6c61  ] = None.....cla
-00014050: 7373 2053 746f 7261 6765 5661 6c75 6528  ss StorageValue(
-00014060: 424d 293a 0a09 6b65 793a 7374 720a 0976  BM):..key:str..v
-00014070: 616c 7565 3a73 7472 0a0a 0a0a 0a63 6c61  alue:str.....cla
-00014080: 7373 2053 746f 7265 5072 6f64 7563 7428  ss StoreProduct(
-00014090: 424d 293a 0a09 6964 3a69 6e74 0a09 7479  BM):..id:int..ty
-000140a0: 7065 3a73 7472 0a09 6973 5f6e 6577 3a4f  pe:str..is_new:O
-000140b0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-000140c0: 4e6f 6e65 0a09 7075 7263 6861 7365 643a  None..purchased:
-000140d0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-000140e0: 204e 6f6e 650a 0961 6374 6976 653a 4f70   None..active:Op
-000140f0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-00014100: 6f6e 650a 0970 726f 6d6f 7465 643a 4f70  one..promoted:Op
-00014110: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-00014120: 6f6e 650a 0970 7572 6368 6173 655f 6461  one..purchase_da
-00014130: 7465 3a4f 7074 696f 6e61 6c5b 696e 745d  te:Optional[int]
-00014140: 203d 204e 6f6e 650a 0974 6974 6c65 3a4f   = None..title:O
-00014150: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00014160: 6f6e 650a 0973 7469 636b 6572 733a 4f70  one..stickers:Op
-00014170: 7469 6f6e 616c 5b22 4261 7365 5374 6963  tional["BaseStic
-00014180: 6b65 7273 4c69 7374 225d 203d 204e 6f6e  kersList"] = Non
-00014190: 650a 0973 7479 6c65 5f73 7469 636b 6572  e..style_sticker
-000141a0: 5f69 6473 3a4f 7074 696f 6e61 6c5b 6c69  _ids:Optional[li
-000141b0: 7374 5b69 6e74 5d5d 203d 204e 6f6e 650a  st[int]] = None.
-000141c0: 0969 636f 6e3a 4f70 7469 6f6e 616c 5b22  .icon:Optional["
-000141d0: 5374 6f72 6550 726f 6475 6374 4963 6f6e  StoreProductIcon
-000141e0: 225d 203d 204e 6f6e 650a 0970 7265 7669  "] = None..previ
-000141f0: 6577 733a 4f70 7469 6f6e 616c 5b6c 6973  ews:Optional[lis
-00014200: 745b 2242 6173 6549 6d61 6765 225d 5d20  t["BaseImage"]] 
-00014210: 3d20 4e6f 6e65 0a09 6861 735f 616e 696d  = None..has_anim
-00014220: 6174 696f 6e3a 4f70 7469 6f6e 616c 5b62  ation:Optional[b
-00014230: 6f6f 6c5d 203d 204e 6f6e 650a 0973 7562  ool] = None..sub
-00014240: 7469 746c 653a 4f70 7469 6f6e 616c 5b73  title:Optional[s
-00014250: 7472 5d20 3d20 4e6f 6e65 0a09 7061 796d  tr] = None..paym
-00014260: 656e 745f 7265 6769 6f6e 3a4f 7074 696f  ent_region:Optio
-00014270: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00014280: 0a0a 636c 6173 7320 5374 6f72 6550 726f  ..class StorePro
-00014290: 6475 6374 4963 6f6e 2842 4d29 3a0a 0970  ductIcon(BM):..p
-000142a0: 6173 730a 0a63 6c61 7373 2053 746f 7265  ass..class Store
-000142b0: 5374 6963 6b65 7273 4b65 7977 6f72 6428  StickersKeyword(
-000142c0: 424d 293a 0a09 776f 7264 733a 6c69 7374  BM):..words:list
-000142d0: 5b73 7472 5d0a 0975 7365 725f 7374 6963  [str]..user_stic
-000142e0: 6b65 7273 3a4f 7074 696f 6e61 6c5b 2253  kers:Optional["S
-000142f0: 746f 7265 5374 6963 6b65 7273 4b65 7977  toreStickersKeyw
-00014300: 6f72 6453 7469 636b 6572 7322 5d20 3d20  ordStickers"] = 
-00014310: 4e6f 6e65 0a09 7072 6f6d 6f74 6564 5f73  None..promoted_s
-00014320: 7469 636b 6572 733a 4f70 7469 6f6e 616c  tickers:Optional
-00014330: 5b22 5374 6f72 6553 7469 636b 6572 734b  ["StoreStickersK
-00014340: 6579 776f 7264 5374 6963 6b65 7273 225d  eywordStickers"]
-00014350: 203d 204e 6f6e 650a 0973 7469 636b 6572   = None..sticker
-00014360: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-00014370: 2253 746f 7265 5374 6963 6b65 7273 4b65  "StoreStickersKe
-00014380: 7977 6f72 6453 7469 636b 6572 225d 5d20  ywordSticker"]] 
-00014390: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2053  = None...class S
-000143a0: 746f 7265 5374 6963 6b65 7273 4b65 7977  toreStickersKeyw
-000143b0: 6f72 6453 7469 636b 6572 2842 4d29 3a0a  ordSticker(BM):.
-000143c0: 0970 6163 6b5f 6964 3a69 6e74 0a09 7374  .pack_id:int..st
-000143d0: 6963 6b65 725f 6964 3a69 6e74 0a0a 0a63  icker_id:int...c
-000143e0: 6c61 7373 2053 746f 7265 5374 6963 6b65  lass StoreSticke
-000143f0: 7273 4b65 7977 6f72 6453 7469 636b 6572  rsKeywordSticker
-00014400: 7328 424d 293a 0a09 7061 7373 0a0a 0a0a  s(BM):..pass....
-00014410: 636c 6173 7320 5374 6f72 6965 7353 746f  class StoriesSto
-00014420: 7279 5374 6174 7353 7461 7465 2845 6e75  ryStatsState(Enu
-00014430: 6d29 3a0a 094f 4e20 3d20 226f 6e22 0a09  m):..ON = "on"..
-00014440: 4f46 4620 3d20 226f 6666 220a 0948 4944  OFF = "off"..HID
-00014450: 4445 4e20 3d20 2268 6964 6465 6e22 0a0a  DEN = "hidden"..
-00014460: 636c 6173 7320 5374 6f72 6965 7353 746f  class StoriesSto
-00014470: 7279 5479 7065 2845 6e75 6d29 3a0a 0950  ryType(Enum):..P
-00014480: 484f 544f 203d 2022 7068 6f74 6f22 0a09  HOTO = "photo"..
-00014490: 5649 4445 4f20 3d20 2276 6964 656f 220a  VIDEO = "video".
-000144a0: 094c 4956 455f 4143 5449 5645 203d 2022  .LIVE_ACTIVE = "
-000144b0: 6c69 7665 5f61 6374 6976 6522 0a09 4c49  live_active"..LI
-000144c0: 5645 5f46 494e 4953 4845 4420 3d20 226c  VE_FINISHED = "l
-000144d0: 6976 655f 6669 6e69 7368 6564 220a 0942  ive_finished"..B
-000144e0: 4952 5448 4441 595f 494e 5649 5445 203d  IRTHDAY_INVITE =
-000144f0: 2022 6269 7274 6864 6179 5f69 6e76 6974   "birthday_invit
-00014500: 6522 0a0a 636c 6173 7320 5374 6f72 6965  e"..class Storie
-00014510: 7355 706c 6f61 644c 696e 6b54 6578 7428  sUploadLinkText(
-00014520: 456e 756d 293a 0a09 544f 5f53 544f 5245  Enum):..TO_STORE
-00014530: 203d 2022 746f 5f73 746f 7265 220a 0956   = "to_store"..V
-00014540: 4f54 4520 3d20 2276 6f74 6522 0a09 4d4f  OTE = "vote"..MO
-00014550: 5245 203d 2022 6d6f 7265 220a 0942 4f4f  RE = "more"..BOO
-00014560: 4b20 3d20 2262 6f6f 6b22 0a09 4f52 4445  K = "book"..ORDE
-00014570: 5220 3d20 226f 7264 6572 220a 0945 4e52  R = "order"..ENR
-00014580: 4f4c 4c20 3d20 2265 6e72 6f6c 6c22 0a09  OLL = "enroll"..
-00014590: 4649 4c4c 203d 2022 6669 6c6c 220a 0953  FILL = "fill"..S
-000145a0: 4947 4e55 5020 3d20 2273 6967 6e75 7022  IGNUP = "signup"
-000145b0: 0a09 4255 5920 3d20 2262 7579 220a 0954  ..BUY = "buy"..T
-000145c0: 4943 4b45 5420 3d20 2274 6963 6b65 7422  ICKET = "ticket"
-000145d0: 0a09 5752 4954 4520 3d20 2277 7269 7465  ..WRITE = "write
-000145e0: 220a 094f 5045 4e20 3d20 226f 7065 6e22  "..OPEN = "open"
-000145f0: 0a09 4c45 4152 4e5f 4d4f 5245 203d 2022  ..LEARN_MORE = "
-00014600: 6c65 6172 6e5f 6d6f 7265 220a 0956 4945  learn_more"..VIE
-00014610: 5720 3d20 2276 6965 7722 0a09 474f 5f54  W = "view"..GO_T
-00014620: 4f20 3d20 2267 6f5f 746f 220a 0943 4f4e  O = "go_to"..CON
-00014630: 5441 4354 203d 2022 636f 6e74 6163 7422  TACT = "contact"
-00014640: 0a09 5741 5443 4820 3d20 2277 6174 6368  ..WATCH = "watch
-00014650: 220a 0950 4c41 5920 3d20 2270 6c61 7922  "..PLAY = "play"
-00014660: 0a09 494e 5354 414c 4c20 3d20 2269 6e73  ..INSTALL = "ins
-00014670: 7461 6c6c 220a 0952 4541 4420 3d20 2272  tall"..READ = "r
-00014680: 6561 6422 0a09 4341 4c45 4e44 4152 203d  ead"..CALENDAR =
-00014690: 2022 6361 6c65 6e64 6172 220a 0a63 6c61   "calendar"..cla
-000146a0: 7373 2053 746f 7269 6573 436c 6963 6b61  ss StoriesClicka
-000146b0: 626c 6541 7265 6128 424d 293a 0a09 783a  bleArea(BM):..x:
-000146c0: 696e 740a 0979 3a69 6e74 0a0a 0a63 6c61  int..y:int...cla
-000146d0: 7373 2053 746f 7269 6573 436c 6963 6b61  ss StoriesClicka
-000146e0: 626c 6553 7469 636b 6572 2842 4d29 3a0a  bleSticker(BM):.
-000146f0: 0963 6c69 636b 6162 6c65 5f61 7265 613a  .clickable_area:
-00014700: 6c69 7374 5b22 5374 6f72 6965 7343 6c69  list["StoriesCli
-00014710: 636b 6162 6c65 4172 6561 225d 0a09 6964  ckableArea"]..id
-00014720: 3a69 6e74 0a09 6861 7368 7461 673a 4f70  :int..hashtag:Op
-00014730: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00014740: 6e65 0a09 6c69 6e6b 5f6f 626a 6563 743a  ne..link_object:
-00014750: 4f70 7469 6f6e 616c 5b22 4261 7365 4c69  Optional["BaseLi
-00014760: 6e6b 225d 203d 204e 6f6e 650a 096d 656e  nk"] = None..men
-00014770: 7469 6f6e 3a4f 7074 696f 6e61 6c5b 7374  tion:Optional[st
-00014780: 725d 203d 204e 6f6e 650a 0974 6f6f 6c74  r] = None..toolt
-00014790: 6970 5f74 6578 743a 4f70 7469 6f6e 616c  ip_text:Optional
-000147a0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6f77  [str] = None..ow
-000147b0: 6e65 725f 6964 3a4f 7074 696f 6e61 6c5b  ner_id:Optional[
-000147c0: 696e 745d 203d 204e 6f6e 650a 0973 746f  int] = None..sto
-000147d0: 7279 5f69 643a 4f70 7469 6f6e 616c 5b69  ry_id:Optional[i
-000147e0: 6e74 5d20 3d20 4e6f 6e65 0a09 7175 6573  nt] = None..ques
-000147f0: 7469 6f6e 3a4f 7074 696f 6e61 6c5b 7374  tion:Optional[st
-00014800: 725d 203d 204e 6f6e 650a 0971 7565 7374  r] = None..quest
-00014810: 696f 6e5f 6275 7474 6f6e 3a4f 7074 696f  ion_button:Optio
-00014820: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00014830: 0970 6c61 6365 5f69 643a 4f70 7469 6f6e  .place_id:Option
-00014840: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00014850: 6d61 726b 6574 5f69 7465 6d3a 4f70 7469  market_item:Opti
-00014860: 6f6e 616c 5b22 4d61 726b 6574 4d61 726b  onal["MarketMark
-00014870: 6574 4974 656d 225d 203d 204e 6f6e 650a  etItem"] = None.
-00014880: 0961 7564 696f 3a4f 7074 696f 6e61 6c5b  .audio:Optional[
-00014890: 2241 7564 696f 4175 6469 6f22 5d20 3d20  "AudioAudio"] = 
-000148a0: 4e6f 6e65 0a09 6175 6469 6f5f 7374 6172  None..audio_star
-000148b0: 745f 7469 6d65 3a4f 7074 696f 6e61 6c5b  t_time:Optional[
-000148c0: 696e 745d 203d 204e 6f6e 650a 0973 7479  int] = None..sty
-000148d0: 6c65 3a4f 7074 696f 6e61 6c5b 7374 725d  le:Optional[str]
-000148e0: 203d 204e 6f6e 650a 0974 7970 653a 7374   = None..type:st
-000148f0: 720a 0973 7562 7479 7065 3a4f 7074 696f  r..subtype:Optio
-00014900: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00014910: 0970 6f73 745f 6f77 6e65 725f 6964 3a4f  .post_owner_id:O
-00014920: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00014930: 6f6e 650a 0970 6f73 745f 6964 3a4f 7074  one..post_id:Opt
-00014940: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00014950: 650a 0970 6f6c 6c3a 4f70 7469 6f6e 616c  e..poll:Optional
-00014960: 5b22 506f 6c6c 7350 6f6c 6c22 5d20 3d20  ["PollsPoll"] = 
-00014970: 4e6f 6e65 0a09 636f 6c6f 723a 4f70 7469  None..color:Opti
-00014980: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00014990: 0a09 7374 6963 6b65 725f 6964 3a4f 7074  ..sticker_id:Opt
-000149a0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-000149b0: 650a 0973 7469 636b 6572 5f70 6163 6b5f  e..sticker_pack_
-000149c0: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-000149d0: 203d 204e 6f6e 650a 0961 7070 3a4f 7074   = None..app:Opt
-000149e0: 696f 6e61 6c5b 2241 7070 7341 7070 4d69  ional["AppsAppMi
-000149f0: 6e22 5d20 3d20 4e6f 6e65 0a09 6170 705f  n"] = None..app_
-00014a00: 636f 6e74 6578 743a 4f70 7469 6f6e 616c  context:Optional
-00014a10: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6861  [str] = None..ha
-00014a20: 735f 6e65 775f 696e 7465 7261 6374 696f  s_new_interactio
-00014a30: 6e73 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ns:Optional[bool
-00014a40: 5d20 3d20 4e6f 6e65 0a09 6973 5f62 726f  ] = None..is_bro
-00014a50: 6164 6361 7374 5f6e 6f74 6966 795f 616c  adcast_notify_al
-00014a60: 6c6f 7765 643a 4f70 7469 6f6e 616c 5b62  lowed:Optional[b
-00014a70: 6f6f 6c5d 203d 204e 6f6e 650a 0973 6974  ool] = None..sit
-00014a80: 7561 7469 6f6e 616c 5f74 6865 6d65 5f69  uational_theme_i
-00014a90: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-00014aa0: 3d20 4e6f 6e65 0a09 7369 7475 6174 696f  = None..situatio
-00014ab0: 6e61 6c5f 6170 705f 7572 6c3a 4f70 7469  nal_app_url:Opti
-00014ac0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00014ad0: 0a0a 0a63 6c61 7373 2053 746f 7269 6573  ...class Stories
-00014ae0: 436c 6963 6b61 626c 6553 7469 636b 6572  ClickableSticker
-00014af0: 7328 424d 293a 0a09 636c 6963 6b61 626c  s(BM):..clickabl
-00014b00: 655f 7374 6963 6b65 7273 3a6c 6973 745b  e_stickers:list[
-00014b10: 2253 746f 7269 6573 436c 6963 6b61 626c  "StoriesClickabl
-00014b20: 6553 7469 636b 6572 225d 0a09 6f72 6967  eSticker"]..orig
-00014b30: 696e 616c 5f68 6569 6768 743a 696e 740a  inal_height:int.
-00014b40: 096f 7269 6769 6e61 6c5f 7769 6474 683a  .original_width:
-00014b50: 696e 740a 0a0a 636c 6173 7320 5374 6f72  int...class Stor
-00014b60: 6965 7346 6565 6449 7465 6d28 424d 293a  iesFeedItem(BM):
-00014b70: 0a09 7479 7065 3a73 7472 0a09 6964 3a4f  ..type:str..id:O
-00014b80: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00014b90: 6f6e 650a 0973 746f 7269 6573 3a4f 7074  one..stories:Opt
-00014ba0: 696f 6e61 6c5b 6c69 7374 5b22 5374 6f72  ional[list["Stor
-00014bb0: 6965 7353 746f 7279 225d 5d20 3d20 4e6f  iesStory"]] = No
-00014bc0: 6e65 0a09 6772 6f75 7065 643a 4f70 7469  ne..grouped:Opti
-00014bd0: 6f6e 616c 5b6c 6973 745b 2253 746f 7269  onal[list["Stori
-00014be0: 6573 4665 6564 4974 656d 225d 5d20 3d20  esFeedItem"]] = 
-00014bf0: 4e6f 6e65 0a09 6170 703a 4f70 7469 6f6e  None..app:Option
-00014c00: 616c 5b22 4170 7073 4170 704d 696e 225d  al["AppsAppMin"]
-00014c10: 203d 204e 6f6e 650a 0970 726f 6d6f 5f64   = None..promo_d
-00014c20: 6174 613a 4f70 7469 6f6e 616c 5b22 5374  ata:Optional["St
-00014c30: 6f72 6965 7350 726f 6d6f 426c 6f63 6b22  oriesPromoBlock"
-00014c40: 5d20 3d20 4e6f 6e65 0a09 6269 7274 6864  ] = None..birthd
-00014c50: 6179 5f75 7365 725f 6964 3a4f 7074 696f  ay_user_id:Optio
-00014c60: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00014c70: 0974 7261 636b 5f63 6f64 653a 4f70 7469  .track_code:Opti
-00014c80: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00014c90: 0a09 6861 735f 756e 7365 656e 3a4f 7074  ..has_unseen:Opt
-00014ca0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00014cb0: 6e65 0a09 6e61 6d65 3a4f 7074 696f 6e61  ne..name:Optiona
-00014cc0: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
-00014cd0: 636c 6173 7320 5374 6f72 6965 7350 726f  class StoriesPro
-00014ce0: 6d6f 426c 6f63 6b28 424d 293a 0a09 6e61  moBlock(BM):..na
-00014cf0: 6d65 3a73 7472 0a09 7068 6f74 6f5f 3530  me:str..photo_50
-00014d00: 3a73 7472 0a09 7068 6f74 6f5f 3130 303a  :str..photo_100:
-00014d10: 7374 720a 096e 6f74 5f61 6e69 6d61 7465  str..not_animate
-00014d20: 643a 626f 6f6c 0a0a 0a63 6c61 7373 2053  d:bool...class S
-00014d30: 746f 7269 6573 5265 706c 6965 7328 424d  toriesReplies(BM
-00014d40: 293a 0a09 636f 756e 743a 696e 740a 096e  ):..count:int..n
-00014d50: 6577 3a4f 7074 696f 6e61 6c5b 696e 745d  ew:Optional[int]
-00014d60: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
-00014d70: 5374 6f72 6965 7353 7461 744c 696e 6528  StoriesStatLine(
-00014d80: 424d 293a 0a09 6e61 6d65 3a73 7472 0a09  BM):..name:str..
-00014d90: 636f 756e 7465 723a 4f70 7469 6f6e 616c  counter:Optional
-00014da0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6973  [int] = None..is
-00014db0: 5f75 6e61 7661 696c 6162 6c65 3a4f 7074  _unavailable:Opt
-00014dc0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00014dd0: 6e65 0a0a 0a63 6c61 7373 2053 746f 7269  ne...class Stori
-00014de0: 6573 5374 6f72 7928 424d 293a 0a09 6163  esStory(BM):..ac
-00014df0: 6365 7373 5f6b 6579 3a4f 7074 696f 6e61  cess_key:Optiona
-00014e00: 6c5b 7374 725d 203d 204e 6f6e 650a 0963  l[str] = None..c
-00014e10: 616e 5f63 6f6d 6d65 6e74 3a4f 7074 696f  an_comment:Optio
-00014e20: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00014e30: 0a09 6361 6e5f 7265 706c 793a 4f70 7469  ..can_reply:Opti
-00014e40: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00014e50: 650a 0963 616e 5f73 6565 3a4f 7074 696f  e..can_see:Optio
-00014e60: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00014e70: 0a09 6361 6e5f 6c69 6b65 3a4f 7074 696f  ..can_like:Optio
-00014e80: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00014e90: 0a09 6361 6e5f 7368 6172 653a 4f70 7469  ..can_share:Opti
-00014ea0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00014eb0: 650a 0963 616e 5f68 6964 653a 4f70 7469  e..can_hide:Opti
-00014ec0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00014ed0: 650a 0964 6174 653a 4f70 7469 6f6e 616c  e..date:Optional
-00014ee0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6578  [int] = None..ex
-00014ef0: 7069 7265 735f 6174 3a4f 7074 696f 6e61  pires_at:Optiona
-00014f00: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
-00014f10: 643a 696e 740a 0969 735f 6465 6c65 7465  d:int..is_delete
-00014f20: 643a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  d:Optional[bool]
-00014f30: 203d 204e 6f6e 650a 0969 735f 6578 7069   = None..is_expi
-00014f40: 7265 643a 4f70 7469 6f6e 616c 5b62 6f6f  red:Optional[boo
-00014f50: 6c5d 203d 204e 6f6e 650a 096c 696e 6b3a  l] = None..link:
-00014f60: 4f70 7469 6f6e 616c 5b22 5374 6f72 6965  Optional["Storie
-00014f70: 7353 746f 7279 4c69 6e6b 225d 203d 204e  sStoryLink"] = N
-00014f80: 6f6e 650a 096f 776e 6572 5f69 643a 696e  one..owner_id:in
-00014f90: 740a 0970 6172 656e 745f 7374 6f72 793a  t..parent_story:
-00014fa0: 4f70 7469 6f6e 616c 5b22 5374 6f72 6965  Optional["Storie
-00014fb0: 7353 746f 7279 225d 203d 204e 6f6e 650a  sStory"] = None.
-00014fc0: 0970 6172 656e 745f 7374 6f72 795f 6163  .parent_story_ac
-00014fd0: 6365 7373 5f6b 6579 3a4f 7074 696f 6e61  cess_key:Optiona
-00014fe0: 6c5b 7374 725d 203d 204e 6f6e 650a 0970  l[str] = None..p
-00014ff0: 6172 656e 745f 7374 6f72 795f 6964 3a4f  arent_story_id:O
-00015000: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00015010: 6f6e 650a 0970 6172 656e 745f 7374 6f72  one..parent_stor
-00015020: 795f 6f77 6e65 725f 6964 3a4f 7074 696f  y_owner_id:Optio
-00015030: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00015040: 0970 686f 746f 3a4f 7074 696f 6e61 6c5b  .photo:Optional[
-00015050: 2250 686f 746f 7350 686f 746f 225d 203d  "PhotosPhoto"] =
-00015060: 204e 6f6e 650a 0972 6570 6c69 6573 3a4f   None..replies:O
-00015070: 7074 696f 6e61 6c5b 2253 746f 7269 6573  ptional["Stories
-00015080: 5265 706c 6965 7322 5d20 3d20 4e6f 6e65  Replies"] = None
-00015090: 0a09 7365 656e 3a4f 7074 696f 6e61 6c5b  ..seen:Optional[
-000150a0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 7479  bool] = None..ty
-000150b0: 7065 3a4f 7074 696f 6e61 6c5b 2253 746f  pe:Optional["Sto
-000150c0: 7269 6573 5374 6f72 7954 7970 6522 5d20  riesStoryType"] 
-000150d0: 3d20 4e6f 6e65 0a09 636c 6963 6b61 626c  = None..clickabl
-000150e0: 655f 7374 6963 6b65 7273 3a4f 7074 696f  e_stickers:Optio
-000150f0: 6e61 6c5b 2253 746f 7269 6573 436c 6963  nal["StoriesClic
-00015100: 6b61 626c 6553 7469 636b 6572 7322 5d20  kableStickers"] 
-00015110: 3d20 4e6f 6e65 0a09 7669 6465 6f3a 4f70  = None..video:Op
-00015120: 7469 6f6e 616c 5b22 5669 6465 6f56 6964  tional["VideoVid
-00015130: 656f 4675 6c6c 225d 203d 204e 6f6e 650a  eoFull"] = None.
-00015140: 0976 6965 7773 3a4f 7074 696f 6e61 6c5b  .views:Optional[
-00015150: 696e 745d 203d 204e 6f6e 650a 0963 616e  int] = None..can
-00015160: 5f61 736b 3a4f 7074 696f 6e61 6c5b 626f  _ask:Optional[bo
-00015170: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
-00015180: 6173 6b5f 616e 6f6e 796d 6f75 733a 4f70  ask_anonymous:Op
-00015190: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-000151a0: 6f6e 650a 096e 6172 7261 7469 7665 735f  one..narratives_
-000151b0: 636f 756e 743a 4f70 7469 6f6e 616c 5b69  count:Optional[i
-000151c0: 6e74 5d20 3d20 4e6f 6e65 0a09 6669 7273  nt] = None..firs
-000151d0: 745f 6e61 7272 6174 6976 655f 7469 746c  t_narrative_titl
-000151e0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-000151f0: 3d20 4e6f 6e65 0a09 6269 7274 6864 6179  = None..birthday
-00015200: 5f77 6973 685f 7573 6572 5f69 643a 4f70  _wish_user_id:Op
-00015210: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00015220: 6e65 0a09 6361 6e5f 7573 655f 696e 5f6e  ne..can_use_in_n
-00015230: 6172 7261 7469 7665 3a4f 7074 696f 6e61  arrative:Optiona
-00015240: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a  l[bool] = None..
-00015250: 0a63 6c61 7373 2053 746f 7269 6573 5374  .class StoriesSt
-00015260: 6f72 794c 696e 6b28 424d 293a 0a09 7465  oryLink(BM):..te
-00015270: 7874 3a73 7472 0a09 7572 6c3a 7374 720a  xt:str..url:str.
-00015280: 096c 696e 6b5f 7572 6c5f 7461 7267 6574  .link_url_target
-00015290: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-000152a0: 204e 6f6e 650a 0a0a 636c 6173 7320 5374   None...class St
-000152b0: 6f72 6965 7353 746f 7279 5374 6174 7328  oriesStoryStats(
-000152c0: 424d 293a 0a09 616e 7377 6572 3a22 5374  BM):..answer:"St
-000152d0: 6f72 6965 7353 746f 7279 5374 6174 7353  oriesStoryStatsS
-000152e0: 7461 7422 0a09 6261 6e73 3a22 5374 6f72  tat"..bans:"Stor
-000152f0: 6965 7353 746f 7279 5374 6174 7353 7461  iesStoryStatsSta
-00015300: 7422 0a09 6f70 656e 5f6c 696e 6b3a 2253  t"..open_link:"S
-00015310: 746f 7269 6573 5374 6f72 7953 7461 7473  toriesStoryStats
-00015320: 5374 6174 220a 0972 6570 6c69 6573 3a22  Stat"..replies:"
-00015330: 5374 6f72 6965 7353 746f 7279 5374 6174  StoriesStoryStat
-00015340: 7353 7461 7422 0a09 7368 6172 6573 3a22  sStat"..shares:"
-00015350: 5374 6f72 6965 7353 746f 7279 5374 6174  StoriesStoryStat
-00015360: 7353 7461 7422 0a09 7375 6273 6372 6962  sStat"..subscrib
-00015370: 6572 733a 2253 746f 7269 6573 5374 6f72  ers:"StoriesStor
-00015380: 7953 7461 7473 5374 6174 220a 0976 6965  yStatsStat"..vie
-00015390: 7773 3a22 5374 6f72 6965 7353 746f 7279  ws:"StoriesStory
-000153a0: 5374 6174 7353 7461 7422 0a09 6c69 6b65  StatsStat"..like
-000153b0: 733a 2253 746f 7269 6573 5374 6f72 7953  s:"StoriesStoryS
-000153c0: 7461 7473 5374 6174 220a 0a0a 636c 6173  tatsStat"...clas
-000153d0: 7320 5374 6f72 6965 7353 746f 7279 5374  s StoriesStorySt
-000153e0: 6174 7353 7461 7428 424d 293a 0a09 636f  atsStat(BM):..co
-000153f0: 756e 743a 4f70 7469 6f6e 616c 5b69 6e74  unt:Optional[int
-00015400: 5d20 3d20 4e6f 6e65 0a09 7374 6174 653a  ] = None..state:
-00015410: 2253 746f 7269 6573 5374 6f72 7953 7461  "StoriesStorySta
-00015420: 7473 5374 6174 6522 0a0a 0a63 6c61 7373  tsState"...class
-00015430: 2053 746f 7269 6573 5669 6577 6572 7349   StoriesViewersI
-00015440: 7465 6d28 424d 293a 0a09 6973 5f6c 696b  tem(BM):..is_lik
-00015450: 6564 3a62 6f6f 6c0a 0975 7365 725f 6964  ed:bool..user_id
-00015460: 3a69 6e74 0a09 7573 6572 3a4f 7074 696f  :int..user:Optio
-00015470: 6e61 6c5b 2255 7365 7273 5573 6572 4675  nal["UsersUserFu
-00015480: 6c6c 225d 203d 204e 6f6e 650a 0a0a 0a0a  ll"] = None.....
-00015490: 636c 6173 7320 5573 6572 7346 6965 6c64  class UsersField
-000154a0: 7328 456e 756d 293a 0a09 4649 5253 545f  s(Enum):..FIRST_
-000154b0: 4e41 4d45 5f4e 4f4d 203d 2022 6669 7273  NAME_NOM = "firs
-000154c0: 745f 6e61 6d65 5f6e 6f6d 220a 0946 4952  t_name_nom"..FIR
-000154d0: 5354 5f4e 414d 455f 4745 4e20 3d20 2266  ST_NAME_GEN = "f
-000154e0: 6972 7374 5f6e 616d 655f 6765 6e22 0a09  irst_name_gen"..
-000154f0: 4649 5253 545f 4e41 4d45 5f44 4154 203d  FIRST_NAME_DAT =
-00015500: 2022 6669 7273 745f 6e61 6d65 5f64 6174   "first_name_dat
-00015510: 220a 0946 4952 5354 5f4e 414d 455f 4143  "..FIRST_NAME_AC
-00015520: 4320 3d20 2266 6972 7374 5f6e 616d 655f  C = "first_name_
-00015530: 6163 6322 0a09 4649 5253 545f 4e41 4d45  acc"..FIRST_NAME
-00015540: 5f49 4e53 203d 2022 6669 7273 745f 6e61  _INS = "first_na
-00015550: 6d65 5f69 6e73 220a 0946 4952 5354 5f4e  me_ins"..FIRST_N
-00015560: 414d 455f 4142 4c20 3d20 2266 6972 7374  AME_ABL = "first
-00015570: 5f6e 616d 655f 6162 6c22 0a09 4c41 5354  _name_abl"..LAST
-00015580: 5f4e 414d 455f 4e4f 4d20 3d20 226c 6173  _NAME_NOM = "las
-00015590: 745f 6e61 6d65 5f6e 6f6d 220a 094c 4153  t_name_nom"..LAS
-000155a0: 545f 4e41 4d45 5f47 454e 203d 2022 6c61  T_NAME_GEN = "la
-000155b0: 7374 5f6e 616d 655f 6765 6e22 0a09 4c41  st_name_gen"..LA
-000155c0: 5354 5f4e 414d 455f 4441 5420 3d20 226c  ST_NAME_DAT = "l
-000155d0: 6173 745f 6e61 6d65 5f64 6174 220a 094c  ast_name_dat"..L
-000155e0: 4153 545f 4e41 4d45 5f41 4343 203d 2022  AST_NAME_ACC = "
-000155f0: 6c61 7374 5f6e 616d 655f 6163 6322 0a09  last_name_acc"..
-00015600: 4c41 5354 5f4e 414d 455f 494e 5320 3d20  LAST_NAME_INS = 
-00015610: 226c 6173 745f 6e61 6d65 5f69 6e73 220a  "last_name_ins".
-00015620: 094c 4153 545f 4e41 4d45 5f41 424c 203d  .LAST_NAME_ABL =
-00015630: 2022 6c61 7374 5f6e 616d 655f 6162 6c22   "last_name_abl"
-00015640: 0a09 5048 4f54 4f5f 4944 203d 2022 7068  ..PHOTO_ID = "ph
-00015650: 6f74 6f5f 6964 220a 0956 4552 4946 4945  oto_id"..VERIFIE
-00015660: 4420 3d20 2276 6572 6966 6965 6422 0a09  D = "verified"..
-00015670: 5345 5820 3d20 2273 6578 220a 0942 4441  SEX = "sex"..BDA
-00015680: 5445 203d 2022 6264 6174 6522 0a09 4244  TE = "bdate"..BD
-00015690: 4154 455f 5649 5349 4249 4c49 5459 203d  ATE_VISIBILITY =
-000156a0: 2022 6264 6174 655f 7669 7369 6269 6c69   "bdate_visibili
-000156b0: 7479 220a 0943 4954 5920 3d20 2263 6974  ty"..CITY = "cit
-000156c0: 7922 0a09 434f 554e 5452 5920 3d20 2263  y"..COUNTRY = "c
-000156d0: 6f75 6e74 7279 220a 0948 4f4d 455f 544f  ountry"..HOME_TO
-000156e0: 574e 203d 2022 686f 6d65 5f74 6f77 6e22  WN = "home_town"
-000156f0: 0a09 4841 535f 5048 4f54 4f20 3d20 2268  ..HAS_PHOTO = "h
-00015700: 6173 5f70 686f 746f 220a 0950 484f 544f  as_photo"..PHOTO
-00015710: 203d 2022 7068 6f74 6f22 0a09 5048 4f54   = "photo"..PHOT
-00015720: 4f5f 5245 4320 3d20 2270 686f 746f 5f72  O_REC = "photo_r
-00015730: 6563 220a 0950 484f 544f 5f35 3020 3d20  ec"..PHOTO_50 = 
-00015740: 2270 686f 746f 5f35 3022 0a09 5048 4f54  "photo_50"..PHOT
-00015750: 4f5f 3130 3020 3d20 2270 686f 746f 5f31  O_100 = "photo_1
-00015760: 3030 220a 0950 484f 544f 5f32 3030 5f4f  00"..PHOTO_200_O
-00015770: 5249 4720 3d20 2270 686f 746f 5f32 3030  RIG = "photo_200
-00015780: 5f6f 7269 6722 0a09 5048 4f54 4f5f 3230  _orig"..PHOTO_20
-00015790: 3020 3d20 2270 686f 746f 5f32 3030 220a  0 = "photo_200".
-000157a0: 0950 484f 544f 5f34 3030 203d 2022 7068  .PHOTO_400 = "ph
-000157b0: 6f74 6f5f 3430 3022 0a09 5048 4f54 4f5f  oto_400"..PHOTO_
-000157c0: 3430 305f 4f52 4947 203d 2022 7068 6f74  400_ORIG = "phot
-000157d0: 6f5f 3430 305f 6f72 6967 220a 0950 484f  o_400_orig"..PHO
-000157e0: 544f 5f42 4947 203d 2022 7068 6f74 6f5f  TO_BIG = "photo_
-000157f0: 6269 6722 0a09 5048 4f54 4f5f 4d45 4449  big"..PHOTO_MEDI
-00015800: 554d 203d 2022 7068 6f74 6f5f 6d65 6469  UM = "photo_medi
-00015810: 756d 220a 0950 484f 544f 5f4d 4544 4955  um"..PHOTO_MEDIU
-00015820: 4d5f 5245 4320 3d20 2270 686f 746f 5f6d  M_REC = "photo_m
-00015830: 6564 6975 6d5f 7265 6322 0a09 5048 4f54  edium_rec"..PHOT
-00015840: 4f5f 4d41 5820 3d20 2270 686f 746f 5f6d  O_MAX = "photo_m
-00015850: 6178 220a 0950 484f 544f 5f4d 4158 5f4f  ax"..PHOTO_MAX_O
-00015860: 5249 4720 3d20 2270 686f 746f 5f6d 6178  RIG = "photo_max
-00015870: 5f6f 7269 6722 0a09 5048 4f54 4f5f 4d41  _orig"..PHOTO_MA
-00015880: 585f 5349 5a45 203d 2022 7068 6f74 6f5f  X_SIZE = "photo_
-00015890: 6d61 785f 7369 7a65 220a 0954 4849 5244  max_size"..THIRD
-000158a0: 5f50 4152 5459 5f42 5554 544f 4e53 203d  _PARTY_BUTTONS =
-000158b0: 2022 7468 6972 645f 7061 7274 795f 6275   "third_party_bu
-000158c0: 7474 6f6e 7322 0a09 4f4e 4c49 4e45 203d  ttons"..ONLINE =
-000158d0: 2022 6f6e 6c69 6e65 220a 094c 4953 5453   "online"..LISTS
-000158e0: 203d 2022 6c69 7374 7322 0a09 444f 4d41   = "lists"..DOMA
-000158f0: 494e 203d 2022 646f 6d61 696e 220a 0948  IN = "domain"..H
-00015900: 4153 5f4d 4f42 494c 4520 3d20 2268 6173  AS_MOBILE = "has
-00015910: 5f6d 6f62 696c 6522 0a09 434f 4e54 4143  _mobile"..CONTAC
-00015920: 5453 203d 2022 636f 6e74 6163 7473 220a  TS = "contacts".
-00015930: 094c 414e 4755 4147 4520 3d20 226c 616e  .LANGUAGE = "lan
-00015940: 6775 6167 6522 0a09 5349 5445 203d 2022  guage"..SITE = "
-00015950: 7369 7465 220a 0945 4455 4341 5449 4f4e  site"..EDUCATION
-00015960: 203d 2022 6564 7563 6174 696f 6e22 0a09   = "education"..
-00015970: 554e 4956 4552 5349 5449 4553 203d 2022  UNIVERSITIES = "
-00015980: 756e 6976 6572 7369 7469 6573 220a 0953  universities"..S
-00015990: 4348 4f4f 4c53 203d 2022 7363 686f 6f6c  CHOOLS = "school
-000159a0: 7322 0a09 5354 4154 5553 203d 2022 7374  s"..STATUS = "st
-000159b0: 6174 7573 220a 094c 4153 545f 5345 454e  atus"..LAST_SEEN
-000159c0: 203d 2022 6c61 7374 5f73 6565 6e22 0a09   = "last_seen"..
-000159d0: 464f 4c4c 4f57 4552 535f 434f 554e 5420  FOLLOWERS_COUNT 
-000159e0: 3d20 2266 6f6c 6c6f 7765 7273 5f63 6f75  = "followers_cou
-000159f0: 6e74 220a 0943 4f55 4e54 4552 5320 3d20  nt"..COUNTERS = 
-00015a00: 2263 6f75 6e74 6572 7322 0a09 434f 4d4d  "counters"..COMM
-00015a10: 4f4e 5f43 4f55 4e54 203d 2022 636f 6d6d  ON_COUNT = "comm
-00015a20: 6f6e 5f63 6f75 6e74 220a 094f 4e4c 494e  on_count"..ONLIN
-00015a30: 455f 494e 464f 203d 2022 6f6e 6c69 6e65  E_INFO = "online
-00015a40: 5f69 6e66 6f22 0a09 4f43 4355 5041 5449  _info"..OCCUPATI
-00015a50: 4f4e 203d 2022 6f63 6375 7061 7469 6f6e  ON = "occupation
-00015a60: 220a 094e 4943 4b4e 414d 4520 3d20 226e  "..NICKNAME = "n
-00015a70: 6963 6b6e 616d 6522 0a09 5245 4c41 5449  ickname"..RELATI
-00015a80: 5645 5320 3d20 2272 656c 6174 6976 6573  VES = "relatives
-00015a90: 220a 0952 454c 4154 494f 4e20 3d20 2272  "..RELATION = "r
-00015aa0: 656c 6174 696f 6e22 0a09 5045 5253 4f4e  elation"..PERSON
-00015ab0: 414c 203d 2022 7065 7273 6f6e 616c 220a  AL = "personal".
-00015ac0: 0943 4f4e 4e45 4354 494f 4e53 203d 2022  .CONNECTIONS = "
-00015ad0: 636f 6e6e 6563 7469 6f6e 7322 0a09 4558  connections"..EX
-00015ae0: 504f 5254 5320 3d20 2265 7870 6f72 7473  PORTS = "exports
-00015af0: 220a 0957 414c 4c5f 434f 4d4d 454e 5453  "..WALL_COMMENTS
-00015b00: 203d 2022 7761 6c6c 5f63 6f6d 6d65 6e74   = "wall_comment
-00015b10: 7322 0a09 5741 4c4c 5f44 4546 4155 4c54  s"..WALL_DEFAULT
-00015b20: 203d 2022 7761 6c6c 5f64 6566 6175 6c74   = "wall_default
-00015b30: 220a 0941 4354 4956 4954 4945 5320 3d20  "..ACTIVITIES = 
-00015b40: 2261 6374 6976 6974 6965 7322 0a09 4143  "activities"..AC
-00015b50: 5449 5649 5459 203d 2022 6163 7469 7669  TIVITY = "activi
-00015b60: 7479 220a 0949 4e54 4552 4553 5453 203d  ty"..INTERESTS =
-00015b70: 2022 696e 7465 7265 7374 7322 0a09 4d55   "interests"..MU
-00015b80: 5349 4320 3d20 226d 7573 6963 220a 094d  SIC = "music"..M
-00015b90: 4f56 4945 5320 3d20 226d 6f76 6965 7322  OVIES = "movies"
-00015ba0: 0a09 5456 203d 2022 7476 220a 0942 4f4f  ..TV = "tv"..BOO
-00015bb0: 4b53 203d 2022 626f 6f6b 7322 0a09 4953  KS = "books"..IS
-00015bc0: 5f4e 4f5f 494e 4445 5820 3d20 2269 735f  _NO_INDEX = "is_
-00015bd0: 6e6f 5f69 6e64 6578 220a 0947 414d 4553  no_index"..GAMES
-00015be0: 203d 2022 6761 6d65 7322 0a09 4142 4f55   = "games"..ABOU
-00015bf0: 5420 3d20 2261 626f 7574 220a 0951 554f  T = "about"..QUO
-00015c00: 5445 5320 3d20 2271 756f 7465 7322 0a09  TES = "quotes"..
-00015c10: 4341 4e5f 504f 5354 203d 2022 6361 6e5f  CAN_POST = "can_
-00015c20: 706f 7374 220a 0943 414e 5f53 4545 5f41  post"..CAN_SEE_A
-00015c30: 4c4c 5f50 4f53 5453 203d 2022 6361 6e5f  LL_POSTS = "can_
-00015c40: 7365 655f 616c 6c5f 706f 7374 7322 0a09  see_all_posts"..
-00015c50: 4341 4e5f 5345 455f 4155 4449 4f20 3d20  CAN_SEE_AUDIO = 
-00015c60: 2263 616e 5f73 6565 5f61 7564 696f 220a  "can_see_audio".
-00015c70: 0943 414e 5f53 4545 5f47 4946 5453 203d  .CAN_SEE_GIFTS =
-00015c80: 2022 6361 6e5f 7365 655f 6769 6674 7322   "can_see_gifts"
-00015c90: 0a09 574f 524b 203d 2022 776f 726b 220a  ..WORK = "work".
-00015ca0: 0950 4c41 4345 5320 3d20 2270 6c61 6365  .PLACES = "place
-00015cb0: 7322 0a09 4341 4e5f 5752 4954 455f 5052  s"..CAN_WRITE_PR
-00015cc0: 4956 4154 455f 4d45 5353 4147 4520 3d20  IVATE_MESSAGE = 
-00015cd0: 2263 616e 5f77 7269 7465 5f70 7269 7661  "can_write_priva
-00015ce0: 7465 5f6d 6573 7361 6765 220a 0943 414e  te_message"..CAN
-00015cf0: 5f53 454e 445f 4652 4945 4e44 5f52 4551  _SEND_FRIEND_REQ
-00015d00: 5545 5354 203d 2022 6361 6e5f 7365 6e64  UEST = "can_send
-00015d10: 5f66 7269 656e 645f 7265 7175 6573 7422  _friend_request"
-00015d20: 0a09 4341 4e5f 5550 4c4f 4144 5f44 4f43  ..CAN_UPLOAD_DOC
-00015d30: 203d 2022 6361 6e5f 7570 6c6f 6164 5f64   = "can_upload_d
-00015d40: 6f63 220a 0949 535f 4641 564f 5249 5445  oc"..IS_FAVORITE
-00015d50: 203d 2022 6973 5f66 6176 6f72 6974 6522   = "is_favorite"
-00015d60: 0a09 4953 5f48 4944 4445 4e5f 4652 4f4d  ..IS_HIDDEN_FROM
-00015d70: 5f46 4545 4420 3d20 2269 735f 6869 6464  _FEED = "is_hidd
-00015d80: 656e 5f66 726f 6d5f 6665 6564 220a 0954  en_from_feed"..T
-00015d90: 494d 455a 4f4e 4520 3d20 2274 696d 657a  IMEZONE = "timez
-00015da0: 6f6e 6522 0a09 5343 5245 454e 5f4e 414d  one"..SCREEN_NAM
-00015db0: 4520 3d20 2273 6372 6565 6e5f 6e61 6d65  E = "screen_name
-00015dc0: 220a 094d 4149 4445 4e5f 4e41 4d45 203d  "..MAIDEN_NAME =
-00015dd0: 2022 6d61 6964 656e 5f6e 616d 6522 0a09   "maiden_name"..
-00015de0: 4352 4f50 5f50 484f 544f 203d 2022 6372  CROP_PHOTO = "cr
-00015df0: 6f70 5f70 686f 746f 220a 0949 535f 4652  op_photo"..IS_FR
-00015e00: 4945 4e44 203d 2022 6973 5f66 7269 656e  IEND = "is_frien
-00015e10: 6422 0a09 4652 4945 4e44 5f53 5441 5455  d"..FRIEND_STATU
-00015e20: 5320 3d20 2266 7269 656e 645f 7374 6174  S = "friend_stat
-00015e30: 7573 220a 0943 4152 4545 5220 3d20 2263  us"..CAREER = "c
-00015e40: 6172 6565 7222 0a09 4d49 4c49 5441 5259  areer"..MILITARY
-00015e50: 203d 2022 6d69 6c69 7461 7279 220a 0942   = "military"..B
-00015e60: 4c41 434b 4c49 5354 4544 203d 2022 626c  LACKLISTED = "bl
-00015e70: 6163 6b6c 6973 7465 6422 0a09 424c 4143  acklisted"..BLAC
-00015e80: 4b4c 4953 5445 445f 4259 5f4d 4520 3d20  KLISTED_BY_ME = 
-00015e90: 2262 6c61 636b 6c69 7374 6564 5f62 795f  "blacklisted_by_
-00015ea0: 6d65 220a 0943 414e 5f53 5542 5343 5249  me"..CAN_SUBSCRI
-00015eb0: 4245 5f50 4f53 5453 203d 2022 6361 6e5f  BE_POSTS = "can_
-00015ec0: 7375 6273 6372 6962 655f 706f 7374 7322  subscribe_posts"
-00015ed0: 0a09 4445 5343 5249 5054 494f 4e53 203d  ..DESCRIPTIONS =
-00015ee0: 2022 6465 7363 7269 7074 696f 6e73 220a   "descriptions".
-00015ef0: 0954 5245 4e44 494e 4720 3d20 2274 7265  .TRENDING = "tre
-00015f00: 6e64 696e 6722 0a09 4d55 5455 414c 203d  nding"..MUTUAL =
-00015f10: 2022 6d75 7475 616c 220a 0946 5249 454e   "mutual"..FRIEN
-00015f20: 4453 4849 505f 5745 454b 5320 3d20 2266  DSHIP_WEEKS = "f
-00015f30: 7269 656e 6473 6869 705f 7765 656b 7322  riendship_weeks"
-00015f40: 0a09 4341 4e5f 494e 5649 5445 5f54 4f5f  ..CAN_INVITE_TO_
-00015f50: 4348 4154 5320 3d20 2263 616e 5f69 6e76  CHATS = "can_inv
-00015f60: 6974 655f 746f 5f63 6861 7473 220a 0953  ite_to_chats"..S
-00015f70: 544f 5249 4553 5f41 5243 4849 5645 5f43  TORIES_ARCHIVE_C
-00015f80: 4f55 4e54 203d 2022 7374 6f72 6965 735f  OUNT = "stories_
-00015f90: 6172 6368 6976 655f 636f 756e 7422 0a09  archive_count"..
-00015fa0: 4841 535f 554e 5345 454e 5f53 544f 5249  HAS_UNSEEN_STORI
-00015fb0: 4553 203d 2022 6861 735f 756e 7365 656e  ES = "has_unseen
-00015fc0: 5f73 746f 7269 6573 220a 0956 4944 454f  _stories"..VIDEO
-00015fd0: 5f4c 4956 4520 3d20 2276 6964 656f 5f6c  _LIVE = "video_l
-00015fe0: 6976 6522 0a09 5649 4445 4f5f 4c49 5645  ive"..VIDEO_LIVE
-00015ff0: 5f4c 4556 454c 203d 2022 7669 6465 6f5f  _LEVEL = "video_
-00016000: 6c69 7665 5f6c 6576 656c 220a 0956 4944  live_level"..VID
-00016010: 454f 5f4c 4956 455f 434f 554e 5420 3d20  EO_LIVE_COUNT = 
-00016020: 2276 6964 656f 5f6c 6976 655f 636f 756e  "video_live_coun
-00016030: 7422 0a09 434c 4950 535f 434f 554e 5420  t"..CLIPS_COUNT 
-00016040: 3d20 2263 6c69 7073 5f63 6f75 6e74 220a  = "clips_count".
-00016050: 0953 4552 5649 4345 5f44 4553 4352 4950  .SERVICE_DESCRIP
-00016060: 5449 4f4e 203d 2022 7365 7276 6963 655f  TION = "service_
-00016070: 6465 7363 7269 7074 696f 6e22 0a09 4341  description"..CA
-00016080: 4e5f 5345 455f 5749 5348 4553 203d 2022  N_SEE_WISHES = "
-00016090: 6361 6e5f 7365 655f 7769 7368 6573 220a  can_see_wishes".
-000160a0: 0949 535f 5355 4253 4352 4942 4544 5f50  .IS_SUBSCRIBED_P
-000160b0: 4f44 4341 5354 5320 3d20 2269 735f 7375  ODCASTS = "is_su
-000160c0: 6273 6372 6962 6564 5f70 6f64 6361 7374  bscribed_podcast
-000160d0: 7322 0a09 4341 4e5f 5355 4253 4352 4942  s"..CAN_SUBSCRIB
-000160e0: 455f 504f 4443 4153 5453 203d 2022 6361  E_PODCASTS = "ca
-000160f0: 6e5f 7375 6273 6372 6962 655f 706f 6463  n_subscribe_podc
-00016100: 6173 7473 220a 0a63 6c61 7373 2055 7365  asts"..class Use
-00016110: 7273 5573 6572 5265 6c61 7469 6f6e 2845  rsUserRelation(E
-00016120: 6e75 6d29 3a0a 094e 4f54 5f53 5045 4349  num):..NOT_SPECI
-00016130: 4649 4544 203d 2030 0a09 5349 4e47 4c45  FIED = 0..SINGLE
-00016140: 203d 2031 0a09 494e 5f41 5f52 454c 4154   = 1..IN_A_RELAT
-00016150: 494f 4e53 4849 5020 3d20 320a 0945 4e47  IONSHIP = 2..ENG
-00016160: 4147 4544 203d 2033 0a09 4d41 5252 4945  AGED = 3..MARRIE
-00016170: 4420 3d20 340a 0943 4f4d 504c 4943 4154  D = 4..COMPLICAT
-00016180: 4544 203d 2035 0a09 4143 5449 5645 4c59  ED = 5..ACTIVELY
-00016190: 5f53 4541 5243 4849 4e47 203d 2036 0a09  _SEARCHING = 6..
-000161a0: 494e 5f4c 4f56 4520 3d20 370a 0949 4e5f  IN_LOVE = 7..IN_
-000161b0: 415f 4349 5649 4c5f 554e 494f 4e20 3d20  A_CIVIL_UNION = 
-000161c0: 380a 0a63 6c61 7373 2055 7365 7273 5573  8..class UsersUs
-000161d0: 6572 5479 7065 2845 6e75 6d29 3a0a 0950  erType(Enum):..P
-000161e0: 524f 4649 4c45 203d 2022 7072 6f66 696c  ROFILE = "profil
-000161f0: 6522 0a0a 636c 6173 7320 5573 6572 7343  e"..class UsersC
-00016200: 6172 6565 7228 424d 293a 0a09 6369 7479  areer(BM):..city
-00016210: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-00016220: 5d20 3d20 4e6f 6e65 0a09 6369 7479 5f6e  ] = None..city_n
-00016230: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
-00016240: 5d20 3d20 4e6f 6e65 0a09 636f 6d70 616e  ] = None..compan
-00016250: 793a 4f70 7469 6f6e 616c 5b73 7472 5d20  y:Optional[str] 
-00016260: 3d20 4e6f 6e65 0a09 636f 756e 7472 795f  = None..country_
-00016270: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-00016280: 203d 204e 6f6e 650a 095f 6672 6f6d 3a4f   = None.._from:O
-00016290: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000162a0: 6f6e 650a 0967 726f 7570 5f69 643a 4f70  one..group_id:Op
-000162b0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000162c0: 6e65 0a09 6964 3a4f 7074 696f 6e61 6c5b  ne..id:Optional[
-000162d0: 696e 745d 203d 204e 6f6e 650a 0970 6f73  int] = None..pos
-000162e0: 6974 696f 6e3a 4f70 7469 6f6e 616c 5b73  ition:Optional[s
-000162f0: 7472 5d20 3d20 4e6f 6e65 0a09 756e 7469  tr] = None..unti
-00016300: 6c3a 4f70 7469 6f6e 616c 5b69 6e74 5d20  l:Optional[int] 
-00016310: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2055  = None...class U
-00016320: 7365 7273 4578 706f 7274 7328 424d 293a  sersExports(BM):
-00016330: 0a09 6661 6365 626f 6f6b 3a4f 7074 696f  ..facebook:Optio
-00016340: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00016350: 096c 6976 656a 6f75 726e 616c 3a4f 7074  .livejournal:Opt
-00016360: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00016370: 650a 0974 7769 7474 6572 3a4f 7074 696f  e..twitter:Optio
-00016380: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00016390: 0a0a 636c 6173 7320 5573 6572 734c 6173  ..class UsersLas
-000163a0: 7453 6565 6e28 424d 293a 0a09 706c 6174  tSeen(BM):..plat
-000163b0: 666f 726d 3a4f 7074 696f 6e61 6c5b 696e  form:Optional[in
-000163c0: 745d 203d 204e 6f6e 650a 0974 696d 653a  t] = None..time:
-000163d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000163e0: 4e6f 6e65 0a0a 0a63 6c61 7373 2055 7365  None...class Use
-000163f0: 7273 4d69 6c69 7461 7279 2842 4d29 3a0a  rsMilitary(BM):.
-00016400: 0963 6f75 6e74 7279 5f69 643a 696e 740a  .country_id:int.
-00016410: 095f 6672 6f6d 3a4f 7074 696f 6e61 6c5b  ._from:Optional[
-00016420: 696e 745d 203d 204e 6f6e 650a 0969 643a  int] = None..id:
-00016430: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00016440: 4e6f 6e65 0a09 756e 6974 3a73 7472 0a09  None..unit:str..
-00016450: 756e 6974 5f69 643a 696e 740a 0975 6e74  unit_id:int..unt
-00016460: 696c 3a4f 7074 696f 6e61 6c5b 696e 745d  il:Optional[int]
-00016470: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
-00016480: 5573 6572 734f 6363 7570 6174 696f 6e28  UsersOccupation(
-00016490: 424d 293a 0a09 6964 3a4f 7074 696f 6e61  BM):..id:Optiona
-000164a0: 6c5b 696e 745d 203d 204e 6f6e 650a 096e  l[int] = None..n
-000164b0: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
-000164c0: 5d20 3d20 4e6f 6e65 0a09 7479 7065 3a4f  ] = None..type:O
-000164d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-000164e0: 6f6e 650a 0a0a 636c 6173 7320 5573 6572  one...class User
-000164f0: 734f 6e6c 696e 6549 6e66 6f28 424d 293a  sOnlineInfo(BM):
-00016500: 0a09 7669 7369 626c 653a 626f 6f6c 0a09  ..visible:bool..
-00016510: 6c61 7374 5f73 6565 6e3a 4f70 7469 6f6e  last_seen:Option
-00016520: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00016530: 6973 5f6f 6e6c 696e 653a 4f70 7469 6f6e  is_online:Option
-00016540: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-00016550: 0961 7070 5f69 643a 4f70 7469 6f6e 616c  .app_id:Optional
-00016560: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6973  [int] = None..is
-00016570: 5f6d 6f62 696c 653a 4f70 7469 6f6e 616c  _mobile:Optional
-00016580: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0973  [bool] = None..s
-00016590: 7461 7475 733a 4f70 7469 6f6e 616c 5b73  tatus:Optional[s
-000165a0: 7472 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  tr] = None...cla
-000165b0: 7373 2055 7365 7273 5065 7273 6f6e 616c  ss UsersPersonal
-000165c0: 2842 4d29 3a0a 0961 6c63 6f68 6f6c 3a4f  (BM):..alcohol:O
-000165d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000165e0: 6f6e 650a 0969 6e73 7069 7265 645f 6279  one..inspired_by
-000165f0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00016600: 204e 6f6e 650a 096c 616e 6773 3a4f 7074   None..langs:Opt
-00016610: 696f 6e61 6c5b 6c69 7374 5b73 7472 5d5d  ional[list[str]]
-00016620: 203d 204e 6f6e 650a 096c 6966 655f 6d61   = None..life_ma
-00016630: 696e 3a4f 7074 696f 6e61 6c5b 696e 745d  in:Optional[int]
-00016640: 203d 204e 6f6e 650a 0970 656f 706c 655f   = None..people_
-00016650: 6d61 696e 3a4f 7074 696f 6e61 6c5b 696e  main:Optional[in
-00016660: 745d 203d 204e 6f6e 650a 0970 6f6c 6974  t] = None..polit
-00016670: 6963 616c 3a4f 7074 696f 6e61 6c5b 696e  ical:Optional[in
-00016680: 745d 203d 204e 6f6e 650a 0972 656c 6967  t] = None..relig
-00016690: 696f 6e3a 4f70 7469 6f6e 616c 5b73 7472  ion:Optional[str
-000166a0: 5d20 3d20 4e6f 6e65 0a09 7265 6c69 6769  ] = None..religi
-000166b0: 6f6e 5f69 643a 4f70 7469 6f6e 616c 5b69  on_id:Optional[i
-000166c0: 6e74 5d20 3d20 4e6f 6e65 0a09 736d 6f6b  nt] = None..smok
-000166d0: 696e 673a 4f70 7469 6f6e 616c 5b69 6e74  ing:Optional[int
-000166e0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
-000166f0: 2055 7365 7273 5265 6c61 7469 7665 2842   UsersRelative(B
-00016700: 4d29 3a0a 0962 6972 7468 5f64 6174 653a  M):..birth_date:
-00016710: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00016720: 4e6f 6e65 0a09 6964 3a4f 7074 696f 6e61  None..id:Optiona
-00016730: 6c5b 696e 745d 203d 204e 6f6e 650a 096e  l[int] = None..n
-00016740: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
-00016750: 5d20 3d20 4e6f 6e65 0a09 7479 7065 3a73  ] = None..type:s
-00016760: 7472 0a0a 0a63 6c61 7373 2055 7365 7273  tr...class Users
-00016770: 5363 686f 6f6c 2842 4d29 3a0a 0963 6974  School(BM):..cit
-00016780: 793a 4f70 7469 6f6e 616c 5b69 6e74 5d20  y:Optional[int] 
-00016790: 3d20 4e6f 6e65 0a09 5f63 6c61 7373 3a4f  = None.._class:O
-000167a0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-000167b0: 6f6e 650a 0963 6f75 6e74 7279 3a4f 7074  one..country:Opt
-000167c0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-000167d0: 650a 0969 643a 4f70 7469 6f6e 616c 5b73  e..id:Optional[s
-000167e0: 7472 5d20 3d20 4e6f 6e65 0a09 6e61 6d65  tr] = None..name
-000167f0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00016800: 204e 6f6e 650a 0974 7970 653a 4f70 7469   None..type:Opti
-00016810: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00016820: 0a09 7479 7065 5f73 7472 3a4f 7074 696f  ..type_str:Optio
-00016830: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00016840: 0979 6561 725f 6672 6f6d 3a4f 7074 696f  .year_from:Optio
-00016850: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00016860: 0979 6561 725f 6772 6164 7561 7465 643a  .year_graduated:
-00016870: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00016880: 4e6f 6e65 0a09 7965 6172 5f74 6f3a 4f70  None..year_to:Op
-00016890: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000168a0: 6e65 0a09 7370 6563 6961 6c69 7479 3a4f  ne..speciality:O
-000168b0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-000168c0: 6f6e 650a 0a0a 636c 6173 7320 5573 6572  one...class User
-000168d0: 7353 7562 7363 7269 7074 696f 6e73 4974  sSubscriptionsIt
-000168e0: 656d 2842 4d29 3a0a 0970 6173 730a 0a63  em(BM):..pass..c
-000168f0: 6c61 7373 2055 7365 7273 556e 6976 6572  lass UsersUniver
-00016900: 7369 7479 2842 4d29 3a0a 0963 6861 6972  sity(BM):..chair
-00016910: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00016920: 204e 6f6e 650a 0963 6861 6972 5f6e 616d   None..chair_nam
-00016930: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-00016940: 3d20 4e6f 6e65 0a09 6369 7479 3a4f 7074  = None..city:Opt
-00016950: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00016960: 650a 0963 6f75 6e74 7279 3a4f 7074 696f  e..country:Optio
-00016970: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00016980: 0965 6475 6361 7469 6f6e 5f66 6f72 6d3a  .education_form:
-00016990: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000169a0: 4e6f 6e65 0a09 6564 7563 6174 696f 6e5f  None..education_
-000169b0: 7374 6174 7573 3a4f 7074 696f 6e61 6c5b  status:Optional[
-000169c0: 7374 725d 203d 204e 6f6e 650a 0966 6163  str] = None..fac
-000169d0: 756c 7479 3a4f 7074 696f 6e61 6c5b 696e  ulty:Optional[in
-000169e0: 745d 203d 204e 6f6e 650a 0966 6163 756c  t] = None..facul
-000169f0: 7479 5f6e 616d 653a 4f70 7469 6f6e 616c  ty_name:Optional
-00016a00: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6772  [str] = None..gr
-00016a10: 6164 7561 7469 6f6e 3a4f 7074 696f 6e61  aduation:Optiona
-00016a20: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
-00016a30: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-00016a40: 3d20 4e6f 6e65 0a09 6e61 6d65 3a4f 7074  = None..name:Opt
-00016a50: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00016a60: 650a 0975 6e69 7665 7273 6974 795f 6772  e..university_gr
-00016a70: 6f75 705f 6964 3a4f 7074 696f 6e61 6c5b  oup_id:Optional[
-00016a80: 696e 745d 203d 204e 6f6e 650a 0a0a 636c  int] = None...cl
-00016a90: 6173 7320 5573 6572 7355 7365 7243 6f6e  ass UsersUserCon
-00016aa0: 6e65 6374 696f 6e73 2842 4d29 3a0a 0973  nections(BM):..s
-00016ab0: 6b79 7065 3a73 7472 0a09 6661 6365 626f  kype:str..facebo
-00016ac0: 6f6b 3a73 7472 0a09 6661 6365 626f 6f6b  ok:str..facebook
-00016ad0: 5f6e 616d 653a 4f70 7469 6f6e 616c 5b73  _name:Optional[s
-00016ae0: 7472 5d20 3d20 4e6f 6e65 0a09 7477 6974  tr] = None..twit
-00016af0: 7465 723a 7374 720a 096c 6976 656a 6f75  ter:str..livejou
-00016b00: 726e 616c 3a4f 7074 696f 6e61 6c5b 7374  rnal:Optional[st
-00016b10: 725d 203d 204e 6f6e 650a 0969 6e73 7461  r] = None..insta
-00016b20: 6772 616d 3a73 7472 0a0a 0a63 6c61 7373  gram:str...class
-00016b30: 2055 7365 7273 5573 6572 436f 756e 7465   UsersUserCounte
-00016b40: 7273 2842 4d29 3a0a 0961 6c62 756d 733a  rs(BM):..albums:
-00016b50: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00016b60: 4e6f 6e65 0a09 6261 6467 6573 3a4f 7074  None..badges:Opt
-00016b70: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00016b80: 650a 0961 7564 696f 733a 4f70 7469 6f6e  e..audios:Option
-00016b90: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00016ba0: 666f 6c6c 6f77 6572 733a 4f70 7469 6f6e  followers:Option
-00016bb0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00016bc0: 6672 6965 6e64 733a 4f70 7469 6f6e 616c  friends:Optional
-00016bd0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6769  [int] = None..gi
-00016be0: 6674 733a 4f70 7469 6f6e 616c 5b69 6e74  fts:Optional[int
-00016bf0: 5d20 3d20 4e6f 6e65 0a09 6772 6f75 7073  ] = None..groups
-00016c00: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00016c10: 204e 6f6e 650a 096e 6f74 6573 3a4f 7074   None..notes:Opt
-00016c20: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00016c30: 650a 096f 6e6c 696e 655f 6672 6965 6e64  e..online_friend
-00016c40: 733a 4f70 7469 6f6e 616c 5b69 6e74 5d20  s:Optional[int] 
-00016c50: 3d20 4e6f 6e65 0a09 7061 6765 733a 4f70  = None..pages:Op
-00016c60: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00016c70: 6e65 0a09 7068 6f74 6f73 3a4f 7074 696f  ne..photos:Optio
-00016c80: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00016c90: 0973 7562 7363 7269 7074 696f 6e73 3a4f  .subscriptions:O
-00016ca0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00016cb0: 6f6e 650a 0975 7365 725f 7068 6f74 6f73  one..user_photos
-00016cc0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00016cd0: 204e 6f6e 650a 0975 7365 725f 7669 6465   None..user_vide
-00016ce0: 6f73 3a4f 7074 696f 6e61 6c5b 696e 745d  os:Optional[int]
-00016cf0: 203d 204e 6f6e 650a 0976 6964 656f 733a   = None..videos:
-00016d00: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00016d10: 4e6f 6e65 0a09 6e65 775f 7068 6f74 6f5f  None..new_photo_
-00016d20: 7461 6773 3a4f 7074 696f 6e61 6c5b 696e  tags:Optional[in
-00016d30: 745d 203d 204e 6f6e 650a 096e 6577 5f72  t] = None..new_r
-00016d40: 6563 6f67 6e69 7469 6f6e 5f74 6167 733a  ecognition_tags:
-00016d50: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00016d60: 4e6f 6e65 0a09 6d75 7475 616c 5f66 7269  None..mutual_fri
-00016d70: 656e 6473 3a4f 7074 696f 6e61 6c5b 696e  ends:Optional[in
-00016d80: 745d 203d 204e 6f6e 650a 0970 6f73 7473  t] = None..posts
-00016d90: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00016da0: 204e 6f6e 650a 0961 7274 6963 6c65 733a   None..articles:
-00016db0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00016dc0: 4e6f 6e65 0a09 7769 7368 6573 3a4f 7074  None..wishes:Opt
-00016dd0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00016de0: 650a 0970 6f64 6361 7374 733a 4f70 7469  e..podcasts:Opti
-00016df0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00016e00: 0a09 636c 6970 733a 4f70 7469 6f6e 616c  ..clips:Optional
-00016e10: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 636c  [int] = None..cl
-00016e20: 6970 735f 666f 6c6c 6f77 6572 733a 4f70  ips_followers:Op
-00016e30: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00016e40: 6e65 0a0a 0a63 6c61 7373 2055 7365 7273  ne...class Users
-00016e50: 5573 6572 4d69 6e28 424d 293a 0a09 6465  UserMin(BM):..de
-00016e60: 6163 7469 7661 7465 643a 4f70 7469 6f6e  activated:Option
-00016e70: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00016e80: 6669 7273 745f 6e61 6d65 3a4f 7074 696f  first_name:Optio
-00016e90: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00016ea0: 0968 6964 6465 6e3a 4f70 7469 6f6e 616c  .hidden:Optional
-00016eb0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6964  [int] = None..id
-00016ec0: 3a69 6e74 0a09 6c61 7374 5f6e 616d 653a  :int..last_name:
-00016ed0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00016ee0: 4e6f 6e65 0a09 6361 6e5f 6163 6365 7373  None..can_access
-00016ef0: 5f63 6c6f 7365 643a 4f70 7469 6f6e 616c  _closed:Optional
-00016f00: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0969  [bool] = None..i
-00016f10: 735f 636c 6f73 6564 3a4f 7074 696f 6e61  s_closed:Optiona
-00016f20: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a  l[bool] = None..
-00016f30: 0a63 6c61 7373 2055 7365 7273 5573 6572  .class UsersUser
-00016f40: 5365 7474 696e 6773 5874 7228 424d 293a  SettingsXtr(BM):
-00016f50: 0a09 636f 6e6e 6563 7469 6f6e 733a 4f70  ..connections:Op
-00016f60: 7469 6f6e 616c 5b22 5573 6572 7355 7365  tional["UsersUse
-00016f70: 7243 6f6e 6e65 6374 696f 6e73 225d 203d  rConnections"] =
-00016f80: 204e 6f6e 650a 0962 6461 7465 3a4f 7074   None..bdate:Opt
-00016f90: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00016fa0: 650a 0962 6461 7465 5f76 6973 6962 696c  e..bdate_visibil
-00016fb0: 6974 793a 4f70 7469 6f6e 616c 5b69 6e74  ity:Optional[int
-00016fc0: 5d20 3d20 4e6f 6e65 0a09 6369 7479 3a4f  ] = None..city:O
-00016fd0: 7074 696f 6e61 6c5b 2242 6173 6543 6974  ptional["BaseCit
-00016fe0: 7922 5d20 3d20 4e6f 6e65 0a09 636f 756e  y"] = None..coun
-00016ff0: 7472 793a 4f70 7469 6f6e 616c 5b22 4261  try:Optional["Ba
-00017000: 7365 436f 756e 7472 7922 5d20 3d20 4e6f  seCountry"] = No
-00017010: 6e65 0a09 6669 7273 745f 6e61 6d65 3a4f  ne..first_name:O
-00017020: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00017030: 6f6e 650a 0968 6f6d 655f 746f 776e 3a73  one..home_town:s
-00017040: 7472 0a09 6c61 7374 5f6e 616d 653a 4f70  tr..last_name:Op
-00017050: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00017060: 6e65 0a09 6d61 6964 656e 5f6e 616d 653a  ne..maiden_name:
-00017070: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00017080: 4e6f 6e65 0a09 6e61 6d65 5f72 6571 7565  None..name_reque
-00017090: 7374 3a4f 7074 696f 6e61 6c5b 2241 6363  st:Optional["Acc
-000170a0: 6f75 6e74 4e61 6d65 5265 7175 6573 7422  ountNameRequest"
-000170b0: 5d20 3d20 4e6f 6e65 0a09 7065 7273 6f6e  ] = None..person
-000170c0: 616c 3a4f 7074 696f 6e61 6c5b 2255 7365  al:Optional["Use
-000170d0: 7273 5065 7273 6f6e 616c 225d 203d 204e  rsPersonal"] = N
-000170e0: 6f6e 650a 0970 686f 6e65 3a4f 7074 696f  one..phone:Optio
-000170f0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00017100: 0972 656c 6174 696f 6e3a 4f70 7469 6f6e  .relation:Option
-00017110: 616c 5b22 5573 6572 7355 7365 7252 656c  al["UsersUserRel
-00017120: 6174 696f 6e22 5d20 3d20 4e6f 6e65 0a09  ation"] = None..
-00017130: 7265 6c61 7469 6f6e 5f70 6172 746e 6572  relation_partner
-00017140: 3a4f 7074 696f 6e61 6c5b 2255 7365 7273  :Optional["Users
-00017150: 5573 6572 4d69 6e22 5d20 3d20 4e6f 6e65  UserMin"] = None
-00017160: 0a09 7265 6c61 7469 6f6e 5f70 656e 6469  ..relation_pendi
-00017170: 6e67 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ng:Optional[bool
-00017180: 5d20 3d20 4e6f 6e65 0a09 7265 6c61 7469  ] = None..relati
-00017190: 6f6e 5f72 6571 7565 7374 733a 4f70 7469  on_requests:Opti
-000171a0: 6f6e 616c 5b6c 6973 745b 2255 7365 7273  onal[list["Users
-000171b0: 5573 6572 4d69 6e22 5d5d 203d 204e 6f6e  UserMin"]] = Non
-000171c0: 650a 0973 6372 6565 6e5f 6e61 6d65 3a4f  e..screen_name:O
-000171d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-000171e0: 6f6e 650a 0973 6578 3a4f 7074 696f 6e61  one..sex:Optiona
-000171f0: 6c5b 2242 6173 6553 6578 225d 203d 204e  l["BaseSex"] = N
-00017200: 6f6e 650a 0973 7461 7475 733a 7374 720a  one..status:str.
-00017210: 0973 7461 7475 735f 6175 6469 6f3a 4f70  .status_audio:Op
-00017220: 7469 6f6e 616c 5b22 4175 6469 6f41 7564  tional["AudioAud
-00017230: 696f 225d 203d 204e 6f6e 650a 0969 6e74  io"] = None..int
-00017240: 6572 6573 7473 3a4f 7074 696f 6e61 6c5b  erests:Optional[
-00017250: 2241 6363 6f75 6e74 5573 6572 5365 7474  "AccountUserSett
-00017260: 696e 6773 496e 7465 7265 7374 7322 5d20  ingsInterests"] 
-00017270: 3d20 4e6f 6e65 0a09 6c61 6e67 7561 6765  = None..language
-00017280: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-00017290: 7374 725d 5d20 3d20 4e6f 6e65 0a0a 0a63  str]] = None...c
-000172a0: 6c61 7373 2055 7365 7273 5573 6572 7341  lass UsersUsersA
-000172b0: 7272 6179 2842 4d29 3a0a 0963 6f75 6e74  rray(BM):..count
-000172c0: 3a69 6e74 0a09 6974 656d 733a 6c69 7374  :int..items:list
-000172d0: 5b69 6e74 5d0a 0a0a 0a0a 636c 6173 7320  [int].....class 
-000172e0: 5574 696c 7344 6f6d 6169 6e52 6573 6f6c  UtilsDomainResol
-000172f0: 7665 6454 7970 6528 456e 756d 293a 0a09  vedType(Enum):..
-00017300: 5553 4552 203d 2022 7573 6572 220a 0947  USER = "user"..G
-00017310: 524f 5550 203d 2022 6772 6f75 7022 0a09  ROUP = "group"..
-00017320: 4150 504c 4943 4154 494f 4e20 3d20 2261  APPLICATION = "a
-00017330: 7070 6c69 6361 7469 6f6e 220a 0950 4147  pplication"..PAG
-00017340: 4520 3d20 2270 6167 6522 0a09 564b 5f41  E = "page"..VK_A
-00017350: 5050 203d 2022 766b 5f61 7070 220a 0943  PP = "vk_app"..C
-00017360: 4f4d 4d55 4e49 5459 5f41 5050 4c49 4341  OMMUNITY_APPLICA
-00017370: 5449 4f4e 203d 2022 636f 6d6d 756e 6974  TION = "communit
-00017380: 795f 6170 706c 6963 6174 696f 6e22 0a0a  y_application"..
-00017390: 636c 6173 7320 5574 696c 734c 696e 6b43  class UtilsLinkC
-000173a0: 6865 636b 6564 5374 6174 7573 2845 6e75  heckedStatus(Enu
-000173b0: 6d29 3a0a 094e 4f54 5f42 414e 4e45 4420  m):..NOT_BANNED 
-000173c0: 3d20 226e 6f74 5f62 616e 6e65 6422 0a09  = "not_banned"..
-000173d0: 4241 4e4e 4544 203d 2022 6261 6e6e 6564  BANNED = "banned
-000173e0: 220a 0950 524f 4345 5353 494e 4720 3d20  "..PROCESSING = 
-000173f0: 2270 726f 6365 7373 696e 6722 0a0a 636c  "processing"..cl
-00017400: 6173 7320 5574 696c 7344 6f6d 6169 6e52  ass UtilsDomainR
-00017410: 6573 6f6c 7665 6428 424d 293a 0a09 6f62  esolved(BM):..ob
-00017420: 6a65 6374 5f69 643a 4f70 7469 6f6e 616c  ject_id:Optional
-00017430: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6772  [int] = None..gr
-00017440: 6f75 705f 6964 3a4f 7074 696f 6e61 6c5b  oup_id:Optional[
-00017450: 696e 745d 203d 204e 6f6e 650a 0974 7970  int] = None..typ
-00017460: 653a 4f70 7469 6f6e 616c 5b22 5574 696c  e:Optional["Util
-00017470: 7344 6f6d 6169 6e52 6573 6f6c 7665 6454  sDomainResolvedT
-00017480: 7970 6522 5d20 3d20 4e6f 6e65 0a0a 0a63  ype"] = None...c
-00017490: 6c61 7373 2055 7469 6c73 4c61 7374 5368  lass UtilsLastSh
-000174a0: 6f72 7465 6e65 644c 696e 6b28 424d 293a  ortenedLink(BM):
-000174b0: 0a09 6163 6365 7373 5f6b 6579 3a4f 7074  ..access_key:Opt
-000174c0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-000174d0: 650a 096b 6579 3a4f 7074 696f 6e61 6c5b  e..key:Optional[
-000174e0: 7374 725d 203d 204e 6f6e 650a 0973 686f  str] = None..sho
-000174f0: 7274 5f75 726c 3a4f 7074 696f 6e61 6c5b  rt_url:Optional[
-00017500: 7374 725d 203d 204e 6f6e 650a 0974 696d  str] = None..tim
-00017510: 6573 7461 6d70 3a4f 7074 696f 6e61 6c5b  estamp:Optional[
-00017520: 696e 745d 203d 204e 6f6e 650a 0975 726c  int] = None..url
-00017530: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00017540: 204e 6f6e 650a 0976 6965 7773 3a4f 7074   None..views:Opt
-00017550: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00017560: 650a 0a0a 636c 6173 7320 5574 696c 734c  e...class UtilsL
-00017570: 696e 6b43 6865 636b 6564 2842 4d29 3a0a  inkChecked(BM):.
-00017580: 096c 696e 6b3a 4f70 7469 6f6e 616c 5b73  .link:Optional[s
-00017590: 7472 5d20 3d20 4e6f 6e65 0a09 7374 6174  tr] = None..stat
-000175a0: 7573 3a4f 7074 696f 6e61 6c5b 2255 7469  us:Optional["Uti
-000175b0: 6c73 4c69 6e6b 4368 6563 6b65 6453 7461  lsLinkCheckedSta
-000175c0: 7475 7322 5d20 3d20 4e6f 6e65 0a0a 0a63  tus"] = None...c
-000175d0: 6c61 7373 2055 7469 6c73 4c69 6e6b 5374  lass UtilsLinkSt
-000175e0: 6174 7328 424d 293a 0a09 6b65 793a 4f70  ats(BM):..key:Op
-000175f0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00017600: 6e65 0a09 7374 6174 733a 4f70 7469 6f6e  ne..stats:Option
-00017610: 616c 5b6c 6973 745b 2255 7469 6c73 5374  al[list["UtilsSt
-00017620: 6174 7322 5d5d 203d 204e 6f6e 650a 0a0a  ats"]] = None...
-00017630: 636c 6173 7320 5574 696c 734c 696e 6b53  class UtilsLinkS
-00017640: 7461 7473 4578 7465 6e64 6564 2842 4d29  tatsExtended(BM)
-00017650: 3a0a 096b 6579 3a4f 7074 696f 6e61 6c5b  :..key:Optional[
-00017660: 7374 725d 203d 204e 6f6e 650a 0973 7461  str] = None..sta
-00017670: 7473 3a4f 7074 696f 6e61 6c5b 6c69 7374  ts:Optional[list
-00017680: 5b22 5574 696c 7353 7461 7473 4578 7465  ["UtilsStatsExte
-00017690: 6e64 6564 225d 5d20 3d20 4e6f 6e65 0a0a  nded"]] = None..
-000176a0: 0a63 6c61 7373 2055 7469 6c73 5368 6f72  .class UtilsShor
-000176b0: 744c 696e 6b28 424d 293a 0a09 6163 6365  tLink(BM):..acce
-000176c0: 7373 5f6b 6579 3a4f 7074 696f 6e61 6c5b  ss_key:Optional[
-000176d0: 7374 725d 203d 204e 6f6e 650a 096b 6579  str] = None..key
+00013590: 0a09 7569 643a 4f70 7469 6f6e 616c 5b69  ..uid:Optional[i
+000135a0: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  nt] = None...cla
+000135b0: 7373 2053 6563 7572 6553 6574 436f 756e  ss SecureSetCoun
+000135c0: 7465 7249 7465 6d28 424d 293a 0a09 6964  terItem(BM):..id
+000135d0: 3a69 6e74 0a09 7265 7375 6c74 3a62 6f6f  :int..result:boo
+000135e0: 6c0a 0a0a 636c 6173 7320 5365 6375 7265  l...class Secure
+000135f0: 536d 734e 6f74 6966 6963 6174 696f 6e28  SmsNotification(
+00013600: 424d 293a 0a09 6170 705f 6964 3a4f 7074  BM):..app_id:Opt
+00013610: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00013620: 650a 0964 6174 653a 4f70 7469 6f6e 616c  e..date:Optional
+00013630: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6964  [str] = None..id
+00013640: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00013650: 204e 6f6e 650a 096d 6573 7361 6765 3a4f   None..message:O
+00013660: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00013670: 6f6e 650a 0975 7365 725f 6964 3a4f 7074  one..user_id:Opt
+00013680: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00013690: 650a 0a0a 636c 6173 7320 5365 6375 7265  e...class Secure
+000136a0: 546f 6b65 6e43 6865 636b 6564 2842 4d29  TokenChecked(BM)
+000136b0: 3a0a 0964 6174 653a 4f70 7469 6f6e 616c  :..date:Optional
+000136c0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6578  [int] = None..ex
+000136d0: 7069 7265 3a4f 7074 696f 6e61 6c5b 696e  pire:Optional[in
+000136e0: 745d 203d 204e 6f6e 650a 0973 7563 6365  t] = None..succe
+000136f0: 7373 3a4f 7074 696f 6e61 6c5b 696e 745d  ss:Optional[int]
+00013700: 203d 204e 6f6e 650a 0975 7365 725f 6964   = None..user_id
+00013710: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00013720: 204e 6f6e 650a 0a0a 636c 6173 7320 5365   None...class Se
+00013730: 6375 7265 5472 616e 7361 6374 696f 6e28  cureTransaction(
+00013740: 424d 293a 0a09 6461 7465 3a4f 7074 696f  BM):..date:Optio
+00013750: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00013760: 0969 643a 4f70 7469 6f6e 616c 5b69 6e74  .id:Optional[int
+00013770: 5d20 3d20 4e6f 6e65 0a09 7569 645f 6672  ] = None..uid_fr
+00013780: 6f6d 3a4f 7074 696f 6e61 6c5b 696e 745d  om:Optional[int]
+00013790: 203d 204e 6f6e 650a 0975 6964 5f74 6f3a   = None..uid_to:
+000137a0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000137b0: 4e6f 6e65 0a09 766f 7465 733a 4f70 7469  None..votes:Opti
+000137c0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000137d0: 0a0a 0a0a 0a63 6c61 7373 2053 7461 7473  .....class Stats
+000137e0: 4163 7469 7669 7479 2842 4d29 3a0a 0963  Activity(BM):..c
+000137f0: 6f6d 6d65 6e74 733a 4f70 7469 6f6e 616c  omments:Optional
+00013800: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 636f  [int] = None..co
+00013810: 7069 6573 3a4f 7074 696f 6e61 6c5b 696e  pies:Optional[in
+00013820: 745d 203d 204e 6f6e 650a 0968 6964 6465  t] = None..hidde
+00013830: 6e3a 4f70 7469 6f6e 616c 5b69 6e74 5d20  n:Optional[int] 
+00013840: 3d20 4e6f 6e65 0a09 6c69 6b65 733a 4f70  = None..likes:Op
+00013850: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00013860: 6e65 0a09 7375 6273 6372 6962 6564 3a4f  ne..subscribed:O
+00013870: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00013880: 6f6e 650a 0975 6e73 7562 7363 7269 6265  one..unsubscribe
+00013890: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+000138a0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2053  = None...class S
+000138b0: 7461 7473 4369 7479 2842 4d29 3a0a 0963  tatsCity(BM):..c
+000138c0: 6f75 6e74 3a4f 7074 696f 6e61 6c5b 696e  ount:Optional[in
+000138d0: 745d 203d 204e 6f6e 650a 096e 616d 653a  t] = None..name:
+000138e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000138f0: 4e6f 6e65 0a09 7661 6c75 653a 4f70 7469  None..value:Opti
+00013900: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00013910: 0a0a 0a63 6c61 7373 2053 7461 7473 436f  ...class StatsCo
+00013920: 756e 7472 7928 424d 293a 0a09 636f 6465  untry(BM):..code
+00013930: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00013940: 204e 6f6e 650a 0963 6f75 6e74 3a4f 7074   None..count:Opt
+00013950: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00013960: 650a 096e 616d 653a 4f70 7469 6f6e 616c  e..name:Optional
+00013970: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7661  [str] = None..va
+00013980: 6c75 653a 4f70 7469 6f6e 616c 5b69 6e74  lue:Optional[int
+00013990: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+000139a0: 2053 7461 7473 5065 7269 6f64 2842 4d29   StatsPeriod(BM)
+000139b0: 3a0a 0961 6374 6976 6974 793a 4f70 7469  :..activity:Opti
+000139c0: 6f6e 616c 5b22 5374 6174 7341 6374 6976  onal["StatsActiv
+000139d0: 6974 7922 5d20 3d20 4e6f 6e65 0a09 7065  ity"] = None..pe
+000139e0: 7269 6f64 5f66 726f 6d3a 4f70 7469 6f6e  riod_from:Option
+000139f0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00013a00: 7065 7269 6f64 5f74 6f3a 4f70 7469 6f6e  period_to:Option
+00013a10: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00013a20: 7265 6163 683a 4f70 7469 6f6e 616c 5b22  reach:Optional["
+00013a30: 5374 6174 7352 6561 6368 225d 203d 204e  StatsReach"] = N
+00013a40: 6f6e 650a 0976 6973 6974 6f72 733a 4f70  one..visitors:Op
+00013a50: 7469 6f6e 616c 5b22 5374 6174 7356 6965  tional["StatsVie
+00013a60: 7773 225d 203d 204e 6f6e 650a 0a0a 636c  ws"] = None...cl
+00013a70: 6173 7320 5374 6174 7352 6561 6368 2842  ass StatsReach(B
+00013a80: 4d29 3a0a 0961 6765 3a4f 7074 696f 6e61  M):..age:Optiona
+00013a90: 6c5b 6c69 7374 5b22 5374 6174 7353 6578  l[list["StatsSex
+00013aa0: 4167 6522 5d5d 203d 204e 6f6e 650a 0963  Age"]] = None..c
+00013ab0: 6974 6965 733a 4f70 7469 6f6e 616c 5b6c  ities:Optional[l
+00013ac0: 6973 745b 2253 7461 7473 4369 7479 225d  ist["StatsCity"]
+00013ad0: 5d20 3d20 4e6f 6e65 0a09 636f 756e 7472  ] = None..countr
+00013ae0: 6965 733a 4f70 7469 6f6e 616c 5b6c 6973  ies:Optional[lis
+00013af0: 745b 2253 7461 7473 436f 756e 7472 7922  t["StatsCountry"
+00013b00: 5d5d 203d 204e 6f6e 650a 096d 6f62 696c  ]] = None..mobil
+00013b10: 655f 7265 6163 683a 4f70 7469 6f6e 616c  e_reach:Optional
+00013b20: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7265  [int] = None..re
+00013b30: 6163 683a 4f70 7469 6f6e 616c 5b69 6e74  ach:Optional[int
+00013b40: 5d20 3d20 4e6f 6e65 0a09 7265 6163 685f  ] = None..reach_
+00013b50: 7375 6273 6372 6962 6572 733a 4f70 7469  subscribers:Opti
+00013b60: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00013b70: 0a09 7365 783a 4f70 7469 6f6e 616c 5b6c  ..sex:Optional[l
+00013b80: 6973 745b 2253 7461 7473 5365 7841 6765  ist["StatsSexAge
+00013b90: 225d 5d20 3d20 4e6f 6e65 0a09 7365 785f  "]] = None..sex_
+00013ba0: 6167 653a 4f70 7469 6f6e 616c 5b6c 6973  age:Optional[lis
+00013bb0: 745b 2253 7461 7473 5365 7841 6765 225d  t["StatsSexAge"]
+00013bc0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+00013bd0: 2053 7461 7473 5365 7841 6765 2842 4d29   StatsSexAge(BM)
+00013be0: 3a0a 0963 6f75 6e74 3a4f 7074 696f 6e61  :..count:Optiona
+00013bf0: 6c5b 696e 745d 203d 204e 6f6e 650a 0976  l[int] = None..v
+00013c00: 616c 7565 3a73 7472 0a09 7265 6163 683a  alue:str..reach:
+00013c10: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00013c20: 4e6f 6e65 0a09 7265 6163 685f 7375 6273  None..reach_subs
+00013c30: 6372 6962 6572 733a 4f70 7469 6f6e 616c  cribers:Optional
+00013c40: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 636f  [int] = None..co
+00013c50: 756e 745f 7375 6273 6372 6962 6572 733a  unt_subscribers:
+00013c60: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00013c70: 4e6f 6e65 0a0a 0a63 6c61 7373 2053 7461  None...class Sta
+00013c80: 7473 5669 6577 7328 424d 293a 0a09 6167  tsViews(BM):..ag
+00013c90: 653a 4f70 7469 6f6e 616c 5b6c 6973 745b  e:Optional[list[
+00013ca0: 2253 7461 7473 5365 7841 6765 225d 5d20  "StatsSexAge"]] 
+00013cb0: 3d20 4e6f 6e65 0a09 6369 7469 6573 3a4f  = None..cities:O
+00013cc0: 7074 696f 6e61 6c5b 6c69 7374 5b22 5374  ptional[list["St
+00013cd0: 6174 7343 6974 7922 5d5d 203d 204e 6f6e  atsCity"]] = Non
+00013ce0: 650a 0963 6f75 6e74 7269 6573 3a4f 7074  e..countries:Opt
+00013cf0: 696f 6e61 6c5b 6c69 7374 5b22 5374 6174  ional[list["Stat
+00013d00: 7343 6f75 6e74 7279 225d 5d20 3d20 4e6f  sCountry"]] = No
+00013d10: 6e65 0a09 6d6f 6269 6c65 5f76 6965 7773  ne..mobile_views
+00013d20: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00013d30: 204e 6f6e 650a 0973 6578 3a4f 7074 696f   None..sex:Optio
+00013d40: 6e61 6c5b 6c69 7374 5b22 5374 6174 7353  nal[list["StatsS
+00013d50: 6578 4167 6522 5d5d 203d 204e 6f6e 650a  exAge"]] = None.
+00013d60: 0973 6578 5f61 6765 3a4f 7074 696f 6e61  .sex_age:Optiona
+00013d70: 6c5b 6c69 7374 5b22 5374 6174 7353 6578  l[list["StatsSex
+00013d80: 4167 6522 5d5d 203d 204e 6f6e 650a 0976  Age"]] = None..v
+00013d90: 6965 7773 3a4f 7074 696f 6e61 6c5b 696e  iews:Optional[in
+00013da0: 745d 203d 204e 6f6e 650a 0976 6973 6974  t] = None..visit
+00013db0: 6f72 733a 4f70 7469 6f6e 616c 5b69 6e74  ors:Optional[int
+00013dc0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+00013dd0: 2053 7461 7473 5761 6c6c 706f 7374 5374   StatsWallpostSt
+00013de0: 6174 2842 4d29 3a0a 0970 6f73 745f 6964  at(BM):..post_id
+00013df0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00013e00: 204e 6f6e 650a 0968 6964 653a 4f70 7469   None..hide:Opti
+00013e10: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00013e20: 0a09 6a6f 696e 5f67 726f 7570 3a4f 7074  ..join_group:Opt
+00013e30: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00013e40: 650a 096c 696e 6b73 3a4f 7074 696f 6e61  e..links:Optiona
+00013e50: 6c5b 696e 745d 203d 204e 6f6e 650a 0972  l[int] = None..r
+00013e60: 6561 6368 5f73 7562 7363 7269 6265 7273  each_subscribers
+00013e70: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00013e80: 204e 6f6e 650a 0972 6561 6368 5f73 7562   None..reach_sub
+00013e90: 7363 7269 6265 7273 5f63 6f75 6e74 3a4f  scribers_count:O
+00013ea0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00013eb0: 6f6e 650a 0972 6561 6368 5f74 6f74 616c  one..reach_total
+00013ec0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00013ed0: 204e 6f6e 650a 0972 6561 6368 5f74 6f74   None..reach_tot
+00013ee0: 616c 5f63 6f75 6e74 3a4f 7074 696f 6e61  al_count:Optiona
+00013ef0: 6c5b 696e 745d 203d 204e 6f6e 650a 0972  l[int] = None..r
+00013f00: 6561 6368 5f76 6972 616c 3a4f 7074 696f  each_viral:Optio
+00013f10: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00013f20: 0972 6561 6368 5f61 6473 3a4f 7074 696f  .reach_ads:Optio
+00013f30: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00013f40: 0972 6570 6f72 743a 4f70 7469 6f6e 616c  .report:Optional
+00013f50: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 746f  [int] = None..to
+00013f60: 5f67 726f 7570 3a4f 7074 696f 6e61 6c5b  _group:Optional[
+00013f70: 696e 745d 203d 204e 6f6e 650a 0975 6e73  int] = None..uns
+00013f80: 7562 7363 7269 6265 3a4f 7074 696f 6e61  ubscribe:Optiona
+00013f90: 6c5b 696e 745d 203d 204e 6f6e 650a 0973  l[int] = None..s
+00013fa0: 6578 5f61 6765 3a4f 7074 696f 6e61 6c5b  ex_age:Optional[
+00013fb0: 6c69 7374 5b22 5374 6174 7353 6578 4167  list["StatsSexAg
+00013fc0: 6522 5d5d 203d 204e 6f6e 650a 0a0a 0a0a  e"]] = None.....
+00013fd0: 636c 6173 7320 5374 6174 7573 5374 6174  class StatusStat
+00013fe0: 7573 2842 4d29 3a0a 0974 6578 743a 7374  us(BM):..text:st
+00013ff0: 720a 0961 7564 696f 3a4f 7074 696f 6e61  r..audio:Optiona
+00014000: 6c5b 2241 7564 696f 4175 6469 6f22 5d20  l["AudioAudio"] 
+00014010: 3d20 4e6f 6e65 0a0a 0a0a 0a63 6c61 7373  = None.....class
+00014020: 2053 7469 636b 6572 7349 6d61 6765 5365   StickersImageSe
+00014030: 7428 424d 293a 0a09 6261 7365 5f75 726c  t(BM):..base_url
+00014040: 3a73 7472 0a09 7665 7273 696f 6e3a 4f70  :str..version:Op
+00014050: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00014060: 6e65 0a0a 0a0a 0a63 6c61 7373 2053 746f  ne.....class Sto
+00014070: 7261 6765 5661 6c75 6528 424d 293a 0a09  rageValue(BM):..
+00014080: 6b65 793a 7374 720a 0976 616c 7565 3a73  key:str..value:s
+00014090: 7472 0a0a 0a0a 0a63 6c61 7373 2053 746f  tr.....class Sto
+000140a0: 7265 5072 6f64 7563 7428 424d 293a 0a09  reProduct(BM):..
+000140b0: 6964 3a69 6e74 0a09 7479 7065 3a73 7472  id:int..type:str
+000140c0: 0a09 6973 5f6e 6577 3a4f 7074 696f 6e61  ..is_new:Optiona
+000140d0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
+000140e0: 7075 7263 6861 7365 643a 4f70 7469 6f6e  purchased:Option
+000140f0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+00014100: 0961 6374 6976 653a 4f70 7469 6f6e 616c  .active:Optional
+00014110: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0970  [bool] = None..p
+00014120: 726f 6d6f 7465 643a 4f70 7469 6f6e 616c  romoted:Optional
+00014130: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0970  [bool] = None..p
+00014140: 7572 6368 6173 655f 6461 7465 3a4f 7074  urchase_date:Opt
+00014150: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00014160: 650a 0974 6974 6c65 3a4f 7074 696f 6e61  e..title:Optiona
+00014170: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
+00014180: 7469 636b 6572 733a 4f70 7469 6f6e 616c  tickers:Optional
+00014190: 5b22 4261 7365 5374 6963 6b65 7273 4c69  ["BaseStickersLi
+000141a0: 7374 225d 203d 204e 6f6e 650a 0973 7479  st"] = None..sty
+000141b0: 6c65 5f73 7469 636b 6572 5f69 6473 3a4f  le_sticker_ids:O
+000141c0: 7074 696f 6e61 6c5b 6c69 7374 5b69 6e74  ptional[list[int
+000141d0: 5d5d 203d 204e 6f6e 650a 0969 636f 6e3a  ]] = None..icon:
+000141e0: 4f70 7469 6f6e 616c 5b22 5374 6f72 6550  Optional["StoreP
+000141f0: 726f 6475 6374 4963 6f6e 225d 203d 204e  roductIcon"] = N
+00014200: 6f6e 650a 0970 7265 7669 6577 733a 4f70  one..previews:Op
+00014210: 7469 6f6e 616c 5b6c 6973 745b 2242 6173  tional[list["Bas
+00014220: 6549 6d61 6765 225d 5d20 3d20 4e6f 6e65  eImage"]] = None
+00014230: 0a09 6861 735f 616e 696d 6174 696f 6e3a  ..has_animation:
+00014240: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00014250: 204e 6f6e 650a 0973 7562 7469 746c 653a   None..subtitle:
+00014260: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00014270: 4e6f 6e65 0a09 7061 796d 656e 745f 7265  None..payment_re
+00014280: 6769 6f6e 3a4f 7074 696f 6e61 6c5b 7374  gion:Optional[st
+00014290: 725d 203d 204e 6f6e 650a 0a0a 636c 6173  r] = None...clas
+000142a0: 7320 5374 6f72 6550 726f 6475 6374 4963  s StoreProductIc
+000142b0: 6f6e 2842 4d29 3a0a 0970 6173 730a 0a63  on(BM):..pass..c
+000142c0: 6c61 7373 2053 746f 7265 5374 6963 6b65  lass StoreSticke
+000142d0: 7273 4b65 7977 6f72 6428 424d 293a 0a09  rsKeyword(BM):..
+000142e0: 776f 7264 733a 6c69 7374 5b73 7472 5d0a  words:list[str].
+000142f0: 0975 7365 725f 7374 6963 6b65 7273 3a4f  .user_stickers:O
+00014300: 7074 696f 6e61 6c5b 2253 746f 7265 5374  ptional["StoreSt
+00014310: 6963 6b65 7273 4b65 7977 6f72 6453 7469  ickersKeywordSti
+00014320: 636b 6572 7322 5d20 3d20 4e6f 6e65 0a09  ckers"] = None..
+00014330: 7072 6f6d 6f74 6564 5f73 7469 636b 6572  promoted_sticker
+00014340: 733a 4f70 7469 6f6e 616c 5b22 5374 6f72  s:Optional["Stor
+00014350: 6553 7469 636b 6572 734b 6579 776f 7264  eStickersKeyword
+00014360: 5374 6963 6b65 7273 225d 203d 204e 6f6e  Stickers"] = Non
+00014370: 650a 0973 7469 636b 6572 733a 4f70 7469  e..stickers:Opti
+00014380: 6f6e 616c 5b6c 6973 745b 2253 746f 7265  onal[list["Store
+00014390: 5374 6963 6b65 7273 4b65 7977 6f72 6453  StickersKeywordS
+000143a0: 7469 636b 6572 225d 5d20 3d20 4e6f 6e65  ticker"]] = None
+000143b0: 0a0a 0a63 6c61 7373 2053 746f 7265 5374  ...class StoreSt
+000143c0: 6963 6b65 7273 4b65 7977 6f72 6453 7469  ickersKeywordSti
+000143d0: 636b 6572 2842 4d29 3a0a 0970 6163 6b5f  cker(BM):..pack_
+000143e0: 6964 3a69 6e74 0a09 7374 6963 6b65 725f  id:int..sticker_
+000143f0: 6964 3a69 6e74 0a0a 0a63 6c61 7373 2053  id:int...class S
+00014400: 746f 7265 5374 6963 6b65 7273 4b65 7977  toreStickersKeyw
+00014410: 6f72 6453 7469 636b 6572 7328 424d 293a  ordStickers(BM):
+00014420: 0a09 7061 7373 0a0a 0a0a 636c 6173 7320  ..pass....class 
+00014430: 5374 6f72 6965 7353 746f 7279 5374 6174  StoriesStoryStat
+00014440: 7353 7461 7465 2845 6e75 6d29 3a0a 094f  sState(Enum):..O
+00014450: 4e20 3d20 226f 6e22 0a09 4f46 4620 3d20  N = "on"..OFF = 
+00014460: 226f 6666 220a 0948 4944 4445 4e20 3d20  "off"..HIDDEN = 
+00014470: 2268 6964 6465 6e22 0a0a 636c 6173 7320  "hidden"..class 
+00014480: 5374 6f72 6965 7353 746f 7279 5479 7065  StoriesStoryType
+00014490: 2845 6e75 6d29 3a0a 0950 484f 544f 203d  (Enum):..PHOTO =
+000144a0: 2022 7068 6f74 6f22 0a09 5649 4445 4f20   "photo"..VIDEO 
+000144b0: 3d20 2276 6964 656f 220a 094c 4956 455f  = "video"..LIVE_
+000144c0: 4143 5449 5645 203d 2022 6c69 7665 5f61  ACTIVE = "live_a
+000144d0: 6374 6976 6522 0a09 4c49 5645 5f46 494e  ctive"..LIVE_FIN
+000144e0: 4953 4845 4420 3d20 226c 6976 655f 6669  ISHED = "live_fi
+000144f0: 6e69 7368 6564 220a 0942 4952 5448 4441  nished"..BIRTHDA
+00014500: 595f 494e 5649 5445 203d 2022 6269 7274  Y_INVITE = "birt
+00014510: 6864 6179 5f69 6e76 6974 6522 0a0a 636c  hday_invite"..cl
+00014520: 6173 7320 5374 6f72 6965 7355 706c 6f61  ass StoriesUploa
+00014530: 644c 696e 6b54 6578 7428 456e 756d 293a  dLinkText(Enum):
+00014540: 0a09 544f 5f53 544f 5245 203d 2022 746f  ..TO_STORE = "to
+00014550: 5f73 746f 7265 220a 0956 4f54 4520 3d20  _store"..VOTE = 
+00014560: 2276 6f74 6522 0a09 4d4f 5245 203d 2022  "vote"..MORE = "
+00014570: 6d6f 7265 220a 0942 4f4f 4b20 3d20 2262  more"..BOOK = "b
+00014580: 6f6f 6b22 0a09 4f52 4445 5220 3d20 226f  ook"..ORDER = "o
+00014590: 7264 6572 220a 0945 4e52 4f4c 4c20 3d20  rder"..ENROLL = 
+000145a0: 2265 6e72 6f6c 6c22 0a09 4649 4c4c 203d  "enroll"..FILL =
+000145b0: 2022 6669 6c6c 220a 0953 4947 4e55 5020   "fill"..SIGNUP 
+000145c0: 3d20 2273 6967 6e75 7022 0a09 4255 5920  = "signup"..BUY 
+000145d0: 3d20 2262 7579 220a 0954 4943 4b45 5420  = "buy"..TICKET 
+000145e0: 3d20 2274 6963 6b65 7422 0a09 5752 4954  = "ticket"..WRIT
+000145f0: 4520 3d20 2277 7269 7465 220a 094f 5045  E = "write"..OPE
+00014600: 4e20 3d20 226f 7065 6e22 0a09 4c45 4152  N = "open"..LEAR
+00014610: 4e5f 4d4f 5245 203d 2022 6c65 6172 6e5f  N_MORE = "learn_
+00014620: 6d6f 7265 220a 0956 4945 5720 3d20 2276  more"..VIEW = "v
+00014630: 6965 7722 0a09 474f 5f54 4f20 3d20 2267  iew"..GO_TO = "g
+00014640: 6f5f 746f 220a 0943 4f4e 5441 4354 203d  o_to"..CONTACT =
+00014650: 2022 636f 6e74 6163 7422 0a09 5741 5443   "contact"..WATC
+00014660: 4820 3d20 2277 6174 6368 220a 0950 4c41  H = "watch"..PLA
+00014670: 5920 3d20 2270 6c61 7922 0a09 494e 5354  Y = "play"..INST
+00014680: 414c 4c20 3d20 2269 6e73 7461 6c6c 220a  ALL = "install".
+00014690: 0952 4541 4420 3d20 2272 6561 6422 0a09  .READ = "read"..
+000146a0: 4341 4c45 4e44 4152 203d 2022 6361 6c65  CALENDAR = "cale
+000146b0: 6e64 6172 220a 0a63 6c61 7373 2053 746f  ndar"..class Sto
+000146c0: 7269 6573 436c 6963 6b61 626c 6541 7265  riesClickableAre
+000146d0: 6128 424d 293a 0a09 783a 696e 740a 0979  a(BM):..x:int..y
+000146e0: 3a69 6e74 0a0a 0a63 6c61 7373 2053 746f  :int...class Sto
+000146f0: 7269 6573 436c 6963 6b61 626c 6553 7469  riesClickableSti
+00014700: 636b 6572 2842 4d29 3a0a 0963 6c69 636b  cker(BM):..click
+00014710: 6162 6c65 5f61 7265 613a 6c69 7374 5b22  able_area:list["
+00014720: 5374 6f72 6965 7343 6c69 636b 6162 6c65  StoriesClickable
+00014730: 4172 6561 225d 0a09 6964 3a69 6e74 0a09  Area"]..id:int..
+00014740: 6861 7368 7461 673a 4f70 7469 6f6e 616c  hashtag:Optional
+00014750: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6c69  [str] = None..li
+00014760: 6e6b 5f6f 626a 6563 743a 4f70 7469 6f6e  nk_object:Option
+00014770: 616c 5b22 4261 7365 4c69 6e6b 225d 203d  al["BaseLink"] =
+00014780: 204e 6f6e 650a 096d 656e 7469 6f6e 3a4f   None..mention:O
+00014790: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000147a0: 6f6e 650a 0974 6f6f 6c74 6970 5f74 6578  one..tooltip_tex
+000147b0: 743a 4f70 7469 6f6e 616c 5b73 7472 5d20  t:Optional[str] 
+000147c0: 3d20 4e6f 6e65 0a09 6f77 6e65 725f 6964  = None..owner_id
+000147d0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+000147e0: 204e 6f6e 650a 0973 746f 7279 5f69 643a   None..story_id:
+000147f0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00014800: 4e6f 6e65 0a09 7175 6573 7469 6f6e 3a4f  None..question:O
+00014810: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00014820: 6f6e 650a 0971 7565 7374 696f 6e5f 6275  one..question_bu
+00014830: 7474 6f6e 3a4f 7074 696f 6e61 6c5b 7374  tton:Optional[st
+00014840: 725d 203d 204e 6f6e 650a 0970 6c61 6365  r] = None..place
+00014850: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
+00014860: 5d20 3d20 4e6f 6e65 0a09 6d61 726b 6574  ] = None..market
+00014870: 5f69 7465 6d3a 4f70 7469 6f6e 616c 5b22  _item:Optional["
+00014880: 4d61 726b 6574 4d61 726b 6574 4974 656d  MarketMarketItem
+00014890: 225d 203d 204e 6f6e 650a 0961 7564 696f  "] = None..audio
+000148a0: 3a4f 7074 696f 6e61 6c5b 2241 7564 696f  :Optional["Audio
+000148b0: 4175 6469 6f22 5d20 3d20 4e6f 6e65 0a09  Audio"] = None..
+000148c0: 6175 6469 6f5f 7374 6172 745f 7469 6d65  audio_start_time
+000148d0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+000148e0: 204e 6f6e 650a 0973 7479 6c65 3a4f 7074   None..style:Opt
+000148f0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00014900: 650a 0974 7970 653a 7374 720a 0973 7562  e..type:str..sub
+00014910: 7479 7065 3a4f 7074 696f 6e61 6c5b 7374  type:Optional[st
+00014920: 725d 203d 204e 6f6e 650a 0970 6f73 745f  r] = None..post_
+00014930: 6f77 6e65 725f 6964 3a4f 7074 696f 6e61  owner_id:Optiona
+00014940: 6c5b 696e 745d 203d 204e 6f6e 650a 0970  l[int] = None..p
+00014950: 6f73 745f 6964 3a4f 7074 696f 6e61 6c5b  ost_id:Optional[
+00014960: 696e 745d 203d 204e 6f6e 650a 0970 6f6c  int] = None..pol
+00014970: 6c3a 4f70 7469 6f6e 616c 5b22 506f 6c6c  l:Optional["Poll
+00014980: 7350 6f6c 6c22 5d20 3d20 4e6f 6e65 0a09  sPoll"] = None..
+00014990: 636f 6c6f 723a 4f70 7469 6f6e 616c 5b73  color:Optional[s
+000149a0: 7472 5d20 3d20 4e6f 6e65 0a09 7374 6963  tr] = None..stic
+000149b0: 6b65 725f 6964 3a4f 7074 696f 6e61 6c5b  ker_id:Optional[
+000149c0: 696e 745d 203d 204e 6f6e 650a 0973 7469  int] = None..sti
+000149d0: 636b 6572 5f70 6163 6b5f 6964 3a4f 7074  cker_pack_id:Opt
+000149e0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000149f0: 650a 0961 7070 3a4f 7074 696f 6e61 6c5b  e..app:Optional[
+00014a00: 2241 7070 7341 7070 4d69 6e22 5d20 3d20  "AppsAppMin"] = 
+00014a10: 4e6f 6e65 0a09 6170 705f 636f 6e74 6578  None..app_contex
+00014a20: 743a 4f70 7469 6f6e 616c 5b73 7472 5d20  t:Optional[str] 
+00014a30: 3d20 4e6f 6e65 0a09 6861 735f 6e65 775f  = None..has_new_
+00014a40: 696e 7465 7261 6374 696f 6e73 3a4f 7074  interactions:Opt
+00014a50: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00014a60: 6e65 0a09 6973 5f62 726f 6164 6361 7374  ne..is_broadcast
+00014a70: 5f6e 6f74 6966 795f 616c 6c6f 7765 643a  _notify_allowed:
+00014a80: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00014a90: 204e 6f6e 650a 0973 6974 7561 7469 6f6e   None..situation
+00014aa0: 616c 5f74 6865 6d65 5f69 643a 4f70 7469  al_theme_id:Opti
+00014ab0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00014ac0: 0a09 7369 7475 6174 696f 6e61 6c5f 6170  ..situational_ap
+00014ad0: 705f 7572 6c3a 4f70 7469 6f6e 616c 5b73  p_url:Optional[s
+00014ae0: 7472 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  tr] = None...cla
+00014af0: 7373 2053 746f 7269 6573 436c 6963 6b61  ss StoriesClicka
+00014b00: 626c 6553 7469 636b 6572 7328 424d 293a  bleStickers(BM):
+00014b10: 0a09 636c 6963 6b61 626c 655f 7374 6963  ..clickable_stic
+00014b20: 6b65 7273 3a6c 6973 745b 2253 746f 7269  kers:list["Stori
+00014b30: 6573 436c 6963 6b61 626c 6553 7469 636b  esClickableStick
+00014b40: 6572 225d 0a09 6f72 6967 696e 616c 5f68  er"]..original_h
+00014b50: 6569 6768 743a 696e 740a 096f 7269 6769  eight:int..origi
+00014b60: 6e61 6c5f 7769 6474 683a 696e 740a 0a0a  nal_width:int...
+00014b70: 636c 6173 7320 5374 6f72 6965 7346 6565  class StoriesFee
+00014b80: 6449 7465 6d28 424d 293a 0a09 7479 7065  dItem(BM):..type
+00014b90: 3a73 7472 0a09 6964 3a4f 7074 696f 6e61  :str..id:Optiona
+00014ba0: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
+00014bb0: 746f 7269 6573 3a4f 7074 696f 6e61 6c5b  tories:Optional[
+00014bc0: 6c69 7374 5b22 5374 6f72 6965 7353 746f  list["StoriesSto
+00014bd0: 7279 225d 5d20 3d20 4e6f 6e65 0a09 6772  ry"]] = None..gr
+00014be0: 6f75 7065 643a 4f70 7469 6f6e 616c 5b6c  ouped:Optional[l
+00014bf0: 6973 745b 2253 746f 7269 6573 4665 6564  ist["StoriesFeed
+00014c00: 4974 656d 225d 5d20 3d20 4e6f 6e65 0a09  Item"]] = None..
+00014c10: 6170 703a 4f70 7469 6f6e 616c 5b22 4170  app:Optional["Ap
+00014c20: 7073 4170 704d 696e 225d 203d 204e 6f6e  psAppMin"] = Non
+00014c30: 650a 0970 726f 6d6f 5f64 6174 613a 4f70  e..promo_data:Op
+00014c40: 7469 6f6e 616c 5b22 5374 6f72 6965 7350  tional["StoriesP
+00014c50: 726f 6d6f 426c 6f63 6b22 5d20 3d20 4e6f  romoBlock"] = No
+00014c60: 6e65 0a09 6269 7274 6864 6179 5f75 7365  ne..birthday_use
+00014c70: 725f 6964 3a4f 7074 696f 6e61 6c5b 696e  r_id:Optional[in
+00014c80: 745d 203d 204e 6f6e 650a 0974 7261 636b  t] = None..track
+00014c90: 5f63 6f64 653a 4f70 7469 6f6e 616c 5b73  _code:Optional[s
+00014ca0: 7472 5d20 3d20 4e6f 6e65 0a09 6861 735f  tr] = None..has_
+00014cb0: 756e 7365 656e 3a4f 7074 696f 6e61 6c5b  unseen:Optional[
+00014cc0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6e61  bool] = None..na
+00014cd0: 6d65 3a4f 7074 696f 6e61 6c5b 7374 725d  me:Optional[str]
+00014ce0: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
+00014cf0: 5374 6f72 6965 7350 726f 6d6f 426c 6f63  StoriesPromoBloc
+00014d00: 6b28 424d 293a 0a09 6e61 6d65 3a73 7472  k(BM):..name:str
+00014d10: 0a09 7068 6f74 6f5f 3530 3a73 7472 0a09  ..photo_50:str..
+00014d20: 7068 6f74 6f5f 3130 303a 7374 720a 096e  photo_100:str..n
+00014d30: 6f74 5f61 6e69 6d61 7465 643a 626f 6f6c  ot_animated:bool
+00014d40: 0a0a 0a63 6c61 7373 2053 746f 7269 6573  ...class Stories
+00014d50: 5265 706c 6965 7328 424d 293a 0a09 636f  Replies(BM):..co
+00014d60: 756e 743a 696e 740a 096e 6577 3a4f 7074  unt:int..new:Opt
+00014d70: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00014d80: 650a 0a0a 636c 6173 7320 5374 6f72 6965  e...class Storie
+00014d90: 7353 7461 744c 696e 6528 424d 293a 0a09  sStatLine(BM):..
+00014da0: 6e61 6d65 3a73 7472 0a09 636f 756e 7465  name:str..counte
+00014db0: 723a 4f70 7469 6f6e 616c 5b69 6e74 5d20  r:Optional[int] 
+00014dc0: 3d20 4e6f 6e65 0a09 6973 5f75 6e61 7661  = None..is_unava
+00014dd0: 696c 6162 6c65 3a4f 7074 696f 6e61 6c5b  ilable:Optional[
+00014de0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 0a63  bool] = None...c
+00014df0: 6c61 7373 2053 746f 7269 6573 5374 6f72  lass StoriesStor
+00014e00: 7928 424d 293a 0a09 6163 6365 7373 5f6b  y(BM):..access_k
+00014e10: 6579 3a4f 7074 696f 6e61 6c5b 7374 725d  ey:Optional[str]
+00014e20: 203d 204e 6f6e 650a 0963 616e 5f63 6f6d   = None..can_com
+00014e30: 6d65 6e74 3a4f 7074 696f 6e61 6c5b 626f  ment:Optional[bo
+00014e40: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
+00014e50: 7265 706c 793a 4f70 7469 6f6e 616c 5b62  reply:Optional[b
+00014e60: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
+00014e70: 5f73 6565 3a4f 7074 696f 6e61 6c5b 626f  _see:Optional[bo
+00014e80: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
+00014e90: 6c69 6b65 3a4f 7074 696f 6e61 6c5b 626f  like:Optional[bo
+00014ea0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
+00014eb0: 7368 6172 653a 4f70 7469 6f6e 616c 5b62  share:Optional[b
+00014ec0: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
+00014ed0: 5f68 6964 653a 4f70 7469 6f6e 616c 5b62  _hide:Optional[b
+00014ee0: 6f6f 6c5d 203d 204e 6f6e 650a 0964 6174  ool] = None..dat
+00014ef0: 653a 4f70 7469 6f6e 616c 5b69 6e74 5d20  e:Optional[int] 
+00014f00: 3d20 4e6f 6e65 0a09 6578 7069 7265 735f  = None..expires_
+00014f10: 6174 3a4f 7074 696f 6e61 6c5b 696e 745d  at:Optional[int]
+00014f20: 203d 204e 6f6e 650a 0969 643a 696e 740a   = None..id:int.
+00014f30: 0969 735f 6465 6c65 7465 643a 4f70 7469  .is_deleted:Opti
+00014f40: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00014f50: 650a 0969 735f 6578 7069 7265 643a 4f70  e..is_expired:Op
+00014f60: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+00014f70: 6f6e 650a 096c 696e 6b3a 4f70 7469 6f6e  one..link:Option
+00014f80: 616c 5b22 5374 6f72 6965 7353 746f 7279  al["StoriesStory
+00014f90: 4c69 6e6b 225d 203d 204e 6f6e 650a 096f  Link"] = None..o
+00014fa0: 776e 6572 5f69 643a 696e 740a 0970 6172  wner_id:int..par
+00014fb0: 656e 745f 7374 6f72 793a 4f70 7469 6f6e  ent_story:Option
+00014fc0: 616c 5b22 5374 6f72 6965 7353 746f 7279  al["StoriesStory
+00014fd0: 225d 203d 204e 6f6e 650a 0970 6172 656e  "] = None..paren
+00014fe0: 745f 7374 6f72 795f 6163 6365 7373 5f6b  t_story_access_k
+00014ff0: 6579 3a4f 7074 696f 6e61 6c5b 7374 725d  ey:Optional[str]
+00015000: 203d 204e 6f6e 650a 0970 6172 656e 745f   = None..parent_
+00015010: 7374 6f72 795f 6964 3a4f 7074 696f 6e61  story_id:Optiona
+00015020: 6c5b 696e 745d 203d 204e 6f6e 650a 0970  l[int] = None..p
+00015030: 6172 656e 745f 7374 6f72 795f 6f77 6e65  arent_story_owne
+00015040: 725f 6964 3a4f 7074 696f 6e61 6c5b 696e  r_id:Optional[in
+00015050: 745d 203d 204e 6f6e 650a 0970 686f 746f  t] = None..photo
+00015060: 3a4f 7074 696f 6e61 6c5b 2250 686f 746f  :Optional["Photo
+00015070: 7350 686f 746f 225d 203d 204e 6f6e 650a  sPhoto"] = None.
+00015080: 0972 6570 6c69 6573 3a4f 7074 696f 6e61  .replies:Optiona
+00015090: 6c5b 2253 746f 7269 6573 5265 706c 6965  l["StoriesReplie
+000150a0: 7322 5d20 3d20 4e6f 6e65 0a09 7365 656e  s"] = None..seen
+000150b0: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+000150c0: 3d20 4e6f 6e65 0a09 7479 7065 3a4f 7074  = None..type:Opt
+000150d0: 696f 6e61 6c5b 2253 746f 7269 6573 5374  ional["StoriesSt
+000150e0: 6f72 7954 7970 6522 5d20 3d20 4e6f 6e65  oryType"] = None
+000150f0: 0a09 636c 6963 6b61 626c 655f 7374 6963  ..clickable_stic
+00015100: 6b65 7273 3a4f 7074 696f 6e61 6c5b 2253  kers:Optional["S
+00015110: 746f 7269 6573 436c 6963 6b61 626c 6553  toriesClickableS
+00015120: 7469 636b 6572 7322 5d20 3d20 4e6f 6e65  tickers"] = None
+00015130: 0a09 7669 6465 6f3a 4f70 7469 6f6e 616c  ..video:Optional
+00015140: 5b22 5669 6465 6f56 6964 656f 4675 6c6c  ["VideoVideoFull
+00015150: 225d 203d 204e 6f6e 650a 0976 6965 7773  "] = None..views
+00015160: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00015170: 204e 6f6e 650a 0963 616e 5f61 736b 3a4f   None..can_ask:O
+00015180: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00015190: 4e6f 6e65 0a09 6361 6e5f 6173 6b5f 616e  None..can_ask_an
+000151a0: 6f6e 796d 6f75 733a 4f70 7469 6f6e 616c  onymous:Optional
+000151b0: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 096e  [bool] = None..n
+000151c0: 6172 7261 7469 7665 735f 636f 756e 743a  arratives_count:
+000151d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000151e0: 4e6f 6e65 0a09 6669 7273 745f 6e61 7272  None..first_narr
+000151f0: 6174 6976 655f 7469 746c 653a 4f70 7469  ative_title:Opti
+00015200: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00015210: 0a09 6269 7274 6864 6179 5f77 6973 685f  ..birthday_wish_
+00015220: 7573 6572 5f69 643a 4f70 7469 6f6e 616c  user_id:Optional
+00015230: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6361  [int] = None..ca
+00015240: 6e5f 7573 655f 696e 5f6e 6172 7261 7469  n_use_in_narrati
+00015250: 7665 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ve:Optional[bool
+00015260: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+00015270: 2053 746f 7269 6573 5374 6f72 794c 696e   StoriesStoryLin
+00015280: 6b28 424d 293a 0a09 7465 7874 3a73 7472  k(BM):..text:str
+00015290: 0a09 7572 6c3a 7374 720a 096c 696e 6b5f  ..url:str..link_
+000152a0: 7572 6c5f 7461 7267 6574 3a4f 7074 696f  url_target:Optio
+000152b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000152c0: 0a0a 636c 6173 7320 5374 6f72 6965 7353  ..class StoriesS
+000152d0: 746f 7279 5374 6174 7328 424d 293a 0a09  toryStats(BM):..
+000152e0: 616e 7377 6572 3a22 5374 6f72 6965 7353  answer:"StoriesS
+000152f0: 746f 7279 5374 6174 7353 7461 7422 0a09  toryStatsStat"..
+00015300: 6261 6e73 3a22 5374 6f72 6965 7353 746f  bans:"StoriesSto
+00015310: 7279 5374 6174 7353 7461 7422 0a09 6f70  ryStatsStat"..op
+00015320: 656e 5f6c 696e 6b3a 2253 746f 7269 6573  en_link:"Stories
+00015330: 5374 6f72 7953 7461 7473 5374 6174 220a  StoryStatsStat".
+00015340: 0972 6570 6c69 6573 3a22 5374 6f72 6965  .replies:"Storie
+00015350: 7353 746f 7279 5374 6174 7353 7461 7422  sStoryStatsStat"
+00015360: 0a09 7368 6172 6573 3a22 5374 6f72 6965  ..shares:"Storie
+00015370: 7353 746f 7279 5374 6174 7353 7461 7422  sStoryStatsStat"
+00015380: 0a09 7375 6273 6372 6962 6572 733a 2253  ..subscribers:"S
+00015390: 746f 7269 6573 5374 6f72 7953 7461 7473  toriesStoryStats
+000153a0: 5374 6174 220a 0976 6965 7773 3a22 5374  Stat"..views:"St
+000153b0: 6f72 6965 7353 746f 7279 5374 6174 7353  oriesStoryStatsS
+000153c0: 7461 7422 0a09 6c69 6b65 733a 2253 746f  tat"..likes:"Sto
+000153d0: 7269 6573 5374 6f72 7953 7461 7473 5374  riesStoryStatsSt
+000153e0: 6174 220a 0a0a 636c 6173 7320 5374 6f72  at"...class Stor
+000153f0: 6965 7353 746f 7279 5374 6174 7353 7461  iesStoryStatsSta
+00015400: 7428 424d 293a 0a09 636f 756e 743a 4f70  t(BM):..count:Op
+00015410: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00015420: 6e65 0a09 7374 6174 653a 2253 746f 7269  ne..state:"Stori
+00015430: 6573 5374 6f72 7953 7461 7473 5374 6174  esStoryStatsStat
+00015440: 6522 0a0a 0a63 6c61 7373 2053 746f 7269  e"...class Stori
+00015450: 6573 5669 6577 6572 7349 7465 6d28 424d  esViewersItem(BM
+00015460: 293a 0a09 6973 5f6c 696b 6564 3a62 6f6f  ):..is_liked:boo
+00015470: 6c0a 0975 7365 725f 6964 3a69 6e74 0a09  l..user_id:int..
+00015480: 7573 6572 3a4f 7074 696f 6e61 6c5b 2255  user:Optional["U
+00015490: 7365 7273 5573 6572 4675 6c6c 225d 203d  sersUserFull"] =
+000154a0: 204e 6f6e 650a 0a0a 0a0a 636c 6173 7320   None.....class 
+000154b0: 5573 6572 7346 6965 6c64 7328 456e 756d  UsersFields(Enum
+000154c0: 293a 0a09 4649 5253 545f 4e41 4d45 5f4e  ):..FIRST_NAME_N
+000154d0: 4f4d 203d 2022 6669 7273 745f 6e61 6d65  OM = "first_name
+000154e0: 5f6e 6f6d 220a 0946 4952 5354 5f4e 414d  _nom"..FIRST_NAM
+000154f0: 455f 4745 4e20 3d20 2266 6972 7374 5f6e  E_GEN = "first_n
+00015500: 616d 655f 6765 6e22 0a09 4649 5253 545f  ame_gen"..FIRST_
+00015510: 4e41 4d45 5f44 4154 203d 2022 6669 7273  NAME_DAT = "firs
+00015520: 745f 6e61 6d65 5f64 6174 220a 0946 4952  t_name_dat"..FIR
+00015530: 5354 5f4e 414d 455f 4143 4320 3d20 2266  ST_NAME_ACC = "f
+00015540: 6972 7374 5f6e 616d 655f 6163 6322 0a09  irst_name_acc"..
+00015550: 4649 5253 545f 4e41 4d45 5f49 4e53 203d  FIRST_NAME_INS =
+00015560: 2022 6669 7273 745f 6e61 6d65 5f69 6e73   "first_name_ins
+00015570: 220a 0946 4952 5354 5f4e 414d 455f 4142  "..FIRST_NAME_AB
+00015580: 4c20 3d20 2266 6972 7374 5f6e 616d 655f  L = "first_name_
+00015590: 6162 6c22 0a09 4c41 5354 5f4e 414d 455f  abl"..LAST_NAME_
+000155a0: 4e4f 4d20 3d20 226c 6173 745f 6e61 6d65  NOM = "last_name
+000155b0: 5f6e 6f6d 220a 094c 4153 545f 4e41 4d45  _nom"..LAST_NAME
+000155c0: 5f47 454e 203d 2022 6c61 7374 5f6e 616d  _GEN = "last_nam
+000155d0: 655f 6765 6e22 0a09 4c41 5354 5f4e 414d  e_gen"..LAST_NAM
+000155e0: 455f 4441 5420 3d20 226c 6173 745f 6e61  E_DAT = "last_na
+000155f0: 6d65 5f64 6174 220a 094c 4153 545f 4e41  me_dat"..LAST_NA
+00015600: 4d45 5f41 4343 203d 2022 6c61 7374 5f6e  ME_ACC = "last_n
+00015610: 616d 655f 6163 6322 0a09 4c41 5354 5f4e  ame_acc"..LAST_N
+00015620: 414d 455f 494e 5320 3d20 226c 6173 745f  AME_INS = "last_
+00015630: 6e61 6d65 5f69 6e73 220a 094c 4153 545f  name_ins"..LAST_
+00015640: 4e41 4d45 5f41 424c 203d 2022 6c61 7374  NAME_ABL = "last
+00015650: 5f6e 616d 655f 6162 6c22 0a09 5048 4f54  _name_abl"..PHOT
+00015660: 4f5f 4944 203d 2022 7068 6f74 6f5f 6964  O_ID = "photo_id
+00015670: 220a 0956 4552 4946 4945 4420 3d20 2276  "..VERIFIED = "v
+00015680: 6572 6966 6965 6422 0a09 5345 5820 3d20  erified"..SEX = 
+00015690: 2273 6578 220a 0942 4441 5445 203d 2022  "sex"..BDATE = "
+000156a0: 6264 6174 6522 0a09 4244 4154 455f 5649  bdate"..BDATE_VI
+000156b0: 5349 4249 4c49 5459 203d 2022 6264 6174  SIBILITY = "bdat
+000156c0: 655f 7669 7369 6269 6c69 7479 220a 0943  e_visibility"..C
+000156d0: 4954 5920 3d20 2263 6974 7922 0a09 434f  ITY = "city"..CO
+000156e0: 554e 5452 5920 3d20 2263 6f75 6e74 7279  UNTRY = "country
+000156f0: 220a 0948 4f4d 455f 544f 574e 203d 2022  "..HOME_TOWN = "
+00015700: 686f 6d65 5f74 6f77 6e22 0a09 4841 535f  home_town"..HAS_
+00015710: 5048 4f54 4f20 3d20 2268 6173 5f70 686f  PHOTO = "has_pho
+00015720: 746f 220a 0950 484f 544f 203d 2022 7068  to"..PHOTO = "ph
+00015730: 6f74 6f22 0a09 5048 4f54 4f5f 5245 4320  oto"..PHOTO_REC 
+00015740: 3d20 2270 686f 746f 5f72 6563 220a 0950  = "photo_rec"..P
+00015750: 484f 544f 5f35 3020 3d20 2270 686f 746f  HOTO_50 = "photo
+00015760: 5f35 3022 0a09 5048 4f54 4f5f 3130 3020  _50"..PHOTO_100 
+00015770: 3d20 2270 686f 746f 5f31 3030 220a 0950  = "photo_100"..P
+00015780: 484f 544f 5f32 3030 5f4f 5249 4720 3d20  HOTO_200_ORIG = 
+00015790: 2270 686f 746f 5f32 3030 5f6f 7269 6722  "photo_200_orig"
+000157a0: 0a09 5048 4f54 4f5f 3230 3020 3d20 2270  ..PHOTO_200 = "p
+000157b0: 686f 746f 5f32 3030 220a 0950 484f 544f  hoto_200"..PHOTO
+000157c0: 5f34 3030 203d 2022 7068 6f74 6f5f 3430  _400 = "photo_40
+000157d0: 3022 0a09 5048 4f54 4f5f 3430 305f 4f52  0"..PHOTO_400_OR
+000157e0: 4947 203d 2022 7068 6f74 6f5f 3430 305f  IG = "photo_400_
+000157f0: 6f72 6967 220a 0950 484f 544f 5f42 4947  orig"..PHOTO_BIG
+00015800: 203d 2022 7068 6f74 6f5f 6269 6722 0a09   = "photo_big"..
+00015810: 5048 4f54 4f5f 4d45 4449 554d 203d 2022  PHOTO_MEDIUM = "
+00015820: 7068 6f74 6f5f 6d65 6469 756d 220a 0950  photo_medium"..P
+00015830: 484f 544f 5f4d 4544 4955 4d5f 5245 4320  HOTO_MEDIUM_REC 
+00015840: 3d20 2270 686f 746f 5f6d 6564 6975 6d5f  = "photo_medium_
+00015850: 7265 6322 0a09 5048 4f54 4f5f 4d41 5820  rec"..PHOTO_MAX 
+00015860: 3d20 2270 686f 746f 5f6d 6178 220a 0950  = "photo_max"..P
+00015870: 484f 544f 5f4d 4158 5f4f 5249 4720 3d20  HOTO_MAX_ORIG = 
+00015880: 2270 686f 746f 5f6d 6178 5f6f 7269 6722  "photo_max_orig"
+00015890: 0a09 5048 4f54 4f5f 4d41 585f 5349 5a45  ..PHOTO_MAX_SIZE
+000158a0: 203d 2022 7068 6f74 6f5f 6d61 785f 7369   = "photo_max_si
+000158b0: 7a65 220a 0954 4849 5244 5f50 4152 5459  ze"..THIRD_PARTY
+000158c0: 5f42 5554 544f 4e53 203d 2022 7468 6972  _BUTTONS = "thir
+000158d0: 645f 7061 7274 795f 6275 7474 6f6e 7322  d_party_buttons"
+000158e0: 0a09 4f4e 4c49 4e45 203d 2022 6f6e 6c69  ..ONLINE = "onli
+000158f0: 6e65 220a 094c 4953 5453 203d 2022 6c69  ne"..LISTS = "li
+00015900: 7374 7322 0a09 444f 4d41 494e 203d 2022  sts"..DOMAIN = "
+00015910: 646f 6d61 696e 220a 0948 4153 5f4d 4f42  domain"..HAS_MOB
+00015920: 494c 4520 3d20 2268 6173 5f6d 6f62 696c  ILE = "has_mobil
+00015930: 6522 0a09 434f 4e54 4143 5453 203d 2022  e"..CONTACTS = "
+00015940: 636f 6e74 6163 7473 220a 094c 414e 4755  contacts"..LANGU
+00015950: 4147 4520 3d20 226c 616e 6775 6167 6522  AGE = "language"
+00015960: 0a09 5349 5445 203d 2022 7369 7465 220a  ..SITE = "site".
+00015970: 0945 4455 4341 5449 4f4e 203d 2022 6564  .EDUCATION = "ed
+00015980: 7563 6174 696f 6e22 0a09 554e 4956 4552  ucation"..UNIVER
+00015990: 5349 5449 4553 203d 2022 756e 6976 6572  SITIES = "univer
+000159a0: 7369 7469 6573 220a 0953 4348 4f4f 4c53  sities"..SCHOOLS
+000159b0: 203d 2022 7363 686f 6f6c 7322 0a09 5354   = "schools"..ST
+000159c0: 4154 5553 203d 2022 7374 6174 7573 220a  ATUS = "status".
+000159d0: 094c 4153 545f 5345 454e 203d 2022 6c61  .LAST_SEEN = "la
+000159e0: 7374 5f73 6565 6e22 0a09 464f 4c4c 4f57  st_seen"..FOLLOW
+000159f0: 4552 535f 434f 554e 5420 3d20 2266 6f6c  ERS_COUNT = "fol
+00015a00: 6c6f 7765 7273 5f63 6f75 6e74 220a 0943  lowers_count"..C
+00015a10: 4f55 4e54 4552 5320 3d20 2263 6f75 6e74  OUNTERS = "count
+00015a20: 6572 7322 0a09 434f 4d4d 4f4e 5f43 4f55  ers"..COMMON_COU
+00015a30: 4e54 203d 2022 636f 6d6d 6f6e 5f63 6f75  NT = "common_cou
+00015a40: 6e74 220a 094f 4e4c 494e 455f 494e 464f  nt"..ONLINE_INFO
+00015a50: 203d 2022 6f6e 6c69 6e65 5f69 6e66 6f22   = "online_info"
+00015a60: 0a09 4f43 4355 5041 5449 4f4e 203d 2022  ..OCCUPATION = "
+00015a70: 6f63 6375 7061 7469 6f6e 220a 094e 4943  occupation"..NIC
+00015a80: 4b4e 414d 4520 3d20 226e 6963 6b6e 616d  KNAME = "nicknam
+00015a90: 6522 0a09 5245 4c41 5449 5645 5320 3d20  e"..RELATIVES = 
+00015aa0: 2272 656c 6174 6976 6573 220a 0952 454c  "relatives"..REL
+00015ab0: 4154 494f 4e20 3d20 2272 656c 6174 696f  ATION = "relatio
+00015ac0: 6e22 0a09 5045 5253 4f4e 414c 203d 2022  n"..PERSONAL = "
+00015ad0: 7065 7273 6f6e 616c 220a 0943 4f4e 4e45  personal"..CONNE
+00015ae0: 4354 494f 4e53 203d 2022 636f 6e6e 6563  CTIONS = "connec
+00015af0: 7469 6f6e 7322 0a09 4558 504f 5254 5320  tions"..EXPORTS 
+00015b00: 3d20 2265 7870 6f72 7473 220a 0957 414c  = "exports"..WAL
+00015b10: 4c5f 434f 4d4d 454e 5453 203d 2022 7761  L_COMMENTS = "wa
+00015b20: 6c6c 5f63 6f6d 6d65 6e74 7322 0a09 5741  ll_comments"..WA
+00015b30: 4c4c 5f44 4546 4155 4c54 203d 2022 7761  LL_DEFAULT = "wa
+00015b40: 6c6c 5f64 6566 6175 6c74 220a 0941 4354  ll_default"..ACT
+00015b50: 4956 4954 4945 5320 3d20 2261 6374 6976  IVITIES = "activ
+00015b60: 6974 6965 7322 0a09 4143 5449 5649 5459  ities"..ACTIVITY
+00015b70: 203d 2022 6163 7469 7669 7479 220a 0949   = "activity"..I
+00015b80: 4e54 4552 4553 5453 203d 2022 696e 7465  NTERESTS = "inte
+00015b90: 7265 7374 7322 0a09 4d55 5349 4320 3d20  rests"..MUSIC = 
+00015ba0: 226d 7573 6963 220a 094d 4f56 4945 5320  "music"..MOVIES 
+00015bb0: 3d20 226d 6f76 6965 7322 0a09 5456 203d  = "movies"..TV =
+00015bc0: 2022 7476 220a 0942 4f4f 4b53 203d 2022   "tv"..BOOKS = "
+00015bd0: 626f 6f6b 7322 0a09 4953 5f4e 4f5f 494e  books"..IS_NO_IN
+00015be0: 4445 5820 3d20 2269 735f 6e6f 5f69 6e64  DEX = "is_no_ind
+00015bf0: 6578 220a 0947 414d 4553 203d 2022 6761  ex"..GAMES = "ga
+00015c00: 6d65 7322 0a09 4142 4f55 5420 3d20 2261  mes"..ABOUT = "a
+00015c10: 626f 7574 220a 0951 554f 5445 5320 3d20  bout"..QUOTES = 
+00015c20: 2271 756f 7465 7322 0a09 4341 4e5f 504f  "quotes"..CAN_PO
+00015c30: 5354 203d 2022 6361 6e5f 706f 7374 220a  ST = "can_post".
+00015c40: 0943 414e 5f53 4545 5f41 4c4c 5f50 4f53  .CAN_SEE_ALL_POS
+00015c50: 5453 203d 2022 6361 6e5f 7365 655f 616c  TS = "can_see_al
+00015c60: 6c5f 706f 7374 7322 0a09 4341 4e5f 5345  l_posts"..CAN_SE
+00015c70: 455f 4155 4449 4f20 3d20 2263 616e 5f73  E_AUDIO = "can_s
+00015c80: 6565 5f61 7564 696f 220a 0943 414e 5f53  ee_audio"..CAN_S
+00015c90: 4545 5f47 4946 5453 203d 2022 6361 6e5f  EE_GIFTS = "can_
+00015ca0: 7365 655f 6769 6674 7322 0a09 574f 524b  see_gifts"..WORK
+00015cb0: 203d 2022 776f 726b 220a 0950 4c41 4345   = "work"..PLACE
+00015cc0: 5320 3d20 2270 6c61 6365 7322 0a09 4341  S = "places"..CA
+00015cd0: 4e5f 5752 4954 455f 5052 4956 4154 455f  N_WRITE_PRIVATE_
+00015ce0: 4d45 5353 4147 4520 3d20 2263 616e 5f77  MESSAGE = "can_w
+00015cf0: 7269 7465 5f70 7269 7661 7465 5f6d 6573  rite_private_mes
+00015d00: 7361 6765 220a 0943 414e 5f53 454e 445f  sage"..CAN_SEND_
+00015d10: 4652 4945 4e44 5f52 4551 5545 5354 203d  FRIEND_REQUEST =
+00015d20: 2022 6361 6e5f 7365 6e64 5f66 7269 656e   "can_send_frien
+00015d30: 645f 7265 7175 6573 7422 0a09 4341 4e5f  d_request"..CAN_
+00015d40: 5550 4c4f 4144 5f44 4f43 203d 2022 6361  UPLOAD_DOC = "ca
+00015d50: 6e5f 7570 6c6f 6164 5f64 6f63 220a 0949  n_upload_doc"..I
+00015d60: 535f 4641 564f 5249 5445 203d 2022 6973  S_FAVORITE = "is
+00015d70: 5f66 6176 6f72 6974 6522 0a09 4953 5f48  _favorite"..IS_H
+00015d80: 4944 4445 4e5f 4652 4f4d 5f46 4545 4420  IDDEN_FROM_FEED 
+00015d90: 3d20 2269 735f 6869 6464 656e 5f66 726f  = "is_hidden_fro
+00015da0: 6d5f 6665 6564 220a 0954 494d 455a 4f4e  m_feed"..TIMEZON
+00015db0: 4520 3d20 2274 696d 657a 6f6e 6522 0a09  E = "timezone"..
+00015dc0: 5343 5245 454e 5f4e 414d 4520 3d20 2273  SCREEN_NAME = "s
+00015dd0: 6372 6565 6e5f 6e61 6d65 220a 094d 4149  creen_name"..MAI
+00015de0: 4445 4e5f 4e41 4d45 203d 2022 6d61 6964  DEN_NAME = "maid
+00015df0: 656e 5f6e 616d 6522 0a09 4352 4f50 5f50  en_name"..CROP_P
+00015e00: 484f 544f 203d 2022 6372 6f70 5f70 686f  HOTO = "crop_pho
+00015e10: 746f 220a 0949 535f 4652 4945 4e44 203d  to"..IS_FRIEND =
+00015e20: 2022 6973 5f66 7269 656e 6422 0a09 4652   "is_friend"..FR
+00015e30: 4945 4e44 5f53 5441 5455 5320 3d20 2266  IEND_STATUS = "f
+00015e40: 7269 656e 645f 7374 6174 7573 220a 0943  riend_status"..C
+00015e50: 4152 4545 5220 3d20 2263 6172 6565 7222  AREER = "career"
+00015e60: 0a09 4d49 4c49 5441 5259 203d 2022 6d69  ..MILITARY = "mi
+00015e70: 6c69 7461 7279 220a 0942 4c41 434b 4c49  litary"..BLACKLI
+00015e80: 5354 4544 203d 2022 626c 6163 6b6c 6973  STED = "blacklis
+00015e90: 7465 6422 0a09 424c 4143 4b4c 4953 5445  ted"..BLACKLISTE
+00015ea0: 445f 4259 5f4d 4520 3d20 2262 6c61 636b  D_BY_ME = "black
+00015eb0: 6c69 7374 6564 5f62 795f 6d65 220a 0943  listed_by_me"..C
+00015ec0: 414e 5f53 5542 5343 5249 4245 5f50 4f53  AN_SUBSCRIBE_POS
+00015ed0: 5453 203d 2022 6361 6e5f 7375 6273 6372  TS = "can_subscr
+00015ee0: 6962 655f 706f 7374 7322 0a09 4445 5343  ibe_posts"..DESC
+00015ef0: 5249 5054 494f 4e53 203d 2022 6465 7363  RIPTIONS = "desc
+00015f00: 7269 7074 696f 6e73 220a 0954 5245 4e44  riptions"..TREND
+00015f10: 494e 4720 3d20 2274 7265 6e64 696e 6722  ING = "trending"
+00015f20: 0a09 4d55 5455 414c 203d 2022 6d75 7475  ..MUTUAL = "mutu
+00015f30: 616c 220a 0946 5249 454e 4453 4849 505f  al"..FRIENDSHIP_
+00015f40: 5745 454b 5320 3d20 2266 7269 656e 6473  WEEKS = "friends
+00015f50: 6869 705f 7765 656b 7322 0a09 4341 4e5f  hip_weeks"..CAN_
+00015f60: 494e 5649 5445 5f54 4f5f 4348 4154 5320  INVITE_TO_CHATS 
+00015f70: 3d20 2263 616e 5f69 6e76 6974 655f 746f  = "can_invite_to
+00015f80: 5f63 6861 7473 220a 0953 544f 5249 4553  _chats"..STORIES
+00015f90: 5f41 5243 4849 5645 5f43 4f55 4e54 203d  _ARCHIVE_COUNT =
+00015fa0: 2022 7374 6f72 6965 735f 6172 6368 6976   "stories_archiv
+00015fb0: 655f 636f 756e 7422 0a09 4841 535f 554e  e_count"..HAS_UN
+00015fc0: 5345 454e 5f53 544f 5249 4553 203d 2022  SEEN_STORIES = "
+00015fd0: 6861 735f 756e 7365 656e 5f73 746f 7269  has_unseen_stori
+00015fe0: 6573 220a 0956 4944 454f 5f4c 4956 4520  es"..VIDEO_LIVE 
+00015ff0: 3d20 2276 6964 656f 5f6c 6976 6522 0a09  = "video_live"..
+00016000: 5649 4445 4f5f 4c49 5645 5f4c 4556 454c  VIDEO_LIVE_LEVEL
+00016010: 203d 2022 7669 6465 6f5f 6c69 7665 5f6c   = "video_live_l
+00016020: 6576 656c 220a 0956 4944 454f 5f4c 4956  evel"..VIDEO_LIV
+00016030: 455f 434f 554e 5420 3d20 2276 6964 656f  E_COUNT = "video
+00016040: 5f6c 6976 655f 636f 756e 7422 0a09 434c  _live_count"..CL
+00016050: 4950 535f 434f 554e 5420 3d20 2263 6c69  IPS_COUNT = "cli
+00016060: 7073 5f63 6f75 6e74 220a 0953 4552 5649  ps_count"..SERVI
+00016070: 4345 5f44 4553 4352 4950 5449 4f4e 203d  CE_DESCRIPTION =
+00016080: 2022 7365 7276 6963 655f 6465 7363 7269   "service_descri
+00016090: 7074 696f 6e22 0a09 4341 4e5f 5345 455f  ption"..CAN_SEE_
+000160a0: 5749 5348 4553 203d 2022 6361 6e5f 7365  WISHES = "can_se
+000160b0: 655f 7769 7368 6573 220a 0949 535f 5355  e_wishes"..IS_SU
+000160c0: 4253 4352 4942 4544 5f50 4f44 4341 5354  BSCRIBED_PODCAST
+000160d0: 5320 3d20 2269 735f 7375 6273 6372 6962  S = "is_subscrib
+000160e0: 6564 5f70 6f64 6361 7374 7322 0a09 4341  ed_podcasts"..CA
+000160f0: 4e5f 5355 4253 4352 4942 455f 504f 4443  N_SUBSCRIBE_PODC
+00016100: 4153 5453 203d 2022 6361 6e5f 7375 6273  ASTS = "can_subs
+00016110: 6372 6962 655f 706f 6463 6173 7473 220a  cribe_podcasts".
+00016120: 0a63 6c61 7373 2055 7365 7273 5573 6572  .class UsersUser
+00016130: 5265 6c61 7469 6f6e 2845 6e75 6d29 3a0a  Relation(Enum):.
+00016140: 094e 4f54 5f53 5045 4349 4649 4544 203d  .NOT_SPECIFIED =
+00016150: 2030 0a09 5349 4e47 4c45 203d 2031 0a09   0..SINGLE = 1..
+00016160: 494e 5f41 5f52 454c 4154 494f 4e53 4849  IN_A_RELATIONSHI
+00016170: 5020 3d20 320a 0945 4e47 4147 4544 203d  P = 2..ENGAGED =
+00016180: 2033 0a09 4d41 5252 4945 4420 3d20 340a   3..MARRIED = 4.
+00016190: 0943 4f4d 504c 4943 4154 4544 203d 2035  .COMPLICATED = 5
+000161a0: 0a09 4143 5449 5645 4c59 5f53 4541 5243  ..ACTIVELY_SEARC
+000161b0: 4849 4e47 203d 2036 0a09 494e 5f4c 4f56  HING = 6..IN_LOV
+000161c0: 4520 3d20 370a 0949 4e5f 415f 4349 5649  E = 7..IN_A_CIVI
+000161d0: 4c5f 554e 494f 4e20 3d20 380a 0a63 6c61  L_UNION = 8..cla
+000161e0: 7373 2055 7365 7273 5573 6572 5479 7065  ss UsersUserType
+000161f0: 2845 6e75 6d29 3a0a 0950 524f 4649 4c45  (Enum):..PROFILE
+00016200: 203d 2022 7072 6f66 696c 6522 0a0a 636c   = "profile"..cl
+00016210: 6173 7320 5573 6572 7343 6172 6565 7228  ass UsersCareer(
+00016220: 424d 293a 0a09 6369 7479 5f69 643a 4f70  BM):..city_id:Op
+00016230: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00016240: 6e65 0a09 6369 7479 5f6e 616d 653a 4f70  ne..city_name:Op
+00016250: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00016260: 6e65 0a09 636f 6d70 616e 793a 4f70 7469  ne..company:Opti
+00016270: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00016280: 0a09 636f 756e 7472 795f 6964 3a4f 7074  ..country_id:Opt
+00016290: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+000162a0: 650a 095f 6672 6f6d 3a4f 7074 696f 6e61  e.._from:Optiona
+000162b0: 6c5b 696e 745d 203d 204e 6f6e 650a 0967  l[int] = None..g
+000162c0: 726f 7570 5f69 643a 4f70 7469 6f6e 616c  roup_id:Optional
+000162d0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6964  [int] = None..id
+000162e0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+000162f0: 204e 6f6e 650a 0970 6f73 6974 696f 6e3a   None..position:
+00016300: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00016310: 4e6f 6e65 0a09 756e 7469 6c3a 4f70 7469  None..until:Opti
+00016320: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00016330: 0a0a 0a63 6c61 7373 2055 7365 7273 4578  ...class UsersEx
+00016340: 706f 7274 7328 424d 293a 0a09 6661 6365  ports(BM):..face
+00016350: 626f 6f6b 3a4f 7074 696f 6e61 6c5b 696e  book:Optional[in
+00016360: 745d 203d 204e 6f6e 650a 096c 6976 656a  t] = None..livej
+00016370: 6f75 726e 616c 3a4f 7074 696f 6e61 6c5b  ournal:Optional[
+00016380: 696e 745d 203d 204e 6f6e 650a 0974 7769  int] = None..twi
+00016390: 7474 6572 3a4f 7074 696f 6e61 6c5b 696e  tter:Optional[in
+000163a0: 745d 203d 204e 6f6e 650a 0a0a 636c 6173  t] = None...clas
+000163b0: 7320 5573 6572 734c 6173 7453 6565 6e28  s UsersLastSeen(
+000163c0: 424d 293a 0a09 706c 6174 666f 726d 3a4f  BM):..platform:O
+000163d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000163e0: 6f6e 650a 0974 696d 653a 4f70 7469 6f6e  one..time:Option
+000163f0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a  al[int] = None..
+00016400: 0a63 6c61 7373 2055 7365 7273 4d69 6c69  .class UsersMili
+00016410: 7461 7279 2842 4d29 3a0a 0963 6f75 6e74  tary(BM):..count
+00016420: 7279 5f69 643a 696e 740a 095f 6672 6f6d  ry_id:int.._from
+00016430: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00016440: 204e 6f6e 650a 0969 643a 4f70 7469 6f6e   None..id:Option
+00016450: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00016460: 756e 6974 3a73 7472 0a09 756e 6974 5f69  unit:str..unit_i
+00016470: 643a 696e 740a 0975 6e74 696c 3a4f 7074  d:int..until:Opt
+00016480: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00016490: 650a 0a0a 636c 6173 7320 5573 6572 734f  e...class UsersO
+000164a0: 6363 7570 6174 696f 6e28 424d 293a 0a09  ccupation(BM):..
+000164b0: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
+000164c0: 203d 204e 6f6e 650a 096e 616d 653a 4f70   = None..name:Op
+000164d0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+000164e0: 6e65 0a09 7479 7065 3a4f 7074 696f 6e61  ne..type:Optiona
+000164f0: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
+00016500: 636c 6173 7320 5573 6572 734f 6e6c 696e  class UsersOnlin
+00016510: 6549 6e66 6f28 424d 293a 0a09 7669 7369  eInfo(BM):..visi
+00016520: 626c 653a 626f 6f6c 0a09 6c61 7374 5f73  ble:bool..last_s
+00016530: 6565 6e3a 4f70 7469 6f6e 616c 5b69 6e74  een:Optional[int
+00016540: 5d20 3d20 4e6f 6e65 0a09 6973 5f6f 6e6c  ] = None..is_onl
+00016550: 696e 653a 4f70 7469 6f6e 616c 5b62 6f6f  ine:Optional[boo
+00016560: 6c5d 203d 204e 6f6e 650a 0961 7070 5f69  l] = None..app_i
+00016570: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+00016580: 3d20 4e6f 6e65 0a09 6973 5f6d 6f62 696c  = None..is_mobil
+00016590: 653a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  e:Optional[bool]
+000165a0: 203d 204e 6f6e 650a 0973 7461 7475 733a   = None..status:
+000165b0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000165c0: 4e6f 6e65 0a0a 0a63 6c61 7373 2055 7365  None...class Use
+000165d0: 7273 5065 7273 6f6e 616c 2842 4d29 3a0a  rsPersonal(BM):.
+000165e0: 0961 6c63 6f68 6f6c 3a4f 7074 696f 6e61  .alcohol:Optiona
+000165f0: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
+00016600: 6e73 7069 7265 645f 6279 3a4f 7074 696f  nspired_by:Optio
+00016610: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00016620: 096c 616e 6773 3a4f 7074 696f 6e61 6c5b  .langs:Optional[
+00016630: 6c69 7374 5b73 7472 5d5d 203d 204e 6f6e  list[str]] = Non
+00016640: 650a 096c 6966 655f 6d61 696e 3a4f 7074  e..life_main:Opt
+00016650: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00016660: 650a 0970 656f 706c 655f 6d61 696e 3a4f  e..people_main:O
+00016670: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00016680: 6f6e 650a 0970 6f6c 6974 6963 616c 3a4f  one..political:O
+00016690: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000166a0: 6f6e 650a 0972 656c 6967 696f 6e3a 4f70  one..religion:Op
+000166b0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+000166c0: 6e65 0a09 7265 6c69 6769 6f6e 5f69 643a  ne..religion_id:
+000166d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000166e0: 4e6f 6e65 0a09 736d 6f6b 696e 673a 4f70  None..smoking:Op
+000166f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00016700: 6e65 0a0a 0a63 6c61 7373 2055 7365 7273  ne...class Users
+00016710: 5265 6c61 7469 7665 2842 4d29 3a0a 0962  Relative(BM):..b
+00016720: 6972 7468 5f64 6174 653a 4f70 7469 6f6e  irth_date:Option
+00016730: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00016740: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
+00016750: 203d 204e 6f6e 650a 096e 616d 653a 4f70   = None..name:Op
+00016760: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00016770: 6e65 0a09 7479 7065 3a73 7472 0a0a 0a63  ne..type:str...c
+00016780: 6c61 7373 2055 7365 7273 5363 686f 6f6c  lass UsersSchool
+00016790: 2842 4d29 3a0a 0963 6974 793a 4f70 7469  (BM):..city:Opti
+000167a0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+000167b0: 0a09 5f63 6c61 7373 3a4f 7074 696f 6e61  .._class:Optiona
+000167c0: 6c5b 7374 725d 203d 204e 6f6e 650a 0963  l[str] = None..c
+000167d0: 6f75 6e74 7279 3a4f 7074 696f 6e61 6c5b  ountry:Optional[
+000167e0: 696e 745d 203d 204e 6f6e 650a 0969 643a  int] = None..id:
+000167f0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00016800: 4e6f 6e65 0a09 6e61 6d65 3a4f 7074 696f  None..name:Optio
+00016810: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00016820: 0974 7970 653a 4f70 7469 6f6e 616c 5b69  .type:Optional[i
+00016830: 6e74 5d20 3d20 4e6f 6e65 0a09 7479 7065  nt] = None..type
+00016840: 5f73 7472 3a4f 7074 696f 6e61 6c5b 7374  _str:Optional[st
+00016850: 725d 203d 204e 6f6e 650a 0979 6561 725f  r] = None..year_
+00016860: 6672 6f6d 3a4f 7074 696f 6e61 6c5b 696e  from:Optional[in
+00016870: 745d 203d 204e 6f6e 650a 0979 6561 725f  t] = None..year_
+00016880: 6772 6164 7561 7465 643a 4f70 7469 6f6e  graduated:Option
+00016890: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+000168a0: 7965 6172 5f74 6f3a 4f70 7469 6f6e 616c  year_to:Optional
+000168b0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7370  [int] = None..sp
+000168c0: 6563 6961 6c69 7479 3a4f 7074 696f 6e61  eciality:Optiona
+000168d0: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
+000168e0: 636c 6173 7320 5573 6572 7353 7562 7363  class UsersSubsc
+000168f0: 7269 7074 696f 6e73 4974 656d 2842 4d29  riptionsItem(BM)
+00016900: 3a0a 0970 6173 730a 0a63 6c61 7373 2055  :..pass..class U
+00016910: 7365 7273 556e 6976 6572 7369 7479 2842  sersUniversity(B
+00016920: 4d29 3a0a 0963 6861 6972 3a4f 7074 696f  M):..chair:Optio
+00016930: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00016940: 0963 6861 6972 5f6e 616d 653a 4f70 7469  .chair_name:Opti
+00016950: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00016960: 0a09 6369 7479 3a4f 7074 696f 6e61 6c5b  ..city:Optional[
+00016970: 696e 745d 203d 204e 6f6e 650a 0963 6f75  int] = None..cou
+00016980: 6e74 7279 3a4f 7074 696f 6e61 6c5b 696e  ntry:Optional[in
+00016990: 745d 203d 204e 6f6e 650a 0965 6475 6361  t] = None..educa
+000169a0: 7469 6f6e 5f66 6f72 6d3a 4f70 7469 6f6e  tion_form:Option
+000169b0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+000169c0: 6564 7563 6174 696f 6e5f 7374 6174 7573  education_status
+000169d0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+000169e0: 204e 6f6e 650a 0966 6163 756c 7479 3a4f   None..faculty:O
+000169f0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00016a00: 6f6e 650a 0966 6163 756c 7479 5f6e 616d  one..faculty_nam
+00016a10: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
+00016a20: 3d20 4e6f 6e65 0a09 6772 6164 7561 7469  = None..graduati
+00016a30: 6f6e 3a4f 7074 696f 6e61 6c5b 696e 745d  on:Optional[int]
+00016a40: 203d 204e 6f6e 650a 0969 643a 4f70 7469   = None..id:Opti
+00016a50: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00016a60: 0a09 6e61 6d65 3a4f 7074 696f 6e61 6c5b  ..name:Optional[
+00016a70: 7374 725d 203d 204e 6f6e 650a 0975 6e69  str] = None..uni
+00016a80: 7665 7273 6974 795f 6772 6f75 705f 6964  versity_group_id
+00016a90: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00016aa0: 204e 6f6e 650a 0a0a 636c 6173 7320 5573   None...class Us
+00016ab0: 6572 7355 7365 7243 6f6e 6e65 6374 696f  ersUserConnectio
+00016ac0: 6e73 2842 4d29 3a0a 0973 6b79 7065 3a73  ns(BM):..skype:s
+00016ad0: 7472 0a09 6661 6365 626f 6f6b 3a73 7472  tr..facebook:str
+00016ae0: 0a09 6661 6365 626f 6f6b 5f6e 616d 653a  ..facebook_name:
+00016af0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00016b00: 4e6f 6e65 0a09 7477 6974 7465 723a 7374  None..twitter:st
+00016b10: 720a 096c 6976 656a 6f75 726e 616c 3a4f  r..livejournal:O
+00016b20: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00016b30: 6f6e 650a 0969 6e73 7461 6772 616d 3a73  one..instagram:s
+00016b40: 7472 0a0a 0a63 6c61 7373 2055 7365 7273  tr...class Users
+00016b50: 5573 6572 436f 756e 7465 7273 2842 4d29  UserCounters(BM)
+00016b60: 3a0a 0961 6c62 756d 733a 4f70 7469 6f6e  :..albums:Option
+00016b70: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00016b80: 6261 6467 6573 3a4f 7074 696f 6e61 6c5b  badges:Optional[
+00016b90: 696e 745d 203d 204e 6f6e 650a 0961 7564  int] = None..aud
+00016ba0: 696f 733a 4f70 7469 6f6e 616c 5b69 6e74  ios:Optional[int
+00016bb0: 5d20 3d20 4e6f 6e65 0a09 666f 6c6c 6f77  ] = None..follow
+00016bc0: 6572 733a 4f70 7469 6f6e 616c 5b69 6e74  ers:Optional[int
+00016bd0: 5d20 3d20 4e6f 6e65 0a09 6672 6965 6e64  ] = None..friend
+00016be0: 733a 4f70 7469 6f6e 616c 5b69 6e74 5d20  s:Optional[int] 
+00016bf0: 3d20 4e6f 6e65 0a09 6769 6674 733a 4f70  = None..gifts:Op
+00016c00: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00016c10: 6e65 0a09 6772 6f75 7073 3a4f 7074 696f  ne..groups:Optio
+00016c20: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00016c30: 096e 6f74 6573 3a4f 7074 696f 6e61 6c5b  .notes:Optional[
+00016c40: 696e 745d 203d 204e 6f6e 650a 096f 6e6c  int] = None..onl
+00016c50: 696e 655f 6672 6965 6e64 733a 4f70 7469  ine_friends:Opti
+00016c60: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00016c70: 0a09 7061 6765 733a 4f70 7469 6f6e 616c  ..pages:Optional
+00016c80: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7068  [int] = None..ph
+00016c90: 6f74 6f73 3a4f 7074 696f 6e61 6c5b 696e  otos:Optional[in
+00016ca0: 745d 203d 204e 6f6e 650a 0973 7562 7363  t] = None..subsc
+00016cb0: 7269 7074 696f 6e73 3a4f 7074 696f 6e61  riptions:Optiona
+00016cc0: 6c5b 696e 745d 203d 204e 6f6e 650a 0975  l[int] = None..u
+00016cd0: 7365 725f 7068 6f74 6f73 3a4f 7074 696f  ser_photos:Optio
+00016ce0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00016cf0: 0975 7365 725f 7669 6465 6f73 3a4f 7074  .user_videos:Opt
+00016d00: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00016d10: 650a 0976 6964 656f 733a 4f70 7469 6f6e  e..videos:Option
+00016d20: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00016d30: 6e65 775f 7068 6f74 6f5f 7461 6773 3a4f  new_photo_tags:O
+00016d40: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00016d50: 6f6e 650a 096e 6577 5f72 6563 6f67 6e69  one..new_recogni
+00016d60: 7469 6f6e 5f74 6167 733a 4f70 7469 6f6e  tion_tags:Option
+00016d70: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00016d80: 6d75 7475 616c 5f66 7269 656e 6473 3a4f  mutual_friends:O
+00016d90: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00016da0: 6f6e 650a 0970 6f73 7473 3a4f 7074 696f  one..posts:Optio
+00016db0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00016dc0: 0961 7274 6963 6c65 733a 4f70 7469 6f6e  .articles:Option
+00016dd0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00016de0: 7769 7368 6573 3a4f 7074 696f 6e61 6c5b  wishes:Optional[
+00016df0: 696e 745d 203d 204e 6f6e 650a 0970 6f64  int] = None..pod
+00016e00: 6361 7374 733a 4f70 7469 6f6e 616c 5b69  casts:Optional[i
+00016e10: 6e74 5d20 3d20 4e6f 6e65 0a09 636c 6970  nt] = None..clip
+00016e20: 733a 4f70 7469 6f6e 616c 5b69 6e74 5d20  s:Optional[int] 
+00016e30: 3d20 4e6f 6e65 0a09 636c 6970 735f 666f  = None..clips_fo
+00016e40: 6c6c 6f77 6572 733a 4f70 7469 6f6e 616c  llowers:Optional
+00016e50: 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63  [int] = None...c
+00016e60: 6c61 7373 2055 7365 7273 5573 6572 4d69  lass UsersUserMi
+00016e70: 6e28 424d 293a 0a09 6465 6163 7469 7661  n(BM):..deactiva
+00016e80: 7465 643a 4f70 7469 6f6e 616c 5b73 7472  ted:Optional[str
+00016e90: 5d20 3d20 4e6f 6e65 0a09 6669 7273 745f  ] = None..first_
+00016ea0: 6e61 6d65 3a4f 7074 696f 6e61 6c5b 7374  name:Optional[st
+00016eb0: 725d 203d 204e 6f6e 650a 0968 6964 6465  r] = None..hidde
+00016ec0: 6e3a 4f70 7469 6f6e 616c 5b69 6e74 5d20  n:Optional[int] 
+00016ed0: 3d20 4e6f 6e65 0a09 6964 3a69 6e74 0a09  = None..id:int..
+00016ee0: 6c61 7374 5f6e 616d 653a 4f70 7469 6f6e  last_name:Option
+00016ef0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00016f00: 6361 6e5f 6163 6365 7373 5f63 6c6f 7365  can_access_close
+00016f10: 643a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  d:Optional[bool]
+00016f20: 203d 204e 6f6e 650a 0969 735f 636c 6f73   = None..is_clos
+00016f30: 6564 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ed:Optional[bool
+00016f40: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+00016f50: 2055 7365 7273 5573 6572 5365 7474 696e   UsersUserSettin
+00016f60: 6773 5874 7228 424d 293a 0a09 636f 6e6e  gsXtr(BM):..conn
+00016f70: 6563 7469 6f6e 733a 4f70 7469 6f6e 616c  ections:Optional
+00016f80: 5b22 5573 6572 7355 7365 7243 6f6e 6e65  ["UsersUserConne
+00016f90: 6374 696f 6e73 225d 203d 204e 6f6e 650a  ctions"] = None.
+00016fa0: 0962 6461 7465 3a4f 7074 696f 6e61 6c5b  .bdate:Optional[
+00016fb0: 7374 725d 203d 204e 6f6e 650a 0962 6461  str] = None..bda
+00016fc0: 7465 5f76 6973 6962 696c 6974 793a 4f70  te_visibility:Op
+00016fd0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00016fe0: 6e65 0a09 6369 7479 3a4f 7074 696f 6e61  ne..city:Optiona
+00016ff0: 6c5b 2242 6173 6543 6974 7922 5d20 3d20  l["BaseCity"] = 
+00017000: 4e6f 6e65 0a09 636f 756e 7472 793a 4f70  None..country:Op
+00017010: 7469 6f6e 616c 5b22 4261 7365 436f 756e  tional["BaseCoun
+00017020: 7472 7922 5d20 3d20 4e6f 6e65 0a09 6669  try"] = None..fi
+00017030: 7273 745f 6e61 6d65 3a4f 7074 696f 6e61  rst_name:Optiona
+00017040: 6c5b 7374 725d 203d 204e 6f6e 650a 0968  l[str] = None..h
+00017050: 6f6d 655f 746f 776e 3a73 7472 0a09 6c61  ome_town:str..la
+00017060: 7374 5f6e 616d 653a 4f70 7469 6f6e 616c  st_name:Optional
+00017070: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6d61  [str] = None..ma
+00017080: 6964 656e 5f6e 616d 653a 4f70 7469 6f6e  iden_name:Option
+00017090: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+000170a0: 6e61 6d65 5f72 6571 7565 7374 3a4f 7074  name_request:Opt
+000170b0: 696f 6e61 6c5b 2241 6363 6f75 6e74 4e61  ional["AccountNa
+000170c0: 6d65 5265 7175 6573 7422 5d20 3d20 4e6f  meRequest"] = No
+000170d0: 6e65 0a09 7065 7273 6f6e 616c 3a4f 7074  ne..personal:Opt
+000170e0: 696f 6e61 6c5b 2255 7365 7273 5065 7273  ional["UsersPers
+000170f0: 6f6e 616c 225d 203d 204e 6f6e 650a 0970  onal"] = None..p
+00017100: 686f 6e65 3a4f 7074 696f 6e61 6c5b 7374  hone:Optional[st
+00017110: 725d 203d 204e 6f6e 650a 0972 656c 6174  r] = None..relat
+00017120: 696f 6e3a 4f70 7469 6f6e 616c 5b22 5573  ion:Optional["Us
+00017130: 6572 7355 7365 7252 656c 6174 696f 6e22  ersUserRelation"
+00017140: 5d20 3d20 4e6f 6e65 0a09 7265 6c61 7469  ] = None..relati
+00017150: 6f6e 5f70 6172 746e 6572 3a4f 7074 696f  on_partner:Optio
+00017160: 6e61 6c5b 2255 7365 7273 5573 6572 4d69  nal["UsersUserMi
+00017170: 6e22 5d20 3d20 4e6f 6e65 0a09 7265 6c61  n"] = None..rela
+00017180: 7469 6f6e 5f70 656e 6469 6e67 3a4f 7074  tion_pending:Opt
+00017190: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+000171a0: 6e65 0a09 7265 6c61 7469 6f6e 5f72 6571  ne..relation_req
+000171b0: 7565 7374 733a 4f70 7469 6f6e 616c 5b6c  uests:Optional[l
+000171c0: 6973 745b 2255 7365 7273 5573 6572 4d69  ist["UsersUserMi
+000171d0: 6e22 5d5d 203d 204e 6f6e 650a 0973 6372  n"]] = None..scr
+000171e0: 6565 6e5f 6e61 6d65 3a4f 7074 696f 6e61  een_name:Optiona
+000171f0: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
+00017200: 6578 3a4f 7074 696f 6e61 6c5b 2242 6173  ex:Optional["Bas
+00017210: 6553 6578 225d 203d 204e 6f6e 650a 0973  eSex"] = None..s
+00017220: 7461 7475 733a 7374 720a 0973 7461 7475  tatus:str..statu
+00017230: 735f 6175 6469 6f3a 4f70 7469 6f6e 616c  s_audio:Optional
+00017240: 5b22 4175 6469 6f41 7564 696f 225d 203d  ["AudioAudio"] =
+00017250: 204e 6f6e 650a 0969 6e74 6572 6573 7473   None..interests
+00017260: 3a4f 7074 696f 6e61 6c5b 2241 6363 6f75  :Optional["Accou
+00017270: 6e74 5573 6572 5365 7474 696e 6773 496e  ntUserSettingsIn
+00017280: 7465 7265 7374 7322 5d20 3d20 4e6f 6e65  terests"] = None
+00017290: 0a09 6c61 6e67 7561 6765 733a 4f70 7469  ..languages:Opti
+000172a0: 6f6e 616c 5b6c 6973 745b 7374 725d 5d20  onal[list[str]] 
+000172b0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2055  = None...class U
+000172c0: 7365 7273 5573 6572 7341 7272 6179 2842  sersUsersArray(B
+000172d0: 4d29 3a0a 0963 6f75 6e74 3a69 6e74 0a09  M):..count:int..
+000172e0: 6974 656d 733a 6c69 7374 5b69 6e74 5d0a  items:list[int].
+000172f0: 0a0a 0a0a 636c 6173 7320 5574 696c 7344  ....class UtilsD
+00017300: 6f6d 6169 6e52 6573 6f6c 7665 6454 7970  omainResolvedTyp
+00017310: 6528 456e 756d 293a 0a09 5553 4552 203d  e(Enum):..USER =
+00017320: 2022 7573 6572 220a 0947 524f 5550 203d   "user"..GROUP =
+00017330: 2022 6772 6f75 7022 0a09 4150 504c 4943   "group"..APPLIC
+00017340: 4154 494f 4e20 3d20 2261 7070 6c69 6361  ATION = "applica
+00017350: 7469 6f6e 220a 0950 4147 4520 3d20 2270  tion"..PAGE = "p
+00017360: 6167 6522 0a09 564b 5f41 5050 203d 2022  age"..VK_APP = "
+00017370: 766b 5f61 7070 220a 0943 4f4d 4d55 4e49  vk_app"..COMMUNI
+00017380: 5459 5f41 5050 4c49 4341 5449 4f4e 203d  TY_APPLICATION =
+00017390: 2022 636f 6d6d 756e 6974 795f 6170 706c   "community_appl
+000173a0: 6963 6174 696f 6e22 0a0a 636c 6173 7320  ication"..class 
+000173b0: 5574 696c 734c 696e 6b43 6865 636b 6564  UtilsLinkChecked
+000173c0: 5374 6174 7573 2845 6e75 6d29 3a0a 094e  Status(Enum):..N
+000173d0: 4f54 5f42 414e 4e45 4420 3d20 226e 6f74  OT_BANNED = "not
+000173e0: 5f62 616e 6e65 6422 0a09 4241 4e4e 4544  _banned"..BANNED
+000173f0: 203d 2022 6261 6e6e 6564 220a 0950 524f   = "banned"..PRO
+00017400: 4345 5353 494e 4720 3d20 2270 726f 6365  CESSING = "proce
+00017410: 7373 696e 6722 0a0a 636c 6173 7320 5574  ssing"..class Ut
+00017420: 696c 7344 6f6d 6169 6e52 6573 6f6c 7665  ilsDomainResolve
+00017430: 6428 424d 293a 0a09 6f62 6a65 6374 5f69  d(BM):..object_i
+00017440: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+00017450: 3d20 4e6f 6e65 0a09 6772 6f75 705f 6964  = None..group_id
+00017460: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00017470: 204e 6f6e 650a 0974 7970 653a 4f70 7469   None..type:Opti
+00017480: 6f6e 616c 5b22 5574 696c 7344 6f6d 6169  onal["UtilsDomai
+00017490: 6e52 6573 6f6c 7665 6454 7970 6522 5d20  nResolvedType"] 
+000174a0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2055  = None...class U
+000174b0: 7469 6c73 4c61 7374 5368 6f72 7465 6e65  tilsLastShortene
+000174c0: 644c 696e 6b28 424d 293a 0a09 6163 6365  dLink(BM):..acce
+000174d0: 7373 5f6b 6579 3a4f 7074 696f 6e61 6c5b  ss_key:Optional[
+000174e0: 7374 725d 203d 204e 6f6e 650a 096b 6579  str] = None..key
+000174f0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00017500: 204e 6f6e 650a 0973 686f 7274 5f75 726c   None..short_url
+00017510: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00017520: 204e 6f6e 650a 0974 696d 6573 7461 6d70   None..timestamp
+00017530: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00017540: 204e 6f6e 650a 0975 726c 3a4f 7074 696f   None..url:Optio
+00017550: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00017560: 0976 6965 7773 3a4f 7074 696f 6e61 6c5b  .views:Optional[
+00017570: 696e 745d 203d 204e 6f6e 650a 0a0a 636c  int] = None...cl
+00017580: 6173 7320 5574 696c 734c 696e 6b43 6865  ass UtilsLinkChe
+00017590: 636b 6564 2842 4d29 3a0a 096c 696e 6b3a  cked(BM):..link:
+000175a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000175b0: 4e6f 6e65 0a09 7374 6174 7573 3a4f 7074  None..status:Opt
+000175c0: 696f 6e61 6c5b 2255 7469 6c73 4c69 6e6b  ional["UtilsLink
+000175d0: 4368 6563 6b65 6453 7461 7475 7322 5d20  CheckedStatus"] 
+000175e0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2055  = None...class U
+000175f0: 7469 6c73 4c69 6e6b 5374 6174 7328 424d  tilsLinkStats(BM
+00017600: 293a 0a09 6b65 793a 4f70 7469 6f6e 616c  ):..key:Optional
+00017610: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7374  [str] = None..st
+00017620: 6174 733a 4f70 7469 6f6e 616c 5b6c 6973  ats:Optional[lis
+00017630: 745b 2255 7469 6c73 5374 6174 7322 5d5d  t["UtilsStats"]]
+00017640: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
+00017650: 5574 696c 734c 696e 6b53 7461 7473 4578  UtilsLinkStatsEx
+00017660: 7465 6e64 6564 2842 4d29 3a0a 096b 6579  tended(BM):..key
+00017670: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+00017680: 204e 6f6e 650a 0973 7461 7473 3a4f 7074   None..stats:Opt
+00017690: 696f 6e61 6c5b 6c69 7374 5b22 5574 696c  ional[list["Util
+000176a0: 7353 7461 7473 4578 7465 6e64 6564 225d  sStatsExtended"]
+000176b0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
+000176c0: 2055 7469 6c73 5368 6f72 744c 696e 6b28   UtilsShortLink(
+000176d0: 424d 293a 0a09 6163 6365 7373 5f6b 6579  BM):..access_key
 000176e0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-000176f0: 204e 6f6e 650a 0973 686f 7274 5f75 726c   None..short_url
-00017700: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00017710: 204e 6f6e 650a 0975 726c 3a4f 7074 696f   None..url:Optio
+000176f0: 204e 6f6e 650a 096b 6579 3a4f 7074 696f   None..key:Optio
+00017700: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00017710: 0973 686f 7274 5f75 726c 3a4f 7074 696f  .short_url:Optio
 00017720: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00017730: 0a0a 636c 6173 7320 5574 696c 7353 7461  ..class UtilsSta
-00017740: 7473 2842 4d29 3a0a 0974 696d 6573 7461  ts(BM):..timesta
-00017750: 6d70 3a4f 7074 696f 6e61 6c5b 696e 745d  mp:Optional[int]
-00017760: 203d 204e 6f6e 650a 0976 6965 7773 3a4f   = None..views:O
-00017770: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00017780: 6f6e 650a 0a0a 636c 6173 7320 5574 696c  one...class Util
-00017790: 7353 7461 7473 4369 7479 2842 4d29 3a0a  sStatsCity(BM):.
-000177a0: 0963 6974 795f 6964 3a4f 7074 696f 6e61  .city_id:Optiona
-000177b0: 6c5b 696e 745d 203d 204e 6f6e 650a 0976  l[int] = None..v
-000177c0: 6965 7773 3a4f 7074 696f 6e61 6c5b 696e  iews:Optional[in
-000177d0: 745d 203d 204e 6f6e 650a 0a0a 636c 6173  t] = None...clas
-000177e0: 7320 5574 696c 7353 7461 7473 436f 756e  s UtilsStatsCoun
-000177f0: 7472 7928 424d 293a 0a09 636f 756e 7472  try(BM):..countr
-00017800: 795f 6964 3a4f 7074 696f 6e61 6c5b 696e  y_id:Optional[in
-00017810: 745d 203d 204e 6f6e 650a 0976 6965 7773  t] = None..views
-00017820: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00017830: 204e 6f6e 650a 0a0a 636c 6173 7320 5574   None...class Ut
-00017840: 696c 7353 7461 7473 4578 7465 6e64 6564  ilsStatsExtended
-00017850: 2842 4d29 3a0a 0963 6974 6965 733a 4f70  (BM):..cities:Op
-00017860: 7469 6f6e 616c 5b6c 6973 745b 2255 7469  tional[list["Uti
-00017870: 6c73 5374 6174 7343 6974 7922 5d5d 203d  lsStatsCity"]] =
-00017880: 204e 6f6e 650a 0963 6f75 6e74 7269 6573   None..countries
-00017890: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
-000178a0: 5574 696c 7353 7461 7473 436f 756e 7472  UtilsStatsCountr
-000178b0: 7922 5d5d 203d 204e 6f6e 650a 0973 6578  y"]] = None..sex
-000178c0: 5f61 6765 3a4f 7074 696f 6e61 6c5b 6c69  _age:Optional[li
-000178d0: 7374 5b22 5574 696c 7353 7461 7473 5365  st["UtilsStatsSe
-000178e0: 7841 6765 225d 5d20 3d20 4e6f 6e65 0a09  xAge"]] = None..
-000178f0: 7469 6d65 7374 616d 703a 4f70 7469 6f6e  timestamp:Option
-00017900: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00017910: 7669 6577 733a 4f70 7469 6f6e 616c 5b69  views:Optional[i
-00017920: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  nt] = None...cla
-00017930: 7373 2055 7469 6c73 5374 6174 7353 6578  ss UtilsStatsSex
-00017940: 4167 6528 424d 293a 0a09 6167 655f 7261  Age(BM):..age_ra
-00017950: 6e67 653a 4f70 7469 6f6e 616c 5b73 7472  nge:Optional[str
-00017960: 5d20 3d20 4e6f 6e65 0a09 6665 6d61 6c65  ] = None..female
-00017970: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00017980: 204e 6f6e 650a 096d 616c 653a 4f70 7469   None..male:Opti
-00017990: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000179a0: 0a0a 0a0a 0a63 6c61 7373 2056 6964 656f  .....class Video
-000179b0: 4c69 7665 496e 666f 2842 4d29 3a0a 0965  LiveInfo(BM):..e
-000179c0: 6e61 626c 6564 3a62 6f6f 6c0a 0969 735f  nabled:bool..is_
-000179d0: 6e6f 7469 6669 6361 7469 6f6e 735f 626c  notifications_bl
-000179e0: 6f63 6b65 643a 4f70 7469 6f6e 616c 5b62  ocked:Optional[b
-000179f0: 6f6f 6c5d 203d 204e 6f6e 650a 0a0a 636c  ool] = None...cl
-00017a00: 6173 7320 5669 6465 6f4c 6976 6553 6574  ass VideoLiveSet
-00017a10: 7469 6e67 7328 424d 293a 0a09 6361 6e5f  tings(BM):..can_
-00017a20: 7265 7769 6e64 3a4f 7074 696f 6e61 6c5b  rewind:Optional[
-00017a30: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6973  bool] = None..is
-00017a40: 5f65 6e64 6c65 7373 3a4f 7074 696f 6e61  _endless:Optiona
-00017a50: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-00017a60: 6d61 785f 6475 7261 7469 6f6e 3a4f 7074  max_duration:Opt
-00017a70: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00017a80: 650a 0a0a 636c 6173 7320 5669 6465 6f53  e...class VideoS
-00017a90: 6176 6552 6573 756c 7428 424d 293a 0a09  aveResult(BM):..
-00017aa0: 6163 6365 7373 5f6b 6579 3a4f 7074 696f  access_key:Optio
-00017ab0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00017ac0: 0964 6573 6372 6970 7469 6f6e 3a4f 7074  .description:Opt
-00017ad0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00017ae0: 650a 096f 776e 6572 5f69 643a 4f70 7469  e..owner_id:Opti
-00017af0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00017b00: 0a09 7469 746c 653a 4f70 7469 6f6e 616c  ..title:Optional
-00017b10: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7570  [str] = None..up
-00017b20: 6c6f 6164 5f75 726c 3a4f 7074 696f 6e61  load_url:Optiona
-00017b30: 6c5b 7374 725d 203d 204e 6f6e 650a 0976  l[str] = None..v
-00017b40: 6964 656f 5f69 643a 4f70 7469 6f6e 616c  ideo_id:Optional
-00017b50: 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a 0a63  [int] = None...c
-00017b60: 6c61 7373 2056 6964 656f 5669 6465 6f28  lass VideoVideo(
-00017b70: 424d 293a 0a09 6163 6365 7373 5f6b 6579  BM):..access_key
-00017b80: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00017b90: 204e 6f6e 650a 0961 6464 696e 675f 6461   None..adding_da
-00017ba0: 7465 3a4f 7074 696f 6e61 6c5b 696e 745d  te:Optional[int]
-00017bb0: 203d 204e 6f6e 650a 0963 616e 5f63 6f6d   = None..can_com
-00017bc0: 6d65 6e74 3a4f 7074 696f 6e61 6c5b 626f  ment:Optional[bo
-00017bd0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
-00017be0: 6564 6974 3a4f 7074 696f 6e61 6c5b 626f  edit:Optional[bo
-00017bf0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
-00017c00: 6c69 6b65 3a4f 7074 696f 6e61 6c5b 626f  like:Optional[bo
-00017c10: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
-00017c20: 7265 706f 7374 3a4f 7074 696f 6e61 6c5b  repost:Optional[
-00017c30: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6361  bool] = None..ca
-00017c40: 6e5f 7375 6273 6372 6962 653a 4f70 7469  n_subscribe:Opti
-00017c50: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00017c60: 650a 0963 616e 5f61 6464 5f74 6f5f 6661  e..can_add_to_fa
-00017c70: 7665 733a 4f70 7469 6f6e 616c 5b62 6f6f  ves:Optional[boo
-00017c80: 6c5d 203d 204e 6f6e 650a 0963 616e 5f61  l] = None..can_a
-00017c90: 6464 3a4f 7074 696f 6e61 6c5b 626f 6f6c  dd:Optional[bool
-00017ca0: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 6174  ] = None..can_at
-00017cb0: 7461 6368 5f6c 696e 6b3a 4f70 7469 6f6e  tach_link:Option
-00017cc0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-00017cd0: 0969 735f 7072 6976 6174 653a 4f70 7469  .is_private:Opti
-00017ce0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00017cf0: 650a 0963 6f6d 6d65 6e74 733a 4f70 7469  e..comments:Opti
-00017d00: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00017d10: 0a09 6461 7465 3a4f 7074 696f 6e61 6c5b  ..date:Optional[
-00017d20: 696e 745d 203d 204e 6f6e 650a 0964 6573  int] = None..des
-00017d30: 6372 6970 7469 6f6e 3a4f 7074 696f 6e61  cription:Optiona
-00017d40: 6c5b 7374 725d 203d 204e 6f6e 650a 0964  l[str] = None..d
-00017d50: 7572 6174 696f 6e3a 4f70 7469 6f6e 616c  uration:Optional
-00017d60: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 696d  [int] = None..im
-00017d70: 6167 653a 4f70 7469 6f6e 616c 5b6c 6973  age:Optional[lis
-00017d80: 745b 2256 6964 656f 5669 6465 6f49 6d61  t["VideoVideoIma
-00017d90: 6765 225d 5d20 3d20 4e6f 6e65 0a09 6669  ge"]] = None..fi
-00017da0: 7273 745f 6672 616d 653a 4f70 7469 6f6e  rst_frame:Option
-00017db0: 616c 5b6c 6973 745b 2256 6964 656f 5669  al[list["VideoVi
-00017dc0: 6465 6f49 6d61 6765 225d 5d20 3d20 4e6f  deoImage"]] = No
-00017dd0: 6e65 0a09 7769 6474 683a 4f70 7469 6f6e  ne..width:Option
-00017de0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-00017df0: 6865 6967 6874 3a4f 7074 696f 6e61 6c5b  height:Optional[
-00017e00: 696e 745d 203d 204e 6f6e 650a 0969 643a  int] = None..id:
-00017e10: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00017e20: 4e6f 6e65 0a09 6f77 6e65 725f 6964 3a4f  None..owner_id:O
-00017e30: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00017e40: 6f6e 650a 0975 7365 725f 6964 3a4f 7074  one..user_id:Opt
-00017e50: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00017e60: 650a 0974 6974 6c65 3a4f 7074 696f 6e61  e..title:Optiona
-00017e70: 6c5b 7374 725d 203d 204e 6f6e 650a 0969  l[str] = None..i
-00017e80: 735f 6661 766f 7269 7465 3a4f 7074 696f  s_favorite:Optio
-00017e90: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00017ea0: 0a09 706c 6179 6572 3a4f 7074 696f 6e61  ..player:Optiona
-00017eb0: 6c5b 7374 725d 203d 204e 6f6e 650a 0970  l[str] = None..p
-00017ec0: 726f 6365 7373 696e 673a 4f70 7469 6f6e  rocessing:Option
-00017ed0: 616c 5b22 4261 7365 5072 6f70 6572 7479  al["BaseProperty
-00017ee0: 4578 6973 7473 225d 203d 204e 6f6e 650a  Exists"] = None.
-00017ef0: 0963 6f6e 7665 7274 696e 673a 4f70 7469  .converting:Opti
-00017f00: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-00017f10: 650a 0961 6464 6564 3a4f 7074 696f 6e61  e..added:Optiona
-00017f20: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-00017f30: 6973 5f73 7562 7363 7269 6265 643a 4f70  is_subscribed:Op
-00017f40: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-00017f50: 6f6e 650a 0974 7261 636b 5f63 6f64 653a  one..track_code:
-00017f60: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00017f70: 4e6f 6e65 0a09 7265 7065 6174 3a4f 7074  None..repeat:Opt
-00017f80: 696f 6e61 6c5b 2242 6173 6550 726f 7065  ional["BasePrope
-00017f90: 7274 7945 7869 7374 7322 5d20 3d20 4e6f  rtyExists"] = No
-00017fa0: 6e65 0a09 7479 7065 3a4f 7074 696f 6e61  ne..type:Optiona
-00017fb0: 6c5b 7374 725d 203d 204e 6f6e 650a 0976  l[str] = None..v
-00017fc0: 6965 7773 3a4f 7074 696f 6e61 6c5b 696e  iews:Optional[in
-00017fd0: 745d 203d 204e 6f6e 650a 096c 6f63 616c  t] = None..local
-00017fe0: 5f76 6965 7773 3a4f 7074 696f 6e61 6c5b  _views:Optional[
-00017ff0: 696e 745d 203d 204e 6f6e 650a 0963 6f6e  int] = None..con
-00018000: 7465 6e74 5f72 6573 7472 6963 7465 643a  tent_restricted:
-00018010: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00018020: 4e6f 6e65 0a09 636f 6e74 656e 745f 7265  None..content_re
-00018030: 7374 7269 6374 6564 5f6d 6573 7361 6765  stricted_message
-00018040: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00018050: 204e 6f6e 650a 0962 616c 616e 6365 3a4f   None..balance:O
-00018060: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00018070: 6f6e 650a 096c 6976 655f 7374 6174 7573  one..live_status
-00018080: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00018090: 204e 6f6e 650a 096c 6976 653a 4f70 7469   None..live:Opti
-000180a0: 6f6e 616c 5b22 4261 7365 5072 6f70 6572  onal["BaseProper
-000180b0: 7479 4578 6973 7473 225d 203d 204e 6f6e  tyExists"] = Non
-000180c0: 650a 0975 7063 6f6d 696e 673a 4f70 7469  e..upcoming:Opti
-000180d0: 6f6e 616c 5b22 4261 7365 5072 6f70 6572  onal["BaseProper
-000180e0: 7479 4578 6973 7473 225d 203d 204e 6f6e  tyExists"] = Non
-000180f0: 650a 096c 6976 655f 7374 6172 745f 7469  e..live_start_ti
-00018100: 6d65 3a4f 7074 696f 6e61 6c5b 696e 745d  me:Optional[int]
-00018110: 203d 204e 6f6e 650a 096c 6976 655f 6e6f   = None..live_no
-00018120: 7469 6679 3a4f 7074 696f 6e61 6c5b 626f  tify:Optional[bo
-00018130: 6f6c 5d20 3d20 4e6f 6e65 0a09 7370 6563  ol] = None..spec
-00018140: 7461 746f 7273 3a4f 7074 696f 6e61 6c5b  tators:Optional[
-00018150: 696e 745d 203d 204e 6f6e 650a 0970 6c61  int] = None..pla
-00018160: 7466 6f72 6d3a 4f70 7469 6f6e 616c 5b73  tform:Optional[s
-00018170: 7472 5d20 3d20 4e6f 6e65 0a09 6c69 6b65  tr] = None..like
-00018180: 733a 4f70 7469 6f6e 616c 5b22 4261 7365  s:Optional["Base
-00018190: 4c69 6b65 7322 5d20 3d20 4e6f 6e65 0a09  Likes"] = None..
-000181a0: 7265 706f 7374 733a 4f70 7469 6f6e 616c  reposts:Optional
-000181b0: 5b22 4261 7365 5265 706f 7374 7349 6e66  ["BaseRepostsInf
-000181c0: 6f22 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  o"] = None...cla
-000181d0: 7373 2056 6964 656f 5669 6465 6f41 6c62  ss VideoVideoAlb
-000181e0: 756d 2842 4d29 3a0a 0969 643a 696e 740a  um(BM):..id:int.
-000181f0: 096f 776e 6572 5f69 643a 696e 740a 0974  .owner_id:int..t
-00018200: 6974 6c65 3a73 7472 0a0a 0a63 6c61 7373  itle:str...class
-00018210: 2056 6964 656f 5669 6465 6f46 696c 6573   VideoVideoFiles
-00018220: 2842 4d29 3a0a 0965 7874 6572 6e61 6c3a  (BM):..external:
-00018230: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00018240: 4e6f 6e65 0a09 6d70 345f 3134 343a 4f70  None..mp4_144:Op
-00018250: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00018260: 6e65 0a09 6d70 345f 3234 303a 4f70 7469  ne..mp4_240:Opti
-00018270: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00018280: 0a09 6d70 345f 3336 303a 4f70 7469 6f6e  ..mp4_360:Option
-00018290: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-000182a0: 6d70 345f 3438 303a 4f70 7469 6f6e 616c  mp4_480:Optional
-000182b0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6d70  [str] = None..mp
-000182c0: 345f 3732 303a 4f70 7469 6f6e 616c 5b73  4_720:Optional[s
-000182d0: 7472 5d20 3d20 4e6f 6e65 0a09 6d70 345f  tr] = None..mp4_
-000182e0: 3130 3830 3a4f 7074 696f 6e61 6c5b 7374  1080:Optional[st
-000182f0: 725d 203d 204e 6f6e 650a 096d 7034 5f31  r] = None..mp4_1
-00018300: 3434 303a 4f70 7469 6f6e 616c 5b73 7472  440:Optional[str
-00018310: 5d20 3d20 4e6f 6e65 0a09 6d70 345f 3231  ] = None..mp4_21
-00018320: 3630 3a4f 7074 696f 6e61 6c5b 7374 725d  60:Optional[str]
-00018330: 203d 204e 6f6e 650a 0966 6c76 5f33 3230   = None..flv_320
-00018340: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00018350: 204e 6f6e 650a 0a0a 0a0a 636c 6173 7320   None.....class 
-00018360: 5761 6c6c 436f 6d6d 656e 7441 7474 6163  WallCommentAttac
-00018370: 686d 656e 7454 7970 6528 456e 756d 293a  hmentType(Enum):
-00018380: 0a09 5048 4f54 4f20 3d20 2270 686f 746f  ..PHOTO = "photo
-00018390: 220a 0941 5544 494f 203d 2022 6175 6469  "..AUDIO = "audi
-000183a0: 6f22 0a09 5649 4445 4f20 3d20 2276 6964  o"..VIDEO = "vid
-000183b0: 656f 220a 0944 4f43 203d 2022 646f 6322  eo"..DOC = "doc"
-000183c0: 0a09 4c49 4e4b 203d 2022 6c69 6e6b 220a  ..LINK = "link".
-000183d0: 094e 4f54 4520 3d20 226e 6f74 6522 0a09  .NOTE = "note"..
-000183e0: 5041 4745 203d 2022 7061 6765 220a 094d  PAGE = "page"..M
-000183f0: 4152 4b45 545f 4d41 524b 4554 5f41 4c42  ARKET_MARKET_ALB
-00018400: 554d 203d 2022 6d61 726b 6574 5f6d 6172  UM = "market_mar
-00018410: 6b65 745f 616c 6275 6d22 0a09 4d41 524b  ket_album"..MARK
-00018420: 4554 203d 2022 6d61 726b 6574 220a 0953  ET = "market"..S
-00018430: 5449 434b 4552 203d 2022 7374 6963 6b65  TICKER = "sticke
-00018440: 7222 0a0a 636c 6173 7320 5761 6c6c 4765  r"..class WallGe
-00018450: 7446 696c 7465 7228 456e 756d 293a 0a09  tFilter(Enum):..
-00018460: 4f57 4e45 5220 3d20 226f 776e 6572 220a  OWNER = "owner".
-00018470: 094f 5448 4552 5320 3d20 226f 7468 6572  .OTHERS = "other
-00018480: 7322 0a09 414c 4c20 3d20 2261 6c6c 220a  s"..ALL = "all".
-00018490: 0950 4f53 5450 4f4e 4544 203d 2022 706f  .POSTPONED = "po
-000184a0: 7374 706f 6e65 6422 0a09 5355 4747 4553  stponed"..SUGGES
-000184b0: 5453 203d 2022 7375 6767 6573 7473 220a  TS = "suggests".
-000184c0: 0941 5243 4849 5645 4420 3d20 2261 7263  .ARCHIVED = "arc
-000184d0: 6869 7665 6422 0a09 444f 4e55 5420 3d20  hived"..DONUT = 
-000184e0: 2264 6f6e 7574 220a 0a63 6c61 7373 2057  "donut"..class W
-000184f0: 616c 6c50 6f73 7453 6f75 7263 6554 7970  allPostSourceTyp
-00018500: 6528 456e 756d 293a 0a09 564b 203d 2022  e(Enum):..VK = "
-00018510: 766b 220a 0957 4944 4745 5420 3d20 2277  vk"..WIDGET = "w
-00018520: 6964 6765 7422 0a09 4150 4920 3d20 2261  idget"..API = "a
-00018530: 7069 220a 0952 5353 203d 2022 7273 7322  pi"..RSS = "rss"
-00018540: 0a09 534d 5320 3d20 2273 6d73 220a 094d  ..SMS = "sms"..M
-00018550: 564b 203d 2022 6d76 6b22 0a0a 636c 6173  VK = "mvk"..clas
-00018560: 7320 5761 6c6c 506f 7374 5479 7065 2845  s WallPostType(E
-00018570: 6e75 6d29 3a0a 0950 4f53 5420 3d20 2270  num):..POST = "p
-00018580: 6f73 7422 0a09 434f 5059 203d 2022 636f  ost"..COPY = "co
-00018590: 7079 220a 0952 4550 4c59 203d 2022 7265  py"..REPLY = "re
-000185a0: 706c 7922 0a09 504f 5354 504f 4e45 203d  ply"..POSTPONE =
-000185b0: 2022 706f 7374 706f 6e65 220a 0953 5547   "postpone"..SUG
-000185c0: 4745 5354 203d 2022 7375 6767 6573 7422  GEST = "suggest"
-000185d0: 0a09 504f 5354 5f41 4453 203d 2022 706f  ..POST_ADS = "po
-000185e0: 7374 5f61 6473 220a 0950 484f 544f 203d  st_ads"..PHOTO =
-000185f0: 2022 7068 6f74 6f22 0a09 5649 4445 4f20   "photo"..VIDEO 
-00018600: 3d20 2276 6964 656f 220a 0a63 6c61 7373  = "video"..class
-00018610: 2057 616c 6c57 616c 6c70 6f73 7441 7474   WallWallpostAtt
-00018620: 6163 686d 656e 7454 7970 6528 456e 756d  achmentType(Enum
-00018630: 293a 0a09 5048 4f54 4f20 3d20 2270 686f  ):..PHOTO = "pho
-00018640: 746f 220a 0950 484f 544f 535f 4c49 5354  to"..PHOTOS_LIST
-00018650: 203d 2022 7068 6f74 6f73 5f6c 6973 7422   = "photos_list"
-00018660: 0a09 504f 5354 4544 5f50 484f 544f 203d  ..POSTED_PHOTO =
-00018670: 2022 706f 7374 6564 5f70 686f 746f 220a   "posted_photo".
-00018680: 0941 5544 494f 203d 2022 6175 6469 6f22  .AUDIO = "audio"
-00018690: 0a09 4155 4449 4f5f 504c 4159 4c49 5354  ..AUDIO_PLAYLIST
-000186a0: 203d 2022 6175 6469 6f5f 706c 6179 6c69   = "audio_playli
-000186b0: 7374 220a 0956 4944 454f 203d 2022 7669  st"..VIDEO = "vi
-000186c0: 6465 6f22 0a09 444f 4320 3d20 2264 6f63  deo"..DOC = "doc
-000186d0: 220a 094c 494e 4b20 3d20 226c 696e 6b22  "..LINK = "link"
-000186e0: 0a09 4752 4146 4649 5449 203d 2022 6772  ..GRAFFITI = "gr
-000186f0: 6166 6669 7469 220a 094e 4f54 4520 3d20  affiti"..NOTE = 
-00018700: 226e 6f74 6522 0a09 4150 5020 3d20 2261  "note"..APP = "a
-00018710: 7070 220a 0950 4f4c 4c20 3d20 2270 6f6c  pp"..POLL = "pol
-00018720: 6c22 0a09 5041 4745 203d 2022 7061 6765  l"..PAGE = "page
-00018730: 220a 0941 4c42 554d 203d 2022 616c 6275  "..ALBUM = "albu
-00018740: 6d22 0a09 4d41 524b 4554 5f41 4c42 554d  m"..MARKET_ALBUM
-00018750: 203d 2022 6d61 726b 6574 5f61 6c62 756d   = "market_album
-00018760: 220a 094d 4152 4b45 5420 3d20 226d 6172  "..MARKET = "mar
-00018770: 6b65 7422 0a09 4556 454e 5420 3d20 2265  ket"..EVENT = "e
-00018780: 7665 6e74 220a 0944 4f4e 5554 5f4c 494e  vent"..DONUT_LIN
-00018790: 4b20 3d20 2264 6f6e 7574 5f6c 696e 6b22  K = "donut_link"
-000187a0: 0a09 4152 5449 434c 4520 3d20 2261 7274  ..ARTICLE = "art
-000187b0: 6963 6c65 220a 0954 4558 544c 4956 4520  icle"..TEXTLIVE 
-000187c0: 3d20 2274 6578 746c 6976 6522 0a09 5445  = "textlive"..TE
-000187d0: 5854 504f 5354 203d 2022 7465 7874 706f  XTPOST = "textpo
-000187e0: 7374 220a 0954 4558 5450 4f53 545f 5055  st"..TEXTPOST_PU
-000187f0: 424c 4953 4820 3d20 2274 6578 7470 6f73  BLISH = "textpos
-00018800: 745f 7075 626c 6973 6822 0a09 5349 5455  t_publish"..SITU
-00018810: 4154 494f 4e41 4c5f 5448 454d 4520 3d20  ATIONAL_THEME = 
-00018820: 2273 6974 7561 7469 6f6e 616c 5f74 6865  "situational_the
-00018830: 6d65 220a 0947 524f 5550 203d 2022 6772  me"..GROUP = "gr
-00018840: 6f75 7022 0a09 5354 4943 4b45 5220 3d20  oup"..STICKER = 
-00018850: 2273 7469 636b 6572 220a 0950 4f44 4341  "sticker"..PODCA
-00018860: 5354 203d 2022 706f 6463 6173 7422 0a0a  ST = "podcast"..
-00018870: 636c 6173 7320 5761 6c6c 4170 7050 6f73  class WallAppPos
-00018880: 7428 424d 293a 0a09 6964 3a4f 7074 696f  t(BM):..id:Optio
-00018890: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-000188a0: 096e 616d 653a 4f70 7469 6f6e 616c 5b73  .name:Optional[s
-000188b0: 7472 5d20 3d20 4e6f 6e65 0a09 7068 6f74  tr] = None..phot
-000188c0: 6f5f 3133 303a 4f70 7469 6f6e 616c 5b73  o_130:Optional[s
-000188d0: 7472 5d20 3d20 4e6f 6e65 0a09 7068 6f74  tr] = None..phot
-000188e0: 6f5f 3630 343a 4f70 7469 6f6e 616c 5b73  o_604:Optional[s
-000188f0: 7472 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  tr] = None...cla
-00018900: 7373 2057 616c 6c41 7474 6163 6865 644e  ss WallAttachedN
-00018910: 6f74 6528 424d 293a 0a09 636f 6d6d 656e  ote(BM):..commen
-00018920: 7473 3a69 6e74 0a09 6461 7465 3a69 6e74  ts:int..date:int
-00018930: 0a09 6964 3a69 6e74 0a09 6f77 6e65 725f  ..id:int..owner_
-00018940: 6964 3a69 6e74 0a09 7265 6164 5f63 6f6d  id:int..read_com
-00018950: 6d65 6e74 733a 696e 740a 0974 6974 6c65  ments:int..title
-00018960: 3a73 7472 0a09 7465 7874 3a4f 7074 696f  :str..text:Optio
-00018970: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00018980: 0970 7269 7661 6379 5f76 6965 773a 4f70  .privacy_view:Op
-00018990: 7469 6f6e 616c 5b6c 6973 745b 7374 725d  tional[list[str]
-000189a0: 5d20 3d20 4e6f 6e65 0a09 7072 6976 6163  ] = None..privac
-000189b0: 795f 636f 6d6d 656e 743a 4f70 7469 6f6e  y_comment:Option
-000189c0: 616c 5b6c 6973 745b 7374 725d 5d20 3d20  al[list[str]] = 
-000189d0: 4e6f 6e65 0a09 6361 6e5f 636f 6d6d 656e  None..can_commen
-000189e0: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
-000189f0: 3d20 4e6f 6e65 0a09 7465 7874 5f77 696b  = None..text_wik
-00018a00: 693a 4f70 7469 6f6e 616c 5b73 7472 5d20  i:Optional[str] 
-00018a10: 3d20 4e6f 6e65 0a09 7669 6577 5f75 726c  = None..view_url
-00018a20: 3a73 7472 0a0a 0a63 6c61 7373 2057 616c  :str...class Wal
-00018a30: 6c43 6172 6f75 7365 6c42 6173 6528 424d  lCarouselBase(BM
-00018a40: 293a 0a09 6361 726f 7573 656c 5f6f 6666  ):..carousel_off
-00018a50: 7365 743a 4f70 7469 6f6e 616c 5b69 6e74  set:Optional[int
-00018a60: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
-00018a70: 2057 616c 6c43 6f6d 6d65 6e74 4174 7461   WallCommentAtta
-00018a80: 6368 6d65 6e74 2842 4d29 3a0a 0961 7564  chment(BM):..aud
-00018a90: 696f 3a4f 7074 696f 6e61 6c5b 2241 7564  io:Optional["Aud
-00018aa0: 696f 4175 6469 6f22 5d20 3d20 4e6f 6e65  ioAudio"] = None
-00018ab0: 0a09 646f 633a 4f70 7469 6f6e 616c 5b22  ..doc:Optional["
-00018ac0: 446f 6373 446f 6322 5d20 3d20 4e6f 6e65  DocsDoc"] = None
-00018ad0: 0a09 6c69 6e6b 3a4f 7074 696f 6e61 6c5b  ..link:Optional[
-00018ae0: 2242 6173 654c 696e 6b22 5d20 3d20 4e6f  "BaseLink"] = No
-00018af0: 6e65 0a09 6d61 726b 6574 3a4f 7074 696f  ne..market:Optio
-00018b00: 6e61 6c5b 224d 6172 6b65 744d 6172 6b65  nal["MarketMarke
-00018b10: 7449 7465 6d22 5d20 3d20 4e6f 6e65 0a09  tItem"] = None..
-00018b20: 6d61 726b 6574 5f6d 6172 6b65 745f 616c  market_market_al
-00018b30: 6275 6d3a 4f70 7469 6f6e 616c 5b22 4d61  bum:Optional["Ma
-00018b40: 726b 6574 4d61 726b 6574 416c 6275 6d22  rketMarketAlbum"
-00018b50: 5d20 3d20 4e6f 6e65 0a09 6e6f 7465 3a4f  ] = None..note:O
-00018b60: 7074 696f 6e61 6c5b 2257 616c 6c41 7474  ptional["WallAtt
-00018b70: 6163 6865 644e 6f74 6522 5d20 3d20 4e6f  achedNote"] = No
-00018b80: 6e65 0a09 7061 6765 3a4f 7074 696f 6e61  ne..page:Optiona
-00018b90: 6c5b 2250 6167 6573 5769 6b69 7061 6765  l["PagesWikipage
-00018ba0: 4675 6c6c 225d 203d 204e 6f6e 650a 0970  Full"] = None..p
-00018bb0: 686f 746f 3a4f 7074 696f 6e61 6c5b 2250  hoto:Optional["P
-00018bc0: 686f 746f 7350 686f 746f 225d 203d 204e  hotosPhoto"] = N
-00018bd0: 6f6e 650a 0973 7469 636b 6572 3a4f 7074  one..sticker:Opt
-00018be0: 696f 6e61 6c5b 2242 6173 6553 7469 636b  ional["BaseStick
-00018bf0: 6572 225d 203d 204e 6f6e 650a 0974 7970  er"] = None..typ
-00018c00: 653a 2257 616c 6c43 6f6d 6d65 6e74 4174  e:"WallCommentAt
-00018c10: 7461 6368 6d65 6e74 5479 7065 220a 0976  tachmentType"..v
-00018c20: 6964 656f 3a4f 7074 696f 6e61 6c5b 2256  ideo:Optional["V
-00018c30: 6964 656f 5669 6465 6f22 5d20 3d20 4e6f  ideoVideo"] = No
-00018c40: 6e65 0a0a 0a63 6c61 7373 2057 616c 6c47  ne...class WallG
-00018c50: 656f 2842 4d29 3a0a 0963 6f6f 7264 696e  eo(BM):..coordin
-00018c60: 6174 6573 3a4f 7074 696f 6e61 6c5b 7374  ates:Optional[st
-00018c70: 725d 203d 204e 6f6e 650a 0970 6c61 6365  r] = None..place
-00018c80: 3a4f 7074 696f 6e61 6c5b 2242 6173 6550  :Optional["BaseP
-00018c90: 6c61 6365 225d 203d 204e 6f6e 650a 0973  lace"] = None..s
-00018ca0: 686f 776d 6170 3a4f 7074 696f 6e61 6c5b  howmap:Optional[
-00018cb0: 696e 745d 203d 204e 6f6e 650a 0974 7970  int] = None..typ
-00018cc0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-00018cd0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2057  = None...class W
-00018ce0: 616c 6c47 7261 6666 6974 6928 424d 293a  allGraffiti(BM):
-00018cf0: 0a09 6964 3a4f 7074 696f 6e61 6c5b 696e  ..id:Optional[in
-00018d00: 745d 203d 204e 6f6e 650a 096f 776e 6572  t] = None..owner
-00018d10: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-00018d20: 5d20 3d20 4e6f 6e65 0a09 7068 6f74 6f5f  ] = None..photo_
-00018d30: 3230 303a 4f70 7469 6f6e 616c 5b73 7472  200:Optional[str
-00018d40: 5d20 3d20 4e6f 6e65 0a09 7068 6f74 6f5f  ] = None..photo_
-00018d50: 3538 363a 4f70 7469 6f6e 616c 5b73 7472  586:Optional[str
-00018d60: 5d20 3d20 4e6f 6e65 0a09 6865 6967 6874  ] = None..height
-00018d70: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00018d80: 204e 6f6e 650a 0975 726c 3a4f 7074 696f   None..url:Optio
-00018d90: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00018da0: 0977 6964 7468 3a4f 7074 696f 6e61 6c5b  .width:Optional[
-00018db0: 696e 745d 203d 204e 6f6e 650a 0961 6363  int] = None..acc
-00018dc0: 6573 735f 6b65 793a 4f70 7469 6f6e 616c  ess_key:Optional
-00018dd0: 5b73 7472 5d20 3d20 4e6f 6e65 0a0a 0a63  [str] = None...c
-00018de0: 6c61 7373 2057 616c 6c50 6f73 7443 6f70  lass WallPostCop
-00018df0: 7972 6967 6874 2842 4d29 3a0a 0969 643a  yright(BM):..id:
-00018e00: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00018e10: 4e6f 6e65 0a09 6c69 6e6b 3a73 7472 0a09  None..link:str..
-00018e20: 6e61 6d65 3a73 7472 0a09 7479 7065 3a73  name:str..type:s
-00018e30: 7472 0a0a 0a63 6c61 7373 2057 616c 6c50  tr...class WallP
-00018e40: 6f73 7453 6f75 7263 6528 424d 293a 0a09  ostSource(BM):..
-00018e50: 6461 7461 3a4f 7074 696f 6e61 6c5b 7374  data:Optional[st
-00018e60: 725d 203d 204e 6f6e 650a 0970 6c61 7466  r] = None..platf
-00018e70: 6f72 6d3a 4f70 7469 6f6e 616c 5b73 7472  orm:Optional[str
-00018e80: 5d20 3d20 4e6f 6e65 0a09 7479 7065 3a4f  ] = None..type:O
-00018e90: 7074 696f 6e61 6c5b 2257 616c 6c50 6f73  ptional["WallPos
-00018ea0: 7453 6f75 7263 6554 7970 6522 5d20 3d20  tSourceType"] = 
-00018eb0: 4e6f 6e65 0a09 7572 6c3a 4f70 7469 6f6e  None..url:Option
-00018ec0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-00018ed0: 6c69 6e6b 3a4f 7074 696f 6e61 6c5b 2242  link:Optional["B
-00018ee0: 6173 654c 696e 6b22 5d20 3d20 4e6f 6e65  aseLink"] = None
-00018ef0: 0a0a 0a63 6c61 7373 2057 616c 6c50 6f73  ...class WallPos
-00018f00: 7465 6450 686f 746f 2842 4d29 3a0a 0969  tedPhoto(BM):..i
-00018f10: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
-00018f20: 3d20 4e6f 6e65 0a09 6f77 6e65 725f 6964  = None..owner_id
-00018f30: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00018f40: 204e 6f6e 650a 0970 686f 746f 5f31 3330   None..photo_130
-00018f50: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00018f60: 204e 6f6e 650a 0970 686f 746f 5f36 3034   None..photo_604
-00018f70: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-00018f80: 204e 6f6e 650a 0a0a 636c 6173 7320 5761   None...class Wa
-00018f90: 6c6c 5669 6577 7328 424d 293a 0a09 636f  llViews(BM):..co
-00018fa0: 756e 743a 4f70 7469 6f6e 616c 5b69 6e74  unt:Optional[int
-00018fb0: 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61 7373  ] = None...class
-00018fc0: 2057 616c 6c57 616c 6c43 6f6d 6d65 6e74   WallWallComment
-00018fd0: 2842 4d29 3a0a 0969 643a 696e 740a 0966  (BM):..id:int..f
-00018fe0: 726f 6d5f 6964 3a69 6e74 0a09 6361 6e5f  rom_id:int..can_
-00018ff0: 6564 6974 3a4f 7074 696f 6e61 6c5b 626f  edit:Optional[bo
-00019000: 6f6c 5d20 3d20 4e6f 6e65 0a09 706f 7374  ol] = None..post
-00019010: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-00019020: 5d20 3d20 4e6f 6e65 0a09 6f77 6e65 725f  ] = None..owner_
-00019030: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-00019040: 203d 204e 6f6e 650a 0970 6172 656e 7473   = None..parents
-00019050: 5f73 7461 636b 3a4f 7074 696f 6e61 6c5b  _stack:Optional[
-00019060: 6c69 7374 5b69 6e74 5d5d 203d 204e 6f6e  list[int]] = Non
-00019070: 650a 0970 686f 746f 5f69 643a 4f70 7469  e..photo_id:Opti
-00019080: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00019090: 0a09 7669 6465 6f5f 6964 3a4f 7074 696f  ..video_id:Optio
-000190a0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-000190b0: 0964 6174 653a 696e 740a 0974 6578 743a  .date:int..text:
-000190c0: 7374 720a 0961 7474 6163 686d 656e 7473  str..attachments
-000190d0: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
-000190e0: 5761 6c6c 436f 6d6d 656e 7441 7474 6163  WallCommentAttac
-000190f0: 686d 656e 7422 5d5d 203d 204e 6f6e 650a  hment"]] = None.
-00019100: 0964 6f6e 7574 3a4f 7074 696f 6e61 6c5b  .donut:Optional[
-00019110: 2257 616c 6c57 616c 6c43 6f6d 6d65 6e74  "WallWallComment
-00019120: 446f 6e75 7422 5d20 3d20 4e6f 6e65 0a09  Donut"] = None..
-00019130: 6c69 6b65 733a 4f70 7469 6f6e 616c 5b22  likes:Optional["
-00019140: 4261 7365 4c69 6b65 7349 6e66 6f22 5d20  BaseLikesInfo"] 
-00019150: 3d20 4e6f 6e65 0a09 7265 616c 5f6f 6666  = None..real_off
-00019160: 7365 743a 4f70 7469 6f6e 616c 5b69 6e74  set:Optional[int
-00019170: 5d20 3d20 4e6f 6e65 0a09 7265 706c 795f  ] = None..reply_
-00019180: 746f 5f75 7365 723a 4f70 7469 6f6e 616c  to_user:Optional
-00019190: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7265  [int] = None..re
-000191a0: 706c 795f 746f 5f63 6f6d 6d65 6e74 3a4f  ply_to_comment:O
-000191b0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000191c0: 6f6e 650a 0974 6872 6561 643a 4f70 7469  one..thread:Opti
-000191d0: 6f6e 616c 5b22 436f 6d6d 656e 7454 6872  onal["CommentThr
-000191e0: 6561 6422 5d20 3d20 4e6f 6e65 0a09 6465  ead"] = None..de
-000191f0: 6c65 7465 643a 4f70 7469 6f6e 616c 5b62  leted:Optional[b
-00019200: 6f6f 6c5d 203d 204e 6f6e 650a 0970 6964  ool] = None..pid
-00019210: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00019220: 204e 6f6e 650a 0a0a 636c 6173 7320 5761   None...class Wa
-00019230: 6c6c 5761 6c6c 436f 6d6d 656e 7444 6f6e  llWallCommentDon
-00019240: 7574 2842 4d29 3a0a 0969 735f 646f 6e3a  ut(BM):..is_don:
-00019250: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00019260: 204e 6f6e 650a 0970 6c61 6365 686f 6c64   None..placehold
-00019270: 6572 3a4f 7074 696f 6e61 6c5b 2257 616c  er:Optional["Wal
-00019280: 6c57 616c 6c43 6f6d 6d65 6e74 446f 6e75  lWallCommentDonu
-00019290: 7450 6c61 6365 686f 6c64 6572 225d 203d  tPlaceholder"] =
-000192a0: 204e 6f6e 650a 0a0a 636c 6173 7320 5761   None...class Wa
-000192b0: 6c6c 5761 6c6c 436f 6d6d 656e 7444 6f6e  llWallCommentDon
-000192c0: 7574 506c 6163 6568 6f6c 6465 7228 424d  utPlaceholder(BM
-000192d0: 293a 0a09 7465 7874 3a73 7472 0a0a 0a63  ):..text:str...c
-000192e0: 6c61 7373 2057 616c 6c57 616c 6c70 6f73  lass WallWallpos
-000192f0: 7428 424d 293a 0a09 6163 6365 7373 5f6b  t(BM):..access_k
-00019300: 6579 3a4f 7074 696f 6e61 6c5b 7374 725d  ey:Optional[str]
-00019310: 203d 204e 6f6e 650a 0969 735f 6465 6c65   = None..is_dele
-00019320: 7465 643a 4f70 7469 6f6e 616c 5b62 6f6f  ted:Optional[boo
-00019330: 6c5d 203d 204e 6f6e 650a 0961 7474 6163  l] = None..attac
-00019340: 686d 656e 7473 3a4f 7074 696f 6e61 6c5b  hments:Optional[
-00019350: 6c69 7374 5b22 5761 6c6c 5761 6c6c 706f  list["WallWallpo
-00019360: 7374 4174 7461 6368 6d65 6e74 225d 5d20  stAttachment"]] 
-00019370: 3d20 4e6f 6e65 0a09 636f 7079 7269 6768  = None..copyrigh
-00019380: 743a 4f70 7469 6f6e 616c 5b22 5761 6c6c  t:Optional["Wall
-00019390: 506f 7374 436f 7079 7269 6768 7422 5d20  PostCopyright"] 
-000193a0: 3d20 4e6f 6e65 0a09 6461 7465 3a4f 7074  = None..date:Opt
-000193b0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-000193c0: 650a 0965 6469 7465 643a 4f70 7469 6f6e  e..edited:Option
-000193d0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-000193e0: 6672 6f6d 5f69 643a 4f70 7469 6f6e 616c  from_id:Optional
-000193f0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6765  [int] = None..ge
-00019400: 6f3a 4f70 7469 6f6e 616c 5b22 5761 6c6c  o:Optional["Wall
-00019410: 4765 6f22 5d20 3d20 4e6f 6e65 0a09 6964  Geo"] = None..id
-00019420: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00019430: 204e 6f6e 650a 0969 735f 6172 6368 6976   None..is_archiv
-00019440: 6564 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ed:Optional[bool
-00019450: 5d20 3d20 4e6f 6e65 0a09 6973 5f66 6176  ] = None..is_fav
-00019460: 6f72 6974 653a 4f70 7469 6f6e 616c 5b62  orite:Optional[b
-00019470: 6f6f 6c5d 203d 204e 6f6e 650a 096c 696b  ool] = None..lik
-00019480: 6573 3a4f 7074 696f 6e61 6c5b 2242 6173  es:Optional["Bas
-00019490: 654c 696b 6573 496e 666f 225d 203d 204e  eLikesInfo"] = N
-000194a0: 6f6e 650a 096f 776e 6572 5f69 643a 4f70  one..owner_id:Op
-000194b0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000194c0: 6e65 0a09 706f 7374 5f69 643a 4f70 7469  ne..post_id:Opti
-000194d0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000194e0: 0a09 7061 7265 6e74 735f 7374 6163 6b3a  ..parents_stack:
-000194f0: 4f70 7469 6f6e 616c 5b6c 6973 745b 696e  Optional[list[in
-00019500: 745d 5d20 3d20 4e6f 6e65 0a09 706f 7374  t]] = None..post
-00019510: 5f73 6f75 7263 653a 4f70 7469 6f6e 616c  _source:Optional
-00019520: 5b22 5761 6c6c 506f 7374 536f 7572 6365  ["WallPostSource
-00019530: 225d 203d 204e 6f6e 650a 0970 6f73 745f  "] = None..post_
-00019540: 7479 7065 3a4f 7074 696f 6e61 6c5b 2257  type:Optional["W
-00019550: 616c 6c50 6f73 7454 7970 6522 5d20 3d20  allPostType"] = 
-00019560: 4e6f 6e65 0a09 7265 706f 7374 733a 4f70  None..reposts:Op
-00019570: 7469 6f6e 616c 5b22 4261 7365 5265 706f  tional["BaseRepo
-00019580: 7374 7349 6e66 6f22 5d20 3d20 4e6f 6e65  stsInfo"] = None
-00019590: 0a09 7369 676e 6572 5f69 643a 4f70 7469  ..signer_id:Opti
-000195a0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-000195b0: 0a09 7465 7874 3a4f 7074 696f 6e61 6c5b  ..text:Optional[
-000195c0: 7374 725d 203d 204e 6f6e 650a 0976 6965  str] = None..vie
-000195d0: 7773 3a4f 7074 696f 6e61 6c5b 2257 616c  ws:Optional["Wal
-000195e0: 6c56 6965 7773 225d 203d 204e 6f6e 650a  lViews"] = None.
-000195f0: 0a0a 636c 6173 7320 5761 6c6c 5761 6c6c  ..class WallWall
-00019600: 706f 7374 4174 7461 6368 6d65 6e74 2842  postAttachment(B
-00019610: 4d29 3a0a 0961 6363 6573 735f 6b65 793a  M):..access_key:
-00019620: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00019630: 4e6f 6e65 0a09 616c 6275 6d3a 4f70 7469  None..album:Opti
-00019640: 6f6e 616c 5b22 5068 6f74 6f73 5068 6f74  onal["PhotosPhot
-00019650: 6f41 6c62 756d 225d 203d 204e 6f6e 650a  oAlbum"] = None.
-00019660: 0961 7070 3a4f 7074 696f 6e61 6c5b 2257  .app:Optional["W
-00019670: 616c 6c41 7070 506f 7374 225d 203d 204e  allAppPost"] = N
-00019680: 6f6e 650a 0961 7564 696f 3a4f 7074 696f  one..audio:Optio
-00019690: 6e61 6c5b 2241 7564 696f 4175 6469 6f22  nal["AudioAudio"
-000196a0: 5d20 3d20 4e6f 6e65 0a09 646f 633a 4f70  ] = None..doc:Op
-000196b0: 7469 6f6e 616c 5b22 446f 6373 446f 6322  tional["DocsDoc"
-000196c0: 5d20 3d20 4e6f 6e65 0a09 6576 656e 743a  ] = None..event:
-000196d0: 4f70 7469 6f6e 616c 5b22 4576 656e 7473  Optional["Events
-000196e0: 4576 656e 7441 7474 6163 6822 5d20 3d20  EventAttach"] = 
-000196f0: 4e6f 6e65 0a09 6772 6f75 703a 4f70 7469  None..group:Opti
-00019700: 6f6e 616c 5b22 4772 6f75 7073 4772 6f75  onal["GroupsGrou
-00019710: 7041 7474 6163 6822 5d20 3d20 4e6f 6e65  pAttach"] = None
-00019720: 0a09 6772 6166 6669 7469 3a4f 7074 696f  ..graffiti:Optio
-00019730: 6e61 6c5b 2257 616c 6c47 7261 6666 6974  nal["WallGraffit
-00019740: 6922 5d20 3d20 4e6f 6e65 0a09 6c69 6e6b  i"] = None..link
-00019750: 3a4f 7074 696f 6e61 6c5b 2242 6173 654c  :Optional["BaseL
-00019760: 696e 6b22 5d20 3d20 4e6f 6e65 0a09 6d61  ink"] = None..ma
-00019770: 726b 6574 3a4f 7074 696f 6e61 6c5b 224d  rket:Optional["M
-00019780: 6172 6b65 744d 6172 6b65 7449 7465 6d22  arketMarketItem"
-00019790: 5d20 3d20 4e6f 6e65 0a09 6d61 726b 6574  ] = None..market
-000197a0: 5f61 6c62 756d 3a4f 7074 696f 6e61 6c5b  _album:Optional[
-000197b0: 224d 6172 6b65 744d 6172 6b65 7441 6c62  "MarketMarketAlb
-000197c0: 756d 225d 203d 204e 6f6e 650a 096e 6f74  um"] = None..not
-000197d0: 653a 4f70 7469 6f6e 616c 5b22 4e6f 7465  e:Optional["Note
-000197e0: 734e 6f74 6522 5d20 3d20 4e6f 6e65 0a09  sNote"] = None..
-000197f0: 7061 6765 3a4f 7074 696f 6e61 6c5b 2250  page:Optional["P
-00019800: 6167 6573 5769 6b69 7061 6765 4675 6c6c  agesWikipageFull
-00019810: 225d 203d 204e 6f6e 650a 0970 686f 746f  "] = None..photo
-00019820: 3a4f 7074 696f 6e61 6c5b 2250 686f 746f  :Optional["Photo
-00019830: 7350 686f 746f 225d 203d 204e 6f6e 650a  sPhoto"] = None.
-00019840: 0970 6f6c 6c3a 4f70 7469 6f6e 616c 5b22  .poll:Optional["
-00019850: 506f 6c6c 7350 6f6c 6c22 5d20 3d20 4e6f  PollsPoll"] = No
-00019860: 6e65 0a09 706f 7374 6564 5f70 686f 746f  ne..posted_photo
-00019870: 3a4f 7074 696f 6e61 6c5b 2257 616c 6c50  :Optional["WallP
-00019880: 6f73 7465 6450 686f 746f 225d 203d 204e  ostedPhoto"] = N
-00019890: 6f6e 650a 0974 7970 653a 2257 616c 6c57  one..type:"WallW
-000198a0: 616c 6c70 6f73 7441 7474 6163 686d 656e  allpostAttachmen
-000198b0: 7454 7970 6522 0a09 7669 6465 6f3a 4f70  tType"..video:Op
-000198c0: 7469 6f6e 616c 5b22 5669 6465 6f56 6964  tional["VideoVid
-000198d0: 656f 4675 6c6c 225d 203d 204e 6f6e 650a  eoFull"] = None.
-000198e0: 0a0a 636c 6173 7320 5761 6c6c 5761 6c6c  ..class WallWall
-000198f0: 706f 7374 436f 6d6d 656e 7473 446f 6e75  postCommentsDonu
-00019900: 7428 424d 293a 0a09 706c 6163 6568 6f6c  t(BM):..placehol
-00019910: 6465 723a 4f70 7469 6f6e 616c 5b22 5761  der:Optional["Wa
-00019920: 6c6c 5761 6c6c 706f 7374 436f 6d6d 656e  llWallpostCommen
-00019930: 7473 446f 6e75 7450 6c61 6365 686f 6c64  tsDonutPlacehold
-00019940: 6572 225d 203d 204e 6f6e 650a 0a0a 636c  er"] = None...cl
-00019950: 6173 7320 5761 6c6c 5761 6c6c 706f 7374  ass WallWallpost
-00019960: 436f 6d6d 656e 7473 446f 6e75 7450 6c61  CommentsDonutPla
-00019970: 6365 686f 6c64 6572 2842 4d29 3a0a 0974  ceholder(BM):..t
-00019980: 6578 743a 7374 720a 0a0a 636c 6173 7320  ext:str...class 
-00019990: 5761 6c6c 5761 6c6c 706f 7374 446f 6e75  WallWallpostDonu
-000199a0: 7428 424d 293a 0a09 6973 5f64 6f6e 7574  t(BM):..is_donut
-000199b0: 3a62 6f6f 6c0a 0970 6169 645f 6475 7261  :bool..paid_dura
-000199c0: 7469 6f6e 3a4f 7074 696f 6e61 6c5b 696e  tion:Optional[in
-000199d0: 745d 203d 204e 6f6e 650a 0970 6c61 6365  t] = None..place
-000199e0: 686f 6c64 6572 3a4f 7074 696f 6e61 6c5b  holder:Optional[
-000199f0: 2257 616c 6c57 616c 6c70 6f73 7444 6f6e  "WallWallpostDon
-00019a00: 7574 506c 6163 6568 6f6c 6465 7222 5d20  utPlaceholder"] 
-00019a10: 3d20 4e6f 6e65 0a09 6361 6e5f 7075 626c  = None..can_publ
-00019a20: 6973 685f 6672 6565 5f63 6f70 793a 4f70  ish_free_copy:Op
-00019a30: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-00019a40: 6f6e 650a 0965 6469 745f 6d6f 6465 3a4f  one..edit_mode:O
-00019a50: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00019a60: 6f6e 650a 0a0a 636c 6173 7320 5761 6c6c  one...class Wall
-00019a70: 5761 6c6c 706f 7374 446f 6e75 7450 6c61  WallpostDonutPla
-00019a80: 6365 686f 6c64 6572 2842 4d29 3a0a 0974  ceholder(BM):..t
-00019a90: 6578 743a 7374 720a 0a0a 636c 6173 7320  ext:str...class 
-00019aa0: 5761 6c6c 5761 6c6c 706f 7374 546f 4964  WallWallpostToId
-00019ab0: 2842 4d29 3a0a 0961 7474 6163 686d 656e  (BM):..attachmen
-00019ac0: 7473 3a4f 7074 696f 6e61 6c5b 6c69 7374  ts:Optional[list
-00019ad0: 5b22 5761 6c6c 5761 6c6c 706f 7374 4174  ["WallWallpostAt
-00019ae0: 7461 6368 6d65 6e74 225d 5d20 3d20 4e6f  tachment"]] = No
-00019af0: 6e65 0a09 636f 6d6d 656e 7473 3a4f 7074  ne..comments:Opt
-00019b00: 696f 6e61 6c5b 2242 6173 6543 6f6d 6d65  ional["BaseComme
-00019b10: 6e74 7349 6e66 6f22 5d20 3d20 4e6f 6e65  ntsInfo"] = None
-00019b20: 0a09 636f 7079 5f6f 776e 6572 5f69 643a  ..copy_owner_id:
-00019b30: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00019b40: 4e6f 6e65 0a09 636f 7079 5f70 6f73 745f  None..copy_post_
-00019b50: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-00019b60: 203d 204e 6f6e 650a 0964 6174 653a 4f70   = None..date:Op
-00019b70: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00019b80: 6e65 0a09 6672 6f6d 5f69 643a 4f70 7469  ne..from_id:Opti
-00019b90: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00019ba0: 0a09 6765 6f3a 4f70 7469 6f6e 616c 5b22  ..geo:Optional["
-00019bb0: 5761 6c6c 4765 6f22 5d20 3d20 4e6f 6e65  WallGeo"] = None
-00019bc0: 0a09 6964 3a4f 7074 696f 6e61 6c5b 696e  ..id:Optional[in
-00019bd0: 745d 203d 204e 6f6e 650a 0969 735f 6661  t] = None..is_fa
-00019be0: 766f 7269 7465 3a4f 7074 696f 6e61 6c5b  vorite:Optional[
-00019bf0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6c69  bool] = None..li
-00019c00: 6b65 733a 4f70 7469 6f6e 616c 5b22 4261  kes:Optional["Ba
-00019c10: 7365 4c69 6b65 7349 6e66 6f22 5d20 3d20  seLikesInfo"] = 
-00019c20: 4e6f 6e65 0a09 706f 7374 5f69 643a 4f70  None..post_id:Op
-00019c30: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00019c40: 6e65 0a09 706f 7374 5f73 6f75 7263 653a  ne..post_source:
-00019c50: 4f70 7469 6f6e 616c 5b22 5761 6c6c 506f  Optional["WallPo
-00019c60: 7374 536f 7572 6365 225d 203d 204e 6f6e  stSource"] = Non
-00019c70: 650a 0970 6f73 745f 7479 7065 3a4f 7074  e..post_type:Opt
-00019c80: 696f 6e61 6c5b 2257 616c 6c50 6f73 7454  ional["WallPostT
-00019c90: 7970 6522 5d20 3d20 4e6f 6e65 0a09 7265  ype"] = None..re
-00019ca0: 706f 7374 733a 4f70 7469 6f6e 616c 5b22  posts:Optional["
-00019cb0: 4261 7365 5265 706f 7374 7349 6e66 6f22  BaseRepostsInfo"
-00019cc0: 5d20 3d20 4e6f 6e65 0a09 7369 676e 6572  ] = None..signer
-00019cd0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-00019ce0: 5d20 3d20 4e6f 6e65 0a09 7465 7874 3a4f  ] = None..text:O
-00019cf0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00019d00: 6f6e 650a 0974 6f5f 6964 3a4f 7074 696f  one..to_id:Optio
-00019d10: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-00019d20: 0a0a 0a0a 636c 6173 7320 5769 6467 6574  ....class Widget
-00019d30: 7343 6f6d 6d65 6e74 4d65 6469 6154 7970  sCommentMediaTyp
-00019d40: 6528 456e 756d 293a 0a09 4155 4449 4f20  e(Enum):..AUDIO 
-00019d50: 3d20 2261 7564 696f 220a 0950 484f 544f  = "audio"..PHOTO
-00019d60: 203d 2022 7068 6f74 6f22 0a09 5649 4445   = "photo"..VIDE
-00019d70: 4f20 3d20 2276 6964 656f 220a 0a63 6c61  O = "video"..cla
-00019d80: 7373 2057 6964 6765 7473 436f 6d6d 656e  ss WidgetsCommen
-00019d90: 744d 6564 6961 2842 4d29 3a0a 0969 7465  tMedia(BM):..ite
-00019da0: 6d5f 6964 3a4f 7074 696f 6e61 6c5b 696e  m_id:Optional[in
-00019db0: 745d 203d 204e 6f6e 650a 096f 776e 6572  t] = None..owner
-00019dc0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-00019dd0: 5d20 3d20 4e6f 6e65 0a09 7468 756d 625f  ] = None..thumb_
-00019de0: 7372 633a 4f70 7469 6f6e 616c 5b73 7472  src:Optional[str
-00019df0: 5d20 3d20 4e6f 6e65 0a09 7479 7065 3a4f  ] = None..type:O
-00019e00: 7074 696f 6e61 6c5b 2257 6964 6765 7473  ptional["Widgets
-00019e10: 436f 6d6d 656e 744d 6564 6961 5479 7065  CommentMediaType
-00019e20: 225d 203d 204e 6f6e 650a 0a0a 636c 6173  "] = None...clas
-00019e30: 7320 5769 6467 6574 7343 6f6d 6d65 6e74  s WidgetsComment
-00019e40: 5265 706c 6965 7328 424d 293a 0a09 6361  Replies(BM):..ca
-00019e50: 6e5f 706f 7374 3a4f 7074 696f 6e61 6c5b  n_post:Optional[
-00019e60: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 636f  bool] = None..co
-00019e70: 756e 743a 4f70 7469 6f6e 616c 5b69 6e74  unt:Optional[int
-00019e80: 5d20 3d20 4e6f 6e65 0a09 7265 706c 6965  ] = None..replie
-00019e90: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-00019ea0: 2257 6964 6765 7473 436f 6d6d 656e 7452  "WidgetsCommentR
-00019eb0: 6570 6c69 6573 4974 656d 225d 5d20 3d20  epliesItem"]] = 
-00019ec0: 4e6f 6e65 0a0a 0a63 6c61 7373 2057 6964  None...class Wid
-00019ed0: 6765 7473 436f 6d6d 656e 7452 6570 6c69  getsCommentRepli
-00019ee0: 6573 4974 656d 2842 4d29 3a0a 0963 6964  esItem(BM):..cid
-00019ef0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-00019f00: 204e 6f6e 650a 0964 6174 653a 4f70 7469   None..date:Opti
-00019f10: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00019f20: 0a09 6c69 6b65 733a 4f70 7469 6f6e 616c  ..likes:Optional
-00019f30: 5b22 5769 6467 6574 7357 6964 6765 744c  ["WidgetsWidgetL
-00019f40: 696b 6573 225d 203d 204e 6f6e 650a 0974  ikes"] = None..t
-00019f50: 6578 743a 4f70 7469 6f6e 616c 5b73 7472  ext:Optional[str
-00019f60: 5d20 3d20 4e6f 6e65 0a09 7569 643a 4f70  ] = None..uid:Op
-00019f70: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-00019f80: 6e65 0a09 7573 6572 3a4f 7074 696f 6e61  ne..user:Optiona
-00019f90: 6c5b 2255 7365 7273 5573 6572 4675 6c6c  l["UsersUserFull
-00019fa0: 225d 203d 204e 6f6e 650a 0a0a 636c 6173  "] = None...clas
-00019fb0: 7320 5769 6467 6574 7357 6964 6765 7443  s WidgetsWidgetC
-00019fc0: 6f6d 6d65 6e74 2842 4d29 3a0a 0961 7474  omment(BM):..att
-00019fd0: 6163 686d 656e 7473 3a4f 7074 696f 6e61  achments:Optiona
-00019fe0: 6c5b 6c69 7374 5b22 5761 6c6c 436f 6d6d  l[list["WallComm
-00019ff0: 656e 7441 7474 6163 686d 656e 7422 5d5d  entAttachment"]]
-0001a000: 203d 204e 6f6e 650a 0963 616e 5f64 656c   = None..can_del
-0001a010: 6574 653a 4f70 7469 6f6e 616c 5b62 6f6f  ete:Optional[boo
-0001a020: 6c5d 203d 204e 6f6e 650a 0963 6f6d 6d65  l] = None..comme
-0001a030: 6e74 733a 4f70 7469 6f6e 616c 5b22 5769  nts:Optional["Wi
-0001a040: 6467 6574 7343 6f6d 6d65 6e74 5265 706c  dgetsCommentRepl
-0001a050: 6965 7322 5d20 3d20 4e6f 6e65 0a09 6461  ies"] = None..da
-0001a060: 7465 3a69 6e74 0a09 6672 6f6d 5f69 643a  te:int..from_id:
-0001a070: 696e 740a 0969 643a 696e 740a 096c 696b  int..id:int..lik
-0001a080: 6573 3a4f 7074 696f 6e61 6c5b 2242 6173  es:Optional["Bas
-0001a090: 654c 696b 6573 496e 666f 225d 203d 204e  eLikesInfo"] = N
-0001a0a0: 6f6e 650a 096d 6564 6961 3a4f 7074 696f  one..media:Optio
-0001a0b0: 6e61 6c5b 2257 6964 6765 7473 436f 6d6d  nal["WidgetsComm
-0001a0c0: 656e 744d 6564 6961 225d 203d 204e 6f6e  entMedia"] = Non
-0001a0d0: 650a 0970 6f73 745f 736f 7572 6365 3a4f  e..post_source:O
-0001a0e0: 7074 696f 6e61 6c5b 2257 616c 6c50 6f73  ptional["WallPos
-0001a0f0: 7453 6f75 7263 6522 5d20 3d20 4e6f 6e65  tSource"] = None
-0001a100: 0a09 706f 7374 5f74 7970 653a 696e 740a  ..post_type:int.
-0001a110: 0972 6570 6f73 7473 3a4f 7074 696f 6e61  .reposts:Optiona
-0001a120: 6c5b 2242 6173 6552 6570 6f73 7473 496e  l["BaseRepostsIn
-0001a130: 666f 225d 203d 204e 6f6e 650a 0974 6578  fo"] = None..tex
-0001a140: 743a 7374 720a 0974 6f5f 6964 3a69 6e74  t:str..to_id:int
-0001a150: 0a09 7573 6572 3a4f 7074 696f 6e61 6c5b  ..user:Optional[
-0001a160: 2255 7365 7273 5573 6572 4675 6c6c 225d  "UsersUserFull"]
-0001a170: 203d 204e 6f6e 650a 0a0a 636c 6173 7320   = None...class 
-0001a180: 5769 6467 6574 7357 6964 6765 744c 696b  WidgetsWidgetLik
-0001a190: 6573 2842 4d29 3a0a 0963 6f75 6e74 3a4f  es(BM):..count:O
-0001a1a0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0001a1b0: 6f6e 650a 0a0a 636c 6173 7320 5769 6467  one...class Widg
-0001a1c0: 6574 7357 6964 6765 7450 6167 6528 424d  etsWidgetPage(BM
-0001a1d0: 293a 0a09 636f 6d6d 656e 7473 3a4f 7074  ):..comments:Opt
-0001a1e0: 696f 6e61 6c5b 2242 6173 654f 626a 6563  ional["BaseObjec
-0001a1f0: 7443 6f75 6e74 225d 203d 204e 6f6e 650a  tCount"] = None.
-0001a200: 0964 6174 653a 4f70 7469 6f6e 616c 5b69  .date:Optional[i
-0001a210: 6e74 5d20 3d20 4e6f 6e65 0a09 6465 7363  nt] = None..desc
-0001a220: 7269 7074 696f 6e3a 4f70 7469 6f6e 616c  ription:Optional
-0001a230: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6964  [str] = None..id
-0001a240: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-0001a250: 204e 6f6e 650a 096c 696b 6573 3a4f 7074   None..likes:Opt
-0001a260: 696f 6e61 6c5b 2242 6173 654f 626a 6563  ional["BaseObjec
-0001a270: 7443 6f75 6e74 225d 203d 204e 6f6e 650a  tCount"] = None.
-0001a280: 0970 6167 655f 6964 3a4f 7074 696f 6e61  .page_id:Optiona
-0001a290: 6c5b 7374 725d 203d 204e 6f6e 650a 0970  l[str] = None..p
-0001a2a0: 686f 746f 3a4f 7074 696f 6e61 6c5b 7374  hoto:Optional[st
-0001a2b0: 725d 203d 204e 6f6e 650a 0974 6974 6c65  r] = None..title
-0001a2c0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-0001a2d0: 204e 6f6e 650a 0975 726c 3a4f 7074 696f   None..url:Optio
+00017730: 0975 726c 3a4f 7074 696f 6e61 6c5b 7374  .url:Optional[st
+00017740: 725d 203d 204e 6f6e 650a 0a0a 636c 6173  r] = None...clas
+00017750: 7320 5574 696c 7353 7461 7473 2842 4d29  s UtilsStats(BM)
+00017760: 3a0a 0974 696d 6573 7461 6d70 3a4f 7074  :..timestamp:Opt
+00017770: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00017780: 650a 0976 6965 7773 3a4f 7074 696f 6e61  e..views:Optiona
+00017790: 6c5b 696e 745d 203d 204e 6f6e 650a 0a0a  l[int] = None...
+000177a0: 636c 6173 7320 5574 696c 7353 7461 7473  class UtilsStats
+000177b0: 4369 7479 2842 4d29 3a0a 0963 6974 795f  City(BM):..city_
+000177c0: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
+000177d0: 203d 204e 6f6e 650a 0976 6965 7773 3a4f   = None..views:O
+000177e0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000177f0: 6f6e 650a 0a0a 636c 6173 7320 5574 696c  one...class Util
+00017800: 7353 7461 7473 436f 756e 7472 7928 424d  sStatsCountry(BM
+00017810: 293a 0a09 636f 756e 7472 795f 6964 3a4f  ):..country_id:O
+00017820: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00017830: 6f6e 650a 0976 6965 7773 3a4f 7074 696f  one..views:Optio
+00017840: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00017850: 0a0a 636c 6173 7320 5574 696c 7353 7461  ..class UtilsSta
+00017860: 7473 4578 7465 6e64 6564 2842 4d29 3a0a  tsExtended(BM):.
+00017870: 0963 6974 6965 733a 4f70 7469 6f6e 616c  .cities:Optional
+00017880: 5b6c 6973 745b 2255 7469 6c73 5374 6174  [list["UtilsStat
+00017890: 7343 6974 7922 5d5d 203d 204e 6f6e 650a  sCity"]] = None.
+000178a0: 0963 6f75 6e74 7269 6573 3a4f 7074 696f  .countries:Optio
+000178b0: 6e61 6c5b 6c69 7374 5b22 5574 696c 7353  nal[list["UtilsS
+000178c0: 7461 7473 436f 756e 7472 7922 5d5d 203d  tatsCountry"]] =
+000178d0: 204e 6f6e 650a 0973 6578 5f61 6765 3a4f   None..sex_age:O
+000178e0: 7074 696f 6e61 6c5b 6c69 7374 5b22 5574  ptional[list["Ut
+000178f0: 696c 7353 7461 7473 5365 7841 6765 225d  ilsStatsSexAge"]
+00017900: 5d20 3d20 4e6f 6e65 0a09 7469 6d65 7374  ] = None..timest
+00017910: 616d 703a 4f70 7469 6f6e 616c 5b69 6e74  amp:Optional[int
+00017920: 5d20 3d20 4e6f 6e65 0a09 7669 6577 733a  ] = None..views:
+00017930: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00017940: 4e6f 6e65 0a0a 0a63 6c61 7373 2055 7469  None...class Uti
+00017950: 6c73 5374 6174 7353 6578 4167 6528 424d  lsStatsSexAge(BM
+00017960: 293a 0a09 6167 655f 7261 6e67 653a 4f70  ):..age_range:Op
+00017970: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00017980: 6e65 0a09 6665 6d61 6c65 3a4f 7074 696f  ne..female:Optio
+00017990: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+000179a0: 096d 616c 653a 4f70 7469 6f6e 616c 5b69  .male:Optional[i
+000179b0: 6e74 5d20 3d20 4e6f 6e65 0a0a 0a0a 0a63  nt] = None.....c
+000179c0: 6c61 7373 2056 6964 656f 4c69 7665 496e  lass VideoLiveIn
+000179d0: 666f 2842 4d29 3a0a 0965 6e61 626c 6564  fo(BM):..enabled
+000179e0: 3a62 6f6f 6c0a 0969 735f 6e6f 7469 6669  :bool..is_notifi
+000179f0: 6361 7469 6f6e 735f 626c 6f63 6b65 643a  cations_blocked:
+00017a00: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00017a10: 204e 6f6e 650a 0a0a 636c 6173 7320 5669   None...class Vi
+00017a20: 6465 6f4c 6976 6553 6574 7469 6e67 7328  deoLiveSettings(
+00017a30: 424d 293a 0a09 6361 6e5f 7265 7769 6e64  BM):..can_rewind
+00017a40: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+00017a50: 3d20 4e6f 6e65 0a09 6973 5f65 6e64 6c65  = None..is_endle
+00017a60: 7373 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ss:Optional[bool
+00017a70: 5d20 3d20 4e6f 6e65 0a09 6d61 785f 6475  ] = None..max_du
+00017a80: 7261 7469 6f6e 3a4f 7074 696f 6e61 6c5b  ration:Optional[
+00017a90: 696e 745d 203d 204e 6f6e 650a 0a0a 636c  int] = None...cl
+00017aa0: 6173 7320 5669 6465 6f53 6176 6552 6573  ass VideoSaveRes
+00017ab0: 756c 7428 424d 293a 0a09 6163 6365 7373  ult(BM):..access
+00017ac0: 5f6b 6579 3a4f 7074 696f 6e61 6c5b 7374  _key:Optional[st
+00017ad0: 725d 203d 204e 6f6e 650a 0964 6573 6372  r] = None..descr
+00017ae0: 6970 7469 6f6e 3a4f 7074 696f 6e61 6c5b  iption:Optional[
+00017af0: 7374 725d 203d 204e 6f6e 650a 096f 776e  str] = None..own
+00017b00: 6572 5f69 643a 4f70 7469 6f6e 616c 5b69  er_id:Optional[i
+00017b10: 6e74 5d20 3d20 4e6f 6e65 0a09 7469 746c  nt] = None..titl
+00017b20: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
+00017b30: 3d20 4e6f 6e65 0a09 7570 6c6f 6164 5f75  = None..upload_u
+00017b40: 726c 3a4f 7074 696f 6e61 6c5b 7374 725d  rl:Optional[str]
+00017b50: 203d 204e 6f6e 650a 0976 6964 656f 5f69   = None..video_i
+00017b60: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+00017b70: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2056  = None...class V
+00017b80: 6964 656f 5669 6465 6f28 424d 293a 0a09  ideoVideo(BM):..
+00017b90: 6163 6365 7373 5f6b 6579 3a4f 7074 696f  access_key:Optio
+00017ba0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00017bb0: 0961 6464 696e 675f 6461 7465 3a4f 7074  .adding_date:Opt
+00017bc0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00017bd0: 650a 0963 616e 5f63 6f6d 6d65 6e74 3a4f  e..can_comment:O
+00017be0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00017bf0: 4e6f 6e65 0a09 6361 6e5f 6564 6974 3a4f  None..can_edit:O
+00017c00: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00017c10: 4e6f 6e65 0a09 6361 6e5f 6c69 6b65 3a4f  None..can_like:O
+00017c20: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00017c30: 4e6f 6e65 0a09 6361 6e5f 7265 706f 7374  None..can_repost
+00017c40: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+00017c50: 3d20 4e6f 6e65 0a09 6361 6e5f 7375 6273  = None..can_subs
+00017c60: 6372 6962 653a 4f70 7469 6f6e 616c 5b62  cribe:Optional[b
+00017c70: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
+00017c80: 5f61 6464 5f74 6f5f 6661 7665 733a 4f70  _add_to_faves:Op
+00017c90: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+00017ca0: 6f6e 650a 0963 616e 5f61 6464 3a4f 7074  one..can_add:Opt
+00017cb0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00017cc0: 6e65 0a09 6361 6e5f 6174 7461 6368 5f6c  ne..can_attach_l
+00017cd0: 696e 6b3a 4f70 7469 6f6e 616c 5b62 6f6f  ink:Optional[boo
+00017ce0: 6c5d 203d 204e 6f6e 650a 0969 735f 7072  l] = None..is_pr
+00017cf0: 6976 6174 653a 4f70 7469 6f6e 616c 5b62  ivate:Optional[b
+00017d00: 6f6f 6c5d 203d 204e 6f6e 650a 0963 6f6d  ool] = None..com
+00017d10: 6d65 6e74 733a 4f70 7469 6f6e 616c 5b69  ments:Optional[i
+00017d20: 6e74 5d20 3d20 4e6f 6e65 0a09 6461 7465  nt] = None..date
+00017d30: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00017d40: 204e 6f6e 650a 0964 6573 6372 6970 7469   None..descripti
+00017d50: 6f6e 3a4f 7074 696f 6e61 6c5b 7374 725d  on:Optional[str]
+00017d60: 203d 204e 6f6e 650a 0964 7572 6174 696f   = None..duratio
+00017d70: 6e3a 4f70 7469 6f6e 616c 5b69 6e74 5d20  n:Optional[int] 
+00017d80: 3d20 4e6f 6e65 0a09 696d 6167 653a 4f70  = None..image:Op
+00017d90: 7469 6f6e 616c 5b6c 6973 745b 2256 6964  tional[list["Vid
+00017da0: 656f 5669 6465 6f49 6d61 6765 225d 5d20  eoVideoImage"]] 
+00017db0: 3d20 4e6f 6e65 0a09 6669 7273 745f 6672  = None..first_fr
+00017dc0: 616d 653a 4f70 7469 6f6e 616c 5b6c 6973  ame:Optional[lis
+00017dd0: 745b 2256 6964 656f 5669 6465 6f49 6d61  t["VideoVideoIma
+00017de0: 6765 225d 5d20 3d20 4e6f 6e65 0a09 7769  ge"]] = None..wi
+00017df0: 6474 683a 4f70 7469 6f6e 616c 5b69 6e74  dth:Optional[int
+00017e00: 5d20 3d20 4e6f 6e65 0a09 6865 6967 6874  ] = None..height
+00017e10: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00017e20: 204e 6f6e 650a 0969 643a 4f70 7469 6f6e   None..id:Option
+00017e30: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00017e40: 6f77 6e65 725f 6964 3a4f 7074 696f 6e61  owner_id:Optiona
+00017e50: 6c5b 696e 745d 203d 204e 6f6e 650a 0975  l[int] = None..u
+00017e60: 7365 725f 6964 3a4f 7074 696f 6e61 6c5b  ser_id:Optional[
+00017e70: 696e 745d 203d 204e 6f6e 650a 0974 6974  int] = None..tit
+00017e80: 6c65 3a4f 7074 696f 6e61 6c5b 7374 725d  le:Optional[str]
+00017e90: 203d 204e 6f6e 650a 0969 735f 6661 766f   = None..is_favo
+00017ea0: 7269 7465 3a4f 7074 696f 6e61 6c5b 626f  rite:Optional[bo
+00017eb0: 6f6c 5d20 3d20 4e6f 6e65 0a09 706c 6179  ol] = None..play
+00017ec0: 6572 3a4f 7074 696f 6e61 6c5b 7374 725d  er:Optional[str]
+00017ed0: 203d 204e 6f6e 650a 0970 726f 6365 7373   = None..process
+00017ee0: 696e 673a 4f70 7469 6f6e 616c 5b22 4261  ing:Optional["Ba
+00017ef0: 7365 5072 6f70 6572 7479 4578 6973 7473  sePropertyExists
+00017f00: 225d 203d 204e 6f6e 650a 0963 6f6e 7665  "] = None..conve
+00017f10: 7274 696e 673a 4f70 7469 6f6e 616c 5b62  rting:Optional[b
+00017f20: 6f6f 6c5d 203d 204e 6f6e 650a 0961 6464  ool] = None..add
+00017f30: 6564 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ed:Optional[bool
+00017f40: 5d20 3d20 4e6f 6e65 0a09 6973 5f73 7562  ] = None..is_sub
+00017f50: 7363 7269 6265 643a 4f70 7469 6f6e 616c  scribed:Optional
+00017f60: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0974  [bool] = None..t
+00017f70: 7261 636b 5f63 6f64 653a 4f70 7469 6f6e  rack_code:Option
+00017f80: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00017f90: 7265 7065 6174 3a4f 7074 696f 6e61 6c5b  repeat:Optional[
+00017fa0: 2242 6173 6550 726f 7065 7274 7945 7869  "BasePropertyExi
+00017fb0: 7374 7322 5d20 3d20 4e6f 6e65 0a09 7479  sts"] = None..ty
+00017fc0: 7065 3a4f 7074 696f 6e61 6c5b 7374 725d  pe:Optional[str]
+00017fd0: 203d 204e 6f6e 650a 0976 6965 7773 3a4f   = None..views:O
+00017fe0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00017ff0: 6f6e 650a 096c 6f63 616c 5f76 6965 7773  one..local_views
+00018000: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00018010: 204e 6f6e 650a 0963 6f6e 7465 6e74 5f72   None..content_r
+00018020: 6573 7472 6963 7465 643a 4f70 7469 6f6e  estricted:Option
+00018030: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00018040: 636f 6e74 656e 745f 7265 7374 7269 6374  content_restrict
+00018050: 6564 5f6d 6573 7361 6765 3a4f 7074 696f  ed_message:Optio
+00018060: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00018070: 0962 616c 616e 6365 3a4f 7074 696f 6e61  .balance:Optiona
+00018080: 6c5b 696e 745d 203d 204e 6f6e 650a 096c  l[int] = None..l
+00018090: 6976 655f 7374 6174 7573 3a4f 7074 696f  ive_status:Optio
+000180a0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+000180b0: 096c 6976 653a 4f70 7469 6f6e 616c 5b22  .live:Optional["
+000180c0: 4261 7365 5072 6f70 6572 7479 4578 6973  BasePropertyExis
+000180d0: 7473 225d 203d 204e 6f6e 650a 0975 7063  ts"] = None..upc
+000180e0: 6f6d 696e 673a 4f70 7469 6f6e 616c 5b22  oming:Optional["
+000180f0: 4261 7365 5072 6f70 6572 7479 4578 6973  BasePropertyExis
+00018100: 7473 225d 203d 204e 6f6e 650a 096c 6976  ts"] = None..liv
+00018110: 655f 7374 6172 745f 7469 6d65 3a4f 7074  e_start_time:Opt
+00018120: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00018130: 650a 096c 6976 655f 6e6f 7469 6679 3a4f  e..live_notify:O
+00018140: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00018150: 4e6f 6e65 0a09 7370 6563 7461 746f 7273  None..spectators
+00018160: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00018170: 204e 6f6e 650a 0970 6c61 7466 6f72 6d3a   None..platform:
+00018180: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00018190: 4e6f 6e65 0a09 6c69 6b65 733a 4f70 7469  None..likes:Opti
+000181a0: 6f6e 616c 5b22 4261 7365 4c69 6b65 7322  onal["BaseLikes"
+000181b0: 5d20 3d20 4e6f 6e65 0a09 7265 706f 7374  ] = None..repost
+000181c0: 733a 4f70 7469 6f6e 616c 5b22 4261 7365  s:Optional["Base
+000181d0: 5265 706f 7374 7349 6e66 6f22 5d20 3d20  RepostsInfo"] = 
+000181e0: 4e6f 6e65 0a0a 0a63 6c61 7373 2056 6964  None...class Vid
+000181f0: 656f 5669 6465 6f41 6c62 756d 2842 4d29  eoVideoAlbum(BM)
+00018200: 3a0a 0969 643a 696e 740a 096f 776e 6572  :..id:int..owner
+00018210: 5f69 643a 696e 740a 0974 6974 6c65 3a73  _id:int..title:s
+00018220: 7472 0a0a 0a63 6c61 7373 2056 6964 656f  tr...class Video
+00018230: 5669 6465 6f46 696c 6573 2842 4d29 3a0a  VideoFiles(BM):.
+00018240: 0965 7874 6572 6e61 6c3a 4f70 7469 6f6e  .external:Option
+00018250: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00018260: 6d70 345f 3134 343a 4f70 7469 6f6e 616c  mp4_144:Optional
+00018270: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6d70  [str] = None..mp
+00018280: 345f 3234 303a 4f70 7469 6f6e 616c 5b73  4_240:Optional[s
+00018290: 7472 5d20 3d20 4e6f 6e65 0a09 6d70 345f  tr] = None..mp4_
+000182a0: 3336 303a 4f70 7469 6f6e 616c 5b73 7472  360:Optional[str
+000182b0: 5d20 3d20 4e6f 6e65 0a09 6d70 345f 3438  ] = None..mp4_48
+000182c0: 303a 4f70 7469 6f6e 616c 5b73 7472 5d20  0:Optional[str] 
+000182d0: 3d20 4e6f 6e65 0a09 6d70 345f 3732 303a  = None..mp4_720:
+000182e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000182f0: 4e6f 6e65 0a09 6d70 345f 3130 3830 3a4f  None..mp4_1080:O
+00018300: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00018310: 6f6e 650a 096d 7034 5f31 3434 303a 4f70  one..mp4_1440:Op
+00018320: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00018330: 6e65 0a09 6d70 345f 3231 3630 3a4f 7074  ne..mp4_2160:Opt
+00018340: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00018350: 650a 0966 6c76 5f33 3230 3a4f 7074 696f  e..flv_320:Optio
+00018360: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00018370: 0a0a 0a0a 636c 6173 7320 5761 6c6c 436f  ....class WallCo
+00018380: 6d6d 656e 7441 7474 6163 686d 656e 7454  mmentAttachmentT
+00018390: 7970 6528 456e 756d 293a 0a09 5048 4f54  ype(Enum):..PHOT
+000183a0: 4f20 3d20 2270 686f 746f 220a 0941 5544  O = "photo"..AUD
+000183b0: 494f 203d 2022 6175 6469 6f22 0a09 5649  IO = "audio"..VI
+000183c0: 4445 4f20 3d20 2276 6964 656f 220a 0944  DEO = "video"..D
+000183d0: 4f43 203d 2022 646f 6322 0a09 4c49 4e4b  OC = "doc"..LINK
+000183e0: 203d 2022 6c69 6e6b 220a 094e 4f54 4520   = "link"..NOTE 
+000183f0: 3d20 226e 6f74 6522 0a09 5041 4745 203d  = "note"..PAGE =
+00018400: 2022 7061 6765 220a 094d 4152 4b45 545f   "page"..MARKET_
+00018410: 4d41 524b 4554 5f41 4c42 554d 203d 2022  MARKET_ALBUM = "
+00018420: 6d61 726b 6574 5f6d 6172 6b65 745f 616c  market_market_al
+00018430: 6275 6d22 0a09 4d41 524b 4554 203d 2022  bum"..MARKET = "
+00018440: 6d61 726b 6574 220a 0953 5449 434b 4552  market"..STICKER
+00018450: 203d 2022 7374 6963 6b65 7222 0a0a 636c   = "sticker"..cl
+00018460: 6173 7320 5761 6c6c 4765 7446 696c 7465  ass WallGetFilte
+00018470: 7228 456e 756d 293a 0a09 4f57 4e45 5220  r(Enum):..OWNER 
+00018480: 3d20 226f 776e 6572 220a 094f 5448 4552  = "owner"..OTHER
+00018490: 5320 3d20 226f 7468 6572 7322 0a09 414c  S = "others"..AL
+000184a0: 4c20 3d20 2261 6c6c 220a 0950 4f53 5450  L = "all"..POSTP
+000184b0: 4f4e 4544 203d 2022 706f 7374 706f 6e65  ONED = "postpone
+000184c0: 6422 0a09 5355 4747 4553 5453 203d 2022  d"..SUGGESTS = "
+000184d0: 7375 6767 6573 7473 220a 0941 5243 4849  suggests"..ARCHI
+000184e0: 5645 4420 3d20 2261 7263 6869 7665 6422  VED = "archived"
+000184f0: 0a09 444f 4e55 5420 3d20 2264 6f6e 7574  ..DONUT = "donut
+00018500: 220a 0a63 6c61 7373 2057 616c 6c50 6f73  "..class WallPos
+00018510: 7453 6f75 7263 6554 7970 6528 456e 756d  tSourceType(Enum
+00018520: 293a 0a09 564b 203d 2022 766b 220a 0957  ):..VK = "vk"..W
+00018530: 4944 4745 5420 3d20 2277 6964 6765 7422  IDGET = "widget"
+00018540: 0a09 4150 4920 3d20 2261 7069 220a 0952  ..API = "api"..R
+00018550: 5353 203d 2022 7273 7322 0a09 534d 5320  SS = "rss"..SMS 
+00018560: 3d20 2273 6d73 220a 094d 564b 203d 2022  = "sms"..MVK = "
+00018570: 6d76 6b22 0a0a 636c 6173 7320 5761 6c6c  mvk"..class Wall
+00018580: 506f 7374 5479 7065 2845 6e75 6d29 3a0a  PostType(Enum):.
+00018590: 0950 4f53 5420 3d20 2270 6f73 7422 0a09  .POST = "post"..
+000185a0: 434f 5059 203d 2022 636f 7079 220a 0952  COPY = "copy"..R
+000185b0: 4550 4c59 203d 2022 7265 706c 7922 0a09  EPLY = "reply"..
+000185c0: 504f 5354 504f 4e45 203d 2022 706f 7374  POSTPONE = "post
+000185d0: 706f 6e65 220a 0953 5547 4745 5354 203d  pone"..SUGGEST =
+000185e0: 2022 7375 6767 6573 7422 0a09 504f 5354   "suggest"..POST
+000185f0: 5f41 4453 203d 2022 706f 7374 5f61 6473  _ADS = "post_ads
+00018600: 220a 0950 484f 544f 203d 2022 7068 6f74  "..PHOTO = "phot
+00018610: 6f22 0a09 5649 4445 4f20 3d20 2276 6964  o"..VIDEO = "vid
+00018620: 656f 220a 0a63 6c61 7373 2057 616c 6c57  eo"..class WallW
+00018630: 616c 6c70 6f73 7441 7474 6163 686d 656e  allpostAttachmen
+00018640: 7454 7970 6528 456e 756d 293a 0a09 5048  tType(Enum):..PH
+00018650: 4f54 4f20 3d20 2270 686f 746f 220a 0950  OTO = "photo"..P
+00018660: 484f 544f 535f 4c49 5354 203d 2022 7068  HOTOS_LIST = "ph
+00018670: 6f74 6f73 5f6c 6973 7422 0a09 504f 5354  otos_list"..POST
+00018680: 4544 5f50 484f 544f 203d 2022 706f 7374  ED_PHOTO = "post
+00018690: 6564 5f70 686f 746f 220a 0941 5544 494f  ed_photo"..AUDIO
+000186a0: 203d 2022 6175 6469 6f22 0a09 4155 4449   = "audio"..AUDI
+000186b0: 4f5f 504c 4159 4c49 5354 203d 2022 6175  O_PLAYLIST = "au
+000186c0: 6469 6f5f 706c 6179 6c69 7374 220a 0956  dio_playlist"..V
+000186d0: 4944 454f 203d 2022 7669 6465 6f22 0a09  IDEO = "video"..
+000186e0: 444f 4320 3d20 2264 6f63 220a 094c 494e  DOC = "doc"..LIN
+000186f0: 4b20 3d20 226c 696e 6b22 0a09 4752 4146  K = "link"..GRAF
+00018700: 4649 5449 203d 2022 6772 6166 6669 7469  FITI = "graffiti
+00018710: 220a 094e 4f54 4520 3d20 226e 6f74 6522  "..NOTE = "note"
+00018720: 0a09 4150 5020 3d20 2261 7070 220a 0950  ..APP = "app"..P
+00018730: 4f4c 4c20 3d20 2270 6f6c 6c22 0a09 5041  OLL = "poll"..PA
+00018740: 4745 203d 2022 7061 6765 220a 0941 4c42  GE = "page"..ALB
+00018750: 554d 203d 2022 616c 6275 6d22 0a09 4d41  UM = "album"..MA
+00018760: 524b 4554 5f41 4c42 554d 203d 2022 6d61  RKET_ALBUM = "ma
+00018770: 726b 6574 5f61 6c62 756d 220a 094d 4152  rket_album"..MAR
+00018780: 4b45 5420 3d20 226d 6172 6b65 7422 0a09  KET = "market"..
+00018790: 4556 454e 5420 3d20 2265 7665 6e74 220a  EVENT = "event".
+000187a0: 0944 4f4e 5554 5f4c 494e 4b20 3d20 2264  .DONUT_LINK = "d
+000187b0: 6f6e 7574 5f6c 696e 6b22 0a09 4152 5449  onut_link"..ARTI
+000187c0: 434c 4520 3d20 2261 7274 6963 6c65 220a  CLE = "article".
+000187d0: 0954 4558 544c 4956 4520 3d20 2274 6578  .TEXTLIVE = "tex
+000187e0: 746c 6976 6522 0a09 5445 5854 504f 5354  tlive"..TEXTPOST
+000187f0: 203d 2022 7465 7874 706f 7374 220a 0954   = "textpost"..T
+00018800: 4558 5450 4f53 545f 5055 424c 4953 4820  EXTPOST_PUBLISH 
+00018810: 3d20 2274 6578 7470 6f73 745f 7075 626c  = "textpost_publ
+00018820: 6973 6822 0a09 5349 5455 4154 494f 4e41  ish"..SITUATIONA
+00018830: 4c5f 5448 454d 4520 3d20 2273 6974 7561  L_THEME = "situa
+00018840: 7469 6f6e 616c 5f74 6865 6d65 220a 0947  tional_theme"..G
+00018850: 524f 5550 203d 2022 6772 6f75 7022 0a09  ROUP = "group"..
+00018860: 5354 4943 4b45 5220 3d20 2273 7469 636b  STICKER = "stick
+00018870: 6572 220a 0950 4f44 4341 5354 203d 2022  er"..PODCAST = "
+00018880: 706f 6463 6173 7422 0a0a 636c 6173 7320  podcast"..class 
+00018890: 5761 6c6c 4170 7050 6f73 7428 424d 293a  WallAppPost(BM):
+000188a0: 0a09 6964 3a4f 7074 696f 6e61 6c5b 696e  ..id:Optional[in
+000188b0: 745d 203d 204e 6f6e 650a 096e 616d 653a  t] = None..name:
+000188c0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000188d0: 4e6f 6e65 0a09 7068 6f74 6f5f 3133 303a  None..photo_130:
+000188e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000188f0: 4e6f 6e65 0a09 7068 6f74 6f5f 3630 343a  None..photo_604:
+00018900: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00018910: 4e6f 6e65 0a0a 0a63 6c61 7373 2057 616c  None...class Wal
+00018920: 6c41 7474 6163 6865 644e 6f74 6528 424d  lAttachedNote(BM
+00018930: 293a 0a09 636f 6d6d 656e 7473 3a69 6e74  ):..comments:int
+00018940: 0a09 6461 7465 3a69 6e74 0a09 6964 3a69  ..date:int..id:i
+00018950: 6e74 0a09 6f77 6e65 725f 6964 3a69 6e74  nt..owner_id:int
+00018960: 0a09 7265 6164 5f63 6f6d 6d65 6e74 733a  ..read_comments:
+00018970: 696e 740a 0974 6974 6c65 3a73 7472 0a09  int..title:str..
+00018980: 7465 7874 3a4f 7074 696f 6e61 6c5b 7374  text:Optional[st
+00018990: 725d 203d 204e 6f6e 650a 0970 7269 7661  r] = None..priva
+000189a0: 6379 5f76 6965 773a 4f70 7469 6f6e 616c  cy_view:Optional
+000189b0: 5b6c 6973 745b 7374 725d 5d20 3d20 4e6f  [list[str]] = No
+000189c0: 6e65 0a09 7072 6976 6163 795f 636f 6d6d  ne..privacy_comm
+000189d0: 656e 743a 4f70 7469 6f6e 616c 5b6c 6973  ent:Optional[lis
+000189e0: 745b 7374 725d 5d20 3d20 4e6f 6e65 0a09  t[str]] = None..
+000189f0: 6361 6e5f 636f 6d6d 656e 743a 4f70 7469  can_comment:Opti
+00018a00: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00018a10: 0a09 7465 7874 5f77 696b 693a 4f70 7469  ..text_wiki:Opti
+00018a20: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00018a30: 0a09 7669 6577 5f75 726c 3a73 7472 0a0a  ..view_url:str..
+00018a40: 0a63 6c61 7373 2057 616c 6c43 6172 6f75  .class WallCarou
+00018a50: 7365 6c42 6173 6528 424d 293a 0a09 6361  selBase(BM):..ca
+00018a60: 726f 7573 656c 5f6f 6666 7365 743a 4f70  rousel_offset:Op
+00018a70: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00018a80: 6e65 0a0a 0a63 6c61 7373 2057 616c 6c43  ne...class WallC
+00018a90: 6f6d 6d65 6e74 4174 7461 6368 6d65 6e74  ommentAttachment
+00018aa0: 2842 4d29 3a0a 0961 7564 696f 3a4f 7074  (BM):..audio:Opt
+00018ab0: 696f 6e61 6c5b 2241 7564 696f 4175 6469  ional["AudioAudi
+00018ac0: 6f22 5d20 3d20 4e6f 6e65 0a09 646f 633a  o"] = None..doc:
+00018ad0: 4f70 7469 6f6e 616c 5b22 446f 6373 446f  Optional["DocsDo
+00018ae0: 6322 5d20 3d20 4e6f 6e65 0a09 6c69 6e6b  c"] = None..link
+00018af0: 3a4f 7074 696f 6e61 6c5b 2242 6173 654c  :Optional["BaseL
+00018b00: 696e 6b22 5d20 3d20 4e6f 6e65 0a09 6d61  ink"] = None..ma
+00018b10: 726b 6574 3a4f 7074 696f 6e61 6c5b 224d  rket:Optional["M
+00018b20: 6172 6b65 744d 6172 6b65 7449 7465 6d22  arketMarketItem"
+00018b30: 5d20 3d20 4e6f 6e65 0a09 6d61 726b 6574  ] = None..market
+00018b40: 5f6d 6172 6b65 745f 616c 6275 6d3a 4f70  _market_album:Op
+00018b50: 7469 6f6e 616c 5b22 4d61 726b 6574 4d61  tional["MarketMa
+00018b60: 726b 6574 416c 6275 6d22 5d20 3d20 4e6f  rketAlbum"] = No
+00018b70: 6e65 0a09 6e6f 7465 3a4f 7074 696f 6e61  ne..note:Optiona
+00018b80: 6c5b 2257 616c 6c41 7474 6163 6865 644e  l["WallAttachedN
+00018b90: 6f74 6522 5d20 3d20 4e6f 6e65 0a09 7061  ote"] = None..pa
+00018ba0: 6765 3a4f 7074 696f 6e61 6c5b 2250 6167  ge:Optional["Pag
+00018bb0: 6573 5769 6b69 7061 6765 4675 6c6c 225d  esWikipageFull"]
+00018bc0: 203d 204e 6f6e 650a 0970 686f 746f 3a4f   = None..photo:O
+00018bd0: 7074 696f 6e61 6c5b 2250 686f 746f 7350  ptional["PhotosP
+00018be0: 686f 746f 225d 203d 204e 6f6e 650a 0973  hoto"] = None..s
+00018bf0: 7469 636b 6572 3a4f 7074 696f 6e61 6c5b  ticker:Optional[
+00018c00: 2242 6173 6553 7469 636b 6572 225d 203d  "BaseSticker"] =
+00018c10: 204e 6f6e 650a 0974 7970 653a 2257 616c   None..type:"Wal
+00018c20: 6c43 6f6d 6d65 6e74 4174 7461 6368 6d65  lCommentAttachme
+00018c30: 6e74 5479 7065 220a 0976 6964 656f 3a4f  ntType"..video:O
+00018c40: 7074 696f 6e61 6c5b 2256 6964 656f 5669  ptional["VideoVi
+00018c50: 6465 6f22 5d20 3d20 4e6f 6e65 0a0a 0a63  deo"] = None...c
+00018c60: 6c61 7373 2057 616c 6c47 656f 2842 4d29  lass WallGeo(BM)
+00018c70: 3a0a 0963 6f6f 7264 696e 6174 6573 3a4f  :..coordinates:O
+00018c80: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00018c90: 6f6e 650a 0970 6c61 6365 3a4f 7074 696f  one..place:Optio
+00018ca0: 6e61 6c5b 2242 6173 6550 6c61 6365 225d  nal["BasePlace"]
+00018cb0: 203d 204e 6f6e 650a 0973 686f 776d 6170   = None..showmap
+00018cc0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00018cd0: 204e 6f6e 650a 0974 7970 653a 4f70 7469   None..type:Opti
+00018ce0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00018cf0: 0a0a 0a63 6c61 7373 2057 616c 6c47 7261  ...class WallGra
+00018d00: 6666 6974 6928 424d 293a 0a09 6964 3a4f  ffiti(BM):..id:O
+00018d10: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00018d20: 6f6e 650a 096f 776e 6572 5f69 643a 4f70  one..owner_id:Op
+00018d30: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00018d40: 6e65 0a09 7068 6f74 6f5f 3230 303a 4f70  ne..photo_200:Op
+00018d50: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00018d60: 6e65 0a09 7068 6f74 6f5f 3538 363a 4f70  ne..photo_586:Op
+00018d70: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00018d80: 6e65 0a09 6865 6967 6874 3a4f 7074 696f  ne..height:Optio
+00018d90: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00018da0: 0975 726c 3a4f 7074 696f 6e61 6c5b 7374  .url:Optional[st
+00018db0: 725d 203d 204e 6f6e 650a 0977 6964 7468  r] = None..width
+00018dc0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+00018dd0: 204e 6f6e 650a 0961 6363 6573 735f 6b65   None..access_ke
+00018de0: 793a 4f70 7469 6f6e 616c 5b73 7472 5d20  y:Optional[str] 
+00018df0: 3d20 4e6f 6e65 0a0a 0a63 6c61 7373 2057  = None...class W
+00018e00: 616c 6c50 6f73 7443 6f70 7972 6967 6874  allPostCopyright
+00018e10: 2842 4d29 3a0a 0969 643a 4f70 7469 6f6e  (BM):..id:Option
+00018e20: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00018e30: 6c69 6e6b 3a73 7472 0a09 6e61 6d65 3a73  link:str..name:s
+00018e40: 7472 0a09 7479 7065 3a73 7472 0a0a 0a63  tr..type:str...c
+00018e50: 6c61 7373 2057 616c 6c50 6f73 7453 6f75  lass WallPostSou
+00018e60: 7263 6528 424d 293a 0a09 6461 7461 3a4f  rce(BM):..data:O
+00018e70: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00018e80: 6f6e 650a 0970 6c61 7466 6f72 6d3a 4f70  one..platform:Op
+00018e90: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00018ea0: 6e65 0a09 7479 7065 3a4f 7074 696f 6e61  ne..type:Optiona
+00018eb0: 6c5b 2257 616c 6c50 6f73 7453 6f75 7263  l["WallPostSourc
+00018ec0: 6554 7970 6522 5d20 3d20 4e6f 6e65 0a09  eType"] = None..
+00018ed0: 7572 6c3a 4f70 7469 6f6e 616c 5b73 7472  url:Optional[str
+00018ee0: 5d20 3d20 4e6f 6e65 0a09 6c69 6e6b 3a4f  ] = None..link:O
+00018ef0: 7074 696f 6e61 6c5b 2242 6173 654c 696e  ptional["BaseLin
+00018f00: 6b22 5d20 3d20 4e6f 6e65 0a0a 0a63 6c61  k"] = None...cla
+00018f10: 7373 2057 616c 6c50 6f73 7465 6450 686f  ss WallPostedPho
+00018f20: 746f 2842 4d29 3a0a 0969 643a 4f70 7469  to(BM):..id:Opti
+00018f30: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00018f40: 0a09 6f77 6e65 725f 6964 3a4f 7074 696f  ..owner_id:Optio
+00018f50: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00018f60: 0970 686f 746f 5f31 3330 3a4f 7074 696f  .photo_130:Optio
+00018f70: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00018f80: 0970 686f 746f 5f36 3034 3a4f 7074 696f  .photo_604:Optio
+00018f90: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+00018fa0: 0a0a 636c 6173 7320 5761 6c6c 5669 6577  ..class WallView
+00018fb0: 7328 424d 293a 0a09 636f 756e 743a 4f70  s(BM):..count:Op
+00018fc0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00018fd0: 6e65 0a0a 0a63 6c61 7373 2057 616c 6c57  ne...class WallW
+00018fe0: 616c 6c43 6f6d 6d65 6e74 2842 4d29 3a0a  allComment(BM):.
+00018ff0: 0969 643a 696e 740a 0966 726f 6d5f 6964  .id:int..from_id
+00019000: 3a69 6e74 0a09 6361 6e5f 6564 6974 3a4f  :int..can_edit:O
+00019010: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00019020: 4e6f 6e65 0a09 706f 7374 5f69 643a 4f70  None..post_id:Op
+00019030: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00019040: 6e65 0a09 6f77 6e65 725f 6964 3a4f 7074  ne..owner_id:Opt
+00019050: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00019060: 650a 0970 6172 656e 7473 5f73 7461 636b  e..parents_stack
+00019070: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b69  :Optional[list[i
+00019080: 6e74 5d5d 203d 204e 6f6e 650a 0970 686f  nt]] = None..pho
+00019090: 746f 5f69 643a 4f70 7469 6f6e 616c 5b69  to_id:Optional[i
+000190a0: 6e74 5d20 3d20 4e6f 6e65 0a09 7669 6465  nt] = None..vide
+000190b0: 6f5f 6964 3a4f 7074 696f 6e61 6c5b 696e  o_id:Optional[in
+000190c0: 745d 203d 204e 6f6e 650a 0964 6174 653a  t] = None..date:
+000190d0: 696e 740a 0974 6578 743a 7374 720a 0961  int..text:str..a
+000190e0: 7474 6163 686d 656e 7473 3a4f 7074 696f  ttachments:Optio
+000190f0: 6e61 6c5b 6c69 7374 5b22 5761 6c6c 436f  nal[list["WallCo
+00019100: 6d6d 656e 7441 7474 6163 686d 656e 7422  mmentAttachment"
+00019110: 5d5d 203d 204e 6f6e 650a 0964 6f6e 7574  ]] = None..donut
+00019120: 3a4f 7074 696f 6e61 6c5b 2257 616c 6c57  :Optional["WallW
+00019130: 616c 6c43 6f6d 6d65 6e74 446f 6e75 7422  allCommentDonut"
+00019140: 5d20 3d20 4e6f 6e65 0a09 6c69 6b65 733a  ] = None..likes:
+00019150: 4f70 7469 6f6e 616c 5b22 4261 7365 4c69  Optional["BaseLi
+00019160: 6b65 7349 6e66 6f22 5d20 3d20 4e6f 6e65  kesInfo"] = None
+00019170: 0a09 7265 616c 5f6f 6666 7365 743a 4f70  ..real_offset:Op
+00019180: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00019190: 6e65 0a09 7265 706c 795f 746f 5f75 7365  ne..reply_to_use
+000191a0: 723a 4f70 7469 6f6e 616c 5b69 6e74 5d20  r:Optional[int] 
+000191b0: 3d20 4e6f 6e65 0a09 7265 706c 795f 746f  = None..reply_to
+000191c0: 5f63 6f6d 6d65 6e74 3a4f 7074 696f 6e61  _comment:Optiona
+000191d0: 6c5b 696e 745d 203d 204e 6f6e 650a 0974  l[int] = None..t
+000191e0: 6872 6561 643a 4f70 7469 6f6e 616c 5b22  hread:Optional["
+000191f0: 436f 6d6d 656e 7454 6872 6561 6422 5d20  CommentThread"] 
+00019200: 3d20 4e6f 6e65 0a09 6465 6c65 7465 643a  = None..deleted:
+00019210: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00019220: 204e 6f6e 650a 0970 6964 3a4f 7074 696f   None..pid:Optio
+00019230: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00019240: 0a0a 636c 6173 7320 5761 6c6c 5761 6c6c  ..class WallWall
+00019250: 436f 6d6d 656e 7444 6f6e 7574 2842 4d29  CommentDonut(BM)
+00019260: 3a0a 0969 735f 646f 6e3a 4f70 7469 6f6e  :..is_don:Option
+00019270: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+00019280: 0970 6c61 6365 686f 6c64 6572 3a4f 7074  .placeholder:Opt
+00019290: 696f 6e61 6c5b 2257 616c 6c57 616c 6c43  ional["WallWallC
+000192a0: 6f6d 6d65 6e74 446f 6e75 7450 6c61 6365  ommentDonutPlace
+000192b0: 686f 6c64 6572 225d 203d 204e 6f6e 650a  holder"] = None.
+000192c0: 0a0a 636c 6173 7320 5761 6c6c 5761 6c6c  ..class WallWall
+000192d0: 436f 6d6d 656e 7444 6f6e 7574 506c 6163  CommentDonutPlac
+000192e0: 6568 6f6c 6465 7228 424d 293a 0a09 7465  eholder(BM):..te
+000192f0: 7874 3a73 7472 0a0a 0a63 6c61 7373 2057  xt:str...class W
+00019300: 616c 6c57 616c 6c70 6f73 7428 424d 293a  allWallpost(BM):
+00019310: 0a09 6163 6365 7373 5f6b 6579 3a4f 7074  ..access_key:Opt
+00019320: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00019330: 650a 0969 735f 6465 6c65 7465 643a 4f70  e..is_deleted:Op
+00019340: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+00019350: 6f6e 650a 0961 7474 6163 686d 656e 7473  one..attachments
+00019360: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
+00019370: 5761 6c6c 5761 6c6c 706f 7374 4174 7461  WallWallpostAtta
+00019380: 6368 6d65 6e74 225d 5d20 3d20 4e6f 6e65  chment"]] = None
+00019390: 0a09 636f 7079 7269 6768 743a 4f70 7469  ..copyright:Opti
+000193a0: 6f6e 616c 5b22 5761 6c6c 506f 7374 436f  onal["WallPostCo
+000193b0: 7079 7269 6768 7422 5d20 3d20 4e6f 6e65  pyright"] = None
+000193c0: 0a09 6461 7465 3a4f 7074 696f 6e61 6c5b  ..date:Optional[
+000193d0: 696e 745d 203d 204e 6f6e 650a 0965 6469  int] = None..edi
+000193e0: 7465 643a 4f70 7469 6f6e 616c 5b69 6e74  ted:Optional[int
+000193f0: 5d20 3d20 4e6f 6e65 0a09 6672 6f6d 5f69  ] = None..from_i
+00019400: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+00019410: 3d20 4e6f 6e65 0a09 6765 6f3a 4f70 7469  = None..geo:Opti
+00019420: 6f6e 616c 5b22 5761 6c6c 4765 6f22 5d20  onal["WallGeo"] 
+00019430: 3d20 4e6f 6e65 0a09 6964 3a4f 7074 696f  = None..id:Optio
+00019440: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00019450: 0969 735f 6172 6368 6976 6564 3a4f 7074  .is_archived:Opt
+00019460: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+00019470: 6e65 0a09 6973 5f66 6176 6f72 6974 653a  ne..is_favorite:
+00019480: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00019490: 204e 6f6e 650a 096c 696b 6573 3a4f 7074   None..likes:Opt
+000194a0: 696f 6e61 6c5b 2242 6173 654c 696b 6573  ional["BaseLikes
+000194b0: 496e 666f 225d 203d 204e 6f6e 650a 096f  Info"] = None..o
+000194c0: 776e 6572 5f69 643a 4f70 7469 6f6e 616c  wner_id:Optional
+000194d0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 706f  [int] = None..po
+000194e0: 7374 5f69 643a 4f70 7469 6f6e 616c 5b69  st_id:Optional[i
+000194f0: 6e74 5d20 3d20 4e6f 6e65 0a09 7061 7265  nt] = None..pare
+00019500: 6e74 735f 7374 6163 6b3a 4f70 7469 6f6e  nts_stack:Option
+00019510: 616c 5b6c 6973 745b 696e 745d 5d20 3d20  al[list[int]] = 
+00019520: 4e6f 6e65 0a09 706f 7374 5f73 6f75 7263  None..post_sourc
+00019530: 653a 4f70 7469 6f6e 616c 5b22 5761 6c6c  e:Optional["Wall
+00019540: 506f 7374 536f 7572 6365 225d 203d 204e  PostSource"] = N
+00019550: 6f6e 650a 0970 6f73 745f 7479 7065 3a4f  one..post_type:O
+00019560: 7074 696f 6e61 6c5b 2257 616c 6c50 6f73  ptional["WallPos
+00019570: 7454 7970 6522 5d20 3d20 4e6f 6e65 0a09  tType"] = None..
+00019580: 7265 706f 7374 733a 4f70 7469 6f6e 616c  reposts:Optional
+00019590: 5b22 4261 7365 5265 706f 7374 7349 6e66  ["BaseRepostsInf
+000195a0: 6f22 5d20 3d20 4e6f 6e65 0a09 7369 676e  o"] = None..sign
+000195b0: 6572 5f69 643a 4f70 7469 6f6e 616c 5b69  er_id:Optional[i
+000195c0: 6e74 5d20 3d20 4e6f 6e65 0a09 7465 7874  nt] = None..text
+000195d0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+000195e0: 204e 6f6e 650a 0976 6965 7773 3a4f 7074   None..views:Opt
+000195f0: 696f 6e61 6c5b 2257 616c 6c56 6965 7773  ional["WallViews
+00019600: 225d 203d 204e 6f6e 650a 0a0a 636c 6173  "] = None...clas
+00019610: 7320 5761 6c6c 5761 6c6c 706f 7374 4174  s WallWallpostAt
+00019620: 7461 6368 6d65 6e74 2842 4d29 3a0a 0961  tachment(BM):..a
+00019630: 6363 6573 735f 6b65 793a 4f70 7469 6f6e  ccess_key:Option
+00019640: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
+00019650: 616c 6275 6d3a 4f70 7469 6f6e 616c 5b22  album:Optional["
+00019660: 5068 6f74 6f73 5068 6f74 6f41 6c62 756d  PhotosPhotoAlbum
+00019670: 225d 203d 204e 6f6e 650a 0961 7070 3a4f  "] = None..app:O
+00019680: 7074 696f 6e61 6c5b 2257 616c 6c41 7070  ptional["WallApp
+00019690: 506f 7374 225d 203d 204e 6f6e 650a 0961  Post"] = None..a
+000196a0: 7564 696f 3a4f 7074 696f 6e61 6c5b 2241  udio:Optional["A
+000196b0: 7564 696f 4175 6469 6f22 5d20 3d20 4e6f  udioAudio"] = No
+000196c0: 6e65 0a09 646f 633a 4f70 7469 6f6e 616c  ne..doc:Optional
+000196d0: 5b22 446f 6373 446f 6322 5d20 3d20 4e6f  ["DocsDoc"] = No
+000196e0: 6e65 0a09 6576 656e 743a 4f70 7469 6f6e  ne..event:Option
+000196f0: 616c 5b22 4576 656e 7473 4576 656e 7441  al["EventsEventA
+00019700: 7474 6163 6822 5d20 3d20 4e6f 6e65 0a09  ttach"] = None..
+00019710: 6772 6f75 703a 4f70 7469 6f6e 616c 5b22  group:Optional["
+00019720: 4772 6f75 7073 4772 6f75 7041 7474 6163  GroupsGroupAttac
+00019730: 6822 5d20 3d20 4e6f 6e65 0a09 6772 6166  h"] = None..graf
+00019740: 6669 7469 3a4f 7074 696f 6e61 6c5b 2257  fiti:Optional["W
+00019750: 616c 6c47 7261 6666 6974 6922 5d20 3d20  allGraffiti"] = 
+00019760: 4e6f 6e65 0a09 6c69 6e6b 3a4f 7074 696f  None..link:Optio
+00019770: 6e61 6c5b 2242 6173 654c 696e 6b22 5d20  nal["BaseLink"] 
+00019780: 3d20 4e6f 6e65 0a09 6d61 726b 6574 3a4f  = None..market:O
+00019790: 7074 696f 6e61 6c5b 224d 6172 6b65 744d  ptional["MarketM
+000197a0: 6172 6b65 7449 7465 6d22 5d20 3d20 4e6f  arketItem"] = No
+000197b0: 6e65 0a09 6d61 726b 6574 5f61 6c62 756d  ne..market_album
+000197c0: 3a4f 7074 696f 6e61 6c5b 224d 6172 6b65  :Optional["Marke
+000197d0: 744d 6172 6b65 7441 6c62 756d 225d 203d  tMarketAlbum"] =
+000197e0: 204e 6f6e 650a 096e 6f74 653a 4f70 7469   None..note:Opti
+000197f0: 6f6e 616c 5b22 4e6f 7465 734e 6f74 6522  onal["NotesNote"
+00019800: 5d20 3d20 4e6f 6e65 0a09 7061 6765 3a4f  ] = None..page:O
+00019810: 7074 696f 6e61 6c5b 2250 6167 6573 5769  ptional["PagesWi
+00019820: 6b69 7061 6765 4675 6c6c 225d 203d 204e  kipageFull"] = N
+00019830: 6f6e 650a 0970 686f 746f 3a4f 7074 696f  one..photo:Optio
+00019840: 6e61 6c5b 2250 686f 746f 7350 686f 746f  nal["PhotosPhoto
+00019850: 225d 203d 204e 6f6e 650a 0970 6f6c 6c3a  "] = None..poll:
+00019860: 4f70 7469 6f6e 616c 5b22 506f 6c6c 7350  Optional["PollsP
+00019870: 6f6c 6c22 5d20 3d20 4e6f 6e65 0a09 706f  oll"] = None..po
+00019880: 7374 6564 5f70 686f 746f 3a4f 7074 696f  sted_photo:Optio
+00019890: 6e61 6c5b 2257 616c 6c50 6f73 7465 6450  nal["WallPostedP
+000198a0: 686f 746f 225d 203d 204e 6f6e 650a 0974  hoto"] = None..t
+000198b0: 7970 653a 2257 616c 6c57 616c 6c70 6f73  ype:"WallWallpos
+000198c0: 7441 7474 6163 686d 656e 7454 7970 6522  tAttachmentType"
+000198d0: 0a09 7669 6465 6f3a 4f70 7469 6f6e 616c  ..video:Optional
+000198e0: 5b22 5669 6465 6f56 6964 656f 4675 6c6c  ["VideoVideoFull
+000198f0: 225d 203d 204e 6f6e 650a 0a0a 636c 6173  "] = None...clas
+00019900: 7320 5761 6c6c 5761 6c6c 706f 7374 436f  s WallWallpostCo
+00019910: 6d6d 656e 7473 446f 6e75 7428 424d 293a  mmentsDonut(BM):
+00019920: 0a09 706c 6163 6568 6f6c 6465 723a 4f70  ..placeholder:Op
+00019930: 7469 6f6e 616c 5b22 5761 6c6c 5761 6c6c  tional["WallWall
+00019940: 706f 7374 436f 6d6d 656e 7473 446f 6e75  postCommentsDonu
+00019950: 7450 6c61 6365 686f 6c64 6572 225d 203d  tPlaceholder"] =
+00019960: 204e 6f6e 650a 0a0a 636c 6173 7320 5761   None...class Wa
+00019970: 6c6c 5761 6c6c 706f 7374 436f 6d6d 656e  llWallpostCommen
+00019980: 7473 446f 6e75 7450 6c61 6365 686f 6c64  tsDonutPlacehold
+00019990: 6572 2842 4d29 3a0a 0974 6578 743a 7374  er(BM):..text:st
+000199a0: 720a 0a0a 636c 6173 7320 5761 6c6c 5761  r...class WallWa
+000199b0: 6c6c 706f 7374 446f 6e75 7428 424d 293a  llpostDonut(BM):
+000199c0: 0a09 6973 5f64 6f6e 7574 3a62 6f6f 6c0a  ..is_donut:bool.
+000199d0: 0970 6169 645f 6475 7261 7469 6f6e 3a4f  .paid_duration:O
+000199e0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000199f0: 6f6e 650a 0970 6c61 6365 686f 6c64 6572  one..placeholder
+00019a00: 3a4f 7074 696f 6e61 6c5b 2257 616c 6c57  :Optional["WallW
+00019a10: 616c 6c70 6f73 7444 6f6e 7574 506c 6163  allpostDonutPlac
+00019a20: 6568 6f6c 6465 7222 5d20 3d20 4e6f 6e65  eholder"] = None
+00019a30: 0a09 6361 6e5f 7075 626c 6973 685f 6672  ..can_publish_fr
+00019a40: 6565 5f63 6f70 793a 4f70 7469 6f6e 616c  ee_copy:Optional
+00019a50: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0965  [bool] = None..e
+00019a60: 6469 745f 6d6f 6465 3a4f 7074 696f 6e61  dit_mode:Optiona
+00019a70: 6c5b 7374 725d 203d 204e 6f6e 650a 0a0a  l[str] = None...
+00019a80: 636c 6173 7320 5761 6c6c 5761 6c6c 706f  class WallWallpo
+00019a90: 7374 446f 6e75 7450 6c61 6365 686f 6c64  stDonutPlacehold
+00019aa0: 6572 2842 4d29 3a0a 0974 6578 743a 7374  er(BM):..text:st
+00019ab0: 720a 0a0a 636c 6173 7320 5761 6c6c 5761  r...class WallWa
+00019ac0: 6c6c 706f 7374 546f 4964 2842 4d29 3a0a  llpostToId(BM):.
+00019ad0: 0961 7474 6163 686d 656e 7473 3a4f 7074  .attachments:Opt
+00019ae0: 696f 6e61 6c5b 6c69 7374 5b22 5761 6c6c  ional[list["Wall
+00019af0: 5761 6c6c 706f 7374 4174 7461 6368 6d65  WallpostAttachme
+00019b00: 6e74 225d 5d20 3d20 4e6f 6e65 0a09 636f  nt"]] = None..co
+00019b10: 6d6d 656e 7473 3a4f 7074 696f 6e61 6c5b  mments:Optional[
+00019b20: 2242 6173 6543 6f6d 6d65 6e74 7349 6e66  "BaseCommentsInf
+00019b30: 6f22 5d20 3d20 4e6f 6e65 0a09 636f 7079  o"] = None..copy
+00019b40: 5f6f 776e 6572 5f69 643a 4f70 7469 6f6e  _owner_id:Option
+00019b50: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+00019b60: 636f 7079 5f70 6f73 745f 6964 3a4f 7074  copy_post_id:Opt
+00019b70: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00019b80: 650a 0964 6174 653a 4f70 7469 6f6e 616c  e..date:Optional
+00019b90: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6672  [int] = None..fr
+00019ba0: 6f6d 5f69 643a 4f70 7469 6f6e 616c 5b69  om_id:Optional[i
+00019bb0: 6e74 5d20 3d20 4e6f 6e65 0a09 6765 6f3a  nt] = None..geo:
+00019bc0: 4f70 7469 6f6e 616c 5b22 5761 6c6c 4765  Optional["WallGe
+00019bd0: 6f22 5d20 3d20 4e6f 6e65 0a09 6964 3a4f  o"] = None..id:O
+00019be0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00019bf0: 6f6e 650a 0969 735f 6661 766f 7269 7465  one..is_favorite
+00019c00: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+00019c10: 3d20 4e6f 6e65 0a09 6c69 6b65 733a 4f70  = None..likes:Op
+00019c20: 7469 6f6e 616c 5b22 4261 7365 4c69 6b65  tional["BaseLike
+00019c30: 7349 6e66 6f22 5d20 3d20 4e6f 6e65 0a09  sInfo"] = None..
+00019c40: 706f 7374 5f69 643a 4f70 7469 6f6e 616c  post_id:Optional
+00019c50: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 706f  [int] = None..po
+00019c60: 7374 5f73 6f75 7263 653a 4f70 7469 6f6e  st_source:Option
+00019c70: 616c 5b22 5761 6c6c 506f 7374 536f 7572  al["WallPostSour
+00019c80: 6365 225d 203d 204e 6f6e 650a 0970 6f73  ce"] = None..pos
+00019c90: 745f 7479 7065 3a4f 7074 696f 6e61 6c5b  t_type:Optional[
+00019ca0: 2257 616c 6c50 6f73 7454 7970 6522 5d20  "WallPostType"] 
+00019cb0: 3d20 4e6f 6e65 0a09 7265 706f 7374 733a  = None..reposts:
+00019cc0: 4f70 7469 6f6e 616c 5b22 4261 7365 5265  Optional["BaseRe
+00019cd0: 706f 7374 7349 6e66 6f22 5d20 3d20 4e6f  postsInfo"] = No
+00019ce0: 6e65 0a09 7369 676e 6572 5f69 643a 4f70  ne..signer_id:Op
+00019cf0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00019d00: 6e65 0a09 7465 7874 3a4f 7074 696f 6e61  ne..text:Optiona
+00019d10: 6c5b 7374 725d 203d 204e 6f6e 650a 0974  l[str] = None..t
+00019d20: 6f5f 6964 3a4f 7074 696f 6e61 6c5b 696e  o_id:Optional[in
+00019d30: 745d 203d 204e 6f6e 650a 0a0a 0a0a 636c  t] = None.....cl
+00019d40: 6173 7320 5769 6467 6574 7343 6f6d 6d65  ass WidgetsComme
+00019d50: 6e74 4d65 6469 6154 7970 6528 456e 756d  ntMediaType(Enum
+00019d60: 293a 0a09 4155 4449 4f20 3d20 2261 7564  ):..AUDIO = "aud
+00019d70: 696f 220a 0950 484f 544f 203d 2022 7068  io"..PHOTO = "ph
+00019d80: 6f74 6f22 0a09 5649 4445 4f20 3d20 2276  oto"..VIDEO = "v
+00019d90: 6964 656f 220a 0a63 6c61 7373 2057 6964  ideo"..class Wid
+00019da0: 6765 7473 436f 6d6d 656e 744d 6564 6961  getsCommentMedia
+00019db0: 2842 4d29 3a0a 0969 7465 6d5f 6964 3a4f  (BM):..item_id:O
+00019dc0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00019dd0: 6f6e 650a 096f 776e 6572 5f69 643a 4f70  one..owner_id:Op
+00019de0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00019df0: 6e65 0a09 7468 756d 625f 7372 633a 4f70  ne..thumb_src:Op
+00019e00: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00019e10: 6e65 0a09 7479 7065 3a4f 7074 696f 6e61  ne..type:Optiona
+00019e20: 6c5b 2257 6964 6765 7473 436f 6d6d 656e  l["WidgetsCommen
+00019e30: 744d 6564 6961 5479 7065 225d 203d 204e  tMediaType"] = N
+00019e40: 6f6e 650a 0a0a 636c 6173 7320 5769 6467  one...class Widg
+00019e50: 6574 7343 6f6d 6d65 6e74 5265 706c 6965  etsCommentReplie
+00019e60: 7328 424d 293a 0a09 6361 6e5f 706f 7374  s(BM):..can_post
+00019e70: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+00019e80: 3d20 4e6f 6e65 0a09 636f 756e 743a 4f70  = None..count:Op
+00019e90: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00019ea0: 6e65 0a09 7265 706c 6965 733a 4f70 7469  ne..replies:Opti
+00019eb0: 6f6e 616c 5b6c 6973 745b 2257 6964 6765  onal[list["Widge
+00019ec0: 7473 436f 6d6d 656e 7452 6570 6c69 6573  tsCommentReplies
+00019ed0: 4974 656d 225d 5d20 3d20 4e6f 6e65 0a0a  Item"]] = None..
+00019ee0: 0a63 6c61 7373 2057 6964 6765 7473 436f  .class WidgetsCo
+00019ef0: 6d6d 656e 7452 6570 6c69 6573 4974 656d  mmentRepliesItem
+00019f00: 2842 4d29 3a0a 0963 6964 3a4f 7074 696f  (BM):..cid:Optio
+00019f10: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+00019f20: 0964 6174 653a 4f70 7469 6f6e 616c 5b69  .date:Optional[i
+00019f30: 6e74 5d20 3d20 4e6f 6e65 0a09 6c69 6b65  nt] = None..like
+00019f40: 733a 4f70 7469 6f6e 616c 5b22 5769 6467  s:Optional["Widg
+00019f50: 6574 7357 6964 6765 744c 696b 6573 225d  etsWidgetLikes"]
+00019f60: 203d 204e 6f6e 650a 0974 6578 743a 4f70   = None..text:Op
+00019f70: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00019f80: 6e65 0a09 7569 643a 4f70 7469 6f6e 616c  ne..uid:Optional
+00019f90: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 7573  [int] = None..us
+00019fa0: 6572 3a4f 7074 696f 6e61 6c5b 2255 7365  er:Optional["Use
+00019fb0: 7273 5573 6572 4675 6c6c 225d 203d 204e  rsUserFull"] = N
+00019fc0: 6f6e 650a 0a0a 636c 6173 7320 5769 6467  one...class Widg
+00019fd0: 6574 7357 6964 6765 7443 6f6d 6d65 6e74  etsWidgetComment
+00019fe0: 2842 4d29 3a0a 0961 7474 6163 686d 656e  (BM):..attachmen
+00019ff0: 7473 3a4f 7074 696f 6e61 6c5b 6c69 7374  ts:Optional[list
+0001a000: 5b22 5761 6c6c 436f 6d6d 656e 7441 7474  ["WallCommentAtt
+0001a010: 6163 686d 656e 7422 5d5d 203d 204e 6f6e  achment"]] = Non
+0001a020: 650a 0963 616e 5f64 656c 6574 653a 4f70  e..can_delete:Op
+0001a030: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001a040: 6f6e 650a 0963 6f6d 6d65 6e74 733a 4f70  one..comments:Op
+0001a050: 7469 6f6e 616c 5b22 5769 6467 6574 7343  tional["WidgetsC
+0001a060: 6f6d 6d65 6e74 5265 706c 6965 7322 5d20  ommentReplies"] 
+0001a070: 3d20 4e6f 6e65 0a09 6461 7465 3a69 6e74  = None..date:int
+0001a080: 0a09 6672 6f6d 5f69 643a 696e 740a 0969  ..from_id:int..i
+0001a090: 643a 696e 740a 096c 696b 6573 3a4f 7074  d:int..likes:Opt
+0001a0a0: 696f 6e61 6c5b 2242 6173 654c 696b 6573  ional["BaseLikes
+0001a0b0: 496e 666f 225d 203d 204e 6f6e 650a 096d  Info"] = None..m
+0001a0c0: 6564 6961 3a4f 7074 696f 6e61 6c5b 2257  edia:Optional["W
+0001a0d0: 6964 6765 7473 436f 6d6d 656e 744d 6564  idgetsCommentMed
+0001a0e0: 6961 225d 203d 204e 6f6e 650a 0970 6f73  ia"] = None..pos
+0001a0f0: 745f 736f 7572 6365 3a4f 7074 696f 6e61  t_source:Optiona
+0001a100: 6c5b 2257 616c 6c50 6f73 7453 6f75 7263  l["WallPostSourc
+0001a110: 6522 5d20 3d20 4e6f 6e65 0a09 706f 7374  e"] = None..post
+0001a120: 5f74 7970 653a 696e 740a 0972 6570 6f73  _type:int..repos
+0001a130: 7473 3a4f 7074 696f 6e61 6c5b 2242 6173  ts:Optional["Bas
+0001a140: 6552 6570 6f73 7473 496e 666f 225d 203d  eRepostsInfo"] =
+0001a150: 204e 6f6e 650a 0974 6578 743a 7374 720a   None..text:str.
+0001a160: 0974 6f5f 6964 3a69 6e74 0a09 7573 6572  .to_id:int..user
+0001a170: 3a4f 7074 696f 6e61 6c5b 2255 7365 7273  :Optional["Users
+0001a180: 5573 6572 4675 6c6c 225d 203d 204e 6f6e  UserFull"] = Non
+0001a190: 650a 0a0a 636c 6173 7320 5769 6467 6574  e...class Widget
+0001a1a0: 7357 6964 6765 744c 696b 6573 2842 4d29  sWidgetLikes(BM)
+0001a1b0: 3a0a 0963 6f75 6e74 3a4f 7074 696f 6e61  :..count:Optiona
+0001a1c0: 6c5b 696e 745d 203d 204e 6f6e 650a 0a0a  l[int] = None...
+0001a1d0: 636c 6173 7320 5769 6467 6574 7357 6964  class WidgetsWid
+0001a1e0: 6765 7450 6167 6528 424d 293a 0a09 636f  getPage(BM):..co
+0001a1f0: 6d6d 656e 7473 3a4f 7074 696f 6e61 6c5b  mments:Optional[
+0001a200: 2242 6173 654f 626a 6563 7443 6f75 6e74  "BaseObjectCount
+0001a210: 225d 203d 204e 6f6e 650a 0964 6174 653a  "] = None..date:
+0001a220: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0001a230: 4e6f 6e65 0a09 6465 7363 7269 7074 696f  None..descriptio
+0001a240: 6e3a 4f70 7469 6f6e 616c 5b73 7472 5d20  n:Optional[str] 
+0001a250: 3d20 4e6f 6e65 0a09 6964 3a4f 7074 696f  = None..id:Optio
+0001a260: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0001a270: 096c 696b 6573 3a4f 7074 696f 6e61 6c5b  .likes:Optional[
+0001a280: 2242 6173 654f 626a 6563 7443 6f75 6e74  "BaseObjectCount
+0001a290: 225d 203d 204e 6f6e 650a 0970 6167 655f  "] = None..page_
+0001a2a0: 6964 3a4f 7074 696f 6e61 6c5b 7374 725d  id:Optional[str]
+0001a2b0: 203d 204e 6f6e 650a 0970 686f 746f 3a4f   = None..photo:O
+0001a2c0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001a2d0: 6f6e 650a 0974 6974 6c65 3a4f 7074 696f  one..title:Optio
 0001a2e0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-0001a2f0: 0a0a 0a0a 636c 6173 7320 4163 636f 756e  ....class Accoun
-0001a300: 7455 7365 7253 6574 7469 6e67 7328 5573  tUserSettings(Us
-0001a310: 6572 7355 7365 724d 696e 2c20 5573 6572  ersUserMin, User
-0001a320: 7355 7365 7253 6574 7469 6e67 7358 7472  sUserSettingsXtr
-0001a330: 293a 0a09 7068 6f74 6f5f 3230 303a 4f70  ):..photo_200:Op
-0001a340: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001a350: 6e65 0a09 6973 5f73 6572 7669 6365 5f61  ne..is_service_a
-0001a360: 6363 6f75 6e74 3a4f 7074 696f 6e61 6c5b  ccount:Optional[
-0001a370: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 636c  bool] = None..cl
-0001a380: 6173 7320 4164 7354 6172 6753 6574 7469  ass AdsTargSetti
-0001a390: 6e67 7328 4164 7343 7269 7465 7269 6129  ngs(AdsCriteria)
-0001a3a0: 3a0a 0969 643a 4f70 7469 6f6e 616c 5b69  :..id:Optional[i
-0001a3b0: 6e74 5d20 3d20 4e6f 6e65 0a09 6361 6d70  nt] = None..camp
-0001a3c0: 6169 676e 5f69 643a 4f70 7469 6f6e 616c  aign_id:Optional
-0001a3d0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a 636c  [int] = None..cl
-0001a3e0: 6173 7320 4170 7073 4170 7028 4170 7073  ass AppsApp(Apps
-0001a3f0: 4170 704d 696e 293a 0a09 6175 7468 6f72  AppMin):..author
-0001a400: 5f75 726c 3a4f 7074 696f 6e61 6c5b 7374  _url:Optional[st
-0001a410: 725d 203d 204e 6f6e 650a 0962 616e 6e65  r] = None..banne
-0001a420: 725f 3131 3230 3a4f 7074 696f 6e61 6c5b  r_1120:Optional[
-0001a430: 7374 725d 203d 204e 6f6e 650a 0962 616e  str] = None..ban
-0001a440: 6e65 725f 3536 303a 4f70 7469 6f6e 616c  ner_560:Optional
-0001a450: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6963  [str] = None..ic
-0001a460: 6f6e 5f31 363a 4f70 7469 6f6e 616c 5b73  on_16:Optional[s
-0001a470: 7472 5d20 3d20 4e6f 6e65 0a09 6973 5f6e  tr] = None..is_n
-0001a480: 6577 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ew:Optional[bool
-0001a490: 5d20 3d20 4e6f 6e65 0a09 7075 7368 5f65  ] = None..push_e
-0001a4a0: 6e61 626c 6564 3a4f 7074 696f 6e61 6c5b  nabled:Optional[
-0001a4b0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 7363  bool] = None..sc
-0001a4c0: 7265 656e 5f6f 7269 656e 7461 7469 6f6e  reen_orientation
-0001a4d0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-0001a4e0: 204e 6f6e 650a 0966 7269 656e 6473 3a4f   None..friends:O
-0001a4f0: 7074 696f 6e61 6c5b 6c69 7374 5b69 6e74  ptional[list[int
-0001a500: 5d5d 203d 204e 6f6e 650a 0963 6174 616c  ]] = None..catal
-0001a510: 6f67 5f70 6f73 6974 696f 6e3a 4f70 7469  og_position:Opti
-0001a520: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-0001a530: 0a09 6465 7363 7269 7074 696f 6e3a 4f70  ..description:Op
-0001a540: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001a550: 6e65 0a09 6765 6e72 653a 4f70 7469 6f6e  ne..genre:Option
-0001a560: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001a570: 6765 6e72 655f 6964 3a4f 7074 696f 6e61  genre_id:Optiona
-0001a580: 6c5b 696e 745d 203d 204e 6f6e 650a 0969  l[int] = None..i
-0001a590: 6e74 6572 6e61 7469 6f6e 616c 3a4f 7074  nternational:Opt
-0001a5a0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-0001a5b0: 6e65 0a09 6973 5f69 6e5f 6361 7461 6c6f  ne..is_in_catalo
-0001a5c0: 673a 4f70 7469 6f6e 616c 5b69 6e74 5d20  g:Optional[int] 
-0001a5d0: 3d20 4e6f 6e65 0a09 6c65 6164 6572 626f  = None..leaderbo
-0001a5e0: 6172 645f 7479 7065 3a4f 7074 696f 6e61  ard_type:Optiona
-0001a5f0: 6c5b 2241 7070 7341 7070 4c65 6164 6572  l["AppsAppLeader
-0001a600: 626f 6172 6454 7970 6522 5d20 3d20 4e6f  boardType"] = No
-0001a610: 6e65 0a09 6d65 6d62 6572 735f 636f 756e  ne..members_coun
-0001a620: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
-0001a630: 3d20 4e6f 6e65 0a09 706c 6174 666f 726d  = None..platform
-0001a640: 5f69 643a 4f70 7469 6f6e 616c 5b73 7472  _id:Optional[str
-0001a650: 5d20 3d20 4e6f 6e65 0a09 7075 626c 6973  ] = None..publis
-0001a660: 6865 645f 6461 7465 3a4f 7074 696f 6e61  hed_date:Optiona
-0001a670: 6c5b 696e 745d 203d 204e 6f6e 650a 0973  l[int] = None..s
-0001a680: 6372 6565 6e5f 6e61 6d65 3a4f 7074 696f  creen_name:Optio
-0001a690: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-0001a6a0: 0973 6563 7469 6f6e 3a4f 7074 696f 6e61  .section:Optiona
-0001a6b0: 6c5b 7374 725d 203d 204e 6f6e 650a 0a63  l[str] = None..c
-0001a6c0: 6c61 7373 2043 616c 6c62 6163 6b43 6f6e  lass CallbackCon
-0001a6d0: 6669 726d 6174 696f 6e28 4361 6c6c 6261  firmation(Callba
-0001a6e0: 636b 4261 7365 293a 0a09 7479 7065 3a4f  ckBase):..type:O
-0001a6f0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0001a700: 6f6e 650a 0a63 6c61 7373 2043 616c 6c62  one..class Callb
-0001a710: 6163 6b4d 6573 7361 6765 416c 6c6f 7728  ackMessageAllow(
-0001a720: 4361 6c6c 6261 636b 4261 7365 293a 0a09  CallbackBase):..
-0001a730: 7479 7065 3a4f 7074 696f 6e61 6c5b 7374  type:Optional[st
-0001a740: 725d 203d 204e 6f6e 650a 096f 626a 6563  r] = None..objec
-0001a750: 743a 2243 616c 6c62 6163 6b4d 6573 7361  t:"CallbackMessa
-0001a760: 6765 416c 6c6f 774f 626a 6563 7422 0a0a  geAllowObject"..
-0001a770: 636c 6173 7320 4361 6c6c 6261 636b 4d65  class CallbackMe
-0001a780: 7373 6167 6545 6469 7428 4361 6c6c 6261  ssageEdit(Callba
-0001a790: 636b 4261 7365 293a 0a09 7479 7065 3a4f  ckBase):..type:O
-0001a7a0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0001a7b0: 6f6e 650a 096f 626a 6563 743a 224d 6573  one..object:"Mes
-0001a7c0: 7361 6765 734d 6573 7361 6765 220a 0a63  sagesMessage"..c
-0001a7d0: 6c61 7373 2043 616c 6c62 6163 6b4d 6573  lass CallbackMes
-0001a7e0: 7361 6765 4e65 7728 4361 6c6c 6261 636b  sageNew(Callback
-0001a7f0: 4261 7365 293a 0a09 7479 7065 3a4f 7074  Base):..type:Opt
-0001a800: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001a810: 650a 096f 626a 6563 743a 6f62 6a65 6374  e..object:object
-0001a820: 0a0a 636c 6173 7320 4361 6c6c 6261 636b  ..class Callback
-0001a830: 4d65 7373 6167 6552 6570 6c79 2843 616c  MessageReply(Cal
-0001a840: 6c62 6163 6b42 6173 6529 3a0a 0974 7970  lbackBase):..typ
-0001a850: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-0001a860: 3d20 4e6f 6e65 0a09 6f62 6a65 6374 3a22  = None..object:"
-0001a870: 4d65 7373 6167 6573 4d65 7373 6167 6522  MessagesMessage"
-0001a880: 0a0a 636c 6173 7320 4461 7461 6261 7365  ..class Database
-0001a890: 4369 7479 2842 6173 654f 626a 6563 7429  City(BaseObject)
-0001a8a0: 3a0a 0961 7265 613a 4f70 7469 6f6e 616c  :..area:Optional
-0001a8b0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7265  [str] = None..re
-0001a8c0: 6769 6f6e 3a4f 7074 696f 6e61 6c5b 7374  gion:Optional[st
-0001a8d0: 725d 203d 204e 6f6e 650a 0969 6d70 6f72  r] = None..impor
-0001a8e0: 7461 6e74 3a4f 7074 696f 6e61 6c5b 626f  tant:Optional[bo
-0001a8f0: 6f6c 5d20 3d20 4e6f 6e65 0a0a 636c 6173  ol] = None..clas
-0001a900: 7320 4672 6965 6e64 7346 7269 656e 6445  s FriendsFriendE
-0001a910: 7874 656e 6465 6453 7461 7475 7328 4672  xtendedStatus(Fr
-0001a920: 6965 6e64 7346 7269 656e 6453 7461 7475  iendsFriendStatu
-0001a930: 7329 3a0a 0969 735f 7265 7175 6573 745f  s):..is_request_
-0001a940: 756e 7265 6164 3a4f 7074 696f 6e61 6c5b  unread:Optional[
-0001a950: 626f 6f6c 5d20 3d20 4e6f 6e65 0a0a 636c  bool] = None..cl
-0001a960: 6173 7320 4772 6f75 7073 4772 6f75 7046  ass GroupsGroupF
-0001a970: 756c 6c28 4772 6f75 7073 4772 6f75 7029  ull(GroupsGroup)
-0001a980: 3a0a 096d 6172 6b65 743a 4f70 7469 6f6e  :..market:Option
-0001a990: 616c 5b22 4772 6f75 7073 4d61 726b 6574  al["GroupsMarket
-0001a9a0: 496e 666f 225d 203d 204e 6f6e 650a 096d  Info"] = None..m
-0001a9b0: 656d 6265 725f 7374 6174 7573 3a4f 7074  ember_status:Opt
-0001a9c0: 696f 6e61 6c5b 2247 726f 7570 7347 726f  ional["GroupsGro
-0001a9d0: 7570 4675 6c6c 4d65 6d62 6572 5374 6174  upFullMemberStat
-0001a9e0: 7573 225d 203d 204e 6f6e 650a 0969 735f  us"] = None..is_
-0001a9f0: 6164 756c 743a 4f70 7469 6f6e 616c 5b62  adult:Optional[b
-0001aa00: 6f6f 6c5d 203d 204e 6f6e 650a 0969 735f  ool] = None..is_
-0001aa10: 6869 6464 656e 5f66 726f 6d5f 6665 6564  hidden_from_feed
-0001aa20: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-0001aa30: 3d20 4e6f 6e65 0a09 6973 5f66 6176 6f72  = None..is_favor
-0001aa40: 6974 653a 4f70 7469 6f6e 616c 5b62 6f6f  ite:Optional[boo
-0001aa50: 6c5d 203d 204e 6f6e 650a 0969 735f 7375  l] = None..is_su
-0001aa60: 6273 6372 6962 6564 3a4f 7074 696f 6e61  bscribed:Optiona
-0001aa70: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0001aa80: 6369 7479 3a4f 7074 696f 6e61 6c5b 2242  city:Optional["B
-0001aa90: 6173 654f 626a 6563 7422 5d20 3d20 4e6f  aseObject"] = No
-0001aaa0: 6e65 0a09 636f 756e 7472 793a 4f70 7469  ne..country:Opti
-0001aab0: 6f6e 616c 5b22 4261 7365 436f 756e 7472  onal["BaseCountr
-0001aac0: 7922 5d20 3d20 4e6f 6e65 0a09 7665 7269  y"] = None..veri
-0001aad0: 6669 6564 3a4f 7074 696f 6e61 6c5b 626f  fied:Optional[bo
-0001aae0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6465 7363  ol] = None..desc
-0001aaf0: 7269 7074 696f 6e3a 4f70 7469 6f6e 616c  ription:Optional
-0001ab00: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7769  [str] = None..wi
-0001ab10: 6b69 5f70 6167 653a 4f70 7469 6f6e 616c  ki_page:Optional
-0001ab20: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6d65  [str] = None..me
-0001ab30: 6d62 6572 735f 636f 756e 743a 4f70 7469  mbers_count:Opti
-0001ab40: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-0001ab50: 0a09 6d65 6d62 6572 735f 636f 756e 745f  ..members_count_
-0001ab60: 7465 7874 3a4f 7074 696f 6e61 6c5b 7374  text:Optional[st
-0001ab70: 725d 203d 204e 6f6e 650a 0972 6571 7565  r] = None..reque
-0001ab80: 7374 735f 636f 756e 743a 4f70 7469 6f6e  sts_count:Option
-0001ab90: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-0001aba0: 7669 6465 6f5f 6c69 7665 5f6c 6576 656c  video_live_level
-0001abb0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-0001abc0: 204e 6f6e 650a 0976 6964 656f 5f6c 6976   None..video_liv
-0001abd0: 655f 636f 756e 743a 4f70 7469 6f6e 616c  e_count:Optional
-0001abe0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 636c  [int] = None..cl
-0001abf0: 6970 735f 636f 756e 743a 4f70 7469 6f6e  ips_count:Option
-0001ac00: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
-0001ac10: 636f 756e 7465 7273 3a4f 7074 696f 6e61  counters:Optiona
-0001ac20: 6c5b 2247 726f 7570 7343 6f75 6e74 6572  l["GroupsCounter
-0001ac30: 7347 726f 7570 225d 203d 204e 6f6e 650a  sGroup"] = None.
-0001ac40: 0963 6f76 6572 3a4f 7074 696f 6e61 6c5b  .cover:Optional[
-0001ac50: 2247 726f 7570 7343 6f76 6572 225d 203d  "GroupsCover"] =
-0001ac60: 204e 6f6e 650a 0963 616e 5f70 6f73 743a   None..can_post:
-0001ac70: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-0001ac80: 204e 6f6e 650a 0963 616e 5f73 7567 6765   None..can_sugge
-0001ac90: 7374 3a4f 7074 696f 6e61 6c5b 626f 6f6c  st:Optional[bool
-0001aca0: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 7570  ] = None..can_up
-0001acb0: 6c6f 6164 5f73 746f 7279 3a4f 7074 696f  load_story:Optio
-0001acc0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001acd0: 0a09 6361 6e5f 7570 6c6f 6164 5f64 6f63  ..can_upload_doc
-0001ace0: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-0001acf0: 3d20 4e6f 6e65 0a09 6361 6e5f 7570 6c6f  = None..can_uplo
-0001ad00: 6164 5f76 6964 656f 3a4f 7074 696f 6e61  ad_video:Optiona
-0001ad10: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0001ad20: 6361 6e5f 7365 655f 616c 6c5f 706f 7374  can_see_all_post
-0001ad30: 733a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  s:Optional[bool]
-0001ad40: 203d 204e 6f6e 650a 0963 616e 5f63 7265   = None..can_cre
-0001ad50: 6174 655f 746f 7069 633a 4f70 7469 6f6e  ate_topic:Option
-0001ad60: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-0001ad70: 0961 6374 6976 6974 793a 4f70 7469 6f6e  .activity:Option
-0001ad80: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001ad90: 6669 7865 645f 706f 7374 3a4f 7074 696f  fixed_post:Optio
-0001ada0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
-0001adb0: 0968 6173 5f70 686f 746f 3a4f 7074 696f  .has_photo:Optio
-0001adc0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001add0: 0a09 6372 6f70 5f70 686f 746f 3a4f 7074  ..crop_photo:Opt
-0001ade0: 696f 6e61 6c5b 2242 6173 6543 726f 7050  ional["BaseCropP
-0001adf0: 686f 746f 225d 203d 204e 6f6e 650a 0973  hoto"] = None..s
-0001ae00: 7461 7475 733a 4f70 7469 6f6e 616c 5b73  tatus:Optional[s
-0001ae10: 7472 5d20 3d20 4e6f 6e65 0a09 7374 6174  tr] = None..stat
-0001ae20: 7573 5f61 7564 696f 3a4f 7074 696f 6e61  us_audio:Optiona
-0001ae30: 6c5b 2241 7564 696f 4175 6469 6f22 5d20  l["AudioAudio"] 
-0001ae40: 3d20 4e6f 6e65 0a09 6d61 696e 5f61 6c62  = None..main_alb
-0001ae50: 756d 5f69 643a 4f70 7469 6f6e 616c 5b69  um_id:Optional[i
-0001ae60: 6e74 5d20 3d20 4e6f 6e65 0a09 6c69 6e6b  nt] = None..link
-0001ae70: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-0001ae80: 2247 726f 7570 734c 696e 6b73 4974 656d  "GroupsLinksItem
-0001ae90: 225d 5d20 3d20 4e6f 6e65 0a09 636f 6e74  "]] = None..cont
-0001aea0: 6163 7473 3a4f 7074 696f 6e61 6c5b 6c69  acts:Optional[li
-0001aeb0: 7374 5b22 4772 6f75 7073 436f 6e74 6163  st["GroupsContac
-0001aec0: 7473 4974 656d 225d 5d20 3d20 4e6f 6e65  tsItem"]] = None
-0001aed0: 0a09 7761 6c6c 3a4f 7074 696f 6e61 6c5b  ..wall:Optional[
-0001aee0: 696e 745d 203d 204e 6f6e 650a 0973 6974  int] = None..sit
-0001aef0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
-0001af00: 3d20 4e6f 6e65 0a09 6d61 696e 5f73 6563  = None..main_sec
-0001af10: 7469 6f6e 3a4f 7074 696f 6e61 6c5b 2247  tion:Optional["G
-0001af20: 726f 7570 7347 726f 7570 4675 6c6c 5365  roupsGroupFullSe
-0001af30: 6374 696f 6e22 5d20 3d20 4e6f 6e65 0a09  ction"] = None..
-0001af40: 7365 636f 6e64 6172 795f 7365 6374 696f  secondary_sectio
-0001af50: 6e3a 4f70 7469 6f6e 616c 5b22 4772 6f75  n:Optional["Grou
-0001af60: 7073 4772 6f75 7046 756c 6c53 6563 7469  psGroupFullSecti
-0001af70: 6f6e 225d 203d 204e 6f6e 650a 0974 7265  on"] = None..tre
-0001af80: 6e64 696e 673a 4f70 7469 6f6e 616c 5b62  nding:Optional[b
-0001af90: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
-0001afa0: 5f6d 6573 7361 6765 3a4f 7074 696f 6e61  _message:Optiona
-0001afb0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0001afc0: 6973 5f6d 6573 7361 6765 735f 626c 6f63  is_messages_bloc
-0001afd0: 6b65 643a 4f70 7469 6f6e 616c 5b62 6f6f  ked:Optional[boo
-0001afe0: 6c5d 203d 204e 6f6e 650a 0963 616e 5f73  l] = None..can_s
-0001aff0: 656e 645f 6e6f 7469 6679 3a4f 7074 696f  end_notify:Optio
-0001b000: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001b010: 0a09 6f6e 6c69 6e65 5f73 7461 7475 733a  ..online_status:
-0001b020: 4f70 7469 6f6e 616c 5b22 4772 6f75 7073  Optional["Groups
-0001b030: 4f6e 6c69 6e65 5374 6174 7573 225d 203d  OnlineStatus"] =
-0001b040: 204e 6f6e 650a 0969 6e76 6974 6564 5f62   None..invited_b
-0001b050: 793a 4f70 7469 6f6e 616c 5b69 6e74 5d20  y:Optional[int] 
-0001b060: 3d20 4e6f 6e65 0a09 6167 655f 6c69 6d69  = None..age_limi
-0001b070: 7473 3a4f 7074 696f 6e61 6c5b 2247 726f  ts:Optional["Gro
-0001b080: 7570 7347 726f 7570 4675 6c6c 4167 654c  upsGroupFullAgeL
-0001b090: 696d 6974 7322 5d20 3d20 4e6f 6e65 0a09  imits"] = None..
-0001b0a0: 6261 6e5f 696e 666f 3a4f 7074 696f 6e61  ban_info:Optiona
-0001b0b0: 6c5b 2247 726f 7570 7347 726f 7570 4261  l["GroupsGroupBa
-0001b0c0: 6e49 6e66 6f22 5d20 3d20 4e6f 6e65 0a09  nInfo"] = None..
-0001b0d0: 6861 735f 6d61 726b 6574 5f61 7070 3a4f  has_market_app:O
-0001b0e0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-0001b0f0: 4e6f 6e65 0a09 7573 696e 675f 766b 7061  None..using_vkpa
-0001b100: 795f 6d61 726b 6574 5f61 7070 3a4f 7074  y_market_app:Opt
-0001b110: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-0001b120: 6e65 0a09 6861 735f 6772 6f75 705f 6368  ne..has_group_ch
-0001b130: 616e 6e65 6c3a 4f70 7469 6f6e 616c 5b62  annel:Optional[b
-0001b140: 6f6f 6c5d 203d 204e 6f6e 650a 0961 6464  ool] = None..add
-0001b150: 7265 7373 6573 3a4f 7074 696f 6e61 6c5b  resses:Optional[
-0001b160: 2247 726f 7570 7341 6464 7265 7373 6573  "GroupsAddresses
-0001b170: 496e 666f 225d 203d 204e 6f6e 650a 0969  Info"] = None..i
-0001b180: 735f 7375 6273 6372 6962 6564 5f70 6f64  s_subscribed_pod
-0001b190: 6361 7374 733a 4f70 7469 6f6e 616c 5b62  casts:Optional[b
-0001b1a0: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
-0001b1b0: 5f73 7562 7363 7269 6265 5f70 6f64 6361  _subscribe_podca
-0001b1c0: 7374 733a 4f70 7469 6f6e 616c 5b62 6f6f  sts:Optional[boo
-0001b1d0: 6c5d 203d 204e 6f6e 650a 0963 616e 5f73  l] = None..can_s
-0001b1e0: 7562 7363 7269 6265 5f70 6f73 7473 3a4f  ubscribe_posts:O
-0001b1f0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-0001b200: 4e6f 6e65 0a09 6c69 7665 5f63 6f76 6572  None..live_cover
-0001b210: 733a 4f70 7469 6f6e 616c 5b22 4772 6f75  s:Optional["Grou
-0001b220: 7073 4c69 7665 436f 7665 7273 225d 203d  psLiveCovers"] =
-0001b230: 204e 6f6e 650a 0973 746f 7269 6573 5f61   None..stories_a
-0001b240: 7263 6869 7665 5f63 6f75 6e74 3a4f 7074  rchive_count:Opt
-0001b250: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0001b260: 650a 0968 6173 5f75 6e73 6565 6e5f 7374  e..has_unseen_st
-0001b270: 6f72 6965 733a 4f70 7469 6f6e 616c 5b62  ories:Optional[b
-0001b280: 6f6f 6c5d 203d 204e 6f6e 650a 0a63 6c61  ool] = None..cla
-0001b290: 7373 204d 6172 6b65 744d 6172 6b65 7449  ss MarketMarketI
-0001b2a0: 7465 6d46 756c 6c28 4d61 726b 6574 4d61  temFull(MarketMa
-0001b2b0: 726b 6574 4974 656d 293a 0a09 616c 6275  rketItem):..albu
-0001b2c0: 6d73 5f69 6473 3a4f 7074 696f 6e61 6c5b  ms_ids:Optional[
-0001b2d0: 6c69 7374 5b69 6e74 5d5d 203d 204e 6f6e  list[int]] = Non
-0001b2e0: 650a 0970 686f 746f 733a 4f70 7469 6f6e  e..photos:Option
-0001b2f0: 616c 5b6c 6973 745b 2250 686f 746f 7350  al[list["PhotosP
-0001b300: 686f 746f 225d 5d20 3d20 4e6f 6e65 0a09  hoto"]] = None..
-0001b310: 6361 6e5f 636f 6d6d 656e 743a 4f70 7469  can_comment:Opti
-0001b320: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-0001b330: 650a 0963 616e 5f72 6570 6f73 743a 4f70  e..can_repost:Op
-0001b340: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-0001b350: 6f6e 650a 096c 696b 6573 3a4f 7074 696f  one..likes:Optio
-0001b360: 6e61 6c5b 2242 6173 654c 696b 6573 225d  nal["BaseLikes"]
-0001b370: 203d 204e 6f6e 650a 0972 6570 6f73 7473   = None..reposts
-0001b380: 3a4f 7074 696f 6e61 6c5b 2242 6173 6552  :Optional["BaseR
-0001b390: 6570 6f73 7473 496e 666f 225d 203d 204e  epostsInfo"] = N
-0001b3a0: 6f6e 650a 0976 6965 7773 5f63 6f75 6e74  one..views_count
-0001b3b0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-0001b3c0: 204e 6f6e 650a 0977 6973 686c 6973 745f   None..wishlist_
-0001b3d0: 6974 656d 5f69 643a 4f70 7469 6f6e 616c  item_id:Optional
-0001b3e0: 5b69 6e74 5d20 3d20 4e6f 6e65 0a09 6361  [int] = None..ca
-0001b3f0: 6e63 656c 5f69 6e66 6f3a 4f70 7469 6f6e  ncel_info:Option
-0001b400: 616c 5b22 4261 7365 4c69 6e6b 225d 203d  al["BaseLink"] =
-0001b410: 204e 6f6e 650a 0975 7365 725f 6167 7265   None..user_agre
-0001b420: 656d 656e 745f 696e 666f 3a4f 7074 696f  ement_info:Optio
-0001b430: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-0001b440: 0961 645f 6964 3a4f 7074 696f 6e61 6c5b  .ad_id:Optional[
-0001b450: 696e 745d 203d 204e 6f6e 650a 0a63 6c61  int] = None..cla
-0001b460: 7373 204d 6573 7361 6765 7347 6574 436f  ss MessagesGetCo
-0001b470: 6e76 6572 7361 7469 6f6e 4279 4964 4578  nversationByIdEx
-0001b480: 7465 6e64 6564 284d 6573 7361 6765 7347  tended(MessagesG
-0001b490: 6574 436f 6e76 6572 7361 7469 6f6e 4279  etConversationBy
-0001b4a0: 4964 293a 0a09 7072 6f66 696c 6573 3a4f  Id):..profiles:O
-0001b4b0: 7074 696f 6e61 6c5b 6c69 7374 5b22 5573  ptional[list["Us
-0001b4c0: 6572 7355 7365 7246 756c 6c22 5d5d 203d  ersUserFull"]] =
-0001b4d0: 204e 6f6e 650a 0967 726f 7570 733a 4f70   None..groups:Op
-0001b4e0: 7469 6f6e 616c 5b6c 6973 745b 2247 726f  tional[list["Gro
-0001b4f0: 7570 7347 726f 7570 4675 6c6c 225d 5d20  upsGroupFull"]] 
-0001b500: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4e65  = None..class Ne
-0001b510: 7773 6665 6564 4974 656d 4175 6469 6f28  wsfeedItemAudio(
-0001b520: 4e65 7773 6665 6564 4974 656d 4261 7365  NewsfeedItemBase
-0001b530: 293a 0a09 6175 6469 6f3a 4f70 7469 6f6e  ):..audio:Option
-0001b540: 616c 5b22 4e65 7773 6665 6564 4974 656d  al["NewsfeedItem
-0001b550: 4175 6469 6f41 7564 696f 225d 203d 204e  AudioAudio"] = N
-0001b560: 6f6e 650a 0970 6f73 745f 6964 3a4f 7074  one..post_id:Opt
-0001b570: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0001b580: 650a 0a63 6c61 7373 204e 6577 7366 6565  e..class Newsfee
-0001b590: 6449 7465 6d44 6967 6573 7428 4e65 7773  dItemDigest(News
-0001b5a0: 6665 6564 4974 656d 4261 7365 293a 0a09  feedItemBase):..
-0001b5b0: 6665 6564 5f69 643a 4f70 7469 6f6e 616c  feed_id:Optional
-0001b5c0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6974  [str] = None..it
-0001b5d0: 656d 733a 4f70 7469 6f6e 616c 5b6c 6973  ems:Optional[lis
-0001b5e0: 745b 224e 6577 7366 6565 6449 7465 6d44  t["NewsfeedItemD
-0001b5f0: 6967 6573 7449 7465 6d22 5d5d 203d 204e  igestItem"]] = N
-0001b600: 6f6e 650a 096d 6169 6e5f 706f 7374 5f69  one..main_post_i
-0001b610: 6473 3a4f 7074 696f 6e61 6c5b 6c69 7374  ds:Optional[list
-0001b620: 5b73 7472 5d5d 203d 204e 6f6e 650a 0974  [str]] = None..t
-0001b630: 656d 706c 6174 653a 4f70 7469 6f6e 616c  emplate:Optional
-0001b640: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6865  [str] = None..he
-0001b650: 6164 6572 3a4f 7074 696f 6e61 6c5b 224e  ader:Optional["N
-0001b660: 6577 7366 6565 6449 7465 6d44 6967 6573  ewsfeedItemDiges
-0001b670: 7448 6561 6465 7222 5d20 3d20 4e6f 6e65  tHeader"] = None
-0001b680: 0a09 666f 6f74 6572 3a4f 7074 696f 6e61  ..footer:Optiona
-0001b690: 6c5b 224e 6577 7366 6565 6449 7465 6d44  l["NewsfeedItemD
-0001b6a0: 6967 6573 7446 6f6f 7465 7222 5d20 3d20  igestFooter"] = 
-0001b6b0: 4e6f 6e65 0a09 7472 6163 6b5f 636f 6465  None..track_code
-0001b6c0: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-0001b6d0: 204e 6f6e 650a 0a63 6c61 7373 204e 6577   None..class New
-0001b6e0: 7366 6565 6449 7465 6d46 7269 656e 6428  sfeedItemFriend(
-0001b6f0: 4e65 7773 6665 6564 4974 656d 4261 7365  NewsfeedItemBase
-0001b700: 293a 0a09 6672 6965 6e64 733a 4f70 7469  ):..friends:Opti
-0001b710: 6f6e 616c 5b22 4e65 7773 6665 6564 4974  onal["NewsfeedIt
-0001b720: 656d 4672 6965 6e64 4672 6965 6e64 7322  emFriendFriends"
-0001b730: 5d20 3d20 4e6f 6e65 0a0a 636c 6173 7320  ] = None..class 
-0001b740: 4e65 7773 6665 6564 4974 656d 5068 6f74  NewsfeedItemPhot
-0001b750: 6f28 5761 6c6c 4361 726f 7573 656c 4261  o(WallCarouselBa
-0001b760: 7365 2c20 4e65 7773 6665 6564 4974 656d  se, NewsfeedItem
-0001b770: 4261 7365 293a 0a09 7068 6f74 6f73 3a4f  Base):..photos:O
-0001b780: 7074 696f 6e61 6c5b 224e 6577 7366 6565  ptional["Newsfee
-0001b790: 6449 7465 6d50 686f 746f 5068 6f74 6f73  dItemPhotoPhotos
-0001b7a0: 225d 203d 204e 6f6e 650a 0970 6f73 745f  "] = None..post_
-0001b7b0: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-0001b7c0: 203d 204e 6f6e 650a 0a63 6c61 7373 204e   = None..class N
-0001b7d0: 6577 7366 6565 6449 7465 6d50 686f 746f  ewsfeedItemPhoto
-0001b7e0: 5461 6728 5761 6c6c 4361 726f 7573 656c  Tag(WallCarousel
-0001b7f0: 4261 7365 2c20 4e65 7773 6665 6564 4974  Base, NewsfeedIt
-0001b800: 656d 4261 7365 293a 0a09 7068 6f74 6f5f  emBase):..photo_
-0001b810: 7461 6773 3a4f 7074 696f 6e61 6c5b 224e  tags:Optional["N
-0001b820: 6577 7366 6565 6449 7465 6d50 686f 746f  ewsfeedItemPhoto
-0001b830: 5461 6750 686f 746f 5461 6773 225d 203d  TagPhotoTags"] =
-0001b840: 204e 6f6e 650a 0970 6f73 745f 6964 3a4f   None..post_id:O
-0001b850: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0001b860: 6f6e 650a 0a63 6c61 7373 204e 6577 7366  one..class Newsf
-0001b870: 6565 6449 7465 6d50 726f 6d6f 4275 7474  eedItemPromoButt
-0001b880: 6f6e 284e 6577 7366 6565 6449 7465 6d42  on(NewsfeedItemB
-0001b890: 6173 6529 3a0a 0974 6578 743a 4f70 7469  ase):..text:Opti
-0001b8a0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0001b8b0: 0a09 7469 746c 653a 4f70 7469 6f6e 616c  ..title:Optional
-0001b8c0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6163  [str] = None..ac
-0001b8d0: 7469 6f6e 3a4f 7074 696f 6e61 6c5b 224e  tion:Optional["N
-0001b8e0: 6577 7366 6565 6449 7465 6d50 726f 6d6f  ewsfeedItemPromo
-0001b8f0: 4275 7474 6f6e 4163 7469 6f6e 225d 203d  ButtonAction"] =
-0001b900: 204e 6f6e 650a 0969 6d61 6765 733a 4f70   None..images:Op
-0001b910: 7469 6f6e 616c 5b6c 6973 745b 224e 6577  tional[list["New
-0001b920: 7366 6565 6449 7465 6d50 726f 6d6f 4275  sfeedItemPromoBu
-0001b930: 7474 6f6e 496d 6167 6522 5d5d 203d 204e  ttonImage"]] = N
-0001b940: 6f6e 650a 0974 7261 636b 5f63 6f64 653a  one..track_code:
-0001b950: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0001b960: 4e6f 6e65 0a0a 636c 6173 7320 4e65 7773  None..class News
-0001b970: 6665 6564 4974 656d 546f 7069 6328 4e65  feedItemTopic(Ne
-0001b980: 7773 6665 6564 4974 656d 4261 7365 293a  wsfeedItemBase):
-0001b990: 0a09 636f 6d6d 656e 7473 3a4f 7074 696f  ..comments:Optio
-0001b9a0: 6e61 6c5b 2242 6173 6543 6f6d 6d65 6e74  nal["BaseComment
-0001b9b0: 7349 6e66 6f22 5d20 3d20 4e6f 6e65 0a09  sInfo"] = None..
-0001b9c0: 6c69 6b65 733a 4f70 7469 6f6e 616c 5b22  likes:Optional["
-0001b9d0: 4261 7365 4c69 6b65 7349 6e66 6f22 5d20  BaseLikesInfo"] 
-0001b9e0: 3d20 4e6f 6e65 0a09 706f 7374 5f69 643a  = None..post_id:
-0001b9f0: 696e 740a 0974 6578 743a 7374 720a 0a63  int..text:str..c
-0001ba00: 6c61 7373 204e 6577 7366 6565 6449 7465  lass NewsfeedIte
-0001ba10: 6d56 6964 656f 2857 616c 6c43 6172 6f75  mVideo(WallCarou
-0001ba20: 7365 6c42 6173 652c 204e 6577 7366 6565  selBase, Newsfee
-0001ba30: 6449 7465 6d42 6173 6529 3a0a 0976 6964  dItemBase):..vid
-0001ba40: 656f 3a4f 7074 696f 6e61 6c5b 224e 6577  eo:Optional["New
-0001ba50: 7366 6565 6449 7465 6d56 6964 656f 5669  sfeedItemVideoVi
-0001ba60: 6465 6f22 5d20 3d20 4e6f 6e65 0a0a 636c  deo"] = None..cl
-0001ba70: 6173 7320 4e65 7773 6665 6564 4c69 7374  ass NewsfeedList
-0001ba80: 4675 6c6c 284e 6577 7366 6565 644c 6973  Full(NewsfeedLis
-0001ba90: 7429 3a0a 096e 6f5f 7265 706f 7374 733a  t):..no_reposts:
-0001baa0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-0001bab0: 204e 6f6e 650a 0973 6f75 7263 655f 6964   None..source_id
-0001bac0: 733a 4f70 7469 6f6e 616c 5b6c 6973 745b  s:Optional[list[
-0001bad0: 696e 745d 5d20 3d20 4e6f 6e65 0a0a 636c  int]] = None..cl
-0001bae0: 6173 7320 4e65 7773 6665 6564 4e65 7773  ass NewsfeedNews
-0001baf0: 6665 6564 5068 6f74 6f28 5068 6f74 6f73  feedPhoto(Photos
-0001bb00: 5068 6f74 6f29 3a0a 096c 696b 6573 3a4f  Photo):..likes:O
-0001bb10: 7074 696f 6e61 6c5b 2242 6173 654c 696b  ptional["BaseLik
-0001bb20: 6573 225d 203d 204e 6f6e 650a 0963 6f6d  es"] = None..com
-0001bb30: 6d65 6e74 733a 4f70 7469 6f6e 616c 5b22  ments:Optional["
-0001bb40: 4261 7365 4f62 6a65 6374 436f 756e 7422  BaseObjectCount"
-0001bb50: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 7265  ] = None..can_re
-0001bb60: 706f 7374 3a4f 7074 696f 6e61 6c5b 626f  post:Optional[bo
-0001bb70: 6f6c 5d20 3d20 4e6f 6e65 0a0a 636c 6173  ol] = None..clas
-0001bb80: 7320 4e6f 7469 6669 6361 7469 6f6e 734e  s NotificationsN
-0001bb90: 6f74 6966 6963 6174 696f 6e50 6172 656e  otificationParen
-0001bba0: 7428 5761 6c6c 5761 6c6c 706f 7374 546f  t(WallWallpostTo
-0001bbb0: 4964 2c20 5068 6f74 6f73 5068 6f74 6f2c  Id, PhotosPhoto,
-0001bbc0: 2042 6f61 7264 546f 7069 632c 2056 6964   BoardTopic, Vid
-0001bbd0: 656f 5669 6465 6f2c 204e 6f74 6966 6963  eoVideo, Notific
-0001bbe0: 6174 696f 6e73 4e6f 7469 6669 6361 7469  ationsNotificati
-0001bbf0: 6f6e 7343 6f6d 6d65 6e74 293a 0a09 7061  onsComment):..pa
-0001bc00: 7373 0a63 6c61 7373 2055 7365 7273 5573  ss.class UsersUs
-0001bc10: 6572 2855 7365 7273 5573 6572 4d69 6e29  er(UsersUserMin)
-0001bc20: 3a0a 0973 6578 3a4f 7074 696f 6e61 6c5b  :..sex:Optional[
-0001bc30: 2242 6173 6553 6578 225d 203d 204e 6f6e  "BaseSex"] = Non
-0001bc40: 650a 0973 6372 6565 6e5f 6e61 6d65 3a4f  e..screen_name:O
-0001bc50: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0001bc60: 6f6e 650a 0970 686f 746f 5f35 303a 4f70  one..photo_50:Op
-0001bc70: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001bc80: 6e65 0a09 7068 6f74 6f5f 3130 303a 4f70  ne..photo_100:Op
-0001bc90: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001bca0: 6e65 0a09 6f6e 6c69 6e65 5f69 6e66 6f3a  ne..online_info:
-0001bcb0: 4f70 7469 6f6e 616c 5b22 5573 6572 734f  Optional["UsersO
-0001bcc0: 6e6c 696e 6549 6e66 6f22 5d20 3d20 4e6f  nlineInfo"] = No
-0001bcd0: 6e65 0a09 6f6e 6c69 6e65 3a4f 7074 696f  ne..online:Optio
-0001bce0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001bcf0: 0a09 6f6e 6c69 6e65 5f6d 6f62 696c 653a  ..online_mobile:
-0001bd00: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-0001bd10: 204e 6f6e 650a 096f 6e6c 696e 655f 6170   None..online_ap
-0001bd20: 703a 4f70 7469 6f6e 616c 5b69 6e74 5d20  p:Optional[int] 
-0001bd30: 3d20 4e6f 6e65 0a09 7665 7269 6669 6564  = None..verified
-0001bd40: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-0001bd50: 3d20 4e6f 6e65 0a09 7472 656e 6469 6e67  = None..trending
-0001bd60: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-0001bd70: 3d20 4e6f 6e65 0a09 6672 6965 6e64 5f73  = None..friend_s
-0001bd80: 7461 7475 733a 4f70 7469 6f6e 616c 5b22  tatus:Optional["
-0001bd90: 4672 6965 6e64 7346 7269 656e 6453 7461  FriendsFriendSta
-0001bda0: 7475 7353 7461 7475 7322 5d20 3d20 4e6f  tusStatus"] = No
-0001bdb0: 6e65 0a09 6d75 7475 616c 3a4f 7074 696f  ne..mutual:Optio
-0001bdc0: 6e61 6c5b 2246 7269 656e 6473 5265 7175  nal["FriendsRequ
-0001bdd0: 6573 7473 4d75 7475 616c 225d 203d 204e  estsMutual"] = N
-0001bde0: 6f6e 650a 0a63 6c61 7373 2055 7365 7273  one..class Users
-0001bdf0: 5573 6572 4675 6c6c 2855 7365 7273 5573  UserFull(UsersUs
-0001be00: 6572 293a 0a09 6669 7273 745f 6e61 6d65  er):..first_name
-0001be10: 5f6e 6f6d 3a4f 7074 696f 6e61 6c5b 7374  _nom:Optional[st
-0001be20: 725d 203d 204e 6f6e 650a 0966 6972 7374  r] = None..first
-0001be30: 5f6e 616d 655f 6765 6e3a 4f70 7469 6f6e  _name_gen:Option
-0001be40: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001be50: 6669 7273 745f 6e61 6d65 5f64 6174 3a4f  first_name_dat:O
-0001be60: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0001be70: 6f6e 650a 0966 6972 7374 5f6e 616d 655f  one..first_name_
-0001be80: 6163 633a 4f70 7469 6f6e 616c 5b73 7472  acc:Optional[str
-0001be90: 5d20 3d20 4e6f 6e65 0a09 6669 7273 745f  ] = None..first_
-0001bea0: 6e61 6d65 5f69 6e73 3a4f 7074 696f 6e61  name_ins:Optiona
-0001beb0: 6c5b 7374 725d 203d 204e 6f6e 650a 0966  l[str] = None..f
-0001bec0: 6972 7374 5f6e 616d 655f 6162 6c3a 4f70  irst_name_abl:Op
-0001bed0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001bee0: 6e65 0a09 6c61 7374 5f6e 616d 655f 6e6f  ne..last_name_no
-0001bef0: 6d3a 4f70 7469 6f6e 616c 5b73 7472 5d20  m:Optional[str] 
-0001bf00: 3d20 4e6f 6e65 0a09 6c61 7374 5f6e 616d  = None..last_nam
-0001bf10: 655f 6765 6e3a 4f70 7469 6f6e 616c 5b73  e_gen:Optional[s
-0001bf20: 7472 5d20 3d20 4e6f 6e65 0a09 6c61 7374  tr] = None..last
-0001bf30: 5f6e 616d 655f 6461 743a 4f70 7469 6f6e  _name_dat:Option
-0001bf40: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001bf50: 6c61 7374 5f6e 616d 655f 6163 633a 4f70  last_name_acc:Op
-0001bf60: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001bf70: 6e65 0a09 6c61 7374 5f6e 616d 655f 696e  ne..last_name_in
-0001bf80: 733a 4f70 7469 6f6e 616c 5b73 7472 5d20  s:Optional[str] 
-0001bf90: 3d20 4e6f 6e65 0a09 6c61 7374 5f6e 616d  = None..last_nam
-0001bfa0: 655f 6162 6c3a 4f70 7469 6f6e 616c 5b73  e_abl:Optional[s
-0001bfb0: 7472 5d20 3d20 4e6f 6e65 0a09 6e69 636b  tr] = None..nick
-0001bfc0: 6e61 6d65 3a4f 7074 696f 6e61 6c5b 7374  name:Optional[st
-0001bfd0: 725d 203d 204e 6f6e 650a 096d 6169 6465  r] = None..maide
-0001bfe0: 6e5f 6e61 6d65 3a4f 7074 696f 6e61 6c5b  n_name:Optional[
-0001bff0: 7374 725d 203d 204e 6f6e 650a 0963 6f6e  str] = None..con
-0001c000: 7461 6374 5f6e 616d 653a 4f70 7469 6f6e  tact_name:Option
-0001c010: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001c020: 646f 6d61 696e 3a4f 7074 696f 6e61 6c5b  domain:Optional[
-0001c030: 7374 725d 203d 204e 6f6e 650a 0962 6461  str] = None..bda
-0001c040: 7465 3a4f 7074 696f 6e61 6c5b 7374 725d  te:Optional[str]
-0001c050: 203d 204e 6f6e 650a 0963 6974 793a 4f70   = None..city:Op
-0001c060: 7469 6f6e 616c 5b22 4261 7365 4369 7479  tional["BaseCity
-0001c070: 225d 203d 204e 6f6e 650a 0963 6f75 6e74  "] = None..count
-0001c080: 7279 3a4f 7074 696f 6e61 6c5b 2242 6173  ry:Optional["Bas
-0001c090: 6543 6f75 6e74 7279 225d 203d 204e 6f6e  eCountry"] = Non
-0001c0a0: 650a 0974 696d 657a 6f6e 653a 4f70 7469  e..timezone:Opti
-0001c0b0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-0001c0c0: 0a09 6f77 6e65 725f 7374 6174 653a 4f70  ..owner_state:Op
-0001c0d0: 7469 6f6e 616c 5b22 4f77 6e65 7253 7461  tional["OwnerSta
-0001c0e0: 7465 225d 203d 204e 6f6e 650a 0970 686f  te"] = None..pho
-0001c0f0: 746f 5f32 3030 3a4f 7074 696f 6e61 6c5b  to_200:Optional[
-0001c100: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
-0001c110: 746f 5f6d 6178 3a4f 7074 696f 6e61 6c5b  to_max:Optional[
-0001c120: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
-0001c130: 746f 5f32 3030 5f6f 7269 673a 4f70 7469  to_200_orig:Opti
-0001c140: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0001c150: 0a09 7068 6f74 6f5f 3430 305f 6f72 6967  ..photo_400_orig
-0001c160: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-0001c170: 204e 6f6e 650a 0970 686f 746f 5f6d 6178   None..photo_max
-0001c180: 5f6f 7269 673a 4f70 7469 6f6e 616c 5b73  _orig:Optional[s
-0001c190: 7472 5d20 3d20 4e6f 6e65 0a09 7068 6f74  tr] = None..phot
-0001c1a0: 6f5f 6964 3a4f 7074 696f 6e61 6c5b 7374  o_id:Optional[st
-0001c1b0: 725d 203d 204e 6f6e 650a 0968 6173 5f70  r] = None..has_p
-0001c1c0: 686f 746f 3a4f 7074 696f 6e61 6c5b 626f  hoto:Optional[bo
-0001c1d0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6861 735f  ol] = None..has_
-0001c1e0: 6d6f 6269 6c65 3a4f 7074 696f 6e61 6c5b  mobile:Optional[
-0001c1f0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6973  bool] = None..is
-0001c200: 5f66 7269 656e 643a 4f70 7469 6f6e 616c  _friend:Optional
-0001c210: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0977  [bool] = None..w
-0001c220: 616c 6c5f 636f 6d6d 656e 7473 3a4f 7074  all_comments:Opt
-0001c230: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-0001c240: 6e65 0a09 6361 6e5f 706f 7374 3a4f 7074  ne..can_post:Opt
-0001c250: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-0001c260: 6e65 0a09 6361 6e5f 7365 655f 616c 6c5f  ne..can_see_all_
-0001c270: 706f 7374 733a 4f70 7469 6f6e 616c 5b62  posts:Optional[b
-0001c280: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
-0001c290: 5f73 6565 5f61 7564 696f 3a4f 7074 696f  _see_audio:Optio
-0001c2a0: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001c2b0: 0a09 7479 7065 3a4f 7074 696f 6e61 6c5b  ..type:Optional[
-0001c2c0: 2255 7365 7273 5573 6572 5479 7065 225d  "UsersUserType"]
-0001c2d0: 203d 204e 6f6e 650a 0965 6d61 696c 3a4f   = None..email:O
-0001c2e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0001c2f0: 6f6e 650a 0973 6b79 7065 3a4f 7074 696f  one..skype:Optio
-0001c300: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-0001c310: 0966 6163 6562 6f6f 6b3a 4f70 7469 6f6e  .facebook:Option
-0001c320: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001c330: 6661 6365 626f 6f6b 5f6e 616d 653a 4f70  facebook_name:Op
-0001c340: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001c350: 6e65 0a09 7477 6974 7465 723a 4f70 7469  ne..twitter:Opti
-0001c360: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0001c370: 0a09 6c69 7665 6a6f 7572 6e61 6c3a 4f70  ..livejournal:Op
-0001c380: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001c390: 6e65 0a09 696e 7374 6167 7261 6d3a 4f70  ne..instagram:Op
-0001c3a0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001c3b0: 6e65 0a09 7465 7374 3a4f 7074 696f 6e61  ne..test:Optiona
-0001c3c0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0001c3d0: 7669 6465 6f5f 6c69 7665 3a4f 7074 696f  video_live:Optio
-0001c3e0: 6e61 6c5b 2256 6964 656f 4c69 7665 496e  nal["VideoLiveIn
-0001c3f0: 666f 225d 203d 204e 6f6e 650a 0969 735f  fo"] = None..is_
-0001c400: 7669 6465 6f5f 6c69 7665 5f6e 6f74 6966  video_live_notif
-0001c410: 6963 6174 696f 6e73 5f62 6c6f 636b 6564  ications_blocked
-0001c420: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-0001c430: 3d20 4e6f 6e65 0a09 6973 5f73 6572 7669  = None..is_servi
-0001c440: 6365 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ce:Optional[bool
-0001c450: 5d20 3d20 4e6f 6e65 0a09 7365 7276 6963  ] = None..servic
-0001c460: 655f 6465 7363 7269 7074 696f 6e3a 4f70  e_description:Op
-0001c470: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001c480: 6e65 0a09 7068 6f74 6f5f 7265 633a 4f70  ne..photo_rec:Op
-0001c490: 7469 6f6e 616c 5b22 5068 6f74 6f73 5068  tional["PhotosPh
-0001c4a0: 6f74 6f46 616c 7365 6162 6c65 225d 203d  otoFalseable"] =
-0001c4b0: 204e 6f6e 650a 0970 686f 746f 5f6d 6564   None..photo_med
-0001c4c0: 6975 6d3a 4f70 7469 6f6e 616c 5b22 5068  ium:Optional["Ph
-0001c4d0: 6f74 6f73 5068 6f74 6f46 616c 7365 6162  otosPhotoFalseab
-0001c4e0: 6c65 225d 203d 204e 6f6e 650a 0970 686f  le"] = None..pho
-0001c4f0: 746f 5f6d 6564 6975 6d5f 7265 633a 4f70  to_medium_rec:Op
-0001c500: 7469 6f6e 616c 5b22 5068 6f74 6f73 5068  tional["PhotosPh
-0001c510: 6f74 6f46 616c 7365 6162 6c65 225d 203d  otoFalseable"] =
-0001c520: 204e 6f6e 650a 0970 686f 746f 3a4f 7074   None..photo:Opt
-0001c530: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001c540: 650a 0970 686f 746f 5f62 6967 3a4f 7074  e..photo_big:Opt
-0001c550: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001c560: 650a 0970 686f 746f 5f34 3030 3a4f 7074  e..photo_400:Opt
-0001c570: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001c580: 650a 0970 686f 746f 5f6d 6178 5f73 697a  e..photo_max_siz
-0001c590: 653a 4f70 7469 6f6e 616c 5b22 5068 6f74  e:Optional["Phot
-0001c5a0: 6f73 5068 6f74 6f22 5d20 3d20 4e6f 6e65  osPhoto"] = None
-0001c5b0: 0a09 6c61 6e67 7561 6765 3a4f 7074 696f  ..language:Optio
-0001c5c0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-0001c5d0: 0973 746f 7269 6573 5f61 7263 6869 7665  .stories_archive
-0001c5e0: 5f63 6f75 6e74 3a4f 7074 696f 6e61 6c5b  _count:Optional[
-0001c5f0: 696e 745d 203d 204e 6f6e 650a 0968 6173  int] = None..has
-0001c600: 5f75 6e73 6565 6e5f 7374 6f72 6965 733a  _unseen_stories:
-0001c610: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-0001c620: 204e 6f6e 650a 0977 616c 6c5f 6465 6661   None..wall_defa
-0001c630: 756c 743a 4f70 7469 6f6e 616c 5b73 7472  ult:Optional[str
-0001c640: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 6361  ] = None..can_ca
-0001c650: 6c6c 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ll:Optional[bool
-0001c660: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 6361  ] = None..can_ca
-0001c670: 6c6c 5f66 726f 6d5f 6772 6f75 703a 4f70  ll_from_group:Op
-0001c680: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-0001c690: 6f6e 650a 0963 616e 5f73 6565 5f77 6973  one..can_see_wis
-0001c6a0: 6865 733a 4f70 7469 6f6e 616c 5b62 6f6f  hes:Optional[boo
-0001c6b0: 6c5d 203d 204e 6f6e 650a 0963 616e 5f73  l] = None..can_s
-0001c6c0: 6565 5f67 6966 7473 3a4f 7074 696f 6e61  ee_gifts:Optiona
-0001c6d0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0001c6e0: 696e 7465 7265 7374 733a 4f70 7469 6f6e  interests:Option
-0001c6f0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001c700: 626f 6f6b 733a 4f70 7469 6f6e 616c 5b73  books:Optional[s
-0001c710: 7472 5d20 3d20 4e6f 6e65 0a09 7476 3a4f  tr] = None..tv:O
-0001c720: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0001c730: 6f6e 650a 0971 756f 7465 733a 4f70 7469  one..quotes:Opti
-0001c740: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0001c750: 0a09 6162 6f75 743a 4f70 7469 6f6e 616c  ..about:Optional
-0001c760: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6761  [str] = None..ga
-0001c770: 6d65 733a 4f70 7469 6f6e 616c 5b73 7472  mes:Optional[str
-0001c780: 5d20 3d20 4e6f 6e65 0a09 6d6f 7669 6573  ] = None..movies
-0001c790: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-0001c7a0: 204e 6f6e 650a 0961 6374 6976 6974 6965   None..activitie
-0001c7b0: 733a 4f70 7469 6f6e 616c 5b73 7472 5d20  s:Optional[str] 
-0001c7c0: 3d20 4e6f 6e65 0a09 6d75 7369 633a 4f70  = None..music:Op
-0001c7d0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001c7e0: 6e65 0a09 6361 6e5f 7772 6974 655f 7072  ne..can_write_pr
-0001c7f0: 6976 6174 655f 6d65 7373 6167 653a 4f70  ivate_message:Op
-0001c800: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
-0001c810: 6f6e 650a 0963 616e 5f73 656e 645f 6672  one..can_send_fr
-0001c820: 6965 6e64 5f72 6571 7565 7374 3a4f 7074  iend_request:Opt
-0001c830: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-0001c840: 6e65 0a09 6361 6e5f 6265 5f69 6e76 6974  ne..can_be_invit
-0001c850: 6564 5f67 726f 7570 3a4f 7074 696f 6e61  ed_group:Optiona
-0001c860: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
-0001c870: 6d6f 6269 6c65 5f70 686f 6e65 3a4f 7074  mobile_phone:Opt
-0001c880: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001c890: 650a 0968 6f6d 655f 7068 6f6e 653a 4f70  e..home_phone:Op
-0001c8a0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001c8b0: 6e65 0a09 7369 7465 3a4f 7074 696f 6e61  ne..site:Optiona
-0001c8c0: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
-0001c8d0: 7461 7475 735f 6175 6469 6f3a 4f70 7469  tatus_audio:Opti
-0001c8e0: 6f6e 616c 5b22 4175 6469 6f41 7564 696f  onal["AudioAudio
-0001c8f0: 225d 203d 204e 6f6e 650a 0973 7461 7475  "] = None..statu
-0001c900: 733a 4f70 7469 6f6e 616c 5b73 7472 5d20  s:Optional[str] 
-0001c910: 3d20 4e6f 6e65 0a09 6163 7469 7669 7479  = None..activity
-0001c920: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
-0001c930: 204e 6f6e 650a 096c 6173 745f 7365 656e   None..last_seen
-0001c940: 3a4f 7074 696f 6e61 6c5b 2255 7365 7273  :Optional["Users
-0001c950: 4c61 7374 5365 656e 225d 203d 204e 6f6e  LastSeen"] = Non
-0001c960: 650a 0965 7870 6f72 7473 3a4f 7074 696f  e..exports:Optio
-0001c970: 6e61 6c5b 2255 7365 7273 4578 706f 7274  nal["UsersExport
-0001c980: 7322 5d20 3d20 4e6f 6e65 0a09 6372 6f70  s"] = None..crop
-0001c990: 5f70 686f 746f 3a4f 7074 696f 6e61 6c5b  _photo:Optional[
-0001c9a0: 2242 6173 6543 726f 7050 686f 746f 225d  "BaseCropPhoto"]
-0001c9b0: 203d 204e 6f6e 650a 0966 6f6c 6c6f 7765   = None..followe
-0001c9c0: 7273 5f63 6f75 6e74 3a4f 7074 696f 6e61  rs_count:Optiona
-0001c9d0: 6c5b 696e 745d 203d 204e 6f6e 650a 0976  l[int] = None..v
-0001c9e0: 6964 656f 5f6c 6976 655f 6c65 7665 6c3a  ideo_live_level:
-0001c9f0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-0001ca00: 4e6f 6e65 0a09 7669 6465 6f5f 6c69 7665  None..video_live
-0001ca10: 5f63 6f75 6e74 3a4f 7074 696f 6e61 6c5b  _count:Optional[
-0001ca20: 696e 745d 203d 204e 6f6e 650a 0963 6c69  int] = None..cli
-0001ca30: 7073 5f63 6f75 6e74 3a4f 7074 696f 6e61  ps_count:Optiona
-0001ca40: 6c5b 696e 745d 203d 204e 6f6e 650a 0962  l[int] = None..b
-0001ca50: 6c61 636b 6c69 7374 6564 3a4f 7074 696f  lacklisted:Optio
-0001ca60: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001ca70: 0a09 626c 6163 6b6c 6973 7465 645f 6279  ..blacklisted_by
-0001ca80: 5f6d 653a 4f70 7469 6f6e 616c 5b62 6f6f  _me:Optional[boo
-0001ca90: 6c5d 203d 204e 6f6e 650a 0969 735f 6661  l] = None..is_fa
-0001caa0: 766f 7269 7465 3a4f 7074 696f 6e61 6c5b  vorite:Optional[
-0001cab0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6973  bool] = None..is
-0001cac0: 5f68 6964 6465 6e5f 6672 6f6d 5f66 6565  _hidden_from_fee
-0001cad0: 643a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  d:Optional[bool]
-0001cae0: 203d 204e 6f6e 650a 0963 6f6d 6d6f 6e5f   = None..common_
-0001caf0: 636f 756e 743a 4f70 7469 6f6e 616c 5b69  count:Optional[i
-0001cb00: 6e74 5d20 3d20 4e6f 6e65 0a09 6f63 6375  nt] = None..occu
-0001cb10: 7061 7469 6f6e 3a4f 7074 696f 6e61 6c5b  pation:Optional[
-0001cb20: 2255 7365 7273 4f63 6375 7061 7469 6f6e  "UsersOccupation
-0001cb30: 225d 203d 204e 6f6e 650a 0963 6172 6565  "] = None..caree
-0001cb40: 723a 4f70 7469 6f6e 616c 5b6c 6973 745b  r:Optional[list[
-0001cb50: 2255 7365 7273 4361 7265 6572 225d 5d20  "UsersCareer"]] 
-0001cb60: 3d20 4e6f 6e65 0a09 6d69 6c69 7461 7279  = None..military
-0001cb70: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
-0001cb80: 5573 6572 734d 696c 6974 6172 7922 5d5d  UsersMilitary"]]
-0001cb90: 203d 204e 6f6e 650a 0975 6e69 7665 7273   = None..univers
-0001cba0: 6974 793a 4f70 7469 6f6e 616c 5b69 6e74  ity:Optional[int
-0001cbb0: 5d20 3d20 4e6f 6e65 0a09 756e 6976 6572  ] = None..univer
-0001cbc0: 7369 7479 5f6e 616d 653a 4f70 7469 6f6e  sity_name:Option
-0001cbd0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a09  al[str] = None..
-0001cbe0: 756e 6976 6572 7369 7479 5f67 726f 7570  university_group
-0001cbf0: 5f69 643a 4f70 7469 6f6e 616c 5b69 6e74  _id:Optional[int
-0001cc00: 5d20 3d20 4e6f 6e65 0a09 6661 6375 6c74  ] = None..facult
-0001cc10: 793a 4f70 7469 6f6e 616c 5b69 6e74 5d20  y:Optional[int] 
-0001cc20: 3d20 4e6f 6e65 0a09 6661 6375 6c74 795f  = None..faculty_
-0001cc30: 6e61 6d65 3a4f 7074 696f 6e61 6c5b 7374  name:Optional[st
-0001cc40: 725d 203d 204e 6f6e 650a 0967 7261 6475  r] = None..gradu
-0001cc50: 6174 696f 6e3a 4f70 7469 6f6e 616c 5b69  ation:Optional[i
-0001cc60: 6e74 5d20 3d20 4e6f 6e65 0a09 6564 7563  nt] = None..educ
-0001cc70: 6174 696f 6e5f 666f 726d 3a4f 7074 696f  ation_form:Optio
-0001cc80: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-0001cc90: 0965 6475 6361 7469 6f6e 5f73 7461 7475  .education_statu
-0001cca0: 733a 4f70 7469 6f6e 616c 5b73 7472 5d20  s:Optional[str] 
-0001ccb0: 3d20 4e6f 6e65 0a09 686f 6d65 5f74 6f77  = None..home_tow
-0001ccc0: 6e3a 4f70 7469 6f6e 616c 5b73 7472 5d20  n:Optional[str] 
-0001ccd0: 3d20 4e6f 6e65 0a09 7265 6c61 7469 6f6e  = None..relation
-0001cce0: 3a4f 7074 696f 6e61 6c5b 2255 7365 7273  :Optional["Users
-0001ccf0: 5573 6572 5265 6c61 7469 6f6e 225d 203d  UserRelation"] =
-0001cd00: 204e 6f6e 650a 0972 656c 6174 696f 6e5f   None..relation_
-0001cd10: 7061 7274 6e65 723a 4f70 7469 6f6e 616c  partner:Optional
-0001cd20: 5b22 5573 6572 7355 7365 724d 696e 225d  ["UsersUserMin"]
-0001cd30: 203d 204e 6f6e 650a 0970 6572 736f 6e61   = None..persona
-0001cd40: 6c3a 4f70 7469 6f6e 616c 5b22 5573 6572  l:Optional["User
-0001cd50: 7350 6572 736f 6e61 6c22 5d20 3d20 4e6f  sPersonal"] = No
-0001cd60: 6e65 0a09 756e 6976 6572 7369 7469 6573  ne..universities
-0001cd70: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b22  :Optional[list["
-0001cd80: 5573 6572 7355 6e69 7665 7273 6974 7922  UsersUniversity"
-0001cd90: 5d5d 203d 204e 6f6e 650a 0973 6368 6f6f  ]] = None..schoo
-0001cda0: 6c73 3a4f 7074 696f 6e61 6c5b 6c69 7374  ls:Optional[list
-0001cdb0: 5b22 5573 6572 7353 6368 6f6f 6c22 5d5d  ["UsersSchool"]]
-0001cdc0: 203d 204e 6f6e 650a 0972 656c 6174 6976   = None..relativ
-0001cdd0: 6573 3a4f 7074 696f 6e61 6c5b 6c69 7374  es:Optional[list
-0001cde0: 5b22 5573 6572 7352 656c 6174 6976 6522  ["UsersRelative"
-0001cdf0: 5d5d 203d 204e 6f6e 650a 0969 735f 7375  ]] = None..is_su
-0001ce00: 6273 6372 6962 6564 5f70 6f64 6361 7374  bscribed_podcast
-0001ce10: 733a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  s:Optional[bool]
-0001ce20: 203d 204e 6f6e 650a 0963 616e 5f73 7562   = None..can_sub
-0001ce30: 7363 7269 6265 5f70 6f64 6361 7374 733a  scribe_podcasts:
-0001ce40: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-0001ce50: 204e 6f6e 650a 0963 616e 5f73 7562 7363   None..can_subsc
-0001ce60: 7269 6265 5f70 6f73 7473 3a4f 7074 696f  ribe_posts:Optio
-0001ce70: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001ce80: 0a09 636f 756e 7465 7273 3a4f 7074 696f  ..counters:Optio
-0001ce90: 6e61 6c5b 2255 7365 7273 5573 6572 436f  nal["UsersUserCo
-0001cea0: 756e 7465 7273 225d 203d 204e 6f6e 650a  unters"] = None.
-0001ceb0: 0961 6363 6573 735f 6b65 793a 4f70 7469  .access_key:Opti
-0001cec0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0001ced0: 0a09 6361 6e5f 7570 6c6f 6164 5f64 6f63  ..can_upload_doc
-0001cee0: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
-0001cef0: 3d20 4e6f 6e65 0a09 6861 7368 3a4f 7074  = None..hash:Opt
-0001cf00: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0001cf10: 650a 0969 735f 6e6f 5f69 6e64 6578 3a4f  e..is_no_index:O
-0001cf20: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-0001cf30: 4e6f 6e65 0a09 636f 6e74 6163 745f 6964  None..contact_id
-0001cf40: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-0001cf50: 204e 6f6e 650a 0969 735f 6d65 7373 6167   None..is_messag
-0001cf60: 655f 7265 7175 6573 743a 4f70 7469 6f6e  e_request:Option
-0001cf70: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
-0001cf80: 0964 6573 6372 6970 7469 6f6e 733a 4f70  .descriptions:Op
-0001cf90: 7469 6f6e 616c 5b6c 6973 745b 7374 725d  tional[list[str]
-0001cfa0: 5d20 3d20 4e6f 6e65 0a09 6c69 7374 733a  ] = None..lists:
-0001cfb0: 4f70 7469 6f6e 616c 5b6c 6973 745b 696e  Optional[list[in
-0001cfc0: 745d 5d20 3d20 4e6f 6e65 0a0a 636c 6173  t]] = None..clas
-0001cfd0: 7320 5573 6572 7355 7365 7258 7472 5479  s UsersUserXtrTy
-0001cfe0: 7065 2855 7365 7273 5573 6572 293a 0a09  pe(UsersUser):..
-0001cff0: 7479 7065 3a4f 7074 696f 6e61 6c5b 2255  type:Optional["U
-0001d000: 7365 7273 5573 6572 5479 7065 225d 203d  sersUserType"] =
-0001d010: 204e 6f6e 650a 0a63 6c61 7373 2056 6964   None..class Vid
-0001d020: 656f 5669 6465 6f41 6c62 756d 4675 6c6c  eoVideoAlbumFull
-0001d030: 2856 6964 656f 5669 6465 6f41 6c62 756d  (VideoVideoAlbum
-0001d040: 293a 0a09 636f 756e 743a 696e 740a 0969  ):..count:int..i
-0001d050: 6d61 6765 3a4f 7074 696f 6e61 6c5b 6c69  mage:Optional[li
-0001d060: 7374 5b22 5669 6465 6f56 6964 656f 496d  st["VideoVideoIm
-0001d070: 6167 6522 5d5d 203d 204e 6f6e 650a 0969  age"]] = None..i
-0001d080: 6d61 6765 5f62 6c75 723a 4f70 7469 6f6e  mage_blur:Option
-0001d090: 616c 5b22 4261 7365 5072 6f70 6572 7479  al["BaseProperty
-0001d0a0: 4578 6973 7473 225d 203d 204e 6f6e 650a  Exists"] = None.
-0001d0b0: 0969 735f 7379 7374 656d 3a4f 7074 696f  .is_system:Optio
-0001d0c0: 6e61 6c5b 2242 6173 6550 726f 7065 7274  nal["BasePropert
-0001d0d0: 7945 7869 7374 7322 5d20 3d20 4e6f 6e65  yExists"] = None
-0001d0e0: 0a09 7570 6461 7465 645f 7469 6d65 3a69  ..updated_time:i
-0001d0f0: 6e74 0a0a 636c 6173 7320 5669 6465 6f56  nt..class VideoV
-0001d100: 6964 656f 4675 6c6c 2856 6964 656f 5669  ideoFull(VideoVi
-0001d110: 6465 6f29 3a0a 0966 696c 6573 3a4f 7074  deo):..files:Opt
-0001d120: 696f 6e61 6c5b 2256 6964 656f 5669 6465  ional["VideoVide
-0001d130: 6f46 696c 6573 225d 203d 204e 6f6e 650a  oFiles"] = None.
-0001d140: 0974 7261 696c 6572 3a4f 7074 696f 6e61  .trailer:Optiona
-0001d150: 6c5b 2256 6964 656f 5669 6465 6f46 696c  l["VideoVideoFil
-0001d160: 6573 225d 203d 204e 6f6e 650a 096c 6976  es"] = None..liv
-0001d170: 655f 7365 7474 696e 6773 3a4f 7074 696f  e_settings:Optio
-0001d180: 6e61 6c5b 2256 6964 656f 4c69 7665 5365  nal["VideoLiveSe
-0001d190: 7474 696e 6773 225d 203d 204e 6f6e 650a  ttings"] = None.
-0001d1a0: 0a63 6c61 7373 2056 6964 656f 5669 6465  .class VideoVide
-0001d1b0: 6f49 6d61 6765 2842 6173 6549 6d61 6765  oImage(BaseImage
-0001d1c0: 293a 0a09 7769 7468 5f70 6164 6469 6e67  ):..with_padding
-0001d1d0: 3a4f 7074 696f 6e61 6c5b 2242 6173 6550  :Optional["BaseP
-0001d1e0: 726f 7065 7274 7945 7869 7374 7322 5d20  ropertyExists"] 
-0001d1f0: 3d20 4e6f 6e65 0a0a 636c 6173 7320 5761  = None..class Wa
-0001d200: 6c6c 5761 6c6c 706f 7374 4675 6c6c 2857  llWallpostFull(W
-0001d210: 616c 6c43 6172 6f75 7365 6c42 6173 652c  allCarouselBase,
-0001d220: 2057 616c 6c57 616c 6c70 6f73 7429 3a0a   WallWallpost):.
-0001d230: 0963 6f70 795f 6869 7374 6f72 793a 4f70  .copy_history:Op
-0001d240: 7469 6f6e 616c 5b6c 6973 745b 2257 616c  tional[list["Wal
-0001d250: 6c57 616c 6c70 6f73 7446 756c 6c22 5d5d  lWallpostFull"]]
-0001d260: 203d 204e 6f6e 650a 0963 616e 5f65 6469   = None..can_edi
-0001d270: 743a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  t:Optional[bool]
-0001d280: 203d 204e 6f6e 650a 0963 7265 6174 6564   = None..created
-0001d290: 5f62 793a 4f70 7469 6f6e 616c 5b69 6e74  _by:Optional[int
-0001d2a0: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 6465  ] = None..can_de
-0001d2b0: 6c65 7465 3a4f 7074 696f 6e61 6c5b 626f  lete:Optional[bo
-0001d2c0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
-0001d2d0: 7069 6e3a 4f70 7469 6f6e 616c 5b62 6f6f  pin:Optional[boo
-0001d2e0: 6c5d 203d 204e 6f6e 650a 0964 6f6e 7574  l] = None..donut
-0001d2f0: 3a4f 7074 696f 6e61 6c5b 2257 616c 6c57  :Optional["WallW
-0001d300: 616c 6c70 6f73 7444 6f6e 7574 225d 203d  allpostDonut"] =
-0001d310: 204e 6f6e 650a 0969 735f 7069 6e6e 6564   None..is_pinned
-0001d320: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
-0001d330: 204e 6f6e 650a 0963 6f6d 6d65 6e74 733a   None..comments:
-0001d340: 4f70 7469 6f6e 616c 5b22 4261 7365 436f  Optional["BaseCo
-0001d350: 6d6d 656e 7473 496e 666f 225d 203d 204e  mmentsInfo"] = N
-0001d360: 6f6e 650a 096d 6172 6b65 645f 6173 5f61  one..marked_as_a
-0001d370: 6473 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ds:Optional[bool
-0001d380: 5d20 3d20 4e6f 6e65 0a09 746f 7069 635f  ] = None..topic_
-0001d390: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
-0001d3a0: 203d 204e 6f6e 650a 0973 686f 7274 5f74   = None..short_t
-0001d3b0: 6578 745f 7261 7465 3a4f 7074 696f 6e61  ext_rate:Optiona
-0001d3c0: 6c5b 696e 745d 203d 204e 6f6e 650a 0968  l[int] = None..h
-0001d3d0: 6173 683a 4f70 7469 6f6e 616c 5b73 7472  ash:Optional[str
-0001d3e0: 5d20 3d20 4e6f 6e65 0a0a 636c 6173 7320  ] = None..class 
-0001d3f0: 4d65 7373 6167 6573 5573 6572 5874 7249  MessagesUserXtrI
-0001d400: 6e76 6974 6564 4279 2855 7365 7273 5573  nvitedBy(UsersUs
-0001d410: 6572 5874 7254 7970 6529 3a0a 0969 6e76  erXtrType):..inv
-0001d420: 6974 6564 5f62 793a 4f70 7469 6f6e 616c  ited_by:Optional
-0001d430: 5b69 6e74 5d20 3d20 4e6f 6e65 0a0a 636c  [int] = None..cl
-0001d440: 6173 7320 4e65 7773 6665 6564 4974 656d  ass NewsfeedItem
-0001d450: 5761 6c6c 706f 7374 284e 6577 7366 6565  Wallpost(Newsfee
-0001d460: 6449 7465 6d42 6173 652c 2057 616c 6c57  dItemBase, WallW
-0001d470: 616c 6c70 6f73 7446 756c 6c29 3a0a 0966  allpostFull):..f
-0001d480: 6565 6462 6163 6b3a 4f70 7469 6f6e 616c  eedback:Optional
-0001d490: 5b22 4e65 7773 6665 6564 4974 656d 5761  ["NewsfeedItemWa
-0001d4a0: 6c6c 706f 7374 4665 6564 6261 636b 225d  llpostFeedback"]
-0001d4b0: 203d 204e 6f6e 650a 0a63 6c61 7373 2047   = None..class G
-0001d4c0: 726f 7570 7355 7365 7258 7472 526f 6c65  roupsUserXtrRole
-0001d4d0: 2855 7365 7273 5573 6572 4675 6c6c 293a  (UsersUserFull):
-0001d4e0: 0a09 726f 6c65 3a4f 7074 696f 6e61 6c5b  ..role:Optional[
-0001d4f0: 2247 726f 7570 7352 6f6c 654f 7074 696f  "GroupsRoleOptio
-0001d500: 6e73 225d 203d 204e 6f6e 650a 0a63 6c61  ns"] = None..cla
-0001d510: 7373 2046 7269 656e 6473 5573 6572 5874  ss FriendsUserXt
-0001d520: 7250 686f 6e65 2855 7365 7273 5573 6572  rPhone(UsersUser
-0001d530: 4675 6c6c 293a 0a09 7068 6f6e 653a 4f70  Full):..phone:Op
-0001d540: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0001d550: 6e65 0a0a 2320 d18d d182 d0be 20d0 bfd0  ne..# ...... ...
-0001d560: b8d0 b7d0 b4d0 b5d1 8620 d0bf d0be d0bb  ......... ......
-0001d570: d0bd d18b d0b9 0a66 6f72 2069 2069 6e20  .......for i in 
-0001d580: 2841 6363 6f75 6e74 4163 636f 756e 7443  (AccountAccountC
-0001d590: 6f75 6e74 6572 732c 2041 6363 6f75 6e74  ounters, Account
-0001d5a0: 496e 666f 2c20 4163 636f 756e 744e 616d  Info, AccountNam
-0001d5b0: 6552 6571 7565 7374 2c20 4163 636f 756e  eRequest, Accoun
-0001d5c0: 744e 616d 6552 6571 7565 7374 5374 6174  tNameRequestStat
-0001d5d0: 7573 2c20 4163 636f 756e 744f 6666 6572  us, AccountOffer
-0001d5e0: 2c20 4163 636f 756e 7450 7573 6843 6f6e  , AccountPushCon
-0001d5f0: 7665 7273 6174 696f 6e73 2c0a 2020 2020  versations,.    
-0001d600: 2020 2020 2020 4163 636f 756e 7450 7573        AccountPus
-0001d610: 6843 6f6e 7665 7273 6174 696f 6e73 4974  hConversationsIt
-0001d620: 656d 2c20 4163 636f 756e 7450 7573 6850  em, AccountPushP
-0001d630: 6172 616d 732c 2041 6363 6f75 6e74 5075  arams, AccountPu
-0001d640: 7368 5061 7261 6d73 4d6f 6465 2c20 4163  shParamsMode, Ac
-0001d650: 636f 756e 7450 7573 6850 6172 616d 734f  countPushParamsO
-0001d660: 6e6f 6666 2c20 4163 636f 756e 7450 7573  noff, AccountPus
-0001d670: 6850 6172 616d 7353 6574 7469 6e67 732c  hParamsSettings,
-0001d680: 0a20 2020 2020 2020 2020 2041 6363 6f75  .          Accou
-0001d690: 6e74 5075 7368 5365 7474 696e 6773 2c20  ntPushSettings, 
-0001d6a0: 4163 636f 756e 7453 7562 7363 7269 7074  AccountSubscript
-0001d6b0: 696f 6e73 2c20 4163 636f 756e 7455 7365  ions, AccountUse
-0001d6c0: 7253 6574 7469 6e67 732c 2041 6363 6f75  rSettings, Accou
-0001d6d0: 6e74 5573 6572 5365 7474 696e 6773 496e  ntUserSettingsIn
-0001d6e0: 7465 7265 7374 2c20 4163 636f 756e 7455  terest, AccountU
-0001d6f0: 7365 7253 6574 7469 6e67 7349 6e74 6572  serSettingsInter
-0001d700: 6573 7473 2c20 4164 6472 6573 7365 7346  ests, AddressesF
-0001d710: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
-0001d720: 2041 6473 4163 6365 7373 526f 6c65 2c20   AdsAccessRole, 
-0001d730: 4164 7341 6363 6573 7352 6f6c 6550 7562  AdsAccessRolePub
-0001d740: 6c69 632c 2041 6473 4163 6365 7373 6573  lic, AdsAccesses
-0001d750: 2c20 4164 7341 6363 6f75 6e74 2c20 4164  , AdsAccount, Ad
-0001d760: 7341 6363 6f75 6e74 5479 7065 2c20 4164  sAccountType, Ad
-0001d770: 7341 642c 2041 6473 4164 4170 7072 6f76  sAd, AdsAdApprov
-0001d780: 6564 2c20 4164 7341 6443 6f73 7454 7970  ed, AdsAdCostTyp
-0001d790: 652c 2041 6473 4164 4c61 796f 7574 2c20  e, AdsAdLayout, 
-0001d7a0: 4164 7341 6453 7461 7475 732c 0a20 2020  AdsAdStatus,.   
-0001d7b0: 2020 2020 2020 2041 6473 4361 6d70 6169         AdsCampai
-0001d7c0: 676e 2c20 4164 7343 616d 7061 6967 6e53  gn, AdsCampaignS
-0001d7d0: 7461 7475 732c 2041 6473 4361 6d70 6169  tatus, AdsCampai
-0001d7e0: 676e 5479 7065 2c20 4164 7343 6174 6567  gnType, AdsCateg
-0001d7f0: 6f72 792c 2041 6473 436c 6965 6e74 2c20  ory, AdsClient, 
-0001d800: 4164 7343 7265 6174 6541 6453 7461 7475  AdsCreateAdStatu
-0001d810: 732c 2041 6473 4372 6561 7465 4361 6d70  s, AdsCreateCamp
-0001d820: 6169 676e 5374 6174 7573 2c20 4164 7343  aignStatus, AdsC
-0001d830: 7269 7465 7269 612c 0a20 2020 2020 2020  riteria,.       
-0001d840: 2020 2041 6473 4372 6974 6572 6961 5365     AdsCriteriaSe
-0001d850: 782c 2041 6473 4465 6d6f 5374 6174 732c  x, AdsDemoStats,
-0001d860: 2041 6473 4465 6d6f 7374 6174 7346 6f72   AdsDemostatsFor
-0001d870: 6d61 742c 2041 6473 466c 6f6f 6453 7461  mat, AdsFloodSta
-0001d880: 7473 2c20 4164 734c 696e 6b53 7461 7475  ts, AdsLinkStatu
-0001d890: 732c 2041 6473 4c6f 6f6b 616c 696b 6552  s, AdsLookalikeR
-0001d8a0: 6571 7565 7374 2c20 4164 734c 6f6f 6b61  equest, AdsLooka
-0001d8b0: 6c69 6b65 5265 7175 6573 7453 6176 6541  likeRequestSaveA
-0001d8c0: 7564 6965 6e63 654c 6576 656c 2c0a 2020  udienceLevel,.  
-0001d8d0: 2020 2020 2020 2020 4164 734d 7573 6963          AdsMusic
-0001d8e0: 6961 6e2c 2041 6473 4f62 6a65 6374 5479  ian, AdsObjectTy
-0001d8f0: 7065 2c20 4164 7350 6172 6167 7261 7068  pe, AdsParagraph
-0001d900: 732c 2041 6473 5072 6f6d 6f74 6564 506f  s, AdsPromotedPo
-0001d910: 7374 5265 6163 682c 2041 6473 5265 6a65  stReach, AdsReje
-0001d920: 6374 5265 6173 6f6e 2c20 4164 7352 756c  ctReason, AdsRul
-0001d930: 6573 2c20 4164 7353 7461 7473 2c20 4164  es, AdsStats, Ad
-0001d940: 7353 7461 7473 4167 652c 2041 6473 5374  sStatsAge, AdsSt
-0001d950: 6174 7343 6974 6965 732c 0a20 2020 2020  atsCities,.     
-0001d960: 2020 2020 2041 6473 5374 6174 7346 6f72       AdsStatsFor
-0001d970: 6d61 742c 2041 6473 5374 6174 7353 6578  mat, AdsStatsSex
-0001d980: 2c20 4164 7353 7461 7473 5365 7841 6765  , AdsStatsSexAge
-0001d990: 2c20 4164 7353 7461 7473 5365 7856 616c  , AdsStatsSexVal
-0001d9a0: 7565 2c20 4164 7353 7461 7473 5669 6577  ue, AdsStatsView
-0001d9b0: 7354 696d 6573 2c20 4164 7354 6172 6753  sTimes, AdsTargS
-0001d9c0: 6574 7469 6e67 732c 2041 6473 5461 7267  ettings, AdsTarg
-0001d9d0: 5374 6174 732c 2041 6473 5461 7267 5375  Stats, AdsTargSu
-0001d9e0: 6767 6573 7469 6f6e 732c 0a20 2020 2020  ggestions,.     
-0001d9f0: 2020 2020 2041 6473 5461 7267 5375 6767       AdsTargSugg
-0001da00: 6573 7469 6f6e 7343 6974 6965 732c 2041  estionsCities, A
+0001a2f0: 0975 726c 3a4f 7074 696f 6e61 6c5b 7374  .url:Optional[st
+0001a300: 725d 203d 204e 6f6e 650a 0a0a 0a0a 636c  r] = None.....cl
+0001a310: 6173 7320 4163 636f 756e 7455 7365 7253  ass AccountUserS
+0001a320: 6574 7469 6e67 7328 5573 6572 7355 7365  ettings(UsersUse
+0001a330: 724d 696e 2c20 5573 6572 7355 7365 7253  rMin, UsersUserS
+0001a340: 6574 7469 6e67 7358 7472 293a 0a09 7068  ettingsXtr):..ph
+0001a350: 6f74 6f5f 3230 303a 4f70 7469 6f6e 616c  oto_200:Optional
+0001a360: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6973  [str] = None..is
+0001a370: 5f73 6572 7669 6365 5f61 6363 6f75 6e74  _service_account
+0001a380: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0001a390: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4164  = None..class Ad
+0001a3a0: 7354 6172 6753 6574 7469 6e67 7328 4164  sTargSettings(Ad
+0001a3b0: 7343 7269 7465 7269 6129 3a0a 0969 643a  sCriteria):..id:
+0001a3c0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0001a3d0: 4e6f 6e65 0a09 6361 6d70 6169 676e 5f69  None..campaign_i
+0001a3e0: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+0001a3f0: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4170  = None..class Ap
+0001a400: 7073 4170 7028 4170 7073 4170 704d 696e  psApp(AppsAppMin
+0001a410: 293a 0a09 6175 7468 6f72 5f75 726c 3a4f  ):..author_url:O
+0001a420: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001a430: 6f6e 650a 0962 616e 6e65 725f 3131 3230  one..banner_1120
+0001a440: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+0001a450: 204e 6f6e 650a 0962 616e 6e65 725f 3536   None..banner_56
+0001a460: 303a 4f70 7469 6f6e 616c 5b73 7472 5d20  0:Optional[str] 
+0001a470: 3d20 4e6f 6e65 0a09 6963 6f6e 5f31 363a  = None..icon_16:
+0001a480: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001a490: 4e6f 6e65 0a09 6973 5f6e 6577 3a4f 7074  None..is_new:Opt
+0001a4a0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+0001a4b0: 6e65 0a09 7075 7368 5f65 6e61 626c 6564  ne..push_enabled
+0001a4c0: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0001a4d0: 3d20 4e6f 6e65 0a09 7363 7265 656e 5f6f  = None..screen_o
+0001a4e0: 7269 656e 7461 7469 6f6e 3a4f 7074 696f  rientation:Optio
+0001a4f0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0001a500: 0966 7269 656e 6473 3a4f 7074 696f 6e61  .friends:Optiona
+0001a510: 6c5b 6c69 7374 5b69 6e74 5d5d 203d 204e  l[list[int]] = N
+0001a520: 6f6e 650a 0963 6174 616c 6f67 5f70 6f73  one..catalog_pos
+0001a530: 6974 696f 6e3a 4f70 7469 6f6e 616c 5b69  ition:Optional[i
+0001a540: 6e74 5d20 3d20 4e6f 6e65 0a09 6465 7363  nt] = None..desc
+0001a550: 7269 7074 696f 6e3a 4f70 7469 6f6e 616c  ription:Optional
+0001a560: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6765  [str] = None..ge
+0001a570: 6e72 653a 4f70 7469 6f6e 616c 5b73 7472  nre:Optional[str
+0001a580: 5d20 3d20 4e6f 6e65 0a09 6765 6e72 655f  ] = None..genre_
+0001a590: 6964 3a4f 7074 696f 6e61 6c5b 696e 745d  id:Optional[int]
+0001a5a0: 203d 204e 6f6e 650a 0969 6e74 6572 6e61   = None..interna
+0001a5b0: 7469 6f6e 616c 3a4f 7074 696f 6e61 6c5b  tional:Optional[
+0001a5c0: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6973  bool] = None..is
+0001a5d0: 5f69 6e5f 6361 7461 6c6f 673a 4f70 7469  _in_catalog:Opti
+0001a5e0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001a5f0: 0a09 6c65 6164 6572 626f 6172 645f 7479  ..leaderboard_ty
+0001a600: 7065 3a4f 7074 696f 6e61 6c5b 2241 7070  pe:Optional["App
+0001a610: 7341 7070 4c65 6164 6572 626f 6172 6454  sAppLeaderboardT
+0001a620: 7970 6522 5d20 3d20 4e6f 6e65 0a09 6d65  ype"] = None..me
+0001a630: 6d62 6572 735f 636f 756e 743a 4f70 7469  mbers_count:Opti
+0001a640: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001a650: 0a09 706c 6174 666f 726d 5f69 643a 4f70  ..platform_id:Op
+0001a660: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0001a670: 6e65 0a09 7075 626c 6973 6865 645f 6461  ne..published_da
+0001a680: 7465 3a4f 7074 696f 6e61 6c5b 696e 745d  te:Optional[int]
+0001a690: 203d 204e 6f6e 650a 0973 6372 6565 6e5f   = None..screen_
+0001a6a0: 6e61 6d65 3a4f 7074 696f 6e61 6c5b 7374  name:Optional[st
+0001a6b0: 725d 203d 204e 6f6e 650a 0973 6563 7469  r] = None..secti
+0001a6c0: 6f6e 3a4f 7074 696f 6e61 6c5b 7374 725d  on:Optional[str]
+0001a6d0: 203d 204e 6f6e 650a 0a63 6c61 7373 2043   = None..class C
+0001a6e0: 616c 6c62 6163 6b43 6f6e 6669 726d 6174  allbackConfirmat
+0001a6f0: 696f 6e28 4361 6c6c 6261 636b 4261 7365  ion(CallbackBase
+0001a700: 293a 0a09 7479 7065 3a4f 7074 696f 6e61  ):..type:Optiona
+0001a710: 6c5b 7374 725d 203d 204e 6f6e 650a 0a63  l[str] = None..c
+0001a720: 6c61 7373 2043 616c 6c62 6163 6b4d 6573  lass CallbackMes
+0001a730: 7361 6765 416c 6c6f 7728 4361 6c6c 6261  sageAllow(Callba
+0001a740: 636b 4261 7365 293a 0a09 7479 7065 3a4f  ckBase):..type:O
+0001a750: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001a760: 6f6e 650a 096f 626a 6563 743a 2243 616c  one..object:"Cal
+0001a770: 6c62 6163 6b4d 6573 7361 6765 416c 6c6f  lbackMessageAllo
+0001a780: 774f 626a 6563 7422 0a0a 636c 6173 7320  wObject"..class 
+0001a790: 4361 6c6c 6261 636b 4d65 7373 6167 6545  CallbackMessageE
+0001a7a0: 6469 7428 4361 6c6c 6261 636b 4261 7365  dit(CallbackBase
+0001a7b0: 293a 0a09 7479 7065 3a4f 7074 696f 6e61  ):..type:Optiona
+0001a7c0: 6c5b 7374 725d 203d 204e 6f6e 650a 096f  l[str] = None..o
+0001a7d0: 626a 6563 743a 224d 6573 7361 6765 734d  bject:"MessagesM
+0001a7e0: 6573 7361 6765 220a 0a63 6c61 7373 2043  essage"..class C
+0001a7f0: 616c 6c62 6163 6b4d 6573 7361 6765 4e65  allbackMessageNe
+0001a800: 7728 4361 6c6c 6261 636b 4261 7365 293a  w(CallbackBase):
+0001a810: 0a09 7479 7065 3a4f 7074 696f 6e61 6c5b  ..type:Optional[
+0001a820: 7374 725d 203d 204e 6f6e 650a 096f 626a  str] = None..obj
+0001a830: 6563 743a 6f62 6a65 6374 0a0a 636c 6173  ect:object..clas
+0001a840: 7320 4361 6c6c 6261 636b 4d65 7373 6167  s CallbackMessag
+0001a850: 6552 6570 6c79 2843 616c 6c62 6163 6b42  eReply(CallbackB
+0001a860: 6173 6529 3a0a 0974 7970 653a 4f70 7469  ase):..type:Opti
+0001a870: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001a880: 0a09 6f62 6a65 6374 3a22 4d65 7373 6167  ..object:"Messag
+0001a890: 6573 4d65 7373 6167 6522 0a0a 636c 6173  esMessage"..clas
+0001a8a0: 7320 4461 7461 6261 7365 4369 7479 2842  s DatabaseCity(B
+0001a8b0: 6173 654f 626a 6563 7429 3a0a 0961 7265  aseObject):..are
+0001a8c0: 613a 4f70 7469 6f6e 616c 5b73 7472 5d20  a:Optional[str] 
+0001a8d0: 3d20 4e6f 6e65 0a09 7265 6769 6f6e 3a4f  = None..region:O
+0001a8e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001a8f0: 6f6e 650a 0969 6d70 6f72 7461 6e74 3a4f  one..important:O
+0001a900: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0001a910: 4e6f 6e65 0a0a 636c 6173 7320 4672 6965  None..class Frie
+0001a920: 6e64 7346 7269 656e 6445 7874 656e 6465  ndsFriendExtende
+0001a930: 6453 7461 7475 7328 4672 6965 6e64 7346  dStatus(FriendsF
+0001a940: 7269 656e 6453 7461 7475 7329 3a0a 0969  riendStatus):..i
+0001a950: 735f 7265 7175 6573 745f 756e 7265 6164  s_request_unread
+0001a960: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0001a970: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4772  = None..class Gr
+0001a980: 6f75 7073 4772 6f75 7046 756c 6c28 4772  oupsGroupFull(Gr
+0001a990: 6f75 7073 4772 6f75 7029 3a0a 096d 6172  oupsGroup):..mar
+0001a9a0: 6b65 743a 4f70 7469 6f6e 616c 5b22 4772  ket:Optional["Gr
+0001a9b0: 6f75 7073 4d61 726b 6574 496e 666f 225d  oupsMarketInfo"]
+0001a9c0: 203d 204e 6f6e 650a 096d 656d 6265 725f   = None..member_
+0001a9d0: 7374 6174 7573 3a4f 7074 696f 6e61 6c5b  status:Optional[
+0001a9e0: 2247 726f 7570 7347 726f 7570 4675 6c6c  "GroupsGroupFull
+0001a9f0: 4d65 6d62 6572 5374 6174 7573 225d 203d  MemberStatus"] =
+0001aa00: 204e 6f6e 650a 0969 735f 6164 756c 743a   None..is_adult:
+0001aa10: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0001aa20: 204e 6f6e 650a 0969 735f 6869 6464 656e   None..is_hidden
+0001aa30: 5f66 726f 6d5f 6665 6564 3a4f 7074 696f  _from_feed:Optio
+0001aa40: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001aa50: 0a09 6973 5f66 6176 6f72 6974 653a 4f70  ..is_favorite:Op
+0001aa60: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001aa70: 6f6e 650a 0969 735f 7375 6273 6372 6962  one..is_subscrib
+0001aa80: 6564 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ed:Optional[bool
+0001aa90: 5d20 3d20 4e6f 6e65 0a09 6369 7479 3a4f  ] = None..city:O
+0001aaa0: 7074 696f 6e61 6c5b 2242 6173 654f 626a  ptional["BaseObj
+0001aab0: 6563 7422 5d20 3d20 4e6f 6e65 0a09 636f  ect"] = None..co
+0001aac0: 756e 7472 793a 4f70 7469 6f6e 616c 5b22  untry:Optional["
+0001aad0: 4261 7365 436f 756e 7472 7922 5d20 3d20  BaseCountry"] = 
+0001aae0: 4e6f 6e65 0a09 7665 7269 6669 6564 3a4f  None..verified:O
+0001aaf0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0001ab00: 4e6f 6e65 0a09 6465 7363 7269 7074 696f  None..descriptio
+0001ab10: 6e3a 4f70 7469 6f6e 616c 5b73 7472 5d20  n:Optional[str] 
+0001ab20: 3d20 4e6f 6e65 0a09 7769 6b69 5f70 6167  = None..wiki_pag
+0001ab30: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
+0001ab40: 3d20 4e6f 6e65 0a09 6d65 6d62 6572 735f  = None..members_
+0001ab50: 636f 756e 743a 4f70 7469 6f6e 616c 5b69  count:Optional[i
+0001ab60: 6e74 5d20 3d20 4e6f 6e65 0a09 6d65 6d62  nt] = None..memb
+0001ab70: 6572 735f 636f 756e 745f 7465 7874 3a4f  ers_count_text:O
+0001ab80: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001ab90: 6f6e 650a 0972 6571 7565 7374 735f 636f  one..requests_co
+0001aba0: 756e 743a 4f70 7469 6f6e 616c 5b69 6e74  unt:Optional[int
+0001abb0: 5d20 3d20 4e6f 6e65 0a09 7669 6465 6f5f  ] = None..video_
+0001abc0: 6c69 7665 5f6c 6576 656c 3a4f 7074 696f  live_level:Optio
+0001abd0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0001abe0: 0976 6964 656f 5f6c 6976 655f 636f 756e  .video_live_coun
+0001abf0: 743a 4f70 7469 6f6e 616c 5b69 6e74 5d20  t:Optional[int] 
+0001ac00: 3d20 4e6f 6e65 0a09 636c 6970 735f 636f  = None..clips_co
+0001ac10: 756e 743a 4f70 7469 6f6e 616c 5b69 6e74  unt:Optional[int
+0001ac20: 5d20 3d20 4e6f 6e65 0a09 636f 756e 7465  ] = None..counte
+0001ac30: 7273 3a4f 7074 696f 6e61 6c5b 2247 726f  rs:Optional["Gro
+0001ac40: 7570 7343 6f75 6e74 6572 7347 726f 7570  upsCountersGroup
+0001ac50: 225d 203d 204e 6f6e 650a 0963 6f76 6572  "] = None..cover
+0001ac60: 3a4f 7074 696f 6e61 6c5b 2247 726f 7570  :Optional["Group
+0001ac70: 7343 6f76 6572 225d 203d 204e 6f6e 650a  sCover"] = None.
+0001ac80: 0963 616e 5f70 6f73 743a 4f70 7469 6f6e  .can_post:Option
+0001ac90: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+0001aca0: 0963 616e 5f73 7567 6765 7374 3a4f 7074  .can_suggest:Opt
+0001acb0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+0001acc0: 6e65 0a09 6361 6e5f 7570 6c6f 6164 5f73  ne..can_upload_s
+0001acd0: 746f 7279 3a4f 7074 696f 6e61 6c5b 626f  tory:Optional[bo
+0001ace0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  ol] = None..can_
+0001acf0: 7570 6c6f 6164 5f64 6f63 3a4f 7074 696f  upload_doc:Optio
+0001ad00: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001ad10: 0a09 6361 6e5f 7570 6c6f 6164 5f76 6964  ..can_upload_vid
+0001ad20: 656f 3a4f 7074 696f 6e61 6c5b 626f 6f6c  eo:Optional[bool
+0001ad30: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 7365  ] = None..can_se
+0001ad40: 655f 616c 6c5f 706f 7374 733a 4f70 7469  e_all_posts:Opti
+0001ad50: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+0001ad60: 650a 0963 616e 5f63 7265 6174 655f 746f  e..can_create_to
+0001ad70: 7069 633a 4f70 7469 6f6e 616c 5b62 6f6f  pic:Optional[boo
+0001ad80: 6c5d 203d 204e 6f6e 650a 0961 6374 6976  l] = None..activ
+0001ad90: 6974 793a 4f70 7469 6f6e 616c 5b73 7472  ity:Optional[str
+0001ada0: 5d20 3d20 4e6f 6e65 0a09 6669 7865 645f  ] = None..fixed_
+0001adb0: 706f 7374 3a4f 7074 696f 6e61 6c5b 696e  post:Optional[in
+0001adc0: 745d 203d 204e 6f6e 650a 0968 6173 5f70  t] = None..has_p
+0001add0: 686f 746f 3a4f 7074 696f 6e61 6c5b 626f  hoto:Optional[bo
+0001ade0: 6f6c 5d20 3d20 4e6f 6e65 0a09 6372 6f70  ol] = None..crop
+0001adf0: 5f70 686f 746f 3a4f 7074 696f 6e61 6c5b  _photo:Optional[
+0001ae00: 2242 6173 6543 726f 7050 686f 746f 225d  "BaseCropPhoto"]
+0001ae10: 203d 204e 6f6e 650a 0973 7461 7475 733a   = None..status:
+0001ae20: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001ae30: 4e6f 6e65 0a09 7374 6174 7573 5f61 7564  None..status_aud
+0001ae40: 696f 3a4f 7074 696f 6e61 6c5b 2241 7564  io:Optional["Aud
+0001ae50: 696f 4175 6469 6f22 5d20 3d20 4e6f 6e65  ioAudio"] = None
+0001ae60: 0a09 6d61 696e 5f61 6c62 756d 5f69 643a  ..main_album_id:
+0001ae70: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0001ae80: 4e6f 6e65 0a09 6c69 6e6b 733a 4f70 7469  None..links:Opti
+0001ae90: 6f6e 616c 5b6c 6973 745b 2247 726f 7570  onal[list["Group
+0001aea0: 734c 696e 6b73 4974 656d 225d 5d20 3d20  sLinksItem"]] = 
+0001aeb0: 4e6f 6e65 0a09 636f 6e74 6163 7473 3a4f  None..contacts:O
+0001aec0: 7074 696f 6e61 6c5b 6c69 7374 5b22 4772  ptional[list["Gr
+0001aed0: 6f75 7073 436f 6e74 6163 7473 4974 656d  oupsContactsItem
+0001aee0: 225d 5d20 3d20 4e6f 6e65 0a09 7761 6c6c  "]] = None..wall
+0001aef0: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+0001af00: 204e 6f6e 650a 0973 6974 653a 4f70 7469   None..site:Opti
+0001af10: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001af20: 0a09 6d61 696e 5f73 6563 7469 6f6e 3a4f  ..main_section:O
+0001af30: 7074 696f 6e61 6c5b 2247 726f 7570 7347  ptional["GroupsG
+0001af40: 726f 7570 4675 6c6c 5365 6374 696f 6e22  roupFullSection"
+0001af50: 5d20 3d20 4e6f 6e65 0a09 7365 636f 6e64  ] = None..second
+0001af60: 6172 795f 7365 6374 696f 6e3a 4f70 7469  ary_section:Opti
+0001af70: 6f6e 616c 5b22 4772 6f75 7073 4772 6f75  onal["GroupsGrou
+0001af80: 7046 756c 6c53 6563 7469 6f6e 225d 203d  pFullSection"] =
+0001af90: 204e 6f6e 650a 0974 7265 6e64 696e 673a   None..trending:
+0001afa0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0001afb0: 204e 6f6e 650a 0963 616e 5f6d 6573 7361   None..can_messa
+0001afc0: 6765 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ge:Optional[bool
+0001afd0: 5d20 3d20 4e6f 6e65 0a09 6973 5f6d 6573  ] = None..is_mes
+0001afe0: 7361 6765 735f 626c 6f63 6b65 643a 4f70  sages_blocked:Op
+0001aff0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001b000: 6f6e 650a 0963 616e 5f73 656e 645f 6e6f  one..can_send_no
+0001b010: 7469 6679 3a4f 7074 696f 6e61 6c5b 626f  tify:Optional[bo
+0001b020: 6f6c 5d20 3d20 4e6f 6e65 0a09 6f6e 6c69  ol] = None..onli
+0001b030: 6e65 5f73 7461 7475 733a 4f70 7469 6f6e  ne_status:Option
+0001b040: 616c 5b22 4772 6f75 7073 4f6e 6c69 6e65  al["GroupsOnline
+0001b050: 5374 6174 7573 225d 203d 204e 6f6e 650a  Status"] = None.
+0001b060: 0969 6e76 6974 6564 5f62 793a 4f70 7469  .invited_by:Opti
+0001b070: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001b080: 0a09 6167 655f 6c69 6d69 7473 3a4f 7074  ..age_limits:Opt
+0001b090: 696f 6e61 6c5b 2247 726f 7570 7347 726f  ional["GroupsGro
+0001b0a0: 7570 4675 6c6c 4167 654c 696d 6974 7322  upFullAgeLimits"
+0001b0b0: 5d20 3d20 4e6f 6e65 0a09 6261 6e5f 696e  ] = None..ban_in
+0001b0c0: 666f 3a4f 7074 696f 6e61 6c5b 2247 726f  fo:Optional["Gro
+0001b0d0: 7570 7347 726f 7570 4261 6e49 6e66 6f22  upsGroupBanInfo"
+0001b0e0: 5d20 3d20 4e6f 6e65 0a09 6861 735f 6d61  ] = None..has_ma
+0001b0f0: 726b 6574 5f61 7070 3a4f 7074 696f 6e61  rket_app:Optiona
+0001b100: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
+0001b110: 7573 696e 675f 766b 7061 795f 6d61 726b  using_vkpay_mark
+0001b120: 6574 5f61 7070 3a4f 7074 696f 6e61 6c5b  et_app:Optional[
+0001b130: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6861  bool] = None..ha
+0001b140: 735f 6772 6f75 705f 6368 616e 6e65 6c3a  s_group_channel:
+0001b150: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0001b160: 204e 6f6e 650a 0961 6464 7265 7373 6573   None..addresses
+0001b170: 3a4f 7074 696f 6e61 6c5b 2247 726f 7570  :Optional["Group
+0001b180: 7341 6464 7265 7373 6573 496e 666f 225d  sAddressesInfo"]
+0001b190: 203d 204e 6f6e 650a 0969 735f 7375 6273   = None..is_subs
+0001b1a0: 6372 6962 6564 5f70 6f64 6361 7374 733a  cribed_podcasts:
+0001b1b0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0001b1c0: 204e 6f6e 650a 0963 616e 5f73 7562 7363   None..can_subsc
+0001b1d0: 7269 6265 5f70 6f64 6361 7374 733a 4f70  ribe_podcasts:Op
+0001b1e0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001b1f0: 6f6e 650a 0963 616e 5f73 7562 7363 7269  one..can_subscri
+0001b200: 6265 5f70 6f73 7473 3a4f 7074 696f 6e61  be_posts:Optiona
+0001b210: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
+0001b220: 6c69 7665 5f63 6f76 6572 733a 4f70 7469  live_covers:Opti
+0001b230: 6f6e 616c 5b22 4772 6f75 7073 4c69 7665  onal["GroupsLive
+0001b240: 436f 7665 7273 225d 203d 204e 6f6e 650a  Covers"] = None.
+0001b250: 0973 746f 7269 6573 5f61 7263 6869 7665  .stories_archive
+0001b260: 5f63 6f75 6e74 3a4f 7074 696f 6e61 6c5b  _count:Optional[
+0001b270: 696e 745d 203d 204e 6f6e 650a 0968 6173  int] = None..has
+0001b280: 5f75 6e73 6565 6e5f 7374 6f72 6965 733a  _unseen_stories:
+0001b290: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0001b2a0: 204e 6f6e 650a 0a63 6c61 7373 204d 6172   None..class Mar
+0001b2b0: 6b65 744d 6172 6b65 7449 7465 6d46 756c  ketMarketItemFul
+0001b2c0: 6c28 4d61 726b 6574 4d61 726b 6574 4974  l(MarketMarketIt
+0001b2d0: 656d 293a 0a09 616c 6275 6d73 5f69 6473  em):..albums_ids
+0001b2e0: 3a4f 7074 696f 6e61 6c5b 6c69 7374 5b69  :Optional[list[i
+0001b2f0: 6e74 5d5d 203d 204e 6f6e 650a 0970 686f  nt]] = None..pho
+0001b300: 746f 733a 4f70 7469 6f6e 616c 5b6c 6973  tos:Optional[lis
+0001b310: 745b 2250 686f 746f 7350 686f 746f 225d  t["PhotosPhoto"]
+0001b320: 5d20 3d20 4e6f 6e65 0a09 6361 6e5f 636f  ] = None..can_co
+0001b330: 6d6d 656e 743a 4f70 7469 6f6e 616c 5b62  mment:Optional[b
+0001b340: 6f6f 6c5d 203d 204e 6f6e 650a 0963 616e  ool] = None..can
+0001b350: 5f72 6570 6f73 743a 4f70 7469 6f6e 616c  _repost:Optional
+0001b360: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 096c  [bool] = None..l
+0001b370: 696b 6573 3a4f 7074 696f 6e61 6c5b 2242  ikes:Optional["B
+0001b380: 6173 654c 696b 6573 225d 203d 204e 6f6e  aseLikes"] = Non
+0001b390: 650a 0972 6570 6f73 7473 3a4f 7074 696f  e..reposts:Optio
+0001b3a0: 6e61 6c5b 2242 6173 6552 6570 6f73 7473  nal["BaseReposts
+0001b3b0: 496e 666f 225d 203d 204e 6f6e 650a 0976  Info"] = None..v
+0001b3c0: 6965 7773 5f63 6f75 6e74 3a4f 7074 696f  iews_count:Optio
+0001b3d0: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0001b3e0: 0977 6973 686c 6973 745f 6974 656d 5f69  .wishlist_item_i
+0001b3f0: 643a 4f70 7469 6f6e 616c 5b69 6e74 5d20  d:Optional[int] 
+0001b400: 3d20 4e6f 6e65 0a09 6361 6e63 656c 5f69  = None..cancel_i
+0001b410: 6e66 6f3a 4f70 7469 6f6e 616c 5b22 4261  nfo:Optional["Ba
+0001b420: 7365 4c69 6e6b 225d 203d 204e 6f6e 650a  seLink"] = None.
+0001b430: 0975 7365 725f 6167 7265 656d 656e 745f  .user_agreement_
+0001b440: 696e 666f 3a4f 7074 696f 6e61 6c5b 7374  info:Optional[st
+0001b450: 725d 203d 204e 6f6e 650a 0961 645f 6964  r] = None..ad_id
+0001b460: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+0001b470: 204e 6f6e 650a 0a63 6c61 7373 204d 6573   None..class Mes
+0001b480: 7361 6765 7347 6574 436f 6e76 6572 7361  sagesGetConversa
+0001b490: 7469 6f6e 4279 4964 4578 7465 6e64 6564  tionByIdExtended
+0001b4a0: 284d 6573 7361 6765 7347 6574 436f 6e76  (MessagesGetConv
+0001b4b0: 6572 7361 7469 6f6e 4279 4964 293a 0a09  ersationById):..
+0001b4c0: 7072 6f66 696c 6573 3a4f 7074 696f 6e61  profiles:Optiona
+0001b4d0: 6c5b 6c69 7374 5b22 5573 6572 7355 7365  l[list["UsersUse
+0001b4e0: 7246 756c 6c22 5d5d 203d 204e 6f6e 650a  rFull"]] = None.
+0001b4f0: 0967 726f 7570 733a 4f70 7469 6f6e 616c  .groups:Optional
+0001b500: 5b6c 6973 745b 2247 726f 7570 7347 726f  [list["GroupsGro
+0001b510: 7570 4675 6c6c 225d 5d20 3d20 4e6f 6e65  upFull"]] = None
+0001b520: 0a0a 636c 6173 7320 4e65 7773 6665 6564  ..class Newsfeed
+0001b530: 4974 656d 4175 6469 6f28 4e65 7773 6665  ItemAudio(Newsfe
+0001b540: 6564 4974 656d 4261 7365 293a 0a09 6175  edItemBase):..au
+0001b550: 6469 6f3a 4f70 7469 6f6e 616c 5b22 4e65  dio:Optional["Ne
+0001b560: 7773 6665 6564 4974 656d 4175 6469 6f41  wsfeedItemAudioA
+0001b570: 7564 696f 225d 203d 204e 6f6e 650a 0970  udio"] = None..p
+0001b580: 6f73 745f 6964 3a4f 7074 696f 6e61 6c5b  ost_id:Optional[
+0001b590: 696e 745d 203d 204e 6f6e 650a 0a63 6c61  int] = None..cla
+0001b5a0: 7373 204e 6577 7366 6565 6449 7465 6d44  ss NewsfeedItemD
+0001b5b0: 6967 6573 7428 4e65 7773 6665 6564 4974  igest(NewsfeedIt
+0001b5c0: 656d 4261 7365 293a 0a09 6665 6564 5f69  emBase):..feed_i
+0001b5d0: 643a 4f70 7469 6f6e 616c 5b73 7472 5d20  d:Optional[str] 
+0001b5e0: 3d20 4e6f 6e65 0a09 6974 656d 733a 4f70  = None..items:Op
+0001b5f0: 7469 6f6e 616c 5b6c 6973 745b 224e 6577  tional[list["New
+0001b600: 7366 6565 6449 7465 6d44 6967 6573 7449  sfeedItemDigestI
+0001b610: 7465 6d22 5d5d 203d 204e 6f6e 650a 096d  tem"]] = None..m
+0001b620: 6169 6e5f 706f 7374 5f69 6473 3a4f 7074  ain_post_ids:Opt
+0001b630: 696f 6e61 6c5b 6c69 7374 5b73 7472 5d5d  ional[list[str]]
+0001b640: 203d 204e 6f6e 650a 0974 656d 706c 6174   = None..templat
+0001b650: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
+0001b660: 3d20 4e6f 6e65 0a09 6865 6164 6572 3a4f  = None..header:O
+0001b670: 7074 696f 6e61 6c5b 224e 6577 7366 6565  ptional["Newsfee
+0001b680: 6449 7465 6d44 6967 6573 7448 6561 6465  dItemDigestHeade
+0001b690: 7222 5d20 3d20 4e6f 6e65 0a09 666f 6f74  r"] = None..foot
+0001b6a0: 6572 3a4f 7074 696f 6e61 6c5b 224e 6577  er:Optional["New
+0001b6b0: 7366 6565 6449 7465 6d44 6967 6573 7446  sfeedItemDigestF
+0001b6c0: 6f6f 7465 7222 5d20 3d20 4e6f 6e65 0a09  ooter"] = None..
+0001b6d0: 7472 6163 6b5f 636f 6465 3a4f 7074 696f  track_code:Optio
+0001b6e0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+0001b6f0: 0a63 6c61 7373 204e 6577 7366 6565 6449  .class NewsfeedI
+0001b700: 7465 6d46 7269 656e 6428 4e65 7773 6665  temFriend(Newsfe
+0001b710: 6564 4974 656d 4261 7365 293a 0a09 6672  edItemBase):..fr
+0001b720: 6965 6e64 733a 4f70 7469 6f6e 616c 5b22  iends:Optional["
+0001b730: 4e65 7773 6665 6564 4974 656d 4672 6965  NewsfeedItemFrie
+0001b740: 6e64 4672 6965 6e64 7322 5d20 3d20 4e6f  ndFriends"] = No
+0001b750: 6e65 0a0a 636c 6173 7320 4e65 7773 6665  ne..class Newsfe
+0001b760: 6564 4974 656d 5068 6f74 6f28 5761 6c6c  edItemPhoto(Wall
+0001b770: 4361 726f 7573 656c 4261 7365 2c20 4e65  CarouselBase, Ne
+0001b780: 7773 6665 6564 4974 656d 4261 7365 293a  wsfeedItemBase):
+0001b790: 0a09 7068 6f74 6f73 3a4f 7074 696f 6e61  ..photos:Optiona
+0001b7a0: 6c5b 224e 6577 7366 6565 6449 7465 6d50  l["NewsfeedItemP
+0001b7b0: 686f 746f 5068 6f74 6f73 225d 203d 204e  hotoPhotos"] = N
+0001b7c0: 6f6e 650a 0970 6f73 745f 6964 3a4f 7074  one..post_id:Opt
+0001b7d0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0001b7e0: 650a 0a63 6c61 7373 204e 6577 7366 6565  e..class Newsfee
+0001b7f0: 6449 7465 6d50 686f 746f 5461 6728 5761  dItemPhotoTag(Wa
+0001b800: 6c6c 4361 726f 7573 656c 4261 7365 2c20  llCarouselBase, 
+0001b810: 4e65 7773 6665 6564 4974 656d 4261 7365  NewsfeedItemBase
+0001b820: 293a 0a09 7068 6f74 6f5f 7461 6773 3a4f  ):..photo_tags:O
+0001b830: 7074 696f 6e61 6c5b 224e 6577 7366 6565  ptional["Newsfee
+0001b840: 6449 7465 6d50 686f 746f 5461 6750 686f  dItemPhotoTagPho
+0001b850: 746f 5461 6773 225d 203d 204e 6f6e 650a  toTags"] = None.
+0001b860: 0970 6f73 745f 6964 3a4f 7074 696f 6e61  .post_id:Optiona
+0001b870: 6c5b 696e 745d 203d 204e 6f6e 650a 0a63  l[int] = None..c
+0001b880: 6c61 7373 204e 6577 7366 6565 6449 7465  lass NewsfeedIte
+0001b890: 6d50 726f 6d6f 4275 7474 6f6e 284e 6577  mPromoButton(New
+0001b8a0: 7366 6565 6449 7465 6d42 6173 6529 3a0a  sfeedItemBase):.
+0001b8b0: 0974 6578 743a 4f70 7469 6f6e 616c 5b73  .text:Optional[s
+0001b8c0: 7472 5d20 3d20 4e6f 6e65 0a09 7469 746c  tr] = None..titl
+0001b8d0: 653a 4f70 7469 6f6e 616c 5b73 7472 5d20  e:Optional[str] 
+0001b8e0: 3d20 4e6f 6e65 0a09 6163 7469 6f6e 3a4f  = None..action:O
+0001b8f0: 7074 696f 6e61 6c5b 224e 6577 7366 6565  ptional["Newsfee
+0001b900: 6449 7465 6d50 726f 6d6f 4275 7474 6f6e  dItemPromoButton
+0001b910: 4163 7469 6f6e 225d 203d 204e 6f6e 650a  Action"] = None.
+0001b920: 0969 6d61 6765 733a 4f70 7469 6f6e 616c  .images:Optional
+0001b930: 5b6c 6973 745b 224e 6577 7366 6565 6449  [list["NewsfeedI
+0001b940: 7465 6d50 726f 6d6f 4275 7474 6f6e 496d  temPromoButtonIm
+0001b950: 6167 6522 5d5d 203d 204e 6f6e 650a 0974  age"]] = None..t
+0001b960: 7261 636b 5f63 6f64 653a 4f70 7469 6f6e  rack_code:Option
+0001b970: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a0a  al[str] = None..
+0001b980: 636c 6173 7320 4e65 7773 6665 6564 4974  class NewsfeedIt
+0001b990: 656d 546f 7069 6328 4e65 7773 6665 6564  emTopic(Newsfeed
+0001b9a0: 4974 656d 4261 7365 293a 0a09 636f 6d6d  ItemBase):..comm
+0001b9b0: 656e 7473 3a4f 7074 696f 6e61 6c5b 2242  ents:Optional["B
+0001b9c0: 6173 6543 6f6d 6d65 6e74 7349 6e66 6f22  aseCommentsInfo"
+0001b9d0: 5d20 3d20 4e6f 6e65 0a09 6c69 6b65 733a  ] = None..likes:
+0001b9e0: 4f70 7469 6f6e 616c 5b22 4261 7365 4c69  Optional["BaseLi
+0001b9f0: 6b65 7349 6e66 6f22 5d20 3d20 4e6f 6e65  kesInfo"] = None
+0001ba00: 0a09 706f 7374 5f69 643a 696e 740a 0974  ..post_id:int..t
+0001ba10: 6578 743a 7374 720a 0a63 6c61 7373 204e  ext:str..class N
+0001ba20: 6577 7366 6565 6449 7465 6d56 6964 656f  ewsfeedItemVideo
+0001ba30: 2857 616c 6c43 6172 6f75 7365 6c42 6173  (WallCarouselBas
+0001ba40: 652c 204e 6577 7366 6565 6449 7465 6d42  e, NewsfeedItemB
+0001ba50: 6173 6529 3a0a 0976 6964 656f 3a4f 7074  ase):..video:Opt
+0001ba60: 696f 6e61 6c5b 224e 6577 7366 6565 6449  ional["NewsfeedI
+0001ba70: 7465 6d56 6964 656f 5669 6465 6f22 5d20  temVideoVideo"] 
+0001ba80: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4e65  = None..class Ne
+0001ba90: 7773 6665 6564 4c69 7374 4675 6c6c 284e  wsfeedListFull(N
+0001baa0: 6577 7366 6565 644c 6973 7429 3a0a 096e  ewsfeedList):..n
+0001bab0: 6f5f 7265 706f 7374 733a 4f70 7469 6f6e  o_reposts:Option
+0001bac0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+0001bad0: 0973 6f75 7263 655f 6964 733a 4f70 7469  .source_ids:Opti
+0001bae0: 6f6e 616c 5b6c 6973 745b 696e 745d 5d20  onal[list[int]] 
+0001baf0: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4e65  = None..class Ne
+0001bb00: 7773 6665 6564 4e65 7773 6665 6564 5068  wsfeedNewsfeedPh
+0001bb10: 6f74 6f28 5068 6f74 6f73 5068 6f74 6f29  oto(PhotosPhoto)
+0001bb20: 3a0a 096c 696b 6573 3a4f 7074 696f 6e61  :..likes:Optiona
+0001bb30: 6c5b 2242 6173 654c 696b 6573 225d 203d  l["BaseLikes"] =
+0001bb40: 204e 6f6e 650a 0963 6f6d 6d65 6e74 733a   None..comments:
+0001bb50: 4f70 7469 6f6e 616c 5b22 4261 7365 4f62  Optional["BaseOb
+0001bb60: 6a65 6374 436f 756e 7422 5d20 3d20 4e6f  jectCount"] = No
+0001bb70: 6e65 0a09 6361 6e5f 7265 706f 7374 3a4f  ne..can_repost:O
+0001bb80: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0001bb90: 4e6f 6e65 0a0a 636c 6173 7320 4e6f 7469  None..class Noti
+0001bba0: 6669 6361 7469 6f6e 734e 6f74 6966 6963  ficationsNotific
+0001bbb0: 6174 696f 6e50 6172 656e 7428 5761 6c6c  ationParent(Wall
+0001bbc0: 5761 6c6c 706f 7374 546f 4964 2c20 5068  WallpostToId, Ph
+0001bbd0: 6f74 6f73 5068 6f74 6f2c 2042 6f61 7264  otosPhoto, Board
+0001bbe0: 546f 7069 632c 2056 6964 656f 5669 6465  Topic, VideoVide
+0001bbf0: 6f2c 204e 6f74 6966 6963 6174 696f 6e73  o, Notifications
+0001bc00: 4e6f 7469 6669 6361 7469 6f6e 7343 6f6d  NotificationsCom
+0001bc10: 6d65 6e74 293a 0a09 7061 7373 0a63 6c61  ment):..pass.cla
+0001bc20: 7373 2055 7365 7273 5573 6572 2855 7365  ss UsersUser(Use
+0001bc30: 7273 5573 6572 4d69 6e29 3a0a 0973 6578  rsUserMin):..sex
+0001bc40: 3a4f 7074 696f 6e61 6c5b 2242 6173 6553  :Optional["BaseS
+0001bc50: 6578 225d 203d 204e 6f6e 650a 0973 6372  ex"] = None..scr
+0001bc60: 6565 6e5f 6e61 6d65 3a4f 7074 696f 6e61  een_name:Optiona
+0001bc70: 6c5b 7374 725d 203d 204e 6f6e 650a 0970  l[str] = None..p
+0001bc80: 686f 746f 5f35 303a 4f70 7469 6f6e 616c  hoto_50:Optional
+0001bc90: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7068  [str] = None..ph
+0001bca0: 6f74 6f5f 3130 303a 4f70 7469 6f6e 616c  oto_100:Optional
+0001bcb0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6f6e  [str] = None..on
+0001bcc0: 6c69 6e65 5f69 6e66 6f3a 4f70 7469 6f6e  line_info:Option
+0001bcd0: 616c 5b22 5573 6572 734f 6e6c 696e 6549  al["UsersOnlineI
+0001bce0: 6e66 6f22 5d20 3d20 4e6f 6e65 0a09 6f6e  nfo"] = None..on
+0001bcf0: 6c69 6e65 3a4f 7074 696f 6e61 6c5b 626f  line:Optional[bo
+0001bd00: 6f6c 5d20 3d20 4e6f 6e65 0a09 6f6e 6c69  ol] = None..onli
+0001bd10: 6e65 5f6d 6f62 696c 653a 4f70 7469 6f6e  ne_mobile:Option
+0001bd20: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+0001bd30: 096f 6e6c 696e 655f 6170 703a 4f70 7469  .online_app:Opti
+0001bd40: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001bd50: 0a09 7665 7269 6669 6564 3a4f 7074 696f  ..verified:Optio
+0001bd60: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001bd70: 0a09 7472 656e 6469 6e67 3a4f 7074 696f  ..trending:Optio
+0001bd80: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001bd90: 0a09 6672 6965 6e64 5f73 7461 7475 733a  ..friend_status:
+0001bda0: 4f70 7469 6f6e 616c 5b22 4672 6965 6e64  Optional["Friend
+0001bdb0: 7346 7269 656e 6453 7461 7475 7353 7461  sFriendStatusSta
+0001bdc0: 7475 7322 5d20 3d20 4e6f 6e65 0a09 6d75  tus"] = None..mu
+0001bdd0: 7475 616c 3a4f 7074 696f 6e61 6c5b 2246  tual:Optional["F
+0001bde0: 7269 656e 6473 5265 7175 6573 7473 4d75  riendsRequestsMu
+0001bdf0: 7475 616c 225d 203d 204e 6f6e 650a 0a63  tual"] = None..c
+0001be00: 6c61 7373 2055 7365 7273 5573 6572 4675  lass UsersUserFu
+0001be10: 6c6c 2855 7365 7273 5573 6572 293a 0a09  ll(UsersUser):..
+0001be20: 6669 7273 745f 6e61 6d65 5f6e 6f6d 3a4f  first_name_nom:O
+0001be30: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001be40: 6f6e 650a 0966 6972 7374 5f6e 616d 655f  one..first_name_
+0001be50: 6765 6e3a 4f70 7469 6f6e 616c 5b73 7472  gen:Optional[str
+0001be60: 5d20 3d20 4e6f 6e65 0a09 6669 7273 745f  ] = None..first_
+0001be70: 6e61 6d65 5f64 6174 3a4f 7074 696f 6e61  name_dat:Optiona
+0001be80: 6c5b 7374 725d 203d 204e 6f6e 650a 0966  l[str] = None..f
+0001be90: 6972 7374 5f6e 616d 655f 6163 633a 4f70  irst_name_acc:Op
+0001bea0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0001beb0: 6e65 0a09 6669 7273 745f 6e61 6d65 5f69  ne..first_name_i
+0001bec0: 6e73 3a4f 7074 696f 6e61 6c5b 7374 725d  ns:Optional[str]
+0001bed0: 203d 204e 6f6e 650a 0966 6972 7374 5f6e   = None..first_n
+0001bee0: 616d 655f 6162 6c3a 4f70 7469 6f6e 616c  ame_abl:Optional
+0001bef0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6c61  [str] = None..la
+0001bf00: 7374 5f6e 616d 655f 6e6f 6d3a 4f70 7469  st_name_nom:Opti
+0001bf10: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001bf20: 0a09 6c61 7374 5f6e 616d 655f 6765 6e3a  ..last_name_gen:
+0001bf30: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001bf40: 4e6f 6e65 0a09 6c61 7374 5f6e 616d 655f  None..last_name_
+0001bf50: 6461 743a 4f70 7469 6f6e 616c 5b73 7472  dat:Optional[str
+0001bf60: 5d20 3d20 4e6f 6e65 0a09 6c61 7374 5f6e  ] = None..last_n
+0001bf70: 616d 655f 6163 633a 4f70 7469 6f6e 616c  ame_acc:Optional
+0001bf80: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6c61  [str] = None..la
+0001bf90: 7374 5f6e 616d 655f 696e 733a 4f70 7469  st_name_ins:Opti
+0001bfa0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001bfb0: 0a09 6c61 7374 5f6e 616d 655f 6162 6c3a  ..last_name_abl:
+0001bfc0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001bfd0: 4e6f 6e65 0a09 6e69 636b 6e61 6d65 3a4f  None..nickname:O
+0001bfe0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001bff0: 6f6e 650a 096d 6169 6465 6e5f 6e61 6d65  one..maiden_name
+0001c000: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+0001c010: 204e 6f6e 650a 0963 6f6e 7461 6374 5f6e   None..contact_n
+0001c020: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
+0001c030: 5d20 3d20 4e6f 6e65 0a09 646f 6d61 696e  ] = None..domain
+0001c040: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+0001c050: 204e 6f6e 650a 0962 6461 7465 3a4f 7074   None..bdate:Opt
+0001c060: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0001c070: 650a 0963 6974 793a 4f70 7469 6f6e 616c  e..city:Optional
+0001c080: 5b22 4261 7365 4369 7479 225d 203d 204e  ["BaseCity"] = N
+0001c090: 6f6e 650a 0963 6f75 6e74 7279 3a4f 7074  one..country:Opt
+0001c0a0: 696f 6e61 6c5b 2242 6173 6543 6f75 6e74  ional["BaseCount
+0001c0b0: 7279 225d 203d 204e 6f6e 650a 0974 696d  ry"] = None..tim
+0001c0c0: 657a 6f6e 653a 4f70 7469 6f6e 616c 5b69  ezone:Optional[i
+0001c0d0: 6e74 5d20 3d20 4e6f 6e65 0a09 6f77 6e65  nt] = None..owne
+0001c0e0: 725f 7374 6174 653a 4f70 7469 6f6e 616c  r_state:Optional
+0001c0f0: 5b22 4f77 6e65 7253 7461 7465 225d 203d  ["OwnerState"] =
+0001c100: 204e 6f6e 650a 0970 686f 746f 5f32 3030   None..photo_200
+0001c110: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+0001c120: 204e 6f6e 650a 0970 686f 746f 5f6d 6178   None..photo_max
+0001c130: 3a4f 7074 696f 6e61 6c5b 7374 725d 203d  :Optional[str] =
+0001c140: 204e 6f6e 650a 0970 686f 746f 5f32 3030   None..photo_200
+0001c150: 5f6f 7269 673a 4f70 7469 6f6e 616c 5b73  _orig:Optional[s
+0001c160: 7472 5d20 3d20 4e6f 6e65 0a09 7068 6f74  tr] = None..phot
+0001c170: 6f5f 3430 305f 6f72 6967 3a4f 7074 696f  o_400_orig:Optio
+0001c180: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+0001c190: 0970 686f 746f 5f6d 6178 5f6f 7269 673a  .photo_max_orig:
+0001c1a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001c1b0: 4e6f 6e65 0a09 7068 6f74 6f5f 6964 3a4f  None..photo_id:O
+0001c1c0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001c1d0: 6f6e 650a 0968 6173 5f70 686f 746f 3a4f  one..has_photo:O
+0001c1e0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0001c1f0: 4e6f 6e65 0a09 6861 735f 6d6f 6269 6c65  None..has_mobile
+0001c200: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0001c210: 3d20 4e6f 6e65 0a09 6973 5f66 7269 656e  = None..is_frien
+0001c220: 643a 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  d:Optional[bool]
+0001c230: 203d 204e 6f6e 650a 0977 616c 6c5f 636f   = None..wall_co
+0001c240: 6d6d 656e 7473 3a4f 7074 696f 6e61 6c5b  mments:Optional[
+0001c250: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6361  bool] = None..ca
+0001c260: 6e5f 706f 7374 3a4f 7074 696f 6e61 6c5b  n_post:Optional[
+0001c270: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6361  bool] = None..ca
+0001c280: 6e5f 7365 655f 616c 6c5f 706f 7374 733a  n_see_all_posts:
+0001c290: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+0001c2a0: 204e 6f6e 650a 0963 616e 5f73 6565 5f61   None..can_see_a
+0001c2b0: 7564 696f 3a4f 7074 696f 6e61 6c5b 626f  udio:Optional[bo
+0001c2c0: 6f6c 5d20 3d20 4e6f 6e65 0a09 7479 7065  ol] = None..type
+0001c2d0: 3a4f 7074 696f 6e61 6c5b 2255 7365 7273  :Optional["Users
+0001c2e0: 5573 6572 5479 7065 225d 203d 204e 6f6e  UserType"] = Non
+0001c2f0: 650a 0965 6d61 696c 3a4f 7074 696f 6e61  e..email:Optiona
+0001c300: 6c5b 7374 725d 203d 204e 6f6e 650a 0973  l[str] = None..s
+0001c310: 6b79 7065 3a4f 7074 696f 6e61 6c5b 7374  kype:Optional[st
+0001c320: 725d 203d 204e 6f6e 650a 0966 6163 6562  r] = None..faceb
+0001c330: 6f6f 6b3a 4f70 7469 6f6e 616c 5b73 7472  ook:Optional[str
+0001c340: 5d20 3d20 4e6f 6e65 0a09 6661 6365 626f  ] = None..facebo
+0001c350: 6f6b 5f6e 616d 653a 4f70 7469 6f6e 616c  ok_name:Optional
+0001c360: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7477  [str] = None..tw
+0001c370: 6974 7465 723a 4f70 7469 6f6e 616c 5b73  itter:Optional[s
+0001c380: 7472 5d20 3d20 4e6f 6e65 0a09 6c69 7665  tr] = None..live
+0001c390: 6a6f 7572 6e61 6c3a 4f70 7469 6f6e 616c  journal:Optional
+0001c3a0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 696e  [str] = None..in
+0001c3b0: 7374 6167 7261 6d3a 4f70 7469 6f6e 616c  stagram:Optional
+0001c3c0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7465  [str] = None..te
+0001c3d0: 7374 3a4f 7074 696f 6e61 6c5b 626f 6f6c  st:Optional[bool
+0001c3e0: 5d20 3d20 4e6f 6e65 0a09 7669 6465 6f5f  ] = None..video_
+0001c3f0: 6c69 7665 3a4f 7074 696f 6e61 6c5b 2256  live:Optional["V
+0001c400: 6964 656f 4c69 7665 496e 666f 225d 203d  ideoLiveInfo"] =
+0001c410: 204e 6f6e 650a 0969 735f 7669 6465 6f5f   None..is_video_
+0001c420: 6c69 7665 5f6e 6f74 6966 6963 6174 696f  live_notificatio
+0001c430: 6e73 5f62 6c6f 636b 6564 3a4f 7074 696f  ns_blocked:Optio
+0001c440: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001c450: 0a09 6973 5f73 6572 7669 6365 3a4f 7074  ..is_service:Opt
+0001c460: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+0001c470: 6e65 0a09 7365 7276 6963 655f 6465 7363  ne..service_desc
+0001c480: 7269 7074 696f 6e3a 4f70 7469 6f6e 616c  ription:Optional
+0001c490: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7068  [str] = None..ph
+0001c4a0: 6f74 6f5f 7265 633a 4f70 7469 6f6e 616c  oto_rec:Optional
+0001c4b0: 5b22 5068 6f74 6f73 5068 6f74 6f46 616c  ["PhotosPhotoFal
+0001c4c0: 7365 6162 6c65 225d 203d 204e 6f6e 650a  seable"] = None.
+0001c4d0: 0970 686f 746f 5f6d 6564 6975 6d3a 4f70  .photo_medium:Op
+0001c4e0: 7469 6f6e 616c 5b22 5068 6f74 6f73 5068  tional["PhotosPh
+0001c4f0: 6f74 6f46 616c 7365 6162 6c65 225d 203d  otoFalseable"] =
+0001c500: 204e 6f6e 650a 0970 686f 746f 5f6d 6564   None..photo_med
+0001c510: 6975 6d5f 7265 633a 4f70 7469 6f6e 616c  ium_rec:Optional
+0001c520: 5b22 5068 6f74 6f73 5068 6f74 6f46 616c  ["PhotosPhotoFal
+0001c530: 7365 6162 6c65 225d 203d 204e 6f6e 650a  seable"] = None.
+0001c540: 0970 686f 746f 3a4f 7074 696f 6e61 6c5b  .photo:Optional[
+0001c550: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
+0001c560: 746f 5f62 6967 3a4f 7074 696f 6e61 6c5b  to_big:Optional[
+0001c570: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
+0001c580: 746f 5f34 3030 3a4f 7074 696f 6e61 6c5b  to_400:Optional[
+0001c590: 7374 725d 203d 204e 6f6e 650a 0970 686f  str] = None..pho
+0001c5a0: 746f 5f6d 6178 5f73 697a 653a 4f70 7469  to_max_size:Opti
+0001c5b0: 6f6e 616c 5b22 5068 6f74 6f73 5068 6f74  onal["PhotosPhot
+0001c5c0: 6f22 5d20 3d20 4e6f 6e65 0a09 6c61 6e67  o"] = None..lang
+0001c5d0: 7561 6765 3a4f 7074 696f 6e61 6c5b 7374  uage:Optional[st
+0001c5e0: 725d 203d 204e 6f6e 650a 0973 746f 7269  r] = None..stori
+0001c5f0: 6573 5f61 7263 6869 7665 5f63 6f75 6e74  es_archive_count
+0001c600: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+0001c610: 204e 6f6e 650a 0968 6173 5f75 6e73 6565   None..has_unsee
+0001c620: 6e5f 7374 6f72 6965 733a 4f70 7469 6f6e  n_stories:Option
+0001c630: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+0001c640: 0977 616c 6c5f 6465 6661 756c 743a 4f70  .wall_default:Op
+0001c650: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0001c660: 6e65 0a09 6361 6e5f 6361 6c6c 3a4f 7074  ne..can_call:Opt
+0001c670: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+0001c680: 6e65 0a09 6361 6e5f 6361 6c6c 5f66 726f  ne..can_call_fro
+0001c690: 6d5f 6772 6f75 703a 4f70 7469 6f6e 616c  m_group:Optional
+0001c6a0: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0963  [bool] = None..c
+0001c6b0: 616e 5f73 6565 5f77 6973 6865 733a 4f70  an_see_wishes:Op
+0001c6c0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001c6d0: 6f6e 650a 0963 616e 5f73 6565 5f67 6966  one..can_see_gif
+0001c6e0: 7473 3a4f 7074 696f 6e61 6c5b 626f 6f6c  ts:Optional[bool
+0001c6f0: 5d20 3d20 4e6f 6e65 0a09 696e 7465 7265  ] = None..intere
+0001c700: 7374 733a 4f70 7469 6f6e 616c 5b73 7472  sts:Optional[str
+0001c710: 5d20 3d20 4e6f 6e65 0a09 626f 6f6b 733a  ] = None..books:
+0001c720: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0001c730: 4e6f 6e65 0a09 7476 3a4f 7074 696f 6e61  None..tv:Optiona
+0001c740: 6c5b 7374 725d 203d 204e 6f6e 650a 0971  l[str] = None..q
+0001c750: 756f 7465 733a 4f70 7469 6f6e 616c 5b73  uotes:Optional[s
+0001c760: 7472 5d20 3d20 4e6f 6e65 0a09 6162 6f75  tr] = None..abou
+0001c770: 743a 4f70 7469 6f6e 616c 5b73 7472 5d20  t:Optional[str] 
+0001c780: 3d20 4e6f 6e65 0a09 6761 6d65 733a 4f70  = None..games:Op
+0001c790: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0001c7a0: 6e65 0a09 6d6f 7669 6573 3a4f 7074 696f  ne..movies:Optio
+0001c7b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+0001c7c0: 0961 6374 6976 6974 6965 733a 4f70 7469  .activities:Opti
+0001c7d0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001c7e0: 0a09 6d75 7369 633a 4f70 7469 6f6e 616c  ..music:Optional
+0001c7f0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 6361  [str] = None..ca
+0001c800: 6e5f 7772 6974 655f 7072 6976 6174 655f  n_write_private_
+0001c810: 6d65 7373 6167 653a 4f70 7469 6f6e 616c  message:Optional
+0001c820: 5b62 6f6f 6c5d 203d 204e 6f6e 650a 0963  [bool] = None..c
+0001c830: 616e 5f73 656e 645f 6672 6965 6e64 5f72  an_send_friend_r
+0001c840: 6571 7565 7374 3a4f 7074 696f 6e61 6c5b  equest:Optional[
+0001c850: 626f 6f6c 5d20 3d20 4e6f 6e65 0a09 6361  bool] = None..ca
+0001c860: 6e5f 6265 5f69 6e76 6974 6564 5f67 726f  n_be_invited_gro
+0001c870: 7570 3a4f 7074 696f 6e61 6c5b 626f 6f6c  up:Optional[bool
+0001c880: 5d20 3d20 4e6f 6e65 0a09 6d6f 6269 6c65  ] = None..mobile
+0001c890: 5f70 686f 6e65 3a4f 7074 696f 6e61 6c5b  _phone:Optional[
+0001c8a0: 7374 725d 203d 204e 6f6e 650a 0968 6f6d  str] = None..hom
+0001c8b0: 655f 7068 6f6e 653a 4f70 7469 6f6e 616c  e_phone:Optional
+0001c8c0: 5b73 7472 5d20 3d20 4e6f 6e65 0a09 7369  [str] = None..si
+0001c8d0: 7465 3a4f 7074 696f 6e61 6c5b 7374 725d  te:Optional[str]
+0001c8e0: 203d 204e 6f6e 650a 0973 7461 7475 735f   = None..status_
+0001c8f0: 6175 6469 6f3a 4f70 7469 6f6e 616c 5b22  audio:Optional["
+0001c900: 4175 6469 6f41 7564 696f 225d 203d 204e  AudioAudio"] = N
+0001c910: 6f6e 650a 0973 7461 7475 733a 4f70 7469  one..status:Opti
+0001c920: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001c930: 0a09 6163 7469 7669 7479 3a4f 7074 696f  ..activity:Optio
+0001c940: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
+0001c950: 096c 6173 745f 7365 656e 3a4f 7074 696f  .last_seen:Optio
+0001c960: 6e61 6c5b 2255 7365 7273 4c61 7374 5365  nal["UsersLastSe
+0001c970: 656e 225d 203d 204e 6f6e 650a 0965 7870  en"] = None..exp
+0001c980: 6f72 7473 3a4f 7074 696f 6e61 6c5b 2255  orts:Optional["U
+0001c990: 7365 7273 4578 706f 7274 7322 5d20 3d20  sersExports"] = 
+0001c9a0: 4e6f 6e65 0a09 6372 6f70 5f70 686f 746f  None..crop_photo
+0001c9b0: 3a4f 7074 696f 6e61 6c5b 2242 6173 6543  :Optional["BaseC
+0001c9c0: 726f 7050 686f 746f 225d 203d 204e 6f6e  ropPhoto"] = Non
+0001c9d0: 650a 0966 6f6c 6c6f 7765 7273 5f63 6f75  e..followers_cou
+0001c9e0: 6e74 3a4f 7074 696f 6e61 6c5b 696e 745d  nt:Optional[int]
+0001c9f0: 203d 204e 6f6e 650a 0976 6964 656f 5f6c   = None..video_l
+0001ca00: 6976 655f 6c65 7665 6c3a 4f70 7469 6f6e  ive_level:Option
+0001ca10: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 0a09  al[int] = None..
+0001ca20: 7669 6465 6f5f 6c69 7665 5f63 6f75 6e74  video_live_count
+0001ca30: 3a4f 7074 696f 6e61 6c5b 696e 745d 203d  :Optional[int] =
+0001ca40: 204e 6f6e 650a 0963 6c69 7073 5f63 6f75   None..clips_cou
+0001ca50: 6e74 3a4f 7074 696f 6e61 6c5b 696e 745d  nt:Optional[int]
+0001ca60: 203d 204e 6f6e 650a 0962 6c61 636b 6c69   = None..blackli
+0001ca70: 7374 6564 3a4f 7074 696f 6e61 6c5b 626f  sted:Optional[bo
+0001ca80: 6f6c 5d20 3d20 4e6f 6e65 0a09 626c 6163  ol] = None..blac
+0001ca90: 6b6c 6973 7465 645f 6279 5f6d 653a 4f70  klisted_by_me:Op
+0001caa0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001cab0: 6f6e 650a 0969 735f 6661 766f 7269 7465  one..is_favorite
+0001cac0: 3a4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  :Optional[bool] 
+0001cad0: 3d20 4e6f 6e65 0a09 6973 5f68 6964 6465  = None..is_hidde
+0001cae0: 6e5f 6672 6f6d 5f66 6565 643a 4f70 7469  n_from_feed:Opti
+0001caf0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+0001cb00: 650a 0963 6f6d 6d6f 6e5f 636f 756e 743a  e..common_count:
+0001cb10: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0001cb20: 4e6f 6e65 0a09 6f63 6375 7061 7469 6f6e  None..occupation
+0001cb30: 3a4f 7074 696f 6e61 6c5b 2255 7365 7273  :Optional["Users
+0001cb40: 4f63 6375 7061 7469 6f6e 225d 203d 204e  Occupation"] = N
+0001cb50: 6f6e 650a 0963 6172 6565 723a 4f70 7469  one..career:Opti
+0001cb60: 6f6e 616c 5b6c 6973 745b 2255 7365 7273  onal[list["Users
+0001cb70: 4361 7265 6572 225d 5d20 3d20 4e6f 6e65  Career"]] = None
+0001cb80: 0a09 6d69 6c69 7461 7279 3a4f 7074 696f  ..military:Optio
+0001cb90: 6e61 6c5b 6c69 7374 5b22 5573 6572 734d  nal[list["UsersM
+0001cba0: 696c 6974 6172 7922 5d5d 203d 204e 6f6e  ilitary"]] = Non
+0001cbb0: 650a 0975 6e69 7665 7273 6974 793a 4f70  e..university:Op
+0001cbc0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0001cbd0: 6e65 0a09 756e 6976 6572 7369 7479 5f6e  ne..university_n
+0001cbe0: 616d 653a 4f70 7469 6f6e 616c 5b73 7472  ame:Optional[str
+0001cbf0: 5d20 3d20 4e6f 6e65 0a09 756e 6976 6572  ] = None..univer
+0001cc00: 7369 7479 5f67 726f 7570 5f69 643a 4f70  sity_group_id:Op
+0001cc10: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0001cc20: 6e65 0a09 6661 6375 6c74 793a 4f70 7469  ne..faculty:Opti
+0001cc30: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001cc40: 0a09 6661 6375 6c74 795f 6e61 6d65 3a4f  ..faculty_name:O
+0001cc50: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0001cc60: 6f6e 650a 0967 7261 6475 6174 696f 6e3a  one..graduation:
+0001cc70: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0001cc80: 4e6f 6e65 0a09 6564 7563 6174 696f 6e5f  None..education_
+0001cc90: 666f 726d 3a4f 7074 696f 6e61 6c5b 7374  form:Optional[st
+0001cca0: 725d 203d 204e 6f6e 650a 0965 6475 6361  r] = None..educa
+0001ccb0: 7469 6f6e 5f73 7461 7475 733a 4f70 7469  tion_status:Opti
+0001ccc0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001ccd0: 0a09 686f 6d65 5f74 6f77 6e3a 4f70 7469  ..home_town:Opti
+0001cce0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0001ccf0: 0a09 7265 6c61 7469 6f6e 3a4f 7074 696f  ..relation:Optio
+0001cd00: 6e61 6c5b 2255 7365 7273 5573 6572 5265  nal["UsersUserRe
+0001cd10: 6c61 7469 6f6e 225d 203d 204e 6f6e 650a  lation"] = None.
+0001cd20: 0972 656c 6174 696f 6e5f 7061 7274 6e65  .relation_partne
+0001cd30: 723a 4f70 7469 6f6e 616c 5b22 5573 6572  r:Optional["User
+0001cd40: 7355 7365 724d 696e 225d 203d 204e 6f6e  sUserMin"] = Non
+0001cd50: 650a 0970 6572 736f 6e61 6c3a 4f70 7469  e..personal:Opti
+0001cd60: 6f6e 616c 5b22 5573 6572 7350 6572 736f  onal["UsersPerso
+0001cd70: 6e61 6c22 5d20 3d20 4e6f 6e65 0a09 756e  nal"] = None..un
+0001cd80: 6976 6572 7369 7469 6573 3a4f 7074 696f  iversities:Optio
+0001cd90: 6e61 6c5b 6c69 7374 5b22 5573 6572 7355  nal[list["UsersU
+0001cda0: 6e69 7665 7273 6974 7922 5d5d 203d 204e  niversity"]] = N
+0001cdb0: 6f6e 650a 0973 6368 6f6f 6c73 3a4f 7074  one..schools:Opt
+0001cdc0: 696f 6e61 6c5b 6c69 7374 5b22 5573 6572  ional[list["User
+0001cdd0: 7353 6368 6f6f 6c22 5d5d 203d 204e 6f6e  sSchool"]] = Non
+0001cde0: 650a 0972 656c 6174 6976 6573 3a4f 7074  e..relatives:Opt
+0001cdf0: 696f 6e61 6c5b 6c69 7374 5b22 5573 6572  ional[list["User
+0001ce00: 7352 656c 6174 6976 6522 5d5d 203d 204e  sRelative"]] = N
+0001ce10: 6f6e 650a 0969 735f 7375 6273 6372 6962  one..is_subscrib
+0001ce20: 6564 5f70 6f64 6361 7374 733a 4f70 7469  ed_podcasts:Opti
+0001ce30: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+0001ce40: 650a 0963 616e 5f73 7562 7363 7269 6265  e..can_subscribe
+0001ce50: 5f70 6f64 6361 7374 733a 4f70 7469 6f6e  _podcasts:Option
+0001ce60: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 650a  al[bool] = None.
+0001ce70: 0963 616e 5f73 7562 7363 7269 6265 5f70  .can_subscribe_p
+0001ce80: 6f73 7473 3a4f 7074 696f 6e61 6c5b 626f  osts:Optional[bo
+0001ce90: 6f6c 5d20 3d20 4e6f 6e65 0a09 636f 756e  ol] = None..coun
+0001cea0: 7465 7273 3a4f 7074 696f 6e61 6c5b 2255  ters:Optional["U
+0001ceb0: 7365 7273 5573 6572 436f 756e 7465 7273  sersUserCounters
+0001cec0: 225d 203d 204e 6f6e 650a 0961 6363 6573  "] = None..acces
+0001ced0: 735f 6b65 793a 4f70 7469 6f6e 616c 5b73  s_key:Optional[s
+0001cee0: 7472 5d20 3d20 4e6f 6e65 0a09 6361 6e5f  tr] = None..can_
+0001cef0: 7570 6c6f 6164 5f64 6f63 3a4f 7074 696f  upload_doc:Optio
+0001cf00: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001cf10: 0a09 6861 7368 3a4f 7074 696f 6e61 6c5b  ..hash:Optional[
+0001cf20: 7374 725d 203d 204e 6f6e 650a 0969 735f  str] = None..is_
+0001cf30: 6e6f 5f69 6e64 6578 3a4f 7074 696f 6e61  no_index:Optiona
+0001cf40: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a09  l[bool] = None..
+0001cf50: 636f 6e74 6163 745f 6964 3a4f 7074 696f  contact_id:Optio
+0001cf60: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0001cf70: 0969 735f 6d65 7373 6167 655f 7265 7175  .is_message_requ
+0001cf80: 6573 743a 4f70 7469 6f6e 616c 5b62 6f6f  est:Optional[boo
+0001cf90: 6c5d 203d 204e 6f6e 650a 0964 6573 6372  l] = None..descr
+0001cfa0: 6970 7469 6f6e 733a 4f70 7469 6f6e 616c  iptions:Optional
+0001cfb0: 5b6c 6973 745b 7374 725d 5d20 3d20 4e6f  [list[str]] = No
+0001cfc0: 6e65 0a09 6c69 7374 733a 4f70 7469 6f6e  ne..lists:Option
+0001cfd0: 616c 5b6c 6973 745b 696e 745d 5d20 3d20  al[list[int]] = 
+0001cfe0: 4e6f 6e65 0a0a 636c 6173 7320 5573 6572  None..class User
+0001cff0: 7355 7365 7258 7472 5479 7065 2855 7365  sUserXtrType(Use
+0001d000: 7273 5573 6572 293a 0a09 7479 7065 3a4f  rsUser):..type:O
+0001d010: 7074 696f 6e61 6c5b 2255 7365 7273 5573  ptional["UsersUs
+0001d020: 6572 5479 7065 225d 203d 204e 6f6e 650a  erType"] = None.
+0001d030: 0a63 6c61 7373 2056 6964 656f 5669 6465  .class VideoVide
+0001d040: 6f41 6c62 756d 4675 6c6c 2856 6964 656f  oAlbumFull(Video
+0001d050: 5669 6465 6f41 6c62 756d 293a 0a09 636f  VideoAlbum):..co
+0001d060: 756e 743a 696e 740a 0969 6d61 6765 3a4f  unt:int..image:O
+0001d070: 7074 696f 6e61 6c5b 6c69 7374 5b22 5669  ptional[list["Vi
+0001d080: 6465 6f56 6964 656f 496d 6167 6522 5d5d  deoVideoImage"]]
+0001d090: 203d 204e 6f6e 650a 0969 6d61 6765 5f62   = None..image_b
+0001d0a0: 6c75 723a 4f70 7469 6f6e 616c 5b22 4261  lur:Optional["Ba
+0001d0b0: 7365 5072 6f70 6572 7479 4578 6973 7473  sePropertyExists
+0001d0c0: 225d 203d 204e 6f6e 650a 0969 735f 7379  "] = None..is_sy
+0001d0d0: 7374 656d 3a4f 7074 696f 6e61 6c5b 2242  stem:Optional["B
+0001d0e0: 6173 6550 726f 7065 7274 7945 7869 7374  asePropertyExist
+0001d0f0: 7322 5d20 3d20 4e6f 6e65 0a09 7570 6461  s"] = None..upda
+0001d100: 7465 645f 7469 6d65 3a69 6e74 0a0a 636c  ted_time:int..cl
+0001d110: 6173 7320 5669 6465 6f56 6964 656f 4675  ass VideoVideoFu
+0001d120: 6c6c 2856 6964 656f 5669 6465 6f29 3a0a  ll(VideoVideo):.
+0001d130: 0966 696c 6573 3a4f 7074 696f 6e61 6c5b  .files:Optional[
+0001d140: 2256 6964 656f 5669 6465 6f46 696c 6573  "VideoVideoFiles
+0001d150: 225d 203d 204e 6f6e 650a 0974 7261 696c  "] = None..trail
+0001d160: 6572 3a4f 7074 696f 6e61 6c5b 2256 6964  er:Optional["Vid
+0001d170: 656f 5669 6465 6f46 696c 6573 225d 203d  eoVideoFiles"] =
+0001d180: 204e 6f6e 650a 096c 6976 655f 7365 7474   None..live_sett
+0001d190: 696e 6773 3a4f 7074 696f 6e61 6c5b 2256  ings:Optional["V
+0001d1a0: 6964 656f 4c69 7665 5365 7474 696e 6773  ideoLiveSettings
+0001d1b0: 225d 203d 204e 6f6e 650a 0a63 6c61 7373  "] = None..class
+0001d1c0: 2056 6964 656f 5669 6465 6f49 6d61 6765   VideoVideoImage
+0001d1d0: 2842 6173 6549 6d61 6765 293a 0a09 7769  (BaseImage):..wi
+0001d1e0: 7468 5f70 6164 6469 6e67 3a4f 7074 696f  th_padding:Optio
+0001d1f0: 6e61 6c5b 2242 6173 6550 726f 7065 7274  nal["BasePropert
+0001d200: 7945 7869 7374 7322 5d20 3d20 4e6f 6e65  yExists"] = None
+0001d210: 0a0a 636c 6173 7320 5761 6c6c 5761 6c6c  ..class WallWall
+0001d220: 706f 7374 4675 6c6c 2857 616c 6c43 6172  postFull(WallCar
+0001d230: 6f75 7365 6c42 6173 652c 2057 616c 6c57  ouselBase, WallW
+0001d240: 616c 6c70 6f73 7429 3a0a 0963 6f70 795f  allpost):..copy_
+0001d250: 6869 7374 6f72 793a 4f70 7469 6f6e 616c  history:Optional
+0001d260: 5b6c 6973 745b 2257 616c 6c57 616c 6c70  [list["WallWallp
+0001d270: 6f73 7446 756c 6c22 5d5d 203d 204e 6f6e  ostFull"]] = Non
+0001d280: 650a 0963 616e 5f65 6469 743a 4f70 7469  e..can_edit:Opti
+0001d290: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+0001d2a0: 650a 0963 7265 6174 6564 5f62 793a 4f70  e..created_by:Op
+0001d2b0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0001d2c0: 6e65 0a09 6361 6e5f 6465 6c65 7465 3a4f  ne..can_delete:O
+0001d2d0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0001d2e0: 4e6f 6e65 0a09 6361 6e5f 7069 6e3a 4f70  None..can_pin:Op
+0001d2f0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+0001d300: 6f6e 650a 0964 6f6e 7574 3a4f 7074 696f  one..donut:Optio
+0001d310: 6e61 6c5b 2257 616c 6c57 616c 6c70 6f73  nal["WallWallpos
+0001d320: 7444 6f6e 7574 225d 203d 204e 6f6e 650a  tDonut"] = None.
+0001d330: 0969 735f 7069 6e6e 6564 3a4f 7074 696f  .is_pinned:Optio
+0001d340: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0001d350: 0963 6f6d 6d65 6e74 733a 4f70 7469 6f6e  .comments:Option
+0001d360: 616c 5b22 4261 7365 436f 6d6d 656e 7473  al["BaseComments
+0001d370: 496e 666f 225d 203d 204e 6f6e 650a 096d  Info"] = None..m
+0001d380: 6172 6b65 645f 6173 5f61 6473 3a4f 7074  arked_as_ads:Opt
+0001d390: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
+0001d3a0: 6e65 0a09 746f 7069 635f 6964 3a4f 7074  ne..topic_id:Opt
+0001d3b0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0001d3c0: 650a 0973 686f 7274 5f74 6578 745f 7261  e..short_text_ra
+0001d3d0: 7465 3a4f 7074 696f 6e61 6c5b 696e 745d  te:Optional[int]
+0001d3e0: 203d 204e 6f6e 650a 0968 6173 683a 4f70   = None..hash:Op
+0001d3f0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0001d400: 6e65 0a0a 636c 6173 7320 4d65 7373 6167  ne..class Messag
+0001d410: 6573 5573 6572 5874 7249 6e76 6974 6564  esUserXtrInvited
+0001d420: 4279 2855 7365 7273 5573 6572 5874 7254  By(UsersUserXtrT
+0001d430: 7970 6529 3a0a 0969 6e76 6974 6564 5f62  ype):..invited_b
+0001d440: 793a 4f70 7469 6f6e 616c 5b69 6e74 5d20  y:Optional[int] 
+0001d450: 3d20 4e6f 6e65 0a0a 636c 6173 7320 4e65  = None..class Ne
+0001d460: 7773 6665 6564 4974 656d 5761 6c6c 706f  wsfeedItemWallpo
+0001d470: 7374 284e 6577 7366 6565 6449 7465 6d42  st(NewsfeedItemB
+0001d480: 6173 652c 2057 616c 6c57 616c 6c70 6f73  ase, WallWallpos
+0001d490: 7446 756c 6c29 3a0a 0966 6565 6462 6163  tFull):..feedbac
+0001d4a0: 6b3a 4f70 7469 6f6e 616c 5b22 4e65 7773  k:Optional["News
+0001d4b0: 6665 6564 4974 656d 5761 6c6c 706f 7374  feedItemWallpost
+0001d4c0: 4665 6564 6261 636b 225d 203d 204e 6f6e  Feedback"] = Non
+0001d4d0: 650a 0a63 6c61 7373 2047 726f 7570 7355  e..class GroupsU
+0001d4e0: 7365 7258 7472 526f 6c65 2855 7365 7273  serXtrRole(Users
+0001d4f0: 5573 6572 4675 6c6c 293a 0a09 726f 6c65  UserFull):..role
+0001d500: 3a4f 7074 696f 6e61 6c5b 2247 726f 7570  :Optional["Group
+0001d510: 7352 6f6c 654f 7074 696f 6e73 225d 203d  sRoleOptions"] =
+0001d520: 204e 6f6e 650a 0a63 6c61 7373 2046 7269   None..class Fri
+0001d530: 656e 6473 5573 6572 5874 7250 686f 6e65  endsUserXtrPhone
+0001d540: 2855 7365 7273 5573 6572 4675 6c6c 293a  (UsersUserFull):
+0001d550: 0a09 7068 6f6e 653a 4f70 7469 6f6e 616c  ..phone:Optional
+0001d560: 5b73 7472 5d20 3d20 4e6f 6e65 0a0a 2320  [str] = None..# 
+0001d570: d18d d182 d0be 20d0 bfd0 b8d0 b7d0 b4d0  ...... .........
+0001d580: b5d1 8620 d0bf d0be d0bb d0bd d18b d0b9  ... ............
+0001d590: 0a66 6f72 2069 2069 6e20 2841 6363 6f75  .for i in (Accou
+0001d5a0: 6e74 4163 636f 756e 7443 6f75 6e74 6572  ntAccountCounter
+0001d5b0: 732c 2041 6363 6f75 6e74 496e 666f 2c20  s, AccountInfo, 
+0001d5c0: 4163 636f 756e 744e 616d 6552 6571 7565  AccountNameReque
+0001d5d0: 7374 2c20 4163 636f 756e 744e 616d 6552  st, AccountNameR
+0001d5e0: 6571 7565 7374 5374 6174 7573 2c20 4163  equestStatus, Ac
+0001d5f0: 636f 756e 744f 6666 6572 2c20 4163 636f  countOffer, Acco
+0001d600: 756e 7450 7573 6843 6f6e 7665 7273 6174  untPushConversat
+0001d610: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+0001d620: 4163 636f 756e 7450 7573 6843 6f6e 7665  AccountPushConve
+0001d630: 7273 6174 696f 6e73 4974 656d 2c20 4163  rsationsItem, Ac
+0001d640: 636f 756e 7450 7573 6850 6172 616d 732c  countPushParams,
+0001d650: 2041 6363 6f75 6e74 5075 7368 5061 7261   AccountPushPara
+0001d660: 6d73 4d6f 6465 2c20 4163 636f 756e 7450  msMode, AccountP
+0001d670: 7573 6850 6172 616d 734f 6e6f 6666 2c20  ushParamsOnoff, 
+0001d680: 4163 636f 756e 7450 7573 6850 6172 616d  AccountPushParam
+0001d690: 7353 6574 7469 6e67 732c 0a20 2020 2020  sSettings,.     
+0001d6a0: 2020 2020 2041 6363 6f75 6e74 5075 7368       AccountPush
+0001d6b0: 5365 7474 696e 6773 2c20 4163 636f 756e  Settings, Accoun
+0001d6c0: 7453 7562 7363 7269 7074 696f 6e73 2c20  tSubscriptions, 
+0001d6d0: 4163 636f 756e 7455 7365 7253 6574 7469  AccountUserSetti
+0001d6e0: 6e67 732c 2041 6363 6f75 6e74 5573 6572  ngs, AccountUser
+0001d6f0: 5365 7474 696e 6773 496e 7465 7265 7374  SettingsInterest
+0001d700: 2c20 4163 636f 756e 7455 7365 7253 6574  , AccountUserSet
+0001d710: 7469 6e67 7349 6e74 6572 6573 7473 2c20  tingsInterests, 
+0001d720: 4164 6472 6573 7365 7346 6965 6c64 732c  AddressesFields,
+0001d730: 0a20 2020 2020 2020 2020 2041 6473 4163  .          AdsAc
+0001d740: 6365 7373 526f 6c65 2c20 4164 7341 6363  cessRole, AdsAcc
+0001d750: 6573 7352 6f6c 6550 7562 6c69 632c 2041  essRolePublic, A
+0001d760: 6473 4163 6365 7373 6573 2c20 4164 7341  dsAccesses, AdsA
+0001d770: 6363 6f75 6e74 2c20 4164 7341 6363 6f75  ccount, AdsAccou
+0001d780: 6e74 5479 7065 2c20 4164 7341 642c 2041  ntType, AdsAd, A
+0001d790: 6473 4164 4170 7072 6f76 6564 2c20 4164  dsAdApproved, Ad
+0001d7a0: 7341 6443 6f73 7454 7970 652c 2041 6473  sAdCostType, Ads
+0001d7b0: 4164 4c61 796f 7574 2c20 4164 7341 6453  AdLayout, AdsAdS
+0001d7c0: 7461 7475 732c 0a20 2020 2020 2020 2020  tatus,.         
+0001d7d0: 2041 6473 4361 6d70 6169 676e 2c20 4164   AdsCampaign, Ad
+0001d7e0: 7343 616d 7061 6967 6e53 7461 7475 732c  sCampaignStatus,
+0001d7f0: 2041 6473 4361 6d70 6169 676e 5479 7065   AdsCampaignType
+0001d800: 2c20 4164 7343 6174 6567 6f72 792c 2041  , AdsCategory, A
+0001d810: 6473 436c 6965 6e74 2c20 4164 7343 7265  dsClient, AdsCre
+0001d820: 6174 6541 6453 7461 7475 732c 2041 6473  ateAdStatus, Ads
+0001d830: 4372 6561 7465 4361 6d70 6169 676e 5374  CreateCampaignSt
+0001d840: 6174 7573 2c20 4164 7343 7269 7465 7269  atus, AdsCriteri
+0001d850: 612c 0a20 2020 2020 2020 2020 2041 6473  a,.          Ads
+0001d860: 4372 6974 6572 6961 5365 782c 2041 6473  CriteriaSex, Ads
+0001d870: 4465 6d6f 5374 6174 732c 2041 6473 4465  DemoStats, AdsDe
+0001d880: 6d6f 7374 6174 7346 6f72 6d61 742c 2041  mostatsFormat, A
+0001d890: 6473 466c 6f6f 6453 7461 7473 2c20 4164  dsFloodStats, Ad
+0001d8a0: 734c 696e 6b53 7461 7475 732c 2041 6473  sLinkStatus, Ads
+0001d8b0: 4c6f 6f6b 616c 696b 6552 6571 7565 7374  LookalikeRequest
+0001d8c0: 2c20 4164 734c 6f6f 6b61 6c69 6b65 5265  , AdsLookalikeRe
+0001d8d0: 7175 6573 7453 6176 6541 7564 6965 6e63  questSaveAudienc
+0001d8e0: 654c 6576 656c 2c0a 2020 2020 2020 2020  eLevel,.        
+0001d8f0: 2020 4164 734d 7573 6963 6961 6e2c 2041    AdsMusician, A
+0001d900: 6473 4f62 6a65 6374 5479 7065 2c20 4164  dsObjectType, Ad
+0001d910: 7350 6172 6167 7261 7068 732c 2041 6473  sParagraphs, Ads
+0001d920: 5072 6f6d 6f74 6564 506f 7374 5265 6163  PromotedPostReac
+0001d930: 682c 2041 6473 5265 6a65 6374 5265 6173  h, AdsRejectReas
+0001d940: 6f6e 2c20 4164 7352 756c 6573 2c20 4164  on, AdsRules, Ad
+0001d950: 7353 7461 7473 2c20 4164 7353 7461 7473  sStats, AdsStats
+0001d960: 4167 652c 2041 6473 5374 6174 7343 6974  Age, AdsStatsCit
+0001d970: 6965 732c 0a20 2020 2020 2020 2020 2041  ies,.          A
+0001d980: 6473 5374 6174 7346 6f72 6d61 742c 2041  dsStatsFormat, A
+0001d990: 6473 5374 6174 7353 6578 2c20 4164 7353  dsStatsSex, AdsS
+0001d9a0: 7461 7473 5365 7841 6765 2c20 4164 7353  tatsSexAge, AdsS
+0001d9b0: 7461 7473 5365 7856 616c 7565 2c20 4164  tatsSexValue, Ad
+0001d9c0: 7353 7461 7473 5669 6577 7354 696d 6573  sStatsViewsTimes
+0001d9d0: 2c20 4164 7354 6172 6753 6574 7469 6e67  , AdsTargSetting
+0001d9e0: 732c 2041 6473 5461 7267 5374 6174 732c  s, AdsTargStats,
+0001d9f0: 2041 6473 5461 7267 5375 6767 6573 7469   AdsTargSuggesti
+0001da00: 6f6e 732c 0a20 2020 2020 2020 2020 2041  ons,.          A
 0001da10: 6473 5461 7267 5375 6767 6573 7469 6f6e  dsTargSuggestion
-0001da20: 7352 6567 696f 6e73 2c20 4164 7354 6172  sRegions, AdsTar
-0001da30: 6753 7567 6765 7374 696f 6e73 5363 686f  gSuggestionsScho
-0001da40: 6f6c 732c 2041 6473 5461 7267 5375 6767  ols, AdsTargSugg
-0001da50: 6573 7469 6f6e 7353 6368 6f6f 6c73 5479  estionsSchoolsTy
-0001da60: 7065 2c20 4164 7354 6172 6765 7447 726f  pe, AdsTargetGro
-0001da70: 7570 2c0a 2020 2020 2020 2020 2020 4164  up,.          Ad
-0001da80: 7355 7064 6174 654f 6666 6963 6555 7365  sUpdateOfficeUse
-0001da90: 7273 5265 7375 6c74 2c20 4164 7355 7365  rsResult, AdsUse
-0001daa0: 7253 7065 6369 6669 6361 7469 6f6e 2c20  rSpecification, 
-0001dab0: 4164 7355 7365 7253 7065 6369 6669 6361  AdsUserSpecifica
-0001dac0: 7469 6f6e 4375 7474 6564 2c20 4164 7355  tionCutted, AdsU
-0001dad0: 7365 7273 2c20 4164 7377 6562 4765 7441  sers, AdswebGetA
-0001dae0: 6443 6174 6567 6f72 6965 7352 6573 706f  dCategoriesRespo
-0001daf0: 6e73 6543 6174 6567 6f72 6965 7343 6174  nseCategoriesCat
-0001db00: 6567 6f72 792c 0a20 2020 2020 2020 2020  egory,.         
-0001db10: 2041 6473 7765 6247 6574 4164 556e 6974   AdswebGetAdUnit
-0001db20: 7352 6573 706f 6e73 6541 6455 6e69 7473  sResponseAdUnits
-0001db30: 4164 556e 6974 2c20 4164 7377 6562 4765  AdUnit, AdswebGe
-0001db40: 7446 7261 7564 4869 7374 6f72 7952 6573  tFraudHistoryRes
-0001db50: 706f 6e73 6545 6e74 7269 6573 456e 7472  ponseEntriesEntr
-0001db60: 792c 2041 6473 7765 6247 6574 5369 7465  y, AdswebGetSite
-0001db70: 7352 6573 706f 6e73 6553 6974 6573 5369  sResponseSitesSi
-0001db80: 7465 2c0a 2020 2020 2020 2020 2020 4164  te,.          Ad
-0001db90: 7377 6562 4765 7453 7461 7469 7374 6963  swebGetStatistic
-0001dba0: 7352 6573 706f 6e73 6549 7465 6d73 4974  sResponseItemsIt
-0001dbb0: 656d 2c20 4170 7057 6964 6765 7473 5068  em, AppWidgetsPh
-0001dbc0: 6f74 6f2c 2041 7070 5769 6467 6574 7350  oto, AppWidgetsP
-0001dbd0: 686f 746f 732c 2041 7070 7341 7070 2c20  hotos, AppsApp, 
-0001dbe0: 4170 7073 4170 704c 6561 6465 7262 6f61  AppsAppLeaderboa
-0001dbf0: 7264 5479 7065 2c20 4170 7073 4170 704d  rdType, AppsAppM
-0001dc00: 696e 2c20 4170 7073 4170 7054 7970 652c  in, AppsAppType,
-0001dc10: 0a20 2020 2020 2020 2020 2041 7070 7343  .          AppsC
-0001dc20: 6174 616c 6f67 4c69 7374 2c20 4170 7073  atalogList, Apps
-0001dc30: 4c65 6164 6572 626f 6172 642c 2041 7070  Leaderboard, App
-0001dc40: 7353 636f 7065 2c20 4175 6469 6f41 7564  sScope, AudioAud
-0001dc50: 696f 2c20 4261 7365 4369 7479 2c20 4261  io, BaseCity, Ba
-0001dc60: 7365 436f 6d6d 656e 7473 496e 666f 2c20  seCommentsInfo, 
-0001dc70: 4261 7365 436f 756e 7472 792c 2042 6173  BaseCountry, Bas
-0001dc80: 6543 726f 7050 686f 746f 2c20 4261 7365  eCropPhoto, Base
-0001dc90: 4372 6f70 5068 6f74 6f43 726f 702c 0a20  CropPhotoCrop,. 
-0001dca0: 2020 2020 2020 2020 2042 6173 6543 726f           BaseCro
-0001dcb0: 7050 686f 746f 5265 6374 2c20 4261 7365  pPhotoRect, Base
-0001dcc0: 4572 726f 722c 2042 6173 6547 656f 2c20  Error, BaseGeo, 
-0001dcd0: 4261 7365 4765 6f43 6f6f 7264 696e 6174  BaseGeoCoordinat
-0001dce0: 6573 2c20 4261 7365 4772 6164 6965 6e74  es, BaseGradient
-0001dcf0: 506f 696e 742c 2042 6173 6549 6d61 6765  Point, BaseImage
-0001dd00: 2c20 4261 7365 4c69 6b65 732c 2042 6173  , BaseLikes, Bas
-0001dd10: 654c 696b 6573 496e 666f 2c20 4261 7365  eLikesInfo, Base
-0001dd20: 4c69 6e6b 2c0a 2020 2020 2020 2020 2020  Link,.          
-0001dd30: 4261 7365 4c69 6e6b 4170 706c 6963 6174  BaseLinkApplicat
-0001dd40: 696f 6e2c 2042 6173 654c 696e 6b41 7070  ion, BaseLinkApp
-0001dd50: 6c69 6361 7469 6f6e 5374 6f72 652c 2042  licationStore, B
-0001dd60: 6173 654c 696e 6b42 7574 746f 6e2c 2042  aseLinkButton, B
-0001dd70: 6173 654c 696e 6b42 7574 746f 6e41 6374  aseLinkButtonAct
-0001dd80: 696f 6e2c 2042 6173 654c 696e 6b42 7574  ion, BaseLinkBut
-0001dd90: 746f 6e41 6374 696f 6e54 7970 652c 2042  tonActionType, B
-0001dda0: 6173 654c 696e 6b42 7574 746f 6e53 7479  aseLinkButtonSty
-0001ddb0: 6c65 2c0a 2020 2020 2020 2020 2020 4261  le,.          Ba
-0001ddc0: 7365 4c69 6e6b 5072 6f64 7563 742c 2042  seLinkProduct, B
-0001ddd0: 6173 654c 696e 6b50 726f 6475 6374 4361  aseLinkProductCa
-0001dde0: 7465 676f 7279 2c20 4261 7365 4c69 6e6b  tegory, BaseLink
-0001ddf0: 5072 6f64 7563 7453 7461 7475 732c 2042  ProductStatus, B
-0001de00: 6173 654c 696e 6b52 6174 696e 672c 2042  aseLinkRating, B
-0001de10: 6173 654d 6573 7361 6765 4572 726f 722c  aseMessageError,
-0001de20: 2042 6173 654f 626a 6563 742c 2042 6173   BaseObject, Bas
-0001de30: 654f 626a 6563 7443 6f75 6e74 2c0a 2020  eObjectCount,.  
-0001de40: 2020 2020 2020 2020 4261 7365 4f62 6a65          BaseObje
-0001de50: 6374 5769 7468 4e61 6d65 2c20 4261 7365  ctWithName, Base
-0001de60: 506c 6163 652c 2042 6173 6550 726f 7065  Place, BasePrope
-0001de70: 7274 7945 7869 7374 732c 2042 6173 6552  rtyExists, BaseR
-0001de80: 6570 6f73 7473 496e 666f 2c20 4261 7365  epostsInfo, Base
-0001de90: 5265 7175 6573 7450 6172 616d 2c20 4261  RequestParam, Ba
-0001dea0: 7365 5365 782c 2042 6173 6553 7469 636b  seSex, BaseStick
-0001deb0: 6572 2c20 4261 7365 5374 6963 6b65 7241  er, BaseStickerA
-0001dec0: 6e69 6d61 7469 6f6e 2c0a 2020 2020 2020  nimation,.      
-0001ded0: 2020 2020 4261 7365 5374 6963 6b65 724e      BaseStickerN
-0001dee0: 6577 2c20 4261 7365 5374 6963 6b65 724f  ew, BaseStickerO
-0001def0: 6c64 2c20 4261 7365 5374 6963 6b65 7273  ld, BaseStickers
-0001df00: 4c69 7374 2c20 4261 7365 5570 6c6f 6164  List, BaseUpload
-0001df10: 5365 7276 6572 2c20 4261 7365 5573 6572  Server, BaseUser
-0001df20: 4772 6f75 7046 6965 6c64 732c 2042 6173  GroupFields, Bas
-0001df30: 6555 7365 7249 642c 2042 6f61 7264 4465  eUserId, BoardDe
-0001df40: 6661 756c 744f 7264 6572 2c20 426f 6172  faultOrder, Boar
-0001df50: 6454 6f70 6963 2c0a 2020 2020 2020 2020  dTopic,.        
-0001df60: 2020 426f 6172 6454 6f70 6963 436f 6d6d    BoardTopicComm
-0001df70: 656e 742c 2043 616c 6c62 6163 6b42 6173  ent, CallbackBas
-0001df80: 652c 2043 616c 6c62 6163 6b42 6f61 7264  e, CallbackBoard
-0001df90: 506f 7374 4465 6c65 7465 2c20 4361 6c6c  PostDelete, Call
-0001dfa0: 6261 636b 436f 6e66 6972 6d61 7469 6f6e  backConfirmation
-0001dfb0: 2c20 4361 6c6c 6261 636b 446f 6e75 744d  , CallbackDonutM
-0001dfc0: 6f6e 6579 5769 7468 6472 6177 2c20 4361  oneyWithdraw, Ca
-0001dfd0: 6c6c 6261 636b 446f 6e75 744d 6f6e 6579  llbackDonutMoney
-0001dfe0: 5769 7468 6472 6177 4572 726f 722c 0a20  WithdrawError,. 
-0001dff0: 2020 2020 2020 2020 2043 616c 6c62 6163           Callbac
-0001e000: 6b44 6f6e 7574 5375 6273 6372 6970 7469  kDonutSubscripti
-0001e010: 6f6e 4361 6e63 656c 6c65 642c 2043 616c  onCancelled, Cal
-0001e020: 6c62 6163 6b44 6f6e 7574 5375 6273 6372  lbackDonutSubscr
-0001e030: 6970 7469 6f6e 4372 6561 7465 2c20 4361  iptionCreate, Ca
-0001e040: 6c6c 6261 636b 446f 6e75 7453 7562 7363  llbackDonutSubsc
-0001e050: 7269 7074 696f 6e45 7870 6972 6564 2c0a  riptionExpired,.
-0001e060: 2020 2020 2020 2020 2020 4361 6c6c 6261            Callba
-0001e070: 636b 446f 6e75 7453 7562 7363 7269 7074  ckDonutSubscript
-0001e080: 696f 6e50 7269 6365 4368 616e 6765 642c  ionPriceChanged,
-0001e090: 2043 616c 6c62 6163 6b44 6f6e 7574 5375   CallbackDonutSu
-0001e0a0: 6273 6372 6970 7469 6f6e 5072 6f6c 6f6e  bscriptionProlon
-0001e0b0: 6765 642c 2043 616c 6c62 6163 6b47 726f  ged, CallbackGro
-0001e0c0: 7570 4368 616e 6765 5068 6f74 6f2c 2043  upChangePhoto, C
+0001da20: 7343 6974 6965 732c 2041 6473 5461 7267  sCities, AdsTarg
+0001da30: 5375 6767 6573 7469 6f6e 7352 6567 696f  SuggestionsRegio
+0001da40: 6e73 2c20 4164 7354 6172 6753 7567 6765  ns, AdsTargSugge
+0001da50: 7374 696f 6e73 5363 686f 6f6c 732c 2041  stionsSchools, A
+0001da60: 6473 5461 7267 5375 6767 6573 7469 6f6e  dsTargSuggestion
+0001da70: 7353 6368 6f6f 6c73 5479 7065 2c20 4164  sSchoolsType, Ad
+0001da80: 7354 6172 6765 7447 726f 7570 2c0a 2020  sTargetGroup,.  
+0001da90: 2020 2020 2020 2020 4164 7355 7064 6174          AdsUpdat
+0001daa0: 654f 6666 6963 6555 7365 7273 5265 7375  eOfficeUsersResu
+0001dab0: 6c74 2c20 4164 7355 7365 7253 7065 6369  lt, AdsUserSpeci
+0001dac0: 6669 6361 7469 6f6e 2c20 4164 7355 7365  fication, AdsUse
+0001dad0: 7253 7065 6369 6669 6361 7469 6f6e 4375  rSpecificationCu
+0001dae0: 7474 6564 2c20 4164 7355 7365 7273 2c20  tted, AdsUsers, 
+0001daf0: 4164 7377 6562 4765 7441 6443 6174 6567  AdswebGetAdCateg
+0001db00: 6f72 6965 7352 6573 706f 6e73 6543 6174  oriesResponseCat
+0001db10: 6567 6f72 6965 7343 6174 6567 6f72 792c  egoriesCategory,
+0001db20: 0a20 2020 2020 2020 2020 2041 6473 7765  .          Adswe
+0001db30: 6247 6574 4164 556e 6974 7352 6573 706f  bGetAdUnitsRespo
+0001db40: 6e73 6541 6455 6e69 7473 4164 556e 6974  nseAdUnitsAdUnit
+0001db50: 2c20 4164 7377 6562 4765 7446 7261 7564  , AdswebGetFraud
+0001db60: 4869 7374 6f72 7952 6573 706f 6e73 6545  HistoryResponseE
+0001db70: 6e74 7269 6573 456e 7472 792c 2041 6473  ntriesEntry, Ads
+0001db80: 7765 6247 6574 5369 7465 7352 6573 706f  webGetSitesRespo
+0001db90: 6e73 6553 6974 6573 5369 7465 2c0a 2020  nseSitesSite,.  
+0001dba0: 2020 2020 2020 2020 4164 7377 6562 4765          AdswebGe
+0001dbb0: 7453 7461 7469 7374 6963 7352 6573 706f  tStatisticsRespo
+0001dbc0: 6e73 6549 7465 6d73 4974 656d 2c20 4170  nseItemsItem, Ap
+0001dbd0: 7057 6964 6765 7473 5068 6f74 6f2c 2041  pWidgetsPhoto, A
+0001dbe0: 7070 5769 6467 6574 7350 686f 746f 732c  ppWidgetsPhotos,
+0001dbf0: 2041 7070 7341 7070 2c20 4170 7073 4170   AppsApp, AppsAp
+0001dc00: 704c 6561 6465 7262 6f61 7264 5479 7065  pLeaderboardType
+0001dc10: 2c20 4170 7073 4170 704d 696e 2c20 4170  , AppsAppMin, Ap
+0001dc20: 7073 4170 7054 7970 652c 0a20 2020 2020  psAppType,.     
+0001dc30: 2020 2020 2041 7070 7343 6174 616c 6f67       AppsCatalog
+0001dc40: 4c69 7374 2c20 4170 7073 4c65 6164 6572  List, AppsLeader
+0001dc50: 626f 6172 642c 2041 7070 7353 636f 7065  board, AppsScope
+0001dc60: 2c20 4175 6469 6f41 7564 696f 2c20 4261  , AudioAudio, Ba
+0001dc70: 7365 4369 7479 2c20 4261 7365 436f 6d6d  seCity, BaseComm
+0001dc80: 656e 7473 496e 666f 2c20 4261 7365 436f  entsInfo, BaseCo
+0001dc90: 756e 7472 792c 2042 6173 6543 726f 7050  untry, BaseCropP
+0001dca0: 686f 746f 2c20 4261 7365 4372 6f70 5068  hoto, BaseCropPh
+0001dcb0: 6f74 6f43 726f 702c 0a20 2020 2020 2020  otoCrop,.       
+0001dcc0: 2020 2042 6173 6543 726f 7050 686f 746f     BaseCropPhoto
+0001dcd0: 5265 6374 2c20 4261 7365 4572 726f 722c  Rect, BaseError,
+0001dce0: 2042 6173 6547 656f 2c20 4261 7365 4765   BaseGeo, BaseGe
+0001dcf0: 6f43 6f6f 7264 696e 6174 6573 2c20 4261  oCoordinates, Ba
+0001dd00: 7365 4772 6164 6965 6e74 506f 696e 742c  seGradientPoint,
+0001dd10: 2042 6173 6549 6d61 6765 2c20 4261 7365   BaseImage, Base
+0001dd20: 4c69 6b65 732c 2042 6173 654c 696b 6573  Likes, BaseLikes
+0001dd30: 496e 666f 2c20 4261 7365 4c69 6e6b 2c0a  Info, BaseLink,.
+0001dd40: 2020 2020 2020 2020 2020 4261 7365 4c69            BaseLi
+0001dd50: 6e6b 4170 706c 6963 6174 696f 6e2c 2042  nkApplication, B
+0001dd60: 6173 654c 696e 6b41 7070 6c69 6361 7469  aseLinkApplicati
+0001dd70: 6f6e 5374 6f72 652c 2042 6173 654c 696e  onStore, BaseLin
+0001dd80: 6b42 7574 746f 6e2c 2042 6173 654c 696e  kButton, BaseLin
+0001dd90: 6b42 7574 746f 6e41 6374 696f 6e2c 2042  kButtonAction, B
+0001dda0: 6173 654c 696e 6b42 7574 746f 6e41 6374  aseLinkButtonAct
+0001ddb0: 696f 6e54 7970 652c 2042 6173 654c 696e  ionType, BaseLin
+0001ddc0: 6b42 7574 746f 6e53 7479 6c65 2c0a 2020  kButtonStyle,.  
+0001ddd0: 2020 2020 2020 2020 4261 7365 4c69 6e6b          BaseLink
+0001dde0: 5072 6f64 7563 742c 2042 6173 654c 696e  Product, BaseLin
+0001ddf0: 6b50 726f 6475 6374 4361 7465 676f 7279  kProductCategory
+0001de00: 2c20 4261 7365 4c69 6e6b 5072 6f64 7563  , BaseLinkProduc
+0001de10: 7453 7461 7475 732c 2042 6173 654c 696e  tStatus, BaseLin
+0001de20: 6b52 6174 696e 672c 2042 6173 654d 6573  kRating, BaseMes
+0001de30: 7361 6765 4572 726f 722c 2042 6173 654f  sageError, BaseO
+0001de40: 626a 6563 742c 2042 6173 654f 626a 6563  bject, BaseObjec
+0001de50: 7443 6f75 6e74 2c0a 2020 2020 2020 2020  tCount,.        
+0001de60: 2020 4261 7365 4f62 6a65 6374 5769 7468    BaseObjectWith
+0001de70: 4e61 6d65 2c20 4261 7365 506c 6163 652c  Name, BasePlace,
+0001de80: 2042 6173 6550 726f 7065 7274 7945 7869   BasePropertyExi
+0001de90: 7374 732c 2042 6173 6552 6570 6f73 7473  sts, BaseReposts
+0001dea0: 496e 666f 2c20 4261 7365 5265 7175 6573  Info, BaseReques
+0001deb0: 7450 6172 616d 2c20 4261 7365 5365 782c  tParam, BaseSex,
+0001dec0: 2042 6173 6553 7469 636b 6572 2c20 4261   BaseSticker, Ba
+0001ded0: 7365 5374 6963 6b65 7241 6e69 6d61 7469  seStickerAnimati
+0001dee0: 6f6e 2c0a 2020 2020 2020 2020 2020 4261  on,.          Ba
+0001def0: 7365 5374 6963 6b65 724e 6577 2c20 4261  seStickerNew, Ba
+0001df00: 7365 5374 6963 6b65 724f 6c64 2c20 4261  seStickerOld, Ba
+0001df10: 7365 5374 6963 6b65 7273 4c69 7374 2c20  seStickersList, 
+0001df20: 4261 7365 5570 6c6f 6164 5365 7276 6572  BaseUploadServer
+0001df30: 2c20 4261 7365 5573 6572 4772 6f75 7046  , BaseUserGroupF
+0001df40: 6965 6c64 732c 2042 6173 6555 7365 7249  ields, BaseUserI
+0001df50: 642c 2042 6f61 7264 4465 6661 756c 744f  d, BoardDefaultO
+0001df60: 7264 6572 2c20 426f 6172 6454 6f70 6963  rder, BoardTopic
+0001df70: 2c0a 2020 2020 2020 2020 2020 426f 6172  ,.          Boar
+0001df80: 6454 6f70 6963 436f 6d6d 656e 742c 2043  dTopicComment, C
+0001df90: 616c 6c62 6163 6b42 6173 652c 2043 616c  allbackBase, Cal
+0001dfa0: 6c62 6163 6b42 6f61 7264 506f 7374 4465  lbackBoardPostDe
+0001dfb0: 6c65 7465 2c20 4361 6c6c 6261 636b 436f  lete, CallbackCo
+0001dfc0: 6e66 6972 6d61 7469 6f6e 2c20 4361 6c6c  nfirmation, Call
+0001dfd0: 6261 636b 446f 6e75 744d 6f6e 6579 5769  backDonutMoneyWi
+0001dfe0: 7468 6472 6177 2c20 4361 6c6c 6261 636b  thdraw, Callback
+0001dff0: 446f 6e75 744d 6f6e 6579 5769 7468 6472  DonutMoneyWithdr
+0001e000: 6177 4572 726f 722c 0a20 2020 2020 2020  awError,.       
+0001e010: 2020 2043 616c 6c62 6163 6b44 6f6e 7574     CallbackDonut
+0001e020: 5375 6273 6372 6970 7469 6f6e 4361 6e63  SubscriptionCanc
+0001e030: 656c 6c65 642c 2043 616c 6c62 6163 6b44  elled, CallbackD
+0001e040: 6f6e 7574 5375 6273 6372 6970 7469 6f6e  onutSubscription
+0001e050: 4372 6561 7465 2c20 4361 6c6c 6261 636b  Create, Callback
+0001e060: 446f 6e75 7453 7562 7363 7269 7074 696f  DonutSubscriptio
+0001e070: 6e45 7870 6972 6564 2c0a 2020 2020 2020  nExpired,.      
+0001e080: 2020 2020 4361 6c6c 6261 636b 446f 6e75      CallbackDonu
+0001e090: 7453 7562 7363 7269 7074 696f 6e50 7269  tSubscriptionPri
+0001e0a0: 6365 4368 616e 6765 642c 2043 616c 6c62  ceChanged, Callb
+0001e0b0: 6163 6b44 6f6e 7574 5375 6273 6372 6970  ackDonutSubscrip
+0001e0c0: 7469 6f6e 5072 6f6c 6f6e 6765 642c 2043  tionProlonged, C
 0001e0d0: 616c 6c62 6163 6b47 726f 7570 4368 616e  allbackGroupChan
-0001e0e0: 6765 5365 7474 696e 6773 2c0a 2020 2020  geSettings,.    
-0001e0f0: 2020 2020 2020 4361 6c6c 6261 636b 4772        CallbackGr
-0001e100: 6f75 704a 6f69 6e2c 2043 616c 6c62 6163  oupJoin, Callbac
-0001e110: 6b47 726f 7570 4a6f 696e 5479 7065 2c20  kGroupJoinType, 
-0001e120: 4361 6c6c 6261 636b 4772 6f75 704c 6561  CallbackGroupLea
-0001e130: 7665 2c20 4361 6c6c 6261 636b 4772 6f75  ve, CallbackGrou
-0001e140: 704d 6172 6b65 742c 2043 616c 6c62 6163  pMarket, Callbac
-0001e150: 6b47 726f 7570 4f66 6669 6365 7252 6f6c  kGroupOfficerRol
-0001e160: 652c 2043 616c 6c62 6163 6b47 726f 7570  e, CallbackGroup
-0001e170: 4f66 6669 6365 7273 4564 6974 2c0a 2020  OfficersEdit,.  
-0001e180: 2020 2020 2020 2020 4361 6c6c 6261 636b          Callback
-0001e190: 4772 6f75 7053 6574 7469 6e67 7343 6861  GroupSettingsCha
-0001e1a0: 6e67 6573 2c20 4361 6c6c 6261 636b 4c69  nges, CallbackLi
-0001e1b0: 6b65 4164 6452 656d 6f76 652c 2043 616c  keAddRemove, Cal
-0001e1c0: 6c62 6163 6b4d 6172 6b65 7443 6f6d 6d65  lbackMarketComme
-0001e1d0: 6e74 2c20 4361 6c6c 6261 636b 4d61 726b  nt, CallbackMark
-0001e1e0: 6574 436f 6d6d 656e 7444 656c 6574 652c  etCommentDelete,
-0001e1f0: 2043 616c 6c62 6163 6b4d 6573 7361 6765   CallbackMessage
-0001e200: 416c 6c6f 772c 0a20 2020 2020 2020 2020  Allow,.         
-0001e210: 2043 616c 6c62 6163 6b4d 6573 7361 6765   CallbackMessage
-0001e220: 416c 6c6f 774f 626a 6563 742c 2043 616c  AllowObject, Cal
-0001e230: 6c62 6163 6b4d 6573 7361 6765 4465 6e79  lbackMessageDeny
-0001e240: 2c20 4361 6c6c 6261 636b 4d65 7373 6167  , CallbackMessag
-0001e250: 6545 6469 742c 2043 616c 6c62 6163 6b4d  eEdit, CallbackM
-0001e260: 6573 7361 6765 4e65 772c 2043 616c 6c62  essageNew, Callb
-0001e270: 6163 6b4d 6573 7361 6765 4f62 6a65 6374  ackMessageObject
-0001e280: 2c20 4361 6c6c 6261 636b 4d65 7373 6167  , CallbackMessag
-0001e290: 6552 6570 6c79 2c0a 2020 2020 2020 2020  eReply,.        
-0001e2a0: 2020 4361 6c6c 6261 636b 5068 6f74 6f43    CallbackPhotoC
-0001e2b0: 6f6d 6d65 6e74 2c20 4361 6c6c 6261 636b  omment, Callback
-0001e2c0: 5068 6f74 6f43 6f6d 6d65 6e74 4465 6c65  PhotoCommentDele
-0001e2d0: 7465 2c20 4361 6c6c 6261 636b 506f 6c6c  te, CallbackPoll
-0001e2e0: 566f 7465 4e65 772c 2043 616c 6c62 6163  VoteNew, Callbac
-0001e2f0: 6b51 7253 6361 6e2c 2043 616c 6c62 6163  kQrScan, Callbac
-0001e300: 6b54 7970 652c 2043 616c 6c62 6163 6b55  kType, CallbackU
-0001e310: 7365 7242 6c6f 636b 2c20 4361 6c6c 6261  serBlock, Callba
-0001e320: 636b 5573 6572 556e 626c 6f63 6b2c 0a20  ckUserUnblock,. 
-0001e330: 2020 2020 2020 2020 2043 616c 6c62 6163           Callbac
-0001e340: 6b56 6964 656f 436f 6d6d 656e 742c 2043  kVideoComment, C
-0001e350: 616c 6c62 6163 6b56 6964 656f 436f 6d6d  allbackVideoComm
-0001e360: 656e 7444 656c 6574 652c 2043 616c 6c62  entDelete, Callb
-0001e370: 6163 6b57 616c 6c43 6f6d 6d65 6e74 4465  ackWallCommentDe
-0001e380: 6c65 7465 2c20 4361 6c6c 7343 616c 6c2c  lete, CallsCall,
-0001e390: 2043 616c 6c73 456e 6453 7461 7465 2c20   CallsEndState, 
-0001e3a0: 4361 6c6c 7350 6172 7469 6369 7061 6e74  CallsParticipant
-0001e3b0: 732c 2043 6c69 656e 7449 6e66 6f46 6f72  s, ClientInfoFor
-0001e3c0: 426f 7473 2c0a 2020 2020 2020 2020 2020  Bots,.          
-0001e3d0: 436f 6d6d 656e 7454 6872 6561 642c 2044  CommentThread, D
-0001e3e0: 6174 6162 6173 6543 6974 792c 2044 6174  atabaseCity, Dat
-0001e3f0: 6162 6173 6543 6974 7942 7949 642c 2044  abaseCityById, D
-0001e400: 6174 6162 6173 6546 6163 756c 7479 2c20  atabaseFaculty, 
-0001e410: 4461 7461 6261 7365 5265 6769 6f6e 2c20  DatabaseRegion, 
-0001e420: 4461 7461 6261 7365 5363 686f 6f6c 2c20  DatabaseSchool, 
-0001e430: 4461 7461 6261 7365 5374 6174 696f 6e2c  DatabaseStation,
-0001e440: 2044 6174 6162 6173 6555 6e69 7665 7273   DatabaseUnivers
-0001e450: 6974 792c 0a20 2020 2020 2020 2020 2044  ity,.          D
-0001e460: 6f63 7344 6f63 2c20 446f 6373 446f 6341  ocsDoc, DocsDocA
-0001e470: 7474 6163 686d 656e 7454 7970 652c 2044  ttachmentType, D
-0001e480: 6f63 7344 6f63 5072 6576 6965 772c 2044  ocsDocPreview, D
-0001e490: 6f63 7344 6f63 5072 6576 6965 7741 7564  ocsDocPreviewAud
-0001e4a0: 696f 4d73 672c 2044 6f63 7344 6f63 5072  ioMsg, DocsDocPr
-0001e4b0: 6576 6965 7747 7261 6666 6974 692c 2044  eviewGraffiti, D
-0001e4c0: 6f63 7344 6f63 5072 6576 6965 7750 686f  ocsDocPreviewPho
-0001e4d0: 746f 2c0a 2020 2020 2020 2020 2020 446f  to,.          Do
-0001e4e0: 6373 446f 6350 7265 7669 6577 5068 6f74  csDocPreviewPhot
-0001e4f0: 6f53 697a 6573 2c20 446f 6373 446f 6350  oSizes, DocsDocP
-0001e500: 7265 7669 6577 5669 6465 6f2c 2044 6f63  reviewVideo, Doc
-0001e510: 7344 6f63 5479 7065 732c 2044 6f6e 7574  sDocTypes, Donut
-0001e520: 446f 6e61 746f 7253 7562 7363 7269 7074  DonatorSubscript
-0001e530: 696f 6e49 6e66 6f2c 2045 7665 6e74 7345  ionInfo, EventsE
-0001e540: 7665 6e74 4174 7461 6368 2c20 4661 7665  ventAttach, Fave
-0001e550: 426f 6f6b 6d61 726b 2c0a 2020 2020 2020  Bookmark,.      
-0001e560: 2020 2020 4661 7665 426f 6f6b 6d61 726b      FaveBookmark
-0001e570: 5479 7065 2c20 4661 7665 5061 6765 2c20  Type, FavePage, 
-0001e580: 4661 7665 5061 6765 5479 7065 2c20 4661  FavePageType, Fa
-0001e590: 7665 5461 672c 2046 7269 656e 6473 4672  veTag, FriendsFr
-0001e5a0: 6965 6e64 4578 7465 6e64 6564 5374 6174  iendExtendedStat
-0001e5b0: 7573 2c20 4672 6965 6e64 7346 7269 656e  us, FriendsFrien
-0001e5c0: 6453 7461 7475 732c 2046 7269 656e 6473  dStatus, Friends
-0001e5d0: 4672 6965 6e64 5374 6174 7573 5374 6174  FriendStatusStat
-0001e5e0: 7573 2c0a 2020 2020 2020 2020 2020 4672  us,.          Fr
-0001e5f0: 6965 6e64 7346 7269 656e 6473 4c69 7374  iendsFriendsList
-0001e600: 2c20 4672 6965 6e64 734d 7574 7561 6c46  , FriendsMutualF
-0001e610: 7269 656e 642c 2046 7269 656e 6473 5265  riend, FriendsRe
-0001e620: 7175 6573 7473 2c20 4672 6965 6e64 7352  quests, FriendsR
-0001e630: 6571 7565 7374 734d 7574 7561 6c2c 2046  equestsMutual, F
-0001e640: 7269 656e 6473 5265 7175 6573 7473 5874  riendsRequestsXt
-0001e650: 724d 6573 7361 6765 2c20 4672 6965 6e64  rMessage, Friend
-0001e660: 7355 7365 7258 7472 5068 6f6e 652c 2047  sUserXtrPhone, G
-0001e670: 6966 7473 4769 6674 2c0a 2020 2020 2020  iftsGift,.      
-0001e680: 2020 2020 4769 6674 7347 6966 7450 7269      GiftsGiftPri
-0001e690: 7661 6379 2c20 4769 6674 734c 6179 6f75  vacy, GiftsLayou
-0001e6a0: 742c 2047 726f 7570 7341 6464 7265 7373  t, GroupsAddress
-0001e6b0: 2c20 4772 6f75 7073 4164 6472 6573 7354  , GroupsAddressT
-0001e6c0: 696d 6574 6162 6c65 2c20 4772 6f75 7073  imetable, Groups
-0001e6d0: 4164 6472 6573 7354 696d 6574 6162 6c65  AddressTimetable
-0001e6e0: 4461 792c 2047 726f 7570 7341 6464 7265  Day, GroupsAddre
-0001e6f0: 7373 576f 726b 496e 666f 5374 6174 7573  ssWorkInfoStatus
-0001e700: 2c0a 2020 2020 2020 2020 2020 4772 6f75  ,.          Grou
-0001e710: 7073 4164 6472 6573 7365 7349 6e66 6f2c  psAddressesInfo,
-0001e720: 2047 726f 7570 7342 616e 496e 666f 2c20   GroupsBanInfo, 
-0001e730: 4772 6f75 7073 4261 6e49 6e66 6f52 6561  GroupsBanInfoRea
-0001e740: 736f 6e2c 2047 726f 7570 7342 616e 6e65  son, GroupsBanne
-0001e750: 6449 7465 6d2c 2047 726f 7570 7343 616c  dItem, GroupsCal
-0001e760: 6c62 6163 6b53 6572 7665 722c 2047 726f  lbackServer, Gro
-0001e770: 7570 7343 616c 6c62 6163 6b53 6574 7469  upsCallbackSetti
-0001e780: 6e67 732c 2047 726f 7570 7343 6f6e 7461  ngs, GroupsConta
-0001e790: 6374 7349 7465 6d2c 0a20 2020 2020 2020  ctsItem,.       
-0001e7a0: 2020 2047 726f 7570 7343 6f75 6e74 6572     GroupsCounter
-0001e7b0: 7347 726f 7570 2c20 4772 6f75 7073 436f  sGroup, GroupsCo
-0001e7c0: 7665 722c 2047 726f 7570 7346 6965 6c64  ver, GroupsField
-0001e7d0: 732c 2047 726f 7570 7346 696c 7465 722c  s, GroupsFilter,
-0001e7e0: 2047 726f 7570 7347 726f 7570 2c20 4772   GroupsGroup, Gr
-0001e7f0: 6f75 7073 4772 6f75 7041 6363 6573 732c  oupsGroupAccess,
-0001e800: 2047 726f 7570 7347 726f 7570 4164 6d69   GroupsGroupAdmi
-0001e810: 6e4c 6576 656c 2c20 4772 6f75 7073 4772  nLevel, GroupsGr
-0001e820: 6f75 7041 6765 4c69 6d69 7473 2c0a 2020  oupAgeLimits,.  
-0001e830: 2020 2020 2020 2020 4772 6f75 7073 4772          GroupsGr
-0001e840: 6f75 7041 7474 6163 682c 2047 726f 7570  oupAttach, Group
-0001e850: 7347 726f 7570 4175 6469 6f2c 2047 726f  sGroupAudio, Gro
-0001e860: 7570 7347 726f 7570 4261 6e49 6e66 6f2c  upsGroupBanInfo,
-0001e870: 2047 726f 7570 7347 726f 7570 4361 7465   GroupsGroupCate
-0001e880: 676f 7279 2c20 4772 6f75 7073 4772 6f75  gory, GroupsGrou
-0001e890: 7043 6174 6567 6f72 7946 756c 6c2c 2047  pCategoryFull, G
-0001e8a0: 726f 7570 7347 726f 7570 4361 7465 676f  roupsGroupCatego
-0001e8b0: 7279 5479 7065 2c0a 2020 2020 2020 2020  ryType,.        
-0001e8c0: 2020 4772 6f75 7073 4772 6f75 7044 6f63    GroupsGroupDoc
-0001e8d0: 732c 2047 726f 7570 7347 726f 7570 4675  s, GroupsGroupFu
-0001e8e0: 6c6c 2c20 4772 6f75 7073 4772 6f75 7046  ll, GroupsGroupF
-0001e8f0: 756c 6c41 6765 4c69 6d69 7473 2c20 4772  ullAgeLimits, Gr
-0001e900: 6f75 7073 4772 6f75 7046 756c 6c4d 656d  oupsGroupFullMem
-0001e910: 6265 7253 7461 7475 732c 2047 726f 7570  berStatus, Group
-0001e920: 7347 726f 7570 4675 6c6c 5365 6374 696f  sGroupFullSectio
-0001e930: 6e2c 2047 726f 7570 7347 726f 7570 4973  n, GroupsGroupIs
-0001e940: 436c 6f73 6564 2c0a 2020 2020 2020 2020  Closed,.        
-0001e950: 2020 4772 6f75 7073 4772 6f75 704d 6172    GroupsGroupMar
-0001e960: 6b65 7443 7572 7265 6e63 792c 2047 726f  ketCurrency, Gro
-0001e970: 7570 7347 726f 7570 5068 6f74 6f73 2c20  upsGroupPhotos, 
-0001e980: 4772 6f75 7073 4772 6f75 7050 7562 6c69  GroupsGroupPubli
-0001e990: 6343 6174 6567 6f72 794c 6973 742c 2047  cCategoryList, G
-0001e9a0: 726f 7570 7347 726f 7570 526f 6c65 2c20  roupsGroupRole, 
-0001e9b0: 4772 6f75 7073 4772 6f75 7053 7562 6a65  GroupsGroupSubje
-0001e9c0: 6374 2c0a 2020 2020 2020 2020 2020 4772  ct,.          Gr
-0001e9d0: 6f75 7073 4772 6f75 7053 7567 6765 7374  oupsGroupSuggest
-0001e9e0: 6564 5072 6976 6163 792c 2047 726f 7570  edPrivacy, Group
-0001e9f0: 7347 726f 7570 5461 672c 2047 726f 7570  sGroupTag, Group
-0001ea00: 7347 726f 7570 546f 7069 6373 2c20 4772  sGroupTopics, Gr
-0001ea10: 6f75 7073 4772 6f75 7054 7970 652c 2047  oupsGroupType, G
-0001ea20: 726f 7570 7347 726f 7570 5669 6465 6f2c  roupsGroupVideo,
-0001ea30: 2047 726f 7570 7347 726f 7570 5761 6c6c   GroupsGroupWall
-0001ea40: 2c20 4772 6f75 7073 4772 6f75 7057 696b  , GroupsGroupWik
-0001ea50: 692c 0a20 2020 2020 2020 2020 2047 726f  i,.          Gro
-0001ea60: 7570 7347 726f 7570 7341 7272 6179 2c20  upsGroupsArray, 
-0001ea70: 4772 6f75 7073 4c69 6e6b 7349 7465 6d2c  GroupsLinksItem,
-0001ea80: 2047 726f 7570 734c 6976 6543 6f76 6572   GroupsLiveCover
-0001ea90: 732c 2047 726f 7570 734c 6f6e 6750 6f6c  s, GroupsLongPol
-0001eaa0: 6c45 7665 6e74 732c 2047 726f 7570 734c  lEvents, GroupsL
-0001eab0: 6f6e 6750 6f6c 6c53 6572 7665 722c 2047  ongPollServer, G
-0001eac0: 726f 7570 734c 6f6e 6750 6f6c 6c53 6574  roupsLongPollSet
-0001ead0: 7469 6e67 732c 2047 726f 7570 734d 6172  tings, GroupsMar
-0001eae0: 6b65 7449 6e66 6f2c 0a20 2020 2020 2020  ketInfo,.       
-0001eaf0: 2020 2047 726f 7570 734d 6172 6b65 7453     GroupsMarketS
-0001eb00: 7461 7465 2c20 4772 6f75 7073 4d65 6d62  tate, GroupsMemb
-0001eb10: 6572 526f 6c65 2c20 4772 6f75 7073 4d65  erRole, GroupsMe
-0001eb20: 6d62 6572 526f 6c65 5065 726d 6973 7369  mberRolePermissi
-0001eb30: 6f6e 2c20 4772 6f75 7073 4d65 6d62 6572  on, GroupsMember
-0001eb40: 526f 6c65 5374 6174 7573 2c20 4772 6f75  RoleStatus, Grou
-0001eb50: 7073 4d65 6d62 6572 5374 6174 7573 2c20  psMemberStatus, 
-0001eb60: 4772 6f75 7073 4d65 6d62 6572 5374 6174  GroupsMemberStat
-0001eb70: 7573 4675 6c6c 2c0a 2020 2020 2020 2020  usFull,.        
-0001eb80: 2020 4772 6f75 7073 4f6e 6c69 6e65 5374    GroupsOnlineSt
-0001eb90: 6174 7573 2c20 4772 6f75 7073 4f6e 6c69  atus, GroupsOnli
-0001eba0: 6e65 5374 6174 7573 5479 7065 2c20 4772  neStatusType, Gr
-0001ebb0: 6f75 7073 4f77 6e65 7258 7472 4261 6e49  oupsOwnerXtrBanI
-0001ebc0: 6e66 6f2c 2047 726f 7570 734f 776e 6572  nfo, GroupsOwner
-0001ebd0: 5874 7242 616e 496e 666f 5479 7065 2c20  XtrBanInfoType, 
-0001ebe0: 4772 6f75 7073 5068 6f74 6f53 697a 652c  GroupsPhotoSize,
-0001ebf0: 2047 726f 7570 7352 6f6c 654f 7074 696f   GroupsRoleOptio
-0001ec00: 6e73 2c0a 2020 2020 2020 2020 2020 4772  ns,.          Gr
-0001ec10: 6f75 7073 5365 6374 696f 6e73 4c69 7374  oupsSectionsList
-0001ec20: 4974 656d 2c20 4772 6f75 7073 5365 7474  Item, GroupsSett
-0001ec30: 696e 6773 5477 6974 7465 722c 2047 726f  ingsTwitter, Gro
-0001ec40: 7570 7353 7562 6a65 6374 4974 656d 2c20  upsSubjectItem, 
-0001ec50: 4772 6f75 7073 546f 6b65 6e50 6572 6d69  GroupsTokenPermi
-0001ec60: 7373 696f 6e53 6574 7469 6e67 2c20 4772  ssionSetting, Gr
-0001ec70: 6f75 7073 5573 6572 5874 7252 6f6c 652c  oupsUserXtrRole,
-0001ec80: 204c 6561 6446 6f72 6d73 416e 7377 6572   LeadFormsAnswer
-0001ec90: 2c0a 2020 2020 2020 2020 2020 4c65 6164  ,.          Lead
-0001eca0: 466f 726d 7341 6e73 7765 7249 7465 6d2c  FormsAnswerItem,
-0001ecb0: 204c 6561 6446 6f72 6d73 466f 726d 2c20   LeadFormsForm, 
-0001ecc0: 4c65 6164 466f 726d 734c 6561 642c 204c  LeadFormsLead, L
-0001ecd0: 6561 6446 6f72 6d73 5175 6573 7469 6f6e  eadFormsQuestion
-0001ece0: 4974 656d 2c20 4c65 6164 466f 726d 7351  Item, LeadFormsQ
-0001ecf0: 7565 7374 696f 6e49 7465 6d4f 7074 696f  uestionItemOptio
-0001ed00: 6e2c 204c 696b 6573 5479 7065 2c20 4c69  n, LikesType, Li
-0001ed10: 6e6b 5461 7267 6574 4f62 6a65 6374 2c0a  nkTargetObject,.
-0001ed20: 2020 2020 2020 2020 2020 4d61 726b 6574            Market
-0001ed30: 4375 7272 656e 6379 2c20 4d61 726b 6574  Currency, Market
-0001ed40: 4d61 726b 6574 416c 6275 6d2c 204d 6172  MarketAlbum, Mar
-0001ed50: 6b65 744d 6172 6b65 7443 6174 6567 6f72  ketMarketCategor
-0001ed60: 792c 204d 6172 6b65 744d 6172 6b65 7443  y, MarketMarketC
-0001ed70: 6174 6567 6f72 794e 6573 7465 642c 204d  ategoryNested, M
-0001ed80: 6172 6b65 744d 6172 6b65 7443 6174 6567  arketMarketCateg
-0001ed90: 6f72 794f 6c64 2c20 4d61 726b 6574 4d61  oryOld, MarketMa
-0001eda0: 726b 6574 4361 7465 676f 7279 5472 6565  rketCategoryTree
-0001edb0: 2c0a 2020 2020 2020 2020 2020 4d61 726b  ,.          Mark
-0001edc0: 6574 4d61 726b 6574 4974 656d 2c20 4d61  etMarketItem, Ma
-0001edd0: 726b 6574 4d61 726b 6574 4974 656d 4176  rketMarketItemAv
-0001ede0: 6169 6c61 6269 6c69 7479 2c20 4d61 726b  ailability, Mark
-0001edf0: 6574 4d61 726b 6574 4974 656d 4675 6c6c  etMarketItemFull
-0001ee00: 2c20 4d61 726b 6574 4f72 6465 722c 204d  , MarketOrder, M
-0001ee10: 6172 6b65 744f 7264 6572 4974 656d 2c20  arketOrderItem, 
-0001ee20: 4d61 726b 6574 5072 6963 652c 204d 6172  MarketPrice, Mar
-0001ee30: 6b65 7453 6563 7469 6f6e 2c0a 2020 2020  ketSection,.    
-0001ee40: 2020 2020 2020 4d61 726b 6574 5365 7276        MarketServ
-0001ee50: 6963 6573 5669 6577 5479 7065 2c20 4d65  icesViewType, Me
-0001ee60: 7373 6167 6573 4175 6469 6f4d 6573 7361  ssagesAudioMessa
-0001ee70: 6765 2c20 4d65 7373 6167 6573 4368 6174  ge, MessagesChat
-0001ee80: 2c20 4d65 7373 6167 6573 4368 6174 4675  , MessagesChatFu
-0001ee90: 6c6c 2c20 4d65 7373 6167 6573 4368 6174  ll, MessagesChat
-0001eea0: 5072 6576 6965 772c 204d 6573 7361 6765  Preview, Message
-0001eeb0: 7343 6861 7450 7573 6853 6574 7469 6e67  sChatPushSetting
-0001eec0: 732c 0a20 2020 2020 2020 2020 204d 6573  s,.          Mes
-0001eed0: 7361 6765 7343 6861 7452 6573 7472 6963  sagesChatRestric
-0001eee0: 7469 6f6e 732c 204d 6573 7361 6765 7343  tions, MessagesC
-0001eef0: 6861 7453 6574 7469 6e67 732c 204d 6573  hatSettings, Mes
-0001ef00: 7361 6765 7343 6861 7453 6574 7469 6e67  sagesChatSetting
-0001ef10: 7341 636c 2c20 4d65 7373 6167 6573 4368  sAcl, MessagesCh
-0001ef20: 6174 5365 7474 696e 6773 5065 726d 6973  atSettingsPermis
-0001ef30: 7369 6f6e 732c 204d 6573 7361 6765 7343  sions, MessagesC
-0001ef40: 6861 7453 6574 7469 6e67 7350 686f 746f  hatSettingsPhoto
-0001ef50: 2c0a 2020 2020 2020 2020 2020 4d65 7373  ,.          Mess
-0001ef60: 6167 6573 4368 6174 5365 7474 696e 6773  agesChatSettings
-0001ef70: 5374 6174 652c 204d 6573 7361 6765 7343  State, MessagesC
-0001ef80: 6f6e 7665 7273 6174 696f 6e2c 204d 6573  onversation, Mes
-0001ef90: 7361 6765 7343 6f6e 7665 7273 6174 696f  sagesConversatio
-0001efa0: 6e43 616e 5772 6974 652c 204d 6573 7361  nCanWrite, Messa
-0001efb0: 6765 7343 6f6e 7665 7273 6174 696f 6e4d  gesConversationM
-0001efc0: 656d 6265 722c 204d 6573 7361 6765 7343  ember, MessagesC
-0001efd0: 6f6e 7665 7273 6174 696f 6e50 6565 722c  onversationPeer,
-0001efe0: 0a20 2020 2020 2020 2020 204d 6573 7361  .          Messa
-0001eff0: 6765 7343 6f6e 7665 7273 6174 696f 6e50  gesConversationP
-0001f000: 6565 7254 7970 652c 204d 6573 7361 6765  eerType, Message
-0001f010: 7343 6f6e 7665 7273 6174 696f 6e53 6f72  sConversationSor
-0001f020: 7449 642c 204d 6573 7361 6765 7343 6f6e  tId, MessagesCon
-0001f030: 7665 7273 6174 696f 6e57 6974 684d 6573  versationWithMes
-0001f040: 7361 6765 2c20 4d65 7373 6167 6573 466f  sage, MessagesFo
-0001f050: 7265 6967 6e4d 6573 7361 6765 2c20 4d65  reignMessage, Me
-0001f060: 7373 6167 6573 466f 7277 6172 642c 0a20  ssagesForward,. 
-0001f070: 2020 2020 2020 2020 204d 6573 7361 6765           Message
-0001f080: 7347 6574 436f 6e76 6572 7361 7469 6f6e  sGetConversation
-0001f090: 4279 4964 2c20 4d65 7373 6167 6573 4765  ById, MessagesGe
-0001f0a0: 7443 6f6e 7665 7273 6174 696f 6e42 7949  tConversationByI
-0001f0b0: 6445 7874 656e 6465 642c 204d 6573 7361  dExtended, Messa
-0001f0c0: 6765 7347 6574 436f 6e76 6572 7361 7469  gesGetConversati
-0001f0d0: 6f6e 4d65 6d62 6572 732c 204d 6573 7361  onMembers, Messa
-0001f0e0: 6765 7347 7261 6666 6974 692c 0a20 2020  gesGraffiti,.   
-0001f0f0: 2020 2020 2020 204d 6573 7361 6765 7348         MessagesH
-0001f100: 6973 746f 7279 4174 7461 6368 6d65 6e74  istoryAttachment
-0001f110: 2c20 4d65 7373 6167 6573 4869 7374 6f72  , MessagesHistor
-0001f120: 794d 6573 7361 6765 4174 7461 6368 6d65  yMessageAttachme
-0001f130: 6e74 2c20 4d65 7373 6167 6573 4869 7374  nt, MessagesHist
-0001f140: 6f72 794d 6573 7361 6765 4174 7461 6368  oryMessageAttach
-0001f150: 6d65 6e74 5479 7065 2c20 4d65 7373 6167  mentType, Messag
-0001f160: 6573 4b65 7962 6f61 7264 2c20 4d65 7373  esKeyboard, Mess
-0001f170: 6167 6573 4b65 7962 6f61 7264 4275 7474  agesKeyboardButt
-0001f180: 6f6e 2c0a 4d65 7373 6167 6573 4b65 7962  on,.MessagesKeyb
-0001f190: 6f61 7264 4275 7474 6f6e 4163 7469 6f6e  oardButtonAction
-0001f1a0: 4361 6c6c 6261 636b 2c20 4d65 7373 6167  Callback, Messag
-0001f1b0: 6573 4b65 7962 6f61 7264 4275 7474 6f6e  esKeyboardButton
-0001f1c0: 4163 7469 6f6e 4c6f 6361 7469 6f6e 2c20  ActionLocation, 
-0001f1d0: 4d65 7373 6167 6573 4b65 7962 6f61 7264  MessagesKeyboard
-0001f1e0: 4275 7474 6f6e 4163 7469 6f6e 4f70 656e  ButtonActionOpen
-0001f1f0: 4170 702c 204d 6573 7361 6765 734b 6579  App, MessagesKey
-0001f200: 626f 6172 6442 7574 746f 6e41 6374 696f  boardButtonActio
-0001f210: 6e4f 7065 6e4c 696e 6b2c 0a4d 6573 7361  nOpenLink,.Messa
-0001f220: 6765 734b 6579 626f 6172 6442 7574 746f  gesKeyboardButto
-0001f230: 6e41 6374 696f 6e4f 7065 6e50 686f 746f  nActionOpenPhoto
-0001f240: 2c20 4d65 7373 6167 6573 4b65 7962 6f61  , MessagesKeyboa
-0001f250: 7264 4275 7474 6f6e 4163 7469 6f6e 5465  rdButtonActionTe
-0001f260: 7874 2c20 4d65 7373 6167 6573 4b65 7962  xt, MessagesKeyb
-0001f270: 6f61 7264 4275 7474 6f6e 4163 7469 6f6e  oardButtonAction
-0001f280: 566b 7061 792c 204d 6573 7361 6765 734b  Vkpay, MessagesK
-0001f290: 6579 626f 6172 6442 7574 746f 6e50 726f  eyboardButtonPro
-0001f2a0: 7065 7274 7941 6374 696f 6e2c 0a4d 6573  pertyAction,.Mes
-0001f2b0: 7361 6765 734c 6173 7441 6374 6976 6974  sagesLastActivit
-0001f2c0: 792c 204d 6573 7361 6765 734c 6f6e 6770  y, MessagesLongp
-0001f2d0: 6f6c 6c4d 6573 7361 6765 732c 204d 6573  ollMessages, Mes
-0001f2e0: 7361 6765 734c 6f6e 6770 6f6c 6c50 6172  sagesLongpollPar
-0001f2f0: 616d 732c 204d 6573 7361 6765 734d 6573  ams, MessagesMes
-0001f300: 7361 6765 2c20 4d65 7373 6167 6573 4d65  sage, MessagesMe
-0001f310: 7373 6167 6541 6374 696f 6e2c 204d 6573  ssageAction, Mes
-0001f320: 7361 6765 734d 6573 7361 6765 4163 7469  sagesMessageActi
-0001f330: 6f6e 5068 6f74 6f2c 0a4d 6573 7361 6765  onPhoto,.Message
-0001f340: 734d 6573 7361 6765 4163 7469 6f6e 5374  sMessageActionSt
-0001f350: 6174 7573 2c20 4d65 7373 6167 6573 4d65  atus, MessagesMe
-0001f360: 7373 6167 6541 7474 6163 686d 656e 742c  ssageAttachment,
-0001f370: 204d 6573 7361 6765 734d 6573 7361 6765   MessagesMessage
-0001f380: 4174 7461 6368 6d65 6e74 5479 7065 2c20  AttachmentType, 
-0001f390: 4d65 7373 6167 6573 4d65 7373 6167 6552  MessagesMessageR
-0001f3a0: 6571 7565 7374 4461 7461 2c20 4d65 7373  equestData, Mess
-0001f3b0: 6167 6573 4d65 7373 6167 6573 4172 7261  agesMessagesArra
-0001f3c0: 792c 0a4d 6573 7361 6765 734f 7574 5265  y,.MessagesOutRe
-0001f3d0: 6164 4279 2c20 4d65 7373 6167 6573 5069  adBy, MessagesPi
-0001f3e0: 6e6e 6564 4d65 7373 6167 652c 204d 6573  nnedMessage, Mes
-0001f3f0: 7361 6765 7350 7573 6853 6574 7469 6e67  sagesPushSetting
-0001f400: 732c 204d 6573 7361 6765 7353 656e 6455  s, MessagesSendU
-0001f410: 7365 7249 6473 5265 7370 6f6e 7365 4974  serIdsResponseIt
-0001f420: 656d 2c20 4d65 7373 6167 6573 5465 6d70  em, MessagesTemp
-0001f430: 6c61 7465 4163 7469 6f6e 5479 7065 4e61  lateActionTypeNa
-0001f440: 6d65 732c 0a4d 6573 7361 6765 7355 7365  mes,.MessagesUse
-0001f450: 7258 7472 496e 7669 7465 6442 792c 204e  rXtrInvitedBy, N
-0001f460: 6577 7366 6565 6443 6f6d 6d65 6e74 7346  ewsfeedCommentsF
-0001f470: 696c 7465 7273 2c20 4e65 7773 6665 6564  ilters, Newsfeed
-0001f480: 4967 6e6f 7265 4974 656d 5479 7065 2c20  IgnoreItemType, 
-0001f490: 4e65 7773 6665 6564 4974 656d 4175 6469  NewsfeedItemAudi
-0001f4a0: 6f2c 204e 6577 7366 6565 6449 7465 6d41  o, NewsfeedItemA
-0001f4b0: 7564 696f 4175 6469 6f2c 204e 6577 7366  udioAudio, Newsf
-0001f4c0: 6565 6449 7465 6d42 6173 652c 0a4e 6577  eedItemBase,.New
-0001f4d0: 7366 6565 6449 7465 6d44 6967 6573 742c  sfeedItemDigest,
-0001f4e0: 204e 6577 7366 6565 6449 7465 6d44 6967   NewsfeedItemDig
-0001f4f0: 6573 7442 7574 746f 6e2c 204e 6577 7366  estButton, Newsf
-0001f500: 6565 6449 7465 6d44 6967 6573 7446 6f6f  eedItemDigestFoo
-0001f510: 7465 722c 204e 6577 7366 6565 6449 7465  ter, NewsfeedIte
-0001f520: 6d44 6967 6573 7446 756c 6c49 7465 6d2c  mDigestFullItem,
-0001f530: 204e 6577 7366 6565 6449 7465 6d44 6967   NewsfeedItemDig
-0001f540: 6573 7448 6561 6465 722c 204e 6577 7366  estHeader, Newsf
-0001f550: 6565 6449 7465 6d44 6967 6573 7449 7465  eedItemDigestIte
-0001f560: 6d2c 0a4e 6577 7366 6565 6449 7465 6d46  m,.NewsfeedItemF
-0001f570: 7269 656e 642c 204e 6577 7366 6565 6449  riend, NewsfeedI
-0001f580: 7465 6d46 7269 656e 6446 7269 656e 6473  temFriendFriends
-0001f590: 2c20 4e65 7773 6665 6564 4974 656d 486f  , NewsfeedItemHo
-0001f5a0: 6c69 6461 7952 6563 6f6d 6d65 6e64 6174  lidayRecommendat
-0001f5b0: 696f 6e73 426c 6f63 6b48 6561 6465 722c  ionsBlockHeader,
-0001f5c0: 204e 6577 7366 6565 6449 7465 6d50 686f   NewsfeedItemPho
-0001f5d0: 746f 2c20 4e65 7773 6665 6564 4974 656d  to, NewsfeedItem
-0001f5e0: 5068 6f74 6f50 686f 746f 732c 0a4e 6577  PhotoPhotos,.New
-0001f5f0: 7366 6565 6449 7465 6d50 686f 746f 5461  sfeedItemPhotoTa
-0001f600: 672c 204e 6577 7366 6565 6449 7465 6d50  g, NewsfeedItemP
-0001f610: 686f 746f 5461 6750 686f 746f 5461 6773  hotoTagPhotoTags
-0001f620: 2c20 4e65 7773 6665 6564 4974 656d 5072  , NewsfeedItemPr
-0001f630: 6f6d 6f42 7574 746f 6e2c 204e 6577 7366  omoButton, Newsf
-0001f640: 6565 6449 7465 6d50 726f 6d6f 4275 7474  eedItemPromoButt
-0001f650: 6f6e 4163 7469 6f6e 2c20 4e65 7773 6665  onAction, Newsfe
-0001f660: 6564 4974 656d 5072 6f6d 6f42 7574 746f  edItemPromoButto
-0001f670: 6e49 6d61 6765 2c0a 4e65 7773 6665 6564  nImage,.Newsfeed
-0001f680: 4974 656d 546f 7069 632c 204e 6577 7366  ItemTopic, Newsf
-0001f690: 6565 6449 7465 6d56 6964 656f 2c20 4e65  eedItemVideo, Ne
-0001f6a0: 7773 6665 6564 4974 656d 5669 6465 6f56  wsfeedItemVideoV
-0001f6b0: 6964 656f 2c20 4e65 7773 6665 6564 4974  ideo, NewsfeedIt
-0001f6c0: 656d 5761 6c6c 706f 7374 2c20 4e65 7773  emWallpost, News
-0001f6d0: 6665 6564 4974 656d 5761 6c6c 706f 7374  feedItemWallpost
-0001f6e0: 4665 6564 6261 636b 2c20 4e65 7773 6665  Feedback, Newsfe
-0001f6f0: 6564 4974 656d 5761 6c6c 706f 7374 4665  edItemWallpostFe
-0001f700: 6564 6261 636b 416e 7377 6572 2c0a 4e65  edbackAnswer,.Ne
-0001f710: 7773 6665 6564 4974 656d 5761 6c6c 706f  wsfeedItemWallpo
-0001f720: 7374 4665 6564 6261 636b 5479 7065 2c20  stFeedbackType, 
-0001f730: 4e65 7773 6665 6564 4c69 7374 2c20 4e65  NewsfeedList, Ne
-0001f740: 7773 6665 6564 4c69 7374 4675 6c6c 2c20  wsfeedListFull, 
-0001f750: 4e65 7773 6665 6564 4e65 7773 6665 6564  NewsfeedNewsfeed
-0001f760: 4974 656d 2c20 4e65 7773 6665 6564 4e65  Item, NewsfeedNe
-0001f770: 7773 6665 6564 4974 656d 5479 7065 2c20  wsfeedItemType, 
+0001e0e0: 6765 5068 6f74 6f2c 2043 616c 6c62 6163  gePhoto, Callbac
+0001e0f0: 6b47 726f 7570 4368 616e 6765 5365 7474  kGroupChangeSett
+0001e100: 696e 6773 2c0a 2020 2020 2020 2020 2020  ings,.          
+0001e110: 4361 6c6c 6261 636b 4772 6f75 704a 6f69  CallbackGroupJoi
+0001e120: 6e2c 2043 616c 6c62 6163 6b47 726f 7570  n, CallbackGroup
+0001e130: 4a6f 696e 5479 7065 2c20 4361 6c6c 6261  JoinType, Callba
+0001e140: 636b 4772 6f75 704c 6561 7665 2c20 4361  ckGroupLeave, Ca
+0001e150: 6c6c 6261 636b 4772 6f75 704d 6172 6b65  llbackGroupMarke
+0001e160: 742c 2043 616c 6c62 6163 6b47 726f 7570  t, CallbackGroup
+0001e170: 4f66 6669 6365 7252 6f6c 652c 2043 616c  OfficerRole, Cal
+0001e180: 6c62 6163 6b47 726f 7570 4f66 6669 6365  lbackGroupOffice
+0001e190: 7273 4564 6974 2c0a 2020 2020 2020 2020  rsEdit,.        
+0001e1a0: 2020 4361 6c6c 6261 636b 4772 6f75 7053    CallbackGroupS
+0001e1b0: 6574 7469 6e67 7343 6861 6e67 6573 2c20  ettingsChanges, 
+0001e1c0: 4361 6c6c 6261 636b 4c69 6b65 4164 6452  CallbackLikeAddR
+0001e1d0: 656d 6f76 652c 2043 616c 6c62 6163 6b4d  emove, CallbackM
+0001e1e0: 6172 6b65 7443 6f6d 6d65 6e74 2c20 4361  arketComment, Ca
+0001e1f0: 6c6c 6261 636b 4d61 726b 6574 436f 6d6d  llbackMarketComm
+0001e200: 656e 7444 656c 6574 652c 2043 616c 6c62  entDelete, Callb
+0001e210: 6163 6b4d 6573 7361 6765 416c 6c6f 772c  ackMessageAllow,
+0001e220: 0a20 2020 2020 2020 2020 2043 616c 6c62  .          Callb
+0001e230: 6163 6b4d 6573 7361 6765 416c 6c6f 774f  ackMessageAllowO
+0001e240: 626a 6563 742c 2043 616c 6c62 6163 6b4d  bject, CallbackM
+0001e250: 6573 7361 6765 4465 6e79 2c20 4361 6c6c  essageDeny, Call
+0001e260: 6261 636b 4d65 7373 6167 6545 6469 742c  backMessageEdit,
+0001e270: 2043 616c 6c62 6163 6b4d 6573 7361 6765   CallbackMessage
+0001e280: 4e65 772c 2043 616c 6c62 6163 6b4d 6573  New, CallbackMes
+0001e290: 7361 6765 4f62 6a65 6374 2c20 4361 6c6c  sageObject, Call
+0001e2a0: 6261 636b 4d65 7373 6167 6552 6570 6c79  backMessageReply
+0001e2b0: 2c0a 2020 2020 2020 2020 2020 4361 6c6c  ,.          Call
+0001e2c0: 6261 636b 5068 6f74 6f43 6f6d 6d65 6e74  backPhotoComment
+0001e2d0: 2c20 4361 6c6c 6261 636b 5068 6f74 6f43  , CallbackPhotoC
+0001e2e0: 6f6d 6d65 6e74 4465 6c65 7465 2c20 4361  ommentDelete, Ca
+0001e2f0: 6c6c 6261 636b 506f 6c6c 566f 7465 4e65  llbackPollVoteNe
+0001e300: 772c 2043 616c 6c62 6163 6b51 7253 6361  w, CallbackQrSca
+0001e310: 6e2c 2043 616c 6c62 6163 6b54 7970 652c  n, CallbackType,
+0001e320: 2043 616c 6c62 6163 6b55 7365 7242 6c6f   CallbackUserBlo
+0001e330: 636b 2c20 4361 6c6c 6261 636b 5573 6572  ck, CallbackUser
+0001e340: 556e 626c 6f63 6b2c 0a20 2020 2020 2020  Unblock,.       
+0001e350: 2020 2043 616c 6c62 6163 6b56 6964 656f     CallbackVideo
+0001e360: 436f 6d6d 656e 742c 2043 616c 6c62 6163  Comment, Callbac
+0001e370: 6b56 6964 656f 436f 6d6d 656e 7444 656c  kVideoCommentDel
+0001e380: 6574 652c 2043 616c 6c62 6163 6b57 616c  ete, CallbackWal
+0001e390: 6c43 6f6d 6d65 6e74 4465 6c65 7465 2c20  lCommentDelete, 
+0001e3a0: 4361 6c6c 7343 616c 6c2c 2043 616c 6c73  CallsCall, Calls
+0001e3b0: 456e 6453 7461 7465 2c20 4361 6c6c 7350  EndState, CallsP
+0001e3c0: 6172 7469 6369 7061 6e74 732c 2043 6c69  articipants, Cli
+0001e3d0: 656e 7449 6e66 6f46 6f72 426f 7473 2c0a  entInfoForBots,.
+0001e3e0: 2020 2020 2020 2020 2020 436f 6d6d 656e            Commen
+0001e3f0: 7454 6872 6561 642c 2044 6174 6162 6173  tThread, Databas
+0001e400: 6543 6974 792c 2044 6174 6162 6173 6543  eCity, DatabaseC
+0001e410: 6974 7942 7949 642c 2044 6174 6162 6173  ityById, Databas
+0001e420: 6546 6163 756c 7479 2c20 4461 7461 6261  eFaculty, Databa
+0001e430: 7365 5265 6769 6f6e 2c20 4461 7461 6261  seRegion, Databa
+0001e440: 7365 5363 686f 6f6c 2c20 4461 7461 6261  seSchool, Databa
+0001e450: 7365 5374 6174 696f 6e2c 2044 6174 6162  seStation, Datab
+0001e460: 6173 6555 6e69 7665 7273 6974 792c 0a20  aseUniversity,. 
+0001e470: 2020 2020 2020 2020 2044 6f63 7344 6f63           DocsDoc
+0001e480: 2c20 446f 6373 446f 6341 7474 6163 686d  , DocsDocAttachm
+0001e490: 656e 7454 7970 652c 2044 6f63 7344 6f63  entType, DocsDoc
+0001e4a0: 5072 6576 6965 772c 2044 6f63 7344 6f63  Preview, DocsDoc
+0001e4b0: 5072 6576 6965 7741 7564 696f 4d73 672c  PreviewAudioMsg,
+0001e4c0: 2044 6f63 7344 6f63 5072 6576 6965 7747   DocsDocPreviewG
+0001e4d0: 7261 6666 6974 692c 2044 6f63 7344 6f63  raffiti, DocsDoc
+0001e4e0: 5072 6576 6965 7750 686f 746f 2c0a 2020  PreviewPhoto,.  
+0001e4f0: 2020 2020 2020 2020 446f 6373 446f 6350          DocsDocP
+0001e500: 7265 7669 6577 5068 6f74 6f53 697a 6573  reviewPhotoSizes
+0001e510: 2c20 446f 6373 446f 6350 7265 7669 6577  , DocsDocPreview
+0001e520: 5669 6465 6f2c 2044 6f63 7344 6f63 5479  Video, DocsDocTy
+0001e530: 7065 732c 2044 6f6e 7574 446f 6e61 746f  pes, DonutDonato
+0001e540: 7253 7562 7363 7269 7074 696f 6e49 6e66  rSubscriptionInf
+0001e550: 6f2c 2045 7665 6e74 7345 7665 6e74 4174  o, EventsEventAt
+0001e560: 7461 6368 2c20 4661 7665 426f 6f6b 6d61  tach, FaveBookma
+0001e570: 726b 2c0a 2020 2020 2020 2020 2020 4661  rk,.          Fa
+0001e580: 7665 426f 6f6b 6d61 726b 5479 7065 2c20  veBookmarkType, 
+0001e590: 4661 7665 5061 6765 2c20 4661 7665 5061  FavePage, FavePa
+0001e5a0: 6765 5479 7065 2c20 4661 7665 5461 672c  geType, FaveTag,
+0001e5b0: 2046 7269 656e 6473 4672 6965 6e64 4578   FriendsFriendEx
+0001e5c0: 7465 6e64 6564 5374 6174 7573 2c20 4672  tendedStatus, Fr
+0001e5d0: 6965 6e64 7346 7269 656e 6453 7461 7475  iendsFriendStatu
+0001e5e0: 732c 2046 7269 656e 6473 4672 6965 6e64  s, FriendsFriend
+0001e5f0: 5374 6174 7573 5374 6174 7573 2c0a 2020  StatusStatus,.  
+0001e600: 2020 2020 2020 2020 4672 6965 6e64 7346          FriendsF
+0001e610: 7269 656e 6473 4c69 7374 2c20 4672 6965  riendsList, Frie
+0001e620: 6e64 734d 7574 7561 6c46 7269 656e 642c  ndsMutualFriend,
+0001e630: 2046 7269 656e 6473 5265 7175 6573 7473   FriendsRequests
+0001e640: 2c20 4672 6965 6e64 7352 6571 7565 7374  , FriendsRequest
+0001e650: 734d 7574 7561 6c2c 2046 7269 656e 6473  sMutual, Friends
+0001e660: 5265 7175 6573 7473 5874 724d 6573 7361  RequestsXtrMessa
+0001e670: 6765 2c20 4672 6965 6e64 7355 7365 7258  ge, FriendsUserX
+0001e680: 7472 5068 6f6e 652c 2047 6966 7473 4769  trPhone, GiftsGi
+0001e690: 6674 2c0a 2020 2020 2020 2020 2020 4769  ft,.          Gi
+0001e6a0: 6674 7347 6966 7450 7269 7661 6379 2c20  ftsGiftPrivacy, 
+0001e6b0: 4769 6674 734c 6179 6f75 742c 2047 726f  GiftsLayout, Gro
+0001e6c0: 7570 7341 6464 7265 7373 2c20 4772 6f75  upsAddress, Grou
+0001e6d0: 7073 4164 6472 6573 7354 696d 6574 6162  psAddressTimetab
+0001e6e0: 6c65 2c20 4772 6f75 7073 4164 6472 6573  le, GroupsAddres
+0001e6f0: 7354 696d 6574 6162 6c65 4461 792c 2047  sTimetableDay, G
+0001e700: 726f 7570 7341 6464 7265 7373 576f 726b  roupsAddressWork
+0001e710: 496e 666f 5374 6174 7573 2c0a 2020 2020  InfoStatus,.    
+0001e720: 2020 2020 2020 4772 6f75 7073 4164 6472        GroupsAddr
+0001e730: 6573 7365 7349 6e66 6f2c 2047 726f 7570  essesInfo, Group
+0001e740: 7342 616e 496e 666f 2c20 4772 6f75 7073  sBanInfo, Groups
+0001e750: 4261 6e49 6e66 6f52 6561 736f 6e2c 2047  BanInfoReason, G
+0001e760: 726f 7570 7342 616e 6e65 6449 7465 6d2c  roupsBannedItem,
+0001e770: 2047 726f 7570 7343 616c 6c62 6163 6b53   GroupsCallbackS
+0001e780: 6572 7665 722c 2047 726f 7570 7343 616c  erver, GroupsCal
+0001e790: 6c62 6163 6b53 6574 7469 6e67 732c 2047  lbackSettings, G
+0001e7a0: 726f 7570 7343 6f6e 7461 6374 7349 7465  roupsContactsIte
+0001e7b0: 6d2c 0a20 2020 2020 2020 2020 2047 726f  m,.          Gro
+0001e7c0: 7570 7343 6f75 6e74 6572 7347 726f 7570  upsCountersGroup
+0001e7d0: 2c20 4772 6f75 7073 436f 7665 722c 2047  , GroupsCover, G
+0001e7e0: 726f 7570 7346 6965 6c64 732c 2047 726f  roupsFields, Gro
+0001e7f0: 7570 7346 696c 7465 722c 2047 726f 7570  upsFilter, Group
+0001e800: 7347 726f 7570 2c20 4772 6f75 7073 4772  sGroup, GroupsGr
+0001e810: 6f75 7041 6363 6573 732c 2047 726f 7570  oupAccess, Group
+0001e820: 7347 726f 7570 4164 6d69 6e4c 6576 656c  sGroupAdminLevel
+0001e830: 2c20 4772 6f75 7073 4772 6f75 7041 6765  , GroupsGroupAge
+0001e840: 4c69 6d69 7473 2c0a 2020 2020 2020 2020  Limits,.        
+0001e850: 2020 4772 6f75 7073 4772 6f75 7041 7474    GroupsGroupAtt
+0001e860: 6163 682c 2047 726f 7570 7347 726f 7570  ach, GroupsGroup
+0001e870: 4175 6469 6f2c 2047 726f 7570 7347 726f  Audio, GroupsGro
+0001e880: 7570 4261 6e49 6e66 6f2c 2047 726f 7570  upBanInfo, Group
+0001e890: 7347 726f 7570 4361 7465 676f 7279 2c20  sGroupCategory, 
+0001e8a0: 4772 6f75 7073 4772 6f75 7043 6174 6567  GroupsGroupCateg
+0001e8b0: 6f72 7946 756c 6c2c 2047 726f 7570 7347  oryFull, GroupsG
+0001e8c0: 726f 7570 4361 7465 676f 7279 5479 7065  roupCategoryType
+0001e8d0: 2c0a 2020 2020 2020 2020 2020 4772 6f75  ,.          Grou
+0001e8e0: 7073 4772 6f75 7044 6f63 732c 2047 726f  psGroupDocs, Gro
+0001e8f0: 7570 7347 726f 7570 4675 6c6c 2c20 4772  upsGroupFull, Gr
+0001e900: 6f75 7073 4772 6f75 7046 756c 6c41 6765  oupsGroupFullAge
+0001e910: 4c69 6d69 7473 2c20 4772 6f75 7073 4772  Limits, GroupsGr
+0001e920: 6f75 7046 756c 6c4d 656d 6265 7253 7461  oupFullMemberSta
+0001e930: 7475 732c 2047 726f 7570 7347 726f 7570  tus, GroupsGroup
+0001e940: 4675 6c6c 5365 6374 696f 6e2c 2047 726f  FullSection, Gro
+0001e950: 7570 7347 726f 7570 4973 436c 6f73 6564  upsGroupIsClosed
+0001e960: 2c0a 2020 2020 2020 2020 2020 4772 6f75  ,.          Grou
+0001e970: 7073 4772 6f75 704d 6172 6b65 7443 7572  psGroupMarketCur
+0001e980: 7265 6e63 792c 2047 726f 7570 7347 726f  rency, GroupsGro
+0001e990: 7570 5068 6f74 6f73 2c20 4772 6f75 7073  upPhotos, Groups
+0001e9a0: 4772 6f75 7050 7562 6c69 6343 6174 6567  GroupPublicCateg
+0001e9b0: 6f72 794c 6973 742c 2047 726f 7570 7347  oryList, GroupsG
+0001e9c0: 726f 7570 526f 6c65 2c20 4772 6f75 7073  roupRole, Groups
+0001e9d0: 4772 6f75 7053 7562 6a65 6374 2c0a 2020  GroupSubject,.  
+0001e9e0: 2020 2020 2020 2020 4772 6f75 7073 4772          GroupsGr
+0001e9f0: 6f75 7053 7567 6765 7374 6564 5072 6976  oupSuggestedPriv
+0001ea00: 6163 792c 2047 726f 7570 7347 726f 7570  acy, GroupsGroup
+0001ea10: 5461 672c 2047 726f 7570 7347 726f 7570  Tag, GroupsGroup
+0001ea20: 546f 7069 6373 2c20 4772 6f75 7073 4772  Topics, GroupsGr
+0001ea30: 6f75 7054 7970 652c 2047 726f 7570 7347  oupType, GroupsG
+0001ea40: 726f 7570 5669 6465 6f2c 2047 726f 7570  roupVideo, Group
+0001ea50: 7347 726f 7570 5761 6c6c 2c20 4772 6f75  sGroupWall, Grou
+0001ea60: 7073 4772 6f75 7057 696b 692c 0a20 2020  psGroupWiki,.   
+0001ea70: 2020 2020 2020 2047 726f 7570 7347 726f         GroupsGro
+0001ea80: 7570 7341 7272 6179 2c20 4772 6f75 7073  upsArray, Groups
+0001ea90: 4c69 6e6b 7349 7465 6d2c 2047 726f 7570  LinksItem, Group
+0001eaa0: 734c 6976 6543 6f76 6572 732c 2047 726f  sLiveCovers, Gro
+0001eab0: 7570 734c 6f6e 6750 6f6c 6c45 7665 6e74  upsLongPollEvent
+0001eac0: 732c 2047 726f 7570 734c 6f6e 6750 6f6c  s, GroupsLongPol
+0001ead0: 6c53 6572 7665 722c 2047 726f 7570 734c  lServer, GroupsL
+0001eae0: 6f6e 6750 6f6c 6c53 6574 7469 6e67 732c  ongPollSettings,
+0001eaf0: 2047 726f 7570 734d 6172 6b65 7449 6e66   GroupsMarketInf
+0001eb00: 6f2c 0a20 2020 2020 2020 2020 2047 726f  o,.          Gro
+0001eb10: 7570 734d 6172 6b65 7453 7461 7465 2c20  upsMarketState, 
+0001eb20: 4772 6f75 7073 4d65 6d62 6572 526f 6c65  GroupsMemberRole
+0001eb30: 2c20 4772 6f75 7073 4d65 6d62 6572 526f  , GroupsMemberRo
+0001eb40: 6c65 5065 726d 6973 7369 6f6e 2c20 4772  lePermission, Gr
+0001eb50: 6f75 7073 4d65 6d62 6572 526f 6c65 5374  oupsMemberRoleSt
+0001eb60: 6174 7573 2c20 4772 6f75 7073 4d65 6d62  atus, GroupsMemb
+0001eb70: 6572 5374 6174 7573 2c20 4772 6f75 7073  erStatus, Groups
+0001eb80: 4d65 6d62 6572 5374 6174 7573 4675 6c6c  MemberStatusFull
+0001eb90: 2c0a 2020 2020 2020 2020 2020 4772 6f75  ,.          Grou
+0001eba0: 7073 4f6e 6c69 6e65 5374 6174 7573 2c20  psOnlineStatus, 
+0001ebb0: 4772 6f75 7073 4f6e 6c69 6e65 5374 6174  GroupsOnlineStat
+0001ebc0: 7573 5479 7065 2c20 4772 6f75 7073 4f77  usType, GroupsOw
+0001ebd0: 6e65 7258 7472 4261 6e49 6e66 6f2c 2047  nerXtrBanInfo, G
+0001ebe0: 726f 7570 734f 776e 6572 5874 7242 616e  roupsOwnerXtrBan
+0001ebf0: 496e 666f 5479 7065 2c20 4772 6f75 7073  InfoType, Groups
+0001ec00: 5068 6f74 6f53 697a 652c 2047 726f 7570  PhotoSize, Group
+0001ec10: 7352 6f6c 654f 7074 696f 6e73 2c0a 2020  sRoleOptions,.  
+0001ec20: 2020 2020 2020 2020 4772 6f75 7073 5365          GroupsSe
+0001ec30: 6374 696f 6e73 4c69 7374 4974 656d 2c20  ctionsListItem, 
+0001ec40: 4772 6f75 7073 5365 7474 696e 6773 5477  GroupsSettingsTw
+0001ec50: 6974 7465 722c 2047 726f 7570 7353 7562  itter, GroupsSub
+0001ec60: 6a65 6374 4974 656d 2c20 4772 6f75 7073  jectItem, Groups
+0001ec70: 546f 6b65 6e50 6572 6d69 7373 696f 6e53  TokenPermissionS
+0001ec80: 6574 7469 6e67 2c20 4772 6f75 7073 5573  etting, GroupsUs
+0001ec90: 6572 5874 7252 6f6c 652c 204c 6561 6446  erXtrRole, LeadF
+0001eca0: 6f72 6d73 416e 7377 6572 2c0a 2020 2020  ormsAnswer,.    
+0001ecb0: 2020 2020 2020 4c65 6164 466f 726d 7341        LeadFormsA
+0001ecc0: 6e73 7765 7249 7465 6d2c 204c 6561 6446  nswerItem, LeadF
+0001ecd0: 6f72 6d73 466f 726d 2c20 4c65 6164 466f  ormsForm, LeadFo
+0001ece0: 726d 734c 6561 642c 204c 6561 6446 6f72  rmsLead, LeadFor
+0001ecf0: 6d73 5175 6573 7469 6f6e 4974 656d 2c20  msQuestionItem, 
+0001ed00: 4c65 6164 466f 726d 7351 7565 7374 696f  LeadFormsQuestio
+0001ed10: 6e49 7465 6d4f 7074 696f 6e2c 204c 696b  nItemOption, Lik
+0001ed20: 6573 5479 7065 2c20 4c69 6e6b 5461 7267  esType, LinkTarg
+0001ed30: 6574 4f62 6a65 6374 2c0a 2020 2020 2020  etObject,.      
+0001ed40: 2020 2020 4d61 726b 6574 4375 7272 656e      MarketCurren
+0001ed50: 6379 2c20 4d61 726b 6574 4d61 726b 6574  cy, MarketMarket
+0001ed60: 416c 6275 6d2c 204d 6172 6b65 744d 6172  Album, MarketMar
+0001ed70: 6b65 7443 6174 6567 6f72 792c 204d 6172  ketCategory, Mar
+0001ed80: 6b65 744d 6172 6b65 7443 6174 6567 6f72  ketMarketCategor
+0001ed90: 794e 6573 7465 642c 204d 6172 6b65 744d  yNested, MarketM
+0001eda0: 6172 6b65 7443 6174 6567 6f72 794f 6c64  arketCategoryOld
+0001edb0: 2c20 4d61 726b 6574 4d61 726b 6574 4361  , MarketMarketCa
+0001edc0: 7465 676f 7279 5472 6565 2c0a 2020 2020  tegoryTree,.    
+0001edd0: 2020 2020 2020 4d61 726b 6574 4d61 726b        MarketMark
+0001ede0: 6574 4974 656d 2c20 4d61 726b 6574 4d61  etItem, MarketMa
+0001edf0: 726b 6574 4974 656d 4176 6169 6c61 6269  rketItemAvailabi
+0001ee00: 6c69 7479 2c20 4d61 726b 6574 4d61 726b  lity, MarketMark
+0001ee10: 6574 4974 656d 4675 6c6c 2c20 4d61 726b  etItemFull, Mark
+0001ee20: 6574 4f72 6465 722c 204d 6172 6b65 744f  etOrder, MarketO
+0001ee30: 7264 6572 4974 656d 2c20 4d61 726b 6574  rderItem, Market
+0001ee40: 5072 6963 652c 204d 6172 6b65 7453 6563  Price, MarketSec
+0001ee50: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0001ee60: 4d61 726b 6574 5365 7276 6963 6573 5669  MarketServicesVi
+0001ee70: 6577 5479 7065 2c20 4d65 7373 6167 6573  ewType, Messages
+0001ee80: 4175 6469 6f4d 6573 7361 6765 2c20 4d65  AudioMessage, Me
+0001ee90: 7373 6167 6573 4368 6174 2c20 4d65 7373  ssagesChat, Mess
+0001eea0: 6167 6573 4368 6174 4675 6c6c 2c20 4d65  agesChatFull, Me
+0001eeb0: 7373 6167 6573 4368 6174 5072 6576 6965  ssagesChatPrevie
+0001eec0: 772c 204d 6573 7361 6765 7343 6861 7450  w, MessagesChatP
+0001eed0: 7573 6853 6574 7469 6e67 732c 0a20 2020  ushSettings,.   
+0001eee0: 2020 2020 2020 204d 6573 7361 6765 7343         MessagesC
+0001eef0: 6861 7452 6573 7472 6963 7469 6f6e 732c  hatRestrictions,
+0001ef00: 204d 6573 7361 6765 7343 6861 7453 6574   MessagesChatSet
+0001ef10: 7469 6e67 732c 204d 6573 7361 6765 7343  tings, MessagesC
+0001ef20: 6861 7453 6574 7469 6e67 7341 636c 2c20  hatSettingsAcl, 
+0001ef30: 4d65 7373 6167 6573 4368 6174 5365 7474  MessagesChatSett
+0001ef40: 696e 6773 5065 726d 6973 7369 6f6e 732c  ingsPermissions,
+0001ef50: 204d 6573 7361 6765 7343 6861 7453 6574   MessagesChatSet
+0001ef60: 7469 6e67 7350 686f 746f 2c0a 2020 2020  tingsPhoto,.    
+0001ef70: 2020 2020 2020 4d65 7373 6167 6573 4368        MessagesCh
+0001ef80: 6174 5365 7474 696e 6773 5374 6174 652c  atSettingsState,
+0001ef90: 204d 6573 7361 6765 7343 6f6e 7665 7273   MessagesConvers
+0001efa0: 6174 696f 6e2c 204d 6573 7361 6765 7343  ation, MessagesC
+0001efb0: 6f6e 7665 7273 6174 696f 6e43 616e 5772  onversationCanWr
+0001efc0: 6974 652c 204d 6573 7361 6765 7343 6f6e  ite, MessagesCon
+0001efd0: 7665 7273 6174 696f 6e4d 656d 6265 722c  versationMember,
+0001efe0: 204d 6573 7361 6765 7343 6f6e 7665 7273   MessagesConvers
+0001eff0: 6174 696f 6e50 6565 722c 0a20 2020 2020  ationPeer,.     
+0001f000: 2020 2020 204d 6573 7361 6765 7343 6f6e       MessagesCon
+0001f010: 7665 7273 6174 696f 6e50 6565 7254 7970  versationPeerTyp
+0001f020: 652c 204d 6573 7361 6765 7343 6f6e 7665  e, MessagesConve
+0001f030: 7273 6174 696f 6e53 6f72 7449 642c 204d  rsationSortId, M
+0001f040: 6573 7361 6765 7343 6f6e 7665 7273 6174  essagesConversat
+0001f050: 696f 6e57 6974 684d 6573 7361 6765 2c20  ionWithMessage, 
+0001f060: 4d65 7373 6167 6573 466f 7265 6967 6e4d  MessagesForeignM
+0001f070: 6573 7361 6765 2c20 4d65 7373 6167 6573  essage, Messages
+0001f080: 466f 7277 6172 642c 0a20 2020 2020 2020  Forward,.       
+0001f090: 2020 204d 6573 7361 6765 7347 6574 436f     MessagesGetCo
+0001f0a0: 6e76 6572 7361 7469 6f6e 4279 4964 2c20  nversationById, 
+0001f0b0: 4d65 7373 6167 6573 4765 7443 6f6e 7665  MessagesGetConve
+0001f0c0: 7273 6174 696f 6e42 7949 6445 7874 656e  rsationByIdExten
+0001f0d0: 6465 642c 204d 6573 7361 6765 7347 6574  ded, MessagesGet
+0001f0e0: 436f 6e76 6572 7361 7469 6f6e 4d65 6d62  ConversationMemb
+0001f0f0: 6572 732c 204d 6573 7361 6765 7347 7261  ers, MessagesGra
+0001f100: 6666 6974 692c 0a20 2020 2020 2020 2020  ffiti,.         
+0001f110: 204d 6573 7361 6765 7348 6973 746f 7279   MessagesHistory
+0001f120: 4174 7461 6368 6d65 6e74 2c20 4d65 7373  Attachment, Mess
+0001f130: 6167 6573 4869 7374 6f72 794d 6573 7361  agesHistoryMessa
+0001f140: 6765 4174 7461 6368 6d65 6e74 2c20 4d65  geAttachment, Me
+0001f150: 7373 6167 6573 4869 7374 6f72 794d 6573  ssagesHistoryMes
+0001f160: 7361 6765 4174 7461 6368 6d65 6e74 5479  sageAttachmentTy
+0001f170: 7065 2c20 4d65 7373 6167 6573 4b65 7962  pe, MessagesKeyb
+0001f180: 6f61 7264 2c20 4d65 7373 6167 6573 4b65  oard, MessagesKe
+0001f190: 7962 6f61 7264 4275 7474 6f6e 2c0a 4d65  yboardButton,.Me
+0001f1a0: 7373 6167 6573 4b65 7962 6f61 7264 4275  ssagesKeyboardBu
+0001f1b0: 7474 6f6e 4163 7469 6f6e 4361 6c6c 6261  ttonActionCallba
+0001f1c0: 636b 2c20 4d65 7373 6167 6573 4b65 7962  ck, MessagesKeyb
+0001f1d0: 6f61 7264 4275 7474 6f6e 4163 7469 6f6e  oardButtonAction
+0001f1e0: 4c6f 6361 7469 6f6e 2c20 4d65 7373 6167  Location, Messag
+0001f1f0: 6573 4b65 7962 6f61 7264 4275 7474 6f6e  esKeyboardButton
+0001f200: 4163 7469 6f6e 4f70 656e 4170 702c 204d  ActionOpenApp, M
+0001f210: 6573 7361 6765 734b 6579 626f 6172 6442  essagesKeyboardB
+0001f220: 7574 746f 6e41 6374 696f 6e4f 7065 6e4c  uttonActionOpenL
+0001f230: 696e 6b2c 0a4d 6573 7361 6765 734b 6579  ink,.MessagesKey
+0001f240: 626f 6172 6442 7574 746f 6e41 6374 696f  boardButtonActio
+0001f250: 6e4f 7065 6e50 686f 746f 2c20 4d65 7373  nOpenPhoto, Mess
+0001f260: 6167 6573 4b65 7962 6f61 7264 4275 7474  agesKeyboardButt
+0001f270: 6f6e 4163 7469 6f6e 5465 7874 2c20 4d65  onActionText, Me
+0001f280: 7373 6167 6573 4b65 7962 6f61 7264 4275  ssagesKeyboardBu
+0001f290: 7474 6f6e 4163 7469 6f6e 566b 7061 792c  ttonActionVkpay,
+0001f2a0: 204d 6573 7361 6765 734b 6579 626f 6172   MessagesKeyboar
+0001f2b0: 6442 7574 746f 6e50 726f 7065 7274 7941  dButtonPropertyA
+0001f2c0: 6374 696f 6e2c 0a4d 6573 7361 6765 734c  ction,.MessagesL
+0001f2d0: 6173 7441 6374 6976 6974 792c 204d 6573  astActivity, Mes
+0001f2e0: 7361 6765 734c 6f6e 6770 6f6c 6c4d 6573  sagesLongpollMes
+0001f2f0: 7361 6765 732c 204d 6573 7361 6765 734c  sages, MessagesL
+0001f300: 6f6e 6770 6f6c 6c50 6172 616d 732c 204d  ongpollParams, M
+0001f310: 6573 7361 6765 734d 6573 7361 6765 2c20  essagesMessage, 
+0001f320: 4d65 7373 6167 6573 4d65 7373 6167 6541  MessagesMessageA
+0001f330: 6374 696f 6e2c 204d 6573 7361 6765 734d  ction, MessagesM
+0001f340: 6573 7361 6765 4163 7469 6f6e 5068 6f74  essageActionPhot
+0001f350: 6f2c 0a4d 6573 7361 6765 734d 6573 7361  o,.MessagesMessa
+0001f360: 6765 4163 7469 6f6e 5374 6174 7573 2c20  geActionStatus, 
+0001f370: 4d65 7373 6167 6573 4d65 7373 6167 6541  MessagesMessageA
+0001f380: 7474 6163 686d 656e 742c 204d 6573 7361  ttachment, Messa
+0001f390: 6765 734d 6573 7361 6765 4174 7461 6368  gesMessageAttach
+0001f3a0: 6d65 6e74 5479 7065 2c20 4d65 7373 6167  mentType, Messag
+0001f3b0: 6573 4d65 7373 6167 6552 6571 7565 7374  esMessageRequest
+0001f3c0: 4461 7461 2c20 4d65 7373 6167 6573 4d65  Data, MessagesMe
+0001f3d0: 7373 6167 6573 4172 7261 792c 0a4d 6573  ssagesArray,.Mes
+0001f3e0: 7361 6765 734f 7574 5265 6164 4279 2c20  sagesOutReadBy, 
+0001f3f0: 4d65 7373 6167 6573 5069 6e6e 6564 4d65  MessagesPinnedMe
+0001f400: 7373 6167 652c 204d 6573 7361 6765 7350  ssage, MessagesP
+0001f410: 7573 6853 6574 7469 6e67 732c 204d 6573  ushSettings, Mes
+0001f420: 7361 6765 7353 656e 6455 7365 7249 6473  sagesSendUserIds
+0001f430: 5265 7370 6f6e 7365 4974 656d 2c20 4d65  ResponseItem, Me
+0001f440: 7373 6167 6573 5465 6d70 6c61 7465 4163  ssagesTemplateAc
+0001f450: 7469 6f6e 5479 7065 4e61 6d65 732c 0a4d  tionTypeNames,.M
+0001f460: 6573 7361 6765 7355 7365 7258 7472 496e  essagesUserXtrIn
+0001f470: 7669 7465 6442 792c 204e 6577 7366 6565  vitedBy, Newsfee
+0001f480: 6443 6f6d 6d65 6e74 7346 696c 7465 7273  dCommentsFilters
+0001f490: 2c20 4e65 7773 6665 6564 4967 6e6f 7265  , NewsfeedIgnore
+0001f4a0: 4974 656d 5479 7065 2c20 4e65 7773 6665  ItemType, Newsfe
+0001f4b0: 6564 4974 656d 4175 6469 6f2c 204e 6577  edItemAudio, New
+0001f4c0: 7366 6565 6449 7465 6d41 7564 696f 4175  sfeedItemAudioAu
+0001f4d0: 6469 6f2c 204e 6577 7366 6565 6449 7465  dio, NewsfeedIte
+0001f4e0: 6d42 6173 652c 0a4e 6577 7366 6565 6449  mBase,.NewsfeedI
+0001f4f0: 7465 6d44 6967 6573 742c 204e 6577 7366  temDigest, Newsf
+0001f500: 6565 6449 7465 6d44 6967 6573 7442 7574  eedItemDigestBut
+0001f510: 746f 6e2c 204e 6577 7366 6565 6449 7465  ton, NewsfeedIte
+0001f520: 6d44 6967 6573 7446 6f6f 7465 722c 204e  mDigestFooter, N
+0001f530: 6577 7366 6565 6449 7465 6d44 6967 6573  ewsfeedItemDiges
+0001f540: 7446 756c 6c49 7465 6d2c 204e 6577 7366  tFullItem, Newsf
+0001f550: 6565 6449 7465 6d44 6967 6573 7448 6561  eedItemDigestHea
+0001f560: 6465 722c 204e 6577 7366 6565 6449 7465  der, NewsfeedIte
+0001f570: 6d44 6967 6573 7449 7465 6d2c 0a4e 6577  mDigestItem,.New
+0001f580: 7366 6565 6449 7465 6d46 7269 656e 642c  sfeedItemFriend,
+0001f590: 204e 6577 7366 6565 6449 7465 6d46 7269   NewsfeedItemFri
+0001f5a0: 656e 6446 7269 656e 6473 2c20 4e65 7773  endFriends, News
+0001f5b0: 6665 6564 4974 656d 486f 6c69 6461 7952  feedItemHolidayR
+0001f5c0: 6563 6f6d 6d65 6e64 6174 696f 6e73 426c  ecommendationsBl
+0001f5d0: 6f63 6b48 6561 6465 722c 204e 6577 7366  ockHeader, Newsf
+0001f5e0: 6565 6449 7465 6d50 686f 746f 2c20 4e65  eedItemPhoto, Ne
+0001f5f0: 7773 6665 6564 4974 656d 5068 6f74 6f50  wsfeedItemPhotoP
+0001f600: 686f 746f 732c 0a4e 6577 7366 6565 6449  hotos,.NewsfeedI
+0001f610: 7465 6d50 686f 746f 5461 672c 204e 6577  temPhotoTag, New
+0001f620: 7366 6565 6449 7465 6d50 686f 746f 5461  sfeedItemPhotoTa
+0001f630: 6750 686f 746f 5461 6773 2c20 4e65 7773  gPhotoTags, News
+0001f640: 6665 6564 4974 656d 5072 6f6d 6f42 7574  feedItemPromoBut
+0001f650: 746f 6e2c 204e 6577 7366 6565 6449 7465  ton, NewsfeedIte
+0001f660: 6d50 726f 6d6f 4275 7474 6f6e 4163 7469  mPromoButtonActi
+0001f670: 6f6e 2c20 4e65 7773 6665 6564 4974 656d  on, NewsfeedItem
+0001f680: 5072 6f6d 6f42 7574 746f 6e49 6d61 6765  PromoButtonImage
+0001f690: 2c0a 4e65 7773 6665 6564 4974 656d 546f  ,.NewsfeedItemTo
+0001f6a0: 7069 632c 204e 6577 7366 6565 6449 7465  pic, NewsfeedIte
+0001f6b0: 6d56 6964 656f 2c20 4e65 7773 6665 6564  mVideo, Newsfeed
+0001f6c0: 4974 656d 5669 6465 6f56 6964 656f 2c20  ItemVideoVideo, 
+0001f6d0: 4e65 7773 6665 6564 4974 656d 5761 6c6c  NewsfeedItemWall
+0001f6e0: 706f 7374 2c20 4e65 7773 6665 6564 4974  post, NewsfeedIt
+0001f6f0: 656d 5761 6c6c 706f 7374 4665 6564 6261  emWallpostFeedba
+0001f700: 636b 2c20 4e65 7773 6665 6564 4974 656d  ck, NewsfeedItem
+0001f710: 5761 6c6c 706f 7374 4665 6564 6261 636b  WallpostFeedback
+0001f720: 416e 7377 6572 2c0a 4e65 7773 6665 6564  Answer,.Newsfeed
+0001f730: 4974 656d 5761 6c6c 706f 7374 4665 6564  ItemWallpostFeed
+0001f740: 6261 636b 5479 7065 2c20 4e65 7773 6665  backType, Newsfe
+0001f750: 6564 4c69 7374 2c20 4e65 7773 6665 6564  edList, Newsfeed
+0001f760: 4c69 7374 4675 6c6c 2c20 4e65 7773 6665  ListFull, Newsfe
+0001f770: 6564 4e65 7773 6665 6564 4974 656d 2c20  edNewsfeedItem, 
 0001f780: 4e65 7773 6665 6564 4e65 7773 6665 6564  NewsfeedNewsfeed
-0001f790: 5068 6f74 6f2c 204e 6f74 6573 4e6f 7465  Photo, NotesNote
-0001f7a0: 2c0a 4e6f 7465 734e 6f74 6543 6f6d 6d65  ,.NotesNoteComme
-0001f7b0: 6e74 2c20 4e6f 7469 6669 6361 7469 6f6e  nt, Notification
-0001f7c0: 7346 6565 6462 6163 6b2c 204e 6f74 6966  sFeedback, Notif
-0001f7d0: 6963 6174 696f 6e73 4e6f 7469 6669 6361  icationsNotifica
-0001f7e0: 7469 6f6e 2c20 4e6f 7469 6669 6361 7469  tion, Notificati
-0001f7f0: 6f6e 734e 6f74 6966 6963 6174 696f 6e49  onsNotificationI
-0001f800: 7465 6d2c 204e 6f74 6966 6963 6174 696f  tem, Notificatio
-0001f810: 6e73 4e6f 7469 6669 6361 7469 6f6e 5061  nsNotificationPa
-0001f820: 7265 6e74 2c0a 4e6f 7469 6669 6361 7469  rent,.Notificati
-0001f830: 6f6e 734e 6f74 6966 6963 6174 696f 6e73  onsNotifications
-0001f840: 436f 6d6d 656e 742c 204e 6f74 6966 6963  Comment, Notific
-0001f850: 6174 696f 6e73 5265 706c 792c 204e 6f74  ationsReply, Not
-0001f860: 6966 6963 6174 696f 6e73 5365 6e64 4d65  ificationsSendMe
-0001f870: 7373 6167 6545 7272 6f72 2c20 4e6f 7469  ssageError, Noti
-0001f880: 6669 6361 7469 6f6e 7353 656e 644d 6573  ficationsSendMes
-0001f890: 7361 6765 4974 656d 2c20 4f61 7574 6845  sageItem, OauthE
-0001f8a0: 7272 6f72 2c20 4f72 6465 7273 416d 6f75  rror, OrdersAmou
-0001f8b0: 6e74 2c0a 4f72 6465 7273 416d 6f75 6e74  nt,.OrdersAmount
-0001f8c0: 4974 656d 2c20 4f72 6465 7273 4f72 6465  Item, OrdersOrde
-0001f8d0: 722c 204f 7264 6572 7353 7562 7363 7269  r, OrdersSubscri
-0001f8e0: 7074 696f 6e2c 204f 776e 6572 5374 6174  ption, OwnerStat
-0001f8f0: 652c 2050 6167 6573 5072 6976 6163 7953  e, PagesPrivacyS
-0001f900: 6574 7469 6e67 732c 2050 6167 6573 5769  ettings, PagesWi
-0001f910: 6b69 7061 6765 2c20 5061 6765 7357 696b  kipage, PagesWik
-0001f920: 6970 6167 6546 756c 6c2c 2050 6167 6573  ipageFull, Pages
-0001f930: 5769 6b69 7061 6765 4869 7374 6f72 792c  WikipageHistory,
-0001f940: 0a50 686f 746f 7349 6d61 6765 2c20 5068  .PhotosImage, Ph
-0001f950: 6f74 6f73 496d 6167 6554 7970 652c 2050  otosImageType, P
-0001f960: 686f 746f 7350 686f 746f 2c20 5068 6f74  hotosPhoto, Phot
-0001f970: 6f73 5068 6f74 6f41 6c62 756d 2c20 5068  osPhotoAlbum, Ph
-0001f980: 6f74 6f73 5068 6f74 6f41 6c62 756d 4675  otosPhotoAlbumFu
-0001f990: 6c6c 2c20 5068 6f74 6f73 5068 6f74 6f46  ll, PhotosPhotoF
-0001f9a0: 616c 7365 6162 6c65 2c20 5068 6f74 6f73  alseable, Photos
-0001f9b0: 5068 6f74 6f46 756c 6c58 7472 5265 616c  PhotoFullXtrReal
-0001f9c0: 4f66 6673 6574 2c0a 5068 6f74 6f73 5068  Offset,.PhotosPh
-0001f9d0: 6f74 6f53 697a 6573 2c20 5068 6f74 6f73  otoSizes, Photos
-0001f9e0: 5068 6f74 6f53 697a 6573 5479 7065 2c20  PhotoSizesType, 
-0001f9f0: 5068 6f74 6f73 5068 6f74 6f54 6167 2c20  PhotosPhotoTag, 
-0001fa00: 5068 6f74 6f73 5068 6f74 6f55 706c 6f61  PhotosPhotoUploa
-0001fa10: 642c 2050 686f 746f 7350 686f 746f 5874  d, PhotosPhotoXt
-0001fa20: 7252 6561 6c4f 6666 7365 742c 2050 686f  rRealOffset, Pho
-0001fa30: 746f 7350 686f 746f 5874 7254 6167 496e  tosPhotoXtrTagIn
-0001fa40: 666f 2c20 5068 6f74 6f73 5461 6773 5375  fo, PhotosTagsSu
-0001fa50: 6767 6573 7469 6f6e 4974 656d 2c0a 5068  ggestionItem,.Ph
+0001f790: 4974 656d 5479 7065 2c20 4e65 7773 6665  ItemType, Newsfe
+0001f7a0: 6564 4e65 7773 6665 6564 5068 6f74 6f2c  edNewsfeedPhoto,
+0001f7b0: 204e 6f74 6573 4e6f 7465 2c0a 4e6f 7465   NotesNote,.Note
+0001f7c0: 734e 6f74 6543 6f6d 6d65 6e74 2c20 4e6f  sNoteComment, No
+0001f7d0: 7469 6669 6361 7469 6f6e 7346 6565 6462  tificationsFeedb
+0001f7e0: 6163 6b2c 204e 6f74 6966 6963 6174 696f  ack, Notificatio
+0001f7f0: 6e73 4e6f 7469 6669 6361 7469 6f6e 2c20  nsNotification, 
+0001f800: 4e6f 7469 6669 6361 7469 6f6e 734e 6f74  NotificationsNot
+0001f810: 6966 6963 6174 696f 6e49 7465 6d2c 204e  ificationItem, N
+0001f820: 6f74 6966 6963 6174 696f 6e73 4e6f 7469  otificationsNoti
+0001f830: 6669 6361 7469 6f6e 5061 7265 6e74 2c0a  ficationParent,.
+0001f840: 4e6f 7469 6669 6361 7469 6f6e 734e 6f74  NotificationsNot
+0001f850: 6966 6963 6174 696f 6e73 436f 6d6d 656e  ificationsCommen
+0001f860: 742c 204e 6f74 6966 6963 6174 696f 6e73  t, Notifications
+0001f870: 5265 706c 792c 204e 6f74 6966 6963 6174  Reply, Notificat
+0001f880: 696f 6e73 5365 6e64 4d65 7373 6167 6545  ionsSendMessageE
+0001f890: 7272 6f72 2c20 4e6f 7469 6669 6361 7469  rror, Notificati
+0001f8a0: 6f6e 7353 656e 644d 6573 7361 6765 4974  onsSendMessageIt
+0001f8b0: 656d 2c20 4f61 7574 6845 7272 6f72 2c20  em, OauthError, 
+0001f8c0: 4f72 6465 7273 416d 6f75 6e74 2c0a 4f72  OrdersAmount,.Or
+0001f8d0: 6465 7273 416d 6f75 6e74 4974 656d 2c20  dersAmountItem, 
+0001f8e0: 4f72 6465 7273 4f72 6465 722c 204f 7264  OrdersOrder, Ord
+0001f8f0: 6572 7353 7562 7363 7269 7074 696f 6e2c  ersSubscription,
+0001f900: 204f 776e 6572 5374 6174 652c 2050 6167   OwnerState, Pag
+0001f910: 6573 5072 6976 6163 7953 6574 7469 6e67  esPrivacySetting
+0001f920: 732c 2050 6167 6573 5769 6b69 7061 6765  s, PagesWikipage
+0001f930: 2c20 5061 6765 7357 696b 6970 6167 6546  , PagesWikipageF
+0001f940: 756c 6c2c 2050 6167 6573 5769 6b69 7061  ull, PagesWikipa
+0001f950: 6765 4869 7374 6f72 792c 0a50 686f 746f  geHistory,.Photo
+0001f960: 7349 6d61 6765 2c20 5068 6f74 6f73 496d  sImage, PhotosIm
+0001f970: 6167 6554 7970 652c 2050 686f 746f 7350  ageType, PhotosP
+0001f980: 686f 746f 2c20 5068 6f74 6f73 5068 6f74  hoto, PhotosPhot
+0001f990: 6f41 6c62 756d 2c20 5068 6f74 6f73 5068  oAlbum, PhotosPh
+0001f9a0: 6f74 6f41 6c62 756d 4675 6c6c 2c20 5068  otoAlbumFull, Ph
+0001f9b0: 6f74 6f73 5068 6f74 6f46 616c 7365 6162  otosPhotoFalseab
+0001f9c0: 6c65 2c20 5068 6f74 6f73 5068 6f74 6f46  le, PhotosPhotoF
+0001f9d0: 756c 6c58 7472 5265 616c 4f66 6673 6574  ullXtrRealOffset
+0001f9e0: 2c0a 5068 6f74 6f73 5068 6f74 6f53 697a  ,.PhotosPhotoSiz
+0001f9f0: 6573 2c20 5068 6f74 6f73 5068 6f74 6f53  es, PhotosPhotoS
+0001fa00: 697a 6573 5479 7065 2c20 5068 6f74 6f73  izesType, Photos
+0001fa10: 5068 6f74 6f54 6167 2c20 5068 6f74 6f73  PhotoTag, Photos
+0001fa20: 5068 6f74 6f55 706c 6f61 642c 2050 686f  PhotoUpload, Pho
+0001fa30: 746f 7350 686f 746f 5874 7252 6561 6c4f  tosPhotoXtrRealO
+0001fa40: 6666 7365 742c 2050 686f 746f 7350 686f  ffset, PhotosPho
+0001fa50: 746f 5874 7254 6167 496e 666f 2c20 5068  toXtrTagInfo, Ph
 0001fa60: 6f74 6f73 5461 6773 5375 6767 6573 7469  otosTagsSuggesti
-0001fa70: 6f6e 4974 656d 4275 7474 6f6e 2c20 506f  onItemButton, Po
-0001fa80: 6463 6173 7443 6f76 6572 2c20 506f 6463  dcastCover, Podc
-0001fa90: 6173 7445 7874 6572 6e61 6c44 6174 612c  astExternalData,
-0001faa0: 2050 6f6c 6c73 416e 7377 6572 2c20 506f   PollsAnswer, Po
-0001fab0: 6c6c 7342 6163 6b67 726f 756e 642c 2050  llsBackground, P
-0001fac0: 6f6c 6c73 4672 6965 6e64 2c20 506f 6c6c  ollsFriend, Poll
-0001fad0: 7350 6f6c 6c2c 2050 6f6c 6c73 506f 6c6c  sPoll, PollsPoll
-0001fae0: 416e 6f6e 796d 6f75 732c 0a50 6f6c 6c73  Anonymous,.Polls
-0001faf0: 566f 7465 7273 2c20 506f 6c6c 7356 6f74  Voters, PollsVot
-0001fb00: 6572 7355 7365 7273 2c20 5072 6574 7479  ersUsers, Pretty
-0001fb10: 4361 7264 7350 7265 7474 7943 6172 642c  CardsPrettyCard,
-0001fb20: 2050 7265 7474 7943 6172 6473 5072 6574   PrettyCardsPret
-0001fb30: 7479 4361 7264 4f72 4572 726f 722c 2053  tyCardOrError, S
-0001fb40: 6561 7263 6848 696e 742c 2053 6561 7263  earchHint, Searc
-0001fb50: 6848 696e 7453 6563 7469 6f6e 2c20 5365  hHintSection, Se
-0001fb60: 6172 6368 4869 6e74 5479 7065 2c0a 5365  archHintType,.Se
-0001fb70: 6375 7265 4769 7665 4576 656e 7453 7469  cureGiveEventSti
-0001fb80: 636b 6572 4974 656d 2c20 5365 6375 7265  ckerItem, Secure
-0001fb90: 4c65 7665 6c2c 2053 6563 7572 6553 6574  Level, SecureSet
-0001fba0: 436f 756e 7465 7249 7465 6d2c 2053 6563  CounterItem, Sec
-0001fbb0: 7572 6553 6d73 4e6f 7469 6669 6361 7469  ureSmsNotificati
-0001fbc0: 6f6e 2c20 5365 6375 7265 546f 6b65 6e43  on, SecureTokenC
-0001fbd0: 6865 636b 6564 2c20 5365 6375 7265 5472  hecked, SecureTr
-0001fbe0: 616e 7361 6374 696f 6e2c 2053 7461 7473  ansaction, Stats
-0001fbf0: 4163 7469 7669 7479 2c20 5374 6174 7343  Activity, StatsC
-0001fc00: 6974 792c 0a53 7461 7473 436f 756e 7472  ity,.StatsCountr
-0001fc10: 792c 2053 7461 7473 5065 7269 6f64 2c20  y, StatsPeriod, 
-0001fc20: 5374 6174 7352 6561 6368 2c20 5374 6174  StatsReach, Stat
-0001fc30: 7353 6578 4167 652c 2053 7461 7473 5669  sSexAge, StatsVi
-0001fc40: 6577 732c 2053 7461 7473 5761 6c6c 706f  ews, StatsWallpo
-0001fc50: 7374 5374 6174 2c20 5374 6174 7573 5374  stStat, StatusSt
-0001fc60: 6174 7573 2c20 5374 6963 6b65 7273 496d  atus, StickersIm
-0001fc70: 6167 6553 6574 2c20 5374 6f72 6167 6556  ageSet, StorageV
-0001fc80: 616c 7565 2c20 5374 6f72 6550 726f 6475  alue, StoreProdu
-0001fc90: 6374 2c0a 5374 6f72 6550 726f 6475 6374  ct,.StoreProduct
-0001fca0: 4963 6f6e 2c20 5374 6f72 6553 7469 636b  Icon, StoreStick
-0001fcb0: 6572 734b 6579 776f 7264 2c20 5374 6f72  ersKeyword, Stor
-0001fcc0: 6553 7469 636b 6572 734b 6579 776f 7264  eStickersKeyword
-0001fcd0: 5374 6963 6b65 722c 2053 746f 7265 5374  Sticker, StoreSt
-0001fce0: 6963 6b65 7273 4b65 7977 6f72 6453 7469  ickersKeywordSti
-0001fcf0: 636b 6572 732c 2053 746f 7269 6573 436c  ckers, StoriesCl
-0001fd00: 6963 6b61 626c 6541 7265 612c 2053 746f  ickableArea, Sto
-0001fd10: 7269 6573 436c 6963 6b61 626c 6553 7469  riesClickableSti
-0001fd20: 636b 6572 2c0a 5374 6f72 6965 7343 6c69  cker,.StoriesCli
-0001fd30: 636b 6162 6c65 5374 6963 6b65 7273 2c20  ckableStickers, 
-0001fd40: 5374 6f72 6965 7346 6565 6449 7465 6d2c  StoriesFeedItem,
-0001fd50: 2053 746f 7269 6573 5072 6f6d 6f42 6c6f   StoriesPromoBlo
-0001fd60: 636b 2c20 5374 6f72 6965 7352 6570 6c69  ck, StoriesRepli
-0001fd70: 6573 2c20 5374 6f72 6965 7353 7461 744c  es, StoriesStatL
-0001fd80: 696e 652c 2053 746f 7269 6573 5374 6f72  ine, StoriesStor
-0001fd90: 792c 2053 746f 7269 6573 5374 6f72 794c  y, StoriesStoryL
-0001fda0: 696e 6b2c 2053 746f 7269 6573 5374 6f72  ink, StoriesStor
-0001fdb0: 7953 7461 7473 2c0a 5374 6f72 6965 7353  yStats,.StoriesS
-0001fdc0: 746f 7279 5374 6174 7353 7461 742c 2053  toryStatsStat, S
-0001fdd0: 746f 7269 6573 5374 6f72 7953 7461 7473  toriesStoryStats
-0001fde0: 5374 6174 652c 2053 746f 7269 6573 5374  State, StoriesSt
-0001fdf0: 6f72 7954 7970 652c 2053 746f 7269 6573  oryType, Stories
-0001fe00: 5570 6c6f 6164 4c69 6e6b 5465 7874 2c20  UploadLinkText, 
-0001fe10: 5374 6f72 6965 7356 6965 7765 7273 4974  StoriesViewersIt
-0001fe20: 656d 2c20 5573 6572 7343 6172 6565 722c  em, UsersCareer,
-0001fe30: 2055 7365 7273 4578 706f 7274 732c 2055   UsersExports, U
-0001fe40: 7365 7273 4669 656c 6473 2c0a 5573 6572  sersFields,.User
-0001fe50: 734c 6173 7453 6565 6e2c 2055 7365 7273  sLastSeen, Users
-0001fe60: 4d69 6c69 7461 7279 2c20 5573 6572 734f  Military, UsersO
-0001fe70: 6363 7570 6174 696f 6e2c 2055 7365 7273  ccupation, Users
-0001fe80: 4f6e 6c69 6e65 496e 666f 2c20 5573 6572  OnlineInfo, User
-0001fe90: 7350 6572 736f 6e61 6c2c 2055 7365 7273  sPersonal, Users
-0001fea0: 5265 6c61 7469 7665 2c20 5573 6572 7353  Relative, UsersS
-0001feb0: 6368 6f6f 6c2c 2055 7365 7273 5375 6273  chool, UsersSubs
-0001fec0: 6372 6970 7469 6f6e 7349 7465 6d2c 2055  criptionsItem, U
-0001fed0: 7365 7273 556e 6976 6572 7369 7479 2c0a  sersUniversity,.
-0001fee0: 5573 6572 7355 7365 722c 2055 7365 7273  UsersUser, Users
-0001fef0: 5573 6572 436f 6e6e 6563 7469 6f6e 732c  UserConnections,
-0001ff00: 2055 7365 7273 5573 6572 436f 756e 7465   UsersUserCounte
-0001ff10: 7273 2c20 5573 6572 7355 7365 7246 756c  rs, UsersUserFul
-0001ff20: 6c2c 2055 7365 7273 5573 6572 4d69 6e2c  l, UsersUserMin,
-0001ff30: 2055 7365 7273 5573 6572 5265 6c61 7469   UsersUserRelati
-0001ff40: 6f6e 2c20 5573 6572 7355 7365 7253 6574  on, UsersUserSet
-0001ff50: 7469 6e67 7358 7472 2c20 5573 6572 7355  tingsXtr, UsersU
-0001ff60: 7365 7254 7970 652c 0a55 7365 7273 5573  serType,.UsersUs
-0001ff70: 6572 5874 7254 7970 652c 2055 7365 7273  erXtrType, Users
-0001ff80: 5573 6572 7341 7272 6179 2c20 5574 696c  UsersArray, Util
-0001ff90: 7344 6f6d 6169 6e52 6573 6f6c 7665 642c  sDomainResolved,
-0001ffa0: 2055 7469 6c73 446f 6d61 696e 5265 736f   UtilsDomainReso
-0001ffb0: 6c76 6564 5479 7065 2c20 5574 696c 734c  lvedType, UtilsL
-0001ffc0: 6173 7453 686f 7274 656e 6564 4c69 6e6b  astShortenedLink
-0001ffd0: 2c20 5574 696c 734c 696e 6b43 6865 636b  , UtilsLinkCheck
-0001ffe0: 6564 2c20 5574 696c 734c 696e 6b43 6865  ed, UtilsLinkChe
-0001fff0: 636b 6564 5374 6174 7573 2c0a 5574 696c  ckedStatus,.Util
-00020000: 734c 696e 6b53 7461 7473 2c20 5574 696c  sLinkStats, Util
-00020010: 734c 696e 6b53 7461 7473 4578 7465 6e64  sLinkStatsExtend
-00020020: 6564 2c20 5574 696c 7353 686f 7274 4c69  ed, UtilsShortLi
-00020030: 6e6b 2c20 5574 696c 7353 7461 7473 2c20  nk, UtilsStats, 
-00020040: 5574 696c 7353 7461 7473 4369 7479 2c20  UtilsStatsCity, 
-00020050: 5574 696c 7353 7461 7473 436f 756e 7472  UtilsStatsCountr
-00020060: 792c 2055 7469 6c73 5374 6174 7345 7874  y, UtilsStatsExt
-00020070: 656e 6465 642c 2055 7469 6c73 5374 6174  ended, UtilsStat
-00020080: 7353 6578 4167 652c 0a56 6964 656f 4c69  sSexAge,.VideoLi
-00020090: 7665 496e 666f 2c20 5669 6465 6f4c 6976  veInfo, VideoLiv
-000200a0: 6553 6574 7469 6e67 732c 2056 6964 656f  eSettings, Video
-000200b0: 5361 7665 5265 7375 6c74 2c20 5669 6465  SaveResult, Vide
-000200c0: 6f56 6964 656f 2c20 5669 6465 6f56 6964  oVideo, VideoVid
-000200d0: 656f 416c 6275 6d2c 2056 6964 656f 5669  eoAlbum, VideoVi
-000200e0: 6465 6f41 6c62 756d 4675 6c6c 2c20 5669  deoAlbumFull, Vi
-000200f0: 6465 6f56 6964 656f 4669 6c65 732c 2056  deoVideoFiles, V
-00020100: 6964 656f 5669 6465 6f46 756c 6c2c 2056  ideoVideoFull, V
-00020110: 6964 656f 5669 6465 6f49 6d61 6765 2c0a  ideoVideoImage,.
-00020120: 5761 6c6c 4170 7050 6f73 742c 2057 616c  WallAppPost, Wal
-00020130: 6c41 7474 6163 6865 644e 6f74 652c 2057  lAttachedNote, W
-00020140: 616c 6c43 6172 6f75 7365 6c42 6173 652c  allCarouselBase,
-00020150: 2057 616c 6c43 6f6d 6d65 6e74 4174 7461   WallCommentAtta
-00020160: 6368 6d65 6e74 2c20 5761 6c6c 436f 6d6d  chment, WallComm
-00020170: 656e 7441 7474 6163 686d 656e 7454 7970  entAttachmentTyp
-00020180: 652c 2057 616c 6c47 656f 2c20 5761 6c6c  e, WallGeo, Wall
-00020190: 4765 7446 696c 7465 722c 2057 616c 6c47  GetFilter, WallG
-000201a0: 7261 6666 6974 692c 0a57 616c 6c50 6f73  raffiti,.WallPos
-000201b0: 7443 6f70 7972 6967 6874 2c20 5761 6c6c  tCopyright, Wall
-000201c0: 506f 7374 536f 7572 6365 2c20 5761 6c6c  PostSource, Wall
-000201d0: 506f 7374 536f 7572 6365 5479 7065 2c20  PostSourceType, 
-000201e0: 5761 6c6c 506f 7374 5479 7065 2c20 5761  WallPostType, Wa
-000201f0: 6c6c 506f 7374 6564 5068 6f74 6f2c 2057  llPostedPhoto, W
-00020200: 616c 6c56 6965 7773 2c20 5761 6c6c 5761  allViews, WallWa
-00020210: 6c6c 436f 6d6d 656e 742c 2057 616c 6c57  llComment, WallW
-00020220: 616c 6c43 6f6d 6d65 6e74 446f 6e75 742c  allCommentDonut,
-00020230: 0a57 616c 6c57 616c 6c43 6f6d 6d65 6e74  .WallWallComment
-00020240: 446f 6e75 7450 6c61 6365 686f 6c64 6572  DonutPlaceholder
-00020250: 2c20 5761 6c6c 5761 6c6c 706f 7374 2c20  , WallWallpost, 
-00020260: 5761 6c6c 5761 6c6c 706f 7374 4174 7461  WallWallpostAtta
-00020270: 6368 6d65 6e74 2c20 5761 6c6c 5761 6c6c  chment, WallWall
-00020280: 706f 7374 4174 7461 6368 6d65 6e74 5479  postAttachmentTy
-00020290: 7065 2c20 5761 6c6c 5761 6c6c 706f 7374  pe, WallWallpost
-000202a0: 436f 6d6d 656e 7473 446f 6e75 742c 0a57  CommentsDonut,.W
-000202b0: 616c 6c57 616c 6c70 6f73 7443 6f6d 6d65  allWallpostComme
-000202c0: 6e74 7344 6f6e 7574 506c 6163 6568 6f6c  ntsDonutPlacehol
-000202d0: 6465 722c 2057 616c 6c57 616c 6c70 6f73  der, WallWallpos
-000202e0: 7444 6f6e 7574 2c20 5761 6c6c 5761 6c6c  tDonut, WallWall
-000202f0: 706f 7374 446f 6e75 7450 6c61 6365 686f  postDonutPlaceho
-00020300: 6c64 6572 2c20 5761 6c6c 5761 6c6c 706f  lder, WallWallpo
-00020310: 7374 4675 6c6c 2c20 5761 6c6c 5761 6c6c  stFull, WallWall
-00020320: 706f 7374 546f 4964 2c20 5769 6467 6574  postToId, Widget
-00020330: 7343 6f6d 6d65 6e74 4d65 6469 612c 0a57  sCommentMedia,.W
-00020340: 6964 6765 7473 436f 6d6d 656e 744d 6564  idgetsCommentMed
-00020350: 6961 5479 7065 2c20 5769 6467 6574 7343  iaType, WidgetsC
-00020360: 6f6d 6d65 6e74 5265 706c 6965 732c 2057  ommentReplies, W
-00020370: 6964 6765 7473 436f 6d6d 656e 7452 6570  idgetsCommentRep
-00020380: 6c69 6573 4974 656d 2c20 5769 6467 6574  liesItem, Widget
-00020390: 7357 6964 6765 7443 6f6d 6d65 6e74 2c20  sWidgetComment, 
-000203a0: 5769 6467 6574 7357 6964 6765 744c 696b  WidgetsWidgetLik
-000203b0: 6573 2c20 5769 6467 6574 7357 6964 6765  es, WidgetsWidge
-000203c0: 7450 6167 6529 3a0a 2020 2020 6966 2069  tPage):.    if i
-000203d0: 7373 7562 636c 6173 7328 692c 424d 293a  ssubclass(i,BM):
-000203e0: 0a20 2020 2020 2020 2069 2e75 7064 6174  .        i.updat
-000203f0: 655f 666f 7277 6172 645f 7265 6673 2829  e_forward_refs()
-00020400: 0a0a 5f5f 616c 6c5f 5f20 3d20 2827 4163  ..__all__ = ('Ac
-00020410: 636f 756e 7441 6363 6f75 6e74 436f 756e  countAccountCoun
-00020420: 7465 7273 272c 2027 4163 636f 756e 7449  ters', 'AccountI
-00020430: 6e66 6f27 2c20 2741 6363 6f75 6e74 4e61  nfo', 'AccountNa
-00020440: 6d65 5265 7175 6573 7427 2c20 2741 6363  meRequest', 'Acc
-00020450: 6f75 6e74 4e61 6d65 5265 7175 6573 7453  ountNameRequestS
-00020460: 7461 7475 7327 2c20 2741 6363 6f75 6e74  tatus', 'Account
-00020470: 4f66 6665 7227 2c20 2741 6363 6f75 6e74  Offer', 'Account
-00020480: 5075 7368 436f 6e76 6572 7361 7469 6f6e  PushConversation
-00020490: 7327 2c20 2741 6363 6f75 6e74 5075 7368  s', 'AccountPush
-000204a0: 436f 6e76 6572 7361 7469 6f6e 7349 7465  ConversationsIte
-000204b0: 6d27 2c20 2741 6363 6f75 6e74 5075 7368  m', 'AccountPush
-000204c0: 5061 7261 6d73 272c 2027 4163 636f 756e  Params', 'Accoun
-000204d0: 7450 7573 6850 6172 616d 734d 6f64 6527  tPushParamsMode'
-000204e0: 2c20 2741 6363 6f75 6e74 5075 7368 5061  , 'AccountPushPa
-000204f0: 7261 6d73 4f6e 6f66 6627 2c20 2741 6363  ramsOnoff', 'Acc
-00020500: 6f75 6e74 5075 7368 5061 7261 6d73 5365  ountPushParamsSe
-00020510: 7474 696e 6773 272c 2027 4163 636f 756e  ttings', 'Accoun
-00020520: 7450 7573 6853 6574 7469 6e67 7327 2c20  tPushSettings', 
-00020530: 2741 6363 6f75 6e74 5375 6273 6372 6970  'AccountSubscrip
-00020540: 7469 6f6e 7327 2c20 2741 6363 6f75 6e74  tions', 'Account
-00020550: 5573 6572 5365 7474 696e 6773 272c 2027  UserSettings', '
-00020560: 4163 636f 756e 7455 7365 7253 6574 7469  AccountUserSetti
-00020570: 6e67 7349 6e74 6572 6573 7427 2c20 2741  ngsInterest', 'A
-00020580: 6363 6f75 6e74 5573 6572 5365 7474 696e  ccountUserSettin
-00020590: 6773 496e 7465 7265 7374 7327 2c20 2741  gsInterests', 'A
-000205a0: 6464 7265 7373 6573 4669 656c 6473 272c  ddressesFields',
-000205b0: 2027 4164 7341 6363 6573 7352 6f6c 6527   'AdsAccessRole'
-000205c0: 2c20 2741 6473 4163 6365 7373 526f 6c65  , 'AdsAccessRole
-000205d0: 5075 626c 6963 272c 2027 4164 7341 6363  Public', 'AdsAcc
-000205e0: 6573 7365 7327 2c20 2741 6473 4163 636f  esses', 'AdsAcco
-000205f0: 756e 7427 2c20 2741 6473 4163 636f 756e  unt', 'AdsAccoun
-00020600: 7454 7970 6527 2c20 2741 6473 4164 272c  tType', 'AdsAd',
-00020610: 2027 4164 7341 6441 7070 726f 7665 6427   'AdsAdApproved'
-00020620: 2c20 2741 6473 4164 436f 7374 5479 7065  , 'AdsAdCostType
-00020630: 272c 2027 4164 7341 644c 6179 6f75 7427  ', 'AdsAdLayout'
-00020640: 2c20 2741 6473 4164 5374 6174 7573 272c  , 'AdsAdStatus',
-00020650: 2027 4164 7343 616d 7061 6967 6e27 2c20   'AdsCampaign', 
-00020660: 2741 6473 4361 6d70 6169 676e 5374 6174  'AdsCampaignStat
-00020670: 7573 272c 2027 4164 7343 616d 7061 6967  us', 'AdsCampaig
-00020680: 6e54 7970 6527 2c20 2741 6473 4361 7465  nType', 'AdsCate
-00020690: 676f 7279 272c 2027 4164 7343 6c69 656e  gory', 'AdsClien
-000206a0: 7427 2c20 2741 6473 4372 6561 7465 4164  t', 'AdsCreateAd
-000206b0: 5374 6174 7573 272c 2027 4164 7343 7265  Status', 'AdsCre
-000206c0: 6174 6543 616d 7061 6967 6e53 7461 7475  ateCampaignStatu
-000206d0: 7327 2c20 2741 6473 4372 6974 6572 6961  s', 'AdsCriteria
-000206e0: 272c 2027 4164 7343 7269 7465 7269 6153  ', 'AdsCriteriaS
-000206f0: 6578 272c 2027 4164 7344 656d 6f53 7461  ex', 'AdsDemoSta
-00020700: 7473 272c 2027 4164 7344 656d 6f73 7461  ts', 'AdsDemosta
-00020710: 7473 466f 726d 6174 272c 2027 4164 7346  tsFormat', 'AdsF
-00020720: 6c6f 6f64 5374 6174 7327 2c20 2741 6473  loodStats', 'Ads
-00020730: 4c69 6e6b 5374 6174 7573 272c 2027 4164  LinkStatus', 'Ad
-00020740: 734c 6f6f 6b61 6c69 6b65 5265 7175 6573  sLookalikeReques
-00020750: 7427 2c20 2741 6473 4c6f 6f6b 616c 696b  t', 'AdsLookalik
-00020760: 6552 6571 7565 7374 5361 7665 4175 6469  eRequestSaveAudi
-00020770: 656e 6365 4c65 7665 6c27 2c20 2741 6473  enceLevel', 'Ads
-00020780: 4d75 7369 6369 616e 272c 2027 4164 734f  Musician', 'AdsO
-00020790: 626a 6563 7454 7970 6527 2c20 2741 6473  bjectType', 'Ads
-000207a0: 5061 7261 6772 6170 6873 272c 2027 4164  Paragraphs', 'Ad
-000207b0: 7350 726f 6d6f 7465 6450 6f73 7452 6561  sPromotedPostRea
-000207c0: 6368 272c 2027 4164 7352 656a 6563 7452  ch', 'AdsRejectR
-000207d0: 6561 736f 6e27 2c20 2741 6473 5275 6c65  eason', 'AdsRule
-000207e0: 7327 2c20 2741 6473 5374 6174 7327 2c20  s', 'AdsStats', 
-000207f0: 2741 6473 5374 6174 7341 6765 272c 2027  'AdsStatsAge', '
-00020800: 4164 7353 7461 7473 4369 7469 6573 272c  AdsStatsCities',
-00020810: 2027 4164 7353 7461 7473 466f 726d 6174   'AdsStatsFormat
-00020820: 272c 2027 4164 7353 7461 7473 5365 7827  ', 'AdsStatsSex'
-00020830: 2c20 2741 6473 5374 6174 7353 6578 4167  , 'AdsStatsSexAg
-00020840: 6527 2c20 2741 6473 5374 6174 7353 6578  e', 'AdsStatsSex
-00020850: 5661 6c75 6527 2c20 2741 6473 5374 6174  Value', 'AdsStat
-00020860: 7356 6965 7773 5469 6d65 7327 2c20 2741  sViewsTimes', 'A
-00020870: 6473 5461 7267 5365 7474 696e 6773 272c  dsTargSettings',
-00020880: 2027 4164 7354 6172 6753 7461 7473 272c   'AdsTargStats',
-00020890: 2027 4164 7354 6172 6753 7567 6765 7374   'AdsTargSuggest
-000208a0: 696f 6e73 272c 2027 4164 7354 6172 6753  ions', 'AdsTargS
-000208b0: 7567 6765 7374 696f 6e73 4369 7469 6573  uggestionsCities
-000208c0: 272c 2027 4164 7354 6172 6753 7567 6765  ', 'AdsTargSugge
-000208d0: 7374 696f 6e73 5265 6769 6f6e 7327 2c20  stionsRegions', 
-000208e0: 2741 6473 5461 7267 5375 6767 6573 7469  'AdsTargSuggesti
-000208f0: 6f6e 7353 6368 6f6f 6c73 272c 2027 4164  onsSchools', 'Ad
-00020900: 7354 6172 6753 7567 6765 7374 696f 6e73  sTargSuggestions
-00020910: 5363 686f 6f6c 7354 7970 6527 2c20 2741  SchoolsType', 'A
-00020920: 6473 5461 7267 6574 4772 6f75 7027 2c20  dsTargetGroup', 
-00020930: 2741 6473 5570 6461 7465 4f66 6669 6365  'AdsUpdateOffice
-00020940: 5573 6572 7352 6573 756c 7427 2c20 2741  UsersResult', 'A
-00020950: 6473 5573 6572 5370 6563 6966 6963 6174  dsUserSpecificat
-00020960: 696f 6e27 2c20 2741 6473 5573 6572 5370  ion', 'AdsUserSp
-00020970: 6563 6966 6963 6174 696f 6e43 7574 7465  ecificationCutte
-00020980: 6427 2c20 2741 6473 5573 6572 7327 2c20  d', 'AdsUsers', 
-00020990: 2741 6473 7765 6247 6574 4164 4361 7465  'AdswebGetAdCate
-000209a0: 676f 7269 6573 5265 7370 6f6e 7365 4361  goriesResponseCa
-000209b0: 7465 676f 7269 6573 4361 7465 676f 7279  tegoriesCategory
-000209c0: 272c 2027 4164 7377 6562 4765 7441 6455  ', 'AdswebGetAdU
-000209d0: 6e69 7473 5265 7370 6f6e 7365 4164 556e  nitsResponseAdUn
-000209e0: 6974 7341 6455 6e69 7427 2c20 2741 6473  itsAdUnit', 'Ads
-000209f0: 7765 6247 6574 4672 6175 6448 6973 746f  webGetFraudHisto
-00020a00: 7279 5265 7370 6f6e 7365 456e 7472 6965  ryResponseEntrie
-00020a10: 7345 6e74 7279 272c 2027 4164 7377 6562  sEntry', 'Adsweb
-00020a20: 4765 7453 6974 6573 5265 7370 6f6e 7365  GetSitesResponse
-00020a30: 5369 7465 7353 6974 6527 2c20 2741 6473  SitesSite', 'Ads
-00020a40: 7765 6247 6574 5374 6174 6973 7469 6373  webGetStatistics
-00020a50: 5265 7370 6f6e 7365 4974 656d 7349 7465  ResponseItemsIte
-00020a60: 6d27 2c20 2741 7070 5769 6467 6574 7350  m', 'AppWidgetsP
-00020a70: 686f 746f 272c 2027 4170 7057 6964 6765  hoto', 'AppWidge
-00020a80: 7473 5068 6f74 6f73 272c 2027 4170 7073  tsPhotos', 'Apps
-00020a90: 4170 7027 2c20 2741 7070 7341 7070 4c65  App', 'AppsAppLe
-00020aa0: 6164 6572 626f 6172 6454 7970 6527 2c20  aderboardType', 
-00020ab0: 2741 7070 7341 7070 4d69 6e27 2c20 2741  'AppsAppMin', 'A
-00020ac0: 7070 7341 7070 5479 7065 272c 2027 4170  ppsAppType', 'Ap
-00020ad0: 7073 4361 7461 6c6f 674c 6973 7427 2c20  psCatalogList', 
-00020ae0: 2741 7070 734c 6561 6465 7262 6f61 7264  'AppsLeaderboard
-00020af0: 272c 2027 4170 7073 5363 6f70 6527 2c20  ', 'AppsScope', 
-00020b00: 2741 7564 696f 4175 6469 6f27 2c20 2762  'AudioAudio', 'b
-00020b10: 6f6f 6c27 2c20 2742 6173 6543 6974 7927  ool', 'BaseCity'
-00020b20: 2c20 2742 6173 6543 6f6d 6d65 6e74 7349  , 'BaseCommentsI
-00020b30: 6e66 6f27 2c20 2742 6173 6543 6f75 6e74  nfo', 'BaseCount
-00020b40: 7279 272c 2027 4261 7365 4372 6f70 5068  ry', 'BaseCropPh
-00020b50: 6f74 6f27 2c20 2742 6173 6543 726f 7050  oto', 'BaseCropP
-00020b60: 686f 746f 4372 6f70 272c 2027 4261 7365  hotoCrop', 'Base
-00020b70: 4372 6f70 5068 6f74 6f52 6563 7427 2c20  CropPhotoRect', 
-00020b80: 2742 6173 6545 7272 6f72 272c 2027 4261  'BaseError', 'Ba
-00020b90: 7365 4765 6f27 2c20 2742 6173 6547 656f  seGeo', 'BaseGeo
-00020ba0: 436f 6f72 6469 6e61 7465 7327 2c20 2742  Coordinates', 'B
-00020bb0: 6173 6547 7261 6469 656e 7450 6f69 6e74  aseGradientPoint
-00020bc0: 272c 2027 4261 7365 496d 6167 6527 2c20  ', 'BaseImage', 
-00020bd0: 2742 6173 654c 696b 6573 272c 2027 4261  'BaseLikes', 'Ba
-00020be0: 7365 4c69 6b65 7349 6e66 6f27 2c20 2742  seLikesInfo', 'B
-00020bf0: 6173 654c 696e 6b27 2c20 2742 6173 654c  aseLink', 'BaseL
-00020c00: 696e 6b41 7070 6c69 6361 7469 6f6e 272c  inkApplication',
-00020c10: 2027 4261 7365 4c69 6e6b 4170 706c 6963   'BaseLinkApplic
-00020c20: 6174 696f 6e53 746f 7265 272c 2027 4261  ationStore', 'Ba
-00020c30: 7365 4c69 6e6b 4275 7474 6f6e 272c 2027  seLinkButton', '
-00020c40: 4261 7365 4c69 6e6b 4275 7474 6f6e 4163  BaseLinkButtonAc
-00020c50: 7469 6f6e 272c 2027 4261 7365 4c69 6e6b  tion', 'BaseLink
-00020c60: 4275 7474 6f6e 4163 7469 6f6e 5479 7065  ButtonActionType
-00020c70: 272c 2027 4261 7365 4c69 6e6b 4275 7474  ', 'BaseLinkButt
-00020c80: 6f6e 5374 796c 6527 2c20 2742 6173 654c  onStyle', 'BaseL
-00020c90: 696e 6b50 726f 6475 6374 272c 2027 4261  inkProduct', 'Ba
-00020ca0: 7365 4c69 6e6b 5072 6f64 7563 7443 6174  seLinkProductCat
-00020cb0: 6567 6f72 7927 2c20 2742 6173 654c 696e  egory', 'BaseLin
-00020cc0: 6b50 726f 6475 6374 5374 6174 7573 272c  kProductStatus',
-00020cd0: 2027 4261 7365 4c69 6e6b 5261 7469 6e67   'BaseLinkRating
-00020ce0: 272c 2027 4261 7365 4d65 7373 6167 6545  ', 'BaseMessageE
-00020cf0: 7272 6f72 272c 2027 4261 7365 4f62 6a65  rror', 'BaseObje
-00020d00: 6374 272c 2027 4261 7365 4f62 6a65 6374  ct', 'BaseObject
-00020d10: 436f 756e 7427 2c20 2742 6173 654f 626a  Count', 'BaseObj
-00020d20: 6563 7457 6974 684e 616d 6527 2c20 2742  ectWithName', 'B
-00020d30: 6173 6550 6c61 6365 272c 2027 4261 7365  asePlace', 'Base
-00020d40: 5072 6f70 6572 7479 4578 6973 7473 272c  PropertyExists',
-00020d50: 2027 4261 7365 5265 706f 7374 7349 6e66   'BaseRepostsInf
-00020d60: 6f27 2c20 2742 6173 6552 6571 7565 7374  o', 'BaseRequest
-00020d70: 5061 7261 6d27 2c20 2742 6173 6553 6578  Param', 'BaseSex
-00020d80: 272c 2027 4261 7365 5374 6963 6b65 7227  ', 'BaseSticker'
-00020d90: 2c20 2742 6173 6553 7469 636b 6572 416e  , 'BaseStickerAn
-00020da0: 696d 6174 696f 6e27 2c20 2742 6173 6553  imation', 'BaseS
-00020db0: 7469 636b 6572 4e65 7727 2c20 2742 6173  tickerNew', 'Bas
-00020dc0: 6553 7469 636b 6572 4f6c 6427 2c20 2742  eStickerOld', 'B
-00020dd0: 6173 6553 7469 636b 6572 734c 6973 7427  aseStickersList'
-00020de0: 2c20 2742 6173 6555 706c 6f61 6453 6572  , 'BaseUploadSer
-00020df0: 7665 7227 2c20 2742 6173 6555 7365 7247  ver', 'BaseUserG
-00020e00: 726f 7570 4669 656c 6473 272c 2027 4261  roupFields', 'Ba
-00020e10: 7365 5573 6572 4964 272c 2027 426f 6172  seUserId', 'Boar
-00020e20: 6444 6566 6175 6c74 4f72 6465 7227 2c20  dDefaultOrder', 
-00020e30: 2742 6f61 7264 546f 7069 6327 2c20 2742  'BoardTopic', 'B
-00020e40: 6f61 7264 546f 7069 6343 6f6d 6d65 6e74  oardTopicComment
-00020e50: 272c 2027 4361 6c6c 6261 636b 4261 7365  ', 'CallbackBase
-00020e60: 272c 2027 4361 6c6c 6261 636b 426f 6172  ', 'CallbackBoar
-00020e70: 6450 6f73 7444 656c 6574 6527 2c20 2743  dPostDelete', 'C
-00020e80: 616c 6c62 6163 6b43 6f6e 6669 726d 6174  allbackConfirmat
-00020e90: 696f 6e27 2c20 2743 616c 6c62 6163 6b44  ion', 'CallbackD
-00020ea0: 6f6e 7574 4d6f 6e65 7957 6974 6864 7261  onutMoneyWithdra
-00020eb0: 7727 2c20 2743 616c 6c62 6163 6b44 6f6e  w', 'CallbackDon
-00020ec0: 7574 4d6f 6e65 7957 6974 6864 7261 7745  utMoneyWithdrawE
-00020ed0: 7272 6f72 272c 2027 4361 6c6c 6261 636b  rror', 'Callback
-00020ee0: 446f 6e75 7453 7562 7363 7269 7074 696f  DonutSubscriptio
-00020ef0: 6e43 616e 6365 6c6c 6564 272c 2027 4361  nCancelled', 'Ca
-00020f00: 6c6c 6261 636b 446f 6e75 7453 7562 7363  llbackDonutSubsc
-00020f10: 7269 7074 696f 6e43 7265 6174 6527 2c20  riptionCreate', 
-00020f20: 2743 616c 6c62 6163 6b44 6f6e 7574 5375  'CallbackDonutSu
-00020f30: 6273 6372 6970 7469 6f6e 4578 7069 7265  bscriptionExpire
-00020f40: 6427 2c20 2743 616c 6c62 6163 6b44 6f6e  d', 'CallbackDon
-00020f50: 7574 5375 6273 6372 6970 7469 6f6e 5072  utSubscriptionPr
-00020f60: 6963 6543 6861 6e67 6564 272c 2027 4361  iceChanged', 'Ca
-00020f70: 6c6c 6261 636b 446f 6e75 7453 7562 7363  llbackDonutSubsc
-00020f80: 7269 7074 696f 6e50 726f 6c6f 6e67 6564  riptionProlonged
-00020f90: 272c 2027 4361 6c6c 6261 636b 4772 6f75  ', 'CallbackGrou
-00020fa0: 7043 6861 6e67 6550 686f 746f 272c 2027  pChangePhoto', '
-00020fb0: 4361 6c6c 6261 636b 4772 6f75 7043 6861  CallbackGroupCha
-00020fc0: 6e67 6553 6574 7469 6e67 7327 2c20 2743  ngeSettings', 'C
-00020fd0: 616c 6c62 6163 6b47 726f 7570 4a6f 696e  allbackGroupJoin
-00020fe0: 272c 2027 4361 6c6c 6261 636b 4772 6f75  ', 'CallbackGrou
-00020ff0: 704a 6f69 6e54 7970 6527 2c20 2743 616c  pJoinType', 'Cal
-00021000: 6c62 6163 6b47 726f 7570 4c65 6176 6527  lbackGroupLeave'
-00021010: 2c20 2743 616c 6c62 6163 6b47 726f 7570  , 'CallbackGroup
-00021020: 4d61 726b 6574 272c 2027 4361 6c6c 6261  Market', 'Callba
-00021030: 636b 4772 6f75 704f 6666 6963 6572 526f  ckGroupOfficerRo
-00021040: 6c65 272c 2027 4361 6c6c 6261 636b 4772  le', 'CallbackGr
-00021050: 6f75 704f 6666 6963 6572 7345 6469 7427  oupOfficersEdit'
-00021060: 2c20 2743 616c 6c62 6163 6b47 726f 7570  , 'CallbackGroup
-00021070: 5365 7474 696e 6773 4368 616e 6765 7327  SettingsChanges'
-00021080: 2c20 2743 616c 6c62 6163 6b4c 696b 6541  , 'CallbackLikeA
-00021090: 6464 5265 6d6f 7665 272c 2027 4361 6c6c  ddRemove', 'Call
-000210a0: 6261 636b 4d61 726b 6574 436f 6d6d 656e  backMarketCommen
-000210b0: 7427 2c20 2743 616c 6c62 6163 6b4d 6172  t', 'CallbackMar
-000210c0: 6b65 7443 6f6d 6d65 6e74 4465 6c65 7465  ketCommentDelete
-000210d0: 272c 2027 4361 6c6c 6261 636b 4d65 7373  ', 'CallbackMess
-000210e0: 6167 6541 6c6c 6f77 272c 2027 4361 6c6c  ageAllow', 'Call
-000210f0: 6261 636b 4d65 7373 6167 6541 6c6c 6f77  backMessageAllow
-00021100: 4f62 6a65 6374 272c 2027 4361 6c6c 6261  Object', 'Callba
-00021110: 636b 4d65 7373 6167 6544 656e 7927 2c20  ckMessageDeny', 
-00021120: 2743 616c 6c62 6163 6b4d 6573 7361 6765  'CallbackMessage
-00021130: 4564 6974 272c 2027 4361 6c6c 6261 636b  Edit', 'Callback
-00021140: 4d65 7373 6167 654e 6577 272c 2027 4361  MessageNew', 'Ca
-00021150: 6c6c 6261 636b 4d65 7373 6167 654f 626a  llbackMessageObj
-00021160: 6563 7427 2c20 2743 616c 6c62 6163 6b4d  ect', 'CallbackM
-00021170: 6573 7361 6765 5265 706c 7927 2c20 2743  essageReply', 'C
-00021180: 616c 6c62 6163 6b50 686f 746f 436f 6d6d  allbackPhotoComm
-00021190: 656e 7427 2c20 2743 616c 6c62 6163 6b50  ent', 'CallbackP
-000211a0: 686f 746f 436f 6d6d 656e 7444 656c 6574  hotoCommentDelet
-000211b0: 6527 2c20 2743 616c 6c62 6163 6b50 6f6c  e', 'CallbackPol
-000211c0: 6c56 6f74 654e 6577 272c 2027 4361 6c6c  lVoteNew', 'Call
-000211d0: 6261 636b 5172 5363 616e 272c 2027 4361  backQrScan', 'Ca
-000211e0: 6c6c 6261 636b 5479 7065 272c 2027 4361  llbackType', 'Ca
-000211f0: 6c6c 6261 636b 5573 6572 426c 6f63 6b27  llbackUserBlock'
-00021200: 2c20 2743 616c 6c62 6163 6b55 7365 7255  , 'CallbackUserU
-00021210: 6e62 6c6f 636b 272c 2027 4361 6c6c 6261  nblock', 'Callba
-00021220: 636b 5669 6465 6f43 6f6d 6d65 6e74 272c  ckVideoComment',
-00021230: 2027 4361 6c6c 6261 636b 5669 6465 6f43   'CallbackVideoC
-00021240: 6f6d 6d65 6e74 4465 6c65 7465 272c 2027  ommentDelete', '
-00021250: 4361 6c6c 6261 636b 5761 6c6c 436f 6d6d  CallbackWallComm
-00021260: 656e 7444 656c 6574 6527 2c20 2743 616c  entDelete', 'Cal
-00021270: 6c73 4361 6c6c 272c 2027 4361 6c6c 7345  lsCall', 'CallsE
-00021280: 6e64 5374 6174 6527 2c20 2743 616c 6c73  ndState', 'Calls
-00021290: 5061 7274 6963 6970 616e 7473 272c 2027  Participants', '
-000212a0: 436c 6965 6e74 496e 666f 466f 7242 6f74  ClientInfoForBot
-000212b0: 7327 2c20 2743 6f6d 6d65 6e74 5468 7265  s', 'CommentThre
-000212c0: 6164 272c 2027 4461 7461 6261 7365 4369  ad', 'DatabaseCi
-000212d0: 7479 272c 2027 4461 7461 6261 7365 4369  ty', 'DatabaseCi
-000212e0: 7479 4279 4964 272c 2027 4461 7461 6261  tyById', 'Databa
-000212f0: 7365 4661 6375 6c74 7927 2c20 2744 6174  seFaculty', 'Dat
-00021300: 6162 6173 6552 6567 696f 6e27 2c20 2744  abaseRegion', 'D
-00021310: 6174 6162 6173 6553 6368 6f6f 6c27 2c20  atabaseSchool', 
-00021320: 2744 6174 6162 6173 6553 7461 7469 6f6e  'DatabaseStation
-00021330: 272c 2027 4461 7461 6261 7365 556e 6976  ', 'DatabaseUniv
-00021340: 6572 7369 7479 272c 2027 446f 6373 446f  ersity', 'DocsDo
-00021350: 6327 2c20 2744 6f63 7344 6f63 4174 7461  c', 'DocsDocAtta
-00021360: 6368 6d65 6e74 5479 7065 272c 2027 446f  chmentType', 'Do
-00021370: 6373 446f 6350 7265 7669 6577 272c 2027  csDocPreview', '
-00021380: 446f 6373 446f 6350 7265 7669 6577 4175  DocsDocPreviewAu
-00021390: 6469 6f4d 7367 272c 2027 446f 6373 446f  dioMsg', 'DocsDo
-000213a0: 6350 7265 7669 6577 4772 6166 6669 7469  cPreviewGraffiti
+0001fa70: 6f6e 4974 656d 2c0a 5068 6f74 6f73 5461  onItem,.PhotosTa
+0001fa80: 6773 5375 6767 6573 7469 6f6e 4974 656d  gsSuggestionItem
+0001fa90: 4275 7474 6f6e 2c20 506f 6463 6173 7443  Button, PodcastC
+0001faa0: 6f76 6572 2c20 506f 6463 6173 7445 7874  over, PodcastExt
+0001fab0: 6572 6e61 6c44 6174 612c 2050 6f6c 6c73  ernalData, Polls
+0001fac0: 416e 7377 6572 2c20 506f 6c6c 7342 6163  Answer, PollsBac
+0001fad0: 6b67 726f 756e 642c 2050 6f6c 6c73 4672  kground, PollsFr
+0001fae0: 6965 6e64 2c20 506f 6c6c 7350 6f6c 6c2c  iend, PollsPoll,
+0001faf0: 2050 6f6c 6c73 506f 6c6c 416e 6f6e 796d   PollsPollAnonym
+0001fb00: 6f75 732c 0a50 6f6c 6c73 566f 7465 7273  ous,.PollsVoters
+0001fb10: 2c20 506f 6c6c 7356 6f74 6572 7355 7365  , PollsVotersUse
+0001fb20: 7273 2c20 5072 6574 7479 4361 7264 7350  rs, PrettyCardsP
+0001fb30: 7265 7474 7943 6172 642c 2050 7265 7474  rettyCard, Prett
+0001fb40: 7943 6172 6473 5072 6574 7479 4361 7264  yCardsPrettyCard
+0001fb50: 4f72 4572 726f 722c 2053 6561 7263 6848  OrError, SearchH
+0001fb60: 696e 742c 2053 6561 7263 6848 696e 7453  int, SearchHintS
+0001fb70: 6563 7469 6f6e 2c20 5365 6172 6368 4869  ection, SearchHi
+0001fb80: 6e74 5479 7065 2c0a 5365 6375 7265 4769  ntType,.SecureGi
+0001fb90: 7665 4576 656e 7453 7469 636b 6572 4974  veEventStickerIt
+0001fba0: 656d 2c20 5365 6375 7265 4c65 7665 6c2c  em, SecureLevel,
+0001fbb0: 2053 6563 7572 6553 6574 436f 756e 7465   SecureSetCounte
+0001fbc0: 7249 7465 6d2c 2053 6563 7572 6553 6d73  rItem, SecureSms
+0001fbd0: 4e6f 7469 6669 6361 7469 6f6e 2c20 5365  Notification, Se
+0001fbe0: 6375 7265 546f 6b65 6e43 6865 636b 6564  cureTokenChecked
+0001fbf0: 2c20 5365 6375 7265 5472 616e 7361 6374  , SecureTransact
+0001fc00: 696f 6e2c 2053 7461 7473 4163 7469 7669  ion, StatsActivi
+0001fc10: 7479 2c20 5374 6174 7343 6974 792c 0a53  ty, StatsCity,.S
+0001fc20: 7461 7473 436f 756e 7472 792c 2053 7461  tatsCountry, Sta
+0001fc30: 7473 5065 7269 6f64 2c20 5374 6174 7352  tsPeriod, StatsR
+0001fc40: 6561 6368 2c20 5374 6174 7353 6578 4167  each, StatsSexAg
+0001fc50: 652c 2053 7461 7473 5669 6577 732c 2053  e, StatsViews, S
+0001fc60: 7461 7473 5761 6c6c 706f 7374 5374 6174  tatsWallpostStat
+0001fc70: 2c20 5374 6174 7573 5374 6174 7573 2c20  , StatusStatus, 
+0001fc80: 5374 6963 6b65 7273 496d 6167 6553 6574  StickersImageSet
+0001fc90: 2c20 5374 6f72 6167 6556 616c 7565 2c20  , StorageValue, 
+0001fca0: 5374 6f72 6550 726f 6475 6374 2c0a 5374  StoreProduct,.St
+0001fcb0: 6f72 6550 726f 6475 6374 4963 6f6e 2c20  oreProductIcon, 
+0001fcc0: 5374 6f72 6553 7469 636b 6572 734b 6579  StoreStickersKey
+0001fcd0: 776f 7264 2c20 5374 6f72 6553 7469 636b  word, StoreStick
+0001fce0: 6572 734b 6579 776f 7264 5374 6963 6b65  ersKeywordSticke
+0001fcf0: 722c 2053 746f 7265 5374 6963 6b65 7273  r, StoreStickers
+0001fd00: 4b65 7977 6f72 6453 7469 636b 6572 732c  KeywordStickers,
+0001fd10: 2053 746f 7269 6573 436c 6963 6b61 626c   StoriesClickabl
+0001fd20: 6541 7265 612c 2053 746f 7269 6573 436c  eArea, StoriesCl
+0001fd30: 6963 6b61 626c 6553 7469 636b 6572 2c0a  ickableSticker,.
+0001fd40: 5374 6f72 6965 7343 6c69 636b 6162 6c65  StoriesClickable
+0001fd50: 5374 6963 6b65 7273 2c20 5374 6f72 6965  Stickers, Storie
+0001fd60: 7346 6565 6449 7465 6d2c 2053 746f 7269  sFeedItem, Stori
+0001fd70: 6573 5072 6f6d 6f42 6c6f 636b 2c20 5374  esPromoBlock, St
+0001fd80: 6f72 6965 7352 6570 6c69 6573 2c20 5374  oriesReplies, St
+0001fd90: 6f72 6965 7353 7461 744c 696e 652c 2053  oriesStatLine, S
+0001fda0: 746f 7269 6573 5374 6f72 792c 2053 746f  toriesStory, Sto
+0001fdb0: 7269 6573 5374 6f72 794c 696e 6b2c 2053  riesStoryLink, S
+0001fdc0: 746f 7269 6573 5374 6f72 7953 7461 7473  toriesStoryStats
+0001fdd0: 2c0a 5374 6f72 6965 7353 746f 7279 5374  ,.StoriesStorySt
+0001fde0: 6174 7353 7461 742c 2053 746f 7269 6573  atsStat, Stories
+0001fdf0: 5374 6f72 7953 7461 7473 5374 6174 652c  StoryStatsState,
+0001fe00: 2053 746f 7269 6573 5374 6f72 7954 7970   StoriesStoryTyp
+0001fe10: 652c 2053 746f 7269 6573 5570 6c6f 6164  e, StoriesUpload
+0001fe20: 4c69 6e6b 5465 7874 2c20 5374 6f72 6965  LinkText, Storie
+0001fe30: 7356 6965 7765 7273 4974 656d 2c20 5573  sViewersItem, Us
+0001fe40: 6572 7343 6172 6565 722c 2055 7365 7273  ersCareer, Users
+0001fe50: 4578 706f 7274 732c 2055 7365 7273 4669  Exports, UsersFi
+0001fe60: 656c 6473 2c0a 5573 6572 734c 6173 7453  elds,.UsersLastS
+0001fe70: 6565 6e2c 2055 7365 7273 4d69 6c69 7461  een, UsersMilita
+0001fe80: 7279 2c20 5573 6572 734f 6363 7570 6174  ry, UsersOccupat
+0001fe90: 696f 6e2c 2055 7365 7273 4f6e 6c69 6e65  ion, UsersOnline
+0001fea0: 496e 666f 2c20 5573 6572 7350 6572 736f  Info, UsersPerso
+0001feb0: 6e61 6c2c 2055 7365 7273 5265 6c61 7469  nal, UsersRelati
+0001fec0: 7665 2c20 5573 6572 7353 6368 6f6f 6c2c  ve, UsersSchool,
+0001fed0: 2055 7365 7273 5375 6273 6372 6970 7469   UsersSubscripti
+0001fee0: 6f6e 7349 7465 6d2c 2055 7365 7273 556e  onsItem, UsersUn
+0001fef0: 6976 6572 7369 7479 2c0a 5573 6572 7355  iversity,.UsersU
+0001ff00: 7365 722c 2055 7365 7273 5573 6572 436f  ser, UsersUserCo
+0001ff10: 6e6e 6563 7469 6f6e 732c 2055 7365 7273  nnections, Users
+0001ff20: 5573 6572 436f 756e 7465 7273 2c20 5573  UserCounters, Us
+0001ff30: 6572 7355 7365 7246 756c 6c2c 2055 7365  ersUserFull, Use
+0001ff40: 7273 5573 6572 4d69 6e2c 2055 7365 7273  rsUserMin, Users
+0001ff50: 5573 6572 5265 6c61 7469 6f6e 2c20 5573  UserRelation, Us
+0001ff60: 6572 7355 7365 7253 6574 7469 6e67 7358  ersUserSettingsX
+0001ff70: 7472 2c20 5573 6572 7355 7365 7254 7970  tr, UsersUserTyp
+0001ff80: 652c 0a55 7365 7273 5573 6572 5874 7254  e,.UsersUserXtrT
+0001ff90: 7970 652c 2055 7365 7273 5573 6572 7341  ype, UsersUsersA
+0001ffa0: 7272 6179 2c20 5574 696c 7344 6f6d 6169  rray, UtilsDomai
+0001ffb0: 6e52 6573 6f6c 7665 642c 2055 7469 6c73  nResolved, Utils
+0001ffc0: 446f 6d61 696e 5265 736f 6c76 6564 5479  DomainResolvedTy
+0001ffd0: 7065 2c20 5574 696c 734c 6173 7453 686f  pe, UtilsLastSho
+0001ffe0: 7274 656e 6564 4c69 6e6b 2c20 5574 696c  rtenedLink, Util
+0001fff0: 734c 696e 6b43 6865 636b 6564 2c20 5574  sLinkChecked, Ut
+00020000: 696c 734c 696e 6b43 6865 636b 6564 5374  ilsLinkCheckedSt
+00020010: 6174 7573 2c0a 5574 696c 734c 696e 6b53  atus,.UtilsLinkS
+00020020: 7461 7473 2c20 5574 696c 734c 696e 6b53  tats, UtilsLinkS
+00020030: 7461 7473 4578 7465 6e64 6564 2c20 5574  tatsExtended, Ut
+00020040: 696c 7353 686f 7274 4c69 6e6b 2c20 5574  ilsShortLink, Ut
+00020050: 696c 7353 7461 7473 2c20 5574 696c 7353  ilsStats, UtilsS
+00020060: 7461 7473 4369 7479 2c20 5574 696c 7353  tatsCity, UtilsS
+00020070: 7461 7473 436f 756e 7472 792c 2055 7469  tatsCountry, Uti
+00020080: 6c73 5374 6174 7345 7874 656e 6465 642c  lsStatsExtended,
+00020090: 2055 7469 6c73 5374 6174 7353 6578 4167   UtilsStatsSexAg
+000200a0: 652c 0a56 6964 656f 4c69 7665 496e 666f  e,.VideoLiveInfo
+000200b0: 2c20 5669 6465 6f4c 6976 6553 6574 7469  , VideoLiveSetti
+000200c0: 6e67 732c 2056 6964 656f 5361 7665 5265  ngs, VideoSaveRe
+000200d0: 7375 6c74 2c20 5669 6465 6f56 6964 656f  sult, VideoVideo
+000200e0: 2c20 5669 6465 6f56 6964 656f 416c 6275  , VideoVideoAlbu
+000200f0: 6d2c 2056 6964 656f 5669 6465 6f41 6c62  m, VideoVideoAlb
+00020100: 756d 4675 6c6c 2c20 5669 6465 6f56 6964  umFull, VideoVid
+00020110: 656f 4669 6c65 732c 2056 6964 656f 5669  eoFiles, VideoVi
+00020120: 6465 6f46 756c 6c2c 2056 6964 656f 5669  deoFull, VideoVi
+00020130: 6465 6f49 6d61 6765 2c0a 5761 6c6c 4170  deoImage,.WallAp
+00020140: 7050 6f73 742c 2057 616c 6c41 7474 6163  pPost, WallAttac
+00020150: 6865 644e 6f74 652c 2057 616c 6c43 6172  hedNote, WallCar
+00020160: 6f75 7365 6c42 6173 652c 2057 616c 6c43  ouselBase, WallC
+00020170: 6f6d 6d65 6e74 4174 7461 6368 6d65 6e74  ommentAttachment
+00020180: 2c20 5761 6c6c 436f 6d6d 656e 7441 7474  , WallCommentAtt
+00020190: 6163 686d 656e 7454 7970 652c 2057 616c  achmentType, Wal
+000201a0: 6c47 656f 2c20 5761 6c6c 4765 7446 696c  lGeo, WallGetFil
+000201b0: 7465 722c 2057 616c 6c47 7261 6666 6974  ter, WallGraffit
+000201c0: 692c 0a57 616c 6c50 6f73 7443 6f70 7972  i,.WallPostCopyr
+000201d0: 6967 6874 2c20 5761 6c6c 506f 7374 536f  ight, WallPostSo
+000201e0: 7572 6365 2c20 5761 6c6c 506f 7374 536f  urce, WallPostSo
+000201f0: 7572 6365 5479 7065 2c20 5761 6c6c 506f  urceType, WallPo
+00020200: 7374 5479 7065 2c20 5761 6c6c 506f 7374  stType, WallPost
+00020210: 6564 5068 6f74 6f2c 2057 616c 6c56 6965  edPhoto, WallVie
+00020220: 7773 2c20 5761 6c6c 5761 6c6c 436f 6d6d  ws, WallWallComm
+00020230: 656e 742c 2057 616c 6c57 616c 6c43 6f6d  ent, WallWallCom
+00020240: 6d65 6e74 446f 6e75 742c 0a57 616c 6c57  mentDonut,.WallW
+00020250: 616c 6c43 6f6d 6d65 6e74 446f 6e75 7450  allCommentDonutP
+00020260: 6c61 6365 686f 6c64 6572 2c20 5761 6c6c  laceholder, Wall
+00020270: 5761 6c6c 706f 7374 2c20 5761 6c6c 5761  Wallpost, WallWa
+00020280: 6c6c 706f 7374 4174 7461 6368 6d65 6e74  llpostAttachment
+00020290: 2c20 5761 6c6c 5761 6c6c 706f 7374 4174  , WallWallpostAt
+000202a0: 7461 6368 6d65 6e74 5479 7065 2c20 5761  tachmentType, Wa
+000202b0: 6c6c 5761 6c6c 706f 7374 436f 6d6d 656e  llWallpostCommen
+000202c0: 7473 446f 6e75 742c 0a57 616c 6c57 616c  tsDonut,.WallWal
+000202d0: 6c70 6f73 7443 6f6d 6d65 6e74 7344 6f6e  lpostCommentsDon
+000202e0: 7574 506c 6163 6568 6f6c 6465 722c 2057  utPlaceholder, W
+000202f0: 616c 6c57 616c 6c70 6f73 7444 6f6e 7574  allWallpostDonut
+00020300: 2c20 5761 6c6c 5761 6c6c 706f 7374 446f  , WallWallpostDo
+00020310: 6e75 7450 6c61 6365 686f 6c64 6572 2c20  nutPlaceholder, 
+00020320: 5761 6c6c 5761 6c6c 706f 7374 4675 6c6c  WallWallpostFull
+00020330: 2c20 5761 6c6c 5761 6c6c 706f 7374 546f  , WallWallpostTo
+00020340: 4964 2c20 5769 6467 6574 7343 6f6d 6d65  Id, WidgetsComme
+00020350: 6e74 4d65 6469 612c 0a57 6964 6765 7473  ntMedia,.Widgets
+00020360: 436f 6d6d 656e 744d 6564 6961 5479 7065  CommentMediaType
+00020370: 2c20 5769 6467 6574 7343 6f6d 6d65 6e74  , WidgetsComment
+00020380: 5265 706c 6965 732c 2057 6964 6765 7473  Replies, Widgets
+00020390: 436f 6d6d 656e 7452 6570 6c69 6573 4974  CommentRepliesIt
+000203a0: 656d 2c20 5769 6467 6574 7357 6964 6765  em, WidgetsWidge
+000203b0: 7443 6f6d 6d65 6e74 2c20 5769 6467 6574  tComment, Widget
+000203c0: 7357 6964 6765 744c 696b 6573 2c20 5769  sWidgetLikes, Wi
+000203d0: 6467 6574 7357 6964 6765 7450 6167 6529  dgetsWidgetPage)
+000203e0: 3a0a 2020 2020 6966 2069 7373 7562 636c  :.    if issubcl
+000203f0: 6173 7328 692c 424d 293a 0a20 2020 2020  ass(i,BM):.     
+00020400: 2020 2069 2e75 7064 6174 655f 666f 7277     i.update_forw
+00020410: 6172 645f 7265 6673 2829 0a0a 5f5f 616c  ard_refs()..__al
+00020420: 6c5f 5f20 3d20 2827 4163 636f 756e 7441  l__ = ('AccountA
+00020430: 6363 6f75 6e74 436f 756e 7465 7273 272c  ccountCounters',
+00020440: 2027 4163 636f 756e 7449 6e66 6f27 2c20   'AccountInfo', 
+00020450: 2741 6363 6f75 6e74 4e61 6d65 5265 7175  'AccountNameRequ
+00020460: 6573 7427 2c20 2741 6363 6f75 6e74 4e61  est', 'AccountNa
+00020470: 6d65 5265 7175 6573 7453 7461 7475 7327  meRequestStatus'
+00020480: 2c20 2741 6363 6f75 6e74 4f66 6665 7227  , 'AccountOffer'
+00020490: 2c20 2741 6363 6f75 6e74 5075 7368 436f  , 'AccountPushCo
+000204a0: 6e76 6572 7361 7469 6f6e 7327 2c20 2741  nversations', 'A
+000204b0: 6363 6f75 6e74 5075 7368 436f 6e76 6572  ccountPushConver
+000204c0: 7361 7469 6f6e 7349 7465 6d27 2c20 2741  sationsItem', 'A
+000204d0: 6363 6f75 6e74 5075 7368 5061 7261 6d73  ccountPushParams
+000204e0: 272c 2027 4163 636f 756e 7450 7573 6850  ', 'AccountPushP
+000204f0: 6172 616d 734d 6f64 6527 2c20 2741 6363  aramsMode', 'Acc
+00020500: 6f75 6e74 5075 7368 5061 7261 6d73 4f6e  ountPushParamsOn
+00020510: 6f66 6627 2c20 2741 6363 6f75 6e74 5075  off', 'AccountPu
+00020520: 7368 5061 7261 6d73 5365 7474 696e 6773  shParamsSettings
+00020530: 272c 2027 4163 636f 756e 7450 7573 6853  ', 'AccountPushS
+00020540: 6574 7469 6e67 7327 2c20 2741 6363 6f75  ettings', 'Accou
+00020550: 6e74 5375 6273 6372 6970 7469 6f6e 7327  ntSubscriptions'
+00020560: 2c20 2741 6363 6f75 6e74 5573 6572 5365  , 'AccountUserSe
+00020570: 7474 696e 6773 272c 2027 4163 636f 756e  ttings', 'Accoun
+00020580: 7455 7365 7253 6574 7469 6e67 7349 6e74  tUserSettingsInt
+00020590: 6572 6573 7427 2c20 2741 6363 6f75 6e74  erest', 'Account
+000205a0: 5573 6572 5365 7474 696e 6773 496e 7465  UserSettingsInte
+000205b0: 7265 7374 7327 2c20 2741 6464 7265 7373  rests', 'Address
+000205c0: 6573 4669 656c 6473 272c 2027 4164 7341  esFields', 'AdsA
+000205d0: 6363 6573 7352 6f6c 6527 2c20 2741 6473  ccessRole', 'Ads
+000205e0: 4163 6365 7373 526f 6c65 5075 626c 6963  AccessRolePublic
+000205f0: 272c 2027 4164 7341 6363 6573 7365 7327  ', 'AdsAccesses'
+00020600: 2c20 2741 6473 4163 636f 756e 7427 2c20  , 'AdsAccount', 
+00020610: 2741 6473 4163 636f 756e 7454 7970 6527  'AdsAccountType'
+00020620: 2c20 2741 6473 4164 272c 2027 4164 7341  , 'AdsAd', 'AdsA
+00020630: 6441 7070 726f 7665 6427 2c20 2741 6473  dApproved', 'Ads
+00020640: 4164 436f 7374 5479 7065 272c 2027 4164  AdCostType', 'Ad
+00020650: 7341 644c 6179 6f75 7427 2c20 2741 6473  sAdLayout', 'Ads
+00020660: 4164 5374 6174 7573 272c 2027 4164 7343  AdStatus', 'AdsC
+00020670: 616d 7061 6967 6e27 2c20 2741 6473 4361  ampaign', 'AdsCa
+00020680: 6d70 6169 676e 5374 6174 7573 272c 2027  mpaignStatus', '
+00020690: 4164 7343 616d 7061 6967 6e54 7970 6527  AdsCampaignType'
+000206a0: 2c20 2741 6473 4361 7465 676f 7279 272c  , 'AdsCategory',
+000206b0: 2027 4164 7343 6c69 656e 7427 2c20 2741   'AdsClient', 'A
+000206c0: 6473 4372 6561 7465 4164 5374 6174 7573  dsCreateAdStatus
+000206d0: 272c 2027 4164 7343 7265 6174 6543 616d  ', 'AdsCreateCam
+000206e0: 7061 6967 6e53 7461 7475 7327 2c20 2741  paignStatus', 'A
+000206f0: 6473 4372 6974 6572 6961 272c 2027 4164  dsCriteria', 'Ad
+00020700: 7343 7269 7465 7269 6153 6578 272c 2027  sCriteriaSex', '
+00020710: 4164 7344 656d 6f53 7461 7473 272c 2027  AdsDemoStats', '
+00020720: 4164 7344 656d 6f73 7461 7473 466f 726d  AdsDemostatsForm
+00020730: 6174 272c 2027 4164 7346 6c6f 6f64 5374  at', 'AdsFloodSt
+00020740: 6174 7327 2c20 2741 6473 4c69 6e6b 5374  ats', 'AdsLinkSt
+00020750: 6174 7573 272c 2027 4164 734c 6f6f 6b61  atus', 'AdsLooka
+00020760: 6c69 6b65 5265 7175 6573 7427 2c20 2741  likeRequest', 'A
+00020770: 6473 4c6f 6f6b 616c 696b 6552 6571 7565  dsLookalikeReque
+00020780: 7374 5361 7665 4175 6469 656e 6365 4c65  stSaveAudienceLe
+00020790: 7665 6c27 2c20 2741 6473 4d75 7369 6369  vel', 'AdsMusici
+000207a0: 616e 272c 2027 4164 734f 626a 6563 7454  an', 'AdsObjectT
+000207b0: 7970 6527 2c20 2741 6473 5061 7261 6772  ype', 'AdsParagr
+000207c0: 6170 6873 272c 2027 4164 7350 726f 6d6f  aphs', 'AdsPromo
+000207d0: 7465 6450 6f73 7452 6561 6368 272c 2027  tedPostReach', '
+000207e0: 4164 7352 656a 6563 7452 6561 736f 6e27  AdsRejectReason'
+000207f0: 2c20 2741 6473 5275 6c65 7327 2c20 2741  , 'AdsRules', 'A
+00020800: 6473 5374 6174 7327 2c20 2741 6473 5374  dsStats', 'AdsSt
+00020810: 6174 7341 6765 272c 2027 4164 7353 7461  atsAge', 'AdsSta
+00020820: 7473 4369 7469 6573 272c 2027 4164 7353  tsCities', 'AdsS
+00020830: 7461 7473 466f 726d 6174 272c 2027 4164  tatsFormat', 'Ad
+00020840: 7353 7461 7473 5365 7827 2c20 2741 6473  sStatsSex', 'Ads
+00020850: 5374 6174 7353 6578 4167 6527 2c20 2741  StatsSexAge', 'A
+00020860: 6473 5374 6174 7353 6578 5661 6c75 6527  dsStatsSexValue'
+00020870: 2c20 2741 6473 5374 6174 7356 6965 7773  , 'AdsStatsViews
+00020880: 5469 6d65 7327 2c20 2741 6473 5461 7267  Times', 'AdsTarg
+00020890: 5365 7474 696e 6773 272c 2027 4164 7354  Settings', 'AdsT
+000208a0: 6172 6753 7461 7473 272c 2027 4164 7354  argStats', 'AdsT
+000208b0: 6172 6753 7567 6765 7374 696f 6e73 272c  argSuggestions',
+000208c0: 2027 4164 7354 6172 6753 7567 6765 7374   'AdsTargSuggest
+000208d0: 696f 6e73 4369 7469 6573 272c 2027 4164  ionsCities', 'Ad
+000208e0: 7354 6172 6753 7567 6765 7374 696f 6e73  sTargSuggestions
+000208f0: 5265 6769 6f6e 7327 2c20 2741 6473 5461  Regions', 'AdsTa
+00020900: 7267 5375 6767 6573 7469 6f6e 7353 6368  rgSuggestionsSch
+00020910: 6f6f 6c73 272c 2027 4164 7354 6172 6753  ools', 'AdsTargS
+00020920: 7567 6765 7374 696f 6e73 5363 686f 6f6c  uggestionsSchool
+00020930: 7354 7970 6527 2c20 2741 6473 5461 7267  sType', 'AdsTarg
+00020940: 6574 4772 6f75 7027 2c20 2741 6473 5570  etGroup', 'AdsUp
+00020950: 6461 7465 4f66 6669 6365 5573 6572 7352  dateOfficeUsersR
+00020960: 6573 756c 7427 2c20 2741 6473 5573 6572  esult', 'AdsUser
+00020970: 5370 6563 6966 6963 6174 696f 6e27 2c20  Specification', 
+00020980: 2741 6473 5573 6572 5370 6563 6966 6963  'AdsUserSpecific
+00020990: 6174 696f 6e43 7574 7465 6427 2c20 2741  ationCutted', 'A
+000209a0: 6473 5573 6572 7327 2c20 2741 6473 7765  dsUsers', 'Adswe
+000209b0: 6247 6574 4164 4361 7465 676f 7269 6573  bGetAdCategories
+000209c0: 5265 7370 6f6e 7365 4361 7465 676f 7269  ResponseCategori
+000209d0: 6573 4361 7465 676f 7279 272c 2027 4164  esCategory', 'Ad
+000209e0: 7377 6562 4765 7441 6455 6e69 7473 5265  swebGetAdUnitsRe
+000209f0: 7370 6f6e 7365 4164 556e 6974 7341 6455  sponseAdUnitsAdU
+00020a00: 6e69 7427 2c20 2741 6473 7765 6247 6574  nit', 'AdswebGet
+00020a10: 4672 6175 6448 6973 746f 7279 5265 7370  FraudHistoryResp
+00020a20: 6f6e 7365 456e 7472 6965 7345 6e74 7279  onseEntriesEntry
+00020a30: 272c 2027 4164 7377 6562 4765 7453 6974  ', 'AdswebGetSit
+00020a40: 6573 5265 7370 6f6e 7365 5369 7465 7353  esResponseSitesS
+00020a50: 6974 6527 2c20 2741 6473 7765 6247 6574  ite', 'AdswebGet
+00020a60: 5374 6174 6973 7469 6373 5265 7370 6f6e  StatisticsRespon
+00020a70: 7365 4974 656d 7349 7465 6d27 2c20 2741  seItemsItem', 'A
+00020a80: 7070 5769 6467 6574 7350 686f 746f 272c  ppWidgetsPhoto',
+00020a90: 2027 4170 7057 6964 6765 7473 5068 6f74   'AppWidgetsPhot
+00020aa0: 6f73 272c 2027 4170 7073 4170 7027 2c20  os', 'AppsApp', 
+00020ab0: 2741 7070 7341 7070 4c65 6164 6572 626f  'AppsAppLeaderbo
+00020ac0: 6172 6454 7970 6527 2c20 2741 7070 7341  ardType', 'AppsA
+00020ad0: 7070 4d69 6e27 2c20 2741 7070 7341 7070  ppMin', 'AppsApp
+00020ae0: 5479 7065 272c 2027 4170 7073 4361 7461  Type', 'AppsCata
+00020af0: 6c6f 674c 6973 7427 2c20 2741 7070 734c  logList', 'AppsL
+00020b00: 6561 6465 7262 6f61 7264 272c 2027 4170  eaderboard', 'Ap
+00020b10: 7073 5363 6f70 6527 2c20 2741 7564 696f  psScope', 'Audio
+00020b20: 4175 6469 6f27 2c20 2762 6f6f 6c27 2c20  Audio', 'bool', 
+00020b30: 2742 6173 6543 6974 7927 2c20 2742 6173  'BaseCity', 'Bas
+00020b40: 6543 6f6d 6d65 6e74 7349 6e66 6f27 2c20  eCommentsInfo', 
+00020b50: 2742 6173 6543 6f75 6e74 7279 272c 2027  'BaseCountry', '
+00020b60: 4261 7365 4372 6f70 5068 6f74 6f27 2c20  BaseCropPhoto', 
+00020b70: 2742 6173 6543 726f 7050 686f 746f 4372  'BaseCropPhotoCr
+00020b80: 6f70 272c 2027 4261 7365 4372 6f70 5068  op', 'BaseCropPh
+00020b90: 6f74 6f52 6563 7427 2c20 2742 6173 6545  otoRect', 'BaseE
+00020ba0: 7272 6f72 272c 2027 4261 7365 4765 6f27  rror', 'BaseGeo'
+00020bb0: 2c20 2742 6173 6547 656f 436f 6f72 6469  , 'BaseGeoCoordi
+00020bc0: 6e61 7465 7327 2c20 2742 6173 6547 7261  nates', 'BaseGra
+00020bd0: 6469 656e 7450 6f69 6e74 272c 2027 4261  dientPoint', 'Ba
+00020be0: 7365 496d 6167 6527 2c20 2742 6173 654c  seImage', 'BaseL
+00020bf0: 696b 6573 272c 2027 4261 7365 4c69 6b65  ikes', 'BaseLike
+00020c00: 7349 6e66 6f27 2c20 2742 6173 654c 696e  sInfo', 'BaseLin
+00020c10: 6b27 2c20 2742 6173 654c 696e 6b41 7070  k', 'BaseLinkApp
+00020c20: 6c69 6361 7469 6f6e 272c 2027 4261 7365  lication', 'Base
+00020c30: 4c69 6e6b 4170 706c 6963 6174 696f 6e53  LinkApplicationS
+00020c40: 746f 7265 272c 2027 4261 7365 4c69 6e6b  tore', 'BaseLink
+00020c50: 4275 7474 6f6e 272c 2027 4261 7365 4c69  Button', 'BaseLi
+00020c60: 6e6b 4275 7474 6f6e 4163 7469 6f6e 272c  nkButtonAction',
+00020c70: 2027 4261 7365 4c69 6e6b 4275 7474 6f6e   'BaseLinkButton
+00020c80: 4163 7469 6f6e 5479 7065 272c 2027 4261  ActionType', 'Ba
+00020c90: 7365 4c69 6e6b 4275 7474 6f6e 5374 796c  seLinkButtonStyl
+00020ca0: 6527 2c20 2742 6173 654c 696e 6b50 726f  e', 'BaseLinkPro
+00020cb0: 6475 6374 272c 2027 4261 7365 4c69 6e6b  duct', 'BaseLink
+00020cc0: 5072 6f64 7563 7443 6174 6567 6f72 7927  ProductCategory'
+00020cd0: 2c20 2742 6173 654c 696e 6b50 726f 6475  , 'BaseLinkProdu
+00020ce0: 6374 5374 6174 7573 272c 2027 4261 7365  ctStatus', 'Base
+00020cf0: 4c69 6e6b 5261 7469 6e67 272c 2027 4261  LinkRating', 'Ba
+00020d00: 7365 4d65 7373 6167 6545 7272 6f72 272c  seMessageError',
+00020d10: 2027 4261 7365 4f62 6a65 6374 272c 2027   'BaseObject', '
+00020d20: 4261 7365 4f62 6a65 6374 436f 756e 7427  BaseObjectCount'
+00020d30: 2c20 2742 6173 654f 626a 6563 7457 6974  , 'BaseObjectWit
+00020d40: 684e 616d 6527 2c20 2742 6173 6550 6c61  hName', 'BasePla
+00020d50: 6365 272c 2027 4261 7365 5072 6f70 6572  ce', 'BaseProper
+00020d60: 7479 4578 6973 7473 272c 2027 4261 7365  tyExists', 'Base
+00020d70: 5265 706f 7374 7349 6e66 6f27 2c20 2742  RepostsInfo', 'B
+00020d80: 6173 6552 6571 7565 7374 5061 7261 6d27  aseRequestParam'
+00020d90: 2c20 2742 6173 6553 6578 272c 2027 4261  , 'BaseSex', 'Ba
+00020da0: 7365 5374 6963 6b65 7227 2c20 2742 6173  seSticker', 'Bas
+00020db0: 6553 7469 636b 6572 416e 696d 6174 696f  eStickerAnimatio
+00020dc0: 6e27 2c20 2742 6173 6553 7469 636b 6572  n', 'BaseSticker
+00020dd0: 4e65 7727 2c20 2742 6173 6553 7469 636b  New', 'BaseStick
+00020de0: 6572 4f6c 6427 2c20 2742 6173 6553 7469  erOld', 'BaseSti
+00020df0: 636b 6572 734c 6973 7427 2c20 2742 6173  ckersList', 'Bas
+00020e00: 6555 706c 6f61 6453 6572 7665 7227 2c20  eUploadServer', 
+00020e10: 2742 6173 6555 7365 7247 726f 7570 4669  'BaseUserGroupFi
+00020e20: 656c 6473 272c 2027 4261 7365 5573 6572  elds', 'BaseUser
+00020e30: 4964 272c 2027 426f 6172 6444 6566 6175  Id', 'BoardDefau
+00020e40: 6c74 4f72 6465 7227 2c20 2742 6f61 7264  ltOrder', 'Board
+00020e50: 546f 7069 6327 2c20 2742 6f61 7264 546f  Topic', 'BoardTo
+00020e60: 7069 6343 6f6d 6d65 6e74 272c 2027 4361  picComment', 'Ca
+00020e70: 6c6c 6261 636b 4261 7365 272c 2027 4361  llbackBase', 'Ca
+00020e80: 6c6c 6261 636b 426f 6172 6450 6f73 7444  llbackBoardPostD
+00020e90: 656c 6574 6527 2c20 2743 616c 6c62 6163  elete', 'Callbac
+00020ea0: 6b43 6f6e 6669 726d 6174 696f 6e27 2c20  kConfirmation', 
+00020eb0: 2743 616c 6c62 6163 6b44 6f6e 7574 4d6f  'CallbackDonutMo
+00020ec0: 6e65 7957 6974 6864 7261 7727 2c20 2743  neyWithdraw', 'C
+00020ed0: 616c 6c62 6163 6b44 6f6e 7574 4d6f 6e65  allbackDonutMone
+00020ee0: 7957 6974 6864 7261 7745 7272 6f72 272c  yWithdrawError',
+00020ef0: 2027 4361 6c6c 6261 636b 446f 6e75 7453   'CallbackDonutS
+00020f00: 7562 7363 7269 7074 696f 6e43 616e 6365  ubscriptionCance
+00020f10: 6c6c 6564 272c 2027 4361 6c6c 6261 636b  lled', 'Callback
+00020f20: 446f 6e75 7453 7562 7363 7269 7074 696f  DonutSubscriptio
+00020f30: 6e43 7265 6174 6527 2c20 2743 616c 6c62  nCreate', 'Callb
+00020f40: 6163 6b44 6f6e 7574 5375 6273 6372 6970  ackDonutSubscrip
+00020f50: 7469 6f6e 4578 7069 7265 6427 2c20 2743  tionExpired', 'C
+00020f60: 616c 6c62 6163 6b44 6f6e 7574 5375 6273  allbackDonutSubs
+00020f70: 6372 6970 7469 6f6e 5072 6963 6543 6861  criptionPriceCha
+00020f80: 6e67 6564 272c 2027 4361 6c6c 6261 636b  nged', 'Callback
+00020f90: 446f 6e75 7453 7562 7363 7269 7074 696f  DonutSubscriptio
+00020fa0: 6e50 726f 6c6f 6e67 6564 272c 2027 4361  nProlonged', 'Ca
+00020fb0: 6c6c 6261 636b 4772 6f75 7043 6861 6e67  llbackGroupChang
+00020fc0: 6550 686f 746f 272c 2027 4361 6c6c 6261  ePhoto', 'Callba
+00020fd0: 636b 4772 6f75 7043 6861 6e67 6553 6574  ckGroupChangeSet
+00020fe0: 7469 6e67 7327 2c20 2743 616c 6c62 6163  tings', 'Callbac
+00020ff0: 6b47 726f 7570 4a6f 696e 272c 2027 4361  kGroupJoin', 'Ca
+00021000: 6c6c 6261 636b 4772 6f75 704a 6f69 6e54  llbackGroupJoinT
+00021010: 7970 6527 2c20 2743 616c 6c62 6163 6b47  ype', 'CallbackG
+00021020: 726f 7570 4c65 6176 6527 2c20 2743 616c  roupLeave', 'Cal
+00021030: 6c62 6163 6b47 726f 7570 4d61 726b 6574  lbackGroupMarket
+00021040: 272c 2027 4361 6c6c 6261 636b 4772 6f75  ', 'CallbackGrou
+00021050: 704f 6666 6963 6572 526f 6c65 272c 2027  pOfficerRole', '
+00021060: 4361 6c6c 6261 636b 4772 6f75 704f 6666  CallbackGroupOff
+00021070: 6963 6572 7345 6469 7427 2c20 2743 616c  icersEdit', 'Cal
+00021080: 6c62 6163 6b47 726f 7570 5365 7474 696e  lbackGroupSettin
+00021090: 6773 4368 616e 6765 7327 2c20 2743 616c  gsChanges', 'Cal
+000210a0: 6c62 6163 6b4c 696b 6541 6464 5265 6d6f  lbackLikeAddRemo
+000210b0: 7665 272c 2027 4361 6c6c 6261 636b 4d61  ve', 'CallbackMa
+000210c0: 726b 6574 436f 6d6d 656e 7427 2c20 2743  rketComment', 'C
+000210d0: 616c 6c62 6163 6b4d 6172 6b65 7443 6f6d  allbackMarketCom
+000210e0: 6d65 6e74 4465 6c65 7465 272c 2027 4361  mentDelete', 'Ca
+000210f0: 6c6c 6261 636b 4d65 7373 6167 6541 6c6c  llbackMessageAll
+00021100: 6f77 272c 2027 4361 6c6c 6261 636b 4d65  ow', 'CallbackMe
+00021110: 7373 6167 6541 6c6c 6f77 4f62 6a65 6374  ssageAllowObject
+00021120: 272c 2027 4361 6c6c 6261 636b 4d65 7373  ', 'CallbackMess
+00021130: 6167 6544 656e 7927 2c20 2743 616c 6c62  ageDeny', 'Callb
+00021140: 6163 6b4d 6573 7361 6765 4564 6974 272c  ackMessageEdit',
+00021150: 2027 4361 6c6c 6261 636b 4d65 7373 6167   'CallbackMessag
+00021160: 654e 6577 272c 2027 4361 6c6c 6261 636b  eNew', 'Callback
+00021170: 4d65 7373 6167 654f 626a 6563 7427 2c20  MessageObject', 
+00021180: 2743 616c 6c62 6163 6b4d 6573 7361 6765  'CallbackMessage
+00021190: 5265 706c 7927 2c20 2743 616c 6c62 6163  Reply', 'Callbac
+000211a0: 6b50 686f 746f 436f 6d6d 656e 7427 2c20  kPhotoComment', 
+000211b0: 2743 616c 6c62 6163 6b50 686f 746f 436f  'CallbackPhotoCo
+000211c0: 6d6d 656e 7444 656c 6574 6527 2c20 2743  mmentDelete', 'C
+000211d0: 616c 6c62 6163 6b50 6f6c 6c56 6f74 654e  allbackPollVoteN
+000211e0: 6577 272c 2027 4361 6c6c 6261 636b 5172  ew', 'CallbackQr
+000211f0: 5363 616e 272c 2027 4361 6c6c 6261 636b  Scan', 'Callback
+00021200: 5479 7065 272c 2027 4361 6c6c 6261 636b  Type', 'Callback
+00021210: 5573 6572 426c 6f63 6b27 2c20 2743 616c  UserBlock', 'Cal
+00021220: 6c62 6163 6b55 7365 7255 6e62 6c6f 636b  lbackUserUnblock
+00021230: 272c 2027 4361 6c6c 6261 636b 5669 6465  ', 'CallbackVide
+00021240: 6f43 6f6d 6d65 6e74 272c 2027 4361 6c6c  oComment', 'Call
+00021250: 6261 636b 5669 6465 6f43 6f6d 6d65 6e74  backVideoComment
+00021260: 4465 6c65 7465 272c 2027 4361 6c6c 6261  Delete', 'Callba
+00021270: 636b 5761 6c6c 436f 6d6d 656e 7444 656c  ckWallCommentDel
+00021280: 6574 6527 2c20 2743 616c 6c73 4361 6c6c  ete', 'CallsCall
+00021290: 272c 2027 4361 6c6c 7345 6e64 5374 6174  ', 'CallsEndStat
+000212a0: 6527 2c20 2743 616c 6c73 5061 7274 6963  e', 'CallsPartic
+000212b0: 6970 616e 7473 272c 2027 436c 6965 6e74  ipants', 'Client
+000212c0: 496e 666f 466f 7242 6f74 7327 2c20 2743  InfoForBots', 'C
+000212d0: 6f6d 6d65 6e74 5468 7265 6164 272c 2027  ommentThread', '
+000212e0: 4461 7461 6261 7365 4369 7479 272c 2027  DatabaseCity', '
+000212f0: 4461 7461 6261 7365 4369 7479 4279 4964  DatabaseCityById
+00021300: 272c 2027 4461 7461 6261 7365 4661 6375  ', 'DatabaseFacu
+00021310: 6c74 7927 2c20 2744 6174 6162 6173 6552  lty', 'DatabaseR
+00021320: 6567 696f 6e27 2c20 2744 6174 6162 6173  egion', 'Databas
+00021330: 6553 6368 6f6f 6c27 2c20 2744 6174 6162  eSchool', 'Datab
+00021340: 6173 6553 7461 7469 6f6e 272c 2027 4461  aseStation', 'Da
+00021350: 7461 6261 7365 556e 6976 6572 7369 7479  tabaseUniversity
+00021360: 272c 2027 446f 6373 446f 6327 2c20 2744  ', 'DocsDoc', 'D
+00021370: 6f63 7344 6f63 4174 7461 6368 6d65 6e74  ocsDocAttachment
+00021380: 5479 7065 272c 2027 446f 6373 446f 6350  Type', 'DocsDocP
+00021390: 7265 7669 6577 272c 2027 446f 6373 446f  review', 'DocsDo
+000213a0: 6350 7265 7669 6577 4175 6469 6f4d 7367  cPreviewAudioMsg
 000213b0: 272c 2027 446f 6373 446f 6350 7265 7669  ', 'DocsDocPrevi
-000213c0: 6577 5068 6f74 6f27 2c20 2744 6f63 7344  ewPhoto', 'DocsD
-000213d0: 6f63 5072 6576 6965 7750 686f 746f 5369  ocPreviewPhotoSi
-000213e0: 7a65 7327 2c20 2744 6f63 7344 6f63 5072  zes', 'DocsDocPr
-000213f0: 6576 6965 7756 6964 656f 272c 2027 446f  eviewVideo', 'Do
-00021400: 6373 446f 6354 7970 6573 272c 2027 446f  csDocTypes', 'Do
-00021410: 6e75 7444 6f6e 6174 6f72 5375 6273 6372  nutDonatorSubscr
-00021420: 6970 7469 6f6e 496e 666f 272c 2027 4576  iptionInfo', 'Ev
-00021430: 656e 7473 4576 656e 7441 7474 6163 6827  entsEventAttach'
-00021440: 2c20 2746 6176 6542 6f6f 6b6d 6172 6b27  , 'FaveBookmark'
-00021450: 2c20 2746 6176 6542 6f6f 6b6d 6172 6b54  , 'FaveBookmarkT
-00021460: 7970 6527 2c20 2746 6176 6550 6167 6527  ype', 'FavePage'
-00021470: 2c20 2746 6176 6550 6167 6554 7970 6527  , 'FavePageType'
-00021480: 2c20 2746 6176 6554 6167 272c 2027 4672  , 'FaveTag', 'Fr
-00021490: 6965 6e64 7346 7269 656e 6445 7874 656e  iendsFriendExten
-000214a0: 6465 6453 7461 7475 7327 2c20 2746 7269  dedStatus', 'Fri
-000214b0: 656e 6473 4672 6965 6e64 5374 6174 7573  endsFriendStatus
-000214c0: 272c 2027 4672 6965 6e64 7346 7269 656e  ', 'FriendsFrien
-000214d0: 6453 7461 7475 7353 7461 7475 7327 2c20  dStatusStatus', 
-000214e0: 2746 7269 656e 6473 4672 6965 6e64 734c  'FriendsFriendsL
-000214f0: 6973 7427 2c20 2746 7269 656e 6473 4d75  ist', 'FriendsMu
-00021500: 7475 616c 4672 6965 6e64 272c 2027 4672  tualFriend', 'Fr
-00021510: 6965 6e64 7352 6571 7565 7374 7327 2c20  iendsRequests', 
-00021520: 2746 7269 656e 6473 5265 7175 6573 7473  'FriendsRequests
-00021530: 4d75 7475 616c 272c 2027 4672 6965 6e64  Mutual', 'Friend
-00021540: 7352 6571 7565 7374 7358 7472 4d65 7373  sRequestsXtrMess
-00021550: 6167 6527 2c20 2746 7269 656e 6473 5573  age', 'FriendsUs
-00021560: 6572 5874 7250 686f 6e65 272c 2027 4769  erXtrPhone', 'Gi
-00021570: 6674 7347 6966 7427 2c20 2747 6966 7473  ftsGift', 'Gifts
-00021580: 4769 6674 5072 6976 6163 7927 2c20 2747  GiftPrivacy', 'G
-00021590: 6966 7473 4c61 796f 7574 272c 2027 4772  iftsLayout', 'Gr
-000215a0: 6f75 7073 4164 6472 6573 7327 2c20 2747  oupsAddress', 'G
-000215b0: 726f 7570 7341 6464 7265 7373 5469 6d65  roupsAddressTime
-000215c0: 7461 626c 6527 2c20 2747 726f 7570 7341  table', 'GroupsA
-000215d0: 6464 7265 7373 5469 6d65 7461 626c 6544  ddressTimetableD
-000215e0: 6179 272c 2027 4772 6f75 7073 4164 6472  ay', 'GroupsAddr
-000215f0: 6573 7357 6f72 6b49 6e66 6f53 7461 7475  essWorkInfoStatu
-00021600: 7327 2c20 2747 726f 7570 7341 6464 7265  s', 'GroupsAddre
-00021610: 7373 6573 496e 666f 272c 2027 4772 6f75  ssesInfo', 'Grou
-00021620: 7073 4261 6e49 6e66 6f27 2c20 2747 726f  psBanInfo', 'Gro
-00021630: 7570 7342 616e 496e 666f 5265 6173 6f6e  upsBanInfoReason
-00021640: 272c 2027 4772 6f75 7073 4261 6e6e 6564  ', 'GroupsBanned
-00021650: 4974 656d 272c 2027 4772 6f75 7073 4361  Item', 'GroupsCa
-00021660: 6c6c 6261 636b 5365 7276 6572 272c 2027  llbackServer', '
-00021670: 4772 6f75 7073 4361 6c6c 6261 636b 5365  GroupsCallbackSe
-00021680: 7474 696e 6773 272c 2027 4772 6f75 7073  ttings', 'Groups
-00021690: 436f 6e74 6163 7473 4974 656d 272c 2027  ContactsItem', '
-000216a0: 4772 6f75 7073 436f 756e 7465 7273 4772  GroupsCountersGr
-000216b0: 6f75 7027 2c20 2747 726f 7570 7343 6f76  oup', 'GroupsCov
-000216c0: 6572 272c 2027 4772 6f75 7073 4669 656c  er', 'GroupsFiel
-000216d0: 6473 272c 2027 4772 6f75 7073 4669 6c74  ds', 'GroupsFilt
-000216e0: 6572 272c 2027 4772 6f75 7073 4772 6f75  er', 'GroupsGrou
-000216f0: 7027 2c20 2747 726f 7570 7347 726f 7570  p', 'GroupsGroup
-00021700: 4163 6365 7373 272c 2027 4772 6f75 7073  Access', 'Groups
-00021710: 4772 6f75 7041 646d 696e 4c65 7665 6c27  GroupAdminLevel'
-00021720: 2c20 2747 726f 7570 7347 726f 7570 4167  , 'GroupsGroupAg
-00021730: 654c 696d 6974 7327 2c20 2747 726f 7570  eLimits', 'Group
-00021740: 7347 726f 7570 4174 7461 6368 272c 2027  sGroupAttach', '
-00021750: 4772 6f75 7073 4772 6f75 7041 7564 696f  GroupsGroupAudio
-00021760: 272c 2027 4772 6f75 7073 4772 6f75 7042  ', 'GroupsGroupB
-00021770: 616e 496e 666f 272c 2027 4772 6f75 7073  anInfo', 'Groups
-00021780: 4772 6f75 7043 6174 6567 6f72 7927 2c20  GroupCategory', 
-00021790: 2747 726f 7570 7347 726f 7570 4361 7465  'GroupsGroupCate
-000217a0: 676f 7279 4675 6c6c 272c 2027 4772 6f75  goryFull', 'Grou
-000217b0: 7073 4772 6f75 7043 6174 6567 6f72 7954  psGroupCategoryT
-000217c0: 7970 6527 2c20 2747 726f 7570 7347 726f  ype', 'GroupsGro
-000217d0: 7570 446f 6373 272c 2027 4772 6f75 7073  upDocs', 'Groups
-000217e0: 4772 6f75 7046 756c 6c27 2c20 2747 726f  GroupFull', 'Gro
-000217f0: 7570 7347 726f 7570 4675 6c6c 4167 654c  upsGroupFullAgeL
-00021800: 696d 6974 7327 2c20 2747 726f 7570 7347  imits', 'GroupsG
-00021810: 726f 7570 4675 6c6c 4d65 6d62 6572 5374  roupFullMemberSt
-00021820: 6174 7573 272c 2027 4772 6f75 7073 4772  atus', 'GroupsGr
-00021830: 6f75 7046 756c 6c53 6563 7469 6f6e 272c  oupFullSection',
-00021840: 2027 4772 6f75 7073 4772 6f75 7049 7343   'GroupsGroupIsC
-00021850: 6c6f 7365 6427 2c20 2747 726f 7570 7347  losed', 'GroupsG
-00021860: 726f 7570 4d61 726b 6574 4375 7272 656e  roupMarketCurren
-00021870: 6379 272c 2027 4772 6f75 7073 4772 6f75  cy', 'GroupsGrou
-00021880: 7050 686f 746f 7327 2c20 2747 726f 7570  pPhotos', 'Group
-00021890: 7347 726f 7570 5075 626c 6963 4361 7465  sGroupPublicCate
-000218a0: 676f 7279 4c69 7374 272c 2027 4772 6f75  goryList', 'Grou
-000218b0: 7073 4772 6f75 7052 6f6c 6527 2c20 2747  psGroupRole', 'G
-000218c0: 726f 7570 7347 726f 7570 5375 626a 6563  roupsGroupSubjec
-000218d0: 7427 2c20 2747 726f 7570 7347 726f 7570  t', 'GroupsGroup
-000218e0: 5375 6767 6573 7465 6450 7269 7661 6379  SuggestedPrivacy
-000218f0: 272c 2027 4772 6f75 7073 4772 6f75 7054  ', 'GroupsGroupT
-00021900: 6167 272c 2027 4772 6f75 7073 4772 6f75  ag', 'GroupsGrou
-00021910: 7054 6f70 6963 7327 2c20 2747 726f 7570  pTopics', 'Group
-00021920: 7347 726f 7570 5479 7065 272c 2027 4772  sGroupType', 'Gr
-00021930: 6f75 7073 4772 6f75 7056 6964 656f 272c  oupsGroupVideo',
-00021940: 2027 4772 6f75 7073 4772 6f75 7057 616c   'GroupsGroupWal
-00021950: 6c27 2c20 2747 726f 7570 7347 726f 7570  l', 'GroupsGroup
-00021960: 5769 6b69 272c 2027 4772 6f75 7073 4772  Wiki', 'GroupsGr
-00021970: 6f75 7073 4172 7261 7927 2c20 2747 726f  oupsArray', 'Gro
-00021980: 7570 734c 696e 6b73 4974 656d 272c 2027  upsLinksItem', '
-00021990: 4772 6f75 7073 4c69 7665 436f 7665 7273  GroupsLiveCovers
-000219a0: 272c 2027 4772 6f75 7073 4c6f 6e67 506f  ', 'GroupsLongPo
-000219b0: 6c6c 4576 656e 7473 272c 2027 4772 6f75  llEvents', 'Grou
-000219c0: 7073 4c6f 6e67 506f 6c6c 5365 7276 6572  psLongPollServer
-000219d0: 272c 2027 4772 6f75 7073 4c6f 6e67 506f  ', 'GroupsLongPo
-000219e0: 6c6c 5365 7474 696e 6773 272c 2027 4772  llSettings', 'Gr
-000219f0: 6f75 7073 4d61 726b 6574 496e 666f 272c  oupsMarketInfo',
-00021a00: 2027 4772 6f75 7073 4d61 726b 6574 5374   'GroupsMarketSt
-00021a10: 6174 6527 2c20 2747 726f 7570 734d 656d  ate', 'GroupsMem
-00021a20: 6265 7252 6f6c 6527 2c20 2747 726f 7570  berRole', 'Group
-00021a30: 734d 656d 6265 7252 6f6c 6550 6572 6d69  sMemberRolePermi
-00021a40: 7373 696f 6e27 2c20 2747 726f 7570 734d  ssion', 'GroupsM
-00021a50: 656d 6265 7252 6f6c 6553 7461 7475 7327  emberRoleStatus'
-00021a60: 2c20 2747 726f 7570 734d 656d 6265 7253  , 'GroupsMemberS
-00021a70: 7461 7475 7327 2c20 2747 726f 7570 734d  tatus', 'GroupsM
-00021a80: 656d 6265 7253 7461 7475 7346 756c 6c27  emberStatusFull'
-00021a90: 2c20 2747 726f 7570 734f 6e6c 696e 6553  , 'GroupsOnlineS
-00021aa0: 7461 7475 7327 2c20 2747 726f 7570 734f  tatus', 'GroupsO
-00021ab0: 6e6c 696e 6553 7461 7475 7354 7970 6527  nlineStatusType'
-00021ac0: 2c20 2747 726f 7570 734f 776e 6572 5874  , 'GroupsOwnerXt
-00021ad0: 7242 616e 496e 666f 272c 2027 4772 6f75  rBanInfo', 'Grou
-00021ae0: 7073 4f77 6e65 7258 7472 4261 6e49 6e66  psOwnerXtrBanInf
-00021af0: 6f54 7970 6527 2c20 2747 726f 7570 7350  oType', 'GroupsP
-00021b00: 686f 746f 5369 7a65 272c 2027 4772 6f75  hotoSize', 'Grou
-00021b10: 7073 526f 6c65 4f70 7469 6f6e 7327 2c20  psRoleOptions', 
-00021b20: 2747 726f 7570 7353 6563 7469 6f6e 734c  'GroupsSectionsL
-00021b30: 6973 7449 7465 6d27 2c20 2747 726f 7570  istItem', 'Group
-00021b40: 7353 6574 7469 6e67 7354 7769 7474 6572  sSettingsTwitter
-00021b50: 272c 2027 4772 6f75 7073 5375 626a 6563  ', 'GroupsSubjec
-00021b60: 7449 7465 6d27 2c20 2747 726f 7570 7354  tItem', 'GroupsT
-00021b70: 6f6b 656e 5065 726d 6973 7369 6f6e 5365  okenPermissionSe
-00021b80: 7474 696e 6727 2c20 2747 726f 7570 7355  tting', 'GroupsU
-00021b90: 7365 7258 7472 526f 6c65 272c 2027 4c65  serXtrRole', 'Le
-00021ba0: 6164 466f 726d 7341 6e73 7765 7227 2c20  adFormsAnswer', 
-00021bb0: 274c 6561 6446 6f72 6d73 416e 7377 6572  'LeadFormsAnswer
-00021bc0: 4974 656d 272c 2027 4c65 6164 466f 726d  Item', 'LeadForm
-00021bd0: 7346 6f72 6d27 2c20 274c 6561 6446 6f72  sForm', 'LeadFor
-00021be0: 6d73 4c65 6164 272c 2027 4c65 6164 466f  msLead', 'LeadFo
-00021bf0: 726d 7351 7565 7374 696f 6e49 7465 6d27  rmsQuestionItem'
-00021c00: 2c20 274c 6561 6446 6f72 6d73 5175 6573  , 'LeadFormsQues
-00021c10: 7469 6f6e 4974 656d 4f70 7469 6f6e 272c  tionItemOption',
-00021c20: 2027 4c69 6b65 7354 7970 6527 2c20 274c   'LikesType', 'L
-00021c30: 696e 6b54 6172 6765 744f 626a 6563 7427  inkTargetObject'
-00021c40: 2c20 274d 6172 6b65 7443 7572 7265 6e63  , 'MarketCurrenc
-00021c50: 7927 2c20 274d 6172 6b65 744d 6172 6b65  y', 'MarketMarke
-00021c60: 7441 6c62 756d 272c 2027 4d61 726b 6574  tAlbum', 'Market
-00021c70: 4d61 726b 6574 4361 7465 676f 7279 272c  MarketCategory',
-00021c80: 2027 4d61 726b 6574 4d61 726b 6574 4361   'MarketMarketCa
-00021c90: 7465 676f 7279 4e65 7374 6564 272c 2027  tegoryNested', '
-00021ca0: 4d61 726b 6574 4d61 726b 6574 4361 7465  MarketMarketCate
-00021cb0: 676f 7279 4f6c 6427 2c20 274d 6172 6b65  goryOld', 'Marke
-00021cc0: 744d 6172 6b65 7443 6174 6567 6f72 7954  tMarketCategoryT
-00021cd0: 7265 6527 2c20 274d 6172 6b65 744d 6172  ree', 'MarketMar
-00021ce0: 6b65 7449 7465 6d27 2c20 274d 6172 6b65  ketItem', 'Marke
-00021cf0: 744d 6172 6b65 7449 7465 6d41 7661 696c  tMarketItemAvail
-00021d00: 6162 696c 6974 7927 2c20 274d 6172 6b65  ability', 'Marke
-00021d10: 744d 6172 6b65 7449 7465 6d46 756c 6c27  tMarketItemFull'
-00021d20: 2c20 274d 6172 6b65 744f 7264 6572 272c  , 'MarketOrder',
-00021d30: 2027 4d61 726b 6574 4f72 6465 7249 7465   'MarketOrderIte
-00021d40: 6d27 2c20 274d 6172 6b65 7450 7269 6365  m', 'MarketPrice
-00021d50: 272c 2027 4d61 726b 6574 5365 6374 696f  ', 'MarketSectio
-00021d60: 6e27 2c20 274d 6172 6b65 7453 6572 7669  n', 'MarketServi
-00021d70: 6365 7356 6965 7754 7970 6527 2c20 274d  cesViewType', 'M
-00021d80: 6573 7361 6765 7341 7564 696f 4d65 7373  essagesAudioMess
-00021d90: 6167 6527 2c20 274d 6573 7361 6765 7343  age', 'MessagesC
-00021da0: 6861 7427 2c20 274d 6573 7361 6765 7343  hat', 'MessagesC
-00021db0: 6861 7446 756c 6c27 2c20 274d 6573 7361  hatFull', 'Messa
-00021dc0: 6765 7343 6861 7450 7265 7669 6577 272c  gesChatPreview',
-00021dd0: 2027 4d65 7373 6167 6573 4368 6174 5075   'MessagesChatPu
-00021de0: 7368 5365 7474 696e 6773 272c 2027 4d65  shSettings', 'Me
-00021df0: 7373 6167 6573 4368 6174 5265 7374 7269  ssagesChatRestri
-00021e00: 6374 696f 6e73 272c 2027 4d65 7373 6167  ctions', 'Messag
-00021e10: 6573 4368 6174 5365 7474 696e 6773 272c  esChatSettings',
-00021e20: 2027 4d65 7373 6167 6573 4368 6174 5365   'MessagesChatSe
-00021e30: 7474 696e 6773 4163 6c27 2c20 274d 6573  ttingsAcl', 'Mes
-00021e40: 7361 6765 7343 6861 7453 6574 7469 6e67  sagesChatSetting
-00021e50: 7350 6572 6d69 7373 696f 6e73 272c 2027  sPermissions', '
-00021e60: 4d65 7373 6167 6573 4368 6174 5365 7474  MessagesChatSett
-00021e70: 696e 6773 5068 6f74 6f27 2c20 274d 6573  ingsPhoto', 'Mes
-00021e80: 7361 6765 7343 6861 7453 6574 7469 6e67  sagesChatSetting
-00021e90: 7353 7461 7465 272c 2027 4d65 7373 6167  sState', 'Messag
-00021ea0: 6573 436f 6e76 6572 7361 7469 6f6e 272c  esConversation',
-00021eb0: 2027 4d65 7373 6167 6573 436f 6e76 6572   'MessagesConver
-00021ec0: 7361 7469 6f6e 4361 6e57 7269 7465 272c  sationCanWrite',
-00021ed0: 2027 4d65 7373 6167 6573 436f 6e76 6572   'MessagesConver
-00021ee0: 7361 7469 6f6e 4d65 6d62 6572 272c 2027  sationMember', '
-00021ef0: 4d65 7373 6167 6573 436f 6e76 6572 7361  MessagesConversa
-00021f00: 7469 6f6e 5065 6572 272c 2027 4d65 7373  tionPeer', 'Mess
-00021f10: 6167 6573 436f 6e76 6572 7361 7469 6f6e  agesConversation
-00021f20: 5065 6572 5479 7065 272c 2027 4d65 7373  PeerType', 'Mess
-00021f30: 6167 6573 436f 6e76 6572 7361 7469 6f6e  agesConversation
-00021f40: 536f 7274 4964 272c 2027 4d65 7373 6167  SortId', 'Messag
-00021f50: 6573 436f 6e76 6572 7361 7469 6f6e 5769  esConversationWi
-00021f60: 7468 4d65 7373 6167 6527 2c20 274d 6573  thMessage', 'Mes
-00021f70: 7361 6765 7346 6f72 6569 676e 4d65 7373  sagesForeignMess
+000213c0: 6577 4772 6166 6669 7469 272c 2027 446f  ewGraffiti', 'Do
+000213d0: 6373 446f 6350 7265 7669 6577 5068 6f74  csDocPreviewPhot
+000213e0: 6f27 2c20 2744 6f63 7344 6f63 5072 6576  o', 'DocsDocPrev
+000213f0: 6965 7750 686f 746f 5369 7a65 7327 2c20  iewPhotoSizes', 
+00021400: 2744 6f63 7344 6f63 5072 6576 6965 7756  'DocsDocPreviewV
+00021410: 6964 656f 272c 2027 446f 6373 446f 6354  ideo', 'DocsDocT
+00021420: 7970 6573 272c 2027 446f 6e75 7444 6f6e  ypes', 'DonutDon
+00021430: 6174 6f72 5375 6273 6372 6970 7469 6f6e  atorSubscription
+00021440: 496e 666f 272c 2027 4576 656e 7473 4576  Info', 'EventsEv
+00021450: 656e 7441 7474 6163 6827 2c20 2746 6176  entAttach', 'Fav
+00021460: 6542 6f6f 6b6d 6172 6b27 2c20 2746 6176  eBookmark', 'Fav
+00021470: 6542 6f6f 6b6d 6172 6b54 7970 6527 2c20  eBookmarkType', 
+00021480: 2746 6176 6550 6167 6527 2c20 2746 6176  'FavePage', 'Fav
+00021490: 6550 6167 6554 7970 6527 2c20 2746 6176  ePageType', 'Fav
+000214a0: 6554 6167 272c 2027 4672 6965 6e64 7346  eTag', 'FriendsF
+000214b0: 7269 656e 6445 7874 656e 6465 6453 7461  riendExtendedSta
+000214c0: 7475 7327 2c20 2746 7269 656e 6473 4672  tus', 'FriendsFr
+000214d0: 6965 6e64 5374 6174 7573 272c 2027 4672  iendStatus', 'Fr
+000214e0: 6965 6e64 7346 7269 656e 6453 7461 7475  iendsFriendStatu
+000214f0: 7353 7461 7475 7327 2c20 2746 7269 656e  sStatus', 'Frien
+00021500: 6473 4672 6965 6e64 734c 6973 7427 2c20  dsFriendsList', 
+00021510: 2746 7269 656e 6473 4d75 7475 616c 4672  'FriendsMutualFr
+00021520: 6965 6e64 272c 2027 4672 6965 6e64 7352  iend', 'FriendsR
+00021530: 6571 7565 7374 7327 2c20 2746 7269 656e  equests', 'Frien
+00021540: 6473 5265 7175 6573 7473 4d75 7475 616c  dsRequestsMutual
+00021550: 272c 2027 4672 6965 6e64 7352 6571 7565  ', 'FriendsReque
+00021560: 7374 7358 7472 4d65 7373 6167 6527 2c20  stsXtrMessage', 
+00021570: 2746 7269 656e 6473 5573 6572 5874 7250  'FriendsUserXtrP
+00021580: 686f 6e65 272c 2027 4769 6674 7347 6966  hone', 'GiftsGif
+00021590: 7427 2c20 2747 6966 7473 4769 6674 5072  t', 'GiftsGiftPr
+000215a0: 6976 6163 7927 2c20 2747 6966 7473 4c61  ivacy', 'GiftsLa
+000215b0: 796f 7574 272c 2027 4772 6f75 7073 4164  yout', 'GroupsAd
+000215c0: 6472 6573 7327 2c20 2747 726f 7570 7341  dress', 'GroupsA
+000215d0: 6464 7265 7373 5469 6d65 7461 626c 6527  ddressTimetable'
+000215e0: 2c20 2747 726f 7570 7341 6464 7265 7373  , 'GroupsAddress
+000215f0: 5469 6d65 7461 626c 6544 6179 272c 2027  TimetableDay', '
+00021600: 4772 6f75 7073 4164 6472 6573 7357 6f72  GroupsAddressWor
+00021610: 6b49 6e66 6f53 7461 7475 7327 2c20 2747  kInfoStatus', 'G
+00021620: 726f 7570 7341 6464 7265 7373 6573 496e  roupsAddressesIn
+00021630: 666f 272c 2027 4772 6f75 7073 4261 6e49  fo', 'GroupsBanI
+00021640: 6e66 6f27 2c20 2747 726f 7570 7342 616e  nfo', 'GroupsBan
+00021650: 496e 666f 5265 6173 6f6e 272c 2027 4772  InfoReason', 'Gr
+00021660: 6f75 7073 4261 6e6e 6564 4974 656d 272c  oupsBannedItem',
+00021670: 2027 4772 6f75 7073 4361 6c6c 6261 636b   'GroupsCallback
+00021680: 5365 7276 6572 272c 2027 4772 6f75 7073  Server', 'Groups
+00021690: 4361 6c6c 6261 636b 5365 7474 696e 6773  CallbackSettings
+000216a0: 272c 2027 4772 6f75 7073 436f 6e74 6163  ', 'GroupsContac
+000216b0: 7473 4974 656d 272c 2027 4772 6f75 7073  tsItem', 'Groups
+000216c0: 436f 756e 7465 7273 4772 6f75 7027 2c20  CountersGroup', 
+000216d0: 2747 726f 7570 7343 6f76 6572 272c 2027  'GroupsCover', '
+000216e0: 4772 6f75 7073 4669 656c 6473 272c 2027  GroupsFields', '
+000216f0: 4772 6f75 7073 4669 6c74 6572 272c 2027  GroupsFilter', '
+00021700: 4772 6f75 7073 4772 6f75 7027 2c20 2747  GroupsGroup', 'G
+00021710: 726f 7570 7347 726f 7570 4163 6365 7373  roupsGroupAccess
+00021720: 272c 2027 4772 6f75 7073 4772 6f75 7041  ', 'GroupsGroupA
+00021730: 646d 696e 4c65 7665 6c27 2c20 2747 726f  dminLevel', 'Gro
+00021740: 7570 7347 726f 7570 4167 654c 696d 6974  upsGroupAgeLimit
+00021750: 7327 2c20 2747 726f 7570 7347 726f 7570  s', 'GroupsGroup
+00021760: 4174 7461 6368 272c 2027 4772 6f75 7073  Attach', 'Groups
+00021770: 4772 6f75 7041 7564 696f 272c 2027 4772  GroupAudio', 'Gr
+00021780: 6f75 7073 4772 6f75 7042 616e 496e 666f  oupsGroupBanInfo
+00021790: 272c 2027 4772 6f75 7073 4772 6f75 7043  ', 'GroupsGroupC
+000217a0: 6174 6567 6f72 7927 2c20 2747 726f 7570  ategory', 'Group
+000217b0: 7347 726f 7570 4361 7465 676f 7279 4675  sGroupCategoryFu
+000217c0: 6c6c 272c 2027 4772 6f75 7073 4772 6f75  ll', 'GroupsGrou
+000217d0: 7043 6174 6567 6f72 7954 7970 6527 2c20  pCategoryType', 
+000217e0: 2747 726f 7570 7347 726f 7570 446f 6373  'GroupsGroupDocs
+000217f0: 272c 2027 4772 6f75 7073 4772 6f75 7046  ', 'GroupsGroupF
+00021800: 756c 6c27 2c20 2747 726f 7570 7347 726f  ull', 'GroupsGro
+00021810: 7570 4675 6c6c 4167 654c 696d 6974 7327  upFullAgeLimits'
+00021820: 2c20 2747 726f 7570 7347 726f 7570 4675  , 'GroupsGroupFu
+00021830: 6c6c 4d65 6d62 6572 5374 6174 7573 272c  llMemberStatus',
+00021840: 2027 4772 6f75 7073 4772 6f75 7046 756c   'GroupsGroupFul
+00021850: 6c53 6563 7469 6f6e 272c 2027 4772 6f75  lSection', 'Grou
+00021860: 7073 4772 6f75 7049 7343 6c6f 7365 6427  psGroupIsClosed'
+00021870: 2c20 2747 726f 7570 7347 726f 7570 4d61  , 'GroupsGroupMa
+00021880: 726b 6574 4375 7272 656e 6379 272c 2027  rketCurrency', '
+00021890: 4772 6f75 7073 4772 6f75 7050 686f 746f  GroupsGroupPhoto
+000218a0: 7327 2c20 2747 726f 7570 7347 726f 7570  s', 'GroupsGroup
+000218b0: 5075 626c 6963 4361 7465 676f 7279 4c69  PublicCategoryLi
+000218c0: 7374 272c 2027 4772 6f75 7073 4772 6f75  st', 'GroupsGrou
+000218d0: 7052 6f6c 6527 2c20 2747 726f 7570 7347  pRole', 'GroupsG
+000218e0: 726f 7570 5375 626a 6563 7427 2c20 2747  roupSubject', 'G
+000218f0: 726f 7570 7347 726f 7570 5375 6767 6573  roupsGroupSugges
+00021900: 7465 6450 7269 7661 6379 272c 2027 4772  tedPrivacy', 'Gr
+00021910: 6f75 7073 4772 6f75 7054 6167 272c 2027  oupsGroupTag', '
+00021920: 4772 6f75 7073 4772 6f75 7054 6f70 6963  GroupsGroupTopic
+00021930: 7327 2c20 2747 726f 7570 7347 726f 7570  s', 'GroupsGroup
+00021940: 5479 7065 272c 2027 4772 6f75 7073 4772  Type', 'GroupsGr
+00021950: 6f75 7056 6964 656f 272c 2027 4772 6f75  oupVideo', 'Grou
+00021960: 7073 4772 6f75 7057 616c 6c27 2c20 2747  psGroupWall', 'G
+00021970: 726f 7570 7347 726f 7570 5769 6b69 272c  roupsGroupWiki',
+00021980: 2027 4772 6f75 7073 4772 6f75 7073 4172   'GroupsGroupsAr
+00021990: 7261 7927 2c20 2747 726f 7570 734c 696e  ray', 'GroupsLin
+000219a0: 6b73 4974 656d 272c 2027 4772 6f75 7073  ksItem', 'Groups
+000219b0: 4c69 7665 436f 7665 7273 272c 2027 4772  LiveCovers', 'Gr
+000219c0: 6f75 7073 4c6f 6e67 506f 6c6c 4576 656e  oupsLongPollEven
+000219d0: 7473 272c 2027 4772 6f75 7073 4c6f 6e67  ts', 'GroupsLong
+000219e0: 506f 6c6c 5365 7276 6572 272c 2027 4772  PollServer', 'Gr
+000219f0: 6f75 7073 4c6f 6e67 506f 6c6c 5365 7474  oupsLongPollSett
+00021a00: 696e 6773 272c 2027 4772 6f75 7073 4d61  ings', 'GroupsMa
+00021a10: 726b 6574 496e 666f 272c 2027 4772 6f75  rketInfo', 'Grou
+00021a20: 7073 4d61 726b 6574 5374 6174 6527 2c20  psMarketState', 
+00021a30: 2747 726f 7570 734d 656d 6265 7252 6f6c  'GroupsMemberRol
+00021a40: 6527 2c20 2747 726f 7570 734d 656d 6265  e', 'GroupsMembe
+00021a50: 7252 6f6c 6550 6572 6d69 7373 696f 6e27  rRolePermission'
+00021a60: 2c20 2747 726f 7570 734d 656d 6265 7252  , 'GroupsMemberR
+00021a70: 6f6c 6553 7461 7475 7327 2c20 2747 726f  oleStatus', 'Gro
+00021a80: 7570 734d 656d 6265 7253 7461 7475 7327  upsMemberStatus'
+00021a90: 2c20 2747 726f 7570 734d 656d 6265 7253  , 'GroupsMemberS
+00021aa0: 7461 7475 7346 756c 6c27 2c20 2747 726f  tatusFull', 'Gro
+00021ab0: 7570 734f 6e6c 696e 6553 7461 7475 7327  upsOnlineStatus'
+00021ac0: 2c20 2747 726f 7570 734f 6e6c 696e 6553  , 'GroupsOnlineS
+00021ad0: 7461 7475 7354 7970 6527 2c20 2747 726f  tatusType', 'Gro
+00021ae0: 7570 734f 776e 6572 5874 7242 616e 496e  upsOwnerXtrBanIn
+00021af0: 666f 272c 2027 4772 6f75 7073 4f77 6e65  fo', 'GroupsOwne
+00021b00: 7258 7472 4261 6e49 6e66 6f54 7970 6527  rXtrBanInfoType'
+00021b10: 2c20 2747 726f 7570 7350 686f 746f 5369  , 'GroupsPhotoSi
+00021b20: 7a65 272c 2027 4772 6f75 7073 526f 6c65  ze', 'GroupsRole
+00021b30: 4f70 7469 6f6e 7327 2c20 2747 726f 7570  Options', 'Group
+00021b40: 7353 6563 7469 6f6e 734c 6973 7449 7465  sSectionsListIte
+00021b50: 6d27 2c20 2747 726f 7570 7353 6574 7469  m', 'GroupsSetti
+00021b60: 6e67 7354 7769 7474 6572 272c 2027 4772  ngsTwitter', 'Gr
+00021b70: 6f75 7073 5375 626a 6563 7449 7465 6d27  oupsSubjectItem'
+00021b80: 2c20 2747 726f 7570 7354 6f6b 656e 5065  , 'GroupsTokenPe
+00021b90: 726d 6973 7369 6f6e 5365 7474 696e 6727  rmissionSetting'
+00021ba0: 2c20 2747 726f 7570 7355 7365 7258 7472  , 'GroupsUserXtr
+00021bb0: 526f 6c65 272c 2027 4c65 6164 466f 726d  Role', 'LeadForm
+00021bc0: 7341 6e73 7765 7227 2c20 274c 6561 6446  sAnswer', 'LeadF
+00021bd0: 6f72 6d73 416e 7377 6572 4974 656d 272c  ormsAnswerItem',
+00021be0: 2027 4c65 6164 466f 726d 7346 6f72 6d27   'LeadFormsForm'
+00021bf0: 2c20 274c 6561 6446 6f72 6d73 4c65 6164  , 'LeadFormsLead
+00021c00: 272c 2027 4c65 6164 466f 726d 7351 7565  ', 'LeadFormsQue
+00021c10: 7374 696f 6e49 7465 6d27 2c20 274c 6561  stionItem', 'Lea
+00021c20: 6446 6f72 6d73 5175 6573 7469 6f6e 4974  dFormsQuestionIt
+00021c30: 656d 4f70 7469 6f6e 272c 2027 4c69 6b65  emOption', 'Like
+00021c40: 7354 7970 6527 2c20 274c 696e 6b54 6172  sType', 'LinkTar
+00021c50: 6765 744f 626a 6563 7427 2c20 274d 6172  getObject', 'Mar
+00021c60: 6b65 7443 7572 7265 6e63 7927 2c20 274d  ketCurrency', 'M
+00021c70: 6172 6b65 744d 6172 6b65 7441 6c62 756d  arketMarketAlbum
+00021c80: 272c 2027 4d61 726b 6574 4d61 726b 6574  ', 'MarketMarket
+00021c90: 4361 7465 676f 7279 272c 2027 4d61 726b  Category', 'Mark
+00021ca0: 6574 4d61 726b 6574 4361 7465 676f 7279  etMarketCategory
+00021cb0: 4e65 7374 6564 272c 2027 4d61 726b 6574  Nested', 'Market
+00021cc0: 4d61 726b 6574 4361 7465 676f 7279 4f6c  MarketCategoryOl
+00021cd0: 6427 2c20 274d 6172 6b65 744d 6172 6b65  d', 'MarketMarke
+00021ce0: 7443 6174 6567 6f72 7954 7265 6527 2c20  tCategoryTree', 
+00021cf0: 274d 6172 6b65 744d 6172 6b65 7449 7465  'MarketMarketIte
+00021d00: 6d27 2c20 274d 6172 6b65 744d 6172 6b65  m', 'MarketMarke
+00021d10: 7449 7465 6d41 7661 696c 6162 696c 6974  tItemAvailabilit
+00021d20: 7927 2c20 274d 6172 6b65 744d 6172 6b65  y', 'MarketMarke
+00021d30: 7449 7465 6d46 756c 6c27 2c20 274d 6172  tItemFull', 'Mar
+00021d40: 6b65 744f 7264 6572 272c 2027 4d61 726b  ketOrder', 'Mark
+00021d50: 6574 4f72 6465 7249 7465 6d27 2c20 274d  etOrderItem', 'M
+00021d60: 6172 6b65 7450 7269 6365 272c 2027 4d61  arketPrice', 'Ma
+00021d70: 726b 6574 5365 6374 696f 6e27 2c20 274d  rketSection', 'M
+00021d80: 6172 6b65 7453 6572 7669 6365 7356 6965  arketServicesVie
+00021d90: 7754 7970 6527 2c20 274d 6573 7361 6765  wType', 'Message
+00021da0: 7341 7564 696f 4d65 7373 6167 6527 2c20  sAudioMessage', 
+00021db0: 274d 6573 7361 6765 7343 6861 7427 2c20  'MessagesChat', 
+00021dc0: 274d 6573 7361 6765 7343 6861 7446 756c  'MessagesChatFul
+00021dd0: 6c27 2c20 274d 6573 7361 6765 7343 6861  l', 'MessagesCha
+00021de0: 7450 7265 7669 6577 272c 2027 4d65 7373  tPreview', 'Mess
+00021df0: 6167 6573 4368 6174 5075 7368 5365 7474  agesChatPushSett
+00021e00: 696e 6773 272c 2027 4d65 7373 6167 6573  ings', 'Messages
+00021e10: 4368 6174 5265 7374 7269 6374 696f 6e73  ChatRestrictions
+00021e20: 272c 2027 4d65 7373 6167 6573 4368 6174  ', 'MessagesChat
+00021e30: 5365 7474 696e 6773 272c 2027 4d65 7373  Settings', 'Mess
+00021e40: 6167 6573 4368 6174 5365 7474 696e 6773  agesChatSettings
+00021e50: 4163 6c27 2c20 274d 6573 7361 6765 7343  Acl', 'MessagesC
+00021e60: 6861 7453 6574 7469 6e67 7350 6572 6d69  hatSettingsPermi
+00021e70: 7373 696f 6e73 272c 2027 4d65 7373 6167  ssions', 'Messag
+00021e80: 6573 4368 6174 5365 7474 696e 6773 5068  esChatSettingsPh
+00021e90: 6f74 6f27 2c20 274d 6573 7361 6765 7343  oto', 'MessagesC
+00021ea0: 6861 7453 6574 7469 6e67 7353 7461 7465  hatSettingsState
+00021eb0: 272c 2027 4d65 7373 6167 6573 436f 6e76  ', 'MessagesConv
+00021ec0: 6572 7361 7469 6f6e 272c 2027 4d65 7373  ersation', 'Mess
+00021ed0: 6167 6573 436f 6e76 6572 7361 7469 6f6e  agesConversation
+00021ee0: 4361 6e57 7269 7465 272c 2027 4d65 7373  CanWrite', 'Mess
+00021ef0: 6167 6573 436f 6e76 6572 7361 7469 6f6e  agesConversation
+00021f00: 4d65 6d62 6572 272c 2027 4d65 7373 6167  Member', 'Messag
+00021f10: 6573 436f 6e76 6572 7361 7469 6f6e 5065  esConversationPe
+00021f20: 6572 272c 2027 4d65 7373 6167 6573 436f  er', 'MessagesCo
+00021f30: 6e76 6572 7361 7469 6f6e 5065 6572 5479  nversationPeerTy
+00021f40: 7065 272c 2027 4d65 7373 6167 6573 436f  pe', 'MessagesCo
+00021f50: 6e76 6572 7361 7469 6f6e 536f 7274 4964  nversationSortId
+00021f60: 272c 2027 4d65 7373 6167 6573 436f 6e76  ', 'MessagesConv
+00021f70: 6572 7361 7469 6f6e 5769 7468 4d65 7373  ersationWithMess
 00021f80: 6167 6527 2c20 274d 6573 7361 6765 7346  age', 'MessagesF
-00021f90: 6f72 7761 7264 272c 2027 4d65 7373 6167  orward', 'Messag
-00021fa0: 6573 4765 7443 6f6e 7665 7273 6174 696f  esGetConversatio
-00021fb0: 6e42 7949 6427 2c20 274d 6573 7361 6765  nById', 'Message
-00021fc0: 7347 6574 436f 6e76 6572 7361 7469 6f6e  sGetConversation
-00021fd0: 4279 4964 4578 7465 6e64 6564 272c 2027  ByIdExtended', '
-00021fe0: 4d65 7373 6167 6573 4765 7443 6f6e 7665  MessagesGetConve
-00021ff0: 7273 6174 696f 6e4d 656d 6265 7273 272c  rsationMembers',
-00022000: 2027 4d65 7373 6167 6573 4772 6166 6669   'MessagesGraffi
-00022010: 7469 272c 2027 4d65 7373 6167 6573 4869  ti', 'MessagesHi
-00022020: 7374 6f72 7941 7474 6163 686d 656e 7427  storyAttachment'
-00022030: 2c20 274d 6573 7361 6765 7348 6973 746f  , 'MessagesHisto
-00022040: 7279 4d65 7373 6167 6541 7474 6163 686d  ryMessageAttachm
-00022050: 656e 7427 2c20 274d 6573 7361 6765 7348  ent', 'MessagesH
-00022060: 6973 746f 7279 4d65 7373 6167 6541 7474  istoryMessageAtt
-00022070: 6163 686d 656e 7454 7970 6527 2c20 274d  achmentType', 'M
-00022080: 6573 7361 6765 734b 6579 626f 6172 6427  essagesKeyboard'
-00022090: 2c20 274d 6573 7361 6765 734b 6579 626f  , 'MessagesKeybo
-000220a0: 6172 6442 7574 746f 6e27 2c20 274d 6573  ardButton', 'Mes
+00021f90: 6f72 6569 676e 4d65 7373 6167 6527 2c20  oreignMessage', 
+00021fa0: 274d 6573 7361 6765 7346 6f72 7761 7264  'MessagesForward
+00021fb0: 272c 2027 4d65 7373 6167 6573 4765 7443  ', 'MessagesGetC
+00021fc0: 6f6e 7665 7273 6174 696f 6e42 7949 6427  onversationById'
+00021fd0: 2c20 274d 6573 7361 6765 7347 6574 436f  , 'MessagesGetCo
+00021fe0: 6e76 6572 7361 7469 6f6e 4279 4964 4578  nversationByIdEx
+00021ff0: 7465 6e64 6564 272c 2027 4d65 7373 6167  tended', 'Messag
+00022000: 6573 4765 7443 6f6e 7665 7273 6174 696f  esGetConversatio
+00022010: 6e4d 656d 6265 7273 272c 2027 4d65 7373  nMembers', 'Mess
+00022020: 6167 6573 4772 6166 6669 7469 272c 2027  agesGraffiti', '
+00022030: 4d65 7373 6167 6573 4869 7374 6f72 7941  MessagesHistoryA
+00022040: 7474 6163 686d 656e 7427 2c20 274d 6573  ttachment', 'Mes
+00022050: 7361 6765 7348 6973 746f 7279 4d65 7373  sagesHistoryMess
+00022060: 6167 6541 7474 6163 686d 656e 7427 2c20  ageAttachment', 
+00022070: 274d 6573 7361 6765 7348 6973 746f 7279  'MessagesHistory
+00022080: 4d65 7373 6167 6541 7474 6163 686d 656e  MessageAttachmen
+00022090: 7454 7970 6527 2c20 274d 6573 7361 6765  tType', 'Message
+000220a0: 734b 6579 626f 6172 6427 2c20 274d 6573  sKeyboard', 'Mes
 000220b0: 7361 6765 734b 6579 626f 6172 6442 7574  sagesKeyboardBut
-000220c0: 746f 6e41 6374 696f 6e43 616c 6c62 6163  tonActionCallbac
-000220d0: 6b27 2c20 274d 6573 7361 6765 734b 6579  k', 'MessagesKey
-000220e0: 626f 6172 6442 7574 746f 6e41 6374 696f  boardButtonActio
-000220f0: 6e4c 6f63 6174 696f 6e27 2c20 274d 6573  nLocation', 'Mes
-00022100: 7361 6765 734b 6579 626f 6172 6442 7574  sagesKeyboardBut
-00022110: 746f 6e41 6374 696f 6e4f 7065 6e41 7070  tonActionOpenApp
-00022120: 272c 2027 4d65 7373 6167 6573 4b65 7962  ', 'MessagesKeyb
-00022130: 6f61 7264 4275 7474 6f6e 4163 7469 6f6e  oardButtonAction
-00022140: 4f70 656e 4c69 6e6b 272c 2027 4d65 7373  OpenLink', 'Mess
-00022150: 6167 6573 4b65 7962 6f61 7264 4275 7474  agesKeyboardButt
-00022160: 6f6e 4163 7469 6f6e 4f70 656e 5068 6f74  onActionOpenPhot
-00022170: 6f27 2c20 274d 6573 7361 6765 734b 6579  o', 'MessagesKey
-00022180: 626f 6172 6442 7574 746f 6e41 6374 696f  boardButtonActio
-00022190: 6e54 6578 7427 2c20 274d 6573 7361 6765  nText', 'Message
-000221a0: 734b 6579 626f 6172 6442 7574 746f 6e41  sKeyboardButtonA
-000221b0: 6374 696f 6e56 6b70 6179 272c 2027 4d65  ctionVkpay', 'Me
-000221c0: 7373 6167 6573 4b65 7962 6f61 7264 4275  ssagesKeyboardBu
-000221d0: 7474 6f6e 5072 6f70 6572 7479 4163 7469  ttonPropertyActi
-000221e0: 6f6e 272c 2027 4d65 7373 6167 6573 4c61  on', 'MessagesLa
-000221f0: 7374 4163 7469 7669 7479 272c 2027 4d65  stActivity', 'Me
-00022200: 7373 6167 6573 4c6f 6e67 706f 6c6c 4d65  ssagesLongpollMe
-00022210: 7373 6167 6573 272c 2027 4d65 7373 6167  ssages', 'Messag
-00022220: 6573 4c6f 6e67 706f 6c6c 5061 7261 6d73  esLongpollParams
-00022230: 272c 2027 4d65 7373 6167 6573 4d65 7373  ', 'MessagesMess
-00022240: 6167 6527 2c20 274d 6573 7361 6765 734d  age', 'MessagesM
-00022250: 6573 7361 6765 4163 7469 6f6e 272c 2027  essageAction', '
-00022260: 4d65 7373 6167 6573 4d65 7373 6167 6541  MessagesMessageA
-00022270: 6374 696f 6e50 686f 746f 272c 2027 4d65  ctionPhoto', 'Me
-00022280: 7373 6167 6573 4d65 7373 6167 6541 6374  ssagesMessageAct
-00022290: 696f 6e53 7461 7475 7327 2c20 274d 6573  ionStatus', 'Mes
-000222a0: 7361 6765 734d 6573 7361 6765 4174 7461  sagesMessageAtta
-000222b0: 6368 6d65 6e74 272c 2027 4d65 7373 6167  chment', 'Messag
-000222c0: 6573 4d65 7373 6167 6541 7474 6163 686d  esMessageAttachm
-000222d0: 656e 7454 7970 6527 2c20 274d 6573 7361  entType', 'Messa
-000222e0: 6765 734d 6573 7361 6765 5265 7175 6573  gesMessageReques
-000222f0: 7444 6174 6127 2c20 274d 6573 7361 6765  tData', 'Message
-00022300: 734d 6573 7361 6765 7341 7272 6179 272c  sMessagesArray',
-00022310: 2027 4d65 7373 6167 6573 4f75 7452 6561   'MessagesOutRea
-00022320: 6442 7927 2c20 274d 6573 7361 6765 7350  dBy', 'MessagesP
-00022330: 696e 6e65 644d 6573 7361 6765 272c 2027  innedMessage', '
-00022340: 4d65 7373 6167 6573 5075 7368 5365 7474  MessagesPushSett
-00022350: 696e 6773 272c 2027 4d65 7373 6167 6573  ings', 'Messages
-00022360: 5365 6e64 5573 6572 4964 7352 6573 706f  SendUserIdsRespo
-00022370: 6e73 6549 7465 6d27 2c20 274d 6573 7361  nseItem', 'Messa
-00022380: 6765 7354 656d 706c 6174 6541 6374 696f  gesTemplateActio
-00022390: 6e54 7970 654e 616d 6573 272c 2027 4d65  nTypeNames', 'Me
-000223a0: 7373 6167 6573 5573 6572 5874 7249 6e76  ssagesUserXtrInv
-000223b0: 6974 6564 4279 272c 2027 4e65 7773 6665  itedBy', 'Newsfe
-000223c0: 6564 436f 6d6d 656e 7473 4669 6c74 6572  edCommentsFilter
-000223d0: 7327 2c20 274e 6577 7366 6565 6449 676e  s', 'NewsfeedIgn
-000223e0: 6f72 6549 7465 6d54 7970 6527 2c20 274e  oreItemType', 'N
-000223f0: 6577 7366 6565 6449 7465 6d41 7564 696f  ewsfeedItemAudio
-00022400: 272c 2027 4e65 7773 6665 6564 4974 656d  ', 'NewsfeedItem
-00022410: 4175 6469 6f41 7564 696f 272c 2027 4e65  AudioAudio', 'Ne
-00022420: 7773 6665 6564 4974 656d 4261 7365 272c  wsfeedItemBase',
-00022430: 2027 4e65 7773 6665 6564 4974 656d 4469   'NewsfeedItemDi
-00022440: 6765 7374 272c 2027 4e65 7773 6665 6564  gest', 'Newsfeed
-00022450: 4974 656d 4469 6765 7374 4275 7474 6f6e  ItemDigestButton
-00022460: 272c 2027 4e65 7773 6665 6564 4974 656d  ', 'NewsfeedItem
-00022470: 4469 6765 7374 466f 6f74 6572 272c 2027  DigestFooter', '
-00022480: 4e65 7773 6665 6564 4974 656d 4469 6765  NewsfeedItemDige
-00022490: 7374 4675 6c6c 4974 656d 272c 2027 4e65  stFullItem', 'Ne
-000224a0: 7773 6665 6564 4974 656d 4469 6765 7374  wsfeedItemDigest
-000224b0: 4865 6164 6572 272c 2027 4e65 7773 6665  Header', 'Newsfe
-000224c0: 6564 4974 656d 4469 6765 7374 4974 656d  edItemDigestItem
+000220c0: 746f 6e27 2c20 274d 6573 7361 6765 734b  ton', 'MessagesK
+000220d0: 6579 626f 6172 6442 7574 746f 6e41 6374  eyboardButtonAct
+000220e0: 696f 6e43 616c 6c62 6163 6b27 2c20 274d  ionCallback', 'M
+000220f0: 6573 7361 6765 734b 6579 626f 6172 6442  essagesKeyboardB
+00022100: 7574 746f 6e41 6374 696f 6e4c 6f63 6174  uttonActionLocat
+00022110: 696f 6e27 2c20 274d 6573 7361 6765 734b  ion', 'MessagesK
+00022120: 6579 626f 6172 6442 7574 746f 6e41 6374  eyboardButtonAct
+00022130: 696f 6e4f 7065 6e41 7070 272c 2027 4d65  ionOpenApp', 'Me
+00022140: 7373 6167 6573 4b65 7962 6f61 7264 4275  ssagesKeyboardBu
+00022150: 7474 6f6e 4163 7469 6f6e 4f70 656e 4c69  ttonActionOpenLi
+00022160: 6e6b 272c 2027 4d65 7373 6167 6573 4b65  nk', 'MessagesKe
+00022170: 7962 6f61 7264 4275 7474 6f6e 4163 7469  yboardButtonActi
+00022180: 6f6e 4f70 656e 5068 6f74 6f27 2c20 274d  onOpenPhoto', 'M
+00022190: 6573 7361 6765 734b 6579 626f 6172 6442  essagesKeyboardB
+000221a0: 7574 746f 6e41 6374 696f 6e54 6578 7427  uttonActionText'
+000221b0: 2c20 274d 6573 7361 6765 734b 6579 626f  , 'MessagesKeybo
+000221c0: 6172 6442 7574 746f 6e41 6374 696f 6e56  ardButtonActionV
+000221d0: 6b70 6179 272c 2027 4d65 7373 6167 6573  kpay', 'Messages
+000221e0: 4b65 7962 6f61 7264 4275 7474 6f6e 5072  KeyboardButtonPr
+000221f0: 6f70 6572 7479 4163 7469 6f6e 272c 2027  opertyAction', '
+00022200: 4d65 7373 6167 6573 4c61 7374 4163 7469  MessagesLastActi
+00022210: 7669 7479 272c 2027 4d65 7373 6167 6573  vity', 'Messages
+00022220: 4c6f 6e67 706f 6c6c 4d65 7373 6167 6573  LongpollMessages
+00022230: 272c 2027 4d65 7373 6167 6573 4c6f 6e67  ', 'MessagesLong
+00022240: 706f 6c6c 5061 7261 6d73 272c 2027 4d65  pollParams', 'Me
+00022250: 7373 6167 6573 4d65 7373 6167 6527 2c20  ssagesMessage', 
+00022260: 274d 6573 7361 6765 734d 6573 7361 6765  'MessagesMessage
+00022270: 4163 7469 6f6e 272c 2027 4d65 7373 6167  Action', 'Messag
+00022280: 6573 4d65 7373 6167 6541 6374 696f 6e50  esMessageActionP
+00022290: 686f 746f 272c 2027 4d65 7373 6167 6573  hoto', 'Messages
+000222a0: 4d65 7373 6167 6541 6374 696f 6e53 7461  MessageActionSta
+000222b0: 7475 7327 2c20 274d 6573 7361 6765 734d  tus', 'MessagesM
+000222c0: 6573 7361 6765 4174 7461 6368 6d65 6e74  essageAttachment
+000222d0: 272c 2027 4d65 7373 6167 6573 4d65 7373  ', 'MessagesMess
+000222e0: 6167 6541 7474 6163 686d 656e 7454 7970  ageAttachmentTyp
+000222f0: 6527 2c20 274d 6573 7361 6765 734d 6573  e', 'MessagesMes
+00022300: 7361 6765 5265 7175 6573 7444 6174 6127  sageRequestData'
+00022310: 2c20 274d 6573 7361 6765 734d 6573 7361  , 'MessagesMessa
+00022320: 6765 7341 7272 6179 272c 2027 4d65 7373  gesArray', 'Mess
+00022330: 6167 6573 4f75 7452 6561 6442 7927 2c20  agesOutReadBy', 
+00022340: 274d 6573 7361 6765 7350 696e 6e65 644d  'MessagesPinnedM
+00022350: 6573 7361 6765 272c 2027 4d65 7373 6167  essage', 'Messag
+00022360: 6573 5075 7368 5365 7474 696e 6773 272c  esPushSettings',
+00022370: 2027 4d65 7373 6167 6573 5365 6e64 5573   'MessagesSendUs
+00022380: 6572 4964 7352 6573 706f 6e73 6549 7465  erIdsResponseIte
+00022390: 6d27 2c20 274d 6573 7361 6765 7354 656d  m', 'MessagesTem
+000223a0: 706c 6174 6541 6374 696f 6e54 7970 654e  plateActionTypeN
+000223b0: 616d 6573 272c 2027 4d65 7373 6167 6573  ames', 'Messages
+000223c0: 5573 6572 5874 7249 6e76 6974 6564 4279  UserXtrInvitedBy
+000223d0: 272c 2027 4e65 7773 6665 6564 436f 6d6d  ', 'NewsfeedComm
+000223e0: 656e 7473 4669 6c74 6572 7327 2c20 274e  entsFilters', 'N
+000223f0: 6577 7366 6565 6449 676e 6f72 6549 7465  ewsfeedIgnoreIte
+00022400: 6d54 7970 6527 2c20 274e 6577 7366 6565  mType', 'Newsfee
+00022410: 6449 7465 6d41 7564 696f 272c 2027 4e65  dItemAudio', 'Ne
+00022420: 7773 6665 6564 4974 656d 4175 6469 6f41  wsfeedItemAudioA
+00022430: 7564 696f 272c 2027 4e65 7773 6665 6564  udio', 'Newsfeed
+00022440: 4974 656d 4261 7365 272c 2027 4e65 7773  ItemBase', 'News
+00022450: 6665 6564 4974 656d 4469 6765 7374 272c  feedItemDigest',
+00022460: 2027 4e65 7773 6665 6564 4974 656d 4469   'NewsfeedItemDi
+00022470: 6765 7374 4275 7474 6f6e 272c 2027 4e65  gestButton', 'Ne
+00022480: 7773 6665 6564 4974 656d 4469 6765 7374  wsfeedItemDigest
+00022490: 466f 6f74 6572 272c 2027 4e65 7773 6665  Footer', 'Newsfe
+000224a0: 6564 4974 656d 4469 6765 7374 4675 6c6c  edItemDigestFull
+000224b0: 4974 656d 272c 2027 4e65 7773 6665 6564  Item', 'Newsfeed
+000224c0: 4974 656d 4469 6765 7374 4865 6164 6572  ItemDigestHeader
 000224d0: 272c 2027 4e65 7773 6665 6564 4974 656d  ', 'NewsfeedItem
-000224e0: 4672 6965 6e64 272c 2027 4e65 7773 6665  Friend', 'Newsfe
-000224f0: 6564 4974 656d 4672 6965 6e64 4672 6965  edItemFriendFrie
-00022500: 6e64 7327 2c20 274e 6577 7366 6565 6449  nds', 'NewsfeedI
-00022510: 7465 6d48 6f6c 6964 6179 5265 636f 6d6d  temHolidayRecomm
-00022520: 656e 6461 7469 6f6e 7342 6c6f 636b 4865  endationsBlockHe
-00022530: 6164 6572 272c 2027 4e65 7773 6665 6564  ader', 'Newsfeed
-00022540: 4974 656d 5068 6f74 6f27 2c20 274e 6577  ItemPhoto', 'New
-00022550: 7366 6565 6449 7465 6d50 686f 746f 5068  sfeedItemPhotoPh
-00022560: 6f74 6f73 272c 2027 4e65 7773 6665 6564  otos', 'Newsfeed
-00022570: 4974 656d 5068 6f74 6f54 6167 272c 2027  ItemPhotoTag', '
-00022580: 4e65 7773 6665 6564 4974 656d 5068 6f74  NewsfeedItemPhot
-00022590: 6f54 6167 5068 6f74 6f54 6167 7327 2c20  oTagPhotoTags', 
-000225a0: 274e 6577 7366 6565 6449 7465 6d50 726f  'NewsfeedItemPro
-000225b0: 6d6f 4275 7474 6f6e 272c 2027 4e65 7773  moButton', 'News
-000225c0: 6665 6564 4974 656d 5072 6f6d 6f42 7574  feedItemPromoBut
-000225d0: 746f 6e41 6374 696f 6e27 2c20 274e 6577  tonAction', 'New
-000225e0: 7366 6565 6449 7465 6d50 726f 6d6f 4275  sfeedItemPromoBu
-000225f0: 7474 6f6e 496d 6167 6527 2c20 274e 6577  ttonImage', 'New
-00022600: 7366 6565 6449 7465 6d54 6f70 6963 272c  sfeedItemTopic',
-00022610: 2027 4e65 7773 6665 6564 4974 656d 5669   'NewsfeedItemVi
-00022620: 6465 6f27 2c20 274e 6577 7366 6565 6449  deo', 'NewsfeedI
-00022630: 7465 6d56 6964 656f 5669 6465 6f27 2c20  temVideoVideo', 
-00022640: 274e 6577 7366 6565 6449 7465 6d57 616c  'NewsfeedItemWal
-00022650: 6c70 6f73 7427 2c20 274e 6577 7366 6565  lpost', 'Newsfee
-00022660: 6449 7465 6d57 616c 6c70 6f73 7446 6565  dItemWallpostFee
-00022670: 6462 6163 6b27 2c20 274e 6577 7366 6565  dback', 'Newsfee
-00022680: 6449 7465 6d57 616c 6c70 6f73 7446 6565  dItemWallpostFee
-00022690: 6462 6163 6b41 6e73 7765 7227 2c20 274e  dbackAnswer', 'N
-000226a0: 6577 7366 6565 6449 7465 6d57 616c 6c70  ewsfeedItemWallp
-000226b0: 6f73 7446 6565 6462 6163 6b54 7970 6527  ostFeedbackType'
-000226c0: 2c20 274e 6577 7366 6565 644c 6973 7427  , 'NewsfeedList'
-000226d0: 2c20 274e 6577 7366 6565 644c 6973 7446  , 'NewsfeedListF
-000226e0: 756c 6c27 2c20 274e 6577 7366 6565 644e  ull', 'NewsfeedN
-000226f0: 6577 7366 6565 6449 7465 6d27 2c20 274e  ewsfeedItem', 'N
-00022700: 6577 7366 6565 644e 6577 7366 6565 6449  ewsfeedNewsfeedI
-00022710: 7465 6d54 7970 6527 2c20 274e 6577 7366  temType', 'Newsf
-00022720: 6565 644e 6577 7366 6565 6450 686f 746f  eedNewsfeedPhoto
-00022730: 272c 2027 4e6f 7465 734e 6f74 6527 2c20  ', 'NotesNote', 
-00022740: 274e 6f74 6573 4e6f 7465 436f 6d6d 656e  'NotesNoteCommen
-00022750: 7427 2c20 274e 6f74 6966 6963 6174 696f  t', 'Notificatio
-00022760: 6e73 4665 6564 6261 636b 272c 2027 4e6f  nsFeedback', 'No
-00022770: 7469 6669 6361 7469 6f6e 734e 6f74 6966  tificationsNotif
-00022780: 6963 6174 696f 6e27 2c20 274e 6f74 6966  ication', 'Notif
-00022790: 6963 6174 696f 6e73 4e6f 7469 6669 6361  icationsNotifica
-000227a0: 7469 6f6e 4974 656d 272c 2027 4e6f 7469  tionItem', 'Noti
-000227b0: 6669 6361 7469 6f6e 734e 6f74 6966 6963  ficationsNotific
-000227c0: 6174 696f 6e50 6172 656e 7427 2c20 274e  ationParent', 'N
-000227d0: 6f74 6966 6963 6174 696f 6e73 4e6f 7469  otificationsNoti
-000227e0: 6669 6361 7469 6f6e 7343 6f6d 6d65 6e74  ficationsComment
-000227f0: 272c 2027 4e6f 7469 6669 6361 7469 6f6e  ', 'Notification
-00022800: 7352 6570 6c79 272c 2027 4e6f 7469 6669  sReply', 'Notifi
-00022810: 6361 7469 6f6e 7353 656e 644d 6573 7361  cationsSendMessa
-00022820: 6765 4572 726f 7227 2c20 274e 6f74 6966  geError', 'Notif
-00022830: 6963 6174 696f 6e73 5365 6e64 4d65 7373  icationsSendMess
-00022840: 6167 6549 7465 6d27 2c20 274f 6175 7468  ageItem', 'Oauth
-00022850: 4572 726f 7227 2c20 274f 7264 6572 7341  Error', 'OrdersA
-00022860: 6d6f 756e 7427 2c20 274f 7264 6572 7341  mount', 'OrdersA
-00022870: 6d6f 756e 7449 7465 6d27 2c20 274f 7264  mountItem', 'Ord
-00022880: 6572 734f 7264 6572 272c 2027 4f72 6465  ersOrder', 'Orde
-00022890: 7273 5375 6273 6372 6970 7469 6f6e 272c  rsSubscription',
-000228a0: 2027 4f77 6e65 7253 7461 7465 272c 2027   'OwnerState', '
-000228b0: 5061 6765 7350 7269 7661 6379 5365 7474  PagesPrivacySett
-000228c0: 696e 6773 272c 2027 5061 6765 7357 696b  ings', 'PagesWik
-000228d0: 6970 6167 6527 2c20 2750 6167 6573 5769  ipage', 'PagesWi
-000228e0: 6b69 7061 6765 4675 6c6c 272c 2027 5061  kipageFull', 'Pa
-000228f0: 6765 7357 696b 6970 6167 6548 6973 746f  gesWikipageHisto
-00022900: 7279 272c 2027 5068 6f74 6f73 496d 6167  ry', 'PhotosImag
-00022910: 6527 2c20 2750 686f 746f 7349 6d61 6765  e', 'PhotosImage
-00022920: 5479 7065 272c 2027 5068 6f74 6f73 5068  Type', 'PhotosPh
-00022930: 6f74 6f27 2c20 2750 686f 746f 7350 686f  oto', 'PhotosPho
-00022940: 746f 416c 6275 6d27 2c20 2750 686f 746f  toAlbum', 'Photo
-00022950: 7350 686f 746f 416c 6275 6d46 756c 6c27  sPhotoAlbumFull'
-00022960: 2c20 2750 686f 746f 7350 686f 746f 4661  , 'PhotosPhotoFa
-00022970: 6c73 6561 626c 6527 2c20 2750 686f 746f  lseable', 'Photo
-00022980: 7350 686f 746f 4675 6c6c 5874 7252 6561  sPhotoFullXtrRea
-00022990: 6c4f 6666 7365 7427 2c20 2750 686f 746f  lOffset', 'Photo
-000229a0: 7350 686f 746f 5369 7a65 7327 2c20 2750  sPhotoSizes', 'P
-000229b0: 686f 746f 7350 686f 746f 5369 7a65 7354  hotosPhotoSizesT
-000229c0: 7970 6527 2c20 2750 686f 746f 7350 686f  ype', 'PhotosPho
-000229d0: 746f 5461 6727 2c20 2750 686f 746f 7350  toTag', 'PhotosP
-000229e0: 686f 746f 5570 6c6f 6164 272c 2027 5068  hotoUpload', 'Ph
-000229f0: 6f74 6f73 5068 6f74 6f58 7472 5265 616c  otosPhotoXtrReal
-00022a00: 4f66 6673 6574 272c 2027 5068 6f74 6f73  Offset', 'Photos
-00022a10: 5068 6f74 6f58 7472 5461 6749 6e66 6f27  PhotoXtrTagInfo'
-00022a20: 2c20 2750 686f 746f 7354 6167 7353 7567  , 'PhotosTagsSug
-00022a30: 6765 7374 696f 6e49 7465 6d27 2c20 2750  gestionItem', 'P
-00022a40: 686f 746f 7354 6167 7353 7567 6765 7374  hotosTagsSuggest
-00022a50: 696f 6e49 7465 6d42 7574 746f 6e27 2c20  ionItemButton', 
-00022a60: 2750 6f64 6361 7374 436f 7665 7227 2c20  'PodcastCover', 
-00022a70: 2750 6f64 6361 7374 4578 7465 726e 616c  'PodcastExternal
-00022a80: 4461 7461 272c 2027 506f 6c6c 7341 6e73  Data', 'PollsAns
-00022a90: 7765 7227 2c20 2750 6f6c 6c73 4261 636b  wer', 'PollsBack
-00022aa0: 6772 6f75 6e64 272c 2027 506f 6c6c 7346  ground', 'PollsF
-00022ab0: 7269 656e 6427 2c20 2750 6f6c 6c73 506f  riend', 'PollsPo
-00022ac0: 6c6c 272c 2027 506f 6c6c 7350 6f6c 6c41  ll', 'PollsPollA
-00022ad0: 6e6f 6e79 6d6f 7573 272c 2027 506f 6c6c  nonymous', 'Poll
-00022ae0: 7356 6f74 6572 7327 2c20 2750 6f6c 6c73  sVoters', 'Polls
-00022af0: 566f 7465 7273 5573 6572 7327 2c20 2750  VotersUsers', 'P
-00022b00: 7265 7474 7943 6172 6473 5072 6574 7479  rettyCardsPretty
-00022b10: 4361 7264 272c 2027 5072 6574 7479 4361  Card', 'PrettyCa
-00022b20: 7264 7350 7265 7474 7943 6172 644f 7245  rdsPrettyCardOrE
-00022b30: 7272 6f72 272c 2027 5365 6172 6368 4869  rror', 'SearchHi
-00022b40: 6e74 272c 2027 5365 6172 6368 4869 6e74  nt', 'SearchHint
-00022b50: 5365 6374 696f 6e27 2c20 2753 6561 7263  Section', 'Searc
-00022b60: 6848 696e 7454 7970 6527 2c20 2753 6563  hHintType', 'Sec
-00022b70: 7572 6547 6976 6545 7665 6e74 5374 6963  ureGiveEventStic
-00022b80: 6b65 7249 7465 6d27 2c20 2753 6563 7572  kerItem', 'Secur
-00022b90: 654c 6576 656c 272c 2027 5365 6375 7265  eLevel', 'Secure
-00022ba0: 5365 7443 6f75 6e74 6572 4974 656d 272c  SetCounterItem',
-00022bb0: 2027 5365 6375 7265 536d 734e 6f74 6966   'SecureSmsNotif
-00022bc0: 6963 6174 696f 6e27 2c20 2753 6563 7572  ication', 'Secur
-00022bd0: 6554 6f6b 656e 4368 6563 6b65 6427 2c20  eTokenChecked', 
-00022be0: 2753 6563 7572 6554 7261 6e73 6163 7469  'SecureTransacti
-00022bf0: 6f6e 272c 2027 5374 6174 7341 6374 6976  on', 'StatsActiv
-00022c00: 6974 7927 2c20 2753 7461 7473 4369 7479  ity', 'StatsCity
-00022c10: 272c 2027 5374 6174 7343 6f75 6e74 7279  ', 'StatsCountry
-00022c20: 272c 2027 5374 6174 7350 6572 696f 6427  ', 'StatsPeriod'
-00022c30: 2c20 2753 7461 7473 5265 6163 6827 2c20  , 'StatsReach', 
-00022c40: 2753 7461 7473 5365 7841 6765 272c 2027  'StatsSexAge', '
-00022c50: 5374 6174 7356 6965 7773 272c 2027 5374  StatsViews', 'St
-00022c60: 6174 7357 616c 6c70 6f73 7453 7461 7427  atsWallpostStat'
-00022c70: 2c20 2753 7461 7475 7353 7461 7475 7327  , 'StatusStatus'
-00022c80: 2c20 2753 7469 636b 6572 7349 6d61 6765  , 'StickersImage
-00022c90: 5365 7427 2c20 2753 746f 7261 6765 5661  Set', 'StorageVa
-00022ca0: 6c75 6527 2c20 2753 746f 7265 5072 6f64  lue', 'StoreProd
-00022cb0: 7563 7427 2c20 2753 746f 7265 5072 6f64  uct', 'StoreProd
-00022cc0: 7563 7449 636f 6e27 2c20 2753 746f 7265  uctIcon', 'Store
-00022cd0: 5374 6963 6b65 7273 4b65 7977 6f72 6427  StickersKeyword'
-00022ce0: 2c20 2753 746f 7265 5374 6963 6b65 7273  , 'StoreStickers
-00022cf0: 4b65 7977 6f72 6453 7469 636b 6572 272c  KeywordSticker',
-00022d00: 2027 5374 6f72 6553 7469 636b 6572 734b   'StoreStickersK
-00022d10: 6579 776f 7264 5374 6963 6b65 7273 272c  eywordStickers',
-00022d20: 2027 5374 6f72 6965 7343 6c69 636b 6162   'StoriesClickab
-00022d30: 6c65 4172 6561 272c 2027 5374 6f72 6965  leArea', 'Storie
-00022d40: 7343 6c69 636b 6162 6c65 5374 6963 6b65  sClickableSticke
-00022d50: 7227 2c20 2753 746f 7269 6573 436c 6963  r', 'StoriesClic
-00022d60: 6b61 626c 6553 7469 636b 6572 7327 2c20  kableStickers', 
-00022d70: 2753 746f 7269 6573 4665 6564 4974 656d  'StoriesFeedItem
-00022d80: 272c 2027 5374 6f72 6965 7350 726f 6d6f  ', 'StoriesPromo
-00022d90: 426c 6f63 6b27 2c20 2753 746f 7269 6573  Block', 'Stories
-00022da0: 5265 706c 6965 7327 2c20 2753 746f 7269  Replies', 'Stori
-00022db0: 6573 5374 6174 4c69 6e65 272c 2027 5374  esStatLine', 'St
-00022dc0: 6f72 6965 7353 746f 7279 272c 2027 5374  oriesStory', 'St
-00022dd0: 6f72 6965 7353 746f 7279 4c69 6e6b 272c  oriesStoryLink',
-00022de0: 2027 5374 6f72 6965 7353 746f 7279 5374   'StoriesStorySt
-00022df0: 6174 7327 2c20 2753 746f 7269 6573 5374  ats', 'StoriesSt
-00022e00: 6f72 7953 7461 7473 5374 6174 272c 2027  oryStatsStat', '
-00022e10: 5374 6f72 6965 7353 746f 7279 5374 6174  StoriesStoryStat
-00022e20: 7353 7461 7465 272c 2027 5374 6f72 6965  sState', 'Storie
-00022e30: 7353 746f 7279 5479 7065 272c 2027 5374  sStoryType', 'St
-00022e40: 6f72 6965 7355 706c 6f61 644c 696e 6b54  oriesUploadLinkT
-00022e50: 6578 7427 2c20 2753 746f 7269 6573 5669  ext', 'StoriesVi
-00022e60: 6577 6572 7349 7465 6d27 2c20 2755 7365  ewersItem', 'Use
-00022e70: 7273 4361 7265 6572 272c 2027 5573 6572  rsCareer', 'User
-00022e80: 7345 7870 6f72 7473 272c 2027 5573 6572  sExports', 'User
-00022e90: 7346 6965 6c64 7327 2c20 2755 7365 7273  sFields', 'Users
-00022ea0: 4c61 7374 5365 656e 272c 2027 5573 6572  LastSeen', 'User
-00022eb0: 734d 696c 6974 6172 7927 2c20 2755 7365  sMilitary', 'Use
-00022ec0: 7273 4f63 6375 7061 7469 6f6e 272c 2027  rsOccupation', '
-00022ed0: 5573 6572 734f 6e6c 696e 6549 6e66 6f27  UsersOnlineInfo'
-00022ee0: 2c20 2755 7365 7273 5065 7273 6f6e 616c  , 'UsersPersonal
-00022ef0: 272c 2027 5573 6572 7352 656c 6174 6976  ', 'UsersRelativ
-00022f00: 6527 2c20 2755 7365 7273 5363 686f 6f6c  e', 'UsersSchool
-00022f10: 272c 2027 5573 6572 7353 7562 7363 7269  ', 'UsersSubscri
-00022f20: 7074 696f 6e73 4974 656d 272c 2027 5573  ptionsItem', 'Us
-00022f30: 6572 7355 6e69 7665 7273 6974 7927 2c20  ersUniversity', 
-00022f40: 2755 7365 7273 5573 6572 272c 2027 5573  'UsersUser', 'Us
-00022f50: 6572 7355 7365 7243 6f6e 6e65 6374 696f  ersUserConnectio
-00022f60: 6e73 272c 2027 5573 6572 7355 7365 7243  ns', 'UsersUserC
-00022f70: 6f75 6e74 6572 7327 2c20 2755 7365 7273  ounters', 'Users
-00022f80: 5573 6572 4675 6c6c 272c 2027 5573 6572  UserFull', 'User
-00022f90: 7355 7365 724d 696e 272c 2027 5573 6572  sUserMin', 'User
-00022fa0: 7355 7365 7252 656c 6174 696f 6e27 2c20  sUserRelation', 
-00022fb0: 2755 7365 7273 5573 6572 5365 7474 696e  'UsersUserSettin
-00022fc0: 6773 5874 7227 2c20 2755 7365 7273 5573  gsXtr', 'UsersUs
-00022fd0: 6572 5479 7065 272c 2027 5573 6572 7355  erType', 'UsersU
-00022fe0: 7365 7258 7472 5479 7065 272c 2027 5573  serXtrType', 'Us
-00022ff0: 6572 7355 7365 7273 4172 7261 7927 2c20  ersUsersArray', 
-00023000: 2755 7469 6c73 446f 6d61 696e 5265 736f  'UtilsDomainReso
-00023010: 6c76 6564 272c 2027 5574 696c 7344 6f6d  lved', 'UtilsDom
-00023020: 6169 6e52 6573 6f6c 7665 6454 7970 6527  ainResolvedType'
-00023030: 2c20 2755 7469 6c73 4c61 7374 5368 6f72  , 'UtilsLastShor
-00023040: 7465 6e65 644c 696e 6b27 2c20 2755 7469  tenedLink', 'Uti
-00023050: 6c73 4c69 6e6b 4368 6563 6b65 6427 2c20  lsLinkChecked', 
-00023060: 2755 7469 6c73 4c69 6e6b 4368 6563 6b65  'UtilsLinkChecke
-00023070: 6453 7461 7475 7327 2c20 2755 7469 6c73  dStatus', 'Utils
-00023080: 4c69 6e6b 5374 6174 7327 2c20 2755 7469  LinkStats', 'Uti
-00023090: 6c73 4c69 6e6b 5374 6174 7345 7874 656e  lsLinkStatsExten
-000230a0: 6465 6427 2c20 2755 7469 6c73 5368 6f72  ded', 'UtilsShor
-000230b0: 744c 696e 6b27 2c20 2755 7469 6c73 5374  tLink', 'UtilsSt
-000230c0: 6174 7327 2c20 2755 7469 6c73 5374 6174  ats', 'UtilsStat
-000230d0: 7343 6974 7927 2c20 2755 7469 6c73 5374  sCity', 'UtilsSt
-000230e0: 6174 7343 6f75 6e74 7279 272c 2027 5574  atsCountry', 'Ut
-000230f0: 696c 7353 7461 7473 4578 7465 6e64 6564  ilsStatsExtended
-00023100: 272c 2027 5574 696c 7353 7461 7473 5365  ', 'UtilsStatsSe
-00023110: 7841 6765 272c 2027 5669 6465 6f4c 6976  xAge', 'VideoLiv
-00023120: 6549 6e66 6f27 2c20 2756 6964 656f 4c69  eInfo', 'VideoLi
-00023130: 7665 5365 7474 696e 6773 272c 2027 5669  veSettings', 'Vi
-00023140: 6465 6f53 6176 6552 6573 756c 7427 2c20  deoSaveResult', 
-00023150: 2756 6964 656f 5669 6465 6f27 2c20 2756  'VideoVideo', 'V
-00023160: 6964 656f 5669 6465 6f41 6c62 756d 272c  ideoVideoAlbum',
-00023170: 2027 5669 6465 6f56 6964 656f 416c 6275   'VideoVideoAlbu
-00023180: 6d46 756c 6c27 2c20 2756 6964 656f 5669  mFull', 'VideoVi
-00023190: 6465 6f46 696c 6573 272c 2027 5669 6465  deoFiles', 'Vide
-000231a0: 6f56 6964 656f 4675 6c6c 272c 2027 5669  oVideoFull', 'Vi
-000231b0: 6465 6f56 6964 656f 496d 6167 6527 2c20  deoVideoImage', 
-000231c0: 2757 616c 6c41 7070 506f 7374 272c 2027  'WallAppPost', '
-000231d0: 5761 6c6c 4174 7461 6368 6564 4e6f 7465  WallAttachedNote
-000231e0: 272c 2027 5761 6c6c 4361 726f 7573 656c  ', 'WallCarousel
-000231f0: 4261 7365 272c 2027 5761 6c6c 436f 6d6d  Base', 'WallComm
-00023200: 656e 7441 7474 6163 686d 656e 7427 2c20  entAttachment', 
-00023210: 2757 616c 6c43 6f6d 6d65 6e74 4174 7461  'WallCommentAtta
-00023220: 6368 6d65 6e74 5479 7065 272c 2027 5761  chmentType', 'Wa
-00023230: 6c6c 4765 6f27 2c20 2757 616c 6c47 6574  llGeo', 'WallGet
-00023240: 4669 6c74 6572 272c 2027 5761 6c6c 4772  Filter', 'WallGr
-00023250: 6166 6669 7469 272c 2027 5761 6c6c 506f  affiti', 'WallPo
-00023260: 7374 436f 7079 7269 6768 7427 2c20 2757  stCopyright', 'W
-00023270: 616c 6c50 6f73 7453 6f75 7263 6527 2c20  allPostSource', 
-00023280: 2757 616c 6c50 6f73 7453 6f75 7263 6554  'WallPostSourceT
-00023290: 7970 6527 2c20 2757 616c 6c50 6f73 7454  ype', 'WallPostT
-000232a0: 7970 6527 2c20 2757 616c 6c50 6f73 7465  ype', 'WallPoste
-000232b0: 6450 686f 746f 272c 2027 5761 6c6c 5669  dPhoto', 'WallVi
-000232c0: 6577 7327 2c20 2757 616c 6c57 616c 6c43  ews', 'WallWallC
-000232d0: 6f6d 6d65 6e74 272c 2027 5761 6c6c 5761  omment', 'WallWa
-000232e0: 6c6c 436f 6d6d 656e 7444 6f6e 7574 272c  llCommentDonut',
-000232f0: 2027 5761 6c6c 5761 6c6c 436f 6d6d 656e   'WallWallCommen
-00023300: 7444 6f6e 7574 506c 6163 6568 6f6c 6465  tDonutPlaceholde
-00023310: 7227 2c20 2757 616c 6c57 616c 6c70 6f73  r', 'WallWallpos
-00023320: 7427 2c20 2757 616c 6c57 616c 6c70 6f73  t', 'WallWallpos
-00023330: 7441 7474 6163 686d 656e 7427 2c20 2757  tAttachment', 'W
+000224e0: 4469 6765 7374 4974 656d 272c 2027 4e65  DigestItem', 'Ne
+000224f0: 7773 6665 6564 4974 656d 4672 6965 6e64  wsfeedItemFriend
+00022500: 272c 2027 4e65 7773 6665 6564 4974 656d  ', 'NewsfeedItem
+00022510: 4672 6965 6e64 4672 6965 6e64 7327 2c20  FriendFriends', 
+00022520: 274e 6577 7366 6565 6449 7465 6d48 6f6c  'NewsfeedItemHol
+00022530: 6964 6179 5265 636f 6d6d 656e 6461 7469  idayRecommendati
+00022540: 6f6e 7342 6c6f 636b 4865 6164 6572 272c  onsBlockHeader',
+00022550: 2027 4e65 7773 6665 6564 4974 656d 5068   'NewsfeedItemPh
+00022560: 6f74 6f27 2c20 274e 6577 7366 6565 6449  oto', 'NewsfeedI
+00022570: 7465 6d50 686f 746f 5068 6f74 6f73 272c  temPhotoPhotos',
+00022580: 2027 4e65 7773 6665 6564 4974 656d 5068   'NewsfeedItemPh
+00022590: 6f74 6f54 6167 272c 2027 4e65 7773 6665  otoTag', 'Newsfe
+000225a0: 6564 4974 656d 5068 6f74 6f54 6167 5068  edItemPhotoTagPh
+000225b0: 6f74 6f54 6167 7327 2c20 274e 6577 7366  otoTags', 'Newsf
+000225c0: 6565 6449 7465 6d50 726f 6d6f 4275 7474  eedItemPromoButt
+000225d0: 6f6e 272c 2027 4e65 7773 6665 6564 4974  on', 'NewsfeedIt
+000225e0: 656d 5072 6f6d 6f42 7574 746f 6e41 6374  emPromoButtonAct
+000225f0: 696f 6e27 2c20 274e 6577 7366 6565 6449  ion', 'NewsfeedI
+00022600: 7465 6d50 726f 6d6f 4275 7474 6f6e 496d  temPromoButtonIm
+00022610: 6167 6527 2c20 274e 6577 7366 6565 6449  age', 'NewsfeedI
+00022620: 7465 6d54 6f70 6963 272c 2027 4e65 7773  temTopic', 'News
+00022630: 6665 6564 4974 656d 5669 6465 6f27 2c20  feedItemVideo', 
+00022640: 274e 6577 7366 6565 6449 7465 6d56 6964  'NewsfeedItemVid
+00022650: 656f 5669 6465 6f27 2c20 274e 6577 7366  eoVideo', 'Newsf
+00022660: 6565 6449 7465 6d57 616c 6c70 6f73 7427  eedItemWallpost'
+00022670: 2c20 274e 6577 7366 6565 6449 7465 6d57  , 'NewsfeedItemW
+00022680: 616c 6c70 6f73 7446 6565 6462 6163 6b27  allpostFeedback'
+00022690: 2c20 274e 6577 7366 6565 6449 7465 6d57  , 'NewsfeedItemW
+000226a0: 616c 6c70 6f73 7446 6565 6462 6163 6b41  allpostFeedbackA
+000226b0: 6e73 7765 7227 2c20 274e 6577 7366 6565  nswer', 'Newsfee
+000226c0: 6449 7465 6d57 616c 6c70 6f73 7446 6565  dItemWallpostFee
+000226d0: 6462 6163 6b54 7970 6527 2c20 274e 6577  dbackType', 'New
+000226e0: 7366 6565 644c 6973 7427 2c20 274e 6577  sfeedList', 'New
+000226f0: 7366 6565 644c 6973 7446 756c 6c27 2c20  sfeedListFull', 
+00022700: 274e 6577 7366 6565 644e 6577 7366 6565  'NewsfeedNewsfee
+00022710: 6449 7465 6d27 2c20 274e 6577 7366 6565  dItem', 'Newsfee
+00022720: 644e 6577 7366 6565 6449 7465 6d54 7970  dNewsfeedItemTyp
+00022730: 6527 2c20 274e 6577 7366 6565 644e 6577  e', 'NewsfeedNew
+00022740: 7366 6565 6450 686f 746f 272c 2027 4e6f  sfeedPhoto', 'No
+00022750: 7465 734e 6f74 6527 2c20 274e 6f74 6573  tesNote', 'Notes
+00022760: 4e6f 7465 436f 6d6d 656e 7427 2c20 274e  NoteComment', 'N
+00022770: 6f74 6966 6963 6174 696f 6e73 4665 6564  otificationsFeed
+00022780: 6261 636b 272c 2027 4e6f 7469 6669 6361  back', 'Notifica
+00022790: 7469 6f6e 734e 6f74 6966 6963 6174 696f  tionsNotificatio
+000227a0: 6e27 2c20 274e 6f74 6966 6963 6174 696f  n', 'Notificatio
+000227b0: 6e73 4e6f 7469 6669 6361 7469 6f6e 4974  nsNotificationIt
+000227c0: 656d 272c 2027 4e6f 7469 6669 6361 7469  em', 'Notificati
+000227d0: 6f6e 734e 6f74 6966 6963 6174 696f 6e50  onsNotificationP
+000227e0: 6172 656e 7427 2c20 274e 6f74 6966 6963  arent', 'Notific
+000227f0: 6174 696f 6e73 4e6f 7469 6669 6361 7469  ationsNotificati
+00022800: 6f6e 7343 6f6d 6d65 6e74 272c 2027 4e6f  onsComment', 'No
+00022810: 7469 6669 6361 7469 6f6e 7352 6570 6c79  tificationsReply
+00022820: 272c 2027 4e6f 7469 6669 6361 7469 6f6e  ', 'Notification
+00022830: 7353 656e 644d 6573 7361 6765 4572 726f  sSendMessageErro
+00022840: 7227 2c20 274e 6f74 6966 6963 6174 696f  r', 'Notificatio
+00022850: 6e73 5365 6e64 4d65 7373 6167 6549 7465  nsSendMessageIte
+00022860: 6d27 2c20 274f 6175 7468 4572 726f 7227  m', 'OauthError'
+00022870: 2c20 274f 7264 6572 7341 6d6f 756e 7427  , 'OrdersAmount'
+00022880: 2c20 274f 7264 6572 7341 6d6f 756e 7449  , 'OrdersAmountI
+00022890: 7465 6d27 2c20 274f 7264 6572 734f 7264  tem', 'OrdersOrd
+000228a0: 6572 272c 2027 4f72 6465 7273 5375 6273  er', 'OrdersSubs
+000228b0: 6372 6970 7469 6f6e 272c 2027 4f77 6e65  cription', 'Owne
+000228c0: 7253 7461 7465 272c 2027 5061 6765 7350  rState', 'PagesP
+000228d0: 7269 7661 6379 5365 7474 696e 6773 272c  rivacySettings',
+000228e0: 2027 5061 6765 7357 696b 6970 6167 6527   'PagesWikipage'
+000228f0: 2c20 2750 6167 6573 5769 6b69 7061 6765  , 'PagesWikipage
+00022900: 4675 6c6c 272c 2027 5061 6765 7357 696b  Full', 'PagesWik
+00022910: 6970 6167 6548 6973 746f 7279 272c 2027  ipageHistory', '
+00022920: 5068 6f74 6f73 496d 6167 6527 2c20 2750  PhotosImage', 'P
+00022930: 686f 746f 7349 6d61 6765 5479 7065 272c  hotosImageType',
+00022940: 2027 5068 6f74 6f73 5068 6f74 6f27 2c20   'PhotosPhoto', 
+00022950: 2750 686f 746f 7350 686f 746f 416c 6275  'PhotosPhotoAlbu
+00022960: 6d27 2c20 2750 686f 746f 7350 686f 746f  m', 'PhotosPhoto
+00022970: 416c 6275 6d46 756c 6c27 2c20 2750 686f  AlbumFull', 'Pho
+00022980: 746f 7350 686f 746f 4661 6c73 6561 626c  tosPhotoFalseabl
+00022990: 6527 2c20 2750 686f 746f 7350 686f 746f  e', 'PhotosPhoto
+000229a0: 4675 6c6c 5874 7252 6561 6c4f 6666 7365  FullXtrRealOffse
+000229b0: 7427 2c20 2750 686f 746f 7350 686f 746f  t', 'PhotosPhoto
+000229c0: 5369 7a65 7327 2c20 2750 686f 746f 7350  Sizes', 'PhotosP
+000229d0: 686f 746f 5369 7a65 7354 7970 6527 2c20  hotoSizesType', 
+000229e0: 2750 686f 746f 7350 686f 746f 5461 6727  'PhotosPhotoTag'
+000229f0: 2c20 2750 686f 746f 7350 686f 746f 5570  , 'PhotosPhotoUp
+00022a00: 6c6f 6164 272c 2027 5068 6f74 6f73 5068  load', 'PhotosPh
+00022a10: 6f74 6f58 7472 5265 616c 4f66 6673 6574  otoXtrRealOffset
+00022a20: 272c 2027 5068 6f74 6f73 5068 6f74 6f58  ', 'PhotosPhotoX
+00022a30: 7472 5461 6749 6e66 6f27 2c20 2750 686f  trTagInfo', 'Pho
+00022a40: 746f 7354 6167 7353 7567 6765 7374 696f  tosTagsSuggestio
+00022a50: 6e49 7465 6d27 2c20 2750 686f 746f 7354  nItem', 'PhotosT
+00022a60: 6167 7353 7567 6765 7374 696f 6e49 7465  agsSuggestionIte
+00022a70: 6d42 7574 746f 6e27 2c20 2750 6f64 6361  mButton', 'Podca
+00022a80: 7374 436f 7665 7227 2c20 2750 6f64 6361  stCover', 'Podca
+00022a90: 7374 4578 7465 726e 616c 4461 7461 272c  stExternalData',
+00022aa0: 2027 506f 6c6c 7341 6e73 7765 7227 2c20   'PollsAnswer', 
+00022ab0: 2750 6f6c 6c73 4261 636b 6772 6f75 6e64  'PollsBackground
+00022ac0: 272c 2027 506f 6c6c 7346 7269 656e 6427  ', 'PollsFriend'
+00022ad0: 2c20 2750 6f6c 6c73 506f 6c6c 272c 2027  , 'PollsPoll', '
+00022ae0: 506f 6c6c 7350 6f6c 6c41 6e6f 6e79 6d6f  PollsPollAnonymo
+00022af0: 7573 272c 2027 506f 6c6c 7356 6f74 6572  us', 'PollsVoter
+00022b00: 7327 2c20 2750 6f6c 6c73 566f 7465 7273  s', 'PollsVoters
+00022b10: 5573 6572 7327 2c20 2750 7265 7474 7943  Users', 'PrettyC
+00022b20: 6172 6473 5072 6574 7479 4361 7264 272c  ardsPrettyCard',
+00022b30: 2027 5072 6574 7479 4361 7264 7350 7265   'PrettyCardsPre
+00022b40: 7474 7943 6172 644f 7245 7272 6f72 272c  ttyCardOrError',
+00022b50: 2027 5365 6172 6368 4869 6e74 272c 2027   'SearchHint', '
+00022b60: 5365 6172 6368 4869 6e74 5365 6374 696f  SearchHintSectio
+00022b70: 6e27 2c20 2753 6561 7263 6848 696e 7454  n', 'SearchHintT
+00022b80: 7970 6527 2c20 2753 6563 7572 6547 6976  ype', 'SecureGiv
+00022b90: 6545 7665 6e74 5374 6963 6b65 7249 7465  eEventStickerIte
+00022ba0: 6d27 2c20 2753 6563 7572 654c 6576 656c  m', 'SecureLevel
+00022bb0: 272c 2027 5365 6375 7265 5365 7443 6f75  ', 'SecureSetCou
+00022bc0: 6e74 6572 4974 656d 272c 2027 5365 6375  nterItem', 'Secu
+00022bd0: 7265 536d 734e 6f74 6966 6963 6174 696f  reSmsNotificatio
+00022be0: 6e27 2c20 2753 6563 7572 6554 6f6b 656e  n', 'SecureToken
+00022bf0: 4368 6563 6b65 6427 2c20 2753 6563 7572  Checked', 'Secur
+00022c00: 6554 7261 6e73 6163 7469 6f6e 272c 2027  eTransaction', '
+00022c10: 5374 6174 7341 6374 6976 6974 7927 2c20  StatsActivity', 
+00022c20: 2753 7461 7473 4369 7479 272c 2027 5374  'StatsCity', 'St
+00022c30: 6174 7343 6f75 6e74 7279 272c 2027 5374  atsCountry', 'St
+00022c40: 6174 7350 6572 696f 6427 2c20 2753 7461  atsPeriod', 'Sta
+00022c50: 7473 5265 6163 6827 2c20 2753 7461 7473  tsReach', 'Stats
+00022c60: 5365 7841 6765 272c 2027 5374 6174 7356  SexAge', 'StatsV
+00022c70: 6965 7773 272c 2027 5374 6174 7357 616c  iews', 'StatsWal
+00022c80: 6c70 6f73 7453 7461 7427 2c20 2753 7461  lpostStat', 'Sta
+00022c90: 7475 7353 7461 7475 7327 2c20 2753 7469  tusStatus', 'Sti
+00022ca0: 636b 6572 7349 6d61 6765 5365 7427 2c20  ckersImageSet', 
+00022cb0: 2753 746f 7261 6765 5661 6c75 6527 2c20  'StorageValue', 
+00022cc0: 2753 746f 7265 5072 6f64 7563 7427 2c20  'StoreProduct', 
+00022cd0: 2753 746f 7265 5072 6f64 7563 7449 636f  'StoreProductIco
+00022ce0: 6e27 2c20 2753 746f 7265 5374 6963 6b65  n', 'StoreSticke
+00022cf0: 7273 4b65 7977 6f72 6427 2c20 2753 746f  rsKeyword', 'Sto
+00022d00: 7265 5374 6963 6b65 7273 4b65 7977 6f72  reStickersKeywor
+00022d10: 6453 7469 636b 6572 272c 2027 5374 6f72  dSticker', 'Stor
+00022d20: 6553 7469 636b 6572 734b 6579 776f 7264  eStickersKeyword
+00022d30: 5374 6963 6b65 7273 272c 2027 5374 6f72  Stickers', 'Stor
+00022d40: 6965 7343 6c69 636b 6162 6c65 4172 6561  iesClickableArea
+00022d50: 272c 2027 5374 6f72 6965 7343 6c69 636b  ', 'StoriesClick
+00022d60: 6162 6c65 5374 6963 6b65 7227 2c20 2753  ableSticker', 'S
+00022d70: 746f 7269 6573 436c 6963 6b61 626c 6553  toriesClickableS
+00022d80: 7469 636b 6572 7327 2c20 2753 746f 7269  tickers', 'Stori
+00022d90: 6573 4665 6564 4974 656d 272c 2027 5374  esFeedItem', 'St
+00022da0: 6f72 6965 7350 726f 6d6f 426c 6f63 6b27  oriesPromoBlock'
+00022db0: 2c20 2753 746f 7269 6573 5265 706c 6965  , 'StoriesReplie
+00022dc0: 7327 2c20 2753 746f 7269 6573 5374 6174  s', 'StoriesStat
+00022dd0: 4c69 6e65 272c 2027 5374 6f72 6965 7353  Line', 'StoriesS
+00022de0: 746f 7279 272c 2027 5374 6f72 6965 7353  tory', 'StoriesS
+00022df0: 746f 7279 4c69 6e6b 272c 2027 5374 6f72  toryLink', 'Stor
+00022e00: 6965 7353 746f 7279 5374 6174 7327 2c20  iesStoryStats', 
+00022e10: 2753 746f 7269 6573 5374 6f72 7953 7461  'StoriesStorySta
+00022e20: 7473 5374 6174 272c 2027 5374 6f72 6965  tsStat', 'Storie
+00022e30: 7353 746f 7279 5374 6174 7353 7461 7465  sStoryStatsState
+00022e40: 272c 2027 5374 6f72 6965 7353 746f 7279  ', 'StoriesStory
+00022e50: 5479 7065 272c 2027 5374 6f72 6965 7355  Type', 'StoriesU
+00022e60: 706c 6f61 644c 696e 6b54 6578 7427 2c20  ploadLinkText', 
+00022e70: 2753 746f 7269 6573 5669 6577 6572 7349  'StoriesViewersI
+00022e80: 7465 6d27 2c20 2755 7365 7273 4361 7265  tem', 'UsersCare
+00022e90: 6572 272c 2027 5573 6572 7345 7870 6f72  er', 'UsersExpor
+00022ea0: 7473 272c 2027 5573 6572 7346 6965 6c64  ts', 'UsersField
+00022eb0: 7327 2c20 2755 7365 7273 4c61 7374 5365  s', 'UsersLastSe
+00022ec0: 656e 272c 2027 5573 6572 734d 696c 6974  en', 'UsersMilit
+00022ed0: 6172 7927 2c20 2755 7365 7273 4f63 6375  ary', 'UsersOccu
+00022ee0: 7061 7469 6f6e 272c 2027 5573 6572 734f  pation', 'UsersO
+00022ef0: 6e6c 696e 6549 6e66 6f27 2c20 2755 7365  nlineInfo', 'Use
+00022f00: 7273 5065 7273 6f6e 616c 272c 2027 5573  rsPersonal', 'Us
+00022f10: 6572 7352 656c 6174 6976 6527 2c20 2755  ersRelative', 'U
+00022f20: 7365 7273 5363 686f 6f6c 272c 2027 5573  sersSchool', 'Us
+00022f30: 6572 7353 7562 7363 7269 7074 696f 6e73  ersSubscriptions
+00022f40: 4974 656d 272c 2027 5573 6572 7355 6e69  Item', 'UsersUni
+00022f50: 7665 7273 6974 7927 2c20 2755 7365 7273  versity', 'Users
+00022f60: 5573 6572 272c 2027 5573 6572 7355 7365  User', 'UsersUse
+00022f70: 7243 6f6e 6e65 6374 696f 6e73 272c 2027  rConnections', '
+00022f80: 5573 6572 7355 7365 7243 6f75 6e74 6572  UsersUserCounter
+00022f90: 7327 2c20 2755 7365 7273 5573 6572 4675  s', 'UsersUserFu
+00022fa0: 6c6c 272c 2027 5573 6572 7355 7365 724d  ll', 'UsersUserM
+00022fb0: 696e 272c 2027 5573 6572 7355 7365 7252  in', 'UsersUserR
+00022fc0: 656c 6174 696f 6e27 2c20 2755 7365 7273  elation', 'Users
+00022fd0: 5573 6572 5365 7474 696e 6773 5874 7227  UserSettingsXtr'
+00022fe0: 2c20 2755 7365 7273 5573 6572 5479 7065  , 'UsersUserType
+00022ff0: 272c 2027 5573 6572 7355 7365 7258 7472  ', 'UsersUserXtr
+00023000: 5479 7065 272c 2027 5573 6572 7355 7365  Type', 'UsersUse
+00023010: 7273 4172 7261 7927 2c20 2755 7469 6c73  rsArray', 'Utils
+00023020: 446f 6d61 696e 5265 736f 6c76 6564 272c  DomainResolved',
+00023030: 2027 5574 696c 7344 6f6d 6169 6e52 6573   'UtilsDomainRes
+00023040: 6f6c 7665 6454 7970 6527 2c20 2755 7469  olvedType', 'Uti
+00023050: 6c73 4c61 7374 5368 6f72 7465 6e65 644c  lsLastShortenedL
+00023060: 696e 6b27 2c20 2755 7469 6c73 4c69 6e6b  ink', 'UtilsLink
+00023070: 4368 6563 6b65 6427 2c20 2755 7469 6c73  Checked', 'Utils
+00023080: 4c69 6e6b 4368 6563 6b65 6453 7461 7475  LinkCheckedStatu
+00023090: 7327 2c20 2755 7469 6c73 4c69 6e6b 5374  s', 'UtilsLinkSt
+000230a0: 6174 7327 2c20 2755 7469 6c73 4c69 6e6b  ats', 'UtilsLink
+000230b0: 5374 6174 7345 7874 656e 6465 6427 2c20  StatsExtended', 
+000230c0: 2755 7469 6c73 5368 6f72 744c 696e 6b27  'UtilsShortLink'
+000230d0: 2c20 2755 7469 6c73 5374 6174 7327 2c20  , 'UtilsStats', 
+000230e0: 2755 7469 6c73 5374 6174 7343 6974 7927  'UtilsStatsCity'
+000230f0: 2c20 2755 7469 6c73 5374 6174 7343 6f75  , 'UtilsStatsCou
+00023100: 6e74 7279 272c 2027 5574 696c 7353 7461  ntry', 'UtilsSta
+00023110: 7473 4578 7465 6e64 6564 272c 2027 5574  tsExtended', 'Ut
+00023120: 696c 7353 7461 7473 5365 7841 6765 272c  ilsStatsSexAge',
+00023130: 2027 5669 6465 6f4c 6976 6549 6e66 6f27   'VideoLiveInfo'
+00023140: 2c20 2756 6964 656f 4c69 7665 5365 7474  , 'VideoLiveSett
+00023150: 696e 6773 272c 2027 5669 6465 6f53 6176  ings', 'VideoSav
+00023160: 6552 6573 756c 7427 2c20 2756 6964 656f  eResult', 'Video
+00023170: 5669 6465 6f27 2c20 2756 6964 656f 5669  Video', 'VideoVi
+00023180: 6465 6f41 6c62 756d 272c 2027 5669 6465  deoAlbum', 'Vide
+00023190: 6f56 6964 656f 416c 6275 6d46 756c 6c27  oVideoAlbumFull'
+000231a0: 2c20 2756 6964 656f 5669 6465 6f46 696c  , 'VideoVideoFil
+000231b0: 6573 272c 2027 5669 6465 6f56 6964 656f  es', 'VideoVideo
+000231c0: 4675 6c6c 272c 2027 5669 6465 6f56 6964  Full', 'VideoVid
+000231d0: 656f 496d 6167 6527 2c20 2757 616c 6c41  eoImage', 'WallA
+000231e0: 7070 506f 7374 272c 2027 5761 6c6c 4174  ppPost', 'WallAt
+000231f0: 7461 6368 6564 4e6f 7465 272c 2027 5761  tachedNote', 'Wa
+00023200: 6c6c 4361 726f 7573 656c 4261 7365 272c  llCarouselBase',
+00023210: 2027 5761 6c6c 436f 6d6d 656e 7441 7474   'WallCommentAtt
+00023220: 6163 686d 656e 7427 2c20 2757 616c 6c43  achment', 'WallC
+00023230: 6f6d 6d65 6e74 4174 7461 6368 6d65 6e74  ommentAttachment
+00023240: 5479 7065 272c 2027 5761 6c6c 4765 6f27  Type', 'WallGeo'
+00023250: 2c20 2757 616c 6c47 6574 4669 6c74 6572  , 'WallGetFilter
+00023260: 272c 2027 5761 6c6c 4772 6166 6669 7469  ', 'WallGraffiti
+00023270: 272c 2027 5761 6c6c 506f 7374 436f 7079  ', 'WallPostCopy
+00023280: 7269 6768 7427 2c20 2757 616c 6c50 6f73  right', 'WallPos
+00023290: 7453 6f75 7263 6527 2c20 2757 616c 6c50  tSource', 'WallP
+000232a0: 6f73 7453 6f75 7263 6554 7970 6527 2c20  ostSourceType', 
+000232b0: 2757 616c 6c50 6f73 7454 7970 6527 2c20  'WallPostType', 
+000232c0: 2757 616c 6c50 6f73 7465 6450 686f 746f  'WallPostedPhoto
+000232d0: 272c 2027 5761 6c6c 5669 6577 7327 2c20  ', 'WallViews', 
+000232e0: 2757 616c 6c57 616c 6c43 6f6d 6d65 6e74  'WallWallComment
+000232f0: 272c 2027 5761 6c6c 5761 6c6c 436f 6d6d  ', 'WallWallComm
+00023300: 656e 7444 6f6e 7574 272c 2027 5761 6c6c  entDonut', 'Wall
+00023310: 5761 6c6c 436f 6d6d 656e 7444 6f6e 7574  WallCommentDonut
+00023320: 506c 6163 6568 6f6c 6465 7227 2c20 2757  Placeholder', 'W
+00023330: 616c 6c57 616c 6c70 6f73 7427 2c20 2757  allWallpost', 'W
 00023340: 616c 6c57 616c 6c70 6f73 7441 7474 6163  allWallpostAttac
-00023350: 686d 656e 7454 7970 6527 2c20 2757 616c  hmentType', 'Wal
-00023360: 6c57 616c 6c70 6f73 7443 6f6d 6d65 6e74  lWallpostComment
-00023370: 7344 6f6e 7574 272c 2027 5761 6c6c 5761  sDonut', 'WallWa
-00023380: 6c6c 706f 7374 436f 6d6d 656e 7473 446f  llpostCommentsDo
-00023390: 6e75 7450 6c61 6365 686f 6c64 6572 272c  nutPlaceholder',
-000233a0: 2027 5761 6c6c 5761 6c6c 706f 7374 446f   'WallWallpostDo
-000233b0: 6e75 7427 2c20 2757 616c 6c57 616c 6c70  nut', 'WallWallp
-000233c0: 6f73 7444 6f6e 7574 506c 6163 6568 6f6c  ostDonutPlacehol
-000233d0: 6465 7227 2c20 2757 616c 6c57 616c 6c70  der', 'WallWallp
-000233e0: 6f73 7446 756c 6c27 2c20 2757 616c 6c57  ostFull', 'WallW
-000233f0: 616c 6c70 6f73 7454 6f49 6427 2c20 2757  allpostToId', 'W
-00023400: 6964 6765 7473 436f 6d6d 656e 744d 6564  idgetsCommentMed
-00023410: 6961 272c 2027 5769 6467 6574 7343 6f6d  ia', 'WidgetsCom
-00023420: 6d65 6e74 4d65 6469 6154 7970 6527 2c20  mentMediaType', 
-00023430: 2757 6964 6765 7473 436f 6d6d 656e 7452  'WidgetsCommentR
-00023440: 6570 6c69 6573 272c 2027 5769 6467 6574  eplies', 'Widget
-00023450: 7343 6f6d 6d65 6e74 5265 706c 6965 7349  sCommentRepliesI
-00023460: 7465 6d27 2c20 2757 6964 6765 7473 5769  tem', 'WidgetsWi
-00023470: 6467 6574 436f 6d6d 656e 7427 2c20 2757  dgetComment', 'W
-00023480: 6964 6765 7473 5769 6467 6574 4c69 6b65  idgetsWidgetLike
-00023490: 7327 2c20 2757 6964 6765 7473 5769 6467  s', 'WidgetsWidg
-000234a0: 6574 5061 6765 2729 0a                   etPage').
+00023350: 686d 656e 7427 2c20 2757 616c 6c57 616c  hment', 'WallWal
+00023360: 6c70 6f73 7441 7474 6163 686d 656e 7454  lpostAttachmentT
+00023370: 7970 6527 2c20 2757 616c 6c57 616c 6c70  ype', 'WallWallp
+00023380: 6f73 7443 6f6d 6d65 6e74 7344 6f6e 7574  ostCommentsDonut
+00023390: 272c 2027 5761 6c6c 5761 6c6c 706f 7374  ', 'WallWallpost
+000233a0: 436f 6d6d 656e 7473 446f 6e75 7450 6c61  CommentsDonutPla
+000233b0: 6365 686f 6c64 6572 272c 2027 5761 6c6c  ceholder', 'Wall
+000233c0: 5761 6c6c 706f 7374 446f 6e75 7427 2c20  WallpostDonut', 
+000233d0: 2757 616c 6c57 616c 6c70 6f73 7444 6f6e  'WallWallpostDon
+000233e0: 7574 506c 6163 6568 6f6c 6465 7227 2c20  utPlaceholder', 
+000233f0: 2757 616c 6c57 616c 6c70 6f73 7446 756c  'WallWallpostFul
+00023400: 6c27 2c20 2757 616c 6c57 616c 6c70 6f73  l', 'WallWallpos
+00023410: 7454 6f49 6427 2c20 2757 6964 6765 7473  tToId', 'Widgets
+00023420: 436f 6d6d 656e 744d 6564 6961 272c 2027  CommentMedia', '
+00023430: 5769 6467 6574 7343 6f6d 6d65 6e74 4d65  WidgetsCommentMe
+00023440: 6469 6154 7970 6527 2c20 2757 6964 6765  diaType', 'Widge
+00023450: 7473 436f 6d6d 656e 7452 6570 6c69 6573  tsCommentReplies
+00023460: 272c 2027 5769 6467 6574 7343 6f6d 6d65  ', 'WidgetsComme
+00023470: 6e74 5265 706c 6965 7349 7465 6d27 2c20  ntRepliesItem', 
+00023480: 2757 6964 6765 7473 5769 6467 6574 436f  'WidgetsWidgetCo
+00023490: 6d6d 656e 7427 2c20 2757 6964 6765 7473  mment', 'Widgets
+000234a0: 5769 6467 6574 4c69 6b65 7327 2c20 2757  WidgetLikes', 'W
+000234b0: 6964 6765 7473 5769 6467 6574 5061 6765  idgetsWidgetPage
+000234c0: 2729 0a                                  ').
```

### Comparing `kavk_api-0.9.7.4/kavk_api/types/responses.py` & `kavk_api-0.9.9/kavk_api/types/responses.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.4/PKG-INFO` & `kavk_api-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kavk-api
-Version: 0.9.7.4
+Version: 0.9.9
 Summary: 
 License: MIT
 Author: Kravandir
 Author-email: kravandir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,26 +34,24 @@
 
 Установка
 ---------
 ``pip install kavk_api``
 
 TODO:
 -------
-* работа над `UserLongPoll`_ (Типизация ивентов, фиксы багов)
 * замена asyncio.run()
 
-.. _UserLongPoll: https://dev.vk.com/api/user-long-poll/getting-started
 
 Пример:
 -------
 .. code-block:: python
 
         import asyncio
         from kavk_api import Vk
-        from kavk_api.bot_longpoll import BotLongPoll
+        from kavk_api.bot import BotLongPoll
 
         async def main():
             vk = Vk('token')
             longpoll = LongPoll(vk)
             await vk.wall.post(message="Привет kavk_api!")
             async for event in longpoll.listen():
                 print(event.type, event.object)
```

