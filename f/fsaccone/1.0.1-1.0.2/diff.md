# Comparing `tmp/fsaccone-1.0.1.tar.gz` & `tmp/fsaccone-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsaccone-1.0.1.tar", max compression
+gzip compressed data, was "fsaccone-1.0.2.tar", max compression
```

## Comparing `fsaccone-1.0.1.tar` & `fsaccone-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-24 15:06:38.075273 fsaccone-1.0.1/fsaccone/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 15:06:38.077273 fsaccone-1.0.1/fsaccone/app/__init__.py
--rw-r--r--   0        0        0     2016 2023-04-24 15:06:38.078790 fsaccone-1.0.1/fsaccone/app/build.py
--rw-r--r--   0        0        0        0 2023-04-24 15:06:38.078790 fsaccone-1.0.1/fsaccone/app/cli/__init__.py
--rw-r--r--   0        0        0      586 2023-04-24 15:06:38.080808 fsaccone-1.0.1/fsaccone/app/cli/confirm.py
--rw-r--r--   0        0        0      316 2023-04-24 15:06:38.080808 fsaccone-1.0.1/fsaccone/app/cli/help.py
--rw-r--r--   0        0        0      291 2023-04-24 15:06:38.081826 fsaccone-1.0.1/fsaccone/app/cli/unknown.py
--rw-r--r--   0        0        0      781 2023-04-24 15:07:50.033405 fsaccone-1.0.1/fsaccone/app/start.py
--rw-r--r--   0        0        0        0 2023-04-24 15:06:38.082827 fsaccone-1.0.1/fsaccone/app/utils/__init__.py
--rw-r--r--   0        0        0      293 2023-04-24 15:06:38.083826 fsaccone-1.0.1/fsaccone/app/utils/fetch.py
--rw-r--r--   0        0        0      931 2023-04-24 15:06:38.084826 fsaccone-1.0.1/fsaccone/app/utils/logger.py
--rw-r--r--   0        0        0      622 2023-04-24 15:06:38.086826 fsaccone-1.0.1/fsaccone/app/utils/templates.py
--rw-r--r--   0        0        0     1141 2023-04-24 15:06:38.086826 fsaccone-1.0.1/fsaccone/args.py
--rw-r--r--   0        0        0      158 2023-04-24 15:06:38.088823 fsaccone-1.0.1/fsaccone/main.py
--rw-r--r--   0        0        0     1095 2023-04-24 15:06:38.074271 fsaccone-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      433 2023-04-24 15:08:10.526762 fsaccone-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      508 2023-04-24 15:06:38.075273 fsaccone-1.0.1/README.md
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 fsaccone-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 15:13:41.473456 fsaccone-1.0.2/fsaccone/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:13:41.473456 fsaccone-1.0.2/fsaccone/app/__init__.py
+-rw-r--r--   0        0        0     1997 2023-04-24 15:35:36.700528 fsaccone-1.0.2/fsaccone/app/build.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:13:41.475469 fsaccone-1.0.2/fsaccone/app/cli/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-24 15:13:41.476467 fsaccone-1.0.2/fsaccone/app/cli/confirm.py
+-rw-r--r--   0        0        0      316 2023-04-24 15:13:41.477468 fsaccone-1.0.2/fsaccone/app/cli/help.py
+-rw-r--r--   0        0        0      291 2023-04-24 15:13:41.478467 fsaccone-1.0.2/fsaccone/app/cli/unknown.py
+-rw-r--r--   0        0        0      929 2023-04-24 15:33:04.578913 fsaccone-1.0.2/fsaccone/app/start.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:13:41.479466 fsaccone-1.0.2/fsaccone/app/utils/__init__.py
+-rw-r--r--   0        0        0      293 2023-04-24 15:13:41.480467 fsaccone-1.0.2/fsaccone/app/utils/fetch.py
+-rw-r--r--   0        0        0      931 2023-04-24 15:13:41.481466 fsaccone-1.0.2/fsaccone/app/utils/logger.py
+-rw-r--r--   0        0        0      622 2023-04-24 15:13:41.482467 fsaccone-1.0.2/fsaccone/app/utils/templates.py
+-rw-r--r--   0        0        0     1273 2023-04-24 15:31:44.768037 fsaccone-1.0.2/fsaccone/args.py
+-rw-r--r--   0        0        0      158 2023-04-24 15:13:41.483725 fsaccone-1.0.2/fsaccone/main.py
+-rw-r--r--   0        0        0     1095 2023-04-24 15:13:41.470931 fsaccone-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      433 2023-04-24 15:14:05.454613 fsaccone-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      569 2023-04-24 15:22:57.867412 fsaccone-1.0.2/README.md
+-rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 fsaccone-1.0.2/PKG-INFO
```

### Comparing `fsaccone-1.0.1/fsaccone/app/cli/confirm.py` & `fsaccone-1.0.2/fsaccone/app/cli/confirm.py`

 * *Files identical despite different names*

### Comparing `fsaccone-1.0.1/fsaccone/app/start.py` & `fsaccone-1.0.2/fsaccone/app/start.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from .build import build_template
 from .cli.confirm import confirmation
 from .cli.help import help_message
 from .cli.unknown import unknown_template_message
 from .utils.templates import get_templates
