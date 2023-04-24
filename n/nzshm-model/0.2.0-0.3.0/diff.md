# Comparing `tmp/nzshm_model-0.2.0.tar.gz` & `tmp/nzshm_model-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzshm_model-0.2.0.tar", max compression
+gzip compressed data, was "nzshm_model-0.3.0.tar", max compression
```

## Comparing `nzshm_model-0.2.0.tar` & `nzshm_model-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      258 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/README.md
--rw-r--r--   0        0        0      310 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/__init__.py
--rw-r--r--   0        0        0     1607 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/nshm_1_0_0.py
--rw-r--r--   0        0        0      518 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/nshm_1_0_4.py
--rw-r--r--   0        0        0    72558 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v8.json
--rw-r--r--   0        0        0    17910 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v8_gmm_v2_final.py
--rw-r--r--   0        0        0    87571 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v9p0p0.json
--rw-r--r--   0        0        0    18070 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v9p0p0.py
--rw-r--r--   0        0        0        0 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/__init__.py
--rw-r--r--   0        0        0     6423 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/logic_tree.py
--rw-r--r--   0        0        0     7836 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/slt_config.py
--rw-r--r--   0        0        0     5920 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/nzshm_model/source_logic_tree/toshi_api.py
--rw-r--r--   0        0        0     2013 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3074 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/scripts/slt.py
--rw-r--r--   0        0        0    12885 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/tests/fixtures/large_SLT_example_A.py
--rw-r--r--   0        0        0     6273 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/tests/test_logic_tree.py
--rw-r--r--   0        0        0      854 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/tests/test_module_import.py
--rw-r--r--   0        0        0     5768 2023-04-04 00:05:10.713327 nzshm_model-0.2.0/tests/test_slt_config.py
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 nzshm_model-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      258 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/README.md
+-rw-r--r--   0        0        0      317 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/__init__.py
+-rw-r--r--   0        0        0     1618 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/nshm_v1_0_0.py
+-rw-r--r--   0        0        0      520 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/nshm_v1_0_4.py
+-rw-r--r--   0        0        0    17910 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/SLT_v8_gmm_v2_final.py
+-rw-r--r--   0        0        0    18070 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/SLT_v9p0p0.py
+-rw-r--r--   0        0        0        0 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/__init__.py
+-rw-r--r--   0        0        0     6465 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/logic_tree.py
+-rw-r--r--   0        0        0    90461 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/nshm_v1.0.0.json
+-rw-r--r--   0        0        0    90470 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/nshm_v1.0.4.json
+-rw-r--r--   0        0        0     8177 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/slt_config.py
+-rw-r--r--   0        0        0     7161 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/nzshm_model/source_logic_tree/toshi_api.py
+-rw-r--r--   0        0        0     2013 2023-04-24 03:09:36.736834 nzshm_model-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3074 2023-04-24 03:09:36.740834 nzshm_model-0.3.0/scripts/slt.py
+-rw-r--r--   0        0        0    12885 2023-04-24 03:09:36.740834 nzshm_model-0.3.0/tests/fixtures/large_SLT_example_A.py
+-rw-r--r--   0        0        0     6276 2023-04-24 03:09:36.740834 nzshm_model-0.3.0/tests/test_logic_tree.py
+-rw-r--r--   0        0        0      859 2023-04-24 03:09:36.740834 nzshm_model-0.3.0/tests/test_module_import.py
+-rw-r--r--   0        0        0     5769 2023-04-24 03:09:36.740834 nzshm_model-0.3.0/tests/test_slt_config.py
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 nzshm_model-0.3.0/PKG-INFO
```

### Comparing `nzshm_model-0.2.0/nzshm_model/nshm_1_0_0.py` & `nzshm_model-0.3.0/nzshm_model/nshm_v1_0_0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! v1_0_0.py
+#! nshm_v1_0_0.py
 
 import itertools
 import json
 from pathlib import Path
 
 import dacite  # for dataclass reconstitution
 
@@ -11,18 +11,18 @@
     Branch,
     BranchAttributeSpec,
     BranchAttributeValue,
     FaultSystemLogicTree,
     SourceLogicTree,
 )
 
-version = 'NSHM_1.0.0'
+version = 'NSHM_v1.0.0'
 title = "Initial version"
 
