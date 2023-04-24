# Comparing `tmp/wxviews-0.7.0.tar.gz` & `tmp/wxviews-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxviews-0.7.0.tar", last modified: Tue Nov 22 14:14:49 2022, max compression
+gzip compressed data, was "wxviews-0.8.0.tar", last modified: Mon Apr 24 12:18:30 2023, max compression
```

## Comparing `wxviews-0.7.0.tar` & `wxviews-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:14:49.015059 wxviews-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2022-11-22 14:13:06.000000 wxviews-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2368 2022-11-22 14:14:49.015059 wxviews-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2022-11-22 14:13:06.000000 wxviews-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2022-11-22 14:13:06.000000 wxviews-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 14:14:49.015059 wxviews-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-22 14:13:06.000000 wxviews-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:14:49.011059 wxviews-0.7.0/wxviews/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:14:49.011059 wxviews-0.7.0/wxviews/core/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      526 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/core/node.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/core/pipes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/core/rendering.py
--rw-r--r--   0 runner    (1001) docker     (122)    10102 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/inspection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3317 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/menus.py
--rw-r--r--   0 runner    (1001) docker     (122)     5058 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/sizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5305 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:14:49.015059 wxviews-0.7.0/wxviews/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3807 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/widgets/binding.py
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/widgets/rendering.py
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2022-11-22 14:13:06.000000 wxviews-0.7.0/wxviews/widgets/setters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 14:14:49.011059 wxviews-0.7.0/wxviews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2368 2022-11-22 14:14:49.000000 wxviews-0.7.0/wxviews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      532 2022-11-22 14:14:49.000000 wxviews-0.7.0/wxviews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 14:14:49.000000 wxviews-0.7.0/wxviews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-11-22 14:14:49.000000 wxviews-0.7.0/wxviews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-22 14:14:49.000000 wxviews-0.7.0/wxviews.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:18:30.889454 wxviews-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 12:16:53.000000 wxviews-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-24 12:18:30.889454 wxviews-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-24 12:16:53.000000 wxviews-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-24 12:16:53.000000 wxviews-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:18:30.889454 wxviews-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 12:16:53.000000 wxviews-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:18:30.885453 wxviews-0.8.0/wxviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:18:30.889454 wxviews-0.8.0/wxviews/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/core/pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/core/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/sizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:18:30.889454 wxviews-0.8.0/wxviews/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/widgets/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/widgets/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-24 12:16:53.000000 wxviews-0.8.0/wxviews/widgets/setters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:18:30.889454 wxviews-0.8.0/wxviews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-24 12:18:30.000000 wxviews-0.8.0/wxviews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-24 12:18:30.000000 wxviews-0.8.0/wxviews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:18:30.000000 wxviews-0.8.0/wxviews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 12:18:30.000000 wxviews-0.8.0/wxviews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 12:18:30.000000 wxviews-0.8.0/wxviews.egg-info/top_level.txt
```

### Comparing `wxviews-0.7.0/LICENSE` & `wxviews-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wxviews-0.7.0/PKG-INFO` & `wxviews-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxviews
-Version: 0.7.0
+Version: 0.8.0
 Summary: Package for creating wx applications in declarative way.
 Project-URL: Homepage, https://github.com/eumis/wxviews
 Keywords: binding,wxviews,wxpython,pyviews,python,mvvm,wx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wxviews-0.7.0/README.md` & `wxviews-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `wxviews-0.7.0/wxviews/app.py` & `wxviews-0.8.0/wxviews/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """wxviews application entry point"""
 
 from typing import cast
 
 from injectool import add_singleton
-from pyviews.binding import use_binding
+from pyviews.binding.config import use_binding
 from pyviews.code import run_code
 from pyviews.presenter import get_presenter_pipeline
-from pyviews.rendering import RenderingPipeline, use_rendering, get_child_context
-from pyviews.rendering.pipeline import use_pipeline
-from pyviews.rendering.views import render_view
-
-from wxviews.containers import get_if_pipeline, get_for_pipeline
-from wxviews.containers import get_view_pipeline, get_container_pipeline
-from wxviews.core import WxRenderingContext
-from wxviews.core.rendering import get_wx_child_context
-from wxviews.menus import get_menu_item_pipeline, get_menu_pipeline, get_menu_bar_pipeline
+from pyviews.rendering.context import get_child_context
+from pyviews.rendering.pipeline import RenderingPipeline, render_view, use_pipeline
+from pyviews.rendering.config import use_rendering
+
+from wxviews.containers import get_container_pipeline, get_for_pipeline, get_if_pipeline, get_view_pipeline
+from wxviews.core.rendering import WxRenderingContext, get_wx_child_context
+from wxviews.menus import get_menu_bar_pipeline, get_menu_item_pipeline, get_menu_pipeline
 from wxviews.sizers import get_growable_col_pipeline, get_growable_row_pipeline, get_sizer_pipeline
-from wxviews.styles import get_styles_view_pipeline, get_style_pipeline
-from wxviews.widgets import get_frame_pipeline, get_app_pipeline, get_wx_pipeline, WxNode
+from wxviews.styles import get_style_pipeline, get_styles_view_pipeline
 from wxviews.widgets.binding import use_events_binding
+from wxviews.widgets.rendering import WxNode, get_app_pipeline, get_frame_pipeline, get_wx_pipeline
 
 
 def register_dependencies():
     """Registers all dependencies needed for application"""
     use_rendering()
     use_binding()
     use_events_binding()
@@ -52,17 +50,17 @@
 
     use_pipeline(get_menu_bar_pipeline(), 'wx.MenuBar')
     use_pipeline(get_menu_pipeline(), 'wx.Menu')
     use_pipeline(get_menu_item_pipeline(), 'wx.MenuItem')
 
     use_pipeline(get_style_pipeline(), 'wxviews.Style')
     use_pipeline(get_styles_view_pipeline(), 'wxviews.StylesView')
-    use_pipeline(RenderingPipeline(pipes=[run_code]), 'wxviews.Code')
+    use_pipeline(RenderingPipeline(pipes = [run_code]), 'wxviews.Code')
 
     use_pipeline(get_presenter_pipeline(), 'wxviews.PresenterNode')
 
 
-def launch(context: WxRenderingContext, root_view=None):
+def launch(context: WxRenderingContext, root_view = None):
     """Runs application. Widgets are created from passed xml_files"""
     root_view = 'root' if root_view is None else root_view
     root = cast(WxNode, render_view(root_view, context))
     root.instance.MainLoop()
```

