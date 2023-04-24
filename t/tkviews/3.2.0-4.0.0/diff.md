# Comparing `tmp/tkviews-3.2.0.tar.gz` & `tmp/tkviews-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkviews-3.2.0.tar", last modified: Thu Nov 17 13:05:13 2022, max compression
+gzip compressed data, was "tkviews-4.0.0.tar", last modified: Mon Apr 24 11:55:37 2023, max compression
```

## Comparing `tkviews-3.2.0.tar` & `tkviews-4.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:13.418162 tkviews-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-17 13:04:48.000000 tkviews-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-17 13:05:13.418162 tkviews-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-11-17 13:04:48.000000 tkviews-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-11-17 13:04:48.000000 tkviews-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 13:05:13.418162 tkviews-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-11-17 13:04:48.000000 tkviews-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:13.414162 tkviews-3.2.0/tkviews/
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:13.414162 tkviews-3.2.0/tkviews/core/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/core/rendering.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/listbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:13.414162 tkviews-3.2.0/tkviews/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4291 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/widgets/binding.py
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/widgets/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/widgets/setters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-11-17 13:04:48.000000 tkviews-3.2.0/tkviews/widgets/ttk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:05:13.414162 tkviews-3.2.0/tkviews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-17 13:05:13.000000 tkviews-3.2.0/tkviews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-11-17 13:05:13.000000 tkviews-3.2.0/tkviews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 13:05:13.000000 tkviews-3.2.0/tkviews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-17 13:05:13.000000 tkviews-3.2.0/tkviews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-17 13:05:13.000000 tkviews-3.2.0/tkviews.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:55:37.750300 tkviews-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 11:55:15.000000 tkviews-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-24 11:55:37.750300 tkviews-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-24 11:55:15.000000 tkviews-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-24 11:55:15.000000 tkviews-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:55:37.750300 tkviews-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 11:55:15.000000 tkviews-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:55:37.746300 tkviews-4.0.0/tkviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:55:37.750300 tkviews-4.0.0/tkviews/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/core/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/listbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:55:37.750300 tkviews-4.0.0/tkviews/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/widgets/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/widgets/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/widgets/setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-24 11:55:15.000000 tkviews-4.0.0/tkviews/widgets/ttk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:55:37.750300 tkviews-4.0.0/tkviews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-24 11:55:37.000000 tkviews-4.0.0/tkviews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-24 11:55:37.000000 tkviews-4.0.0/tkviews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:55:37.000000 tkviews-4.0.0/tkviews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 11:55:37.000000 tkviews-4.0.0/tkviews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 11:55:37.000000 tkviews-4.0.0/tkviews.egg-info/top_level.txt
```

### Comparing `tkviews-3.2.0/LICENSE` & `tkviews-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkviews-3.2.0/PKG-INFO` & `tkviews-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkviews
-Version: 3.2.0
+Version: 4.0.0
 Summary: Package for creating tkinter applications in declarative way.
 Project-URL: Homepage, https://github.com/eumis/tkviews
 Keywords: binding,tkinter,tk,tkviews,pyviews,python,mvvm,views
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
@@ -52,12 +52,16 @@
 To run demo app execute following commands
 
 ```
 cd [root_folder]\demo
 python run.py
 ```
 
