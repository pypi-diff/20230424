# Comparing `tmp/rubpy-6.0.5.tar.gz` & `tmp/rubpy-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.0.5.tar", last modified: Sun Apr 23 23:00:10 2023, max compression
+gzip compressed data, was "rubpy-6.1.0.tar", last modified: Mon Apr 24 00:07:29 2023, max compression
```

## Comparing `rubpy-6.0.5.tar` & `rubpy-6.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.825636 rubpy-6.0.5/
--rw-rw-rw-   0        0        0     3351 2023-04-23 23:00:10.825636 rubpy-6.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2211 2023-04-23 22:58:42.000000 rubpy-6.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.715755 rubpy-6.0.5/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-23 22:59:05.000000 rubpy-6.0.5/rubpy/__init__.py
--rw-rw-rw-   0        0        0    28909 2023-04-23 22:57:42.000000 rubpy-6.0.5/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.788873 rubpy-6.0.5/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.810063 rubpy-6.0.5/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.0.5/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25132 2023-04-23 22:57:45.000000 rubpy-6.0.5/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14156 2023-04-23 17:52:25.000000 rubpy-6.0.5/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.810063 rubpy-6.0.5/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.0.5/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.825636 rubpy-6.0.5/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.825636 rubpy-6.0.5/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.0.5/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.778863 rubpy-6.0.5/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3351 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 23:00:10.841257 rubpy-6.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-04-23 22:58:22.000000 rubpy-6.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.222798 rubpy-6.1.0/
+-rw-rw-rw-   0        0        0     3347 2023-04-24 00:07:29.207178 rubpy-6.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2207 2023-04-24 00:06:56.000000 rubpy-6.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.191556 rubpy-6.1.0/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-24 00:07:06.000000 rubpy-6.1.0/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    29264 2023-04-24 00:05:02.000000 rubpy-6.1.0/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.0/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25878 2023-04-24 00:03:50.000000 rubpy-6.1.0/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 rubpy-6.1.0/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.1.0/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.0/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.0/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-24 00:07:29.207178 rubpy-6.1.0/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 00:07:29.000000 rubpy-6.1.0/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 00:07:29.222798 rubpy-6.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-04-24 00:06:27.000000 rubpy-6.1.0/setup.py
```

### Comparing `rubpy-6.0.5/PKG-INFO` & `rubpy-6.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.5
+Version: 6.1.0
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -91,9 +91,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==6.0.5
+pip3 install -U rubpy
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.5 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.0 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -31,8 +31,8 @@
 Install Rubpy with pip and start building your applications right away. -
 **Easy**: Makes the Rubika API simple and intuitive, while still allowing
 advanced usages. - **Elegant**: Low-level details are abstracted and re-
 presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
 high-performance cryptography library written in C. - **Async**: Fully
 asynchronous (also usable synchronously if wanted, for convenience). -
 **Powerful**: Full access to Rubika's API to execute any official client action
-and more. ### Installing ``` bash pip3 install rubpy==6.0.5 ```
+and more. ### Installing ``` bash pip3 install -U rubpy ```
```

### Comparing `rubpy-6.0.5/README.md` & `rubpy-6.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,9 +66,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==6.0.5
+pip3 install -U rubpy
 ```
```

#### html2text {}

```diff
@@ -16,8 +16,8 @@
 Install Rubpy with pip and start building your applications right away. -
 **Easy**: Makes the Rubika API simple and intuitive, while still allowing
 advanced usages. - **Elegant**: Low-level details are abstracted and re-
 presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
 high-performance cryptography library written in C. - **Async**: Fully
 asynchronous (also usable synchronously if wanted, for convenience). -
 **Powerful**: Full access to Rubika's API to execute any official client action
-and more. ### Installing ``` bash pip3 install rubpy==6.0.5 ```
+and more. ### Installing ``` bash pip3 install -U rubpy ```
```

