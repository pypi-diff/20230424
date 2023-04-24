# Comparing `tmp/COMTool-3.1.2.tar.gz` & `tmp/COMTool-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "COMTool-3.1.2.tar", last modified: Sat Aug 27 16:36:16 2022, max compression
+gzip compressed data, was "COMTool-3.2.0.tar", last modified: Mon Apr 24 09:48:43 2023, max compression
```

## Comparing `COMTool-3.1.2.tar` & `COMTool-3.2.0.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.181919 COMTool-3.1.2/
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.096037 COMTool-3.1.2/COMTool/
--rw-rw-rw-   0        0        0     1012 2021-12-05 06:22:12.000000 COMTool-3.1.2/COMTool/Combobox.py
--rw-rw-rw-   0        0        0      598 2022-08-27 15:30:30.000000 COMTool-3.1.2/COMTool/Main.py
--rw-rw-rw-   0        0        0       57 2021-12-05 08:58:15.000000 COMTool-3.1.2/COMTool/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.142888 COMTool-3.1.2/COMTool/assets/
--rw-rw-rw-   0        0        0    34855 2017-12-04 14:52:29.000000 COMTool-3.1.2/COMTool/assets/RaspberryPiScreenshot.png
--rw-rw-rw-   0        0        0      187 2021-12-05 05:31:34.000000 COMTool-3.1.2/COMTool/assets/arrow-down.png
--rw-rw-rw-   0        0        0      620 2021-12-04 12:29:22.000000 COMTool-3.1.2/COMTool/assets/arrow-left-white.png
--rw-rw-rw-   0        0        0      760 2021-12-04 12:30:24.000000 COMTool-3.1.2/COMTool/assets/arrow-left.png
--rw-rw-rw-   0        0        0      620 2021-12-04 12:29:27.000000 COMTool-3.1.2/COMTool/assets/arrow-right-white.png
--rw-rw-rw-   0        0        0      760 2021-12-04 12:30:28.000000 COMTool-3.1.2/COMTool/assets/arrow-right.png
--rw-rw-rw-   0        0        0      422 2022-03-21 15:08:01.000000 COMTool-3.1.2/COMTool/assets/close.png
--rw-rw-rw-   0        0        0    21138 2022-04-01 14:36:03.000000 COMTool-3.1.2/COMTool/assets/donate_alipay.jpg
--rw-rw-rw-   0        0        0    13294 2022-04-01 14:35:25.000000 COMTool-3.1.2/COMTool/assets/donate_wechat.jpg
--rw-rw-rw-   0        0        0      645 2021-12-04 12:34:44.000000 COMTool-3.1.2/COMTool/assets/help-white.png
--rw-rw-rw-   0        0        0      810 2021-12-04 12:34:39.000000 COMTool-3.1.2/COMTool/assets/help.png
--rw-rw-rw-   0        0        0      260 2022-03-21 15:22:21.000000 COMTool-3.1.2/COMTool/assets/left.png
--rw-rw-rw-   0        0        0    39706 2019-07-04 13:00:02.000000 COMTool-3.1.2/COMTool/assets/logo.icns
--rw-rw-rw-   0        0        0   370070 2017-12-04 14:02:14.000000 COMTool-3.1.2/COMTool/assets/logo.ico
--rw-rw-rw-   0        0        0    25270 2022-04-23 15:02:30.000000 COMTool-3.1.2/COMTool/assets/logo.png
--rw-rw-rw-   0        0        0    20959 2017-12-04 14:02:14.000000 COMTool-3.1.2/COMTool/assets/logo2.png
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.145880 COMTool-3.1.2/COMTool/assets/qss/
--rw-rw-rw-   0        0        0    10548 2022-08-27 13:43:39.000000 COMTool-3.1.2/COMTool/assets/qss/style-dark.qss
--rw-rw-rw-   0        0        0    10397 2022-08-27 13:43:33.000000 COMTool-3.1.2/COMTool/assets/qss/style.qss
--rw-rw-rw-   0        0        0      244 2022-03-21 15:22:34.000000 COMTool-3.1.2/COMTool/assets/right.png
--rw-rw-rw-   0        0        0    23575 2017-12-04 14:02:14.000000 COMTool-3.1.2/COMTool/assets/screenshot_V1.0.png
--rw-rw-rw-   0        0        0    21695 2017-12-04 14:02:14.000000 COMTool-3.1.2/COMTool/assets/screenshot_V1.3.png
--rw-rw-rw-   0        0        0    50561 2017-12-04 14:02:14.000000 COMTool-3.1.2/COMTool/assets/screenshot_V1.4_night.png
--rw-rw-rw-   0        0        0    23942 2018-11-28 08:45:54.000000 COMTool-3.1.2/COMTool/assets/screenshot_V1.7.png
--rw-rw-rw-   0        0        0   175686 2022-04-07 13:18:05.000000 COMTool-3.1.2/COMTool/assets/screenshot_graph.png
--rw-rw-rw-   0        0        0    76071 2022-03-05 08:46:22.000000 COMTool-3.1.2/COMTool/assets/screenshot_protocol_v2.3.png
--rw-rw-rw-   0        0        0    47979 2022-03-18 11:25:06.000000 COMTool-3.1.2/COMTool/assets/screenshot_terminal.png
--rw-rw-rw-   0        0        0    70084 2021-12-09 14:09:03.000000 COMTool-3.1.2/COMTool/assets/screenshot_v2.png
--rw-rw-rw-   0        0        0    67071 2021-12-09 14:20:48.000000 COMTool-3.1.2/COMTool/assets/screenshot_v2_white.png
--rw-rw-rw-   0        0        0      714 2021-12-04 12:37:20.000000 COMTool-3.1.2/COMTool/assets/skin-white.png
--rw-rw-rw-   0        0        0      860 2021-12-04 12:33:37.000000 COMTool-3.1.2/COMTool/assets/skin.png
--rw-rw-rw-   0        0        0    15142 2022-03-07 13:37:08.000000 COMTool-3.1.2/COMTool/assets/tcp_udp.png
--rw-rw-rw-   0        0        0      562 2017-12-04 15:41:24.000000 COMTool-3.1.2/COMTool/assets/wave-white.png
--rw-rw-rw-   0        0        0      665 2017-12-04 15:41:50.000000 COMTool-3.1.2/COMTool/assets/wave.png
--rw-rw-rw-   0        0        0     3220 2022-03-21 10:53:04.000000 COMTool-3.1.2/COMTool/autoUpdate.py
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.152862 COMTool-3.1.2/COMTool/conn/
--rw-rw-rw-   0        0        0      159 2022-03-19 05:53:59.000000 COMTool-3.1.2/COMTool/conn/__init__.py
--rw-rw-rw-   0        0        0     1856 2022-03-27 15:04:30.000000 COMTool-3.1.2/COMTool/conn/base.py
--rw-rw-rw-   0        0        0    20415 2022-08-20 15:22:13.000000 COMTool-3.1.2/COMTool/conn/conn_serial.py
--rw-rw-rw-   0        0        0    16515 2022-03-28 13:38:36.000000 COMTool-3.1.2/COMTool/conn/conn_ssh.py
--rw-rw-rw-   0        0        0    24898 2022-04-07 13:18:05.000000 COMTool-3.1.2/COMTool/conn/conn_tcp_udp.py
--rw-rw-rw-   0        0        0     1224 2022-03-06 06:48:53.000000 COMTool-3.1.2/COMTool/conn/test_tcp_udp.py
--rw-rw-rw-   0        0        0     2152 2022-04-05 08:20:31.000000 COMTool-3.1.2/COMTool/helpAbout.py
--rw-rw-rw-   0        0        0     5071 2022-04-17 09:20:56.000000 COMTool-3.1.2/COMTool/i18n.py
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.067114 COMTool-3.1.2/COMTool/locales/
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.065119 COMTool-3.1.2/COMTool/locales/en/
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.154857 COMTool-3.1.2/COMTool/locales/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      443 2022-08-27 14:34:33.000000 COMTool-3.1.2/COMTool/locales/en/LC_MESSAGES/messages.mo
--rw-rw-rw-   0        0        0    18489 2022-08-27 14:05:33.000000 COMTool-3.1.2/COMTool/locales/en/LC_MESSAGES/messages.po
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.066117 COMTool-3.1.2/COMTool/locales/ja/
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.156852 COMTool-3.1.2/COMTool/locales/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7717 2022-08-27 14:34:33.000000 COMTool-3.1.2/COMTool/locales/ja/LC_MESSAGES/messages.mo
--rw-rw-rw-   0        0        0    22870 2022-08-27 14:05:33.000000 COMTool-3.1.2/COMTool/locales/ja/LC_MESSAGES/messages.po
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.066117 COMTool-3.1.2/COMTool/locales/zh_CN/
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.158846 COMTool-3.1.2/COMTool/locales/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10838 2022-08-27 14:34:33.000000 COMTool-3.1.2/COMTool/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-rw-rw-   0        0        0    21068 2022-08-27 14:08:02.000000 COMTool-3.1.2/COMTool/locales/zh_CN/LC_MESSAGES/messages.po
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.067114 COMTool-3.1.2/COMTool/locales/zh_TW/
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.162859 COMTool-3.1.2/COMTool/locales/zh_TW/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9918 2022-08-27 14:34:33.000000 COMTool-3.1.2/COMTool/locales/zh_TW/LC_MESSAGES/messages.mo
--rw-rw-rw-   0        0        0    21639 2022-08-27 14:13:03.000000 COMTool-3.1.2/COMTool/locales/zh_TW/LC_MESSAGES/messages.po
--rw-rw-rw-   0        0        0     3384 2022-03-21 10:09:54.000000 COMTool-3.1.2/COMTool/logger.py
--rw-rw-rw-   0        0        0    28482 2022-04-23 14:57:54.000000 COMTool-3.1.2/COMTool/main2.py
--rw-rw-rw-   0        0        0     4467 2022-04-23 14:57:57.000000 COMTool-3.1.2/COMTool/parameters.py
--rw-rw-rw-   0        0        0    12469 2022-04-07 13:18:05.000000 COMTool-3.1.2/COMTool/pluginItems.py
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.179924 COMTool-3.1.2/COMTool/plugins/
--rw-rw-rw-   0        0        0      304 2022-08-27 13:44:01.000000 COMTool-3.1.2/COMTool/plugins/__init__.py
--rw-rw-rw-   0        0        0     7160 2022-05-04 10:27:24.000000 COMTool-3.1.2/COMTool/plugins/base.py
--rw-rw-rw-   0        0        0     3580 2021-12-20 12:39:16.000000 COMTool-3.1.2/COMTool/plugins/crc.py
--rw-rw-rw-   0        0        0    39176 2022-08-21 16:45:40.000000 COMTool-3.1.2/COMTool/plugins/dbg.py
--rw-rw-rw-   0        0        0     7679 2022-08-27 14:10:24.000000 COMTool-3.1.2/COMTool/plugins/graph.py
--rw-rw-rw-   0        0        0      275 2022-04-07 13:18:05.000000 COMTool-3.1.2/COMTool/plugins/graph_protocol.py
--rw-rw-rw-   0        0        0    34150 2022-08-27 14:03:18.000000 COMTool-3.1.2/COMTool/plugins/graph_widget_metasenselite.py
--rw-rw-rw-   0        0        0    14068 2022-08-27 14:01:57.000000 COMTool-3.1.2/COMTool/plugins/graph_widgets.py
--rw-rw-rw-   0        0        0      793 2022-08-27 14:02:44.000000 COMTool-3.1.2/COMTool/plugins/graph_widgets_base.py
--rw-rw-rw-   0        0        0     2794 2022-03-21 15:40:48.000000 COMTool-3.1.2/COMTool/plugins/myplugin.py
--rw-rw-rw-   0        0        0    25913 2022-04-07 13:18:05.000000 COMTool-3.1.2/COMTool/plugins/protocol.py
--rw-rw-rw-   0        0        0      602 2022-03-03 14:20:49.000000 COMTool-3.1.2/COMTool/plugins/protocols.py
--rw-rw-rw-   0        0        0    26986 2022-05-01 04:42:00.000000 COMTool-3.1.2/COMTool/plugins/terminal.py
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.180922 COMTool-3.1.2/COMTool/protocols/
--rw-rw-rw-   0        0        0    20434 2022-03-02 13:31:15.000000 COMTool-3.1.2/COMTool/protocols/maix-smart.py
--rw-rw-rw-   0        0        0    10420 2021-12-24 13:51:24.000000 COMTool-3.1.2/COMTool/qta_icon_browser.py
--rw-rw-rw-   0        0        0      952 2021-12-05 09:14:36.000000 COMTool-3.1.2/COMTool/settings.py
--rw-rw-rw-   0        0        0     3144 2021-12-19 10:24:48.000000 COMTool-3.1.2/COMTool/test.py
--rw-rw-rw-   0        0        0     2823 2022-04-06 14:21:02.000000 COMTool-3.1.2/COMTool/utils.py
--rw-rw-rw-   0        0        0     1537 2022-03-03 13:26:46.000000 COMTool-3.1.2/COMTool/utils_ui.py
--rw-rw-rw-   0        0        0      928 2022-08-27 16:14:05.000000 COMTool-3.1.2/COMTool/version.py
--rw-rw-rw-   0        0        0     1475 2017-12-06 14:29:18.000000 COMTool-3.1.2/COMTool/wave.py
--rw-rw-rw-   0        0        0    31633 2022-04-23 14:57:59.000000 COMTool-3.1.2/COMTool/widgets.py
--rw-rw-rw-   0        0        0     3615 2022-03-28 16:25:18.000000 COMTool-3.1.2/COMTool/win32_utils.py
-drwxrwxrwx   0        0        0        0 2022-08-27 16:36:16.103571 COMTool-3.1.2/COMTool.egg-info/
--rw-rw-rw-   0        0        0    16743 2022-08-27 16:36:14.000000 COMTool-3.1.2/COMTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2573 2022-08-27 16:36:14.000000 COMTool-3.1.2/COMTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-27 16:36:14.000000 COMTool-3.1.2/COMTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2022-08-27 16:36:14.000000 COMTool-3.1.2/COMTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      101 2022-08-27 16:36:14.000000 COMTool-3.1.2/COMTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-27 16:36:14.000000 COMTool-3.1.2/COMTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7642 2021-12-09 14:09:03.000000 COMTool-3.1.2/LICENSE
--rw-rw-rw-   0        0        0       52 2017-12-04 14:03:40.000000 COMTool-3.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    16743 2022-08-27 16:36:16.181919 COMTool-3.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    12631 2022-08-27 13:43:28.000000 COMTool-3.1.2/README.MD
--rw-rw-rw-   0        0        0       97 2022-08-27 16:36:16.187903 COMTool-3.1.2/setup.cfg
--rw-rw-rw-   0        0        0     4954 2022-05-01 11:29:10.000000 COMTool-3.1.2/setup.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.446301 COMTool-3.2.0/
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.422302 COMTool-3.2.0/COMTool/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1012 2021-12-15 02:14:16.000000 COMTool-3.2.0/COMTool/Combobox.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      598 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/Main.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)       57 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/__init__.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.438301 COMTool-3.2.0/COMTool/assets/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    34855 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/RaspberryPiScreenshot.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      187 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/arrow-down.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      620 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/arrow-left-white.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      760 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/arrow-left.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      620 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/arrow-right-white.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      760 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/arrow-right.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      422 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/assets/close.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    21138 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/assets/donate_alipay.jpg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    13294 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/assets/donate_wechat.jpg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      645 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/help-white.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      810 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/help.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      260 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/assets/left.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    39706 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/logo.icns
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)   370070 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/logo.ico
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    25270 2022-03-04 03:00:33.000000 COMTool-3.2.0/COMTool/assets/logo.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    20959 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/logo2.png
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.438301 COMTool-3.2.0/COMTool/assets/qss/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    10548 2022-08-31 02:14:24.000000 COMTool-3.2.0/COMTool/assets/qss/style-dark.qss
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    10397 2022-08-31 02:14:24.000000 COMTool-3.2.0/COMTool/assets/qss/style.qss
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      244 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/assets/right.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    23575 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/screenshot_V1.0.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    21695 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/screenshot_V1.3.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    50561 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/screenshot_V1.4_night.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    23942 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/screenshot_V1.7.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)   175686 2022-08-31 02:14:25.000000 COMTool-3.2.0/COMTool/assets/screenshot_graph.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    45043 2022-11-29 05:51:35.000000 COMTool-3.2.0/COMTool/assets/screenshot_macos.jpg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    76071 2022-03-04 02:31:25.000000 COMTool-3.2.0/COMTool/assets/screenshot_protocol_v2.3.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    47979 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/assets/screenshot_terminal.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    70084 2021-12-09 10:13:07.000000 COMTool-3.2.0/COMTool/assets/screenshot_v2.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    67071 2021-12-10 02:58:51.000000 COMTool-3.2.0/COMTool/assets/screenshot_v2_white.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      714 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/skin-white.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      860 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/skin.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    15142 2022-03-07 08:24:24.000000 COMTool-3.2.0/COMTool/assets/tcp_udp.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      562 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/wave-white.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      665 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/assets/wave.png
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3220 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/autoUpdate.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.438301 COMTool-3.2.0/COMTool/conn/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      159 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/conn/__init__.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1856 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/conn/base.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    20415 2022-12-16 09:04:15.000000 COMTool-3.2.0/COMTool/conn/conn_serial.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    16515 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/conn/conn_ssh.py
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)    25526 2023-04-24 06:59:55.000000 COMTool-3.2.0/COMTool/conn/conn_tcp_udp.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1224 2022-03-04 10:42:33.000000 COMTool-3.2.0/COMTool/conn/test_tcp_udp.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2152 2022-04-06 01:55:14.000000 COMTool-3.2.0/COMTool/helpAbout.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     5071 2022-05-07 10:26:38.000000 COMTool-3.2.0/COMTool/i18n.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.418302 COMTool-3.2.0/COMTool/locales/
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.418302 COMTool-3.2.0/COMTool/locales/en/
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.438301 COMTool-3.2.0/COMTool/locales/en/LC_MESSAGES/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      445 2023-04-21 07:04:55.000000 COMTool-3.2.0/COMTool/locales/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    18550 2022-11-29 07:00:04.000000 COMTool-3.2.0/COMTool/locales/en/LC_MESSAGES/messages.po
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.418302 COMTool-3.2.0/COMTool/locales/ja/
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.442301 COMTool-3.2.0/COMTool/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     7957 2023-04-21 07:04:55.000000 COMTool-3.2.0/COMTool/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    23051 2022-11-29 07:00:04.000000 COMTool-3.2.0/COMTool/locales/ja/LC_MESSAGES/messages.po
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.418302 COMTool-3.2.0/COMTool/locales/zh_CN/
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.442301 COMTool-3.2.0/COMTool/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    11256 2023-04-21 07:04:55.000000 COMTool-3.2.0/COMTool/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    21300 2022-11-29 07:00:04.000000 COMTool-3.2.0/COMTool/locales/zh_CN/LC_MESSAGES/messages.po
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.418302 COMTool-3.2.0/COMTool/locales/zh_TW/
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.442301 COMTool-3.2.0/COMTool/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    10351 2023-04-21 07:04:55.000000 COMTool-3.2.0/COMTool/locales/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    21886 2022-11-29 07:00:04.000000 COMTool-3.2.0/COMTool/locales/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3384 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/logger.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    28482 2022-05-07 10:26:38.000000 COMTool-3.2.0/COMTool/main2.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     4467 2022-04-07 06:22:34.000000 COMTool-3.2.0/COMTool/parameters.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    12469 2022-04-07 03:26:43.000000 COMTool-3.2.0/COMTool/pluginItems.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.446301 COMTool-3.2.0/COMTool/plugins/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      304 2022-08-31 02:14:25.000000 COMTool-3.2.0/COMTool/plugins/__init__.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     7160 2022-05-07 10:26:38.000000 COMTool-3.2.0/COMTool/plugins/base.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3580 2021-12-20 11:08:12.000000 COMTool-3.2.0/COMTool/plugins/crc.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    42828 2022-11-29 07:35:09.000000 COMTool-3.2.0/COMTool/plugins/dbg.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     8008 2023-04-24 08:06:27.000000 COMTool-3.2.0/COMTool/plugins/graph.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      275 2022-08-31 02:14:25.000000 COMTool-3.2.0/COMTool/plugins/graph_protocol.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    34150 2022-08-31 02:14:25.000000 COMTool-3.2.0/COMTool/plugins/graph_widget_metasenselite.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    14366 2023-04-24 07:49:09.000000 COMTool-3.2.0/COMTool/plugins/graph_widgets.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      793 2022-08-31 02:14:25.000000 COMTool-3.2.0/COMTool/plugins/graph_widgets_base.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2794 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/plugins/myplugin.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    25913 2022-04-07 03:08:29.000000 COMTool-3.2.0/COMTool/plugins/protocol.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      602 2022-03-04 03:00:33.000000 COMTool-3.2.0/COMTool/plugins/protocols.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    26986 2022-05-07 10:26:38.000000 COMTool-3.2.0/COMTool/plugins/terminal.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.446301 COMTool-3.2.0/COMTool/protocols/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    20434 2022-03-02 09:33:14.000000 COMTool-3.2.0/COMTool/protocols/maix-smart.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    10420 2021-12-24 09:08:21.000000 COMTool-3.2.0/COMTool/qta_icon_browser.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      952 2021-12-06 01:52:19.000000 COMTool-3.2.0/COMTool/settings.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3144 2021-12-23 10:37:40.000000 COMTool-3.2.0/COMTool/test.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2823 2022-04-07 01:38:48.000000 COMTool-3.2.0/COMTool/utils.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1537 2022-03-03 07:16:48.000000 COMTool-3.2.0/COMTool/utils_ui.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      928 2023-04-24 08:52:35.000000 COMTool-3.2.0/COMTool/version.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1475 2020-10-12 05:08:27.000000 COMTool-3.2.0/COMTool/wave.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    31633 2022-11-29 05:54:30.000000 COMTool-3.2.0/COMTool/widgets.py
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3615 2022-04-02 09:29:28.000000 COMTool-3.2.0/COMTool/win32_utils.py
+drwxrwxr-x   0 neucrack  (1000) neucrack  (1000)        0 2023-04-24 09:48:43.422302 COMTool-3.2.0/COMTool.egg-info/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    13543 2023-04-24 09:48:43.000000 COMTool-3.2.0/COMTool.egg-info/PKG-INFO
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2609 2023-04-24 09:48:43.000000 COMTool-3.2.0/COMTool.egg-info/SOURCES.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)        1 2023-04-24 09:48:43.000000 COMTool-3.2.0/COMTool.egg-info/dependency_links.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)       99 2023-04-24 09:48:43.000000 COMTool-3.2.0/COMTool.egg-info/entry_points.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      101 2023-04-24 09:48:43.000000 COMTool-3.2.0/COMTool.egg-info/requires.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)        8 2023-04-24 09:48:43.000000 COMTool-3.2.0/COMTool.egg-info/top_level.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     7642 2021-12-09 11:16:14.000000 COMTool-3.2.0/LICENSE
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)       52 2020-10-12 05:08:27.000000 COMTool-3.2.0/MANIFEST.in
+-rw-rw-r--   0 neucrack  (1000) neucrack  (1000)    13543 2023-04-24 09:48:43.446301 COMTool-3.2.0/PKG-INFO
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    12699 2023-01-03 02:16:58.000000 COMTool-3.2.0/README.MD
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)       88 2023-04-24 09:48:43.446301 COMTool-3.2.0/setup.cfg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     4954 2022-05-07 10:26:38.000000 COMTool-3.2.0/setup.py
```

### Comparing `COMTool-3.1.2/COMTool/Combobox.py` & `COMTool-3.2.0/COMTool/Combobox.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/Main.py` & `COMTool-3.2.0/COMTool/Main.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/RaspberryPiScreenshot.png` & `COMTool-3.2.0/COMTool/assets/RaspberryPiScreenshot.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/arrow-left-white.png` & `COMTool-3.2.0/COMTool/assets/arrow-left-white.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/arrow-left.png` & `COMTool-3.2.0/COMTool/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/arrow-right-white.png` & `COMTool-3.2.0/COMTool/assets/arrow-right-white.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/arrow-right.png` & `COMTool-3.2.0/COMTool/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/donate_alipay.jpg` & `COMTool-3.2.0/COMTool/assets/donate_alipay.jpg`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/donate_wechat.jpg` & `COMTool-3.2.0/COMTool/assets/donate_wechat.jpg`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/help-white.png` & `COMTool-3.2.0/COMTool/assets/help-white.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/help.png` & `COMTool-3.2.0/COMTool/assets/help.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/logo.icns` & `COMTool-3.2.0/COMTool/assets/logo.icns`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/logo.ico` & `COMTool-3.2.0/COMTool/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/logo.png` & `COMTool-3.2.0/COMTool/assets/logo.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/logo2.png` & `COMTool-3.2.0/COMTool/assets/logo2.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/qss/style-dark.qss` & `COMTool-3.2.0/COMTool/assets/qss/style-dark.qss`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/qss/style.qss` & `COMTool-3.2.0/COMTool/assets/qss/style.qss`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_V1.0.png` & `COMTool-3.2.0/COMTool/assets/screenshot_V1.0.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_V1.3.png` & `COMTool-3.2.0/COMTool/assets/screenshot_V1.3.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_V1.4_night.png` & `COMTool-3.2.0/COMTool/assets/screenshot_V1.4_night.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_V1.7.png` & `COMTool-3.2.0/COMTool/assets/screenshot_V1.7.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_graph.png` & `COMTool-3.2.0/COMTool/assets/screenshot_graph.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_protocol_v2.3.png` & `COMTool-3.2.0/COMTool/assets/screenshot_protocol_v2.3.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_terminal.png` & `COMTool-3.2.0/COMTool/assets/screenshot_terminal.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_v2.png` & `COMTool-3.2.0/COMTool/assets/screenshot_v2.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/screenshot_v2_white.png` & `COMTool-3.2.0/COMTool/assets/screenshot_v2_white.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/skin-white.png` & `COMTool-3.2.0/COMTool/assets/skin-white.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/skin.png` & `COMTool-3.2.0/COMTool/assets/skin.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/tcp_udp.png` & `COMTool-3.2.0/COMTool/assets/tcp_udp.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/wave-white.png` & `COMTool-3.2.0/COMTool/assets/wave-white.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/assets/wave.png` & `COMTool-3.2.0/COMTool/assets/wave.png`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/autoUpdate.py` & `COMTool-3.2.0/COMTool/autoUpdate.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/conn/base.py` & `COMTool-3.2.0/COMTool/conn/base.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/conn/conn_serial.py` & `COMTool-3.2.0/COMTool/conn/conn_serial.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/conn/conn_ssh.py` & `COMTool-3.2.0/COMTool/conn/conn_ssh.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/conn/conn_tcp_udp.py` & `COMTool-3.2.0/COMTool/conn/conn_tcp_udp.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self.serialSettingsLayout.addWidget(self.clientsCombobox, 4, 0, 1, 2)
         self.serialSettingsLayout.addWidget(self.disconnetClientBtn, 4, 2, 1, 1)
         self.serialSettingsLayout.addWidget(self.autoReconnetLable, 5, 0, 1, 1)
         self.serialSettingsLayout.addWidget(self.autoReconnect, 5, 1, 1, 1)
         self.serialSettingsLayout.addWidget(self.autoReconnectIntervalEdit, 5, 2, 1, 1)
         self.serialSettingsLayout.addWidget(self.serialOpenCloseButton, 6, 0, 1, 3)
         serialSetting.setLayout(self.serialSettingsLayout)
