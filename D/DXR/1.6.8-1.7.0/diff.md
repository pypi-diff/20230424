# Comparing `tmp/DXR-1.6.8.tar.gz` & `tmp/DXR-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.6.8.tar", last modified: Fri Apr 14 07:14:53 2023, max compression
+gzip compressed data, was "DXR-1.7.0.tar", last modified: Mon Apr 24 04:58:32 2023, max compression
```

## Comparing `DXR-1.6.8.tar` & `DXR-1.7.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.977959 DXR-1.6.8/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.886055 DXR-1.6.8/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1291 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-14 07:14:53.000000 DXR-1.6.8/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.892933 DXR-1.6.8/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.6.8/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.6.8/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.6.8/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.901272 DXR-1.6.8/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.6.8/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.920457 DXR-1.6.8/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2724 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.6.8/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.6.8/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.944034 DXR-1.6.8/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.6.8/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.6.8/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.6.8/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.6.8/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.6.8/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.948708 DXR-1.6.8/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.6.8/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.6.8/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.6.8/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.6.8/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.6.8/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.950724 DXR-1.6.8/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.955634 DXR-1.6.8/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.6.8/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.6.8/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.958259 DXR-1.6.8/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.6.8/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.961505 DXR-1.6.8/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.972410 DXR-1.6.8/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.975367 DXR-1.6.8/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.6.8/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.6.8/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-14 07:14:53.976563 DXR-1.6.8/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.6.8/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.6.8/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-14 07:14:53.977081 DXR-1.6.8/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.6.8/README.md
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-14 07:14:53.978145 DXR-1.6.8/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-14 07:14:44.000000 DXR-1.6.8/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.331879 DXR-1.7.0/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.180817 DXR-1.7.0/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-24 04:58:32.000000 DXR-1.7.0/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1291 2023-04-24 04:58:32.000000 DXR-1.7.0/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-24 04:58:32.000000 DXR-1.7.0/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-24 04:58:32.000000 DXR-1.7.0/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-24 04:58:32.000000 DXR-1.7.0/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.182522 DXR-1.7.0/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.7.0/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.0/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.0/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.205165 DXR-1.7.0/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.0/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.263617 DXR-1.7.0/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.0/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.0/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3319 2023-04-24 04:57:52.000000 DXR-1.7.0/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.7.0/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.0/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.278221 DXR-1.7.0/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.0/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.0/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.0/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.0/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.0/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.0/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.0/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.0/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.301047 DXR-1.7.0/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.0/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.7.0/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.0/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.0/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.0/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.307764 DXR-1.7.0/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.312321 DXR-1.7.0/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.0/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.0/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.316444 DXR-1.7.0/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.0/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.319997 DXR-1.7.0/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.328384 DXR-1.7.0/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.330065 DXR-1.7.0/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.0/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.0/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 04:58:32.331189 DXR-1.7.0/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.0/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.0/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-24 04:58:32.331529 DXR-1.7.0/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.0/README.md
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 04:58:32.332015 DXR-1.7.0/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-24 04:58:16.000000 DXR-1.7.0/setup.py
```

### Comparing `DXR-1.6.8/DXR.egg-info/SOURCES.txt` & `DXR-1.7.0/DXR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_Chat/ChatGPT.py` & `DXR-1.7.0/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_Chat/utils.py` & `DXR-1.7.0/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_bytes/Dxr_bytes.py` & `DXR-1.7.0/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_file/dxr_file.py` & `DXR-1.7.0/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_file/dxr_request.py` & `DXR-1.7.0/Dxr_file/dxr_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,80 +1,96 @@
 import requests
 
 # 使用requests库，发送get请求
-def ssh_create_dir(path, ip, *args, **kwargs):
+def ssh_create_dir(path, ip, args, kwargs)
     # 通过requests库，发送POST请求, path是文件的绝对路径
-    url = 'http://%s:5000/add_user' % ip
-    data = {'user_name': path}
-    try:
-        r = requests.post(url, data=data, timeout=1)
+    url = 'http%s6050add_user' % ip
+    print(f'url is {url}, path is {path}')
+    data = {'user_name' path}
+    try
+        # r = requests.post(url, data=data, timeout=1)
+        r = requests.get(f'{url}{path.split()[-1]}', timeout=1)
         print(r.json())
-        if r.json()['code'] == 200:
+        if r.json()['code'] == 200
             return True
-        else:
+        else
             return False
-    except Exception as e:
+    except Exception as e
         print(e)
         return False
     
 # 使用requests库，发送post请求
-def ssh_delete_dir(path, ip, *args, **kwargs):
+def ssh_delete_dir(path, ip, args, kwargs)
     # 通过requests库，发送POST请求, path是文件的绝对路径
-    url = 'http://%s:5000/delete_user' % ip
-    data = {'user_name': path}
-    try:
+    url = 'http%s5000delete_user' % ip
+    data = {'user_name' path}
+    try
         r = requests.post(url, data=data, timeout=1)
         print(r.json())
-        if r.json()['code'] == 200:
+        if r.json()['code'] == 200
             return True
-        else:
+        else
             return False
-    except Exception as e:
+    except Exception as e
         print(e)
         return False
     
