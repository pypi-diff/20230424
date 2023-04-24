# Comparing `tmp/rainbowlog-2.0.3.tar.gz` & `tmp/rainbowlog-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbowlog-2.0.3.tar", max compression
+gzip compressed data, was "rainbowlog-2.0.4.tar", max compression
```

## Comparing `rainbowlog-2.0.3.tar` & `rainbowlog-2.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2022-08-17 19:12:31.315991 rainbowlog-2.0.3/LICENSE
--rw-r--r--   0        0        0     2843 2022-08-17 19:12:31.315991 rainbowlog-2.0.3/README.md
--rw-r--r--   0        0        0      811 2022-08-17 19:12:40.228239 rainbowlog-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      288 2022-08-17 19:12:31.315991 rainbowlog-2.0.3/rainbowlog/__init__.py
--rw-r--r--   0        0        0     2533 2022-08-17 19:12:31.315991 rainbowlog-2.0.3/rainbowlog/_formatter.py
--rw-r--r--   0        0        0        1 2022-08-17 19:12:31.315991 rainbowlog-2.0.3/rainbowlog/py.typed
--rw-r--r--   0        0        0     3678 2022-08-17 19:12:41.305214 rainbowlog-2.0.3/setup.py
--rw-r--r--   0        0        0     3730 2022-08-17 19:12:41.305613 rainbowlog-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-24 13:51:49.273647 rainbowlog-2.0.4/LICENSE
+-rw-r--r--   0        0        0     2843 2023-04-24 13:51:49.273647 rainbowlog-2.0.4/README.md
+-rw-r--r--   0        0        0      811 2023-04-24 13:52:05.941698 rainbowlog-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-04-24 13:51:49.273647 rainbowlog-2.0.4/rainbowlog/__init__.py
+-rw-r--r--   0        0        0     2533 2023-04-24 13:51:49.273647 rainbowlog-2.0.4/rainbowlog/_formatter.py
+-rw-r--r--   0        0        0        1 2023-04-24 13:51:49.273647 rainbowlog-2.0.4/rainbowlog/py.typed
+-rw-r--r--   0        0        0     3678 2023-04-24 13:52:07.185662 rainbowlog-2.0.4/setup.py
+-rw-r--r--   0        0        0     3730 2023-04-24 13:52:07.186052 rainbowlog-2.0.4/PKG-INFO
```

### Comparing `rainbowlog-2.0.3/LICENSE` & `rainbowlog-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rainbowlog-2.0.3/README.md` & `rainbowlog-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rainbowlog-2.0.3/pyproject.toml` & `rainbowlog-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "rainbowlog"
 # Version is overwritten at build time by CI based on git tag
