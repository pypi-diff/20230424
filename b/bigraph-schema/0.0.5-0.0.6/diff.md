# Comparing `tmp/bigraph-schema-0.0.5.tar.gz` & `tmp/bigraph-schema-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigraph-schema-0.0.5.tar", last modified: Thu Apr 20 03:37:58 2023, max compression
+gzip compressed data, was "bigraph-schema-0.0.6.tar", last modified: Mon Apr 24 01:31:22 2023, max compression
```

## Comparing `bigraph-schema-0.0.5.tar` & `bigraph-schema-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      151 2023-04-11 21:38:33.000000 bigraph-schema-0.0.5/README.md
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/bigraph_schema/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.5/bigraph_schema/__init__.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.5/bigraph_schema/parse.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18287 2023-04-20 03:36:19.000000 bigraph-schema-0.0.5/bigraph_schema/registry.py
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18379 2023-04-20 03:37:11.000000 bigraph-schema-0.0.5/bigraph_schema/schema.py
-drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/bigraph_schema.egg-info/
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1081 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/PKG-INFO
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      310 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       18 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/requires.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-20 03:37:58.000000 bigraph-schema-0.0.5/bigraph_schema.egg-info/top_level.txt
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-20 03:37:58.729590 bigraph-schema-0.0.5/setup.cfg
--rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-20 03:37:27.000000 bigraph-schema-0.0.5/setup.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      378 2023-04-24 01:31:10.000000 bigraph-schema-0.0.6/README.md
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/bigraph_schema/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      106 2023-04-19 21:19:48.000000 bigraph-schema-0.0.6/bigraph_schema/__init__.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     2140 2023-04-11 21:34:23.000000 bigraph-schema-0.0.6/bigraph_schema/parse.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      919 2023-04-20 03:53:50.000000 bigraph-schema-0.0.6/bigraph_schema/protocol.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    18353 2023-04-24 01:15:10.000000 bigraph-schema-0.0.6/bigraph_schema/registry.py
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)    19757 2023-04-24 01:30:22.000000 bigraph-schema-0.0.6/bigraph_schema/schema.py
+drwxrwxr-x   0 youdonotexist  (1000) youdonotexist  (1000)        0 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/bigraph_schema.egg-info/
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1309 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)      337 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)        1 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       25 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/requires.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       15 2023-04-24 01:31:22.000000 bigraph-schema-0.0.6/bigraph_schema.egg-info/top_level.txt
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)       38 2023-04-24 01:31:22.147589 bigraph-schema-0.0.6/setup.cfg
+-rw-rw-r--   0 youdonotexist  (1000) youdonotexist  (1000)     1327 2023-04-24 01:30:56.000000 bigraph-schema-0.0.6/setup.py
```

### Comparing `bigraph-schema-0.0.5/PKG-INFO` & `bigraph-schema-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.5
+Version: 0.0.6
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,12 +20,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # bigraph-schema
 
 A serializable type schema for compositional systems biology simulations
 
-## installation
+## Installation
 
 ```console
 pip install bigraph-schema
 ```
