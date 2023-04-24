# Comparing `tmp/ravdl-0.8.tar.gz` & `tmp/ravdl-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ravdl-0.8.tar", last modified: Fri Sep 16 10:11:29 2022, max compression
+gzip compressed data, was "ravdl-0.9.tar", last modified: Fri Oct 14 08:38:14 2022, max compression
```

## Comparing `ravdl-0.8.tar` & `ravdl-0.9.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.163897 ravdl-0.8/
--rw-r--r--   0 apple      (501) staff       (20)     1070 2022-07-14 10:02:21.000000 ravdl-0.8/LICENSE.rst
--rw-r--r--   0 apple      (501) staff       (20)    10866 2022-09-16 10:11:29.164081 ravdl-0.8/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)    10540 2022-09-15 13:15:54.000000 ravdl-0.8/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.149981 ravdl-0.8/ravdl/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-07-14 10:12:19.000000 ravdl-0.8/ravdl/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      746 2022-07-14 10:11:09.000000 ravdl-0.8/ravdl/globals.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.154672 ravdl-0.8/ravdl/utils/
--rw-r--r--   0 apple      (501) staff       (20)       84 2022-07-14 10:11:09.000000 ravdl-0.8/ravdl/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      379 2022-07-14 10:11:09.000000 ravdl-0.8/ravdl/utils/data_manipulation.py
--rw-r--r--   0 apple      (501) staff       (20)      260 2022-07-14 10:11:09.000000 ravdl-0.8/ravdl/utils/data_operations.py
--rw-r--r--   0 apple      (501) staff       (20)      433 2022-07-14 10:11:09.000000 ravdl-0.8/ravdl/utils/misc.py
--rw-r--r--   0 apple      (501) staff       (20)      433 2022-07-14 10:11:09.000000 ravdl-0.8/ravdl/utils_singleton.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.159790 ravdl-0.8/ravdl/v1/
--rw-r--r--   0 apple      (501) staff       (20)     7563 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/NeuralNetwork.py
--rw-r--r--   0 apple      (501) staff       (20)       41 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      970 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/activation_functions.py
--rw-r--r--   0 apple      (501) staff       (20)    33633 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/layers.py
--rw-r--r--   0 apple      (501) staff       (20)     8182 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/load_onnx_model.py
--rw-r--r--   0 apple      (501) staff       (20)     1105 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/loss_functions.py
--rw-r--r--   0 apple      (501) staff       (20)     1598 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v1/optimizers.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.162146 ravdl-0.8/ravdl/v2/
--rw-r--r--   0 apple      (501) staff       (20)     8519 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/NeuralNetwork.py
--rw-r--r--   0 apple      (501) staff       (20)       40 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    12319 2022-09-16 10:10:35.000000 ravdl-0.8/ravdl/v2/layers.py
--rw-r--r--   0 apple      (501) staff       (20)     1092 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/loss_functions.py
--rw-r--r--   0 apple      (501) staff       (20)      918 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/optimizers.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.163554 ravdl-0.8/ravdl/v2/utils/
--rw-r--r--   0 apple      (501) staff       (20)       64 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)      379 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/utils/data_manipulation.py
--rw-r--r--   0 apple      (501) staff       (20)     1067 2022-09-15 13:15:54.000000 ravdl-0.8/ravdl/v2/utils/data_operations.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-09-16 10:11:29.152266 ravdl-0.8/ravdl.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)    10866 2022-09-16 10:11:28.000000 ravdl-0.8/ravdl.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      742 2022-09-16 10:11:29.000000 ravdl-0.8/ravdl.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2022-09-16 10:11:28.000000 ravdl-0.8/ravdl.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       70 2022-09-16 10:11:28.000000 ravdl-0.8/ravdl.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2022-09-16 10:11:28.000000 ravdl-0.8/ravdl.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      107 2022-09-16 10:11:29.164791 ravdl-0.8/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      693 2022-09-16 10:11:21.000000 ravdl-0.8/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-14 08:38:14.805264 ravdl-0.9/
+-rw-r--r--   0 apple      (501) staff       (20)     1070 2022-07-14 10:02:21.000000 ravdl-0.9/LICENSE.rst
+-rw-r--r--   0 apple      (501) staff       (20)    10866 2022-10-14 08:38:14.805480 ravdl-0.9/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)    10540 2022-09-15 13:15:54.000000 ravdl-0.9/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-14 08:38:14.789767 ravdl-0.9/ravdl/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-07-14 10:12:19.000000 ravdl-0.9/ravdl/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      746 2022-07-14 10:11:09.000000 ravdl-0.9/ravdl/globals.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-14 08:38:14.794451 ravdl-0.9/ravdl/utils/
+-rw-r--r--   0 apple      (501) staff       (20)       84 2022-07-14 10:11:09.000000 ravdl-0.9/ravdl/utils/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      379 2022-07-14 10:11:09.000000 ravdl-0.9/ravdl/utils/data_manipulation.py
+-rw-r--r--   0 apple      (501) staff       (20)     1067 2022-10-14 08:35:43.000000 ravdl-0.9/ravdl/utils/data_operations.py
+-rw-r--r--   0 apple      (501) staff       (20)      433 2022-07-14 10:11:09.000000 ravdl-0.9/ravdl/utils/misc.py
+-rw-r--r--   0 apple      (501) staff       (20)      433 2022-07-14 10:11:09.000000 ravdl-0.9/ravdl/utils_singleton.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-14 08:38:14.800146 ravdl-0.9/ravdl/v1/
+-rw-r--r--   0 apple      (501) staff       (20)     7563 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v1/NeuralNetwork.py
+-rw-r--r--   0 apple      (501) staff       (20)       41 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v1/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)      970 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v1/activation_functions.py
+-rw-r--r--   0 apple      (501) staff       (20)    33633 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v1/layers.py
+-rw-r--r--   0 apple      (501) staff       (20)     8182 2022-10-14 08:35:43.000000 ravdl-0.9/ravdl/v1/load_onnx_model.py
+-rw-r--r--   0 apple      (501) staff       (20)     1105 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v1/loss_functions.py
+-rw-r--r--   0 apple      (501) staff       (20)     1598 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v1/optimizers.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-14 08:38:14.804758 ravdl-0.9/ravdl/v2/
+-rw-r--r--   0 apple      (501) staff       (20)     8283 2022-10-14 08:35:43.000000 ravdl-0.9/ravdl/v2/NeuralNetwork.py
+-rw-r--r--   0 apple      (501) staff       (20)       40 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v2/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    21095 2022-10-14 08:35:43.000000 ravdl-0.9/ravdl/v2/layers.py
+-rw-r--r--   0 apple      (501) staff       (20)     8832 2022-10-14 08:35:43.000000 ravdl-0.9/ravdl/v2/load_onnx_model.py
+-rw-r--r--   0 apple      (501) staff       (20)     1093 2022-10-14 08:35:43.000000 ravdl-0.9/ravdl/v2/loss_functions.py
+-rw-r--r--   0 apple      (501) staff       (20)      918 2022-09-15 13:15:54.000000 ravdl-0.9/ravdl/v2/optimizers.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-14 08:38:14.791941 ravdl-0.9/ravdl.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)    10866 2022-10-14 08:38:14.000000 ravdl-0.9/ravdl.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      673 2022-10-14 08:38:14.000000 ravdl-0.9/ravdl.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2022-10-14 08:38:14.000000 ravdl-0.9/ravdl.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       70 2022-10-14 08:38:14.000000 ravdl-0.9/ravdl.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        6 2022-10-14 08:38:14.000000 ravdl-0.9/ravdl.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)      107 2022-10-14 08:38:14.806301 ravdl-0.9/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      693 2022-10-14 08:36:56.000000 ravdl-0.9/setup.py
```

### Comparing `ravdl-0.8/LICENSE.rst` & `ravdl-0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/PKG-INFO` & `ravdl-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravdl
-Version: 0.8
+Version: 0.9
 Summary: UNKNOWN
 Home-page: https://github.com/ravenprotocol/ravdl
 Author: Raven Protocol
 Author-email: kailash@ravenprotocol.com
 License: MIT
 Keywords: Ravdl,deep learning library,algorithms
 Platform: UNKNOWN
