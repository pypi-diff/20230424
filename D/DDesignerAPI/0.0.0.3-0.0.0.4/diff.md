# Comparing `tmp/DDesignerAPI-0.0.0.3-py3-none-any.whl.zip` & `tmp/DDesignerAPI-0.0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 45794 bytes, number of entries: 19
+Zip file size: 45377 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx      726 b- defN 23-Apr-24 07:15 ddesigner_api/__init__.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Apr-24 07:21 ddesigner_api/tensorflow/__init__.py
 -rw-rw-r--  2.0 unx    11305 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/dpi_blocks.py
 -rw-rw-r--  2.0 unx     6208 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/dpi_layers.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Apr-24 07:21 ddesigner_api/tensorflow/examples/__init__.py
--rw-rw-r--  2.0 unx     1845 b- defN 23-Apr-24 07:04 ddesigner_api/tensorflow/examples/example_keras.py
--rw-rw-r--  2.0 unx     2450 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/examples/example_tensorflow.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-24 07:24 ddesigner_api/tensorflow/examples/__init__.py
+-rw-rw-r--  2.0 unx     1850 b- defN 23-Apr-24 07:25 ddesigner_api/tensorflow/examples/example_keras.py
+-rw-rw-r--  2.0 unx     2458 b- defN 23-Apr-24 07:26 ddesigner_api/tensorflow/examples/example_tensorflow.py
 -rw-rw-r--  2.0 unx      790 b- defN 23-Apr-24 07:16 ddesigner_api/tensorflow/xwn/__init__.py
 -rw-rw-r--  2.0 unx    16306 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/base_conv.py
 -rw-rw-r--  2.0 unx   141656 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/convolutional.py
 -rw-rw-r--  2.0 unx    29694 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/keras_layers.py
 -rw-rw-r--  2.0 unx     4297 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/keras_opt.py
 -rw-rw-r--  2.0 unx     9208 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/tf_nn.py
 -rw-rw-r--  2.0 unx     3440 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/tf_opt.py
--rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 07:22 DDesignerAPI-0.0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 23-Apr-24 07:22 DDesignerAPI-0.0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 07:22 DDesignerAPI-0.0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 07:22 DDesignerAPI-0.0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1792 b- defN 23-Apr-24 07:22 DDesignerAPI-0.0.0.3.dist-info/RECORD
-19 files, 241045 bytes uncompressed, 42794 bytes compressed:  82.2%
+-rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 07:27 DDesignerAPI-0.0.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-Apr-24 07:27 DDesignerAPI-0.0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 07:27 DDesignerAPI-0.0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 07:27 DDesignerAPI-0.0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1790 b- defN 23-Apr-24 07:27 DDesignerAPI-0.0.0.4.dist-info/RECORD
+19 files, 240242 bytes uncompressed, 42377 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: ddesigner_api/tensorflow/xwn/tf_nn.py
 Comment: 
 
 Filename: ddesigner_api/tensorflow/xwn/tf_opt.py
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.3.dist-info/LICENSE
+Filename: DDesignerAPI-0.0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.3.dist-info/METADATA
+Filename: DDesignerAPI-0.0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.3.dist-info/WHEEL
+Filename: DDesignerAPI-0.0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.3.dist-info/top_level.txt
+Filename: DDesignerAPI-0.0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.3.dist-info/RECORD
+Filename: DDesignerAPI-0.0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddesigner_api/tensorflow/examples/__init__.py