### Comparing `wxviews-0.7.0/wxviews/containers.py` & `wxviews-0.8.0/wxviews/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """Contains methods for node setups creation"""
 from functools import partial
 
-from pyviews.containers import render_container_children, render_view_content, \
-    rerender_on_view_change, render_for_items, rerender_on_items_change, render_if, \
-    rerender_on_condition_change
-from pyviews.core import Observable
-from pyviews.rendering import RenderingPipeline
+from pyviews.containers import (render_container_children, render_for_items, render_if, render_view_content,
+                                rerender_on_condition_change, rerender_on_items_change, rerender_on_view_change)
+from pyviews.core.binding import Bindable
+from pyviews.rendering.pipeline import RenderingPipeline
 
-from wxviews.core import WxRenderingContext, apply_attributes
+from wxviews.core.pipes import apply_attributes
+from wxviews.core.rendering import WxRenderingContext
 
 
-def layout_parent_on_change(changed_property: str, container: Observable,
-                            context: WxRenderingContext):
+def layout_parent_on_change(changed_property: str, container: Bindable, context: WxRenderingContext):
     """Call parent.Layout() on property change"""
     if context.parent:
         container.observe(changed_property, lambda _, __: context.parent.Layout())
 
 
 def get_container_pipeline() -> RenderingPipeline:
     """Returns setup for container"""
     return RenderingPipeline(pipes=[
         apply_attributes,
         render_container_children
-    ], name='container pipeline')
+    ], name='container pipeline') # yapf: disable
 
 
 def get_view_pipeline() -> RenderingPipeline:
     """Returns setup for container"""
     return RenderingPipeline(pipes=[
         apply_attributes,
         render_view_content,
         rerender_on_view_change,
         partial(layout_parent_on_change, 'name')
-    ], name='view pipeline')
+    ], name='view pipeline') # yapf: disable
 
 
 def get_for_pipeline() -> RenderingPipeline:
     """Returns setup for For node"""
     return RenderingPipeline(pipes=[
         apply_attributes,
         render_for_items,
         rerender_on_items_change,
         partial(layout_parent_on_change, 'items')
-    ], name='for pipeline')
+    ], name='for pipeline') # yapf: disable
 
 
 def get_if_pipeline() -> RenderingPipeline:
     """Returns setup for For node"""
     return RenderingPipeline(pipes=[
         apply_attributes,
         render_if,
         rerender_on_condition_change,
         partial(layout_parent_on_change, 'condition')
-    ], name='if pipeline')
+    ], name='if pipeline') # yapf: disable
```

### Comparing `wxviews-0.7.0/wxviews/core/node.py` & `wxviews-0.8.0/wxviews/core/node.py`

 * *Files identical despite different names*

### Comparing `wxviews-0.7.0/wxviews/core/pipes.py` & `wxviews-0.8.0/wxviews/core/pipes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Common pipeline functionality"""
 
-from pyviews.core import Node
+from pyviews.core.rendering import Node
 from pyviews.pipes import apply_attribute
 
-from .node import Sizerable
-from .rendering import WxRenderingContext
+from wxviews.core.node import Sizerable
+from wxviews.core.rendering import WxRenderingContext
 
 
 def apply_attributes(node: Node, _: WxRenderingContext):
     """Applies attributes for node"""
     attrs = [attr for attr in node.xml_node.attrs if attr.namespace not in ['init']]
     for attr in attrs:
         apply_attribute(node, attr)
```

### Comparing `wxviews-0.7.0/wxviews/core/rendering.py` & `wxviews-0.8.0/wxviews/core/rendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Common"""
 
 from typing import Any, Optional
 
-from pyviews.core import InheritedDict, XmlAttr, XmlNode, Node
-from pyviews.expression import is_expression, parse_expression, execute
-from pyviews.rendering.common import RenderingContext
+from pyviews.core.expression import execute, is_expression, parse_expression
+from pyviews.core.rendering import NodeGlobals
+from pyviews.core.xml import XmlAttr, XmlNode
+from pyviews.rendering.context import Node, RenderingContext
 from wx import Sizer
 
 
 class WxRenderingContext(RenderingContext):
     """wxviews rendering context"""
 
     @property
@@ -26,49 +27,48 @@
         return self.get('sizer')
 
     @sizer.setter
     def sizer(self, value: Sizer):
         self['sizer'] = value
 
     @property
-    def node_styles(self) -> InheritedDict:
+    def node_styles(self) -> NodeGlobals:
         """Node styles"""
         return self.get('node_styles')
 
     @node_styles.setter
