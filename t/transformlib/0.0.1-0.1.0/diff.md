# Comparing `tmp/transformlib-0.0.1.tar.gz` & `tmp/transformlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformlib-0.0.1.tar", last modified: Sun Jan 10 15:07:51 2021, max compression
+gzip compressed data, was "transformlib-0.1.0.tar", last modified: Mon Apr 24 21:00:46 2023, max compression
```

## Comparing `transformlib-0.0.1.tar` & `transformlib-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 15:07:51.133448 transformlib-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     2397 2021-01-10 15:07:51.133448 transformlib-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1491 2021-01-10 15:07:41.000000 transformlib-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-10 15:07:51.133448 transformlib-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      643 2021-01-10 15:07:41.000000 transformlib-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 15:07:51.133448 transformlib-0.0.1/transformlib/
--rw-r--r--   0 runner    (1001) docker     (116)      352 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      209 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      223 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2659 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/node.py
--rw-r--r--   0 runner    (1001) docker     (116)     5349 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)      828 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/testing.py
--rw-r--r--   0 runner    (1001) docker     (116)     4512 2021-01-10 15:07:41.000000 transformlib-0.0.1/transformlib/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-10 15:07:51.133448 transformlib-0.0.1/transformlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2397 2021-01-10 15:07:50.000000 transformlib-0.0.1/transformlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      368 2021-01-10 15:07:51.000000 transformlib-0.0.1/transformlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-10 15:07:50.000000 transformlib-0.0.1/transformlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2021-01-10 15:07:50.000000 transformlib-0.0.1/transformlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-01-10 15:07:50.000000 transformlib-0.0.1/transformlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.508098 transformlib-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 21:00:46.508098 transformlib-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 21:00:33.000000 transformlib-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:00:46.508098 transformlib-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-24 21:00:33.000000 transformlib-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.504098 transformlib-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.504098 transformlib-0.1.0/src/transformlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 21:00:33.000000 transformlib-0.1.0/src/transformlib/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.508098 transformlib-0.1.0/src/transformlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 21:00:46.000000 transformlib-0.1.0/src/transformlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:00:46.508098 transformlib-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:00:33.000000 transformlib-0.1.0/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-24 21:00:33.000000 transformlib-0.1.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-24 21:00:33.000000 transformlib-0.1.0/tests/test_transform.py
```

### Comparing `transformlib-0.0.1/transformlib/pipeline.py` & `transformlib-0.1.0/src/transformlib/pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,92 @@
-# TODO:
-#   - Sort using graphlib in python 3.9
 from transformlib import Transform
 
 from transformlib.exceptions import TransformlibCycleException
 from transformlib.exceptions import TransformlibDuplicateTransformException
 
-from typing import List
 from typing import Dict
+from typing import List
+from typing import Optional
 
+from collections import deque
+from pathlib import Path
 import importlib
 import pkgutil
+import sys
 import time
-from collections import deque
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 # A graph is a dictionary of transforms (keys) to a list of transformations (value) which have
 # outputs that are inputs to given transform (key).
 Graph = Dict[Transform, List[Transform]]
 
 
 class Pipeline:
-    """A pipeline is a topologically ordered list of transforms."""
+    """A `Pipeline` is a topologically ordered list of transforms.
+
+    A `Pipeline` can be run from the command line:
+
+    .. highlight:: bash
+    .. code-block:: bash
+
+        transform path/to/transforms/*.py
+        transform -v path/to/transforms/*.py
 
-    def __init__(self, transforms: List[Transform] = []):
-        self.transforms = transforms
+    This will topologically sort and run all Transform objects found in the py files and save/load
+    the data from the `config.ROOT_DIR`.
+    """
+
+    def __init__(self, transforms: Optional[List[Transform]] = None):
+        if transforms is None:
+            self.transforms = []
+        else:
+            self.transforms = transforms
 
     @property
     def tasks(self):
