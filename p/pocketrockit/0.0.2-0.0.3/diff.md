# Comparing `tmp/pocketrockit-0.0.2.tar.gz` & `tmp/pocketrockit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketrockit-0.0.2.tar", max compression
+gzip compressed data, was "pocketrockit-0.0.3.tar", max compression
```

## Comparing `pocketrockit-0.0.2.tar` & `pocketrockit-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2636 2023-04-24 06:19:57.288246 pocketrockit-0.0.2/Readme.md
--rw-r--r--   0        0        0        0 2023-04-21 04:17:33.520420 pocketrockit-0.0.2/pocketrockit/__init__.py
--rwxr-xr-x   0        0        0      532 2023-04-23 12:22:42.315502 pocketrockit-0.0.2/pocketrockit/cli.py
--rwxr-xr-x   0        0        0    10698 2023-04-24 06:09:42.435969 pocketrockit-0.0.2/pocketrockit/decorated.py
--rwxr-xr-x   0        0        0     8253 2023-04-24 06:09:42.407969 pocketrockit-0.0.2/pocketrockit/engine.py
--rw-r--r--   0        0        0     1868 2023-04-24 06:22:20.691311 pocketrockit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 pocketrockit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2636 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/pocketrockit/__init__.py
+-rwxr-xr-x   0        0        0      532 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/pocketrockit/cli.py
+-rwxr-xr-x   0        0        0    10829 2023-04-24 08:05:55.081996 pocketrockit-0.0.3/pocketrockit/decorated.py
+-rwxr-xr-x   0        0        0     8253 2023-04-24 06:41:37.681837 pocketrockit-0.0.3/pocketrockit/engine.py
+-rw-r--r--   0        0        0     1868 2023-04-24 08:08:10.873576 pocketrockit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 pocketrockit-0.0.3/PKG-INFO
```

### Comparing `pocketrockit-0.0.2/Readme.md` & `pocketrockit-0.0.3/Readme.md`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.2/pocketrockit/cli.py` & `pocketrockit-0.0.3/pocketrockit/cli.py`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.2/pocketrockit/decorated.py` & `pocketrockit-0.0.3/pocketrockit/decorated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python3
 
 """API for fancy decorator based track definitions"""
 
 from collections.abc import Sequence
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from itertools import count
 
 from .engine import run
 
 
 @dataclass
 class Env:
+    """Some global environment"""
     bpm: int = 60
 
 
 @dataclass
 class Singleton:
-    env: Env = Env()
+    """Not yet a Singleton - access to the currently played music"""
+    env: Env = field(default_factory=Env)
     active: bool = False
     players: None | list = None
     new_track: None | list = None
     file_to_track: None | str = None
     tick: int = 0
```

### Comparing `pocketrockit-0.0.2/pocketrockit/engine.py` & `pocketrockit-0.0.3/pocketrockit/engine.py`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.2/pyproject.toml` & `pocketrockit-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pocketrockit"
-version = "0.0.2"
+version = "0.0.3"
 description = "pocketrockit"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/pocketrockit.git"
 readme = "Readme.md"
 packages = [
   {include = "pocketrockit"}
 ]
```

### Comparing `pocketrockit-0.0.2/PKG-INFO` & `pocketrockit-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketrockit
-Version: 0.0.2
+Version: 0.0.3
 Summary: pocketrockit
 Home-page: https://projects.om-office.de/frans/pocketrockit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