-    def node_styles(self, value: InheritedDict):
+    def node_styles(self, value: NodeGlobals):
         self['node_styles'] = value
 
 
-def get_attr_args(xml_node, namespace: str, node_globals: Optional[InheritedDict] = None) -> dict:
+def get_attr_args(xml_node, namespace: str, node_globals: Optional[NodeGlobals] = None) -> dict:
     """Returns args from attributes with provided namespace"""
     init_attrs = [attr for attr in xml_node.attrs if attr.namespace == namespace]
     args = {}
     for attr in init_attrs:
         value = get_init_value(attr, node_globals)
         if attr.name == '':
             args = {**args, **value}
         else:
             args[attr.name] = value
     return args
 
 
-def get_init_value(attr: XmlAttr, node_globals: Optional[InheritedDict]) -> Any:
+def get_init_value(attr: XmlAttr, node_globals: Optional[NodeGlobals]) -> Any:
     """Evaluates attribute value and returns it"""
     stripped_value = attr.value.strip() if attr.value else ''
     if is_expression(stripped_value):
         body = parse_expression(stripped_value)[1]
-        parameters = node_globals.to_dictionary() if node_globals else {}
+        parameters = node_globals if node_globals else {}
         return execute(body, parameters)
     return attr.value
 
 
-def get_wx_child_context(xml_node: XmlNode, parent_node: Node,
-                         context: WxRenderingContext) -> WxRenderingContext:
+def get_wx_child_context(xml_node: XmlNode, parent_node: Node, context: WxRenderingContext) -> WxRenderingContext:
     """Return child node context"""
     return WxRenderingContext({
         'parent_node': parent_node,
         'parent': context.parent,
-        'node_globals': InheritedDict(parent_node.node_globals),
+        'node_globals': NodeGlobals(parent_node.node_globals),
         'sizer': context.sizer,
         'xml_node': xml_node
     })
```

### Comparing `wxviews-0.7.0/wxviews/inspection.py` & `wxviews-0.8.0/wxviews/inspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,90 +1,38 @@
 """Extension of wxpython InspectionTool to show view nodes"""
 
-from os import linesep
 import inspect
+from os import linesep
 from traceback import format_exc
-from typing import Any, Optional, Union, List
+from typing import Any, List, Optional, Union
 from unittest.mock import patch
 
-from pyviews.binding import ExpressionBinding, ObservableBinding, TwoWaysBinding
-from pyviews.core import Node, InstanceNode
 import wx
-from wx import Point, DefaultPosition, Size, MenuBar
-from wx import Menu, MenuItem, Window, Sizer, SizerItem
+from pyviews.binding.expression import ExpressionBinding
+from pyviews.binding.observable import ObservableBinding
+from pyviews.binding.twoways import TwoWaysBinding
+from pyviews.core.rendering import InstanceNode, Node
+from wx import DefaultPosition, Menu, MenuBar, MenuItem, Point, Size, Sizer, SizerItem, Window
 from wx.lib import inspection
 from wx.lib.agw.customtreectrl import GenericTreeItem
-from wx.lib.inspection import InspectionTree, InspectionFrame, InspectionInfoPanel
-
-from wxviews.widgets import WxNode, get_root, EventBinding
-
-
-class ViewInspectionTool:
-    """
-    The :class:`ViewInspectionTool` is a singleton that manages creating and
-    showing an :class:`ViewInspectionFrame`.
-    """
-
-    def __init__(self, pos: Point = DefaultPosition, size: Size = Size(850, 700),
-                 config=None, crust_locals: Optional[dict] = None):
-        self._frame: Optional[ViewInspectionFrame] = None
-        self._pos: Point = pos
-        self._size: Size = size
-        self._config = config
-        self._crust_locals: Optional[dict] = crust_locals
-        if not hasattr(self, '_app'):
-            self._app: WxNode = get_root()
-
-    def show(self, select_obj: Any = None):
-        """
-        Creates the inspection frame if it hasn't been already, and
-        raises it if neccessary.
+from wx.lib.inspection import InspectionFrame, InspectionInfoPanel, InspectionTree
 
-        :param select_obj: Pass a widget or sizer to have that object be
-                     preselected in widget tree.
-        """
-        if not self._frame:
-            self._frame = ViewInspectionFrame(parent=self._app.instance.GetTopWindow(),
-                                              pos=self._pos,
-                                              size=self._size,
-                                              config=self._config,
-                                              locals=self._crust_locals,
-                                              app=self._app.instance,
-                                              root=self._app)
-        self._frame.SetObj(select_obj if select_obj else self._app)
-        self._frame.Show()
-        if self._frame.IsIconized():
-            self._frame.Iconize(False)
-        self._frame.Raise()
-
-
-class ViewInspectionFrame(InspectionFrame):
-    """
-    This class is the frame that holds the wxPython inspection tools.
-    The toolbar and AUI splitters/floating panes are also managed
-    here.  The contents of the tool windows are handled by other
-    classes.
-    """
-
-    def __init__(self, *args, root=None, **kwargs):
-        with patch(f'{inspection.__name__}.{InspectionTree.__name__}', ViewInspectionTree),\
-         patch(f'{inspection.__name__}.{InspectionInfoPanel.__name__}', ViewInspectionInfoPanel):
-            InspectionFrame.__init__(self, *args, **kwargs)
-            self.locals['root'] = root
+from wxviews.widgets.binding import EventBinding
+from wxviews.widgets.rendering import WxNode, get_root
 
 
 class ViewInspectionTree(InspectionTree):
     """Extends wx.lib.inspection.InspectionTree to show view nodes"""
 
