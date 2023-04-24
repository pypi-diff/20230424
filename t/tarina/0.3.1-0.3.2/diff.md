# Comparing `tmp/tarina-0.3.1.tar.gz` & `tmp/tarina-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.3.1.tar", last modified: Sun Apr 23 14:34:17 2023, max compression
+gzip compressed data, was "tarina-0.3.2.tar", last modified: Mon Apr 24 12:59:09 2023, max compression
```

## Comparing `tarina-0.3.1.tar` & `tarina-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-23 14:33:58.000000 tarina-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 14:33:58.000000 tarina-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-23 14:34:17.126438 tarina-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 14:33:58.000000 tarina-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-23 14:33:58.000000 tarina-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 14:34:17.126438 tarina-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-23 14:33:58.000000 tarina-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.122438 tarina-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_op.h
--rw-r--r--   0 runner    (1001) docker     (123)   193906 2023-04-23 14:34:08.000000 tarina-0.3.1/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/guard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/src/tarina/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/i18n/.config.json
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/i18n/en-US.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/i18n/zh-CN.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-23 14:33:58.000000 tarina-0.3.1/src/tarina/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 14:34:17.126438 tarina-0.3.1/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 14:34:17.000000 tarina-0.3.1/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:09.263594 tarina-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 12:58:46.000000 tarina-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-24 12:58:46.000000 tarina-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 12:59:09.263594 tarina-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 12:58:46.000000 tarina-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 12:58:46.000000 tarina-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:59:09.263594 tarina-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 12:58:46.000000 tarina-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:09.259593 tarina-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:09.263594 tarina-0.3.2/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24132 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (123)   193906 2023-04-24 12:58:56.000000 tarina-0.3.2/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/guard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:09.263594 tarina-0.3.2/src/tarina/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/i18n/.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/i18n/en-US.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/i18n/zh-CN.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-24 12:58:46.000000 tarina-0.3.2/src/tarina/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:59:09.263594 tarina-0.3.2/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 12:59:09.000000 tarina-0.3.2/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-24 12:59:09.000000 tarina-0.3.2/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:59:09.000000 tarina-0.3.2/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 12:59:09.000000 tarina-0.3.2/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 12:59:09.000000 tarina-0.3.2/src/tarina.egg-info/top_level.txt
```

### Comparing `tarina-0.3.1/LICENSE` & `tarina-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/PKG-INFO` & `tarina-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.3.1/pyproject.toml` & `tarina-0.3.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tarina"
-version = "0.3.1"
+version = "0.3.2"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
```

### Comparing `tarina-0.3.1/setup.py` & `tarina-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_lru_c.c` & `tarina-0.3.2/src/tarina/_lru_c.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+/*
+
+Copyright (c) Amit Dev R
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+*/
+
 #include <Python.h>
 
 /*
  * This is a simple implementation of LRU Dict that uses a Python dict and an associated doubly linked
  * list to keep track of recently inserted/accessed items.
  *
  * Dict will store: key -> Node mapping, where Node is a linked list node.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tarina-0.3.1/src/tarina/_lru_c.pyi` & `tarina-0.3.2/src/tarina/_lru_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_lru_py.py` & `tarina-0.3.2/src/tarina/_lru_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_op.h` & `tarina-0.3.2/src/tarina/_op.h`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_string_c.c` & `tarina-0.3.2/src/tarina/_string_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_string_c.pyi` & `tarina-0.3.2/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_string_c.pyx` & `tarina-0.3.2/src/tarina/_string_c.pyx`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/_string_py.py` & `tarina-0.3.2/src/tarina/_string_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/context.py` & `tarina-0.3.2/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/generic.py` & `tarina-0.3.2/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/guard.py` & `tarina-0.3.2/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/lang.py` & `tarina-0.3.2/src/tarina/lang.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,58 @@
 from __future__ import annotations
-from typing import Final, final, Any
-from typing_extensions import Self
+from typing import Final, final, Any, TypedDict
+from typing_extensions import Self, NotRequired
 from pathlib import Path
 import json
+import locale
+import sys
 
 root_dir: Final[Path] = Path(__file__).parent / "i18n"
+WINDOWS = sys.platform.startswith("win") or (sys.platform == "cli" and os.name == "nt")
+
+
+class _LangDict(TypedDict):
+    default: NotRequired[str]
+    frozen: NotRequired[list[str]]
+    require: NotRequired[list[str]]
+
+
+def _get_win_locale_with_ctypes() -> str | None:
+    import ctypes
+
+    kernel32 = ctypes.windll.kernel32
+    lcid: int = kernel32.GetUserDefaultUILanguage()
+    return locale.windows_locale.get(lcid)
+
+
+def _get_win_locale_from_registry() -> str | None:
+    import winreg
+
+    with contextlib.suppress(Exception):
+        with winreg.OpenKey(
+            winreg.HKEY_CURRENT_USER, r"Control Panel\International"
+        ) as key:
+            if lcid := winreg.QueryValueEx(key, "Locale")[0]:
+                return locale.windows_locale.get(int(lcid, 16))
+
+
+if WINDOWS:
+    try:
+        import ctypes
+
+        _get_win_locale = _get_win_locale_with_ctypes
+    except ImportError:
+        _get_win_locale = _get_win_locale_from_registry
+
+
+def get_locale() -> str | None:
+    if WINDOWS:
+        return _get_win_locale()
+
+    return locale.getlocale(locale.LC_MESSAGES)[0]
 
 
 def _get_config(root: Path) -> dict[str, Any]:
     if not (root / ".config.json").exists():
         return {}
     with (root / ".config.json").open("r", encoding="utf-8") as f:
         return json.load(f)
@@ -42,88 +86,84 @@
 @final
 class _LangConfig:
     def __init__(self):
         __config = _get_config(root_dir)
         self.__scope: str = __config["default"]
         self.__frozen: list[str] = __config["frozen"]
         self.__require: list[str] = __config["require"]
-        self.__scopes = _get_scopes(root_dir)
-        self.__langs = {t: _get_lang(root_dir, t) for t in self.__scopes}
+        self.__langs = {t.replace("_", "-"): _get_lang(root_dir, t) for t in _get_scopes(root_dir)}
+        self.__scopes = set(self.__langs.keys())
+        self.select_local()
 
     @property
     def scopes(self):
         return self.__scopes
 
-    def scope(self, item: str) -> Self:
+    @property
+    def current(self):
+        return self.__scope
+
+    def select_local(self):
+        """
+        依据系统语言尝试自动选择语言
+        """
+        if (lc := get_locale()) and lc.replace("_", "-") in self.__langs:
+            self.__scope = lc.replace("_", "-")
+        return self
+
+    def select(self, item: str) -> Self:
+        item = item.replace("_", "-")
         if item not in self.__langs:
             raise ValueError(self.require("lang", "scope_error").format(target=item))
         self.__scope = item
         return self
 
     def save(self, root: Path | None = None):
         _root = root or root_dir
         config = _get_config(_root)
         config["default"] = self.__scope
         with (_root / ".config.json").open("w+", encoding="utf-8") as f:
             json.dump(config, f, ensure_ascii=False, indent=2)
 
-    def __getattr__(self, item: str):
-        _lang = self.__langs[self.__scope]
-        if item not in _lang:
-            raise ValueError(
-                _lang["lang"]["type_error"].format(target=item, scope=self.__scope)
-            )
-
-        class _getter:
-            def __init__(_self, prefix: str):
-                _self.prefix = prefix
-
-        def __getattr__(_self, _item: str):
-            _config = _lang[_self.prefix]
-            if not _config.get(_item):
-                raise AttributeError(
-                    _lang["lang"]["name_error"].format(
-                        target=_item, scope=self.__scope, type=_self.prefix
-                    )
-                )
-            return _config[_item]
-
-        return type(
-            f"{self.__scope}_{item}_getter", (_getter,), {"__getattr__": __getattr__}
-        )(item)
-
-    def load_file(self, filepath: Path):
-        _type = filepath.stem
-        if _type in self.__scopes:
-            self.__langs[_type] = merge(
-                _get_lang(filepath.parent, _type), self.__langs[_type], self.__frozen
+    def load_data(self, scope: str, data: dict[str, dict[str, str]]):
+        if scope in self.__langs:
+            self.__langs[scope] = merge(
+                data, self.__langs[scope], self.__frozen
             )
         else:
-            self.__scopes.append(_type)
-            self.__langs[_type] = _get_lang(filepath.parent, _type)
+            self.__scopes.add(scope)
+            self.__langs[scope] = data
         for key in self.__require:
-            t, n = key.split(".", 1)
-            if t not in self.__langs[_type]:
+            parts = key.split(".", 1)
+            t = parts[0]
+            n = parts[1] if len(parts) > 1 else None
+            if t not in self.__langs[scope]:
                 raise KeyError(
-                    self.require("lang", "miss_require_type", _type).format(
-                        scope=_type, target=t
+                    self.require("lang", "miss_require_type", scope).format(
+                        scope=scope, target=t
                     )
                 )
-            if n and n not in self.__langs[_type][t]:
+            if n and n not in self.__langs[scope][t]:
                 raise KeyError(
-                    self.require("lang", "miss_require_name", _type).format(
-                        scope=_type, type=t, target=n
+                    self.require("lang", "miss_require_name", scope).format(
+                        scope=scope, type=t, target=n
                     )
                 )
 
-    def load(self, root: Path):
-        config = _get_config(root)
+    def load_file(self, filepath: Path):
+        return self.load_data(filepath.stem, _get_lang(filepath.parent, filepath.stem))
+
+    def load_config(self, config: _LangDict):
         self.__scope = config.get("default", self.__scope)
         self.__frozen.extend(config.get("frozen", []))
         self.__require.extend(config.get("require", []))
+        self.select_local()
+
+    def load(self, root: Path):
+        self.load_config(_get_config(root))
         for i in root.iterdir():
             if i.is_file() and not i.name.startswith("."):
                 continue
             self.load_file(i)
 
     def require(self, _type: str, _name: str, scope: str | None = None) -> str:
         scope = scope or self.__scope
@@ -131,24 +171,28 @@
             raise ValueError(
                 self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope)
             )
         if _type in self.__langs[scope]:
             _types = self.__langs[scope][_type]
         elif _type in self.__langs[self.__scope]:
             _types = self.__langs[self.__scope][_type]
+        elif _type in self.__langs[(default := _get_config(root_dir)["default"])]:
+            _types = self.__langs[default][_type]
         else:
             raise ValueError(
                 self.__langs[scope]["lang"]["type_error"].format(
                     target=_type, scope=scope
                 )
             )
         if _name in _types:
             return _types[_name]
         elif _name in self.__langs[self.__scope][_type]:
             return self.__langs[self.__scope][_type][_name]
+        elif _name in self.__langs[(default := _get_config(root_dir)["default"])][_type]:
+            return self.__langs[default][_type][_name]
         else:
             raise ValueError(
                 self.__langs[scope]["lang"]["name_error"].format(
                     target=_name, scope=scope, type=_type
                 )
             )
 
@@ -169,17 +213,7 @@
     def __repr__(self):
         return f"<LangConfig: {self.__scope}>"
 
 
 lang: _LangConfig = _LangConfig()
 
 __all__ = ["lang"]
-
-if __name__ == "__main__":
-    print(lang.scopes)
-    print(lang.lang.name_error)
-    print(lang.require("lang", "name_error"))
-    print(lang.require("lang", "name_error", "en-US"))
-    print(lang.scope("en-US"))
-    print(lang.lang.name_error)
-    print(lang.lang.type_error)
-    print(lang.lang.scope_error)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tarina-0.3.1/src/tarina/lru.pyi` & `tarina-0.3.2/src/tarina/lru.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/signature.py` & `tarina-0.3.2/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/string.py` & `tarina-0.3.2/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina/tools.py` & `tarina-0.3.2/src/tarina/tools.py`

 * *Files identical despite different names*

### Comparing `tarina-0.3.1/src/tarina.egg-info/PKG-INFO` & `tarina-0.3.2/src/tarina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.3.1/src/tarina.egg-info/SOURCES.txt` & `tarina-0.3.2/src/tarina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