-def ssh_delete_file(path, ip, *args, **kwargs):
+def ssh_delete_file(path, ip, args, kwargs)
     # 通过requests库，发送POST请求, path是文件的绝对路径
-    url = 'http://%s:5000/delete_image' % ip
-    data = {'user_name': path}
-    try:
+    url = 'http%s5000delete_image' % ip
+    data = {'user_name' path}
+    try
         r = requests.post(url, data=data, timeout=1)
         print(r.json())
-        if r.json()['code'] == 200:
+        if r.json()['code'] == 200
             return True
-        else:
+        else
             return False
-    except Exception as e:
+    except Exception as e
         print(e)
         return False
     
-def ssh_upload_file(local_path, remote_path, ip, *args, **kwargs):
+def ssh_upload_file(local_path, remote_path, ip, args, kwargs)
     # 通过requests库，发送POST请求, local_path是本地文件的绝对路径，remote_path是远程文件的绝对路径
-    url = 'http://%s:5000/upload_image' % ip
-    data = {'user_name': remote_path}
-    files = {'file': open(local_path, 'rb')}
-    try:
+    url = 'http%s5000upload_image' % ip
+    data = {'user_name' remote_path}
+    files = {'file' open(local_path, 'rb')}
+    try
         r = requests.post(url, data=data, files=files, timeout=1)
         print(r.json())
-        if r.json()['code'] == 200:
+        if r.json()['code'] == 200
             return True
-        else:
+        else
             return False
-    except Exception as e:
+    except Exception as e
         print(e)
         return False
     
-if __name__ == '__main__':
+def ssh_upload_face(local_path, remote_path, ip, args, kwargs)
+    # 通过requests库，发送POST请求, local_path是本地文件的绝对路径，remote_path是远程文件的绝对路径
+    url = 'http%s81upload_image' % ip
+    data = {'user_name' remote_path}
+    files = {'file' open(local_path, 'rb')}
+    try
+        r = requests.post(url, data=data, files=files, timeout=1)
+        print(r.json())
+        if r.json()['code'] == 200
+            return True
+        else
+            return False
+    except Exception as e
+        print(e)
+        return False
+    
+if __name__ == '__main__'
     print('删除文件夹')
-    res = ssh_delete_dir('/root/DXR_Project/DXR_FaceRec/face/database/test', '10.10.11.93','root', '123456', port=22)
+    res = ssh_delete_dir('rootDXR_ProjectDXR_FaceRecfacedatabasetest', '10.10.11.93','root', '123456', port=22)
     print(res)
     # print('创建文件夹')
-    # res = ssh_create_dir('/root/DXR_Project/DXR_FaceRec/face/database/test', '10.10.11.93','root', '123456', port=22)
+    # res = ssh_create_dir('rootDXR_ProjectDXR_FaceRecfacedatabasetest', '10.10.11.93','root', '123456', port=22)
     # print(res)
     # print('上传文件')
-    # res = ssh_upload_file('dxr_ssh.py', '/root/DXR_Project/DXR_FaceRec/face/database/test', '10.10.11.93','root', '123456', port=22)
+    # res = ssh_upload_file('dxr_ssh.py', 'rootDXR_ProjectDXR_FaceRecfacedatabasetest', '10.10.11.93','root', '123456', port=22)
     # print(res)
     # print('删除文件')
-    # res = ssh_delete_file('/root/face_tmp/dxr_ssh.py', '10.10.11.93','root', '123456', port=22)
-    # print(res)
-    
-    
+    # res = ssh_delete_file('rootface_tmpdxr_ssh.py', '10.10.11.93','root', '123456', port=22)
+    # print(res)
```

### Comparing `DXR-1.6.8/Dxr_file/dxr_request_ros.py` & `DXR-1.7.0/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_file/dxr_ssh.py` & `DXR-1.7.0/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/Datas_pb2.py` & `DXR-1.7.0/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.7.0/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/audios_pb2.py` & `DXR-1.7.0/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.7.0/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.7.0/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.7.0/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.7.0/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.7.0/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_isapi/api.py` & `DXR-1.7.0/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_isapi/error.py` & `DXR-1.7.0/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_isapi/ir_client.py` & `DXR-1.7.0/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_log/log.py` & `DXR-1.7.0/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.7.0/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.7.0/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_mqtt/msg.py` & `DXR-1.7.0/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_serial/Dxr_serial.py` & `DXR-1.7.0/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_utils/dxr_ftp.py` & `DXR-1.7.0/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_utils/dxr_utils.py` & `DXR-1.7.0/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/Datas_pb2.py` & `DXR-1.7.0/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.7.0/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/HCNetSDK.py` & `DXR-1.7.0/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/PlayCtrl.py` & `DXR-1.7.0/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/test_main.py` & `DXR-1.7.0/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/video.py` & `DXR-1.7.0/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/video_hk.py` & `DXR-1.7.0/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_video/video_server.py` & `DXR-1.7.0/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_voice/dxr_tts.py` & `DXR-1.7.0/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/Dxr_yaml/Dxr_yaml.py` & `DXR-1.7.0/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/README.md` & `DXR-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.6.8/setup.py` & `DXR-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.6.8',
+    version='1.7.0',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