```diff
@@ -1,51 +0,0 @@
-00000000: 2320 436f 7079 7269 6768 7420 3230 3233  # Copyright 2023
-00000010: 2054 6865 2044 6565 7065 722d 4920 4175   The Deeper-I Au
-00000020: 7468 6f72 732e 2041 6c6c 2052 6967 6874  thors. All Right
-00000030: 7320 5265 7365 7276 6564 2e0a 230a 2320  s Reserved..#.# 
-00000040: 4c69 6365 6e73 6564 2075 6e64 6572 2074  Licensed under t
-00000050: 6865 2041 7061 6368 6520 4c69 6365 6e73  he Apache Licens
-00000060: 652c 2056 6572 7369 6f6e 2032 2e30 2028  e, Version 2.0 (
-00000070: 7468 6520 224c 6963 656e 7365 2229 3b0a  the "License");.
-00000080: 2320 796f 7520 6d61 7920 6e6f 7420 7573  # you may not us
-00000090: 6520 7468 6973 2066 696c 6520 6578 6365  e this file exce
-000000a0: 7074 2069 6e20 636f 6d70 6c69 616e 6365  pt in compliance
-000000b0: 2077 6974 6820 7468 6520 4c69 6365 6e73   with the Licens
-000000c0: 652e 0a23 2059 6f75 206d 6179 206f 6274  e..# You may obt
-000000d0: 6169 6e20 6120 636f 7079 206f 6620 7468  ain a copy of th
-000000e0: 6520 4c69 6365 6e73 6520 6174 0a23 0a23  e License at.#.#
-000000f0: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
-00000100: 6170 6163 6865 2e6f 7267 2f6c 6963 656e  apache.org/licen
-00000110: 7365 732f 4c49 4345 4e53 452d 322e 300a  ses/LICENSE-2.0.
-00000120: 230a 2320 556e 6c65 7373 2072 6571 7569  #.# Unless requi
-00000130: 7265 6420 6279 2061 7070 6c69 6361 626c  red by applicabl
-00000140: 6520 6c61 7720 6f72 2061 6772 6565 6420  e law or agreed 
-00000150: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
-00000160: 6f66 7477 6172 650a 2320 6469 7374 7269  oftware.# distri
-00000170: 6275 7465 6420 756e 6465 7220 7468 6520  buted under the 
-00000180: 4c69 6365 6e73 6520 6973 2064 6973 7472  License is distr
-00000190: 6962 7574 6564 206f 6e20 616e 2022 4153  ibuted on an "AS
-000001a0: 2049 5322 2042 4153 4953 2c0a 2320 5749   IS" BASIS,.# WI
-000001b0: 5448 4f55 5420 5741 5252 414e 5449 4553  THOUT WARRANTIES
-000001c0: 204f 5220 434f 4e44 4954 494f 4e53 204f   OR CONDITIONS O
-000001d0: 4620 414e 5920 4b49 4e44 2c20 6569 7468  F ANY KIND, eith
-000001e0: 6572 2065 7870 7265 7373 206f 7220 696d  er express or im
-000001f0: 706c 6965 642e 0a23 2053 6565 2074 6865  plied..# See the
-00000200: 204c 6963 656e 7365 2066 6f72 2074 6865   License for the
-00000210: 2073 7065 6369 6669 6320 6c61 6e67 7561   specific langua
-00000220: 6765 2067 6f76 6572 6e69 6e67 2070 6572  ge governing per
-00000230: 6d69 7373 696f 6e73 2061 6e64 0a23 206c  missions and.# l
-00000240: 696d 6974 6174 696f 6e73 2075 6e64 6572  imitations under
-00000250: 2074 6865 204c 6963 656e 7365 2e0a 2320   the License..# 
-00000260: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000270: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000002a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-000002b0: 0a66 726f 6d20 6464 6573 6967 6e65 725f  .from ddesigner_
-000002c0: 6170 692e 7465 6e73 6f72 666c 6f77 2e65  api.tensorflow.e
-000002d0: 7861 6d70 6c65 7320 696d 706f 7274 2065  xamples import e
-000002e0: 7861 6d70 6c65 5f6b 6572 6173 0a66 726f  xample_keras.fro
-000002f0: 6d20 6464 6573 6967 6e65 725f 6170 692e  m ddesigner_api.
-00000300: 7465 6e73 6f72 666c 6f77 2e65 7861 6d70  tensorflow.examp
-00000310: 6c65 7320 696d 706f 7274 2065 7861 6d70  les import examp
-00000320: 6c65 5f74 656e 736f 7266 6c6f 770a       le_tensorflow.
```

## ddesigner_api/tensorflow/examples/example_keras.py

```diff
@@ -15,17 +15,17 @@
 
 import numpy as np
 import tensorflow as tf
 from ddesigner_api.tensorflow.xwn import keras_layers as klayers
 
 
 
-print('====== KERAS ======')
+print('====== KERAS Example======')
 input_shape = (1, 5, 5, 1)
-# x = tf.random.normal(input_shape)
+x = tf.random.normal(input_shape)
 print('====== tf.keras.layers.Conv2D ======')
 c = tf.keras.layers.Conv2D(
     2, 3, activation='relu', 
     kernel_initializer=tf.keras.initializers.RandomUniform(minval=0., maxval=1., seed=87),
     input_shape=input_shape[1:],
     
 )
```

## ddesigner_api/tensorflow/examples/example_tensorflow.py

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 import tensorflow as tf
-from dpi.tensorflow import nn_ops as dpi_nn
+from ddesigner_api.tensorflow.xwn import tf_nn as nn
 
 
 
