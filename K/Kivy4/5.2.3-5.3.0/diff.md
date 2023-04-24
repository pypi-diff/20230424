# Comparing `tmp/Kivy4-5.2.3.tar.gz` & `tmp/Kivy4-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kivy4-5.2.3.tar", last modified: Fri Oct 21 17:11:58 2022, max compression
+gzip compressed data, was "Kivy4-5.3.0.tar", last modified: Mon Apr 24 09:12:46 2023, max compression
```

## Comparing `Kivy4-5.2.3.tar` & `Kivy4-5.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nadav      (501) staff       (20)        0 2022-10-21 17:11:58.158519 Kivy4-5.2.3/
-drwxr-xr-x   0 nadav      (501) staff       (20)        0 2022-10-21 17:11:58.158177 Kivy4-5.2.3/Kivy4.egg-info/
--rw-r--r--   0 nadav      (501) staff       (20)      441 2022-10-21 17:11:58.000000 Kivy4-5.2.3/Kivy4.egg-info/PKG-INFO
--rw-r--r--   0 nadav      (501) staff       (20)      192 2022-10-21 17:11:58.000000 Kivy4-5.2.3/Kivy4.egg-info/SOURCES.txt
--rw-r--r--   0 nadav      (501) staff       (20)        1 2022-10-21 17:11:58.000000 Kivy4-5.2.3/Kivy4.egg-info/dependency_links.txt
--rw-r--r--   0 nadav      (501) staff       (20)       44 2022-10-21 17:11:58.000000 Kivy4-5.2.3/Kivy4.egg-info/requires.txt
--rw-r--r--   0 nadav      (501) staff       (20)        6 2022-10-21 17:11:58.000000 Kivy4-5.2.3/Kivy4.egg-info/top_level.txt
--rw-r--r--   0 nadav      (501) staff       (20)     1079 2022-09-22 17:31:53.000000 Kivy4-5.2.3/LICENSE.txt
--rw-r--r--   0 nadav      (501) staff       (20)      441 2022-10-21 17:11:58.158419 Kivy4-5.2.3/PKG-INFO
--rw-r--r--   0 nadav      (501) staff       (20)       95 2022-09-22 17:31:53.000000 Kivy4-5.2.3/README.md
-drwxr-xr-x   0 nadav      (501) staff       (20)        0 2022-10-21 17:11:58.158273 Kivy4-5.2.3/kivy4/
--rw-r--r--   0 nadav      (501) staff       (20)    15641 2022-10-21 17:11:57.000000 Kivy4-5.2.3/kivy4/__init__.py
--rw-r--r--   0 nadav      (501) staff       (20)       38 2022-10-21 17:11:58.158555 Kivy4-5.2.3/setup.cfg
--rw-r--r--   0 nadav      (501) staff       (20)      203 2022-09-22 17:31:53.000000 Kivy4-5.2.3/setup.py
+drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 09:12:46.810738 Kivy4-5.3.0/
+drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 09:12:46.809844 Kivy4-5.3.0/Kivy4.egg-info/
+-rw-r--r--   0 yoav       (501) staff       (20)      403 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/PKG-INFO
+-rw-r--r--   0 yoav       (501) staff       (20)      192 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/SOURCES.txt
+-rw-r--r--   0 yoav       (501) staff       (20)        1 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/dependency_links.txt
+-rw-r--r--   0 yoav       (501) staff       (20)       44 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/requires.txt
+-rw-r--r--   0 yoav       (501) staff       (20)        6 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/top_level.txt
+-rw-r--r--   0 yoav       (501) staff       (20)     1079 2023-04-24 09:08:52.000000 Kivy4-5.3.0/LICENSE.txt
+-rw-r--r--   0 yoav       (501) staff       (20)      403 2023-04-24 09:12:46.810510 Kivy4-5.3.0/PKG-INFO
+-rw-r--r--   0 yoav       (501) staff       (20)       95 2023-04-24 09:08:52.000000 Kivy4-5.3.0/README.md
+drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 09:12:46.810002 Kivy4-5.3.0/kivy4/
+-rw-r--r--   0 yoav       (501) staff       (20)    15659 2023-04-24 09:10:39.000000 Kivy4-5.3.0/kivy4/__init__.py
+-rw-r--r--   0 yoav       (501) staff       (20)       38 2023-04-24 09:12:46.810799 Kivy4-5.3.0/setup.cfg
+-rw-r--r--   0 yoav       (501) staff       (20)      203 2023-04-24 09:08:52.000000 Kivy4-5.3.0/setup.py
```

### Comparing `Kivy4-5.2.3/LICENSE.txt` & `Kivy4-5.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kivy4-5.2.3/kivy4/__init__.py` & `Kivy4-5.3.0/kivy4/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-import json
-import darkdetect
-import os
-import pyperclip
-import threading
-import time
-import sys
+import json, darkdetect, os, pyperclip, threading, time, sys
 from kivy import Config
 from kivy.uix.boxlayout import BoxLayout
 from kivymd.uix.button import MDFlatButton
 from kivymd.uix.dialog import MDDialog
 from kivymd.uix.pickers import MDDatePicker, MDTimePicker
 
 Config.set('graphics', 'resizable', 0)
@@ -19,15 +13,15 @@
 from kivy.core.window import Window
 from kivy.lang import Builder
 from kivy.uix.settings import ContentPanel
 from kivy.properties import *
 from kivymd.app import MDApp
 from screeninfo import get_monitors
 
-__version__ = '5.2.3'
+__version__ = '5.3.0'
 
 
 class Content(BoxLayout):
     pass
 
 
 def icons(search_value: str = ''):
@@ -144,14 +138,23 @@
     if is_json:
         value = json.dumps(value, indent=2, ensure_ascii=False)
 
     with open(file_path, 'w', encoding=encoding) as f:
         f.write(value)
 
 
+def get_app_data(app_name: str) -> str:
+    is_windows = sys.platform.startswith('win')
+
+    if is_windows:
+        return os.path.join(os.getenv('APPDATA'), app_name)
+
+    return f'./appdata'
+
+
 class Kivy4(MDApp):
     dark_mode_icon = StringProperty('')
 
     def __init__(self, string: str = '', app_name: str = '', dict_of_files: dict[str, str] = None,
                  list_of_dirs: list[str] = None,
                  screen_size=None, minimum=None, center: bool = True,
                  sun_icon: str = 'white-balance-sunny', moon_icon: str = 'weather-night',
@@ -167,23 +170,20 @@
         self.builder_string = '''<Content>
     orientation: "vertical"
     spacing: "12dp"
     size_hint_y: None
     height: "100dp"'''
 
         if app_data:
-            is_windows = sys.platform.startswith('win')
-            app_data_path = os.getenv('APPDATA') + '/' + app_name if is_windows else app_name
-
-            self.appdata_path = app_data_path
+            self.appdata_path = get_app_data(app_name)
             self.create_files(dict_of_files)
             self.create_dirs(list_of_dirs)
 
             self.moon_icon = moon_icon
-            self.sun_icon = sun_icon
+            self.sun_iconf = sun_icon
             self.is_dark_mode()
 
         self.dialog = None
         self.set_properties(main_color, icon, toolbar, string, pre_string, toolbar_name)
         self.disable_x = disable_x
 
         screen = get_monitors()[0]
```