-version = "2.0.3"
+version = "2.0.4"
 description = "Format your python logs with colours based on the log levels."
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/rainbowlog"
 documentation = "https://abrahammurciano.github.io/rainbowlog/rainbowlog/"
 keywords = ["logging", "color"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-metadata = ">=4.11"
-constyle = ">=1.0.2"
+constyle = ">=2.0.3"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1"
 pdoc3 = ">=0.10.0"
 types-toml = ">=0.10.7"
 black = { version = ">=22.3.0", allow-prereleases = true }
 mypy = ">=0.961"
```

### Comparing `rainbowlog-2.0.3/rainbowlog/_formatter.py` & `rainbowlog-2.0.4/rainbowlog/_formatter.py`

 * *Files identical despite different names*

### Comparing `rainbowlog-2.0.3/setup.py` & `rainbowlog-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['rainbowlog']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['constyle>=1.0.2', 'importlib-metadata>=4.11']
+['constyle>=2.0.3', 'importlib-metadata>=4.11']
 
 setup_kwargs = {
     'name': 'rainbowlog',
-    'version': '2.0.3',
+    'version': '2.0.4',
     'description': 'Format your python logs with colours based on the log levels.',
     'long_description': '# Rainbow Log\n\nFormat your python logs with colours based on the log levels.\n\n## Installation\n\nYou can instll the package with pip or conda.\n```sh\n$ pip install rainbowlog\n```\n```sh\n$ conda install rainbowlog -c abrahammurciano\n```\n```sh\n$ conda install rainbowlog -c conda-forge\n```\n\n## Links\n\n* [Documentation](https://abrahammurciano.github.io/rainbowlog/rainbowlog)\n* [Github](https://github.com/abrahammurciano/rainbowlog)\n* [PyPI](https://pypi.org/project/rainbowlog/)\n\n## Usage\n\nHere\'s a basic example of a script that logs colorfully to the console, but regularly to a file.\n\n```python\nimport logging\nimport rainbowlog\n\nlogger = logging.getLogger(__name__)\n\n# This one will write to the console\nstream_handler = logging.StreamHandler()\n\n# This one will write to a file\nfile_handler = logging.FileHandler("output.log")\n\n# Here we decide how we want the logs to look like\nformatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")\n\n# We want the stream handler to be colorful\nstream_handler.setFormatter(rainbowlog.Formatter(formatter))\n\n# We don\'t want the file handler to be colorful\nfile_handler.setFormatter(formatter)\n\n# Finally we add the handlers to the logger\nlogger.addHandler(stream_handler)\nlogger.addHandler(file_handler)\n\nif __name__ == "__main__":\n\tlogger.debug("This is a debug message")\n\tlogger.info("This is an info message")\n\tlogger.warning("This is a warning message")\n\tlogger.error("This is an error message")\n\tlogger.critical("This is a critical message")\n```\n\nIf you want to change the format of the logs for each log level, you can use any callable that takes a string and returns the same string with ANSI codes surrounding it. There are many libraries you can use to provide such callables.\n\n```py\nimport logging\nfrom rainbowlog import Formatter\n\n# Here are some libraries you can use to get a style callable without dealing with ANSI codes\nfrom constyle import Style, Attributes as Attrs\nimport termcolor\nfrom functools import partial\n\n\nformatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")\ncolor_formatter = Formatter(\n\tformatter,\n\tlog_styles={\n\t\tlogging.DEBUG: Style(Attrs.BLUE, Attrs.FAINT), # An example using constyle\n\t\tlogging.INFO: lambda s: f"\\033[32m{s}\\033[0m", # An example using lambdas\n\t\tlogging.WARNING: termcolor.red, # An example using termcolor\'s predifined functions\n\t\tlogging.ERROR: partial(termcolor.colored, color="red", on_color="on_white", attrs=["bold"]), # An example using functools.partial\n\t\tlogging.CRITICAL: Attrs.RED + Attrs.ON_YELLOW + Attrs.BOLD + Attrs.UNDERLINE, # An example using constyle\'s added attributes\n\t}\n\texception_style=lambda s: f"{Attrs.RED + Attrs.ON_WHITE + Attrs.BOLD}{s}{Attrs.RESET}" # An example using lambdas and constyle,\n\tstack_style=Attrs.RED, # An example using a single constyle attribute\n)\n```',
     'author': 'Abraham Murciano',
     'author_email': 'abrahammurciano@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/abrahammurciano/rainbowlog',
```

### Comparing `rainbowlog-2.0.3/PKG-INFO` & `rainbowlog-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rainbowlog
-Version: 2.0.3
+Version: 2.0.4
 Summary: Format your python logs with colours based on the log levels.
 Home-page: https://github.com/abrahammurciano/rainbowlog
 License: MIT
 Keywords: logging,color
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: constyle (>=1.0.2)
+Requires-Dist: constyle (>=2.0.3)
 Requires-Dist: importlib-metadata (>=4.11)
 Project-URL: Documentation, https://abrahammurciano.github.io/rainbowlog/rainbowlog/
 Project-URL: Repository, https://github.com/abrahammurciano/rainbowlog
 Description-Content-Type: text/markdown
 
 # Rainbow Log
```

