# Comparing `tmp/Kivy4-5.3.0.tar.gz` & `tmp/Kivy4-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kivy4-5.3.0.tar", last modified: Mon Apr 24 09:12:46 2023, max compression
+gzip compressed data, was "Kivy4-5.3.1.tar", last modified: Mon Apr 24 11:04:14 2023, max compression
```

## Comparing `Kivy4-5.3.0.tar` & `Kivy4-5.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 09:12:46.810738 Kivy4-5.3.0/
-drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 09:12:46.809844 Kivy4-5.3.0/Kivy4.egg-info/
--rw-r--r--   0 yoav       (501) staff       (20)      403 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/PKG-INFO
--rw-r--r--   0 yoav       (501) staff       (20)      192 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/SOURCES.txt
--rw-r--r--   0 yoav       (501) staff       (20)        1 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/dependency_links.txt
--rw-r--r--   0 yoav       (501) staff       (20)       44 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/requires.txt
--rw-r--r--   0 yoav       (501) staff       (20)        6 2023-04-24 09:12:46.000000 Kivy4-5.3.0/Kivy4.egg-info/top_level.txt
--rw-r--r--   0 yoav       (501) staff       (20)     1079 2023-04-24 09:08:52.000000 Kivy4-5.3.0/LICENSE.txt
--rw-r--r--   0 yoav       (501) staff       (20)      403 2023-04-24 09:12:46.810510 Kivy4-5.3.0/PKG-INFO
--rw-r--r--   0 yoav       (501) staff       (20)       95 2023-04-24 09:08:52.000000 Kivy4-5.3.0/README.md
-drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 09:12:46.810002 Kivy4-5.3.0/kivy4/
--rw-r--r--   0 yoav       (501) staff       (20)    15659 2023-04-24 09:10:39.000000 Kivy4-5.3.0/kivy4/__init__.py
--rw-r--r--   0 yoav       (501) staff       (20)       38 2023-04-24 09:12:46.810799 Kivy4-5.3.0/setup.cfg
--rw-r--r--   0 yoav       (501) staff       (20)      203 2023-04-24 09:08:52.000000 Kivy4-5.3.0/setup.py
+drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 11:04:14.762481 Kivy4-5.3.1/
+drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 11:04:14.761954 Kivy4-5.3.1/Kivy4.egg-info/
+-rw-r--r--   0 yoav       (501) staff       (20)      403 2023-04-24 11:04:14.000000 Kivy4-5.3.1/Kivy4.egg-info/PKG-INFO
+-rw-r--r--   0 yoav       (501) staff       (20)      192 2023-04-24 11:04:14.000000 Kivy4-5.3.1/Kivy4.egg-info/SOURCES.txt
+-rw-r--r--   0 yoav       (501) staff       (20)        1 2023-04-24 11:04:14.000000 Kivy4-5.3.1/Kivy4.egg-info/dependency_links.txt
+-rw-r--r--   0 yoav       (501) staff       (20)       44 2023-04-24 11:04:14.000000 Kivy4-5.3.1/Kivy4.egg-info/requires.txt
+-rw-r--r--   0 yoav       (501) staff       (20)        6 2023-04-24 11:04:14.000000 Kivy4-5.3.1/Kivy4.egg-info/top_level.txt
+-rw-r--r--   0 yoav       (501) staff       (20)     1079 2023-04-24 09:08:52.000000 Kivy4-5.3.1/LICENSE.txt
+-rw-r--r--   0 yoav       (501) staff       (20)      403 2023-04-24 11:04:14.762328 Kivy4-5.3.1/PKG-INFO
+-rw-r--r--   0 yoav       (501) staff       (20)       95 2023-04-24 09:08:52.000000 Kivy4-5.3.1/README.md
+drwxr-xr-x   0 yoav       (501) staff       (20)        0 2023-04-24 11:04:14.762099 Kivy4-5.3.1/kivy4/
+-rw-r--r--   0 yoav       (501) staff       (20)    15658 2023-04-24 11:04:13.000000 Kivy4-5.3.1/kivy4/__init__.py
+-rw-r--r--   0 yoav       (501) staff       (20)       38 2023-04-24 11:04:14.762532 Kivy4-5.3.1/setup.cfg
+-rw-r--r--   0 yoav       (501) staff       (20)      203 2023-04-24 09:08:52.000000 Kivy4-5.3.1/setup.py
```

### Comparing `Kivy4-5.3.0/LICENSE.txt` & `Kivy4-5.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kivy4-5.3.0/kivy4/__init__.py` & `Kivy4-5.3.1/kivy4/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from kivy.core.window import Window
 from kivy.lang import Builder
 from kivy.uix.settings import ContentPanel
 from kivy.properties import *
 from kivymd.app import MDApp
 from screeninfo import get_monitors
 
-__version__ = '5.3.0'
+__version__ = '5.3.1'
 
 
 class Content(BoxLayout):
     pass
 
 
 def icons(search_value: str = ''):
@@ -406,15 +406,15 @@
             name = self.app_name
 
         return f'''
 Screen:
     MDTopAppBar:
         id: toolbar
         pos_hint: {{"top": 1}}
-        elevation: 10
+        elevation: 3
         title: "{name}"
         right_action_items: {right_icons}
         left_action_items: {left_icons}
 
     MDNavigationLayout:
         x: toolbar.height
         ScreenManager:
```