+
+## Tutorials
+[Demo notebook](https://vivarium-collective.github.io/bigraph-schema/notebooks/demo.html).
+
+Also check out [Bigraph Schema Basics Tutorial](https://vivarium-collective.github.io/bigraph-viz/notebooks/basics.html).
```

### Comparing `bigraph-schema-0.0.5/bigraph_schema/parse.py` & `bigraph-schema-0.0.6/bigraph_schema/parse.py`

 * *Files identical despite different names*

### Comparing `bigraph-schema-0.0.5/bigraph_schema/registry.py` & `bigraph-schema-0.0.6/bigraph_schema/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,18 @@
                     raise Exception(
                         'registry already contains an entry for {}: {} --> {}'.format(
                             registry_key, self.registry[key], item))
             else:
                 self.registry[registry_key] = item
         self.main_keys.add(key)
 
+    def register_multiple(self, schemas, force=False):
+        for key, schema in schemas.items():
+            self.register(key, schema, force=force)
+
     def access(self, key):
         """Get an item by key from the registry."""
         return self.registry.get(key)
 
     def list(self):
         return list(self.main_keys)
 
@@ -145,21 +149,21 @@
 
 class TypeRegistry(Registry):
 
     def __init__(self):
         super().__init__()
 
         self.supers = {}
-        self.register('_', {})
+        self.register('any', {})
 
 
     def register(self, key, item, alternate_keys=tuple(), force=False):
         item = copy.deepcopy(item)
         if isinstance(item, dict):
-            supers = item.get('_super', ['_']) # list of immediate supers
+            supers = item.get('_super', ['any']) # list of immediate supers
             if isinstance(supers, str):
                 supers = [supers]
                 item['_super'] = supers
             for su in supers:
                 assert isinstance(
                     su, str), f"super for {key} must be a string, not {su}"
             self.supers[key] = supers
@@ -202,16 +206,15 @@
 
     def substitute_type(self, schema):
         if isinstance(schema, str):
             schema = self.access(schema)
         elif '_type' in schema:
             type_key = schema['_type']
             type_schema = self.access(type_key)
-            schema = schema.copy()
-            schema.pop('_type')
+            type_schema = copy.deepcopy(type_schema)
             schema.update(type_schema)
 
         return schema
 
 
     def expand_schema(self, schema):
         # make this only show the types at the leaves
@@ -436,37 +439,14 @@
         '_apply': 'replace',
         '_serialize': 'str',
         '_deserialize': 'str',
         '_divide': 'divide_int',
         '_description': '64-bit integer'
     },
 
-    # 'float binomial division': {
-    #     '_divide': 'divide_binomial',
-    #     '_description': '64-bit integer',
-    #     '_super': 'float', 
-    # },
-
-    'shape': {},
-
-    'rectangle': {
-        'width': {'_type': 'int'},
-        'height': {'_type': 'int'},
-        '_divide': 'divide_longest',
-        '_description': 'a two-dimensional value',
-        '_super': 'shape',
-    },
-
-    # if we override an existing non-_ key, throw an error?
-    # cannot override existing keys unless it is of a subtype
-    'cube': {
-        'depth': {'_type': 'int'},
-        '_super': 'rectangle',
-    },
-
     'list': {
         '_default': '[]',
         '_apply': 'concatenate',
         '_serialize': 'str',
         '_deserialize': 'eval',
         '_divide': 'divide_list',
         '_type_parameters': ['A'],
@@ -493,16 +473,15 @@
     #     'process': {'_type': 'process instance'},
     #     'config': {'_type': 'dict'},
     #     '_super': 'edge',
     # },
 }
 
 
-for key, schema in type_library.items():
-    type_registry.register(key, schema)
+type_registry.register_multiple(type_library)
 
 
 supported_units = {
     'm/s': {
         '_default': 0.0,
         '_apply': 'accumulate',
         '_serialize': 'str',
@@ -594,14 +573,36 @@
             'cytoplasm': cytoplasm_schema
         }
     }, {
         
     })
 
 
