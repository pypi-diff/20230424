# Comparing `tmp/rubpy-6.0.4.tar.gz` & `tmp/rubpy-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.0.4.tar", last modified: Fri Apr 21 01:44:12 2023, max compression
+gzip compressed data, was "rubpy-6.0.5.tar", last modified: Sun Apr 23 23:00:10 2023, max compression
```

## Comparing `rubpy-6.0.4.tar` & `rubpy-6.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.822224 rubpy-6.0.4/
--rw-rw-rw-   0        0        0     3351 2023-04-21 01:44:12.822224 rubpy-6.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2211 2023-04-21 01:42:49.000000 rubpy-6.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.774895 rubpy-6.0.4/rubpy/
--rw-rw-rw-   0        0        0      193 2023-04-21 01:36:02.000000 rubpy-6.0.4/rubpy/__init__.py
--rw-rw-rw-   0        0        0    11974 2023-04-16 00:00:51.000000 rubpy-6.0.4/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.790916 rubpy-6.0.4/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.806539 rubpy-6.0.4/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      909 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25221 2023-04-19 09:40:07.000000 rubpy-6.0.4/rubpy/gadgets/json_methods.py
--rw-rw-rw-   0        0        0    14160 2023-04-21 01:05:40.000000 rubpy-6.0.4/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.806539 rubpy-6.0.4/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.0.4/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.806539 rubpy-6.0.4/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.822224 rubpy-6.0.4/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15142 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.790916 rubpy-6.0.4/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3351 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 01:44:12.822224 rubpy-6.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-21 01:43:31.000000 rubpy-6.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.825636 rubpy-6.0.5/
+-rw-rw-rw-   0        0        0     3351 2023-04-23 23:00:10.825636 rubpy-6.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2211 2023-04-23 22:58:42.000000 rubpy-6.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.715755 rubpy-6.0.5/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-23 22:59:05.000000 rubpy-6.0.5/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    28909 2023-04-23 22:57:42.000000 rubpy-6.0.5/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.788873 rubpy-6.0.5/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.810063 rubpy-6.0.5/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.0.5/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25132 2023-04-23 22:57:45.000000 rubpy-6.0.5/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14156 2023-04-23 17:52:25.000000 rubpy-6.0.5/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.810063 rubpy-6.0.5/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.0.5/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.825636 rubpy-6.0.5/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.825636 rubpy-6.0.5/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.0.5/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.0.5/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:00:10.778863 rubpy-6.0.5/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3351 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-23 23:00:10.000000 rubpy-6.0.5/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 23:00:10.841257 rubpy-6.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-04-23 22:58:22.000000 rubpy-6.0.5/setup.py
```

### Comparing `rubpy-6.0.4/PKG-INFO` & `rubpy-6.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.4
+Version: 6.0.5
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
-pip3 install rubpy==6.0.4
+pip3 install rubpy==6.0.5
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.4 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.5 Summary: This is an unofficial
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
-and more. ### Installing ``` bash pip3 install rubpy==6.0.4 ```
+and more. ### Installing ``` bash pip3 install rubpy==6.0.5 ```
```

### Comparing `rubpy-6.0.4/README.md` & `rubpy-6.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,9 +66,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==6.0.4
+pip3 install rubpy==6.0.5
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
-and more. ### Installing ``` bash pip3 install rubpy==6.0.4 ```
+and more. ### Installing ``` bash pip3 install rubpy==6.0.5 ```
```

### Comparing `rubpy-6.0.4/rubpy/crypto/crypto.py` & `rubpy-6.0.5/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/gadgets/classino.py` & `rubpy-6.0.5/rubpy/gadgets/classino.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                     f' "{name}", "{result}"? correct it')
 
         if result is not None or not exception:
             if result is None:
                 result = name
             return type(result, __base, {'__name__': result, **kwargs})
 
