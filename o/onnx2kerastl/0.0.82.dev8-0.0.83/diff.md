# Comparing `tmp/onnx2kerastl-0.0.82.dev8.tar.gz` & `tmp/onnx2kerastl-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.82.dev8.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.83.tar", max compression
```

## Comparing `onnx2kerastl-0.0.82.dev8.tar` & `onnx2kerastl-0.0.83.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/LICENSE
--rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13188 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-04-13 13:17:22.638560 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9300 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3693 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-04-13 13:17:22.654560 onnx2kerastl-0.0.82.dev8/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5328 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15397 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     2940 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17567 2023-04-13 13:17:22.642560 onnx2kerastl-0.0.82.dev8/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1035 2023-04-13 13:23:53.671617 onnx2kerastl-0.0.82.dev8/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.82.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/LICENSE
+-rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.83/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13188 2023-04-24 08:19:57.529136 onnx2kerastl-0.0.83/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.83/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      499 2023-04-24 08:20:01.601311 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-24 08:32:43.815742 onnx2kerastl-0.0.83/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-24 08:32:43.811742 onnx2kerastl-0.0.83/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3309 2023-04-24 08:20:01.601311 onnx2kerastl-0.0.83/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.83/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5328 2023-04-24 06:18:47.644616 onnx2kerastl-0.0.83/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-24 08:32:43.803742 onnx2kerastl-0.0.83/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-24 08:32:43.807742 onnx2kerastl-0.0.83/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    16675 2023-04-24 08:32:43.807742 onnx2kerastl-0.0.83/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5354 2023-04-24 08:32:43.803742 onnx2kerastl-0.0.83/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.83/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-04-24 08:32:43.823742 onnx2kerastl-0.0.83/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.83/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.82.dev8/LICENSE` & `onnx2kerastl-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.83/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.83/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/elementwise_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     logger = logging.getLogger('onnx2keras.add')
 
     if len(node.input) != 2:
         raise AttributeError('Number of inputs is not equal 2 for element-wise layer')
 
     input_0 = layers[node.input[0]]
     input_1 = layers[node.input[1]]
-    input_0_is_non_keras = is_numpy(input_0) or isinstance(input_1, EagerTensor)
+    input_0_is_non_keras = is_numpy(input_0) or isinstance(input_0, EagerTensor)
     input_1_is_non_keras = is_numpy(input_1) or isinstance(input_1, EagerTensor)
     try:
         if not input_0_is_non_keras and not input_1_is_non_keras:
             to_add = input_1
             if input_0.shape != input_1.shape and input_0.shape[:-1] == input_1.shape:
                 to_add = tf.repeat(tf.expand_dims(input_1, axis=-1), input_0.shape[-1], axis=-1)
 
@@ -138,16 +138,16 @@
     logger = logging.getLogger('onnx2keras.sub')
 
     if len(node.input) != 2:
         raise AttributeError('Number of inputs is not equal 2 for element-wise layer')
 
     input_0 = layers[node.input[0]]
     input_1 = layers[node.input[1]]
-    input_0_is_np = is_numpy(input_0)
-    input_1_is_np = is_numpy(input_1)
+    input_0_is_np = is_numpy(input_0) or isinstance(input_0, EagerTensor)
+    input_1_is_np = is_numpy(input_1) or isinstance(input_1, EagerTensor)
 
     try:
         if not input_0_is_np and not input_1_is_np:
             sub = keras.layers.Subtract(name=keras_name)
             layers[node_name] = sub([input_0, input_1])
         else:
             raise ValueError('Operands are different.')
