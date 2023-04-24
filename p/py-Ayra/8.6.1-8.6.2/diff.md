# Comparing `tmp/py-Ayra-8.6.1.tar.gz` & `tmp/py-Ayra-8.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-8.6.1.tar", last modified: Sun Apr 23 18:23:25 2023, max compression
+gzip compressed data, was "py-Ayra-8.6.2.tar", last modified: Mon Apr 24 18:24:25 2023, max compression
```

## Comparing `py-Ayra-8.6.1.tar` & `py-Ayra-8.6.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.135594 py-Ayra-8.6.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.131595 py-Ayra-8.6.1/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3034 2023-04-23 15:12:06.000000 py-Ayra-8.6.1/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.131595 py-Ayra-8.6.1/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-04-23 15:12:06.000000 py-Ayra-8.6.1/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.135594 py-Ayra-8.6.1/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1951 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-23 18:23:04.000000 py-Ayra-8.6.1/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-04-23 18:23:04.000000 py-Ayra-8.6.1/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.135594 py-Ayra-8.6.1/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19939 2023-04-23 01:47:25.000000 py-Ayra-8.6.1/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    26017 2023-04-22 18:23:10.000000 py-Ayra-8.6.1/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.135594 py-Ayra-8.6.1/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-04-20 13:10:06.000000 py-Ayra-8.6.1/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18429 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2284 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-23 18:23:04.000000 py-Ayra-8.6.1/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3387 2023-04-23 18:23:25.135594 py-Ayra-8.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 18:23:25.135594 py-Ayra-8.6.1/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3387 2023-04-23 18:23:25.000000 py-Ayra-8.6.1/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-04-23 18:23:25.000000 py-Ayra-8.6.1/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 18:23:25.000000 py-Ayra-8.6.1/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 18:23:25.000000 py-Ayra-8.6.1/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-23 18:23:25.000000 py-Ayra-8.6.1/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 18:23:25.139594 py-Ayra-8.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 16:51:17.000000 py-Ayra-8.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.954029 py-Ayra-8.6.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.950029 py-Ayra-8.6.2/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-04-23 15:12:06.000000 py-Ayra-8.6.2/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.950029 py-Ayra-8.6.2/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-04-23 15:12:06.000000 py-Ayra-8.6.2/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.950029 py-Ayra-8.6.2/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-23 18:23:04.000000 py-Ayra-8.6.2/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-24 18:24:04.000000 py-Ayra-8.6.2/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.954029 py-Ayra-8.6.2/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19939 2023-04-23 01:47:25.000000 py-Ayra-8.6.2/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28695 2023-04-24 18:24:04.000000 py-Ayra-8.6.2/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.954029 py-Ayra-8.6.2/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-04-20 13:10:06.000000 py-Ayra-8.6.2/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18429 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-24 18:24:04.000000 py-Ayra-8.6.2/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-04-24 18:24:25.954029 py-Ayra-8.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:24:25.954029 py-Ayra-8.6.2/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-04-24 18:24:25.000000 py-Ayra-8.6.2/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-24 18:24:25.000000 py-Ayra-8.6.2/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:24:25.000000 py-Ayra-8.6.2/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:24:25.000000 py-Ayra-8.6.2/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 18:24:25.000000 py-Ayra-8.6.2/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:24:25.954029 py-Ayra-8.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-04-19 16:51:17.000000 py-Ayra-8.6.2/setup.py
```

### Comparing `py-Ayra-8.6.1/Ayra/__init__.py` & `py-Ayra-8.6.2/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/__main__.py` & `py-Ayra-8.6.2/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/_misc/__init__.py` & `py-Ayra-8.6.2/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/_misc/_assistant.py` & `py-Ayra-8.6.2/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/_misc/_decorators.py` & `py-Ayra-8.6.2/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/_misc/_supporter.py` & `py-Ayra-8.6.2/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/_misc/_wrappers.py` & `py-Ayra-8.6.2/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/configs.py` & `py-Ayra-8.6.2/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/__init__.py` & `py-Ayra-8.6.2/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/afk_db.py` & `py-Ayra-8.6.2/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/antiflood_db.py` & `py-Ayra-8.6.2/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/asst_fns.py` & `py-Ayra-8.6.2/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/asstcmd_db.py` & `py-Ayra-8.6.2/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/autoban_db.py` & `py-Ayra-8.6.2/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/blacklist_db.py` & `py-Ayra-8.6.2/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/botchat_db.py` & `py-Ayra-8.6.2/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/broadcast_db.py` & `py-Ayra-8.6.2/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/ch_db.py` & `py-Ayra-8.6.2/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/dnd_db.py` & `py-Ayra-8.6.2/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/echo_db.py` & `py-Ayra-8.6.2/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/filestore_db.py` & `py-Ayra-8.6.2/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/filter_db.py` & `py-Ayra-8.6.2/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/forcesub_db.py` & `py-Ayra-8.6.2/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/gban_mute_db.py` & `py-Ayra-8.6.2/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-8.6.2/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/greetings_db.py` & `py-Ayra-8.6.2/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/logusers_db.py` & `py-Ayra-8.6.2/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/mute_db.py` & `py-Ayra-8.6.2/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/night_db.py` & `py-Ayra-8.6.2/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/notes_db.py` & `py-Ayra-8.6.2/Ayra/dB/notes_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def rem_note(user, word):
     ok = get_stuff()
     if ok.get(int(user)) and ok[int(user)].get(word):
         ok[int(user)].pop(word)
         return udB.set_key("NOTE", ok)
 
 
