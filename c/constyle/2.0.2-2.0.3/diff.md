# Comparing `tmp/constyle-2.0.2.tar.gz` & `tmp/constyle-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constyle-2.0.2.tar", max compression
+gzip compressed data, was "constyle-2.0.3.tar", max compression
```

## Comparing `constyle-2.0.2.tar` & `constyle-2.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-08-17 20:57:29.587528 constyle-2.0.2/LICENSE
--rw-r--r--   0        0        0     5429 2022-08-17 20:57:29.587528 constyle-2.0.2/README.md
--rw-r--r--   0        0        0      332 2022-08-17 20:57:29.587528 constyle-2.0.2/constyle/__init__.py
--rw-r--r--   0        0        0     1839 2022-08-17 20:57:29.587528 constyle-2.0.2/constyle/__main__.py
--rw-r--r--   0        0        0     7399 2022-08-17 20:57:29.591528 constyle-2.0.2/constyle/_attributes.py
--rw-r--r--   0        0        0     3015 2022-08-17 20:57:29.591528 constyle-2.0.2/constyle/_style.py
--rw-r--r--   0        0        0     2913 2022-08-17 20:57:29.591528 constyle-2.0.2/constyle/custom_colours.py
--rw-r--r--   0        0        0        1 2022-08-17 20:57:29.591528 constyle-2.0.2/constyle/py.typed
--rw-r--r--   0        0        0      903 2022-08-17 20:57:40.919513 constyle-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6422 2022-08-17 20:57:42.227549 constyle-2.0.2/setup.py
--rw-r--r--   0        0        0     6361 2022-08-17 20:57:42.228093 constyle-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 13:19:44.006688 constyle-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5429 2023-04-24 13:19:44.006688 constyle-2.0.3/README.md
+-rw-r--r--   0        0        0      332 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/__init__.py
+-rw-r--r--   0        0        0     1839 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/__main__.py
+-rw-r--r--   0        0        0     7465 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/_attributes.py
+-rw-r--r--   0        0        0     3015 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/_style.py
+-rw-r--r--   0        0        0     2913 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/custom_colours.py
+-rw-r--r--   0        0        0        1 2023-04-24 13:19:44.006688 constyle-2.0.3/constyle/py.typed
+-rw-r--r--   0        0        0      903 2023-04-24 13:19:56.390661 constyle-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6422 2023-04-24 13:19:57.221118 constyle-2.0.3/setup.py
+-rw-r--r--   0        0        0     6361 2023-04-24 13:19:57.221652 constyle-2.0.3/PKG-INFO
```

### Comparing `constyle-2.0.2/LICENSE` & `constyle-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `constyle-2.0.2/README.md` & `constyle-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `constyle-2.0.2/constyle/__main__.py` & `constyle-2.0.3/constyle/__main__.py`

 * *Files identical despite different names*

### Comparing `constyle-2.0.2/constyle/_attributes.py` & `constyle-2.0.3/constyle/_attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
-from ._style import Style
+
 from attributes_doc import attributes_doc
 
