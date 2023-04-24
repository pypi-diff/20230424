# Comparing `tmp/DDesignerAPI-0.0.0.5-py3-none-any.whl.zip` & `tmp/DDesignerAPI-0.0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 45481 bytes, number of entries: 19
+Zip file size: 45707 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx      726 b- defN 23-Apr-24 07:15 ddesigner_api/__init__.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Apr-24 07:21 ddesigner_api/tensorflow/__init__.py
 -rw-rw-r--  2.0 unx    11305 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/dpi_blocks.py
 -rw-rw-r--  2.0 unx     6208 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/dpi_layers.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-24 07:24 ddesigner_api/tensorflow/examples/__init__.py
--rw-rw-r--  2.0 unx     2077 b- defN 23-Apr-24 07:33 ddesigner_api/tensorflow/examples/examples_keras.py
--rw-rw-r--  2.0 unx     2702 b- defN 23-Apr-24 07:34 ddesigner_api/tensorflow/examples/examples_tensorflow.py
+-rw-rw-r--  2.0 unx     2361 b- defN 23-Apr-24 07:51 ddesigner_api/tensorflow/examples/examples_keras.py
+-rw-rw-r--  2.0 unx     2986 b- defN 23-Apr-24 07:52 ddesigner_api/tensorflow/examples/examples_tensorflow.py
 -rw-rw-r--  2.0 unx      790 b- defN 23-Apr-24 07:16 ddesigner_api/tensorflow/xwn/__init__.py
 -rw-rw-r--  2.0 unx    16306 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/base_conv.py
 -rw-rw-r--  2.0 unx   141656 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/convolutional.py
 -rw-rw-r--  2.0 unx    29694 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/keras_layers.py
 -rw-rw-r--  2.0 unx     4297 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/keras_opt.py
 -rw-rw-r--  2.0 unx     9208 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/tf_nn.py
 -rw-rw-r--  2.0 unx     3440 b- defN 23-Apr-24 05:44 ddesigner_api/tensorflow/xwn/tf_opt.py
--rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 07:35 DDesignerAPI-0.0.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      399 b- defN 23-Apr-24 07:35 DDesignerAPI-0.0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 07:35 DDesignerAPI-0.0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 07:35 DDesignerAPI-0.0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1792 b- defN 23-Apr-24 07:35 DDesignerAPI-0.0.0.5.dist-info/RECORD
-19 files, 240715 bytes uncompressed, 42477 bytes compressed:  82.4%
+-rwxrwxr-x  2.0 unx     9136 b- defN 23-Apr-24 07:53 DDesignerAPI-0.0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      399 b- defN 23-Apr-24 07:53 DDesignerAPI-0.0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 07:53 DDesignerAPI-0.0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 07:53 DDesignerAPI-0.0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1792 b- defN 23-Apr-24 07:53 DDesignerAPI-0.0.0.6.dist-info/RECORD
+19 files, 241283 bytes uncompressed, 42703 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: ddesigner_api/tensorflow/xwn/tf_nn.py
 Comment: 
 
 Filename: ddesigner_api/tensorflow/xwn/tf_opt.py
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.5.dist-info/LICENSE
+Filename: DDesignerAPI-0.0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.5.dist-info/METADATA
+Filename: DDesignerAPI-0.0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.5.dist-info/WHEEL
+Filename: DDesignerAPI-0.0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.5.dist-info/top_level.txt
+Filename: DDesignerAPI-0.0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: DDesignerAPI-0.0.0.5.dist-info/RECORD
+Filename: DDesignerAPI-0.0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddesigner_api/tensorflow/examples/examples_keras.py

```diff
@@ -54,10 +54,28 @@
         input_shape=input_shape[1:], 
     )
     y = c(x)
     print(y)
     print('==========================')
 
 
-if __name__ == '__main__':
+def main(args):
     print('====== KERAS Examples======')
-    print('1. random_input')
+    print('1. Random Input')
+    print('Q. Quit')
+
+    cmd = '1'
+    while True:
+        print('>>> Select Test:')
+        cmd = input()
+        if cmd == '1':
+            random_input()
+        elif cmd == 'Q': 
+            break
+        
+    return True
+
+
+
+if __name__ == '__main__':
+    import sys
+    main(sys.argv[1:])
```

## ddesigner_api/tensorflow/examples/examples_tensorflow.py

```diff
@@ -58,10 +58,29 @@
             transform=True,
             bit=4,
             max_scale=4.0,
         )
     )
     print('==========================')
 
-if __name__ == '__main__':
+
+def main(args):
     print('====== TENSORFLOW Examples======')
-    print('1. fixed input')
+    print('1. Fixed Input')
+    print('Q. Quit')
+
+    cmd = '1'
+    while True:
+        print('>>> Select Test:')
+        cmd = input()
+        if cmd == '1':
+            fixed_input()
+        elif cmd == 'Q': 
+            break
+        
+    return True
+
+
+
+if __name__ == '__main__':
+    import sys
+    main(sys.argv[1:])
```