+## Docs
+
+See some documentation in [docs](https://github.com/eumis/tkviews/tree/dev/docs) folder
+
 ## License
 
 [MIT](http://opensource.org/licenses/MIT)
 
 Copyright (c) 2017-present, eumis (Eugen Misievich)
```

### Comparing `tkviews-3.2.0/README.md` & `tkviews-4.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,16 @@
 To run demo app execute following commands
 
 ```
 cd [root_folder]\demo
 python run.py
 ```
 
+## Docs
+
+See some documentation in [docs](https://github.com/eumis/tkviews/tree/dev/docs) folder
+
 ## License
 
 [MIT](http://opensource.org/licenses/MIT)
 
-Copyright (c) 2017-present, eumis (Eugen Misievich)
+Copyright (c) 2017-present, eumis (Eugen Misievich)
```

### Comparing `tkviews-3.2.0/tkviews/__init__.py` & `tkviews-4.0.0/tkviews/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Package adapts pyviews for using with tkinter"""
 
-__version__ = '3.2.0'
+__version__ = '4.0.0'
 
 from pyviews.setters import import_global, inject_global, call, set_global, Args, call_args
 from pyviews.code import Code
 from pyviews.containers import Container, View, For, If
 from pyviews.presenter import PresenterNode, add_reference
 
 from .styles import Style, StylesView, StyleItem, apply_styles
```

### Comparing `tkviews-3.2.0/tkviews/app.py` & `tkviews-4.0.0/tkviews/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """tkinter application entry point"""
 
 from typing import Optional, cast
 
 from injectool import add_singleton
-from pyviews.binding import use_binding
+from pyviews.binding.config import use_binding
 from pyviews.code import run_code
-from pyviews.containers import get_container_pipeline, get_view_pipeline, get_for_pipeline, get_if_pipeline
+from pyviews.containers import get_container_pipeline, get_for_pipeline, get_if_pipeline, get_view_pipeline
+from pyviews.core.rendering import NodeGlobals
 from pyviews.presenter import get_presenter_pipeline
-from pyviews.rendering import RenderingPipeline, use_rendering, get_child_context
-from pyviews.rendering.pipeline import use_pipeline
-from pyviews.rendering.views import render_view
+from pyviews.rendering.context import get_child_context
+from pyviews.rendering.pipeline import RenderingPipeline, render_view, use_pipeline
+from pyviews.rendering.config import use_rendering
 
 from tkviews.canvas import get_canvas_pipeline
 from tkviews.core.rendering import TkRenderingContext, get_tk_child_context
 from tkviews.listbox import get_listboxitem_pipeline
 from tkviews.styles import get_style_pipeline, get_styles_view_pipeline
-from tkviews.widgets import get_root_pipeline, get_widget_pipeline, Root
-from tkviews.widgets import use_variables_binding
+from tkviews.widgets import Root, get_root_pipeline, get_widget_pipeline, use_variables_binding
 from tkviews.widgets.ttk import get_ttk_style_pipeline
 
 
 def register_dependencies():
     """Registers all dependencies needed for application"""
     use_rendering()
     use_binding()
@@ -43,15 +43,16 @@
 
     use_pipeline(get_style_pipeline(), 'tkviews.Style')
     use_pipeline(get_styles_view_pipeline(), 'tkviews.StylesView')
     use_pipeline(get_ttk_style_pipeline(), 'tkviews.TtkStyle')
     use_pipeline(get_canvas_pipeline(), 'tkviews.canvas')
     use_pipeline(get_listboxitem_pipeline(), 'tkviews.ListboxItem')
 
-    use_pipeline(RenderingPipeline(pipes=[run_code]), 'tkviews.Code')
+    use_pipeline(RenderingPipeline(pipes = [run_code]), 'tkviews.Code')
 
 
-def launch(root_view: Optional[str] = None):
+def launch(root_view: str, view_globals: Optional[dict] = None):
     """Runs application. Widgets are created from passed xml_files"""
     root_view = 'root' if root_view is None else root_view
-    root: Root = cast(Root, render_view(root_view, TkRenderingContext()))
+    rendering_context = TkRenderingContext({'node_globals': NodeGlobals(view_globals)} if view_globals else {})
+    root: Root = cast(Root, render_view(root_view, rendering_context))
     root.instance.mainloop()
```

### Comparing `tkviews-3.2.0/tkviews/canvas.py` & `tkviews-4.0.0/tkviews/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Wrappers for canvas elements"""
 
 from abc import ABC, abstractmethod
 from functools import partial
 from tkinter import Canvas
 from typing import Optional, cast
 
-from pyviews.core import XmlNode, InheritedDict, Node
+from pyviews.core.rendering import Node, NodeGlobals, RenderingError
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import apply_attributes
-from pyviews.rendering import RenderingPipeline, RenderingError, get_type
+from pyviews.rendering.pipeline import RenderingPipeline, get_type
 
 from tkviews.core.rendering import TkRenderingContext
 
 
 class CanvasItemNode(Node, ABC):
     """Base class for wrappers"""
 
-    def __init__(self, master: Canvas, xml_node: XmlNode,
-                 node_globals: Optional[InheritedDict] = None):
-        super().__init__(xml_node, node_globals=node_globals)
+    def __init__(self, master: Canvas, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(xml_node, node_globals = node_globals)
         self._canvas: Canvas = master
         self._item_id: Optional[int] = None
         self.place: list = []
 
     @property
     def item_id(self) -> Optional[int]:
         """id returned from create method of canvas"""
@@ -122,15 +122,15 @@
         setup_temp_binding,
         apply_attributes,
         create_item,
         setup_config_setter,
         setup_event_binding,
         apply_temp_events,
         clear_temp
-    ], create_node=create_canvas_node)
+    ], create_node=create_canvas_node) # yapf: disable
 
 
 def create_canvas_node(context: TkRenderingContext) -> Node:
     """Creates node_type instance"""
     node_type = get_type(context.xml_node)
     if not isinstance(context.master, Canvas):
         raise RenderingError(f'{node_type.__name__} parent should be Canvas')
@@ -150,15 +150,15 @@
         node.attr_values[key] = value
 
 
 def setup_temp_binding(node: CanvasItemNode, _: TkRenderingContext):
     """Stores event callbacks to temp dictionary"""
     node.events = {}
     node.bind_source = node.bind
-    node.bind = lambda event, command, n=node: _bind(n, event, command)
+    node.bind = lambda event, command, n = node: _bind(n, event, command)
 
 
 def _bind(node: CanvasItemNode, event, command):
     node.events[event] = command
 
 
 def create_item(node: CanvasItemNode, _: TkRenderingContext):
```

### Comparing `tkviews-3.2.0/tkviews/core/rendering.py` & `tkviews-4.0.0/tkviews/core/rendering.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Common rendering functionality"""
 
 from tkinter import Widget
-from typing import Tuple, Any
+from typing import Any, Tuple
 
-from pyviews.core import Node, XmlAttr, Setter, XmlNode, InheritedDict
-from pyviews.expression import is_expression, parse_expression, Expression, execute
+from pyviews.core.expression import Expression, execute, is_expression, parse_expression
+from pyviews.core.rendering import Node, NodeGlobals, RenderingContext, Setter, XmlNode
+from pyviews.core.xml import XmlAttr
 from pyviews.pipes import get_setter
-from pyviews.rendering import RenderingContext
 
 
 class TkRenderingContext(RenderingContext):
     """tkviews rendering context"""
 
     @property
     def master(self) -> Widget:
@@ -24,19 +24,19 @@
 
 def render_attribute(node: Node, xml_attr: XmlAttr) -> Tuple[Setter, Any]:
     """Returns setter and value"""
     setter = get_setter(xml_attr)
     value = xml_attr.value if xml_attr.value else ''
     if is_expression(value):
         expression_ = Expression(parse_expression(value)[1])
-        value = execute(expression_, node.node_globals.to_dictionary())
+        value = execute(expression_, node.node_globals)
     return setter, value
 
 
 def get_tk_child_context(child_xml_node: XmlNode, node: Node, context: TkRenderingContext) -> TkRenderingContext:
     """Return rendering context for child node"""
     return TkRenderingContext({
         'parent_node': node,
         'master': context.master,
-        'node_globals': InheritedDict(node.node_globals),
+        'node_globals': NodeGlobals(node.node_globals),
         'xml_node': child_xml_node
     })
```

### Comparing `tkviews-3.2.0/tkviews/listbox.py` & `tkviews-4.0.0/tkviews/listbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from tkinter import Listbox
 from typing import Callable, Optional
 
-from pyviews.core import Node, XmlNode, InheritedDict
+from pyviews.core.rendering import Node, NodeGlobals, RenderingError
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import apply_attributes
-from pyviews.rendering import RenderingPipeline, RenderingError
+from pyviews.rendering.pipeline import RenderingPipeline
 
 from tkviews.core import TkRenderingContext
 
 
 class ListboxItem(Node):
-    def __init__(self, xml_node: XmlNode,
-                 node_globals: Optional[InheritedDict] = None):
-        super().__init__(xml_node, node_globals=node_globals)
-        self.on_updated: Callable[[ListboxItem], None] = None
+
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(xml_node, node_globals = node_globals)
+        self.on_updated: Optional[Callable[[ListboxItem], None]] = None
         self._index: Optional[int] = None
         self._value: str = ''
 
     @property
     def index(self) -> Optional[int]:
         return self._index
 
@@ -40,15 +41,15 @@
 def get_listboxitem_pipeline() -> RenderingPipeline[ListboxItem, TkRenderingContext]:
     """Returns setup for canvas"""
     return RenderingPipeline[ListboxItem, TkRenderingContext](pipes=[
         apply_attributes,
         insert_item,
         setup_on_updated,
         setup_on_destroy
-    ])
+    ]) # yapf: disable
 
 
 def insert_item(node: ListboxItem, context: TkRenderingContext):
     if not isinstance(context.master, Listbox):
         raise RenderingError(f'{ListboxItem.__name__} parent should be Listbox')
     listbox: Listbox = context.master
     node.index = node.index if node.index else listbox.size()
```

### Comparing `tkviews-3.2.0/tkviews/styles.py` & `tkviews-4.0.0/tkviews/styles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Contains rendering steps for style nodes"""
 from tkinter import Widget
 from typing import Any, List, Optional
 
-from pyviews.core import PyViewsError, Setter, Node, XmlNode, InheritedDict, XmlAttr
-from pyviews.expression import parse_expression, is_expression, execute
-from pyviews.pipes import render_children, get_setter, apply_attributes
-from pyviews.rendering import RenderingPipeline
-
 from pyviews.containers import render_view_content
+from pyviews.core.error import PyViewsError
+from pyviews.core.expression import execute, is_expression, parse_expression
+from pyviews.core.rendering import Node, NodeGlobals, Setter
+from pyviews.core.xml import XmlAttr, XmlNode
+from pyviews.pipes import apply_attributes, get_setter, render_children
+from pyviews.rendering.pipeline import RenderingPipeline
 
 from tkviews.core import TkRenderingContext
 
 STYLES_KEY = '_node_styles'
 
 
 class StyleError(PyViewsError):
@@ -51,114 +52,115 @@
     def __eq__(self, other):
         return hash(self) == hash(other)
 
 
 class Style(Node):
     """Node for storing config options"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
         super().__init__(xml_node, node_globals)
         self.name: Optional[str] = None
         self.items = {}
 
 
 def get_style_pipeline() -> RenderingPipeline:
     """Returns pipeline for style node"""
     return RenderingPipeline(pipes=[
         setup_node_styles,
         apply_style_items,
         apply_parent_items,
         store_to_node_styles,
         render_child_styles
-    ], name='styles pipeline')
+    ], name='styles pipeline') # yapf: disable
 
 
 def setup_node_styles(_: Style, context: TkRenderingContext):
     """Initializes node styles"""
     if STYLES_KEY not in context.parent_node.node_globals:
-        context.parent_node.node_globals[STYLES_KEY] = InheritedDict()
+        context.parent_node.node_globals[STYLES_KEY] = NodeGlobals()
 
 
 def apply_style_items(node: Style, _: TkRenderingContext):
     """Parsing step. Parses attributes to style items and sets them to style"""
     attrs = node.xml_node.attrs
     try:
         node.name = next(attr.value for attr in attrs if attr.name == 'name')
     except StopIteration as error:
         raise StyleError('Style name is missing', node.xml_node.view_info) from error
-    node.items = {
-        f'{attr.namespace}{attr.name}':
-            _get_style_item(node, attr) for attr in attrs if attr.name != 'name'
-    }
+    node.items = {f'{attr.namespace}{attr.name}': _get_style_item(node, attr) for attr in attrs if attr.name != 'name'}
 
 
 def _get_style_item(node: Style, attr: XmlAttr):
     setter = get_setter(attr)
     value = attr.value if attr.value else ''
     if is_expression(value):
         expression_body = parse_expression(value).body
-        value = execute(expression_body, node.node_globals.to_dictionary())
+        value = execute(expression_body, node.node_globals)
     return StyleItem(setter, attr.name, value)
 
 
 def apply_parent_items(node: Style, context: TkRenderingContext):
     """Sets style items from parent style"""
     if isinstance(context.parent_node, Style):
         node.items = {**context.parent_node.items, **node.items}
 
 
 def store_to_node_styles(node: Style, context: TkRenderingContext):
     """Store styles to node styles"""
     _get_styles(context)[node.name] = node.items.values()
 
 
-def _get_styles(context: TkRenderingContext) -> InheritedDict:
+def _get_styles(context: TkRenderingContext) -> NodeGlobals:
     return context.parent_node.node_globals[STYLES_KEY]
 
 
 def render_child_styles(node: Style, context: TkRenderingContext):
     """Renders child styles"""
-    render_children(node, context, lambda x, n, _: TkRenderingContext({
-        'parent_node': n,
-        'node_globals': InheritedDict(node.node_globals),
-        'node_styles': _get_styles(context),
-        'xml_node': x
-    }))
+    render_children(
+        node,
+        context,
+        lambda x,
+        n,
+        _: TkRenderingContext({
+            'parent_node': n,
+            'node_globals': NodeGlobals(node.node_globals),
+            'node_styles': _get_styles(context),
+            'xml_node': x
+        })
+    )
 
 
 class StylesView(Node):
     """Loads styles from separate file"""
 
-    def __init__(self, master: Widget, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
-        super().__init__(xml_node, node_globals=node_globals)
+    def __init__(self, master: Widget, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(xml_node, node_globals = node_globals)
         self.name = None
         self.master = master
 
     def set_content(self, content: Node):
         """Destroys current """
         self._children = [content]
 
 
 def get_styles_view_pipeline() -> RenderingPipeline:
     """Returns setup for container"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_view_content,
-        store_to_globals
-    ], name='styles view pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, render_view_content, store_to_globals], name = 'styles view pipeline'
+    )
 
 
 def store_to_globals(view: StylesView, context: TkRenderingContext):
     """Stores styles to parent node globals"""
     child: Node = view.children[0]