```

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from .operation_layers import convert_clip, convert_exp, convert_neg, convert_reduce_sum, convert_reduce_mean, \
     convert_log, convert_pow, convert_sqrt, convert_split, convert_cast, convert_floor, convert_identity, \
     convert_argmax, convert_reduce_l2, convert_reduce_max, convert_reciprocal, convert_abs
 from .elementwise_layers import convert_elementwise_div, convert_elementwise_add, convert_elementwise_mul, \
     convert_elementwise_sub, convert_max, convert_min, convert_mean, convert_equal, convert_where, convert_scatter_nd
 from .linear_layers import convert_gemm
 from .reshape_layers import convert_transpose, convert_shape, convert_gather, convert_unsqueeze, \
-    convert_concat, convert_reshape, convert_flatten, convert_slice, convert_squeeze, convert_expand, convert_resize
+    convert_concat, convert_reshape, convert_flatten, convert_slice, convert_squeeze, convert_expand, convert_resize,\
+    convert_tile
 from .constant_layers import convert_constant, convert_constant_of_shape
 from .normalization_layers import convert_batchnorm, convert_instancenorm, convert_dropout, convert_lrn
 from .pooling_layers import convert_avgpool, convert_maxpool, convert_global_avg_pool
 from .padding_layers import convert_padding
 from .upsampling_layers import convert_upsample
 from .caffe2_layers import convert_alias_with_name, convert_resize_nearest
+from .sampling_layers import convert_gridsample, convert_range
 
 AVAILABLE_CONVERTERS = {
     'Abs': convert_abs,
     'AliasWithName': convert_alias_with_name,
     'Conv': convert_conv,
     'ConvTranspose': convert_convtranspose,
     'Relu': convert_relu,
@@ -80,11 +82,14 @@
     'Flatten': convert_flatten,
     'Upsample': convert_upsample,
     'Erf': convert_erf,
     'Reciprocal': convert_reciprocal,
     'ConstantOfShape': convert_constant_of_shape,
     'Equal': convert_equal,
     'Where': convert_where,
-    'LSTM': convert_lstm
+    'LSTM': convert_lstm,
+    'Tile': convert_tile,
+    'GridSample': convert_gridsample,
+    'Range': convert_range
 
 
 }
```

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/ltsm_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import tensorflow as tf
 import numpy as np
-from onnx2kerastl.customonnxlayer.onnxlstm import OnnxLSTM
 
 from .exceptions import UnsupportedLayer
 from .utils import ensure_tf_type, ensure_numpy_type
 
 
 def convert_lstm(node, params, layers, lambda_func, node_name, keras_name):
     """
@@ -24,27 +23,28 @@
         raise UnsupportedLayer('LSTM with non default sequence_lens')
     if 'direction' in params:
         direction = params['direction']
         if isinstance(direction, bytes):
             direction = direction.decode("utf-8")
         if direction != 'forward':
             raise UnsupportedLayer(f"LSTM with {direction} direction")
-    should_return_state = len(node.output) == 3
+
     input_tensor = tf.transpose(ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name[0]), perm=[1, 0, 2])
     weights_w = ensure_numpy_type(layers[node.input[1]])[0]
     weights_r = ensure_numpy_type(layers[node.input[2]])[0]
     weights_b = ensure_numpy_type(layers[node.input[3]])[0]
 
     initial_h_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[5]]), axis=1), input_tensor.dtype)
     initial_c_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[6]]), axis=1), input_tensor.dtype)
 
     tf.keras.backend.set_image_data_format("channels_last")
     hidden_size = params['hidden_size']
-    lstm_layer = OnnxLSTM(hidden_size, return_sequences=True, return_lstm_state=should_return_state)
-    res = lstm_layer(input_tensor, initial_h_state, initial_c_state)
+    lstm_tensor = tf.keras.layers.LSTM(hidden_size, return_sequences=True) \
+        (input_tensor, initial_state=[initial_h_state, initial_c_state])
+
     # prepare the keras lstm weights from the onnx inputs:
     w1 = np.concatenate([weights_w[0:hidden_size, :], weights_w[2 * hidden_size:3 * hidden_size, :],
                          weights_w[3 * hidden_size:4 * hidden_size, :],
                          weights_w[hidden_size:2 * hidden_size, :]]).transpose()
     w2 = np.concatenate([weights_r[0:hidden_size, :], weights_r[2 * hidden_size:3 * hidden_size, :],
                          weights_r[3 * hidden_size:4 * hidden_size, :],
                          weights_r[hidden_size:2 * hidden_size, :]]).transpose()
@@ -53,22 +53,14 @@
     bias1 = np.concatenate([weights_b_part1[0:hidden_size], weights_b_part1[2 * hidden_size:3 * hidden_size],
                             weights_b_part1[3 * hidden_size:4 * hidden_size],
                             weights_b_part1[hidden_size:2 * hidden_size]]).transpose()
     bias2 = np.concatenate([weights_b_part2[0:hidden_size], weights_b_part2[2 * hidden_size:3 * hidden_size],
                             weights_b_part2[3 * hidden_size:4 * hidden_size],
                             weights_b_part2[hidden_size:2 * hidden_size]]).transpose()
     bias = bias1 + bias2
-    res.node.layer.set_weights([w1, w2, bias])
+    lstm_tensor.node.layer.set_weights([w1, w2, bias])
     tf.keras.backend.set_image_data_format("channels_first")
-    if should_return_state:
-        c_out = res[:, -hidden_size:]
-        h_out = res[:, -2*hidden_size:-hidden_size]
-        flat_lstm_tensor = res[:, :-2*hidden_size]
-        lstm_tensor = tf.keras.layers.Reshape((-1, hidden_size))(flat_lstm_tensor)
-        layers[node.output[1]] = c_out
-        layers[node.output[2]] = h_out
-    else:
-        lstm_tensor = res
+
     lstm_tensor_in_onnx_order = tf.transpose(lstm_tensor, perm=[1, 0, 2])
     lstm_tensor_in_onnx_order = tf.expand_dims(lstm_tensor_in_onnx_order, axis=1)
-    layers[node_name] = lstm_tensor_in_onnx_order
 
+    layers[node_name] = lstm_tensor_in_onnx_order
```

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/operation_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,20 +135,27 @@
     :param keras_name: resulting layer name
     :return: None
     """
     if len(node.input) != 1:
         assert AttributeError('More than 1 input for reduce sum layer.')
 
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
+    if 'axes' not in params:
+        axis = layers[node.input[1]]
+    else:
+        axis = params['axes']
+
+    keep_dims = True
+    if 'keepdims' in params:
+        if params['keepdims'] == 0:
+            keep_dims = False
 