-        self.widgetConfMap["protocol"]       = self.protoclTcpRadioBtn
+        self.widgetConfMap["protocol"]       = [self.protoclTcpRadioBtn, self.protoclUdpRadioBtn]
         self.widgetConfMap["mode"]    = self.modeClientRadioBtn
         self.widgetConfMap["target"]    = self.targetCombobox
         self.widgetConfMap["port"]    = self.porttEdit
         self.widgetConfMap["auto_reconnect"] = self.autoReconnect
         self.widgetConfMap["auto_reconnect_interval"] = self.autoReconnectIntervalEdit
         self.initEvet()
         self.widget = serialSetting
@@ -271,28 +271,32 @@
                 pass
 
     def onPortChanged(self):
         text = self.porttEdit.text()
         while 1:
             try:
                 port = int(text)
+                self.config['port'] = port
                 break
             except Exception:
                 text = text[:-1]
+                break
         self.porttEdit.setText(text)
 
     def onSerialConfigChanged(self, conf_type, obj, value_type, caller=""):
         pass
 
     def setSerialConfig(self, conf_type, obj, value):
         if conf_type == "protocol":
             if value == "tcp":
-                obj.setChecked(True)
+                obj[0].setChecked(True)
+                obj[1].setChecked(False)
             else:
-                obj.setChecked(False)
+                obj[0].setChecked(False)
+                obj[1].setChecked(True)
         elif conf_type == "mode":
             if value == "client":
                 obj.setChecked(True)
                 self.changeMode("client", init=True)
             else:
                 obj.setChecked(False)
                 self.modeServerRadioBtn.setChecked(True)
@@ -334,28 +338,31 @@
 
     def openCloseSerialProcess(self):
         if self.isOpened:
             print("-- disconnect")
             try:
                 # set status first to prevent auto reconnect
                 self.status = ConnectionStatus.CLOSED
+                for addr, conn in self.serverModeClientsConns.items():
+                    try:
+                        print(f"-- close client {addr} conn")
+                        conn.close()
+                    except Exception as e:
+                        print(f"close client {addr} conn error: ", e)
+                        pass
                 if not self.conn is None:
                     time.sleep(0.1) # wait receive thread exit
                     try:
                         self.conn.close()
-                    except Exception:
+                    except Exception as e:
+                        print("close conn error: ", e)
                         pass
                     self.conn = None
-                for k, conn in self.serverModeClientsConns.items():
-                    try:
-                        conn.close()
-                    except Exception:
-                        pass
             except Exception as e:
-                print(e)
+                print("openCloseSerialProcess", e)
                 pass
             self.onConnectionStatus.emit(self.status, "")
             self.showSwitchSignal.emit(self.status)
         else:
             try:
                 if self.config["protocol"] == "tcp":
                     if self.config["mode"] == "client":
@@ -371,15 +378,15 @@
                         print("-- connect success")
                         self.receiveProcess = threading.Thread(target=self.receiveDataProcess, args=(self.conn, ))
                         self.receiveProcess.setDaemon(True)
                         self.receiveProcess.start()
                     else:
                         print("-- server mode, wait client connect")
                         self.conn = socket.socket()
-                        self.conn.setsockopt(socket.SOL_SOCKET,socket.SO_REUSEADDR,1)
+                        self.conn.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
                         self.conn.bind(("0.0.0.0", self.config["port"]))
                         self.conn.listen(100)
                         self.status = ConnectionStatus.CONNECTED
                         self.waitClentsProcess = threading.Thread(target=self.waitClientsProcess)
                         self.waitClentsProcess.setDaemon(True)
                         self.waitClentsProcess.start()
                 else:
@@ -444,30 +451,35 @@
 
     def updateStyle(self, widget):
         self.widget.style().unpolish(widget)
         self.widget.style().polish(widget)
         self.widget.update()
 
     def waitClientsProcess(self):
+        print("-- wait for client connect")
         while self.status != ConnectionStatus.CLOSED:
-            print("-- wait for client connect")
+            # accept connection with non-blocking to check close status
+            self.conn.settimeout(0.06)
             try:
                 conn, addr = self.conn.accept()
+            except socket.timeout:
+                continue
             except Exception as e:
                 if self.status != ConnectionStatus.CLOSED:
                     print("-- accept connection fail:", str(e))
                 continue
             print("-- client connected, ip:", addr)
             addr_str = f'{addr[0]}:{addr[1]}'
             self.updateClientsSignal.emit(True, addr)
             self.onConnectionStatus.emit(ConnectionStatus.CONNECTED, _("Client connected:") + " " + addr_str)
             self.serverModeClientsConns[addr_str] = conn
             t = threading.Thread(target=self.receiveDataProcess, args=(conn, addr))
             t.setDaemon(True)
             t.start()