-def rem_all_note(chat):
+def rem_all_note(user):
     ok = get_stuff()
     if ok.get(int(user)):
         ok.pop(int(user))
         return udB.set_key("NOTE", ok)
 
 
 def get_notes(user, word):
@@ -39,8 +39,8 @@
     if ok.get(int(user)) and ok[int(user)].get(word):
         return ok[int(user)][word]
 
 
 def list_note(user):
     ok = get_stuff()
     if ok.get(int(user)):
-        return "".join(f"**๏ {z}**\n" for z in ok[user])
+        return "".join(f"**๏** `{z}`\n" for z in ok[user])
```

### Comparing `py-Ayra-8.6.1/Ayra/dB/nsfw_db.py` & `py-Ayra-8.6.2/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/pmpermit_db.py` & `py-Ayra-8.6.2/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/snips_db.py` & `py-Ayra-8.6.2/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/vc_sudos.py` & `py-Ayra-8.6.2/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/dB/warn_db.py` & `py-Ayra-8.6.2/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/FastTelethon.py` & `py-Ayra-8.6.2/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/__init__.py` & `py-Ayra-8.6.2/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/admins.py` & `py-Ayra-8.6.2/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/executor.py` & `py-Ayra-8.6.2/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/gDrive.py` & `py-Ayra-8.6.2/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/google_image.py` & `py-Ayra-8.6.2/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/helper.py` & `py-Ayra-8.6.2/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/info.py` & `py-Ayra-8.6.2/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/misc.py` & `py-Ayra-8.6.2/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/fns/tools.py` & `py-Ayra-8.6.2/Ayra/fns/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 # This file is a part of < https://github.com/senpai80/Ayra/ >
 # PLease read the GNU Affero General Public License in
 # <https://www.github.com/senpai80/Ayra/blob/main/LICENSE/>.
 
 import json
 import math
 import os
-import os.path
 import random
 import re
 import secrets
 import ssl
 import aiohttp
 from io import BytesIO
 from json.decoder import JSONDecodeError
 from traceback import format_exc
 
+import requests
+
 from .. import *
 from ..exceptions import DependencyMissingError
 from .helper import bash, run_async
 
 try:
     import certifi
 except ImportError:
@@ -52,14 +53,18 @@
     np = None
 
 try:
     from telegraph import Telegraph
 except ImportError:
     Telegraph = None
 
+try:
+    from bs4 import BeautifulSoup
+except ImportError:
+    BeautifulSoup = None
 
 async def async_searcher(
     url: str,
     post: bool = None,
     headers: dict = None,
     params: dict = None,
     json: dict = None,
@@ -539,32 +544,37 @@
         html_content=html,
     )
     return page["url"]
 
 
 async def Carbon(
     code,
-    base_url="https://rayso-api-desvhu-33.koyeb.app/generate",
+    base_url="https://carbonara.vercel.app/api/cook",
     file_name="ayra",
     download=False,
     rayso=False,
     **kwargs,
 ):
-    # if rayso:
-    kwargs["text"] = code
-    kwargs["theme"] = kwargs.get("theme", "meadow")
-    kwargs["darkMode"] = kwargs.get("darkMode", True)
-    kwargs["title"] = kwargs.get("title", "Ayra")
-    # else:
-    #    kwargs["code"] = code
+    if rayso:
+        base_url = "https://rayso-api-desvhu-33.koyeb.app/generate"
+        kwargs["text"] = code
+        kwargs["theme"] = kwargs.get("theme", "breeze")
+        kwargs["darkMode"] = kwargs.get("darkMode", True)
+        kwargs["title"] = kwargs.get("title", "Ayra")
+    else:
+        kwargs["code"] = code
     con = await async_searcher(base_url, post=True, json=kwargs, re_content=True)
     if not download:
         file = BytesIO(con)
         file.name = file_name + ".jpg"
     else:
+        try:
+            return json_parser(con.decode())
+        except Exception:
+            pass
         file = file_name + ".jpg"
         with open(file, "wb") as f:
             f.write(con)
     return file
 
 
 async def get_file_link(msg):
@@ -870,8 +880,73 @@
         return None, None
     _, chat, msg_id = matches[0]
     if chat.isdigit():
         chat = int("-100" + chat)
     return chat, int(msg_id)
 
 
+async def get_google_images(query):
+    soup = BeautifulSoup(
+        await async_searcher(
+            "https://google.com/search",
+            params={"q": query, "tbm": "isch"},
+            headers={"User-Agent": random.choice(some_random_headers)},
+        ),
+        "lxml",
+    )
+    google_images = []
+    all_script_tags = soup.select("script")
+    matched_images_data = "".join(
+        re.findall(r"AF_initDataCallback\(([^<]+)\);", str(all_script_tags))
+    )
+    matched_images_data_fix = json.dumps(matched_images_data)
+    matched_images_data_json = json.loads(matched_images_data_fix)
+    matched_google_image_data = re.findall(
+        r"\"b-GRID_STATE0\"(.*)sideChannel:\s?{}}", matched_images_data_json
+    )
+    matched_google_images_thumbnails = ", ".join(
+        re.findall(
+            r"\[\"(https\:\/\/encrypted-tbn0\.gstatic\.com\/images\?.*?)\",\d+,\d+\]",
+            str(matched_google_image_data),
+        )
+    ).split(", ")
+    thumbnails = [
+        bytes(bytes(thumbnail, "ascii").decode("unicode-escape"), "ascii").decode(
+            "unicode-escape"
+        )
+        for thumbnail in matched_google_images_thumbnails
+    ]
+    removed_matched_google_images_thumbnails = re.sub(
+        r"\[\"(https\:\/\/encrypted-tbn0\.gstatic\.com\/images\?.*?)\",\d+,\d+\]",
+        "",
+        str(matched_google_image_data),
+    )
+    matched_google_full_resolution_images = re.findall(
+        r"(?:'|,),\[\"(https:|http.*?)\",\d+,\d+\]",
+        removed_matched_google_images_thumbnails,
+    )
+    full_res_images = [
+        bytes(bytes(img, "ascii").decode("unicode-escape"), "ascii").decode(
+            "unicode-escape"
+        )
+        for img in matched_google_full_resolution_images
+    ]
+    for index, (metadata, thumbnail, original) in enumerate(
+        zip(soup.select(".isv-r.PNCib.MSM1fd.BUooTd"), thumbnails, full_res_images),
+        start=1,
+    ):
+        google_images.append(
+            {
+                "title": metadata.select_one(".VFACy.kGQAp.sMi44c.lNHeqe.WGvvNb")[
+                    "title"
+                ],
+                "link": metadata.select_one(".VFACy.kGQAp.sMi44c.lNHeqe.WGvvNb")[
+                    "href"
+                ],
+                "source": metadata.select_one(".fxgdke").text,
+                "thumbnail": thumbnail,
+                "original": original,
+            }
+        )
+    random.shuffle(google_images)
+    return google_images
 # --------- END --------- #
```

### Comparing `py-Ayra-8.6.1/Ayra/fns/ytdl.py` & `py-Ayra-8.6.2/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/kynan.py` & `py-Ayra-8.6.2/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/loader.py` & `py-Ayra-8.6.2/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/BaseClient.py` & `py-Ayra-8.6.2/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/__init__.py` & `py-Ayra-8.6.2/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/_database.py` & `py-Ayra-8.6.2/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/_extra.py` & `py-Ayra-8.6.2/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/connections.py` & `py-Ayra-8.6.2/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/funcs.py` & `py-Ayra-8.6.2/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/loader.py` & `py-Ayra-8.6.2/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/Ayra/startup/utils.py` & `py-Ayra-8.6.2/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/LICENSE` & `py-Ayra-8.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/PKG-INFO` & `py-Ayra-8.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.6.1
+Version: 8.6.2
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.6.1/README.md` & `py-Ayra-8.6.2/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/py_Ayra.egg-info/PKG-INFO` & `py-Ayra-8.6.2/py_Ayra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 8.6.1
+Version: 8.6.2
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-8.6.1/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-8.6.2/py_Ayra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayra-8.6.1/setup.py` & `py-Ayra-8.6.2/setup.py`

 * *Files identical despite different names*