-    axis = params['axes']
-
-    def target_layer(x, axis=axis):
+    def target_layer(x, axis=axis, keep_dims=keep_dims):
         import keras.backend as K
-        return K.sum(x, keepdims=True, axis=axis)
+        return K.sum(x, keepdims=keep_dims, axis=axis)
 
     lambda_layer = keras.layers.Lambda(target_layer, name=keras_name)
     layers[node_name] = lambda_layer(input_0)
     layers[node_name].set_shape(layers[node_name].shape)
     lambda_func[keras_name] = target_layer
```

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/padding_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,18 @@
     :param lambda_func: function for keras Lambda layer
     :param node_name: internal converter name
     :param keras_name: resulting layer name
     :return: None
     """
     # It's binary by-default
     logger = logging.getLogger("onnx2keras.padding")
-    params['mode'] = params['mode'].decode('ascii')
+    if 'mode' in params:
+        params['mode'] = params['mode'].decode('ascii')
+    else:
+        params['mode'] = 'constant'
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
 
     if 'pads' in params:
         pads = params['pads']
     else:
         pads = layers[node.input[1]]
```

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/reshape_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,18 @@
         layers[node_name] = gathered
     else:
         input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
         if not isinstance(layers[node.input[1]], np.ndarray) and \
                 K.is_keras_tensor(layers[node.input[1]]):
             indices = layers[node.input[1]]
         else:
-            indices = layers[node.input[1]].tolist()
+            indices = layers[node.input[1]]
+            if not is_numpy(layers[node.input[1]]):
+                indices = indices.numpy()
+            indices = indices.tolist()
         if "is_embedding" in params:
             if len(input_0.shape) == 2:
                 emb = tf.keras.layers.Embedding(input_0.shape[0], input_0.shape[1], weights=[layers[node.input[0]]],
                                                 name=keras_name)
                 if isinstance(indices, list):
                     layers[node_name] = emb(np.array(indices))
                 else:
@@ -198,39 +201,28 @@
                     layers[node_name] = input_0
 
                 reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
                 layers[node_name] = reshape(layers[node_name])
 
             else:
                 input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
