# Comparing `tmp/exceptnotifier-0.2.2.tar.gz` & `tmp/exceptnotifier-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.2.2.tar", last modified: Mon Apr 24 12:17:09 2023, max compression
+gzip compressed data, was "exceptnotifier-0.2.3.tar", last modified: Mon Apr 24 16:12:45 2023, max compression
```

## Comparing `exceptnotifier-0.2.2.tar` & `exceptnotifier-0.2.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.560119 exceptnotifier-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.408519 exceptnotifier-0.2.2/ExceptNotifier/
--rw-rw-rw-   0        0        0     4748 2023-04-24 12:16:22.000000 exceptnotifier-0.2.2/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.476055 exceptnotifier-0.2.2/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1382 2023-04-24 12:16:24.000000 exceptnotifier-0.2.2/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      532 2023-04-24 11:00:44.000000 exceptnotifier-0.2.2/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.2/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.2/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0     1009 2023-04-24 12:13:54.000000 exceptnotifier-0.2.2/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.2/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.2/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.2/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.2/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.2/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.2/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.2/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.2/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.2/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.2/ExceptNotifier/base/whatsapp_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.508670 exceptnotifier-0.2.2/ExceptNotifier/ipycore/
--rw-rw-rw-   0        0        0     1472 2023-04-24 12:16:28.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/__init__.py
--rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/beep_notifier_ipython.py
--rw-rw-rw-   0        0        0     2020 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/chime_notifier_ipython.py
--rw-rw-rw-   0        0        0     2422 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/desktop_notifier_ipython.py
--rw-rw-rw-   0        0        0     2030 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/discord_notifier_ipython.py
--rw-rw-rw-   0        0        0     2017 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/kakao_notifier_ipython.py
--rw-rw-rw-   0        0        0     2025 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/line_notifier_ipython.py
--rw-rw-rw-   0        0        0     2740 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/mail_notifier_ipython.py
--rw-rw-rw-   0        0        0     2021 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/slack_notifier_ipython.py
--rw-rw-rw-   0        0        0     2298 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/sms_notifier_ipython.py
--rw-rw-rw-   0        0        0     2025 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/teams_notifier_ipython.py
--rw-rw-rw-   0        0        0     2027 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/telegram_notifier_ipython.py
--rw-rw-rw-   0        0        0     2031 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/wechat_notifier_ipython.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.544580 exceptnotifier-0.2.2/ExceptNotifier/pycore/
--rw-rw-rw-   0        0        0     2009 2023-04-24 12:16:30.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/__init__.py
--rw-rw-rw-   0        0        0     1988 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/beep_notifier.py
--rw-rw-rw-   0        0        0     6782 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/chime_notifier.py
--rw-rw-rw-   0        0        0     6267 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/desktop_notifier.py
--rw-rw-rw-   0        0        0     7093 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/discord_notifier.py
--rw-rw-rw-   0        0        0     7168 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/kakao_notifier.py
--rw-rw-rw-   0        0        0     6711 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/line_notifier.py
--rw-rw-rw-   0        0        0     8862 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/mail_notifier.py
--rw-rw-rw-   0        0        0     6689 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/slack_notifier.py
--rw-rw-rw-   0        0        0     7926 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/sms_notifier.py
--rw-rw-rw-   0        0        0     6670 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/teams_notifier.py
--rw-rw-rw-   0        0        0     6897 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/telegram_notifier.py
--rw-rw-rw-   0        0        0     6686 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.553586 exceptnotifier-0.2.2/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      265 2023-04-24 12:16:33.000000 exceptnotifier-0.2.2/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.2/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.438800 exceptnotifier-0.2.2/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    34136 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    34136 2023-04-24 12:17:09.559121 exceptnotifier-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    33088 2023-04-24 10:05:15.000000 exceptnotifier-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 12:17:09.560119 exceptnotifier-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-04-24 12:15:45.000000 exceptnotifier-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:45.132893 exceptnotifier-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:44.986512 exceptnotifier-0.2.3/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4748 2023-04-24 16:12:12.000000 exceptnotifier-0.2.3/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:45.049242 exceptnotifier-0.2.3/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1382 2023-04-24 16:12:24.000000 exceptnotifier-0.2.3/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 exceptnotifier-0.2.3/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.3/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.3/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1005 2023-04-24 14:23:06.000000 exceptnotifier-0.2.3/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.3/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.3/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.3/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.3/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.3/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.3/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.3/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.3/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.3/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.3/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:45.084084 exceptnotifier-0.2.3/ExceptNotifier/ipycore/
+-rw-rw-rw-   0        0        0     1472 2023-04-24 16:12:15.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2104 2023-04-24 13:50:33.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2509 2023-04-24 15:05:53.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2114 2023-04-24 13:49:34.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2101 2023-04-24 13:43:54.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2109 2023-04-24 13:43:24.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     3092 2023-04-24 15:56:56.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2105 2023-04-24 13:42:15.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2390 2023-04-24 13:41:15.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2109 2023-04-24 13:40:55.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2111 2023-04-24 13:41:38.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2032 2023-04-24 13:41:53.000000 exceptnotifier-0.2.3/ExceptNotifier/ipycore/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:45.116828 exceptnotifier-0.2.3/ExceptNotifier/pycore/
+-rw-rw-rw-   0        0        0     2009 2023-04-24 16:12:18.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/__init__.py
+-rw-rw-rw-   0        0        0     2257 2023-04-24 13:57:14.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/beep_notifier.py
+-rw-rw-rw-   0        0        0     6879 2023-04-24 13:58:46.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/chime_notifier.py
+-rw-rw-rw-   0        0        0     6395 2023-04-24 14:24:50.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/desktop_notifier.py
+-rw-rw-rw-   0        0        0     7190 2023-04-24 14:12:17.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/discord_notifier.py
+-rw-rw-rw-   0        0        0     7260 2023-04-24 14:15:48.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/kakao_notifier.py
+-rw-rw-rw-   0        0        0     6804 2023-04-24 14:17:18.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/line_notifier.py
+-rw-rw-rw-   0        0        0     8862 2023-04-24 11:11:19.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/mail_notifier.py
+-rw-rw-rw-   0        0        0     6786 2023-04-24 14:17:53.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/slack_notifier.py
+-rw-rw-rw-   0        0        0     8002 2023-04-24 14:23:54.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/sms_notifier.py
+-rw-rw-rw-   0        0        0     6767 2023-04-24 15:06:20.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/teams_notifier.py
+-rw-rw-rw-   0        0        0     6994 2023-04-24 14:21:11.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/telegram_notifier.py
+-rw-rw-rw-   0        0        0     6784 2023-04-24 14:21:51.000000 exceptnotifier-0.2.3/ExceptNotifier/pycore/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:45.126304 exceptnotifier-0.2.3/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      265 2023-04-24 16:12:21.000000 exceptnotifier-0.2.3/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.3/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:12:45.012578 exceptnotifier-0.2.3/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    34802 2023-04-24 16:12:44.000000 exceptnotifier-0.2.3/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-04-24 16:12:44.000000 exceptnotifier-0.2.3/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:12:44.000000 exceptnotifier-0.2.3/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-24 16:12:44.000000 exceptnotifier-0.2.3/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 16:12:44.000000 exceptnotifier-0.2.3/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-24 16:12:44.000000 exceptnotifier-0.2.3/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    34802 2023-04-24 16:12:45.131891 exceptnotifier-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    33754 2023-04-24 16:03:08.000000 exceptnotifier-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 16:12:45.132893 exceptnotifier-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-04-24 16:12:08.000000 exceptnotifier-0.2.3/setup.py
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/__init__.py` & `exceptnotifier-0.2.3/ExceptNotifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,9 +123,9 @@
     "ExceptMailIpython",
     "ExceptSlackIpython",
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
 ]
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     "send_whatsapp_msg",
     "send_sms_msg",
     "beep",
     "receive_openai_advice",
     "get_resp_openai_advice",
 ]
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/beep_sender.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
+from os import system
 import platform
 
 
 def beep(sec=1, freq=1000) -> None:
     """Make beep sound
 
     :param sec: Beep duration, defaults to 1
@@ -16,8 +16,8 @@
     sys = platform.system()
 
     if sys == "Windows":
         import winsound
 
         winsound.Beep(int(1000 * sec), freq)
     else:
-        os.system("play -nq -t alsa synth {} sine {}".format(sec, freq))
+        system("play -nq -t alsa synth {} sine {}".format(sec, freq))
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/discord_sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,20 @@
     :param msg: Message text
     :type msg: str
     :return: Response according to REST API request
     :rtype: dict
     """
     try:
         from discord import Webhook, RequestsWebhookAdapter