-        raise AttributeError(f'module has no attribute ({name})')
+        raise AttributeError(f'module has no attribute ({name})')
```

### Comparing `rubpy-6.0.4/rubpy/gadgets/exceptions.py` & `rubpy-6.0.5/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/gadgets/json_methods.py` & `rubpy-6.0.5/rubpy/gadgets/grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from json import loads
-
-grouping = loads("""{
+grouping = {
     "users": {
         "Values": ["Block", "Unblock"],
         "GetUserInfo": {
             "params": {
                 "user_guid": {"types": "str"}
             }
         },
@@ -150,19 +148,20 @@
         },
         "SetGroupLink": {
             "params": {
                 "group_guid": {"types": "str"}
             }
         },
         "EditGroupInfo": {
-            "updated_parameters": true,
+            "updated_parameters": True,
             "params": {
                 "group_guid": {"types": "str"},
                 "title": {"types": ["str", "optional"]},
                 "description": {"types": ["str", "optional"]},
+                "slow_mode": {"types": ["int", "optional"]},
                 "chat_history_for_new_members": {"types": ["str", "optional"], "alloweds": ["Hidden", "Visible"]}
             }
         },
         "SetGroupAdmin": {
             "params": {
                 "group_guid": {"types": "str"},
                 "member_guid": {"types": "str"},
@@ -236,15 +235,15 @@
             "Pin","Unpin", "Text", "Gif", "File", "Image", "Voice", "Music", "Video", "FileInline", "Quiz", "Regular", "FromMin", "FromMax", "Local", "Global"], 
         "SendMessage": {
             "params": {
                 "object_guid": {"types": "str"},
                 "message": {
                     "types": ["dict", "Struct", "str", "optional"],
                     "ifs": {
-                        "str": {"func": "to_metadata", "unpack": true},
+                        "str": {"func": "to_metadata", "unpack": True},
                         "otherwise": {"cname": "sticker", "func": "to_array"}
                     } 
                 },
                 "reply_to_message_id": {
                     "types": ["str", "int", "optional"],
                     "func": "to_string"
                 },
@@ -256,15 +255,15 @@
                 "rnd": {"types": ["str", "int", "optional"], "default": {"func": "random_number"}, "func": "to_string"}
             }
         },
         "EditMessage": {
             "params": {
                 "object_guid": {"types": "str"},
                 "message_id": {"types": ["str", "int"], "func": "to_string"},
-                "text": {"types": "str", "func": "to_metadata", "unpack": true}
+                "text": {"types": "str", "func": "to_metadata", "unpack": True}
             }
         },
         "DeleteMessages": {
             "params": {
                 "object_guid": {"types": "str"},
                 "message_ids": {"types": ["int", "str", "list"], "func": "to_array"},
                 "type": {"types": ["str", "optional"], "alloweds": ["Local", "Global"], "default": "Global"}
@@ -284,19 +283,19 @@
                 "message_ids": {"types": ["int", "str", "list"], "func": "to_array"},
                 "rnd": {"types": ["str", "int", "optional"], "default": {"func": "random_number"}, "func": "to_string"}
             }
         },
         "CreatePoll": {
             "params": {
                 "object_guid": {"types": "str"},
-                "question": {"types": "str", "func": "to_metadata", "unpack": true},
+                "question": {"types": "str", "func": "to_metadata", "unpack": True},
                 "options": {"types": "list", "minimum": 2},
                 "type": {"types": ["str", "optional"], "alloweds": ["Quiz", "Regular"], "default": "Regular"},
-                "is_anonymous": {"types": ["bool", "optional"], "default": true},
-                "allows_multiple_answers": {"types": ["bool", "optional"], "default": false},
+                "is_anonymous": {"types": ["bool", "optional"], "default": True},
+                "allows_multiple_answers": {"types": ["bool", "optional"], "default": False},
                 "correct_option_index": {"types": ["str", "int", "optional"], "default": 0, "func": "to_number"},
                 "explanation": {"types": ["str", "optional"]},
                 "rnd": {"types": ["str", "int", "optional"], "default": {"func": "random_number"}, "func": "to_string"},
                 "reply_to_message_id": {"types": "int"}, "default": 0
             }
         },
         "VotePoll": {
@@ -348,26 +347,24 @@
                 "object_guid": {"types": "str"},
                 "message_ids": {"types": ["int", "str", "list"], "func": "to_array"}
             }
         },
         "GetMessages": {
             "params": {
                 "object_guid": {"types": "str"},
-                "sort": {"types": ["str", "optional"], "alloweds": ["FromMin", "FromMax"], "default": "FromMin"},
                 "min_id": {"types": ["str", "int"], "func": "to_number"},
                 "max_id": {"types": ["str", "int"], "func": "to_number"},
+                "sort": {"types": ["str", "optional"], "alloweds": ["FromMin", "FromMax"], "default": "FromMin"},
                 "limit": {"types": ["str", "int"], "func": "to_number", "default": 10},
-                "type": {"types": ["str", "optional"]}
             }
         },
         "GetMessagesInterval": {
             "params": {
                 "object_guid": {"types": "str"},
                 "middle_message_id": {"types": ["str", "int"], "func": "to_string"},
-                "type": {"types": ["str", "optional"]}
             }
         }
     },
     "channels": {
         "Values": ["Join", "Remove", "Archive", "Set", "Unset"],
         "AddChannel": {
             "params": {
@@ -382,15 +379,15 @@
         },
         "GetChannelInfo": {
             "params": {
                 "channel_guid": {"types": "str"}
             }
         },
         "EditChannelInfo": {
-            "updated_parameters": true,
+            "updated_parameters": True,
             "params": {
                 "channel_guid": {"types": "str"},
                 "title": {"types": "str"},
                 "description": {"types": ["str", "optional"]},
                 "channel_type": {"types": ["str", "optional"], "alloweds": ["Public", "Private"]},
                 "sign_messages": {"types": ["str", "optional"]}
             }
@@ -461,15 +458,15 @@
         "GetChannelAdminAccessList": {
             "params": {
                 "channel_guid": {"types": "str"},
                 "member_guid": {"types": "str"}
             }
         }
     },
-    "conracts": {
+    "contacts": {
         "Values": [],
         "DeleteContact": {
             "params": {
                 "user_guid": {"types": "str"}
             }
         },
         "AddAddressBook": {
@@ -489,15 +486,15 @@
                 "start_id": {"types": ["int", "str", "optional"], "func": "to_number"}
             }
         }
     },
     "settings": {
         "Values": ["Nobody", "Everybody", "MyContacts", "Bots", "Groups", "Contacts", "Channels", "NonConatcts"],
         "SetSetting": {
-            "updated_parameters": true,
+            "updated_parameters": True,
             "params": {
                 "show_my_last_online": {"types": ["str", "optional"], "alloweds": ["Nobody", "Everybody", "MyContacts"]},
                 "show_my_phone_number": {"types": ["str", "optional"], "alloweds": ["Nobody", "Everybody", "MyContacts"]},
                 "show_my_profile_photo": {"types": ["str", "optional"], "alloweds": ["Everybody", "MyContacts"]},
                 "link_forward_message": {"types": ["str", "optional"], "alloweds": ["Nobody", "Everybody", "MyContacts"]},
                 "can_join_chat_by": {"types": ["str", "optional"], "alloweds": ["Everybody", "MyContacts"]}
             }
@@ -517,15 +514,15 @@
         },
         "GetFolders": {
             "params": {
                 "last_state": {"types": ["int", "str"], "defualt": {"func": "timestamp"}, "func": "to_number"}
             }
         },
         "EditFolder": {
-            "updated_parameters": true,
+            "updated_parameters": True,
             "params": {
                 "cname": {"types": "str"},
                 "include_chat_types": {
                     "types": ["str", "list", "optional"],
                     "alloweds": ["Bots", "Groups", "Contacts", "Channels", "NonConatcts"], "func": "to_array", "default": []},
                 "exclude_chat_types": {
                     "types": ["str", "list", "optional"],
@@ -536,31 +533,31 @@
         },
         "DeleteFolder": {
             "params": {
                 "folder_id": {"types": "str"}
             }
         },
         "UpdateProfile": {
-            "updated_parameters": true,
+            "updated_parameters": True,
             "params": {
                 "first_name": {"types": ["str", "optional"]},
                 "last_name": {"types": ["str", "optional"]},
                 "bio": {"types": ["str", "optional"]}
             }
         },
         "UpdateUsername": {
             "params": {
                 "username": {"types": "str"}
             }
         },
-        "GetTwoPasscodeStatus": null,
-        "GetSuggestedFolders": null,
-        "GetPrivacySetting": null,
-        "GetBlockedUsers": null,
-        "GetMySessions": null,
+        "GetTwoPasscodeStatus": None,
+        "GetSuggestedFolders": None,
+        "GetPrivacySetting": None,
+        "GetBlockedUsers": None,
+        "GetMySessions": None,
         "TerminateSession": {
             "params": {
                 "session_key": {"types": "str"}
             }
         },
         "SetupTwoStepVerification": {
             "params": {
@@ -568,15 +565,15 @@
                 "hint": {"types": ["str", "int"], "func": "to_string"},
                 "recovery_email": {"types": "str"}
             }
         }
     },
     "stickers": {
         "Values": ["All", "Add", "Remove"],
-        "GetMyStickerSets": null,
+        "GetMyStickerSets": None,
         "SearchStickers": {
             "params": {
                 "search_text": {"types": ["str", "optional"], "default": ""},
                 "start_id": {"types": ["int", "str", "optional"], "func": "to_number"}
             }
         },
         "GetStickerSetByID": {
@@ -608,45 +605,45 @@
         }
 
     },
     "authorisations": {
         "Values": ["SMS", "Internal"],
         "GetDCs": {
             "urls": ["https://getdcmess.iranlms.ir/"],
-            "encrypt": false,
+            "encrypt": False,
             "params": {
                 "api_version": {"types": ["int", "str"], "func": "to_string", "default": "4"}
             }
         },
         "SignIn": {
-            "tmp_session": true,
+            "tmp_session": True,
             "params": {
                 "phone_code": {"types": "str"},
                 "phone_number": {"types": "str", "func": "get_phone"},
                 "phone_code_hash": {"types": "str"}
             }
         },
         "SendCode": {
-            "tmp_session": true,
+            "tmp_session": True,
             "params": {
                 "phone_number": {"types": "str", "func": "get_phone"},
-                "pass_key": {"types": ["str", "optional"], "default": null},
+                "pass_key": {"types": ["str", "optional"], "default": None},
                 "send_type": {"types": ["str", "optional"], "alloweds": ["SMS", "Internal"], "default": "SMS"}
             }
         },
         "RegisterDevice": {
             "params": {
-                "uaer_agent": {"types": "str", "func": "get_browser", "unpack": true},
+                "uaer_agent": {"types": "str", "func": "get_browser", "unpack": True},
                 "app_version": {"types": "str"}, 
                 "lang_code": {"types": ["str", "optional"], "default": "fa"}
             }
         },
         "LoginDisableTwoStep": {
-            "tmp_session": true,
+            "tmp_session": True,
             "params": {
                 "phone_number": {"types": "str", "func": "get_phone"},
                 "email_code": {"types": ["str", "int"], "func": "to_string"},
                 "forget_password_code_hash": {"types": "str"}
             }
         }
     }
-}""")
+}
```

### Comparing `rubpy-6.0.4/rubpy/gadgets/methods.py` & `rubpy-6.0.5/rubpy/gadgets/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from .classino import Classino
+from .grouping import grouping
 import re
 import sys
 import time
 import random
 import warnings
