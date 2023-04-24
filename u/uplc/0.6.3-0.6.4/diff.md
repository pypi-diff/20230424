# Comparing `tmp/uplc-0.6.3.tar.gz` & `tmp/uplc-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplc-0.6.3.tar", last modified: Thu Apr 13 21:05:39 2023, max compression
+gzip compressed data, was "uplc-0.6.4.tar", last modified: Mon Apr 24 17:44:30 2023, max compression
```

## Comparing `uplc-0.6.3.tar` & `uplc-0.6.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.850954 uplc-0.6.3/
--rw-r--r--   0 travis    (1000) travis    (1000)     1077 2023-04-13 20:58:12.000000 uplc-0.6.3/LICENSE.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-13 21:05:39.850954 uplc-0.6.3/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     2034 2023-04-13 20:58:12.000000 uplc-0.6.3/README.md
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-13 21:05:39.850954 uplc-0.6.3/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     2056 2023-04-13 20:58:12.000000 uplc-0.6.3/setup.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.842954 uplc-0.6.3/uplc/
--rw-r--r--   0 travis    (1000) travis    (1000)      555 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4935 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    26686 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9066 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/flat_decoder.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10052 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/flat_encoder.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1202 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/lexer.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3357 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/machine.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.846954 uplc-0.6.3/uplc/optimizer/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/optimizer/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      630 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/optimizer/pre_evaluation.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10960 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/parser.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.846954 uplc-0.6.3/uplc/tests/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3391 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/test_acceptance.py
--rw-r--r--   0 travis    (1000) travis    (1000)    14104 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/test_hypothesis.py
--rw-r--r--   0 travis    (1000) travis    (1000)   211128 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/test_misc.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1998 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tools.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.850954 uplc-0.6.3/uplc/transformer/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      784 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/debrujin_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)      938 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/undebrujin_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1947 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/unique_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3009 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.846954 uplc-0.6.3/uplc.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      673 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       44 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      110 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        5 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.313256 uplc-0.6.4/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1077 2023-04-24 17:34:06.000000 uplc-0.6.4/LICENSE.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-24 17:44:30.313256 uplc-0.6.4/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     2034 2023-04-24 17:34:06.000000 uplc-0.6.4/README.md
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-24 17:44:30.313256 uplc-0.6.4/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     2056 2023-04-24 17:34:06.000000 uplc-0.6.4/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.305256 uplc-0.6.4/uplc/
+-rw-r--r--   0 travis    (1000) travis    (1000)      555 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4935 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/__main__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    28464 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9066 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/flat_decoder.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10052 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/flat_encoder.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1202 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/lexer.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3357 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/machine.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.309256 uplc-0.6.4/uplc/optimizer/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/optimizer/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      630 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/optimizer/pre_evaluation.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10960 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/parser.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.309256 uplc-0.6.4/uplc/tests/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3391 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/test_acceptance.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    14584 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/test_hypothesis.py
+-rw-r--r--   0 travis    (1000) travis    (1000)   211128 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tests/test_misc.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1998 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/tools.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.313256 uplc-0.6.4/uplc/transformer/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      784 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/debrujin_variables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      938 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/undebrujin_variables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1947 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/transformer/unique_variables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3009 2023-04-24 17:34:06.000000 uplc-0.6.4/uplc/util.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-24 17:44:30.309256 uplc-0.6.4/uplc.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      673 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       44 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      110 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        5 2023-04-24 17:44:30.000000 uplc-0.6.4/uplc.egg-info/top_level.txt
```

### Comparing `uplc-0.6.3/LICENSE.txt` & `uplc-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/PKG-INFO` & `uplc-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uplc
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python implementation of untyped plutus language core
 Home-page: https://github.com/opshin/uplc
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `uplc-0.6.3/README.md` & `uplc-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/setup.py` & `uplc-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/__init__.py` & `uplc-0.6.4/uplc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 import logging
 
 
-VERSION = (0, 6, 3)
+VERSION = (0, 6, 4)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/opshin/uplc"
```

### Comparing `uplc-0.6.3/uplc/__main__.py` & `uplc-0.6.4/uplc/__main__.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/ast.py` & `uplc-0.6.4/uplc/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,52 +338,70 @@
 
     def typestring(self, dialect=UPLCDialect.Aiken):
         return "data"
 
     def valuestring(self, dialect=UPLCDialect.Aiken):
         return f"#{plutus_cbor_dumps(self).hex()}"
 
-    def to_cbor(self) -> bytes:
+    def to_cbor(self) -> Any:
         """Returns a CBOR encodable representation of this object"""
         raise NotImplementedError
 
+    def to_json(self) -> dict:
+        """Returns a JSON encodable representation of this object"""
+        raise NotImplementedError
+
 
 @dataclass(frozen=True)
 class PlutusAtomic(PlutusData):
     value: Any
 
     def to_cbor(self):
         return self
 
 
 @dataclass(frozen=True, eq=True)
 class PlutusInteger(PlutusAtomic):
     value: int
 
+    def to_json(self):
+        return {"int": self.value}
+
 
 @dataclass(frozen=True, eq=True)
 class PlutusByteString(PlutusAtomic):
     value: bytes
 
+    def to_json(self):
+        return {"bytes": self.value.hex()}
+
 
 @dataclass(frozen=True, eq=True)
 class PlutusList(PlutusData):
     value: Union[List[PlutusData], frozenlist.FrozenList]
 
     def to_cbor(self):
         return [d.to_cbor() for d in self.value]
 
+    def to_json(self):
+        return {"list": [v.to_json() for v in self.value]}
+
 
 @dataclass(frozen=True, eq=True)
 class PlutusMap(PlutusData):
     value: Union[Dict[PlutusData, PlutusData], frozendict.frozendict]
 
     def to_cbor(self):
         return {k.to_cbor(): v.to_cbor() for k, v in self.value.items()}
 