-json_slt = Path(__file__).parent / "source_logic_tree" / "SLT_v8.json"
+json_slt = Path(__file__).parent / "source_logic_tree" / "nshm_v1.0.0.json"
 
 
 def source_logic_tree():
     return dacite.from_dict(data_class=SourceLogicTree, data=json.load(open(json_slt)))
 
 
 def build_crustal_branches():
```

### Comparing `nzshm_model-0.2.0/nzshm_model/nshm_1_0_4.py` & `nzshm_model-0.3.0/nzshm_model/nshm_v1_0_4.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 import dacite  # for dataclass reconstitution
 
 import nzshm_model.source_logic_tree.SLT_v9p0p0 as slt_config  # NOQA F401
 from nzshm_model.source_logic_tree.logic_tree import SourceLogicTree
 
-version = 'NSHM_1.0.4'
+version = 'NSHM_v1.0.4'
 title = "NSHM version 1.0.4, corrected fault geometry"
 
-json_slt = Path(__file__).parent / "source_logic_tree" / "SLT_v9p0p0.json"
+json_slt = Path(__file__).parent / "source_logic_tree" / "nshm_v1.0.4.json"
 
 
 def source_logic_tree():
     return dacite.from_dict(data_class=SourceLogicTree, data=json.load(open(json_slt)))
