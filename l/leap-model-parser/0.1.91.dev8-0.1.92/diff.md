# Comparing `tmp/leap_model_parser-0.1.91.dev8.tar.gz` & `tmp/leap_model_parser-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.91.dev8.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.92.tar", max compression
```

## Comparing `leap_model_parser-0.1.91.dev8.tar` & `leap_model_parser-0.1.92.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/LICENSE
--rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/README.md
--rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43326 2023-04-13 14:41:50.222916 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   416303 2023-04-13 14:41:50.222916 leap_model_parser-0.1.91.dev8/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2804 2023-04-13 14:41:50.214917 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     6768 2023-04-13 14:41:50.226917 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1062 2023-04-13 14:41:50.210917 leap_model_parser-0.1.91.dev8/pyproject.toml
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 leap_model_parser-0.1.91.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/LICENSE
+-rw-r--r--   0        0        0       68 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/README.md
+-rw-r--r--   0        0        0      132 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43172 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   414214 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.936891 leap_model_parser-0.1.92/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2786 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-07-18 07:29:48.940891 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     5799 2023-04-24 08:36:26.808246 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-04-04 06:58:15.124228 leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1052 2023-04-24 08:38:14.580216 leap_model_parser-0.1.92/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.92/PKG-INFO
```

### Comparing `leap_model_parser-0.1.91.dev8/LICENSE` & `leap_model_parser-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.92/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.92/leap_model_parser/contract/nodedata.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,14 @@
     Ftrl = "Ftrl"
     Nadam = "Nadam"
     RMSprop = "RMSprop"
     SGD = "SGD"
     OnnxAbs = "OnnxAbs"
     OnnxErf = "OnnxErf"
     OnnxHardSigmoid = "OnnxHardSigmoid"
-    OnnxLSTM = "OnnxLSTM"
     OnnxReduceMean = "OnnxReduceMean"
     OnnxSqrt = "OnnxSqrt"
     Dataset = "Dataset"
     Input = "Input"
     RepresentationBlock = "RepresentationBlock"
     GroundTruth = "GroundTruth"
     CustomLayer = "CustomLayer"
@@ -1805,22 +1804,14 @@
 class OnnxHardSigmoid:
     alpha: float
     beta: float
     type: NodeType
 
 
 @dataclass
-class OnnxLSTM:
-    units: int
-    return_sequences: bool
-    return_lstm_state: bool
-    type: NodeType
-
-
-@dataclass
 class OnnxReduceMean:
     axes: List[int]
     keepdims: bool
     type: NodeType
 
 
 @dataclass
@@ -1927,10 +1918,10 @@
                  SeparableConv1D, SeparableConv2D, SimpleRNN, SimpleRNNCell, Softmax, SpatialDropout1D, 
                  SpatialDropout2D, SpatialDropout3D, StringLookup, Subtract, SyncBatchNormalization, TextVectorization, 
                  ThresholdedReLU, TimeDistributed, UnitNormalization, UpSampling1D, UpSampling2D, UpSampling3D, 
                  ZeroPadding1D, ZeroPadding2D, ZeroPadding3D, BinaryCrossentropy, BinaryFocalCrossentropy, 
                  CategoricalCrossentropy, CategoricalHinge, CosineSimilarity, Hinge, Huber, KLDivergence, LogCosh, 
                  MeanAbsoluteError, MeanAbsolutePercentageError, MeanSquaredError, MeanSquaredLogarithmicError, Poisson, 
                  SquaredHinge, Adadelta, Adagrad, Adam, Adamax, Ftrl, Nadam, RMSprop, SGD, OnnxAbs, OnnxErf, 
-                 OnnxHardSigmoid, OnnxLSTM, OnnxReduceMean, OnnxSqrt, Dataset, Input, RepresentationBlock, GroundTruth, 
+                 OnnxHardSigmoid, OnnxReduceMean, OnnxSqrt, Dataset, Input, RepresentationBlock, GroundTruth, 
                  CustomLayer, CustomLoss, Visualizer, Metric, Lambda, TFOpLambda, SlicingOpLambda, Repeat, Variable, 
                  Gather, FixedDropout]
```

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.92/leap_model_parser/contract/ui_components.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9934640522875817%*

 * *Differences: {'delete': '[135]'}*

```diff
@@ -14570,91 +14570,14 @@
                     "approval_connection": [
                         "Input",
                         "Dataset",
                         "Layer",
                         "CustomLayer"
                     ],
                     "name": "input"