+            print("-- wait for client connect")
         print("-- wait connection thread exit")
 
 
     def receiveDataProcess(self, conn, remote_addr:tuple = None):
         waitingReconnect = False
         buffer = b''
         t = 0
@@ -552,16 +564,16 @@
                     except Exception:
                         pass
                     waitingReconnect = True
                     self.onConnectionStatus.emit(ConnectionStatus.LOSE, _("Connection lose!"))
                     self.showSwitchSignal.emit(ConnectionStatus.LOSE)
                     time.sleep(self.config["auto_reconnect_interval"])
         # server mode remove client
-        if self.config["mode"] == "server":
-            remote_str = f'{remote_addr[0]}:{remote_addr[1]}'
+        remote_str = f'{remote_addr[0]}:{remote_addr[1]}'
+        if remote_str in self.serverModeClientsConns:
             print(f"-- client {remote_str} disconnect")
             self.updateClientsSignal.emit(False, remote_addr)
             if remote_str == self.serverModeSelectedClient:
                 self.serverModeSelectedClient = None
             self.serverModeClientsConns.pop(remote_str)
         print("-- receiveDataProcess exit")
```

### Comparing `COMTool-3.1.2/COMTool/conn/test_tcp_udp.py` & `COMTool-3.2.0/COMTool/conn/test_tcp_udp.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/helpAbout.py` & `COMTool-3.2.0/COMTool/helpAbout.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/i18n.py` & `COMTool-3.2.0/COMTool/i18n.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/locales/en/LC_MESSAGES/messages.po` & `COMTool-3.2.0/COMTool/locales/en/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:21+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 #: helpAbout.py:40
 msgid "Config path"
 msgstr ""
 
 #: helpAbout.py:42
 msgid "Old config backup in"
@@ -66,19 +66,18 @@
 msgid "Load plugin from file"
 msgstr ""
 
 #: conn/conn_serial.py:331 conn/conn_ssh.py:289 conn/conn_tcp_udp.py:403
 #: main2.py:229 main2.py:279 main2.py:422 main2.py:427 main2.py:723
 #: pluginItems.py:169 pluginItems.py:172 pluginItems.py:273 pluginItems.py:285
 #: plugins/base.py:165 plugins/base.py:170 plugins/base.py:186
-#: plugins/base.py:195 plugins/dbg.py:401 plugins/dbg.py:410 plugins/dbg.py:531
-#: plugins/dbg.py:548 plugins/dbg.py:605 plugins/dbg.py:613
+#: plugins/base.py:195 plugins/dbg.py:426 plugins/dbg.py:435 plugins/dbg.py:574
+#: plugins/dbg.py:591 plugins/dbg.py:648 plugins/dbg.py:656
 #: plugins/graph.py:205 plugins/graph_widget_metasenselite.py:591
 #: plugins/graph_widgets.py:141 plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/protocol.py:466 plugins/protocol.py:480 plugins/protocol.py:489
 #: plugins/protocol.py:552
 msgid "Error"
 msgstr ""
 
 #: main2.py:229
@@ -86,15 +85,15 @@
 msgstr ""
 
 #: main2.py:250
 msgid "Load plugin fail"
 msgstr ""
 
 #: conn/conn_ssh.py:232 main2.py:273 pluginItems.py:149 pluginItems.py:162
-#: plugins/dbg.py:423 plugins/dbg.py:437
+#: plugins/dbg.py:448 plugins/dbg.py:462
 msgid "Select file"
 msgstr ""
 
 #: main2.py:275
 msgid "python script (*.py)"
 msgstr ""
 
@@ -168,15 +167,15 @@
 "to "
 msgstr ""
 
 #: pluginItems.py:172
 msgid "Config is not for this plugin, config is for plugin:"
 msgstr ""
 
-#: pluginItems.py:175 plugins/dbg.py:366 plugins/dbg.py:534
+#: pluginItems.py:175 plugins/dbg.py:384 plugins/dbg.py:577
 #: plugins/protocol.py:574 plugins/protocol.py:596
 msgid "Warning"
 msgstr ""
 
 #: pluginItems.py:176
 msgid "Config version not same, plugin config version:"
 msgstr ""
@@ -215,15 +214,15 @@
 msgid "Help"
 msgstr ""
 
 #: widgets.py:661
 msgid "Input remark"
 msgstr ""
 
-#: plugins/dbg.py:191 widgets.py:671 widgets.py:742
+#: plugins/dbg.py:197 widgets.py:671 widgets.py:742
 msgid "Record"
 msgstr ""
 
 #: widgets.py:676
 msgid "Input value"
 msgstr ""
 
@@ -235,15 +234,15 @@
 msgid "Shortcut"
 msgstr ""
 
 #: widgets.py:682
 msgid "Press key to record, or click Cancel"
 msgstr ""
 
-#: plugins/dbg.py:394 widgets.py:685 widgets.py:703
+#: plugins/dbg.py:419 widgets.py:685 widgets.py:703
 msgid "OK"
 msgstr ""
 
 #: widgets.py:686 widgets.py:729
 msgid "Cancel"
 msgstr ""
 
@@ -338,15 +337,15 @@
 msgid "Input"
 msgstr ""
 
 #: conn/conn_ssh.py:215
 msgid "error"
 msgstr ""
 
-#: conn/conn_ssh.py:234 plugins/dbg.py:425
+#: conn/conn_ssh.py:234 plugins/dbg.py:450
 msgid "All Files (*)"
 msgstr ""
 
 #: conn/conn_ssh.py:288 conn/conn_tcp_udp.py:402
 msgid "Connect Failed"
 msgstr ""
 
@@ -446,204 +445,222 @@
 msgid "Clear Send Area"
 msgstr ""
 
 #: plugins/dbg.py:72
 msgid "Clear Receive Area"
 msgstr ""
 
-#: plugins/dbg.py:146
+#: plugins/dbg.py:149
 msgid "Receive Settings"
 msgstr ""
 
-#: plugins/dbg.py:147 plugins/dbg.py:176 plugins/protocol.py:261
+#: plugins/dbg.py:150 plugins/dbg.py:182 plugins/protocol.py:261
 msgid "ASCII"
 msgstr ""
 
-#: plugins/dbg.py:148
+#: plugins/dbg.py:151
 msgid ""
 "Show recived data as visible format, select decode method at top right "
 "corner"
 msgstr ""
 
-#: plugins/dbg.py:149 plugins/dbg.py:177 plugins/protocol.py:262
+#: plugins/dbg.py:152 plugins/dbg.py:183 plugins/protocol.py:262
 msgid "HEX"
 msgstr ""
 
-#: plugins/dbg.py:150
+#: plugins/dbg.py:153
 msgid "Show recived data as hex format"
 msgstr ""
 
-#: plugins/dbg.py:152
+#: plugins/dbg.py:155
 #, fuzzy
 msgid ""
 "Auto\n"
 "Linefeed\n"
 "ms"
 msgstr ""
 "Auto\n"
 "Linefeed\n"
 "ms"
 
-#: plugins/dbg.py:153 plugins/dbg.py:156
+#: plugins/dbg.py:156 plugins/dbg.py:159
 msgid "Auto linefeed after interval, unit: ms"
 msgstr ""
 
-#: plugins/dbg.py:159
+#: plugins/dbg.py:162
 msgid "Timestamp"
 msgstr ""
 
-#: plugins/dbg.py:160
+#: plugins/dbg.py:163
 msgid ""
 "Add timestamp before received data, will automatically enable auto line "
 "feed"
 msgstr ""
 
-#: plugins/dbg.py:161
+#: plugins/dbg.py:164
 msgid "Color"
 msgstr ""
 
-#: plugins/dbg.py:162
+#: plugins/dbg.py:165
 msgid "Enable unix terminal color support, e.g. \\33[31;43mhello\\33[0m"
 msgstr ""
 
-#: plugins/dbg.py:175
+#: plugins/dbg.py:166
+msgid "Display wrap"
+msgstr ""
+
+#: plugins/dbg.py:167
+msgid ""
+"When content in a line is too long, always auto wrap to show, and no "
+"scroll bar"
+msgstr ""
+
+#: plugins/dbg.py:181
 msgid "Send Settings"
 msgstr ""
 
-#: plugins/dbg.py:178 plugins/protocol.py:263
+#: plugins/dbg.py:184 plugins/protocol.py:263
 msgid ""
 "Get send data as visible format, select encoding method at top right "
 "corner"
 msgstr ""
 
-#: plugins/dbg.py:179 plugins/protocol.py:264
+#: plugins/dbg.py:185 plugins/protocol.py:264
 msgid "Get send data as hex format, e.g. hex '31 32 33' equal to ascii '123'"
 msgstr ""
 
-#: plugins/dbg.py:181
+#: plugins/dbg.py:187
 msgid ""
 "Timed Send\n"
 "ms"
 msgstr ""
 
-#: plugins/dbg.py:182 plugins/dbg.py:185
+#: plugins/dbg.py:188 plugins/dbg.py:191
 msgid "Timed send, unit: ms"
 msgstr ""
 
-#: plugins/dbg.py:188 plugins/protocol.py:266
+#: plugins/dbg.py:194 plugins/protocol.py:266
 msgid "<CRLF>"
 msgstr ""
 
-#: plugins/dbg.py:189 plugins/protocol.py:267
+#: plugins/dbg.py:195 plugins/protocol.py:267
 msgid "Select to send \\r\\n instead of \\n"
 msgstr ""
 
-#: plugins/dbg.py:192
+#: plugins/dbg.py:198
 msgid "Record send data"
 msgstr ""
 
-#: plugins/dbg.py:193 plugins/protocol.py:269
+#: plugins/dbg.py:199 plugins/protocol.py:269
 msgid "Escape"
 msgstr ""
 
-#: plugins/dbg.py:194 plugins/protocol.py:270
+#: plugins/dbg.py:200 plugins/protocol.py:270
 msgid "Enable escape characters support like \\t \\r \\n \\x01 \\001"
 msgstr ""
 
-#: plugins/dbg.py:195
+#: plugins/dbg.py:201
 msgid "Newline"
 msgstr ""
 
-#: plugins/dbg.py:196
+#: plugins/dbg.py:202
 msgid "Auto add new line when send"
 msgstr ""
 
-#: plugins/dbg.py:224
+#: plugins/dbg.py:230
 msgid "Auto line feed value error, must be integer"
 msgstr ""
 
-#: plugins/dbg.py:225
+#: plugins/dbg.py:231
 msgid "Timed send value error, must be integer"
 msgstr ""
 
-#: plugins/dbg.py:235
+#: plugins/dbg.py:242
 msgid "Open File"
 msgstr ""
 
-#: plugins/dbg.py:236
+#: plugins/dbg.py:243
 msgid "Send File"
 msgstr ""
 
-#: plugins/dbg.py:237
+#: plugins/dbg.py:244
 msgid "Clear History"
 msgstr ""
 
-#: plugins/dbg.py:240
+#: plugins/dbg.py:247
 msgid "Sendding File"
 msgstr ""
 
-#: plugins/dbg.py:246
+#: plugins/dbg.py:253
 msgid "Save log"
 msgstr ""
 
-#: plugins/dbg.py:249
+#: plugins/dbg.py:256
 msgid "Cutom send"
 msgstr ""
 
-#: plugins/dbg.py:280
+#: plugins/dbg.py:288
 msgid "Log path"
 msgstr ""
 
-#: plugins/dbg.py:366
+#: plugins/dbg.py:289
+msgid "Auto new file"
+msgstr ""
+
+#: plugins/dbg.py:290
+msgid "When start a new connection, will automatically create a new log file"
+msgstr ""
+
+#: plugins/dbg.py:384
 msgid "linefeed always on if timestamp or record send is on"
 msgstr ""
 
-#: plugins/dbg.py:394
+#: plugins/dbg.py:419
 msgid "History cleared!"
 msgstr ""
 
-#: plugins/dbg.py:401 plugins/graph.py:205 plugins/protocol.py:489
+#: plugins/dbg.py:426 plugins/graph.py:205 plugins/protocol.py:489
 msgid "Send data failed!"
 msgstr ""
 
-#: plugins/dbg.py:406
+#: plugins/dbg.py:431
 msgid "Send file"
 msgstr ""
 
-#: plugins/dbg.py:410
+#: plugins/dbg.py:435
 msgid "Send file failed!"
 msgstr ""
 
-#: plugins/dbg.py:439
+#: plugins/dbg.py:464
 msgid "Log file (*.log);;txt file (*.txt);;All Files (*)"
 msgstr ""
 
-#: plugins/dbg.py:531
+#: plugins/dbg.py:574
 msgid ""
 "File path error\n"
 "path"
 msgstr ""
 
-#: plugins/dbg.py:534
+#: plugins/dbg.py:577
 msgid "Connect first please"
 msgstr ""
 
-#: plugins/dbg.py:537
+#: plugins/dbg.py:580
 msgid "Sending file"
 msgstr ""
 
-#: plugins/dbg.py:548
+#: plugins/dbg.py:591
 msgid "Time format error"
 msgstr ""
 
-#: plugins/dbg.py:605
+#: plugins/dbg.py:648
 msgid "Send Error"
 msgstr ""
 
-#: plugins/dbg.py:613
+#: plugins/dbg.py:656
 msgid "get data error"
 msgstr ""
 
 #: plugins/graph.py:48
 msgid "Graph"
 msgstr ""
 
@@ -689,15 +706,14 @@
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:309
 msgid "AT+ISP=0\\r"
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:310 plugins/myplugin.py:43
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:51
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:51
 msgid "Send"
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:315
 msgid "ISP"
 msgstr ""
@@ -783,15 +799,14 @@
 msgstr ""
 
 #: plugins/myplugin.py:22
 msgid "my plugin"
 msgstr ""
 
 #: plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 msgid "Input data first please"
 msgstr ""
 
 #: plugins/protocol.py:58
 msgid "protocol"
 msgstr ""
@@ -857,15 +872,14 @@
 msgid "Please select a code profile name first to delete"
 msgstr ""
 
 #: plugins/terminal.py:674
 msgid "terminal"
 msgstr ""
 
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:30
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:30
 msgid "my plugin2"
 msgstr ""
 
 #~ msgid "Pack date:"
 #~ msgstr ""
```

### Comparing `COMTool-3.1.2/COMTool/locales/ja/LC_MESSAGES/messages.mo` & `COMTool-3.2.0/COMTool/locales/ja/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "<CRLF>"
 msgstr "<CRLF>"
 
 msgid "ASCII"
 msgstr "ASCII"
 
@@ -41,14 +41,17 @@
 
 msgid "Auto line feed value error, must be integer"
 msgstr "自動改行値エラー、整数である必要があります"
 
 msgid "Auto linefeed after interval, unit: ms"
 msgstr "超オーバー・トタイム時自PP换行、単位：ms"
 
+msgid "Auto new file"
+msgstr "自動新規ファイル"
+
 msgid "Baudrate"
 msgstr "ボーレート"
 
 msgid "CLOSE"
 msgstr "関闭"
 
 msgid "COMTool is a Open source project create by"
@@ -301,14 +304,17 @@
 
 msgid "Warning"
 msgstr "警告"
 
 msgid "Welcome to improve it together and add plugins"
 msgstr "一緒に改善することを歓迎します"
 
+msgid "When start a new connection, will automatically create a new log file"
+msgstr "新しい接続を開始すると、自動的に新しいログファイルが作成されます"
+
 msgid "You can buy me half a cup of coffee if this software helpes you"
 msgstr "このソフトウェアを使っていただくと、私に半つのコーヒーを買います"
 
 msgid "and get latest version at"
 msgstr "最新版はこちら"
 
 msgid "bytes"
