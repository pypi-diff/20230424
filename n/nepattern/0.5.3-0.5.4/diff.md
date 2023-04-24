# Comparing `tmp/nepattern-0.5.3.tar.gz` & `tmp/nepattern-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.5.3.tar", last modified: Mon Apr 17 06:24:33 2023, max compression
+gzip compressed data, was "nepattern-0.5.4.tar", last modified: Mon Apr 24 13:41:55 2023, max compression
```

## Comparing `nepattern-0.5.3.tar` & `nepattern-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.3/LICENSE
--rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.3/nepattern/__init__.py
--rw-r--r--   0        0        0     8644 2023-04-17 06:05:25.544604 nepattern-0.5.3/nepattern/base.py
--rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.3/nepattern/context.py
--rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.3/nepattern/context.pyi
--rw-r--r--   0        0        0    14689 2023-04-17 06:05:25.471903 nepattern-0.5.3/nepattern/core.py
--rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.3/nepattern/exception.py
--rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.3/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.3/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.3/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0    10183 2023-04-17 06:15:54.768610 nepattern-0.5.3/nepattern/main.py
--rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.3/nepattern/util.py
--rw-r--r--   0        0        0     1738 2023-04-17 05:50:23.807298 nepattern-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.3/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.4/LICENSE
+-rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.4/nepattern/__init__.py
+-rw-r--r--   0        0        0     8885 2023-04-24 13:27:27.344009 nepattern-0.5.4/nepattern/base.py
+-rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.4/nepattern/context.py
+-rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.4/nepattern/context.pyi
+-rw-r--r--   0        0        0    15361 2023-04-24 13:27:05.487874 nepattern-0.5.4/nepattern/core.py
+-rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.4/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.4/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.4/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.4/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0    10183 2023-04-17 06:15:54.768610 nepattern-0.5.4/nepattern/main.py
+-rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.4/nepattern/util.py
+-rw-r--r--   0        0        0     1738 2023-04-24 13:15:20.006654 nepattern-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.4/README.md
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.4/PKG-INFO
```

### Comparing `nepattern-0.5.3/LICENSE` & `nepattern-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/nepattern/__init__.py` & `nepattern-0.5.4/nepattern/__init__.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/nepattern/base.py` & `nepattern-0.5.4/nepattern/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from __future__ import annotations
 
 import re
-from typing import Iterable, Any, Literal, TypeVar, Dict, Union
+from typing import Any, Dict, Iterable, Literal, TypeVar, Union
+
 from tarina import Empty
 from tarina.lang import lang
 
 from .core import BasePattern, MatchMode
 from .exception import MatchFailed
 
 
 class RegexPattern(BasePattern[Union[dict, tuple]]):
     """针对正则的特化匹配，支持正则组"""
 
     def __init__(self, pattern: str, alias: str | None = None):
-        super().__init__(pattern, origin=Union[dict, tuple], alias=alias or 'regex[:group]')  # type: ignore
+        super().__init__(pattern, origin=Union[dict, tuple], alias=alias or "regex[:group]")  # type: ignore
 
     def match(self, input_: str | Any):
         if not isinstance(input_, str):
-            raise MatchFailed(lang.nepattern.type_error.format(target=input_))
+            raise MatchFailed(
+                lang.require("nepattern", "type_error").format(target=input_)
+            )
         if mat := self.regex_pattern.match(input_):
             return mat.groupdict() or mat.groups()
-        raise MatchFailed(lang.nepattern.content_error.format(target=input_))
+        raise MatchFailed(
+            lang.require("nepattern", "content_error").format(target=input_)
+        )
 
 
 class UnionPattern(BasePattern):
     """多类型参数的匹配"""
 
     optional: bool
     base: list[BasePattern | object | str]
@@ -44,26 +49,26 @@
             elif isinstance(arg, BasePattern):
                 self.for_validate.append(arg)
             else:
                 self.for_equal.append(arg)
         alias_content = "|".join(
             [repr(a) for a in self.for_validate] + [repr(a) for a in self.for_equal]
         )
-        super().__init__(
-            r"(.+?)", MatchMode.KEEP, str, alias=alias_content, anti=anti
-        )
+        super().__init__(r"(.+?)", MatchMode.KEEP, str, alias=alias_content, anti=anti)
 
     def match(self, text: str | Any):
         if not text:
             text = None
         if text not in self.for_equal:
             for pat in self.for_validate:
                 if (res := pat.validate(text)).success:
                     return res.value
