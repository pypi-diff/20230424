# Comparing `tmp/chroma-feedback-9.1.0.tar.gz` & `tmp/chroma-feedback-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chroma-feedback-9.1.0.tar", last modified: Tue May 25 22:13:57 2021, max compression
+gzip compressed data, was "dist/chroma-feedback-9.1.1.tar", last modified: Tue Jun  1 00:03:30 2021, max compression
```

## Comparing `chroma-feedback-9.1.0.tar` & `chroma-feedback-9.1.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)    18158 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/PKG-INFO
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)    12024 2021-05-25 21:30:30.000000 chroma-feedback-9.1.0/README.md
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.760327 chroma-feedback-9.1.0/bin/
--rwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)      881 2021-01-08 13:27:01.000000 chroma-feedback-9.1.0/bin/chroma-feedback
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.760327 chroma-feedback-9.1.0/chroma_feedback/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)        0 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1629 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/color.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.760327 chroma-feedback-9.1.0/chroma_feedback/consumer/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      267 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/__init__.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.760327 chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      674 2021-05-19 12:41:08.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      739 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      947 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/device.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      854 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/core.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.760327 chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      656 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      720 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      889 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/device.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.764327 chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      651 2021-05-18 22:53:08.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      716 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      887 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/device.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.764327 chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-01-10 12:21:03.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      522 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1032 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1077 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/group.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      925 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/light.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.764327 chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      638 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      708 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      883 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/device.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.764327 chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      620 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1313 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1202 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/light.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.764327 chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      738 2021-01-09 22:11:26.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1388 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      851 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/light.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      738 2021-01-10 14:40:37.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1897 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1344 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/group.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1314 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/light.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      566 2021-01-08 15:47:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      703 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2266 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/device.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      642 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      710 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      933 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/device.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-01-10 16:05:53.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      901 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1341 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1001 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/light.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      701 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/api.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1421 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      832 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/light.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1804 2021-05-24 08:44:13.000000 chroma-feedback-9.1.0/chroma_feedback/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1177 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/helper.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      549 2021-05-19 22:17:57.000000 chroma-feedback-9.1.0/chroma_feedback/install.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      448 2021-05-25 21:22:42.000000 chroma-feedback-9.1.0/chroma_feedback/metadata.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/producer/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      204 2021-05-25 20:24:23.000000 chroma-feedback-9.1.0/chroma_feedback/producer/__init__.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/producer/appveyor/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/appveyor/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1860 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/appveyor/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      540 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/appveyor/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.768327 chroma-feedback-9.1.0/chroma_feedback/producer/azure/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-25 09:16:32.000000 chroma-feedback-9.1.0/chroma_feedback/producer/azure/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1540 2021-05-25 22:10:37.000000 chroma-feedback-9.1.0/chroma_feedback/producer/azure/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      645 2021-05-25 22:07:13.000000 chroma-feedback-9.1.0/chroma_feedback/producer/azure/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/bamboo/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/bamboo/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1433 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/bamboo/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      578 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/bamboo/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/bitbucket/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-01-04 10:27:43.000000 chroma-feedback-9.1.0/chroma_feedback/producer/bitbucket/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1685 2021-05-25 09:16:39.000000 chroma-feedback-9.1.0/chroma_feedback/producer/bitbucket/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      531 2021-05-25 09:16:39.000000 chroma-feedback-9.1.0/chroma_feedback/producer/bitbucket/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/buddy/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/buddy/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2476 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/producer/buddy/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      483 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/buddy/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/circle/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/circle/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2589 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/circle/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      578 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/circle/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/codeship/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/codeship/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     3300 2021-05-23 20:52:50.000000 chroma-feedback-9.1.0/chroma_feedback/producer/codeship/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      603 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/codeship/normalize.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      781 2021-05-15 16:42:29.000000 chroma-feedback-9.1.0/chroma_feedback/producer/core.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/github/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/github/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2487 2021-05-24 08:46:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/github/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      634 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/github/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/gitlab/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/gitlab/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1861 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/gitlab/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      563 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/gitlab/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/jenkins/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/jenkins/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1418 2021-05-23 22:25:38.000000 chroma-feedback-9.1.0/chroma_feedback/producer/jenkins/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      595 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/jenkins/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/teamcity/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/teamcity/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2065 2021-05-23 22:55:15.000000 chroma-feedback-9.1.0/chroma_feedback/producer/teamcity/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      601 2021-05-23 22:51:36.000000 chroma-feedback-9.1.0/chroma_feedback/producer/teamcity/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/travis/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/travis/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1571 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/travis/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      570 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/travis/normalize.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/chroma_feedback/producer/wercker/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/wercker/__init__.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1891 2021-05-14 20:05:46.000000 chroma-feedback-9.1.0/chroma_feedback/producer/wercker/core.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      601 2021-05-23 22:38:45.000000 chroma-feedback-9.1.0/chroma_feedback/producer/wercker/normalize.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2930 2021-05-25 09:16:47.000000 chroma-feedback-9.1.0/chroma_feedback/reporter.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      599 2021-05-24 08:48:45.000000 chroma-feedback-9.1.0/chroma_feedback/request.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2534 2021-05-25 09:16:47.000000 chroma-feedback-9.1.0/chroma_feedback/systray.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       91 2021-05-18 22:50:04.000000 chroma-feedback-9.1.0/chroma_feedback/typing.py
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1264 2021-05-19 12:41:08.000000 chroma-feedback-9.1.0/chroma_feedback/wording.py
-drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-05-25 22:13:57.760327 chroma-feedback-9.1.0/chroma_feedback.egg-info/
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)    18158 2021-05-25 22:13:57.000000 chroma-feedback-9.1.0/chroma_feedback.egg-info/PKG-INFO
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     4820 2021-05-25 22:13:57.000000 chroma-feedback-9.1.0/chroma_feedback.egg-info/SOURCES.txt
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)        1 2021-05-25 22:13:57.000000 chroma-feedback-9.1.0/chroma_feedback.egg-info/dependency_links.txt
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      178 2021-05-25 22:13:57.000000 chroma-feedback-9.1.0/chroma_feedback.egg-info/requires.txt
--rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       16 2021-05-25 22:13:57.000000 chroma-feedback-9.1.0/chroma_feedback.egg-info/top_level.txt
--rw-r--r--   0 redaxmedia  (1000) redaxmedia  (1000)       79 2021-05-25 22:13:57.772327 chroma-feedback-9.1.0/setup.cfg
--rwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)     2173 2021-05-25 20:24:23.000000 chroma-feedback-9.1.0/setup.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)    12475 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/PKG-INFO
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)    12024 2021-05-31 23:46:39.000000 chroma-feedback-9.1.1/README.md
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.583834 chroma-feedback-9.1.1/bin/
+-rwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)      881 2021-05-31 22:43:24.000000 chroma-feedback-9.1.1/bin/chroma-feedback
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.583834 chroma-feedback-9.1.1/chroma_feedback/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)        0 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1629 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/color.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.583834 chroma-feedback-9.1.1/chroma_feedback/consumer/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      267 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/__init__.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.583834 chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      674 2021-05-19 12:41:08.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      739 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      895 2021-05-31 23:58:54.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/device.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      854 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/core.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      656 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      720 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      837 2021-05-31 23:58:54.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/device.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      651 2021-05-18 22:53:08.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      716 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      835 2021-05-31 23:58:54.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/device.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-01-10 12:21:03.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      522 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1032 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1071 2021-05-31 11:10:39.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/group.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      919 2021-05-31 11:10:39.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/light.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      638 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      708 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      831 2021-05-31 23:58:54.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/device.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      620 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1313 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      907 2021-05-31 13:20:43.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/light.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      738 2021-01-09 22:11:26.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1388 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      726 2021-05-31 13:21:13.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/light.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      738 2021-01-10 14:40:37.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1897 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1020 2021-05-31 13:20:56.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/group.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      990 2021-05-31 13:20:56.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/light.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.587834 chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      566 2021-01-08 15:47:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      703 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1557 2021-05-31 23:21:08.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/device.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      642 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      710 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      881 2021-05-31 23:58:54.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/device.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-01-10 16:05:53.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      901 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1341 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      995 2021-05-31 11:10:39.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/light.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      701 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/api.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1421 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      826 2021-05-31 23:21:08.000000 chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/light.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1804 2021-05-31 23:58:30.000000 chroma-feedback-9.1.1/chroma_feedback/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1177 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/helper.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      549 2021-05-31 13:57:54.000000 chroma-feedback-9.1.1/chroma_feedback/install.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      448 2021-06-01 00:01:23.000000 chroma-feedback-9.1.1/chroma_feedback/metadata.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/producer/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      204 2021-05-25 20:24:23.000000 chroma-feedback-9.1.1/chroma_feedback/producer/__init__.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/producer/appveyor/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/appveyor/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1860 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/appveyor/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      540 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/appveyor/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/producer/azure/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-25 09:16:32.000000 chroma-feedback-9.1.1/chroma_feedback/producer/azure/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1540 2021-05-25 22:10:37.000000 chroma-feedback-9.1.1/chroma_feedback/producer/azure/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      645 2021-05-25 22:07:13.000000 chroma-feedback-9.1.1/chroma_feedback/producer/azure/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/producer/bamboo/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/bamboo/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1433 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/bamboo/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      578 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/bamboo/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/producer/bitbucket/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-01-04 10:27:43.000000 chroma-feedback-9.1.1/chroma_feedback/producer/bitbucket/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1685 2021-05-25 09:16:39.000000 chroma-feedback-9.1.1/chroma_feedback/producer/bitbucket/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      531 2021-05-25 09:16:39.000000 chroma-feedback-9.1.1/chroma_feedback/producer/bitbucket/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.591834 chroma-feedback-9.1.1/chroma_feedback/producer/buddy/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/buddy/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2476 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/producer/buddy/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      483 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/buddy/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/circle/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/circle/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2589 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/circle/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      578 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/circle/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/codeship/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/codeship/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     3300 2021-05-23 20:52:50.000000 chroma-feedback-9.1.1/chroma_feedback/producer/codeship/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      603 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/codeship/normalize.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      781 2021-05-15 16:42:29.000000 chroma-feedback-9.1.1/chroma_feedback/producer/core.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/github/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/github/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2487 2021-05-24 08:46:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/github/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      634 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/github/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/gitlab/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/gitlab/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1861 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/gitlab/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      563 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/gitlab/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/jenkins/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/jenkins/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1418 2021-05-23 22:25:38.000000 chroma-feedback-9.1.1/chroma_feedback/producer/jenkins/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      595 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/jenkins/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/teamcity/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/teamcity/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2065 2021-05-23 22:55:15.000000 chroma-feedback-9.1.1/chroma_feedback/producer/teamcity/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      601 2021-05-23 22:51:36.000000 chroma-feedback-9.1.1/chroma_feedback/producer/teamcity/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/travis/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/travis/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1571 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/travis/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      570 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/travis/normalize.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/chroma_feedback/producer/wercker/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       28 2020-04-26 23:58:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/wercker/__init__.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1891 2021-05-14 20:05:46.000000 chroma-feedback-9.1.1/chroma_feedback/producer/wercker/core.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      601 2021-05-23 22:38:45.000000 chroma-feedback-9.1.1/chroma_feedback/producer/wercker/normalize.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2930 2021-05-25 09:16:47.000000 chroma-feedback-9.1.1/chroma_feedback/reporter.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      599 2021-05-24 08:48:45.000000 chroma-feedback-9.1.1/chroma_feedback/request.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     2488 2021-05-31 23:59:41.000000 chroma-feedback-9.1.1/chroma_feedback/systray.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       91 2021-05-18 22:50:04.000000 chroma-feedback-9.1.1/chroma_feedback/typing.py
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     1264 2021-05-31 13:57:54.000000 chroma-feedback-9.1.1/chroma_feedback/wording.py
+drwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)        0 2021-06-01 00:03:30.583834 chroma-feedback-9.1.1/chroma_feedback.egg-info/
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)    12475 2021-06-01 00:03:30.000000 chroma-feedback-9.1.1/chroma_feedback.egg-info/PKG-INFO
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)     4820 2021-06-01 00:03:30.000000 chroma-feedback-9.1.1/chroma_feedback.egg-info/SOURCES.txt
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)        1 2021-06-01 00:03:30.000000 chroma-feedback-9.1.1/chroma_feedback.egg-info/dependency_links.txt
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)      178 2021-06-01 00:03:30.000000 chroma-feedback-9.1.1/chroma_feedback.egg-info/requires.txt
+-rw-rw-r--   0 redaxmedia  (1000) redaxmedia  (1000)       16 2021-06-01 00:03:30.000000 chroma-feedback-9.1.1/chroma_feedback.egg-info/top_level.txt
+-rw-r--r--   0 redaxmedia  (1000) redaxmedia  (1000)       79 2021-06-01 00:03:30.595834 chroma-feedback-9.1.1/setup.cfg
+-rwxrwxr-x   0 redaxmedia  (1000) redaxmedia  (1000)     2173 2021-05-31 23:58:30.000000 chroma-feedback-9.1.1/setup.py
```

### Comparing `chroma-feedback-9.1.0/README.md` & `chroma-feedback-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/bin/chroma-feedback` & `chroma-feedback-9.1.1/bin/chroma-feedback`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/color.py` & `chroma-feedback-9.1.1/chroma_feedback/color.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/agile_innovative_blinkstick/device.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/agile_innovative_blinkstick/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 	for device in devices:
 		result.append(
 		{
 			'consumer': 'agile_innovative_blinkstick',
 			'type': 'device',
 			'name': device.info['product_string'] + ' (' + device.info['serial_number'] + ')',
-			'active': static_device(device, color.get_by_status(status)),
+			'active': set_device(device, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_device(device : Any, color_config : Dict[str, Any]) -> bool:
-	return device.on((color_config['rgb'][0], color_config['rgb'][1], color_config['rgb'][2])) is None
+def set_device(device : Any, color_config : Dict[str, Any]) -> bool:
+	return device.on(tuple(color_config['rgb'])) is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/embrava_blynclight/device.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/embrava_blynclight/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 	for device in devices:
 		result.append(
 		{
 			'consumer': 'embrava_blynclight',
 			'type': 'device',
 			'name': device.info['product_string'],
-			'active': static_device(device, color.get_by_status(status)),
+			'active': set_device(device, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_device(device : Any, color_config : Dict[str, Any]) -> bool:
-	return device.on((color_config['rgb'][0], color_config['rgb'][1], color_config['rgb'][2])) is None
+def set_device(device : Any, color_config : Dict[str, Any]) -> bool:
+	return device.on(tuple(color_config['rgb'])) is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/kuando_busylight/device.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/device.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	result = []
 
 	# process devices
 
 	for device in devices:
 		result.append(
 		{
-			'consumer': 'kuando_busylight',
+			'consumer': 'luxafor_flag',
 			'type': 'device',
 			'name': device.info['product_string'],
-			'active': static_device(device, color.get_by_status(status)),
+			'active': set_device(device, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_device(device : Any, color_config : Dict[str, Any]) -> bool:
-	return device.on((color_config['rgb'][0], color_config['rgb'][1], color_config['rgb'][2])) is None
+def set_device(device : Any, color_config : Dict[str, Any]) -> bool:
+	return device.on(tuple(color_config['rgb'])) is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/group.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/group.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 
 	for group in groups:
 		result.append(
 		{
 			'consumer': 'lifx_light',
 			'type': 'group',
 			'name': get_group_name(group),
-			'active': static_group(group, color.get_by_status(status)),
+			'active': set_group(group, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_group(group : Any, color_config : Dict[str, Any]) -> bool:
+def set_group(group : Any, color_config : Dict[str, Any]) -> bool:
 	return group.set_power('on') is None and group.set_color(
 	[
 		color_config['hue'],
 		color_config['saturation'][2],
 		color_config['brightness'][2],
 		color_config['kelvin']
 	]) is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/lifx_light/light.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/lifx_light/light.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 	for light in lights:
 		result.append(
 		{
 			'consumer': 'lifx_light',
 			'type': 'light',
 			'name': light.get_label(),
-			'active': static_light(light, color.get_by_status(status)),
+			'active': set_light(light, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_light(light : Any, color_config : Dict[str, Any]) -> bool:
+def set_light(light : Any, color_config : Dict[str, Any]) -> bool:
 	return light.set_power('on') is None and light.set_color(
 	[
 		color_config['hue'],
 		color_config['saturation'][2],
 		color_config['brightness'][2],
 		color_config['kelvin']
 	]) is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/luxafor_flag/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/luxafor_flag/device.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/kuando_busylight/device.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 	result = []
 
 	# process devices
 
 	for device in devices:
 		result.append(
 		{
-			'consumer': 'luxafor_flag',
+			'consumer': 'kuando_busylight',
 			'type': 'device',
 			'name': device.info['product_string'],
-			'active': static_device(device, color.get_by_status(status)),
+			'active': set_device(device, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_device(device : Any, color_config : Dict[str, Any]) -> bool:
-	return device.on((color_config['rgb'][0], color_config['rgb'][1], color_config['rgb'][2])) is None
+def set_device(device : Any, color_config : Dict[str, Any]) -> bool:
+	return device.on(tuple(color_config['rgb'])) is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/magic_hue/light.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/magic_hue/light.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,43 +19,27 @@
 
 	for light in lights:
 		result.append(
 		{
 			'consumer': 'magic_hue',
 			'type': 'light',
 			'name': light.name,
-			'active': static_light(light, color.get_by_status(status)),
+			'active': set_light(light, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_light(light : Any, color_config : Dict[str, Any]) -> bool:
+def set_light(light : Any, color_config : Dict[str, Any]) -> bool:
 	modes = get_modes()
 
 	if modes:
 		light.mode = modes.CustomMode(
 			mode = modes.MODE_GRADUALLY,
 			speed = 1,
 			colors =\
 			[
 				color_config['rgb'],
 				color_config['rgb']
 			]
 		)
 	return light.update_status() is None
-
-
-def pulsate_light(light : Any, color_config : Dict[str, Any]) -> bool:
-	modes = get_modes()
-
-	if modes:
-		light.mode = modes.CustomMode(
-			mode = modes.MODE_GRADUALLY,
-			speed = 1,
-			colors =\
-			[
-				color_config['rgb'],
-				(0, 0, 0)
-			]
-		)
-	return light.update_status() is None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/nanoleaf_light/light.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/nanoleaf_light/light.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 
 	for light in lights:
 		result.append(
 		{
 			'consumer': 'nanoleaf_light',
 			'type': 'light',
 			'name': light.get_name(),
-			'active': static_light(light, color.get_by_status(status)),
+			'active': set_light(light, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_light(light : Any, color_config : Dict[str, Any]) -> bool:
+def set_light(light : Any, color_config : Dict[str, Any]) -> bool:
 	return light.set_color(color_config['rgb'])
-
-
-def pulsate_light(light : Any, color_config : Dict[str, Any]) -> bool:
-	return light.pulsate(color_config['rgb'], 5)
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/group.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/group.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,37 +20,24 @@
 
 	for index in groups:
 		result.append(
 		{
 			'consumer': 'philips_hue',
 			'type': 'group',
 			'name': groups[index]['name'],
-			'active': static_group(groups[index]['name'], color.get_by_status(status)),
+			'active': set_group(groups[index]['name'], color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_group(group_name : str, color_config : Dict[str, Any]) -> bool:
+def set_group(group_name : str, color_config : Dict[str, Any]) -> bool:
 	api = get_api(None)
 
 	return api is not None and api.set_group(group_name,
 	{
 		'hue': color_config['hue'],
 		'sat': color_config['saturation'][1],
 		'bri': color_config['brightness'][1],
 		'on': True,
 		'alert': 'none'
 	}) is not None
-
-
-def pulsate_group(group_name : str, color_config : Dict[str, Any]) -> bool:
-	api = get_api(None)
-
-	return api is not None and api.set_group(group_name,
-	{
-		'hue': color_config['hue'],
-		'sat': color_config['saturation'][1],
-		'bri': color_config['brightness'][1],
-		'on': True,
-		'alert': 'lselect'
-	}) is not None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/philips_hue/light.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/philips_hue/light.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,37 +20,24 @@
 
 	for light in lights:
 		result.append(
 		{
 			'consumer': 'philips_hue',
 			'type': 'light',
 			'name': light.name,
-			'active': static_light(light.name, color.get_by_status(status)),
+			'active': set_light(light.name, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_light(light_name : str, color_config : Dict[str, Any]) -> bool:
+def set_light(light_name : str, color_config : Dict[str, Any]) -> bool:
 	api = get_api(None)
 
 	return api is not None and api.set_light(light_name,
 	{
 		'hue': color_config['hue'],
 		'sat': color_config['saturation'][1],
 		'bri': color_config['brightness'][1],
 		'on': True,
 		'alert': 'none'
 	}) is not None
-
-
-def pulsate_light(light_name : str, color_config : Dict[str, Any]) -> bool:
-	api = get_api(None)
-
-	return api is not None and api.set_light(light_name,
-	{
-		'hue': color_config['hue'],
-		'sat': color_config['saturation'][1],
-		'bri': color_config['brightness'][1],
-		'on': True,
-		'alert': 'lselect'
-	}) is not None
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/razer_chroma/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/razer_chroma/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/thingm_blink1/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/thingm_blink1/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/wiz_light/light.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/wiz_light/light.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 	for light in lights:
 		result.append(
 		{
 			'consumer': 'wiz_light',
 			'type': 'light',
 			'name': get_light_name(light),
-			'active': static_light(light, color.get_by_status(status)),
+			'active': set_light(light, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
 def get_light_name(light : Any) -> str:
 	loop = get_loop()
 	config = loop.run_until_complete(light.get_bulbtype())
 	return config.name
 
 
-def static_light(light : Any, color_config : Dict[str, Any]) -> bool:
+def set_light(light : Any, color_config : Dict[str, Any]) -> bool:
 	loop = get_loop()
 	builder = get_builder()
 	loop.run_until_complete(light.turn_on(builder(rgb = color_config['rgb'])))
 	return loop.is_closed() is False
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/api.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/api.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/core.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/consumer/xiaomi_yeelight/light.py` & `chroma-feedback-9.1.1/chroma_feedback/consumer/xiaomi_yeelight/light.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 	for light in lights:
 		result.append(
 		{
 			'consumer': 'xiaomi_yeelight',
 			'type': 'light',
 			'name': light.get_properties()['name'],
-			'active': static_light(light, color.get_by_status(status)),
+			'active': set_light(light, color.get_by_status(status)),
 			'status': status
 		})
 	return result
 
 
-def static_light(light : Any, color_config : Dict[str, Any]) -> bool:
+def set_light(light : Any, color_config : Dict[str, Any]) -> bool:
 	return light.turn_on() == 'ok' and light.set_rgb(color_config['rgb'][0], color_config['rgb'][1], color_config['rgb'][2]) == 'ok'
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/core.py` & `chroma-feedback-9.1.1/chroma_feedback/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/helper.py` & `chroma-feedback-9.1.1/chroma_feedback/helper.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/install.py` & `chroma-feedback-9.1.1/chroma_feedback/install.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/appveyor/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/appveyor/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/appveyor/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/appveyor/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/azure/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/azure/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/azure/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/azure/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/bamboo/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/bamboo/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/bamboo/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/bamboo/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/bitbucket/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/bitbucket/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/bitbucket/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/bitbucket/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/buddy/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/buddy/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/circle/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/circle/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/circle/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/circle/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/codeship/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/codeship/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/codeship/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/codeship/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/github/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/github/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/github/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/github/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/gitlab/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/gitlab/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/gitlab/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/gitlab/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/jenkins/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/jenkins/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/jenkins/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/jenkins/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/teamcity/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/teamcity/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/teamcity/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/teamcity/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/travis/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/travis/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/travis/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/travis/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/wercker/core.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/wercker/core.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/producer/wercker/normalize.py` & `chroma-feedback-9.1.1/chroma_feedback/producer/wercker/normalize.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/reporter.py` & `chroma-feedback-9.1.1/chroma_feedback/reporter.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/request.py` & `chroma-feedback-9.1.1/chroma_feedback/request.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback/systray.py` & `chroma-feedback-9.1.1/chroma_feedback/systray.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 	return menu
 
 
 def create_icon(status : StatusType) -> str:
 	color_config = color.get_by_status(status)
 	image = Image.new('RGBA', (100, 100), (0, 0, 0, 0))
 	draw = ImageDraw.Draw(image)
-	draw.ellipse((20, 20, 80, 80), fill = (color_config['rgb'][0], color_config['rgb'][1], color_config['rgb'][2]))
+	draw.ellipse((20, 20, 80, 80), fill = tuple(color_config['rgb']))
 	path = tempfile.mktemp('.png')
 	image.save(path)
 	return path
 
 
 def about(menu_item : Any) -> None:
 	logo = GdkPixbuf.Pixbuf.new_from_file_at_size(create_icon('passed'), 20, 20)
```

### Comparing `chroma-feedback-9.1.0/chroma_feedback/wording.py` & `chroma-feedback-9.1.1/chroma_feedback/wording.py`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/chroma_feedback.egg-info/SOURCES.txt` & `chroma-feedback-9.1.1/chroma_feedback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chroma-feedback-9.1.0/setup.py` & `chroma-feedback-9.1.1/setup.py`

 * *Files identical despite different names*