```

### Comparing `COMTool-3.1.2/COMTool/locales/ja/LC_MESSAGES/messages.po` & `COMTool-3.2.0/COMTool/locales/ja/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 #: helpAbout.py:40
 msgid "Config path"
 msgstr "設定ファイルのパス"
 
 #: helpAbout.py:42
 msgid "Old config backup in"
@@ -66,19 +66,18 @@
 msgid "Load plugin from file"
 msgstr "ファイルからプラグインを読み込む"
 
 #: conn/conn_serial.py:331 conn/conn_ssh.py:289 conn/conn_tcp_udp.py:403
 #: main2.py:229 main2.py:279 main2.py:422 main2.py:427 main2.py:723
 #: pluginItems.py:169 pluginItems.py:172 pluginItems.py:273 pluginItems.py:285
 #: plugins/base.py:165 plugins/base.py:170 plugins/base.py:186
-#: plugins/base.py:195 plugins/dbg.py:401 plugins/dbg.py:410 plugins/dbg.py:531
-#: plugins/dbg.py:548 plugins/dbg.py:605 plugins/dbg.py:613
+#: plugins/base.py:195 plugins/dbg.py:426 plugins/dbg.py:435 plugins/dbg.py:574
+#: plugins/dbg.py:591 plugins/dbg.py:648 plugins/dbg.py:656
 #: plugins/graph.py:205 plugins/graph_widget_metasenselite.py:591
 #: plugins/graph_widgets.py:141 plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/protocol.py:466 plugins/protocol.py:480 plugins/protocol.py:489
 #: plugins/protocol.py:552
 msgid "Error"
 msgstr "間違い"
 
 #: main2.py:229
@@ -87,15 +86,15 @@
 msgstr "プラグインの読み込みに失敗しました"
 
 #: main2.py:250
 msgid "Load plugin fail"
 msgstr "プラグインの読み込みに失敗しました"
 
 #: conn/conn_ssh.py:232 main2.py:273 pluginItems.py:149 pluginItems.py:162
-#: plugins/dbg.py:423 plugins/dbg.py:437
+#: plugins/dbg.py:448 plugins/dbg.py:462
 msgid "Select file"
 msgstr "ファイルを選択"
 
 #: main2.py:275
 msgid "python script (*.py)"
 msgstr "Python スクリプト (*.py)"
 
@@ -169,15 +168,15 @@
 "to "
 msgstr ""
 
 #: pluginItems.py:172
 msgid "Config is not for this plugin, config is for plugin:"
 msgstr ""
 
-#: pluginItems.py:175 plugins/dbg.py:366 plugins/dbg.py:534
+#: pluginItems.py:175 plugins/dbg.py:384 plugins/dbg.py:577
 #: plugins/protocol.py:574 plugins/protocol.py:596
 msgid "Warning"
 msgstr "警告"
 
 #: pluginItems.py:176
 msgid "Config version not same, plugin config version:"
 msgstr ""
@@ -216,15 +215,15 @@
 msgid "Help"
 msgstr ""
 
 #: widgets.py:661
 msgid "Input remark"
 msgstr ""
 
-#: plugins/dbg.py:191 widgets.py:671 widgets.py:742
+#: plugins/dbg.py:197 widgets.py:671 widgets.py:742
 msgid "Record"
 msgstr "記録"
 
 #: widgets.py:676
 msgid "Input value"
 msgstr ""
 
@@ -238,15 +237,15 @@
 msgid "Shortcut"
 msgstr "ホットキー："
 
 #: widgets.py:682
 msgid "Press key to record, or click Cancel"
 msgstr ""
 
-#: plugins/dbg.py:394 widgets.py:685 widgets.py:703
+#: plugins/dbg.py:419 widgets.py:685 widgets.py:703
 msgid "OK"
 msgstr ""
 
 #: widgets.py:686 widgets.py:729
 msgid "Cancel"
 msgstr ""
 
@@ -341,15 +340,15 @@
 msgid "Input"
 msgstr "入力"
 
 #: conn/conn_ssh.py:215
 msgid "error"
 msgstr "エラー"
 
-#: conn/conn_ssh.py:234 plugins/dbg.py:425
+#: conn/conn_ssh.py:234 plugins/dbg.py:450
 msgid "All Files (*)"
 msgstr "すべてのファイル (*)"
 
 #: conn/conn_ssh.py:288 conn/conn_tcp_udp.py:402
 #, fuzzy
 msgid "Connect Failed"
 msgstr "最初に接続してください"
@@ -459,211 +458,229 @@
 msgid "Clear Send Area"
 msgstr "送信エリアをクリアする"
 
 #: plugins/dbg.py:72
 msgid "Clear Receive Area"
 msgstr "清除接収区"
 
-#: plugins/dbg.py:146
+#: plugins/dbg.py:149
 msgid "Receive Settings"
 msgstr "受信設定"
 
-#: plugins/dbg.py:147 plugins/dbg.py:176 plugins/protocol.py:261
+#: plugins/dbg.py:150 plugins/dbg.py:182 plugins/protocol.py:261
 msgid "ASCII"
 msgstr "ASCII"
 
-#: plugins/dbg.py:148
+#: plugins/dbg.py:151
 msgid ""
 "Show recived data as visible format, select decode method at top right "
 "corner"
 msgstr "表示されている文字を使用して受信データを表示し、右上隅でデコード方法を選択します"
 
-#: plugins/dbg.py:149 plugins/dbg.py:177 plugins/protocol.py:262
+#: plugins/dbg.py:152 plugins/dbg.py:183 plugins/protocol.py:262
 msgid "HEX"
 msgstr "HEX"
 
-#: plugins/dbg.py:150
+#: plugins/dbg.py:153
 msgid "Show recived data as hex format"
 msgstr "16進表記を使用して受信データを表示します"
 
-#: plugins/dbg.py:152
+#: plugins/dbg.py:155
 msgid ""
 "Auto\n"
 "Linefeed\n"
 "ms"
 msgstr ""
 "自動\n"
 "ラインフィード\n"
 "ms"
 
-#: plugins/dbg.py:153 plugins/dbg.py:156
+#: plugins/dbg.py:156 plugins/dbg.py:159
 msgid "Auto linefeed after interval, unit: ms"
 msgstr "超オーバー・トタイム時自PP换行、単位：ms"
 
-#: plugins/dbg.py:159
+#: plugins/dbg.py:162
 msgid "Timestamp"
 msgstr "タイムスタンプ"
 
-#: plugins/dbg.py:160
+#: plugins/dbg.py:163
 msgid ""
 "Add timestamp before received data, will automatically enable auto line "
 "feed"
 msgstr "受信データの前にタイムスタンプを追加すると、自動改行が自動的に有効になります"
 
-#: plugins/dbg.py:161
+#: plugins/dbg.py:164
 msgid "Color"
 msgstr "顔色"
 
-#: plugins/dbg.py:162
+#: plugins/dbg.py:165
 msgid "Enable unix terminal color support, e.g. \\33[31;43mhello\\33[0m"
 msgstr "UNIX端末の色のサポートを有効にする, 例えば \\33[31;43mhello\\33[0m"
 
-#: plugins/dbg.py:175
+#: plugins/dbg.py:166
+msgid "Display wrap"
+msgstr ""
+
+#: plugins/dbg.py:167
+msgid ""
+"When content in a line is too long, always auto wrap to show, and no "
+"scroll bar"
+msgstr ""
+
+#: plugins/dbg.py:181
 msgid "Send Settings"
 msgstr "送信設定"
 
-#: plugins/dbg.py:178 plugins/protocol.py:263
+#: plugins/dbg.py:184 plugins/protocol.py:263
 msgid ""
 "Get send data as visible format, select encoding method at top right "
 "corner"
 msgstr "表示文字形式で送信するデータを取得し、右上隅でエンコード方法を選択します"
 
-#: plugins/dbg.py:179 plugins/protocol.py:264
+#: plugins/dbg.py:185 plugins/protocol.py:264
 msgid "Get send data as hex format, e.g. hex '31 32 33' equal to ascii '123'"
 msgstr "16進数の「313233」などの16進数形式で送信するデータを取得し、ASCIIコードの「123」は同等です。"
 
-#: plugins/dbg.py:181
+#: plugins/dbg.py:187
 msgid ""
 "Timed Send\n"
 "ms"
 msgstr ""
 "時限送信\n"
 "ms"
 
-#: plugins/dbg.py:182 plugins/dbg.py:185
+#: plugins/dbg.py:188 plugins/dbg.py:191
 msgid "Timed send, unit: ms"
 msgstr "定時間P送、単位：ms"
 
-#: plugins/dbg.py:188 plugins/protocol.py:266
+#: plugins/dbg.py:194 plugins/protocol.py:266
 msgid "<CRLF>"
 msgstr "<CRLF>"
 
-#: plugins/dbg.py:189 plugins/protocol.py:267
+#: plugins/dbg.py:195 plugins/protocol.py:267
 msgid "Select to send \\r\\n instead of \\n"
 msgstr "選択中ρ送信\\ r \\ n圧電不是\\ n"
 
-#: plugins/dbg.py:192
+#: plugins/dbg.py:198
 msgid "Record send data"
 msgstr "送信データを記録する"
 
-#: plugins/dbg.py:193 plugins/protocol.py:269
+#: plugins/dbg.py:199 plugins/protocol.py:269
 msgid "Escape"
 msgstr "エスケープ"
 
-#: plugins/dbg.py:194 plugins/protocol.py:270
+#: plugins/dbg.py:200 plugins/protocol.py:270
 msgid "Enable escape characters support like \\t \\r \\n \\x01 \\001"
 msgstr "\\t \\r \\n \\x01 \\001 のようなエスケープ文字のサポートを有効にする"
 
-#: plugins/dbg.py:195
+#: plugins/dbg.py:201
 msgid "Newline"
 msgstr ""
 
-#: plugins/dbg.py:196
+#: plugins/dbg.py:202
 msgid "Auto add new line when send"
 msgstr ""
 
-#: plugins/dbg.py:224
+#: plugins/dbg.py:230
 msgid "Auto line feed value error, must be integer"
 msgstr "自動改行値エラー、整数である必要があります"
 
-#: plugins/dbg.py:225
+#: plugins/dbg.py:231
 msgid "Timed send value error, must be integer"
 msgstr "時限送信値エラー。整数である必要があります"
 
-#: plugins/dbg.py:235
+#: plugins/dbg.py:242
 msgid "Open File"
 msgstr "打開き文件"
 
-#: plugins/dbg.py:236
+#: plugins/dbg.py:243
 msgid "Send File"
 msgstr "ファイルを送信"
 
-#: plugins/dbg.py:237
+#: plugins/dbg.py:244
 msgid "Clear History"
 msgstr "履歴のクリア"
 
-#: plugins/dbg.py:240
+#: plugins/dbg.py:247
 msgid "Sendding File"
 msgstr "ファイルの送信"
 
-#: plugins/dbg.py:246
+#: plugins/dbg.py:253
 msgid "Save log"
 msgstr "ログを保存"
 
-#: plugins/dbg.py:249
+#: plugins/dbg.py:256
 msgid "Cutom send"
 msgstr "カスタム送信"
 
-#: plugins/dbg.py:280
+#: plugins/dbg.py:288
 msgid "Log path"
 msgstr "ログパス"
 
-#: plugins/dbg.py:366
+#: plugins/dbg.py:289
+msgid "Auto new file"
+msgstr "自動新規ファイル"
+
+#: plugins/dbg.py:290
+msgid "When start a new connection, will automatically create a new log file"
+msgstr "新しい接続を開始すると、自動的に新しいログファイルが作成されます"
+
+#: plugins/dbg.py:384
 msgid "linefeed always on if timestamp or record send is on"
 msgstr "タイムスタンプまたはレコード送信がオンの場合、改行は常にオンになります"
 
-#: plugins/dbg.py:394
+#: plugins/dbg.py:419
 msgid "History cleared!"
 msgstr "履歴がクリアされました！"
 
-#: plugins/dbg.py:401 plugins/graph.py:205 plugins/protocol.py:489
+#: plugins/dbg.py:426 plugins/graph.py:205 plugins/protocol.py:489
 #, fuzzy
 msgid "Send data failed!"
 msgstr "ファイルを開くことができませんでした！"
 
-#: plugins/dbg.py:406
+#: plugins/dbg.py:431
 #, fuzzy
 msgid "Send file"
 msgstr "ファイルを送信"
 
-#: plugins/dbg.py:410
+#: plugins/dbg.py:435
 #, fuzzy
 msgid "Send file failed!"
 msgstr "ファイルを開くことができませんでした！"
 
-#: plugins/dbg.py:439
+#: plugins/dbg.py:464
 msgid "Log file (*.log);;txt file (*.txt);;All Files (*)"
 msgstr ""
 
-#: plugins/dbg.py:531
+#: plugins/dbg.py:574
 msgid ""
 "File path error\n"
 "path"
 msgstr ""
 "ファイルパスエラー\n"
 "ファイルパス"
 
-#: plugins/dbg.py:534
+#: plugins/dbg.py:577
 msgid "Connect first please"
 msgstr "最初に接続してください"
 
-#: plugins/dbg.py:537
+#: plugins/dbg.py:580
 #, fuzzy
 msgid "Sending file"
 msgstr "ファイルの送信"
 
-#: plugins/dbg.py:548
+#: plugins/dbg.py:591
 msgid "Time format error"
 msgstr "タイムフォーマットエラー"
 
-#: plugins/dbg.py:605
+#: plugins/dbg.py:648
 msgid "Send Error"
 msgstr "エラーの送信"
 
-#: plugins/dbg.py:613
+#: plugins/dbg.py:656
 #, fuzzy
 msgid "get data error"
 msgstr "タイムフォーマットエラー"
 
 #: plugins/graph.py:48
 msgid "Graph"
 msgstr ""
@@ -711,15 +728,14 @@
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:309
 msgid "AT+ISP=0\\r"
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:310 plugins/myplugin.py:43
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:51
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:51
 #, fuzzy
 msgid "Send"
 msgstr "クローズ"
 
 #: plugins/graph_widget_metasenselite.py:315
 msgid "ISP"
@@ -809,15 +825,14 @@
 msgstr ""
 
 #: plugins/myplugin.py:22
 msgid "my plugin"
 msgstr ""
 
 #: plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 #, fuzzy
 msgid "Input data first please"
 msgstr "最初に接続してください"
 
 #: plugins/protocol.py:58
 msgid "protocol"
@@ -890,15 +905,14 @@
 msgid "Please select a code profile name first to delete"
 msgstr ""
 
 #: plugins/terminal.py:674
 msgid "terminal"
 msgstr ""
 
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:30
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:30
 msgid "my plugin2"
 msgstr ""
 
 #~ msgid "Send"
 #~ msgstr "送信"
```

### Comparing `COMTool-3.1.2/COMTool/locales/zh_CN/LC_MESSAGES/messages.mo` & `COMTool-3.2.0/COMTool/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: https://github.com/Neutree/COMTool/issues\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "<CRLF>"
 msgstr "<CRLF>"
 
 msgid "ASCII"
 msgstr "ASCII"
 
@@ -43,14 +43,17 @@
 
 msgid "Auto line feed value error, must be integer"
 msgstr "自动换行值错误，必须是整数"
 
 msgid "Auto linefeed after interval, unit: ms"
 msgstr "超过这个时间自动换行，单位：ms"
 
+msgid "Auto new file"
+msgstr "自动新建文件"
+
 msgid "Auto reconnect"
 msgstr "自动重连"
 
 msgid "Baudrate"
 msgstr "波特率"
 
 msgid "CLOSE"
@@ -151,14 +154,17 @@
 
 msgid "Delete"
 msgstr "删除"
 
 msgid "Disconnect"
 msgstr "断开连接"
 
+msgid "Display wrap"
+msgstr "显示换行"
+
 msgid "Double click graph item to add a graph widget"
 msgstr "双击图表项以添加一个图表控件"
 
 msgid "Double click to add a graph widget"
 msgstr "双击以添加一个图表控件"
 
 msgid "En-decoding settings"
@@ -517,14 +523,22 @@
 
 msgid "Warning"
 msgstr "警告"
 
 msgid "Welcome to improve it together and add plugins"
 msgstr "欢迎一起改进以及编写插件"
 