-    styles: InheritedDict = child.node_globals[STYLES_KEY]
+    styles: NodeGlobals = child.node_globals[STYLES_KEY]
     if STYLES_KEY in context.parent_node.node_globals:
         parent_styles = context.parent_node.node_globals[STYLES_KEY]
-        merged_styles = {**parent_styles.to_dictionary(), **styles.to_dictionary()}
-        styles = InheritedDict(merged_styles)
+        merged_styles = {**parent_styles, **styles}
+        styles = NodeGlobals(merged_styles)
     context.parent_node.node_globals[STYLES_KEY] = styles
 
 
 def apply_styles(node: Node, _: str, keys: List[str]):
     """Applies styles to node"""
     if isinstance(keys, str):
         keys = [key.strip() for key in keys.split(',') if key]
```

### Comparing `tkviews-3.2.0/tkviews/widgets/binding.py` & `tkviews-4.0.0/tkviews/widgets/binding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Widgets binding"""
 
-from tkinter import Widget, Variable, Entry, Checkbutton, Radiobutton, StringVar, BooleanVar, \
-    IntVar, DoubleVar, Scale, Spinbox
+from tkinter import (BooleanVar, Checkbutton, DoubleVar, Entry, IntVar, Radiobutton, Scale, Spinbox, StringVar,
+                     Variable, Widget)
 from typing import Type, Union
 
-from injectool import inject
-from pyviews.binding import BindingContext, TwoWaysBinding, ExpressionBinding, Binder, \
-    get_expression_callback
-from pyviews.core import BindingCallback, Binding, \
-    BindingError, PyViewsError
-from pyviews.core import error_handling
-from pyviews.expression import Expression, execute
+from injectool import In, inject
+from pyviews.binding.binder import Binder, BindingContext
+from pyviews.binding.expression import ExpressionBinding, get_expression_callback
+from pyviews.binding.twoways import TwoWaysBinding
+from pyviews.core.binding import Binding, BindingCallback, BindingError
+from pyviews.core.error import PyViewsError, error_handling
+from pyviews.core.expression import Expression, execute
 
 
 class VariableBinding(Binding):
     """Binding is subscribed on tkinter Var changes"""
 
     def __init__(self, callback: BindingCallback, var: Variable):
         super().__init__()
@@ -40,59 +40,72 @@
     def destroy(self):
         """Destroys binding"""
         if self._trace_id:
             self._var.trace_remove('write', self._trace_id)
         self._trace_id = None
 
 
-@inject(binder=Binder)
-def use_variables_binding(binder: Binder = None):
+@inject(binder = Binder)
+def use_variables_binding(binder: Binder = In):
     """Adds tkinter variables bindings"""
-    binder.add_rule('twoways', lambda ctx: bind_variable_and_expression(StringVar, ctx),
-                    lambda ctx: check_widget_and_property(Entry, 'textvariable', ctx))
-    binder.add_rule('twoways', lambda ctx: bind_variable_and_expression(BooleanVar, ctx),
-                    lambda ctx: check_widget_and_property(Checkbutton, 'variable', ctx))
-    binder.add_rule('twoways', lambda ctx: bind_variable_and_expression(IntVar, ctx),
-                    lambda ctx: check_widget_and_property(Radiobutton, 'variable', ctx))
-    binder.add_rule('twoways', lambda ctx: bind_variable_and_expression(DoubleVar, ctx),
-                    lambda ctx: check_widget_and_property(Scale, 'variable', ctx))
-    binder.add_rule('twoways', lambda ctx: bind_variable_and_expression(StringVar, ctx),
-                    lambda ctx: check_widget_and_property(Spinbox, 'textvariable', ctx))
+    binder.add_rule(
+        'twoways',
+        lambda ctx: bind_variable_and_expression(StringVar, ctx),
+        lambda ctx: check_widget_and_property(Entry, 'textvariable', ctx)
+    )
+    binder.add_rule(
+        'twoways',
+        lambda ctx: bind_variable_and_expression(BooleanVar, ctx),
+        lambda ctx: check_widget_and_property(Checkbutton, 'variable', ctx)
+    )
+    binder.add_rule(
+        'twoways',
+        lambda ctx: bind_variable_and_expression(IntVar, ctx),
+        lambda ctx: check_widget_and_property(Radiobutton, 'variable', ctx)
+    )
+    binder.add_rule(
+        'twoways',
+        lambda ctx: bind_variable_and_expression(DoubleVar, ctx),
+        lambda ctx: check_widget_and_property(Scale, 'variable', ctx)
+    )
+    binder.add_rule(
+        'twoways',
+        lambda ctx: bind_variable_and_expression(StringVar, ctx),
+        lambda ctx: check_widget_and_property(Spinbox, 'textvariable', ctx)
+    )
     binder.add_rule('var', bind_custom_variable_and_expression)
 
 
-def bind_variable_and_expression(variable: Union[Variable, Type[Variable]],
-                                 context: BindingContext) -> TwoWaysBinding:
+def bind_variable_and_expression(variable: Union[Variable, Type[Variable]], context: BindingContext) -> TwoWaysBinding:
     """Create two ways binding between variable and expression"""
     if isinstance(variable, type):
         variable = variable()
     context.setter(context.node, context.xml_attr.name, variable)
     property_expression = Expression(context.expression_body)
 
     expr_binding = ExpressionBinding(variable.set, property_expression, context.node.node_globals)
     expression_callback = get_expression_callback(property_expression, context.node.node_globals)
     var_binding = VariableBinding(expression_callback, variable)
     two_ways_binding = TwoWaysBinding(expr_binding, var_binding)
     two_ways_binding.bind()
     return two_ways_binding
 
 
-def check_widget_and_property(widget_type: Type[Widget], var_property: str,
-                              context: BindingContext) -> bool:
+def check_widget_and_property(widget_type: Type[Widget], var_property: str, context: BindingContext) -> bool:
     """Return true if type and property are matched with values from context"""
     try:
         return isinstance(context.node.instance, widget_type) \
                and context.xml_attr.name == var_property
     except AttributeError:
         return False
 
 
 def bind_custom_variable_and_expression(context: BindingContext) -> TwoWaysBinding:
     """
     Create two ways binding between variable and expression.
     Expression should be "[binding type]:{[variable to bind]}:{[expression to bind]}"
     """
     (var_body, value_body) = context.expression_body.split('}:{')
-    variable: Variable = execute(Expression(var_body), context.node.node_globals.to_dictionary())
+    variable: Variable = execute(Expression(var_body), context.node.node_globals)
     custom_context = BindingContext(context)
     custom_context.expression_body = value_body
     return bind_variable_and_expression(variable, custom_context)
```

### Comparing `tkviews-3.2.0/tkviews/widgets/node.py` & `tkviews-4.0.0/tkviews/widgets/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Tkinter widgets nodes"""
 from functools import partial