-            raise MatchFailed(lang.nepattern.content_error.format(target=text))
+            raise MatchFailed(
+                lang.require("nepattern", "content_error").format(target=text)
+            )
         return text
 
     def __repr__(self):
         return ("!" if self.anti else "") + (
             "|".join(repr(a) for a in (*self.for_validate, *self.for_equal))
         )
 
@@ -113,33 +118,37 @@
                 r"\((.+?)\)", MatchMode.REGEX_MATCH, form, alias=f"tuple[{base}]"
             )
         elif form is set:
             super().__init__(
                 r"\{(.+?)\}", MatchMode.REGEX_MATCH, form, alias=f"set[{base}]"
             )
         else:
-            raise ValueError(lang.nepattern.sequence_form_error.format(target=str(form)))
+            raise ValueError(
+                lang.require("nepattern", "sequence_form_error").format(
+                    target=str(form)
+                )
+            )
 
     def match(self, text: str | Any):
         _res = super().match(text)
         _max = 0
         success: list[tuple[int, Any]] = []
         fail: list[tuple[int, MatchFailed]] = []
         for _max, s in enumerate(
-                re.split(r"\s*,\s*", _res) if isinstance(_res, str) else _res
+            re.split(r"\s*,\s*", _res) if isinstance(_res, str) else _res
         ):
             try:
                 success.append((_max, self.base.match(s)))
             except MatchFailed:
                 fail.append((_max, MatchFailed(f"{s} is not matched with {self.base}")))
 
         if (
-                (self._mode == "all" and fail)
-                or (self._mode == "pre" and fail and fail[0][0] == 0)
-                or (self._mode == "suf" and fail and fail[-1][0] == _max)
+            (self._mode == "all" and fail)
+            or (self._mode == "pre" and fail and fail[0][0] == 0)
+            or (self._mode == "suf" and fail and fail[-1][0] == _max)
         ):
             raise fail[0][1]
         if self._mode == "pre" and fail:
             return self.origin(i[1] for i in success if i[0] < fail[0][0])
         if self._mode == "suf" and fail:
             return self.origin(i[1] for i in success if i[0] > fail[-1][0])
         return self.origin(i[1] for i in success)
@@ -201,17 +210,17 @@
                         _max,
                         MatchFailed(
                             f"{k}: {v} is not matched with {self.key}: {self.value}"
                         ),
                     )
                 )
         if (
-                (self._mode == "all" and fail)
-                or (self._mode == "pre" and fail and fail[0][0] == 0)
-                or (self._mode == "suf" and fail and fail[-1][0] == _max)
+            (self._mode == "all" and fail)
+            or (self._mode == "pre" and fail and fail[0][0] == 0)
+            or (self._mode == "suf" and fail and fail[-1][0] == _max)
         ):
             raise fail[0][1]
         if self._mode == "pre" and fail:
             return {i[1]: i[2] for i in success if i[0] < fail[0][0]}
         if self._mode == "suf" and fail:
             return {i[1]: i[2] for i in success if i[0] > fail[-1][0]}
         return {i[1]: i[2] for i in success}
@@ -243,11 +252,19 @@
 
     def match(self, input_: Any) -> _TCase:
         try:
             return self.switch[input_]
         except KeyError as e:
             if Ellipsis in self.switch:
                 return self.switch[...]
-            raise MatchFailed(lang.nepattern.content_error.format(target=input_)) from e
+            raise MatchFailed(
+                lang.require("nepattern", "content_error").format(target=input_)
+            ) from e
 
 
-__all__ = ["RegexPattern", "UnionPattern", "SequencePattern", "MappingPattern", "SwitchPattern"]
+__all__ = [
+    "RegexPattern",
+    "UnionPattern",
+    "SequencePattern",
+    "MappingPattern",
+    "SwitchPattern",
+]
```

### Comparing `nepattern-0.5.3/nepattern/context.py` & `nepattern-0.5.4/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/nepattern/context.pyi` & `nepattern-0.5.4/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/nepattern/core.py` & `nepattern-0.5.4/nepattern/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from __future__ import annotations
 
 import re
-from enum import IntEnum, Enum
 from copy import deepcopy
-from typing import (
-    TypeVar,
-    Callable,
-    Any,
-    Generic,
-    overload,
-)
 from dataclasses import dataclass, field