+msgid ""
+"When content in a line is too long, always auto wrap to show, and no scroll "
+"bar"
+msgstr "当一行的内容太长时，总是自动换行显示，不会产生横向滚动条"
+
+msgid "When start a new connection, will automatically create a new log file"
+msgstr "每次连接成功时，会自动新建一个日志文件"
+
 msgid "You can buy me half a cup of coffee if this software helpes you"
 msgstr "如果有帮助到你，可以赏半杯咖啡"
 
 msgid "and get latest version at"
 msgstr "在此获取最新版本："
 
 msgid "bytes"
```

### Comparing `COMTool-3.1.2/COMTool/locales/zh_CN/LC_MESSAGES/messages.po` & `COMTool-3.2.0/COMTool/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: https://github.com/Neutree/COMTool/issues\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 #: helpAbout.py:40
 msgid "Config path"
 msgstr "配置路径"
 
 #: helpAbout.py:42
 msgid "Old config backup in"
@@ -66,19 +66,18 @@
 msgid "Load plugin from file"
 msgstr "从文件加载插件"
 
 #: conn/conn_serial.py:331 conn/conn_ssh.py:289 conn/conn_tcp_udp.py:403
 #: main2.py:229 main2.py:279 main2.py:422 main2.py:427 main2.py:723
 #: pluginItems.py:169 pluginItems.py:172 pluginItems.py:273 pluginItems.py:285
 #: plugins/base.py:165 plugins/base.py:170 plugins/base.py:186
-#: plugins/base.py:195 plugins/dbg.py:401 plugins/dbg.py:410 plugins/dbg.py:531
-#: plugins/dbg.py:548 plugins/dbg.py:605 plugins/dbg.py:613
+#: plugins/base.py:195 plugins/dbg.py:426 plugins/dbg.py:435 plugins/dbg.py:574
+#: plugins/dbg.py:591 plugins/dbg.py:648 plugins/dbg.py:656
 #: plugins/graph.py:205 plugins/graph_widget_metasenselite.py:591
 #: plugins/graph_widgets.py:141 plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/protocol.py:466 plugins/protocol.py:480 plugins/protocol.py:489
 #: plugins/protocol.py:552
 msgid "Error"
 msgstr "错误"
 
 #: main2.py:229
@@ -86,15 +85,15 @@
 msgstr "加载插件失败"
 
 #: main2.py:250
 msgid "Load plugin fail"
 msgstr "加载插件失败"
 
 #: conn/conn_ssh.py:232 main2.py:273 pluginItems.py:149 pluginItems.py:162
-#: plugins/dbg.py:423 plugins/dbg.py:437
+#: plugins/dbg.py:448 plugins/dbg.py:462
 msgid "Select file"
 msgstr "选择文件"
 
 #: main2.py:275
 msgid "python script (*.py)"
 msgstr "python 脚本 (*.py)"
 
@@ -168,15 +167,15 @@
 "to "
 msgstr "不支持加载全局配置，你可以手动拷贝文件到 "
 
 #: pluginItems.py:172
 msgid "Config is not for this plugin, config is for plugin:"
 msgstr "配置不是这个插件的，配置是这个插件的: "
 
-#: pluginItems.py:175 plugins/dbg.py:366 plugins/dbg.py:534
+#: pluginItems.py:175 plugins/dbg.py:384 plugins/dbg.py:577
 #: plugins/protocol.py:574 plugins/protocol.py:596
 msgid "Warning"
 msgstr "警告"
 
 #: pluginItems.py:176
 msgid "Config version not same, plugin config version:"
 msgstr "配置版本不同，插件配置版本:"
@@ -215,15 +214,15 @@
 msgid "Help"
 msgstr "帮助"
 
 #: widgets.py:661
 msgid "Input remark"
 msgstr "输入标记"
 
-#: plugins/dbg.py:191 widgets.py:671 widgets.py:742
+#: plugins/dbg.py:197 widgets.py:671 widgets.py:742
 msgid "Record"
 msgstr "记录"
 
 #: widgets.py:676
 msgid "Input value"
 msgstr "输入值"
 
@@ -235,15 +234,15 @@
 msgid "Shortcut"
 msgstr "快捷键"
 
 #: widgets.py:682
 msgid "Press key to record, or click Cancel"
 msgstr "按键以记录，或点击取消按钮"
 
-#: plugins/dbg.py:394 widgets.py:685 widgets.py:703
+#: plugins/dbg.py:419 widgets.py:685 widgets.py:703
 msgid "OK"
 msgstr "完成"
 
 #: widgets.py:686 widgets.py:729
 msgid "Cancel"
 msgstr "取消"
 
@@ -338,15 +337,15 @@
 msgid "Input"
 msgstr "输入"
 
 #: conn/conn_ssh.py:215
 msgid "error"
 msgstr "错误"
 
-#: conn/conn_ssh.py:234 plugins/dbg.py:425
+#: conn/conn_ssh.py:234 plugins/dbg.py:450
 msgid "All Files (*)"
 msgstr "所有文件 (*)"
 
 #: conn/conn_ssh.py:288 conn/conn_tcp_udp.py:402
 msgid "Connect Failed"
 msgstr "连接失败"
 
@@ -446,202 +445,220 @@
 msgid "Clear Send Area"
 msgstr "清除发送区"
 
 #: plugins/dbg.py:72
 msgid "Clear Receive Area"
 msgstr "清除接收区"
 
-#: plugins/dbg.py:146
+#: plugins/dbg.py:149
 msgid "Receive Settings"
 msgstr "接收设置"
 
-#: plugins/dbg.py:147 plugins/dbg.py:176 plugins/protocol.py:261
+#: plugins/dbg.py:150 plugins/dbg.py:182 plugins/protocol.py:261
 msgid "ASCII"
 msgstr "ASCII"
 
-#: plugins/dbg.py:148
+#: plugins/dbg.py:151
 msgid ""
 "Show recived data as visible format, select decode method at top right "
 "corner"
 msgstr "使用可见字符显示收到的数据，在右上角选择解码的方法"
 
-#: plugins/dbg.py:149 plugins/dbg.py:177 plugins/protocol.py:262
+#: plugins/dbg.py:152 plugins/dbg.py:183 plugins/protocol.py:262
 msgid "HEX"
 msgstr "HEX"
 
-#: plugins/dbg.py:150
+#: plugins/dbg.py:153
 msgid "Show recived data as hex format"
 msgstr "使用十六进制表示方法显示收到的数据"
 
-#: plugins/dbg.py:152
+#: plugins/dbg.py:155
 msgid ""
 "Auto\n"
 "Linefeed\n"
 "ms"
 msgstr "自动换行"
 
-#: plugins/dbg.py:153 plugins/dbg.py:156
+#: plugins/dbg.py:156 plugins/dbg.py:159
 msgid "Auto linefeed after interval, unit: ms"
 msgstr "超过这个时间自动换行，单位：ms"
 
-#: plugins/dbg.py:159
+#: plugins/dbg.py:162
 msgid "Timestamp"
 msgstr "时间戳"
 
-#: plugins/dbg.py:160
+#: plugins/dbg.py:163
 msgid ""
 "Add timestamp before received data, will automatically enable auto line "
 "feed"
 msgstr "在收到的数据前添加时间戳， 会自动使能自动换行"
 
-#: plugins/dbg.py:161
+#: plugins/dbg.py:164
 msgid "Color"
 msgstr "颜色"
 
-#: plugins/dbg.py:162
+#: plugins/dbg.py:165
 msgid "Enable unix terminal color support, e.g. \\33[31;43mhello\\33[0m"
 msgstr "使能 unix 终端颜色支持，比如：\\33[31;43mhello\\33[0m"
 
-#: plugins/dbg.py:175
+#: plugins/dbg.py:166
+msgid "Display wrap"
+msgstr "显示换行"
+
+#: plugins/dbg.py:167
+msgid ""
+"When content in a line is too long, always auto wrap to show, and no "
+"scroll bar"
+msgstr "当一行的内容太长时，总是自动换行显示，不会产生横向滚动条"
+
+#: plugins/dbg.py:181
 msgid "Send Settings"
 msgstr "发送设置"
 
-#: plugins/dbg.py:178 plugins/protocol.py:263
+#: plugins/dbg.py:184 plugins/protocol.py:263
 msgid ""
 "Get send data as visible format, select encoding method at top right "
 "corner"
 msgstr "以可见字符的方式获取将要发送的数据，在右上角选择编码的方法"
 
-#: plugins/dbg.py:179 plugins/protocol.py:264
+#: plugins/dbg.py:185 plugins/protocol.py:264
 msgid "Get send data as hex format, e.g. hex '31 32 33' equal to ascii '123'"
 msgstr "以十六进制的格式获取将要发送的数据，比如 十六进制的'31 32 33' 和 ascii编码的 '123' 等效"
 
-#: plugins/dbg.py:181
+#: plugins/dbg.py:187
 msgid ""
 "Timed Send\n"
 "ms"
 msgstr "定时发送"
 
-#: plugins/dbg.py:182 plugins/dbg.py:185
+#: plugins/dbg.py:188 plugins/dbg.py:191
 msgid "Timed send, unit: ms"
 msgstr "定时发送，单位：ms"
 
-#: plugins/dbg.py:188 plugins/protocol.py:266
+#: plugins/dbg.py:194 plugins/protocol.py:266
 msgid "<CRLF>"
 msgstr "<CRLF>"
 
-#: plugins/dbg.py:189 plugins/protocol.py:267
+#: plugins/dbg.py:195 plugins/protocol.py:267
 msgid "Select to send \\r\\n instead of \\n"
 msgstr "选中发送 \\r\\n 而不是 \\n"
 
-#: plugins/dbg.py:192
+#: plugins/dbg.py:198
 msgid "Record send data"
 msgstr "记录发送的数据"
 
-#: plugins/dbg.py:193 plugins/protocol.py:269
+#: plugins/dbg.py:199 plugins/protocol.py:269
 msgid "Escape"
 msgstr "转义符"
 
-#: plugins/dbg.py:194 plugins/protocol.py:270
+#: plugins/dbg.py:200 plugins/protocol.py:270
 msgid "Enable escape characters support like \\t \\r \\n \\x01 \\001"
 msgstr "使能转义字符支持，比如 \\t \\r \\n \\x01 \\001"
 
-#: plugins/dbg.py:195
+#: plugins/dbg.py:201
 msgid "Newline"
 msgstr "新行"
 
-#: plugins/dbg.py:196
+#: plugins/dbg.py:202
 msgid "Auto add new line when send"
 msgstr "发送时自动添加回车符"
 
-#: plugins/dbg.py:224
+#: plugins/dbg.py:230
 msgid "Auto line feed value error, must be integer"
 msgstr "自动换行值错误，必须是整数"
 
-#: plugins/dbg.py:225
+#: plugins/dbg.py:231
 msgid "Timed send value error, must be integer"
 msgstr "定时发送值错误，必须是整数"
 
-#: plugins/dbg.py:235
+#: plugins/dbg.py:242
 msgid "Open File"
 msgstr "打开文件"
 
-#: plugins/dbg.py:236
+#: plugins/dbg.py:243
 msgid "Send File"
 msgstr "发送文件"
 
-#: plugins/dbg.py:237
+#: plugins/dbg.py:244
 msgid "Clear History"
 msgstr "清除历史"
 
-#: plugins/dbg.py:240
+#: plugins/dbg.py:247
 msgid "Sendding File"
 msgstr "发送文件中"
 
-#: plugins/dbg.py:246
+#: plugins/dbg.py:253
 msgid "Save log"
 msgstr "保存日志"
 
-#: plugins/dbg.py:249
+#: plugins/dbg.py:256
 msgid "Cutom send"
 msgstr "自定义发送"
 
-#: plugins/dbg.py:280
+#: plugins/dbg.py:288
 msgid "Log path"
 msgstr "日志路径"
 
-#: plugins/dbg.py:366
+#: plugins/dbg.py:289
+msgid "Auto new file"
+msgstr "自动新建文件"
+
+#: plugins/dbg.py:290
+msgid "When start a new connection, will automatically create a new log file"
+msgstr "每次连接成功时，会自动新建一个日志文件"
+
+#: plugins/dbg.py:384
 msgid "linefeed always on if timestamp or record send is on"
 msgstr "当时间戳和记录发送时，自动换行需要打开"
 
-#: plugins/dbg.py:394
+#: plugins/dbg.py:419
 msgid "History cleared!"
 msgstr "历史已清除"
 
-#: plugins/dbg.py:401 plugins/graph.py:205 plugins/protocol.py:489
+#: plugins/dbg.py:426 plugins/graph.py:205 plugins/protocol.py:489
 msgid "Send data failed!"
 msgstr "发送数据失败！"
 
-#: plugins/dbg.py:406
+#: plugins/dbg.py:431
 msgid "Send file"
 msgstr "发送文件"
 
-#: plugins/dbg.py:410
+#: plugins/dbg.py:435
 msgid "Send file failed!"
 msgstr "发送文件失败！"
 
-#: plugins/dbg.py:439
+#: plugins/dbg.py:464
 msgid "Log file (*.log);;txt file (*.txt);;All Files (*)"
 msgstr "日志文件 (*.log);;文本文件 (*.txt);;所有文件 (*)"
 
-#: plugins/dbg.py:531
+#: plugins/dbg.py:574
 msgid ""
 "File path error\n"
 "path"
 msgstr ""
 "文件路径错误\n"
 "路径"
 
-#: plugins/dbg.py:534
+#: plugins/dbg.py:577
 msgid "Connect first please"
 msgstr "请先连接"
 
-#: plugins/dbg.py:537
+#: plugins/dbg.py:580
 msgid "Sending file"
 msgstr "发送文件中"
 
-#: plugins/dbg.py:548
+#: plugins/dbg.py:591
 msgid "Time format error"
 msgstr "时间格式错误"
 
-#: plugins/dbg.py:605
+#: plugins/dbg.py:648
 msgid "Send Error"
 msgstr "发送出错"
 
-#: plugins/dbg.py:613
+#: plugins/dbg.py:656
 msgid "get data error"
 msgstr "获取数据错误"
 
 #: plugins/graph.py:48
 msgid "Graph"
 msgstr "图表"
 
@@ -687,15 +704,14 @@
 msgstr "裸命令:"
 
 #: plugins/graph_widget_metasenselite.py:309
 msgid "AT+ISP=0\\r"
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:310 plugins/myplugin.py:43
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:51
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:51
 msgid "Send"
 msgstr "发送"
 
 #: plugins/graph_widget_metasenselite.py:315
 msgid "ISP"
 msgstr ""
@@ -784,15 +800,14 @@
 "协议示例代码参见帮助"
 
 #: plugins/myplugin.py:22
 msgid "my plugin"
 msgstr "我的插件"
 
 #: plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 msgid "Input data first please"
 msgstr "请先输入数据"
 
 #: plugins/protocol.py:58
 msgid "protocol"
 msgstr "协议"
@@ -858,15 +873,14 @@
 msgid "Please select a code profile name first to delete"
 msgstr "请先选择要删除的存档名"
 
 #: plugins/terminal.py:674
 msgid "terminal"
 msgstr "终端"
 
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:30
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:30
 msgid "my plugin2"
 msgstr "我的插件2"
 
 #~ msgid "Donate"
 #~ msgstr "捐献"
```

### Comparing `COMTool-3.1.2/COMTool/locales/zh_TW/LC_MESSAGES/messages.mo` & `COMTool-3.2.0/COMTool/locales/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hant_TW\n"
 "Language-Team: zh_Hant_TW <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "<CRLF>"
 msgstr "<CRLF>"
 
 msgid "ASCII"
 msgstr "ASCII"
 
@@ -43,14 +43,17 @@
 
 msgid "Auto line feed value error, must be integer"
 msgstr "自動換行值錯誤，必須是整數"
 
 msgid "Auto linefeed after interval, unit: ms"
 msgstr "超過這個時間自動換行，單位：ms"
 
+msgid "Auto new file"
+msgstr "自動新建文件"
+
 msgid "Auto reconnect"
 msgstr "自動重連"
 
 msgid "Baudrate"
 msgstr "波特率"
 
 msgid "CLOSE"
