# Comparing `tmp/qinglan-bot-0.0.8.tar.gz` & `tmp/qinglan-bot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qinglan-bot-0.0.8.tar", last modified: Mon Feb 20 14:38:29 2023, max compression
+gzip compressed data, was "qinglan-bot-0.1.0.tar", last modified: Mon Apr 24 13:04:44 2023, max compression
```

## Comparing `qinglan-bot-0.0.8.tar` & `qinglan-bot-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.671998 qinglan-bot-0.0.8/
--rw-rw-rw-   0        0        0    35184 2023-01-24 12:09:17.000000 qinglan-bot-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3695 2023-02-20 14:38:29.670618 qinglan-bot-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3213 2023-01-24 15:27:00.000000 qinglan-bot-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.607584 qinglan-bot-0.0.8/qinglan_bot/
--rw-rw-rw-   0        0        0      558 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.621548 qinglan-bot-0.0.8/qinglan_bot/cli/
--rw-rw-rw-   0        0        0      208 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/cli/__init__.py
--rw-rw-rw-   0        0        0      819 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/cli/bot.py
--rw-rw-rw-   0        0        0     1230 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/cli/utils.py
--rw-rw-rw-   0        0        0       65 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/cli_start.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.624539 qinglan-bot-0.0.8/qinglan_bot/database/
--rw-rw-rw-   0        0        0       18 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/database/__init__.py
--rw-rw-rw-   0        0        0     7753 2023-02-15 13:23:03.000000 qinglan-bot-0.0.8/qinglan_bot/database/db.py
--rw-rw-rw-   0        0        0     1796 2023-02-15 13:17:36.000000 qinglan-bot-0.0.8/qinglan_bot/database/models.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.630558 qinglan-bot-0.0.8/qinglan_bot/plugins/
--rw-rw-rw-   0        0        0      198 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/__init__.py
--rw-rw-rw-   0        0        0      907 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/auto_delete.py
--rw-rw-rw-   0        0        0      715 2023-02-15 12:11:25.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/connected_servers.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.633516 qinglan-bot-0.0.8/qinglan_bot/plugins/display_server_name/
--rw-rw-rw-   0        0        0       39 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/display_server_name/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/display_server_name/display_off.py
--rw-rw-rw-   0        0        0     1393 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/display_server_name/display_on.py
--rw-rw-rw-   0        0        0      728 2023-02-12 13:11:40.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/help.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.635511 qinglan-bot-0.0.8/qinglan_bot/plugins/on_msg/
--rw-rw-rw-   0        0        0      888 2023-02-20 14:20:22.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/on_msg/__init__.py
--rw-rw-rw-   0        0        0     8203 2023-02-20 14:22:20.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/on_msg/data_source.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.640496 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/
--rw-rw-rw-   0        0        0     1311 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/__init__.py
--rw-rw-rw-   0        0        0     1286 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/change_ip.py
--rw-rw-rw-   0        0        0     1324 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/change_password.py
--rw-rw-rw-   0        0        0     1308 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/change_port.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.643488 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_cmd/
--rw-rw-rw-   0        0        0       41 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_cmd/__init__.py
--rw-rw-rw-   0        0        0     1252 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py
--rw-rw-rw-   0        0        0     1243 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.647477 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_msg/
--rw-rw-rw-   0        0        0       41 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_msg/__init__.py
--rw-rw-rw-   0        0        0     1252 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py
--rw-rw-rw-   0        0        0     1243 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.650472 qinglan-bot-0.0.8/qinglan_bot/plugins/send_group_name/
--rw-rw-rw-   0        0        0       33 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/send_group_name/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/send_group_name/send_off.py
--rw-rw-rw-   0        0        0     1094 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/send_group_name/send_on.py
--rw-rw-rw-   0        0        0      757 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/servers.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.655458 qinglan-bot-0.0.8/qinglan_bot/plugins/sub/
--rw-rw-rw-   0        0        0       45 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/sub/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/sub/add_sub.py
--rw-rw-rw-   0        0        0     1418 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/sub/delete_sub.py
--rw-rw-rw-   0        0        0     1065 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/plugins/sub/sub_list.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.669616 qinglan-bot-0.0.8/qinglan_bot/utils/
--rw-rw-rw-   0        0        0    14245 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/utils/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/utils/config.py
--rw-rw-rw-   0        0        0      538 2023-02-07 07:04:52.000000 qinglan-bot-0.0.8/qinglan_bot/ws_server.py
-drwxrwxrwx   0        0        0        0 2023-02-20 14:38:29.617558 qinglan-bot-0.0.8/qinglan_bot.egg-info/
--rw-rw-rw-   0        0        0     3695 2023-02-20 14:38:29.000000 qinglan-bot-0.0.8/qinglan_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1653 2023-02-20 14:38:29.000000 qinglan-bot-0.0.8/qinglan_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 14:38:29.000000 qinglan-bot-0.0.8/qinglan_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-02-20 14:38:29.000000 qinglan-bot-0.0.8/qinglan_bot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-02-20 14:38:29.000000 qinglan-bot-0.0.8/qinglan_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-20 14:38:29.000000 qinglan-bot-0.0.8/qinglan_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-20 14:38:29.671998 qinglan-bot-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1390 2023-02-20 14:35:10.000000 qinglan-bot-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.680428 qinglan-bot-0.1.0/
+-rw-rw-rw-   0        0        0    35184 2023-01-24 12:09:17.000000 qinglan-bot-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3695 2023-04-24 13:04:44.679427 qinglan-bot-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3213 2023-01-24 15:27:00.000000 qinglan-bot-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.643497 qinglan-bot-0.1.0/qinglan_bot/
+-rw-rw-rw-   0        0        0      651 2023-04-23 17:35:52.000000 qinglan-bot-0.1.0/qinglan_bot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.656509 qinglan-bot-0.1.0/qinglan_bot/cli/
+-rw-rw-rw-   0        0        0      208 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/cli/__init__.py
+-rw-rw-rw-   0        0        0     1039 2023-04-24 08:48:41.000000 qinglan-bot-0.1.0/qinglan_bot/cli/bot.py
+-rw-rw-rw-   0        0        0     1230 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/cli/utils.py
+-rw-rw-rw-   0        0        0       65 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/cli_start.py
+-rw-rw-rw-   0        0        0      250 2023-04-23 17:35:52.000000 qinglan-bot-0.1.0/qinglan_bot/config.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.659511 qinglan-bot-0.1.0/qinglan_bot/database/
+-rw-rw-rw-   0        0        0       20 2023-04-23 16:47:21.000000 qinglan-bot-0.1.0/qinglan_bot/database/__init__.py
+-rw-rw-rw-   0        0        0     8541 2023-04-23 17:35:52.000000 qinglan-bot-0.1.0/qinglan_bot/database/db.py
+-rw-rw-rw-   0        0        0     1796 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/database/models.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.663221 qinglan-bot-0.1.0/qinglan_bot/plugins/
+-rw-rw-rw-   0        0        0      198 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/auto_delete.py
+-rw-rw-rw-   0        0        0      865 2023-04-23 17:18:07.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/connected_servers.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.665218 qinglan-bot-0.1.0/qinglan_bot/plugins/display_server_name/
+-rw-rw-rw-   0        0        0       39 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/display_server_name/__init__.py
+-rw-rw-rw-   0        0        0     1402 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/display_server_name/display_off.py
+-rw-rw-rw-   0        0        0     1393 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/display_server_name/display_on.py
+-rw-rw-rw-   0        0        0      728 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/help.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.666420 qinglan-bot-0.1.0/qinglan_bot/plugins/on_msg/
+-rw-rw-rw-   0        0        0      994 2023-04-23 17:12:12.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/on_msg/__init__.py
+-rw-rw-rw-   0        0        0     5887 2023-04-24 09:16:25.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/on_msg/data_source.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.669418 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/
+-rw-rw-rw-   0        0        0     1169 2023-04-24 09:29:05.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/__init__.py
+-rw-rw-rw-   0        0        0     1286 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/change_ip.py
+-rw-rw-rw-   0        0        0     1324 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/change_password.py
+-rw-rw-rw-   0        0        0     1308 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/change_port.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.671419 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_cmd/
+-rw-rw-rw-   0        0        0       41 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_cmd/__init__.py
+-rw-rw-rw-   0        0        0     1252 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py
+-rw-rw-rw-   0        0        0     1243 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.673421 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_msg/
+-rw-rw-rw-   0        0        0       41 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_msg/__init__.py
+-rw-rw-rw-   0        0        0     1252 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py
+-rw-rw-rw-   0        0        0     1243 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.675423 qinglan-bot-0.1.0/qinglan_bot/plugins/send_group_name/
+-rw-rw-rw-   0        0        0       33 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/send_group_name/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/send_group_name/send_off.py
+-rw-rw-rw-   0        0        0     1094 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/send_group_name/send_on.py
+-rw-rw-rw-   0        0        0      717 2023-04-23 17:18:07.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/servers.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.678426 qinglan-bot-0.1.0/qinglan_bot/plugins/sub/
+-rw-rw-rw-   0        0        0       45 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/sub/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/sub/add_sub.py
+-rw-rw-rw-   0        0        0     1418 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/sub/delete_sub.py
+-rw-rw-rw-   0        0        0     1065 2023-04-23 13:54:19.000000 qinglan-bot-0.1.0/qinglan_bot/plugins/sub/sub_list.py
+-rw-rw-rw-   0        0        0    10864 2023-04-23 17:35:52.000000 qinglan-bot-0.1.0/qinglan_bot/utils.py
+-rw-rw-rw-   0        0        0      542 2023-04-23 17:35:52.000000 qinglan-bot-0.1.0/qinglan_bot/ws_server.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:04:44.654507 qinglan-bot-0.1.0/qinglan_bot.egg-info/
+-rw-rw-rw-   0        0        0     3695 2023-04-24 13:04:44.000000 qinglan-bot-0.1.0/qinglan_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2023-04-24 13:04:44.000000 qinglan-bot-0.1.0/qinglan_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:04:44.000000 qinglan-bot-0.1.0/qinglan_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-24 13:04:44.000000 qinglan-bot-0.1.0/qinglan_bot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      201 2023-04-24 13:04:44.000000 qinglan-bot-0.1.0/qinglan_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 13:04:44.000000 qinglan-bot-0.1.0/qinglan_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:04:44.680428 qinglan-bot-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1419 2023-04-24 13:02:53.000000 qinglan-bot-0.1.0/setup.py
```

### Comparing `qinglan-bot-0.0.8/LICENSE` & `qinglan-bot-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/PKG-INFO` & `qinglan-bot-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.0.8
+Version: 0.1.0
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.0.8/README.md` & `qinglan-bot-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/cli/bot.py` & `qinglan-bot-0.1.0/qinglan_bot/cli/bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import sys
-from os import path
-
+import importlib
 import nonebot
