# Comparing `tmp/easyrv-0.1.8-py3-none-any.whl.zip` & `tmp/easyrv-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 40054 bytes, number of entries: 20
+Zip file size: 40085 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat       89 b- defN 22-Jul-22 02:27 easyrv/__init__.py
--rw-rw-rw-  2.0 fat     6779 b- defN 22-Sep-15 00:01 easyrv/camera_operate.py
+-rw-rw-rw-  2.0 fat     6890 b- defN 23-Mar-20 13:48 easyrv/camera_operate.py
 -rw-rw-rw-  2.0 fat     1420 b- defN 22-Nov-29 02:53 easyrv/data_make.py
 -rw-rw-rw-  2.0 fat     2614 b- defN 22-Sep-10 18:29 easyrv/data_move.py
 -rw-rw-rw-  2.0 fat     1822 b- defN 22-Nov-29 02:51 easyrv/easy_os.py
 -rw-rw-rw-  2.0 fat      720 b- defN 22-Jul-22 02:43 easyrv/image_draw.py
 -rw-rw-rw-  2.0 fat      860 b- defN 23-Mar-03 02:43 easyrv/image_trans.py
 -rw-rw-rw-  2.0 fat      126 b- defN 22-Jul-22 00:33 easyrv/rv_hello.py
 -rw-rw-rw-  2.0 fat     5917 b- defN 22-Sep-27 14:44 easyrv/MvImport/CameraParams_const.py
 -rw-rw-rw-  2.0 fat    56524 b- defN 22-Oct-11 00:56 easyrv/MvImport/CameraParams_header.py
 -rw-rw-rw-  2.0 fat    43834 b- defN 22-Oct-11 00:56 easyrv/MvImport/MvCameraControl_class.py
 -rw-rw-rw-  2.0 fat    33504 b- defN 22-May-11 04:07 easyrv/MvImport/MvCameraControl_header.py
 -rw-rw-rw-  2.0 fat     6784 b- defN 22-Sep-27 14:44 easyrv/MvImport/MvErrorDefine_const.py
 -rw-rw-rw-  2.0 fat      701 b- defN 22-May-11 04:07 easyrv/MvImport/PixelType_const.py
 -rw-rw-rw-  2.0 fat     7250 b- defN 22-Sep-27 14:44 easyrv/MvImport/PixelType_header.py
 -rw-rw-rw-  2.0 fat      109 b- defN 22-Sep-10 18:33 easyrv/MvImport/__init__.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Mar-03 02:43 easyrv-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-03 02:43 easyrv-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-03 02:43 easyrv-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1646 b- defN 23-Mar-03 02:43 easyrv-0.1.8.dist-info/RECORD
-20 files, 171183 bytes uncompressed, 37372 bytes compressed:  78.2%
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Mar-20 13:48 easyrv-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-20 13:48 easyrv-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-20 13:48 easyrv-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1646 b- defN 23-Mar-20 13:48 easyrv-0.1.9.dist-info/RECORD
+20 files, 171294 bytes uncompressed, 37403 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: easyrv/MvImport/PixelType_header.py
 Comment: 
 
 Filename: easyrv/MvImport/__init__.py
 Comment: 
 
-Filename: easyrv-0.1.8.dist-info/METADATA
+Filename: easyrv-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: easyrv-0.1.8.dist-info/WHEEL
+Filename: easyrv-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: easyrv-0.1.8.dist-info/top_level.txt
+Filename: easyrv-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: easyrv-0.1.8.dist-info/RECORD
+Filename: easyrv-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## easyrv/camera_operate.py

```diff
@@ -106,15 +106,15 @@
         ret = self._cam.MV_CC_StartGrabbing()
         if ret != 0:
             print("start grabbing fail! ret[0x%x]" % ret)
         #  返回获取图像缓存区。
         self._data_buf = (c_ubyte * self._nPayloadSize)()
         #  date_buf前面的转化不用，不然报错，因为转了是浮点型
 
-    def get_image(self, exposure_time=20000, frame_rate=60, reverse_x=False, reverse_y=False):
+    def get_image(self, color='RGB', exposure_time=20000, frame_rate=60, reverse_x=False, reverse_y=False):
         # --------------- 设置曝光时间 和 缓冲区信息 -----------------------------------
         st_frame_info = MV_FRAME_OUT_INFO_EX()
         memset(byref(st_frame_info), 0, sizeof(st_frame_info))
 
         st_float_param_exposure_time = MVCC_FLOATVALUE()
         memset(byref(st_float_param_exposure_time), 0, sizeof(MVCC_FLOATVALUE))
 
@@ -125,14 +125,16 @@
 
         # 采用超时机制获取一帧图片，SDK内部等待直到有数据时返回，成功返回0
         ret = self._cam.MV_CC_GetOneFrameTimeout(self._data_buf, self._nPayloadSize, st_frame_info, 1000)
 
         self.image = np.asarray(self._data_buf)  # 将c_ubyte_Array转化成ndarray得到（3686400，）
         self.image = self.image.reshape((st_frame_info.nHeight, st_frame_info.nWidth, -1))  # 根据自己分辨率进行转化
         self.image = cv2.cvtColor(self.image, cv2.COLOR_BAYER_BG2RGB)
+        if color == 'BGR':
+            self.image = cv2.cvtColor(self.image, cv2.COLOR_RGB2BGR)
         return self.image
 
     def close_device(self):
         """
         关闭设备
         """
         # ch:停止取流 | en:Stop grab image
```