+        """A topologically ordered list of transforms."""
         if len(set(self.transforms)) != len(self.transforms):
             raise TransformlibDuplicateTransformException(f"Duplicate {self.transforms}")
         return _get_tasks(self.transforms)  # Topologically sort the transforms.
 
     def __repr__(self):
         return (
             'Pipeline('
             + ', '.join(map(repr, self.tasks))
             + ')'
         )
 
-    def run(self):
+    def run(self) -> None:
         """Used to run all the transforms in the pipeline."""
         logger.info(f'Beginning running of {self}.')
-        start = time.time()
+        start = time.perf_counter()
         for transform in self.tasks:
             transform.run()
-        logger.info(f'Completed running of {self} took {time.time() - start}.')
+        logger.info(f'Completed running of {self} took {time.perf_counter() - start}.')
 
     @classmethod
     def discover_transforms(cls, *plugins):
         """Find and import all transforms in plugins.
 
         This function will automatically disover transforms from plugins
         using namespace packages e.g. fixed namespace(s), as defined by
         the input plugins args to the function, where plugins are saved.
 
+        Assuming you have a module called `transforms`. You can then find and
+        run all the Transform objects in this module:
+
+        >>> import transforms
+        >>> from transformlib.pipeline import Pipeline
+        >>> pipeline = Pipeline.discover_transforms(transforms)
+        >>> pipeline.run()
+
         Args:
             *plugins (module): Module(s) that contains transforms.
 
         Returns:
             Pipeline: A pipeline of the discovered transforms.
 
         References:
@@ -83,14 +108,33 @@
                 for attrname in dir(plugin_module):
                     new_attr = getattr(plugin_module, attrname)
                     if isinstance(new_attr, Transform):
                         logger.info(f"Discovered {new_attr} in {name}.")
                         transforms.append(new_attr)
         return cls(transforms)
 
+    def add_transforms_from_path(self, plugin_path: Path) -> None:
+        """Find and import all transform from a file.
+
+        Args:
+            plugin_path (Path): A path to a py file with Transform to
+                be added to the Pipeline.
+        """
+        try:
+            sys.path.insert(0, str(plugin_path.parent))
+            name = plugin_path.stem
+            plugin_module = importlib.import_module(name)
+            for attrname in dir(plugin_module):
+                new_attr = getattr(plugin_module, attrname)
+                if isinstance(new_attr, Transform):
+                    logger.info(f"Discovered {new_attr} in {name}.")
+                    self.transforms.append(new_attr)
+        finally:
+            sys.path.pop(0)
+
 
 def _get_tasks(transforms: List[Transform]) -> List[Transform]:
     """Get the tasks in order of execution.
 
     Args:
         transforms (List[Transform]): A list of transforms to be topologically ordered.
```

### Comparing `transformlib-0.0.1/transformlib/transform.py` & `transformlib-0.1.0/src/transformlib/transform.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,40 @@
 """Contains the Transform abstraction and helper methods.
 """
 from transformlib import Node
 from transformlib import Output
 from transformlib import Input
 
-from typing import List
+import time
 from typing import Tuple
 from typing import Dict
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class Transform:
     """Used to organize transformations of data.
 
-    A Transform is a many to many mapping between Inputs and Outputs. When run the Inputs are
-    loaded and the calculated outputs from the function is written to the Outputs.
+    A `Transform` is a many to many mapping between `Input` and `Output` nodes. When run the
+    `Input` nodes are loaded and the calculated outputs from the function is written to the
+    `Output` nodes.
     """
 
-    def __init__(self, output_args, func, input_kwargs):
-        self.output_args = output_args
+    def __init__(self, output_kwargs, func, input_kwargs):
+        self.output_kwargs = output_kwargs
         self.func = func
         self.input_kwargs = input_kwargs
 
     @property
-    def output_args(self):
-        """Output arguments of the transform.
-        """
-        return self._output_args
-
-    @output_args.setter
-    def output_args(self, value):
-        if len(set(value)) != len(value):
-            raise ValueError(f"Duplicate {value}")
-        self._output_args = value
-
-    @property
-    def input_kwargs(self):
-        """Input key value arguments of the transform.
-        """
-        return self._input_kwargs
-
-    @input_kwargs.setter
-    def input_kwargs(self, value):
-        if len(set(value.values())) != len(value.values()):
-            raise ValueError(f"Duplicate {value}")
-        self._input_kwargs = value
-
-    @property
     def outputs(self) -> Tuple[Output]:
         """A tuple with all the Outputs of the Transform.
         """
