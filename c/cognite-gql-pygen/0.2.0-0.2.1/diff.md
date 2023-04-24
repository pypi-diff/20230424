# Comparing `tmp/cognite_gql_pygen-0.2.0.tar.gz` & `tmp/cognite_gql_pygen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.2.0.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.2.1.tar", max compression
```

## Comparing `cognite_gql_pygen-0.2.0.tar` & `cognite_gql_pygen-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11349 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/LICENSE
--rw-r--r--   0        0        0     4050 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/README.md
--rw-r--r--   0        0        0     8930 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      238 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/_functions.sh
--rwxr-xr-x   0        0        0      572 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/cdf_signin.sh
--rwxr-xr-x   0        0        0      379 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/schema_publish.sh
--rwxr-xr-x   0        0        0      209 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/schema_render.sh
--rw-r--r--   0        0        0      167 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19068 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3910 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2629 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      346 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6259 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3046 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    15859 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     3609 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7034 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0      868 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/main.py
--rw-r--r--   0        0        0     1423 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1868 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1560 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     2008 2023-04-19 05:11:21.585093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      416 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1288 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1333 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      803 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1965 2023-04-19 05:11:21.589093 cognite_gql_pygen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5062 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4050 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/README.md
+-rw-r--r--   0        0        0     8930 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      238 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/bin/_functions.sh
+-rwxr-xr-x   0        0        0      572 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/bin/cdf_signin.sh
+-rwxr-xr-x   0        0        0      379 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/bin/schema_publish.sh
+-rwxr-xr-x   0        0        0      209 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/bin/schema_render.sh
+-rw-r--r--   0        0        0      167 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19068 2023-04-24 12:58:07.505374 cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3910 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      346 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6259 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3046 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    15859 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     3609 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0      868 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/main.py
+-rw-r--r--   0        0        0     1423 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1868 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1560 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     2008 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      416 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1288 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1333 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      803 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1965 2023-04-24 12:58:07.509374 cognite_gql_pygen-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5062 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.2.1/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.2.0/LICENSE` & `cognite_gql_pygen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/README.md` & `cognite_gql_pygen-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/bin/cdf_signin.sh` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/bin/cdf_signin.sh`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/domain_modeling/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import Dict, Generic, List, Optional, Type, TypeVar, Union, cast, get_args
+from typing import Dict, Generic, List, Optional, Type, TypeVar, Union, cast, get_args, get_type_hints
 
 import strawberry
 from strawberry.experimental.pydantic import UnregisteredTypeException
 from strawberry.schema.config import StrawberryConfig
 
 from cognite.dm_clients.domain_modeling.domain_model import DomainModel
 from cognite.dm_clients.misc import to_snake
@@ -109,20 +109,20 @@
         # this method could be called recursively, so avoid duplicate work:
         if name in self._processed_names:
             return
         self._processed_names.append(name)
 
         # all field names on our DomainModel:
         field_names = [key for key in cls.__fields__ if key not in {"externalId"}]
+        cls_annotations = get_type_hints(cls)
 
         # find any custom scalar fields (e.g: Timestamp, JSONObject), they need special consideration:
         scalar_fields = {}
         for field_name in field_names:
-            field = cls.__fields__[field_name]
-            field_type = field.annotation
+            field_type = cls_annotations[field_name]
             # find out if there is a custom scalar in this field's annotation:
             while type_args := get_args(field_type):
                 field_type = type_args[0]
 
             type_name = field_type.__name__
             scalar_name = f"{type_name}Scalar"
             # if there is, make a corresponding strawberry scalar (only once), and
```

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/main.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.2.1/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.2.1/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.2.1/cognite/gqlpygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/gqlpygen/main.py` & `cognite_gql_pygen-0.2.1/cognite/gqlpygen/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.2.1/cognite/gqlpygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.2.1/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.2.1/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.2.0/pyproject.toml` & `cognite_gql_pygen-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.2.0"
+version = "0.2.1"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
```

### Comparing `cognite_gql_pygen-0.2.0/PKG-INFO` & `cognite_gql_pygen-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Cognite graphQL Python generation SDK
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