+from enum import Enum, IntEnum
+from typing import Any, Callable, Generic, TypeVar, overload
+
 from tarina import Empty, generic_isinstance
 from tarina.lang import lang
 
 try:
     from typing import Annotated, Self, get_origin  # type: ignore
 except ImportError:
     from typing_extensions import Annotated, Self, get_origin
@@ -71,15 +66,14 @@
 
     @property
     def value(self) -> TVOrigin:
         if self.flag == ResultFlag.ERROR or self._value == Empty:
             raise RuntimeError("cannot access value")
         return self._value  # type: ignore
 
-
     @property
     def error(self) -> Exception | None:
         if self.flag == ResultFlag.ERROR and self._error != Empty:
             assert isinstance(self._error, Exception)
             return self._error
 
     @property
@@ -114,15 +108,15 @@
         if callable(other) and self.success:
             return other(self.value)
         if self.success and hasattr(self.value, "__rshift__"):
             return self.value | other  # type: ignore
         return self
 
     @overload
-    def __rshift__(self, other: type[T]| T) -> T:
+    def __rshift__(self, other: type[T] | T) -> T:
         ...
 
     @overload
     def __rshift__(self, other: Callable[[TVOrigin], T]) -> T | Self:
         ...
 
     @overload
@@ -180,15 +174,19 @@
         validators: list[Callable[[TOrigin], bool]] | None = None,
         anti: bool = False,
     ):
         """
         初始化参数匹配表达式
         """
         if pattern.startswith("^") or pattern.endswith("$"):
-            raise ValueError(lang.nepattern.pattern_head_or_tail_error.format(target=pattern))
+            raise ValueError(
+                lang.require("nepattern", "pattern_head_or_tail_error").format(
+                    target=pattern
+                )
+            )
         self.pattern = pattern
         self.regex_pattern = re.compile(f"^{pattern}$")
         self.mode = MatchMode(model)
         self.origin = origin
         self.alias = alias
         self.previous = previous
         accepts = accepts or []
@@ -207,16 +205,20 @@
         self.anti = anti
 
     def __repr__(self):
         if self.mode == MatchMode.KEEP:
             if self.alias:
                 return self.alias
             return (
-                "Any" if not self.type_accepts and not self.pattern_accepts else
-                "|".join([x.__name__ for x in self.type_accepts] + [x.__repr__() for x in self.pattern_accepts])
+                "Any"
+                if not self.type_accepts and not self.pattern_accepts
+                else "|".join(
+                    [x.__name__ for x in self.type_accepts]
+                    + [x.__repr__() for x in self.pattern_accepts]
+                )
             )
 
         if not self.alias:
             name = getattr(self.origin, "__name__", str(self.origin))
             if self.mode == MatchMode.REGEX_MATCH:
                 text = self.pattern
             elif self.mode == MatchMode.REGEX_CONVERT or (
@@ -306,76 +308,97 @@
             input_, self.pattern_accepts, self.type_accepts
         ):
             if not self.previous or not _accept(
                 input_ := self.previous.match(input_),
                 self.pattern_accepts,
                 self.type_accepts,
             ):  # pragma: no cover
-                raise MatchFailed(lang.nepattern.type_error.format(target=input_.__class__))
+                raise MatchFailed(
+                    lang.require("nepattern", "type_error").format(
+                        target=input_.__class__
+                    )
+                )
         if self.mode == MatchMode.KEEP:
             return input_  # type: ignore
         if self.mode == MatchMode.TYPE_CONVERT:
             res = self.converter(self, input_)
             if res is None and self.origin == Any:  # pragma: no cover
-                raise MatchFailed(lang.nepattern.content_error.format(target=input_))
+                raise MatchFailed(
+                    lang.require("nepattern", "content_error").format(target=input_)
+                )
             if not generic_isinstance(res, self.origin):
                 if not self.previous or not generic_isinstance(
-                    res := self.converter(self, self.previous.match(input_)), self.origin
+                    res := self.converter(self, self.previous.match(input_)),
+                    self.origin,
                 ):
-                    raise MatchFailed(lang.nepattern.content_error.format(target=input_))
+                    raise MatchFailed(
+                        lang.require("nepattern", "content_error").format(target=input_)
+                    )
             return res
         if not isinstance(input_, str):
             if not self.previous or not isinstance(
                 input_ := self.previous.match(input_), str
             ):
