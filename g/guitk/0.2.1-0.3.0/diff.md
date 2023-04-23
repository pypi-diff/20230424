# Comparing `tmp/guitk-0.2.1.tar.gz` & `tmp/guitk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guitk-0.2.1.tar", max compression
+gzip compressed data, was "guitk-0.3.0.tar", max compression
```

## Comparing `guitk-0.2.1.tar` & `guitk-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.2.1/LICENSE
--rw-r--r--   0        0        0    18916 2023-04-23 18:56:54.325743 guitk-0.2.1/README.md
--rw-r--r--   0        0        0     1095 2023-04-23 18:58:08.640279 guitk-0.2.1/guitk/__init__.py
--rw-r--r--   0        0        0    18484 2023-02-17 19:39:03.000000 guitk-0.2.1/guitk/__main__.py
--rw-r--r--   0        0        0      195 2023-02-14 15:07:46.000000 guitk-0.2.1/guitk/constants.py
--rw-r--r--   0        0        0     2844 2021-03-10 13:52:24.000000 guitk-0.2.1/guitk/redirect.py
--rw-r--r--   0        0        0     2726 2023-02-17 17:18:36.000000 guitk-0.2.1/guitk/tkroot.py
--rw-r--r--   0        0        0     8651 2021-03-08 00:27:37.000000 guitk-0.2.1/guitk/tooltips.py
--rw-r--r--   0        0        0      268 2023-02-15 06:15:34.000000 guitk-0.2.1/guitk/utils.py
--rw-r--r--   0        0        0     1644 2023-04-23 16:31:21.000000 guitk-0.2.1/guitk/widgets/__init__.py
--rw-r--r--   0        0        0     1328 2023-02-16 14:26:34.000000 guitk-0.2.1/guitk/widgets/debugwindow.py
--rw-r--r--   0        0        0     1827 2023-02-16 05:38:10.121090 guitk-0.2.1/guitk/widgets/events.py
--rw-r--r--   0        0        0     3414 2023-02-15 06:05:03.000000 guitk-0.2.1/guitk/widgets/menu.py
--rw-r--r--   0        0        0    10075 2023-04-23 15:10:08.000000 guitk-0.2.1/guitk/widgets/tk_text.py
--rw-r--r--   0        0        0    11231 2023-02-18 21:33:17.000000 guitk-0.2.1/guitk/widgets/ttk_button.py
--rw-r--r--   0        0        0     4309 2023-04-23 16:27:37.000000 guitk-0.2.1/guitk/widgets/ttk_checkbutton.py
--rw-r--r--   0        0        0     3656 2023-04-23 16:26:00.000000 guitk-0.2.1/guitk/widgets/ttk_combobox.py
--rw-r--r--   0        0        0     8950 2023-04-23 15:10:08.000000 guitk-0.2.1/guitk/widgets/ttk_entry.py
--rw-r--r--   0        0        0     6852 2023-04-22 15:34:37.000000 guitk-0.2.1/guitk/widgets/ttk_label.py
--rw-r--r--   0        0        0     5150 2023-04-23 16:28:15.000000 guitk-0.2.1/guitk/widgets/ttk_notebook.py
--rw-r--r--   0        0        0     4655 2023-04-23 16:28:49.000000 guitk-0.2.1/guitk/widgets/ttk_progressbar.py
--rw-r--r--   0        0        0     5496 2023-04-23 16:29:42.000000 guitk-0.2.1/guitk/widgets/ttk_radiobutton.py
--rw-r--r--   0        0        0     4462 2023-04-22 16:14:22.000000 guitk-0.2.1/guitk/widgets/ttk_scale.py
--rw-r--r--   0        0        0    11640 2023-04-23 16:26:50.000000 guitk-0.2.1/guitk/widgets/ttk_treeview.py
--rw-r--r--   0        0        0      290 2023-04-22 15:10:54.000000 guitk-0.2.1/guitk/widgets/types.py
--rw-r--r--   0        0        0     1842 2023-02-17 18:33:45.000000 guitk-0.2.1/guitk/widgets/utils.py
--rw-r--r--   0        0        0     2875 2023-02-18 17:40:47.000000 guitk-0.2.1/guitk/widgets/widget.py
--rw-r--r--   0        0        0    20899 2023-04-22 16:40:19.000000 guitk-0.2.1/guitk/widgets/window.py
--rw-r--r--   0        0        0      590 2023-04-23 18:58:08.641233 guitk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    19488 1970-01-01 00:00:00.000000 guitk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.3.0/LICENSE
+-rw-r--r--   0        0        0    20755 2023-04-23 23:35:05.323243 guitk-0.3.0/README.md
+-rw-r--r--   0        0        0     1137 2023-04-23 23:35:20.854105 guitk-0.3.0/guitk/__init__.py
+-rw-r--r--   0        0        0    18484 2023-02-17 19:39:03.000000 guitk-0.3.0/guitk/__main__.py
+-rw-r--r--   0        0        0      195 2023-02-14 15:07:46.000000 guitk-0.3.0/guitk/constants.py
+-rw-r--r--   0        0        0     2844 2021-03-10 13:52:24.000000 guitk-0.3.0/guitk/redirect.py
+-rw-r--r--   0        0        0     2726 2023-02-17 17:18:36.000000 guitk-0.3.0/guitk/tkroot.py
+-rw-r--r--   0        0        0     8651 2021-03-08 00:27:37.000000 guitk-0.3.0/guitk/tooltips.py
+-rw-r--r--   0        0        0      268 2023-02-15 06:15:34.000000 guitk-0.3.0/guitk/utils.py
+-rw-r--r--   0        0        0     1729 2023-04-23 23:35:05.330433 guitk-0.3.0/guitk/widgets/__init__.py
+-rw-r--r--   0        0        0     1328 2023-02-16 14:26:34.000000 guitk-0.3.0/guitk/widgets/debugwindow.py
+-rw-r--r--   0        0        0     2048 2023-04-23 23:35:05.331122 guitk-0.3.0/guitk/widgets/events.py
+-rw-r--r--   0        0        0     1767 2023-04-23 23:35:05.331577 guitk-0.3.0/guitk/widgets/layout.py
+-rw-r--r--   0        0        0     3414 2023-02-15 06:05:03.000000 guitk-0.3.0/guitk/widgets/menu.py
+-rw-r--r--   0        0        0    10075 2023-04-23 20:56:32.282982 guitk-0.3.0/guitk/widgets/tk_text.py
+-rw-r--r--   0        0        0    11231 2023-04-23 20:51:03.320462 guitk-0.3.0/guitk/widgets/ttk_button.py
+-rw-r--r--   0        0        0     4309 2023-04-23 16:27:37.000000 guitk-0.3.0/guitk/widgets/ttk_checkbutton.py
+-rw-r--r--   0        0        0     3656 2023-04-23 16:26:00.000000 guitk-0.3.0/guitk/widgets/ttk_combobox.py
+-rw-r--r--   0        0        0     8950 2023-04-23 15:10:08.000000 guitk-0.3.0/guitk/widgets/ttk_entry.py
+-rw-r--r--   0        0        0     6852 2023-04-23 21:03:50.313984 guitk-0.3.0/guitk/widgets/ttk_label.py
+-rw-r--r--   0        0        0     5158 2023-04-23 23:35:05.332225 guitk-0.3.0/guitk/widgets/ttk_notebook.py
+-rw-r--r--   0        0        0     4655 2023-04-23 16:28:49.000000 guitk-0.3.0/guitk/widgets/ttk_progressbar.py
+-rw-r--r--   0        0        0     5496 2023-04-23 16:29:42.000000 guitk-0.3.0/guitk/widgets/ttk_radiobutton.py
+-rw-r--r--   0        0        0     4462 2023-04-22 16:14:22.000000 guitk-0.3.0/guitk/widgets/ttk_scale.py
+-rw-r--r--   0        0        0    11640 2023-04-23 16:26:50.000000 guitk-0.3.0/guitk/widgets/ttk_treeview.py
+-rw-r--r--   0        0        0      290 2023-04-22 15:10:54.000000 guitk-0.3.0/guitk/widgets/types.py
+-rw-r--r--   0        0        0     1842 2023-02-17 18:33:45.000000 guitk-0.3.0/guitk/widgets/utils.py
+-rw-r--r--   0        0        0     3492 2023-04-23 23:35:05.332899 guitk-0.3.0/guitk/widgets/widget.py
+-rw-r--r--   0        0        0    22895 2023-04-23 23:35:05.333911 guitk-0.3.0/guitk/widgets/window.py
+-rw-r--r--   0        0        0      590 2023-04-23 23:35:20.854795 guitk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    21327 1970-01-01 00:00:00.000000 guitk-0.3.0/PKG-INFO
```

### Comparing `guitk-0.2.1/LICENSE` & `guitk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/README.md` & `guitk-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 # Python GUI Toolkit for TK (guitk)
 
 ## Synopsis
 
 guitk is an experiment to design a lightweight framework that simplifies creating simple GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html).  This is very much early alpha stage but in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!
 