```

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v8.json` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/nshm_v1.0.4.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6201636904761905%*

 * *Differences: {"'correlations'": "[OrderedDict([('primary_short_name', 'HIK'), ('secondary_short_name', 'PUY'), "*

 * *                   "('primary_values', [OrderedDict([('name', 'dm'), ('long_name', 'deformation "*

 * *                   "model'), ('value', 'TL')]), OrderedDict([('name', 'bN'), ('long_name', 'bN "*

 * *                   "pair'), ('value', [0.95, 16.5])]), OrderedDict([('name', 'C'), ('long_name', "*

 * *                   "'area-magnitude scaling'), ('value', 4.0)]), OrderedDict([('name', 's'), "*

 * *                   "('l […]*

```diff
@@ -1,17 +1,505 @@
 {
-    "correlations": [],
+    "correlations": [
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.95,
+                        16.5
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 0.42
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 0.28
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.95,
+                        16.5
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.0
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.0
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.95,
+                        16.5
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.58
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.72
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        1.097,
+                        21.5
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 0.42
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 0.28
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        1.097,
+                        21.5
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.0
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.0
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        1.097,
+                        21.5
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.58
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.72
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        1.241,
+                        27.9
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 0.42
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 0.28
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        1.241,
+                        27.9
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.0
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.0
+                }
+            ]
+        },
+        {
+            "primary_short_name": "HIK",
+            "primary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "TL"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        1.241,
+                        27.9
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.58
+                }
+            ],
+            "secondary_short_name": "PUY",
+            "secondary_values": [
+                {
+                    "long_name": "deformation model",
+                    "name": "dm",
+                    "value": "0.7"
+                },
+                {
+                    "long_name": "bN pair",
+                    "name": "bN",
+                    "value": [
+                        0.902,
+                        4.6
+                    ]
+                },
+                {
+                    "long_name": "area-magnitude scaling",
+                    "name": "C",
+                    "value": 4.0
+                },
+                {
+                    "long_name": "moment rate scaling",
+                    "name": "s",
+                    "value": 1.72
+                }
+            ]
+        }
+    ],
     "fault_system_lts": [
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NTM=",
-                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQ2",
+                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTI5MTM3OA==",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcxNw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2NTc=",
+                    "rupture_set_id": "RmlsZToxMjkwOTg0",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "0.7"
                         },
                         {
@@ -33,17 +521,18 @@
                             "value": 0.28
                         }
                     ],
                     "weight": 0.21
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NTQ=",
-                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQz",
+                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTI5MTM4Mg==",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcyMw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2NjE=",
+                    "rupture_set_id": "RmlsZToxMjkwOTg0",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "0.7"
                         },
                         {
@@ -65,17 +554,18 @@
                             "value": 1.0
                         }
                     ],
                     "weight": 0.52
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NTU=",
-                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQ1",
+                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTI5MTM4Ng==",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcyOQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2NjY=",
+                    "rupture_set_id": "RmlsZToxMjkwOTg0",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "0.7"
                         },
                         {
@@ -105,15 +595,16 @@
         },
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MjAw",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQyOA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MTE=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -137,15 +628,16 @@
                     ],
                     "weight": 0.147216637218474
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzQ=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MjAy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxNw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MDU=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -169,15 +661,16 @@
                     ],
                     "weight": 0.281154911079988
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MjA0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQyOQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MDM=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -201,15 +694,16 @@
                     ],
                     "weight": 0.148371277510384
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mzg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTk0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQyNA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTk=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -233,15 +727,16 @@
                     ],
                     "weight": 0.0887399956599006
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTk2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxMw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MDg=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -265,15 +760,16 @@
                     ],
                     "weight": 0.169475991711261
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTk4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxNg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MTM=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -297,15 +793,16 @@
                     ],
                     "weight": 0.0894359956258606
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDQ=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTY0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxNA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTg=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -329,15 +826,16 @@
                     ],
                     "weight": 0.0192986223768806
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTY2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQwNg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTA=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -361,15 +859,16 @@
                     ],
                     "weight": 0.0368565846962387
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTY4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQwOQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTE=",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -399,15 +898,16 @@
         },
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzIy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5OA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MDE=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -436,15 +936,16 @@
                     ],
                     "weight": 0.0168335471189857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzE3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxMQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODY=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -473,15 +974,16 @@
                     ],
                     "weight": 0.0408928149352719
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzQx",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkwNA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MDI=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -510,15 +1012,16 @@
                     ],
                     "weight": 0.0216771620919014
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzYx",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxNw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODI=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -547,15 +1050,16 @@
                     ],
                     "weight": 0.0282427120823285
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzUz",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkwNg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODM=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -584,15 +1088,16 @@
                     ],
                     "weight": 0.0686084751056566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzU3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkwOA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTA=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -621,15 +1126,16 @@
                     ],
                     "weight": 0.0363691528229985
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzM0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxMw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTE=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -658,15 +1164,16 @@
                     ],
                     "weight": 0.00792374079868575
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzI4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxMg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTY=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -695,15 +1202,16 @@
                     ],
                     "weight": 0.0192487099590715
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzMw",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkyNA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTQ=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -732,15 +1240,16 @@
                     ],
                     "weight": 0.0102036850851
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzA4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4Ng==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NzM=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -769,15 +1278,16 @@
                     ],
                     "weight": 0.0236560148670262
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzA3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5Nw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODE=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -806,15 +1316,16 @@
                     ],
                     "weight": 0.0574662625307477
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzA1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg3NA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0Njg=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -843,15 +1354,16 @@
                     ],
                     "weight": 0.0304626983900857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzAy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5Mw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NjQ=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -880,15 +1392,16 @@
                     ],
                     "weight": 0.0271169544446554
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjk4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4OQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NzY=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -917,15 +1430,16 @@
                     ],
                     "weight": 0.0658737336745166
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjk2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg3MQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0Njc=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -954,15 +1468,16 @@
                     ],
                     "weight": 0.0349194743556176
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjcy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4MQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NjA=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -991,15 +1506,16 @@
                     ],
                     "weight": 0.00222703068831837
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjc2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5Mg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NzU=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1028,15 +1544,16 @@
                     ],
                     "weight": 0.00541000379473566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjc1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4Mg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NjM=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1065,15 +1582,16 @@
                     ],
                     "weight": 0.00286782725429677
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODI2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk2NQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1Mzk=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1102,15 +1620,16 @@
                     ],
                     "weight": 0.0168335471189857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODQ2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk2Mw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1Mzc=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1139,15 +1658,16 @@
                     ],
                     "weight": 0.0408928149352719
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODI0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1Ng==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTM=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1176,15 +1696,16 @@
                     ],
                     "weight": 0.0216771620919014
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODY1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1Mw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NDQ=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1213,15 +1734,16 @@
                     ],
                     "weight": 0.0282427120823285
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODYz",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk2Nw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTk=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1250,15 +1772,16 @@
                     ],
                     "weight": 0.0686084751056566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODY5",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1NA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTE=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1287,15 +1810,16 @@
                     ],
                     "weight": 0.0363691528229985
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODQ3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk3Mw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTg=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1324,15 +1848,16 @@
                     ],
                     "weight": 0.00792374079868575
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODE4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1NQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NDE=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1361,15 +1886,16 @@
                     ],
                     "weight": 0.0192487099590715
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODM3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk3NA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NjI=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1398,15 +1924,16 @@
                     ],
                     "weight": 0.0102036850851
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODE1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzNg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjI=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1435,15 +1962,16 @@
                     ],
                     "weight": 0.0236560148670263
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODEx",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkyNw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjM=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1472,15 +2000,16 @@
                     ],
                     "weight": 0.0574662625307477
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODE2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzMg==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjA=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1509,15 +2038,16 @@
                     ],
                     "weight": 0.0304626983900857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODA3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1MQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MTY=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1546,15 +2076,16 @@
                     ],
                     "weight": 0.0271169544446554
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzk2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk0NA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1Mjk=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1583,15 +2114,16 @@
                     ],
                     "weight": 0.0658737336745166
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODA5",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk0OA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MTU=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1620,15 +2152,16 @@
                     ],
                     "weight": 0.0349194743556176
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzg4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzNA==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MzM=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1657,15 +2190,16 @@
                     ],
                     "weight": 0.00222703068831837
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzg3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzMQ==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjY=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1694,15 +2228,16 @@
                     ],
                     "weight": 0.00541000379473566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzc4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk0Mw==",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MzE=",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1738,18 +2273,30 @@
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMjEwMzM=",
                     "inversion_solution_id": null,
                     "inversion_solution_type": null,
                     "onfault_nrml_id": "",
-                    "values": [],
+                    "rupture_set_id": "",
+                    "values": [
+                        {
+                            "long_name": "earthquake rates",
+                            "name": "r",
+                            "value": "uniform"
+                        },
+                        {
+                            "long_name": "hypocentral depths",
+                            "name": "d",
+                            "value": 1
+                        }
+                    ],
                     "weight": 1.0
                 }
             ],
             "long_name": "Intra-slab",
             "short_name": "SLAB"
         }
     ],
-    "title": "",
-    "version": "NSHM_1.0.0"
+    "title": "NSHM version 1.0.4, corrected fault geometry",
+    "version": "NSHM_v1.0.4"
 }
```

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v8_gmm_v2_final.py` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/SLT_v8_gmm_v2_final.py`

 * *Files identical despite different names*

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v9p0p0.json` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/nshm_v1.0.0.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7455357142857143%*

 * *Differences: {"'fault_system_lts'": "{0: {'branches': {0: {'onfault_nrml_id': "*

 * *                       "'SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcxNw==', 'inversion_solution_id': "*

 * *                       "'U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQ2', 'rupture_set_id': "*

 * *                       "'RmlsZToxNzU3My4wQUYzU1o='}, 1: {'onfault_nrml_id': "*

 * *                       "'SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcyMw==', 'inversion_solution_id': "*

 * *                       "'U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQz', 'rupture_set_id': "*

 * *  […]*

```diff
@@ -488,17 +488,18 @@
         }
     ],
     "fault_system_lts": [
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NTM=",
-                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTI5MTM3OA==",
+                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQ2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2NTc=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcxNw==",
+                    "rupture_set_id": "RmlsZToxNzU3My4wQUYzU1o=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "0.7"
                         },
                         {
@@ -520,17 +521,18 @@
                             "value": 0.28
                         }
                     ],
                     "weight": 0.21
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NTQ=",
-                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTI5MTM4Mg==",
+                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQz",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2NjE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcyMw==",
+                    "rupture_set_id": "RmlsZToxNzU3My4wQUYzU1o=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "0.7"
                         },
                         {
@@ -552,17 +554,18 @@
                             "value": 1.0
                         }
                     ],
                     "weight": 0.52
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NTU=",
-                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTI5MTM4Ng==",
+                    "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE4NTQ1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2NjY=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExODcyOQ==",
+                    "rupture_set_id": "RmlsZToxNzU3My4wQUYzU1o=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "0.7"
                         },
                         {
@@ -592,15 +595,16 @@
         },
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MjAw",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MTE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQyOA==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -624,15 +628,16 @@
                     ],
                     "weight": 0.147216637218474
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzQ=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MjAy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MDU=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxNw==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -656,15 +661,16 @@
                     ],
                     "weight": 0.281154911079988
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MjA0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MDM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQyOQ==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -688,15 +694,16 @@
                     ],
                     "weight": 0.148371277510384
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mzg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTk0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTk=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQyNA==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -720,15 +727,16 @@
                     ],
                     "weight": 0.0887399956599006
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTk2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MDg=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxMw==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -752,15 +760,16 @@
                     ],
                     "weight": 0.169475991711261
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTk4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE2MTM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxNg==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -784,15 +793,16 @@
                     ],
                     "weight": 0.0894359956258606
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDQ=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTY0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTg=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQxNA==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -816,15 +826,16 @@
                     ],
                     "weight": 0.0192986223768806
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTY2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTA=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQwNg==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -848,15 +859,16 @@
                     ],
                     "weight": 0.0368565846962387
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3NDg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTE0MTY4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1OTE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjExNDQwOQ==",
+                    "rupture_set_id": "RmlsZTo3MTQ3LjVramh3Rg==",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "TL"
                         },
                         {
@@ -886,15 +898,16 @@
         },
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzIy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MDE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5OA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -923,15 +936,16 @@
                     ],
                     "weight": 0.0168335471189857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzE3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODY=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxMQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -960,15 +974,16 @@
                     ],
                     "weight": 0.0408928149352719
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzQx",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MDI=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkwNA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -997,15 +1012,16 @@
                     ],
                     "weight": 0.0216771620919014
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzYx",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODI=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxNw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1034,15 +1050,16 @@
                     ],
                     "weight": 0.0282427120823285
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzUz",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkwNg==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1071,15 +1088,16 @@
                     ],
                     "weight": 0.0686084751056566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzU3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTA=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkwOA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1108,15 +1126,16 @@
                     ],
                     "weight": 0.0363691528229985
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzM0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxMw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1145,15 +1164,16 @@
                     ],
                     "weight": 0.00792374079868575
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzI4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTY=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkxMg==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1182,15 +1202,16 @@
                     ],
                     "weight": 0.0192487099590715
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzMw",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0OTQ=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkyNA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1219,15 +1240,16 @@
                     ],
                     "weight": 0.0102036850851
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzA4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NzM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4Ng==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1256,15 +1278,16 @@
                     ],
                     "weight": 0.0236560148670262
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzA3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0ODE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5Nw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1293,15 +1316,16 @@
                     ],
                     "weight": 0.0574662625307477
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzA1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0Njg=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg3NA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1330,15 +1354,16 @@
                     ],
                     "weight": 0.0304626983900857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzAy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NjQ=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5Mw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1367,15 +1392,16 @@
                     ],
                     "weight": 0.0271169544446554
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjk4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NzY=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4OQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1404,15 +1430,16 @@
                     ],
                     "weight": 0.0658737336745166
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjk2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0Njc=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg3MQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1441,15 +1468,16 @@
                     ],
                     "weight": 0.0349194743556176
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjcy",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NjA=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4MQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1478,15 +1506,16 @@
                     ],
                     "weight": 0.00222703068831837
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjc2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NzU=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg5Mg==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1515,15 +1544,16 @@
                     ],
                     "weight": 0.00541000379473566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNjc1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE0NjM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDg4Mg==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1552,15 +1582,16 @@
                     ],
                     "weight": 0.00286782725429677
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODI2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1Mzk=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk2NQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1589,15 +1620,16 @@
                     ],
                     "weight": 0.0168335471189857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODQ2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1Mzc=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk2Mw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1626,15 +1658,16 @@
                     ],
                     "weight": 0.0408928149352719
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODI0",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1Ng==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1663,15 +1696,16 @@
                     ],
                     "weight": 0.0216771620919014
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODY1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NDQ=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1Mw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1700,15 +1734,16 @@
                     ],
                     "weight": 0.0282427120823285
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODYz",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTk=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk2Nw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1737,15 +1772,16 @@
                     ],
                     "weight": 0.0686084751056566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODY5",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1NA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1774,15 +1810,16 @@
                     ],
                     "weight": 0.0363691528229985
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODQ3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NTg=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk3Mw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1811,15 +1848,16 @@
                     ],
                     "weight": 0.00792374079868575
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODE4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NDE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1NQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1848,15 +1886,16 @@
                     ],
                     "weight": 0.0192487099590715
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODM3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1NjI=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk3NA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geodetic"
                         },
                         {
@@ -1885,15 +1924,16 @@
                     ],
                     "weight": 0.0102036850851
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MDc=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODE1",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjI=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzNg==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1922,15 +1962,16 @@
                     ],
                     "weight": 0.0236560148670263
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTA=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODEx",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkyNw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1959,15 +2000,16 @@
                     ],
                     "weight": 0.0574662625307477
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTM=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODE2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjA=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzMg==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -1996,15 +2038,16 @@
                     ],
                     "weight": 0.0304626983900857
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTY=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODA3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MTY=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk1MQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -2033,15 +2076,16 @@
                     ],
                     "weight": 0.0271169544446554
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MTk=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzk2",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1Mjk=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk0NA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -2070,15 +2114,16 @@
                     ],
                     "weight": 0.0658737336745166
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjI=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwODA5",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MTU=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk0OA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -2107,15 +2152,16 @@
                     ],
                     "weight": 0.0349194743556176
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MjU=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzg4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MzM=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzNA==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -2144,15 +2190,16 @@
                     ],
                     "weight": 0.00222703068831837
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3Mjg=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzg3",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MjY=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDkzMQ==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -2181,15 +2228,16 @@
                     ],
                     "weight": 0.00541000379473566
                 },
                 {
                     "distributed_nrml_id": "RmlsZToxMzA3MzE=",
                     "inversion_solution_id": "U2NhbGVkSW52ZXJzaW9uU29sdXRpb246MTIwNzc4",
                     "inversion_solution_type": "ScaledInversionSolution",
-                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyOTE1MzE=",
+                    "onfault_nrml_id": "SW52ZXJzaW9uU29sdXRpb25Ocm1sOjEyMDk0Mw==",
+                    "rupture_set_id": "RmlsZToxMDAwODc=",
                     "values": [
                         {
                             "long_name": "deformation model",
                             "name": "dm",
                             "value": "geologic"
                         },
                         {
@@ -2225,14 +2273,15 @@
         {
             "branches": [
                 {
                     "distributed_nrml_id": "RmlsZToxMjEwMzM=",
                     "inversion_solution_id": null,
                     "inversion_solution_type": null,
                     "onfault_nrml_id": "",
+                    "rupture_set_id": "",
                     "values": [
                         {
                             "long_name": "earthquake rates",
                             "name": "r",
                             "value": "uniform"
                         },
                         {
@@ -2244,10 +2293,10 @@
                     "weight": 1.0
                 }
             ],
             "long_name": "Intra-slab",
             "short_name": "SLAB"
         }
     ],
-    "title": "NSHM version 1.0.4, corrected fault geometry",
-    "version": "NSHM_1.0.4"
+    "title": "aka SLT_v8_gmm_v2_final",
+    "version": "NSHM_v1.0.0"
 }
```

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/SLT_v9p0p0.py` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/SLT_v9p0p0.py`

 * *Files identical despite different names*

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/logic_tree.py` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/logic_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 class Branch:
     values: List[BranchAttributeValue]
     weight: float = 1.0
     onfault_nrml_id: Union[str, None] = ""
     distributed_nrml_id: Union[str, None] = ""
     inversion_solution_id: Union[str, None] = ""
     inversion_solution_type: Union[str, None] = ""
+    rupture_set_id: Union[str, None] = ""
 
 
 @dataclass
 class FaultSystemLogicTreeSpec:
     short_name: str
     long_name: str
     branches: List['BranchAttributeValue'] = field(default_factory=list)
```

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/slt_config.py` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/slt_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     SourceLogicTree,
     SourceLogicTreeCorrelation,
 )
 
 log = logging.getLogger(__name__)
 
 try:
-    from .toshi_api import toshi_api
+    from .toshi_api import solution_rupt_set_id, toshi_api
 except ModuleNotFoundError:
     log.warning("warning Toshi API module dependency not available, maybe you want to install with nzshm-model[toshi]")
 
 
 def get_config_groups(logic_tree_permutations) -> Generator:
     for permutation in logic_tree_permutations[0][0]['permute']:
         yield permutation
@@ -211,16 +211,24 @@
         )
 
     return correlations
 
 
 def resolve_toshi_source_ids(slt: SourceLogicTree) -> SourceLogicTree:
     new_slt = copy.deepcopy(slt)
+
+    # SKIP_FS_NAMES =['HIK', 'CRU'] #, 'CRU'
+
     for fslt in new_slt.fault_system_lts:
+        # if fslt.short_name in SKIP_FS_NAMES: #CRU
+        #     continue
         if fslt:  # fslt can be None
             for branch in fslt.branches:
                 nrml_info = toshi_api.get_source_from_nrml(branch.onfault_nrml_id)
                 # print(nrml_info)
                 branch.inversion_solution_id = nrml_info.solution_id
                 branch.inversion_solution_type = nrml_info.typename
+                if nrml_info.solution_id is not None:
+                    branch.rupture_set_id = solution_rupt_set_id(nrml_info.solution_id)
+                # print(branch) #, end='', flush=True)
                 # print('.', end='', flush=True)
     return new_slt
```

### Comparing `nzshm_model-0.2.0/nzshm_model/source_logic_tree/toshi_api.py` & `nzshm_model-0.3.0/nzshm_model/source_logic_tree/toshi_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,38 +116,80 @@
                 typename=executed['node']['source_solution']['__typename'],
                 solution_id=executed['node']['source_solution']['id'],
             )
             if executed.get('node')
             else InversionInfo()
         )
 