### Comparing `rubpy-6.0.5/rubpy/client.py` & `rubpy-6.1.0/rubpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,21 +327,30 @@
     async def get_group_link(self, group_guid: str):
         return await self(methods.groups.GetGroupLink(group_guid))
 
     async def set_group_link(self, group_guid: str):
         return await self(methods.groups.SetGroupLink(group_guid))
 
     async def edit_group_info(self,
-        group_guid: str,
-        title: str = None,
-        description: str = None,
-        chat_history_for_new_members: str = None,
-    ):
+         group_guid: str,
+         title: str = None,
+         description: str = None,
+         chat_history_for_new_members: str = None,
+     ):
+        updated_parameters = []
+
+        if title:
+            updated_parameters.append('title')
+        if description:
+            updated_parameters.append('description')
+        if chat_history_for_new_members:
+            updated_parameters.append('chat_history_for_new_members')
+
         return await self(methods.groups.EditGroupInfo(
-            group_guid, title, description, chat_history_for_new_members))
+            group_guid, updated_parameters, title, description, chat_history_for_new_members))
 
     async def set_group_admin(self,
         group_guid: str,
         member_guid: str,
         access_list: list,
         action: str = 'SetAdmin',
     ):
@@ -377,15 +386,15 @@
     async def delete_no_access_group_chat(self, group_guid: str):
         return await self(methods.groups.DeleteNoAccessGroupChat(group_guid))
 
     async def get_group_admin_access_list(self, group_guid: str, member_guid: str):
         return await self(methods.groups.GetGroupAdminAccessList(group_guid, member_guid))
 
     async def set_group_timer(self, group_guid: str, time: int):
