# Comparing `tmp/pytreeclass-0.3.1.tar.gz` & `tmp/pytreeclass-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.1.tar", last modified: Sat Apr 22 05:26:51 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.2.tar", last modified: Mon Apr 24 01:04:21 2023, max compression
```

## Comparing `pytreeclass-0.3.1.tar` & `pytreeclass-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.105200 pytreeclass-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-04-22 05:26:51.105200 pytreeclass-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16700 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30822 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/pytreeclass/_src/tree_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 05:26:51.000000 pytreeclass-0.3.1/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:26:51.105200 pytreeclass-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:51.101200 pytreeclass-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-22 05:26:39.000000 pytreeclass-0.3.1/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24197 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.141938 pytreeclass-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.141938 pytreeclass-0.3.2/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30880 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/pytreeclass/_src/tree_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 01:04:21.000000 pytreeclass-0.3.2/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:21.145938 pytreeclass-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-24 01:04:08.000000 pytreeclass-0.3.2/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.1/LICENSE` & `pytreeclass-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/PKG-INFO` & `pytreeclass-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.1
+Version: 0.3.2
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
 |[**Quick Example**](#quick_example)
 |[**StatefulComputation**](#stateful_computation)
 |[**More**](#more)
 |[**Acknowledgements**](#acknowledgements)
 
 ![Tests](https://github.com/ASEM000/pytreeclass/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.8%203.9%203.10%203.11_-red)
-![pyver](https://img.shields.io/badge/jax-0.4.7+-red)
+![pyver](https://img.shields.io/badge/jax->=0.4.7-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/intro.ipynb)
 [![Downloads](https://pepy.tech/badge/pytreeclass)](https://pepy.tech/project/pytreeclass)
 [![codecov](https://codecov.io/gh/ASEM000/pytreeclass/branch/main/graph/badge.svg?token=TZBRMO0UQH)](https://codecov.io/gh/ASEM000/pytreeclass)
 [![Documentation Status](https://readthedocs.org/projects/pytreeclass/badge/?version=latest)](https://pytreeclass.readthedocs.io/en/latest/?badge=latest)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ASEM000/pytreeclass)
 [![DOI](https://zenodo.org/badge/512717921.svg)](https://zenodo.org/badge/latestdoi/512717921)
```

### Comparing `pytreeclass-0.3.1/README.md` & `pytreeclass-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 |[**Quick Example**](#quick_example)
 |[**StatefulComputation**](#stateful_computation)
 |[**More**](#more)
 |[**Acknowledgements**](#acknowledgements)
 
 ![Tests](https://github.com/ASEM000/pytreeclass/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.8%203.9%203.10%203.11_-red)
-![pyver](https://img.shields.io/badge/jax-0.4.7+-red)
+![pyver](https://img.shields.io/badge/jax->=0.4.7-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/intro.ipynb)
 [![Downloads](https://pepy.tech/badge/pytreeclass)](https://pepy.tech/project/pytreeclass)
 [![codecov](https://codecov.io/gh/ASEM000/pytreeclass/branch/main/graph/badge.svg?token=TZBRMO0UQH)](https://codecov.io/gh/ASEM000/pytreeclass)
 [![Documentation Status](https://readthedocs.org/projects/pytreeclass/badge/?version=latest)](https://pytreeclass.readthedocs.io/en/latest/?badge=latest)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ASEM000/pytreeclass)
 [![DOI](https://zenodo.org/badge/512717921.svg)](https://zenodo.org/badge/latestdoi/512717921)
```

### Comparing `pytreeclass-0.3.1/docs/conf.py` & `pytreeclass-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/pytreeclass/__init__.py` & `pytreeclass-0.3.2/pytreeclass/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytreeclass._src.tree_decorator import TreeClass, field
+from pytreeclass._src.tree_decorator import TreeClass, field, fields
 from pytreeclass._src.tree_freeze import freeze, is_frozen, is_nondiff, unfreeze
 from pytreeclass._src.tree_indexer import bcmap, is_tree_equal, tree_indexer
 from pytreeclass._src.tree_pprint import (
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
@@ -17,14 +17,15 @@
 )
 
 __all__ = (
     # general utils
     "TreeClass",
     "is_tree_equal",
     "field",
+    "fields",
     # pprint utils
     "tree_diagram",
     "tree_mermaid",
     "tree_repr",
     "tree_str",
     "tree_indent",
     "tree_summary",
@@ -39,8 +40,8 @@
     "tree_indexer",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
 )
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
```

### Comparing `pytreeclass-0.3.1/pytreeclass/_src/tree_decorator.py` & `pytreeclass-0.3.2/pytreeclass/_src/tree_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any, Callable, Hashable, NamedTuple, Sequence, TypeVar
 
 import jax.tree_util as jtu
 from typing_extensions import dataclass_transform
 
 from pytreeclass._src.tree_freeze import tree_hash
 from pytreeclass._src.tree_indexer import (
+    AtIndexer,
     _leafwise_transform,
     _mutable_context,
     _mutable_instance_registry,
     is_tree_equal,
     tree_copy,
     tree_indexer,
 )
@@ -27,15 +28,14 @@
     __repr__ = lambda _: "?"
 
 
 T = TypeVar("T", bound=Hashable)
 PyTree = Any
 
 _NOT_SET = NOT_SET()
-_FIELDS = "_fields"
 _POST_INIT = "__post_init__"
 _MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
 
 
 """Define a class decorator that is compatible with JAX's transformation."""
 
 
@@ -161,22 +161,22 @@
         metadata=metadata,  # type: ignore
         callbacks=callbacks,
         alias=alias,
     )
 
 
 @ft.lru_cache
-def _generate_field_map(klass: type) -> MappingProxyType[str, Field]:
+def build_field_map(klass: type) -> MappingProxyType[str, Field]:
     field_map = dict()  # type: dict[str, Field]
 
     if klass is object:
         return MappingProxyType(field_map)
 
     for base in reversed(klass.__mro__[1:]):
-        field_map.update(_generate_field_map(base))
+        field_map.update(build_field_map(base))
 
     # TODO: use inspect to get annotations, once we are on minimum python version >3.9
     if "__annotations__" not in vars(klass):
         return MappingProxyType(field_map)
 
     for name in (annotation_map := vars(klass)["__annotations__"]):
         value = vars(klass).get(name, _NOT_SET)
@@ -212,14 +212,20 @@
         else:
             # case: `x: int = 1`
             field_map[name] = Field(name=name, type=type, default=value)
 
     return MappingProxyType(field_map)
 
 
+def fields(tree: Any) -> Sequence[Field]:
+    """Returns a tuple of `Field` objects for the given instance or class."""
+    klass = tree if isinstance(tree, type) else type(tree)
+    return tuple(build_field_map(klass).values())
+
+
 @ft.lru_cache
 def _generate_init_code(fields: Sequence[Field]) -> str:
     head = body = ""
 
     for field in fields:
         name = field.name  # name in body
         alias = field.alias or name  # name in constructor
@@ -238,54 +244,45 @@
         else:
             head += f"{alias}, " if field.init else ""
             body += f"\t\tself.{name}={alias}\n " if field.init else ""
 
         if field.pos_only and field.init:
             head = head.replace("/,", "") + "/, "
 
-    body += "\t\tpass"  # add pass to avoid syntax error if all fields are ignored
+    body += "\t\tpass"  # add pass to avoid syntax error if all fieds are ignored
     body = "\tdef __init__(self, " + head[:-2] + "):\n" + body
     body = f"def closure(field_map):\n{body}\n\treturn __init__"
     return body.expandtabs(4)
 
 
 def _generate_init_method(klass: type) -> FunctionType:
-    field_map = _generate_field_map(klass)
+    field_map = build_field_map(klass)
     init_code = _generate_init_code(tuple(field_map.values()))
     exec(init_code, vars(sys.modules[klass.__module__]), local_namespace := dict())  # type: ignore
     method = local_namespace["closure"](field_map)
     method.__qualname__ = f"{klass.__qualname__}.__init__"
     return method
 
 
 def _setattr(tree: PyTree, key: str, value: Any) -> None:
     if id(tree) not in _mutable_instance_registry:
         msg = f"Cannot set attribute `{key}` = {value!r} on immutable instance of "
         msg += f"`{type(tree).__name__}`.\nUse `.at[`{key}`].set({value!r})` instead."
         raise AttributeError(msg)
 
-    if key in (field_map := vars(tree).get(_FIELDS, ())):
+    if key in (field_map := build_field_map(type(tree))):
         for callback in field_map[key].callbacks:
             try:
                 # callback is a function that takes the value of the field
                 # and returns a modified value
                 value = callback(value)
             except Exception as e:
                 msg = f"Error for field=`{key}`:\n{e}"
                 raise type(e)(msg)
 
-    elif isinstance(value, TreeClass):
-        # auto registers the instance value if it is a registered `treeclass`
-        # this behavior is similar to PyTorch behavior in `nn.Module`
-        # with instances of `Parameter`/`Module`.
-        # the behavior is useful to avoid repetitive code pattern in field definition and
-        # and initialization inside init method.
-        field = Field(type=type(value), init=False, name=key)
-        vars(tree)[_FIELDS] = MappingProxyType({**field_map, key: field})  # type: ignore
-
     vars(tree)[key] = value  # type: ignore
 
 
 def _delattr(tree, key: str) -> None:
     # delete the attribute under `_mutable_context` context
     # otherwise raise an error
     if id(tree) not in _mutable_instance_registry:
@@ -324,35 +321,32 @@
 
     return klass
 
 
 def _register_treeclass(klass: type[T]) -> type[T]:
     # handle all registration logic for `treeclass`
 
-    def tree_unflatten(treedef: Any, leaves: list[Any]) -> T:
+    def tree_unflatten(keys: tuple[str, ...], leaves: tuple[Any, ...]) -> T:
         # unflatten rule for `treeclass` to use with `jax.tree_unflatten`
         tree = getattr(object, "__new__")(klass)
-        vars(tree).update(treedef[1])
-        vars(tree).update(zip(treedef[0], leaves))
+        vars(tree).update(zip(keys, leaves))
         return tree
 
-    def tree_flatten(tree: T):
+    def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
         # flatten rule for `treeclass` to use with `jax.tree_flatten`
-        static, dynamic = dict(vars(tree)), dict()
-        for key in static.get(_FIELDS, ()):
-            dynamic[key] = static.pop(key)
-        return list(dynamic.values()), (tuple(dynamic.keys()), static)
+        keys, leaves = zip(*vars(tree).items())
+        return leaves, keys
 
-    def tree_flatten_with_keys(tree: PyTree):
+    def tree_flatten_with_keys(tree: T):
         # flatten rule for `treeclass` to use with `jax.tree_util.tree_flatten_with_path`
-        static, dynamic = dict(vars(tree)), dict()
-        for key in static.get(_FIELDS, ()):
-            entry = NamedSequenceKey(len(dynamic), key)
-            dynamic[key] = (entry, static.pop(key))
-        return list(dynamic.values()), (tuple(dynamic.keys()), static)
+        dynamic = dict(vars(tree))
+        for idx, key in enumerate(vars(tree)):
+            entry = NamedSequenceKey(idx, key)
+            dynamic[key] = (entry, dynamic[key])
+        return tuple(dynamic.values()), tuple(dynamic.keys())
 
     jtu.register_pytree_with_keys(
         nodetype=klass,
         flatten_func=tree_flatten,
         flatten_with_keys=tree_flatten_with_keys,
         unflatten_func=tree_unflatten,
     )
@@ -360,39 +354,38 @@
 
 
 class TreeClassMeta(ABCMeta):
     def __call__(klass: type[T], *a, **k) -> T:
         self = getattr(klass, "__new__")(klass, *a, **k)
 
         with _mutable_context(self):
-            setattr(self, _FIELDS, _generate_field_map(klass))
             getattr(klass, "__init__")(self, *a, **k)
 
             if post_init_func := getattr(klass, _POST_INIT, None):
                 # to simplify the logic, we call the post init method
                 # even if the init method is not code-generated.
                 post_init_func(self)
 
         # handle non-initialized fields
-        if len(keys := set(getattr(self, _FIELDS)) - set(vars(self))) > 0:
+        if len(keys := set(build_field_map(klass)) - set(vars(self))) > 0:
             msg = f"Uninitialized fields: ({', '.join(keys)}) in the instance of `{type(self).__name__}`"
             raise AttributeError(msg)
         return self
 
 
 @dataclass_transform(field_specifiers=(field, Field), frozen_default=True)
 class TreeClass(metaclass=TreeClassMeta):
     """Convert a class to a JAX compatible tree structure.
 
     Example:
         >>> import functools as ft
         >>> import jax
         >>> import pytreeclass as pytc
 
-        >>> # Tree leaves are defined by type hinted fields at the class level
+        >>> # Tree leaves are instance attributes
         >>> class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> jax.tree_util.tree_leaves(tree)
         [1, 2.0]
 
@@ -401,15 +394,15 @@
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree + 1
         Tree(a=2, b=3.0)
 
         >>> # Advanced indexing is supported using `at` property
-        ... class Tree(pytc.TreeClass):
+        >>> class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree.at["a"].get()
         Tree(a=1, b=None)
         >>> tree.at[0].get()
         Tree(a=1, b=None)
@@ -451,7 +444,11 @@
     """
 
     def __init_subclass__(klass: type[T], *a, leafwise: bool = False, **k) -> None:
         super().__init_subclass__(*a, **k)
         klass = _register_treeclass(klass)
         klass = _leafwise_transform(klass) if leafwise else klass
         klass = _treeclass_transform(klass)
+
+    @property
+    def at(self) -> AtIndexer:
+        ...
```

### Comparing `pytreeclass-0.3.1/pytreeclass/_src/tree_freeze.py` & `pytreeclass-0.3.2/pytreeclass/_src/tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/pytreeclass/_src/tree_indexer.py` & `pytreeclass-0.3.2/pytreeclass/_src/tree_indexer.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.2/pytreeclass/_src/tree_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,16 @@
     depth: int,
 ) -> str:
     name = type(node).__name__
     if depth == 0:
         fmt = "..."
 
     else:
-        kvs = ((k, vars(node)[k]) for k, f in node._fields.items() if f.repr)
+        skip = [f.name for f in pytc.fields(node) if not f.repr]
+        kvs = ((k, v) for k, v in vars(node).items() if k not in skip)
         fmt = (f"{k}={_node_pprint(v,indent+1,kind,width,depth-1)}" for k, v in kvs)
         fmt = (", \n" + "\t" * (indent + 1)).join(fmt)
     fmt = f"{name}(\n" + "\t" * (indent + 1) + (fmt) + "\n" + "\t" * (indent) + ")"
     return _format_width(fmt, width)
 
 
 def _node_type_pprint(
```

### Comparing `pytreeclass-0.3.1/pytreeclass/_src/tree_trace.py` & `pytreeclass-0.3.2/pytreeclass/_src/tree_trace.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.2/pytreeclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.1
+Version: 0.3.2
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
 |[**Quick Example**](#quick_example)
 |[**StatefulComputation**](#stateful_computation)
 |[**More**](#more)
 |[**Acknowledgements**](#acknowledgements)
 
 ![Tests](https://github.com/ASEM000/pytreeclass/actions/workflows/tests.yml/badge.svg)
 ![pyver](https://img.shields.io/badge/python-3.8%203.9%203.10%203.11_-red)
-![pyver](https://img.shields.io/badge/jax-0.4.7+-red)
+![pyver](https://img.shields.io/badge/jax->=0.4.7-red)
 ![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ASEM000/PyTreeClass/blob/main/assets/intro.ipynb)
 [![Downloads](https://pepy.tech/badge/pytreeclass)](https://pepy.tech/project/pytreeclass)
 [![codecov](https://codecov.io/gh/ASEM000/pytreeclass/branch/main/graph/badge.svg?token=TZBRMO0UQH)](https://codecov.io/gh/ASEM000/pytreeclass)
 [![Documentation Status](https://readthedocs.org/projects/pytreeclass/badge/?version=latest)](https://pytreeclass.readthedocs.io/en/latest/?badge=latest)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ASEM000/pytreeclass)
 [![DOI](https://zenodo.org/badge/512717921.svg)](https://zenodo.org/badge/latestdoi/512717921)
```

### Comparing `pytreeclass-0.3.1/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.2/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/setup.py` & `pytreeclass-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_indexing.py` & `pytreeclass-0.3.2/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_nn.py` & `pytreeclass-0.3.2/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_tree_freeze.py` & `pytreeclass-0.3.2/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_tree_operator.py` & `pytreeclass-0.3.2/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_tree_pprint.py` & `pytreeclass-0.3.2/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_tree_viz_util.py` & `pytreeclass-0.3.2/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.1/tests/test_treeclass.py` & `pytreeclass-0.3.2/tests/test_treeclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
-def test_field_metadata():
-    class Test(pytc.TreeClass, leafwise=True):
-        a: int = pytc.field(default=1, metadata={"a": 1})
-
-    assert Test()._fields["a"].metadata["a"] == 1
-
-
 def test_field_mutually_exclusive():
     with pytest.raises(ValueError):
         pytc.field(default=1, factory=lambda: 1)
 
     with pytest.raises(ValueError):
         pytc.field(default=1, pos_only=True, kw_only=True)
 
 
+def test_fields():
+    class Test(pytc.TreeClass):
+        a: int = pytc.field(default=1, metadata={"meta": 1})
+        b: int = 2
+
+    assert len(pytc.fields(Test)) == 2
+    assert pytc.fields(Test)[0].metadata == {"meta": 1}
+
+
 def test_field():
     assert pytc.field(default=1).default == 1
 
     with pytest.raises(TypeError):
         pytc.field(metadata=1)
 
     class Test(pytc.TreeClass):
@@ -185,15 +187,15 @@
             self.d = 5
 
         def inc(self, x):
             return x + 10
 
     l1 = L1()
 
-    assert jtu.tree_leaves(l1) == [2, 4, 5]
+    assert jtu.tree_leaves(l1) == [2, 4, 5, 5]
     assert l1.inc(10) == 20
     assert l1.sub(10) == 0
     assert l1.d == 5
 
     class L1(L0):
         a: int = 2
         b: int = 4
@@ -535,18 +537,16 @@
         def add_param(self, name, param):
             return setattr(self, name, param)
 
     tree = Tree()
 
     _, tree_with_weight = tree.at["add_param"]("weight", Parameter(3))
 
-    assert tree._fields != tree_with_weight._fields
     assert tree_with_weight.weight == Parameter(3)
     assert "weight" not in vars(tree)
-    assert "weight" not in tree._fields
 
 
 def test_field_factory():
     class Tree(pytc.TreeClass):
         a: int = pytc.field(factory=lambda: 1)
 
     assert Tree().a == 1
```

### Comparing `pytreeclass-0.3.1/tests/test_under_jit.py` & `pytreeclass-0.3.2/tests/test_under_jit.py`

 * *Files identical despite different names*