-
         webhook = Webhook.from_url(
             _DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter()
         )
         resp = webhook.send(msg)
     except:
         from discord import SyncWebhook
-
         webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL)  # Initializing webhook
         resp = webhook.send(content=msg[:1900])
     return resp
 
 
 # if __name__ == "__main__":
 #     _DISCORD_WEBHOOK_URL = "xxxxx"
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/wechat_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.2.3/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/__init__.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
 ]
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/beep_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/beep_notifier_ipython.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/chime_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/discord_notifier_ipython.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.chime_sender import send_chime_msg
+from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptChimeIpython(
+def ExceptDiscordIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Chime message.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Discord.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -30,19 +31,19 @@
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
 
-    send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/desktop_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/telegram_notifier_ipython.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.desktop_sender import send_desktop_msg
+from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptDesktopIpython(
+def ExceptTelegramIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Desktop notification via plyer.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Telegram.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -28,25 +28,22 @@
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
-        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
-    data["head"] = "[Except Notifier] :warning: Error! Python Code Exception Detected."
-    data[
-        "body"
-    ] = f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
-    send_desktop_msg(data["head"], data["body"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_desktop_msg(os.environ["_CHIME_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+
+    send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/discord_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/mail_notifier_ipython.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,72 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+import smtplib
+import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptDiscordIpython(
+def ExceptMailIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Discord.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Gmail.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
     :param tb: TraceBack object of Ipython
     :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
+    SMTP_SERVER = "smtp.gmail.com"
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {
-        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    exceptNotifier = {
+        "TO": environ["_GAMIL_RECIPIENT_ADDR"],
+        "FROM": environ["_GMAIL_SENDER_ADDR"],
+        "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected.",
+        "BODY": f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}",
     }
-
-    send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    print(exceptNotifier["BODY"])
+    exceptNotifier["ALL"] = "From: %s\nTo: %s\nSubject: %s\n\n%s" % (
+        exceptNotifier["FROM"],
+        exceptNotifier["TO"],
+        exceptNotifier["SUBJECT"],
+        exceptNotifier["BODY"],
+    )
+    smtp = smtplib.SMTP_SSL(SMTP_SERVER, 465)
+    smtp.login(
+        environ["_GMAIL_SENDER_ADDR"], environ["_GMAIL_APP_PASSWORD_OF_SENDER"],
+    )
+    smtp.sendmail(exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message,
+            )  # NO-QA
+            exceptNotifier = {
+                "TO": environ["_GAMIL_RECIPIENT_ADDR"],
+                "FROM": environ["_GMAIL_SENDER_ADDR"],
+                "SUBJECT": "[Except AI Debugging] Error! chatGPT Debugging guide.",
+                "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}",
+            }
+            smtp.sendmail(
+                exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
+            )
+
+        except Exception as e:
+            print(e)
+            pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/kakao_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/kakao_notifier_ipython.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -31,19 +31,19 @@
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/line_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/line_notifier_ipython.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.line_sender import send_line_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -31,19 +31,19 @@
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/slack_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/slack_notifier_ipython.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
+from os import environ
 import datetime
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.slack_sender import send_slack_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
@@ -31,19 +31,19 @@
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
 
-    send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_slack_msg(environ["_SLACK_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/sms_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/wechat_notifier_ipython.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.sms_sender import send_sms_msg
+from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptSMSIpython(
+def ExceptWechatIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending SMS.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Wechat message.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -28,32 +28,22 @@
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
-        "text": f"[Except Notifier] ** Error ** Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}"
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_sms_msg(
-        os.environ["_TWILIO_SID"],
-        os.environ["_TWILIO_TOKEN"],
-        os.environ["_SENDER_PHONE_NUMBER"],
-        os.environ["_RECIPIENT_PHONE_NUMBER"],
-        data["text"],
-    )
+    send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
+
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
         advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_sms_msg(
-            os.environ["_TWILIO_SID"],
-            os.environ["_TWILIO_TOKEN"],
-            os.environ["_SENDER_PHONE_NUMBER"],
-            os.environ["_RECIPIENT_PHONE_NUMBER"],
-            advice_msg,
+            environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
         )
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
+
     except Exception as e:
         print(e)
         pass
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/teams_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/teams_notifier_ipython.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier.base.teams_sender import send_teams_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -31,20 +31,20 @@
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
+    send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
-    send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/telegram_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/chime_notifier_ipython.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.telegram_sender import send_telegram_msg
+from ExceptNotifier.base.chime_sender import send_chime_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
-
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptTelegramIpython(
+def ExceptChimeIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Telegram.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Chime message.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -28,22 +27,22 @@
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
-        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
 
-    send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/ipycore/wechat_notifier_ipython.py` & `exceptnotifier-0.2.3/ExceptNotifier/ipycore/desktop_notifier_ipython.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import datetime
+from os import environ
 from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier.base.wechat_sender import send_wechat_msg
+from ExceptNotifier.base.desktop_sender import send_desktop_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptWechatIpython(
+def ExceptDesktopIpython(
     shell: object, etype: object, evalue: object, tb: object, tb_offset=1
 ) -> None:
-    """ExceptNotifier function for overriding custom execute in ipython for sending Wechat message.
+    """ExceptNotifier function for overriding custom execute in ipython for sending Desktop notification via plyer.
 
     :param shell: Excecuted shell, ZMQInteractiveShell object.
     :type shell: object
     :param etype: Error type
     :type etype: object
     :param evalue: Error value
     :type evalue: object
@@ -28,22 +28,25 @@
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
-        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
     }
-
-    send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
-
-    try:
-        error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(
-            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-        )
-        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], advice_msg)
-
-    except Exception as e:
-        print(e)
-        pass
+    data["head"] = "[Except Notifier] :warning: Error! Python Code Exception Detected."
+    data[
+        "body"
+    ] = f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    send_desktop_msg(data["head"], data["body"])
+    if environ.get('_OPEN_AI_API') is not None:
+        try:
+            error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
+            advice_msg = receive_openai_advice(
+                environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+            )
+            send_desktop_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+
+        except Exception as e:
+            print(e)
+            pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/__init__.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,9 +64,9 @@
     "ExceptWechat",
     "SendWechat",
     "SuccessDesktop",
     "ExceptDesktop",
     "SendDesktop",
 ]
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/beep_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/beep_notifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import platform
+from os import environ
+from os import system
 from ExceptNotifier import beep
 
 
 class ExceptBeep(BaseException):
     """Override excepthook to send error message to beep.
 
     :param etype: Error Type
@@ -16,20 +17,22 @@
     :type tb: _type_
     """
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-
-        beep(os.environ["BEEP_TIME"])
-        beep(os.environ["BEEP_TIME"])
-        beep(os.environ["BEEP_TIME"])
-        beep(os.environ["BEEP_TIME"])
-        beep(os.environ["BEEP_TIME"])
+        if environ.get('BEEP_TIME') is not None:
+            beep(environ["BEEP_TIME"])
+            beep(environ["BEEP_TIME"])
+            beep(environ["BEEP_TIME"])
+        else:
+            beep()
+            beep()
+            beep()
 
     @staticmethod
     def beep(sec=1, freq=1000) -> None:
         """Make beep sound
 
         :param sec: beep duration, defaults to 1
         :type sec: int, optional
@@ -40,42 +43,48 @@
         sys = platform.system()
 
         if sys == "Windows":
             import winsound
 
             winsound.Beep(int(1000 * sec), freq)
         else:
-            os.system("play -nq -t alsa synth {} sine {}".format(sec, freq))
+            system("play -nq -t alsa synth {} sine {}".format(sec, freq))
 
 
 class SuccessBeep:
     """Success beep
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
-        beep(os.environ["BEEP_TIME"])
-        beep(os.environ["BEEP_TIME"])
-
+        if environ.get('BEEP_TIME') is not None:
+            beep(environ["BEEP_TIME"])
+            beep(environ["BEEP_TIME"])
+        else:
+            beep()
+            beep()
 
 class SendBeep:
     """Send beep
     """
 
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
-        beep(os.environ["BEEP_TIME"])
+        if environ.get('BEEP_TIME') is not None:
+            beep(environ["BEEP_TIME"])
+        else:
+            beep()
 
 
 # if __name__ == "__main__":
-#     os.environ['BEEP_TIME'] = 1
+#     environ['BEEP_TIME'] = 1
 #     sys.excepthook = ExceptBeep.__call__
 #     try:
 #         print(1 / 20)
 #         SuccessBeep().__call__()  # 1 success beep-beep
 #     except ExceptBeep as e:  # 2 except beep-beep
 #         sys.exit()
 #     SendBeep().__call__()  # 3 customized beep-beep
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/chime_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/chime_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import json
 import urllib3
 import datetime
 import traceback
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.chime_sender import send_chime_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -68,31 +68,31 @@
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], advice_msg)
-        except Exception as e:
-            print(e)
-            pass
+        send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_chime_msg(environ["_CHIME_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_chime_msg(_CHIME_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through chime app's webhook url.
 
         :param _CHIME_WEBHOOK_URL: Webhook url from chime app
         :type _CHIME_WEBHOOK_URL: str
@@ -126,15 +126,15 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
+        send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 class SendChime:
     """Sending message to AWS Chime
     """
 
     def __init__(self) -> None:
@@ -149,24 +149,24 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
+        send_chime_msg(environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
 
 #     """Get your Webhook _CHIME_WEBHOOK_URL from your chatroom.
 #     https://docs.aws.amazon.com/chime/latest/ag/webhooks.html"""
-# os.environ['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx"
-# os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+# environ['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx"
+# environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 # sys.excepthook = ExceptChime.__call__
 # try:
 #     print(1 / 0)
 #     SuccessChime().__call__()  # 1 success sender
 # except ExceptChime as e:  # 2 except sender
 #     sys.exit()
 # SendChime().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/desktop_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/desktop_notifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import datetime
 import traceback
+from os import environ
 from plyer import notification
 from email.message import EmailMessage
 from ExceptNotifier.base.desktop_sender import send_desktop_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -70,31 +70,32 @@
 
         print(exceptNotifier["BODY"])
 
         send_desktop_msg(
             title=exceptNotifier["SUBJECT"], message=exceptNotifier["BODY"]
         )
 
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_desktop_msg(
-                title="chatGPT: How to Debug your code.", message=advice_msg
-            )
-        except Exception as e:
-            print(e)
-            pass
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_desktop_msg(
+                    title="chatGPT: How to Debug your code.", message=advice_msg
+                )
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_desktop_msg(title_msg: str, body_msg: str, DISP_TIME=5) -> None:
         """Sending notification to desktop
 
         :param title_msg: Title of message
         :type title_msg: str
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/discord_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/discord_notifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import datetime
 import traceback
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -67,31 +67,31 @@
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], advice_msg)
-        except Exception as e:
-            print(e)
-            pass
+        send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_discord_msg(_DISCORD_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through discord app's webhook url.
 
         :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
         :type _DISCORD_WEBHOOK_URL: str
@@ -130,15 +130,15 @@
             "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
+        send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
 
 
 class SendDiscord:
     """Sending message to Discord
     """
 
     def __init__(self) -> None:
@@ -153,23 +153,23 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
+        send_discord_msg(environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
 
 
 # if __name__ == "__main__":
 #     """Get your _DISCORD_WEBHOOK_URL from HERE.
 # #     https://discord.com/developers/docs/resources/webhook"""
-#     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-#     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
-#     os.environ['_DISCORD_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxx"
+#     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     environ['_DISCORD_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxx"
 #     sys.excepthook = ExceptDiscord.__call__
 #     try:
 #         print(1 / 20)
 #         SuccessDiscord().__call__()  # 1 success sender
 #     except ExceptDiscord as e:  # 2 except sender
 #         sys.exit()
 #     SendDiscord().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/kakao_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/kakao_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import json
 import datetime
 import requests
 import traceback
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
@@ -68,44 +68,43 @@
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], advice_msg)
-        except Exception as e:
-            print(e)
-            pass
+        send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], advice_msg)
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_kakao_msg(_KAKAO_TOKEN_PATH: str, msg: str) -> dict:
         """Send message to chat room through kakaotalk app's REST API.
 
         :param _KAKAO_TOKEN_PATH: Kakaotalk token path
         :type _KAKAO_TOKEN_PATH: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
-
         with open(_KAKAO_TOKEN_PATH, "r") as kakao:
             tokens = json.load(kakao)
 
         url = "https://kapi.kakao.com/v2/api/talk/memo/default/send"
         headers = {"Authorization": "Bearer " + tokens["access_token"]}
         data = {
             "object_type": "text",
@@ -138,15 +137,15 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
+        send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
 
 
 class SendKakao:
     """Sending message to Kakaotalk
     """
 
     def __init__(self) -> None:
@@ -161,26 +160,26 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        with open(os.environ["_KAKAO_TOKEN_PATH"], "r") as kakao:
+        with open(environ["_KAKAO_TOKEN_PATH"], "r") as kakao:
             tokens = json.load(kakao)
 
-        send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
+        send_kakao_msg(environ["_KAKAO_TOKEN_PATH"], data["text"])
 
 
 # if __name__ == "__main__":
-#     os.environ['_KAKAO_TOKEN_PATH'] = (
+#     environ['_KAKAO_TOKEN_PATH'] = (
 #         r"C:\Users\parkm\Desktop\git\ExceptionNotifier\tutorials\token.json"
 #     )
-#     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-#     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     sys.excepthook = ExceptKakao.__call__
 #     try:
 #         print(1 / 0)
 #         SuccessKakao().__call__()  # 1 success sender
 #     except ExceptKakao as e:  # 2 except sender
 #         sys.exit()
 #     SendKakao().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/line_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/line_notifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import datetime
 import requests
 import traceback
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.line_sender import send_line_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -68,30 +68,30 @@
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
-        except Exception as e:
-            pass
+        send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
+            except Exception as e:
+                pass
 
     @staticmethod
     def send_line_msg(_LINE_NOTIFY_API_TOKEN: str, msg: str) -> dict:
         """Send message to chat room through Line app's REST API.
 
         :param _LINE_NOTIFY_API_TOKEN: Line notify API token
         :type _LINE_NOTIFY_API_TOKEN: str
@@ -124,15 +124,15 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
+        send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 class SendLine:
     """Sending success message to Line
     """
 
     def __init__(self) -> None:
@@ -147,23 +147,23 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
+        send_line_msg(environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 # if __name__ == "__main__":
 #     """Get your URL from HERE.
 #     https://notify-bot.line.me/my/"""
-# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
-#     os.environ['_LINE_NOTIFY_API_TOKEN'] = "xxxxxxxxxxx"
+# #     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     environ['_LINE_NOTIFY_API_TOKEN'] = "xxxxxxxxxxx"
 #     sys.excepthook = ExceptLine.__call__
 #     try:
 #         print(1 / 20)
 #         SuccessLine().__call__()  # 1 success sender
 #     except ExceptLine as e:  # 2 except sender
 #         sys.exit()
 #     SendLine().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/mail_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/slack_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/slack_notifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import datetime
 import requests
 import traceback
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier import send_slack_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -67,31 +67,31 @@
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], advice_msg)
-        except Exception as e:
-            print(e)
-            pass
+        send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_slack_msg(environ["_SLACK_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_slack_msg(_SLACK_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through slack app's api.
 
         :param _SLACK_WEBHOOK_URL: _SLACK_WEBHOOK_URL from slack app
         :type _SLACK_WEBHOOK_URL: str
@@ -121,15 +121,15 @@
             "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
+        send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
 
 
 class SendSlack:
     """Sending message to Slack
     """
 
     def __init__(self) -> None:
@@ -143,24 +143,24 @@
             "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
+        send_slack_msg(environ["_SLACK_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
 #     # Get your slack bot and enter _SLACK_WEBHOOK_URL
 #     """Get your _SLACK_WEBHOOK_URL from HERE.
-# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+# #     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     https://api.slack.com/messaging/webhooks#create_a_webhook"""
-#     os.environ['_SLACK_WEBHOOK_URL'] ='xxxxxxx'
+#     environ['_SLACK_WEBHOOK_URL'] ='xxxxxxx'
 #     sys.excepthook = ExceptSlack.__call__
 #     try:
 #         print(1 / 0)
 #         SuccessSlack().__call__()  # 1 success sender
 #     except ExceptSlack as e:  # 2 except sender
 #         sys.exit()
 #     SendSlack().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/sms_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/sms_notifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 import re
-import os
 import datetime
 import traceback
+from os import environ
 from twilio.rest import Client
 from email.message import EmailMessage
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
@@ -69,42 +69,42 @@
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_sms_msg(
-            os.environ["_TWILIO_SID"],
-            os.environ["_TWILIO_TOKEN"],
-            os.environ["_SENDER_PHONE_NUMBER"],
-            os.environ["_RECIPIENT_PHONE_NUMBER"],
+            environ["_TWILIO_SID"],
+            environ["_TWILIO_TOKEN"],
+            environ["_SENDER_PHONE_NUMBER"],
+            environ["_RECIPIENT_PHONE_NUMBER"],
             data["text"],
         )
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_sms_msg(
-                os.environ["_TWILIO_SID"],
-                os.environ["_TWILIO_TOKEN"],
-                os.environ["_SENDER_PHONE_NUMBER"],
-                os.environ["_RECIPIENT_PHONE_NUMBER"],
-                advice_msg,
-            )
-        except Exception as e:
-            print(e)
-            pass
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_sms_msg(
+                    environ["_TWILIO_SID"],
+                    environ["_TWILIO_TOKEN"],
+                    environ["_SENDER_PHONE_NUMBER"],
+                    environ["_RECIPIENT_PHONE_NUMBER"],
+                    advice_msg,
+                )
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_sms_msg(
         _TWILIO_SID: str,
         _TWILIO_TOKEN: str,
         _SENDER_PHONE_NUMBER: str,
         _RECIPIENT_PHONE_NUMBER: str,
@@ -151,18 +151,18 @@
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_sms_msg(
-            os.environ["_TWILIO_SID"],
-            os.environ["_TWILIO_TOKEN"],
-            os.environ["_SENDER_PHONE_NUMBER"],
-            os.environ["_RECIPIENT_PHONE_NUMBER"],
+            environ["_TWILIO_SID"],
+            environ["_TWILIO_TOKEN"],
+            environ["_SENDER_PHONE_NUMBER"],
+            environ["_RECIPIENT_PHONE_NUMBER"],
             data["text"],
         )
 
 
 class SendSMS:
     """Sending message to SMS
     """
@@ -180,31 +180,31 @@
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_sms_msg(
-            os.environ["_TWILIO_SID"],
-            os.environ["_TWILIO_TOKEN"],
-            os.environ["_SENDER_PHONE_NUMBER"],
-            os.environ["_RECIPIENT_PHONE_NUMBER"],
+            environ["_TWILIO_SID"],
+            environ["_TWILIO_TOKEN"],
+            environ["_SENDER_PHONE_NUMBER"],
+            environ["_RECIPIENT_PHONE_NUMBER"],
             data["text"],
         )
 
 
 # if __name__ == "__main__":
 #     """https://www.twilio.com/en-us"""
-#     os.environ['_TWILIO_SID'] = "xxxx"
-#     os.environ['_TWILIO_TOKEN'] = "yyyyyy"
-#     os.environ['_RECIPIENT_PHONE_NUMBER'] = ("+aaaaaa",)
-#     os.environ['_SENDER_PHONE_NUMBER'] = ("+bbbbbb",)
+#     environ['_TWILIO_SID'] = "xxxx"
+#     environ['_TWILIO_TOKEN'] = "yyyyyy"
+#     environ['_RECIPIENT_PHONE_NUMBER'] = ("+aaaaaa",)
+#     environ['_SENDER_PHONE_NUMBER'] = ("+bbbbbb",)
 #     sys.excepthook = ExceptSMS.__call__
-# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+# #     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     try:
 #         print(1 / 10)
 #         SuccessSMS().__call__()  # 1 success sender
 #     except ExceptSMS as e:  # 2 except sender
 #         with open("exceptError.pickle", "wb") as f:
 #             pickle.dump(e, f)
 #         raise pickle.load(f)
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/teams_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/teams_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import os
 import re
 import json
 import datetime
 import requests
 import traceback
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.teams_sender import send_teams_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
@@ -67,31 +67,31 @@
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
-        except Exception as e:
-            print(e)
-            pass
+        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
         """Send message to chat room through microsoft teams app's webhook url.
 
         :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
         :type _TEAMS_WEBHOOK_URL: str
@@ -126,15 +126,15 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
 
 class SendTeams:
     """Sending message to microsoft teams
     """
 
     def __init__(self) -> None:
@@ -149,22 +149,22 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        send_teams_msg(environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
 #     """Follow next page"""
-#     os.environ['_TEAMS_WEBHOOK_URL'] = "microsoft webhook _TEAMS_WEBHOOK_URL"
-# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     environ['_TEAMS_WEBHOOK_URL'] = "microsoft webhook _TEAMS_WEBHOOK_URL"
+# #     environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     sys.excepthook = ExceptTeams.__call__
 #     try:
 #         print(1 / 20)
 #         SuccessTeams().__call__()  # 1 success sender
 #     except ExceptTeams as e:  # 2 except sender
 #         sys.exit()
 #     SendTeams().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/telegram_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/telegram_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import requests
 import traceback
 import datetime
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
@@ -64,32 +64,32 @@
             for key, val in frame.f_locals.items():
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], advice_msg)
-
-        except Exception as e:
-            print(e)
-            pass
+        send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_telegram_msg(environ["_TELEGRAM_TOKEN"], advice_msg)
+
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_telegram_msg(_TELEGRAM_TOKEN: str, msg: str) -> dict:
         """Send message via telegram bot.
 
         :param _TELEGRAM_TOKEN: Telegram secure bot Token
         :type _TELEGRAM_TOKEN: str
@@ -125,15 +125,15 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
+        send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 class SendTelegram:
     """Sending message to telegram
     """
 
     def __init__(self) -> None:
@@ -148,23 +148,23 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
+        send_telegram_msg(environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 # if __name__ == "__main__":
 #     """Get your bot from botfather.
 #     https://core.telegram.org/bots/tutorial"""
-#     os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
-#     # os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-#     # os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
+#     # environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     # environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     sys.excepthook = ExceptTelegram.__call__
 #     try:
 #         print(1 / 0)
 #         SuccessTelegram().__call__()  # 1 success sender
 #     except ExceptTelegram as e:  # 2 except sender
 #         sys.exit()
 #     SendTelegram().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/pycore/wechat_notifier.py` & `exceptnotifier-0.2.3/ExceptNotifier/pycore/wechat_notifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import os
 import requests
 import traceback
 import datetime
+from os import environ
 from email.message import EmailMessage
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
@@ -64,31 +64,31 @@
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_wechat_msg(os.enviro["_WECHAT_WEBHOOK_URL"], data["text"])
-
-        try:
-            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
-                line[0],
-                line[2],
-                line[1],
-                line[3],
-            )
-            advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
-            )  # NO-QA
-            send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], advice_msg)
-        except Exception as e:
-            print(e)
-            pass
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
+        if environ.get('_OPEN_AI_API') is not None:
+            try:
+                error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+                advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                    line[0],
+                    line[2],
+                    line[1],
+                    line[3],
+                )
+                advice_msg += receive_openai_advice(
+                    environ["_OPEN_AI_MODEL"], environ["_OPEN_AI_API"], error_message
+                )  # NO-QA
+                send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], advice_msg)
+            except Exception as e:
+                print(e)
+                pass
 
     @staticmethod
     def send_wechat_msg(_WECHAT_WEBHOOK_URL: str, msg: str) -> None:
         """Send message to wechat.
 
         :param _WECHAT_WEBHOOK_URL: Wechat Webhook URL https://work.weixin.qq.com/api/doc/90000/90136/91770
         :type _WECHAT_WEBHOOK_URL: str
@@ -116,15 +116,15 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
 
 class SendWechat:
     """Sending message to wechat
     """
 
     def __init__(self) -> None:
@@ -139,23 +139,23 @@
         }
         exceptNotifier[
             "BODY"
         ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
+        send_wechat_msg(environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
 #     """Get your wechat webhook URL.
 #     https://work.weixin.qq.com/api/doc/90000/90136/91770"""
-#     os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
-#     # os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
-#     # os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
+#     # environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     # environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     sys.excepthook = ExceptWechat.__call__
 #     try:
 #         print(1 / 0)
 #         SuccessWechat().__call__()  # 1 success sender
 #     except ExceptWechat as e:  # 2 except sender
 #         sys.exit()
 #     SendWechat().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.2.3/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.2.3/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.2
+Version: 0.2.3
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -138,17 +138,17 @@
 |:--:|:--|:--:|:--:|:--:|:---:|
 |Beep|N/A|Free|N/A|0min|[ExceptBeep](./tutorials/ExceptBeep/GUIDE.md)|
 |Desktop|N/A|Free|N/A|0min|[ExceptDesktop](./tutorials/ExceptDesktop/GUIDE.md)|
 |Telegram|`_TELEGRAM_TOKEN`|Freemium|Easy|2min|[ExceptTelegram](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) |
 |Discord|`_DISCORD_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptDiscord](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) |
 |AWS Chime|`_CHIME_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptChime](./tutorials/ExceptChime/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) |
-|G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md)|
+|G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) |
-|SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md)|
+|SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/ExceptTeams/GUIDE.md)|
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
@@ -193,15 +193,15 @@
     print(1/0)
 except ExceptTelegram:    # sending except message to telegram
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
-![](./assets/imgs/ex02.png)
+![](./assets/imgs/ex02_1.png)
 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