+guitk allows you to build complete GUI applications with a few lines of code. guitk allows you to use either an event loop, inspired by [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI#example-2---interactive-window), or callbacks for event handling. For simple apps, I find an event loop is easy and intuitive to use. guitk also allows you to layout your app using a simple grid, also inspired by [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI#layouts-are-funny-lol-) -- no need to learn about tkinter packing or grid managers. You provide your layout as a list of lists where each row in the list represents a row in a grid and each element in the row represents a column in the grid. This makes laying out your app very easy and intuitive. guitk also provides a hierarchical layout system inspired by [SwiftUI](https://developer.apple.com/documentation/swiftui) and [applepy](https://github.com/eduardohleite/applepy) which allows you to create complex layouts with minimal code.
+
 ## Code Example
 
+### List of Lists Layout
+
 ![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")
 
 ```python
 """Simple Hello World example using guitk """
 
 import guitk
 
@@ -38,29 +42,74 @@
 
 
 # run your event loop
 if __name__ == "__main__":
     HelloWindow().run()
 ```
 
-## Motivation
+### Hierarchical Layout
+
+![context_layout.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/context_layout.py.png "Hierarchical layout example")
+
+```python
+"""Demo to show how to use context managers to create widget layout"""
+
+import guitk
+
+
+class ShoppingList(guitk.Window):
+    def config(self):
+        self.title = "My Shopping List"
+
+        with guitk.Layout() as layout:
+            with guitk.HStack() as hs:
+                # these will be stacked horizontally (side by side)
+                guitk.Label("Item to buy:")
+                guitk.Entry(key="item", events=True)
+                guitk.Button("Add", key="add")
+            with guitk.VStack() as vs:
+                # these will be stacked vertically (one on top of the other)
+                guitk.Label("Shopping list", anchor="center")
+                guitk.ListBox(key="list")
+                guitk.Button("Quit", key="quit")
+
+        self.layout = layout
 
-I did not set out to create yet another python GUI framework -* there are already many of these, some of them quite good.  I wanted to create a simple GUI for [another python project](https://github.com/RhetTbull/osxphotos) and started down the path using [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI).  PySimpleGUI has an amazingly simple interface that allows creation of nice looking GUIs with just a few lines of code.  Unfortunately, after spending some time prototyping with PySimpleGUI, I discovered a few issues with PySimpleGUI (see below).  I evaluated several other GUI frameworks including [Toga](https://github.com/beeware/toga), [wxPython](https://www.wxpython.org/), [pyglet](https://github.com/pyglet/pyglet), [remi](https://github.com/dddomodossola/remi), and [tkinter](https://docs.python.org/3/library/tkinter.html).  None of these was as simple as PySimpleGUI and several had other issues, e.g. errors running under MacOS, steep learning curve, etc. 
+    def handle_event(self, event: guitk.Event):
+        print(event)
+        if (
+            event.key == "item" and event.event.keysym == "Return"
+        ) or event.key == "add":
+            # add item to the list if user presses Enter in the Entry field
+            # or clicks the Add button
+            name = self["item"].value
+            self["list"].append(name)
+
+            # clear the Entry field
+            self["item"].value = ""
 
-I settled on using tkinter because it's included with python, well-supported on multiple platforms, and relatively light-weight.  However, I found tkinter took a bit too much boiler plate compared to PySimpleGUI and I missed the simplicity of PySimpleGUI's single event loop for quick prototyping.  
+        if event.key == "quit":
+            self.quit()
 
-guitk is my attempt to provide an event-loop interface to tkinter.  It is not intended to abstract away the tkinter interface and you'll need some knowledge of tkinter to use guitk.  I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.  guitk also provides a callback style interface if you prefer that over a single event-loop.
+
+if __name__ == "__main__":
+    ShoppingList().run()
+```
+
+## Motivation
+
+The goal of guitk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), and [applepy](https://github.com/eduardohleite/applepy). guitk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. guitk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.
+
+guitk is not intended to fully abstract away the tkinter interface and you'll need some knowledge of tkinter to use guitk.  I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.
 
 ## Installation
 
 * `python3 -m pip install guitk`
 
-Once this gets past the early alpha stage, I'll package for PyPI.
-
-## Anatomy of a guitk program 
+## Anatomy of a guitk program
 
 ![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")
 
 ```python
 """Hello World example using guitk """
 
 import guitk
@@ -220,15 +269,14 @@
 
 if __name__ == "__main__":
     LayoutDemo().run()
 ```
 
 Because layouts are simply lists of lists, you can use python to create layouts programmatically, for example using list comprehensions.
 
-
 ![layout2.py example](https://github.com/RhetTbull/guitk/raw/main/examples/layout2.py.png "Layout using list comprehensions, with tooltips!")
 
 ```python
 """ Example for guitk showing how to use list comprehensions to create a GUI """
 
 import guitk
 
@@ -345,15 +393,14 @@
 if __name__ == "__main__":
     # add some padding around GUI elements to make it prettier
     HelloWorld().run()
 ```
 
 You can create virtual events that fire after a time delay and these can be repeating.
 
-
 ![bind_timer_event example](https://github.com/RhetTbull/guitk/raw/main/examples/bind_timer_event.py.png "Creating timed virtual events.")
 
 ```python
 """ Example showing how to use bind_timer_event """
 
 import time
 import tkinter as tk
@@ -460,15 +507,15 @@
 
 ## Documentation
 
 Not much documentation at this point.  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.
 
 ## Testing
 
-There are currently no automated tests as I haven't figured out how to do these with tkinter.  You can run `python3 -m guitk` which opens a window with examples of all the widgets.  I currently use this for testing to ensure each widget still works but it's a manual process. 
+There are currently no automated tests as I haven't figured out how to do these with tkinter.  You can run `python3 -m guitk` which opens a window with examples of all the widgets.  I currently use this for testing to ensure each widget still works but it's a manual process.
 
 ## Contributors
 
 Contributions welcome! If this project interests you, open an Issue or send a PR!
 
 ## TODO
 
@@ -481,14 +528,15 @@
 * [x] Radiobutton
 * [x] Text
 * [x] ScrolledText
 * [x] Treeview
 * [x] Listbox
 * [x] Combobox
 * [ ] Other widgets
+* [ ] Menus
 * [x] Tooltips
 * [ ] Documentation
 * [x] Add docstrings
 * [x] Add type hints to public API
 * [ ] Tests
 
 ## License
```

### Comparing `guitk-0.2.1/guitk/__init__.py` & `guitk-0.3.0/guitk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # TODO: add way to specify tooltip delay
 # TODO: add style to all controls
 # TODO: standardize value_type
 
 from .tkroot import *
 from .widgets import *
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 __author__ = "Rhet Turnbull"
 
 __all__ = [
     "BrowseDirectoryButton",
     "BrowseFileButton",
     "Button",
     "CheckButton",
@@ -29,18 +29,20 @@
     "Command",
     "DebugWindow",
     "Entry",
     "Event",
     "EventCommand",
     "EventType",
     "Frame",
+    "HStack",
     "Label",
     "LabelEntry",
     "LabelFrame",
     "Labelframe",
+    "Layout",
     "LinkLabel",
     "Linklabel",
     "ListBox",
     "Listbox",
     "Menu",
     "NoteBook",
     "Notebook",
@@ -50,9 +52,10 @@
     "ProgressBar",
     "Progressbar",
     "RadioButton",
     "Radiobutton",
     "Text",
     "TreeView",
     "Treeview",
+    "VStack",
     "Window",
 ]
```

### Comparing `guitk-0.2.1/guitk/__main__.py` & `guitk-0.3.0/guitk/__main__.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/redirect.py` & `guitk-0.3.0/guitk/redirect.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/tkroot.py` & `guitk-0.3.0/guitk/tkroot.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/tooltips.py` & `guitk-0.3.0/guitk/tooltips.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/__init__.py` & `guitk-0.3.0/guitk/widgets/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .debugwindow import DebugWindow
 from .events import Event, EventCommand, EventType
+from .layout import Layout
 from .menu import Command, Menu
 from .tk_text import Output, Text
 from .ttk_button import BrowseDirectoryButton, BrowseFileButton, Button
 from .ttk_checkbutton import Checkbutton, CheckButton
 from .ttk_combobox import Combobox, ComboBox
 from .ttk_entry import Entry, LabelEntry
 from .ttk_label import Label, LinkLabel
@@ -13,15 +14,15 @@
     PROGRESS_INDETERMINATE,
     Progressbar,
     ProgressBar,
 )
 from .ttk_radiobutton import Radiobutton, RadioButton
 from .ttk_scale import Scale
 from .ttk_treeview import Listbox, ListBox, Treeview, TreeView
-from .window import Frame, LabelFrame, Widget, Window
+from .window import Frame, HStack, LabelFrame, VStack, Widget, Window
 
 __all__ = [
     "BrowseDirectoryButton",
     "BrowseFileButton",
     "Button",
     "CheckButton",
     "Checkbutton",
@@ -30,17 +31,19 @@
     "Command",
     "DebugWindow",
     "Entry",
     "Event",
     "EventCommand",
     "EventType",
     "Frame",
+    "HStack",
     "Label",
     "LabelEntry",
     "LabelFrame",
+    "Layout",
     "LinkLabel",
     "ListBox",
     "Listbox",
     "Menu",
     "NoteBook",
     "Notebook",
     "Output",
@@ -50,14 +53,15 @@
     "Progressbar",
     "RadioButton",
     "Radiobutton",
     "Scale",
     "Text",
     "TreeView",
     "Treeview",
+    "VStack",
     "Widget",
     "Window",
 ]
 
 
 def _get_docstring(name):
     """Return the docstring of an object with name"""
```

### Comparing `guitk-0.2.1/guitk/widgets/debugwindow.py` & `guitk-0.3.0/guitk/widgets/debugwindow.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/events.py` & `guitk-0.3.0/guitk/widgets/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 """Events """
 
+from __future__ import annotations
 
+import tkinter
 from collections import namedtuple
+from typing import Hashable, TypeVar
 
 EventCommand = namedtuple("EventCommand", ["widget", "key", "event_type", "command"])
 
 from enum import Enum, auto
 
+Window = TypeVar("Window")
+Widget = TypeVar("Widget")
+
 
 class Event:
     """Event that occurred and values for widgets in the window"""
 
-    def __init__(self, widget: object, window: "Window", key, event_type):
-        self.id = id(window)
-        self.widget = widget
-        self.key = key
-        self.event_type = event_type
-        self.event = None  # placeholder for Tk event, will be set in _make_callback
+    def __init__(self, widget: object, window: Window, key, event_type):
+        self.id: int = id(window)
+        self.widget: Widget = widget
+        self.key: Hashable = key
+        self.event_type: EventType = event_type
+        self.event: tkinter.Event | None = (
+            None  # placeholder for Tk event, will be set in _make_callback
+        )
 
     def __str__(self):
         return f"id={self.id}, widget={self.widget}, key={self.key}, event_type={self.event_type}, event={self.event}"
 
+
 class EventType(Enum):
     """Constants for event types"""
 
     BrowseFile = "<<BrowseFile>>"
     BrowseDirectory = "<<BrowseDirectory>>"
     ButtonPress = "<<Button>>"
     Checkbutton = "<<Checkbutton>>"
```

### Comparing `guitk-0.2.1/guitk/widgets/menu.py` & `guitk-0.3.0/guitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/tk_text.py` & `guitk-0.3.0/guitk/widgets/tk_text.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_button.py` & `guitk-0.3.0/guitk/widgets/ttk_button.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_checkbutton.py` & `guitk-0.3.0/guitk/widgets/ttk_checkbutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_combobox.py` & `guitk-0.3.0/guitk/widgets/ttk_combobox.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_entry.py` & `guitk-0.3.0/guitk/widgets/ttk_entry.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_label.py` & `guitk-0.3.0/guitk/widgets/ttk_label.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_notebook.py` & `guitk-0.3.0/guitk/widgets/ttk_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tkinter.ttk as ttk
 from typing import Hashable, TypeVar
 
 from .events import Event, EventCommand, EventType
 from .types import CommandType, TabType, TooltipType
 from .widget import Widget
-from .window import Frame, _Layout
+from .window import Frame, LayoutMixin
 
 __all__ = ["Notebook", "NoteBook"]
 
 _valid_standard_attributes = {
     "width",
     "height",
     "padding",
@@ -24,15 +24,15 @@
 
 _valid_ttk_notebook_attributes = _valid_standard_attributes
 
 
 Window = TypeVar("Window")
 
 
-class Notebook(Widget, _Layout):
+class Notebook(Widget, LayoutMixin):
     """
     ttk.Notebook widget
     """
 
     def __init__(
         self,
         key: Hashable | None = None,
```

### Comparing `guitk-0.2.1/guitk/widgets/ttk_progressbar.py` & `guitk-0.3.0/guitk/widgets/ttk_progressbar.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_radiobutton.py` & `guitk-0.3.0/guitk/widgets/ttk_radiobutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_scale.py` & `guitk-0.3.0/guitk/widgets/ttk_scale.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/ttk_treeview.py` & `guitk-0.3.0/guitk/widgets/ttk_treeview.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/utils.py` & `guitk-0.3.0/guitk/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `guitk-0.2.1/guitk/widgets/widget.py` & `guitk-0.3.0/guitk/widgets/widget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """ Widget base class """
 
 from __future__ import annotations
 
 import tkinter as tk
-import tkinter.ttk as ttk
 from typing import Any, Callable, Hashable
 
 from guitk.tkroot import _TKRoot
 
-from .events import Event, EventCommand, EventType
+from .events import Event, EventCommand
 from .types import CommandType, TooltipType, ValueType
 
+from .layout import get_parent
+
 
 class Widget:
     """Basic abstract base class for all tk widgets"""
 
     def __init__(
         self,
         key: Hashable | None = None,
@@ -93,7 +94,22 @@
     @property
     def disabled(self) -> bool:
         return self.widget["state"] == "disabled"
 
     @disabled.setter
     def disabled(self, value: bool) -> None:
         self.widget["state"] = "disabled" if value else "normal"
+
+    def __init_subclass__(subclass, *args, **kwargs):
+        """Ensure that all widgets are added to the parent layout"""
+
+        # This rewrites the __init__ method of the subclass to add the widget to the parent layout
+        super().__init_subclass__(*args, **kwargs)
+
+        def new_init(self, *args, init=subclass.__init__, **kwargs):
+            init(self, *args, **kwargs)
+            if subclass is type(self):
+                # only do this for the bottom grandchild class
+                # in th case of subclassed widgets
+                get_parent().add_widget(self)
+
+        subclass.__init__ = new_init
```

### Comparing `guitk-0.2.1/guitk/widgets/window.py` & `guitk-0.3.0/guitk/widgets/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 
 from __future__ import annotations
 
 import contextlib
 import time
 import tkinter as tk
 from tkinter import ttk
+from typing import Any
 
 from guitk.constants import GUITK
 from guitk.tkroot import _TKRoot
 from guitk.tooltips import Hovertip
 
 from .events import Event, EventCommand, EventType
+from .layout import get_parent, pop_parent, push_parent
 from .menu import Command, Menu
 from .ttk_label import Label
 from .types import TooltipType
 from .widget import Widget
 
 LayoutType = list[list[Widget | None]]
 
 
 class _WindowBaseClass:
     # only needed to keep typing happy
     pass
 
 
-class _Layout:
+class LayoutMixin:
     """Mixin class to provide layout"""
 
     layout = []
 
     def __init__(self, *args, **kwargs):
         pass
 
@@ -70,15 +72,15 @@
                 window._widget_by_key[widget.key] = widget
                 if widget.rowspan and widget.rowspan > 1:
                     row_offset += widget.rowspan - 1
                 if widget.columnspan and widget.columnspan > 1:
                     col_offset += widget.columnspan - 1
 
 
-class Window(_Layout, _WindowBaseClass):
+class Window(LayoutMixin, _WindowBaseClass):
     """Basic Window class from which all windows are derived
 
     Notes:
         Classes which inherit from window should implement handle_event, setup, and teardown as needed
     """
 
     def __init__(
@@ -230,14 +232,16 @@
 
         self.tooltip = None
         """ A callable which returns the tooltip text for a given key or a str """
 
         self.modal = False
         """ Set to True to create modal window """
 
+        push_parent(self)
+
     def config(self):
         pass
 
     def handle_event(self, event):
         """Handle event objects, inheriting classes should implement handle_event"""
         if event.event_type == EventType.Quit:
             self.quit(self._return_value)
@@ -326,14 +330,18 @@
         """Return Tk root instance"""
         return self._tk.root
 
     def children(self):
         """Return child windows"""
         return self._tk.get_children(self)
 
+    def add_widget(self, widget: Any):
+        """Dummy method to allow widgets to be addeded with Layout()"""
+        pass
+
     def _add_menus(self, menu: Menu, menu_items, path=None):
         path = f"MENU:{menu._label}" if path is None else path
         for m in menu_items:
             if type(m) == dict:
                 # submenu
                 for subm in m:
                     subm._create_widget(menu._menu, self)
@@ -430,15 +438,15 @@
     def __getitem__(self, key) -> "Widget":
         try:
             return self._widget_by_key[key]
         except KeyError:
             raise KeyError(f"Invalid key: no widget with key {key}")
 
 
-class _Frame(Widget, _Layout):
+class _Frame(Widget, LayoutMixin):
     """Frame base class for Frame and LabelFrame"""
 
     def __init__(
         self,
         frametype: GUITK = GUITK.ELEMENT_FRAME,
         width: int | None = None,
         key: str | None = None,
@@ -480,15 +488,15 @@
         self.rowspan = rowspan
         self.width = width
         self.height = height
         self.style = style
         self.borderwidth = borderwidth
         self.padding = padding
         self.relief = relief
-        self.layout = layout
+        self.layout = layout or [[]]
         self.text = text
         self.labelanchor = labelanchor or "nw"
 
     def _create_widget(self, parent, window: "Window", row, col):
         self.window = window
         self._parent = parent
 
@@ -558,14 +566,26 @@
     def value(self):
         pass
 
     @value.setter
     def value(self, value):
         pass
 
+    def add_widget(self, widget: Widget):
+        """Add a widget to the frame's layout"""
+        self.layout[0].append(widget)
+
+    def __enter__(self):
+        push_parent(self)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pop_parent()
+        return False
+
 
 class Frame(_Frame):
     def __init__(
         self,
         layout: LayoutType | None = None,
         key: str | None = None,
         width: int | None = None,
@@ -635,7 +655,61 @@
             rowspan=rowspan,
             columnspan=columnspan,
             labelanchor=labelanchor,
             sticky=sticky,
             tooltip=tooltip,
             autoframe=autoframe,
         )
+
+
+class VStack(_Frame):
+    """A frame that stacks widgets vertically when added to a Layout"""
+
+    def __init__(
+        self,
+        key: str | None = None,
+        width: int | None = None,
+        height: int | None = None,
+        style: str | None = None,
+        borderwidth: int | None = None,
+        padding: int | None = None,
+        relief: str = None,
+        disabled: bool | None = False,
+        rowspan: int | None = None,
+        columnspan: int | None = None,
+        sticky: bool | None = None,
+        tooltip: TooltipType | None = None,
+        autoframe: bool = True,
+    ):
+        super().__init__(
+            frametype=GUITK.ELEMENT_FRAME,
+            key=key,
+            width=width,
+            height=height,
+            layout=None,
+            style=style,
+            borderwidth=borderwidth,
+            padding=padding,
+            relief=relief,
+            disabled=disabled,
+            rowspan=rowspan,
+            columnspan=columnspan,
+            sticky=sticky,
+            tooltip=tooltip,
+            autoframe=autoframe,
+        )
+
+    def __enter__(self):
+        push_parent(self)
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        # reorder the layout to be vertical
+        self.layout = [[x] for x in self.layout[0]]
+        pop_parent()
+        return False
+
+
+class HStack(Frame):
+    """A frame that stacks widgets horizontally when added to a Layout"""
+
+    pass
```

### Comparing `guitk-0.2.1/pyproject.toml` & `guitk-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guitk"
-version = "0.2.1"
+version = "0.3.0"
 description = "Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python."
 authors = ["Rhet Turnbull <rturnbull+git@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `guitk-0.2.1/PKG-INFO` & `guitk-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guitk
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python.
 License: MIT
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,16 +17,20 @@
 
 # Python GUI Toolkit for TK (guitk)
 
 ## Synopsis
 
 guitk is an experiment to design a lightweight framework that simplifies creating simple GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html).  This is very much early alpha stage but in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!
 
+guitk allows you to build complete GUI applications with a few lines of code. guitk allows you to use either an event loop, inspired by [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI#example-2---interactive-window), or callbacks for event handling. For simple apps, I find an event loop is easy and intuitive to use. guitk also allows you to layout your app using a simple grid, also inspired by [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI#layouts-are-funny-lol-) -- no need to learn about tkinter packing or grid managers. You provide your layout as a list of lists where each row in the list represents a row in a grid and each element in the row represents a column in the grid. This makes laying out your app very easy and intuitive. guitk also provides a hierarchical layout system inspired by [SwiftUI](https://developer.apple.com/documentation/swiftui) and [applepy](https://github.com/eduardohleite/applepy) which allows you to create complex layouts with minimal code.
+
 ## Code Example
 
+### List of Lists Layout
+
 ![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")
 
 ```python
 """Simple Hello World example using guitk """
 
 import guitk
 
@@ -53,29 +57,74 @@
 
 
 # run your event loop
 if __name__ == "__main__":
     HelloWindow().run()
 ```
 
-## Motivation
+### Hierarchical Layout
+
+![context_layout.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/context_layout.py.png "Hierarchical layout example")
+
+```python
+"""Demo to show how to use context managers to create widget layout"""
+
+import guitk
+
+
+class ShoppingList(guitk.Window):
+    def config(self):
+        self.title = "My Shopping List"
+
+        with guitk.Layout() as layout:
+            with guitk.HStack() as hs:
+                # these will be stacked horizontally (side by side)
+                guitk.Label("Item to buy:")
+                guitk.Entry(key="item", events=True)
+                guitk.Button("Add", key="add")
+            with guitk.VStack() as vs:
+                # these will be stacked vertically (one on top of the other)
+                guitk.Label("Shopping list", anchor="center")
+                guitk.ListBox(key="list")
+                guitk.Button("Quit", key="quit")
+
+        self.layout = layout
 
-I did not set out to create yet another python GUI framework -* there are already many of these, some of them quite good.  I wanted to create a simple GUI for [another python project](https://github.com/RhetTbull/osxphotos) and started down the path using [PySimpleGUI](https://github.com/PySimpleGUI/PySimpleGUI).  PySimpleGUI has an amazingly simple interface that allows creation of nice looking GUIs with just a few lines of code.  Unfortunately, after spending some time prototyping with PySimpleGUI, I discovered a few issues with PySimpleGUI (see below).  I evaluated several other GUI frameworks including [Toga](https://github.com/beeware/toga), [wxPython](https://www.wxpython.org/), [pyglet](https://github.com/pyglet/pyglet), [remi](https://github.com/dddomodossola/remi), and [tkinter](https://docs.python.org/3/library/tkinter.html).  None of these was as simple as PySimpleGUI and several had other issues, e.g. errors running under MacOS, steep learning curve, etc. 
+    def handle_event(self, event: guitk.Event):
+        print(event)
+        if (
+            event.key == "item" and event.event.keysym == "Return"
+        ) or event.key == "add":
+            # add item to the list if user presses Enter in the Entry field
+            # or clicks the Add button
+            name = self["item"].value
+            self["list"].append(name)
+
+            # clear the Entry field
+            self["item"].value = ""
 
-I settled on using tkinter because it's included with python, well-supported on multiple platforms, and relatively light-weight.  However, I found tkinter took a bit too much boiler plate compared to PySimpleGUI and I missed the simplicity of PySimpleGUI's single event loop for quick prototyping.  
+        if event.key == "quit":
+            self.quit()
 
-guitk is my attempt to provide an event-loop interface to tkinter.  It is not intended to abstract away the tkinter interface and you'll need some knowledge of tkinter to use guitk.  I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.  guitk also provides a callback style interface if you prefer that over a single event-loop.
+
+if __name__ == "__main__":
+    ShoppingList().run()
+```
+
+## Motivation
+
+The goal of guitk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), and [applepy](https://github.com/eduardohleite/applepy). guitk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. guitk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.
+
+guitk is not intended to fully abstract away the tkinter interface and you'll need some knowledge of tkinter to use guitk.  I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.
 
 ## Installation
 
 * `python3 -m pip install guitk`
 
-Once this gets past the early alpha stage, I'll package for PyPI.
-
-## Anatomy of a guitk program 
+## Anatomy of a guitk program
 
 ![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")
 
 ```python
 """Hello World example using guitk """
 
 import guitk
@@ -235,15 +284,14 @@
 
 if __name__ == "__main__":
     LayoutDemo().run()
 ```
 
 Because layouts are simply lists of lists, you can use python to create layouts programmatically, for example using list comprehensions.
 
-
 ![layout2.py example](https://github.com/RhetTbull/guitk/raw/main/examples/layout2.py.png "Layout using list comprehensions, with tooltips!")
 
 ```python
 """ Example for guitk showing how to use list comprehensions to create a GUI """
 
 import guitk
 
@@ -360,15 +408,14 @@
 if __name__ == "__main__":
     # add some padding around GUI elements to make it prettier
     HelloWorld().run()
 ```
 
 You can create virtual events that fire after a time delay and these can be repeating.
 
-
 ![bind_timer_event example](https://github.com/RhetTbull/guitk/raw/main/examples/bind_timer_event.py.png "Creating timed virtual events.")
 
 ```python
 """ Example showing how to use bind_timer_event """
 
 import time
 import tkinter as tk
@@ -475,15 +522,15 @@
 
 ## Documentation
 
 Not much documentation at this point.  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.
 
 ## Testing
 
-There are currently no automated tests as I haven't figured out how to do these with tkinter.  You can run `python3 -m guitk` which opens a window with examples of all the widgets.  I currently use this for testing to ensure each widget still works but it's a manual process. 
+There are currently no automated tests as I haven't figured out how to do these with tkinter.  You can run `python3 -m guitk` which opens a window with examples of all the widgets.  I currently use this for testing to ensure each widget still works but it's a manual process.
 
 ## Contributors
 
 Contributions welcome! If this project interests you, open an Issue or send a PR!
 
 ## TODO
 
@@ -496,14 +543,15 @@
 * [x] Radiobutton
 * [x] Text
 * [x] ScrolledText
 * [x] Treeview
 * [x] Listbox
 * [x] Combobox
 * [ ] Other widgets
+* [ ] Menus
 * [x] Tooltips
 * [ ] Documentation
 * [x] Add docstrings
 * [x] Add type hints to public API
 * [ ] Tests
 
 ## License
```