-        return await self(methods.groups.EditGroupInfo(group_guid, slow_mode=time))
+        return await self(methods.groups.EditGroupInfo(group_guid, slow_mode=time, updated_parameters=['slow_mode']))
 
 # Messages Methods
 
     async def send_message(self,
         object_guid: str,
         message=None,
         reply_to_message_id: str = None,
```

### Comparing `rubpy-6.0.5/rubpy/crypto/crypto.py` & `rubpy-6.1.0/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/gadgets/classino.py` & `rubpy-6.1.0/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/gadgets/exceptions.py` & `rubpy-6.1.0/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/gadgets/grouping.py` & `rubpy-6.1.0/rubpy/gadgets/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,19 @@
                 "group_guid": {"types": "str"}
             }
         },
         "EditGroupInfo": {
             "updated_parameters": True,
             "params": {
                 "group_guid": {"types": "str"},
+                "updated_parameters": {"types": ["list"], "alloweds": ["title", "description", "slow_mode", "chat_history_for_new_members"]},
                 "title": {"types": ["str", "optional"]},
                 "description": {"types": ["str", "optional"]},
-                "slow_mode": {"types": ["int", "optional"]},
-                "chat_history_for_new_members": {"types": ["str", "optional"], "alloweds": ["Hidden", "Visible"]}
+                "slow_mode": {"types": ["int", "str", "optional"]},
+                "chat_history_for_new_members": {"types": ["str", "optional"], "alloweds": ["Hidden", "Visible"]},
             }
         },
         "SetGroupAdmin": {
             "params": {
                 "group_guid": {"types": "str"},
                 "member_guid": {"types": "str"},
                 "access_list": {"types": ["str", "list"], "alloweds": ["SetAdmin", "BanMember", "ChangeInfo", "PinMessages", "SetJoinLink", "SetMemberAccess", "DeleteGlobalAllMessages"], "func": "to_array"},
@@ -382,14 +383,15 @@
                 "channel_guid": {"types": "str"}
             }
         },
         "EditChannelInfo": {
             "updated_parameters": True,
             "params": {
                 "channel_guid": {"types": "str"},
+                "updated_parameters": {"types": ["list"], "alloweds": ["title", "description", "channel_type", "sign_messages"]},
                 "title": {"types": "str"},
                 "description": {"types": ["str", "optional"]},
                 "channel_type": {"types": ["str", "optional"], "alloweds": ["Public", "Private"]},
                 "sign_messages": {"types": ["str", "optional"]}
             }
         },
         "JoinChannelAction": {
@@ -488,14 +490,15 @@
         }
     },
     "settings": {
         "Values": ["Nobody", "Everybody", "MyContacts", "Bots", "Groups", "Contacts", "Channels", "NonConatcts"],
         "SetSetting": {
             "updated_parameters": True,
             "params": {
+                "updated_parameters": {"types": ["list"], "alloweds": ["show_my_last_online", "show_my_phone_number", "show_my_profile_photo", "link_forward_message", "can_join_chat_by"]},
                 "show_my_last_online": {"types": ["str", "optional"], "alloweds": ["Nobody", "Everybody", "MyContacts"]},
                 "show_my_phone_number": {"types": ["str", "optional"], "alloweds": ["Nobody", "Everybody", "MyContacts"]},
                 "show_my_profile_photo": {"types": ["str", "optional"], "alloweds": ["Everybody", "MyContacts"]},
                 "link_forward_message": {"types": ["str", "optional"], "alloweds": ["Nobody", "Everybody", "MyContacts"]},
                 "can_join_chat_by": {"types": ["str", "optional"], "alloweds": ["Everybody", "MyContacts"]}
             }
         },
@@ -516,14 +519,15 @@
             "params": {
                 "last_state": {"types": ["int", "str"], "defualt": {"func": "timestamp"}, "func": "to_number"}
             }
         },
         "EditFolder": {
             "updated_parameters": True,
             "params": {
+                "updated_parameters": {"types": ["list"], "alloweds": ["include_chat_types", "exclude_chat_types", "include_object_guids", "exclude_object_guids"]},
                 "cname": {"types": "str"},
                 "include_chat_types": {
                     "types": ["str", "list", "optional"],
                     "alloweds": ["Bots", "Groups", "Contacts", "Channels", "NonConatcts"], "func": "to_array", "default": []},
                 "exclude_chat_types": {
                     "types": ["str", "list", "optional"],
                     "alloweds": ["Bots", "Groups", "Contacts", "Channels", "NonConatcts"], "func": "to_array", "default": []},
@@ -535,14 +539,15 @@
             "params": {
                 "folder_id": {"types": "str"}
             }
         },
         "UpdateProfile": {
             "updated_parameters": True,
             "params": {
+                "updated_parameters": {"types": ["list"], "alloweds": ["first_name", "last_name", "bio"]},
                 "first_name": {"types": ["str", "optional"]},
                 "last_name": {"types": ["str", "optional"]},
                 "bio": {"types": ["str", "optional"]}
             }
         },
         "UpdateUsername": {
             "params": {
```

### Comparing `rubpy-6.0.5/rubpy/gadgets/methods.py` & `rubpy-6.1.0/rubpy/gadgets/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,14 +365,15 @@
                 self.request = {
                     'method': self.method_name, 'input': self.request}
 
             self.request['urls'] = self.method.get('urls')
             self.request['encrypt'] = self.method.get('encrypt', True)
             self.request['tmp_session'] = bool(self.method.get('tmp_session'))
 
+            #print(self.request)
             return self.request
         else:
             return {
                 'urls': None,
                 'input': {},
                 'method': self.method_name,
                 'encrypt': True,
```

### Comparing `rubpy-6.0.5/rubpy/gadgets/thumbnail.py` & `rubpy-6.1.0/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/network/connection.py` & `rubpy-6.1.0/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/network/proxies.py` & `rubpy-6.1.0/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/sessions/sqliteSession.py` & `rubpy-6.1.0/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/sessions/stringSession.py` & `rubpy-6.1.0/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/structs/handlers.py` & `rubpy-6.1.0/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/structs/models.py` & `rubpy-6.1.0/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/structs/results.py` & `rubpy-6.1.0/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy/structs/struct.py` & `rubpy-6.1.0/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/rubpy.egg-info/PKG-INFO` & `rubpy-6.1.0/rubpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.5
+Version: 6.1.0
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -91,9 +91,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==6.0.5
+pip3 install -U rubpy
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.5 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.0 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -31,8 +31,8 @@
 Install Rubpy with pip and start building your applications right away. -
 **Easy**: Makes the Rubika API simple and intuitive, while still allowing
 advanced usages. - **Elegant**: Low-level details are abstracted and re-
 presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
 high-performance cryptography library written in C. - **Async**: Fully
 asynchronous (also usable synchronously if wanted, for convenience). -
 **Powerful**: Full access to Rubika's API to execute any official client action
-and more. ### Installing ``` bash pip3 install rubpy==6.0.5 ```
+and more. ### Installing ``` bash pip3 install -U rubpy ```
```

### Comparing `rubpy-6.0.5/rubpy.egg-info/SOURCES.txt` & `rubpy-6.1.0/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.5/setup.py` & `rubpy-6.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.0.5',
+    version = '6.1.0',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