+from ._style import Style
+
 
 @attributes_doc
 class Attributes(Style, Enum):
     """
     This enum contains almost all ANSI sequences known to man.
 
     Due to inconsistencies across implementations you may find that there are sometimes conflicting attributes with the same param.
@@ -208,9 +210,12 @@
     FRAMED = 51
     """Framed text. Implemented as "emoji variation selector" in mintty."""
     ENCIRCLED = 52
     """Encircled text. Implemented as "emoji variation selector" in mintty."""
     NO_FRAMED_ENCIRCLED = 54
     """Unset framed/encircled text"""
 
+    def __str__(self) -> str:
+        return super().__str__()
+
     def __repr__(self) -> str:
         return self.name
```

### Comparing `constyle-2.0.2/constyle/_style.py` & `constyle-2.0.3/constyle/_style.py`

 * *Files identical despite different names*

### Comparing `constyle-2.0.2/constyle/custom_colours.py` & `constyle-2.0.3/constyle/custom_colours.py`

 * *Files identical despite different names*

### Comparing `constyle-2.0.2/pyproject.toml` & `constyle-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "constyle"
 # Version is overwritten at build time by CI based on git tag
-version = "2.0.2"
+version = "2.0.3"
 description = "A Python library to add style to your console."
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-constyle"
 documentation = "https://abrahammurciano.github.io/python-constyle/constyle"
 keywords = [
```

### Comparing `constyle-2.0.2/setup.py` & `constyle-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['attributes-doc>=0.3.0', 'importlib-metadata>=4.11.0']
 
 entry_points = \
 {'console_scripts': ['constyle = constyle.__main__:main']}
 
 setup_kwargs = {
     'name': 'constyle',
-    'version': '2.0.2',
+    'version': '2.0.3',
     'description': 'A Python library to add style to your console.',
     'long_description': '# constyle\nA Python library to add style to your console.\n\nThe name of the library comes from merging the words **CONSoLE** and **STYLE**. Also "con" means "with" in Spanish.\n\n## Installation\n\nYou can install this package with pip or conda.\n```sh\n$ pip install constyle\n```\n```sh\n$ conda install -c conda-forge constyle\n```\n```sh\n$ conda install -c abrahammurciano constyle\n```\n\n## Links\n\n[![Documentation](https://img.shields.io/badge/Documentation-C61C3E?style=for-the-badge&logo=Read+the+Docs&logoColor=%23FFFFFF)](https://abrahammurciano.github.io/python-constyle/constyle)\n\n[![Source Code - GitHub](https://img.shields.io/badge/Source_Code-GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=%23FFFFFF)](https://github.com/abrahammurciano/python-constyle.git)\n\n[![PyPI - constyle](https://img.shields.io/badge/PyPI-constyle-006DAD?style=for-the-badge&logo=PyPI&logoColor=%23FFD242)](https://pypi.org/project/constyle/)\n\n[![Anaconda - constyle](https://img.shields.io/badge/Anaconda-constyle-44A833?style=for-the-badge&logo=Anaconda&logoColor=%23FFFFFF)](https://anaconda.org/abrahammurciano/constyle)\n\n[![Discord - Community](https://img.shields.io/badge/Discord-Community-5865F2?style=for-the-badge&logo=Discord&logoColor=FFFFFF)](https://discord.gg/nUmsrhNDSs)\n\n## Usage\n\nThere are a couple of ways to use this library.\n\n### The `style` function\n\nThe simplest way is with the `style` function.\n\n```py\nfrom constyle import style, Attributes\n\nprint(style(\'Hello World\', Attributes.GREEN, Attributes.BOLD, Attributes.ON_BLUE))\n```\n\n### `Style` objects\n\nYou can also use `Style` objects to create a reusable style with any number of attributes.\n\n#### Calling a `Style` object\n\n`Style` objects are callable and take a string as input and return a styled string.\n\n```py\nwarning = Style(Attributes.YELLOW, Attributes.BOLD)\nprint(warning(\'You shall not pass!\'))\n```\n\n#### Adding `Style` objects\n\nAdding together `Style` objects will also create `Style` objects.\n\n```py\nwhisper = Attributes.GREY + Attributes.DIM + Attributes.SUPERSCRIPT\nprint(whisper(\'Fly you fools\'))\n```\n\n#### Converting `Style` objects to strings\n\n`Style` objects can be converted to strings to obtain the ANSI escape sequence for that style.\n\n```py\nwarning = Style(Attributes.YELLOW, Attributes.BOLD)\nprint(f"{warning}You shall not pass!{Attributes.RESET}")\n```\n\n### Attributes\n\nThe `Attributes` enum contains all the available ANSI attributes. You can read more about them [here](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters).\n\n`Attributes` are also `Style` objects, and as such, as demonstrated above, they too can be called to style a string, added together and to other `Style` objects, and converted to strings to obtain their ANSI sequence.\n\nYou\'ll find there is limited support for all the ANSI attributes among some consoles.\n\nIf you find more attributes that aren\'t provided in this enum, you can create your own by constructing a `Style` with an integer.\n\n### Nesting\n\nIn order to nest styles, you can use the `end=` keyword argument of the `style` function or the `Style` class. Usually when applying a style, the `RESET` attribute is appended to the end. This can be undesirable when nesting (see the example below).\n\n```py\nbold = Attributes.BOLD\nyellow = Attributes.YELLOW\ngreen = Attributes.GREEN\n\nprint(yellow(bold(\'This is bold and yellow\')))\nprint(green(f"This is green. {yellow(\'This is yellow.\')} This is no longer green"))\n```\n\nIn order to achieve the desired result in the above example, you would have to use the `end=` keyword argument of the `style` function. You can pass any `Style` to `end`.\n\n```py\nprint(green(f"This is green. {bold(\'This is green and bold.\', end=Attributes.NO_BOLD)} This is still green but not bold anymore"))\nprint(green(f"This is green. {yellow(\'This is yellow.\', end=green)} This is now green again"))\n```\n\n### Custom colours\n\nThe `constyle.custom_colours` module contains a few classes that can be used to create custom colours.\n\n#### RGB colours\n\nYou can create a `Style` for a custom RGB colour by using the `RGB` class. This is not well supported by all consoles.\n\n```py\nfrom constyle.custom_colours import RGB\n\nprint(style(\'This is pink\', RGB(255, 192, 203)))\n```\n\n#### 8-bit colours\n\nSome consoles support 8-bit colours. You can create a `Style` for an 8-bit colour by using the `EightBit` class, passing a single integer to it, or you can use the `EightBitRGB` class to create an 8-bit colour style as close to the RGB values as possible.\n\n## The command line interface\n\nThis package also provides a very basic command line interface to print styled strings.\n\nYou can pass it any number of strings and it will print them all together (like `echo`). You can pass `--attribute` (or `-a`) with the name of an attribute to apply to the other strings being printed. You can pass `--attribute` as many times as you like.\n\nYou can use `constyle --help` to see more specific details, as well as all available attributes.\n\nFor example you can use `constyle` from your shell to print some styled text.\n\n```sh\n$ constyle Hello World! -a green -a bold -a on_white\n```\n\nOr if you\'re writing a shell script you can make an alias or a function to reuse a certain style.\n\n```sh\n#!/bin/bash\nalias error="constyle --attribute bold --attribute red" # With an alias\nwarn() { constyle $@ -a bold -a yellow } # With a function\nerror You shall not pass!\nwarn Fly you fools!\n```',
     'author': 'Abraham Murciano',
     'author_email': 'abrahammurciano@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/abrahammurciano/python-constyle',
```

### Comparing `constyle-2.0.2/PKG-INFO` & `constyle-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constyle
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Python library to add style to your console.
 Home-page: https://github.com/abrahammurciano/python-constyle
 License: GPLv3
 Keywords: terminal,console,style,color,colors,colour,colours,ansi
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.7,<4.0
```