+    def get_rupture_set_id(self, solution_id):
+        qry = '''
+        query file0 ($id: ID!) {
+          node(id: $id) {
+            __typename
+            ... on PredecessorsInterface {
+              predecessors {
+                id
+                typename
+                relationship
+                depth
+                file_node: node {
+                  __typename
+                  ... on Node {id}
+                  ... on File {
+                    file_name
+                  }
+                }
+              }
+            }
+          }
+        }
+        '''
+        # print(qry)
+        input_variables = dict(id=solution_id)
+        # print(input_variables)
+        executed = self.run_query(qry, input_variables)
+        return executed['node']
+
 
 if 'TEST' in API_URL.upper():
     API_KEY = get_secret("NZSHM22_TOSHI_API_SECRET_TEST", "us-east-1").get("NZSHM22_TOSHI_API_KEY_TEST")
 elif 'PROD' in API_URL.upper():
     API_KEY = get_secret("NZSHM22_TOSHI_API_SECRET_PROD", "us-east-1").get("NZSHM22_TOSHI_API_KEY_PROD")
 else:
     API_KEY = os.getenv('NZSHM22_TOSHI_API_KEY', "")
 headers = {"x-api-key": API_KEY}
 toshi_api = ToshiApi(API_URL, None, with_schema_validation=False, headers=headers)
 
 