+    def to_json(self):
+        return {
+            "map": [{"k": k.to_json(), "v": v.to_json()} for k, v in self.value.items()]
+        }
+
 
 @dataclass(frozen=True, eq=True)
 class PlutusConstr(PlutusData):
     constructor: int
     fields: Union[List[PlutusData], frozenlist.FrozenList]
 
     def to_cbor(self):
@@ -396,14 +414,20 @@
                 (self.constructor - 7) + 1280, [f.to_cbor() for f in self.fields]
             )
         else:
             return cbor2.CBORTag(
                 102, [self.constructor, [f.to_cbor() for f in self.fields]]
             )
 
+    def to_json(self):
+        return {
+            "constructor": self.constructor,
+            "fields": [v.to_json() for v in self.fields],
+        }
+
 
 def _int_to_bytes(x: int):
     return x.to_bytes((x.bit_length() + 7) // 8, byteorder="big")
 
 
 def default_encoder(encoder: CBOREncoder, value: PlutusData):
     """A fallback function that encodes PlutusData objects"""
@@ -471,21 +495,56 @@
         return PlutusList(entries)
     if isinstance(cbor, dict):
         return PlutusMap(
             frozendict.frozendict(
                 {data_from_cbortag(k): data_from_cbortag(v) for k, v in cbor.items()}
             )
         )
+    raise NotImplementedError(f"Unknown cbor type notation in {cbor}")
 
 
 def data_from_cbor(cbor: bytes) -> PlutusData:
     raw_datum = cbor2.loads(cbor)
     return data_from_cbortag(raw_datum)
 
 
+def data_from_json_dict(d: dict) -> PlutusData:
+    if "constructor" in d:
+        fields = frozenlist.FrozenList([data_from_json_dict(f) for f in d["fields"]])
+        fields.freeze()
+        return PlutusConstr(d["constructor"], fields)
+    if "int" in d:
+        return PlutusInteger(d["int"])
+    if "bytes" in d:
+        return PlutusByteString(bytes.fromhex(d["bytes"]))
+    if "list" in d:
+        entries = frozenlist.FrozenList(list(map(data_from_json_dict, d["list"])))
+        entries.freeze()
+        return PlutusList(entries)
+    if "map" in d:
+        return PlutusMap(
+            frozendict.frozendict(
+                {
+                    data_from_json_dict(m["k"]): data_from_json_dict(m["v"])
+                    for m in d["map"]
+                }
+            )
+        )
+    raise NotImplementedError(f"Unknown json notation in {d}")
+
+
+def data_from_json(json_string: str) -> PlutusData:
+    raw_datum = json.loads(json_string)
+    return data_from_json_dict(raw_datum)
+
+
+def plutus_json_dumps(x: PlutusData):
+    return json.dumps(x.to_json())
+
+
 class ConstantType(Enum):
     integer = auto()
     bytestring = auto()
     string = auto()
     unit = auto()
     bool = auto()
     pair = auto()
```

### Comparing `uplc-0.6.3/uplc/flat_decoder.py` & `uplc-0.6.4/uplc/flat_decoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/flat_encoder.py` & `uplc-0.6.4/uplc/flat_encoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/lexer.py` & `uplc-0.6.4/uplc/lexer.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/machine.py` & `uplc-0.6.4/uplc/machine.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/optimizer/pre_evaluation.py` & `uplc-0.6.4/uplc/optimizer/pre_evaluation.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/parser.py` & `uplc-0.6.4/uplc/parser.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/tests/test_acceptance.py` & `uplc-0.6.4/uplc/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/tests/test_hypothesis.py` & `uplc-0.6.4/uplc/tests/test_hypothesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,7 +393,19 @@
     )
     @hypothesis.example(Program(version=(1, 0, 0), term=BuiltinUnit()))
     def test_flat_unflat_roundtrip(self, p: Program):
         p_unique = unique_variables.UniqueVariableTransformer().visit(p)
         self.assertEqual(p_unique, unflatten(flatten(p)), "incorrect flatten roundtrip")
 
     # TODO test invalid programs being detected with an free variable error
+
+    @hypothesis.given(uplc_data)
+    def test_cbor_plutus_data_roundtrip(self, p: PlutusData):
+        encoded = plutus_cbor_dumps(p)
+        decoded = data_from_cbor(encoded)
+        self.assertEqual(p, decoded, "incorrect cbor roundtrip")
+
+    @hypothesis.given(uplc_data)
+    def test_json_plutus_data_roundtrip(self, p: PlutusData):
+        encoded = p.to_json()
+        decoded = data_from_json_dict(encoded)
+        self.assertEqual(p, decoded, "incorrect json roundtrip")
```

### Comparing `uplc-0.6.3/uplc/tests/test_misc.py` & `uplc-0.6.4/uplc/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/tools.py` & `uplc-0.6.4/uplc/tools.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/transformer/debrujin_variables.py` & `uplc-0.6.4/uplc/transformer/debrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/transformer/undebrujin_variables.py` & `uplc-0.6.4/uplc/transformer/undebrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/transformer/unique_variables.py` & `uplc-0.6.4/uplc/transformer/unique_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc/util.py` & `uplc-0.6.4/uplc/util.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.3/uplc.egg-info/PKG-INFO` & `uplc-0.6.4/uplc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uplc
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python implementation of untyped plutus language core
 Home-page: https://github.com/opshin/uplc
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `uplc-0.6.3/uplc.egg-info/SOURCES.txt` & `uplc-0.6.4/uplc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

