# Comparing `tmp/wmwpy-0.0.1a0.tar.gz` & `tmp/wmwpy-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.0.1a0.tar", last modified: Mon Mar 13 17:18:37 2023, max compression
+gzip compressed data, was "wmwpy-0.1.0b0.tar", last modified: Mon Apr 24 18:54:34 2023, max compression
```

## Comparing `wmwpy-0.0.1a0.tar` & `wmwpy-0.1.0b0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.036089 wmwpy-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-03-13 17:18:37.036089 wmwpy-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 17:18:37.036089 wmwpy-0.0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.024089 wmwpy-0.0.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.028089 wmwpy-0.0.1a0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.028089 wmwpy-0.0.1a0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.032089 wmwpy-0.0.1a0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.032089 wmwpy-0.0.1a0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.032089 wmwpy-0.0.1a0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/Imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.036089 wmwpy-0.0.1a0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/Widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-13 17:18:26.000000 wmwpy-0.0.1a0/src/wmwpy/gameobject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 17:18:37.028089 wmwpy-0.0.1a0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-03-13 17:18:37.000000 wmwpy-0.0.1a0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-13 17:18:37.000000 wmwpy-0.0.1a0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 17:18:37.000000 wmwpy-0.0.1a0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-13 17:18:37.000000 wmwpy-0.0.1a0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-13 17:18:37.000000 wmwpy-0.0.1a0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.714650 wmwpy-0.1.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/Utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/Utils/waltex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/sprite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.722650 wmwpy-0.1.0b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/Widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-04-24 18:54:19.000000 wmwpy-0.1.0b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:54:34.718650 wmwpy-0.1.0b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 18:54:34.000000 wmwpy-0.1.0b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.0.1a0/LICENSE` & `wmwpy-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/PKG-INFO` & `wmwpy-0.1.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.0.1a0
+Version: 0.1.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.0.1a0/README.md` & `wmwpy-0.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/pyproject.toml` & `wmwpy-0.1.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/src/wmwpy/Game.py` & `wmwpy-0.1.0b0/src/wmwpy/Game.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,165 +1,189 @@
 import os
-import pathlib
-import lxml
-from lxml import etree
-import natsort
-import zipfile
+import typing
 
 from .Utils import Filesystem
 from .Utils import Texture
-from .Utils.path import joinPath
 from .classes import *
 
-os.path.isdir
-
 class Game():
-    def __init__(this, gamepath : str, assets : str = '/assets', db : str = '/Data/water.db', profile : str = None) -> None:
+    _DB = '/Data/water.db'
+    _BASEASSETS = '/'
+    _PROFILE = None
+    
+    game = 'WMW'
+    
+    def __init__(
+        this,
+        gamepath : str, assets : str = '/assets',
+        db : str = '/Data/water.db',
+        profile : str = None,
+        baseassets : str = '/',
+        platform : typing.Literal['android', 'ios'] = 'android',
+        hook : typing.Callable[[int, str, int], typing.Any] = None,
+    ) -> None:
         """load game
 
         Args:
             gamepath (str): Folder to extracted game.
             assets (str, optional): Relative path to assets folder. Defaults to '/assets'.
             db (str, optional): Relative path to database file from assets folder. Defaults to '/Data/water.db'.
             profile (str, optional): Relative path to profile file in WMW2. Defaults to `None`
+            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+            platform (Literal['android', 'ios'], optional): What platform this game is for. Can be 'android' or 'ios'. Defaults to 'android'.
+            hook (Callable[[int, str, int], Any], optional): Hook for loading assets, useful for guis. The function gets called with the paramaters `(progress : int, current : str, max : int)`. Defaults to None.
         """
+        if gamepath == None:
+            return
+        
         this.gamepath = os.path.abspath(gamepath)
-        print(f'{gamepath = }\n{this.gamepath = }')
+        # print(f'{gamepath = }\n{this.gamepath = }')
         this.assets = assets
-        this.db = db
-        this.profile = profile
+        this.db = db or this._DB
+        this.profile = profile or this._PROFILE
+        this.baseassets = baseassets or this._BASEASSETS
+        this.platform = platform
         
-        this.updateFilesystem()
         