@@ -148,14 +151,17 @@
 
 msgid "Delete"
 msgstr "刪除"
 
 msgid "Disconnect"
 msgstr "斷開"
 
+msgid "Display wrap"
+msgstr "显示换行"
+
 msgid "En-decoding settings"
 msgstr "編解碼設置"
 
 msgid "Enable escape characters support like \\t \\r \\n \\x01 \\001"
 msgstr "使能轉義符支持，比如 \\t \\r \\n \\x01 \\001"
 
 msgid "Enable unix terminal color support, e.g. \\33[31;43mhello\\33[0m"
@@ -474,14 +480,22 @@
 
 msgid "Warning"
 msgstr "警告"
 
 msgid "Welcome to improve it together and add plugins"
 msgstr "歡迎您一起改進它，並加入插件"
 
+msgid ""
+"When content in a line is too long, always auto wrap to show, and no scroll "
+"bar"
+msgstr "当一行的内容太长时，总是自动换行显示，不会产生横向滚动条"
+
+msgid "When start a new connection, will automatically create a new log file"
+msgstr "当開始一個新的連接時，會自動創建一個新的日誌文件"
+
 msgid "You can buy me half a cup of coffee if this software helpes you"
 msgstr "如果這個軟件幫助您，我可以給您一杯咖啡"
 
 msgid "and get latest version at"
 msgstr "取得最新版本："
 
 msgid "bytes"
```

### Comparing `COMTool-3.1.2/COMTool/locales/zh_TW/LC_MESSAGES/messages.po` & `COMTool-3.2.0/COMTool/locales/zh_TW/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-27 22:05+0800\n"
+"POT-Creation-Date: 2022-11-29 15:00+0800\n"
 "PO-Revision-Date: 2021-12-04 15:20+0800\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hant_TW\n"
 "Language-Team: zh_Hant_TW <LL@li.org>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 #: helpAbout.py:40
 msgid "Config path"
 msgstr "配置路徑"
 
 #: helpAbout.py:42
 msgid "Old config backup in"
@@ -66,19 +66,18 @@
 msgid "Load plugin from file"
 msgstr "從檔案載入外掛程式"
 
 #: conn/conn_serial.py:331 conn/conn_ssh.py:289 conn/conn_tcp_udp.py:403
 #: main2.py:229 main2.py:279 main2.py:422 main2.py:427 main2.py:723
 #: pluginItems.py:169 pluginItems.py:172 pluginItems.py:273 pluginItems.py:285
 #: plugins/base.py:165 plugins/base.py:170 plugins/base.py:186
-#: plugins/base.py:195 plugins/dbg.py:401 plugins/dbg.py:410 plugins/dbg.py:531
-#: plugins/dbg.py:548 plugins/dbg.py:605 plugins/dbg.py:613
+#: plugins/base.py:195 plugins/dbg.py:426 plugins/dbg.py:435 plugins/dbg.py:574
+#: plugins/dbg.py:591 plugins/dbg.py:648 plugins/dbg.py:656
 #: plugins/graph.py:205 plugins/graph_widget_metasenselite.py:591
 #: plugins/graph_widgets.py:141 plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/protocol.py:466 plugins/protocol.py:480 plugins/protocol.py:489
 #: plugins/protocol.py:552
 msgid "Error"
 msgstr "錯誤"
 
 #: main2.py:229
@@ -86,15 +85,15 @@
 msgstr "載入外掛程式失敗"
 
 #: main2.py:250
 msgid "Load plugin fail"
 msgstr "載入外掛程式失敗"
 
 #: conn/conn_ssh.py:232 main2.py:273 pluginItems.py:149 pluginItems.py:162
-#: plugins/dbg.py:423 plugins/dbg.py:437
+#: plugins/dbg.py:448 plugins/dbg.py:462
 msgid "Select file"
 msgstr "選擇文件"
 
 #: main2.py:275
 msgid "python script (*.py)"
 msgstr "python 程式 (*.py)"
 
@@ -168,15 +167,15 @@
 "to "
 msgstr "不支持載入全局配置文件，您可以手動將配置文件複製到"
 
 #: pluginItems.py:172
 msgid "Config is not for this plugin, config is for plugin:"
 msgstr "配置文件不是此外掛程式的，配置文件是外掛程式："
 
-#: pluginItems.py:175 plugins/dbg.py:366 plugins/dbg.py:534
+#: pluginItems.py:175 plugins/dbg.py:384 plugins/dbg.py:577
 #: plugins/protocol.py:574 plugins/protocol.py:596
 msgid "Warning"
 msgstr "警告"
 
 #: pluginItems.py:176
 msgid "Config version not same, plugin config version:"
 msgstr "配置文件版本不同，外掛程式配置文件版本："
@@ -215,15 +214,15 @@
 msgid "Help"
 msgstr "幫助"
 
 #: widgets.py:661
 msgid "Input remark"
 msgstr "輸入備註"
 
-#: plugins/dbg.py:191 widgets.py:671 widgets.py:742
+#: plugins/dbg.py:197 widgets.py:671 widgets.py:742
 msgid "Record"
 msgstr "記錄"
 
 #: widgets.py:676
 msgid "Input value"
 msgstr ""
 
@@ -235,15 +234,15 @@
 msgid "Shortcut"
 msgstr "快捷鍵"
 
 #: widgets.py:682
 msgid "Press key to record, or click Cancel"
 msgstr "按下快捷鍵記錄，或者按取消"
 
-#: plugins/dbg.py:394 widgets.py:685 widgets.py:703
+#: plugins/dbg.py:419 widgets.py:685 widgets.py:703
 msgid "OK"
 msgstr "確定"
 
 #: widgets.py:686 widgets.py:729
 msgid "Cancel"
 msgstr "取消"
 
@@ -338,15 +337,15 @@
 msgid "Input"
 msgstr "輸入"
 
 #: conn/conn_ssh.py:215
 msgid "error"
 msgstr "錯誤"
 
-#: conn/conn_ssh.py:234 plugins/dbg.py:425
+#: conn/conn_ssh.py:234 plugins/dbg.py:450
 msgid "All Files (*)"
 msgstr "所有文件 (*)"
 
 #: conn/conn_ssh.py:288 conn/conn_tcp_udp.py:402
 msgid "Connect Failed"
 msgstr "連接失敗"
 
@@ -446,202 +445,220 @@
 msgid "Clear Send Area"
 msgstr "清除發送區"
 
 #: plugins/dbg.py:72
 msgid "Clear Receive Area"
 msgstr "清除接收區"
 
-#: plugins/dbg.py:146
+#: plugins/dbg.py:149
 msgid "Receive Settings"
 msgstr "接收設置"
 
-#: plugins/dbg.py:147 plugins/dbg.py:176 plugins/protocol.py:261
+#: plugins/dbg.py:150 plugins/dbg.py:182 plugins/protocol.py:261
 msgid "ASCII"
 msgstr "ASCII"
 
-#: plugins/dbg.py:148
+#: plugins/dbg.py:151
 msgid ""
 "Show recived data as visible format, select decode method at top right "
 "corner"
 msgstr "使用可見字符顯示收到的數據，在右上角選擇解碼的方法"
 
-#: plugins/dbg.py:149 plugins/dbg.py:177 plugins/protocol.py:262
+#: plugins/dbg.py:152 plugins/dbg.py:183 plugins/protocol.py:262
 msgid "HEX"
 msgstr "HEX"
 
-#: plugins/dbg.py:150
+#: plugins/dbg.py:153
 msgid "Show recived data as hex format"
 msgstr "使用十六進製表示方法顯示收到的數據"
 
-#: plugins/dbg.py:152
+#: plugins/dbg.py:155
 msgid ""
 "Auto\n"
 "Linefeed\n"
 "ms"
 msgstr "自動換行"
 
-#: plugins/dbg.py:153 plugins/dbg.py:156
+#: plugins/dbg.py:156 plugins/dbg.py:159
 msgid "Auto linefeed after interval, unit: ms"
 msgstr "超過這個時間自動換行，單位：ms"
 
-#: plugins/dbg.py:159
+#: plugins/dbg.py:162
 msgid "Timestamp"
 msgstr "時間戳"
 
-#: plugins/dbg.py:160
+#: plugins/dbg.py:163
 msgid ""
 "Add timestamp before received data, will automatically enable auto line "
 "feed"
 msgstr "在接收的數據前添加時間戳， 會自動使能自動換行"
 
-#: plugins/dbg.py:161
+#: plugins/dbg.py:164
 msgid "Color"
 msgstr "顏色"
 
-#: plugins/dbg.py:162
+#: plugins/dbg.py:165
 msgid "Enable unix terminal color support, e.g. \\33[31;43mhello\\33[0m"
 msgstr "使能 unix 終端樣式的顏色支持， 比如： \\33[31;43mhello\\33[0m"
 
-#: plugins/dbg.py:175
+#: plugins/dbg.py:166
+msgid "Display wrap"
+msgstr "显示换行"
+
+#: plugins/dbg.py:167
+msgid ""
+"When content in a line is too long, always auto wrap to show, and no "
+"scroll bar"
+msgstr "当一行的内容太长时，总是自动换行显示，不会产生横向滚动条"
+
+#: plugins/dbg.py:181
 msgid "Send Settings"
 msgstr "發送設置"
 
-#: plugins/dbg.py:178 plugins/protocol.py:263
+#: plugins/dbg.py:184 plugins/protocol.py:263
 msgid ""
 "Get send data as visible format, select encoding method at top right "
 "corner"
 msgstr "以可見字符的方式獲取將要發送的數據，在右上角選擇編碼的方法"
 
-#: plugins/dbg.py:179 plugins/protocol.py:264
+#: plugins/dbg.py:185 plugins/protocol.py:264
 msgid "Get send data as hex format, e.g. hex '31 32 33' equal to ascii '123'"
 msgstr "以十六進制的格式獲取將要發送的數據，比如 十六進制的'31 32 33' 和 ascii編碼的 '123' 等效"
 
-#: plugins/dbg.py:181
+#: plugins/dbg.py:187
 msgid ""
 "Timed Send\n"
 "ms"
 msgstr "定時發送"
 
-#: plugins/dbg.py:182 plugins/dbg.py:185
+#: plugins/dbg.py:188 plugins/dbg.py:191
 msgid "Timed send, unit: ms"
 msgstr "定時發送，單位：ms"
 
-#: plugins/dbg.py:188 plugins/protocol.py:266
+#: plugins/dbg.py:194 plugins/protocol.py:266
 msgid "<CRLF>"
 msgstr "<CRLF>"
 
-#: plugins/dbg.py:189 plugins/protocol.py:267
+#: plugins/dbg.py:195 plugins/protocol.py:267
 msgid "Select to send \\r\\n instead of \\n"
 msgstr "選中發出通知\\r\\n不是\\n"
 
-#: plugins/dbg.py:192
+#: plugins/dbg.py:198
 msgid "Record send data"
 msgstr "記錄發送的數據"
 
-#: plugins/dbg.py:193 plugins/protocol.py:269
+#: plugins/dbg.py:199 plugins/protocol.py:269
 msgid "Escape"
 msgstr "轉義符"
 
-#: plugins/dbg.py:194 plugins/protocol.py:270
+#: plugins/dbg.py:200 plugins/protocol.py:270
 msgid "Enable escape characters support like \\t \\r \\n \\x01 \\001"
 msgstr "使能轉義符支持，比如 \\t \\r \\n \\x01 \\001"
 
-#: plugins/dbg.py:195
+#: plugins/dbg.py:201
 msgid "Newline"
 msgstr "新行"
 
-#: plugins/dbg.py:196
+#: plugins/dbg.py:202
 msgid "Auto add new line when send"
 msgstr "發送時自動添加新行"
 
-#: plugins/dbg.py:224
+#: plugins/dbg.py:230
 msgid "Auto line feed value error, must be integer"
 msgstr "自動換行值錯誤，必須是整數"
 
-#: plugins/dbg.py:225
+#: plugins/dbg.py:231
 msgid "Timed send value error, must be integer"
 msgstr "定時發送值錯誤，必須是整數"
 
-#: plugins/dbg.py:235
+#: plugins/dbg.py:242
 msgid "Open File"
 msgstr "打開文件"
 
-#: plugins/dbg.py:236
+#: plugins/dbg.py:243
 msgid "Send File"
 msgstr "發送文件"
 
-#: plugins/dbg.py:237
+#: plugins/dbg.py:244
 msgid "Clear History"
 msgstr "清除歷史"
 
-#: plugins/dbg.py:240
+#: plugins/dbg.py:247
 msgid "Sendding File"
 msgstr "發送文件中"
 
-#: plugins/dbg.py:246
+#: plugins/dbg.py:253
 msgid "Save log"
 msgstr "保存日誌"
 
-#: plugins/dbg.py:249
+#: plugins/dbg.py:256
 msgid "Cutom send"
 msgstr "自定義發送"
 
-#: plugins/dbg.py:280
+#: plugins/dbg.py:288
 msgid "Log path"
 msgstr "日誌路徑"
 
-#: plugins/dbg.py:366
+#: plugins/dbg.py:289
+msgid "Auto new file"
+msgstr "自動新建文件"
+
+#: plugins/dbg.py:290
+msgid "When start a new connection, will automatically create a new log file"
+msgstr "当開始一個新的連接時，會自動創建一個新的日誌文件"
+
+#: plugins/dbg.py:384
 msgid "linefeed always on if timestamp or record send is on"
 msgstr "當時間戳和發送記錄打開是，必須將自動換行也打開"
 
-#: plugins/dbg.py:394
+#: plugins/dbg.py:419
 msgid "History cleared!"
 msgstr "歷史已清除！"
 
-#: plugins/dbg.py:401 plugins/graph.py:205 plugins/protocol.py:489
+#: plugins/dbg.py:426 plugins/graph.py:205 plugins/protocol.py:489
 msgid "Send data failed!"
 msgstr "发送数据失敗"
 
-#: plugins/dbg.py:406
+#: plugins/dbg.py:431
 msgid "Send file"
 msgstr "發送文件"
 
-#: plugins/dbg.py:410
+#: plugins/dbg.py:435
 msgid "Send file failed!"
 msgstr "发送文件失敗"
 
-#: plugins/dbg.py:439
+#: plugins/dbg.py:464
 msgid "Log file (*.log);;txt file (*.txt);;All Files (*)"
 msgstr "日誌文件 (*.log);;文本文件 (*.txt);;所有文件 (*)"
 
-#: plugins/dbg.py:531
+#: plugins/dbg.py:574
 msgid ""
 "File path error\n"
 "path"
 msgstr ""
 "文件路徑錯誤\n"
 "路徑"
 
-#: plugins/dbg.py:534
+#: plugins/dbg.py:577
 msgid "Connect first please"
 msgstr "請先連接"
 
-#: plugins/dbg.py:537
+#: plugins/dbg.py:580
 msgid "Sending file"
 msgstr "發送文件中"
 
-#: plugins/dbg.py:548
+#: plugins/dbg.py:591
 msgid "Time format error"
 msgstr "時間格式錯誤"
 
-#: plugins/dbg.py:605
+#: plugins/dbg.py:648
 msgid "Send Error"
 msgstr "發送出錯"
 
-#: plugins/dbg.py:613
+#: plugins/dbg.py:656
 msgid "get data error"
 msgstr "獲取數據出錯"
 
 #: plugins/graph.py:48
 msgid "Graph"
 msgstr ""
 
@@ -687,15 +704,14 @@
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:309
 msgid "AT+ISP=0\\r"
 msgstr ""
 
 #: plugins/graph_widget_metasenselite.py:310 plugins/myplugin.py:43
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:51
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:51
 msgid "Send"
 msgstr "發送"
 
 #: plugins/graph_widget_metasenselite.py:315
 msgid "ISP"
 msgstr ""
@@ -781,15 +797,14 @@
 msgstr ""
 
 #: plugins/myplugin.py:22
 msgid "my plugin"
 msgstr ""
 
 #: plugins/myplugin.py:61
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:69
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:69
 msgid "Input data first please"
 msgstr "請先輸入數據"
 
 #: plugins/protocol.py:58
 msgid "protocol"
 msgstr "協議"