+def test_cube():
+    cube_schema = {
+        'shape': {},
+        
+        'rectangle': {
+            'width': {'_type': 'int'},
+            'height': {'_type': 'int'},
+            '_divide': 'divide_longest',
+            '_description': 'a two-dimensional value',
+            '_super': 'shape',
+        },
+        
+        # cannot override existing keys unless it is of a subtype
+        'cube': {
+            'depth': {'_type': 'int'},
+            '_super': 'rectangle',
+        },
+    }
+
+    type_registry.register_multiple(cube_schema)
+
+
 def test_generate_default():
     int_default = type_registry.generate_default(
         {'_type': 'int'}
     )
     assert int_default == 0
 
     cube_default = type_registry.generate_default(
@@ -625,10 +626,11 @@
         type_registry.register('int', type_library['string'])
 
     type_registry.register('int', type_library['string'], force=True)
     type_registry.register('int', type_library['int'], force=True)
 
 
 if __name__ == '__main__':
+    test_cube()
     test_generate_default()
     test_expand_schema()
     test_reregister_type()
```

### Comparing `bigraph-schema-0.0.5/bigraph_schema/schema.py` & `bigraph-schema-0.0.6/bigraph_schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import pprint
-from bigraph_schema.registry import registry_registry, type_schema_keys, optional_schema_keys, type_library, deep_merge
+from bigraph_schema.registry import registry_registry, type_schema_keys, optional_schema_keys, type_library, deep_merge, test_cube
 
 
 type_registry = registry_registry.access('_type')
+apply_registry = registry_registry.access('_apply')
 serialize_registry = registry_registry.access('_serialize')
 deserialize_registry = registry_registry.access('_deserialize')
 
 
 def validate_schema(schema, enforce_connections=False):
     # add ports and wires
     # validate ports are wired to a matching type,
@@ -235,15 +236,41 @@
 def fill(schema, state=None):
     if state is not None:
         state = copy.deepcopy(state)
     return fill_state(schema, state=state)
 
 
 def apply_update(schema, state, update):
-    pass
+    # expects an expanded schema
+
+    if '_apply' in schema:
+        apply_function = apply_registry.access(schema['_apply'])
+        state = apply_function(state, update)
+    elif isinstance(update, dict):
+        for key, branch in update.items():
+            if key not in schema:
+                raise Exception(f'trying to update a key that is not in the schema {key} for state:\n{state}\nwith schema:\n{schema}')
+            else:
+                subupdate = apply_update(
+                    schema[key],
+                    state[key],
+                    branch
+                )
+
+                state[key] = subupdate
+    else:
+        raise Exception(f'trying to apply an update that is unrecognized {update} for state:\n{state}\nwith schema:\n{schema}')
+
+    return state
+
+
+def apply(schema, initial, update):
+    expanded = type_registry.expand(schema)
+    state = copy.deepcopy(initial)
+    return apply_update(expanded, initial, update)
 
 
 def link_place(place, link):
     pass
 
 
 def compose(a, b):
@@ -709,22 +736,44 @@
                 'e0.1': 'v4',
                 'e0.2': ('v4', 'v5')}}}    
 
     result = link_place(placegraph, hypergraph)
     # assert result == merged
 
 
+def test_apply_update():
+    schema = {'_type': 'cube'}
+    state = {
+        'width': 11,
+        'height': 13,
+        'depth': 44,
+    }
+    update = {
+        'depth': -5
+    }
+
+    new_state = apply(
+        schema,
+        state,
+        update
+    )
+
+    assert new_state['width'] == 11
+    assert new_state['depth'] == 39
+
+
 if __name__ == '__main__':
+    test_cube()
     test_validate_schema()
     test_fill_int()
     test_fill_cube()
     test_establish_path()
     test_fill_in_missing_nodes()
     test_expected_schema()
-
+    test_apply_update()
```

### Comparing `bigraph-schema-0.0.5/bigraph_schema.egg-info/PKG-INFO` & `bigraph-schema-0.0.6/bigraph_schema.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigraph-schema
-Version: 0.0.5
+Version: 0.0.6
 Summary: A serializable type schema for compositional systems biology
 Home-page: https://github.com/vivarium-collective/bigraph-schema
 Author: Eran Agmon, Ryan Spangler
 Author-email: agmon.eran@gmail.com, ryan.spangler@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,12 +20,17 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # bigraph-schema
 
 A serializable type schema for compositional systems biology simulations
 
-## installation
+## Installation
 
 ```console
 pip install bigraph-schema
 ```
+
+## Tutorials
+[Demo notebook](https://vivarium-collective.github.io/bigraph-schema/notebooks/demo.html).
+
+Also check out [Bigraph Schema Basics Tutorial](https://vivarium-collective.github.io/bigraph-viz/notebooks/basics.html).
```

### Comparing `bigraph-schema-0.0.5/setup.py` & `bigraph-schema-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
 
 
 setup(
@@ -34,9 +34,10 @@
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
     install_requires=[
         # List your package dependencies here
         "parsimonious",
         "fire",
+        "pytest",
     ],
 )
```