-    def BuildTree(self, startWidget, includeSizers=False, expandFrame=False):
+    def BuildTree(self, startWidget, includeSizers = False, expandFrame = False):
         """setup root"""
         if isinstance(startWidget, Node):
             self.build_node_tree(startWidget)
         else:
-            super().BuildTree(startWidget, includeSizers=includeSizers, expandFrame=expandFrame)
+            super().BuildTree(startWidget, includeSizers = includeSizers, expandFrame = expandFrame)
 
     def build_node_tree(self, start_node: Node):
         """setup root"""
         if self.GetCount():
             self.DeleteAllItems()
             self.roots = []
             self.built = False
@@ -104,17 +52,15 @@
     def _get_node_name(self, node: Union[Node, InstanceNode]):
         node_name = node.__class__.__name__
         try:
             return f'{self.GetTextForWidget(node.instance)}[{node_name}]'
         except AttributeError:
             return node_name
 
-    def add_node(self,
-                 parent_item: GenericTreeItem,
-                 node: Union[Node, InstanceNode]) -> GenericTreeItem:
+    def add_node(self, parent_item: GenericTreeItem, node: Union[Node, InstanceNode]) -> GenericTreeItem:
         """Adds node item"""
         text = self._get_node_name(node)
         item = self.AppendItem(parent_item, text)
         self.SetItemData(item, node)
 
         for child in node.children:
             self.add_node(item, child)
@@ -193,15 +139,15 @@
             "Node:",
             self.Fmt('class', obj.__class__),
             self.Fmt('bases', obj.__class__.__bases__),
             self.Fmt('module', inspect.getmodule(obj)),
             "node_globals:"
         ]
 
-        for key, value in obj.node_globals.to_dictionary().items():
+        for key, value in obj.node_globals.items():
             lines.append(self.Fmt(key, value))
 
         if obj._bindings:
             lines.append("binding:")
             for binding in obj._bindings:
                 self._get_binding(binding, lines)
 
@@ -254,21 +200,83 @@
         """Formats Menu info"""
         lines = [
             "Menu:",
             self.Fmt('class', obj.__class__),
             self.Fmt('bases', obj.__class__.__bases__),
             self.Fmt('module', inspect.getmodule(obj)),
             self.Fmt('style', obj.GetStyle()),
-            self.Fmt('title', obj.GetTitle())]
+            self.Fmt('title', obj.GetTitle())
+        ]
         return lines
 
     def format_menu_item(self, obj: MenuItem):
         """Formats MenuItem info"""
         lines = [
             "MenuItem:",
             self.Fmt('class', obj.__class__),
             self.Fmt('bases', obj.__class__.__bases__),
             self.Fmt('module', inspect.getmodule(obj)),
             self.Fmt('id', obj.GetId()),
             self.Fmt('label', obj.GetLabel()),
-            self.Fmt('kind', obj.GetKind())]
+            self.Fmt('kind', obj.GetKind())
+        ]
         return lines
+
+
+class ViewInspectionTool:
+    """
+    The :class:`ViewInspectionTool` is a singleton that manages creating and
+    showing an :class:`ViewInspectionFrame`.
+    """
+
+    def __init__(
+        self,
+        pos: Point = DefaultPosition,
+        size: Size = Size(850, 700),
+        config = None,
+        crust_locals: Optional[dict] = None
+    ):
+        self._frame: Optional[ViewInspectionFrame] = None
+        self._pos: Point = pos
+        self._size: Size = size
+        self._config = config
+        self._crust_locals: Optional[dict] = crust_locals
+        if not hasattr(self, '_app'):
+            self._app: WxNode = get_root()
+
+    def show(self, select_obj: Any = None):
+        """
+        Creates the inspection frame if it hasn't been already, and
+        raises it if neccessary.
+        :param select_obj: Pass a widget or sizer to have that object be
+                     preselected in widget tree.
+        """
+        if not self._frame:
+            self._frame = ViewInspectionFrame(
+                parent = self._app.instance.GetTopWindow(),
+                pos = self._pos,
+                size = self._size,
+                config = self._config,
+                locals = self._crust_locals,
+                app = self._app.instance,
+                root = self._app
+            )
+        self._frame.SetObj(select_obj if select_obj else self._app)
+        self._frame.Show()
+        if self._frame.IsIconized():
+            self._frame.Iconize(False)
+        self._frame.Raise()
+
+
+class ViewInspectionFrame(InspectionFrame):
+    """
+    This class is the frame that holds the wxPython inspection tools.
+    The toolbar and AUI splitters/floating panes are also managed
+    here.  The contents of the tool windows are handled by other
+    classes.
+    """
+
+    def __init__(self, *args, root = None, **kwargs):
+        with patch(f'{inspection.__name__}.{InspectionTree.__name__}', ViewInspectionTree),\
+         patch(f'{inspection.__name__}.{InspectionInfoPanel.__name__}', ViewInspectionInfoPanel):
+            InspectionFrame.__init__(self, *args, **kwargs)
+            self.locals['root'] = root
```

### Comparing `wxviews-0.7.0/wxviews/menus.py` & `wxviews-0.8.0/wxviews/menus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 """Rendering pipeline for menus"""
 
-from pyviews.core import InstanceNode, InheritedDict, XmlNode
+from pyviews.core.rendering import InstanceNode, NodeGlobals
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import render_children
-from pyviews.rendering import RenderingPipeline, get_type
-from wx import Frame, MenuBar, Menu
+from pyviews.rendering.pipeline import RenderingPipeline, get_type
+from wx import Frame, Menu, MenuBar
 