-from .classino import Classino
-from .json_methods import grouping
 
 class Functions:
     system_versions = {
         'Windows NT 10.0': 'Windows 10',
         'Windows NT 6.2': 'Windows 8',
         'Windows NT 6.1': 'Windows 7',
         'Windows NT 6.0': 'Windows Vista',
```

### Comparing `rubpy-6.0.4/rubpy/gadgets/thumbnail.py` & `rubpy-6.0.5/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/network/connection.py` & `rubpy-6.0.5/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/network/proxies.py` & `rubpy-6.0.5/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/sessions/sqliteSession.py` & `rubpy-6.0.5/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/sessions/stringSession.py` & `rubpy-6.0.5/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/structs/handlers.py` & `rubpy-6.0.5/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/structs/models.py` & `rubpy-6.0.5/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/structs/results.py` & `rubpy-6.0.5/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.4/rubpy/structs/struct.py` & `rubpy-6.0.5/rubpy/structs/struct.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -436,8 +436,8 @@
 
         if message_ids is None:
             message_ids = self.message_id
 
         return await self._client(
             methods.messages.DeleteMessages(
                 object_guid=object_guid,
-                message_ids=message_ids, *args, **kwargs))
+                message_ids=message_ids, *args, **kwargs))
```

### Comparing `rubpy-6.0.4/rubpy.egg-info/PKG-INFO` & `rubpy-6.0.5/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.4
+Version: 6.0.5
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
-pip3 install rubpy==6.0.4
+pip3 install rubpy==6.0.5
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.4 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.5 Summary: This is an unofficial
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
-and more. ### Installing ``` bash pip3 install rubpy==6.0.4 ```
+and more. ### Installing ``` bash pip3 install rubpy==6.0.5 ```
```

### Comparing `rubpy-6.0.4/rubpy.egg-info/SOURCES.txt` & `rubpy-6.0.5/rubpy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 rubpy.egg-info/requires.txt
 rubpy.egg-info/top_level.txt
 rubpy/crypto/__init__.py
 rubpy/crypto/crypto.py
 rubpy/gadgets/__init__.py
 rubpy/gadgets/classino.py
 rubpy/gadgets/exceptions.py
-rubpy/gadgets/json_methods.py
+rubpy/gadgets/grouping.py
 rubpy/gadgets/methods.py
 rubpy/gadgets/thumbnail.py
 rubpy/network/__init__.py
 rubpy/network/connection.py
 rubpy/network/proxies.py
 rubpy/sessions/__init__.py
 rubpy/sessions/sqliteSession.py
```

### Comparing `rubpy-6.0.4/setup.py` & `rubpy-6.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
+requirements = ['aiohttp', 'pycryptodome']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.0.4',
+    version = '6.0.5',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

