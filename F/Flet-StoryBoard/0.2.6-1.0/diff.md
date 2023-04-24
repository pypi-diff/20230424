# Comparing `tmp/Flet StoryBoard-0.2.6.tar.gz` & `tmp/Flet StoryBoard-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flet StoryBoard-0.2.6.tar", last modified: Mon Mar 20 13:38:59 2023, max compression
+gzip compressed data, was "Flet StoryBoard-1.0.tar", last modified: Mon Apr 24 14:35:43 2023, max compression
```

## Comparing `Flet StoryBoard-0.2.6.tar` & `Flet StoryBoard-1.0.tar`

### file list

```diff
@@ -1,39 +1,60 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.853498 Flet StoryBoard-0.2.6/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.851203 Flet StoryBoard-0.2.6/Flet_StoryBoard/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.852226 Flet StoryBoard-0.2.6/Flet_StoryBoard/Engines/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-03-18 10:15:30.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/Engines/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    15023 2023-03-18 08:00:26.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/Engines/edit_control_engine.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5368 2023-03-18 08:39:40.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/Engines/preview_engine.py
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       52 2023-03-18 09:30:26.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.852460 Flet StoryBoard-0.2.6/Flet_StoryBoard/built_in_widgets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-03-16 18:56:44.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/built_in_widgets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2945 2023-03-18 08:42:15.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/built_in_widgets/color_picker.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    10123 2023-03-18 08:41:06.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/createStoryBoard.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      459 2023-03-18 09:20:56.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/edit.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5796 2023-03-20 12:30:52.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/editStoryBoard.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      550 2023-03-18 07:49:44.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/loadFletStoryboard.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.852803 Flet StoryBoard-0.2.6/Flet_StoryBoard/pages/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-03-18 10:15:38.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/pages/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-03-18 09:26:22.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/pages/help.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1700 2023-03-18 09:01:00.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/pages/settings.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      839 2023-03-20 13:29:42.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/pyodide.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.853155 Flet StoryBoard-0.2.6/Flet_StoryBoard/tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-03-18 10:15:46.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6905 2023-03-18 08:11:20.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/tools/all_controls.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1241 2023-03-18 08:48:06.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/tools/create_storyboard_file.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.853385 Flet StoryBoard-0.2.6/Flet_StoryBoard/ui_set/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-03-18 10:15:54.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/ui_set/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1227 2023-03-18 05:36:32.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard/ui_set/pick_control_section.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-03-20 13:38:59.851815 Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3275 2023-03-20 13:38:59.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      963 2023-03-20 13:38:59.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-03-20 13:38:59.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        5 2023-03-20 13:38:59.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-03-20 13:38:59.000000 Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 Flet StoryBoard-0.2.6/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       24 2023-02-14 13:25:28.000000 Flet StoryBoard-0.2.6/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3275 2023-03-20 13:38:59.853583 Flet StoryBoard-0.2.6/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     2822 2023-03-18 09:40:30.000000 Flet StoryBoard-0.2.6/README.md
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 Flet StoryBoard-0.2.6/pyproject.toml
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      551 2023-03-20 13:38:59.853839 Flet StoryBoard-0.2.6/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      615 2023-03-20 13:37:15.000000 Flet StoryBoard-0.2.6/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.175756 Flet StoryBoard-1.0/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.169269 Flet StoryBoard-1.0/Flet_StoryBoard/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.170673 Flet StoryBoard-1.0/Flet_StoryBoard/Engines/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:35.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Engines/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8326 2023-04-23 11:23:40.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Engines/edit_subwidgets_engin.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8400 2023-04-23 09:53:37.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Engines/edit_widget_engine.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 14:04:07.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Engines/suggesting_engine.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2696 2023-04-23 09:44:45.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Engines/viewer_engine.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.171726 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:59.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3030 2023-04-21 16:25:25.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/color_picker.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      937 2023-04-24 13:56:24.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/create_storyboard.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      702 2023-04-22 11:06:35.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/get_url_icon.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2857 2023-04-22 13:53:33.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/list_picker.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      118 2023-04-20 11:35:46.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/page_info.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1463 2023-04-24 11:20:56.000000 Flet StoryBoard-1.0/Flet_StoryBoard/Tools/storyboard_class.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.172004 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1117 2023-04-24 11:25:41.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/All.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:18.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.173781 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:25.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2836 2023-04-24 10:12:52.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1966 2023-04-24 13:07:17.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/image.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2954 2023-04-23 15:09:29.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/label.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2077 2023-04-22 15:19:21.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/markdown.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2592 2023-04-24 11:23:12.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/navigator.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3514 2023-04-23 15:22:36.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/open_url.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1696 2023-04-23 15:09:43.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/padding.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2919 2023-04-24 08:30:46.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/paragraph.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7286 2023-04-23 15:54:32.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4927 2023-04-24 10:03:48.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/textfield.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2782 2023-04-23 19:24:28.000000 Flet StoryBoard-1.0/Flet_StoryBoard/WIDGETS/widgets/title.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       92 2023-04-22 14:25:13.000000 Flet StoryBoard-1.0/Flet_StoryBoard/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1057 2023-04-21 16:27:16.000000 Flet StoryBoard-1.0/Flet_StoryBoard/edit.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1170 2023-04-24 11:12:41.000000 Flet StoryBoard-1.0/Flet_StoryBoard/load_storyboard.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.174214 Flet StoryBoard-1.0/Flet_StoryBoard/pages/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:41.000000 Flet StoryBoard-1.0/Flet_StoryBoard/pages/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9938 2023-04-24 13:56:02.000000 Flet StoryBoard-1.0/Flet_StoryBoard/pages/create_new_file.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9683 2023-04-24 14:01:56.000000 Flet StoryBoard-1.0/Flet_StoryBoard/pages/main_page.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.174755 Flet StoryBoard-1.0/Flet_StoryBoard/sections/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:43:49.000000 Flet StoryBoard-1.0/Flet_StoryBoard/sections/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      623 2023-04-23 08:24:47.000000 Flet StoryBoard-1.0/Flet_StoryBoard/sections/edit_section.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2033 2023-04-24 08:50:35.000000 Flet StoryBoard-1.0/Flet_StoryBoard/sections/left_section.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      880 2023-04-24 10:23:00.000000 Flet StoryBoard-1.0/Flet_StoryBoard/sections/preview_section.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.175254 Flet StoryBoard-1.0/Flet_StoryBoard/ui_toolkit/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-04-23 17:44:08.000000 Flet StoryBoard-1.0/Flet_StoryBoard/ui_toolkit/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      784 2023-04-22 17:35:05.000000 Flet StoryBoard-1.0/Flet_StoryBoard/ui_toolkit/widget_browser_frame.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-04-24 14:35:43.169948 Flet StoryBoard-1.0/Flet_StoryBoard.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      386 2023-04-24 14:35:43.000000 Flet StoryBoard-1.0/Flet_StoryBoard.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1762 2023-04-24 14:35:43.000000 Flet StoryBoard-1.0/Flet_StoryBoard.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-04-24 14:35:43.000000 Flet StoryBoard-1.0/Flet_StoryBoard.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       21 2023-04-24 14:35:43.000000 Flet StoryBoard-1.0/Flet_StoryBoard.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       16 2023-04-24 14:35:43.000000 Flet StoryBoard-1.0/Flet_StoryBoard.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-02-14 13:25:28.000000 Flet StoryBoard-1.0/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       24 2023-02-14 13:25:28.000000 Flet StoryBoard-1.0/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      386 2023-04-24 14:35:43.175591 Flet StoryBoard-1.0/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     2487 2023-04-24 14:34:26.000000 Flet StoryBoard-1.0/README.md
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-02-14 13:25:28.000000 Flet StoryBoard-1.0/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-04-24 14:35:43.175872 Flet StoryBoard-1.0/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      525 2023-04-24 14:35:18.000000 Flet StoryBoard-1.0/setup.py
```

### Comparing `Flet StoryBoard-0.2.6/Flet_StoryBoard/Engines/preview_engine.py` & `Flet StoryBoard-1.0/Flet_StoryBoard/Engines/suggesting_engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,107 @@
-from ..tools.all_controls import get_all_supported_controls
+import json
 import flet
