# Comparing `tmp/async_tkinter_loop-0.7.0.tar.gz` & `tmp/async_tkinter_loop-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_tkinter_loop-0.7.0.tar", max compression
+gzip compressed data, was "async_tkinter_loop-0.8.0.tar", max compression
```

## Comparing `async_tkinter_loop-0.7.0.tar` & `async_tkinter_loop-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2022-11-14 17:10:06.997911 async_tkinter_loop-0.7.0/LICENSE
--rw-r--r--   0        0        0     6160 2022-11-14 17:10:06.997911 async_tkinter_loop-0.7.0/README.md
--rw-r--r--   0        0        0     2402 2022-11-14 17:10:06.997911 async_tkinter_loop-0.7.0/async_tkinter_loop.py
--rw-r--r--   0        0        0     1293 2022-11-14 17:10:06.997911 async_tkinter_loop-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7079 1970-01-01 00:00:00.000000 async_tkinter_loop-0.7.0/setup.py
--rw-r--r--   0        0        0     7336 1970-01-01 00:00:00.000000 async_tkinter_loop-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-24 18:22:36.143923 async_tkinter_loop-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6448 2023-04-24 18:22:36.143923 async_tkinter_loop-0.8.0/README.md
+-rw-r--r--   0        0        0     2498 2023-04-24 18:22:36.143923 async_tkinter_loop-0.8.0/async_tkinter_loop.py
+-rw-r--r--   0        0        0     1292 2023-04-24 18:22:36.147923 async_tkinter_loop-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 async_tkinter_loop-0.8.0/PKG-INFO
```

### Comparing `async_tkinter_loop-0.7.0/LICENSE` & `async_tkinter_loop-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_tkinter_loop-0.7.0/README.md` & `async_tkinter_loop-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/async-tkinter-loop)
 <!--![PyPI - Downloads](https://img.shields.io/pypi/dm/async-tkinter-loop)-->
 
 Implementation of asynchronous `mainloop` for tkinter, the use of which allows using `async` handler functions.
 It is intended to be as simple to use as possible. No fancy unusual syntax or constructions - just use an alternative
 function instead of `root.mainloop()` and wrap asynchronous handlers into a helper function.
 
+> Please, fill free to [report bugs](https://github.com/insolor/async-tkinter-loop/issues), add [pull requests](https://github.com/insolor/async-tkinter-loop/pulls) or [share your thoughts / ask questions, etc.](https://github.com/insolor/async-tkinter-loop/discussions) about the module.
+
 Based on ideas from:
 
 * my answer on ru.stackoverflow.com: <https://ru.stackoverflow.com/a/1043146>
 * answer of [Terry Jan Reedy](https://stackoverflow.com/users/722804) on stackoverflow.com:
   <https://stackoverflow.com/a/47896365>
 * answer of [jfs](https://ru.stackoverflow.com/users/23044) on ru.stackoverflow.com:
   <https://ru.stackoverflow.com/a/804609>
@@ -29,15 +31,15 @@
 pip install async-tkinter-loop
 ```
 or
 ```
 pip install async-tkinter-loop[examples]
 ```
 
-- `[examples]` part is needed to install optional dependencies (such as `aiohttp` and `pillow`) to run some of the
+- `[examples]` part is needed to install optional dependencies (such as `httpx` and `pillow`) to run some of the
   examples. If you're not going to run examples, remove the `[examples]` part from the command
 - Use `pip3` instead of `pip` on Linux systems to install the package for python3 (not python2)
 - Probably you'll want to create a virtual environment for experiments with this library, but this is optional.
 - If you want to try examples, download the entire repository as an archive (green "code" button on
   [the github page](https://github.com/insolor/async-tkinter-loop) →
   "Download ZIP"), unpack, run any example (of course, you need to install optional dependencies)
```

### Comparing `async_tkinter_loop-0.7.0/async_tkinter_loop.py` & `async_tkinter_loop-0.8.0/async_tkinter_loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import _tkinter
 import asyncio
 import tkinter
 from functools import wraps
 from typing import Any, Callable, Coroutine
 
 from tkinter import TclError
 
@@ -9,17 +10,20 @@
 async def main_loop(root: tkinter.Tk) -> None:
     """
     An asynchronous implementation of tkinter mainloop
     :param root: tkinter root object
     :return: nothing
     """
     while True:
+        # Process all pending events
+        while root.dooneevent(_tkinter.DONT_WAIT):
+            pass
+
         try:
             root.winfo_exists()  # Will throw TclError if the main window is destroyed
-            root.update()
         except TclError:
             break
 
         await asyncio.sleep(0.01)
 
 
 def _get_event_loop() -> asyncio.AbstractEventLoop:
```

### Comparing `async_tkinter_loop-0.7.0/pyproject.toml` & `async_tkinter_loop-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-tkinter-loop"
-version = "0.7.0"
+version = "0.8.0"
 description = "Asynchronous mainloop implementation for tkinter"
 authors = ["insolor <insolor@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/insolor/async-tkinter-loop"
 repository = "https://github.com/insolor/async-tkinter-loop"
 keywords = ["tkinter", "async", "async-await", "asyncio", "aiohttp"]
@@ -16,24 +16,24 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 asyncio = "^3.4.3"
 Pillow = {version = "^9.1.1", optional = true}
-httpx = {version = "^0.23.0", optional = true}
+httpx = {version = "^0.23.1", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
+pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-timeout = "^2.0.1"
 flake8 = "^5.0.4"
 tkinter-stubs = { url = "https://github.com/insolor/tkinter-stubs/releases/download/0.1.0/tkinter_stubs-0.1.0-py3-none-any.whl" }
-black = "^22.10.0"
-isort = "^5.10.1"
+black = "^23.3.0"
+isort = "^5.11.5"
 
 [tool.poetry.extras]
 examples = ["httpx", "Pillow"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_tkinter_loop-0.7.0/setup.py` & `async_tkinter_loop-0.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,198 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: async-tkinter-loop
+Version: 0.8.0
+Summary: Asynchronous mainloop implementation for tkinter
+Home-page: https://github.com/insolor/async-tkinter-loop
+License: MIT
+Keywords: tkinter,async,async-await,asyncio,aiohttp
+Author: insolor
+Author-email: insolor@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: examples
+Requires-Dist: Pillow (>=9.1.1,<10.0.0) ; extra == "examples"
+Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: httpx (>=0.23.1,<0.24.0) ; extra == "examples"
+Project-URL: Repository, https://github.com/insolor/async-tkinter-loop
+Description-Content-Type: text/markdown
 
-modules = \
-['async_tkinter_loop']
-install_requires = \
-['asyncio>=3.4.3,<4.0.0']
-
-extras_require = \
-{'examples': ['Pillow>=9.1.1,<10.0.0', 'httpx>=0.23.0,<0.24.0']}
-
-setup_kwargs = {
-    'name': 'async-tkinter-loop',
-    'version': '0.7.0',
-    'description': 'Asynchronous mainloop implementation for tkinter',
-    'long_description': '# Asynchronous Tkinter Mainloop\n\n[![Python tests](https://github.com/insolor/async-tkinter-loop/actions/workflows/python-tests.yml/badge.svg)](https://github.com/insolor/async-tkinter-loop/actions/workflows/python-tests.yml)\n[![Coverage Status](https://coveralls.io/repos/github/insolor/async-tkinter-loop/badge.svg?branch=main)](https://coveralls.io/github/insolor/async-tkinter-loop?branch=main)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2566146b14ef72177613/maintainability)](https://codeclimate.com/github/insolor/async-tkinter-loop/maintainability)\n[![PyPI](https://img.shields.io/pypi/v/async-tkinter-loop)](https://pypi.org/project/async-tkinter-loop/)\n![Supported Python versions](https://img.shields.io/pypi/pyversions/async-tkinter-loop)\n<!--![PyPI - Downloads](https://img.shields.io/pypi/dm/async-tkinter-loop)-->\n\nImplementation of asynchronous `mainloop` for tkinter, the use of which allows using `async` handler functions.\nIt is intended to be as simple to use as possible. No fancy unusual syntax or constructions - just use an alternative\nfunction instead of `root.mainloop()` and wrap asynchronous handlers into a helper function.\n\nBased on ideas from:\n\n* my answer on ru.stackoverflow.com: <https://ru.stackoverflow.com/a/1043146>\n* answer of [Terry Jan Reedy](https://stackoverflow.com/users/722804) on stackoverflow.com:\n  <https://stackoverflow.com/a/47896365>\n* answer of [jfs](https://ru.stackoverflow.com/users/23044) on ru.stackoverflow.com:\n  <https://ru.stackoverflow.com/a/804609>\n\n## Installation\n\n### Release version\n\nInstall the package with the following command:\n\n```\npip install async-tkinter-loop\n```\nor\n```\npip install async-tkinter-loop[examples]\n```\n\n- `[examples]` part is needed to install optional dependencies (such as `aiohttp` and `pillow`) to run some of the\n  examples. If you\'re not going to run examples, remove the `[examples]` part from the command\n- Use `pip3` instead of `pip` on Linux systems to install the package for python3 (not python2)\n- Probably you\'ll want to create a virtual environment for experiments with this library, but this is optional.\n- If you want to try examples, download the entire repository as an archive (green "code" button on\n  [the github page](https://github.com/insolor/async-tkinter-loop) →\n  "Download ZIP"), unpack, run any example (of course, you need to install optional dependencies)\n\n### Development version\n\n1. Install [Poetry](https://python-poetry.org), e.g., with `pip install poetry` (`pip3 install poetry`) command\n   (other possible ways of installation see [here](https://python-poetry.org/docs/#installation))\n2. Download and unpack or clone [the repository](https://github.com/insolor/async-tkinter-loop).\n3. Run the command `poetry install` or `poetry install -E examples` (the later command installs optional dependencies\n   needed to run some examples). This command will create `.venv` directory with a virtual environment and\n   install dependencies into it.\n   - Run any example with `poetry run python examples/sparks.py` (insert a file name of an example).\n   - Or activate the virtual environment with `poetry shell` and run an example with `python examples/sparks.py`\n     command. You can also open the directory with the project in some IDE (e.g., PyCharm or VS Code) \n     and select Python interpreter from the virtual environment as a project interpreter,\n     then run examples directly from the IDE.\n\n## Some examples\n\nBasic example:\n```python\nimport asyncio\nimport tkinter as tk\n\nfrom async_tkinter_loop import async_handler, async_mainloop\n\n\nasync def counter():\n    i = 0\n    while True:\n        i += 1\n        label.config(text=str(i))\n        await asyncio.sleep(1.0)\n\n\nroot = tk.Tk()\n\nlabel = tk.Label(root)\nlabel.pack()\n\ntk.Button(root, text="Start", command=async_handler(counter)).pack()\n\nasync_mainloop(root)\n```\n\nAlso, `async_handler` function can be used as a decorator (but it makes a decorated function syncroneous):\n\n```python\nimport asyncio\nimport tkinter as tk\n\nfrom async_tkinter_loop import async_handler, async_mainloop\n\n\n@async_handler\nasync def counter():\n    i = 0\n    while True:\n        i += 1\n        label.config(text=str(i))\n        await asyncio.sleep(1.0)\n\n\nroot = tk.Tk()\n\nlabel = tk.Label(root)\nlabel.pack()\n\ntk.Button(root, text="Start", command=counter).pack()\n\nasync_mainloop(root)\n```\n\nA more practical example, downloading an image from the Internet with [httpx](https://github.com/encode/httpx)\n(you can use [aiohttp](https://github.com/aio-libs/aiohttp) as well)\nand displaying it in the Tkinter window:\n\n```python\nimport tkinter as tk\nfrom io import BytesIO\n\nimport httpx\nfrom PIL import Image, ImageTk\n\nfrom async_tkinter_loop import async_handler, async_mainloop\n\n\nasync def load_image(url):\n    button.config(state=tk.DISABLED)\n    label.config(text="Loading...", image="")\n\n    async with httpx.AsyncClient() as client:\n        response = await client.get(url, follow_redirects=True)\n        if response.status_code != 200:\n            label.config(text=f"HTTP error {response.status_code}")\n        else:\n            content = response.content\n            pil_image = Image.open(BytesIO(content))\n            image = ImageTk.PhotoImage(pil_image)\n            label.image = image\n            label.config(image=image, text="")\n            button.config(state=tk.NORMAL)\n\n\nurl = "https://picsum.photos/800/640"\n\nroot = tk.Tk()\nroot.geometry("800x640")\n\nbutton = tk.Button(root, text="Load an image", command=async_handler(load_image, url))\nbutton.pack()\n\nlabel = tk.Label(root)\nlabel.pack(expand=1, fill=tk.BOTH)\n\nasync_mainloop(root)\n```\n\nMore examples see in the [`examples`](https://github.com/insolor/async-tkinter-loop/tree/main/examples) directory.\n\n\n## Similar projects\n\n* [Starwort/asynctk](https://github.com/Starwort/asynctk) ([on PyPi](https://pypi.org/project/asynctk/))\n* [gottadiveintopython/asynctkinter](https://github.com/gottadiveintopython/asynctkinter) ([on PyPi](https://pypi.org/project/asynctkinter/))\n* [Lucretiel/tkinter-async](https://github.com/Lucretiel/tkinter-async)\n* [fluentpython/asyncio-tkinter](https://github.com/fluentpython/asyncio-tkinter)\n',
-    'author': 'insolor',
-    'author_email': 'insolor@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/insolor/async-tkinter-loop',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+# Asynchronous Tkinter Mainloop
 
+[![Python tests](https://github.com/insolor/async-tkinter-loop/actions/workflows/python-tests.yml/badge.svg)](https://github.com/insolor/async-tkinter-loop/actions/workflows/python-tests.yml)
+[![Coverage Status](https://coveralls.io/repos/github/insolor/async-tkinter-loop/badge.svg?branch=main)](https://coveralls.io/github/insolor/async-tkinter-loop?branch=main)
+[![Maintainability](https://api.codeclimate.com/v1/badges/2566146b14ef72177613/maintainability)](https://codeclimate.com/github/insolor/async-tkinter-loop/maintainability)
+[![PyPI](https://img.shields.io/pypi/v/async-tkinter-loop)](https://pypi.org/project/async-tkinter-loop/)
+![Supported Python versions](https://img.shields.io/pypi/pyversions/async-tkinter-loop)
+<!--![PyPI - Downloads](https://img.shields.io/pypi/dm/async-tkinter-loop)-->
+
+Implementation of asynchronous `mainloop` for tkinter, the use of which allows using `async` handler functions.
+It is intended to be as simple to use as possible. No fancy unusual syntax or constructions - just use an alternative
+function instead of `root.mainloop()` and wrap asynchronous handlers into a helper function.
+
+> Please, fill free to [report bugs](https://github.com/insolor/async-tkinter-loop/issues), add [pull requests](https://github.com/insolor/async-tkinter-loop/pulls) or [share your thoughts / ask questions, etc.](https://github.com/insolor/async-tkinter-loop/discussions) about the module.
+
+Based on ideas from:
+
+* my answer on ru.stackoverflow.com: <https://ru.stackoverflow.com/a/1043146>
+* answer of [Terry Jan Reedy](https://stackoverflow.com/users/722804) on stackoverflow.com:
+  <https://stackoverflow.com/a/47896365>
+* answer of [jfs](https://ru.stackoverflow.com/users/23044) on ru.stackoverflow.com:
+  <https://ru.stackoverflow.com/a/804609>
+
+## Installation
+
+### Release version
+
+Install the package with the following command:
+
+```
+pip install async-tkinter-loop
+```
+or
+```
+pip install async-tkinter-loop[examples]
+```
+
+- `[examples]` part is needed to install optional dependencies (such as `httpx` and `pillow`) to run some of the
+  examples. If you're not going to run examples, remove the `[examples]` part from the command
+- Use `pip3` instead of `pip` on Linux systems to install the package for python3 (not python2)
+- Probably you'll want to create a virtual environment for experiments with this library, but this is optional.
+- If you want to try examples, download the entire repository as an archive (green "code" button on
+  [the github page](https://github.com/insolor/async-tkinter-loop) →
+  "Download ZIP"), unpack, run any example (of course, you need to install optional dependencies)
+
+### Development version
+
+1. Install [Poetry](https://python-poetry.org), e.g., with `pip install poetry` (`pip3 install poetry`) command
+   (other possible ways of installation see [here](https://python-poetry.org/docs/#installation))
+2. Download and unpack or clone [the repository](https://github.com/insolor/async-tkinter-loop).
+3. Run the command `poetry install` or `poetry install -E examples` (the later command installs optional dependencies
+   needed to run some examples). This command will create `.venv` directory with a virtual environment and
+   install dependencies into it.
+   - Run any example with `poetry run python examples/sparks.py` (insert a file name of an example).
+   - Or activate the virtual environment with `poetry shell` and run an example with `python examples/sparks.py`
+     command. You can also open the directory with the project in some IDE (e.g., PyCharm or VS Code) 
+     and select Python interpreter from the virtual environment as a project interpreter,
+     then run examples directly from the IDE.
+
+## Some examples
+
+Basic example:
+```python
+import asyncio
+import tkinter as tk
+
+from async_tkinter_loop import async_handler, async_mainloop
+
+
+async def counter():
+    i = 0
+    while True:
+        i += 1
+        label.config(text=str(i))
+        await asyncio.sleep(1.0)
+
+
+root = tk.Tk()
+
+label = tk.Label(root)
+label.pack()
+
+tk.Button(root, text="Start", command=async_handler(counter)).pack()
+
+async_mainloop(root)
+```
+
+Also, `async_handler` function can be used as a decorator (but it makes a decorated function syncroneous):
+
+```python
+import asyncio
+import tkinter as tk
+
+from async_tkinter_loop import async_handler, async_mainloop
+
+
+@async_handler
+async def counter():
+    i = 0
+    while True:
+        i += 1
+        label.config(text=str(i))
+        await asyncio.sleep(1.0)
+
+
+root = tk.Tk()
+
+label = tk.Label(root)
+label.pack()
+
+tk.Button(root, text="Start", command=counter).pack()
+
+async_mainloop(root)
+```
+
+A more practical example, downloading an image from the Internet with [httpx](https://github.com/encode/httpx)
+(you can use [aiohttp](https://github.com/aio-libs/aiohttp) as well)
+and displaying it in the Tkinter window:
+
+```python
+import tkinter as tk
+from io import BytesIO
+
+import httpx
+from PIL import Image, ImageTk
+
+from async_tkinter_loop import async_handler, async_mainloop
+
+
+async def load_image(url):
+    button.config(state=tk.DISABLED)
+    label.config(text="Loading...", image="")
+
+    async with httpx.AsyncClient() as client:
+        response = await client.get(url, follow_redirects=True)
+        if response.status_code != 200:
+            label.config(text=f"HTTP error {response.status_code}")
+        else:
+            content = response.content
+            pil_image = Image.open(BytesIO(content))
+            image = ImageTk.PhotoImage(pil_image)
+            label.image = image
+            label.config(image=image, text="")
+            button.config(state=tk.NORMAL)
+
+
+url = "https://picsum.photos/800/640"
+
+root = tk.Tk()
+root.geometry("800x640")
+
+button = tk.Button(root, text="Load an image", command=async_handler(load_image, url))
+button.pack()
+
+label = tk.Label(root)
+label.pack(expand=1, fill=tk.BOTH)
+
+async_mainloop(root)
+```
+
+More examples see in the [`examples`](https://github.com/insolor/async-tkinter-loop/tree/main/examples) directory.
+
+
+## Similar projects
+
+* [Starwort/asynctk](https://github.com/Starwort/asynctk) ([on PyPi](https://pypi.org/project/asynctk/))
+* [gottadiveintopython/asynctkinter](https://github.com/gottadiveintopython/asynctkinter) ([on PyPi](https://pypi.org/project/asynctkinter/))
+* [Lucretiel/tkinter-async](https://github.com/Lucretiel/tkinter-async)
+* [fluentpython/asyncio-tkinter](https://github.com/fluentpython/asyncio-tkinter)
 
-setup(**setup_kwargs)
```

