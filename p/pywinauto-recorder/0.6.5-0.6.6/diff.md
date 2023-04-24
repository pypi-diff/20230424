# Comparing `tmp/pywinauto_recorder-0.6.5.tar.gz` & `tmp/pywinauto_recorder-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywinauto_recorder-0.6.5.tar", last modified: Wed Mar  1 14:36:58 2023, max compression
+gzip compressed data, was "pywinauto_recorder-0.6.6.tar", last modified: Mon Apr 24 08:03:39 2023, max compression
```

## Comparing `pywinauto_recorder-0.6.5.tar` & `pywinauto_recorder-0.6.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:36:58.282050 pywinauto_recorder-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-01 14:36:58.282050 pywinauto_recorder-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:36:58.282050 pywinauto_recorder-0.6.5/pywinauto_recorder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:36:58.282050 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/
--rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/IconPyRec.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/check.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/comments.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/cross.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/favourite.ico
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/folder.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/help.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/light-on.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/paste.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/play.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/power.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/record.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/search.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/settings.ico
--rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/stop.ico
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/element_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/ocr_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    34835 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/player.py
--rw-r--r--   0 runner    (1001) docker     (123)    40609 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/pywinauto_recorder/recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:36:58.282050 pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-01 14:36:58.000000 pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-01 14:36:58.000000 pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 14:36:58.000000 pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-01 14:36:58.000000 pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 14:36:58.000000 pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 14:36:58.282050 pywinauto_recorder-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-01 14:36:48.000000 pywinauto_recorder-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:03:39.150487 pywinauto_recorder-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-24 08:03:39.150487 pywinauto_recorder-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:03:39.146487 pywinauto_recorder-0.6.6/pywinauto_recorder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:03:39.150487 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/IconPyRec.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/check.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/comments.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/cross.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/favourite.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/folder.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/help.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/light-on.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/paste.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/play.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/power.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/record.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/search.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    56150 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/stop.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/element_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/ocr_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36316 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38830 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/pywinauto_recorder/recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:03:39.146487 pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-24 08:03:39.000000 pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-24 08:03:39.000000 pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:03:39.000000 pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 08:03:39.000000 pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 08:03:39.000000 pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:03:39.150487 pywinauto_recorder-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-24 08:03:28.000000 pywinauto_recorder-0.6.6/setup.py
```

### Comparing `pywinauto_recorder-0.6.5/LICENSE` & `pywinauto_recorder-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/PKG-INFO` & `pywinauto_recorder-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinauto_recorder
-Version: 0.6.5
+Version: 0.6.6
 Summary: Records/Replays GUI actions
 Home-page: https://github.com/beuaaa/pywinauto_recorder
 Author: david pratmarty
 Author-email: david.pratmarty@gmail.com
 License: MIT
 Project-URL: Documentation, https://pywinauto-recorder.readthedocs.io
 Project-URL: Source, https://github.com/beuaaa/pywinauto_recorder
```

### Comparing `pywinauto_recorder-0.6.5/README.rst` & `pywinauto_recorder-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/IconPyRec.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/IconPyRec.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/check.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/check.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/comments.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/comments.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/cross.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/cross.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/favourite.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/favourite.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/folder.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/folder.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/help.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/help.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/light-on.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/light-on.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/paste.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/paste.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/play.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/play.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/power.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/power.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/record.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/record.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/search.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/search.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/settings.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/settings.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/Icons/stop.ico` & `pywinauto_recorder-0.6.6/pywinauto_recorder/Icons/stop.ico`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/__init__.py` & `pywinauto_recorder-0.6.6/pywinauto_recorder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 """
     Pywinauto recorder records user interface actions and saves them in a Python script.
     The generated Python script plays back user interface actions in the order in which the user recorded them.
 
     Pywinauto recorder uses accessibility technologies via the Pywinauto_ library.
 """
 
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 
 from .player import *
 from .recorder import Recorder
```

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/core.py` & `pywinauto_recorder-0.6.6/pywinauto_recorder/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
 import re
-import traceback
 from enum import Enum
 import configparser
 import ast
 from pywinauto import Desktop as PywinautoDesktop
 from pywinauto.controls.uiawrapper import UIAWrapper
 from pywinauto import findwindows