+import random
 import os
-import json
-
+import requests
 
+class SuggestingEngine:
+    def __init__(self, main_class):
+        self.main_class = main_class
 
-class previewEngine :
+        self.main_col = flet.Column(width=self.main_class.left_section.main_container.width, 
+        height=self.main_class.left_section.main_container.height, scroll=True)
 
-    def __init__ (self, main_class, mainview=None, development=True, file_path="", bgview=None, functions={}):
-        self.main_class = main_class
-        self.development = development
-        self.functions = functions
+    def push_new_suggestion(self):
+        settings = self.main_class.dict_content["storyboard_settings"]
+        applied = settings["storyboard_suggestions"]
+        if applied == False: return # if `storyboard suggestions` is off.
+        # -----------------------------------------------------------------------
+        suggestions_rules_name = self.main_class.dict_content["pages"][self.main_class.current_page_name]["settings"]["suggestions_rules"]
+        if suggestions_rules_name == "none": return
+        #? Get the rules file
+        if not os.path.isdir("rules"):
+            os.mkdir("rules")
         
-        if mainview == None:
-            if os.path.isfile(file_path) == False:
-                raise OSError(f"cannot find storyboard with name '{file_path}'")
-            file_as_dict = json.loads(open(file_path, encoding="utf-8").read())
-        else:
-            file_as_dict = main_class.file_as_dict
-        self.file_as_dict = file_as_dict
-        self.page_info = file_as_dict["page_settings"]
-        self.controls = file_as_dict["controls"]
-        self.mainview = mainview
-        self.bgview=bgview
-
-        if mainview == None:
-            self.loader()
-        else:
-            self.update()
-    
-
-    def update (self):
-        self.page_info = self.file_as_dict["page_settings"]
-        self.controls = self.file_as_dict["controls"]
-
-        if self.mainview == None:
-            mainview : flet.Page = self.page
-            mainview.auto_scroll = self.page_info["auto_scroll"]
-            mainview.clean()
-            mainview.scroll = self.page_info["scroll"]
-            mainview.title = self.page_info["title"]
-            mainview.window_width = self.page_info["width"]
-            mainview.window_height = self.page_info["height"]
-            mainview.window_full_screen = self.page_info["auto_fullscreen"]
-            mainview.window_resizable = self.page_info["allow_resize"]
-            mainview.bgcolor = self.page_info["bgcolor"]
-            if self.page_info["center_all"]:
-                mainview.vertical_alignment = flet.MainAxisAlignment.CENTER
-            mainview.update()
-        else:
-            mainview : flet.Column = self.mainview
-            mainview.auto_scroll = self.page_info["auto_scroll"]
-            mainview.scroll = self.page_info["scroll"]
-            self.bgview.bgcolor = self.page_info["bgcolor"]
-            if mainview.page != None: mainview.clean()
-
-        # generate_elements
-        num = 0
-        for control in self.controls:
-            if control["kind"] == "control":
-                new_con = self.generate_control(control, num)
-                mainview.controls.append(new_con)
-            num = num + 1
+        if not os.path.isfile(f"rules/{suggestions_rules_name}.json"):
+            all_rules = requests.get("https://raw.githubusercontent.com/SKbarbon/Flet_StoryBoard/main/rules/all.json").text
+            all_rules = json.loads(all_rules)
+            if suggestions_rules_name not in all_rules["all_rules"]: return
+            else:
+                rf = requests.get(all_rules["all_rules"][suggestions_rules_name]).text
+                open(f"rules/{suggestions_rules_name}.json", "w+", encoding="utf-8").write(rf)
         