-if __name__ == "__main__":
+def solution_rupt_set_id(solution_id) -> str:
+    data = toshi_api.get_rupture_set_id(solution_id)
+    for itm in data['predecessors']:
+        if itm["typename"] == "File":
+            return itm['file_node']['id']
+    return ""
+
 
+if __name__ == "__main__":
+    """This should be a test!"""
     import dataclasses
     from pathlib import Path
 
     from nzshm_model.source_logic_tree.slt_config import from_config
 
+    SKIP_FS_NAMES = ['SLAB', 'HIK']  # , 'CRU'
+
     config_path = Path(__file__).parent / 'SLT_v8_gmm_v2_final.py'
     slt = from_config(config_path)
 
     for fslt in slt.fault_system_lts:
+        if fslt.short_name in SKIP_FS_NAMES:  # CRU
+            continue
         for branch in fslt.branches[-2:]:
             nrml_info = toshi_api.get_source_from_nrml(branch.onfault_nrml_id)
             print(nrml_info)
             branch.inversion_solution_id = nrml_info.solution_id
             branch.inversion_solution_type = nrml_info.typename
-            print('.', end='', flush=True)
+            branch.rupture_set_id = solution_rupt_set_id(nrml_info.solution_id)
+            print(branch)  # , end='', flush=True)
 
     j = json.dumps(dataclasses.asdict(slt), indent=4)