-print('====== TENSORFLOW ======')
+print('====== TENSORFLOW Example======')
 x_in = np.array([[                                                                            
     [[2], [1], [2], [0], [1]],                                                                  
     [[1], [3], [2], [2], [3]],                                                                  
     [[1], [1], [3], [3], [0]],                                                                  
     [[2], [2], [0], [1], [1]],
     [[0], [0], [3], [1], [2]], ]])                                                              
 kernel_in = np.array([                                                                        
@@ -35,26 +35,26 @@
 
 print('====== tf.nn.conv2d ======')
 print(tf.nn.conv2d(x, kernel, strides=[1, 1, 1, 1], padding='VALID'))
 print('==========================')
 
 print('====== dpi_nn.conv2d (without opt) =====')
 print(
-    dpi_nn.conv2d(
+    nn.conv2d(
         x, 
         kernel, 
         strides=[1, 1, 1, 1], 
         padding='VALID',
     )
 )
 print('==========================')
 
 print('====== dpi_nn.conv2d (with opt) =====')
 print(
-    dpi_nn.conv2d(
+    nn.conv2d(
         x, 
         kernel, 
         strides=[1, 1, 1, 1], 
         padding='VALID',
         transform=True,
         bit=4,
         max_scale=4.0,
```

## Comparing `DDesignerAPI-0.0.0.3.dist-info/LICENSE` & `DDesignerAPI-0.0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DDesignerAPI-0.0.0.3.dist-info/RECORD` & `DDesignerAPI-0.0.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ddesigner_api/__init__.py,sha256=CZXoonSpxauAB_ttNzA-RoRepZ9nPdQZTvYucpWciTg,726
 ddesigner_api/tensorflow/__init__.py,sha256=q4RdbPLAQVOiRpf5H4WNGeTqWu8GbeW9gav3RFLev18,873
 ddesigner_api/tensorflow/dpi_blocks.py,sha256=718HmuyfdB5Xc0q6Dc2AWQs4OFYVbyUxRQSqRJEcC2I,11305
 ddesigner_api/tensorflow/dpi_layers.py,sha256=9MDHfltJ5brfRE7pQhKBE6mnfi3o2jEkvE64hv_IyQc,6208
-ddesigner_api/tensorflow/examples/__init__.py,sha256=Fl-k1lKkNOS8k9mE7sjWTT588nyWzrv7JT34pzYDRv0,814
-ddesigner_api/tensorflow/examples/example_keras.py,sha256=IXMhvMWqc2REI7WbvmAYmR8cSeZURH9BnQLZzU6UrAw,1845
-ddesigner_api/tensorflow/examples/example_tensorflow.py,sha256=OOtNQVBSgowZJcYUEskTwSTcgfwork-W3rrO2bz-fTI,2450
+ddesigner_api/tensorflow/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ddesigner_api/tensorflow/examples/example_keras.py,sha256=9py3TyttAxYPwnJznLMI8xeITX33OjgVnrQ-8wQWUzY,1850
+ddesigner_api/tensorflow/examples/example_tensorflow.py,sha256=abAk371lzA0sgMhI6XSDcn5DrCdoYtz9Prw20j_h9Hw,2458
 ddesigner_api/tensorflow/xwn/__init__.py,sha256=raA9SRLD8OupFBsA2ujBA5xCPTYHS-EO7PYVPIRXL_0,790
 ddesigner_api/tensorflow/xwn/base_conv.py,sha256=dNx2o0KRrIfDz2JZp6dYX6eSGDmMbp7RZ40AdDHseWE,16306
 ddesigner_api/tensorflow/xwn/convolutional.py,sha256=pktLHQezveU36Y3UBzRQ5E0b8Vkt2sC9OYs00MxX6xk,141656
 ddesigner_api/tensorflow/xwn/keras_layers.py,sha256=_I92lFrPy-YzYgZyOMW1uyHom1d9kezb-_xBe-ccu_c,29694
 ddesigner_api/tensorflow/xwn/keras_opt.py,sha256=CN_tlkA4UQWE7JOM1rIfCSWraxnEwyi4L1knoFpoQjM,4297
 ddesigner_api/tensorflow/xwn/tf_nn.py,sha256=24uhIwBzAHqQL3xt4Lkdbsjr1GrCGFlOJxfJEigqVpo,9208
 ddesigner_api/tensorflow/xwn/tf_opt.py,sha256=AEOnTniL95F0yrcl-6gVkokq4KWt5oOAAC0IM358krg,3440
-DDesignerAPI-0.0.0.3.dist-info/LICENSE,sha256=BIg47KsjFz_m25s6T12eL1SAuGkt_KVW_tSqA5yga8g,9136
-DDesignerAPI-0.0.0.3.dist-info/METADATA,sha256=l69b7fS7mwBeBjeqogkgIV0YtomALAUDGsI7Fd6kGTA,399
-DDesignerAPI-0.0.0.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-DDesignerAPI-0.0.0.3.dist-info/top_level.txt,sha256=qYDp5VPzyYyterLRCKrHqsvRLXTHSMOd-Xiwy2HJ_Ow,14
-DDesignerAPI-0.0.0.3.dist-info/RECORD,,
+DDesignerAPI-0.0.0.4.dist-info/LICENSE,sha256=BIg47KsjFz_m25s6T12eL1SAuGkt_KVW_tSqA5yga8g,9136
+DDesignerAPI-0.0.0.4.dist-info/METADATA,sha256=SKv_ouyW5l_T4pflzZo-K9Db5Tlj9FKLup_EelZjeJQ,399
+DDesignerAPI-0.0.0.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+DDesignerAPI-0.0.0.4.dist-info/top_level.txt,sha256=qYDp5VPzyYyterLRCKrHqsvRLXTHSMOd-Xiwy2HJ_Ow,14
+DDesignerAPI-0.0.0.4.dist-info/RECORD,,
```

