# Comparing `tmp/exceptnotifier-0.2.1.tar.gz` & `tmp/exceptnotifier-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.2.1.tar", last modified: Mon Apr 24 08:17:47 2023, max compression
+gzip compressed data, was "exceptnotifier-0.2.2.tar", last modified: Mon Apr 24 12:17:09 2023, max compression
```

## Comparing `exceptnotifier-0.2.1.tar` & `exceptnotifier-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.972786 exceptnotifier-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.826871 exceptnotifier-0.2.1/ExceptNotifier/
--rw-rw-rw-   0        0        0     4663 2023-04-24 08:16:39.000000 exceptnotifier-0.2.1/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.890412 exceptnotifier-0.2.1/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1382 2023-04-24 08:16:46.000000 exceptnotifier-0.2.1/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      532 2023-04-20 06:16:28.000000 exceptnotifier-0.2.1/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.1/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0     1002 2023-04-23 07:06:21.000000 exceptnotifier-0.2.1/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.1/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.1/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.1/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.1/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.1/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.1/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      930 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      582 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1470 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/base/whatsapp_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.924670 exceptnotifier-0.2.1/ExceptNotifier/ipython/
--rw-rw-rw-   0        0        0     1472 2023-04-24 08:16:42.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/__init__.py
--rw-rw-rw-   0        0        0      565 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/beep_notifier_ipython.py
--rw-rw-rw-   0        0        0     1808 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/chime_notifier_ipython.py
--rw-rw-rw-   0        0        0     2189 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/desktop_notifier_ipython.py
--rw-rw-rw-   0        0        0     1820 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/discord_notifier_ipython.py
--rw-rw-rw-   0        0        0     1807 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/kakao_notifier_ipython.py
--rw-rw-rw-   0        0        0     1813 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/line_notifier_ipython.py
--rw-rw-rw-   0        0        0     2579 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/mail_notifier_ipython.py
--rw-rw-rw-   0        0        0     1807 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/slack_notifier_ipython.py
--rw-rw-rw-   0        0        0     2096 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/sms_notifier_ipython.py
--rw-rw-rw-   0        0        0     1811 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/teams_notifier_ipython.py
--rw-rw-rw-   0        0        0     1721 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/telegram_notifier_ipython.py
--rw-rw-rw-   0        0        0     1815 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/ipython/wechat_notifier_ipython.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.957266 exceptnotifier-0.2.1/ExceptNotifier/python/
--rw-rw-rw-   0        0        0     1955 2023-04-24 08:16:48.000000 exceptnotifier-0.2.1/ExceptNotifier/python/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/beep_notifier.py
--rw-rw-rw-   0        0        0     6722 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/chime_notifier.py
--rw-rw-rw-   0        0        0     6177 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/desktop_notifier.py
--rw-rw-rw-   0        0        0     7029 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/discord_notifier.py
--rw-rw-rw-   0        0        0     7108 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/kakao_notifier.py
--rw-rw-rw-   0        0        0     6634 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/line_notifier.py
--rw-rw-rw-   0        0        0     8807 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/mail_notifier.py
--rw-rw-rw-   0        0        0     6645 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/slack_notifier.py
--rw-rw-rw-   0        0        0     7879 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/sms_notifier.py
--rw-rw-rw-   0        0        0     6610 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/teams_notifier.py
--rw-rw-rw-   0        0        0     6834 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/telegram_notifier.py
--rw-rw-rw-   0        0        0     6625 2023-04-23 15:01:26.000000 exceptnotifier-0.2.1/ExceptNotifier/python/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.966265 exceptnotifier-0.2.1/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      265 2023-04-24 08:16:52.000000 exceptnotifier-0.2.1/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.1/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:17:47.855873 exceptnotifier-0.2.1/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    33926 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-24 08:17:47.000000 exceptnotifier-0.2.1/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    33926 2023-04-24 08:17:47.971790 exceptnotifier-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    32878 2023-04-23 13:32:03.000000 exceptnotifier-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 08:17:47.972786 exceptnotifier-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1958 2023-04-24 08:16:31.000000 exceptnotifier-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.560119 exceptnotifier-0.2.2/
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.408519 exceptnotifier-0.2.2/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4748 2023-04-24 12:16:22.000000 exceptnotifier-0.2.2/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.476055 exceptnotifier-0.2.2/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1382 2023-04-24 12:16:24.000000 exceptnotifier-0.2.2/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-04-24 11:00:44.000000 exceptnotifier-0.2.2/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      792 2023-04-23 07:06:13.000000 exceptnotifier-0.2.2/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-23 15:01:26.000000 exceptnotifier-0.2.2/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1009 2023-04-24 12:13:54.000000 exceptnotifier-0.2.2/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 exceptnotifier-0.2.2/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 exceptnotifier-0.2.2/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-04-23 07:06:32.000000 exceptnotifier-0.2.2/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     2321 2023-04-23 10:27:50.000000 exceptnotifier-0.2.2/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 exceptnotifier-0.2.2/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 exceptnotifier-0.2.2/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 exceptnotifier-0.2.2/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      928 2023-04-24 11:00:12.000000 exceptnotifier-0.2.2/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 exceptnotifier-0.2.2/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 exceptnotifier-0.2.2/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.508670 exceptnotifier-0.2.2/ExceptNotifier/ipycore/
+-rw-rw-rw-   0        0        0     1472 2023-04-24 12:16:28.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2020 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2422 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2030 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2017 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2025 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2740 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2021 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2298 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2025 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2027 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2031 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/ipycore/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.544580 exceptnotifier-0.2.2/ExceptNotifier/pycore/
+-rw-rw-rw-   0        0        0     2009 2023-04-24 12:16:30.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/__init__.py
+-rw-rw-rw-   0        0        0     1988 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/beep_notifier.py
+-rw-rw-rw-   0        0        0     6782 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/chime_notifier.py
+-rw-rw-rw-   0        0        0     6267 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/desktop_notifier.py
+-rw-rw-rw-   0        0        0     7093 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/discord_notifier.py
+-rw-rw-rw-   0        0        0     7168 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/kakao_notifier.py
+-rw-rw-rw-   0        0        0     6711 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/line_notifier.py
+-rw-rw-rw-   0        0        0     8862 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/mail_notifier.py
+-rw-rw-rw-   0        0        0     6689 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/slack_notifier.py
+-rw-rw-rw-   0        0        0     7926 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/sms_notifier.py
+-rw-rw-rw-   0        0        0     6670 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/teams_notifier.py
+-rw-rw-rw-   0        0        0     6897 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/telegram_notifier.py
+-rw-rw-rw-   0        0        0     6686 2023-04-24 11:11:19.000000 exceptnotifier-0.2.2/ExceptNotifier/pycore/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.553586 exceptnotifier-0.2.2/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      265 2023-04-24 12:16:33.000000 exceptnotifier-0.2.2/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.2.2/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:17:09.438800 exceptnotifier-0.2.2/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    34136 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-24 12:17:09.000000 exceptnotifier-0.2.2/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    34136 2023-04-24 12:17:09.559121 exceptnotifier-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    33088 2023-04-24 10:05:15.000000 exceptnotifier-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:17:09.560119 exceptnotifier-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-04-24 12:15:45.000000 exceptnotifier-0.2.2/setup.py
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/__init__.py` & `exceptnotifier-0.2.2/ExceptNotifier/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,38 +12,54 @@
 from ExceptNotifier.base.whatsapp_sender import send_whatsapp_msg
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.beep_sender import beep
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 from ExceptNotifier.base.openai_receiver import get_resp_openai_advice
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 from ExceptNotifier.base.desktop_sender import send_desktop_msg
-from ExceptNotifier.python.mail_notifier import SuccessMail, ExceptMail, SendMail
-from ExceptNotifier.python.slack_notifier import SuccessSlack, ExceptSlack, SendSlack
-from ExceptNotifier.python.telegram_notifier import SuccessTelegram, ExceptTelegram, SendTelegram
-from ExceptNotifier.python.chime_notifier import SuccessChime, ExceptChime, SendChime
-from ExceptNotifier.python.discord_notifier import SuccessDiscord, ExceptDiscord, SendDiscord
-from ExceptNotifier.python.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
-from ExceptNotifier.python.line_notifier import SuccessLine, ExceptLine, SendLine
-from ExceptNotifier.python.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
-from ExceptNotifier.python.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
-from ExceptNotifier.python.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
-from ExceptNotifier.python.wechat_notifier import SuccessWechat,ExceptWechat, SendWechat
-from ExceptNotifier.python.desktop_notifier import SuccessDesktop, ExceptDesktop, SendDesktop
-from ExceptNotifier.ipython.telegram_notifier_ipython import ExceptTelegramIpython
-from ExceptNotifier.ipython.chime_notifier_ipython import ExceptChimeIpython
-from ExceptNotifier.ipython.discord_notifier_ipython import ExceptDiscordIpython
-from ExceptNotifier.ipython.kakao_notifier_ipython import ExceptKakaoIpython
-from ExceptNotifier.ipython.line_notifier_ipython import ExceptLineIpython
-from ExceptNotifier.ipython.mail_notifier_ipython import ExceptMailIpython
-from ExceptNotifier.ipython.slack_notifier_ipython import ExceptSlackIpython
-from ExceptNotifier.ipython.sms_notifier_ipython import ExceptSMSIpython
-from ExceptNotifier.ipython.teams_notifier_ipython import ExceptTeamsIpython
-from ExceptNotifier.ipython.wechat_notifier_ipython import ExceptWechatIpython
-from ExceptNotifier.ipython.beep_notifier_ipython import ExceptBeepIpython
-from ExceptNotifier.ipython.desktop_notifier_ipython import ExceptDesktopIpython
+from ExceptNotifier.pycore.mail_notifier import SuccessMail, ExceptMail, SendMail
+from ExceptNotifier.pycore.slack_notifier import SuccessSlack, ExceptSlack, SendSlack
+from ExceptNotifier.pycore.telegram_notifier import (
+    SuccessTelegram,
+    ExceptTelegram,
+    SendTelegram,
+)
+from ExceptNotifier.pycore.chime_notifier import SuccessChime, ExceptChime, SendChime
+from ExceptNotifier.pycore.discord_notifier import (
+    SuccessDiscord,
+    ExceptDiscord,
+    SendDiscord,
+)
+from ExceptNotifier.pycore.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
+from ExceptNotifier.pycore.line_notifier import SuccessLine, ExceptLine, SendLine
+from ExceptNotifier.pycore.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
+from ExceptNotifier.pycore.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
+from ExceptNotifier.pycore.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
+from ExceptNotifier.pycore.wechat_notifier import (
+    SuccessWechat,
+    ExceptWechat,
+    SendWechat,
+)
+from ExceptNotifier.pycore.desktop_notifier import (
+    SuccessDesktop,
+    ExceptDesktop,
+    SendDesktop,
+)
+from ExceptNotifier.ipycore.telegram_notifier_ipython import ExceptTelegramIpython
+from ExceptNotifier.ipycore.chime_notifier_ipython import ExceptChimeIpython
+from ExceptNotifier.ipycore.discord_notifier_ipython import ExceptDiscordIpython
+from ExceptNotifier.ipycore.kakao_notifier_ipython import ExceptKakaoIpython
+from ExceptNotifier.ipycore.line_notifier_ipython import ExceptLineIpython
+from ExceptNotifier.ipycore.mail_notifier_ipython import ExceptMailIpython
+from ExceptNotifier.ipycore.slack_notifier_ipython import ExceptSlackIpython
+from ExceptNotifier.ipycore.sms_notifier_ipython import ExceptSMSIpython
+from ExceptNotifier.ipycore.teams_notifier_ipython import ExceptTeamsIpython
+from ExceptNotifier.ipycore.wechat_notifier_ipython import ExceptWechatIpython
+from ExceptNotifier.ipycore.beep_notifier_ipython import ExceptBeepIpython
+from ExceptNotifier.ipycore.desktop_notifier_ipython import ExceptDesktopIpython
 
 __all__ = [
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
     "get_resp_openai_advice",
     "SuccessMail",
     "ExceptMail",
@@ -107,9 +123,9 @@
     "ExceptMailIpython",
     "ExceptSlackIpython",
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     "send_whatsapp_msg",
     "send_sms_msg",
     "beep",
     "receive_openai_advice",
     "get_resp_openai_advice",
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/beep_sender.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 import platform
 
 
 def beep(sec=1, freq=1000) -> None:
     """Make beep sound
 
-    :param sec: beep duration, defaults to 1
+    :param sec: Beep duration, defaults to 1
     :type sec: int, optional
-    :param freq: beep fequency, defaults to 1000
+    :param freq: Beep fequency, defaults to 1000
     :type freq: int, optional
     """
 
     sys = platform.system()
 
     if sys == "Windows":
         import winsound
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/discord_sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             _DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter()
         )
         resp = webhook.send(msg)
     except:
         from discord import SyncWebhook
 
         webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL)  # Initializing webhook