@@ -311,15 +311,15 @@
   print(1/0)
 except:
   raise
 ```
 
 *Example code With Open AI API*
 
-![](./assets/imgs/ex07.png)
+![](./assets/imgs/ex07_1.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
 os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"    
@@ -445,14 +445,16 @@
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
 ## *Mail*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)
+
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en). 
 
 *API TEST*
 ```python
 from ExceptNotifier import send_gmail_msg
@@ -685,14 +687,16 @@
 
 SendLine().__call__()        #3 customized sender          
 ```
 
 <Br>
 
 ## *SMS*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)
+
 - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://www.twilio.com/en-us)
 - b. Click Console in the upper right corner.
 - c. Copy the variables provided in the console.
 
 
 *API TEST*
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.2 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.3 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -99,29 +99,34 @@
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/
 ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/1-
 dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) | |G-Mail|`_GAMIL_RECIPIENT_ADDR`,
 `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted
-free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md)|
+free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/
 ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) | |SMS|`_TWILIO_SID`,
 `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not
-free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md)| |Microsoft
-Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/
-ExceptTeams/GUIDE.md)| |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min
-(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you
-add the following two variables to the required variables for each application
-in the table above, you can receive error location and explanation, as well as
-examples, from OpenAI's model | API | Required Variables | Free or Paid | Ease
-of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:-
--:|:---:| | OpenAI API |`Required variables for each application`+
+free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
+|Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./
+tutorials/ExceptTeams/GUIDE.md)|
+|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|
+[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you add the following two
+variables to the required variables for each application in the table above,
+you can receive error location and explanation, as well as examples, from
+OpenAI's model | API | Required Variables | Free or Paid | Ease of Setup | Time
+Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |
+OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
 APIOpenAI/GUIDE.md)|
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
@@ -139,17 +144,17 @@
 
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex02.png) You can receive debugging information
-from ChatGPT via OpenAI's API when using the Except statement. The syntax
-remains the same, but you'll need to configure these two variables:
+Notification ![](./assets/imgs/ex02_1.png) You can receive debugging
+information from ChatGPT via OpenAI's API when using the Except statement. The
+syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
 ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
 Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
 Type: Class
@@ -191,15 +196,15 @@
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier. - Format: Except[appName] -
 Type: function
 *Example code without Open AI API* ![](./assets/imgs/ex06.png) ```python from
 ExceptNotifier import ExceptTelegramIpython import os os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) try: print(1/0) except: raise ``` *Example code With
-Open AI API* ![](./assets/imgs/ex07.png) ```python from ExceptNotifier import
+Open AI API* ![](./assets/imgs/ex07_1.png) ```python from ExceptNotifier import
 ExceptTelegramIpython import os get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"
 os.environ['_OPEN_AI_API'] = "sk-xxxxx" os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 try: print(1/0) except: raise ``` ## Success`Notifier` in Ipython ![](./assets/
 imgs/ex08.png) - Same syntax in Python. See Python Core above. ```python import
 sys import os from ExceptNotifier import SuccessTelegram os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" try: print(1/20) # Your Code Here SuccessTelegram
@@ -244,16 +249,19 @@
 update it so that other models can be used later. *Notifier* ```python from
 ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import sys,
 os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
 "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion
 ['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
 success sender except ExceptTelegram as e: #2. except sender sys.exit()
 SendTelegram().__call__() #3. customized sender ```
-## *Mail* In the except statement, an email is sent along with the error
-message. Additionally, you can send emails from any desired line.
+## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
+email is sent along with the error message. Additionally, you can send emails
+from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
 (https://myaccount.google.com/u/3/apppasswords?utm_source=google-
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
 *API TEST* ```python from ExceptNotifier import send_gmail_msg
@@ -341,29 +349,31 @@
 ```python import sys from ExceptNotifier import ExceptLine, SuccessLine,
 SendLine sys.excepthook = ExceptLine.__call__ # Define the next two variables
 optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
 ['_LINE_NOTIFY_API_TOKEN'] = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
 ().__call__() #1 success sender except ExceptLine as e: #2 except sender
 sys.exit() SendLine().__call__() #3 customized sender ```
-## *SMS* - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://
-www.twilio.com/en-us) - b. Click Console in the upper right corner. - c. Copy
-the variables provided in the console. *API TEST* ```python from ExceptNotifier
-import send_sms_msg _TWILIO_SID = 'xxxx' _TWILIO_TOKEN = "xxxx"
-_SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER = "xxxx" send_sms_msg
-( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER,
-"Any Test Message") ``` *Notifier* ```python import sys from ExceptNotifier
-import ExceptSMS, SuccessSMS, SendSMS sys.excepthook = ExceptSMS.__call__ #
-Define the next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_TWILIO_SID'] = 'xxxx' os.environ['_TWILIO_TOKEN'] = 'yyyyyy'
-os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa", os.environ
-['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS().__call__() #1
-success sender except ExceptSMS as e: #2 except sender sys.exit() SendSMS
-().__call__() #3 customized sender ```
+## *SMS* [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing) - a. Sign up for Twilio. [https:
+//www.twilio.com/en-us](https://www.twilio.com/en-us) - b. Click Console in the
+upper right corner. - c. Copy the variables provided in the console. *API TEST*
+```python from ExceptNotifier import send_sms_msg _TWILIO_SID = 'xxxx'
+_TWILIO_TOKEN = "xxxx" _SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER =
+"xxxx" send_sms_msg( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER,
+_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` *Notifier* ```python import
+sys from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
+ExceptSMS.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TWILIO_SID'] = 'xxxx' os.environ
+['_TWILIO_TOKEN'] = 'yyyyyy' os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa",
+os.environ['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS
+().__call__() #1 success sender except ExceptSMS as e: #2 except sender
+sys.exit() SendSMS().__call__() #3 customized sender ```
 ## *Teams* - a. Create the channel that you want to notify. - b. `App` -
 `Search: webhook` - `Incoming Webhook` [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
```

### Comparing `exceptnotifier-0.2.2/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.2.3/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/LICENSE` & `exceptnotifier-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.2/PKG-INFO` & `exceptnotifier-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.2
+Version: 0.2.3
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -138,17 +138,17 @@
 |:--:|:--|:--:|:--:|:--:|:---:|
 |Beep|N/A|Free|N/A|0min|[ExceptBeep](./tutorials/ExceptBeep/GUIDE.md)|
 |Desktop|N/A|Free|N/A|0min|[ExceptDesktop](./tutorials/ExceptDesktop/GUIDE.md)|
 |Telegram|`_TELEGRAM_TOKEN`|Freemium|Easy|2min|[ExceptTelegram](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) |
 |Discord|`_DISCORD_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptDiscord](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) |
 |AWS Chime|`_CHIME_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptChime](./tutorials/ExceptChime/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) |
-|G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md)|
+|G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) |
-|SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md)|
+|SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/ExceptTeams/GUIDE.md)|
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
@@ -193,15 +193,15 @@
     print(1/0)
 except ExceptTelegram:    # sending except message to telegram
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
-![](./assets/imgs/ex02.png)
+![](./assets/imgs/ex02_1.png)
 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