-from tkinter import Tk, Widget, PanedWindow
+from tkinter import PanedWindow, Tk, Widget
+from typing import Optional
 
-from pyviews.core import XmlNode, InstanceNode, InheritedDict, XmlAttr
-from pyviews.pipes import apply_attributes, render_children, apply_attribute
-from pyviews.rendering import RenderingPipeline, get_type, create_instance
+from pyviews.core.rendering import InstanceNode, NodeGlobals
+from pyviews.core.xml import XmlAttr, XmlNode
+from pyviews.pipes import apply_attribute, apply_attributes, render_children
+from pyviews.rendering.pipeline import RenderingPipeline, create_instance, get_type
 
 from tkviews.core import TkRenderingContext
 
 
 class Root(InstanceNode):
     """Wrapper under tkinter Root"""
 
-    def __init__(self, xml_node: XmlNode):
-        super().__init__(Tk(), xml_node)
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(Tk(), xml_node, node_globals)
         self._icon = None
 
     @property
     def state(self):
         """Widget state"""
         return self.instance.state()
 
@@ -29,15 +31,15 @@
     def icon(self):
         """Icon path"""
         return self._icon
 
     @icon.setter
     def icon(self, value):
         self._icon = value
-        self.instance.iconbitmap(default=value)
+        self.instance.iconbitmap(default = value)
 
     def bind(self, event, command):
         """Calls widget bind"""
         self.instance.bind(event, command)
 
     def bind_all(self, event, command):
         """Calls widget bind"""