-from cachetools import func
+from thefuzz import fuzz
+from .ocr_wrapper import find_all_ocr, OCRWrapper
 
 
-__all__ = ['path_separator', 'type_separator', 'Strategy', 'is_int',
+__all__ = ['path_separator', 'type_separator', 'Strategy', 'is_int', 'is_absolute_path',
            'get_wrapper_path', 'get_entry_list', 'get_entry', 'match_entry_list', 'get_sorted_region',
            'find_elements', 'read_config_file']
 
 desktop = PywinautoDesktop(backend='uia', allow_magic_lookup=False)
 
 
 class CoreSettings:
@@ -47,23 +47,22 @@
 	try:
 		path = ''
 		wrapper_top_level_parent = wrapper.top_level_parent()
 		while wrapper != wrapper_top_level_parent:
 			path = path_separator + wrapper.element_info.name + type_separator + wrapper.element_info.control_type + path
 			wrapper = wrapper.parent()
 		return wrapper.element_info.name + type_separator + wrapper.element_info.control_type + path
-	except Exception as e:
-		traceback.print_exc()
-		print(e.message)
+	except Exception:
 		return ''
 
 
 def get_entry_list(path):
 	"""
 	It splits the path into a list of entries
+	It only handles one #[y,x] at the end. It does not handle the #[y,x] in the middle.
 	
 	:param path: the path to the element
 	:return: A list of the entries.
 	"""
 	i = path.rfind("#[")
 	if i != -1:
 		i = path.rfind(path_separator, 0, i)
@@ -90,21 +89,27 @@
 	try:
 		int(s)
 		return True
 	except ValueError:
 		return False
 
 
+def is_absolute_path(entry):
+	return entry[-16:] == '~Absolute_UIPath'
+
+
 def get_entry(entry):
 	"""
-	It takes a string of the form `"name"#["y",x]%(dx,dy)` and returns a tuple of the form `(name, type, [y,x], (dx,dy))`
+	It takes a string of the form "name"#["y",x]%(dx,dy)~Absolute_UIPath and returns a tuple of the form (name, type, [y,x], (dx,dy))
 	
 	:param entry: the string that is the entry in the listbox
 	:return: The name of the entry, the type of the entry, the size of the entry, and the dx and dy of the entry.
 	"""
+	if is_absolute_path(entry):
+		entry = entry[:-16]
 	if entry[0:7] == "RegEx: ":
 		entry = entry[7:]
 	i = entry.find(type_separator)
 	if i == -1:
 		return entry, None, None, None
 	while i < len(entry) and entry[i] == type_separator[0]:
 		i = i + 1
@@ -119,28 +124,28 @@
 		entry3 = entry2[0:i]
 	else:
 		str_dx_dy = None
 		entry3 = entry2
 	
 	i = entry3.rfind("""#[""")
 	if i != -1:
-		str_array = entry3[i + 2:]
+		str_array = entry3[i + 2:-1]
 		str_type = entry3[0:i]
 	else:
 		str_array = None
 		str_type = entry3
 	
 	if str_type == '':
 		str_type = None
 	if str_array:
 		words = str_array.split(',')
 		y = words[0]
 		if is_int(y):
 			y = int(y)
-		x = int(words[1][:-1])
+		x = int(words[1])
 		y_x = [y, x]
 	else:
 		y_x = None
 	if str_dx_dy:
 		words = str_dx_dy.split(',')
 		dx_dy = (float(words[0]), float(words[1].split(')')[0]))
 	else:
@@ -171,93 +176,34 @@
 	entry_name, entry_type, _, _ = get_entry(entry)
 	if is_regex_entry(template):
 		return re.match(template_name, entry_name) and (template_type == entry_type or not template_type)
 	else:
 		return template_name == entry_name and (template_type == entry_type or not template_type)
 
 
-def match_entry_sequence(i_e, entry_list, sequence_list):
-	"""
-	If the entry at index `i_e` in `entry_list` matches the first entry in `sequence_list`, and the entry at index `i_e+1`
-	in `entry_list` matches the second entry in `sequence_list`, and so on, then return `True`. Otherwise, return `False`
-	
-	:param i_e: the index of the entry in the entry list that we're currently looking at
-	:param entry_list: a list of entries, each entry is a list of words
-	:param sequence_list: a list of strings, each of which is a sequence of characters
-	:return: A boolean value.
-	"""
-	if (i_e + len(sequence_list)) > len(entry_list):
-		return False
-	for i_s in range(len(sequence_list)):
-		if not match_entry(entry_list[i_e + i_s], sequence_list[i_s]):
-			return False
-	return True
-
-
-def find_entry_sequence_after(i_e, entry_list, sequence_list):
-	"""
-	> Find the index of the first entry in the entry list that matches the sequence list, starting at index i_e
-	
-	:param i_e: the index of the entry in the entry list
-	:param entry_list: a list of entries
-	:param sequence_list: a list of sequences, each sequence is a list of entries
-	:return: The index of the first entry in the entry list that matches the sequence list.
-	"""
-	while i_e < len(entry_list):
-		if match_entry_sequence(i_e, entry_list, sequence_list):
-			return i_e
-		else:
-			i_e += 1
-	return -1
-
-
-def match_entry_list(entry_list, template_list):
+def match_entry_list(l1, l2):
 	"""
 	It takes an entry list and a template list, and returns True if the entry list matches the template list
-	
-	:param entry_list: entry list of one of the elements found in descendants
-	:param template_list: list of the entries of the element pattern (already completed with UIPath)
+
+	:param l1: the entry list of an element
+	:param l2: the template list (already completed with UIPath)
 	:return: True if the entry list matches the template list.
 	"""
-	
-	try:
-		# print("match_entry_list: entry_list: " + str(entry_list) + " template_list: " + str(template_list))
-		# using list comprehension + zip() + slicing + enumerate()
-		# Split list into lists by particular value
-		size = len(template_list)
-		idx_list = [idx + 1 for idx, val in enumerate(template_list) if val == '*']
-		if idx_list:
-			res = [template_list[i: j] for i, j in zip([0] + idx_list, idx_list + ([size] if idx_list[-1] != size else []))]
-			# Debug trace: print("The index list after splitting by a value : " + str(idx_list))
-			# Debug trace: print("The list after splitting by a value : " + str(res))
-			for sequence_list in res:
-				if sequence_list[-1] == '*':
-					del sequence_list[-1]
-		else:
-			res = [template_list]
-		# print("The template list after splitting by ->*-> : " + str(res))
-		i_e = 0
-		if not match_entry_sequence(i_e, entry_list, res[0]):
-			return False
-		# print("The first sequence is matched: " + str(res[0]))
-		i_e += len(res[0])
-		res.pop(0)
-		for sequence_t in res:
-			i_e = find_entry_sequence_after(i_e, entry_list, sequence_t)
-			if i_e == -1:
-				# print("The sequence is not matched: " + str(sequence_t))
-				return False
-			# print("The sequence is matched: " + str(sequence_t))
-			i_e = i_e + len(sequence_t)
-		if i_e != len(entry_list):
-			return False
-		
-		return True
-	except Exception as e:
-		print("match_entry_list exception: " + str(e))
+	if (l1 == []):
+		return (l2 == [] or l2 == ['*'])
+	if (l2 == [] or l2[0] == '*'):
+		return match_entry_list(l2, l1)
+	if (l1[0] == '*'):
+		return (match_entry_list(l1, l2[1:]) or match_entry_list(l1[1:], l2))
+	if is_regex_entry(l1[0]):
+		if match_entry(l2[0], l1[0]):
+			return match_entry_list(l1[1:], l2[1:])
+	elif match_entry(l1[0], l2[0]):
+		return match_entry_list(l1[1:], l2[1:])
+	else:
 		return False
 
 
 def is_filter_criteria_ok(child, min_height=8, max_height=200, min_width=8, max_width=800):
 	"""
 	"Return True if the child is visible and its height and width are within the specified ranges."
 	
@@ -395,64 +341,75 @@
 	else:
 		window_candidates = list(filter(
 			lambda w: not any(substr in w.element_info.name for substr in core_settings.window_filtering.ignore_windows),
 			window_candidates))
 	return window_candidates
 
 
-@func.ttl_cache(ttl=10)
+def find_ocr_elements(ocr_text, window, entry_list):
+	entry_list = entry_list[:-1]
+	title, control_type, _, _ = get_entry(entry_list[-1])
+	while entry_list[-1] == '*':
+		entry_list = entry_list[:-1]
+		title, control_type, _, _ = get_entry(entry_list[-1])
+	descendants = window.descendants(title=title, control_type=control_type)
+	candidates = list(filter(lambda e: match_entry_list(get_entry_list(get_wrapper_path(e)), entry_list), descendants))
+	ocr_candidates = []
+	if not candidates:
+		candidates = [window]
+	for wrapper in candidates:
+		results = find_all_ocr(wrapper)
+		for r in results:
+			if fuzz.partial_ratio(ocr_text, r[1]) > 90:
+				ocr_candidates.append(OCRWrapper(r))
+	perfect_candidate = [ocr_candidate for ocr_candidate in ocr_candidates if ocr_candidate.result[1] == ocr_text]
+	if len(perfect_candidate) == 1:
+		return perfect_candidate
+	return ocr_candidates
+
+
 def find_elements(full_element_path=None, visible_only=True, enabled_only=True, active_only=True):
 	"""
-	It takes an entry list and returns the unique element that matches the entry list
+	It takes an entry list and returns the elements that matche the entry list
 
 	:param full_element_path: full path of the element(s) to find
 	:param visible_only: If True, only visible elements are returned, defaults to True (optional)
 	:param enabled_only: If True, only enabled controls are returned, defaults to True (optional)
 	:param active_only: If True, only active windows are considered, defaults to True (optional)
-	:return: The element and the list of candidates
+	:return: The elements found
 	"""
-	# t0 = time.time()
 	entry_list = get_entry_list(full_element_path)
-	window_candidates = find_window_candidates(entry_list[0],
-	                                           visible_only=visible_only, enabled_only=enabled_only,
+	window_candidates = find_window_candidates(entry_list[0], visible_only=visible_only, enabled_only=enabled_only,
 	                                           active_only=active_only)
 	if window_candidates is None:
-		return None, []
-	
+		return []
 	window_candidates = filter_window_candidates(window_candidates)
-	
 	if len(entry_list) == 1 and len(window_candidates) == 1:
-		return window_candidates[0], []
+		return [window_candidates[0]]
 
 	candidates = []
+	title, control_type, _, _ = get_entry(entry_list[-1])
 	for window in window_candidates:
-		title, control_type, _, _ = get_entry(entry_list[-1])
 		if is_regex_entry(entry_list[-1]):
-			eis = findwindows.find_elements(title_re=title, control_type=control_type,
-			                                backend="uia", parent=window, top_level_only=False)
+			eis = findwindows.find_elements(title_re=title, control_type=control_type, backend="uia", parent=window, top_level_only=False)
 			descendants = [UIAWrapper(ei) for ei in eis]
-			candidates += filter(lambda e: match_entry_list(get_entry_list(get_wrapper_path(e)),
-			                                                entry_list), descendants)
+			candidates += filter(lambda e: match_entry_list(get_entry_list(get_wrapper_path(e)), entry_list), descendants)
 		else:
-			descendants = window.descendants(title=title,
-			                                 control_type=control_type)  # , depth=max(1, len(entry_list)-2)
-			candidates += filter(lambda e: match_entry_list(get_entry_list(get_wrapper_path(e)),
-			                                                entry_list), descendants)
-	
+			if control_type == "OCR_Text":
+				candidates += find_ocr_elements(title, window, entry_list)
+			else:
+				descendants = window.descendants(title=title, control_type=control_type)  # , depth=max(1, len(entry_list)-2)
+				candidates += filter(lambda e: match_entry_list(get_entry_list(get_wrapper_path(e)), entry_list), descendants)
 	if not candidates:
 		if active_only:
 			return find_elements(full_element_path, visible_only=True, enabled_only=False, active_only=False)
 		else:
-			return None, []
-	elif len(candidates) == 1:
-		#t1 = time.time()
-		#print("duration: ", t1 - t0)
-		return candidates[0], []
+			return []
 	else:
-		return None, candidates
+		return candidates
 
 
 # The following code should be called in recoder.py because it's useful only when recording
 def read_config_file():
 	"""
 	It reads the configuration file and stores the settings in the global variable `core_settings`
 	"""
```

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/element_observer.py` & `pywinauto_recorder-0.6.6/pywinauto_recorder/element_observer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import overlay_arrows_and_more as oaam
 from pywinauto_recorder.core import path_separator, get_wrapper_path, get_entry
 from pywinauto import Desktop
 from win32api import GetSystemMetrics, GetCursorPos
 from time import sleep
 from multiprocessing import Process, Event
 from pywinauto_recorder.recorder import IconSet, _find_common_path, _overlay_add_mode_icon
-
+import traceback
 
 wrapper_old_info_tip = None
 common_path_info_tip = ''
 
 
 def _display_info_tiptool(desktop, info_overlay, screen_width):
 	global wrapper_old_info_tip
 	global common_path_info_tip
 	tooltip_width = 500
 	tooltip_height = 25
 	
 	x, y = GetCursorPos()
-	wrapper = desktop.from_point(x,y)
+	wrapper = desktop.from_point(x, y)
 	
 	if wrapper is None:
 		return
 	
 	common_path_info_tip = ''
 	parent_wrapper = None
 	if wrapper != wrapper_old_info_tip:
@@ -54,20 +54,21 @@
 	text = ''
 	text_width = 0
 	for c in common_path_info_tip:
 		if c == '\n':
 			text_width = 0
 			tooltip_height = tooltip_height + 16
 		else:
-			text_width = text_width + 6.8
+			text_width = text_width + 7.8
 		text = text + c
 		if text_width > tooltip_width:
 			text = text + '\n'
 			text_width = 0
 			tooltip_height = tooltip_height + 16
+	text = common_path_info_tip # TEST
 	
 	tooltip2_height = tooltip_height
 	text2 = ''
 	text_width = 0
 	for c in end_path:
 		if c == '\n':
 			text_width = 0
@@ -75,14 +76,16 @@
 		else:
 			text_width = text_width + 6.8
 		text2 = text2 + c
 		if text_width > tooltip_width:
 			text2 = text2 + '\n'
 			text_width = 0
 			tooltip2_height = tooltip2_height + 16
+	text2 = end_path # TEST
+
 	if x > screen_width / 2:
 		info_left = 9
 	else:
 		info_left = screen_width - tooltip_width - 10
 	info_top = 150
 
 	_overlay_add_mode_icon(info_overlay, IconSet.hicon_search, info_left, info_top - 54)
@@ -90,27 +93,27 @@
 	info_overlay.add(
 		geometry=oaam.Shape.rectangle, x=info_left, y=info_top - 2, width=tooltip_width, height=tooltip_height,
 		thickness=1, color=(0, 0, 0), brush=oaam.Brush.solid, brush_color=(222, 254, 255))
 	info_overlay.add(
 		x=info_left + 5, y=info_top + 1, width=tooltip_width - 7,
 		height=tooltip_height - 5,
 		text=text,
-		text_format="win32con.DT_LEFT|win32con.DT_TOP|win32con.DT_WORDBREAK|win32con.DT_NOCLIP|win32con.DT_VCENTER",
+		text_format="win32con.DT_LEFT|win32con.DT_WORDBREAK|win32con.DT_EXPANDTABS|win32con.DT_EDITCONTROL|win32con.DT_NOCLIP",
 		font_size=16, text_color=(255, 0, 255), brush=oaam.Brush.solid, brush_color=(222, 254, 255),
 		geometry=oaam.Shape.rectangle, thickness=0
 	)
 	info_overlay.add(
 		geometry=oaam.Shape.rectangle, x=info_left, y=info_top - 2 + tooltip_height,
 		width=tooltip_width, height=tooltip2_height,
 		thickness=1, color=(0, 0, 0), brush=oaam.Brush.solid, brush_color=(180, 254, 255))
 	info_overlay.add(
 		x=info_left + 5, y=info_top + tooltip_height, width=tooltip_width - 7,
 		height=tooltip_height - 5,
 		text=text2,
-		text_format="win32con.DT_LEFT|win32con.DT_TOP|win32con.DT_WORDBREAK|win32con.DT_NOCLIP|win32con.DT_VCENTER",
+		text_format="win32con.DT_LEFT | win32con.DT_WORDBREAK | win32con.DT_EXPANDTABS | win32con.DT_EDITCONTROL|win32con.DT_NOCLIP",
 		font_size=16, text_color=(0, 0, 255), brush=oaam.Brush.solid, brush_color=(180, 254, 255),
 		geometry=oaam.Shape.rectangle, thickness=0
 	)
 	
 	text = ""
 	try:
 		has_get_value = getattr(wrapper, "get_value", None)
@@ -160,44 +163,51 @@
 		else:
 			text_width = text_width + 6.8
 		text3 = text3 + c
 		if text_width > tooltip_width:
 			text3 = text3 + '\n'
 			text_width = 0
 			tooltip3_height = tooltip3_height + 16
+	text3 = text
 	if text3:
 		info_overlay.add(
 			geometry=oaam.Shape.rectangle, x=info_left, y=info_top - 4 + tooltip_height + tooltip2_height,
 			width=tooltip_width,
 			height=tooltip3_height, thickness=1, color=(0, 0, 0), brush=oaam.Brush.solid, brush_color=(2, 254, 255))
 		info_overlay.add(
 			x=info_left + 5, y=info_top + tooltip_height + tooltip2_height, width=tooltip_width - 7,
 			height=tooltip3_height - 5,
 			text=text3,
-			text_format="win32con.DT_LEFT|win32con.DT_TOP|win32con.DT_WORDBREAK|win32con.DT_NOCLIP|win32con.DT_VCENTER",
+			text_format="win32con.DT_LEFT|win32con.DT_WORDBREAK|win32con.DT_EXPANDTABS|win32con.DT_EDITCONTROL|win32con.DT_NOCLIP",
 			font_size=16, text_color=(0, 0, 0), brush=oaam.Brush.solid, brush_color=(2, 254, 255),
 			geometry=oaam.Shape.rectangle, thickness=0
 		)
 	info_overlay.refresh()
 
 
 def task(info_mode_event, info_mode_quit_event):
+	global wrapper_old_info_tip
+	global common_path_info_tip
 	screen_width = GetSystemMetrics(0)
 	info_overlay = oaam.Overlay(transparency=0.0)
 	desktop = Desktop(backend='uia', allow_magic_lookup=False)
 	while not info_mode_quit_event.is_set():
-		if info_mode_event.is_set():
-			try:
-				_display_info_tiptool(desktop, info_overlay, screen_width)
-			except:
-				pass
-		else:
+		try:
+			if info_mode_event.is_set():
+					_display_info_tiptool(desktop, info_overlay, screen_width)
+			else:
+				info_overlay.clear_all()
+				info_overlay.refresh()
+			sleep(0.1)
+		except:
+			wrapper_old_info_tip = None
+			common_path_info_tip = ''
 			info_overlay.clear_all()
 			info_overlay.refresh()
-		sleep(0.1)
+			sleep(2.0)
 	info_overlay.clear_all()
 	info_overlay.refresh()
 	info_overlay.quit()
 
 
 class ElementInfoTooltip:
 	def __init__(self):
```

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/player.py` & `pywinauto_recorder-0.6.6/pywinauto_recorder/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """This module contains functions to replay a sequence of user actions automatically."""
 
 # print('__file__={0:<35} | __name__={1:<20} | __package__={2:<20}'.format(__file__, __name__, str(__package__)))
 from enum import Enum
 from typing import Optional, Union, NewType
 import time
 import re
+import pathlib
 import pywinauto
 from win32api import GetCursorPos as win32api_GetCursorPos
 from win32api import GetSystemMetrics as win32api_GetSystemMetrics
 from win32api import mouse_event as win32api_mouse_event
 from win32gui import LoadCursor as win32gui_LoadCursor
 from win32gui import GetCursorInfo as win32gui_GetCursorInfo
 from win32con import IDC_WAIT, MOUSEEVENTF_MOVE, MOUSEEVENTF_ABSOLUTE, MOUSEEVENTF_LEFTDOWN, MOUSEEVENTF_LEFTUP, \
 	MOUSEEVENTF_MIDDLEDOWN, MOUSEEVENTF_MIDDLEUP, MOUSEEVENTF_RIGHTDOWN, MOUSEEVENTF_RIGHTUP, MOUSEEVENTF_WHEEL, \
 	WHEEL_DELTA
 from .core import type_separator, path_separator, get_entry, get_entry_list, find_elements, get_sorted_region, \
-	get_wrapper_path, is_int
-from functools import partial, update_wrapper, lru_cache
+	get_wrapper_path, is_int, is_absolute_path
+from functools import partial, update_wrapper
+from cachetools import func
 import math
+from .ocr_wrapper import OCRWrapper
 
 
 UI_Coordinates = NewType('UI_Coordinates', (float, float))
 UI_Path = str
 PYWINAUTO_Wrapper = pywinauto.controls.uiawrapper.UIAWrapper
 UI_Selector = Union[UI_Path, PYWINAUTO_Wrapper, UI_Coordinates]
 
 
 class PywinautoRecorderException(Exception):
 	"""Base class for other exceptions."""
-	pass
+	...
 
 
 class FailedSearch(PywinautoRecorderException):
 	"""FailedSearch is a subclass of *PywinautoRecorderException* that is raised when a search for a control fails."""
-	pass
+	...
 
 
 __all__ = ['PlayerSettings', 'MoveMode', 'ButtonLocation', 'load_dictionary', 'shortcut', 'full_definition', 'UIPath',
            'Window', 'Region', 'find', 'find_all', 'move', 'click', 'left_click', 'right_click',
            'double_left_click', 'triple_left_click', 'double_click', 'triple_click',
            'drag_and_drop', 'middle_drag_and_drop', 'right_drag_and_drop', 'menu_click',
            'mouse_wheel', 'send_keys', 'set_combobox', 'set_text', 'exists', 'select_file', 'playback',
@@ -50,39 +53,48 @@
 		string = string.replace(*r)
 	return string
 
 
 class PlayerSettings:
 	"""The player settings class contains the default settings."""
 	
+	typing_pause = 0.1
+	"""The pause time between characters typed"""
+	
 	mouse_move_duration = 0.5
 	"""Mouse move duration (in seconds)."""
 	
 	timeout = 10
 	"""Maximum duration (in seconds) to wait for the :func:`find` function to search an element before giving up.
 	If the element is not found after the given timeout, the search is interrupted."""
 
 	use_cache = True
 	"""If True, the :func:`find` function caches the results of the search.
 	This is useful if the search is called several times on the same element."""
 	
 	@staticmethod
-	def _apply_settings(mouse_move_duration: Optional[float] = None, timeout: Optional[float] = None) -> dict:
+	def _apply_settings(
+			typing_pause: Optional[float] = None,
+			mouse_move_duration: Optional[float] = None,
+			timeout: Optional[float] = None) -> dict:
 		"""
 		If the duration and timeout arguments are None, set them to the default values.
 		
+		:param typing_duration: The pause time between characters typed
 		:param mouse_move_duration: The duration of the mouse movement
 		:param timeout: The maximum duration to wait for the :func:`find` function to find an element before giving up
 		:return: The duration and timeout are being returned.
 		"""
+		if typing_pause is None:
+			typing_pause = PlayerSettings.typing_pause
 		if mouse_move_duration is None:
 			mouse_move_duration = PlayerSettings.mouse_move_duration
 		if timeout is None:
 			timeout = PlayerSettings.timeout
-		return {"mouse_move_duration": mouse_move_duration, "timeout": timeout}
+		return {"typing_pause": typing_pause, "mouse_move_duration": mouse_move_duration, "timeout": timeout}
 
 
 class MoveMode(Enum):
 	"""The MoveMode class is an enumeration of the different ways that the mouse can move."""
 	
 	linear = 0
 	"""The mouse cursor moves in a straight line from the start point to the end point with a constant speed."""
@@ -238,15 +250,15 @@
 
 		:param element_path: Optional[UI_Path] = None
 		:type element_path: Optional[UI_Path]
 		:return: The full path of the element.
 		"""
 		if element_path is None or element_path == "":
 			return path_separator.join(UIPath._path_list)
-		elif UIPath._path_list:
+		elif UIPath._path_list and not is_absolute_path(element_path):
 			return path_separator.join(UIPath._path_list) + path_separator + element_path
 		else:
 			return element_path
 	
 	def __init__(self, relative_path=None, regex_title=False):
 		self.relative_path = relative_path
 		self.regex_title = regex_title  # UIPath._regex_list must be removed
@@ -270,15 +282,15 @@
 def find_cache_clear():
 	"""
 	Clears the cache of the :func:`find` function.
 	"""
 	_cached_find.cache_clear()
 
 
-@lru_cache(maxsize=128)
+@func.ttl_cache(ttl=60)
 def _cached_find(
 		full_element_path: Optional[UI_Selector] = None,
 		timeout: Optional[float] = None) -> PYWINAUTO_Wrapper:
 	"""
 	Finds the element defined by the full_element_path.
 	
 	full_element_path must not contain the relative coordinates.
@@ -287,78 +299,81 @@
 
 
 def _find(
 		full_element_path: Optional[UI_Selector] = None,
 		timeout: Optional[float] = None) -> PYWINAUTO_Wrapper:
 	"""
 	Finds the element defined by the full_element_path.
+	
+	When the [] operator is used and only one element is found, the row and column indices are not tested and the element is returned.
 	"""
 	_, _, y_x, _ = get_entry(get_entry_list(full_element_path)[-1])
-	unique_element = None
-	elements = None
+	elements = []
 	t0 = time.time()
 	while (time.time() - t0) < timeout:
-		while (not y_x and unique_element is None and not elements) or (y_x and unique_element is None and not elements):
+		while not elements:
+			if (time.time() - t0) > timeout:
+				msg = "No element found with the UIPath '" + full_element_path + "' after " + str(timeout) + " s of searching."
+				raise FailedSearch(msg)
 			try:
-				# print("find_element(...): ")
-				unique_element, elements = find_elements(full_element_path)
-				if (not y_x and unique_element is None and not elements) or (y_x and unique_element is None and not elements):
+				elements = find_elements(full_element_path)
+				if not elements:
+					#print("🔴", end="")
 					time.sleep(2.0)
 			except Exception:
+				#print("🟢", end="")
 				pass
-			if (time.time() - t0) > timeout:
-				msg = "No element found with the UIPath '" + full_element_path + "' after " + str(timeout) + " s of searching."
-				raise FailedSearch(msg)
+
+		if len(elements) == 1:
+				return elements[0]
 		
 		if y_x is not None:
-			if unique_element:
-				return unique_element   # TODO: remove this test and replace (unique_element, elements) by elements in all the code of all modules
+			nb_y, _, candidates = get_sorted_region(elements)
+			if is_int(y_x[0]):
+				return candidates[int(y_x[0])][int(y_x[1])]
 			else:
-				nb_y, nb_x, candidates = get_sorted_region(elements)
-				if is_int(y_x[0]):
-					unique_element = candidates[int(y_x[0])][int(y_x[1])]
-				else:
-					full_smart_element_path = UIPath.get_full_path(y_x[0])
-					ref_unique_element, _ = find_elements(full_smart_element_path)
-					if not ref_unique_element:
-						msg = "No element found with the UIPath '" + full_smart_element_path + "' in the array line."
-						raise FailedSearch(msg)
-					ref_r = ref_unique_element.rectangle()
-					r_y = 0
-					while r_y < nb_y:
-						for candidate in candidates[r_y]:
-							y_candidate = candidate.rectangle().mid_point()[1]
-							if ref_r.top < y_candidate < ref_r.bottom:
-								unique_element = candidates[r_y][y_x[1]]
-								return unique_element
-						r_y = r_y + 1
-		if unique_element is not None:
-			break
+				full_smart_element_path = UIPath.get_full_path(y_x[0])
+				ref_unique_element = find_elements(full_smart_element_path)
+				if len(ref_unique_element) > 1:
+					msg = "No element found with the UIPath '" + full_smart_element_path + "' in the array line."
+					raise FailedSearch(msg)
+				ref_r = ref_unique_element[0].rectangle()
+				r_y = 0
+				while r_y < nb_y:
+					for candidate in candidates[r_y]:
+						y_candidate = candidate.rectangle().mid_point()[1]
+						if ref_r.top < y_candidate < ref_r.bottom:
+							return candidates[r_y][y_x[1]]
+					r_y = r_y + 1
 		time.sleep(0.1)
-	if not unique_element:
-		if elements:
-			message = "There are " + str(len(elements)) + " elements that match the path '" + full_element_path + "':"
-			for e in elements:
+
+	if len(elements) > 1:
+		message = "There are " + str(len(elements)) + " undiscriminated elements that match the path '" + full_element_path + "':"
+		for e in elements:
+			if isinstance(e, OCRWrapper):
+				message += "\n" + str(e.result)
+			else:
 				message += "\n" + get_wrapper_path(e)
-			raise FailedSearch(message)
-		raise FailedSearch("Unique element not found using path '", full_element_path + "'")
-	return unique_element
+		raise FailedSearch(message)
+	raise FailedSearch("Unique element not found using path '", full_element_path + "'")
 
 
 def find(
 		element_path: Optional[UI_Selector] = None,
 		regex: bool = False,
 		timeout: Optional[float] = None) -> PYWINAUTO_Wrapper:
 	"""
 	Finds the element matching element_path.
 	
 	This function is called in all the other functions (:func:`click`, :func:`move`, ...) that require to search an element.
 	To significantly increase search performance, the user can enable a cache with 'Player.Setting.use_cache = True'.
 	When the cache is active, it is sometimes necessary to empty it with the :func:`find_cache_clear` function.
 
+	When the [] operator is used and only one element is found, the row and column indices are not tested and the element is returned.
+
 	.. code-block:: python
 		:caption: Example of code using the 'find' function::
 		:emphasize-lines: 3,3
 		
 		from pywinauto_recorder.player import UIPath, find
 		with UIPath("RegEx: .* Google Chrome$||Pane"):
 			find().set_focus()  # Set focus to the Google Chrome window.
@@ -441,30 +456,28 @@
 	entry_list = get_entry_list(full_element_path)
 	_, _, y_x, _ = get_entry(entry_list[-1])
 	if y_x:
 		return find(element_path, timeout=timeout)
 	t0 = time.time()
 	while (time.time() - t0) < timeout:
 		try:
-			unique_element, elements = find_elements(full_element_path)
-			if unique_element:
-				return [unique_element]
+			elements = find_elements(full_element_path)
 			if elements:
 				return elements
 			time.sleep(2.0)
 		except Exception:
 			pass
 		time.sleep(0.1)
 	msg = "No element found with the UIPath '" + full_element_path + "' after " + str(timeout) + " s of searching."
 	raise FailedSearch(msg)
 
 
 def _move(x, y, xd, yd, duration=1, refresh_rate=25):
 	"""
-	It moves the mouse from (x, y) to (xd, yd) in a straight line, with a duration of `duration` seconds.
+	It moves the mouse from (x, y) to (xd, yd) in a straight line, with a duration of duration seconds.
 	
 	:param x: The x-coordinate of the mouse cursor before the move
 	:param y: The y-coordinate of the mouse cursor before the move
 	:param xd: The x-coordinate of the mouse cursor after the move
 	:param yd: The y-coordinate of the mouse cursor after the move
 	:param duration: The time (in seconds) it takes to move the mouse from (x, y) to (xd, yd)
 	:param refresh_rate: 25 Hz is the default refresh rate of the mouse move
@@ -509,15 +522,22 @@
 	"""
 	duration = PlayerSettings._apply_settings(mouse_move_duration=duration)["mouse_move_duration"]
 	if duration == -1:
 		return
 	
 	if element_path is None or isinstance(element_path, str):
 		unique_element = find(element_path, timeout=timeout)
-		w_r = unique_element.rectangle()
+		try:
+			w_r = unique_element.rectangle()
+		except Exception:
+			#with _cached_find.cache_lock:
+			#	_cached_find.cache.pop(_cached_find.cache_key(element_path, timeout=timeout), None)
+			find_cache_clear()
+			unique_element = find(element_path, timeout=timeout)
+			w_r = unique_element.rectangle()
 		xd, yd = w_r.mid_point()
 		if element_path:
 			_, _, _, dx_dy = get_entry(get_entry_list(element_path)[-1])
 			if dx_dy:
 				dx, dy = dx_dy
 				xd, yd = round(xd + dx/100.0*(w_r.width()/2-1), 0), round(yd + dy/100.0*(w_r.height()/2-1), 0)
 	elif isinstance(element_path, pywinauto.base_wrapper.BaseWrapper):
@@ -603,18 +623,28 @@
 		has_get_value = getattr(wrapper, "click", None)
 		if callable(has_get_value):
 			wrapper.click()
 		else:
 			wrapper.click_input()
 		return wrapper
 	else:
-		wrapper = move(element_path, duration=duration, mode=mode, timeout=timeout)
-		if wait_ready and wrapper:
+		
+		
+		if wait_ready and \
+			(element_path is None or isinstance(element_path, str) or isinstance(element_path, pywinauto.base_wrapper.BaseWrapper)):
+			use_cache_old = PlayerSettings.use_cache
+			PlayerSettings.use_cache = False
+			if isinstance(element_path, pywinauto.base_wrapper.BaseWrapper):
+				wrapper = element_path
+			else:
+				wrapper = move(element_path, duration=duration, mode=mode, timeout=timeout)
 			wait_is_ready_try1(wrapper, timeout=timeout)
-
+			PlayerSettings.use_cache = use_cache_old
+		else:
+			wrapper = move(element_path, duration=duration, mode=mode, timeout=timeout)
 	_win32api_mouse_click(button, click_count)
 	return wrapper
 
 
 def wrapped_partial(func, *args, **kwargs):
 	partial_func = partial(func, *args, **kwargs)
 	update_wrapper(partial_func, func)
@@ -675,15 +705,16 @@
 middle_drag_and_drop = wrapped_partial(drag_and_drop, button=ButtonLocation.middle)
 right_drag_and_drop = wrapped_partial(drag_and_drop, button=ButtonLocation.right)
 
 
 def menu_click(
 		menu_path: str,
 		duration: Optional[float] = None,
-		timeout: Optional[float] = None) -> PYWINAUTO_Wrapper:
+		timeout: Optional[float] = None,
+		absolute_path = False) -> PYWINAUTO_Wrapper:
 	"""
 	Clicks on the menu items.
 	
 	.. code-block:: python
 		:caption: Example of code using the 'menu_click' function to automate 'Notepad++'::
 		:emphasize-lines: 5,5
 		
@@ -700,17 +731,15 @@
 		from pywinauto_recorder.player import UIPath, find, click, menu_click
 		
 		with UIPath("Document - WordPad||Window"):
 			find().set_focus()
 			click("*->File tab||Button")
 			menu_click("New")
 			
-	In the above code, the 'File tab' element that opens the menu is not of type 'MenuItem',
-	so it is not possible to call 'menu_click("File tab->New")'.
-	In this case the menu must be opened with 'click("*->File tab||Button")' before calling :func:`menu_click`.
+	In the above code, the 'File tab' element that opens the menu is not of type 'MenuItem', so it is not possible to call 'menu_click("File tab->New")'. In this case the menu must be opened with 'click("*->File tab||Button")' before calling :func:`menu_click`.
 	
 	:param menu_path: menu item path
 	:param duration: duration in seconds of the mouse move (it doesn't take into account the time it takes to find)
 		(if duration is -1 the mouse cursor doesn't move, it just sends WM_CLICK window message,
 		useful for minimized or non-active window).
 	:param timeout: period of time in seconds that will be allowed to find the element
 	:return: Pywinauto wrapper of the clicked item
@@ -735,20 +764,21 @@
 	def distance(pt_1, pt_2):
 		return math.hypot(pt_2[0] - pt_1[0], pt_2[1] - pt_2[1])
 	
 	if duration not in [None, -1]:
 		duration = float(duration)/2
 		
 	menu_entry_list = menu_path.split(path_separator)
+	str_menu_item = 'MenuItem~Absolute_UIPath' if absolute_path else 'MenuItem'
 	for i, menu_entry in enumerate(menu_entry_list):
 		if i > 0:
 			SAV_UIPath_path_list, SAV_UIPath_regex_list = UIPath._path_list, UIPath._regex_list
 			UIPath._path_list = UIPath._regex_list = []
 		mouse_cursor_pos = win32api_GetCursorPos()
-		ws = find_all('*' + path_separator + menu_entry + type_separator + 'MenuItem', timeout=timeout)
+		ws = find_all('*' + path_separator + menu_entry + type_separator + str_menu_item, timeout=timeout)
 		ws.sort(key=lambda w: distance(w.rectangle().mid_point(), mouse_cursor_pos))
 		w = ws[0]
 		item_pos = w.rectangle().mid_point()
 		r = w.parent().rectangle()
 		nearest_p_point = nearest_perimeter_point(r, mouse_cursor_pos)
 		move(nearest_p_point, duration=duration)
 		click(item_pos, duration=duration)
@@ -774,15 +804,15 @@
 			else:
 				win32api_mouse_event(MOUSEEVENTF_WHEEL, 0, 0, -WHEEL_DELTA, 0)
 			time.sleep(pause)
 
 
 def send_keys(
 		str_keys: str,
-		pause: float = 0.1,
+		pause: Optional[float] = None,
 		with_spaces: bool = True,
 		with_tabs: bool = True,
 		with_newlines: bool = True,
 		turn_off_numlock: bool = True,
 		vk_packet: bool = True) -> None:
 	"""
 	Parses the keys and type them
