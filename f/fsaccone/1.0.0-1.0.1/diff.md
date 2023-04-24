# Comparing `tmp/fsaccone-1.0.0.tar.gz` & `tmp/fsaccone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsaccone-1.0.0.tar", max compression
+gzip compressed data, was "fsaccone-1.0.1.tar", max compression
```

## Comparing `fsaccone-1.0.0.tar` & `fsaccone-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-24 10:21:07.809675 fsaccone-1.0.0/fsaccone/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 10:54:07.938217 fsaccone-1.0.0/fsaccone/app/__init__.py
--rw-r--r--   0        0        0     1956 2023-04-24 14:17:24.826788 fsaccone-1.0.0/fsaccone/app/build.py
--rw-r--r--   0        0        0        0 2023-04-24 12:04:27.429480 fsaccone-1.0.0/fsaccone/app/cli/__init__.py
--rw-r--r--   0        0        0      565 2023-04-24 14:17:44.846457 fsaccone-1.0.0/fsaccone/app/cli/confirm.py
--rw-r--r--   0        0        0      306 2023-04-24 14:25:01.096065 fsaccone-1.0.0/fsaccone/app/cli/help.py
--rw-r--r--   0        0        0      283 2023-04-24 14:19:26.195818 fsaccone-1.0.0/fsaccone/app/cli/unknown.py
--rw-r--r--   0        0        0      711 2023-04-24 14:21:18.746049 fsaccone-1.0.0/fsaccone/app/start.py
--rw-r--r--   0        0        0        0 2023-04-24 12:39:20.835488 fsaccone-1.0.0/fsaccone/app/utils/__init__.py
--rw-r--r--   0        0        0      279 2023-04-24 14:17:36.449607 fsaccone-1.0.0/fsaccone/app/utils/fetch.py
--rw-r--r--   0        0        0      889 2023-04-24 14:16:41.750397 fsaccone-1.0.0/fsaccone/app/utils/logger.py
--rw-r--r--   0        0        0      593 2023-04-24 14:19:58.860367 fsaccone-1.0.0/fsaccone/app/utils/templates.py
--rw-r--r--   0        0        0     1088 2023-04-24 13:36:07.838041 fsaccone-1.0.0/fsaccone/args.py
--rw-r--r--   0        0        0      148 2023-04-24 14:16:59.879491 fsaccone-1.0.0/fsaccone/main.py
--rw-r--r--   0        0        0     1074 2023-04-24 14:29:34.714879 fsaccone-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      433 2023-04-24 14:51:38.587880 fsaccone-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      454 2023-04-24 14:30:16.702462 fsaccone-1.0.0/README.md
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 fsaccone-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 15:06:38.075273 fsaccone-1.0.1/fsaccone/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:06:38.077273 fsaccone-1.0.1/fsaccone/app/__init__.py
+-rw-r--r--   0        0        0     2016 2023-04-24 15:06:38.078790 fsaccone-1.0.1/fsaccone/app/build.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:06:38.078790 fsaccone-1.0.1/fsaccone/app/cli/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-24 15:06:38.080808 fsaccone-1.0.1/fsaccone/app/cli/confirm.py
+-rw-r--r--   0        0        0      316 2023-04-24 15:06:38.080808 fsaccone-1.0.1/fsaccone/app/cli/help.py
+-rw-r--r--   0        0        0      291 2023-04-24 15:06:38.081826 fsaccone-1.0.1/fsaccone/app/cli/unknown.py
+-rw-r--r--   0        0        0      781 2023-04-24 15:07:50.033405 fsaccone-1.0.1/fsaccone/app/start.py
+-rw-r--r--   0        0        0        0 2023-04-24 15:06:38.082827 fsaccone-1.0.1/fsaccone/app/utils/__init__.py
+-rw-r--r--   0        0        0      293 2023-04-24 15:06:38.083826 fsaccone-1.0.1/fsaccone/app/utils/fetch.py
+-rw-r--r--   0        0        0      931 2023-04-24 15:06:38.084826 fsaccone-1.0.1/fsaccone/app/utils/logger.py
+-rw-r--r--   0        0        0      622 2023-04-24 15:06:38.086826 fsaccone-1.0.1/fsaccone/app/utils/templates.py
+-rw-r--r--   0        0        0     1141 2023-04-24 15:06:38.086826 fsaccone-1.0.1/fsaccone/args.py
+-rw-r--r--   0        0        0      158 2023-04-24 15:06:38.088823 fsaccone-1.0.1/fsaccone/main.py
+-rw-r--r--   0        0        0     1095 2023-04-24 15:06:38.074271 fsaccone-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      433 2023-04-24 15:08:10.526762 fsaccone-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      508 2023-04-24 15:06:38.075273 fsaccone-1.0.1/README.md
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 fsaccone-1.0.1/PKG-INFO
```

### Comparing `fsaccone-1.0.0/fsaccone/app/cli/confirm.py` & `fsaccone-1.0.1/fsaccone/app/cli/confirm.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from ..utils import logger
-
-
-def _get_confirmation_input() -> bool:
-    logger.log_important("(y/n) ", newline=False)
-    confirmation = input().lower().strip()
-
-    if not (confirmation == "y" or confirmation == "n"):
-        return _get_confirmation_input()
-
-    return True if confirmation == "y" else False
-
-
-def confirmation(dir: str) -> bool:
-    logger.log_information(
-        "Are you sure you want to continue?",
-        newline=False,
-    )
-    logger.log_important(f' All of the files in "{dir}" will be deleted.')
-
-    return _get_confirmation_input()
+from ..utils import logger
+
+
+def _get_confirmation_input() -> bool:
+    logger.log_important("(y/n) ", newline=False)
+    confirmation = input().lower().strip()
+
+    if not (confirmation == "y" or confirmation == "n"):
+        return _get_confirmation_input()
+
+    return True if confirmation == "y" else False
+
+
+def confirmation(dir: str) -> bool:
+    logger.log_information(
+        "Are you sure you want to continue?",
+        newline=False,
+    )
+    logger.log_important(f' All of the files in "{dir}" will be deleted.')
+
+    return _get_confirmation_input()
```

### Comparing `fsaccone-1.0.0/fsaccone/app/start.py` & `fsaccone-1.0.1/fsaccone/app/start.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 def start_app(args) -> None:
     templates = get_templates()
 
     template = args["template"]
     directory = os.path.abspath(args["directory"]) if args["directory"] else os.getcwd()
 
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
     if not template:
         help_message(templates)
         return
 
     if not template in templates:
         unknown_template_message(template, templates)
         return