@@ -47,23 +49,22 @@
 def get_root_pipeline() -> RenderingPipeline:
     """Returns setup for root"""
     return RenderingPipeline(pipes=[
         setup_widget_setter,
         setup_widget_destroy,
         apply_attributes,
         render_widget_children
-    ], name='root pipeline')
+    ], name='root pipeline') # yapf: disable
 
 
 class WidgetNode(InstanceNode):
     """Wrapper under tkinter widget"""
 
-    def __init__(self, widget: Widget, xml_node: XmlNode,
-                 node_globals: InheritedDict = None):
-        super().__init__(widget, xml_node, node_globals=node_globals)
+    def __init__(self, widget: Widget, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(widget, xml_node, node_globals = node_globals)
 
     def bind(self, event, command):
         """Calls widget bind"""
         self.instance.bind(event, command)
 
     def bind_all(self, event, command):
         """Calls widget bind"""
@@ -75,15 +76,15 @@
     return RenderingPipeline(pipes=[
         setup_widget_setter,
         setup_widget_destroy,
         apply_attributes,
         apply_text,
         add_to_panedwindow,
         render_widget_children
-    ], create_node=_create_widget_node, name='widget pipeline')
+    ], create_node=_create_widget_node, name='widget pipeline') # yapf: disable
 
 
 def setup_widget_setter(node: WidgetNode, _: TkRenderingContext):
     """Sets up setter"""
     node.set_attr = partial(_widget_node_setter, node)
 
 