-                raise MatchFailed(lang.nepattern.type_error.format(target=type(input_)))
+                raise MatchFailed(
+                    lang.require("nepattern", "type_error").format(target=type(input_))
+                )
         if mat := self.regex_pattern.match(input_):
             glen = len(mat.groups())
             return (
                 self.converter(self, mat[1] if glen > 0 else mat[0])
                 if self.mode == MatchMode.REGEX_CONVERT
-                else mat[1] if glen > 0 else mat[0]
+                else mat[1]
+                if glen > 0
+                else mat[0]
             )
-        raise MatchFailed(lang.nepattern.content_error.format(target=input_))
+        raise MatchFailed(
+            lang.require("nepattern", "content_error").format(target=input_)
+        )
 
     @overload
     def validate(self, input_: Any) -> ValidateResult[TOrigin]:
         ...
 
     @overload
-    def validate(self, input_: Any, default: TDefault) -> ValidateResult[TOrigin | TDefault]:
+    def validate(
+        self, input_: Any, default: TDefault
+    ) -> ValidateResult[TOrigin | TDefault]:
         ...
 
     def validate(  # type: ignore
         self, input_: Any, default: TDefault | None = None
     ) -> ValidateResult[TOrigin | TDefault]:
         """
         对传入的值进行正向验证，返回可能的匹配与转化结果。
 
         若传入默认值，验证失败会返回默认值
         """
         try:
             res = self.match(input_)
             for i in self.validators:
                 if not i(res):
-                    raise MatchFailed(lang.nepattern.content_error.format(target=input_))
+                    raise MatchFailed(
+                        lang.require("nepattern", "content_error").format(target=input_)
+                    )
             return ValidateResult(_value=res, flag=ResultFlag.VALID)
         except Exception as e:
             if default is None:
                 return ValidateResult(_error=e, flag=ResultFlag.ERROR)
             return ValidateResult(
                 _value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
             )
 
     @overload
     def invalidate(self, input_: Any) -> ValidateResult[Any]:
         ...
 
     @overload
-    def invalidate(self, input_: Any, default: TDefault) -> ValidateResult[Any | TDefault]:
+    def invalidate(
+        self, input_: Any, default: TDefault
+    ) -> ValidateResult[Any | TDefault]:
         ...
 
     def invalidate(
         self, input_: Any, default: TDefault | None = None
     ) -> ValidateResult[Any | TDefault]:
         """
         对传入的值进行反向验证，返回可能的匹配与转化结果。
@@ -388,29 +411,33 @@
             return ValidateResult(_value=input_, flag=ResultFlag.VALID)
         else:
             for i in self.validators:
                 if not i(res):
                     return ValidateResult(_value=input_, flag=ResultFlag.VALID)
             if default is None:
                 return ValidateResult(
-                    _error=MatchFailed(lang.nepattern.content_error.format(target=input_)),
+                    _error=MatchFailed(
+                        lang.require("nepattern", "content_error").format(target=input_)
+                    ),
                     flag=ResultFlag.ERROR,
                 )
             return ValidateResult(
                 _value=None if default is Empty else default, flag=ResultFlag.DEFAULT
             )
 
-
     @overload
     def __call__(self, input_: Any) -> ValidateResult[TOrigin]:
         ...
 
     @overload
-    def __call__(self, input_: Any, default: TDefault) -> ValidateResult[TOrigin | TDefault]:
+    def __call__(
+        self, input_: Any, default: TDefault
+    ) -> ValidateResult[TOrigin | TDefault]:
         ...
+
     def __call__(self, input_: Any, default: TDefault | None = None) -> ValidateResult[TOrigin | TDefault | None]:  # type: ignore
         """
         依据 anti 值 自动选择验证方式
         """
         if self.anti:
             return self.invalidate(input_, default)
         else:
```

### Comparing `nepattern-0.5.3/nepattern/main.py` & `nepattern-0.5.4/nepattern/main.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/nepattern/util.py` & `nepattern-0.5.4/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/pyproject.toml` & `nepattern-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nepattern"
-version = "0.5.3"
+version = "0.5.4"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "tarina>=0.3.0",
+    "tarina>=0.3.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "typing",
     "pattern",
     "converter",
```

### Comparing `nepattern-0.5.3/README.md` & `nepattern-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.3/PKG-INFO` & `nepattern-0.5.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.5.3
+Version: 0.5.4
 Summary: a complex pattern, support typing
 License: MIT
 Keywords: typing,pattern,converter,validator
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