@@ -311,15 +311,15 @@
   print(1/0)
 except:
   raise
 ```
 
 *Example code With Open AI API*
 
-![](./assets/imgs/ex07.png)
+![](./assets/imgs/ex07_1.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
 os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"    
@@ -445,14 +445,16 @@
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
 ## *Mail*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)
+
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en). 
 
 *API TEST*
 ```python
 from ExceptNotifier import send_gmail_msg
@@ -685,14 +687,16 @@
 
 SendLine().__call__()        #3 customized sender          
 ```
 
 <Br>
 
 ## *SMS*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)
+
 - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://www.twilio.com/en-us)
 - b. Click Console in the upper right corner.
 - c. Copy the variables provided in the console.
 
 
 *API TEST*
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.2 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.3 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -99,29 +99,34 @@
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/
 ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/1-
 dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) | |G-Mail|`_GAMIL_RECIPIENT_ADDR`,
 `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted
-free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md)|
+free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/
 ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) | |SMS|`_TWILIO_SID`,
 `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not
-free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md)| |Microsoft
-Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/
-ExceptTeams/GUIDE.md)| |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min
-(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you
-add the following two variables to the required variables for each application
-in the table above, you can receive error location and explanation, as well as
-examples, from OpenAI's model | API | Required Variables | Free or Paid | Ease
-of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:-
--:|:---:| | OpenAI API |`Required variables for each application`+
+free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
+|Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./
+tutorials/ExceptTeams/GUIDE.md)|
+|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|
+[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you add the following two
+variables to the required variables for each application in the table above,
+you can receive error location and explanation, as well as examples, from
+OpenAI's model | API | Required Variables | Free or Paid | Ease of Setup | Time
+Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |
+OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
 APIOpenAI/GUIDE.md)|
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
@@ -139,17 +144,17 @@
 
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex02.png) You can receive debugging information
-from ChatGPT via OpenAI's API when using the Except statement. The syntax
-remains the same, but you'll need to configure these two variables:
+Notification ![](./assets/imgs/ex02_1.png) You can receive debugging
+information from ChatGPT via OpenAI's API when using the Except statement. The
+syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
 ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
 Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
 Type: Class
@@ -191,15 +196,15 @@
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier. - Format: Except[appName] -
 Type: function
 *Example code without Open AI API* ![](./assets/imgs/ex06.png) ```python from
 ExceptNotifier import ExceptTelegramIpython import os os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) try: print(1/0) except: raise ``` *Example code With
-Open AI API* ![](./assets/imgs/ex07.png) ```python from ExceptNotifier import
+Open AI API* ![](./assets/imgs/ex07_1.png) ```python from ExceptNotifier import
 ExceptTelegramIpython import os get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"
 os.environ['_OPEN_AI_API'] = "sk-xxxxx" os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 try: print(1/0) except: raise ``` ## Success`Notifier` in Ipython ![](./assets/
 imgs/ex08.png) - Same syntax in Python. See Python Core above. ```python import
 sys import os from ExceptNotifier import SuccessTelegram os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" try: print(1/20) # Your Code Here SuccessTelegram
@@ -244,16 +249,19 @@
 update it so that other models can be used later. *Notifier* ```python from
 ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import sys,
 os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
 "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion
 ['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
 success sender except ExceptTelegram as e: #2. except sender sys.exit()
 SendTelegram().__call__() #3. customized sender ```
-## *Mail* In the except statement, an email is sent along with the error
-message. Additionally, you can send emails from any desired line.
+## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
+email is sent along with the error message. Additionally, you can send emails
+from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
 (https://myaccount.google.com/u/3/apppasswords?utm_source=google-
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
 *API TEST* ```python from ExceptNotifier import send_gmail_msg
@@ -341,29 +349,31 @@
 ```python import sys from ExceptNotifier import ExceptLine, SuccessLine,
 SendLine sys.excepthook = ExceptLine.__call__ # Define the next two variables
 optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
 ['_LINE_NOTIFY_API_TOKEN'] = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
 ().__call__() #1 success sender except ExceptLine as e: #2 except sender
 sys.exit() SendLine().__call__() #3 customized sender ```
-## *SMS* - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://
-www.twilio.com/en-us) - b. Click Console in the upper right corner. - c. Copy
-the variables provided in the console. *API TEST* ```python from ExceptNotifier
-import send_sms_msg _TWILIO_SID = 'xxxx' _TWILIO_TOKEN = "xxxx"
-_SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER = "xxxx" send_sms_msg
-( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER,
-"Any Test Message") ``` *Notifier* ```python import sys from ExceptNotifier
-import ExceptSMS, SuccessSMS, SendSMS sys.excepthook = ExceptSMS.__call__ #
-Define the next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_TWILIO_SID'] = 'xxxx' os.environ['_TWILIO_TOKEN'] = 'yyyyyy'
-os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa", os.environ
-['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS().__call__() #1
-success sender except ExceptSMS as e: #2 except sender sys.exit() SendSMS
-().__call__() #3 customized sender ```
+## *SMS* [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing) - a. Sign up for Twilio. [https:
+//www.twilio.com/en-us](https://www.twilio.com/en-us) - b. Click Console in the
+upper right corner. - c. Copy the variables provided in the console. *API TEST*
+```python from ExceptNotifier import send_sms_msg _TWILIO_SID = 'xxxx'
+_TWILIO_TOKEN = "xxxx" _SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER =
+"xxxx" send_sms_msg( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER,
+_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` *Notifier* ```python import
+sys from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
+ExceptSMS.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TWILIO_SID'] = 'xxxx' os.environ
+['_TWILIO_TOKEN'] = 'yyyyyy' os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa",
+os.environ['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS
+().__call__() #1 success sender except ExceptSMS as e: #2 except sender
+sys.exit() SendSMS().__call__() #3 customized sender ```
 ## *Teams* - a. Create the channel that you want to notify. - b. `App` -
 `Search: webhook` - `Incoming Webhook` [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
```

### Comparing `exceptnotifier-0.2.2/README.md` & `exceptnotifier-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,17 +116,17 @@
 |:--:|:--|:--:|:--:|:--:|:---:|
 |Beep|N/A|Free|N/A|0min|[ExceptBeep](./tutorials/ExceptBeep/GUIDE.md)|
 |Desktop|N/A|Free|N/A|0min|[ExceptDesktop](./tutorials/ExceptDesktop/GUIDE.md)|
 |Telegram|`_TELEGRAM_TOKEN`|Freemium|Easy|2min|[ExceptTelegram](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) |
 |Discord|`_DISCORD_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptDiscord](./tutorials/ExceptTelegram/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lwsIBpql_1zgEdIWRw6O_jBOZKJdHqBh?usp=sharing) |
 |AWS Chime|`_CHIME_WEBHOOK_URL`|Freemium|Easy|1min|[ExceptChime](./tutorials/ExceptChime/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) |
-|G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md)|
+|G-Mail|`_GAMIL_RECIPIENT_ADDR`, `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) |
-|SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md)|
+|SMS|`_TWILIO_SID`, `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
 |Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/ExceptTeams/GUIDE.md)|
 |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)|
 
 
 If you add the following two variables to the required variables for each application in the table above, you can receive error location and explanation, as well as examples, from OpenAI's model
 
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
@@ -171,15 +171,15 @@
     print(1/0)
 except ExceptTelegram:    # sending except message to telegram
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
-![](./assets/imgs/ex02.png)
+![](./assets/imgs/ex02_1.png)
 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
@@ -289,15 +289,15 @@
   print(1/0)
 except:
   raise
 ```
 
 *Example code With Open AI API*
 