+
+from os import path
 from nonebot.adapters.onebot.v11 import Adapter
 from nonebot.log import default_format, logger
 
 nonebot.init()
 driver = nonebot.get_driver()
 driver.register_adapter(Adapter)
 app = nonebot.get_asgi()
 
 # 删除 qinglan_bot 导入，否则 nonebot 导入时会忽略
 del sys.modules["qinglan_bot"]
 nonebot.load_plugin("qinglan_bot")
-nonebot.load_plugin("nonebot_plugin_gocqhttp")
+
+tqdm_loader = importlib.util.find_spec("nonebot_plugin_gocqhttp")
+if tqdm_loader:
+    nonebot.load_plugin("nonebot_plugin_gocqhttp")
+else:
+    nonebot.logger.info("未找到 nonebot_plugin_gocqhttp 包，请使用go-cqhttp独立连接程序")
 
 # Modify some config / config depends on loaded configs
 #
 # config = nonebot.get_driver().config
 # do something...
 
 logger.add(
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/cli/utils.py` & `qinglan-bot-0.1.0/qinglan_bot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/database/db.py` & `qinglan-bot-0.1.0/qinglan_bot/database/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,51 @@
 from pathlib import Path
 from typing import Optional, List
 
 from nonebot import get_driver
+from pydantic import BaseModel
 from tortoise import Tortoise, connections
 from .models import Sub, Server, Group, Guild
-from ..utils.config import get_mc_qq_dir
-
-server_list = []
 
 
 def get_path(*other):
     """获取数据文件绝对路径"""
+    from .. import plugin_config
 
-    dir_path = Path(get_mc_qq_dir() if get_mc_qq_dir() else "./data/")
+    dir_path = Path(plugin_config.mc_qq_dir if plugin_config.mc_qq_dir else "./data/")
     if not Path(dir_path).exists():
         dir_path.mkdir()
     dir_path = dir_path.resolve()
     return str(dir_path.joinpath(*other))
 
 
+class GroupConfig(BaseModel):
+    """群配置"""
+    type: str
+    type_id: int
+    display_server_name: Optional[bool] = False
+
+
+class MinecraftServer(BaseModel):
+    """服务器配置"""
+    # 服务器名称
+    server_name: str
+    # 服务器群列表
+    all_group_list: Optional[List[GroupConfig]] = []
+    # 是否用 Rcon 发送消息
+    rcon_msg: Optional[bool] = False
+    # 是否用 Rcon 发送命令
+    rcon_cmd: Optional[bool] = False
+
+
+server_list: List[MinecraftServer] = []
+rule_group_list: List[int] = []
+rule_guild_list: List[str] = []
+
+
 class DB:
     """数据库交互类，与增删改查无关的部分不应该在这里面实现"""
 
     @classmethod
     async def init(cls):
         """初始化数据库"""
         from . import models
@@ -181,42 +204,44 @@
     async def get_sub_list(cls, type, type_id) -> List[Sub]:
         """获取指定位置的互通列表"""
         return await cls.get_subs(type=type, type_id=type_id)
 
     @classmethod
     async def delete_sub_list(cls, type, type_id):
         """删除指定位置的互通列表"""
-        async for sub in Sub.get(type=type, type_id=type_id):
+        async for sub in await Sub.get(type=type, type_id=type_id):
             await cls.delete_sub(server_name=sub.server_name, type=sub.type, type_id=sub.type_id)
         await cls.update_server_list()
 
     @classmethod
     async def update_server_list(cls):
         """更新需要推送的 服务器 主列表"""
         subs = Sub.all()
         servers = Server.all()
         server_list.clear()
         async for server in servers:
-            server_list.append(
-                {
-                    "server_name": server.server_name,
-                    "all_group_list": [],
-                    "rcon_msg": server.rcon_msg,
-                    "rcon_cmd": server.rcon_cmd,
-                }
-            )
+            server_list.append(MinecraftServer(
+                server_name=server.server_name,
+                all_group_list=[],  # 服务器的所有群聊列表
+                rcon_msg=server.rcon_msg,
+                rcon_cmd=server.rcon_cmd
+            ))
 
         for per_server in server_list:
             async for sub in subs:
-                if per_server["server_name"] == sub.server_name:
+                if per_server.server_name == sub.server_name:
                     # 向全群聊列表里装入每个互通记录
-                    per_server["all_group_list"].append(
-                        {
-                            "type": sub.type,
-                            "type_id": sub.type_id,
-                            "display_server_name": sub.display_server_name
-                        }
-                    )
+                    per_server.all_group_list.append(GroupConfig(
+                        type=sub.type,
+                        type_id=sub.type_id,
+                        display_server_name=sub.display_server_name
+                    ))
+        groups = Group.all()
+        async for group in groups:
+            rule_group_list.append(group.group_id)
+        guilds = Guild.all()
+        async for guild in guilds:
+            rule_guild_list.append(f"{guild.guild_id}:{guild.channel_id}")
 
 
 get_driver().on_startup(DB.init)
 get_driver().on_shutdown(connections.close_all)
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/database/models.py` & `qinglan-bot-0.1.0/qinglan_bot/database/models.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/auto_delete.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/auto_delete.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/connected_servers.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/connected_servers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageEvent
 
-from .on_msg.data_source import CLIENTS
+from mcqq_tool.utils import CLIENTS
 from ..utils import permission_check, to_me
 
 connected_servers = on_command("已连接服务器列表", rule=to_me(), priority=3)
 connected_servers.__doc__ = """已连接服务器列表（管理员）"""
 
 connected_servers.handle()(permission_check)
 
 
 @connected_servers.handle()
 async def _(event: MessageEvent):
     """发送所有已连接至 WebSocket 的服务器"""
     message = "已连接至 WebSocket 的服务器列表\n\n"
 
-    for per_client in CLIENTS:
-        message += f'{per_client["server_name"]}\n'
+    for server_name, server in CLIENTS.items():
+        message += (
+            f"{server_name} "
+            f"WebSocket: {'开' if server.websocket else '关'}, "
+            f"Rcon: {'开' if server.rcon else '关'}\n"
+        )
     await connected_servers.finish(message=message)
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/display_server_name/display_off.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/display_server_name/display_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/display_server_name/display_on.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/display_server_name/display_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/help.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/help.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/on_msg/__init__.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/on_msg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from nonebot import on_message, on_command
+from nonebot.adapters import Message
+from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
+from typing import Union
 
-from .data_source import send_msg_to_mc, send_command_to_mc
+from .data_source import send_msg_to_mc, send_cmd_to_mc
 from ...utils import msg_rule, permission_check
-from typing import Union
 
-mc_qq = on_message(priority=5, rule=msg_rule)
-mc_qq_command = on_command(
-    "mcc",
-    priority=3,
-    rule=msg_rule,
-    block=True
-)
-mc_qq_command.handle()(permission_check)
+mc_qq = on_message(priority=2, rule=msg_rule)
+
+mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
+
+mc_qq_cmd.handle()(permission_check)
 
 
-# 收到 群/频 道消息时
+# 收到消息时
 @mc_qq.handle()
 async def msg_first_receive(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     await send_msg_to_mc(bot=bot, event=event)
 
 
-# 收到 群/频道 命令时
-@mc_qq_command.handle()
-async def cmd_first_receive(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
-    await send_command_to_mc(bot=bot, event=event)
+# 收到命令时
+@mc_qq_cmd.handle()
+async def cmd_first_receive(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent], args: Message = CommandArg()):
+    await send_cmd_to_mc(bot=bot, event=event, cmd=args.extract_plain_text())
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/on_msg/data_source.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/on_msg/data_source.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,163 +1,111 @@
-import json
 import aiomcrcon
 import websockets
+from typing import Optional, Union, List
+from mcqq_tool.config import CLIENTS, Client
+from mcqq_tool.utils import send_msg_to_qq, remove_client, rcon_connect, get_client
 from nonebot import get_bot, logger
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
+from nonebot.adapters.onebot.v11 import GroupMessageEvent, Bot
 from nonebot_plugin_guild_patch import GuildMessageEvent
 
-from typing import Union, Optional
-from ...utils import process_msg_for_ws, send_msg_to_qq, get_type_id, process_msg_for_rcon
-from ...database.db import server_list
+from ...database.db import server_list, MinecraftServer
+from ...utils import process_msg_for_ws, process_msg_for_rcon, get_type_id
 
-CLIENTS = []
-"""客户端列表"""
 
-
-async def ws_client(websocket):
+async def ws_client(websocket: websockets.WebSocketServerProtocol):
     """WebSocket"""
     try:
         server_name = websocket.request_headers["x-self-name"].encode('utf-8').decode('unicode_escape')
-    except KeyError:
-        server_name = ""
-    # 服务器名为空
-    if not server_name:
-        logger.error("[MC_QQ]丨未获取到该服务器的名称，连接断开")
+    except KeyError as e:
+        # 服务器名为空
+        logger.error(f"[MC_QQ]丨未获取到该服务器的名称，连接断开：{e}")
         await websocket.close(1008, "[MC_QQ]丨未获取到该服务器的名称，连接断开")
         return
     else:
-        for client in CLIENTS:
-            # 重复连接
-            if server_name == client["server_name"]:
-                logger.error(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器，无需重复连接")
-                await websocket.close(1008, f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器，无需重复连接")
-                return
-    # 准备加入客户端列表
-    try:
-        from ...database import DB as db
-        server = await db.get_server(server_name=server_name)
-        # rcon状态：rcon_msg rcon_cmd rcon_password不等于默认密码
-        rcon_status = (server.rcon_msg or server.rcon_cmd) and server.rcon_password != "change_password"
-    except AttributeError:
-        rcon_status = False
-
-    if rcon_status:
-        rcon_client = aiomcrcon.Client(server.rcon_ip, server.rcon_port, server.rcon_password)
-        await rcon_connect(client=rcon_client, server_name=server_name)
-    else:
-        rcon_client: Optional[aiomcrcon.Client] = None
+        try:
+            client = CLIENTS[server_name]
+        except KeyError as e:
+            # 准备加入客户端列表
+            from ...database import DB as db
+            rcon_client: Optional[aiomcrcon.Client] = None
+            if server := await db.get_server(server_name=server_name):
+                # rcon状态：rcon_msg rcon_cmd rcon_password不等于默认密码
+                if (server.rcon_msg or server.rcon_cmd) and server.rcon_password != "change_password":
+                    rcon_client = aiomcrcon.Client(server.rcon_ip, server.rcon_port, server.rcon_password)
+                    await rcon_connect(rcon_client=rcon_client, server_name=server_name)
+            CLIENTS[server_name] = Client(server_name=server_name, websocket=websocket, rcon=rcon_client)
+            logger.success(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器")
 
-    CLIENTS.append({
-        "server_name": server_name, "ws_client": websocket, "rcon_connection": {
-            "rcon": rcon_client, "is_open": rcon_status
-        }
-    })
-    logger.success(f"[MC_QQ]丨[Server:{server_name}] 已连接至 WebSocket 服务器")
-    try:
-        async for message in websocket:
-            await send_msg_to_qq(bot=get_bot(), json_msg=json.loads(message))
-    except websockets.WebSocketException:
-        # 移除当前客户端
-        await remove_client(server_name)
-    if websocket.closed and CLIENTS:
-        await remove_client(server_name)
+            try:
+                async for message in websocket:
+                    await send_msg_to_qq(bot=get_bot(), message=message)
+            except websockets.WebSocketException as e:
+                # 移除当前客户端
+                await remove_client(server_name=server_name)
+                logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开：{e}")
+            else:
+                if websocket.closed:
+                    await remove_client(server_name=server_name)
+                    logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开")
+        else:
+            logger.error(f"[MC_QQ]丨[Server:{server_name}] 重复连接，连接断开")
+            await websocket.close(1008, f"[MC_QQ]丨[Server:{server_name}] 重复连接，连接断开")
 
 
 async def send_msg_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     """发送消息到 MC"""
     # 处理来自QQ的消息
     if client_list := await get_clients(event=event):
-        for client in client_list:
+        for client_server in client_list:
+            client = CLIENTS.get(client_server.server_name)
             # 如果 服务器的rcon已连接 且 服务器切换为rcon发送消息
-            if client["client"]["rcon_connection"]["is_open"] and client["server"]["rcon_msg"] and \
-                    client["client"]["rcon_connection"]["rcon"]:
+            if client.rcon and client_server.rcon_msg:
                 text_msg, msgJson = await process_msg_for_rcon(bot=bot, event=event)
                 try:
-                    await client["client"]["rcon_connection"]["rcon"].send_cmd(msgJson)
-                    logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client['client']['server_name']}] 的消息 \"{text_msg}\"")
+                    await client.rcon.send_cmd(msgJson)
                 except aiomcrcon.ClientNotConnectedError:
-                    logger.error(f"[MC_QQ]丨[Server:{client['client']['server_name']}] 的Rcon未连接，发送消息失败")
+                    logger.error(f"[MC_QQ]丨[Server:{client.server_name}] 的Rcon未连接，发送消息失败")
+                else:
+                    logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的消息 \"{text_msg}\"")
 
-            elif client["client"]['ws_client']:
+            elif client.websocket:
                 text_msg, msgJson = await process_msg_for_ws(bot=bot, event=event)
                 try:
-                    await client["client"]['ws_client'].send(msgJson)
-                    logger.success(f"[MC_QQ]丨发送至 [server:{client['client']['server_name']}] 的消息 \"{text_msg}\"")
+                    await client.websocket.send(msgJson)
                 except websockets.WebSocketException:
-                    logger.error(f"[MC_QQ]丨发送至 [Server:{client['client']['server_name']}] 的过程中出现了错误")
-                    await remove_client(client['client']['server_name'])
+                    logger.error(f"[MC_QQ]丨发送至 [Server:{client.server_name}] 的过程中出现了错误")
+                    await remove_client(client.server_name)
+                else:
+                    logger.success(f"[MC_QQ]丨发送至 [server:{client.server_name}] 的消息 \"{text_msg}\"")
 
 
-async def send_command_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
+async def send_cmd_to_mc(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent], cmd: str):
     """发送命令到 Minecraft"""
     if client_list := await get_clients(event=event):