```

### Comparing `fsaccone-1.0.0/fsaccone/app/utils/logger.py` & `fsaccone-1.0.1/fsaccone/app/utils/logger.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from rich.console import Console
-from typing import List
-
-console = Console(color_system="standard")
-
-
-def log_status(*text: List[str], newline=True) -> None:
-    console.print(
-        *text,
-        style="cyan",
-        end="\n" if newline else "",
-    )
-
-
-def log_important(*text: List[str], newline=True) -> None:
-    console.print(
-        *text,
-        style="bold red",
-        end="\n" if newline else "",
-    )
-
-
-def log_information(*text: List[str], newline=True) -> None:
-    console.print(
-        *text,
-        style="italic bright_black",
-        end="\n" if newline else "",
-    )
-
-
-def log_list(list: List[str], newline=True) -> None:
-    for element in list:
-        console.print(
-            "  - ",
-            style="bright_black",
-            end="",
-        )
-        console.print(
-            element,
-            style="green",
-            end="\n",
-        )
+from rich.console import Console
+from typing import List
+
+console = Console(color_system="standard")
+
+
+def log_status(*text: List[str], newline=True) -> None:
+    console.print(
+        *text,
+        style="cyan",
+        end="\n" if newline else "",
+    )
+
+
+def log_important(*text: List[str], newline=True) -> None:
+    console.print(
+        *text,
+        style="bold red",
+        end="\n" if newline else "",
+    )
+
+
+def log_information(*text: List[str], newline=True) -> None:
+    console.print(
+        *text,
+        style="italic bright_black",
+        end="\n" if newline else "",
+    )
+
+
+def log_list(list: List[str], newline=True) -> None:
+    for element in list:
+        console.print(
+            "  - ",
+            style="bright_black",
+            end="",
+        )
+        console.print(
+            element,
+            style="green",
+            end="\n",
+        )
```

### Comparing `fsaccone-1.0.0/LICENSE.txt` & `fsaccone-1.0.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Francesco Saccone
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Francesco Saccone
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `fsaccone-1.0.0/PKG-INFO` & `fsaccone-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsaccone
-Version: 1.0.0
+Version: 1.0.1
 Summary: A CLI that creates opinionated project templates.
 Home-page: https://github.com/fsaccone/cli
 License: MIT
 Author: Francesco Saccone
 Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rich (==13.3.4)
 Description-Content-Type: text/markdown
 
-# CLI (fsaccone)
+# CLI ([fsaccone](https://pypi.org/project/fsaccone/))
 A CLI that creates opinionated project templates.
 
 ## Installation
 > `pip install fsaccone`
 
 ## Usage
 > `fsaccone --template <TEMPLATE>`
```