-        resp = webhook.send(content=msg)
+        resp = webhook.send(content=msg[:1900])
     return resp
 
 
 # if __name__ == "__main__":
 #     _DISCORD_WEBHOOK_URL = "xxxxx"
 #     msg = "Sending Test"
 #     send_discord_msg(_DISCORD_WEBHOOK_URL, msg)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/telegram_sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-
 import requests
 
 
 def send_telegram_msg(_TELEGRAM_TOKEN: str, msg: str) -> dict:
     """Send message via telegram bot.
 
     :param _TELEGRAM_TOKEN: Telegram secure bot Token
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/wechat_sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-
 import requests
 
 
 def send_wechat_msg(_WECHAT_WEBHOOK_URL: str, msg: str) -> None:
     """Send message to wechat.
 
     :param _WECHAT_WEBHOOK_URL: Wechat Webhook URL https://work.weixin.qq.com/api/doc/90000/90136/91770
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.2.2/ExceptNotifier/base/whatsapp_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import logging
 import requests
 
 
 def send_whatsapp_msg(
     msg: str,
     sender_phone_number_id: str,
     TOKEN: str,
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/__init__.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright 2023 parkminwoo
-from ExceptNotifier.ipython.telegram_notifier_ipython import ExceptTelegramIpython
-from ExceptNotifier.ipython.chime_notifier_ipython import ExceptChimeIpython
-from ExceptNotifier.ipython.discord_notifier_ipython import ExceptDiscordIpython
-from ExceptNotifier.ipython.kakao_notifier_ipython import ExceptKakaoIpython
-from ExceptNotifier.ipython.line_notifier_ipython import ExceptLineIpython
-from ExceptNotifier.ipython.mail_notifier_ipython import ExceptMailIpython
-from ExceptNotifier.ipython.slack_notifier_ipython import ExceptSlackIpython
-from ExceptNotifier.ipython.sms_notifier_ipython import ExceptSMSIpython
-from ExceptNotifier.ipython.teams_notifier_ipython import ExceptTeamsIpython
-from ExceptNotifier.ipython.wechat_notifier_ipython import ExceptWechatIpython
-from ExceptNotifier.ipython.beep_notifier_ipython import ExceptBeepIpython
-from ExceptNotifier.ipython.desktop_notifier_ipython import ExceptDesktopIpython
-from ExceptNotifier.ipython.beep_notifier_ipython import ExceptBeepIpython
+from ExceptNotifier.ipycore.telegram_notifier_ipython import ExceptTelegramIpython
+from ExceptNotifier.ipycore.chime_notifier_ipython import ExceptChimeIpython
+from ExceptNotifier.ipycore.discord_notifier_ipython import ExceptDiscordIpython
+from ExceptNotifier.ipycore.kakao_notifier_ipython import ExceptKakaoIpython
+from ExceptNotifier.ipycore.line_notifier_ipython import ExceptLineIpython
+from ExceptNotifier.ipycore.mail_notifier_ipython import ExceptMailIpython
+from ExceptNotifier.ipycore.slack_notifier_ipython import ExceptSlackIpython
+from ExceptNotifier.ipycore.sms_notifier_ipython import ExceptSMSIpython
+from ExceptNotifier.ipycore.teams_notifier_ipython import ExceptTeamsIpython
+from ExceptNotifier.ipycore.wechat_notifier_ipython import ExceptWechatIpython
+from ExceptNotifier.ipycore.beep_notifier_ipython import ExceptBeepIpython
+from ExceptNotifier.ipycore.desktop_notifier_ipython import ExceptDesktopIpython
+from ExceptNotifier.ipycore.beep_notifier_ipython import ExceptBeepIpython
 
 __all__ = [
     "ExceptTelegramIpython",
     "ExceptChimeIpython",
     "ExceptDiscordIpython",
     "ExceptKakaoIpython",
     "ExceptLineIpython",
@@ -24,9 +24,9 @@
     "ExceptSMSIpython",
     "ExceptTeamsIpython",
     "ExceptWechatIpython",
     "ExceptBeepIpython",
     "ExceptDesktopIpython",
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/chime_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/chime_notifier_ipython.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_chime_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.chime_sender import send_chime_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptChimeIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptChimeIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Chime message.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/desktop_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/desktop_notifier_ipython.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_desktop_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.desktop_sender import send_desktop_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptDesktopIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptDesktopIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Desktop notification via plyer.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/discord_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/discord_notifier_ipython.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_discord_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.discord_sender import send_discord_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptDiscordIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptDiscordIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Discord.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/kakao_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/kakao_notifier_ipython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_kakao_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.kakao_sender import send_kakao_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptKakaoIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptKakaoIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Kakaotalk.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/line_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/line_notifier_ipython.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_line_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.line_sender import send_line_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptLineIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptLineIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Line message.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/mail_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/mail_notifier_ipython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
+import os
 import datetime
 import smtplib
 import datetime
-from ExceptNotifier import receive_openai_advice
-import os
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptMailIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptMailIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Gmail.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     SMTP_SERVER = "smtp.gmail.com"
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/slack_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/slack_notifier_ipython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_slack_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.slack_sender import send_slack_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptSlackIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptSlackIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending slack message.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/sms_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/sms_notifier_ipython.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_sms_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.sms_sender import send_sms_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptSMSIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptSMSIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending SMS.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/teams_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/telegram_notifier_ipython.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_teams_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.telegram_sender import send_telegram_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptTeamsIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptTelegramIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Telegram.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
-
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
+    send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
         advice_msg = receive_openai_advice(
             os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
         )
-        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
+        send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], advice_msg)
 
     except Exception as e:
         print(e)
         pass
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/telegram_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/wechat_notifier_ipython.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,49 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_telegram_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.wechat_sender import send_wechat_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptTelegramIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptWechatIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending Wechat message.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
+    :param tb_offset: Offset of traceback, defaults to 1
+    :type tb_offset: int, optional
     """
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
+    send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
         advice_msg = receive_openai_advice(
             os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
         )
-        send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], advice_msg)
+        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
         pass
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/ipython/wechat_notifier_ipython.py` & `exceptnotifier-0.2.2/ExceptNotifier/ipycore/teams_notifier_ipython.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,50 @@
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-from IPython.core.ultratb import AutoFormattedTB
-from ExceptNotifier import send_wechat_msg, receive_openai_advice
 import os
 import datetime
+from IPython.core.ultratb import AutoFormattedTB
+from ExceptNotifier.base.teams_sender import send_teams_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-def ExceptWechatIpython(shell, etype, evalue, tb, tb_offset=1):
-    """ExceptNotifier function for overriding custom execute in ipython
+def ExceptTeamsIpython(
+    shell: object, etype: object, evalue: object, tb: object, tb_offset=1
+) -> None:
+    """ExceptNotifier function for overriding custom execute in ipython for sending teams message.
 
-    :param shell: Excecuted shell 
-    :type shell: _type_
+    :param shell: Excecuted shell, ZMQInteractiveShell object.
+    :type shell: object
     :param etype: Error type
-    :type etype: _type_
+    :type etype: object
     :param evalue: Error value
-    :type evalue: _type_
-    :param tb: TraceBack
-    :type tb: _type_
+    :type evalue: object
+    :param tb: TraceBack object of Ipython
+    :type tb: object
     :param tb_offset: Offset of traceback, defaults to 1
     :type tb_offset: int, optional
     """