-from wxviews.core import WxRenderingContext, apply_attributes, \
-    get_attr_args, get_init_value
-from wxviews.widgets import WxNode
+from wxviews.core.pipes import apply_attributes
+from wxviews.core.rendering import WxRenderingContext, get_attr_args, get_init_value
+from wxviews.widgets.rendering import WxNode
 
 
 def create_menu_node(context: WxRenderingContext) -> WxNode:
     """Creates node from xml node using namespace as module and tag name as class name"""
     inst_type = get_type(context.xml_node)
     args = get_attr_args(context.xml_node, 'init', context.node_globals)
     inst = inst_type(**args)
-    return WxNode(inst, context.xml_node, node_globals=context.node_globals)
+    return WxNode(inst, context.xml_node, node_globals = context.node_globals)
 
 
 def get_menu_bar_pipeline() -> RenderingPipeline[WxNode, WxRenderingContext]:
     """Return render pipeline for MenuBar"""
-    return RenderingPipeline[WxNode, WxRenderingContext](pipes=[
-        apply_attributes,
-        render_menu_children,
-        set_to_frame
-    ], create_node=create_menu_node, name='menu bar pipeline')
+    return RenderingPipeline[WxNode, WxRenderingContext](
+        pipes = [apply_attributes, render_menu_children, set_to_frame],
+        create_node = create_menu_node,
+        name = 'menu bar pipeline'
+    )
 
 
 def render_menu_children(node: WxNode, context: WxRenderingContext):
     """Renders sizer children"""
     render_children(node, context, _get_menu_child_context)
 
 
-def _get_menu_child_context(child_xml_node: XmlNode, node: InstanceNode,
-                            _: WxRenderingContext) -> WxRenderingContext:
+def _get_menu_child_context(child_xml_node: XmlNode, node: InstanceNode, _: WxRenderingContext) -> WxRenderingContext:
     return WxRenderingContext({
         'parent_node': node,
         'parent': node.instance,
-        'node_globals': InheritedDict(node.node_globals),
+        'node_globals': NodeGlobals(node.node_globals),
         'xml_node': child_xml_node
     })
 
 
 def set_to_frame(node: InstanceNode, context: WxRenderingContext):
     """Sets menu bar for parent Frame"""
     if not isinstance(context.parent, Frame):
         msg = f'parent for MenuBar should be Frame, but it is {context.parent}'
         raise TypeError(msg)
     context.parent.SetMenuBar(node.instance)
 
 
 def get_menu_pipeline() -> RenderingPipeline:
     """Return render pipeline for Menu"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_menu_children,
-        set_to_menu_bar
-    ], create_node=create_menu_node, name='menu pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, render_menu_children, set_to_menu_bar],
+        create_node = create_menu_node,
+        name = 'menu pipeline'
+    )
 
 
 def set_to_menu_bar(node: WxNode, context: WxRenderingContext):
     """Adds menu to parent MenuBar"""
     if not isinstance(context.parent, MenuBar):
         msg = f'parent for Menu should be MenuBar, but it is {context.parent}'
         raise TypeError(msg)
@@ -71,18 +71,17 @@
     except StopIteration:
         title = str(node.instance)
     context.parent.Append(node.instance, title)
 
 
 def get_menu_item_pipeline() -> RenderingPipeline:
     """Returns rendering pipeline for menu item"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        set_to_menu
-    ], create_node=create_menu_node, name='menu item pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, set_to_menu], create_node = create_menu_node, name = 'menu item pipeline'
+    )
 
 
 def set_to_menu(node: InstanceNode, context: WxRenderingContext):
     """Adds menu item to parent Menu"""
     if not isinstance(context.parent, Menu):
         msg = f'parent for MenuItem should be Menu, but it is {context.parent}'
         raise TypeError(msg)
```

### Comparing `wxviews-0.7.0/wxviews/sizers.py` & `wxviews-0.8.0/wxviews/sizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """Rendering pipeline for SizerNode"""
 
 from typing import Any, Optional
 
-from pyviews.core import InheritedDict, InstanceNode, Node, XmlNode
+from pyviews.core.rendering import InstanceNode, Node, NodeGlobals
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import render_children
-from pyviews.rendering import RenderingPipeline, get_type
-from wx import Sizer, GridSizer, StaticBoxSizer
+from pyviews.rendering.pipeline import RenderingPipeline, get_type
+from wx import GridSizer, Sizer, StaticBoxSizer
 
-from wxviews.core import Sizerable, WxRenderingContext, apply_attributes, add_to_sizer, \
-    get_init_value, get_attr_args
+from wxviews.core.node import Sizerable
+from wxviews.core.pipes import add_to_sizer, apply_attributes
+from wxviews.core.rendering import WxRenderingContext, get_attr_args, get_init_value
 
 
 class SizerNode(InstanceNode, Sizerable):
     """Wrapper under sizer"""
 
-    def __init__(self, instance: Sizer, xml_node: XmlNode,
-                 node_globals: Optional[InheritedDict] = None, parent=None, sizer=None):
-        InstanceNode.__init__(self, instance, xml_node, node_globals=node_globals)
+    def __init__(
+        self,
+        instance: Sizer,
+        xml_node: XmlNode,
+        node_globals: Optional[NodeGlobals] = None,
+        parent = None,
+        sizer = None
+    ):
+        InstanceNode.__init__(self, instance, xml_node, node_globals = node_globals)
         Sizerable.__init__(self)
         self._parent = parent
         self._parent_sizer = sizer
 
     @property
     def sizer_item(self) -> Any:
         return self._instance
