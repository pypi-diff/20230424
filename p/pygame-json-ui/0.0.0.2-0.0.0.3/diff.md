# Comparing `tmp/pygame-json-ui-0.0.0.2.tar.gz` & `tmp/pygame-json-ui-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-json-ui-0.0.0.2.tar", last modified: Mon Apr 24 10:03:14 2023, max compression
+gzip compressed data, was "pygame-json-ui-0.0.0.3.tar", last modified: Mon Apr 24 17:37:37 2023, max compression
```

## Comparing `pygame-json-ui-0.0.0.2.tar` & `pygame-json-ui-0.0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:03:14.451739 pygame-json-ui-0.0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0     7933 2023-04-24 10:03:14.451739 pygame-json-ui-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7340 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.2/README.md
--rw-rw-rw-   0        0        0      671 2023-04-24 10:02:01.000000 pygame-json-ui-0.0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 10:03:14.451739 pygame-json-ui-0.0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 10:03:14.405573 pygame-json-ui-0.0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 10:03:14.436099 pygame-json-ui-0.0.0.2/src/pygame_json_ui.egg-info/
--rw-rw-rw-   0        0        0     7933 2023-04-24 10:03:14.000000 pygame-json-ui-0.0.0.2/src/pygame_json_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-04-24 10:03:14.000000 pygame-json-ui-0.0.0.2/src/pygame_json_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:03:14.000000 pygame-json-ui-0.0.0.2/src/pygame_json_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 10:03:14.000000 pygame-json-ui-0.0.0.2/src/pygame_json_ui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 10:03:14.451739 pygame-json-ui-0.0.0.2/src/pygame_ui/
--rw-rw-rw-   0        0        0      681 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.2/src/pygame_ui/__init__.py
--rw-rw-rw-   0        0        0     4166 2023-04-21 12:44:21.000000 pygame-json-ui-0.0.0.2/src/pygame_ui/base.py
--rw-rw-rw-   0        0        0      371 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.2/src/pygame_ui/constants.py
--rw-rw-rw-   0        0        0     4284 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.2/src/pygame_ui/elements.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9186 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8593 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/README.md
+-rw-rw-rw-   0        0        0      671 2023-04-24 17:36:24.000000 pygame-json-ui-0.0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.604939 pygame-json-ui-0.0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.652539 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/
+-rw-rw-rw-   0        0        0     9186 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 17:37:37.000000 pygame-json-ui-0.0.0.3/src/pygame_json_ui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:37:37.685185 pygame-json-ui-0.0.0.3/src/pygame_ui/
+-rw-rw-rw-   0        0        0      711 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/__init__.py
+-rw-rw-rw-   0        0        0     4566 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/base.py
+-rw-rw-rw-   0        0        0      404 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/constants.py
+-rw-rw-rw-   0        0        0     5765 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.3/src/pygame_ui/elements.py
```

### Comparing `pygame-json-ui-0.0.0.2/LICENSE` & `pygame-json-ui-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame-json-ui-0.0.0.2/PKG-INFO` & `pygame-json-ui-0.0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-Metadata-Version: 2.1
-Name: pygame-json-ui
-Version: 0.0.0.2
-Summary: Pygame UI is a package for building user interfaces for pygame in a JSON Format.
-Author-email: Xander de Haan <sissydeslang@gmail.com>
-Project-URL: Homepage, https://github.com/RednaxGaming/pygame_ui
-Project-URL: Bug Tracker, https://github.com/RednaxGaming/pygame_ui/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # Pygame UI README
 