@@ -855,15 +870,14 @@
 msgid "Please select a code profile name first to delete"
 msgstr "請先選擇一個代碼配置名稱以刪除"
 
 #: plugins/terminal.py:674
 msgid "terminal"
 msgstr "終端"
 
-#: plugins/myplugin2/build/lib/comtool_plugin_myplugin2/myplugin2.py:30
 #: plugins/myplugin2/comtool_plugin_myplugin2/myplugin2.py:30
 msgid "my plugin2"
 msgstr ""
 
 #~ msgid "Send"
 #~ msgstr "發送"
```

### Comparing `COMTool-3.1.2/COMTool/logger.py` & `COMTool-3.2.0/COMTool/logger.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/main2.py` & `COMTool-3.2.0/COMTool/main2.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/parameters.py` & `COMTool-3.2.0/COMTool/parameters.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/pluginItems.py` & `COMTool-3.2.0/COMTool/pluginItems.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/base.py` & `COMTool-3.2.0/COMTool/plugins/base.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/crc.py` & `COMTool-3.2.0/COMTool/plugins/crc.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/dbg.py` & `COMTool-3.2.0/COMTool/plugins/dbg.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,33 +86,36 @@
             "sendScheduled" : False,
             "sendScheduledTime" : 300,
             "sendAutoNewline": False,
             "useCRLF" : True,
             "showTimestamp" : False,
             "recordSend" : False,
             "saveLogPath" : "",
+            "saveLogPath2" : "",
             "saveLog" : False,
+            "wrap": False,
+            "saveLogAutoNew": False,
             "color" : False,
             "sendEscape" : False,
             "customSendItems" : [],
             "sendHistoryList" : [],
         }
         for k in default:
             if not k in self.config:
                 self.config[k] = default[k]
+        self.lastShowTail = ''
+        self.justSent = False # sent data before received data flag
 
     def onWidgetMain(self, parent):
         self.mainWidget = QSplitter(Qt.Vertical)
         # widgets receive and send area
         self.receiveArea = QTextEdit()
         font = QFont('Menlo,Consolas,Bitstream Vera Sans Mono,Courier New,monospace, Microsoft YaHei', 10)
         self.receiveArea.setFont(font)
-        self.receiveArea.setLineWrapMode(QTextEdit.NoWrap)
         self.sendArea = QTextEdit()
-        self.sendArea.setLineWrapMode(QTextEdit.NoWrap)
         self.sendArea.setAcceptRichText(False)
         self.clearReceiveButtion = QPushButton("")
         utils_ui.setButtonIcon(self.clearReceiveButtion, "mdi6.broom")
         self.sendButton = QPushButton("")
         utils_ui.setButtonIcon(self.sendButton, "fa.send")
         self.sendHistory = ComboBox()
         sendWidget = QWidget()
@@ -156,20 +159,23 @@
         self.receiveSettingsAutoLinefeedTime.setToolTip(_("Auto linefeed after interval, unit: ms"))
         self.receiveSettingsAutoLinefeed.setMaximumWidth(75)
         self.receiveSettingsAutoLinefeedTime.setMaximumWidth(75)
         self.receiveSettingsTimestamp = QCheckBox(_("Timestamp"))
         self.receiveSettingsTimestamp.setToolTip(_("Add timestamp before received data, will automatically enable auto line feed"))
         self.receiveSettingsColor = QCheckBox(_("Color"))
         self.receiveSettingsColor.setToolTip(_("Enable unix terminal color support, e.g. \\33[31;43mhello\\33[0m"))
+        self.receiveSettingsWrap = QCheckBox(_("Display wrap"))
+        self.receiveSettingsWrap.setToolTip(_("When content in a line is too long, always auto wrap to show, and no scroll bar"))
         serialReceiveSettingsLayout.addWidget(self.receiveSettingsAscii,1,0,1,1)
         serialReceiveSettingsLayout.addWidget(self.receiveSettingsHex,1,1,1,1)
         serialReceiveSettingsLayout.addWidget(self.receiveSettingsAutoLinefeed, 2, 0, 1, 1)
         serialReceiveSettingsLayout.addWidget(self.receiveSettingsAutoLinefeedTime, 2, 1, 1, 1)
         serialReceiveSettingsLayout.addWidget(self.receiveSettingsTimestamp, 3, 0, 1, 1)
         serialReceiveSettingsLayout.addWidget(self.receiveSettingsColor, 3, 1, 1, 1)
+        serialReceiveSettingsLayout.addWidget(self.receiveSettingsWrap, 4, 0, 1, 1)
         serialReceiveSettingsGroupBox.setLayout(serialReceiveSettingsLayout)
         serialReceiveSettingsGroupBox.setAlignment(Qt.AlignHCenter)
         layout.addWidget(serialReceiveSettingsGroupBox)
 
         # serial send settings
         serialSendSettingsLayout = QGridLayout()
         serialSendSettingsGroupBox = QGroupBox(_("Send Settings"))
@@ -220,14 +226,15 @@
         self.sendSettingsAppendNewLine.clicked.connect(lambda: self.bindVar(self.sendSettingsAppendNewLine, self.config, "sendAutoNewline"))
         self.sendSettingsEscape.clicked.connect(lambda: self.bindVar(self.sendSettingsEscape, self.config, "sendEscape"))
         self.sendSettingsCRLF.clicked.connect(lambda: self.bindVar(self.sendSettingsCRLF, self.config, "useCRLF"))
         self.receiveSettingsColor.clicked.connect(self.onSetColorChanged)
         self.receiveSettingsAutoLinefeedTime.textChanged.connect(lambda: self.bindVar(self.receiveSettingsAutoLinefeedTime, self.config, "receiveAutoLindefeedTime", vtype=int, vErrorMsg=_("Auto line feed value error, must be integer"), emptyDefault = "200"))
         self.sendSettingsScheduled.textChanged.connect(lambda: self.bindVar(self.sendSettingsScheduled, self.config, "sendScheduledTime", vtype=int, vErrorMsg=_("Timed send value error, must be integer"), emptyDefault = "300"))
         self.sendSettingsScheduledCheckBox.clicked.connect(lambda: self.bindVar(self.sendSettingsScheduledCheckBox, self.config, "sendScheduled"))
+        self.receiveSettingsWrap.clicked.connect(self.onSettingWrap)
         return widget
 
 
     def onWidgetFunctional(self, parent):
         sendFunctionalLayout = QVBoxLayout()
         sendFunctionalLayout.setContentsMargins(0,0,0,0)
         # right functional layout
@@ -270,33 +277,39 @@
         customItems.setLayout(self.customSendItemsLayout)
         customSendItemsLayoutWrapper.addWidget(customItems)
         customSendItemsLayoutWrapper.addWidget(self.addButton)
         #   set wrapper widget
         self.customSendScroll.setWidget(cutomSendItemsWraper)
         self.customSendScroll.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         #
+        logFileWrapper = QVBoxLayout()
         logFileLayout = QHBoxLayout()
         self.saveLogCheckbox = QCheckBox()
         self.logFilePath = QLineEdit()
         self.logFileBtn = QPushButton(_("Log path"))
+        self.saveLogAutoNew = QCheckBox(_("Auto new file"))
+        self.saveLogAutoNew.setToolTip(_("When start a new connection, will automatically create a new log file"))
         logFileLayout.addWidget(self.saveLogCheckbox)
         logFileLayout.addWidget(self.logFilePath)
         logFileLayout.addWidget(self.logFileBtn)
-        self.logFileGroupBox.setLayout(logFileLayout)
+        logFileWrapper.addLayout(logFileLayout)
+        logFileWrapper.addWidget(self.saveLogAutoNew)
+        self.logFileGroupBox.setLayout(logFileWrapper)
         sendFunctionalLayout.addWidget(self.logFileGroupBox)
         sendFunctionalLayout.addWidget(self.fileSendGroupBox)
         sendFunctionalLayout.addWidget(self.clearHistoryButton)
         sendFunctionalLayout.addWidget(customSendGroupBox)
         sendFunctionalLayout.addStretch(1)
         self.funcWidget = QWidget()
         self.funcWidget.setLayout(sendFunctionalLayout)
         # event
         self.sendFileButton.clicked.connect(self.sendFile)
         self.saveLogCheckbox.clicked.connect(self.setSaveLog)
         self.logFileBtn.clicked.connect(self.selectLogFile)
+        self.saveLogAutoNew.clicked.connect(lambda: self.bindVar(self.saveLogAutoNew, self.config, "saveLogAutoNew"))
         self.openFileButton.clicked.connect(self.selectFile)
         self.addButton.clicked.connect(self.customSendAdd)
         self.clearHistoryButton.clicked.connect(self.clearHistory)
         self.funcParent = parent
         return self.funcWidget
 
     def onWidgetStatusBar(self, parent):
@@ -310,14 +323,15 @@
         try:
             interval = int(paramObj["receiveAutoLindefeedTime"])
             paramObj["receiveAutoLindefeedTime"] = interval
         except Exception:
             interval = parameters.Parameters.receiveAutoLindefeedTime
         self.receiveSettingsAutoLinefeedTime.setText(str(interval) if interval > 0 else str(parameters.Parameters.receiveAutoLindefeedTime))
         self.receiveSettingsTimestamp.setChecked(paramObj["showTimestamp"])
+        self.receiveSettingsWrap.setChecked(paramObj["wrap"])
         self.sendSettingsHex.setChecked(not paramObj["sendAscii"])
         self.sendSettingsScheduledCheckBox.setChecked(paramObj["sendScheduled"])
         try:
             interval = int(paramObj["sendScheduledTime"])
             paramObj["sendScheduledTime"] = interval
         except Exception:
             interval = parameters.Parameters.sendScheduledTime
@@ -328,15 +342,19 @@
         self.sendSettingsEscape.setChecked(paramObj["sendEscape"])
         for i in range(0, len(paramObj["sendHistoryList"])):
             text = paramObj["sendHistoryList"][i]
             self.sendHistory.addItem(text)
         self.logFilePath.setText(paramObj["saveLogPath"])
         self.logFilePath.setToolTip(paramObj["saveLogPath"])
         self.saveLogCheckbox.setChecked(paramObj["saveLog"])
+        self.saveLogAutoNew.setChecked(paramObj["saveLogAutoNew"])
         self.receiveSettingsColor.setChecked(paramObj["color"])
+        # wrap
+        self.receiveArea.setLineWrapMode(QTextEdit.WidgetWidth if paramObj["wrap"] else QTextEdit.NoWrap)
+        self.sendArea.setLineWrapMode(QTextEdit.WidgetWidth if paramObj["wrap"] else QTextEdit.NoWrap)
         # send items
         for text in paramObj["customSendItems"]:
             self.insertSendItem(text, load=True)
 
         self.receiveProcess = threading.Thread(target=self.receiveDataProcess)
         self.receiveProcess.setDaemon(True)
         self.receiveProcess.start()
@@ -374,14 +392,21 @@
 
     def onRecordSendClicked(self):
         self.config["recordSend"] = self.sendSettingsRecord.isChecked()
         if self.config["recordSend"]:
             self.config["receiveAutoLinefeed"] = True
             self.receiveSettingsAutoLinefeed.setChecked(True)
 
+    def onSettingWrap(self):
+        wrap = self.receiveSettingsWrap.isChecked()
+        self.config["wrap"] = wrap
+        flag = QTextEdit.WidgetWidth if wrap else QTextEdit.NoWrap
+        self.receiveArea.setLineWrapMode(flag)
+        self.sendArea.setLineWrapMode(flag)
+
     def onEscapeSendClicked(self):
         self.config["sendEscape"] = self.sendSettingsEscape.isChecked()
 
     def onSetColorChanged(self):
         self.config["color"] = self.receiveSettingsColor.isChecked()
 
     def onSendHistoryIndexChanged(self, idx):
@@ -439,20 +464,38 @@
                                     _("Log file (*.log);;txt file (*.txt);;All Files (*)"))
 
         if fileName_choose == "":
             return
         self.logFilePath.setText(fileName_choose)
         self.logFilePath.setToolTip(fileName_choose)
         self.config["saveLogPath"] = fileName_choose
+        self.config["saveLogPath2"] = fileName_choose
+
+    def updateLogPath(self):
+        '''
+            update log path add datetiem and com port name
+        '''
+        if not self.config["saveLogPath"]:
+            return
+        date = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
+        path = os.path.splitext(self.config['saveLogPath'])
+        self.config["saveLogPath2"] = f"{path[0]}_{date}{path[1]}"
+
 
     def onLog(self, text):
-        if self.config["saveLogPath"]:
-            with open(self.config["saveLogPath"], "a+", encoding=self.configGlobal["encoding"], newline="\n") as f:
+        path = self.config["saveLogPath2"] if self.config["saveLogAutoNew"] else self.config["saveLogPath"]
+        if self.config["saveLog"] and path:
+            with open(path, "a+", encoding=self.configGlobal["encoding"], newline="\n") as f:
                 f.write(text)
 
+    def onConnChanged(self, status:ConnectionStatus, msg:str):
+        super().onConnChanged(status, msg)
+        if status == ConnectionStatus.CONNECTED and self.config["saveLogAutoNew"]:
+            self.updateLogPath()
+
     def onKeyPressEvent(self, event):
         if event.key() == Qt.Key_Control:
             self.keyControlPressed = True
         elif event.key() == Qt.Key_Return or event.key()==Qt.Key_Enter:
             if self.keyControlPressed:
                 self.onSendData()
         elif event.key() == Qt.Key_L:
@@ -464,18 +507,27 @@
 
     def onKeyReleaseEvent(self, event):
         if event.key() == Qt.Key_Control:
             self.keyControlPressed = False
 
     def insertSendItem(self, text="", load = False):
         itemsNum = self.customSendItemsLayout.count() + 1
+        # TODO: here auto set scroll area height is ugly, maybe have better way
         height = parameters.customSendItemHeight * (itemsNum + 1) + 20
         topHeight = self.fileSendGroupBox.height() + self.logFileGroupBox.height() + 100
-        if height + topHeight > self.funcParent.height():
-            height = self.funcParent.height() - topHeight
+        # print("1:", parameters.customSendItemHeight, itemsNum + 1, height, topHeight)
+        # print("2:", height + topHeight, self.funcParent.height())
+        # if height + topHeight > self.funcParent.height():
+        #     height = self.funcParent.height() - topHeight
+        # if height < 0:
+        #     height = self.funcParent.height() // 3
+        screenH = QApplication.desktop().screenGeometry().height()
+        screenH -= screenH // 3
+        if height + topHeight >= screenH:
+            height = screenH - topHeight
         if height < 0:
             height = self.funcParent.height() // 3
         self.customSendScroll.setMinimumHeight(height)
         item = QWidget()
         layout = QHBoxLayout()
         layout.setContentsMargins(0,0,0,0)
         item.setLayout(layout)
@@ -497,19 +549,24 @@
         self.customSendItemsLayout.addWidget(item)
         if not load:
             self.config["customSendItems"].append("")
 
     def deleteSendItem(self, idx, item):
         item.setParent(None)
         self.config["customSendItems"].pop(idx)
+        # TODO: here auto set scroll area height is ugly, maybe have better way
         itemsNum = self.customSendItemsLayout.count()
         height = parameters.customSendItemHeight * (itemsNum + 1) + 20
         topHeight = self.fileSendGroupBox.height() + self.logFileGroupBox.height() + 100
-        if height + topHeight > self.funcParent.height():
-            height = self.funcParent.height() - topHeight
+        # if height + topHeight > self.funcParent.height():
+        #     height = self.funcParent.height() - topHeight
+        screenH = QApplication.desktop().screenGeometry().height()
+        screenH -= screenH // 3
+        if height + topHeight >= screenH:
+            height = screenH - topHeight
         self.customSendScroll.setMinimumHeight(height)
 
     def onCustomItemChange(self, idx, edit, send):
         text = edit.text()
         edit.setToolTip(text)
         send.setToolTip(text)
         self.config["customSendItems"][idx] = text