@@ -29,110 +37,111 @@
         super().destroy()
         if self._parent_sizer is None and self._parent is not None:
             self._parent.SetSizer(None, True)
 
 
 def get_sizer_pipeline() -> RenderingPipeline:
     """Returns rendering pipeline for SizerNode"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        add_to_sizer,
-        render_sizer_children,
-        set_sizer_to_parent
-    ], create_node=_create_sizer_node, name='sizer pipeline')
+    return RenderingPipeline(
+        pipes = [apply_attributes, add_to_sizer, render_sizer_children, set_sizer_to_parent],
+        create_node = _create_sizer_node,
+        name = 'sizer pipeline'
+    )
 
 
 def _create_sizer_node(context: WxRenderingContext) -> SizerNode:
     inst_type = get_type(context.xml_node)
     if issubclass(inst_type, GridSizer):
         args = _get_init_values(context.xml_node, context.node_globals)
         inst = inst_type(*args)
-        return SizerNode(inst, context.xml_node, node_globals=context.node_globals)
+        return SizerNode(inst, context.xml_node, node_globals = context.node_globals)
 
     if issubclass(inst_type, StaticBoxSizer):
         init_args = get_attr_args(context.xml_node, 'init', context.node_globals)
         args = []
         try:
             static_box = init_args.pop('box')
             args.append(static_box)
         except KeyError:
             args.append(init_args.pop('orient'))
             args.append(context.parent)
         inst = inst_type(*args, **init_args)
-        return SizerNode(inst, context.xml_node,
-                         node_globals=context.node_globals,
-                         parent=inst.GetStaticBox(),
-                         sizer=context.sizer)
+        return SizerNode(
+            inst,
+            context.xml_node,
+            node_globals = context.node_globals,
+            parent = inst.GetStaticBox(),
+            sizer = context.sizer
+        )
     args = get_attr_args(context.xml_node, 'init', context.node_globals)
     inst = inst_type(**args)
-    return SizerNode(inst, context.xml_node,
-                     node_globals=context.node_globals,
-                     parent=context.parent,
-                     sizer=context.sizer)
+    return SizerNode(
+        inst, context.xml_node, node_globals = context.node_globals, parent = context.parent, sizer = context.sizer
+    )
 
 
-def _get_init_values(xml_node: XmlNode, node_globals: Optional[InheritedDict] = None) -> list:
+def _get_init_values(xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None) -> list:
     init_attrs = [attr for attr in xml_node.attrs if attr.namespace == 'init']
     return [get_init_value(attr, node_globals) for attr in init_attrs]
 
 
 def render_sizer_children(node: SizerNode, context: WxRenderingContext):
     """Renders sizer children"""
-    render_children(node, context, lambda x, n, ctx: WxRenderingContext({
-        'parent_node': n,
-        'parent': ctx.parent,
-        'node_globals': InheritedDict(node.node_globals),
-        'sizer': node.instance,
-        'xml_node': x
-    }))
+    render_children(
+        node,
+        context,
+        lambda x,
+        n,
+        ctx: WxRenderingContext({
+            'parent_node': n,
+            'parent': ctx.parent,
+            'node_globals': NodeGlobals(node.node_globals),
+            'sizer': node.instance,
+            'xml_node': x
+        })
+    )
 
 
 def set_sizer_to_parent(node, context: WxRenderingContext):
     """Pass sizer to parent SetSizer"""
     if context.parent is not None and context.sizer is None:
         context.parent.SetSizer(node.instance, True)
 
 
 class GrowableRow(Node):
     """Represents FlexGridSizer.AddGrowableRow method"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
-        super().__init__(xml_node, node_globals=node_globals)
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(xml_node, node_globals = node_globals)
         self.idx = None
         self.proportion = 0
 
 
 def get_growable_row_pipeline() -> RenderingPipeline:
     """Returns rendering pipeline for GrowableRow"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        add_growable_row_to_sizer
-    ], name='growable row pipeline')
+    return RenderingPipeline(pipes = [apply_attributes, add_growable_row_to_sizer], name = 'growable row pipeline')
 
 
 def add_growable_row_to_sizer(node: GrowableRow, context: WxRenderingContext):
     """Calls AddGrowableRow for sizer"""
     context.sizer.AddGrowableRow(node.idx, node.proportion)
 
 
 class GrowableCol(Node):
     """Represents FlexGridSizer.AddGrowableRow method"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
-        super().__init__(xml_node, node_globals=node_globals)
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        super().__init__(xml_node, node_globals = node_globals)
         self.idx = None
         self.proportion = 0
 
 
 def get_growable_col_pipeline() -> RenderingPipeline:
     """Returns rendering pipeline for GrowableRow"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        add_growable_col_to_sizer
-    ], name='growable col pipeline')
+    return RenderingPipeline(pipes = [apply_attributes, add_growable_col_to_sizer], name = 'growable col pipeline')
 
 
 def add_growable_col_to_sizer(node: GrowableCol, context: WxRenderingContext):
     """Calls AddGrowableCol for sizer"""
     context.sizer.AddGrowableCol(node.idx, node.proportion)
```

### Comparing `wxviews-0.7.0/wxviews/styles.py` & `wxviews-0.8.0/wxviews/styles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Contains rendering steps for style nodes"""
 
 from typing import Any, List, Optional
 