```

### Comparing `ravdl-0.8/README.md` & `ravdl-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/globals.py` & `ravdl-0.9/ravdl/globals.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v1/NeuralNetwork.py` & `ravdl-0.9/ravdl/v1/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v1/activation_functions.py` & `ravdl-0.9/ravdl/v1/activation_functions.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v1/layers.py` & `ravdl-0.9/ravdl/v1/layers.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v1/load_onnx_model.py` & `ravdl-0.9/ravdl/v1/load_onnx_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 from .NeuralNetwork import NeuralNetwork
 from .layers import BatchNormalization, Dense, Activation, Flatten, MaxPooling2D, Dropout, Conv2D
 import onnx
 from onnx import numpy_helper
 from onnx import shape_inference
-import ravop.ravop as R
+import ravop as R
 
 def load_onnx(loss=None, optimizer=None, model_file_path=None):
     onnx_model = onnx.load(model_file_path)
     infer_model = shape_inference.infer_shapes(onnx_model)
-    print(infer_model.graph.value_info[0].type.tensor_type.shape)
+    # print(infer_model.graph.value_info[0].type.tensor_type.shape)
 
 
     input_all = [node.name for node in onnx_model.graph.input]
     input_initializer =  [node.name for node in onnx_model.graph.initializer]
     net_feed_input = list(set(input_all)  - set(input_initializer))
     input_shape = []
     for net_input in net_feed_input:
@@ -177,15 +177,15 @@
                 if attr.name == 'kernel_shape':
                     kernel_shape = attr.ints
                 # !!!!!!!!!!! To be added later !!!!!!!!!!!
                 # elif attr.name == 'strides': 
                 #     strides = attr.ints
                 # elif attr.name == 'pads':
                 #     pads = attr.ints
-            print("kernel_shape: ", kernel_shape)
+            # print("kernel_shape: ", kernel_shape)
             if input_flag:
                 model.add(Conv2D(W.shape[0], filter_shape=tuple(kernel_shape), input_shape=input_shape))
             else:
                 model.add(Conv2D(W.shape[0], filter_shape=tuple(kernel_shape)))
 
             model.layers[-1].W = R.t(W)
             model.layers[-1].w0 = R.t(w0)
@@ -197,15 +197,15 @@
                     kernel_shape = attr.ints
                 
                 elif attr.name == 'strides': 
                     stride = attr.ints[0]
                 # !!!!!!!!!!! To be added later !!!!!!!!!!!
                 # elif attr.name == 'pads':
                 #     pads = attr.ints
-            print("kernel_shape: ", kernel_shape)
+            # print("kernel_shape: ", kernel_shape)
             if input_flag:
                 model.add(MaxPooling2D(pool_shape=kernel_shape, stride=stride, input_shape = input_shape))
             else:
                 model.add(MaxPooling2D(pool_shape=kernel_shape, stride=stride))
```

### Comparing `ravdl-0.8/ravdl/v1/loss_functions.py` & `ravdl-0.9/ravdl/v1/loss_functions.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v1/optimizers.py` & `ravdl-0.9/ravdl/v1/optimizers.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v2/NeuralNetwork.py` & `ravdl-0.9/ravdl/v2/NeuralNetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ravop as R
 import onnx
 from terminaltables import AsciiTable
