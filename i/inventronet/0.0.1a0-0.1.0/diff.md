# Comparing `tmp/inventronet-0.0.1a0.tar.gz` & `tmp/inventronet-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventronet-0.0.1a0.tar", last modified: Mon Apr 24 15:08:38 2023, max compression
+gzip compressed data, was "inventronet-0.1.0.tar", last modified: Mon Apr 24 14:43:12 2023, max compression
```

## Comparing `inventronet-0.0.1a0.tar` & `inventronet-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.113605 inventronet-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 15:08:38.113605 inventronet-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.105605 inventronet-0.0.1a0/activations/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/activations/tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.105605 inventronet-0.0.1a0/inventronet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 15:08:38.000000 inventronet-0.0.1a0/inventronet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-24 15:08:38.000000 inventronet-0.0.1a0/inventronet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:08:38.000000 inventronet-0.0.1a0/inventronet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 15:08:38.000000 inventronet-0.0.1a0/inventronet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 15:08:38.000000 inventronet-0.0.1a0/inventronet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.105605 inventronet-0.0.1a0/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/layers/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/layers/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/layers/shape_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.109605 inventronet-0.0.1a0/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/losses/binary_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/losses/categorical_cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/losses/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/losses/mean_squared_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.109605 inventronet-0.0.1a0/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/metrics/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.109605 inventronet-0.0.1a0/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/models/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.109605 inventronet-0.0.1a0/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/optimizers/stochastic_gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:08:38.113605 inventronet-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:38.113605 inventronet-0.0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    24067 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-24 15:08:24.000000 inventronet-0.0.1a0/tests/test_optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.182567 inventronet-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 14:42:55.000000 inventronet-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 14:43:12.182567 inventronet-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-24 14:42:55.000000 inventronet-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.174567 inventronet-0.1.0/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-24 14:42:55.000000 inventronet-0.1.0/activations/tanh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.174567 inventronet-0.1.0/inventronet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 14:43:12.000000 inventronet-0.1.0/inventronet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-24 14:43:12.000000 inventronet-0.1.0/inventronet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:43:12.000000 inventronet-0.1.0/inventronet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 14:43:12.000000 inventronet-0.1.0/inventronet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 14:43:12.000000 inventronet-0.1.0/inventronet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.178567 inventronet-0.1.0/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 14:42:55.000000 inventronet-0.1.0/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 14:42:55.000000 inventronet-0.1.0/layers/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-24 14:42:55.000000 inventronet-0.1.0/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 14:42:55.000000 inventronet-0.1.0/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-24 14:42:55.000000 inventronet-0.1.0/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-24 14:42:55.000000 inventronet-0.1.0/layers/shape_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.178567 inventronet-0.1.0/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-24 14:42:55.000000 inventronet-0.1.0/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-24 14:42:55.000000 inventronet-0.1.0/losses/binary_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 14:42:55.000000 inventronet-0.1.0/losses/categorical_cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 14:42:55.000000 inventronet-0.1.0/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 14:42:55.000000 inventronet-0.1.0/losses/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-24 14:42:55.000000 inventronet-0.1.0/losses/mean_squared_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.178567 inventronet-0.1.0/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 14:42:55.000000 inventronet-0.1.0/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 14:42:55.000000 inventronet-0.1.0/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 14:42:55.000000 inventronet-0.1.0/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 14:42:55.000000 inventronet-0.1.0/metrics/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.178567 inventronet-0.1.0/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 14:42:55.000000 inventronet-0.1.0/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-24 14:42:55.000000 inventronet-0.1.0/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-24 14:42:55.000000 inventronet-0.1.0/models/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.178567 inventronet-0.1.0/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 14:42:55.000000 inventronet-0.1.0/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 14:42:55.000000 inventronet-0.1.0/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 14:42:55.000000 inventronet-0.1.0/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 14:42:55.000000 inventronet-0.1.0/optimizers/stochastic_gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:43:12.182567 inventronet-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-24 14:42:55.000000 inventronet-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:43:12.182567 inventronet-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24067 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-24 14:42:55.000000 inventronet-0.1.0/tests/test_optimizers.py
```

### Comparing `inventronet-0.0.1a0/LICENSE` & `inventronet-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/PKG-INFO` & `inventronet-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.1a0
+Version: 0.1.0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `inventronet-0.0.1a0/README.md` & `inventronet-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/activation.py` & `inventronet-0.1.0/activations/activation.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/leaky_relu.py` & `inventronet-0.1.0/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/linear.py` & `inventronet-0.1.0/activations/linear.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/relu.py` & `inventronet-0.1.0/activations/relu.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/sigmoid.py` & `inventronet-0.1.0/activations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/softmax.py` & `inventronet-0.1.0/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/activations/tanh.py` & `inventronet-0.1.0/activations/tanh.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/inventronet.egg-info/PKG-INFO` & `inventronet-0.1.0/inventronet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventronet
-Version: 0.0.1a0
+Version: 0.1.0
 Summary: A package for building and testing neural networks
 Home-page: https://github.com/inventrohyder/inventronet
 Author: inventrohyder
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `inventronet-0.0.1a0/inventronet.egg-info/SOURCES.txt` & `inventronet-0.1.0/inventronet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/layers/batch_normalization.py` & `inventronet-0.1.0/layers/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/layers/dense.py` & `inventronet-0.1.0/layers/dense.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/layers/dropout.py` & `inventronet-0.1.0/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/layers/layer.py` & `inventronet-0.1.0/layers/layer.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/losses/binary_cross_entropy.py` & `inventronet-0.1.0/losses/binary_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/losses/categorical_cross_entropy.py` & `inventronet-0.1.0/losses/categorical_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/losses/loss.py` & `inventronet-0.1.0/losses/loss.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/losses/mean_absolute_error.py` & `inventronet-0.1.0/losses/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/losses/mean_squared_error.py` & `inventronet-0.1.0/losses/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/models/model.py` & `inventronet-0.1.0/models/model.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/models/sequential.py` & `inventronet-0.1.0/models/sequential.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/optimizers/adam.py` & `inventronet-0.1.0/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/setup.py` & `inventronet-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 package_name = "inventronet"
-package_version = "0.0.1-alpha"
+package_version = "0.1.0"
 package_description = "A package for building and testing neural networks"
 
 # Read the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     package_long_description = f.read()
 
 package_url = "https://github.com/inventrohyder/inventronet"
@@ -30,15 +30,15 @@
 }
 
 setup(
     name=package_name,
     version=package_version,
     description=package_description,
     long_description=package_long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     url=package_url,
     author=package_author,
     license=package_license,
     packages=find_packages(),
     install_requires=package_install_requires,
     classifiers=package_classifiers,
     extras_require=package_extras_require,
```

### Comparing `inventronet-0.0.1a0/tests/test_activations.py` & `inventronet-0.1.0/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/tests/test_layers.py` & `inventronet-0.1.0/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/tests/test_loss.py` & `inventronet-0.1.0/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/tests/test_metrics.py` & `inventronet-0.1.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/tests/test_model.py` & `inventronet-0.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `inventronet-0.0.1a0/tests/test_optimizers.py` & `inventronet-0.1.0/tests/test_optimizers.py`

 * *Files identical despite different names*