+
     itb = AutoFormattedTB(mode="Plain", tb_offset=1)
     shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
     stb = itb.structured_traceback(etype, evalue, tb)
     sstb = itb.stb2text(stb)
     start_time = datetime.datetime.now()
     data = {
         "text": f"[Except Notifier] ⚠️ Error! Python Code Exception Detected \n \n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {sstb}"
     }
 
-    send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
+    send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
     try:
         error_message = f"error sheel=={shell}, error_type_document=={etype.__doc__}, error_value=={evalue}, error message in ipython cell=={sstb}"
         advice_msg = receive_openai_advice(
             os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
         )
-        send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], advice_msg)
+        send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], advice_msg)
 
     except Exception as e:
         print(e)
         pass
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/__init__.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from ExceptNotifier.python.mail_notifier import SuccessMail, ExceptMail, SendMail
-from ExceptNotifier.python.slack_notifier import SuccessSlack, ExceptSlack, SendSlack
-from ExceptNotifier.python.telegram_notifier import (
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
+from ExceptNotifier.pycore.mail_notifier import SuccessMail, ExceptMail, SendMail
+from ExceptNotifier.pycore.slack_notifier import SuccessSlack, ExceptSlack, SendSlack
+from ExceptNotifier.pycore.telegram_notifier import (
     SuccessTelegram,
     ExceptTelegram,
     SendTelegram,
 )
-from ExceptNotifier.python.chime_notifier import SuccessChime, ExceptChime, SendChime
-from ExceptNotifier.python.discord_notifier import (
+from ExceptNotifier.pycore.chime_notifier import SuccessChime, ExceptChime, SendChime
+from ExceptNotifier.pycore.discord_notifier import (
     SuccessDiscord,
     ExceptDiscord,
     SendDiscord,
 )
-from ExceptNotifier.python.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
-from ExceptNotifier.python.line_notifier import SuccessLine, ExceptLine, SendLine
-from ExceptNotifier.python.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
-from ExceptNotifier.python.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
-from ExceptNotifier.python.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
-from ExceptNotifier.python.wechat_notifier import (
+from ExceptNotifier.pycore.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
+from ExceptNotifier.pycore.line_notifier import SuccessLine, ExceptLine, SendLine
+from ExceptNotifier.pycore.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
+from ExceptNotifier.pycore.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
+from ExceptNotifier.pycore.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
+from ExceptNotifier.pycore.wechat_notifier import (
     SuccessWechat,
     ExceptWechat,
     SendWechat,
 )
-from ExceptNotifier.python.desktop_notifier import (
+from ExceptNotifier.pycore.desktop_notifier import (
     SuccessDesktop,
     ExceptDesktop,
     SendDesktop,
 )
 
 __all__ = [
     "SuccessMail",
@@ -62,9 +64,9 @@
     "ExceptWechat",
     "SendWechat",
     "SuccessDesktop",
     "ExceptDesktop",
     "SendDesktop",
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/beep_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/beep_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import sys
 import os
 import platform
 from ExceptNotifier import beep
 
 
 class ExceptBeep(BaseException):
     """Override excepthook to send error message to beep.
@@ -12,20 +11,20 @@
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
 
-
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
 
     @staticmethod
@@ -47,25 +46,27 @@
         else:
             os.system("play -nq -t alsa synth {} sine {}".format(sec, freq))
 
 
 class SuccessBeep:
     """Success beep
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         beep(os.environ["BEEP_TIME"])
         beep(os.environ["BEEP_TIME"])
 
 
 class SendBeep:
     """Send beep
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         beep(os.environ["BEEP_TIME"])
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/chime_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/chime_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import traceback
 import re
+import os
+import json
+import urllib3
 import datetime
+import traceback
 from email.message import EmailMessage
-import sys
-import urllib3
-import json
-from ExceptNotifier import receive_openai_advice, send_chime_msg
-import os
+from ExceptNotifier.base.chime_sender import send_chime_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptChime(BaseException):
     """Override excepthook to send error message to AWS Chime.
@@ -20,14 +20,15 @@
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -108,14 +109,15 @@
 
         return resp
 
 
 class SuccessChime:
     """Sending success message to AWS Chime
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -130,14 +132,15 @@
 
         send_chime_msg(os.environ["_CHIME_WEBHOOK_URL"], data["text"])
 
 
 class SendChime:
     """Sending message to AWS Chime
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/desktop_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/desktop_notifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import re
-import sys
+import os
 import datetime
 import traceback
 from plyer import notification
 from email.message import EmailMessage
-from ExceptNotifier import send_desktop_msg, receive_openai_advice
-import os
+from ExceptNotifier.base.desktop_sender import send_desktop_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptDesktop(BaseException):
     """Override excepthook to send error message to Desktop.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -78,15 +79,15 @@
             advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
                 line[0],
                 line[2],
                 line[1],
                 line[3],
             )
             advice_msg += receive_openai_advice(
-                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+                os.environ["_OPEN_AI_MODEL"], os.environ["_OPEN_AI_API"], error_message
             )  # NO-QA
             send_desktop_msg(
                 title="chatGPT: How to Debug your code.", message=advice_msg
             )
         except Exception as e:
             print(e)
             pass
@@ -104,14 +105,15 @@
         """
         notification.notify(title=title_msg, message=body_msg, timeout=DISP_TIME)
 
 
 class SuccessDesktop:
     """Sending success message to Desktop
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -126,14 +128,15 @@
             title=exceptNotifier["SUBJECT"][:20], message=exceptNotifier["BODY"][:200]
         )
 
 
 class SendDesktop:
     """Sending message to Desktop
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/discord_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/discord_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import traceback
 import re
+import os
 import datetime
+import traceback
 from email.message import EmailMessage
-import sys
-from ExceptNotifier import send_discord_msg, receive_openai_advice
-import os
+from ExceptNotifier.base.discord_sender import send_discord_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptDiscord(BaseException):
     """Override excepthook to send error message to Discord.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
 
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
@@ -112,14 +114,15 @@
             resp = webhook.send(content=msg)
         return resp
 
 
 class SuccessDiscord:
     """Sending success message to Discord
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -133,14 +136,15 @@
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_discord_msg(os.environ["_DISCORD_WEBHOOK_URL"], data["text"][:2000])
 
 
 class SendDiscord:
     """Sending message to Discord
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/kakao_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/kakao_notifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import requests
-import traceback
 import re
+import os
+import json
 import datetime
+import requests
+import traceback
 from email.message import EmailMessage
-import sys
-import json
-import os
-from ExceptNotifier import send_kakao_msg, receive_openai_advice
+from ExceptNotifier.base.kakao_sender import send_kakao_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptKakao(BaseException):
     """Override excepthook to send error message to Kakaotalk.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -120,14 +121,15 @@
 
         return resp
 
 
 class SuccessKakao:
     """Sending success message to Kakaotalk
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -142,14 +144,15 @@
 
         send_kakao_msg(os.environ["_KAKAO_TOKEN_PATH"], data["text"])
 
 
 class SendKakao:
     """Sending message to Kakaotalk
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/line_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/line_notifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# Copyright 2023 parkminwoo Authors.
-import requests
-import traceback
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import re
+import os
 import datetime
+import requests
+import traceback
 from email.message import EmailMessage
-import sys
-from ExceptNotifier import send_line_msg, receive_openai_advice
-import os
+from ExceptNotifier.base.line_sender import send_line_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptLine(BaseException):
     """Override excepthook to send error message to Line.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -104,14 +107,15 @@
         resp = requests.post(api_url, headers=headers, data=message)
         return resp
 
 
 class SuccessLine:
     """Sending success message to Line
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -126,14 +130,15 @@
 
         send_line_msg(os.environ["_LINE_NOTIFY_API_TOKEN"], data["text"])
 
 
 class SendLine:
     """Sending success message to Line
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/mail_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/mail_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-import sys
-import traceback
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import re
+import os
 import smtplib
 import datetime
+import traceback
 from email.message import EmailMessage
-from ExceptNotifier import send_gmail_msg, receive_openai_advice
-import os
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptMail(BaseException):
     """Override excepthook to send error message to Gmail.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
 
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
@@ -150,14 +153,15 @@
 
         return resp
 
 
 class SuccessMail:
     """Sending success message to Gmail
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
@@ -181,14 +185,15 @@
         smtp.send_message(message)
         smtp.quit()
 
 
 class SendMail:
     """Sending message to Gmail
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/slack_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/slack_notifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import requests
-import traceback
 import re
+import os
 import datetime
+import requests
+import traceback
 from email.message import EmailMessage
-import sys
-import os
-from ExceptNotifier import send_slack_msg, receive_openai_advice
+from ExceptNotifier import send_slack_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptSlack(BaseException):
     """Override excepthook to send error message to Slack.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
 
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
@@ -103,14 +105,15 @@
         resp = requests.post(url=_SLACK_WEBHOOK_URL, json=data["text"])
         return resp
 
 
 class SuccessSlack:
     """Sending success message to Slack
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -124,14 +127,15 @@
         data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_slack_msg(os.environ["_SLACK_WEBHOOK_URL"], data["text"])
 
 
 class SendSlack:
     """Sending message to Slack
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/sms_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/sms_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import traceback
+
 import re
+import os
 import datetime
-from email.message import EmailMessage
-import sys
-import pickle
+import traceback
 from twilio.rest import Client
-import os
-from ExceptNotifier import send_sms_msg, receive_openai_advice
+from email.message import EmailMessage
+from ExceptNotifier.base.sms_sender import send_sms_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptSMS(BaseException):
     """Override excepthook to send error message to SMS.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -131,14 +133,15 @@
         )
         return resp
 
 
 class SuccessSMS:
     """Sending success message to SMS
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -159,14 +162,15 @@
             data["text"],
         )
 
 
 class SendSMS:
     """Sending message to SMS
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/teams_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/teams_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import requests
-import traceback
+import os
 import re
+import json
 import datetime
+import requests
+import traceback
 from email.message import EmailMessage
-import sys
-import json
-import os
-from ExceptNotifier import send_teams_msg, receive_openai_advice
+from ExceptNotifier.base.teams_sender import send_teams_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptTeams(BaseException):
     """Override excepthook to send error message to Microsoft Teams.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -108,14 +109,15 @@
 
         return resp
 
 
 class SuccessTeams:
     """Sending success message to microsoft teams
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -130,14 +132,15 @@
 
         send_teams_msg(os.environ["_TEAMS_WEBHOOK_URL"], data["text"])
 
 
 class SendTeams:
     """Sending message to microsoft teams
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/telegram_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/telegram_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
+import re
+import os
 import requests
 import traceback
-import re
 import datetime
 from email.message import EmailMessage
-import os
-import sys
-from ExceptNotifier import send_telegram_msg, receive_openai_advice
+from ExceptNotifier.base.telegram_sender import send_telegram_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptTelegram(BaseException):
     """Override excepthook to send error message to Telegram.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
 
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
@@ -107,14 +108,15 @@
 
         return resp
 
 
 class SuccessTelegram:
     """Sending success message to telegram
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -129,14 +131,15 @@
 
         send_telegram_msg(os.environ["_TELEGRAM_TOKEN"], data["text"])
 
 
 class SendTelegram:
     """Sending message to telegram
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/python/wechat_notifier.py` & `exceptnotifier-0.2.2/ExceptNotifier/pycore/wechat_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
+import re
+import os
 import requests
 import traceback
-import re
 import datetime
 from email.message import EmailMessage
-import sys
-from ExceptNotifier import send_wechat_msg, receive_openai_advice
-import os
+from ExceptNotifier.base.wechat_sender import send_wechat_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptWechat(BaseException):
     """Override excepthook to send error message to Wechat.
 
     :param etype: Error Type
     :type etype: _type_
     :param value: Error Value
     :type value: _type_
     :param tb: Traceback Information
     :type tb: _type_
     """
+
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         excType = re.sub(
             "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
         ).strip()
@@ -98,14 +99,15 @@
         msg_template["text"]["content"] = "\n".join(msg)
         requests.post(_WECHAT_WEBHOOK_URL, json=msg_template)
 
 
 class SuccessWechat:
     """Sending success message to wechat
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
@@ -120,14 +122,15 @@
 
         send_wechat_msg(os.environ["_WECHAT_WEBHOOK_URL"], data["text"])
 
 
 class SendWechat:
     """Sending message to wechat
     """
+
     def __init__(self) -> None:
         pass
 
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
         f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.2.2/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.2.2/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -29,14 +29,16 @@
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
+
 </p>
 
 ![](./assets/imgs/main3.png)
 ##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
@@ -904,22 +906,23 @@
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
 
 <Br><br><br>
+# License
+MIT
 
-
+# Bugs and Issues
+[Open a new issue](https://github.com/dsdanielpark/ExceptNotifier/issues)
+ 
 # Contributing Guide
 I will announce contributing rules when the code development status changes to beta soon. Until then, please create an issue for feature requests and bug reports. I would greatly appreciate it if you use it a lot and give your opinions generously. Thank you sincerely.
 
-# License
-MIT
-
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
 
 # Contacts
 Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
 Email parkminwoo1991@gmail.com <br>
 - Developer note: [Link](./documents/DEV_NOTE.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.1 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.2 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -14,15 +14,16 @@
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Development Status :: 2 - Pre-Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 Before QA
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-             [PyPI package] [PyPI] [Downloads] [Code_style:_black]
+[PyPI package] [PyPI] [Downloads] [Code_style:_black] [https://img.shields.io/
+                         badge/License-MIT-yellow.svg]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
 shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
 /hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
 (https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
 flexible approach to receiving notifications by enhancing Python's try-except
 statement. This package enables you to receive alerts through various messaging
@@ -423,24 +424,25 @@
 ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
 try: print(1/0) SuccessDesktop().__call__() #1 success sender except
 ExceptDesktop as e: #2 except sender sys.exit() SendDesktop().__call__() #3
 customized sender ```
 
 
 
-# Contributing Guide I will announce contributing rules when the code
-development status changes to beta soon. Until then, please create an issue for
-feature requests and bug reports. I would greatly appreciate it if you use it a
-lot and give your opinions generously. Thank you sincerely. # License MIT #
-Code of Conduct Everyone participating in the `ExceptNotifier` project, and in
-particular in the issue tracker, pull requests, and social media activity, is
-expected to treat other people with respect and more generally to follow the
-guidelines articulated in [the Python Community Code of Conduct](https://
-www.python.org/psf/conduct/). # Contacts Core maintainers: [Daniel Park, South
-Korea](https://github.com/DSDanielPark)
+# License MIT # Bugs and Issues [Open a new issue](https://github.com/
+dsdanielpark/ExceptNotifier/issues) # Contributing Guide I will announce
+contributing rules when the code development status changes to beta soon. Until
+then, please create an issue for feature requests and bug reports. I would
+greatly appreciate it if you use it a lot and give your opinions generously.
+Thank you sincerely. # Code of Conduct Everyone participating in the
+`ExceptNotifier` project, and in particular in the issue tracker, pull
+requests, and social media activity, is expected to treat other people with
+respect and more generally to follow the guidelines articulated in [the Python
+Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts
+Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark)
 Email parkminwoo1991@gmail.com
 - Developer note: [Link](./documents/DEV_NOTE.md) #### Could you kindly add
 this badge to your repository? ``` ![Except-Notifier](https://img.shields.io/
 badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if you could share
 the document widely by specifying that the source is the ExceptNotifier
 official github. ##### The package is currently in the development and QA
 stages, and the development stage will be updated at the top of this page. If
```

### Comparing `exceptnotifier-0.2.1/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.2.2/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,40 +19,40 @@
 ExceptNotifier/base/openai_receiver.py
 ExceptNotifier/base/slack_sender.py
 ExceptNotifier/base/sms_sender.py
 ExceptNotifier/base/teams_sender.py
 ExceptNotifier/base/telegram_sender.py
 ExceptNotifier/base/wechat_sender.py
 ExceptNotifier/base/whatsapp_sender.py
-ExceptNotifier/ipython/__init__.py
-ExceptNotifier/ipython/beep_notifier_ipython.py
-ExceptNotifier/ipython/chime_notifier_ipython.py
-ExceptNotifier/ipython/desktop_notifier_ipython.py
-ExceptNotifier/ipython/discord_notifier_ipython.py
-ExceptNotifier/ipython/kakao_notifier_ipython.py
-ExceptNotifier/ipython/line_notifier_ipython.py
-ExceptNotifier/ipython/mail_notifier_ipython.py
-ExceptNotifier/ipython/slack_notifier_ipython.py
-ExceptNotifier/ipython/sms_notifier_ipython.py
-ExceptNotifier/ipython/teams_notifier_ipython.py
-ExceptNotifier/ipython/telegram_notifier_ipython.py
-ExceptNotifier/ipython/wechat_notifier_ipython.py
-ExceptNotifier/python/__init__.py
-ExceptNotifier/python/beep_notifier.py
-ExceptNotifier/python/chime_notifier.py
-ExceptNotifier/python/desktop_notifier.py
-ExceptNotifier/python/discord_notifier.py
-ExceptNotifier/python/kakao_notifier.py
-ExceptNotifier/python/line_notifier.py
-ExceptNotifier/python/mail_notifier.py
-ExceptNotifier/python/slack_notifier.py
-ExceptNotifier/python/sms_notifier.py
-ExceptNotifier/python/teams_notifier.py
-ExceptNotifier/python/telegram_notifier.py
-ExceptNotifier/python/wechat_notifier.py
+ExceptNotifier/ipycore/__init__.py
+ExceptNotifier/ipycore/beep_notifier_ipython.py
+ExceptNotifier/ipycore/chime_notifier_ipython.py
+ExceptNotifier/ipycore/desktop_notifier_ipython.py
+ExceptNotifier/ipycore/discord_notifier_ipython.py
+ExceptNotifier/ipycore/kakao_notifier_ipython.py
+ExceptNotifier/ipycore/line_notifier_ipython.py
+ExceptNotifier/ipycore/mail_notifier_ipython.py
+ExceptNotifier/ipycore/slack_notifier_ipython.py
+ExceptNotifier/ipycore/sms_notifier_ipython.py
+ExceptNotifier/ipycore/teams_notifier_ipython.py
+ExceptNotifier/ipycore/telegram_notifier_ipython.py
+ExceptNotifier/ipycore/wechat_notifier_ipython.py
+ExceptNotifier/pycore/__init__.py
+ExceptNotifier/pycore/beep_notifier.py
+ExceptNotifier/pycore/chime_notifier.py
+ExceptNotifier/pycore/desktop_notifier.py
+ExceptNotifier/pycore/discord_notifier.py
+ExceptNotifier/pycore/kakao_notifier.py
+ExceptNotifier/pycore/line_notifier.py
+ExceptNotifier/pycore/mail_notifier.py
+ExceptNotifier/pycore/slack_notifier.py
+ExceptNotifier/pycore/sms_notifier.py
+ExceptNotifier/pycore/teams_notifier.py
+ExceptNotifier/pycore/telegram_notifier.py
+ExceptNotifier/pycore/wechat_notifier.py
 ExceptNotifier/utils/__init__.py
 ExceptNotifier/utils/kakao_token.py
 exceptnotifier.egg-info/PKG-INFO
 exceptnotifier.egg-info/SOURCES.txt
 exceptnotifier.egg-info/dependency_links.txt
 exceptnotifier.egg-info/entry_points.txt
 exceptnotifier.egg-info/requires.txt
```

### Comparing `exceptnotifier-0.2.1/LICENSE` & `exceptnotifier-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.2.1/PKG-INFO` & `exceptnotifier-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.2.1
+Version: 0.2.2
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -29,14 +29,16 @@
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
+
 </p>
 
 ![](./assets/imgs/main3.png)
 ##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
@@ -904,22 +906,23 @@
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
 
 <Br><br><br>
+# License
+MIT
 
-
+# Bugs and Issues
+[Open a new issue](https://github.com/dsdanielpark/ExceptNotifier/issues)
+ 
 # Contributing Guide
 I will announce contributing rules when the code development status changes to beta soon. Until then, please create an issue for feature requests and bug reports. I would greatly appreciate it if you use it a lot and give your opinions generously. Thank you sincerely.
 
-# License
-MIT
-
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
 
 # Contacts
 Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
 Email parkminwoo1991@gmail.com <br>
 - Developer note: [Link](./documents/DEV_NOTE.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.1 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.2.2 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -14,15 +14,16 @@
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Development Status :: 2 - Pre-Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 Before QA
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-             [PyPI package] [PyPI] [Downloads] [Code_style:_black]
+[PyPI package] [PyPI] [Downloads] [Code_style:_black] [https://img.shields.io/
+                         badge/License-MIT-yellow.svg]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
 shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
 /hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
 (https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
 flexible approach to receiving notifications by enhancing Python's try-except
 statement. This package enables you to receive alerts through various messaging
@@ -423,24 +424,25 @@
 ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
 try: print(1/0) SuccessDesktop().__call__() #1 success sender except
 ExceptDesktop as e: #2 except sender sys.exit() SendDesktop().__call__() #3
 customized sender ```
 
 
 
-# Contributing Guide I will announce contributing rules when the code
-development status changes to beta soon. Until then, please create an issue for
-feature requests and bug reports. I would greatly appreciate it if you use it a
-lot and give your opinions generously. Thank you sincerely. # License MIT #
-Code of Conduct Everyone participating in the `ExceptNotifier` project, and in
-particular in the issue tracker, pull requests, and social media activity, is
-expected to treat other people with respect and more generally to follow the
-guidelines articulated in [the Python Community Code of Conduct](https://
-www.python.org/psf/conduct/). # Contacts Core maintainers: [Daniel Park, South
-Korea](https://github.com/DSDanielPark)
+# License MIT # Bugs and Issues [Open a new issue](https://github.com/
+dsdanielpark/ExceptNotifier/issues) # Contributing Guide I will announce
+contributing rules when the code development status changes to beta soon. Until
+then, please create an issue for feature requests and bug reports. I would
+greatly appreciate it if you use it a lot and give your opinions generously.
+Thank you sincerely. # Code of Conduct Everyone participating in the
+`ExceptNotifier` project, and in particular in the issue tracker, pull
+requests, and social media activity, is expected to treat other people with
+respect and more generally to follow the guidelines articulated in [the Python
+Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts
+Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark)
 Email parkminwoo1991@gmail.com
 - Developer note: [Link](./documents/DEV_NOTE.md) #### Could you kindly add
 this badge to your repository? ``` ![Except-Notifier](https://img.shields.io/
 badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if you could share
 the document widely by specifying that the source is the ExceptNotifier
 official github. ##### The package is currently in the development and QA
 stages, and the development stage will be updated at the top of this page. If
```

### Comparing `exceptnotifier-0.2.1/README.md` & `exceptnotifier-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 <h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
 <a><img alt="PyPI package" src="https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
+
 </p>
 
 ![](./assets/imgs/main3.png)
 ##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)](https://hits.seeyoufarm.com)                 
@@ -882,22 +884,23 @@
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
 
 <Br><br><br>
+# License
+MIT
 
-
+# Bugs and Issues
+[Open a new issue](https://github.com/dsdanielpark/ExceptNotifier/issues)
+ 
 # Contributing Guide
 I will announce contributing rules when the code development status changes to beta soon. Until then, please create an issue for feature requests and bug reports. I would greatly appreciate it if you use it a lot and give your opinions generously. Thank you sincerely.
 
-# License
-MIT
-
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
 
 # Contacts
 Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark) <br>
 Email parkminwoo1991@gmail.com <br>
 - Developer note: [Link](./documents/DEV_NOTE.md)
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 Development Status :: 2 - Pre-Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 Before QA
 ![](https://exceptnotifier.readthedocs.io/en/latest/_images/logo.png)
    ** Integrates AI-assisted debugging notifications into Python try-except
                statements for various messaging applications. **
-             [PyPI package] [PyPI] [Downloads] [Code_style:_black]
+[PyPI package] [PyPI] [Downloads] [Code_style:_black] [https://img.shields.io/
+                         badge/License-MIT-yellow.svg]
 ![](./assets/imgs/main3.png) ##### Provides a notification from the application
 shown in the captured screen. # Python Package: ExceptNotifier [![Hits](https:/
 /hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2Fdsdanielpark%2FExceptNotifier&count_bg=%2379C83D&title_bg=%23555555&icon=python.svg&icon_color=%23E7E7E7&title=ExceptNotifier&edge_flat=false)]
 (https://hits.seeyoufarm.com) The `ExceptNotifier` Python package offers a
 flexible approach to receiving notifications by enhancing Python's try-except
 statement. This package enables you to receive alerts through various messaging
@@ -409,24 +410,25 @@
 ['_OPEN_AI_MODEL']="gpt-3.5-turbo" # os.environ['_OPEN_AI_API']="sk-xxxxxx"
 try: print(1/0) SuccessDesktop().__call__() #1 success sender except
 ExceptDesktop as e: #2 except sender sys.exit() SendDesktop().__call__() #3
 customized sender ```
 
 
 
-# Contributing Guide I will announce contributing rules when the code
-development status changes to beta soon. Until then, please create an issue for
-feature requests and bug reports. I would greatly appreciate it if you use it a
-lot and give your opinions generously. Thank you sincerely. # License MIT #
-Code of Conduct Everyone participating in the `ExceptNotifier` project, and in
-particular in the issue tracker, pull requests, and social media activity, is
-expected to treat other people with respect and more generally to follow the
-guidelines articulated in [the Python Community Code of Conduct](https://
-www.python.org/psf/conduct/). # Contacts Core maintainers: [Daniel Park, South
-Korea](https://github.com/DSDanielPark)
+# License MIT # Bugs and Issues [Open a new issue](https://github.com/
+dsdanielpark/ExceptNotifier/issues) # Contributing Guide I will announce
+contributing rules when the code development status changes to beta soon. Until
+then, please create an issue for feature requests and bug reports. I would
+greatly appreciate it if you use it a lot and give your opinions generously.
+Thank you sincerely. # Code of Conduct Everyone participating in the
+`ExceptNotifier` project, and in particular in the issue tracker, pull
+requests, and social media activity, is expected to treat other people with
+respect and more generally to follow the guidelines articulated in [the Python
+Community Code of Conduct](https://www.python.org/psf/conduct/). # Contacts
+Core maintainers: [Daniel Park, South Korea](https://github.com/DSDanielPark)
 Email parkminwoo1991@gmail.com
 - Developer note: [Link](./documents/DEV_NOTE.md) #### Could you kindly add
 this badge to your repository? ``` ![Except-Notifier](https://img.shields.io/
 badge/pypi-ExceptNotifier-orange) ``` I would appreciate it if you could share
 the document widely by specifying that the source is the ExceptNotifier
 official github. ##### The package is currently in the development and QA
 stages, and the development stage will be updated at the top of this page. If
```

### Comparing `exceptnotifier-0.2.1/setup.py` & `exceptnotifier-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,31 @@
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.2.1",
+    version="0.2.2",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=["twilio", "plyer", "openai", "discord", "sphinx-rtd-theme", "Sphinx"],
+    install_requires=[
+        "twilio",
+        "plyer",
+        "openai",
+        "discord",
+        "sphinx-rtd-theme",
+        "Sphinx",
+    ],
     keywords="Exception, Python, Python Exception Alarm, Error notifications, Customizable notifications, Traceback management, Single line alarm",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```

