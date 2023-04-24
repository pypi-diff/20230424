# Comparing `tmp/DXR-1.7.1.tar.gz` & `tmp/DXR-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.7.1.tar", last modified: Mon Apr 24 05:11:17 2023, max compression
+gzip compressed data, was "DXR-1.7.2.tar", last modified: Mon Apr 24 05:11:58 2023, max compression
```

## Comparing `DXR-1.7.1.tar` & `DXR-1.7.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.850229 DXR-1.7.1/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.788802 DXR-1.7.1/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-24 05:11:17.000000 DXR-1.7.1/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1316 2023-04-24 05:11:17.000000 DXR-1.7.1/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-24 05:11:17.000000 DXR-1.7.1/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-24 05:11:17.000000 DXR-1.7.1/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-24 05:11:17.000000 DXR-1.7.1/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.790711 DXR-1.7.1/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.7.1/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.1/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.1/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.793837 DXR-1.7.1/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.1/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.798613 DXR-1.7.1/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.1/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.1/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3365 2023-04-24 05:11:06.000000 DXR-1.7.1/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.7.1/Dxr_file/dxr_request_ros.py
--r--r--r--   0 luzhipeng   (501) staff       (20)     3414 2023-04-24 05:05:38.000000 DXR-1.7.1/Dxr_file/dxr_requests.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.1/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.811187 DXR-1.7.1/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.1/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.1/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.1/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.1/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.1/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.1/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.1/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.1/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.817924 DXR-1.7.1/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.1/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.7.1/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.1/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.1/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.1/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.821123 DXR-1.7.1/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.828650 DXR-1.7.1/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.1/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.1/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.831241 DXR-1.7.1/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.1/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.835490 DXR-1.7.1/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.845421 DXR-1.7.1/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.847065 DXR-1.7.1/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.1/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.1/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:17.848916 DXR-1.7.1/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.1/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.1/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-24 05:11:17.849606 DXR-1.7.1/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.1/README.md
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 05:11:17.850384 DXR-1.7.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-24 05:11:13.000000 DXR-1.7.1/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.088211 DXR-1.7.2/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.038993 DXR-1.7.2/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-24 05:11:57.000000 DXR-1.7.2/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1316 2023-04-24 05:11:57.000000 DXR-1.7.2/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-24 05:11:57.000000 DXR-1.7.2/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-24 05:11:57.000000 DXR-1.7.2/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      114 2023-04-24 05:11:57.000000 DXR-1.7.2/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.040598 DXR-1.7.2/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.7.2/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.2/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.2/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.042659 DXR-1.7.2/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.2/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.045722 DXR-1.7.2/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.2/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.2/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2724 2023-04-24 05:11:48.000000 DXR-1.7.2/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2715 2023-02-24 03:33:13.000000 DXR-1.7.2/Dxr_file/dxr_request_ros.py
+-r--r--r--   0 luzhipeng   (501) staff       (20)     3414 2023-04-24 05:05:38.000000 DXR-1.7.2/Dxr_file/dxr_requests.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.2/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.050549 DXR-1.7.2/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.2/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.2/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.2/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.2/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.2/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.2/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.2/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.2/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.055227 DXR-1.7.2/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.2/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28811 2023-04-13 01:29:11.000000 DXR-1.7.2/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.2/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.2/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.2/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.058897 DXR-1.7.2/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.068847 DXR-1.7.2/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.2/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.2/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.073451 DXR-1.7.2/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.2/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.077789 DXR-1.7.2/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.083947 DXR-1.7.2/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.084719 DXR-1.7.2/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.2/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.2/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-24 05:11:58.085704 DXR-1.7.2/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.2/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.2/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-24 05:11:58.087731 DXR-1.7.2/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.2/README.md
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 05:11:58.088337 DXR-1.7.2/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      563 2023-04-24 05:11:54.000000 DXR-1.7.2/setup.py
```

### Comparing `DXR-1.7.1/DXR.egg-info/SOURCES.txt` & `DXR-1.7.2/DXR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_Chat/ChatGPT.py` & `DXR-1.7.2/Dxr_Chat/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_Chat/utils.py` & `DXR-1.7.2/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_bytes/Dxr_bytes.py` & `DXR-1.7.2/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_file/dxr_file.py` & `DXR-1.7.2/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_file/dxr_request.py` & `DXR-1.7.2/Dxr_file/dxr_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import requests
 
 # 使用requests库，发送get请求
 def ssh_create_dir(path, ip, *args, **kwargs):
     # 通过requests库，发送POST请求, path是文件的绝对路径
-    url = 'http://%s:6050/add_user' % ip
-    print(f'url is {url}, path is {path}')
+    url = 'http://%s:5000/add_user' % ip
     data = {'user_name': path}
     try:
-        r = requests.get(f'{url}{path.split()[-1]}', timeout=1)
+        r = requests.post(url, data=data, timeout=1)
         print(r.json())
         if r.json()['code'] == 200:
             return True
         else:
             return False
     except Exception as e:
         print(e)
@@ -54,30 +53,14 @@
     data = {'user_name': remote_path}
     files = {'file': open(local_path, 'rb')}
     try:
         r = requests.post(url, data=data, files=files, timeout=1)
         print(r.json())
         if r.json()['code'] == 200:
             return True
-        else:
-            return False
-    except Exception as e:
-        print(e)
-        return False
-
-def ssh_upload_face(local_path, remote_path, ip,, *args, **kwargs):
-    # 通过requests库，发送POST请求, local_path是本地文件的绝对路径，remote_path是远程文件的绝对路径
-    url = 'http://%s:81/upload_image' % ip
-    data = {'user_name': remote_path}
-    files = {'file': open(local_path, 'rb')}
-    try:
-        r = requests.post(url, data=data, files=files, timeout=1)
-        print(r.json())
-        if r.json()['code'] == 200:
-            return True
         else:
             return False
     except Exception as e:
         print(e)
         return False
     
 if __name__ == '__main__':
```

### Comparing `DXR-1.7.1/Dxr_file/dxr_request_ros.py` & `DXR-1.7.2/Dxr_file/dxr_request_ros.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_file/dxr_requests.py` & `DXR-1.7.2/Dxr_file/dxr_requests.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_file/dxr_ssh.py` & `DXR-1.7.2/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/Datas_pb2.py` & `DXR-1.7.2/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.7.2/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/audios_pb2.py` & `DXR-1.7.2/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.7.2/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.7.2/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.7.2/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.7.2/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.7.2/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_isapi/api.py` & `DXR-1.7.2/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_isapi/error.py` & `DXR-1.7.2/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_isapi/ir_client.py` & `DXR-1.7.2/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_log/log.py` & `DXR-1.7.2/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.7.2/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.7.2/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_mqtt/msg.py` & `DXR-1.7.2/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_serial/Dxr_serial.py` & `DXR-1.7.2/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_utils/dxr_ftp.py` & `DXR-1.7.2/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_utils/dxr_utils.py` & `DXR-1.7.2/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/Datas_pb2.py` & `DXR-1.7.2/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.7.2/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/HCNetSDK.py` & `DXR-1.7.2/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/PlayCtrl.py` & `DXR-1.7.2/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/test_main.py` & `DXR-1.7.2/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/video.py` & `DXR-1.7.2/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/video_hk.py` & `DXR-1.7.2/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_video/video_server.py` & `DXR-1.7.2/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_voice/dxr_tts.py` & `DXR-1.7.2/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/Dxr_yaml/Dxr_yaml.py` & `DXR-1.7.2/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/README.md` & `DXR-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.7.1/setup.py` & `DXR-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.7.1',
+    version='1.7.2',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