+from .utils.logger import log_information
 import os
+import pkg_resources
 
 
 def start_app(args) -> None:
+    if args["version"]:
+        print(f'v{pkg_resources.get_distribution("fsaccone").version}')
+        return
+
     templates = get_templates()
 
     template = args["template"]
     directory = os.path.abspath(args["directory"]) if args["directory"] else os.getcwd()
 
-    if not os.path.exists(directory):
-        os.makedirs(directory)
+    os.makedirs(directory, exist_ok=True)
 
     if not template:
         help_message(templates)
         return
 
     if not template in templates:
         unknown_template_message(template, templates)
```

### Comparing `fsaccone-1.0.1/fsaccone/app/utils/logger.py` & `fsaccone-1.0.2/fsaccone/app/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fsaccone-1.0.1/fsaccone/app/utils/templates.py` & `fsaccone-1.0.2/fsaccone/app/utils/templates.py`

 * *Files identical despite different names*

### Comparing `fsaccone-1.0.1/fsaccone/args.py` & `fsaccone-1.0.2/fsaccone/args.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,62 @@
-import argparse
-import sys
-from typing import Dict
-
-
-def _parse_args() -> argparse.Namespace:
-    args_parser = argparse.ArgumentParser()
-
-    args_parser.add_argument(
-        "--directory",
-        "--dir",
-        "-d",
-        action="store",
-        default=[None],
-        nargs=1,
-        type=str,
-    )
-    args_parser.add_argument(
-        "--template",
-        "-t",
-        action="store",
-        default=[None],
-        nargs=1,
-        type=str,
-    )
-    args_parser.add_argument(
-        "-y",
-        action="store_true",
-        default=False,
-    )
-
-    args, unknown = args_parser.parse_known_args(sys.argv[1:])
-    return args
-
-
-def get_none_or_normalized_string(string: str | None) -> str | None:
-    return string.lower().strip() if type(string) == str else None
-
-
-def get_args() -> Dict:
-    args = _parse_args()
-
-    directory = get_none_or_normalized_string(args.directory[0])
-
-    template = get_none_or_normalized_string(args.template[0])
-
-    y: bool = args.y
-
-    return {
-        "directory": directory,
-        "template": template,
-        "y": y,
-    }
+import argparse
+import sys
+from typing import Dict
+
+
+def _parse_args() -> argparse.Namespace:
+    args_parser = argparse.ArgumentParser()
+
+    args_parser.add_argument(
+        "--directory",
+        "--dir",
+        "-d",
+        action="store",
+        default=[None],
+        nargs=1,
+        type=str,
+    )
+    args_parser.add_argument(
+        "--template",
+        "-t",
+        action="store",
+        default=[None],
+        nargs=1,
+        type=str,
+    )
+    args_parser.add_argument(
+        "--version",
+        "-v",
+        action="store_true",
+        default=False,
+    )
+    args_parser.add_argument(
+        "-y",
+        action="store_true",
+        default=False,
+    )
+
+    args, unknown = args_parser.parse_known_args(sys.argv[1:])
+    return args
+
+
+def get_none_or_normalized_string(string: str | None) -> str | None:
+    return string.lower().strip() if type(string) == str else None
+
+
+def get_args() -> Dict:
+    args = _parse_args()
+
+    directory = get_none_or_normalized_string(args.directory[0])
+
+    template = get_none_or_normalized_string(args.template[0])
+
+    version: bool = args.version
+
+    y: bool = args.y
+
+    return {
+        "directory": directory,
+        "template": template,
+        "version": version,
+        "y": y,
+    }
```

### Comparing `fsaccone-1.0.1/LICENSE.txt` & `fsaccone-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fsaccone-1.0.1/PKG-INFO` & `fsaccone-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsaccone
-Version: 1.0.1
+Version: 1.0.2
 Summary: A CLI that creates opinionated project templates.
 Home-page: https://github.com/fsaccone/cli
 License: MIT
 Author: Francesco Saccone
 Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,16 @@
 ## Installation
 > `pip install fsaccone`
 
 ## Usage
 > `fsaccone --template <TEMPLATE>`
 
 ## Flags
+- `--version` / `-v`                          - Prints the package version.
+
 - `--template` / `-t` `<TEMPLATE>`            - The name of the template to utilize.
 - `--directory` / `-dir` / `-d` `<DIRECTORY>` - The directory to build the template in.
 - `-y`                                        - Skips the confirmation alert.
 
 ## License
 [MIT License](LICENSE.txt)
```