-        for client in client_list:
-            if client["client"]["rcon_connection"]["is_open"] and client["server"]["rcon_cmd"] and \
-                    client["client"]["rcon_connection"]["rcon"]:
+        for client_server in client_list:
+            client = CLIENTS.get(client_server.server_name)
+
+            if client.rcon and client_server.rcon_cmd:
                 # 获取命令
-                ori_cmd = event.raw_message.strip("/").strip("mcc").strip()
                 try:
                     # 发送命令并获得返回消息
-                    back_msg = (await client["client"]["rcon_connection"]["rcon"].send_cmd(ori_cmd))[0]
+                    back_msg = await client.rcon.send_cmd(cmd)
                     # 机器人发送信息
-                    await bot.send(event, message=back_msg)
-                    logger.success(
-                        f"[MC_QQ_Rcon]丨发送至 [server:{client['client']['server_name']}] 的命令 \"{event.raw_message.strip('/mcc').strip()}\""
-                    )
+                    await bot.send(event, message=back_msg[0])
                 except aiomcrcon.ClientNotConnectedError:
-                    logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client['client']['server_name']}] 的过程中出现了错误")
                     # 连接关闭则移除客户端
-                    await remove_client(client['client']['server_name'])
+                    await remove_client(client.server_name)
+                    logger.error(f"[MC_QQ_Rcon]丨发送至 [Server:{client.server_name}] 的过程中出现了错误")
+                else:
+                    logger.success(f"[MC_QQ_Rcon]丨发送至 [server:{client.server_name}] 的命令 \"{cmd}\"")
 
 
-async def get_clients(event: Union[GroupMessageEvent, GuildMessageEvent]):
+async def get_clients(event: Union[GroupMessageEvent, GuildMessageEvent]) -> List[MinecraftServer]:
     """获取 服务器名、ws客户端、rcon连接"""