-from pyviews.core import PyViewsError, Setter, Node, XmlNode, InheritedDict, XmlAttr
-from pyviews.expression import parse_expression, is_expression, execute
-from pyviews.pipes import render_children, get_setter
-from pyviews.rendering import RenderingPipeline
+from pyviews.core.error import PyViewsError
+from pyviews.core.expression import execute, is_expression, parse_expression
+from pyviews.core.rendering import Node, NodeGlobals, Setter
+from pyviews.core.xml import XmlAttr, XmlNode
+from pyviews.pipes import get_setter, render_children
+from pyviews.rendering.pipeline import RenderingPipeline
 
 from wxviews.containers import render_view_content
-from wxviews.core import WxRenderingContext, apply_attributes
+from wxviews.core.pipes import apply_attributes
+from wxviews.core.rendering import WxRenderingContext
 
 STYLES_KEY = '_node_styles'
 
 
 class StyleError(PyViewsError):
     """Error for style"""
 
@@ -50,109 +53,107 @@
     def __eq__(self, other):
         return hash(self) == hash(other)
 
 
 class Style(Node):
     """Node for storing config options"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
         super().__init__(xml_node, node_globals)
         self.name: Optional[str] = None
         self.items: dict = {}
 
 
 def get_style_pipeline() -> RenderingPipeline:
     """Returns pipeline for style node"""
-    return RenderingPipeline(pipes=[
-        setup_node_styles,
-        apply_style_items,
-        apply_parent_items,
-        store_to_node_styles,
-        render_child_styles
-    ], name='style pipeline')
+    return RenderingPipeline(
+        pipes = [setup_node_styles, apply_style_items, apply_parent_items, store_to_node_styles, render_child_styles],
+        name = 'style pipeline'
+    )
 
 
 def setup_node_styles(_: Style, context: WxRenderingContext):
     """Initializes node styles"""
     if STYLES_KEY not in context.parent_node.node_globals:
-        context.parent_node.node_globals[STYLES_KEY] = InheritedDict()
+        context.parent_node.node_globals[STYLES_KEY] = NodeGlobals()
 
 
 def apply_style_items(node: Style, _: WxRenderingContext):
     """Parsing step. Parses attributes to style items and sets them to style"""
     attrs = node.xml_node.attrs
     try:
         node.name = next(attr.value for attr in attrs if attr.name == 'name')
     except StopIteration as err:
         raise StyleError('Style name is missing', node.xml_node.view_info) from err
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
 
 
 def apply_parent_items(node: Style, context: WxRenderingContext):
     """Sets style items from parent style"""
     if isinstance(context.parent_node, Style):
         node.items = {**context.parent_node.items, **node.items}
 
 
 def store_to_node_styles(node: Style, context: WxRenderingContext):
     """Store styles to node styles"""
     _get_styles(context)[node.name] = node.items.values()
 
 
-def _get_styles(context: WxRenderingContext) -> InheritedDict:
+def _get_styles(context: WxRenderingContext) -> NodeGlobals:
     return context.parent_node.node_globals[STYLES_KEY]
 
 
 def render_child_styles(node: Style, context: WxRenderingContext):
     """Renders child styles"""
-    render_children(node, context, lambda x, n, _: WxRenderingContext({
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
+        _: WxRenderingContext({
+            'parent_node': n,
+            'node_globals': NodeGlobals(node.node_globals),
+            'node_styles': _get_styles(context),
+            'xml_node': x
+        })
+    )
 
 
 class StylesView(Node):
     """Loads styles from separate file"""
 
-    def __init__(self, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
+    def __init__(self, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
         super().__init__(xml_node, node_globals)
         self.name = None
 
 
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
 
 
 def store_to_globals(view: StylesView, context: WxRenderingContext):
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
 
 
 def style(node: Node, _: str, keys: List[str]):
     """Applies styles to node"""
     if isinstance(keys, str):
         keys = [key.strip() for key in keys.split(',') if key]
```

### Comparing `wxviews-0.7.0/wxviews/widgets/binding.py` & `wxviews-0.8.0/wxviews/widgets/binding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Binding based on events"""
 
 from functools import partial
 from typing import Callable, Any, Optional, Type, cast
 
-from injectool import inject
-from pyviews.binding import ExpressionBinding, TwoWaysBinding, BindingContext, \
-    get_expression_callback, Binder
-from pyviews.core import Binding, BindingCallback
-from pyviews.expression import Expression
+from injectool import In, inject
+from pyviews.binding.binder import Binder, BindingContext
+from pyviews.binding.twoways import TwoWaysBinding
+from pyviews.binding.expression import ExpressionBinding, get_expression_callback
+from pyviews.core.binding import Binding, BindingCallback
+from pyviews.core.expression import Expression
 from wx import Event, CommandEvent, EVT_TEXT, EVT_CHECKBOX
 from wx import EvtHandler, TextEntry, CheckBox
 
 
 class EventBinding(Binding):
     """Binds target to wx event"""
 
@@ -39,15 +40,15 @@
     def destroy(self):
         if self._bound:
             self._evt_handler.Unbind(self._event, handler=self._update_target)
             self._bound = False
 
 
 @inject(binder=Binder)
-def use_events_binding(binder: Binder = None):
+def use_events_binding(binder: Binder = In):
     """Adds twoways binding rules"""
     binder.add_rule('twoways', bind_text_and_expression,
                     lambda ctx: check_control_and_property(cast(Type[EvtHandler], TextEntry), ctx))
     binder.add_rule('twoways', bind_check_and_expression,
                     lambda ctx: check_control_and_property(CheckBox, ctx))