@@ -115,15 +116,15 @@
 
 def _get_child_context(xml_node: XmlNode, node: WidgetNode, _: TkRenderingContext):
     """Renders child widgets"""
     child_context = TkRenderingContext()
     child_context.xml_node = xml_node
     child_context.parent_node = node
     child_context.master = node.instance
-    child_context.node_globals = InheritedDict(node.node_globals)
+    child_context.node_globals = NodeGlobals(node.node_globals)
     return child_context
 
 
 def _create_widget_node(context: TkRenderingContext):
     inst_type = get_type(context.xml_node)
     inst = create_instance(inst_type, context)
     return create_instance(WidgetNode, {'widget': inst, **context})
```

### Comparing `tkviews-3.2.0/tkviews/widgets/setters.py` & `tkviews-4.0.0/tkviews/widgets/setters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Common setters for widgets nodes"""
 
 from tkinter import Event
 
-from pyviews.core import PyViewsError
-from pyviews.core import error_handling, ViewInfo
+from pyviews.core.error import PyViewsError, ViewInfo, error_handling
 
 from tkviews.widgets.node import WidgetNode
 
 
 class CallbackError(PyViewsError):
     """Error from callback"""
```

### Comparing `tkviews-3.2.0/tkviews/widgets/ttk.py` & `tkviews-4.0.0/tkviews/widgets/ttk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """ttk specific implementation"""
 from functools import partial
 from tkinter.ttk import Style
 from typing import Any
+from pyviews.core.error import Optional
+
+from pyviews.core.rendering import Node, NodeGlobals, XmlNode
+from pyviews.rendering.pipeline import RenderingPipeline
 
-from pyviews.core import XmlNode, Node, InheritedDict
-from pyviews.rendering import RenderingPipeline
 
 from tkviews.core.rendering import TkRenderingContext, render_attribute
 
 
 class TtkStyle(Node):
     """Node for tkk style"""
 
-    def __init__(self, xml_node: XmlNode, parent_name=None, node_globals: InheritedDict = None):
+    def __init__(self, xml_node: XmlNode, parent_name=None, node_globals: Optional[NodeGlobals] = None):
         super().__init__(xml_node, node_globals=node_globals)
         self.values = {}
         self._parent_name = parent_name
         self.name = None
 
     @property
     def full_name(self):
```

### Comparing `tkviews-3.2.0/tkviews.egg-info/PKG-INFO` & `tkviews-4.0.0/tkviews.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkviews
-Version: 3.2.0
+Version: 4.0.0
 Summary: Package for creating tkinter applications in declarative way.
 Project-URL: Homepage, https://github.com/eumis/tkviews
 Keywords: binding,tkinter,tk,tkviews,pyviews,python,mvvm,views
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
@@ -52,12 +52,16 @@
 To run demo app execute following commands
 
 ```
 cd [root_folder]\demo
 python run.py
 ```
 
+## Docs
+
+See some documentation in [docs](https://github.com/eumis/tkviews/tree/dev/docs) folder
+
 ## License
 
 [MIT](http://opensource.org/licenses/MIT)
 
 Copyright (c) 2017-present, eumis (Eugen Misievich)
```