-                input_0_shape = input_0.shape
-                first_mismatch = np.argmin(np.array(input_0_shape[:len(input_1)]) == input_1)
-                if (input_1 == None).any() and (np.array(input_0_shape) == None).any() and len(input_1) < len(input_0_shape)\
-                        and input_1[first_mismatch] == -1: #reshape end
-                    end_match_arr = np.array(input_0_shape[-len(input_1):]) == input_1
-                    end_idx_match = np.argmax((np.array(input_0_shape[-len(input_1):]) == input_1))
-                    end_idx_match = end_idx_match + len(input_0_shape) - len(input_1) if end_idx_match > first_mismatch \
-                                                     and end_match_arr[end_idx_match] else len(input_0_shape) + 1
-                    tf_shape = tf.shape(input_0)
-                    layers[node_name] = tf.reshape(input_0, [*tf_shape[:first_mismatch], -1, *tf_shape[end_idx_match:]])
+                logger.debug('The first argument is Keras/tf layer. Apply keras.Reshape.')
+                logger.debug('Target shape :')
+                logger.debug(np.int32(input_1[1:]))
+
+                if len(np.int32(input_1[1:])) == 1 and np.int32(input_1[1:])[0] == -1:
+                    logger.debug('The first argument is Keras/tf layer. Apply keras.Flatten.')
+                    flatten = keras.layers.Flatten(name=keras_name)
+                    layers[node_name] = flatten(input_0)
                 else:
-                    logger.debug('The first argument is Keras/tf layer. Apply keras.Reshape.')
-                    logger.debug('Target shape :')
-                    logger.debug(np.int32(input_1[1:]))
-
-                    if len(np.int32(input_1[1:])) == 1 and np.int32(input_1[1:])[0] == -1:
-                        logger.debug('The first argument is Keras/tf layer. Apply keras.Flatten.')
-                        flatten = keras.layers.Flatten(name=keras_name)
-                        layers[node_name] = flatten(input_0)
+                    if input_0.shape[0] != input_1[0]:  # keras reshape don't work
+                        layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
                     else:
-                        if input_0.shape[0] != input_1[0]:  # keras reshape don't work
-                            layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
-                        else:
-                            reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
-                            layers[node_name] = reshape(input_0)
+                        reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
+                        layers[node_name] = reshape(input_0)
     else:
         raise AttributeError('Can\'t reshape dynamic size.')
 
 
 def convert_unsqueeze(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert unsqueeze.
@@ -327,23 +319,23 @@
             axis_index = axes_positives.index(axis)
             start = starts[axis_index]
             end = ends[axis_index] if ends[axis_index] < 2147483647 else None
             step = steps[axis_index]
             slice_spec_param.append({'start': start, 'step': step, 'stop': end})
         else:
             slice_spec_param.append({'start': None, 'step': None, 'stop': None})
-    if is_numpy(layers[node.input[0]]) and not np.array([not x is None for x in layers[node.input[0]]]).all(): # shape with None
-        sliced = layers[node.input[0]][start:end:step]
+
+    input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
+    slicing_layer = SlicingOpLambda(tf.__operators__.getitem)
+    sliced = slicing_layer(input_0, slice_spec=slice_spec_param)
+
+    if is_numpy(layers[node.input[0]]):
+        layers[node_name] = sliced.numpy()
     else:
-        input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
-        slicing_layer = SlicingOpLambda(tf.__operators__.getitem)
-        sliced = slicing_layer(input_0, slice_spec=slice_spec_param)
-        if is_numpy(layers[node.input[0]]):
-            sliced = sliced.numpy()
-    layers[node_name] = sliced
+        layers[node_name] = sliced
 
 
 def convert_squeeze(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert Squeeze layer
     :param node: current operation node
     :param params: operation attributes
@@ -417,9 +409,12 @@
     """
     if len(node.input) != 2:
         assert AttributeError('More than 2 input for expand layer.')
 
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
     input_1 = ensure_numpy_type(layers[node.input[1]]).astype(np.int32)
 
-    layers[node_name] = input_0 * tf.ones(input_1)
+    layers[node_name] = input_0 * tf.ones(input_1, dtype=input_0.dtype)
+
 
+def convert_tile(node, params, layers, lambda_func, node_name, keras_name):
+    layers[node_name] = tf.tile(layers[node.input[0]], layers[node.input[1]])
```

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.83/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.83/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev8/pyproject.toml` & `onnx2kerastl-0.0.83/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.82.dev8"
+version = "0.0.83"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.82.dev8/PKG-INFO` & `onnx2kerastl-0.0.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.82.dev8
+Version: 0.0.83
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