-    res = []
-    for per_client in CLIENTS:
-        for per_server in server_list:
-            # 如果 服务器名 == ws客户端中记录的服务器名，且ws客户端存在
-            if per_client['ws_client'] and per_server['server_name'] == per_client['server_name']:
-                for per_group in per_server['all_group_list']:
-                    if await get_type_id(event) == per_group["type_id"]:
-                        res.append({"client": per_client, "server": per_server})
+    res: List[MinecraftServer] = []
+    for per_server in server_list:
+        if client := get_client(per_server.server_name):
+            if client.websocket and client.server_name == per_server.server_name:
+                for per_group in per_server.all_group_list:
+                    if await get_type_id(event) == per_group.type_id:
+                        res.append(per_server)
     return res
-
-
-async def connect_rcon():
-    """服务器启动时，连接启用rcon的服务器"""
-    for server in server_list:
-        if (server.rcon_msg | server.rcon_cmd) and server.rcon_password != "change_password":
-            rcon_client = aiomcrcon.Client(server.rcon_ip, server.rcon_port, server.rcon_password)
-            try:
-                await rcon_client.connect()
-                # 连接成功后装入rcon连接列表
-                for client in CLIENTS:
-                    if server.server_name == client["server_name"]:
-                        client["rcon_connection"]["rcon"] = rcon_client
-                        client["rcon_connection"]["is_open"] = True
-                    logger.success(f"[MC_QQ]丨[Server:{client['server_name']}] 的Rcon连接成功")
-            except aiomcrcon.RCONConnectionError:
-                logger.error(f"[MC_QQ]丨[Server:{server.server_name}] 的Rcon连接失败")
-            except aiomcrcon.IncorrectPasswordError:
-                logger.error(f"[MC_QQ]丨[Server:{server.server_name}] 的Rcon密码错误")
-
-
-async def rcon_connect(client: aiomcrcon.Client, server_name: str):
-    """连接 Rcon"""
-    try:
-        await client.connect()
-        logger.success(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接成功")
-    except aiomcrcon.RCONConnectionError:
-        logger.error(f"[MC_QQ]丨[Server:{server_name}] 的Rcon连接失败")
-    except aiomcrcon.IncorrectPasswordError:
-        logger.error(f"[MC_QQ]丨[Server:{server_name}] 的Rcon密码错误")
-
-
-async def remove_client(server_name: str):
-    """移除客户端"""
-    for client in CLIENTS:
-        if server_name == client["server_name"]:
-            if client["rcon_connection"]["is_open"]:
-                await client["rcon_connection"]["rcon"].close()
-                logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 Rcon 连接已断开")
-            CLIENTS.remove(client)
-            logger.error(f"[MC_QQ]丨[Server:{server_name}] 的 WebSocket 连接已断开")
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/change_ip.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/change_ip.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/change_password.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/change_password.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon/change_port.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon/change_port.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_cmd/rcon_cmd_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_cmd/rcon_cmd_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_msg/rcon_msg_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/rcon_msg/rcon_msg_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/send_group_name/send_off.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/send_group_name/send_off.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/send_group_name/send_on.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/send_group_name/send_on.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/servers.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/servers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageEvent
 
-from ..database.models import Server
+from ..database.db import server_list
 from ..utils import permission_check, to_me
 
 servers = on_command("服务器列表", rule=to_me(), priority=3)
 
 servers.handle()(permission_check)
 
 
 @servers.handle()
 async def _(event: MessageEvent):
     """发送数据库中所有服务器"""
     message = "数据库中的服务器列表\n\n"
-    server_list = Server.all()
-    async for server in server_list:
+    for server in server_list:
         message += (
             f"{server.server_name}："
             f"Rcon_Msg：{'开' if server.rcon_msg else '关'}，"
-            f"Rcon_CMD：{'开' if server.rcon_cmd else '关'}，\n"
+            f"Rcon_CMD：{'开' if server.rcon_cmd else '关'}\n"
         )
     await servers.finish(message=message)
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/sub/add_sub.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/sub/add_sub.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/sub/delete_sub.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/sub/delete_sub.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/plugins/sub/sub_list.py` & `qinglan-bot-0.1.0/qinglan_bot/plugins/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `qinglan-bot-0.0.8/qinglan_bot/utils/__init__.py` & `qinglan-bot-0.1.0/qinglan_bot/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 from typing import Union
 
-from nonebot import logger
+from mcqq_tool.utils import get_member_nickname
+from nonebot.adapters.onebot.v11 import Message, GroupMessageEvent, Bot, GROUP_ADMIN, GROUP_OWNER, PrivateMessageEvent
 from nonebot.exception import FinishedException
 from nonebot.internal.permission import Permission
 from nonebot.internal.rule import Rule
 from nonebot.matcher import Matcher
 from nonebot.params import ArgPlainText, CommandArg
-from nonebot.adapters.onebot.v11 import Message, GroupMessageEvent, Bot, GROUP_ADMIN, GROUP_OWNER, PrivateMessageEvent
 from nonebot.permission import SUPERUSER
 from nonebot_plugin_guild_patch import ChannelDestroyedNoticeEvent, GuildMessageEvent
 
-from .config import get_mc_qq_mcrcon_guild_admin_roles, get_mc_qq_to_me
-from ..database import DB as db
-from ..database.db import server_list
+from . import plugin_config
+from .database.db import rule_group_list, rule_guild_list
 
 
 def to_me():
-    if get_mc_qq_to_me():
+    if plugin_config.mc_qq_to_me:
         from nonebot.rule import to_me
 
         return to_me()
 
     async def _to_me() -> bool:
         return True
 
@@ -33,15 +32,15 @@
         role["role_name"]
         for role in (
             await bot.get_guild_member_profile(
                 guild_id=event.guild_id, user_id=event.user_id
             )
         )["roles"]
     )
-    return bool(roles & set(get_mc_qq_mcrcon_guild_admin_roles()))
+    return bool(roles & set(plugin_config.mc_qq_guild_admin_roles))
 
 
 GUILD_ADMIN: Permission = Permission(_guild_admin)
 
 
 async def permission_check(
         bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent, PrivateMessageEvent]
@@ -83,114 +82,41 @@
 ):
     server_name = server_name.strip()
     matcher.set_arg("server_name", Message(server_name))
 
 
 async def get_type_id(event: Union[GroupMessageEvent, GuildMessageEvent, ChannelDestroyedNoticeEvent]):
     if isinstance(event, GuildMessageEvent) or isinstance(event, ChannelDestroyedNoticeEvent):
-        from ..database import DB as db
+        from .database import DB as db
         return await db.get_guild_type_id(event.guild_id, event.channel_id)
     return event.group_id
 
 
 async def msg_rule(event: Union[GroupMessageEvent, GuildMessageEvent]) -> bool:
     """Rule 消息规则"""
-    if server_list:
-        for per_server in server_list:
-            for per_group in per_server["all_group_list"]:
-                if await get_type_id(event) == per_group["type_id"]:
-                    return True
-    return False
-
-
-async def msg_to_qq_process(json_msg):
-    """处理来自MC的消息，并返回处理后的消息"""
-    message = {
-        "PlayerJoinEvent": f"{json_msg['player']['nickname']} 加入了服务器",
-        "PlayerQuitEvent": f"{json_msg['player']['nickname']} 离开了服务器",
-        "AsyncPlayerChatEvent": f"{json_msg['player']['nickname']} 说：{json_msg['message']}",
-        "PlayerDeathEvent": f"{json_msg['message']}",
-    }
-    return message[json_msg['event_name']]
-
-
-async def send_msg_to_qq(bot: Bot, json_msg):
-    """发送消息到 QQ"""
-    msg = await msg_to_qq_process(json_msg)
-    # 循环服务器列表并发送消息
-    # 如果服务器列表不为空
-    if server_list:
-        # 开始循环
-        for per_server in server_list:
-            # 如果服务器名相匹配
-            if per_server['server_name'] == json_msg['server_name']:
-                # 如果全群聊列表存在
-                if per_server['all_group_list']:
-                    # 循环全群聊列表
-                    for per_group in per_server['all_group_list']:
-                        # 是否需要发送服务器名称
-                        if per_group["display_server_name"]:
-                            msg = f"[{json_msg['server_name']}] {msg}"
-                        # 发送至群聊
-                        if per_group["type"] == "group":
-                            logger.success(
-                                f"[MC_QQ]丨from [{json_msg['server_name']}] to [群:{per_group['type_id']}] \"{msg}\"")
-                            await bot.send_group_msg(
-                                group_id=per_group['type_id'],
-                                message=msg
-                            )
-                        # 发送至频道
-                        else:
-                            guild = await db.get_guild(id=per_group['type_id'])
-                            logger.success(
-                                f"[MC_QQ]丨from [{json_msg['server_name']}] to [频道:{guild.guild_id}/{guild.channel_id}] \"{msg}\"")
-                            await bot.send_guild_channel_msg(
-                                guild_id=guild.guild_id,
-                                channel_id=guild.channel_id,
-                                message=msg
-                            )
-
-
-async def get_member_nickname(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent], user_id):
-    """获取昵称"""
-    # 判断从 群/频道 获取成员信息
     if isinstance(event, GroupMessageEvent):
-        # 如果获取发送者的昵称
-        if event.user_id == int(user_id):
-            return event.sender.card if event.sender.card else event.sender.nickname
-        # 如果获取其他人的昵称
-        else:
-            return (await bot.get_group_member_info(
-                group_id=event.group_id,
-                user_id=user_id,
-                no_cache=True
-            ))['nickname']
+        return event.group_id in rule_group_list
     elif isinstance(event, GuildMessageEvent):
-        # 返回频道成员昵称
-        if event.user_id == user_id:
-            return event.sender.nickname
-        else:
-            return (await bot.get_guild_member_profile(
-                guild_id=event.guild_id,
-                user_id=user_id))['nickname']
+        return f"{event.guild_id}:{event.channel_id}" in rule_guild_list
+    return False
 
 
 async def process_msg_for_ws(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     """处理发送至MC的信息"""
     # 获取昵称
     member_nickname = await get_member_nickname(bot, event, event.user_id)
 
     # 初始化消息
     text_msg = member_nickname + "说："
 
     # 初始化消息字典
     messageList = []
 
     # 发送群聊名称
-    from ..database import DB as db
+    from .database import DB as db
     if isinstance(event, GroupMessageEvent) and (await db.get_group(group_id=event.group_id)).send_group_name:
         group_name = {'msgType': "group_name",
                       'msgData': (await bot.get_group_info(group_id=event.group_id))['group_name']}
         messageList.append(group_name)
     elif isinstance(event, GuildMessageEvent) and (
             await db.get_guild(guild_id=event.guild_id, channel_id=event.channel_id)).send_group_name:
         group_name = {'msgType': "group_name"}
@@ -250,15 +176,15 @@
         text_msg += " "
 
         # 装入消息数据
         per_msg['msgData'] = msgData
         # 放入消息列表
         messageList.append(per_msg)
 
-    return text_msg, '{"message": ' + str(messageList) + '}'
+    return text_msg, str({"message": messageList})
 
 
 async def process_msg_for_rcon(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
     """消息处理"""
     # 获取昵称
     member_nickname = await get_member_nickname(bot, event, event.user_id)
 
@@ -267,15 +193,15 @@
 
     command_msg = "tellraw @p "
 
     message_list = [
         {"text": "[MC_QQ] ", "color": "yellow"},
     ]
     # 是否发送群聊名称
-    from ..database import DB as db
+    from .database import DB as db
     # 群
     if isinstance(event, GroupMessageEvent) and (await db.get_group(group_id=event.group_id)).send_group_name:
         message_list.append(
             {"text": (await bot.get_group_info(group_id=event.group_id))['group_name'] + " ", "color": "aqua"})
     # 频道
     elif isinstance(event, GuildMessageEvent) and (
             await db.get_guild(guild_id=event.guild_id, channel_id=event.channel_id)).send_group_name:
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot/ws_server.py` & `qinglan-bot-0.1.0/qinglan_bot/ws_server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import websockets
 from nonebot import logger
 
 from .plugins.on_msg.data_source import ws_client
-from .utils import config
+from . import plugin_config
 
 
 async def start_ws_server():
     """启动 WebSocket 服务器"""
     global ws
-    ws = await websockets.serve(ws_client, config.get_mc_qq_ws_ip(), config.get_mc_qq_ws_port())
+    ws = await websockets.serve(ws_client, plugin_config.mc_qq_ws_ip, plugin_config.mc_qq_ws_port)
     logger.success("[MC_QQ]丨WebSocket 服务器已开启")
 
 
 async def stop_ws_server():
     """关闭 WebSocket 服务器"""
     global ws
     ws.close()
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot.egg-info/PKG-INFO` & `qinglan-bot-0.1.0/qinglan_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qinglan-bot
-Version: 0.0.8
+Version: 0.1.0
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通机器人
 Home-page: https://github.com/17TheWord/qinglan_bot
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qinglan-bot-0.0.8/qinglan_bot.egg-info/SOURCES.txt` & `qinglan-bot-0.1.0/qinglan_bot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 setup.py
 qinglan_bot/__init__.py
 qinglan_bot/cli_start.py
+qinglan_bot/config.py
+qinglan_bot/utils.py
 qinglan_bot/ws_server.py
 qinglan_bot.egg-info/PKG-INFO
 qinglan_bot.egg-info/SOURCES.txt
 qinglan_bot.egg-info/dependency_links.txt
 qinglan_bot.egg-info/entry_points.txt
 qinglan_bot.egg-info/requires.txt
 qinglan_bot.egg-info/top_level.txt
@@ -38,10 +40,8 @@
 qinglan_bot/plugins/rcon_msg/rcon_msg_on.py
 qinglan_bot/plugins/send_group_name/__init__.py
 qinglan_bot/plugins/send_group_name/send_off.py
 qinglan_bot/plugins/send_group_name/send_on.py
 qinglan_bot/plugins/sub/__init__.py
 qinglan_bot/plugins/sub/add_sub.py
 qinglan_bot/plugins/sub/delete_sub.py
-qinglan_bot/plugins/sub/sub_list.py
-qinglan_bot/utils/__init__.py
-qinglan_bot/utils/config.py
+qinglan_bot/plugins/sub/sub_list.py
```

### Comparing `qinglan-bot-0.0.8/setup.py` & `qinglan-bot-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="qinglan-bot",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.8",  # 程序版本
+    version="0.1.0",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通机器人",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/qinglan_bot",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.9
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'nonebot2>=2.0.0rc3',
+        'mcqq-tool>=0.0.5',
+        'nonebot2>=2.0.0rc4',
         'nonebot-adapter-onebot>=2.1.5',
         'nonebot-plugin-guild-patch>=0.2.0',
         'nonebot-plugin-gocqhttp>=0.6.3',
         'websockets>=10.3',
-        'tortoise-orm>=0.19.2',
+        'tortoise-orm>=0.19.3',
         'aio-mc-rcon>=3.2.0',
         'click>=8.0.4',
     ],
     entry_points={'console_scripts': [
         'ql=qinglan_bot.cli_start:main',
     ]},
 )
```

