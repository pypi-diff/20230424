# Comparing `tmp/exceptnotifier-0.2.0.tar.gz` & `tmp/exceptnotifier-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.2.0.tar", last modified: Fri Apr 21 19:19:41 2023, max compression
+gzip compressed data, was "exceptnotifier-0.2.1.tar", last modified: Mon Apr 24 08:17:47 2023, max compression
```

## Comparing `exceptnotifier-0.2.0.tar` & `exceptnotifier-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.459294 exceptnotifier-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.323945 exceptnotifier-0.2.0/ExceptNotifier/
--rw-rw-rw-   0        0        0     4626 2023-04-21 19:18:38.000000 exceptnotifier-0.2.0/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.382956 exceptnotifier-0.2.0/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1380 2023-04-21 19:18:43.000000 exceptnotifier-0.2.0/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      532 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      788 2023-04-19 19:04:19.000000 exceptnotifier-0.2.0/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      536 2023-04-19 19:04:19.000000 exceptnotifier-0.2.0/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0     1004 2023-04-21 17:09:30.000000 exceptnotifier-0.2.0/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1323 2023-04-19 22:26:04.000000 exceptnotifier-0.2.0/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.0/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1865 2023-04-19 22:25:57.000000 exceptnotifier-0.2.0/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     2338 2023-04-21 14:57:38.000000 exceptnotifier-0.2.0/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.0/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1413 2023-04-19 22:25:46.000000 exceptnotifier-0.2.0/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      637 2023-04-19 19:04:19.000000 exceptnotifier-0.2.0/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      932 2023-04-19 22:25:37.000000 exceptnotifier-0.2.0/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      582 2023-04-21 13:09:42.000000 exceptnotifier-0.2.0/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1470 2023-04-19 19:04:19.000000 exceptnotifier-0.2.0/ExceptNotifier/base/whatsapp_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.413155 exceptnotifier-0.2.0/ExceptNotifier/ipython/
--rw-rw-rw-   0        0        0     1356 2023-04-21 19:18:47.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/__init__.py
--rw-rw-rw-   0        0        0      163 2023-04-21 18:39:14.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/beep_notifier_ipython.py
--rw-rw-rw-   0        0        0     1774 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/chime_notifier_ipython.py
--rw-rw-rw-   0        0        0     2135 2023-04-21 18:37:56.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/desktop_notifier_ipython.py
--rw-rw-rw-   0        0        0     1786 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/discord_notifier_ipython.py
--rw-rw-rw-   0        0        0     1773 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/kakao_notifier_ipython.py
--rw-rw-rw-   0        0        0     1779 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/line_notifier_ipython.py
--rw-rw-rw-   0        0        0     2630 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/mail_notifier_ipython.py
--rw-rw-rw-   0        0        0     1773 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/slack_notifier_ipython.py
--rw-rw-rw-   0        0        0     2086 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/sms_notifier_ipython.py
--rw-rw-rw-   0        0        0     1781 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/teams_notifier_ipython.py
--rw-rw-rw-   0        0        0     1687 2023-04-21 18:12:10.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/telegram_notifier_ipython.py
--rw-rw-rw-   0        0        0     1781 2023-04-21 18:11:41.000000 exceptnotifier-0.2.0/ExceptNotifier/ipython/wechat_notifier_ipython.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.443812 exceptnotifier-0.2.0/ExceptNotifier/python/
--rw-rw-rw-   0        0        0     1860 2023-04-21 19:18:52.000000 exceptnotifier-0.2.0/ExceptNotifier/python/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/beep_notifier.py
--rw-rw-rw-   0        0        0     6601 2023-04-21 18:13:41.000000 exceptnotifier-0.2.0/ExceptNotifier/python/chime_notifier.py
--rw-rw-rw-   0        0        0     6110 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/desktop_notifier.py
--rw-rw-rw-   0        0        0     6834 2023-04-21 18:13:45.000000 exceptnotifier-0.2.0/ExceptNotifier/python/discord_notifier.py
--rw-rw-rw-   0        0        0     6948 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/kakao_notifier.py
--rw-rw-rw-   0        0        0     6439 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/line_notifier.py
--rw-rw-rw-   0        0        0     8676 2023-04-21 14:16:30.000000 exceptnotifier-0.2.0/ExceptNotifier/python/mail_notifier.py
--rw-rw-rw-   0        0        0     6540 2023-04-21 18:14:06.000000 exceptnotifier-0.2.0/ExceptNotifier/python/slack_notifier.py
--rw-rw-rw-   0        0        0     6942 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/sms_notifier.py
--rw-rw-rw-   0        0        0     6399 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/teams_notifier.py
--rw-rw-rw-   0        0        0     6730 2023-04-21 12:51:31.000000 exceptnotifier-0.2.0/ExceptNotifier/python/telegram_notifier.py
--rw-rw-rw-   0        0        0     6488 2023-04-20 06:16:28.000000 exceptnotifier-0.2.0/ExceptNotifier/python/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.452989 exceptnotifier-0.2.0/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      265 2023-04-21 19:18:57.000000 exceptnotifier-0.2.0/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.0/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:19:41.349317 exceptnotifier-0.2.0/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    33527 2023-04-21 19:19:41.000000 exceptnotifier-0.2.0/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-04-21 19:19:41.000000 exceptnotifier-0.2.0/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:19:41.000000 exceptnotifier-0.2.0/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-21 19:19:41.000000 exceptnotifier-0.2.0/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-04-21 19:19:41.000000 exceptnotifier-0.2.0/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-21 19:19:41.000000 exceptnotifier-0.2.0/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    33527 2023-04-21 19:19:41.458282 exceptnotifier-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    32479 2023-04-21 19:13:49.000000 exceptnotifier-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 19:19:41.459294 exceptnotifier-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1928 2023-04-21 19:18:30.000000 exceptnotifier-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.972786 exceptnotifier-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.826871 exceptnotifier-0.2.1/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4663 2023-04-24 08:16:39.000000 exceptnotifier-0.2.1/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.890412 exceptnotifier-0.2.1/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1382 2023-04-24 08:16:46.000000 exceptnotifier-0.2.1/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-04-20 06:16:28.000000 exceptnotifier-0.2.1/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.1/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1002 2023-04-23 07:06:21.000000 exceptnotifier-0.2.1/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.1/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.1/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.1/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.1/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.1/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.1/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      930 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      582 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1470 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.924670 exceptnotifier-0.2.1/ExceptNotifier/ipython/
+-rw-rw-rw-   0        0        0     1472 2023-04-24 08:16:42.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1808 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2189 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1820 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1807 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1813 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2579 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1807 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2096 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1811 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1721 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     1815 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.957266 exceptnotifier-0.2.1/ExceptNotifier/python/
+-rw-rw-rw-   0        0        0     1955 2023-04-24 08:16:48.000000 exceptnotifier-0.2.1/ExceptNotifier/python/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/beep_notifier.py
+-rw-rw-rw-   0        0        0     6722 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/chime_notifier.py
+-rw-rw-rw-   0        0        0     6177 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/desktop_notifier.py
+-rw-rw-rw-   0        0        0     7029 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/discord_notifier.py
+-rw-rw-rw-   0        0        0     7108 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/kakao_notifier.py
+-rw-rw-rw-   0        0        0     6634 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/line_notifier.py
+-rw-rw-rw-   0        0        0     8807 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/mail_notifier.py
+-rw-rw-rw-   0        0        0     6645 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/slack_notifier.py
+-rw-rw-rw-   0        0        0     7879 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/sms_notifier.py
+-rw-rw-rw-   0        0        0     6610 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/teams_notifier.py
+-rw-rw-rw-   0        0        0     6834 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/telegram_notifier.py
+-rw-rw-rw-   0        0        0     6625 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.966265 exceptnotifier-0.2.1/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      265 2023-04-24 08:16:52.000000 exceptnotifier-0.2.1/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.1/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.855873 exceptnotifier-0.2.1/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    33926 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    33926 2023-04-24 08:17:47.971790 exceptnotifier-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    32878 2023-04-23 13:32:03.000000 exceptnotifier-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:17:47.972786 exceptnotifier-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1958 2023-04-24 08:16:31.000000 exceptnotifier-0.2.1/setup.py
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/__init__.py` & `exceptnotifier-0.2.1/ExceptNotifier/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-
 from ExceptNotifier.utils.kakao_token import get_authorize_code, save_token
-
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.mail_sender import send_gmail_msg
 from ExceptNotifier.base.slack_sender import send_slack_msg
 from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.chime_sender import send_chime_msg
 from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.line_sender import send_line_msg
@@ -14,45 +12,43 @@
 from ExceptNotifier.base.whatsapp_sender import send_whatsapp_msg
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.beep_sender import beep
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 from ExceptNotifier.base.openai_receiver import get_resp_openai_advice
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.desktop_sender import send_desktop_msg
-
 from ExceptNotifier.python.mail_notifier import SuccessMail, ExceptMail, SendMail
 from ExceptNotifier.python.slack_notifier import SuccessSlack, ExceptSlack, SendSlack
 from ExceptNotifier.python.telegram_notifier import SuccessTelegram, ExceptTelegram, SendTelegram
 from ExceptNotifier.python.chime_notifier import SuccessChime, ExceptChime, SendChime
 from ExceptNotifier.python.discord_notifier import SuccessDiscord, ExceptDiscord, SendDiscord
 from ExceptNotifier.python.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
 from ExceptNotifier.python.line_notifier import SuccessLine, ExceptLine, SendLine
 from ExceptNotifier.python.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
 from ExceptNotifier.python.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
 from ExceptNotifier.python.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
-from ExceptNotifier.python.wechat_notifier import SuccessWechat, ExceptWechat, SendWechat
+from ExceptNotifier.python.wechat_notifier import SuccessWechat,ExceptWechat, SendWechat
 from ExceptNotifier.python.desktop_notifier import SuccessDesktop, ExceptDesktop, SendDesktop
-
 from ExceptNotifier.ipython.telegram_notifier_ipython import ExceptTelegramIpython
 from ExceptNotifier.ipython.chime_notifier_ipython import ExceptChimeIpython
 from ExceptNotifier.ipython.discord_notifier_ipython import ExceptDiscordIpython
 from ExceptNotifier.ipython.kakao_notifier_ipython import ExceptKakaoIpython
 from ExceptNotifier.ipython.line_notifier_ipython import ExceptLineIpython
 from ExceptNotifier.ipython.mail_notifier_ipython import ExceptMailIpython
 from ExceptNotifier.ipython.slack_notifier_ipython import ExceptSlackIpython
 from ExceptNotifier.ipython.sms_notifier_ipython import ExceptSMSIpython
 from ExceptNotifier.ipython.teams_notifier_ipython import ExceptTeamsIpython
 from ExceptNotifier.ipython.wechat_notifier_ipython import ExceptWechatIpython
 from ExceptNotifier.ipython.beep_notifier_ipython import ExceptBeepIpython
 from ExceptNotifier.ipython.desktop_notifier_ipython import ExceptDesktopIpython
 
-
 __all__ = [
-    "ExceptBeepIpython", "ExceptDesktopIpython"
-    "get_resp_openai_advice"
+    "ExceptBeepIpython",
+    "ExceptDesktopIpython",
+    "get_resp_openai_advice",
     "SuccessMail",
     "ExceptMail",
     "SendMail",
     "SuccessSlack",
     "ExceptSlack",
     "SendSlack",
     "SuccessTelegram",
@@ -94,16 +90,26 @@
     "receive_openai_advice",
     "beep",
     "send_gmail_msg",
     "SuccessWechat",
     "ExceptWechat",
     "SendWechat",
     "send_wechat_msg",
-    "send_desktop_msg","SuccessDesktop", "ExceptDesktop", "SendDesktop", "ExceptTelegramIpython",
-    "ExceptTelegramIpython", "ExceptChimeIpython", "ExceptDiscordIpython",
-           "ExceptKakaoIpython", "ExceptLineIpython", "ExceptMailIpython", "ExceptSlackIpython",
-           "ExceptSMSIpython", "ExceptTeamsIpython", "ExceptWechatIpython"
-
+    "send_desktop_msg",
+    "SuccessDesktop",
+    "ExceptDesktop",
+    "SendDesktop",
+    "ExceptTelegramIpython",
+    "ExceptTelegramIpython",
+    "ExceptChimeIpython",
+    "ExceptDiscordIpython",
+    "ExceptKakaoIpython",
+    "ExceptLineIpython",
+    "ExceptMailIpython",
+    "ExceptSlackIpython",
+    "ExceptSMSIpython",
+    "ExceptTeamsIpython",
+    "ExceptWechatIpython",
 ]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.mail_sender import send_gmail_msg
 from ExceptNotifier.base.slack_sender import send_slack_msg
 from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.chime_sender import send_chime_msg
 from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.line_sender import send_line_msg
