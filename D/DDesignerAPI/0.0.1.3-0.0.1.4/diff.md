# Comparing `tmp/DDesignerAPI-0.0.1.3-py3-none-any.whl.zip` & `tmp/DDesignerAPI-0.0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 29798 bytes, number of entries: 18
+Zip file size: 29787 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      726 b- defN 23-Apr-24 07:15 ddesigner_api/__init__.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Apr-24 07:21 ddesigner_api/tensorflow/__init__.py
 -rw-rw-r--  2.0 unx    11329 b- defN 23-Apr-24 10:04 ddesigner_api/tensorflow/dpi_blocks.py
 -rw-rw-r--  2.0 unx     6208 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/dpi_layers.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-24 07:24 ddesigner_api/tensorflow/examples/__init__.py
 -rw-rw-r--  2.0 unx     2328 b- defN 23-Apr-24 10:24 ddesigner_api/tensorflow/examples/examples_keras.py
 -rw-rw-r--  2.0 unx     2953 b- defN 23-Apr-24 10:25 ddesigner_api/tensorflow/examples/examples_tensorflow.py
 -rw-rw-r--  2.0 unx      790 b- defN 23-Apr-24 07:16 ddesigner_api/tensorflow/xwn/__init__.py
 -rw-rw-r--  2.0 unx    16322 b- defN 23-Apr-24 10:13 ddesigner_api/tensorflow/xwn/base_conv.py
 -rw-rw-r--  2.0 unx    29774 b- defN 23-Apr-24 10:03 ddesigner_api/tensorflow/xwn/keras_layers.py
 -rw-rw-r--  2.0 unx     4297 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/keras_opt.py
--rw-rw-r--  2.0 unx     9224 b- defN 23-Apr-24 10:01 ddesigner_api/tensorflow/xwn/tf_nn.py
+-rw-rw-r--  2.0 unx     9240 b- defN 23-Apr-24 10:28 ddesigner_api/tensorflow/xwn/tf_nn.py
 -rw-rw-r--  2.0 unx     3456 b- defN 23-Apr-24 10:00 ddesigner_api/tensorflow/xwn/tf_opt.py
--rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 10:25 DDesignerAPI-0.0.1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2793 b- defN 23-Apr-24 10:25 DDesignerAPI-0.0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 10:25 DDesignerAPI-0.0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 10:25 DDesignerAPI-0.0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1689 b- defN 23-Apr-24 10:25 DDesignerAPI-0.0.1.3.dist-info/RECORD
-18 files, 102004 bytes uncompressed, 26960 bytes compressed:  73.6%
+-rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 10:28 DDesignerAPI-0.0.1.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2793 b- defN 23-Apr-24 10:28 DDesignerAPI-0.0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 10:28 DDesignerAPI-0.0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 10:28 DDesignerAPI-0.0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1689 b- defN 23-Apr-24 10:28 DDesignerAPI-0.0.1.4.dist-info/RECORD
+18 files, 102020 bytes uncompressed, 26949 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: ddesigner_api/tensorflow/xwn/tf_nn.py
 Comment: 
 
 Filename: ddesigner_api/tensorflow/xwn/tf_opt.py
 Comment: 
 
-Filename: DDesignerAPI-0.0.1.3.dist-info/LICENSE
+Filename: DDesignerAPI-0.0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: DDesignerAPI-0.0.1.3.dist-info/METADATA
+Filename: DDesignerAPI-0.0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: DDesignerAPI-0.0.1.3.dist-info/WHEEL
+Filename: DDesignerAPI-0.0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: DDesignerAPI-0.0.1.3.dist-info/top_level.txt
+Filename: DDesignerAPI-0.0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: DDesignerAPI-0.0.1.3.dist-info/RECORD
+Filename: DDesignerAPI-0.0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddesigner_api/tensorflow/xwn/tf_nn.py

```diff
@@ -73,18 +73,18 @@
       A `Tensor`.  Has the same type as input.
     Raises:
       ValueError: if `data_format` is invalid.
     """
     # pylint: enable=line-too-long
     filters = optimization(
         filters, 
-        use_transform=transform, 
+        use_transform=use_transform, 
         bit=bit, 
         max_scale=max_scale,
-        use_pruning=pruning, 
+        use_pruning=use_pruning, 
         prun_weight=prun_weight,
     )
     
     return tf.nn.conv1d(input,  # pylint: disable=redefined-builtin
                   filters,
                   strides,
                   padding,
@@ -95,16 +95,16 @@
 
 def conv2d(input,  # pylint: disable=redefined-builtin
             filters,
             strides,
             padding,
             data_format="NHWC",
             dilations=None,
-            transform=False, 
-            pruning=False, 
+            use_transform=False, 
+            use_pruning=False, 
             bit=4, 
             max_scale=4.0,
             prun_weight=0.5,
             name=None):
 
     # pylint: disable=line-too-long
     r"""Computes a 2-D convolution given `input` and 4-D `filters` tensors.
```