@@ -793,19 +823,21 @@
 	:param pause: pause in seconds between each typed key
 	:param with_spaces: if False spaces are not taken into account
 	:param with_tabs: if False tabs are not taken into account
 	:param with_newlines: if False newlines are not taken into account
 	:param turn_off_numlock: if True numlock is turned off
 	:param vk_packet: For Windows only, pywinauto defaults to sending a virtual key packet (VK_PACKET) for textual input
 	"""
+	typing_pause = PlayerSettings._apply_settings(typing_pause=pause)["typing_pause"]
+	
 	for r in (('(', '{(}'),  (')', '{)}'), ('+', '{+}')):
 		str_keys = str_keys.replace(*r)
 	pywinauto.keyboard.send_keys(   # lgtm [py/call/wrong-named-argument]
 		str_keys,
-		pause=pause,
+		pause=typing_pause,
 		with_spaces=with_spaces,
 		with_tabs=with_tabs,
 		with_newlines=with_newlines,
 		turn_off_numlock=turn_off_numlock,
 		vk_packet=vk_packet
 	)
 
@@ -836,32 +868,33 @@
 
 def set_text(
 		element_path: UI_Selector,
 		value: str,
 		duration: Optional[float] = None,
 		mode: Enum = MoveMode.linear,
 		timeout: Optional[float] = None,
-		pause: float = 0.1) -> None:
+		pause: float = None) -> None:
 	"""
 	Sets the value of a text field.
 	
 	:param element_path: element path
 	:param value: value of the combobox
 	:param duration: duration in seconds of the mouse move (it doesn't take into account the time it takes to find)
 		(if duration is -1 the mouse cursor doesn't move, it just sends WM_CLICK window message,
 		useful for minimized or non-active window).
 	:param mode: move mouse mode: MoveMode.linear, MoveMode.x_first, MoveMode.y_first
 	:param timeout: period of time in seconds that will be allowed to find the element
 	:param pause: pause in seconds between each typed key
 	:raises FailedSearch: if the element is not found
 	"""
+	typing_pause = PlayerSettings._apply_settings(typing_pause=pause)["typing_pause"]
 	double_left_click(element_path, duration=duration, mode=mode, timeout=timeout)
 	send_keys("{VK_CONTROL down}a{VK_CONTROL up}", pause=0)
 	time.sleep(0.1)
-	send_keys(value + "{ENTER}", pause=pause)
+	send_keys(value + "{ENTER}", pause=typing_pause)
 
 
 def exists(
 		element_path: UI_Selector,
 		timeout: Optional[float] = None) -> PYWINAUTO_Wrapper:
 	"""
 	Tests if the user interface element exists. It returns the element if it exists, None otherwise.
@@ -895,29 +928,34 @@
 		
 		select_file("Document - WordPad||Window->Open||Window", "Documents/file.txt")
 	
 	To make this code work, you must first launch 'WordPad' and click on 'File->Open'.
 
 	:param window_path: window path of the file dialog (e.g. "Untitled - Paint||Window->Save As||Window"
 	:param full_path: the full path of the file to select
-	:param force_slow_path_typing: if True it will type the path even if the current path of the dialog box is the same
-	as the file to select
+	:param force_slow_path_typing: if True it will type the path even if the current path of the dialog box is the same as the file to select
 	:raises FailedSearch: if an element is not found
 	"""
-	import pyperclip
-	import pathlib
 	p = pathlib.Path(full_path)
 	folder = p.parent
 	filename = p.name
 	with UIPath(window_path):
 		find().set_focus()
 		click("*->All locations||SplitButton")
 	if not force_slow_path_typing:
-		send_keys("{VK_CONTROL down}c{VK_CONTROL up}")
-	if force_slow_path_typing or pathlib.Path(pyperclip.paste()) != folder:
+		with UIPath(window_path):
+			try:
+				old_folder = find("*->Address||ComboBox->Address||Edit").get_value()
+			except Exception:
+				find_cache_clear()
+				#with _cached_find.cache_lock:
+				#	_cached_find.cache.pop(_cached_find.cache_key("*->Address||ComboBox->Address||Edit"), None)
+				old_folder = find("*->Address||ComboBox->Address||Edit").get_value()
+			
+	if force_slow_path_typing or old_folder != folder:
 		send_keys(str(folder))
 	send_keys("{ENTER}")
 	with UIPath(window_path):
 		double_left_click("*->File name:||ComboBox->File name:||Edit")
 		send_keys(filename + "{ENTER}")
 
 
@@ -939,15 +977,15 @@
 			str_code = python_file.read()
 	try:
 		script_dir = os.path.abspath(os.path.dirname(filename))
 		os.chdir(os.path.abspath(script_dir))
 		sys.path.append(script_dir)
 		compiled_code = compile(str_code, filename, 'exec')
 		exec(compiled_code)
-	except Exception as e:
+	except Exception:
 		windll.user32.ShowWindow(windll.kernel32.GetConsoleWindow(), 3)
 		exc_type, exc_value, exc_traceback = sys.exc_info()
 		output = traceback.format_exception(exc_type, exc_value, exc_traceback)
 		i_line = d_line = 0
 		full_traceback = False
 		if not full_traceback:
 			for line in output:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder/recorder.py` & `pywinauto_recorder-0.6.6/pywinauto_recorder/recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,24 @@
 import keyboard
 import mouse
 from collections import namedtuple
 import pyperclip
 import codecs
 from .core import path_separator, type_separator, Strategy, is_int, \
                     get_wrapper_path, get_entry_list, get_entry, get_sorted_region, \
-                    find_elements, read_config_file
+                    read_config_file
+from .core import find_elements as not_ttl_cached_find_elements
 from .player import playback
+from cachetools import func
+
+
+@func.ttl_cache(ttl=10)
+def find_elements(full_element_path=None, visible_only=True, enabled_only=True, active_only=True):
+	return not_ttl_cached_find_elements(full_element_path=full_element_path, visible_only=visible_only, enabled_only=enabled_only, active_only=active_only)
+
 
 __all__ = ['Recorder']
 
 ElementEvent = namedtuple('ElementEvent', ['strategy', 'rectangle', 'path'])
 SendKeysEvent = namedtuple('SendKeysEvent', ['line'])
 MouseWheelEvent = namedtuple('MouseWheelEvent', ['delta'])
 DragAndDropEvent = namedtuple('DragAndDropEvent', ['path', 'dx1', 'dy1', 'path2', 'dx2', 'dy2'])
@@ -631,17 +639,15 @@
 							continue
 						if wrapper_path2 == previous_wrapper_path2:
 							continue
 						if get_entry_list(wrapper_path2)[0] != window_title:
 							continue
 						previous_wrapper_path2 = wrapper_path2
 						
-						unique_candidate2, _ = find_elements(get_wrapper_path(wrapper2))
-						
-						if unique_candidate2 is not None:
+						if find_elements(get_wrapper_path(wrapper2)):
 							r = wrapper2_rectangle
 							self.main_overlay.add(
 								geometry=oaam.Shape.rectangle, x=r.left, y=r.top,
 								width=r.width(), height=r.height(),
 								thickness=1, color=(0, 0, 255), brush=oaam.Brush.solid,
 								brush_color=(0, 0, 255))
 							r = wrapper_rectangle
@@ -796,15 +802,14 @@
 		win32api.keybd_event(160, 0, win32con.KEYEVENTF_EXTENDEDKEY | win32con.KEYEVENTF_KEYUP, 0)
 		ev_list = keyboard.stop_recording()
 		if not ev_list and os.path.isfile(dir_path + r"\pywinauto_recorder.exe"):
 			print("Couldn't set keyboard hooks. Trying once again...\n")
 			time.sleep(0.5)
 			os.system(dir_path + r"\pywinauto_recorder.exe --no_splash_screen")
 			sys.exit(1)
-		unique_candidate = None
 		elements = []
 		i = 0
 		previous_wrapper_path = None
 		unique_wrapper_path = None
 		strategies = [Strategy.unique_path, Strategy.array_2D, Strategy.array_1D]
 		i_strategy = 0
 		self.mode = "Info"
@@ -831,75 +836,33 @@
 							i_strategy = 1
 						if i_strategy >= len(strategies):
 							i_strategy = len(strategies) - 1
 				else:
 					# strategy_unique_path_again_done = False
 					i_strategy = 0
 					previous_wrapper_path = wrapper_path
-					t0 = time.time()
-					unique_candidate, elements = find_elements(wrapper_path)
-					t1 = time.time()
-					# print("duration", t1-t0, " find_elements(" + wrapper_path + ")")
+					elements = find_elements(wrapper_path)
 				#if wrapper_path == previous_wrapper_path and unique_wrapper_path:
 				#	strategy = Strategy.unique_path_again
 				# else:
 				#	strategy = strategies[i_strategy]
 				strategy = strategies[i_strategy]
 				unique_wrapper_path = None
 				# *** ----> this block of code must start a new while iteration if mouse cursor is outside wrapper rectangle
 				# => add tests to leave if mouse cursor is outside wrapper rectangle
 				wrapper_rectangle = wrapper.rectangle()
 				
-				'''
-				# TODO: cette strategie n'est utile que pour palier à self.desktop.from_point(*cursor_pos) qui ne fn pas
-				# dans tous les cas (par exemple CMD.exe). L'autre solution est de reimplementer from_point
-				if strategy == Strategy.unique_path_again and unique_candidate and not strategy_unique_path_again_done:
-					x_new, y_new = win32api.GetCursorPos()
-					if not ((wrapper_rectangle.left < x_new < wrapper_rectangle.right) and (
-							wrapper_rectangle.top < y_new < wrapper_rectangle.bottom)):
-						i_strategy = 0
-						continue
-					better_candidates = []
-					better_father_candidates = []
-					curent_wrapper = unique_candidate.top_level_parent()
-					for curent_wrapper_child in curent_wrapper.children():
-						rect_child = curent_wrapper_child.rectangle()
-						if ((rect_child.left < x_new < rect_child.right) and (rect_child.top < y_new < rect_child.bottom)):
-							better_father_candidates.append(curent_wrapper_child)
-							
-					while better_father_candidates:
-						curent_wrapper = better_father_candidates.pop()
-						curent_wrapper_children = curent_wrapper.children()
-						if curent_wrapper_children:
-							for curent_wrapper_child in curent_wrapper_children:
-								rect_child = curent_wrapper_child.rectangle()
-								if ((rect_child.left < x_new < rect_child.right) and (
-										rect_child.top < y_new < rect_child.bottom)):
-									better_father_candidates.append(curent_wrapper_child)
-						else:
-							better_candidates.append(curent_wrapper)
-					if better_candidates:
-						better_candidates.sort(key=lambda widget: widget.rectangle().width() * widget.rectangle().height())
-						unique_candidate = better_candidates[0]
-						wrapper = unique_candidate
-						wrapper_rectangle = wrapper.rectangle()
-					strategy_unique_path_again_done = True
-				'''
-				
 				#if strategy in [Strategy.unique_path, Strategy.unique_path_again]:
 				if strategy is Strategy.unique_path:
-					'''
 					x_new, y_new = win32api.GetCursorPos()
 					if not ((wrapper_rectangle.left < x_new < wrapper_rectangle.right) and (
 							wrapper_rectangle.top < y_new < wrapper_rectangle.bottom)):
 						i_strategy = 0
 						continue
-					'''
-					if unique_candidate is not None:
-						# unique_wrapper_path = get_wrapper_path(unique_candidate)
+					if len(elements)==1:
 						unique_wrapper_path = wrapper_path
 						r = wrapper_rectangle
 						self.main_overlay.add(
 							geometry=oaam.Shape.rectangle, x=r.left, y=r.top, width=r.width(), height=r.height(),
 							thickness=1, color=(0, 128, 0), brush=oaam.Brush.solid, brush_color=(0, 255, 0))
 					else:
 						for e in elements:
@@ -969,15 +932,15 @@
 				self.main_overlay.refresh()
 				
 				loop_duration = time.time() - self._loop_t0
 				while loop_duration < 0.1:
 					time.sleep(0.01)
 					loop_duration = time.time() - self._loop_t0
 				time.sleep(0.01)  # main_overlay.clear_all() doit attendre la fin de main_overlay.refresh()
-			except Exception as e:
+			except Exception:
 				exc_type, exc_value, exc_traceback = sys.exc_info()
 				print(repr(traceback.format_exception(exc_type, exc_value, exc_traceback)))
 				self.common_path_info_tip = ""
 				self.wrapper_old_info_tip = None
 		if self.event_list:
 			self.stop_recording()
 		mouse.unhook_all()
```

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/PKG-INFO` & `pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinauto-recorder
-Version: 0.6.5
+Version: 0.6.6
 Summary: Records/Replays GUI actions
 Home-page: https://github.com/beuaaa/pywinauto_recorder
 Author: david pratmarty
 Author-email: david.pratmarty@gmail.com
 License: MIT
 Project-URL: Documentation, https://pywinauto-recorder.readthedocs.io
 Project-URL: Source, https://github.com/beuaaa/pywinauto_recorder
```

### Comparing `pywinauto_recorder-0.6.5/pywinauto_recorder.egg-info/SOURCES.txt` & `pywinauto_recorder-0.6.6/pywinauto_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywinauto_recorder-0.6.5/setup.py` & `pywinauto_recorder-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     },
     license='MIT',
     author='david pratmarty',
     author_email='david.pratmarty@gmail.com',
     description='Records/Replays GUI actions',
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    install_requires=['pywinauto', 'keyboard', 'mouse', 'overlay_arrows_and_more', 'enum34', 'pyperclip'],
+    install_requires=['pywinauto', 'keyboard', 'mouse', 'overlay_arrows_and_more', 'enum34', 'pyperclip', 'cachetools', 'thefuzz', 'Pillow'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Environment :: Win32 (MS Windows)',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