-from .utils.data_manipulation import batch_iterator
+from ..utils.data_manipulation import batch_iterator
 
 loss_op_mapping = {
     'SquareLoss': {
         'loss': R.square_loss,
         # 'accuracy': R.square_loss_accuracy,
         'gradient': R.square_loss_gradient
     },
@@ -90,34 +90,31 @@
         loss_grad = self.loss_function['gradient'](y, y_pred)  #R.cross_entropy_gradient(y, y_pred)
         # print('   Loss Gradient: ', loss_grad())
         # Backpropagate. Update weights
         self._backward_pass(loss_grad=loss_grad)
 
         return loss #, acc
 
-    def fit(self, X, y, n_epochs, batch_size, save_model = False, persist_weights=False):
+    def fit(self, X, y, n_epochs, batch_size, save_model = False):
         """ Trains the model for a fixed number of epochs """
         for epoch in range(1, n_epochs + 1):
             print('\nEpoch: ', epoch)
             batch_error = []
             batch_num = 1
             for X_batch, y_batch in batch_iterator(X, y, batch_size=batch_size):
                 loss = self.train_on_batch(X_batch, y_batch)
                 loss.persist_op(name = "training_loss_epoch_{}_batch_{}".format(epoch,batch_num))
                 batch_num += 1
 
             # if self.val_set is not None:
             #     val_loss, _ = self.test_on_batch(self.val_set["X"], self.val_set["y"])
             #     val_loss.persist_op(name="val_loss_epoch_{}".format(epoch))
         
-        if persist_weights:
-            self.persist_model()
-
-        # if save_model:
-        #     self.save_model()
+        if save_model:
+            self.save_model()
             
     def _forward_pass(self, X, training=True):
         """ Calculate the output of the NN """
         layer_output = X
         for layer in self.layers:
             if layer == self.layers[0]:
                 layer_output = layer._forward_pass(layer_output, input_layer="True", training = training)
@@ -154,24 +151,19 @@
         print (AsciiTable(table_data).table)
         print ("Total Parameters: %d\n" % tot_params)
 
     def predict(self, X):
         """ Use the trained model to predict labels of X """
         X = R.t(X)
         return self._forward_pass(X, training=False)
-
-    def persist_model(self):
-        """ Save the model's weights to a file """
-        for layer in self.layers:
-            layer.persist_weights()
     
     def save_model(self):
         """ Save the model's weights to a file """
         for layer in self.layers:
-            layer.save_weights()
+            layer.persist_weights()
 
     def get_onnx_model(self, model_name):
         """ Get an ONNX model of the network """
         model_input_name = "X"
         input_shape = [None]
         input_shape.extend(list(self.layers[0].input_shape))
```

### Comparing `ravdl-0.8/ravdl/v2/loss_functions.py` & `ravdl-0.9/ravdl/v2/loss_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import division
 import ravop as R
-from .utils.data_operations import accuracy_score
+from ..utils.data_operations import accuracy_score
 
 class Loss(object):
     def loss(self, y_true, y_pred):
         return NotImplementedError()
 
     def gradient(self, y, y_pred):
         raise NotImplementedError()
```

### Comparing `ravdl-0.8/ravdl/v2/optimizers.py` & `ravdl-0.9/ravdl/v2/optimizers.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl/v2/utils/data_operations.py` & `ravdl-0.9/ravdl/utils/data_operations.py`

 * *Files identical despite different names*

### Comparing `ravdl-0.8/ravdl.egg-info/PKG-INFO` & `ravdl-0.9/ravdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ravdl
-Version: 0.8
+Version: 0.9
 Summary: UNKNOWN
 Home-page: https://github.com/ravenprotocol/ravdl
 Author: Raven Protocol
 Author-email: kailash@ravenprotocol.com
 License: MIT
 Keywords: Ravdl,deep learning library,algorithms
 Platform: UNKNOWN
```

### Comparing `ravdl-0.8/ravdl.egg-info/SOURCES.txt` & `ravdl-0.9/ravdl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,10 @@
 ravdl/v1/layers.py
 ravdl/v1/load_onnx_model.py
 ravdl/v1/loss_functions.py
 ravdl/v1/optimizers.py
 ravdl/v2/NeuralNetwork.py
 ravdl/v2/__init__.py
 ravdl/v2/layers.py
+ravdl/v2/load_onnx_model.py
 ravdl/v2/loss_functions.py
-ravdl/v2/optimizers.py
-ravdl/v2/utils/__init__.py
-ravdl/v2/utils/data_manipulation.py
-ravdl/v2/utils/data_operations.py
+ravdl/v2/optimizers.py
```

### Comparing `ravdl-0.8/setup.py` & `ravdl-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ravdl",
-    version="0.8",
+    version="0.9",
     license='MIT',
     author="Raven Protocol",
     author_email='kailash@ravenprotocol.com',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ravenprotocol/ravdl',
```