@@ -12,27 +11,27 @@
 from ExceptNotifier.base.whatsapp_sender import send_whatsapp_msg
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.beep_sender import beep
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.openai_receiver import get_resp_openai_advice
 
-
 __all__ = [
     "send_kakao_msg",
     "send_gmail_msg",
     "send_slack_msg",
     "send_telegram_msg",
     "send_chime_msg",
     "send_discord_msg",
     "send_line_msg",
     "send_wechat_msg",
     "send_line_msg",
     "send_teams_msg",
     "send_whatsapp_msg",
     "send_sms_msg",
     "beep",
-    "receive_openai_advice", "get_resp_openai_advice"
+    "receive_openai_advice",
+    "get_resp_openai_advice",
 ]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/chime_sender.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,11 +22,10 @@
     message = {"Content": msg}
     encoded_msg = json.dumps(message).encode("utf-8")
     resp = http.request("POST", url, body=encoded_msg)
 
     return resp
 
 
-if __name__ == "__main__":
-    _CHIME_WEBHOOK_URL = "xxxxx"
-
-    send_chime_msg(_CHIME_WEBHOOK_URL, "Test")
+# if __name__ == "__main__":
+#     _CHIME_WEBHOOK_URL = "xxxxx"
+#     send_chime_msg(_CHIME_WEBHOOK_URL, "Test")
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/discord_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,9 +26,8 @@
         resp = webhook.send(content=msg)
     return resp
 
 
 # if __name__ == "__main__":
 #     _DISCORD_WEBHOOK_URL = "xxxxx"
 #     msg = "Sending Test"
-
 #     send_discord_msg(_DISCORD_WEBHOOK_URL, msg)
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/kakao_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,11 +36,10 @@
 
 
 # if __name__ == "__main__":
 #     global _KAKAO_TOKEN_PATH
 #     _KAKAO_TOKEN_PATH = (
 #         r"C:\Users\parkm\Desktop\git\ExceptionNotifier\tutorials\token.json"
 #     )
-
 #     msg = "Sending Message Test"
 #     resp_status = send_kakao_msg(_KAKAO_TOKEN_PATH, msg)
 #     print(resp_status)
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/mail_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 # if __name__ == "__main__":  # No-QA
 #     _GMAIL_SENDER_ADDR = "xxxxx@gmail.com"
 #     _GMAIL_APP_PASSWORD_OF_SENDER = "yyyyy"
 #     _GAMIL_RECIPIENT_ADDR = "zzzzz@gmail.com"
 #     subject_msg = "Python Code Alarm: Process End."
 #     body_msg = "Python Code Notice: \nA notification has arrived from your code."
-
 #     send_gmail_msg(
 #         _GMAIL_SENDER_ADDR,
 #         _GAMIL_RECIPIENT_ADDR,
 #         _GMAIL_APP_PASSWORD_OF_SENDER,
 #         subject_msg,
 #         body_msg,
 #     )
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/openai_receiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import openai
 
 
-def receive_openai_advice(_OPEN_AI_MODEL: str, _OPEN_AI_API: str, error_message: str) -> str:
+def receive_openai_advice(
+    _OPEN_AI_MODEL: str, _OPEN_AI_API: str, error_message: str
+) -> str:
     """Receive debugging information about your code from models in open ai.
 
     :param _OPEN_AI_MODEL: model name of open ai
     :type _OPEN_AI_MODEL: str
     :param _OPEN_AI_API: API KEY value of open ai
     :type _OPEN_AI_API: str
     :param error_message: Error message
@@ -23,16 +25,18 @@
     resp = openai.ChatCompletion.create(
         model=model_engine, messages=[{"role": "user", "content": input_text}]
     )
     advice_msg = resp["choices"][0]["message"]["content"]
     return advice_msg
 
 
-def get_resp_openai_advice(_OPEN_AI_MODEL: str, _OPEN_AI_API: str, error_message: str) -> dict:
-    """Receive debugging information about your code from models in open ai.
+def get_resp_openai_advice(
+    _OPEN_AI_MODEL: str, _OPEN_AI_API: str, error_message: str
+) -> dict:
+    """Check response of Open AI API status
 
     :param _OPEN_AI_MODEL: model name of open ai
     :type _OPEN_AI_MODEL: str
     :param _OPEN_AI_API: API KEY value of open ai
     :type _OPEN_AI_API: str
     :param error_message: Error message
     :type error_message: str
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/sms_sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,10 @@
 
 #     _TWILIO_SID = "xxxxx"
 #     _TWILIO_TOKEN = "yyyyy"
 #     client = Client(_TWILIO_SID, _TWILIO_TOKEN)
 #     _SENDER_PHONE_NUMBER = "+aaaaa"
 #     _RECIPIENT_PHONE_NUMBER = "+bbbbb"
 #     msg = "ExceptNotifier Test"
-
 #     send_sms_msg(
 #         _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, msg
 #     )
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/telegram_sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,10 @@
     bot_url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/sendMessage?chat_id={bot_id}&text={msg}"
     resp = requests.get(bot_url).json()
 
     return resp
 
 
 # if __name__ == "__main__":
-
 #     _TELEGRAM_TOKEN = "xxxxxxxxxx"
 #     msg = "Test Message"
 #     send_telegram_msg(_TELEGRAM_TOKEN, msg)
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/wechat_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.2.1/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/__init__.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,26 @@
 from ExceptNotifier.ipython.mail_notifier_ipython import ExceptMailIpython
 from ExceptNotifier.ipython.slack_notifier_ipython import ExceptSlackIpython
 from ExceptNotifier.ipython.sms_notifier_ipython import ExceptSMSIpython
 from ExceptNotifier.ipython.teams_notifier_ipython import ExceptTeamsIpython
 from ExceptNotifier.ipython.wechat_notifier_ipython import ExceptWechatIpython
 from ExceptNotifier.ipython.beep_notifier_ipython import ExceptBeepIpython
 from ExceptNotifier.ipython.desktop_notifier_ipython import ExceptDesktopIpython
+from ExceptNotifier.ipython.beep_notifier_ipython import ExceptBeepIpython
 
-__all__ = ["ExceptTelegramIpython", "ExceptChimeIpython", "ExceptDiscordIpython",
-           "ExceptKakaoIpython", "ExceptLineIpython", "ExceptMailIpython", "ExceptSlackIpython",
-           "ExceptSMSIpython", "ExceptTeamsIpython", "ExceptWechatIpython", "ExceptBeepIpython", "ExceptDesktopIpython"]
+__all__ = [
+    "ExceptTelegramIpython",
+    "ExceptChimeIpython",
+    "ExceptDiscordIpython",
+    "ExceptKakaoIpython",
+    "ExceptLineIpython",
+    "ExceptMailIpython",
+    "ExceptSlackIpython",
+    "ExceptSMSIpython",
+    "ExceptTeamsIpython",
+    "ExceptWechatIpython",
+    "ExceptBeepIpython",
+    "ExceptDesktopIpython",
+]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/chime_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/chime_notifier_ipython.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_chime_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptChimeIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,24 +17,28 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}" }
-    
-    send_chime_msg(os.environ['_CHIME_WEBHOOK_URL'], data['text'])
+    data = {
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    }
+
+    send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/desktop_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/desktop_notifier_ipython.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_desktop_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptDesktopIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,25 +17,31 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}" }
-    data['head'] = '[Except Notifier] :warning: Error! Python Code Exception Detected.'
-    data['body'] = f'IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}'
-    send_desktop_msg(data['head'], data['body'])
+    data = {
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    }
+    data["head"] = "[Except Notifier] :warning: Error! Python Code Exception Detected."
+    data[
+        "body"
+    ] = f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    send_desktop_msg(data["head"], data["body"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_desktop_msg(os.environ["_CHIME_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/discord_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/discord_notifier_ipython.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_discord_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptDiscordIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,24 +17,28 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}" }
-    
-    send_discord_msg(os.environ['_DISCORD_WEBHOOK_URL'], data['text'])
+    data = {
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    }
+
+    send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/kakao_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/kakao_notifier_ipython.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_kakao_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptKakaoIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,24 +17,28 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}" }
-    
-    send_kakao_msg(os.environ['_KAKAO_TOKEN_PATH'], data['text'])
+    data = {
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+    }
+
+    send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/line_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/line_notifier_ipython.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_line_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptLineIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,24 +17,28 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}" }
-    
-    send_line_msg(os.environ['_LINE_NOTIFY_API_TOKEN'], data['text'])
+    data = {
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+    }
+
+    send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/mail_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/mail_notifier_ipython.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 import datetime
 import smtplib
 import datetime
 from ExceptNotifier import receive_openai_advice
 import os
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptMailIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -19,46 +20,41 @@
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     SMTP_SERVER = "smtp.gmail.com"
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     exceptNotifier = {
-    "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
-    "FROM": os.environ["_GMAIL_SENDER_ADDR"],
-    "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected.",
-    "BODY": f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}",
+        "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
+        "FROM": os.environ["_GMAIL_SENDER_ADDR"],
+        "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected.",
+        "BODY": f"IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}",
     }
     smtp = smtplib.SMTP_SSL(SMTP_SERVER, 465)
     smtp.login(
-        os.environ["_GMAIL_SENDER_ADDR"],
-        os.environ["_GMAIL_APP_PASSWORD_OF_SENDER"],
-    )
-    smtp.sendmail(
-        exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
+        os.environ["_GMAIL_SENDER_ADDR"], os.environ["_GMAIL_APP_PASSWORD_OF_SENDER"],
     )
+    smtp.sendmail(exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"])
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
         advice_msg = receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"],
-                os.environ["_OPEN_AI_API"],
-                error_message,
-            )  # NO-QA
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message,
+        )  # NO-QA
         exceptNotifier = {
             "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
             "FROM": os.environ["_GMAIL_SENDER_ADDR"],
             "SUBJECT": "[Except AI Debugging] Error! chatGPT Debugging guide.",
             "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}",
         }
         smtp.sendmail(
             exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
         )
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/slack_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/slack_notifier_ipython.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_slack_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptSlackIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,24 +17,28 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] :warning: Error! Python Code Exception Detected \n IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}" }
-    
+    data = {
+        "text": f"[Except Notifier] :warning: Error! Python Code Exception Detected \n IMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry:  {sstb}"
+    }
+
     send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/sms_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/sms_notifier_ipython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_sms_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptSMSIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,34 +17,38 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] ** Error ** Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}" }
-    
+    data = {
+        "text": f"[Except Notifier] ** Error ** Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n * Code Status: Fail.🛠 \n * Detail: Python Code Ran Exceptions. \n * Time: {start_time.strftime(DATE_FORMAT)} \n\n ** {sstb}"
+    }
+
     send_sms_msg(
-            os.environ["_TWILIO_SID"],
-            os.environ["_TWILIO_TOKEN"],
-            os.environ["_SENDER_PHONE_NUMBER"],
-            os.environ["_RECIPIENT_PHONE_NUMBER"],
-            data["text"],
-        )
+        os.environ["_TWILIO_SID"],
+        os.environ["_TWILIO_TOKEN"],
+        os.environ["_SENDER_PHONE_NUMBER"],
+        os.environ["_RECIPIENT_PHONE_NUMBER"],
+        data["text"],
+    )
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_sms_msg(
             os.environ["_TWILIO_SID"],
             os.environ["_TWILIO_TOKEN"],
             os.environ["_SENDER_PHONE_NUMBER"],
             os.environ["_RECIPIENT_PHONE_NUMBER"],
             advice_msg,
         )
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/teams_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/teams_notifier_ipython.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_teams_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptTeamsIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,25 +17,29 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}" }
-    
-    send_teams_msg(os.environ['_TEAMS_WEBHOOK_URL'], data['text'])
+    data = {
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+    }
+
+    send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/telegram_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/telegram_notifier_ipython.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_telegram_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptTelegramIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -14,24 +15,28 @@
     :param etype: Error type
     :type etype: _type_
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}" }
-    
-    send_telegram_msg(os.environ['_TELEGRAM_TOKEN'], data['text'])
+    data = {
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+    }
+
+    send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/ipython/wechat_notifier_ipython.py` & `exceptnotifier-0.2.1/ExceptNotifier/ipython/wechat_notifier_ipython.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2023 parkminwoo
 from IPython.core.ultratb import AutoFormattedTB
 from ExceptNotifier import send_wechat_msg, receive_openai_advice
 import os
 import datetime
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def ExceptWechatIpython(shell, etype, evalue, tb, tb_offset=1):
     """ExceptNotifier function for overriding custom execute in ipython
 
     :param shell: Excecuted shell 