-        return tuple(self.output_args)
+        return tuple(self.output_kwargs.values())
 
     @property
     def inputs(self) -> Tuple[Input]:
         """A tuple with all the Inputs of the Transform.
         """
         return tuple(self.input_kwargs.values())
 
@@ -69,15 +46,18 @@
 
     def __call__(self, *args, **kwargs):
         return self.func(*args, **kwargs)
 
     def __repr__(self):
         return (
             f'{self.__class__}('
-            + ', '.join(map(repr, self.output_args))
+            + ', '.join(map(
+                lambda key: key + '=' + repr(self.output_kwargs[key]),
+                self.output_kwargs
+            ))
             + ', '.join(map(
                 lambda key: key + '=' + repr(self.input_kwargs[key]),
                 self.input_kwargs
             ))
             + ')'
         )
 
@@ -86,70 +66,46 @@
 
     def __eq__(self, other):
         if set(self.nodes) == set(other.nodes):
             return True
         return False
 
     def __hash__(self):
-        return hash((self.func, *self.output_args, *self.input_kwargs.items()))
-
-    def run(self, **param_kwargs):
-        """Runs a transform, the param_kwargs is overwritten by transform kwargs.
-
-        A parameter to a transform is an external transform input which is
-        NOT a DataFrame. This could be a model or the like.
-
-        Args:
-           *param_kwargs (Dict[str, Any]): A list og keyword argument
-                parameters to a transform.
+        return hash((self.func, *self.output_kwargs.items(), *self.input_kwargs.items()))
 
-        Returns:
-            Tuple[Output]: A tuple with the calculated outputs.
-        """
+    def run(self) -> None:
+        """Runs a transform."""
         logger.info(f'Beginning running of {self}.')
-        calc_outputs = self(
-            **param_kwargs,
-            **{
-                key: self.input_kwargs[key].load()
-                for key in self.input_kwargs
-            }
-        )
-        if len(self.outputs) == 1:
-            calc_outputs = (calc_outputs, )
-        else:
-            calc_outputs = tuple(calc_outputs)
-        for idx, output in enumerate(self.outputs):
-            output.save(calc_outputs[idx])
-        logger.info(f'Completed running of {self}.')
-        return calc_outputs
+        start = time.perf_counter()
+        self(**self.output_kwargs, **self.input_kwargs)
+        logger.info(f'Completed running of {self} took {time.perf_counter() - start}.')
 
 
-def transform(*args: Output, **kwargs: Input):
+def transform(**kwargs: Node):
     """Convert a function to a Transform.
 
     Args:
-        *args (List[Input]): The outputs of the transform.
-        **kwargs (Dict[str, Input]): The inputs to the transform.
+        **kwargs (Dict[str, Node]): The nodes of the transform.
 
     Returns:
         function: A decorator that returns a Transform object.
     """
     def decorator(func) -> Transform:
-        output_args = _filter_outputs(args)
+        output_kwargs = _filter_outputs(kwargs)
         input_kwargs = _filter_inputs(kwargs)
-        return Transform(output_args, func, input_kwargs)
+        return Transform(output_kwargs, func, input_kwargs)
     return decorator
 
 
-def _filter_outputs(args) -> List[Output]:
+def _filter_outputs(kwargs) -> Dict[str, Output]:
     """Filter out anything that is not an Output."""
-    return [
-        arg for arg in args
-        if isinstance(arg, Output)
-    ]
+    return {
+        key: kwargs[key] for key in kwargs
+        if isinstance(kwargs[key], Output)
+    }
 
 
 def _filter_inputs(kwargs) -> Dict[str, Input]:
     """Filter out anything that is not an Input."""
     return {
         key: kwargs[key] for key in kwargs
         if isinstance(kwargs[key], Input)
```