-![](./assets/imgs/ex07.png)
+![](./assets/imgs/ex07_1.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
 os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"    
@@ -423,14 +423,16 @@
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
 ## *Mail*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)
+
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en). 
 
 *API TEST*
 ```python
 from ExceptNotifier import send_gmail_msg
@@ -663,14 +665,16 @@
 
 SendLine().__call__()        #3 customized sender          
 ```
 
 <Br>
 
 ## *SMS*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)
+
 - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://www.twilio.com/en-us)
 - b. Click Console in the upper right corner.
 - c. Copy the variables provided in the console.
 
 
 *API TEST*
 ```python
```

#### html2text {}

```diff
@@ -85,29 +85,34 @@
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1hUMMQ6He9M4MlspZ88J9kO8juxvC5b3a?usp=sharing)|
 |Slack|`_SLACK_WEBHOOK_URL`|Freemium|Easy|3min|[ExceptSlack](./tutorials/
 ExceptSlack/GUIDE.md) [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/1-
 dAaKl_gwX481FxH424aCVFqsq-thGXK?usp=sharing) | |G-Mail|`_GAMIL_RECIPIENT_ADDR`,
 `_GMAIL_SENDER_ADDR`, `_GMAIL_APP_PASSWORD_OF_SENDER` |Restricted
-free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md)|
+free|Medium|3min|[ExceptMail](./tutorials/ExceptMail/GUIDE.md) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing)|
 |Line|`_LINE_NOTIFY_API_TOKEN`|Freemium|Medium|4min|[ExceptLine](./tutorials/
 ExceptLine/GUIDE.md) [![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
 1PDrJqxDq4NE6BRUrRkFvDBiMHQz0WbZh?usp=sharing) | |SMS|`_TWILIO_SID`,
 `_TWILIO_TOKEN`, `_RECIPIENT_PHONE_NUMBER`, `_SENDER_PHONE_NUMBER`|Not
-free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md)| |Microsoft
-Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./tutorials/
-ExceptTeams/GUIDE.md)| |KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min
-(Token refreshes daily)|[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you
-add the following two variables to the required variables for each application
-in the table above, you can receive error location and explanation, as well as
-examples, from OpenAI's model | API | Required Variables | Free or Paid | Ease
-of Setup | Time Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:-
--:|:---:| | OpenAI API |`Required variables for each application`+
+free|Medium|5min|[ExceptSMS](./tutorials/ExceptSMS/GUIDE.md) [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing)|
+|Microsoft Teams|`_TEAMS_WEBHOOK_URL`|Not Free|Medium|5min|[ExceptTeams](./
+tutorials/ExceptTeams/GUIDE.md)|
+|KakaoTalk|`_KAKAO_TOKEN_PATH`|Freemium|Hell|>=10min(Token refreshes daily)|
+[ExceptKakao](./tutorials/ExceptKakao/GUIDE.md)| If you add the following two
+variables to the required variables for each application in the table above,
+you can receive error location and explanation, as well as examples, from
+OpenAI's model | API | Required Variables | Free or Paid | Ease of Setup | Time
+Required for Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |
+OpenAI API |`Required variables for each application`+
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](./documents/
 APIOpenAI/GUIDE.md)|
 # Tutorial I will update tutorial ASAP. `README.md` is sufficient, but read the
 application's official documentation if necessary. However, we are preparing a
 more detailed and friendly tutorial. 1. Main-tutorials: [Notebook](https://
 github.com/DSDanielPark/ExceptNotifier/blob/main/tutorial/ExceptNotifier.ipynb)
 2. Sub-tutorial-folder: Tutorials for each function can be found in this
@@ -125,17 +130,17 @@
 
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex02.png) You can receive debugging information
-from ChatGPT via OpenAI's API when using the Except statement. The syntax
-remains the same, but you'll need to configure these two variables:
+Notification ![](./assets/imgs/ex02_1.png) You can receive debugging
+information from ChatGPT via OpenAI's API when using the Except statement. The
+syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
 ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
 Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
 Type: Class
@@ -177,15 +182,15 @@
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier. - Format: Except[appName] -
 Type: function
 *Example code without Open AI API* ![](./assets/imgs/ex06.png) ```python from
 ExceptNotifier import ExceptTelegramIpython import os os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) try: print(1/0) except: raise ``` *Example code With
-Open AI API* ![](./assets/imgs/ex07.png) ```python from ExceptNotifier import
+Open AI API* ![](./assets/imgs/ex07_1.png) ```python from ExceptNotifier import
 ExceptTelegramIpython import os get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"
 os.environ['_OPEN_AI_API'] = "sk-xxxxx" os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 try: print(1/0) except: raise ``` ## Success`Notifier` in Ipython ![](./assets/
 imgs/ex08.png) - Same syntax in Python. See Python Core above. ```python import
 sys import os from ExceptNotifier import SuccessTelegram os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" try: print(1/20) # Your Code Here SuccessTelegram
@@ -230,16 +235,19 @@
 update it so that other models can be used later. *Notifier* ```python from
 ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram import sys,
 os sys.excepthook = ExceptTelegram.__call__ os.environ['_TELEGRAM_TOKEN'] =
 "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-turbo" os.envirion
 ['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
 success sender except ExceptTelegram as e: #2. except sender sys.exit()
 SendTelegram().__call__() #3. customized sender ```
-## *Mail* In the except statement, an email is sent along with the error
-message. Additionally, you can send emails from any desired line.
+## *Mail* [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+1IfDIliImFKG4UuM0yzerhubL_Kx_TFKF?usp=sharing) In the except statement, an
+email is sent along with the error message. Additionally, you can send emails
+from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
 (https://myaccount.google.com/u/3/apppasswords?utm_source=google-
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
 *API TEST* ```python from ExceptNotifier import send_gmail_msg
@@ -327,29 +335,31 @@
 ```python import sys from ExceptNotifier import ExceptLine, SuccessLine,
 SendLine sys.excepthook = ExceptLine.__call__ # Define the next two variables
 optionally when using OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx" os.environ
 ['_LINE_NOTIFY_API_TOKEN'] = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
 ().__call__() #1 success sender except ExceptLine as e: #2 except sender
 sys.exit() SendLine().__call__() #3 customized sender ```
-## *SMS* - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://
-www.twilio.com/en-us) - b. Click Console in the upper right corner. - c. Copy
-the variables provided in the console. *API TEST* ```python from ExceptNotifier
-import send_sms_msg _TWILIO_SID = 'xxxx' _TWILIO_TOKEN = "xxxx"
-_SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER = "xxxx" send_sms_msg
-( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER,
-"Any Test Message") ``` *Notifier* ```python import sys from ExceptNotifier
-import ExceptSMS, SuccessSMS, SendSMS sys.excepthook = ExceptSMS.__call__ #
-Define the next two variables optionally when using OpenAI's API. # os.environ
-['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
-os.environ['_TWILIO_SID'] = 'xxxx' os.environ['_TWILIO_TOKEN'] = 'yyyyyy'
-os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa", os.environ
-['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS().__call__() #1
-success sender except ExceptSMS as e: #2 except sender sys.exit() SendSMS
-().__call__() #3 customized sender ```
+## *SMS* [![Open In Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/drive/
+13NuBhAxhwo67oc4jn3y8zpJiJrR-LHrP?usp=sharing) - a. Sign up for Twilio. [https:
+//www.twilio.com/en-us](https://www.twilio.com/en-us) - b. Click Console in the
+upper right corner. - c. Copy the variables provided in the console. *API TEST*
+```python from ExceptNotifier import send_sms_msg _TWILIO_SID = 'xxxx'
+_TWILIO_TOKEN = "xxxx" _SENDER_PHONE_NUMBER = "xxxx" _RECIPIENT_PHONE_NUMBER =
+"xxxx" send_sms_msg( _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER,
+_RECIPIENT_PHONE_NUMBER, "Any Test Message") ``` *Notifier* ```python import
+sys from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
+ExceptSMS.__call__ # Define the next two variables optionally when using
+OpenAI's API. # os.environ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ
+['_OPEN_AI_API']="sk-xxxxxx" os.environ['_TWILIO_SID'] = 'xxxx' os.environ
+['_TWILIO_TOKEN'] = 'yyyyyy' os.environ['_RECIPIENT_PHONE_NUMBER']="+aaaaaa",
+os.environ['_SENDER_PHONE_NUMBER']="+bbbbbb", try: print(1/10) SuccessSMS
+().__call__() #1 success sender except ExceptSMS as e: #2 except sender
+sys.exit() SendSMS().__call__() #3 customized sender ```
 ## *Teams* - a. Create the channel that you want to notify. - b. `App` -
 `Search: webhook` - `Incoming Webhook` [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
```

### Comparing `exceptnotifier-0.2.2/setup.py` & `exceptnotifier-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.2.2",
+    version="0.2.3",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```