@@ -16,24 +17,28 @@
     :param evalue: Error value
     :type evalue: _type_
     :param tb: TraceBack
     :type tb: _type_
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-    itb = AutoFormattedTB(mode = 'Plain', tb_offset = 1)
+    itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
-    data = {'text' : f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}" }
-    
-    send_wechat_msg(os.environ['_WECHAT_WEBHOOK_URL'], data['text'])
+    data = {
+        "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
+    }
+
+    send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
-        advice_msg = receive_openai_advice(os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message)
+        advice_msg = receive_openai_advice(
+            os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
+        )
         send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
-        pass
+        pass
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/__init__.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 from ExceptNotifier.python.mail_notifier import SuccessMail, ExceptMail, SendMail
 from ExceptNotifier.python.slack_notifier import SuccessSlack, ExceptSlack, SendSlack
-from ExceptNotifier.python.telegram_notifier import SuccessTelegram, ExceptTelegram, SendTelegram
+from ExceptNotifier.python.telegram_notifier import (
+    SuccessTelegram,
+    ExceptTelegram,
+    SendTelegram,
+)
 from ExceptNotifier.python.chime_notifier import SuccessChime, ExceptChime, SendChime
-from ExceptNotifier.python.discord_notifier import SuccessDiscord, ExceptDiscord, SendDiscord
+from ExceptNotifier.python.discord_notifier import (
+    SuccessDiscord,
+    ExceptDiscord,
+    SendDiscord,
+)
 from ExceptNotifier.python.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
 from ExceptNotifier.python.line_notifier import SuccessLine, ExceptLine, SendLine
 from ExceptNotifier.python.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
 from ExceptNotifier.python.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
 from ExceptNotifier.python.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
-from ExceptNotifier.python.wechat_notifier import SuccessWechat, ExceptWechat, SendWechat
-from ExceptNotifier.python.desktop_notifier import SuccessDesktop, ExceptDesktop, SendDesktop
+from ExceptNotifier.python.wechat_notifier import (
+    SuccessWechat,
+    ExceptWechat,
+    SendWechat,
+)
+from ExceptNotifier.python.desktop_notifier import (
+    SuccessDesktop,
+    ExceptDesktop,
+    SendDesktop,
+)
 
 __all__ = [
     "SuccessMail",
     "ExceptMail",
     "SendMail",
     "SuccessSlack",
     "ExceptSlack",
@@ -41,12 +57,14 @@
     "SendSMS",
     "SuccessBeep",
     "ExceptBeep",
     "SendBeep",
     "SuccessWechat",
     "ExceptWechat",
     "SendWechat",
-    "SuccessDesktop", "ExceptDesktop", "SendDesktop"
+    "SuccessDesktop",
+    "ExceptDesktop",
+    "SendDesktop",
 ]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/beep_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/beep_notifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import sys
 import os
 import platform
 from ExceptNotifier import beep
 
 
 class ExceptBeep(BaseException):
+    """Override excepthook to send error message to beep.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Line.
 
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
 
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
 
@@ -44,35 +45,36 @@
 
             winsound.Beep(int(1000 * sec), freq)
         else:
             os.system("play -nq -t alsa synth {} sine {}".format(sec, freq))
 
 
 class SuccessBeep:
+    """Success beep
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
 
 
 class SendBeep:
+    """Send beep
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         beep(os.environ["BEEP_TIME"])
 
 
 # if __name__ == "__main__":
-#     BEEP_TIME = 1
+#     os.environ['BEEP_TIME'] = 1
 #     sys.excepthook = ExceptBeep.__call__
-
 #     try:
 #         print(1 / 20)
 #         SuccessBeep().__call__()  # 1 success beep-beep
-
 #     except ExceptBeep as e:  # 2 except beep-beep
 #         sys.exit()
-
 #     SendBeep().__call__()  # 3 customized beep-beep
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/chime_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/chime_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 import os
 
 http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptChime(BaseException):
+    """Override excepthook to send error message to AWS Chime.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to AWS Chime.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
             "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
@@ -106,14 +106,16 @@
         encoded_msg = json.dumps(message).encode("utf-8")
         resp = http.request("POST", url, body=encoded_msg)
 
         return resp
 
 
 class SuccessChime:
+    """Sending success message to AWS Chime
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -126,14 +128,16 @@
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 class SendChime:
+    """Sending message to AWS Chime
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -149,22 +153,17 @@
         send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
 
 #     """Get your Webhook _CHIME_WEBHOOK_URL from your chatroom.
 #     https://docs.aws.amazon.com/chime/latest/ag/webhooks.html"""
-
-
-# _CHIME_WEBHOOK_URL = "xxxxxxxxxxxxxxxxxx"
-# _OPEN_AI_API = "xxxxxxxxxxxxx"
-# _OPEN_AI_MODEL = "gpt-3.5-turbo"
+# os.environ['_CHIME_WEBHOOK_URL'] = "xxxxxxxxxxxxxxxxxx"
+# os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 # sys.excepthook = ExceptChime.__call__
-
 # try:
 #     print(1 / 0)
 #     SuccessChime().__call__()  # 1 success sender
-
 # except ExceptChime as e:  # 2 except sender
 #     sys.exit()
-
 # SendChime().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/desktop_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/desktop_notifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from ExceptNotifier import send_desktop_msg, receive_openai_advice
 import os
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptDesktop(BaseException):
+    """Override excepthook to send error message to Desktop.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Line.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
             "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
@@ -102,14 +102,16 @@
         :param DISP_TIME: Time duration, defaults to 5
         :type DISP_TIME: int, optional
         """
         notification.notify(title=title_msg, message=body_msg, timeout=DISP_TIME)
 
 
 class SuccessDesktop:
+    """Sending success message to Desktop
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -122,14 +124,16 @@
 
         send_desktop_msg(
             title=exceptNotifier["SUBJECT"][:20], message=exceptNotifier["BODY"][:200]
         )
 
 
 class SendDesktop:
+    """Sending message to Desktop
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/discord_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/wechat_notifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
+import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-from ExceptNotifier import send_discord_msg, receive_openai_advice
+from ExceptNotifier import send_wechat_msg, receive_openai_advice
 import os
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptDiscord(BaseException):
+class ExceptWechat(BaseException):
+    """Override excepthook to send error message to Wechat.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Discord.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
-            "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
-            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
         }
         for line in traceback.extract_tb(tb):
             exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
@@ -47,125 +48,113 @@
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-
         exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
             exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
                 frame.f_code.co_name,
                 frame.f_code.co_filename,
                 frame.f_lineno,
             )
             for key, val in frame.f_locals.items():
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        print(exceptNotifier["BODY"])
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"])
+        send_wechat_msg(os.enviro["_WECHAT_WEBHOOK_URL"], data["text"])
 
         try:
             error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
             advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
             )
             advice_msg += receive_openai_advice(
                 os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
             )  # NO-QA
-            send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], advice_msg)
+            send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], advice_msg)
         except Exception as e:
             print(e)
             pass
 
     @staticmethod
-    def send_discord_msg(_DISCORD_WEBHOOK_URL: str, msg: str) -> dict:
-        """Send message to chat room through discord app's webhook url.
+    def send_wechat_msg(_WECHAT_WEBHOOK_URL: str, msg: str) -> None:
+        """Send message to wechat.
 
-        :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
-        :type _DISCORD_WEBHOOK_URL: str
-        :param msg: Message text
+        :param _WECHAT_WEBHOOK_URL: Wechat Webhook URL https://work.weixin.qq.com/api/doc/90000/90136/91770
+        :type _WECHAT_WEBHOOK_URL: str
+        :param msg: Message to send
         :type msg: str
-        :return: Response according to REST API request
-        :rtype: dict
         """
-        try:
-            from discord import Webhook, RequestsWebhookAdapter
-
-            webhook = Webhook.from_url(
-                _DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter()
-            )
-            resp = webhook.send(msg)
-        except:
-            from discord import SyncWebhook
-
-            webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL)  # Initializing webhook
-            resp = webhook.send(content=msg)
-        return resp
+        msg_template = {"msgtype": "text", "text": {"content": ""}}
+        msg_template["text"]["content"] = "\n".join(msg)
+        requests.post(_WECHAT_WEBHOOK_URL, json=msg_template)
 
 
-class SuccessDiscord:
+class SuccessWechat:
+    """Sending success message to wechat
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
-            "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
 
+        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
-class SendDiscord:
+
+class SendWechat:
+    """Sending message to wechat
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
-            "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
+        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
-
-#     """Get your _DISCORD_WEBHOOK_URL from HERE.
-#     https://discord.com/developers/docs/resources/webhook"""
-
-
-#     _DISCORD_WEBHOOK_URL = "xxxxxxxxxxxxxxxxx"
-
-#     sys.excepthook = ExceptDiscord.__call__
-
+#     """Get your wechat webhook URL.
+#     https://work.weixin.qq.com/api/doc/90000/90136/91770"""
+#     os.environ['_WECHAT_WEBHOOK_URL'] = "xxxxxxxxxxx"
+#     # os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     # os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     sys.excepthook = ExceptWechat.__call__
 #     try:
-#         print(1 / 20)
-#         SuccessDiscord().__call__()  # 1 success sender
-
-#     except ExceptDiscord as e:  # 2 except sender
+#         print(1 / 0)
+#         SuccessWechat().__call__()  # 1 success sender
+#     except ExceptWechat as e:  # 2 except sender
 #         sys.exit()
-
-#     SendDiscord().__call__()  # 3 customized sender
+#     SendWechat().__call__()  # 3 customized sender
+#     send = SendWechat()  # You can use it like this, too.
+#     send() # 3 cusotomized sender
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/kakao_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/kakao_notifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 import os
 from ExceptNotifier import send_kakao_msg, receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptKakao(BaseException):
+    """Override excepthook to send error message to Kakaotalk.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Kakaotalk.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
             "SUBJECT": "[Except Notifier] ** Error! ** Python Code Exception Detected",
@@ -118,14 +118,16 @@
         data = {"template_object": json.dumps(data)}
         resp = requests.post(url, headers=headers, data=data)
 
         return resp
 
 
 class SuccessKakao:
+    """Sending success message to Kakaotalk
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -138,14 +140,16 @@
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
 
 
 class SendKakao:
+    """Sending message to Kakaotalk
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -161,25 +165,19 @@
         with open(os.environ["_KAKAO_TOKEN_PATH"], "r") as kakao:
             tokens = json.load(kakao)
 
         send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
 
 
 # if __name__ == "__main__":
-
-#     """Follow next notebooks"""
-
-
-#     _KAKAO_TOKEN_PATH = (
+#     os.environ['_KAKAO_TOKEN_PATH'] = (
 #         r"C:\Users\parkm\Desktop\git\ExceptionNotifier\tutorials\token.json"
 #     )
-
+#     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     sys.excepthook = ExceptKakao.__call__
-
 #     try:
 #         print(1 / 0)
 #         SuccessKakao().__call__()  # 1 success sender
-
 #     except ExceptKakao as e:  # 2 except sender
 #         sys.exit()
-
 #     SendKakao().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/line_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/line_notifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # Copyright 2023 parkminwoo Authors.
-
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 from ExceptNotifier import send_line_msg, receive_openai_advice
 import os
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptLine(BaseException):
+    """Override excepthook to send error message to Line.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Line.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
             "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
@@ -103,14 +102,16 @@
         headers = {"Authorization": "Bearer " + _LINE_NOTIFY_API_TOKEN}
         message = {"message": msg}
         resp = requests.post(api_url, headers=headers, data=message)
         return resp
 
 
 class SuccessLine:
+    """Sending success message to Line
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -123,14 +124,16 @@
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 class SendLine:
+    """Sending success message to Line
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -143,24 +146,19 @@
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 # if __name__ == "__main__":
-
 #     """Get your URL from HERE.
 #     https://notify-bot.line.me/my/"""
-
-
-#     _LINE_NOTIFY_API_TOKEN = "xxxxxxxxxxx"
-
+# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     os.environ['_LINE_NOTIFY_API_TOKEN'] = "xxxxxxxxxxx"
 #     sys.excepthook = ExceptLine.__call__
-
 #     try:
 #         print(1 / 20)
 #         SuccessLine().__call__()  # 1 success sender
-
 #     except ExceptLine as e:  # 2 except sender
 #         sys.exit()
-
 #     SendLine().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/mail_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/mail_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 from ExceptNotifier import send_gmail_msg, receive_openai_advice
 import os
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptMail(BaseException):
+    """Override excepthook to send error message to Gmail.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Gmail.
 
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         exceptNotifier = {
             "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
             "FROM": os.environ["_GMAIL_SENDER_ADDR"],
             "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected",
@@ -89,17 +90,15 @@
             advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
             )
             advice_msg += receive_openai_advice(
-                os.environ["_OPEN_AI_MODEL"],
-                os.environ["_OPEN_AI_API"],
-                error_message,
+                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message,
             )  # NO-QA
             exceptNotifier = {
                 "TO": os.environ["_GAMIL_RECIPIENT_ADDR"],
                 "FROM": os.environ["_GMAIL_SENDER_ADDR"],
                 "SUBJECT": "[Except AI Debugging] Error! chatGPT Debugging guide.",
                 "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}",
             }
@@ -149,14 +148,16 @@
         resp = smtp.send_message(message)
         smtp.quit()
 
         return resp
 
 
 class SuccessMail:
+    """Sending success message to Gmail
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
@@ -178,14 +179,16 @@
         message["To"] = os.environ["_GAMIL_RECIPIENT_ADDR"]
 
         smtp.send_message(message)
         smtp.quit()
 
 
 class SendMail:
+    """Sending message to Gmail
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
@@ -206,23 +209,21 @@
         message["From"] = os.environ["_GMAIL_SENDER_ADDR"]
         message["To"] = os.environ["_GAMIL_RECIPIENT_ADDR"]
         smtp.send_message(message)
         smtp.quit()
 
 
 # if __name__ == "__main__":
-
 #     # Set global variables
+# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     global _GAMIL_RECIPIENT_ADDR, _GMAIL_SENDER_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER
-#     _GAMIL_RECIPIENT_ADDR = "parkminwoo1991@gmail.com"
-#     _GMAIL_SENDER_ADDR = "heydudenotice@gmail.com"
+#     _GAMIL_RECIPIENT_ADDR = "xxx@gmail.com"
+#     _GMAIL_SENDER_ADDR = "xxxx@gmail.com"
 #     _GMAIL_APP_PASSWORD_OF_SENDER = "xxxxxxxxxxx"
 #     sys.excepthook = ExceptMail.__call__
-
 #     try:
 #         print(1 / 0)
 #         SuccessMail().__call__()  # 1 success sender
-
 #     except ExceptMail as e:  # 2 except sender
 #         sys.exit()
-
 #     SendMail().__call__()  # 3 Any line sender
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/slack_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/teams_notifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 # Copyright 2023 parkminwoo
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
+import json
 import os
-from ExceptNotifier import send_slack_msg, receive_openai_advice
+from ExceptNotifier import send_teams_msg, receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptSlack(BaseException):
+class ExceptTeams(BaseException):
+    """Override excepthook to send error message to Microsoft Teams.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Slack.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
-            "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
-            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
         }
         for line in traceback.extract_tb(tb):
             exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
@@ -49,114 +50,118 @@
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
 
-        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
+        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
         for frame in stack:
             exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
                 frame.f_code.co_name,
                 frame.f_code.co_filename,
                 frame.f_lineno,
             )
             for key, val in frame.f_locals.items():
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
+
+        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
         try:
             error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
             advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
             )
             advice_msg += receive_openai_advice(
                 os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
             )  # NO-QA
-            send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], advice_msg)
+            send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
         except Exception as e:
             print(e)
             pass
 
     @staticmethod
-    def send_slack_msg(_SLACK_WEBHOOK_URL: str, msg: str) -> dict:
-        """Send message to chat room through slack app's api.
+    def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
+        """Send message to chat room through microsoft teams app's webhook url.
 
-        :param _SLACK_WEBHOOK_URL: _SLACK_WEBHOOK_URL from slack app
-        :type _SLACK_WEBHOOK_URL: str
+        :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
+        :type _TEAMS_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
 
-        data = {"text": msg}
-        resp = requests.post(url=_SLACK_WEBHOOK_URL, json=data["text"])
+        payload = {"text": msg}
+        headers = {"Content-Type": "application/json"}
+        resp = requests.post(
+            _TEAMS_WEBHOOK_URL, headers=headers, data=json.dumps(payload)
+        )
+
         return resp
 
 
-class SuccessSlack:
+class SuccessTeams:
+    """Sending success message to microsoft teams
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
-            "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data['text'])
+
+        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
 
-class SendSlack:
+class SendTeams:
+    """Sending message to microsoft teams
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
-            "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
-
 
-# if __name__ == "__main__":
-
-#     # Get your slack bot and enter _SLACK_WEBHOOK_URL
-#     """Get your _SLACK_WEBHOOK_URL from HERE.
-#     https://api.slack.com/messaging/webhooks#create_a_webhook"""
-
-
-#     os.environ['_SLACK_WEBHOOK_URL'] ='https://hooks.slack.com/services/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'
+        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
-#     sys.excepthook = ExceptSlack.__call__
 
+# if __name__ == "__main__":
+#     """Follow next page"""
+#     os.environ['_TEAMS_WEBHOOK_URL'] = "microsoft webhook _TEAMS_WEBHOOK_URL"
+# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     sys.excepthook = ExceptTeams.__call__
 #     try:
-#         print(1 / 0)
-#         SuccessSlack().__call__()  # 1 success sender
-
-#     except ExceptSlack as e:  # 2 except sender
+#         print(1 / 20)
+#         SuccessTeams().__call__()  # 1 success sender
+#     except ExceptTeams as e:  # 2 except sender
 #         sys.exit()
-
-#     SendSlack().__call__()  # 3 customized sender
+#     SendTeams().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/sms_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/sms_notifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 import os
 from ExceptNotifier import send_sms_msg, receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptSMS(BaseException):
+    """Override excepthook to send error message to SMS.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to SMS.
-
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
             "SUBJECT": "[Except Notifier] ** Error! ** Python Code Exception Detected",
@@ -98,23 +98,47 @@
             )
         except Exception as e:
             print(e)
             pass
 
     @staticmethod
     def send_sms_msg(
-        _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, msg
-    ):
+        _TWILIO_SID: str,
+        _TWILIO_TOKEN: str,
+        _SENDER_PHONE_NUMBER: str,
+        _RECIPIENT_PHONE_NUMBER: str,
+        msg: str,
+    ) -> dict:
+        """Send SMS through twilio platform.
+        https://www.twilio.com/en-us
+
+        :param _TWILIO_SID: Twilio personal _TWILIO_SID
+        :type _TWILIO_SID: str
+        :param _TWILIO_TOKEN: Twilio personal _TWILIO_TOKEN
+        :type _TWILIO_TOKEN: str
+        :param _SENDER_PHONE_NUMBER: Sender phone number
+        :type _SENDER_PHONE_NUMBER: str
+        :param _RECIPIENT_PHONE_NUMBER: Recipient phone number
+        :type _RECIPIENT_PHONE_NUMBER: str
+        :param msg: SMS content
+        :type msg: str
+        :return: Response dict
+        :rtype: dict
+        """
+
         client = Client(_TWILIO_SID, _TWILIO_TOKEN)
-        client.messages.create(
-            to=_RECIPIENT_PHONE_NUMBER, from_=_SENDER_PHONE_NUMBER, body=msg
+        resp = client.messages.create(
+            to=_RECIPIENT_PHONE_NUMBER, from_=_SENDER_PHONE_NUMBER, body=msg[:1500]
         )
+        return resp
 
 
 class SuccessSMS:
+    """Sending success message to SMS
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -133,14 +157,16 @@
             os.environ["_SENDER_PHONE_NUMBER"],
             os.environ["_RECIPIENT_PHONE_NUMBER"],
             data["text"],
         )
 
 
 class SendSMS:
+    """Sending message to SMS
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -159,29 +185,24 @@
             os.environ["_SENDER_PHONE_NUMBER"],
             os.environ["_RECIPIENT_PHONE_NUMBER"],
             data["text"],
         )
 
 
 # if __name__ == "__main__":
-
 #     """https://www.twilio.com/en-us"""
-
-
-#     _TWILIO_SID = "xxxx"
-#     _TWILIO_TOKEN = "yyyyyy"
-#     _RECIPIENT_PHONE_NUMBER = ("+aaaaaa",)
-#     _SENDER_PHONE_NUMBER = ("+bbbbbb",)
-
+#     os.environ['_TWILIO_SID'] = "xxxx"
+#     os.environ['_TWILIO_TOKEN'] = "yyyyyy"
+#     os.environ['_RECIPIENT_PHONE_NUMBER'] = ("+aaaaaa",)
+#     os.environ['_SENDER_PHONE_NUMBER'] = ("+bbbbbb",)
 #     sys.excepthook = ExceptSMS.__call__
-
+# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     try:
 #         print(1 / 10)
 #         SuccessSMS().__call__()  # 1 success sender
-
 #     except ExceptSMS as e:  # 2 except sender
 #         with open("exceptError.pickle", "wb") as f:
 #             pickle.dump(e, f)
 #         raise pickle.load(f)
 #         sys.exit()
-
 #     SendSMS().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/teams_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/slack_notifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 # Copyright 2023 parkminwoo
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-import json
 import os
-from ExceptNotifier import send_teams_msg, receive_openai_advice
+from ExceptNotifier import send_slack_msg, receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptTeams(BaseException):
+class ExceptSlack(BaseException):
+    """Override excepthook to send error message to Slack.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Microsoft Teams.
 
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
-            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
-            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
+            "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
         }
         for line in traceback.extract_tb(tb):
             exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
@@ -50,119 +50,113 @@
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
 
-        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
             exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
                 frame.f_code.co_name,
                 frame.f_code.co_filename,
                 frame.f_lineno,
             )
             for key, val in frame.f_locals.items():
                 exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
                     exceptNotifier["BODY"] += str(val)
                 except:
                     exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
 
         try:
             error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
             advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
             )
             advice_msg += receive_openai_advice(
                 os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
             )  # NO-QA
-            send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+            send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], advice_msg)
         except Exception as e:
             print(e)
             pass
 
     @staticmethod
-    def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
-        """Send message to chat room through microsoft teams app's webhook url.
+    def send_slack_msg(_SLACK_WEBHOOK_URL: str, msg: str) -> dict:
+        """Send message to chat room through slack app's api.
 
-        :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
-        :type _TEAMS_WEBHOOK_URL: str
+        :param _SLACK_WEBHOOK_URL: _SLACK_WEBHOOK_URL from slack app
+        :type _SLACK_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
 
-        payload = {"text": msg}
-        headers = {"Content-Type": "application/json"}
-        resp = requests.post(
-            _TEAMS_WEBHOOK_URL, headers=headers, data=json.dumps(payload)
-        )
-
+        data = {"text": msg}
+        resp = requests.post(url=_SLACK_WEBHOOK_URL, json=data["text"])
         return resp
 
 
-class SuccessTeams:
+class SuccessSlack:
+    """Sending success message to Slack
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
-            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+            "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
 
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
-
-class SendTeams:
+class SendSlack:
+    """Sending message to Slack
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
         exceptNotifier = {
-            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+            "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
         }
         exceptNotifier[
             "BODY"
-        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
-
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
+        send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
 
 
 # if __name__ == "__main__":
-
-#     """Follow next page"""
-
-
-#     _TEAMS_WEBHOOK_URL = "microsoft webhook _TEAMS_WEBHOOK_URL"
-
-#     sys.excepthook = ExceptTeams.__call__
-
+#     # Get your slack bot and enter _SLACK_WEBHOOK_URL
+#     """Get your _SLACK_WEBHOOK_URL from HERE.
+# #     os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+# #     os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
+#     https://api.slack.com/messaging/webhooks#create_a_webhook"""
+#     os.environ['_SLACK_WEBHOOK_URL'] ='xxxxxxx'
+#     sys.excepthook = ExceptSlack.__call__
 #     try:
-#         print(1 / 20)
-#         SuccessTeams().__call__()  # 1 success sender
-
-#     except ExceptTeams as e:  # 2 except sender
+#         print(1 / 0)
+#         SuccessSlack().__call__()  # 1 success sender
+#     except ExceptSlack as e:  # 2 except sender
 #         sys.exit()
-
-#     SendTeams().__call__()  # 3 customized sender
+#     SendSlack().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/python/telegram_notifier.py` & `exceptnotifier-0.2.1/ExceptNotifier/python/telegram_notifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 import sys
 from ExceptNotifier import send_telegram_msg, receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptTelegram(BaseException):
+    """Override excepthook to send error message to Telegram.
+
+    :param etype: Error Type
+    :type etype: _type_
+    :param value: Error Value
+    :type value: _type_
+    :param tb: Traceback Information
+    :type tb: _type_
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Telegram.
 
-        :param etype: Error Type
-        :type etype: _type_
-        :param value: Error Value
-        :type value: _type_
-        :param tb: Traceback Information
-        :type tb: _type_
-        """
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
         start_time = datetime.datetime.now()
 
         exceptNotifier = {
             "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
@@ -104,14 +105,16 @@
         bot_url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/sendMessage?chat_id={bot_id}&text={msg}"
         resp = requests.get(bot_url).json()
 
         return resp
 
 
 class SuccessTelegram:
+    """Sending success message to telegram
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -124,14 +127,16 @@
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 class SendTelegram:
+    """Sending message to telegram
+    """
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -144,28 +149,21 @@
 
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
         send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 # if __name__ == "__main__":
-
 #     """Get your bot from botfather.
 #     https://core.telegram.org/bots/tutorial"""
-
-
 #     os.environ['_TELEGRAM_TOKEN'] = "xxxxxxxxx"
-#     # _OPEN_AI_MODEL = "gpt-3.5-turbo"
-#     # _OPEN_AI_API = "sk-xxxxxxxxx"
+#     # os.environ['_OPEN_AI_API'] = "xxxxxxxxxxxxx"  #optional
+#     # os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo" #optional
 #     sys.excepthook = ExceptTelegram.__call__
-
 #     try:
 #         print(1 / 0)
 #         SuccessTelegram().__call__()  # 1 success sender
-
 #     except ExceptTelegram as e:  # 2 except sender
 #         sys.exit()
-
 #     SendTelegram().__call__()  # 3 customized sender
-
 #     send = SendTelegram()  # You can use it like this, too.
 #     send()
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.2.1/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.2.1/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.0
+Version: 0.2.1
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,33 +20,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Development Status :: 2 - Pre-Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
 Before QA<br> 
 
-![](./assets/imgs/logo2.png)
+![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
-<a href="(https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
+<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ![](./assets/imgs/main3.png)
 ##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
+![](./assets/imgs/core02.png)
+
 <Br>
 
 
 # Supporting Applications
 Applicable to both [IPython](https://ipython.org/) and [Python](https://www.python.org/), but needs to be ported differently only in `ExceptNotifier`. Please refer to the detailed example. (`SuccessNotifier` and `SendNotifier` have the same syntax.)
 - [Telegram](https://telegram.org/)
 - [Discord](https://discord.com/)
@@ -76,25 +79,31 @@
 
 <br><br><br>
 
 # Contents
 
 - [App Setup Overview](#app-setup-overview)
 - [Tutorial](#tutorial)
+<Br>
+
 - [Python Core](#python-core)
   * [Except`Notifier`](#exceptnotifier)
     + [AI Debbugging Infomation Notification](#ai-debbugging-infomation-notification)
   * [Success`Notifier`](#successnotifier)
   * [Send`Notifier`](#sendnotifier)
   * [Sender](#sender)
+<br>
+
 - [IPython Core](#ipython-core)
   * [Except`Notifier` in Ipython](#exceptnotifier-in-ipython)
   * [Success`Notifier` in Ipython](#successnotifier-in-ipython)
   * [Send`Notifier` in Ipython](#sendnotifier-in-ipython)
   * [Sender in Ipython](#sender-in-ipython)
+<br>
+
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
@@ -157,15 +166,15 @@
 <Br>
 
 # Python Core
 To use the desired application, you must define the necessary variables. Ensure that the variable names remain unchanged, and you can use either local or global variables. If you are using `Telegram`, an example is attached as an image.
 
 
 ## Except`Notifier`
-![](./assets/imgs/ex1.png)
+![](./assets/imgs/ex01.png)
 If you use Python's try except statement as it is, but change except as follows, you can receive notifications through your application.
 - Format: Except`[appName]` <Br>
 - Type: class
 *ExampleClass*
 ```
 ExceptChime, ExceptTelegram, ExceptDiscord, ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams, ExceptDesktope, ExceptBeep
 ```
@@ -182,15 +191,15 @@
     print(1/0)
 except ExceptTelegram:    # sending except message to telegram
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
-![](./assets/imgs/ex2.png)
+![](./assets/imgs/ex02.png)
 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
@@ -205,15 +214,15 @@
     print(1/0)
 except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
     sys.exit()
 ```
 
 
 ## Success`Notifier`
-![](./assets/imgs/ex3.png)
+![](./assets/imgs/ex03.png)
 
 - Format: Success`[appName]`
 - Type: Class <br>
 *ExampleClass* <br>
 By placing the try except in python at the end of the try statement, applications can be notified that the try statement worked normally.
 ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail, SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope, SuccessBeep
@@ -230,15 +239,15 @@
     print(1/20)
     SuccessTelgeram().__call__()  # sending success message to telegram
 except:
     sys.exit()
 ```
 
 ## Send`Notifier`
-![](./assets/imgs/ex4.png)
+![](./assets/imgs/ex04.png)
 - Format: Send`[appName]` 
 - Type: class <br>
 *ExampleClass* <br>
 Place it anywhere on the line of code you want, and you'll be notified when that line of code is reached.
 ```
 SendChime, SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack, SendTeams, SendDesktope, SendBeep
 ```
@@ -254,15 +263,15 @@
 
 noti = SendTelegram()
 noti()                    # sending message to telegram
 ```
 
 
 ## Sender
-![](./assets/imgs/ex5.png)
+![](./assets/imgs/ex05.png)
 It is recommended to conduct a simple message sending test through the `sender`. Assuming that you can communicate with REST API or WEBHOOK normally, `ExceptNotifier` can work normally.
 - Every application's ExceptNotifier uses the sender method.
 - Format: send_`[appName]`_msg 
 - Type: Function <br>
 *Example* <br>
 ```
 send_chime_msg, send_telegram_msg, send_discord_msg, send_sms_msg, send_gmail_msg, send_kakao_msg, send_line_msg, send_slack_msg, send_teams_msg, send_desktop_msg, beep
@@ -284,15 +293,15 @@
 ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier.
 - Format: Except[appName]
 - Type: function <br>
 
 *Example code without Open AI API*
 
-![](./assets/imgs/ipyex1.png)
+![](./assets/imgs/ex06.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
@@ -300,15 +309,15 @@
   print(1/0)
 except:
   raise
 ```
 
 *Example code With Open AI API*
 
-![](./assets/imgs/ipyex2.png)
+![](./assets/imgs/ex07.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
 os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"    
@@ -318,15 +327,15 @@
 try:
   print(1/0)
 except:
   raise
 ```
 
 ## Success`Notifier` in Ipython
-![](./assets/imgs/ipyex3.png)
+![](./assets/imgs/ex08.png)
 - Same syntax in Python. See Python Core above.
 ```python
 import sys
 import os
 from ExceptNotifier import SuccessTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 
@@ -336,29 +345,29 @@
 except:
   raise
 ```
 
 
 ## Send`Notifier` in Ipython
 
-![](./assets/imgs/ipyex4.png)
+![](./assets/imgs/ex09.png)
 
 - Same syntax in Python. See Python Core above.
 ```python
 import sys
 import os
 from ExceptNotifier import SendTelegram 
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 
 SendTelegram().__call__()         # Sending telegram message
 ```
 
 ## Sender in Ipython
 
-![](./assets/imgs/ipyex5.png)
+![](./assets/imgs/ex10.png)
 
 - Same syntax in Python. See Python Core above.
 ```python
 from ExceptNotifier import send_telegram_msg
 
 _TELEGRAM_TOKEN =  "xxxxx"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.0 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.1 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -11,30 +11,33 @@
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Development Status :: 2 - Pre-Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 Before QA
-![](./assets/imgs/logo2.png)
+![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-                     [PyPI] [Downloads] [Code_style:_black]
+             [PyPI package] [PyPI] [Downloads] [Code_style:_black]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
-shown in the captured screen. # Python Package: ExceptNotifier The
-`ExceptNotifier` Python package offers a flexible approach to receiving
-notifications by enhancing Python's try-except statement. This package enables
-you to receive alerts through various messaging applications or emails.
+shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
+/hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
+(https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
+flexible approach to receiving notifications by enhancing Python's try-except
+statement. This package enables you to receive alerts through various messaging
+applications or emails.
 
 With `ExceptNotifier`, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
-accessible, streamlining your debugging process.
+accessible, streamlining your debugging process. ![](./assets/imgs/core02.png)
 # Supporting Applications Applicable to both [IPython](https://ipython.org/
 ) and [Python](https://www.python.org/), but needs to be ported differently
 only in `ExceptNotifier`. Please refer to the detailed example.
 (`SuccessNotifier` and `SendNotifier` have the same syntax.) - [Telegram]
 (https://telegram.org/) - [Discord](https://discord.com/) - [Slack](https://
 slack.com/) - [Google Mail](https://mail.google.com/) - [Line](https://line.me/
 en/) - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/) -
@@ -50,26 +53,27 @@
 exceptnotifier ```
 
 
 # Contents - [App Setup Overview](#app-setup-overview) - [Tutorial](#tutorial)
 - [Python Core](#python-core) * [Except`Notifier`](#exceptnotifier) + [AI
 Debbugging Infomation Notification](#ai-debbugging-infomation-notification) *
 [Success`Notifier`](#successnotifier) * [Send`Notifier`](#sendnotifier) *
-[Sender](#sender) - [IPython Core](#ipython-core) * [Except`Notifier` in
-Ipython](#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython]
-(#successnotifier-in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-
-ipython) * [Sender in Ipython](#sender-in-ipython) - [Applied in each
-application](#applied-in-each-application) * [*Telegram*](#telegram) + [a.
-Notifier without OpenAI API](#a-notifier-without-openai-api) + [b. Notifier
-with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail) * [*Discord*]
-(#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line) * [*SMS*]
-(#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*](#wechat) *
-[*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide](#contributing-
-guide) - [License](#license) - [Code of Conduct](#code-of-conduct) - [Contacts]
-(#contacts)
+[Sender](#sender)
+- [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
+(#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
+in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
+in Ipython](#sender-in-ipython)
+- [Applied in each application](#applied-in-each-application) * [*Telegram*]
+(#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
++ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail)
+* [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*]
+(#line) * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) *
+[*Wechat*](#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing
+Guide](#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
+conduct) - [Contacts](#contacts)
 
 
 
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - As you already know, API Keys or security tokens must be
 secured. Note that the key values which exposured in github will be expired
@@ -124,54 +128,55 @@
 The tutorial is synchronized with the Python file name provided by
 ExceptNotifier. **In this example, some API keys were exposed by creating and
 removing a test application, but for security reasons, your API key should not
 be exposed to the outside world.**
 # Python Core To use the desired application, you must define the necessary
 variables. Ensure that the variable names remain unchanged, and you can use
 either local or global variables. If you are using `Telegram`, an example is
-attached as an image. ## Except`Notifier` ![](./assets/imgs/ex1.png) If you use
-Python's try except statement as it is, but change except as follows, you can
-receive notifications through your application. - Format: Except`[appName]`
+attached as an image. ## Except`Notifier` ![](./assets/imgs/ex01.png) If you
+use Python's try except statement as it is, but change except as follows, you
+can receive notifications through your application. - Format: Except`[appName]`
+
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex2.png) You can receive debugging information
+Notification ![](./assets/imgs/ex02.png) You can receive debugging information
 from ChatGPT via OpenAI's API when using the Except statement. The syntax
 remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
 ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
-Success`Notifier` ![](./assets/imgs/ex3.png) - Format: Success`[appName]` -
+Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
 Type: Class
 *ExampleClass*
 By placing the try except in python at the end of the try statement,
 applications can be notified that the try statement worked normally. ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail,
 SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope,
 SuccessBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SuccessTelgeram sys.excepthook = ExceptTelegram.__call__ os.environ
 ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/20) SuccessTelgeram().__call__() #
 sending success message to telegram except: sys.exit() ``` ## Send`Notifier` !
-[](./assets/imgs/ex4.png) - Format: Send`[appName]` - Type: class
+[](./assets/imgs/ex04.png) - Format: Send`[appName]` - Type: class
 *ExampleClass*
 Place it anywhere on the line of code you want, and you'll be notified when
 that line of code is reached. ``` SendChime, SendTelegram, SendDiscord,
 SendSMS, SendMail, SendKakao, SendLine, SendSlack, SendTeams, SendDesktope,
 SendBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SendTelegram sys.excepthook = ExceptTelegram.__call__ os.environ
 ['_TELEGRAM_TOKEN'] = "xxxx" SendTelegram().__call__() # sending message to
 telegram noti = SendTelegram() noti() # sending message to telegram ``` ##
-Sender ![](./assets/imgs/ex5.png) It is recommended to conduct a simple message
-sending test through the `sender`. Assuming that you can communicate with REST
-API or WEBHOOK normally, `ExceptNotifier` can work normally. - Every
+Sender ![](./assets/imgs/ex05.png) It is recommended to conduct a simple
+message sending test through the `sender`. Assuming that you can communicate
+with REST API or WEBHOOK normally, `ExceptNotifier` can work normally. - Every
 application's ExceptNotifier uses the sender method. - Format: send_`
 [appName]`_msg - Type: Function
 *Example*
 ``` send_chime_msg, send_telegram_msg, send_discord_msg, send_sms_msg,
 send_gmail_msg, send_kakao_msg, send_line_msg, send_slack_msg, send_teams_msg,
 send_desktop_msg, beep ``` *Example* ```python from ExceptNotifier import
 send_telegram_msg send_telegram_msg(_TELEGRAM_TOKEN, "Any Test Message") ```
@@ -181,31 +186,31 @@
 `SendNotifier`, and `Sender` functions can all be used same in IPython without
 any special processing. Only `ExceptNotifier` is need to be defined. - Example
 in Telegram [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier. - Format: Except[appName] -
 Type: function
-*Example code without Open AI API* ![](./assets/imgs/ipyex1.png) ```python from
+*Example code without Open AI API* ![](./assets/imgs/ex06.png) ```python from
 ExceptNotifier import ExceptTelegramIpython import os os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) try: print(1/0) except: raise ``` *Example code With
-Open AI API* ![](./assets/imgs/ipyex2.png) ```python from ExceptNotifier import
+Open AI API* ![](./assets/imgs/ex07.png) ```python from ExceptNotifier import
 ExceptTelegramIpython import os get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"
 os.environ['_OPEN_AI_API'] = "sk-xxxxx" os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 try: print(1/0) except: raise ``` ## Success`Notifier` in Ipython ![](./assets/
-imgs/ipyex3.png) - Same syntax in Python. See Python Core above. ```python
-import sys import os from ExceptNotifier import SuccessTelegram os.environ
+imgs/ex08.png) - Same syntax in Python. See Python Core above. ```python import
+sys import os from ExceptNotifier import SuccessTelegram os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" try: print(1/20) # Your Code Here SuccessTelegram
 ().__call__() # Sending Success message except: raise ``` ## Send`Notifier` in
-Ipython ![](./assets/imgs/ipyex4.png) - Same syntax in Python. See Python Core
+Ipython ![](./assets/imgs/ex09.png) - Same syntax in Python. See Python Core
 above. ```python import sys import os from ExceptNotifier import SendTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx" SendTelegram().__call__() # Sending
-telegram message ``` ## Sender in Ipython ![](./assets/imgs/ipyex5.png) - Same
+telegram message ``` ## Sender in Ipython ![](./assets/imgs/ex10.png) - Same
 syntax in Python. See Python Core above. ```python from ExceptNotifier import
 send_telegram_msg _TELEGRAM_TOKEN = "xxxxx" send_telegram_msg(_TELEGRAM_TOKEN,
 "This is test message") ```
 # Applied in each application You can receive debugging information from
 ChatGPT via OpenAI's API when using the Except statement. The syntax remains
 the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
```

### Comparing `exceptnotifier-0.2.0/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.2.1/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/LICENSE` & `exceptnotifier-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.0/PKG-INFO` & `exceptnotifier-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.0
+Version: 0.2.1
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -20,33 +20,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Development Status :: 2 - Pre-Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
 Before QA<br> 
 
-![](./assets/imgs/logo2.png)
+![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
-<a href="(https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
+<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ![](./assets/imgs/main3.png)
 ##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
+![](./assets/imgs/core02.png)
+
 <Br>
 
 
 # Supporting Applications
 Applicable to both [IPython](https://ipython.org/) and [Python](https://www.python.org/), but needs to be ported differently only in `ExceptNotifier`. Please refer to the detailed example. (`SuccessNotifier` and `SendNotifier` have the same syntax.)
 - [Telegram](https://telegram.org/)
 - [Discord](https://discord.com/)
@@ -76,25 +79,31 @@
 
 <br><br><br>
 
 # Contents
 
 - [App Setup Overview](#app-setup-overview)
 - [Tutorial](#tutorial)
+<Br>
+
 - [Python Core](#python-core)
   * [Except`Notifier`](#exceptnotifier)
     + [AI Debbugging Infomation Notification](#ai-debbugging-infomation-notification)
   * [Success`Notifier`](#successnotifier)
   * [Send`Notifier`](#sendnotifier)
   * [Sender](#sender)
+<br>
+
 - [IPython Core](#ipython-core)
   * [Except`Notifier` in Ipython](#exceptnotifier-in-ipython)
   * [Success`Notifier` in Ipython](#successnotifier-in-ipython)
   * [Send`Notifier` in Ipython](#sendnotifier-in-ipython)
   * [Sender in Ipython](#sender-in-ipython)
+<br>
+
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
@@ -157,15 +166,15 @@
 <Br>
 
 # Python Core
 To use the desired application, you must define the necessary variables. Ensure that the variable names remain unchanged, and you can use either local or global variables. If you are using `Telegram`, an example is attached as an image.
 
 
 ## Except`Notifier`
-![](./assets/imgs/ex1.png)
+![](./assets/imgs/ex01.png)
 If you use Python's try except statement as it is, but change except as follows, you can receive notifications through your application.
 - Format: Except`[appName]` <Br>
 - Type: class
 *ExampleClass*
 ```
 ExceptChime, ExceptTelegram, ExceptDiscord, ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams, ExceptDesktope, ExceptBeep
 ```
@@ -182,15 +191,15 @@
     print(1/0)
 except ExceptTelegram:    # sending except message to telegram
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
-![](./assets/imgs/ex2.png)
+![](./assets/imgs/ex02.png)
 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
@@ -205,15 +214,15 @@
     print(1/0)
 except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
     sys.exit()
 ```
 
 
 ## Success`Notifier`
-![](./assets/imgs/ex3.png)
+![](./assets/imgs/ex03.png)
 
 - Format: Success`[appName]`
 - Type: Class <br>
 *ExampleClass* <br>
 By placing the try except in python at the end of the try statement, applications can be notified that the try statement worked normally.
 ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail, SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope, SuccessBeep
@@ -230,15 +239,15 @@
     print(1/20)
     SuccessTelgeram().__call__()  # sending success message to telegram
 except:
     sys.exit()
 ```
 
 ## Send`Notifier`
-![](./assets/imgs/ex4.png)
+![](./assets/imgs/ex04.png)
 - Format: Send`[appName]` 
 - Type: class <br>
 *ExampleClass* <br>
 Place it anywhere on the line of code you want, and you'll be notified when that line of code is reached.
 ```
 SendChime, SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack, SendTeams, SendDesktope, SendBeep
 ```
@@ -254,15 +263,15 @@
 
 noti = SendTelegram()
 noti()                    # sending message to telegram
 ```
 
 
 ## Sender
-![](./assets/imgs/ex5.png)
+![](./assets/imgs/ex05.png)
 It is recommended to conduct a simple message sending test through the `sender`. Assuming that you can communicate with REST API or WEBHOOK normally, `ExceptNotifier` can work normally.
 - Every application's ExceptNotifier uses the sender method.
 - Format: send_`[appName]`_msg 
 - Type: Function <br>
 *Example* <br>
 ```
 send_chime_msg, send_telegram_msg, send_discord_msg, send_sms_msg, send_gmail_msg, send_kakao_msg, send_line_msg, send_slack_msg, send_teams_msg, send_desktop_msg, beep
@@ -284,15 +293,15 @@
 ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier.
 - Format: Except[appName]
 - Type: function <br>
 
 *Example code without Open AI API*
 
-![](./assets/imgs/ipyex1.png)
+![](./assets/imgs/ex06.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
@@ -300,15 +309,15 @@
   print(1/0)
 except:
   raise
 ```
 
 *Example code With Open AI API*
 
-![](./assets/imgs/ipyex2.png)
+![](./assets/imgs/ex07.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
 os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"    
@@ -318,15 +327,15 @@
 try:
   print(1/0)
 except:
   raise
 ```
 
 ## Success`Notifier` in Ipython
-![](./assets/imgs/ipyex3.png)
+![](./assets/imgs/ex08.png)
 - Same syntax in Python. See Python Core above.
 ```python
 import sys
 import os
 from ExceptNotifier import SuccessTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 
@@ -336,29 +345,29 @@
 except:
   raise
 ```
 
 
 ## Send`Notifier` in Ipython
 
-![](./assets/imgs/ipyex4.png)
+![](./assets/imgs/ex09.png)
 
 - Same syntax in Python. See Python Core above.
 ```python
 import sys
 import os
 from ExceptNotifier import SendTelegram 
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 
 SendTelegram().__call__()         # Sending telegram message
 ```
 
 ## Sender in Ipython
 
-![](./assets/imgs/ipyex5.png)
+![](./assets/imgs/ex10.png)
 
 - Same syntax in Python. See Python Core above.
 ```python
 from ExceptNotifier import send_telegram_msg
 
 _TELEGRAM_TOKEN =  "xxxxx"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.0 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.1 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -11,30 +11,33 @@
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Development Status :: 2 - Pre-Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 Before QA
-![](./assets/imgs/logo2.png)
+![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-                     [PyPI] [Downloads] [Code_style:_black]
+             [PyPI package] [PyPI] [Downloads] [Code_style:_black]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
-shown in the captured screen. # Python Package: ExceptNotifier The
-`ExceptNotifier` Python package offers a flexible approach to receiving
-notifications by enhancing Python's try-except statement. This package enables
-you to receive alerts through various messaging applications or emails.
+shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
+/hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
+(https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
+flexible approach to receiving notifications by enhancing Python's try-except
+statement. This package enables you to receive alerts through various messaging
+applications or emails.
 
 With `ExceptNotifier`, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
-accessible, streamlining your debugging process.
+accessible, streamlining your debugging process. ![](./assets/imgs/core02.png)
 # Supporting Applications Applicable to both [IPython](https://ipython.org/
 ) and [Python](https://www.python.org/), but needs to be ported differently
 only in `ExceptNotifier`. Please refer to the detailed example.
 (`SuccessNotifier` and `SendNotifier` have the same syntax.) - [Telegram]
 (https://telegram.org/) - [Discord](https://discord.com/) - [Slack](https://
 slack.com/) - [Google Mail](https://mail.google.com/) - [Line](https://line.me/
 en/) - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/) -
@@ -50,26 +53,27 @@
 exceptnotifier ```
 
 
 # Contents - [App Setup Overview](#app-setup-overview) - [Tutorial](#tutorial)
 - [Python Core](#python-core) * [Except`Notifier`](#exceptnotifier) + [AI
 Debbugging Infomation Notification](#ai-debbugging-infomation-notification) *
 [Success`Notifier`](#successnotifier) * [Send`Notifier`](#sendnotifier) *
-[Sender](#sender) - [IPython Core](#ipython-core) * [Except`Notifier` in
-Ipython](#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython]
-(#successnotifier-in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-
-ipython) * [Sender in Ipython](#sender-in-ipython) - [Applied in each
-application](#applied-in-each-application) * [*Telegram*](#telegram) + [a.
-Notifier without OpenAI API](#a-notifier-without-openai-api) + [b. Notifier
-with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail) * [*Discord*]
-(#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line) * [*SMS*]
-(#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*](#wechat) *
-[*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide](#contributing-
-guide) - [License](#license) - [Code of Conduct](#code-of-conduct) - [Contacts]
-(#contacts)
+[Sender](#sender)
+- [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
+(#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
+in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
+in Ipython](#sender-in-ipython)
+- [Applied in each application](#applied-in-each-application) * [*Telegram*]
+(#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
++ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail)
+* [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*]
+(#line) * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) *
+[*Wechat*](#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing
+Guide](#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
+conduct) - [Contacts](#contacts)
 
 
 
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - As you already know, API Keys or security tokens must be
 secured. Note that the key values which exposured in github will be expired
@@ -124,54 +128,55 @@
 The tutorial is synchronized with the Python file name provided by
 ExceptNotifier. **In this example, some API keys were exposed by creating and
 removing a test application, but for security reasons, your API key should not
 be exposed to the outside world.**
 # Python Core To use the desired application, you must define the necessary
 variables. Ensure that the variable names remain unchanged, and you can use
 either local or global variables. If you are using `Telegram`, an example is
-attached as an image. ## Except`Notifier` ![](./assets/imgs/ex1.png) If you use
-Python's try except statement as it is, but change except as follows, you can
-receive notifications through your application. - Format: Except`[appName]`
+attached as an image. ## Except`Notifier` ![](./assets/imgs/ex01.png) If you
+use Python's try except statement as it is, but change except as follows, you
+can receive notifications through your application. - Format: Except`[appName]`
+
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex2.png) You can receive debugging information
+Notification ![](./assets/imgs/ex02.png) You can receive debugging information
 from ChatGPT via OpenAI's API when using the Except statement. The syntax
 remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
 ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
-Success`Notifier` ![](./assets/imgs/ex3.png) - Format: Success`[appName]` -
+Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
 Type: Class
 *ExampleClass*
 By placing the try except in python at the end of the try statement,
 applications can be notified that the try statement worked normally. ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail,
 SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope,
 SuccessBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SuccessTelgeram sys.excepthook = ExceptTelegram.__call__ os.environ
 ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/20) SuccessTelgeram().__call__() #
 sending success message to telegram except: sys.exit() ``` ## Send`Notifier` !
-[](./assets/imgs/ex4.png) - Format: Send`[appName]` - Type: class
+[](./assets/imgs/ex04.png) - Format: Send`[appName]` - Type: class
 *ExampleClass*
 Place it anywhere on the line of code you want, and you'll be notified when
 that line of code is reached. ``` SendChime, SendTelegram, SendDiscord,
 SendSMS, SendMail, SendKakao, SendLine, SendSlack, SendTeams, SendDesktope,
 SendBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SendTelegram sys.excepthook = ExceptTelegram.__call__ os.environ
 ['_TELEGRAM_TOKEN'] = "xxxx" SendTelegram().__call__() # sending message to
 telegram noti = SendTelegram() noti() # sending message to telegram ``` ##
-Sender ![](./assets/imgs/ex5.png) It is recommended to conduct a simple message
-sending test through the `sender`. Assuming that you can communicate with REST
-API or WEBHOOK normally, `ExceptNotifier` can work normally. - Every
+Sender ![](./assets/imgs/ex05.png) It is recommended to conduct a simple
+message sending test through the `sender`. Assuming that you can communicate
+with REST API or WEBHOOK normally, `ExceptNotifier` can work normally. - Every
 application's ExceptNotifier uses the sender method. - Format: send_`
 [appName]`_msg - Type: Function
 *Example*
 ``` send_chime_msg, send_telegram_msg, send_discord_msg, send_sms_msg,
 send_gmail_msg, send_kakao_msg, send_line_msg, send_slack_msg, send_teams_msg,
 send_desktop_msg, beep ``` *Example* ```python from ExceptNotifier import
 send_telegram_msg send_telegram_msg(_TELEGRAM_TOKEN, "Any Test Message") ```
@@ -181,31 +186,31 @@
 `SendNotifier`, and `Sender` functions can all be used same in IPython without
 any special processing. Only `ExceptNotifier` is need to be defined. - Example
 in Telegram [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier. - Format: Except[appName] -
 Type: function
-*Example code without Open AI API* ![](./assets/imgs/ipyex1.png) ```python from
+*Example code without Open AI API* ![](./assets/imgs/ex06.png) ```python from
 ExceptNotifier import ExceptTelegramIpython import os os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) try: print(1/0) except: raise ``` *Example code With
-Open AI API* ![](./assets/imgs/ipyex2.png) ```python from ExceptNotifier import
+Open AI API* ![](./assets/imgs/ex07.png) ```python from ExceptNotifier import
 ExceptTelegramIpython import os get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"
 os.environ['_OPEN_AI_API'] = "sk-xxxxx" os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 try: print(1/0) except: raise ``` ## Success`Notifier` in Ipython ![](./assets/
-imgs/ipyex3.png) - Same syntax in Python. See Python Core above. ```python
-import sys import os from ExceptNotifier import SuccessTelegram os.environ
+imgs/ex08.png) - Same syntax in Python. See Python Core above. ```python import
+sys import os from ExceptNotifier import SuccessTelegram os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" try: print(1/20) # Your Code Here SuccessTelegram
 ().__call__() # Sending Success message except: raise ``` ## Send`Notifier` in
-Ipython ![](./assets/imgs/ipyex4.png) - Same syntax in Python. See Python Core
+Ipython ![](./assets/imgs/ex09.png) - Same syntax in Python. See Python Core
 above. ```python import sys import os from ExceptNotifier import SendTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx" SendTelegram().__call__() # Sending
-telegram message ``` ## Sender in Ipython ![](./assets/imgs/ipyex5.png) - Same
+telegram message ``` ## Sender in Ipython ![](./assets/imgs/ex10.png) - Same
 syntax in Python. See Python Core above. ```python from ExceptNotifier import
 send_telegram_msg _TELEGRAM_TOKEN = "xxxxx" send_telegram_msg(_TELEGRAM_TOKEN,
 "This is test message") ```
 # Applied in each application You can receive debugging information from
 ChatGPT via OpenAI's API when using the Except statement. The syntax remains
 the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
```

### Comparing `exceptnotifier-0.2.0/README.md` & `exceptnotifier-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Development Status :: 2 - Pre-Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*<br>
 Before QA<br> 
 
-![](./assets/imgs/logo2.png)
+![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
 
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
-<a href="(https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
+<a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ![](./assets/imgs/main3.png)
 ##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
+![](./assets/imgs/core02.png)
+
 <Br>
 
 
 # Supporting Applications
 Applicable to both [IPython](https://ipython.org/) and [Python](https://www.python.org/), but needs to be ported differently only in `ExceptNotifier`. Please refer to the detailed example. (`SuccessNotifier` and `SendNotifier` have the same syntax.)
 - [Telegram](https://telegram.org/)
 - [Discord](https://discord.com/)
@@ -54,25 +57,31 @@
 
 <br><br><br>
 
 # Contents
 
 - [App Setup Overview](#app-setup-overview)
 - [Tutorial](#tutorial)
+<Br>
+
 - [Python Core](#python-core)
   * [Except`Notifier`](#exceptnotifier)
     + [AI Debbugging Infomation Notification](#ai-debbugging-infomation-notification)
   * [Success`Notifier`](#successnotifier)
   * [Send`Notifier`](#sendnotifier)
   * [Sender](#sender)
+<br>
+
 - [IPython Core](#ipython-core)
   * [Except`Notifier` in Ipython](#exceptnotifier-in-ipython)
   * [Success`Notifier` in Ipython](#successnotifier-in-ipython)
   * [Send`Notifier` in Ipython](#sendnotifier-in-ipython)
   * [Sender in Ipython](#sender-in-ipython)
+<br>
+
 - [Applied in each application](#applied-in-each-application)
   * [*Telegram*](#telegram)
     + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
     + [b. Notifier with OpenAI API](#b-notifier-with-openai-api)
   * [*Mail*](#mail)
   * [*Discord*](#discord)
   * [*Chime*](#chime)
@@ -135,15 +144,15 @@
 <Br>
 
 # Python Core
 To use the desired application, you must define the necessary variables. Ensure that the variable names remain unchanged, and you can use either local or global variables. If you are using `Telegram`, an example is attached as an image.
 
 
 ## Except`Notifier`
-![](./assets/imgs/ex1.png)
+![](./assets/imgs/ex01.png)
 If you use Python's try except statement as it is, but change except as follows, you can receive notifications through your application.
 - Format: Except`[appName]` <Br>
 - Type: class
 *ExampleClass*
 ```
 ExceptChime, ExceptTelegram, ExceptDiscord, ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams, ExceptDesktope, ExceptBeep
 ```
@@ -160,15 +169,15 @@
     print(1/0)
 except ExceptTelegram:    # sending except message to telegram
     sys.exit()
 ```
 
 
 ### AI Debbugging Infomation Notification
-![](./assets/imgs/ex2.png)
+![](./assets/imgs/ex02.png)
 
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 *Example*
 ```python
 import sys, os
@@ -183,15 +192,15 @@
     print(1/0)
 except ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram
     sys.exit()
 ```
 
 
 ## Success`Notifier`
-![](./assets/imgs/ex3.png)
+![](./assets/imgs/ex03.png)
 
 - Format: Success`[appName]`
 - Type: Class <br>
 *ExampleClass* <br>
 By placing the try except in python at the end of the try statement, applications can be notified that the try statement worked normally.
 ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail, SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope, SuccessBeep
@@ -208,15 +217,15 @@
     print(1/20)
     SuccessTelgeram().__call__()  # sending success message to telegram
 except:
     sys.exit()
 ```
 
 ## Send`Notifier`
-![](./assets/imgs/ex4.png)
+![](./assets/imgs/ex04.png)
 - Format: Send`[appName]` 
 - Type: class <br>
 *ExampleClass* <br>
 Place it anywhere on the line of code you want, and you'll be notified when that line of code is reached.
 ```
 SendChime, SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack, SendTeams, SendDesktope, SendBeep
 ```
@@ -232,15 +241,15 @@
 
 noti = SendTelegram()
 noti()                    # sending message to telegram
 ```
 
 
 ## Sender
-![](./assets/imgs/ex5.png)
+![](./assets/imgs/ex05.png)
 It is recommended to conduct a simple message sending test through the `sender`. Assuming that you can communicate with REST API or WEBHOOK normally, `ExceptNotifier` can work normally.
 - Every application's ExceptNotifier uses the sender method.
 - Format: send_`[appName]`_msg 
 - Type: Function <br>
 *Example* <br>
 ```
 send_chime_msg, send_telegram_msg, send_discord_msg, send_sms_msg, send_gmail_msg, send_kakao_msg, send_line_msg, send_slack_msg, send_teams_msg, send_desktop_msg, beep
@@ -262,15 +271,15 @@
 ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier.
 - Format: Except[appName]
 - Type: function <br>
 
 *Example code without Open AI API*
 
-![](./assets/imgs/ipyex1.png)
+![](./assets/imgs/ex06.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
@@ -278,15 +287,15 @@
   print(1/0)
 except:
   raise
 ```
 
 *Example code With Open AI API*
 
-![](./assets/imgs/ipyex2.png)
+![](./assets/imgs/ex07.png)
 
 ```python
 from ExceptNotifier import ExceptTelegramIpython
 import os
 get_ipython().set_custom_exc((Exception,), ExceptTelegramIpython)
 
 os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"    
@@ -296,15 +305,15 @@
 try:
   print(1/0)
 except:
   raise
 ```
 
 ## Success`Notifier` in Ipython
-![](./assets/imgs/ipyex3.png)
+![](./assets/imgs/ex08.png)
 - Same syntax in Python. See Python Core above.
 ```python
 import sys
 import os
 from ExceptNotifier import SuccessTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 
@@ -314,29 +323,29 @@
 except:
   raise
 ```
 
 
 ## Send`Notifier` in Ipython
 
-![](./assets/imgs/ipyex4.png)
+![](./assets/imgs/ex09.png)
 
 - Same syntax in Python. See Python Core above.
 ```python
 import sys
 import os
 from ExceptNotifier import SendTelegram 
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 
 SendTelegram().__call__()         # Sending telegram message
 ```
 
 ## Sender in Ipython
 
-![](./assets/imgs/ipyex5.png)
+![](./assets/imgs/ex10.png)
 
 - Same syntax in Python. See Python Core above.
 ```python
 from ExceptNotifier import send_telegram_msg
 
 _TELEGRAM_TOKEN =  "xxxxx"
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
 Development Status :: 2 - Pre-Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 Before QA
-![](./assets/imgs/logo2.png)
+![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-                     [PyPI] [Downloads] [Code_style:_black]
+             [PyPI package] [PyPI] [Downloads] [Code_style:_black]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
-shown in the captured screen. # Python Package: ExceptNotifier The
-`ExceptNotifier` Python package offers a flexible approach to receiving
-notifications by enhancing Python's try-except statement. This package enables
-you to receive alerts through various messaging applications or emails.
+shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
+/hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
+(https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
+flexible approach to receiving notifications by enhancing Python's try-except
+statement. This package enables you to receive alerts through various messaging
+applications or emails.
 
 With `ExceptNotifier`, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
-accessible, streamlining your debugging process.
+accessible, streamlining your debugging process. ![](./assets/imgs/core02.png)
 # Supporting Applications Applicable to both [IPython](https://ipython.org/
 ) and [Python](https://www.python.org/), but needs to be ported differently
 only in `ExceptNotifier`. Please refer to the detailed example.
 (`SuccessNotifier` and `SendNotifier` have the same syntax.) - [Telegram]
 (https://telegram.org/) - [Discord](https://discord.com/) - [Slack](https://
 slack.com/) - [Google Mail](https://mail.google.com/) - [Line](https://line.me/
 en/) - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/) -
@@ -36,26 +39,27 @@
 exceptnotifier ```
 
 
 # Contents - [App Setup Overview](#app-setup-overview) - [Tutorial](#tutorial)
 - [Python Core](#python-core) * [Except`Notifier`](#exceptnotifier) + [AI
 Debbugging Infomation Notification](#ai-debbugging-infomation-notification) *
 [Success`Notifier`](#successnotifier) * [Send`Notifier`](#sendnotifier) *
-[Sender](#sender) - [IPython Core](#ipython-core) * [Except`Notifier` in
-Ipython](#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython]
-(#successnotifier-in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-
-ipython) * [Sender in Ipython](#sender-in-ipython) - [Applied in each
-application](#applied-in-each-application) * [*Telegram*](#telegram) + [a.
-Notifier without OpenAI API](#a-notifier-without-openai-api) + [b. Notifier
-with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail) * [*Discord*]
-(#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*](#line) * [*SMS*]
-(#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) * [*Wechat*](#wechat) *
-[*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing Guide](#contributing-
-guide) - [License](#license) - [Code of Conduct](#code-of-conduct) - [Contacts]
-(#contacts)
+[Sender](#sender)
+- [IPython Core](#ipython-core) * [Except`Notifier` in Ipython]
+(#exceptnotifier-in-ipython) * [Success`Notifier` in Ipython](#successnotifier-
+in-ipython) * [Send`Notifier` in Ipython](#sendnotifier-in-ipython) * [Sender
+in Ipython](#sender-in-ipython)
+- [Applied in each application](#applied-in-each-application) * [*Telegram*]
+(#telegram) + [a. Notifier without OpenAI API](#a-notifier-without-openai-api)
++ [b. Notifier with OpenAI API](#b-notifier-with-openai-api) * [*Mail*](#mail)
+* [*Discord*](#discord) * [*Chime*](#chime) * [*Slack*](#slack) * [*Line*]
+(#line) * [*SMS*](#sms) * [*Teams*](#teams) * [*Kakaotalk*](#kakaotalk) *
+[*Wechat*](#wechat) * [*Beep*](#beep) * [*Desktop*](#desktop) - [Contributing
+Guide](#contributing-guide) - [License](#license) - [Code of Conduct](#code-of-
+conduct) - [Contacts](#contacts)
 
 
 
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - As you already know, API Keys or security tokens must be
 secured. Note that the key values which exposured in github will be expired
@@ -110,54 +114,55 @@
 The tutorial is synchronized with the Python file name provided by
 ExceptNotifier. **In this example, some API keys were exposed by creating and
 removing a test application, but for security reasons, your API key should not
 be exposed to the outside world.**
 # Python Core To use the desired application, you must define the necessary
 variables. Ensure that the variable names remain unchanged, and you can use
 either local or global variables. If you are using `Telegram`, an example is
-attached as an image. ## Except`Notifier` ![](./assets/imgs/ex1.png) If you use
-Python's try except statement as it is, but change except as follows, you can
-receive notifications through your application. - Format: Except`[appName]`
+attached as an image. ## Except`Notifier` ![](./assets/imgs/ex01.png) If you
+use Python's try except statement as it is, but change except as follows, you
+can receive notifications through your application. - Format: Except`[appName]`
+
 - Type: class *ExampleClass* ``` ExceptChime, ExceptTelegram, ExceptDiscord,
 ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams,
 ExceptDesktope, ExceptBeep ``` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.environ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/0) except ExceptTelegram: #
 sending except message to telegram sys.exit() ``` ### AI Debbugging Infomation
-Notification ![](./assets/imgs/ex2.png) You can receive debugging information
+Notification ![](./assets/imgs/ex02.png) You can receive debugging information
 from ChatGPT via OpenAI's API when using the Except statement. The syntax
 remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API` *Example* ```python import sys, os from
 ExceptNotifier import ExceptTelegram sys.excepthook = ExceptTelegram.__call__
 os.envirion['_TELEGRAM_TOKEN'] = "xxxx" os.envirion['_OPEN_AI_MODEL']="gpt-3.5-
 turbo" os.envirion['_OPEN_AI_API']="sk-xxxxxx" try: print(1/0) except
 ExceptTelegram: # sending msg WITH AI DEBUGGING to telegram sys.exit() ``` ##
-Success`Notifier` ![](./assets/imgs/ex3.png) - Format: Success`[appName]` -
+Success`Notifier` ![](./assets/imgs/ex03.png) - Format: Success`[appName]` -
 Type: Class
 *ExampleClass*
 By placing the try except in python at the end of the try statement,
 applications can be notified that the try statement worked normally. ```
 SuccessChime, SuccessTelegram, SuccessDiscord, SuccessSMS, SuccessMail,
 SuccessKakao, SuccessLine, SuccessSlack, SuccessTeams, SuccessDesktope,
 SuccessBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SuccessTelgeram sys.excepthook = ExceptTelegram.__call__ os.environ
 ['_TELEGRAM_TOKEN'] = "xxxx" try: print(1/20) SuccessTelgeram().__call__() #
 sending success message to telegram except: sys.exit() ``` ## Send`Notifier` !
-[](./assets/imgs/ex4.png) - Format: Send`[appName]` - Type: class
+[](./assets/imgs/ex04.png) - Format: Send`[appName]` - Type: class
 *ExampleClass*
 Place it anywhere on the line of code you want, and you'll be notified when
 that line of code is reached. ``` SendChime, SendTelegram, SendDiscord,
 SendSMS, SendMail, SendKakao, SendLine, SendSlack, SendTeams, SendDesktope,
 SendBeep ``` *Example* ```python import sys, os from ExceptNotifier import
 SendTelegram sys.excepthook = ExceptTelegram.__call__ os.environ
 ['_TELEGRAM_TOKEN'] = "xxxx" SendTelegram().__call__() # sending message to
 telegram noti = SendTelegram() noti() # sending message to telegram ``` ##
-Sender ![](./assets/imgs/ex5.png) It is recommended to conduct a simple message
-sending test through the `sender`. Assuming that you can communicate with REST
-API or WEBHOOK normally, `ExceptNotifier` can work normally. - Every
+Sender ![](./assets/imgs/ex05.png) It is recommended to conduct a simple
+message sending test through the `sender`. Assuming that you can communicate
+with REST API or WEBHOOK normally, `ExceptNotifier` can work normally. - Every
 application's ExceptNotifier uses the sender method. - Format: send_`
 [appName]`_msg - Type: Function
 *Example*
 ``` send_chime_msg, send_telegram_msg, send_discord_msg, send_sms_msg,
 send_gmail_msg, send_kakao_msg, send_line_msg, send_slack_msg, send_teams_msg,
 send_desktop_msg, beep ``` *Example* ```python from ExceptNotifier import
 send_telegram_msg send_telegram_msg(_TELEGRAM_TOKEN, "Any Test Message") ```
@@ -167,31 +172,31 @@
 `SendNotifier`, and `Sender` functions can all be used same in IPython without
 any special processing. Only `ExceptNotifier` is need to be defined. - Example
 in Telegram [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1jwWGs7eCUJQvj_g7SEMqm3a4Kdrp9ZQP?usp=sharing) ## Except`Notifier` in Ipython
 You have to use `raise` in Ipython ExceptNotifier. - Format: Except[appName] -
 Type: function
-*Example code without Open AI API* ![](./assets/imgs/ipyex1.png) ```python from
+*Example code without Open AI API* ![](./assets/imgs/ex06.png) ```python from
 ExceptNotifier import ExceptTelegramIpython import os os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) try: print(1/0) except: raise ``` *Example code With
-Open AI API* ![](./assets/imgs/ipyex2.png) ```python from ExceptNotifier import
+Open AI API* ![](./assets/imgs/ex07.png) ```python from ExceptNotifier import
 ExceptTelegramIpython import os get_ipython().set_custom_exc((Exception,),
 ExceptTelegramIpython) os.environ['_OPEN_AI_MODEL'] = "gpt-3.5-turbo"
 os.environ['_OPEN_AI_API'] = "sk-xxxxx" os.environ['_TELEGRAM_TOKEN'] = "xxxxx"
 try: print(1/0) except: raise ``` ## Success`Notifier` in Ipython ![](./assets/
-imgs/ipyex3.png) - Same syntax in Python. See Python Core above. ```python
-import sys import os from ExceptNotifier import SuccessTelegram os.environ
+imgs/ex08.png) - Same syntax in Python. See Python Core above. ```python import
+sys import os from ExceptNotifier import SuccessTelegram os.environ
 ['_TELEGRAM_TOKEN'] = "xxxxx" try: print(1/20) # Your Code Here SuccessTelegram
 ().__call__() # Sending Success message except: raise ``` ## Send`Notifier` in
-Ipython ![](./assets/imgs/ipyex4.png) - Same syntax in Python. See Python Core
+Ipython ![](./assets/imgs/ex09.png) - Same syntax in Python. See Python Core
 above. ```python import sys import os from ExceptNotifier import SendTelegram
 os.environ['_TELEGRAM_TOKEN'] = "xxxxx" SendTelegram().__call__() # Sending
-telegram message ``` ## Sender in Ipython ![](./assets/imgs/ipyex5.png) - Same
+telegram message ``` ## Sender in Ipython ![](./assets/imgs/ex10.png) - Same
 syntax in Python. See Python Core above. ```python from ExceptNotifier import
 send_telegram_msg _TELEGRAM_TOKEN = "xxxxx" send_telegram_msg(_TELEGRAM_TOKEN,
 "This is test message") ```
 # Applied in each application You can receive debugging information from
 ChatGPT via OpenAI's API when using the Except statement. The syntax remains
 the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
```

### Comparing `exceptnotifier-0.2.0/setup.py` & `exceptnotifier-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.2.0",
+    version="0.2.1",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=["twilio", "plyer", "openai", "discord"],
+    install_requires=["twilio", "plyer", "openai", "discord", "sphinx-rtd-theme", "Sphinx"],
     keywords="Exception, Python, Python Exception Alarm, Error notifications, Customizable notifications, Traceback management, Single line alarm",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```