@@ -563,25 +620,25 @@
                 if self.config["recordSend"]:
                     head = '=> '
                     if self.config["showTimestamp"]:
                         head += '[{}] '.format(utils.datetime_format_ms(datetime.now()))
                     isHexStr, sendStr, sendStrsColored = self.bytes2String(data, not self.config["receiveAscii"], encoding=self.configGlobal["encoding"])
                     if isHexStr:
                         sendStr = sendStr.upper()
-                        sendStrsColored= sendStr
                         head += "[HEX] "
                     if self.config["useCRLF"]:
                         head = "\r\n" + head
                     else:
                         head = "\n" + head
                     if head.strip() != '=>':
                         head = '{}: '.format(head.rstrip())
-                    self.receiveUpdateSignal.emit(head, [sendStrsColored], self.configGlobal["encoding"])
+                    self.receiveUpdateSignal.emit(head, [sendStr], self.configGlobal["encoding"])
                     self.sendRecord.insert(0, head + sendStr)
                 self.send(data_bytes=data, callback = self.onSent)
+                self.justSent = True # flag for receive thread
                 if data_bytes:
                     data = str(data_bytes)
                 else:
                     data = self.sendArea.toPlainText()
                 self.sendHistoryFindDelete(data)
                 self.sendHistory.insertItem(0,data)
                 self.sendHistory.setCurrentIndex(0)
@@ -784,39 +841,49 @@
             logData = None
             head = ""
             self.lock.acquire()
             new = b"".join(self.receivedData)
             buffer += new
             self.receivedData = []
             # timeout, add new line
-            if time.time() - timeLastReceive> self.config["receiveAutoLindefeedTime"]:
+            # self.justSent means just sent data, need show head
+            if time.time() - timeLastReceive > self.config["receiveAutoLindefeedTime"] / 1000 or self.justSent:
                 if self.config["showTimestamp"] or self.config["receiveAutoLinefeed"]:
                     if self.config["useCRLF"]:
                         head += "\r\n"
                     else:
                         head += "\n"
                     new_line = True
+                    self.justSent = False
             data = ""
             # have data in buffer
             if len(buffer) > 0:
                 hexstr = False
                 # show as hex, just show
                 if not self.config["receiveAscii"]:
                     data = utils.bytes_to_hex_str(buffer)
                     colorData = data
                     buffer = b''
                     hexstr = True
                 # show as string, and don't need to render color
                 elif not self.config["color"]:
                     data = buffer.decode(encoding=self.configGlobal["encoding"], errors="ignore")
+                    # self.lastShowTail for separated \r\n, prevent show two linefeed
+                    # if last msg endswith "\r", and this msg startswith "\n", don't show "\n", if you have different thought, add issue to github
+                    if self.lastShowTail == "\r" and data[0] == "\n":
+                        data = data[1:]
                     colorData = data
                     buffer = b''
+                    if data and data[-1] == "\r":
+                        self.lastShowTail = data[-1]
+                    else:
+                        self.lastShowTail = ""
                 # show as string, and need to render color, wait for \n or until timeout to ensure color flag in buffer
                 else:
-                    if time.time() - timeLastReceive >  self.config["receiveAutoLindefeedTime"] or b'\n' in buffer:
+                    if time.time() - timeLastReceive >  self.config["receiveAutoLindefeedTime"] / 1000 or b'\n' in buffer:
                         data, colorData, remain = self.getColoredText(buffer, self.configGlobal["encoding"])
                         buffer = remain
                 # add time receive head
                 # get data from buffer, now render
                 if data:
                     # add time header, head format(send receive '123' for example):
                     # '123'  '[2021-12-20 11:02:08.02.754]: 123' '=> 12' '<= 123'
```

### Comparing `COMTool-3.1.2/COMTool/plugins/graph.py` & `COMTool-3.2.0/COMTool/plugins/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,23 @@
     connChilds = []          # children ids
     id = "graph"
     name = _("Graph")
 
     enabled = False          # user enabled this plugin
     active  = False          # using this plugin
 
-    help = '{}<br><br>{}<br>Python:<br><pre>{}</pre><br>C/C++:<br><pre>{}</pre>'.format(_("Double click graph item to add a graph widget"), _("line chart plot protocol:"),
+    help = '{}<br><br>{}<br><h2>Python</h2><br><pre>{}</pre><p><p>{}<br>{}</p><p>{}</p></p><br><h2>C/C++</h2><br><pre>{}</pre>'.format(
+        _("Double click graph item to add a graph widget"), _("line chart plot protocol:"),
 '''
-from COMTool.plugin import graph_protocol
-frame = graph_protocol.plot_pack(name, x, y, header= b'\xAA\xCC\xEE\xBB')
+from COMTool.plugins import graph_protocol
+frame = graph_protocol.plot_pack(name, x, y, header= b'\\xAA\\xCC\\xEE\\xBB')
 ''',
+        _("Full demo see:"),
+        '<a href="https://github.com/Neutree/COMTool/tree/master/tool/send_curve_demo.py">https://github.com/Neutree/COMTool/tree/master/tool/send_curve_demo.py</a>',
+        _("Install comtool by <code>pip install comtool</code> first"),
 '''
 void plot_pack(uint8_t *buff, int buff_len,
                uint8_t *header, int header_len,
                char *name,
                double x, double y)
 {
     uint8_t len = (uint8_t)strlen(name);
```

### Comparing `COMTool-3.1.2/COMTool/plugins/graph_widget_metasenselite.py` & `COMTool-3.2.0/COMTool/plugins/graph_widget_metasenselite.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/graph_widgets.py` & `COMTool-3.2.0/COMTool/plugins/graph_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # from PyQt5.QtWidgets import (QWidget, QVBoxLayout, QLabel, QSlider, QLineEdit, QGridLayout, QPushButton, QCheckBox, QHBoxLayout, QInputDialog)
 # from PyQt5.QtCore import pyqtSignal
 # from PyQt5.QtGui import QDoubleValidator
-import numpy as np
 import os
 from PyQt5.QtWidgets import (QWidget, QVBoxLayout, QLabel, QSlider, QLineEdit,
                              QGridLayout, QPushButton, QCheckBox, QHBoxLayout, QInputDialog, QComboBox, QFileDialog)
 from PyQt5.QtCore import pyqtSignal, Qt
 from PyQt5.QtGui import QDoubleValidator
 
 try:
@@ -15,15 +14,15 @@
     from widgets import EditRemarDialog
 except Exception:
     from COMTool.i18n import _
     from COMTool import utils_ui
     from COMTool import utils
     from COMTool.widgets import EditRemarDialog
 
-from .graph_widget_metasenselite import Graph_MetaSenseLite
+# from .graph_widget_metasenselite import Graph_MetaSenseLite
 from .graph_widgets_base import Graph_Widget_Base
 import pyqtgraph as pg
 from struct import unpack, pack
 import time
 
 
 
@@ -44,14 +43,15 @@
             self.config["header"], escape=True, encoding="utf-8")
         self.layout = QGridLayout()
         self.setLayout(self.layout)
         self.plotWin = pg.GraphicsLayoutWidget()
         self.plotWin.setMinimumHeight(200)
         pg.setConfigOptions(antialias=True)
         rmBtn = QPushButton(_("Remove"))
+        clearBtn = QPushButton(_("Clear"))
         rangeLabel = QLabel(_("Range:"))
         rangeConf = QLineEdit(str(self.config["xRange"]))
         rangeEnable = QCheckBox(_("Enable"))
         rangeEnable.setChecked(self.config["xRangeEnable"])
         headerLabel = QLabel(_("Header:"))
         headerConf = QLineEdit(self.config["header"])
         self.headerBtn = QPushButton(_("Set"))
@@ -60,14 +60,15 @@
         headerConf.setToolTip(hint)
         headerLabel.setToolTip(hint)
         self.headerBtn.setToolTip(hint)
         validator = QDoubleValidator()
         rangeConf.setValidator(validator)
         self.layout.addWidget(self.plotWin, 0, 0, 1, 3)
         self.layout.addWidget(rmBtn, 1, 0, 1, 1)
+        self.layout.addWidget(clearBtn, 1, 2, 1, 1)
         self.layout.addWidget(rangeLabel, 2, 0, 1, 1)
         self.layout.addWidget(rangeConf, 2, 1, 1, 1)
         self.layout.addWidget(rangeEnable, 2, 2, 1, 1)
         self.layout.addWidget(headerLabel, 3, 0, 1, 1)
         self.layout.addWidget(headerConf, 3, 1, 1, 1)
         self.layout.addWidget(self.headerBtn, 3, 2, 1, 1)
         self.resize(600, 400)
@@ -108,18 +109,26 @@
         rangeConf.textChanged.connect(self.setRange)
         rangeEnable.clicked.connect(
             lambda: self.setEnableRange(rangeEnable.isChecked()))
         self.headerBtn.clicked.connect(
             lambda: self.setHeader(headerConf.text()))
         rmBtn.clicked.connect(self.remove)
         headerConf.textChanged.connect(self.headerChanged)
+        clearBtn.clicked.connect(self.clear)
 
     def remove(self):
         self.rmCallback(self)
 
+    def clear(self):
+        self.data = {}
+        self.curves = {}
+        self.notUsedColors = self.builtinColors.copy()
+        self.colors = {}
+        self.p.clear()
+
     def setRange(self, text):
         if text:
             self.config["xRange"] = float(text)
 
     def setEnableRange(self, en):
         self.config["xRangeEnable"] = en
 
@@ -369,9 +378,9 @@
             self.pressedKeys.remove(key)
 
 
 graphWidgets = {
     Graph_Plot.id: Graph_Plot,
     Graph_Button.id: Graph_Button,
     # Graph_DragTof.id: Graph_DragTof,
-    Graph_MetaSenseLite.id: Graph_MetaSenseLite,
+    # Graph_MetaSenseLite.id: Graph_MetaSenseLite,
 }
```

### Comparing `COMTool-3.1.2/COMTool/plugins/graph_widgets_base.py` & `COMTool-3.2.0/COMTool/plugins/graph_widgets_base.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/myplugin.py` & `COMTool-3.2.0/COMTool/plugins/myplugin.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/protocol.py` & `COMTool-3.2.0/COMTool/plugins/protocol.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/protocols.py` & `COMTool-3.2.0/COMTool/plugins/protocols.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/plugins/terminal.py` & `COMTool-3.2.0/COMTool/plugins/terminal.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/protocols/maix-smart.py` & `COMTool-3.2.0/COMTool/protocols/maix-smart.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/qta_icon_browser.py` & `COMTool-3.2.0/COMTool/qta_icon_browser.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/settings.py` & `COMTool-3.2.0/COMTool/settings.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/test.py` & `COMTool-3.2.0/COMTool/test.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/utils.py` & `COMTool-3.2.0/COMTool/utils.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/utils_ui.py` & `COMTool-3.2.0/COMTool/utils_ui.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/version.py` & `COMTool-3.2.0/COMTool/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 major = 3
-minor = 1
-dev   = 2
+minor = 2
+dev   = 0
 
 __version__ = "{}.{}.{}".format(major, minor, dev)
 
 class Version:
     def __init__(self, major=major, minor=minor, dev=dev, name="", desc=""):
         self.major = major
         self.minor = minor
```

### Comparing `COMTool-3.1.2/COMTool/wave.py` & `COMTool-3.2.0/COMTool/wave.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool/widgets.py` & `COMTool-3.2.0/COMTool/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,16 +581,16 @@
         self.rxCount += count
         msg = '{}({}): {}'.format(_("Received"), _("bytes"), self.rxCount)
         self.updateUiSignal.emit("rx", msg)
 
     def addTx(self, count):
         if not self.rxTxCount:
             return
-        self.rxCount += count
-        msg = '{}({}): {}'.format(_("Sent"), _("bytes"), self.rxCount)
+        self.txCount += count
+        msg = '{}({}): {}'.format(_("Sent"), _("bytes"), self.txCount)
         self.updateUiSignal.emit("tx", msg)
 
     def clear(self):
         self.rxCount = 0
         self.txCount = 0
         self.addTx(0)
         self.addRx(0)
```

### Comparing `COMTool-3.1.2/COMTool/win32_utils.py` & `COMTool-3.2.0/COMTool/win32_utils.py`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/COMTool.egg-info/SOURCES.txt` & `COMTool-3.2.0/COMTool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 COMTool/assets/logo2.png
 COMTool/assets/right.png
 COMTool/assets/screenshot_V1.0.png
 COMTool/assets/screenshot_V1.3.png
 COMTool/assets/screenshot_V1.4_night.png
 COMTool/assets/screenshot_V1.7.png
 COMTool/assets/screenshot_graph.png
+COMTool/assets/screenshot_macos.jpg
 COMTool/assets/screenshot_protocol_v2.3.png
 COMTool/assets/screenshot_terminal.png
 COMTool/assets/screenshot_v2.png
 COMTool/assets/screenshot_v2_white.png
 COMTool/assets/skin-white.png
 COMTool/assets/skin.png
 COMTool/assets/tcp_udp.png
```

### Comparing `COMTool-3.1.2/LICENSE` & `COMTool-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `COMTool-3.1.2/README.MD` & `COMTool-3.2.0/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 COMTool
 ========
 
 English | [中文](./README_ZH.MD)
 
- ![GitHub](https://img.shields.io/github/license/neutree/comtool) [![PyPI](https://img.shields.io/pypi/v/comtool.svg)](https://pypi.python.org/pypi/comtool/) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/neutree/comtool/pack) ![GitHub repo size](https://img.shields.io/github/repo-size/neutree/comtool) ![GitHub Repo stars](https://img.shields.io/github/stars/neutree/comtool?style=social)
+ ![GitHub](https://img.shields.io/github/license/neutree/comtool) [![PyPI](https://img.shields.io/pypi/v/comtool.svg)](https://pypi.python.org/pypi/comtool/) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/neutree/comtool/pack.yml?branch=master) ![GitHub repo size](https://img.shields.io/github/repo-size/neutree/comtool) ![GitHub Repo stars](https://img.shields.io/github/stars/neutree/comtool?style=social)
 
  [![GitHub all releases](https://img.shields.io/github/downloads/neutree/comtool/total?label=release%20downloads)](https://github.com/Neutree/COMTool/releases) [![PyPI - Downloads](https://img.shields.io/pypi/dm/comtool?label=pypi%20downloads)](https://pypi.org/project/COMTool/) [![SourceForge](https://img.shields.io/sourceforge/dt/comtool?label=sourceforge%20downloads)](https://sourceforge.net/projects/comtool)
 
 
 A cross platform serial debug tools written by python
 
 --------
 
 | Windows | Linux | Raspberry Pi | macOS |
 | ------- | ----- | ------------ | ----- |
-| ![comtool Windows screenshot](./COMTool/assets/screenshot_v2_white.png) | ![comtool linux screenshot](./COMTool/assets/screenshot_V1.4_night.png) | ![comtool Raspberry Pi screenshot](./COMTool/assets/RaspberryPiScreenshot.png)
- | |
+| ![comtool Windows screenshot](./COMTool/assets/screenshot_v2_white.png) | ![comtool linux screenshot](./COMTool/assets/screenshot_V1.4_night.png) | ![comtool Raspberry Pi screenshot](./COMTool/assets/RaspberryPiScreenshot.png) | ![](./COMTool/assets/screenshot_macos.jpg) |
 
 
 | White theme | Dark theme | protocol plugin | TCP/UDP | Terminal | Graph |
 | ----------- | ---------- | --------------- | ------- | -------- | ----- |
 | ![comtool white theme](./COMTool/assets/screenshot_v2_white.png) | ![comtool dark theme](./COMTool/assets/screenshot_v2.png) | ![comtool protocol plugin](./COMTool/assets/screenshot_protocol_v2.3.png) | ![tcp udp plugin](./COMTool/assets/tcp_udp.png) | ![terminal](./COMTool/assets/screenshot_terminal.png) | ![plugin graph](./COMTool/assets/screenshot_graph.png) |
```

### Comparing `COMTool-3.1.2/setup.py` & `COMTool-3.2.0/setup.py`

 * *Files identical despite different names*