-[Pygame UI](https://github.com/RednaxGaming/pygame_ui) is a package for building user interfaces in [pygame](https://www.pygame.org/).
+[![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+[Pygame UI](https://github.com/RednaxGaming/pygame_ui) is a package for building user interfaces for [pygame](https://www.pygame.org/) in JSON.
 
 It is currently a work in progress, but if you wanna test it out, feel free to do so :)
 
 ## Table Of Content
 
 - [Quick Start](#quick-start)
    - [Installation](#installation)
@@ -28,44 +16,53 @@
       - [JSON](#json-file)
 - [Element List](#element-list)
 - [Attribute List](#attribute-list)
    - [General](#general)
    - [Frame](#frame)
    - [Label](#label)
    - [Button](#button)
+   - [Switch](#switch)
+   - [Slider](#slider)
 - [Frames](#frames)
    - [Frame Path](#frame-path)
 - [Examples](#examples)
 - [FAQ](#faq)
 
 ## Quick Start
 
 ### Installation
 
-First of all, you'll need to manually add the pygame_ui folder to your site-packages, because the module is not yet available on pip.
+Pygame UI is available on PyPi:
+
+```shell
+pip install pygame-json-ui
+```
+In case this doesn't work, you'll need to manually add the pygame_ui folder to your site-packages.
 
 When this is done you can test your installation, by executing the following:
 ```python
 >>> import pygame_ui
 >>> pygame_ui.test()
 Successfully installed! enjoy :)
 Version: x.x.x.x
 ```
 
 ### Setup
 
 You will have two files in the same folder:
 - whatever.py
-- Interface.json <-- Specifically with that name and capitalization!
+- Interface.json <-- Name for automatically loading the file
+
+If you prefer a different name for the json file, or Pygame UI is having issues locating it automatically, you can pass the absolute path to it's parent folder as an argument for `pygame_ui.init()`.
 
 Here a simple example for making a label:
 
 #### Python File
 
-Notice that the `event_handler` is actually not required unless you want interactive elements to function as expected.
+Notice that the `event_handler` is not required unless you want interactive elements to function as expected.
 
 ```python
 import pygame
 import pygame_ui
 
 # Creating a window
 pygame.init()
@@ -91,15 +88,15 @@
    Interface.draw(screen)
 
    pygame.display.flip()
    clock.tick(60)
 ```
 
 #### JSON File
-MUST be named `Interface.json` and in the same folder as python file!
+MUST be named `Interface.json` and in the same folder as python file for loading the json file automatically!
 
 ```json
 {
    "label": {
       "name": "test_label",
       "position": [200,100],
       "size": [120,80],
@@ -113,60 +110,86 @@
 
 ## Element List
 
 All of the following items will be refered to as `elements`:
 - Frame
 - Label
 - Button
-- Switch (not implemented yet)
-- Slider (...)
-- Dropdown (...)
+- Switch
+- Slider
+- Dropdown (Coming soon)
 
 ## Attribute List
-
+- `attribute: type` description (default value).
 ### General
 These attributes can be given to any element type
-- `name: str` MUST be given to every element.
-- `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box.
-- `size: [x,y]` Sets the size of the element boundry box.
-- `background_color: (r,g,b)` The boundry box will be filled with this color. Don't set this for transparency.
-- `is_visible: bool` (default = true).
-- `is_hoverable: bool` (default = false).
-- `is_clickable: bool` (default = false).
+- `name: str` REQUIRED, used to access the element in python.
+- `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
+- `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
+- `background_color: (r,g,b)` The boundry box will be filled with this color (none).
+- `is_visible: bool` (true).
+- `is_hoverable: bool` (false).
+- `is_clickable: bool` (false).
 
 ### Frame
 - `contents: {}` See [frames](#frames) for more info.
 
 ### Label
 
 - `text: str` Exactly what you think it is.
-- `text_color: (r,g,b)` (default = (255,255,255))
-- `text_aa: bool` anti-aliasing (default = true)
-- `font_name: str` (default = 'Arial')
-- `font_size: int` (default = 10)
-- `font_bold: bool` (default = false)
-- `font_italic: bool` (default = false)
-- `auto_size: bool` This will overwrite size of the boundry box to fit the text within (default = false).
+- `text_color: (r,g,b)` ([255,255,255])
+- `text_aa: bool` anti-aliasing (true)
+- `font_name: str` ('Arial')
+- `font_size: int` (10)
+- `font_bold: bool` (false)
+- `font_italic: bool` (false)
+- `auto_size: bool` This will overwrite size of the boundry box to fit the text within (false).
 
 ### Button
 
 - `contents: {}` The button is basically just a frame with the following default attributes added to it. Making a button manually from a frame is possible, but deprecated.
-- `is_clickable: bool` (default = true)
-- `is_hoverable: bool` (default = true)
-- `click_start: bool` (default = false)
-- `click_end: bool` (default = false)
-- `held: bool` (default = false)
-- `hover_start: bool` (default = false)
-- `hover_end: bool` (default = false)
-- `hovered: bool` (default = false)
+- `is_clickable: bool` (true)
+- `is_hoverable: bool` (true)
+- `click_start: bool` (false)
+- `click_end: bool` (false)
+- `click_held: bool` (false)
+- `hover_start: bool` (false)
+- `hover_end: bool` (false)
+- `hover_held: bool` (false)
+
+### Switch
+- `state: bool` Represents the current state of the switch on/off (false)
+- `preset: str` A preset for it's looks. Only existing preset is currently: "simple" (none)
+- `is_clickable: bool` (true)
+- `is_hoverable: bool` (true)
+- `click_start: bool` (false)
+- `click_end: bool` (false)
+- `click_held: bool` (false)
+- `hover_start: bool` (false)
+- `hover_end: bool` (false)
+- `hover_held: bool` (false)
+
+### Slider
+- `value_min: int/float` Lower end of the slider (0)
+- `value_max: int/float` Uppper end of the slider (1)
+- `value: int/float` Represents the current value of the slider (0)
+- `preset: str` A preset for it's looks. Only existing preset is currently: "simple" (none)
+- `is_clickable: bool` (true)
+- `is_hoverable: bool` (true)
+- `click_start: bool` (false)
+- `click_end: bool` (false)
+- `click_held: bool` (false)
+- `hover_start: bool` (false)
+- `hover_end: bool` (false)
+- `hover_held: bool` (false)
 
 ## Frames
 
 Frames can contain `elements` Just like how a folder can contain files and other folders.
-Frames can also hold other frames, and yes, those can contain frames aswell (see [Frame-ception](#frame-ception)). When a frame is invisible, it's `elements` will also be invisable. Deleting a frame will also delete it's `elements`.
+Frames can also hold other frames, and yes, those can contain frames aswell (see [Frame-ception](#frame-ception)). When a frame is invisible, it's `elements` will also be invisible. Deleting a frame will also delete it's `elements`.
 
 ### Frame Path
 
 A frame path is a string representation of the route to a certain frame.
 
 Say we have the following json file
 ```json
@@ -189,16 +212,16 @@
    }
 }
 ```
 
 and i wanted to access `Pippinpaddleopsicopolis`
 
 The syntax for the frame path is very simple:
-```
-Arthur->Bertha->Pippinpaddleopsicopolis
+```python
+"Arthur->Bertha->Pippinpaddleopsicopolis"
 ```
 
 ## Examples
 
 All examples use [this](#python-file) python file as base.
 
 ### A button
@@ -301,8 +324,8 @@
       "contents": {}
    }
 }
 ```
 
 ## FAQ
 
-Nothing yet lol.
+Nothing yet lol.
```

### Comparing `pygame-json-ui-0.0.0.2/pyproject.toml` & `pygame-json-ui-0.0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygame-json-ui"
-version = "0.0.0.2"
+version = "0.0.0.3"
 authors = [
   { name="Xander de Haan", email="sissydeslang@gmail.com" },
 ]
 description = "Pygame UI is a package for building user interfaces for pygame in a JSON Format."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pygame-json-ui-0.0.0.2/src/pygame_json_ui.egg-info/PKG-INFO` & `pygame-json-ui-0.0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pygame-json-ui
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: Pygame UI is a package for building user interfaces for pygame in a JSON Format.
 Author-email: Xander de Haan <sissydeslang@gmail.com>
 Project-URL: Homepage, https://github.com/RednaxGaming/pygame_ui
 Project-URL: Bug Tracker, https://github.com/RednaxGaming/pygame_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Pygame UI README
 
-[Pygame UI](https://github.com/RednaxGaming/pygame_ui) is a package for building user interfaces in [pygame](https://www.pygame.org/).
+[![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+[Pygame UI](https://github.com/RednaxGaming/pygame_ui) is a package for building user interfaces for [pygame](https://www.pygame.org/) in JSON.
 
 It is currently a work in progress, but if you wanna test it out, feel free to do so :)
 
 ## Table Of Content
 
 - [Quick Start](#quick-start)
    - [Installation](#installation)
@@ -28,44 +30,53 @@
       - [JSON](#json-file)
 - [Element List](#element-list)
 - [Attribute List](#attribute-list)
    - [General](#general)
    - [Frame](#frame)
    - [Label](#label)
    - [Button](#button)
+   - [Switch](#switch)
+   - [Slider](#slider)
 - [Frames](#frames)
    - [Frame Path](#frame-path)
 - [Examples](#examples)
 - [FAQ](#faq)
 
 ## Quick Start
 
 ### Installation
 
-First of all, you'll need to manually add the pygame_ui folder to your site-packages, because the module is not yet available on pip.
+Pygame UI is available on PyPi:
+
+```shell
+pip install pygame-json-ui
+```
+In case this doesn't work, you'll need to manually add the pygame_ui folder to your site-packages.
 
 When this is done you can test your installation, by executing the following:
 ```python
 >>> import pygame_ui
 >>> pygame_ui.test()
 Successfully installed! enjoy :)
 Version: x.x.x.x
 ```
 
 ### Setup
 
 You will have two files in the same folder:
 - whatever.py
-- Interface.json <-- Specifically with that name and capitalization!
+- Interface.json <-- Name for automatically loading the file
+
+If you prefer a different name for the json file, or Pygame UI is having issues locating it automatically, you can pass the absolute path to it's parent folder as an argument for `pygame_ui.init()`.
 
 Here a simple example for making a label:
 
 #### Python File
 
-Notice that the `event_handler` is actually not required unless you want interactive elements to function as expected.
+Notice that the `event_handler` is not required unless you want interactive elements to function as expected.
 
 ```python
 import pygame
 import pygame_ui
 
 # Creating a window
 pygame.init()
@@ -91,15 +102,15 @@
    Interface.draw(screen)
 
    pygame.display.flip()
    clock.tick(60)
 ```
 
 #### JSON File
-MUST be named `Interface.json` and in the same folder as python file!
+MUST be named `Interface.json` and in the same folder as python file for loading the json file automatically!
 
 ```json
 {
    "label": {
       "name": "test_label",
       "position": [200,100],
       "size": [120,80],
@@ -113,60 +124,86 @@
 
 ## Element List
 
 All of the following items will be refered to as `elements`:
 - Frame
 - Label
 - Button
-- Switch (not implemented yet)
-- Slider (...)
-- Dropdown (...)
+- Switch
+- Slider
+- Dropdown (Coming soon)
 
 ## Attribute List
-
+- `attribute: type` description (default value).
 ### General
 These attributes can be given to any element type
-- `name: str` MUST be given to every element.
-- `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box.
-- `size: [x,y]` Sets the size of the element boundry box.
-- `background_color: (r,g,b)` The boundry box will be filled with this color. Don't set this for transparency.
-- `is_visible: bool` (default = true).
-- `is_hoverable: bool` (default = false).
-- `is_clickable: bool` (default = false).
+- `name: str` REQUIRED, used to access the element in python.
+- `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
+- `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
+- `background_color: (r,g,b)` The boundry box will be filled with this color (none).
+- `is_visible: bool` (true).
+- `is_hoverable: bool` (false).
+- `is_clickable: bool` (false).
 
 ### Frame
 - `contents: {}` See [frames](#frames) for more info.
 
 ### Label
 
 - `text: str` Exactly what you think it is.
-- `text_color: (r,g,b)` (default = (255,255,255))
-- `text_aa: bool` anti-aliasing (default = true)
-- `font_name: str` (default = 'Arial')
-- `font_size: int` (default = 10)
-- `font_bold: bool` (default = false)
-- `font_italic: bool` (default = false)
-- `auto_size: bool` This will overwrite size of the boundry box to fit the text within (default = false).
+- `text_color: (r,g,b)` ([255,255,255])
+- `text_aa: bool` anti-aliasing (true)
+- `font_name: str` ('Arial')
+- `font_size: int` (10)
+- `font_bold: bool` (false)
+- `font_italic: bool` (false)
+- `auto_size: bool` This will overwrite size of the boundry box to fit the text within (false).
 
 ### Button
 
 - `contents: {}` The button is basically just a frame with the following default attributes added to it. Making a button manually from a frame is possible, but deprecated.
-- `is_clickable: bool` (default = true)
-- `is_hoverable: bool` (default = true)
-- `click_start: bool` (default = false)
-- `click_end: bool` (default = false)
-- `held: bool` (default = false)
-- `hover_start: bool` (default = false)
-- `hover_end: bool` (default = false)
-- `hovered: bool` (default = false)
+- `is_clickable: bool` (true)
+- `is_hoverable: bool` (true)
+- `click_start: bool` (false)
+- `click_end: bool` (false)
+- `click_held: bool` (false)
+- `hover_start: bool` (false)
+- `hover_end: bool` (false)
+- `hover_held: bool` (false)
+
+### Switch
+- `state: bool` Represents the current state of the switch on/off (false)
+- `preset: str` A preset for it's looks. Only existing preset is currently: "simple" (none)
+- `is_clickable: bool` (true)
+- `is_hoverable: bool` (true)
+- `click_start: bool` (false)
+- `click_end: bool` (false)
+- `click_held: bool` (false)
+- `hover_start: bool` (false)
+- `hover_end: bool` (false)
+- `hover_held: bool` (false)
+
+### Slider
+- `value_min: int/float` Lower end of the slider (0)
+- `value_max: int/float` Uppper end of the slider (1)
+- `value: int/float` Represents the current value of the slider (0)
+- `preset: str` A preset for it's looks. Only existing preset is currently: "simple" (none)
+- `is_clickable: bool` (true)
+- `is_hoverable: bool` (true)
+- `click_start: bool` (false)
+- `click_end: bool` (false)
+- `click_held: bool` (false)
+- `hover_start: bool` (false)
+- `hover_end: bool` (false)
+- `hover_held: bool` (false)
 
 ## Frames
 
 Frames can contain `elements` Just like how a folder can contain files and other folders.
-Frames can also hold other frames, and yes, those can contain frames aswell (see [Frame-ception](#frame-ception)). When a frame is invisible, it's `elements` will also be invisable. Deleting a frame will also delete it's `elements`.
+Frames can also hold other frames, and yes, those can contain frames aswell (see [Frame-ception](#frame-ception)). When a frame is invisible, it's `elements` will also be invisible. Deleting a frame will also delete it's `elements`.
 
 ### Frame Path
 
 A frame path is a string representation of the route to a certain frame.
 
 Say we have the following json file
 ```json
@@ -189,16 +226,16 @@
    }
 }
 ```
 
 and i wanted to access `Pippinpaddleopsicopolis`
 
 The syntax for the frame path is very simple:
-```
-Arthur->Bertha->Pippinpaddleopsicopolis
+```python
+"Arthur->Bertha->Pippinpaddleopsicopolis"
 ```
 
 ## Examples
 
 All examples use [this](#python-file) python file as base.
 
 ### A button
```

### Comparing `pygame-json-ui-0.0.0.2/src/pygame_ui/__init__.py` & `pygame-json-ui-0.0.0.3/src/pygame_ui/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 Make sure you read the ``Getting started`` section of the documentation in the library folder.
 """
 
 from pygame_ui.base import *
 from pygame_ui.elements import *
 
 # release, year, month, session
-__version__ = '0.0.0.2'
+__version__ = '0.0.0.3'
 
 #print('Pygame UI ' + __version__)
 
 def test():
-    import pygame_ui.base
-    import pygame_ui.constants
-    import pygame_ui.elements
-    print('Successfully installed! enjoy :)\nversion: '+__version__)
-    del pygame_ui.base, pygame_ui.constants, pygame_ui.elements
+	try:
+		import pygame_ui.base
+		import pygame_ui.constants
+		import pygame_ui.elements
+		print('Successfully installed! enjoy :)\nversion: '+__version__)
+		del pygame_ui.base, pygame_ui.constants, pygame_ui.elements
+	except:
+		print(ISSUE_REPORT)
 
 # Base64
 # VGhpcyBjb2RlIHdhcyB3cml0dGVuIGJ5IFJlZG5heEdhbWluZyBvbiBnaXRodWI=
```

### Comparing `pygame-json-ui-0.0.0.2/src/pygame_ui/base.py` & `pygame-json-ui-0.0.0.3/src/pygame_ui/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,36 +77,46 @@
 		"""
 		This handles all interactive elements.
 
 		Must be called in the following context:
 		>>> for event in pygame.event.get():
 			Interface.event_handler(event)
 		"""
+
 		self.get_interactive_elements()
 
 		element = None
+		lmb, rmb, mmb = pygmouse.get_pressed(3)
+		mpos = pygmouse.get_pos()
 		
 		for i in self.interactive_elements:
-			if i.is_clickable or i.is_hoverable:
-				mouse_in_boundry = i.rectangle.collidepoint(pygmouse.get_pos())
-			
+			mouse_in_boundry = i.rectangle.collidepoint(mpos)
+
 			if mouse_in_boundry:
 				if event.type in [pyglocal.MOUSEBUTTONDOWN, pyglocal.MOUSEBUTTONUP] and i.is_clickable:
 					element = i
 				elif event.type in [pyglocal.MOUSEMOTION, pyglocal.MOUSEWHEEL] and i.is_hoverable:
 					element = i
+			elif event.type in [pyglocal.MOUSEBUTTONUP, pyglocal.MOUSEMOTION, pyglocal.MOUSEWHEEL] and i.click_held:
+				element = i
+			
+			if event.type == pyglocal.MOUSEBUTTONUP and lmb == 0:
+				i.click_end = True
+				i.click_held = False
 
 		if element != None:
-			if event.type == pyglocal.MOUSEBUTTONDOWN and pygmouse.get_pressed(3)[0] == 1:
+			if event.type in [pyglocal.MOUSEMOTION, pyglocal.MOUSEWHEEL]:
+				if isinstance(element, pygame_ui.slider) and element.click_held:
+					i.set_value_from_pos(mpos)
+
+			elif event.type == pyglocal.MOUSEBUTTONDOWN and lmb == 1:
 				element.click_start = True
-				element.held = True
-		
-			elif event.type == pyglocal.MOUSEBUTTONUP and pygmouse.get_pressed(3)[0] == 0:
-				element.click_end = True
-				element.held = False
+				element.click_held = True
+				if isinstance(element, pygame_ui.switch):
+					element.state = not element.state
 
 		return 1
 	
 	def draw(self, pygame_window):
 		"""
 		Main draw function which will draw all visible things layered like painter-style.
 		
@@ -117,38 +127,38 @@
 
 		for i in self.elements.values():
 			if i.is_visible:
 				if i.background_color != None:
 					i.draw_bg(pygame_window)
 				i.draw(pygame_window)
 		
+		# Reset all temporary attribute values
 		for i in self.interactive_elements:
 			if i.is_clickable:
 				i.click_start = False
 				i.click_end = False
 			if i.is_hoverable:
 				i.hover_start = False
 				i.hover_end = False
 				
 		return 1
 
 
-def init():
+def init(path_to_json:str='Interface.json'):
 	"""
 	This loads in the ``Interface.json`` file and created a GUI with it
 	"""
 
 	import json
 	import os
-	from pathlib import Path
-
-	for i in os.listdir():
-		if os.path.isdir(i):
-			pass
-	file = open(os.path.abspath('Interface.json'))
+	
+	try:
+		file = open(os.path.abspath(path_to_json))
+	except FileNotFoundError:
+		print(ISSUE_REPORT)
 	UI = json.load(file)
 	file.close()
 
 	interface = Graphical_UI(UI)
 
 	# clearing up namespace
 	del json, os, pygame_ui.elements
```

### Comparing `pygame-json-ui-0.0.0.2/src/pygame_ui/elements.py` & `pygame-json-ui-0.0.0.3/src/pygame_ui/elements.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class UI_Element:
 	is_visible = True
 	is_hoverable = False
 	is_clickable = False
 	position = [0,0]
 	size = [0,0]
+	anchor = "absolute"
 	auto_size = False
 	background_color = None
 
 	def __init__(self, initial_data, kwargs):
 		for dictionary in initial_data:
 			for key in dictionary:
 				setattr(self, key, dictionary[key])
@@ -88,25 +89,14 @@
 		for i in self.elements.values():
 			if i.is_visible:
 				if i.background_color != None:
 					i.draw_bg(pygame_window)
 				i.draw(pygame_window)
 
 
-class button(frame):
-	is_clickable = True
-	is_hoverable = True
-	click_start = False
-	click_end = False
-	held = False
-	hover_start = False
-	hover_end = False
-	hovered = False
-
-
 class label(UI_Element):
 	"""
 	The UI element for text.
 
 	Anything with letters will use this class.
 	"""
 	
@@ -138,35 +128,96 @@
 		self.font = pygfont.SysFont(self.font_name, self.font_size, self.font_bold, self.font_italic)
 
 	def draw(self, pygame_window):
 		text_render = self.font.render(self.text, self.text_aa, self.text_color, self.background_color)
 		pygame_window.blit(text_render, self.position)
 
 
+class button(frame):
+	"""
+	The UI element for a button.
+
+	What does this button do?
+	"""
+	is_clickable = True
+	is_hoverable = True
+	click_start = False
+	click_end = False
+	click_held = False
+	hover_start = False
+	hover_end = False
+	hover_held = False
+
+
 class switch(UI_Element):
+	"""
+	The UI element for a switch.
+
+	Switcharoo!
+	"""
 	is_clickable = True
+	is_hoverable = True
+	click_start = False
+	click_end = False
+	click_held = False
+	hover_start = False
+	hover_end = False
+	hover_held = False
+	state = False
+	preset = None
 
 	def __init__(self, *initial_data, **kwargs):
 		super().__init__(initial_data, kwargs)
 
 	def draw(self, pygame_window):
-		pass
+		if self.preset == 'simple':
+			size = [self.size[0]/2-5, self.size[1]-10]
+			position = [self.position[0]+5+size[0]*int(self.state), self.position[1]+5]
+			pygdraw.rect(pygame_window, (200,200,200), pygrect.Rect(position, size))
 
 
 class slider(UI_Element):
+	"""
+	The UI element that slides.
+
+	Sliiide to the left, sliiide to the right, criss cross!
+	"""
 	is_clickable = True
+	is_hoverable = True
+	click_start = False
+	click_end = False
+	click_held = False
+	hover_start = False
+	hover_end = False
+	hover_held = False
+	value_min = 0
+	value_max = 1
+	value = 0
+	preset = None
 
 	def __init__(self, *initial_data, **kwargs):
 		super().__init__(initial_data, kwargs)
 
+	def set_value_from_pos(self, position):
+		if self.preset == 'simple':
+			self.value/(self.value_max-self.value_min)
+			x = (self.value_max - self.value_min) * (position[0]-self.size[1]/2 - self.position[0])/(self.size[0]-self.size[1])
+			self.value = max(min(self.value_max, x), self.value_min)
+
 	def draw(self, pygame_window):
-		pass
+		if self.preset == 'simple':
+			size = [self.size[1]-10, self.size[1]-10]
+			position = [self.position[0]+5+(self.size[0]-self.size[1])*self.value/(self.value_max-self.value_min), self.position[1]+5]
+			pygdraw.rect(pygame_window, (200,200,200), pygrect.Rect(position, size))
 
 
 class dropdown(UI_Element):
+	"""
+	Unfinished
+	"""
 	is_clickable = True
 
 	def __init__(self, *initial_data, **kwargs):
 		super().__init__(initial_data, kwargs)
 
 	def draw(self, pygame_window):
 		pass
```