## Comparing `DDesignerAPI-0.0.1.3.dist-info/LICENSE` & `DDesignerAPI-0.0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DDesignerAPI-0.0.1.3.dist-info/METADATA` & `DDesignerAPI-0.0.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DDesignerAPI
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Deep-learning Designer: Deep-Learning Training Optimization & Layers API(like Keras)
 Home-page: https://github.com/DPI/TrainingAPI
 Author: dean
 Author-email: dean@deeper-i.com
 License: Apache-2.0
 Keywords: dpi,xwn,tensorflow,keras
 Platform: UNKNOWN
```

## Comparing `DDesignerAPI-0.0.1.3.dist-info/RECORD` & `DDesignerAPI-0.0.1.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 ddesigner_api/tensorflow/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ddesigner_api/tensorflow/examples/examples_keras.py,sha256=w9nYn7lAglXevTxtoRYxYX2JQ4nwWqJip88WxjmwgoA,2328
 ddesigner_api/tensorflow/examples/examples_tensorflow.py,sha256=vILptIA39fPp6QYql3CvIbcdYR4QSUDuzRqPehhOMhQ,2953
 ddesigner_api/tensorflow/xwn/__init__.py,sha256=raA9SRLD8OupFBsA2ujBA5xCPTYHS-EO7PYVPIRXL_0,790
 ddesigner_api/tensorflow/xwn/base_conv.py,sha256=9ZXF9lkGhxU8K1VX8NRfJstV1t94oqE3iw5PAH3xVwk,16322
 ddesigner_api/tensorflow/xwn/keras_layers.py,sha256=i3ASZIwqOh7qdoazi5sFzeS8URMlpVrB7JMyf49WSSI,29774
 ddesigner_api/tensorflow/xwn/keras_opt.py,sha256=CN_tlkA4UQWE7JOM1rIfCSWraxnEwyi4L1knoFpoQjM,4297
-ddesigner_api/tensorflow/xwn/tf_nn.py,sha256=sUmcNZq48j8o-36jNJvJAqv9QioPDl4mFFJhJbwYnoM,9224
+ddesigner_api/tensorflow/xwn/tf_nn.py,sha256=oaIXhbau-gtFyndce2dF3xWCDOpNhAwCJNLDkR5b5iU,9240
 ddesigner_api/tensorflow/xwn/tf_opt.py,sha256=zxQXkk4oM_tYUSibBGJXzhZt0P-qmHGYxIdmpqCXWfM,3456
-DDesignerAPI-0.0.1.3.dist-info/LICENSE,sha256=BIg47KsjFz_m25s6T12eL1SAuGkt_KVW_tSqA5yga8g,9136
-DDesignerAPI-0.0.1.3.dist-info/METADATA,sha256=T7PAVGKmfLa-tFsLT7aZwo1quzvjV3ty8BbVOUbflBI,2793
-DDesignerAPI-0.0.1.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-DDesignerAPI-0.0.1.3.dist-info/top_level.txt,sha256=qYDp5VPzyYyterLRCKrHqsvRLXTHSMOd-Xiwy2HJ_Ow,14
-DDesignerAPI-0.0.1.3.dist-info/RECORD,,
+DDesignerAPI-0.0.1.4.dist-info/LICENSE,sha256=BIg47KsjFz_m25s6T12eL1SAuGkt_KVW_tSqA5yga8g,9136
+DDesignerAPI-0.0.1.4.dist-info/METADATA,sha256=jJJlxelv-hC1043RQWDxLolMWiScsBTen8_d7jwctaY,2793
+DDesignerAPI-0.0.1.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+DDesignerAPI-0.0.1.4.dist-info/top_level.txt,sha256=qYDp5VPzyYyterLRCKrHqsvRLXTHSMOd-Xiwy2HJ_Ow,14
+DDesignerAPI-0.0.1.4.dist-info/RECORD,,
```