## Comparing `easyrv-0.1.8.dist-info/RECORD` & `easyrv-0.1.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 easyrv/__init__.py,sha256=nWvZts59NfkR2Trum6czHevAy2WQnuIvnMyF6FiKQa8,89
-easyrv/camera_operate.py,sha256=l9K8NqiJmsqWJZ7vjUkO0PybStQCkh-5xa9mbg_-dtA,6779
+easyrv/camera_operate.py,sha256=UWQ5pnrXB4tYOdOtRk0OdrGoGwySl2aY39lrTGyiga4,6890
 easyrv/data_make.py,sha256=vTLLGwwo2j6WZiEL03aTIdkSKajpqNNOXVii_1wIAIg,1420
 easyrv/data_move.py,sha256=gg1e24ogqFODPcP-gEHyqTn_FetF7ox4nKMRfFrNIfc,2614
 easyrv/easy_os.py,sha256=uYbb3yDlcFL0WGDZRxyinGk8L-Gqe0r5SFJPYdFr50k,1822
 easyrv/image_draw.py,sha256=U_9wenVPfpdyD1-JB_cAbFD5bypp4WPJQzKlRokldME,720
 easyrv/image_trans.py,sha256=U3Mv4wwM0t-8X-b5BKv-JpU_Z_pV8j7LP78l88sCqxM,860
 easyrv/rv_hello.py,sha256=R6HfAqSj11Be2tNTqmbAKC2zGr75iAkEAq_nf8XKpxk,126
 easyrv/MvImport/CameraParams_const.py,sha256=oTSdRG_Ox0ZJ87Ex06YAreYPyv9JtCCjODqoBkuHD38,5917
 easyrv/MvImport/CameraParams_header.py,sha256=mQ-GFnp__eRiX4iU15ajQjjg5ETSppbkDJY_YwwhhTE,56524
 easyrv/MvImport/MvCameraControl_class.py,sha256=pkJMxQYhFfUK75Nz5R7sF2MJXrcjMRMPnpy0BKVIezs,43834
 easyrv/MvImport/MvCameraControl_header.py,sha256=d8tldHl-Nq7FEVqUoD0AqQ0bq35sbDdzZesQILVmGrE,33504
 easyrv/MvImport/MvErrorDefine_const.py,sha256=2NN4K-Ia2WVhQXJVadRqhxDs3siE11W0dp6QaOwVtdI,6784
 easyrv/MvImport/PixelType_const.py,sha256=IUWc2edlzaMvMyOZA3lUR7kalGfqUyWwjJuC0D74FG0,701
 easyrv/MvImport/PixelType_header.py,sha256=s_HH1abif18BrpIsCHa_rtbbs8bYEXjWd2hzEV4QlyI,7250
 easyrv/MvImport/__init__.py,sha256=g-rIj80UQmWr_2B9kXE7028wJ0nVGgGdIgxS3oS_24s,109
-easyrv-0.1.8.dist-info/METADATA,sha256=NSwB0p2xmqMzajPbC_koFaTyYv2oKb7MWy10WYM3ywM,385
-easyrv-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-easyrv-0.1.8.dist-info/top_level.txt,sha256=cgZx71fOwfnw3uyr2WPjedZqUGu89bjgXZHw-LzVnyY,7
-easyrv-0.1.8.dist-info/RECORD,,
+easyrv-0.1.9.dist-info/METADATA,sha256=5Dea5Rk8kOQsJUOc9ltUfaZIVk4OPASwc7jk29lH76U,385
+easyrv-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+easyrv-0.1.9.dist-info/top_level.txt,sha256=cgZx71fOwfnw3uyr2WPjedZqUGu89bjgXZHw-LzVnyY,7
+easyrv-0.1.9.dist-info/RECORD,,
```

