# Comparing `tmp/tusuan-0.0.3.tar.gz` & `tmp/tusuan-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tusuan-0.0.3.tar", last modified: Fri Apr 21 16:47:51 2023, max compression
+gzip compressed data, was "tusuan-0.0.4.tar", last modified: Sun Apr 23 09:24:19 2023, max compression
```

## Comparing `tusuan-0.0.3.tar` & `tusuan-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,25 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:47:51.855028 tusuan-0.0.3/
--rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.3/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-04-21 16:47:51.854903 tusuan-0.0.3/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.3/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-21 16:47:51.000000 tusuan-0.0.3/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-04-21 16:47:51.855074 tusuan-0.0.3/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1587 2023-04-21 16:47:24.000000 tusuan-0.0.3/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:47:51.853355 tusuan-0.0.3/tusuan/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.3/tusuan/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.3/tusuan/file_function.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.3/tusuan/hello.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:47:51.854263 tusuan-0.0.3/tusuan/image_video_utils/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.3/tusuan/image_video_utils/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2132 2023-04-21 16:34:53.000000 tusuan-0.0.3/tusuan/image_video_utils/cropper.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      819 2023-03-29 17:22:55.000000 tusuan-0.0.3/tusuan/image_video_utils/display.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.3/tusuan/image_video_utils/image_visual_selector.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:47:51.854750 tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-27 18:37:55.000000 tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1029 2023-03-28 17:38:39.000000 tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/image_reader.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      359 2023-03-28 09:28:38.000000 tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/image_writer.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2181 2023-03-30 07:44:11.000000 tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/video_reader.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1419 2023-03-30 04:51:48.000000 tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/video_writer.py
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.3/tusuan/path_utils.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:47:51.853863 tusuan-0.0.3/tusuan.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-04-21 16:47:51.000000 tusuan-0.0.3/tusuan.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      736 2023-04-21 16:47:51.000000 tusuan-0.0.3/tusuan.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-04-21 16:47:51.000000 tusuan-0.0.3/tusuan.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-21 16:47:51.000000 tusuan-0.0.3/tusuan.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-04-21 16:47:51.000000 tusuan-0.0.3/tusuan.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.484348 tusuan-0.0.4/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.4/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-04-23 09:24:19.484232 tusuan-0.0.4/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.4/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-23 09:24:18.000000 tusuan-0.0.4/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-04-23 09:24:19.484399 tusuan-0.0.4/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1587 2023-04-21 17:22:54.000000 tusuan-0.0.4/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.483019 tusuan-0.0.4/tusuan/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.4/tusuan/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.4/tusuan/file_function.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.4/tusuan/hello.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.484088 tusuan-0.0.4/tusuan/image_video_utils/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.4/tusuan/image_video_utils/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2132 2023-04-21 16:34:53.000000 tusuan-0.0.4/tusuan/image_video_utils/cropper.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      819 2023-03-29 17:22:55.000000 tusuan-0.0.4/tusuan/image_video_utils/display.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.4/tusuan/image_video_utils/image_visual_selector.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     3341 2023-04-21 17:20:22.000000 tusuan-0.0.4/tusuan/image_video_utils/readers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1974 2023-04-21 17:19:04.000000 tusuan-0.0.4/tusuan/image_video_utils/writers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.4/tusuan/path_utils.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.483493 tusuan-0.0.4/tusuan.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      507 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/top_level.txt
```

### Comparing `tusuan-0.0.3/PKG-INFO` & `tusuan-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.3
+Version: 0.0.4
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.3/setup.py` & `tusuan-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from read import read
 from setuptools import setup, find_packages
 
 setup(name='tusuan',  # 包名
       python_requires='>=3.8.0',  # python环境
-      version='0.0.3',  # 包的版本
+      version='0.0.4',  # 包的版本
       description="useful functions.",  # 包简介，显示在PyPI上
 
       long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
       long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
       author="tusuan",  # 作者相关信息
       author_email='btk@qq.com',
```

### Comparing `tusuan-0.0.3/tusuan/file_function.py` & `tusuan-0.0.4/tusuan/file_function.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.3/tusuan/image_video_utils/cropper.py` & `tusuan-0.0.4/tusuan/image_video_utils/cropper.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.3/tusuan/image_video_utils/display.py` & `tusuan-0.0.4/tusuan/image_video_utils/display.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.3/tusuan/image_video_utils/image_visual_selector.py` & `tusuan-0.0.4/tusuan/image_video_utils/image_visual_selector.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.3/tusuan/image_video_utils/readers_and_writers/video_reader.py` & `tusuan-0.0.4/tusuan/image_video_utils/readers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,48 @@
 import sys
 
 import cv2
 import numpy
+from PIL import Image
+
+
+def get_image_info(image_path):
+    """
+    要获取图像的尺寸，最快的方式是使用Pillow库中的Image类，而不是使用OpenCV。
+
+    :param image_path: 图像路径
+    :return:  width, height
+    """
+    with Image.open(image_path) as img:
+        # 获取图像尺寸
+        width, height = img.size
+
+    return height, width
+
+
+def read_image(image_path, grey: bool = False, to_rgb: bool = False):
+    """
+    读取图像函数
+
+    :param image_path: 图像路径
+    :param grey: 是否将图像转换为灰度图像，默认为False
+    :param to_rgb: 是否将图像转换为RGB格式，默认为True
+    :return: 读取到的图像数组
+    """
+    if grey:
+        # 读取灰度图像
+        image = cv2.imread(image_path, cv2.IMREAD_GRAYSCALE)
+    else:
+        # 读取彩色图像
+        image = cv2.imread(image_path)
+        if to_rgb:
+            # 将BGR格式转换为RGB格式
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+
+    return image
 
 
 def get_video_info(video_path):
     """
     获取帧速率、帧数、宽度和高度
     :param video_path: 视频文件地址
     :return: 帧数、宽度、高度和帧速率。如果视频文件无法打开，则返回None。
@@ -14,58 +51,60 @@
     cap = cv2.VideoCapture(video_path)
 
     # 检查视频文件是否成功打开
     if not cap.isOpened():
         return None
 
     # 获取帧速率、帧数、宽度和高度
-    fps = int(cap.get(cv2.CAP_PROP_FPS))
     frames_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+    fps = int(cap.get(cv2.CAP_PROP_FPS))
     height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+    width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
 
     # 释放VideoCapture对象
     cap.release()
 
     # 返回帧数、宽度、高度和帧速率
-    return frames_count, width, height, fps
+    return frames_count, fps, height, width
 
 
-def read_video(video_path, stop: int = sys.maxsize, step: int = 1, to_rgb=True):
+def read_video(video_path, stop: int = sys.maxsize, step: int = 1, to_rgb=False):
     """
     这个函数可以读取视频文件，并返回指定范围内的帧。
 
     :param video_path: 视频文件路径
     :param start: 要读取的起始帧索引（默认为 0）
     :param stop: 要读取的结束帧索引（默认为 sys.maxsize，即读取所有帧）
     :param step: 读取帧的步长（默认为 1）
+    :param to_rgb: 是否转化为RGB图像（默认为 False，保持和cv2返回结果一致）
     :return: 读取成功返回一个代表对应帧所组成的numpy数组，读取失败返回None
     """
     cap = cv2.VideoCapture(video_path)
 
     if not cap.isOpened():
         return None
 
     # 结束帧数不应超过总帧数
-
-    frames_count, width, height, fps = get_video_info(video_path)
+    frames_count = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     stop = min(frames_count, stop)
 
     # cap_iter = iter(lambda: cap.read(), null)
 
     # 按给定的范围读取视频帧
     # 由于视频不能跳帧读取，所以先读取完整的一段，再筛选其中符合特定步长的帧
     video = []
-    for i in range(0, stop):
-        ret, frame = cap.read()
-        if ret:
-            if to_rgb:
-                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-            video.append(frame)
+    for i in range(stop):
+        # 只选取其中符合特定步长的帧
+        if i % step == 0:
+            ret, frame = cap.read()
+            if ret:
+                if to_rgb:
+                    frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                video.append(frame)
         else:
+            ret = cap.grab()
+
+        if not ret:
             break
 
-    # 只选取其中符合特定步长的帧
-    video = video[slice(0, stop, step)]
     cap.release()
-
-    return numpy.stack(video, axis=0), fps
+    return numpy.stack(video, axis=0)
```

### Comparing `tusuan-0.0.3/tusuan.egg-info/PKG-INFO` & `tusuan-0.0.4/tusuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.3
+Version: 0.0.4
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

