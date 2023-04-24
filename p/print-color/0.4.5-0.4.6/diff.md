# Comparing `tmp/print-color-0.4.5.tar.gz` & `tmp/print_color-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "print-color-0.4.5.tar", max compression
+gzip compressed data, was "print_color-0.4.6.tar", max compression
```

## Comparing `print-color-0.4.5.tar` & `print_color-0.4.6.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2021-10-12 11:56:35.124626 print-color-0.4.5/LICENSE
--rw-r--r--   0        0        0     1897 2021-10-12 11:56:35.124626 print-color-0.4.5/README.md
--rw-r--r--   0        0        0       50 2021-10-12 11:56:35.124626 print-color-0.4.5/print_color/__init__.py
--rw-r--r--   0        0        0     2477 2021-10-12 11:56:35.124626 print-color-0.4.5/print_color/print_color.py
--rw-r--r--   0        0        0      471 2021-10-12 11:56:57.244633 print-color-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2661 2021-10-12 11:56:57.752827 print-color-0.4.5/setup.py
--rw-r--r--   0        0        0     2625 2021-10-12 11:56:57.753158 print-color-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 17:42:53.748422 print_color-0.4.6/LICENSE
+-rw-r--r--   0        0        0     2040 2023-04-24 17:42:53.748422 print_color-0.4.6/README.md
+-rw-r--r--   0        0        0       50 2023-04-24 17:42:53.748422 print_color-0.4.6/print_color/__init__.py
+-rw-r--r--   0        0        0     4497 2023-04-24 17:42:53.748422 print_color-0.4.6/print_color/print_color.py
+-rw-r--r--   0        0        0      477 2023-04-24 17:43:20.032039 print_color-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2730 1970-01-01 00:00:00.000000 print_color-0.4.6/PKG-INFO
```

### Comparing `print-color-0.4.5/LICENSE` & `print_color-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `print-color-0.4.5/README.md` & `print_color-0.4.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # print-color
 
+[![test](https://github.com/xy3/print-color/actions/workflows/ci.yml/badge.svg)](https://github.com/xy3/print-color/actions/workflows/ci.yml)
+
 Print Color is a minimalist approach to terminal color printing in Python. It is a wrapper around the `print()` function, and simply allows you to provide extra optional parameters such as:
 
 - `tag`
 - `tag_color` or `tag_colour`
 - `color` or `colour`
 - `background`
 - `format`
@@ -51,15 +53,15 @@
 
 ```shell
 pip3 install print-color
 ```
 
 ### Requirements
 
-- python 3.5^
+- python 3.7^
 
 ### Usage
 
 ```python
 from print_color import print
 
 print("Hello world", tag='success', tag_color='green', color='white')
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-# print-color Print Color is a minimalist approach to terminal color printing
-in Python. It is a wrapper around the `print()` function, and simply allows you
-to provide extra optional parameters such as: - `tag` - `tag_color` or
-`tag_colour` - `color` or `colour` - `background` - `format` It aims to be a
-customizable logger for your applications, and makes formatting warnings, info
-messages and errors a breeze. --- ## Information This project has no
-dependencies, apart from `pytest` for testing. Check out this project on [PyPi
-here](https://pypi.org/project/print-color/). Colors: ```text purple blue green
-yellow red magenta cyan white black ``` ### Parameter values: - `tag` - any
-string - `tag_color` or `tag_colour` - color - `color` or `colour` - color -
+# print-color [![test](https://github.com/xy3/print-color/actions/workflows/
+ci.yml/badge.svg)](https://github.com/xy3/print-color/actions/workflows/ci.yml)
+Print Color is a minimalist approach to terminal color printing in Python. It
+is a wrapper around the `print()` function, and simply allows you to provide
+extra optional parameters such as: - `tag` - `tag_color` or `tag_colour` -
+`color` or `colour` - `background` - `format` It aims to be a customizable
+logger for your applications, and makes formatting warnings, info messages and
+errors a breeze. --- ## Information This project has no dependencies, apart
+from `pytest` for testing. Check out this project on [PyPi here](https://
+pypi.org/project/print-color/). Colors: ```text purple blue green yellow red
+magenta cyan white black ``` ### Parameter values: - `tag` - any string -
+`tag_color` or `tag_colour` - color - `color` or `colour` - color -
 `background` - color - `format` - bold - underline - blink ### Installing
-```shell pip3 install print-color ``` ### Requirements - python 3.5^ ### Usage
+```shell pip3 install print-color ``` ### Requirements - python 3.7^ ### Usage
 ```python from print_color import print print("Hello world", tag='success',
 tag_color='green', color='white') ``` ![Success tag](https://i.imgur.com/
 qmeYTkR.png) ```python print("Error detected", tag='failure', tag_color='red',
 color='magenta') ``` ![Error tag](https://i.imgur.com/dksa03u.png) ```python
 print("Printing in color", color='green', format='underline',
 background='grey') ``` ![Printing in color is easy](https://i.imgur.com/
 3sUTi8z.png) ## Contributing Feel free to add or improve this project :) Just
```

### Comparing `print-color-0.4.5/setup.py` & `print_color-0.4.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: print-color
+Version: 0.4.6
+Summary: A simple package to print in color to the terminal
+Home-page: https://github.com/xy3/print-color
+License: MIT
+Author: xy3
+Author-email: a@xsq.pw
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/xy3/print-color
+Description-Content-Type: text/markdown
 
-packages = \
-['print_color']
+# print-color
 
-package_data = \
-{'': ['*']}
+[![test](https://github.com/xy3/print-color/actions/workflows/ci.yml/badge.svg)](https://github.com/xy3/print-color/actions/workflows/ci.yml)
 
-install_requires = \
-['pytest>=6.2.5,<7.0.0']
-
-setup_kwargs = {
-    'name': 'print-color',
-    'version': '0.4.5',
-    'description': 'A simple package to print in color to the terminal',
-    'long_description': '# print-color\n\nPrint Color is a minimalist approach to terminal color printing in Python. It is a wrapper around the `print()` function, and simply allows you to provide extra optional parameters such as:\n\n- `tag`\n- `tag_color` or `tag_colour`\n- `color` or `colour`\n- `background`\n- `format`\n\nIt aims to be a customizable logger for your applications, and makes formatting warnings, info messages and errors a breeze.\n\n---\n\n## Information\n\nThis project has no dependencies, apart from `pytest` for testing.\n\nCheck out this project on [PyPi here](https://pypi.org/project/print-color/).\n\nColors:\n\n```text\npurple\nblue\ngreen\nyellow\nred\nmagenta\ncyan\nwhite\nblack\n```\n\n### Parameter values:\n\n- `tag`\n  - any string\n- `tag_color` or `tag_colour`\n  - color\n- `color` or `colour`\n  - color\n- `background`\n  - color\n- `format`\n  - bold\n  - underline\n  - blink\n\n### Installing\n\n```shell\npip3 install print-color\n```\n\n### Requirements\n\n- python 3.5^\n\n### Usage\n\n```python\nfrom print_color import print\n\nprint("Hello world", tag=\'success\', tag_color=\'green\', color=\'white\')\n```\n\n![Success tag](https://i.imgur.com/qmeYTkR.png)\n\n```python\nprint("Error detected", tag=\'failure\', tag_color=\'red\', color=\'magenta\')\n```\n\n![Error tag](https://i.imgur.com/dksa03u.png)\n\n```python\nprint("Printing in color", color=\'green\', format=\'underline\', background=\'grey\')\n```\n\n![Printing in color is easy](https://i.imgur.com/3sUTi8z.png)\n\n## Contributing\n\nFeel free to add or improve this project :) Just create a pull request and explain the changes you propose.\nNote that as this is a very simple project, feature requests should be kept minimal - things like more colors, formats etc would be ideal.\n\n## Credits\n\nBuilt with [Python Poetry](https://python-poetry.org/).\n\n### Contributors\n\n<a href="https://github.com/xy3/print-color/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=xy3/print-color" />\n</a>\n',
-    'author': 'xy3',
-    'author_email': 'a@xsq.pw',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/xy3/print-color',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+Print Color is a minimalist approach to terminal color printing in Python. It is a wrapper around the `print()` function, and simply allows you to provide extra optional parameters such as:
 
+- `tag`
+- `tag_color` or `tag_colour`
+- `color` or `colour`
+- `background`
+- `format`
+
+It aims to be a customizable logger for your applications, and makes formatting warnings, info messages and errors a breeze.
+
+---
+
+## Information
+
+This project has no dependencies, apart from `pytest` for testing.
+
+Check out this project on [PyPi here](https://pypi.org/project/print-color/).
+
+Colors:
+
+```text
+purple
+blue
+green
+yellow
+red
+magenta
+cyan
+white
+black
+```
+
+### Parameter values:
+
+- `tag`
+  - any string
+- `tag_color` or `tag_colour`
+  - color
+- `color` or `colour`
+  - color
+- `background`
+  - color
+- `format`
+  - bold
+  - underline
+  - blink
+
+### Installing
+
+```shell
+pip3 install print-color
+```
+
+### Requirements
+
+- python 3.7^
+
+### Usage
+
+```python
+from print_color import print
+
+print("Hello world", tag='success', tag_color='green', color='white')
+```
+
+![Success tag](https://i.imgur.com/qmeYTkR.png)
+
+```python
+print("Error detected", tag='failure', tag_color='red', color='magenta')
+```
+
+![Error tag](https://i.imgur.com/dksa03u.png)
+
+```python
+print("Printing in color", color='green', format='underline', background='grey')
+```
+
+![Printing in color is easy](https://i.imgur.com/3sUTi8z.png)
+
+## Contributing
+
+Feel free to add or improve this project :) Just create a pull request and explain the changes you propose.
+Note that as this is a very simple project, feature requests should be kept minimal - things like more colors, formats etc would be ideal.
+
+## Credits
+
+Built with [Python Poetry](https://python-poetry.org/).
+
+### Contributors
+
+<a href="https://github.com/xy3/print-color/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=xy3/print-color" />
+</a>
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['print_color'] package_data = \ {'': ['*']} install_requires = \
-['pytest>=6.2.5,<7.0.0'] setup_kwargs = { 'name': 'print-color', 'version':
-'0.4.5', 'description': 'A simple package to print in color to the terminal',
-'long_description': '# print-color\n\nPrint Color is a minimalist approach to
-terminal color printing in Python. It is a wrapper around the `print()`
-function, and simply allows you to provide extra optional parameters such as:
-\n\n- `tag`\n- `tag_color` or `tag_colour`\n- `color` or `colour`\n-
-`background`\n- `format`\n\nIt aims to be a customizable logger for your
-applications, and makes formatting warnings, info messages and errors a
-breeze.\n\n---\n\n## Information\n\nThis project has no dependencies, apart
-from `pytest` for testing.\n\nCheck out this project on [PyPi here](https://
-pypi.org/project/print-color/).\n\nColors:
-\n\n```text\npurple\nblue\ngreen\nyellow\nred\nmagenta\ncyan\nwhite\nblack\n```\n\n###
-Parameter values:\n\n- `tag`\n - any string\n- `tag_color` or `tag_colour`\n -
-color\n- `color` or `colour`\n - color\n- `background`\n - color\n- `format`\n
-- bold\n - underline\n - blink\n\n### Installing\n\n```shell\npip3 install
-print-color\n```\n\n### Requirements\n\n- python 3.5^\n\n###
-Usage\n\n```python\nfrom print_color import print\n\nprint("Hello world",
-tag=\'success\', tag_color=\'green\', color=\'white\')\n```\n\n![Success tag]
-(https://i.imgur.com/qmeYTkR.png)\n\n```python\nprint("Error detected",
-tag=\'failure\', tag_color=\'red\', color=\'magenta\')\n```\n\n![Error tag]
-(https://i.imgur.com/dksa03u.png)\n\n```python\nprint("Printing in color",
-color=\'green\', format=\'underline\', background=\'grey\')\n```\n\n![Printing
-in color is easy](https://i.imgur.com/3sUTi8z.png)\n\n## Contributing\n\nFeel
-free to add or improve this project :) Just create a pull request and explain
-the changes you propose.\nNote that as this is a very simple project, feature
-requests should be kept minimal - things like more colors, formats etc would be
-ideal.\n\n## Credits\n\nBuilt with [Python Poetry](https://python-poetry.org/
-).\n\n### Contributors\n\n\n_[https://contrib.rocks/image?repo=xy3/print-
-color]\n\n', 'author': 'xy3', 'author_email': 'a@xsq.pw', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/xy3/print-color',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.6,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: print-color Version: 0.4.6 Summary: A simple
+package to print in color to the terminal Home-page: https://github.com/xy3/
+print-color License: MIT Author: xy3 Author-email: a@xsq.pw Requires-Python:
+>=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Project-URL:
+Repository, https://github.com/xy3/print-color Description-Content-Type: text/
+markdown # print-color [![test](https://github.com/xy3/print-color/actions/
+workflows/ci.yml/badge.svg)](https://github.com/xy3/print-color/actions/
+workflows/ci.yml) Print Color is a minimalist approach to terminal color
+printing in Python. It is a wrapper around the `print()` function, and simply
+allows you to provide extra optional parameters such as: - `tag` - `tag_color`
+or `tag_colour` - `color` or `colour` - `background` - `format` It aims to be a
+customizable logger for your applications, and makes formatting warnings, info
+messages and errors a breeze. --- ## Information This project has no
+dependencies, apart from `pytest` for testing. Check out this project on [PyPi
+here](https://pypi.org/project/print-color/). Colors: ```text purple blue green
+yellow red magenta cyan white black ``` ### Parameter values: - `tag` - any
+string - `tag_color` or `tag_colour` - color - `color` or `colour` - color -
+`background` - color - `format` - bold - underline - blink ### Installing
+```shell pip3 install print-color ``` ### Requirements - python 3.7^ ### Usage
+```python from print_color import print print("Hello world", tag='success',
+tag_color='green', color='white') ``` ![Success tag](https://i.imgur.com/
+qmeYTkR.png) ```python print("Error detected", tag='failure', tag_color='red',
+color='magenta') ``` ![Error tag](https://i.imgur.com/dksa03u.png) ```python
+print("Printing in color", color='green', format='underline',
+background='grey') ``` ![Printing in color is easy](https://i.imgur.com/
+3sUTi8z.png) ## Contributing Feel free to add or improve this project :) Just
+create a pull request and explain the changes you propose. Note that as this is
+a very simple project, feature requests should be kept minimal - things like
+more colors, formats etc would be ideal. ## Credits Built with [Python Poetry]
+(https://python-poetry.org/). ### Contributors [https://contrib.rocks/
+image?repo=xy3/print-color]
```