```

### Comparing `wxviews-0.7.0/wxviews/widgets/rendering.py` & `wxviews-0.8.0/wxviews/widgets/rendering.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Rendering pipeline for WidgetNode"""
 
 from typing import Callable, Optional
 
-from pyviews.core import InheritedDict, InstanceNode, XmlNode
+from pyviews.core.rendering import InstanceNode, NodeGlobals
+from pyviews.core.xml import XmlNode
 from pyviews.pipes import render_children
-from pyviews.rendering import RenderingPipeline, get_type
-from wx import PyEventBinder, Event
+from pyviews.rendering.pipeline import RenderingPipeline, get_type
+from wx import Event, PyEventBinder
 from wx.py.dispatcher import Any
 
-from wxviews.core import Sizerable, WxRenderingContext, get_attr_args
-from wxviews.core import apply_attributes, add_to_sizer
+from wxviews.core.node import Sizerable
+from wxviews.core.pipes import add_to_sizer, apply_attributes
+from wxviews.core.rendering import WxRenderingContext, get_attr_args
 
 
 class WxNode(InstanceNode, Sizerable):
     """Wrapper under wx widget"""
 
     Root: Optional['WxNode'] = None
 
-    def __init__(self, instance, xml_node: XmlNode, node_globals: Optional[InheritedDict] = None):
-        InstanceNode.__init__(self, instance, xml_node, node_globals=node_globals)
+    def __init__(self, instance, xml_node: XmlNode, node_globals: Optional[NodeGlobals] = None):
+        InstanceNode.__init__(self, instance, xml_node, node_globals = node_globals)
         Sizerable.__init__(self)
 
     @property
     def sizer_item(self) -> Any:
         return self._instance
 
     def bind(self, event: PyEventBinder, handler: Callable[[Event], None], **args):
@@ -32,68 +34,70 @@
     def destroy(self):
         super().destroy()
         self.instance.Destroy()
 
 
 def get_wx_pipeline() -> RenderingPipeline:
     """Returns rendering pipeline for WidgetNode"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        add_to_sizer,
-        render_wx_children
-    ], create_node=_create_widget_node)
+    return RenderingPipeline(
+        pipes = [apply_attributes, add_to_sizer, render_wx_children], create_node = _create_widget_node
+    )
 
 
 def _create_widget_node(context: WxRenderingContext) -> WxNode:
     inst_type = get_type(context.xml_node)
     args = get_attr_args(context.xml_node, 'init', context.node_globals)
     inst = inst_type(context.parent, **args)
-    return WxNode(inst, context.xml_node, node_globals=context.node_globals)
+    return WxNode(inst, context.xml_node, node_globals = context.node_globals)
 
 
 def render_wx_children(node: WxNode, context: WxRenderingContext):
     """Renders WidgetNode children"""
-    render_children(node, context, lambda xn, n, ctx: WxRenderingContext({
-        'parent': n.instance,
-        'parent_node': n,
-        'node_globals': InheritedDict(n.node_globals),
-        'xml_node': xn
-    }))
+    render_children(
+        node,
+        context,
+        lambda xn,
+        n,
+        ctx: WxRenderingContext({
+            'parent': n.instance, 'parent_node': n, 'node_globals': NodeGlobals(n.node_globals), 'xml_node': xn
+        })
+    )
 
 
 def get_frame_pipeline():
     """Returns rendering pipeline for Frame"""
-    return RenderingPipeline(pipes=[
-        apply_attributes,
-        render_wx_children,
-        lambda node, ctx: node.instance.Show()
-    ], create_node=_create_widget_node)
+    return RenderingPipeline(
+        pipes = [apply_attributes, render_wx_children, lambda node, ctx: node.instance.Show()],
+        create_node = _create_widget_node
+    )
 
 
 def get_app_pipeline():
     """Returns rendering pipeline for App"""
-    return RenderingPipeline(pipes=[
-        store_root,
-        apply_attributes,
-        render_app_children,
-    ], create_node=_create_widget_node)
+    return RenderingPipeline(
+        pipes = [store_root, apply_attributes, render_app_children, ], create_node = _create_widget_node
+    )
 
 
 def store_root(node: WxNode, _: WxRenderingContext):
     """Store root node to global property"""
     WxNode.Root = node
 
 
 def render_app_children(node: WxNode, context: WxRenderingContext):
     """Renders App children"""
-    render_children(node, context, lambda x, n, ctx: WxRenderingContext({
-        'xml_node': x,
-        'parent_node': n,
-        'node_globals': InheritedDict(node.node_globals)
-    }))
+    render_children(
+        node,
+        context,
+        lambda x,
+        n,
+        ctx: WxRenderingContext({
+            'xml_node': x, 'parent_node': n, 'node_globals': NodeGlobals(node.node_globals)
+        })
+    )
 
 
 def get_root() -> WxNode:
     """returns root"""
     if WxNode.Root is None:
         raise ValueError("Root is not set")
     return WxNode.Root
```

### Comparing `wxviews-0.7.0/wxviews/widgets/setters.py` & `wxviews-0.8.0/wxviews/widgets/setters.py`

 * *Files identical despite different names*

### Comparing `wxviews-0.7.0/wxviews.egg-info/PKG-INFO` & `wxviews-0.8.0/wxviews.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxviews
-Version: 0.7.0
+Version: 0.8.0
 Summary: Package for creating wx applications in declarative way.
 Project-URL: Homepage, https://github.com/eumis/wxviews
 Keywords: binding,wxviews,wxpython,pyviews,python,mvvm,wx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wxviews-0.7.0/wxviews.egg-info/SOURCES.txt` & `wxviews-0.8.0/wxviews.egg-info/SOURCES.txt`

 * *Files identical despite different names*