-    def updateFilesystem(this):
+        this.updateFilesystem(hook = hook)
+        
+    def updateFilesystem(this, hook : typing.Callable[[int, str, int], typing.Any] = None):
         this.filesystem = Filesystem(this.gamepath, this.assets)
-        this.filesystem.getAssets()
+        this.filesystem.getAssets(hook = hook)
         
-    def loadLevel(this, xmlPath : str = None, imagePath : str = None, ):
+    def Level(this, xmlPath : str = None, imagePath : str = None, ):
         """
         Load level
 
         Args:
             xmlPath (str, optional): Path to xml file. Defaults to None.
             imagePath (str, optional): Path to image file. Defaults to None.
         """
+        split = os.path.splitext(xmlPath)
+        if split[1] == '':
+            imagePath = '.'.join([split[0], 'png'])
+            xmlPath = '.'.join([split[0], 'xml'])
+        
         xml = None
         if xmlPath:
             xml = this.filesystem.get(xmlPath)
         
         image = None
         if imagePath:
             image = this.filesystem.get(imagePath)
         
-        return Level(
+        level = Level(
             xml=xml,
             image=image,
             filesystem=this.filesystem,
         )
+        level.filename = xmlPath
+        
+        return level
     
-    def loadObject(
+    def Object(
         this,
         object : str,
         **kwargs
     ):
         """
         Loads object
 
         Args:
             object (str): Path to `.hs` object file.
 
         Returns:
             classes.object.Object: Where's My Water? object.
         """
         
-        return Object(
+        obj = Object(
             this.filesystem.get(object),
             filesystem = this.filesystem,
             **kwargs
         )
+        obj.filename = object
+        return obj
     
-    def loadImagelist(
+    def Imagelist(
         this,
-        imagelist : str,
+        imagelist : str = None,
         HD = False,
     ):
         """
         Load imagelist
 
         Args:
-            imagelist (str): Path to `.imagelist` file.
+            imagelist (str): Path to `.imagelist` file. Defaults to None
             HD (bool, optional): Whether to use HD textures. Defaults to False.
 
         Returns:
             classes.imagelist.Imagelist: Imagelist object.
         """
-        return Imagelist(
+        
+        imagelistObject = Imagelist(
             this.filesystem.get(imagelist),
             filesystem = this.filesystem,
             HD = False,
         )
+        imagelistObject.filename = imagelist
+        return imagelistObject
     
-    def loadSprite(
+    def Sprite(
         this,
         sprite : str,
         **kwargs
     ):
         """
         Loads sprite.
 
         Args:
             sprite (str): Path to `.sprite` file.`
 
         Returns:
             classes.sprite.Sprite: Sprite object.
         """
-        return Sprite(
+        
+        spriteObject = Sprite(
             this.filesystem.get(sprite),
             filesystem = this.filesystem,
             **kwargs
         )
+        spriteObject.filename = sprite
+        return spriteObject
     
-    def loadTexture(
+    def Texture(
         this,
         texture : str,
     ):
         """
         Get image texture. Doesn't matter if it's a `.waltex` image or not.
 
         Args:
-            this (_type_): _description_
             texture (str): Path to image file.
 
         Returns:
             Utils.textures.Texture: Texture object.
         """
+        
         return Texture(
             this.filesystem.get(texture)
         )
     
-    def loadLayout(this, layout : str):
+    def Layout(this, layout : str):
         raise NotImplementedError('load layout is not implemented yet.')
     
-    def generateFileManifest(this, writeFile : bool = True):
-        manifest = []
-        assets = joinPath(this.gamepath, this.assets)
-        for dir, subdir, files in os.walk(assets):
-            for file in files:
-                # print(f'{file = }\n{dir = }\n{subdir = }')
-                
-                path = pathlib.Path('/', os.path.relpath(os.path.join(dir, file), assets)).as_posix()
-                # path = pathlib.Path(path).parts
-                # print(f'{path = }')
-                manifest.append(path)
-                
-        manifest = natsort.natsorted(manifest)
-        
-        content = '\n'.join(manifest)
-        
-        path = joinPath(this.gamepath, this.assets, 'FileManifest.txt')
-        # print(path)
+    def generateFileManifest(this, writeFile : bool = True, filename : str = '/FileManifest.txt'):
+        """Generate the `FileManifest.txt` file needed for some games, such as WMM. This just generates a text file with the paths to every file in the `assets` folder (which includes the `FileManifest.txt` file).
+
+        Args:
+            writeFile (bool, optional): Write the manifest to the `FileManifest.txt` file. Defaults to True.
+            filename (str, optional): Filename for FileManifest.txt. Defaults to 'filename'.
+
+        Returns:
+            str: Contents of `FileManifest.txt`
+        """
+        manifest = '\n'.join(this.filesystem.listdir(recursive = True))
         
         if writeFile:
-            with open(path, 'w') as file:
-                file.write(content)
-                
+            this.filesystem.add(filename, manifest, replace = True)
+        
         return manifest
```

### Comparing `wmwpy-0.0.1a0/src/wmwpy/Utils/Types/Documents.py` & `wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Documents.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.1.0b0/src/wmwpy/Utils/Types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/src/wmwpy/Utils/textures.py` & `wmwpy-0.1.0b0/src/wmwpy/Utils/textures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,70 @@
 import os
-import pathlib
-import numpy
 from lxml import etree
 from .waltex import WaltexImage, Waltex
 from PIL import Image
-import io
 
 from .path import joinPath
 from .XMLTools import findTag
 from .filesystem import Filesystem, Folder, File
 
 _cachedWaltextImages = {}
 
 class Texture():
     def __init__(this, image : Image.Image | Waltex | File) -> None:
+        """Texture for image.
+
+        Args:
+            image (Image.Image | Waltex | File): Image object. Can be PIL.Image.Image, Waltex image, or file.
+
+        Raises:
+            TypeError: image must be PIL.Image.Image, Waltex, or filesystem.File.
+        """
         this._image = image
         
         if isinstance(this._image, File):
             this._image = this._image.read()
         
         if isinstance(this._image, Waltex):
             this.image = this._image.image
         elif isinstance(this._image, Image.Image):
             this.image = this._image
         else:
-            raise TypeError('image must be PIL.Image.Image or Waltex')
+            raise TypeError('image must be PIL.Image.Image, Waltex, or filesystem.File.')
         
     @property
     def size(this):
         return this.image.size
 
-def getHDFile(file):
+def getHDFile(file : str) -> str:
+    """Get HD filename.
+
+    Args:
+        file (str): Filename
+
+    Returns:
+        str: HD filename.
+    """
     split = os.path.splitext(file)
     split = list(split)
     split.insert(1, '-HD')
     return ''.join(split)
             
 def getTexture(path : str, textureSettings : dict, size : tuple, cache = True) -> Image.Image:
+    """Get image.
+
+    Args:
+        path (str): Path to Image.
+        textureSettings (dict): Texture settings.
+        size (tuple[width,height]): Size of image.
+        cache (bool, optional): Whether to cache waltex images. Defaults to True.
+
+    Returns:
+        Image.Image: PIL Image.
+    """
     type = os.path.splitext(path)[1][1:]
     image = None
     if type == 'waltex':
         if cache:
             try:
                 image = _cachedWaltextImages[path].copy()
             except:
```

### Comparing `wmwpy-0.0.1a0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.1.0b0/src/wmwpy/Utils/waltex.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 from PIL import Image, ImageFile
 import math
 import struct
 import io
 import sys
 # import json
 
-# try:
-import filetype
+try:
+    import filetype
 
-class _WaltexFile(filetype.Type):
-    MIME = 'image/waltex'
-    EXTENSION = 'waltex'
-
-    def __init__(self):
-        super(_WaltexFile, self).__init__(
-            mime=_WaltexFile.MIME,
-            extension=_WaltexFile.EXTENSION,
-        )
-
-    def match(self, buf):
-        return (len(buf) > 3 and
-                buf[0] == 0x57 and
-                buf[1] == 0x41 and
-                buf[2] == 0x4C and
-                buf[3] == 0x54)
+    class _WaltexFile(filetype.Type):
+        MIME = 'image/waltex'
+        EXTENSION = 'waltex'
+
+        def __init__(self):
+            super(_WaltexFile, self).__init__(
+                mime=_WaltexFile.MIME,
+                extension=_WaltexFile.EXTENSION,
+            )
+
+        def match(self, buf):
+            return (len(buf) > 3 and
+                    buf[0] == 0x57 and
+                    buf[1] == 0x41 and
+                    buf[2] == 0x4C and
+                    buf[3] == 0x54)
 
-filetype.add_type(_WaltexFile())
+    filetype.add_type(_WaltexFile())
 # filetype.guess()
-# except:
+except:
     # optional filetype addition
-    # pass
+    pass
 
 # add waltex image to PIL
 # Thanks to Mark Setchell for most of this code https://stackoverflow.com/a/75511423/17129659
 def _accept(prefix):
     return prefix[:4] == b"WALT"
 
 class _WaltexImageFile(ImageFile.ImageFile):
@@ -82,16 +82,30 @@
 )
 
 # main class
  
 class Waltex():
     format = 'waltex'
     format_description = "Walaber image file"
-    
-    def __init__(this, file : str | bytes, byte_order : str = 'little') -> None:
+
+    def __init__(
+        this,
+        file : str | bytes,
+        byte_order : str = 'little'
+    ) -> None:
+        """Waltex image
+
+        Args:
+            file (str | bytes): Waltex file. Can be path to file, contents of file as bytes, or file-like object.
+            byte_order (str, optional): 'little' or 'big'. Defaults to 'little'.
+
+        Raises:
+            TypeError: file has to be a 'str', 'bytes' or file-like object.
+        """
+        
         this._colorspecs = [
             {
                 'order': 'rgba',
                 'bpp': [8,8,8,8],
                 'spec': 'rgba8888',
             },
             {
```

### Comparing `wmwpy-0.0.1a0/src/wmwpy/classes/Imagelist.py` & `wmwpy-0.1.0b0/src/wmwpy/classes/level.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,239 +1,227 @@
-from ..Utils.textures import getHDFile, getTextueSettings, getTexture
-from ..Utils.filesystem import *
-from ..Utils import joinPath, Texture
-from ..gameobject import GameObject
-
-import numpy
-import PIL.Image
+import io
 from lxml import etree
+from PIL import Image
 
-import io
-import os
+from ..Utils.filesystem import *
+from .object import Object
+from ..gameobject import GameObject
 
-class Imagelist(GameObject):
-    class Type():
-        IMAGELIST = 0
-        PAGES = 1
+class Level(GameObject):
+    XML_TEMPLATE = b"""<?xml version="1.0"?>
+    <Objects>
+    </Objects>
+    """
+    
+    IMAGE_TEMPLATE = Image.new('P', (90,127), 'white').quantize(colors=256)
+    IMAGE_FORMAT = 'PNG'
     
     def __init__(
         this,
-        file : str | bytes | File,
+        xml : str | bytes | File = None,
+        image : str | bytes | File = None,
         filesystem : Filesystem | Folder = None,
-        gamepath : str = None, assets : str = '/assets',
-        HD : bool = False
+        gamepath : str = None,
+        assets : str = '/assets',
+        baseassets : str = '/',
     ) -> None:
-        """
-        Get imagelist from file
+        """Load level
+
         Args:
-            file (str | bytes | File): File to read.
+            xml (str | bytes | File): XML file for level.
+            image (str | bytes | File): Image file for level.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
-            HD (bool, optional): Whether to use HD textures. Defaults to False.
-            gamepath (str, optional): Path to game. Only is used when filesystem is `Folder` or `None`. Defaults to None.
-            assets (str, optional): Path to assets relative to gamepath. Defaults to '/assets'.
-        Raises:
-            FileNotFoundError: Filesystem is not usable and no gamepath.
+            gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+            assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+            baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
         """
         
-        super().__init__(filesystem, gamepath, assets)
+        this.gamepath = gamepath
+        this.assets = assets
+        this.filename = ''
+        if this.assets == None:
+            this.assets = '/assets'
+        
+        super().__init__(filesystem, gamepath, assets, baseassets)
+        
+        this.xml_file = super().get_file(xml, template = this.XML_TEMPLATE)
+        
+        this.xml = etree.parse(this.xml_file).getroot()
+        
+        this.image_file = super().get_file(image)
+        if this.image_file == None:
+            this.image = this.IMAGE_TEMPLATE.copy()
+        else:
+            this.image = Image.open(this.image_file).quantize(colors=256)
+        
+        this.objects = []
+        this.properties = {}
+        this.room = (0,0)
         
-        this.file = super().test_file(file)
-
-        this.HD = HD
-        this.xml = etree.parse(this.file).getroot()
-        this.textureBasePath = '/Textures/'
-        this.pages = []
-        this.type = this.Type.IMAGELIST
-
-        this.images = {}
-
         this.read()
     
     def read(this):
-        this.type = this.Type.IMAGELIST
+        """Read level XML
+        """
+        this.objects : list[Object] = []
+        this.properties = {}
         
         for element in this.xml:
+            # comment safe-guard
             if element is etree.Comment:
                 continue
             
-            if element.tag == 'Page':
-                this.type = this.Type.PAGES
-                page = this.Page(
-                    element,
+            if element.tag == 'Object':
+                properties = {}
+                pos = (0,0)
+                name = element.get('name')
+                
+                for el in element:
+                    if not el is etree.Comment:
+                        if el.tag == 'AbsoluteLocation':
+                            pos = el.get('value')
+                        
+                        elif el.tag == 'Properties':
+                            for property in el:
+                                if not property is etree.Comment and property.tag == 'Property':
+                                    properties[property.get('name')] = property.get('value')
+                
+                obj = Object(
+                    this.filesystem.get(properties['Filename']), # get file because `Object` does not take filepath
                     filesystem = this.filesystem,
-                    HD = this.HD,
+                    properties = properties,
+                    pos = pos,
+                    name = name,
                 )
                 
-                this.pages.append(page)
-        
-        if this.type == this.Type.IMAGELIST:
-            page = this.Page(
-                this.xml,
-                filesystem = this.filesystem,
-                HD = this.HD,
-            )
+                this.objects.append(obj)
             
-            this.pages.append(page)
+            if element.tag == 'Properties':
+                for el in element:
+                    if el is etree.Comment:
+                        continue
+                    
+                    if el.tag == 'Property':
+                        this.properties[el.get('name')] = el.get('name')
+            
+            if element.tag == 'Room':
+                for el in element:
+                    if el is etree.Comment:
+                        continue
+                    
+                    if el.tag == 'AbsoluteLocation':
+                        this.room = tuple([float(_) for _ in el.get('value').split()])
     
-    def getImage(this, name : str):
-        for page in this.pages:
-            image = page.getImage(name)
-            if image:
-                return image
-            
-        return None
+    def export(
+        this,
+        filename : str = None,
+        exportObjects : bool = False,
+    ) -> bytes:
+        """Export level
+
+        Args:
+            filename (str, optional): Path to level. Defaults to Level.filename.
+            exportObjects (bool, optional): Whether to export objects. Defaults to False.
+
+        Raises:
+            TypeError: Path is not a file.
+
+        Returns:
+            bytes: XML file.
+        """
+        if filename == None:
+            if this.filename:
+                filename = this.filename
+        else:
+            this.filename = filename
         
-        # return this.filesystem.get(os.path.join(this.textureBasePath, name))
-    
-    class Page(GameObject):
-        def __init__(
-            this,
-            element : etree.ElementBase,
-            filesystem: Filesystem | Folder = None,
-            gamepath: str = None,
-            assets: str = '/assets',
-            HD = False,
-        ) -> None:
-            super().__init__(filesystem, gamepath, assets)
-            
-            this.xml = element
-            
-            this.HD = HD
-            this.id = ''
-            this.imgSize = (1,1)
-            this.textureBasePath = '/Textures/'
-            this.file = ''
-            this.atlas = None
-            this.images = {}
+        xml : etree.ElementBase = etree.Element('Objects')
+        for object in this.objects:
+            if exportObjects:
+                object.export()
             
-            this.read()
+            xml.append(object.getLevelXML())
         
-        class Image():
-            def __init__(
-                this,
-                atlas : PIL.Image.Image,
-                properties : dict
-            ) -> None:
-                """Image for Imagelist
-
-                Args:
-                    this (_type_): _description_
-                    atlas (PIL.Image.Image): Atlas file containing all images
-                    properties (dict): Properties for Image
-                """
-
-                this.atlas = atlas
-                this.properties = properties
-
-                this.size = (1,1)
-                this.offset = (0,0)
-                this.rect = (0,0,0,0)
-                this.name = ''
-
-                this.image = PIL.Image.new('RGBA', this.size)
-
-                this.rawdata = io.BytesIO()
-
-                this.getData()
-                this.getImage()
-
-            def getData(this):
-                if 'size' in this.properties:
-                    this.size = tuple([int(v) for v in this.properties['size'].split(' ')])
-                if 'offset' in this.properties:
-                    this.offset = tuple([int(v) for v in this.properties['offset'].split(' ')])
-                if 'rect' in this.properties:
-                    this.rect = tuple([int(v) for v in this.properties['rect'].split(' ')])
-                if 'name' in this.properties:
-                    this.name = this.properties['name']
-
-            def getImage(this):
-                this.image = this.atlas.crop(numpy.add(this.rect, (0,0) + this.rect[0:2]))
-                this.image = this.image.resize(this.size)
-                
-                this.image.save(this.rawdata, format = os.path.splitext(this.name)[1][1::])
-                return this.image
-
-            def show(this):
-                this.image.show()
-
+        room = etree.Element('Room')
+        etree.SubElement(room, 'AbsoluteLocation', value = ' '.join([str(_) for _ in this.room]))
 
-        def read(this):
-            this.attributes = this.xml.attrib
-            if 'imgSize' in this.attributes:
-                this.size = tuple([int(v) for v in this.attributes['imgSize'].split(' ')])
-            if 'textureBasePath' in this.attributes:
-                this.textureBasePath = this.attributes['textureBasePath']
-            if 'file' in this.attributes:
-                this.file = this.attributes['file']
-            if 'id' in this.attributes:
-                this.id = this.attributes['id']
-    
-            if this.HD:
-                hd = getHDFile(this.file)
-                if this.filesystem.exists(hd):
-                    this.file = hd
-    
-            this.fullAtlasPath = ''
-    
-            if this.gamepath:
-                this.fullAtlasPath = joinPath(this.gamepath, this.assets, this.file)
-                print(this.fullAtlasPath)
-    
-            this.getAtlas()
-            this.getImages()
-    
-    
-        def getAtlas(this):
-            if this.filesystem.exists(this.file):
-                file = this.filesystem.get(this.file)
-                image = Texture(file.read())
-                this.atlas = image.image.copy()
-            else:
-                this.textureSettings = getTextueSettings(
-                    this.gamepath,
-                    this.assets,
-                    joinPath(os.path.dirname(os.path.dirname(this.textureBasePath)), 'Data/textureSettings.xml'),
-                    this.name
-                )
-    
-                this.atlas = getTexture(this.fullAtlasPath, this.textureSettings, this.size)
-    
-        def getImages(this):
-            for image in this.xml:
-                if not image.tag is etree.Comment:
-                    if image.tag == 'Image':
-                        texture = this.Image(this.atlas, properties = image.attrib)
-                        this.images[image.get('name')] = texture
-                        
-                        # print(f'{this.textureBasePath = }')
-                        # print(f'{texture.name = }')
-    
-                        this.filesystem.add(
-                            joinPath(this.textureBasePath, texture.name),
-                            texture.rawdata.getvalue(),
-                            replace = True
-                        )
-    
-        def getImage(this, name : str) -> Image:
-            if name in this.images:
-                return this.images[name]
+        properties = etree.Element('Properties')
+        for name in this.properties:
+            value = this.properties[name]
+            etree.SubElement(properties, 'Property', name = name, value = value)
+        
+        if len(properties):
+            xml.append(properties)
+        
+        this.xml = xml
+        
+        output = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
+        
+        if (file := this.filesystem.get(filename)) != None:
+            if isinstance(file, File):
+                file.write(output)
             else:
-                return None
+                raise TypeError(f'Path {filename} is not a file.')
+                
+        else:
+            this.filesystem.add(filename, output)
+        
+        return output
     
-        def getNO_TEX(this):
-            NO_TEX_settings = getTextueSettings(
-                this.gamepath,
-                this.assets,
-                joinPath(os.path.dirname(os.path.dirname(this.textureBasePath)), 'Data/textureSettings.xml'),
-                os.path.join(this.textureBasePath, 'NO_TEX.png')
+    def addObject(
+        this,
+        filename : str | Object,
+        properties : dict = {},
+        pos : tuple[float,float] = (0,0),
+        name : str = 'Obj'
+    ):
+        """Add object to level.
+
+        Args:
+            filename (str | Object): Filename for object. If it's a wmwpy.classes.Object class, then it will use that instead.
+            properties (dict, optional): Object properties. Defaults to {}.
+            pos (tuple[x,y], optional): Position of object in level. Defaults to (0,0).
+            name (str, optional): Name of object. May get renamed if object with name alread exists. Defaults to 'Obj'.
+
+        Returns:
+            Object: wmwpy Object.
+        """
+        if not isinstance(filename, Object):
+            filename = Object(
+                this.filesystem.get(filename),
+                filesystem = this.filesystem,
+                properties = properties,
+                pos = pos,
+                name = name,
             )
-            NO_TEX_image = PIL.Image.open(joinPath(this.gamepath, this.assets, this.textureBasePath, 'NO_TEX.png')).convert('RGBA')
-            this.NO_TEX = this.Image(NO_TEX_image, {
-                'size': ' '.join([str(x) for x in NO_TEX_image.size]),
-                'rect': ' '.join([str(x) for x in (0,0) + NO_TEX_image.size]),
-                'name': 'NO_TEX.png',
-            })
-            # this.Image(this.atlas, image.attrib)
-    
+        else:
+            filename.name = name
+            filename.pos = pos
+            filename.setProperty(properties)
+        
+        obj = filename
+        
+        if this.getObject(obj.name) != None:
+            objnum = 0
+            name = obj.name
+            
+            while this.getObject(obj.name) != None:
+                objnum += 1
+                obj.name = f'{name}{str(objnum)}'
+        
+        this.objects.append(obj)
+        
+        return obj
     
+    def getObject(this, name : str):
+        """
+        Get object by name
 
+        Args:
+            name (str): Object name.
+        """
+        
+        for obj in this.objects:
+            if obj.name == name:
+                return obj
+        
+        return None
```

### Comparing `wmwpy-0.0.1a0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.1.0b0/src/wmwpy/classes/Widgets.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/src/wmwpy/classes/curves.py` & `wmwpy-0.1.0b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.0.1a0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.1.0b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.0.1a0
+Version: 0.1.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `wmwpy-0.0.1a0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.1.0b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 src/wmwpy/Game.py
 src/wmwpy/__init__.py
 src/wmwpy/gameobject.py
+src/wmwpy/gametemplate.py
 src/wmwpy.egg-info/PKG-INFO
 src/wmwpy.egg-info/SOURCES.txt
 src/wmwpy.egg-info/dependency_links.txt
 src/wmwpy.egg-info/requires.txt
 src/wmwpy.egg-info/top_level.txt
 src/wmwpy/Font/__init__.py
 src/wmwpy/Utils/XMLTools.py
@@ -15,18 +16,18 @@
 src/wmwpy/Utils/filesystem.py
 src/wmwpy/Utils/path.py
 src/wmwpy/Utils/textures.py
 src/wmwpy/Utils/waltex.py
 src/wmwpy/Utils/Types/Documents.py
 src/wmwpy/Utils/Types/Images.py
 src/wmwpy/Utils/Types/__init__.py
-src/wmwpy/classes/Imagelist.py
 src/wmwpy/classes/Widgets.py
 src/wmwpy/classes/__init__.py
 src/wmwpy/classes/curves.py
+src/wmwpy/classes/imagelist.py
 src/wmwpy/classes/layout.py
 src/wmwpy/classes/level.py
 src/wmwpy/classes/object.py
 src/wmwpy/classes/sprite.py
 src/wmwpy/classes/widget/WT_CANVAS.py
 src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
 src/wmwpy/classes/widget/WT_GROUP.py
```