## Comparing `DDesignerAPI-0.0.0.5.dist-info/LICENSE` & `DDesignerAPI-0.0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `DDesignerAPI-0.0.0.5.dist-info/RECORD` & `DDesignerAPI-0.0.0.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ddesigner_api/__init__.py,sha256=CZXoonSpxauAB_ttNzA-RoRepZ9nPdQZTvYucpWciTg,726
 ddesigner_api/tensorflow/__init__.py,sha256=q4RdbPLAQVOiRpf5H4WNGeTqWu8GbeW9gav3RFLev18,873
 ddesigner_api/tensorflow/dpi_blocks.py,sha256=718HmuyfdB5Xc0q6Dc2AWQs4OFYVbyUxRQSqRJEcC2I,11305
 ddesigner_api/tensorflow/dpi_layers.py,sha256=9MDHfltJ5brfRE7pQhKBE6mnfi3o2jEkvE64hv_IyQc,6208
 ddesigner_api/tensorflow/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ddesigner_api/tensorflow/examples/examples_keras.py,sha256=Xy5OZHPA8sDVVn7NZ9S_Z1P7ysWZXc3X95uao-E8-1I,2077
-ddesigner_api/tensorflow/examples/examples_tensorflow.py,sha256=AgJBRgVf-V27DpHPuCJMlKXRpOUneaWUQhLX6tYcjjk,2702
+ddesigner_api/tensorflow/examples/examples_keras.py,sha256=ZNDiT2tCe_DT6pmkcIOgmmsRg_WJN7l6j6cHTBCMA68,2361
+ddesigner_api/tensorflow/examples/examples_tensorflow.py,sha256=4YagzdPAzJKG7ySmP3k2uhKnnK9e5DDiJIv8aefBOe4,2986
 ddesigner_api/tensorflow/xwn/__init__.py,sha256=raA9SRLD8OupFBsA2ujBA5xCPTYHS-EO7PYVPIRXL_0,790
 ddesigner_api/tensorflow/xwn/base_conv.py,sha256=dNx2o0KRrIfDz2JZp6dYX6eSGDmMbp7RZ40AdDHseWE,16306
 ddesigner_api/tensorflow/xwn/convolutional.py,sha256=pktLHQezveU36Y3UBzRQ5E0b8Vkt2sC9OYs00MxX6xk,141656
 ddesigner_api/tensorflow/xwn/keras_layers.py,sha256=_I92lFrPy-YzYgZyOMW1uyHom1d9kezb-_xBe-ccu_c,29694
 ddesigner_api/tensorflow/xwn/keras_opt.py,sha256=CN_tlkA4UQWE7JOM1rIfCSWraxnEwyi4L1knoFpoQjM,4297
 ddesigner_api/tensorflow/xwn/tf_nn.py,sha256=24uhIwBzAHqQL3xt4Lkdbsjr1GrCGFlOJxfJEigqVpo,9208
 ddesigner_api/tensorflow/xwn/tf_opt.py,sha256=AEOnTniL95F0yrcl-6gVkokq4KWt5oOAAC0IM358krg,3440
-DDesignerAPI-0.0.0.5.dist-info/LICENSE,sha256=BIg47KsjFz_m25s6T12eL1SAuGkt_KVW_tSqA5yga8g,9136
-DDesignerAPI-0.0.0.5.dist-info/METADATA,sha256=vjwHugDKgFJOAMusTt8qu0U96cEnvT3wDVZobEX1Nyg,399
-DDesignerAPI-0.0.0.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-DDesignerAPI-0.0.0.5.dist-info/top_level.txt,sha256=qYDp5VPzyYyterLRCKrHqsvRLXTHSMOd-Xiwy2HJ_Ow,14
-DDesignerAPI-0.0.0.5.dist-info/RECORD,,
+DDesignerAPI-0.0.0.6.dist-info/LICENSE,sha256=BIg47KsjFz_m25s6T12eL1SAuGkt_KVW_tSqA5yga8g,9136
+DDesignerAPI-0.0.0.6.dist-info/METADATA,sha256=xljGNcEQcFq_YaYQRu3VnQllpLJ67q8xY3ZmDUHBxqg,399
+DDesignerAPI-0.0.0.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+DDesignerAPI-0.0.0.6.dist-info/top_level.txt,sha256=qYDp5VPzyYyterLRCKrHqsvRLXTHSMOd-Xiwy2HJ_Ow,14
+DDesignerAPI-0.0.0.6.dist-info/RECORD,,
```