-        if isinstance(mainview, flet.Page) == False:
-            if mainview.page != None:
-                mainview.update()
+        rules_file = json.loads(open(f"rules/{suggestions_rules_name}.json", encoding="utf-8").read())
+
+        #? step1: Get current widgets.
+        current_widgets = list(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"])
+
+        #? step2: Count classes on widgets.
+        classes_in_widgets = {}
+        for c in current_widgets:
+            if c["widget_class_name"] not in classes_in_widgets:
+                classes_in_widgets[c["widget_class_name"]] = 1
+            else:
+                classes_in_widgets[c["widget_class_name"]] = classes_in_widgets[c["widget_class_name"]] + 1
         
 
-    def loader (self):
-        def main (page:flet.Page):
-            self.page = page
-            self.development = False
-            self.update()
-            page.update()
-        flet.app(target=main)
+        #? step3: Search for the correct case on the rules file.
+        for rule in rules_file["rules"]:
+            if rule["case"] == classes_in_widgets:
+                self.change_left_section_into_suggestion(rule["sugs"])
+                break
     
-    def generate_control (self, control_dict, number_on_list):
-        def on_action (control, action_name, actions_dict):
-            def DoThis (me):
-                if action_name in actions_dict:
-                    if actions_dict[action_name] in self.functions:
-                        self.functions[actions_dict[action_name]]()
-                    else:
-                        print(f"Pass Exception: there is no function called '{actions_dict[action_name]}' that givin.")
-                else:
-                    pass
-            setattr(control, action_name, DoThis)
-            
-
-        def edit_now (me):
-            self.main_class.on_start_edit_control(control_dict["class"], False, number_on_list)
-        # ---
-        if self.mainview == None: self.development = False
-        control_class = get_all_supported_controls()[control_dict["class"]]["class"]
-        control = control_class()
-        for i in control_dict["properties"]:
-            if hasattr(control, i):
-                setattr(control, i, control_dict["properties"][i])
-        if "functions" in control_dict:
-            if self.development == False:
-                for i in control_dict["functions"]:
-                    
-                    if str(control_dict["functions"][i]) == "": pass
-                    else:
-                        if hasattr(control, i):
-                            on_action(control, i, control_dict["functions"])
+
+    def change_left_section_into_suggestion (self, suggestions):
+        def go_back (e):
+            if last_on_section == self.main_col:
+                self.main_class.left_section.show_all_widgets()
+            else:
+                self.main_class.left_section.show_new_content(last_on_section)
         
-        #! -- for support sub-controls
-        if "support_controls" in get_all_supported_controls()[control_dict["class"]]:
-            self.development = False
-            num = 0
-            for i in control_dict["controls"]:
-                s_control = self.generate_control(i, num)
-                control.controls.append(s_control)
-                num = num + 1
-            if self.mainview != None: self.development = True
-        #!! -- for support sub-controls
+        main_clo = self.main_col
+        main_clo.controls.clear()
         
-        if self.development == True:
-            if "expand" in control_dict["properties"]:
-                if control_dict["properties"]["expand"] == True:
-                    contain = flet.Container(content=control, tooltip="click to edit!", on_click=edit_now, expand=True)
-                    return contain
-                else:
-                    contain = flet.Container(content=control, tooltip="click to edit!", on_click=edit_now)
-                    return contain
-            else:
-                contain = flet.Container(content=control, tooltip="click to edit!", on_click=edit_now)
-                return contain
-        else:
-            return control
+        back_btn = flet.TextButton("< Back", on_click=go_back)
+        main_clo.controls.append(back_btn)
+
+        title = flet.Text("Suggestions ✨", weight="bold", size=22, color="white")
+        main_clo.controls.append(title)
+
+        main_clo.controls.append(flet.Row([flet.Text("", color="white", size=13)], alignment="center"))
+
+        for sug in suggestions:
+            sc = self.suggestion_card(sug, go_back)
+            main_clo.controls.append(flet.Row([sc], alignment="center"))
+
+        last_on_section = self.main_class.left_section.main_container
+        self.main_class.left_section.show_new_content(self.main_col)
+
+    def suggestion_card (self, suggestion_dict, go_back_function):
+        def add_widget (e):
+            go_back_function(e)
+            w = self.main_class.add_new_widget(suggestion_dict["class"])
+            w.update(suggestion_dict["props"])
+            self.main_class.preview_section.update_preview(self.main_class.current_page_name)
+            self.main_class.edit_a_widget(len(self.main_class.dict_content["pages"][self.main_class.current_page_name]["widgets"])-1)
+            self.main_class.page.update()
+        # -----
+        colors = ["white", "#F5DEE5", "yellow"]
+        card_container = flet.Container(bgcolor=random.choice(colors), width=170, height=225, border_radius=13)
+        collumn = flet.Column()
+        card_container.content = collumn
+
+        class_name = suggestion_dict["class"]
+        why_to_add = suggestion_dict["about"]
+
+        title = flet.Text(value=f"\n   {class_name}", size=23, weight="bold", color="black", width=card_container.width)
+        collumn.controls.append(title)
+
+        about = flet.Text(value=f"{why_to_add}", size=13, color="black", width=card_container.width-37, height=90)
+        collumn.controls.append(flet.Row([about], alignment="center"))
+
+        apply_button = flet.Container(flet.Row([
+            flet.Text("Add", color="white")
+        ], alignment="center"), bgcolor="black", width=card_container.width-15, height=40, border_radius=13, on_click=add_widget)
+        collumn.controls.append(flet.Row([apply_button], alignment="center"))
+
+        return card_container
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Flet StoryBoard-0.2.6/Flet_StoryBoard/built_in_widgets/color_picker.py` & `Flet StoryBoard-1.0/Flet_StoryBoard/Tools/color_picker.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def none(*args):
     pass
 
 class colorPicker:
 
     def __init__(self, mainview=None, selected_color="white", on_choose_color=none, add_it=True, title_name="select color", drop_width=200, color_prev_width=50) -> None:
         if mainview == None: return
-        self.__all_colors = ["None", "white", "black", "pink", "red", "green", "yellow", "hex-color"]
+        self.__all_colors = ["None", "white", "black", "pink", "red", "green", "yellow", "blue", "hex-color"]
 
         self.drop_width = drop_width
         self.on_choose_color = on_choose_color
         self.mainview = mainview
         self.selected_color = selected_color
 
         v = Container()
@@ -73,8 +73,13 @@
             self.on_choose_color(new_color_selected)
         
         self.v.update()
     
     def update(self):
         self.mainDropdown.value = self.selected_color
         self.color_preview.bgcolor = self.selected_color
-        self.v.update()
+        self.v.update()
+    
+
+    @property
+    def value (self):
+        return self.selected_color
```

### Comparing `Flet StoryBoard-0.2.6/Flet_StoryBoard/createStoryBoard.py` & `Flet StoryBoard-1.0/Flet_StoryBoard/pages/main_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,281 +1,246 @@
+#! This is the editing page of a storyboard.
+from flet import Page, Row, Text
+from ..WIDGETS.All import all_widgets
 import flet
-import time
-import random
 import os
-import threading
-import random
-
-# local imports
-from .built_in_widgets.color_picker import colorPicker
-from .tools.create_storyboard_file import createStoryboardFile
-
-class CreateStoryBoard :
-
-    def __init__ (self):
-        def run (page:flet.Page):
-            self.page = page
-            page.title = "Create new StoryBoard!"
-            page.window_resizable = False
-            page.window_center()
-            page.bgcolor = "white"
-            page.theme = flet.Theme(color_scheme_seed="white")
-            page.vertical_alignment = flet.MainAxisAlignment.CENTER
-            page.update()
-            
-            self.__page_one()
-
-            page.window_center()
-            page.update()
-        flet.app(run)
-    
-    def create_the_storyboard (self, *args):
-        anm = self.animated_view
-        main = flet.Container()
-        mainc = flet.Column()
-        main.content = mainc
-
-        mainc.controls.append(flet.Text("\n\n"))
-
-        Teas_Title = flet.Text("          Building things,\n          Just for you.", weight="bold", size=45, color="white")
-        mainc.controls.append(Teas_Title)
-
-        mainc.controls.append(flet.Text("\n\n\n\n"))
-
-        Loading = flet.Text("🏃‍♀️.", color="white", size=20)
-        mainc.controls.append(flet.Row([Loading], alignment="center"))
-
-        hints = ["you can click settings tab to edit the page settings", "you can set the page to make it auto full screen!",
-        f"Flet website: https://flet.dev"]
-        hint_text = flet.Text(f"short info: {random.choice(hints)}", color="white", size=10)
-        mainc.controls.append(flet.Row([hint_text], alignment="center"))
-
-        anm.content = main
-        anm.update()
-
-        Loading.value = Loading.value + "."
-        Loading.update()
-        time.sleep(1.5)
-        createStoryboardFile(self.PAGE_NAME, self.page_bg_color_selected.selected_color)
-        Loading.value = Loading.value + "."
-        Loading.update()
-        time.sleep(0.5)
-        Loading.value = Loading.value + "."
-        Loading.update()
-        if os.path.isfile(f"{self.PAGE_NAME}.fletsb"):
-            Loading.value = Loading.value + "✅"
-            Loading.update()
-        else:
-            Loading.value = "There is error wile creating the file!"
-            Loading.color = "red"
-            Loading.update()
-        time.sleep(1.5)
-        self.page.window_close()
-        
-
-    def __page_one (self):
-        # To set page's title.
-        page : flet.Page = self.page
-        page.clean()
-
-        m = flet.Row(alignment="center", expand=True)
-        page.add(m)
-
-        dt = flet.Text("Create a StoryBoard!", color="white")
-        ShowCaseBtn = flet.Container(content=flet.Row(alignment="center", controls=[dt])
-        , width=220, height=50, border_radius=10, bgcolor="black")
-        m.controls.append(ShowCaseBtn)
-        page.update()
+import json
+import time
+import requests
 
-        time.sleep(0.3)
 
-        current_wid = ShowCaseBtn.width
-        current_hei = ShowCaseBtn.height
+#* local imports
+from ..sections.left_section import leftSection
+from ..sections.preview_section import previewSection
+from ..sections.edit_section import editSection
+from ..Engines.edit_widget_engine import editWidgetsEngine
+from ..Engines.edit_subwidgets_engin import editSubWidgetsEngine
+from ..Engines.suggesting_engine import SuggestingEngine
+from ..WIDGETS.All import all_widgets
 
-        for i in range(30):
-            ShowCaseBtn.width = ShowCaseBtn.width - 0.5
-            ShowCaseBtn.height = ShowCaseBtn.height - 0.2
-            ShowCaseBtn.update()
-            # time.sleep(0.001)
-            time.sleep(i/450)
 
-        page.bgcolor = "black"
-        dt.color = "black"
-        ShowCaseBtn.bgcolor = "white"
-        page.update()
-        
-        while ShowCaseBtn.width != current_wid and ShowCaseBtn.height != current_hei:
-            if ShowCaseBtn.width != current_wid: ShowCaseBtn.width = ShowCaseBtn.width + 0.1
-            if ShowCaseBtn.height != current_hei: ShowCaseBtn.height = ShowCaseBtn.height + 0.1
-            ShowCaseBtn.update()
-            time.sleep(0.002)
+class mainPage:
+    def __init__(self, file_path):
+        if not os.path.isfile(file_path):
+            raise FileExistsError(f"There is no Flet StoryBoard on path '{file_path}' .")
         
-        for i in range(10):
-            ShowCaseBtn.opacity = ShowCaseBtn.opacity - 0.1
-            ShowCaseBtn.update()
-            time.sleep(0.001)
-        m.controls.remove(ShowCaseBtn)
-        m.update()
-        
-        page.clean()
-        page.update()
 
-        
-        main = flet.Container(expand=True, opacity=0.0)
-        mainc = flet.Column()
-        main.content = mainc
+        self.current_page_name = "main"
+        self.file_path = file_path
+        self.development_mode = True
+        self.dict_content = json.loads(open(file_path, encoding="utf-8").read())
 
-        animated = flet.AnimatedSwitcher(content=main, expand=True,
-        transition=flet.AnimatedSwitcherTransition.FADE, duration=3000,
-        reverse_duration=100, switch_in_curve=flet.AnimationCurve.EASE,
-        switch_out_curve=flet.AnimationCurve.EASE)
-        self.animated_view = animated
-        page.add(animated)
+        #? Copy of classes
+        self.all_widgets = all_widgets
+        self._editWidgetsEngine = editWidgetsEngine
+        self._editSubWidgetsEngine = editSubWidgetsEngine
 
+        #? Run the app
+        flet.app(target=self.app)
 
-        mainc.controls.append(flet.Text("\n\n"))
-
-        Teas_Title = flet.Text("          Your imagine.\n          With ease.", weight="bold", size=45, color="white")
-        mainc.controls.append(Teas_Title)
-
-        mainc.controls.append(flet.Text(
-        "                             Its so easy to build your UI\n                             using your imagine and Flet Storyboard."
-        , color="white"))
-
-        mainc.controls.append(flet.Text("\n\n\n\n\n"))
+    def app (self, page:Page):
+        page.title = f"Flet StoryBoard - {self.file_path}"
+        page.spacing = 0
+        page.bgcolor = "black"
+        page.window_width = 850
+        page.window_height = 650
+        page.window_min_width = 850
+        page.window_min_height = 640
+        self.page = page
+        page.appbar = self.generate_app_bar()
+        page.window_center()
+        page.update()
+
+        # The main row
+        self.main_row = Row(scroll=False)
+        page.add(self.main_row)
+
+        #? append the sections
+        self.left_section = leftSection(page, self, self.main_row)
+        self.preview_section = previewSection(page, self, self.main_row)
+        self.edit_section = editSection(page, self, self.main_row)
+
+        #? Set finals of page.
+        page.on_resize = self.on_page_resize
+        page.on_keyboard_event = self.manage_keyboard_commands
 
-        NextButton = flet.Container(content=flet.Row([flet.Text("Build your's!", color="black", weight="bold")], alignment="center")
-        , bgcolor="white", width=page.width/2, height=50,
-        border_radius=10, on_click=self.__page_two)
-        mainc.controls.append(flet.Row([NextButton], alignment="center"))
 
+        #? Setup the storyboard suggestions engine.
+        self.suggesting_engine = SuggestingEngine(self)
+        time.sleep(0.5)
+        self.suggesting_engine.push_new_suggestion()
 
-        for i in range(10):
-            main.opacity = main.opacity + 0.1
-            main.update()
-            time.sleep(0.02)
+    def on_page_resize (self, *event):
+        page = self.page
+        self.left_section.main_container.width = self.page.width / 4 - 30
+        self.left_section.main_container.height = self.page.height - 70
+        self.preview_section.main_view.width = page.width-(page.width/4)*2
+        self.preview_section.main_view.height = page.height-150
+        self.edit_section.main_column.width = self.page.width / 4 - 10
+        self.edit_section.main_column.height = page.height - 70
 
-        page.update()
+        self.page.update()
     
-
-    def __page_two (self, *args):
-        def on_change_app_name (tf):
-            text = InputStoryboardName.value
-            win_theme[0].value = text
-            self.PAGE_NAME = text
-            if os.path.isfile (f"{text}.fletsb"):
-                InputStoryboardName.focused_color = flet.colors.AMBER
-                InputStoryboardName.label = "There is a file with same name"
-            else:
-                InputStoryboardName.focused_color = flet.colors.BLUE
-                InputStoryboardName.label = "App title"
+    def pages_browser (self):
+        def create_a_page (e):
+            self.create_new_page(str(e.control.value))
+            self.page.appbar = self.generate_app_bar()
             self.page.update()
-    
-        page : flet.Page = self.page
-
-        self.done_page_two = False
-        main = flet.Container(expand=True)
-        mainc = flet.Column()
-        main.content = mainc
-        animated = self.animated_view
-        animated.content = main
-
-        mainc.controls.append(flet.Text("\n\n"))
-
-        Teas_Title = flet.Text("          Your App.\n          Your title.", weight="bold", size=45, color="white")
-        mainc.controls.append(Teas_Title)
-
-        mainc.controls.append(flet.Text(
-        "                             Set your app name that will be displayed\n                             on the top bar of the app"
-        , color="white"))
-
-        mainc.controls.append(flet.Text("\n"))
-
-        InputStoryboardName = flet.TextField(bgcolor="white", width=250, text_size=18, color="black", 
-        border_radius=12, on_change=on_change_app_name, on_submit=self.__page_three, label="App title", 
-        focused_border_color=flet.colors.BLACK45)
-        mainc.controls.append(flet.Row([InputStoryboardName], alignment="center"))
+        def open_a_page (e):
+            page_name = str(e.control.content.controls[0].value)
+            if page_name in self.dict_content["pages"]:
+                self.current_page_name = page_name
+            self.preview_section.update_preview(self.current_page_name)
+            self.last_checked_page_button.bgcolor = flet.colors.GREY_700
+            self.last_checked_page_button = e.control
+            e.control.bgcolor = "blue"
+            time.sleep(0.3)
+            self.suggesting_engine.push_new_suggestion()
+            self.page.update()
+        def ask_for_new_page_name (e):
+            mr.scroll = False
+            tf = flet.TextField(label="Page name", on_submit=create_a_page, height=40, color="white")
+            mr.controls = [tf]
+            mr.update()
+            tf.focus()
+        mr = flet.Row([], width=250, scroll=True)
+        mr.controls.append(flet.TextButton(content=flet.Text("✨", size=18), on_click=self.edit_page_suggestion_state, width=35))
+        new_page_button = flet.Container(flet.Row([flet.Text("+ Page", size=12)], alignment="center"), on_click=ask_for_new_page_name, 
+        bgcolor="white", width=60, height=30, border_radius=12)
+        mr.controls.append(new_page_button)
+
+        for p in self.dict_content["pages"]:
+            c = flet.Container(flet.Row([
+                flet.Text(p, color="white", size=12)
+            ], alignment="center"), bgcolor=flet.colors.GREY_700, width=60, height=30, border_radius=12, on_click=open_a_page)
+            mr.controls.append(c)
+            if str(p) == str(self.current_page_name):
+                c.bgcolor = "blue"
+                self.last_checked_page_button = c
 
-        mainc.controls.append(flet.Text("\n\n"))
-        win_theme = window_theme (mainc)
+        return mr
+    
+    def generate_app_bar (self):
+        a = flet.AppBar(
+            bgcolor=self.page.bgcolor,
+            leading=flet.Row([
+                Text("    "),
+                flet.Icon(flet.icons.DASHBOARD_ROUNDED, size=18, color="white"),
+                Text("Flet StoryBoard", color="white", weight="bold", size=15)
+            ], spacing=15
+            ),
+            actions=[
+                Row([
+                    flet.TextButton(content=flet.Text("Settings", size=12, color="white")),
+                    flet.ElevatedButton("Save", bgcolor="white", color="black", width=100, height=35, 
+                    on_click=self.save_all, tooltip="click to save | also control + S"),
+                    Text("    ")
+                ], alignment=15)
+            ],
+            title=self.pages_browser(),
+            center_title=True
+        )
 
-        page.update()
+        return a
+    
 
-        def after_a_while ():
-            time.sleep(10)
-            if self.done_page_two == False:
-                page.title = str(page.title) + " - Click enter on the textfield after the end."
-                page.update()
-        threading.Thread(target=after_a_while, daemon=True).start()
+    def manage_keyboard_commands (self, event):
+        key = event.key # It would be a key like: 'A' or 'Enter'.
+        shift = event.shift # It would be a bool value of where the shift key is clicked or not.
+        ctrl = event.ctrl # It would be a bool value of where the control key is clicked or not.
+        alt = event.alt # It would be a bool value of where the option key is clicked or not.
+        meta = event.meta # It would be a bool value of where the command key is clicked or not.
+
+        if str(key).lower() == "s" and ctrl:
+            #? Clicked to save file
+            self.save_all()
+        elif str(key).lower() == "s" and meta:
+            #? Clicked to save file
+            self.save_all()
     
-    def __page_three (self, *args):
-        def on_change_bgcolor (color):
-            wn[1].bgcolor = color
-            wn[1].update()
 
-        self.done_page_two = True
+    def save_all (self, *args):
+        new_content = json.dumps(self.dict_content)
+        file = open(self.file_path, "w+", encoding="utf-8")
+        file.write(new_content)
+
         page = self.page
-        page.title = str(page.title).replace(" - Click enter on the textfield after the end.", "")
+        page.snack_bar = flet.SnackBar(
+            content=flet.Text(f"This Flet StoryBoard '{self.file_path}' is saved!"),
+            action="Alright!"
+        )
+        page.snack_bar.open = True
         page.update()
-        animated = self.animated_view
-        main = flet.Container(expand=True)
-        mainc = flet.Column()
-        main.content = mainc
-
-        mainc.controls.append(flet.Text("\n\n"))
-
-        Teas_Title = flet.Text("          Customize.\n          The bgcolor.", weight="bold", size=45, color="white")
-        mainc.controls.append(Teas_Title)
-
-        mainc.controls.append(flet.Text(
-        "                             Set your app background color.\n                             It always good.",
-        color="white"))
-
-        mainc.controls.append(flet.Text("\n"))
-
-        cp = colorPicker(mainc, add_it=False, on_choose_color=on_change_bgcolor)
-        self.page_bg_color_selected = cp
-        mainc.controls.append(flet.Row([cp.v], alignment="center"))
+    
 
-        next_button = flet.Container(content=flet.Row([flet.Text("Done!", color="black", size=13)], alignment="center"), bgcolor="white", width=85,
-        height=30, border_radius=8, on_click=self.create_the_storyboard)
-        mainc.controls.append(flet.Row([next_button], alignment="center"))
+    def add_new_widget (self, widget_name, page_name=None):
+        widget_number = len(self.dict_content["pages"][self.current_page_name]["widgets"])-1
+        widget_class = all_widgets[widget_name]["class"]
+        widget_class = widget_class(self, self.preview_section.main_view_collumn, widget_number=widget_number)
         
-        mainc.controls.append(flet.Text("\n\n"))
-        wn = window_theme (mainc, self.PAGE_NAME)
-
-        animated.content = main
-        animated.update()
-        cp.mainDropdown.focus()
-
-
-
-
-
-# tools
-def none(*args):
-    pass
-def window_theme (view:flet.Column, app_title="App"):
+        self.dict_content["pages"][self.current_page_name]["widgets"].append(widget_class.template)
+        
+        self.preview_section.update_preview(self.current_page_name)
+        self.page.update()
 
-    App_Title = flet.Text(app_title, color="black", expand=True)
+        self.edit_a_widget(len(self.dict_content["pages"][self.current_page_name]["widgets"])-1)
+        
+        time.sleep(0.5)
+        self.suggesting_engine.push_new_suggestion()
 
-    top_bar = flet.Row(controls=[
-        flet.Text(" "),
-        flet.Icon(flet.icons.EMOJI_EMOTIONS, color="black", size=20),
-        App_Title,
-        flet.Row(controls=[
-            flet.Container(width=15, height=15, bgcolor="red", border_radius=7.5, on_hover=none),
-            flet.Container(width=15, height=15, bgcolor="yellow", border_radius=7.5, on_hover=none),
-            flet.Container(width=15, height=15, bgcolor="green", border_radius=7.5, on_hover=none),
-            flet.Text("  ")
-        ],alignment="left")
-    ])
-    mv = flet.Column(controls=[
-        flet.Text("", height=5),
-        flet.Container(top_bar, border=flet.border.only(bottom=flet.border.BorderSide(0.3, "black")), bgcolor="white"),
-        flet.Text("", height=5)
-    ])
+        return widget_class
+    
+    def edit_a_widget (self, widget_number_on_content):
+        self.edit_section.edit_widget_using_engine(widget_number_on_content)
+        self.page.update()
+    
 
-    main_cont = flet.Container(mv, width=450, height=300, bgcolor="white", border_radius=10)
+    def create_new_page (self, page_name):
+        page_dict = {
+            "settings" : {
+                "bgcolor" : "black",
+                "suggestions_rules" : "none"
+            },
+                "widgets" : [
+                            
+            ]
+        }
+        self.dict_content["pages"][page_name] = page_dict
+        self.current_page_name = str(page_name)
+        self.page.appbar = self.generate_app_bar()
+        self.preview_section.update_preview(self.current_page_name)
+    
 
-    view.controls.append(flet.Row([main_cont], alignment="center"))
-    return App_Title, main_cont
+    def edit_page_suggestion_state (self, *a):
+        def go_back (e):
+            self.left_section.show_new_content(last_content)
+            self.page.update()
+        
+        def apply_and_start (name_of_sug):
+            self.dict_content["pages"][self.current_page_name]["settings"]["suggestions_rules"] = str(name_of_sug)
+            go_back("")
+            self.suggesting_engine.push_new_suggestion()
+
+        def make_a_rule_button_option (name):
+            def on_choose (e):
+                apply_and_start(name)
+            b = flet.ElevatedButton(f"{name}", on_click=on_choose, bgcolor="white", color="blacK", width=150, height=45)
+            return flet.Row([b], alignment="center")
+
+        last_content = self.left_section.main_container
+        c = flet.Column(width=last_content.width, height=last_content.height)
+
+        back_btn = flet.TextButton("< Back", on_click=go_back)
+        c.controls.append(back_btn)
+
+        title = flet.Text("Chose the suggestion rules for this page.", color="white", size=17, weight="bold")
+        c.controls.append(title)
+
+        all_rules = requests.get("https://raw.githubusercontent.com/SKbarbon/Flet_StoryBoard/main/rules/all.json").text
+        all_rules = json.loads(all_rules)
+        
+        for rule_option in all_rules["all_rules"]:
+            c.controls.append(make_a_rule_button_option(rule_option))
+
+        c.controls.append(flet.Row([flet.Text("more will come soon", color="white", size=13)], alignment="center"))
+        c.scroll = True
+        self.left_section.show_new_content(c)
```

### Comparing `Flet StoryBoard-0.2.6/Flet_StoryBoard.egg-info/PKG-INFO` & `Flet StoryBoard-1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: Flet-StoryBoard
-Version: 0.2.6
-Summary: A UI-Builder that helps programmers build the front-end without codding it.
-Home-page: https://github.com/SKbarbon/Flet-StoryBoard
-Author: SKbarbon
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Flet StoryBoard
 Flet StoryBoard is a python library that have an easy to use tools for building graphical interfaces based on python `flet` library. Powerful interfaces with simple usability.
 You can use these tools with only two main and simple functions!
 
 ## Goal 🏁
 My goal is to allow programmers to focus on the back-end, and build the front-end using just a simple easy-to-use window without any front-end coding require.
 
@@ -25,64 +12,50 @@
 for Upgrade:
 > `pip install Flet-StoryBoard --upgrade`
 
 if there was anything wrong, and its not upgrading properly, you should uninstall this package and reinstall it:
 > `pip uninstall Flet_StoryBoard` To uninstall
 
 ## requirements ❗️
-- `flet` python library -it will auto install it if you dont have it-.
+- `flet` python library - it will auto install it if you dont have it-.
+- `requests` python library - it will auto install it if you dont have it-.
 - up than python3.7
 
-## whats new on `Flet_StoryBoard` `0.2` 🎉
-- Redesign the editor.
-- We done a major update to the way you create a storyboard, just to make it even more simple to use.
-- Major bug fixes and ui fix.
-- Support Row & Collumn.
-- Support Row-Collumn's sub-controls.
-- Support full page building, instead of just a small widgets.
-- Support editing the storyboard from the cmd/terminal.
-- Big improvment to the preview engine. What you see while edit, its what you will see on the product case.
+## whats new on `Flet_StoryBoard` `1.0` 🎉
+- ReSupport custom widgets with flet.
+- Multiple pages support.
+- New Suggestions
+- New way to load the StoryBoard on your app.
+- The ability of add external `flet` controls inside of the StoryBoard.
+- New Feature called `Smart suggestions`. It get your goal then suggest things based on it.
+- Support templates. A template is a file contain pre-set props for all StoryBoard's widgets, like fonts and default text color. - soon -
+- ReBuild the architecture of the library.
+* Please read the docs to know more about library usage. [docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki)
 * if there is any another issues not fixed yet, please create an issue here: [issues page](https://github.com/SKbarbon/Flet_StoryBoard/issues)
 
 
-## usage 🤝
-There is two main cases you can use with Flet_Storyboard. Lets start with the edit case.
-### edit case.
-To edit an exist storyboard or to create a new one you can use the same cmd command:
-* To create a new one:
-```cmd
-python3 -m Flet_StoryBoard.edit
-```
-* To edit an exist one:
+## usage & examples 🤝
+There is a very simple docs here about library usage.
+[docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki)
+
+### create/edit your own StoryBoard
 ```cmd
-python3 -m Flet_StoryBoard.edit <Your StoryBoard file path>
+python3 -m Flet_StoryBoard.edit myUI.fletsb
 ```
+It will edit the exist one or create a new one if not.
 
-### product case.
-To view your storyboard as a `flet` page, you can write this command:
-```python
-from Flet_StoryBoard import load_flet_storyboard
-
-fsb = load_flet_storyboard("My_File")
-fsb.run()
-```
-Easy right 😇 ?
+### load a StoryBoard
+To load your StoryBoard on your app, you can do this example code:
 
-To link your functions with your buttons or whatever, you can add the functions like this:
 ```python
-from Flet_StoryBoard import load_flet_storyboard
+from Flet_StoryBoard import LoadStoryBoard, StoryBoard
 
-my_functions = {
-    "MyFirstFunction" : MyFirstFunction
-}
+def main (storyBoard:StoryBoard):
+    pass
 
-fsb = load_flet_storyboard("My_File", functions=my_functions)
-fsb.run()
+LoadStoryBoard(target_function=main, storyboard_file_path="myUI.fletsb")
 ```
-Then inside the editor you can type the function name inside the action field of a control.
+
+To know more about the `StoryBoard` class, follow the [docs page](https://github.com/SKbarbon/Flet_StoryBoard/wiki) .
 
 ## comming soon 🔜
-- support more `flet` built-in controls.
-- put a pre-templates UIs to make it even more simple and fast for developers to build their own GUIs.
-- add custom non-built-in `flet` widgets. like `ColorPicker` and `AudioPlayer` widgets.
-- support external-custom widgets from users/programmers.
-- Learn/Help page on the editor to help them learing or with solving problems.
+- add custom non-built-in `flet` widgets. like `ColorPicker` and `AudioPlayer` widgets.
```

### Comparing `Flet StoryBoard-0.2.6/LICENSE` & `Flet StoryBoard-1.0/LICENSE`

 * *Files identical despite different names*