-                },
-                {
-                    "approval_connection": [
-                        "Input",
-                        "Dataset",
-                        "Layer",
-                        "CustomLayer"
-                    ],
-                    "name": "initial_h_state"
-                },
-                {
-                    "approval_connection": [
-                        "Input",
-                        "Dataset",
-                        "Layer",
-                        "CustomLayer"
-                    ],
-                    "name": "initial_c_state"
-                }
-            ]
-        },
-        "menu_sections": [
-            "Layer",
-            "Onnx"
-        ],
-        "name": "OnnxLSTM",
-        "options": null,
-        "outputs_data": {
-            "outputs": [
-                {
-                    "name": "feature_map"
-                }
-            ]
-        },
-        "parents": [
-            "onnx2kerastl",
-            "customonnxlayer",
-            "onnxlstm"
-        ],
-        "properties": [
-            {
-                "default_val": null,
-                "isdefault": false,
-                "name": "units",
-                "type": "int"
-            },
-            {
-                "default_val": null,
-                "isdefault": false,
-                "name": "return_sequences",
-                "type": "bool"
-            },
-            {
-                "default_val": null,
-                "isdefault": false,
-                "name": "return_lstm_state",
-                "type": "bool"
-            }
-        ],
-        "receptive_fields_func": "IdentityReceptiveFieldsFunc",
-        "shape_calc": [
-            "IdentityFunc"
-        ],
-        "type": "Layer"
-    },
-    {
-        "inputs_data": {
-            "add_input_by_drag": false,
-            "inputs": [
-                {
-                    "approval_connection": [
-                        "Input",
-                        "Dataset",
-                        "Layer",
-                        "CustomLayer"
-                    ],
-                    "name": "input"
                 }
             ]
         },
         "menu_sections": [
             "Layer",
             "Onnx"
         ],
```

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.92/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.92/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.92/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.92/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 classes.append(cls_dict)
 
         return classes
 
     @staticmethod
     def get_type(func, pval):
         dtype_map = {'int': ['int', 'Integer', 'number'], 'float': ['float'], 'str': ['string', 'str'],
-                     'name': ['name'], 'tuple': ["tuple", "Tuple"], 'bool': ['bool']}
+                     'name': ['name'], 'tuple': ["tuple", "Tuple"]}
         if pval.default != inspect._empty:
             return str(type(pval.default)).split('\'')[1]
         # TODO: comment out due to missing CallableMeta type in python 3.8, if an error occurs from this section consider
         # finding the right way to write this if in python 3.8
         # if isinstance(pval.annotation, CallableMeta):
         #     return Callable
         if pval.annotation is str:
```

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
-from typing import List, Optional, Callable, Any
+from typing import List, Optional
 
 import yaml
 from leap_model_parser.utils.layerpedia.layerpedia import Layerpedia
 from leap_model_parser.utils.tlinspection.leapinspection import LeapInspect
-from copy import deepcopy
 
 
 class TensorFlowInspection(LeapInspect):
 
     def __init__(self):
         file_path = os.path.dirname(os.path.abspath(__file__))
         with open(f'{file_path}/ui_components_config.yaml') as f:
@@ -52,32 +51,14 @@
                     arg['default_val'] = override_def
             _args.append(arg)
         return _args
 
     def filter_node(self, node):
         return node['name'] in self.ignores['clsignore']
 
-    def get_filled_group_values(self, node_type: str, class_pointer: Callable[..., Any]) -> dict:
-        if node_type == 'customonnxlayer':
-            var_names = class_pointer.__dict__['call'].__code__.co_varnames
-            arg_names = var_names[1:class_pointer.__dict__['call'].__code__.co_argcount]  # remove self
-            if len(arg_names) == 1:
-                return self.group_type[node_type]
-            else:
-                config_dict = deepcopy(self.group_type[node_type])
-                inputs_list = config_dict['inputs_data']['inputs']
-                for arg in arg_names[1:]:
-                    inputs_list.append(
-                        {'name': f'{arg}',
-                         'approval_connection': ['Input', 'Dataset', 'Layer', 'CustomLayer']}
-                    )
-                return config_dict
-        else:
-            return self.group_type[node_type]
-
     def inspect_lib(self, lib):
         # TODO: extract only classes and not aliases
         classes = LeapInspect.get_classes(lib, self.ignores['lib_ignore'])
         nodes = []
         for node_cls in classes:
             if self.filter_node(node_cls):
                 continue
@@ -93,15 +74,15 @@
             enable_bigger_input_rank = self.query_layerpedia_enable_bigger_input_rank(
                 node_cls['name'])
             if enable_bigger_input_rank:
                 node['enable_bigger_input_rank'] = enable_bigger_input_rank
             template_node = {}
             for d in [*node_cls['parents'], node['name']]:
                 if d in self.group_type:
-                    template_node = {**template_node, **self.get_filled_group_values(d, node_cls['class'])}
+                    template_node = {**template_node, **self.group_type[d]}
             node = {**template_node, **node}
             if 'hash' in node and not self.query_layerpedia_is_trainable(node_cls['name']):
                 node.pop('hash')
             nodes.append(node)
         return nodes
 
     def inspect(self, dist: str) -> List[dict]:
```

### Comparing `leap_model_parser-0.1.91.dev8/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.92/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.91.dev8/pyproject.toml` & `leap_model_parser-0.1.92/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.91.dev8"
+version = "0.1.92"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.82.dev8"
+onnx2kerastl = "0.0.83"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.91.dev8/PKG-INFO` & `leap_model_parser-0.1.92/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.91.dev8
+Version: 0.1.92
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.82.dev8)
+Requires-Dist: onnx2kerastl (==0.0.83)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