-    print(j)
+    # print(j)
```

### Comparing `nzshm_model-0.2.0/pyproject.toml` & `nzshm_model-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nzshm-model"
-version = "0.2.0"
+version = "0.3.0"
 description = "The logic tree definitions, final configurations, and versioning of the New Zealand | Aotearoa National Seismic Hazard Model"
 authors = ["Chris DiCaprio <c.dicaprio@gns.cri.nz>", "Chris Chamberlain <chrisbc@artisan.co.nz>"]
 license = "AGPL3"
 readme = "README.md"
 packages = [
 	{include = "nzshm_model"},
 	{include = "scripts"},
```

### Comparing `nzshm_model-0.2.0/scripts/slt.py` & `nzshm_model-0.3.0/scripts/slt.py`

 * *Files identical despite different names*

### Comparing `nzshm_model-0.2.0/tests/fixtures/large_SLT_example_A.py` & `nzshm_model-0.3.0/tests/fixtures/large_SLT_example_A.py`

 * *Files identical despite different names*

### Comparing `nzshm_model-0.2.0/tests/test_logic_tree.py` & `nzshm_model-0.3.0/tests/test_logic_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     f = FaultSystemLogicTree('Hik', 'Hikurangi', [b])
     print(f)
     assert f.branches[0].values[0].value == 4
 
 
 def test_fslt_example():
-    model_v1_0_0 = nzshm_model.get_model_version('NSHM_1.0.0')
+    model_v1_0_0 = nzshm_model.get_model_version('NSHM_v1.0.0')
     fslt = model_v1_0_0.build_crustal_branches()
 
     print(fslt)
     assert fslt.branches[-1].values[0].name == 'C'
     assert fslt.branches[-1].values[0].long_name == 'area-magnitude scaling'
     assert fslt.branches[-1].values[0].value == 4
 
@@ -76,22 +76,22 @@
     assert fslt.branches[-1].values[2].value == (0.95, 19.2)
     assert fslt.branches[-1].values[3].value == 'Geologic'
 
     assert fslt.validate_weights()
 
 
 def test_full_slt():
-    model_v1_0_0 = nzshm_model.get_model_version('NSHM_1.0.0')
+    model_v1_0_0 = nzshm_model.get_model_version('NSHM_v1.0.0')
     slt = SourceLogicTree('NSHM_1.0.0', 'initial', fault_system_lts=[model_v1_0_0.build_crustal_branches()])
     print(slt)
     assert slt.fault_system_lts[0].branches[-1].values[0].name == 'C'
 
 
 def test_serialise_slt():
-    model_v1_0_0 = nzshm_model.get_model_version('NSHM_1.0.0')
+    model_v1_0_0 = nzshm_model.get_model_version('NSHM_v1.0.0')
     slt = SourceLogicTree('NSHM_1.0.0', 'initial', fault_system_lts=[model_v1_0_0.build_crustal_branches()])
 
     slt_dict = dataclasses.asdict(slt)
     print(slt_dict)
     assert (
         slt.fault_system_lts[0].branches[-1].values[0].name
         == slt_dict['fault_system_lts'][0]['branches'][-1]['values'][0]['name']
```

### Comparing `nzshm_model-0.2.0/tests/test_slt_config.py` & `nzshm_model-0.3.0/tests/test_slt_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     get_config_group_tag_permutations,
     get_config_groups,
 )
 
 
 class TestStructure:
     def setup(self):
-        self.model = nzshm_model.get_model_version('NSHM_1.0.0')
+        self.model = nzshm_model.get_model_version('NSHM_v1.0.0')
 
     def test_slt_groups_v1_0_0(self):
         v1_0_0 = self.model
         groups = list(get_config_groups(v1_0_0.slt_config.logic_tree_permutations))
         for slt in groups:
             print(f'group {slt}')
         assert len(groups) == 4
```

### Comparing `nzshm_model-0.2.0/PKG-INFO` & `nzshm_model-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzshm-model
-Version: 0.2.0
+Version: 0.3.0
 Summary: The logic tree definitions, final configurations, and versioning of the New Zealand | Aotearoa National Seismic Hazard Model
 License: AGPL3
 Author: Chris DiCaprio
 Author-email: c.dicaprio@gns.cri.nz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

